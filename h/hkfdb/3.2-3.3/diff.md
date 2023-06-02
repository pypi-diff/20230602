# Comparing `tmp/hkfdb-3.2.tar.gz` & `tmp/hkfdb-3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hkfdb-3.2.tar", last modified: Fri May 12 14:38:22 2023, max compression
+gzip compressed data, was "hkfdb-3.3.tar", last modified: Fri Jun  2 12:32:06 2023, max compression
```

## Comparing `hkfdb-3.2.tar` & `hkfdb-3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 14:38:22.924455 hkfdb-3.2/
--rw-rw-rw-   0        0        0    35149 2021-07-30 00:33:11.000000 hkfdb-3.2/LICENSE
--rw-rw-rw-   0        0        0     1651 2023-05-12 14:38:22.924455 hkfdb-3.2/PKG-INFO
--rw-rw-rw-   0        0        0     1243 2023-03-30 03:29:25.000000 hkfdb-3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 14:38:22.917452 hkfdb-3.2/hkfdb/
--rw-rw-rw-   0        0        0    93289 2023-05-12 14:37:56.000000 hkfdb-3.2/hkfdb/Database.py
--rw-rw-rw-   0        0        0       23 2021-09-12 13:30:45.000000 hkfdb-3.2/hkfdb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 14:38:22.923453 hkfdb-3.2/hkfdb.egg-info/
--rw-rw-rw-   0        0        0     1651 2023-05-12 14:38:22.000000 hkfdb-3.2/hkfdb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-05-12 14:38:22.000000 hkfdb-3.2/hkfdb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 14:38:22.000000 hkfdb-3.2/hkfdb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-12 14:38:22.000000 hkfdb-3.2/hkfdb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-12 14:38:22.000000 hkfdb-3.2/hkfdb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-12 14:38:22.924455 hkfdb-3.2/setup.cfg
--rw-rw-rw-   0        0        0      761 2023-05-12 14:38:09.000000 hkfdb-3.2/setup.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-02 12:32:06.495645 hkfdb-3.3/
+-rw-rw-rw-   0 cmw        (501) staff       (20)    35149 2021-07-30 00:33:11.000000 hkfdb-3.3/LICENSE
+-rw-r--r--   0 cmw        (501) staff       (20)     1618 2023-06-02 12:32:06.495274 hkfdb-3.3/PKG-INFO
+-rw-rw-rw-   0 cmw        (501) staff       (20)     1243 2023-03-30 03:29:25.000000 hkfdb-3.3/README.md
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-02 12:32:06.493827 hkfdb-3.3/hkfdb/
+-rw-rw-rw-   0 cmw        (501) staff       (20)   106387 2023-06-02 05:18:47.000000 hkfdb-3.3/hkfdb/Database.py
+-rw-rw-rw-   0 cmw        (501) staff       (20)       23 2021-09-12 13:30:45.000000 hkfdb-3.3/hkfdb/__init__.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-02 12:32:06.494991 hkfdb-3.3/hkfdb.egg-info/
+-rw-rw-rw-   0 cmw        (501) staff       (20)     1618 2023-06-02 12:32:06.000000 hkfdb-3.3/hkfdb.egg-info/PKG-INFO
+-rw-rw-rw-   0 cmw        (501) staff       (20)      206 2023-06-02 12:32:06.000000 hkfdb-3.3/hkfdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)        1 2023-06-02 12:32:06.000000 hkfdb-3.3/hkfdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)       44 2023-06-02 12:32:06.000000 hkfdb-3.3/hkfdb.egg-info/requires.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)        6 2023-06-02 12:32:06.000000 hkfdb-3.3/hkfdb.egg-info/top_level.txt
+-rw-r--r--   0 cmw        (501) staff       (20)       38 2023-06-02 12:32:06.495722 hkfdb-3.3/setup.cfg
+-rw-rw-rw-   0 cmw        (501) staff       (20)      761 2023-06-02 12:31:47.000000 hkfdb-3.3/setup.py
```

### Comparing `hkfdb-3.2/LICENSE` & `hkfdb-3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hkfdb-3.2/PKG-INFO` & `hkfdb-3.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,74 @@
-Metadata-Version: 2.1
-Name: hkfdb
-Version: 3.2
-Summary: Hong Kong Finance Database.
-Home-page: https://www.hkfdb.net
-Author: Hong Kong Finance Database Team
-Author-email: info@hkfdb.net
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Hong Kong Finance Database
-
-To install the latest version:
-```
-pip install hkfdb
-```
-
-Before you start, please make sure you have done the following:
-* **subscribe** the data from our website
-* get the personal authToken 
-* create an client object from class Database
-* have fun!
-
-create client object with authToken and class Database:
-```
-import hkfdb
-
-authToken = 'personal_authToken'
-client = hkfdb.Database(authToken)
-```
-
-**Major Functions**
-
-Price Data:
-* get_hk_stock_ohlc() 
-* get_us_stock_ohlc()
-* get_hk_fut_ohlc()
-* get_hk_deri_daily_market_report()
-
-CCASS Data:
-* get_ccass_all_id()
-* get_ccass_by_code()
-* get_ccass_holding_rank()
-* get_ccass_by_id()
-* get_ccass_by_id_change()
-
-Index list:
-* get_spx_index_const()
-* get_hk_index_const()
-* get_hk_stock_plate_const()
-* get_all_hk_index_name()
-* get_all_hk_stock_plate_name()
-
-Earning Calendar:
-* get_us_earning_calendar_by_date()
-* get_us_earning_calendar_by_code()
-* get_hk_earning_calendar_by_code()
-* get_hk_earning_calendar_by_date()
-
-Other:
-* get_hk_market_cap_hist()
-* get_hk_ipo_hist()
-* get_north_water()
-* get_market_highlight()
-* get_hk_buyback_by_date()
-* get_hk_buyback_by_code()
-* get_basic_hk_stock_info()
+Metadata-Version: 2.1
+Name: hkfdb
+Version: 3.3
+Summary: Hong Kong Finance Database.
+Home-page: https://www.hkfdb.net
+Author: Hong Kong Finance Database Team
+Author-email: info@hkfdb.net
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Hong Kong Finance Database
+
+To install the latest version:
+```
+pip install hkfdb
+```
+
+Before you start, please make sure you have done the following:
+* **subscribe** the data from our website
+* get the personal authToken 
+* create an client object from class Database
+* have fun!
+
+create client object with authToken and class Database:
+```
+import hkfdb
+
+authToken = 'personal_authToken'
+client = hkfdb.Database(authToken)
+```
+
+**Major Functions**
+
+Price Data:
+* get_hk_stock_ohlc() 
+* get_us_stock_ohlc()
+* get_hk_fut_ohlc()
+* get_hk_deri_daily_market_report()
+
+CCASS Data:
+* get_ccass_all_id()
+* get_ccass_by_code()
+* get_ccass_holding_rank()
+* get_ccass_by_id()
+* get_ccass_by_id_change()
+
+Index list:
+* get_spx_index_const()
+* get_hk_index_const()
+* get_hk_stock_plate_const()
+* get_all_hk_index_name()
+* get_all_hk_stock_plate_name()
+
+Earning Calendar:
+* get_us_earning_calendar_by_date()
+* get_us_earning_calendar_by_code()
+* get_hk_earning_calendar_by_code()
+* get_hk_earning_calendar_by_date()
+
+Other:
+* get_hk_market_cap_hist()
+* get_hk_ipo_hist()
+* get_north_water()
+* get_market_highlight()
+* get_hk_buyback_by_date()
+* get_hk_buyback_by_code()
+* get_basic_hk_stock_info()
+
+
```

### Comparing `hkfdb-3.2/README.md` & `hkfdb-3.3/README.md`

 * *Files identical despite different names*

### Comparing `hkfdb-3.2/hkfdb/Database.py` & `hkfdb-3.3/hkfdb/Database.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import time
 import requests
 import pandas as pd
 import json
 import ast
-import pymongo
 import datetime
+import calendar
 from dateutil.relativedelta import relativedelta, FR
 from bs4 import BeautifulSoup
 
+
 class Database:
 
     def __init__(self,authToken):
         self.authToken = authToken
 
     def get_hk_stock_ohlc(self, code, start_date, end_date, freq, price_adj=False, vol_adj=False):
 
@@ -69,15 +70,16 @@
                     df['datetime'] = df['date']
                     df['datetime'] = pd.to_datetime(df['datetime'], format='%Y%m%d')
                     cols = ['datetime', 'date', 'open', 'high', 'low', 'close', 'volume']
 
                 elif freq == '1DW':
                     df['datetime'] = df['date']
                     df['datetime'] = pd.to_datetime(df['datetime'], format='%Y%m%d')
-                    cols = ['datetime','date','open','high','low','close','volume','susp','auc_close','adj_close','gross_volume','turnover','VWAP']
+                    cols = ['datetime','date','open','high','low','close','volume','susp','auc_close',
+                            'adj_close','gross_volume','turnover','VWAP']
                     df['susp'] = df['susp'].astype(bool)
 
                 df = df[cols]
                 df = df.set_index(keys='datetime')
                 df = df.sort_index()
 
                 if price_adj == True:
@@ -137,15 +139,16 @@
                             df[col] = df[col].map(lambda x: round(x, 0))
                             df[col] = df[col].astype(int)
 
                     if 'T' in freq:
                         df = df[['date', 'time', 'open', 'high', 'low', 'close', 'volume']]
                     else:
                         if freq == '1DW':
-                            df = df[['date','open','high','low','close','volume','susp','auc_close','gross_volume','turnover','VWAP']]
+                            df = df[['date','open','high','low','close','volume','susp',
+                                     'auc_close','gross_volume','turnover','VWAP']]
                         elif freq == '1D':
                             df = df[['date','open','high','low','close','volume']]
 
                 df['date'] = df['date'].astype(int)
                 if 'T' in freq:
                     df['time'] = df['time'].astype(int)
                 else:
@@ -199,14 +202,296 @@
         else:
             err_msg = 'Error in: '
             for error in check_bool_dict:
                 if check_bool_dict[error] == False:
                     err_msg += error + ','
             print(err_msg)
 
+
+    ## Futures
+    expiry_dict = {}
+    rolling_day = 0
+    rolling_time = 0
+
+    def apply_rolling_day(self, row):
+        rolling_day = self.rolling_day
+        rolling_time = self.rolling_time
+
+        if row.current_month_expiry_date_diff < rolling_day:  # less than rolling_day, keep next month
+            if not row.current_month:  # next month, keep it
+                return True
+            else:
+                return False
+
+        elif row.current_month_expiry_date_diff > rolling_day:  # more than rolling_dat, keep current
+            if row.current_month:  # current month, keep it
+                return True
+            else:
+                return False
+
+        else:  # current_month_expiry_date_diff == rolling_day, need to consider time
+            if row.time >= rolling_time:  # need to keep next month
+                if not row.current_month:  # next month, keep it
+                    return True
+                else:
+                    return False
+
+            else:  # need to keep current month
+                if row.current_month:  # next month, keep it
+                    return True
+                else:
+                    return False
+
+    def apply_rolling_1D(self, row):
+        rolling_day = self.rolling_day
+
+        if row.current_month_expiry_date_diff <= rolling_day:  # less than rolling_day, keep next month
+            if not row.current_month:  # next month, keep it
+                return True
+            else:
+                return False
+
+        elif row.current_month_expiry_date_diff > rolling_day:  # more than rolling_dat, keep current
+            if row.current_month:  # current month, keep it
+                return True
+            else:
+                return False
+
+
+    def apply_RTH_ATH(self, row):
+        if (row.time > 90000 and row.time < 163000):
+            return True
+        else:
+            return False
+
+
+    def apply_roll_diff(self, row):
+        rolling_day = self.rolling_day
+        rolling_time = self.rolling_time
+        roll_diff = self.roll_diff
+        if row.current_month_expiry_date_diff == rolling_day and row.time == rolling_time:
+            return roll_diff
+        else:
+            return 0
+
+    def get_hk_futures_ohlc(self, index, start_date, end_date, freq, rolling_day, rolling_time=0, rth_only=False):
+
+        check_bool_dict = self.check_hk_fut_ohlc_args(index, freq, start_date, end_date, rolling_day, rolling_time)
+
+        self.rolling_day = rolling_day
+        self.rolling_time = rolling_time
+
+
+        if False not in list(check_bool_dict.values()):
+
+            link_url = 'http://www.hkfdb.net/data_api?'
+            token = str(self.authToken)
+            start_date_str = str(start_date)
+            # end_date_str = str(end_date)[:4], str(end_date)[4:6]
+            _, last_day = calendar.monthrange( int(str(end_date)[:4]), int(str(end_date)[4:6]))
+            end_date_str = f'{str(end_date)[:4]}{str(end_date)[4:6]}{last_day}'
+            link_str = f'{link_url}token={token}&database=hk_futures_ohlc&index={index}&freq={freq}&start_date={start_date_str}&end_date={end_date_str}'
+
+            response = requests.get(link_str)
+            response_ok = response_check(response)
+
+
+            if response_ok == True:
+
+                result_list = json.loads(json.loads(response.content).replace("'", "\"").replace("True", "true").replace("False", "false") )
+
+                columns = ['datetime', 'open', 'high', 'low', 'close', 'volume',
+                           'trade_date_mask', 'expiry_date', 'current_month',
+                           'current_month_expiry_date', 'current_month_expiry_date_diff']
+
+
+                if freq == '1D':
+                    dfs = []
+                    for item in list(reversed(result_list)):
+                        df_single = pd.DataFrame(item['content'], columns=columns)
+                        df_single['datetime'] = pd.to_datetime(df_single['datetime'])
+                        df_single['date'] = pd.to_datetime(df_single['datetime']).dt.strftime('%Y%m%d').astype(int)
+                        df_single['time'] = pd.to_datetime(df_single['datetime']).dt.strftime('%H%M%S').astype(int)
+                        df_single['RTH'] = df_single.apply(self.apply_RTH_ATH, axis=1)
+
+                        if rth_only:
+                            df_single = df_single[df_single['RTH'] == True]
+
+                        df_all = []
+
+                        for current_month in [True, False]:
+                            df_current = df_single[df_single['current_month'] == current_month].sort_values(
+                                by=['datetime']).reset_index(drop=True)
+                            df = df_current.head(1).copy()
+
+                            df['open'] = df_current.at[0, 'open']
+                            df['high'] = df_current['high'].max()
+                            df['low'] = df_current['low'].min()
+                            df['close'] = df_current.at[1, 'close']
+                            df['volume'] = df_current['volume'].sum()
+
+                            df_all.append(df.copy())
+
+                        dfs.append(pd.concat(df_all))
+
+                    df = pd.concat(dfs)
+                    df['datetime'] = pd.to_datetime(df['datetime'])
+
+                    ## Find the valid expiry date to processed , ie within date range
+                    expiry_dates = list(df['expiry_date'].unique())
+                    expiry_dates.sort()
+
+                    # # Calculate roll diff
+                    roll_diff_dict = {}
+
+                    for expiry_date in expiry_dates:
+                        try:
+                            exact_rolling_date = df[(df['expiry_date'] == expiry_date) &
+                                                    (df['current_month_expiry_date_diff'] == rolling_day) &
+                                                    (df['current_month'] == True)].reset_index(drop=True).sort_values(
+                                by=['datetime']).at[0, 'date']
+
+                            df_roll = df[(df['date'] == exact_rolling_date)].copy()
+                            df_roll = df_roll.sort_values(by=['datetime']).reset_index(drop=True)
+
+                            roll_diff_dict[expiry_date] = {}
+
+                            roll_diff = df_roll.at[0, 'close'] - df_roll.at[1, 'close']
+                            roll_diff_dict[expiry_date]['rolling_day'] = exact_rolling_date
+                            roll_diff_dict[expiry_date]['roll_diff'] = roll_diff
+                        except:
+                            pass
+
+                    df = df.sort_values(by=['datetime']).reset_index(drop=True)
+
+                    df['roll_diff'] = 0
+
+                    for expiry_date in roll_diff_dict.keys():
+                        d = roll_diff_dict[expiry_date]['rolling_day']
+                        diff = roll_diff_dict[expiry_date]['roll_diff']
+
+                        condition = (df['date'] == d) & (df['current_month'] == False)
+                        indices = df[condition].index[0]
+                        df.at[indices, 'roll_diff'] = diff
+
+                    df['keep'] = df.apply(self.apply_rolling_1D, axis=1)
+                    df = df[df['keep'] == True]
+                    selected_columns = ['datetime', 'date', 'time', 'open', 'high', 'low', 'close', 'volume',
+                                        'expiry_date', 'roll_diff']
+                    df = df[selected_columns]
+                    df = df.sort_values(by=['datetime']).set_index('datetime', drop=True)
+
+                    df.index = df.index.strftime('%Y-%m-%d')
+                    df['time'] = 0
+                    df['open'] = df['open'].astype(int)
+                    df['high'] = df['high'].astype(int)
+                    df['low'] = df['low'].astype(int)
+                    df['close'] = df['close'].astype(int)
+
+                    return df
+
+
+                else:  # 1T, 5T, 15T
+                    df_list = []
+                    for item in result_list:
+                        date_int = item['_id']
+                        df = pd.DataFrame(item['content'], columns=columns)
+                        if len(df) > 0:
+                            df['date'] = str(date_int)
+                            df_list.append(df)
+                    df = pd.concat(df_list, )
+
+                    df['datetime'] = pd.to_datetime(df['datetime'])
+
+                    df = df.copy()
+                    df['date'] = pd.to_datetime(df['datetime']).dt.strftime('%Y%m%d').astype(int)
+                    df['time'] = pd.to_datetime(df['datetime']).dt.strftime('%H%M%S').astype(int)
+                    condition = df['time'] == 120000  # remove 120000 time
+                    df = df[~condition]
+                    df['RTH'] = df.apply(self.apply_RTH_ATH, axis=1)  # Determine RTH and ATH
+
+                    ## Find the valid expiry date to processed , ie within date range
+                    expiry_dates = list(df['expiry_date'].unique())
+                    expiry_dates.sort()
+                    # print(expiry_dates)
+
+                    # Calculate roll diff
+                    roll_diff_dict = {}
+
+                    for expiry_date in expiry_dates:
+                        try:
+                            exact_rolling_date = df[(df['expiry_date'] == expiry_date) &
+                                                    (df['current_month_expiry_date_diff'] == rolling_day) &
+                                                    (df['current_month'] == True)].sort_values(by=['datetime']).reset_index(drop=True).reset_index(drop=True).at[0, 'date']
+
+                            df_roll = df[(df['date'] == exact_rolling_date)].copy()
+                            df_roll = df_roll[df_roll['time'] == rolling_time].sort_values(by=['expiry_date']).reset_index(drop=True)
+
+                            roll_diff_dict[expiry_date] = {}
+
+                            if len(df_roll) == 2:
+                                roll_diff = df_roll.at[0, 'close'] - df_roll.at[1, 'close']
+                                roll_diff_dict[expiry_date]['rolling_day'] = exact_rolling_date
+                                roll_diff_dict[expiry_date]['roll_diff'] = roll_diff
+                                roll_diff_dict[expiry_date]['rolling_time'] = rolling_time
+
+                            else:
+                                # Cannot find rolling time, assume roll at RTH last trade
+                                df_roll = df[(df['date'] == exact_rolling_date) & (df['RTH'] == True)].copy()
+                                df_roll = df_roll.sort_values(by=['time', 'expiry_date']).reset_index(drop=True)
+                                df_roll = df_roll.tail(2).sort_values(by=['expiry_date']).reset_index(drop=True)
+                                roll_diff = df_roll.at[0, 'close'] - df_roll.at[1, 'close']
+                                roll_diff_dict[expiry_date]['rolling_day'] = exact_rolling_date
+                                roll_diff_dict[expiry_date]['roll_diff'] = roll_diff
+                                roll_diff_dict[expiry_date]['rolling_time'] = df_roll.at[0, 'time']
+                        except:
+                            pass
+
+                    df = df.reset_index(drop=True)
+                    df['roll_diff'] = 0
+
+                    for expiry_date in roll_diff_dict.keys():
+                        d = roll_diff_dict[expiry_date]['rolling_day']
+                        t = roll_diff_dict[expiry_date]['rolling_time']
+                        diff = roll_diff_dict[expiry_date]['roll_diff']
+
+                        condition = (df['date'] == d) & (df['time'] == t) & (df['current_month'] == False)
+                        indices = df[condition].index[0]
+                        df.at[indices, 'roll_diff'] = diff
+
+                    ## Exclude ATH if needed
+                    if rth_only:
+                        df = df[df['RTH'] == True]
+
+                    ## Calculate rolling day and determine keep or not
+                    df['keep'] = df.apply(self.apply_rolling_day, axis=1)
+                    df = df[df['keep'] == True]
+                    selected_columns = ['datetime', 'date', 'time', 'open', 'high', 'low', 'close', 'volume',
+                                        'expiry_date', 'RTH', 'roll_diff']
+                    df = df[selected_columns]
+                    df = df.sort_values(by=['datetime']).set_index('datetime', drop=True)
+
+                    df['time'] = df['time'].astype(str).str.zfill(6)
+                    df['open'] = df['open'].astype(int)
+                    df['high'] = df['high'].astype(int)
+                    df['low'] = df['low'].astype(int)
+                    df['close'] = df['close'].astype(int)
+
+
+                    return df
+
+
+        else:
+            err_msg = 'Error in: '
+            for error in check_bool_dict:
+                if check_bool_dict[error] == False:
+                    err_msg += error + ','
+            print(err_msg)
+
+
     def get_hk_fut_ohlc(self, index, start_date, end_date, freq, rolling_day, rolling_time=0, rth_only=False):
 
         check_bool_dict = self.check_hk_fut_ohlc_args(index, freq, start_date, end_date, rolling_day, rolling_time)
 
         if False not in list(check_bool_dict.values()):
 
             if freq == '1D':
@@ -265,15 +550,16 @@
             index_str = 'index=' + index
             freq_str = 'freq=' + freq
             start_date_str = 'start_date=' + str(start_date)
             end_date_str = 'end_date=' + str(end_date)
             rolling_day_str = 'rolling_day=' + str(rolling_day)
             rolling_time_str = 'rolling_time=' + str(rolling_time)
             year_month_involved_list_str = 'year_month_involved_list=' + year_month_involved_list_str
-            link_str = link_url + index_str + '&' + freq_str + '&' + rolling_day_str + '&' + rolling_time_str + '&' + year_month_involved_list_str + '&' \
+            link_str = link_url + index_str + '&' + freq_str + '&' + rolling_day_str + '&' + rolling_time_str + \
+                       '&' + year_month_involved_list_str + '&' \
                        + token_str + '&' + database_str + '&' \
                        + start_date_str + '&' + end_date_str
 
             response = requests.get(link_str)
             response_ok = response_check(response)
             if response_ok == True:
 
@@ -1270,15 +1556,16 @@
                 df[col] = df[col].str.replace(',', '', regex=False)
                 df[col] = df[col].astype(float)
 
             for col in int_col_list:
                 df[col] = df[col].astype('int64')
             df['lot_size'] = df['lot_size'].astype(int)
 
-            df = df[['code','stock_name','price','PE','EPS','dividend','volume','turnover','share_issued','lot_size','market_capital','ipo_date','year_end_date', 'stop_trading','category']]
+            df = df[['code','stock_name','price','PE','EPS','dividend','volume','turnover','share_issued',
+                     'lot_size','market_capital','ipo_date','year_end_date', 'stop_trading','category']]
             return df
 
     def get_hk_ipo_hist(self):
 
         link_url = 'http://www.hkfdb.net/data_api?'
         token_str = 'token=' + str(self.authToken)
         database_str = 'database=' + 'hk_ipo_hist'
@@ -2182,15 +2469,16 @@
     dict1 = {'expiry_date': expiry_date_list, 'public_holiday': holiday_list, 'half_day_mkt': half_day_mkt_list}
     return dict1
 
 
 def get_current_us_holiday(format='int', str_format='%Y%m%d'):
     url = 'https://www.nasdaqtrader.com/Trader.aspx?id=Calendar'
     headers = {
-        'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/86.0.4240.193 Safari/537.36'}
+        'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) \
+        Chrome/86.0.4240.193 Safari/537.36'}
     r = requests.get(url, headers=headers)
     r.raise_for_status()
     r.encoding = r.apparent_encoding
     text = r.text
 
     soup = BeautifulSoup(text, 'lxml')
```

### Comparing `hkfdb-3.2/hkfdb.egg-info/PKG-INFO` & `hkfdb-3.3/hkfdb.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,74 @@
-Metadata-Version: 2.1
-Name: hkfdb
-Version: 3.2
-Summary: Hong Kong Finance Database.
-Home-page: https://www.hkfdb.net
-Author: Hong Kong Finance Database Team
-Author-email: info@hkfdb.net
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Hong Kong Finance Database
-
-To install the latest version:
-```
-pip install hkfdb
-```
-
-Before you start, please make sure you have done the following:
-* **subscribe** the data from our website
-* get the personal authToken 
-* create an client object from class Database
-* have fun!
-
-create client object with authToken and class Database:
-```
-import hkfdb
-
-authToken = 'personal_authToken'
-client = hkfdb.Database(authToken)
-```
-
-**Major Functions**
-
-Price Data:
-* get_hk_stock_ohlc() 
-* get_us_stock_ohlc()
-* get_hk_fut_ohlc()
-* get_hk_deri_daily_market_report()
-
-CCASS Data:
-* get_ccass_all_id()
-* get_ccass_by_code()
-* get_ccass_holding_rank()
-* get_ccass_by_id()
-* get_ccass_by_id_change()
-
-Index list:
-* get_spx_index_const()
-* get_hk_index_const()
-* get_hk_stock_plate_const()
-* get_all_hk_index_name()
-* get_all_hk_stock_plate_name()
-
-Earning Calendar:
-* get_us_earning_calendar_by_date()
-* get_us_earning_calendar_by_code()
-* get_hk_earning_calendar_by_code()
-* get_hk_earning_calendar_by_date()
-
-Other:
-* get_hk_market_cap_hist()
-* get_hk_ipo_hist()
-* get_north_water()
-* get_market_highlight()
-* get_hk_buyback_by_date()
-* get_hk_buyback_by_code()
-* get_basic_hk_stock_info()
+Metadata-Version: 2.1
+Name: hkfdb
+Version: 3.3
+Summary: Hong Kong Finance Database.
+Home-page: https://www.hkfdb.net
+Author: Hong Kong Finance Database Team
+Author-email: info@hkfdb.net
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Hong Kong Finance Database
+
+To install the latest version:
+```
+pip install hkfdb
+```
+
+Before you start, please make sure you have done the following:
+* **subscribe** the data from our website
+* get the personal authToken 
+* create an client object from class Database
+* have fun!
+
+create client object with authToken and class Database:
+```
+import hkfdb
+
+authToken = 'personal_authToken'
+client = hkfdb.Database(authToken)
+```
+
+**Major Functions**
+
+Price Data:
+* get_hk_stock_ohlc() 
+* get_us_stock_ohlc()
+* get_hk_fut_ohlc()
+* get_hk_deri_daily_market_report()
+
+CCASS Data:
+* get_ccass_all_id()
+* get_ccass_by_code()
+* get_ccass_holding_rank()
+* get_ccass_by_id()
+* get_ccass_by_id_change()
+
+Index list:
+* get_spx_index_const()
+* get_hk_index_const()
+* get_hk_stock_plate_const()
+* get_all_hk_index_name()
+* get_all_hk_stock_plate_name()
+
+Earning Calendar:
+* get_us_earning_calendar_by_date()
+* get_us_earning_calendar_by_code()
+* get_hk_earning_calendar_by_code()
+* get_hk_earning_calendar_by_date()
+
+Other:
+* get_hk_market_cap_hist()
+* get_hk_ipo_hist()
+* get_north_water()
+* get_market_highlight()
+* get_hk_buyback_by_date()
+* get_hk_buyback_by_code()
+* get_basic_hk_stock_info()
+
+
```

### Comparing `hkfdb-3.2/setup.py` & `hkfdb-3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hkfdb",
-    version="3.2",
+    version="3.3",
     author="Hong Kong Finance Database Team",
     author_email="info@hkfdb.net",
     description="Hong Kong Finance Database.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.hkfdb.net",
     packages=setuptools.find_packages(),
```

