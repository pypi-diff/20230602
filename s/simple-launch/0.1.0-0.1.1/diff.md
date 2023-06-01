# Comparing `tmp/simple_launch-0.1.0-py3-none-any.whl.zip` & `tmp/simple_launch-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 13905 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat    27930 b- defN 23-May-31 22:37 simple_launch.py
--rw-rw-rw-  2.0 fat    11554 b- defN 23-Jun-01 00:56 simple_launch-0.1.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     4367 b- defN 23-Jun-01 00:56 simple_launch-0.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-01 00:56 simple_launch-0.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       53 b- defN 23-Jun-01 00:56 simple_launch-0.1.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       14 b- defN 23-Jun-01 00:56 simple_launch-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      596 b- defN 23-Jun-01 00:56 simple_launch-0.1.0.dist-info/RECORD
-7 files, 44606 bytes uncompressed, 12841 bytes compressed:  71.2%
+Zip file size: 14093 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat    28851 b- defN 23-Jun-01 21:50 simple_launch.py
+-rw-rw-rw-  2.0 fat    11554 b- defN 23-Jun-01 21:57 simple_launch-0.1.1.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     4405 b- defN 23-Jun-01 21:57 simple_launch-0.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-01 21:57 simple_launch-0.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       53 b- defN 23-Jun-01 21:57 simple_launch-0.1.1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       14 b- defN 23-Jun-01 21:57 simple_launch-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      596 b- defN 23-Jun-01 21:57 simple_launch-0.1.1.dist-info/RECORD
+7 files, 45565 bytes uncompressed, 13029 bytes compressed:  71.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: simple_launch.py
 Comment: 
 
-Filename: simple_launch-0.1.0.dist-info/LICENSE.txt
+Filename: simple_launch-0.1.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: simple_launch-0.1.0.dist-info/METADATA
+Filename: simple_launch-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: simple_launch-0.1.0.dist-info/WHEEL
+Filename: simple_launch-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: simple_launch-0.1.0.dist-info/entry_points.txt
+Filename: simple_launch-0.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: simple_launch-0.1.0.dist-info/top_level.txt
+Filename: simple_launch-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: simple_launch-0.1.0.dist-info/RECORD
+Filename: simple_launch-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## simple_launch.py

```diff
@@ -278,15 +278,15 @@
 
         return SimpleSubprocessImpl(process,job_handle)
 
     else:
         #TODO: Use "start_new_session=True" arg for new process
         process = await asyncio.create_subprocess_exec(process,*args, \
             stdout=asyncio.subprocess.PIPE,stderr=asyncio.subprocess.PIPE,\
-            env=env, cwd=cwd, close_fds=True, preexec_fn=os.setsid )
+            env=env, cwd=cwd, close_fds=True, start_new_session=True )
         return SimpleSubprocessImpl(process)
 
 
 class SimpleSubprocessImpl:
     def __init__(self, asyncio_subprocess, job_handle = None):
         self._process = asyncio_subprocess
         self._job_handle = job_handle
@@ -471,54 +471,78 @@
             res = ctypes.windll.kernel32.QueryInformationJobObject(job, subprocess_impl_win32.JobObjectBasicProcessIdList, ctypes.pointer(win32_thread_info), ctypes.sizeof(win32_thread_info), None)
             if not res:
                 return
             pids = []
             for i in range(win32_thread_info.NumberOfProcessIdsInList):
                 pids.append(win32_thread_info.ProcessIdList[i])
 
-            for p in pids:
-                subprocess_impl_win32.win32_send_pid_wm_close(p)
+            subprocess_impl_win32.win32_send_pid_wm_close(pids)
 
         def win32_send_pid_wm_close(pid):        
-            subprocess_impl_win32._win32_send_pid_wm_close_hwnd_message(pid)
-            subprocess_impl_win32._win32_send_pid_wm_close_hwnd_main(pid)
+            subprocess_impl_win32._win32_send_wm_close_hwnd_message(pid)
             subprocess_impl_win32._win32_send_ctrl_c_event(pid)
 
-        def _win32_send_pid_wm_close_hwnd_message(pid):
+        
+        def _win32_find_message_hwnds(pids):
+            if not isinstance(pids, list):
+                pids = [pids]
             hWnd_child_after = 0
+            hwnds = []
 
             while True:
                 hWnd = ctypes.windll.user32.FindWindowExW(subprocess_impl_win32.HWND_MESSAGE, hWnd_child_after, None, None)
                 # print(hWnd)    
                 if hWnd == 0:
                     break
                 process_id = ctypes.wintypes.DWORD()
                 ctypes.windll.user32.GetWindowThreadProcessId(hWnd,ctypes.byref(process_id))
-                if pid == process_id.value:
-                    ctypes.windll.user32.PostMessageW(hWnd,subprocess_impl_win32.WM_CLOSE,0,0)
+                if process_id.value in pids:
+                    hwnds.append(hWnd)
+                    #ctypes.windll.user32.PostMessageW(hWnd,subprocess_impl_win32.WM_CLOSE,0,0)
                 hWnd_child_after = hWnd
+            return hwnds
+        
+        def _win32_find_main_hwnds(pids):
+            if not isinstance(pids, list):
+                pids = [pids]
 
-        def _win32_send_pid_wm_close_hwnd_main(pid):
-            
+            hwnds = []
 
+            # Create list of top level windows
+            
             def worker(hWnd, lParam):
                 process_id = ctypes.wintypes.DWORD()
                 ctypes.windll.user32.GetWindowThreadProcessId(hWnd,ctypes.byref(process_id))
                 if lParam == process_id.value:
-                    ctypes.windll.user32.PostMessageW(hWnd,subprocess_impl_win32.WM_CLOSE,0,0)
+                    hwnds.append(hWnd)
                 return True
-
+            
             cb_worker = subprocess_impl_win32.WNDENUMPROC(worker)
-            if not ctypes.windll.user32.EnumWindows(cb_worker, pid):
-                return
+            if not ctypes.windll.user32.EnumWindows(cb_worker, pids[0]):
+                return hwnds
+            
+            # Filter out windows that are children of other windows
+            hwnds = [hWnd for hWnd in hwnds if not ctypes.windll.user32.GetParent(hWnd)]
+            return hwnds
+        
+        def _win32_send_wm_close_hwnd_message(pid):
+            # check for main window first, then send to message windows
+            hwnds = subprocess_impl_win32._win32_find_main_hwnds(pid)
+            print(f"main hwnds: {hwnds}")
+            if not hwnds:
+                hwnds = subprocess_impl_win32._win32_find_message_hwnds(pid)
+            for hWnd in hwnds:
+                ctypes.windll.user32.PostMessageW(hWnd,subprocess_impl_win32.WM_CLOSE,0,0)
 
         def _win32_send_ctrl_c_event(pid):
-            ctypes.windll.kernel32.GenerateConsoleCtrlEvent(1,pid)
-
-    _CtrlCHandlerRoutine = ctypes.WINFUNCTYPE(ctypes.wintypes.BOOL, ctypes.wintypes.DWORD)
+            if isinstance(pid, list):
+                for p in pid:
+                    subprocess_impl_win32._win32_send_ctrl_c_event(p)
+                return
+            ctypes.windll.kernel32.GenerateConsoleCtrlEvent(0,pid)
 
 def parse_task_launch_from_yaml(yaml_dict, cwd):
     # parse yaml_dict into SimpleTask tuple
     name = yaml_dict["name"]
     program = yaml_dict["program"]
     cwd = yaml_dict.get("cwd", cwd)
     args = yaml_dict.get("args", None)
```

## Comparing `simple_launch-0.1.0.dist-info/LICENSE.txt` & `simple_launch-0.1.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `simple_launch-0.1.0.dist-info/METADATA` & `simple_launch-0.1.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: simple-launch
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple launcher for Robotics applications
 Author-email: John Wason <wason@wasontech.com>
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyyaml
 Requires-Dist: appdirs
+Requires-Dist: simple-launch-process
 Provides-Extra: test
 Requires-Dist: pytest ; extra == 'test'
 Requires-Dist: pywin32 ; (platform_system == "Windows") and extra == 'test'
 
 # Simple Launch
 
 **WARNING: THIS IS UNFINISHED SOFTWARE**
```

## Comparing `simple_launch-0.1.0.dist-info/RECORD` & `simple_launch-0.1.1.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-simple_launch.py,sha256=5dPhD6xnfBQqmkj0KA-Tq6kPniPA5UJzctvStYaqzmc,27930
-simple_launch-0.1.0.dist-info/LICENSE.txt,sha256=Tl1tRxWGtrUEp-8aQr9k8kNBVeVc0FnOcSY8m7eKPfc,11554
-simple_launch-0.1.0.dist-info/METADATA,sha256=HyTo948oC9X11xZNnOUhc2ZGO3DKJq1rgb5hKngMZgg,4367
-simple_launch-0.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-simple_launch-0.1.0.dist-info/entry_points.txt,sha256=JChfbuwosdveFeg7BjKxTRbFaVjtpv1AciY-cPMbKTM,53
-simple_launch-0.1.0.dist-info/top_level.txt,sha256=vtmpRZhVMrLBO5is2vEsoZYfglFbpitYPqdpKbOuLng,14
-simple_launch-0.1.0.dist-info/RECORD,,
+simple_launch.py,sha256=UaSb0i9h4CYWdZkxTf4Oyum4MJ3h8ho0Rk0NFOCouF8,28851
+simple_launch-0.1.1.dist-info/LICENSE.txt,sha256=Tl1tRxWGtrUEp-8aQr9k8kNBVeVc0FnOcSY8m7eKPfc,11554
+simple_launch-0.1.1.dist-info/METADATA,sha256=NUuO8PK_w5xCyBhdG180fO3ATkj0wZfU4xgolZ-1bso,4405
+simple_launch-0.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+simple_launch-0.1.1.dist-info/entry_points.txt,sha256=JChfbuwosdveFeg7BjKxTRbFaVjtpv1AciY-cPMbKTM,53
+simple_launch-0.1.1.dist-info/top_level.txt,sha256=vtmpRZhVMrLBO5is2vEsoZYfglFbpitYPqdpKbOuLng,14
+simple_launch-0.1.1.dist-info/RECORD,,
```

