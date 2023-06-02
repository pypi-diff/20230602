# Comparing `tmp/amplitude-data-wrapper-0.4.1.tar.gz` & `tmp/amplitude-data-wrapper-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amplitude-data-wrapper-0.4.1.tar", last modified: Sun May 21 20:30:51 2023, max compression
+gzip compressed data, was "amplitude-data-wrapper-0.4.2.tar", last modified: Fri Jun  2 18:55:24 2023, max compression
```

## Comparing `amplitude-data-wrapper-0.4.1.tar` & `amplitude-data-wrapper-0.4.2.tar`

### file list

```diff
@@ -1,24 +1,14 @@
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 20:30:51.561487 amplitude-data-wrapper-0.4.1/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      130 2023-05-21 17:43:48.000000 amplitude-data-wrapper-0.4.1/.gitignore
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       23 2023-05-20 20:06:46.000000 amplitude-data-wrapper-0.4.1/CODEOWNERS
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1062 2023-05-20 20:06:46.000000 amplitude-data-wrapper-0.4.1/LICENSE
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      820 2023-05-21 20:22:43.000000 amplitude-data-wrapper-0.4.1/Makefile
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     5925 2023-05-21 20:30:51.560445 amplitude-data-wrapper-0.4.1/PKG-INFO
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     4322 2023-05-20 20:06:46.000000 amplitude-data-wrapper-0.4.1/README.md
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 20:30:51.543777 amplitude-data-wrapper-0.4.1/amplitude_data_wrapper/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       51 2023-05-21 19:02:17.000000 amplitude-data-wrapper-0.4.1/amplitude_data_wrapper/__init__.py
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 20:30:51.552338 amplitude-data-wrapper-0.4.1/amplitude_data_wrapper/amplitude_data_wrapper.egg-info/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     5925 2023-05-21 20:30:51.000000 amplitude-data-wrapper-0.4.1/amplitude_data_wrapper/amplitude_data_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      577 2023-05-21 20:30:51.000000 amplitude-data-wrapper-0.4.1/amplitude_data_wrapper/amplitude_data_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-05-21 20:30:51.000000 amplitude-data-wrapper-0.4.1/amplitude_data_wrapper/amplitude_data_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       99 2023-05-21 20:30:51.000000 amplitude-data-wrapper-0.4.1/amplitude_data_wrapper/amplitude_data_wrapper.egg-info/requires.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-05-21 20:30:51.000000 amplitude-data-wrapper-0.4.1/amplitude_data_wrapper/amplitude_data_wrapper.egg-info/top_level.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)    15281 2023-05-20 20:06:46.000000 amplitude-data-wrapper-0.4.1/amplitude_data_wrapper/analytics_api.py
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     2295 2023-05-21 17:25:27.000000 amplitude-data-wrapper-0.4.1/example.py
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      773 2023-05-21 20:29:57.000000 amplitude-data-wrapper-0.4.1/pyproject.toml
-drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-05-21 20:30:51.558812 amplitude-data-wrapper-0.4.1/requirements/
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       43 2023-05-21 17:43:48.000000 amplitude-data-wrapper-0.4.1/requirements/dev.in
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)     2831 2023-05-21 20:20:58.000000 amplitude-data-wrapper-0.4.1/requirements/dev.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       13 2023-05-21 17:43:48.000000 amplitude-data-wrapper-0.4.1/requirements/main.in
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)      412 2023-05-21 20:20:52.000000 amplitude-data-wrapper-0.4.1/requirements/main.txt
--rw-r--r--   0 tobiasmcvey   (501) staff       (20)       38 2023-05-21 20:30:51.561678 amplitude-data-wrapper-0.4.1/setup.cfg
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-02 18:55:24.509167 amplitude-data-wrapper-0.4.2/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     1062 2023-05-20 20:06:46.000000 amplitude-data-wrapper-0.4.2/LICENSE
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      343 2023-06-02 18:55:24.509325 amplitude-data-wrapper-0.4.2/PKG-INFO
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)     4322 2023-05-20 20:06:46.000000 amplitude-data-wrapper-0.4.2/README.md
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-02 18:55:24.504127 amplitude-data-wrapper-0.4.2/amplitude_data_wrapper/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)        0 2023-06-01 19:50:54.000000 amplitude-data-wrapper-0.4.2/amplitude_data_wrapper/__init__.py
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)    15281 2023-05-20 20:06:46.000000 amplitude-data-wrapper-0.4.2/amplitude_data_wrapper/analytics_api.py
+drwxr-xr-x   0 tobiasmcvey   (501) staff       (20)        0 2023-06-02 18:55:24.508505 amplitude-data-wrapper-0.4.2/amplitude_data_wrapper.egg-info/
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      343 2023-06-02 18:55:24.000000 amplitude-data-wrapper-0.4.2/amplitude_data_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      295 2023-06-02 18:55:24.000000 amplitude-data-wrapper-0.4.2/amplitude_data_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)        1 2023-06-02 18:55:24.000000 amplitude-data-wrapper-0.4.2/amplitude_data_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       23 2023-06-02 18:55:24.000000 amplitude-data-wrapper-0.4.2/amplitude_data_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)      464 2023-06-02 18:55:24.510942 amplitude-data-wrapper-0.4.2/setup.cfg
+-rw-r--r--   0 tobiasmcvey   (501) staff       (20)       36 2023-06-02 18:31:26.000000 amplitude-data-wrapper-0.4.2/setup.py
```

### Comparing `amplitude-data-wrapper-0.4.1/LICENSE` & `amplitude-data-wrapper-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `amplitude-data-wrapper-0.4.1/PKG-INFO` & `amplitude-data-wrapper-0.4.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: amplitude-data-wrapper
-Version: 0.4.1
-Summary: python wrapper for using the amplitude analytics and taxonomy APIs
-Author-email: Tobias McVey <tobias.mcvey@nav.no>
-License: MIT License
-        
-        Copyright (c) 2022 NAV IT
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Project-URL: Homepage, https://github.com/navikt/amplitude-data-wrapper
-Keywords: amplitude
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Amplitude data wrapper
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 This is a wrapper for [Amplitude](https://amplitude.com/) APIs. You can use it to query and export data from your account and use the taxonomy API.
 
 Built with [requests](https://requests.readthedocs.io/en/latest/) and [tqdm](https://github.com/tqdm/tqdm)
@@ -194,8 +162,8 @@
 [Get all event types](https://developers.amplitude.com/docs/taxonomy-api#get-all-event-types)
 
 ```python
 types = get_all_event_types(
     api_key=api_key, 
     secret=api_secret, 
     region=1)
-```
+```
```

### Comparing `amplitude-data-wrapper-0.4.1/amplitude_data_wrapper/analytics_api.py` & `amplitude-data-wrapper-0.4.2/amplitude_data_wrapper/analytics_api.py`

 * *Files identical despite different names*

