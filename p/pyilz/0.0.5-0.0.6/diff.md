# Comparing `tmp/pyilz-0.0.5.tar.gz` & `tmp/pyilz-0.0.6.tar.gz`

## Comparing `pyilz-0.0.5.tar` & `pyilz-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pyilz-0.0.5/requirements.txt
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 pyilz-0.0.5/.github/workflows/main.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyilz-0.0.5/pyilz/__init__.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pyilz-0.0.5/pyilz/get_device_id.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 pyilz-0.0.5/pyilz/get_game_state.py
--rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 pyilz-0.0.5/pyilz/get_timers.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 pyilz-0.0.5/pyilz/get_token.py
--rw-r--r--   0        0        0     5729 2020-02-02 00:00:00.000000 pyilz-0.0.5/pyilz/parse_land.py
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 pyilz-0.0.5/pyilz/refresh_token.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyilz-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0   264324 2020-02-02 00:00:00.000000 pyilz-0.0.5/tests/example_game_state.json
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 pyilz-0.0.5/tests/test_e2e.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 pyilz-0.0.5/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pyilz-0.0.5/LICENSE
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 pyilz-0.0.5/README.md
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 pyilz-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 pyilz-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pyilz-0.0.6/requirements.txt
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 pyilz-0.0.6/.github/workflows/main.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyilz-0.0.6/pyilz/__init__.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pyilz-0.0.6/pyilz/get_device_id.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 pyilz-0.0.6/pyilz/get_game_state.py
+-rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 pyilz-0.0.6/pyilz/get_timers.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 pyilz-0.0.6/pyilz/get_token.py
+-rw-r--r--   0        0        0     5729 2020-02-02 00:00:00.000000 pyilz-0.0.6/pyilz/parse_land.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 pyilz-0.0.6/pyilz/refresh_token.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyilz-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0   264324 2020-02-02 00:00:00.000000 pyilz-0.0.6/tests/example_game_state.json
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 pyilz-0.0.6/tests/test_e2e.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 pyilz-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pyilz-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 pyilz-0.0.6/README.md
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 pyilz-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 pyilz-0.0.6/PKG-INFO
```

### Comparing `pyilz-0.0.5/.github/workflows/main.yml` & `pyilz-0.0.6/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pyilz-0.0.5/pyilz/get_device_id.py` & `pyilz-0.0.6/pyilz/get_device_id.py`

 * *Files identical despite different names*

### Comparing `pyilz-0.0.5/pyilz/get_game_state.py` & `pyilz-0.0.6/pyilz/get_game_state.py`

 * *Files identical despite different names*

### Comparing `pyilz-0.0.5/pyilz/get_timers.py` & `pyilz-0.0.6/pyilz/get_timers.py`

 * *Files identical despite different names*

### Comparing `pyilz-0.0.5/pyilz/parse_land.py` & `pyilz-0.0.6/pyilz/parse_land.py`

 * *Files identical despite different names*

### Comparing `pyilz-0.0.5/pyilz/refresh_token.py` & `pyilz-0.0.6/pyilz/refresh_token.py`

 * *Files identical despite different names*

### Comparing `pyilz-0.0.5/tests/example_game_state.json` & `pyilz-0.0.6/tests/example_game_state.json`

 * *Files identical despite different names*

### Comparing `pyilz-0.0.5/.gitignore` & `pyilz-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pyilz-0.0.5/LICENSE` & `pyilz-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyilz-0.0.5/README.md` & `pyilz-0.0.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -15,32 +15,35 @@
 Install using `pip`...
 
     pip install pyilz
 
 
 # Example
 ```py
-from pyilz import get_token, get_game_state, parse_land, get_timers
+from pyilz.get_token import get_token
+from pyilz.get_game_state import get_game_state
+from pyilz.parse_land import parse_land
+from pyilz.get_timers import get_timers
 
 # Load ACCESS_TOKEN and REFRESH_TOKEN env vars
 import dotenv
 dotenv.load_dotenv()
 
 # Get access token
-token = get_token.get_token()
+token = get_token()
 
 # Get list of plots
-plots = get_game_state.get_game_state(token)
+plots = get_game_state(token)['data']
 
 # Get Current, Automatic and Completed Actions
 land = plots[2]['data']
-_, _, ca, aa, completed = parse_land.parse_land(land)
+_, _, ca, aa, completed = parse_land(land)
 
 # Get timers from actions
-timers = get_timers.get_timers(ca, aa, completed)
+timers = get_timers(ca, aa, completed)
 print(timers)
 ```
 
 # Package management
 ### Build
 ```ps
 py -m pip install --upgrade build
```

### Comparing `pyilz-0.0.5/pyproject.toml` & `pyilz-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyilz"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Nick Jordan", email="nickjordan289@gmail.com" },
 ]
 description = "A Python Library for Illuvium Zero Land Management"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pyilz-0.0.5/PKG-INFO` & `pyilz-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyilz
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python Library for Illuvium Zero Land Management
 Project-URL: Homepage, https://github.com/NickJordan289/pyilz
 Project-URL: Bug Tracker, https://github.com/NickJordan289/pyilz/issues
 Author-email: Nick Jordan <nickjordan289@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -29,32 +29,35 @@
 Install using `pip`...
 
     pip install pyilz
 
 
 # Example
 ```py
-from pyilz import get_token, get_game_state, parse_land, get_timers
+from pyilz.get_token import get_token
+from pyilz.get_game_state import get_game_state
+from pyilz.parse_land import parse_land
+from pyilz.get_timers import get_timers
 
 # Load ACCESS_TOKEN and REFRESH_TOKEN env vars
 import dotenv
 dotenv.load_dotenv()
 
 # Get access token
-token = get_token.get_token()
+token = get_token()
 
 # Get list of plots
-plots = get_game_state.get_game_state(token)
+plots = get_game_state(token)['data']
 
 # Get Current, Automatic and Completed Actions
 land = plots[2]['data']
-_, _, ca, aa, completed = parse_land.parse_land(land)
+_, _, ca, aa, completed = parse_land(land)
 
 # Get timers from actions
-timers = get_timers.get_timers(ca, aa, completed)
+timers = get_timers(ca, aa, completed)
 print(timers)
 ```
 
 # Package management
 ### Build
 ```ps
 py -m pip install --upgrade build
```

