# Comparing `tmp/yeref-0.1.75.tar.gz` & `tmp/yeref-0.1.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.75.tar", last modified: Fri Jun  2 13:45:23 2023, max compression
+gzip compressed data, was "yeref-0.1.76.tar", last modified: Fri Jun  2 15:56:25 2023, max compression
```

## Comparing `yeref-0.1.75.tar` & `yeref-0.1.76.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-02 13:45:23.140634 yeref-0.1.75/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-02 13:45:23.140894 yeref-0.1.75/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-02 13:45:23.141853 yeref-0.1.75/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-02 13:35:58.000000 yeref-0.1.75/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-02 13:45:23.132649 yeref-0.1.75/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.75/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   495651 2023-06-02 13:35:03.000000 yeref-0.1.75/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   208414 2023-06-02 10:26:58.000000 yeref-0.1.75/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-02 13:45:23.139942 yeref-0.1.75/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-02 13:45:23.000000 yeref-0.1.75/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-02 13:45:23.000000 yeref-0.1.75/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-02 13:45:23.000000 yeref-0.1.75/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-02 13:45:23.000000 yeref-0.1.75/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-02 15:56:25.906054 yeref-0.1.76/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-02 15:56:25.906199 yeref-0.1.76/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-02 15:56:25.906786 yeref-0.1.76/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-02 15:56:03.000000 yeref-0.1.76/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-02 15:56:25.898257 yeref-0.1.76/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.76/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   497116 2023-06-02 15:47:41.000000 yeref-0.1.76/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   208414 2023-06-02 10:26:58.000000 yeref-0.1.76/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-02 15:56:25.905672 yeref-0.1.76/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-02 15:56:25.000000 yeref-0.1.76/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-02 15:56:25.000000 yeref-0.1.76/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-02 15:56:25.000000 yeref-0.1.76/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-02 15:56:25.000000 yeref-0.1.76/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.75/setup.py` & `yeref-0.1.76/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.75',
+      version='0.1.76',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
```

### Comparing `yeref-0.1.75/yeref/l_.py` & `yeref-0.1.76/yeref/l_.py`

 * *Files 2% similar despite different names*

```diff
@@ -7308,9 +7308,74 @@
     'en': ': dice',
     'es': 'Save',
     'fr': 'Save',
     'zh': 'Save',
     'ar': 'Save',
 }
 
+
+l_check_box_pin_message = {
+    'ru': 'Закреп сообщения',
+    'en': 'Pin message',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_check_box_protect_message = {
+    'ru': 'Защита сообщения',
+    'en': 'Protect message',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_check_box_edit_message = {
+    'ru': 'Изменить текущее сообщение',
+    'en': 'Edit current message',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_check_box_auto_format = {
+    'ru': 'Авто формат сообщения',
+    'en': 'Auto format message',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_check_box_auto_typing = {
+    'ru': 'Авто печатание сообщения',
+    'en': 'Auto typing message',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_check_box_preview = {
+    'ru': 'Превью контент',
+    'en': 'Preview content',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_check_box_spoiler = {
+    'ru': 'Гиф/фото/видео спойлер',
+    'en': 'Gif/photo/video spoiler',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
+l_check_box_silence = {
+    'ru': 'Тихое сообщение',
+    'en': 'Silent message',
+    'es': 'Save',
+    'fr': 'Save',
+    'zh': 'Save',
+    'ar': 'Save',
+}
 # endregion
 # endregion
```

### Comparing `yeref-0.1.75/yeref/yeref.py` & `yeref-0.1.76/yeref/yeref.py`

 * *Files identical despite different names*

