# Comparing `tmp/cmsis_stream-1.2.0-py3-none-any.whl.zip` & `tmp/cmsis_stream-1.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 68003 bytes, number of entries: 53
+Zip file size: 75082 bytes, number of entries: 66
 -rw-rw-rw-  2.0 fat      298 b- defN 23-May-11 12:29 cmsis_stream/__init__.py
 -rw-rw-rw-  2.0 fat      546 b- defN 23-Jun-02 06:34 cmsis_stream/cmsis_stream.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-11 12:29 cmsis_stream/cg/__init__.py
 -rw-rw-rw-  2.0 fat     7448 b- defN 23-May-11 12:29 cmsis_stream/cg/types.py
 -rw-rw-rw-  2.0 fat     1925 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/CFFT.py
 -rw-rw-rw-  2.0 fat     1990 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/Duplicate.py
 -rw-rw-rw-  2.0 fat     1930 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/ICFFT.py
@@ -29,27 +29,40 @@
 -rw-rw-rw-  2.0 fat     3018 b- defN 23-Jun-02 05:04 cmsis_stream/cg/scheduler/ccode.py
 -rw-rw-rw-  2.0 fat     6628 b- defN 23-Jun-02 06:51 cmsis_stream/cg/scheduler/config.py
 -rw-rw-rw-  2.0 fat    41560 b- defN 23-Jun-02 05:04 cmsis_stream/cg/scheduler/description.py
 -rw-rw-rw-  2.0 fat     1784 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/graphviz.py
 -rw-rw-rw-  2.0 fat    29225 b- defN 23-Jun-02 07:49 cmsis_stream/cg/scheduler/node.py
 -rw-rw-rw-  2.0 fat     1796 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/pythoncode.py
 -rw-rw-rw-  2.0 fat     8260 b- defN 23-Jun-01 13:08 cmsis_stream/cg/scheduler/standard.py
--rw-rw-rw-  2.0 fat    14002 b- defN 23-Jun-02 08:01 cmsis_stream/cg/scheduler/templates/GenericNodes.h
--rw-rw-rw-  2.0 fat     2006 b- defN 23-Jun-02 08:01 cmsis_stream/cg/scheduler/templates/cg_status.h
+-rw-rw-rw-  2.0 fat    14002 b- defN 23-Jun-02 08:07 cmsis_stream/cg/scheduler/templates/GenericNodes.h
+-rw-rw-rw-  2.0 fat     2006 b- defN 23-Jun-02 08:07 cmsis_stream/cg/scheduler/templates/cg_status.h
 -rw-rw-rw-  2.0 fat      431 b- defN 23-Jun-01 13:09 cmsis_stream/cg/scheduler/templates/cmsis.cpp
 -rw-rw-rw-  2.0 fat      279 b- defN 23-Jun-02 07:46 cmsis_stream/cg/scheduler/templates/cmsis.py
 -rw-rw-rw-  2.0 fat      674 b- defN 23-Jun-01 13:13 cmsis_stream/cg/scheduler/templates/cmsisCheck.cpp
 -rw-rw-rw-  2.0 fat      297 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/templates/cmsisNode.cpp
 -rw-rw-rw-  2.0 fat     1232 b- defN 23-Jun-02 07:49 cmsis_stream/cg/scheduler/templates/code.cpp
 -rw-rw-rw-  2.0 fat     1111 b- defN 23-Jun-02 05:31 cmsis_stream/cg/scheduler/templates/code.h
 -rw-rw-rw-  2.0 fat     2199 b- defN 23-Jun-02 07:49 cmsis_stream/cg/scheduler/templates/code.py
 -rw-rw-rw-  2.0 fat     3185 b- defN 23-Jun-01 11:18 cmsis_stream/cg/scheduler/templates/codeSwitch.cpp
 -rw-rw-rw-  2.0 fat     4482 b- defN 23-Jun-02 05:31 cmsis_stream/cg/scheduler/templates/commonc.cpp
 -rw-rw-rw-  2.0 fat     1051 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/templates/defineConfig.h
 -rw-rw-rw-  2.0 fat     4848 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/templates/dot_template.dot
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-02 08:01 cmsis_stream-1.2.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     3109 b- defN 23-Jun-02 08:01 cmsis_stream-1.2.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-02 08:01 cmsis_stream-1.2.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       59 b- defN 23-Jun-02 08:01 cmsis_stream-1.2.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       13 b- defN 23-Jun-02 08:01 cmsis_stream-1.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     4955 b- defN 23-Jun-02 08:01 cmsis_stream-1.2.0.dist-info/RECORD
-53 files, 200127 bytes uncompressed, 59945 bytes compressed:  70.0%
+-rw-rw-rw-  2.0 fat      188 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/templates/project/ARMCM55_FP_MVE_config.txt
+-rw-rw-rw-  2.0 fat      192 b- defN 23-Jun-02 06:56 cmsis_stream/cg/scheduler/templates/project/Makefile.linux
+-rw-rw-rw-  2.0 fat      267 b- defN 23-Jun-02 06:56 cmsis_stream/cg/scheduler/templates/project/Makefile.mac
+-rw-rw-rw-  2.0 fat      369 b- defN 23-Jun-02 06:57 cmsis_stream/cg/scheduler/templates/project/Makefile.windows
+-rw-rw-rw-  2.0 fat      826 b- defN 23-Jun-02 06:47 cmsis_stream/cg/scheduler/templates/project/main_board.c
+-rw-rw-rw-  2.0 fat      212 b- defN 23-Jun-02 06:51 cmsis_stream/cg/scheduler/templates/project/run.bat
+-rw-rw-rw-  2.0 fat      589 b- defN 23-Jun-02 07:20 cmsis_stream/cg/scheduler/templates/project/simple.cproject.yml
+-rw-rw-rw-  2.0 fat     1416 b- defN 23-Jun-02 07:20 cmsis_stream/cg/scheduler/templates/project/simple.csolution_ac6.yml
+-rw-rw-rw-  2.0 fat     2178 b- defN 23-Jun-02 06:48 cmsis_stream/cg/scheduler/templates/project/start_project_appnodes.h
+-rw-rw-rw-  2.0 fat       73 b- defN 23-Jun-02 06:10 cmsis_stream/cg/scheduler/templates/project/start_project_custom.h
+-rw-rw-rw-  2.0 fat     1798 b- defN 23-Jun-02 06:26 cmsis_stream/cg/scheduler/templates/project/start_project_graph.py
+-rw-rw-rw-  2.0 fat      197 b- defN 23-Jun-02 06:05 cmsis_stream/cg/scheduler/templates/project/start_project_main.c
+-rw-rw-rw-  2.0 fat      860 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/templates/project/vht.clayer.yml
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-02 08:07 cmsis_stream-1.2.1.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     3253 b- defN 23-Jun-02 08:07 cmsis_stream-1.2.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-02 08:07 cmsis_stream-1.2.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       59 b- defN 23-Jun-02 08:07 cmsis_stream-1.2.1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Jun-02 08:07 cmsis_stream-1.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     6488 b- defN 23-Jun-02 08:07 cmsis_stream-1.2.1.dist-info/RECORD
+66 files, 210969 bytes uncompressed, 64430 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -135,26 +135,65 @@
 
 Filename: cmsis_stream/cg/scheduler/templates/defineConfig.h
 Comment: 
 
 Filename: cmsis_stream/cg/scheduler/templates/dot_template.dot
 Comment: 
 
-Filename: cmsis_stream-1.2.0.dist-info/LICENSE.txt
+Filename: cmsis_stream/cg/scheduler/templates/project/ARMCM55_FP_MVE_config.txt
 Comment: 
 
-Filename: cmsis_stream-1.2.0.dist-info/METADATA
+Filename: cmsis_stream/cg/scheduler/templates/project/Makefile.linux
 Comment: 
 
-Filename: cmsis_stream-1.2.0.dist-info/WHEEL
+Filename: cmsis_stream/cg/scheduler/templates/project/Makefile.mac
 Comment: 
 
-Filename: cmsis_stream-1.2.0.dist-info/entry_points.txt
+Filename: cmsis_stream/cg/scheduler/templates/project/Makefile.windows
 Comment: 
 
-Filename: cmsis_stream-1.2.0.dist-info/top_level.txt
+Filename: cmsis_stream/cg/scheduler/templates/project/main_board.c
 Comment: 
 
-Filename: cmsis_stream-1.2.0.dist-info/RECORD
+Filename: cmsis_stream/cg/scheduler/templates/project/run.bat
+Comment: 
+
+Filename: cmsis_stream/cg/scheduler/templates/project/simple.cproject.yml
+Comment: 
+
+Filename: cmsis_stream/cg/scheduler/templates/project/simple.csolution_ac6.yml
+Comment: 
+
+Filename: cmsis_stream/cg/scheduler/templates/project/start_project_appnodes.h
+Comment: 
+
+Filename: cmsis_stream/cg/scheduler/templates/project/start_project_custom.h
+Comment: 
+
+Filename: cmsis_stream/cg/scheduler/templates/project/start_project_graph.py
+Comment: 
+
+Filename: cmsis_stream/cg/scheduler/templates/project/start_project_main.c
+Comment: 
+
+Filename: cmsis_stream/cg/scheduler/templates/project/vht.clayer.yml
+Comment: 
+
+Filename: cmsis_stream-1.2.1.dist-info/LICENSE.txt
+Comment: 
+
+Filename: cmsis_stream-1.2.1.dist-info/METADATA
+Comment: 
+
+Filename: cmsis_stream-1.2.1.dist-info/WHEEL
+Comment: 
+
+Filename: cmsis_stream-1.2.1.dist-info/entry_points.txt
+Comment: 
+
+Filename: cmsis_stream-1.2.1.dist-info/top_level.txt
+Comment: 
+
+Filename: cmsis_stream-1.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cmsis_stream-1.2.0.dist-info/LICENSE.txt` & `cmsis_stream-1.2.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `cmsis_stream-1.2.0.dist-info/METADATA` & `cmsis_stream-1.2.1.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmsis-stream
-Version: 1.2.0
+Version: 1.2.1
 Summary: CMSIS-Stream graph description
 Home-page: https://github.com/ARM-software/CMSIS-Stream
 Author: Copyright (C) 2010-2023 ARM Limited or its affiliates. All rights reserved.
 Author-email: christophe.favergeon@arm.com
 License: License :: OSI Approved :: Apache Software License
 Project-URL: Bug Reports, https://github.com/ARM-software/CMSIS-Stream/issues
 Project-URL: Source, https://github.com/ARM-software/CMSIS-Stream
@@ -40,14 +40,20 @@
 
 * Define new compute nodes
 * Connect them into a dataflow graph to process streams
 * Generate a C scheduler to run the graph on your target
 
 # Change history
 
+## Version 1.2.1:
+
+* Correct an issue in 1.2.0. Some templates needed
+by the new command line tool had not been included in the
+package.
+
 ## Version 1.2.0:
 
 * The file cg_status.h can now also be created from
 the python package
 
 * A new heapAllocate option has been introduced. When true,
 FIFO and node objects are allocated on the heap and no more
```

