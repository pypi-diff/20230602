# Comparing `tmp/SRIrepo-0.1.tar.gz` & `tmp/SRIrepo-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SRIrepo-0.1.tar", last modified: Thu Jun  1 07:14:48 2023, max compression
+gzip compressed data, was "dist\SRIrepo-0.2.tar", last modified: Fri Jun  2 06:40:08 2023, max compression
```

## Comparing `SRIrepo-0.1.tar` & `SRIrepo-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 07:14:48.000000 SRIrepo-0.1/
--rw-rw-rw-   0        0        0      205 2023-06-01 07:14:48.000000 SRIrepo-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-01 07:14:48.000000 SRIrepo-0.1/SRIrepo/
--rw-rw-rw-   0        0        0     1667 2023-06-01 07:12:16.000000 SRIrepo-0.1/SRIrepo/SRIrepo.py
--rw-rw-rw-   0        0        0       41 2023-06-01 07:13:04.000000 SRIrepo-0.1/SRIrepo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 07:14:48.000000 SRIrepo-0.1/SRIrepo.egg-info/
--rw-rw-rw-   0        0        0      205 2023-06-01 07:14:48.000000 SRIrepo-0.1/SRIrepo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-06-01 07:14:48.000000 SRIrepo-0.1/SRIrepo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 07:14:48.000000 SRIrepo-0.1/SRIrepo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-01 07:14:48.000000 SRIrepo-0.1/SRIrepo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-01 07:14:48.000000 SRIrepo-0.1/SRIrepo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 07:14:48.000000 SRIrepo-0.1/setup.cfg
--rw-rw-rw-   0        0        0      262 2023-06-01 07:13:56.000000 SRIrepo-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 06:40:08.000000 SRIrepo-0.2/
+-rw-rw-rw-   0        0        0      428 2023-06-02 06:40:08.000000 SRIrepo-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-02 06:40:08.000000 SRIrepo-0.2/SRIrepo/
+-rw-rw-rw-   0        0        0     1765 2023-06-02 06:35:23.000000 SRIrepo-0.2/SRIrepo/SRIrepo.py
+-rw-rw-rw-   0        0        0       41 2023-06-01 07:15:45.000000 SRIrepo-0.2/SRIrepo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 06:40:08.000000 SRIrepo-0.2/SRIrepo.egg-info/
+-rw-rw-rw-   0        0        0      428 2023-06-02 06:40:08.000000 SRIrepo-0.2/SRIrepo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-06-02 06:40:08.000000 SRIrepo-0.2/SRIrepo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 06:40:08.000000 SRIrepo-0.2/SRIrepo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-02 06:40:08.000000 SRIrepo-0.2/SRIrepo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-02 06:40:08.000000 SRIrepo-0.2/SRIrepo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 06:40:08.000000 SRIrepo-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      526 2023-06-02 06:40:04.000000 SRIrepo-0.2/setup.py
```

### Comparing `SRIrepo-0.1/SRIrepo/SRIrepo.py` & `SRIrepo-0.2/SRIrepo/SRIrepo.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,12 @@
+
 import pandas as pd
+import warnings 
+warnings.filterwarnings("ignore")
+
 data = pd.read_excel(r'Pharma_entity_list.xlsx')
 
 def get_pharma_entities(text):
     global Company_list
     global output
     Company_List = []
     Type_List=[]
@@ -47,10 +51,11 @@
     positions = data.loc[data["Entity Name"].isin(common_elements_list), 'Entity Name'].index.values
     
     
     data_copy = pd.read_excel(r'Pharma_entity_list.xlsx',index_col=False)
     data_copy = data_copy[['Entity Name', 'Type']]
     output = data_copy.loc[positions,:]
     output=pd.DataFrame(output)
-    output_print = print(output.to_string(index=False))
-    return output_print
-    
+    output= output.reset_index()
+    output = output.drop('index', axis=1)
+    output.style.hide_index()
+    return output
```

