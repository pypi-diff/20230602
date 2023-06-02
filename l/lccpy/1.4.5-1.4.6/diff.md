# Comparing `tmp/lccpy-1.4.5.tar.gz` & `tmp/lccpy-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lccpy-1.4.5.tar", last modified: Sat Apr 22 15:47:55 2023, max compression
+gzip compressed data, was "lccpy-1.4.6.tar", last modified: Fri Jun  2 15:20:18 2023, max compression
```

## Comparing `lccpy-1.4.5.tar` & `lccpy-1.4.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 lccpy-1.4.5/LICENSE
--rw-r--r--   0        0        0      119 2023-04-10 04:12:12.772589 lccpy-1.4.5/README.md
--rw-r--r--   0        0        0        0 2023-04-10 03:05:49.119798 lccpy-1.4.5/lccpy/__init__.py
--rw-r--r--   0        0        0      143 2023-04-11 02:41:01.880058 lccpy-1.4.5/lccpy/_mtype.py
--rw-r--r--   0        0        0    11357 2022-10-25 20:46:40.000000 lccpy-1.4.5/lccpy/asymongo/Licenses of dependent packages/motor/LICENSE
--rw-r--r--   0        0        0      168 2023-04-10 03:51:03.558895 lccpy-1.4.5/lccpy/asymongo/__init__.py
--rw-r--r--   0        0        0    20512 2023-04-11 02:42:19.557384 lccpy-1.4.5/lccpy/asymongo/_asymongo.py
--rw-r--r--   0        0        0     1070 2022-05-08 19:03:55.000000 lccpy-1.4.5/lccpy/asymysql/Licenses of dependent packages/aiomysql/LICENSE
--rw-r--r--   0        0        0       89 2023-04-10 03:50:24.852505 lccpy-1.4.5/lccpy/asymysql/__init__.py
--rw-r--r--   0        0        0    22806 2023-04-19 04:50:36.901729 lccpy-1.4.5/lccpy/asymysql/_asymysql.py
--rw-r--r--   0        0        0      273 2023-04-09 17:36:47.380717 lccpy-1.4.5/lccpy/coolfunc/__init__.py
--rw-r--r--   0        0        0     2787 2023-04-10 03:18:54.132549 lccpy-1.4.5/lccpy/coolfunc/_coolfunc.py
--rw-r--r--   0        0        0    11357 2022-11-17 21:35:25.000000 lccpy-1.4.5/lccpy/coolmongo/Licenses of dependent packages/pymongo/LICENSE
--rw-r--r--   0        0        0      169 2023-04-10 03:53:42.961556 lccpy-1.4.5/lccpy/coolmongo/__init__.py
--rw-r--r--   0        0        0    20930 2023-04-11 02:42:37.661736 lccpy-1.4.5/lccpy/coolmongo/_coolmongo.py
--rw-r--r--   0        0        0     1070 2013-11-27 14:43:24.000000 lccpy-1.4.5/lccpy/coolmysql/Licenses of dependent packages/pymysql/LICENSE
--rw-r--r--   0        0        0       90 2023-04-10 03:53:46.616102 lccpy-1.4.5/lccpy/coolmysql/__init__.py
--rw-r--r--   0        0        0    22832 2023-04-19 07:49:15.385992 lccpy-1.4.5/lccpy/coolmysql/_coolmysql.py
--rw-r--r--   0        0        0     2926 2023-01-27 23:35:02.000000 lccpy-1.4.5/lccpy/encrypt256/Licenses of dependent packages/pycryptodome/LICENSE
--rw-r--r--   0        0        0       35 2022-11-15 14:17:28.000000 lccpy-1.4.5/lccpy/encrypt256/__init__.py
--rw-r--r--   0        0        0     5141 2023-03-09 14:58:17.055833 lccpy-1.4.5/lccpy/encrypt256/_encrypt256.py
--rw-r--r--   0        0        0       35 2023-04-07 08:40:27.218236 lccpy-1.4.5/lccpy/increment/__init__.py
--rw-r--r--   0        0        0     1544 2023-04-12 06:50:22.634385 lccpy-1.4.5/lccpy/increment/_increment.py
--rw-r--r--   0        0        0       32 2023-02-19 09:41:05.530766 lccpy-1.4.5/lccpy/rstyleslice/__init__.py
--rw-r--r--   0        0        0     2903 2023-03-09 15:08:02.859531 lccpy-1.4.5/lccpy/rstyleslice/_rstyleslice.py
--rw-r--r--   0        0        0      175 2023-04-09 15:53:54.291702 lccpy-1.4.5/lccpy/vtype/__init__.py
--rw-r--r--   0        0        0     3546 2023-04-09 15:28:10.501541 lccpy-1.4.5/lccpy/vtype/_cooltime.py
--rw-r--r--   0        0        0    11771 2023-04-12 12:56:02.300717 lccpy-1.4.5/lccpy/vtype/_vtype.py
--rw-r--r--   0        0        0      573 2023-04-22 15:38:43.104610 lccpy-1.4.5/pyproject.toml
--rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 lccpy-1.4.5/PKG-INFO
+-rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 lccpy-1.4.6/LICENSE
+-rw-r--r--   0        0        0      114 2023-04-30 19:30:52.062289 lccpy-1.4.6/README.md
+-rw-r--r--   0        0        0        0 2023-04-10 03:05:49.119798 lccpy-1.4.6/lccpy/__init__.py
+-rw-r--r--   0        0        0      143 2023-04-11 02:41:01.880058 lccpy-1.4.6/lccpy/_mtype.py
+-rw-r--r--   0        0        0    11357 2022-10-25 20:46:40.000000 lccpy-1.4.6/lccpy/asymongo/Licenses of dependent packages/motor/LICENSE
+-rw-r--r--   0        0        0      168 2023-04-10 03:51:03.558895 lccpy-1.4.6/lccpy/asymongo/__init__.py
+-rw-r--r--   0        0        0    20512 2023-04-11 02:42:19.557384 lccpy-1.4.6/lccpy/asymongo/_asymongo.py
+-rw-r--r--   0        0        0     1070 2022-05-08 19:03:55.000000 lccpy-1.4.6/lccpy/asymysql/Licenses of dependent packages/aiomysql/LICENSE
+-rw-r--r--   0        0        0       89 2023-04-10 03:50:24.852505 lccpy-1.4.6/lccpy/asymysql/__init__.py
+-rw-r--r--   0        0        0    22806 2023-04-19 04:50:36.901729 lccpy-1.4.6/lccpy/asymysql/_asymysql.py
+-rw-r--r--   0        0        0      273 2023-04-09 17:36:47.380717 lccpy-1.4.6/lccpy/coolfunc/__init__.py
+-rw-r--r--   0        0        0     2787 2023-04-10 03:18:54.132549 lccpy-1.4.6/lccpy/coolfunc/_coolfunc.py
+-rw-r--r--   0        0        0    11357 2022-11-17 21:35:25.000000 lccpy-1.4.6/lccpy/coolmongo/Licenses of dependent packages/pymongo/LICENSE
+-rw-r--r--   0        0        0      169 2023-04-10 03:53:42.961556 lccpy-1.4.6/lccpy/coolmongo/__init__.py
+-rw-r--r--   0        0        0    20930 2023-04-11 02:42:37.661736 lccpy-1.4.6/lccpy/coolmongo/_coolmongo.py
+-rw-r--r--   0        0        0     1070 2013-11-27 14:43:24.000000 lccpy-1.4.6/lccpy/coolmysql/Licenses of dependent packages/pymysql/LICENSE
+-rw-r--r--   0        0        0       90 2023-04-10 03:53:46.616102 lccpy-1.4.6/lccpy/coolmysql/__init__.py
+-rw-r--r--   0        0        0    22832 2023-04-19 07:49:15.385992 lccpy-1.4.6/lccpy/coolmysql/_coolmysql.py
+-rw-r--r--   0        0        0     2926 2023-01-27 23:35:02.000000 lccpy-1.4.6/lccpy/encrypt256/Licenses of dependent packages/pycryptodome/LICENSE
+-rw-r--r--   0        0        0       35 2022-11-15 14:17:28.000000 lccpy-1.4.6/lccpy/encrypt256/__init__.py
+-rw-r--r--   0        0        0     5141 2023-03-09 14:58:17.055833 lccpy-1.4.6/lccpy/encrypt256/_encrypt256.py
+-rw-r--r--   0        0        0       35 2023-04-07 08:40:27.218236 lccpy-1.4.6/lccpy/increment/__init__.py
+-rw-r--r--   0        0        0     1586 2023-06-02 08:06:48.314577 lccpy-1.4.6/lccpy/increment/_increment.py
+-rw-r--r--   0        0        0       32 2023-02-19 09:41:05.530766 lccpy-1.4.6/lccpy/rstyleslice/__init__.py
+-rw-r--r--   0        0        0     2903 2023-03-09 15:08:02.859531 lccpy-1.4.6/lccpy/rstyleslice/_rstyleslice.py
+-rw-r--r--   0        0        0      175 2023-04-09 15:53:54.291702 lccpy-1.4.6/lccpy/vtype/__init__.py
+-rw-r--r--   0        0        0     3546 2023-04-09 15:28:10.501541 lccpy-1.4.6/lccpy/vtype/_cooltime.py
+-rw-r--r--   0        0        0    11771 2023-04-12 12:56:02.300717 lccpy-1.4.6/lccpy/vtype/_vtype.py
+-rw-r--r--   0        0        0      565 2023-06-02 15:18:23.324861 lccpy-1.4.6/pyproject.toml
+-rw-r--r--   0        0        0      575 1970-01-01 00:00:00.000000 lccpy-1.4.6/PKG-INFO
```

### Comparing `lccpy-1.4.5/LICENSE` & `lccpy-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.5/lccpy/asymongo/Licenses of dependent packages/motor/LICENSE` & `lccpy-1.4.6/lccpy/asymongo/Licenses of dependent packages/motor/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.5/lccpy/asymongo/_asymongo.py` & `lccpy-1.4.6/lccpy/asymongo/_asymongo.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.5/lccpy/asymysql/Licenses of dependent packages/aiomysql/LICENSE` & `lccpy-1.4.6/lccpy/asymysql/Licenses of dependent packages/aiomysql/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.5/lccpy/asymysql/_asymysql.py` & `lccpy-1.4.6/lccpy/asymysql/_asymysql.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.5/lccpy/coolfunc/_coolfunc.py` & `lccpy-1.4.6/lccpy/coolfunc/_coolfunc.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.5/lccpy/coolmongo/Licenses of dependent packages/pymongo/LICENSE` & `lccpy-1.4.6/lccpy/coolmongo/Licenses of dependent packages/pymongo/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.5/lccpy/coolmongo/_coolmongo.py` & `lccpy-1.4.6/lccpy/coolmongo/_coolmongo.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.5/lccpy/coolmysql/Licenses of dependent packages/pymysql/LICENSE` & `lccpy-1.4.6/lccpy/coolmysql/Licenses of dependent packages/pymysql/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.5/lccpy/coolmysql/_coolmysql.py` & `lccpy-1.4.6/lccpy/coolmysql/_coolmysql.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.5/lccpy/encrypt256/Licenses of dependent packages/pycryptodome/LICENSE` & `lccpy-1.4.6/lccpy/encrypt256/Licenses of dependent packages/pycryptodome/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.5/lccpy/encrypt256/_encrypt256.py` & `lccpy-1.4.6/lccpy/encrypt256/_encrypt256.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.5/lccpy/increment/_increment.py` & `lccpy-1.4.6/lccpy/increment/_increment.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,34 +18,35 @@
         while num:
             num, i = divmod(num, LenChars)
             rn.appendleft(Characters[i])
         return ''.join(rn)
     return Characters[0]
 
 getTid = lambda : EncodeNum(int(time.time() * 1000))  # 一般毫秒后面的数值没有分辨率
-pid = EncodeNum(os.getpid())
+pid = EncodeNum(os.getpid())  # 进程ID
 
 class incrementer():
     def __init__(self, macid=None, macidSize=4):
-        self._threads = []  # 线程安全
+        self._threads = [1]  # 线程安全
         self._ContPool = deque()  # 线程安全
         self.macid = macid or ''.join(choices(Characters, k=macidSize or 1))
         self._TMP = f"{getTid()}_{self.macid}_{pid}"
 
     def _getid(self):
         try:
             cont = self._ContPool.popleft()
         except:
-            _ = []  # 随便1个可变对象即可
-            self._threads.append(_)
-            cont = [EncodeNum(self._threads.index(_)), 0]
+            class ele: ...
+            self._threads.append(ele)
+            x = EncodeNum(self._threads.index(ele))
+            cont = ['', 0] if x == '1' else [f"{x}-", 0]
         cont[1] += 1
         x, y = cont
         self._ContPool.append(cont)
-        return f"{x}_{y}"
+        return f"{x}{y}"
 
     # 使用创建进程时的时间
     def pk1(self): return f"{self._TMP}_{self._getid()}"
 
     # 使用当前时间 
     def pk2(self): return f"{getTid()}_{self.macid}_{pid}_{self._getid()}"
```

### Comparing `lccpy-1.4.5/lccpy/rstyleslice/_rstyleslice.py` & `lccpy-1.4.6/lccpy/rstyleslice/_rstyleslice.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.5/lccpy/vtype/_cooltime.py` & `lccpy-1.4.6/lccpy/vtype/_cooltime.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.5/lccpy/vtype/_vtype.py` & `lccpy-1.4.6/lccpy/vtype/_vtype.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.5/pyproject.toml` & `lccpy-1.4.6/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "lccpy"
-version = "1.4.5"
-description = "The dependent package of project <Make Python simpler> ."
+version = "1.4.6"
+description = "项目 <让 Python 更简单一点> 的依赖包"
 dependencies = ["motor", "aiomysql", "pymongo", "pymysql", "pycryptodome"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
```

### Comparing `lccpy-1.4.5/PKG-INFO` & `lccpy-1.4.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: lccpy
-Version: 1.4.5
-Summary: The dependent package of project <Make Python simpler> .
+Version: 1.4.6
+Summary: 项目 <让 Python 更简单一点> 的依赖包
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: motor
 Requires-Dist: aiomysql
 Requires-Dist: pymongo
 Requires-Dist: pymysql
 Requires-Dist: pycryptodome
 Project-URL: HomePage, https://github.com/lcctoor/lccpy#readme
 
-# Project description
+# 项目描述
 
-The dependent package of project \<[Make Python simpler](https://github.com/lcctoor/lccpy)\> .
+项目 \<[让 Python 更简单一点](https://github.com/lcctoor/lccpy#readme)\> 的依赖包。
```

