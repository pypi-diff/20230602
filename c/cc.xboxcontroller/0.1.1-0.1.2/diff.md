# Comparing `tmp/cc.xboxcontroller-0.1.1.tar.gz` & `tmp/cc.xboxcontroller-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cc.xboxcontroller-0.1.1.tar", last modified: Thu Jun  1 22:41:02 2023, max compression
+gzip compressed data, was "cc.xboxcontroller-0.1.2.tar", last modified: Thu Jun  1 22:58:54 2023, max compression
```

## Comparing `cc.xboxcontroller-0.1.1.tar` & `cc.xboxcontroller-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 22:41:02.077659 cc.xboxcontroller-0.1.1/
--rw-rw-rw-   0        0        0     1090 2023-06-01 22:38:24.000000 cc.xboxcontroller-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1271 2023-06-01 22:41:02.041140 cc.xboxcontroller-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      746 2023-06-01 22:38:24.000000 cc.xboxcontroller-0.1.1/README.md
--rw-rw-rw-   0        0        0       86 2023-06-01 22:38:24.000000 cc.xboxcontroller-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-01 22:41:02.077659 cc.xboxcontroller-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      897 2023-06-01 22:40:47.000000 cc.xboxcontroller-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 22:41:02.013167 cc.xboxcontroller-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-01 22:41:02.022156 cc.xboxcontroller-0.1.1/src/cc/
--rw-rw-rw-   0        0        0       56 2023-06-01 22:38:42.000000 cc.xboxcontroller-0.1.1/src/cc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 22:41:02.040138 cc.xboxcontroller-0.1.1/src/cc/xboxcontroller/
--rw-rw-rw-   0        0        0       58 2023-06-01 22:38:40.000000 cc.xboxcontroller-0.1.1/src/cc/xboxcontroller/__init__.py
--rw-rw-rw-   0        0        0    14000 2023-06-01 22:38:24.000000 cc.xboxcontroller-0.1.1/src/cc/xboxcontroller/xboxcontroller.py
-drwxrwxrwx   0        0        0        0 2023-06-01 22:41:02.037140 cc.xboxcontroller-0.1.1/src/cc.xboxcontroller.egg-info/
--rw-rw-rw-   0        0        0     1271 2023-06-01 22:41:01.000000 cc.xboxcontroller-0.1.1/src/cc.xboxcontroller.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2023-06-01 22:41:02.000000 cc.xboxcontroller-0.1.1/src/cc.xboxcontroller.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 22:41:01.000000 cc.xboxcontroller-0.1.1/src/cc.xboxcontroller.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-01 22:41:01.000000 cc.xboxcontroller-0.1.1/src/cc.xboxcontroller.egg-info/requires.txt
--rw-rw-rw-   0        0        0        3 2023-06-01 22:41:01.000000 cc.xboxcontroller-0.1.1/src/cc.xboxcontroller.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 22:58:54.452936 cc.xboxcontroller-0.1.2/
+-rw-rw-rw-   0        0        0     1090 2023-06-01 22:51:15.000000 cc.xboxcontroller-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1274 2023-06-01 22:58:54.451939 cc.xboxcontroller-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      749 2023-06-01 22:58:16.000000 cc.xboxcontroller-0.1.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-01 22:51:15.000000 cc.xboxcontroller-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-01 22:58:54.452936 cc.xboxcontroller-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      897 2023-06-01 22:58:38.000000 cc.xboxcontroller-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:58:54.415936 cc.xboxcontroller-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-01 22:58:54.425938 cc.xboxcontroller-0.1.2/src/cc/
+-rw-rw-rw-   0        0        0       56 2023-06-01 22:57:25.000000 cc.xboxcontroller-0.1.2/src/cc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:58:54.449935 cc.xboxcontroller-0.1.2/src/cc/xboxcontroller/
+-rw-rw-rw-   0        0        0       58 2023-06-01 22:57:25.000000 cc.xboxcontroller-0.1.2/src/cc/xboxcontroller/__init__.py
+-rw-rw-rw-   0        0        0    14074 2023-06-01 22:57:54.000000 cc.xboxcontroller-0.1.2/src/cc/xboxcontroller/xboxcontroller.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:58:54.445937 cc.xboxcontroller-0.1.2/src/cc.xboxcontroller.egg-info/
+-rw-rw-rw-   0        0        0     1274 2023-06-01 22:58:54.000000 cc.xboxcontroller-0.1.2/src/cc.xboxcontroller.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2023-06-01 22:58:54.000000 cc.xboxcontroller-0.1.2/src/cc.xboxcontroller.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 22:58:54.000000 cc.xboxcontroller-0.1.2/src/cc.xboxcontroller.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-01 22:58:54.000000 cc.xboxcontroller-0.1.2/src/cc.xboxcontroller.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        3 2023-06-01 22:58:54.000000 cc.xboxcontroller-0.1.2/src/cc.xboxcontroller.egg-info/top_level.txt
```

### Comparing `cc.xboxcontroller-0.1.1/LICENSE` & `cc.xboxcontroller-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cc.xboxcontroller-0.1.1/PKG-INFO` & `cc.xboxcontroller-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cc.xboxcontroller
-Version: 0.1.1
+Version: 0.1.2
 Summary: Getting input from Microsoft XBox 360 controllers via the XInput library on Windows.
 Home-page: https://github.com/uncertainty-cc/XboxController-Python
 Author: Uncertainty.
 Author-email: t_k_233@outlook.email
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,15 +36,15 @@
     stick = XboxController(0)
 
     while True:
         stick.update()
         stick.setRumble(Hand.LEFT, abs(stick.axes["LTrigger"]))
         stick.setRumble(Hand.RIGHT, abs(stick.axes["RTrigger"]))
         print("A Btn:", stick.getAButton(), end="")
-        print("\tPOV:", stick.getPOV(), end="")
+        print("\tD-pad:", stick.getDPad(), end="")
         print("\tX Axis:", stick.getX(Hand.LEFT))
         time.sleep(.01)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `cc.xboxcontroller-0.1.1/README.md` & `cc.xboxcontroller-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     stick = XboxController(0)
 
     while True:
         stick.update()
         stick.setRumble(Hand.LEFT, abs(stick.axes["LTrigger"]))
         stick.setRumble(Hand.RIGHT, abs(stick.axes["RTrigger"]))
         print("A Btn:", stick.getAButton(), end="")
-        print("\tPOV:", stick.getPOV(), end="")
+        print("\tD-pad:", stick.getDPad(), end="")
         print("\tX Axis:", stick.getX(Hand.LEFT))
         time.sleep(.01)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `cc.xboxcontroller-0.1.1/setup.py` & `cc.xboxcontroller-0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cc.xboxcontroller",
-    version="0.1.1",
+    version="0.1.2",
     author="Uncertainty.",
     author_email="t_k_233@outlook.email",
     description="Getting input from Microsoft XBox 360 controllers via the XInput library on Windows.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/uncertainty-cc/XboxController-Python",
     project_urls={
```

### Comparing `cc.xboxcontroller-0.1.1/src/cc/xboxcontroller/xboxcontroller.py` & `cc.xboxcontroller-0.1.2/src/cc/xboxcontroller/xboxcontroller.py`

 * *Files 1% similar despite different names*

```diff
@@ -373,15 +373,19 @@
 
     def getStartButton(self):
         return self.buttons[Button.START]
         
     def getBackButton(self):
         return self.buttons[Button.BACK]
 
+    @deprecated
     def getPOV(self):
+        return self.getDPad()
+
+    def getDPad(self):
         if not self.buttons[Button.DPAD_L] and not self.buttons[Button.DPAD_R] and self.buttons[Button.DPAD_U] and not self.buttons[Button.DPAD_D]:
             return 0
         elif not self.buttons[Button.DPAD_L] and self.buttons[Button.DPAD_R] and self.buttons[Button.DPAD_U] and not self.buttons[Button.DPAD_D]:
             return 45
         elif not self.buttons[Button.DPAD_L] and self.buttons[Button.DPAD_R] and not self.buttons[Button.DPAD_U] and not self.buttons[Button.DPAD_D]:
             return 90
         elif not self.buttons[Button.DPAD_L] and self.buttons[Button.DPAD_R] and not self.buttons[Button.DPAD_U] and self.buttons[Button.DPAD_D]:
```

### Comparing `cc.xboxcontroller-0.1.1/src/cc.xboxcontroller.egg-info/PKG-INFO` & `cc.xboxcontroller-0.1.2/src/cc.xboxcontroller.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cc.xboxcontroller
-Version: 0.1.1
+Version: 0.1.2
 Summary: Getting input from Microsoft XBox 360 controllers via the XInput library on Windows.
 Home-page: https://github.com/uncertainty-cc/XboxController-Python
 Author: Uncertainty.
 Author-email: t_k_233@outlook.email
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,15 +36,15 @@
     stick = XboxController(0)
 
     while True:
         stick.update()
         stick.setRumble(Hand.LEFT, abs(stick.axes["LTrigger"]))
         stick.setRumble(Hand.RIGHT, abs(stick.axes["RTrigger"]))
         print("A Btn:", stick.getAButton(), end="")
-        print("\tPOV:", stick.getPOV(), end="")
+        print("\tD-pad:", stick.getDPad(), end="")
         print("\tX Axis:", stick.getX(Hand.LEFT))
         time.sleep(.01)
 
 
 if __name__ == "__main__":
     main()
```

