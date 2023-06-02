# Comparing `tmp/django-restricted-sessions-0.2.0.tar.gz` & `tmp/django-restricted-sessions-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Thu Apr  6 14:19:57 2017, from Unix
+gzip compressed data, was "dist/django-restricted-sessions-0.3.0.tar", last modified: Tue Dec  3 21:09:33 2019, max compression
```

## Comparing `django-restricted-sessions-0.2.0.tar` & `django-restricted-sessions-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2017-04-06 14:19:50.000000 django-restricted-sessions-0.2.0/
--rw-r--r--   0 erik       (501) staff       (20)      244 2017-04-06 13:12:30.000000 django-restricted-sessions-0.2.0/AUTHORS.rst
--rw-r--r--   0 erik       (501) staff       (20)     3344 2017-04-06 13:00:42.000000 django-restricted-sessions-0.2.0/CONTRIBUTING.rst
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2017-04-06 14:19:01.000000 django-restricted-sessions-0.2.0/django_restricted_sessions.egg-info/
--rw-r--r--   0 erik       (501) staff       (20)     1139 2017-04-06 13:12:30.000000 django-restricted-sessions-0.2.0/HISTORY.rst
--rw-r--r--   0 erik       (501) staff       (20)     1499 2017-04-06 13:00:42.000000 django-restricted-sessions-0.2.0/LICENSE
--rw-r--r--   0 erik       (501) staff       (20)      179 2017-04-06 13:00:42.000000 django-restricted-sessions-0.2.0/MANIFEST.in
--rw-r--r--   0 erik       (501) staff       (20)     4583 2017-04-06 14:19:30.000000 django-restricted-sessions-0.2.0/PKG-INFO
--rw-r--r--   0 erik       (501) staff       (20)     1775 2017-04-06 14:19:50.000000 django-restricted-sessions-0.2.0/README.rst
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2017-04-06 14:19:01.000000 django-restricted-sessions-0.2.0/restrictedsessions/
--rw-r--r--   0 erik       (501) staff       (20)       82 2017-04-06 14:19:01.000000 django-restricted-sessions-0.2.0/setup.cfg
--rwxr-xr-x   0 erik       (501) staff       (20)     1780 2017-04-06 13:12:30.000000 django-restricted-sessions-0.2.0/setup.py
--rw-r--r--   0 erik       (501) staff       (20)       22 2017-04-06 14:12:25.000000 django-restricted-sessions-0.2.0/restrictedsessions/__init__.py
--rw-r--r--   0 erik       (501) staff       (20)     4477 2017-04-06 13:12:30.000000 django-restricted-sessions-0.2.0/restrictedsessions/middleware.py
--rw-r--r--   0 erik       (501) staff       (20)        1 2017-04-06 14:18:59.000000 django-restricted-sessions-0.2.0/django_restricted_sessions.egg-info/dependency_links.txt
--rw-r--r--   0 erik       (501) staff       (20)        1 2016-05-26 20:53:58.000000 django-restricted-sessions-0.2.0/django_restricted_sessions.egg-info/not-zip-safe
--rw-r--r--   0 erik       (501) staff       (20)     4623 2017-04-06 14:18:59.000000 django-restricted-sessions-0.2.0/django_restricted_sessions.egg-info/PKG-INFO
--rw-r--r--   0 erik       (501) staff       (20)       16 2017-04-06 14:18:59.000000 django-restricted-sessions-0.2.0/django_restricted_sessions.egg-info/requires.txt
--rw-r--r--   0 erik       (501) staff       (20)      452 2017-04-06 14:19:01.000000 django-restricted-sessions-0.2.0/django_restricted_sessions.egg-info/SOURCES.txt
--rw-r--r--   0 erik       (501) staff       (20)       19 2017-04-06 14:18:59.000000 django-restricted-sessions-0.2.0/django_restricted_sessions.egg-info/top_level.txt
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2019-12-03 21:09:33.000000 django-restricted-sessions-0.3.0/
+-rw-r--r--   0 sasha      (501) staff       (20)     4832 2019-12-03 21:09:33.000000 django-restricted-sessions-0.3.0/PKG-INFO
+-rw-r--r--   0 sasha      (501) staff       (20)     1499 2017-04-06 13:00:42.000000 django-restricted-sessions-0.3.0/LICENSE
+-rw-r--r--   0 sasha      (501) staff       (20)     3377 2019-12-03 20:47:54.000000 django-restricted-sessions-0.3.0/CONTRIBUTING.rst
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2019-12-03 21:09:33.000000 django-restricted-sessions-0.3.0/restrictedsessions/
+-rw-r--r--   0 sasha      (501) staff       (20)       22 2019-12-03 21:06:34.000000 django-restricted-sessions-0.3.0/restrictedsessions/__init__.py
+-rw-r--r--   0 sasha      (501) staff       (20)     4538 2019-12-03 20:58:39.000000 django-restricted-sessions-0.3.0/restrictedsessions/middleware.py
+drwxr-xr-x   0 sasha      (501) staff       (20)        0 2019-12-03 21:09:33.000000 django-restricted-sessions-0.3.0/django_restricted_sessions.egg-info/
+-rw-r--r--   0 sasha      (501) staff       (20)     4832 2019-12-03 21:09:25.000000 django-restricted-sessions-0.3.0/django_restricted_sessions.egg-info/PKG-INFO
+-rw-r--r--   0 sasha      (501) staff       (20)        1 2016-05-26 20:53:58.000000 django-restricted-sessions-0.3.0/django_restricted_sessions.egg-info/not-zip-safe
+-rw-r--r--   0 sasha      (501) staff       (20)      452 2019-12-03 21:09:33.000000 django-restricted-sessions-0.3.0/django_restricted_sessions.egg-info/SOURCES.txt
+-rw-r--r--   0 sasha      (501) staff       (20)       16 2019-12-03 21:09:25.000000 django-restricted-sessions-0.3.0/django_restricted_sessions.egg-info/requires.txt
+-rw-r--r--   0 sasha      (501) staff       (20)       19 2019-12-03 21:09:25.000000 django-restricted-sessions-0.3.0/django_restricted_sessions.egg-info/top_level.txt
+-rw-r--r--   0 sasha      (501) staff       (20)        1 2019-12-03 21:09:25.000000 django-restricted-sessions-0.3.0/django_restricted_sessions.egg-info/dependency_links.txt
+-rw-r--r--   0 sasha      (501) staff       (20)      179 2017-04-06 13:00:42.000000 django-restricted-sessions-0.3.0/MANIFEST.in
+-rwxr-xr-x   0 sasha      (501) staff       (20)     1777 2019-12-03 21:04:55.000000 django-restricted-sessions-0.3.0/setup.py
+-rw-r--r--   0 sasha      (501) staff       (20)     1295 2019-12-03 21:06:23.000000 django-restricted-sessions-0.3.0/HISTORY.rst
+-rw-r--r--   0 sasha      (501) staff       (20)      241 2019-12-03 20:43:30.000000 django-restricted-sessions-0.3.0/AUTHORS.rst
+-rw-r--r--   0 sasha      (501) staff       (20)       82 2019-12-03 21:09:33.000000 django-restricted-sessions-0.3.0/setup.cfg
+-rw-r--r--   0 sasha      (501) staff       (20)     1782 2019-12-03 20:40:20.000000 django-restricted-sessions-0.3.0/README.rst
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `django-restricted-sessions-0.2.0/CONTRIBUTING.rst` & `django-restricted-sessions-0.3.0/CONTRIBUTING.rst`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 Types of Contributions
 ----------------------
 
 Report Bugs
 ~~~~~~~~~~~
 
-Report bugs at https://github.com/erikr/django-restricted-sessions/issues.
+Report bugs at https://github.com/mxsasha/django-restricted-sessions/issues.
 
 If you are reporting a bug, please include:
 
 * Your operating system name and version.
 * Any details about your local setup that might be helpful in troubleshooting.
 * Detailed steps to reproduce the bug.
 
@@ -39,15 +39,15 @@
 django-restricted-sessions could always use more documentation, whether as part of the 
 official django-restricted-sessions docs, in docstrings, or even on the web in blog posts,
 articles, and such.
 
 Submit Feedback
 ~~~~~~~~~~~~~~~
 
-The best way to send feedback is to file an issue at https://github.com/erikr/django-restricted-sessions/issues.
+The best way to send feedback is to file an issue at https://github.com/mxsasha/django-restricted-sessions/issues.
 
 If you are proposing a feature:
 
 * Explain in detail how it would work.
 * Keep the scope as narrow as possible, to make it easier to implement.
 * Remember that this is a volunteer-driven project, and that contributions
   are welcome :)
@@ -96,16 +96,16 @@
 
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests.
 2. If the pull request adds functionality, the docs should be updated. Put
    your new functionality into a function with a docstring, and add the
    feature to the list in README.rst.
-3. The pull request should work for Python 2.6, 2.7, and 3.3, and for PyPy. Check 
-   https://travis-ci.org/erikr/django-restricted-sessions/pull_requests
+3. The pull request should work for Python 2.7 (Django 1.11 only), 3.5 (Django <3.0 only), 3.6 and 3.7. Check
+   https://travis-ci.org/mxsasha/django-restricted-sessions/pull_requests
    and make sure that the tests pass for all supported Python versions.
 
 Tips
 ----
 
 To run a subset of tests::
```

### Comparing `django-restricted-sessions-0.2.0/HISTORY.rst` & `django-restricted-sessions-0.3.0/HISTORY.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 .. :changelog:
 
 History
 -------
 
+0.3.0 (2019-12-03)
+++++++++++++++++++
+
+* Updated Django support to 1.11, 2.2 and 3.0.
+* Fixed issues when ``X_FORWARDED_FOR`` contains multiple addresses.
+
 0.2.0 (2017-04-06)
 ++++++++++++++++++
 
 * For Django 1.10+ support, changed from `object` to `django.utils.deprecation.MiddlewareMixin`
 * Added PyPI trove classifiers for Django versions and more Python versions
 * Updated `travis.yml` for more Python versions
```

### Comparing `django-restricted-sessions-0.2.0/LICENSE` & `django-restricted-sessions-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-restricted-sessions-0.2.0/PKG-INFO` & `django-restricted-sessions-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 1.1
 Name: django-restricted-sessions
-Version: 0.2.0
+Version: 0.3.0
 Summary: Restrict Django sessions to IP and/or user agent.
-Home-page: https://github.com/erikr/django-restricted-sessions
+Home-page: https://github.com/mxsasha/django-restricted-sessions
 Author: django-restricted-sessions
-Author-email: eromijn@solidlinks.nl
+Author-email: github@mxsasha.eu
 License: BSD
 Description: =============================
         django-restricted-sessions
         =============================
         
         .. image:: https://badge.fury.io/py/django-restricted-sessions.png
             :target: http://badge.fury.io/py/django-restricted-sessions
         
-        .. image:: https://travis-ci.org/erikr/django-restricted-sessions.png?branch=master
-            :target: https://travis-ci.org/erikr/django-restricted-sessions
+        .. image:: https://travis-ci.org/mxsasha/django-restricted-sessions.png?branch=master
+            :target: https://travis-ci.org/mxsasha/django-restricted-sessions
         
-        .. image:: https://coveralls.io/repos/erikr/django-restricted-sessions/badge.png?branch=master&
-            :target: https://coveralls.io/r/erikr/django-restricted-sessions?branch=master
+        .. image:: https://coveralls.io/repos/mxsasha/django-restricted-sessions/badge.png?branch=master&
+            :target: https://coveralls.io/r/mxsasha/django-restricted-sessions?branch=master
         
         Restricts Django sessions to IP and/or user agent.
         
         If the IP or user agent changes after creating the session, the a 400 response is given to the request, the session is
         flushed (all session data deleted, new session created) and a warning is logged. The goal of this middleware is to
         make it harder for an attacker to use a session ID they obtained. It does not make abuse of session IDs impossible.
         
@@ -54,14 +54,20 @@
         
         
         
         
         History
         -------
         
+        0.3.0 (2019-12-03)
+        ++++++++++++++++++
+        
+        * Updated Django support to 1.11, 2.2 and 3.0.
+        * Fixed issues when ``X_FORWARDED_FOR`` contains multiple addresses.
+        
         0.2.0 (2017-04-06)
         ++++++++++++++++++
         
         * For Django 1.10+ support, changed from `object` to `django.utils.deprecation.MiddlewareMixin`
         * Added PyPI trove classifiers for Django versions and more Python versions
         * Updated `travis.yml` for more Python versions
         
@@ -101,18 +107,19 @@
         
         * First release on PyPI.
         
 Keywords: django-restricted-sessions
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 1.8
-Classifier: Framework :: Django :: 1.10
+Classifier: Framework :: Django :: 1.11
+Classifier: Framework :: Django :: 2.2
+Classifier: Framework :: Django :: 3.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
```

### Comparing `django-restricted-sessions-0.2.0/README.rst` & `django-restricted-sessions-0.3.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 =============================
 django-restricted-sessions
 =============================
 
 .. image:: https://badge.fury.io/py/django-restricted-sessions.png
     :target: http://badge.fury.io/py/django-restricted-sessions
 
-.. image:: https://travis-ci.org/erikr/django-restricted-sessions.png?branch=master
-    :target: https://travis-ci.org/erikr/django-restricted-sessions
+.. image:: https://travis-ci.org/mxsasha/django-restricted-sessions.png?branch=master
+    :target: https://travis-ci.org/mxsasha/django-restricted-sessions
 
-.. image:: https://coveralls.io/repos/erikr/django-restricted-sessions/badge.png?branch=master&
-    :target: https://coveralls.io/r/erikr/django-restricted-sessions?branch=master
+.. image:: https://coveralls.io/repos/mxsasha/django-restricted-sessions/badge.png?branch=master&
+    :target: https://coveralls.io/r/mxsasha/django-restricted-sessions?branch=master
 
-Restricts Django sessions to IP and/or user agent. 
+Restricts Django sessions to IP and/or user agent.
 
 If the IP or user agent changes after creating the session, the a 400 response is given to the request, the session is
 flushed (all session data deleted, new session created) and a warning is logged. The goal of this middleware is to
 make it harder for an attacker to use a session ID they obtained. It does not make abuse of session IDs impossible.
 
 For compatibility with IPv6 privacy extensions, by default only the first 64 bits of an IPv6 address are checked.
```

### Comparing `django-restricted-sessions-0.2.0/setup.py` & `django-restricted-sessions-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,36 +25,36 @@
 
 setup(
     name='django-restricted-sessions',
     version=version,
     description="""Restrict Django sessions to IP and/or user agent.""",
     long_description=readme + '\n\n' + history,
     author='django-restricted-sessions',
-    author_email='eromijn@solidlinks.nl',
-    url='https://github.com/erikr/django-restricted-sessions',
+    author_email='github@mxsasha.eu',
+    url='https://github.com/mxsasha/django-restricted-sessions',
     packages=[
         'restrictedsessions',
     ],
     include_package_data=True,
     install_requires=[
         'netaddr>=0.7.10',
     ],
     license="BSD",
     zip_safe=False,
     keywords='django-restricted-sessions',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Framework :: Django',
-        'Framework :: Django :: 1.8',
-        'Framework :: Django :: 1.10',
         'Framework :: Django :: 1.11',
+        'Framework :: Django :: 2.2',
+        'Framework :: Django :: 3.0',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Natural Language :: English',
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
     ],
 )
```

### Comparing `django-restricted-sessions-0.2.0/restrictedsessions/middleware.py` & `django-restricted-sessions-0.3.0/restrictedsessions/middleware.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 from netaddr import IPNetwork, IPAddress, AddrConversionError, AddrFormatError
 import logging
 
 from django.conf import settings
 from django.http import HttpResponse
-from django.core.urlresolvers import reverse
+from django.urls import reverse
 from django.shortcuts import redirect
 from django.utils.encoding import force_text
 
 try:
     from django.utils.deprecation import MiddlewareMixin
 except ImportError:
     MiddlewareMixin = object
@@ -26,20 +26,22 @@
         if not hasattr(request, 'session'):
             return
 
         # Short circuit for option to require authed users
         if getattr(settings, 'RESTRICTEDSESSIONS_AUTHED_ONLY', False):
             user = getattr(request, 'user', None)
             # No logged in user -- ignore checks
-            if not user or not hasattr(user, 'is_authenticated') or not user.is_authenticated():
+            if not user or not hasattr(user, 'is_authenticated') or not user.is_authenticated:
                 return
 
         # Extract remote IP address for validation purposes
         remote_addr_key = getattr(settings, 'RESTRICTEDSESSIONS_REMOTE_ADDR_KEY', 'REMOTE_ADDR')
         remote_addr = request.META.get(remote_addr_key)
+        if remote_addr:
+            remote_addr = remote_addr.split(',')[0]
 
         # Clear the session and handle response when request doesn't validate
         if not self.validate_ip(request, remote_addr) or not self.validate_ua(request):
             if getattr(settings, 'RESTRICTEDSESSIONS_AUTHED_ONLY', False):
                 from django.contrib.auth import logout
                 logout(request)
             else:  # logout(...) flushes the session so ensure it only happens once
```

### Comparing `django-restricted-sessions-0.2.0/django_restricted_sessions.egg-info/PKG-INFO` & `django-restricted-sessions-0.3.0/django_restricted_sessions.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 1.1
 Name: django-restricted-sessions
-Version: 0.2.0
+Version: 0.3.0
 Summary: Restrict Django sessions to IP and/or user agent.
-Home-page: https://github.com/erikr/django-restricted-sessions
+Home-page: https://github.com/mxsasha/django-restricted-sessions
 Author: django-restricted-sessions
-Author-email: eromijn@solidlinks.nl
+Author-email: github@mxsasha.eu
 License: BSD
 Description: =============================
         django-restricted-sessions
         =============================
         
         .. image:: https://badge.fury.io/py/django-restricted-sessions.png
             :target: http://badge.fury.io/py/django-restricted-sessions
         
-        .. image:: https://travis-ci.org/erikr/django-restricted-sessions.png?branch=master
-            :target: https://travis-ci.org/erikr/django-restricted-sessions
+        .. image:: https://travis-ci.org/mxsasha/django-restricted-sessions.png?branch=master
+            :target: https://travis-ci.org/mxsasha/django-restricted-sessions
         
-        .. image:: https://coveralls.io/repos/erikr/django-restricted-sessions/badge.png?branch=master&
-            :target: https://coveralls.io/r/erikr/django-restricted-sessions?branch=master
+        .. image:: https://coveralls.io/repos/mxsasha/django-restricted-sessions/badge.png?branch=master&
+            :target: https://coveralls.io/r/mxsasha/django-restricted-sessions?branch=master
         
         Restricts Django sessions to IP and/or user agent.
         
         If the IP or user agent changes after creating the session, the a 400 response is given to the request, the session is
         flushed (all session data deleted, new session created) and a warning is logged. The goal of this middleware is to
         make it harder for an attacker to use a session ID they obtained. It does not make abuse of session IDs impossible.
         
@@ -54,14 +54,20 @@
         
         
         
         
         History
         -------
         
+        0.3.0 (2019-12-03)
+        ++++++++++++++++++
+        
+        * Updated Django support to 1.11, 2.2 and 3.0.
+        * Fixed issues when ``X_FORWARDED_FOR`` contains multiple addresses.
+        
         0.2.0 (2017-04-06)
         ++++++++++++++++++
         
         * For Django 1.10+ support, changed from `object` to `django.utils.deprecation.MiddlewareMixin`
         * Added PyPI trove classifiers for Django versions and more Python versions
         * Updated `travis.yml` for more Python versions
         
@@ -101,19 +107,19 @@
         
         * First release on PyPI.
         
 Keywords: django-restricted-sessions
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 1.8
-Classifier: Framework :: Django :: 1.10
 Classifier: Framework :: Django :: 1.11
+Classifier: Framework :: Django :: 2.2
+Classifier: Framework :: Django :: 3.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
```

