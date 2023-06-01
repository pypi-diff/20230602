# Comparing `tmp/hydrobotdbc-0.0.8.tar.gz` & `tmp/hydrobotdbc-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrobotdbc-0.0.8.tar", last modified: Sun Mar 12 21:05:36 2023, max compression
+gzip compressed data, was "hydrobotdbc-0.0.9.tar", last modified: Sun Mar 12 21:24:32 2023, max compression
```

## Comparing `hydrobotdbc-0.0.8.tar` & `hydrobotdbc-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 21:05:36.312189 hydrobotdbc-0.0.8/
--rw-r--r--   0 root         (0) root         (0)      386 2023-03-12 21:05:36.312189 hydrobotdbc-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      197 2023-03-12 19:24:23.000000 hydrobotdbc-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 21:05:36.302189 hydrobotdbc-0.0.8/hydrobotdbc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-12 19:24:23.000000 hydrobotdbc-0.0.8/hydrobotdbc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3217 2023-03-12 19:24:23.000000 hydrobotdbc-0.0.8/hydrobotdbc/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 21:05:36.312189 hydrobotdbc-0.0.8/hydrobotdbc/models/
--rw-r--r--   0 root         (0) root         (0)      278 2023-03-12 19:24:23.000000 hydrobotdbc-0.0.8/hydrobotdbc/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      302 2023-03-12 19:24:23.000000 hydrobotdbc-0.0.8/hydrobotdbc/models/collection.py
--rw-r--r--   0 root         (0) root         (0)     1310 2023-03-12 20:54:09.000000 hydrobotdbc-0.0.8/hydrobotdbc/models/daily_claim.py
--rw-r--r--   0 root         (0) root         (0)     1506 2023-03-12 20:58:07.000000 hydrobotdbc-0.0.8/hydrobotdbc/models/poll.py
--rw-r--r--   0 root         (0) root         (0)     1887 2023-03-12 19:24:23.000000 hydrobotdbc-0.0.8/hydrobotdbc/models/user.py
--rw-r--r--   0 root         (0) root         (0)     1378 2023-03-12 19:24:23.000000 hydrobotdbc-0.0.8/hydrobotdbc/models/user_birthday.py
--rw-r--r--   0 root         (0) root         (0)     1537 2023-03-12 19:24:23.000000 hydrobotdbc-0.0.8/hydrobotdbc/models/user_session.py
--rw-r--r--   0 root         (0) root         (0)     1372 2023-03-12 19:24:23.000000 hydrobotdbc-0.0.8/hydrobotdbc/models/user_voicestate.py
--rw-r--r--   0 root         (0) root         (0)     1453 2023-03-12 19:24:23.000000 hydrobotdbc-0.0.8/hydrobotdbc/models/user_wallet.py
--rw-r--r--   0 root         (0) root         (0)     1513 2023-03-12 19:24:23.000000 hydrobotdbc-0.0.8/hydrobotdbc/models/wallet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 21:05:36.302189 hydrobotdbc-0.0.8/hydrobotdbc.egg-info/
--rw-r--r--   0 root         (0) root         (0)      386 2023-03-12 21:05:36.000000 hydrobotdbc-0.0.8/hydrobotdbc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      562 2023-03-12 21:05:36.000000 hydrobotdbc-0.0.8/hydrobotdbc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-12 21:05:36.000000 hydrobotdbc-0.0.8/hydrobotdbc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-03-12 21:05:36.000000 hydrobotdbc-0.0.8/hydrobotdbc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-03-12 21:05:36.000000 hydrobotdbc-0.0.8/hydrobotdbc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-12 21:05:36.312189 hydrobotdbc-0.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      510 2023-03-12 21:05:04.000000 hydrobotdbc-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 21:24:32.762176 hydrobotdbc-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)      386 2023-03-12 21:24:32.762176 hydrobotdbc-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      197 2023-03-12 19:24:23.000000 hydrobotdbc-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 21:24:32.752176 hydrobotdbc-0.0.9/hydrobotdbc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-12 19:24:23.000000 hydrobotdbc-0.0.9/hydrobotdbc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3217 2023-03-12 19:24:23.000000 hydrobotdbc-0.0.9/hydrobotdbc/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 21:24:32.762176 hydrobotdbc-0.0.9/hydrobotdbc/models/
+-rw-r--r--   0 root         (0) root         (0)      301 2023-03-12 21:23:32.000000 hydrobotdbc-0.0.9/hydrobotdbc/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      302 2023-03-12 19:24:23.000000 hydrobotdbc-0.0.9/hydrobotdbc/models/collection.py
+-rw-r--r--   0 root         (0) root         (0)     1310 2023-03-12 20:54:09.000000 hydrobotdbc-0.0.9/hydrobotdbc/models/daily_claim.py
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-03-12 20:58:07.000000 hydrobotdbc-0.0.9/hydrobotdbc/models/poll.py
+-rw-r--r--   0 root         (0) root         (0)     1887 2023-03-12 19:24:23.000000 hydrobotdbc-0.0.9/hydrobotdbc/models/user.py
+-rw-r--r--   0 root         (0) root         (0)     1378 2023-03-12 19:24:23.000000 hydrobotdbc-0.0.9/hydrobotdbc/models/user_birthday.py
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-03-12 19:24:23.000000 hydrobotdbc-0.0.9/hydrobotdbc/models/user_session.py
+-rw-r--r--   0 root         (0) root         (0)     1372 2023-03-12 19:24:23.000000 hydrobotdbc-0.0.9/hydrobotdbc/models/user_voicestate.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2023-03-12 19:24:23.000000 hydrobotdbc-0.0.9/hydrobotdbc/models/user_wallet.py
+-rw-r--r--   0 root         (0) root         (0)     1513 2023-03-12 19:24:23.000000 hydrobotdbc-0.0.9/hydrobotdbc/models/wallet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 21:24:32.762176 hydrobotdbc-0.0.9/hydrobotdbc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      386 2023-03-12 21:24:32.000000 hydrobotdbc-0.0.9/hydrobotdbc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      562 2023-03-12 21:24:32.000000 hydrobotdbc-0.0.9/hydrobotdbc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-12 21:24:32.000000 hydrobotdbc-0.0.9/hydrobotdbc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-03-12 21:24:32.000000 hydrobotdbc-0.0.9/hydrobotdbc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-03-12 21:24:32.000000 hydrobotdbc-0.0.9/hydrobotdbc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-03-12 21:24:32.762176 hydrobotdbc-0.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      510 2023-03-12 21:23:47.000000 hydrobotdbc-0.0.9/setup.py
```

### Comparing `hydrobotdbc-0.0.8/hydrobotdbc/client.py` & `hydrobotdbc-0.0.9/hydrobotdbc/client.py`

 * *Files identical despite different names*

### Comparing `hydrobotdbc-0.0.8/hydrobotdbc/models/daily_claim.py` & `hydrobotdbc-0.0.9/hydrobotdbc/models/daily_claim.py`

 * *Files identical despite different names*

### Comparing `hydrobotdbc-0.0.8/hydrobotdbc/models/poll.py` & `hydrobotdbc-0.0.9/hydrobotdbc/models/poll.py`

 * *Files identical despite different names*

### Comparing `hydrobotdbc-0.0.8/hydrobotdbc/models/user.py` & `hydrobotdbc-0.0.9/hydrobotdbc/models/user.py`

 * *Files identical despite different names*

### Comparing `hydrobotdbc-0.0.8/hydrobotdbc/models/user_birthday.py` & `hydrobotdbc-0.0.9/hydrobotdbc/models/user_birthday.py`

 * *Files identical despite different names*

### Comparing `hydrobotdbc-0.0.8/hydrobotdbc/models/user_session.py` & `hydrobotdbc-0.0.9/hydrobotdbc/models/user_session.py`

 * *Files identical despite different names*

### Comparing `hydrobotdbc-0.0.8/hydrobotdbc/models/user_voicestate.py` & `hydrobotdbc-0.0.9/hydrobotdbc/models/user_voicestate.py`

 * *Files identical despite different names*

### Comparing `hydrobotdbc-0.0.8/hydrobotdbc/models/user_wallet.py` & `hydrobotdbc-0.0.9/hydrobotdbc/models/user_wallet.py`

 * *Files identical despite different names*

### Comparing `hydrobotdbc-0.0.8/hydrobotdbc/models/wallet.py` & `hydrobotdbc-0.0.9/hydrobotdbc/models/wallet.py`

 * *Files identical despite different names*

### Comparing `hydrobotdbc-0.0.8/hydrobotdbc.egg-info/SOURCES.txt` & `hydrobotdbc-0.0.9/hydrobotdbc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

