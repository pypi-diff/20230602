# Comparing `tmp/ic50-0.0.99.1.tar.gz` & `tmp/ic50-0.0.99.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ic50-0.0.99.1.tar", last modified: Thu Jun  1 21:38:34 2023, max compression
+gzip compressed data, was "ic50-0.0.99.2.tar", last modified: Thu Jun  1 22:30:09 2023, max compression
```

## Comparing `ic50-0.0.99.1.tar` & `ic50-0.0.99.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 niux10     (501) staff       (20)        0 2023-06-01 21:38:34.301465 ic50-0.0.99.1/
--rw-r--r--   0 niux10     (501) staff       (20)      491 2023-06-01 21:38:34.301309 ic50-0.0.99.1/PKG-INFO
-drwxr-xr-x   0 niux10     (501) staff       (20)        0 2023-06-01 21:38:34.300171 ic50-0.0.99.1/ic50/
--rw-r--r--   0 niux10     (501) staff       (20)       19 2023-06-01 18:16:47.000000 ic50-0.0.99.1/ic50/__init__.py
--rw-r--r--   0 niux10     (501) staff       (20)    15211 2023-06-01 21:32:31.000000 ic50-0.0.99.1/ic50/ic50.py
-drwxr-xr-x   0 niux10     (501) staff       (20)        0 2023-06-01 21:38:34.301096 ic50-0.0.99.1/ic50.egg-info/
--rw-r--r--   0 niux10     (501) staff       (20)      491 2023-06-01 21:38:34.000000 ic50-0.0.99.1/ic50.egg-info/PKG-INFO
--rw-r--r--   0 niux10     (501) staff       (20)      177 2023-06-01 21:38:34.000000 ic50-0.0.99.1/ic50.egg-info/SOURCES.txt
--rw-r--r--   0 niux10     (501) staff       (20)        1 2023-06-01 21:38:34.000000 ic50-0.0.99.1/ic50.egg-info/dependency_links.txt
--rw-r--r--   0 niux10     (501) staff       (20)       23 2023-06-01 21:38:34.000000 ic50-0.0.99.1/ic50.egg-info/requires.txt
--rw-r--r--   0 niux10     (501) staff       (20)        5 2023-06-01 21:38:34.000000 ic50-0.0.99.1/ic50.egg-info/top_level.txt
--rw-r--r--   0 niux10     (501) staff       (20)       38 2023-06-01 21:38:34.301519 ic50-0.0.99.1/setup.cfg
--rw-r--r--   0 niux10     (501) staff       (20)      846 2023-06-01 21:38:25.000000 ic50-0.0.99.1/setup.py
+drwxr-xr-x   0 niux10     (501) staff       (20)        0 2023-06-01 22:30:09.168293 ic50-0.0.99.2/
+-rw-r--r--   0 niux10     (501) staff       (20)      497 2023-06-01 22:30:09.168153 ic50-0.0.99.2/PKG-INFO
+drwxr-xr-x   0 niux10     (501) staff       (20)        0 2023-06-01 22:30:09.167194 ic50-0.0.99.2/ic50/
+-rw-r--r--   0 niux10     (501) staff       (20)       19 2023-06-01 18:16:47.000000 ic50-0.0.99.2/ic50/__init__.py
+-rw-r--r--   0 niux10     (501) staff       (20)    15262 2023-06-01 22:28:31.000000 ic50-0.0.99.2/ic50/ic50.py
+drwxr-xr-x   0 niux10     (501) staff       (20)        0 2023-06-01 22:30:09.167958 ic50-0.0.99.2/ic50.egg-info/
+-rw-r--r--   0 niux10     (501) staff       (20)      497 2023-06-01 22:30:09.000000 ic50-0.0.99.2/ic50.egg-info/PKG-INFO
+-rw-r--r--   0 niux10     (501) staff       (20)      177 2023-06-01 22:30:09.000000 ic50-0.0.99.2/ic50.egg-info/SOURCES.txt
+-rw-r--r--   0 niux10     (501) staff       (20)        1 2023-06-01 22:30:09.000000 ic50-0.0.99.2/ic50.egg-info/dependency_links.txt
+-rw-r--r--   0 niux10     (501) staff       (20)       23 2023-06-01 22:30:09.000000 ic50-0.0.99.2/ic50.egg-info/requires.txt
+-rw-r--r--   0 niux10     (501) staff       (20)        5 2023-06-01 22:30:09.000000 ic50-0.0.99.2/ic50.egg-info/top_level.txt
+-rw-r--r--   0 niux10     (501) staff       (20)       38 2023-06-01 22:30:09.168343 ic50-0.0.99.2/setup.cfg
+-rw-r--r--   0 niux10     (501) staff       (20)      852 2023-06-01 22:24:12.000000 ic50-0.0.99.2/setup.py
```

### Comparing `ic50-0.0.99.1/ic50/ic50.py` & `ic50-0.0.99.2/ic50/ic50.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         self.fitted_params = None
         
     @property
     def version(self):
         return "0.0.99"
     
     def __repr__(self):
-        return f"IC50 Predictor with {len(self.concentrations)} data points and IC50 of {self.ic50}"
+        return f"IC50 Predictor with {len(self.concentrations)} data points and pIC50 of {self.ic50}"
 
     def _fit_linear_interpolation(self) -> dict:
         """Calculate IC50/pIC50 using linear interpolation.
         
         Returns
         -------
         A dict with `ic50`, `slope` and other values.
@@ -248,15 +248,15 @@
             elif method == 'sigmoid':
                 params = fitting_function(maxfev, **params)
             elif method == 'hill':
                 params = fitting_function(hill_params, maxfev, **params)
             else:
                 params = fitting_function()
             self.method = method
-            self.ic50 = params['ic50']  
+            self.ic50 = -params['ic50']  
             self.fitted_params = params  
         else:
             raise ValueError(f"Invalid method '{method}' specified.")
 
         return self
     
     def _predict_interpolation(self, concentrations):
@@ -416,25 +416,26 @@
         Plot of concentration-response curve IC50.
         """
         
         concentrations = np.linspace(min(self.concentrations), max(self.concentrations), n)
         responses = self.predict_response(concentrations)
     
         plt.figure()
-        plt.scatter(self.concentrations, self.responses, color='blue', label='Data')
-        plt.plot(concentrations, responses, color='red', label='Fitted Curve')
-        plt.axvline(x=self.ic50, color='green', linestyle='--', label='IC50')
-        plt.xlabel('Concentration (log)')
-        plt.ylabel('Response (x 100%)')
+        plt.scatter(10**self.concentrations, self.responses*100, color='blue', label='Data')
+        plt.plot(10**concentrations, responses*100, color='red', label='Fitted Curve')
+        plt.axvline(x=10**-self.ic50, color='green', linestyle='--', label='IC50')
+        plt.xlabel('Concentration (log10)')
+        plt.ylabel('Response')
         plt.title('Data and Fitted Curve with IC50')
+        plt.xscale('log',base=10) 
         plt.legend()
         plt.show()
         
         return None
 
     
 if __name__ == "__main__":
     # Example usage
-    concentrations = np.array([0.1, 1, 10, 100, 1000])
+    concentrations = 10**np.arange(-9,-4, dtype=float)
     responses = np.array([1, 4, 16, 64, 100])
     ic50 = IC50Predictor(concentrations, responses)
     ic50 = ic50.calculate_ic50()
```

### Comparing `ic50-0.0.99.1/setup.py` & `ic50-0.0.99.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.99.1' 
+VERSION = '0.0.99.2' 
 DESCRIPTION = 'IC50 prediction'
-LONG_DESCRIPTION = 'Calculate IC50 values using a variety of methods.'
+LONG_DESCRIPTION = 'Calculate IC50/pIC50 values using a variety of methods.'
 
 setup(
         name="ic50", 
         version=VERSION,
         author="Steve Niu",
         author_email="<niuacademics@gmail.com>",
         description=DESCRIPTION,
```

