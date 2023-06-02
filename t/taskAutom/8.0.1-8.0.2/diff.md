# Comparing `tmp/taskAutom-8.0.1.tar.gz` & `tmp/taskAutom-8.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskAutom-8.0.1.tar", last modified: Tue May 30 14:00:23 2023, max compression
+gzip compressed data, was "taskAutom-8.0.2.tar", last modified: Fri Jun  2 18:41:30 2023, max compression
```

## Comparing `taskAutom-8.0.1.tar` & `taskAutom-8.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-30 14:00:23.798750 taskAutom-8.0.1/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1527 2023-01-27 17:25:37.000000 taskAutom-8.0.1/LICENSE
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      512 2023-05-30 14:00:23.798750 taskAutom-8.0.1/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     6721 2023-01-30 15:05:44.000000 taskAutom-8.0.1/README.md
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-05-30 14:00:23.798750 taskAutom-8.0.1/setup.cfg
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      999 2023-05-30 14:00:13.000000 taskAutom-8.0.1/setup.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-30 14:00:23.794750 taskAutom-8.0.1/src/
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-30 14:00:23.794750 taskAutom-8.0.1/src/taskAutom/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       52 2023-05-30 14:00:09.000000 taskAutom-8.0.1/src/taskAutom/__init__.py
--rwxrwxr-x   0 lucas     (1000) lucas     (1000)    66714 2023-05-30 13:59:08.000000 taskAutom-8.0.1/src/taskAutom/taskAutom.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-30 14:00:23.798750 taskAutom-8.0.1/taskAutom.egg-info/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      512 2023-05-30 14:00:23.000000 taskAutom-8.0.1/taskAutom.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      279 2023-05-30 14:00:23.000000 taskAutom-8.0.1/taskAutom.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-05-30 14:00:23.000000 taskAutom-8.0.1/taskAutom.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       59 2023-05-30 14:00:23.000000 taskAutom-8.0.1/taskAutom.egg-info/entry_points.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       80 2023-05-30 14:00:23.000000 taskAutom-8.0.1/taskAutom.egg-info/requires.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       14 2023-05-30 14:00:23.000000 taskAutom-8.0.1/taskAutom.egg-info/top_level.txt
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-02 18:41:30.814967 taskAutom-8.0.2/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1527 2023-01-27 17:25:37.000000 taskAutom-8.0.2/LICENSE
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      512 2023-06-02 18:41:30.814967 taskAutom-8.0.2/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     6721 2023-01-30 15:05:44.000000 taskAutom-8.0.2/README.md
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-06-02 18:41:30.814967 taskAutom-8.0.2/setup.cfg
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      999 2023-06-02 18:41:22.000000 taskAutom-8.0.2/setup.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-02 18:41:30.814967 taskAutom-8.0.2/src/
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-02 18:41:30.814967 taskAutom-8.0.2/src/taskAutom/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       52 2023-06-02 18:41:16.000000 taskAutom-8.0.2/src/taskAutom/__init__.py
+-rwxrwxr-x   0 lucas     (1000) lucas     (1000)    66936 2023-06-02 18:38:17.000000 taskAutom-8.0.2/src/taskAutom/taskAutom.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-02 18:41:30.814967 taskAutom-8.0.2/taskAutom.egg-info/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      512 2023-06-02 18:41:30.000000 taskAutom-8.0.2/taskAutom.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      279 2023-06-02 18:41:30.000000 taskAutom-8.0.2/taskAutom.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-06-02 18:41:30.000000 taskAutom-8.0.2/taskAutom.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       59 2023-06-02 18:41:30.000000 taskAutom-8.0.2/taskAutom.egg-info/entry_points.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       80 2023-06-02 18:41:30.000000 taskAutom-8.0.2/taskAutom.egg-info/requires.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       14 2023-06-02 18:41:30.000000 taskAutom-8.0.2/taskAutom.egg-info/top_level.txt
```

### Comparing `taskAutom-8.0.1/LICENSE` & `taskAutom-8.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `taskAutom-8.0.1/PKG-INFO` & `taskAutom-8.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskAutom
-Version: 8.0.1
+Version: 8.0.2
 Summary: A simple task automation tool
 Home-page: https://github.com/laimaretto/taskAutom
 Author: Lucas Aimaretto
 Author-email: laimaretto@gmail.com
 License: BSD 3-clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `taskAutom-8.0.1/README.md` & `taskAutom-8.0.2/README.md`

 * *Files identical despite different names*

### Comparing `taskAutom-8.0.1/setup.py` & `taskAutom-8.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from importlib.metadata import entry_points
 from setuptools import setup
 
 setup(
     name='taskAutom',
-    version='8.0.1',
+    version='8.0.2',
     description='A simple task automation tool',
     long_description='A simple task automation tool for NOKIA SROS based routers',
     long_description_content_type='text/x-rst',
     url='https://github.com/laimaretto/taskAutom',
     author='Lucas Aimaretto',
     author_email='laimaretto@gmail.com',
     license='BSD 3-clause',
```

### Comparing `taskAutom-8.0.1/src/taskAutom/taskAutom.py` & `taskAutom-8.0.2/src/taskAutom/taskAutom.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 import yaml
 import docx
 from docx.enum.style import WD_STYLE_TYPE 
 from docx.enum.text import WD_LINE_SPACING
 from docx.shared import Pt
 
 
-LATEST_VERSION = '8.0.1'
+LATEST_VERSION = '8.0.2'
 
 # Constants
 IP_LOCALHOST  = "127.0.0.1"
 LOG_GLOBAL    = []
 LOG_CONSOLE   = []
 DICT_PARAM    = dict(
 	outputJob        = 0,
@@ -75,15 +75,15 @@
 
 # - Parameters per vendor
 DICT_VENDOR = dict(
 	nokia_sros=dict(
 		START_SCRIPT     = "", 
 		FIRST_LINE       = "/environment no more\n",
 		LAST_LINE        = "\nexit all\n",
-		FIN_SCRIPT       = "",
+		FIN_SCRIPT       = "#FINSCRIPT",
 		VERSION 	     = "show version", # no \n in the end
 		VERSION_REGEX    = "(TiMOS-[A-Z]-\d{1,2}.\d{1,2}.R\d{1,2})",
 		HOSTNAME         = "/show chassis | match Name", # no \n in the end
 		HOSTNAME_REGEX   = "Name\s+:\s(\S+)",
 		HW_TYPE          = "/show chassis | match Type", # no \n in the end
 		HW_TYPE_REGEX    = "Type\s+:\s(.+)",
 		SHOW             = "",
@@ -113,15 +113,15 @@
 		REMOTE_PORT      = 22,
 		SFTP_PORT        = 22,
 	),	
 	nokia_sros_telnet=dict(
 		START_SCRIPT     = "", 
 		FIRST_LINE       = "\n/environment no more\n",
 		LAST_LINE        = "\nexit all\n",
-		FIN_SCRIPT       = "",
+		FIN_SCRIPT       = "#FINSCRIPT",
 		VERSION 	     = "show version", # no \n in the end
 		VERSION_REGEX    = "(TiMOS-[A-Z]-\d{1,2}.\d{1,2}.R\d{1,2})",
 		HOSTNAME         = "/show chassis | match Name", # no \n in the end
 		HOSTNAME_REGEX   = "Name\s+:\s(\S+)",
 		HW_TYPE          = "/show chassis | match Type", # no \n in the end
 		HW_TYPE_REGEX    = "Type\s+:\s(.+)",
 		SHOW             = "",
@@ -936,15 +936,15 @@
 
 		# We update the outputjob relevant information...
 		if self.outputJob == 2:
 			self.connInfo['pluginScript'] = DICT_VENDOR[self.connInfo['deviceType']]['START_SCRIPT'] + \
 											DICT_VENDOR[self.connInfo['deviceType']]['FIRST_LINE'] + \
 											routerInfo['pluginScript'][-1] + \
 											DICT_VENDOR[self.connInfo['deviceType']]['LAST_LINE'] + \
-											DICT_VENDOR[self.connInfo['deviceType']]['FIN_SCRIPT']
+											DICT_VENDOR[self.connInfo['deviceType']]['FIN_SCRIPT']	
 		elif self.outputJob == 3:
 			self.connInfo['ftpFiles'] = routerInfo['ftpFiles']
 			self.connInfo['ftpTotalTxFiles'] = 0
 
 		# Do we you use jumpHosts?
 		if self.connInfo['useSSHTunnel'] is True or dictParam['inventoryFile'] != None:
 			self.connInfo['jumpHost'] = [x for i,x in enumerate(self.connInfo['jumpHosts']) if self.connInfo['num'] % len(self.connInfo['jumpHosts']) == i][0]
@@ -1410,14 +1410,15 @@
 
 		# Sending script to ALU
 		tStart 		 = time.time()
 
 		major_error_list = DICT_VENDOR[connInfo['deviceType']]['MAJOR_ERROR_LIST']
 		minor_error_list = DICT_VENDOR[connInfo['deviceType']]['MINOR_ERROR_LIST']
 		info_error_list  = DICT_VENDOR[connInfo['deviceType']]['INFO_ERROR_LIST']
+		fin_script       = [DICT_VENDOR[connInfo['deviceType']]['FIN_SCRIPT']]
 
 		if connInfo['cronTime']['type'] is not None:
 			datos = connInfo['cronScript']
 			fncPrintConsole(connInfo['strConn'] + "Establishing script with CRON...", show=1)
 		else:
 			datos = connInfo['pluginScript']
 			fncPrintConsole(connInfo['strConn'] + "Running script per line...", show=1)
@@ -1435,14 +1436,16 @@
 			
 			if any([re.compile(error, flags=re.MULTILINE).search(outRx) for error in major_error_list]):
 				aluLogReason = "MajorFailed"
 			elif any([re.compile(error, flags=re.MULTILINE).search(outRx) for error in minor_error_list]):				
 				aluLogReason = "MinorFailed"
 			elif any([re.compile(error, flags=re.MULTILINE).search(outRx) for error in info_error_list]):
 				aluLogReason = "InfoFailed"
+			elif not any([re.compile(error, flags=re.MULTILINE).search(outRx) for error in fin_script]):
+				aluLogReason = 'Incomplete'
 			else:
 				aluLogReason = "SendSuccess"
 
 		fncPrintConsole(connInfo['strConn'] + "Time: " + fncFormatTime(tDiff) + ". Result: " + aluLogReason, show=1)
 
 		connInfo['aluLogReason'] = aluLogReason
 		connInfo['runStatus']    = runStatus
```

### Comparing `taskAutom-8.0.1/taskAutom.egg-info/PKG-INFO` & `taskAutom-8.0.2/taskAutom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskAutom
-Version: 8.0.1
+Version: 8.0.2
 Summary: A simple task automation tool
 Home-page: https://github.com/laimaretto/taskAutom
 Author: Lucas Aimaretto
 Author-email: laimaretto@gmail.com
 License: BSD 3-clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

