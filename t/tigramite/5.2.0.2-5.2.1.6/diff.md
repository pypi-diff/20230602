# Comparing `tmp/tigramite-5.2.0.2.tar.gz` & `tmp/tigramite-5.2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tigramite-5.2.0.2.tar", last modified: Fri Apr 14 15:04:51 2023, max compression
+gzip compressed data, was "tigramite-5.2.1.6.tar", last modified: Fri Jun  2 16:50:51 2023, max compression
```

## Comparing `tigramite-5.2.0.2.tar` & `tigramite-5.2.1.6.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-04-14 15:04:51.185576 tigramite-5.2.0.2/
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     8784 2023-04-14 15:04:51.185576 tigramite-5.2.0.2/PKG-INFO
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     8006 2023-04-14 15:04:40.000000 tigramite-5.2.0.2/README.md
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)       79 2023-04-14 15:04:51.185576 tigramite-5.2.0.2/setup.cfg
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     3100 2023-04-14 15:04:40.000000 tigramite-5.2.0.2/setup.py
-drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-04-14 15:04:51.181576 tigramite-5.2.0.2/tests/
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     5485 2023-04-14 15:04:40.000000 tigramite-5.2.0.2/tests/test_construct_array.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    38249 2023-04-14 15:04:40.000000 tigramite-5.2.0.2/tests/test_independence_tests.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     3894 2023-04-14 15:04:40.000000 tigramite-5.2.0.2/tests/test_models.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    26762 2023-04-14 15:04:40.000000 tigramite-5.2.0.2/tests/test_pcmci_calculations.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    17546 2023-04-14 15:04:40.000000 tigramite-5.2.0.2/tests/test_pcmci_construction.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    13375 2023-04-14 15:04:40.000000 tigramite-5.2.0.2/tests/test_var_process.py
-drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-04-14 15:04:51.181576 tigramite-5.2.0.2/tigramite/
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-04-14 15:04:40.000000 tigramite-5.2.0.2/tigramite/__init__.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)   102754 2023-04-14 15:04:40.000000 tigramite-5.2.0.2/tigramite/causal_effects.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    65894 2023-04-14 15:04:40.000000 tigramite-5.2.0.2/tigramite/data_processing.py
-drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-04-14 15:04:51.185576 tigramite-5.2.0.2/tigramite/independence_tests/
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    43660 2023-04-14 15:04:40.000000 tigramite-5.2.0.2/tigramite/independence_tests/LBFGS.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-04-14 15:04:40.000000 tigramite-5.2.0.2/tigramite/independence_tests/__init__.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    17887 2023-04-14 15:04:40.000000 tigramite-5.2.0.2/tigramite/independence_tests/cmiknn.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    10370 2023-04-14 15:04:40.000000 tigramite-5.2.0.2/tigramite/independence_tests/cmisymb.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    23994 2023-04-14 15:04:40.000000 tigramite-5.2.0.2/tigramite/independence_tests/gpdc.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    31190 2023-04-14 15:04:40.000000 tigramite-5.2.0.2/tigramite/independence_tests/gpdc_torch.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     6459 2023-04-14 15:04:40.000000 tigramite-5.2.0.2/tigramite/independence_tests/gsquared.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    41968 2023-04-14 15:04:40.000000 tigramite-5.2.0.2/tigramite/independence_tests/independence_tests_base.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    62833 2023-04-14 15:04:40.000000 tigramite-5.2.0.2/tigramite/independence_tests/oracle_conditional_independence.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     9979 2023-04-14 15:04:40.000000 tigramite-5.2.0.2/tigramite/independence_tests/parcorr.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    12267 2023-04-14 15:04:40.000000 tigramite-5.2.0.2/tigramite/independence_tests/parcorr_mult.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    17975 2023-04-14 15:04:40.000000 tigramite-5.2.0.2/tigramite/independence_tests/parcorr_wls.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    13647 2023-04-14 15:04:40.000000 tigramite-5.2.0.2/tigramite/independence_tests/regressionCI.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    13402 2023-04-14 15:04:40.000000 tigramite-5.2.0.2/tigramite/independence_tests/robust_parcorr.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)   170545 2023-04-14 15:04:40.000000 tigramite-5.2.0.2/tigramite/lpcmci.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    75920 2023-04-14 15:04:40.000000 tigramite-5.2.0.2/tigramite/models.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)   171329 2023-04-14 15:04:40.000000 tigramite-5.2.0.2/tigramite/pcmci.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    46472 2023-04-14 15:04:40.000000 tigramite-5.2.0.2/tigramite/pcmci_base.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)   159892 2023-04-14 15:04:40.000000 tigramite-5.2.0.2/tigramite/plotting.py
-drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-04-14 15:04:51.185576 tigramite-5.2.0.2/tigramite/toymodels/
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-04-14 15:04:40.000000 tigramite-5.2.0.2/tigramite/toymodels/__init__.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    41858 2023-04-14 15:04:40.000000 tigramite-5.2.0.2/tigramite/toymodels/structural_causal_processes.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    12722 2023-04-14 15:04:40.000000 tigramite-5.2.0.2/tigramite/toymodels/surrogate_generator.py
-drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-04-14 15:04:51.181576 tigramite-5.2.0.2/tigramite.egg-info/
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     8784 2023-04-14 15:04:51.000000 tigramite-5.2.0.2/tigramite.egg-info/PKG-INFO
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     1298 2023-04-14 15:04:51.000000 tigramite-5.2.0.2/tigramite.egg-info/SOURCES.txt
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)        1 2023-04-14 15:04:51.000000 tigramite-5.2.0.2/tigramite.egg-info/dependency_links.txt
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)      402 2023-04-14 15:04:51.000000 tigramite-5.2.0.2/tigramite.egg-info/requires.txt
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)       10 2023-04-14 15:04:51.000000 tigramite-5.2.0.2/tigramite.egg-info/top_level.txt
+drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-06-02 16:50:51.774601 tigramite-5.2.1.6/
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     8784 2023-06-02 16:50:51.774601 tigramite-5.2.1.6/PKG-INFO
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     8006 2023-06-02 16:50:38.000000 tigramite-5.2.1.6/README.md
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)       79 2023-06-02 16:50:51.774601 tigramite-5.2.1.6/setup.cfg
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     3150 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/setup.py
+drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-06-02 16:50:51.766601 tigramite-5.2.1.6/tests/
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     5485 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tests/test_construct_array.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    38249 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tests/test_independence_tests.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     3894 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tests/test_models.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    26762 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tests/test_pcmci_calculations.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    17546 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tests/test_pcmci_construction.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    13375 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tests/test_var_process.py
+drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-06-02 16:50:51.770601 tigramite-5.2.1.6/tigramite/
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/__init__.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)   103626 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/causal_effects.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    65916 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/data_processing.py
+drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-06-02 16:50:51.774601 tigramite-5.2.1.6/tigramite/independence_tests/
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    43660 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/independence_tests/LBFGS.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/independence_tests/__init__.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    17895 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/independence_tests/cmiknn.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    10905 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/independence_tests/cmisymb.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    23994 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/independence_tests/gpdc.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    31189 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/independence_tests/gpdc_torch.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     6459 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/independence_tests/gsquared.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    41951 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/independence_tests/independence_tests_base.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    62833 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/independence_tests/oracle_conditional_independence.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     9979 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/independence_tests/parcorr.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    12267 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/independence_tests/parcorr_mult.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    17975 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/independence_tests/parcorr_wls.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    13647 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/independence_tests/regressionCI.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    13402 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/independence_tests/robust_parcorr.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)   170551 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/lpcmci.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    77764 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/models.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)   169431 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/pcmci.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    41334 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/pcmci_base.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)   164901 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/plotting.py
+drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-06-02 16:50:51.774601 tigramite-5.2.1.6/tigramite/toymodels/
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/toymodels/__init__.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    41858 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/toymodels/structural_causal_processes.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    12722 2023-06-02 16:50:39.000000 tigramite-5.2.1.6/tigramite/toymodels/surrogate_generator.py
+drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-06-02 16:50:51.770601 tigramite-5.2.1.6/tigramite.egg-info/
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     8784 2023-06-02 16:50:51.000000 tigramite-5.2.1.6/tigramite.egg-info/PKG-INFO
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     1298 2023-06-02 16:50:51.000000 tigramite-5.2.1.6/tigramite.egg-info/SOURCES.txt
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)        1 2023-06-02 16:50:51.000000 tigramite-5.2.1.6/tigramite.egg-info/dependency_links.txt
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)      428 2023-06-02 16:50:51.000000 tigramite-5.2.1.6/tigramite.egg-info/requires.txt
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)       10 2023-06-02 16:50:51.000000 tigramite-5.2.1.6/tigramite.egg-info/top_level.txt
```

### Comparing `tigramite-5.2.0.2/PKG-INFO` & `tigramite-5.2.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigramite
-Version: 5.2.0.2
+Version: 5.2.1.6
 Summary: Tigramite causal inference for time series
 Home-page: https://github.com/jakobrunge/tigramite/
 Author: Jakob Runge
 Author-email: jakob@jakob-runge.com
 License: GNU General Public License v3.0
 Keywords: causal inference,causal discovery,prediction,time series
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tigramite-5.2.0.2/README.md` & `tigramite-5.2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.2/setup.py` & `tigramite-5.2.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,16 @@
         "scikit-learn>=1.2",  # Gaussian Process (GP) Regression
         "matplotlib>=3.7.0",  # plotting
         "seaborn>=0.12.2",    # plotting
         "networkx>=3.0",      # plotting
         "pytorch>=1.13.1",    # GPDC torch version
         "gpytorch>=1.9.1",    # GPDC gpytorch version
         "dcor>=0.6",          # GPDC distance correlation version
-        "joblib>=1.2.0",      # CMIsymb shuffle parallelization
+        "joblib>=1.2.0",      # CMIsymb shuffle parallelization and others
+        "ortools>=9.2",       # RPCMCI
     ]
 }
 
 # Define the packages needed for testing
 TESTS_REQUIRE = ["nose", "pytest", "networkx>=3.0", "scikit-learn>=1.2",
                  "pytorch>=1.13.1", "gpytorch>=1.9.1", "dcor>=0.6"]
 EXTRAS_REQUIRE["test"] = TESTS_REQUIRE
@@ -57,15 +58,15 @@
 
 # Use a custom build to handle numpy.include_dirs() when building
 CMDCLASS = {"build_ext": UseNumpyHeadersBuildExt}
 
 # Run the setup
 setup(
     name="tigramite",
-    version="5.2.0.2",
+    version="5.2.1.6",
     packages=["tigramite", "tigramite.independence_tests", "tigramite.toymodels"],
     license="GNU General Public License v3.0",
     description="Tigramite causal inference for time series",
     author="Jakob Runge",
     author_email="jakob@jakob-runge.com",
     url="https://github.com/jakobrunge/tigramite/",
     long_description=long_description,
```

### Comparing `tigramite-5.2.0.2/tests/test_construct_array.py` & `tigramite-5.2.1.6/tests/test_construct_array.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.2/tests/test_independence_tests.py` & `tigramite-5.2.1.6/tests/test_independence_tests.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.2/tests/test_models.py` & `tigramite-5.2.1.6/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.2/tests/test_pcmci_calculations.py` & `tigramite-5.2.1.6/tests/test_pcmci_calculations.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.2/tests/test_pcmci_construction.py` & `tigramite-5.2.1.6/tests/test_pcmci_construction.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.2/tests/test_var_process.py` & `tigramite-5.2.1.6/tests/test_var_process.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.2/tigramite/causal_effects.py` & `tigramite-5.2.1.6/tigramite/causal_effects.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Tigramite causal discovery for time series."""
+"""Tigramite causal inference for time series."""
 
 # Author: Jakob Runge <jakob@jakob-runge.com>
 #
 # License: GNU General Public License v3.0
 
 import numpy as np
 import math
@@ -2360,14 +2360,43 @@
                 q = [100*(1. - c_int), 100*c_int])[:,:,0]
 
         if return_individual_bootstrap_results:
             return bootstrap_predicted_array, confidence_interval
 
         return confidence_interval
 
+    @staticmethod
+    def get_dict_from_graph(graph, parents_only=False):
+        """Helper function to convert graph to dictionary of links.
+
+        Parameters
+        ---------
+        graph : array of shape (N, N, tau_max+1)
+            Matrix format of graph in string format.
+
+        parents_only : bool
+            Whether to only return parents ('-->' in graph)
+
+        Returns
+        -------
+        links : dict
+            Dictionary of form {0:{(0, -1): o-o, ...}, 1:{...}, ...}.
+        """
+        N = graph.shape[0]
+
+        links = dict([(j, {}) for j in range(N)])
+
+        if parents_only:
+            for (i, j, tau) in zip(*np.where(graph=='-->')):
+                links[j][(i, -tau)] = graph[i,j,tau]
+        else:
+            for (i, j, tau) in zip(*np.where(graph!='')):
+                links[j][(i, -tau)] = graph[i,j,tau]
+
+        return links
 
     @staticmethod
     def get_graph_from_dict(links, tau_max=None):
         """Helper function to convert dictionary of links to graph array format.
 
         Parameters
         ---------
```

### Comparing `tigramite-5.2.0.2/tigramite/data_processing.py` & `tigramite-5.2.1.6/tigramite/data_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,25 +34,25 @@
             OR
             2) Dictionary whose values are numpy arrays of shape
             (observations T_i, variables N), where the number of observations
             T_i may vary across the multiple datasets but the number of variables
             N is fixed. 
     mask : array-like, optional (default: None)
         Optional mask array, must be of same format and shape as data.
-   type_mask : array-like
+   data_type : array-like
         Binary data array of same shape as array which describes whether 
         individual samples in a variable (or all samples) are continuous 
         or discrete: 0s for continuous variables and 1s for discrete variables.
     missing_flag : number, optional (default: None)
         Flag for missing values in dataframe. Dismisses all time slices of
         samples where missing values occur in any variable. For
         remove_missing_upto_maxlag=True also flags samples for all lags up to
         2*tau_max (more precisely, this depends on the cut_off argument in
         self.construct_array(), see further below). This avoids biases, see
-        section on masking in Supplement of [1]_.
+        section on masking in Supplement of Runge et al. SciAdv (2019).
     vector_vars : dict
         Dictionary of vector variables of the form,
         Eg. {0: [(0, 0), (1, 0)], 1: [(2, 0)], 2: [(3, 0)], 3: [(4, 0)]}
         The keys are the new vectorized variables and respective tuple values
         are the individual components of the vector variables. In the method of
         construct_array(), the individual components are parsed from vector_vars
         and added (accounting for lags) to the list that creates X, Y and Z for
@@ -113,15 +113,15 @@
                 Is data
     self.datasets: list
         List of the keys identifiying the multiple datasets, i.e.,
         list(self.values.keys())
     self.mask : dictionary
         Mask internally mapped to a dictionary representation in the same way as
         data is mapped to self.values
-    self.type_mask : array-like
+    self.data_type : array-like
         Binary data array of same shape as array which describes whether 
         individual samples in a variable (or all samples) are continuous 
         or discrete: 0s for continuous variables and 1s for discrete variables.
     self.missing_flag:
         Is missing_flag
     self.var_names:
         If var_names is not None:
@@ -156,15 +156,15 @@
         observation exists in the dataset.
     self.bootstrap : dictionary
         Whether to use bootstrap. Must be a dictionary with keys random_state,
         boot_samples, and boot_blocklength.
     """
 
     def __init__(self, data, mask=None, missing_flag=None, vector_vars=None, var_names=None,
-        type_mask=None, datatime=None, analysis_mode ='single', reference_points=None,
+        data_type=None, datatime=None, analysis_mode ='single', reference_points=None,
         time_offsets=None, remove_missing_upto_maxlag=False):
 
         # Check that a valid analysis mode, specified by the argument
         # 'analysis_mode', has been chosen
         if analysis_mode in ['single', 'multiple']:
             self.analysis_mode = analysis_mode
         else:
@@ -320,17 +320,17 @@
         else:
             self.var_names = var_names
 
         self.mask = None
         if mask is not None:
             self.mask = self._check_mask(mask = mask)
             
-        self.type_mask = None
-        if type_mask is not None:
-            self.type_mask = self._check_mask(mask = type_mask, check_type_mask=True)
+        self.data_type = None
+        if data_type is not None:
+            self.data_type = self._check_mask(mask = data_type, check_data_type=True)
 
         # Check and prepare the time offsets
         self._check_and_set_time_offsets(time_offsets)
         self.time_offsets_is_none = time_offsets is None
 
         # Set the default datatime if unspecified
         if datatime is None:
@@ -358,15 +358,15 @@
         self.remove_missing_upto_maxlag = remove_missing_upto_maxlag
 
         # If PCMCI.run_bootstrap_of is called, then the
         # bootstrap random draw can be set here
         self.bootstrap = None
 
 
-    def _check_mask(self, mask, check_type_mask=False):
+    def _check_mask(self, mask, check_data_type=False):
         """Checks that the mask is:
             * The same shape as the data
             * Is an numpy ndarray (or subtype)
             * Does not contain any NaN entries
 
         """
         # Check that there is a mask if required
@@ -413,15 +413,15 @@
 
             # Check for consistency with shape of 'self.values' and for NaNs
             for dataset_key, dataset_data in self.values.items():
                 _use_mask_dict_data = _use_mask_dict[dataset_key] 
                 if _use_mask_dict_data.shape == dataset_data.shape:
                     if np.sum(np.isnan(_use_mask_dict_data)) != 0:
                         raise ValueError("NaNs in the data mask")
-                    if check_type_mask:
+                    if check_data_type:
                         if not set(np.unique(_use_mask_dict_data)).issubset(set([0, 1])):
                             raise ValueError("Type mask contains other values than 0 and 1")
                 else:
                     if self.analysis_mode == 'single':
                         raise ValueError("Shape mismatch: 'data' is of shape "\
                             "{}, 'mask' is of shape {}. Must be "\
                             "identical.".format(dataset_data.shape,
@@ -545,15 +545,15 @@
             raise ValueError("No valid reference point.") 
 
 
     def construct_array(self, X, Y, Z, tau_max,
                         extraZ=None,
                         mask=None,
                         mask_type=None,
-                        type_mask=None,
+                        data_type=None,
                         return_cleaned_xyz=False,
                         do_checks=True,
                         remove_overlaps=True,
                         cut_off='2xtau_max',
                         verbosity=0):
         """Constructs array from variables X, Y, Z from data.
         Data is of shape (T, N) if analysis_mode == 'single', where T is the
@@ -573,19 +573,19 @@
             Optional mask array, must be of same shape as data.  If it is set,
             then it overrides the self.mask assigned to the dataframe. If it is
             None, then the self.mask is used, if it exists.
         mask_type : {None, 'y','x','z','xy','xz','yz','xyz'}
             Masking mode: Indicators for which variables in the dependence
             measure I(X; Y | Z) the samples should be masked. If None, the mask
             is not used. Explained in tutorial on masking and missing values.
-        type_mask : array-like
+        data_type : array-like
             Binary data array of same shape as array which describes whether 
             individual samples in a variable (or all samples) are continuous 
             or discrete: 0s for continuous variables and 1s for discrete variables.
-            If it is set, then it overrides the self.type_mask assigned to the dataframe.
+            If it is set, then it overrides the self.data_type assigned to the dataframe.
         return_cleaned_xyz : bool, optional (default: False)
             Whether to return cleaned X,Y,Z, where possible duplicates are
             removed.
         do_checks : bool, optional (default: True)
             Whether to perform sanity checks on input X,Y,Z
         remove_overlaps : bool, optional (default: True)
             Whether to remove variables from Z/extraZ if they overlap with X or Y.
@@ -638,15 +638,15 @@
                 the same for all MCI tests, the samples themselves may be
                 different.
         verbosity : int, optional (default: 0)
             Level of verbosity.
 
         Returns
         -------
-        array, xyz [,XYZ], type_mask : Tuple of data array of shape (dim, n_samples),
+        array, xyz [,XYZ], data_type : Tuple of data array of shape (dim, n_samples),
             xyz identifier array of shape (dim,) identifying which row in array
             corresponds to X, Y, and Z, and the type mask that indicates which samples
             are continuous or discrete. For example:: X = [(0, -1)],
             Y = [(1, 0)], Z = [(1, -1), (0, -2)] yields an array of shape
             (4, n_samples) and xyz is xyz = numpy.array([0,1,2,2]). If
             return_cleaned_xyz is True, also outputs the cleaned XYZ lists.
         """
@@ -696,19 +696,19 @@
         # Use the mask, override if needed
         _mask = mask
         if _mask is None:
             _mask = self.mask
         else:
             _mask = self._check_mask(mask = _mask)
             
-        _type_mask = type_mask
-        if _type_mask is None:
-            _type_mask = self.type_mask
+        _data_type = data_type
+        if _data_type is None:
+            _data_type = self.data_type
         else:
-            _type_mask = self._check_mask(mask = _type_mask, check_type_mask=True)
+            _data_type = self._check_mask(mask = _data_type, check_data_type=True)
 
         # Figure out what cut off we will be using
         if cut_off == '2xtau_max':
             max_lag = 2*tau_max
         elif cut_off == 'max_lag':
             max_lag = abs(np.array(XYZ)[:, 1].min())
         elif cut_off == 'tau_max':
@@ -730,15 +730,15 @@
         xyz = np.array([index_code[name]
                         for var, name in zip([X, Y, Z, extraZ], ['x', 'y', 'z', 'e'])
                         for _ in var])
 
         # Run through all datasets and fill a dictionary holding the
         # samples taken from the individual datasets
         samples_datasets = dict()
-        type_masks = dict()
+        data_types = dict()
         self.use_indices_dataset_dict = dict()
 
         for dataset_key, dataset_data in self.values.items():
 
             # Apply time offset to the reference points
             ref_points_here = self.reference_points - self.time_offsets[dataset_key]
 
@@ -824,19 +824,19 @@
                 for i, (var, lag) in enumerate(XYZ):
                     mask_dataset[i, :] = _mask[dataset_key][ref_points_here + lag, var]
 
             # Take care of masking
             use_indices_dataset = np.ones(len(ref_points_here), dtype = 'int')
 
             # Build the type mask array corresponding to this dataset
-            if _type_mask is not None:
-                type_mask_dataset = np.zeros((dim, len(ref_points_here)), dtype = 'bool')
+            if _data_type is not None:
+                data_type_dataset = np.zeros((dim, len(ref_points_here)), dtype = 'bool')
                 for i, (var, lag) in enumerate(XYZ):
-                    type_mask_dataset[i, :] = _type_mask[dataset_key][ref_points_here + lag, var]
-                type_masks[dataset_key] = type_mask_dataset
+                    data_type_dataset[i, :] = _data_type[dataset_key][ref_points_here + lag, var]
+                data_types[dataset_key] = data_type_dataset
             
             # Remove all values that have missing value flag, and optionally as well the time
             # slices that occur up to max_lag after
             if self.missing_flag is not None:
                 missing_anywhere = np.array(np.where(np.any(np.isnan(samples_datasets[dataset_key]), axis=0))[0])
 
                 if self.remove_missing_upto_maxlag:
@@ -871,16 +871,16 @@
         if len(ref_points_here) > 0:
             self.use_indices_dataset_dict[dataset_key] = ref_points_here[use_indices_dataset==1]
         else:
             self.use_indices_dataset_dict[dataset_key] = []
 
         # Concatenate the arrays of all datasets
         array = np.concatenate(tuple(samples_datasets.values()), axis = 1)
-        if _type_mask is not None:
-            type_array = np.concatenate(tuple(type_masks.values()), axis = 1)
+        if _data_type is not None:
+            type_array = np.concatenate(tuple(data_types.values()), axis = 1)
         else:
             type_array = None
         
         # print(np.where(np.isnan(array)))
         # print(array.shape)
 
         # Check whether there is any valid sample
@@ -927,15 +927,15 @@
                 or np.any(np.array(XYZ)[:, 0] < 0)):
             raise ValueError("var indices %s," % str(np.array(XYZ)[:, 0]) +
                              " but must be in [0, %d]" % (N - 1))
         # if np.all(np.array(Y)[:, 1] != 0):
         #     raise ValueError("Y-nodes are %s, " % str(Y) +
         #                      "but one of the Y-nodes must have zero lag")
 
-    def print_array_info(self, array, X, Y, Z, missing_flag, mask_type, type_mask=None, extraZ=None):
+    def print_array_info(self, array, X, Y, Z, missing_flag, mask_type, data_type=None, extraZ=None):
         """
         Print info about the constructed array
 
         Parameters
         ----------
         array : Data array of shape (dim, T)
             Data array.
@@ -949,15 +949,15 @@
             missing values occur in any variable and also flags samples for all
             lags up to 2*tau_max. This avoids biases, see section on masking in
             Supplement of [1]_.
         mask_type : {'y','x','z','xy','xz','yz','xyz'}
             Masking mode: Indicators for which variables in the dependence
             measure I(X; Y | Z) the samples should be masked. If None, the mask
             is not used. Explained in tutorial on masking and missing values.
-        type_mask : array-like
+        data_type : array-like
             Binary data array of same shape as array which describes whether 
             individual samples in a variable (or all samples) are continuous 
             or discrete: 0s for continuous variables and 1s for discrete variables.
         """
         if extraZ is None:
             extraZ = []
         indt = " " * 12
@@ -965,16 +965,16 @@
               "\n" + indt + "X = %s" % str(X) +
               "\n" + indt + "Y = %s" % str(Y) +
               "\n" + indt + "Z = %s" % str(Z))
         if extraZ is not None:  
             print(indt + "extraZ = %s" % str(extraZ))
         if self.mask is not None and mask_type is not None:
             print(indt+"with masked samples in %s removed" % mask_type)
-        if self.type_mask is not None:
-            print(indt+"with %s % discrete values" % np.sum(type_mask)/type_mask.size)
+        if self.data_type is not None:
+            print(indt+"with %s % discrete values" % np.sum(data_type)/data_type.size)
         if self.missing_flag is not None:
             print(indt+"with missing values = %s removed" % self.missing_flag)
 
 
 def get_acf(series, max_lag=None):
     """Returns autocorrelation function.
```

### Comparing `tigramite-5.2.0.2/tigramite/independence_tests/LBFGS.py` & `tigramite-5.2.1.6/tigramite/independence_tests/LBFGS.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.2/tigramite/independence_tests/cmiknn.py` & `tigramite-5.2.1.6/tigramite/independence_tests/cmiknn.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from __future__ import print_function
 from scipy import special, spatial
 import numpy as np
 from .independence_tests_base import CondIndTest
 from numba import jit
 import warnings
 
+
 class CMIknn(CondIndTest):
     r"""Conditional mutual information test based on nearest-neighbor estimator.
 
     Conditional mutual information is the most general dependency measure coming
     from an information-theoretic framework. It makes no assumptions about the
     parametric form of the dependencies by directly estimating the underlying
     joint density. The test here is based on the estimator in  S. Frenzel and B.
@@ -472,13 +473,13 @@
 
     T = 1000
     dimz = 1
 
     # Continuous data
     z = random_state.standard_normal((T, dimz))
     x = (0.8*z[:,0] + random_state.standard_normal(T)).reshape(T, 1)
-    y = (0.8*z[:,0] + random_state.standard_normal).reshape(T, 1)
+    y = (0.8*z[:,0] + random_state.standard_normal(T)).reshape(T, 1)
 
-    print('X _|_ Y')
-    print(cmi.run_test_raw(x, y, z=None))
+    # print('X _|_ Y')
+    # print(cmi.run_test_raw(x, y, z=None))
     print('X _|_ Y | Z')
     print(cmi.run_test_raw(x, y, z=z))
```

### Comparing `tigramite-5.2.0.2/tigramite/independence_tests/cmisymb.py` & `tigramite-5.2.1.6/tigramite/independence_tests/cmisymb.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 #
 # License: GNU General Public License v3.0
 
 from __future__ import print_function
 import warnings
 import numpy as np
 from scipy.stats.contingency import crosstab
-from joblib import Parallel, delayed
-import multiprocessing
+# from joblib import Parallel, delayed
+# import dask
 from numba import jit
 
 from .independence_tests_base import CondIndTest
 
 class CMIsymb(CondIndTest):
     r"""Conditional mutual information test for discrete/categorical data.
 
@@ -184,19 +184,24 @@
             # Create neighbor indices of length z_comb with default as -1.
             neighbors = np.full((len(z_comb), T), -1)
             # Neighborhood indices for each unique combination in z_comb.
             for i in range(len(z_comb)):
                 neighbor_indices = np.where((z_array == z_comb[i]).all(axis=1))[0]
                 neighbors[i, :len(neighbor_indices)] = neighbor_indices
 
-            num_cores = multiprocessing.cpu_count()
             random_seeds = self.random_state.integers(np.iinfo(np.int32).max, size=self.sig_samples)
-            null_dist = Parallel(n_jobs=num_cores)(
-                delayed(self.parallelize_shuffles)(array, xyz, z_indices, x_indices, T, z_comb, neighbors, seed=seed) for seed in random_seeds)
-            null_dist = np.asarray(null_dist)
+            # null_dist = Parallel(n_jobs=-1)(
+            #     delayed(self.parallelize_shuffles)(array, xyz, z_indices, x_indices, T, z_comb, neighbors, seed=seed) for seed in random_seeds)
+            # dask_jobs = [dask.delayed(self.parallelize_shuffles)(array, xyz, z_indices, x_indices, T, z_comb, neighbors, seed=seed) for seed in random_seeds]
+            # null_dist = dask.compute(dask_jobs)
+            # null_dist = np.asarray(null_dist)
+
+            null_dist = np.zeros(self.sig_samples)
+            for i, seed in enumerate(random_seeds):
+                null_dist[i] = self.parallelize_shuffles(array, xyz, z_indices, x_indices, T, z_comb, neighbors, seed=seed)
 
         else:
             null_dist = \
                 self._get_shuffle_dist(array, xyz,
                                        self.get_dependence_measure,
                                        sig_samples=self.sig_samples,
                                        sig_blocklength=self.sig_blocklength,
@@ -247,26 +252,33 @@
 
 if __name__ == '__main__':
     
     import tigramite
     from tigramite.data_processing import DataFrame
     import tigramite.data_processing as pp
     import numpy as np
+    # from dask.distributed import Client
 
+    # client = dask.distributed.Client(processes=True)
     seed = 42
     random_state = np.random.default_rng(seed=seed)
-    cmi = CMIsymb(sig_samples=100, seed=seed)
+    cmi = CMIsymb(sig_samples=200, seed=seed)
 
     T = 1000
-    dimz = 10
+    dimz = 5
     z = random_state.binomial(n=1, p=0.5, size=(T, dimz)).reshape(T, dimz)
     x = np.empty(T).reshape(T, 1)
     y = np.empty(T).reshape(T, 1)
     for t in range(T):
         val = z[t, 0].squeeze()
         prob = 0.2+val*0.6
         x[t] = random_state.choice([0,1], p=[prob, 1.-prob])
         y[t] = random_state.choice([0,1, 2], p=[prob, (1.-prob)/2., (1.-prob)/2.])
 
     print('start')
-    print(cmi.run_test_raw(x, y, z=None))
+    # print(client.dashboard_link)
+    # print(cmi.run_test_raw(x, y, z=None))
     print(cmi.run_test_raw(x, y, z=z))
+
+    # client.close()
+
+
```

### Comparing `tigramite-5.2.0.2/tigramite/independence_tests/gpdc.py` & `tigramite-5.2.1.6/tigramite/independence_tests/gpdc.py`

 * *Files 0% similar despite different names*

```diff
@@ -540,20 +540,20 @@
         x_vals = self._get_single_residuals(array, target_var=0)
         y_vals = self._get_single_residuals(array, target_var=1)
         val = self._get_dcorr(np.array([x_vals, y_vals]))
         return val
 
 
     def _get_dcorr(self, array_resid):
-        """Return distance correlation coefficient.
+        r"""Return distance correlation coefficient.
 
         The variables are transformed to uniform marginals using the empirical
         cumulative distribution function beforehand. Here the null distribution
         is not analytically available, but can be precomputed with the function
-        generate_and_save_nulldists(...) which saves a \*.npz file containing
+        generate_and_save_nulldists(...) which saves a *.npz file containing
         the null distribution for different sample sizes. This file can then be
         supplied as null_dist_filename.
 
         Parameters
         ----------
         array_resid : array-like
             data array must be of shape (2, T)
```

### Comparing `tigramite-5.2.0.2/tigramite/independence_tests/gpdc_torch.py` & `tigramite-5.2.1.6/tigramite/independence_tests/gpdc_torch.py`

 * *Files 0% similar despite different names*

```diff
@@ -701,15 +701,15 @@
 
     def _get_dcorr(self, array_resid):
         """Return distance correlation coefficient.
 
         The variables are transformed to uniform marginals using the empirical
         cumulative distribution function beforehand. Here the null distribution
         is not analytically available, but can be precomputed with the function
-        generate_and_save_nulldists(...) which saves a \*.npz file containing
+        generate_and_save_nulldists(...) which saves a *.npz file containing
         the null distribution for different sample sizes. This file can then be
         supplied as null_dist_filename.
 
         Parameters
         ----------
         array_resid : array-like
             data array must be of shape (2, T)
```

### Comparing `tigramite-5.2.0.2/tigramite/independence_tests/gsquared.py` & `tigramite-5.2.1.6/tigramite/independence_tests/gsquared.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.2/tigramite/independence_tests/independence_tests_base.py` & `tigramite-5.2.1.6/tigramite/independence_tests/independence_tests_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -215,15 +215,15 @@
         Base class assumption that this is not implemented.  Concrete classes
         should override when possible.
         """
         raise NotImplementedError("Analytic significance not"+\
                                   " implemented for %s" % self.measure)
 
     def get_shuffle_significance(self, array, xyz, value,
-                                 type_mask=None,
+                                 data_type=None,
                                  return_null_dist=False):
         """
         Base class assumption that this is not implemented.  Concrete classes
         should override when possible.
         """
         raise NotImplementedError("Shuffle significance not"+\
                                   " implemented for %s" % self.measure)
@@ -353,15 +353,15 @@
         Returns
         -------
         val, pval : Tuple of floats
             The test statistic value and the p-value.
         """
 
         # Get the array to test on
-        array, xyz, XYZ, type_mask = self._get_array(X, Y, Z, tau_max, cut_off, self.verbosity)
+        array, xyz, XYZ, data_type = self._get_array(X, Y, Z, tau_max, cut_off, self.verbosity)
         X, Y, Z = XYZ
         
         # Record the dimensions
         dim, T = array.shape
         # Ensure it is a valid array
         if np.any(np.isnan(array)):
             raise ValueError("nans in the array!")
@@ -370,15 +370,15 @@
 
         if combined_hash in self.cached_ci_results.keys():
             cached = True
             val, pval = self.cached_ci_results[combined_hash]
         else:
             cached = False
             # Get the dependence measure, reycling residuals if need be
-            val = self._get_dependence_measure_recycle(X, Y, Z, xyz, array, type_mask)
+            val = self._get_dependence_measure_recycle(X, Y, Z, xyz, array, data_type)
             # Get the p-value
             pval = self.get_significance(val, array, xyz, T, dim)
             self.cached_ci_results[combined_hash] = (val, pval)
 
         if self.verbosity > 1:
             self._print_cond_ind_results(val=val, pval=pval, cached=cached,
                                          conf=None)
@@ -414,69 +414,69 @@
                              " where dimension can be 1.")
 
         if z is not None and np.ndim(z) != 2:
             raise ValueError("z must be array of shape (samples, dimension)"
                              " where dimension can be 1.")
 
         if x_type is not None or y_type is not None or z_type is not None:
-            has_type_mask = True
+            has_data_type = True
         else:
-            has_type_mask = False
+            has_data_type = False
 
-        if x_type is None and has_type_mask:
+        if x_type is None and has_data_type:
             x_type = np.zeros(x.shape, dtype='int')
 
-        if y_type is None and has_type_mask:
+        if y_type is None and has_data_type:
             y_type = np.zeros(y.shape, dtype='int')
 
         if z is None:
             # Get the array to test on
             array = np.vstack((x.T, y.T))
-            if has_type_mask:
-                type_mask = np.vstack((x_type.T, y_type.T))
+            if has_data_type:
+                data_type = np.vstack((x_type.T, y_type.T))
 
             # xyz is the dimension indicator
             xyz = np.array([0 for i in range(x.shape[1])] +
                            [1 for i in range(y.shape[1])])
 
         else:
             # Get the array to test on
             array = np.vstack((x.T, y.T, z.T))
-            if z_type is None and has_type_mask:
+            if z_type is None and has_data_type:
                 z_type = np.zeros(z.shape, dtype='int')
 
-            if has_type_mask:
-                type_mask = np.vstack((x_type.T, y_type.T, z_type.T))
+            if has_data_type:
+                data_type = np.vstack((x_type.T, y_type.T, z_type.T))
             # xyz is the dimension indicator
             xyz = np.array([0 for i in range(x.shape[1])] +
                            [1 for i in range(y.shape[1])] +
                            [2 for i in range(z.shape[1])])
 
         # Record the dimensions
         dim, T = array.shape
         # Ensure it is a valid array
         if np.isnan(array).sum() != 0:
             raise ValueError("nans in the array!")
         # Get the dependence measure
-        if has_type_mask:
-            val = self.get_dependence_measure(array, xyz, type_mask=type_mask)
+        if has_data_type:
+            val = self.get_dependence_measure(array, xyz, data_type=data_type)
         else:
             val = self.get_dependence_measure(array, xyz)
 
         # Get the p-value
-        if has_type_mask:
+        if has_data_type:
             pval = self.get_significance(val=val, array=array, xyz=xyz, 
-                    T=T, dim=dim, type_mask=type_mask)
+                    T=T, dim=dim, data_type=data_type)
         else:
             pval = self.get_significance(val=val, array=array, xyz=xyz, 
                     T=T, dim=dim)            
         # Return the value and the pvalue
         return val, pval
 
-    def _get_dependence_measure_recycle(self, X, Y, Z, xyz, array, type_mask=None):
+    def _get_dependence_measure_recycle(self, X, Y, Z, xyz, array, data_type=None):
         """Get the dependence_measure, optionally recycling residuals
 
         If self.recycle_residuals is True, also _get_single_residuals must be
         available.
 
         Parameters
         ----------
@@ -486,15 +486,15 @@
 
         xyz : array of ints
             XYZ identifier array of shape (dim,).
 
         array : array
             Data array of shape (dim, T)
 
-       type_mask : array-like
+       data_type : array-like
             Binary data array of same shape as array which describes whether 
             individual samples in a variable (or all samples) are continuous 
             or discrete: 0s for continuous variables and 1s for discrete variables.
 
         Return
         ------
         val : float
@@ -509,17 +509,17 @@
             array_resid = np.array([x_resid, y_resid])
             xyz_resid = np.array([0, 1])
             # Return the dependence measure
             # data type can only be continuous in this case
             return self.get_dependence_measure(array_resid, xyz_resid)
 
         # If not, return the dependence measure on the array and xyz
-        if type_mask is not None:
+        if data_type is not None:
             return self.get_dependence_measure(array, xyz, 
-                                        type_mask=type_mask)
+                                        data_type=data_type)
         else:
             return self.get_dependence_measure(array, xyz)
 
     def _get_cached_residuals(self, x_nodes, z_nodes, array, target_var):
         """
         Retrieve or calculate the cached residuals for the given node sets.
 
@@ -552,15 +552,15 @@
             x_resid = self._get_single_residuals(array, target_var=target_var)
             if z_nodes:
                 self.residuals[self._keyfy(x_nodes, z_nodes)] = x_resid
         # Return these residuals
         return x_resid
 
     def get_significance(self, val, array, xyz, T, dim,
-                         type_mask=None,
+                         data_type=None,
                          sig_override=None):
         """
         Returns the p-value from whichever significance function is specified
         for this test.  If an override is used, then it will call a different
         function then specified by self.significance
 
         Parameters
@@ -576,15 +576,15 @@
 
         T : int
             Sample length
 
         dim : int
             Dimensionality, ie, number of features.
             
-       type_mask : array-like
+       data_type : array-like
             Binary data array of same shape as array which describes whether 
             individual samples in a variable (or all samples) are continuous 
             or discrete: 0s for continuous variables and 1s for discrete variables.
 
         sig_override : string
             Must be in 'analytic', 'shuffle_test', 'fixed_thres'
 
@@ -612,15 +612,15 @@
                     fixed_thres=self.fixed_thres)
         else:
             raise ValueError("%s not known." % self.significance)
         # Return the calculated value
         return pval
 
     def get_measure(self, X, Y, Z=None, tau_max=0, 
-                    type_mask=None):
+                    data_type=None):
         """Estimate dependence measure.
 
         Calls the dependence measure function. The child classes must specify
         a function get_dependence_measure.
 
         Parameters
         ----------
@@ -628,15 +628,15 @@
             X,Y,Z are of the form [(var, -tau)], where var specifies the
             variable index and tau the time lag.
 
         tau_max : int, optional (default: 0)
             Maximum time lag. This may be used to make sure that estimates for
             different lags in X, Z, all have the same sample size.
         
-       type_mask : array-like
+       data_type : array-like
             Binary data array of same shape as array which describes whether 
             individual samples in a variable (or all samples) are continuous 
             or discrete: 0s for continuous variables and 1s for discrete variables.
 
 
         Returns
         -------
@@ -650,15 +650,15 @@
         # Check it is valid
         if np.isnan(array).sum() != 0:
             raise ValueError("nans in the array!")
         # Return the dependence measure
         return self._get_dependence_measure_recycle(X, Y, Z, xyz, array)
 
     def get_confidence(self, X, Y, Z=None, tau_max=0,
-                       type_mask=None):
+                       data_type=None):
         """Perform confidence interval estimation.
 
         Calls the dependence measure and confidence test functions. The child
         classes can specify a function get_dependence_measure and
         get_analytic_confidence or get_bootstrap_confidence. If confidence is
         False, (numpy.nan, numpy.nan) is returned.
 
@@ -668,15 +668,15 @@
             X,Y,Z are of the form [(var, -tau)], where var specifies the
             variable index and tau the time lag.
 
         tau_max : int, optional (default: 0)
             Maximum time lag. This may be used to make sure that estimates for
             different lags in X, Z, all have the same sample size.
             
-       type_mask : array-like
+       data_type : array-like
             Binary data array of same shape as array which describes whether 
             individual samples in a variable (or all samples) are continuous 
             or discrete: 0s for continuous variables and 1s for discrete variables.
 
         Returns
         -------
         (conf_lower, conf_upper) : Tuple of floats
@@ -691,15 +691,15 @@
             half_conf = self.conf_samples * (1. - self.conf_lev)/2.
             if self.confidence == 'bootstrap' and  half_conf < 1.:
                 raise ValueError("conf_samples*(1.-conf_lev)/2 is %.2f"
                                  % half_conf + ", must be >> 1")
 
         if self.confidence:
             # Make and check the array
-            array, xyz, _, type_mask = self._get_array(X, Y, Z, tau_max, verbosity=0)
+            array, xyz, _, data_type = self._get_array(X, Y, Z, tau_max, verbosity=0)
             dim, T = array.shape
             if np.isnan(array).sum() != 0:
                 raise ValueError("nans in the array!")
 
             # Check if we are using analytic confidence or bootstrapping it
             if self.confidence == 'analytic':
                 val = self.get_dependence_measure(array, xyz)
@@ -750,15 +750,15 @@
             printstr += " %s" % ({0:"", 1:"[cached]"}[cached])
 
         print(printstr)
 
     def get_bootstrap_confidence(self, array, xyz, dependence_measure=None,
                                  conf_samples=100, conf_blocklength=None,
                                  conf_lev=.95, 
-                                 type_mask=None,
+                                 data_type=None,
                                  verbosity=0):
         """Perform bootstrap confidence interval estimation.
 
         With conf_blocklength > 1 or None a block-bootstrap is performed.
 
         Parameters
         ----------
@@ -779,15 +779,15 @@
             Number of samples for bootstrap.
 
         conf_blocklength : int, optional (default: None)
             Block length for block-bootstrap. If None, the block length is
             determined from the decay of the autocovariance as explained in
             [1]_.
 
-       type_mask : array-like
+       data_type : array-like
             Binary data array of same shape as array which describes whether 
             individual samples in a variable (or all samples) are continuous 
             or discrete: 0s for continuous variables and 1s for discrete variables.
 
         verbosity : int, optional (default: 0)
             Level of verbosity.
 
@@ -931,15 +931,15 @@
             try:
                 popt, _ = optimize.curve_fit(
                     f=func,
                     xdata=np.arange(0, max_lag+1),
                     ydata=hilbert,
                 )
                 phi = popt[1]
-                # Formula of Peifer (2005) assuming non-overlapping blocks
+                # Formula assuming non-overlapping blocks
                 l_opt = (4. * T * (phi / (1. - phi) + phi**2 / (1. - phi)**2)**2
                          / (1. + 2. * phi / (1. - phi))**2)**(1. / 3.)
                 block_len = max(block_len, int(l_opt))
             except RuntimeError:
                 print("Error - curve_fit failed in block_shuffle, using"
                       " block_len = %d" % (int(.05 * T)))
                 # block_len = max(int(.05 * T), block_len)
```

### Comparing `tigramite-5.2.0.2/tigramite/independence_tests/oracle_conditional_independence.py` & `tigramite-5.2.1.6/tigramite/independence_tests/oracle_conditional_independence.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.2/tigramite/independence_tests/parcorr.py` & `tigramite-5.2.1.6/tigramite/independence_tests/parcorr.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.2/tigramite/independence_tests/parcorr_mult.py` & `tigramite-5.2.1.6/tigramite/independence_tests/parcorr_mult.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.2/tigramite/independence_tests/parcorr_wls.py` & `tigramite-5.2.1.6/tigramite/independence_tests/parcorr_wls.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,25 +124,25 @@
 
         if self.measure in ['par_corr_wls']:
             if len(X) > 1 or len(Y) > 1:
                 raise ValueError("X and Y for %s must be univariate." %
                                  self.measure)
 
         # Call the wrapped function
-        array, xyz, XYZ, type_mask = self.dataframe.construct_array(X=X, Y=Y, Z=Z,
+        array, xyz, XYZ, data_type = self.dataframe.construct_array(X=X, Y=Y, Z=Z,
                                                             tau_max=tau_max,
                                                             mask_type=self.mask_type,
                                                             return_cleaned_xyz=return_cleaned_xyz,
                                                             do_checks=True,
                                                             remove_overlaps=True,
                                                             cut_off=cut_off,
                                                             verbosity=verbosity)
         array_copy = array.copy()
         self._get_stds(array_copy, X, Y, Z, tau_max, cut_off, verbosity)
-        return array, xyz, XYZ, type_mask
+        return array, xyz, XYZ, data_type
 
     def _estimate_std_time(self, arr, target_var):
         """
         Estimate the standard deviations of the error terms using the squared-residuals approach. First calculate
         the absolute value of the residuals using OLS, then smooth them using a sliding window while keeping the time
         order of the residuals.
         In this way we can approximate variances that are time-dependent.
```

### Comparing `tigramite-5.2.0.2/tigramite/independence_tests/regressionCI.py` & `tigramite-5.2.1.6/tigramite/independence_tests/regressionCI.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,31 +72,31 @@
         self.dataframe = dataframe
         
         if self.mask_type is not None:
             if dataframe.mask is None:
                 raise ValueError("mask_type is not None, but no mask in dataframe.")
             dataframe._check_mask(dataframe.mask)
         
-        if dataframe.type_mask is None:
-            raise ValueError("type_mask cannot be None for RegressionCI.")
-        dataframe._check_mask(dataframe.type_mask, check_type_mask=True)
+        if dataframe.data_type is None:
+            raise ValueError("data_type cannot be None for RegressionCI.")
+        dataframe._check_mask(dataframe.data_type, check_data_type=True)
 
     # @jit(forceobj=True)
-    def get_dependence_measure(self, array, xyz, type_mask):
+    def get_dependence_measure(self, array, xyz, data_type):
         """Returns test statistic.
 
         Parameters
         ----------
         array : array-like
             data array with X, Y, Z in rows and observations in columns.
 
         xyz : array of ints
             XYZ identifier array of shape (dim,).
 
-        type_mask : array-like
+        data_type : array-like
             array of same shape as array which describes whether samples
             are continuous or discrete: 0s for continuous and
             1s for discrete
 
         Returns
         -------
         val : float
@@ -120,15 +120,15 @@
             for i in range(0, len(var_type)):
                 if var_type[i] == 1:
                     nb_classes = len(set(X[:, i]))
                     X_new = np.hstack((X_new, convert_to_one_hot(X[:, i].astype(int), nb_classes=nb_classes)))
                 elif var_type[i] == 0:
                     X_new = np.hstack((X_new, X[:, i].reshape((T, 1))))
                 else:
-                    raise ValueError("type_mask only allows entries in {0, 1}")
+                    raise ValueError("data_type only allows entries in {0, 1}")
             return X_new
 
         def calc_deviance_logistic(X, y, var_type):
             """Calculates the deviance (i.e., 2 * log-likelihood) for a multinomial logistic regression
             (with standard regression assumptions)
             """
 
@@ -174,23 +174,23 @@
         x_indices = np.where(xyz == 0)[0]
         y_indices = np.where(xyz == 1)[0]
         z_indices = np.where(xyz == 2)[0]
 
         x = array[x_indices].T
         y = array[y_indices].T
 
-        x_type = type_mask[x_indices]
-        y_type = type_mask[y_indices]
+        x_type = data_type[x_indices]
+        y_type = data_type[y_indices]
 
         if len(z_indices) == 0:
             z = np.ones((array.shape[1], 1))
             z_type = [0]
         else:
             z = array[z_indices].T
-            z_type = type_mask[z_indices]
+            z_type = data_type[z_indices]
             z_type = z_type.max(axis=1)
 
         # check, whether within X and within Y all datapoints have the same datatype
         if ((x_type.max() != x_type.min()) or (y_type.max() != y_type.min())):
             raise ValueError("All samples regarding X or respectively Y must have the same datatype")
         
         x_type = x_type.max()
@@ -348,21 +348,21 @@
         else:
             z_type = None
 
         val, pval = ci.run_test_raw(x, y, z=z, x_type=x_type, y_type=y_type, z_type=z_type)
         rate[i] = pval
 
         # data = np.hstack((x, y, z))
-        # type_mask = np.zeros(data.shape)
-        # type_mask[:, 0] = x_example == "discrete"
-        # type_mask[:, 1] = y_example == "discrete"
-        # type_mask[:, 2] = z_example == "discrete"
-        # type_mask = type_mask.astype('int')
-        # # print(type_mask)
-        # dataframe = pp.DataFrame(data=data, type_mask=type_mask)
+        # data_type = np.zeros(data.shape)
+        # data_type[:, 0] = x_example == "discrete"
+        # data_type[:, 1] = y_example == "discrete"
+        # data_type[:, 2] = z_example == "discrete"
+        # data_type = data_type.astype('int')
+        # # print(data_type)
+        # dataframe = pp.DataFrame(data=data, data_type=data_type)
         # ci.set_dataframe(dataframe)
         
         # val, pval = ci.run_test(X=[(0, 0)], Y=[(1, 0)], Z=[(2, 0)])
         # rate[i] = pval
 
     print((rate <= 0.05).mean())
```

### Comparing `tigramite-5.2.0.2/tigramite/independence_tests/robust_parcorr.py` & `tigramite-5.2.1.6/tigramite/independence_tests/robust_parcorr.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
             resid = y
             mean = None
 
         if return_means:
             return (resid, mean)
         return resid
 
-    def get_dependence_measure(self, array, xyz, type_mask=None):
+    def get_dependence_measure(self, array, xyz, data_type=None):
         """Return partial correlation.
 
         Marginals are firstly transformed to standard normal scale. Dependence
         Measure is then estimated as the Pearson correlation of the residuals
         of a linear OLS regression.
 
         Parameters
```

### Comparing `tigramite-5.2.0.2/tigramite/lpcmci.py` & `tigramite-5.2.1.6/tigramite/lpcmci.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 from copy import deepcopy
 
 from .pcmci_base import PCMCIbase
 
 class LPCMCI(PCMCIbase):
     """ LPCMCI is an algorithm for causal discovery in large-scale times series that allows for latent confounders and
     learns lag-specific causal relationships. The algorithm is introduced and explained in:
+
     [1] Gerhardus, A. & Runge, J. High-recall causal discovery for autocorrelated time series with latent confounders.
     Advances in Neural Information Processing Systems, 2020, 33.
     https://proceedings.neurips.cc/paper/2020/hash/94e70705efae423efda1088614128d0b-Abstract.html
+    
     NOTE: This method is still EXPERIMENTAL since the default settings of hyperparameters are still being fine-tuned.
     We actually invite feedback on which work best in applications and numerical experiments.
     The main function, which applies the algorithm, is 'run_lpcmci'.
 
     Parameters passed to the constructor:
     - dataframe:
         Tigramite dataframe object that contains the the time series dataset \bold{X}
```

### Comparing `tigramite-5.2.0.2/tigramite/models.py` & `tigramite-5.2.1.6/tigramite/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Tigramite causal discovery for time series."""
+"""Tigramite causal inference for time series."""
 
 # Author: Jakob Runge <jakob@jakob-runge.com>
 #
 # License: GNU General Public License v3.0
 
 from __future__ import print_function
 from copy import deepcopy
@@ -75,14 +75,15 @@
 
     # @profile    
     def get_general_fitted_model(self, 
                 Y, X, Z=None,
                 conditions=None,
                 tau_max=None,
                 cut_off='max_lag_or_tau_max',
+                empty_predictors_function=np.mean,
                 return_data=False):
         """Fit time series model.
 
         For each variable in selected_variables, the sklearn model is fitted
         with :math:`y` given by the target variable, and :math:`X` given by its
         parents. The fitted model class is returned for later use.
 
@@ -97,14 +98,16 @@
         cut_off : {'max_lag_or_tau_max', '2xtau_max', 'max_lag'}
             How many samples to cutoff at the beginning. The default is
             'max_lag_or_tau_max', which uses the maximum of tau_max and the
             conditions. This is useful to compare multiple models on the same
             sample. Other options are '2xtau_max', which guarantees that MCI
             tests are all conducted on the same samples. Last, 'max_lag' uses
             as much samples as possible.
+        empty_predictors_function : function
+            Function to apply to y if no predictors are given.
         return_data : bool, optional (default: False)
             Whether to save the data array.
 
         Returns
         -------
         fit_results : dictionary of sklearn model objects for each variable
             Returns the sklearn model after fitting. Also returns the data
@@ -184,14 +187,23 @@
             predictor_indices =  list(np.where(xyz==0)[0]) \
                                + list(np.where(xyz==3)[0]) \
                                + list(np.where(xyz==2)[0])
             predictor_array = array[predictor_indices, :].T
             # Target is only first entry of Y, ie [y]
             target_array = array[np.where(xyz==1)[0][0], :]
 
+            if predictor_array.size == 0:
+                # Just fit default (eg, mean)
+                class EmptyPredictorModel:
+                    def fit(self, X, y):
+                        self.result = empty_predictors_function(y)
+                    def predict(self, X):
+                        return self.result
+                a_model = EmptyPredictorModel()
+            
             a_model.fit(X=predictor_array, y=target_array)
             
             # Cache the results
             fit_results[y] = {}
             fit_results[y]['observation_array'] = array
             fit_results[y]['xyz'] = xyz
             fit_results[y]['model'] = a_model
@@ -342,14 +354,15 @@
             return predicted_array
 
 
     def fit_full_model(self, all_parents,
                 selected_variables=None,
                 tau_max=None,
                 cut_off='max_lag_or_tau_max',
+                empty_predictors_function=np.mean,
                 return_data=False):
         """Fit time series model.
 
         For each variable in selected_variables, the sklearn model is fitted
         with :math:`y` given by the target variable, and :math:`X` given by its
         parents. The fitted model class is returned for later use.
 
@@ -366,14 +379,16 @@
         cut_off : {'max_lag_or_tau_max', '2xtau_max', 'max_lag'}
             How many samples to cutoff at the beginning. The default is
             'max_lag_or_tau_max', which uses the maximum of tau_max and the
             conditions. This is useful to compare multiple models on the same
             sample. Other options are '2xtau_max', which guarantees that MCI
             tests are all conducted on the same samples. Last, 'max_lag' uses
             as much samples as possible.
+        empty_predictors_function : function
+            Function to apply to y if no predictors are given.
         return_data : bool, optional (default: False)
             Whether to save the data array.
 
         Returns
         -------
         fit_results : dictionary of sklearn model objects for each variable
             Returns the sklearn model after fitting. Also returns the data
@@ -424,21 +439,30 @@
             # Cache the data transform
             fit_results[j]['data_transform'] = deepcopy(self.data_transform)
 
             if return_data:
                 # Cache the data if needed
                 fit_results[j]['data'] = array
                 fit_results[j]['used_indices'] = self.dataframe.use_indices_dataset_dict
-            # Fit the model if there are any parents for this variable to fit
+            # Copy and fit the model if there are any parents for this variable to fit
+            a_model = deepcopy(self.model)
             if dim_z > 0:
-                # Copy and fit the model
-                a_model = deepcopy(self.model)
+                a_model.fit(X=array[2:].T, y=array[1])
+            else:
+                # Just fit default (eg, mean)
+                class EmptyPredictorModel:
+                    def fit(self, X, y):
+                        self.result = empty_predictors_function(y)
+                    def predict(self, X):
+                        return self.result
+                a_model = EmptyPredictorModel()
+                # a_model = empty_predictors_model(array[1])
                 a_model.fit(X=array[2:].T, y=array[1])
 
-                fit_results[j]['model'] = a_model
+            fit_results[j]['model'] = a_model
 
         # Cache and return the fit results
         self.fit_results = fit_results
         return fit_results
 
     def get_coefs(self):
         """Returns dictionary of coefficients for linear models.
@@ -588,15 +612,15 @@
                         dataframe=dataframe,
                         model=this_model,
                         data_transform=data_transform,
                         mask_type=mask_type,
                         verbosity=verbosity)
 
     def fit_model(self, all_parents, tau_max=None):
-        """Fit linear time series model.
+        r"""Fit linear time series model.
 
         Fits a sklearn.linear_model.LinearRegression model to the parents of
         each variable and computes the coefficient matrices :math:`\Phi` and
         :math:`\Psi` as described in [4]_. Does accept contemporaneous links.
 
         Parameters
         ----------
@@ -614,15 +638,15 @@
         # Cache the results in the member variables
         coeffs = self.get_coefs()
         self.phi = self._get_phi(coeffs)
         self.psi = self._get_psi(self.phi)
         self.all_psi_k = self._get_all_psi_k(self.phi)
 
         self.all_parents = all_parents
-        self.tau_max = tau_max
+        # self.tau_max = tau_max
 
     def fit_model_bootstrap(self, 
             boot_blocklength=1,
             seed=None,
             boot_samples=100):
         """Fits boostrap-versions of Phi, Psi, etc.
 
@@ -661,24 +685,22 @@
             else:
                 random_state = np.random.default_rng(seed+b)
 
             dataframe_here = deepcopy(self.dataframe)
 
             dataframe_here.bootstrap = {'boot_blocklength':boot_blocklength,
                                         'random_state':random_state}
-
             model = Models(dataframe=dataframe_here,
                            model=sklearn.linear_model.LinearRegression(**self.model_params),
                            data_transform=self.data_transform,
                            mask_type=self.mask_type,
                            verbosity=0)
 
             model.fit_full_model(all_parents=self.all_parents,
                            tau_max=self.tau_max)
-
             # Cache the results in the member variables
             coeffs = model.get_coefs()
             phi = self._get_phi(coeffs)
             self.phi_boots[b] = phi
             self.psi_boots[b] = self._get_psi(phi)
             self.all_psi_k_boots[b] = self._get_all_psi_k(phi)
 
@@ -1674,37 +1696,38 @@
             Whether to save the data array.
 
         Returns
         -------
         self : instance of self
         """
 
+        if selected_targets is None:
+            self.selected_targets = range(self.N)
+        else:
+            self.selected_targets = selected_targets
+
         if tau_max is None:
             # Find the maximal parents lag
             max_parents_lag = 0
             for j in self.selected_targets:
                 if target_predictors[j]:
                     this_parent_lag = np.abs(np.array(target_predictors[j])[:, 1]).max()
                     max_parents_lag = max(max_parents_lag, this_parent_lag)
         else:
             max_parents_lag = tau_max
 
         if len(set(np.array(self.test_indices) - max_parents_lag)
                 .intersection(self.train_indices)) > 0:
-            warnings.warn("test_indices - maxlag(predictors) [or tau_max] "
+            if self.verbosity > 0:
+                warnings.warn("test_indices - maxlag(predictors) [or tau_max] "
                 "overlaps with train_indices: Choose test_indices "
                 "such that there is a gap of max_lag to train_indices!")
 
         self.target_predictors = target_predictors
 
-        if selected_targets is None:
-            self.selected_targets = range(self.N)
-        else:
-            self.selected_targets = selected_targets
-
         for target in self.selected_targets:
             if target not in list(self.target_predictors):
                 raise ValueError("No predictors given for target %s" % target)
 
         self.fitted_model = \
             self.fit_full_model(all_parents=self.target_predictors,
                          selected_variables=self.selected_targets,
@@ -1753,41 +1776,42 @@
         elif isinstance(target, list):
             target_list = target
         else:
             raise ValueError("target must be either int or list of integers "
                              "indicating the index of the variables to "
                              "predict.")
 
-        if target_list == range(self.N):
+        if target_list == list(range(self.N)):
             return_type = 'array'
         elif len(target_list) == 1:
             return_type = 'series'
         else:
             return_type = 'list'
 
         pred_list = []
+        self.stored_test_array = {}
         for target in target_list:
             # Print message
             if self.verbosity > 0:
                 print("\n##\n## Predicting target %s\n##" % target)
                 if pred_params is not None:
                     for key in list(pred_params):
                         print("%s = %s" % (key, pred_params[key]))
             # Default value for pred_params
             if pred_params is None:
                 pred_params = {}
             # Check this is a valid target
             if target not in self.selected_targets:
                 raise ValueError("Target %s not yet fitted" % target)
             # Construct the array form of the data
-            Y = [(target, 0)]
+            Y = [(target, 0)]  # dummy
             X = [(target, 0)]  # dummy
             Z = self.target_predictors[target]
+
             # Check if we've passed a new dataframe object
-            test_array = None
             if new_data is not None:
                 # if new_data.mask is None:
                 #     # if no mask is supplied, use the same mask as for the fitted array
                 #     new_data_mask = self.test_mask
                 # else:
                 new_data_mask = new_data.mask
                 test_array, _, _ = new_data.construct_array(X, Y, Z,
@@ -1808,83 +1832,99 @@
                                                    remove_overlaps=True,
                                                    verbosity=self.verbosity)
             # Transform the data if needed
             a_transform = self.fitted_model[target]['data_transform']
             if a_transform is not None:
                 test_array = a_transform.transform(X=test_array.T).T
             # Cache the test array
-            self.test_array = test_array
+            self.stored_test_array[target] = test_array
             # Run the predictor
-            pred_list.append(self.fitted_model[target]['model'].predict(
-                X=test_array[2:].T, **pred_params))
+            predicted = self.fitted_model[target]['model'].predict(
+                X=test_array[2:].T, **pred_params)
+
+            if test_array[2:].size == 0:
+                # If there are no predictors, return the value of 
+                # empty_predictors_function, which is np.mean 
+                # and expand to the test array length
+                predicted = predicted * np.ones(test_array.shape[1])
+
+            pred_list.append(predicted)
 
         if return_type == 'series':
             return pred_list[0]
         elif return_type == 'list':
             return pred_list
         elif return_type == 'array':
             return np.array(pred_list).transpose()
 
     def get_train_array(self, j):
-        """Returns training array."""
+        """Returns training array for variable j."""
         return self.fitted_model[j]['data']
 
-    def get_test_array(self):
-        """Returns test array."""
-        return self.test_array
+    def get_test_array(self, j):
+        """Returns test array for variable j."""
+        return self.stored_test_array[j]
 
 if __name__ == '__main__':
    
     import tigramite
     import tigramite.data_processing as pp
     from tigramite.toymodels import structural_causal_processes as toys
-    from tigramite.independence_tests import ParCorr
+    from tigramite.independence_tests.parcorr import ParCorr
     import tigramite.plotting as tp
 
+    from sklearn.linear_model import LinearRegression
+
     def lin_f(x): return x
  
     T = 1000
     
     links = {0: [((0, -1), 0.9, lin_f)],
              1: [((1, -1), 0.9, lin_f), ((0, 0), -0.8, lin_f)],
              2: [((2, -1), 0.9, lin_f), ((0, 0), 0.9, lin_f),  ((1, 0), 0.8, lin_f)],
-             3: [((3, -1), 0.9, lin_f), ((1, 0), 0.8, lin_f),  ((2, 0), -0.9, lin_f)]
+             # 3: [((3, -1), 0.9, lin_f), ((1, 0), 0.8, lin_f),  ((2, 0), -0.9, lin_f)]
              }
     # noises = [np.random.randn for j in links.keys()]
     data, nonstat = toys.structural_causal_process(links, T=T, noises=None, seed=7)
 
     missing_flag = 999
-    for i in range(0, 20):
-        data[i::100] = missing_flag
+    # for i in range(0, 20):
+    #     data[i::100] = missing_flag
 
     parents = toys._get_true_parent_neighbor_dict(links)
     dataframe = pp.DataFrame(data, missing_flag = missing_flag)
 
+
+    # model = LinearRegression()
+    # model.fit(X=np.random.randn(10,2), y=np.random.randn(10))
+    # model.predict(X=np.random.randn(10,2)[:,2:])
+    # sys.exit(0)
+
     med = LinearMediation(dataframe=dataframe, 
         data_transform=None)
-    med.fit_model(all_parents=parents, tau_max=10)
+    med.fit_model(all_parents=parents, tau_max=None)
     med.fit_model_bootstrap( 
                 boot_blocklength='cube_root',
                 seed = 42,
                 )
 
-    # print(med.get_val_matrix())
+    # # print(med.get_val_matrix())
 
-    print (med.get_ce(i=0, tau=0,  j=3))
-    print(med.get_bootstrap_of(function='get_ce', 
-        function_args={'i':0, 'tau':0,   'j':3}, conf_lev=0.9))
-
-    print (med.get_coeff(i=0, tau=-2, j=1))
-
-    print (med.get_ce_max(i=0, j=2))
-    print (med.get_ce(i=0, tau=0, j=3))
-    print (med.get_mce(i=0, tau=0, k=[2], j=3))
-    print (med.get_mce(i=0, tau=0, k=[1,2], j=3) - med.get_mce(i=0, tau=0, k=[1], j=3))
-    print (med.get_conditional_mce(i=0, tau=0, k=[2], notk=[1], j=3))
-    print (med.get_bootstrap_of('get_conditional_mce', {'i':0, 'tau':0, 'k':[2], 'notk':[1], 'j':3}))
+    # print (med.get_ce(i=0, tau=0,  j=3))
+    # print(med.get_bootstrap_of(function='get_ce', 
+    #     function_args={'i':0, 'tau':0,   'j':3}, conf_lev=0.9))
+
+    # print (med.get_coeff(i=0, tau=-2, j=1))
+
+    # print (med.get_ce_max(i=0, j=2))
+    # print (med.get_ce(i=0, tau=0, j=3))
+    # print (med.get_mce(i=0, tau=0, k=[2], j=3))
+    # print (med.get_mce(i=0, tau=0, k=[1,2], j=3) - med.get_mce(i=0, tau=0, k=[1], j=3))
+    # print (med.get_conditional_mce(i=0, tau=0, k=[2], notk=[1], j=3))
+    # print (med.get_bootstrap_of('get_conditional_mce', {'i':0, 'tau':0, 'k':[2], 'notk':[1], 'j':3}))
 
     # print(med.get_joint_ce(i=0, j=2))
     # print(med.get_joint_mce(i=0, j=2, k=1))
 
     # print(med.get_joint_ce_matrix(i=0, j=2))
 
     # i=0; tau=4; j=2
@@ -1933,21 +1973,21 @@
     # #                        selected_targets=[2],
     # #                        selected_links=None,
     # #                        steps_ahead=1,
     # #                        tau_max=1,
     # #                        pc_alpha=0.2,
     # #                        max_conds_dim=None,
     # #                        max_combinations=1)
-    # predictors = {0: [(0, -1)],
+    # predictors = {0: [], # [(0, -1)],
     #              1: [(1, -1), (0, -1)],
     #              2: [(2, -1), (1, 0)]}
     # pred.fit(target_predictors=predictors,
     #         selected_targets=None, tau_max=None, return_data=False)
 
-    # res = pred.predict(target=2,
+    # res = pred.predict(target=0,
     #             new_data=None,
     #             pred_params=None,
     #             cut_off='max_lag_or_tau_max')
 
     # print(data[:,2])
     # print(res)
```

### Comparing `tigramite-5.2.0.2/tigramite/pcmci.py` & `tigramite-5.2.1.6/tigramite/pcmci.py`

 * *Files 1% similar despite different names*

```diff
@@ -1970,16 +1970,16 @@
         links) under the standard assumptions of Causal Sufficiency,
         Faithfulness and the Markov condition.
 
         PCMCIplus estimates time-lagged and contemporaneous causal links by a
         four-step procedure:
 
         1.  Condition-selection (same as for PCMCI): For each variable
-        :math:`j`, estimate a *superset* of lagged parents :math:`\\widehat{
-        \\mathcal{B}}_t^-( X^j_t)` with the iterative PC1 algorithm,
+        :math:`j`, estimate a *superset* of lagged parents :math:`\widehat{
+        \mathcal{B}}_t^-( X^j_t)` with the iterative PC1 algorithm,
         implemented as ``run_pc_stable``. The condition-selection step
         reduces the dimensionality and avoids conditioning on irrelevant
         variables.
 
         2.   PC skeleton phase with contemporaneous conditions and *Momentary
         conditional independence* (MCI) tests: Iterate through subsets
         :math:`\\mathcal{S}` of contemporaneous adjacencies and conduct MCI
@@ -2056,57 +2056,14 @@
         :math:`\\widehat{ \\mathcal{B}}_t^-( X^j_t)`. For
         ``reset_lagged_links=True``, *all* lagged links are considered again,
         which improves detection power for lagged links, but also leads to
         larger runtimes.
 
         Further optional parameters are discussed in [5]_.
 
-        Examples
-        --------
-        >>> import numpy as np
-        >>> from tigramite.pcmci import PCMCI
-        >>> from tigramite.independence_tests import ParCorr
-        >>> import tigramite.data_processing as pp
-        >>> from tigramite.toymodels import structural_causal_processes as toys
-        >>> # Example process to play around with
-        >>> # Each key refers to a variable and the incoming links are supplied
-        >>> # as a list of format [((var, -lag), coeff, function), ...]
-        >>> def lin_f(x): return x
-        >>> links = {0: [((0, -1), 0.9, lin_f)],
-                     1: [((1, -1), 0.8, lin_f), ((0, -1), 0.8, lin_f)],
-                     2: [((2, -1), 0.7, lin_f), ((1, 0), 0.6, lin_f)],
-                     3: [((3, -1), 0.7, lin_f), ((2, 0), -0.5, lin_f)],
-                     }
-        >>> data, nonstat = toys.structural_causal_process(links,
-                            T=1000, seed=7)
-        >>> # Data must be array of shape (time, variables)
-        >>> print (data.shape)
-        (1000, 4)
-        >>> dataframe = pp.DataFrame(data)
-        >>> cond_ind_test = ParCorr()
-        >>> pcmci = PCMCI(dataframe=dataframe, cond_ind_test=cond_ind_test)
-        >>> results = pcmci.run_pcmciplus(tau_min=0, tau_max=2, pc_alpha=0.01)
-        >>> pcmci.print_results(results, alpha_level=0.01)
-            ## Significant links at alpha = 0.01:
-
-            Variable 0 has 1 link(s):
-                (0 -1): pval = 0.00000 | val =  0.676
-
-            Variable 1 has 2 link(s):
-                (1 -1): pval = 0.00000 | val =  0.602
-                (0 -1): pval = 0.00000 | val =  0.599
-
-            Variable 2 has 2 link(s):
-                (1  0): pval = 0.00000 | val =  0.486
-                (2 -1): pval = 0.00000 | val =  0.466
-
-            Variable 3 has 2 link(s):
-                (3 -1): pval = 0.00000 | val =  0.524
-                (2  0): pval = 0.00000 | val = -0.449 
-
         Parameters
         ----------
         selected_links : dict or None
             Deprecated, replaced by link_assumptions
         link_assumptions : dict
             Dictionary of form {j:{(i, -tau): link_type, ...}, ...} specifying
             assumptions about links. This initializes the graph with entries
@@ -3721,31 +3678,31 @@
         optimal_results = results[optimal_alpha]
         optimal_results['optimal_alpha'] = optimal_alpha
         return optimal_results
 
 
 
 if __name__ == '__main__':
-    from tigramite.independence_tests import ParCorr, CMIknn, ParCorrMult
+    from tigramite.independence_tests.parcorr import ParCorr
     import tigramite.data_processing as pp
     from tigramite.toymodels import structural_causal_processes as toys
     import tigramite.plotting as tp
     from matplotlib import pyplot as plt
 
     random_state = np.random.default_rng(seed=43)
     # Example process to play around with
     # Each key refers to a variable and the incoming links are supplied
     # as a list of format [((var, -lag), coeff, function), ...]
     def lin_f(x): return x
     def nonlin_f(x): return (x + 5. * x ** 2 * np.exp(-x ** 2 / 20.))
 
-    T = 2000
-    data = random_state.standar_normal((T, 4))
+    T = 20000
+    data = random_state.standard_normal((T, 4))
     # Simple sun
-    data[:,3] = np.sin(np.arange(T)*20/np.pi) + 0.1*random_state.standar_normal((T))
+    data[:,3] = np.sin(np.arange(T)*20/np.pi) + 0.1*random_state.standard_normal((T))
     c = 0.8
     for t in range(1, T):
         data[t, 0] += 0.4*data[t-1, 0] + 0.4*data[t-1, 1] + c*data[t-1,3]
         data[t, 1] += 0.5*data[t-1, 1] + c*data[t-1,3]
         data[t, 2] += 0.6*data[t-1, 2] + 0.3*data[t-2, 1] + c*data[t-1,3]
     dataframe = pp.DataFrame(data, var_names=[r'$X^0$', r'$X^1$', r'$X^2$', 'Sun'])
     # tp.plot_timeseries(dataframe); plt.show()
@@ -3776,15 +3733,16 @@
 
     print(link_assumptions)
     pcmci_parcorr = PCMCI(
         dataframe=dataframe, 
         cond_ind_test=parcorr,
         verbosity=2)
     results = pcmci_parcorr.run_pcmciplus(tau_max=tau_max, pc_alpha=0.01, 
-                                      link_assumptions=link_assumptions) #, alpha_level = 0.01)
+                                      # link_assumptions=link_assumptions
+                                      ) #, alpha_level = 0.01)
     print(results['graph'].shape)
     print(results['graph'][:,3,:])
     # Plot time series graph
     # tp.plot_time_series_graph(
     #     val_matrix=results['val_matrix'],
     #     graph=results['graph'],
     #     var_names=[r'$X^0$', r'$X^1$', r'$X^2$', 'Sun'],
```

### Comparing `tigramite-5.2.0.2/tigramite/pcmci_base.py` & `tigramite-5.2.1.6/tigramite/pcmci_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import itertools
 from collections import defaultdict
 from copy import deepcopy
 import numpy as np
 import scipy.stats
 import math
 
-
 class PCMCIbase():
     r"""PCMCI base class.
 
     Parameters
     ----------
     dataframe : data object
         This is the Tigramite dataframe object. Among others, it has the
@@ -771,131 +770,14 @@
         # Generate summary results
         summary_results = self.return_summary_results(results=window_results, 
                                                       conf_lev=conf_lev)
 
         return {'summary_results': summary_results, 
                 'window_results': window_results}
 
-    def run_bootstrap_of(self, method, method_args, 
-                        boot_samples=100,
-                        boot_blocklength=1,
-                        conf_lev=0.9, seed=None):
-        """Runs chosen method on bootstrap samples drawn from DataFrame.
-        
-        Bootstraps for tau=0 are drawn from [2xtau_max, ..., T] and all lagged
-        variables constructed in DataFrame.construct_array are consistently
-        shifted with respect to this bootsrap sample to ensure that lagged
-        relations in the bootstrap sample are preserved.
-
-        The function returns summary_results and all_results (containing the
-        individual bootstrap results). summary_results contains
-        val_matrix_mean and val_matrix_interval, the latter containing the
-        confidence bounds for conf_lev. If the method also returns a graph,
-        then 'most_frequent_links' containing the most frequent link outcome
-        (specific link type) in each entry of graph, as well
-        as 'link_frequency', containing the occurence frequency of the most
-        frequent link outcome, are returned. 
-
-        Assumes that method uses cond_ind_test.run_test() function with cut_off
-        = '2xtau_max'.
-
-        Parameters
-        ----------
-        method : str
-            Chosen method among valid functions in PCMCI.
-        method_args : dict
-            Arguments passed to method.
-        boot_samples : int
-            Number of bootstrap samples to draw.
-        boot_blocklength : int, optional (default: 1)
-            Block length for block-bootstrap.
-        conf_lev : float, optional (default: 0.9)
-            Two-sided confidence interval for summary results.
-        seed : int, optional(default = None)
-            Seed for RandomState (default_rng)
-
-        Returns
-        -------
-        Dictionary of summary results and results for every bootstrap sample.
-        """
-
-        valid_methods = ['run_pc_stable',
-                          'run_mci',
-                          'get_lagged_dependencies',
-                          'run_fullci',
-                          'run_bivci',
-                          'run_pcmci',
-                          'run_pcalg',
-                          'run_pcalg_non_timeseries_data',
-                          'run_pcmciplus',
-                          'run_lpcmci',
-                          ]
-
-        if method not in valid_methods:
-            raise ValueError("method must be one of %s" % str(valid_methods))
-
-        T = self.dataframe.largest_time_step
-
-        global_random_state = np.random.default_rng(seed)
-
-        # Extract tau_max to construct bootstrap draws
-        if 'tau_max' not in method_args:
-            raise ValueError("tau_max must be explicitely set in method_args.")
-        tau_max = method_args['tau_max']
-
-        if self.cond_ind_test.recycle_residuals:
-            # recycle_residuals clashes with bootstrap draws...
-            raise ValueError("cond_ind_test.recycle_residuals must be False.")
-
-        if self.verbosity > 0:
-            print("\n##\n## Running Bootstrap of %s " % method +
-                  "\n##\n" +
-                  "\nboot_samples = %s \n" % boot_samples +
-                  "\nboot_blocklength = %s \n" % boot_blocklength
-                  )
-
-        # Set bootstrap attribute to be passed to dataframe
-        self.dataframe.bootstrap = {}
-        self.dataframe.bootstrap['boot_blocklength'] = boot_blocklength
-
-        boot_results = {}
-        for b in range(boot_samples):
-            # Generate random state for this boot and set it in dataframe
-            # which will generate a draw with replacement
-            boot_seed = global_random_state.integers(0, boot_samples, 1)
-            boot_random_state = np.random.default_rng(boot_seed)
-            self.dataframe.bootstrap['random_state'] = boot_random_state
-
-            boot_res = getattr(self, method)(**method_args)
-
-            # Aggregate val_matrix and other arrays to new arrays with
-            # boot_samples as first dimension. Lists and other objects
-            # are stored in dictionary
-            for key in boot_res:
-                res_item = boot_res[key]
-                if type(res_item) is np.ndarray:
-                    if b == 0:
-                        boot_results[key] = np.empty((boot_samples,) 
-                                                     + res_item.shape,
-                                                     dtype=res_item.dtype) 
-                    boot_results[key][b] = res_item
-                else:
-                    if b == 0:
-                        boot_results[key] = {}
-                    boot_results[key][b] = res_item
-
-        # Generate summary results
-        summary_results = self.return_summary_results(results=boot_results, 
-                                                      conf_lev=conf_lev)
-
-        # Reset bootstrap to None
-        self.dataframe.bootstrap = None
-
-        return {'summary_results': summary_results, 
-                'boot_results': boot_results}
 
     @staticmethod
     def return_summary_results(results, conf_lev=0.9):
         """Return summary results for causal graphs.
 
         The function returns summary_results of an array of PCMCI(+) results.
         Summary_results contains val_matrix_mean and val_matrix_interval, the latter 
@@ -993,17 +875,14 @@
         links : dict
             Dictionary of form {0:{(0, -1): o-o, ...}, 1:{...}, ...}.
         """
         N = graph.shape[0]
 
         links = dict([(j, {}) for j in range(N)])
 
-        # if np.any(dag=='o-o') or np.any(dag=='x-x'):
-        #     raise ValueError("graph must be DAG.")
-
         for (i, j, tau) in zip(*np.where(graph!='')):
             links[j][(i, -tau)] = graph[i,j,tau]
 
         return links
 
     # @staticmethod
     def _dict_to_graph(self, links, tau_max=None):
@@ -1134,8 +1013,8 @@
         
         for j, links_j in link_assumptions_absent_link_means_no_knowledge.items():
             for (i, lag_i), link_ij in links_j.items():
                 if link_ij == "": 
                     del out[j][(i, lag_i)]
                 else:
                     out[j][(i, lag_i)] = link_ij
-        return out
+        return out
```

### Comparing `tigramite-5.2.0.2/tigramite/plotting.py` & `tigramite-5.2.1.6/tigramite/plotting.py`

 * *Files 3% similar despite different names*

```diff
@@ -1512,22 +1512,26 @@
     inner_edge_curved=False,
     inner_edge_style="solid",
     # network_lower_bound=0.2,
     network_left_bound=None,
     show_colorbar=True,
     special_nodes=None,
     autodep_sig_lags=None,
-    show_autodependency_lags=False
+    show_autodependency_lags=False,
+    transform='data',
 ):
     """Function to draw a network from networkx graph instance.
     Various attributes are used to specify the graph's properties.
     This function is just a beta-template for now that can be further
     customized.
     """
 
+    if transform == 'data':
+        transform = ax.transData
+
     from matplotlib.patches import FancyArrowPatch, Circle, Ellipse
 
     ax.spines["left"].set_color("none")
     ax.spines["right"].set_color("none")
     ax.spines["bottom"].set_color("none")
     ax.spines["top"].set_color("none")
     ax.set_xticks([])
@@ -1679,14 +1683,15 @@
                 clip_on=False,
                 patchA=n1,
                 patchB=n2,
                 shrinkA=7,
                 shrinkB=0,
                 zorder=-1,
                 capstyle="butt",
+                transform=transform,
             )
             ax.add_artist(e_p)
 
             e_p_back = FancyArrowPatch(
               coor2,
               coor1,
               arrowstyle=arrowstyle,
@@ -1700,14 +1705,15 @@
               clip_on=False,
               patchA=n2,
               patchB=n1,
               shrinkA=7,
               shrinkB=0,
               zorder=-1,
               capstyle="butt",
+              transform=transform,
             )  
             ax.add_artist(e_p_back)
 
         else:
             if arrowstyle == '-':
                 lw = 1*width
             else:
@@ -1744,16 +1750,17 @@
                 linestyle=linestyle,
                 color=facecolor,
                 clip_on=False,
                 patchA=n1,
                 patchB=n2,
                 shrinkA=0,
                 shrinkB=0,
-                zorder=-1,
+                # zorder=-1,
                 capstyle="butt",
+                transform=transform,
             )
             ax.add_artist(e_p)
 
         e_p_marker = FancyArrowPatch(
                 coor1,
                 coor2,
                 arrowstyle='-',
@@ -1767,363 +1774,425 @@
                 clip_on=False,
                 patchA=n1,
                 patchB=n2,
                 shrinkA=0,
                 shrinkB=0,
                 zorder=-10,
                 capstyle="butt",
+                transform=transform,
         )
         ax.add_artist(e_p_marker)
 
-        path = e_p_marker.get_path()
-        vertices = path.vertices.copy()
+        # marker_path = e_p_marker.get_path()
+        vertices = e_p_marker.get_path().vertices.copy()
+        # vertices = e_p_marker.get_verts()
+        # vertices = e_p_marker.get_path().to_polygons(transform=None)[0]
+        # print(vertices.shape)
         m, n = vertices.shape
 
         # print(vertices)
         start = vertices[0]
         end = vertices[-1]
 
         # This must be added to avoid rescaling of the plot, when no 'o'
         # or 'x' is added to the graph.
-        ax.scatter(*start, zorder=-10, alpha=0)
+        ax.scatter(*start, zorder=-10, alpha=0, transform=transform,)
 
         if outer_edge:
             if d.get("outer_edge_type") in ["o->", "o--"]:
                 circle_marker_start = ax.scatter(
                     *start,
                     marker="o",
                     s=marker_size,
                     facecolor="w",
                     edgecolor=facecolor,
                     zorder=1,
+                    transform=transform,
                 )
                 ax.add_collection(circle_marker_start)
             elif d.get("outer_edge_type") == "<-o":
                 circle_marker_end = ax.scatter(
                     *start,
                     marker="o",
                     s=marker_size,
                     facecolor="w",
                     edgecolor=facecolor,
                     zorder=1,
+                    transform=transform,
                 )
                 ax.add_collection(circle_marker_end)
             elif d.get("outer_edge_type") == "--o":
                 circle_marker_end = ax.scatter(
                     *end,
                     marker="o",
                     s=marker_size,
                     facecolor="w",
                     edgecolor=facecolor,
                     zorder=1,
+                    transform=transform,
                 )
                 ax.add_collection(circle_marker_end)
             elif d.get("outer_edge_type") in ["x--", "x->"]:
                 circle_marker_start = ax.scatter(
                     *start,
                     marker="X",
                     s=marker_size,
                     facecolor="w",
                     edgecolor=facecolor,
                     zorder=1,
+                    transform=transform,
                 )
                 ax.add_collection(circle_marker_start)
             elif d.get("outer_edge_type") in ["+--", "+->"]:
                 circle_marker_start = ax.scatter(
                     *start,
                     marker="P",
                     s=marker_size,
                     facecolor="w",
                     edgecolor=facecolor,
                     zorder=1,
+                    transform=transform,
                 )
                 ax.add_collection(circle_marker_start)
             elif d.get("outer_edge_type") == "<-x":
                 circle_marker_end = ax.scatter(
                     *start,
                     marker="X",
                     s=marker_size,
                     facecolor="w",
                     edgecolor=facecolor,
                     zorder=1,
+                    transform=transform,
                 )
                 ax.add_collection(circle_marker_end)
             elif d.get("outer_edge_type") == "<-+":
                 circle_marker_end = ax.scatter(
                     *start,
                     marker="P",
                     s=marker_size,
                     facecolor="w",
                     edgecolor=facecolor,
                     zorder=1,
+                    transform=transform,
                 )
                 ax.add_collection(circle_marker_end)
             elif d.get("outer_edge_type") == "--x":
                 circle_marker_end = ax.scatter(
                     *end,
                     marker="X",
                     s=marker_size,
                     facecolor="w",
                     edgecolor=facecolor,
                     zorder=1,
+                    transform=transform,
                 )
                 ax.add_collection(circle_marker_end)
             elif d.get("outer_edge_type") == "o-o":
                 circle_marker_start = ax.scatter(
                     *start,
                     marker="o",
                     s=marker_size,
                     facecolor="w",
                     edgecolor=facecolor,
                     zorder=1,
+                    transform=transform,
                 )
                 ax.add_collection(circle_marker_start)
                 circle_marker_end = ax.scatter(
                     *end,
                     marker="o",
                     s=marker_size,
                     facecolor="w",
                     edgecolor=facecolor,
                     zorder=1,
+                    transform=transform,
                 )
                 ax.add_collection(circle_marker_end)
             elif d.get("outer_edge_type") == "x-x":
                 circle_marker_start = ax.scatter(
                     *start,
                     marker="X",
                     s=marker_size,
                     facecolor="w",
                     edgecolor=facecolor,
                     zorder=1,
+                    transform=transform,
                 )
                 ax.add_collection(circle_marker_start)
                 circle_marker_end = ax.scatter(
                     *end,
                     marker="X",
                     s=marker_size,
                     facecolor="w",
                     edgecolor=facecolor,
                     zorder=1,
+                    transform=transform,
                 )
                 ax.add_collection(circle_marker_end)
             elif d.get("outer_edge_type") == "o-x":
                 circle_marker_start = ax.scatter(
                     *start,
                     marker="o",
                     s=marker_size,
                     facecolor="w",
                     edgecolor=facecolor,
                     zorder=1,
+                    transform=transform,
                 )
                 ax.add_collection(circle_marker_start)
                 circle_marker_end = ax.scatter(
                     *end,
                     marker="X",
                     s=marker_size,
                     facecolor="w",
                     edgecolor=facecolor,
                     zorder=1,
+                    transform=transform,
                 )
                 ax.add_collection(circle_marker_end)
             elif d.get("outer_edge_type") == "x-o":
                 circle_marker_start = ax.scatter(
                     *start,
                     marker="X",
                     s=marker_size,
                     facecolor="w",
                     edgecolor=facecolor,
                     zorder=1,
+                    transform=transform,
                 )
                 ax.add_collection(circle_marker_start)
                 circle_marker_end = ax.scatter(
                     *end,
                     marker="o",
                     s=marker_size,
                     facecolor="w",
                     edgecolor=facecolor,
                     zorder=1,
+                    transform=transform,
                 )
                 ax.add_collection(circle_marker_end)
 
         else:
             if d.get("inner_edge_type") in ["o->", "o--"]:
                 circle_marker_start = ax.scatter(
                     *start,
                     marker="o",
                     s=marker_size,
                     facecolor="w",
                     edgecolor=facecolor,
                     zorder=1,
+                    transform=transform,
                 )
                 ax.add_collection(circle_marker_start)
             elif d.get("inner_edge_type") == "<-o":
                 circle_marker_end = ax.scatter(
                     *start,
                     marker="o",
                     s=marker_size,
                     facecolor="w",
                     edgecolor=facecolor,
                     zorder=1,
+                    transform=transform,
                 )
                 ax.add_collection(circle_marker_end)
             elif d.get("inner_edge_type") == "--o":
                 circle_marker_end = ax.scatter(
                     *end,
                     marker="o",
                     s=marker_size,
                     facecolor="w",
                     edgecolor=facecolor,
                     zorder=1,
+                    transform=transform,
                 )
                 ax.add_collection(circle_marker_end)
             elif d.get("inner_edge_type") in ["x--", "x->"]:
                 circle_marker_start = ax.scatter(
                     *start,
                     marker="X",
                     s=marker_size,
                     facecolor="w",
                     edgecolor=facecolor,
                     zorder=1,
+                    transform=transform,
                 )
                 ax.add_collection(circle_marker_start)
             elif d.get("inner_edge_type") in ["+--", "+->"]:
                 circle_marker_start = ax.scatter(
                     *start,
                     marker="P",
                     s=marker_size,
                     facecolor="w",
                     edgecolor=facecolor,
                     zorder=1,
+                    transform=transform,
                 )
                 ax.add_collection(circle_marker_start)
             elif d.get("inner_edge_type") == "<-x":
                 circle_marker_end = ax.scatter(
                     *start,
                     marker="X",
                     s=marker_size,
                     facecolor="w",
                     edgecolor=facecolor,
                     zorder=1,
+                    transform=transform,
                 )
                 ax.add_collection(circle_marker_end)
             elif d.get("inner_edge_type") == "<-+":
                 circle_marker_end = ax.scatter(
                     *start,
                     marker="P",
                     s=marker_size,
                     facecolor="w",
                     edgecolor=facecolor,
                     zorder=1,
+                    transform=transform,
                 )
                 ax.add_collection(circle_marker_end)
             elif d.get("inner_edge_type") == "--x":
                 circle_marker_end = ax.scatter(
                     *end,
                     marker="X",
                     s=marker_size,
                     facecolor="w",
                     edgecolor=facecolor,
                     zorder=1,
+                    transform=transform,
                 )
                 ax.add_collection(circle_marker_end)
             elif d.get("inner_edge_type") == "o-o":
                 circle_marker_start = ax.scatter(
                     *start,
                     marker="o",
                     s=marker_size,
                     facecolor="w",
                     edgecolor=facecolor,
                     zorder=1,
+                    transform=transform,
                 )
                 ax.add_collection(circle_marker_start)
                 circle_marker_end = ax.scatter(
                     *end,
                     marker="o",
                     s=marker_size,
                     facecolor="w",
                     edgecolor=facecolor,
                     zorder=1,
+                    transform=transform,
                 )
                 ax.add_collection(circle_marker_end)
             elif d.get("inner_edge_type") == "x-x":
                 circle_marker_start = ax.scatter(
                     *start,
                     marker="X",
                     s=marker_size,
                     facecolor="w",
                     edgecolor=facecolor,
                     zorder=1,
+                    transform=transform,
                 )
                 ax.add_collection(circle_marker_start)
                 circle_marker_end = ax.scatter(
                     *end,
                     marker="X",
                     s=marker_size,
                     facecolor="w",
                     edgecolor=facecolor,
                     zorder=1,
+                    transform=transform,
                 )
                 ax.add_collection(circle_marker_end)
             elif d.get("inner_edge_type") == "o-x":
                 circle_marker_start = ax.scatter(
                     *start,
                     marker="o",
                     s=marker_size,
                     facecolor="w",
                     edgecolor=facecolor,
                     zorder=1,
+                    transform=transform,
                 )
                 ax.add_collection(circle_marker_start)
                 circle_marker_end = ax.scatter(
                     *end,
                     marker="X",
                     s=marker_size,
                     facecolor="w",
                     edgecolor=facecolor,
                     zorder=1,
+                    transform=transform,
                 )
                 ax.add_collection(circle_marker_end)
             elif d.get("inner_edge_type") == "x-o":
                 circle_marker_start = ax.scatter(
                     *start,
                     marker="X",
                     s=marker_size,
                     facecolor="w",
                     edgecolor=facecolor,
                     zorder=1,
+                    transform=transform,
                 )
                 ax.add_collection(circle_marker_start)
                 circle_marker_end = ax.scatter(
                     *end,
                     marker="o",
                     s=marker_size,
                     facecolor="w",
                     edgecolor=facecolor,
                     zorder=1,
+                    transform=transform,
                 )
                 ax.add_collection(circle_marker_end)
 
+
+
         if d["label"] is not None and outer_edge:
+            def closest_node(node, nodes):
+                nodes = np.asarray(nodes)
+                node = node.reshape(1, 2)
+                dist_2 = np.sum((nodes - node)**2, axis=1)
+                return np.argmin(dist_2)
+
             # Attach labels of lags
-            trans = None  # patch.get_transform()
-            path = e_p.get_path()
-            verts = path.to_polygons(trans)[0]
-            if len(verts) > 2:
-                label_vert = verts[1, :]
+            # trans = None  # patch.get_transform()
+            # path = e_p.get_path()
+            vertices = e_p_marker.get_path().vertices.copy()
+            verts = e_p.get_path().to_polygons(transform=None)[0]
+            # print(verts)
+            # print(verts.shape)
+            # print(vertices.shape)
+            # for num, vert in enumerate(verts):
+            #     ax.text(vert[0], vert[1], str(num), 
+            #         transform=transform,)
+            # ax.scatter(verts[:,0], verts[:,1])
+            # mid_point = np.array([(start[0] + end[0])/2., (start[1] + end[1])/2.])
+            # print(start, end, mid_point)
+            # ax.scatter(mid_point[0], mid_point[1], marker='x', 
+            #     s=100, zorder=10, transform=transform,)
+            closest_node = closest_node(vertices[int(len(vertices)/2.),:], verts)
+            # print(closest_node, verts[closest_node])
+            # ax.scatter(verts[closest_node][0], verts[closest_node][1], marker='x')
+
+            if len(vertices) > 2:
+                # label_vert = vertices[int(len(vertices)/2.),:] #verts[1, :]
+                label_vert = verts[closest_node] #verts[1, :]
                 l = d["label"]
                 string = str(l)
                 txt = ax.text(
                     label_vert[0],
                     label_vert[1],
                     string,
                     fontsize=link_label_fontsize,
                     verticalalignment="center",
                     horizontalalignment="center",
                     color="w",
                     zorder=1,
+                    transform=transform,
                 )
                 txt.set_path_effects(
                     [PathEffects.withStroke(linewidth=2, foreground="k")]
                 )
 
         return rad
 
@@ -2325,14 +2394,15 @@
                 pos[n],
                 width=node_sizes[: ring + 1].sum(axis=0)[n] * node_aspect,
                 height=node_sizes[: ring + 1].sum(axis=0)[n],
                 clip_on=False,
                 facecolor=color_here,
                 edgecolor=color_here,
                 zorder=-ring - 1 + 2,
+                transform=transform,
             )
 
             # else:
             #     if special_nodes is not None and n in special_nodes:
             #         color_here = special_nodes[n]
             #     else:
             #         color_here = colors[n]
@@ -2361,26 +2431,28 @@
                     pos[n][0],
                     pos[n][1],
                     node_labels[n],
                     fontsize=node_label_size,
                     horizontalalignment="center",
                     verticalalignment="center",
                     alpha=1.0,
-                    zorder=5.
+                    zorder=5.,
+                    transform=transform,
                 )
                 if show_autodependency_lags:
                     ax.text(
                         pos[n][0],
                         pos[n][1],
                         autodep_sig_lags[n],
                         fontsize=link_label_fontsize,
                         horizontalalignment="center",
                         verticalalignment="center",
                         color="black",
-                        zorder=5.
+                        zorder=5.,
+                        transform=transform,
                     )
 
     # Draw edges
     seen = {}
     for (u, v, d) in G.edges(data=True):
         if d.get("no_links"):
             d["inner_edge_alpha"] = 1e-8
@@ -2470,15 +2542,17 @@
         Array of val_matrix.shape specifying relative link width with maximum
         given by arrow_linewidth. If None, all links have same width.
     link_attribute : array-like, optional (default: None)
         String array of val_matrix.shape specifying link attributes.
     node_pos : dictionary, optional (default: None)
         Dictionary of node positions in axis coordinates of form
         node_pos = {'x':array of shape (N,), 'y':array of shape(N)}. These
-        coordinates could have been transformed before for basemap plots.
+        coordinates could have been transformed before for basemap plots. You can
+        also add a key 'transform':ccrs.PlateCarree() in order to plot graphs on 
+        a map using cartopy.
     arrow_linewidth : float, optional (default: 30)
         Linewidth.
     vmin_edges : float, optional (default: -1)
         Link colorbar scale lower bound.
     vmax_edges : float, optional (default: 1)
         Link colorbar scale upper bound.
     edge_ticks : float, optional (default: 0.4)
@@ -2740,14 +2814,18 @@
     if node_pos is None:
         pos = nx.circular_layout(deepcopy(G))
     else:
         pos = {}
         for i in range(N):
             pos[i] = (node_pos["x"][i], node_pos["y"][i])
 
+    if node_pos is not None and 'transform' in node_pos: 
+        transform = node_pos['transform']
+    else: transform = ax.transData
+
     if cmap_nodes is None:
         node_color = None
 
     node_rings = {
         0: {
             "sizes": None,
             "color_array": node_color,
@@ -2792,15 +2870,16 @@
         link_label_fontsize=link_label_fontsize,
         link_colorbar_label=link_colorbar_label,
         # network_lower_bound=network_lower_bound,
         show_colorbar=show_colorbar,
         # label_fraction=label_fraction,
         special_nodes=special_nodes,
         autodep_sig_lags=autodep_sig_lags,
-        show_autodependency_lags=show_autodependency_lags
+        show_autodependency_lags=show_autodependency_lags,
+        transform=transform
     )
 
     if save_name is not None:
         pyplot.savefig(save_name, dpi=300)
     else:
         return fig, ax
 
@@ -3719,15 +3798,17 @@
         Node colorbar label.
     link_width : array-like, optional (default: None)
         Array of val_matrix.shape specifying relative link width with maximum
         given by arrow_linewidth. If None, all links have same width.
     node_pos : dictionary, optional (default: None)
         Dictionary of node positions in axis coordinates of form
         node_pos = {'x':array of shape (N,), 'y':array of shape(N)}. These
-        coordinates could have been transformed before for basemap plots.
+        coordinates could have been transformed before for basemap plots. You can
+        also add a key 'transform':ccrs.PlateCarree() in order to plot graphs on 
+        a map using cartopy.
     arrow_linewidth : float, optional (default: 30)
         Linewidth.
     vmin_edges : float, optional (default: -1)
         Link colorbar scale lower bound.
     vmax_edges : float, optional (default: 1)
         Link colorbar scale upper bound.
     edge_ticks : float, optional (default: 0.4)
@@ -3892,14 +3973,18 @@
         pos = nx.circular_layout(deepcopy(G))
     #            pos = nx.spring_layout(deepcopy(G))
     else:
         pos = {}
         for i in range(N):
             pos[i] = (node_pos["x"][i], node_pos["y"][i])
 
+    if node_pos is not None and 'transform' in node_pos: 
+        transform = node_pos['transform']
+    else: transform = ax.transData
+
     node_rings = {
         0: {
             "sizes": None,
             "color_array": node_color,
             "cmap": cmap_nodes,
             "vmin": vmin_nodes,
             "vmax": vmax_nodes,
@@ -3938,14 +4023,15 @@
         curved_radius=curved_radius,
         label_fontsize=label_fontsize,
         link_label_fontsize=link_label_fontsize,
         link_colorbar_label=link_colorbar_label,
         # network_lower_bound=network_lower_bound,
         # label_fraction=label_fraction,
         # inner_edge_style=inner_edge_style
+        transform=transform
     )
 
     # fig.subplots_adjust(left=0.1, right=.9, bottom=.25, top=.95)
     # savestring = os.path.expanduser(save_name)
     if save_name is not None:
         pyplot.savefig(save_name)
     else:
@@ -4409,89 +4495,127 @@
     # sys.exit(0)
 
 
     # val_matrix = np.zeros((4, 4, 3))
 
     # Complete test case
     graph = np.zeros((3,3,2), dtype='<U3')
-    val_matrix = np.random.rand(*graph.shape)
+    val_matrix = 0.*np.random.rand(*graph.shape)
     val_matrix[:,:,0] = 0.2
     graph[:] = ""
-    graph[0, 1, 0] = "<-+"
-    graph[1, 0, 0] = "+->"
+    # graph[0, 1, 0] = "<-+"
+    # graph[1, 0, 0] = "+->"
     graph[0, 0, 1] = "-->"
     graph[1, 1, 1] = "-->"
 
     graph[0, 1, 1] = "+->"
-    graph[1, 0, 1] = "o-o"
+    # graph[1, 0, 1] = "o-o"
 
-    graph[1, 2, 0] = "<->"
-    graph[2, 1, 0] = "<->"
+    # graph[1, 2, 0] = "<->"
+    # graph[2, 1, 0] = "<->"
 
-    graph[0, 2, 0] = "x-x"
-    graph[2, 0, 0] = "x-x"
+    # graph[0, 2, 0] = "x-x"
+    # graph[2, 0, 0] = "x-x"
     nolinks = np.zeros(graph.shape)
     # nolinks[range(4), range(4), 1] = 1
 
-    fig, axes = pyplot.subplots(nrows=2, ncols=2, figsize=(6, 5))
-    label_space_left = 0.2
-    label_space_top = 0.
+    # graph = graph[:2, :2, :]
+
+    # fig, axes = pyplot.subplots(nrows=1, ncols=1, figsize=(6, 5))
+
+
+    # import cartopy.crs as ccrs
+    graph = np.ones((5, 5, 2), dtype='<U3')
+    graph[:] = ""
+    graph[3, :, 1] = '+->' 
+
+    # fig = pyplot.figure(figsize=(8, 6))
+    # fig = pyplot.figure(figsize=(10, 5))
+    # ax = fig.add_subplot(1, 1, 1, projection=ccrs.Mollweide())
+    # make the map global rather than have it zoom in to
+    # the extents of any plotted data
+    # ax.set_global()
+    # ax.stock_img()
+    # ax.coastlines()
+    # # ymax = 1.
+    # node_pos = {'x':np.linspace(0, ymax, graph.shape[0]), 'y':np.linspace(0, ymax, graph.shape[0]),}
+    # node_pos = {'x':np.array([10,-20,80,-50,80]),
+    #             'y':np.array([-10,70,60,-40,50]), 
+    #         'transform':ccrs.PlateCarree(), # t.PlateCarree()
+    #         }
+
+    plot_time_series_graph(graph=graph,
+        # fig_ax = (fig, ax),
+        # val_matrix=val_matrix,
+        # figsize=(5, 5),
+        # var_names = ['Var %s' %i for i in range(len(graph))],
+        # arrow_linewidth=6,
+        # label_space_left = label_space_left,
+        # label_space_top = label_space_top,
+        # # network_lower_bound=network_lower_bound,
+        save_name="tsg_test.pdf"
+        )
+    pyplot.tight_layout()
+
     # network_lower_bound = 0.
-    show_colorbar=True
+    # show_colorbar=True
     # plot_graph(graph=graph,
-    #     # fig_ax = (fig, axes),
-    #     val_matrix=val_matrix,
+    #     fig_ax = (fig, ax),
+    #     node_pos = node_pos,
+    #     node_size = 20,
+    #     # val_matrix=val_matrix,
     #     # figsize=(5, 5),
-    #     var_names = ['Var %s' %i for i in range(len(graph))],
+    #     # var_names = ['Var %s' %i for i in range(len(graph))],
     #     # arrow_linewidth=6,
     #     # label_space_left = label_space_left,
     #     # label_space_top = label_space_top,
     #     # # network_lower_bound=network_lower_bound,
-    #     # save_name="tsg_test.pdf"
+    #     save_name="tsg_test.pdf"
     #     )
-
+    # pyplot.tight_layout()
     # axes[0,0].scatter(np.random.rand(100), np.random.rand(100))
 
-    plot_graph(graph=graph,
-        fig_ax = (fig, axes[0,0]),
-        val_matrix=val_matrix,
-        # figsize=(5, 5),
-        var_names = ['Variable %s' %i for i in range(len(graph))],
-        arrow_linewidth=6,
-        # label_space_left = label_space_left,
-        # label_space_top = label_space_top,
-        # save_name="tsg_test.pdf"
-        )
-    plot_graph(graph=graph,
-        fig_ax = (fig, axes[0,1]),
-        val_matrix=val_matrix,
-        var_names = ['Var %s' %i for i in range(len(graph))],
-        arrow_linewidth=6,
-        # label_space_left = label_space_left,
-        # label_space_top = label_space_top,
-        )
-    plot_graph(graph=graph,
-        fig_ax = (fig, axes[1,0]),
-        val_matrix=val_matrix,
-        var_names = ['Var %s' %i for i in range(len(graph))],
-        arrow_linewidth=6,
-        # label_space_left = label_space_left,
-        # label_space_top = label_space_top,
-        )
-    plot_graph(graph=graph,
-        fig_ax = (fig, axes[1,1]),
-        val_matrix=val_matrix,
-        var_names = ['Var %s' %i for i in range(len(graph))],
-        arrow_linewidth=6,
-        # label_space_left = label_space_left,
-        # label_space_top = label_space_top,
-        )
-    # pyplot.subplots_adjust(wspace=0.3, hspace=0.2)
-    pyplot.tight_layout()
-    pyplot.savefig("test.pdf")
+    # plot_graph(graph=graph,
+    #     fig_ax = (fig, axes[0,0]),
+    #     val_matrix=val_matrix,
+    #     # figsize=(5, 5),
+    #     var_names = ['Variable %s' %i for i in range(len(graph))],
+    #     arrow_linewidth=6,
+    #     # label_space_left = label_space_left,
+    #     # label_space_top = label_space_top,
+    #     # save_name="tsg_test.pdf"
+    #     )
+    # plot_graph(graph=graph,
+    #     fig_ax = (fig, axes[0,1]),
+    #     val_matrix=val_matrix,
+    #     var_names = ['Var %s' %i for i in range(len(graph))],
+    #     arrow_linewidth=6,
+    #     # label_space_left = label_space_left,
+    #     # label_space_top = label_space_top,
+    #     )
+    # plot_graph(graph=graph,
+    #     fig_ax = (fig, axes[1,0]),
+    #     val_matrix=val_matrix,
+    #     var_names = ['Var %s' %i for i in range(len(graph))],
+    #     arrow_linewidth=6,
+    #     # label_space_left = label_space_left,
+    #     # label_space_top = label_space_top,
+    #     )
+    # plot_graph(graph=graph,
+    #     fig_ax = (fig, axes[1,1]),
+    #     val_matrix=val_matrix,
+    #     var_names = ['Var %s' %i for i in range(len(graph))],
+    #     arrow_linewidth=6,
+    #     n
+    #     # label_space_left = label_space_left,
+    #     # label_space_top = label_space_top,
+    #     )
+    # # pyplot.subplots_adjust(wspace=0.3, hspace=0.2)
+    # pyplot.tight_layout()
+    # pyplot.savefig("test.pdf")
 
     # def lin_f(x): return x
 
     # links_coeffs = {0: [((0, -1), 0.3, lin_f)], #, ((1, -1), 0.5, lin_f)],
     #             1: [((1, -1), 0.3, lin_f), ((0, 0), 0.7, lin_f), ((2, -1), 0.5, lin_f)],
     #             2: [],
     #             3: [((3, -1), 0., lin_f), ((2, 0), 0.6, lin_f),]
```

### Comparing `tigramite-5.2.0.2/tigramite/toymodels/structural_causal_processes.py` & `tigramite-5.2.1.6/tigramite/toymodels/structural_causal_processes.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.2/tigramite/toymodels/surrogate_generator.py` & `tigramite-5.2.1.6/tigramite/toymodels/surrogate_generator.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.2/tigramite.egg-info/PKG-INFO` & `tigramite-5.2.1.6/tigramite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigramite
-Version: 5.2.0.2
+Version: 5.2.1.6
 Summary: Tigramite causal inference for time series
 Home-page: https://github.com/jakobrunge/tigramite/
 Author: Jakob Runge
 Author-email: jakob@jakob-runge.com
 License: GNU General Public License v3.0
 Keywords: causal inference,causal discovery,prediction,time series
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tigramite-5.2.0.2/tigramite.egg-info/SOURCES.txt` & `tigramite-5.2.1.6/tigramite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

