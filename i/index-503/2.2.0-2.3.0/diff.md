# Comparing `tmp/index_503-2.2.0.tar.gz` & `tmp/index_503-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "index_503-2.2.0.tar", max compression
+gzip compressed data, was "index_503-2.3.0.tar", max compression
```

## Comparing `index_503-2.2.0.tar` & `index_503-2.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1072 2023-06-02 12:04:11.586886 index_503-2.2.0/LICENSE
--rw-r--r--   0        0        0     3477 2023-06-02 12:04:11.586886 index_503-2.2.0/README.md
--rw-r--r--   0        0        0     2299 2023-06-02 12:04:12.386897 index_503-2.2.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-02 12:04:12.342896 index_503-2.2.0/src/index_503/__init__.py
--rw-r--r--   0        0        0     1147 2023-06-02 12:04:11.586886 index_503-2.2.0/src/index_503/cache.py
--rw-r--r--   0        0        0     1336 2023-06-02 12:04:11.586886 index_503-2.2.0/src/index_503/file.py
--rw-r--r--   0        0        0     6936 2023-06-02 12:04:11.586886 index_503-2.2.0/src/index_503/index.py
--rw-r--r--   0        0        0      434 2023-06-02 12:04:11.586886 index_503-2.2.0/src/index_503/main.py
--rw-r--r--   0        0        0     1840 2023-06-02 12:04:11.586886 index_503-2.2.0/src/index_503/metadata.py
--rw-r--r--   0        0        0     2384 2023-06-02 12:04:11.586886 index_503-2.2.0/src/index_503/page_generator.py
--rw-r--r--   0        0        0        0 2023-06-02 12:04:11.586886 index_503-2.2.0/src/index_503/py.typed
--rw-r--r--   0        0        0     1513 2023-06-02 12:04:11.586886 index_503-2.2.0/src/index_503/util.py
--rw-r--r--   0        0        0     5152 2023-06-02 12:04:11.586886 index_503-2.2.0/src/index_503/wheel_file.py
--rw-r--r--   0        0        0     4742 1970-01-01 00:00:00.000000 index_503-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-02 12:16:05.855511 index_503-2.3.0/LICENSE
+-rw-r--r--   0        0        0     3810 2023-06-02 12:16:05.855511 index_503-2.3.0/README.md
+-rw-r--r--   0        0        0     2299 2023-06-02 12:16:06.851519 index_503-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-02 12:16:06.799519 index_503-2.3.0/src/index_503/__init__.py
+-rw-r--r--   0        0        0     1147 2023-06-02 12:16:05.855511 index_503-2.3.0/src/index_503/cache.py
+-rw-r--r--   0        0        0     1336 2023-06-02 12:16:05.855511 index_503-2.3.0/src/index_503/file.py
+-rw-r--r--   0        0        0     6936 2023-06-02 12:16:05.855511 index_503-2.3.0/src/index_503/index.py
+-rw-r--r--   0        0        0      434 2023-06-02 12:16:05.855511 index_503-2.3.0/src/index_503/main.py
+-rw-r--r--   0        0        0     1840 2023-06-02 12:16:05.855511 index_503-2.3.0/src/index_503/metadata.py
+-rw-r--r--   0        0        0     2384 2023-06-02 12:16:05.855511 index_503-2.3.0/src/index_503/page_generator.py
+-rw-r--r--   0        0        0        0 2023-06-02 12:16:05.855511 index_503-2.3.0/src/index_503/py.typed
+-rw-r--r--   0        0        0     1513 2023-06-02 12:16:05.855511 index_503-2.3.0/src/index_503/util.py
+-rw-r--r--   0        0        0     5152 2023-06-02 12:16:05.855511 index_503-2.3.0/src/index_503/wheel_file.py
+-rw-r--r--   0        0        0     5075 1970-01-01 00:00:00.000000 index_503-2.3.0/PKG-INFO
```

### Comparing `index_503-2.2.0/LICENSE` & `index_503-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `index_503-2.2.0/README.md` & `index_503-2.3.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -40,14 +40,22 @@
 
 This will produce a `musllinux-index` directory with a PEP 503 index symlinked to the original directory without disturbing the original directory.
 
 Running this again will replace the original index and delete the old index in an atomic manner.
 
 A lock will be held in the parent directory to prevent concurrent executions.
 
+## Example
+
+For image builds
+`pip3 install --no-cache-dir --dry-run --only-binary=:all: --index-url "https://wheels.koston.org/musllinux-index/" -r requirements.txt`
+
+For run time installs
+`pip3 install --no-cache-dir --dry-run --only-binary=:all: --extra-index-url "https://wheels.koston.org/musllinux-index/" -r requirements.txt`
+
 ## Installation
 
 Install this via pip (or your favourite package manager):
 
 `pip install index-503`
 
 ## Credits
```

#### html2text {}

```diff
@@ -3,13 +3,18 @@
                          [Poetry] [black] [pre-commit]
              [PyPI_Version] [Supported Python versions] [License]
 PEP 503 index builder ## Usage If you have a directory full of wheels like
 `musllinux`: `index-503 musllinux` This will produce a `musllinux-index`
 directory with a PEP 503 index symlinked to the original directory without
 disturbing the original directory. Running this again will replace the original
 index and delete the old index in an atomic manner. A lock will be held in the
-parent directory to prevent concurrent executions. ## Installation Install this
-via pip (or your favourite package manager): `pip install index-503` ## Credits
-This package was created with [Copier](https://copier.readthedocs.io/) and the
-[browniebroke/pypackage-template](https://github.com/browniebroke/pypackage-
-template) project template. This project borrows heavily from Dominic Davis-
-Foster's simple503 https://github.com/repo-helper/simple503
+parent directory to prevent concurrent executions. ## Example For image builds
+`pip3 install --no-cache-dir --dry-run --only-binary=:all: --index-url "https:/
+/wheels.koston.org/musllinux-index/" -r requirements.txt` For run time installs
+`pip3 install --no-cache-dir --dry-run --only-binary=:all: --extra-index-url
+"https://wheels.koston.org/musllinux-index/" -r requirements.txt` ##
+Installation Install this via pip (or your favourite package manager): `pip
+install index-503` ## Credits This package was created with [Copier](https://
+copier.readthedocs.io/) and the [browniebroke/pypackage-template](https://
+github.com/browniebroke/pypackage-template) project template. This project
+borrows heavily from Dominic Davis-Foster's simple503 https://github.com/repo-
+helper/simple503
```

### Comparing `index_503-2.2.0/pyproject.toml` & `index_503-2.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "index-503"
-version = "2.2.0"
+version = "2.3.0"
 description = "PEP 503 index builder"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bdraco/index-503"
 documentation = "https://index-503.readthedocs.io"
 classifiers = [
```

### Comparing `index_503-2.2.0/src/index_503/cache.py` & `index_503-2.3.0/src/index_503/cache.py`

 * *Files identical despite different names*

### Comparing `index_503-2.2.0/src/index_503/file.py` & `index_503-2.3.0/src/index_503/file.py`

 * *Files identical despite different names*

### Comparing `index_503-2.2.0/src/index_503/index.py` & `index_503-2.3.0/src/index_503/index.py`

 * *Files identical despite different names*

### Comparing `index_503-2.2.0/src/index_503/metadata.py` & `index_503-2.3.0/src/index_503/metadata.py`

 * *Files identical despite different names*

### Comparing `index_503-2.2.0/src/index_503/page_generator.py` & `index_503-2.3.0/src/index_503/page_generator.py`

 * *Files identical despite different names*

### Comparing `index_503-2.2.0/src/index_503/util.py` & `index_503-2.3.0/src/index_503/util.py`

 * *Files identical despite different names*

### Comparing `index_503-2.2.0/src/index_503/wheel_file.py` & `index_503-2.3.0/src/index_503/wheel_file.py`

 * *Files identical despite different names*

### Comparing `index_503-2.2.0/PKG-INFO` & `index_503-2.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: index-503
-Version: 2.2.0
+Version: 2.3.0
 Summary: PEP 503 index builder
 Home-page: https://github.com/bdraco/index-503
 License: MIT
 Author: J. Nick Koston
 Author-email: nick@koston.org
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -71,14 +71,22 @@
 
 This will produce a `musllinux-index` directory with a PEP 503 index symlinked to the original directory without disturbing the original directory.
 
 Running this again will replace the original index and delete the old index in an atomic manner.
 
 A lock will be held in the parent directory to prevent concurrent executions.
 
+## Example
+
+For image builds
+`pip3 install --no-cache-dir --dry-run --only-binary=:all: --index-url "https://wheels.koston.org/musllinux-index/" -r requirements.txt`
+
+For run time installs
+`pip3 install --no-cache-dir --dry-run --only-binary=:all: --extra-index-url "https://wheels.koston.org/musllinux-index/" -r requirements.txt`
+
 ## Installation
 
 Install this via pip (or your favourite package manager):
 
 `pip install index-503`
 
 ## Credits
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: index-503 Version: 2.2.0 Summary: PEP 503 index
+Metadata-Version: 2.1 Name: index-503 Version: 2.3.0 Summary: PEP 503 index
 builder Home-page: https://github.com/bdraco/index-503 License: MIT Author: J.
 Nick Koston Author-email: nick@koston.org Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
@@ -20,13 +20,18 @@
                          [Poetry] [black] [pre-commit]
              [PyPI_Version] [Supported Python versions] [License]
 PEP 503 index builder ## Usage If you have a directory full of wheels like
 `musllinux`: `index-503 musllinux` This will produce a `musllinux-index`
 directory with a PEP 503 index symlinked to the original directory without
 disturbing the original directory. Running this again will replace the original
 index and delete the old index in an atomic manner. A lock will be held in the
-parent directory to prevent concurrent executions. ## Installation Install this
-via pip (or your favourite package manager): `pip install index-503` ## Credits
-This package was created with [Copier](https://copier.readthedocs.io/) and the
-[browniebroke/pypackage-template](https://github.com/browniebroke/pypackage-
-template) project template. This project borrows heavily from Dominic Davis-
-Foster's simple503 https://github.com/repo-helper/simple503
+parent directory to prevent concurrent executions. ## Example For image builds
+`pip3 install --no-cache-dir --dry-run --only-binary=:all: --index-url "https:/
+/wheels.koston.org/musllinux-index/" -r requirements.txt` For run time installs
+`pip3 install --no-cache-dir --dry-run --only-binary=:all: --extra-index-url
+"https://wheels.koston.org/musllinux-index/" -r requirements.txt` ##
+Installation Install this via pip (or your favourite package manager): `pip
+install index-503` ## Credits This package was created with [Copier](https://
+copier.readthedocs.io/) and the [browniebroke/pypackage-template](https://
+github.com/browniebroke/pypackage-template) project template. This project
+borrows heavily from Dominic Davis-Foster's simple503 https://github.com/repo-
+helper/simple503
```

