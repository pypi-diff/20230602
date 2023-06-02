# Comparing `tmp/binsreg-2.0.1.tar.gz` & `tmp/binsreg-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/rmasini/Dropbox/binsreg/Python/binsreg/dist/.tmp-n2_kagxg/binsreg-2.0.1.tar", last modified: Sun Mar 19 16:51:55 2023, max compression
+gzip compressed data, was "/Users/rmasini/Dropbox/binsreg/Python/binsreg/dist/.tmp-_s3g92e7/binsreg-2.0.2.tar", last modified: Fri Jun  2 17:45:44 2023, max compression
```

## Comparing `binsreg-2.0.1.tar` & `binsreg-2.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-03-19 16:51:55.211243 binsreg-2.0.1/
--rw-r--r--   0 rmasini    (501) staff       (20)     3829 2023-03-19 16:51:55.211424 binsreg-2.0.1/PKG-INFO
--rw-r--r--   0 rmasini    (501) staff       (20)     3232 2023-03-19 16:41:53.000000 binsreg-2.0.1/README.md
--rw-r--r--   0 rmasini    (501) staff       (20)      108 2021-09-05 04:38:28.000000 binsreg-2.0.1/pyproject.toml
--rw-r--r--   0 rmasini    (501) staff       (20)      808 2023-03-19 16:51:55.212315 binsreg-2.0.1/setup.cfg
-drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-03-19 16:51:55.155338 binsreg-2.0.1/src/
-drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-03-19 16:51:55.202025 binsreg-2.0.1/src/binsreg/
--rw-r--r--   0 rmasini    (501) staff       (20)      189 2021-09-05 04:38:11.000000 binsreg-2.0.1/src/binsreg/__init__.py
--rw-r--r--   0 rmasini    (501) staff       (20)    78748 2023-03-19 16:50:05.000000 binsreg-2.0.1/src/binsreg/binsglm.py
--rw-r--r--   0 rmasini    (501) staff       (20)    42114 2023-03-19 16:50:34.000000 binsreg-2.0.1/src/binsreg/binspwc.py
--rw-r--r--   0 rmasini    (501) staff       (20)    72025 2023-03-19 16:50:14.000000 binsreg-2.0.1/src/binsreg/binsqreg.py
--rw-r--r--   0 rmasini    (501) staff       (20)    71509 2023-03-19 16:49:54.000000 binsreg-2.0.1/src/binsreg/binsreg.py
--rw-r--r--   0 rmasini    (501) staff       (20)    24480 2023-03-19 16:51:01.000000 binsreg-2.0.1/src/binsreg/binsregselect.py
--rw-r--r--   0 rmasini    (501) staff       (20)    46034 2023-03-19 16:50:26.000000 binsreg-2.0.1/src/binsreg/binstest.py
--rw-r--r--   0 rmasini    (501) staff       (20)    59921 2023-03-17 14:33:38.000000 binsreg-2.0.1/src/binsreg/funs.py
-drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-03-19 16:51:55.208250 binsreg-2.0.1/src/binsreg.egg-info/
--rw-r--r--   0 rmasini    (501) staff       (20)     3829 2023-03-19 16:51:55.000000 binsreg-2.0.1/src/binsreg.egg-info/PKG-INFO
--rw-r--r--   0 rmasini    (501) staff       (20)      433 2023-03-19 16:51:55.000000 binsreg-2.0.1/src/binsreg.egg-info/SOURCES.txt
--rw-r--r--   0 rmasini    (501) staff       (20)        1 2023-03-19 16:51:55.000000 binsreg-2.0.1/src/binsreg.egg-info/dependency_links.txt
--rw-r--r--   0 rmasini    (501) staff       (20)       40 2023-03-19 16:51:55.000000 binsreg-2.0.1/src/binsreg.egg-info/requires.txt
--rw-r--r--   0 rmasini    (501) staff       (20)        8 2023-03-19 16:51:55.000000 binsreg-2.0.1/src/binsreg.egg-info/top_level.txt
-drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-03-19 16:51:55.210592 binsreg-2.0.1/test/
--rw-r--r--   0 rmasini    (501) staff       (20)     5008 2021-09-06 17:46:18.000000 binsreg-2.0.1/test/test_funs.py
--rw-r--r--   0 rmasini    (501) staff       (20)     7212 2023-03-17 17:09:40.000000 binsreg-2.0.1/test/test_pkg.py
+drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-06-02 17:45:44.163064 binsreg-2.0.2/
+-rw-r--r--   0 rmasini    (501) staff       (20)     3829 2023-06-02 17:45:44.163304 binsreg-2.0.2/PKG-INFO
+-rw-r--r--   0 rmasini    (501) staff       (20)     3232 2023-03-19 16:41:53.000000 binsreg-2.0.2/README.md
+-rw-r--r--   0 rmasini    (501) staff       (20)      108 2021-09-05 04:38:28.000000 binsreg-2.0.2/pyproject.toml
+-rw-r--r--   0 rmasini    (501) staff       (20)      823 2023-06-02 17:45:44.164517 binsreg-2.0.2/setup.cfg
+drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-06-02 17:45:44.121616 binsreg-2.0.2/src/
+drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-06-02 17:45:44.154708 binsreg-2.0.2/src/binsreg/
+-rw-r--r--   0 rmasini    (501) staff       (20)      189 2021-09-05 04:38:11.000000 binsreg-2.0.2/src/binsreg/__init__.py
+-rw-r--r--   0 rmasini    (501) staff       (20)    78872 2023-06-02 17:37:44.000000 binsreg-2.0.2/src/binsreg/binsglm.py
+-rw-r--r--   0 rmasini    (501) staff       (20)    42236 2023-06-02 17:45:11.000000 binsreg-2.0.2/src/binsreg/binspwc.py
+-rw-r--r--   0 rmasini    (501) staff       (20)    72147 2023-06-02 17:37:50.000000 binsreg-2.0.2/src/binsreg/binsqreg.py
+-rw-r--r--   0 rmasini    (501) staff       (20)    71631 2023-06-02 17:37:37.000000 binsreg-2.0.2/src/binsreg/binsreg.py
+-rw-r--r--   0 rmasini    (501) staff       (20)    24602 2023-06-02 17:37:27.000000 binsreg-2.0.2/src/binsreg/binsregselect.py
+-rw-r--r--   0 rmasini    (501) staff       (20)    46156 2023-06-02 17:41:48.000000 binsreg-2.0.2/src/binsreg/binstest.py
+-rw-r--r--   0 rmasini    (501) staff       (20)    60005 2023-06-02 17:38:02.000000 binsreg-2.0.2/src/binsreg/funs.py
+drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-06-02 17:45:44.159072 binsreg-2.0.2/src/binsreg.egg-info/
+-rw-r--r--   0 rmasini    (501) staff       (20)     3829 2023-06-02 17:45:44.000000 binsreg-2.0.2/src/binsreg.egg-info/PKG-INFO
+-rw-r--r--   0 rmasini    (501) staff       (20)      433 2023-06-02 17:45:44.000000 binsreg-2.0.2/src/binsreg.egg-info/SOURCES.txt
+-rw-r--r--   0 rmasini    (501) staff       (20)        1 2023-06-02 17:45:44.000000 binsreg-2.0.2/src/binsreg.egg-info/dependency_links.txt
+-rw-r--r--   0 rmasini    (501) staff       (20)       55 2023-06-02 17:45:44.000000 binsreg-2.0.2/src/binsreg.egg-info/requires.txt
+-rw-r--r--   0 rmasini    (501) staff       (20)        8 2023-06-02 17:45:44.000000 binsreg-2.0.2/src/binsreg.egg-info/top_level.txt
+drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2023-06-02 17:45:44.160980 binsreg-2.0.2/test/
+-rw-r--r--   0 rmasini    (501) staff       (20)     5008 2021-09-06 17:46:18.000000 binsreg-2.0.2/test/test_funs.py
+-rw-r--r--   0 rmasini    (501) staff       (20)     8799 2023-06-02 17:40:13.000000 binsreg-2.0.2/test/test_pkg.py
```

### Comparing `binsreg-2.0.1/PKG-INFO` & `binsreg-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binsreg
-Version: 2.0.1
+Version: 2.0.2
 Summary: Implements binscatter methods, including partition selection, point estimation, pointwise and uniform inference methods, and graphical procedures.
 Home-page: https://github.com/nppackages/binsreg
 Author: Ricardo Masini
 Author-email: rmasini@princeton.edu
 Project-URL: Bug Tracker, https://github.com/nppackages/binsreg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `binsreg-2.0.1/README.md` & `binsreg-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `binsreg-2.0.1/setup.cfg` & `binsreg-2.0.2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = binsreg
-version = 2.0.1
+version = 2.0.2
 author = Ricardo Masini
 author_email = rmasini@princeton.edu
 description = Implements binscatter methods, including partition selection, point estimation, pointwise and uniform inference methods, and graphical procedures.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nppackages/binsreg
 project_urls = 
@@ -17,17 +17,17 @@
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	numpy
-	pandas
+	pandas>=2.0.0
 	scipy
-	statsmodels
+	statsmodels>=0.14.0
 	plotnine
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build =
```

### Comparing `binsreg-2.0.1/src/binsreg/binsglm.py` & `binsreg-2.0.2/src/binsreg/binsglm.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         all factor variables (if specified) are excluded from the evaluation (set as zero).
 
     dist : str
         Distribution of the error term. Possible values are "Gaussian" (default),"Binomial","Gamma","Poisson".
         For furher options refer to statsmodels package documentation.
 
     link : str
-        Link function to be used together with dist. Possible values are "identity","logit","log","probit".
+        Link function to be used together with dist. Possible values are "Identity","Logit","Log","Probit".
         The default is link = None, in that case the default link dor the specified dist is used. 
         For furher options and details refer to statsmodels package documentation.
     
     nolink : bool
         If true, the function within the inverse link function is reported instead of the conditional mean function for the outcome.
 
     deriv : int 
@@ -387,14 +387,15 @@
     if w is not None:
         w = np.array(w).reshape(len(w),-1)
         nwvar = ncol(w)
     else: nwvar = 0
     if by is not None:
         by = np.array(by).reshape(len(by),-1)
     if cluster is not None:
+        warnings.warn("cluster-robust standard error not implemented in statsmodel.api; HC standard error used instead.")
         cluster = np.array(cluster).reshape(len(cluster),-1)
     if weights is not None:
         weights = np.array(weights).reshape(len(weights),-1)
 
     # extract subset
     if subset is not None:
         subset = np.array(subset).reshape(-1)
@@ -432,15 +433,15 @@
     if at is None: at = "mean"
 
     ### extract family obj using dist and link
     if link is None: 
         family_str = f'sm.families.{dist}()'
         link = 'default'
     else: 
-        family_str = f'sm.families.{dist}(sm.families.links.{link})'
+        family_str = f'sm.families.{dist}(sm.families.links.{link}())'
     
     family = eval(family_str)
     linkinv = family.link.inverse
     linkinv_1 = family.link.inverse_deriv
     linkinv_2 = family.link.inverse_deriv2
 
     ##########################################
```

### Comparing `binsreg-2.0.1/src/binsreg/binspwc.py` & `binsreg-2.0.2/src/binsreg/binspwc.py`

 * *Files 0% similar despite different names*

```diff
@@ -304,14 +304,15 @@
     if w is not None:
         w = np.array(w).reshape(len(w),-1)
         nwvar = ncol(w)
     else: nwvar = 0
     if by is not None:
         by = np.array(by).reshape(len(by),-1)
     if cluster is not None:
+        warnings.warn("cluster-robust standard error not implemented in statsmodel.api; HC standard error used instead.")
         cluster = np.array(cluster).reshape(len(cluster),-1)
     if weights is not None:
         weights = np.array(weights).reshape(len(weights),-1)
 
     # extract subset
     if subset is not None:
         subset = np.array(subset).reshape(-1)
```

### Comparing `binsreg-2.0.1/src/binsreg/binsqreg.py` & `binsreg-2.0.2/src/binsreg/binsqreg.py`

 * *Files 0% similar despite different names*

```diff
@@ -377,14 +377,15 @@
     if w is not None:
         w = np.array(w).reshape(len(w),-1)
         nwvar = ncol(w)
     else: nwvar = 0
     if by is not None:
         by = np.array(by).reshape(len(by),-1)
     if cluster is not None:
+        warnings.warn("cluster-robust standard error not implemented in statsmodel.api; HC standard error used instead.")
         cluster = np.array(cluster).reshape(len(cluster),-1)
     if weights is not None:
         weights = np.array(weights).reshape(len(weights),-1)
 
     # extract subset
     if subset is not None:
         subset = np.array(subset).reshape(-1)
```

### Comparing `binsreg-2.0.1/src/binsreg/binsreg.py` & `binsreg-2.0.2/src/binsreg/binsreg.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,14 +370,15 @@
     if w is not None:
         w = np.array(w).reshape(len(w),-1)
         nwvar = ncol(w)
     else: nwvar = 0
     if by is not None:
         by = np.array(by).reshape(len(by),-1)
     if cluster is not None:
+        warnings.warn("cluster-robust standard error not implemented in statsmodel.api; HC standard error used instead.")
         cluster = np.array(cluster).reshape(len(cluster),-1)
     if weights is not None:
         weights = np.array(weights).reshape(len(weights),-1)
 
     # extract subset
     if subset is not None:
         subset = np.array(subset).reshape(-1)
@@ -644,16 +645,16 @@
     if selection=="J":
         if ((ci_p is not None) and (ci_p<=dots_p)):
             ci_p = dots_p+1 
             ci_s = ci_p
             warnings.warn("Degree for ci has been changed. It must be greater than the degree for dots.")
 
         if ((cb_p is not None) and (cb_p<=dots_p)):
-            cb_p = dots.p+1
-            cb_s = cb.p
+            cb_p = dots_p+1
+            cb_s = cb_p
             warnings.warn("Degree for cb has been changed. It must be greater than the degree for dots.")
         
     if selection=="U":
         if ((ci is not None) or (cb is not None)):
             warnings.warn("Confidence intervals/bands are valid when nbins is much larger than the IMSE-optimal choice.")
 
     localcheck = massadj = True
```

### Comparing `binsreg-2.0.1/src/binsreg/binsregselect.py` & `binsreg-2.0.2/src/binsreg/binsregselect.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,14 +245,15 @@
     x = np.array(x).reshape(-1,1)
     y = np.array(y).reshape(-1,1)
     if w is not None:
         w = np.array(w).reshape(len(w),-1)
         nwvar = ncol(w)
     else: nwvar = 0
     if cluster is not None:
+        warnings.warn("cluster-robust standard error not implemented in statsmodel.api; HC standard error used instead.")
         cluster = np.array(cluster).reshape(len(cluster),-1)
     if weights is not None:
         weights = np.array(weights).reshape(len(weights),-1)
 
     # extract subset
     if subset is not None:
         subset = np.array(subset).reshape(-1)
```

### Comparing `binsreg-2.0.1/src/binsreg/binstest.py` & `binsreg-2.0.2/src/binsreg/binstest.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,14 +316,15 @@
     x = np.array(x).reshape(-1,1)
     y = np.array(y).reshape(-1,1)
     if w is not None:
         w = np.array(w).reshape(len(w),-1)
         nwvar = ncol(w)
     else: nwvar = 0
     if cluster is not None:
+        warnings.warn("cluster-robust standard error not implemented in statsmodel.api; HC standard error used instead.")
         cluster = np.array(cluster).reshape(len(cluster),-1)
     if weights is not None:
         weights = np.array(weights).reshape(len(weights),-1)
 
     # extract subset
     if subset is not None:
         subset = np.array(subset).reshape(-1)
```

### Comparing `binsreg-2.0.1/src/binsreg/funs.py` & `binsreg-2.0.2/src/binsreg/funs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1119,15 +1119,15 @@
 # slightly modified mean function
 def binsreg_summ(x, w = None, std=False):
     sig = np.nan
     if w is None:
         mu = np.mean(x)
         if std: sig = np.std(x,ddof = 1)
     else:
-        mu = np.average(x, weights=w)
+        mu = np.average(x,weights = w)
         if std: sig = np.sqrt(np.sum(w*(x-mu)**2)/(np.sum(w)-1))
     return mu, sig
 
 # IMSE V constant
 def imse_vcons(p, deriv):
     n = p + 1
     V = 1/np.array([np.arange(j,n+j) for j in range(1,n+1)])
@@ -1167,40 +1167,41 @@
     x_p = nanmat(N, p+qrot+1)
     for j in range(p+qrot+1):  x_p[:,j] = (x**j).reshape(-1)
     if w is not None: P = np.column_stack((x_p, w))
     else: P = x_p
 
     est = binsreg_fit(y, P, weights = weights)
     beta = est.params
-    est = est.fittedvalues
+    est = est.fittedvalues.reshape(-1,1)
 
     # variance constant
-    s2 =  binsreg_fit(y**2, P, weights = weights).fittedvalues - est**2
+    s2 =  binsreg_fit(y**2, P, weights = weights).fittedvalues.reshape(-1,1) - est**2
     if norotnorm: fz = 1
     else:
         mu, sig = binsreg_summ(x, w=weights, std=True)
         fz = norm.pdf(x, loc = mu, scale = sig)
         # trim density from below
         cutval = norm.pdf(norm.ppf(den_alpha)*sig, loc = 0, scale = sig)
         fz[fz<cutval] = cutval
-        fz = fz.reshape(-1,)
+        fz = fz.reshape(-1,1)
     if es: s2 = s2 / fz
     else: s2 = s2 * (fz**(2*deriv))
-    s2 = binsreg_summ(s2, w = weights, std=False)[0]
+    s2v = s2.reshape(-1,1)
+    s2 = binsreg_summ(s2v, w = weights, std=False)[0]
     vcons = imse_vcons(p, deriv)
     imse_v = vcons * s2
 
     # bias constant
     bcons = imse_bcons(p, deriv = deriv, s=0)
     mu_m_hat = 0
     for j in range(p,p+qrot):
         mu_m_hat +=  x**(j-p)*beta[j+1]*np.math.factorial(j+1)/np.math.factorial(j-p)
     mu_m_hat = mu_m_hat**2
     if not es:
-        mu_m_hat = mu_m_hat / (fz**(2*ord-2*deriv))
+        mu_m_hat = mu_m_hat/(fz.reshape(-1,1)**(2*ord-2*deriv))
     imse_b = bcons * binsreg_summ(mu_m_hat, w=weights, std=False)[0]
     aux000num = imse_b*2*(ord-deriv)
     aux000dem = imse_v*(1+2*deriv)
     aux000 = aux000num/aux000dem
     aux00 = aux000**(1/(2*ord+1))
     aux0 = aux00 * eN**(1/(2*ord+1))
     aux1 = np.ceil(aux0)
@@ -1246,15 +1247,15 @@
     else: basis = B
     if w is not None: P = np.column_stack((B, w))
     else: P = B
     model  = binsreg_fit(y, P, weights = weights, cov_type=vce, cluster=cluster)
     pos = np.invert(np.isnan(model.params[:k]))
     k_new = np.sum(pos)
     vcv = model.cov_params()[:k_new,:k_new]
-    m_s2 = binsreg_summ(np.sum(np.matmul(basis[:,pos], vcv) * basis[:,pos],1), w=weights, std=False)[0]
+    m_s2 = binsreg_summ(np.sum(np.matmul(basis[:,pos], vcv) * basis[:,pos],1).reshape(-1,1), w=weights, std=False)[0]
     return m_s2
 
 
 def genB(y, x, w, p, s, deriv, knot, weights=None):
     B  = binsreg_spdes(x=x, p=p+1, s=s+1, knot=knot, deriv=0)  # use smoothest spline
     k  = ncol(B)
     if w is not None: P = np.column_stack((B, w))
```

### Comparing `binsreg-2.0.1/src/binsreg.egg-info/PKG-INFO` & `binsreg-2.0.2/src/binsreg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binsreg
-Version: 2.0.1
+Version: 2.0.2
 Summary: Implements binscatter methods, including partition selection, point estimation, pointwise and uniform inference methods, and graphical procedures.
 Home-page: https://github.com/nppackages/binsreg
 Author: Ricardo Masini
 Author-email: rmasini@princeton.edu
 Project-URL: Bug Tracker, https://github.com/nppackages/binsreg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `binsreg-2.0.1/test/test_funs.py` & `binsreg-2.0.2/test/test_funs.py`

 * *Files identical despite different names*

### Comparing `binsreg-2.0.1/test/test_pkg.py` & `binsreg-2.0.2/test/test_pkg.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,30 @@
 # -*- coding: utf-8 -*-
 """
 TEST SUIT FOR BINSREG
 
 @author: rmasini
 """
 
+
+# LIST of ISSUES:
+# • Line 439 of binsglm.py should read: family_str = f’sm.families.{dist}(sm.families.links.{link}())’. IT CHANGED FOR THE NEW VERSION OF STAT MODELS (0.14.0)
+# • The “link” parameter string should be title-cased, or user should be instructed to supply it in this way.  IT CHANGED FOR THE NEW VERSION OF STAT MODELS (0.14.0)
+# • “at” parameter does not seem to be evaluating at the correct point, very different behavior in R and Python. TESTED ALL CONFIGURATION. MATCHS R IN THE SIMULATION FILE
+# • “polyreg” > 1 has very different behavior in R and Python, does not seem to be fitting the curve correctly. TESTED ALL POLYREGS UP TO 5. THEY ALL MATCH R'S CONTERPART
+# • When “nbins” is not specified and “weights” are supplied, we run into the following error: TypeError: Axis must be specified when shapes of a
+# and weights differ. DONE!
+# • “cluster” errors when Pandas series of Numpy array is supplied as the cluster id. CLUSTER SD ARE NOT IMPLEMENTED IN STATMODELS API
+# • When “nbins” is not specified (i.e. optimal setup), we are unable to handle large numbers of covariates, consider including sparse matrix
+# functionality when “w” is large. I COULD RUN UP TO 900 COVARIATES (WITH 1000 OBSERVATIONS) WITH NO PROBLEM.
+# • Include error message when “cb=(0,0)” is specified. DONE!
+
+# NOTE:  Once you update to Pandas 2.0.2, things stop working. Need to change indexes and update stat model (0.14.0). Now things run fine.
+
+
 import numpy as np
 import pandas as pd
 import time
 
 ####### To install the package from PyPi ##########
 # (in terminal) pip install binsreg
 # from binsreg import *
@@ -19,29 +35,28 @@
 # (in terminal) pip install -i https://test.pypi.org/simple/ binsreg==X.X.X
 # from binsreg import *
 #############################################################################
 
 ####### To install the package locally ###############################
 # (in terminal) pip uninstall binsreg
 # (in terminal) python3 -m pip install ./dist/binsreg-X.X.X.tar.gz
-# from binsreg import *
+from binsreg import *
 #######################################################################
 
 ########## To run from the source ##################################################
 # (in terminal) pip uninstall binsreg
-import sys
-import numpy as np
-sys.path.insert(0, '/Users/rmasini/Dropbox/binsreg/Python/binsreg/src/binsreg')
-from binsregselect import binsregselect
-from binsreg import binsreg
-from binsglm import binsglm
-from binsqreg import binsqreg
-from binstest import binstest
-from binspwc import binspwc
-from funs import *
+# import sys
+# sys.path.insert(0, '/Users/rmasini/Dropbox/binsreg/Python/binsreg/src/binsreg')
+# from binsregselect import binsregselect
+# from binsreg import binsreg
+# from binsglm import binsglm
+# from binsqreg import binsqreg
+# from binstest import binstest
+# from binspwc import binspwc
+# from funs import *
 ###################################################################################
 
 
 # NEW Issues:
 # Condition on the line, CI and CB output of binsreg will never evaluate to False because it is a matrix on NAs
 
 
@@ -67,193 +82,210 @@
 # 6) binsregselect uses cluster = x as default. Is that expected?
 # 7) Vcov of quantile regrssion does not change with vce changes. Probably not yet implemented in statmodels
 
 # TO DO:
 # 1) Fix the link to the papers in PyPi description
 # 2) Fix the links to the illustration file and simulated data
 
-#############################
-#### Test Binsregselect #####
-#############################
+############################
+### Test Binsregselect #####
+############################
 
 # Basic Syntax
-# out = binsregselect(y, x)
-# print(out)
-# out.summary()
+out = binsregselect(y, x)
+print(out)
+out.summary()
 
 # Add covariates
-# out = binsregselect(y, x, w)
-# print(out)
-# out.summary()
+out = binsregselect(y, x, w)
+print(out)
+out.summary()
 
 # Save the grid
-# out = binsregselect(y, x, w, savegrid = True)
-# print(out)
-# out.summary()
-
-# #############################
-# #### Test Binsreg ###########
-# #############################
-
-# # Default syntax
-# out  =  binsreg(y, x)
-# print(out)
-# out.summary()
-# print(out.data_plot[0].dots)
+out = binsregselect(y, x, w, savegrid = True)
+print(out)
+out.summary()
+
+############################
+### Test Binsreg ###########
+############################
+
+# Default syntax
+out  =  binsreg(y, x)
+print(out)
+out.summary()
+print(out.data_plot[0].dots)
+
+# Include weights
+weights = np.repeat(np.arange(1,11),100)
+out  =  binsreg(y, x, weights = weights)
+print(out)
+out.summary()
 
 # Default syntax with data
-# out =  binsreg(y='y', x = 'x', w = 'w', data = data, nbins = 21)
-# print(out)
-# out.summary
-# print(out.data_plot[0].dots)
-
-# # Evaluate the estimated function at median of w rather than the mean
-# out = binsreg(y, x, w, nbins = 21, at="median")
-# print(out)
-# out.summary
-# print(out.data_plot[0].dots)
-
-# # Setting quantile-spaced bins to J=20, add a linear fit
-# est = binsreg(y, x, w, nbins=20, polyreg=1)
-# print(est)
-
-# # Adding line
-# est = binsreg(y, x, w, nbins=20, line=(3,3))
-# print(est)
-# print(est.data_plot[0].line)
-
-# # Adding a CI
-# est = binsreg(y, x, w, nbins=20, ci=(3,3))
-# print(est)
-# print(est.data_plot[0].ci)
-
-# # Adding a CB
-# est = binsreg(y, x, w, nbins=20,cb=(3,3))
-# print(est)
-# print(est.data_plot[0].cb)
-
-# # Adding a polyreg
-# est = binsreg(y, x, w, nbins=20, polyreg = 4)
-# print(est)
-# print(est.data_plot[0].poly)
-
-# # Adding line, ci, cb and polyreg together
-# out = binsreg(y, x, w, nbins=20, line = (3,3), ci =(3,3), cb =(3,3), polyreg = 4)
-# print(out)
-# out.summary()
+out =  binsreg(y='y', x = 'x', w = 'w', data = data, nbins = 21)
+print(out)
+out.summary
+print(out.data_plot[0].dots)
+
+# Evaluate the estimated function at median/zero of w rather than the mean
+out = binsreg(y, x, w, nbins = 21, at = "zero")
+print(out)
+out.summary
+
+# Setting quantile-spaced bins to J=20, add a linear fit
+est = binsreg(y, x, w, nbins=20, polyreg=1)
+print(est)
+
+# Adding line
+est = binsreg(y, x, w, nbins=20, line=(3,3))
+print(est)
+print(est.data_plot[0].line)
+
+# Adding a CI
+est = binsreg(y, x, w, nbins=20, ci=(3,3))
+print(est)
+print(est.data_plot[0].ci)
+
+# Adding a CB
+est = binsreg(y, x, w, cb=(0,0))
+print(est)
+print(est.data_plot[0].cb)
+
+# Adding a polyreg
+est = binsreg(y, x, w, nbins=20, polyreg = 5)
+print(est)
+print(est.data_plot[0].poly)
+
+# Adding line, ci, cb and polyreg together
+out = binsreg(y, x, w, nbins=20, line = (3,3), ci =(3,3), cb =(3,3), polyreg = 4)
+print(out)
+out.summary()
 
 # Using multiple nbins
-# out = binsreg(y,x,w, nbins = np.arange(20), pselect = 1, sselect=1)
-# print(out)
-# out.summary()
+out = binsreg(y,x,w, nbins = np.arange(20), pselect = 1, sselect=1)
+print(out)
+out.summary()
 
 # Using pselect/sselect
-# out = binsreg(y,x,w, nbins = 10, pselect = np.arange(5), sselect=np.arange(5))
-# print(out)
-# out.summary()
+out = binsreg(y,x,w, nbins = 10, pselect = np.arange(5), sselect=np.arange(5))
+print(out)
+out.summary()
 
 # # Comparison by groups
-# out = binsreg(y, x, w, by=t, line=(3,3), cb=(3,3),
-#                  bycolors=("blue", "red"), bysymbols=('o','^'))
-# print(out)
-# out.summary()
-
-# out = binsreg(y, 'x', w, nbins=20, by='t', data=data, line=(3,3), cb=(3,3),
-#               bycolors=("blue", "red"), bysymbols=('o','^'))
-# out.summary()
-
-# #############################
-# #### Test Binsglm ###########
-# #############################
+out = binsreg(y, x, w, by=t, line=(3,3), cb=(3,3),
+                 bycolors=("blue", "red"), bysymbols=('o','^'))
+print(out)
+out.summary()
+
+out = binsreg(y, 'x', w, nbins=20, by='t', data=data, line=(3,3), cb=(3,3),
+              bycolors=("blue", "red"), bysymbols=('o','^'))
+out.summary()
+
+# Test a Large Number of covariates with  Default syntax
+ncov = 900
+w_large = np.random.rand(len(y),ncov)
+out  =  binsreg(y, x, w = w_large)
+print(out)
+out.summary()
+
+# Include cluster variable
+out  =  binsreg(y, x, cluster = id)
+print(out)
+out.summary()
+
+
+#############################
+#### Test Binsglm ###########
+#############################
 
 # Basic syntax
-# out = binsglm(d, x, dist = 'Binomial')
-# print(out)
-# out.summary()
+out = binsglm(d, x, dist = 'Binomial')
+print(out)
+out.summary()
 
 # Altering optimizer parameters
-# out = binsglm(d, x, dist = 'Binomial', maxiter = 500, tol = 1e-6)
-# print(out)
-# out.summary()
+out = binsglm(d, x, dist = 'Binomial', maxiter = 500, tol = 1e-6)
+print(out)
+out.summary()
 
 # Explict nbins and link
-# out = binsglm(d, x, w, nbins=10, dist = 'Binomial', link = 'logit')
-# print(out)
-# out.summary()
+out = binsglm(d, x, w, nbins=10, dist = 'Binomial', link = 'Probit')
+print(out)
+out.summary()
 
 # Plot the function in the inverse link (logistic) function rather than the conditional probability
-# out = binsglm(d, x, w, nbins = 17, dist = 'Binomial', nolink = True)
-# print(out)
-# out.summary()
-
-# ##############################
-# #### Test Binsqreg ###########
-# ##############################
+out = binsglm(d, x, w, nbins = 17, dist = 'Binomial', nolink = True)
+print(out)
+out.summary()
+
+##############################
+#### Test Binsqreg ###########
+##############################
 
 # Basic Syntax
-# out = binsqreg(y, x)
-# print(out)
-# out.summary()
-
-# out = binsqreg(y, x, w, data=data, quantile=0.25, ci=(3,3))
-# print(out)
-# out.summary()
+out = binsqreg(y, x)
+print(out)
+out.summary()
+
+out = binsqreg(y, x, w, data=data, quantile=0.25, ci=(3,3))
+print(out)
+out.summary()
 
 # Change Optimizer parameters
-# out = binsqreg(y, x, max_iter = 5000, p_tol = 1e-6)
-# print(out)
-# out.summary()
-
-# ####################################
-# ############ BINSTEST ##############
-# ####################################
-
-# # basic syntax: linearity? (default method: least squares regression)
-# out = binstest(y, x)
-# print(out)
-# out.summary()
-
-
-# # Test many things simultaneously
-# out = binstest(y, x, w, nbins=20, testshaper=(-2,0), testshapel=4,
-#                     testmodelpoly=1, nsims=1000, simsgrid=30)
-# print(out)
-# out.summary()
-
-# # Quantile regression - Median regression: linear?
-# out = binstest(y, x, w, estmethod="qreg", quantile=0.5, testmodelpoly=1)
-# print(out)
-# out.summary()
-
-# # Logistic Regression - Shape restriction test: increasing?
-# out = binstest(d, x, w, estmethod="glm", dist= 'Binomial', deriv=1, nbins=20, testshaper=0)
-# print(out)
-# out.summary()
-
-# #######################################
-# ########## BINSPWC ####################
-# #######################################
+out = binsqreg(y, x, max_iter = 5000, p_tol = 1e-6)
+print(out)
+out.summary()
+
+###################################
+########### BINSTEST ##############
+###################################
+
+# basic syntax: linearity? (default method: least squares regression)
+out = binstest(y, x)
+print(out)
+out.summary()
+
+# Test many things simultaneously
+out = binstest(y, x, w, nbins=20, testshaper=(-2,0), testshapel=4,
+                    testmodelpoly=1, nsims=1000, simsgrid=30)
+print(out)
+out.summary()
+
+# Quantile regression - Median regression: linear?
+out = binstest(y, x, w, estmethod="qreg", quantile=0.5, testmodelpoly=1)
+print(out)
+out.summary()
+
+# Logistic Regression - Shape restriction test: increasing?
+out = binstest(d, x, w, estmethod="glm", dist= 'Binomial', deriv=1, nbins=20, testshaper=0)
+print(out)
+out.summary()
+
+######################################
+######### BINSPWC ####################
+######################################
 
 # Basic syntax
-# out = binspwc(y, x)
-# print(out)
-# out.summary()
+out = binspwc(y, x)
+print(out)
+out.summary()
 
 # Basic syntax 2
-# out = binspwc(y, x, by=t)
-# print(out)
-# out.summary()
+out = binspwc(y, x, by=t)
+print(out)
+out.summary()
 
 # Basic syntax with pre-specified # of bins
-# out = binspwc(y, x, w, bynbins =(5,4), by=t)
-# print(out)
-# out.summary()
+out = binspwc(y, x, w, bynbins =(5,4), by=t)
+print(out)
+out.summary()
 
 # Compare GLM  with pre-specified # of bins
-# out = binspwc(d, x, w, bynbins =(5,4), by=t, estmethod="glm", dist='Binomial')
-# print(out)
-# out.summary()
-
-#  Compare quantile regression functions
-# out =  binspwc(y, x, w, bynbins = (5,4), by=t, estmethod="qreg", quantile=0.2)
-# print(out)
-# out.summary()
+out = binspwc(d, x, w, bynbins =(5,4), by=t, estmethod="glm", dist='Binomial')
+print(out)
+out.summary()
+
+# Compare quantile regression functions
+out =  binspwc(y, x, w, bynbins = (5,4), by=t, estmethod="qreg", quantile=0.2)
+print(out)
+out.summary()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

