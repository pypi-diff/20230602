# Comparing `tmp/cc.xboxcontroller-0.0.4.tar.gz` & `tmp/cc.xboxcontroller-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cc.xboxcontroller-0.0.4.tar", last modified: Sat Feb 18 18:13:55 2023, max compression
+gzip compressed data, was "cc.xboxcontroller-0.1.0.tar", last modified: Thu Jun  1 22:27:53 2023, max compression
```

## Comparing `cc.xboxcontroller-0.0.4.tar` & `cc.xboxcontroller-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-02-18 18:13:55.538578 cc.xboxcontroller-0.0.4/
--rw-rw-rw-   0        0        0     1090 2023-02-11 22:46:06.000000 cc.xboxcontroller-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     1271 2023-02-18 18:13:55.535577 cc.xboxcontroller-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      746 2023-02-11 22:46:06.000000 cc.xboxcontroller-0.0.4/README.md
--rw-rw-rw-   0        0        0       86 2023-02-11 22:46:06.000000 cc.xboxcontroller-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-18 18:13:55.538578 cc.xboxcontroller-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      897 2023-02-18 18:12:43.000000 cc.xboxcontroller-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-18 18:13:55.511560 cc.xboxcontroller-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-02-18 18:13:55.519560 cc.xboxcontroller-0.0.4/src/cc/
--rw-rw-rw-   0        0        0       48 2023-02-11 22:46:06.000000 cc.xboxcontroller-0.0.4/src/cc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-18 18:13:55.534577 cc.xboxcontroller-0.0.4/src/cc/xboxcontroller/
--rw-rw-rw-   0        0        0       50 2023-02-11 22:46:06.000000 cc.xboxcontroller-0.0.4/src/cc/xboxcontroller/__init__.py
--rw-rw-rw-   0        0        0    12874 2023-02-18 18:13:37.000000 cc.xboxcontroller-0.0.4/src/cc/xboxcontroller/xboxcontroller.py
-drwxrwxrwx   0        0        0        0 2023-02-18 18:13:55.531569 cc.xboxcontroller-0.0.4/src/cc.xboxcontroller.egg-info/
--rw-rw-rw-   0        0        0     1271 2023-02-18 18:13:55.000000 cc.xboxcontroller-0.0.4/src/cc.xboxcontroller.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2023-02-18 18:13:55.000000 cc.xboxcontroller-0.0.4/src/cc.xboxcontroller.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-18 18:13:55.000000 cc.xboxcontroller-0.0.4/src/cc.xboxcontroller.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-02-18 18:13:55.000000 cc.xboxcontroller-0.0.4/src/cc.xboxcontroller.egg-info/requires.txt
--rw-rw-rw-   0        0        0        3 2023-02-18 18:13:55.000000 cc.xboxcontroller-0.0.4/src/cc.xboxcontroller.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 22:27:53.881653 cc.xboxcontroller-0.1.0/
+-rw-rw-rw-   0        0        0     1090 2023-06-01 22:14:43.000000 cc.xboxcontroller-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1271 2023-06-01 22:27:53.880647 cc.xboxcontroller-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      746 2023-06-01 22:14:43.000000 cc.xboxcontroller-0.1.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-01 22:14:43.000000 cc.xboxcontroller-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-01 22:27:53.881653 cc.xboxcontroller-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      897 2023-06-01 22:26:59.000000 cc.xboxcontroller-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:27:53.839931 cc.xboxcontroller-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-01 22:27:53.859651 cc.xboxcontroller-0.1.0/src/cc/
+-rw-rw-rw-   0        0        0       48 2023-06-01 22:14:43.000000 cc.xboxcontroller-0.1.0/src/cc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:27:53.879647 cc.xboxcontroller-0.1.0/src/cc/xboxcontroller/
+-rw-rw-rw-   0        0        0       50 2023-06-01 22:14:43.000000 cc.xboxcontroller-0.1.0/src/cc/xboxcontroller/__init__.py
+-rw-rw-rw-   0        0        0    14000 2023-06-01 22:26:21.000000 cc.xboxcontroller-0.1.0/src/cc/xboxcontroller/xboxcontroller.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:27:53.877648 cc.xboxcontroller-0.1.0/src/cc.xboxcontroller.egg-info/
+-rw-rw-rw-   0        0        0     1271 2023-06-01 22:27:53.000000 cc.xboxcontroller-0.1.0/src/cc.xboxcontroller.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2023-06-01 22:27:53.000000 cc.xboxcontroller-0.1.0/src/cc.xboxcontroller.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 22:27:53.000000 cc.xboxcontroller-0.1.0/src/cc.xboxcontroller.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-01 22:27:53.000000 cc.xboxcontroller-0.1.0/src/cc.xboxcontroller.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        3 2023-06-01 22:27:53.000000 cc.xboxcontroller-0.1.0/src/cc.xboxcontroller.egg-info/top_level.txt
```

### Comparing `cc.xboxcontroller-0.0.4/LICENSE` & `cc.xboxcontroller-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cc.xboxcontroller-0.0.4/PKG-INFO` & `cc.xboxcontroller-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cc.xboxcontroller
-Version: 0.0.4
+Version: 0.1.0
 Summary: Getting input from Microsoft XBox 360 controllers via the XInput library on Windows.
 Home-page: https://github.com/uncertainty-cc/XboxController-Python
 Author: Uncertainty.
 Author-email: t_k_233@outlook.email
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cc.xboxcontroller-0.0.4/README.md` & `cc.xboxcontroller-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cc.xboxcontroller-0.0.4/setup.py` & `cc.xboxcontroller-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cc.xboxcontroller",
-    version="0.0.4",
+    version="0.1.0",
     author="Uncertainty.",
     author_email="t_k_233@outlook.email",
     description="Getting input from Microsoft XBox 360 controllers via the XInput library on Windows.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/uncertainty-cc/XboxController-Python",
     project_urls={
```

### Comparing `cc.xboxcontroller-0.0.4/src/cc/xboxcontroller/xboxcontroller.py` & `cc.xboxcontroller-0.1.0/src/cc/xboxcontroller/xboxcontroller.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,18 +11,14 @@
 from itertools import count, starmap
 
 from pyglet import event
 
 # structs according to
 # http://msdn.microsoft.com/en-gb/library/windows/desktop/ee417001%28v=vs.85%29.aspx
 
-# add deadzones and dampen noise
-# try appropriate values or simply follow 
-# http://msdn.microsoft.com/en-gb/library/windows/desktop/ee417001%28v=vs.85%29.aspx#dead_zone
-
 
 class XINPUT_GAMEPAD(ctypes.Structure):
     _fields_ = [
         ("buttons", ctypes.c_ushort),       # wButtons
         ("LTrigger", ctypes.c_ubyte),   # bLeftTrigger
         ("RTrigger", ctypes.c_ubyte),  # bLeftTrigger
         ("LX", ctypes.c_short),      # sThumbLX
@@ -109,27 +105,48 @@
 
 
 class Hand:
     LEFT = 0
     RIGHT = 1
 
 
+class Button:
+    Y = 1
+    X = 2
+    B = 3
+    A = 4
+    L = 5
+    BUMPER_R = 7
+    BUMPER_L = 8
+    STICK_R = 9
+    STICK_L = 10
+    BACK = 11
+    START = 12
+    DPAD_R = 13
+    DPAD_L = 14
+    DPAD_D = 15
+    DPAD_U = 16
+
+
+# add deadzones and dampen noise
+# try appropriate values or simply follow 
+# http://msdn.microsoft.com/en-gb/library/windows/desktop/ee417001%28v=vs.85%29.aspx#dead_zone
+
 DEADZONE = 0.08000000000000000
 DAMPEN = 0.00000000500000000
-
+    
 """
 A stateful wrapper to the XboxController, using pyglet event 
 model, that binds to one XInput device and dispatches events 
 when states change.
 
 Example:
 stick = XboxController(0)
 """
 class XboxController(event.EventDispatcher):
-
     max_devices = 4
 
     """
     Returns a list of connected devices.
     """
     @staticmethod
     def enumerateDevices():
@@ -333,47 +350,53 @@
     def getTrigger(self, hand):
         if hand == Hand.LEFT:
             return self.axes["LTrigger"]
         if hand == Hand.RIGHT:
             return self.axes["RTrigger"]
 
     def getYButton(self):
-        return self.buttons[1]
+        return self.buttons[Button.Y]
 
     def getXButton(self):
-        return self.buttons[2]
+        return self.buttons[Button.X]
 
     def getBButton(self):
-        return self.buttons[3]
+        return self.buttons[Button.B]
 
     def getAButton(self):
-        return self.buttons[4]
+        return self.buttons[Button.A]
 
     def getBumper(self, hand):
         if hand == Hand.LEFT:
-            return self.buttons[8]
+            return self.buttons[Button.BUMPER_L]
         if hand == Hand.RIGHT:
-            return self.buttons[7]
+            return self.buttons[Button.BUMPER_R]
+
+    def getStartButton(self):
+        return self.buttons[Button.START]
+        
+    def getBackButton(self):
+        return self.buttons[Button.BACK]
 
     def getPOV(self):
-        if not self.buttons[14] and self.buttons[16] and not self.buttons[13]:
+        if not self.buttons[Button.DPAD_L] and not self.buttons[Button.DPAD_R] and self.buttons[Button.DPAD_U] and not self.buttons[Button.DPAD_D]:
             return 0
-        if self.buttons[16] and self.buttons[13]:
+        elif not self.buttons[Button.DPAD_L] and self.buttons[Button.DPAD_R] and self.buttons[Button.DPAD_U] and not self.buttons[Button.DPAD_D]:
             return 45
-        if not self.buttons[16] and self.buttons[13] and not self.buttons[15]:
+        elif not self.buttons[Button.DPAD_L] and self.buttons[Button.DPAD_R] and not self.buttons[Button.DPAD_U] and not self.buttons[Button.DPAD_D]:
             return 90
-        if self.buttons[13] and self.buttons[15]:
+        elif not self.buttons[Button.DPAD_L] and self.buttons[Button.DPAD_R] and not self.buttons[Button.DPAD_U] and self.buttons[Button.DPAD_D]:
             return 135
-        if not self.buttons[13] and self.buttons[15] and not self.buttons[14]:
+        elif not self.buttons[Button.DPAD_L] and not self.buttons[Button.DPAD_R] and not self.buttons[Button.DPAD_U] and self.buttons[Button.DPAD_D]:
             return 180
-        if self.buttons[14] and self.buttons[15]:
+        elif self.buttons[Button.DPAD_L] and not self.buttons[Button.DPAD_R] and not self.buttons[Button.DPAD_U] and self.buttons[Button.DPAD_D]:
             return 225
-        if not self.buttons[15] and self.buttons[14] and not self.buttons[16]:
+        elif self.buttons[Button.DPAD_L] and not self.buttons[Button.DPAD_R] and not self.buttons[Button.DPAD_U] and not self.buttons[Button.DPAD_D]:
             return 270
-        if self.buttons[14] and self.buttons[16]:
+        elif self.buttons[Button.DPAD_L] and not self.buttons[Button.DPAD_R] and self.buttons[Button.DPAD_U] and not self.buttons[Button.DPAD_D]:
             return 315
         return -1
 
     def onStateChanged(self, state):
         pass
 
     def onAxis(self, axis, value):
```

### Comparing `cc.xboxcontroller-0.0.4/src/cc.xboxcontroller.egg-info/PKG-INFO` & `cc.xboxcontroller-0.1.0/src/cc.xboxcontroller.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cc.xboxcontroller
-Version: 0.0.4
+Version: 0.1.0
 Summary: Getting input from Microsoft XBox 360 controllers via the XInput library on Windows.
 Home-page: https://github.com/uncertainty-cc/XboxController-Python
 Author: Uncertainty.
 Author-email: t_k_233@outlook.email
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

