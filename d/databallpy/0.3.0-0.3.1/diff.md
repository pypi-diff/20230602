# Comparing `tmp/databallpy-0.3.0.tar.gz` & `tmp/databallpy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databallpy-0.3.0.tar", max compression
+gzip compressed data, was "databallpy-0.3.1.tar", max compression
```

## Comparing `databallpy-0.3.0.tar` & `databallpy-0.3.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rwxr-xr-x   0        0        0     1085 2023-01-24 11:30:08.329567 databallpy-0.3.0/LICENSE
--rw-r--r--   0        0        0     5601 2023-06-02 18:05:51.279039 databallpy-0.3.0/README.md
--rw-r--r--   0        0        0      191 2023-05-13 07:28:52.676655 databallpy-0.3.0/databallpy/__init__.py
--rw-r--r--   0        0        0      188 2023-05-13 07:28:52.676769 databallpy-0.3.0/databallpy/errors.py
--rw-r--r--   0        0        0        0 2023-05-23 13:42:10.199898 databallpy-0.3.0/databallpy/features/__init__.py
--rw-r--r--   0        0        0      977 2023-06-02 17:51:23.224996 databallpy-0.3.0/databallpy/features/velocity.py
--rw-r--r--   0        0        0    14220 2023-06-02 17:51:23.225230 databallpy-0.3.0/databallpy/get_match.py
--rw-r--r--   0        0        0        0 2023-02-10 10:17:56.160462 databallpy-0.3.0/databallpy/load_data/__init__.py
--rw-r--r--   0        0        0        0 2023-02-10 10:17:56.160612 databallpy-0.3.0/databallpy/load_data/event_data/__init__.py
--rw-r--r--   0        0        0     1554 2023-03-12 15:25:48.209137 databallpy-0.3.0/databallpy/load_data/event_data/_normalize_playing_direction_events.py
--rw-r--r--   0        0        0    11983 2023-05-23 13:42:10.200791 databallpy-0.3.0/databallpy/load_data/event_data/instat.py
--rw-r--r--   0        0        0     6046 2023-05-07 15:03:40.624364 databallpy-0.3.0/databallpy/load_data/event_data/metrica_event_data.py
--rw-r--r--   0        0        0    13205 2023-06-02 17:51:23.225484 databallpy-0.3.0/databallpy/load_data/event_data/opta.py
--rw-r--r--   0        0        0     8024 2023-05-30 11:34:09.440544 databallpy-0.3.0/databallpy/load_data/metadata.py
--rw-r--r--   0        0        0    11737 2023-05-23 13:42:10.201042 databallpy-0.3.0/databallpy/load_data/metrica_metadata.py
--rw-r--r--   0        0        0        0 2023-02-10 10:17:56.161101 databallpy-0.3.0/databallpy/load_data/tracking_data/__init__.py
--rw-r--r--   0        0        0      757 2023-05-07 15:03:40.625076 databallpy-0.3.0/databallpy/load_data/tracking_data/_add_ball_data_to_dict.py
--rw-r--r--   0        0        0     1644 2023-05-23 13:42:10.201200 databallpy-0.3.0/databallpy/load_data/tracking_data/_add_periods_to_tracking_data.py
--rw-r--r--   0        0        0      961 2023-04-25 15:26:54.930980 databallpy-0.3.0/databallpy/load_data/tracking_data/_add_player_tracking_data_to_dict.py
--rw-r--r--   0        0        0     3527 2023-05-23 13:42:10.201343 databallpy-0.3.0/databallpy/load_data/tracking_data/_get_matchtime.py
--rw-r--r--   0        0        0     1031 2023-02-10 10:17:56.162980 databallpy-0.3.0/databallpy/load_data/tracking_data/_insert_missing_rows.py
--rw-r--r--   0        0        0     1160 2023-05-01 15:00:27.444838 databallpy-0.3.0/databallpy/load_data/tracking_data/_normalize_playing_direction_tracking.py
--rw-r--r--   0        0        0    11401 2023-06-02 17:51:23.225734 databallpy-0.3.0/databallpy/load_data/tracking_data/_quality_check_tracking_data.py
--rw-r--r--   0        0        0    10444 2023-05-23 13:42:10.201633 databallpy-0.3.0/databallpy/load_data/tracking_data/inmotio.py
--rw-r--r--   0        0        0     6106 2023-05-07 15:03:40.625412 databallpy-0.3.0/databallpy/load_data/tracking_data/metrica_tracking_data.py
--rw-r--r--   0        0        0     8771 2023-05-23 13:42:10.201789 databallpy-0.3.0/databallpy/load_data/tracking_data/tracab.py
--rw-r--r--   0        0        0    19833 2023-06-02 17:51:23.226003 databallpy-0.3.0/databallpy/match.py
--rw-r--r--   0        0        0        0 2023-05-07 15:03:40.625878 databallpy-0.3.0/databallpy/utils/__init__.py
--rw-r--r--   0        0        0    10874 2023-06-02 17:51:23.226279 databallpy-0.3.0/databallpy/utils/synchronise_tracking_and_event_data.py
--rw-r--r--   0        0        0     2003 2023-05-13 08:42:27.134855 databallpy-0.3.0/databallpy/utils/tz_modification.py
--rw-r--r--   0        0        0     2931 2023-05-23 13:42:10.202310 databallpy-0.3.0/databallpy/utils/utils.py
--rw-r--r--   0        0        0    18381 2023-05-01 14:32:31.340350 databallpy-0.3.0/databallpy/visualize.py
--rw-r--r--   0        0        0      190 2023-05-23 13:42:10.202488 databallpy-0.3.0/databallpy/warnings.py
--rw-r--r--   0        0        0     2524 2023-06-02 17:59:04.862948 databallpy-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6800 1970-01-01 00:00:00.000000 databallpy-0.3.0/setup.py
--rw-r--r--   0        0        0     7146 1970-01-01 00:00:00.000000 databallpy-0.3.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1085 2023-01-24 11:30:08.329567 databallpy-0.3.1/LICENSE
+-rw-r--r--   0        0        0     5601 2023-06-02 19:11:50.897716 databallpy-0.3.1/README.md
+-rw-r--r--   0        0        0      191 2023-05-13 07:28:52.676655 databallpy-0.3.1/databallpy/__init__.py
+-rw-r--r--   0        0        0      188 2023-05-13 07:28:52.676769 databallpy-0.3.1/databallpy/errors.py
+-rw-r--r--   0        0        0        0 2023-05-23 13:42:10.199898 databallpy-0.3.1/databallpy/features/__init__.py
+-rw-r--r--   0        0        0      977 2023-06-02 17:51:23.224996 databallpy-0.3.1/databallpy/features/velocity.py
+-rw-r--r--   0        0        0    14276 2023-06-02 19:33:15.009434 databallpy-0.3.1/databallpy/get_match.py
+-rw-r--r--   0        0        0        0 2023-02-10 10:17:56.160462 databallpy-0.3.1/databallpy/load_data/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-10 10:17:56.160612 databallpy-0.3.1/databallpy/load_data/event_data/__init__.py
+-rw-r--r--   0        0        0     1554 2023-03-12 15:25:48.209137 databallpy-0.3.1/databallpy/load_data/event_data/_normalize_playing_direction_events.py
+-rw-r--r--   0        0        0    11983 2023-05-23 13:42:10.200791 databallpy-0.3.1/databallpy/load_data/event_data/instat.py
+-rw-r--r--   0        0        0     6046 2023-05-07 15:03:40.624364 databallpy-0.3.1/databallpy/load_data/event_data/metrica_event_data.py
+-rw-r--r--   0        0        0    13205 2023-06-02 17:51:23.225484 databallpy-0.3.1/databallpy/load_data/event_data/opta.py
+-rw-r--r--   0        0        0     8024 2023-05-30 11:34:09.440544 databallpy-0.3.1/databallpy/load_data/metadata.py
+-rw-r--r--   0        0        0    11737 2023-05-23 13:42:10.201042 databallpy-0.3.1/databallpy/load_data/metrica_metadata.py
+-rw-r--r--   0        0        0        0 2023-02-10 10:17:56.161101 databallpy-0.3.1/databallpy/load_data/tracking_data/__init__.py
+-rw-r--r--   0        0        0      757 2023-05-07 15:03:40.625076 databallpy-0.3.1/databallpy/load_data/tracking_data/_add_ball_data_to_dict.py
+-rw-r--r--   0        0        0     1644 2023-05-23 13:42:10.201200 databallpy-0.3.1/databallpy/load_data/tracking_data/_add_periods_to_tracking_data.py
+-rw-r--r--   0        0        0      961 2023-04-25 15:26:54.930980 databallpy-0.3.1/databallpy/load_data/tracking_data/_add_player_tracking_data_to_dict.py
+-rw-r--r--   0        0        0     3527 2023-05-23 13:42:10.201343 databallpy-0.3.1/databallpy/load_data/tracking_data/_get_matchtime.py
+-rw-r--r--   0        0        0     1031 2023-02-10 10:17:56.162980 databallpy-0.3.1/databallpy/load_data/tracking_data/_insert_missing_rows.py
+-rw-r--r--   0        0        0     1160 2023-05-01 15:00:27.444838 databallpy-0.3.1/databallpy/load_data/tracking_data/_normalize_playing_direction_tracking.py
+-rw-r--r--   0        0        0    11401 2023-06-02 17:51:23.225734 databallpy-0.3.1/databallpy/load_data/tracking_data/_quality_check_tracking_data.py
+-rw-r--r--   0        0        0    10444 2023-05-23 13:42:10.201633 databallpy-0.3.1/databallpy/load_data/tracking_data/inmotio.py
+-rw-r--r--   0        0        0     6106 2023-05-07 15:03:40.625412 databallpy-0.3.1/databallpy/load_data/tracking_data/metrica_tracking_data.py
+-rw-r--r--   0        0        0     8771 2023-05-23 13:42:10.201789 databallpy-0.3.1/databallpy/load_data/tracking_data/tracab.py
+-rw-r--r--   0        0        0    19833 2023-06-02 17:51:23.226003 databallpy-0.3.1/databallpy/match.py
+-rw-r--r--   0        0        0        0 2023-05-07 15:03:40.625878 databallpy-0.3.1/databallpy/utils/__init__.py
+-rw-r--r--   0        0        0    10874 2023-06-02 17:51:23.226279 databallpy-0.3.1/databallpy/utils/synchronise_tracking_and_event_data.py
+-rw-r--r--   0        0        0     2003 2023-05-13 08:42:27.134855 databallpy-0.3.1/databallpy/utils/tz_modification.py
+-rw-r--r--   0        0        0     2931 2023-05-23 13:42:10.202310 databallpy-0.3.1/databallpy/utils/utils.py
+-rw-r--r--   0        0        0    18381 2023-05-01 14:32:31.340350 databallpy-0.3.1/databallpy/visualize.py
+-rw-r--r--   0        0        0      190 2023-05-23 13:42:10.202488 databallpy-0.3.1/databallpy/warnings.py
+-rw-r--r--   0        0        0     2524 2023-06-02 19:35:42.133775 databallpy-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6800 1970-01-01 00:00:00.000000 databallpy-0.3.1/setup.py
+-rw-r--r--   0        0        0     7146 1970-01-01 00:00:00.000000 databallpy-0.3.1/PKG-INFO
```

### Comparing `databallpy-0.3.0/LICENSE` & `databallpy-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `databallpy-0.3.0/README.md` & `databallpy-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `databallpy-0.3.0/databallpy/features/velocity.py` & `databallpy-0.3.1/databallpy/features/velocity.py`

 * *Files identical despite different names*

### Comparing `databallpy-0.3.0/databallpy/get_match.py` & `databallpy-0.3.1/databallpy/get_match.py`

 * *Files 0% similar despite different names*

```diff
@@ -363,9 +363,10 @@
         home_players=metadata.home_players,
         away_team_id=metadata.away_team_id,
         away_formation=metadata.away_formation,
         away_score=metadata.away_score,
         away_team_name=metadata.away_team_name,
         away_players=metadata.away_players,
         country="",
+        allow_synchronise_tracking_and_event_data=True,
     )
     return match
```

### Comparing `databallpy-0.3.0/databallpy/load_data/event_data/_normalize_playing_direction_events.py` & `databallpy-0.3.1/databallpy/load_data/event_data/_normalize_playing_direction_events.py`

 * *Files identical despite different names*

### Comparing `databallpy-0.3.0/databallpy/load_data/event_data/instat.py` & `databallpy-0.3.1/databallpy/load_data/event_data/instat.py`

 * *Files identical despite different names*

### Comparing `databallpy-0.3.0/databallpy/load_data/event_data/metrica_event_data.py` & `databallpy-0.3.1/databallpy/load_data/event_data/metrica_event_data.py`

 * *Files identical despite different names*

### Comparing `databallpy-0.3.0/databallpy/load_data/event_data/opta.py` & `databallpy-0.3.1/databallpy/load_data/event_data/opta.py`

 * *Files identical despite different names*

### Comparing `databallpy-0.3.0/databallpy/load_data/metadata.py` & `databallpy-0.3.1/databallpy/load_data/metadata.py`

 * *Files identical despite different names*

### Comparing `databallpy-0.3.0/databallpy/load_data/metrica_metadata.py` & `databallpy-0.3.1/databallpy/load_data/metrica_metadata.py`

 * *Files identical despite different names*

### Comparing `databallpy-0.3.0/databallpy/load_data/tracking_data/_add_ball_data_to_dict.py` & `databallpy-0.3.1/databallpy/load_data/tracking_data/_add_ball_data_to_dict.py`

 * *Files identical despite different names*

### Comparing `databallpy-0.3.0/databallpy/load_data/tracking_data/_add_periods_to_tracking_data.py` & `databallpy-0.3.1/databallpy/load_data/tracking_data/_add_periods_to_tracking_data.py`

 * *Files identical despite different names*

### Comparing `databallpy-0.3.0/databallpy/load_data/tracking_data/_add_player_tracking_data_to_dict.py` & `databallpy-0.3.1/databallpy/load_data/tracking_data/_add_player_tracking_data_to_dict.py`

 * *Files identical despite different names*

### Comparing `databallpy-0.3.0/databallpy/load_data/tracking_data/_get_matchtime.py` & `databallpy-0.3.1/databallpy/load_data/tracking_data/_get_matchtime.py`

 * *Files identical despite different names*

### Comparing `databallpy-0.3.0/databallpy/load_data/tracking_data/_insert_missing_rows.py` & `databallpy-0.3.1/databallpy/load_data/tracking_data/_insert_missing_rows.py`

 * *Files identical despite different names*

### Comparing `databallpy-0.3.0/databallpy/load_data/tracking_data/_normalize_playing_direction_tracking.py` & `databallpy-0.3.1/databallpy/load_data/tracking_data/_normalize_playing_direction_tracking.py`

 * *Files identical despite different names*

### Comparing `databallpy-0.3.0/databallpy/load_data/tracking_data/_quality_check_tracking_data.py` & `databallpy-0.3.1/databallpy/load_data/tracking_data/_quality_check_tracking_data.py`

 * *Files identical despite different names*

### Comparing `databallpy-0.3.0/databallpy/load_data/tracking_data/inmotio.py` & `databallpy-0.3.1/databallpy/load_data/tracking_data/inmotio.py`

 * *Files identical despite different names*

### Comparing `databallpy-0.3.0/databallpy/load_data/tracking_data/metrica_tracking_data.py` & `databallpy-0.3.1/databallpy/load_data/tracking_data/metrica_tracking_data.py`

 * *Files identical despite different names*

### Comparing `databallpy-0.3.0/databallpy/load_data/tracking_data/tracab.py` & `databallpy-0.3.1/databallpy/load_data/tracking_data/tracab.py`

 * *Files identical despite different names*

### Comparing `databallpy-0.3.0/databallpy/match.py` & `databallpy-0.3.1/databallpy/match.py`

 * *Files identical despite different names*

### Comparing `databallpy-0.3.0/databallpy/utils/synchronise_tracking_and_event_data.py` & `databallpy-0.3.1/databallpy/utils/synchronise_tracking_and_event_data.py`

 * *Files identical despite different names*

### Comparing `databallpy-0.3.0/databallpy/utils/tz_modification.py` & `databallpy-0.3.1/databallpy/utils/tz_modification.py`

 * *Files identical despite different names*

### Comparing `databallpy-0.3.0/databallpy/utils/utils.py` & `databallpy-0.3.1/databallpy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `databallpy-0.3.0/databallpy/visualize.py` & `databallpy-0.3.1/databallpy/visualize.py`

 * *Files identical despite different names*

### Comparing `databallpy-0.3.0/pyproject.toml` & `databallpy-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databallpy"
-version = "0.3.0"
+version = "0.3.1"
 description = "A package for loading, preprocessing, vizualising and synchronizing soccere event aand tracking data."
 authors = [
     "Alexander Oonk <alexanderoonk26@gmail.com>",
     "Daan Grob <daaniogrob@gmail.com>",
 ]
 maintainers = [
     "Alexander Oonk <alexanderoonk26@gmail.com>",
```

### Comparing `databallpy-0.3.0/setup.py` & `databallpy-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'numpy>=1.24.1,<2.0.0',
  'pandas==2.0.1',
  'requests>=2.28.2,<3.0.0',
  'tqdm>=4.64.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'databallpy',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'A package for loading, preprocessing, vizualising and synchronizing soccere event aand tracking data.',
     'long_description': '# databallpy\n\nA package for loading, preprocessing, vizualising and synchronizing soccer event- and tracking data.\n\nThis package is developed to create a standardized way to analyse soccer matches using both event- and tracking data. Other packages, like [kloppy](https://github.com/PySport/kloppy) and [floodlight](https://github.com/floodlight-sports/floodlight), already standardize the import of data sources. The current package goes a step further in combining different data streams from the same match. In this case, the `Match` object combines information from the event and tracking data.\n\n### Changelog for version 0.3.0\n\n- Added way to save Match objects, and to load saved Match objects\n- Fixed bug in opta event data, own goals are now parsed as seperate event type\n- Added parser for Inmotio tracking data\n- Added parser for Instat event data\n- Added quality checks for the data, raises warning if quality is not good enough\n\n### Planned changes\n\n- Adding different filters to filter the tracking data\n- Adding features to quantify pressure, ball possession, etc. (if you have any ideas/requests, please open an issue!)\n- Standardizing events in the event data\n- Adding expected passing and goals models\n\n## Installation\n\n```bash\n$ pip install databallpy\n```\n\n## Usage\n\nThe package is centered around the `Match` object. A `Match` has tracking data, event data metadata about the match.\nFor a more elaborate example, see the [example file](https://databallpy.readthedocs.io/en/latest/example.html)\n\n```console\n$ from databallpy import get_match, get_open_match\n$\n$ match = get_match(\n$   tracking_data_loc="../data/tracking_data.dat",\n$   tracking_metadata_loc="../data/tracking_metadata.xml",\n$   tracking_data_provider="tracab"\n$   event_data_loc="../data/event_data_f24.xml",\n$   event_metadata_loc="../data/event_metadata_f7.xml",\n$   event_data_provider="opta",\n$ )\n$\n$ # or to load an open metrica dataset of tracking and event data\n$ match = get_open_match()\n$\n$ match.home_team_name # the team name of the home playing team\n$ match.away_players # pandas dataframe with the names, ids, shirt numbers and positions of the away team\n$ match.tracking_data # pandas dataframe with tracking data of the match\n$ match.event_data # pandas dataframe with event data of the match\n```\n\nSee [the documentation](https://databallpy.readthedocs.io/en/latest/autoapi/databallpy/match/index.html) of the `Match` object and the [example usage](https://databallpy.readthedocs.io/en/latest/example.html) for more options. Note that this package is developed to combine event and tracking data, for now both datastreams are necessary to create a `Match` object.\n\n## Synchronization of tracking and event data\n\nTracking and event data is often poorly synchronized. For instance, when taking the event data of Opta and tracking data of Tracab, you can sync the fist frame with the kick-off pass. Now you can sync the other events with the tracking data based on the time difference between the event and the kick off pass. If you do this, how get something like this:\n\n<video width="640" height="480" controls>\n  <source src="https://raw.githubusercontent.com/Alek050/databallpy/main/docs/example_data/not_synced.mp4" type="video/mp4">\n  Your browser does not support the video tag.\n</video>\n\nhttps://user-images.githubusercontent.com/49450063/224564808-fa71735f-5510-464d-8499-9044227a02e8.mp4\n\n\nAs you can see, the timing (and placing) of the events do not correspond good with the tracking data locations, especially when events follow up quickly or around shots. Using the methodology of [this](https://kwiatkowski.io/sync.soccer) article, this package is able to synchronize tracking and event data using the Needleman-Wunsch algorithm. \n\nAfter running the following command, the events are better synchronized to the tracking data:\n\n```batch\n$ match.synchronise_tracking_and_event_data()\n```\n\n<video width="640" height="480" controls>\n  <source src="https://raw.githubusercontent.com/Alek050/databallpy/main/docs/example_data/synced.mp4" type="video/mp4">\n  Your browser does not support the video tag.\n</video>\n\n\nhttps://user-images.githubusercontent.com/49450063/224564913-4091faf7-f6ef-4429-b132-7f93ce5e1d91.mp4\n\n\n## Documentation\n\nThe official documentation can be found [here](https://databallpy.readthedocs.io/en/latest/autoapi/databallpy/index.html).\n\n## Providers\n\nFor now we limited providers. We are planning on adding more providers later on.\n\nEvent data providers:\n- Opta\n- Metrica\n- Instat\n\nTracking data providers:\n- Tracab\n- Metrica\n- Inmotio\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n#### Maintainers & owners\n\n- [Alek050](https://github.com/Alek050/)\n- [DaanGro](https://github.com/DaanGro/)\n\n#### Contributors\n\n- [rdghe](https://github.com/rdghe/)\n\n## License\n\n`databallpy` was created by Alexander Oonk & Daan Grob. It is licensed under the terms of the MIT license.\n\n## Similar projects\n\nAlthough we think this package helps when starting to analyse soccer data, other packages may be better suited for your specific needs. Make sure to check out the following packages as well:\n- [kloppy](https://github.com/PySport/kloppy)\n- [floodlight](https://github.com/floodlight-sports/floodlight)\n- [codeball](https://github.com/metrica-sports/codeball)\n\nAnd for a more specific toturials on how to get started with soccer data"\n- [Friends of Tracking](https://github.com/Friends-of-Tracking-Data-FoTD)\n\n\n\n',
     'author': 'Alexander Oonk',
     'author_email': 'alexanderoonk26@gmail.com',
     'maintainer': 'Alexander Oonk',
     'maintainer_email': 'alexanderoonk26@gmail.com',
     'url': 'https://pypi.org/project/databallpy/',
```

### Comparing `databallpy-0.3.0/PKG-INFO` & `databallpy-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databallpy
-Version: 0.3.0
+Version: 0.3.1
 Summary: A package for loading, preprocessing, vizualising and synchronizing soccere event aand tracking data.
 Home-page: https://pypi.org/project/databallpy/
 License: MIT
 Keywords: soccer,football,tracking data,event data
 Author: Alexander Oonk
 Author-email: alexanderoonk26@gmail.com
 Maintainer: Alexander Oonk
```

