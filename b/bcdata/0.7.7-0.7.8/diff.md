# Comparing `tmp/bcdata-0.7.7.tar.gz` & `tmp/bcdata-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcdata-0.7.7.tar", last modified: Thu Apr 13 19:52:21 2023, max compression
+gzip compressed data, was "bcdata-0.7.8.tar", last modified: Fri Jun  2 00:01:56 2023, max compression
```

## Comparing `bcdata-0.7.7.tar` & `bcdata-0.7.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-04-13 19:52:21.462252 bcdata-0.7.7/
--rw-r--r--   0 snorris    (501) staff       (20)     6314 2023-04-13 19:45:00.000000 bcdata-0.7.7/CHANGES.txt
--rw-r--r--   0 snorris    (501) staff       (20)     1080 2018-01-17 01:59:21.000000 bcdata-0.7.7/LICENSE.txt
--rw-r--r--   0 snorris    (501) staff       (20)    16421 2023-04-13 19:52:21.462130 bcdata-0.7.7/PKG-INFO
--rw-r--r--   0 snorris    (501) staff       (20)    15601 2023-04-13 19:41:37.000000 bcdata-0.7.7/README.md
-drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-04-13 19:52:21.460509 bcdata-0.7.7/bcdata/
--rw-r--r--   0 snorris    (501) staff       (20)      349 2023-04-13 19:42:43.000000 bcdata-0.7.7/bcdata/__init__.py
--rw-r--r--   0 snorris    (501) staff       (20)     5267 2022-09-26 21:48:59.000000 bcdata-0.7.7/bcdata/bc2pg.py
--rw-r--r--   0 snorris    (501) staff       (20)     3876 2022-11-18 22:34:58.000000 bcdata-0.7.7/bcdata/bcdc.py
--rw-r--r--   0 snorris    (501) staff       (20)     9795 2023-04-13 19:45:53.000000 bcdata-0.7.7/bcdata/cli.py
--rw-r--r--   0 snorris    (501) staff       (20)     6342 2022-09-29 00:22:24.000000 bcdata-0.7.7/bcdata/database.py
--rw-r--r--   0 snorris    (501) staff       (20)     3034 2022-11-18 22:34:58.000000 bcdata-0.7.7/bcdata/wcs.py
--rw-r--r--   0 snorris    (501) staff       (20)    11387 2023-04-13 19:45:53.000000 bcdata-0.7.7/bcdata/wfs.py
-drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-04-13 19:52:21.461455 bcdata-0.7.7/bcdata.egg-info/
--rw-r--r--   0 snorris    (501) staff       (20)    16421 2023-04-13 19:52:21.000000 bcdata-0.7.7/bcdata.egg-info/PKG-INFO
--rw-r--r--   0 snorris    (501) staff       (20)      474 2023-04-13 19:52:21.000000 bcdata-0.7.7/bcdata.egg-info/SOURCES.txt
--rw-r--r--   0 snorris    (501) staff       (20)        1 2023-04-13 19:52:21.000000 bcdata-0.7.7/bcdata.egg-info/dependency_links.txt
--rw-r--r--   0 snorris    (501) staff       (20)       42 2023-04-13 19:52:21.000000 bcdata-0.7.7/bcdata.egg-info/entry_points.txt
--rw-r--r--   0 snorris    (501) staff       (20)        1 2019-11-08 06:25:25.000000 bcdata-0.7.7/bcdata.egg-info/not-zip-safe
--rw-r--r--   0 snorris    (501) staff       (20)      123 2023-04-13 19:52:21.000000 bcdata-0.7.7/bcdata.egg-info/requires.txt
--rw-r--r--   0 snorris    (501) staff       (20)        7 2023-04-13 19:52:21.000000 bcdata-0.7.7/bcdata.egg-info/top_level.txt
--rw-r--r--   0 snorris    (501) staff       (20)      173 2022-07-16 00:28:03.000000 bcdata-0.7.7/pyproject.toml
--rw-r--r--   0 snorris    (501) staff       (20)      104 2023-02-01 22:20:34.000000 bcdata-0.7.7/requirements.txt
--rw-r--r--   0 snorris    (501) staff       (20)       38 2023-04-13 19:52:21.462284 bcdata-0.7.7/setup.cfg
--rw-r--r--   0 snorris    (501) staff       (20)     1732 2022-07-20 16:54:44.000000 bcdata-0.7.7/setup.py
-drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-04-13 19:52:21.461974 bcdata-0.7.7/tests/
--rw-r--r--   0 snorris    (501) staff       (20)     3851 2022-11-18 21:53:34.000000 bcdata-0.7.7/tests/test_bc2pg.py
--rw-r--r--   0 snorris    (501) staff       (20)     6049 2023-04-13 19:25:05.000000 bcdata-0.7.7/tests/test_bcdata.py
--rw-r--r--   0 snorris    (501) staff       (20)    11548 2022-07-20 16:54:44.000000 bcdata-0.7.7/tests/test_bcdc.py
--rw-r--r--   0 snorris    (501) staff       (20)     2393 2022-07-20 16:54:44.000000 bcdata-0.7.7/tests/test_cli.py
+drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-06-02 00:01:56.715017 bcdata-0.7.8/
+-rw-r--r--   0 snorris    (501) staff       (20)     6388 2023-06-02 00:00:04.000000 bcdata-0.7.8/CHANGES.txt
+-rw-r--r--   0 snorris    (501) staff       (20)     1080 2018-01-17 01:59:21.000000 bcdata-0.7.8/LICENSE.txt
+-rw-r--r--   0 snorris    (501) staff       (20)    16453 2023-06-02 00:01:56.714888 bcdata-0.7.8/PKG-INFO
+-rw-r--r--   0 snorris    (501) staff       (20)    15633 2023-06-02 00:00:04.000000 bcdata-0.7.8/README.md
+drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-06-02 00:01:56.712977 bcdata-0.7.8/bcdata/
+-rw-r--r--   0 snorris    (501) staff       (20)      349 2023-06-02 00:00:04.000000 bcdata-0.7.8/bcdata/__init__.py
+-rw-r--r--   0 snorris    (501) staff       (20)     5267 2022-09-26 21:48:59.000000 bcdata-0.7.8/bcdata/bc2pg.py
+-rw-r--r--   0 snorris    (501) staff       (20)     3876 2022-11-18 22:34:58.000000 bcdata-0.7.8/bcdata/bcdc.py
+-rw-r--r--   0 snorris    (501) staff       (20)     9795 2023-04-13 19:53:56.000000 bcdata-0.7.8/bcdata/cli.py
+-rw-r--r--   0 snorris    (501) staff       (20)     6342 2022-09-29 00:22:24.000000 bcdata-0.7.8/bcdata/database.py
+-rw-r--r--   0 snorris    (501) staff       (20)     3034 2022-11-18 22:34:58.000000 bcdata-0.7.8/bcdata/wcs.py
+-rw-r--r--   0 snorris    (501) staff       (20)    11387 2023-04-13 19:53:56.000000 bcdata-0.7.8/bcdata/wfs.py
+drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-06-02 00:01:56.713909 bcdata-0.7.8/bcdata.egg-info/
+-rw-r--r--   0 snorris    (501) staff       (20)    16453 2023-06-02 00:01:56.000000 bcdata-0.7.8/bcdata.egg-info/PKG-INFO
+-rw-r--r--   0 snorris    (501) staff       (20)      474 2023-06-02 00:01:56.000000 bcdata-0.7.8/bcdata.egg-info/SOURCES.txt
+-rw-r--r--   0 snorris    (501) staff       (20)        1 2023-06-02 00:01:56.000000 bcdata-0.7.8/bcdata.egg-info/dependency_links.txt
+-rw-r--r--   0 snorris    (501) staff       (20)       42 2023-06-02 00:01:56.000000 bcdata-0.7.8/bcdata.egg-info/entry_points.txt
+-rw-r--r--   0 snorris    (501) staff       (20)        1 2019-11-08 06:25:25.000000 bcdata-0.7.8/bcdata.egg-info/not-zip-safe
+-rw-r--r--   0 snorris    (501) staff       (20)      121 2023-06-02 00:01:56.000000 bcdata-0.7.8/bcdata.egg-info/requires.txt
+-rw-r--r--   0 snorris    (501) staff       (20)        7 2023-06-02 00:01:56.000000 bcdata-0.7.8/bcdata.egg-info/top_level.txt
+-rw-r--r--   0 snorris    (501) staff       (20)      173 2022-07-16 00:28:03.000000 bcdata-0.7.8/pyproject.toml
+-rw-r--r--   0 snorris    (501) staff       (20)      102 2023-05-29 23:57:06.000000 bcdata-0.7.8/requirements.txt
+-rw-r--r--   0 snorris    (501) staff       (20)       38 2023-06-02 00:01:56.715048 bcdata-0.7.8/setup.cfg
+-rw-r--r--   0 snorris    (501) staff       (20)     1732 2022-07-20 16:54:44.000000 bcdata-0.7.8/setup.py
+drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-06-02 00:01:56.714644 bcdata-0.7.8/tests/
+-rw-r--r--   0 snorris    (501) staff       (20)     3851 2022-11-18 21:53:34.000000 bcdata-0.7.8/tests/test_bc2pg.py
+-rw-r--r--   0 snorris    (501) staff       (20)     6049 2023-04-13 19:53:56.000000 bcdata-0.7.8/tests/test_bcdata.py
+-rw-r--r--   0 snorris    (501) staff       (20)    11548 2022-07-20 16:54:44.000000 bcdata-0.7.8/tests/test_bcdc.py
+-rw-r--r--   0 snorris    (501) staff       (20)     2393 2022-07-20 16:54:44.000000 bcdata-0.7.8/tests/test_cli.py
```

### Comparing `bcdata-0.7.7/CHANGES.txt` & `bcdata-0.7.8/CHANGES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changes
 =======
 
+0.7.8 ()
+------------------
+- pin geopandas requirement to <v0.13 (#129)
+
 0.7.7 (2023-04-13)
 ------------------
 - add option to lowercasify properties keys / column names (#126)
 
 0.7.6 (2023-02-01)
 ------------------
 - better handling of connection errors (#118)
```

### Comparing `bcdata-0.7.7/LICENSE.txt` & `bcdata-0.7.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bcdata-0.7.7/PKG-INFO` & `bcdata-0.7.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcdata
-Version: 0.7.7
+Version: 0.7.8
 Summary: Python tools for quick access to DataBC geo-data available via WFS
 Home-page: https://github.com/smnorris/bcdata
 Author: Simon Norris
 Author-email: snorris@hillcrestgeo.ca
 License: Apache
 Keywords: gis geospatial data BC DataBC download "Britsh Columbia"
 Classifier: Development Status :: 3 - Alpha
@@ -32,26 +32,24 @@
 
 
 **Disclaimer**  
 *It is the user's responsibility to check the licensing for any downloads, data are generally licensed as [OGL-BC](http://www2.gov.bc.ca/gov/content/governments/about-the-bc-government/databc/open-data/open-government-license-bc)*
 
 ## Installation
 
-### pip
-
-    $ pip install bcdata
-
-### conda
-
 `bcdata` has several dependencies that may not easily be installed via `pip` (`gdal`, `fiona`, `geopandas`, `rasterio`)
 Installing via `miniconda`, the [conda package manager](https://conda.io/en/latest/miniconda.html) is recommended on Windows or if you do not wish to install these dependencies yourself.  Once `conda` is installed, download the provided `environment.yml` file to your system, open the `Anaconda Prompt` command line from the start menu, navigate to the folder where you saved `environment.yml` and create/actvate the environment.
 
     conda env create -f environment.yml
     conda activate bcdataenv
 
+Once requirements are installed, install with pip:
+
+    $ pip install bcdata
+
 
 ### Configuration
 
 #### Default PostgreSQL database
 
 The default target database connection (used by `bc2pg`) can be set via the `DATABASE_URL` environment variable (the password parameter should not be required if using a [.pgpass file](https://www.postgresql.org/docs/current/libpq-pgpass.html))
```

### Comparing `bcdata-0.7.7/README.md` & `bcdata-0.7.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,26 +10,24 @@
 
 
 **Disclaimer**  
 *It is the user's responsibility to check the licensing for any downloads, data are generally licensed as [OGL-BC](http://www2.gov.bc.ca/gov/content/governments/about-the-bc-government/databc/open-data/open-government-license-bc)*
 
 ## Installation
 
-### pip
-
-    $ pip install bcdata
-
-### conda
-
 `bcdata` has several dependencies that may not easily be installed via `pip` (`gdal`, `fiona`, `geopandas`, `rasterio`)
 Installing via `miniconda`, the [conda package manager](https://conda.io/en/latest/miniconda.html) is recommended on Windows or if you do not wish to install these dependencies yourself.  Once `conda` is installed, download the provided `environment.yml` file to your system, open the `Anaconda Prompt` command line from the start menu, navigate to the folder where you saved `environment.yml` and create/actvate the environment.
 
     conda env create -f environment.yml
     conda activate bcdataenv
 
+Once requirements are installed, install with pip:
+
+    $ pip install bcdata
+
 
 ### Configuration
 
 #### Default PostgreSQL database
 
 The default target database connection (used by `bc2pg`) can be set via the `DATABASE_URL` environment variable (the password parameter should not be required if using a [.pgpass file](https://www.postgresql.org/docs/current/libpq-pgpass.html))
```

### Comparing `bcdata-0.7.7/bcdata/bc2pg.py` & `bcdata-0.7.8/bcdata/bc2pg.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.7.7/bcdata/bcdc.py` & `bcdata-0.7.8/bcdata/bcdc.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.7.7/bcdata/cli.py` & `bcdata-0.7.8/bcdata/cli.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.7.7/bcdata/database.py` & `bcdata-0.7.8/bcdata/database.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.7.7/bcdata/wcs.py` & `bcdata-0.7.8/bcdata/wcs.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.7.7/bcdata/wfs.py` & `bcdata-0.7.8/bcdata/wfs.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.7.7/bcdata.egg-info/PKG-INFO` & `bcdata-0.7.8/bcdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcdata
-Version: 0.7.7
+Version: 0.7.8
 Summary: Python tools for quick access to DataBC geo-data available via WFS
 Home-page: https://github.com/smnorris/bcdata
 Author: Simon Norris
 Author-email: snorris@hillcrestgeo.ca
 License: Apache
 Keywords: gis geospatial data BC DataBC download "Britsh Columbia"
 Classifier: Development Status :: 3 - Alpha
@@ -32,26 +32,24 @@
 
 
 **Disclaimer**  
 *It is the user's responsibility to check the licensing for any downloads, data are generally licensed as [OGL-BC](http://www2.gov.bc.ca/gov/content/governments/about-the-bc-government/databc/open-data/open-government-license-bc)*
 
 ## Installation
 
-### pip
-
-    $ pip install bcdata
-
-### conda
-
 `bcdata` has several dependencies that may not easily be installed via `pip` (`gdal`, `fiona`, `geopandas`, `rasterio`)
 Installing via `miniconda`, the [conda package manager](https://conda.io/en/latest/miniconda.html) is recommended on Windows or if you do not wish to install these dependencies yourself.  Once `conda` is installed, download the provided `environment.yml` file to your system, open the `Anaconda Prompt` command line from the start menu, navigate to the folder where you saved `environment.yml` and create/actvate the environment.
 
     conda env create -f environment.yml
     conda activate bcdataenv
 
+Once requirements are installed, install with pip:
+
+    $ pip install bcdata
+
 
 ### Configuration
 
 #### Default PostgreSQL database
 
 The default target database connection (used by `bc2pg`) can be set via the `DATABASE_URL` environment variable (the password parameter should not be required if using a [.pgpass file](https://www.postgresql.org/docs/current/libpq-pgpass.html))
```

### Comparing `bcdata-0.7.7/setup.py` & `bcdata-0.7.8/setup.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.7.7/tests/test_bc2pg.py` & `bcdata-0.7.8/tests/test_bc2pg.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.7.7/tests/test_bcdata.py` & `bcdata-0.7.8/tests/test_bcdata.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.7.7/tests/test_bcdc.py` & `bcdata-0.7.8/tests/test_bcdc.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.7.7/tests/test_cli.py` & `bcdata-0.7.8/tests/test_cli.py`

 * *Files identical despite different names*

