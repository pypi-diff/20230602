# Comparing `tmp/python-sonarqube-api-2.0.2.tar.gz` & `tmp/python-sonarqube-api-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sonarqube-api-2.0.2.tar", last modified: Sun May 28 13:14:42 2023, max compression
+gzip compressed data, was "dist/python-sonarqube-api-2.0.3.tar", last modified: Fri Jun  2 15:15:26 2023, max compression
```

## Comparing `python-sonarqube-api-2.0.2.tar` & `python-sonarqube-api-2.0.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-28 13:14:42.616214 python-sonarqube-api-2.0.2/
--rw-r--r--   0 shijialiang   (501) staff       (20)    34523 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/LICENSE
--rw-r--r--   0 shijialiang   (501) staff       (20)       33 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/MANIFEST.in
--rw-r--r--   0 shijialiang   (501) staff       (20)     5856 2023-05-28 13:14:42.615965 python-sonarqube-api-2.0.2/PKG-INFO
--rw-r--r--   0 shijialiang   (501) staff       (20)     4737 2023-05-28 13:13:25.000000 python-sonarqube-api-2.0.2/README.rst
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-28 13:14:42.598734 python-sonarqube-api-2.0.2/python_sonarqube_api.egg-info/
--rw-r--r--   0 shijialiang   (501) staff       (20)     5856 2023-05-28 13:14:42.000000 python-sonarqube-api-2.0.2/python_sonarqube_api.egg-info/PKG-INFO
--rw-r--r--   0 shijialiang   (501) staff       (20)     1144 2023-05-28 13:14:42.000000 python-sonarqube-api-2.0.2/python_sonarqube_api.egg-info/SOURCES.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)        1 2023-05-28 13:14:42.000000 python-sonarqube-api-2.0.2/python_sonarqube_api.egg-info/dependency_links.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)        9 2023-05-28 13:14:42.000000 python-sonarqube-api-2.0.2/python_sonarqube_api.egg-info/requires.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)       10 2023-05-28 13:14:42.000000 python-sonarqube-api-2.0.2/python_sonarqube_api.egg-info/top_level.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)        9 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/requirements.txt
--rw-r--r--   0 shijialiang   (501) staff       (20)       38 2023-05-28 13:14:42.616272 python-sonarqube-api-2.0.2/setup.cfg
--rw-r--r--   0 shijialiang   (501) staff       (20)     2497 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/setup.py
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-28 13:14:42.599020 python-sonarqube-api-2.0.2/sonarqube/
--rw-r--r--   0 shijialiang   (501) staff       (20)      192 2023-05-28 13:13:25.000000 python-sonarqube-api-2.0.2/sonarqube/__init__.py
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-28 13:14:42.612925 python-sonarqube-api-2.0.2/sonarqube/rest/
--rw-r--r--   0 shijialiang   (501) staff       (20)     6232 2023-05-28 13:13:25.000000 python-sonarqube-api-2.0.2/sonarqube/rest/__init__.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      988 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/audit_logs.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      622 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/auth.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2110 2023-05-28 13:13:25.000000 python-sonarqube-api-2.0.2/sonarqube/rest/ce.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      814 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/duplications.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      742 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/editions.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      786 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/favorites.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     8130 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/issues.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      723 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/languages.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1272 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/measures.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      947 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/metrics.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1917 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/project_analyses.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1250 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/project_badges.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      725 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/project_branches.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1072 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/project_dump.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      849 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/project_tags.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2159 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/projects.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2389 2023-05-28 13:13:25.000000 python-sonarqube-api-2.0.2/sonarqube/rest/qualitygates.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     3115 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/qualityprofiles.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     8231 2023-05-28 13:13:25.000000 python-sonarqube-api-2.0.2/sonarqube/rest/rules.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      623 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/server.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2928 2023-05-28 13:13:25.000000 python-sonarqube-api-2.0.2/sonarqube/rest/user_groups.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2018 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/user_tokens.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1034 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/users.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     1627 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/rest/views.py
-drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-05-28 13:14:42.614893 python-sonarqube-api-2.0.2/sonarqube/utils/
--rw-r--r--   0 shijialiang   (501) staff       (20)       69 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/utils/__init__.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     3631 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/utils/common.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     2370 2023-05-28 13:13:25.000000 python-sonarqube-api-2.0.2/sonarqube/utils/config.py
--rw-r--r--   0 shijialiang   (501) staff       (20)      401 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/utils/exceptions.py
--rw-r--r--   0 shijialiang   (501) staff       (20)     4841 2023-05-26 14:48:52.000000 python-sonarqube-api-2.0.2/sonarqube/utils/rest_client.py
+drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-06-02 15:15:26.000000 python-sonarqube-api-2.0.3/
+-rw-r--r--   0 shijialiang   (501) staff       (20)    34523 2023-05-26 14:22:04.000000 python-sonarqube-api-2.0.3/LICENSE
+-rw-r--r--   0 shijialiang   (501) staff       (20)       33 2023-05-26 14:22:04.000000 python-sonarqube-api-2.0.3/MANIFEST.in
+-rw-r--r--   0 shijialiang   (501) staff       (20)     6883 2023-06-02 15:15:26.000000 python-sonarqube-api-2.0.3/PKG-INFO
+-rw-r--r--   0 shijialiang   (501) staff       (20)     4824 2023-06-02 14:25:09.000000 python-sonarqube-api-2.0.3/README.rst
+drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-06-02 15:15:26.000000 python-sonarqube-api-2.0.3/python_sonarqube_api.egg-info/
+-rw-r--r--   0 shijialiang   (501) staff       (20)     6883 2023-06-02 15:15:26.000000 python-sonarqube-api-2.0.3/python_sonarqube_api.egg-info/PKG-INFO
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1144 2023-06-02 15:15:26.000000 python-sonarqube-api-2.0.3/python_sonarqube_api.egg-info/SOURCES.txt
+-rw-r--r--   0 shijialiang   (501) staff       (20)        1 2023-06-02 15:15:26.000000 python-sonarqube-api-2.0.3/python_sonarqube_api.egg-info/dependency_links.txt
+-rw-r--r--   0 shijialiang   (501) staff       (20)        9 2023-06-02 15:15:26.000000 python-sonarqube-api-2.0.3/python_sonarqube_api.egg-info/requires.txt
+-rw-r--r--   0 shijialiang   (501) staff       (20)       10 2023-06-02 15:15:26.000000 python-sonarqube-api-2.0.3/python_sonarqube_api.egg-info/top_level.txt
+-rw-r--r--   0 shijialiang   (501) staff       (20)        9 2023-05-26 14:22:04.000000 python-sonarqube-api-2.0.3/requirements.txt
+-rw-r--r--   0 shijialiang   (501) staff       (20)       38 2023-06-02 15:15:26.000000 python-sonarqube-api-2.0.3/setup.cfg
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2524 2023-06-02 15:15:14.000000 python-sonarqube-api-2.0.3/setup.py
+drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-06-02 15:15:26.000000 python-sonarqube-api-2.0.3/sonarqube/
+-rw-r--r--   0 shijialiang   (501) staff       (20)      192 2023-06-02 15:10:53.000000 python-sonarqube-api-2.0.3/sonarqube/__init__.py
+drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-06-02 15:15:26.000000 python-sonarqube-api-2.0.3/sonarqube/rest/
+-rw-r--r--   0 shijialiang   (501) staff       (20)     6232 2023-05-28 13:08:14.000000 python-sonarqube-api-2.0.3/sonarqube/rest/__init__.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      988 2023-05-26 14:22:04.000000 python-sonarqube-api-2.0.3/sonarqube/rest/audit_logs.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      622 2023-05-26 14:35:59.000000 python-sonarqube-api-2.0.3/sonarqube/rest/auth.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2110 2023-05-28 13:03:06.000000 python-sonarqube-api-2.0.3/sonarqube/rest/ce.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      814 2023-05-26 14:22:04.000000 python-sonarqube-api-2.0.3/sonarqube/rest/duplications.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      742 2023-05-26 14:22:04.000000 python-sonarqube-api-2.0.3/sonarqube/rest/editions.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      786 2023-05-26 14:36:14.000000 python-sonarqube-api-2.0.3/sonarqube/rest/favorites.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     8130 2023-05-26 14:36:44.000000 python-sonarqube-api-2.0.3/sonarqube/rest/issues.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      723 2023-05-26 14:22:04.000000 python-sonarqube-api-2.0.3/sonarqube/rest/languages.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1272 2023-05-26 14:37:00.000000 python-sonarqube-api-2.0.3/sonarqube/rest/measures.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      947 2023-05-26 14:22:04.000000 python-sonarqube-api-2.0.3/sonarqube/rest/metrics.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1917 2023-05-26 14:37:35.000000 python-sonarqube-api-2.0.3/sonarqube/rest/project_analyses.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1250 2023-05-26 14:37:53.000000 python-sonarqube-api-2.0.3/sonarqube/rest/project_badges.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      725 2023-05-26 14:38:08.000000 python-sonarqube-api-2.0.3/sonarqube/rest/project_branches.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1072 2023-05-26 14:22:04.000000 python-sonarqube-api-2.0.3/sonarqube/rest/project_dump.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      849 2023-05-26 14:38:21.000000 python-sonarqube-api-2.0.3/sonarqube/rest/project_tags.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2159 2023-05-26 14:39:31.000000 python-sonarqube-api-2.0.3/sonarqube/rest/projects.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2389 2023-05-28 13:03:56.000000 python-sonarqube-api-2.0.3/sonarqube/rest/qualitygates.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     3115 2023-05-26 14:41:06.000000 python-sonarqube-api-2.0.3/sonarqube/rest/qualityprofiles.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     8231 2023-05-28 13:06:04.000000 python-sonarqube-api-2.0.3/sonarqube/rest/rules.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      623 2023-05-26 14:22:04.000000 python-sonarqube-api-2.0.3/sonarqube/rest/server.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2928 2023-05-28 13:06:43.000000 python-sonarqube-api-2.0.3/sonarqube/rest/user_groups.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2018 2023-05-26 14:22:04.000000 python-sonarqube-api-2.0.3/sonarqube/rest/user_tokens.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1034 2023-05-26 14:42:56.000000 python-sonarqube-api-2.0.3/sonarqube/rest/users.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     1627 2023-05-26 14:43:56.000000 python-sonarqube-api-2.0.3/sonarqube/rest/views.py
+drwxr-xr-x   0 shijialiang   (501) staff       (20)        0 2023-06-02 15:15:26.000000 python-sonarqube-api-2.0.3/sonarqube/utils/
+-rw-r--r--   0 shijialiang   (501) staff       (20)       69 2023-05-26 14:22:04.000000 python-sonarqube-api-2.0.3/sonarqube/utils/__init__.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     3631 2023-05-26 14:22:05.000000 python-sonarqube-api-2.0.3/sonarqube/utils/common.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     2370 2023-05-28 13:08:01.000000 python-sonarqube-api-2.0.3/sonarqube/utils/config.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)      401 2023-05-26 14:22:05.000000 python-sonarqube-api-2.0.3/sonarqube/utils/exceptions.py
+-rw-r--r--   0 shijialiang   (501) staff       (20)     4841 2023-05-26 14:22:05.000000 python-sonarqube-api-2.0.3/sonarqube/utils/rest_client.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `python-sonarqube-api-2.0.2/LICENSE` & `python-sonarqube-api-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.2/PKG-INFO` & `python-sonarqube-api-2.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,139 +1,140 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: python-sonarqube-api
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python wrapper for the SonarQube and SonarCloud API.
 Home-page: https://github.com/shijl0925/python-sonarqube-api
 Author: Jialiang Shi
 Author-email: kevin09254930sjl@gmail.com
-License: AGPL
+License: AGPLv3
+Description: 
+        .. image:: https://img.shields.io/pypi/pyversions/python-sonarqube-api.svg
+            :target: https://pypi.python.org/pypi/python-sonarqube-api
+        .. image:: https://img.shields.io/pypi/v/python-sonarqube-api.svg
+            :target: https://pypi.python.org/pypi/python-sonarqube-api
+        .. image:: https://pepy.tech/badge/python-sonarqube-api
+            :target: https://pepy.tech/project/python-sonarqube-api
+        .. image:: https://static.pepy.tech/badge/python-sonarqube-api/month
+            :target: https://pepy.tech/project/python-sonarqube-api
+        .. image:: https://sonarcloud.io/api/project_badges/measure?project=shijl0925_python-sonarqube-api&metric=alert_status
+            :target: https://sonarcloud.io/dashboard?id=shijl0925_python-sonarqube-api
+        .. image:: https://img.shields.io/github/license/shijl0925/python-sonarqube-api.svg
+            :target: LICENSE
+        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+            :target: https://github.com/psf/black
+        
+        
+        ==========================================================================================================================================
+        Python Client library for interacting with Community, Developer, and Enterprise Editions SonarQube's REST APIs and SonarCloud's REST APIs.
+        ==========================================================================================================================================
+        
+        python-sonarqube-api provides a simple interface for clients to interact with SonarQube via the REST API.
+        
+        Editions
+        ========
+        
+        There are two editions of python-sonarqube-api:
+        
+         * Community Edition (CE) is available freely under the GNU Affero General Public License v3.0.
+         * Professional Edition (PE) includes `extra features <https://python-sonarqube-pro-api.readthedocs.io/en/latest/#api-reference>`_
+           that are more useful for developers with more than 280 interface functions. To use PE and get timely Email support and continuous updates,
+           please become a Purchaser(https://shijl0925.gumroad.com/l/nlokc) and become a subscriber(https://shijl0925.gumroad.com/subscribe).
+        
+        +---------------------+---------------------+-----------------------+
+        | Differences         | Community Edition   | Professional Edition  |
+        +=====================+=====================+=======================+
+        | License             | GNU AGPLv3 License  | MIT License           |
+        +---------------------+---------------------+-----------------------+
+        | Commercial Use      | No                  | Yes                   |
+        +---------------------+---------------------+-----------------------+
+        | Supported APIs      | 40                  | more than 280         |
+        | (SonarQube Web APIs)|                     |                       |
+        +---------------------+---------------------+-----------------------+
+        | Compatibility       | 7.9.x - 8.9.x       | 7.9.x - 10.x          |
+        | (SonarQube Versions)|                     |                       |
+        +---------------------+---------------------+-----------------------+
+        
+        **Payment only needs to be made once, and library updates will be provided for free.**
+        
+        Installation
+        ============
+        
+        Community Edition
+        -----------------
+        
+        The easiest way to install the latest version is by using pip to pull it from PyPI::
+        
+            pip install  --upgrade python-sonarqube-api
+        
+        Professional Edition
+        --------------------
+        Use command pip to install the Python wheel or source package, Use --force-reinstall to force an installation If necessary::
+        
+            pip install python_sonarqube_pro_api-x.y.z-py3-none-any.whl
+        
+        
+        Documentation
+        =============
+        
+        The full documentation for API is available on `readthedocs
+        <https://python-sonarqube-pro-api.readthedocs.io/en/latest/>`_.
+        
+        
+        Compatibility
+        =============
+        
+        * This package is compatible Python versions 2.7, 3.3+.
+        * Tested with SonarQube Community Edition 8.9.x LTS and SonarCloud Server.
+        
+        Donate
+        ======
+        
+        donations are not mandatory but very welcomed
+        If you like my work and want to support development or buy me a coffee `PayPal Donate <https://paypal.me/shijialiang0925>`_
+        
+        Usage
+        =====
+        
+        The Client is easy to use, you just need to initialize it with the
+        connection parameters (default sonarqube url is http://localhost:9000).
+        
+        Example::
+        
+            from sonarqube import SonarQubeClient
+        
+            sonar = SonarQubeClient(sonarqube_url="http://localhost:9000", username='admin', password='admin')
+        
+        
+        Sonar authentication tokens can also be used in place of username and password::
+        
+            sonar = SonarQubeClient(sonarqube_url="http://localhost:9000", token='*****************')
+        
+        
+        API example
+        -----------
+        
+        The example documentation for SonarQubeClient APIs is available on `API examples
+        <https://python-sonarqube-pro-api.readthedocs.io/en/latest/examples.html>`_.
+        
+        
+        Licensing
+        -----------
+        See the `LICENSE <https://github.com/shijl0925/python-sonarqube-api/blob/master/LICENSE>`_ file for licensing information as it pertains to files in this repository.
+        
 Keywords: api sonarqube sonar client wrapper sonarcloud
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
-License-File: LICENSE
-
-
-.. image:: https://img.shields.io/pypi/pyversions/python-sonarqube-api.svg
-    :target: https://pypi.python.org/pypi/python-sonarqube-api
-.. image:: https://img.shields.io/pypi/v/python-sonarqube-api.svg
-    :target: https://pypi.python.org/pypi/python-sonarqube-api
-.. image:: https://pepy.tech/badge/python-sonarqube-api
-    :target: https://pepy.tech/project/python-sonarqube-api
-.. image:: https://static.pepy.tech/badge/python-sonarqube-api/month
-    :target: https://pepy.tech/project/python-sonarqube-api
-.. image:: https://sonarcloud.io/api/project_badges/measure?project=shijl0925_python-sonarqube-api&metric=alert_status
-    :target: https://sonarcloud.io/dashboard?id=shijl0925_python-sonarqube-api
-.. image:: https://img.shields.io/github/license/shijl0925/python-sonarqube-api.svg
-    :target: LICENSE
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-    :target: https://github.com/psf/black
-
-
-==========================================================================================================================================
-Python Client library for interacting with Community, Developer, and Enterprise Editions SonarQube's REST APIs and SonarCloud's REST APIs.
-==========================================================================================================================================
-
-python-sonarqube-api provides a simple interface for clients to interact with SonarQube via the REST API.
-
-Editions
-========
-
-There are two editions of python-sonarqube-api:
-
- * Community Edition (CE) is available freely under the GNU Affero General Public License v3.0.
- * Professional Edition (PE) includes `extra features <https://python-sonarqube-pro-api.readthedocs.io/en/latest/#api-reference>`_
-   that are more useful for developers with more than 280 interface functions. To use PE and get timely Email support and continuous updates,
-   please become a Purchaser(https://shijl0925.gumroad.com/l/nlokc) and become a subscriber(https://shijl0925.gumroad.com/subscribe).
-
-+---------------------+---------------------+-----------------------+
-| Differences         | Community Edition   | Professional Edition  |
-+=====================+=====================+=======================+
-| License             | GNU AGPLv3 License  | MIT License           |
-+---------------------+---------------------+-----------------------+
-| Commercial Use      | No                  | Yes                   |
-+---------------------+---------------------+-----------------------+
-| Functions           | 40                  | more than 280         |
-| (REST APIs)         |                     |                       |
-+---------------------+---------------------+-----------------------+
-| Compatibility       | 7.9.x - 8.9.x       | 7.9.x - 10.x          |
-| (SonarQube Versions)|                     |                       |
-+---------------------+---------------------+-----------------------+
-
-Installation
-============
-
-Community Edition
------------------
-
-The easiest way to install the latest version is by using pip to pull it from PyPI::
-
-    pip install  --upgrade python-sonarqube-api
-
-
-Professional Edition
---------------------
-Use command pip to install the Python wheel or source package, Use --force-reinstall to force an installation If necessary::
-
-    pip install python_sonarqube_pro_api-x.y.z-py3-none-any.whl
-
-
-Documentation
-=============
-
-The full documentation for API is available on `readthedocs
-<https://python-sonarqube-pro-api.readthedocs.io/en/latest/>`_.
-
-
-Compatibility
-=============
-
-* This package is compatible Python versions 2.7, 3.3+.
-* Tested with SonarQube Community Edition 8.9.x LTS and SonarCloud Server.
-
-Donate
-======
-
-donations are not mandatory but very welcomed
-If you like my work and want to support development or buy me a coffee `PayPal Donate <https://paypal.me/shijialiang0925>`_
-
-Usage
-=====
-
-The Client is easy to use, you just need to initialize it with the
-connection parameters (default sonarqube url is http://localhost:9000).
-
-Example::
-
-    from sonarqube import SonarQubeClient
-
-    sonar = SonarQubeClient(sonarqube_url="http://localhost:9000", username='admin', password='admin')
-
-
-Sonar authentication tokens can also be used in place of username and password::
-
-    sonar = SonarQubeClient(sonarqube_url="http://localhost:9000", token='*****************')
-
-
-API example
------------
-
-The example documentation for SonarQubeClient APIs is available on `API examples
-<https://python-sonarqube-pro-api.readthedocs.io/en/latest/examples.html>`_.
-
-
-Licensing
------------
-See the `LICENSE <https://github.com/shijl0925/python-sonarqube-api/blob/master/LICENSE>`_ file for licensing information as it pertains to files in this repository.
```

### Comparing `python-sonarqube-api-2.0.2/README.rst` & `python-sonarqube-api-2.0.3/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -34,32 +34,33 @@
 +---------------------+---------------------+-----------------------+
 | Differences         | Community Edition   | Professional Edition  |
 +=====================+=====================+=======================+
 | License             | GNU AGPLv3 License  | MIT License           |
 +---------------------+---------------------+-----------------------+
 | Commercial Use      | No                  | Yes                   |
 +---------------------+---------------------+-----------------------+
-| Functions           | 40                  | more than 280         |
-| (REST APIs)         |                     |                       |
+| Supported APIs      | 40                  | more than 280         |
+| (SonarQube Web APIs)|                     |                       |
 +---------------------+---------------------+-----------------------+
 | Compatibility       | 7.9.x - 8.9.x       | 7.9.x - 10.x          |
 | (SonarQube Versions)|                     |                       |
 +---------------------+---------------------+-----------------------+
 
+**Payment only needs to be made once, and library updates will be provided for free.**
+
 Installation
 ============
 
 Community Edition
 -----------------
 
 The easiest way to install the latest version is by using pip to pull it from PyPI::
 
     pip install  --upgrade python-sonarqube-api
 
-
 Professional Edition
 --------------------
 Use command pip to install the Python wheel or source package, Use --force-reinstall to force an installation If necessary::
 
     pip install python_sonarqube_pro_api-x.y.z-py3-none-any.whl
```

### Comparing `python-sonarqube-api-2.0.2/python_sonarqube_api.egg-info/PKG-INFO` & `python-sonarqube-api-2.0.3/python_sonarqube_api.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,139 +1,140 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: python-sonarqube-api
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python wrapper for the SonarQube and SonarCloud API.
 Home-page: https://github.com/shijl0925/python-sonarqube-api
 Author: Jialiang Shi
 Author-email: kevin09254930sjl@gmail.com
-License: AGPL
+License: AGPLv3
+Description: 
+        .. image:: https://img.shields.io/pypi/pyversions/python-sonarqube-api.svg
+            :target: https://pypi.python.org/pypi/python-sonarqube-api
+        .. image:: https://img.shields.io/pypi/v/python-sonarqube-api.svg
+            :target: https://pypi.python.org/pypi/python-sonarqube-api
+        .. image:: https://pepy.tech/badge/python-sonarqube-api
+            :target: https://pepy.tech/project/python-sonarqube-api
+        .. image:: https://static.pepy.tech/badge/python-sonarqube-api/month
+            :target: https://pepy.tech/project/python-sonarqube-api
+        .. image:: https://sonarcloud.io/api/project_badges/measure?project=shijl0925_python-sonarqube-api&metric=alert_status
+            :target: https://sonarcloud.io/dashboard?id=shijl0925_python-sonarqube-api
+        .. image:: https://img.shields.io/github/license/shijl0925/python-sonarqube-api.svg
+            :target: LICENSE
+        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+            :target: https://github.com/psf/black
+        
+        
+        ==========================================================================================================================================
+        Python Client library for interacting with Community, Developer, and Enterprise Editions SonarQube's REST APIs and SonarCloud's REST APIs.
+        ==========================================================================================================================================
+        
+        python-sonarqube-api provides a simple interface for clients to interact with SonarQube via the REST API.
+        
+        Editions
+        ========
+        
+        There are two editions of python-sonarqube-api:
+        
+         * Community Edition (CE) is available freely under the GNU Affero General Public License v3.0.
+         * Professional Edition (PE) includes `extra features <https://python-sonarqube-pro-api.readthedocs.io/en/latest/#api-reference>`_
+           that are more useful for developers with more than 280 interface functions. To use PE and get timely Email support and continuous updates,
+           please become a Purchaser(https://shijl0925.gumroad.com/l/nlokc) and become a subscriber(https://shijl0925.gumroad.com/subscribe).
+        
+        +---------------------+---------------------+-----------------------+
+        | Differences         | Community Edition   | Professional Edition  |
+        +=====================+=====================+=======================+
+        | License             | GNU AGPLv3 License  | MIT License           |
+        +---------------------+---------------------+-----------------------+
+        | Commercial Use      | No                  | Yes                   |
+        +---------------------+---------------------+-----------------------+
+        | Supported APIs      | 40                  | more than 280         |
+        | (SonarQube Web APIs)|                     |                       |
+        +---------------------+---------------------+-----------------------+
+        | Compatibility       | 7.9.x - 8.9.x       | 7.9.x - 10.x          |
+        | (SonarQube Versions)|                     |                       |
+        +---------------------+---------------------+-----------------------+
+        
+        **Payment only needs to be made once, and library updates will be provided for free.**
+        
+        Installation
+        ============
+        
+        Community Edition
+        -----------------
+        
+        The easiest way to install the latest version is by using pip to pull it from PyPI::
+        
+            pip install  --upgrade python-sonarqube-api
+        
+        Professional Edition
+        --------------------
+        Use command pip to install the Python wheel or source package, Use --force-reinstall to force an installation If necessary::
+        
+            pip install python_sonarqube_pro_api-x.y.z-py3-none-any.whl
+        
+        
+        Documentation
+        =============
+        
+        The full documentation for API is available on `readthedocs
+        <https://python-sonarqube-pro-api.readthedocs.io/en/latest/>`_.
+        
+        
+        Compatibility
+        =============
+        
+        * This package is compatible Python versions 2.7, 3.3+.
+        * Tested with SonarQube Community Edition 8.9.x LTS and SonarCloud Server.
+        
+        Donate
+        ======
+        
+        donations are not mandatory but very welcomed
+        If you like my work and want to support development or buy me a coffee `PayPal Donate <https://paypal.me/shijialiang0925>`_
+        
+        Usage
+        =====
+        
+        The Client is easy to use, you just need to initialize it with the
+        connection parameters (default sonarqube url is http://localhost:9000).
+        
+        Example::
+        
+            from sonarqube import SonarQubeClient
+        
+            sonar = SonarQubeClient(sonarqube_url="http://localhost:9000", username='admin', password='admin')
+        
+        
+        Sonar authentication tokens can also be used in place of username and password::
+        
+            sonar = SonarQubeClient(sonarqube_url="http://localhost:9000", token='*****************')
+        
+        
+        API example
+        -----------
+        
+        The example documentation for SonarQubeClient APIs is available on `API examples
+        <https://python-sonarqube-pro-api.readthedocs.io/en/latest/examples.html>`_.
+        
+        
+        Licensing
+        -----------
+        See the `LICENSE <https://github.com/shijl0925/python-sonarqube-api/blob/master/LICENSE>`_ file for licensing information as it pertains to files in this repository.
+        
 Keywords: api sonarqube sonar client wrapper sonarcloud
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
-License-File: LICENSE
-
-
-.. image:: https://img.shields.io/pypi/pyversions/python-sonarqube-api.svg
-    :target: https://pypi.python.org/pypi/python-sonarqube-api
-.. image:: https://img.shields.io/pypi/v/python-sonarqube-api.svg
-    :target: https://pypi.python.org/pypi/python-sonarqube-api
-.. image:: https://pepy.tech/badge/python-sonarqube-api
-    :target: https://pepy.tech/project/python-sonarqube-api
-.. image:: https://static.pepy.tech/badge/python-sonarqube-api/month
-    :target: https://pepy.tech/project/python-sonarqube-api
-.. image:: https://sonarcloud.io/api/project_badges/measure?project=shijl0925_python-sonarqube-api&metric=alert_status
-    :target: https://sonarcloud.io/dashboard?id=shijl0925_python-sonarqube-api
-.. image:: https://img.shields.io/github/license/shijl0925/python-sonarqube-api.svg
-    :target: LICENSE
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-    :target: https://github.com/psf/black
-
-
-==========================================================================================================================================
-Python Client library for interacting with Community, Developer, and Enterprise Editions SonarQube's REST APIs and SonarCloud's REST APIs.
-==========================================================================================================================================
-
-python-sonarqube-api provides a simple interface for clients to interact with SonarQube via the REST API.
-
-Editions
-========
-
-There are two editions of python-sonarqube-api:
-
- * Community Edition (CE) is available freely under the GNU Affero General Public License v3.0.
- * Professional Edition (PE) includes `extra features <https://python-sonarqube-pro-api.readthedocs.io/en/latest/#api-reference>`_
-   that are more useful for developers with more than 280 interface functions. To use PE and get timely Email support and continuous updates,
-   please become a Purchaser(https://shijl0925.gumroad.com/l/nlokc) and become a subscriber(https://shijl0925.gumroad.com/subscribe).
-
-+---------------------+---------------------+-----------------------+
-| Differences         | Community Edition   | Professional Edition  |
-+=====================+=====================+=======================+
-| License             | GNU AGPLv3 License  | MIT License           |
-+---------------------+---------------------+-----------------------+
-| Commercial Use      | No                  | Yes                   |
-+---------------------+---------------------+-----------------------+
-| Functions           | 40                  | more than 280         |
-| (REST APIs)         |                     |                       |
-+---------------------+---------------------+-----------------------+
-| Compatibility       | 7.9.x - 8.9.x       | 7.9.x - 10.x          |
-| (SonarQube Versions)|                     |                       |
-+---------------------+---------------------+-----------------------+
-
-Installation
-============
-
-Community Edition
------------------
-
-The easiest way to install the latest version is by using pip to pull it from PyPI::
-
-    pip install  --upgrade python-sonarqube-api
-
-
-Professional Edition
---------------------
-Use command pip to install the Python wheel or source package, Use --force-reinstall to force an installation If necessary::
-
-    pip install python_sonarqube_pro_api-x.y.z-py3-none-any.whl
-
-
-Documentation
-=============
-
-The full documentation for API is available on `readthedocs
-<https://python-sonarqube-pro-api.readthedocs.io/en/latest/>`_.
-
-
-Compatibility
-=============
-
-* This package is compatible Python versions 2.7, 3.3+.
-* Tested with SonarQube Community Edition 8.9.x LTS and SonarCloud Server.
-
-Donate
-======
-
-donations are not mandatory but very welcomed
-If you like my work and want to support development or buy me a coffee `PayPal Donate <https://paypal.me/shijialiang0925>`_
-
-Usage
-=====
-
-The Client is easy to use, you just need to initialize it with the
-connection parameters (default sonarqube url is http://localhost:9000).
-
-Example::
-
-    from sonarqube import SonarQubeClient
-
-    sonar = SonarQubeClient(sonarqube_url="http://localhost:9000", username='admin', password='admin')
-
-
-Sonar authentication tokens can also be used in place of username and password::
-
-    sonar = SonarQubeClient(sonarqube_url="http://localhost:9000", token='*****************')
-
-
-API example
------------
-
-The example documentation for SonarQubeClient APIs is available on `API examples
-<https://python-sonarqube-pro-api.readthedocs.io/en/latest/examples.html>`_.
-
-
-Licensing
------------
-See the `LICENSE <https://github.com/shijl0925/python-sonarqube-api/blob/master/LICENSE>`_ file for licensing information as it pertains to files in this repository.
```

### Comparing `python-sonarqube-api-2.0.2/python_sonarqube_api.egg-info/SOURCES.txt` & `python-sonarqube-api-2.0.3/python_sonarqube_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.2/setup.py` & `python-sonarqube-api-2.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,22 +34,22 @@
     version=get_version(),
 
     description='Python wrapper for the SonarQube and SonarCloud API.',
     long_description=long_description,
     url='https://github.com/shijl0925/python-sonarqube-api',
     author='Jialiang Shi',
     author_email='kevin09254930sjl@gmail.com',
-    license='AGPL',
+    license='AGPLv3',
 
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Plugins',
         'Intended Audience :: Developers',
-        'License :: OSI Approved :: BSD License',
+        'License :: OSI Approved :: GNU Affero General Public License v3',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

### Comparing `python-sonarqube-api-2.0.2/sonarqube/rest/__init__.py` & `python-sonarqube-api-2.0.3/sonarqube/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.2/sonarqube/rest/audit_logs.py` & `python-sonarqube-api-2.0.3/sonarqube/rest/audit_logs.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.2/sonarqube/rest/auth.py` & `python-sonarqube-api-2.0.3/sonarqube/rest/auth.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.2/sonarqube/rest/ce.py` & `python-sonarqube-api-2.0.3/sonarqube/rest/ce.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.2/sonarqube/rest/duplications.py` & `python-sonarqube-api-2.0.3/sonarqube/rest/duplications.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.2/sonarqube/rest/editions.py` & `python-sonarqube-api-2.0.3/sonarqube/rest/editions.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.2/sonarqube/rest/favorites.py` & `python-sonarqube-api-2.0.3/sonarqube/rest/favorites.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.2/sonarqube/rest/issues.py` & `python-sonarqube-api-2.0.3/sonarqube/rest/issues.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.2/sonarqube/rest/languages.py` & `python-sonarqube-api-2.0.3/sonarqube/rest/languages.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.2/sonarqube/rest/measures.py` & `python-sonarqube-api-2.0.3/sonarqube/rest/measures.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.2/sonarqube/rest/metrics.py` & `python-sonarqube-api-2.0.3/sonarqube/rest/metrics.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.2/sonarqube/rest/project_analyses.py` & `python-sonarqube-api-2.0.3/sonarqube/rest/project_analyses.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.2/sonarqube/rest/project_badges.py` & `python-sonarqube-api-2.0.3/sonarqube/rest/project_badges.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.2/sonarqube/rest/project_branches.py` & `python-sonarqube-api-2.0.3/sonarqube/rest/project_branches.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.2/sonarqube/rest/project_dump.py` & `python-sonarqube-api-2.0.3/sonarqube/rest/project_dump.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.2/sonarqube/rest/project_tags.py` & `python-sonarqube-api-2.0.3/sonarqube/rest/project_tags.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.2/sonarqube/rest/projects.py` & `python-sonarqube-api-2.0.3/sonarqube/rest/projects.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.2/sonarqube/rest/qualitygates.py` & `python-sonarqube-api-2.0.3/sonarqube/rest/qualitygates.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.2/sonarqube/rest/qualityprofiles.py` & `python-sonarqube-api-2.0.3/sonarqube/rest/qualityprofiles.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.2/sonarqube/rest/rules.py` & `python-sonarqube-api-2.0.3/sonarqube/rest/rules.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.2/sonarqube/rest/server.py` & `python-sonarqube-api-2.0.3/sonarqube/rest/server.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.2/sonarqube/rest/user_groups.py` & `python-sonarqube-api-2.0.3/sonarqube/rest/user_groups.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.2/sonarqube/rest/user_tokens.py` & `python-sonarqube-api-2.0.3/sonarqube/rest/user_tokens.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.2/sonarqube/rest/users.py` & `python-sonarqube-api-2.0.3/sonarqube/rest/users.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.2/sonarqube/rest/views.py` & `python-sonarqube-api-2.0.3/sonarqube/rest/views.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.2/sonarqube/utils/common.py` & `python-sonarqube-api-2.0.3/sonarqube/utils/common.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.2/sonarqube/utils/config.py` & `python-sonarqube-api-2.0.3/sonarqube/utils/config.py`

 * *Files identical despite different names*

### Comparing `python-sonarqube-api-2.0.2/sonarqube/utils/rest_client.py` & `python-sonarqube-api-2.0.3/sonarqube/utils/rest_client.py`

 * *Files identical despite different names*

