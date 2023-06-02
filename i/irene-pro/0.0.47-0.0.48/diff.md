# Comparing `tmp/irene_pro-0.0.47.tar.gz` & `tmp/irene_pro-0.0.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irene_pro-0.0.47.tar", last modified: Tue May 30 10:48:16 2023, max compression
+gzip compressed data, was "irene_pro-0.0.48.tar", last modified: Fri Jun  2 07:48:47 2023, max compression
```

## Comparing `irene_pro-0.0.47.tar` & `irene_pro-0.0.48.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 10:48:16.336006 irene_pro-0.0.47/
--rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.47/LICENSE
--rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.47/MANIFEST.in
--rw-rw-rw-   0        0        0     1740 2023-05-30 10:48:16.327030 irene_pro-0.0.47/PKG-INFO
--rw-rw-rw-   0        0        0     1165 2023-05-25 07:51:23.000000 irene_pro-0.0.47/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 10:48:16.294118 irene_pro-0.0.47/irene_pro/
--rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.47/irene_pro/__init__.py
--rw-rw-rw-   0        0        0     4980 2023-05-30 10:44:24.000000 irene_pro-0.0.47/irene_pro/logic.py
--rw-rw-rw-   0        0        0    32045 2023-05-26 07:13:56.000000 irene_pro-0.0.47/irene_pro/widgets.py
-drwxrwxrwx   0        0        0        0 2023-05-30 10:48:16.324038 irene_pro-0.0.47/irene_pro.egg-info/
--rw-rw-rw-   0        0        0     1740 2023-05-30 10:48:16.000000 irene_pro-0.0.47/irene_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-05-30 10:48:16.000000 irene_pro-0.0.47/irene_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 10:48:16.000000 irene_pro-0.0.47/irene_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-30 10:48:16.000000 irene_pro-0.0.47/irene_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-30 10:48:16.000000 irene_pro-0.0.47/irene_pro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 10:48:16.337004 irene_pro-0.0.47/setup.cfg
--rw-rw-rw-   0        0        0     1164 2023-05-30 10:46:49.000000 irene_pro-0.0.47/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 07:48:47.766466 irene_pro-0.0.48/
+-rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.48/LICENSE
+-rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.48/MANIFEST.in
+-rw-rw-rw-   0        0        0     1940 2023-06-02 07:48:47.764499 irene_pro-0.0.48/PKG-INFO
+-rw-rw-rw-   0        0        0     1360 2023-06-02 07:47:21.000000 irene_pro-0.0.48/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 07:48:47.748820 irene_pro-0.0.48/irene_pro/
+-rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.48/irene_pro/__init__.py
+-rw-rw-rw-   0        0        0     5920 2023-06-02 07:39:01.000000 irene_pro-0.0.48/irene_pro/logic.py
+-rw-rw-rw-   0        0        0    32045 2023-05-26 07:13:56.000000 irene_pro-0.0.48/irene_pro/widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-02 07:48:47.762535 irene_pro-0.0.48/irene_pro.egg-info/
+-rw-rw-rw-   0        0        0     1940 2023-06-02 07:48:47.000000 irene_pro-0.0.48/irene_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-06-02 07:48:47.000000 irene_pro-0.0.48/irene_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 07:48:47.000000 irene_pro-0.0.48/irene_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-02 07:48:47.000000 irene_pro-0.0.48/irene_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-02 07:48:47.000000 irene_pro-0.0.48/irene_pro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 07:48:47.766466 irene_pro-0.0.48/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2023-06-02 07:39:47.000000 irene_pro-0.0.48/setup.py
```

### Comparing `irene_pro-0.0.47/PKG-INFO` & `irene_pro-0.0.48/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene_pro
-Version: 0.0.47
+Version: 0.0.48
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -39,8 +39,13 @@
 # get the sign_in_btn
 login_btn = sign.Login_btn()
 # call a function if the validation is successfully
 login_btn.config(command = sign.validate_login(callback = func_to_call, saved_username, saved_password))
 
 # SQLITE3 DATABASE ADDED IN LOGIC LIBRALY
 # Sub menu to extend the functionalities like edit, delete and getting some details on the selected label
+# converting datetime string into seconds
+from irene_pro.logic import DateTime
+date_obj = DateTime()
+seconds = date_obj.convert_to_seconds(datetime_str = "14 days, 03:26:00")
+print(seconds)
```

### Comparing `irene_pro-0.0.47/README.md` & `irene_pro-0.0.48/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -22,8 +22,13 @@
 # get the sign_in_btn
 login_btn = sign.Login_btn()
 # call a function if the validation is successfully
 login_btn.config(command = sign.validate_login(callback = func_to_call, saved_username, saved_password))
 
 # SQLITE3 DATABASE ADDED IN LOGIC LIBRALY
 # Sub menu to extend the functionalities like edit, delete and getting some details on the selected label
+# converting datetime string into seconds
+from irene_pro.logic import DateTime
+date_obj = DateTime()
+seconds = date_obj.convert_to_seconds(datetime_str = "14 days, 03:26:00")
+print(seconds)
```

### Comparing `irene_pro-0.0.47/irene_pro/logic.py` & `irene_pro-0.0.48/irene_pro/logic.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,14 +20,37 @@
         date1 = datetime.strptime(start, "%Y-%m-%d %H:%M:%S")
         date2 = datetime.strptime(end, "%Y-%m-%d %H:%M:%S")
         delta = date2 - date1
         return delta
     @property
     def combinedDate(self):
         return [self.year, self.month, self.current_weeks, self.day, self.combined]
+    
+    def convert_to_seconds(self, datetime_str:str):
+        # SPLIT WITH ,
+        comma_split = datetime_str.split(",")
+        if len(comma_split) == 2:
+            days, hours = comma_split
+            only_day_num = int(float(days.split(" ")[0]))
+            hr, minute, sec = hours.split(":")
+            hr = int(float(hr))
+            minute = int(float(minute))
+            sec = int(float(sec))
+            seconds = (only_day_num * 86400) + (hr * 3600) + (minute*60) + sec
+            return seconds
+        elif len(comma_split) == 1:
+            try:
+                hr, minute, sec = comma_split[0].split(":")
+                hr = int(float(hr))
+                minute = int(float(minute))
+                sec = int(float(sec))
+                seconds = (hr * 3600) + (minute*60) + sec
+                return seconds
+            except ValueError:
+                return "INVALID TOTAL TIME FORMAT"
 
 def separate(numbers):
     floating = []
     new_str = ""
     float_pos = 0
     decision = ""
     sign_negative = ""
```

### Comparing `irene_pro-0.0.47/irene_pro/widgets.py` & `irene_pro-0.0.48/irene_pro/widgets.py`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.47/irene_pro.egg-info/PKG-INFO` & `irene_pro-0.0.48/irene_pro.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene-pro
-Version: 0.0.47
+Version: 0.0.48
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -39,8 +39,13 @@
 # get the sign_in_btn
 login_btn = sign.Login_btn()
 # call a function if the validation is successfully
 login_btn.config(command = sign.validate_login(callback = func_to_call, saved_username, saved_password))
 
 # SQLITE3 DATABASE ADDED IN LOGIC LIBRALY
 # Sub menu to extend the functionalities like edit, delete and getting some details on the selected label
+# converting datetime string into seconds
+from irene_pro.logic import DateTime
+date_obj = DateTime()
+seconds = date_obj.convert_to_seconds(datetime_str = "14 days, 03:26:00")
+print(seconds)
```

### Comparing `irene_pro-0.0.47/setup.py` & `irene_pro-0.0.48/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 286f 732e 7061 7468 2e6a 6f69 6e28 6865  (os.path.join(he
 000000a0: 7265 2c20 2252 4541 444d 452e 6d64 2229  re, "README.md")
 000000b0: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
 000000c0: 3822 2920 6173 2066 683a 0d0a 2020 2020  8") as fh:..    
 000000d0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000e0: 203d 2022 5c6e 2220 2b20 6668 2e72 6561   = "\n" + fh.rea
 000000f0: 6428 290d 0a0d 0a56 4552 5349 4f4e 203d  d()....VERSION =
-00000100: 2027 302e 302e 3437 270d 0a44 4553 4352   '0.0.47'..DESCR
+00000100: 2027 302e 302e 3438 270d 0a44 4553 4352   '0.0.48'..DESCR
 00000110: 4950 5449 4f4e 203d 2027 5573 6520 6375  IPTION = 'Use cu
 00000120: 7374 6f6d 697a 6564 2047 5549 270d 0a4c  stomized GUI'..L
 00000130: 4f4e 475f 4445 5343 5249 5054 494f 4e20  ONG_DESCRIPTION 
 00000140: 3d20 2741 2070 6163 6b61 6765 2074 6861  = 'A package tha
 00000150: 7420 616c 6c6f 7773 2079 6f75 2074 6f20  t allows you to 
 00000160: 7573 6520 7374 796c 6573 2061 6e64 2077  use styles and w
 00000170: 6964 6765 7420 6f66 2073 7570 6572 206c  idget of super l
```

