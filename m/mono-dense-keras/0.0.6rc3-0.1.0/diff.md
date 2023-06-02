# Comparing `tmp/mono-dense-keras-0.0.6rc3.tar.gz` & `tmp/mono-dense-keras-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mono-dense-keras-0.0.6rc3.tar", last modified: Fri Jun  2 14:14:31 2023, max compression
+gzip compressed data, was "mono-dense-keras-0.1.0.tar", last modified: Fri Jun  2 14:21:12 2023, max compression
```

## Comparing `mono-dense-keras-0.0.6rc3.tar` & `mono-dense-keras-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-02 14:14:31.598461 mono-dense-keras-0.0.6rc3/
--rw-r--r--   0 davor     (1000) davor     (1000)    20848 2022-09-02 19:27:53.000000 mono-dense-keras-0.0.6rc3/LICENSE
--rw-rw-r--   0 davor     (1000) davor     (1000)      111 2022-08-18 19:39:58.000000 mono-dense-keras-0.0.6rc3/MANIFEST.in
--rw-rw-r--   0 davor     (1000) davor     (1000)    10344 2023-06-02 14:14:31.598461 mono-dense-keras-0.0.6rc3/PKG-INFO
--rw-rw-r--   0 davor     (1000) davor     (1000)     9231 2023-06-02 14:13:16.000000 mono-dense-keras-0.0.6rc3/README.md
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-02 14:14:31.598461 mono-dense-keras-0.0.6rc3/mono_dense_keras/
--rw-rw-r--   0 davor     (1000) davor     (1000)      463 2023-06-02 14:14:28.000000 mono-dense-keras-0.0.6rc3/mono_dense_keras/__init__.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-02 14:14:31.598461 mono-dense-keras-0.0.6rc3/mono_dense_keras/_components/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-02 14:14:28.000000 mono-dense-keras-0.0.6rc3/mono_dense_keras/_components/__init__.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    23910 2023-06-02 14:14:28.000000 mono-dense-keras-0.0.6rc3/mono_dense_keras/_components/mono_dense_layer.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    10897 2023-06-02 14:14:28.000000 mono-dense-keras-0.0.6rc3/mono_dense_keras/_modidx.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    14065 2023-06-02 14:14:28.000000 mono-dense-keras-0.0.6rc3/mono_dense_keras/experiments.py
--rw-rw-r--   0 davor     (1000) davor     (1000)      288 2023-06-02 14:14:28.000000 mono-dense-keras-0.0.6rc3/mono_dense_keras/helpers.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-02 14:14:31.598461 mono-dense-keras-0.0.6rc3/mono_dense_keras.egg-info/
--rw-r--r--   0 davor     (1000) davor     (1000)    10344 2023-06-02 14:14:31.000000 mono-dense-keras-0.0.6rc3/mono_dense_keras.egg-info/PKG-INFO
--rw-r--r--   0 davor     (1000) davor     (1000)      539 2023-06-02 14:14:31.000000 mono-dense-keras-0.0.6rc3/mono_dense_keras.egg-info/SOURCES.txt
--rw-r--r--   0 davor     (1000) davor     (1000)        1 2023-06-02 14:14:31.000000 mono-dense-keras-0.0.6rc3/mono_dense_keras.egg-info/dependency_links.txt
--rw-r--r--   0 davor     (1000) davor     (1000)       54 2023-06-02 14:14:31.000000 mono-dense-keras-0.0.6rc3/mono_dense_keras.egg-info/entry_points.txt
--rw-r--r--   0 davor     (1000) davor     (1000)        1 2022-12-06 04:51:35.000000 mono-dense-keras-0.0.6rc3/mono_dense_keras.egg-info/not-zip-safe
--rw-r--r--   0 davor     (1000) davor     (1000)      224 2023-06-02 14:14:31.000000 mono-dense-keras-0.0.6rc3/mono_dense_keras.egg-info/requires.txt
--rw-r--r--   0 davor     (1000) davor     (1000)       17 2023-06-02 14:14:31.000000 mono-dense-keras-0.0.6rc3/mono_dense_keras.egg-info/top_level.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)      969 2023-06-02 14:14:19.000000 mono-dense-keras-0.0.6rc3/settings.ini
--rw-rw-r--   0 davor     (1000) davor     (1000)       38 2023-06-02 14:14:31.598461 mono-dense-keras-0.0.6rc3/setup.cfg
--rw-rw-r--   0 davor     (1000) davor     (1000)     3093 2023-06-02 14:08:39.000000 mono-dense-keras-0.0.6rc3/setup.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-02 14:21:12.916188 mono-dense-keras-0.1.0/
+-rw-r--r--   0 davor     (1000) davor     (1000)    20848 2022-09-02 19:27:53.000000 mono-dense-keras-0.1.0/LICENSE
+-rw-rw-r--   0 davor     (1000) davor     (1000)      111 2022-08-18 19:39:58.000000 mono-dense-keras-0.1.0/MANIFEST.in
+-rw-rw-r--   0 davor     (1000) davor     (1000)    10249 2023-06-02 14:21:12.916188 mono-dense-keras-0.1.0/PKG-INFO
+-rw-rw-r--   0 davor     (1000) davor     (1000)     9189 2023-06-02 14:20:05.000000 mono-dense-keras-0.1.0/README.md
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-02 14:21:12.912187 mono-dense-keras-0.1.0/mono_dense_keras/
+-rw-rw-r--   0 davor     (1000) davor     (1000)      460 2023-06-02 14:20:34.000000 mono-dense-keras-0.1.0/mono_dense_keras/__init__.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-02 14:21:12.916188 mono-dense-keras-0.1.0/mono_dense_keras/_components/
+-rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-06-02 14:20:34.000000 mono-dense-keras-0.1.0/mono_dense_keras/_components/__init__.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    23910 2023-06-02 14:20:34.000000 mono-dense-keras-0.1.0/mono_dense_keras/_components/mono_dense_layer.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    10897 2023-06-02 14:20:34.000000 mono-dense-keras-0.1.0/mono_dense_keras/_modidx.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    14065 2023-06-02 14:20:34.000000 mono-dense-keras-0.1.0/mono_dense_keras/experiments.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)      288 2023-06-02 14:20:34.000000 mono-dense-keras-0.1.0/mono_dense_keras/helpers.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-06-02 14:21:12.912187 mono-dense-keras-0.1.0/mono_dense_keras.egg-info/
+-rw-r--r--   0 davor     (1000) davor     (1000)    10249 2023-06-02 14:21:12.000000 mono-dense-keras-0.1.0/mono_dense_keras.egg-info/PKG-INFO
+-rw-r--r--   0 davor     (1000) davor     (1000)      539 2023-06-02 14:21:12.000000 mono-dense-keras-0.1.0/mono_dense_keras.egg-info/SOURCES.txt
+-rw-r--r--   0 davor     (1000) davor     (1000)        1 2023-06-02 14:21:12.000000 mono-dense-keras-0.1.0/mono_dense_keras.egg-info/dependency_links.txt
+-rw-r--r--   0 davor     (1000) davor     (1000)       54 2023-06-02 14:21:12.000000 mono-dense-keras-0.1.0/mono_dense_keras.egg-info/entry_points.txt
+-rw-r--r--   0 davor     (1000) davor     (1000)        1 2022-12-06 04:51:35.000000 mono-dense-keras-0.1.0/mono_dense_keras.egg-info/not-zip-safe
+-rw-r--r--   0 davor     (1000) davor     (1000)      224 2023-06-02 14:21:12.000000 mono-dense-keras-0.1.0/mono_dense_keras.egg-info/requires.txt
+-rw-r--r--   0 davor     (1000) davor     (1000)       17 2023-06-02 14:21:12.000000 mono-dense-keras-0.1.0/mono_dense_keras.egg-info/top_level.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)      966 2023-06-02 14:19:42.000000 mono-dense-keras-0.1.0/settings.ini
+-rw-rw-r--   0 davor     (1000) davor     (1000)       38 2023-06-02 14:21:12.916188 mono-dense-keras-0.1.0/setup.cfg
+-rw-rw-r--   0 davor     (1000) davor     (1000)     3093 2023-06-02 14:08:39.000000 mono-dense-keras-0.1.0/setup.py
```

### Comparing `mono-dense-keras-0.0.6rc3/LICENSE` & `mono-dense-keras-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mono-dense-keras-0.0.6rc3/PKG-INFO` & `mono-dense-keras-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: mono-dense-keras
-Version: 0.0.6rc3
+Version: 0.1.0
 Summary: Monotonic Dense Layer implemented in Keras
 Home-page: https://github.com/airtai/mono-dense-keras
 Author: AIRT Technologies d.o.o.
 Author-email: info@airt.ai
 License: Creative Commons License
 Project-URL: Bug Tracker, https://github.com/airtai/mono-dense-keras/issues
 Project-URL: CI, https://github.com/airtai/mono-dense-keras/actions
 Project-URL: Documentation, https://mono-dense-keras.airt.ai/
 Keywords: tensorflow monotone monotonic dense layer nbdev nbdev-mkdocs jupyter notebook python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: Free for non-commercial use
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 Monotonic Dense Layer
 ================
 
@@ -41,15 +40,15 @@
   author={Davor Runje and Sharath M. Shankaranarayana},
   booktitle={Proceedings of the 40th {International Conference on Machine Learning}},
   year={2023}
 }
 ```
 
 This package contains an implementation of our Monotonic Dense Layer
-[`MonoDense`](https://mono-dense-keras.airt.ai/0.0.6rc1/api/mono_dense_keras/MonoDense/#mono_dense_keras.MonoDense)
+[`MonoDense`](https://mono-dense-keras.airt.ai/0.1.0/api/mono_dense_keras/MonoDense/#mono_dense_keras.MonoDense)
 (Constrained Monotonic Fully Connected Layer). Below is the figure from
 the paper for reference.
 
 In the code, the variable `monotonicity_indicator` corresponds to **t**
 in the figure and parameters `is_convex`, `is_concave` and
 `activation_weights` are used to calculate the activation selector **s**
 as follows:
@@ -80,16 +79,14 @@
 In this example, we’ll assume we have a simple dataset with three inputs
 values $x_1$, $x_2$ and $x_3$ sampled from the normal distribution,
 while the output value $y$ is calculated according to the following
 formula before adding Gaussian noise to it:
 
 $y = x_1^3 + \sin\left(\frac{x_2}{2 \pi}\right) + e^{-x_3}$
 
-<style type="text/css">
-</style>
 <table id="T_6be9e">
   <thead>
     <tr>
       <th id="T_6be9e_level0_col0" class="col_heading level0 col0" >x0</th>
       <th id="T_6be9e_level0_col1" class="col_heading level0 col1" >x1</th>
       <th id="T_6be9e_level0_col2" class="col_heading level0 col2" >x2</th>
       <th id="T_6be9e_level0_col3" class="col_heading level0 col3" >y</th>
@@ -126,18 +123,18 @@
       <td id="T_6be9e_row4_col2" class="data row4 col2" >0.467509</td>
       <td id="T_6be9e_row4_col3" class="data row4 col3" >0.780875</td>
     </tr>
   </tbody>
 </table>
 
 Now, we’ll use the
-[`MonoDense`](https://mono-dense-keras.airt.ai/0.0.6rc1/api/mono_dense_keras/MonoDense/#mono_dense_keras.MonoDense)
+[`MonoDense`](https://mono-dense-keras.airt.ai/0.1.0/api/mono_dense_keras/MonoDense/#mono_dense_keras.MonoDense)
 layer instead of `Dense` layer to build a simple monotonic network. By
 default, the
-[`MonoDense`](https://mono-dense-keras.airt.ai/0.0.6rc1/api/mono_dense_keras/MonoDense/#mono_dense_keras.MonoDense)
+[`MonoDense`](https://mono-dense-keras.airt.ai/0.1.0/api/mono_dense_keras/MonoDense/#mono_dense_keras.MonoDense)
 layer assumes the output of the layer is monotonically increasing with
 all inputs. This assumtion is always true for all layers except possibly
 the first one. For the first layer, we use `monotonicity_indicator` to
 specify which input parameters are monotonic and to specify are they
 increasingly or decreasingly monotonic:
 
 - set 1 for increasingly monotonic parameter,
```

### Comparing `mono-dense-keras-0.0.6rc3/README.md` & `mono-dense-keras-0.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   author={Davor Runje and Sharath M. Shankaranarayana},
   booktitle={Proceedings of the 40th {International Conference on Machine Learning}},
   year={2023}
 }
 ```
 
 This package contains an implementation of our Monotonic Dense Layer
-[`MonoDense`](https://mono-dense-keras.airt.ai/0.0.6rc1/api/mono_dense_keras/MonoDense/#mono_dense_keras.MonoDense)
+[`MonoDense`](https://mono-dense-keras.airt.ai/0.1.0/api/mono_dense_keras/MonoDense/#mono_dense_keras.MonoDense)
 (Constrained Monotonic Fully Connected Layer). Below is the figure from
 the paper for reference.
 
 In the code, the variable `monotonicity_indicator` corresponds to **t**
 in the figure and parameters `is_convex`, `is_concave` and
 `activation_weights` are used to calculate the activation selector **s**
 as follows:
@@ -54,16 +54,14 @@
 In this example, we’ll assume we have a simple dataset with three inputs
 values $x_1$, $x_2$ and $x_3$ sampled from the normal distribution,
 while the output value $y$ is calculated according to the following
 formula before adding Gaussian noise to it:
 
 $y = x_1^3 + \sin\left(\frac{x_2}{2 \pi}\right) + e^{-x_3}$
 
-<style type="text/css">
-</style>
 <table id="T_6be9e">
   <thead>
     <tr>
       <th id="T_6be9e_level0_col0" class="col_heading level0 col0" >x0</th>
       <th id="T_6be9e_level0_col1" class="col_heading level0 col1" >x1</th>
       <th id="T_6be9e_level0_col2" class="col_heading level0 col2" >x2</th>
       <th id="T_6be9e_level0_col3" class="col_heading level0 col3" >y</th>
@@ -100,18 +98,18 @@
       <td id="T_6be9e_row4_col2" class="data row4 col2" >0.467509</td>
       <td id="T_6be9e_row4_col3" class="data row4 col3" >0.780875</td>
     </tr>
   </tbody>
 </table>
 
 Now, we’ll use the
-[`MonoDense`](https://mono-dense-keras.airt.ai/0.0.6rc1/api/mono_dense_keras/MonoDense/#mono_dense_keras.MonoDense)
+[`MonoDense`](https://mono-dense-keras.airt.ai/0.1.0/api/mono_dense_keras/MonoDense/#mono_dense_keras.MonoDense)
 layer instead of `Dense` layer to build a simple monotonic network. By
 default, the
-[`MonoDense`](https://mono-dense-keras.airt.ai/0.0.6rc1/api/mono_dense_keras/MonoDense/#mono_dense_keras.MonoDense)
+[`MonoDense`](https://mono-dense-keras.airt.ai/0.1.0/api/mono_dense_keras/MonoDense/#mono_dense_keras.MonoDense)
 layer assumes the output of the layer is monotonically increasing with
 all inputs. This assumtion is always true for all layers except possibly
 the first one. For the first layer, we use `monotonicity_indicator` to
 specify which input parameters are monotonic and to specify are they
 increasingly or decreasingly monotonic:
 
 - set 1 for increasingly monotonic parameter,
```

### Comparing `mono-dense-keras-0.0.6rc3/mono_dense_keras/_components/mono_dense_layer.py` & `mono-dense-keras-0.1.0/mono_dense_keras/_components/mono_dense_layer.py`

 * *Files identical despite different names*

### Comparing `mono-dense-keras-0.0.6rc3/mono_dense_keras/_modidx.py` & `mono-dense-keras-0.1.0/mono_dense_keras/_modidx.py`

 * *Files identical despite different names*

### Comparing `mono-dense-keras-0.0.6rc3/mono_dense_keras/experiments.py` & `mono-dense-keras-0.1.0/mono_dense_keras/experiments.py`

 * *Files identical despite different names*

### Comparing `mono-dense-keras-0.0.6rc3/mono_dense_keras.egg-info/PKG-INFO` & `mono-dense-keras-0.1.0/mono_dense_keras.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: mono-dense-keras
-Version: 0.0.6rc3
+Version: 0.1.0
 Summary: Monotonic Dense Layer implemented in Keras
 Home-page: https://github.com/airtai/mono-dense-keras
 Author: AIRT Technologies d.o.o.
 Author-email: info@airt.ai
 License: Creative Commons License
 Project-URL: Bug Tracker, https://github.com/airtai/mono-dense-keras/issues
 Project-URL: CI, https://github.com/airtai/mono-dense-keras/actions
 Project-URL: Documentation, https://mono-dense-keras.airt.ai/
 Keywords: tensorflow monotone monotonic dense layer nbdev nbdev-mkdocs jupyter notebook python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: Free for non-commercial use
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 Monotonic Dense Layer
 ================
 
@@ -41,15 +40,15 @@
   author={Davor Runje and Sharath M. Shankaranarayana},
   booktitle={Proceedings of the 40th {International Conference on Machine Learning}},
   year={2023}
 }
 ```
 
 This package contains an implementation of our Monotonic Dense Layer
-[`MonoDense`](https://mono-dense-keras.airt.ai/0.0.6rc1/api/mono_dense_keras/MonoDense/#mono_dense_keras.MonoDense)
+[`MonoDense`](https://mono-dense-keras.airt.ai/0.1.0/api/mono_dense_keras/MonoDense/#mono_dense_keras.MonoDense)
 (Constrained Monotonic Fully Connected Layer). Below is the figure from
 the paper for reference.
 
 In the code, the variable `monotonicity_indicator` corresponds to **t**
 in the figure and parameters `is_convex`, `is_concave` and
 `activation_weights` are used to calculate the activation selector **s**
 as follows:
@@ -80,16 +79,14 @@
 In this example, we’ll assume we have a simple dataset with three inputs
 values $x_1$, $x_2$ and $x_3$ sampled from the normal distribution,
 while the output value $y$ is calculated according to the following
 formula before adding Gaussian noise to it:
 
 $y = x_1^3 + \sin\left(\frac{x_2}{2 \pi}\right) + e^{-x_3}$
 
-<style type="text/css">
-</style>
 <table id="T_6be9e">
   <thead>
     <tr>
       <th id="T_6be9e_level0_col0" class="col_heading level0 col0" >x0</th>
       <th id="T_6be9e_level0_col1" class="col_heading level0 col1" >x1</th>
       <th id="T_6be9e_level0_col2" class="col_heading level0 col2" >x2</th>
       <th id="T_6be9e_level0_col3" class="col_heading level0 col3" >y</th>
@@ -126,18 +123,18 @@
       <td id="T_6be9e_row4_col2" class="data row4 col2" >0.467509</td>
       <td id="T_6be9e_row4_col3" class="data row4 col3" >0.780875</td>
     </tr>
   </tbody>
 </table>
 
 Now, we’ll use the
-[`MonoDense`](https://mono-dense-keras.airt.ai/0.0.6rc1/api/mono_dense_keras/MonoDense/#mono_dense_keras.MonoDense)
+[`MonoDense`](https://mono-dense-keras.airt.ai/0.1.0/api/mono_dense_keras/MonoDense/#mono_dense_keras.MonoDense)
 layer instead of `Dense` layer to build a simple monotonic network. By
 default, the
-[`MonoDense`](https://mono-dense-keras.airt.ai/0.0.6rc1/api/mono_dense_keras/MonoDense/#mono_dense_keras.MonoDense)
+[`MonoDense`](https://mono-dense-keras.airt.ai/0.1.0/api/mono_dense_keras/MonoDense/#mono_dense_keras.MonoDense)
 layer assumes the output of the layer is monotonically increasing with
 all inputs. This assumtion is always true for all layers except possibly
 the first one. For the first layer, we use `monotonicity_indicator` to
 specify which input parameters are monotonic and to specify are they
 increasingly or decreasingly monotonic:
 
 - set 1 for increasingly monotonic parameter,
```

### Comparing `mono-dense-keras-0.0.6rc3/mono_dense_keras.egg-info/SOURCES.txt` & `mono-dense-keras-0.1.0/mono_dense_keras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mono-dense-keras-0.0.6rc3/setup.py` & `mono-dense-keras-0.1.0/setup.py`

 * *Files identical despite different names*

