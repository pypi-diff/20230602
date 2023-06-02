# Comparing `tmp/pyilz-0.0.4.tar.gz` & `tmp/pyilz-0.0.5.tar.gz`

## Comparing `pyilz-0.0.4.tar` & `pyilz-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyilz-0.0.4/build.bat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyilz-0.0.4/pyilz/__init__.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pyilz-0.0.4/pyilz/get_device_id.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 pyilz-0.0.4/pyilz/get_game_state.py
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 pyilz-0.0.4/pyilz/get_timers.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 pyilz-0.0.4/pyilz/get_token.py
--rw-r--r--   0        0        0     5723 2020-02-02 00:00:00.000000 pyilz-0.0.4/pyilz/parse_land.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 pyilz-0.0.4/pyilz/refresh_token.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyilz-0.0.4/tests/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyilz-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 pyilz-0.0.4/tests/test_e2e.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 pyilz-0.0.4/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pyilz-0.0.4/LICENSE
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pyilz-0.0.4/README.md
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pyilz-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 pyilz-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pyilz-0.0.5/requirements.txt
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 pyilz-0.0.5/.github/workflows/main.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyilz-0.0.5/pyilz/__init__.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pyilz-0.0.5/pyilz/get_device_id.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 pyilz-0.0.5/pyilz/get_game_state.py
+-rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 pyilz-0.0.5/pyilz/get_timers.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 pyilz-0.0.5/pyilz/get_token.py
+-rw-r--r--   0        0        0     5729 2020-02-02 00:00:00.000000 pyilz-0.0.5/pyilz/parse_land.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 pyilz-0.0.5/pyilz/refresh_token.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyilz-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0   264324 2020-02-02 00:00:00.000000 pyilz-0.0.5/tests/example_game_state.json
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 pyilz-0.0.5/tests/test_e2e.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 pyilz-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pyilz-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 pyilz-0.0.5/README.md
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 pyilz-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 pyilz-0.0.5/PKG-INFO
```

### Comparing `pyilz-0.0.4/pyilz/get_device_id.py` & `pyilz-0.0.5/pyilz/get_device_id.py`

 * *Files identical despite different names*

### Comparing `pyilz-0.0.4/pyilz/get_game_state.py` & `pyilz-0.0.5/pyilz/get_game_state.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,10 +15,8 @@
     if response.status_code == 401:
         print('Token expired, refreshing...')
         API_KEY = refresh_token.refresh_token()
         response = requests.get(url, headers={'Authorization':
                                               'Bearer ' + API_KEY})
         os.environ['API_KEY'] = API_KEY
 
-    response_json = response.json()
-    plots = response_json['data']
-    return plots
+    return response.json()
```

### Comparing `pyilz-0.0.4/pyilz/get_timers.py` & `pyilz-0.0.5/pyilz/get_timers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,81 +1,90 @@
 import pandas as pd
 import pytz
 import pyilz.parse_land as parse_land
 
 
-def get_timers(gamestate):
+def get_timers_from_state(gamestate):
     _, _, ca, aa, completed = parse_land.parse_land(gamestate)
     return get_timers(ca, aa, completed)
 
 
 def get_timers(ca, aa, completed, init=False):
     timers = {}
     if ca is not None:
         for i, row in ca.iterrows():
             end_time = row['currentActivity.EndTime'].replace(
                 tzinfo=pytz.utc)
             cur_time = pd.Timestamp.now(tz='utc')
             diff_minutes = (end_time - cur_time).total_seconds() / 60
 
-            # Calculate percentage based on currentActivity.StartTime and currentActivity.EndTime
+            # Calculate percentage based on currentActivity.StartTime 
+            # and currentActivity.EndTime
             start_time = row['currentActivity.StartTime'].replace(
                 tzinfo=pytz.utc)
             total_time = (end_time - start_time).total_seconds() / 60
             elapsed_time = (cur_time - start_time).total_seconds() / 60
             percentage = elapsed_time / total_time * 100
 
             notified = False
             if init and diff_minutes <= 0:
                 notified = True
-            timers[f'{row["uid"]}-current'] = {'uid': row['uid'], 'name': row['buildingTypeString'],
-                                               'type': row['currentActivity.Type'], 'minutes': diff_minutes, 'notified': notified, 'percentage': percentage}
+            timers[f'{row["uid"]}-current'] = {'uid': row['uid'], 
+                                               'name': row['buildingTypeString'],
+                                               'type': row['currentActivity.Type'], 
+                                               'minutes': diff_minutes, 
+                                               'notified': notified, 
+                                               'percentage': percentage}
 
     if aa is not None:
         for i, row in aa.iterrows():
             end_time = row['autoActivity.EndTime'].replace(tzinfo=pytz.utc)
             cur_time = pd.Timestamp.now(tz='utc')
             diff_minutes = (end_time - cur_time).total_seconds() / 60
 
-            # Calculate percentage based on currentActivity.StartTime and currentActivity.EndTime
+            # Calculate percentage based on currentActivity.StartTime 
+            # and currentActivity.EndTime
             start_time = row['autoActivity.StartTime'].replace(
                 tzinfo=pytz.utc)
             total_time = (end_time - start_time).total_seconds() / 60
             elapsed_time = (cur_time - start_time).total_seconds() / 60
             percentage = elapsed_time / total_time * 100
 
-            # if row['buildingTypeString'] in ['SEQUESTRIAN_PLANT_4', 'PHOTODISINTEGRATION_PLANT_4', 'CONDENSER_PLANT_4']:
-            #    percentage = (int(row['autoActivity.GeneratedResources']) / 7500) * 100
-
             notified = False
             if init and diff_minutes <= 0:
                 notified = True
-            timers[f'{row["uid"]}-auto'] = {'uid': row['uid'], 'name': row['buildingTypeString'],
-                                            'type': row['autoActivity.Type'], 'minutes': diff_minutes, 'notified': notified, 'percentage': percentage}
+            timers[f'{row["uid"]}-auto'] = {'uid': row['uid'], 
+                                            'name': row['buildingTypeString'],
+                                            'type': row['autoActivity.Type'], 
+                                            'minutes': diff_minutes, 
+                                            'notified': notified, 
+                                            'percentage': percentage}
 
     if completed is not None:
         for i, row in completed.iterrows():
             end_time = row['completedActivity.EndTime'].replace(
                 tzinfo=pytz.utc)
             cur_time = pd.Timestamp.now(tz='utc')
             diff_minutes = (end_time - cur_time).total_seconds() / 60
 
-            # Calculate percentage based on currentActivity.StartTime and currentActivity.EndTime
+            # Calculate percentage based on currentActivity.StartTime 
+            # and currentActivity.EndTime
             start_time = row['completedActivity.StartTime'].replace(
                 tzinfo=pytz.utc)
             total_time = (end_time - start_time).total_seconds() / 60
             elapsed_time = (cur_time - start_time).total_seconds() / 60
             percentage = elapsed_time / total_time * 100
 
-            # if row['buildingTypeString'] in ['SEQUESTRIAN_PLANT_4', 'PHOTODISINTEGRATION_PLANT_4', 'CONDENSER_PLANT_4']:
-            #    percentage = (int(row['completedActivity.GeneratedResources']) / 7500) * 100
-
             notified = False
             if init and diff_minutes <= 0:
                 notified = True
-            timers[f'{row["uid"]}-current'] = {'uid': row['uid'], 'name': row['buildingTypeString'],
-                                               'type': row['completedActivity.Type'], 'minutes': diff_minutes, 'notified': notified, 'percentage': percentage}
+            timers[f'{row["uid"]}-current'] = {'uid': row['uid'], 
+                                               'name': row['buildingTypeString'],
+                                               'type': row['completedActivity.Type'], 
+                                               'minutes': diff_minutes, 
+                                               'notified': notified, 
+                                               'percentage': percentage}
 
     # sort by minutes
     timers = {k: v for k, v in sorted(
         timers.items(), key=lambda item: item[1]['minutes'])}
     return timers
```

### Comparing `pyilz-0.0.4/pyilz/parse_land.py` & `pyilz-0.0.5/pyilz/parse_land.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,17 +63,17 @@
         aa = aa.drop(columns=['autoActivity'])
         # convert autoActivity.StartTime and autoActivity.EndTime to datetime
         aa['autoActivity.StartTime'] = pd.to_datetime(
             aa['autoActivity.StartTime'])
         aa['autoActivity.EndTime'] = pd.to_datetime(aa['autoActivity.EndTime'])
         # remove _{number} from autoActivity.Type and put into column autoActivity.Level
         aa['autoActivity.Level'] = buildings['buildingTypeString'].str.extract(
-            '(\d+)$', expand=False).fillna(0).astype(int)
+            r'(\d+)$', expand=False).fillna(0).astype(int)
         aa['autoActivity.Type'] = buildings['buildingTypeString'].str.extract(
-            '(.+?)\d+$', expand=False).str.rstrip('_') + '_AUTOMATIC'
+            r'(.+?)\d+$', expand=False).str.rstrip('_') + '_AUTOMATIC'
         # aa['autoActivity.GeneratedResources'] = buildings['fractionalGeneratedResources']
     else:
         aa = None
 
     if 'completedActivity' in buildings.columns:
         # get rows where completedActivity is not null
         completed = buildings[buildings['completedActivity'].notnull()]
@@ -87,17 +87,17 @@
         # convert completedActivity.StartTime and completedActivity.EndTime to datetime
         completed['completedActivity.StartTime'] = pd.to_datetime(
             completed['completedActivity.StartTime'])
         completed['completedActivity.EndTime'] = pd.to_datetime(
             completed['completedActivity.EndTime'])
         # remove _{number} from completedActivity.Type and put into column completedActivity.Level
         completed['completedActivity.Level'] = buildings['buildingTypeString'].str.extract(
-            '(\d+)$', expand=False).fillna(0).astype(int)
+            r'(\d+)$', expand=False).fillna(0).astype(int)
         completed['completedActivity.Type'] = buildings['buildingTypeString'].str.extract(
-            '(.+?)\d+$', expand=False).str.rstrip('_') + '_AUTOMATIC'
+            r'(.+?)\d+$', expand=False).str.rstrip('_') + '_AUTOMATIC'
         # completed['completedActivity.GeneratedResources'] = buildings['fractionalGeneratedResources']
     else:
         completed = None
 
     # drop columns uid, state, startTime
     buildings = buildings.drop(columns=[
         'uid', 'state', 'startTime',
@@ -105,19 +105,19 @@
 
     # convert generatedResources to int
     if 'generatedResources' in buildings.columns:
         buildings['generatedResources'] = buildings['generatedResources'].astype(
             int)
 
     # create column that is the last number of the buildingTypeString
-    buildings['level'] = buildings['buildingTypeString'].str.extract('(\d+)$',
+    buildings['level'] = buildings['buildingTypeString'].str.extract(r'(\d+)$',
                                                                      expand=False)
 
     buildings['name'] = buildings['buildingTypeString'].str.extract(
-        '(.+?)\d+$', expand=False).str.rstrip('_')
+        r'(.+?)\d+$', expand=False).str.rstrip('_')
 
     # if name is nan set name to buildingTypeString
     buildings['name'] = buildings['name'].fillna(
         buildings['buildingTypeString'])
     buildings['level'] = buildings['level'].fillna(0)
 
     buildings = buildings.drop(columns=['buildingTypeString'])
```

### Comparing `pyilz-0.0.4/pyilz/refresh_token.py` & `pyilz-0.0.5/pyilz/refresh_token.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,13 +23,13 @@
     }, timeout=5)
 
     if response.status_code != 200:
         raise Exception(
             f'Failed to refresh token. {response.status_code} {response.text}')
 
     authentication_result = response.json()['AuthenticationResult']
-    access_token = authentication_result['AccessToken']
-    expires_in = authentication_result['ExpiresIn']
+    #access_token = authentication_result['AccessToken']
+    #expires_in = authentication_result['ExpiresIn']
     id_token = authentication_result['IdToken']
-    token_type = authentication_result['TokenType']
+    #token_type = authentication_result['TokenType']
 
     return id_token
```

### Comparing `pyilz-0.0.4/.gitignore` & `pyilz-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pyilz-0.0.4/LICENSE` & `pyilz-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyilz-0.0.4/pyproject.toml` & `pyilz-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyilz"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Nick Jordan", email="nickjordan289@gmail.com" },
 ]
-description = "pyilz"
+description = "A Python Library for Illuvium Zero Land Management"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

