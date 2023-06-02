# Comparing `tmp/nxsrecselector-3.27.0.tar.gz` & `tmp/nxsrecselector-3.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nxsrecselector-3.27.0.tar", last modified: Fri May 26 09:17:26 2023, max compression
+gzip compressed data, was "nxsrecselector-3.28.0.tar", last modified: Fri Jun  2 09:07:25 2023, max compression
```

## Comparing `nxsrecselector-3.27.0.tar` & `nxsrecselector-3.28.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-26 09:17:26.668372 nxsrecselector-3.27.0/
--rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2018-10-10 09:18:56.000000 nxsrecselector-3.27.0/COPYRIGHT
--rw-r--r--   0 jkotan   (15949) irc         (39)       93 2016-05-11 08:07:11.000000 nxsrecselector-3.27.0/MANIFEST.in
--rwxr-xr-x   0 jkotan   (15949) irc         (39)      941 2017-06-19 15:02:38.000000 nxsrecselector-3.27.0/NXSRecSelector
--rw-r--r--   0 jkotan   (15949) irc         (39)     7061 2023-05-26 09:17:26.668372 nxsrecselector-3.27.0/PKG-INFO
--rw-r--r--   0 jkotan   (15949) irc         (39)     4306 2023-02-01 13:37:17.000000 nxsrecselector-3.27.0/README.rst
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-26 09:17:26.664372 nxsrecselector-3.27.0/man/
--rw-r--r--   0 jkotan   (15949) irc         (39)      938 2017-03-18 22:59:30.000000 nxsrecselector-3.27.0/man/NXSRecSelector.1
--rw-r--r--   0 jkotan   (15949) irc         (39)   109341 2023-03-10 08:35:11.000000 nxsrecselector-3.27.0/man/nxsrecconfig.1
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-26 09:17:26.668372 nxsrecselector-3.27.0/nxsrecconfig/
--rw-r--r--   0 jkotan   (15949) irc         (39)     6486 2023-02-01 13:37:17.000000 nxsrecselector-3.27.0/nxsrecconfig/CheckerThread.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    10979 2020-01-31 13:48:24.000000 nxsrecselector-3.27.0/nxsrecconfig/Converter.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    23789 2023-02-01 13:37:17.000000 nxsrecselector-3.27.0/nxsrecconfig/Describer.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    22847 2023-02-01 13:37:17.000000 nxsrecselector-3.27.0/nxsrecconfig/DynamicComponent.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    19515 2023-02-01 13:37:17.000000 nxsrecselector-3.27.0/nxsrecconfig/MacroServerPools.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    74862 2023-05-26 09:16:32.000000 nxsrecselector-3.27.0/nxsrecconfig/NXSConfig.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    59225 2023-05-26 09:16:32.000000 nxsrecselector-3.27.0/nxsrecconfig/ProfileManager.py
--rw-r--r--   0 jkotan   (15949) irc         (39)      930 2023-05-26 09:16:32.000000 nxsrecselector-3.27.0/nxsrecconfig/Release.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     9075 2020-01-31 13:48:24.000000 nxsrecselector-3.27.0/nxsrecconfig/Selection.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    16157 2023-02-01 13:37:17.000000 nxsrecselector-3.27.0/nxsrecconfig/Selector.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    43477 2023-05-26 09:16:32.000000 nxsrecselector-3.27.0/nxsrecconfig/Settings.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5795 2023-03-09 16:17:52.000000 nxsrecselector-3.27.0/nxsrecconfig/StreamSet.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    29259 2023-05-26 09:16:32.000000 nxsrecselector-3.27.0/nxsrecconfig/Utils.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1683 2023-02-01 13:37:17.000000 nxsrecselector-3.27.0/nxsrecconfig/__init__.py
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-26 09:17:26.668372 nxsrecselector-3.27.0/nxsrecselector.egg-info/
--rw-r--r--   0 jkotan   (15949) irc         (39)     7061 2023-05-26 09:17:26.000000 nxsrecselector-3.27.0/nxsrecselector.egg-info/PKG-INFO
--rw-r--r--   0 jkotan   (15949) irc         (39)      710 2023-05-26 09:17:26.000000 nxsrecselector-3.27.0/nxsrecselector.egg-info/SOURCES.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)        1 2023-05-26 09:17:26.000000 nxsrecselector-3.27.0/nxsrecselector.egg-info/dependency_links.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)        1 2021-12-01 13:43:40.000000 nxsrecselector-3.27.0/nxsrecselector.egg-info/not-zip-safe
--rw-r--r--   0 jkotan   (15949) irc         (39)       17 2023-05-26 09:17:26.000000 nxsrecselector-3.27.0/nxsrecselector.egg-info/requires.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)       13 2023-05-26 09:17:26.000000 nxsrecselector-3.27.0/nxsrecselector.egg-info/top_level.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)      213 2023-05-26 09:17:26.668372 nxsrecselector-3.27.0/setup.cfg
--rw-r--r--   0 jkotan   (15949) irc         (39)     3985 2022-05-18 15:32:00.000000 nxsrecselector-3.27.0/setup.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-06-02 09:07:25.342510 nxsrecselector-3.28.0/
+-rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2018-10-10 09:18:56.000000 nxsrecselector-3.28.0/COPYRIGHT
+-rw-r--r--   0 jkotan   (15949) irc         (39)       93 2016-05-11 08:07:11.000000 nxsrecselector-3.28.0/MANIFEST.in
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)      941 2017-06-19 15:02:38.000000 nxsrecselector-3.28.0/NXSRecSelector
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7061 2023-06-02 09:07:25.342510 nxsrecselector-3.28.0/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4306 2023-02-01 13:37:17.000000 nxsrecselector-3.28.0/README.rst
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-06-02 09:07:25.338510 nxsrecselector-3.28.0/man/
+-rw-r--r--   0 jkotan   (15949) irc         (39)      938 2017-03-18 22:59:30.000000 nxsrecselector-3.28.0/man/NXSRecSelector.1
+-rw-r--r--   0 jkotan   (15949) irc         (39)   109341 2023-03-10 08:35:11.000000 nxsrecselector-3.28.0/man/nxsrecconfig.1
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-06-02 09:07:25.342510 nxsrecselector-3.28.0/nxsrecconfig/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6669 2023-06-02 09:06:46.000000 nxsrecselector-3.28.0/nxsrecconfig/CheckerThread.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    10979 2020-01-31 13:48:24.000000 nxsrecselector-3.28.0/nxsrecconfig/Converter.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    23789 2023-02-01 13:37:17.000000 nxsrecselector-3.28.0/nxsrecconfig/Describer.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    22847 2023-02-01 13:37:17.000000 nxsrecselector-3.28.0/nxsrecconfig/DynamicComponent.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    19957 2023-06-02 09:06:46.000000 nxsrecselector-3.28.0/nxsrecconfig/MacroServerPools.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    75512 2023-06-02 09:06:46.000000 nxsrecselector-3.28.0/nxsrecconfig/NXSConfig.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    59225 2023-05-26 09:16:32.000000 nxsrecselector-3.28.0/nxsrecconfig/ProfileManager.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      930 2023-06-01 15:59:20.000000 nxsrecselector-3.28.0/nxsrecconfig/Release.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     9075 2020-01-31 13:48:24.000000 nxsrecselector-3.28.0/nxsrecconfig/Selection.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    16157 2023-02-01 13:37:17.000000 nxsrecselector-3.28.0/nxsrecconfig/Selector.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    44983 2023-06-02 09:06:46.000000 nxsrecselector-3.28.0/nxsrecconfig/Settings.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5795 2023-03-09 16:17:52.000000 nxsrecselector-3.28.0/nxsrecconfig/StreamSet.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    29259 2023-05-26 09:16:32.000000 nxsrecselector-3.28.0/nxsrecconfig/Utils.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1683 2023-02-01 13:37:17.000000 nxsrecselector-3.28.0/nxsrecconfig/__init__.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-06-02 09:07:25.342510 nxsrecselector-3.28.0/nxsrecselector.egg-info/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7061 2023-06-02 09:07:25.000000 nxsrecselector-3.28.0/nxsrecselector.egg-info/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)      710 2023-06-02 09:07:25.000000 nxsrecselector-3.28.0/nxsrecselector.egg-info/SOURCES.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        1 2023-06-02 09:07:25.000000 nxsrecselector-3.28.0/nxsrecselector.egg-info/dependency_links.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        1 2021-12-01 13:43:40.000000 nxsrecselector-3.28.0/nxsrecselector.egg-info/not-zip-safe
+-rw-r--r--   0 jkotan   (15949) irc         (39)       17 2023-06-02 09:07:25.000000 nxsrecselector-3.28.0/nxsrecselector.egg-info/requires.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)       13 2023-06-02 09:07:25.000000 nxsrecselector-3.28.0/nxsrecselector.egg-info/top_level.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)      213 2023-06-02 09:07:25.342510 nxsrecselector-3.28.0/setup.cfg
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3985 2022-05-18 15:32:00.000000 nxsrecselector-3.28.0/setup.py
```

### Comparing `nxsrecselector-3.27.0/COPYRIGHT` & `nxsrecselector-3.28.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.27.0/NXSRecSelector` & `nxsrecselector-3.28.0/NXSRecSelector`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.27.0/PKG-INFO` & `nxsrecselector-3.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: nxsrecselector
-Version: 3.27.0
+Version: 3.28.0
 Summary: Selector Server for NeXus Sardana recorder
 Home-page: https://github.com/jkotan/nexdatas/
 Author: Jan Kotanski
 Author-email: jankotan@gmail.com
 License: GNU GENERAL PUBLIC LICENSE v3
 Description: ========================================
         Welcome to nxsrecconfig's documentation!
```

### Comparing `nxsrecselector-3.27.0/README.rst` & `nxsrecselector-3.28.0/README.rst`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.27.0/man/NXSRecSelector.1` & `nxsrecselector-3.28.0/man/NXSRecSelector.1`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.27.0/man/nxsrecconfig.1` & `nxsrecselector-3.28.0/man/nxsrecconfig.1`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.27.0/nxsrecconfig/CheckerThread.py` & `nxsrecselector-3.28.0/nxsrecconfig/CheckerThread.py`

 * *Files 6% similar despite different names*

```diff
@@ -102,58 +102,61 @@
         """
         threading.Thread.__init__(self)
         #: (:obj:`int`) thread index
         self.index = index
         #: (:class:`Queue.Queue`) queue with runnable elements
         self.__queue = queue
 
+        #: (:obj:`list` <:obj:`str`>) tango datasources error states
+        self.tangoSourceErrorStates = [
+            "OFF", "INIT", "INSERT", "CLOSE", "UNKNOWN", "FAULT", "DISABLE"]
+
+        #: (:obj:`list` <:obj:`str`>) tango datasources warning states
+        self.tangoSourceWarningStates = ["ALARM"]
+
     def run(self):
         """ runner
 
         :brief: It runs the defined thread
         """
         full = True
         while full:
             try:
                 elem = self.__queue.get(block=False)
                 self.__check(elem)
 
             except Queue.Empty:
                 full = False
 
-    @classmethod
-    def __check(cls, checkeritem):
+    def __check(self, checkeritem):
         """ checks oen device list item which usually corresponds
         to one components
 
         :param checkeritem: device list item
         :type checkeritem: :obj:`list` <:class:`CheckerItem`>
         """
+        # print("E", self.tangoSourceErrorStates)
+        # print("W", self.tangoSourceWarningStates)
         for ds in checkeritem:
             try:
                 if ds.attr:
                     dvat = "%s/%s" % (ds.device or ds.name, ds.attr)
                 else:
                     dvat = "%s" % (ds.device or ds.name)
                 dp = tango.DeviceProxy(ds.device or ds.name)
                 # read real value (not polled)
                 dp.set_source(tango.DevSource.DEV)
                 # wait when DeviceProxy is ready
                 TangoUtils.wait(dp, state=None)
                 dp.set_timeout_millis(10000)
                 state = dp.state()
-                if state in [tango.DevState.FAULT,
-                             tango.DevState.DISABLE]:
+                if str(state) in self.tangoSourceErrorStates:
                     raise FaultStateError("%s STATE" % state)
-                if state in [tango.DevState.OFF,
-                             tango.DevState.INIT,
-                             tango.DevState.INSERT,
-                             tango.DevState.CLOSE,
-                             tango.DevState.UNKNOWN]:
-                    raise OffStateError("%s STATE" % state)
+                # if str(state) in self.tangoSourceOffStates:
+                #     raise OffStateError("%s STATE" % state)
                 dp.ping()
                 if not ds.attr:
                     for gattr in ATTRIBUTESTOCHECK:
                         if hasattr(dp, gattr):
                             at = getattr(dp, gattr)
                             if at is None:
                                 raise Exception("Empty Attribute")
@@ -163,18 +166,18 @@
                     at = getattr(dp, ds.attr[:-2])
                     if at is None:
                         raise Exception("Empty Attribute")
                 else:
                     v = dp.read_attributes([ds.attr])
                     if v[0].has_failed or v[0].value is None:
                         raise Exception("Empty Attribute")
-                if state in [tango.DevState.ALARM]:
-                    raise AlarmStateError("ALARM STATE")
-            except AlarmStateError:
-                checkeritem.message = "ALARM_STATE"
+                if str(state) in self.tangoSourceWarningStates:
+                    raise AlarmStateError("%s STATE" % state)
+            except AlarmStateError as e:
+                checkeritem.message = Utils.tostr(e)
                 if ds.name != dvat:
                     checkeritem.errords = "%s [%s]" % (ds.name, dvat)
                 else:
                     checkeritem.errords = ds.name
             except Exception as e:
                 checkeritem.message = Utils.tostr(e)
                 if ds.name != dvat:
```

### Comparing `nxsrecselector-3.27.0/nxsrecconfig/Converter.py` & `nxsrecselector-3.28.0/nxsrecconfig/Converter.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.27.0/nxsrecconfig/Describer.py` & `nxsrecselector-3.28.0/nxsrecconfig/Describer.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.27.0/nxsrecconfig/DynamicComponent.py` & `nxsrecselector-3.28.0/nxsrecconfig/DynamicComponent.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.27.0/nxsrecconfig/MacroServerPools.py` & `nxsrecselector-3.28.0/nxsrecconfig/MacroServerPools.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,16 +42,14 @@
     unicode = str
 
 
 class MacroServerPools(object):
 
     """ sardanamacro server and pools """
 
-    #
-
     def __init__(self, numberOfThreads):
         """ constructor
 
         :param numberOfThreads: number of threads
         :type numberOfThreads: :obj:`str`
         """
         self.__numberOfThreads = numberOfThreads
@@ -80,14 +78,21 @@
             "ConfigDevice",
             "WriterDevice",
             "Door",
             "MntGrp",
             "ScanDir"
         ]
 
+        #: (:obj:`list` <:obj:`str`>) tango datasources off states
+        self.tangoSourceErrorStates = [
+            "OFF", "INIT", "INSERT", "CLOSE", "UNKNOWN", "FAULT", "DISABLE"]
+
+        #: (:obj:`list` <:obj:`str`>) tango datasources warning states
+        self.tangoSourceWarningStates = ["ALARM"]
+
     def updateMacroServer(self, door):
         """ updates MacroServer and sardana pools for given door
 
         :param door: door device name
         :type door: :obj:`str`
         """
         self.__macroserver = ""
@@ -292,14 +297,16 @@
         for checkeritem in toCheck:
             cqueue.put(checkeritem)
         if self.__numberOfThreads < 1:
             self.__numberOfThreads = len(toCheck)
 
         for i in range(min(self.__numberOfThreads, len(toCheck))):
             thd = CheckerThread(i, cqueue)
+            thd.tangoSourceErrorStates = self.tangoSourceErrorStates
+            thd.tangoSourceWarningStates = self.tangoSourceWarningStates
             threads.append(thd)
             thd.start()
 
         for th in threads:
             th.join()
 
         for checkeritem in toCheck:
```

### Comparing `nxsrecselector-3.27.0/nxsrecconfig/NXSConfig.py` & `nxsrecselector-3.28.0/nxsrecconfig/NXSConfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,20 @@
             or ["*tip551*"]
         self.__stg.mutedPreScanAttrFilters = self.MutedPreScanAttrFilters or []
         self.__stg.adminDataNames = self.AdminDataNames or []
         self.__stg.defaultPreselectedComponents = \
             self.DefaultPreselectedComponents or []
         self.__stg.defaultCanFailDataSources = \
             self.DefaultCanFailDataSources or []
+        self.__stg.tangoSourceErrorStates = \
+            self.TangoSourceErrorStates or []
+        self.__stg.tangoSourceWarningStates = \
+            self.TangoSourceWarningStates or []
+        # print(self.TangoSourceErrorStates)
+        # print(self.TangoSourceWarningStates)
         self.__stg.clientRecordKeys = \
             self.ClientRecordKeys or []
 
     def always_executed_hook(self):
         """ Always excuted hook method
         """
         self.debug_stream("In always_excuted_hook()")
@@ -1885,14 +1891,23 @@
         [tango.DevBoolean,
          "the master timer channel of MG with the index: 0",
          [False]],
         'DefaultCanFailDataSources':
         [tango.DevVarStringArray,
          "list of default datasources in the CanFail mode",
          []],
+        'TangoSourceErrorStates':
+        [tango.DevVarStringArray,
+         "list of tango error states for tango datasources",
+         ["OFF", "INIT", "INSERT", "CLOSE", "UNKNOWN",
+          "FAULT", "DISABLE"]],
+        'TangoSourceWarningStates':
+        [tango.DevVarStringArray,
+         "list of tango warning states for tango datasources",
+         ["ALARM"]],
     }
 
     #: (:obj:`dict` <:obj:`str`, \
     #:       [[ :class:`tango.CmdArgType`, :obj:`str`]] >)
     #:       Command definitions
     cmd_list = {
         'SetScanEnvVariables':
```

### Comparing `nxsrecselector-3.27.0/nxsrecconfig/ProfileManager.py` & `nxsrecselector-3.28.0/nxsrecconfig/ProfileManager.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.27.0/nxsrecconfig/Release.py` & `nxsrecselector-3.28.0/nxsrecconfig/Release.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 #    You should have received a copy of the GNU General Public License
 #    along with nexdatas.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 """  NeXus Sardana Recorder Settings - Release """
 
 #: (:obj:`str`) package version
-__version__ = "3.27.0"
+__version__ = "3.28.0"
```

### Comparing `nxsrecselector-3.27.0/nxsrecconfig/Selection.py` & `nxsrecselector-3.28.0/nxsrecconfig/Selection.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.27.0/nxsrecconfig/Selector.py` & `nxsrecselector-3.28.0/nxsrecconfig/Selector.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.27.0/nxsrecconfig/Settings.py` & `nxsrecselector-3.28.0/nxsrecconfig/Settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         self._streams = StreamSet(weakref.ref(server) if server else None)
 
         #: (:obj:`str`) default NeXus path
         self.defaultNeXusPath = defaultnexuspath or \
             "/$var.entryname#'scan'$var.serialno:NXentry/" \
             "NXinstrument/collection"
 
-        #: (:obj:`str`) default CanFail DataSources
+        #: (:obj:`list` <:obj:`str`>) default CanFail DataSources
         self.defaultCanFailDataSources = []
 
         #: (:obj:`str`) default time zone
         self.defaultTimeZone = defaulttimezone or "Europe/Berlin"
 
         #: (:obj:`str`) default measurement group
         self.defaultMntGrp = defaultmntgrp or "nxsmntgrp"
@@ -314,14 +314,58 @@
 
     #: (:obj:`list` <:obj:`str`>) default PreselectedComponents
     defaultPreselectedComponents = property(
         __getDefaultPreselectedComponents,
         __setDefaultPreselectedComponents,
         doc='default Preselected components')
 
+    def __getTangoSourceErrorStates(self):
+        """ get method for tangoSourceErrorStates attribute
+
+        :returns: list of state
+        :rtype: :obj:`list` <:obj:`str`>
+        """
+        return self.__msp.tangoSourceErrorStates
+
+    def __setTangoSourceErrorStates(self, states):
+        """ set method for tangoSourceErrorStates attribute
+
+        :param states: list of states
+        :type states: :obj:`list` <:obj:`str`>
+        """
+        self.__msp.tangoSourceErrorStates = [st for st in states if st]
+
+    #: (:obj:`list` <:obj:`str`>) tango source fault state
+    tangoSourceErrorStates = property(
+        __getTangoSourceErrorStates,
+        __setTangoSourceErrorStates,
+        doc='tango sources error states')
+
+    def __getTangoSourceWarningStates(self):
+        """ get method for tangoSourceWarningStates attribute
+
+        :returns: list of state
+        :rtype: :obj:`list` <:obj:`str`>
+        """
+        return self.__msp.tangoSourceWarningStates
+
+    def __setTangoSourceWarningStates(self, states):
+        """ set method for tangoSourceWarningStates attribute
+
+        :param states: list of states
+        :type states: :obj:`list` <:obj:`str`>
+        """
+        self.__msp.tangoSourceWarningStates = [st for st in states if st]
+
+    #: (:obj:`list` <:obj:`str`>) tango source alarm state
+    tangoSourceWarningStates = property(
+        __getTangoSourceWarningStates,
+        __setTangoSourceWarningStates,
+        doc='tango sources warning states')
+
     def __getClientRecordKeys(self):
         """ get method for clientRecordKeys attribute
 
         :returns: list of components
         :rtype: :obj:`list` <:obj:`str`>
         """
         return self.__profileManager.clientRecordKeys
```

### Comparing `nxsrecselector-3.27.0/nxsrecconfig/StreamSet.py` & `nxsrecselector-3.28.0/nxsrecconfig/StreamSet.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.27.0/nxsrecconfig/Utils.py` & `nxsrecselector-3.28.0/nxsrecconfig/Utils.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.27.0/nxsrecconfig/__init__.py` & `nxsrecselector-3.28.0/nxsrecconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.27.0/nxsrecselector.egg-info/PKG-INFO` & `nxsrecselector-3.28.0/nxsrecselector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: nxsrecselector
-Version: 3.27.0
+Version: 3.28.0
 Summary: Selector Server for NeXus Sardana recorder
 Home-page: https://github.com/jkotan/nexdatas/
 Author: Jan Kotanski
 Author-email: jankotan@gmail.com
 License: GNU GENERAL PUBLIC LICENSE v3
 Description: ========================================
         Welcome to nxsrecconfig's documentation!
```

### Comparing `nxsrecselector-3.27.0/nxsrecselector.egg-info/SOURCES.txt` & `nxsrecselector-3.28.0/nxsrecselector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.27.0/setup.py` & `nxsrecselector-3.28.0/setup.py`

 * *Files identical despite different names*

