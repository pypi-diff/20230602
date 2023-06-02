# Comparing `tmp/gmltools-0.0.75.tar.gz` & `tmp/gmltools-0.0.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmltools-0.0.75.tar", last modified: Sun May 28 20:00:25 2023, max compression
+gzip compressed data, was "gmltools-0.0.76.tar", last modified: Fri Jun  2 10:17:30 2023, max compression
```

## Comparing `gmltools-0.0.75.tar` & `gmltools-0.0.76.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 20:00:25.467955 gmltools-0.0.75/
--rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.75/LICENSE
--rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.75/Models.ipynb
--rw-rw-rw-   0        0        0     1021 2023-05-28 20:00:25.464958 gmltools-0.0.75/PKG-INFO
--rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.75/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 20:00:25.043456 gmltools-0.0.75/dist/
--rw-rw-rw-   0        0        0    74791 2023-04-14 10:52:54.000000 gmltools-0.0.75/dist/gmltools-0.0.59.tar.gz
--rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.75/gmltools.yml
--rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.75/mltools.yml
--rw-rw-rw-   0        0        0      546 2023-05-28 19:59:49.000000 gmltools-0.0.75/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-28 20:00:25.467955 gmltools-0.0.75/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-05-28 19:59:42.000000 gmltools-0.0.75/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-28 20:00:24.901303 gmltools-0.0.75/src/
-drwxrwxrwx   0        0        0        0 2023-05-28 20:00:25.088387 gmltools-0.0.75/src/gmltools/
--rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.75/src/gmltools/To_Do.txt
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.75/src/gmltools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 20:00:25.187967 gmltools-0.0.75/src/gmltools/eda/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.75/src/gmltools/eda/__init__.py
--rw-rw-rw-   0        0        0    42993 2023-05-28 19:59:17.000000 gmltools-0.0.75/src/gmltools/eda/eda.py
-drwxrwxrwx   0        0        0        0 2023-05-28 20:00:25.334186 gmltools-0.0.75/src/gmltools/models/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.75/src/gmltools/models/__init__.py
--rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.75/src/gmltools/models/bayes.py
--rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.75/src/gmltools/models/custom_scorings.py
--rw-rw-rw-   0        0        0     5653 2023-05-24 10:54:18.000000 gmltools-0.0.75/src/gmltools/models/dummy_model.py
--rw-rw-rw-   0        0        0   126821 2023-05-26 07:49:29.000000 gmltools-0.0.75/src/gmltools/models/model.py
--rw-rw-rw-   0        0        0     6170 2023-05-22 07:56:38.000000 gmltools-0.0.75/src/gmltools/models/models_info.py
--rw-rw-rw-   0        0        0    13212 2023-05-12 09:20:42.000000 gmltools-0.0.75/src/gmltools/models/timeseriesplit.py
-drwxrwxrwx   0        0        0        0 2023-05-28 20:00:25.386561 gmltools-0.0.75/src/gmltools/models_analysis/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.75/src/gmltools/models_analysis/__init__.py
--rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.75/src/gmltools/models_analysis/classification_analysis.py
--rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.75/src/gmltools/models_analysis/xai.py
-drwxrwxrwx   0        0        0        0 2023-05-28 20:00:25.461433 gmltools-0.0.75/src/gmltools/preprocess/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.75/src/gmltools/preprocess/__init__.py
--rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.75/src/gmltools/preprocess/autoregressive_features.py
--rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.75/src/gmltools/preprocess/manage_holidays.py
--rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.75/src/gmltools/preprocess/preprocess.py
-drwxrwxrwx   0        0        0        0 2023-05-28 20:00:25.159505 gmltools-0.0.75/src/gmltools.egg-info/
--rw-rw-rw-   0        0        0     1021 2023-05-28 20:00:24.000000 gmltools-0.0.75/src/gmltools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      934 2023-05-28 20:00:24.000000 gmltools-0.0.75/src/gmltools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 20:00:24.000000 gmltools-0.0.75/src/gmltools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-05-28 20:00:24.000000 gmltools-0.0.75/src/gmltools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-28 20:00:24.000000 gmltools-0.0.75/src/gmltools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 10:17:30.328075 gmltools-0.0.76/
+-rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.76/LICENSE
+-rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.76/Models.ipynb
+-rw-rw-rw-   0        0        0     1021 2023-06-02 10:17:30.328075 gmltools-0.0.76/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.76/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 10:17:30.138412 gmltools-0.0.76/dist/
+-rw-rw-rw-   0        0        0    74791 2023-04-14 10:52:54.000000 gmltools-0.0.76/dist/gmltools-0.0.59.tar.gz
+-rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.76/gmltools.yml
+-rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.76/mltools.yml
+-rw-rw-rw-   0        0        0      546 2023-06-02 10:15:53.000000 gmltools-0.0.76/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-02 10:17:30.329156 gmltools-0.0.76/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-06-02 10:15:42.000000 gmltools-0.0.76/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:17:30.035285 gmltools-0.0.76/src/
+drwxrwxrwx   0        0        0        0 2023-06-02 10:17:30.160144 gmltools-0.0.76/src/gmltools/
+-rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.76/src/gmltools/To_Do.txt
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.76/src/gmltools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:17:30.207078 gmltools-0.0.76/src/gmltools/eda/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.76/src/gmltools/eda/__init__.py
+-rw-rw-rw-   0        0        0    42538 2023-05-29 11:18:21.000000 gmltools-0.0.76/src/gmltools/eda/eda.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:17:30.273550 gmltools-0.0.76/src/gmltools/models/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.76/src/gmltools/models/__init__.py
+-rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.76/src/gmltools/models/bayes.py
+-rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.76/src/gmltools/models/custom_scorings.py
+-rw-rw-rw-   0        0        0     5653 2023-05-24 10:54:18.000000 gmltools-0.0.76/src/gmltools/models/dummy_model.py
+-rw-rw-rw-   0        0        0   127158 2023-06-02 10:16:23.000000 gmltools-0.0.76/src/gmltools/models/model.py
+-rw-rw-rw-   0        0        0     6170 2023-05-22 07:56:38.000000 gmltools-0.0.76/src/gmltools/models/models_info.py
+-rw-rw-rw-   0        0        0    13212 2023-05-12 09:20:42.000000 gmltools-0.0.76/src/gmltools/models/timeseriesplit.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:17:30.295963 gmltools-0.0.76/src/gmltools/models_analysis/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.76/src/gmltools/models_analysis/__init__.py
+-rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.76/src/gmltools/models_analysis/classification_analysis.py
+-rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.76/src/gmltools/models_analysis/xai.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:17:30.327043 gmltools-0.0.76/src/gmltools/preprocess/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.76/src/gmltools/preprocess/__init__.py
+-rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.76/src/gmltools/preprocess/autoregressive_features.py
+-rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.76/src/gmltools/preprocess/manage_holidays.py
+-rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.76/src/gmltools/preprocess/preprocess.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:17:30.194339 gmltools-0.0.76/src/gmltools.egg-info/
+-rw-rw-rw-   0        0        0     1021 2023-06-02 10:17:29.000000 gmltools-0.0.76/src/gmltools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      934 2023-06-02 10:17:29.000000 gmltools-0.0.76/src/gmltools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 10:17:29.000000 gmltools-0.0.76/src/gmltools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-06-02 10:17:29.000000 gmltools-0.0.76/src/gmltools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-02 10:17:29.000000 gmltools-0.0.76/src/gmltools.egg-info/top_level.txt
```

### Comparing `gmltools-0.0.75/LICENSE` & `gmltools-0.0.76/LICENSE`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.75/Models.ipynb` & `gmltools-0.0.76/Models.ipynb`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.75/PKG-INFO` & `gmltools-0.0.76/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.75
+Version: 0.0.76
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.75/README.md` & `gmltools-0.0.76/README.md`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.75/dist/gmltools-0.0.59.tar.gz` & `gmltools-0.0.76/dist/gmltools-0.0.59.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.75/gmltools.yml` & `gmltools-0.0.76/gmltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.75/mltools.yml` & `gmltools-0.0.76/mltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.75/pyproject.toml` & `gmltools-0.0.76/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gmltools"
-version = "0.0.75"
+version = "0.0.76"
 description = "Machine Learning library aiming for a higher level programming, organizing best tools"
 authors = ["Diego Sanz-Gadea Sánchez"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gmltools-0.0.75/setup.py` & `gmltools-0.0.76/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.3,<4.0.0', 'numpy>=1.21.6,<2.0.0', 'pandas>=1.5.0,<2.0.0', 'xgboost==1.5.0']
 
 setup_kwargs = {
     'name': 'gmltools',
-    'version': '0.0.75',
+    'version': '0.0.76',
     'description': 'Machine Learning library aiming for a higher level programming, organizing best tools',
     'long_description': '# gmltools\n\nMachine Learning library aiming for a higher level programming, organizing best tools\n\n```bash\n$ pip install gmltools\n```\n\n## Usage\n\n- TODO\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`gmltutils` was created by Diego Sanz-Gadea Sánchez. It is licensed under the terms of the GNU General Public License v3.0 license.\n\n## Credits\n\n`gmltutils` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'Diego Sanz-Gadea Sánchez',
     'author_email': 'dsanzgadeasanchez@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `gmltools-0.0.75/src/gmltools/To_Do.txt` & `gmltools-0.0.76/src/gmltools/To_Do.txt`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.75/src/gmltools/eda/eda.py` & `gmltools-0.0.76/src/gmltools/eda/eda.py`

 * *Files 0% similar despite different names*

```diff
@@ -521,16 +521,15 @@
             
             pio.write_image(fig, save_path + f'{title}_correlation_heatmap.png')
 
 
 
 
 
-    def plot_distribution(self, bins:int=50, figsize:tuple=(600, 400), save_name="", category_column=None, x_range=None, shared_yaxes:bool=False, shared_xaxes:bool=False, histnorm=None, label_size:int=14, tick_size:int=12, title_size:int=16
-                          , save=False, save_path="./imgs/distributions/"):
+    def plot_distribution(self, bins:int=50, figsize:tuple=(600, 400), save_name="", category_column=None, x_range=None, shared_yaxes:bool=False, shared_xaxes:bool=False, histnorm=None, label_size:int=14, tick_size:int=12, title_size:int=16):
         """
         Plot the distribution of the numeric columns in the dataset. When category_column is provided, the distribution of each category is plotted 
         with the boxplot. Otherwise, the distribution of the entire dataset is plotted with the histogram. You can select the number of bins for the histogram,
         the range of the x-axis and the type of normalization for the histogram. histnorm="probability density" or None.
 
         Parameters
         ----------
@@ -584,23 +583,15 @@
             #add the subplot title
             hist.update_yaxes(title_text="Count", title_font=dict(size=label_size), tickfont=dict(size=tick_size))
 
             hist.update_layout(height=figsize[1], width=figsize[0], title_text=f"Distribution of {col_}", title_font=dict(size=title_size), title_x=0.5)
             hist.show()
 
                     # Check if save is set to True
-            if save:
-                # Check if the directory exists
-                if not os.path.exists(save_path):
-                    # If the directory does not exist, create it
-                    os.makedirs(save_path)
-
-                # Save the figure
-                # Save the figure
-                hist.write_image(save_path + f'{col_}_dist_{save_name}.png')
+
 
                 #pio.write_image(hist, save_path + f'{col_}_dist_{save_name}.png')
 
 
 
     def correlation_sum_combinations(self , target_var:str,remove_vars:list=None):
         """
```

### Comparing `gmltools-0.0.75/src/gmltools/models/bayes.py` & `gmltools-0.0.76/src/gmltools/models/bayes.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.75/src/gmltools/models/custom_scorings.py` & `gmltools-0.0.76/src/gmltools/models/custom_scorings.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.75/src/gmltools/models/dummy_model.py` & `gmltools-0.0.76/src/gmltools/models/dummy_model.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.75/src/gmltools/models/model.py` & `gmltools-0.0.76/src/gmltools/models/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1163,15 +1163,15 @@
         self.model = None
         self.model_name = model_name
         self.X_train = X_train
         self.y_train = y_train
         self.X_prev = X_prev
         self.cv = cv
 
-    def RandomForest_Regressor(self,  ordinal_cat_cols=None, scoring='neg_mean_squared_error', criterion="friedman_mse",
+    def RandomForest_Regressor(self,  ordinal_cat_cols=None, categories='auto', scoring='neg_mean_squared_error', criterion="friedman_mse",
                             grid_params={'RF__n_estimators': [100, 200, 300, 400, 500],
                                 'RF__max_depth': [3,5,7,10],
                                 'RF__min_samples_split': [2,3,4],
                                 'RF__min_samples_leaf': [4,5,6],
                                 'RF__max_features': ['auto','sqrt','log2',None]}, 
                             random_params=None, random_n_iter = 10, bayes_pbounds=None, 
                             bayes_int_params=None, bayes_n_iter = 30, sample_weight=None, random_state=None, n_jobs=-1, 
@@ -1247,15 +1247,15 @@
             elif random_params is not None:
                 assert all('RF__' in s for s in random_params.keys()), "In case of random search, random_params must start with 'RF__'"
             elif bayes_pbounds is not None:
                 assert all('RF__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'RF__'"
                 assert all('RF__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'RF__'"
 
             #Preprocess the data automatically
-            preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols)
+            preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols,categories=categories)
             pipe = Pipeline(steps=[('Prep', preprocessor),
                                 ('RF', RandomForestRegressor(criterion=criterion,random_state=random_state,n_jobs=n_jobs))]) # Model always the last step
             #Select Grid Search, Random Search or Bayesian Optimization
             select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=self.cv,n_jobs=n_jobs)
             select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
             self.model=select_searchcv.fit(X_prev=self.X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
             
@@ -1265,15 +1265,15 @@
             
             self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
                                         'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
                                         'scoring':str(scoring), 'cv':str(self.cv), 'criterion':str(criterion), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
             print(self.model.best_params_)
 
     
-    def XGB_Regressor(self, ordinal_cat_cols=None, scoring='neg_mean_squared_error',
+    def XGB_Regressor(self, ordinal_cat_cols=None, categories='auto', scoring='neg_mean_squared_error',
                             grid_params={'XGB__n_estimators': [100, 200, 300, 400, 500],
                                 'XGB__max_depth': [3,5,7,10],
                                 'XGB__learning_rate': [0.01,0.05,0.1,0.15,0.2],
                                 'XGB__min_child_weight': [1,3,5,7],
                                 'XGB__gamma': [0.0,0.1,0.2,0.3,0.4],
                                 'XGB__colsample_bytree': [0.3,0.4,0.5,0.7]}, 
                             random_params=None, random_n_iter=10, bayes_pbounds=None, bayes_int_params=None,
@@ -1350,15 +1350,15 @@
                 assert all('XGB__' in s for s in random_params.keys()), "In case of random search, random_params must start with 'XGB__'"
             elif bayes_pbounds is not None:
                 assert all('XGB__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'XGB__'"
                 assert all('XGB__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'XGB__'"
             
 
             #Preprocess the data automatically
-            preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols)
+            preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols,categories=categories)
             pipe = Pipeline(steps=[('Prep', preprocessor),
                                 ('XGB', XGBRegressor(random_state=random_state,n_jobs=n_jobs,verbosity=verbosity))]) # Model always the last step
             #Select Grid Search, Random Search or Bayesian Optimization
             select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=self.cv,n_jobs=n_jobs)
             select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
             self.model=select_searchcv.fit(X_prev=self.X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
             
@@ -1369,15 +1369,15 @@
             self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
                                         'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
                                         'scoring':str(scoring), 'cv':str(self.cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
             print(self.model.best_params_)
 
 
     
-    def Linear_Regression(self,  ordinal_cat_cols=None, scoring='neg_mean_squared_error',
+    def Linear_Regression(self,  ordinal_cat_cols=None, categories='auto', scoring='neg_mean_squared_error',
                             grid_params={'LR__fit_intercept': [True, False],
                                 'LR__normalize': [True, False],
                                 'LR__copy_X': [True, False]}, 
                             random_params=None, random_n_iter=10, bayes_pbounds=None,
                             bayes_int_params=None, bayes_n_iter=30, sample_weight=None, random_state=None, n_jobs=-1,
                             columns_lags=None, column_rolled_lags=None,lags=None,rolled_lags=None, rolled_metrics=None, column_rolled_lags_initial=None):
             
@@ -1449,15 +1449,15 @@
                 assert all('LR__' in s for s in grid_params.keys()), "In case of grid search, grid_param_grid must start with 'LR__'"
             elif random_params is not None:
                 assert all('LR__' in s for s in random_params.keys()), "In case of random search, random_params must start with 'LR__'"
             elif bayes_pbounds is not None:
                 assert all('LR__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'LR__'"
                 assert all('LR__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'LR__'"
             
-            preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols)
+            preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols,categories=categories)
             pipe = Pipeline(steps=[('Prep', preprocessor),
                                 ('LR', LinearRegression())]) # Model always the last step
             #Select Grid Search, Random Search or Bayesian Optimization
             select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=self.cv,n_jobs=n_jobs)
             select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
             self.model=select_searchcv.fit(X_prev=self.X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
             
@@ -1467,15 +1467,15 @@
             
             self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
                                         'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
                                         'scoring':str(scoring), 'cv':str(self.cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
             print(self.model.best_params_)
 
     
-    def KNN_Regressor(self, ordinal_cat_cols=None, scoring='neg_mean_squared_error',
+    def KNN_Regressor(self, ordinal_cat_cols=None, categories='auto', scoring='neg_mean_squared_error',
                             grid_params={'KNN__n_neighbors': [3,5,7,9,11,13,15,17,19,21,23,25,27,29,31,33,35,37,39,41,43,45,47,49,51,53,55,57,59,61,63,65,67,69,71,73,75,77,79,81,83,85,87,89,91,93,95,97,99],
                                 'KNN__weights': ['uniform', 'distance'],
                                 'KNN__algorithm': ['auto', 'ball_tree', 'kd_tree', 'brute'],
                                 'KNN__leaf_size': [10,20,30,40,50,60,70,80,90,100],
                                 'KNN__p': [1,2]}, 
                             random_params=None, random_n_iter=10, bayes_pbounds=None, bayes_int_params=None,
                             bayes_n_iter=30, sample_weight=None ,random_state=None, n_jobs=-1, 
@@ -1549,15 +1549,15 @@
                 assert all('KNN__' in s for s in grid_params.keys()), "In case of grid search, grid_param_grid must start with 'KNN__'"
             elif random_params is not None:
                 assert all('KNN__' in s for s in random_params.keys()), "In case of random search, random_params must start with 'KNN__'"
             elif bayes_pbounds is not None:
                 assert all('KNN__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'KNN__'"
                 assert all('KNN__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'KNN__'"
 
-            preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols)
+            preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols,categories=categories)
             pipe = Pipeline(steps=[('Prep', preprocessor),
                                 ('KNN', KNeighborsRegressor())]) # Model always the last step
             #Select Grid Search, Random Search or Bayesian Optimization
             select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=self.cv,n_jobs=n_jobs)
             select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
             self.model=select_searchcv.fit(X_prev=self.X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
             
@@ -1569,15 +1569,15 @@
                                         'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
                                         'scoring':str(scoring), 'cv':str(self.cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
             print(self.model.best_params_)
     
 
 
     
-    def DecisionTree_Regressor(self, ordinal_cat_cols=None, scoring='neg_mean_squared_error',
+    def DecisionTree_Regressor(self, ordinal_cat_cols=None, categories='auto', scoring='neg_mean_squared_error',
                             grid_params={'DT__criterion': ["squared_error", "friedman_mse", "absolute_error", "poisson"],
                                 'DT__max_depth': [None,2,3,4,5],
                                 'DT__min_samples_split': [2,3,4,],
                                 'DT__max_features': ['auto', 'sqrt', 'log2'],
                                 'DT__min_impurity_decrease': [0.0,0.1,0.2]}, 
                             random_params=None, random_n_iter=10, bayes_pbounds=None,
                             bayes_int_params=None, bayes_n_iter=30, sample_weight=None, random_state=None, n_jobs=-1,
@@ -1651,15 +1651,15 @@
                 assert all('DT__' in s for s in grid_params.keys()), "In case of grid search, grid_param_grid must start with 'DT__'"
             elif random_params is not None:
                 assert all('DT__' in s for s in random_params.keys()), "In case of random search, random_params must start with 'DT__'"
             elif bayes_pbounds is not None:
                 assert all('DT__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'DT__'"
                 assert all('DT__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'DT__'"
             
-            preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols)
+            preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols,categories=categories)
             pipe = Pipeline(steps=[('Prep', preprocessor),
                                 ('DT', DecisionTreeRegressor(random_state=random_state))]) # Model always the last step
             #Select Grid Search, Random Search or Bayesian Optimization
             select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=self.cv,n_jobs=n_jobs)
             select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
             self.model=select_searchcv.fit(X_prev=self.X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
             
@@ -1669,15 +1669,15 @@
             
             self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
                                         'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
                                         'scoring':str(scoring), 'cv':str(self.cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
             print(self.model.best_params_)
 
     
-    def MLP_Regressor(self, ordinal_cat_cols=None, scoring='neg_mean_squared_error',
+    def MLP_Regressor(self, ordinal_cat_cols=None, categories='auto', scoring='neg_mean_squared_error',
                             grid_params={'MLP__hidden_layer_sizes': [(3,),(5,)],
                                 'MLP__activation': ['identity', 'logistic', 'tanh', 'relu'],
                                 'MLP__solver': ['lbfgs', 'sgd', 'adam'],
                                 'MLP__alpha': [0.0001,0.001,0.01,0.1,1,10,100],
                                 'MLP__max_iter': [200]},
                             random_params=None, random_n_iter=10,bayes_pbounds=None,
                             bayes_int_params=None, bayes_n_iter=30, sample_weight=None,random_state=None, n_jobs=-1,
@@ -1756,15 +1756,15 @@
                 assert all('MLP__' in s for s in grid_params.keys()), "In case of grid search, grid_param_grid must start with 'MLP__'"
             elif random_params is not None:
                 assert all('MLP__' in s for s in random_params.keys()), "In case of random search, random_params must start with 'MLP__'"
             elif bayes_pbounds is not None:
                 assert all('MLP__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'MLP__'"
                 assert all('MLP__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'MLP__'"
 
-            preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols)
+            preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols,categories=categories)
             pipe = Pipeline(steps=[('Prep', preprocessor),
                                 ('MLP', MLPRegressor(random_state=random_state))]) # Model always the last step
             #Select Grid Search, Random Search or Bayesian Optimization
             select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=self.cv,n_jobs=n_jobs)
             select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
             self.model=select_searchcv.fit(X_prev=self.X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
             
@@ -1775,15 +1775,15 @@
             self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
                                         'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
                                         'scoring':str(scoring), 'cv':str(self.cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
         
             print(self.model.best_params_)
 
 
-    def SVR_Regressor(self, ordinal_cat_cols=None, scoring='neg_mean_squared_error',
+    def SVR_Regressor(self, ordinal_cat_cols=None, categories='auto', scoring='neg_mean_squared_error',
                             grid_params={'SVR__kernel':['linear','poly','rbf'],
                                 'SVR__C': [0.00001,0.0001,0.001,0.01,0.1,1,10,100,1000],
                                 'SVR__gamma':[0.0001,0.001,0.01,0.1,1,10]}, 
                             random_params=None, random_n_iter=10, bayes_pbounds=None,
                             bayes_int_params=None, bayes_n_iter=30, sample_weight=None, n_jobs=-1,
                             columns_lags=None, column_rolled_lags=None,lags=None,rolled_lags=None, rolled_metrics=None, column_rolled_lags_initial=None):
             
@@ -1857,15 +1857,15 @@
                 assert all('SVR__' in s for s in grid_params.keys()), "In case of grid search, grid_param_grid must start with 'SVR__'"
             elif random_params is not None:
                 assert all('SVR__' in s for s in random_params.keys()), "In case of random search, random_params must start with 'SVR__'"
             elif bayes_pbounds is not None:
                 assert all('SVR__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'SVR__'"
                 assert all('SVR__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'SVR__'"
             
-            preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols)
+            preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols,categories=categories)
             pipe = Pipeline(steps=[('Prep', preprocessor),
                                 ('SVR', SVR())]) # Model always the last step
             #Select Grid Search, Random Search or Bayesian Optimization
             select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=self.cv,n_jobs=n_jobs)
             select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
             self.model=select_searchcv.fit(X_prev=self.X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
             
@@ -1956,15 +1956,15 @@
         """
         assert self.model_name in os.listdir('./models'), "Model not found"
         assert self.model_name+'.joblib' in os.listdir(f'./models/{self.model_name}'), "Model not found"
         path = f'./models/{self.model_name}/{self.model_name}'+'.joblib'
         self.model = joblib.load(path)
         return self.model
     
-    def _automatic_preprocessor(self, X_train, ordinal_cat_cols:List[str]=None):
+    def _automatic_preprocessor(self, X_train, ordinal_cat_cols:List[str]=None,categories:List[str]='auto'):
         #Arguments assertion not needed because they are already checked in the model method of the classes that are the ones that call this function
         """
         This function performs a preprocessor for the data. It automatically detects the categorical and numeric variables and performs the following steps:
             - Numeric variables: imputation by scaling. STANDARD SCALER
             - Categorical variables: imputation by encoding. ONE HOT ENCODER
             - Ordinal categorical variables: imputation by encoding. ORDINAL ENCODER
 
@@ -1989,15 +1989,15 @@
             ordinal_cat_cols = []
         else:
             for col in ordinal_cat_cols:
                 cat_cols.remove(col)
             cat_cols_onehot = cat_cols
 
         # Prepare the categorical variables by encoding the categories    
-        categorical_transformer_onehot = Pipeline(steps=[('onehot', OneHotEncoder(handle_unknown='ignore', drop='first'))])
+        categorical_transformer_onehot = Pipeline(steps=[('onehot', OneHotEncoder(handle_unknown='ignore', drop='first',categories=categories))])
         categorical_transformer_ordinal = Pipeline(steps=[('ordinal', OrdinalEncoder())])
         # Prepare the numeric variables by imputing by scaling
         numeric_transformer = Pipeline(steps=[('scaler', StandardScaler())])
 
         preprocessor = ColumnTransformer(transformers=[
             ('num', numeric_transformer, num_cols), #numeric variables
             ('cat_onehot', categorical_transformer_onehot, cat_cols_onehot), #categorical variables
```

### Comparing `gmltools-0.0.75/src/gmltools/models/models_info.py` & `gmltools-0.0.76/src/gmltools/models/models_info.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.75/src/gmltools/models/timeseriesplit.py` & `gmltools-0.0.76/src/gmltools/models/timeseriesplit.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.75/src/gmltools/models_analysis/classification_analysis.py` & `gmltools-0.0.76/src/gmltools/models_analysis/classification_analysis.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.75/src/gmltools/models_analysis/xai.py` & `gmltools-0.0.76/src/gmltools/models_analysis/xai.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.75/src/gmltools/preprocess/autoregressive_features.py` & `gmltools-0.0.76/src/gmltools/preprocess/autoregressive_features.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.75/src/gmltools/preprocess/manage_holidays.py` & `gmltools-0.0.76/src/gmltools/preprocess/manage_holidays.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.75/src/gmltools/preprocess/preprocess.py` & `gmltools-0.0.76/src/gmltools/preprocess/preprocess.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.75/src/gmltools.egg-info/PKG-INFO` & `gmltools-0.0.76/src/gmltools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.75
+Version: 0.0.76
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.75/src/gmltools.egg-info/SOURCES.txt` & `gmltools-0.0.76/src/gmltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

