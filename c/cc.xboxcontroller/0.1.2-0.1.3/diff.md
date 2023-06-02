# Comparing `tmp/cc.xboxcontroller-0.1.2.tar.gz` & `tmp/cc.xboxcontroller-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cc.xboxcontroller-0.1.2.tar", last modified: Thu Jun  1 22:58:54 2023, max compression
+gzip compressed data, was "cc.xboxcontroller-0.1.3.tar", last modified: Fri Jun  2 00:02:25 2023, max compression
```

## Comparing `cc.xboxcontroller-0.1.2.tar` & `cc.xboxcontroller-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 22:58:54.452936 cc.xboxcontroller-0.1.2/
--rw-rw-rw-   0        0        0     1090 2023-06-01 22:51:15.000000 cc.xboxcontroller-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     1274 2023-06-01 22:58:54.451939 cc.xboxcontroller-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      749 2023-06-01 22:58:16.000000 cc.xboxcontroller-0.1.2/README.md
--rw-rw-rw-   0        0        0       86 2023-06-01 22:51:15.000000 cc.xboxcontroller-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-01 22:58:54.452936 cc.xboxcontroller-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      897 2023-06-01 22:58:38.000000 cc.xboxcontroller-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 22:58:54.415936 cc.xboxcontroller-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-01 22:58:54.425938 cc.xboxcontroller-0.1.2/src/cc/
--rw-rw-rw-   0        0        0       56 2023-06-01 22:57:25.000000 cc.xboxcontroller-0.1.2/src/cc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 22:58:54.449935 cc.xboxcontroller-0.1.2/src/cc/xboxcontroller/
--rw-rw-rw-   0        0        0       58 2023-06-01 22:57:25.000000 cc.xboxcontroller-0.1.2/src/cc/xboxcontroller/__init__.py
--rw-rw-rw-   0        0        0    14074 2023-06-01 22:57:54.000000 cc.xboxcontroller-0.1.2/src/cc/xboxcontroller/xboxcontroller.py
-drwxrwxrwx   0        0        0        0 2023-06-01 22:58:54.445937 cc.xboxcontroller-0.1.2/src/cc.xboxcontroller.egg-info/
--rw-rw-rw-   0        0        0     1274 2023-06-01 22:58:54.000000 cc.xboxcontroller-0.1.2/src/cc.xboxcontroller.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2023-06-01 22:58:54.000000 cc.xboxcontroller-0.1.2/src/cc.xboxcontroller.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 22:58:54.000000 cc.xboxcontroller-0.1.2/src/cc.xboxcontroller.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-01 22:58:54.000000 cc.xboxcontroller-0.1.2/src/cc.xboxcontroller.egg-info/requires.txt
--rw-rw-rw-   0        0        0        3 2023-06-01 22:58:54.000000 cc.xboxcontroller-0.1.2/src/cc.xboxcontroller.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 00:02:25.471769 cc.xboxcontroller-0.1.3/
+-rw-rw-rw-   0        0        0     1090 2023-06-01 23:58:02.000000 cc.xboxcontroller-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     1262 2023-06-02 00:02:25.471769 cc.xboxcontroller-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      737 2023-06-01 23:58:02.000000 cc.xboxcontroller-0.1.3/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-01 23:58:02.000000 cc.xboxcontroller-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-02 00:02:25.471769 cc.xboxcontroller-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      897 2023-06-01 23:59:24.000000 cc.xboxcontroller-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 00:02:25.450753 cc.xboxcontroller-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-02 00:02:25.455751 cc.xboxcontroller-0.1.3/src/cc/
+-rw-rw-rw-   0        0        0       56 2023-06-01 23:58:02.000000 cc.xboxcontroller-0.1.3/src/cc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 00:02:25.470750 cc.xboxcontroller-0.1.3/src/cc/xboxcontroller/
+-rw-rw-rw-   0        0        0       58 2023-06-01 23:58:02.000000 cc.xboxcontroller-0.1.3/src/cc/xboxcontroller/__init__.py
+-rw-rw-rw-   0        0        0    14001 2023-06-02 00:01:19.000000 cc.xboxcontroller-0.1.3/src/cc/xboxcontroller/xboxcontroller.py
+drwxrwxrwx   0        0        0        0 2023-06-02 00:02:25.468750 cc.xboxcontroller-0.1.3/src/cc.xboxcontroller.egg-info/
+-rw-rw-rw-   0        0        0     1262 2023-06-02 00:02:25.000000 cc.xboxcontroller-0.1.3/src/cc.xboxcontroller.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2023-06-02 00:02:25.000000 cc.xboxcontroller-0.1.3/src/cc.xboxcontroller.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 00:02:25.000000 cc.xboxcontroller-0.1.3/src/cc.xboxcontroller.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-02 00:02:25.000000 cc.xboxcontroller-0.1.3/src/cc.xboxcontroller.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        3 2023-06-02 00:02:25.000000 cc.xboxcontroller-0.1.3/src/cc.xboxcontroller.egg-info/top_level.txt
```

### Comparing `cc.xboxcontroller-0.1.2/LICENSE` & `cc.xboxcontroller-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cc.xboxcontroller-0.1.2/PKG-INFO` & `cc.xboxcontroller-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cc.xboxcontroller
-Version: 0.1.2
+Version: 0.1.3
 Summary: Getting input from Microsoft XBox 360 controllers via the XInput library on Windows.
 Home-page: https://github.com/uncertainty-cc/XboxController-Python
 Author: Uncertainty.
 Author-email: t_k_233@outlook.email
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,15 +22,14 @@
 pip install cc-xboxcontroller
 ```
 
 ## Usage
 
 ```python
 import time
-import sys
 
 from cc.xboxcontroller import XboxController, Hand
 
 def main():
     """
     """
     stick = XboxController(0)
```

### Comparing `cc.xboxcontroller-0.1.2/README.md` & `cc.xboxcontroller-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 pip install cc-xboxcontroller
 ```
 
 ## Usage
 
 ```python
 import time
-import sys
 
 from cc.xboxcontroller import XboxController, Hand
 
 def main():
     """
     """
     stick = XboxController(0)
```

### Comparing `cc.xboxcontroller-0.1.2/setup.py` & `cc.xboxcontroller-0.1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cc.xboxcontroller",
-    version="0.1.2",
+    version="0.1.3",
     author="Uncertainty.",
     author_email="t_k_233@outlook.email",
     description="Getting input from Microsoft XBox 360 controllers via the XInput library on Windows.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/uncertainty-cc/XboxController-Python",
     project_urls={
```

### Comparing `cc.xboxcontroller-0.1.2/src/cc/xboxcontroller/xboxcontroller.py` & `cc.xboxcontroller-0.1.3/src/cc/xboxcontroller/xboxcontroller.py`

 * *Files 1% similar despite different names*

```diff
@@ -373,18 +373,14 @@
 
     def getStartButton(self):
         return self.buttons[Button.START]
         
     def getBackButton(self):
         return self.buttons[Button.BACK]
 
-    @deprecated
-    def getPOV(self):
-        return self.getDPad()
-
     def getDPad(self):
         if not self.buttons[Button.DPAD_L] and not self.buttons[Button.DPAD_R] and self.buttons[Button.DPAD_U] and not self.buttons[Button.DPAD_D]:
             return 0
         elif not self.buttons[Button.DPAD_L] and self.buttons[Button.DPAD_R] and self.buttons[Button.DPAD_U] and not self.buttons[Button.DPAD_D]:
             return 45
         elif not self.buttons[Button.DPAD_L] and self.buttons[Button.DPAD_R] and not self.buttons[Button.DPAD_U] and not self.buttons[Button.DPAD_D]:
             return 90
```

### Comparing `cc.xboxcontroller-0.1.2/src/cc.xboxcontroller.egg-info/PKG-INFO` & `cc.xboxcontroller-0.1.3/src/cc.xboxcontroller.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cc.xboxcontroller
-Version: 0.1.2
+Version: 0.1.3
 Summary: Getting input from Microsoft XBox 360 controllers via the XInput library on Windows.
 Home-page: https://github.com/uncertainty-cc/XboxController-Python
 Author: Uncertainty.
 Author-email: t_k_233@outlook.email
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,15 +22,14 @@
 pip install cc-xboxcontroller
 ```
 
 ## Usage
 
 ```python
 import time
-import sys
 
 from cc.xboxcontroller import XboxController, Hand
 
 def main():
     """
     """
     stick = XboxController(0)
```

