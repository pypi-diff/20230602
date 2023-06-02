# Comparing `tmp/baozun_winrobot-0.0.3.tar.gz` & `tmp/baozun_winrobot-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/baozun_winrobot-0.0.3.tar", last modified: Fri Jun  2 05:36:16 2023, max compression
+gzip compressed data, was "dist/baozun_winrobot-0.0.4.tar", last modified: Fri Jun  2 05:46:26 2023, max compression
```

## Comparing `baozun_winrobot-0.0.3.tar` & `baozun_winrobot-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 wcgz-dz-100285   (501) staff       (20)        0 2023-06-02 05:36:16.736966 baozun_winrobot-0.0.3/
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)       81 2023-06-02 05:36:16.736567 baozun_winrobot-0.0.3/PKG-INFO
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)       11 2023-06-01 10:21:00.000000 baozun_winrobot-0.0.3/README.md
-drwxr-xr-x   0 wcgz-dz-100285   (501) staff       (20)        0 2023-06-02 05:36:16.732885 baozun_winrobot-0.0.3/baozun_winrobot.egg-info/
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)       81 2023-06-02 05:36:16.000000 baozun_winrobot-0.0.3/baozun_winrobot.egg-info/PKG-INFO
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)      246 2023-06-02 05:36:16.000000 baozun_winrobot-0.0.3/baozun_winrobot.egg-info/SOURCES.txt
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)        1 2023-06-02 05:36:16.000000 baozun_winrobot-0.0.3/baozun_winrobot.egg-info/dependency_links.txt
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)        1 2023-06-02 05:36:16.000000 baozun_winrobot-0.0.3/baozun_winrobot.egg-info/not-zip-safe
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)        7 2023-06-02 05:36:16.000000 baozun_winrobot-0.0.3/baozun_winrobot.egg-info/top_level.txt
-drwxr-xr-x   0 wcgz-dz-100285   (501) staff       (20)        0 2023-06-02 05:36:16.735595 baozun_winrobot-0.0.3/coupon/
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)        0 2023-06-02 03:31:30.000000 baozun_winrobot-0.0.3/coupon/__init__.py
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)      645 2023-06-01 08:01:21.000000 baozun_winrobot-0.0.3/coupon/main.py
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)       38 2023-06-02 05:36:16.737088 baozun_winrobot-0.0.3/setup.cfg
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)      283 2023-06-02 03:13:32.000000 baozun_winrobot-0.0.3/setup.py
+drwxr-xr-x   0 wcgz-dz-100285   (501) staff       (20)        0 2023-06-02 05:46:26.185025 baozun_winrobot-0.0.4/
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)       81 2023-06-02 05:46:26.184697 baozun_winrobot-0.0.4/PKG-INFO
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)       11 2023-06-01 10:21:00.000000 baozun_winrobot-0.0.4/README.md
+drwxr-xr-x   0 wcgz-dz-100285   (501) staff       (20)        0 2023-06-02 05:46:26.182418 baozun_winrobot-0.0.4/baozun_winrobot.egg-info/
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)       81 2023-06-02 05:46:26.000000 baozun_winrobot-0.0.4/baozun_winrobot.egg-info/PKG-INFO
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)      303 2023-06-02 05:46:26.000000 baozun_winrobot-0.0.4/baozun_winrobot.egg-info/SOURCES.txt
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)        1 2023-06-02 05:46:26.000000 baozun_winrobot-0.0.4/baozun_winrobot.egg-info/dependency_links.txt
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)        1 2023-06-02 05:46:26.000000 baozun_winrobot-0.0.4/baozun_winrobot.egg-info/not-zip-safe
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)        9 2023-06-02 05:46:26.000000 baozun_winrobot-0.0.4/baozun_winrobot.egg-info/top_level.txt
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)       38 2023-06-02 05:46:26.185141 baozun_winrobot-0.0.4/setup.cfg
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)      283 2023-06-02 05:46:08.000000 baozun_winrobot-0.0.4/setup.py
+drwxr-xr-x   0 wcgz-dz-100285   (501) staff       (20)        0 2023-06-02 05:46:26.183107 baozun_winrobot-0.0.4/winrobot/
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)        0 2023-06-02 03:31:30.000000 baozun_winrobot-0.0.4/winrobot/__init__.py
+drwxr-xr-x   0 wcgz-dz-100285   (501) staff       (20)        0 2023-06-02 05:46:26.183827 baozun_winrobot-0.0.4/winrobot/config/
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)        0 2023-06-02 05:45:29.000000 baozun_winrobot-0.0.4/winrobot/config/__init__.py
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)      694 2023-06-01 07:49:58.000000 baozun_winrobot-0.0.4/winrobot/config/tmall.py
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)      647 2023-06-02 05:45:40.000000 baozun_winrobot-0.0.4/winrobot/main.py
```

### Comparing `baozun_winrobot-0.0.3/coupon/main.py` & `baozun_winrobot-0.0.4/winrobot/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging; logging.basicConfig(level=logging.INFO)
 import requests;
 from requests.cookies import RequestsCookieJar;
-from conf.tmall import TMALL_DEFAULT_HEADERS;
+from config.tmall import TMALL_DEFAULT_HEADERS;
 
 def get_coupon_info(cookie_list = []):
   url = "https://shell.mkt.taobao.com/coupon/getActivityInfo"
   payload = "{\"id\":\"5907348532\",\"queryDetail\":\"true\",\"couponType\":\"0\"}"
   cookie_jar = RequestsCookieJar()
   for cookie_item in cookie_list:
     cookie_jar.set(cookie_item['name'], cookie_item['value'], domain=cookie_item['domain'])
```

