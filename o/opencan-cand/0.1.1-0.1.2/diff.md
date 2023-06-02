# Comparing `tmp/opencan-cand-0.1.1.tar.gz` & `tmp/opencan-cand-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencan-cand-0.1.1.tar", last modified: Mon May 29 16:16:54 2023, max compression
+gzip compressed data, was "opencan-cand-0.1.2.tar", last modified: Fri Jun  2 20:25:45 2023, max compression
```

## Comparing `opencan-cand-0.1.1.tar` & `opencan-cand-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 dmezh      (501) staff       (20)        0 2023-05-29 16:16:54.473917 opencan-cand-0.1.1/
--rw-r--r--   0 dmezh      (501) staff       (20)    16725 2022-11-07 05:40:35.000000 opencan-cand-0.1.1/LICENSE
--rw-r--r--   0 dmezh      (501) staff       (20)     1585 2023-05-29 16:16:54.473801 opencan-cand-0.1.1/PKG-INFO
--rw-r--r--   0 dmezh      (501) staff       (20)     1216 2022-09-20 08:07:41.000000 opencan-cand-0.1.1/README.md
-drwxr-xr-x   0 dmezh      (501) staff       (20)        0 2023-05-29 16:16:54.472912 opencan-cand-0.1.1/cand/
--rw-r--r--   0 dmezh      (501) staff       (20)      133 2022-09-20 08:16:39.000000 opencan-cand-0.1.1/cand/__init__.py
--rwxr-xr-x   0 dmezh      (501) staff       (20)     3482 2022-09-20 08:16:39.000000 opencan-cand-0.1.1/cand/cand
--rw-r--r--   0 dmezh      (501) staff       (20)     1760 2022-09-20 08:16:39.000000 opencan-cand-0.1.1/cand/client.py
--rw-r--r--   0 dmezh      (501) staff       (20)      209 2022-09-20 08:16:39.000000 opencan-cand-0.1.1/cand/config.py
--rw-r--r--   0 dmezh      (501) staff       (20)     1889 2023-02-04 01:12:19.000000 opencan-cand-0.1.1/cand/listener.py
--rw-r--r--   0 dmezh      (501) staff       (20)      751 2022-09-20 08:16:39.000000 opencan-cand-0.1.1/cand/serialization.py
--rw-r--r--   0 dmezh      (501) staff       (20)     2403 2023-05-29 16:15:35.000000 opencan-cand-0.1.1/cand/talker.py
--rw-r--r--   0 dmezh      (501) staff       (20)      387 2022-09-20 08:16:39.000000 opencan-cand-0.1.1/cand/util.py
-drwxr-xr-x   0 dmezh      (501) staff       (20)        0 2023-05-29 16:16:54.473438 opencan-cand-0.1.1/opencan_cand.egg-info/
--rw-r--r--   0 dmezh      (501) staff       (20)     1585 2023-05-29 16:16:54.000000 opencan-cand-0.1.1/opencan_cand.egg-info/PKG-INFO
--rw-r--r--   0 dmezh      (501) staff       (20)      367 2023-05-29 16:16:54.000000 opencan-cand-0.1.1/opencan_cand.egg-info/SOURCES.txt
--rw-r--r--   0 dmezh      (501) staff       (20)        1 2023-05-29 16:16:54.000000 opencan-cand-0.1.1/opencan_cand.egg-info/dependency_links.txt
--rw-r--r--   0 dmezh      (501) staff       (20)       83 2023-05-29 16:16:54.000000 opencan-cand-0.1.1/opencan_cand.egg-info/requires.txt
--rw-r--r--   0 dmezh      (501) staff       (20)        5 2023-05-29 16:16:54.000000 opencan-cand-0.1.1/opencan_cand.egg-info/top_level.txt
--rw-r--r--   0 dmezh      (501) staff       (20)      611 2023-05-29 16:15:35.000000 opencan-cand-0.1.1/pyproject.toml
--rw-r--r--   0 dmezh      (501) staff       (20)       38 2023-05-29 16:16:54.473949 opencan-cand-0.1.1/setup.cfg
--rwxr-xr-x   0 dmezh      (501) staff       (20)      107 2022-09-20 18:17:54.000000 opencan-cand-0.1.1/setup.py
-drwxr-xr-x   0 dmezh      (501) staff       (20)        0 2023-05-29 16:16:54.473533 opencan-cand-0.1.1/test/
--rw-r--r--   0 dmezh      (501) staff       (20)      533 2022-09-20 08:10:52.000000 opencan-cand-0.1.1/test/test_send_rate.py
+drwxr-xr-x   0 dmezh      (501) staff       (20)        0 2023-06-02 20:25:45.263607 opencan-cand-0.1.2/
+-rw-r--r--   0 dmezh      (501) staff       (20)    16725 2022-11-07 05:40:35.000000 opencan-cand-0.1.2/LICENSE
+-rw-r--r--   0 dmezh      (501) staff       (20)     1585 2023-06-02 20:25:45.263457 opencan-cand-0.1.2/PKG-INFO
+-rw-r--r--   0 dmezh      (501) staff       (20)     1216 2022-09-20 08:07:41.000000 opencan-cand-0.1.2/README.md
+drwxr-xr-x   0 dmezh      (501) staff       (20)        0 2023-06-02 20:25:45.261973 opencan-cand-0.1.2/cand/
+-rw-r--r--   0 dmezh      (501) staff       (20)      133 2022-09-20 08:16:39.000000 opencan-cand-0.1.2/cand/__init__.py
+-rwxr-xr-x   0 dmezh      (501) staff       (20)     3618 2023-06-02 20:24:58.000000 opencan-cand-0.1.2/cand/cand
+-rw-r--r--   0 dmezh      (501) staff       (20)     2178 2023-06-02 20:24:42.000000 opencan-cand-0.1.2/cand/client.py
+-rw-r--r--   0 dmezh      (501) staff       (20)      209 2022-09-20 08:16:39.000000 opencan-cand-0.1.2/cand/config.py
+-rw-r--r--   0 dmezh      (501) staff       (20)     1889 2023-02-04 01:12:19.000000 opencan-cand-0.1.2/cand/listener.py
+-rw-r--r--   0 dmezh      (501) staff       (20)      751 2022-09-20 08:16:39.000000 opencan-cand-0.1.2/cand/serialization.py
+-rw-r--r--   0 dmezh      (501) staff       (20)     2403 2023-05-29 16:15:35.000000 opencan-cand-0.1.2/cand/talker.py
+-rw-r--r--   0 dmezh      (501) staff       (20)      387 2022-09-20 08:16:39.000000 opencan-cand-0.1.2/cand/util.py
+drwxr-xr-x   0 dmezh      (501) staff       (20)        0 2023-06-02 20:25:45.262987 opencan-cand-0.1.2/opencan_cand.egg-info/
+-rw-r--r--   0 dmezh      (501) staff       (20)     1585 2023-06-02 20:25:45.000000 opencan-cand-0.1.2/opencan_cand.egg-info/PKG-INFO
+-rw-r--r--   0 dmezh      (501) staff       (20)      367 2023-06-02 20:25:45.000000 opencan-cand-0.1.2/opencan_cand.egg-info/SOURCES.txt
+-rw-r--r--   0 dmezh      (501) staff       (20)        1 2023-06-02 20:25:45.000000 opencan-cand-0.1.2/opencan_cand.egg-info/dependency_links.txt
+-rw-r--r--   0 dmezh      (501) staff       (20)       83 2023-06-02 20:25:45.000000 opencan-cand-0.1.2/opencan_cand.egg-info/requires.txt
+-rw-r--r--   0 dmezh      (501) staff       (20)        5 2023-06-02 20:25:45.000000 opencan-cand-0.1.2/opencan_cand.egg-info/top_level.txt
+-rw-r--r--   0 dmezh      (501) staff       (20)      611 2023-06-02 20:25:17.000000 opencan-cand-0.1.2/pyproject.toml
+-rw-r--r--   0 dmezh      (501) staff       (20)       38 2023-06-02 20:25:45.263660 opencan-cand-0.1.2/setup.cfg
+-rwxr-xr-x   0 dmezh      (501) staff       (20)      107 2022-09-20 18:17:54.000000 opencan-cand-0.1.2/setup.py
+drwxr-xr-x   0 dmezh      (501) staff       (20)        0 2023-06-02 20:25:45.263115 opencan-cand-0.1.2/test/
+-rw-r--r--   0 dmezh      (501) staff       (20)      533 2022-09-20 08:10:52.000000 opencan-cand-0.1.2/test/test_send_rate.py
```

### Comparing `opencan-cand-0.1.1/LICENSE` & `opencan-cand-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `opencan-cand-0.1.1/PKG-INFO` & `opencan-cand-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencan-cand
-Version: 0.1.1
+Version: 0.1.2
 Summary: A fast and super useful daemon for decoding and encoding CAN messages.
 Author-email: OpenCAN <info@opencan.org>
 License: MPL-2.0
 Project-URL: Homepage, https://github.com/opencan/cand
 Keywords: cand,can,canbus,can bus
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `opencan-cand-0.1.1/README.md` & `opencan-cand-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `opencan-cand-0.1.1/cand/cand` & `opencan-cand-0.1.2/cand/cand`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,18 @@
 
     cfg.init(_bus=_bus, _dbc=_dbc, _rdb=_rdb)
 
     # Flush Redis as the last thing before we start
     if not args.no_flush:
         _rdb.flushdb()
 
+    log.info("Populating message metadata.")
+    for msg in _dbc.messages:
+        cfg.rdb.set(f"msginfo:{msg.name}:id", msg.frame_id)
+
     # Start processes
     listen_p = mp.Process(target=listener_process)
     talk_p = mp.Process(target=talker_process)
 
     listen_p.start()
     talk_p.start()
```

### Comparing `opencan-cand-0.1.1/cand/client.py` & `opencan-cand-0.1.2/cand/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -53,14 +53,26 @@
 
     def get_time_delta(self, name: str) -> int:
         data = self.get(name)
 
         if data is not None:
             return time_ns() - data[0]
 
+    def get_message_id(self, name: str) -> int:
+        try:
+            id = self._rdb.get(f"msginfo:{name}:id")
+            if id is None:
+                self._log.debug(f"Tried to get message id for '{name}' and it was unavailable")
+                return None
+
+            return int(id)
+        except Exception as e:
+            self._log.error(f"Error getting message id for {name}: {e}")
+            raise e
+
     def send(self, name: str, data: dict) -> None:
         try:
             data = serialize((name, data))
 
             self._rdb.rpush("queue:cansend", data)
 
         except Exception as e:
```

### Comparing `opencan-cand-0.1.1/cand/listener.py` & `opencan-cand-0.1.2/cand/listener.py`

 * *Files identical despite different names*

### Comparing `opencan-cand-0.1.1/cand/serialization.py` & `opencan-cand-0.1.2/cand/serialization.py`

 * *Files identical despite different names*

### Comparing `opencan-cand-0.1.1/cand/talker.py` & `opencan-cand-0.1.2/cand/talker.py`

 * *Files identical despite different names*

### Comparing `opencan-cand-0.1.1/opencan_cand.egg-info/PKG-INFO` & `opencan-cand-0.1.2/opencan_cand.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencan-cand
-Version: 0.1.1
+Version: 0.1.2
 Summary: A fast and super useful daemon for decoding and encoding CAN messages.
 Author-email: OpenCAN <info@opencan.org>
 License: MPL-2.0
 Project-URL: Homepage, https://github.com/opencan/cand
 Keywords: cand,can,canbus,can bus
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `opencan-cand-0.1.1/pyproject.toml` & `opencan-cand-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "opencan-cand"
-version = "0.1.1"
+version = "0.1.2"
 description = "A fast and super useful daemon for decoding and encoding CAN messages."
 authors = [
     {name = "OpenCAN", email = "info@opencan.org"},
 ]
 
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `opencan-cand-0.1.1/test/test_send_rate.py` & `opencan-cand-0.1.2/test/test_send_rate.py`

 * *Files identical despite different names*

