# Comparing `tmp/TorchSisso-1.0.1.tar.gz` & `tmp/TorchSisso-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TorchSisso-1.0.1.tar", last modified: Thu Jun  1 22:43:30 2023, max compression
+gzip compressed data, was "TorchSisso-1.0.2.tar", last modified: Fri Jun  2 02:50:38 2023, max compression
```

## Comparing `TorchSisso-1.0.1.tar` & `TorchSisso-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-01 22:43:30.976373 TorchSisso-1.0.1/
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      423 2023-06-01 22:43:30.975374 TorchSisso-1.0.1/PKG-INFO
-drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-01 22:43:30.955371 TorchSisso-1.0.1/TorchSisso/
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)    19482 2023-06-01 22:28:34.000000 TorchSisso-1.0.1/TorchSisso/FC_copy.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)    19482 2023-06-01 22:27:12.000000 TorchSisso-1.0.1/TorchSisso/FC_copy_working.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)    19482 2023-06-01 22:41:08.000000 TorchSisso-1.0.1/TorchSisso/FeatureSpaceConstruction.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)    20922 2023-06-01 22:40:53.000000 TorchSisso-1.0.1/TorchSisso/Feature_space_construction_1.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)    10816 2023-06-01 14:09:28.000000 TorchSisso-1.0.1/TorchSisso/SISSORegressor.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)    10870 2023-06-01 14:04:04.000000 TorchSisso-1.0.1/TorchSisso/SISSORegressor_L1L0.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      222 2023-06-01 14:47:33.000000 TorchSisso-1.0.1/TorchSisso/__init__.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)     5777 2023-06-01 22:07:47.000000 TorchSisso-1.0.1/TorchSisso/testRegressor.py
-drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-01 22:43:30.971373 TorchSisso-1.0.1/TorchSisso.egg-info/
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      423 2023-06-01 22:43:30.000000 TorchSisso-1.0.1/TorchSisso.egg-info/PKG-INFO
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      425 2023-06-01 22:43:30.000000 TorchSisso-1.0.1/TorchSisso.egg-info/SOURCES.txt
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)        1 2023-06-01 22:43:30.000000 TorchSisso-1.0.1/TorchSisso.egg-info/dependency_links.txt
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)       19 2023-06-01 22:43:30.000000 TorchSisso-1.0.1/TorchSisso.egg-info/requires.txt
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)       11 2023-06-01 22:43:30.000000 TorchSisso-1.0.1/TorchSisso.egg-info/top_level.txt
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)       38 2023-06-01 22:43:30.977372 TorchSisso-1.0.1/setup.cfg
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      738 2023-06-01 22:42:14.000000 TorchSisso-1.0.1/setup.py
+drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-02 02:50:38.371388 TorchSisso-1.0.2/
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      423 2023-06-02 02:50:38.370393 TorchSisso-1.0.2/PKG-INFO
+drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-02 02:50:38.352385 TorchSisso-1.0.2/TorchSisso/
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    23644 2023-06-02 01:56:01.000000 TorchSisso-1.0.2/TorchSisso/FC_copy.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    19482 2023-06-01 22:27:12.000000 TorchSisso-1.0.2/TorchSisso/FC_copy_working.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    23644 2023-06-02 02:49:37.000000 TorchSisso-1.0.2/TorchSisso/FeatureSpaceConstruction.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    20851 2023-06-01 23:34:05.000000 TorchSisso-1.0.2/TorchSisso/Feature_space_construction_1.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    10816 2023-06-01 14:09:28.000000 TorchSisso-1.0.2/TorchSisso/SISSORegressor.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    10870 2023-06-01 14:04:04.000000 TorchSisso-1.0.2/TorchSisso/SISSORegressor_L1L0.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      222 2023-06-01 14:47:33.000000 TorchSisso-1.0.2/TorchSisso/__init__.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)     5866 2023-06-02 02:07:18.000000 TorchSisso-1.0.2/TorchSisso/testRegressor.py
+drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-02 02:50:38.367385 TorchSisso-1.0.2/TorchSisso.egg-info/
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      423 2023-06-02 02:50:38.000000 TorchSisso-1.0.2/TorchSisso.egg-info/PKG-INFO
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      425 2023-06-02 02:50:38.000000 TorchSisso-1.0.2/TorchSisso.egg-info/SOURCES.txt
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)        1 2023-06-02 02:50:38.000000 TorchSisso-1.0.2/TorchSisso.egg-info/dependency_links.txt
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)       19 2023-06-02 02:50:38.000000 TorchSisso-1.0.2/TorchSisso.egg-info/requires.txt
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)       11 2023-06-02 02:50:38.000000 TorchSisso-1.0.2/TorchSisso.egg-info/top_level.txt
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)       38 2023-06-02 02:50:38.372391 TorchSisso-1.0.2/setup.cfg
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      738 2023-06-02 02:50:09.000000 TorchSisso-1.0.2/setup.py
```

### Comparing `TorchSisso-1.0.1/TorchSisso/FC_copy.py` & `TorchSisso-1.0.2/TorchSisso/FC_copy_working.py`

 * *Files identical despite different names*

### Comparing `TorchSisso-1.0.1/TorchSisso/FC_copy_working.py` & `TorchSisso-1.0.2/TorchSisso/Feature_space_construction_1.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-Created on Tue May 30 13:31:55 2023
+Created on Thu Jun  1 18:40:28 2023
 
 @author: muthyala.7
 """
 
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
@@ -59,29 +59,24 @@
     
     #Creating empty tensor for single operators
     self.feature_values = torch.empty(self.df.shape[0],0).to(self.device)
     self.feature_names = []
     #creating empty tensor for combinations
     self.feature_values1 = torch.empty(self.df.shape[0],0).to(self.device)
     self.feature_names1 = []
-    self.feature_values2 = []
-    self.feature_values3 = []
   '''
   ###############################################################################################################
 
   Construct all the features that can be constructed using the single operators like log, exp, sqrt etc..
 
   ###############################################################################################################
   '''
 
-  def single_variable(self,operators_set): 
-    #Check for the validity of the operator set given
-    self.feature_values = torch.empty(self.df.shape[0],0).to(self.device)
-    self.feature_names = []
-    self.feature_values3 = []
+  def single_variable(self,operators_set):
+    #Check for the validity of the operator set given 
     for op in operators_set:
 
       if op in ['exp','sin','cos','sqrt','cbrt','log','ln','^-1','^2','^3','exp(-1)','abs']:
         continue
       else:
         raise TypeError('Invalid Operator found in the given operator set')
     
@@ -93,207 +88,212 @@
       #Looping over all the initial feature set with the specific operator set 
 
       for i in range(len(self.columns)):
         if op == 'exp':
 
           #Applying the operator and adding to the new dataframe
           feature = f'{op}({self.columns[i]})'
-          value = torch.exp(self.df_feature_values[:,i])
-          self.feature_values3.append(value.unsqueeze(1))
+          value = torch.exp(self.df_feature_values[:,i]).to(self.device)
+          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1).to(self.device)
           self.feature_names.append(feature)
+          #self.new_features_values[feature] = value.cpu().numpy()
 
         elif op == 'ln':
 
           #Applying the log operator to the feature and feature values\
           #This is the exponential not the base 10
           feature = f'{op}({self.columns[i]})'
-          value = torch.log(self.df_feature_values[:,i])
-          self.feature_values3.append(value.unsqueeze(1))
+          value = torch.log(self.df_feature_values[:,i]).to(self.device)
+          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1).to(self.device)
           self.feature_names.append(feature)
+          #self.new_features_values[feature] = value.cpu().numpy()
         
         elif op == 'sin':
           #Applying the sin operator to the featrure and feature values
           feature = f'{op}({self.columns[i]})'
-          value = torch.sin(self.df_feature_values[:,i])
-          self.feature_values3.append(value.unsqueeze(1))
+          value = torch.sin(self.df_feature_values[:,i]).to(self.device)
+          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1).to(self.device)
+          #self.new_features_values[feature] = value.cpu().numpy()
           self.feature_names.append(feature)
         
         elif op =='log':
 
           #Applying the log10 operator to the feature and feature values
           feature = f'{op}({self.columns[i]})'
-          value = torch.log10(self.df_feature_values[:,i])
-          self.feature_values3.append(value.unsqueeze(1))
+          value = torch.log10(self.df_feature_values[:,i]).to(self.device)
+          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1).to(self.device)
           self.feature_names.append(feature)
+          #self.new_features_values[feature] = value.cpu().numpy()
         
         elif op =='cos':
 
           #Applying the cos operator to the feature and feature values
           feature = f'{op}({self.columns[i]})'
-          value = torch.cos(self.df_feature_values[:,i])
-          self.feature_values3.append(value.unsqueeze(1))
+          value = torch.cos(self.df_feature_values[:,i]).to(self.device)
+          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1).to(self.device)
           self.feature_names.append(feature)
+#          self.new_features_values[feature] = value.cpu().numpy()
         
         elif op =='cbrt':
 
           #Applying the cuberoot function to the feature and feature values 
           feature = f'{op}({self.columns[i]})'
-          value = torch.pow(self.df_feature_values[:,i],1/3)
-          self.feature_values3.append(value.unsqueeze(1))
+          value = torch.pow(self.df_feature_values[:,i],1/3).to(self.device)
+          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1).to(self.device)
           self.feature_names.append(feature)
+#          self.new_features_values[feature] = value.cpu().numpy()
         
         elif op =='sqrt':
 
           #Applying the sqaureroot function to the feature and feature values
           feature = f'{op}({self.columns[i]})'
-          value = torch.sqrt(self.df_feature_values[:,i])
-          self.feature_values3.append(value.unsqueeze(1))
+          value = torch.sqrt(self.df_feature_values[:,i]).to(self.device)
+          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1).to(self.device)
           self.feature_names.append(feature)
+#          self.new_features_values[feature] = value.cpu().numpy()
 
         elif op =='^2':
 
           #Applying the square function to the feature and feature values
           feature = f'({self.columns[i]}){op}'
-          value = torch.pow(self.df_feature_values[:,i],2)
-          self.feature_values3.append(value.unsqueeze(1))
+          value = torch.pow(self.df_feature_values[:,i],2).to(self.device)
+          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1).to(self.device)
           self.feature_names.append(feature)
+          #self.new_features_values[feature] = value.cpu().numpy()
         
         elif op =='^3':
 
           #Applying the cube function to the feature and feature values
           feature = f'({self.columns[i]}){op}'
-          value = torch.pow(self.df_feature_values[:,i],3)
-          self.feature_values3.append(value.unsqueeze(1))
+          value = torch.pow(self.df_feature_values[:,i],3).to(self.device)
+          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1).to(self.device)
           self.feature_names.append(feature)
+#          self.new_features_values[feature] = value.cpu().numpy()
         
         elif op == '^-1':
 
           #Applying the inverse function to the feature and feature valuies
           feature = f'({self.columns[i]}){op}'
-          value = torch.reciprocal(self.df_feature_values[:,i])
-          self.feature_values3.append(value.unsqueeze(1))
+          value = torch.reciprocal(self.df_feature_values[:,i]).to(self.device)
+          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1).to(self.device)
           self.feature_names.append(feature)
+#          self.new_features_values[feature] = value.cpu().numpy()
 
         elif op =='exp(-1)':
 
           #Appying the inverse exponential to the feature and feature values
           feature = f'{op}({self.columns[i]})'
-          value = torch.reciprocal(torch.exp(self.df_feature_values[:,i]))
-          self.feature_values3.append(value.unsqueeze(1))
+          value = torch.reciprocal(torch.exp(self.df_feature_values[:,i])).to(self.device)
+          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1).to(self.device)
           self.feature_names.append(feature)
+          #self.new_features_values[feature] = value.cpu().numpy()
             
-    #Check for empty lists 
-    if len(self.feature_names) == 0:
-        return self.feature_values, self.feature_names
-    else:
-        # create Boolean masks for NaN and Inf values
-        self.feature_values =  torch.cat(self.feature_values3,dim=1)
-        nan_columns = torch.any(torch.isnan(self.feature_values), dim=0)
-        inf_columns = torch.any(torch.isinf(self.feature_values), dim=0)
-        nan_or_inf_columns = nan_columns | inf_columns
-    
-        # Remove columns from tensor
-        self.feature_values = self.feature_values[:, ~nan_or_inf_columns]
-    
-        # Remove corresponding elements from list
-        self.feature_names = [elem for i, elem in enumerate(self.feature_names) if not nan_or_inf_columns[i]]
-        return self.feature_values, self.feature_names #self.new_features_values
+    # create Boolean masks for NaN and Inf values
+    nan_columns = torch.any(torch.isnan(self.feature_values), dim=0)
+    inf_columns = torch.any(torch.isinf(self.feature_values), dim=0)
+    nan_or_inf_columns = nan_columns | inf_columns
+
+    # Remove columns from tensor
+    self.feature_values = self.feature_values[:, ~nan_or_inf_columns]
+
+    # Remove corresponding elements from list
+    self.feature_names = [elem for i, elem in enumerate(self.feature_names) if not nan_or_inf_columns[i]]
+
+    return self.feature_values, self.feature_names #self.new_features_values
   
 
 
   '''
   ################################################################################################
 
   Defining method to perform the combinations of the variables with the initial feature set
   ################################################################################################
   '''
   def combinations(self,operators_set):
-      #creating empty tensor for combinations
-      self.feature_values1 = torch.empty(self.df.shape[0],0).to(self.device)
-      self.feature_names1 = []
-      self.feature_values2 = []
+
     #Checking for the operator set
       for op in operators_set:
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
       #Applying the operators to the combinations created
       for comb in combinations:
+
+        #Get the index position of the combination created
         index1 = np.where(column_array == comb[0])[0][0]
         index2 = np.where(column_array == comb[1])[0][0]
         index_1 = torch.tensor([index1,index2]).to(self.device)
         #Extract the values from the original tensor 
         values = torch.tensor(self.df_feature_values[:,index_1]).to(self.device)
         for op in operators_set:
           
           #Apply the conditions of operators
           if op =='+':
-            feature_value = torch.add(values[:,0],values[:,1])
-            self.feature_values2.append(feature_value.unsqueeze(1))
+            feature_value = torch.add(values[:,0],values[:,1]).to(self.device)
+            #print(feature_value.device,self.feature_values1.device)
+            self.feature_values1 = torch.cat((self.feature_values1,feature_value.unsqueeze(1)), dim=1).to(self.device)
             col_name = f'({comb[0]}{op}{comb[1]})'
             self.feature_names1.append(col_name)
+            #print(feature_value.device,self.feature_values1.device)
           elif op =='-':
-            feature_value = torch.sub(values[:,0],values[:,1])
-            self.feature_values2.append(feature_value.unsqueeze(1))
+            feature_value = torch.sub(values[:,0],values[:,1]).to(self.device)
+            self.feature_values1 = torch.cat((self.feature_values1,feature_value.unsqueeze(1)), dim=1).to(self.device)
             col_name = f'({comb[0]}{op}{comb[1]})'
             self.feature_names1.append(col_name)
             #feature_value1 = torch.sub(values[:,1],values[:,0]).to(self.device)
-            #self.feature_values2.append(feature_value1.unsqueeze(1))
+            #self.feature_values1 = torch.cat((self.feature_values1,feature_value1.unsqueeze(1)), dim=1).to(self.device)
             #col_name = f'({comb[1]}{op}{comb[0]})'
             #self.feature_names1.append(col_name)
+            #print(feature_value.device,self.feature_values1.device)
           elif op == '*':
-            feature_value = torch.mul(values[:,0],values[:,1])
-            self.feature_values2.append(feature_value.unsqueeze(1))
+            feature_value = torch.mul(values[:,0],values[:,1]).to(self.device)
+            self.feature_values1 = torch.cat((self.feature_values1,feature_value.unsqueeze(1)), dim=1).to(self.device)
             col_name = f'({comb[0]}{op}{comb[1]})'
             self.feature_names1.append(col_name)
+            #print(feature_value.device,self.feature_values1.device)
           elif op =='/':
-            feature_value = torch.div(values[:,0],values[:,1])
-            self.feature_values2.append(feature_value.unsqueeze(1))
+            feature_value = torch.div(values[:,0],values[:,1]).to(self.device)
+            self.feature_values1 = torch.cat((self.feature_values1,feature_value.unsqueeze(1)), dim=1).to(self.device)
             col_name = f'({comb[0]}{op}{comb[1]})'
             self.feature_names1.append(col_name)
-            feature_value1 = torch.div(values[:,1],values[:,0]).to(self.device)
-            self.feature_values2.append(feature_value1.unsqueeze(1))
-            col_name = f'({comb[1]}{op}{comb[0]})'
-            self.feature_names1.append(col_name)
+            #print(feature_value.device,self.feature_values1.device)
+#            feature_value1 = torch.div(values[:,1],values[:,0]).to(self.device)
+#            self.feature_values1 = torch.cat((self.feature_values1,feature_value1.unsqueeze(1)), dim=1).to(self.device)
+#            col_name = f'({comb[1]}{op}{comb[0]})'
+#            self.feature_names1.append(col_name)
           elif op == 'abs':
-            feature_value = torch.abs(torch.sub(values[:,0],values[:,1]))
-            self.feature_values2.append(feature_value.unsqueeze(1))
+            feature_value = torch.abs(torch.sub(values[:,0],values[:,1])).to(self.device)
+            self.feature_values1 = torch.cat((self.feature_values1,feature_value.unsqueeze(1)), dim=1).to(self.device)
             col_name = f'(|{comb[0]}-{comb[1]}|)'
             self.feature_names1.append(col_name)      
       
-      #Checking whether the lists are empty
-      if len(self.feature_names1) == 0:
-          return self.feature_values1, self.feature_names1
-      else:
-          #Removing Nan and inf columns from tenosr and corresponding variable name form the list
-          self.feature_values1 = torch.cat(self.feature_values2,dim=1)
-          nan_columns = torch.any(torch.isnan(self.feature_values1), dim=0)
-          inf_columns = torch.any(torch.isinf(self.feature_values1), dim=0)
-          nan_or_inf_columns = nan_columns | inf_columns
-    
-          # Remove columns from tensor
-          self.feature_values1 = self.feature_values1[:, ~nan_or_inf_columns]
-    
-          # Remove corresponding elements from list
-          self.feature_names1 = [elem for i, elem in enumerate(self.feature_names1) if not nan_or_inf_columns[i]]
-    
-          #Returning the dataframe created
-          return self.feature_values1,self.feature_names1 #created_space
+      #Removing Nan and inf columns from tenosr and corresponding variable name form the list
+      nan_columns = torch.any(torch.isnan(self.feature_values1), dim=0)
+      inf_columns = torch.any(torch.isinf(self.feature_values1), dim=0)
+      nan_or_inf_columns = nan_columns | inf_columns
+
+      # Remove columns from tensor
+      self.feature_values1 = self.feature_values1[:, ~nan_or_inf_columns]
+
+      # Remove corresponding elements from list
+      self.feature_names1 = [elem for i, elem in enumerate(self.feature_names1) if not nan_or_inf_columns[i]]
+
+      #Returning the dataframe created
+      return self.feature_values1,self.feature_names1 #created_space
   
 
   '''
   ##########################################################################################################
 
   Creating the space based on the given set of conditions
 
@@ -302,47 +302,48 @@
   '''
 
   def feature_space(self):
     #based on the dimension we will be performing the feature space creation
     start_time = time.time()
     basic_operators = [op for op in self.operators if op in ['+', '-', '*', '/']]
     other_operators = [op for op in self.operators if op not in ['+', '-', '*', '/']]
-    
     values, names = self.combinations(basic_operators)
     values1, names1 = self.single_variable(other_operators)
     #Merging two dataframes
     space_created = torch.cat((self.df_feature_values,values,values1), dim=1).to(self.device)
     self.columns = self.columns + names + names1 
     del values, values1, names, names1
+    print('Time for phi 1 creation is: ',time.time() - start_time)
     print('First Feature Space building is completed with features count: ',int(space_created.shape[1]))
-    print('Time for phi1 creation is: ',round(time.time() - start_time,3),' seconds')
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
     space = space.round(7)
     #space = space.dropna(axis=1, how='any')
     # Transpose the dataframe
     space = space.T.drop_duplicates().T
+
+    print('Time taken to create and remove redundant features in phi2 is ', time.time() - start_time)
     del space_created
     del values, values1, names, names1
     self.columns = space.columns.tolist()
     self.df_feature_values = torch.tensor(space.values).to(self.device)
-    print('Second Feature Space building is completed with features count: ',int(space.shape[1]))
-    print('Time taken to create and remove redundant features in phi2 is ', round(time.time() - start_time,3), ' seconds')
+    print('Second Feature Space building is completed',space.shape)
 
     if self.no_of_operators >3: 
       for i in range(4,self.no_of_operators+1):
         if i == 4:
           values, names = self.combinations(basic_operators)
           values1,names1 = self.single_variable(other_operators)
           space_created_3 = torch.cat((self.df_feature_values,values,values1),dim=1).to(self.device)
```

### Comparing `TorchSisso-1.0.1/TorchSisso/FeatureSpaceConstruction.py` & `TorchSisso-1.0.2/TorchSisso/FC_copy.py`

 * *Files 18% similar despite different names*

```diff
@@ -94,96 +94,163 @@
 
       for i in range(len(self.columns)):
         if op == 'exp':
 
           #Applying the operator and adding to the new dataframe
           feature = f'{op}({self.columns[i]})'
           value = torch.exp(self.df_feature_values[:,i])
-          self.feature_values3.append(value.unsqueeze(1))
-          self.feature_names.append(feature)
+          if self.device == 'cuda':
+              self.device = torch.device('cpu')
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              self.device = torch.device('cuda')
+          else:
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              
 
         elif op == 'ln':
 
           #Applying the log operator to the feature and feature values\
           #This is the exponential not the base 10
           feature = f'{op}({self.columns[i]})'
           value = torch.log(self.df_feature_values[:,i])
-          self.feature_values3.append(value.unsqueeze(1))
-          self.feature_names.append(feature)
+          if self.device == 'cuda':
+              self.device = torch.device('cpu')
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              self.device = torch.device('cuda')
+          else:
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
         
         elif op == 'sin':
           #Applying the sin operator to the featrure and feature values
           feature = f'{op}({self.columns[i]})'
           value = torch.sin(self.df_feature_values[:,i])
-          self.feature_values3.append(value.unsqueeze(1))
-          self.feature_names.append(feature)
+          if self.device == 'cuda':
+              self.device = torch.device('cpu')
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              self.device = torch.device('cuda')
+          else:
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
         
         elif op =='log':
 
           #Applying the log10 operator to the feature and feature values
           feature = f'{op}({self.columns[i]})'
           value = torch.log10(self.df_feature_values[:,i])
-          self.feature_values3.append(value.unsqueeze(1))
-          self.feature_names.append(feature)
+          if self.device == 'cuda':
+              self.device = torch.device('cpu')
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              self.device = torch.device('cuda')
+          else:
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
         
         elif op =='cos':
 
           #Applying the cos operator to the feature and feature values
           feature = f'{op}({self.columns[i]})'
           value = torch.cos(self.df_feature_values[:,i])
-          self.feature_values3.append(value.unsqueeze(1))
-          self.feature_names.append(feature)
+          if self.device == 'cuda':
+              self.device = torch.device('cpu')
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              self.device = torch.device('cuda')
+          else:
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
         
         elif op =='cbrt':
 
           #Applying the cuberoot function to the feature and feature values 
           feature = f'{op}({self.columns[i]})'
           value = torch.pow(self.df_feature_values[:,i],1/3)
-          self.feature_values3.append(value.unsqueeze(1))
-          self.feature_names.append(feature)
+          if self.device == 'cuda':
+              self.device = torch.device('cpu')
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              self.device = torch.device('cuda')
+          else:
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
         
         elif op =='sqrt':
 
           #Applying the sqaureroot function to the feature and feature values
           feature = f'{op}({self.columns[i]})'
           value = torch.sqrt(self.df_feature_values[:,i])
-          self.feature_values3.append(value.unsqueeze(1))
-          self.feature_names.append(feature)
+          if self.device == 'cuda':
+              self.device = torch.device('cpu')
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              self.device = torch.device('cuda')
+          else:
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
 
         elif op =='^2':
 
           #Applying the square function to the feature and feature values
           feature = f'({self.columns[i]}){op}'
           value = torch.pow(self.df_feature_values[:,i],2)
-          self.feature_values3.append(value.unsqueeze(1))
-          self.feature_names.append(feature)
+          if self.device == 'cuda':
+              self.device = torch.device('cpu')
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              self.device = torch.device('cuda')
+          else:
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
         
         elif op =='^3':
 
           #Applying the cube function to the feature and feature values
           feature = f'({self.columns[i]}){op}'
           value = torch.pow(self.df_feature_values[:,i],3)
-          self.feature_values3.append(value.unsqueeze(1))
-          self.feature_names.append(feature)
+          if self.device == 'cuda':
+              self.device = torch.device('cpu')
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              self.device = torch.device('cuda')
+          else:
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
         
         elif op == '^-1':
 
           #Applying the inverse function to the feature and feature valuies
           feature = f'({self.columns[i]}){op}'
           value = torch.reciprocal(self.df_feature_values[:,i])
-          self.feature_values3.append(value.unsqueeze(1))
-          self.feature_names.append(feature)
+          if self.device == 'cuda':
+              self.device = torch.device('cpu')
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              self.device = torch.device('cuda')
+          else:
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
 
         elif op =='exp(-1)':
 
           #Appying the inverse exponential to the feature and feature values
           feature = f'{op}({self.columns[i]})'
           value = torch.reciprocal(torch.exp(self.df_feature_values[:,i]))
-          self.feature_values3.append(value.unsqueeze(1))
-          self.feature_names.append(feature)
+          if self.device == 'cuda':
+              self.device = torch.device('cpu')
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              self.device = torch.device('cuda')
+          else:
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
             
     #Check for empty lists 
     if len(self.feature_names) == 0:
         return self.feature_values, self.feature_names
     else:
         # create Boolean masks for NaN and Inf values
         self.feature_values =  torch.cat(self.feature_values3,dim=1)
@@ -236,45 +303,72 @@
         #Extract the values from the original tensor 
         values = torch.tensor(self.df_feature_values[:,index_1]).to(self.device)
         for op in operators_set:
           
           #Apply the conditions of operators
           if op =='+':
             feature_value = torch.add(values[:,0],values[:,1])
-            self.feature_values2.append(feature_value.unsqueeze(1))
             col_name = f'({comb[0]}{op}{comb[1]})'
-            self.feature_names1.append(col_name)
+            if self.device =='cuda':
+                self.device = torch.device('cpu')
+                self.feature_values2.append(feature_value.unsqueeze(1))
+                self.feature_names1.append(col_name)
+                self.device = torch.device('cuda')
+            else:
+                self.feature_values2.append(feature_value.unsqueeze(1))
+                self.feature_names1.append(col_name)
+                
           elif op =='-':
             feature_value = torch.sub(values[:,0],values[:,1])
-            self.feature_values2.append(feature_value.unsqueeze(1))
             col_name = f'({comb[0]}{op}{comb[1]})'
-            self.feature_names1.append(col_name)
-            #feature_value1 = torch.sub(values[:,1],values[:,0]).to(self.device)
-            #self.feature_values2.append(feature_value1.unsqueeze(1))
-            #col_name = f'({comb[1]}{op}{comb[0]})'
-            #self.feature_names1.append(col_name)
+            if self.device =='cuda':
+                self.device = torch.device('cpu')
+                self.feature_values2.append(feature_value.unsqueeze(1))
+                self.feature_names1.append(col_name)
+                self.device = torch.device('cuda')
+            else:
+                self.feature_values2.append(feature_value.unsqueeze(1))
+                self.feature_names1.append(col_name)
           elif op == '*':
             feature_value = torch.mul(values[:,0],values[:,1])
-            self.feature_values2.append(feature_value.unsqueeze(1))
             col_name = f'({comb[0]}{op}{comb[1]})'
-            self.feature_names1.append(col_name)
+            if self.device =='cuda':
+                self.device = torch.device('cpu')
+                self.feature_values2.append(feature_value.unsqueeze(1))
+                self.feature_names1.append(col_name)
+                self.device = torch.device('cuda')
+            else:
+                self.feature_values2.append(feature_value.unsqueeze(1))
+                self.feature_names1.append(col_name)
           elif op =='/':
             feature_value = torch.div(values[:,0],values[:,1])
-            self.feature_values2.append(feature_value.unsqueeze(1))
+            feature_value1 = torch.div(values[:,1],values[:,0])
             col_name = f'({comb[0]}{op}{comb[1]})'
-            self.feature_names1.append(col_name)
-            feature_value1 = torch.div(values[:,1],values[:,0]).to(self.device)
-            self.feature_values2.append(feature_value1.unsqueeze(1))
-            col_name = f'({comb[1]}{op}{comb[0]})'
-            self.feature_names1.append(col_name)
+            col_name1 = f'({comb[1]}{op}{comb[0]})'
+            if self.device =='cuda':
+                self.device = torch.device('cpu')
+                self.feature_values2.append(feature_value.unsqueeze(1))
+                self.feature_names1.append(col_name)
+                self.feature_values2.append(feature_value1.unsqueeze(1))
+                self.feature_names1.append(col_name1)
+                self.device = torch.device('cuda')
+            else:
+                self.feature_values2.append(feature_value.unsqueeze(1))
+                self.feature_names1.append(col_name)
           elif op == 'abs':
             feature_value = torch.abs(torch.sub(values[:,0],values[:,1]))
-            self.feature_values2.append(feature_value.unsqueeze(1))
             col_name = f'(|{comb[0]}-{comb[1]}|)'
-            self.feature_names1.append(col_name)      
+            if self.device =='cuda':
+                self.device = torch.device('cpu')
+                self.feature_values2.append(feature_value.unsqueeze(1))
+                self.feature_names1.append(col_name)
+                self.device = torch.device('cuda')
+            else:
+                self.feature_values2.append(feature_value.unsqueeze(1))
+                self.feature_names1.append(col_name)  
       
       #Checking whether the lists are empty
       if len(self.feature_names1) == 0:
           return self.feature_values1, self.feature_names1
       else:
           #Removing Nan and inf columns from tenosr and corresponding variable name form the list
           self.feature_values1 = torch.cat(self.feature_values2,dim=1)
```

### Comparing `TorchSisso-1.0.1/TorchSisso/Feature_space_construction_1.py` & `TorchSisso-1.0.2/TorchSisso/FeatureSpaceConstruction.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-Created on Thu Jun  1 18:40:28 2023
+Created on Tue May 30 13:31:55 2023
 
 @author: muthyala.7
 """
 
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
@@ -59,24 +59,29 @@
     
     #Creating empty tensor for single operators
     self.feature_values = torch.empty(self.df.shape[0],0).to(self.device)
     self.feature_names = []
     #creating empty tensor for combinations
     self.feature_values1 = torch.empty(self.df.shape[0],0).to(self.device)
     self.feature_names1 = []
+    self.feature_values2 = []
+    self.feature_values3 = []
   '''
   ###############################################################################################################
 
   Construct all the features that can be constructed using the single operators like log, exp, sqrt etc..
 
   ###############################################################################################################
   '''
 
-  def single_variable(self,operators_set):
-    #Check for the validity of the operator set given 
+  def single_variable(self,operators_set): 
+    #Check for the validity of the operator set given
+    self.feature_values = torch.empty(self.df.shape[0],0).to(self.device)
+    self.feature_names = []
+    self.feature_values3 = []
     for op in operators_set:
 
       if op in ['exp','sin','cos','sqrt','cbrt','log','ln','^-1','^2','^3','exp(-1)','abs']:
         continue
       else:
         raise TypeError('Invalid Operator found in the given operator set')
     
@@ -88,213 +93,301 @@
       #Looping over all the initial feature set with the specific operator set 
 
       for i in range(len(self.columns)):
         if op == 'exp':
 
           #Applying the operator and adding to the new dataframe
           feature = f'{op}({self.columns[i]})'
-          value = torch.exp(self.df_feature_values[:,i]).to(self.device)
-          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1).to(self.device)
-          self.feature_names.append(feature)
-          #self.new_features_values[feature] = value.cpu().numpy()
+          value = torch.exp(self.df_feature_values[:,i])
+          if self.device == 'cuda':
+              self.device = torch.device('cpu')
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              self.device = torch.device('cuda')
+          else:
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              
 
         elif op == 'ln':
 
           #Applying the log operator to the feature and feature values\
           #This is the exponential not the base 10
           feature = f'{op}({self.columns[i]})'
-          value = torch.log(self.df_feature_values[:,i]).to(self.device)
-          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1).to(self.device)
-          self.feature_names.append(feature)
-          #self.new_features_values[feature] = value.cpu().numpy()
+          value = torch.log(self.df_feature_values[:,i])
+          if self.device == 'cuda':
+              self.device = torch.device('cpu')
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              self.device = torch.device('cuda')
+          else:
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
         
         elif op == 'sin':
           #Applying the sin operator to the featrure and feature values
           feature = f'{op}({self.columns[i]})'
-          value = torch.sin(self.df_feature_values[:,i]).to(self.device)
-          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1).to(self.device)
-          #self.new_features_values[feature] = value.cpu().numpy()
-          self.feature_names.append(feature)
+          value = torch.sin(self.df_feature_values[:,i])
+          if self.device == 'cuda':
+              self.device = torch.device('cpu')
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              self.device = torch.device('cuda')
+          else:
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
         
         elif op =='log':
 
           #Applying the log10 operator to the feature and feature values
           feature = f'{op}({self.columns[i]})'
-          value = torch.log10(self.df_feature_values[:,i]).to(self.device)
-          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1).to(self.device)
-          self.feature_names.append(feature)
-          #self.new_features_values[feature] = value.cpu().numpy()
+          value = torch.log10(self.df_feature_values[:,i])
+          if self.device == 'cuda':
+              self.device = torch.device('cpu')
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              self.device = torch.device('cuda')
+          else:
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
         
         elif op =='cos':
 
           #Applying the cos operator to the feature and feature values
           feature = f'{op}({self.columns[i]})'
-          value = torch.cos(self.df_feature_values[:,i]).to(self.device)
-          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1).to(self.device)
-          self.feature_names.append(feature)
-#          self.new_features_values[feature] = value.cpu().numpy()
+          value = torch.cos(self.df_feature_values[:,i])
+          if self.device == 'cuda':
+              self.device = torch.device('cpu')
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              self.device = torch.device('cuda')
+          else:
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
         
         elif op =='cbrt':
 
           #Applying the cuberoot function to the feature and feature values 
           feature = f'{op}({self.columns[i]})'
-          value = torch.pow(self.df_feature_values[:,i],1/3).to(self.device)
-          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1).to(self.device)
-          self.feature_names.append(feature)
-#          self.new_features_values[feature] = value.cpu().numpy()
+          value = torch.pow(self.df_feature_values[:,i],1/3)
+          if self.device == 'cuda':
+              self.device = torch.device('cpu')
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              self.device = torch.device('cuda')
+          else:
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
         
         elif op =='sqrt':
 
           #Applying the sqaureroot function to the feature and feature values
           feature = f'{op}({self.columns[i]})'
-          value = torch.sqrt(self.df_feature_values[:,i]).to(self.device)
-          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1).to(self.device)
-          self.feature_names.append(feature)
-#          self.new_features_values[feature] = value.cpu().numpy()
+          value = torch.sqrt(self.df_feature_values[:,i])
+          if self.device == 'cuda':
+              self.device = torch.device('cpu')
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              self.device = torch.device('cuda')
+          else:
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
 
         elif op =='^2':
 
           #Applying the square function to the feature and feature values
           feature = f'({self.columns[i]}){op}'
-          value = torch.pow(self.df_feature_values[:,i],2).to(self.device)
-          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1).to(self.device)
-          self.feature_names.append(feature)
-          #self.new_features_values[feature] = value.cpu().numpy()
+          value = torch.pow(self.df_feature_values[:,i],2)
+          if self.device == 'cuda':
+              self.device = torch.device('cpu')
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              self.device = torch.device('cuda')
+          else:
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
         
         elif op =='^3':
 
           #Applying the cube function to the feature and feature values
           feature = f'({self.columns[i]}){op}'
-          value = torch.pow(self.df_feature_values[:,i],3).to(self.device)
-          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1).to(self.device)
-          self.feature_names.append(feature)
-#          self.new_features_values[feature] = value.cpu().numpy()
+          value = torch.pow(self.df_feature_values[:,i],3)
+          if self.device == 'cuda':
+              self.device = torch.device('cpu')
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              self.device = torch.device('cuda')
+          else:
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
         
         elif op == '^-1':
 
           #Applying the inverse function to the feature and feature valuies
           feature = f'({self.columns[i]}){op}'
-          value = torch.reciprocal(self.df_feature_values[:,i]).to(self.device)
-          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1).to(self.device)
-          self.feature_names.append(feature)
-#          self.new_features_values[feature] = value.cpu().numpy()
+          value = torch.reciprocal(self.df_feature_values[:,i])
+          if self.device == 'cuda':
+              self.device = torch.device('cpu')
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              self.device = torch.device('cuda')
+          else:
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
 
         elif op =='exp(-1)':
 
           #Appying the inverse exponential to the feature and feature values
           feature = f'{op}({self.columns[i]})'
-          value = torch.reciprocal(torch.exp(self.df_feature_values[:,i])).to(self.device)
-          self.feature_values = torch.cat((self.feature_values,value.unsqueeze(1)), dim=1).to(self.device)
-          self.feature_names.append(feature)
-          #self.new_features_values[feature] = value.cpu().numpy()
+          value = torch.reciprocal(torch.exp(self.df_feature_values[:,i]))
+          if self.device == 'cuda':
+              self.device = torch.device('cpu')
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
+              self.device = torch.device('cuda')
+          else:
+              self.feature_values3.append(value.unsqueeze(1))
+              self.feature_names.append(feature)
             
-    # create Boolean masks for NaN and Inf values
-    nan_columns = torch.any(torch.isnan(self.feature_values), dim=0)
-    inf_columns = torch.any(torch.isinf(self.feature_values), dim=0)
-    nan_or_inf_columns = nan_columns | inf_columns
-
-    # Remove columns from tensor
-    self.feature_values = self.feature_values[:, ~nan_or_inf_columns]
-
-    # Remove corresponding elements from list
-    self.feature_names = [elem for i, elem in enumerate(self.feature_names) if not nan_or_inf_columns[i]]
-
-    return self.feature_values, self.feature_names #self.new_features_values
+    #Check for empty lists 
+    if len(self.feature_names) == 0:
+        return self.feature_values, self.feature_names
+    else:
+        # create Boolean masks for NaN and Inf values
+        self.feature_values =  torch.cat(self.feature_values3,dim=1)
+        nan_columns = torch.any(torch.isnan(self.feature_values), dim=0)
+        inf_columns = torch.any(torch.isinf(self.feature_values), dim=0)
+        nan_or_inf_columns = nan_columns | inf_columns
+    
+        # Remove columns from tensor
+        self.feature_values = self.feature_values[:, ~nan_or_inf_columns]
+    
+        # Remove corresponding elements from list
+        self.feature_names = [elem for i, elem in enumerate(self.feature_names) if not nan_or_inf_columns[i]]
+        return self.feature_values, self.feature_names #self.new_features_values
   
 
 
   '''
   ################################################################################################
 
   Defining method to perform the combinations of the variables with the initial feature set
   ################################################################################################
   '''
   def combinations(self,operators_set):
-
+      #creating empty tensor for combinations
+      self.feature_values1 = torch.empty(self.df.shape[0],0).to(self.device)
+      self.feature_names1 = []
+      self.feature_values2 = []
     #Checking for the operator set
       for op in operators_set:
         if op in ['+','-','*','/','abs']:
           continue
         else:
           raise TypeError("Valid set of operators +,-,*,/, abs please check the operators set")
           break
       
       #Defining the set of combinations to be performed
+      import itertools
       from itertools import combinations
 
       #getting list of cobinations without replacement using itertools 
       combinations = list(combinations(self.columns,2))
       #Creating a list for the adding the features combinations created
       #Converting columns to numpy array to support on GPU if not the indexing doesn't support to GPU
       column_array = np.array(self.columns)
       #Applying the operators to the combinations created
       for comb in combinations:
-
-        #Get the index position of the combination created
         index1 = np.where(column_array == comb[0])[0][0]
         index2 = np.where(column_array == comb[1])[0][0]
         index_1 = torch.tensor([index1,index2]).to(self.device)
         #Extract the values from the original tensor 
         values = torch.tensor(self.df_feature_values[:,index_1]).to(self.device)
         for op in operators_set:
           
           #Apply the conditions of operators
           if op =='+':
-            feature_value = torch.add(values[:,0],values[:,1]).to(self.device)
-            #print(feature_value.device,self.feature_values1.device)
-            self.feature_values1 = torch.cat((self.feature_values1,feature_value.unsqueeze(1)), dim=1).to(self.device)
+            feature_value = torch.add(values[:,0],values[:,1])
             col_name = f'({comb[0]}{op}{comb[1]})'
-            self.feature_names1.append(col_name)
-            #print(feature_value.device,self.feature_values1.device)
+            if self.device =='cuda':
+                self.device = torch.device('cpu')
+                self.feature_values2.append(feature_value.unsqueeze(1))
+                self.feature_names1.append(col_name)
+                self.device = torch.device('cuda')
+            else:
+                self.feature_values2.append(feature_value.unsqueeze(1))
+                self.feature_names1.append(col_name)
+                
           elif op =='-':
-            feature_value = torch.sub(values[:,0],values[:,1]).to(self.device)
-            self.feature_values1 = torch.cat((self.feature_values1,feature_value.unsqueeze(1)), dim=1).to(self.device)
+            feature_value = torch.sub(values[:,0],values[:,1])
             col_name = f'({comb[0]}{op}{comb[1]})'
-            self.feature_names1.append(col_name)
-            #feature_value1 = torch.sub(values[:,1],values[:,0]).to(self.device)
-            #self.feature_values1 = torch.cat((self.feature_values1,feature_value1.unsqueeze(1)), dim=1).to(self.device)
-            #col_name = f'({comb[1]}{op}{comb[0]})'
-            #self.feature_names1.append(col_name)
-            #print(feature_value.device,self.feature_values1.device)
+            if self.device =='cuda':
+                self.device = torch.device('cpu')
+                self.feature_values2.append(feature_value.unsqueeze(1))
+                self.feature_names1.append(col_name)
+                self.device = torch.device('cuda')
+            else:
+                self.feature_values2.append(feature_value.unsqueeze(1))
+                self.feature_names1.append(col_name)
           elif op == '*':
-            feature_value = torch.mul(values[:,0],values[:,1]).to(self.device)
-            self.feature_values1 = torch.cat((self.feature_values1,feature_value.unsqueeze(1)), dim=1).to(self.device)
+            feature_value = torch.mul(values[:,0],values[:,1])
             col_name = f'({comb[0]}{op}{comb[1]})'
-            self.feature_names1.append(col_name)
-            #print(feature_value.device,self.feature_values1.device)
+            if self.device =='cuda':
+                self.device = torch.device('cpu')
+                self.feature_values2.append(feature_value.unsqueeze(1))
+                self.feature_names1.append(col_name)
+                self.device = torch.device('cuda')
+            else:
+                self.feature_values2.append(feature_value.unsqueeze(1))
+                self.feature_names1.append(col_name)
           elif op =='/':
-            feature_value = torch.div(values[:,0],values[:,1]).to(self.device)
-            self.feature_values1 = torch.cat((self.feature_values1,feature_value.unsqueeze(1)), dim=1).to(self.device)
+            feature_value = torch.div(values[:,0],values[:,1])
+            feature_value1 = torch.div(values[:,1],values[:,0])
             col_name = f'({comb[0]}{op}{comb[1]})'
-            self.feature_names1.append(col_name)
-            #print(feature_value.device,self.feature_values1.device)
-#            feature_value1 = torch.div(values[:,1],values[:,0]).to(self.device)
-#            self.feature_values1 = torch.cat((self.feature_values1,feature_value1.unsqueeze(1)), dim=1).to(self.device)
-#            col_name = f'({comb[1]}{op}{comb[0]})'
-#            self.feature_names1.append(col_name)
+            col_name1 = f'({comb[1]}{op}{comb[0]})'
+            if self.device =='cuda':
+                self.device = torch.device('cpu')
+                self.feature_values2.append(feature_value.unsqueeze(1))
+                self.feature_names1.append(col_name)
+                self.feature_values2.append(feature_value1.unsqueeze(1))
+                self.feature_names1.append(col_name1)
+                self.device = torch.device('cuda')
+            else:
+                self.feature_values2.append(feature_value.unsqueeze(1))
+                self.feature_names1.append(col_name)
           elif op == 'abs':
-            feature_value = torch.abs(torch.sub(values[:,0],values[:,1])).to(self.device)
-            self.feature_values1 = torch.cat((self.feature_values1,feature_value.unsqueeze(1)), dim=1).to(self.device)
+            feature_value = torch.abs(torch.sub(values[:,0],values[:,1]))
             col_name = f'(|{comb[0]}-{comb[1]}|)'
-            self.feature_names1.append(col_name)
-            print(feature_value.device,self.feature_values1.device)         
+            if self.device =='cuda':
+                self.device = torch.device('cpu')
+                self.feature_values2.append(feature_value.unsqueeze(1))
+                self.feature_names1.append(col_name)
+                self.device = torch.device('cuda')
+            else:
+                self.feature_values2.append(feature_value.unsqueeze(1))
+                self.feature_names1.append(col_name)  
       
-      #Removing Nan and inf columns from tenosr and corresponding variable name form the list
-      nan_columns = torch.any(torch.isnan(self.feature_values1), dim=0)
-      inf_columns = torch.any(torch.isinf(self.feature_values1), dim=0)
-      nan_or_inf_columns = nan_columns | inf_columns
-
-      # Remove columns from tensor
-      self.feature_values1 = self.feature_values1[:, ~nan_or_inf_columns]
-
-      # Remove corresponding elements from list
-      self.feature_names1 = [elem for i, elem in enumerate(self.feature_names1) if not nan_or_inf_columns[i]]
-
-      #Returning the dataframe created
-      return self.feature_values1,self.feature_names1 #created_space
+      #Checking whether the lists are empty
+      if len(self.feature_names1) == 0:
+          return self.feature_values1, self.feature_names1
+      else:
+          #Removing Nan and inf columns from tenosr and corresponding variable name form the list
+          self.feature_values1 = torch.cat(self.feature_values2,dim=1)
+          nan_columns = torch.any(torch.isnan(self.feature_values1), dim=0)
+          inf_columns = torch.any(torch.isinf(self.feature_values1), dim=0)
+          nan_or_inf_columns = nan_columns | inf_columns
+    
+          # Remove columns from tensor
+          self.feature_values1 = self.feature_values1[:, ~nan_or_inf_columns]
+    
+          # Remove corresponding elements from list
+          self.feature_names1 = [elem for i, elem in enumerate(self.feature_names1) if not nan_or_inf_columns[i]]
+    
+          #Returning the dataframe created
+          return self.feature_values1,self.feature_names1 #created_space
   
 
   '''
   ##########################################################################################################
 
   Creating the space based on the given set of conditions
 
@@ -303,48 +396,47 @@
   '''
 
   def feature_space(self):
     #based on the dimension we will be performing the feature space creation
     start_time = time.time()
     basic_operators = [op for op in self.operators if op in ['+', '-', '*', '/']]
     other_operators = [op for op in self.operators if op not in ['+', '-', '*', '/']]
+    
     values, names = self.combinations(basic_operators)
     values1, names1 = self.single_variable(other_operators)
     #Merging two dataframes
     space_created = torch.cat((self.df_feature_values,values,values1), dim=1).to(self.device)
     self.columns = self.columns + names + names1 
     del values, values1, names, names1
-    print('Time for phi 1 creation is: ',time.time() - start_time)
     print('First Feature Space building is completed with features count: ',int(space_created.shape[1]))
+    print('Time for phi1 creation is: ',round(time.time() - start_time,3),' seconds')
     #Update the columns according to the new phi created for the next phase features
     self.df_feature_values = (space_created).to(self.device)
     #Creating the phi2 based on the space created 
     start_time = time.time()
     values, names = self.combinations(basic_operators)
-    print('Time taken for combinations', time.time()-start_time)
     values1, names1 = self.single_variable(other_operators)
     space_created_2 = torch.cat((space_created,values,values1), dim=1).to(self.device)
     self.columns = self.columns + names + names1 
     #######################
     #code to remove duplicate columns from dataframe
     #########################
     #Converting tensor to numpy and then dataframe to remove duplicates
     #space1 = space_created_2.cpu().numpy()
     space = pd.DataFrame(space_created_2.cpu(),columns = self.columns)
     space = space.round(7)
     #space = space.dropna(axis=1, how='any')
     # Transpose the dataframe
     space = space.T.drop_duplicates().T
-
-    print('Time taken to create and remove redundant features in phi2 is ', time.time() - start_time)
     del space_created
     del values, values1, names, names1
     self.columns = space.columns.tolist()
     self.df_feature_values = torch.tensor(space.values).to(self.device)
-    print('Second Feature Space building is completed',space.shape)
+    print('Second Feature Space building is completed with features count: ',int(space.shape[1]))
+    print('Time taken to create and remove redundant features in phi2 is ', round(time.time() - start_time,3), ' seconds')
 
     if self.no_of_operators >3: 
       for i in range(4,self.no_of_operators+1):
         if i == 4:
           values, names = self.combinations(basic_operators)
           values1,names1 = self.single_variable(other_operators)
           space_created_3 = torch.cat((self.df_feature_values,values,values1),dim=1).to(self.device)
```

### Comparing `TorchSisso-1.0.1/TorchSisso/SISSORegressor.py` & `TorchSisso-1.0.2/TorchSisso/SISSORegressor.py`

 * *Files identical despite different names*

### Comparing `TorchSisso-1.0.1/TorchSisso/SISSORegressor_L1L0.py` & `TorchSisso-1.0.2/TorchSisso/SISSORegressor_L1L0.py`

 * *Files identical despite different names*

### Comparing `TorchSisso-1.0.1/TorchSisso/testRegressor.py` & `TorchSisso-1.0.2/TorchSisso/testRegressor.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 Created on Sat May 13 21:101:33 2023
 
 @author: muthyala.7
 """
 
 import FeatureSpaceConstruction
+import Feature_space_construction_1
 import SISSORegressor
 import SISSORegressor_L1L0
 import FC_copy
 import torch
 import numpy as np 
 import pandas as pd 
 import time
@@ -30,32 +31,34 @@
 #######################################################################################################
 '''
 x = [np.random.uniform(0,2,size=10) for i in range(4)]
 df = pd.DataFrame()
 for i in range(len(x)):
   variable = 'x'+str(i+1)
   df[variable] = x[i]
-operators = ['+','/','*']
+operators = ['+','/']
 y = 10*((df.iloc[:,0])/(df.iloc[:,1]*(df.iloc[:,2]+df.iloc[:,3]))) + 3 + 0.01*np.random.normal(0,1,10)
 df.insert(0,'Target',y)
 #df['x10'] = np.random.choice([0, 1], size=len(df), p=[0.100, 0.100])
 start_c = time.time()
-#fc = FeatureSpaceConstruction.feature_space_construction(operators,df,3,'cpu')
+#fc = FeatureSpaceConstruction.feature_space_construction(operators,df,3,'cuda')
 #df_created = fc.feature_space()
+#print(time.time()-start_c)
 start_f = time.time()
 FC = FC_copy.feature_space_construction(operators, df,3,'cpu')
 df_created = FC.feature_space()
+print(time.time()-start_f)
 #print('Time taken to create the feature space: ', time.time()-start_f,' seconds')
 
 #Create Instace for class 
 x = torch.tensor(df_created.iloc[:,1:].values)
 y = torch.tensor(df_created.iloc[:,0])
 names = df_created.iloc[:,1:].columns
 start = time.time()
-sr = SISSORegressor.SISSO_Regressor(x,y,names,1,20,'cpu','L1_L0')
+sr = SISSORegressor.SISSO_Regressor(x,y,names,1,20,'cuda','L1_L0')
 rmse, equation = sr.SISSO()
 print('SISSO Completed',time.time()-start_c,'\n')
 print('\n')
 
 #Implementing LASSO on the initial dataset
 x = df.iloc[:,1:]
 y = df.iloc[:,0]
@@ -119,15 +122,15 @@
 '''
 ##########################################################################################################
 
 #CaseStudy-3
 
 #########################################################################################################
 '''
-x = [np.random.uniform(0,2,size=10) for i in range(4)]
+x = [np.random.uniform(0,2,size=10) for i in range(3)]
 df = pd.DataFrame()
 for i in range(len(x)):
   variable = 'x'+str(i+1)
   df[variable] = x[i]
 y2 = 3*(np.exp(df.iloc[:,3])/(df.iloc[:,2]+np.exp(df.iloc[:,1]))) + 0.01*np.random.normal(0,1,10)
 df.insert(0,'Target',y2)
 operators = ['/','+','exp']
```

### Comparing `TorchSisso-1.0.1/setup.py` & `TorchSisso-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 import setuptools
 
 
 setuptools.setup(
     name="TorchSisso",
-    version="1.0.1",
+    version="1.0.2",
     author="Madhav Muthyala",
     author_email="madhavreddymuthyala@gmail.com",
     description="GPU Supported Sure Independence Screening and Sparsifying Operator Package",
     url="https://github.com/MR1319/TorchSisso",
     packages=setuptools.find_packages(),
     install_requires=[
         "torch",
```

