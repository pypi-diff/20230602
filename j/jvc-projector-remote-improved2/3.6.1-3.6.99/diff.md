# Comparing `tmp/jvc_projector_remote_improved2-3.6.1.tar.gz` & `tmp/jvc_projector_remote_improved2-3.6.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jvc_projector_remote_improved2-3.6.1.tar", last modified: Sun May 14 15:00:05 2023, max compression
+gzip compressed data, was "jvc_projector_remote_improved2-3.6.99.tar", last modified: Fri Jun  2 00:46:05 2023, max compression
```

## Comparing `jvc_projector_remote_improved2-3.6.1.tar` & `jvc_projector_remote_improved2-3.6.99.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:00:05.414622 jvc_projector_remote_improved2-3.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-14 14:59:54.000000 jvc_projector_remote_improved2-3.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-05-14 15:00:05.414622 jvc_projector_remote_improved2-3.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-05-14 14:59:54.000000 jvc_projector_remote_improved2-3.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:00:05.414622 jvc_projector_remote_improved2-3.6.1/jvc_projector/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-14 14:59:54.000000 jvc_projector_remote_improved2-3.6.1/jvc_projector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-05-14 14:59:54.000000 jvc_projector_remote_improved2-3.6.1/jvc_projector/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    22639 2023-05-14 14:59:54.000000 jvc_projector_remote_improved2-3.6.1/jvc_projector/jvc_projector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:00:05.414622 jvc_projector_remote_improved2-3.6.1/jvc_projector_remote_improved2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-05-14 15:00:05.000000 jvc_projector_remote_improved2-3.6.1/jvc_projector_remote_improved2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-14 15:00:05.000000 jvc_projector_remote_improved2-3.6.1/jvc_projector_remote_improved2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 15:00:05.000000 jvc_projector_remote_improved2-3.6.1/jvc_projector_remote_improved2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-14 15:00:05.000000 jvc_projector_remote_improved2-3.6.1/jvc_projector_remote_improved2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 15:00:05.418622 jvc_projector_remote_improved2-3.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-14 14:59:54.000000 jvc_projector_remote_improved2-3.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:00:05.414622 jvc_projector_remote_improved2-3.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:59:54.000000 jvc_projector_remote_improved2-3.6.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-14 14:59:54.000000 jvc_projector_remote_improved2-3.6.1/tests/testLowLatency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:46:05.123386 jvc_projector_remote_improved2-3.6.99/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-02 00:45:53.000000 jvc_projector_remote_improved2-3.6.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-06-02 00:46:05.123386 jvc_projector_remote_improved2-3.6.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-02 00:45:53.000000 jvc_projector_remote_improved2-3.6.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:46:05.123386 jvc_projector_remote_improved2-3.6.99/jvc_projector/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-02 00:45:53.000000 jvc_projector_remote_improved2-3.6.99/jvc_projector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-06-02 00:45:53.000000 jvc_projector_remote_improved2-3.6.99/jvc_projector/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23096 2023-06-02 00:45:53.000000 jvc_projector_remote_improved2-3.6.99/jvc_projector/jvc_projector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:46:05.123386 jvc_projector_remote_improved2-3.6.99/jvc_projector_remote_improved2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-06-02 00:46:05.000000 jvc_projector_remote_improved2-3.6.99/jvc_projector_remote_improved2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-02 00:46:05.000000 jvc_projector_remote_improved2-3.6.99/jvc_projector_remote_improved2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 00:46:05.000000 jvc_projector_remote_improved2-3.6.99/jvc_projector_remote_improved2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-02 00:46:05.000000 jvc_projector_remote_improved2-3.6.99/jvc_projector_remote_improved2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 00:46:05.123386 jvc_projector_remote_improved2-3.6.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-02 00:45:53.000000 jvc_projector_remote_improved2-3.6.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:46:05.123386 jvc_projector_remote_improved2-3.6.99/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 00:45:53.000000 jvc_projector_remote_improved2-3.6.99/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-02 00:45:53.000000 jvc_projector_remote_improved2-3.6.99/tests/testLowLatency.py
```

### Comparing `jvc_projector_remote_improved2-3.6.1/LICENSE` & `jvc_projector_remote_improved2-3.6.99/LICENSE`

 * *Files identical despite different names*

### Comparing `jvc_projector_remote_improved2-3.6.1/PKG-INFO` & `jvc_projector_remote_improved2-3.6.99/jvc_projector_remote_improved2.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: jvc_projector_remote_improved2
-Version: 3.6.1
+Name: jvc-projector-remote-improved2
+Version: 3.6.99
 Summary: A package to control JVC projectors over IP
 Home-page: https://github.com/iloveicedgreentea/jvc_projector_improved
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -128,14 +128,18 @@
 ## Supported Commands
 
 `$command,$parameter`
 example: "anamorphic,off"
 example: "anamorphic,d"
 example: "laser_dim,auto3"
 
+It also supports using remote codes as ASCII [found here](https://support.jvc.com/consumer/support/documents/DILAremoteControlGuide.pdf) (Code A only)
+
+`jvc.emulate_remote("23")`
+
 ```
 Currently Supported Commands:
         anamorphic
         aperture
         enhance
         eshift
         graphic_mode
```

### Comparing `jvc_projector_remote_improved2-3.6.1/README.md` & `jvc_projector_remote_improved2-3.6.99/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -116,14 +116,18 @@
 ## Supported Commands
 
 `$command,$parameter`
 example: "anamorphic,off"
 example: "anamorphic,d"
 example: "laser_dim,auto3"
 
+It also supports using remote codes as ASCII [found here](https://support.jvc.com/consumer/support/documents/DILAremoteControlGuide.pdf) (Code A only)
+
+`jvc.emulate_remote("23")`
+
 ```
 Currently Supported Commands:
         anamorphic
         aperture
         enhance
         eshift
         graphic_mode
```

### Comparing `jvc_projector_remote_improved2-3.6.1/jvc_projector/commands.py` & `jvc_projector_remote_improved2-3.6.99/jvc_projector/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,14 +290,15 @@
     input_mode = b"IP", InputModes, ACKs.input_ack
 
     # status commands - Reference: ?
     # These should not be used directly
     power_status = b"PW"
     current_output = b"IP"
     info = b"RC7374"
+    remote = b"RC73"
 
     # Checking for model code
     # response -> \x40\x89\x01\x4D\x44(the model code)\x0A
     get_model = b"MD"
 
     # software version
     get_software_version = b"IFSV", str, ACKs.info_ack
```

### Comparing `jvc_projector_remote_improved2-3.6.1/jvc_projector/jvc_projector.py` & `jvc_projector_remote_improved2-3.6.99/jvc_projector/jvc_projector.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,15 +199,15 @@
         """
         Only useful for testing
         """
         self.client.close()
 
     def _send_command(
         self,
-        send_command: Union[list[bytes], bytes],
+        send_command: Union[list[str], str],
         command_type: bytes = b"!",
         ack: bytes = None,
     ) -> tuple[str, bool]:
         """
         Sends a command with a flag to expect an ack.
 
         The PJ API returns nothing if a command is in flight
@@ -224,44 +224,38 @@
             )
         """
         # Check commands
         self.logger.debug("Command_type: %s", command_type)
         self.logger.debug("Send command: %s", send_command)
         self.logger.debug("Send ack: %s", ack)
         if command_type == Header.reference.value:
-            result, success = self._do_command(send_command, ack, command_type)
-
-            return result, success
+            return self._do_command(send_command, ack, command_type)
 
         if isinstance(send_command, list):
+            # check emulate remote first
+            if send_command[0] == "remote":
+                return self.emulate_remote(send_command[1])
             for cmd in send_command:
                 cons_command, ack = self._construct_command(cmd, command_type)
                 if not ack:
                     return cons_command, ack
                 # need a delay otherwise it kills connection
                 time.sleep(0.1)
-                result, success = self._do_command(
-                    cons_command, ack.value, command_type
-                )
-                if not success:
-                    return result, success
+                return self._do_command(cons_command, ack.value, command_type)
+
+        # legacy since HA seems to always use a list
         else:
             try:
                 cons_command, ack = self._construct_command(send_command, command_type)
             except TypeError:
                 cons_command = send_command
 
             if not ack:
                 return cons_command, ack
-            result, success = self._do_command(cons_command, ack.value, command_type)
-            if not success:
-                return result, success
-
-        self.logger.debug("send command result: %s", result)
-        return "ok", True
+            return self._do_command(cons_command, ack.value, command_type)
 
     def _do_command(
         self,
         command: bytes,
         ack: bytes,
         command_type: bytes = b"!",
     ) -> tuple[Union[str, bytes], bool]:
@@ -428,14 +422,33 @@
 
         return self._send_command(
             cmd,
             ack=ACKs.menu_ack,
             command_type=Header.operation.value,
         )
 
+    def emulate_remote(self, remote_code: str) -> tuple[str, bool]:
+        """
+        Send a cmd via remote emulation
+
+        remote_code: str- ASCII of the remote code like 23 or D4 https://support.jvc.com/consumer/support/documents/DILAremoteControlGuide.pdf
+        """
+        cmd = (
+            Header.operation.value
+            + Header.pj_unit.value
+            + Commands.remote.value
+            + Footer.close.value
+        )
+
+        return self._send_command(
+            cmd + remote_code,
+            ack=ACKs.menu_ack,
+            command_type=Header.operation.value,
+        )
+
     def power_on(
         self,
     ) -> tuple[str, bool]:
         """
         Turns on PJ
         """
         return self.exec_command("power,on")
```

### Comparing `jvc_projector_remote_improved2-3.6.1/jvc_projector_remote_improved2.egg-info/PKG-INFO` & `jvc_projector_remote_improved2-3.6.99/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: jvc-projector-remote-improved2
-Version: 3.6.1
+Name: jvc_projector_remote_improved2
+Version: 3.6.99
 Summary: A package to control JVC projectors over IP
 Home-page: https://github.com/iloveicedgreentea/jvc_projector_improved
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -128,14 +128,18 @@
 ## Supported Commands
 
 `$command,$parameter`
 example: "anamorphic,off"
 example: "anamorphic,d"
 example: "laser_dim,auto3"
 
+It also supports using remote codes as ASCII [found here](https://support.jvc.com/consumer/support/documents/DILAremoteControlGuide.pdf) (Code A only)
+
+`jvc.emulate_remote("23")`
+
 ```
 Currently Supported Commands:
         anamorphic
         aperture
         enhance
         eshift
         graphic_mode
```

### Comparing `jvc_projector_remote_improved2-3.6.1/setup.py` & `jvc_projector_remote_improved2-3.6.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="jvc_projector_remote_improved2",
-    version="3.6.1",
+    version="3.6.99",
     author="iloveicedgreentea",
     description="A package to control JVC projectors over IP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iloveicedgreentea/jvc_projector_improved",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `jvc_projector_remote_improved2-3.6.1/tests/testLowLatency.py` & `jvc_projector_remote_improved2-3.6.99/tests/testLowLatency.py`

 * *Files identical despite different names*

