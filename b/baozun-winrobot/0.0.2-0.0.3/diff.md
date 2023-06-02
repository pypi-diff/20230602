# Comparing `tmp/baozun_winrobot-0.0.2.tar.gz` & `tmp/baozun_winrobot-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/baozun_winrobot-0.0.2.tar", last modified: Thu Jun  1 10:23:19 2023, max compression
+gzip compressed data, was "dist/baozun_winrobot-0.0.3.tar", last modified: Fri Jun  2 05:36:16 2023, max compression
```

## Comparing `baozun_winrobot-0.0.2.tar` & `baozun_winrobot-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxr-xr-x   0 wcgz-dz-100285   (501) staff       (20)        0 2023-06-01 10:23:19.469315 baozun_winrobot-0.0.2/
-drwxr-xr-x   0 wcgz-dz-100285   (501) staff       (20)        0 2023-06-01 10:23:19.467274 baozun_winrobot-0.0.2/Baozun_Winrobot.egg-info/
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)       81 2023-06-01 10:23:19.000000 baozun_winrobot-0.0.2/Baozun_Winrobot.egg-info/PKG-INFO
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)      406 2023-06-01 10:23:19.000000 baozun_winrobot-0.0.2/Baozun_Winrobot.egg-info/SOURCES.txt
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)        1 2023-06-01 10:23:19.000000 baozun_winrobot-0.0.2/Baozun_Winrobot.egg-info/dependency_links.txt
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)        1 2023-06-01 08:06:03.000000 baozun_winrobot-0.0.2/Baozun_Winrobot.egg-info/not-zip-safe
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)        1 2023-06-01 10:23:19.000000 baozun_winrobot-0.0.2/Baozun_Winrobot.egg-info/top_level.txt
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)       81 2023-06-01 10:23:19.468204 baozun_winrobot-0.0.2/PKG-INFO
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)       11 2023-06-01 10:21:00.000000 baozun_winrobot-0.0.2/README.md
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)       38 2023-06-01 10:23:19.469538 baozun_winrobot-0.0.2/setup.cfg
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)      283 2023-06-01 10:22:17.000000 baozun_winrobot-0.0.2/setup.py
+drwxr-xr-x   0 wcgz-dz-100285   (501) staff       (20)        0 2023-06-02 05:36:16.736966 baozun_winrobot-0.0.3/
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)       81 2023-06-02 05:36:16.736567 baozun_winrobot-0.0.3/PKG-INFO
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)       11 2023-06-01 10:21:00.000000 baozun_winrobot-0.0.3/README.md
+drwxr-xr-x   0 wcgz-dz-100285   (501) staff       (20)        0 2023-06-02 05:36:16.732885 baozun_winrobot-0.0.3/baozun_winrobot.egg-info/
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)       81 2023-06-02 05:36:16.000000 baozun_winrobot-0.0.3/baozun_winrobot.egg-info/PKG-INFO
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)      246 2023-06-02 05:36:16.000000 baozun_winrobot-0.0.3/baozun_winrobot.egg-info/SOURCES.txt
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)        1 2023-06-02 05:36:16.000000 baozun_winrobot-0.0.3/baozun_winrobot.egg-info/dependency_links.txt
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)        1 2023-06-02 05:36:16.000000 baozun_winrobot-0.0.3/baozun_winrobot.egg-info/not-zip-safe
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)        7 2023-06-02 05:36:16.000000 baozun_winrobot-0.0.3/baozun_winrobot.egg-info/top_level.txt
+drwxr-xr-x   0 wcgz-dz-100285   (501) staff       (20)        0 2023-06-02 05:36:16.735595 baozun_winrobot-0.0.3/coupon/
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)        0 2023-06-02 03:31:30.000000 baozun_winrobot-0.0.3/coupon/__init__.py
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)      645 2023-06-01 08:01:21.000000 baozun_winrobot-0.0.3/coupon/main.py
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)       38 2023-06-02 05:36:16.737088 baozun_winrobot-0.0.3/setup.cfg
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)      283 2023-06-02 03:13:32.000000 baozun_winrobot-0.0.3/setup.py
```

