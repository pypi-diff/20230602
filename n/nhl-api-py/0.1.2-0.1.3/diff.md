# Comparing `tmp/nhl_api_py-0.1.2.tar.gz` & `tmp/nhl_api_py-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nhl_api_py-0.1.2.tar", max compression
+gzip compressed data, was "nhl_api_py-0.1.3.tar", max compression
```

## Comparing `nhl_api_py-0.1.2.tar` & `nhl_api_py-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0      966 2023-06-01 21:42:25.752450 nhl_api_py-0.1.2/README.md
--rw-r--r--   0        0        0       32 2023-06-01 15:54:04.739415 nhl_api_py-0.1.2/nhlpy/__init__.py
--rw-r--r--   0        0        0      309 2023-06-01 16:00:57.059417 nhl_api_py-0.1.2/nhlpy/api/__init__.py
--rw-r--r--   0        0        0      472 2023-06-01 16:03:00.509418 nhl_api_py-0.1.2/nhlpy/api/core.py
--rw-r--r--   0        0        0      778 2023-06-01 17:09:37.399440 nhl_api_py-0.1.2/nhlpy/api/standings.py
--rw-r--r--   0        0        0      846 2023-06-01 16:57:52.189436 nhl_api_py-0.1.2/nhlpy/api/teams.py
--rw-r--r--   0        0        0      209 2023-06-01 17:01:57.729437 nhl_api_py-0.1.2/nhlpy/nhlclient.py
--rw-r--r--   0        0        0     1257 2023-06-01 21:39:21.482451 nhl_api_py-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 nhl_api_py-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1370 2023-06-02 19:17:51.559748 nhl_api_py-0.1.3/README.md
+-rw-r--r--   0        0        0       33 2023-06-02 18:53:59.479744 nhl_api_py-0.1.3/nhlpy/__init__.py
+-rw-r--r--   0        0        0      309 2023-06-01 16:00:57.059417 nhl_api_py-0.1.3/nhlpy/api/__init__.py
+-rw-r--r--   0        0        0      472 2023-06-01 16:03:00.509418 nhl_api_py-0.1.3/nhlpy/api/core.py
+-rw-r--r--   0        0        0     1884 2023-06-02 19:14:40.749748 nhl_api_py-0.1.3/nhlpy/api/players.py
+-rw-r--r--   0        0        0      389 2023-06-02 18:52:47.229744 nhl_api_py-0.1.3/nhlpy/api/schedule.py
+-rw-r--r--   0        0        0     1365 2023-06-02 19:18:58.449748 nhl_api_py-0.1.3/nhlpy/api/standings.py
+-rw-r--r--   0        0        0     1073 2023-06-02 18:40:42.149742 nhl_api_py-0.1.3/nhlpy/api/teams.py
+-rw-r--r--   0        0        0      392 2023-06-02 19:19:13.409748 nhl_api_py-0.1.3/nhlpy/nhl_client.py
+-rw-r--r--   0        0        0     1257 2023-06-02 19:22:11.479749 nhl_api_py-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2402 1970-01-01 00:00:00.000000 nhl_api_py-0.1.3/PKG-INFO
```

### Comparing `nhl_api_py-0.1.2/README.md` & `nhl_api_py-0.1.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # NHL-py-api
 
 NHL-py-api is a Python package that provides a simple wrapper around the 
 NHL API, allowing you to easily access and retrieve NHL data in your Python 
 applications.
 
 Note: This is very early, I created this to help me with some machine learning
-projects around the NHL and the NHL data sets.
+projects around the NHL and the NHL data sets.  Special thanks to https://github.com/erunion/sport-api-specifications/tree/master/nhl.
 
 
 ## Installation
 
 You can install NHL-py-api using pip:
 
 ```shell
@@ -35,14 +35,20 @@
 client.teams.get_team_next_game(id=1)
 client.teams.get_team_previous_game(id=1)
 client.teams.get_team_stats(id=1)
 
 # Standings
 client.standings.get_standings(season="20222023", detailed_record=False)
 client.standings.get_standing_types()
+
+# Player Stats
+client.players.get_player_stats(person_id=8477949, season="20222023", stat_type="statsSingleSeason")
+client.players.get_player_stats(person_id=8477949, season="20222023", stat_type="goalsByGameSituation")
+client.players.get_player_stats(person_id=8477949, season="20222023", stat_type="yearByYear")
+
 ```
 
 - - - 
 
 
 ### Developers
```

### Comparing `nhl_api_py-0.1.2/nhlpy/api/teams.py` & `nhl_api_py-0.1.3/nhlpy/api/teams.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,9 +18,15 @@
 
     def get_team_next_game(self, id: int) -> dict:
         return self._get(resource=f"teams/{id}?expand=team.schedule.next").json()
 
     def get_team_previous_game(self, id: int) -> dict:
         return self._get(resource=f"teams/{id}?expand=team.schedule.previous").json()
 
+    def get_team_with_stats(self, id: int) -> dict:
+        return self._get(resource=f"teams/{id}?expand=team.stats").json()
+
+    def get_team_roster(self, id: int) -> dict:
+        return self._get(resource=f"teams/{id}/roster").json()
+
     def get_team_stats(self, id: int) -> dict:
-        return self._get(resource=f"teams/{id}?expand=team.stats").json()
+        return self._get(resource=f"teams/{id}/stats").json()
```

### Comparing `nhl_api_py-0.1.2/pyproject.toml` & `nhl_api_py-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nhl-api-py"
-version = "0.1.2"
+version = "0.1.3"
 description = "NHL API Wrapper.  For standings, team stats and outcomes."
 authors = ["Corey Schaf <cschaf@gmail.com>"]
 readme = "README.md"
 packages = [{include = "nhlpy"}]
 license = "GPL-3.0-or-later"
 homepage = "https://github.com/coreyjs/nhl-api-py"
 repository = "https://github.com/coreyjs/nhl-api-py"
```

### Comparing `nhl_api_py-0.1.2/PKG-INFO` & `nhl_api_py-0.1.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nhl-api-py
-Version: 0.1.2
+Version: 0.1.3
 Summary: NHL API Wrapper.  For standings, team stats and outcomes.
 Home-page: https://github.com/coreyjs/nhl-api-py
 License: GPL-3.0-or-later
 Keywords: nhl,api,wrapper,hockey,sports
 Author: Corey Schaf
 Author-email: cschaf@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -28,15 +28,15 @@
 # NHL-py-api
 
 NHL-py-api is a Python package that provides a simple wrapper around the 
 NHL API, allowing you to easily access and retrieve NHL data in your Python 
 applications.
 
 Note: This is very early, I created this to help me with some machine learning
-projects around the NHL and the NHL data sets.
+projects around the NHL and the NHL data sets.  Special thanks to https://github.com/erunion/sport-api-specifications/tree/master/nhl.
 
 
 ## Installation
 
 You can install NHL-py-api using pip:
 
 ```shell
@@ -59,14 +59,20 @@
 client.teams.get_team_next_game(id=1)
 client.teams.get_team_previous_game(id=1)
 client.teams.get_team_stats(id=1)
 
 # Standings
 client.standings.get_standings(season="20222023", detailed_record=False)
 client.standings.get_standing_types()
+
+# Player Stats
+client.players.get_player_stats(person_id=8477949, season="20222023", stat_type="statsSingleSeason")
+client.players.get_player_stats(person_id=8477949, season="20222023", stat_type="goalsByGameSituation")
+client.players.get_player_stats(person_id=8477949, season="20222023", stat_type="yearByYear")
+
 ```
 
 - - - 
 
 
 ### Developers
```

