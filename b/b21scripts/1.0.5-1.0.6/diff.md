# Comparing `tmp/b21scripts-1.0.5.tar.gz` & `tmp/b21scripts-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/dls/science/groups/b21/PYTHON3/packages/b21scripts/dist/.tmp-pn6ft4hd/b21scripts-1.0.5.tar", last modified: Tue Feb 28 16:12:28 2023, max compression
+gzip compressed data, was "/Users/nathan/Documents/PYTHON/b21scripts/dist/.tmp-_qn04csr/b21scripts-1.0.6.tar", last modified: Fri Jun  2 09:21:38 2023, max compression
```

## Comparing `b21scripts-1.0.5.tar` & `b21scripts-1.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwsr-x   0 xaf46449 (1207847) b21_staff (37577)        0 2023-02-28 16:12:28.000000 b21scripts-1.0.5/
--rw-rw-r--   0 xaf46449 (1207847) b21_staff (37577)     1084 2023-01-31 10:29:54.000000 b21scripts-1.0.5/LICENCE
--rw-rw-r--   0 xaf46449 (1207847) b21_staff (37577)     2445 2023-02-28 16:12:28.000000 b21scripts-1.0.5/PKG-INFO
--rw-rw-r--   0 xaf46449 (1207847) b21_staff (37577)     1903 2023-01-31 10:29:54.000000 b21scripts-1.0.5/README.md
--rw-rw-r--   0 xaf46449 (1207847) b21_staff (37577)       84 2023-01-31 10:29:54.000000 b21scripts-1.0.5/pyproject.toml
--rw-rw-r--   0 xaf46449 (1207847) b21_staff (37577)      735 2023-02-28 16:12:28.000000 b21scripts-1.0.5/setup.cfg
-drwxrwsr-x   0 xaf46449 (1207847) b21_staff (37577)        0 2023-02-28 16:12:28.000000 b21scripts-1.0.5/src/
-drwxrwsr-x   0 xaf46449 (1207847) b21_staff (37577)        0 2023-02-28 16:12:28.000000 b21scripts-1.0.5/src/b21scripts/
--rw-rw-r--   0 xaf46449 (1207847) b21_staff (37577)        0 2023-01-31 10:29:54.000000 b21scripts-1.0.5/src/b21scripts/__init__.py
-drwxrwsr-x   0 xaf46449 (1207847) b21_staff (37577)        0 2023-02-28 16:12:28.000000 b21scripts-1.0.5/src/b21scripts/readwrite/
--rw-rw-r--   0 xaf46449 (1207847) b21_staff (37577)        0 2023-01-31 10:29:54.000000 b21scripts-1.0.5/src/b21scripts/readwrite/__init__.py
--rw-rw-r--   0 xaf46449 (1207847) b21_staff (37577)     6146 2023-02-28 15:13:24.000000 b21scripts-1.0.5/src/b21scripts/readwrite/dat.py
--rw-rw-r--   0 xaf46449 (1207847) b21_staff (37577)      395 2023-01-31 10:29:54.000000 b21scripts-1.0.5/src/b21scripts/readwrite/interface.py
--rw-rw-r--   0 xaf46449 (1207847) b21_staff (37577)    13786 2023-01-31 10:29:54.000000 b21scripts-1.0.5/src/b21scripts/readwrite/pdb.py
-drwxrwsr-x   0 xaf46449 (1207847) b21_staff (37577)        0 2023-02-28 16:12:28.000000 b21scripts-1.0.5/src/b21scripts/saxs/
--rw-rw-r--   0 xaf46449 (1207847) b21_staff (37577)        0 2023-01-31 10:29:54.000000 b21scripts-1.0.5/src/b21scripts/saxs/__init__.py
--rwxrwxr-x   0 xaf46449 (1207847) b21_staff (37577)    11290 2023-01-31 10:29:54.000000 b21scripts-1.0.5/src/b21scripts/saxs/saxs_calc.py
-drwxrwsr-x   0 xaf46449 (1207847) b21_staff (37577)        0 2023-02-28 16:12:28.000000 b21scripts-1.0.5/src/b21scripts.egg-info/
--rw-rw-r--   0 xaf46449 (1207847) b21_staff (37577)     2445 2023-02-28 16:12:28.000000 b21scripts-1.0.5/src/b21scripts.egg-info/PKG-INFO
--rw-rw-r--   0 xaf46449 (1207847) b21_staff (37577)      462 2023-02-28 16:12:28.000000 b21scripts-1.0.5/src/b21scripts.egg-info/SOURCES.txt
--rw-rw-r--   0 xaf46449 (1207847) b21_staff (37577)        1 2023-02-28 16:12:28.000000 b21scripts-1.0.5/src/b21scripts.egg-info/dependency_links.txt
--rw-rw-r--   0 xaf46449 (1207847) b21_staff (37577)        6 2023-02-28 16:12:28.000000 b21scripts-1.0.5/src/b21scripts.egg-info/requires.txt
--rw-rw-r--   0 xaf46449 (1207847) b21_staff (37577)       11 2023-02-28 16:12:28.000000 b21scripts-1.0.5/src/b21scripts.egg-info/top_level.txt
+drwxr-xr-x   0 nathan     (503) staff       (20)        0 2023-06-02 09:21:38.000000 b21scripts-1.0.6/
+-rw-r--r--   0 nathan     (503) staff       (20)     1084 2022-09-09 14:05:16.000000 b21scripts-1.0.6/LICENCE
+-rw-r--r--   0 nathan     (503) staff       (20)     2445 2023-06-02 09:21:38.000000 b21scripts-1.0.6/PKG-INFO
+-rw-r--r--   0 nathan     (503) staff       (20)     1903 2022-09-19 18:19:39.000000 b21scripts-1.0.6/README.md
+-rw-r--r--   0 nathan     (503) staff       (20)       84 2022-09-09 14:05:16.000000 b21scripts-1.0.6/pyproject.toml
+-rw-r--r--   0 nathan     (503) staff       (20)      747 2023-06-02 09:21:38.000000 b21scripts-1.0.6/setup.cfg
+drwxr-xr-x   0 nathan     (503) staff       (20)        0 2023-06-02 09:21:38.000000 b21scripts-1.0.6/src/
+drwxr-xr-x   0 nathan     (503) staff       (20)        0 2023-06-02 09:21:38.000000 b21scripts-1.0.6/src/b21scripts/
+-rw-r--r--   0 nathan     (503) staff       (20)        0 2022-09-09 14:05:16.000000 b21scripts-1.0.6/src/b21scripts/__init__.py
+drwxr-xr-x   0 nathan     (503) staff       (20)        0 2023-06-02 09:21:38.000000 b21scripts-1.0.6/src/b21scripts/readwrite/
+-rw-r--r--   0 nathan     (503) staff       (20)        0 2022-09-09 14:05:16.000000 b21scripts-1.0.6/src/b21scripts/readwrite/__init__.py
+-rw-r--r--   0 nathan     (503) staff       (20)     7517 2023-06-02 09:16:26.000000 b21scripts-1.0.6/src/b21scripts/readwrite/dat.py
+-rw-r--r--   0 nathan     (503) staff       (20)      395 2022-09-09 14:05:16.000000 b21scripts-1.0.6/src/b21scripts/readwrite/interface.py
+-rw-r--r--   0 nathan     (503) staff       (20)    13786 2022-09-09 14:05:16.000000 b21scripts-1.0.6/src/b21scripts/readwrite/pdb.py
+drwxr-xr-x   0 nathan     (503) staff       (20)        0 2023-06-02 09:21:38.000000 b21scripts-1.0.6/src/b21scripts/saxs/
+-rw-r--r--   0 nathan     (503) staff       (20)        0 2022-09-19 18:10:28.000000 b21scripts-1.0.6/src/b21scripts/saxs/__init__.py
+-rwxr-xr-x   0 nathan     (503) staff       (20)    11290 2022-09-19 16:24:23.000000 b21scripts-1.0.6/src/b21scripts/saxs/saxs_calc.py
+drwxr-xr-x   0 nathan     (503) staff       (20)        0 2023-06-02 09:21:38.000000 b21scripts-1.0.6/src/b21scripts.egg-info/
+-rw-r--r--   0 nathan     (503) staff       (20)     2445 2023-06-02 09:21:38.000000 b21scripts-1.0.6/src/b21scripts.egg-info/PKG-INFO
+-rw-r--r--   0 nathan     (503) staff       (20)      462 2023-06-02 09:21:38.000000 b21scripts-1.0.6/src/b21scripts.egg-info/SOURCES.txt
+-rw-r--r--   0 nathan     (503) staff       (20)        1 2023-06-02 09:21:38.000000 b21scripts-1.0.6/src/b21scripts.egg-info/dependency_links.txt
+-rw-r--r--   0 nathan     (503) staff       (20)       17 2023-06-02 09:21:38.000000 b21scripts-1.0.6/src/b21scripts.egg-info/requires.txt
+-rw-r--r--   0 nathan     (503) staff       (20)       11 2023-06-02 09:21:38.000000 b21scripts-1.0.6/src/b21scripts.egg-info/top_level.txt
```

### Comparing `b21scripts-1.0.5/LICENCE` & `b21scripts-1.0.6/LICENCE`

 * *Files identical despite different names*

### Comparing `b21scripts-1.0.5/PKG-INFO` & `b21scripts-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: b21scripts
-Version: 1.0.5
+Version: 1.0.6
 Summary: Libraries for SAXS data manipulation and analysis
 Home-page: https://github.com/nathancowieson/b21scripts.git
 Author: Nathan Cowieson
 Author-email: nathan.cowieson@diamond.ac.uk
 Project-URL: Bug Tracker, https://github.com/pypa/b21scripts/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `b21scripts-1.0.5/README.md` & `b21scripts-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `b21scripts-1.0.5/setup.cfg` & `b21scripts-1.0.6/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = b21scripts
-version = 1.0.5
+version = 1.0.6
 author = Nathan Cowieson
 author_email = nathan.cowieson@diamond.ac.uk
 description = Libraries for SAXS data manipulation and analysis
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nathancowieson/b21scripts.git
 project_urls = 
@@ -17,14 +17,15 @@
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	numpy
+	matplotlib
 
 [build-system]
 requires = ["setuptools"]
 
 [options.packages.find]
 where = src
```

### Comparing `b21scripts-1.0.5/src/b21scripts/readwrite/dat.py` & `b21scripts-1.0.6/src/b21scripts/readwrite/dat.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,32 +23,38 @@
         streamhandler = logging.StreamHandler()
         streamhandler.setFormatter(formatter)
         if len(self.logger.handlers) == 0:
             self.logger.addHandler(streamhandler)
             self.logger.info('Starting a new readwrite.DAT job')        
         self.type = 'dat'
         self.is_outlier = False
-        if hasattr(self, 'datfile'):
-            if os.path.isfile(datfile) and datfile[-4:] == '.dat':
-                self.datfile = datfile
-            else:
-                self.datfile = None
-                self.logger.info('No datfile was specified, will instantiate with an empty array')
-        else:
-            self.datfile = None
-            self.logger.info('No datfile was specified, will instantiate with an empty array')
 
         self.hashdata = {'Q': [], 'I': [], 'E': []}
         self.high_q_window_range = (0.68,0.79)
         self.low_q_window_range = (0.02,0.05)
         self.low_q_window = 0
         self.high_q_window = 0
         if self.datfile:
             self.parse_file()
 
+    def set_datfile(self, datfile):
+        '''Set the datfile'''
+        if datfile == None:
+            self.logger.info('No dat file provided, instantiating with empty data array')
+            self.datfile = None
+            return False
+        elif os.path.isfile(datfile) and str(datfile)[-4:] == '.dat':
+            self.datfile = str(datfile)
+            self.logger.info(f'{datfile} lookks like a valid datfile')
+            return True
+        else:
+            self.datfile = None
+            self.logger.error(f'{datfile} either does not exist or is not of type ".dat"')
+            return False
+            
     def parse_file(self):
         self.logger.info(f'Reading and parsing dat file: {self.datfile}')
         qdata = []
         idata = []
         edata = []
         
         datafile = open(self.datfile, "r")
@@ -142,25 +148,59 @@
              log_x=False,
              linewidth=2,
              height=8,
              width=15,
              fontsize=16,
              title=None,
              x_label=r'Q ($\AA^{-1}$)',
-             y_label=r'Intensity (cm$^{-1}$)'
+             y_label=r'Intensity (cm$^{-1}$)',
+             qrange_min=None,
+             qrange_max=None,
+             filename=None,
+             label='',
+             show=True
              ):
         '''Use pyplt to graph the dat data'''
+        min_index = 0
+        max_index = len(self.hashdata['Q'])-1
+        if qrange_min:
+            try:
+                qrange_min = float(qrange_min)
+                for i, q in enumerate(self.hashdata['Q']):
+                    if q<qrange_min:
+                        min_index = i
+                    else:
+                        break
+            except:
+                self.logger.error('qrange_min parameter for plot function should be a number')
+
+        if qrange_max:
+            try:
+                qrange_min = float(qrange_min)
+                for i, q in enumerate(self.hashdata['Q']):
+                    if q>qrange_max:
+                        max_index = i
+                        break
+            except:
+                self.logger.error('1qrange_max parameter for plot function should be a number')
+        if not show:
+            plt.ioff()
         plt.rc('xtick',labelsize=fontsize-2)
         plt.rc('ytick',labelsize=fontsize-2)
         fig, ax = plt.subplots()
         fig.set_figwidth(width)
         fig.set_figheight(height)
         if log_y:
             plt.yscale('log')
         if log_x:
             plt.xscale('log')
         if title:
             ax.set_title(f'{title}', fontsize=fontsize)
         plt.rc('lines', linewidth=linewidth)
         ax.set_ylabel(y_label, fontsize=fontsize)
         ax.set_xlabel(x_label, fontsize=fontsize)
-        plt.plot(self.hashdata['Q'],self.hashdata['I'])
+        plt.plot(self.hashdata['Q'][min_index:max_index],self.hashdata['I'][min_index:max_index])
+        plt.title(f'{label}')
+        if filename:
+            plt.savefig(f'{filename}')
+        if not show:
+            plt.close(fig)
```

### Comparing `b21scripts-1.0.5/src/b21scripts/readwrite/pdb.py` & `b21scripts-1.0.6/src/b21scripts/readwrite/pdb.py`

 * *Files identical despite different names*

### Comparing `b21scripts-1.0.5/src/b21scripts/saxs/saxs_calc.py` & `b21scripts-1.0.6/src/b21scripts/saxs/saxs_calc.py`

 * *Files identical despite different names*

### Comparing `b21scripts-1.0.5/src/b21scripts.egg-info/PKG-INFO` & `b21scripts-1.0.6/src/b21scripts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: b21scripts
-Version: 1.0.5
+Version: 1.0.6
 Summary: Libraries for SAXS data manipulation and analysis
 Home-page: https://github.com/nathancowieson/b21scripts.git
 Author: Nathan Cowieson
 Author-email: nathan.cowieson@diamond.ac.uk
 Project-URL: Bug Tracker, https://github.com/pypa/b21scripts/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

