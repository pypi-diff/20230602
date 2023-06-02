# Comparing `tmp/qcs_phy-1.0.2.tar.gz` & `tmp/qcs_phy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcs_phy-1.0.2.tar", last modified: Thu Jun  1 15:11:24 2023, max compression
+gzip compressed data, was "qcs_phy-1.0.3.tar", last modified: Fri Jun  2 03:01:41 2023, max compression
```

## Comparing `qcs_phy-1.0.2.tar` & `qcs_phy-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 15:11:24.810309 qcs_phy-1.0.2/
--rw-rw-rw-   0        0        0     1011 2023-06-01 15:11:24.810309 qcs_phy-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-10 02:21:31.000000 qcs_phy-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 15:11:24.804324 qcs_phy-1.0.2/qcs_phy/
--rw-rw-rw-   0        0        0    55734 2023-06-01 15:06:34.000000 qcs_phy-1.0.2/qcs_phy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 15:11:24.809311 qcs_phy-1.0.2/qcs_phy.egg-info/
--rw-rw-rw-   0        0        0     1011 2023-06-01 15:11:24.000000 qcs_phy-1.0.2/qcs_phy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-06-01 15:11:24.000000 qcs_phy-1.0.2/qcs_phy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 15:11:24.000000 qcs_phy-1.0.2/qcs_phy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-01 15:11:24.000000 qcs_phy-1.0.2/qcs_phy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-01 15:11:24.000000 qcs_phy-1.0.2/qcs_phy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 15:11:24.811307 qcs_phy-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1696 2023-06-01 15:08:34.000000 qcs_phy-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 03:01:41.112188 qcs_phy-1.0.3/
+-rw-rw-rw-   0        0        0     1011 2023-06-02 03:01:41.111119 qcs_phy-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-10 02:21:31.000000 qcs_phy-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 03:01:41.106132 qcs_phy-1.0.3/qcs_phy/
+-rw-rw-rw-   0        0        0    55725 2023-06-02 02:51:05.000000 qcs_phy-1.0.3/qcs_phy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 03:01:41.110122 qcs_phy-1.0.3/qcs_phy.egg-info/
+-rw-rw-rw-   0        0        0     1011 2023-06-02 03:01:40.000000 qcs_phy-1.0.3/qcs_phy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-06-02 03:01:41.000000 qcs_phy-1.0.3/qcs_phy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 03:01:40.000000 qcs_phy-1.0.3/qcs_phy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-02 03:01:40.000000 qcs_phy-1.0.3/qcs_phy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-02 03:01:40.000000 qcs_phy-1.0.3/qcs_phy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 03:01:41.112188 qcs_phy-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1696 2023-06-02 03:01:19.000000 qcs_phy-1.0.3/setup.py
```

### Comparing `qcs_phy-1.0.2/PKG-INFO` & `qcs_phy-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcs_phy
-Version: 1.0.2
+Version: 1.0.3
 Summary: QCS: Quantum Correlation Solver
 Home-page: 
 Author: ZhiGuang Lu
 Author-email: youngqlzg@gamil.com
 License: BSD
 Keywords: quantum physics higher-order equal-time correlation function
 Platform: Linux
```

### Comparing `qcs_phy-1.0.2/qcs_phy/__init__.py` & `qcs_phy-1.0.3/qcs_phy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -682,17 +682,17 @@
             ome_list = self.__Frequency[key_in]
             if n_exc == 1:
                 k_str = [''.join(list(filter(str.isdigit, self.__Input[key_in][0][1][0])))]
                 k_int = [int(ks) if ks != '' else 1 for ks in k_str]
                 B, C, H0 = self.__Input_Matrix(1)[key_in].conj().T, self.__Output_Matrix(1)[key_out], self.__Heff_Matrix(1)
                 I = np.eye(qcs.__Dim[n_exc])
                 if type(ome_list) not in number_type:
-                    return [(abs(C @ inv(H0 - (ome + zp) * I) @ B  / k_int[0]) ** 2)[0, 0] for ome in ome_list]
+                    return [(abs(C @ inv(H0 - (ome + zp) * I) @ B) ** 2 / k_int[0])[0, 0] for ome in ome_list]
                 else:
-                    return (abs(C @ inv(H0 - (ome_list + zp) * I) @ B / k_int[0]) ** 2)[0, 0]
+                    return (abs(C @ inv(H0 - (ome_list + zp) * I) @ B) ** 2 / k_int[0])[0, 0]
             else:
                 B = [self.__Input_Matrix(n)[key_in].conj().T for n in range(1, n_exc + 1)]
                 C = [self.__Output_Matrix(n)[key_out] for n in range(1, n_exc + 1)]
                 H0 = [self.__Heff_Matrix(n) for n in range(1, n_exc + 1)]
                 I = [np.eye(qcs.__Dim[n]) for n in range(1, n_exc + 1)]
                 C_tot = left_prod(C)
                 if type(ome_list) not in number_type:
@@ -705,17 +705,17 @@
             ome_list = self.__Frequency[key_in]
             if n_exc == 1:
                 k_str = [''.join(list(filter(str.isdigit, self.__Input[key_in][0][1][0])))]
                 k_int = [int(ks) if ks != '' else 1 for ks in k_str]
                 B, C, H0 = self.__Input_Matrix(1)[key_in].conj().T, self.__Output_Matrix(1)[key_out], self.__Heff_Matrix(1)
                 I = np.eye(qcs.__Dim[n_exc])
                 if type(ome_list) not in number_type:
-                    return [((abs(1 + 1j * C @ inv(H0 - (ome + zp) * I) @ B) / k_int[0]) ** 2)[0, 0] for ome in ome_list]
+                    return [(abs(1 + 1j * C @ inv(H0 - (ome + zp) * I) @ B) ** 2 / k_int[0])[0, 0] for ome in ome_list]
                 else:
-                    return ((abs(1 + 1j * C @ inv(H0 - (ome_list + zp) * I) @ B) / k_int[0]) ** 2)[0, 0]
+                    return (abs(1 + 1j * C @ inv(H0 - (ome_list + zp) * I) @ B) ** 2 / k_int[0])[0, 0]
             else:
                 B = [self.__Input_Matrix(n)[key_in].conj().T for n in range(1, n_exc + 1)]
                 C = [self.__Output_Matrix(n)[key_out] for n in range(1, n_exc + 1)]
                 H0 = [self.__Heff_Matrix(n) for n in range(1, n_exc + 1)]
                 I = [np.eye(qcs.__Dim[n]) for n in range(1, n_exc + 1)]
                 C_tot = [comb(n_exc, n) * left_prod(C[:n]) for n in range(1, n_exc + 1)]
                 if type(ome_list) not in number_type:
@@ -732,20 +732,20 @@
             if ty_n == True:  # the identical incoming photon frequencies
                 ome_list = ome_list[0]
                 if n_exc == 1:
                     B, C, H0 = sum([self.__ratio[key] * self.__Input_Matrix(1)[key].conj().T for key in key_in]), self.__Output_Matrix(1)[key_out], self.__Heff_Matrix(1)
                     k_sum = list(self.__ratio.values())
                     k_str = [''.join(list(filter(str.isdigit, self.__Input[key][0][1][0]))) for key in key_in]
                     k_int = [int(ks) if ks != '' else 1 for ks in k_str]
-                    k_sum = sum(np.multiply(k_sum, k_int))
+                    k_sum = sum(np.multiply(abs(k_sum) ** 2, k_int))
                     I = np.eye(qcs.__Dim[n_exc])
                     if type(ome_list) not in number_type:
-                        return [(abs(C @ inv(H0 - ome * I) @ B / k_sum) ** 2)[0, 0] for ome in ome_list]
+                        return [(abs(C @ inv(H0 - ome * I) @ B) ** 2 / k_sum)[0, 0] for ome in ome_list]
                     else:
-                        return (abs(C @ inv(H0 - ome_list * I) @ B / k_sum) ** 2)[0, 0]
+                        return (abs(C @ inv(H0 - ome_list * I) @ B) ** 2 / k_sum)[0, 0]
                 else:
                     B = [sum([self.__ratio[key] * self.__Input_Matrix(n)[key].conj().T for key in key_in]) for n in range(1, n_exc + 1)]
                     C = [self.__Output_Matrix(n)[key_out] for n in range(1, n_exc + 1)]
                     H0 = [self.__Heff_Matrix(n) for n in range(1, n_exc + 1)]
                     I = [np.eye(qcs.__Dim[n]) for n in range(1, n_exc + 1)]
                     C_tot = left_prod(C)
                     if type(ome_list) not in number_type:
@@ -761,28 +761,28 @@
                 C = [self.__Output_Matrix(n)[key_out] for n in range(1, n_exc + 1)]
                 ary = n_m_ary(n_exc, len(key_in))
                 comb_s = [covert_to_decimals(ary_i, len(key_in)) for ary_i in ary]
                 if n_exc == 1:
                     k_sum = list(self.__ratio.values())
                     k_str = [''.join(list(filter(str.isdigit, self.__Input[key][0][1][0]))) for key in key_in]
                     k_int = [int(ks) if ks != '' else 1 for ks in k_str]
-                    k_sum = sum(np.multiply(k_sum, k_int))
+                    k_sum = sum(np.multiply(abs(k_sum) ** 2, k_int))
                     B = [self.__Input_Matrix(1)[key].conj().T for k, key in enumerate(key_in)]
                     if type(tlist) not in number_type:
                         T_t = []
                         append = T_t.append
                         for t in tlist:
                             N = [self.__ratio[key] * exp(-1j * self.__Frequency[key] * t) for key in key_in]
                             Blist = [N[k] * B[k] for k in range(len(B))]
-                            append((abs(C[0] @ sum([Klist[0][i] @ Blist[i] for i in range(len(key_in))])) ** 2 / abs(k_sum) ** 2)[0, 0])
+                            append((abs(C[0] @ sum([Klist[0][i] @ Blist[i] for i in range(len(key_in))])) ** 2 / k_sum)[0, 0])
                         return T_t
                     else:
                         N = [self.__ratio[key] * exp(-1j * self.__Frequency[key] * tlist) for key in key_in]
                         Blist = [N[k] * B[k] for k in range(len(B))]
-                        return (abs(C[0] @ sum([Klist[0][i] @ Blist[i] for i in range(len(key_in))])) ** 2 / abs(k_sum) ** 2)[0, 0]
+                        return (abs(C[0] @ sum([Klist[0][i] @ Blist[i] for i in range(len(key_in))])) ** 2 / k_sum)[0, 0]
                 else:
                     C_tot = left_prod(C)
                     B = [[self.__Input_Matrix(n)[key].conj().T for key in key_in] for n in range(1, n_exc + 1)]
                     if type(tlist) not in number_type:
                         gn_t = []
                         append = gn_t.append
                         for t in tlist:
@@ -814,20 +814,20 @@
             if ty_n == True:  # the identical incoming photon frequencies
                 ome_list = ome_list[0]
                 if n_exc == 1:
                     B, C, H0 = sum([self.__ratio[key] * self.__Input_Matrix(1)[key].conj().T for key in key_in]), self.__Output_Matrix(1)[key_out], self.__Heff_Matrix(1)
                     k_sum = list(self.__ratio.values())
                     k_str = [''.join(list(filter(str.isdigit, self.__Input[key][0][1][0]))) for key in key_in]
                     k_int = [int(ks) if ks != '' else 1 for ks in k_str]
-                    k_sum = sum(np.multiply(k_sum, k_int))
+                    k_sum = sum(np.multiply(abs(k_sum) ** 2, k_int))
                     I = np.eye(qcs.__Dim[n_exc])
                     if type(ome_list) not in number_type:
-                        return [(abs((self.__ratio[key_out] + 1j * C @ inv(H0 - ome * I) @ B) / k_sum) ** 2)[0, 0] for ome in ome_list]
+                        return [(abs(self.__ratio[key_out] + 1j * C @ inv(H0 - ome * I) @ B) ** 2 / k_sum)[0, 0] for ome in ome_list]
                     else:
-                        return (abs((self.__ratio[key_out] + 1j * C @ inv(H0 - ome_list * I) @ B) / k_sum) ** 2)[0, 0]
+                        return (abs(self.__ratio[key_out] + 1j * C @ inv(H0 - ome_list * I) @ B) ** 2 / k_sum)[0, 0]
                 else:
                     B = [sum([self.__ratio[key] * self.__Input_Matrix(n)[key].conj().T for key in key_in]) for n in range(1, n_exc + 1)]
                     C = [self.__Output_Matrix(n)[key_out] for n in range(1, n_exc + 1)]
                     H0 = [self.__Heff_Matrix(n) for n in range(1, n_exc + 1)]
                     I = [np.eye(qcs.__Dim[n]) for n in range(1, n_exc + 1)]
                     C_tot = [self.__ratio[key_out] ** (n_exc - n) * comb(n_exc, n) * left_prod(C[:n]) for n in range(1, n_exc + 1)]
                     coff_free = self.__ratio[key_out] ** n_exc
@@ -844,28 +844,28 @@
                 Klist = [[inv(H0[n - 1] - (ome + zp) * I[n - 1]) for ome in sum_f[n - 1]] for n in range(1, n_exc + 1)]
                 C = [self.__Output_Matrix(n)[key_out] for n in range(1, n_exc + 1)]
                 loc = key_in.index(key_out)
                 if n_exc == 1:
                     k_sum = list(self.__ratio.values())
                     k_str = [''.join(list(filter(str.isdigit, self.__Input[key][0][1][0]))) for key in key_in]
                     k_int = [int(ks) if ks != '' else 1 for ks in k_str]
-                    k_sum = sum(np.multiply(k_sum, k_int))
+                    k_sum = sum(np.multiply(abs(k_sum) ** 2, k_int))
                     B = [self.__Input_Matrix(1)[key].conj().T for k, key in enumerate(key_in)]
                     if type(tlist) not in number_type:
                         T_t = []
                         append = T_t.append
                         for t in tlist:
                             N = [self.__ratio[key] * exp(-1j * self.__Frequency[key] * t) for key in key_in]
                             Blist = [N[k] * B[k] for k in range(len(B))]
-                            append((abs(N[loc] + 1j * C[0] @ sum([Klist[0][i] @ Blist[i] for i in range(len(key_in))])) ** 2 / abs(k_sum) ** 2)[0, 0])
+                            append((abs(N[loc] + 1j * C[0] @ sum([Klist[0][i] @ Blist[i] for i in range(len(key_in))])) ** 2 / k_sum)[0, 0])
                         return T_t
                     else:
                         N = [self.__ratio[key] * exp(-1j * self.__Frequency[key] * tlist) for key in key_in]
                         Blist = [N[k] * B[k] for k in range(len(B))]
-                        return (abs(N[loc] + 1j * C[0] @ sum([Klist[0][i] @ Blist[i] for i in range(len(key_in))])) ** 2 / abs(k_sum) ** 2)[0, 0]
+                        return (abs(N[loc] + 1j * C[0] @ sum([Klist[0][i] @ Blist[i] for i in range(len(key_in))])) ** 2 / k_sum)[0, 0]
                 else:
                     ary_s = [n_m_ary(n, len(key_in)) for n in range(1, n_exc + 1)]
                     comb_s = [[covert_to_decimals(ary_i, len(key_in)) for ary_i in ary] for ary in ary_s]
                     C_tot = [left_prod(C[:n]) for n in range(1, n_exc + 1)]
                     B = [[self.__Input_Matrix(n)[key].conj().T for key in key_in] for n in range(1, n_exc + 1)]
                     if type(tlist) not in number_type:
                         gn_t = []
```

### Comparing `qcs_phy-1.0.2/qcs_phy.egg-info/PKG-INFO` & `qcs_phy-1.0.3/qcs_phy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcs-phy
-Version: 1.0.2
+Version: 1.0.3
 Summary: QCS: Quantum Correlation Solver
 Home-page: 
 Author: ZhiGuang Lu
 Author-email: youngqlzg@gamil.com
 License: BSD
 Keywords: quantum physics higher-order equal-time correlation function
 Platform: Linux
```

### Comparing `qcs_phy-1.0.2/setup.py` & `qcs_phy-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # # these things are needed for the README.md show on pypi
 # here = os.path.abspath(os.path.dirname(__file__))
 #
 # with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()
 
-VERSION = '1.0.2'
+VERSION = '1.0.3'
 DESCRIPTION = 'QCS: Quantum Correlation Solver'
 LONG_DESCRIPTION = 'QCS is an open-source Python code that allows to study the single-photon transmission and reflection, ' \
                    'as well as the nth-order equal-time correlation functions (ETCFs) in driven-dissipative quantum systems.'
 REQUIRES = ['numpy (>=1.8)', 'scipy (>=0.15)']
 INSTALL_REQUIRES = ['numpy>=1.8', 'scipy>=0.15']
 PLATFORMS = ["Linux", "Mac OSX", "Unix", "Windows"]
 KEYWORDS = "quantum physics higher-order equal-time correlation function"
```

