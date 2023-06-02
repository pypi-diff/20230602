# Comparing `tmp/plone.app.transmogrifier-3.0.0.tar.gz` & `tmp/plone.app.transmogrifier-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.transmogrifier-3.0.0.tar", last modified: Thu Jun 30 01:27:46 2022, max compression
+gzip compressed data, was "plone.app.transmogrifier-3.0.1.tar", last modified: Fri Jun  2 17:48:42 2023, max compression
```

## Comparing `plone.app.transmogrifier-3.0.0.tar` & `plone.app.transmogrifier-3.0.1.tar`

### file list

```diff
@@ -1,67 +1,66 @@
-drwxrwxr-x   0 ericof    (1000) ericof    (1000)        0 2022-06-30 01:27:46.972913 plone.app.transmogrifier-3.0.0/
--rw-rw-r--   0 ericof    (1000) ericof    (1000)      963 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/.editorconfig
--rw-rw-r--   0 ericof    (1000) ericof    (1000)       23 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/.gitattributes
--rw-rw-r--   0 ericof    (1000) ericof    (1000)      405 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/.gitignore
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     3404 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/CHANGES.rst
--rw-rw-r--   0 ericof    (1000) ericof    (1000)      120 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/CONTRIBUTORS.rst
--rw-rw-r--   0 ericof    (1000) ericof    (1000)      362 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/DEVELOP.rst
--rw-rw-r--   0 ericof    (1000) ericof    (1000)       81 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/MANIFEST.in
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     3533 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/Makefile
--rw-rw-r--   0 ericof    (1000) ericof    (1000)    43334 2022-06-30 01:27:46.972913 plone.app.transmogrifier-3.0.0/PKG-INFO
--rw-rw-r--   0 ericof    (1000) ericof    (1000)      694 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/README.rst
--rw-rw-r--   0 ericof    (1000) ericof    (1000)      678 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/TODO.rst
--rw-rw-r--   0 ericof    (1000) ericof    (1000)    41948 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/compiled-doc.rst
-drwxrwxr-x   0 ericof    (1000) ericof    (1000)        0 2022-06-30 01:27:46.972913 plone.app.transmogrifier-3.0.0/docs/
--rw-rw-r--   0 ericof    (1000) ericof    (1000)      282 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/docs/INSTALL.rst
--rw-rw-r--   0 ericof    (1000) ericof    (1000)    12282 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/docs/LICENSE.GPL
--rw-rw-r--   0 ericof    (1000) ericof    (1000)      722 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/docs/LICENSE.rst
--rw-rw-r--   0 ericof    (1000) ericof    (1000)      604 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/pyproject.toml
--rw-rw-r--   0 ericof    (1000) ericof    (1000)      117 2022-06-30 01:27:46.972913 plone.app.transmogrifier-3.0.0/setup.cfg
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     3456 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/setup.py
-drwxrwxr-x   0 ericof    (1000) ericof    (1000)        0 2022-06-30 01:27:46.972913 plone.app.transmogrifier-3.0.0/src/
-drwxrwxr-x   0 ericof    (1000) ericof    (1000)        0 2022-06-30 01:27:46.972913 plone.app.transmogrifier-3.0.0/src/plone/
--rw-rw-r--   0 ericof    (1000) ericof    (1000)      245 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/src/plone/__init__.py
-drwxrwxr-x   0 ericof    (1000) ericof    (1000)        0 2022-06-30 01:27:46.972913 plone.app.transmogrifier-3.0.0/src/plone/app/
--rw-rw-r--   0 ericof    (1000) ericof    (1000)      245 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/src/plone/app/__init__.py
-drwxrwxr-x   0 ericof    (1000) ericof    (1000)        0 2022-06-30 01:27:46.972913 plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/
--rw-rw-r--   0 ericof    (1000) ericof    (1000)        0 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/.htpasswd-users
--rw-rw-r--   0 ericof    (1000) ericof    (1000)        0 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/__init__.py
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     1855 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/browserdefault.py
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     3949 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/browserdefault.rst
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     2170 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/configure.zcml
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     2927 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/datesupdater.py
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     3373 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/datesupdater.rst
--rw-rw-r--   0 ericof    (1000) ericof    (1000)       72 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/default-content.csv
-drwxrwxr-x   0 ericof    (1000) ericof    (1000)        0 2022-06-30 01:27:46.972913 plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/empty-site/
--rw-rw-r--   0 ericof    (1000) ericof    (1000)       51 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/empty-site/.gitignore
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     1715 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/mimeencapsulator.py
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     3541 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/mimeencapsulator.rst
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     2336 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/pathfixer.py
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     1723 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/pathfixer.rst
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     1531 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/portaltransforms.py
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     3449 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/portaltransforms.rst
--rw-rw-r--   0 ericof    (1000) ericof    (1000)      302 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/redirector.csv
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     6693 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/redirector.py
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     3510 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/redirector.rst
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     2016 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/reindexobject.py
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     4654 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/reindexobject.rst
--rw-rw-r--   0 ericof    (1000) ericof    (1000)    19706 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/tests.py
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     1880 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/uidupdater.py
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     3141 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/uidupdater.rst
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     1451 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/urlnormalizer.py
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     5947 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/urlnormalizer.rst
--rw-rw-r--   0 ericof    (1000) ericof    (1000)      428 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/utils.py
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     2126 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/versioning.py
--rw-rw-r--   0 ericof    (1000) ericof    (1000)      641 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/versioning.rst
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     2789 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/workflowupdater.py
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     3851 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/workflowupdater.rst
--rw-rw-r--   0 ericof    (1000) ericof    (1000)    32210 2022-06-30 01:27:45.000000 plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/xmlwalker.cfg
-drwxrwxr-x   0 ericof    (1000) ericof    (1000)        0 2022-06-30 01:27:46.972913 plone.app.transmogrifier-3.0.0/src/plone.app.transmogrifier.egg-info/
--rw-rw-r--   0 ericof    (1000) ericof    (1000)    43334 2022-06-30 01:27:46.000000 plone.app.transmogrifier-3.0.0/src/plone.app.transmogrifier.egg-info/PKG-INFO
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     2103 2022-06-30 01:27:46.000000 plone.app.transmogrifier-3.0.0/src/plone.app.transmogrifier.egg-info/SOURCES.txt
--rw-rw-r--   0 ericof    (1000) ericof    (1000)        1 2022-06-30 01:27:46.000000 plone.app.transmogrifier-3.0.0/src/plone.app.transmogrifier.egg-info/dependency_links.txt
--rw-rw-r--   0 ericof    (1000) ericof    (1000)       40 2022-06-30 01:27:46.000000 plone.app.transmogrifier-3.0.0/src/plone.app.transmogrifier.egg-info/entry_points.txt
--rw-rw-r--   0 ericof    (1000) ericof    (1000)       16 2022-06-30 01:27:46.000000 plone.app.transmogrifier-3.0.0/src/plone.app.transmogrifier.egg-info/namespace_packages.txt
--rw-rw-r--   0 ericof    (1000) ericof    (1000)        1 2022-06-30 01:27:46.000000 plone.app.transmogrifier-3.0.0/src/plone.app.transmogrifier.egg-info/not-zip-safe
--rw-rw-r--   0 ericof    (1000) ericof    (1000)      127 2022-06-30 01:27:46.000000 plone.app.transmogrifier-3.0.0/src/plone.app.transmogrifier.egg-info/requires.txt
--rw-rw-r--   0 ericof    (1000) ericof    (1000)        6 2022-06-30 01:27:46.000000 plone.app.transmogrifier-3.0.0/src/plone.app.transmogrifier.egg-info/top_level.txt
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-02 17:48:42.501337 plone.app.transmogrifier-3.0.1/
+-rw-r--r--   0 ericof     (501) staff       (20)      963 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/.editorconfig
+-rw-r--r--   0 ericof     (501) staff       (20)       23 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/.gitattributes
+-rw-r--r--   0 ericof     (501) staff       (20)      405 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/.gitignore
+-rw-r--r--   0 ericof     (501) staff       (20)     3790 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/CHANGES.rst
+-rw-r--r--   0 ericof     (501) staff       (20)      120 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/CONTRIBUTORS.rst
+-rw-r--r--   0 ericof     (501) staff       (20)      362 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/DEVELOP.rst
+-rw-r--r--   0 ericof     (501) staff       (20)       81 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/MANIFEST.in
+-rw-r--r--   0 ericof     (501) staff       (20)     3264 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/Makefile
+-rw-r--r--   0 ericof     (501) staff       (20)    43802 2023-06-02 17:48:42.501434 plone.app.transmogrifier-3.0.1/PKG-INFO
+-rw-r--r--   0 ericof     (501) staff       (20)      694 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/README.rst
+-rw-r--r--   0 ericof     (501) staff       (20)      678 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/TODO.rst
+-rw-r--r--   0 ericof     (501) staff       (20)    42334 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/compiled-doc.rst
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-02 17:48:42.495833 plone.app.transmogrifier-3.0.1/docs/
+-rw-r--r--   0 ericof     (501) staff       (20)      282 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/docs/INSTALL.rst
+-rw-r--r--   0 ericof     (501) staff       (20)    12282 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/docs/LICENSE.GPL
+-rw-r--r--   0 ericof     (501) staff       (20)      722 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/docs/LICENSE.rst
+-rw-r--r--   0 ericof     (501) staff       (20)      760 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/pyproject.toml
+-rw-r--r--   0 ericof     (501) staff       (20)      117 2023-06-02 17:48:42.501737 plone.app.transmogrifier-3.0.1/setup.cfg
+-rw-r--r--   0 ericof     (501) staff       (20)     3436 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/setup.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-02 17:48:42.493358 plone.app.transmogrifier-3.0.1/src/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-02 17:48:42.495960 plone.app.transmogrifier-3.0.1/src/plone/
+-rw-r--r--   0 ericof     (501) staff       (20)      245 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-02 17:48:42.497180 plone.app.transmogrifier-3.0.1/src/plone/app/
+-rw-r--r--   0 ericof     (501) staff       (20)      245 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone/app/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-02 17:48:42.501052 plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/.htpasswd-users
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1856 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/browserdefault.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3949 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/browserdefault.rst
+-rw-r--r--   0 ericof     (501) staff       (20)     2170 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     2927 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/datesupdater.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3373 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/datesupdater.rst
+-rw-r--r--   0 ericof     (501) staff       (20)       72 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/default-content.csv
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-02 17:48:42.501184 plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/empty-site/
+-rw-r--r--   0 ericof     (501) staff       (20)       51 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/empty-site/.gitignore
+-rw-r--r--   0 ericof     (501) staff       (20)     1715 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/mimeencapsulator.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3541 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/mimeencapsulator.rst
+-rw-r--r--   0 ericof     (501) staff       (20)     2336 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/pathfixer.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1723 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/pathfixer.rst
+-rw-r--r--   0 ericof     (501) staff       (20)     1531 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/portaltransforms.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3449 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/portaltransforms.rst
+-rw-r--r--   0 ericof     (501) staff       (20)      302 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/redirector.csv
+-rw-r--r--   0 ericof     (501) staff       (20)     6693 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/redirector.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3510 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/redirector.rst
+-rw-r--r--   0 ericof     (501) staff       (20)     2016 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/reindexobject.py
+-rw-r--r--   0 ericof     (501) staff       (20)     4654 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/reindexobject.rst
+-rw-r--r--   0 ericof     (501) staff       (20)    19708 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/tests.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1880 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/uidupdater.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3141 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/uidupdater.rst
+-rw-r--r--   0 ericof     (501) staff       (20)     1451 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/urlnormalizer.py
+-rw-r--r--   0 ericof     (501) staff       (20)     5947 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/urlnormalizer.rst
+-rw-r--r--   0 ericof     (501) staff       (20)      428 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/utils.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1644 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/versioning.py
+-rw-r--r--   0 ericof     (501) staff       (20)      641 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/versioning.rst
+-rw-r--r--   0 ericof     (501) staff       (20)     2789 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/workflowupdater.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3851 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/workflowupdater.rst
+-rw-r--r--   0 ericof     (501) staff       (20)    32210 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/xmlwalker.cfg
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-02 17:48:42.497070 plone.app.transmogrifier-3.0.1/src/plone.app.transmogrifier.egg-info/
+-rw-r--r--   0 ericof     (501) staff       (20)    43802 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone.app.transmogrifier.egg-info/PKG-INFO
+-rw-r--r--   0 ericof     (501) staff       (20)     2048 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone.app.transmogrifier.egg-info/SOURCES.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        1 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone.app.transmogrifier.egg-info/dependency_links.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       16 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone.app.transmogrifier.egg-info/namespace_packages.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        1 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone.app.transmogrifier.egg-info/not-zip-safe
+-rw-r--r--   0 ericof     (501) staff       (20)      100 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone.app.transmogrifier.egg-info/requires.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        6 2023-06-02 17:48:42.000000 plone.app.transmogrifier-3.0.1/src/plone.app.transmogrifier.egg-info/top_level.txt
```

### Comparing `plone.app.transmogrifier-3.0.0/.editorconfig` & `plone.app.transmogrifier-3.0.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `plone.app.transmogrifier-3.0.0/CHANGES.rst` & `plone.app.transmogrifier-3.0.1/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,29 @@
 Changelog
 =========
 
+3.0.1 (2023-06-02)
+------------------
+
+- Remove Python 2.4 compatibility code.
+  [wesleybl]
+
+- Add Python 3.10 and 3.11 support.
+  [wesleybl]
+
+- Remove ``z3c.autoinclude`` of entry_points.
+  [wesleybl]
+
+- Remove dependency on ``zest.releaser`` in extra test.
+  [wesleybl]
+
+- Fix ``ModuleNotFoundError: No module named 'Products.CMFDynamicViewFTI.interface'`` in Plone 6.
+  [wesleybl]
+
+
 3.0.0 (2022-06-29)
 ------------------
 
 - Implement plone/code-analysis-action
   [ericof]
 
 - Drop support to Plone versions 4.3, 5.0 and 5.1
```

### Comparing `plone.app.transmogrifier-3.0.0/Makefile` & `plone.app.transmogrifier-3.0.1/Makefile`

 * *Files 23% similar despite different names*

```diff
@@ -14,100 +14,95 @@
 GREEN=`tput setaf 2`
 RESET=`tput sgr0`
 YELLOW=`tput setaf 3`
 
 PLONE5=5.2-latest
 PLONE6=6.0-latest
 
-CODE_QUALITY_VERSION=1.0.1
-LINT=docker run --rm -v "$(PWD)":/github/workspace plone/code-quality:${CODE_QUALITY_VERSION} check
-
-PACKAGE_NAME=plone.app.transmogrifier
-PACKAGE_PATH=src/
-CHECK_PATH=setup.py $(PACKAGE_PATH)
+ifndef LOG_LEVEL
+	LOG_LEVEL=INFO
+endif
+
+CODE_QUALITY_VERSION=2.1.0
+CURRENT_USER=$$(whoami)
+USER_INFO=$$(id -u ${CURRENT_USER}):$$(getent group ${CURRENT_USER}|cut -d: -f3)
+BASE_FOLDER=$(shell dirname $(realpath $(firstword $(MAKEFILE_LIST))))
+LINT=docker run -e LOG_LEVEL="${LOG_LEVEL}" --rm -v "${BASE_FOLDER}":/github/workspace plone/code-quality:${CODE_QUALITY_VERSION} check
+FORMAT=docker run --user="${USER_INFO}" -e LOG_LEVEL="${LOG_LEVEL}" --rm -v "${BASE_FOLDER}":/github/workspace plone/code-quality:${CODE_QUALITY_VERSION} format
 
 all: build
 
 # Add the following 'help' target to your Makefile
 # And add help text after each target name starting with '\#\#'
 .PHONY: help
 help: ## This help message
 	@grep -E '^[a-zA-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'
 
 bin/pip:
 	@echo "$(GREEN)==> Setup Virtual Env$(RESET)"
-	python3 -m venv .
+	python3.11 -m venv .
 	bin/pip install -U pip wheel
 
-bin/black bin/isort bin/pyroma bin/zpretty: bin/pip
-	@echo "$(GREEN)==> Install Code Quality tools$(RESET)"
-	bin/pip install -r https://raw.githubusercontent.com/plone/code-quality/v$(CODE_QUALITY_VERSION)/requirements.txt
-	@echo "$(GREEN)==> Install pre-commit hook$(RESET)"
-	echo -e '#!/usr/bin/env bash\nmake lint' > .git/hooks/pre-commit && chmod ug+x .git/hooks/pre-commit
-
-.PHONY: build-plone-5.2
-build-plone-5.2: bin/pip bin/black ## Build Plone 5.2
-	@echo "$(GREEN)==> Build with Plone 5.2$(RESET)"
-	bin/pip install Plone -c https://dist.plone.org/release/$(PLONE5)/constraints.txt
-	bin/pip install -e ".[test]"
-	bin/mkwsgiinstance -d . -u admin:admin
-
-.PHONY: build-plone-6.0
-build-plone-6.0: bin/pip bin/black ## Build Plone 6.0
+.PHONY: build
+build: bin/pip ## Build Plone 6.0
 	@echo "$(GREEN)==> Build with Plone 6.0$(RESET)"
 	bin/pip install Plone -c https://dist.plone.org/release/$(PLONE6)/constraints.txt
+	bin/pip install "zest.releaser[recommended]"
 	bin/pip install -e ".[test]"
 	bin/mkwsgiinstance -d . -u admin:admin
 
-.PHONY: build
-build: build-plone-6.0 ## Build Plone 6.0
-
 .PHONY: clean
 clean: ## Remove old virtualenv and creates a new one
 	@echo "$(RED)==> Cleaning environment and build$(RESET)"
 	rm -rf bin lib lib64 include share etc var inituser pyvenv.cfg .installed.cfg
 
-.PHONY: black
-black: bin/black ## Format codebase
-	bin/black $(CHECK_PATH)
-
-.PHONY: isort
-isort: bin/isort ## Format imports in the codebase
-	bin/isort $(CHECK_PATH)
-
-zpretty: bin/zpretty ## Format xml and zcml with zpretty
-	find "${PACKAGE_PATH}" -name '*.xml' | xargs bin/zpretty -x -i
-	find "${PACKAGE_PATH}" -name '*.zcml' | xargs bin/zpretty -z -i
-
 .PHONY: format
-format: black isort zpretty ## Format the codebase according to our standards
+format: ## Format the codebase according to our standards
+	@echo "$(GREEN)==> Format codebase$(RESET)"
+	$(FORMAT)
+
+.PHONY: format-black
+format-black:  ## Format the codebase with black
+	@echo "$(GREEN)==> Format codebase with black$(RESET)"
+	$(FORMAT) black ${CODEPATH}
+
+.PHONY: format-isort
+format-isort:  ## Format the codebase with isort
+	@echo "$(GREEN)==> Format codebase with isort$(RESET)"
+	$(FORMAT) isort ${CODEPATH}
+
+.PHONY: format-zpretty
+format-zpretty:  ## Format the codebase with zpretty
+	@echo "$(GREEN)==> Format codebase with zpretty$(RESET)"
+	$(FORMAT) zpretty ${CODEPATH}
 
 .PHONY: lint
-lint: lint-isort lint-black lint-flake8 lint-zpretty ## check code style
+lint: ## check code style
+	$(LINT)
 
 .PHONY: lint-black
 lint-black: ## validate black formating
-	$(LINT) black "$(CHECK_PATH)"
+	$(LINT) black ${CODEPATH}
 
 .PHONY: lint-flake8
 lint-flake8: ## validate black formating
-	$(LINT) flake8 "$(CHECK_PATH)"
+	$(LINT) flake8 ${CODEPATH}
 
 .PHONY: lint-isort
 lint-isort: ## validate using isort
-	$(LINT) isort "$(CHECK_PATH)"
+	$(LINT) isort ${CODEPATH}
 
 .PHONY: lint-pyroma
 lint-pyroma: ## validate using pyroma
-	$(LINT) .
+	$(LINT) pyroma ${CODEPATH}
 
 .PHONY: lint-zpretty
 lint-zpretty: ## validate ZCML/XML using zpretty
-	$(LINT) zpretty "$(PACKAGE_PATH)"
+	$(LINT) zpretty ${CODEPATH}
 
 .PHONY: test
 test: ## run tests
-	PYTHONWARNINGS=ignore ./bin/zope-testrunner --auto-color --auto-progress --test-path $(PACKAGE_PATH)
+	PYTHONWARNINGS=ignore ./bin/zope-testrunner --auto-color --auto-progress --test-path src/
 
 .PHONY: start
 start: ## Start a Plone instance on localhost:8080
 	PYTHONWARNINGS=ignore ./bin/runwsgi etc/zope.ini
```

### Comparing `plone.app.transmogrifier-3.0.0/PKG-INFO` & `plone.app.transmogrifier-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: plone.app.transmogrifier
-Version: 3.0.0
+Version: 3.0.1
 Summary: Plone blueprints for collective.transmogrifier pipelines
 Home-page: https://github.com/collective/plone.app.transmogrifier
 Author: Jarn
 Author-email: info@jarn.com
 License: GPL
 Project-URL: PyPI, https://pypi.python.org/pypi/plone.app.transmogrifier
 Project-URL: Source, https://github.com/collective/plone.app.transmogrifier
 Project-URL: Tracker, https://github.com/collective/plone.app.transmogrifier/issues
 Keywords: content import filtering plone
-Platform: UNKNOWN
 Classifier: Development Status :: 6 - Mature
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone :: 5.2
 Classifier: Framework :: Plone :: 6.0
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone
 Classifier: Framework :: Zope2
 Classifier: Framework :: Zope3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Provides-Extra: test
 
 ===============================
@@ -1152,14 +1153,33 @@
      ('spam/eggs/baz', 'eggs'),
      ('spam/eggs/bla', 'spam')]
 
 
 Changelog
 =========
 
+3.0.1 (2023-06-02)
+------------------
+
+- Remove Python 2.4 compatibility code.
+  [wesleybl]
+
+- Add Python 3.10 and 3.11 support.
+  [wesleybl]
+
+- Remove ``z3c.autoinclude`` of entry_points.
+  [wesleybl]
+
+- Remove dependency on ``zest.releaser`` in extra test.
+  [wesleybl]
+
+- Fix ``ModuleNotFoundError: No module named 'Products.CMFDynamicViewFTI.interface'`` in Plone 6.
+  [wesleybl]
+
+
 3.0.0 (2022-06-29)
 ------------------
 
 - Implement plone/code-analysis-action
   [ericof]
 
 - Drop support to Plone versions 4.3, 5.0 and 5.1
@@ -1299,9 +1319,7 @@
 
 1.0 (2009-08-09)
 ----------------
 
 - Initial package.
   [mj]
 
-
-
```

### Comparing `plone.app.transmogrifier-3.0.0/README.rst` & `plone.app.transmogrifier-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.transmogrifier-3.0.0/TODO.rst` & `plone.app.transmogrifier-3.0.1/TODO.rst`

 * *Files identical despite different names*

### Comparing `plone.app.transmogrifier-3.0.0/compiled-doc.rst` & `plone.app.transmogrifier-3.0.1/src/plone.app.transmogrifier.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,40 @@
+Metadata-Version: 2.1
+Name: plone.app.transmogrifier
+Version: 3.0.1
+Summary: Plone blueprints for collective.transmogrifier pipelines
+Home-page: https://github.com/collective/plone.app.transmogrifier
+Author: Jarn
+Author-email: info@jarn.com
+License: GPL
+Project-URL: PyPI, https://pypi.python.org/pypi/plone.app.transmogrifier
+Project-URL: Source, https://github.com/collective/plone.app.transmogrifier
+Project-URL: Tracker, https://github.com/collective/plone.app.transmogrifier/issues
+Keywords: content import filtering plone
+Classifier: Development Status :: 6 - Mature
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Plone :: 5.2
+Classifier: Framework :: Plone :: 6.0
+Classifier: Framework :: Plone :: Addon
+Classifier: Framework :: Plone
+Classifier: Framework :: Zope2
+Classifier: Framework :: Zope3
+Classifier: License :: OSI Approved :: GNU General Public License (GPL)
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.7
+Provides-Extra: test
+
 ===============================
 Plone transmogrifier blueprints
 ===============================
 
 .. contents::
 
 This package contains several blueprints for `collective.transmogrifier`_
@@ -1120,14 +1153,33 @@
      ('spam/eggs/baz', 'eggs'),
      ('spam/eggs/bla', 'spam')]
 
 
 Changelog
 =========
 
+3.0.1 (2023-06-02)
+------------------
+
+- Remove Python 2.4 compatibility code.
+  [wesleybl]
+
+- Add Python 3.10 and 3.11 support.
+  [wesleybl]
+
+- Remove ``z3c.autoinclude`` of entry_points.
+  [wesleybl]
+
+- Remove dependency on ``zest.releaser`` in extra test.
+  [wesleybl]
+
+- Fix ``ModuleNotFoundError: No module named 'Products.CMFDynamicViewFTI.interface'`` in Plone 6.
+  [wesleybl]
+
+
 3.0.0 (2022-06-29)
 ------------------
 
 - Implement plone/code-analysis-action
   [ericof]
 
 - Drop support to Plone versions 4.3, 5.0 and 5.1
```

### Comparing `plone.app.transmogrifier-3.0.0/docs/LICENSE.GPL` & `plone.app.transmogrifier-3.0.1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.transmogrifier-3.0.0/docs/LICENSE.rst` & `plone.app.transmogrifier-3.0.1/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `plone.app.transmogrifier-3.0.0/setup.py` & `plone.app.transmogrifier-3.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     )
 )
 open("compiled-doc.rst", "w").write(long_description)
 
 
 setup(
     name="plone.app.transmogrifier",
-    version="3.0.0",
+    version="3.0.1",
     description="Plone blueprints for collective.transmogrifier pipelines",
     long_description=long_description,
     classifiers=[
         "Development Status :: 6 - Mature",
         "Environment :: Web Environment",
         "Framework :: Plone :: 5.2",
         "Framework :: Plone :: 6.0",
@@ -60,14 +60,16 @@
         "Framework :: Zope2",
         "Framework :: Zope3",
         "License :: OSI Approved :: GNU General Public License (GPL)",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python",
         "Topic :: Software Development :: Libraries :: Application Frameworks",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     keywords="content import filtering plone",
     author="Jarn",
     author_email="info@jarn.com",
@@ -90,15 +92,10 @@
         "plone.uuid",
         "setuptools",
         "zope.component",
     ],
     extras_require={
         "test": [
             "zope.testrunner",
-            "zest.releaser[recommended]",
         ]
     },
-    entry_points="""
-    [z3c.autoinclude.plugin]
-    target = plone
-    """,
 )
```

### Comparing `plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/browserdefault.py` & `plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/browserdefault.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from collective.transmogrifier.interfaces import ISection
 from collective.transmogrifier.interfaces import ISectionBlueprint
 from collective.transmogrifier.utils import defaultMatcher
 from collective.transmogrifier.utils import traverse
-from Products.CMFDynamicViewFTI.interface import ISelectableBrowserDefault
+from Products.CMFDynamicViewFTI.interfaces import ISelectableBrowserDefault
 from zope.interface import implementer
 from zope.interface import provider
 
 
 @provider(ISectionBlueprint)
 @implementer(ISection)
 class BrowserDefaultSection:
```

### Comparing `plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/browserdefault.rst` & `plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/browserdefault.rst`

 * *Files identical despite different names*

### Comparing `plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/configure.zcml` & `plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/datesupdater.py` & `plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/datesupdater.py`

 * *Files identical despite different names*

### Comparing `plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/datesupdater.rst` & `plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/datesupdater.rst`

 * *Files identical despite different names*

### Comparing `plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/mimeencapsulator.py` & `plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/mimeencapsulator.py`

 * *Files identical despite different names*

### Comparing `plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/mimeencapsulator.rst` & `plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/mimeencapsulator.rst`

 * *Files identical despite different names*

### Comparing `plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/pathfixer.py` & `plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/pathfixer.py`

 * *Files identical despite different names*

### Comparing `plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/pathfixer.rst` & `plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/pathfixer.rst`

 * *Files identical despite different names*

### Comparing `plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/portaltransforms.py` & `plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/portaltransforms.py`

 * *Files identical despite different names*

### Comparing `plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/portaltransforms.rst` & `plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/portaltransforms.rst`

 * *Files identical despite different names*

### Comparing `plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/redirector.py` & `plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/redirector.py`

 * *Files identical despite different names*

### Comparing `plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/redirector.rst` & `plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/redirector.rst`

 * *Files identical despite different names*

### Comparing `plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/reindexobject.py` & `plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/reindexobject.py`

 * *Files identical despite different names*

### Comparing `plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/reindexobject.rst` & `plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/reindexobject.rst`

 * *Files identical despite different names*

### Comparing `plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/tests.py` & `plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 
     provideUtility(WorkflowSource, name="plone.app.transmogrifier.tests.workflowsource")
 
 
 def browserDefaultSetUp(test):
     sectionsSetUp(test)
 
-    from Products.CMFDynamicViewFTI.interface import ISelectableBrowserDefault
+    from Products.CMFDynamicViewFTI.interfaces import ISelectableBrowserDefault
 
     @implementer(ISelectableBrowserDefault)
     class MockPortal(MockObjectManager):
 
         updated = []
 
         def setLayout(self, layout):
@@ -176,15 +176,15 @@
         name="plone.app.transmogrifier.tests.browserdefaultsource",
     )
 
 
 def urlNormalizerSetUp(test):
     sectionsSetUp(test)
 
-    from Products.CMFDynamicViewFTI.interface import ISelectableBrowserDefault
+    from Products.CMFDynamicViewFTI.interfaces import ISelectableBrowserDefault
 
     @implementer(ISelectableBrowserDefault)
     class MockPortal(MockObjectManager):
         pass
 
     test.globs["plone"] = MockPortal()
     test.globs["transmogrifier"].context = test.globs["plone"]
```

### Comparing `plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/uidupdater.py` & `plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/uidupdater.py`

 * *Files identical despite different names*

### Comparing `plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/uidupdater.rst` & `plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/uidupdater.rst`

 * *Files identical despite different names*

### Comparing `plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/urlnormalizer.py` & `plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/urlnormalizer.py`

 * *Files identical despite different names*

### Comparing `plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/urlnormalizer.rst` & `plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/urlnormalizer.rst`

 * *Files identical despite different names*

### Comparing `plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/versioning.py` & `plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/versioning.py`

 * *Files 17% similar despite different names*

```diff
@@ -32,31 +32,20 @@
         versionable[:] = ()
 
 
 @provider(ISectionBlueprint)
 class DisableVersioningSection(BaseVersioningSection):
     def __iter__(self):
         for item in self.previous:
-            # http://stackoverflow.com/questions/2339358/workaround-for-python-2-4s-yield-not-allowed-in-try-block-with-finally-clause
-            # try:
-            #    self.save()
-            #    self.clear()
-            #    yield item
-            # finally:
-            #    self.restore()
-
-            # XXX I'm not entirely sure if the code below does the same thing
-            # as the code above. [aclark]
             try:
                 self.save()
                 self.clear()
                 yield item
-            except (AttributeError, KeyError, ValueError):
+            finally:
                 self.restore()
-            self.restore()
 
 
 @provider(ISectionBlueprint)
 class EnableVersioningSection(BaseVersioningSection):
     def __iter__(self):
         for item in self.previous:
             self.restore()
```

### Comparing `plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/versioning.rst` & `plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/versioning.rst`

 * *Files identical despite different names*

### Comparing `plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/workflowupdater.py` & `plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/workflowupdater.py`

 * *Files identical despite different names*

### Comparing `plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/workflowupdater.rst` & `plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/workflowupdater.rst`

 * *Files identical despite different names*

### Comparing `plone.app.transmogrifier-3.0.0/src/plone/app/transmogrifier/xmlwalker.cfg` & `plone.app.transmogrifier-3.0.1/src/plone/app/transmogrifier/xmlwalker.cfg`

 * *Files identical despite different names*

### Comparing `plone.app.transmogrifier-3.0.0/src/plone.app.transmogrifier.egg-info/PKG-INFO` & `plone.app.transmogrifier-3.0.1/compiled-doc.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: plone.app.transmogrifier
-Version: 3.0.0
-Summary: Plone blueprints for collective.transmogrifier pipelines
-Home-page: https://github.com/collective/plone.app.transmogrifier
-Author: Jarn
-Author-email: info@jarn.com
-License: GPL
-Project-URL: PyPI, https://pypi.python.org/pypi/plone.app.transmogrifier
-Project-URL: Source, https://github.com/collective/plone.app.transmogrifier
-Project-URL: Tracker, https://github.com/collective/plone.app.transmogrifier/issues
-Keywords: content import filtering plone
-Platform: UNKNOWN
-Classifier: Development Status :: 6 - Mature
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Plone :: 5.2
-Classifier: Framework :: Plone :: 6.0
-Classifier: Framework :: Plone :: Addon
-Classifier: Framework :: Plone
-Classifier: Framework :: Zope2
-Classifier: Framework :: Zope3
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
-Provides-Extra: test
-
 ===============================
 Plone transmogrifier blueprints
 ===============================
 
 .. contents::
 
 This package contains several blueprints for `collective.transmogrifier`_
@@ -1152,14 +1120,33 @@
      ('spam/eggs/baz', 'eggs'),
      ('spam/eggs/bla', 'spam')]
 
 
 Changelog
 =========
 
+3.0.1 (2023-06-02)
+------------------
+
+- Remove Python 2.4 compatibility code.
+  [wesleybl]
+
+- Add Python 3.10 and 3.11 support.
+  [wesleybl]
+
+- Remove ``z3c.autoinclude`` of entry_points.
+  [wesleybl]
+
+- Remove dependency on ``zest.releaser`` in extra test.
+  [wesleybl]
+
+- Fix ``ModuleNotFoundError: No module named 'Products.CMFDynamicViewFTI.interface'`` in Plone 6.
+  [wesleybl]
+
+
 3.0.0 (2022-06-29)
 ------------------
 
 - Implement plone/code-analysis-action
   [ericof]
 
 - Drop support to Plone versions 4.3, 5.0 and 5.1
@@ -1299,9 +1286,7 @@
 
 1.0 (2009-08-09)
 ----------------
 
 - Initial package.
   [mj]
 
-
-
```

### Comparing `plone.app.transmogrifier-3.0.0/src/plone.app.transmogrifier.egg-info/SOURCES.txt` & `plone.app.transmogrifier-3.0.1/src/plone.app.transmogrifier.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 docs/INSTALL.rst
 docs/LICENSE.GPL
 docs/LICENSE.rst
 src/plone/__init__.py
 src/plone.app.transmogrifier.egg-info/PKG-INFO
 src/plone.app.transmogrifier.egg-info/SOURCES.txt
 src/plone.app.transmogrifier.egg-info/dependency_links.txt
-src/plone.app.transmogrifier.egg-info/entry_points.txt
 src/plone.app.transmogrifier.egg-info/namespace_packages.txt
 src/plone.app.transmogrifier.egg-info/not-zip-safe
 src/plone.app.transmogrifier.egg-info/requires.txt
 src/plone.app.transmogrifier.egg-info/top_level.txt
 src/plone/app/__init__.py
 src/plone/app/transmogrifier/.htpasswd-users
 src/plone/app/transmogrifier/__init__.py
```

