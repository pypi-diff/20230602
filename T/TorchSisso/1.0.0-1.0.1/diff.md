# Comparing `tmp/TorchSisso-1.0.0.tar.gz` & `tmp/TorchSisso-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TorchSisso-1.0.0.tar", last modified: Wed May 17 13:54:49 2023, max compression
+gzip compressed data, was "TorchSisso-1.0.1.tar", last modified: Thu Jun  1 22:43:30 2023, max compression
```

## Comparing `TorchSisso-1.0.0.tar` & `TorchSisso-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-05-17 13:54:49.899884 TorchSisso-1.0.0/
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      423 2023-05-17 13:54:49.898890 TorchSisso-1.0.0/PKG-INFO
-drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-05-17 13:54:49.882883 TorchSisso-1.0.0/TorchSisso/
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)    20473 2023-05-17 13:49:30.000000 TorchSisso-1.0.0/TorchSisso/FeatureSpaceConstruction.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)     6918 2023-05-17 03:04:00.000000 TorchSisso-1.0.0/TorchSisso/SISSORegressor.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      221 2023-05-17 13:27:00.000000 TorchSisso-1.0.0/TorchSisso/__init__.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)     3661 2023-05-17 13:30:48.000000 TorchSisso-1.0.0/TorchSisso/testRegressor.py
-drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-05-17 13:54:49.896883 TorchSisso-1.0.0/TorchSisso.egg-info/
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      423 2023-05-17 13:54:49.000000 TorchSisso-1.0.0/TorchSisso.egg-info/PKG-INFO
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      296 2023-05-17 13:54:49.000000 TorchSisso-1.0.0/TorchSisso.egg-info/SOURCES.txt
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)        1 2023-05-17 13:54:49.000000 TorchSisso-1.0.0/TorchSisso.egg-info/dependency_links.txt
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)       19 2023-05-17 13:54:49.000000 TorchSisso-1.0.0/TorchSisso.egg-info/requires.txt
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)       11 2023-05-17 13:54:49.000000 TorchSisso-1.0.0/TorchSisso.egg-info/top_level.txt
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)       38 2023-05-17 13:54:49.900883 TorchSisso-1.0.0/setup.cfg
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      738 2023-05-17 13:52:36.000000 TorchSisso-1.0.0/setup.py
+drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-01 22:43:30.976373 TorchSisso-1.0.1/
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      423 2023-06-01 22:43:30.975374 TorchSisso-1.0.1/PKG-INFO
+drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-01 22:43:30.955371 TorchSisso-1.0.1/TorchSisso/
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    19482 2023-06-01 22:28:34.000000 TorchSisso-1.0.1/TorchSisso/FC_copy.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    19482 2023-06-01 22:27:12.000000 TorchSisso-1.0.1/TorchSisso/FC_copy_working.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    19482 2023-06-01 22:41:08.000000 TorchSisso-1.0.1/TorchSisso/FeatureSpaceConstruction.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    20922 2023-06-01 22:40:53.000000 TorchSisso-1.0.1/TorchSisso/Feature_space_construction_1.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    10816 2023-06-01 14:09:28.000000 TorchSisso-1.0.1/TorchSisso/SISSORegressor.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    10870 2023-06-01 14:04:04.000000 TorchSisso-1.0.1/TorchSisso/SISSORegressor_L1L0.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      222 2023-06-01 14:47:33.000000 TorchSisso-1.0.1/TorchSisso/__init__.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)     5777 2023-06-01 22:07:47.000000 TorchSisso-1.0.1/TorchSisso/testRegressor.py
+drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-01 22:43:30.971373 TorchSisso-1.0.1/TorchSisso.egg-info/
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      423 2023-06-01 22:43:30.000000 TorchSisso-1.0.1/TorchSisso.egg-info/PKG-INFO
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      425 2023-06-01 22:43:30.000000 TorchSisso-1.0.1/TorchSisso.egg-info/SOURCES.txt
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)        1 2023-06-01 22:43:30.000000 TorchSisso-1.0.1/TorchSisso.egg-info/dependency_links.txt
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)       19 2023-06-01 22:43:30.000000 TorchSisso-1.0.1/TorchSisso.egg-info/requires.txt
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)       11 2023-06-01 22:43:30.000000 TorchSisso-1.0.1/TorchSisso.egg-info/top_level.txt
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)       38 2023-06-01 22:43:30.977372 TorchSisso-1.0.1/setup.cfg
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      738 2023-06-01 22:42:14.000000 TorchSisso-1.0.1/setup.py
```

### Comparing `TorchSisso-1.0.0/TorchSisso/FeatureSpaceConstruction.py` & `TorchSisso-1.0.1/TorchSisso/Feature_space_construction_1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
+Created on Thu Jun  1 18:40:28 2023
+
+@author: muthyala.7
+"""
+
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
 Created on Sat May 13 21:42:41 2023
 
 @author: muthyala.7
 """
 import torch 
 import pandas as pd 
 import numpy as np 
@@ -207,15 +215,14 @@
         if op in ['+','-','*','/','abs']:
           continue
         else:
           raise TypeError("Valid set of operators +,-,*,/, abs please check the operators set")
           break
       
       #Defining the set of combinations to be performed
-      import itertools
       from itertools import combinations
 
       #getting list of cobinations without replacement using itertools 
       combinations = list(combinations(self.columns,2))
       #Creating a list for the adding the features combinations created
       #Converting columns to numpy array to support on GPU if not the indexing doesn't support to GPU
       column_array = np.array(self.columns)
@@ -233,43 +240,47 @@
           #Apply the conditions of operators
           if op =='+':
             feature_value = torch.add(values[:,0],values[:,1]).to(self.device)
             #print(feature_value.device,self.feature_values1.device)
             self.feature_values1 = torch.cat((self.feature_values1,feature_value.unsqueeze(1)), dim=1).to(self.device)
             col_name = f'({comb[0]}{op}{comb[1]})'
             self.feature_names1.append(col_name)
+            #print(feature_value.device,self.feature_values1.device)
           elif op =='-':
             feature_value = torch.sub(values[:,0],values[:,1]).to(self.device)
             self.feature_values1 = torch.cat((self.feature_values1,feature_value.unsqueeze(1)), dim=1).to(self.device)
             col_name = f'({comb[0]}{op}{comb[1]})'
             self.feature_names1.append(col_name)
             #feature_value1 = torch.sub(values[:,1],values[:,0]).to(self.device)
             #self.feature_values1 = torch.cat((self.feature_values1,feature_value1.unsqueeze(1)), dim=1).to(self.device)
             #col_name = f'({comb[1]}{op}{comb[0]})'
             #self.feature_names1.append(col_name)
+            #print(feature_value.device,self.feature_values1.device)
           elif op == '*':
             feature_value = torch.mul(values[:,0],values[:,1]).to(self.device)
             self.feature_values1 = torch.cat((self.feature_values1,feature_value.unsqueeze(1)), dim=1).to(self.device)
             col_name = f'({comb[0]}{op}{comb[1]})'
             self.feature_names1.append(col_name)
+            #print(feature_value.device,self.feature_values1.device)
           elif op =='/':
             feature_value = torch.div(values[:,0],values[:,1]).to(self.device)
             self.feature_values1 = torch.cat((self.feature_values1,feature_value.unsqueeze(1)), dim=1).to(self.device)
             col_name = f'({comb[0]}{op}{comb[1]})'
             self.feature_names1.append(col_name)
-            #feature_value1 = torch.div(values[:,1],values[:,0]).to(self.device)
-            #self.feature_values1 = torch.cat((self.feature_values1,feature_value1.unsqueeze(1)), dim=1).to(self.device)
-            #col_name = f'({comb[1]}{op}{comb[0]})'
-            #self.feature_names1.append(col_name)
+            #print(feature_value.device,self.feature_values1.device)
+#            feature_value1 = torch.div(values[:,1],values[:,0]).to(self.device)
+#            self.feature_values1 = torch.cat((self.feature_values1,feature_value1.unsqueeze(1)), dim=1).to(self.device)
+#            col_name = f'({comb[1]}{op}{comb[0]})'
+#            self.feature_names1.append(col_name)
           elif op == 'abs':
             feature_value = torch.abs(torch.sub(values[:,0],values[:,1])).to(self.device)
             self.feature_values1 = torch.cat((self.feature_values1,feature_value.unsqueeze(1)), dim=1).to(self.device)
             col_name = f'(|{comb[0]}-{comb[1]}|)'
             self.feature_names1.append(col_name)
-            
+            print(feature_value.device,self.feature_values1.device)         
       
       #Removing Nan and inf columns from tenosr and corresponding variable name form the list
       nan_columns = torch.any(torch.isnan(self.feature_values1), dim=0)
       inf_columns = torch.any(torch.isinf(self.feature_values1), dim=0)
       nan_or_inf_columns = nan_columns | inf_columns
 
       # Remove columns from tensor
@@ -305,29 +316,28 @@
     print('Time for phi 1 creation is: ',time.time() - start_time)
     print('First Feature Space building is completed with features count: ',int(space_created.shape[1]))
     #Update the columns according to the new phi created for the next phase features
     self.df_feature_values = (space_created).to(self.device)
     #Creating the phi2 based on the space created 
     start_time = time.time()
     values, names = self.combinations(basic_operators)
+    print('Time taken for combinations', time.time()-start_time)
     values1, names1 = self.single_variable(other_operators)
     space_created_2 = torch.cat((space_created,values,values1), dim=1).to(self.device)
     self.columns = self.columns + names + names1 
     #######################
     #code to remove duplicate columns from dataframe
     #########################
     #Converting tensor to numpy and then dataframe to remove duplicates
     #space1 = space_created_2.cpu().numpy()
     space = pd.DataFrame(space_created_2.cpu(),columns = self.columns)
-    print(space.shape)
     space = space.round(7)
     #space = space.dropna(axis=1, how='any')
     # Transpose the dataframe
     space = space.T.drop_duplicates().T
-    print(space.shape)
 
     print('Time taken to create and remove redundant features in phi2 is ', time.time() - start_time)
     del space_created
     del values, values1, names, names1
     self.columns = space.columns.tolist()
     self.df_feature_values = torch.tensor(space.values).to(self.device)
     print('Second Feature Space building is completed',space.shape)
```

### Comparing `TorchSisso-1.0.0/TorchSisso/SISSORegressor.py` & `TorchSisso-1.0.1/TorchSisso/SISSORegressor_L1L0.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 import torch
 import warnings
 warnings.filterwarnings('ignore')
 import itertools
 import time 
 from sklearn.linear_model import LinearRegression
 from sklearn.metrics import mean_squared_error
-
+from sklearn.linear_model import Lasso, LassoCV
 class SISSO_Regressor:
     
-    def __init__(self,x,y,names,dimension=1,sis_features=20,device='cpu'):
+    def __init__(self,x,y,names,dimension=1,sis_features=20,device='cpu',method='L0'):
         print(f'Starting SISSO in {device}')
         self.device = torch.device(device)
         self.x = x.to(self.device)
         self.y =y.to(self.device)
         self.dimension= dimension
         self.sis_features = sis_features
         self.feature_names = names
@@ -29,14 +29,70 @@
         self.y_mean = self.y.mean().to(self.device)
         self.y_centered = (self.y - self.y_mean).to(self.device)
         self.x_standardized = ((self.x - self.x_mean)/self.x_std).to(self.device)
         self.scores = []
         self.indices = []
         self.residual = torch.empty(self.y_centered.shape).to(self.device)
         self.x_std_clone = torch.clone(self.x_standardized).to(self.device)
+        self.method = method
+    
+    def L1_L0_regularization(self,iteration):
+        
+        min_error = torch.dot(self.y_centered,self.y_centered).to(self.device)
+        for indices in self.indices:
+            self.x_standardized[:,indices] = 0
+        scores = torch.abs(torch.mm(self.residual,self.x_standardized)).to(self.device)
+        scores[torch.isnan(scores)] = 0
+        for indices in self.indices:
+            self.x_standardized[:,indices] = self.x_std_clone[:,indices]
+        sorted_scores,sorted_indices = torch.topk(scores,k=self.sis_features)
+        self.scores.append(sorted_scores)
+        self.indices.append(sorted_indices)
+        start_c = time.time()
+        #Implementing L1 regularization on the screened features to avoid combinations explosion
+        index_pos = torch.cat(self.indices).flatten().to(self.device)
+        x_sub = self.x_standardized[:,index_pos].to(self.device)
+        lasso = LassoCV(cv=int(self.y.shape[0]))
+        #lasso = Lasso(alpha=0.01)
+        lasso.fit(x_sub.cpu().numpy(),self.y_centered.cpu().numpy())
+        #Get the non-zero coefficients
+        non_zeros = torch.nonzero(torch.tensor(lasso.coef_).to(self.device)).to(self.device)
+        
+        if len(non_zeros) == 0:
+            #fit the normal LASSO 
+            print('entering normal fit')
+            lasso = Lasso(alpha = 0.1)
+            lasso.fit(x_sub.cpu().numpy(),self.y_centered.cpu().numpy())
+            #Get the non-zero coefficients
+            non_zeros = torch.nonzero(torch.tensor(lasso.coef_).to(self.device)).to(self.device)
+            
+        combinations_generated = itertools.combinations(non_zeros,iteration)
+        for combinations in combinations_generated:
+            x_sub = self.x_standardized[:,combinations].to(self.device)
+            coefficients = x_sub.pinverse()@self.y_centered.reshape(-1,1).to(self.device)
+            sum_of_residuals = torch.sum((x_sub @ coefficients - self.y_centered.reshape(-1,1))**2).to(self.device)
+            index = torch.tensor(combinations)
+            try:
+                if sum_of_residuals <min_error:
+                    min_error = sum_of_residuals
+                    coefs_min, indices_min = coefficients,index
+            except:
+                pass
+        print('L1L0 regularization is completed in :',time.time()-start_c)
+        rmse = torch.sqrt(min_error/int(self.y_centered.shape[0])).to(self.device)
+        non_std_coeff = ((coefs_min.T/self.x_std[indices_min])).to(self.device)
+        non_std_intercept = self.y.mean() - torch.dot(self.x_mean[indices_min]/self.x_std[indices_min],coefs_min.flatten()).to(self.device)
+        self.residual = self.y_centered - torch.mm(coefs_min.T,self.x_standardized[:,indices_min].T).to(self.device)
+        terms = []
+        for i in range(len(non_std_coeff.squeeze())):
+          term = str(round(float(non_std_coeff.squeeze()[i]),3)) + "*" + str(self.feature_names[int(indices_min[i])])
+          terms.append(term)
+        return rmse,terms,non_std_intercept,non_std_coeff
+        
+        
     
     def higherdimension(self):
         
         min_error = torch.dot(self.y_centered,self.y_centered).to(self.device)
         for indices in self.indices:
             self.x_standardized[:,indices] = 0
         scores = torch.abs(torch.mm(self.residual,self.x_standardized)).to(self.device)
@@ -50,27 +106,28 @@
         #print(len(self.indices),len(list(combinations_generated)))
         start_c = time.time()
         for combinations in combinations_generated:
             x_sub = self.x_standardized[:,combinations].to(self.device)
             coefficients = x_sub.pinverse()@self.y_centered.reshape(-1,1).to(self.device)
             sum_of_residuals = torch.sum((x_sub @ coefficients - self.y_centered.reshape(-1,1))**2).to(self.device)
             index = torch.tensor(combinations)
-            if sum_of_residuals <min_error:
-                min_error = sum_of_residuals
-                coefs_min, indices_min = coefficients,torch.tensor(combinations)
-            else:
-                continue
+            try:
+                if sum_of_residuals <min_error:
+                    min_error = sum_of_residuals
+                    coefs_min, indices_min = coefficients,index
+            except:
+                pass
         print('Time taken to go through all combinations is:', time.time()-start_c)
         rmse = torch.sqrt(min_error/int(self.y_centered.shape[0])).to(self.device)
         non_std_coeff = ((coefs_min.T/self.x_std[indices_min])).to(self.device)
         non_std_intercept = self.y.mean() - torch.dot(self.x_mean[indices_min]/self.x_std[indices_min],coefs_min.flatten()).to(self.device)
         self.residual = self.y_centered - torch.mm(coefs_min.T,self.x_standardized[:,indices_min].T).to(self.device)
         terms = []
         for i in range(len(non_std_coeff.squeeze())):
-          term = str(float(non_std_coeff.squeeze()[i])) + "*" + str(self.feature_names[int(indices_min[i])])
+          term = str(round(float(non_std_coeff.squeeze()[i]),3)) + "*" + str(self.feature_names[int(indices_min[i])])
           terms.append(term)
         return rmse,terms,non_std_intercept,non_std_coeff
 
     
     
     def SISSO(self):
         
@@ -111,25 +168,41 @@
                     print('RMSE:', float(rmse))
                 else:
                     equation = str(float(coeff)) + '*' + str(self.feature_names[selected_index]) + '-' + str(float(intercept))[1:]
                     print('Equation: ',equation)
                     print('RMSE',float(rmse))
             else:
                 start_time = time.time()
-                rmse,terms,intercept,coefs = self.higherdimension()
-                equation = ''
-                for k in range(len(terms)):
-                  print(f'{k+1} term in the equation is {terms[k]}')
-                  if coefs.flatten()[k] > 0:
-                      equation = equation + (str(terms[k])) + '+ '
-                  else:
-                    equation = equation + (str(terms[k])) 
-                print(f'{i} term equation:',equation[:len(equation)-2])
-                print('Intercept:', float(intercept))
-                print('RMSE:',float(rmse))
-                print(f'Time taken for {i} dimension is: ', time.time()-start_time)
+                if self.method == 'L0':
+                    rmse,terms,intercept,coefs = self.higherdimension()
+                    equation = ''
+                    for k in range(len(terms)):
+                      print(f'{k+1} term in the equation is {terms[k]}')
+                      if coefs.flatten()[k] > 0:
+                          equation = equation + ' + ' + (str(terms[k])) 
+                      else:
+                        equation = equation + (str(terms[k])) + '  '
+                    print(f'{i} term equation:',equation[:len(equation)-1])
+                    print('Intercept:', float(intercept))
+                    print('RMSE:',float(rmse))
+                    print(f'Time taken for {i} dimension is: ', time.time()-start_time)
+                else:
+                    print('Performing L1L0 regularization method')
+                    rmse,terms,intercept,coefs = self.L1_L0_regularization(i)
+                    print('RMSE:',rmse)
+                    equation = ''
+                    for k in range(len(terms)):
+                      print(f'{k+1} term in the equation is {terms[k]}')
+                      if coefs.flatten()[k] > 0:
+                          equation = equation + ' + ' + (str(terms[k])) 
+                      else:
+                        equation = equation + (str(terms[k])) + '  '
+                    
+        rmse = 'RMSE: ' + str(float(rmse))
+        equation = 'Equation: ' + equation[:len(equation)-2]
+        return rmse,equation
```

### Comparing `TorchSisso-1.0.0/setup.py` & `TorchSisso-1.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 import setuptools
 
 
 setuptools.setup(
     name="TorchSisso",
-    version="1.0.0",
+    version="1.0.1",
     author="Madhav Muthyala",
     author_email="madhavreddymuthyala@gmail.com",
     description="GPU Supported Sure Independence Screening and Sparsifying Operator Package",
     url="https://github.com/MR1319/TorchSisso",
     packages=setuptools.find_packages(),
     install_requires=[
         "torch",
```

