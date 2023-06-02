# Comparing `tmp/compressbinarytable-0.1.9.tar.gz` & `tmp/compressbinarytable-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compressbinarytable-0.1.9.tar", max compression
+gzip compressed data, was "compressbinarytable-0.2.0.tar", max compression
```

## Comparing `compressbinarytable-0.1.9.tar` & `compressbinarytable-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1113 2023-04-14 14:14:27.887908 compressbinarytable-0.1.9/README.md
--rw-r--r--   0        0        0        0 2023-04-14 10:19:30.058694 compressbinarytable-0.1.9/compressbinarytable/__init__.py
--rw-r--r--   0        0        0     7780 2023-04-14 14:16:55.244395 compressbinarytable-0.1.9/compressbinarytable/compressbinarytable.py
--rw-r--r--   0        0        0      675 2023-04-14 14:17:50.925130 compressbinarytable-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     1912 1970-01-01 00:00:00.000000 compressbinarytable-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-02 10:53:25.410384 compressbinarytable-0.2.0/compressbinarytable/__init__.py
+-rw-r--r--   0        0        0     9578 2023-06-02 11:42:40.491116 compressbinarytable-0.2.0/compressbinarytable/compressbinarytable.py
+-rw-r--r--   0        0        0      700 2023-06-02 11:50:26.852099 compressbinarytable-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1176 2023-06-02 10:53:25.409364 compressbinarytable-0.2.0/README.md
+-rw-r--r--   0        0        0     1912 1970-01-01 00:00:00.000000 compressbinarytable-0.2.0/PKG-INFO
```

### Comparing `compressbinarytable-0.1.9/README.md` & `compressbinarytable-0.2.0/README.md`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-# CompressBinaryTable
- 
-## Basic Usage:
-
-```console
-cbt -i input_file -o output_file -c 
-```
-
-## Options:
-
-```console
--i = input, required 
--o = output, required 
--c = compression 
--d = decompression 
--t = output type, either csv or tsv 
---override = to override output file if it exist 
-```
-
-## Available Python functions:
-
-```
-# Returns numpy array of file as uncompressed, useful for ML (same as load as pandas df, and to_numpy())
-cbt_to_array(compressed_file)
-
-# Returns numpy array of name of the mutations as uncompressed, useful for ML, (same as load pandas df and use df.colums)
-cbt_columns(compressed_file)
-```
-
-## Required file example:
-
-### CSV:
-
-```
-strain_name,mut1,mut2,mut3,mut4,outcome
-strain1,0,1,1,1,1,1
-strain2,0,0,1,1,1,0
-strain3,0,1,0,1,1,0
-strain4,1,1,1,1,1,1
-```
-
-### TSV:
-
-```
-strain_name mut1    mut2    mut3    mut4    outcome
-strain1 0   1   1   1   1   1
-strain2 0   0   1   1   1   0
-strain3 0   1   0   1   1   0
-strain4 1   1   1   1   1   1
-```
-
-### CBT:
-
-```
-1;mut1;mut2;mut3;mut4;outcome
-strain1;6;43;87;102
-strain2;16;43;87;102
-strain3;6;53;78;112
-strain4;61;413;824;942
-```
-
-
-
+# CompressBinaryTable
+ 
+## Basic Usage:
+
+```console
+cbt -i input_file -o output_file -c 
+```
+
+## Options:
+
+```console
+-i = input, required 
+-o = output, required 
+-c = compression 
+-d = decompression 
+-t = output type, either csv or tsv 
+--override = to override output file if it exist 
+```
+
+## Available Python functions:
+
+```
+# Returns numpy array of file as uncompressed, useful for ML (same as load as pandas df, and to_numpy())
+cbt_to_array(compressed_file)
+
+# Returns numpy array of name of the mutations as uncompressed, useful for ML, (same as load pandas df and use df.colums)
+cbt_columns(compressed_file)
+```
+
+## Required file example:
+
+### CSV:
+
+```
+strain_name,mut1,mut2,mut3,mut4,outcome
+strain1,0,1,1,1,1,1
+strain2,0,0,1,1,1,0
+strain3,0,1,0,1,1,0
+strain4,1,1,1,1,1,1
+```
+
+### TSV:
+
+```
+strain_name mut1    mut2    mut3    mut4    outcome
+strain1 0   1   1   1   1   1
+strain2 0   0   1   1   1   0
+strain3 0   1   0   1   1   0
+strain4 1   1   1   1   1   1
+```
+
+### CBT:
+
+```
+1;mut1;mut2;mut3;mut4;outcome
+strain1;6;43;87;102
+strain2;16;43;87;102
+strain3;6;53;78;112
+strain4;61;413;824;942
+```
+
+
+
```

### Comparing `compressbinarytable-0.1.9/pyproject.toml` & `compressbinarytable-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-[tool.poetry]
-name = "compressbinarytable"
-version = "0.1.9"
-repository = "https://github.com/kalininalab/CompressBinaryTable"
-readme = "README.md"
-description = "Compression of binary table"
-authors = ["Alper Yurtseven <alper.yurtseven@helmholtz-hips.de>"]
-classifiers = [
-    "Development Status :: 3 - Alpha",
-    "Operating System :: OS Independent"
-]
-
-[tool.poetry.dependencies]
-python = ">=3.8,<4.0"
-numpy = "^1.21.4"
-pandas = "^1.5.3"
-
-[tool.poetry.dev-dependencies]
-pytest = "^6.2.5"
-
-[tool.poetry.scripts]
-compressbinarytable = "compressbinarytable.compressbinarytable:main"
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
+[tool.poetry]
+name = "compressbinarytable"
+version = "0.2.0"
+repository = "https://github.com/kalininalab/CompressBinaryTable"
+readme = "README.md"
+description = "Compression of binary table"
+authors = ["Alper Yurtseven <alper.yurtseven@helmholtz-hips.de>"]
+classifiers = [
+    "Development Status :: 3 - Alpha",
+    "Operating System :: OS Independent"
+]
+
+[tool.poetry.dependencies]
+python = ">=3.8,<4.0"
+numpy = "^1.21.4"
+pandas = "^1.5.3"
+
+[tool.poetry.dev-dependencies]
+pytest = "^6.2.5"
+
+[tool.poetry.scripts]
+compressbinarytable = "compressbinarytable.compressbinarytable:main"
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `compressbinarytable-0.1.9/PKG-INFO` & `compressbinarytable-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compressbinarytable
-Version: 0.1.9
+Version: 0.2.0
 Summary: Compression of binary table
 Home-page: https://github.com/kalininalab/CompressBinaryTable
 Author: Alper Yurtseven
 Author-email: alper.yurtseven@helmholtz-hips.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
```

