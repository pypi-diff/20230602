# Comparing `tmp/baozun_winrobot-0.0.4.tar.gz` & `tmp/baozun_winrobot-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/baozun_winrobot-0.0.4.tar", last modified: Fri Jun  2 05:46:26 2023, max compression
+gzip compressed data, was "dist/baozun_winrobot-0.0.5.tar", last modified: Fri Jun  2 05:49:20 2023, max compression
```

## Comparing `baozun_winrobot-0.0.4.tar` & `baozun_winrobot-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 wcgz-dz-100285   (501) staff       (20)        0 2023-06-02 05:46:26.185025 baozun_winrobot-0.0.4/
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)       81 2023-06-02 05:46:26.184697 baozun_winrobot-0.0.4/PKG-INFO
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)       11 2023-06-01 10:21:00.000000 baozun_winrobot-0.0.4/README.md
-drwxr-xr-x   0 wcgz-dz-100285   (501) staff       (20)        0 2023-06-02 05:46:26.182418 baozun_winrobot-0.0.4/baozun_winrobot.egg-info/
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)       81 2023-06-02 05:46:26.000000 baozun_winrobot-0.0.4/baozun_winrobot.egg-info/PKG-INFO
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)      303 2023-06-02 05:46:26.000000 baozun_winrobot-0.0.4/baozun_winrobot.egg-info/SOURCES.txt
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)        1 2023-06-02 05:46:26.000000 baozun_winrobot-0.0.4/baozun_winrobot.egg-info/dependency_links.txt
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)        1 2023-06-02 05:46:26.000000 baozun_winrobot-0.0.4/baozun_winrobot.egg-info/not-zip-safe
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)        9 2023-06-02 05:46:26.000000 baozun_winrobot-0.0.4/baozun_winrobot.egg-info/top_level.txt
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)       38 2023-06-02 05:46:26.185141 baozun_winrobot-0.0.4/setup.cfg
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)      283 2023-06-02 05:46:08.000000 baozun_winrobot-0.0.4/setup.py
-drwxr-xr-x   0 wcgz-dz-100285   (501) staff       (20)        0 2023-06-02 05:46:26.183107 baozun_winrobot-0.0.4/winrobot/
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)        0 2023-06-02 03:31:30.000000 baozun_winrobot-0.0.4/winrobot/__init__.py
-drwxr-xr-x   0 wcgz-dz-100285   (501) staff       (20)        0 2023-06-02 05:46:26.183827 baozun_winrobot-0.0.4/winrobot/config/
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)        0 2023-06-02 05:45:29.000000 baozun_winrobot-0.0.4/winrobot/config/__init__.py
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)      694 2023-06-01 07:49:58.000000 baozun_winrobot-0.0.4/winrobot/config/tmall.py
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)      647 2023-06-02 05:45:40.000000 baozun_winrobot-0.0.4/winrobot/main.py
+drwxr-xr-x   0 wcgz-dz-100285   (501) staff       (20)        0 2023-06-02 05:49:20.077270 baozun_winrobot-0.0.5/
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)       81 2023-06-02 05:49:20.076893 baozun_winrobot-0.0.5/PKG-INFO
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)       11 2023-06-01 10:21:00.000000 baozun_winrobot-0.0.5/README.md
+drwxr-xr-x   0 wcgz-dz-100285   (501) staff       (20)        0 2023-06-02 05:49:20.074188 baozun_winrobot-0.0.5/baozun_winrobot.egg-info/
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)       81 2023-06-02 05:49:19.000000 baozun_winrobot-0.0.5/baozun_winrobot.egg-info/PKG-INFO
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)      303 2023-06-02 05:49:19.000000 baozun_winrobot-0.0.5/baozun_winrobot.egg-info/SOURCES.txt
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)        1 2023-06-02 05:49:19.000000 baozun_winrobot-0.0.5/baozun_winrobot.egg-info/dependency_links.txt
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)        1 2023-06-02 05:49:19.000000 baozun_winrobot-0.0.5/baozun_winrobot.egg-info/not-zip-safe
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)        9 2023-06-02 05:49:19.000000 baozun_winrobot-0.0.5/baozun_winrobot.egg-info/top_level.txt
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)       38 2023-06-02 05:49:20.077404 baozun_winrobot-0.0.5/setup.cfg
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)      283 2023-06-02 05:49:17.000000 baozun_winrobot-0.0.5/setup.py
+drwxr-xr-x   0 wcgz-dz-100285   (501) staff       (20)        0 2023-06-02 05:49:20.074798 baozun_winrobot-0.0.5/winrobot/
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)        0 2023-06-02 03:31:30.000000 baozun_winrobot-0.0.5/winrobot/__init__.py
+drwxr-xr-x   0 wcgz-dz-100285   (501) staff       (20)        0 2023-06-02 05:49:20.075794 baozun_winrobot-0.0.5/winrobot/config/
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)        0 2023-06-02 05:45:29.000000 baozun_winrobot-0.0.5/winrobot/config/__init__.py
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)      694 2023-06-01 07:49:58.000000 baozun_winrobot-0.0.5/winrobot/config/tmall.py
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)      656 2023-06-02 05:48:58.000000 baozun_winrobot-0.0.5/winrobot/main.py
```

### Comparing `baozun_winrobot-0.0.4/winrobot/config/tmall.py` & `baozun_winrobot-0.0.5/winrobot/config/tmall.py`

 * *Files identical despite different names*

### Comparing `baozun_winrobot-0.0.4/winrobot/main.py` & `baozun_winrobot-0.0.5/winrobot/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging; logging.basicConfig(level=logging.INFO)
 import requests;
 from requests.cookies import RequestsCookieJar;
-from config.tmall import TMALL_DEFAULT_HEADERS;
+from winrobot.config.tmall import TMALL_DEFAULT_HEADERS;
 
 def get_coupon_info(cookie_list = []):
   url = "https://shell.mkt.taobao.com/coupon/getActivityInfo"
   payload = "{\"id\":\"5907348532\",\"queryDetail\":\"true\",\"couponType\":\"0\"}"
   cookie_jar = RequestsCookieJar()
   for cookie_item in cookie_list:
     cookie_jar.set(cookie_item['name'], cookie_item['value'], domain=cookie_item['domain'])
```

