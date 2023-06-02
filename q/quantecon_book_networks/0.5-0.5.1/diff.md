# Comparing `tmp/quantecon_book_networks-0.5.tar.gz` & `tmp/quantecon_book_networks-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantecon_book_networks-0.5.tar", last modified: Wed May 31 23:24:21 2023, max compression
+gzip compressed data, was "quantecon_book_networks-0.5.1.tar", last modified: Fri Jun  2 10:49:46 2023, max compression
```

## Comparing `quantecon_book_networks-0.5.tar` & `quantecon_book_networks-0.5.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1809 2023-05-31 23:24:02.097214 quantecon_book_networks-0.5/.gitignore
--rw-r--r--   0        0        0     1066 2022-04-26 05:31:28.511561 quantecon_book_networks-0.5/LICENSE
--rw-r--r--   0        0        0      516 2022-04-27 00:12:00.909091 quantecon_book_networks-0.5/README.md
--rw-r--r--   0        0        0      594 2023-05-31 23:24:02.097333 quantecon_book_networks-0.5/pyproject.toml
--rw-r--r--   0        0        0      149 2023-05-31 23:24:02.097457 quantecon_book_networks-0.5/quantecon_book_networks/__init__.py
--rw-r--r--   0        0        0      415 2022-05-10 03:48:00.023039 quantecon_book_networks-0.5/quantecon_book_networks/configure.py
--rw-r--r--   0        0        0    13273 2023-05-31 23:24:02.097618 quantecon_book_networks-0.5/quantecon_book_networks/data.py
--rw-r--r--   0        0        0     3049 2023-05-31 23:24:02.097710 quantecon_book_networks-0.5/quantecon_book_networks/data/README.md
--rw-r--r--   0        0        0    49091 2022-03-10 22:35:44.809827 quantecon_book_networks-0.5/quantecon_book_networks/data/commercial-aircraft-sitcr2-7924-yr2019/sitcr2-7924-aircraft-network-2019-layout.json
--rw-r--r--   0        0        0    29687 2022-03-10 22:35:44.810127 quantecon_book_networks-0.5/quantecon_book_networks/data/commercial-aircraft-sitcr2-7924-yr2019/sitcr2-7924-aircraft-network-2019.gexf
--rw-r--r--   0        0        0    69048 2023-05-31 23:24:02.098083 quantecon_book_networks-0.5/quantecon_book_networks/data/crude_oil_sitcr2_3330_yr2021/data.csv
--rw-r--r--   0        0        0    20758 2023-05-31 23:24:02.098427 quantecon_book_networks-0.5/quantecon_book_networks/data/crude_oil_sitcr2_3330_yr2021/regions-iso3c.csv
--rw-r--r--   0        0        0   221879 2023-05-31 23:24:02.099810 quantecon_book_networks-0.5/quantecon_book_networks/data/crude_oil_sitcr2_3330_yr2021/sankey-diagram-crude-oil-sitc3330-yr2019.png
--rw-r--r--   0        0        0     2164 2023-05-31 23:24:02.099914 quantecon_book_networks-0.5/quantecon_book_networks/data/csv_files/adjacency_matrix_31-12-2022.csv
--rw-r--r--   0        0        0   118381 2022-03-10 22:35:44.814135 quantecon_book_networks-0.5/quantecon_book_networks/data/csv_files/forbes-global2000.csv
--rw-r--r--   0        0        0    30803 2023-05-31 23:24:02.100172 quantecon_book_networks-0.5/quantecon_book_networks/data/csv_files/make_114_aus_20-21.csv
--rw-r--r--   0        0        0     2812 2023-05-31 23:24:02.100270 quantecon_book_networks-0.5/quantecon_book_networks/data/csv_files/make_15_2021.csv
--rw-r--r--   0        0        0    27013 2023-05-31 23:24:02.100577 quantecon_book_networks-0.5/quantecon_book_networks/data/csv_files/make_71_2021.csv
--rw-r--r--   0        0        0    33877 2023-05-31 23:24:02.100670 quantecon_book_networks-0.5/quantecon_book_networks/data/csv_files/use_114_aus_20-21.csv
--rw-r--r--   0        0        0     4848 2023-05-31 23:24:02.100762 quantecon_book_networks-0.5/quantecon_book_networks/data/csv_files/use_15_2021.csv
--rw-r--r--   0        0        0    36530 2023-05-31 23:24:02.100869 quantecon_book_networks-0.5/quantecon_book_networks/data/csv_files/use_71_2021.csv
--rw-r--r--   0        0        0     4162 2023-05-31 23:24:02.101021 quantecon_book_networks-0.5/quantecon_book_networks/input_output.py
--rw-r--r--   0        0        0     4518 2023-05-31 23:24:02.101146 quantecon_book_networks-0.5/quantecon_book_networks/plotting.py
--rw-r--r--   0        0        0      987 1970-01-01 00:00:00.000000 quantecon_book_networks-0.5/PKG-INFO
+-rw-r--r--   0        0        0     1809 2023-05-31 23:24:02.097214 quantecon_book_networks-0.5.1/.gitignore
+-rw-r--r--   0        0        0     1066 2022-04-26 05:31:28.511561 quantecon_book_networks-0.5.1/LICENSE
+-rw-r--r--   0        0        0      516 2022-04-27 00:12:00.909091 quantecon_book_networks-0.5.1/README.md
+-rw-r--r--   0        0        0      594 2023-05-31 23:24:02.097333 quantecon_book_networks-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      151 2023-06-02 10:49:25.040650 quantecon_book_networks-0.5.1/quantecon_book_networks/__init__.py
+-rw-r--r--   0        0        0      415 2022-05-10 03:48:00.023039 quantecon_book_networks-0.5.1/quantecon_book_networks/configure.py
+-rw-r--r--   0        0        0    13210 2023-06-02 10:49:25.040833 quantecon_book_networks-0.5.1/quantecon_book_networks/data.py
+-rw-r--r--   0        0        0     3135 2023-06-02 10:49:25.040995 quantecon_book_networks-0.5.1/quantecon_book_networks/data/README.md
+-rw-r--r--   0        0        0    29687 2023-06-02 10:49:25.041522 quantecon_book_networks-0.5.1/quantecon_book_networks/data/commercial_aircraft/aircraft_network.gexf
+-rw-r--r--   0        0        0    49091 2023-06-02 10:49:25.041958 quantecon_book_networks-0.5.1/quantecon_book_networks/data/commercial_aircraft/aircraft_network_layout.json
+-rw-r--r--   0        0        0    69048 2023-06-02 10:49:25.042314 quantecon_book_networks-0.5.1/quantecon_book_networks/data/crude_oil/data.csv
+-rw-r--r--   0        0        0    20758 2023-06-02 10:49:25.042623 quantecon_book_networks-0.5.1/quantecon_book_networks/data/crude_oil/regions-iso3c.csv
+-rw-r--r--   0        0        0   221879 2023-06-02 10:49:25.044151 quantecon_book_networks-0.5.1/quantecon_book_networks/data/crude_oil/sankey-diagram-crude-oil-sitc3330-yr2019.png
+-rw-r--r--   0        0        0     2164 2023-06-02 10:49:25.044259 quantecon_book_networks-0.5.1/quantecon_book_networks/data/csv_files/adjacency_matrix.csv
+-rw-r--r--   0        0        0   118381 2022-03-10 22:35:44.814135 quantecon_book_networks-0.5.1/quantecon_book_networks/data/csv_files/forbes-global2000.csv
+-rw-r--r--   0        0        0    30803 2023-06-02 10:49:25.044655 quantecon_book_networks-0.5.1/quantecon_book_networks/data/csv_files/make_114_aus.csv
+-rw-r--r--   0        0        0     2812 2023-06-02 10:49:25.044871 quantecon_book_networks-0.5.1/quantecon_book_networks/data/csv_files/make_15.csv
+-rw-r--r--   0        0        0    27013 2023-06-02 10:49:25.045268 quantecon_book_networks-0.5.1/quantecon_book_networks/data/csv_files/make_71.csv
+-rw-r--r--   0        0        0    33877 2023-06-02 10:49:25.045359 quantecon_book_networks-0.5.1/quantecon_book_networks/data/csv_files/use_114_aus.csv
+-rw-r--r--   0        0        0     4848 2023-06-02 10:49:25.045448 quantecon_book_networks-0.5.1/quantecon_book_networks/data/csv_files/use_15.csv
+-rw-r--r--   0        0        0    36530 2023-06-02 10:49:25.045545 quantecon_book_networks-0.5.1/quantecon_book_networks/data/csv_files/use_71.csv
+-rw-r--r--   0        0        0     4162 2023-05-31 23:24:02.101021 quantecon_book_networks-0.5.1/quantecon_book_networks/input_output.py
+-rw-r--r--   0        0        0     4518 2023-05-31 23:24:02.101146 quantecon_book_networks-0.5.1/quantecon_book_networks/plotting.py
+-rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 quantecon_book_networks-0.5.1/PKG-INFO
```

### Comparing `quantecon_book_networks-0.5/.gitignore` & `quantecon_book_networks-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `quantecon_book_networks-0.5/LICENSE` & `quantecon_book_networks-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quantecon_book_networks-0.5/README.md` & `quantecon_book_networks-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `quantecon_book_networks-0.5/pyproject.toml` & `quantecon_book_networks-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quantecon_book_networks-0.5/quantecon_book_networks/data.py` & `quantecon_book_networks-0.5.1/quantecon_book_networks/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numpy as np
 import pandas as pd
 import networkx as nx
 import json
 from pandas_datareader import wb
 
 ## Utilities
-def read_Z(data_file='data/csv_files/adjacency_matrix_31-12-2022.csv', t=10):
+def read_Z(data_file='data/csv_files/adjacency_matrix.csv', t=10):
     """
     Build the Z matrix from the use table.
     
     * Z[i, j] = sales from sector i to sector j
     
     """
     data_file = pkg_resources.resource_stream(__name__, data_file)
@@ -29,15 +29,15 @@
 
     Z = np.asarray(df3.values.tolist(), dtype=np.float64)
     Z_visual = np.where(Z < t, 0, Z)
     
     output = {'Z':Z,'Z_visual':Z_visual, 'countries':countries}
     return output
 
-def read_industry_Z(data_file='data/csv_files/use_15_2021.csv', 
+def read_industry_Z(data_file='data/csv_files/use_15.csv', 
            N=15, 
            columnlist=['Name',
                        'Total Intermediate',
                        'Personal consumption expenditures',
                        'Private fixed investment',
                        'Change in private inventories',
                        'Exports of goods and services',
@@ -56,25 +56,25 @@
         df3 = df2.drop(columns=columnlist)
     else:
         df3 = df2
     df4 = df3.replace('---', 0)
     Z = np.asarray(df4.values.tolist(), dtype=np.float64)
     return Z
 
-def read_industry_X(data_file='data/csv_files/make_15_2021.csv',
+def read_industry_X(data_file='data/csv_files/make_15.csv',
            colname='Total Industry Output',
            N=15):
     """
     Read total industry sales column from the make table.
 
     """
     data_file = pkg_resources.resource_stream(__name__, data_file)
     df5 = pd.read_csv(data_file)
     X = np.asarray(df5[colname])
-    X = X[0:N].astype(np.float)
+    X = X[0:N].astype(np.float64)
     return X
 
 
 def build_coefficient_matrices(Z, X):
     """
     Build coefficient matrices A and F from Z and X via 
     
@@ -100,39 +100,39 @@
         Returns:
             ch_data (dict): Dictionary of data names and associated data objects. Note: some data objects are further nested as dictionaries. 
     """
     
     ch_data = {}
 
     ## Crude oil
-    data_file = "data/crude_oil_sitcr2_3330_yr2021/data.csv"
+    data_file = "data/crude_oil/data.csv"
     data_file = pkg_resources.resource_stream(__name__, data_file)
     crude_oil = pd.read_csv(data_file, dtype={'product_id': str})
 
-    exporters = crude_oil.groupby(by=["location_code"]).sum().sort_values("export_value", ascending=False)[:10].index
-
-    importers = crude_oil.groupby(by=["partner_code"]).sum().sort_values("export_value", ascending=False)[:21].index
+    exporters = crude_oil[["export_value", "location_code"]].groupby(by=["location_code"]).sum().sort_values("export_value", ascending=False)[:10].index
+    
+    importers = crude_oil[["export_value", "partner_code"]].groupby(by=["partner_code"]).sum().sort_values("export_value", ascending=False)[:21].index
     # importers = set(importers.drop("ANS"))
     importers = set(importers)
 
     # Aggregate Data for Rest of the World
     row_concord = {}
     other_importers = set(crude_oil.partner_code.unique()).difference(importers)
     for cntry in other_importers:
         row_concord[cntry] = "ROW"
     importers.add("ROW")
     importers = pd.Index(importers, name='partner_code')
 
     # Aggregate Partner Locations
     crude_oil.partner_code = crude_oil.partner_code.replace(to_replace=row_concord)
 
-    chart_data = crude_oil.groupby(by=["location_code", "partner_code"]).sum().reset_index()
+    chart_data = crude_oil[["export_value", "location_code", "partner_code"]].groupby(by=["location_code", "partner_code"]).sum().reset_index()
 
     # country data
-    data_file = "data/crude_oil_sitcr2_3330_yr2021/regions-iso3c.csv"
+    data_file = "data/crude_oil/regions-iso3c.csv"
     data_file = pkg_resources.resource_stream(__name__, data_file)
     cdata = pd.read_csv(data_file)
     country_names = cdata[["alpha-3","name"]].set_index("alpha-3").to_dict()['name']
     country_names["ROW"] = "Rest of World"
     country_names['TWN'] = "Taiwan"
     country_names['GBR'] = "United Kingdom"
 
@@ -142,40 +142,40 @@
             continue
         if row.partner_code not in importers:
             continue
         DG_crude.add_weighted_edges_from([(country_names[row.location_code], country_names[row.partner_code], row.export_value)])
 
     ch_data["crude_oil"] = DG_crude
 
-    ## aircraft_network_2019
-    data_file = "data/commercial-aircraft-sitcr2-7924-yr2019/sitcr2-7924-aircraft-network-2019.gexf"
+    ## aircraft_network
+    data_file = "data/commercial_aircraft/aircraft_network.gexf"
     data_file = pkg_resources.resource_stream(__name__, data_file)
 
-    ch_data["aircraft_network_2019"] = nx.read_gexf(data_file)
+    ch_data["aircraft_network"] = nx.read_gexf(data_file)
 
-    data_file = "data/commercial-aircraft-sitcr2-7924-yr2019/sitcr2-7924-aircraft-network-2019-layout.json"
+    data_file = "data/commercial_aircraft/aircraft_network_layout.json"
     data_file = pkg_resources.resource_stream(__name__, data_file)
     f = open(data_file.name, "r")
     data = json.loads(f.read())
     pos = {}
     for nd in data['nodes']:
         pos[nd['id']] = np.array([nd['x'], nd['y']])
-    ch_data["aircraft_network_2019_pos"] = pos
+    ch_data["aircraft_network_pos"] = pos
     
     ## forbes-global2000
     data_file = 'data/csv_files/forbes-global2000.csv'
     data_file = pkg_resources.resource_stream(__name__, data_file)
     dfff = pd.read_csv(data_file)
     dfff = dfff[['Country', 'Sales', 'Profits', 'Assets', 'Market Value']]
     dfff = dfff.sort_values('Market Value', ascending=False)
     ch_data["forbes_global_2000"] = dfff
     
-    ## adjacency_matrix_2022
-    data_file='data/csv_files/adjacency_matrix_31-12-2022.csv'
-    ch_data["adjacency_matrix_2022"] = read_Z(data_file, t=0)
+    ## adjacency_matrix
+    data_file='data/csv_files/adjacency_matrix.csv'
+    ch_data["adjacency_matrix"] = read_Z(data_file, t=0)
 
     return ch_data
 
 
 def production():
     """
     Load data used in Production chapter. 
@@ -204,22 +204,22 @@
            'ar',  
            'ot',  
            'go')
     }
 
     ch_data["us_sectors_15"] =  us_sectors_15
 
-    data_file = 'data/csv_files/use_71_2021.csv'
+    data_file = 'data/csv_files/use_71.csv'
     Z_71 = read_industry_Z(
         data_file, N=71,
          columnlist=['Unnamed: 0', 'T001', 'F010', 'F02E', 'F02N', 
                              'F02R', 'F02S', 'F030', 'F040', 'F06C', 'F06E', 
                              'F06N', 'F06S', 'F07C', 'F07E', 'F07N', 'F07S', 
                              'F10C', 'F10E', 'F10N', 'F10S', 'T019'])
-    data_file = 'data/csv_files/make_71_2021.csv'
+    data_file = 'data/csv_files/make_71.csv'
     X_71 = read_industry_X(data_file, N=71)
     A_71, F_71 = build_coefficient_matrices(Z_71, X_71)
 
     us_sectors_71 = {
         "adjacency_matrix": A_71,
         "total_industry_sales": X_71,
         'codes': ('111CA',
@@ -293,20 +293,20 @@
          'GFE',
          'GSLG',
          'GSLE')
     }
 
     ch_data["us_sectors_71"] =  us_sectors_71
 
-    data_file='data/csv_files/use_114_aus_20-21.csv'
+    data_file='data/csv_files/use_114_aus.csv'
     Z_114 = read_industry_Z(data_file,
                  N=114,
                  columnlist=None)
     
-    data_file='data/csv_files/make_114_aus_20-21.csv'
+    data_file='data/csv_files/make_114_aus.csv'
     X_114 = read_industry_X(data_file, colname='total', N=114)
     A_114, F_114 = build_coefficient_matrices(Z_114, X_114)
 
     au_sectors_114 = {
         "adjacency_matrix": A_114,
         "total_industry_sales": X_114,
         'codes': ('0101',
```

### Comparing `quantecon_book_networks-0.5/quantecon_book_networks/data/README.md` & `quantecon_book_networks-0.5.1/quantecon_book_networks/data/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 # About the datasets
 
 ---
 
-### `data/commercial-aircraft-sitcr2-7924-yr2019`
+### `data/commercial_aircraft`
+
+Time:
+
+2019
 
 Description:
 
 This dataset is obtained and cleaned from [Harvard, CID Dataverse](https://dataverse.harvard.edu/dataverse/atlas).
 
+The original file path was `/commercial_aircraft-sitcr2-7924-yr2019`
+
 Not updated.
 
 ---
 
-### `data/crude_oil_sitcr2_3330_yr2021`
+### `data/crude_oil`
+
+Time:
+
+2021
 
 Description:
 
 This dataset is obtained and cleaned from `HS92` file in [CEPII - BACI](http://www.cepii.fr/CEPII/en/bdd_modele/bdd_modele_item.asp?id=37).
 
 The original `HS92` file has data for multiple goods where you can find a `Product category (HS 6-digit code)` attribute.
 
@@ -30,15 +40,19 @@
 * regions-iso3c.csv
   * to look up the ISO3C country codes
 
 ---
 
 ### `data/csv_files`
 
-#### `adjacency_matrix_31-12-2022.csv`
+#### `adjacency_matrix.csv`
+
+Time:
+
+31/12/2022
 
 Description:
 
 These data are obtained from the [BIS consolidated banking statistics](https://www.bis.org/statistics/consstats.htm), for Q4 of 2022. Our calculations used the immediate counterparty basis for financial claims of domestic and foreign banks, which calculates the sum of cross-border claims and local claims of foreign affiliates in both foreign and local currency. The foreign claim of a node to itself is set to zero.
 
 These data are originally obtained in countries and then formed into one single file.
 
@@ -57,29 +71,37 @@
 
 This dataset is scrapped in [this](https://github.com/QuantEcon/high_dim_data/blob/main/cross_section/webscrape_forbes.ipynb) file
 
 Not updated.
 
 ---
 
-#### `(make|use)_(15|71)_2021.csv`
+#### `(make|use)_(15|71).csv`
+
+Time:
+
+2021
 
 Description:
 
 Obtained and cleaned from the Supply Tables and Use Tables from [Input-Output Accounts Data](https://www.bea.gov/industry/input-output-accounts-data).
 
 Representing domestic supply and use of commodities by 15 and 71 industries in the US.
 
 The attributes we want for `Total Industry Output` in the original dataset should be `T013`, `Total product supply (basic prices)`.
 
 We need to use the code of industries instead of names in `use_71_2021.csv` as the code is written in this way.
 
 ---
 
-#### `(make|use)_114_aus_20-21.csv`
+#### `(make|use)_114_aus.csv`
+
+Time:
+
+2020-2021
 
 Description:
 
 Obtained from [ABS](https://www.abs.gov.au/statistics/economy/national-accounts/australian-national-accounts-input-output-tables/latest-release).
 
 Representing domestic supply and use of commodities by 114 industries in Australia.
```

### Comparing `quantecon_book_networks-0.5/quantecon_book_networks/data/commercial-aircraft-sitcr2-7924-yr2019/sitcr2-7924-aircraft-network-2019-layout.json` & `quantecon_book_networks-0.5.1/quantecon_book_networks/data/commercial_aircraft/aircraft_network_layout.json`

 * *Files identical despite different names*

### Comparing `quantecon_book_networks-0.5/quantecon_book_networks/data/commercial-aircraft-sitcr2-7924-yr2019/sitcr2-7924-aircraft-network-2019.gexf` & `quantecon_book_networks-0.5.1/quantecon_book_networks/data/commercial_aircraft/aircraft_network.gexf`

 * *Files identical despite different names*

### Comparing `quantecon_book_networks-0.5/quantecon_book_networks/data/crude_oil_sitcr2_3330_yr2021/data.csv` & `quantecon_book_networks-0.5.1/quantecon_book_networks/data/crude_oil/data.csv`

 * *Files identical despite different names*

### Comparing `quantecon_book_networks-0.5/quantecon_book_networks/data/crude_oil_sitcr2_3330_yr2021/regions-iso3c.csv` & `quantecon_book_networks-0.5.1/quantecon_book_networks/data/crude_oil/regions-iso3c.csv`

 * *Files identical despite different names*

### Comparing `quantecon_book_networks-0.5/quantecon_book_networks/data/crude_oil_sitcr2_3330_yr2021/sankey-diagram-crude-oil-sitc3330-yr2019.png` & `quantecon_book_networks-0.5.1/quantecon_book_networks/data/crude_oil/sankey-diagram-crude-oil-sitc3330-yr2019.png`

 * *Files identical despite different names*

### Comparing `quantecon_book_networks-0.5/quantecon_book_networks/data/csv_files/adjacency_matrix_31-12-2022.csv` & `quantecon_book_networks-0.5.1/quantecon_book_networks/data/csv_files/adjacency_matrix.csv`

 * *Files identical despite different names*

### Comparing `quantecon_book_networks-0.5/quantecon_book_networks/data/csv_files/forbes-global2000.csv` & `quantecon_book_networks-0.5.1/quantecon_book_networks/data/csv_files/forbes-global2000.csv`

 * *Files identical despite different names*

### Comparing `quantecon_book_networks-0.5/quantecon_book_networks/data/csv_files/make_114_aus_20-21.csv` & `quantecon_book_networks-0.5.1/quantecon_book_networks/data/csv_files/make_114_aus.csv`

 * *Files identical despite different names*

### Comparing `quantecon_book_networks-0.5/quantecon_book_networks/data/csv_files/make_15_2021.csv` & `quantecon_book_networks-0.5.1/quantecon_book_networks/data/csv_files/make_15.csv`

 * *Files identical despite different names*

### Comparing `quantecon_book_networks-0.5/quantecon_book_networks/data/csv_files/make_71_2021.csv` & `quantecon_book_networks-0.5.1/quantecon_book_networks/data/csv_files/make_71.csv`

 * *Files identical despite different names*

### Comparing `quantecon_book_networks-0.5/quantecon_book_networks/data/csv_files/use_114_aus_20-21.csv` & `quantecon_book_networks-0.5.1/quantecon_book_networks/data/csv_files/use_114_aus.csv`

 * *Files identical despite different names*

### Comparing `quantecon_book_networks-0.5/quantecon_book_networks/data/csv_files/use_15_2021.csv` & `quantecon_book_networks-0.5.1/quantecon_book_networks/data/csv_files/use_15.csv`

 * *Files identical despite different names*

### Comparing `quantecon_book_networks-0.5/quantecon_book_networks/data/csv_files/use_71_2021.csv` & `quantecon_book_networks-0.5.1/quantecon_book_networks/data/csv_files/use_71.csv`

 * *Files identical despite different names*

### Comparing `quantecon_book_networks-0.5/quantecon_book_networks/input_output.py` & `quantecon_book_networks-0.5.1/quantecon_book_networks/input_output.py`

 * *Files identical despite different names*

### Comparing `quantecon_book_networks-0.5/quantecon_book_networks/plotting.py` & `quantecon_book_networks-0.5.1/quantecon_book_networks/plotting.py`

 * *Files identical despite different names*

### Comparing `quantecon_book_networks-0.5/PKG-INFO` & `quantecon_book_networks-0.5.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantecon_book_networks
-Version: 0.5
+Version: 0.5.1
 Summary: Companion package for book-networks
 Author-email: QuantEcon Developers <contact@quantecon.org>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: pandas
```

