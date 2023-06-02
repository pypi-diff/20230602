# Comparing `tmp/pylibffm-0.2.3.tar.gz` & `tmp/pylibffm-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylibffm-0.2.3.tar", last modified: Fri Jun  2 12:59:09 2023, max compression
+gzip compressed data, was "pylibffm-0.2.4.tar", last modified: Fri Jun  2 13:48:08 2023, max compression
```

## Comparing `pylibffm-0.2.3.tar` & `pylibffm-0.2.4.tar`

### file list

```diff
@@ -1,60 +1,20 @@
-drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-02 12:59:09.801900 pylibffm-0.2.3/
--rw-rw-r--   0 julien    (1003) julien    (1003)     1064 2023-06-01 12:37:51.000000 pylibffm-0.2.3/LICENSE
--rw-rw-r--   0 julien    (1003) julien    (1003)       28 2023-06-02 12:46:04.000000 pylibffm-0.2.3/MANIFEST.in
--rw-rw-r--   0 julien    (1003) julien    (1003)     1302 2023-06-02 12:59:09.801900 pylibffm-0.2.3/PKG-INFO
--rw-rw-r--   0 julien    (1003) julien    (1003)      815 2023-06-02 12:35:18.000000 pylibffm-0.2.3/README.md
-drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-02 12:59:09.797900 pylibffm-0.2.3/libffm/
--rw-rw-r--   0 julien    (1003) julien    (1003)       31 2023-06-01 12:37:52.000000 pylibffm-0.2.3/libffm/.git
--rw-rw-r--   0 julien    (1003) julien    (1003)     1478 2023-06-01 12:37:54.000000 pylibffm-0.2.3/libffm/COPYRIGHT
--rw-rw-r--   0 julien    (1003) julien    (1003)      626 2023-06-01 12:37:54.000000 pylibffm-0.2.3/libffm/Makefile
--rw-rw-r--   0 julien    (1003) julien    (1003)      697 2023-06-01 12:37:54.000000 pylibffm-0.2.3/libffm/Makefile.win
--rw-rw-r--   0 julien    (1003) julien    (1003)     8692 2023-06-01 12:37:54.000000 pylibffm-0.2.3/libffm/README
--rwxrwxr-x   0 julien    (1003) julien    (1003)    71240 2023-06-02 07:29:22.000000 pylibffm-0.2.3/libffm/ffm-predict
--rw-rw-r--   0 julien    (1003) julien    (1003)     2396 2023-06-01 12:37:54.000000 pylibffm-0.2.3/libffm/ffm-predict.cpp
--rwxrwxr-x   0 julien    (1003) julien    (1003)    75448 2023-06-02 07:29:21.000000 pylibffm-0.2.3/libffm/ffm-train
--rw-rw-r--   0 julien    (1003) julien    (1003)     5214 2023-06-02 07:25:19.000000 pylibffm-0.2.3/libffm/ffm-train.cpp
--rw-rw-r--   0 julien    (1003) julien    (1003)    19754 2023-06-02 07:04:48.000000 pylibffm-0.2.3/libffm/ffm.cpp
--rw-rw-r--   0 julien    (1003) julien    (1003)     1133 2023-06-01 12:37:54.000000 pylibffm-0.2.3/libffm/ffm.h
--rw-rw-r--   0 julien    (1003) julien    (1003)      570 2023-06-01 12:37:54.000000 pylibffm-0.2.3/libffm/timer.cpp
--rw-rw-r--   0 julien    (1003) julien    (1003)      232 2023-06-01 12:37:54.000000 pylibffm-0.2.3/libffm/timer.h
--rw-rw-r--   0 julien    (1003) julien    (1003)     1975 2023-06-02 07:29:15.000000 pylibffm-0.2.3/libffm/tmp.ffm
--rw-rw-r--   0 julien    (1003) julien    (1003)     1360 2023-06-02 07:29:27.000000 pylibffm-0.2.3/libffm/tmp.ffm.bin
--rw-rw-r--   0 julien    (1003) julien    (1003)      141 2023-06-02 07:29:27.000000 pylibffm-0.2.3/libffm/tmp.ffm.model
--rw-rw-r--   0 julien    (1003) julien    (1003)      361 2023-06-01 12:37:51.000000 pylibffm-0.2.3/libffm-makefile
--rw-rw-r--   0 julien    (1003) julien    (1003)      724 2023-06-01 12:37:51.000000 pylibffm-0.2.3/makefile
-drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-02 12:59:09.801900 pylibffm-0.2.3/pybind11/
--rw-rw-r--   0 julien    (1003) julien    (1003)     1271 2023-06-01 12:37:54.000000 pylibffm-0.2.3/pybind11/.appveyor.yml
--rw-rw-r--   0 julien    (1003) julien    (1003)      996 2023-06-01 12:37:54.000000 pylibffm-0.2.3/pybind11/.clang-format
--rw-rw-r--   0 julien    (1003) julien    (1003)     2605 2023-06-01 12:37:54.000000 pylibffm-0.2.3/pybind11/.clang-tidy
--rw-rw-r--   0 julien    (1003) julien    (1003)     2196 2023-06-01 12:37:54.000000 pylibffm-0.2.3/pybind11/.cmake-format.yaml
--rw-rw-r--   0 julien    (1003) julien    (1003)     1308 2023-06-01 12:37:54.000000 pylibffm-0.2.3/pybind11/.codespell-ignore-lines
--rw-rw-r--   0 julien    (1003) julien    (1003)       33 2023-06-01 12:37:54.000000 pylibffm-0.2.3/pybind11/.git
--rw-rw-r--   0 julien    (1003) julien    (1003)       18 2023-06-01 12:37:54.000000 pylibffm-0.2.3/pybind11/.gitattributes
--rw-rw-r--   0 julien    (1003) julien    (1003)      502 2023-06-01 12:37:54.000000 pylibffm-0.2.3/pybind11/.gitignore
--rw-rw-r--   0 julien    (1003) julien    (1003)     3600 2023-06-01 12:37:54.000000 pylibffm-0.2.3/pybind11/.pre-commit-config.yaml
--rw-rw-r--   0 julien    (1003) julien    (1003)       62 2023-06-01 12:37:54.000000 pylibffm-0.2.3/pybind11/.readthedocs.yml
--rw-rw-r--   0 julien    (1003) julien    (1003)    12067 2023-06-01 12:37:54.000000 pylibffm-0.2.3/pybind11/CMakeLists.txt
--rw-rw-r--   0 julien    (1003) julien    (1003)     1684 2023-06-01 12:37:54.000000 pylibffm-0.2.3/pybind11/LICENSE
--rw-rw-r--   0 julien    (1003) julien    (1003)      247 2023-06-01 12:37:54.000000 pylibffm-0.2.3/pybind11/MANIFEST.in
--rw-rw-r--   0 julien    (1003) julien    (1003)     7686 2023-06-01 12:37:54.000000 pylibffm-0.2.3/pybind11/README.rst
--rw-rw-r--   0 julien    (1003) julien    (1003)      688 2023-06-01 12:37:54.000000 pylibffm-0.2.3/pybind11/SECURITY.md
--rw-rw-r--   0 julien    (1003) julien    (1003)     2765 2023-06-01 12:37:54.000000 pylibffm-0.2.3/pybind11/noxfile.py
--rw-rw-r--   0 julien    (1003) julien    (1003)     2360 2023-06-01 12:37:54.000000 pylibffm-0.2.3/pybind11/pyproject.toml
--rw-rw-r--   0 julien    (1003) julien    (1003)     1452 2023-06-01 12:37:54.000000 pylibffm-0.2.3/pybind11/setup.cfg
--rw-rw-r--   0 julien    (1003) julien    (1003)     4877 2023-06-01 12:37:54.000000 pylibffm-0.2.3/pybind11/setup.py
-drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-02 12:59:09.801900 pylibffm-0.2.3/pylibffm/
--rw-rw-r--   0 julien    (1003) julien    (1003)       19 2023-06-02 06:22:22.000000 pylibffm-0.2.3/pylibffm/__init__.py
--rw-rw-r--   0 julien    (1003) julien    (1003)     5288 2023-06-02 07:22:36.000000 pylibffm-0.2.3/pylibffm/api.py
--rwxrwxr-x   0 julien    (1003) julien    (1003)   325896 2023-06-02 12:43:03.000000 pylibffm-0.2.3/pylibffm/wrapper.cpython-310-x86_64-linux-gnu.so
--rwxrwxr-x   0 julien    (1003) julien    (1003)   330280 2023-06-02 12:43:08.000000 pylibffm-0.2.3/pylibffm/wrapper.cpython-311-x86_64-linux-gnu.so
--rwxrwxr-x   0 julien    (1003) julien    (1003)   325856 2023-06-02 12:42:46.000000 pylibffm-0.2.3/pylibffm/wrapper.cpython-37m-x86_64-linux-gnu.so
--rwxrwxr-x   0 julien    (1003) julien    (1003)   325760 2023-06-02 12:42:52.000000 pylibffm-0.2.3/pylibffm/wrapper.cpython-38-x86_64-linux-gnu.so
--rwxrwxr-x   0 julien    (1003) julien    (1003)   326104 2023-06-02 12:42:57.000000 pylibffm-0.2.3/pylibffm/wrapper.cpython-39-x86_64-linux-gnu.so
-drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-02 12:59:09.801900 pylibffm-0.2.3/pylibffm.egg-info/
--rw-rw-r--   0 julien    (1003) julien    (1003)     1302 2023-06-02 12:59:09.000000 pylibffm-0.2.3/pylibffm.egg-info/PKG-INFO
--rw-rw-r--   0 julien    (1003) julien    (1003)     1205 2023-06-02 12:59:09.000000 pylibffm-0.2.3/pylibffm.egg-info/SOURCES.txt
--rw-rw-r--   0 julien    (1003) julien    (1003)        1 2023-06-02 12:59:09.000000 pylibffm-0.2.3/pylibffm.egg-info/dependency_links.txt
--rw-rw-r--   0 julien    (1003) julien    (1003)       12 2023-06-02 12:59:09.000000 pylibffm-0.2.3/pylibffm.egg-info/requires.txt
--rw-rw-r--   0 julien    (1003) julien    (1003)        9 2023-06-02 12:59:09.000000 pylibffm-0.2.3/pylibffm.egg-info/top_level.txt
--rw-rw-r--   0 julien    (1003) julien    (1003)       38 2023-06-02 12:59:09.801900 pylibffm-0.2.3/setup.cfg
--rw-rw-r--   0 julien    (1003) julien    (1003)     1523 2023-06-02 12:59:06.000000 pylibffm-0.2.3/setup.py
+drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-02 13:48:08.245881 pylibffm-0.2.4/
+-rw-rw-r--   0 julien    (1003) julien    (1003)       28 2023-06-02 12:46:04.000000 pylibffm-0.2.4/MANIFEST.in
+-rw-rw-r--   0 julien    (1003) julien    (1003)     1590 2023-06-02 13:48:08.245881 pylibffm-0.2.4/PKG-INFO
+-rw-rw-r--   0 julien    (1003) julien    (1003)      815 2023-06-02 12:35:18.000000 pylibffm-0.2.4/README.md
+drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-02 13:48:08.245881 pylibffm-0.2.4/pylibffm/
+-rw-rw-r--   0 julien    (1003) julien    (1003)       19 2023-06-02 06:22:22.000000 pylibffm-0.2.4/pylibffm/__init__.py
+-rw-rw-r--   0 julien    (1003) julien    (1003)     5295 2023-06-02 13:43:33.000000 pylibffm-0.2.4/pylibffm/api.py
+-rwxrwxr-x   0 julien    (1003) julien    (1003)   325896 2023-06-02 13:45:27.000000 pylibffm-0.2.4/pylibffm/wrapper.cpython-310-x86_64-linux-gnu.so
+-rwxrwxr-x   0 julien    (1003) julien    (1003)   330280 2023-06-02 13:45:32.000000 pylibffm-0.2.4/pylibffm/wrapper.cpython-311-x86_64-linux-gnu.so
+-rwxrwxr-x   0 julien    (1003) julien    (1003)   325856 2023-06-02 13:45:13.000000 pylibffm-0.2.4/pylibffm/wrapper.cpython-37m-x86_64-linux-gnu.so
+-rwxrwxr-x   0 julien    (1003) julien    (1003)   325760 2023-06-02 13:45:18.000000 pylibffm-0.2.4/pylibffm/wrapper.cpython-38-x86_64-linux-gnu.so
+-rwxrwxr-x   0 julien    (1003) julien    (1003)   326104 2023-06-02 13:45:23.000000 pylibffm-0.2.4/pylibffm/wrapper.cpython-39-x86_64-linux-gnu.so
+drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-02 13:48:08.245881 pylibffm-0.2.4/pylibffm.egg-info/
+-rw-rw-r--   0 julien    (1003) julien    (1003)     1590 2023-06-02 13:48:08.000000 pylibffm-0.2.4/pylibffm.egg-info/PKG-INFO
+-rw-rw-r--   0 julien    (1003) julien    (1003)      469 2023-06-02 13:48:08.000000 pylibffm-0.2.4/pylibffm.egg-info/SOURCES.txt
+-rw-rw-r--   0 julien    (1003) julien    (1003)        1 2023-06-02 13:48:08.000000 pylibffm-0.2.4/pylibffm.egg-info/dependency_links.txt
+-rw-rw-r--   0 julien    (1003) julien    (1003)       12 2023-06-02 13:48:08.000000 pylibffm-0.2.4/pylibffm.egg-info/requires.txt
+-rw-rw-r--   0 julien    (1003) julien    (1003)        9 2023-06-02 13:48:08.000000 pylibffm-0.2.4/pylibffm.egg-info/top_level.txt
+-rw-rw-r--   0 julien    (1003) julien    (1003)       38 2023-06-02 13:48:08.245881 pylibffm-0.2.4/setup.cfg
+-rw-rw-r--   0 julien    (1003) julien    (1003)     1523 2023-06-02 13:48:04.000000 pylibffm-0.2.4/setup.py
```

### Comparing `pylibffm-0.2.3/PKG-INFO` & `pylibffm-0.2.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 Metadata-Version: 2.1
 Name: pylibffm
-Version: 0.2.3
+Version: 0.2.4
 Summary: A library wrapping libffm
 Home-page: https://github.com/Sinacam/pylibffm
 Author: ntumlgroup
 License: MIT License
+Description: # pylibffm
+        
+        pylibffm is a wrapper around libffm to allow using scipy and numpy arrays as input.
+        
+        ## Installing
+        If you're running python 3.7~3.11 on linux
+        ```bash
+        pip install pylibffm
+        ```
+        Otherwise
+        ```bash
+        git clone https://github.com/Sinacam/pylibffm
+        cd pylibffm
+        make
+        pip install .
+        ```
+        Currently, the distribution is incredibly hacky and cannot be pip installed from source.
+        Windows build support is lacking, but code should be correct.
+        
+        ## Documentation
+        The API only consists of
+        + `train`
+        + `load`
+        + `Model`
+            + `Model.save`
+            + `Model.predict`
+        
+        Use `help` or read their docstring for their usage.
+        
+        ## Diff with libffm
+        To be deterministic, set openmp threads to 1. For pylibffm, do
+        ```bash
+        OMP_NUM_THREADS=1 python <script>.py
+        ```
+        
+        For libffm, run with `-s 1` (the default). This should yield identical models.
+Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# pylibffm
-
-pylibffm is a wrapper around libffm to allow using scipy and numpy arrays as input.
-
-## Installing
-If you're running python 3.7~3.11 on linux
-```bash
-pip install pylibffm
-```
-Otherwise
-```bash
-git clone https://github.com/Sinacam/pylibffm
-cd pylibffm
-make
-pip install .
-```
-Currently, the distribution is incredibly hacky and cannot be pip installed from source.
-Windows build support is lacking, but code should be correct.
-
-## Documentation
-The API only consists of
-+ `train`
-+ `load`
-+ `Model`
-    + `Model.save`
-    + `Model.predict`
-
-Use `help` or read their docstring for their usage.
-
-## Diff with libffm
-To be deterministic, set openmp threads to 1. For pylibffm, do
-```bash
-OMP_NUM_THREADS=1 python <script>.py
-```
-
-For libffm, run with `-s 1` (the default). This should yield identical models.
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_zg908nc0_/tmp6_y9cs4d_TarContainer/0/3", line 52, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_zg908nc0_/tmp6_y9cs4d_TarContainer/0/3", line 52, column 0: CDATA terminal not found*

```diff
@@ -1,14 +1,10 @@
-Metadata-Version: 2.1 Name: pylibffm Version: 0.2.3 Summary: A library wrapping
+Metadata-Version: 2.1 Name: pylibffm Version: 0.2.4 Summary: A library wrapping
 libffm Home-page: https://github.com/Sinacam/pylibffm Author: ntumlgroup
-License: MIT License Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Description-Content-Type:
-text/markdown License-File: LICENSE # pylibffm pylibffm is a wrapper around
+License: MIT License Description: # pylibffm pylibffm is a wrapper around
 libffm to allow using scipy and numpy arrays as input. ## Installing If you're
 running python 3.7~3.11 on linux ```bash pip install pylibffm ``` Otherwise
 ```bash git clone https://github.com/Sinacam/pylibffm cd pylibffm make pip
 install . ``` Currently, the distribution is incredibly hacky and cannot be pip
 installed from source. Windows build support is lacking, but code should be
 correct. ## Documentation The API only consists of + `train` + `load` + `Model`
 + `Model.save` + `Model.predict` Use `help` or read their docstring for their
```

### Comparing `pylibffm-0.2.3/README.md` & `pylibffm-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.3/pylibffm/api.py` & `pylibffm-0.2.4/pylibffm/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
         Returns:
             np.ndarray: An array with dimension number of instances.
         """
         if x.shape[1] != fields.shape[0]:
             raise ValueError("input matrix shapes do not match")
 
-        wrapper.predict(
+        return wrapper.predict(
             self.n,
             self.m,
             self.k,
             self.W,
             self.normalization,
             x.shape[0],
             x.shape[1],
```

### Comparing `pylibffm-0.2.3/pylibffm/wrapper.cpython-310-x86_64-linux-gnu.so` & `pylibffm-0.2.4/pylibffm/wrapper.cpython-310-x86_64-linux-gnu.so`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 0% similar despite different names*

#### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: fd399112843269393df6286b2d0fb646d16ca032
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 80fa12b76b9f81ee0a85f230524520853a472e5f
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -5697,22 +5697,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x8(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r15d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r15d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r15d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r15d,%esi
 	movslq %esi,%rsi
 	call   91c0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r15d,%ecx
 	cmp    %ebp,%r15d
 	jge    101a0 <pybind11::array_t<float, 1> (anonymous namespace)::predict<float>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<float, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x1f0>
 	sub    $0x1,%ebp
@@ -5862,22 +5862,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x8(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91c0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    10470 <pybind11::array_t<float, 1> (anonymous namespace)::predict<unsigned char>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<unsigned char, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x8(%rsp),%rdx
@@ -6030,22 +6030,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x8(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91c0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    10730 <pybind11::array_t<float, 1> (anonymous namespace)::predict<unsigned int>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<unsigned int, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	sub    $0x1,%ebp
@@ -6198,22 +6198,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x10(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91c0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    109f0 <pybind11::array_t<float, 1> (anonymous namespace)::predict<long>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<long, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x10(%rsp),%rdx
@@ -6365,22 +6365,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x10(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91c0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    10cb0 <pybind11::array_t<float, 1> (anonymous namespace)::predict<short>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<short, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x10(%rsp),%rdx
@@ -6533,22 +6533,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x8(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91c0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    10f70 <pybind11::array_t<float, 1> (anonymous namespace)::predict<signed char>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<signed char, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x8(%rsp),%rdx
@@ -6701,22 +6701,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x8(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91c0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    11230 <pybind11::array_t<float, 1> (anonymous namespace)::predict<int>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	sub    $0x1,%ebp
@@ -6868,22 +6868,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x10(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91c0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    11520 <pybind11::array_t<float, 1> (anonymous namespace)::predict<unsigned long>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<unsigned long, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x230>
 	mov    0x10(%rsp),%rdi
@@ -7048,22 +7048,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x10(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91c0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    117e0 <pybind11::array_t<float, 1> (anonymous namespace)::predict<unsigned short>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<unsigned short, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x10(%rsp),%rdx
@@ -7216,22 +7216,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x8(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91c0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    11aa0 <pybind11::array_t<float, 1> (anonymous namespace)::predict<bool>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<bool, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x8(%rsp),%rdx
@@ -7384,22 +7384,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x10(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91c0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    11d60 <pybind11::array_t<float, 1> (anonymous namespace)::predict<double>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<double, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x10(%rsp),%rdx
```

### Comparing `pylibffm-0.2.3/pylibffm/wrapper.cpython-311-x86_64-linux-gnu.so` & `pylibffm-0.2.4/pylibffm/wrapper.cpython-311-x86_64-linux-gnu.so`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 0% similar despite different names*

#### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: c7c6ac3dcc187e37b1a3943cde2f8f1856c113eb
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 3c6c3e3ba1434c094e0391d506551ea7716ace0c
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -6006,22 +6006,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x10(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91e0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    10750 <pybind11::array_t<float, 1> (anonymous namespace)::predict<unsigned short>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<unsigned short, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x10(%rsp),%rdx
@@ -6174,22 +6174,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x10(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91e0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    10a10 <pybind11::array_t<float, 1> (anonymous namespace)::predict<long>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<long, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x10(%rsp),%rdx
@@ -6342,22 +6342,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x8(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r15d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r15d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r15d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r15d,%esi
 	movslq %esi,%rsi
 	call   91e0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r15d,%ecx
 	cmp    %ebp,%r15d
 	jge    10cc0 <pybind11::array_t<float, 1> (anonymous namespace)::predict<float>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<float, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x1f0>
 	sub    $0x1,%ebp
@@ -6507,22 +6507,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x8(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91e0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    10f90 <pybind11::array_t<float, 1> (anonymous namespace)::predict<signed char>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<signed char, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x8(%rsp),%rdx
@@ -6675,22 +6675,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x10(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91e0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    11250 <pybind11::array_t<float, 1> (anonymous namespace)::predict<short>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<short, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x10(%rsp),%rdx
@@ -6843,22 +6843,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x10(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91e0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    11540 <pybind11::array_t<float, 1> (anonymous namespace)::predict<unsigned long>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<unsigned long, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x230>
 	mov    0x10(%rsp),%rdi
@@ -7023,22 +7023,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x10(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91e0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    11800 <pybind11::array_t<float, 1> (anonymous namespace)::predict<double>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<double, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x10(%rsp),%rdx
@@ -7190,22 +7190,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x8(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91e0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    11ac0 <pybind11::array_t<float, 1> (anonymous namespace)::predict<int>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	sub    $0x1,%ebp
@@ -7357,22 +7357,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x8(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91e0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    11d80 <pybind11::array_t<float, 1> (anonymous namespace)::predict<unsigned char>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<unsigned char, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x8(%rsp),%rdx
@@ -7525,22 +7525,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x8(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91e0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    12040 <pybind11::array_t<float, 1> (anonymous namespace)::predict<bool>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<bool, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x8(%rsp),%rdx
@@ -7693,22 +7693,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x8(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91e0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    12300 <pybind11::array_t<float, 1> (anonymous namespace)::predict<unsigned int>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<unsigned int, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	sub    $0x1,%ebp
```

### Comparing `pylibffm-0.2.3/pylibffm/wrapper.cpython-37m-x86_64-linux-gnu.so` & `pylibffm-0.2.4/pylibffm/wrapper.cpython-37m-x86_64-linux-gnu.so`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 0% similar despite different names*

#### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: d63744d1936477cc5354b1886e186fd95b5317b7
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 3bf9a5cd3413be667d362b3557997dc6e2cc19c3
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -5095,22 +5095,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x8(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91a0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    f6d0 <pybind11::array_t<float, 1> (anonymous namespace)::predict<signed char>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<signed char, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x8(%rsp),%rdx
@@ -5263,22 +5263,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x8(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91a0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    f990 <pybind11::array_t<float, 1> (anonymous namespace)::predict<unsigned int>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<unsigned int, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	sub    $0x1,%ebp
@@ -5431,22 +5431,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x10(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91a0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    fc50 <pybind11::array_t<float, 1> (anonymous namespace)::predict<double>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<double, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x10(%rsp),%rdx
@@ -5598,22 +5598,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x8(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91a0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    ff10 <pybind11::array_t<float, 1> (anonymous namespace)::predict<bool>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<bool, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x8(%rsp),%rdx
@@ -5767,22 +5767,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x8(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r15d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r15d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r15d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r15d,%esi
 	movslq %esi,%rsi
 	call   91a0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r15d,%ecx
 	cmp    %ebp,%r15d
 	jge    101c0 <pybind11::array_t<float, 1> (anonymous namespace)::predict<float>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<float, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x1f0>
 	sub    $0x1,%ebp
@@ -5932,22 +5932,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x10(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91a0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    10490 <pybind11::array_t<float, 1> (anonymous namespace)::predict<long>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<long, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x10(%rsp),%rdx
@@ -6099,22 +6099,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x10(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91a0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    10750 <pybind11::array_t<float, 1> (anonymous namespace)::predict<short>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<short, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x10(%rsp),%rdx
@@ -6267,22 +6267,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x10(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91a0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    10a10 <pybind11::array_t<float, 1> (anonymous namespace)::predict<unsigned short>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<unsigned short, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x10(%rsp),%rdx
@@ -6435,22 +6435,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x8(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91a0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    10cd0 <pybind11::array_t<float, 1> (anonymous namespace)::predict<unsigned char>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<unsigned char, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x8(%rsp),%rdx
@@ -6603,22 +6603,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x10(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91a0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    10fc0 <pybind11::array_t<float, 1> (anonymous namespace)::predict<unsigned long>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<unsigned long, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x230>
 	mov    0x10(%rsp),%rdi
@@ -6783,22 +6783,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x8(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91a0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    11280 <pybind11::array_t<float, 1> (anonymous namespace)::predict<int>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	sub    $0x1,%ebp
```

### Comparing `pylibffm-0.2.3/pylibffm/wrapper.cpython-38-x86_64-linux-gnu.so` & `pylibffm-0.2.4/pylibffm/wrapper.cpython-38-x86_64-linux-gnu.so`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 1% similar despite different names*

#### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: bf87d21c655828d63eee93be8ca4211e8c35bfb6
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: bbd43731a214952e9d84632c645f01eeedd0ebbc
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -5680,22 +5680,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x10(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   9190 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    100f0 <pybind11::array_t<float, 1> (anonymous namespace)::predict<short>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<short, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x10(%rsp),%rdx
@@ -5848,22 +5848,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x10(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   9190 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    103e0 <pybind11::array_t<float, 1> (anonymous namespace)::predict<unsigned long>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<unsigned long, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x230>
 	mov    0x10(%rsp),%rdi
@@ -6028,22 +6028,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x10(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   9190 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    106a0 <pybind11::array_t<float, 1> (anonymous namespace)::predict<unsigned short>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<unsigned short, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x10(%rsp),%rdx
@@ -6196,22 +6196,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x8(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   9190 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    10960 <pybind11::array_t<float, 1> (anonymous namespace)::predict<int>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	sub    $0x1,%ebp
@@ -6363,22 +6363,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x8(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   9190 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    10c20 <pybind11::array_t<float, 1> (anonymous namespace)::predict<unsigned int>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<unsigned int, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	sub    $0x1,%ebp
@@ -6531,22 +6531,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x8(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   9190 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    10ee0 <pybind11::array_t<float, 1> (anonymous namespace)::predict<bool>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<bool, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x8(%rsp),%rdx
@@ -6700,22 +6700,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x8(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r15d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r15d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r15d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r15d,%esi
 	movslq %esi,%rsi
 	call   9190 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r15d,%ecx
 	cmp    %ebp,%r15d
 	jge    11190 <pybind11::array_t<float, 1> (anonymous namespace)::predict<float>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<float, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x1f0>
 	sub    $0x1,%ebp
@@ -6865,22 +6865,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x10(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   9190 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    11460 <pybind11::array_t<float, 1> (anonymous namespace)::predict<long>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<long, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x10(%rsp),%rdx
@@ -7032,22 +7032,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x10(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   9190 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    11720 <pybind11::array_t<float, 1> (anonymous namespace)::predict<double>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<double, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x10(%rsp),%rdx
@@ -7199,22 +7199,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x8(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   9190 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    119e0 <pybind11::array_t<float, 1> (anonymous namespace)::predict<unsigned char>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<unsigned char, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x8(%rsp),%rdx
@@ -7367,22 +7367,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x8(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   9190 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    11ca0 <pybind11::array_t<float, 1> (anonymous namespace)::predict<signed char>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<signed char, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x8(%rsp),%rdx
```

### Comparing `pylibffm-0.2.3/pylibffm/wrapper.cpython-39-x86_64-linux-gnu.so` & `pylibffm-0.2.4/pylibffm/wrapper.cpython-39-x86_64-linux-gnu.so`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 0% similar despite different names*

#### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 99119abf2651387ce514e14e2323032c8ef0098a
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 5d04bcf77c8e4a9aa25ac1c84dc6f6c0e5dd75e0
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -5701,22 +5701,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x8(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91c0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    101a0 <pybind11::array_t<float, 1> (anonymous namespace)::predict<bool>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<bool, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x8(%rsp),%rdx
@@ -5869,22 +5869,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x8(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91c0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    10460 <pybind11::array_t<float, 1> (anonymous namespace)::predict<int>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	sub    $0x1,%ebp
@@ -6036,22 +6036,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x10(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91c0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    10750 <pybind11::array_t<float, 1> (anonymous namespace)::predict<unsigned long>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<unsigned long, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x230>
 	mov    0x10(%rsp),%rdi
@@ -6216,22 +6216,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x10(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91c0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    10a10 <pybind11::array_t<float, 1> (anonymous namespace)::predict<short>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<short, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x10(%rsp),%rdx
@@ -6384,22 +6384,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x8(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91c0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    10cd0 <pybind11::array_t<float, 1> (anonymous namespace)::predict<signed char>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<signed char, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x8(%rsp),%rdx
@@ -6552,22 +6552,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x10(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91c0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    10f90 <pybind11::array_t<float, 1> (anonymous namespace)::predict<double>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<double, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x10(%rsp),%rdx
@@ -6719,22 +6719,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x10(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91c0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    11250 <pybind11::array_t<float, 1> (anonymous namespace)::predict<unsigned short>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<unsigned short, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x10(%rsp),%rdx
@@ -6887,22 +6887,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x8(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91c0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    11510 <pybind11::array_t<float, 1> (anonymous namespace)::predict<unsigned char>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<unsigned char, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x8(%rsp),%rdx
@@ -7055,22 +7055,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x8(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91c0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    117d0 <pybind11::array_t<float, 1> (anonymous namespace)::predict<unsigned int>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<unsigned int, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	sub    $0x1,%ebp
@@ -7223,22 +7223,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x10(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r14d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r14d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r14d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r14d,%esi
 	movslq %esi,%rsi
 	call   91c0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r14d,%ecx
 	cmp    %ebp,%r14d
 	jge    11a90 <pybind11::array_t<float, 1> (anonymous namespace)::predict<long>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<long, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x200>
 	mov    0x10(%rsp),%rdx
@@ -7391,22 +7391,22 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x8(%rsp),%rax
 	add    $0x4,%rax
 	mov    %rax,0x30(%rsp)
 	lea    0x44(%rsp),%rax
 	mov    %rax,0x38(%rsp)
 	nopl   0x0(%rax,%rax,1)
-	mov    -0x4(%r12),%r15d
 	mov    (%r12),%ebp
+	mov    -0x4(%r12),%r15d
 	pxor   %xmm1,%xmm1
 	movq   $0x0,0x60(%rsp)
 	mov    0x18(%rsp),%rdi
 	movaps %xmm1,0x50(%rsp)
-	mov    %r15d,%esi
-	sub    %ebp,%esi
+	mov    %ebp,%esi
+	sub    %r15d,%esi
 	movslq %esi,%rsi
 	call   91c0 <std::vector<ffm::ffm_node, std::allocator<ffm::ffm_node> >::reserve(unsigned long)@plt>
 	mov    0x58(%rsp),%rsi
 	mov    %r15d,%ecx
 	cmp    %ebp,%r15d
 	jge    11d40 <pybind11::array_t<float, 1> (anonymous namespace)::predict<float>(int, int, int, pybind11::array_t<float, 1>, bool, int, int, pybind11::array_t<int, 1>, pybind11::array_t<float, 1>, pybind11::array_t<int, 1>, pybind11::array_t<int, 1>)+0x1f0>
 	sub    $0x1,%ebp
```

### Comparing `pylibffm-0.2.3/pylibffm.egg-info/PKG-INFO` & `pylibffm-0.2.4/pylibffm.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 Metadata-Version: 2.1
 Name: pylibffm
-Version: 0.2.3
+Version: 0.2.4
 Summary: A library wrapping libffm
 Home-page: https://github.com/Sinacam/pylibffm
 Author: ntumlgroup
 License: MIT License
+Description: # pylibffm
+        
+        pylibffm is a wrapper around libffm to allow using scipy and numpy arrays as input.
+        
+        ## Installing
+        If you're running python 3.7~3.11 on linux
+        ```bash
+        pip install pylibffm
+        ```
+        Otherwise
+        ```bash
+        git clone https://github.com/Sinacam/pylibffm
+        cd pylibffm
+        make
+        pip install .
+        ```
+        Currently, the distribution is incredibly hacky and cannot be pip installed from source.
+        Windows build support is lacking, but code should be correct.
+        
+        ## Documentation
+        The API only consists of
+        + `train`
+        + `load`
+        + `Model`
+            + `Model.save`
+            + `Model.predict`
+        
+        Use `help` or read their docstring for their usage.
+        
+        ## Diff with libffm
+        To be deterministic, set openmp threads to 1. For pylibffm, do
+        ```bash
+        OMP_NUM_THREADS=1 python <script>.py
+        ```
+        
+        For libffm, run with `-s 1` (the default). This should yield identical models.
+Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# pylibffm
-
-pylibffm is a wrapper around libffm to allow using scipy and numpy arrays as input.
-
-## Installing
-If you're running python 3.7~3.11 on linux
-```bash
-pip install pylibffm
-```
-Otherwise
-```bash
-git clone https://github.com/Sinacam/pylibffm
-cd pylibffm
-make
-pip install .
-```
-Currently, the distribution is incredibly hacky and cannot be pip installed from source.
-Windows build support is lacking, but code should be correct.
-
-## Documentation
-The API only consists of
-+ `train`
-+ `load`
-+ `Model`
-    + `Model.save`
-    + `Model.predict`
-
-Use `help` or read their docstring for their usage.
-
-## Diff with libffm
-To be deterministic, set openmp threads to 1. For pylibffm, do
-```bash
-OMP_NUM_THREADS=1 python <script>.py
-```
-
-For libffm, run with `-s 1` (the default). This should yield identical models.
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_zg908nc0_/tmp6_y9cs4d_TarContainer/0/53", line 52, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_zg908nc0_/tmp6_y9cs4d_TarContainer/0/53", line 52, column 0: CDATA terminal not found*

```diff
@@ -1,14 +1,10 @@
-Metadata-Version: 2.1 Name: pylibffm Version: 0.2.3 Summary: A library wrapping
+Metadata-Version: 2.1 Name: pylibffm Version: 0.2.4 Summary: A library wrapping
 libffm Home-page: https://github.com/Sinacam/pylibffm Author: ntumlgroup
-License: MIT License Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Description-Content-Type:
-text/markdown License-File: LICENSE # pylibffm pylibffm is a wrapper around
+License: MIT License Description: # pylibffm pylibffm is a wrapper around
 libffm to allow using scipy and numpy arrays as input. ## Installing If you're
 running python 3.7~3.11 on linux ```bash pip install pylibffm ``` Otherwise
 ```bash git clone https://github.com/Sinacam/pylibffm cd pylibffm make pip
 install . ``` Currently, the distribution is incredibly hacky and cannot be pip
 installed from source. Windows build support is lacking, but code should be
 correct. ## Documentation The API only consists of + `train` + `load` + `Model`
 + `Model.save` + `Model.predict` Use `help` or read their docstring for their
```

### Comparing `pylibffm-0.2.3/setup.py` & `pylibffm-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pathlib
 import setuptools
 
 name = "pylibffm"
-version = "0.2.3"
+version = "0.2.4"
 author = "ntumlgroup"
 license = "MIT License"
 license_file = "LICENSE"
 description = "A library wrapping libffm"
 long_description = (pathlib.Path(__file__).parent / "README.md").read_text()
 long_description_content_type = "text/markdown"
 url = "https://github.com/Sinacam/pylibffm"
```

