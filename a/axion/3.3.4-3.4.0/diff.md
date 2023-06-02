# Comparing `tmp/axion-3.3.4-cp311-cp311-win_amd64.whl.zip` & `tmp/axion-3.4.0-cp311-cp311-macosx_10_9_universal2.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 631072 bytes, number of entries: 20
--rw-rw-rw-  2.0 fat     1080 b- defN 23-May-22 04:08 axion-3.3.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1288 b- defN 23-May-22 04:08 axion-3.3.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-May-22 04:08 axion-3.3.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-May-22 04:08 axion-3.3.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      376 b- defN 23-May-22 04:08 axion-3.3.4.dist-info/RECORD
--rw-rw-rw-  2.0 fat    20992 b- defN 23-May-22 04:08 axion/__init__.pyd
--rw-rw-rw-  2.0 fat    79872 b- defN 23-May-22 04:08 axion/executor.pyd
--rw-rw-rw-  2.0 fat   288256 b- defN 23-May-22 04:08 axion/factory.pyd
--rw-rw-rw-  2.0 fat    78336 b- defN 23-May-22 04:08 axion/pipeline.pyd
--rw-rw-rw-  2.0 fat    52736 b- defN 23-May-22 04:08 axion/queues.pyd
--rw-rw-rw-  2.0 fat   208384 b- defN 23-May-22 04:08 axion/recorder.pyd
--rw-rw-rw-  2.0 fat    54272 b- defN 23-May-22 04:08 axion/scheduler.pyd
--rw-rw-rw-  2.0 fat    71168 b- defN 23-May-22 04:08 axion/service.pyd
--rw-rw-rw-  2.0 fat    54784 b- defN 23-May-22 04:08 axion/thread.pyd
--rw-rw-rw-  2.0 fat    22016 b- defN 23-May-22 04:08 axion/inst/__init__.pyd
--rw-rw-rw-  2.0 fat    49664 b- defN 23-May-22 04:08 axion/inst/ibase.pyd
--rw-rw-rw-  2.0 fat   222208 b- defN 23-May-22 04:08 axion/inst/nbase.pyd
--rw-rw-rw-  2.0 fat    85504 b- defN 23-May-22 04:08 axion/inst/sbase.pyd
--rw-rw-rw-  2.0 fat    62976 b- defN 23-May-22 04:08 axion/inst/tbase.pyd
--rw-rw-rw-  2.0 fat    61440 b- defN 23-May-22 04:08 axion/inst/utility.pyd
-20 files, 1415455 bytes uncompressed, 628668 bytes compressed:  55.6%
+Zip file size: 1466141 bytes, number of entries: 20
+-rw-r--r--  2.0 unx     1059 b- defN 23-Jun-02 02:54 axion-3.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1234 b- defN 23-Jun-02 02:54 axion-3.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      115 b- defN 23-Jun-02 02:54 axion-3.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-02 02:54 axion-3.4.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      376 b- defN 23-Jun-02 02:54 axion-3.4.0.dist-info/RECORD
+-rwxr-xr-x  2.0 unx   122336 b- defN 23-Jun-02 02:52 axion/__init__.so
+-rwxr-xr-x  2.0 unx   305424 b- defN 23-Jun-02 02:53 axion/executor.so
+-rwxr-xr-x  2.0 unx   875375 b- defN 23-Jun-02 02:52 axion/factory.so
+-rwxr-xr-x  2.0 unx   289360 b- defN 23-Jun-02 02:53 axion/pipeline.so
+-rwxr-xr-x  2.0 unx   217534 b- defN 23-Jun-02 02:51 axion/queues.so
+-rwxr-xr-x  2.0 unx   726400 b- defN 23-Jun-02 02:52 axion/recorder.so
+-rwxr-xr-x  2.0 unx   218961 b- defN 23-Jun-02 02:53 axion/scheduler.so
+-rwxr-xr-x  2.0 unx   272655 b- defN 23-Jun-02 02:51 axion/service.so
+-rwxr-xr-x  2.0 unx   220350 b- defN 23-Jun-02 02:51 axion/thread.so
+-rwxr-xr-x  2.0 unx   122464 b- defN 23-Jun-02 02:54 axion/inst/__init__.so
+-rwxr-xr-x  2.0 unx   216253 b- defN 23-Jun-02 02:53 axion/inst/ibase.so
+-rwxr-xr-x  2.0 unx   729005 b- defN 23-Jun-02 02:54 axion/inst/nbase.so
+-rwxr-xr-x  2.0 unx   309485 b- defN 23-Jun-02 02:54 axion/inst/sbase.so
+-rwxr-xr-x  2.0 unx   255133 b- defN 23-Jun-02 02:54 axion/inst/tbase.so
+-rwxr-xr-x  2.0 unx   236191 b- defN 23-Jun-02 02:53 axion/inst/utility.so
+20 files, 5119711 bytes uncompressed, 1463767 bytes compressed:  71.4%
```

## zipnote {}

```diff
@@ -1,61 +1,61 @@
-Filename: axion-3.3.4.dist-info/LICENSE
+Filename: axion-3.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: axion-3.3.4.dist-info/METADATA
+Filename: axion-3.4.0.dist-info/METADATA
 Comment: 
 
-Filename: axion-3.3.4.dist-info/WHEEL
+Filename: axion-3.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: axion-3.3.4.dist-info/top_level.txt
+Filename: axion-3.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: axion-3.3.4.dist-info/RECORD
+Filename: axion-3.4.0.dist-info/RECORD
 Comment: 
 
-Filename: axion/__init__.pyd
+Filename: axion/__init__.so
 Comment: 
 
-Filename: axion/executor.pyd
+Filename: axion/executor.so
 Comment: 
 
-Filename: axion/factory.pyd
+Filename: axion/factory.so
 Comment: 
 
-Filename: axion/pipeline.pyd
+Filename: axion/pipeline.so
 Comment: 
 
-Filename: axion/queues.pyd
+Filename: axion/queues.so
 Comment: 
 
-Filename: axion/recorder.pyd
+Filename: axion/recorder.so
 Comment: 
 
-Filename: axion/scheduler.pyd
+Filename: axion/scheduler.so
 Comment: 
 
-Filename: axion/service.pyd
+Filename: axion/service.so
 Comment: 
 
-Filename: axion/thread.pyd
+Filename: axion/thread.so
 Comment: 
 
-Filename: axion/inst/__init__.pyd
+Filename: axion/inst/__init__.so
 Comment: 
 
-Filename: axion/inst/ibase.pyd
+Filename: axion/inst/ibase.so
 Comment: 
 
-Filename: axion/inst/nbase.pyd
+Filename: axion/inst/nbase.so
 Comment: 
 
-Filename: axion/inst/sbase.pyd
+Filename: axion/inst/sbase.so
 Comment: 
 
-Filename: axion/inst/tbase.pyd
+Filename: axion/inst/tbase.so
 Comment: 
 
-Filename: axion/inst/utility.pyd
+Filename: axion/inst/utility.so
 Comment: 
 
 Zip file comment:
```

## Comparing `axion-3.3.4.dist-info/METADATA` & `axion-3.4.0.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-Metadata-Version: 2.1
-Name: axion
-Version: 3.3.4
-Summary: Dream It Possible!
-Home-page: https://gitee.com/
-Author: YL Feng
-Author-email: fengyulong@pku.edu.cn
-License: MIT
-Project-URL: source, https://gitee.com
-Keywords: Hello,World!
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: Chinese (Simplified)
-Classifier: Natural Language :: English
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.10.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy (>=1.20.0)
-Requires-Dist: h5py (>=3.0.0)
-Requires-Dist: psutil (>=5.8.0)
-Requires-Dist: srpc (>=4.2.8)
-Requires-Dist: zee (>=0.0.2)
-Requires-Dist: dill (>=0.3.4)
-Requires-Dist: networkx (>=2.5.0)
-Requires-Dist: pyparsing (>3.0.0)
-
-#### 介绍
-
-
-#### 软件架构
-
-
-#### 安装教程
-
-
-#### 使用说明
-
-
-#### 参与贡献
-
-
-#### 特技
-
-
-
-
-
+Metadata-Version: 2.1
+Name: axion
+Version: 3.4.0
+Summary: Dream It Possible!
+Home-page: https://gitee.com/
+Author: YL Feng
+Author-email: fengyulong@pku.edu.cn
+License: MIT
+Project-URL: source, https://gitee.com
+Keywords: Hello,World!
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: Chinese (Simplified)
+Classifier: Natural Language :: English
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Physics
+Requires-Python: >=3.10.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy (>=1.20.0)
+Requires-Dist: h5py (>=3.0.0)
+Requires-Dist: psutil (>=5.8.0)
+Requires-Dist: srpc (>=4.2.8)
+Requires-Dist: zee (>=0.0.2)
+Requires-Dist: dill (>=0.3.4)
+Requires-Dist: networkx (>=2.5.0)
+Requires-Dist: pyparsing (>3.0.0)
+
+#### 介绍
+
+
+#### 软件架构
+
+
+#### 安装教程
+
+
+#### 使用说明
+
+
+#### 参与贡献
+
+
+#### 特技
+
+
+
+
+
```

