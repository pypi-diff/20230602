# Comparing `tmp/GISPython-59.1.tar.gz` & `tmp/GISPython-59.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\GISPython-59.1.tar", last modified: Thu Mar 23 07:15:11 2023, max compression
+gzip compressed data, was "dist\GISPython-59.2.tar", last modified: Fri Jun  2 11:14:51 2023, max compression
```

## Comparing `GISPython-59.1.tar` & `GISPython-59.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-03-23 07:15:11.000000 GISPython-59.1/
--rw-rw-rw-   0        0        0       61 2018-07-19 06:01:11.000000 GISPython-59.1/.gitignore
--rw-rw-rw-   0        0        0      142 2018-07-19 06:01:11.000000 GISPython-59.1/.pypirc
-drwxrwxrwx   0        0        0        0 2023-03-23 07:15:11.000000 GISPython-59.1/GISPython/
--rw-rw-rw-   0        0        0    14560 2022-01-23 15:44:36.000000 GISPython-59.1/GISPython/AGServerHelper.py
--rw-rw-rw-   0        0        0    35027 2022-08-29 12:45:25.000000 GISPython-59.1/GISPython/AGServerHelperNTLM.py
--rw-rw-rw-   0        0        0    23880 2022-01-23 15:44:36.000000 GISPython-59.1/GISPython/AGServerHelperToken.py
--rw-rw-rw-   0        0        0     4254 2018-07-19 06:01:12.000000 GISPython-59.1/GISPython/CachingHelper.py
--rw-rw-rw-   0        0        0     4731 2018-07-19 06:01:12.000000 GISPython-59.1/GISPython/FTPHleper.py
--rw-rw-rw-   0        0        0    22306 2022-02-21 08:26:12.000000 GISPython-59.1/GISPython/GDBHelper.py
--rw-rw-rw-   0        0        0     8354 2018-07-19 06:01:12.000000 GISPython-59.1/GISPython/GDPSyncroniserHelper.py
--rw-rw-rw-   0        0        0    26395 2022-03-16 23:36:27.000000 GISPython-59.1/GISPython/GDPSyncroniserHelper2.py
--rw-rw-rw-   0        0        0    12712 2022-04-21 07:54:14.000000 GISPython-59.1/GISPython/GISPythonModule.py
--rw-rw-rw-   0        0        0     2251 2018-07-19 06:01:12.000000 GISPython-59.1/GISPython/GISPythonTool.py
--rw-rw-rw-   0        0        0    19237 2022-11-06 11:41:17.000000 GISPython-59.1/GISPython/GISPythonToolBase.py
--rw-rw-rw-   0        0        0     3368 2019-09-06 06:11:22.000000 GISPython-59.1/GISPython/JsonParamsHelper.py
--rw-rw-rw-   0        0        0     4023 2023-03-23 06:54:39.000000 GISPython-59.1/GISPython/MailHelper.py
--rw-rw-rw-   0        0        0     9520 2022-03-18 07:59:10.000000 GISPython-59.1/GISPython/MXDHelper.py
--rw-rw-rw-   0        0        0      858 2018-07-19 06:01:12.000000 GISPython-59.1/GISPython/MyError.py
-drwxrwxrwx   0        0        0        0 2023-03-23 07:15:11.000000 GISPython-59.1/GISPython/PShell/
--rw-rw-rw-   0        0        0      696 2018-07-19 06:01:12.000000 GISPython-59.1/GISPython/PShell/BackupOldFiles.ps1
--rw-rw-rw-   0        0        0      410 2018-07-19 06:01:12.000000 GISPython-59.1/GISPython/PShell/ClearDir.ps1
--rw-rw-rw-   0        0        0      661 2018-07-19 06:01:12.000000 GISPython-59.1/GISPython/PShell/GetLog.ps1
--rw-rw-rw-   0        0        0    20804 2022-03-20 16:00:04.000000 GISPython-59.1/GISPython/PublisherHealper.py
--rw-rw-rw-   0        0        0      658 2018-07-19 06:01:12.000000 GISPython-59.1/GISPython/RarHelper.py
--rw-rw-rw-   0        0        0     2479 2022-07-15 16:06:08.000000 GISPython-59.1/GISPython/SFTPHelper.py
--rw-rw-rw-   0        0        0    18601 2018-12-03 01:07:07.000000 GISPython-59.1/GISPython/SimpleFileOps.py
--rw-rw-rw-   0        0        0     5836 2020-08-12 04:42:32.000000 GISPython-59.1/GISPython/SimpleFileOpsSafe.py
--rw-rw-rw-   0        0        0    12757 2022-04-21 07:43:29.000000 GISPython-59.1/GISPython/SysGISTools.py
--rw-rw-rw-   0        0        0      160 2023-03-23 07:14:14.000000 GISPython-59.1/GISPython/SysGISToolsSysParams.py
--rw-rw-rw-   0        0        0     1701 2019-05-24 06:27:11.000000 GISPython-59.1/GISPython/SysTools_unittest.py
--rw-rw-rw-   0        0        0     2371 2022-03-14 22:32:29.000000 GISPython-59.1/GISPython/TimerHelper.py
--rw-rw-rw-   0        0        0     3311 2022-01-20 07:27:45.000000 GISPython-59.1/GISPython/xmlParamsHealper.py
--rw-rw-rw-   0        0        0     3764 2022-01-20 07:27:45.000000 GISPython-59.1/GISPython/ZipHelper.py
--rw-rw-rw-   0        0        0      906 2018-07-19 06:01:11.000000 GISPython-59.1/GISPython/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-23 07:15:11.000000 GISPython-59.1/GISPython.egg-info/
--rw-rw-rw-   0        0        0        1 2023-03-23 07:15:10.000000 GISPython-59.1/GISPython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1172 2023-03-23 07:15:10.000000 GISPython-59.1/GISPython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       79 2023-03-23 07:15:10.000000 GISPython-59.1/GISPython.egg-info/requires.txt
--rw-rw-rw-   0        0        0     1087 2023-03-23 07:15:10.000000 GISPython-59.1/GISPython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       10 2023-03-23 07:15:10.000000 GISPython-59.1/GISPython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35793 2018-07-19 06:01:12.000000 GISPython-59.1/LICENSE
--rw-rw-rw-   0        0        0      274 2018-07-19 06:01:12.000000 GISPython-59.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1172 2023-03-23 07:15:11.000000 GISPython-59.1/PKG-INFO
--rwxrwxrwx   0        0        0      718 2018-08-15 04:52:21.000000 GISPython-59.1/pypi_upload.bat
--rw-rw-rw-   0        0        0    17075 2019-05-24 06:27:11.000000 GISPython-59.1/README.md
--rw-rw-rw-   0        0        0       63 2018-07-19 06:01:12.000000 GISPython-59.1/README.rst
--rw-rw-rw-   0        0        0       42 2023-03-23 07:15:11.000000 GISPython-59.1/setup.cfg
--rw-rw-rw-   0        0        0     2734 2020-01-08 05:52:53.000000 GISPython-59.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 11:14:51.000000 GISPython-59.2/
+-rw-rw-rw-   0        0        0       61 2018-07-19 06:01:11.000000 GISPython-59.2/.gitignore
+-rw-rw-rw-   0        0        0      142 2018-07-19 06:01:11.000000 GISPython-59.2/.pypirc
+drwxrwxrwx   0        0        0        0 2023-06-02 11:14:50.000000 GISPython-59.2/GISPython/
+-rw-rw-rw-   0        0        0    14560 2022-01-23 15:44:36.000000 GISPython-59.2/GISPython/AGServerHelper.py
+-rw-rw-rw-   0        0        0    35075 2023-06-01 07:58:46.000000 GISPython-59.2/GISPython/AGServerHelperNTLM.py
+-rw-rw-rw-   0        0        0    23880 2022-01-23 15:44:36.000000 GISPython-59.2/GISPython/AGServerHelperToken.py
+-rw-rw-rw-   0        0        0     4254 2018-07-19 06:01:12.000000 GISPython-59.2/GISPython/CachingHelper.py
+-rw-rw-rw-   0        0        0     4731 2018-07-19 06:01:12.000000 GISPython-59.2/GISPython/FTPHleper.py
+-rw-rw-rw-   0        0        0    22306 2022-02-21 08:26:12.000000 GISPython-59.2/GISPython/GDBHelper.py
+-rw-rw-rw-   0        0        0     8354 2018-07-19 06:01:12.000000 GISPython-59.2/GISPython/GDPSyncroniserHelper.py
+-rw-rw-rw-   0        0        0    26395 2022-03-16 23:36:27.000000 GISPython-59.2/GISPython/GDPSyncroniserHelper2.py
+-rw-rw-rw-   0        0        0    12712 2022-04-21 07:54:14.000000 GISPython-59.2/GISPython/GISPythonModule.py
+-rw-rw-rw-   0        0        0     2251 2018-07-19 06:01:12.000000 GISPython-59.2/GISPython/GISPythonTool.py
+-rw-rw-rw-   0        0        0    19237 2022-11-06 11:41:17.000000 GISPython-59.2/GISPython/GISPythonToolBase.py
+-rw-rw-rw-   0        0        0     3368 2019-09-06 06:11:22.000000 GISPython-59.2/GISPython/JsonParamsHelper.py
+-rw-rw-rw-   0        0        0     4023 2023-03-23 06:54:39.000000 GISPython-59.2/GISPython/MailHelper.py
+-rw-rw-rw-   0        0        0     9520 2022-03-18 07:59:10.000000 GISPython-59.2/GISPython/MXDHelper.py
+-rw-rw-rw-   0        0        0      858 2018-07-19 06:01:12.000000 GISPython-59.2/GISPython/MyError.py
+drwxrwxrwx   0        0        0        0 2023-06-02 11:14:51.000000 GISPython-59.2/GISPython/PShell/
+-rw-rw-rw-   0        0        0      696 2018-07-19 06:01:12.000000 GISPython-59.2/GISPython/PShell/BackupOldFiles.ps1
+-rw-rw-rw-   0        0        0      410 2018-07-19 06:01:12.000000 GISPython-59.2/GISPython/PShell/ClearDir.ps1
+-rw-rw-rw-   0        0        0      661 2018-07-19 06:01:12.000000 GISPython-59.2/GISPython/PShell/GetLog.ps1
+-rw-rw-rw-   0        0        0    20804 2022-03-20 16:00:04.000000 GISPython-59.2/GISPython/PublisherHealper.py
+-rw-rw-rw-   0        0        0      658 2018-07-19 06:01:12.000000 GISPython-59.2/GISPython/RarHelper.py
+-rw-rw-rw-   0        0        0     2479 2022-07-15 16:06:08.000000 GISPython-59.2/GISPython/SFTPHelper.py
+-rw-rw-rw-   0        0        0    18601 2018-12-03 01:07:07.000000 GISPython-59.2/GISPython/SimpleFileOps.py
+-rw-rw-rw-   0        0        0     5836 2020-08-12 04:42:32.000000 GISPython-59.2/GISPython/SimpleFileOpsSafe.py
+-rw-rw-rw-   0        0        0    12757 2022-04-21 07:43:29.000000 GISPython-59.2/GISPython/SysGISTools.py
+-rw-rw-rw-   0        0        0      160 2023-06-02 11:09:38.000000 GISPython-59.2/GISPython/SysGISToolsSysParams.py
+-rw-rw-rw-   0        0        0     1701 2019-05-24 06:27:11.000000 GISPython-59.2/GISPython/SysTools_unittest.py
+-rw-rw-rw-   0        0        0     2371 2022-03-14 22:32:29.000000 GISPython-59.2/GISPython/TimerHelper.py
+-rw-rw-rw-   0        0        0     3311 2022-01-20 07:27:45.000000 GISPython-59.2/GISPython/xmlParamsHealper.py
+-rw-rw-rw-   0        0        0     3764 2022-01-20 07:27:45.000000 GISPython-59.2/GISPython/ZipHelper.py
+-rw-rw-rw-   0        0        0      906 2018-07-19 06:01:11.000000 GISPython-59.2/GISPython/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 11:14:51.000000 GISPython-59.2/GISPython.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-02 11:14:49.000000 GISPython-59.2/GISPython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1172 2023-06-02 11:14:49.000000 GISPython-59.2/GISPython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       79 2023-06-02 11:14:49.000000 GISPython-59.2/GISPython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     1087 2023-06-02 11:14:49.000000 GISPython-59.2/GISPython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       10 2023-06-02 11:14:49.000000 GISPython-59.2/GISPython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35793 2018-07-19 06:01:12.000000 GISPython-59.2/LICENSE
+-rw-rw-rw-   0        0        0      274 2018-07-19 06:01:12.000000 GISPython-59.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1172 2023-06-02 11:14:51.000000 GISPython-59.2/PKG-INFO
+-rwxrwxrwx   0        0        0      718 2018-08-15 04:52:21.000000 GISPython-59.2/pypi_upload.bat
+-rw-rw-rw-   0        0        0    17075 2019-05-24 06:27:11.000000 GISPython-59.2/README.md
+-rw-rw-rw-   0        0        0       63 2018-07-19 06:01:12.000000 GISPython-59.2/README.rst
+-rw-rw-rw-   0        0        0       42 2023-06-02 11:14:51.000000 GISPython-59.2/setup.cfg
+-rw-rw-rw-   0        0        0     2734 2020-01-08 05:52:53.000000 GISPython-59.2/setup.py
```

### Comparing `GISPython-59.1/GISPython/AGServerHelper.py` & `GISPython-59.2/GISPython/AGServerHelper.py`

 * *Files identical despite different names*

### Comparing `GISPython-59.1/GISPython/AGServerHelperNTLM.py` & `GISPython-59.2/GISPython/AGServerHelperNTLM.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,16 +208,17 @@
         data = self.__request_from_server(url, params)
 
         try:
             service_list = json.loads(data)
         except urllib2.URLError, exception:
             raise MyError.MyError(exception)
 
-        for single in service_list["services"]:
-            services.append(folder + single['serviceName'] + '.' + single['type'])
+        if "services" in service_list:
+            for single in service_list["services"]:
+                services.append(folder + single['serviceName'] + '.' + single['type'])
 
         folder_list = service_list["folders"] if u'folders' in service_list else []
         if u'Utilities' in service_list:
             folder_list.remove("Utilities")
         if u'System' in service_list:
             folder_list.remove("System")
```

### Comparing `GISPython-59.1/GISPython/AGServerHelperToken.py` & `GISPython-59.2/GISPython/AGServerHelperToken.py`

 * *Files identical despite different names*

### Comparing `GISPython-59.1/GISPython/CachingHelper.py` & `GISPython-59.2/GISPython/CachingHelper.py`

 * *Files identical despite different names*

### Comparing `GISPython-59.1/GISPython/FTPHleper.py` & `GISPython-59.2/GISPython/FTPHleper.py`

 * *Files identical despite different names*

### Comparing `GISPython-59.1/GISPython/GDBHelper.py` & `GISPython-59.2/GISPython/GDBHelper.py`

 * *Files identical despite different names*

### Comparing `GISPython-59.1/GISPython/GDPSyncroniserHelper.py` & `GISPython-59.2/GISPython/GDPSyncroniserHelper.py`

 * *Files identical despite different names*

### Comparing `GISPython-59.1/GISPython/GDPSyncroniserHelper2.py` & `GISPython-59.2/GISPython/GDPSyncroniserHelper2.py`

 * *Files identical despite different names*

### Comparing `GISPython-59.1/GISPython/GISPythonModule.py` & `GISPython-59.2/GISPython/GISPythonModule.py`

 * *Files identical despite different names*

### Comparing `GISPython-59.1/GISPython/GISPythonTool.py` & `GISPython-59.2/GISPython/GISPythonTool.py`

 * *Files identical despite different names*

### Comparing `GISPython-59.1/GISPython/GISPythonToolBase.py` & `GISPython-59.2/GISPython/GISPythonToolBase.py`

 * *Files identical despite different names*

### Comparing `GISPython-59.1/GISPython/JsonParamsHelper.py` & `GISPython-59.2/GISPython/JsonParamsHelper.py`

 * *Files identical despite different names*

### Comparing `GISPython-59.1/GISPython/MailHelper.py` & `GISPython-59.2/GISPython/MailHelper.py`

 * *Files identical despite different names*

### Comparing `GISPython-59.1/GISPython/MXDHelper.py` & `GISPython-59.2/GISPython/MXDHelper.py`

 * *Files identical despite different names*

### Comparing `GISPython-59.1/GISPython/MyError.py` & `GISPython-59.2/GISPython/MyError.py`

 * *Files identical despite different names*

### Comparing `GISPython-59.1/GISPython/PShell/BackupOldFiles.ps1` & `GISPython-59.2/GISPython/PShell/BackupOldFiles.ps1`

 * *Files identical despite different names*

### Comparing `GISPython-59.1/GISPython/PShell/GetLog.ps1` & `GISPython-59.2/GISPython/PShell/GetLog.ps1`

 * *Files identical despite different names*

### Comparing `GISPython-59.1/GISPython/PublisherHealper.py` & `GISPython-59.2/GISPython/PublisherHealper.py`

 * *Files identical despite different names*

### Comparing `GISPython-59.1/GISPython/RarHelper.py` & `GISPython-59.2/GISPython/RarHelper.py`

 * *Files identical despite different names*

### Comparing `GISPython-59.1/GISPython/SFTPHelper.py` & `GISPython-59.2/GISPython/SFTPHelper.py`

 * *Files identical despite different names*

### Comparing `GISPython-59.1/GISPython/SimpleFileOps.py` & `GISPython-59.2/GISPython/SimpleFileOps.py`

 * *Files identical despite different names*

### Comparing `GISPython-59.1/GISPython/SimpleFileOpsSafe.py` & `GISPython-59.2/GISPython/SimpleFileOpsSafe.py`

 * *Files identical despite different names*

### Comparing `GISPython-59.1/GISPython/SysGISTools.py` & `GISPython-59.2/GISPython/SysGISTools.py`

 * *Files identical despite different names*

### Comparing `GISPython-59.1/GISPython/SysTools_unittest.py` & `GISPython-59.2/GISPython/SysTools_unittest.py`

 * *Files identical despite different names*

### Comparing `GISPython-59.1/GISPython/TimerHelper.py` & `GISPython-59.2/GISPython/TimerHelper.py`

 * *Files identical despite different names*

### Comparing `GISPython-59.1/GISPython/xmlParamsHealper.py` & `GISPython-59.2/GISPython/xmlParamsHealper.py`

 * *Files identical despite different names*

### Comparing `GISPython-59.1/GISPython/ZipHelper.py` & `GISPython-59.2/GISPython/ZipHelper.py`

 * *Files identical despite different names*

### Comparing `GISPython-59.1/GISPython/__init__.py` & `GISPython-59.2/GISPython/__init__.py`

 * *Files identical despite different names*

### Comparing `GISPython-59.1/GISPython.egg-info/PKG-INFO` & `GISPython-59.2/GISPython.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: GISPython
-Version: 59.1
+Version: 59.2
 Summary: Additional tools for administering and automating different ArcPy and ArcGIS Server geoprocessing operations. Package is intended for use with ArcGIS 10.2.1 and later (has been tested on ArcGIS 10.3.1, ArcGIS 10.4, ArcGIS 10.5, ArcGIS 10.6.1)
 Home-page: https://github.com/lvmgeo/GISPython
 Author: LVM GEO
 Author-email: lvmGEOGit@lvm.lv
 License: GPLv3
 Description: For readme see GitHub https://github.com/lvmgeo/GISPython
 Keywords: ArcGIS,ArcPy,ArcGIS Server,automation
```

### Comparing `GISPython-59.1/GISPython.egg-info/SOURCES.txt` & `GISPython-59.2/GISPython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GISPython-59.1/LICENSE` & `GISPython-59.2/LICENSE`

 * *Files identical despite different names*

### Comparing `GISPython-59.1/PKG-INFO` & `GISPython-59.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: GISPython
-Version: 59.1
+Version: 59.2
 Summary: Additional tools for administering and automating different ArcPy and ArcGIS Server geoprocessing operations. Package is intended for use with ArcGIS 10.2.1 and later (has been tested on ArcGIS 10.3.1, ArcGIS 10.4, ArcGIS 10.5, ArcGIS 10.6.1)
 Home-page: https://github.com/lvmgeo/GISPython
 Author: LVM GEO
 Author-email: lvmGEOGit@lvm.lv
 License: GPLv3
 Description: For readme see GitHub https://github.com/lvmgeo/GISPython
 Keywords: ArcGIS,ArcPy,ArcGIS Server,automation
```

### Comparing `GISPython-59.1/pypi_upload.bat` & `GISPython-59.2/pypi_upload.bat`

 * *Files identical despite different names*

### Comparing `GISPython-59.1/README.md` & `GISPython-59.2/README.md`

 * *Files identical despite different names*

### Comparing `GISPython-59.1/setup.py` & `GISPython-59.2/setup.py`

 * *Files identical despite different names*

