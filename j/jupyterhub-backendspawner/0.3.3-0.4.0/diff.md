# Comparing `tmp/jupyterhub-backendspawner-0.3.3.tar.gz` & `tmp/jupyterhub-backendspawner-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterhub-backendspawner-0.3.3.tar", last modified: Wed May 31 12:30:58 2023, max compression
+gzip compressed data, was "jupyterhub-backendspawner-0.4.0.tar", last modified: Fri Jun  2 13:19:34 2023, max compression
```

## Comparing `jupyterhub-backendspawner-0.3.3.tar` & `jupyterhub-backendspawner-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 12:30:58.691146 jupyterhub-backendspawner-0.3.3/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-04-24 08:18:45.000000 jupyterhub-backendspawner-0.3.3/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-05-31 12:30:58.691146 jupyterhub-backendspawner-0.3.3/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      102 2023-04-24 08:20:17.000000 jupyterhub-backendspawner-0.3.3/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 12:30:58.691146 jupyterhub-backendspawner-0.3.3/backendspawner/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.3.3/backendspawner/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5197 2023-05-31 12:29:40.000000 jupyterhub-backendspawner-0.3.3/backendspawner/api_events.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17765 2023-05-31 10:15:11.000000 jupyterhub-backendspawner-0.3.3/backendspawner/backendspawner.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10280 2023-05-31 10:13:29.000000 jupyterhub-backendspawner-0.3.3/backendspawner/eventspawner.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 12:30:58.691146 jupyterhub-backendspawner-0.3.3/jupyterhub_backendspawner.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-05-31 12:30:58.000000 jupyterhub-backendspawner-0.3.3/jupyterhub_backendspawner.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      390 2023-05-31 12:30:58.000000 jupyterhub-backendspawner-0.3.3/jupyterhub_backendspawner.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-31 12:30:58.000000 jupyterhub-backendspawner-0.3.3/jupyterhub_backendspawner.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-05-31 12:30:58.000000 jupyterhub-backendspawner-0.3.3/jupyterhub_backendspawner.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-05-31 12:30:58.000000 jupyterhub-backendspawner-0.3.3/jupyterhub_backendspawner.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-31 12:30:58.691146 jupyterhub-backendspawner-0.3.3/setup.cfg
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-05-31 12:30:14.000000 jupyterhub-backendspawner-0.3.3/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-02 13:19:34.296278 jupyterhub-backendspawner-0.4.0/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-04-24 08:18:45.000000 jupyterhub-backendspawner-0.4.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-06-02 13:19:34.296278 jupyterhub-backendspawner-0.4.0/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      102 2023-04-24 08:20:17.000000 jupyterhub-backendspawner-0.4.0/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-02 13:19:34.296278 jupyterhub-backendspawner-0.4.0/backendspawner/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.4.0/backendspawner/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5197 2023-05-31 12:29:40.000000 jupyterhub-backendspawner-0.4.0/backendspawner/api_events.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17776 2023-06-02 13:15:46.000000 jupyterhub-backendspawner-0.4.0/backendspawner/backendspawner.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10280 2023-05-31 10:13:29.000000 jupyterhub-backendspawner-0.4.0/backendspawner/eventspawner.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-02 13:19:34.296278 jupyterhub-backendspawner-0.4.0/jupyterhub_backendspawner.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-06-02 13:19:34.000000 jupyterhub-backendspawner-0.4.0/jupyterhub_backendspawner.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      390 2023-06-02 13:19:34.000000 jupyterhub-backendspawner-0.4.0/jupyterhub_backendspawner.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-02 13:19:34.000000 jupyterhub-backendspawner-0.4.0/jupyterhub_backendspawner.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-06-02 13:19:34.000000 jupyterhub-backendspawner-0.4.0/jupyterhub_backendspawner.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-06-02 13:19:34.000000 jupyterhub-backendspawner-0.4.0/jupyterhub_backendspawner.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-02 13:19:34.296278 jupyterhub-backendspawner-0.4.0/setup.cfg
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-06-02 13:16:19.000000 jupyterhub-backendspawner-0.4.0/setup.py
```

### Comparing `jupyterhub-backendspawner-0.3.3/LICENSE` & `jupyterhub-backendspawner-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.3.3/backendspawner/api_events.py` & `jupyterhub-backendspawner-0.4.0/backendspawner/api_events.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.3.3/backendspawner/backendspawner.py` & `jupyterhub-backendspawner-0.4.0/backendspawner/backendspawner.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,26 +88,27 @@
     def get_request_kwargs(self):
         if callable(self.request_kwargs):
             request_kwargs = self.request_kwargs(self)
         else:
             request_kwargs = self.request_kwargs
         return request_kwargs
 
-    port = Union(
+    custom_port = Union(
         [Integer(), Callable()],
         default_value=8080,
         help="""
         """,
     ).tag(config=True)
 
-    async def get_port(self):
-        if callable(self.port):
-            port = await maybe_future(self.port(self))
+    @default('port')
+    def get_port(self):
+        if callable(self.custom_port):
+            port = self.custom_port(self)
         else:
-            port = self.port
+            port = self.custom_port
         return port
 
     poll_interval = Union(
         [Integer(), Callable()],
         default_value=0,
         help="""
         Interval (in seconds) on which to poll the spawner for single-user server's status.
@@ -438,15 +439,15 @@
             # available again faster.
             self.already_stopped = True
             self.already_post_stop_hooked = True
 
             raise e
 
         service_address = self.get_service_address()
-        port = await self.get_port()
+        port = self.port
         self.log.debug(
             f"Expect JupyterLab at {service_address}:{port}",
             extra={
                 "uuidcode": self.name,
                 "log_name": self._log_name,
                 "user": self.user.name,
             },
```

### Comparing `jupyterhub-backendspawner-0.3.3/backendspawner/eventspawner.py` & `jupyterhub-backendspawner-0.4.0/backendspawner/eventspawner.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.3.3/setup.py` & `jupyterhub-backendspawner-0.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="jupyterhub-backendspawner",
-    version="0.3.3",
+    version="0.4.0",
     description="JupyterHub Spawner to spawn on different systems.",
     url="https://github.com/kreuzert/jupyterhub-backendspawner",
     author="Tim Kreuzer",
     author_email="t.kreuzer@fz-juelich.de",
     license="3-BSD",
     packages=find_packages(),
     install_requires=["jupyterhub","traitlets"],
```

