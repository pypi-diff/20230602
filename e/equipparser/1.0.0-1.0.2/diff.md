# Comparing `tmp/equipparser-1.0.0.tar.gz` & `tmp/equipparser-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "equipparser-1.0.0.tar", last modified: Fri Jun  2 06:45:44 2023, max compression
+gzip compressed data, was "equipparser-1.0.2.tar", last modified: Fri Jun  2 06:48:26 2023, max compression
```

## Comparing `equipparser-1.0.0.tar` & `equipparser-1.0.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 06:45:44.296808 equipparser-1.0.0/
--rw-rw-rw-   0        0        0     1090 2023-06-02 06:06:24.000000 equipparser-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       60 2023-06-02 06:06:24.000000 equipparser-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      664 2023-06-02 06:45:44.296808 equipparser-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    30185 2023-06-02 06:06:24.000000 equipparser-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 06:45:44.276794 equipparser-1.0.0/equipparser.egg-info/
--rw-rw-rw-   0        0        0      664 2023-06-02 06:45:44.000000 equipparser-1.0.0/equipparser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1032 2023-06-02 06:45:44.000000 equipparser-1.0.0/equipparser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 06:45:44.000000 equipparser-1.0.0/equipparser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      126 2023-06-02 06:45:44.000000 equipparser-1.0.0/equipparser.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2023-06-02 06:45:44.000000 equipparser-1.0.0/equipparser.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-02 06:45:44.000000 equipparser-1.0.0/equipparser.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-02 06:45:44.287806 equipparser-1.0.0/irs_reader/
--rw-rw-rw-   0        0        0        6 2023-06-02 06:06:24.000000 equipparser-1.0.0/irs_reader/__init__.py
--rw-rw-rw-   0        0        0       23 2023-06-02 06:41:38.000000 equipparser-1.0.0/irs_reader/_version.py
--rw-rw-rw-   0        0        0      359 2023-06-02 06:06:24.000000 equipparser-1.0.0/irs_reader/dir_utils.py
--rw-rw-rw-   0        0        0     2266 2023-06-02 06:06:24.000000 equipparser-1.0.0/irs_reader/file_utils.py
--rw-rw-rw-   0        0        0     7724 2023-06-02 06:06:24.000000 equipparser-1.0.0/irs_reader/filing.py
--rw-rw-rw-   0        0        0      549 2023-06-02 06:06:24.000000 equipparser-1.0.0/irs_reader/flatten_utils.py
--rw-rw-rw-   0        0        0     3516 2023-06-02 06:06:24.000000 equipparser-1.0.0/irs_reader/irsx_cli.py
--rw-rw-rw-   0        0        0     1452 2023-06-02 06:06:24.000000 equipparser-1.0.0/irs_reader/irsx_index_cli.py
--rw-rw-rw-   0        0        0     2715 2023-06-02 06:06:24.000000 equipparser-1.0.0/irs_reader/irsx_retrieve_cli.py
--rw-rw-rw-   0        0        0     3487 2023-06-02 06:06:24.000000 equipparser-1.0.0/irs_reader/keyerror_utils.py
--rw-rw-rw-   0        0        0      519 2023-06-02 06:06:24.000000 equipparser-1.0.0/irs_reader/local_settings-example.py
--rw-rw-rw-   0        0        0      630 2023-06-02 06:06:24.000000 equipparser-1.0.0/irs_reader/log_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-02 06:45:44.295807 equipparser-1.0.0/irs_reader/metadata/
--rw-rw-rw-   0        0        0     1157 2023-06-02 06:22:53.000000 equipparser-1.0.0/irs_reader/metadata/.gitignore
--rw-rw-rw-   0        0        0     1069 2023-06-02 06:22:53.000000 equipparser-1.0.0/irs_reader/metadata/LICENSE
--rw-rw-rw-   0        0        0      462 2023-06-02 06:22:53.000000 equipparser-1.0.0/irs_reader/metadata/README.md
--rw-rw-rw-   0        0        0  1194190 2023-06-02 06:22:54.000000 equipparser-1.0.0/irs_reader/metadata/descriptions.csv
--rw-rw-rw-   0        0        0    21662 2023-06-02 06:22:54.000000 equipparser-1.0.0/irs_reader/metadata/groups.csv
--rw-rw-rw-   0        0        0   954575 2023-06-02 06:22:54.000000 equipparser-1.0.0/irs_reader/metadata/line_numbers.csv
--rw-rw-rw-   0        0        0    12778 2023-06-02 06:22:54.000000 equipparser-1.0.0/irs_reader/metadata/schedule_parts.csv
--rw-rw-rw-   0        0        0   945434 2023-06-02 06:22:54.000000 equipparser-1.0.0/irs_reader/metadata/variables.csv
--rw-rw-rw-   0        0        0    66249 2023-06-02 06:06:24.000000 equipparser-1.0.0/irs_reader/object_ids.py
--rw-rw-rw-   0        0        0     2873 2023-06-02 06:06:24.000000 equipparser-1.0.0/irs_reader/settings.py
--rw-rw-rw-   0        0        0    10171 2023-06-02 06:06:24.000000 equipparser-1.0.0/irs_reader/sked_dict_reader.py
--rw-rw-rw-   0        0        0     6698 2023-06-02 06:06:24.000000 equipparser-1.0.0/irs_reader/standardizer.py
--rw-rw-rw-   0        0        0     5547 2023-06-02 06:06:24.000000 equipparser-1.0.0/irs_reader/text_format_utils.py
--rw-rw-rw-   0        0        0      281 2023-06-02 06:06:24.000000 equipparser-1.0.0/irs_reader/type_utils.py
--rw-rw-rw-   0        0        0     7483 2023-06-02 06:06:24.000000 equipparser-1.0.0/irs_reader/xmlrunner.py
--rw-rw-rw-   0        0        0       86 2023-06-02 06:45:44.297807 equipparser-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1749 2023-06-02 06:35:52.000000 equipparser-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 06:48:26.168646 equipparser-1.0.2/
+-rw-rw-rw-   0        0        0     1090 2023-06-02 06:06:24.000000 equipparser-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0       60 2023-06-02 06:06:24.000000 equipparser-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      556 2023-06-02 06:48:26.168646 equipparser-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    30185 2023-06-02 06:06:24.000000 equipparser-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 06:48:26.146633 equipparser-1.0.2/equipparser.egg-info/
+-rw-rw-rw-   0        0        0      556 2023-06-02 06:48:26.000000 equipparser-1.0.2/equipparser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1032 2023-06-02 06:48:26.000000 equipparser-1.0.2/equipparser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 06:48:26.000000 equipparser-1.0.2/equipparser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      126 2023-06-02 06:48:26.000000 equipparser-1.0.2/equipparser.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2023-06-02 06:48:26.000000 equipparser-1.0.2/equipparser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-02 06:48:26.000000 equipparser-1.0.2/equipparser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 06:48:26.159647 equipparser-1.0.2/irs_reader/
+-rw-rw-rw-   0        0        0        6 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-06-02 06:41:38.000000 equipparser-1.0.2/irs_reader/_version.py
+-rw-rw-rw-   0        0        0      359 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/dir_utils.py
+-rw-rw-rw-   0        0        0     2266 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/file_utils.py
+-rw-rw-rw-   0        0        0     7724 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/filing.py
+-rw-rw-rw-   0        0        0      549 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/flatten_utils.py
+-rw-rw-rw-   0        0        0     3516 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/irsx_cli.py
+-rw-rw-rw-   0        0        0     1452 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/irsx_index_cli.py
+-rw-rw-rw-   0        0        0     2715 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/irsx_retrieve_cli.py
+-rw-rw-rw-   0        0        0     3487 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/keyerror_utils.py
+-rw-rw-rw-   0        0        0      519 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/local_settings-example.py
+-rw-rw-rw-   0        0        0      630 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/log_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-02 06:48:26.166646 equipparser-1.0.2/irs_reader/metadata/
+-rw-rw-rw-   0        0        0     1157 2023-06-02 06:22:53.000000 equipparser-1.0.2/irs_reader/metadata/.gitignore
+-rw-rw-rw-   0        0        0     1069 2023-06-02 06:22:53.000000 equipparser-1.0.2/irs_reader/metadata/LICENSE
+-rw-rw-rw-   0        0        0      462 2023-06-02 06:22:53.000000 equipparser-1.0.2/irs_reader/metadata/README.md
+-rw-rw-rw-   0        0        0  1194190 2023-06-02 06:22:54.000000 equipparser-1.0.2/irs_reader/metadata/descriptions.csv
+-rw-rw-rw-   0        0        0    21662 2023-06-02 06:22:54.000000 equipparser-1.0.2/irs_reader/metadata/groups.csv
+-rw-rw-rw-   0        0        0   954575 2023-06-02 06:22:54.000000 equipparser-1.0.2/irs_reader/metadata/line_numbers.csv
+-rw-rw-rw-   0        0        0    12778 2023-06-02 06:22:54.000000 equipparser-1.0.2/irs_reader/metadata/schedule_parts.csv
+-rw-rw-rw-   0        0        0   945434 2023-06-02 06:22:54.000000 equipparser-1.0.2/irs_reader/metadata/variables.csv
+-rw-rw-rw-   0        0        0    66249 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/object_ids.py
+-rw-rw-rw-   0        0        0     2873 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/settings.py
+-rw-rw-rw-   0        0        0    10171 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/sked_dict_reader.py
+-rw-rw-rw-   0        0        0     6698 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/standardizer.py
+-rw-rw-rw-   0        0        0     5547 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/text_format_utils.py
+-rw-rw-rw-   0        0        0      281 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/type_utils.py
+-rw-rw-rw-   0        0        0     7483 2023-06-02 06:06:24.000000 equipparser-1.0.2/irs_reader/xmlrunner.py
+-rw-rw-rw-   0        0        0       86 2023-06-02 06:48:26.169648 equipparser-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1614 2023-06-02 06:48:11.000000 equipparser-1.0.2/setup.py
```

### Comparing `equipparser-1.0.0/LICENSE` & `equipparser-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.0/README.md` & `equipparser-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.0/equipparser.egg-info/SOURCES.txt` & `equipparser-1.0.2/equipparser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.0/irs_reader/file_utils.py` & `equipparser-1.0.2/irs_reader/file_utils.py`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.0/irs_reader/filing.py` & `equipparser-1.0.2/irs_reader/filing.py`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.0/irs_reader/flatten_utils.py` & `equipparser-1.0.2/irs_reader/flatten_utils.py`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.0/irs_reader/irsx_cli.py` & `equipparser-1.0.2/irs_reader/irsx_cli.py`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.0/irs_reader/irsx_index_cli.py` & `equipparser-1.0.2/irs_reader/irsx_index_cli.py`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.0/irs_reader/irsx_retrieve_cli.py` & `equipparser-1.0.2/irs_reader/irsx_retrieve_cli.py`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.0/irs_reader/keyerror_utils.py` & `equipparser-1.0.2/irs_reader/keyerror_utils.py`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.0/irs_reader/local_settings-example.py` & `equipparser-1.0.2/irs_reader/local_settings-example.py`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.0/irs_reader/log_utils.py` & `equipparser-1.0.2/irs_reader/log_utils.py`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.0/irs_reader/metadata/.gitignore` & `equipparser-1.0.2/irs_reader/metadata/.gitignore`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.0/irs_reader/metadata/LICENSE` & `equipparser-1.0.2/irs_reader/metadata/LICENSE`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.0/irs_reader/metadata/descriptions.csv` & `equipparser-1.0.2/irs_reader/metadata/descriptions.csv`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.0/irs_reader/metadata/groups.csv` & `equipparser-1.0.2/irs_reader/metadata/groups.csv`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.0/irs_reader/metadata/line_numbers.csv` & `equipparser-1.0.2/irs_reader/metadata/line_numbers.csv`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.0/irs_reader/metadata/schedule_parts.csv` & `equipparser-1.0.2/irs_reader/metadata/schedule_parts.csv`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.0/irs_reader/metadata/variables.csv` & `equipparser-1.0.2/irs_reader/metadata/variables.csv`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.0/irs_reader/object_ids.py` & `equipparser-1.0.2/irs_reader/object_ids.py`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.0/irs_reader/settings.py` & `equipparser-1.0.2/irs_reader/settings.py`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.0/irs_reader/sked_dict_reader.py` & `equipparser-1.0.2/irs_reader/sked_dict_reader.py`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.0/irs_reader/standardizer.py` & `equipparser-1.0.2/irs_reader/standardizer.py`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.0/irs_reader/text_format_utils.py` & `equipparser-1.0.2/irs_reader/text_format_utils.py`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.0/irs_reader/xmlrunner.py` & `equipparser-1.0.2/irs_reader/xmlrunner.py`

 * *Files identical despite different names*

### Comparing `equipparser-1.0.0/setup.py` & `equipparser-1.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,28 +5,27 @@
 HUMAN_NAME = 'equipparser'
 HERE = os.path.abspath(os.path.dirname(__file__))
 version_ns = {}
 with open(os.path.join(HERE, 'irs_reader', '_version.py')) as f:
     exec(f.read(), {}, version_ns)
 
 setup(name=HUMAN_NAME,
-      description = "Turn the IRS' versioned XML 990's into python objects \
-        with original line number and description.",
-      version = version_ns['__version__'],
+      description = "XML Parser",
+      version = '1.0.2',
       author = 'Vishal Avalani',
       author_email = 'vishal.avalani@gmail.com',
       url = 'https://github.com/vishalavalani/990-xml-reader',
       license = 'MIT',
       setup_requires = ["setuptools", ],
       install_requires = ['requests', 'xmltodict', 'unicodecsv'],
       tests_require = ['nose', 'requests', 'xmltodict', 'unicodecsv', 'tox', 'tox-pyenv',],
       packages = ['irsx'],
       package_dir = {'irsx': 'irs_reader'},
       package_data = {'irsx': ['metadata/*.csv']},
-      keywords = ['990', 'nonprofit', 'tax'],
+      keywords = ['XML'],
       entry_points = {
           "console_scripts": ["irsx=irsx.irsx_cli:main",
                               "irsx_index=irsx.irsx_index_cli:main",
                               "irsx_retrieve=irsx.irsx_retrieve_cli:main"]
       },
       classifiers=[
           # How mature is this project? Common values are
```

