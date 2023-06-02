# Comparing `tmp/exergenics-etl-1.0.6.tar.gz` & `tmp/exergenics-etl-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exergenics-etl-1.0.6.tar", last modified: Wed May 31 03:25:23 2023, max compression
+gzip compressed data, was "exergenics-etl-1.1.0.tar", last modified: Fri Jun  2 07:03:40 2023, max compression
```

## Comparing `exergenics-etl-1.0.6.tar` & `exergenics-etl-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:25:23.094276 exergenics-etl-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-31 03:25:18.000000 exergenics-etl-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-31 03:25:23.094276 exergenics-etl-1.0.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:25:23.090276 exergenics-etl-1.0.6/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:25:23.090276 exergenics-etl-1.0.6/app/exergenics_etl/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-31 03:25:18.000000 exergenics-etl-1.0.6/app/exergenics_etl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:25:23.094276 exergenics-etl-1.0.6/app/exergenics_etl/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 03:25:18.000000 exergenics-etl-1.0.6/app/exergenics_etl/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49892 2023-05-31 03:25:18.000000 exergenics-etl-1.0.6/app/exergenics_etl/src/exergenics_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-31 03:25:18.000000 exergenics-etl-1.0.6/app/exergenics_etl/src/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:25:23.094276 exergenics-etl-1.0.6/app/exergenics_etl/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 03:25:18.000000 exergenics-etl-1.0.6/app/exergenics_etl/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-31 03:25:18.000000 exergenics-etl-1.0.6/app/exergenics_etl/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    35886 2023-05-31 03:25:18.000000 exergenics-etl-1.0.6/app/exergenics_etl/test/test_exergenics_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-31 03:25:18.000000 exergenics-etl-1.0.6/app/exergenics_etl/test/test_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:25:23.094276 exergenics-etl-1.0.6/app/exergenics_etl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-31 03:25:23.000000 exergenics-etl-1.0.6/app/exergenics_etl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-31 03:25:23.000000 exergenics-etl-1.0.6/app/exergenics_etl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 03:25:23.000000 exergenics-etl-1.0.6/app/exergenics_etl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-31 03:25:23.000000 exergenics-etl-1.0.6/app/exergenics_etl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-31 03:25:23.000000 exergenics-etl-1.0.6/app/exergenics_etl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 03:25:23.094276 exergenics-etl-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-31 03:25:21.000000 exergenics-etl-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:03:40.080631 exergenics-etl-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-02 07:03:37.000000 exergenics-etl-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-02 07:03:40.080631 exergenics-etl-1.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:03:40.080631 exergenics-etl-1.1.0/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:03:40.080631 exergenics-etl-1.1.0/app/exergenics_etl/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-02 07:03:37.000000 exergenics-etl-1.1.0/app/exergenics_etl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:03:40.080631 exergenics-etl-1.1.0/app/exergenics_etl/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:03:37.000000 exergenics-etl-1.1.0/app/exergenics_etl/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50236 2023-06-02 07:03:37.000000 exergenics-etl-1.1.0/app/exergenics_etl/src/exergenics_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-02 07:03:37.000000 exergenics-etl-1.1.0/app/exergenics_etl/src/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:03:40.080631 exergenics-etl-1.1.0/app/exergenics_etl/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:03:37.000000 exergenics-etl-1.1.0/app/exergenics_etl/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-02 07:03:37.000000 exergenics-etl-1.1.0/app/exergenics_etl/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34199 2023-06-02 07:03:37.000000 exergenics-etl-1.1.0/app/exergenics_etl/test/test_exergenics_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-02 07:03:37.000000 exergenics-etl-1.1.0/app/exergenics_etl/test/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:03:40.080631 exergenics-etl-1.1.0/app/exergenics_etl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-02 07:03:40.000000 exergenics-etl-1.1.0/app/exergenics_etl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-02 07:03:40.000000 exergenics-etl-1.1.0/app/exergenics_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 07:03:40.000000 exergenics-etl-1.1.0/app/exergenics_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-02 07:03:40.000000 exergenics-etl-1.1.0/app/exergenics_etl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-02 07:03:40.000000 exergenics-etl-1.1.0/app/exergenics_etl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 07:03:40.080631 exergenics-etl-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-02 07:03:39.000000 exergenics-etl-1.1.0/setup.py
```

### Comparing `exergenics-etl-1.0.6/LICENSE` & `exergenics-etl-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.0.6/app/exergenics_etl/__init__.py` & `exergenics-etl-1.1.0/app/exergenics_etl/__init__.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.0.6/app/exergenics_etl/src/exergenics_etl.py` & `exergenics-etl-1.1.0/app/exergenics_etl/src/exergenics_etl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import os
 import zipfile
 import sqlalchemy
-from ..src.logger import ETLLogger as Logger
+try:
+    from ..src.logger import ETLLogger as Logger
+except:
+    from logger import ETLLogger as Logger
 import pandas as pd
 from pytz import timezone
 from datetime import datetime
-from typing import Union, Dict
+from typing import Union, Dict, Callable
 from exergenics import exergenics
 from urllib.parse import quote_plus
 from sqlalchemy import create_engine
 from Levenshtein import distance as levenshtein_distance
 import regex as re
 import dateparser
 from collections import Counter
@@ -28,14 +31,16 @@
 TIMESTAMP_HEADER_DISTANCE = 4
 LOG_HEADER = ['timepretty', 'observation', 'datapoint']
 TIME, NAME, VALUE = LOG_HEADER
 N_COLUMN_LONG_DATA = 3  # The number of columns in a long-format data table
 DEFAULT_POSITION_DAY = 0  # The default position of the day of month in timestamps
 SUMMARY_COLUMNS = ['count', 'mean', 'std',
                    'min', '25%', '50%', '75%', 'max']
+EMPTY_COLUMN_NAME_PREFIX = "Unnamed"  # Prefix of auto generated column name when column name is not found
+
 
 
 logger = Logger(loggerName='Exergenics-ETL',
                 component='python_package', subComponent='exergenics_etl')
 
 
 class EtlError(Exception):
@@ -336,36 +341,37 @@
         Args:
             nRowsVerify (int, optional): Numbers of rows to verify in each CSV. Defaults to 10.
         """
         self.logger = Logger()
         self.skiprows = None
         self.nRowsVerify = nRowsVerify
 
-    def validate_headers(self, df0: pd.DataFrame):
+    def validate_headers(self, headers: pd.Series):
         """This function validates the value of skiprows by checking the types of header.
-        A header should be a non-nan string only, ideally with a length greater than 5,
+        A header should not be a column header that is automatically generated by Pandas.
+        It should be a non-nan string only, ideally with a length greater than 5,
         and not a string of numbers.
 
         Args:
             df0 (pd.DataFrame): Pandas DataFrame for header validation.
 
         Raises:
             EtlError: If invalid column headers are found.
         """
 
-        # Drop rows with NA in timestamps (the 1st column)
-        df = df0[~pd.isna(df0[df0.columns[0]])]
-
-        # Get all headers
-        headers = df.iloc[0]
-
         # Validate each header
         for v in headers:
 
             try:
+                assert not v.startswith(EMPTY_COLUMN_NAME_PREFIX)
+            except AssertionError as e:
+                self.logger.error(e)
+                raise EtlError(e)
+
+            try:
                 # Check header is a string but not a string of numbers
                 pd.to_numeric(v)
 
                 # Raise and log error
                 errorMessage = f"Test Failed: Can do to_numeric on header: {v} of type {type(v)}; \
                     the header can't be numbers, a string of numbers, an empty string, None, np.nan or boolean."
                 self.logger.error(errorMessage)
@@ -377,124 +383,119 @@
 
             try:
                 assert len(v) > 5, f'Expected the length of header to be ideally greater than 5 \
                     but the actual length of header "{v}" was {len(v)}'
             except AssertionError as e:
                 self.logger.warn(e)
 
-        self.logger.info(f'1st verification passed ...')
-
         return
+    
+    def _auto_skiprows(self, fileName: str, zf: zipfile.ZipFile, readFileFunc: Callable) -> Tuple[pd.DataFrame, int, int]:
 
-    def _auto_skiprows_csv(self, fileName: str, zf: zipfile.ZipFile) -> Tuple[pd.DataFrame, int, int]:
         """
-        Reads a CSV file from a zip file object and 
-        returns a Pandas dataframe, header row index, 
-        and number of rows to skip from the beginning of the file.
+        Automatically determines the number of rows to skip in a CSV or XLSX file to locate the header row.
 
         Args:
-            filepath (str): Absolute path of the CSV file to apply skip rows.
-            zf (zipfile.ZipFile): Zipped folder where the file is.
+            fileName (str): The name of the file within the zip file to be read.
+            zf (zipfile.ZipFile): The ZipFile object containing the file.
+            readFileFunc (Callable): A function to read the file.
 
         Returns:
-            tuple (pd.DataFrame, int, int): Return a dataframe of the input 
-            filepath with rows skipped and header row ID if verification passed and None otherwise.
+            Tuple[pd.DataFrame, int, int]: A tuple containing the pandas DataFrame (`df`), the number of rows to skip (`skiprows`),
+            and the row ID of the header (`headerRowID`).
+
+        Raises:
+            EtlError: If reading file failed after trying from 1 to 10 as the skiprows value.
+
         """
 
         # Try reading the file with different numbers of rows to skip
         skiprowsTrials = range(10)
 
         for skiprowsTrial in skiprowsTrials:
             try:
                 # Try reading the CSV file with the current number of rows to skip
-                df = pd.read_csv(zf.open(fileName),
-                                 skiprows=skiprowsTrial, header=None)
+                df = readFileFunc(zf.open(fileName),
+                                 skiprows=skiprowsTrial, header=None, nrows=skiprowsTrial+12)
                 skiprows = skiprowsTrial
-                headerRowID = 0
+
+                # Find the row ID of header and compute the number of rows to skip
+                col1 = df[df.columns[1]]
+                headerRowID = col1.dropna().index[0]  # The row number of the first non-na value
+                skiprows = skiprowsTrial + headerRowID
 
                 self.logger.info(
                     f'Found skiprows value = {skiprowsTrial}')
+
                 return df, skiprows, headerRowID
 
             except:
                 continue
 
         errorMessage = f"Table in the data file should start at the first 10 rows."
         self.logger.error(errorMessage)
         raise EtlError(errorMessage)
 
-    def _auto_skiprows_excel(self, fileName: str, zf: zipfile.ZipFile) -> Tuple[pd.DataFrame, int, int]:
-        """Skip rows before headers for DataFrame read from an Excel sheet.
-        Assume redundant stuffs in excel sheets are in the first column above timestamps.
-        That is, the header of a data point is the first non-NA string in that column.
-        Verify after skipping rows.
-
-        Args:
-            filepath (str): Absolute path of the Excel file to apply skip rows.
-            zf (zipfile.ZipFile): Zipped folder where the file is.
-
-        Returns:
-            tuple (pd.DataFrame, int): Return a dataframe of the input 
-            filepath with rows skipped and header row ID if verification passed and None otherwise.
-        """
-        df = pd.read_excel(zf.open(fileName), index_col=False, header=None)
-
-        # Find the row ID of header and compute the number of rows to skip
-        col1 = df[df.columns[1]]
-        headerRowID = col1.dropna().index[0]
-        skiprows = headerRowID
-
-        # Skip rows
-        df.drop(labels=range(skiprows), inplace=True)
-
-        self.logger.info(f'Found skiprows = {skiprows}')
-
-        return df, skiprows, headerRowID
-
     def read(self, fileName: str, zf: zipfile.ZipFile = None) -> pd.DataFrame:
-        """Reads a data file from a zipped folder while skipping non-data rows on top of the file.
+        """Read a data file from a zipped folder while skipping non-data rows on top of the file.
+        If a skiprows value exists, try reading the file with the existing skiprows value.
+        If it failed, find the skiprows value again and read the file.
 
         Args:
             fileName (str): File name of the file to apply skip rows.
             zf (zipfile.ZipFile): Zipped folder where the file is.
 
         Returns:
             pd.DataFrame: Pandas DataFrame of the input CSV file with skipped rows.  
         """
 
         try:
             # Get the filename extension of the current data file
             extension = [
                 extension for extension in EXTENSIONS if fileName.endswith(extension)][0]
-
+            
+            # Get the pandas method for openning data file
+            if extension == 'csv':
+                readFileFunc = pd.read_csv
+            elif extension == 'xlsx':
+                readFileFunc = pd.read_excel
+            
             if self.skiprows is None:
-                # Find skiprows value to read the data file
-                if extension == 'xlsx':
-                    df, self.skiprows, headerRowId = self._auto_skiprows_excel(fileName, zf)
-                elif extension == 'csv':
-                    df, self.skiprows, headerRowId = self._auto_skiprows_csv(fileName, zf)
-
-            else:
-                # Read the data file with the last skiprows value
-                if extension == 'csv':
-                    df = pd.read_csv(zf.open(fileName), skiprows=self.skiprows, header=None)
-                elif extension == 'xlsx':
-                    df = pd.read_excel(zf.open(fileName), skiprows=self.skiprows, header=None)
                 
-                headerRowId = 0
+                # Find skiprows value
+                df, self.skiprows, headerRowID = self._auto_skiprows(fileName, zf, readFileFunc)
 
-            # Validate that headers are strings
-            self.validate_headers(df)
+                # Validate header after skipping text rows
+                self.validate_headers(df.iloc[headerRowID])
 
-            # Set header as column names
-            df.columns = df.loc[headerRowId].values
+                # Finally, open data file with skiprows value and headers as dataframe columns
+                df = readFileFunc(zf.open(fileName),
+                                        skiprows=self.skiprows)
 
-            # Remove headers from values
-            df.drop(labels=headerRowId, inplace=True)
-            df.reset_index(inplace=True, drop=True)  # Replace and reset index
+            else:
+                try:
+                    # Try reading data file with the previously found skiprows value
+                    df = readFileFunc(zf.open(fileName),
+                                        skiprows=self.skiprows)
+                    self.validate_headers(df.columns)
+                    
+                except:
+                    msg = f'The current file ({fileName}) probably has a different skiprows value. Rerun auto skiprows.'
+                    self.logger.warn(msg)
+
+                    # If failed, reset and find skiprows value again
+                    self.skiprows = None
+                    df, self.skiprows, headerRowID = self._auto_skiprows(fileName, zf, readFileFunc)
+
+                    # Validate that headers are strings
+                    self.validate_headers(df.iloc[headerRowID])
+
+                    # Finally, open data file with skiprows value and headers as dataframe columns
+                    df = readFileFunc(zf.open(fileName),
+                                            skiprows=self.skiprows)
         
         except Exception as e:
             self.logger.error(e)
             raise EtlError('Error in opening data file.')
 
         return df
```

### Comparing `exergenics-etl-1.0.6/app/exergenics_etl/src/logger.py` & `exergenics-etl-1.1.0/app/exergenics_etl/src/logger.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.0.6/app/exergenics_etl/test/conftest.py` & `exergenics-etl-1.1.0/app/exergenics_etl/test/conftest.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.0.6/app/exergenics_etl/test/test_exergenics_etl.py` & `exergenics-etl-1.1.0/app/exergenics_etl/test/test_exergenics_etl.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,48 +2,32 @@
 import os
 import sys
 import pandas as pd
 from pandas import Timestamp
 import numpy as np
 import shutil
 import zipfile
-from ..src.logger import ETLLogger as Logger
 from dotenv import load_dotenv
 
-from ..src.exergenics_etl import (
-    EtlError,
-    create_api,
-    create_sql_engine,
-    get_time_now,
-    create_tmp_folder,
-    generate_CSV_name,
-    strftime_for_NaT,
-    generate_one_manifest_row,
-    generate_output_file_path,
-    get_file_name_list,
-    SkipRowsMachine,
-    convertable_to_float,
-    InputValidation,
-    calculate_time_interval,
-    DatetimeParser,
-    DEFAULT_POSITION_DAY,
-    transform_columns_to_long_dataframes,
-    get_point_summary,
-    get_statistical_summary,
-    merge_long_dataframes,
-    merge_wide_dataframes,
-    save_file_to_portal
-)
-
+try:
+    from ..src.logger import ETLLogger as Logger
+    from ..src.exergenics_etl import *
+except:
+    path = os.getcwd()
+    sys.path.insert(0, path)
+    from app.exergenics_etl.src.logger import ETLLogger as Logger
+    from app.exergenics_etl.src.exergenics_etl import *
 
 load_dotenv()
 
 logger = Logger(loggerName='UnitTest',
                 component='data_modules', subComponent='pre_merged')
 
+TEST_DATA_DIR = "app/exergenics_etl/test/testData"
+
 
 class TestCreateApiClass:
 
     @pytest.fixture(scope='class', params=['staging', 'production'])
     def my_valid_environment(self, request):
         return request.param
 
@@ -213,61 +197,35 @@
         fileNames = get_file_name_list(my_manual_zipfile)
         assert len(fileNames) == 4
 
 
 class TestSkipRowsMachineClass:
 
     @pytest.fixture(scope='class')
-    def my_expected_first_row(self):
-        """The first row of the expected output form skipRowsMachine.read."""
-        return pd.Series(['Timestamp', 'Test data point'])
+    def my_expected_columns(self):
+        """The expected column headers of the dataframe returned form skipRowsMachine.read."""
+        return pd.Series(['Timestamp', 'Test value column'])
     
     @pytest.fixture(scope='function')
     def my_skipRowsMachine(self):
         skipRowsMachine = SkipRowsMachine()
         return skipRowsMachine
-
-    def test_skiprows1(self, my_expected_first_row, my_skipRowsMachine):
-        """Test for finding skiprows value with _auto_skiprows_csv and applying the value on a XLSX sheet."""
-        myTestFileNames = ["skiprows_test/skiprows.csv", "skiprows_test/skiprows.xlsx"]
-        myTestZipfilePath = "app/exergenics_etl/test/testData/skiprows_test.zip"
-        myTestZippedFile = zipfile.ZipFile(myTestZipfilePath)
-
-        for fileName in myTestFileNames:
-            df = my_skipRowsMachine.read(fileName, myTestZippedFile)
-            assert all(df.columns.values == my_expected_first_row)
-
-    def test_skiprows2(self, my_expected_first_row, my_skipRowsMachine):
-        """Test for finding skiprows value with _auto_skiprows_excel and applying the value on a CSV."""
-        myTestFileNames = ["skiprows_test/skiprows.xlsx", "skiprows_test/skiprows.csv"]
-        myTestZipfilePath = "app/exergenics_etl/test/testData/skiprows_test.zip"
-        myTestZippedFile = zipfile.ZipFile(myTestZipfilePath)
-
-        for fileName in myTestFileNames:
-            df = my_skipRowsMachine.read(fileName, myTestZippedFile)
-            assert all(df.columns.values == my_expected_first_row)
-    
-    def test_skiprows3(self, my_expected_first_row, my_skipRowsMachine):
-        """Test for finding skiprows value with _auto_skiprows_csv and applying the value on a XLSX sheet."""
-        myTestFileNames = ["skiprows_test2/skiprows.xlsx", "skiprows_test2/skiprows.csv"]
-        myTestZipfilePath = "app/exergenics_etl/test/testData/skiprows_test2.zip"
-        myTestZippedFile = zipfile.ZipFile(myTestZipfilePath)
-
-        for fileName in myTestFileNames:
-            df = my_skipRowsMachine.read(fileName, myTestZippedFile)
-            assert all(df.columns.values == my_expected_first_row)
-
-    def test_skiprows4(self, my_expected_first_row, my_skipRowsMachine):
-        myTestFileNames = ["skiprows_test2/skiprows.csv", "skiprows_test2/skiprows.xlsx"]
-        myTestZipfilePath = "app/exergenics_etl/test/testData/skiprows_test2.zip"
+        
+    def test_skiprows(self, my_expected_columns, my_skipRowsMachine):
+        """Test auto skiprows on files with mixed skiprows values and format."""
+        myTestFileNames = ['test_skipRows/oneSkipRows_noComma.csv', 'test_skipRows/oneSkipRows.csv', 
+                           'test_skipRows/twoSkipRows.csv', 'test_skipRows/twoSkipRows_noComma.csv', 
+                           'test_skipRows/zeroSkipRows.csv', 'test_skipRows/oneSkipRows.xlsx', 
+                           'test_skipRows/twoSkipRows.xlsx', 'test_skipRows/zeroSkipRows.xlsx']
+        myTestZipfilePath = f"{TEST_DATA_DIR}/test_skipRows.zip"
         myTestZippedFile = zipfile.ZipFile(myTestZipfilePath)
 
         for fileName in myTestFileNames:
             df = my_skipRowsMachine.read(fileName, myTestZippedFile)
-            assert all(df.columns.values == my_expected_first_row)
+            assert all(df.columns.values == my_expected_columns)
 
 
 class TestConvertableToFloatClass:
 
     @pytest.mark.parametrize("string, expected", [
     ("3.14", True),  # Valid float string
     ("0", True),     # Valid float string
```

### Comparing `exergenics-etl-1.0.6/app/exergenics_etl.egg-info/SOURCES.txt` & `exergenics-etl-1.1.0/app/exergenics_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.0.6/setup.py` & `exergenics-etl-1.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 # with open("app/Readme.md", "r") as f:
 #     long_description = f.read()
 
 setup(
     name="exergenics-etl",
-    version="v1.0.6",
+    version="v1.1.0",
     description="Exergenics shared Data ETL functions",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description="### Exergenics ETL Pytho package",
     long_description_content_type="text/markdown",
     url="",
     author="Nobel Wong",
```

