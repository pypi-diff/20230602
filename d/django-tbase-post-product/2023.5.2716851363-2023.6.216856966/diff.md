# Comparing `tmp/django_tbase_post_product-2023.5.2716851363.tar.gz` & `tmp/django_tbase_post_product-2023.6.216856966.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tbase_post_product-2023.5.2716851363.tar", last modified: Fri May 26 21:25:59 2023, max compression
+gzip compressed data, was "django_tbase_post_product-2023.6.216856966.tar", last modified: Fri Jun  2 09:04:18 2023, max compression
```

## Comparing `django_tbase_post_product-2023.5.2716851363.tar` & `django_tbase_post_product-2023.6.216856966.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-26 21:25:59.906149 django_tbase_post_product-2023.5.2716851363/
--rw-r--r--   0 terry     (1000) terry     (1000)      143 2023-05-20 17:05:28.000000 django_tbase_post_product-2023.5.2716851363/MANIFEST.in
--rw-r--r--   0 terry     (1000) terry     (1000)     1370 2023-05-26 21:25:59.906149 django_tbase_post_product-2023.5.2716851363/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)     1010 2023-05-20 15:52:49.000000 django_tbase_post_product-2023.5.2716851363/README.md
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-26 21:25:59.896149 django_tbase_post_product-2023.5.2716851363/django_tbase_post_product.egg-info/
--rw-r--r--   0 terry     (1000) terry     (1000)     1370 2023-05-26 21:25:59.000000 django_tbase_post_product-2023.5.2716851363/django_tbase_post_product.egg-info/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)     2109 2023-05-26 21:25:59.000000 django_tbase_post_product-2023.5.2716851363/django_tbase_post_product.egg-info/SOURCES.txt
--rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-05-26 21:25:59.000000 django_tbase_post_product-2023.5.2716851363/django_tbase_post_product.egg-info/dependency_links.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       83 2023-05-26 21:25:59.000000 django_tbase_post_product-2023.5.2716851363/django_tbase_post_product.egg-info/requires.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       11 2023-05-26 21:25:59.000000 django_tbase_post_product-2023.5.2716851363/django_tbase_post_product.egg-info/top_level.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-05-26 21:25:59.906149 django_tbase_post_product-2023.5.2716851363/setup.cfg
--rw-r--r--   0 terry     (1000) terry     (1000)     2305 2023-05-26 20:53:14.000000 django_tbase_post_product-2023.5.2716851363/setup.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-26 21:25:59.896149 django_tbase_post_product-2023.5.2716851363/tbase_post/
--rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/__init__.py
--rw-r--r--   0 terry     (1000) terry     (1000)     1727 2023-05-15 18:15:03.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/admin.py
--rw-r--r--   0 terry     (1000) terry     (1000)      146 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/apps.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-26 21:25:59.906149 django_tbase_post_product-2023.5.2716851363/tbase_post/migrations/
--rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/migrations/__init__.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-26 21:25:59.906149 django_tbase_post_product-2023.5.2716851363/tbase_post/migrations/__pycache__/
--rw-r--r--   0 terry     (1000) terry     (1000)     1062 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     1092 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/migrations/__pycache__/0002_auto_20230421_1307.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     1081 2023-05-05 14:25:13.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/migrations/__pycache__/0003_auto_20230505_1424.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     1498 2023-05-05 15:03:52.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/migrations/__pycache__/0004_auto_20230505_1503.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)      591 2023-05-05 15:05:58.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/migrations/__pycache__/0005_rename_banner_img_post_article_img.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     1059 2023-05-05 15:46:35.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/migrations/__pycache__/0006_auto_20230505_1546.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)      168 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/migrations/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     3388 2023-05-05 15:46:17.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/models.py
--rw-r--r--   0 terry     (1000) terry     (1000)      479 2023-05-12 18:21:31.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/sitemaps.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-26 21:25:59.896149 django_tbase_post_product-2023.5.2716851363/tbase_post/static/
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-26 21:25:59.906149 django_tbase_post_product-2023.5.2716851363/tbase_post/static/images/
--rw-r--r--   0 terry     (1000) terry     (1000)    59619 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg
--rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg:Zone.Identifier
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-26 21:25:59.906149 django_tbase_post_product-2023.5.2716851363/tbase_post/templates/
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-26 21:25:59.906149 django_tbase_post_product-2023.5.2716851363/tbase_post/templates/post/
--rw-r--r--   0 terry     (1000) terry     (1000)     2723 2023-05-09 11:19:05.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/templates/post/article_list_by_tag.html
--rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/templates/post/article_list_by_tag.html:Zone.Identifier
--rw-r--r--   0 terry     (1000) terry     (1000)     2120 2023-05-09 11:29:39.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/templates/post/blog_index.html
--rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/templates/post/blog_index.html:Zone.Identifier
--rw-r--r--   0 terry     (1000) terry     (1000)     4026 2023-05-26 21:25:28.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/templates/post/detail.html
--rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/templates/post/detail.html:Zone.Identifier
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-26 21:25:59.906149 django_tbase_post_product-2023.5.2716851363/tbase_post/templates/post/extras/
--rw-r--r--   0 terry     (1000) terry     (1000)      443 2023-05-09 11:22:22.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/templates/post/extras/amazon_link.html
--rw-r--r--   0 terry     (1000) terry     (1000)      376 2023-05-08 23:37:48.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/templates/post/extras/last_update.html
--rw-r--r--   0 terry     (1000) terry     (1000)      294 2023-05-08 23:37:59.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/templates/post/extras/related_post_by_tags.html
--rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/templates/post/extras/related_post_by_tags.html:Zone.Identifier
--rw-r--r--   0 terry     (1000) terry     (1000)      415 2023-05-01 19:23:09.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/templates/post/extras/tags.html
--rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/templates/post/extras/tags.html:Zone.Identifier
--rw-r--r--   0 terry     (1000) terry     (1000)      391 2023-05-05 16:55:19.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/templates/sitemap.xml
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-26 21:25:59.906149 django_tbase_post_product-2023.5.2716851363/tbase_post/templatetags/
--rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/templatetags/__init__.py
--rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/templatetags/__init__.py:Zone.Identifier
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-26 21:25:59.906149 django_tbase_post_product-2023.5.2716851363/tbase_post/templatetags/__pycache__/
--rw-r--r--   0 terry     (1000) terry     (1000)      170 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/templatetags/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     3002 2023-05-11 17:20:31.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     5044 2023-05-09 11:42:47.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/templatetags/post_extras.py
--rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/templatetags/post_extras.py:Zone.Identifier
--rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/tests.py
--rw-r--r--   0 terry     (1000) terry     (1000)      725 2023-05-05 16:36:02.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/urls.py
--rw-r--r--   0 terry     (1000) terry     (1000)     3256 2023-05-05 16:15:07.000000 django_tbase_post_product-2023.5.2716851363/tbase_post/views.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-02 09:04:18.855703 django_tbase_post_product-2023.6.216856966/
+-rw-r--r--   0 terry     (1000) terry     (1000)      143 2023-05-20 17:05:28.000000 django_tbase_post_product-2023.6.216856966/MANIFEST.in
+-rw-r--r--   0 terry     (1000) terry     (1000)     1423 2023-06-02 09:04:18.855703 django_tbase_post_product-2023.6.216856966/PKG-INFO
+-rw-r--r--   0 terry     (1000) terry     (1000)     1101 2023-06-02 09:03:18.000000 django_tbase_post_product-2023.6.216856966/README.md
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-02 09:04:18.795704 django_tbase_post_product-2023.6.216856966/django_tbase_post_product.egg-info/
+-rw-r--r--   0 terry     (1000) terry     (1000)     1423 2023-06-02 09:04:18.000000 django_tbase_post_product-2023.6.216856966/django_tbase_post_product.egg-info/PKG-INFO
+-rw-r--r--   0 terry     (1000) terry     (1000)     2109 2023-06-02 09:04:18.000000 django_tbase_post_product-2023.6.216856966/django_tbase_post_product.egg-info/SOURCES.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-06-02 09:04:18.000000 django_tbase_post_product-2023.6.216856966/django_tbase_post_product.egg-info/dependency_links.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       83 2023-06-02 09:04:18.000000 django_tbase_post_product-2023.6.216856966/django_tbase_post_product.egg-info/requires.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       11 2023-06-02 09:04:18.000000 django_tbase_post_product-2023.6.216856966/django_tbase_post_product.egg-info/top_level.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-06-02 09:04:18.855703 django_tbase_post_product-2023.6.216856966/setup.cfg
+-rw-r--r--   0 terry     (1000) terry     (1000)     2305 2023-05-26 20:53:14.000000 django_tbase_post_product-2023.6.216856966/setup.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-02 09:04:18.835703 django_tbase_post_product-2023.6.216856966/tbase_post/
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.6.216856966/tbase_post/__init__.py
+-rw-r--r--   0 terry     (1000) terry     (1000)     1727 2023-05-15 18:15:03.000000 django_tbase_post_product-2023.6.216856966/tbase_post/admin.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      146 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.6.216856966/tbase_post/apps.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-02 09:04:18.835703 django_tbase_post_product-2023.6.216856966/tbase_post/migrations/
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.216856966/tbase_post/migrations/__init__.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-02 09:04:18.835703 django_tbase_post_product-2023.6.216856966/tbase_post/migrations/__pycache__/
+-rw-r--r--   0 terry     (1000) terry     (1000)     1062 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.6.216856966/tbase_post/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     1092 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.6.216856966/tbase_post/migrations/__pycache__/0002_auto_20230421_1307.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     1081 2023-05-05 14:25:13.000000 django_tbase_post_product-2023.6.216856966/tbase_post/migrations/__pycache__/0003_auto_20230505_1424.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     1498 2023-05-05 15:03:52.000000 django_tbase_post_product-2023.6.216856966/tbase_post/migrations/__pycache__/0004_auto_20230505_1503.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)      591 2023-05-05 15:05:58.000000 django_tbase_post_product-2023.6.216856966/tbase_post/migrations/__pycache__/0005_rename_banner_img_post_article_img.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     1059 2023-05-05 15:46:35.000000 django_tbase_post_product-2023.6.216856966/tbase_post/migrations/__pycache__/0006_auto_20230505_1546.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)      168 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.6.216856966/tbase_post/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     3388 2023-05-05 15:46:17.000000 django_tbase_post_product-2023.6.216856966/tbase_post/models.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      479 2023-05-12 18:21:31.000000 django_tbase_post_product-2023.6.216856966/tbase_post/sitemaps.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-02 09:04:18.795704 django_tbase_post_product-2023.6.216856966/tbase_post/static/
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-02 09:04:18.845703 django_tbase_post_product-2023.6.216856966/tbase_post/static/images/
+-rw-r--r--   0 terry     (1000) terry     (1000)    59619 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.216856966/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.216856966/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg:Zone.Identifier
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-02 09:04:18.845703 django_tbase_post_product-2023.6.216856966/tbase_post/templates/
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-02 09:04:18.845703 django_tbase_post_product-2023.6.216856966/tbase_post/templates/post/
+-rw-r--r--   0 terry     (1000) terry     (1000)     2799 2023-06-02 09:00:28.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templates/post/article_list_by_tag.html
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templates/post/article_list_by_tag.html:Zone.Identifier
+-rw-r--r--   0 terry     (1000) terry     (1000)     2120 2023-05-09 11:29:39.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templates/post/blog_index.html
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templates/post/blog_index.html:Zone.Identifier
+-rw-r--r--   0 terry     (1000) terry     (1000)     4173 2023-06-02 08:58:32.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templates/post/detail.html
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templates/post/detail.html:Zone.Identifier
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-02 09:04:18.855703 django_tbase_post_product-2023.6.216856966/tbase_post/templates/post/extras/
+-rw-r--r--   0 terry     (1000) terry     (1000)      443 2023-05-09 11:22:22.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templates/post/extras/amazon_link.html
+-rw-r--r--   0 terry     (1000) terry     (1000)      376 2023-05-08 23:37:48.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templates/post/extras/last_update.html
+-rw-r--r--   0 terry     (1000) terry     (1000)      294 2023-05-08 23:37:59.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templates/post/extras/related_post_by_tags.html
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templates/post/extras/related_post_by_tags.html:Zone.Identifier
+-rw-r--r--   0 terry     (1000) terry     (1000)      415 2023-05-01 19:23:09.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templates/post/extras/tags.html
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templates/post/extras/tags.html:Zone.Identifier
+-rw-r--r--   0 terry     (1000) terry     (1000)      391 2023-05-05 16:55:19.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templates/sitemap.xml
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-02 09:04:18.855703 django_tbase_post_product-2023.6.216856966/tbase_post/templatetags/
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templatetags/__init__.py
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templatetags/__init__.py:Zone.Identifier
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-06-02 09:04:18.855703 django_tbase_post_product-2023.6.216856966/tbase_post/templatetags/__pycache__/
+-rw-r--r--   0 terry     (1000) terry     (1000)      170 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templatetags/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     3002 2023-05-11 17:20:31.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     5044 2023-05-09 11:42:47.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templatetags/post_extras.py
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.6.216856966/tbase_post/templatetags/post_extras.py:Zone.Identifier
+-rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.6.216856966/tbase_post/tests.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      725 2023-05-05 16:36:02.000000 django_tbase_post_product-2023.6.216856966/tbase_post/urls.py
+-rw-r--r--   0 terry     (1000) terry     (1000)     3823 2023-06-02 08:57:44.000000 django_tbase_post_product-2023.6.216856966/tbase_post/views.py
```

### Comparing `django_tbase_post_product-2023.5.2716851363/PKG-INFO` & `django_tbase_post_product-2023.6.216856966/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: django_tbase_post_product
-Version: 2023.5.2716851363
+Version: 2023.6.216856966
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post_product/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post_product
 
 用于产品的文章模块
 
 
@@ -35,14 +33,20 @@
 
  ]
 ```
 
 
 
 
+# 2023/06/02
+加入seo优化，对tags内容过少（小于10）的页面添加noindex
+
+
+
+
 ## Getting Started
 
 Download links:
 
 SSH clone URL: ssh://git@git.jetbrains.space/terrychanorg/django-expand/tbase_post_product.git
 
 HTTPS clone URL: https://git.jetbrains.space/terrychanorg/django-expand/tbase_post_product.git
@@ -62,9 +66,7 @@
 ## Deployment
 
 Add additional notes about how to deploy this on a production system.
 
 ## Resources
 
 Add links to external resources for this project, such as CI server, bug tracker, etc.
-
-
```

### Comparing `django_tbase_post_product-2023.5.2716851363/README.md` & `django_tbase_post_product-2023.6.216856966/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,20 @@
 
  ]
 ```
 
 
 
 
+# 2023/06/02
+加入seo优化，对tags内容过少（小于10）的页面添加noindex
+
+
+
+
 ## Getting Started
 
 Download links:
 
 SSH clone URL: ssh://git@git.jetbrains.space/terrychanorg/django-expand/tbase_post_product.git
 
 HTTPS clone URL: https://git.jetbrains.space/terrychanorg/django-expand/tbase_post_product.git
```

### Comparing `django_tbase_post_product-2023.5.2716851363/django_tbase_post_product.egg-info/PKG-INFO` & `django_tbase_post_product-2023.6.216856966/django_tbase_post_product.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: django-tbase-post-product
-Version: 2023.5.2716851363
+Version: 2023.6.216856966
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post_product/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post_product
 
 用于产品的文章模块
 
 
@@ -35,14 +33,20 @@
 
  ]
 ```
 
 
 
 
+# 2023/06/02
+加入seo优化，对tags内容过少（小于10）的页面添加noindex
+
+
+
+
 ## Getting Started
 
 Download links:
 
 SSH clone URL: ssh://git@git.jetbrains.space/terrychanorg/django-expand/tbase_post_product.git
 
 HTTPS clone URL: https://git.jetbrains.space/terrychanorg/django-expand/tbase_post_product.git
@@ -62,9 +66,7 @@
 ## Deployment
 
 Add additional notes about how to deploy this on a production system.
 
 ## Resources
 
 Add links to external resources for this project, such as CI server, bug tracker, etc.
-
-
```

### Comparing `django_tbase_post_product-2023.5.2716851363/django_tbase_post_product.egg-info/SOURCES.txt` & `django_tbase_post_product-2023.6.216856966/django_tbase_post_product.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.5.2716851363/setup.py` & `django_tbase_post_product-2023.6.216856966/setup.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.5.2716851363/tbase_post/admin.py` & `django_tbase_post_product-2023.6.216856966/tbase_post/admin.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.5.2716851363/tbase_post/migrations/__pycache__/0001_initial.cpython-310.pyc` & `django_tbase_post_product-2023.6.216856966/tbase_post/migrations/__pycache__/0001_initial.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.5.2716851363/tbase_post/migrations/__pycache__/0002_auto_20230421_1307.cpython-310.pyc` & `django_tbase_post_product-2023.6.216856966/tbase_post/migrations/__pycache__/0002_auto_20230421_1307.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.5.2716851363/tbase_post/migrations/__pycache__/0003_auto_20230505_1424.cpython-310.pyc` & `django_tbase_post_product-2023.6.216856966/tbase_post/migrations/__pycache__/0003_auto_20230505_1424.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.5.2716851363/tbase_post/migrations/__pycache__/0004_auto_20230505_1503.cpython-310.pyc` & `django_tbase_post_product-2023.6.216856966/tbase_post/migrations/__pycache__/0004_auto_20230505_1503.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.5.2716851363/tbase_post/migrations/__pycache__/0005_rename_banner_img_post_article_img.cpython-310.pyc` & `django_tbase_post_product-2023.6.216856966/tbase_post/migrations/__pycache__/0005_rename_banner_img_post_article_img.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.5.2716851363/tbase_post/migrations/__pycache__/0006_auto_20230505_1546.cpython-310.pyc` & `django_tbase_post_product-2023.6.216856966/tbase_post/migrations/__pycache__/0006_auto_20230505_1546.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.5.2716851363/tbase_post/models.py` & `django_tbase_post_product-2023.6.216856966/tbase_post/models.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.5.2716851363/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg` & `django_tbase_post_product-2023.6.216856966/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.5.2716851363/tbase_post/templates/post/article_list_by_tag.html` & `django_tbase_post_product-2023.6.216856966/tbase_post/templates/post/article_list_by_tag.html`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 
 {% block top_nav %}
 
 {% endblock %}
 
 
 {% block head %}
+{% if meta.noindex %} 
+<meta name="robots" content="noindex">
+{% endif %} 
+
 {% endblock %}
 
 {% block body_class_expand %}tag{% endblock %}
  {% block article_list %}
 
  {% for detail in object_list %}
```

#### html2text {}

```diff
@@ -1,12 +1,14 @@
 {% extends 'blog/blog.html' %} {% load static %} {% comment %} {% extends
 'base.html' %} {% endcomment %} {% load post_extras %} {% block title %}
-{% endblock %} {% block top_nav %} {% endblock %} {% block head %} {% endblock
-%} {% block body_class_expand %}tag{% endblock %} {% block article_list %} {%
-for detail in object_list %}   {%if detail.article_img%}
+{% endblock %} {% block top_nav %} {% endblock %} {% block head %} {% if
+meta.noindex %}
+ {% endif %} {% endblock %} {% block body_class_expand %}tag{% endblock %} {%
+block article_list %} {% for detail in object_list %}   {%if
+detail.article_img%}
 [{{detail.product_name}}]
 {%endif%}
 {{detail.title}}
 By David_Grzyb, Published on {{detail.created_on}}
 {% comment %} éå¶ææ¬é¿åº¦ {% endcomment %} {
 {detail.content|truncatechars:3}}
 {% tags detail.tags.all%}
```

### Comparing `django_tbase_post_product-2023.5.2716851363/tbase_post/templates/post/blog_index.html` & `django_tbase_post_product-2023.6.216856966/tbase_post/templates/post/blog_index.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.5.2716851363/tbase_post/templates/post/detail.html` & `django_tbase_post_product-2023.6.216856966/tbase_post/templates/post/detail.html`

 * *Files 3% similar despite different names*

```diff
@@ -52,14 +52,17 @@
 {% block title %}<title>{{detail.title}} : {{title}}</title>{% endblock %}
 
 
 {% block head %}
 {% tag_names object.tags.all 4 as tag%}
 <meta name="description" content="{{detail.content|truncatechars:128}}">
 <meta name="keywords" content="{{detail.product_name}},{{ tag.names_text}}">
+{% if meta.noindex %} 
+<meta name="robots" content="noindex">
+{% endif %} 
 <!-- <meta name="author" content="Terry"> -->
 
 {% endblock %}
 
 {% block top_header %} {% endblock %}
 
 {% block top_nav %}
@@ -129,22 +132,22 @@
 <!--上一页下一页链接区域-->
 
 {% block article_previous_next %}
 
                 {% if detail.get_previous_by_created_on  %}
                 <a href="{% url 'detail_view' detail.get_previous_by_created_on.pk %}" class="w-1/2 bg-white shadow hover:shadow-md text-left p-6">
                     <p class="text-lg text-blue-800 font-bold flex items-center"><i class="fas fa-arrow-left pr-1"></i> {{detail.get_previous_by_created_on.title}}</p>
- 
+                    <p class="pt-2"></p>
                 </a>
 
     {%endif%}
                 {% if detail.get_next_by_created_on  %}
                 <a href="{% url 'detail_view' detail.get_next_by_created_on.pk %}" class="w-1/2 bg-white shadow hover:shadow-md text-right p-6">
                     <p class="text-lg text-blue-800 font-bold flex items-center justify-end">{{detail.get_next_by_created_on.title}} <i class="fas fa-arrow-right pl-1"></i></p>
-       
+                    <p class="pt-2"></p>
                 </a>
 
             {%endif%}
 {% endblock %}
 <!--上一页下一页链接区域 结束-->
```

#### html2text {}

```diff
@@ -1,17 +1,19 @@
 {% extends 'blog/post.html' %} {% comment %} å è½½åº {% endcomment %} {% load
 static %} {% comment %} {% extends 'base.html' %} {% endcomment %} {% load
 martortags %} {% load post_extras %} {% load solo_tags %} {% comment %}
 å è½½åº ç»æ {% endcomment %} {% block tailwind_css %}
  {% endblock %} {% block title %}
 {% endblock %} {% block head %} {% tag_names object.tags.all 4 as tag%}
 
-  {% endblock %} {% block top_header %} {% endblock %} {% block top_nav %} {%
-endblock %} {% block body_class_expand %}detail{% endblock %} {% block
-text_header %} {% endblock %} {% block article_img %} {%if detail.article_img%}
+ {% if meta.noindex %}
+ {% endif %}  {% endblock %} {% block top_header %} {% endblock %} {% block
+top_nav %} {% endblock %} {% block body_class_expand %}detail{% endblock %} {%
+block text_header %} {% endblock %} {% block article_img %} {%if
+detail.article_img%}
 [{{detail.product_name}}]
 {%endif%} {% endblock %} {% block article %}
 {{detail.product_name}}
 ****** {{detail.title}} ******
 {% comment %} Lorem_Ipsum_Dolor_Sit_Amet_Dolor_Sit_Amet {% endcomment %}
 {% comment %} By David_Grzyb, {% endcomment %} Published on {
 {detail.created_on}}
```

### Comparing `django_tbase_post_product-2023.5.2716851363/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc` & `django_tbase_post_product-2023.6.216856966/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.5.2716851363/tbase_post/templatetags/post_extras.py` & `django_tbase_post_product-2023.6.216856966/tbase_post/templatetags/post_extras.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.5.2716851363/tbase_post/urls.py` & `django_tbase_post_product-2023.6.216856966/tbase_post/urls.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.5.2716851363/tbase_post/views.py` & `django_tbase_post_product-2023.6.216856966/tbase_post/views.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django.shortcuts import render
 from django.views import View
-from django.http import HttpResponse
-# Create your views here.
 
+# Create your views here.
+from django.http import HttpResponse, Http404
 
 from taggit.models import TaggedItem
 from taggit.models import Tag
 from django.views.generic.base import TemplateView
 from django.views import generic
 from . import models
 # class DetailView(TemplateView):
@@ -76,29 +76,45 @@
         return context
 
 
 class TagListView(generic.ListView):
     model = models.Post
     template_name = 'post/article_list_by_tag.html'
     context_object_name = 'posts'
-    paginate_by = 10
+    paginate_by = 20
     ordering = ['-created_on']
     def get_queryset(self):
         # retrieve the tag from the URL
         tag_slug = self.kwargs['pk']
         # get the tag object based on the slug
         tag = Tag.objects.get(pk=tag_slug)
         # filter articles based on the tag
         articles = self.model.objects.filter(tags=tag)
-
+        # if len(articles)<500:
+        #     print("No articles")
+            # return Http404('project list dose not exist')
         return articles
 
     def get_context_data(self, *args, **kwargs):
         """
 
         """
         context = super().get_context_data(**kwargs)
         # 获取tag的标签
         tag_slug = self.kwargs['pk']
         tag = Tag.objects.get(pk=tag_slug)
         context['title'] = tag
+        # print("context", context)
+   
+        if len(context['object_list'])<10:
+            print("No")
+            context['meta'] = {
+            'noindex':True
+            }
+            # return Http404('project list dose not exist')
+            # return View.defaults.page_not_found()
+            # raise Http404("Poll does not exist")
+        else:
+            context['meta'] = {
+            'noindex':False
+             }
         return context
```

