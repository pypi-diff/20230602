# Comparing `tmp/customtkinterx-0.1.4.tar.gz` & `tmp/customtkinterx-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customtkinterx-0.1.4.tar", max compression
+gzip compressed data, was "customtkinterx-0.1.5.tar", max compression
```

## Comparing `customtkinterx-0.1.4.tar` & `customtkinterx-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      251 2023-05-27 08:34:56.407692 customtkinterx-0.1.4/customtkinterx/__init__.py
--rw-r--r--   0        0        0      175 2023-05-27 12:34:54.450444 customtkinterx-0.1.4/customtkinterx/__main__.py
--rw-r--r--   0        0        0     4283 2023-05-28 11:12:48.677370 customtkinterx-0.1.4/customtkinterx/CTkCustom.py
--rw-r--r--   0        0        0     5311 2023-05-27 14:55:38.518710 customtkinterx-0.1.4/customtkinterx/CTkFluentTheme.py
--rw-r--r--   0        0        0     1204 2023-05-27 11:45:12.773768 customtkinterx-0.1.4/customtkinterx/CTkListBox.py
--rw-r--r--   0        0        0     4700 2023-05-27 15:00:01.395429 customtkinterx-0.1.4/customtkinterx/Fluent.json
--rw-r--r--   0        0        0     2417 2023-05-27 12:33:24.813013 customtkinterx-0.1.4/customtkinterx/LaunchMusix.py
--rw-r--r--   0        0        0      343 2023-05-28 11:12:48.665370 customtkinterx-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1048 2023-05-27 09:39:01.342825 customtkinterx-0.1.4/README.md
--rw-r--r--   0        0        0     1630 1970-01-01 00:00:00.000000 customtkinterx-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      328 2023-06-02 12:01:52.133697 customtkinterx-0.1.5/customtkinterx/__init__.py
+-rw-r--r--   0        0        0      175 2023-05-27 12:34:54.450444 customtkinterx-0.1.5/customtkinterx/__main__.py
+-rw-r--r--   0        0        0     4379 2023-06-02 11:54:36.599580 customtkinterx-0.1.5/customtkinterx/CTkCustom.py
+-rw-r--r--   0        0        0     5624 2023-06-02 12:01:52.102632 customtkinterx-0.1.5/customtkinterx/CTkFluentTheme.py
+-rw-r--r--   0        0        0     3191 2023-06-02 11:54:36.513646 customtkinterx-0.1.5/customtkinterx/CTkInfoBar.py
+-rw-r--r--   0        0        0     1244 2023-06-02 11:00:54.754723 customtkinterx-0.1.5/customtkinterx/CTkListBox.py
+-rw-r--r--   0        0        0     5002 2023-06-02 11:05:57.727124 customtkinterx-0.1.5/customtkinterx/Fluent.json
+-rw-r--r--   0        0        0     2417 2023-05-27 12:33:24.813013 customtkinterx-0.1.5/customtkinterx/LaunchMusix.py
+-rw-r--r--   0        0        0      343 2023-06-02 12:02:17.150168 customtkinterx-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1489 2023-06-02 11:54:36.456311 customtkinterx-0.1.5/README.md
+-rw-r--r--   0        0        0     2054 1970-01-01 00:00:00.000000 customtkinterx-0.1.5/PKG-INFO
```

### Comparing `customtkinterx-0.1.4/customtkinterx/CTkCustom.py` & `customtkinterx-0.1.5/customtkinterx/CTkCustom.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,14 +91,18 @@
         return self.__label_title
 
     @property
     def titlebar_closebutton(self):
         return self.__button_close
 
     @property
+    def titlebar_minimizebutton(self):
+        return self.__button_minimize
+
+    @property
     def mainframe(self):
         return self.__frame_border
 
     def _click(self, event):
         self.x, self.y = event.x, event.y
 
     def _move(self, event):
```

### Comparing `customtkinterx-0.1.4/customtkinterx/CTkFluentTheme.py` & `customtkinterx-0.1.5/customtkinterx/CTkFluentTheme.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 fluent_json = """
 {
+  "CTkInfoBar": {
+    "corner_radius": 8,
+    "border_width": 0,
+    "fg_color": ["#f7f7f7", "#2f2f2f"],
+    "border_color": ["#b0b2b2", "#424556"],
+
+    "success_color": ["#dff6dd", "#393d1b"],
+    "caution_color": ["#fff4ce", "#433519"],
+    "critical_color": ["#fde7e9", "#442726"]
+  },
+
   "CTk": {
     "fg_color": ["#ffffff", "#101010"]
   },
   "CTkToplevel": {
     "fg_color": ["#ffffff", "#101010"]
   },
   "CTkFrame": {
@@ -43,17 +54,17 @@
     "hover_color": ["#3B8ED0", "#1F6AA5"],
     "checkmark_color": ["#DCE4EE", "gray90"],
     "text_color": ["gray10", "#DCE4EE"],
     "text_color_disabled": ["gray60", "gray45"]
   },
   "CTkSwitch": {
     "corner_radius": 1000,
-    "border_width": 1,
+    "border_width": 0.1,
     "button_length": 0,
-    "fg_color": ["#939BA2", "#4A4D50"],
+    "fg_color": ["#ededed", "#1d1d1d"],
     "progress_color": ["#0067c0", "#4cc2ff"],
     "button_color": ["#f3f3f3", "#000000"],
     "button_hover_color": ["#bfbfbf", "#050505"],
     "text_color": ["gray10", "#DCE4EE"],
     "text_color_disabled": ["gray60", "gray45"]
   },
   "CTkRadiobutton": {
@@ -139,15 +150,15 @@
   "CTkFont": {
     "macOS": {
       "family": "SF Display",
       "size": 13,
       "weight": "normal"
     },
     "Windows": {
-      "family": "Roboto",
+      "family": "Microsoft YaHei",
       "size": 13,
       "weight": "normal"
     },
     "Linux": {
       "family": "Roboto",
       "size": 13,
       "weight": "normal"
```

### Comparing `customtkinterx-0.1.4/customtkinterx/CTkListBox.py` & `customtkinterx-0.1.5/customtkinterx/CTkListBox.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,15 +20,17 @@
         return __frame, __label
 
     def clear(self):
         for index in self.winfo_children(): index.destroy()
 
 
 if __name__ == '__main__':
-    from customtkinterx import CTkCustom
+    from customtkinterx import CTkCustom, CTkFluentTheme
+
+    CTkFluentTheme()
 
     root = CTkCustom()
     root.create_sizegrip()
 
     list = CTkList(root.mainframe)
 
     for index in range(20):
```

### Comparing `customtkinterx-0.1.4/customtkinterx/Fluent.json` & `customtkinterx-0.1.5/customtkinterx/Fluent.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9493055555555555%*

 * *Differences: {"'CTkFont'": "{'Windows': {'size': 13}}",*

 * * "'CTkInfoBar'": "OrderedDict([('corner_radius', 8), ('border_width', 0), ('fg_color', ['#f7f7f7', "*

 * *                 "'#2f2f2f']), ('border_color', ['#b0b2b2', '#424556']), ('success_color', "*

 * *                 "['#dff6dd', '#393d1b']), ('caution_color', ['#fff4ce', '#433519']), "*

 * *                 "('critical_color', ['#fde7e9', '#442726'])])"}*

```diff
@@ -109,15 +109,15 @@
         "Linux": {
             "family": "Roboto",
             "size": 13,
             "weight": "normal"
         },
         "Windows": {
             "family": "Microsoft YaHei",
-            "size": 12,
+            "size": 13,
             "weight": "normal"
         },
         "macOS": {
             "family": "SF Display",
             "size": 13,
             "weight": "normal"
         }
@@ -134,14 +134,38 @@
             "#1c1c1c"
         ],
         "top_fg_color": [
             "#ffffff",
             "#2c2c2c"
         ]
     },
+    "CTkInfoBar": {
+        "border_color": [
+            "#b0b2b2",
+            "#424556"
+        ],
+        "border_width": 0,
+        "caution_color": [
+            "#fff4ce",
+            "#433519"
+        ],
+        "corner_radius": 8,
+        "critical_color": [
+            "#fde7e9",
+            "#442726"
+        ],
+        "fg_color": [
+            "#f7f7f7",
+            "#2f2f2f"
+        ],
+        "success_color": [
+            "#dff6dd",
+            "#393d1b"
+        ]
+    },
     "CTkLabel": {
         "corner_radius": 0,
         "fg_color": "transparent",
         "text_color": [
             "gray10",
             "#DCE4EE"
         ]
```

### Comparing `customtkinterx-0.1.4/customtkinterx/LaunchMusix.py` & `customtkinterx-0.1.5/customtkinterx/LaunchMusix.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.1.4/PKG-INFO` & `customtkinterx-0.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: customtkinterx
-Version: 0.1.4
+Version: 0.1.5
 Summary: extra widgets for customtkinter
 Author: XiangQinxi
 Author-email: XiangQinxi@outlook.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -23,19 +23,29 @@
 ```python
 from customtkinter import *
 from customtkinterx import *
 
 CTkFluentTheme()
 ```
 
-## 自定义窗口
+## CTkCustom 自定义窗口
 原窗口因标题栏与边框的限制，导致界面效果极差，但是仍可以通过一些方法自定义窗口`wm_overrideredirect`。
 平台支持`Windows` `MacOS` `Linux`，其中界面效果支持最好的是`Windows`，`MacOS` `Linux`无法使用透明色，完全消除边框使用圆角，
 及将图标保留至任务栏，采用置顶的方法保持窗口的显示。
 
+### 组件结构
+```markdown
+| CTkCustom -> CTk
+|-->> __frame_border(mainframe): CTkFrame
+|-->> __frame_title(titlebar): CTkFrame
+|-->> __label_title(titlebar_title): CTkLabel
+|-->> __button_close(titlebar_closebutton): CTkButton
+|-->> __button_minimize(titlebar_minimizebutton): CTkButton
+```
+
 ### 基础示例
 ```python
 from customtkinter import *
 from customtkinterx import *
 
 root = CTkCustom()
 
@@ -51,7 +61,14 @@
 from customtkinterx import *
 
 root = CTkCustom()
 root.create_sizegrip()
 
 root.mainloop()
 ```
+
+## CTkInfoBar 消息栏
+### 组件结构
+```markdown
+| CTkInforBar -> CTkFrame
+|-->> __label_info(info): CTkLabel
+```
```

