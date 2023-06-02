# Comparing `tmp/databallpy-0.2.3.tar.gz` & `tmp/databallpy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databallpy-0.2.3.tar", max compression
+gzip compressed data, was "databallpy-0.3.0.tar", max compression
```

## Comparing `databallpy-0.2.3.tar` & `databallpy-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,36 @@
--rwxr-xr-x   0        0        0     1085 2023-01-24 11:30:08.329567 databallpy-0.2.3/LICENSE
--rw-r--r--   0        0        0     5252 2023-03-12 15:16:14.548439 databallpy-0.2.3/README.md
--rw-r--r--   0        0        0      304 2023-03-10 13:55:09.165274 databallpy-0.2.3/databallpy/__init__.py
--rw-r--r--   0        0        0        0 2023-02-10 10:17:56.160462 databallpy-0.2.3/databallpy/load_data/__init__.py
--rw-r--r--   0        0        0        0 2023-02-10 10:17:56.160612 databallpy-0.2.3/databallpy/load_data/event_data/__init__.py
--rw-r--r--   0        0        0     1554 2023-03-10 11:37:51.954815 databallpy-0.2.3/databallpy/load_data/event_data/_normalize_playing_direction_events.py
--rw-r--r--   0        0        0     5891 2023-03-12 15:14:04.088586 databallpy-0.2.3/databallpy/load_data/event_data/metrica_event_data.py
--rw-r--r--   0        0        0    11920 2023-03-10 11:37:51.955156 databallpy-0.2.3/databallpy/load_data/event_data/opta.py
--rw-r--r--   0        0        0     7126 2023-03-10 11:37:51.955359 databallpy-0.2.3/databallpy/load_data/metadata.py
--rw-r--r--   0        0        0     9907 2023-03-10 11:37:51.955501 databallpy-0.2.3/databallpy/load_data/metrica_metadata.py
--rw-r--r--   0        0        0        0 2023-02-10 10:17:56.161101 databallpy-0.2.3/databallpy/load_data/tracking_data/__init__.py
--rw-r--r--   0        0        0      698 2023-02-24 18:54:05.247634 databallpy-0.2.3/databallpy/load_data/tracking_data/_add_ball_data_to_dict.py
--rw-r--r--   0        0        0     1568 2023-03-10 11:37:51.955584 databallpy-0.2.3/databallpy/load_data/tracking_data/_add_periods_to_tracking_data.py
--rw-r--r--   0        0        0      969 2023-02-24 18:54:05.247989 databallpy-0.2.3/databallpy/load_data/tracking_data/_add_player_tracking_data_to_dict.py
--rw-r--r--   0        0        0     3473 2023-03-10 11:37:51.956055 databallpy-0.2.3/databallpy/load_data/tracking_data/_get_matchtime.py
--rw-r--r--   0        0        0     1031 2023-02-10 10:17:56.162980 databallpy-0.2.3/databallpy/load_data/tracking_data/_insert_missing_rows.py
--rw-r--r--   0        0        0     1172 2023-03-10 11:37:51.956324 databallpy-0.2.3/databallpy/load_data/tracking_data/_normalize_playing_direction_tracking.py
--rw-r--r--   0        0        0     6148 2023-03-12 15:14:04.088795 databallpy-0.2.3/databallpy/load_data/tracking_data/metrica_tracking_data.py
--rw-r--r--   0        0        0     8298 2023-03-10 11:37:51.956660 databallpy-0.2.3/databallpy/load_data/tracking_data/tracab.py
--rw-r--r--   0        0        0    30840 2023-03-12 15:19:34.977197 databallpy-0.2.3/databallpy/match.py
--rw-r--r--   0        0        0      763 2023-03-10 11:37:51.957026 databallpy-0.2.3/databallpy/utils.py
--rw-r--r--   0        0        0    18377 2023-03-12 15:19:34.977869 databallpy-0.2.3/databallpy/visualize.py
--rw-r--r--   0        0        0     2525 2023-03-12 15:14:22.570473 databallpy-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     6396 1970-01-01 00:00:00.000000 databallpy-0.2.3/setup.py
--rw-r--r--   0        0        0     6804 1970-01-01 00:00:00.000000 databallpy-0.2.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1085 2023-01-24 11:30:08.329567 databallpy-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5601 2023-06-02 18:05:51.279039 databallpy-0.3.0/README.md
+-rw-r--r--   0        0        0      191 2023-05-13 07:28:52.676655 databallpy-0.3.0/databallpy/__init__.py
+-rw-r--r--   0        0        0      188 2023-05-13 07:28:52.676769 databallpy-0.3.0/databallpy/errors.py
+-rw-r--r--   0        0        0        0 2023-05-23 13:42:10.199898 databallpy-0.3.0/databallpy/features/__init__.py
+-rw-r--r--   0        0        0      977 2023-06-02 17:51:23.224996 databallpy-0.3.0/databallpy/features/velocity.py
+-rw-r--r--   0        0        0    14220 2023-06-02 17:51:23.225230 databallpy-0.3.0/databallpy/get_match.py
+-rw-r--r--   0        0        0        0 2023-02-10 10:17:56.160462 databallpy-0.3.0/databallpy/load_data/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-10 10:17:56.160612 databallpy-0.3.0/databallpy/load_data/event_data/__init__.py
+-rw-r--r--   0        0        0     1554 2023-03-12 15:25:48.209137 databallpy-0.3.0/databallpy/load_data/event_data/_normalize_playing_direction_events.py
+-rw-r--r--   0        0        0    11983 2023-05-23 13:42:10.200791 databallpy-0.3.0/databallpy/load_data/event_data/instat.py
+-rw-r--r--   0        0        0     6046 2023-05-07 15:03:40.624364 databallpy-0.3.0/databallpy/load_data/event_data/metrica_event_data.py
+-rw-r--r--   0        0        0    13205 2023-06-02 17:51:23.225484 databallpy-0.3.0/databallpy/load_data/event_data/opta.py
+-rw-r--r--   0        0        0     8024 2023-05-30 11:34:09.440544 databallpy-0.3.0/databallpy/load_data/metadata.py
+-rw-r--r--   0        0        0    11737 2023-05-23 13:42:10.201042 databallpy-0.3.0/databallpy/load_data/metrica_metadata.py
+-rw-r--r--   0        0        0        0 2023-02-10 10:17:56.161101 databallpy-0.3.0/databallpy/load_data/tracking_data/__init__.py
+-rw-r--r--   0        0        0      757 2023-05-07 15:03:40.625076 databallpy-0.3.0/databallpy/load_data/tracking_data/_add_ball_data_to_dict.py
+-rw-r--r--   0        0        0     1644 2023-05-23 13:42:10.201200 databallpy-0.3.0/databallpy/load_data/tracking_data/_add_periods_to_tracking_data.py
+-rw-r--r--   0        0        0      961 2023-04-25 15:26:54.930980 databallpy-0.3.0/databallpy/load_data/tracking_data/_add_player_tracking_data_to_dict.py
+-rw-r--r--   0        0        0     3527 2023-05-23 13:42:10.201343 databallpy-0.3.0/databallpy/load_data/tracking_data/_get_matchtime.py
+-rw-r--r--   0        0        0     1031 2023-02-10 10:17:56.162980 databallpy-0.3.0/databallpy/load_data/tracking_data/_insert_missing_rows.py
+-rw-r--r--   0        0        0     1160 2023-05-01 15:00:27.444838 databallpy-0.3.0/databallpy/load_data/tracking_data/_normalize_playing_direction_tracking.py
+-rw-r--r--   0        0        0    11401 2023-06-02 17:51:23.225734 databallpy-0.3.0/databallpy/load_data/tracking_data/_quality_check_tracking_data.py
+-rw-r--r--   0        0        0    10444 2023-05-23 13:42:10.201633 databallpy-0.3.0/databallpy/load_data/tracking_data/inmotio.py
+-rw-r--r--   0        0        0     6106 2023-05-07 15:03:40.625412 databallpy-0.3.0/databallpy/load_data/tracking_data/metrica_tracking_data.py
+-rw-r--r--   0        0        0     8771 2023-05-23 13:42:10.201789 databallpy-0.3.0/databallpy/load_data/tracking_data/tracab.py
+-rw-r--r--   0        0        0    19833 2023-06-02 17:51:23.226003 databallpy-0.3.0/databallpy/match.py
+-rw-r--r--   0        0        0        0 2023-05-07 15:03:40.625878 databallpy-0.3.0/databallpy/utils/__init__.py
+-rw-r--r--   0        0        0    10874 2023-06-02 17:51:23.226279 databallpy-0.3.0/databallpy/utils/synchronise_tracking_and_event_data.py
+-rw-r--r--   0        0        0     2003 2023-05-13 08:42:27.134855 databallpy-0.3.0/databallpy/utils/tz_modification.py
+-rw-r--r--   0        0        0     2931 2023-05-23 13:42:10.202310 databallpy-0.3.0/databallpy/utils/utils.py
+-rw-r--r--   0        0        0    18381 2023-05-01 14:32:31.340350 databallpy-0.3.0/databallpy/visualize.py
+-rw-r--r--   0        0        0      190 2023-05-23 13:42:10.202488 databallpy-0.3.0/databallpy/warnings.py
+-rw-r--r--   0        0        0     2524 2023-06-02 17:59:04.862948 databallpy-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6800 1970-01-01 00:00:00.000000 databallpy-0.3.0/setup.py
+-rw-r--r--   0        0        0     7146 1970-01-01 00:00:00.000000 databallpy-0.3.0/PKG-INFO
```

### Comparing `databallpy-0.2.3/LICENSE` & `databallpy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `databallpy-0.2.3/README.md` & `databallpy-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # databallpy
 
 A package for loading, preprocessing, vizualising and synchronizing soccer event- and tracking data.
 
 This package is developed to create a standardized way to analyse soccer matches using both event- and tracking data. Other packages, like [kloppy](https://github.com/PySport/kloppy) and [floodlight](https://github.com/floodlight-sports/floodlight), already standardize the import of data sources. The current package goes a step further in combining different data streams from the same match. In this case, the `Match` object combines information from the event and tracking data.
 
-### Changelog for version 0.2.0
+### Changelog for version 0.3.0
 
-- Added parser for Metrica, including an open dataset
-- Added functionality to synchronize tracking and event data
-- Added functionality to plot events
-- Fixed bug, now both tracking and event data are normalized in direction
-- Fixed unexpected behaviour, all date related objects are now datetime objects
+- Added way to save Match objects, and to load saved Match objects
+- Fixed bug in opta event data, own goals are now parsed as seperate event type
+- Added parser for Inmotio tracking data
+- Added parser for Instat event data
+- Added quality checks for the data, raises warning if quality is not good enough
 
 ### Planned changes
 
 - Adding different filters to filter the tracking data
-- Make the `Match` object more accesable if you don't have tracking or event data
 - Adding features to quantify pressure, ball possession, etc. (if you have any ideas/requests, please open an issue!)
+- Standardizing events in the event data
 - Adding expected passing and goals models
 
 ## Installation
 
 ```bash
 $ pip install databallpy
 ```
 
 ## Usage
 
 The package is centered around the `Match` object. A `Match` has tracking data, event data metadata about the match.
 For a more elaborate example, see the [example file](https://databallpy.readthedocs.io/en/latest/example.html)
 
 ```console
-$ from databallpy.match import get_match, get_open_match
+$ from databallpy import get_match, get_open_match
 $
 $ match = get_match(
 $   tracking_data_loc="../data/tracking_data.dat",
 $   tracking_metadata_loc="../data/tracking_metadata.xml",
 $   tracking_data_provider="tracab"
 $   event_data_loc="../data/event_data_f24.xml",
 $   event_metadata_loc="../data/event_metadata_f7.xml",
@@ -58,47 +58,65 @@
 Tracking and event data is often poorly synchronized. For instance, when taking the event data of Opta and tracking data of Tracab, you can sync the fist frame with the kick-off pass. Now you can sync the other events with the tracking data based on the time difference between the event and the kick off pass. If you do this, how get something like this:
 
 <video width="640" height="480" controls>
   <source src="https://raw.githubusercontent.com/Alek050/databallpy/main/docs/example_data/not_synced.mp4" type="video/mp4">
   Your browser does not support the video tag.
 </video>
 
+https://user-images.githubusercontent.com/49450063/224564808-fa71735f-5510-464d-8499-9044227a02e8.mp4
+
+
 As you can see, the timing (and placing) of the events do not correspond good with the tracking data locations, especially when events follow up quickly or around shots. Using the methodology of [this](https://kwiatkowski.io/sync.soccer) article, this package is able to synchronize tracking and event data using the Needleman-Wunsch algorithm. 
 
 After running the following command, the events are better synchronized to the tracking data:
 
 ```batch
 $ match.synchronise_tracking_and_event_data()
 ```
 
 <video width="640" height="480" controls>
   <source src="https://raw.githubusercontent.com/Alek050/databallpy/main/docs/example_data/synced.mp4" type="video/mp4">
   Your browser does not support the video tag.
 </video>
 
+
+https://user-images.githubusercontent.com/49450063/224564913-4091faf7-f6ef-4429-b132-7f93ce5e1d91.mp4
+
+
 ## Documentation
 
 The official documentation can be found [here](https://databallpy.readthedocs.io/en/latest/autoapi/databallpy/index.html).
 
 ## Providers
 
 For now we limited providers. We are planning on adding more providers later on.
 
 Event data providers:
 - Opta
 - Metrica
+- Instat
 
 Tracking data providers:
 - Tracab
 - Metrica
+- Inmotio
 
 ## Contributing
 
 Interested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.
 
+#### Maintainers & owners
+
+- [Alek050](https://github.com/Alek050/)
+- [DaanGro](https://github.com/DaanGro/)
+
+#### Contributors
+
+- [rdghe](https://github.com/rdghe/)
+
 ## License
 
 `databallpy` was created by Alexander Oonk & Daan Grob. It is licensed under the terms of the MIT license.
 
 ## Similar projects
 
 Although we think this package helps when starting to analyse soccer data, other packages may be better suited for your specific needs. Make sure to check out the following packages as well:
```

### Comparing `databallpy-0.2.3/databallpy/load_data/event_data/_normalize_playing_direction_events.py` & `databallpy-0.3.0/databallpy/load_data/event_data/_normalize_playing_direction_events.py`

 * *Files identical despite different names*

### Comparing `databallpy-0.2.3/databallpy/load_data/event_data/metrica_event_data.py` & `databallpy-0.3.0/databallpy/load_data/event_data/metrica_event_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 )
 from databallpy.load_data.metadata import Metadata
 from databallpy.load_data.metrica_metadata import (
     _get_metadata,
     _get_td_channels,
     _update_metadata,
 )
-from databallpy.utils import _to_float, _to_int
+from databallpy.utils.utils import _to_float, _to_int
 
 
 def load_metrica_event_data(
     event_data_loc: str, metadata_loc: str
 ) -> Tuple[pd.DataFrame, Metadata]:
     """Function to load the metrica event data.
 
@@ -45,15 +45,15 @@
         pass
     else:
         raise TypeError(
             "tracking_data_loc must be either a str or a StringIO object,"
             f" not a {type(event_data_loc)}"
         )
 
-    metadata = _get_metadata(metadata_loc)
+    metadata = _get_metadata(metadata_loc, is_tracking_data=False, is_event_data=True)
     td_channels = _get_td_channels(metadata_loc, metadata)
     metadata = _update_metadata(td_channels, metadata)
     event_data = _get_event_data(event_data_loc)
 
     # rescale the event locations, metrica data is scaled between 0 and 1.
     for col in [x for x in event_data.columns if "_x" in x]:
         event_data[col] = (
@@ -67,22 +67,25 @@
         )
 
     # add datetime based on frame numbers
     first_frame = metadata.periods_frames.loc[
         metadata.periods_frames["period"] == 1, "start_frame"
     ].iloc[0]
     start_time = metadata.periods_frames.loc[
-        metadata.periods_frames["period"] == 1, "start_time_td"
+        metadata.periods_frames["period"] == 1, "start_datetime_ed"
     ].iloc[0]
     frame_rate = metadata.frame_rate
     rel_timedelta = [
         dt.timedelta(milliseconds=(x - first_frame) / frame_rate * 1000)
         for x in event_data["td_frame"]
     ]
-    event_data["datetime"] = [pd.to_datetime(start_time) + x for x in rel_timedelta]
+    # no idea about time zone since we have no real data, so just assume utc
+    event_data["datetime"] = [
+        pd.to_datetime(start_time, utc=True) + x for x in rel_timedelta
+    ]
 
     event_data = _normalize_playing_direction_events(
         event_data, metadata.home_team_id, metadata.away_team_id
     )
 
     return event_data, metadata
```

### Comparing `databallpy-0.2.3/databallpy/load_data/event_data/opta.py` & `databallpy-0.3.0/databallpy/load_data/tracking_data/inmotio.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,357 +1,302 @@
-import datetime as dt
+import os
 from typing import Tuple
 
+import bs4
 import numpy as np
 import pandas as pd
 from bs4 import BeautifulSoup
+from tqdm import tqdm
 
 from databallpy.load_data.metadata import Metadata
+from databallpy.load_data.tracking_data._add_ball_data_to_dict import (
+    _add_ball_data_to_dict,
+)
+from databallpy.load_data.tracking_data._add_periods_to_tracking_data import (
+    _add_periods_to_tracking_data,
+)
+from databallpy.load_data.tracking_data._add_player_tracking_data_to_dict import (
+    _add_player_tracking_data_to_dict,
+)
+from databallpy.load_data.tracking_data._get_matchtime import _get_matchtime
+from databallpy.load_data.tracking_data._insert_missing_rows import _insert_missing_rows
+from databallpy.load_data.tracking_data._normalize_playing_direction_tracking import (
+    _normalize_playing_direction_tracking,
+)
+from databallpy.utils.tz_modification import utc_to_local_datetime
+from databallpy.utils.utils import MISSING_INT, _to_float, _to_int
 
-EVENT_TYPE_IDS = {
-    1: "pass",
-    2: "offside pass",
-    3: "take on",
-    4: "foul",
-    5: "out",
-    6: "corner awarded",
-    7: "tackle",
-    8: "interception",
-    9: "turnover",
-    10: "save",
-    11: "claim",
-    12: "clearance",
-    13: "miss",
-    14: "post",
-    15: "attempt saved",
-    16: "goal",
-    17: "card",
-    18: "player off",
-    19: "player on",
-    20: "player retired",
-    21: "player returns",
-    22: "player becomes goalkeeper",
-    23: "goalkeeper becomes player",
-    24: "condition change",
-    25: "official change",
-    27: "start delay",
-    28: "end delay",
-    29: "unknown event 29",
-    30: "end",
-    31: "unknown event 31",
-    32: "start",
-    33: "unknown event 33",
-    34: "team set up",
-    35: "player changed position",
-    36: "player changed jersey number",
-    37: "collection end",
-    38: "temp_goal",
-    39: "temp_attempt",
-    40: "formation change",
-    41: "punch",
-    42: "good skill",
-    43: "deleted event",
-    44: "aerial",
-    45: "challenge",
-    46: "unknown event 46",
-    47: "rescinded card",
-    48: "unknown event 46",
-    49: "ball recovery",
-    50: "dispossessed",
-    51: "error",
-    52: "keeper pick-up",
-    53: "cross not claimed",
-    54: "smother",
-    55: "offside provoked",
-    56: "shield ball opp",
-    57: "foul throw in",
-    58: "penalty faced",
-    59: "keeper sweeper",
-    60: "chance missed",
-    61: "ball touch",
-    62: "unknown event 62",
-    63: "temp_save",
-    64: "resume",
-    65: "contentious referee decision",
-    66: "possession data",
-    67: "50/50",
-    68: "referee drop ball",
-    69: "failed to block",
-    70: "injury time announcement",
-    71: "coach setup",
-    72: "caught offside",
-    73: "other ball contact",
-    74: "blocked pass",
-    75: "delayed start",
-    76: "early end",
-    77: "player off pitch",
-}
 
-
-def load_opta_event_data(
-    f7_loc: str, f24_loc: str, pitch_dimensions: list = [106.0, 68.0]
+def load_inmotio_tracking_data(
+    tracking_data_loc: str, metadata_loc: str, verbose: bool = True
 ) -> Tuple[pd.DataFrame, Metadata]:
-    """This function retrieves the metadata and event data of a specific match. The x
-    and y coordinates provided have been scaled to the dimensions of the pitch, with
-    (0, 0) being the center. Additionally, the coordinates have been standardized so
-    that the home team is represented as playing from left to right for the entire
-    match, and the away team is represented as playing from right to left.
+    """Function to load inmotio tracking data.
 
     Args:
-        f7_loc (str): location of the f7.xml file.
-        f24_loc (str): location of the f24.xml file.
-        pitch_dimensions (list, optional): the length and width of the pitch in meters
+        tracking_data_loc (str): location of the tracking data .txt file
+        metadata_loc (str): location of the metadata .xml file
+        verbose (bool, optional): whether to print information about the progress
+        in the terminall. Defaults to True.
+
+    Raises:
+        TypeError: if tracking_data_loc is not a string
 
     Returns:
-        Tuple[pd.DataFrame, Metadata]: the event data of the match and the metadata
+        Tuple[pd.DataFrame, Metadata]: tracking and metadata of the match
     """
+    if isinstance(tracking_data_loc, str):
+        assert os.path.exists(tracking_data_loc)
+        assert os.path.exists(metadata_loc)
+    else:
+        raise TypeError(
+            f"tracking_data_loc must be  a str, not a {type(tracking_data_loc)}"
+        )
 
-    assert isinstance(f7_loc, str), f"f7_loc should be a string, not a {type(f7_loc)}"
-    assert isinstance(
-        f24_loc, str
-    ), f"f24_loc should be a string, not a {type(f24_loc)}"
-    assert f7_loc[-4:] == ".xml", "f7 opta file should by of .xml format"
-    assert f24_loc[-4:] == ".xml", "f24 opta file should be of .xml format"
-
-    event_data = _load_event_data(f24_loc)
-    metadata = _load_metadata(f7_loc, pitch_dimensions=pitch_dimensions)
-
-    # Add player names to the event data dataframe
-    home_players = dict(
-        zip(metadata.home_players["id"], metadata.home_players["full_name"])
+    metadata = _get_metadata(metadata_loc)
+    td_channels = _get_td_channels(metadata_loc, metadata)
+    tracking_data = _get_tracking_data(
+        tracking_data_loc, td_channels, metadata.pitch_dimensions, verbose
     )
-    away_players = dict(
-        zip(metadata.away_players["id"], metadata.away_players["full_name"])
+    first_frame = metadata.periods_frames[metadata.periods_frames["start_frame"] > 0][
+        "start_frame"
+    ].min()
+    last_frame = metadata.periods_frames["end_frame"].max()
+    tracking_data = tracking_data[
+        (tracking_data["frame"] >= first_frame) & (tracking_data["frame"] <= last_frame)
+    ].reset_index(drop=True)
+    tracking_data = _normalize_playing_direction_tracking(
+        tracking_data, metadata.periods_frames
     )
-
-    home_mask = (event_data["team_id"] == metadata.home_team_id) & ~pd.isnull(
-        event_data["player_id"]
+    tracking_data["period"] = _add_periods_to_tracking_data(
+        tracking_data["frame"], metadata.periods_frames
     )
-    away_mask = (event_data["team_id"] == metadata.away_team_id) & ~pd.isnull(
-        event_data["player_id"]
+    tracking_data["matchtime_td"] = _get_matchtime(
+        tracking_data["frame"], tracking_data["period"], metadata
     )
 
-    event_data.loc[home_mask, "player_name"] = event_data.loc[
-        home_mask, "player_id"
-    ].map(home_players)
-    event_data.loc[away_mask, "player_name"] = event_data.loc[
-        away_mask, "player_id"
-    ].map(away_players)
-
-    # Rescale the x and y coordinates relative to the pitch dimensions
-    # The original dimension of the x and y coordinates range from 0 to 100
-    event_data.loc[:, ["start_x"]] = (
-        event_data.loc[:, ["start_x"]] / 100 * pitch_dimensions[0]
-    ) - (pitch_dimensions[0] / 2.0)
-    event_data.loc[:, ["start_y"]] = (
-        event_data.loc[:, ["start_y"]] / 100 * pitch_dimensions[1]
-    ) - (pitch_dimensions[1] / 2.0)
-
-    # Change direction of play of the away team so it is represented from right to left
-    event_data.loc[
-        event_data["team_id"] == metadata.away_team_id, ["start_x", "start_y"]
-    ] *= -1
-
-    return event_data, metadata
+    return tracking_data, metadata
 
 
-def _load_metadata(f7_loc: str, pitch_dimensions: list) -> Metadata:
-    """Function to load metadata from the f7.xml opta file
+def _get_tracking_data(
+    tracking_data_loc: str,
+    td_channels: list,
+    pitch_dimensions: list,
+    verbose: bool = True,
+) -> pd.DataFrame:
+    """Function to load in inmotio format tracking_data
 
     Args:
-        f7_loc (str): location of the f7.xml opta file
-        pitch_dimensions (list): the length and width of the pitch in meters
+        tracking_data_loc (str): location of the tracking .txt file
+        td_channels (list): the order of which players are referred
+        to in the raw tracking data
+        pitch_dimensions (list): x and y dimensions of the pitch in meters
+        verbose (bool, optional): whether to print information about the progress in the
+        terminal. Defaults to True.
 
     Returns:
-        MetaData: all metadata information of the current match
+        pd.DataFrame: tracking data of the match in a pd dataframe
     """
-    file = open(f7_loc, "r")
-    lines = file.read()
-    soup = BeautifulSoup(lines, "xml")
-
-    # Obtain match id
-    match_id = int(soup.find("SoccerDocument").attrs["uID"][1:])
+    if verbose:
+        print(f"Reading in {tracking_data_loc}", end="")
+    file = open(tracking_data_loc, "r")
+    lines = file.readlines()
+    if verbose:
+        print(" - Completed")
+    file.close()
 
-    # Obtain match start and end of period datetime
-    periods = {
-        "period": [1, 2, 3, 4, 5],
-        "start_datetime_opta": [],
-        "end_datetime_opta": [],
+    size_lines = len(lines)
+    data = {
+        "frame": [np.nan] * size_lines,
+        "ball_x": [np.nan] * size_lines,
+        "ball_y": [np.nan] * size_lines,
+        "ball_z": [np.nan] * size_lines,
+        "ball_status": [None] * size_lines,
+        "ball_posession": [None] * size_lines,
     }
-    start_period_1 = soup.find("Stat", attrs={"Type": "first_half_start"})
-    end_period_1 = soup.find("Stat", attrs={"Type": "first_half_stop"})
-    start_period_2 = soup.find("Stat", attrs={"Type": "second_half_start"})
-    end_period_2 = soup.find("Stat", attrs={"Type": "second_half_stop"})
-    for start, end in zip(
-        [start_period_1, start_period_2], [end_period_1, end_period_2]
-    ):
-        # Add one hour to go from utc to Dutch time
-        periods["start_datetime_opta"].append(
-            pd.to_datetime(start.contents[0]).tz_localize(None) + dt.timedelta(hours=1)
-        )
-        periods["end_datetime_opta"].append(
-            pd.to_datetime(end.contents[0]).tz_localize(None) + dt.timedelta(hours=1)
+
+    if verbose:
+        print("Writing lines to dataframe:")
+        lines = tqdm(lines)
+
+    for idx, line in enumerate(lines):
+
+        frame, players_home, players_away, ball_info = line.split(":")
+        frame = _to_int(frame)
+        data["frame"][idx] = frame
+        players_info = players_home + ";" + players_away
+        players = players_info.split(";")
+        for i, player in enumerate(players):
+            y, x = player.split(",")
+            team = td_channels[i].split("_")[0]
+            shirt_num = td_channels[i].split("_")[1]
+            data = _add_player_tracking_data_to_dict(
+                team, shirt_num, _to_float(x), _to_float(y), data, idx
+            )
+
+        y, x, z, _, ball_status = ball_info.replace("\n", "").split(",")
+        data = _add_ball_data_to_dict(
+            _to_float(x), _to_float(y), _to_float(z), None, ball_status, data, idx
         )
-    for _ in range(3):
-        periods["start_datetime_opta"].append(pd.to_datetime("NaT"))
-        periods["end_datetime_opta"].append(pd.to_datetime("NaT"))
-
-    # Opta has a TeamData and Team attribute in the f7 file
-    team_datas = soup.find_all("TeamData")
-    teams = soup.find_all("Team")
-    teams_info = {}
-    teams_player_info = {}
-    for team_data, team in zip(team_datas, teams):
-
-        # Team information
-        team_name = team.findChildren("Name")[0].contents[0]
-        team_info = {}
-        team_info["team_name"] = team_name
-        team_info["side"] = team_data["Side"].lower()
-        team_info["formation"] = team_data["Formation"]
-        team_info["score"] = int(team_data["Score"])
-        team_info["team_id"] = int(team_data["TeamRef"][1:])
-        teams_info[team_info["side"]] = team_info
-
-        # Player information
-        players_data = [
-            player.attrs for player in team_data.findChildren("MatchPlayer")
-        ]
-        players_names = {}
-        for player in team.findChildren("Player"):
-            player_id = int(player.attrs["uID"][1:])
-            first_name = player.contents[1].contents[1].text
-
-            if "Last" in str(player.contents[1].contents[3]):
-                last_name_idx = 3
-            else:
-                last_name_idx = 5
-            last_name = player.contents[1].contents[last_name_idx].contents[0]
-            if first_name:
-                players_names[str(player_id)] = f"{first_name} {last_name}"
-            else:
-                players_names[str(player_id)] = last_name
 
-        player_info = _get_player_info(players_data, players_names)
-        teams_player_info[team_info["side"]] = player_info
+    df = pd.DataFrame(data)
+    df["ball_status"] = ["alive" if x == "1" else "dead" for x in df["ball_status"]]
+    for col in [x for x in df.columns if "_x" in x]:
+        df[col] = df[col] - (pitch_dimensions[0] / 2)
+        df[col] *= -1
 
-    file.close()
+    for col in [x for x in df.columns if "_y" in x]:
+        df[col] = df[col] - (pitch_dimensions[1] / 2)
 
-    metadata = Metadata(
-        match_id=match_id,
-        pitch_dimensions=pitch_dimensions,
-        periods_frames=pd.DataFrame(periods),
-        frame_rate=np.nan,
-        home_team_id=teams_info["home"]["team_id"],
-        home_team_name=str(teams_info["home"]["team_name"]),
-        home_players=teams_player_info["home"],
-        home_score=teams_info["home"]["score"],
-        home_formation=teams_info["home"]["formation"],
-        away_team_id=teams_info["away"]["team_id"],
-        away_team_name=str(teams_info["away"]["team_name"]),
-        away_players=teams_player_info["away"],
-        away_score=teams_info["away"]["score"],
-        away_formation=teams_info["away"]["formation"],
-    )
-    return metadata
+    df = _insert_missing_rows(df, "frame")
+
+    return df
 
 
-def _get_player_info(players_data: list, players_names: dict) -> pd.DataFrame:
-    """Function to loop over all players and save data in a pd.DataFrame
+def _get_td_channels(metadata_loc: str, metadata: Metadata) -> list:
+    """Function to get the channels the order of which players
+    are referred to in the raw tracking data
 
     Args:
-        players_data (list): for every player a dictionary with info about the player
-        except the player name
-        players_names (dict): dictionary with player id as key and the player name as
-        value
+        metadata_loc (str): location of the metadata
+        metadata (Metadata): the Metadata of the match
 
     Returns:
-        pd.DataFrame: all information of the players
+        list: List with the order of which players are referred to
+        in the raw tracking data
     """
-    result_dict = {
-        "id": [],
-        "full_name": [],
-        "formation_place": [],
-        "position": [],
-        "starter": [],
-        "shirt_num": [],
-    }
+    file = open(metadata_loc, "r", encoding="UTF-8")
+    lines = file.read()
+    soup = BeautifulSoup(lines, "xml")
+    file.close()
 
-    for player in players_data:
-        player_id = int(player["PlayerRef"][1:])
-        result_dict["id"].append(player_id)
-        result_dict["full_name"].append(players_names[str(player_id)])
-        result_dict["formation_place"].append(int(player["Formation_Place"]))
-        position = (
-            player["Position"]
-            if player["Position"] != "Substitute"
-            else player["SubPosition"]
-        )
-        result_dict["position"].append(position.lower())
-        result_dict["starter"].append(player["Status"] == "Start")
-        result_dict["shirt_num"].append(int(player["ShirtNumber"]))
+    res = []
+    for channel in soup.find_all("PlayerChannel"):
+        player_id = int(channel.attrs["id"].split("_")[0][2:])
+        value = channel.attrs["id"].split("_")[1]
+        if "y" in value:
+            continue
+        home_mask = metadata.home_players["id"] == player_id
+        away_mask = metadata.away_players["id"] == player_id
+        if home_mask.any():
+            team = "home"
+            shirt_num = metadata.home_players.loc[home_mask, "shirt_num"].values[0]
+        else:
+            team = "away"
+            shirt_num = metadata.away_players.loc[away_mask, "shirt_num"].values[0]
+        res.append(f"{team}_{shirt_num}")
 
-    return pd.DataFrame(result_dict)
+    return res
 
 
-def _load_event_data(f24_loc: str) -> pd.DataFrame:
-    """Function to load the f27 .xml, the events of the match.
-    Note: this function does ignore qualifiers for now
+def _get_metadata(metadata_loc: str) -> Metadata:
+    """Function to get the metadata of the match
 
     Args:
-        f24_loc (str): location of the f24.xml file
+        metadata_loc (str): Location of the metadata .xml file
 
     Returns:
-        pd.DataFrame: all events of the match in a pd dataframe
+        Metadata: all information of the match
     """
 
-    file = open(f24_loc, "r")
+    file = open(metadata_loc, "r", encoding="UTF-8")
     lines = file.read()
     soup = BeautifulSoup(lines, "xml")
+    file.close()
 
-    result_dict = {
-        "event_id": [],
-        "type_id": [],
-        "event": [],
-        "period_id": [],
-        "minutes": [],
-        "seconds": [],
-        "player_id": [],
-        "team_id": [],
-        "outcome": [],
-        "start_x": [],
-        "start_y": [],
-        "datetime": [],
+    periods_dict = {
+        "period": [1, 2, 3, 4, 5],
+        "start_frame": [MISSING_INT] * 5,
+        "end_frame": [MISSING_INT] * 5,
+        "start_datetime_td": [pd.to_datetime("NaT")] * 5,
+        "end_datetime_td": [pd.to_datetime("NaT")] * 5,
     }
+    periods = soup.find_all("Session")
 
-    events = soup.find_all("Event")
-    for event in events:
-        result_dict["event_id"].append(int(event.attrs["id"]))
-        event_type_id = int(event.attrs["type_id"])
-        result_dict["type_id"].append(event_type_id)
+    i = 0
+    for period in periods:
+        if period.SessionType.text == "Period":
+            values = [int(x.text) for x in period.find_all("Value")]
+            periods_dict["start_frame"][i] = _to_int(values[0])
+            periods_dict["end_frame"][i] = _to_int(values[1])
+            periods_dict["start_datetime_td"][i] = pd.to_datetime(
+                period.find("Start").text, utc=True
+            )
+            periods_dict["end_datetime_td"][i] = pd.to_datetime(
+                period.find("End").text, utc=True
+            )
+            i += 1
+    periods_frames = pd.DataFrame(periods_dict)
+
+    competition = soup.find("Competition").text.split(",")[0]
+
+    # set to the right timezone
+    periods_frames["start_datetime_td"] = utc_to_local_datetime(
+        periods_frames["start_datetime_td"], competition
+    )
+    periods_frames["end_datetime_td"] = utc_to_local_datetime(
+        periods_frames["end_datetime_td"], competition
+    )
 
-        if event_type_id in EVENT_TYPE_IDS.keys():
-            event_name = EVENT_TYPE_IDS[event_type_id].lower()
-        else:
-            # Unknown event
-            event_name = None
+    home_team = soup.Teams.find_all("Team")[0]
+    home_team_id = home_team.attrs["id"]
+    home_team_name = home_team.Name.text
+    home_team_player_data = soup.find_all("Player", {"teamId": home_team_id})
+    home_players = _get_player_data(home_team_player_data)
+    home_score = int(soup.LocalTeamScore.text)
+
+    away_team = soup.Teams.find_all("Team")[1]
+    away_team_id = away_team.attrs["id"]
+    away_team_name = away_team.Name.text
+    away_team_player_data = soup.find_all("Player", {"teamId": away_team_id})
+    away_players = _get_player_data(away_team_player_data)
+    away_score = int(soup.VisitingTeamScore.text)
+
+    metadata = Metadata(
+        match_id=int(soup.Session.attrs["id"]),
+        pitch_dimensions=[
+            float(soup.MatchParameters.FieldSize.Length.text),
+            float(soup.MatchParameters.FieldSize.Width.text),
+        ],
+        periods_frames=periods_frames,
+        frame_rate=int(soup.FrameRate.text),
+        home_team_id=home_team_id,
+        home_team_name=home_team_name,
+        home_players=home_players,
+        home_score=home_score,
+        home_formation="",
+        away_team_id=away_team_id,
+        away_team_name=away_team_name,
+        away_players=away_players,
+        away_score=away_score,
+        away_formation="",
+        country="",
+    )
+    return metadata
 
-        result_dict["event"].append(event_name)
-        result_dict["period_id"].append(int(event.attrs["period_id"]))
-        result_dict["minutes"].append(int(event.attrs["min"]))
-        result_dict["seconds"].append(int(event.attrs["sec"]))
 
-        if "player_id" in event.attrs.keys():
-            result_dict["player_id"].append(int(event.attrs["player_id"]))
-        else:
-            result_dict["player_id"].append(np.nan)
+def _get_player_data(team: bs4.element.Tag) -> pd.DataFrame:
+    """Function that creates a df containing info on all players for a team
+    Args:
+        team (bs4.element.Tag): containing info no all players of a team
+    Returns:
+        pd.DataFrame: contains all player information for a team
+    """
 
-        result_dict["team_id"].append(int(event.attrs["team_id"]))
-        result_dict["outcome"].append(int(event.attrs["outcome"]))
-        result_dict["start_x"].append(float(event.attrs["x"]))
-        result_dict["start_y"].append(float(event.attrs["y"]))
-        result_dict["datetime"].append(
-            pd.to_datetime(event.attrs["timestamp"]) + dt.timedelta(hours=1)
-        )
+    player_dict = {
+        "id": [],
+        "full_name": [],
+        "shirt_num": [],
+        "player_type": [],
+        "start_frame": [],
+        "end_frame": [],
+    }
+    for player in team:
+        player_dict["id"].append(int(player["id"][2:]))
+        player_dict["full_name"].append(player.Name.text)
+        player_dict["shirt_num"].append(int(player.ShirtNumber.text))
+        values = [x.text for x in player.find_all("Value")]
+        player_dict["player_type"].append(values[0])
+        player_dict["start_frame"].append(int(values[1]))
+        player_dict["end_frame"].append(int(values[2]))
+    df = pd.DataFrame(player_dict)
 
-    file.close()
-    return pd.DataFrame(result_dict)
+    return df
```

### Comparing `databallpy-0.2.3/databallpy/load_data/metadata.py` & `databallpy-0.3.0/databallpy/load_data/metadata.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from dataclasses import dataclass
 
+import numpy as np
 import pandas as pd
 
 
 @dataclass
 class Metadata:
     match_id: int
     pitch_dimensions: list
@@ -18,14 +19,16 @@
 
     away_team_id: int
     away_team_name: str
     away_players: pd.DataFrame
     away_score: int
     away_formation: str
 
+    country: str
+
     def __post_init__(self):
         # match id
         if not isinstance(self.match_id, int):
             raise TypeError(
                 f"match_id ({self.match_id}) should be an integer, not \
                     {type(self.match_id)}"
             )
@@ -63,14 +66,21 @@
         ) or not all(self.periods_frames["period"].value_counts() == 1):
 
             res = self.periods_frames["period"]
             raise ValueError(
                 f"'period' column in period_frames should contain only the values \
                     [1, 2, 3, 4, 5]. Now it's {res}"
             )
+        for col in [col for col in self.periods_frames if "datetime" in col]:
+            if pd.isnull(self.periods_frames[col]).all():
+                continue
+            if self.periods_frames[col].dt.tz is None:
+                raise ValueError(
+                    f"{col} column in period_frames should have a timezone"
+                )
 
         # frame_rate
         if not pd.isnull(self.frame_rate):
             if not isinstance(self.frame_rate, int):
                 raise TypeError(
                     f"frame_rate should be an integer, not a {type(self.frame_rate)}"
                 )
@@ -115,17 +125,17 @@
             ["home", "away"], [self.home_formation, self.away_formation]
         ):
             if not pd.isnull(form):
                 if not isinstance(form, str):
                     raise TypeError(
                         f"{team} team formation should be a string, not a {type(form)}"
                     )
-                if len(form) > 4:
+                if len(form) > 5:
                     raise ValueError(
-                        f"{team} team formation should be of length 4 or smaller, not \
+                        f"{team} team formation should be of length 5 or smaller, not \
                             {len(form)}"
                     )
 
         # team players
         for team, players in zip(
             ["home", "away"], [self.home_players, self.away_players]
         ):
@@ -138,41 +148,51 @@
                 [x in players.columns for x in ["id", "full_name", "shirt_num"]]
             ):
                 raise ValueError(
                     f"{team} team players should contain at least the column \
                         ['id', 'full_name', 'shirt_num'], now its {players.columns}"
                 )
 
-    def __eq__(self, other):
-        result = [
-            self.match_id == other.match_id,
-            all(
-                [s == o for s, o in zip(self.pitch_dimensions, other.pitch_dimensions)]
-            ),
-            self.periods_frames.equals(other.periods_frames),
-            self.frame_rate == other.frame_rate
-            if not pd.isnull(self.frame_rate)
-            else pd.isnull(other.frame_rate),
-            self.home_team_id == other.home_team_id,
-            self.home_team_name == other.home_team_name,
-            self.home_players.equals(other.home_players),
-            self.home_score == other.home_score
-            if not pd.isnull(self.home_score)
-            else pd.isnull(other.home_score),
-            self.home_formation == other.home_formation,
-            self.away_team_id == other.away_team_id,
-            self.away_team_name == other.away_team_name,
-            self.away_players.equals(other.away_players),
-            self.away_score == other.away_score
-            if not pd.isnull(self.away_score)
-            else pd.isnull(other.away_score),
-            self.away_formation == other.away_formation,
-        ]
+        # country
+        if not isinstance(self.country, str):
+            raise TypeError(f"country should be a string, not a {type(self.country)}")
 
-        return all(result)
+    def __eq__(self, other):
+        if isinstance(other, Metadata):
+            result = [
+                self.match_id == other.match_id,
+                all(
+                    [
+                        s == o if not np.isnan(s) else np.isnan(o)
+                        for s, o in zip(self.pitch_dimensions, other.pitch_dimensions)
+                    ]
+                ),
+                self.periods_frames.equals(other.periods_frames),
+                self.frame_rate == other.frame_rate
+                if not pd.isnull(self.frame_rate)
+                else pd.isnull(other.frame_rate),
+                self.home_team_id == other.home_team_id,
+                self.home_team_name == other.home_team_name,
+                self.home_players.equals(other.home_players),
+                self.home_score == other.home_score
+                if not pd.isnull(self.home_score)
+                else pd.isnull(other.home_score),
+                self.home_formation == other.home_formation,
+                self.away_team_id == other.away_team_id,
+                self.away_team_name == other.away_team_name,
+                self.away_players.equals(other.away_players),
+                self.away_score == other.away_score
+                if not pd.isnull(self.away_score)
+                else pd.isnull(other.away_score),
+                self.away_formation == other.away_formation,
+                self.country == other.country,
+            ]
+            return all(result)
+        else:
+            return False
 
     def copy(self):
         return Metadata(
             match_id=self.match_id,
             pitch_dimensions=list(self.pitch_dimensions),
             periods_frames=self.periods_frames.copy(),
             frame_rate=self.frame_rate,
@@ -182,8 +202,9 @@
             home_score=self.home_score,
             home_formation=self.home_formation,
             away_team_id=self.away_team_id,
             away_team_name=self.away_team_name,
             away_players=self.away_players.copy(),
             away_score=self.away_score,
             away_formation=self.away_formation,
+            country=self.country,
         )
```

### Comparing `databallpy-0.2.3/databallpy/load_data/metrica_metadata.py` & `databallpy-0.3.0/databallpy/load_data/metrica_metadata.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,76 +2,81 @@
 import os
 
 import numpy as np
 import pandas as pd
 from bs4 import BeautifulSoup
 
 from databallpy.load_data.metadata import Metadata
-from databallpy.utils import _to_float, _to_int
+from databallpy.utils.utils import MISSING_INT, _to_float, _to_int
 
 
 def _get_td_channels(metadata_loc: str, metadata: Metadata) -> pd.DataFrame:
     """Function to get the channels for every timeperiod with what players are
     referred to in the raw tracking data
 
     Args:
         metadata_loc (str): locatin of the metadata
         metadata (Metadata): the Metadata of the match
 
     Returns:
-        pd.DataFrame: df with for every timestamp what players are referred to in
+        pd.DataFrame: df with for every frame what players are referred to in
         the raw tracking data
     """
     if os.path.exists(metadata_loc):
         file = open(metadata_loc, "r")
         lines = file.read()
         file.close()
         soup = BeautifulSoup(lines, "xml")
     else:
         soup = BeautifulSoup(metadata_loc.strip(), "xml")
 
+    channel_id_to_player_id_dict = {}
+    for player in soup.find_all("PlayerChannel"):
+        channel_id = player.attrs["id"].split("_")[0]
+        value = player.attrs["id"].split("_")[1]
+        if "y" in value:
+            continue
+        channel_id_to_player_id_dict[channel_id] = int(player.attrs["playerId"][1:])
+
     res = {"start": [], "end": [], "ids": []}
     for idx, data_format_specification in enumerate(
         soup.find_all("DataFormatSpecification")
     ):
         res["ids"].append([])
         res["start"].append(int(data_format_specification.attrs["startFrame"]))
         res["end"].append(int(data_format_specification.attrs["endFrame"]))
         for channel in data_format_specification.findChildren("PlayerChannelRef"):
-            full_name = channel.attrs["playerChannelId"].split("_")[0]
+            channel_id = channel.attrs["playerChannelId"].split("_")[0]
             value = channel.attrs["playerChannelId"].split("_")[1]
             if "y" in value:
                 continue
-            home_mask = (
-                metadata.home_players["full_name"]
-                .str.lower()
-                .str.replace(" ", "")
-                .isin([full_name])
-            )
-            away_mask = (
-                metadata.away_players["full_name"]
-                .str.lower()
-                .str.replace(" ", "")
-                .isin([full_name])
-            )
+            player_id = channel_id_to_player_id_dict[channel_id]
+            home_mask = metadata.home_players["id"] == player_id
+            away_mask = metadata.away_players["id"] == player_id
             if home_mask.any():
                 team = "home"
-                shirt_num = metadata.home_players.loc[home_mask, "shirt_num"].iloc[0]
+                shirt_num = metadata.home_players.loc[home_mask, "shirt_num"].values[0]
             else:
                 team = "away"
-                shirt_num = metadata.away_players.loc[away_mask, "shirt_num"].iloc[0]
+                shirt_num = metadata.away_players.loc[away_mask, "shirt_num"].values[0]
             res["ids"][idx].append(f"{team}_{shirt_num}")
     return pd.DataFrame(res)
 
 
-def _get_metadata(metadata_loc: str) -> Metadata:
+def _get_metadata(
+    metadata_loc: str, is_tracking_data: bool = True, is_event_data: bool = False
+) -> Metadata:
     """Function to get the metadata of the match
 
     Args:
         metadata_loc (str): Location of the metadata .xml file
+        is_tracking_data (bool, optional): Whether the metadata is from the tracking
+        data. Defaults to True.
+        is_event_data (bool, optional): Whether the metadata is from the event data.
+        Defaults to False
 
     Returns:
         Metadata: all information of the match
     """
     if os.path.exists(metadata_loc):
         file = open(metadata_loc, "r")
         lines = file.read()
@@ -80,23 +85,29 @@
     else:
         soup = BeautifulSoup(metadata_loc.strip(), "xml")
 
     match_id = _to_int(soup.find("Session").attrs["id"])
     pitch_size_x = _to_float(soup.find("FieldSize").find("Width").text)
     pitch_size_y = _to_float(soup.find("FieldSize").find("Height").text)
     frame_rate = _to_int(soup.find("FrameRate").text)
-    datetime = pd.to_datetime(soup.find("Start").text).tz_localize(None)
+
+    # no idea about time zone, so just assume utc
+    datetime = pd.to_datetime(soup.find("Start").text, utc=True)
 
     periods_dict = {
         "period": [],
         "start_frame": [],
         "end_frame": [],
-        "start_time_td": [],
-        "end_time_td": [],
     }
+    if is_tracking_data:
+        periods_dict["start_datetime_td"] = []
+        periods_dict["end_datetime_td"] = []
+    if is_event_data:
+        periods_dict["start_datetime_ed"] = []
+        periods_dict["end_datetime_ed"] = []
 
     periods_map = {
         "first_half_start": 1,
         "first_half_end": 1,
         "second_half_start": 2,
         "second_half_end": 2,
         "first_extra_half_start": 3,
@@ -107,45 +118,70 @@
 
     for period_soup in soup.find("ProviderGlobalParameters").find_all(
         "ProviderParameter"
     ):
         name = period_soup.find("Name").text
         period = periods_map[name]
 
-        current_timestamp = _to_int(period_soup.find("Value").text)
+        current_frame = _to_int(period_soup.find("Value").text)
 
         if "start" in name:
             periods_dict["period"].append(period)
-            periods_dict["start_frame"].append(current_timestamp)
-            first_timestamp = periods_dict["start_frame"][0]
-            seconds = (current_timestamp - first_timestamp) / frame_rate
-            periods_dict["start_time_td"].append(
-                datetime + dt.timedelta(milliseconds=seconds * 1000)
-            ) if not current_timestamp == -999 else periods_dict[
-                "start_time_td"
-            ].append(
-                pd.to_datetime("NaT")
-            )
+            periods_dict["start_frame"].append(current_frame)
+            first_frame = periods_dict["start_frame"][0]
+            if is_tracking_data:
+                seconds = (current_frame - first_frame) / frame_rate
+                periods_dict["start_datetime_td"].append(
+                    datetime + dt.timedelta(milliseconds=seconds * 1000)
+                ) if not current_frame == MISSING_INT else periods_dict[
+                    "start_datetime_td"
+                ].append(
+                    pd.to_datetime("NaT")
+                )
+            if is_event_data:
+                seconds = (current_frame - first_frame) / frame_rate
+                periods_dict["start_datetime_ed"].append(
+                    datetime + dt.timedelta(milliseconds=seconds * 1000)
+                ) if not current_frame == MISSING_INT else periods_dict[
+                    "start_datetime_ed"
+                ].append(
+                    pd.to_datetime("NaT")
+                )
 
         elif "end" in name:
-            periods_dict["end_frame"].append(current_timestamp)
-            first_timestamp = periods_dict["start_frame"][0]
-            seconds = (current_timestamp - first_timestamp) / frame_rate
-            periods_dict["end_time_td"].append(
-                datetime + dt.timedelta(milliseconds=seconds * 1000)
-            ) if not current_timestamp == -999 else periods_dict["end_time_td"].append(
-                pd.to_datetime("NaT")
-            )
+            periods_dict["end_frame"].append(current_frame)
+            first_frame = periods_dict["start_frame"][0]
+            seconds = (current_frame - first_frame) / frame_rate
+            if is_tracking_data:
+                periods_dict["end_datetime_td"].append(
+                    datetime + dt.timedelta(milliseconds=seconds * 1000)
+                ) if not current_frame == MISSING_INT else periods_dict[
+                    "end_datetime_td"
+                ].append(
+                    pd.to_datetime("NaT")
+                )
+            if is_event_data:
+                periods_dict["end_datetime_ed"].append(
+                    datetime + dt.timedelta(milliseconds=seconds * 1000)
+                ) if not current_frame == MISSING_INT else periods_dict[
+                    "end_datetime_ed"
+                ].append(
+                    pd.to_datetime("NaT")
+                )
 
     # add fifth period
     periods_dict["period"].append(5)
-    periods_dict["start_frame"].append(-999)
-    periods_dict["end_frame"].append(-999)
-    periods_dict["start_time_td"].append(pd.to_datetime("NaT"))
-    periods_dict["end_time_td"].append(pd.to_datetime("NaT"))
+    periods_dict["start_frame"].append(MISSING_INT)
+    periods_dict["end_frame"].append(MISSING_INT)
+    if is_tracking_data:
+        periods_dict["start_datetime_td"].append(pd.to_datetime("NaT"))
+        periods_dict["end_datetime_td"].append(pd.to_datetime("NaT"))
+    if is_event_data:
+        periods_dict["start_datetime_ed"].append(pd.to_datetime("NaT"))
+        periods_dict["end_datetime_ed"].append(pd.to_datetime("NaT"))
 
     teams_info = {}
     for team in soup.find_all("Team"):
         team_info = {}
         team_info["team_name"] = team.find("Name").text
         team_info["team_id"] = team.attrs["id"]
         team_info["formation"] = ""
@@ -216,14 +252,15 @@
         home_score=teams_info["home"]["score"],
         home_formation=teams_info["home"]["formation"],
         away_team_id=teams_info["away"]["team_id"],
         away_team_name=teams_info["away"]["team_name"],
         away_players=pd.DataFrame(away_players),
         away_score=teams_info["away"]["score"],
         away_formation=teams_info["away"]["formation"],
+        country="",
     )
     return metadata
 
 
 def _update_metadata(td_channels: pd.DataFrame, metadata: Metadata) -> Metadata:
     """Function to add the starters and formation based on the metadata and tracking
     data channels to the metadata
```

### Comparing `databallpy-0.2.3/databallpy/load_data/tracking_data/_add_ball_data_to_dict.py` & `databallpy-0.3.0/databallpy/load_data/tracking_data/_add_ball_data_to_dict.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from databallpy.utils.utils import _to_float
+
+
 def _add_ball_data_to_dict(
     ball_x: str,
     ball_y: str,
     ball_z: str,
     posession: str,
     status: str,
     data: dict,
@@ -14,14 +17,14 @@
         data (dict): data dictionary to write results to
         idx (int): indicates position in data dictionary
 
     Returns:
         dict: contains all tracking data
     """
 
-    data["ball_x"][idx] = float(ball_x)
-    data["ball_y"][idx] = float(ball_y)
-    data["ball_z"][idx] = float(ball_z)
+    data["ball_x"][idx] = _to_float(ball_x)
+    data["ball_y"][idx] = _to_float(ball_y)
+    data["ball_z"][idx] = _to_float(ball_z)
     data["ball_posession"][idx] = posession
     data["ball_status"][idx] = status
 
     return data
```

### Comparing `databallpy-0.2.3/databallpy/load_data/tracking_data/_add_periods_to_tracking_data.py` & `databallpy-0.3.0/databallpy/load_data/tracking_data/_add_periods_to_tracking_data.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import numpy as np
 import pandas as pd
 
+from databallpy.utils.utils import MISSING_INT
+
 
 def _add_periods_to_tracking_data(
     timestamps: pd.Series, periods_frames: pd.DataFrame
 ) -> pd.Series:
     """Function to add periods
 
     Args:
@@ -30,18 +32,18 @@
         & (timestamps < periods_frames.loc[3, "end_frame"]),
         (timestamps > periods_frames.loc[3, "end_frame"])
         & (timestamps < periods_frames.loc[4, "start_frame"]),
         (timestamps > periods_frames.loc[4, "start_frame"]),
     ]
     period_values = [
         1,
-        -999,
+        MISSING_INT,
         2,
-        -999,
+        MISSING_INT,
         3,
-        -999,
+        MISSING_INT,
         4,
-        -999,
+        MISSING_INT,
         5,
     ]
 
     return np.select(period_conditions, period_values).astype("int64")
```

### Comparing `databallpy-0.2.3/databallpy/load_data/tracking_data/_add_player_tracking_data_to_dict.py` & `databallpy-0.3.0/databallpy/load_data/tracking_data/_add_player_tracking_data_to_dict.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,14 @@
         idx (int): indicates position in data dictionary
 
     Returns:
         dict: contains all tracking data
     """
 
     if f"{team}_{shirt_num}_x" not in data.keys():  # create keys for new player
-        data[f"{team}_{shirt_num}_x"] = [np.nan] * len(data["timestamp"])
-        data[f"{team}_{shirt_num}_y"] = [np.nan] * len(data["timestamp"])
+        data[f"{team}_{shirt_num}_x"] = [np.nan] * len(data["frame"])
+        data[f"{team}_{shirt_num}_y"] = [np.nan] * len(data["frame"])
 
     data[f"{team}_{shirt_num}_x"][idx] = float(x)
     data[f"{team}_{shirt_num}_y"][idx] = float(y)
 
     return data
```

### Comparing `databallpy-0.2.3/databallpy/load_data/tracking_data/_get_matchtime.py` & `databallpy-0.3.0/databallpy/load_data/tracking_data/_get_matchtime.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 import pandas as pd
 
 from databallpy.load_data.metadata import Metadata
+from databallpy.utils.utils import MISSING_INT
 
 
 def _to_matchtime(secs: int, max_m: int, start_m: int) -> str:
     """Transforms the number of seconds into matchtime format
 
     Args:
         s (int): number of seconds since period started
@@ -61,15 +62,15 @@
             periods_frames["period"],
             periods_frames["end_frame"] - periods_frames["start_frame"],
         )
     )
 
     rel_timestamp = np.array(
         [
-            x - period_start_dict[p] if p > 0 else -999 * frame_rate
+            x - period_start_dict[p] if p > 0 else MISSING_INT * frame_rate
             for x, p in zip(timestamp_column.values, period_column.values)
         ]
     )
     seconds = rel_timestamp // frame_rate
     df = pd.DataFrame(
         {
             "seconds": seconds,
```

### Comparing `databallpy-0.2.3/databallpy/load_data/tracking_data/_insert_missing_rows.py` & `databallpy-0.3.0/databallpy/load_data/tracking_data/_insert_missing_rows.py`

 * *Files identical despite different names*

### Comparing `databallpy-0.2.3/databallpy/load_data/tracking_data/_normalize_playing_direction_tracking.py` & `databallpy-0.3.0/databallpy/load_data/tracking_data/_normalize_playing_direction_tracking.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,16 +16,16 @@
         such a way that the home team is represented of playing from left to right
         for the full match.
     """
 
     home_x = [x for x in td.columns if "_x" in x and "home" in x]
     all_x_y = [x for x in td.columns if "_x" in x or "_y" in x]
     for _, period_row in periods.iterrows():
-        if len(td[td["timestamp"] == period_row["start_frame"]].index) > 0:
+        if len(td[td["frame"] == period_row["start_frame"]].index) > 0:
 
-            idx_start = td[td["timestamp"] == period_row["start_frame"]].index[0]
-            idx_end = td[td["timestamp"] == period_row["end_frame"]].index[0]
+            idx_start = td[td["frame"] == period_row["start_frame"]].index[0]
+            idx_end = td[td["frame"] == period_row["end_frame"]].index[0]
 
             if td.loc[idx_start, home_x].mean() > 0:
                 td.loc[idx_start:idx_end, all_x_y] *= -1
 
     return td
```

### Comparing `databallpy-0.2.3/databallpy/load_data/tracking_data/metrica_tracking_data.py` & `databallpy-0.3.0/databallpy/load_data/tracking_data/metrica_tracking_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     _add_player_tracking_data_to_dict,
 )
 from databallpy.load_data.tracking_data._get_matchtime import _get_matchtime
 from databallpy.load_data.tracking_data._insert_missing_rows import _insert_missing_rows
 from databallpy.load_data.tracking_data._normalize_playing_direction_tracking import (
     _normalize_playing_direction_tracking,
 )
-from databallpy.utils import _to_int
+from databallpy.utils.utils import _to_int
 
 
 def load_metrica_tracking_data(
     tracking_data_loc: str, metadata_loc: str, verbose: bool = True
 ) -> Tuple[pd.DataFrame, Metadata]:
     """Function to load metrica tracking data.
 
@@ -66,18 +66,18 @@
         tracking_data_loc, td_channels, metadata.pitch_dimensions, verbose=verbose
     )
 
     tracking_data = _normalize_playing_direction_tracking(
         tracking_data, metadata.periods_frames
     )
     tracking_data["period"] = _add_periods_to_tracking_data(
-        tracking_data["timestamp"], metadata.periods_frames
+        tracking_data["frame"], metadata.periods_frames
     )
     tracking_data["matchtime_td"] = _get_matchtime(
-        tracking_data["timestamp"], tracking_data["period"], metadata
+        tracking_data["frame"], tracking_data["period"], metadata
     )
 
     return tracking_data, metadata
 
 
 def load_metrica_open_tracking_data(
     verbose: bool = True,
@@ -109,15 +109,15 @@
     pitch_dimensions: list,
     verbose: bool = True,
 ) -> pd.DataFrame:
     """Function to load the tracking data of metrica.
 
     Args:
         tracking_data_loc (Union[str, io.StringIO]): location of the tracking data .txt
-        file channels (dict): dictionary with for all timestamps the order of which
+        file channels (dict): dictionary with for all frames the order of which
         players are referred to in the raw tracking data
         pitch_dimensions (list): x and y dimensions of the pitch in meters
         verbose (bool, optional): whether to print information about the progress in the
         terminal. Defaults to True.
 
     Returns:
         pd.DataFrame: tracking data of the match in a pd dataframe
@@ -128,34 +128,34 @@
         lines = file.readlines()
         file.close()
     else:
         lines = tracking_data_loc.readlines()
 
     size_lines = len(lines)
     data = {
-        "timestamp": [np.nan] * size_lines,
+        "frame": [np.nan] * size_lines,
         "ball_x": [np.nan] * size_lines,
         "ball_y": [np.nan] * size_lines,
         "ball_z": [np.nan] * size_lines,
         "ball_status": [None] * size_lines,
         "ball_posession": [None] * size_lines,
     }
 
     if verbose:
         print("Writing lines to dataframe:")
         lines = tqdm(lines)
 
     for idx, line in enumerate(lines):
 
-        timestamp, players_info, ball_info = line.split(":")
-        timestamp = _to_int(timestamp)
-        data["timestamp"][idx] = timestamp
+        frame, players_info, ball_info = line.split(":")
+        frame = _to_int(frame)
+        data["frame"][idx] = frame
 
         channel = channels.loc[
-            (channels["start"] <= timestamp) & (channels["end"] >= timestamp),
+            (channels["start"] <= frame) & (channels["end"] >= frame),
             "ids",
         ].iloc[0]
 
         players = players_info.split(";")
         for i, player in enumerate(players):
             x, y = player.split(",")
             team = channel[i].split("_")[0]
@@ -170,10 +170,10 @@
 
     for col in [x for x in df.columns if "_x" in x]:
         df[col] = df[col] * pitch_dimensions[0] - (pitch_dimensions[0] / 2)
 
     for col in [x for x in df.columns if "_y" in x]:
         df[col] = df[col] * pitch_dimensions[1] - (pitch_dimensions[1] / 2)
 
-    df = _insert_missing_rows(df, "timestamp")
+    df = _insert_missing_rows(df, "frame")
 
     return df
```

### Comparing `databallpy-0.2.3/databallpy/load_data/tracking_data/tracab.py` & `databallpy-0.3.0/databallpy/load_data/tracking_data/tracab.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     _add_player_tracking_data_to_dict,
 )
 from databallpy.load_data.tracking_data._get_matchtime import _get_matchtime
 from databallpy.load_data.tracking_data._insert_missing_rows import _insert_missing_rows
 from databallpy.load_data.tracking_data._normalize_playing_direction_tracking import (
     _normalize_playing_direction_tracking,
 )
+from databallpy.utils.tz_modification import localize_datetime
+from databallpy.utils.utils import MISSING_INT
 
 
 def load_tracab_tracking_data(
     tracab_loc: str, metadata_loc: str, verbose: bool = True
 ) -> Tuple[pd.DataFrame, Metadata]:
     """Function to load tracking data and metadata from the tracab format
 
@@ -38,18 +40,18 @@
         Tuple[pd.DataFrame, Metadata], the tracking data and metadata class
     """
 
     tracking_data = _get_tracking_data(tracab_loc, verbose)
     metadata = _get_metadata(metadata_loc)
 
     tracking_data["period"] = _add_periods_to_tracking_data(
-        tracking_data["timestamp"], metadata.periods_frames
+        tracking_data["frame"], metadata.periods_frames
     )
     tracking_data["matchtime_td"] = _get_matchtime(
-        tracking_data["timestamp"], tracking_data["period"], metadata
+        tracking_data["frame"], tracking_data["period"], metadata
     )
     tracking_data = _normalize_playing_direction_tracking(
         tracking_data, metadata.periods_frames
     )
 
     return tracking_data, metadata
 
@@ -73,30 +75,30 @@
     if verbose:
         print(" - Completed")
 
     file.close()
     size_lines = len(lines)
 
     data = {
-        "timestamp": [np.nan] * size_lines,
+        "frame": [np.nan] * size_lines,
         "ball_x": [np.nan] * size_lines,
         "ball_y": [np.nan] * size_lines,
         "ball_z": [np.nan] * size_lines,
         "ball_status": [None] * size_lines,
         "ball_posession": [None] * size_lines,
     }
 
     if verbose:
         print("Writing lines to dataframe:")
         lines = tqdm(lines)
 
     for idx, line in enumerate(lines):
 
-        timestamp, players_info, ball_info, _ = line.split(":")
-        data["timestamp"][idx] = int(timestamp)
+        frame, players_info, ball_info, _ = line.split(":")
+        data["frame"][idx] = int(frame)
 
         players = players_info.split(";")[:-1]
         for player in players:
             team_id, _, shirt_num, x, y, _ = player.split(",")
             team_ids = {0: "away", 1: "home"}
             team = team_ids.get(int(team_id))
             if team is None:  # player is unknown or referee
@@ -114,15 +116,15 @@
 
     df = pd.DataFrame(data)
 
     for col in df.columns:
         if "_x" in col or "_y" in col or "_z" in col:
             df[col] = np.round(df[col] / 100, 3)  # change cm to m
 
-    df = _insert_missing_rows(df, "timestamp")
+    df = _insert_missing_rows(df, "frame")
 
     return df
 
 
 def _get_metadata(metadata_loc: str) -> Metadata:
     """Function that reads metadata.xml file and stores it in Metadata class
 
@@ -145,38 +147,47 @@
     datetime_string = soup.find("match")["dtDate"]
     date = pd.to_datetime(datetime_string[:10])
 
     frames_dict = {
         "period": [],
         "start_frame": [],
         "end_frame": [],
-        "start_time_td": [],
-        "end_time_td": [],
+        "start_datetime_td": [],
+        "end_datetime_td": [],
     }
     for _, period in enumerate(soup.find_all("period")):
         frames_dict["period"].append(int(period["iId"]))
         start_frame = int(period["iStartFrame"])
         end_frame = int(period["iEndFrame"])
 
         if start_frame != 0:
             frames_dict["start_frame"].append(start_frame)
             frames_dict["end_frame"].append(end_frame)
-            frames_dict["start_time_td"].append(
+            frames_dict["start_datetime_td"].append(
                 date + dt.timedelta(milliseconds=int((start_frame / frame_rate) * 1000))
             )
-            frames_dict["end_time_td"].append(
+            frames_dict["end_datetime_td"].append(
                 date + dt.timedelta(milliseconds=int((end_frame / frame_rate) * 1000))
             )
         else:
-            frames_dict["start_frame"].append(-999)
-            frames_dict["end_frame"].append(-999)
-            frames_dict["start_time_td"].append(pd.to_datetime("NaT"))
-            frames_dict["end_time_td"].append(pd.to_datetime("NaT"))
+            frames_dict["start_frame"].append(MISSING_INT)
+            frames_dict["end_frame"].append(MISSING_INT)
+            frames_dict["start_datetime_td"].append(pd.to_datetime("NaT"))
+            frames_dict["end_datetime_td"].append(pd.to_datetime("NaT"))
     df_frames = pd.DataFrame(frames_dict)
 
+    # set to right timezone, tracab has no location/competition info
+    # in metadata, so we have to guess
+    df_frames["start_datetime_td"] = localize_datetime(
+        df_frames["start_datetime_td"], "Netherlands"
+    )
+    df_frames["end_datetime_td"] = localize_datetime(
+        df_frames["end_datetime_td"], "Netherlands"
+    )
+
     home_team = soup.find("HomeTeam")
     home_team_name = home_team.find("LongName").text
     home_team_id = int(home_team.find("TeamId").text)
     home_players_info = []
     for player in home_team.find_all("Player"):
         player_dict = {}
         for element in player.findChildren():
@@ -201,20 +212,21 @@
         pitch_dimensions=[pitch_size_x, pitch_size_y],
         periods_frames=df_frames,
         frame_rate=frame_rate,
         home_team_id=home_team_id,
         home_team_name=home_team_name,
         home_players=df_home_players,
         home_score=np.nan,
-        home_formation=None,
+        home_formation="",
         away_team_id=away_team_id,
         away_team_name=away_team_name,
         away_players=df_away_players,
         away_score=np.nan,
-        away_formation=None,
+        away_formation="",
+        country="",
     )
 
     file.close()
 
     return metadata
```

### Comparing `databallpy-0.2.3/databallpy/visualize.py` & `databallpy-0.3.0/databallpy/visualize.py`

 * *Files 2% similar despite different names*

```diff
@@ -368,16 +368,16 @@
         in the clip, this is a pd.Series that should have the same index
         (start_idx:end_idx) as the tracking data that will be plotted. Defaults to None.
         verbose (bool, optional): Whether or not to print info in the terminal on the
         progress
     """
 
     td = match.tracking_data.loc[start_idx:end_idx]
-    td_ht = td[[x for x in match.home_players_column_ids if "_x" in x or "_y" in x]]
-    td_at = td[[x for x in match.away_players_column_ids if "_x" in x or "_y" in x]]
+    td_ht = td[[x for x in match.home_players_column_ids() if "_x" in x or "_y" in x]]
+    td_at = td[[x for x in match.away_players_column_ids() if "_x" in x or "_y" in x]]
 
     if variable_of_interest is not None:
         assert (
             variable_of_interest.index == td.index
         ).all(), (
             "Index of variable of interest and of the tracking data should be alike!"
         )
```

### Comparing `databallpy-0.2.3/pyproject.toml` & `databallpy-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databallpy"
-version = "0.2.3"
+version = "0.3.0"
 description = "A package for loading, preprocessing, vizualising and synchronizing soccere event aand tracking data."
 authors = [
     "Alexander Oonk <alexanderoonk26@gmail.com>",
     "Daan Grob <daaniogrob@gmail.com>",
 ]
 maintainers = [
     "Alexander Oonk <alexanderoonk26@gmail.com>",
@@ -26,15 +26,15 @@
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Topic :: Scientific/Engineering",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-pandas = "^1.5.3"
+pandas = "2.0.1"
 numpy = "^1.24.1"
 beautifulsoup4 = "^4.11.1"
 lxml = "^4.9.2"
 tqdm = "^4.64.1"
 matplotlib = "^3.6.3"
 requests = "^2.28.2"
```

### Comparing `databallpy-0.2.3/setup.py` & `databallpy-0.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['databallpy',
+ 'databallpy.features',
  'databallpy.load_data',
  'databallpy.load_data.event_data',
- 'databallpy.load_data.tracking_data']
+ 'databallpy.load_data.tracking_data',
+ 'databallpy.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['beautifulsoup4>=4.11.1,<5.0.0',
  'lxml>=4.9.2,<5.0.0',
  'matplotlib>=3.6.3,<4.0.0',
  'numpy>=1.24.1,<2.0.0',
- 'pandas>=1.5.3,<2.0.0',
+ 'pandas==2.0.1',
  'requests>=2.28.2,<3.0.0',
  'tqdm>=4.64.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'databallpy',
-    'version': '0.2.3',
+    'version': '0.3.0',
     'description': 'A package for loading, preprocessing, vizualising and synchronizing soccere event aand tracking data.',
-    'long_description': '# databallpy\n\nA package for loading, preprocessing, vizualising and synchronizing soccer event- and tracking data.\n\nThis package is developed to create a standardized way to analyse soccer matches using both event- and tracking data. Other packages, like [kloppy](https://github.com/PySport/kloppy) and [floodlight](https://github.com/floodlight-sports/floodlight), already standardize the import of data sources. The current package goes a step further in combining different data streams from the same match. In this case, the `Match` object combines information from the event and tracking data.\n\n### Changelog for version 0.2.0\n\n- Added parser for Metrica, including an open dataset\n- Added functionality to synchronize tracking and event data\n- Added functionality to plot events\n- Fixed bug, now both tracking and event data are normalized in direction\n- Fixed unexpected behaviour, all date related objects are now datetime objects\n\n### Planned changes\n\n- Adding different filters to filter the tracking data\n- Make the `Match` object more accesable if you don\'t have tracking or event data\n- Adding features to quantify pressure, ball possession, etc. (if you have any ideas/requests, please open an issue!)\n- Adding expected passing and goals models\n\n## Installation\n\n```bash\n$ pip install databallpy\n```\n\n## Usage\n\nThe package is centered around the `Match` object. A `Match` has tracking data, event data metadata about the match.\nFor a more elaborate example, see the [example file](https://databallpy.readthedocs.io/en/latest/example.html)\n\n```console\n$ from databallpy.match import get_match, get_open_match\n$\n$ match = get_match(\n$   tracking_data_loc="../data/tracking_data.dat",\n$   tracking_metadata_loc="../data/tracking_metadata.xml",\n$   tracking_data_provider="tracab"\n$   event_data_loc="../data/event_data_f24.xml",\n$   event_metadata_loc="../data/event_metadata_f7.xml",\n$   event_data_provider="opta",\n$ )\n$\n$ # or to load an open metrica dataset of tracking and event data\n$ match = get_open_match()\n$\n$ match.home_team_name # the team name of the home playing team\n$ match.away_players # pandas dataframe with the names, ids, shirt numbers and positions of the away team\n$ match.tracking_data # pandas dataframe with tracking data of the match\n$ match.event_data # pandas dataframe with event data of the match\n```\n\nSee [the documentation](https://databallpy.readthedocs.io/en/latest/autoapi/databallpy/match/index.html) of the `Match` object and the [example usage](https://databallpy.readthedocs.io/en/latest/example.html) for more options. Note that this package is developed to combine event and tracking data, for now both datastreams are necessary to create a `Match` object.\n\n## Synchronization of tracking and event data\n\nTracking and event data is often poorly synchronized. For instance, when taking the event data of Opta and tracking data of Tracab, you can sync the fist frame with the kick-off pass. Now you can sync the other events with the tracking data based on the time difference between the event and the kick off pass. If you do this, how get something like this:\n\n<video width="640" height="480" controls>\n  <source src="https://raw.githubusercontent.com/Alek050/databallpy/main/docs/example_data/not_synced.mp4" type="video/mp4">\n  Your browser does not support the video tag.\n</video>\n\nAs you can see, the timing (and placing) of the events do not correspond good with the tracking data locations, especially when events follow up quickly or around shots. Using the methodology of [this](https://kwiatkowski.io/sync.soccer) article, this package is able to synchronize tracking and event data using the Needleman-Wunsch algorithm. \n\nAfter running the following command, the events are better synchronized to the tracking data:\n\n```batch\n$ match.synchronise_tracking_and_event_data()\n```\n\n<video width="640" height="480" controls>\n  <source src="https://raw.githubusercontent.com/Alek050/databallpy/main/docs/example_data/synced.mp4" type="video/mp4">\n  Your browser does not support the video tag.\n</video>\n\n## Documentation\n\nThe official documentation can be found [here](https://databallpy.readthedocs.io/en/latest/autoapi/databallpy/index.html).\n\n## Providers\n\nFor now we limited providers. We are planning on adding more providers later on.\n\nEvent data providers:\n- Opta\n- Metrica\n\nTracking data providers:\n- Tracab\n- Metrica\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`databallpy` was created by Alexander Oonk & Daan Grob. It is licensed under the terms of the MIT license.\n\n## Similar projects\n\nAlthough we think this package helps when starting to analyse soccer data, other packages may be better suited for your specific needs. Make sure to check out the following packages as well:\n- [kloppy](https://github.com/PySport/kloppy)\n- [floodlight](https://github.com/floodlight-sports/floodlight)\n- [codeball](https://github.com/metrica-sports/codeball)\n\nAnd for a more specific toturials on how to get started with soccer data"\n- [Friends of Tracking](https://github.com/Friends-of-Tracking-Data-FoTD)\n\n\n\n',
+    'long_description': '# databallpy\n\nA package for loading, preprocessing, vizualising and synchronizing soccer event- and tracking data.\n\nThis package is developed to create a standardized way to analyse soccer matches using both event- and tracking data. Other packages, like [kloppy](https://github.com/PySport/kloppy) and [floodlight](https://github.com/floodlight-sports/floodlight), already standardize the import of data sources. The current package goes a step further in combining different data streams from the same match. In this case, the `Match` object combines information from the event and tracking data.\n\n### Changelog for version 0.3.0\n\n- Added way to save Match objects, and to load saved Match objects\n- Fixed bug in opta event data, own goals are now parsed as seperate event type\n- Added parser for Inmotio tracking data\n- Added parser for Instat event data\n- Added quality checks for the data, raises warning if quality is not good enough\n\n### Planned changes\n\n- Adding different filters to filter the tracking data\n- Adding features to quantify pressure, ball possession, etc. (if you have any ideas/requests, please open an issue!)\n- Standardizing events in the event data\n- Adding expected passing and goals models\n\n## Installation\n\n```bash\n$ pip install databallpy\n```\n\n## Usage\n\nThe package is centered around the `Match` object. A `Match` has tracking data, event data metadata about the match.\nFor a more elaborate example, see the [example file](https://databallpy.readthedocs.io/en/latest/example.html)\n\n```console\n$ from databallpy import get_match, get_open_match\n$\n$ match = get_match(\n$   tracking_data_loc="../data/tracking_data.dat",\n$   tracking_metadata_loc="../data/tracking_metadata.xml",\n$   tracking_data_provider="tracab"\n$   event_data_loc="../data/event_data_f24.xml",\n$   event_metadata_loc="../data/event_metadata_f7.xml",\n$   event_data_provider="opta",\n$ )\n$\n$ # or to load an open metrica dataset of tracking and event data\n$ match = get_open_match()\n$\n$ match.home_team_name # the team name of the home playing team\n$ match.away_players # pandas dataframe with the names, ids, shirt numbers and positions of the away team\n$ match.tracking_data # pandas dataframe with tracking data of the match\n$ match.event_data # pandas dataframe with event data of the match\n```\n\nSee [the documentation](https://databallpy.readthedocs.io/en/latest/autoapi/databallpy/match/index.html) of the `Match` object and the [example usage](https://databallpy.readthedocs.io/en/latest/example.html) for more options. Note that this package is developed to combine event and tracking data, for now both datastreams are necessary to create a `Match` object.\n\n## Synchronization of tracking and event data\n\nTracking and event data is often poorly synchronized. For instance, when taking the event data of Opta and tracking data of Tracab, you can sync the fist frame with the kick-off pass. Now you can sync the other events with the tracking data based on the time difference between the event and the kick off pass. If you do this, how get something like this:\n\n<video width="640" height="480" controls>\n  <source src="https://raw.githubusercontent.com/Alek050/databallpy/main/docs/example_data/not_synced.mp4" type="video/mp4">\n  Your browser does not support the video tag.\n</video>\n\nhttps://user-images.githubusercontent.com/49450063/224564808-fa71735f-5510-464d-8499-9044227a02e8.mp4\n\n\nAs you can see, the timing (and placing) of the events do not correspond good with the tracking data locations, especially when events follow up quickly or around shots. Using the methodology of [this](https://kwiatkowski.io/sync.soccer) article, this package is able to synchronize tracking and event data using the Needleman-Wunsch algorithm. \n\nAfter running the following command, the events are better synchronized to the tracking data:\n\n```batch\n$ match.synchronise_tracking_and_event_data()\n```\n\n<video width="640" height="480" controls>\n  <source src="https://raw.githubusercontent.com/Alek050/databallpy/main/docs/example_data/synced.mp4" type="video/mp4">\n  Your browser does not support the video tag.\n</video>\n\n\nhttps://user-images.githubusercontent.com/49450063/224564913-4091faf7-f6ef-4429-b132-7f93ce5e1d91.mp4\n\n\n## Documentation\n\nThe official documentation can be found [here](https://databallpy.readthedocs.io/en/latest/autoapi/databallpy/index.html).\n\n## Providers\n\nFor now we limited providers. We are planning on adding more providers later on.\n\nEvent data providers:\n- Opta\n- Metrica\n- Instat\n\nTracking data providers:\n- Tracab\n- Metrica\n- Inmotio\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n#### Maintainers & owners\n\n- [Alek050](https://github.com/Alek050/)\n- [DaanGro](https://github.com/DaanGro/)\n\n#### Contributors\n\n- [rdghe](https://github.com/rdghe/)\n\n## License\n\n`databallpy` was created by Alexander Oonk & Daan Grob. It is licensed under the terms of the MIT license.\n\n## Similar projects\n\nAlthough we think this package helps when starting to analyse soccer data, other packages may be better suited for your specific needs. Make sure to check out the following packages as well:\n- [kloppy](https://github.com/PySport/kloppy)\n- [floodlight](https://github.com/floodlight-sports/floodlight)\n- [codeball](https://github.com/metrica-sports/codeball)\n\nAnd for a more specific toturials on how to get started with soccer data"\n- [Friends of Tracking](https://github.com/Friends-of-Tracking-Data-FoTD)\n\n\n\n',
     'author': 'Alexander Oonk',
     'author_email': 'alexanderoonk26@gmail.com',
     'maintainer': 'Alexander Oonk',
     'maintainer_email': 'alexanderoonk26@gmail.com',
     'url': 'https://pypi.org/project/databallpy/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `databallpy-0.2.3/PKG-INFO` & `databallpy-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databallpy
-Version: 0.2.3
+Version: 0.3.0
 Summary: A package for loading, preprocessing, vizualising and synchronizing soccere event aand tracking data.
 Home-page: https://pypi.org/project/databallpy/
 License: MIT
 Keywords: soccer,football,tracking data,event data
 Author: Alexander Oonk
 Author-email: alexanderoonk26@gmail.com
 Maintainer: Alexander Oonk
@@ -23,55 +23,55 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: matplotlib (>=3.6.3,<4.0.0)
 Requires-Dist: numpy (>=1.24.1,<2.0.0)
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: pandas (==2.0.1)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Project-URL: Documentation, https://github.com/Alek050/databallpy/tree/main/docs
 Project-URL: Repository, https://github.com/Alek050/databallpy
 Description-Content-Type: text/markdown
 
 # databallpy
 
 A package for loading, preprocessing, vizualising and synchronizing soccer event- and tracking data.
 
 This package is developed to create a standardized way to analyse soccer matches using both event- and tracking data. Other packages, like [kloppy](https://github.com/PySport/kloppy) and [floodlight](https://github.com/floodlight-sports/floodlight), already standardize the import of data sources. The current package goes a step further in combining different data streams from the same match. In this case, the `Match` object combines information from the event and tracking data.
 
-### Changelog for version 0.2.0
+### Changelog for version 0.3.0
 
-- Added parser for Metrica, including an open dataset
-- Added functionality to synchronize tracking and event data
-- Added functionality to plot events
-- Fixed bug, now both tracking and event data are normalized in direction
-- Fixed unexpected behaviour, all date related objects are now datetime objects
+- Added way to save Match objects, and to load saved Match objects
+- Fixed bug in opta event data, own goals are now parsed as seperate event type
+- Added parser for Inmotio tracking data
+- Added parser for Instat event data
+- Added quality checks for the data, raises warning if quality is not good enough
 
 ### Planned changes
 
 - Adding different filters to filter the tracking data
-- Make the `Match` object more accesable if you don't have tracking or event data
 - Adding features to quantify pressure, ball possession, etc. (if you have any ideas/requests, please open an issue!)
+- Standardizing events in the event data
 - Adding expected passing and goals models
 
 ## Installation
 
 ```bash
 $ pip install databallpy
 ```
 
 ## Usage
 
 The package is centered around the `Match` object. A `Match` has tracking data, event data metadata about the match.
 For a more elaborate example, see the [example file](https://databallpy.readthedocs.io/en/latest/example.html)
 
 ```console
-$ from databallpy.match import get_match, get_open_match
+$ from databallpy import get_match, get_open_match
 $
 $ match = get_match(
 $   tracking_data_loc="../data/tracking_data.dat",
 $   tracking_metadata_loc="../data/tracking_metadata.xml",
 $   tracking_data_provider="tracab"
 $   event_data_loc="../data/event_data_f24.xml",
 $   event_metadata_loc="../data/event_metadata_f7.xml",
@@ -94,47 +94,65 @@
 Tracking and event data is often poorly synchronized. For instance, when taking the event data of Opta and tracking data of Tracab, you can sync the fist frame with the kick-off pass. Now you can sync the other events with the tracking data based on the time difference between the event and the kick off pass. If you do this, how get something like this:
 
 <video width="640" height="480" controls>
   <source src="https://raw.githubusercontent.com/Alek050/databallpy/main/docs/example_data/not_synced.mp4" type="video/mp4">
   Your browser does not support the video tag.
 </video>
 
+https://user-images.githubusercontent.com/49450063/224564808-fa71735f-5510-464d-8499-9044227a02e8.mp4
+
+
 As you can see, the timing (and placing) of the events do not correspond good with the tracking data locations, especially when events follow up quickly or around shots. Using the methodology of [this](https://kwiatkowski.io/sync.soccer) article, this package is able to synchronize tracking and event data using the Needleman-Wunsch algorithm. 
 
 After running the following command, the events are better synchronized to the tracking data:
 
 ```batch
 $ match.synchronise_tracking_and_event_data()
 ```
 
 <video width="640" height="480" controls>
   <source src="https://raw.githubusercontent.com/Alek050/databallpy/main/docs/example_data/synced.mp4" type="video/mp4">
   Your browser does not support the video tag.
 </video>
 
+
+https://user-images.githubusercontent.com/49450063/224564913-4091faf7-f6ef-4429-b132-7f93ce5e1d91.mp4
+
+
 ## Documentation
 
 The official documentation can be found [here](https://databallpy.readthedocs.io/en/latest/autoapi/databallpy/index.html).
 
 ## Providers
 
 For now we limited providers. We are planning on adding more providers later on.
 
 Event data providers:
 - Opta
 - Metrica
+- Instat
 
 Tracking data providers:
 - Tracab
 - Metrica
+- Inmotio
 
 ## Contributing
 
 Interested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.
 
+#### Maintainers & owners
+
+- [Alek050](https://github.com/Alek050/)
+- [DaanGro](https://github.com/DaanGro/)
+
+#### Contributors
+
+- [rdghe](https://github.com/rdghe/)
+
 ## License
 
 `databallpy` was created by Alexander Oonk & Daan Grob. It is licensed under the terms of the MIT license.
 
 ## Similar projects
 
 Although we think this package helps when starting to analyse soccer data, other packages may be better suited for your specific needs. Make sure to check out the following packages as well:
```

