# Comparing `tmp/pydecs-2023.3.22.tar.gz` & `tmp/pydecs-2023.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydecs-2023.3.22.tar", last modified: Wed Mar 22 01:25:25 2023, max compression
+gzip compressed data, was "pydecs-2023.6.2.tar", last modified: Fri Jun  2 11:00:04 2023, max compression
```

## Comparing `pydecs-2023.3.22.tar` & `pydecs-2023.6.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        0 2023-03-22 01:25:26.251730 pydecs-2023.3.22/
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    11357 2023-03-22 00:25:32.000000 pydecs-2023.3.22/LICENSE.txt
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      537 2023-03-22 01:25:26.251730 pydecs-2023.3.22/PKG-INFO
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      484 2023-03-22 00:25:32.000000 pydecs-2023.3.22/README.md
-drwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        0 2023-03-22 01:25:26.141958 pydecs-2023.3.22/pydecs/
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      257 2023-03-22 00:25:32.000000 pydecs-2023.3.22/pydecs/__init__.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    34329 2023-03-22 00:25:32.000000 pydecs-2023.3.22/pydecs/aux_EdefCorrection_VASP.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     2258 2023-03-22 00:25:32.000000 pydecs-2023.3.22/pydecs/aux_check_equilibrium_phases.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     5274 2023-03-22 00:25:32.000000 pydecs-2023.3.22/pydecs/aux_convDOS.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     1343 2023-03-22 00:25:32.000000 pydecs-2023.3.22/pydecs/aux_convGasEne.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     1792 2023-03-22 00:25:32.000000 pydecs-2023.3.22/pydecs/aux_plot_defectdata.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      671 2023-03-22 00:25:32.000000 pydecs-2023.3.22/pydecs/common.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    11528 2023-03-22 00:25:32.000000 pydecs-2023.3.22/pydecs/defects.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    18343 2023-03-22 01:03:27.000000 pydecs-2023.3.22/pydecs/eqcond.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     4946 2023-03-22 00:25:32.000000 pydecs-2023.3.22/pydecs/host.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    51639 2023-03-22 00:25:32.000000 pydecs-2023.3.22/pydecs/inout.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     4506 2023-03-22 00:25:32.000000 pydecs-2023.3.22/pydecs/pydecs.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     8513 2023-03-22 00:25:32.000000 pydecs-2023.3.22/pydecs/reference_phases.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    32129 2023-03-22 00:25:32.000000 pydecs-2023.3.22/pydecs/solver.py
-drwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        0 2023-03-22 01:25:26.236105 pydecs-2023.3.22/pydecs.egg-info/
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      537 2023-03-22 01:25:25.000000 pydecs-2023.3.22/pydecs.egg-info/PKG-INFO
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      570 2023-03-22 01:25:25.000000 pydecs-2023.3.22/pydecs.egg-info/SOURCES.txt
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        1 2023-03-22 01:25:25.000000 pydecs-2023.3.22/pydecs.egg-info/dependency_links.txt
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      420 2023-03-22 01:25:25.000000 pydecs-2023.3.22/pydecs.egg-info/entry_points.txt
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        1 2023-03-22 01:25:25.000000 pydecs-2023.3.22/pydecs.egg-info/not-zip-safe
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)       35 2023-03-22 01:25:25.000000 pydecs-2023.3.22/pydecs.egg-info/requires.txt
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        7 2023-03-22 01:25:25.000000 pydecs-2023.3.22/pydecs.egg-info/top_level.txt
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)       91 2023-03-22 00:25:32.000000 pydecs-2023.3.22/pyproject.toml
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     1098 2023-03-22 01:25:26.251730 pydecs-2023.3.22/setup.cfg
+drwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        0 2023-06-02 11:00:03.954791 pydecs-2023.6.2/
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    11357 2023-06-02 10:33:14.000000 pydecs-2023.6.2/LICENSE.txt
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      536 2023-06-02 11:00:03.954791 pydecs-2023.6.2/PKG-INFO
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      484 2023-06-02 10:33:14.000000 pydecs-2023.6.2/README.md
+drwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        0 2023-06-02 11:00:03.147533 pydecs-2023.6.2/pydecs/
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      257 2023-06-02 10:33:14.000000 pydecs-2023.6.2/pydecs/__init__.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    34447 2023-06-02 10:51:12.000000 pydecs-2023.6.2/pydecs/aux_EdefCorrection_VASP.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     2258 2023-06-02 10:33:14.000000 pydecs-2023.6.2/pydecs/aux_check_equilibrium_phases.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     5274 2023-06-02 10:33:14.000000 pydecs-2023.6.2/pydecs/aux_convDOS.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     1343 2023-06-02 10:33:14.000000 pydecs-2023.6.2/pydecs/aux_convGasEne.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     1792 2023-06-02 10:33:14.000000 pydecs-2023.6.2/pydecs/aux_plot_defectdata.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      671 2023-06-02 10:33:14.000000 pydecs-2023.6.2/pydecs/common.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    11528 2023-06-02 10:33:14.000000 pydecs-2023.6.2/pydecs/defects.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    18343 2023-06-02 10:33:14.000000 pydecs-2023.6.2/pydecs/eqcond.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     4946 2023-06-02 10:33:14.000000 pydecs-2023.6.2/pydecs/host.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    51639 2023-06-02 10:33:14.000000 pydecs-2023.6.2/pydecs/inout.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     4506 2023-06-02 10:33:14.000000 pydecs-2023.6.2/pydecs/pydecs.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     8513 2023-06-02 10:33:14.000000 pydecs-2023.6.2/pydecs/reference_phases.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    32129 2023-06-02 10:33:14.000000 pydecs-2023.6.2/pydecs/solver.py
+drwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        0 2023-06-02 11:00:03.858086 pydecs-2023.6.2/pydecs.egg-info/
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      536 2023-06-02 11:00:00.000000 pydecs-2023.6.2/pydecs.egg-info/PKG-INFO
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      570 2023-06-02 11:00:01.000000 pydecs-2023.6.2/pydecs.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        1 2023-06-02 11:00:00.000000 pydecs-2023.6.2/pydecs.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      420 2023-06-02 11:00:00.000000 pydecs-2023.6.2/pydecs.egg-info/entry_points.txt
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        1 2023-06-02 10:59:59.000000 pydecs-2023.6.2/pydecs.egg-info/not-zip-safe
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)       35 2023-06-02 11:00:00.000000 pydecs-2023.6.2/pydecs.egg-info/requires.txt
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        7 2023-06-02 11:00:00.000000 pydecs-2023.6.2/pydecs.egg-info/top_level.txt
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)       91 2023-06-02 10:33:14.000000 pydecs-2023.6.2/pyproject.toml
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     1098 2023-06-02 11:00:03.984469 pydecs-2023.6.2/setup.cfg
```

### Comparing `pydecs-2023.3.22/LICENSE.txt` & `pydecs-2023.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydecs-2023.3.22/PKG-INFO` & `pydecs-2023.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydecs
-Version: 2023.3.22
+Version: 2023.6.2
 Summary: This tool enables us to analyze equilibrium concentrations of point and complex defects in crystalline solids
 Home-page: https://gitlab.com/tkog/pydecs
 Author: Takafumi Ogawa
 Author-email: takafumi.ogawa.1+pydecs@gmail.com
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `pydecs-2023.3.22/pydecs/aux_EdefCorrection_VASP.py` & `pydecs-2023.6.2/pydecs/aux_EdefCorrection_VASP.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,18 @@
             l1=fin.readline()
             l1=fin.readline()
             n1=0
             if len(pots_list)>0:
                 pots_list=[]
             while n1<sum(natoms):
                 l1=fin.readline()
-                l2=l1.split()[1::2]
+                l2=[]
+                for t2 in l1.split():
+                    if "-" in t2:
+                        l2.append(float(t2[t2.find("-"):]))
                 for t2 in l2:
                     n1+=1
                     pots_list.append(float(t2))
         l1=fin.readline()
     NELECT_neutral=0.0
     for i1,n1 in enumerate(natoms):
         NELECT_neutral+=n1*zvals[i1]
```

### Comparing `pydecs-2023.3.22/pydecs/aux_check_equilibrium_phases.py` & `pydecs-2023.6.2/pydecs/aux_check_equilibrium_phases.py`

 * *Files identical despite different names*

### Comparing `pydecs-2023.3.22/pydecs/aux_convDOS.py` & `pydecs-2023.6.2/pydecs/aux_convDOS.py`

 * *Files identical despite different names*

### Comparing `pydecs-2023.3.22/pydecs/aux_convGasEne.py` & `pydecs-2023.6.2/pydecs/aux_convGasEne.py`

 * *Files identical despite different names*

### Comparing `pydecs-2023.3.22/pydecs/aux_plot_defectdata.py` & `pydecs-2023.6.2/pydecs/aux_plot_defectdata.py`

 * *Files identical despite different names*

### Comparing `pydecs-2023.3.22/pydecs/common.py` & `pydecs-2023.6.2/pydecs/common.py`

 * *Files identical despite different names*

### Comparing `pydecs-2023.3.22/pydecs/defects.py` & `pydecs-2023.6.2/pydecs/defects.py`

 * *Files identical despite different names*

### Comparing `pydecs-2023.3.22/pydecs/eqcond.py` & `pydecs-2023.6.2/pydecs/eqcond.py`

 * *Files identical despite different names*

### Comparing `pydecs-2023.3.22/pydecs/host.py` & `pydecs-2023.6.2/pydecs/host.py`

 * *Files identical despite different names*

### Comparing `pydecs-2023.3.22/pydecs/inout.py` & `pydecs-2023.6.2/pydecs/inout.py`

 * *Files identical despite different names*

### Comparing `pydecs-2023.3.22/pydecs/pydecs.py` & `pydecs-2023.6.2/pydecs/pydecs.py`

 * *Files identical despite different names*

### Comparing `pydecs-2023.3.22/pydecs/reference_phases.py` & `pydecs-2023.6.2/pydecs/reference_phases.py`

 * *Files identical despite different names*

### Comparing `pydecs-2023.3.22/pydecs/solver.py` & `pydecs-2023.6.2/pydecs/solver.py`

 * *Files identical despite different names*

### Comparing `pydecs-2023.3.22/pydecs.egg-info/PKG-INFO` & `pydecs-2023.6.2/pydecs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydecs
-Version: 2023.3.22
+Version: 2023.6.2
 Summary: This tool enables us to analyze equilibrium concentrations of point and complex defects in crystalline solids
 Home-page: https://gitlab.com/tkog/pydecs
 Author: Takafumi Ogawa
 Author-email: takafumi.ogawa.1+pydecs@gmail.com
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `pydecs-2023.3.22/pydecs.egg-info/SOURCES.txt` & `pydecs-2023.6.2/pydecs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydecs-2023.3.22/setup.cfg` & `pydecs-2023.6.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pydecs
-version = 2023.03.22
+version = 2023.06.02
 description = This tool enables us to analyze equilibrium concentrations of point and complex defects in crystalline solids
 author = Takafumi Ogawa
 author_email = takafumi.ogawa.1+pydecs@gmail.com
 url = https://gitlab.com/tkog/pydecs
 lisense_file = LICENSE.txt
 classifiers = 
 	Intended Audience :: Science/Research
```

