# Comparing `tmp/MarkupSafe-2.1.2.tar.gz` & `tmp/MarkupSafe-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MarkupSafe-2.1.2.tar", last modified: Tue Jan 17 17:52:09 2023, max compression
+gzip compressed data, was "MarkupSafe-2.1.3.tar", last modified: Fri Jun  2 21:13:25 2023, max compression
```

## Comparing `MarkupSafe-2.1.2.tar` & `MarkupSafe-2.1.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 17:52:09.244761 MarkupSafe-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-01-17 17:51:51.000000 MarkupSafe-2.1.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-01-17 17:51:51.000000 MarkupSafe-2.1.2/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-01-17 17:51:51.000000 MarkupSafe-2.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-01-17 17:52:09.244761 MarkupSafe-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-01-17 17:51:51.000000 MarkupSafe-2.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 17:52:09.236761 MarkupSafe-2.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-01-17 17:51:51.000000 MarkupSafe-2.1.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-01-17 17:51:51.000000 MarkupSafe-2.1.2/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-01-17 17:51:51.000000 MarkupSafe-2.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-01-17 17:51:51.000000 MarkupSafe-2.1.2/docs/escaping.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-01-17 17:51:51.000000 MarkupSafe-2.1.2/docs/formatting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-01-17 17:51:51.000000 MarkupSafe-2.1.2/docs/html.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-01-17 17:51:51.000000 MarkupSafe-2.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-01-17 17:51:51.000000 MarkupSafe-2.1.2/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-01-17 17:51:51.000000 MarkupSafe-2.1.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 17:52:09.240761 MarkupSafe-2.1.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-01-17 17:51:51.000000 MarkupSafe-2.1.2/requirements/build.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-01-17 17:51:51.000000 MarkupSafe-2.1.2/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-01-17 17:51:51.000000 MarkupSafe-2.1.2/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-01-17 17:51:51.000000 MarkupSafe-2.1.2/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-01-17 17:51:51.000000 MarkupSafe-2.1.2/requirements/typing.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-01-17 17:52:09.248761 MarkupSafe-2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-01-17 17:51:51.000000 MarkupSafe-2.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 17:52:09.228761 MarkupSafe-2.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 17:52:09.240761 MarkupSafe-2.1.2/src/MarkupSafe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-01-17 17:52:09.000000 MarkupSafe-2.1.2/src/MarkupSafe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-01-17 17:52:09.000000 MarkupSafe-2.1.2/src/MarkupSafe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 17:52:09.000000 MarkupSafe-2.1.2/src/MarkupSafe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-17 17:52:09.000000 MarkupSafe-2.1.2/src/MarkupSafe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 17:52:09.244761 MarkupSafe-2.1.2/src/markupsafe/
--rw-r--r--   0 runner    (1001) docker     (123)     9306 2023-01-17 17:51:51.000000 MarkupSafe-2.1.2/src/markupsafe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-01-17 17:51:51.000000 MarkupSafe-2.1.2/src/markupsafe/_native.py
--rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-01-17 17:51:51.000000 MarkupSafe-2.1.2/src/markupsafe/_speedups.c
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-01-17 17:51:51.000000 MarkupSafe-2.1.2/src/markupsafe/_speedups.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 17:51:51.000000 MarkupSafe-2.1.2/src/markupsafe/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 17:52:09.244761 MarkupSafe-2.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-01-17 17:51:51.000000 MarkupSafe-2.1.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-01-17 17:51:51.000000 MarkupSafe-2.1.2/tests/test_escape.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-01-17 17:51:51.000000 MarkupSafe-2.1.2/tests/test_exception_custom_html.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-01-17 17:51:51.000000 MarkupSafe-2.1.2/tests/test_leak.py
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-01-17 17:51:51.000000 MarkupSafe-2.1.2/tests/test_markupsafe.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-01-17 17:51:51.000000 MarkupSafe-2.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:13:25.750226 MarkupSafe-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-02 21:13:16.000000 MarkupSafe-2.1.3/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-02 21:13:16.000000 MarkupSafe-2.1.3/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-02 21:13:16.000000 MarkupSafe-2.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-06-02 21:13:25.750226 MarkupSafe-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-02 21:13:16.000000 MarkupSafe-2.1.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:13:25.750226 MarkupSafe-2.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-02 21:13:16.000000 MarkupSafe-2.1.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-02 21:13:16.000000 MarkupSafe-2.1.3/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-02 21:13:16.000000 MarkupSafe-2.1.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-02 21:13:16.000000 MarkupSafe-2.1.3/docs/escaping.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-02 21:13:16.000000 MarkupSafe-2.1.3/docs/formatting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-02 21:13:16.000000 MarkupSafe-2.1.3/docs/html.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-02 21:13:16.000000 MarkupSafe-2.1.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-02 21:13:16.000000 MarkupSafe-2.1.3/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-02 21:13:16.000000 MarkupSafe-2.1.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:13:25.750226 MarkupSafe-2.1.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-02 21:13:16.000000 MarkupSafe-2.1.3/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-02 21:13:16.000000 MarkupSafe-2.1.3/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-02 21:13:16.000000 MarkupSafe-2.1.3/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-02 21:13:16.000000 MarkupSafe-2.1.3/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-02 21:13:16.000000 MarkupSafe-2.1.3/requirements/typing.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-02 21:13:25.754227 MarkupSafe-2.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-02 21:13:16.000000 MarkupSafe-2.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:13:25.746226 MarkupSafe-2.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:13:25.750226 MarkupSafe-2.1.3/src/MarkupSafe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-06-02 21:13:25.000000 MarkupSafe-2.1.3/src/MarkupSafe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-02 21:13:25.000000 MarkupSafe-2.1.3/src/MarkupSafe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 21:13:25.000000 MarkupSafe-2.1.3/src/MarkupSafe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-02 21:13:25.000000 MarkupSafe-2.1.3/src/MarkupSafe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:13:25.750226 MarkupSafe-2.1.3/src/markupsafe/
+-rw-r--r--   0 runner    (1001) docker     (123)    10338 2023-06-02 21:13:16.000000 MarkupSafe-2.1.3/src/markupsafe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-02 21:13:16.000000 MarkupSafe-2.1.3/src/markupsafe/_native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-06-02 21:13:16.000000 MarkupSafe-2.1.3/src/markupsafe/_speedups.c
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-02 21:13:16.000000 MarkupSafe-2.1.3/src/markupsafe/_speedups.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 21:13:16.000000 MarkupSafe-2.1.3/src/markupsafe/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:13:25.750226 MarkupSafe-2.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-02 21:13:16.000000 MarkupSafe-2.1.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-02 21:13:16.000000 MarkupSafe-2.1.3/tests/test_escape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-02 21:13:16.000000 MarkupSafe-2.1.3/tests/test_exception_custom_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-02 21:13:16.000000 MarkupSafe-2.1.3/tests/test_leak.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-06-02 21:13:16.000000 MarkupSafe-2.1.3/tests/test_markupsafe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-02 21:13:16.000000 MarkupSafe-2.1.3/tox.ini
```

### Comparing `MarkupSafe-2.1.2/CHANGES.rst` & `MarkupSafe-2.1.3/CHANGES.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Version 2.1.3
+-------------
+
+Released 2023-06-02
+
+-   Implement ``format_map``, ``casefold``, ``removeprefix``, and ``removesuffix``
+    methods. :issue:`370`
+-   Fix static typing for basic ``str`` methods on ``Markup``. :issue:`358`
+-   Use ``Self`` for annotating return types. :pr:`379`
+
+
 Version 2.1.2
 -------------
 
 Released 2023-01-17
 
 -   Fix ``striptags`` not stripping tags containing newlines.
     :issue:`310`
```

### Comparing `MarkupSafe-2.1.2/LICENSE.rst` & `MarkupSafe-2.1.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `MarkupSafe-2.1.2/PKG-INFO` & `MarkupSafe-2.1.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
 Name: MarkupSafe
-Version: 2.1.2
+Version: 2.1.3
 Summary: Safely add untrusted strings to HTML/XML markup.
 Home-page: https://palletsprojects.com/p/markupsafe/
-Author: Armin Ronacher
-Author-email: armin.ronacher@active-4.com
 Maintainer: Pallets
 Maintainer-email: contact@palletsprojects.com
 License: BSD-3-Clause
 Project-URL: Donate, https://palletsprojects.com/donate
 Project-URL: Documentation, https://markupsafe.palletsprojects.com/
 Project-URL: Changes, https://markupsafe.palletsprojects.com/changes/
 Project-URL: Source Code, https://github.com/pallets/markupsafe/
 Project-URL: Issue Tracker, https://github.com/pallets/markupsafe/issues/
-Project-URL: Twitter, https://twitter.com/PalletsTeam
 Project-URL: Chat, https://discord.gg/pallets
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -89,10 +86,8 @@
 -----
 
 -   Documentation: https://markupsafe.palletsprojects.com/
 -   Changes: https://markupsafe.palletsprojects.com/changes/
 -   PyPI Releases: https://pypi.org/project/MarkupSafe/
 -   Source Code: https://github.com/pallets/markupsafe/
 -   Issue Tracker: https://github.com/pallets/markupsafe/issues/
--   Website: https://palletsprojects.com/p/markupsafe/
--   Twitter: https://twitter.com/PalletsTeam
 -   Chat: https://discord.gg/pallets
```

#### html2text {}

```diff
@@ -1,40 +1,37 @@
-Metadata-Version: 2.1 Name: MarkupSafe Version: 2.1.2 Summary: Safely add
+Metadata-Version: 2.1 Name: MarkupSafe Version: 2.1.3 Summary: Safely add
 untrusted strings to HTML/XML markup. Home-page: https://palletsprojects.com/p/
-markupsafe/ Author: Armin Ronacher Author-email: armin.ronacher@active-4.com
-Maintainer: Pallets Maintainer-email: contact@palletsprojects.com License: BSD-
-3-Clause Project-URL: Donate, https://palletsprojects.com/donate Project-URL:
-Documentation, https://markupsafe.palletsprojects.com/ Project-URL: Changes,
-https://markupsafe.palletsprojects.com/changes/ Project-URL: Source Code,
-https://github.com/pallets/markupsafe/ Project-URL: Issue Tracker, https://
-github.com/pallets/markupsafe/issues/ Project-URL: Twitter, https://
-twitter.com/PalletsTeam Project-URL: Chat, https://discord.gg/pallets
-Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
-:: Web Environment Classifier: Intended Audience :: Developers Classifier:
-License :: OSI Approved :: BSD License Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python Classifier: Topic ::
-Internet :: WWW/HTTP :: Dynamic Content Classifier: Topic :: Text Processing ::
-Markup :: HTML Requires-Python: >=3.7 Description-Content-Type: text/x-rst
-License-File: LICENSE.rst MarkupSafe ========== MarkupSafe implements a text
-object that escapes characters so it is safe to use in HTML and XML. Characters
-that have special meanings are replaced so that they display as the actual
-characters. This mitigates injection attacks, meaning untrusted user input can
-safely be displayed on a page. Installing ---------- Install and update using
-`pip`_: .. code-block:: text pip install -U MarkupSafe .. _pip: https://
-pip.pypa.io/en/stable/getting-started/ Examples -------- .. code-block:: pycon
->>> from markupsafe import Markup, escape >>> # escape replaces special
-characters and wraps in Markup >>> escape("
+markupsafe/ Maintainer: Pallets Maintainer-email: contact@palletsprojects.com
+License: BSD-3-Clause Project-URL: Donate, https://palletsprojects.com/donate
+Project-URL: Documentation, https://markupsafe.palletsprojects.com/ Project-
+URL: Changes, https://markupsafe.palletsprojects.com/changes/ Project-URL:
+Source Code, https://github.com/pallets/markupsafe/ Project-URL: Issue Tracker,
+https://github.com/pallets/markupsafe/issues/ Project-URL: Chat, https://
+discord.gg/pallets Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment Classifier: Intended Audience ::
+Developers Classifier: License :: OSI Approved :: BSD License Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content Classifier: Topic
+:: Text Processing :: Markup :: HTML Requires-Python: >=3.7 Description-
+Content-Type: text/x-rst License-File: LICENSE.rst MarkupSafe ==========
+MarkupSafe implements a text object that escapes characters so it is safe to
+use in HTML and XML. Characters that have special meanings are replaced so that
+they display as the actual characters. This mitigates injection attacks,
+meaning untrusted user input can safely be displayed on a page. Installing ----
+------ Install and update using `pip`_: .. code-block:: text pip install -
+U MarkupSafe .. _pip: https://pip.pypa.io/en/stable/getting-started/ Examples -
+------- .. code-block:: pycon >>> from markupsafe import Markup, escape >>> #
+escape replaces special characters and wraps in Markup >>> escape("
 ") Markup('<script>alert(document.cookie);</script>') >>> # wrap in Markup to
 mark text "safe" and prevent escaping >>> Markup("Hello") Markup('hello') >>>
 escape(Markup("Hello")) Markup('hello') >>> # Markup is a str subclass >>> #
 methods and operators escape their arguments >>> template = Markup("Hello
 {name}") >>> template.format(name='"World"') Markup('Hello "World"') Donate ---
 --- The Pallets organization develops and supports MarkupSafe and other popular
 packages. In order to grow the community of contributors and users, and allow
 the maintainers to devote more time to the projects, `please donate today`_. ..
 _please donate today: https://palletsprojects.com/donate Links ----- -
 Documentation: https://markupsafe.palletsprojects.com/ - Changes: https://
 markupsafe.palletsprojects.com/changes/ - PyPI Releases: https://pypi.org/
 project/MarkupSafe/ - Source Code: https://github.com/pallets/markupsafe/ -
-Issue Tracker: https://github.com/pallets/markupsafe/issues/ - Website: https:/
-/palletsprojects.com/p/markupsafe/ - Twitter: https://twitter.com/PalletsTeam -
-Chat: https://discord.gg/pallets
+Issue Tracker: https://github.com/pallets/markupsafe/issues/ - Chat: https://
+discord.gg/pallets
```

### Comparing `MarkupSafe-2.1.2/README.rst` & `MarkupSafe-2.1.3/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -60,10 +60,8 @@
 -----
 
 -   Documentation: https://markupsafe.palletsprojects.com/
 -   Changes: https://markupsafe.palletsprojects.com/changes/
 -   PyPI Releases: https://pypi.org/project/MarkupSafe/
 -   Source Code: https://github.com/pallets/markupsafe/
 -   Issue Tracker: https://github.com/pallets/markupsafe/issues/
--   Website: https://palletsprojects.com/p/markupsafe/
--   Twitter: https://twitter.com/PalletsTeam
 -   Chat: https://discord.gg/pallets
```

#### html2text {}

```diff
@@ -15,10 +15,9 @@
 --- The Pallets organization develops and supports MarkupSafe and other popular
 packages. In order to grow the community of contributors and users, and allow
 the maintainers to devote more time to the projects, `please donate today`_. ..
 _please donate today: https://palletsprojects.com/donate Links ----- -
 Documentation: https://markupsafe.palletsprojects.com/ - Changes: https://
 markupsafe.palletsprojects.com/changes/ - PyPI Releases: https://pypi.org/
 project/MarkupSafe/ - Source Code: https://github.com/pallets/markupsafe/ -
-Issue Tracker: https://github.com/pallets/markupsafe/issues/ - Website: https:/
-/palletsprojects.com/p/markupsafe/ - Twitter: https://twitter.com/PalletsTeam -
-Chat: https://discord.gg/pallets
+Issue Tracker: https://github.com/pallets/markupsafe/issues/ - Chat: https://
+discord.gg/pallets
```

### Comparing `MarkupSafe-2.1.2/docs/Makefile` & `MarkupSafe-2.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `MarkupSafe-2.1.2/docs/conf.py` & `MarkupSafe-2.1.3/docs/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,16 +28,14 @@
 html_theme_options = {"index_sidebar_logo": False}
 html_context = {
     "project_links": [
         ProjectLink("Donate", "https://palletsprojects.com/donate"),
         ProjectLink("PyPI Releases", "https://pypi.org/project/MarkupSafe/"),
         ProjectLink("Source Code", "https://github.com/pallets/markupsafe/"),
         ProjectLink("Issue Tracker", "https://github.com/pallets/markupsafe/issues/"),
-        ProjectLink("Website", "https://palletsprojects.com/p/markupsafe/"),
-        ProjectLink("Twitter", "https://twitter.com/PalletsTeam"),
         ProjectLink("Chat", "https://discord.gg/pallets"),
     ]
 }
 html_sidebars = {
     "index": ["project.html", "localtoc.html", "searchbox.html", "ethicalads.html"],
     "**": ["localtoc.html", "relations.html", "searchbox.html", "ethicalads.html"],
 }
```

### Comparing `MarkupSafe-2.1.2/docs/formatting.rst` & `MarkupSafe-2.1.3/docs/formatting.rst`

 * *Files identical despite different names*

### Comparing `MarkupSafe-2.1.2/docs/html.rst` & `MarkupSafe-2.1.3/docs/html.rst`

 * *Files identical despite different names*

### Comparing `MarkupSafe-2.1.2/docs/index.rst` & `MarkupSafe-2.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `MarkupSafe-2.1.2/docs/make.bat` & `MarkupSafe-2.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `MarkupSafe-2.1.2/requirements/dev.txt` & `MarkupSafe-2.1.3/requirements/dev.txt`

 * *Files 23% similar despite different names*

```diff
@@ -4,61 +4,61 @@
 # To update, run:
 #
 #    pip-compile-multi
 #
 -r docs.txt
 -r tests.txt
 -r typing.txt
-build==0.9.0
+build==0.10.0
     # via pip-tools
-cachetools==5.2.0
+cachetools==5.3.1
     # via tox
 cfgv==3.3.1
     # via pre-commit
 chardet==5.1.0
     # via tox
 click==8.1.3
     # via
     #   pip-compile-multi
     #   pip-tools
 colorama==0.4.6
     # via tox
 distlib==0.3.6
     # via virtualenv
-filelock==3.9.0
+filelock==3.12.0
     # via
     #   tox
     #   virtualenv
-identify==2.5.11
+identify==2.5.24
     # via pre-commit
-nodeenv==1.7.0
+nodeenv==1.8.0
     # via pre-commit
-pep517==0.13.0
-    # via build
-pip-compile-multi==2.6.1
+pip-compile-multi==2.6.3
     # via -r requirements/dev.in
-pip-tools==6.12.1
+pip-tools==6.13.0
     # via pip-compile-multi
-platformdirs==2.6.2
+platformdirs==3.5.1
     # via
     #   tox
     #   virtualenv
-pre-commit==2.21.0
+pre-commit==3.3.2
     # via -r requirements/dev.in
-pyproject-api==1.2.1
+pyproject-api==1.5.1
     # via tox
+pyproject-hooks==1.0.0
+    # via build
 pyyaml==6.0
     # via pre-commit
-toposort==1.7
+toposort==1.10
     # via pip-compile-multi
-tox==4.1.0
+tox==4.5.2
     # via -r requirements/dev.in
-virtualenv==20.17.1
+virtualenv==20.23.0
     # via
     #   pre-commit
     #   tox
-wheel==0.38.4
+wheel==0.40.0
     # via pip-tools
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `MarkupSafe-2.1.2/requirements/docs.txt` & `MarkupSafe-2.1.3/requirements/docs.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,61 @@
 # SHA1:45c590f97fe95b8bdc755eef796e91adf5fbe4ea
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
-alabaster==0.7.12
+alabaster==0.7.13
     # via sphinx
-babel==2.11.0
+babel==2.12.1
     # via sphinx
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
-charset-normalizer==2.1.1
+charset-normalizer==3.1.0
     # via requests
-docutils==0.19
+docutils==0.20.1
     # via sphinx
 idna==3.4
     # via requests
 imagesize==1.4.1
     # via sphinx
 jinja2==3.1.2
     # via sphinx
-markupsafe==2.1.1
+markupsafe==2.1.2
     # via jinja2
-packaging==22.0
+packaging==23.1
     # via
     #   pallets-sphinx-themes
     #   sphinx
-pallets-sphinx-themes==2.0.3
+pallets-sphinx-themes==2.1.0
     # via -r requirements/docs.in
-pygments==2.13.0
+pygments==2.15.1
     # via sphinx
-pytz==2022.7
-    # via babel
-requests==2.28.1
+requests==2.31.0
     # via sphinx
 snowballstemmer==2.2.0
     # via sphinx
-sphinx==6.0.0
+sphinx==7.0.1
     # via
     #   -r requirements/docs.in
     #   pallets-sphinx-themes
     #   sphinx-issues
     #   sphinxcontrib-log-cabinet
 sphinx-issues==3.0.1
     # via -r requirements/docs.in
-sphinxcontrib-applehelp==1.0.2
+sphinxcontrib-applehelp==1.0.4
     # via sphinx
 sphinxcontrib-devhelp==1.0.2
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.0
+sphinxcontrib-htmlhelp==2.0.1
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-log-cabinet==1.0.1
     # via -r requirements/docs.in
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
-urllib3==1.26.13
+urllib3==2.0.2
     # via requests
```

### Comparing `MarkupSafe-2.1.2/setup.cfg` & `MarkupSafe-2.1.3/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,17 @@
 url = https://palletsprojects.com/p/markupsafe/
 project_urls = 
 	Donate = https://palletsprojects.com/donate
 	Documentation = https://markupsafe.palletsprojects.com/
 	Changes = https://markupsafe.palletsprojects.com/changes/
 	Source Code = https://github.com/pallets/markupsafe/
 	Issue Tracker = https://github.com/pallets/markupsafe/issues/
-	Twitter = https://twitter.com/PalletsTeam
 	Chat = https://discord.gg/pallets
 license = BSD-3-Clause
 license_files = LICENSE.rst
-author = Armin Ronacher
-author_email = armin.ronacher@active-4.com
 maintainer = Pallets
 maintainer_email = contact@palletsprojects.com
 description = Safely add untrusted strings to HTML/XML markup.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 classifiers = 
 	Development Status :: 5 - Production/Stable
@@ -38,14 +35,15 @@
 [options.packages.find]
 where = src
 
 [tool:pytest]
 testpaths = tests
 filterwarnings = 
 	error
+	ignore:ast:DeprecationWarning
 
 [coverage:run]
 branch = True
 source = 
 	markupsafe
 	tests
```

### Comparing `MarkupSafe-2.1.2/setup.py` & `MarkupSafe-2.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `MarkupSafe-2.1.2/src/MarkupSafe.egg-info/PKG-INFO` & `MarkupSafe-2.1.3/src/MarkupSafe.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
 Name: MarkupSafe
-Version: 2.1.2
+Version: 2.1.3
 Summary: Safely add untrusted strings to HTML/XML markup.
 Home-page: https://palletsprojects.com/p/markupsafe/
-Author: Armin Ronacher
-Author-email: armin.ronacher@active-4.com
 Maintainer: Pallets
 Maintainer-email: contact@palletsprojects.com
 License: BSD-3-Clause
 Project-URL: Donate, https://palletsprojects.com/donate
 Project-URL: Documentation, https://markupsafe.palletsprojects.com/
 Project-URL: Changes, https://markupsafe.palletsprojects.com/changes/
 Project-URL: Source Code, https://github.com/pallets/markupsafe/
 Project-URL: Issue Tracker, https://github.com/pallets/markupsafe/issues/
-Project-URL: Twitter, https://twitter.com/PalletsTeam
 Project-URL: Chat, https://discord.gg/pallets
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -89,10 +86,8 @@
 -----
 
 -   Documentation: https://markupsafe.palletsprojects.com/
 -   Changes: https://markupsafe.palletsprojects.com/changes/
 -   PyPI Releases: https://pypi.org/project/MarkupSafe/
 -   Source Code: https://github.com/pallets/markupsafe/
 -   Issue Tracker: https://github.com/pallets/markupsafe/issues/
--   Website: https://palletsprojects.com/p/markupsafe/
--   Twitter: https://twitter.com/PalletsTeam
 -   Chat: https://discord.gg/pallets
```

#### html2text {}

```diff
@@ -1,40 +1,37 @@
-Metadata-Version: 2.1 Name: MarkupSafe Version: 2.1.2 Summary: Safely add
+Metadata-Version: 2.1 Name: MarkupSafe Version: 2.1.3 Summary: Safely add
 untrusted strings to HTML/XML markup. Home-page: https://palletsprojects.com/p/
-markupsafe/ Author: Armin Ronacher Author-email: armin.ronacher@active-4.com
-Maintainer: Pallets Maintainer-email: contact@palletsprojects.com License: BSD-
-3-Clause Project-URL: Donate, https://palletsprojects.com/donate Project-URL:
-Documentation, https://markupsafe.palletsprojects.com/ Project-URL: Changes,
-https://markupsafe.palletsprojects.com/changes/ Project-URL: Source Code,
-https://github.com/pallets/markupsafe/ Project-URL: Issue Tracker, https://
-github.com/pallets/markupsafe/issues/ Project-URL: Twitter, https://
-twitter.com/PalletsTeam Project-URL: Chat, https://discord.gg/pallets
-Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
-:: Web Environment Classifier: Intended Audience :: Developers Classifier:
-License :: OSI Approved :: BSD License Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python Classifier: Topic ::
-Internet :: WWW/HTTP :: Dynamic Content Classifier: Topic :: Text Processing ::
-Markup :: HTML Requires-Python: >=3.7 Description-Content-Type: text/x-rst
-License-File: LICENSE.rst MarkupSafe ========== MarkupSafe implements a text
-object that escapes characters so it is safe to use in HTML and XML. Characters
-that have special meanings are replaced so that they display as the actual
-characters. This mitigates injection attacks, meaning untrusted user input can
-safely be displayed on a page. Installing ---------- Install and update using
-`pip`_: .. code-block:: text pip install -U MarkupSafe .. _pip: https://
-pip.pypa.io/en/stable/getting-started/ Examples -------- .. code-block:: pycon
->>> from markupsafe import Markup, escape >>> # escape replaces special
-characters and wraps in Markup >>> escape("
+markupsafe/ Maintainer: Pallets Maintainer-email: contact@palletsprojects.com
+License: BSD-3-Clause Project-URL: Donate, https://palletsprojects.com/donate
+Project-URL: Documentation, https://markupsafe.palletsprojects.com/ Project-
+URL: Changes, https://markupsafe.palletsprojects.com/changes/ Project-URL:
+Source Code, https://github.com/pallets/markupsafe/ Project-URL: Issue Tracker,
+https://github.com/pallets/markupsafe/issues/ Project-URL: Chat, https://
+discord.gg/pallets Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment Classifier: Intended Audience ::
+Developers Classifier: License :: OSI Approved :: BSD License Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content Classifier: Topic
+:: Text Processing :: Markup :: HTML Requires-Python: >=3.7 Description-
+Content-Type: text/x-rst License-File: LICENSE.rst MarkupSafe ==========
+MarkupSafe implements a text object that escapes characters so it is safe to
+use in HTML and XML. Characters that have special meanings are replaced so that
+they display as the actual characters. This mitigates injection attacks,
+meaning untrusted user input can safely be displayed on a page. Installing ----
+------ Install and update using `pip`_: .. code-block:: text pip install -
+U MarkupSafe .. _pip: https://pip.pypa.io/en/stable/getting-started/ Examples -
+------- .. code-block:: pycon >>> from markupsafe import Markup, escape >>> #
+escape replaces special characters and wraps in Markup >>> escape("
 ") Markup('<script>alert(document.cookie);</script>') >>> # wrap in Markup to
 mark text "safe" and prevent escaping >>> Markup("Hello") Markup('hello') >>>
 escape(Markup("Hello")) Markup('hello') >>> # Markup is a str subclass >>> #
 methods and operators escape their arguments >>> template = Markup("Hello
 {name}") >>> template.format(name='"World"') Markup('Hello "World"') Donate ---
 --- The Pallets organization develops and supports MarkupSafe and other popular
 packages. In order to grow the community of contributors and users, and allow
 the maintainers to devote more time to the projects, `please donate today`_. ..
 _please donate today: https://palletsprojects.com/donate Links ----- -
 Documentation: https://markupsafe.palletsprojects.com/ - Changes: https://
 markupsafe.palletsprojects.com/changes/ - PyPI Releases: https://pypi.org/
 project/MarkupSafe/ - Source Code: https://github.com/pallets/markupsafe/ -
-Issue Tracker: https://github.com/pallets/markupsafe/issues/ - Website: https:/
-/palletsprojects.com/p/markupsafe/ - Twitter: https://twitter.com/PalletsTeam -
-Chat: https://discord.gg/pallets
+Issue Tracker: https://github.com/pallets/markupsafe/issues/ - Chat: https://
+discord.gg/pallets
```

### Comparing `MarkupSafe-2.1.2/src/MarkupSafe.egg-info/SOURCES.txt` & `MarkupSafe-2.1.3/src/MarkupSafe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MarkupSafe-2.1.2/src/markupsafe/__init__.py` & `MarkupSafe-2.1.3/src/markupsafe/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 import functools
 import re
 import string
+import sys
 import typing as t
 
 if t.TYPE_CHECKING:
     import typing_extensions as te
 
     class HasHTML(te.Protocol):
         def __html__(self) -> str:
             pass
 
+    _P = te.ParamSpec("_P")
 
-__version__ = "2.1.2"
+
+__version__ = "2.1.3"
 
 _strip_comments_re = re.compile(r"<!--.*?-->", re.DOTALL)
 _strip_tags_re = re.compile(r"<.*?>", re.DOTALL)
 
 
-def _simple_escaping_wrapper(name: str) -> t.Callable[..., "Markup"]:
-    orig = getattr(str, name)
-
-    @functools.wraps(orig)
-    def wrapped(self: "Markup", *args: t.Any, **kwargs: t.Any) -> "Markup":
-        args = _escape_argspec(list(args), enumerate(args), self.escape)  # type: ignore
+def _simple_escaping_wrapper(func: "t.Callable[_P, str]") -> "t.Callable[_P, Markup]":
+    @functools.wraps(func)
+    def wrapped(self: "Markup", *args: "_P.args", **kwargs: "_P.kwargs") -> "Markup":
+        arg_list = _escape_argspec(list(args), enumerate(args), self.escape)
         _escape_argspec(kwargs, kwargs.items(), self.escape)
-        return self.__class__(orig(self, *args, **kwargs))
+        return self.__class__(func(self, *arg_list, **kwargs))  # type: ignore[arg-type]
 
-    return wrapped
+    return wrapped  # type: ignore[return-value]
 
 
 class Markup(str):
     """A string that is ready to be safely inserted into an HTML or XML
     document, either because it was escaped or because it was marked
     safe.
 
@@ -65,47 +66,47 @@
     Markup('<em>Hello</em> &lt;foo&gt;')
     """
 
     __slots__ = ()
 
     def __new__(
         cls, base: t.Any = "", encoding: t.Optional[str] = None, errors: str = "strict"
-    ) -> "Markup":
+    ) -> "te.Self":
         if hasattr(base, "__html__"):
             base = base.__html__()
 
         if encoding is None:
             return super().__new__(cls, base)
 
         return super().__new__(cls, base, encoding, errors)
 
-    def __html__(self) -> "Markup":
+    def __html__(self) -> "te.Self":
         return self
 
-    def __add__(self, other: t.Union[str, "HasHTML"]) -> "Markup":
+    def __add__(self, other: t.Union[str, "HasHTML"]) -> "te.Self":
         if isinstance(other, str) or hasattr(other, "__html__"):
             return self.__class__(super().__add__(self.escape(other)))
 
         return NotImplemented
 
-    def __radd__(self, other: t.Union[str, "HasHTML"]) -> "Markup":
+    def __radd__(self, other: t.Union[str, "HasHTML"]) -> "te.Self":
         if isinstance(other, str) or hasattr(other, "__html__"):
             return self.escape(other).__add__(self)
 
         return NotImplemented
 
-    def __mul__(self, num: "te.SupportsIndex") -> "Markup":
+    def __mul__(self, num: "te.SupportsIndex") -> "te.Self":
         if isinstance(num, int):
             return self.__class__(super().__mul__(num))
 
         return NotImplemented
 
     __rmul__ = __mul__
 
-    def __mod__(self, arg: t.Any) -> "Markup":
+    def __mod__(self, arg: t.Any) -> "te.Self":
         if isinstance(arg, tuple):
             # a tuple of arguments, each wrapped
             arg = tuple(_MarkupEscapeHelper(x, self.escape) for x in arg)
         elif hasattr(type(arg), "__getitem__") and not isinstance(arg, str):
             # a mapping of arguments, wrapped
             arg = _MarkupEscapeHelper(arg, self.escape)
         else:
@@ -113,34 +114,36 @@
             arg = (_MarkupEscapeHelper(arg, self.escape),)
 
         return self.__class__(super().__mod__(arg))
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({super().__repr__()})"
 
-    def join(self, seq: t.Iterable[t.Union[str, "HasHTML"]]) -> "Markup":
+    def join(self, seq: t.Iterable[t.Union[str, "HasHTML"]]) -> "te.Self":
         return self.__class__(super().join(map(self.escape, seq)))
 
     join.__doc__ = str.join.__doc__
 
-    def split(  # type: ignore
+    def split(  # type: ignore[override]
         self, sep: t.Optional[str] = None, maxsplit: int = -1
-    ) -> t.List["Markup"]:
+    ) -> t.List["te.Self"]:
         return [self.__class__(v) for v in super().split(sep, maxsplit)]
 
     split.__doc__ = str.split.__doc__
 
-    def rsplit(  # type: ignore
+    def rsplit(  # type: ignore[override]
         self, sep: t.Optional[str] = None, maxsplit: int = -1
-    ) -> t.List["Markup"]:
+    ) -> t.List["te.Self"]:
         return [self.__class__(v) for v in super().rsplit(sep, maxsplit)]
 
     rsplit.__doc__ = str.rsplit.__doc__
 
-    def splitlines(self, keepends: bool = False) -> t.List["Markup"]:  # type: ignore
+    def splitlines(  # type: ignore[override]
+        self, keepends: bool = False
+    ) -> t.List["te.Self"]:
         return [self.__class__(v) for v in super().splitlines(keepends)]
 
     splitlines.__doc__ = str.splitlines.__doc__
 
     def unescape(self) -> str:
         """Convert escaped markup back into a text string. This replaces
         HTML entities with the characters they represent.
@@ -159,65 +162,71 @@
         >>> Markup("Main &raquo;\t<em>About</em>").striptags()
         'Main » About'
         """
         # Use two regexes to avoid ambiguous matches.
         value = _strip_comments_re.sub("", self)
         value = _strip_tags_re.sub("", value)
         value = " ".join(value.split())
-        return Markup(value).unescape()
+        return self.__class__(value).unescape()
 
     @classmethod
-    def escape(cls, s: t.Any) -> "Markup":
+    def escape(cls, s: t.Any) -> "te.Self":
         """Escape a string. Calls :func:`escape` and ensures that for
         subclasses the correct type is returned.
         """
         rv = escape(s)
 
         if rv.__class__ is not cls:
             return cls(rv)
 
-        return rv
-
-    for method in (
-        "__getitem__",
-        "capitalize",
-        "title",
-        "lower",
-        "upper",
-        "replace",
-        "ljust",
-        "rjust",
-        "lstrip",
-        "rstrip",
-        "center",
-        "strip",
-        "translate",
-        "expandtabs",
-        "swapcase",
-        "zfill",
-    ):
-        locals()[method] = _simple_escaping_wrapper(method)
+        return rv  # type: ignore[return-value]
 
-    del method
+    __getitem__ = _simple_escaping_wrapper(str.__getitem__)
+    capitalize = _simple_escaping_wrapper(str.capitalize)
+    title = _simple_escaping_wrapper(str.title)
+    lower = _simple_escaping_wrapper(str.lower)
+    upper = _simple_escaping_wrapper(str.upper)
+    replace = _simple_escaping_wrapper(str.replace)
+    ljust = _simple_escaping_wrapper(str.ljust)
+    rjust = _simple_escaping_wrapper(str.rjust)
+    lstrip = _simple_escaping_wrapper(str.lstrip)
+    rstrip = _simple_escaping_wrapper(str.rstrip)
+    center = _simple_escaping_wrapper(str.center)
+    strip = _simple_escaping_wrapper(str.strip)
+    translate = _simple_escaping_wrapper(str.translate)
+    expandtabs = _simple_escaping_wrapper(str.expandtabs)
+    swapcase = _simple_escaping_wrapper(str.swapcase)
+    zfill = _simple_escaping_wrapper(str.zfill)
+    casefold = _simple_escaping_wrapper(str.casefold)
+
+    if sys.version_info >= (3, 9):
+        removeprefix = _simple_escaping_wrapper(str.removeprefix)
+        removesuffix = _simple_escaping_wrapper(str.removesuffix)
 
-    def partition(self, sep: str) -> t.Tuple["Markup", "Markup", "Markup"]:
+    def partition(self, sep: str) -> t.Tuple["te.Self", "te.Self", "te.Self"]:
         l, s, r = super().partition(self.escape(sep))
         cls = self.__class__
         return cls(l), cls(s), cls(r)
 
-    def rpartition(self, sep: str) -> t.Tuple["Markup", "Markup", "Markup"]:
+    def rpartition(self, sep: str) -> t.Tuple["te.Self", "te.Self", "te.Self"]:
         l, s, r = super().rpartition(self.escape(sep))
         cls = self.__class__
         return cls(l), cls(s), cls(r)
 
-    def format(self, *args: t.Any, **kwargs: t.Any) -> "Markup":
+    def format(self, *args: t.Any, **kwargs: t.Any) -> "te.Self":
         formatter = EscapeFormatter(self.escape)
         return self.__class__(formatter.vformat(self, args, kwargs))
 
-    def __html_format__(self, format_spec: str) -> "Markup":
+    def format_map(  # type: ignore[override]
+        self, map: t.Mapping[str, t.Any]
+    ) -> "te.Self":
+        formatter = EscapeFormatter(self.escape)
+        return self.__class__(formatter.vformat(self, (), map))
+
+    def __html_format__(self, format_spec: str) -> "te.Self":
         if format_spec:
             raise ValueError("Unsupported format specification for Markup.")
 
         return self
 
 
 class EscapeFormatter(string.Formatter):
@@ -264,16 +273,16 @@
 
     __slots__ = ("obj", "escape")
 
     def __init__(self, obj: t.Any, escape: t.Callable[[t.Any], Markup]) -> None:
         self.obj = obj
         self.escape = escape
 
-    def __getitem__(self, item: t.Any) -> "_MarkupEscapeHelper":
-        return _MarkupEscapeHelper(self.obj[item], self.escape)
+    def __getitem__(self, item: t.Any) -> "te.Self":
+        return self.__class__(self.obj[item], self.escape)
 
     def __str__(self) -> str:
         return str(self.escape(self.obj))
 
     def __repr__(self) -> str:
         return str(self.escape(repr(self.obj)))
```

### Comparing `MarkupSafe-2.1.2/src/markupsafe/_native.py` & `MarkupSafe-2.1.3/src/markupsafe/_native.py`

 * *Files identical despite different names*

### Comparing `MarkupSafe-2.1.2/src/markupsafe/_speedups.c` & `MarkupSafe-2.1.3/src/markupsafe/_speedups.c`

 * *Files identical despite different names*

### Comparing `MarkupSafe-2.1.2/tests/conftest.py` & `MarkupSafe-2.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `MarkupSafe-2.1.2/tests/test_escape.py` & `MarkupSafe-2.1.3/tests/test_escape.py`

 * *Files identical despite different names*

### Comparing `MarkupSafe-2.1.2/tests/test_leak.py` & `MarkupSafe-2.1.3/tests/test_leak.py`

 * *Files identical despite different names*

### Comparing `MarkupSafe-2.1.2/tests/test_markupsafe.py` & `MarkupSafe-2.1.3/tests/test_markupsafe.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,19 @@
     result = Markup("{0[1][bar]}").format([0, {"bar": "<bar/>"}])
     assert result == "&lt;bar/&gt;"
 
     result = Markup("{0[1][bar]}").format([0, {"bar": Markup("<bar/>")}])
     assert result == "<bar/>"
 
 
+def test_format_map():
+    result = Markup("<em>{value}</em>").format_map({"value": "<value>"})
+    assert result == "<em>&lt;value&gt;</em>"
+
+
 def test_formatting_empty():
     formatted = Markup("{}").format(0)
     assert formatted == Markup("0")
 
 
 def test_custom_formatting():
     class HasHTMLOnly:
```

### Comparing `MarkupSafe-2.1.2/tox.ini` & `MarkupSafe-2.1.3/tox.ini`

 * *Files identical despite different names*

