# Comparing `tmp/wastimate-0.0.4.tar.gz` & `tmp/wastimate-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wastimate-0.0.4.tar", last modified: Fri Jun  2 20:20:35 2023, max compression
+gzip compressed data, was "wastimate-0.0.5.tar", last modified: Fri Jun  2 21:15:05 2023, max compression
```

## Comparing `wastimate-0.0.4.tar` & `wastimate-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 20:20:35.223761 wastimate-0.0.4/
--rw-rw-rw-   0        0        0      710 2023-06-02 20:20:35.200246 wastimate-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-02 20:20:35.223761 wastimate-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1198 2023-06-02 20:20:16.000000 wastimate-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:20:35.197246 wastimate-0.0.4/wastimate/
--rw-rw-rw-   0        0        0       24 2023-06-01 18:54:29.000000 wastimate-0.0.4/wastimate/__init__.py
--rw-rw-rw-   0        0        0    10504 2023-06-02 20:14:44.000000 wastimate-0.0.4/wastimate/framework.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:20:35.199246 wastimate-0.0.4/wastimate.egg-info/
--rw-rw-rw-   0        0        0      710 2023-06-02 20:20:35.000000 wastimate-0.0.4/wastimate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-06-02 20:20:35.000000 wastimate-0.0.4/wastimate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 20:20:35.000000 wastimate-0.0.4/wastimate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-02 20:20:35.000000 wastimate-0.0.4/wastimate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-02 20:20:35.000000 wastimate-0.0.4/wastimate.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 21:15:05.530466 wastimate-0.0.5/
+-rw-rw-rw-   0        0        0      710 2023-06-02 21:15:05.503770 wastimate-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-02 21:15:05.530466 wastimate-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1198 2023-06-02 21:14:55.000000 wastimate-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 21:15:05.501768 wastimate-0.0.5/wastimate/
+-rw-rw-rw-   0        0        0       24 2023-06-01 18:54:29.000000 wastimate-0.0.5/wastimate/__init__.py
+-rw-rw-rw-   0        0        0    10227 2023-06-02 21:14:31.000000 wastimate-0.0.5/wastimate/framework.py
+drwxrwxrwx   0        0        0        0 2023-06-02 21:15:05.503770 wastimate-0.0.5/wastimate.egg-info/
+-rw-rw-rw-   0        0        0      710 2023-06-02 21:15:05.000000 wastimate-0.0.5/wastimate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-06-02 21:15:05.000000 wastimate-0.0.5/wastimate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 21:15:05.000000 wastimate-0.0.5/wastimate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-02 21:15:05.000000 wastimate-0.0.5/wastimate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-02 21:15:05.000000 wastimate-0.0.5/wastimate.egg-info/top_level.txt
```

### Comparing `wastimate-0.0.4/PKG-INFO` & `wastimate-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: wastimate
-Version: 0.0.4
+Version: 0.0.5
 Summary: General framework for estimating waste quantities in time.
 Home-page: UNKNOWN
 Author: Hando Tohver
 Author-email: <handotohver@gmail.com>
 License: UNKNOWN
 Description: Package that offers a general framework for estimating radioactive waste quantities in time and enables the modeling of various waste management strategies.
 Keywords: python,radioactive waste,Modeling
```

### Comparing `wastimate-0.0.4/setup.py` & `wastimate-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4' 
+VERSION = '0.0.5' 
 DESCRIPTION = 'General framework for estimating waste quantities in time.'
 LONG_DESCRIPTION = 'Package that offers a general framework for estimating radioactive waste quantities in time and enables the modeling of various waste management strategies.'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="wastimate",
```

### Comparing `wastimate-0.0.4/wastimate/framework.py` & `wastimate-0.0.5/wastimate/framework.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         self.StateLinkFixed = [[0 for _ in range(len(self.Nodes))] for _ in range(len(self.Nodes))]
         self.StateLinkProp  = [[0 for _ in range(len(self.Nodes))] for _ in range(len(self.Nodes))]
         self.StateLinkRel   = [[1 for _ in range(len(self.Nodes))] for _ in range(len(self.Nodes))]
 
         for link in self.Links:
             link.timestep = self.Settings.timestep; link.reset()
             
-            if link.LinkType == "Fixed":
+            if link.LinkType == "fixed":
                 self.StateLinkFixed[self.NodeDict[link.HomeObj]][self.NodeDict[link.AwayObj]] = link.LinkState
             else:
                 self.StateLinkProp[self.NodeDict[link.HomeObj]][self.NodeDict[link.AwayObj]] = link.LinkState
 
             self.StateLinkRel[self.NodeDict[link.HomeObj]][self.NodeDict[link.AwayObj]] = link.VRFState
 
         # Convert rest of the connections to list of zeroes.
@@ -155,29 +155,28 @@
                 
                 if s == 0:
                     continue
             
                 for idxLink, link in enumerate(StateLinkFixed[idxState]):
                     
                     compensator = 0
-                    
                     if NewState[idxState] < link[timestep]:
-                        compensator = State[idxState] - link[timestep]
+                        compensator = NewState[idxState] - link[timestep]
         
                     NewState[idxState] -= (link[timestep] + compensator) * StateLinkRel[idxState][idxState][timestep]
                     NewState[idxLink]  += (link[timestep] + compensator) * StateLinkRel[idxState][idxLink][timestep]
                     
                 for idxLink, link in enumerate(StateLinkProp[idxState]):
                     
                     compensator = 0
-                    if NewState[idxState] < link[timestep] * NewState[idxState]:
-                        compensator = State[idxState] - link[timestep]  * State[idxState]
+                    if NewState[idxState] < link[timestep] * State[idxState]:
+                        compensator = NewState[idxState] - link[timestep]  * NewState[idxState]
         
-                    NewState[idxState] -= (link[timestep] * State[idxState] + compensator) * StateLinkRel[idxState][idxState][timestep]
-                    NewState[idxLink]  += (link[timestep] * State[idxState] + compensator) * StateLinkRel[idxState][idxLink][timestep]
+                    NewState[idxState] -= (link[timestep] * NewState[idxState] + compensator) * StateLinkRel[idxState][idxState][timestep]
+                    NewState[idxLink]  += (link[timestep] * NewState[idxState] + compensator) * StateLinkRel[idxState][idxLink][timestep]
             
             State = NewState[:]
             StateHistory.append(State[:])
         
         self.GlobalStateHistory.append(StateHistory)
 
 
@@ -202,16 +201,16 @@
         
         if timestep != False:
             self.Settings.timestep = temp_timestep
     
     def get_timeseries(self, Obj, batch)  -> "array containing the timeseries":
         return self.GlobalStateHistory[batch,:,self.NodeDict[Obj]]
     
-    def get_batch(self, Obj, timestep)  -> "array containing the timeseries":
-        return self.GlobalStateHistory[:,timestep,self.NodeDict[Obj]] #self.GlobalStateHistory[batch,:,self.NodeDict[Obj]]
+    def get_batch(self, Obj, timestep)  -> "array containing the batch":
+        return self.GlobalStateHistory[:,timestep,self.NodeDict[Obj]]
 
 
     def Plot(self, Obj, bin_number=100, filename="", colormap="jet", scale="lin"):
         
         image = []
         data = np.transpose(self.GlobalStateHistory[:,:,self.NodeDict[Obj]])
         min_value = np.min(data)
@@ -247,30 +246,22 @@
             plt.savefig(f'{filename}.png')
         else:
             plt.show()
 
 
 if __name__ == "__main__":
 
-    Node1 = Node(sc.uniform(loc=1, scale=2))
-    Node2 = Node(sc.uniform(loc=0, scale=2))
+    Node1 = Node(sc.uniform(loc=3, scale=2))
+    Node2 = Node(sc.uniform(loc=0, scale=0))
     Node3 = Node(sc.uniform(loc=0, scale=0))
 
-    Link12 = Link(Node1, Node2, sc.uniform(loc=0.03, scale=0.05), LinkType="Var")
-    Link23 = Link(Node2, Node3, sc.uniform(loc=0.03, scale=0.05), LinkType="Var")
-    Link31 = Link(Node3, Node1, sc.uniform(loc=0.05, scale=0.05), LinkType="Fixed")
+    Link12 = Link(Node1, Node2, sc.uniform(loc=0.05, scale=0.07), LinkType="fixed")
+    Link23 = Link(Node2, Node3, sc.uniform(loc=0.03, scale=0.05), LinkType="var")
+    Link31 = Link(Node3, Node1, sc.uniform(loc=0.04, scale=0.01), LinkType="var")
 
     settings = Settings()
-    settings.timestep = 100
     settings.batches = 1000
 
     verse = Universe() + Node1 + Node2 + Node3 + Link12 + Link23 + Link31 + settings
     verse.simulate(100)
-
-    verse = verse - Link12
-    verse.simulate(100)
-
-    verse = verse + Link12
-    Link12.Dist = sc.uniform(loc=0.05, scale=0.2); Link12.LinkType="Var"
-    verse.simulate(100)
-
-    verse.Plot(Node1, scale="log")
+    
+    verse.Plot(Node3, scale="log")
```

### Comparing `wastimate-0.0.4/wastimate.egg-info/PKG-INFO` & `wastimate-0.0.5/wastimate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: wastimate
-Version: 0.0.4
+Version: 0.0.5
 Summary: General framework for estimating waste quantities in time.
 Home-page: UNKNOWN
 Author: Hando Tohver
 Author-email: <handotohver@gmail.com>
 License: UNKNOWN
 Description: Package that offers a general framework for estimating radioactive waste quantities in time and enables the modeling of various waste management strategies.
 Keywords: python,radioactive waste,Modeling
```

