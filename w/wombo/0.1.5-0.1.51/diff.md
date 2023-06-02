# Comparing `tmp/wombo-0.1.5.tar.gz` & `tmp/wombo-0.1.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wombo-0.1.5.tar", max compression
+gzip compressed data, was "wombo-0.1.51.tar", max compression
```

## Comparing `wombo-0.1.5.tar` & `wombo-0.1.51.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1066 2023-06-02 14:02:35.382424 wombo-0.1.5/LICENSE
--rw-r--r--   0        0        0     1335 2023-06-02 16:53:17.418424 wombo-0.1.5/README.md
--rw-r--r--   0        0        0      340 2023-06-02 16:54:17.362424 wombo-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       70 2023-06-02 14:20:19.386424 wombo-0.1.5/wombo/__init__.py
--rw-r--r--   0        0        0     4013 2023-06-02 15:51:51.722424 wombo-0.1.5/wombo/async_dream.py
--rw-r--r--   0        0        0     3421 2023-06-02 15:37:20.226424 wombo-0.1.5/wombo/dream.py
--rw-r--r--   0        0        0       93 2023-06-02 14:55:39.890424 wombo-0.1.5/wombo/models/__init__.py
--rw-r--r--   0        0        0      524 2023-06-02 15:01:24.554424 wombo-0.1.5/wombo/models/check_task.py
--rw-r--r--   0        0        0      513 2023-06-02 14:46:35.578424 wombo-0.1.5/wombo/models/create_task.py
--rw-r--r--   0        0        0     3274 2023-06-02 14:21:55.846424 wombo-0.1.5/wombo/urls.py
--rw-r--r--   0        0        0     1858 1970-01-01 00:00:00.000000 wombo-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-02 14:02:35.382424 wombo-0.1.51/LICENSE
+-rw-r--r--   0        0        0     1407 2023-06-02 16:56:22.134424 wombo-0.1.51/README.md
+-rw-r--r--   0        0        0      341 2023-06-02 16:56:27.506424 wombo-0.1.51/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-06-02 14:20:19.386424 wombo-0.1.51/wombo/__init__.py
+-rw-r--r--   0        0        0     4013 2023-06-02 15:51:51.722424 wombo-0.1.51/wombo/async_dream.py
+-rw-r--r--   0        0        0     3421 2023-06-02 15:37:20.226424 wombo-0.1.51/wombo/dream.py
+-rw-r--r--   0        0        0       93 2023-06-02 14:55:39.890424 wombo-0.1.51/wombo/models/__init__.py
+-rw-r--r--   0        0        0      524 2023-06-02 15:01:24.554424 wombo-0.1.51/wombo/models/check_task.py
+-rw-r--r--   0        0        0      513 2023-06-02 14:46:35.578424 wombo-0.1.51/wombo/models/create_task.py
+-rw-r--r--   0        0        0     3274 2023-06-02 14:21:55.846424 wombo-0.1.51/wombo/urls.py
+-rw-r--r--   0        0        0     1931 1970-01-01 00:00:00.000000 wombo-0.1.51/PKG-INFO
```

### Comparing `wombo-0.1.5/LICENSE` & `wombo-0.1.51/LICENSE`

 * *Files identical despite different names*

### Comparing `wombo-0.1.5/README.md` & `wombo-0.1.51/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 - photo_url_list Only the already generated image has. To check the image, use check_task(). Return io.BytesIO()
 ```
 gif = await dream.gif(task.photo_url_list)
 
 gif = await dream.gif(task.photo_url_list, thread=False)
 # Used if you don't want to use an asynchronous thread.
 # to generate a gif, it is true since the generation is quite long
+# Generation in the thread is not available for the synchronous library
 ```
 
 
 <h2>requirements</h2>
 
 - [httpx](https://pypi.org/project/httpx/)
 - [pillow](https://pypi.org/project/Pillow/)
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_cuwb0rpb_/tmpsl18kls__TarContainer/0/1.md", line 45, column 0: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_cuwb0rpb_/tmpsl18kls__TarContainer/0/1.md", line 45, column 0: Levels of opening and closing headings don't match*

```diff
@@ -8,10 +8,11 @@
 ``` task = await dream.check_task(task.id) # To get information about readiness
      in bool format task = await dream.check_task(task.id, False) # To get
    information about readiness ``` #### Create gif - photo_url_list Only the
    already generated image has. To check the image, use check_task(). Return
     io.BytesIO() ``` gif = await dream.gif(task.photo_url_list) gif = await
 dream.gif(task.photo_url_list, thread=False) # Used if you don't want to use an
  asynchronous thread. # to generate a gif, it is true since the generation is
-                       quite long ```requirements ******
+  quite long # Generation in the thread is not available for the synchronous
+                        library ```requirements ******
 - [httpx](https://pypi.org/project/httpx/) - [pillow](https://pypi.org/project/
 Pillow/) - [pydantic](https://pypi.org/project/pydantic/)
```

### Comparing `wombo-0.1.5/wombo/async_dream.py` & `wombo-0.1.51/wombo/async_dream.py`

 * *Files identical despite different names*

### Comparing `wombo-0.1.5/wombo/dream.py` & `wombo-0.1.51/wombo/dream.py`

 * *Files identical despite different names*

### Comparing `wombo-0.1.5/wombo/models/check_task.py` & `wombo-0.1.51/wombo/models/check_task.py`

 * *Files identical despite different names*

### Comparing `wombo-0.1.5/wombo/models/create_task.py` & `wombo-0.1.51/wombo/models/create_task.py`

 * *Files identical despite different names*

### Comparing `wombo-0.1.5/wombo/urls.py` & `wombo-0.1.51/wombo/urls.py`

 * *Files identical despite different names*

### Comparing `wombo-0.1.5/PKG-INFO` & `wombo-0.1.51/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wombo
-Version: 0.1.5
+Version: 0.1.51
 Summary: Dream api
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -47,14 +47,15 @@
 - photo_url_list Only the already generated image has. To check the image, use check_task(). Return io.BytesIO()
 ```
 gif = await dream.gif(task.photo_url_list)
 
 gif = await dream.gif(task.photo_url_list, thread=False)
 # Used if you don't want to use an asynchronous thread.
 # to generate a gif, it is true since the generation is quite long
+# Generation in the thread is not available for the synchronous library
 ```
 
 
 <h2>requirements</h2>
 
 - [httpx](https://pypi.org/project/httpx/)
 - [pillow](https://pypi.org/project/Pillow/)
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_cuwb0rpb_/tmpsl18kls__TarContainer/0/10", line 63, column 0: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_cuwb0rpb_/tmpsl18kls__TarContainer/0/10", line 63, column 0: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wombo Version: 0.1.5 Summary: Dream api License:
+Metadata-Version: 2.1 Name: wombo Version: 0.1.51 Summary: Dream api License:
 MIT Author: Your Name Author-email: you@example.com Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: httpx
 (>=0.24.1,<0.25.0) Requires-Dist: pillow (>=9.5.0,<10.0.0) Requires-Dist:
 pydantic (>=1.10.8,<2.0.0) Description-Content-Type: text/markdown
  ****** Hi there, I'm Wombo ### I am a module for using wombo dream ai (neural
@@ -15,10 +15,11 @@
 ``` task = await dream.check_task(task.id) # To get information about readiness
      in bool format task = await dream.check_task(task.id, False) # To get
    information about readiness ``` #### Create gif - photo_url_list Only the
    already generated image has. To check the image, use check_task(). Return
     io.BytesIO() ``` gif = await dream.gif(task.photo_url_list) gif = await
 dream.gif(task.photo_url_list, thread=False) # Used if you don't want to use an
  asynchronous thread. # to generate a gif, it is true since the generation is
-                       quite long ```requirements ******
+  quite long # Generation in the thread is not available for the synchronous
+                        library ```requirements ******
 - [httpx](https://pypi.org/project/httpx/) - [pillow](https://pypi.org/project/
 Pillow/) - [pydantic](https://pypi.org/project/pydantic/)
```

