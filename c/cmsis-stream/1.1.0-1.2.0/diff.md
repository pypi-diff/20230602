# Comparing `tmp/cmsis_stream-1.1.0-py3-none-any.whl.zip` & `tmp/cmsis_stream-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 66893 bytes, number of entries: 50
+Zip file size: 68003 bytes, number of entries: 53
 -rw-rw-rw-  2.0 fat      298 b- defN 23-May-11 12:29 cmsis_stream/__init__.py
+-rw-rw-rw-  2.0 fat      546 b- defN 23-Jun-02 06:34 cmsis_stream/cmsis_stream.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-11 12:29 cmsis_stream/cg/__init__.py
 -rw-rw-rw-  2.0 fat     7448 b- defN 23-May-11 12:29 cmsis_stream/cg/types.py
 -rw-rw-rw-  2.0 fat     1925 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/CFFT.py
 -rw-rw-rw-  2.0 fat     1990 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/Duplicate.py
 -rw-rw-rw-  2.0 fat     1930 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/ICFFT.py
 -rw-rw-rw-  2.0 fat     1645 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/InterleavedStereoToMono.py
 -rw-rw-rw-  2.0 fat     1974 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/MFCC.py
@@ -20,33 +21,35 @@
 -rw-rw-rw-  2.0 fat     2916 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/host/VHT.py
 -rw-rw-rw-  2.0 fat      871 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/host/VHTCGSTATIC.py
 -rw-rw-rw-  2.0 fat     2029 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/host/WavSink.py
 -rw-rw-rw-  2.0 fat     2092 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/host/WavSource.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/host/__init__.py
 -rw-rw-rw-  2.0 fat     4018 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/host/message.py
 -rw-rw-rw-  2.0 fat      118 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/__init__.py
--rw-rw-rw-  2.0 fat     3194 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/ccode.py
--rw-rw-rw-  2.0 fat     5086 b- defN 23-Jun-01 08:50 cmsis_stream/cg/scheduler/config.py
--rw-rw-rw-  2.0 fat    43229 b- defN 23-May-31 09:41 cmsis_stream/cg/scheduler/description.py
+-rw-rw-rw-  2.0 fat     1691 b- defN 23-Jun-02 05:41 cmsis_stream/cg/scheduler/args.py
+-rw-rw-rw-  2.0 fat     3018 b- defN 23-Jun-02 05:04 cmsis_stream/cg/scheduler/ccode.py
+-rw-rw-rw-  2.0 fat     6628 b- defN 23-Jun-02 06:51 cmsis_stream/cg/scheduler/config.py
+-rw-rw-rw-  2.0 fat    41560 b- defN 23-Jun-02 05:04 cmsis_stream/cg/scheduler/description.py
 -rw-rw-rw-  2.0 fat     1784 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/graphviz.py
--rw-rw-rw-  2.0 fat    31509 b- defN 23-May-31 09:44 cmsis_stream/cg/scheduler/node.py
+-rw-rw-rw-  2.0 fat    29225 b- defN 23-Jun-02 07:49 cmsis_stream/cg/scheduler/node.py
 -rw-rw-rw-  2.0 fat     1796 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/pythoncode.py
--rw-rw-rw-  2.0 fat     8319 b- defN 23-May-31 13:14 cmsis_stream/cg/scheduler/standard.py
--rw-rw-rw-  2.0 fat    13936 b- defN 23-Jun-01 09:34 cmsis_stream/cg/scheduler/templates/GenericNodes.h
--rw-rw-rw-  2.0 fat      419 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/templates/cmsis.cpp
--rw-rw-rw-  2.0 fat      267 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/templates/cmsis.py
--rw-rw-rw-  2.0 fat      658 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/templates/cmsisCheck.cpp
+-rw-rw-rw-  2.0 fat     8260 b- defN 23-Jun-01 13:08 cmsis_stream/cg/scheduler/standard.py
+-rw-rw-rw-  2.0 fat    14002 b- defN 23-Jun-02 08:01 cmsis_stream/cg/scheduler/templates/GenericNodes.h
+-rw-rw-rw-  2.0 fat     2006 b- defN 23-Jun-02 08:01 cmsis_stream/cg/scheduler/templates/cg_status.h
+-rw-rw-rw-  2.0 fat      431 b- defN 23-Jun-01 13:09 cmsis_stream/cg/scheduler/templates/cmsis.cpp
+-rw-rw-rw-  2.0 fat      279 b- defN 23-Jun-02 07:46 cmsis_stream/cg/scheduler/templates/cmsis.py
+-rw-rw-rw-  2.0 fat      674 b- defN 23-Jun-01 13:13 cmsis_stream/cg/scheduler/templates/cmsisCheck.cpp
 -rw-rw-rw-  2.0 fat      297 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/templates/cmsisNode.cpp
--rw-rw-rw-  2.0 fat     1226 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/templates/code.cpp
--rw-rw-rw-  2.0 fat      983 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/templates/code.h
--rw-rw-rw-  2.0 fat     2192 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/templates/code.py
--rw-rw-rw-  2.0 fat     4534 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/templates/codeArray.cpp
--rw-rw-rw-  2.0 fat     2960 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/templates/codeSwitch.cpp
--rw-rw-rw-  2.0 fat     2464 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/templates/commonc.cpp
+-rw-rw-rw-  2.0 fat     1232 b- defN 23-Jun-02 07:49 cmsis_stream/cg/scheduler/templates/code.cpp
+-rw-rw-rw-  2.0 fat     1111 b- defN 23-Jun-02 05:31 cmsis_stream/cg/scheduler/templates/code.h
+-rw-rw-rw-  2.0 fat     2199 b- defN 23-Jun-02 07:49 cmsis_stream/cg/scheduler/templates/code.py
+-rw-rw-rw-  2.0 fat     3185 b- defN 23-Jun-01 11:18 cmsis_stream/cg/scheduler/templates/codeSwitch.cpp
+-rw-rw-rw-  2.0 fat     4482 b- defN 23-Jun-02 05:31 cmsis_stream/cg/scheduler/templates/commonc.cpp
 -rw-rw-rw-  2.0 fat     1051 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/templates/defineConfig.h
 -rw-rw-rw-  2.0 fat     4848 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/templates/dot_template.dot
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-01 09:34 cmsis_stream-1.1.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     2494 b- defN 23-Jun-01 09:34 cmsis_stream-1.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-01 09:34 cmsis_stream-1.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 23-Jun-01 09:34 cmsis_stream-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     4682 b- defN 23-Jun-01 09:34 cmsis_stream-1.1.0.dist-info/RECORD
-50 files, 199627 bytes uncompressed, 59271 bytes compressed:  70.3%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-02 08:01 cmsis_stream-1.2.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     3109 b- defN 23-Jun-02 08:01 cmsis_stream-1.2.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-02 08:01 cmsis_stream-1.2.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       59 b- defN 23-Jun-02 08:01 cmsis_stream-1.2.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Jun-02 08:01 cmsis_stream-1.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     4955 b- defN 23-Jun-02 08:01 cmsis_stream-1.2.0.dist-info/RECORD
+53 files, 200127 bytes uncompressed, 59945 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: cmsis_stream/__init__.py
 Comment: 
 
+Filename: cmsis_stream/cmsis_stream.py
+Comment: 
+
 Filename: cmsis_stream/cg/__init__.py
 Comment: 
 
 Filename: cmsis_stream/cg/types.py
 Comment: 
 
 Filename: cmsis_stream/cg/nodes/CFFT.py
@@ -69,14 +72,17 @@
 
 Filename: cmsis_stream/cg/nodes/host/message.py
 Comment: 
 
 Filename: cmsis_stream/cg/scheduler/__init__.py
 Comment: 
 
+Filename: cmsis_stream/cg/scheduler/args.py
+Comment: 
+
 Filename: cmsis_stream/cg/scheduler/ccode.py
 Comment: 
 
 Filename: cmsis_stream/cg/scheduler/config.py
 Comment: 
 
 Filename: cmsis_stream/cg/scheduler/description.py
@@ -93,14 +99,17 @@
 
 Filename: cmsis_stream/cg/scheduler/standard.py
 Comment: 
 
 Filename: cmsis_stream/cg/scheduler/templates/GenericNodes.h
 Comment: 
 
+Filename: cmsis_stream/cg/scheduler/templates/cg_status.h
+Comment: 
+
 Filename: cmsis_stream/cg/scheduler/templates/cmsis.cpp
 Comment: 
 
 Filename: cmsis_stream/cg/scheduler/templates/cmsis.py
 Comment: 
 
 Filename: cmsis_stream/cg/scheduler/templates/cmsisCheck.cpp
@@ -114,38 +123,38 @@
 
 Filename: cmsis_stream/cg/scheduler/templates/code.h
 Comment: 
 
 Filename: cmsis_stream/cg/scheduler/templates/code.py
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/codeArray.cpp
-Comment: 
-
 Filename: cmsis_stream/cg/scheduler/templates/codeSwitch.cpp
 Comment: 
 
 Filename: cmsis_stream/cg/scheduler/templates/commonc.cpp
 Comment: 
 
 Filename: cmsis_stream/cg/scheduler/templates/defineConfig.h
 Comment: 
 
 Filename: cmsis_stream/cg/scheduler/templates/dot_template.dot
 Comment: 
 
-Filename: cmsis_stream-1.1.0.dist-info/LICENSE.txt
+Filename: cmsis_stream-1.2.0.dist-info/LICENSE.txt
+Comment: 
+
+Filename: cmsis_stream-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: cmsis_stream-1.1.0.dist-info/METADATA
+Filename: cmsis_stream-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: cmsis_stream-1.1.0.dist-info/WHEEL
+Filename: cmsis_stream-1.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: cmsis_stream-1.1.0.dist-info/top_level.txt
+Filename: cmsis_stream-1.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: cmsis_stream-1.1.0.dist-info/RECORD
+Filename: cmsis_stream-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cmsis_stream/cg/scheduler/ccode.py

```diff
@@ -43,23 +43,19 @@
 
     if isinstance(config.cOptionalArgs,list):
        spc = " " * 30
        config.cOptionalArgs = f",\n{spc}".join(config.cOptionalArgs)
 
     # Asychronous implies code array and switchCase
     if config.asynchronous:
-       config.codeArray = True 
        config.switchCase = True
        config.memoryOptimization = False
 
-    if config.codeArray:
-       if config.switchCase:
-          ctemplate = env.get_template("codeSwitch.cpp")
-       else:
-          ctemplate = env.get_template("codeArray.cpp")
+    if config.switchCase:
+       ctemplate = env.get_template("codeSwitch.cpp")
        nb = 0
        for s in sched.schedule:
          schedDescription = schedDescription + ("%d," % sched.nodes[s].codeID)
          nb = nb + 1
          if nb == 40:
             nb=0 
             schedDescription = schedDescription + "\n"
@@ -74,15 +70,14 @@
     nbFifos = len(sched._graph._allFIFOs)
     
     with open(cfile,"w") as f:
          print(ctemplate.render(fifos=sched._graph._allFIFOs,
             nbFifos=nbFifos,
             nbNodes=len(sched.nodes),
             nodes=sched.nodes,
-            pureNodes=sched.pureNodes,
             schedule=sched.schedule,
             schedLen=len(sched.schedule),
             config=config,
             sched=sched,
             schedDescription=schedDescription
             ),file=f)
```

## cmsis_stream/cg/scheduler/config.py

```diff
@@ -21,14 +21,15 @@
 # distributed under the License is distributed on an AS IS BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ############################################
 from jinja2 import Environment, PackageLoader, select_autoescape
 import os.path
+import os
 
 """Configuration of C code generation"""
 class Configuration:
 
     def __init__(self):
 
         #########################
@@ -86,18 +87,14 @@
 
         # Prefix to add before the global FIFO buffer names
         self.prefix = ""
 
         # Path to CG  module for Python simu 
         self.pathToCGModule="../../.."
 
-        # When codeArray  is true, instead of using
-        # function calls we parse un array giving
-        # the index of functions to call in another array
-        self.codeArray = True
         # If users do not want to use function pointers,
         # we can generate a switch/case instead
         self.switchCase = True
 
         # Enable support for CMSIS Event Recorder 
         self.eventRecorder = False
 
@@ -111,27 +108,30 @@
 
         # Name of post custom files
         self.postCustomCName = ""
 
         # Name of generic nodes headers
         self.genericNodeCName = "GenericNodes.h"
 
+        # Name of cg_status header for error codes
+        self.cgStatusCName = "cg_status.h"
+
         # Name of scheduler source and header files
         self.schedulerCFileName = "scheduler"
         self.schedulerPythonFileName = "sched"
 
         # True is C API for the scheduler
         self.CAPI = True
 
         # By default arm_math.h is included
         self.CMSISDSP = False
 
         # Asynchronous scheduling using
         # synchronous as first start
-        # It implies switchCase and codeArray
+        # It implies switchCase
         # It disables memory optimizations
         # Also FIFO cannot be used any more as just
         # buffers.
         self.asynchronous = False
 
         # Increase in percent of the FIFOs.
         # Used in asynchronous mode
@@ -140,14 +140,17 @@
         # synchronous scheduling.
         self.FIFOIncrease = 0
 
         # Default asynchronous more for pure functions 
         # like CMSIS-DSP
         self.asyncDefaultSkip = True
 
+        self.heapAllocation = False
+
+
        
     @property
     def debug(self):
         return (self.debugLimit > 0)
     
 
 def generateGenericNodes(folder):
@@ -157,7 +160,50 @@
        trim_blocks=True
     )
 
     ctemplate = env.get_template("GenericNodes.h")
     path=os.path.join(folder,"GenericNodes.h")
     with open(path,"w") as f:
         print(ctemplate.render(),file=f)
+
+def generateCGStatus(folder):
+    env = Environment(
+       loader=PackageLoader("cmsis_stream.cg.scheduler"),
+       autoescape=select_autoescape(),
+       trim_blocks=True
+    )
+
+    ctemplate = env.get_template("cg_status.h")
+    path=os.path.join(folder,"cg_status.h")
+    with open(path,"w") as f:
+        print(ctemplate.render(),file=f)
+
+def createEmptyProject(project_name):
+    env = Environment(
+       loader=PackageLoader("cmsis_stream.cg.scheduler"),
+       autoescape=select_autoescape(),
+       trim_blocks=True
+    )
+    try:
+        os.mkdir(project_name)
+    except Exception as e:
+        pass
+
+    all_files={"start_project_appnodes.h":"AppNodes.h"
+              ,"start_project_custom.h":"custom.h"
+              ,"start_project_main.c":"main_host.c"
+              ,"start_project_graph.py":"graph.py"
+              ,"Makefile.linux":"Makefile.linux"
+              ,"Makefile.mac":"Makefile.mac"
+              ,"Makefile.windows":"Makefile.windows"
+              ,"main_board.c":"main.c"
+              ,"simple.csolution_ac6.yml":"simple.csolution_ac6.yml"
+              ,"simple.cproject.yml":"simple.cproject.yml"
+              ,"vht.clayer.yml":"vht.clayer.yml"
+              ,"run.bat":"run_vht.bat"
+              ,"ARMCM55_FP_MVE_config.txt":"ARMCM55_FP_MVE_config.txt"};
+    for src_name in all_files:
+        dst_name = all_files[src_name]
+        ctemplate = env.get_template(f"project/{src_name}")
+        path = os.path.join(project_name,dst_name)
+        with open(path,"w") as f:
+            print(ctemplate.render(),file=f)
```

## cmsis_stream/cg/scheduler/description.py

```diff
@@ -1016,83 +1016,46 @@
         self._allBuffers = allBuffers
 
         if config.dumpSchedule:
             print("Schedule")
             for nodeID in schedule:
                 print(self._sortedNodes[nodeID].nodeName)
             print("")
-        return(Schedule(self,self._sortedNodes,self._sortedEdges,schedule))
+        return(Schedule(self,self._sortedNodes,self._sortedEdges,schedule,config))
 
 
 class Schedule:
-    def __init__(self,g,sortedNodes,sortedEdges,schedule):
+    def __init__(self,g,sortedNodes,sortedEdges,schedule,config):
         self._sortedNodes=sortedNodes
         self._sortedEdges=sortedEdges
         self._schedule = schedule 
         self._graph = g
+        self._config = config
         # Nodes containing pure functions (no state) like some
         # CMSIS-DSP functions.
-        # When scheduling is using the option codeArray, the
-        # schedule is encoded as an array.
-        # Function calls cannot be inlined anymore and we need
-        # to create new nodes for those function calls.
-        # The pureNode structure is done for this.
-        # It is a record because we want to reuse nodes for same
-        # types.
-        self._pureNodes={}
+        
         nodeCodeID = 0
         pureClassID = 1
         for n in self.nodes:
             n.codeID = nodeCodeID
             nodeCodeID = nodeCodeID + 1
             # Constant nodes are ignored since they have
             # no arcs, and are connected to no FIFOs
-            theArgs=[] 
-            theArgTypes=[]
-            i,o=n.allIOs()
-            for io in i:
-                # An io connected to a constant node has no fifo 
-                if len(io.fifo) > 0:
-                   theArgs.append(self.fifoID(io.fifo))
-                   theArgTypes.append(io.ctype)
-                else:
-                # Instead the arg is the name of a constant node
-                # instead of being a fifo ID
-                   theArgs.append(io.constantNode.name)
-                   theArgTypes.append(io.constantNode.name)
-            for io in o:
-                theArgs.append(self.fifoID(io.fifo))
-                theArgTypes.append(io.ctype)
-            n.args=theArgs
-
-            # Analyze the nature of arguments for pure functions
-            # The information created during this analysis
-            # is useful when generating a class containing the
-            # pure function
-            if not n.hasState:
-               theType=(n.nodeName,tuple(theArgTypes))
-               if not theType in self._pureNodes:
-                  self._pureNodes[theType]=n
-                  n.pureClassID = pureClassID 
-                  pureClassID = pureClassID + 1
-               else:
-                  n.pureClassID = self._pureNodes[theType].pureClassID
-               n.pureNodeType=theType
-               n.analyzeArgs()
+            
+            pureClassID=n.createArgsWithSchedulerFifoID(pureClassID,self._config,self.fifoID)
+            
+
+            
 
     def hasDelay(self,edge):
         return(self._graph.hasDelay(edge))
 
     def getDelay(self,edge):
         return(self._graph.getDelay(edge))
 
-    @property
-    def pureNodes(self):
-        return self._pureNodes
-    
 
     @property
     def constantEdges(self):
         return self._graph.constantEdges
 
     @property
     def nodes(self):
```

## cmsis_stream/cg/scheduler/node.py

```diff
@@ -26,15 +26,15 @@
 """Description of the basic types used to build a dataflow graph"""
 from jinja2 import Environment, FileSystemLoader, PackageLoader,select_autoescape
 import pathlib
 import os.path
 import numpy as np
 
 from sympy.core.numbers import ilcm
-
+from .args import *
 
 class NoFunctionArrayInPython(Exception):
     pass
 
 class NoAsynchronousModeInPython(Exception):
     pass
 
@@ -363,33 +363,83 @@
         """
         return self._nodeName
 
     # For code generation
 
 
 
-    def allIOs(self):
+    def createArgsWithSchedulerFifoID(self,pureClassID,config,fifoID):
         """Get list of IO objects for inputs and outputs"""
-        ins=[] 
-        outs=[]
+        i=[] 
+        o=[]
+        theArgs=[] 
+        theArgTypes=[]
         # Use orderd io names
         for io in self.inputNames:
             x = self._inputs[io]
-            ins.append(x)
+            i.append(x)
 
         for io in self.outputNames:
             x = self._outputs[io]
-            outs.append(x)
+            o.append(x)
 
         
-        return(ins,outs)
-
+        for io in i:
+                # An io connected to a constant node has no fifo 
+                if len(io.fifo) > 0:
+                   theArgs.append(fifoID(io.fifo))
+                   theArgTypes.append(io.ctype)
+                else:
+                # Instead the arg is the name of a constant node
+                # instead of being a fifo ID
+                   theArgs.append(io.constantNode.name)
+                   theArgTypes.append(io.constantNode.name)
+        for io in o:
+                theArgs.append(fifoID(io.fifo))
+                theArgTypes.append(io.ctype)
+
+        if not self.hasState:
+           # For pure function, analyze how many
+           # real arguments (FIFO) we have
+           self.analyzeConstantArgs()
+
+        self.setArgsWith(theArgs,config)
+
+        # Used to know how to call the run function of the
+        # node in the CRun functions.
+        if config.heapAllocation:
+            self.nodeVariable=ArgsPtrObj(self.nodeName,owner="nodes")
+        else:
+            self.nodeVariable=ArgsObject(self.nodeName)
+       
 
+        return(pureClassID)
 
     
+    # Compute how many real inputs and outputs we have
+    # Other are constant ndoes
+    def analyzeConstantArgs(self):
+        inputid=0
+        outputid=0
+        
+        # Use ordered io names
+        for io in self.inputNames:
+            x = self._inputs[io]
+            if not x.constantNode:
+               inputid = inputid + 1
+
+        for io in self.outputNames:
+            x = self._outputs[io]
+            if not x.constantNode:
+               outputid = outputid + 1
+               
+
+        self._realInputs = inputid
+        self._realOutputs = outputid
+        
 
     def ioTemplate(self):
         """Template arguments for C
            input type, input size ...
            output type, output size ...
 
            Some nodes may customize it
@@ -447,23 +497,23 @@
             else:
                 m = np.max(x.nbSamples)
                 ios.append("%d" % m)
 
         
         return("".join(joinit(ios,",")))
 
-    def cRun(self,ctemplate=True):
+    def cRun(self,config,ctemplate=True):
         """Run function
 
            Some nodes may customize it
         """
         if ctemplate:
-           return ("cgStaticError = %s.run();" % self.nodeName)
+           return (f"cgStaticError = {self.nodeVariable.access}run();")
         else:
-           return ("cgStaticError = %s.run()" % self.nodeName)
+           return (f"cgStaticError = {self.nodeVariable.access}run()")
 
     def cFunc(self,ctemplate=True):
         """Function call for code array scheduler
 
            Some nodes may customize it
         """
         if ctemplate:
@@ -478,46 +528,46 @@
         return self._args
 
 
     @property
     def args(self):
         """String of fifo args for object initialization
             with literal argument and variable arguments"""
-        allArgs=self.listOfargs
+        allArgs=[x.reference for x in self.listOfargs]
         # Add specific argrs after FIFOs
         if self.schedArgs:
             for lit in self.schedArgs:
                 allArgs.append(lit.arg)
         return "".join(joinit(allArgs,","))
     
-    def setArgsWith(self,fifoIDs):
+    def setArgsWith(self,fifoIDs,config):
         res=[]
         # Template args is used only for code array
         # scheduler when we create on the fly a new class
         # for a function.
         # In this case, the arguments of the template must only be
         # fifos and not constant.
         templateargs=[]
         for x in fifoIDs:
           # If args is a FIFO we generate a name using fifo ids
           if isinstance(x,int):
-             res.append("fifo%d" % x)
-             templateargs.append("fifo%d" % x)
+             if config.heapAllocation:
+                fifoArg = FifoPtrID(x,owner="fifos")
+             else:
+                fifoArg = FifoID(x)
+             res.append(fifoArg)
+             templateargs.append(fifoArg)
           # If args is a constant node, we just use the constant node name
           # (Defined in C code)
           else:
-             res.append(x)
+             res.append(ArgsObject(x))
         self._args=res
         self._templateargs=templateargs
 
-    @args.setter
-    def args(self,fifoIDs):
-       self.setArgsWith(fifoIDs)
-       
-
+    
     # For graphviz generation
 
 
 
     @property
     def graphvizName(self):
         """Name for graph vizualization"""
@@ -708,106 +758,24 @@
 
     PYTEMPLATE = ENV.get_template("cmsis.py")
 
     def __init__(self,funcname,theType,length):
         if not (funcname in GenericFunction.NODEID):
             GenericFunction.NODEID[funcname]=1 
 
-        self._pureNodeID = GenericFunction.PUREID
         GenericFunction.PUREID = GenericFunction.PUREID + 1
         GenericNode.__init__(self,"%s%d" % (funcname,GenericFunction.NODEID[funcname]))
 
         self._hasState = False
         self._length = length 
         self._nodeName = funcname
         self._isPureNode = True
 
         GenericFunction.NODEID[funcname]=GenericFunction.NODEID[funcname]+1
 
-
-    # For class generated on the fly to contain a function call
-    # Analyze which args are constant instead of being FIFOs
-    def analyzeArgs(self):
-        inputid=0 
-        outputid=0
-        # Arguments to use when calling the constructor
-        ios=[]
-        # Template params
-        temptypes=[]
-        specializedtemptypes=[]
-        # template args
-        tempargs=[]
-        # Template params for the generic node
-        tempgen=[]
-        # Datatypes for the constructor
-        constructortypes=[]
-        # Args for the generic constructor
-        genericconstructorargs=[]
-
-        typenameID = 1
-        # Use ordered io names
-        for io in self.inputNames:
-            x = self._inputs[io]
-            if not x.constantNode:
-               inputid = inputid + 1
-               temptypes.append("typename T%d, int input%dSize" % (typenameID,inputid))
-               specializedtemptypes.append("int input%dSize" % (inputid))
-               tempargs.append("%s,input%dSize" % (x.ctype,inputid))
-               tempgen.append("%s,input%dSize" % (x.ctype,inputid))
-               constructortypes.append("FIFOBase<%s> &src%d" % (x.ctype,inputid))
-               genericconstructorargs.append("src%d" % inputid)
-               # For cyclo static scheduling, nbSamples may be a list
-               if isinstance(x.nbSamples,int):
-                  ios.append("%s,%d" % (x.ctype,x.nbSamples))
-               else:
-                  m = np.max(x.nbSamples)
-                  ios.append("%s,%d" % (x.ctype,m))
-               typenameID = typenameID + 1
-
-        for io in self.outputNames:
-            x = self._outputs[io]
-            if not x.constantNode:
-               outputid = outputid + 1
-               temptypes.append("typename T%d,int output%dSize" % (typenameID,outputid))
-               specializedtemptypes.append("int output%dSize" % (outputid))
-               tempargs.append("%s,output%dSize" % (x.ctype,outputid))
-               tempgen.append("%s,output%dSize" % (x.ctype,outputid))
-               constructortypes.append("FIFOBase<%s> &dst%d" % (x.ctype,outputid))
-               genericconstructorargs.append("dst%d" % outputid)
-               if isinstance(x.nbSamples,int):
-                  ios.append("%s,%d" % (x.ctype,x.nbSamples))
-               else:
-                  m = np.max(x.nbSamples)
-                  ios.append("%s,%d" % (x.ctype,m))
-               typenameID = typenameID + 1
-
-        self._realInputs = inputid
-        self._realOutputs = outputid
-        # Arguments to use when calling the constructor
-        self._constructorTypes = "".join(joinit(ios,","))
-        # Argument 
-        self._constructorArguments = "".join(joinit(self._templateargs,",")) 
-        # Template parameters to use when defining the template
-        self._templateParameters = "".join(joinit(temptypes,","))
-        # Template parameters to use when defining the template
-        self._specializedTemplateParameters = "".join(joinit(specializedtemptypes,","))
-        # Template parameters to use when defining the template
-        self._templateArguments = "".join(joinit(tempargs,","))
-        # Template parameters to use when defining the template
-        self._templateParametersForGeneric = "".join(joinit(tempgen,","))
-        # Datatypes for the constructors 
-        self._datatypeForConstructor = "".join(joinit(constructortypes,","))
-        # Args for the generic constructor
-        self._genericConstructorArgs = "".join(joinit(genericconstructorargs,","))
-
-    @property
-    def pureNodeID(self):
-        return self._pureNodeID
-    
-
     @property
     def realInputs(self):
         return self._realInputs
     
     @property
     def realOutputs(self):
         return self._realOutputs
@@ -956,29 +924,18 @@
            node=self,
            asyncDefaultSkip = asyncDefaultSkip
            )
         return(result)
         
 
     # To clean
-    def cRun(self,ctemplate=True,codeArray=False):
+    def cRun(self,config,ctemplate=True):
        params = self._prepareForCodeGen(ctemplate)
 
        if ctemplate:
-           if codeArray:
-              result=Dsp.CNODETEMPLATE.render(func=self._nodeName,
-               theType = params["theType"],
-               nb = params["nb"],
-               ptrs = params["ptrs"],
-               args = params["args"],
-               inputs=params["inputs"], 
-               outputs=params["outputs"],
-               node=self
-               )
-           else:
               result=Dsp.CTEMPLATE.render(func=self._nodeName,
                theType = params["theType"],
                nb = params["nb"],
                ptrs = params["ptrs"],
                args = params["args"],
                inputs=params["inputs"], 
                outputs=params["outputs"],
@@ -994,18 +951,15 @@
             outArgs= params["outArgsStr"], 
             inputs=params["inputs"], 
             outputs=params["outputs"],
             node=self
             )
        return(result)
 
-    def codeArrayRun(self):
-        return(self.cRun(codeArray=True))
-
-
+    
 class Unary(GenericFunction):
     def __init__(self,funcname,theType,length):
         GenericFunction.__init__(self,funcname,theType,length)
 
         self.addInput("i",theType,length)
         self.addOutput("o",theType,length)
```

## cmsis_stream/cg/scheduler/standard.py

```diff
@@ -173,28 +173,24 @@
     @property
     def args(self):
         """String of fifo args for object initialization
             with literal argument and variable arguments"""
         allArgs=self.listOfargs
         theInput = allArgs[0]
         nb = len(allArgs) - 1
-        others = ",{" + "".join(joinit(["&"+x for x in allArgs[1:]],",")) + "}"
+        others = ",{" + "".join(joinit([x.pointer for x in allArgs[1:]],",")) + "}"
         # Add specific argrs after FIFOs
         sched = []
         if self.schedArgs:
             for lit in self.schedArgs:
                 sched.append(lit.arg)
         if sched:
-            return (theInput + others + "," + "".join(joinit(sched,",")))
+            return (theInput.reference + others + "," + "".join(joinit(sched,",")))
         else:
-           return (theInput + others)
-
-    @args.setter
-    def args(self,fifoIDs):
-       self.setArgsWith(fifoIDs)
+           return (theInput.reference + others)
 
     def ioTemplate(self):
         """ioTemplate is different for window
         """
         theType=self._inputs[self.inputNames[0]].ctype  
         ios="%s,%d" % (theType,self._length)
         return(ios)
```

## cmsis_stream/cg/scheduler/templates/GenericNodes.h

```diff
@@ -31,14 +31,15 @@
 #include <cstring>
 #include <stdarg.h>
 /* 
 Defined in cg_status.h by default but user
 may want to use a different header to define the 
 error codes of the application
 */
+#define CG_SUCCESS_ID_CODE (0)
 #define CG_SKIP_EXECUTION_ID_CODE (-5)
 #define CG_BUFFER_ERROR_ID_CODE (-6)
 
 // FIFOS 
 
 #ifdef DEBUGSCHED
 
@@ -445,27 +446,27 @@
            if (this->willOverflow(inputOutputSize,i))
            {
               return(CG_SKIP_EXECUTION_ID_CODE); // Skip execution
            }
         }
 
 
-        return(0);
+        return(CG_SUCCESS_ID_CODE);
     };
 
     int run() final {
         IO *a=this->getReadBuffer();
         
         for(unsigned int i=0;i<mDstList.size();i++)
         {
            IO *b=this->getWriteBuffer(inputOutputSize,i);
            memcpy(b,a,sizeof(IO)*inputOutputSize);
         }
         
-        return(0);
+        return(CG_SUCCESS_ID_CODE);
     };
 
 protected:
     IO * getWriteBuffer(int nb = inputOutputSize,int id=1){return mDstList[id]->getWriteBuffer(nb);};
     IO * getReadBuffer(int nb = inputOutputSize){return mSrc.getReadBuffer(nb);};
 
     bool willOverflow(int nb = inputOutputSize,int id=1){return mDstList[id]->willOverflowWith(nb);};
```

## cmsis_stream/cg/scheduler/templates/cmsis.cpp

```diff
@@ -1,15 +1,15 @@
 
                   {
 
 {% for ptr in ptrs %}
                    {{theType}}* {{ptr}};
 {% endfor %}
 {% for ptr in inputs %}
-                   {{ptr[0]}}={{ptr[1]}}.getReadBuffer({{nb}});
+                   {{ptr[0]}}={{ptr[1].access}}getReadBuffer({{nb}});
 {% endfor %}
 {% for ptr in outputs %}
-                   {{ptr[0]}}={{ptr[1]}}.getWriteBuffer({{nb}});
+                   {{ptr[0]}}={{ptr[1].access}}getWriteBuffer({{nb}});
 {% endfor %}
                    {{func}}({{args}},{{nb}});
                    cgStaticError = 0;
                   }
```

## cmsis_stream/cg/scheduler/templates/cmsis.py

```diff
@@ -1,10 +1,10 @@
 
 {% for ptr in inputs %}
-       {{ptr[0]}}={{ptr[1]}}.getReadBuffer({{nb}})
+       {{ptr[0]}}={{ptr[1].access}}getReadBuffer({{nb}})
 {% endfor %}
 {% for ptr in outputs %}
-       {{ptr[0]}}={{ptr[1]}}.getWriteBuffer({{nb}})
+       {{ptr[0]}}={{ptr[1].access}}getWriteBuffer({{nb}})
 {% endfor %}
        {{outArgs}}[:]=dsp.{{func}}({{inArgs}})
        cgStaticError = 0
```

## cmsis_stream/cg/scheduler/templates/cmsisCheck.cpp

```diff
@@ -1,14 +1,14 @@
                     
                     bool canRun=true;
 {% for ptr in inputs %}
-                    canRun &= !{{ptr[1]}}.willUnderflowWith({{nb}});
+                    canRun &= !({{ptr[1].access}}willUnderflowWith({{nb}}));
 {% endfor %}
 {% for ptr in outputs %}
-                    canRun &= !{{ptr[1]}}.willOverflowWith({{nb}});
+                    canRun &= !({{ptr[1].access}}willOverflowWith({{nb}}));
 {% endfor %}
 
                     if (!canRun)
                     {
 {% if asyncDefaultSkip %}
                       cgStaticError = CG_SKIP_EXECUTION_ID_CODE;
 {% else %}
```

## cmsis_stream/cg/scheduler/templates/code.cpp

```diff
@@ -17,15 +17,15 @@
        {% endif -%}
        CG_BEFORE_ITERATION;
 {% for s in schedule %}
        {% if config.eventRecorder -%}
        EventRecord2 (Evt_Node, {{nodes[s].codeID}}, 0);
        {% endif -%}
        CG_BEFORE_NODE_EXECUTION;
-       {{nodes[s].cRun()}}
+       {{nodes[s].cRun(config)}}
        CG_AFTER_NODE_EXECUTION;
        {% if config.eventRecorder -%}
        if (cgStaticError<0)
        {
            EventRecord2 (Evt_Error, cgStaticError, 0);
        }
        {% endif -%}
```

## cmsis_stream/cg/scheduler/templates/code.h

```diff
@@ -28,14 +28,18 @@
 
 #define Evt_Scheduler   EventID (EventLevelAPI,   EvtSched, 0x00)
 #define Evt_Node        EventID (EventLevelAPI,   EvtSched, 0x01)
 #define Evt_Error       EventID (EventLevelError,   EvtSched, 0x02)
 
 {% endif %}
 
+{% if config.heapAllocation %}
+extern int init_{{config.schedName}}();
+extern void free_{{config.schedName}}();
+{% endif %}
 extern uint32_t {{config.schedName}}(int *error{{optionalargs()}});
 
 {% if config.CAPI -%}
 #ifdef   __cplusplus
 }
 #endif
 {% endif %}
```

## cmsis_stream/cg/scheduler/templates/code.py

```diff
@@ -69,15 +69,15 @@
     while((cgStaticError==0) and (debugCounter > 0)):
 {% else %}
     while(cgStaticError==0):
 {% endif %}
        nbSchedule = nbSchedule + 1
 
 {% for s in schedule %}
-       {{nodes[s].cRun(False)}}
+       {{nodes[s].cRun(config,False)}}
        if cgStaticError < 0:
           break
 {% if config.dumpFIFO %}
 {% for fifoID in sched.outputFIFOs(nodes[s]) %}
        print("{{nodes[s].nodeName}}:{{fifoID[1]}}")
        fifo{{fifoID[0]}}.dump()
 {% endfor %}
```

## cmsis_stream/cg/scheduler/templates/codeSwitch.cpp

```diff
@@ -36,16 +36,20 @@
             cgStaticError = 0;
             switch(schedule[id])
             {
                 {% for nodeID in range(nbNodes) -%}
                 case {{nodeID}}:
                 {
                     {% if not nodes[nodeID].isPureNode -%}
+                    {%- if not config.heapAllocation -%}
                     cgStaticError = {{nodes[nodeID].nodeName}}.prepareForRunning();
                     {%- else -%}
+                    cgStaticError = nodes.{{nodes[nodeID].nodeName}}->prepareForRunning();
+                    {%- endif -%}
+                    {%- else -%}
                     {{nodes[nodeID].cCheck(config.asyncDefaultSkip)}}
                     {%- endif %}
 
                 }
                 break;
 
                 {% endfor -%}
@@ -72,15 +76,15 @@
             {% endif -%}
 
             switch(schedule[id])
             {
                 {% for nodeID in range(nbNodes) -%}
                 case {{nodeID}}:
                 {
-                   {{nodes[nodeID].cRun()}}
+                   {{nodes[nodeID].cRun(config)}}
 
                    {%- if config.dumpFIFO %}
                    {%- for fifoID in sched.outputFIFOs(nodes[nodeID]) %}
                    
                    std::cout << "{{nodes[nodeID].nodeName}}:{{fifoID[1]}}" << std::endl;
                    fifo{{fifoID[0]}}.dump();
                    {%- endfor %}
```

## cmsis_stream/cg/scheduler/templates/commonc.cpp

```diff
@@ -14,14 +14,15 @@
 {% if config.CMSISDSP -%}
 #include "arm_math.h"
 {% else %}
 #include <cstdint>
 {% endif %}
 #include "{{config.customCName}}"
 #include "{{config.genericNodeCName}}"
+#include "{{config.cgStatusCName}}"
 #include "{{config.appNodesCName}}"
 #include "{{config.schedulerCFileName}}.h"
 {% if config.postCustomCName -%}
 #include "{{config.postCustomCName}}"
 {% endif %}
 
 {% include "defineConfig.h" %}
@@ -53,23 +54,100 @@
 {% for buf in sched._graph._allBuffers %}
 #define BUFFERSIZE{{buf._bufferID}} {{buf._length}}
 CG_BEFORE_BUFFER
 {{buf._theType.ctype}} {{config.prefix}}buf{{buf._bufferID}}[BUFFERSIZE{{buf._bufferID}}]={0};
 
 {% endfor %}
 
+{% if config.heapAllocation %}
+typedef struct {
+{% for id in range(nbFifos) %}
+{{fifos[id].fifoClass}}<{{fifos[id].theType.ctype}},FIFOSIZE{{id}},{{fifos[id].isArrayAsInt}},{{async()}}> *fifo{{id}};
+{% endfor %}
+} fifos_t;
+
+typedef struct {
+{% for node in nodes %}
+{% if node.hasState %}
+    {{node.typeName}}<{{node.ioTemplate()}}> *{{node.nodeName}};
+{% endif %}
+{% endfor %}
+} nodes_t;
+
+CG_BEFORE_BUFFER
+static fifos_t fifos={0};
+
+CG_BEFORE_BUFFER
+static nodes_t nodes={0};
+
+int init_{{config.schedName}}()
+{
+    CG_BEFORE_FIFO_INIT;
+{% for id in range(nbFifos) %}
+{% if fifos[id].hasDelay %}
+    fifos.fifo{{id}} = new {{fifos[id].fifoClass}}<{{fifos[id].theType.ctype}},FIFOSIZE{{id}},{{fifos[id].isArrayAsInt}},{{async()}}>({{config.prefix}}buf{{fifos[id].buffer._bufferID}},{{fifos[id].delay}});
+    if (fifos.fifo{{id}}==NULL)
+    {
+        return(CG_MEMORY_ALLOCATION_FAILURE);
+    }
+{% else %}
+    fifos.fifo{{id}} = new {{fifos[id].fifoClass}}<{{fifos[id].theType.ctype}},FIFOSIZE{{id}},{{fifos[id].isArrayAsInt}},{{async()}}>({{config.prefix}}buf{{fifos[id].buffer._bufferID}});
+    if (fifos.fifo{{id}}==NULL)
+    {
+        return(CG_MEMORY_ALLOCATION_FAILURE);
+    }
+{% endif %}
+{% endfor %}
+
+    CG_BEFORE_NODE_INIT;
+{% for node in nodes %}
+{% if node.hasState %}
+    nodes.{{node.nodeName}} = new {{node.typeName}}<{{node.ioTemplate()}}>({{node.args}});
+    if (nodes.{{node.nodeName}}==NULL)
+    {
+        return(CG_MEMORY_ALLOCATION_FAILURE);
+    }
+{% endif %}
+{% endfor %}
+
+    return(CG_SUCCESS);
+
+}
+
+void free_{{config.schedName}}()
+{
+{% for id in range(nbFifos) %}
+    if (fifos.fifo{{id}}!=NULL)
+    {
+       delete fifos.fifo{{id}};
+    }
+{% endfor %}
+
+{% for node in nodes %}
+{% if node.hasState %}
+    if (nodes.{{node.nodeName}}!=NULL)
+    {
+        delete nodes.{{node.nodeName}};
+    }
+{% endif %}
+{% endfor %}
+}
+
+{% endif %}
+
 CG_BEFORE_SCHEDULER_FUNCTION
 uint32_t {{config.schedName}}(int *error{{optionalargs()}})
 {
     int cgStaticError=0;
     uint32_t nbSchedule=0;
 {% if config.debug %}
     int32_t debugCounter={{config.debugLimit}};
 {% endif %}
 
+{% if not config.heapAllocation %}
     CG_BEFORE_FIFO_INIT;
     /*
     Create FIFOs objects
     */
 {% for id in range(nbFifos) %}
 {% if fifos[id].hasDelay %}
     {{fifos[id].fifoClass}}<{{fifos[id].theType.ctype}},FIFOSIZE{{id}},{{fifos[id].isArrayAsInt}},{{async()}}> fifo{{id}}({{config.prefix}}buf{{fifos[id].buffer._bufferID}},{{fifos[id].delay}});
@@ -83,14 +161,15 @@
     Create node objects
     */
 {% for node in nodes %}
 {% if node.hasState %}
     {{node.typeName}}<{{node.ioTemplate()}}> {{node.nodeName}}({{node.args}});
 {% endif %}
 {% endfor %}
+{% endif %}
 
     /* Run several schedule iterations */
 {% block scheduleLoop %}
 {% endblock %}
 errorHandling:
     CG_AFTER_SCHEDULE;
     *error=cgStaticError;
```

## Comparing `cmsis_stream-1.1.0.dist-info/LICENSE.txt` & `cmsis_stream-1.2.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `cmsis_stream-1.1.0.dist-info/METADATA` & `cmsis_stream-1.2.0.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmsis-stream
-Version: 1.1.0
+Version: 1.2.0
 Summary: CMSIS-Stream graph description
 Home-page: https://github.com/ARM-software/CMSIS-Stream
 Author: Copyright (C) 2010-2023 ARM Limited or its affiliates. All rights reserved.
 Author-email: christophe.favergeon@arm.com
 License: License :: OSI Approved :: Apache Software License
 Project-URL: Bug Reports, https://github.com/ARM-software/CMSIS-Stream/issues
 Project-URL: Source, https://github.com/ARM-software/CMSIS-Stream
@@ -40,14 +40,25 @@
 
 * Define new compute nodes
 * Connect them into a dataflow graph to process streams
 * Generate a C scheduler to run the graph on your target
 
 # Change history
 
+## Version 1.2.0:
+
+* The file cg_status.h can now also be created from
+the python package
+
+* A new heapAllocate option has been introduced. When true,
+FIFO and node objects are allocated on the heap and no more
+on the stack. Two new functions are generated in the scheduler to initialize or free those objects
+
+* A new command line tool cmsis-stream is available. It can be used to quickly create a project with : cmsis-stream create TestFolder. The folder will contain makefiles for windows, mac and linux. It will also contain a CMSIS build tool solution file to build for Arm Virtual Hardware CS 300
+
 ## Version 1.1.0:
 
 * The file GenericNodes.h can now be created from the
 python package. Like that, it is possible to start using
 CMSIS-Stream by only installing the Python package.
 Of course, if other specifics nodes are required (FFT, MFCC) the CMSIS-Stream repository will have to be used to get the headers
```

## Comparing `cmsis_stream-1.1.0.dist-info/RECORD` & `cmsis_stream-1.2.0.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 cmsis_stream/__init__.py,sha256=8gVWTuduHPk4Eu0cz_jvNXAdj5knn28sMkK3Gl59Cz4,298
+cmsis_stream/cmsis_stream.py,sha256=sU64sGuSpzVeiSogQci1bIfD7U6mN1ndjFt-9ffWdyQ,546
 cmsis_stream/cg/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cmsis_stream/cg/types.py,sha256=K5r2dv5gZLoFcSAnJM9IIu6ZPL5wlZAf9b_2x7-H-7E,7448
 cmsis_stream/cg/nodes/CFFT.py,sha256=3MkAn73PLnSzwnipjfBhDXPNhBoo11h7zynPAM8ot4g,1925
 cmsis_stream/cg/nodes/Duplicate.py,sha256=gPs2NMVeYXra05udPDU5-dIGDuVarHC0FYBprdAb6u0,1990
 cmsis_stream/cg/nodes/ICFFT.py,sha256=wVQVNnoIS0m1mh1B8IsAcQ87H8aQQ8mt4uaUAXcCIkY,1930
 cmsis_stream/cg/nodes/InterleavedStereoToMono.py,sha256=YBoW1FrZea8oOSYoxM8xVcsma-jTpgAo8lP-YEvRcsU,1645
 cmsis_stream/cg/nodes/MFCC.py,sha256=SmmiDXWSIuTOwg3iQw7U8l29y-PkfsPx5NrOkSOw48g,1974
@@ -19,32 +20,34 @@
 cmsis_stream/cg/nodes/host/VHT.py,sha256=jsn5v7bju9-tLqF2gKxrJnOljE2KeegC2fgY2Zd8V5s,2916
 cmsis_stream/cg/nodes/host/VHTCGSTATIC.py,sha256=zNXVzkZZROzGwHBq62uzFuAVIummPwMcxW0JhpaI-88,871
 cmsis_stream/cg/nodes/host/WavSink.py,sha256=ldo5e9wjaIp0Ef6GvRgZIICuuk3H1V7B-hn1et6S7Wo,2029
 cmsis_stream/cg/nodes/host/WavSource.py,sha256=KywcbHsrCqrAQD6HuZaxOxVj_ekYDYIgzx_6Nh2R4Gk,2092
 cmsis_stream/cg/nodes/host/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cmsis_stream/cg/nodes/host/message.py,sha256=e2hto5-Ly08sUCKN8F94qH3O3lAxcGGIGBLkf6cLJCY,4018
 cmsis_stream/cg/scheduler/__init__.py,sha256=-GMWFk8b3LpReDjD7yHF_SLrFDu5PRZuxN1RbjkY6nk,118
-cmsis_stream/cg/scheduler/ccode.py,sha256=wJkbN2-adg48wxxbeHa91AiBMo3MwTpAfnEshjIft8U,3194
-cmsis_stream/cg/scheduler/config.py,sha256=esuIy4KxwzNGT7Z4Dn1wNXI-kc8Hsr-ntpK2mgux7oE,5086
-cmsis_stream/cg/scheduler/description.py,sha256=Kryyd9XiUv3Zi42XT0rZbNeEFGcMTnOYQJRA3rupJo8,43229
+cmsis_stream/cg/scheduler/args.py,sha256=mepFm7CJa2wnB-21a-h1FrufP5KtI78l_B3HNb87ayk,1691
+cmsis_stream/cg/scheduler/ccode.py,sha256=f57rHk2gtgkikywW_ZEkdXlibV4wnHbOQ5vi0fHRcME,3018
+cmsis_stream/cg/scheduler/config.py,sha256=x5mQRXHxqGiNS8czDYuqul-r0GDeobFod_8QrXrVmVI,6628
+cmsis_stream/cg/scheduler/description.py,sha256=6ob9d7bfo1TXUBFWq9aPnnY1wFPklsqi7poXPECxFA4,41560
 cmsis_stream/cg/scheduler/graphviz.py,sha256=wmbSzhIlOD9Z1E5NBsNklk4LvpaLQfs9Tmw-vAxwSPM,1784
-cmsis_stream/cg/scheduler/node.py,sha256=LhyPXNZgDNPljBZYA0QMMX-5GyfjpwwDYtx-yAgys2o,31509
+cmsis_stream/cg/scheduler/node.py,sha256=LJuuFbkWp8xJALM4aSXASaisYkhDQVfAfKlz0sQYnq4,29225
 cmsis_stream/cg/scheduler/pythoncode.py,sha256=bDtCVYvgtLO_wpl33HlyyAEZtfyW6wHyANQsdPvdlBA,1796
-cmsis_stream/cg/scheduler/standard.py,sha256=NjvilC9jSbIrEL24NkdJLQjM6sgC_ty2rHWpFXPjk9M,8319
-cmsis_stream/cg/scheduler/templates/GenericNodes.h,sha256=IaySD6PQJYaIK1Yp3Yo99f4fWQXHAd_bi9N2V-61Zl0,13936
-cmsis_stream/cg/scheduler/templates/cmsis.cpp,sha256=SXk_9pL_sBgbLIg7YqnbnQiEprAycKN0K0zLZYHrPDA,419
-cmsis_stream/cg/scheduler/templates/cmsis.py,sha256=Rv9OGK38-lSa3sSals0ur-xz_8q6sHOIP01AK6e1pX8,267
-cmsis_stream/cg/scheduler/templates/cmsisCheck.cpp,sha256=8L_D_F5OkhevXlIjUJt70NNXPp8uNB3UYqlpviM23I0,658
+cmsis_stream/cg/scheduler/standard.py,sha256=EEPGxII61ykghjLnVSkVV2s5DW2ZHfKI2ryhnDByhkU,8260
+cmsis_stream/cg/scheduler/templates/GenericNodes.h,sha256=6r6w3HloYzH3u8WGz5mDjEyhOkdcumxf3o4qOjx2CM0,14002
+cmsis_stream/cg/scheduler/templates/cg_status.h,sha256=1ZBdMG2s9FMyTzdvFtxpPIK624-jnfRd_Q2Qxe_MwTM,2006
+cmsis_stream/cg/scheduler/templates/cmsis.cpp,sha256=yNiZSHN-riYPkzCenN6UUoZD9ZieCI8L9viXYkQCCz0,431
+cmsis_stream/cg/scheduler/templates/cmsis.py,sha256=wbXrZ1fWz2YmD-yyvMshlaXvWXgTmfKokVEFu6SwAVk,279
+cmsis_stream/cg/scheduler/templates/cmsisCheck.cpp,sha256=bo05ISPFatzhi09c36ioA4HSJUtJc30k3T-z31oWN-8,674
 cmsis_stream/cg/scheduler/templates/cmsisNode.cpp,sha256=luXUXScO1ncXx1m2kI2e40DyjobwbwVucCY0QernoGc,297
-cmsis_stream/cg/scheduler/templates/code.cpp,sha256=I5xJUpY8hGj8k40jyahqn_0vO_43Ktn0QFjSQNUjytA,1226
-cmsis_stream/cg/scheduler/templates/code.h,sha256=44_GjsFb_yoLafY3JU_q3ysLna44qFiONUL12O27IWU,983
-cmsis_stream/cg/scheduler/templates/code.py,sha256=JIq8hsm_KUEQ8hGVQeFIfzezCCNmEp2fRk-1meKPQhM,2192
-cmsis_stream/cg/scheduler/templates/codeArray.cpp,sha256=Pxq9jo2uRVndDcmpbV2bqvE45osckA3ZHb3TDvLZEs8,4534
-cmsis_stream/cg/scheduler/templates/codeSwitch.cpp,sha256=RAn-QDuZLjL7mFYYpX0t0Jz9N3rvyG9z1hjZGr6dMHM,2960
-cmsis_stream/cg/scheduler/templates/commonc.cpp,sha256=bOgQWAL0KnkbQV7_Eb9gRiXYsR4ki4HNj258nzZY4YQ,2464
+cmsis_stream/cg/scheduler/templates/code.cpp,sha256=uiJEAmZyGoMq_AqYqZ3aXRyX9L7cRKdkUFazGLc1eP0,1232
+cmsis_stream/cg/scheduler/templates/code.h,sha256=BULWyJn9FAU6laXpg6UjyP5TtHHMCW_3zTccu_EtjKU,1111
+cmsis_stream/cg/scheduler/templates/code.py,sha256=eOK6r2DkCD-JftAKAi0K3PxOwidRWtdtal4N8_xC6wk,2199
+cmsis_stream/cg/scheduler/templates/codeSwitch.cpp,sha256=6fn_IVXZy77h8TQN2vSsuwMUVJFjyPtVzURjhnriAo0,3185
+cmsis_stream/cg/scheduler/templates/commonc.cpp,sha256=nmlbxVoBiujXLYerA056T_GPRL-LZSo0IFcz6BHdTHc,4482
 cmsis_stream/cg/scheduler/templates/defineConfig.h,sha256=h9R25-RcgG_kDKg4-xsGih4yPnffdNbZwkZMe5UXmhA,1051
 cmsis_stream/cg/scheduler/templates/dot_template.dot,sha256=GJyuIQkdt3RZvq2SRSBYrmuWj7QW9T4wVO-1GRGB8B0,4848
-cmsis_stream-1.1.0.dist-info/LICENSE.txt,sha256=4DukHX-rIHAHaf5BGLq1DYAMt0-ZA1OgXS9f_xwig2M,11558
-cmsis_stream-1.1.0.dist-info/METADATA,sha256=hRm8M0G5pdHnt7pxrNQEUlWGcdgPUzHUJvzGCs7wv1w,2494
-cmsis_stream-1.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-cmsis_stream-1.1.0.dist-info/top_level.txt,sha256=a7ZhPCd-XkrgWSSuOstN5Jgqe60MV4q7-tWximJBomA,13
-cmsis_stream-1.1.0.dist-info/RECORD,,
+cmsis_stream-1.2.0.dist-info/LICENSE.txt,sha256=4DukHX-rIHAHaf5BGLq1DYAMt0-ZA1OgXS9f_xwig2M,11558
+cmsis_stream-1.2.0.dist-info/METADATA,sha256=t5GdKdrGC6BEisEcf48Q77Xq5wVleUlAhf7Sb6ean9s,3109
+cmsis_stream-1.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+cmsis_stream-1.2.0.dist-info/entry_points.txt,sha256=WOEqwaMTN0K5CT8Yfd-z53mE82xfyzsM16a0eR4Ipds,59
+cmsis_stream-1.2.0.dist-info/top_level.txt,sha256=a7ZhPCd-XkrgWSSuOstN5Jgqe60MV4q7-tWximJBomA,13
+cmsis_stream-1.2.0.dist-info/RECORD,,
```

