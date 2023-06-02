# Comparing `tmp/lkcom-0.3.1.tar.gz` & `tmp/lkcom-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lkcom-0.3.1.tar", last modified: Wed Mar  1 08:05:29 2023, max compression
+gzip compressed data, was "lkcom-0.3.2.tar", last modified: Fri Jun  2 10:19:44 2023, max compression
```

## Comparing `lkcom-0.3.1.tar` & `lkcom-0.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-03-01 08:05:29.221575 lkcom-0.3.1/
--rw-rw-rw-   0        0        0      759 2023-03-01 08:05:29.221575 lkcom-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      332 2021-11-15 10:30:15.000000 lkcom-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-01 08:05:29.214574 lkcom-0.3.1/lkcom/
--rw-rw-rw-   0        0        0      188 2023-03-01 07:58:07.000000 lkcom-0.3.1/lkcom/__init__.py
--rw-rw-rw-   0        0        0     3183 2023-03-01 07:58:13.000000 lkcom-0.3.1/lkcom/cfgparse.py
--rw-rw-rw-   0        0        0    22749 2023-03-01 07:58:18.000000 lkcom-0.3.1/lkcom/dataio.py
--rw-rw-rw-   0        0        0    14989 2023-03-01 07:58:23.000000 lkcom-0.3.1/lkcom/image.py
--rw-rw-rw-   0        0        0    46239 2023-03-01 07:58:28.000000 lkcom-0.3.1/lkcom/plot.py
--rw-rw-rw-   0        0        0     1780 2023-03-01 07:58:32.000000 lkcom-0.3.1/lkcom/standard_func.py
--rw-rw-rw-   0        0        0    25812 2023-03-01 07:58:35.000000 lkcom-0.3.1/lkcom/string.py
--rw-rw-rw-   0        0        0    30037 2023-03-01 07:58:39.000000 lkcom-0.3.1/lkcom/util.py
-drwxrwxrwx   0        0        0        0 2023-03-01 08:05:29.220575 lkcom-0.3.1/lkcom.egg-info/
--rw-rw-rw-   0        0        0      759 2023-03-01 08:05:29.000000 lkcom-0.3.1/lkcom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-03-01 08:05:29.000000 lkcom-0.3.1/lkcom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-01 08:05:29.000000 lkcom-0.3.1/lkcom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-03-01 08:05:29.000000 lkcom-0.3.1/lkcom.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-03-01 08:05:29.000000 lkcom-0.3.1/lkcom.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-01 08:05:29.222577 lkcom-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1327 2022-12-15 15:01:50.000000 lkcom-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:19:44.888178 lkcom-0.3.2/
+-rw-rw-rw-   0        0        0      759 2023-06-02 10:19:44.887178 lkcom-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2021-11-15 10:30:15.000000 lkcom-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 10:19:44.880177 lkcom-0.3.2/lkcom/
+-rw-rw-rw-   0        0        0      188 2023-03-02 15:31:24.000000 lkcom-0.3.2/lkcom/__init__.py
+-rw-rw-rw-   0        0        0     3183 2023-03-01 07:58:13.000000 lkcom-0.3.2/lkcom/cfgparse.py
+-rw-rw-rw-   0        0        0    30480 2023-06-01 06:51:50.000000 lkcom-0.3.2/lkcom/dataio.py
+-rw-rw-rw-   0        0        0    14989 2023-03-01 07:58:23.000000 lkcom-0.3.2/lkcom/image.py
+-rw-rw-rw-   0        0        0    48811 2023-05-22 05:36:02.000000 lkcom-0.3.2/lkcom/plot.py
+-rw-rw-rw-   0        0        0     1780 2023-03-01 07:58:32.000000 lkcom-0.3.2/lkcom/standard_func.py
+-rw-rw-rw-   0        0        0    26131 2023-04-27 13:46:59.000000 lkcom-0.3.2/lkcom/string.py
+-rw-rw-rw-   0        0        0    32944 2023-05-26 06:41:38.000000 lkcom-0.3.2/lkcom/util.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:19:44.886179 lkcom-0.3.2/lkcom.egg-info/
+-rw-rw-rw-   0        0        0      759 2023-06-02 10:19:44.000000 lkcom-0.3.2/lkcom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-06-02 10:19:44.000000 lkcom-0.3.2/lkcom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 10:19:44.000000 lkcom-0.3.2/lkcom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-06-02 10:19:44.000000 lkcom-0.3.2/lkcom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-02 10:19:44.000000 lkcom-0.3.2/lkcom.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 10:19:44.888178 lkcom-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1327 2022-12-15 15:01:50.000000 lkcom-0.3.2/setup.py
```

### Comparing `lkcom-0.3.1/PKG-INFO` & `lkcom-0.3.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lkcom
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Python library of useful routines.
 Home-page: https://bitbucket.org/lukaskontenis/lkcom/
 Author: Lukas Kontenis
 Author-email: dse.ssd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lkcom-0.3.1/lkcom/cfgparse.py` & `lkcom-0.3.2/lkcom/cfgparse.py`

 * *Files identical despite different names*

### Comparing `lkcom-0.3.1/lkcom/dataio.py` & `lkcom-0.3.2/lkcom/dataio.py`

 * *Files 17% similar despite different names*

```diff
@@ -44,14 +44,35 @@
 
 def get_file_mod_date_str(file_name):
     date = get_file_mod_date(file_name)
     if date:
         return time.strftime("%Y-%m-%d", time.gmtime(date))
 
 
+def get_file_timestamp_str(file_name, format='%Y-%m-%d', parent_file_ext=None):
+    """Get file time stamp string based on OS creation date.
+
+    The parent_file_ext argument can be used to check whether the parent
+    directory contains an h5 or zip file from which the data file could have
+    been produced later and thus would have an incorrect creation timestamp.
+    """
+    data_file_name = file_name
+    if parent_file_ext:
+        parent_file_names = list_files_with_extension(get_parent_dir(file_name), parent_file_ext)
+        if len(parent_file_names == 1):
+            print("Using parent file timestamp")
+            data_file_name = parent_file_names[0]
+        elif len(parent_file_names > 1):
+            print("WARNING: Multiple parent files found in the parent directory, using the first one")
+            data_file_name = parent_file_names[0]
+
+    return get_file_creation_date_str(data_file_name)
+
+
+
 def parse_csv_header(file_name, key):
     """Find a value for a given key in the header of a CSV file.
 
     The expected CSV file format is:
     # Comments, key1: value1, key2: value2, ...
     # Var1 (Unit1), Var2 (Unit2)
     [Data]
@@ -178,38 +199,48 @@
         data_name = data_names[key_ind]
         print("Exporting " + data_name)
         farr = np.array(data_file.get(
             key + '/dev1940/demods/0/sample/frequency'))
         varr = np.array(data_file.get(
             key + '/dev1940/demods/0/sample/r'))
         parr_dbm = 10*np.log10(varr**2/50*1E3)
-        bw = np.array(data_file.get('000/dev1940/demods/0/sample/bandwidth'))
+        bw = np.array(data_file.get(key+ '/dev1940/demods/0/sample/bandwidth'))
+        parr_dbmhz = parr_dbm - 10*np.log10(bw)
         if (np.diff(bw[np.logical_not(np.isnan(bw))]) != 0).any():
             print("WARNING: data has variable bandwidth")
+            bw_str = '{:.0f} - {:.0f} Hz'.format(np.nanmin(bw), np.nanmax(bw))
+        else:
+            bw_str = '{:.0f}'.format(np.nanmean(bw))
         file_name = '{:d}_{:s}.dat'.format(
             key_ind, data_name.replace(':', '_'))
         header_str = \
-            'HF2LI sweeper data, index: {:d}, name: {:s}, bw: {:.0f}'.format(
-                key_ind, data_name, np.nanmean(bw))
-        header_str += '\nFrequency (Hz), Amplitude (dbm)'
-        np.savetxt(file_name, np.transpose([farr, parr_dbm]), delimiter=',',
+            'HF2LI sweeper data, index: {:d}, name: {:s}, bw: {:s}'.format(
+                key_ind, data_name, bw_str)
+
+        header_str += '\nFrequency (Hz), Amplitude (dBm), PSD (dBm/Hz)'
+        np.savetxt(file_name, np.transpose([farr, parr_dbm, parr_dbmhz]), delimiter=',',
                    header=header_str)
 
     print("\nAll done.")
     input("Press any key to continue...")
 
 
 def check_file_exists(file_path):
     """Check if a file exists."""
     try:
         return os.path.isfile(file_path)
     except FileNotFoundError:
         return False
 
 
+def read_tek_csv(FileName):
+    """Read Tektronix CSV file."""
+    return np.loadtxt(FileName, skiprows=21, delimiter=',')
+
+
 def read_bin_file(file_name):
     """Read a serialized 3D array.
 
     Read a binary file containting a serialized 3D array of uint32 values. The
     first three words of the array are the original 3D array dimmensions.
 
     Btw, this is the default way that LabVIEW writes binary data.
@@ -266,14 +297,18 @@
 
     if ext[0] == '.':
         print("Specify extension as 'txt', do not include the dot")
 
     if path is None:
         path = '.\\'
 
+    if not check_dir_exists(path):
+        print("Directory does not exist")
+        return None
+
     if recursive_dir_search:
         List = []
         for root, subdirs, files in os.walk(path):
             List += [Path(root) / Path(file_name) for file_name in files]
     else:
         List = [Path(entry) for entry in os.listdir(path)]
 
@@ -289,20 +324,20 @@
                         break
             else:
                 if(str(FileName).find(name_exclude_filter1) != -1):
                     filter_hit = True
                     break
 
         if name_include_filter:
-            if(str(FileName).find(name_include_filter) == -1):
+            if(str(FileName).lower().find(name_include_filter.lower()) == -1):
                 filter_hit = True
                 continue
 
         if not filter_hit and FileName.suffix[1:] == ext:
-            Paths.append(str(FileName.absolute()))
+            Paths.append(str(Path(path) / FileName))
 
     return Paths
 
 
 def list_files_with_filter(filter_str="*"):
     return glob.glob(filter_str)
 
@@ -344,20 +379,49 @@
         return [Path(path).joinpath(Path(file_name)) for
                 file_name in matched_file_names]
     else:
         return matched_file_names
 
 
 def check_file_exists(file_path):
+    """Check if a file exists."""
     try:
         return os.path.isfile(file_path)
     except FileNotFoundError:
         return False
 
 
+def check_dir_exists(dir_path):
+    """Check if a directory exists."""
+    try:
+        return os.path.isdir(dir_path)
+    except FileNotFoundError:
+        return False
+
+
+def get_parent_dir(file_name):
+    """Get the absolute path to the parent directory of a file"""
+    return Path(file_name).parent.absolute()
+
+
+def open_csv_file(file_name, archive_file_name=None):
+    """Open a CSV file with ZIP archive support.
+
+    Open a CSV file which can reside in a ZIP archive.
+    """
+    if archive_file_name:
+        archive = zipfile.ZipFile(archive_file_name, mode='r')
+        file = io.BufferedReader(
+            archive.open(file_name, mode='r'))
+    else:
+        file = open(file_name)
+
+    return file
+
+
 def read_big_file(FileName, max_row=None):
     f_sz = get_file_sz(FileName)
 
     fin = open(FileName, 'r')
     line = ' '
     ind = 0
     try:
@@ -395,16 +459,18 @@
 
     fin.close()
 
     return np.resize(D, [ind, num_col])
 
 
 def read_starlab_file(FileName, max_row=None):
-    """
-    Read a text log file produced by StarLab.
+    """Read a text log file produced by StarLab.
+
+    StarLab logs data with second timestamps. Times are converted to hours to
+    match PowerMeter data.
     """
     f_sz = get_file_sz(FileName)
 
     fin = open(FileName, 'r')
     line = ''
     ind = 0
     try:
@@ -413,63 +479,81 @@
                 if line == '' or line[0] == ';' or line[0] == '!' \
                         or line == '\n':
                     continue
 
                 if line.find('Timestamp') != -1:
                     continue
 
-                l_data = line.strip().split('\t')
+                l_data = [val_str.strip() for val_str in line.split('\t')]
 
                 if ind == 0:
                     l_sz = len(line)
                     num_row = int(np.ceil(f_sz/l_sz))
                     f_num_row = num_row
                     if max_row is not None and num_row > max_row:
                         num_row = max_row
                     num_col = len(l_data)
 
                     D = np.ndarray([num_row, num_col])
 
+                if len(l_data) < num_col:
+                    print("Line {:d} is truncated, skipping".format(ind))
+                    continue
+
                 for indC in range(0, num_col):
-                    D[ind, indC] = float(l_data[indC])
+                    try:
+                        D[ind, indC] = float(l_data[indC])
+                    except ValueError:
+                        D[ind, indC] = np.nan
 
                 ind = ind + 1
 
                 if ind % 1E5 == 0:
                     print("{:d}k lines read, {:.3f} of chunk, {:.3f} of "
                           "file".format(ind/1E3, ind/num_row, ind/f_num_row))
 
                 if max_row is not None and ind >= max_row:
                     break
 
-    except Exception:
-        print("Error while reading file")
-        exc_type, _, exc_tb = sys.exc_info()
-        fname = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
-        print(exc_type, fname, exc_tb.tb_lineno)
+    except Exception as excpt:
+        print("Error while reading file at ind {:d}: {:}".format(ind, excpt))
 
     fin.close()
 
     D = np.resize(D, [ind, num_col])
 
-    return D
+    data = dict()
+    for ind in range(num_col - 2):
+        vals = D[:, ind+1]
+        mask = np.logical_not(np.isnan(vals))
+
+        # StarLab data is in seconds, convert to hours as PowerMeter
+        data['tarr{:d}'.format(ind)] = D[mask, 0]/60/60
+
+        data['vals{:d}'.format(ind)] = vals[mask]
+
+    return data
 
 
 def read_text_sa_file(file_name):
     """Read a generic text file containing spectrum analyzer data."""
     data = np.loadtxt(file_name, delimiter=',')
 
     rbw = None
     attn = None
     with open(file_name) as file_h:
         for line in file_h:
             if line[0] != '#':
                 break
             if line.find('bw:') != -1:
-                rbw = float(line.split('bw: ')[1].split(',')[0])
+                rbw_str = line.split('bw: ')[1].split(',')[0]
+                if rbw_str.find('-') != -1:
+                    rbw = 'variable'
+                else:
+                    rbw = float(line.split('bw: ')[1].split(',')[0])
 
     cfg = {'RBW': rbw, 'Attenuation': attn}
 
     return data, cfg
 
 
 def read_rigol_sa_csv(file_name):
@@ -586,14 +670,17 @@
         for dir_name_month in list_dirs('positioning'):
             for dir_name_day in list_dirs('positioning/' + dir_name_month):
                 dir_list = 'positioning/' + dir_name_month + '/' + dir_name_day
 
     for dir in dir_list:
         for ind, signal in enumerate(signal_names):
             file_name = dir + '/{:s}.txt'.format(signal)
+            if not check_file_exists(file_name):
+                print("File '{:}' not found, skipping signal".format(file_name))
+                continue
             print("Reading file ", file_name)
             try:
                 if Path(Path(file_name).parts[0]).suffix == '.zip':
                     zip_file_name = Path(Path(file_name).parts[0])
                     archive = zipfile.ZipFile(zip_file_name, mode='r')
                     file = io.BufferedReader(
                         archive.open(Path(
@@ -662,7 +749,129 @@
                                pos_log[ind]['t0']).total_seconds()/60/60))
 
                     pos_log[ind]['val'] = np.append(
                         pos_log[ind]['val'],
                         data_val)
 
     return pos_log
+
+
+def read_powerscanner_tsv(file_name=None, ):
+    """Read a PowerScanner TSV file.
+
+    The file contains tab-separated values. The header is three rows, likely
+    alwayws, but may be different if the data is unnamed.
+
+    The columns are wavelength in nm, transmission in % for s and p
+    polarization and background in counts. When transmission is in %, the
+    background column is likely unuseable.
+    """
+    try:
+        with open(file_name) as data_file:
+            header = data_file.readline()
+
+        col_names = [col_name.lower() for col_name in header.split('\t')]
+
+        data_keys = {'wavl', 'trans_s', 'trans_p'}
+        data_col_names = {'wavl': 'wavelength', 'trans_s': 'transmittance(s)', 'trans_p': 'transmittance(p)'}
+        data_fac = {'wavl': 1, 'trans_s': 1E-2, 'trans_p': 1E-2}
+
+        # File column to data key mapping
+        data_col_inds = dict([(data_key, None) for data_key in data_keys])
+
+        for ind, file_col_name in enumerate(col_names):
+            for data_key in data_col_names.keys():
+                if file_col_name == data_col_names[data_key]:
+                    data_col_inds[data_key] = ind
+
+        if data_col_inds['wavl'] is None:
+            raise Exception("Could not find wavelength column")
+
+        if data_col_inds['trans_s'] is None and data_col_inds['trans_p']:
+            raise Exception("Could not find transmission columns")
+
+        filter_data = np.loadtxt(file_name, skiprows=3, delimiter='\t')
+
+        # Output data dict
+        data = dict([(data_key, None) for data_key in data_keys])
+
+        for data_key in data_col_inds.keys():
+            data[data_key] = filter_data[:, data_col_inds[data_key]]*data_fac[data_key]
+
+        return data
+    except Exception as excpt:
+        if isinstance(excpt, OSError) and excpt.errno == 9:
+            print("Cannot open data file due to OSError 9. If the file is on OneDrive, it is likely the file is not synched to the local computer. ")
+        else:
+            print("A general exception occurred while reading the data file")
+
+        raise excpt
+
+
+def float_loc_parser(str):
+    """Localized float parser to handle comma decimal separation."""
+    return float(str.decode('utf8').replace(',', '.'))
+
+
+def read_rdisp_temporal_envelope(file_name):
+    """Read RDisp temporal envelope."""
+
+    fid = open(file_name)
+    fid.readline()
+    data = None
+    data_cols = None
+    for line in fid:
+        data_row = line.split(',')
+        if data_cols:
+            for ind, val in enumerate(data_row):
+                if val:
+                    data_cols[ind].append(float(val))
+        else:
+            data_cols = [[float(val)] for val in data_row]
+
+    col_names = 'tarr_tl', 'ampl_tl', 'tarr', 'ampl'
+    data = {}
+    for ind, col_name in enumerate(col_names):
+        data[col_name] = np.array(data_cols[ind])
+
+    if np.all(data['tarr_tl'] == 0):
+        data['tarr_tl'] = np.linspace(-1000, 1000, len(data['tarr_tl']))
+        print("WARNING: CSV file contains no time values, assuming -1 ps to 1 ps")
+
+    if np.all(data['tarr'] == 0):
+        data['tarr'] = np.linspace(-1000, 1000, len(data['tarr']))
+        print("WARNING: CSV file contains no time values, assuming -1 ps to 1 ps")
+
+    return data
+
+
+
+
+def read_frog_temporal_envelope(dir_name):
+    """Read FROG retrieval temporal envelope."""
+    if check_dir_exists(dir_name):
+        file_name = list_files_with_extension(
+            dir_name, ext='dat', name_include_filter='Ek')[0]
+    elif check_file_exists(dir_name):
+        file_name = dir_name
+
+    data = np.loadtxt(file_name)
+
+    return {'tarr': data[:, 0], 'ampl': data[:, 1]}
+
+
+def read_d_scan_spectrum(dir_name):
+    """Read spectrum from a Sphere Photonics d-scan retrieval."""
+    file_name = list_files_with_extension(dir_name, ext='txt', name_include_filter='spectrum')[0]
+
+    data = np.loadtxt(file_name, converters={0: float_loc_parser, 1:float_loc_parser, 2:float_loc_parser, 3:float_loc_parser}, skiprows=1)
+
+    return {'wavl': data[:, 0], 'spec': data[:, 1], 'spec_ret': data[:, 2], 'spec_phase': data[:, 3]}
+
+
+def read_d_scan_temporal_envelope(dir_name):
+    """Read temporal envelope from a Sphere Photonics d-scan retrieval."""
+    file_name = list_files_with_extension(dir_name, ext='txt', name_include_filter='retrieved_pulse')[0]
+
+    data = np.loadtxt(file_name, converters={0: float_loc_parser, 1:float_loc_parser, 2:float_loc_parser}, skiprows=1)
+
+    return {'tarr': data[:, 0], 'ampl_ds': data[:, 1], 'ampl_tl': data[:, 2]}
```

### Comparing `lkcom-0.3.1/lkcom/image.py` & `lkcom-0.3.2/lkcom/image.py`

 * *Files identical despite different names*

### Comparing `lkcom-0.3.1/lkcom/plot.py` & `lkcom-0.3.2/lkcom/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from PIL import Image
 
 from subprocess import Popen
 
 from lkcom.util import isnone, get_color, bin_and_slice_data, hex2byte, \
     get_granularity, handle_general_exception, hist_bin_centers_to_edges, \
-    extend_range, printmsg
+    extend_range, printmsg, estimate_fwhm
 from lkcom.string import get_human_val_str, rem_extension, strip_whitespace
 from lkcom.standard_func import gaussian_1D
 
 
 def get_pt2mm():
     """Get points per mm."""
     pt2mm = 0.352778
@@ -78,21 +78,29 @@
     panel_gap = 15
 
     fig_w = panel_w*numc + panel_gap*(numc-1)
     fig_h = panel_h*numr + panel_gap*(numr-1)
 
     return [fig_w/25.4, fig_h/25.4]
 
-def get_figure_size(fig_width='1.5x'):
+
+def get_figure_size(fig_width='1.5x', fig_height=None, **kwargs):
+    fig_size = [4.724, 2.635]
     if fig_width == '1x':
-        return [3.504, 2.635]
+        fig_size[0] = 3.504
     elif fig_width == '1.5x':
-        return [4.724, 2.635]
+        fig_size[0] = 4.724
     elif fig_width == '2x':
-        return [7.205, 2.635]
+        fig_size[0] = 7.205
+
+    if fig_height:
+        fig_size[1] = 2.635*float(fig_height.replace('x', ''))
+
+    return fig_size
+
 
 def figure_with_subplots(numr=2, numc=2, title=None):
     """Create a figure with a subplot grid."""
     plt.figure(num=title, figsize=get_def_fig_size(numr, numc),)
     subplot_grid = gridspec.GridSpec(numr, numc, wspace=0.2, hspace=0.2)
     return subplot_grid
 
@@ -110,14 +118,15 @@
 
     return plt.figure(fig_id)
 
 
 def export_figure(
         fig_name, size=None, output_format='.png', pdf_also=False,
         resize=False, suffix="", verbose=False,
+        parent_file_path=None,
         fig_dpi=200, remove_fig_ext=True, **kwargs):
     """Export a figure to a PNG file.
 
     To save a PDF in addition to the selected output format set pdf_also
     to True. This is useful to generte a vector figure for post-processing in
     addition to the raster figure for quick viewing.
     """
@@ -157,14 +166,17 @@
         fig_file_name = rem_extension(fig_name) + suffix + output_format
     else:
         fig_file_name = fig_name + suffix + output_format
 
     if(verbose):
         print("Exporting figure " + fig_file_name + "...")
 
+    if parent_file_path:
+        fig_file_name = Path(*[*Path(parent_file_path).parts[:-1], fig_file_name])
+
     try:
         # Setting the bbox_inches option to 'tight' produces an exception in
         # Tkinter
         # plt.savefig(fig_file_name, dpi=600, bbox_inches='tight')
         plt.savefig(fig_file_name, dpi=fig_dpi)
     except Exception:
         handle_general_exception("Could not export figure")
@@ -178,17 +190,19 @@
 
 
 def show_png_ext(FileName):
     Popen([r'C:\Program Files (x86)\XnView\xnview.exe', FileName])
 
 
 def hist(
-        yarr, yrng=None, target_num_bins=256, hist_bin_sz_fac=1, ygran=None,
+        yarr, bins=None, yrng=None, target_num_bins=256, hist_bin_sz_fac=1, ygran=None,
         with_histogram_dither=False, hist_dith_factor=4, hide_x_labels=False,
+        hide_data_labels=False, hide_count_labels=False,
         orientation="vertical", xmarkers=None, ymarkers=None, ylim=None, log=False, legend_str=None,
+        fit_envelope=False, ref_envelope_width=None,
         color=matplotlib.cm.get_cmap('Blues')(0.95)):
     """Plot a nice histogram with dithering and data granularity awareness."""
     if yrng is None:
         yrng = [np.min(yarr), np.max(yarr)]
 
     yspan = yrng[1] - yrng[0]
 
@@ -204,24 +218,25 @@
     ymean = np.nanmean(yarr_all)
 
     print('Y granularity is {:.2e}, scale range is {:.2f} bits'.format(
         ygran, np.log2(yspan/ygran)))
 
     unique_vals = np.unique(yarr_all)
 
-    if len(unique_vals) < target_num_bins:
-        # If the number of unique data values is less than the number of
-        # target histogram bins, the histogram will have bins with no values in
-        # them, which indicates that the histogram resolution is too high.
-        bins = hist_bin_centers_to_edges(np.unique(yarr_all))
-    else:
-        num_bins = yspan/ygran
-        ygrans_per_bin = np.max([np.round(num_bins/target_num_bins), 1])
-        bins = np.arange(
-            yrng[0], yrng[1], ygran*ygrans_per_bin*hist_bin_sz_fac)
+    if bins is None:
+        if len(unique_vals) < target_num_bins:
+            # If the number of unique data values is less than the number of
+            # target histogram bins, the histogram will have bins with no values in
+            # them, which indicates that the histogram resolution is too high.
+            bins = hist_bin_centers_to_edges(np.unique(yarr_all))
+        else:
+            num_bins = yspan/ygran
+            ygrans_per_bin = np.max([np.round(num_bins/target_num_bins), 1])
+            bins = np.arange(
+                yrng[0], yrng[1], ygran*ygrans_per_bin*hist_bin_sz_fac)
 
     num_bins = len(bins)
 
     if abs(len(bins)/target_num_bins - 1) > 0.1:
         print("Number of histogram bins requested: {:d}, actual number is {:d}"
               " due to data granularity".format(target_num_bins, num_bins))
 
@@ -240,16 +255,31 @@
               " the histogram with and without dithering.")
 
     else:
         dith = 1
 
     yarr = [arr*dith for arr in yarr]
 
-    plt.hist(yarr, bins=bins, orientation=orientation, stacked=True,
-             color=color, zorder=10, log=log, alpha=0.5)
+    bin_counts = plt.hist(yarr, bins=bins, orientation=orientation, stacked=True,
+             color=color, zorder=10, log=log, alpha=0.5)[0]
+
+    envelope_xarr = np.linspace(yrng[0], yrng[1], 500)
+    if fit_envelope:
+        fit_envelope_yarr = gaussian_1D(envelope_xarr, A=np.max(bin_counts), sigma=np.std(yarr), c=np.mean(yarr))
+        if log:
+            plt.semilogy(envelope_xarr, fit_envelope_yarr, c='r')
+        else:
+            plt.plot(envelope_xarr, fit_envelope_yarr, c='r')
+
+    if ref_envelope_width:
+        ref_envelope_yarr = gaussian_1D(envelope_xarr, A=np.max(bin_counts), sigma=ref_envelope_width, c=np.mean(yarr))
+        if log:
+            plt.semilogy(envelope_xarr, ref_envelope_yarr, c='k', ls='--')
+        else:
+            plt.plot(envelope_xarr, ref_envelope_yarr, c='k', ls='--')
 
     if legend_str:
         plt.legend(legend_str)
 
     ax = plt.gca()
 
     if xmarkers:
@@ -257,24 +287,35 @@
             add_x_marker(xmarker, c=[0, 0, 0], ls='-')
 
     if ymarkers:
         # Add histogram y markers
         for ymarker in ymarkers:
             add_y_marker(ymarker, c=[0.75, 0.75, 0.75], ls='-', zorder=1)
 
-    plt.xlim([bins[0], bins[-1]])
-    plt.gca().set_ylim(bottom=1)
-
-    plt.ylim(ylim)
-    plt.plot(plt.xlim(), [0, 0], color=[0, 0, 0, 0.25])
-    if hide_x_labels:
-        plt.xticks([])
-        ax.axes.yaxis.set_ticklabels([])
+    if orientation == 'vertical':
+        plt.xlim(yrng)
+        plt.gca().set_ylim(bottom=1)
+        plt.ylim(ylim)
+        plt.plot(plt.xlim(), [0, 0], color=[0, 0, 0, 0.25])
+        ax = plt.gca()
+        if hide_data_labels:
+            ax.xaxis.set_ticklabels([])
+        if hide_count_labels:
+            ax.yaxis.set_ticklabels([])
+    else:
+        plt.ylim(yrng)
+        plt.xlim(ylim)
+        plt.plot(plt.ylim(), [0, 0], color=[0, 0, 0, 0.25])
+        ax = plt.gca()
+        if hide_data_labels:
+            ax.yaxis.set_ticklabels([])
+        if hide_count_labels:
+            ax.xaxis.set_ticklabels([])
 
-    plt.gca().tick_params(axis='both', direction='in')
+    set_ticks_inside()
     plt.grid('on')
 
     return ax
 
 
 def make_histogram_panel(varr, ax_hist=None, ylim=None, rsd_val=None,
         ax_trace=None, hist_orientation='horizontal',
@@ -352,21 +393,28 @@
 
 no_signal_color = [0.25, 0.25, 0.25]
 
 
 def imshow_ex(
         img, ax=None,
         vmin=None, vmax=None, vrng_algorithm='minmax', min_vspan=None,
+        vrng_symmetric=False,
         auto_vrng_percentile_min=0, auto_vrng_percentile_max=99.5,
         bad_color=no_signal_color, logscale=False, cmap='viridis',
-        title_str=None, with_hist=True, is_angle=False):
+        title_str=None, with_hist=True, is_angle=False, **kwargs):
     """Show an image with a histogram and colorbar.
 
     TODO: ShowImage says it does the same, integrate the two.
     """
+    if kwargs.get('roi_sz'):
+        roi_sz = kwargs.get('roi_sz')
+        roi_ofs = kwargs.get('roi_sz', np.array(img.shape)/2)
+        img = img[int(roi_ofs[0] - roi_sz[0]/2):int(roi_ofs[0] + roi_sz[0]/2),
+                  int(roi_ofs[1] - roi_sz[1]/2):int(roi_ofs[1] + roi_sz[1]/2)]
+
 
     if ax is None:
         ax = plt.gca()
 
     if is_angle:
         img = img/np.pi*180
 
@@ -395,14 +443,18 @@
             vmax = np.nanpercentile(img.flatten(), auto_vrng_percentile_max)
 
     if min_vspan is not None and vmax - vmin < min_vspan:
         vmean = np.mean([vmin, vmax])
         vmin = vmean - min_vspan/2
         vmax = vmean + min_vspan/2
 
+    if vrng_symmetric:
+        vmax = np.max(np.abs([vmin, vmax]))
+        vmin = -vmax
+
     cmap = copy.copy(matplotlib.cm.get_cmap(cmap))
     cmap.set_bad(color=bad_color)
 
     plt.imshow(img, cmap=cmap, vmin=vmin, vmax=vmax)
     hide_axes()
 
     if title_str is None:
@@ -539,15 +591,19 @@
                 text_x = xl[1] - ofs_x
                 text_ha = 'right'
 
         if not text_y:
             if infobox_vpos == 'top':
                 if ref_y is None:
                     ref_y = yl[1]
-                text_y = ref_y - ofs_y
+                if plt.gca().get_yaxis().get_scale() == 'log':
+                    text_y = ref_y**(1-0.07)
+                else:
+                    text_y = ref_y - ofs_y
+
             elif infobox_vpos == 'middle':
                 text_y = (yl[1] - yl[0])/2
             elif infobox_vpos == 'bottom':
                 if ref_y is None:
                     ref_y = yl[0]
                 text_y = ref_y + ofs_y
 
@@ -618,18 +674,18 @@
                     xpos = xlim[0]+xspan*0.075
                     label_ha = 'left'
                 else:
                     xpos = xlim[1]-xspan*0.075
                     label_ha = 'right'
             elif scale_type == 'log':
                 if label_pos == 'left':
-                    xpos = 10**(np.log10(xlim[0])+np.log10(xspan)*0.075)
+                    xpos = 10**(np.log10(xlim[0])+np.log10(xspan)*0.03)
                     label_ha = 'left'
                 else:
-                    xpos = 10**(np.log10(xlim[0])-np.log10(xspan)*0.075)
+                    xpos = 10**(np.log10(xlim[0])-np.log10(xspan)*0.03)
                     label_ha = 'right'
 
         if verbose:
             print("Adding '{:}' label at ({:}, {:})".format(label, xpos, ypos))
         plt.text(
             xpos, ypos, label, ha=label_ha, va=label_va,
             **text_opts)
@@ -644,14 +700,26 @@
 
 
 def add_y_marker(pos, label=None, **kwargs):
     """Add a marker line at Y position."""
     add_marker(pos, label, axis='y', **kwargs)
 
 
+def fwhm_marker(xarr, yarr, color='k', ls='-', standoff=None):
+    """Mark FWHM with a line."""
+    color = np.append(np.copy(color), 0.75)
+    fwhm_rng = estimate_fwhm(xarr, yarr)
+    if standoff:
+        xspan = np.diff(plt.xlim())
+        fwhm_rng[0] += xspan*standoff
+        fwhm_rng[1] -= xspan*standoff
+
+    plt.plot(fwhm_rng, np.array([1, 1])*np.nanmax(yarr)/2, ls=ls, color=color)
+
+
 def add_watermark(watermark_pos='center', fig=None):
     """Add a LC watermark to the figure."""
     if watermark_pos is None:
         return
 
     if watermark_pos not in ['center', 'upper-left', 'bottom-left']:
         print("Unsupported watermark position ''{:s}''".format(watermark_pos))
@@ -1130,14 +1198,15 @@
 
     ax_hist = None
     if(with_hist):
         ax_hist = plt.subplot(grid[0, 4])
         y_span = yl[1] - yl[0]
         y_gran = get_granularity(Y)
 
+        y_units = 's'
         try:
             if ylabel:
                 y_units = strip_whitespace(ylabel.split(',')[1])
         except Exception:
             y_units = ''
         printmsg('Y granularity is {:.2e} {:s}, '.format(y_gran, y_units) +
                  'scale range is {:.2f} bits'.format(np.log2(y_span/y_gran)),
```

### Comparing `lkcom-0.3.1/lkcom/standard_func.py` & `lkcom-0.3.2/lkcom/standard_func.py`

 * *Files identical despite different names*

### Comparing `lkcom-0.3.1/lkcom/string.py` & `lkcom-0.3.2/lkcom/string.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,32 @@
 Copyright 2015-2023 Lukas Kontenis
 Contact: dse.ssd@gmail.com
 """
 import string
 import pathlib
 import numpy as np
 
+import datetime
+
 from lkcom.util import isnone, isarray, grep, msdo, warning_with_info, \
     handle_general_exception, find_closest
 
 
 def strip_nonnum(s):
     return strip_alpha(strip_punctuation(strip_whitespace(s)))
 
 
+def str_is_decimal_num(str):
+    try:
+        val = int(str)
+        return True
+    except Exception as excpt:
+        return False
+
+
 def strip_punctuation(s):
     return s.translate(str.maketrans('', '', string.punctuation))
 
 
 def strip_alpha(s):
     return s.translate(str.maketrans('', '', string.ascii_letters))
 
@@ -289,18 +299,22 @@
 
     if(not np.all(output_str_arr == output_str)):
         warning_with_info("Not all parsed values are consistent")
 
     return output_str
 
 
-def format_timestamp_string(t_str):
-    """
-    Format a filename-safe time stamp string 'HH_MM_SS_.mmm_' to a nicer
-    'HH:MM:SS.mmm from'.
+def parse_timestamp_str(t_str):
+    """Parse timestamp string.
+
+    Format a filename-safe timestamp string 'HH_MM_SS_.mmm_' to a nicer form
+    'HH:MM:SS.mmm'.
+
+    NOT: this function was called format_timestamp_string, but was renamed to
+    not be confused with format_timestamp_into_string.
     """
 
     pieces = t_str.split('_')
     [HH, MM, SS, mmm] = pieces[0:3]
     mmm.strip('.')
 
     return (HH + ':' + MM + ':' + SS + '.' + mmm)
```

### Comparing `lkcom-0.3.1/lkcom/util.py` & `lkcom-0.3.2/lkcom/util.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import time
 
 import numpy as np
 from matplotlib.colors import LinearSegmentedColormap
 from matplotlib.pyplot import get_cmap
 
 
-
 class MultiPrinter(object):
     def __init__(self, *targets):
         self.targets = targets
 
     def write(self, obj):
         for f in self.targets:
             f.write(obj)
@@ -60,23 +59,23 @@
 def isnone(var):
     """Test if a variable is None.
 
     Works for numpy arrays, returns a single boolean result even if the
     variable is an array of None.
 
     """
-    if(isarray(var)):
-        if(type(var) == np.ndarray):
+    if isarray(var):
+        if type(var) == np.ndarray:
             return var.size == 0
         if isinstance(var, type([])):
             # Iterate over the list
             for v in var:
                 # Call isnone recursively for each list element. This should
                 # handle lists of lists
-                if(not isnone(v)):
+                if v is not None:
                     # If at least one element is not None, the list is not None
                     return False
             # If the loop finishes, all elements are none
             return True
         warning_with_info("Asked for isnone() for an unknown array type")
 
     if isinstance(var, type(None)):
@@ -177,15 +176,15 @@
 def msdo(val):
     """Get the order of the most significant digit.
 
     The integer part of a base-10 logarithm is the order of the most
     significant digit.
 
     """
-    if(val == 0):
+    if val == 0:
         return 1
     else:
         return np.floor(np.log10(np.abs(val)))
 
 
 def arg2grep(arr, substr):
     g_inds = []
@@ -201,32 +200,42 @@
 def arggrep(arr, substr):
     g_inds = arg2grep(arr, substr)[0]
     return g_inds
 
 
 def grep(arr, substr, return_inds=False):
     g_inds, g_el = arg2grep(arr, substr)
-    if(return_inds):
+    if return_inds:
         return (g_el, g_inds)
     else:
         return g_el
 
 
 def get_rsd(A):
     """Get the relative standard deviation of an array."""
     return np.nanstd(A)/np.nanmean(A)
 
 
-def find_first(arr, val, equal_only=False, fail_with_nan=False):
+def find_first(
+        arr, val, equal_only=False, fail_with_nan=False, start_ind=None):
     """
     Find the index of the first element in arr that is larger than or equal
     to val. If equal_only is True only equal elements are considered. If no
     elements are found None is returned, unless fail_with_nan is True, in which
     case NaN is returned insread.
     """
+    if start_ind is not None:
+        index = find_first(
+            arr[start_ind:], val, equal_only=equal_only,
+            fail_with_nan=fail_with_nan)
+        if index:
+            return start_ind + index
+        else:
+            return None
+
     if val is None:
         if fail_with_nan:
             return np.nan
         else:
             return None
 
     for index, item in enumerate(arr):
@@ -270,28 +279,45 @@
     """
     if type(arr) == list:
         arr = np.array(arr)
 
     if isarray(val):
         return [find_closest(arr, val1) for val1 in val]
     else:
-        return np.nanargmin((arr-val)**2)
+        if val is None:
+            return None
+        else:
+            return np.nanargmin((arr-val)**2)
 
 
 def interp(xval, xarr, yarr):
     """1D interpolation for increasing or decreasing xarr."""
     if (np.diff(xarr) > 0).all():
         return np.interp(xval, xarr, yarr)
     elif (np.diff(xarr) < 0).all():
         return np.interp(xval, xarr[::-1], yarr[::-1])
     else:
         print("WARNING: xarr is nonmonotonous, interpolation impossible")
         return None
 
 
+def interp_closest(xarr, yarr, yval, yrng=0.1):
+    """Interpolate closest intersection point."""
+    center_ind = find_closest(yarr, yval)
+    from_ind = find_closest(yarr, yval - yrng/2)
+    to_ind = find_closest(yarr, yval + yrng/2)
+    if to_ind - from_ind < 3:
+        from_ind = center_ind - 1
+        to_ind = center_ind + 2
+
+    # NB: the numpy interp variant fails silently for nonincreasing data, i.e.
+    # the falling edge of the peak, and gives subtly wrong results
+    return interp(yval, yarr[from_ind:to_ind], xarr[from_ind:to_ind])
+
+
 def cap_in_range(val, rng):
     """Cap a value inside the given range."""
     if val < rng[0]:
         return rng[0]
     if val > rng[1]:
         return rng[1]
     return val
@@ -358,22 +384,23 @@
     for ind in range(0, lenC*bins):
         from_ind = stride*ind
         to_ind = from_ind + stride
 
         C[indC:indC + stride, ind_bin] = A[from_ind:to_ind]
 
         ind_bin = ind_bin + 1
-        if(ind_bin == bins):
+        if ind_bin == bins:
             ind_bin = 0
             indC = indC + stride
 
     return C
 
 
-def cut_by_x_range(X, Y, rng=None, rng_fr=None, rng_to=None, round_far_range_up=False):
+def cut_by_x_range(X, Y, rng=None, rng_fr=None, rng_to=None,
+                   round_far_range_up=False, action='cut'):
     """Cut X, Y arrays to a range in X.
 
     The X array is assumed to contain monotonously increasing values. The X and
     Y arrays are sorted before cutting.
 
     The range can be specified either as tuple via 'rng', or as from and to
     X values via 'rng_fr' and 'rng_to'. If only either from or to bound is
@@ -390,57 +417,64 @@
         print("X and Y need to have equal lengths")
         return [X, Y]
 
     if rng is not None:
         rng_fr = rng[0]
         rng_to = rng[1]
 
+    if rng_fr is None and rng_to is None:
+        return [X, Y]
+
     # Don't do anything if the X array already fits the requested range
     if np.nanmin(X) > rng_fr and np.nanmax(X) < rng_to:
         return [X, Y]
 
     # Sort arrays
     sort_order = np.argsort(X)
     X = X[sort_order]
     Y = Y[sort_order]
 
-    if(isnone(rng_fr) and isnone(rng_to)):
-        return [X, Y]
-
-    if(isnone(rng_fr)):
+    if rng_fr is None:
         rng_fr_ind = 0
     else:
         rng_fr_ind = find_closest(X, rng_fr)
 
-    if(isnone(rng_to)):
+    if rng_to is None:
         rng_to_ind = -1
     else:
         rng_to_ind = find_closest(X, rng_to)
 
     if round_far_range_up:
         rng_to_ind += 1
 
-    return [X[rng_fr_ind:rng_to_ind], Y[rng_fr_ind:rng_to_ind]]
+    if action == 'cut':
+        return [X[rng_fr_ind:rng_to_ind], Y[rng_fr_ind:rng_to_ind]]
+    elif action == 'nan':
+        X[:rng_fr_ind] = np.nan
+        X[rng_to_ind:] = np.nan
+        Y[:rng_fr_ind] = np.nan
+        Y[rng_to_ind:] = np.nan
+        return [X, Y]
 
 
 def remove_duplicate_points(X, Y):
     """
     Remove points that have duplicate consecutive X values.
     """
 
     X2 = np.empty_like(X)
     Y2 = np.empty_like(Y)
 
     last_val = None
     ind2 = 0
     for ind in range(0, len(X2)):
-        if(isnone(last_val)):
+        if last_val is None:
             duplicate = False
         else:
-            if(Y[ind] == last_val):
+            if Y[ind] == last_val:
                 duplicate = True
             else:
                 duplicate = False
 
         if not duplicate:
             X2[ind2] = X[ind]
             Y2[ind2] = Y[ind]
@@ -553,25 +587,67 @@
     """
     if plus_minus_range:
         return angle - np.round(angle/period)*period
     else:
         return angle - np.floor(angle/period)*period
 
 
-def reduce_trace(X, Y, szr=None, Yred_method='mean'):
-    """
-    Reduce trace to a given number of samples.
-    """
+def get_d4sigma(xarr, yarr, ignore_spacing_check=False, **kwargs):
+    """Get 1D 4-sigma width."""
+    if not ignore_spacing_check and np.std(np.diff(xarr)) != 0:
+        raise RuntimeError("Does not work for data with unequal time spacing")
+
+    xstep = np.mean(np.diff(xarr))
+    xcenter = np.sum(yarr * xarr * xstep) / np.sum(yarr * xstep)
+    mom2 = np.sum(yarr * (xarr - xcenter)**2 * xstep) / np.sum(yarr * xstep)
+
+    # D4sigma in 2D is 2*np.sqrt(2)*np.sqrt(mom2x + mom2y)
+    return 4*np.sqrt(mom2)
+
+
+def estimate_fwhm(xarr, yarr):
+    """Estimate FWHM from a single-peak trace."""
+    return [interp_closest(
+        xarr[:np.argmax(yarr)], yarr[:np.argmax(yarr)], np.max(yarr)/2),
+            interp_closest(
+        xarr[np.argmax(yarr):], yarr[np.argmax(yarr):], np.max(yarr)/2)]
+
+
+def get_pulse_duration(tau_arr, ac_arr, autocorrelation=True, **kwargs):
+    """Estimate FHWM and D4sigma pulse duration from a trace."""
+    pulse_dur = dict()
+
+    pulse_dur['fwhm_pos'] = estimate_fwhm(tau_arr, ac_arr)
+    pulse_dur['fwhm'] = np.abs(np.diff(pulse_dur['fwhm_pos'])[0])
+
+    if autocorrelation:
+        pulse_dur['fwhm'] /= np.sqrt(2)
 
-    if(isnone(szr)):
+    pulse_dur['d4s'] = get_d4sigma(tau_arr, ac_arr, **kwargs)
+
+    # Estimate equivalent FWHM duration from the D4sigma duration of the
+    # autocorrelation trace. The conversion factor for the time envelope
+    # would be 0.589, this includes the np.sqrt(2) second-order
+    # autocorrelation factor.
+    if autocorrelation:
+        pulse_dur['d4s_fwhmeq'] = pulse_dur['d4s']*0.416
+    else:
+        pulse_dur['d4s_fwhmeq'] = pulse_dur['d4s']*0.589
+
+    return pulse_dur
+
+
+def reduce_trace(X, Y, szr=None, Yred_method='mean'):
+    """Reduce trace to a given number of samples."""
+    if szr is None:
         szr = 300
 
     sz = len(X)
 
-    if(sz <= szr):
+    if sz <= szr:
         Xr = X
         Yr = Y
         Yr_sd = np.zeros_like(Xr)
         return [Xr, Yr, Yr_sd]
 
     stepr = round(sz/szr)
 
@@ -580,21 +656,21 @@
     Yr_sd = np.ndarray(szr)
 
     for ind in range(0, szr):
 
         ind_fr = ind*stepr
         ind_to = (ind+1)*stepr
 
-        if(ind_to > sz):
+        if ind_to > sz:
             ind_to = sz
 
         Xr[ind] = np.mean(X[ind_fr:ind_to])
-        if(Yred_method == 'mean'):
+        if Yred_method == 'mean':
             Yr[ind] = np.mean(Y[ind_fr:ind_to])
-        elif(Yred_method == 'bin'):
+        elif Yred_method == 'bin':
             Yr[ind] = np.sum(Y[ind_fr:ind_to])
 
         Yr_sd[ind] = np.std(Y[ind_fr:ind_to])
 
     return [Xr, Yr, Yr_sd]
 
 
@@ -614,29 +690,28 @@
     binE[0] = binC[0] - (binC[1] - binC[0])/2
     binE[-1] = binC[-1] + (binC[-1] - binC[-2])/2
     for ind in range(1, len(binC)):
         binE[ind] = binC[ind] + (binC[ind-1] - binC[ind])/2
 
     return binE
 
+
 def bin_data(D, binsz):
-    """
-    Bin data into bins of a given size.
-    """
+    """Bin data into bins of a given size."""
 
     Dlen = len(D)
     Blen = int(np.floor(Dlen/binsz))
 
     B = np.ndarray(Blen)
 
     for indB in range(0, Blen):
         ind_fr = indB*binsz
         ind_to = (indB+1)*binsz
 
-        if(ind_to > Dlen):
+        if ind_to > Dlen:
             ind_to = Dlen
 
         B[indB] = D[ind_fr:ind_to].sum()
 
     return B
 
 
@@ -652,22 +727,22 @@
     TODO: support nonequal X spacing
     """
 
     xlen = len(X)
 
     bins = [0]
     t = time.time()
-    while(1):
+    while True:
         ind = find_closest(X, X[bins[-1]] + binsz_X)
 
-        if(time.time() - t > 0.2):
+        if time.time() - t > 0.2:
             print("Binning data: {:.3f}".format(ind/xlen))
             t = time.time()
 
-        if(ind >= xlen and ind == bins[-1]):
+        if ind >= xlen and ind == bins[-1]:
             break
 
         bins.append(ind)
 
     numb = len(bins) - 1
 
     Xb = np.ndarray(numb)
@@ -736,35 +811,35 @@
     for ind, arr in enumerate(arrs):
         arr2d[:, ind] = arr
 
     return arr2d
 
 
 def bin_and_slice_data(X=None, Y=None, num_slcs=None, num_bins=None):
-    """
+    """Put data into bins with mean and percentiles.
+
     Combine the data into bins, slice each bin at equidistant percentile levels
     and calculate the value ranges of each level. The number of final bins is
     given by num_bins. The number of slices parameter (num_slcs) specifies the
     number of slices between 0 and median, so that if e.g. num_slcs = 2 the
     data is sliced at 1.0, 0.75, 0.5, 0.25 and 0 fractional levels and there
     are 2 slices above (1 to 0.75, 0.75 to 0.5) and below (0.5 to 0.25, 0.25
     to 0) the median level.
     """
-
-    if(isnone(num_slcs)):
+    if num_slcs is None:
         num_slcs = 10
 
     fracs = np.linspace(100, 0, 2*num_slcs+1)
 
-    if(isnone(num_bins)):
+    if num_bins is None:
         num_bins = 500
 
     sz = len(X)
 
-    if(sz <= num_bins):
+    if sz <= num_bins:
         Xb = X
         Yb = Y
         Yb_lvls = None
         return [Xb, Yb, Yb_lvls]
 
     bin_step = round(sz/num_bins)
 
@@ -773,33 +848,32 @@
     Yb_lvls = np.ndarray([num_bins, len(fracs)])
 
     for ind in range(0, num_bins):
 
         ind_fr = ind*bin_step
         ind_to = (ind+1)*bin_step
 
-        if(ind_to > sz):
+        if ind_to > sz:
             ind_to = sz
 
         Xb[ind] = np.mean(X[ind_fr:ind_to])
         Yb[ind] = np.mean(Y[ind_fr:ind_to])
 
         if ind_fr < ind_to:
             Yb_lvls[ind, :] = np.percentile(Y[ind_fr:ind_to], fracs)
         else:
             Yb_lvls[ind, :] = np.nan
 
-
     return [Xb, Yb, Yb_lvls]
 
 
 def warning_with_info(message):
     print(message)
     exc_type, exc_obj, exc_tb = sys.exc_info()
-    if(not isnone(exc_obj)):
+    if exc_obj is not None:
         fname = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
         print(exc_obj, exc_type, " in ", fname, exc_tb.tb_lineno)
 
 
 def get_exception_info_str():
     """Get exception info string.
 
@@ -874,252 +948,251 @@
         if ans == '' and default is not None:
             return valid_input[default]
 
         if ans in valid_input.keys():
             return valid_input[ans]
 
 
-def get_colour(name):
-    """
-    Get a nice standard colour.
-    """
-
-    if(name == "darkred" or name == "dr"):
+def get_color(name):
+    """Get RGBA values for standard colors."""
+    if name == "darkred" or name == "dr":
         return hex2byte("e94040ff")/255
 
-    if(name == "red" or name == "r"):
+    if name == "red" or name == "r":
         return hex2byte("ffb9b9ff")/255
 
-    if(name == "lightred" or name == "lr"):
+    if name == "lightred" or name == "lr":
         return hex2byte("fad1d1ff")/255
 
-    if(name == "darkgreen" or name == "dg"):
+    if name == "darkgreen" or name == "dg":
         return hex2byte("52b656ff")/255
 
-    if(name == "green" or name == "g"):
+    if name == "green" or name == "g":
         return hex2byte("a0e4a1ff")/255
 
-    if(name == "lightgreen" or name == "lg"):
+    if name == "lightgreen" or name == "lg":
         return hex2byte("d9f2d9ff")/255
 
-    if(name == "darkblue" or name == "db"):
+    if name == "darkblue" or name == "db":
         return hex2byte("458ddeff")/255
 
-    if(name == "blue" or name == "b"):
+    if name == "blue" or name == "b":
         return hex2byte("97b9f7ff")/255
 
-    if(name == "darkorange" or name == "do"):
+    if name == "darkorange" or name == "do":
         return hex2byte("ee8e4aff")/255
 
-    if(name == "yellow" or name == "y"):
+    if name == "yellow" or name == "y":
         return hex2byte("ffea97ff")/255
 
-    if(name == "lightgray" or name == "lgr"):
+    if name == "lightgray" or name == "lgr":
         return [230/255, 230/255, 230/255]
 
-    if(name == "gray" or name == "gr"):
+    if name == "gray" or name == "gr":
         return [0.5, 0.5, 0.5]
 
-    if(name == "black" or name == "k"):
+    if name == "black" or name == "k":
         return [0, 0, 0]
 
     # Vega/D3 Category20
-    if(name == "C20_0"):
+    if name == "C20_0":
         return [0.1216, 0.4667, 0.7059]  # 1f77b4
 
-    if(name == "C20_1"):
+    if name == "C20_1":
         return [0.6824, 0.7804, 0.9098]  # aec7e8
 
-    if(name == "C20_2"):
+    if name == "C20_2":
         return [1.0000, 0.4980, 0.0549]  # ff7f0e
 
-    if(name == "C20_3"):
+    if name == "C20_3":
         return [1.0000, 0.7333, 0.4706]  # ffbb78
 
-    if(name == "C20_4"):
+    if name == "C20_4":
         return [0.1725, 0.6275, 0.1725]  # 2ca02c
 
-    if(name == "C20_5"):
+    if name == "C20_5":
         return [0.5961, 0.8745, 0.5412]  # 98df8a
 
-    if(name == "C20_6"):
+    if name == "C20_6":
         return [0.8392, 0.1529, 0.1569]  # d62728
 
-    if(name == "C20_7"):
+    if name == "C20_7":
         return [1.0000, 0.5961, 0.5882]  # ff9896
 
-    if(name == "C20_8"):
+    if name == "C20_8":
         return [0.5804, 0.4039, 0.7412]  # 9467bd
 
-    if(name == "C20_9"):
+    if name == "C20_9":
         return [0.7725, 0.6902, 0.8353]  # c5b0d5
 
-    if(name == "C20_10"):
+    if name == "C20_10":
         return [0.5490, 0.3373, 0.2941]  # 8c564b
 
-    if(name == "C20_11"):
+    if name == "C20_11":
         return [0.7686, 0.6118, 0.5804]  # c49c94
 
-    if(name == "C20_12"):
+    if name == "C20_12":
         return [0.8902, 0.4667, 0.7608]  # e377c2
 
-    if(name == "C20_13"):
+    if name == "C20_13":
         return [0.9686, 0.7137, 0.8235]  # f7b6d2
 
-    if(name == "C20_14"):
+    if name == "C20_14":
         return [0.4980, 0.4980, 0.4980]  # 7f7f7f
 
-    if(name == "C20_15"):
+    if name == "C20_15":
         return [0.7804, 0.7804, 0.7804]  # c7c7c7
 
-    if(name == "C20_16"):
+    if name == "C20_16":
         return [0.7373, 0.7412, 0.1333]  # bcbd22
 
-    if(name == "C20_17"):
+    if name == "C20_17":
         return [0.8588, 0.8588, 0.5529]  # dbdb8d
 
-    if(name == "C20_18"):
+    if name == "C20_18":
         return [0.0902, 0.7451, 0.8118]  # 17becf
 
-    if(name == "C20_19"):
+    if name == "C20_19":
         return [0.6196, 0.8549, 0.8980]  # 9edae5
 
     # Vega/D3 Category20b
-    if(name == "C20b_0"):
+    if name == "C20b_0":
         return [0.2235, 0.2314, 0.4745]  # 393b79
 
-    if(name == "C20b_1"):
+    if name == "C20b_1":
         return [0.3216, 0.3294, 0.6392]  # 5254a3
 
-    if(name == "C20b_2"):
+    if name == "C20b_2":
         return [0.4196, 0.4314, 0.8118]  # 6b6ecf
 
-    if(name == "C20b_3"):
+    if name == "C20b_3":
         return [0.6118, 0.6196, 0.8706]  # 9c9ede
 
-    if(name == "C20b_4"):
+    if name == "C20b_4":
         return [0.3882, 0.4745, 0.2235]  # 637939
 
-    if(name == "C20b_5"):
+    if name == "C20b_5":
         return [0.5490, 0.6353, 0.3216]  # 8ca252
 
-    if(name == "C20b_6"):
+    if name == "C20b_6":
         return [0.7098, 0.8118, 0.4196]  # b5cf6b
 
-    if(name == "C20b_7"):
+    if name == "C20b_7":
         return [0.8078, 0.8588, 0.6118]  # cedb9c
 
-    if(name == "C20b_8"):
+    if name == "C20b_8":
         return [0.5490, 0.4275, 0.1922]  # 8c6d31
 
-    if(name == "C20b_9"):
+    if name == "C20b_9":
         return [0.7412, 0.6196, 0.2235]  # bd9e39
 
-    if(name == "C20b_10"):
+    if name == "C20b_10":
         return [0.9059, 0.7294, 0.3216]  # e7ba52
 
-    if(name == "C20b_11"):
+    if name == "C20b_11":
         return [0.9059, 0.7961, 0.5804]  # e7cb94
 
-    if(name == "C20b_12"):
+    if name == "C20b_12":
         return [0.5176, 0.2353, 0.2235]  # 843c39
 
-    if(name == "C20b_13"):
+    if name == "C20b_13":
         return [0.6784, 0.2863, 0.2902]  # ad494a
 
-    if(name == "C20b_14"):
+    if name == "C20b_14":
         return [0.8392, 0.3804, 0.4196]  # d6616b
 
-    if(name == "C20b_15"):
+    if name == "C20b_15":
         return [0.9059, 0.5882, 0.6118]  # e7969c
 
-    if(name == "C20b_16"):
+    if name == "C20b_16":
         return [0.4824, 0.2549, 0.4510]  # 7b4173
 
-    if(name == "C20b_17"):
+    if name == "C20b_17":
         return [0.6471, 0.3176, 0.5804]  # a55194
 
-    if(name == "C20b_18"):
+    if name == "C20b_18":
         return [0.8078, 0.4275, 0.7412]  # ce6dbd
 
-    if(name == "C20b_19"):
+    if name == "C20b_19":
         return [0.8706, 0.6196, 0.8392]  # de9ed6
 
     print("Undefined colour '" + name + "'")
     return get_colour("gray")
 
 
-def get_color(name):
-    return get_colour(name)
+def get_colour(name):
+    """British wrapper for get_color()."""
+    return get_color(name)
 
 
 def get_color_seq(names=None, seq_name='Vega20'):
-    """
-    Get a color sequence for indexing.
-    """
+    """Get a color sequence for indexing."""
     if not seq_name:
         seq_name = 'rgb'
 
     if seq_name == 'rgb':
         names = ['dr', 'dg', 'db', 'r', 'g', 'b']
+    elif seq_name == 'Vega10':
+        names = []
+        for ind in np.arange(1, 10):
+            names.append('C10_{:d}'.format(ind))
     elif seq_name == 'Vega20b':
         names = []
-        for ind in np.arange(2, 20, 2):
+        for ind in np.arange(0, 20, 2):
             names.append('C20b_{:d}'.format(ind))
     elif seq_name == 'Vega20':
         names = []
-        for ind in np.arange(2, 20, 2):
+        for ind in np.arange(0, 20, 2):
             names.append('C20_{:d}'.format(ind))
 
     c = []
     for name in names:
         c.append(get_color(name))
 
     return c
 
 
 def get_colourmap(name):
-    """Get one of the default colourmaps by its name."""
-
-    if(name == "KBW_Nice"):
+    """Get a custom colourmap."""
+    if name == "KBW_Nice":
         colors = [(0, 0, 0), (151/255, 185/255, 247/255), (1, 1, 1)]
         return LinearSegmentedColormap.from_list(
                 name, colors, N=256)
 
-    if(name == "KPW_Nice"):
+    if name == "KPW_Nice":
         colors = [(0, 0, 0), (190/255, 70/255, 196/255), (1, 1, 1)]
         return LinearSegmentedColormap.from_list(
                 name, colors, N=256)
 
-    if(name == "KGW_Nice"):
+    if name == "KGW_Nice":
         colors = [(0, 0, 0), (160/255, 255/255, 161/255), (1, 1, 1)]
         return LinearSegmentedColormap.from_list(
                 name, colors, N=256)
 
-    if(name == "KOW_Nice"):
+    if name == "KOW_Nice":
         colors = [(0, 0, 0), (255/255, 180/255, 128/255), (1, 1, 1)]
         return LinearSegmentedColormap.from_list(
                 name, colors, N=256)
 
-    if(name == "KRW_Nice"):
+    if name == "KRW_Nice":
         colors = [(0, 0, 0), (233/255, 64/255, 64/255), (1, 1, 1)]
         return LinearSegmentedColormap.from_list(
                 name, colors, N=256)
 
-    if(name == "GYOR_Nice"):
+    if name == "GYOR_Nice":
         colors = [(0.0, (130/255, 220/255, 132/255)),
                   (0.25, (130/255, 220/255, 132/255)),
                   (0.5, (255/255, 234/255, 151/255)),
                   (0.75, (255/255, 180/255, 128/255)),
                   (1.0, (255/255, 180/255, 185/255))]
 
         return LinearSegmentedColormap.from_list(
                 name, colors, N=256)
 
-    if(name == 'gray_sat'):
+    if name == 'gray_sat':
         cm = get_cmap('gray')
         cm.set_over('r')
         cm.set_under('b')
 
         return cm
 
     return get_cmap(name)
```

### Comparing `lkcom-0.3.1/lkcom.egg-info/PKG-INFO` & `lkcom-0.3.2/lkcom.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lkcom
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Python library of useful routines.
 Home-page: https://bitbucket.org/lukaskontenis/lkcom/
 Author: Lukas Kontenis
 Author-email: dse.ssd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lkcom-0.3.1/setup.py` & `lkcom-0.3.2/setup.py`

 * *Files identical despite different names*

