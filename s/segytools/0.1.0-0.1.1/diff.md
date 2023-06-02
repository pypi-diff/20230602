# Comparing `tmp/segytools-0.1.0.tar.gz` & `tmp/segytools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segytools-0.1.0.tar", max compression
+gzip compressed data, was "segytools-0.1.1.tar", max compression
```

## Comparing `segytools-0.1.0.tar` & `segytools-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1055 2022-06-22 10:42:33.628006 segytools-0.1.0/LICENSE
--rw-r--r--   0        0        0      957 2023-01-15 17:30:25.519354 segytools-0.1.0/README.md
--rw-r--r--   0        0        0      731 2023-01-15 18:04:32.342661 segytools-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      290 2023-01-15 17:36:44.622683 segytools-0.1.0/src/segytools/__init__.py
--rw-r--r--   0        0        0     1115 2023-01-13 13:32:30.422936 segytools-0.1.0/src/segytools/datatypes.py
--rw-r--r--   0        0        0     7373 2023-01-14 17:54:45.936139 segytools-0.1.0/src/segytools/segy_abstract_header.py
--rw-r--r--   0        0        0    11496 2023-01-14 14:39:42.446165 segytools-0.1.0/src/segytools/segy_file_header.py
--rw-r--r--   0        0        0     8075 2023-01-14 14:52:19.189497 segytools-0.1.0/src/segytools/segy_header_item.py
--rw-r--r--   0        0        0    32346 2023-01-14 12:47:16.106089 segytools-0.1.0/src/segytools/segy_trace_header.py
--rw-r--r--   0        0        0     2857 2023-01-14 13:16:58.562732 segytools-0.1.0/src/segytools/toolkit.py
--rw-r--r--   0        0        0      200 2023-01-10 09:00:46.712856 segytools-0.1.0/src/segytools/utils.py
--rw-r--r--   0        0        0     1696 1970-01-01 00:00:00.000000 segytools-0.1.0/setup.py
--rw-r--r--   0        0        0     1573 1970-01-01 00:00:00.000000 segytools-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1055 2022-06-22 10:42:33.628006 segytools-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1020 2023-02-02 11:46:01.496827 segytools-0.1.1/README.md
+-rw-r--r--   0        0        0      786 2023-06-02 08:15:34.847622 segytools-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      215 2023-02-04 10:18:01.553258 segytools-0.1.1/src/segytools/__init__.py
+-rw-r--r--   0        0        0     1165 2023-01-29 16:40:13.789248 segytools-0.1.1/src/segytools/datatypes.py
+-rw-r--r--   0        0        0     4192 2023-06-02 08:15:34.847622 segytools-0.1.1/src/segytools/segy_abstract_header.py
+-rw-r--r--   0        0        0    13599 2023-06-02 08:15:34.847622 segytools-0.1.1/src/segytools/segy_file_header.py
+-rw-r--r--   0        0        0     8542 2023-06-02 08:15:34.847622 segytools-0.1.1/src/segytools/segy_header_item.py
+-rw-r--r--   0        0        0    35111 2023-06-02 08:15:34.847622 segytools-0.1.1/src/segytools/segy_trace_header.py
+-rw-r--r--   0        0        0      497 2023-01-29 16:40:13.789248 segytools-0.1.1/src/segytools/toolkit.py
+-rw-r--r--   0        0        0       95 2023-01-29 16:40:13.789248 segytools-0.1.1/src/segytools/utils.py
+-rw-r--r--   0        0        0     1636 1970-01-01 00:00:00.000000 segytools-0.1.1/PKG-INFO
```

### Comparing `segytools-0.1.0/LICENSE` & `segytools-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `segytools-0.1.0/README.md` & `segytools-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
 # segytools
 
+[Documentation](https://anthonytorlucci.github.io/segytools/)
+
 `segytools` is a simple python library that provides low level tools for analyzing and parsing segy formatted files. There is no `read_segy()` function per se because that assumes the data is properly formatted in which case there are other tools much better suited, e.g. [segyio](https://github.com/equinor/segyio). The tools here are designed to aid in the analysis of "non-standard" segy files and converting those files to a more standard form easily read by other third party software.
 
 Currently only segy revision 2 file header and trace header formats are provided. However, custom header containers can be created by inheriting `SegyAbstractHeader`.
 
 Originally, much of the work had been derived from another open-source segy package [segpy](https://github.com/sixty-north/segpy), but version `0.1.0` has been almost completely rewritten. IBM float conversion is done with [enthought/ibm2ieee](https://github.com/enthought/ibm2ieee).
```

### Comparing `segytools-0.1.0/pyproject.toml` & `segytools-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "segytools"
-version = "0.1.0"
+version = "0.1.1"
 description = "low level toolkit for manipulating and analyzing segy formatted data"
 authors = ["anthonytorlucci <anthonytorlucci@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -19,11 +19,14 @@
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 jupyter = "^1.0.0"
 myst-nb = {version = "^0.17.1", python = "^3.9"}
 sphinx-autoapi = "^2.0.0"
 sphinx-rtd-theme = "^1.1.1"
+flake8 = "^6.0.0"
+black = "^22.12.0"
+isort = "^5.12.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `segytools-0.1.0/src/segytools/datatypes.py` & `segytools-0.1.1/src/segytools/datatypes.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 """Mappings between the coding systems used for sample types.
 """
 
 # A mapping from data sample format codes to SEG Y types.
 from collections import namedtuple
 
-DataSampleFormat = namedtuple('DataSampleFormat', ['format', 'ctype', 'size_in_bytes'])
+DataSampleFormat = namedtuple(
+    'DataSampleFormat', ['format', 'ctype', 'size_in_bytes'])
 
 # https://docs.python.org/3/library/struct.html
-DATA_SAMPLE_FORMAT_INT8 = DataSampleFormat(format='b', ctype='char', size_in_bytes=1)
-DATA_SAMPLE_FORMAT_UINT8 = DataSampleFormat(format='B', ctype='unsigned char', size_in_bytes=1)
-DATA_SAMPLE_FORMAT_INT16 = DataSampleFormat(format='h', ctype='short', size_in_bytes=2)
-DATA_SAMPLE_FORMAT_UINT16 = DataSampleFormat(format='H', ctype='unsigned short', size_in_bytes=2)
-DATA_SAMPLE_FORMAT_INT32 = DataSampleFormat(format='i', ctype='int', size_in_bytes=4)
-DATA_SAMPLE_FORMAT_UINT32 = DataSampleFormat(format='I', ctype='unsigned int', size_in_bytes=4)
-DATA_SAMPLE_FORMAT_FLOAT32 = DataSampleFormat(format='f', ctype='float', size_in_bytes=4)
-DATA_SAMPLE_FORMAT_FLOAT64 = DataSampleFormat(format='d', ctype='double', size_in_bytes=8)
-DATA_SAMPLE_FORMAT_IBM = DataSampleFormat(format='ibm', ctype='ibm', size_in_bytes=4)
+DATA_SAMPLE_FORMAT_INT8 = DataSampleFormat(
+    format='b', ctype='char', size_in_bytes=1)
+DATA_SAMPLE_FORMAT_UINT8 = DataSampleFormat(
+    format='B', ctype='unsigned char', size_in_bytes=1)
+DATA_SAMPLE_FORMAT_INT16 = DataSampleFormat(
+    format='h', ctype='short', size_in_bytes=2)
+DATA_SAMPLE_FORMAT_UINT16 = DataSampleFormat(
+    format='H', ctype='unsigned short', size_in_bytes=2)
+DATA_SAMPLE_FORMAT_INT32 = DataSampleFormat(
+    format='i', ctype='int', size_in_bytes=4)
+DATA_SAMPLE_FORMAT_UINT32 = DataSampleFormat(
+    format='I', ctype='unsigned int', size_in_bytes=4)
+DATA_SAMPLE_FORMAT_FLOAT32 = DataSampleFormat(
+    format='f', ctype='float', size_in_bytes=4)
+DATA_SAMPLE_FORMAT_FLOAT64 = DataSampleFormat(
+    format='d', ctype='double', size_in_bytes=8)
+DATA_SAMPLE_FORMAT_IBM = DataSampleFormat(
+    format='ibm', ctype='ibm', size_in_bytes=4)
```

### Comparing `segytools-0.1.0/src/segytools/segy_file_header.py` & `segytools-0.1.1/src/segytools/segy_file_header.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,121 +1,119 @@
 '''
 segy file header aka binary header
 '''
 
 # import python standard modules
 
-
 # import 3rd party libraries
 
-
 # import local python
-from segytools.datatypes import DataSampleFormat, \
-    DATA_SAMPLE_FORMAT_INT16, DATA_SAMPLE_FORMAT_INT32
-from segytools.segy_header_item import SegyHeaderItem
+from segytools.datatypes import (DATA_SAMPLE_FORMAT_INT16,
+                                 DATA_SAMPLE_FORMAT_INT32)
 from segytools.segy_abstract_header import SegyAbstractHeader
-
+from segytools.segy_header_item import SegyHeaderItem
 
 # --- Mappings
 # bytes 25-26
 DATA_SAMPLE_FORMAT_CODE = {
-    0: 'undefined',
-    1: 'ibm',
-    2: 'int32',
-    3: 'int16',
-    5: 'float32',
-    8: 'int8'
+    0: "undefined",
+    1: "ibm",
+    2: "int32",
+    3: "int16",
+    5: "float32",
+    8: "int8",
 }
 
 # bytes 29-30
 TRACE_SORTING_CODE = {
-    -1: 'Other',
-    0: 'Unknown',
-    1: 'As Recorded (no sorting)',
-    2: 'CDP Ensemble',
-    3: 'Single fold continuous profile',
-    4: 'Horizontally stacked',
-    5: 'Common source point',
-    6: 'Common receiver point',
-    7: 'Common offset point',
-    8: 'Common mid-point',
-    9: 'Common Conversion point'
+    -1: "Other",
+    0: "Unknown",
+    1: "As Recorded (no sorting)",
+    2: "CDP Ensemble",
+    3: "Single fold continuous profile",
+    4: "Horizontally stacked",
+    5: "Common source point",
+    6: "Common receiver point",
+    7: "Common offset point",
+    8: "Common mid-point",
+    9: "Common Conversion point",
 }
 
 # bytes 39-40
 SWEEP_TYPE_CODE = {
-    0: 'undefined',
-    1: 'linear',
-    2: 'parabolic',
-    3: 'exponential',
-    4: 'other'
+    0: "undefined",
+    1: "linear",
+    2: "parabolic",
+    3: "exponential",
+    4: "other",
 }
 
 # bytes 47-48
 TAPER_TYPE = {
-    0: 'undefined',
-    1: 'linear',
-    2: 'cos**2',
-    3: 'other'
+    0: "undefined",
+    1: "linear",
+    2: "cos**2",
+    3: "other",
 }
 
 # bytes 49-50
 CORRELATED_DATA_TRACES = {
-    0: 'undefined',
-    1: 'no',
-    2: 'yes'
+    0: "undefined",
+    1: "no",
+    2: "yes",
 }
 
 # bytes 51-52
 BINARY_GAIN_RECOVERED = {
-    0: 'undefined',
-    1: 'yes',
-    2: 'no'
+    0: "undefined",
+    1: "yes",
+    2: "no",
 }
 
 # bytes 53-54
 AMPLITUDE_RECOVERY_METHOD = {
-    0: 'undefined',
-    1: 'none',
-    2: 'spherical divergence',
-    3: 'agc',
-    4: 'other'
+    0: "undefined",
+    1: "none",
+    2: "spherical divergence",
+    3: "agc",
+    4: "other",
 }
 
 # bytes 55-56
 MEASUREMENT_SYSTEM = {
-    0: 'undefined',
-    1: 'meters',
-    2: 'feet'
+    0: "undefined",
+    1: "meters",
+    2: "feet",
 }
 
 # bytes 57-58
 IMPULSE_SIGNAL_POLARITY = {
-    0: 'undefined',
-    1: 'incerase in pressure or upward geophone case movement gives negative number on tape',
-    2: 'incerase in pressure or upward geophone case movement gives positive number on tape'
+    0: "undefined",
+    1: "incerase in pressure or upward geophone case movement gives negative \
+        number on tape",
+    2: "incerase in pressure or upward geophone case movement gives positive \
+        number on tape",
 }
 
 # bytes 59-60
 VIBRATORY_POLARITY_CODE = {
-    0: 'undefined',
-    1: '337.5 (deg) to 22.5 (deg)',
-    2: '22.5 (deg) to 67.5 (deg)',
-    3: '67.5 (deg) to 112.5 (deg)',
-    4: '112.5 (deg) to 157.5 (deg)',
-    5: '157.5 (deg) to 202.5 (deg)',
-    6: '202.5 (deg) to 247.5 (deg)',
-    7: '247.5 (deg) to 292.5 (deg)',
-    8: '292.5 (deg) to 337.5 (deg)'
+    0: "undefined",
+    1: "337.5 (deg) to 22.5 (deg)",
+    2: "22.5 (deg) to 67.5 (deg)",
+    3: "67.5 (deg) to 112.5 (deg)",
+    4: "112.5 (deg) to 157.5 (deg)",
+    5: "157.5 (deg) to 202.5 (deg)",
+    6: "202.5 (deg) to 247.5 (deg)",
+    7: "247.5 (deg) to 292.5 (deg)",
+    8: "292.5 (deg) to 337.5 (deg)",
 }
 
 
 class SegyFileHeaderRev2(SegyAbstractHeader):
-    """
-    File or binary header definition of a segy file.
+    """File or binary header definition of a segy file.
 
     Parameters
     ----------
     jobid : SegyHeaderItem
         job identification number
     line_number : SegyHeaderItem
         line number
@@ -173,174 +171,243 @@
         seg y format revision number
     fixed_length : SegyHeaderItem
         fixed length trace flag
     num_txt_headers : SegyHeaderItem
         number of 3200 byte ext file header records following
     """
 
-    def __init__(self):
+    def __init__(self, segy_logger=None):
         super().__init__()
-        self.byte_length = 400
+        self.byte_length = 400  # segy standard byte length
+        self.segy_logger = segy_logger  # used for writing information to terminal or file; see https://docs.python.org/3.10/library/logging.html
         self.jobid = SegyHeaderItem(
-            sample_format=DATA_SAMPLE_FORMAT_INT32, 
+            sample_format=DATA_SAMPLE_FORMAT_INT32,
             start_byte=1,
-            description='job identification number')
+            description="job identification number",
+            segy_logger=self.segy_logger,
+        )
         self.line_number = SegyHeaderItem(
-            sample_format=DATA_SAMPLE_FORMAT_INT32, 
+            sample_format=DATA_SAMPLE_FORMAT_INT32,
             start_byte=5,
-            description='line number')
+            description="line number",
+            segy_logger=self.segy_logger,
+        )
         self.reel_number = SegyHeaderItem(
-            sample_format=DATA_SAMPLE_FORMAT_INT32, 
+            sample_format=DATA_SAMPLE_FORMAT_INT32,
             start_byte=9,
-            description='reel number')
+            description="reel number",
+            segy_logger=self.segy_logger,
+        )
         self.num_traces_per_ensemble = SegyHeaderItem(
-            sample_format=DATA_SAMPLE_FORMAT_INT16, 
+            sample_format=DATA_SAMPLE_FORMAT_INT16,
             start_byte=13,
-            description='number of data traces per ensemble')
+            description="number of data traces per ensemble",
+            segy_logger=self.segy_logger,
+        )
         self.num_aux_traces_per_ensemble = SegyHeaderItem(
-            sample_format=DATA_SAMPLE_FORMAT_INT16, 
+            sample_format=DATA_SAMPLE_FORMAT_INT16,
             start_byte=15,
-            description='number of auxiliary traces per ensemble')
+            description="number of auxiliary traces per ensemble",
+            segy_logger=self.segy_logger,
+        )
         self.sample_interval = SegyHeaderItem(
-            sample_format=DATA_SAMPLE_FORMAT_INT16, 
+            sample_format=DATA_SAMPLE_FORMAT_INT16,
             start_byte=17,
-            description='sample interval in microseconds')
+            description="sample interval in microseconds",
+            segy_logger=self.segy_logger,
+        )
         self.original_sample_interval = SegyHeaderItem(
-            sample_format=DATA_SAMPLE_FORMAT_INT16, 
+            sample_format=DATA_SAMPLE_FORMAT_INT16,
             start_byte=19,
-            description='sample interval in microseconds or original recording')
+            description="sample interval in microseconds or original recording",
+            segy_logger=self.segy_logger,
+        )
         self.num_samples_per_trace = SegyHeaderItem(
-            sample_format=DATA_SAMPLE_FORMAT_INT16, 
+            sample_format=DATA_SAMPLE_FORMAT_INT16,
             start_byte=21,
-            description='number of samples per data trace')
+            description="number of samples per data trace",
+            segy_logger=self.segy_logger,
+        )
         self.original_num_samples_per_trace = SegyHeaderItem(
-            sample_format=DATA_SAMPLE_FORMAT_INT16, 
+            sample_format=DATA_SAMPLE_FORMAT_INT16,
             start_byte=23,
-            description='number of samples per data trace or original recording')
+            description="number of samples per data trace or original recording",
+            segy_logger=self.segy_logger,
+        )
         self.data_sample_format_code = SegyHeaderItem(
-            sample_format=DATA_SAMPLE_FORMAT_INT16, 
+            sample_format=DATA_SAMPLE_FORMAT_INT16,
             start_byte=25,
-            description='data sample format code',
-            map_dict=DATA_SAMPLE_FORMAT_CODE)
+            description="data sample format code",
+            map_dict=DATA_SAMPLE_FORMAT_CODE,
+            segy_logger=self.segy_logger,
+        )
         self.fold = SegyHeaderItem(
-            sample_format=DATA_SAMPLE_FORMAT_INT16, 
+            sample_format=DATA_SAMPLE_FORMAT_INT16,
             start_byte=27,
-            description='ensemble fold')
+            description="ensemble fold",
+            segy_logger=self.segy_logger,
+        )
         self.sort_code = SegyHeaderItem(
-            sample_format=DATA_SAMPLE_FORMAT_INT16, 
+            sample_format=DATA_SAMPLE_FORMAT_INT16,
             start_byte=29,
-            description='trace sorting code',
-            map_dict=TRACE_SORTING_CODE)
+            description="trace sorting code",
+            map_dict=TRACE_SORTING_CODE,
+            segy_logger=self.segy_logger,
+        )
         self.vertical_sum_code = SegyHeaderItem(
-            sample_format=DATA_SAMPLE_FORMAT_INT16, 
+            sample_format=DATA_SAMPLE_FORMAT_INT16,
             start_byte=31,
-            description='vertical sum code')
+            description="vertical sum code",
+            segy_logger=self.segy_logger,
+        )
         self.sweep_freq_start = SegyHeaderItem(
-            sample_format=DATA_SAMPLE_FORMAT_INT16, 
+            sample_format=DATA_SAMPLE_FORMAT_INT16,
             start_byte=33,
-            description='sweep frequency at start')
+            description="sweep frequency at start",
+            segy_logger=self.segy_logger,
+        )
         self.sweep_freq_end = SegyHeaderItem(
-            sample_format=DATA_SAMPLE_FORMAT_INT16, 
+            sample_format=DATA_SAMPLE_FORMAT_INT16,
             start_byte=35,
-            description='sweep frequency at end')
+            description="sweep frequency at end",
+            segy_logger=self.segy_logger,
+        )
         self.sweep_length = SegyHeaderItem(
-            sample_format=DATA_SAMPLE_FORMAT_INT16, 
+            sample_format=DATA_SAMPLE_FORMAT_INT16,
             start_byte=37,
-            description='sweep length')
+            description="sweep length",
+            segy_logger=self.segy_logger,
+        )
         self.sweep_code = SegyHeaderItem(
-            sample_format=DATA_SAMPLE_FORMAT_INT16, 
+            sample_format=DATA_SAMPLE_FORMAT_INT16,
             start_byte=39,
-            description='sweep type code',
-            map_dict=SWEEP_TYPE_CODE)
+            description="sweep type code",
+            map_dict=SWEEP_TYPE_CODE,
+            segy_logger=self.segy_logger,
+        )
         self.sweep_chan = SegyHeaderItem(
-            sample_format=DATA_SAMPLE_FORMAT_INT16, 
+            sample_format=DATA_SAMPLE_FORMAT_INT16,
             start_byte=41,
-            description='trace number of sweep channel')
+            description="trace number of sweep channel",
+            segy_logger=self.segy_logger,
+        )
         self.sweep_taper_length_start = SegyHeaderItem(
-            sample_format=DATA_SAMPLE_FORMAT_INT16, 
+            sample_format=DATA_SAMPLE_FORMAT_INT16,
             start_byte=43,
-            description='sweep trace taper length in ms at start')
+            description="sweep trace taper length in ms at start",
+            segy_logger=self.segy_logger,
+        )
         self.sweep_taper_length_end = SegyHeaderItem(
-            sample_format=DATA_SAMPLE_FORMAT_INT16, 
+            sample_format=DATA_SAMPLE_FORMAT_INT16,
             start_byte=45,
-            description='sweep trace taper length in ms at end')
+            description="sweep trace taper length in ms at end",
+            segy_logger=self.segy_logger,
+        )
         self.taper_type = SegyHeaderItem(
-            sample_format=DATA_SAMPLE_FORMAT_INT16, 
+            sample_format=DATA_SAMPLE_FORMAT_INT16,
             start_byte=47,
-            description='taper type',
-            map_dict=TAPER_TYPE)
+            description="taper type",
+            map_dict=TAPER_TYPE,
+            segy_logger=self.segy_logger,
+        )
         self.correlated_traces = SegyHeaderItem(
-            sample_format=DATA_SAMPLE_FORMAT_INT16, 
+            sample_format=DATA_SAMPLE_FORMAT_INT16,
             start_byte=49,
-            description='correlated data traces',
-            map_dict=CORRELATED_DATA_TRACES)
+            description="correlated data traces",
+            map_dict=CORRELATED_DATA_TRACES,
+            segy_logger=self.segy_logger,
+        )
         self.binary_gain = SegyHeaderItem(
-            sample_format=DATA_SAMPLE_FORMAT_INT16, 
+            sample_format=DATA_SAMPLE_FORMAT_INT16,
             start_byte=51,
-            description='binary gain recovered',
-            map_dict=BINARY_GAIN_RECOVERED)
+            description="binary gain recovered",
+            map_dict=BINARY_GAIN_RECOVERED,
+            segy_logger=self.segy_logger,
+        )
         self.amp_recovery_method = SegyHeaderItem(
-            sample_format=DATA_SAMPLE_FORMAT_INT16, 
+            sample_format=DATA_SAMPLE_FORMAT_INT16,
             start_byte=53,
-            description='amplitude recovery method',
-            map_dict=AMPLITUDE_RECOVERY_METHOD)
+            description="amplitude recovery method",
+            map_dict=AMPLITUDE_RECOVERY_METHOD,
+            segy_logger=self.segy_logger,
+        )
         self.measurement_system = SegyHeaderItem(
-            sample_format=DATA_SAMPLE_FORMAT_INT16, 
+            sample_format=DATA_SAMPLE_FORMAT_INT16,
             start_byte=55,
-            description='measurement system',
-            map_dict=MEASUREMENT_SYSTEM)
+            description="measurement system",
+            map_dict=MEASUREMENT_SYSTEM,
+            segy_logger=self.segy_logger,
+        )
         self.polarity = SegyHeaderItem(
-            sample_format=DATA_SAMPLE_FORMAT_INT16, 
+            sample_format=DATA_SAMPLE_FORMAT_INT16,
             start_byte=57,
-            description='impulse signal polarity',
-            map_dict=IMPULSE_SIGNAL_POLARITY)
+            description="impulse signal polarity",
+            map_dict=IMPULSE_SIGNAL_POLARITY,
+            segy_logger=self.segy_logger,
+        )
         self.vibe_polarity = SegyHeaderItem(
             sample_format=DATA_SAMPLE_FORMAT_INT16,
             start_byte=59,
-            description='vibratory polarity code',
-            map_dict=VIBRATORY_POLARITY_CODE)
+            description="vibratory polarity code",
+            map_dict=VIBRATORY_POLARITY_CODE,
+            segy_logger=self.segy_logger,
+        )
         # unassigned
         self.segy_revision = SegyHeaderItem(
-            sample_format=DATA_SAMPLE_FORMAT_INT16, 
+            sample_format=DATA_SAMPLE_FORMAT_INT16,
             start_byte=301,
-            description='segy format revision number',
-            value=2)
+            description="segy format revision number",
+            value=2,
+            segy_logger=self.segy_logger,
+        )
         self.fixed_length = SegyHeaderItem(
-            sample_format=DATA_SAMPLE_FORMAT_INT16, 
+            sample_format=DATA_SAMPLE_FORMAT_INT16,
             start_byte=303,
-            description='fixed length trace flag')
+            description="fixed length trace flag",
+            segy_logger=self.segy_logger,
+        )
         self.num_txt_headers = SegyHeaderItem(
-            sample_format=DATA_SAMPLE_FORMAT_INT16, 
+            sample_format=DATA_SAMPLE_FORMAT_INT16,
             start_byte=305,
-            description='number of 3200 byte ext file header records following')
+            description="number of 3200 byte ext file header records following",
+            segy_logger=self.segy_logger,
+        )
         # unassigned
 
     # --- METHODS ---
     def segy_type(self) -> str:
-        """Return the segy type, e.g. 'ibm', 'int32', 'int16', 'float32', or 'int8'.
+        """Return the segy type, e.g. 'ibm', 'int32', 'int16', 'float32', or \
+            'int8'.
         """
+        # TODO: warning if unable to map value to DATA_SAMPLE_FORMAT_CODE; "segytools will not be able to unpack"
+        # if self.data_sample_format_code.value not in [0, 1, 2, 3, 5, 8]
         return self.data_sample_format_code._mapped_value
 
     def sample_format_size_in_bytes(self) -> int:
-        """Return the number of bytes in each sample based on the `data_sample_format_code`.
+        """Return the number of bytes in each sample based on the \
+            `data_sample_format_code`.
         """
         fmt = self.data_sample_format_code._mapped_value
         byte_size = 4  # default
-        if fmt == 'ibm':
+        if fmt == "ibm":
             byte_size = 4
-        elif fmt == 'float32':
+        elif fmt == "float32":
             byte_size = 4
-        elif fmt == 'int32':
+        elif fmt == "int32":
             byte_size = 4
-        elif fmt == 'int16':
+        elif fmt == "int16":
             byte_size = 2
-        elif fmt == 'int8':
+        elif fmt == "int8":
             byte_size = 1
         else:
-            raise ValueError("Unable to determine sample format size in bytes as sample format is undefined.")
+            raise ValueError(
+                "Unable to determine sample format size in bytes \
+                as sample format is undefined."
+            )
+        # self.segy_logger.debug(f'sample format {fmt} size in bytes is {byte_size}')
         return byte_size
-    
+
     # TODO: def is_fixed_length(self):
     #     if self.fixedlen == ??:
     #         return True
     #     else:
     #         return False
```

### Comparing `segytools-0.1.0/src/segytools/segy_header_item.py` & `segytools-0.1.1/src/segytools/segy_header_item.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,124 +1,141 @@
 '''
 segy header item
 '''
 
 # import python standard modules
 import struct
+import logging
 
 # import 3rd party libraries
 import numpy
-from ibm2ieee import ibm2float32, ibm2float64
+from ibm2ieee import ibm2float32
 
 # import local python
 from segytools.datatypes import DataSampleFormat
 
 
 class SegyHeaderItem(object):
-    """Used to describe a single header item or field in a segy file header or trace header.
+    """Used to describe a single header item or field in a segy file header \
+        or trace header.
 
     Parameters
     ----------
     name : str
         Header item identifier.
     sample_format : DataSampleFormat
         data sample format that tells the system how to interpret the bytes
     start_byte : int
-        Index of the first byte to read. Uses SEGY standard notation which starts a header container at one, not zero. 
-        For example, reading a 4-byte integer header from a bytes or bytearray object, b[0:4] would have a start_byte = 1.
+        Index of the first byte to read. Uses SEGY standard notation which \
+            starts a header container at one, not zero.
+        For example, reading a 4-byte integer header from a bytes or \
+            bytearray object, b[0:4] would have a start_byte = 1.
     description : str
         Description of the header item.
     map_dict : `dict`
-        Dictionary in which the key is the interpreted value. Required if map_bool is True.
+        Dictionary in which the key is the interpreted value. Required if \
+            map_bool is True.
     value : Any
         Header item value.
 
     Methods
     -------
     has_mapping_dictionary
     """
 
-    def __init__(self, sample_format:DataSampleFormat, start_byte:int=0, description:str='', map_dict:dict={}, value=0):
-        self._sample_format = sample_format  # TODO: assert derived from DataSampleFormat name tuple
-        self._n_bytes = sample_format.size_in_bytes  # length of the header in bytes; default to 4, but may be 2
-        self._start_byte = start_byte      # the relative byte location to start reading
-        self._description = description  # defualt to empty string
-        self._value = value              # the value obtained from the segy file
-        self._supplementary = ''         # any additional supplementary material
-        self._map_dict = map_dict        # name of the dictionary to map to
+    def __init__(self, sample_format: DataSampleFormat, start_byte: int = 0,
+                 description: str = '', map_dict: dict = {}, value=0, segy_logger=None):
+        """Constructor"""
+        # TODO: assert derived from DataSampleFormat name tuple
+        self._sample_format = sample_format
+        # length of the header in bytes; default to 4, but may be 2
+        self._n_bytes = sample_format.size_in_bytes
+        # the relative byte location to start reading
+        self._start_byte = start_byte
+        # defualt to empty string
+        self._description = description
+        # the value obtained from the segy file
+        self._value = value
+        # any additional supplementary material
+        self._supplementary = ''
+        # name of the dictionary to map to
+        self._map_dict = map_dict
         self._mapped_value = None
         if map_dict:
             self._mapped_value = map_dict[value]
+        self.segy_logger = segy_logger
 
     def __str__(self):
         s = 'description: ' + self._description + ', '
         s += 'start byte: ' + str(self._start_byte) + ', '
         s += 'byte length: ' + str(self._n_bytes) + ', '
         s += 'value: ' + str(self._value)
         return s
 
     @property
     def sample_format(self) -> DataSampleFormat:
         """Get the sample format of the data."""
         return self._sample_format
-    
+
     @sample_format.setter
-    def sample_format(self, sample_format:DataSampleFormat):
+    def sample_format(self, sample_format: DataSampleFormat):
         """Set the item's data sample format.
 
         Parameters
         ----------
         sample_format : DataSampleFormat
             The format to be set.
         """
-        # TODO: sample format validation; must be a valid DataSampleFormat Enum Type
+        # TODO: sample format validation; must be a valid
+        #   DataSampleFormat Enum Type
         # TODO: convert the value to this format
         self._sample_format = sample_format
         self._n_bytes = sample_format.size_in_bytes
 
     @property
     def n_bytes(self) -> int:
         """Get the item's number of bytes."""
         return self._n_bytes
 
     # NOTE: no _nbytes setter; must be set with data_sample_format()
-    
+
     @property
     def start_byte(self) -> int:
         """Get the item's start byte."""
         return self._start_byte
 
     @start_byte.setter
-    def start_byte(self, start_byte:int):
+    def start_byte(self, start_byte: int):
         """Set the item's start byte.
 
         Parameters
         ----------
         start_byte : int
             start byte value to be set.
         """
         # TODO: start_byte validation; must be non-negative integer
-        self._start_byte = start_byte   
+        self._start_byte = start_byte
 
     @property
     def description(self) -> str:
         """Get the item's description."""
         return self._description
 
     @description.setter
-    def description(self, description:str):
+    def description(self, description: str):
         """Set the item's description.
 
         Parameters
         ----------
         description : str
             Description of item to be set.
         """
         # TODO: description validation; assert is string.
-        # should be short, but doesn't have to be. A very long string may indicate something is being improperly set.
+        # should be short, but doesn't have to be. A very long string
+        #   may indicate something is being improperly set.
         self._description = description
 
     @property
     def value(self):
         """Get the item's value."""
         return self._value
 
@@ -127,110 +144,124 @@
         """Set the item's value.
 
         Parameter
         ---------
         value : Any
             The value to be set.
         """
-        # TODO: if this item is mapped to another value, assert this value assigned matches the type in the mapping.
+        # TODO: if this item is mapped to another value, assert this value
+        #   assigned matches the type in the mapping.
         self._value = value
         if self._map_dict:
             try:
                 self._mapped_value = self._map_dict[value]
             except KeyError:
-                print(f"Unable to map value {value} to header item {self._description}")
+                if self.segy_logger:
+                    self.segy_logger.debug(f"Unable to map value {value} to header item {self._description}")
 
     @property
     def supplementary(self) -> str:
         """Get the item's supplementary content."""
         return self._supplementary
 
     @supplementary.setter
-    def supplementary(self, supplementary:str):
+    def supplementary(self, supplementary: str):
         """Set the item's supplementary content.
 
         Parameters
         ----------
         supplementary : str
             The supplementary content to be set.
         """
         self._supplementary = supplementary
-    
+
     @property
     def map_dict(self) -> dict:
-        """Get the item's mapping dictionary. If not mapping dictionary provided, returns an empty dict."""
+        """Get the item's mapping dictionary. If not mapping dictionary \
+            provided, returns an empty dict."""
         return self._map_dict
 
     @map_dict.setter
-    def map_dict(self, mapping_dictionary:dict):
+    def map_dict(self, mapping_dictionary: dict):
         """Set the item's mapping dictionary."""
         self._map_dict = mapping_dictionary
         self._mapped_value = self._map_dict[self._value]
-    
+
     @property
     def mapped_value(self):
         """Get the item's mapped_value."""
         return self._mapped_value
-    
+
     def has_mapping_dictionary(self) -> bool:
-        """Returns True if there is a mapping dictionary provided to map the interpreted value to another value. Otherwise, returns False."""
+        """Returns True if there is a mapping dictionary provided to map the \
+            interpreted value to another value. Otherwise, returns False."""
         tmp_out = False
         if self._map_dict:
             tmp_out = True
         return tmp_out
 
-
     def to_bytes(self, endianess: str) -> bytes:
-        """Convert the segy header item to a bytes object for writing back out to segy format.
-        
+        """Convert the segy header item to a bytes object for writing back \
+            out to segy format.
+
         Parameters
         ----------
         endianess : str
             '>' for big endian, '<' for little.
         """
         if self._sample_format == 'ibm':
-            raise NotImplementedError("IBM floats are not supported for writing to bytes. Use DataSampleFormat_FLOAT32.")
+            raise NotImplementedError("IBM floats are not supported for \
+                writing to bytes. Use DataSampleFormat_FLOAT32.")
         else:
             fmt = ''.join([endianess, self._sample_format.format])
-            #val = self._value
+            # val = self._value
             bout = struct.pack(fmt, self._value)
         return bout
 
     @staticmethod
-    def value_from_buffer(buf:bytes, endianess:str, sample_format:DataSampleFormat):
+    def value_from_buffer(buf: bytes, endianess: str,
+                          sample_format: DataSampleFormat):
         """Unpack value from buffer.
 
         Parameters
         ----------
         buf : bytes
             buffer
         endianess : str
             either '<' for little or '>' for big endian
         sample_format : DataSampleFormat
             data sample format used for interpreting bytes object.
         """
         if sample_format.format == 'ibm':
             # NOTE: only 32-bit ibm floats currently tested and supported
-            fmt = ''.join([endianess,'u4'])
+            fmt = ''.join([endianess, 'u4'])
             val = ibm2float32(numpy.frombuffer(buffer=buf, dtype='>u4'))
         else:
             fmt = ''.join([endianess, sample_format.format])
             val = struct.unpack(fmt, buf)
             val = val[0]  # unpack always returns a tuple
         return val
-    
-    
+
     @classmethod
-    def from_bytes(cls, buf:bytes, endianess: str, sample_format:DataSampleFormat, start_byte:int=0, description:str='', map_dict:dict={}):
+    def from_bytes(cls, buf: bytes, endianess: str,
+                   sample_format: DataSampleFormat, start_byte: int = 0,
+                   description: str = '', map_dict: dict = {}):
         """Create a segy header item from a bytes object.
 
         Parameters
         ----------
         buf : bytes
             The byte data.
         endianess : str
             '>' for big endian, '<' for little
         """
-        header_item = SegyHeaderItem(sample_format=sample_format, start_byte=start_byte, description=description, map_dict=map_dict)
-        header_item.value = cls.value_from_buffer(buf=buf, endianess=endianess, sample_format=sample_format)
+        header_item = SegyHeaderItem(
+            sample_format=sample_format,
+            start_byte=start_byte,
+            description=description,
+            map_dict=map_dict)
+        header_item.value = cls.value_from_buffer(
+            buf=buf,
+            endianess=endianess,
+            sample_format=sample_format)
 
         return header_item
```

### Comparing `segytools-0.1.0/PKG-INFO` & `segytools-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segytools
-Version: 0.1.0
+Version: 0.1.1
 Summary: low level toolkit for manipulating and analyzing segy formatted data
 License: MIT
 Author: anthonytorlucci
 Author-email: anthonytorlucci@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,13 +13,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: ibm2ieee (>=1.2.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # segytools
 
+[Documentation](https://anthonytorlucci.github.io/segytools/)
+
 `segytools` is a simple python library that provides low level tools for analyzing and parsing segy formatted files. There is no `read_segy()` function per se because that assumes the data is properly formatted in which case there are other tools much better suited, e.g. [segyio](https://github.com/equinor/segyio). The tools here are designed to aid in the analysis of "non-standard" segy files and converting those files to a more standard form easily read by other third party software.
 
 Currently only segy revision 2 file header and trace header formats are provided. However, custom header containers can be created by inheriting `SegyAbstractHeader`.
 
 Originally, much of the work had been derived from another open-source segy package [segpy](https://github.com/sixty-north/segpy), but version `0.1.0` has been almost completely rewritten. IBM float conversion is done with [enthought/ibm2ieee](https://github.com/enthought/ibm2ieee).
```

