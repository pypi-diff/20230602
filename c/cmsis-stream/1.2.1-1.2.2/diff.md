# Comparing `tmp/cmsis_stream-1.2.1-py3-none-any.whl.zip` & `tmp/cmsis_stream-1.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 75082 bytes, number of entries: 66
+Zip file size: 74867 bytes, number of entries: 66
 -rw-rw-rw-  2.0 fat      298 b- defN 23-May-11 12:29 cmsis_stream/__init__.py
 -rw-rw-rw-  2.0 fat      546 b- defN 23-Jun-02 06:34 cmsis_stream/cmsis_stream.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-11 12:29 cmsis_stream/cg/__init__.py
 -rw-rw-rw-  2.0 fat     7448 b- defN 23-May-11 12:29 cmsis_stream/cg/types.py
 -rw-rw-rw-  2.0 fat     1925 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/CFFT.py
 -rw-rw-rw-  2.0 fat     1990 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/Duplicate.py
 -rw-rw-rw-  2.0 fat     1930 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/ICFFT.py
@@ -23,46 +23,46 @@
 -rw-rw-rw-  2.0 fat     2029 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/host/WavSink.py
 -rw-rw-rw-  2.0 fat     2092 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/host/WavSource.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/host/__init__.py
 -rw-rw-rw-  2.0 fat     4018 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/host/message.py
 -rw-rw-rw-  2.0 fat      118 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/__init__.py
 -rw-rw-rw-  2.0 fat     1691 b- defN 23-Jun-02 05:41 cmsis_stream/cg/scheduler/args.py
 -rw-rw-rw-  2.0 fat     3018 b- defN 23-Jun-02 05:04 cmsis_stream/cg/scheduler/ccode.py
--rw-rw-rw-  2.0 fat     6628 b- defN 23-Jun-02 06:51 cmsis_stream/cg/scheduler/config.py
+-rw-rw-rw-  2.0 fat     6615 b- defN 23-Jun-02 08:15 cmsis_stream/cg/scheduler/config.py
 -rw-rw-rw-  2.0 fat    41560 b- defN 23-Jun-02 05:04 cmsis_stream/cg/scheduler/description.py
 -rw-rw-rw-  2.0 fat     1784 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/graphviz.py
 -rw-rw-rw-  2.0 fat    29225 b- defN 23-Jun-02 07:49 cmsis_stream/cg/scheduler/node.py
 -rw-rw-rw-  2.0 fat     1796 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/pythoncode.py
 -rw-rw-rw-  2.0 fat     8260 b- defN 23-Jun-01 13:08 cmsis_stream/cg/scheduler/standard.py
--rw-rw-rw-  2.0 fat    14002 b- defN 23-Jun-02 08:07 cmsis_stream/cg/scheduler/templates/GenericNodes.h
--rw-rw-rw-  2.0 fat     2006 b- defN 23-Jun-02 08:07 cmsis_stream/cg/scheduler/templates/cg_status.h
+-rw-rw-rw-  2.0 fat      188 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/templates/ARMCM55_FP_MVE_config.txt
+-rw-rw-rw-  2.0 fat    14002 b- defN 23-Jun-02 08:20 cmsis_stream/cg/scheduler/templates/GenericNodes.h
+-rw-rw-rw-  2.0 fat      192 b- defN 23-Jun-02 06:56 cmsis_stream/cg/scheduler/templates/Makefile.linux
+-rw-rw-rw-  2.0 fat      267 b- defN 23-Jun-02 06:56 cmsis_stream/cg/scheduler/templates/Makefile.mac
+-rw-rw-rw-  2.0 fat      369 b- defN 23-Jun-02 06:57 cmsis_stream/cg/scheduler/templates/Makefile.windows
+-rw-rw-rw-  2.0 fat     2006 b- defN 23-Jun-02 08:20 cmsis_stream/cg/scheduler/templates/cg_status.h
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
--rw-rw-rw-  2.0 fat      188 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/templates/project/ARMCM55_FP_MVE_config.txt
--rw-rw-rw-  2.0 fat      192 b- defN 23-Jun-02 06:56 cmsis_stream/cg/scheduler/templates/project/Makefile.linux
--rw-rw-rw-  2.0 fat      267 b- defN 23-Jun-02 06:56 cmsis_stream/cg/scheduler/templates/project/Makefile.mac
--rw-rw-rw-  2.0 fat      369 b- defN 23-Jun-02 06:57 cmsis_stream/cg/scheduler/templates/project/Makefile.windows
--rw-rw-rw-  2.0 fat      826 b- defN 23-Jun-02 06:47 cmsis_stream/cg/scheduler/templates/project/main_board.c
--rw-rw-rw-  2.0 fat      212 b- defN 23-Jun-02 06:51 cmsis_stream/cg/scheduler/templates/project/run.bat
--rw-rw-rw-  2.0 fat      589 b- defN 23-Jun-02 07:20 cmsis_stream/cg/scheduler/templates/project/simple.cproject.yml
--rw-rw-rw-  2.0 fat     1416 b- defN 23-Jun-02 07:20 cmsis_stream/cg/scheduler/templates/project/simple.csolution_ac6.yml
--rw-rw-rw-  2.0 fat     2178 b- defN 23-Jun-02 06:48 cmsis_stream/cg/scheduler/templates/project/start_project_appnodes.h
--rw-rw-rw-  2.0 fat       73 b- defN 23-Jun-02 06:10 cmsis_stream/cg/scheduler/templates/project/start_project_custom.h
--rw-rw-rw-  2.0 fat     1798 b- defN 23-Jun-02 06:26 cmsis_stream/cg/scheduler/templates/project/start_project_graph.py
--rw-rw-rw-  2.0 fat      197 b- defN 23-Jun-02 06:05 cmsis_stream/cg/scheduler/templates/project/start_project_main.c
--rw-rw-rw-  2.0 fat      860 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/templates/project/vht.clayer.yml
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-02 08:07 cmsis_stream-1.2.1.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     3253 b- defN 23-Jun-02 08:07 cmsis_stream-1.2.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-02 08:07 cmsis_stream-1.2.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       59 b- defN 23-Jun-02 08:07 cmsis_stream-1.2.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       13 b- defN 23-Jun-02 08:07 cmsis_stream-1.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     6488 b- defN 23-Jun-02 08:07 cmsis_stream-1.2.1.dist-info/RECORD
-66 files, 210969 bytes uncompressed, 64430 bytes compressed:  69.5%
+-rw-rw-rw-  2.0 fat      826 b- defN 23-Jun-02 06:47 cmsis_stream/cg/scheduler/templates/main_board.c
+-rw-rw-rw-  2.0 fat      212 b- defN 23-Jun-02 06:51 cmsis_stream/cg/scheduler/templates/run.bat
+-rw-rw-rw-  2.0 fat      589 b- defN 23-Jun-02 07:20 cmsis_stream/cg/scheduler/templates/simple.cproject.yml
+-rw-rw-rw-  2.0 fat     1416 b- defN 23-Jun-02 07:20 cmsis_stream/cg/scheduler/templates/simple.csolution_ac6.yml
+-rw-rw-rw-  2.0 fat     2178 b- defN 23-Jun-02 06:48 cmsis_stream/cg/scheduler/templates/start_project_appnodes.h
+-rw-rw-rw-  2.0 fat       73 b- defN 23-Jun-02 06:10 cmsis_stream/cg/scheduler/templates/start_project_custom.h
+-rw-rw-rw-  2.0 fat     1798 b- defN 23-Jun-02 06:26 cmsis_stream/cg/scheduler/templates/start_project_graph.py
+-rw-rw-rw-  2.0 fat      197 b- defN 23-Jun-02 06:05 cmsis_stream/cg/scheduler/templates/start_project_main.c
+-rw-rw-rw-  2.0 fat      860 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/templates/vht.clayer.yml
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-02 08:20 cmsis_stream-1.2.2.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     3253 b- defN 23-Jun-02 08:20 cmsis_stream-1.2.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-02 08:20 cmsis_stream-1.2.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       59 b- defN 23-Jun-02 08:20 cmsis_stream-1.2.2.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Jun-02 08:20 cmsis_stream-1.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     6384 b- defN 23-Jun-02 08:20 cmsis_stream-1.2.2.dist-info/RECORD
+66 files, 210852 bytes uncompressed, 64423 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -96,17 +96,29 @@
 
 Filename: cmsis_stream/cg/scheduler/pythoncode.py
 Comment: 
 
 Filename: cmsis_stream/cg/scheduler/standard.py
 Comment: 
 
+Filename: cmsis_stream/cg/scheduler/templates/ARMCM55_FP_MVE_config.txt
+Comment: 
+
 Filename: cmsis_stream/cg/scheduler/templates/GenericNodes.h
 Comment: 
 
+Filename: cmsis_stream/cg/scheduler/templates/Makefile.linux
+Comment: 
+
+Filename: cmsis_stream/cg/scheduler/templates/Makefile.mac
+Comment: 
+
+Filename: cmsis_stream/cg/scheduler/templates/Makefile.windows
+Comment: 
+
 Filename: cmsis_stream/cg/scheduler/templates/cg_status.h
 Comment: 
 
 Filename: cmsis_stream/cg/scheduler/templates/cmsis.cpp
 Comment: 
 
 Filename: cmsis_stream/cg/scheduler/templates/cmsis.py
@@ -135,65 +147,53 @@
 
 Filename: cmsis_stream/cg/scheduler/templates/defineConfig.h
 Comment: 
 
 Filename: cmsis_stream/cg/scheduler/templates/dot_template.dot
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/project/ARMCM55_FP_MVE_config.txt
-Comment: 
-
-Filename: cmsis_stream/cg/scheduler/templates/project/Makefile.linux
-Comment: 
-
-Filename: cmsis_stream/cg/scheduler/templates/project/Makefile.mac
-Comment: 
-
-Filename: cmsis_stream/cg/scheduler/templates/project/Makefile.windows
-Comment: 
-
-Filename: cmsis_stream/cg/scheduler/templates/project/main_board.c
+Filename: cmsis_stream/cg/scheduler/templates/main_board.c
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/project/run.bat
+Filename: cmsis_stream/cg/scheduler/templates/run.bat
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/project/simple.cproject.yml
+Filename: cmsis_stream/cg/scheduler/templates/simple.cproject.yml
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/project/simple.csolution_ac6.yml
+Filename: cmsis_stream/cg/scheduler/templates/simple.csolution_ac6.yml
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/project/start_project_appnodes.h
+Filename: cmsis_stream/cg/scheduler/templates/start_project_appnodes.h
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/project/start_project_custom.h
+Filename: cmsis_stream/cg/scheduler/templates/start_project_custom.h
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/project/start_project_graph.py
+Filename: cmsis_stream/cg/scheduler/templates/start_project_graph.py
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/project/start_project_main.c
+Filename: cmsis_stream/cg/scheduler/templates/start_project_main.c
 Comment: 
 
-Filename: cmsis_stream/cg/scheduler/templates/project/vht.clayer.yml
+Filename: cmsis_stream/cg/scheduler/templates/vht.clayer.yml
 Comment: 
 
-Filename: cmsis_stream-1.2.1.dist-info/LICENSE.txt
+Filename: cmsis_stream-1.2.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: cmsis_stream-1.2.1.dist-info/METADATA
+Filename: cmsis_stream-1.2.2.dist-info/METADATA
 Comment: 
 
-Filename: cmsis_stream-1.2.1.dist-info/WHEEL
+Filename: cmsis_stream-1.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: cmsis_stream-1.2.1.dist-info/entry_points.txt
+Filename: cmsis_stream-1.2.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: cmsis_stream-1.2.1.dist-info/top_level.txt
+Filename: cmsis_stream-1.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: cmsis_stream-1.2.1.dist-info/RECORD
+Filename: cmsis_stream-1.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cmsis_stream/cg/scheduler/config.py

```diff
@@ -199,11 +199,11 @@
               ,"simple.csolution_ac6.yml":"simple.csolution_ac6.yml"
               ,"simple.cproject.yml":"simple.cproject.yml"
               ,"vht.clayer.yml":"vht.clayer.yml"
               ,"run.bat":"run_vht.bat"
               ,"ARMCM55_FP_MVE_config.txt":"ARMCM55_FP_MVE_config.txt"};
     for src_name in all_files:
         dst_name = all_files[src_name]
-        ctemplate = env.get_template(f"project/{src_name}")
+        ctemplate = env.get_template(src_name)
         path = os.path.join(project_name,dst_name)
         with open(path,"w") as f:
             print(ctemplate.render(),file=f)
```

## Comparing `cmsis_stream/cg/scheduler/templates/project/main_board.c` & `cmsis_stream/cg/scheduler/templates/main_board.c`

 * *Files identical despite different names*

## Comparing `cmsis_stream/cg/scheduler/templates/project/simple.cproject.yml` & `cmsis_stream/cg/scheduler/templates/simple.cproject.yml`

 * *Files identical despite different names*

## Comparing `cmsis_stream/cg/scheduler/templates/project/simple.csolution_ac6.yml` & `cmsis_stream/cg/scheduler/templates/simple.csolution_ac6.yml`

 * *Files identical despite different names*

## Comparing `cmsis_stream/cg/scheduler/templates/project/start_project_appnodes.h` & `cmsis_stream/cg/scheduler/templates/start_project_appnodes.h`

 * *Files identical despite different names*

## Comparing `cmsis_stream/cg/scheduler/templates/project/start_project_graph.py` & `cmsis_stream/cg/scheduler/templates/start_project_graph.py`

 * *Files identical despite different names*

## Comparing `cmsis_stream/cg/scheduler/templates/project/vht.clayer.yml` & `cmsis_stream/cg/scheduler/templates/vht.clayer.yml`

 * *Files identical despite different names*

## Comparing `cmsis_stream-1.2.1.dist-info/LICENSE.txt` & `cmsis_stream-1.2.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `cmsis_stream-1.2.1.dist-info/METADATA` & `cmsis_stream-1.2.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmsis-stream
-Version: 1.2.1
+Version: 1.2.2
 Summary: CMSIS-Stream graph description
 Home-page: https://github.com/ARM-software/CMSIS-Stream
 Author: Copyright (C) 2010-2023 ARM Limited or its affiliates. All rights reserved.
 Author-email: christophe.favergeon@arm.com
 License: License :: OSI Approved :: Apache Software License
 Project-URL: Bug Reports, https://github.com/ARM-software/CMSIS-Stream/issues
 Project-URL: Source, https://github.com/ARM-software/CMSIS-Stream
```

## Comparing `cmsis_stream-1.2.1.dist-info/RECORD` & `cmsis_stream-1.2.2.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -22,45 +22,45 @@
 cmsis_stream/cg/nodes/host/WavSink.py,sha256=ldo5e9wjaIp0Ef6GvRgZIICuuk3H1V7B-hn1et6S7Wo,2029
 cmsis_stream/cg/nodes/host/WavSource.py,sha256=KywcbHsrCqrAQD6HuZaxOxVj_ekYDYIgzx_6Nh2R4Gk,2092
 cmsis_stream/cg/nodes/host/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cmsis_stream/cg/nodes/host/message.py,sha256=e2hto5-Ly08sUCKN8F94qH3O3lAxcGGIGBLkf6cLJCY,4018
 cmsis_stream/cg/scheduler/__init__.py,sha256=-GMWFk8b3LpReDjD7yHF_SLrFDu5PRZuxN1RbjkY6nk,118
 cmsis_stream/cg/scheduler/args.py,sha256=mepFm7CJa2wnB-21a-h1FrufP5KtI78l_B3HNb87ayk,1691
 cmsis_stream/cg/scheduler/ccode.py,sha256=f57rHk2gtgkikywW_ZEkdXlibV4wnHbOQ5vi0fHRcME,3018
-cmsis_stream/cg/scheduler/config.py,sha256=x5mQRXHxqGiNS8czDYuqul-r0GDeobFod_8QrXrVmVI,6628
+cmsis_stream/cg/scheduler/config.py,sha256=IOnoVpfq6PuCgLyaOiUgnUPtuxq6w6txaWB4tZmg4NU,6615
 cmsis_stream/cg/scheduler/description.py,sha256=6ob9d7bfo1TXUBFWq9aPnnY1wFPklsqi7poXPECxFA4,41560
 cmsis_stream/cg/scheduler/graphviz.py,sha256=wmbSzhIlOD9Z1E5NBsNklk4LvpaLQfs9Tmw-vAxwSPM,1784
 cmsis_stream/cg/scheduler/node.py,sha256=LJuuFbkWp8xJALM4aSXASaisYkhDQVfAfKlz0sQYnq4,29225
 cmsis_stream/cg/scheduler/pythoncode.py,sha256=bDtCVYvgtLO_wpl33HlyyAEZtfyW6wHyANQsdPvdlBA,1796
 cmsis_stream/cg/scheduler/standard.py,sha256=EEPGxII61ykghjLnVSkVV2s5DW2ZHfKI2ryhnDByhkU,8260
+cmsis_stream/cg/scheduler/templates/ARMCM55_FP_MVE_config.txt,sha256=Yn4YtMgyACdeesvFcPkP1xZ9Q8rIEarIAIrJeQNn3sw,188
 cmsis_stream/cg/scheduler/templates/GenericNodes.h,sha256=6r6w3HloYzH3u8WGz5mDjEyhOkdcumxf3o4qOjx2CM0,14002
+cmsis_stream/cg/scheduler/templates/Makefile.linux,sha256=4x9Z6tbRIswUvBQuTuD9t0Co-DCwEGevAnaMc3CC5NU,192
+cmsis_stream/cg/scheduler/templates/Makefile.mac,sha256=-2ldN02pnOEKwS1QqxY9-97qnUse6MEDZO9Ru1CkplQ,267
+cmsis_stream/cg/scheduler/templates/Makefile.windows,sha256=p6ic8tdH0H0Fm6A8-877JIvIqgnhaScSjUKNSgB7Wb8,369
 cmsis_stream/cg/scheduler/templates/cg_status.h,sha256=1ZBdMG2s9FMyTzdvFtxpPIK624-jnfRd_Q2Qxe_MwTM,2006
 cmsis_stream/cg/scheduler/templates/cmsis.cpp,sha256=yNiZSHN-riYPkzCenN6UUoZD9ZieCI8L9viXYkQCCz0,431
 cmsis_stream/cg/scheduler/templates/cmsis.py,sha256=wbXrZ1fWz2YmD-yyvMshlaXvWXgTmfKokVEFu6SwAVk,279
 cmsis_stream/cg/scheduler/templates/cmsisCheck.cpp,sha256=bo05ISPFatzhi09c36ioA4HSJUtJc30k3T-z31oWN-8,674
 cmsis_stream/cg/scheduler/templates/cmsisNode.cpp,sha256=luXUXScO1ncXx1m2kI2e40DyjobwbwVucCY0QernoGc,297
 cmsis_stream/cg/scheduler/templates/code.cpp,sha256=uiJEAmZyGoMq_AqYqZ3aXRyX9L7cRKdkUFazGLc1eP0,1232
 cmsis_stream/cg/scheduler/templates/code.h,sha256=BULWyJn9FAU6laXpg6UjyP5TtHHMCW_3zTccu_EtjKU,1111
 cmsis_stream/cg/scheduler/templates/code.py,sha256=eOK6r2DkCD-JftAKAi0K3PxOwidRWtdtal4N8_xC6wk,2199
 cmsis_stream/cg/scheduler/templates/codeSwitch.cpp,sha256=6fn_IVXZy77h8TQN2vSsuwMUVJFjyPtVzURjhnriAo0,3185
 cmsis_stream/cg/scheduler/templates/commonc.cpp,sha256=nmlbxVoBiujXLYerA056T_GPRL-LZSo0IFcz6BHdTHc,4482
 cmsis_stream/cg/scheduler/templates/defineConfig.h,sha256=h9R25-RcgG_kDKg4-xsGih4yPnffdNbZwkZMe5UXmhA,1051
 cmsis_stream/cg/scheduler/templates/dot_template.dot,sha256=GJyuIQkdt3RZvq2SRSBYrmuWj7QW9T4wVO-1GRGB8B0,4848
-cmsis_stream/cg/scheduler/templates/project/ARMCM55_FP_MVE_config.txt,sha256=Yn4YtMgyACdeesvFcPkP1xZ9Q8rIEarIAIrJeQNn3sw,188
-cmsis_stream/cg/scheduler/templates/project/Makefile.linux,sha256=4x9Z6tbRIswUvBQuTuD9t0Co-DCwEGevAnaMc3CC5NU,192
-cmsis_stream/cg/scheduler/templates/project/Makefile.mac,sha256=-2ldN02pnOEKwS1QqxY9-97qnUse6MEDZO9Ru1CkplQ,267
-cmsis_stream/cg/scheduler/templates/project/Makefile.windows,sha256=p6ic8tdH0H0Fm6A8-877JIvIqgnhaScSjUKNSgB7Wb8,369
-cmsis_stream/cg/scheduler/templates/project/main_board.c,sha256=DJCtYtjQimSzK2OeN4c38qAFKVSmK5pc1FCE8m8KwgU,826
-cmsis_stream/cg/scheduler/templates/project/run.bat,sha256=kYGYp4pNuKJFiWPqQyBoT0u7MXzuth6iTZ7CTBZVfDg,212
-cmsis_stream/cg/scheduler/templates/project/simple.cproject.yml,sha256=1Zpzt5Ebl30KDJ-5nh_9Ypg-igqrPiA_ek_2kGAJGzc,589
-cmsis_stream/cg/scheduler/templates/project/simple.csolution_ac6.yml,sha256=0VoVxmTd-uY5ChO-uLZeNKZ7nd9GRB1aruqgSavSnFc,1416
-cmsis_stream/cg/scheduler/templates/project/start_project_appnodes.h,sha256=LDAWX_fxyxi9y1WScVRdx0mWBQX67y06DYPTWGks1As,2178
-cmsis_stream/cg/scheduler/templates/project/start_project_custom.h,sha256=_Hk_xhNBISqUU61sXkhmQfeG9YjmoyVPD5TD7a_P0lc,73
-cmsis_stream/cg/scheduler/templates/project/start_project_graph.py,sha256=gTSFIiNYAVGFSSQ-aSs6_BL6bMbk0oEIjk8d32fr9AM,1798
-cmsis_stream/cg/scheduler/templates/project/start_project_main.c,sha256=CFz0ZKrUafNi9bF3fIVcBBGhrwFNoxmxxODSaDCO4sQ,197
-cmsis_stream/cg/scheduler/templates/project/vht.clayer.yml,sha256=KYF6zwS9iDaoH9iUWGZjuoX880f-Az7-LnQIsaAIRTQ,860
-cmsis_stream-1.2.1.dist-info/LICENSE.txt,sha256=4DukHX-rIHAHaf5BGLq1DYAMt0-ZA1OgXS9f_xwig2M,11558
-cmsis_stream-1.2.1.dist-info/METADATA,sha256=nOOUMyrixNZQvLkRlscfwsymZp_ZNygu87jquDYQ0rk,3253
-cmsis_stream-1.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-cmsis_stream-1.2.1.dist-info/entry_points.txt,sha256=WOEqwaMTN0K5CT8Yfd-z53mE82xfyzsM16a0eR4Ipds,59
-cmsis_stream-1.2.1.dist-info/top_level.txt,sha256=a7ZhPCd-XkrgWSSuOstN5Jgqe60MV4q7-tWximJBomA,13
-cmsis_stream-1.2.1.dist-info/RECORD,,
+cmsis_stream/cg/scheduler/templates/main_board.c,sha256=DJCtYtjQimSzK2OeN4c38qAFKVSmK5pc1FCE8m8KwgU,826
+cmsis_stream/cg/scheduler/templates/run.bat,sha256=kYGYp4pNuKJFiWPqQyBoT0u7MXzuth6iTZ7CTBZVfDg,212
+cmsis_stream/cg/scheduler/templates/simple.cproject.yml,sha256=1Zpzt5Ebl30KDJ-5nh_9Ypg-igqrPiA_ek_2kGAJGzc,589
+cmsis_stream/cg/scheduler/templates/simple.csolution_ac6.yml,sha256=0VoVxmTd-uY5ChO-uLZeNKZ7nd9GRB1aruqgSavSnFc,1416
+cmsis_stream/cg/scheduler/templates/start_project_appnodes.h,sha256=LDAWX_fxyxi9y1WScVRdx0mWBQX67y06DYPTWGks1As,2178
+cmsis_stream/cg/scheduler/templates/start_project_custom.h,sha256=_Hk_xhNBISqUU61sXkhmQfeG9YjmoyVPD5TD7a_P0lc,73
+cmsis_stream/cg/scheduler/templates/start_project_graph.py,sha256=gTSFIiNYAVGFSSQ-aSs6_BL6bMbk0oEIjk8d32fr9AM,1798
+cmsis_stream/cg/scheduler/templates/start_project_main.c,sha256=CFz0ZKrUafNi9bF3fIVcBBGhrwFNoxmxxODSaDCO4sQ,197
+cmsis_stream/cg/scheduler/templates/vht.clayer.yml,sha256=KYF6zwS9iDaoH9iUWGZjuoX880f-Az7-LnQIsaAIRTQ,860
+cmsis_stream-1.2.2.dist-info/LICENSE.txt,sha256=4DukHX-rIHAHaf5BGLq1DYAMt0-ZA1OgXS9f_xwig2M,11558
+cmsis_stream-1.2.2.dist-info/METADATA,sha256=nxY3JaWaH92IgKDeKQtcLujPRWDt1F0ffEmutStUVsg,3253
+cmsis_stream-1.2.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+cmsis_stream-1.2.2.dist-info/entry_points.txt,sha256=WOEqwaMTN0K5CT8Yfd-z53mE82xfyzsM16a0eR4Ipds,59
+cmsis_stream-1.2.2.dist-info/top_level.txt,sha256=a7ZhPCd-XkrgWSSuOstN5Jgqe60MV4q7-tWximJBomA,13
+cmsis_stream-1.2.2.dist-info/RECORD,,
```

