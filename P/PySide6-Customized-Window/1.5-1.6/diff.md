# Comparing `tmp/PySide6_Customized_Window-1.5-py3-none-any.whl.zip` & `tmp/PySide6_Customized_Window-1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 11548 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat    47876 b- defN 23-Jun-02 14:29 PySide6_Customized_Window.py
--rw-rw-rw-  2.0 fat        1 b- defN 23-Jun-02 14:39 PySide6_Customized_Window-1.5.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-02 14:39 PySide6_Customized_Window-1.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     2669 b- defN 23-Jun-02 14:39 PySide6_Customized_Window-1.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat      452 b- defN 23-Jun-02 14:39 PySide6_Customized_Window-1.5.dist-info/RECORD
-5 files, 51095 bytes uncompressed, 10706 bytes compressed:  79.0%
+Zip file size: 11554 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat    47878 b- defN 23-Jun-02 15:13 PySide6_Customized_Window.py
+-rw-rw-rw-  2.0 fat        1 b- defN 23-Jun-02 15:28 PySide6_Customized_Window-1.6.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-02 15:28 PySide6_Customized_Window-1.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     2669 b- defN 23-Jun-02 15:28 PySide6_Customized_Window-1.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      452 b- defN 23-Jun-02 15:28 PySide6_Customized_Window-1.6.dist-info/RECORD
+5 files, 51097 bytes uncompressed, 10712 bytes compressed:  79.0%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: PySide6_Customized_Window.py
 Comment: 
 
-Filename: PySide6_Customized_Window-1.5.dist-info/top_level.txt
+Filename: PySide6_Customized_Window-1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: PySide6_Customized_Window-1.5.dist-info/WHEEL
+Filename: PySide6_Customized_Window-1.6.dist-info/WHEEL
 Comment: 
 
-Filename: PySide6_Customized_Window-1.5.dist-info/METADATA
+Filename: PySide6_Customized_Window-1.6.dist-info/METADATA
 Comment: 
 
-Filename: PySide6_Customized_Window-1.5.dist-info/RECORD
+Filename: PySide6_Customized_Window-1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## PySide6_Customized_Window.py

```diff
@@ -94,15 +94,15 @@
         self.ACCENT_ENABLE_BLURBEHIND = 3
         self.ACCENT_ENABLE_ACRYLICBLURBEHIND = 4
         self.SetWindowCompositionAttribute = ctypes.windll.user32.SetWindowCompositionAttribute
         self.accentPolicy = ACCENT_POLICY()
         self.winCompAttrData = WINDOWCOMPOSITIONATTRIBDATA()
         self.winCompAttrData.Attribute = self.WCA_ACCENT_POLICY
         self.winCompAttrData.SizeOfData = ctypes.sizeof(self.accentPolicy)
-        self.winCompAttrData.Data = ctypes.byref(self.accentPolicy)
+        self.winCompAttrData.Data = ctypes.pointer(self.accentPolicy)
     def setAeroEffect(self, hWnd, gradientColor='01000000', isEnableShadow=True, animationId=0):
         gradientColor = ctypes.c_ulong(int(gradientColor, base=16))
         animationId = ctypes.c_ulong(animationId)
         accentFlags = ctypes.c_ulong(0x20 | 0x40 | 0x80 | 0x100 | 0x200) if isEnableShadow else ctypes.c_ulong(0)
         self.accentPolicy.AccentState = self.ACCENT_ENABLE_BLURBEHIND
         self.accentPolicy.GradientColor = gradientColor
         self.accentPolicy.AccentFlags = accentFlags
```

## Comparing `PySide6_Customized_Window-1.5.dist-info/METADATA` & `PySide6_Customized_Window-1.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySide6-Customized-Window
-Version: 1.5
+Version: 1.6
 Summary: A customized window based on PySideX.
 Home-page: https://yuzhouren86.github.io
 Author: YuZhouRen86
 Author-email: UNKNOWN
 License: UNKNOWN
 Keywords: Python GUI PySide
 Platform: UNKNOWN
```

