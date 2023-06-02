# Comparing `tmp/equipparser-1.0.2.tar.gz` & `tmp/equipparser-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "equipparser-1.0.2.tar", last modified: Fri Jun  2 06:48:26 2023, max compression
+gzip compressed data, was "equipparser-1.0.3.tar", last modified: Fri Jun  2 07:11:35 2023, max compression
```

## Comparing `equipparser-1.0.2.tar` & `equipparser-1.0.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 06:48:26.168646 equipparser-1.0.2/
--rw-rw-rw-   0        0        0     1090 2023-06-02 06:06:24.000000 equipparser-1.0.2/LICENSE
--rw-rw-rw-   0        0        0       60 2023-06-02 06:06:24.000000 equipparser-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      556 2023-06-02 06:48:26.168646 equipparser-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    30185 2023-06-02 06:06:24.000000 equipparser-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 06:48:26.146633 equipparser-1.0.2/equipparser.egg-info/
--rw-rw-rw-   0        0        0      556 2023-06-02 06:48:26.000000 equipparser-1.0.2/equipparser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1032 2023-06-02 06:48:26.000000 equipparser-1.0.2/equipparser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 06:48:26.000000 equipparser-1.0.2/equipparser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      126 2023-06-02 06:48:26.000000 equipparser-1.0.2/equipparser.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2023-06-02 06:48:26.000000 equipparser-1.0.2/equipparser.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-02 06:48:26.000000 equipparser-1.0.2/equipparser.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-02 06:48:26.159647 equipparser-1.0.2/irs_reader/
--rw-rw-rw-   0        0        0        6 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/__init__.py
--rw-rw-rw-   0        0        0       23 2023-06-02 06:41:38.000000 equipparser-1.0.2/irs_reader/_version.py
--rw-rw-rw-   0        0        0      359 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/dir_utils.py
--rw-rw-rw-   0        0        0     2266 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/file_utils.py
--rw-rw-rw-   0        0        0     7724 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/filing.py
--rw-rw-rw-   0        0        0      549 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/flatten_utils.py
--rw-rw-rw-   0        0        0     3516 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/irsx_cli.py
--rw-rw-rw-   0        0        0     1452 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/irsx_index_cli.py
--rw-rw-rw-   0        0        0     2715 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/irsx_retrieve_cli.py
--rw-rw-rw-   0        0        0     3487 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/keyerror_utils.py
--rw-rw-rw-   0        0        0      519 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/local_settings-example.py
--rw-rw-rw-   0        0        0      630 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/log_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-02 06:48:26.166646 equipparser-1.0.2/irs_reader/metadata/
--rw-rw-rw-   0        0        0     1157 2023-06-02 06:22:53.000000 equipparser-1.0.2/irs_reader/metadata/.gitignore
--rw-rw-rw-   0        0        0     1069 2023-06-02 06:22:53.000000 equipparser-1.0.2/irs_reader/metadata/LICENSE
--rw-rw-rw-   0        0        0      462 2023-06-02 06:22:53.000000 equipparser-1.0.2/irs_reader/metadata/README.md
--rw-rw-rw-   0        0        0  1194190 2023-06-02 06:22:54.000000 equipparser-1.0.2/irs_reader/metadata/descriptions.csv
--rw-rw-rw-   0        0        0    21662 2023-06-02 06:22:54.000000 equipparser-1.0.2/irs_reader/metadata/groups.csv
--rw-rw-rw-   0        0        0   954575 2023-06-02 06:22:54.000000 equipparser-1.0.2/irs_reader/metadata/line_numbers.csv
--rw-rw-rw-   0        0        0    12778 2023-06-02 06:22:54.000000 equipparser-1.0.2/irs_reader/metadata/schedule_parts.csv
--rw-rw-rw-   0        0        0   945434 2023-06-02 06:22:54.000000 equipparser-1.0.2/irs_reader/metadata/variables.csv
--rw-rw-rw-   0        0        0    66249 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/object_ids.py
--rw-rw-rw-   0        0        0     2873 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/settings.py
--rw-rw-rw-   0        0        0    10171 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/sked_dict_reader.py
--rw-rw-rw-   0        0        0     6698 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/standardizer.py
--rw-rw-rw-   0        0        0     5547 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/text_format_utils.py
--rw-rw-rw-   0        0        0      281 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/type_utils.py
--rw-rw-rw-   0        0        0     7483 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/xmlrunner.py
--rw-rw-rw-   0        0        0       86 2023-06-02 06:48:26.169648 equipparser-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1614 2023-06-02 06:48:11.000000 equipparser-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 07:11:35.070395 equipparser-1.0.3/
+-rw-rw-rw-   0        0        0     1090 2023-06-02 06:06:24.000000 equipparser-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0       60 2023-06-02 06:06:24.000000 equipparser-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      556 2023-06-02 07:11:35.070395 equipparser-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    30185 2023-06-02 06:06:24.000000 equipparser-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 07:11:35.005280 equipparser-1.0.3/equipparser.egg-info/
+-rw-rw-rw-   0        0        0      556 2023-06-02 07:11:34.000000 equipparser-1.0.3/equipparser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1032 2023-06-02 07:11:34.000000 equipparser-1.0.3/equipparser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 07:11:34.000000 equipparser-1.0.3/equipparser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      154 2023-06-02 07:11:34.000000 equipparser-1.0.3/equipparser.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2023-06-02 07:11:34.000000 equipparser-1.0.3/equipparser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-02 07:11:34.000000 equipparser-1.0.3/equipparser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 07:11:35.019853 equipparser-1.0.3/irs_reader/
+-rw-rw-rw-   0        0        0        6 2023-06-02 06:06:24.000000 equipparser-1.0.3/irs_reader/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-06-02 06:41:38.000000 equipparser-1.0.3/irs_reader/_version.py
+-rw-rw-rw-   0        0        0      359 2023-06-02 06:06:24.000000 equipparser-1.0.3/irs_reader/dir_utils.py
+-rw-rw-rw-   0        0        0     2266 2023-06-02 06:06:24.000000 equipparser-1.0.3/irs_reader/file_utils.py
+-rw-rw-rw-   0        0        0     7724 2023-06-02 06:06:24.000000 equipparser-1.0.3/irs_reader/filing.py
+-rw-rw-rw-   0        0        0      549 2023-06-02 06:06:24.000000 equipparser-1.0.3/irs_reader/flatten_utils.py
+-rw-rw-rw-   0        0        0     3516 2023-06-02 06:06:24.000000 equipparser-1.0.3/irs_reader/irsx_cli.py
+-rw-rw-rw-   0        0        0     1452 2023-06-02 06:06:24.000000 equipparser-1.0.3/irs_reader/irsx_index_cli.py
+-rw-rw-rw-   0        0        0     2715 2023-06-02 06:06:24.000000 equipparser-1.0.3/irs_reader/irsx_retrieve_cli.py
+-rw-rw-rw-   0        0        0     3487 2023-06-02 06:06:24.000000 equipparser-1.0.3/irs_reader/keyerror_utils.py
+-rw-rw-rw-   0        0        0      519 2023-06-02 06:06:24.000000 equipparser-1.0.3/irs_reader/local_settings-example.py
+-rw-rw-rw-   0        0        0      630 2023-06-02 06:06:24.000000 equipparser-1.0.3/irs_reader/log_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-02 07:11:35.068397 equipparser-1.0.3/irs_reader/metadata/
+-rw-rw-rw-   0        0        0     1157 2023-06-02 06:22:53.000000 equipparser-1.0.3/irs_reader/metadata/.gitignore
+-rw-rw-rw-   0        0        0     1069 2023-06-02 06:22:53.000000 equipparser-1.0.3/irs_reader/metadata/LICENSE
+-rw-rw-rw-   0        0        0      462 2023-06-02 06:22:53.000000 equipparser-1.0.3/irs_reader/metadata/README.md
+-rw-rw-rw-   0        0        0  1194190 2023-06-02 06:22:54.000000 equipparser-1.0.3/irs_reader/metadata/descriptions.csv
+-rw-rw-rw-   0        0        0    21662 2023-06-02 06:22:54.000000 equipparser-1.0.3/irs_reader/metadata/groups.csv
+-rw-rw-rw-   0        0        0   954575 2023-06-02 06:22:54.000000 equipparser-1.0.3/irs_reader/metadata/line_numbers.csv
+-rw-rw-rw-   0        0        0    12778 2023-06-02 06:22:54.000000 equipparser-1.0.3/irs_reader/metadata/schedule_parts.csv
+-rw-rw-rw-   0        0        0   945434 2023-06-02 06:22:54.000000 equipparser-1.0.3/irs_reader/metadata/variables.csv
+-rw-rw-rw-   0        0        0    66249 2023-06-02 06:06:24.000000 equipparser-1.0.3/irs_reader/object_ids.py
+-rw-rw-rw-   0        0        0     2873 2023-06-02 06:06:24.000000 equipparser-1.0.3/irs_reader/settings.py
+-rw-rw-rw-   0        0        0    10171 2023-06-02 06:06:24.000000 equipparser-1.0.3/irs_reader/sked_dict_reader.py
+-rw-rw-rw-   0        0        0     6698 2023-06-02 06:06:24.000000 equipparser-1.0.3/irs_reader/standardizer.py
+-rw-rw-rw-   0        0        0     5547 2023-06-02 06:06:24.000000 equipparser-1.0.3/irs_reader/text_format_utils.py
+-rw-rw-rw-   0        0        0      281 2023-06-02 06:06:24.000000 equipparser-1.0.3/irs_reader/type_utils.py
+-rw-rw-rw-   0        0        0     7483 2023-06-02 06:06:24.000000 equipparser-1.0.3/irs_reader/xmlrunner.py
+-rw-rw-rw-   0        0        0       86 2023-06-02 07:11:35.071395 equipparser-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1663 2023-06-02 07:11:05.000000 equipparser-1.0.3/setup.py
```

### Comparing `equipparser-1.0.2/LICENSE` & `equipparser-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.2/PKG-INFO` & `equipparser-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equipparser
-Version: 1.0.2
+Version: 1.0.3
 Summary: XML Parser
 Home-page: https://github.com/vishalavalani/990-xml-reader
 Author: Vishal Avalani
 Author-email: vishal.avalani@gmail.com
 License: MIT
 Keywords: XML
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `equipparser-1.0.2/README.md` & `equipparser-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.2/equipparser.egg-info/PKG-INFO` & `equipparser-1.0.3/equipparser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equipparser
-Version: 1.0.2
+Version: 1.0.3
 Summary: XML Parser
 Home-page: https://github.com/vishalavalani/990-xml-reader
 Author: Vishal Avalani
 Author-email: vishal.avalani@gmail.com
 License: MIT
 Keywords: XML
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `equipparser-1.0.2/equipparser.egg-info/SOURCES.txt` & `equipparser-1.0.3/equipparser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.2/irs_reader/file_utils.py` & `equipparser-1.0.3/irs_reader/file_utils.py`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.2/irs_reader/filing.py` & `equipparser-1.0.3/irs_reader/filing.py`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.2/irs_reader/flatten_utils.py` & `equipparser-1.0.3/irs_reader/flatten_utils.py`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.2/irs_reader/irsx_cli.py` & `equipparser-1.0.3/irs_reader/irsx_cli.py`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.2/irs_reader/irsx_index_cli.py` & `equipparser-1.0.3/irs_reader/irsx_index_cli.py`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.2/irs_reader/irsx_retrieve_cli.py` & `equipparser-1.0.3/irs_reader/irsx_retrieve_cli.py`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.2/irs_reader/keyerror_utils.py` & `equipparser-1.0.3/irs_reader/keyerror_utils.py`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.2/irs_reader/local_settings-example.py` & `equipparser-1.0.3/irs_reader/local_settings-example.py`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.2/irs_reader/log_utils.py` & `equipparser-1.0.3/irs_reader/log_utils.py`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.2/irs_reader/metadata/.gitignore` & `equipparser-1.0.3/irs_reader/metadata/.gitignore`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.2/irs_reader/metadata/LICENSE` & `equipparser-1.0.3/irs_reader/metadata/LICENSE`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.2/irs_reader/metadata/descriptions.csv` & `equipparser-1.0.3/irs_reader/metadata/descriptions.csv`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.2/irs_reader/metadata/groups.csv` & `equipparser-1.0.3/irs_reader/metadata/groups.csv`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.2/irs_reader/metadata/line_numbers.csv` & `equipparser-1.0.3/irs_reader/metadata/line_numbers.csv`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.2/irs_reader/metadata/schedule_parts.csv` & `equipparser-1.0.3/irs_reader/metadata/schedule_parts.csv`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.2/irs_reader/metadata/variables.csv` & `equipparser-1.0.3/irs_reader/metadata/variables.csv`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.2/irs_reader/object_ids.py` & `equipparser-1.0.3/irs_reader/object_ids.py`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.2/irs_reader/settings.py` & `equipparser-1.0.3/irs_reader/settings.py`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.2/irs_reader/sked_dict_reader.py` & `equipparser-1.0.3/irs_reader/sked_dict_reader.py`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.2/irs_reader/standardizer.py` & `equipparser-1.0.3/irs_reader/standardizer.py`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.2/irs_reader/text_format_utils.py` & `equipparser-1.0.3/irs_reader/text_format_utils.py`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.2/irs_reader/xmlrunner.py` & `equipparser-1.0.3/irs_reader/xmlrunner.py`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.2/setup.py` & `equipparser-1.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 HERE = os.path.abspath(os.path.dirname(__file__))
 version_ns = {}
 with open(os.path.join(HERE, 'irs_reader', '_version.py')) as f:
     exec(f.read(), {}, version_ns)
 
 setup(name=HUMAN_NAME,
       description = "XML Parser",
-      version = '1.0.2',
+      version = '1.0.3',
       author = 'Vishal Avalani',
       author_email = 'vishal.avalani@gmail.com',
       url = 'https://github.com/vishalavalani/990-xml-reader',
       license = 'MIT',
       setup_requires = ["setuptools", ],
       install_requires = ['requests', 'xmltodict', 'unicodecsv'],
       tests_require = ['nose', 'requests', 'xmltodict', 'unicodecsv', 'tox', 'tox-pyenv',],
-      packages = ['irsx'],
-      package_dir = {'irsx': 'irs_reader'},
-      package_data = {'irsx': ['metadata/*.csv']},
+      packages = ['equipparser'],
+      package_dir = {'equipparser': 'irs_reader'},
+      package_data = {'equipparser': ['metadata/*.csv']},
       keywords = ['XML'],
       entry_points = {
-          "console_scripts": ["irsx=irsx.irsx_cli:main",
-                              "irsx_index=irsx.irsx_index_cli:main",
-                              "irsx_retrieve=irsx.irsx_retrieve_cli:main"]
+          "console_scripts": ["equipparser=equipparser.irsx_cli:main",
+                              "irsx_index=equipparser.irsx_index_cli:main",
+                              "irsx_retrieve=equipparser.irsx_retrieve_cli:main"]
       },
       classifiers=[
           # How mature is this project? Common values are
           #   3 - Alpha
           #   4 - Beta
           #   5 - Production/Stable
           'Development Status :: 3 - Alpha',
```

