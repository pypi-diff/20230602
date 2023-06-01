# Comparing `tmp/ic50-0.0.99.2.tar.gz` & `tmp/ic50-0.0.99.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ic50-0.0.99.2.tar", last modified: Thu Jun  1 22:30:09 2023, max compression
+gzip compressed data, was "ic50-0.0.99.3.tar", last modified: Thu Jun  1 22:39:53 2023, max compression
```

## Comparing `ic50-0.0.99.2.tar` & `ic50-0.0.99.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 niux10     (501) staff       (20)        0 2023-06-01 22:30:09.168293 ic50-0.0.99.2/
--rw-r--r--   0 niux10     (501) staff       (20)      497 2023-06-01 22:30:09.168153 ic50-0.0.99.2/PKG-INFO
-drwxr-xr-x   0 niux10     (501) staff       (20)        0 2023-06-01 22:30:09.167194 ic50-0.0.99.2/ic50/
--rw-r--r--   0 niux10     (501) staff       (20)       19 2023-06-01 18:16:47.000000 ic50-0.0.99.2/ic50/__init__.py
--rw-r--r--   0 niux10     (501) staff       (20)    15262 2023-06-01 22:28:31.000000 ic50-0.0.99.2/ic50/ic50.py
-drwxr-xr-x   0 niux10     (501) staff       (20)        0 2023-06-01 22:30:09.167958 ic50-0.0.99.2/ic50.egg-info/
--rw-r--r--   0 niux10     (501) staff       (20)      497 2023-06-01 22:30:09.000000 ic50-0.0.99.2/ic50.egg-info/PKG-INFO
--rw-r--r--   0 niux10     (501) staff       (20)      177 2023-06-01 22:30:09.000000 ic50-0.0.99.2/ic50.egg-info/SOURCES.txt
--rw-r--r--   0 niux10     (501) staff       (20)        1 2023-06-01 22:30:09.000000 ic50-0.0.99.2/ic50.egg-info/dependency_links.txt
--rw-r--r--   0 niux10     (501) staff       (20)       23 2023-06-01 22:30:09.000000 ic50-0.0.99.2/ic50.egg-info/requires.txt
--rw-r--r--   0 niux10     (501) staff       (20)        5 2023-06-01 22:30:09.000000 ic50-0.0.99.2/ic50.egg-info/top_level.txt
--rw-r--r--   0 niux10     (501) staff       (20)       38 2023-06-01 22:30:09.168343 ic50-0.0.99.2/setup.cfg
--rw-r--r--   0 niux10     (501) staff       (20)      852 2023-06-01 22:24:12.000000 ic50-0.0.99.2/setup.py
+drwxr-xr-x   0 niux10     (501) staff       (20)        0 2023-06-01 22:39:53.198210 ic50-0.0.99.3/
+-rw-r--r--   0 niux10     (501) staff       (20)      497 2023-06-01 22:39:53.198068 ic50-0.0.99.3/PKG-INFO
+drwxr-xr-x   0 niux10     (501) staff       (20)        0 2023-06-01 22:39:53.196680 ic50-0.0.99.3/ic50/
+-rw-r--r--   0 niux10     (501) staff       (20)       19 2023-06-01 18:16:47.000000 ic50-0.0.99.3/ic50/__init__.py
+-rw-r--r--   0 niux10     (501) staff       (20)    15266 2023-06-01 22:39:22.000000 ic50-0.0.99.3/ic50/ic50.py
+drwxr-xr-x   0 niux10     (501) staff       (20)        0 2023-06-01 22:39:53.197870 ic50-0.0.99.3/ic50.egg-info/
+-rw-r--r--   0 niux10     (501) staff       (20)      497 2023-06-01 22:39:53.000000 ic50-0.0.99.3/ic50.egg-info/PKG-INFO
+-rw-r--r--   0 niux10     (501) staff       (20)      177 2023-06-01 22:39:53.000000 ic50-0.0.99.3/ic50.egg-info/SOURCES.txt
+-rw-r--r--   0 niux10     (501) staff       (20)        1 2023-06-01 22:39:53.000000 ic50-0.0.99.3/ic50.egg-info/dependency_links.txt
+-rw-r--r--   0 niux10     (501) staff       (20)       23 2023-06-01 22:39:53.000000 ic50-0.0.99.3/ic50.egg-info/requires.txt
+-rw-r--r--   0 niux10     (501) staff       (20)        5 2023-06-01 22:39:53.000000 ic50-0.0.99.3/ic50.egg-info/top_level.txt
+-rw-r--r--   0 niux10     (501) staff       (20)       38 2023-06-01 22:39:53.198258 ic50-0.0.99.3/setup.cfg
+-rw-r--r--   0 niux10     (501) staff       (20)      852 2023-06-01 22:39:34.000000 ic50-0.0.99.3/setup.py
```

### Comparing `ic50-0.0.99.2/ic50/ic50.py` & `ic50-0.0.99.3/ic50/ic50.py`

 * *Files 0% similar despite different names*

```diff
@@ -420,15 +420,15 @@
         responses = self.predict_response(concentrations)
     
         plt.figure()
         plt.scatter(10**self.concentrations, self.responses*100, color='blue', label='Data')
         plt.plot(10**concentrations, responses*100, color='red', label='Fitted Curve')
         plt.axvline(x=10**-self.ic50, color='green', linestyle='--', label='IC50')
         plt.xlabel('Concentration (log10)')
-        plt.ylabel('Response')
+        plt.ylabel('Response (%)')
         plt.title('Data and Fitted Curve with IC50')
         plt.xscale('log',base=10) 
         plt.legend()
         plt.show()
         
         return None
```

### Comparing `ic50-0.0.99.2/setup.py` & `ic50-0.0.99.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.99.2' 
+VERSION = '0.0.99.3' 
 DESCRIPTION = 'IC50 prediction'
 LONG_DESCRIPTION = 'Calculate IC50/pIC50 values using a variety of methods.'
 
 setup(
         name="ic50", 
         version=VERSION,
         author="Steve Niu",
```

