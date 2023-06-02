# Comparing `tmp/weather_command-6.1.0.tar.gz` & `tmp/weather_command-6.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weather_command-6.1.0.tar", max compression
+gzip compressed data, was "weather_command-6.1.1.tar", max compression
```

## Comparing `weather_command-6.1.0.tar` & `weather_command-6.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1069 2023-04-20 09:12:21.835913 weather_command-6.1.0/LICENSE
--rw-r--r--   0        0        0     3015 2023-04-20 09:12:21.835913 weather_command-6.1.0/README.md
--rw-r--r--   0        0        0     1841 2023-04-20 09:12:21.839913 weather_command-6.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-20 09:12:21.839913 weather_command-6.1.0/weather_command/__init__.py
--rw-r--r--   0        0        0       95 2023-04-20 09:12:21.839913 weather_command-6.1.0/weather_command/__main__.py
--rw-r--r--   0        0        0    18650 2023-04-20 09:12:21.843913 weather_command-6.1.0/weather_command/_builder.py
--rw-r--r--   0        0        0     5268 2023-04-20 09:12:21.843913 weather_command-6.1.0/weather_command/_cache.py
--rw-r--r--   0        0        0     5262 2023-04-20 09:12:21.843913 weather_command-6.1.0/weather_command/_config.py
--rw-r--r--   0        0        0     2667 2023-04-20 09:12:21.843913 weather_command-6.1.0/weather_command/_location.py
--rw-r--r--   0        0        0      473 2023-04-20 09:12:21.843913 weather_command-6.1.0/weather_command/_utils.py
--rw-r--r--   0        0        0     2849 2023-04-20 09:12:21.843913 weather_command-6.1.0/weather_command/_weather.py
--rw-r--r--   0        0        0      459 2023-04-20 09:12:21.843913 weather_command-6.1.0/weather_command/errors.py
--rw-r--r--   0        0        0     9084 2023-04-20 09:12:21.843913 weather_command-6.1.0/weather_command/main.py
--rw-r--r--   0        0        0        0 2023-04-20 09:12:21.843913 weather_command-6.1.0/weather_command/models/__init__.py
--rw-r--r--   0        0        0      133 2023-04-20 09:12:21.843913 weather_command-6.1.0/weather_command/models/location.py
--rw-r--r--   0        0        0     3053 2023-04-20 09:12:21.843913 weather_command-6.1.0/weather_command/models/weather.py
--rw-r--r--   0        0        0        0 2023-04-20 09:12:21.843913 weather_command-6.1.0/weather_command/py.typed
--rw-r--r--   0        0        0     2816 2023-04-20 09:12:21.843913 weather_command-6.1.0/weather_command/settings_commands.py
--rw-r--r--   0        0        0     4062 1970-01-01 00:00:00.000000 weather_command-6.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-02 02:22:00.480474 weather_command-6.1.1/LICENSE
+-rw-r--r--   0        0        0     3393 2023-06-02 02:22:00.480474 weather_command-6.1.1/README.md
+-rw-r--r--   0        0        0     1793 2023-06-02 02:22:00.484476 weather_command-6.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-02 02:22:00.484476 weather_command-6.1.1/weather_command/__init__.py
+-rw-r--r--   0        0        0       95 2023-06-02 02:22:00.484476 weather_command-6.1.1/weather_command/__main__.py
+-rw-r--r--   0        0        0    18650 2023-06-02 02:22:00.484476 weather_command-6.1.1/weather_command/_builder.py
+-rw-r--r--   0        0        0     5340 2023-06-02 02:22:00.484476 weather_command-6.1.1/weather_command/_cache.py
+-rw-r--r--   0        0        0     5262 2023-06-02 02:22:00.484476 weather_command-6.1.1/weather_command/_config.py
+-rw-r--r--   0        0        0     2667 2023-06-02 02:22:00.484476 weather_command-6.1.1/weather_command/_location.py
+-rw-r--r--   0        0        0      473 2023-06-02 02:22:00.484476 weather_command-6.1.1/weather_command/_utils.py
+-rw-r--r--   0        0        0     2849 2023-06-02 02:22:00.484476 weather_command-6.1.1/weather_command/_weather.py
+-rw-r--r--   0        0        0      459 2023-06-02 02:22:00.484476 weather_command-6.1.1/weather_command/errors.py
+-rw-r--r--   0        0        0     9084 2023-06-02 02:22:00.484476 weather_command-6.1.1/weather_command/main.py
+-rw-r--r--   0        0        0        0 2023-06-02 02:22:00.484476 weather_command-6.1.1/weather_command/models/__init__.py
+-rw-r--r--   0        0        0      133 2023-06-02 02:22:00.484476 weather_command-6.1.1/weather_command/models/location.py
+-rw-r--r--   0        0        0     3053 2023-06-02 02:22:00.484476 weather_command-6.1.1/weather_command/models/weather.py
+-rw-r--r--   0        0        0        0 2023-06-02 02:22:00.484476 weather_command-6.1.1/weather_command/py.typed
+-rw-r--r--   0        0        0     2816 2023-06-02 02:22:00.484476 weather_command-6.1.1/weather_command/settings_commands.py
+-rw-r--r--   0        0        0     4440 1970-01-01 00:00:00.000000 weather_command-6.1.1/PKG-INFO
```

### Comparing `weather_command-6.1.0/LICENSE` & `weather_command-6.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `weather_command-6.1.0/pyproject.toml` & `weather_command-6.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 [tool.poetry]
 name = "weather-command"
-version = "6.1.0"
+version = "6.1.1"
 description = "Command line weather app"
 authors = ["Paul Sanders <psanders1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sanders41/weather-command"
 homepage = "https://github.com/sanders41/weather-command"
 documentation = "https://github.com/sanders41/weather-command"
 keywords = ["weather", "cli"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-rich = "13.3.4"
-httpx = "0.24.0"
-pydantic = "1.10.7"
+rich = "13.4.1"
+httpx = "0.24.1"
+pydantic = "1.10.8"
 camel-converter = {version = "3.0.0", extras = ["pydantic"]}
-typer = "0.7.0"
+typer = "0.9.0"
 tenacity = "8.2.2"
 pyyaml = "6.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "23.3.0"
-mypy = "1.2.0"
+mypy = "1.3.0"
 pre-commit = "2.21.0"
 pytest = "7.3.1"
-pytest-cov = "4.0.0"
-tox = "4.4.12"
-ruff = "0.0.262"
+pytest-cov = "4.1.0"
+ruff = "0.0.270"
 tomli = {version = "2.0.1", python = "<3.11"}
-types-pyyaml = "6.0.12.9"
+types-pyyaml = "6.0.12.10"
 pytest-asyncio = "0.21.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
@@ -77,11 +76,12 @@
 addopts = "--cov=weather_command --cov-report term-missing"
 asyncio_mode = "auto"
 
 [tool.coverage.report]
 exclude_lines = ["if __name__ == .__main__.:", "pragma: no cover"]
 
 [tool.ruff]
-select = ["E", "F", "T201", "T203", "I001"]
-ignore = ["E501", "D100", "D101", "D102", "D103", "D104", "D105", "D106", "D107"]
+select = ["E", "F", "UP", "I001", "T201", "T203"]
+ignore = ["E501"]
 line-length = 100
+target-version = "py37"
 fix = true
```

### Comparing `weather_command-6.1.0/weather_command/_builder.py` & `weather_command-6.1.1/weather_command/_builder.py`

 * *Files identical despite different names*

### Comparing `weather_command-6.1.0/weather_command/_cache.py` & `weather_command-6.1.1/weather_command/_cache.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-from __future__ import annotations
-
 import json
 import os
-from datetime import date, datetime
+from datetime import date, datetime, timezone
 from json import JSONEncoder
 from pathlib import Path
-from typing import Any, Optional
+from typing import Any, Dict, Optional, Union
 
 from camel_converter.pydantic_base import CamelBase
 
 from weather_command.models.location import Location
 from weather_command.models.weather import CurrentWeather, OneCallWeather
 
 
@@ -49,44 +47,44 @@
     )
     return settings_path.resolve()
 
 
 class Cache:
     get_default_directory = staticmethod(_get_default_directory)
 
-    def __init__(self, cache_dir: Path | None = None) -> None:
+    def __init__(self, cache_dir: Union[Path, None] = None) -> None:
         self.cache_dir = cache_dir or Cache.get_default_directory()
         self._cache_file = self.cache_dir / "cache.json"
         if not self.cache_dir.exists():
             self.cache_dir.mkdir(parents=True)
 
-        self._cache: dict[str, CacheItem] | None = self._load()
+        self._cache: Union[Dict[str, CacheItem], None] = self._load()
 
     def add(
         self,
         *,
         cache_key: str,
-        location: Location | None = None,
-        current_weather: CurrentWeather | None = None,
-        one_call_weather: OneCallWeather | None = None,
+        location: Union[Location, None] = None,
+        current_weather: Union[CurrentWeather, None] = None,
+        one_call_weather: Union[OneCallWeather, None] = None,
         cache_size: int = 5,
     ) -> None:
         def save_cache() -> None:
             cache: dict[str, Any] = {}
             location_cache = location.dict() if location else None
             current_weather_cache = (
                 CurrentWeatherCache(
-                    date_time_saved=datetime.utcnow(), current_weather=current_weather
+                    date_time_saved=datetime.now(tz=timezone.utc), current_weather=current_weather
                 ).dict()
                 if current_weather
                 else None
             )
             one_call_weather_cache = (
                 OneCallWeatherCache(
-                    date_time_saved=datetime.utcnow(), one_call_weather=one_call_weather
+                    date_time_saved=datetime.now(tz=timezone.utc), one_call_weather=one_call_weather
                 ).dict()
                 if one_call_weather
                 else None
             )
 
             cache_hit = self.get(cache_key)
 
@@ -125,32 +123,32 @@
             del self._cache[last_key]
             save_cache()
 
     def clear(self) -> None:
         if self._cache_file.exists():
             self._cache_file.unlink()
 
-    def get(self, cache_key: str) -> CacheItem | None:
+    def get(self, cache_key: str) -> Union[CacheItem, None]:
         if not self._cache or not self._cache.get(cache_key):
             return None
 
         cache = self._cache[cache_key.lower()]
         if cache.current_weather:
-            time_diff = datetime.utcnow() - cache.current_weather.date_time_saved
+            time_diff = datetime.now(tz=timezone.utc) - cache.current_weather.date_time_saved
             if (time_diff.total_seconds() / 60) > cache.current_weather.cache_duration_minutes:
                 cache.current_weather = None
 
         if cache.one_call_weather:
-            time_diff = datetime.utcnow() - cache.one_call_weather.date_time_saved
+            time_diff = datetime.now(tz=timezone.utc) - cache.one_call_weather.date_time_saved
             if (time_diff.total_seconds() / 60) > cache.one_call_weather.cache_duration_minutes:
                 cache.one_call_weather = None
 
         return cache
 
-    def _load(self) -> dict[str, CacheItem] | None:
+    def _load(self) -> Union[Dict[str, CacheItem], None]:
         if not self._cache_file.exists():
             return None
 
-        with open(self._cache_file, "r") as f:
+        with open(self._cache_file) as f:
             json_cache = json.load(f)
 
         return {k: CacheItem(**v) for k, v in json_cache.items()}
```

### Comparing `weather_command-6.1.0/weather_command/_config.py` & `weather_command-6.1.1/weather_command/_config.py`

 * *Files identical despite different names*

### Comparing `weather_command-6.1.0/weather_command/_location.py` & `weather_command-6.1.1/weather_command/_location.py`

 * *Files identical despite different names*

### Comparing `weather_command-6.1.0/weather_command/_weather.py` & `weather_command-6.1.1/weather_command/_weather.py`

 * *Files identical despite different names*

### Comparing `weather_command-6.1.0/weather_command/main.py` & `weather_command-6.1.1/weather_command/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from weather_command._builder import show_current, show_daily, show_hourly
 from weather_command._cache import Cache
 from weather_command._config import console, load_settings
 from weather_command._location import build_location_url, get_location_details
 from weather_command._utils import build_weather_url
 from weather_command._weather import get_current_weather, get_one_call_weather
 
-__version__ = "6.1.0"
+__version__ = "6.1.1"
 
 app = Typer()
 app.add_typer(settings_commands.app, name="settings", help="Manage saved settings.")
 
 
 class ForecastType(str, Enum):
     CURRENT = "current"
```

### Comparing `weather_command-6.1.0/weather_command/models/weather.py` & `weather_command-6.1.1/weather_command/models/weather.py`

 * *Files identical despite different names*

### Comparing `weather_command-6.1.0/weather_command/settings_commands.py` & `weather_command-6.1.1/weather_command/settings_commands.py`

 * *Files identical despite different names*

### Comparing `weather_command-6.1.0/PKG-INFO` & `weather_command-6.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weather-command
-Version: 6.1.0
+Version: 6.1.1
 Summary: Command line weather app
 Home-page: https://github.com/sanders41/weather-command
 License: MIT
 Keywords: weather,cli
 Author: Paul Sanders
 Author-email: psanders1@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -12,20 +12,20 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: camel-converter[pydantic] (==3.0.0)
-Requires-Dist: httpx (==0.24.0)
-Requires-Dist: pydantic (==1.10.7)
+Requires-Dist: httpx (==0.24.1)
+Requires-Dist: pydantic (==1.10.8)
 Requires-Dist: pyyaml (==6.0)
-Requires-Dist: rich (==13.3.4)
+Requires-Dist: rich (==13.4.1)
 Requires-Dist: tenacity (==8.2.2)
-Requires-Dist: typer (==0.7.0)
+Requires-Dist: typer (==0.9.0)
 Project-URL: Documentation, https://github.com/sanders41/weather-command
 Project-URL: Repository, https://github.com/sanders41/weather-command
 Description-Content-Type: text/markdown
 
 # Weather Command
 
 [![Tests Status](https://github.com/sanders41/weather-command/workflows/Testing/badge.svg?branch=main&event=push)](https://github.com/sanders41/weather-command/actions?query=workflow%3ATesting+branch%3Amain+event%3Apush)
@@ -82,35 +82,35 @@
 After adding this to the `~/.zshrc` you will need to restart your terminal. After that typing `we`
 will get the current forecast, `wed` will get the daily forecast and `weh` will get the hourly forecast.
 
 ## Examples
 
 - Current Weather
 
-![Current weather](./assets/current.png)
+![Current weather](https://raw.githubusercontent.com/sanders41/weather-command/main/assets/current.png)
 
 - Current Weather Temp Only
 
-![Current weather temp only](./assets/current_temp_only.png)
+![Current weather temp only](https://raw.githubusercontent.com/sanders41/weather-command/main/assets/current_temp_only.png)
 
 - Daily Weather
 
-![Daily weather](./assets/daily.png)
+![Daily weather](https://raw.githubusercontent.com/sanders41/weather-command/main/assets/daily.png)
 
 - Daily Weather Temp Only
 
-![Daily weather temp only](./assets/daily_temp_only.png)
+![Daily weather temp only](https://raw.githubusercontent.com/sanders41/weather-command/main/assets/daily_temp_only.png)
 
 - Hourly Weather
 
-![Hourly weather](./assets/hourly.png)
+![Hourly weather](https://raw.githubusercontent.com/sanders41/weather-command/main/assets/hourly.png)
 
 - Hourly Weather Temp Only
 
-![Hourl weather temp only](./assets/hourly_temp_only.png)
+![Hourl weather temp only](https://raw.githubusercontent.com/sanders41/weather-command/main/assets/hourly_temp_only.png)
 
 ## Settings
 weather now has the ability to save settings to default certain flags. The list of possible settings can be seen with:
 
 ```sh
 weather settings --help
 ```
```

