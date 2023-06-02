# Comparing `tmp/phable-0.1.7.tar.gz` & `tmp/phable-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phable-0.1.7.tar", max compression
+gzip compressed data, was "phable-0.1.8.tar", max compression
```

## Comparing `phable-0.1.7.tar` & `phable-0.1.8.tar`

### file list

```diff
@@ -1,10 +1,13 @@
--rw-r--r--   0        0        0     1069 2023-03-18 20:20:49.329618 phable-0.1.7/LICENSE
--rw-r--r--   0        0        0     1208 2023-05-16 00:55:42.481814 phable-0.1.7/README.md
--rw-r--r--   0        0        0        0 2023-03-18 18:42:50.546791 phable-0.1.7/phable/__init__.py
--rw-r--r--   0        0        0     3135 2023-05-07 00:57:47.871901 phable-0.1.7/phable/http.py
--rw-r--r--   0        0        0     8540 2023-05-15 15:18:43.774165 phable-0.1.7/phable/json_parser.py
--rw-r--r--   0        0        0     3188 2023-05-15 15:14:57.155754 phable-0.1.7/phable/kinds.py
--rw-r--r--   0        0        0     4242 2023-05-16 00:48:45.882638 phable-0.1.7/phable/phable.py
--rw-r--r--   0        0        0    15105 2023-05-15 15:11:51.287039 phable-0.1.7/phable/scram.py
--rw-r--r--   0        0        0      721 2023-05-16 00:57:02.754083 phable-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1600 1970-01-01 00:00:00.000000 phable-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-03-18 20:20:49.329618 phable-0.1.8/LICENSE
+-rw-r--r--   0        0        0     2894 2023-06-02 16:37:32.321897 phable-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-03-18 18:42:50.546791 phable-0.1.8/phable/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-02 02:17:33.194840 phable-0.1.8/phable/auth/__init__.py
+-rw-r--r--   0        0        0     7571 2023-06-02 15:16:52.369248 phable-0.1.8/phable/auth/scram.py
+-rw-r--r--   0        0        0     9577 2023-06-02 15:45:01.035920 phable-0.1.8/phable/client.py
+-rw-r--r--   0        0        0      663 2023-06-02 02:25:41.532878 phable-0.1.8/phable/exceptions.py
+-rw-r--r--   0        0        0     1785 2023-06-02 14:50:39.440150 phable-0.1.8/phable/http.py
+-rw-r--r--   0        0        0     4268 2023-06-02 14:33:04.856035 phable-0.1.8/phable/kinds.py
+-rw-r--r--   0        0        0        0 2023-06-02 02:17:33.196550 phable-0.1.8/phable/parser/__init__.py
+-rw-r--r--   0        0        0     4826 2023-06-02 02:17:33.196760 phable-0.1.8/phable/parser/json.py
+-rw-r--r--   0        0        0      721 2023-06-02 16:40:43.139404 phable-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3247 1970-01-01 00:00:00.000000 phable-0.1.8/PKG-INFO
```

### Comparing `phable-0.1.7/LICENSE` & `phable-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `phable-0.1.7/pyproject.toml` & `phable-0.1.8/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "phable"
-version = "0.1.7"
+version = "0.1.8"
 description = ""
 authors = ["Rick Jennings <rjennings055@gmail.com>"]
 readme = "README.md"
 packages = [{include = "phable"}]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.11"
-pandas = "^2.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 flake8 = "^6.0.0"
 mypy = "^1.1.1"
 pytest = "^7.3.0"
 isort = "^5.12.0"
+pandas = "^2.0.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 log_cli = true
```

