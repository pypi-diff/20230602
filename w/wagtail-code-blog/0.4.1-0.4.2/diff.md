# Comparing `tmp/wagtail_code_blog-0.4.1.tar.gz` & `tmp/wagtail_code_blog-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_code_blog-0.4.1.tar", max compression
+gzip compressed data, was "wagtail_code_blog-0.4.2.tar", max compression
```

## Comparing `wagtail_code_blog-0.4.1.tar` & `wagtail_code_blog-0.4.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      107 2022-10-31 14:09:25.573057 wagtail_code_blog-0.4.1/README.md
--rw-r--r--   0        0        0     1956 2023-05-13 15:59:24.194338 wagtail_code_blog-0.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-13 14:40:36.156994 wagtail_code_blog-0.4.1/wagtail_code_blog/__init__.py
--rw-r--r--   0        0        0      296 2022-10-31 14:09:25.581057 wagtail_code_blog-0.4.1/wagtail_code_blog/apps.py
--rw-r--r--   0        0        0     1830 2022-10-31 14:09:25.581057 wagtail_code_blog-0.4.1/wagtail_code_blog/migrations/0001_initial.py
--rw-r--r--   0        0        0      382 2022-10-31 14:09:25.581057 wagtail_code_blog-0.4.1/wagtail_code_blog/migrations/0002_auto_20200302_0745.py
--rw-r--r--   0        0        0     1110 2022-10-31 14:09:25.581057 wagtail_code_blog-0.4.1/wagtail_code_blog/migrations/0003_auto_20200307_0845.py
--rw-r--r--   0        0        0      437 2022-10-31 14:09:25.581057 wagtail_code_blog-0.4.1/wagtail_code_blog/migrations/0004_auto_20200317_1728.py
--rw-r--r--   0        0        0      617 2022-10-31 14:09:25.581057 wagtail_code_blog-0.4.1/wagtail_code_blog/migrations/0005_blogindexpage_search_image.py
--rw-r--r--   0        0        0        0 2022-10-31 14:09:25.581057 wagtail_code_blog-0.4.1/wagtail_code_blog/migrations/__init__.py
--rw-r--r--   0        0        0     4407 2023-05-13 14:49:27.525988 wagtail_code_blog-0.4.1/wagtail_code_blog/models.py
--rw-r--r--   0        0        0     2064 2022-10-31 14:09:25.581057 wagtail_code_blog-0.4.1/wagtail_code_blog/static/wagtail_code_blog/css/blog_index_page.css
--rw-r--r--   0        0        0      468 2022-10-31 14:09:25.581057 wagtail_code_blog-0.4.1/wagtail_code_blog/static/wagtail_code_blog/css/markdown_code_blocks.css
--rw-r--r--   0        0        0     4073 2022-10-31 14:09:25.581057 wagtail_code_blog-0.4.1/wagtail_code_blog/static/wagtail_code_blog/css/pygments.css
--rw-r--r--   0        0        0      370 2022-10-31 14:09:25.581057 wagtail_code_blog-0.4.1/wagtail_code_blog/static/wagtail_code_blog/css/responsive_width.css
--rw-r--r--   0        0        0    24556 2022-10-31 14:09:25.581057 wagtail_code_blog-0.4.1/wagtail_code_blog/static/wagtail_code_blog/images/default_user.png
--rw-r--r--   0        0        0     1697 2022-10-31 14:09:25.581057 wagtail_code_blog-0.4.1/wagtail_code_blog/static/wagtail_code_blog/input.css
--rw-r--r--   0        0        0    11299 2023-05-13 15:54:08.102467 wagtail_code_blog-0.4.1/wagtail_code_blog/static/wagtail_code_blog/output.css
--rw-r--r--   0        0        0      208 2022-10-31 14:09:25.581057 wagtail_code_blog-0.4.1/wagtail_code_blog/templates/wagtail_code_blog/blog_index_page.html
--rw-r--r--   0        0        0     1280 2022-10-31 14:09:25.581057 wagtail_code_blog-0.4.1/wagtail_code_blog/templates/wagtail_code_blog/blog_index_page_body.html
--rw-r--r--   0        0        0      216 2022-10-31 14:09:25.581057 wagtail_code_blog-0.4.1/wagtail_code_blog/templates/wagtail_code_blog/blog_index_page_head.html
--rw-r--r--   0        0        0      375 2022-10-31 14:09:25.581057 wagtail_code_blog-0.4.1/wagtail_code_blog/templates/wagtail_code_blog/blog_page.html
--rw-r--r--   0        0        0     1183 2022-10-31 14:09:25.581057 wagtail_code_blog-0.4.1/wagtail_code_blog/templates/wagtail_code_blog/blog_page_body.html
--rw-r--r--   0        0        0      678 2022-10-31 14:09:25.581057 wagtail_code_blog-0.4.1/wagtail_code_blog/templates/wagtail_code_blog/blog_page_head.html
--rw-r--r--   0        0        0      957 2022-10-31 14:09:25.581057 wagtail_code_blog-0.4.1/wagtail_code_blog/templates/wagtail_code_blog/static_dependencies.html
--rw-r--r--   0        0        0     1547 1970-01-01 00:00:00.000000 wagtail_code_blog-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      107 2023-06-02 12:18:02.597368 wagtail_code_blog-0.4.2/README.md
+-rw-r--r--   0        0        0     1955 2023-06-02 12:18:02.597368 wagtail_code_blog-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-02 12:18:02.597368 wagtail_code_blog-0.4.2/wagtail_code_blog/__init__.py
+-rw-r--r--   0        0        0      296 2023-06-02 12:18:02.597368 wagtail_code_blog-0.4.2/wagtail_code_blog/apps.py
+-rw-r--r--   0        0        0     1830 2023-06-02 12:18:02.597368 wagtail_code_blog-0.4.2/wagtail_code_blog/migrations/0001_initial.py
+-rw-r--r--   0        0        0      382 2023-06-02 12:18:02.597368 wagtail_code_blog-0.4.2/wagtail_code_blog/migrations/0002_auto_20200302_0745.py
+-rw-r--r--   0        0        0     1110 2023-06-02 12:18:02.597368 wagtail_code_blog-0.4.2/wagtail_code_blog/migrations/0003_auto_20200307_0845.py
+-rw-r--r--   0        0        0      437 2023-06-02 12:18:02.597368 wagtail_code_blog-0.4.2/wagtail_code_blog/migrations/0004_auto_20200317_1728.py
+-rw-r--r--   0        0        0      617 2023-06-02 12:18:02.597368 wagtail_code_blog-0.4.2/wagtail_code_blog/migrations/0005_blogindexpage_search_image.py
+-rw-r--r--   0        0        0        0 2023-06-02 12:18:02.597368 wagtail_code_blog-0.4.2/wagtail_code_blog/migrations/__init__.py
+-rw-r--r--   0        0        0     4407 2023-06-02 12:18:02.597368 wagtail_code_blog-0.4.2/wagtail_code_blog/models.py
+-rw-r--r--   0        0        0     2064 2023-06-02 12:18:02.597368 wagtail_code_blog-0.4.2/wagtail_code_blog/static/wagtail_code_blog/css/blog_index_page.css
+-rw-r--r--   0        0        0      468 2023-06-02 12:18:02.597368 wagtail_code_blog-0.4.2/wagtail_code_blog/static/wagtail_code_blog/css/markdown_code_blocks.css
+-rw-r--r--   0        0        0     4073 2023-06-02 12:18:02.597368 wagtail_code_blog-0.4.2/wagtail_code_blog/static/wagtail_code_blog/css/pygments.css
+-rw-r--r--   0        0        0      370 2023-06-02 12:18:02.597368 wagtail_code_blog-0.4.2/wagtail_code_blog/static/wagtail_code_blog/css/responsive_width.css
+-rw-r--r--   0        0        0    24556 2023-06-02 12:18:02.597368 wagtail_code_blog-0.4.2/wagtail_code_blog/static/wagtail_code_blog/images/default_user.png
+-rw-r--r--   0        0        0     1697 2023-06-02 12:18:02.597368 wagtail_code_blog-0.4.2/wagtail_code_blog/static/wagtail_code_blog/input.css
+-rw-r--r--   0        0        0    11299 2023-06-02 12:18:16.449607 wagtail_code_blog-0.4.2/wagtail_code_blog/static/wagtail_code_blog/output.css
+-rw-r--r--   0        0        0      208 2023-06-02 12:18:02.597368 wagtail_code_blog-0.4.2/wagtail_code_blog/templates/wagtail_code_blog/blog_index_page.html
+-rw-r--r--   0        0        0     1280 2023-06-02 12:18:02.601368 wagtail_code_blog-0.4.2/wagtail_code_blog/templates/wagtail_code_blog/blog_index_page_body.html
+-rw-r--r--   0        0        0      216 2023-06-02 12:18:02.601368 wagtail_code_blog-0.4.2/wagtail_code_blog/templates/wagtail_code_blog/blog_index_page_head.html
+-rw-r--r--   0        0        0      375 2023-06-02 12:18:02.601368 wagtail_code_blog-0.4.2/wagtail_code_blog/templates/wagtail_code_blog/blog_page.html
+-rw-r--r--   0        0        0     1183 2023-06-02 12:18:02.601368 wagtail_code_blog-0.4.2/wagtail_code_blog/templates/wagtail_code_blog/blog_page_body.html
+-rw-r--r--   0        0        0      678 2023-06-02 12:18:02.601368 wagtail_code_blog-0.4.2/wagtail_code_blog/templates/wagtail_code_blog/blog_page_head.html
+-rw-r--r--   0        0        0      957 2023-06-02 12:18:02.601368 wagtail_code_blog-0.4.2/wagtail_code_blog/templates/wagtail_code_blog/static_dependencies.html
+-rw-r--r--   0        0        0     1423 1970-01-01 00:00:00.000000 wagtail_code_blog-0.4.2/PKG-INFO
```

### Comparing `wagtail_code_blog-0.4.1/pyproject.toml` & `wagtail_code_blog-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "wagtail-code-blog"
-version = "0.4.1"
+version = "0.4.2"
 license = "MIT"
 description = "A wagtail code blog"
 authors = ["Dani Hodovic <dani.hodovic@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/honeylogic-io/wagtail-code-blog"
 repository = "https://github.com/honeylogic-io/wagtail-code-blog"
 documentation = "https://github.com/honeylogic-io/wagtail-code-blog"
@@ -34,15 +34,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 wagtail = "5.*"
 wagtail-metadata = "4.*"
 readtime = "^1.1.1"
-beautifulsoup4 = "4.8"
+beautifulsoup4 = "^4"
 django-json-ld = "^0.0.5 "
 django-model-utils = "^4.2.0"
 django = "4.*"
 
 [tool.poetry.group.dev.dependencies]
 pudb = "2022.1.2"
 pytest = "^7.3.1"
```

### Comparing `wagtail_code_blog-0.4.1/wagtail_code_blog/migrations/0001_initial.py` & `wagtail_code_blog-0.4.2/wagtail_code_blog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_code_blog-0.4.1/wagtail_code_blog/migrations/0003_auto_20200307_0845.py` & `wagtail_code_blog-0.4.2/wagtail_code_blog/migrations/0003_auto_20200307_0845.py`

 * *Files identical despite different names*

### Comparing `wagtail_code_blog-0.4.1/wagtail_code_blog/migrations/0005_blogindexpage_search_image.py` & `wagtail_code_blog-0.4.2/wagtail_code_blog/migrations/0005_blogindexpage_search_image.py`

 * *Files identical despite different names*

### Comparing `wagtail_code_blog-0.4.1/wagtail_code_blog/models.py` & `wagtail_code_blog-0.4.2/wagtail_code_blog/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_code_blog-0.4.1/wagtail_code_blog/static/wagtail_code_blog/css/blog_index_page.css` & `wagtail_code_blog-0.4.2/wagtail_code_blog/static/wagtail_code_blog/css/blog_index_page.css`

 * *Files identical despite different names*

### Comparing `wagtail_code_blog-0.4.1/wagtail_code_blog/static/wagtail_code_blog/css/pygments.css` & `wagtail_code_blog-0.4.2/wagtail_code_blog/static/wagtail_code_blog/css/pygments.css`

 * *Files identical despite different names*

### Comparing `wagtail_code_blog-0.4.1/wagtail_code_blog/static/wagtail_code_blog/images/default_user.png` & `wagtail_code_blog-0.4.2/wagtail_code_blog/static/wagtail_code_blog/images/default_user.png`

 * *Files identical despite different names*

### Comparing `wagtail_code_blog-0.4.1/wagtail_code_blog/static/wagtail_code_blog/input.css` & `wagtail_code_blog-0.4.2/wagtail_code_blog/static/wagtail_code_blog/input.css`

 * *Files identical despite different names*

### Comparing `wagtail_code_blog-0.4.1/wagtail_code_blog/static/wagtail_code_blog/output.css` & `wagtail_code_blog-0.4.2/wagtail_code_blog/static/wagtail_code_blog/output.css`

 * *Files identical despite different names*

### Comparing `wagtail_code_blog-0.4.1/wagtail_code_blog/templates/wagtail_code_blog/blog_index_page_body.html` & `wagtail_code_blog-0.4.2/wagtail_code_blog/templates/wagtail_code_blog/blog_index_page_body.html`

 * *Files identical despite different names*

### Comparing `wagtail_code_blog-0.4.1/wagtail_code_blog/templates/wagtail_code_blog/blog_page_body.html` & `wagtail_code_blog-0.4.2/wagtail_code_blog/templates/wagtail_code_blog/blog_page_body.html`

 * *Files identical despite different names*

### Comparing `wagtail_code_blog-0.4.1/wagtail_code_blog/templates/wagtail_code_blog/blog_page_head.html` & `wagtail_code_blog-0.4.2/wagtail_code_blog/templates/wagtail_code_blog/blog_page_head.html`

 * *Files identical despite different names*

### Comparing `wagtail_code_blog-0.4.1/wagtail_code_blog/templates/wagtail_code_blog/static_dependencies.html` & `wagtail_code_blog-0.4.2/wagtail_code_blog/templates/wagtail_code_blog/static_dependencies.html`

 * *Files identical despite different names*

### Comparing `wagtail_code_blog-0.4.1/PKG-INFO` & `wagtail_code_blog-0.4.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-code-blog
-Version: 0.4.1
+Version: 0.4.2
 Summary: A wagtail code blog
 Home-page: https://github.com/honeylogic-io/wagtail-code-blog
 License: MIT
 Keywords: wagtail,django,blog,cms
 Author: Dani Hodovic
 Author-email: dani.hodovic@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -16,23 +16,21 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: beautifulsoup4 (==4.8)
-Requires-Dist: django (>=4.0.0,<5.0.0)
+Requires-Dist: beautifulsoup4 (>=4,<5)
+Requires-Dist: django (==4.*)
 Requires-Dist: django-json-ld (>=0.0.5,<0.0.6)
 Requires-Dist: django-model-utils (>=4.2.0,<5.0.0)
 Requires-Dist: readtime (>=1.1.1,<2.0.0)
-Requires-Dist: wagtail (>=5.0.0,<6.0.0)
-Requires-Dist: wagtail-metadata (>=4.0.0,<5.0.0)
+Requires-Dist: wagtail (==5.*)
+Requires-Dist: wagtail-metadata (==4.*)
 Project-URL: Documentation, https://github.com/honeylogic-io/wagtail-code-blog
 Project-URL: Repository, https://github.com/honeylogic-io/wagtail-code-blog
 Description-Content-Type: text/markdown
 
 # A code blog for wagtail
 
 Built with wagtail-code-blog:
```

