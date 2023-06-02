# Comparing `tmp/quera-ahs-utils-0.4.1.tar.gz` & `tmp/quera-ahs-utils-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quera-ahs-utils-0.4.1.tar", last modified: Mon May  1 15:41:56 2023, max compression
+gzip compressed data, was "quera-ahs-utils-0.4.2.tar", last modified: Fri Jun  2 01:01:08 2023, max compression
```

## Comparing `quera-ahs-utils-0.4.1.tar` & `quera-ahs-utils-0.4.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:41:56.580983 quera-ahs-utils-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-05-01 15:41:08.000000 quera-ahs-utils-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-01 15:41:56.580983 quera-ahs-utils-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-01 15:41:08.000000 quera-ahs-utils-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-01 15:41:08.000000 quera-ahs-utils-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 15:41:56.580983 quera-ahs-utils-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:41:56.576982 quera-ahs-utils-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:41:56.580983 quera-ahs-utils-0.4.1/src/quera_ahs_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-01 15:41:08.000000 quera-ahs-utils-0.4.1/src/quera_ahs_utils/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-05-01 15:41:08.000000 quera-ahs-utils-0.4.1/src/quera_ahs_utils/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-05-01 15:41:08.000000 quera-ahs-utils-0.4.1/src/quera_ahs_utils/ir.py
--rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-05-01 15:41:08.000000 quera-ahs-utils-0.4.1/src/quera_ahs_utils/parallelize.py
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-05-01 15:41:08.000000 quera-ahs-utils-0.4.1/src/quera_ahs_utils/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:41:56.580983 quera-ahs-utils-0.4.1/src/quera_ahs_utils/quera_ir/
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-01 15:41:08.000000 quera-ahs-utils-0.4.1/src/quera_ahs_utils/quera_ir/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-05-01 15:41:08.000000 quera-ahs-utils-0.4.1/src/quera_ahs_utils/quera_ir/task_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-05-01 15:41:08.000000 quera-ahs-utils-0.4.1/src/quera_ahs_utils/quera_ir/task_specification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:41:56.580983 quera-ahs-utils-0.4.1/src/quera_ahs_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-01 15:41:56.000000 quera-ahs-utils-0.4.1/src/quera_ahs_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-01 15:41:56.000000 quera-ahs-utils-0.4.1/src/quera_ahs_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 15:41:56.000000 quera-ahs-utils-0.4.1/src/quera_ahs_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-01 15:41:56.000000 quera-ahs-utils-0.4.1/src/quera_ahs_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-01 15:41:56.000000 quera-ahs-utils-0.4.1/src/quera_ahs_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:41:56.580983 quera-ahs-utils-0.4.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-05-01 15:41:08.000000 quera-ahs-utils-0.4.1/test/test_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-01 15:41:08.000000 quera-ahs-utils-0.4.1/test/test_ir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-01 15:41:08.000000 quera-ahs-utils-0.4.1/test/test_parallelize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-01 15:41:08.000000 quera-ahs-utils-0.4.1/test/test_plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:01:08.304256 quera-ahs-utils-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-06-02 01:00:24.000000 quera-ahs-utils-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-02 01:01:08.304256 quera-ahs-utils-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-06-02 01:00:24.000000 quera-ahs-utils-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-02 01:00:24.000000 quera-ahs-utils-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 01:01:08.304256 quera-ahs-utils-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:01:08.300256 quera-ahs-utils-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:01:08.304256 quera-ahs-utils-0.4.2/src/quera_ahs_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-02 01:00:24.000000 quera-ahs-utils-0.4.2/src/quera_ahs_utils/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-06-02 01:00:24.000000 quera-ahs-utils-0.4.2/src/quera_ahs_utils/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-06-02 01:00:24.000000 quera-ahs-utils-0.4.2/src/quera_ahs_utils/ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-06-02 01:00:24.000000 quera-ahs-utils-0.4.2/src/quera_ahs_utils/parallelize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-06-02 01:00:24.000000 quera-ahs-utils-0.4.2/src/quera_ahs_utils/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:01:08.304256 quera-ahs-utils-0.4.2/src/quera_ahs_utils/quera_ir/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-02 01:00:24.000000 quera-ahs-utils-0.4.2/src/quera_ahs_utils/quera_ir/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-06-02 01:00:24.000000 quera-ahs-utils-0.4.2/src/quera_ahs_utils/quera_ir/task_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-06-02 01:00:24.000000 quera-ahs-utils-0.4.2/src/quera_ahs_utils/quera_ir/task_specification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:01:08.304256 quera-ahs-utils-0.4.2/src/quera_ahs_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-02 01:01:08.000000 quera-ahs-utils-0.4.2/src/quera_ahs_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-02 01:01:08.000000 quera-ahs-utils-0.4.2/src/quera_ahs_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 01:01:08.000000 quera-ahs-utils-0.4.2/src/quera_ahs_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-02 01:01:08.000000 quera-ahs-utils-0.4.2/src/quera_ahs_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-02 01:01:08.000000 quera-ahs-utils-0.4.2/src/quera_ahs_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:01:08.304256 quera-ahs-utils-0.4.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-02 01:00:24.000000 quera-ahs-utils-0.4.2/test/test_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-02 01:00:24.000000 quera-ahs-utils-0.4.2/test/test_ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-02 01:00:24.000000 quera-ahs-utils-0.4.2/test/test_parallelize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-02 01:00:24.000000 quera-ahs-utils-0.4.2/test/test_plotting.py
```

### Comparing `quera-ahs-utils-0.4.1/LICENSE` & `quera-ahs-utils-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.1/PKG-INFO` & `quera-ahs-utils-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quera-ahs-utils
-Version: 0.4.1
+Version: 0.4.2
 Summary: Various tools to interact with Braket Analog Hamiltonian Computing
 Author-email: Phillip Weinberg <pweinberg@quera.com>, John Long <jlong@quera.com>
 Maintainer-email: Phillip Weinberg <pweinberg@quera.com>, John Long <jlong@quera.com>
 Project-URL: Homepage, https://github.com/QuEraComputing/quera-ahs-utils
 Project-URL: Bug Tracker, https://github.com/QuEraComputing/quera-ahs-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `quera-ahs-utils-0.4.1/README.md` & `quera-ahs-utils-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.1/pyproject.toml` & `quera-ahs-utils-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quera-ahs-utils"
-version = "0.4.1"
+version = "0.4.2"
 authors = [
   { name="Phillip Weinberg", email="pweinberg@quera.com" },
   { name="John Long", email="jlong@quera.com" }
 ]
 maintainers = [
   { name="Phillip Weinberg", email="pweinberg@quera.com" },
   { name="John Long", email="jlong@quera.com" }
@@ -30,8 +30,8 @@
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/QuEraComputing/quera-ahs-utils"
 "Bug Tracker" = "https://github.com/QuEraComputing/quera-ahs-utils/issues"
 
 [tool.setuptools.packages.find]
-where = ["src"]
+where = ["src"]
```

### Comparing `quera-ahs-utils-0.4.1/src/quera_ahs_utils/analysis.py` & `quera-ahs-utils-0.4.2/src/quera_ahs_utils/analysis.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.1/src/quera_ahs_utils/drive.py` & `quera-ahs-utils-0.4.2/src/quera_ahs_utils/drive.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.1/src/quera_ahs_utils/ir.py` & `quera-ahs-utils-0.4.2/src/quera_ahs_utils/ir.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.1/src/quera_ahs_utils/parallelize.py` & `quera-ahs-utils-0.4.2/src/quera_ahs_utils/parallelize.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.1/src/quera_ahs_utils/plotting.py` & `quera-ahs-utils-0.4.2/src/quera_ahs_utils/plotting.py`

 * *Files 21% similar despite different names*

```diff
@@ -244,7 +244,83 @@
     plt.colorbar(sm, ax=ax, label=cbar_label)
     
     if return_fig:
         return fig,ax
     else:
         return None,ax
 
+
+
+def plot_task(task,show_register=False):
+    rabi_times = np.array(task.hamiltonian.amplitude.time_series.times())/1e-6
+    rabi_vals  = np.array(task.hamiltonian.amplitude.time_series.values())/1e6
+    
+    phase_times = np.array(task.hamiltonian.phase.time_series.times())/1e-6
+    phase_vals  = np.array(task.hamiltonian.phase.time_series.values())
+    
+    detuning_times = np.array(task.hamiltonian.detuning.time_series.times())/1e-6
+    detuning_vals  = np.array(task.hamiltonian.detuning.time_series.values())/1e6
+    
+    pos_filled = np.array([atom.coordinate for atom in task.register if atom.site_type == SiteType.FILLED])*1e6
+    pos_empty = np.array([atom.coordinate for atom in task.register if atom.site_type == SiteType.VACANT])*1e6
+    
+    if show_register==False:
+        fig = plt.figure(figsize=(8,8))
+        ax = plt.subplot(3,1,1)
+        plt.plot(rabi_times,rabi_vals,"k.-",linewidth=2)
+        plt.fill_between(rabi_times,rabi_vals,color="#C2477F",alpha=0.2)
+        ax.axis([min(rabi_times) - 0.05*max(rabi_times),max(rabi_times)*1.05,ax.axis()[2],ax.axis()[3]])
+        ax.set_yticks(np.linspace(0,15,4))
+        plt.ylabel("$\\Omega(t)$ (rad/usec)")
+        #xlabel("Time along protocol (sec)")
+        
+        ax = plt.subplot(3,1,2)
+        plt.plot(detuning_times,detuning_vals,"k.-",linewidth=2)
+        plt.fill_between(detuning_times,detuning_vals,color="#55de79",alpha=0.2)
+        plt.axis([min(detuning_times) - 0.05*max(detuning_times),max(rabi_times)*1.05,ax.axis()[2],ax.axis()[3]])
+        plt.ylabel("$\\Delta(t)$ (rad/usec)")
+        #xlabel("Time along protocol (sec)")
+        
+        ax = plt.subplot(3,1,3)
+        for ind in range(len(phase_vals)-1):
+            plt.plot([phase_times[ind],phase_times[ind+1]] , [phase_vals[ind], phase_vals[ind]],'k.-',linewidth=2)
+        ax.axis([min(phase_times) - 0.05*max(phase_times),max(phase_times)*1.05,ax.axis()[2],ax.axis()[3]])
+        plt.ylabel("$\\phi(t)$ (rad)")
+        plt.xlabel("Time along protocol (usec)")
+        
+        plt.subplots_adjust(left=0.175)
+    else:
+        fig = plt.figure(figsize=(16,8))
+        ax = plt.subplot(3,2,1)
+        ax.set_yticks(np.linspace(0,15,4))
+        plt.plot(rabi_times,rabi_vals,"k.-",linewidth=2)
+        plt.fill_between(rabi_times,rabi_vals,color="#C2477F",alpha=0.2)
+        plt.axis([min(rabi_times) - 0.05*max(rabi_times),max(rabi_times)*1.05,plt.axis()[2],plt.axis()[3]])
+        plt.ylabel("$\\Omega(t)$ (rad/usec)")
+        #xlabel("Time along protocol (sec)")
+        
+        ax = plt.subplot(3,2,3)
+        plt.plot(detuning_times,detuning_vals,"k.-",linewidth=2)
+        plt.fill_between(detuning_times,detuning_vals,color="#55de79",alpha=0.2)
+        ax.axis([min(detuning_times) - 0.05*max(detuning_times),max(rabi_times)*1.05,ax.axis()[2],ax.axis()[3]])
+        plt.ylabel("$\\Delta(t)$ (rad/usec)")
+        #xlabel("Time along protocol (sec)")
+        
+        ax = plt.subplot(3,2,5)
+        for ind in range(len(phase_vals)-1):
+            plt.plot([phase_times[ind],phase_times[ind+1]] , [phase_vals[ind], phase_vals[ind]],'k.-',linewidth=2)
+        ax.axis([min(phase_times) - 0.05*max(phase_times),max(phase_times)*1.05,ax.axis()[2],ax.axis()[3]])
+        plt.ylabel("$\\phi(t)$ (rad)")
+        plt.xlabel("Time along protocol (usec)")
+        
+        ax = plt.subplot(1,2,2)
+        #axis([-1,76,-1,76])
+        ax.axis([-5,80,-5,80])
+        
+        
+        if len(pos_filled)>0:
+            plt.scatter(pos_filled[:,0],pos_filled[:,1],color="#6437FF",s=200)
+        if len(pos_empty)>0:
+            plt.scatter(pos_empty[:,0],pos_empty[:,1],color="grey",s=200)
+        ax.set_aspect("equal")
+        
+        plt.subplots_adjust(left=0.175/2)
```

### Comparing `quera-ahs-utils-0.4.1/src/quera_ahs_utils/quera_ir/capabilities.py` & `quera-ahs-utils-0.4.2/src/quera_ahs_utils/quera_ir/capabilities.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.1/src/quera_ahs_utils/quera_ir/task_results.py` & `quera-ahs-utils-0.4.2/src/quera_ahs_utils/quera_ir/task_results.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.1/src/quera_ahs_utils/quera_ir/task_specification.py` & `quera-ahs-utils-0.4.2/src/quera_ahs_utils/quera_ir/task_specification.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.1/src/quera_ahs_utils.egg-info/PKG-INFO` & `quera-ahs-utils-0.4.2/src/quera_ahs_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quera-ahs-utils
-Version: 0.4.1
+Version: 0.4.2
 Summary: Various tools to interact with Braket Analog Hamiltonian Computing
 Author-email: Phillip Weinberg <pweinberg@quera.com>, John Long <jlong@quera.com>
 Maintainer-email: Phillip Weinberg <pweinberg@quera.com>, John Long <jlong@quera.com>
 Project-URL: Homepage, https://github.com/QuEraComputing/quera-ahs-utils
 Project-URL: Bug Tracker, https://github.com/QuEraComputing/quera-ahs-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `quera-ahs-utils-0.4.1/src/quera_ahs_utils.egg-info/SOURCES.txt` & `quera-ahs-utils-0.4.2/src/quera_ahs_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.1/test/test_drive.py` & `quera-ahs-utils-0.4.2/test/test_drive.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.1/test/test_ir.py` & `quera-ahs-utils-0.4.2/test/test_ir.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.1/test/test_parallelize.py` & `quera-ahs-utils-0.4.2/test/test_parallelize.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.4.1/test/test_plotting.py` & `quera-ahs-utils-0.4.2/test/test_plotting.py`

 * *Files identical despite different names*

