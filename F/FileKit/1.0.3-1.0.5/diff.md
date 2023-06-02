# Comparing `tmp/FileKit-1.0.3.tar.gz` & `tmp/FileKit-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FileKit-1.0.3.tar", last modified: Thu Jun  1 14:39:33 2023, max compression
+gzip compressed data, was "FileKit-1.0.5.tar", last modified: Fri Jun  2 08:26:55 2023, max compression
```

## Comparing `FileKit-1.0.3.tar` & `FileKit-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 14:39:33.237682 FileKit-1.0.3/
-drwxrwxrwx   0        0        0        0 2023-06-01 14:39:33.230702 FileKit-1.0.3/FileKit/
--rw-rw-rw-   0        0        0     1280 2023-06-01 13:44:42.000000 FileKit-1.0.3/FileKit/File.py
--rw-rw-rw-   0        0        0       24 2023-06-01 11:55:48.000000 FileKit-1.0.3/FileKit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 14:39:33.235688 FileKit-1.0.3/FileKit.egg-info/
--rw-rw-rw-   0        0        0      669 2023-06-01 14:39:33.000000 FileKit-1.0.3/FileKit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-06-01 14:39:33.000000 FileKit-1.0.3/FileKit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 14:39:33.000000 FileKit-1.0.3/FileKit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-01 14:39:33.000000 FileKit-1.0.3/FileKit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      669 2023-06-01 14:39:33.237682 FileKit-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      556 2023-06-01 14:32:32.000000 FileKit-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-01 14:39:33.237682 FileKit-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      415 2023-06-01 14:39:29.000000 FileKit-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 08:26:55.297110 FileKit-1.0.5/
+drwxrwxrwx   0        0        0        0 2023-06-02 08:26:55.291127 FileKit-1.0.5/FileKit/
+-rw-rw-rw-   0        0        0     1302 2023-06-02 08:25:51.000000 FileKit-1.0.5/FileKit/File.py
+-rw-rw-rw-   0        0        0       21 2023-06-02 08:25:07.000000 FileKit-1.0.5/FileKit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 08:26:55.295115 FileKit-1.0.5/FileKit.egg-info/
+-rw-rw-rw-   0        0        0      669 2023-06-02 08:26:55.000000 FileKit-1.0.5/FileKit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-06-02 08:26:55.000000 FileKit-1.0.5/FileKit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 08:26:55.000000 FileKit-1.0.5/FileKit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-02 08:26:55.000000 FileKit-1.0.5/FileKit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      669 2023-06-02 08:26:55.297110 FileKit-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      556 2023-06-01 14:32:32.000000 FileKit-1.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-02 08:26:55.297110 FileKit-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      415 2023-06-02 08:26:47.000000 FileKit-1.0.5/setup.py
```

### Comparing `FileKit-1.0.3/FileKit/File.py` & `FileKit-1.0.5/FileKit/File.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
     简易使用python的 文件读写内置模块，
     如果需要相对复杂操作请使用原生的python内置读写模块，以更可靠与高效
 """
 
 
-def read(file_name, encoding='utf-8'):
+def read(file_name, encoding='utf-8', mode='r'):
     """ 读取文本文件全部内容 """
-    file = open(file_name, mode='r', encoding=encoding)
+    file = open(file_name, mode=mode, encoding=encoding)
     text = file.read()
     file.close()
     return text
 
 
-def write(file_name, text, encoding='utf-8'):
+def write(file_name, text, encoding='utf-8', mode='w'):
     """  覆盖模式写入文本文件内容， 如果文件不存在会新建 """
-    file = open(file_name, mode='w', encoding=encoding)
+    file = open(file_name, mode=mode, encoding=encoding)
     file.write(text)
     file.close()
 
 
 def read_lines(file_name, encoding='utf-8'):
     """  读取文件为数组 """
     file = open(file_name, mode='r', encoding=encoding)
```

### Comparing `FileKit-1.0.3/FileKit.egg-info/PKG-INFO` & `FileKit-1.0.5/FileKit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FileKit
-Version: 1.0.3
+Version: 1.0.5
 Author: 孙亮
 Description-Content-Type: text/markdown
 
 # Filekit
 
 简易使用 Python 的文件读写内置模块，针对单词读写操作。省去 open 和 close。
```

### Comparing `FileKit-1.0.3/PKG-INFO` & `FileKit-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FileKit
-Version: 1.0.3
+Version: 1.0.5
 Author: 孙亮
 Description-Content-Type: text/markdown
 
 # Filekit
 
 简易使用 Python 的文件读写内置模块，针对单词读写操作。省去 open 和 close。
```

### Comparing `FileKit-1.0.3/README.md` & `FileKit-1.0.5/README.md`

 * *Files identical despite different names*

