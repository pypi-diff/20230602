# Comparing `tmp/brunospackage-0.0.5.tar.gz` & `tmp/brunospackage-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brunospackage-0.0.5.tar", last modified: Fri Jun  2 04:58:12 2023, max compression
+gzip compressed data, was "brunospackage-0.0.6.tar", last modified: Fri Jun  2 04:59:36 2023, max compression
```

## Comparing `brunospackage-0.0.5.tar` & `brunospackage-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 bdtacchi   (501) staff       (20)        0 2023-06-02 04:58:12.799708 brunospackage-0.0.5/
--rw-r--r--   0 bdtacchi   (501) staff       (20)      540 2023-06-02 04:58:12.799587 brunospackage-0.0.5/PKG-INFO
-drwxr-xr-x   0 bdtacchi   (501) staff       (20)        0 2023-06-02 04:58:12.798639 brunospackage-0.0.5/brunospackage/
--rw-r--r--   0 bdtacchi   (501) staff       (20)       52 2023-06-02 04:36:45.000000 brunospackage-0.0.5/brunospackage/__init__.py
--rw-r--r--   0 bdtacchi   (501) staff       (20)     2482 2023-06-02 04:54:33.000000 brunospackage-0.0.5/brunospackage/functions.py
-drwxr-xr-x   0 bdtacchi   (501) staff       (20)        0 2023-06-02 04:58:12.799396 brunospackage-0.0.5/brunospackage.egg-info/
--rw-r--r--   0 bdtacchi   (501) staff       (20)      540 2023-06-02 04:58:12.000000 brunospackage-0.0.5/brunospackage.egg-info/PKG-INFO
--rw-r--r--   0 bdtacchi   (501) staff       (20)      245 2023-06-02 04:58:12.000000 brunospackage-0.0.5/brunospackage.egg-info/SOURCES.txt
--rw-r--r--   0 bdtacchi   (501) staff       (20)        1 2023-06-02 04:58:12.000000 brunospackage-0.0.5/brunospackage.egg-info/dependency_links.txt
--rw-r--r--   0 bdtacchi   (501) staff       (20)       18 2023-06-02 04:58:12.000000 brunospackage-0.0.5/brunospackage.egg-info/requires.txt
--rw-r--r--   0 bdtacchi   (501) staff       (20)       14 2023-06-02 04:58:12.000000 brunospackage-0.0.5/brunospackage.egg-info/top_level.txt
--rw-r--r--   0 bdtacchi   (501) staff       (20)       38 2023-06-02 04:58:12.799764 brunospackage-0.0.5/setup.cfg
--rw-r--r--   0 bdtacchi   (501) staff       (20)     1630 2023-06-02 04:58:08.000000 brunospackage-0.0.5/setup.py
+drwxr-xr-x   0 bdtacchi   (501) staff       (20)        0 2023-06-02 04:59:36.519449 brunospackage-0.0.6/
+-rw-r--r--   0 bdtacchi   (501) staff       (20)      540 2023-06-02 04:59:36.519343 brunospackage-0.0.6/PKG-INFO
+drwxr-xr-x   0 bdtacchi   (501) staff       (20)        0 2023-06-02 04:59:36.518513 brunospackage-0.0.6/brunospackage/
+-rw-r--r--   0 bdtacchi   (501) staff       (20)       52 2023-06-02 04:36:45.000000 brunospackage-0.0.6/brunospackage/__init__.py
+-rw-r--r--   0 bdtacchi   (501) staff       (20)     2522 2023-06-02 04:59:15.000000 brunospackage-0.0.6/brunospackage/functions.py
+drwxr-xr-x   0 bdtacchi   (501) staff       (20)        0 2023-06-02 04:59:36.519163 brunospackage-0.0.6/brunospackage.egg-info/
+-rw-r--r--   0 bdtacchi   (501) staff       (20)      540 2023-06-02 04:59:36.000000 brunospackage-0.0.6/brunospackage.egg-info/PKG-INFO
+-rw-r--r--   0 bdtacchi   (501) staff       (20)      245 2023-06-02 04:59:36.000000 brunospackage-0.0.6/brunospackage.egg-info/SOURCES.txt
+-rw-r--r--   0 bdtacchi   (501) staff       (20)        1 2023-06-02 04:59:36.000000 brunospackage-0.0.6/brunospackage.egg-info/dependency_links.txt
+-rw-r--r--   0 bdtacchi   (501) staff       (20)       18 2023-06-02 04:59:36.000000 brunospackage-0.0.6/brunospackage.egg-info/requires.txt
+-rw-r--r--   0 bdtacchi   (501) staff       (20)       14 2023-06-02 04:59:36.000000 brunospackage-0.0.6/brunospackage.egg-info/top_level.txt
+-rw-r--r--   0 bdtacchi   (501) staff       (20)       38 2023-06-02 04:59:36.519494 brunospackage-0.0.6/setup.cfg
+-rw-r--r--   0 bdtacchi   (501) staff       (20)     1630 2023-06-02 04:59:32.000000 brunospackage-0.0.6/setup.py
```

### Comparing `brunospackage-0.0.5/PKG-INFO` & `brunospackage-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brunospackage
-Version: 0.0.5
+Version: 0.0.6
 Summary: Helper functions that I use often
 Author: Bruno Tacchi
 Author-email: bruno_tacchi@hotmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `brunospackage-0.0.5/brunospackage/functions.py` & `brunospackage-0.0.6/brunospackage/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
             match = re.search(self.unit_pattern, column_name)
             if match:
                 ax.set_ylabel(match.group(1))  # Group 1 should be the units
             # Remove units from column name
             column_name = re.sub(self.unit_pattern, '', column_name)
 
         ax.set_title(column_name)
+        ax.set_xlabel(self.time_column)
         self.canvas.draw()
 
     def next_plot(self):
         self.current_column_index = (self.current_column_index + 1) % len(self.columns)
         self.plot_current_column()
 
     def previous_plot(self):
```

### Comparing `brunospackage-0.0.5/brunospackage.egg-info/PKG-INFO` & `brunospackage-0.0.6/brunospackage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brunospackage
-Version: 0.0.5
+Version: 0.0.6
 Summary: Helper functions that I use often
 Author: Bruno Tacchi
 Author-email: bruno_tacchi@hotmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `brunospackage-0.0.5/setup.py` & `brunospackage-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.5' 
+VERSION = '0.0.6' 
 DESCRIPTION = 'Helper functions that I use often'
 LONG_DESCRIPTION = '''A package that allows me to import functions that I use often.'''
 # DataFramePlotter - given a dataframe with multiple variables, plots each variable against time in a tkinter window. Requires pandas, matplotlib, tkinter, and re. The usage is: 
 #     import brunospackage as bp
 #     plotter = bp.DataFramePlotter(df, nameOfTimeColumn, unit_format)
 #     plotter.run()'''
```

