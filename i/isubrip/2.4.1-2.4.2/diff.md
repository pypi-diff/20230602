# Comparing `tmp/isubrip-2.4.1.tar.gz` & `tmp/isubrip-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isubrip-2.4.1.tar", last modified: Thu May 25 09:09:54 2023, max compression
+gzip compressed data, was "isubrip-2.4.2.tar", last modified: Fri Jun  2 18:34:52 2023, max compression
```

## Comparing `isubrip-2.4.1.tar` & `isubrip-2.4.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 09:09:54.720051 isubrip-2.4.1/
--rw-rw-rw-   0        0        0     1093 2022-01-28 09:13:22.000000 isubrip-2.4.1/LICENSE
--rw-rw-rw-   0        0        0     3536 2023-05-25 09:09:54.719053 isubrip-2.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     2411 2023-05-25 08:44:47.000000 isubrip-2.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 09:09:54.704043 isubrip-2.4.1/isubrip/
--rw-rw-rw-   0        0        0       23 2023-05-25 08:44:47.000000 isubrip-2.4.1/isubrip/__init__.py
--rw-rw-rw-   0        0        0    12873 2023-05-25 08:19:55.000000 isubrip-2.4.1/isubrip/__main__.py
--rw-rw-rw-   0        0        0    11798 2023-05-25 08:19:55.000000 isubrip-2.4.1/isubrip/config.py
--rw-rw-rw-   0        0        0     2178 2023-05-24 22:34:46.000000 isubrip-2.4.1/isubrip/constants.py
--rw-rw-rw-   0        0        0     6053 2023-05-24 22:34:46.000000 isubrip-2.4.1/isubrip/data_structures.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:09:54.710051 isubrip-2.4.1/isubrip/resources/
--rw-rw-rw-   0        0        0      595 2023-05-23 20:01:27.000000 isubrip-2.4.1/isubrip/resources/default_config.toml
-drwxrwxrwx   0        0        0        0 2023-05-25 09:09:54.714050 isubrip-2.4.1/isubrip/scrapers/
--rw-rw-rw-   0        0        0        0 2023-05-24 22:34:46.000000 isubrip-2.4.1/isubrip/scrapers/__init__.py
--rw-rw-rw-   0        0        0    15845 2023-05-24 22:34:46.000000 isubrip-2.4.1/isubrip/scrapers/appletv_scraper.py
--rw-rw-rw-   0        0        0     4375 2023-05-24 22:34:46.000000 isubrip-2.4.1/isubrip/scrapers/itunes_scraper.py
--rw-rw-rw-   0        0        0    22230 2023-05-24 22:34:46.000000 isubrip-2.4.1/isubrip/scrapers/scraper.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:09:54.718051 isubrip-2.4.1/isubrip/subtitle_formats/
--rw-rw-rw-   0        0        0        0 2023-05-24 22:34:46.000000 isubrip-2.4.1/isubrip/subtitle_formats/__init__.py
--rw-rw-rw-   0        0        0     1383 2023-05-24 22:34:46.000000 isubrip-2.4.1/isubrip/subtitle_formats/subrip.py
--rw-rw-rw-   0        0        0     7909 2023-05-24 22:34:46.000000 isubrip-2.4.1/isubrip/subtitle_formats/subtitles.py
--rw-rw-rw-   0        0        0     9220 2023-05-24 22:34:46.000000 isubrip-2.4.1/isubrip/subtitle_formats/webvtt.py
--rw-rw-rw-   0        0        0    13341 2023-05-25 08:19:55.000000 isubrip-2.4.1/isubrip/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:09:54.709051 isubrip-2.4.1/isubrip.egg-info/
--rw-rw-rw-   0        0        0     3536 2023-05-25 09:09:54.000000 isubrip-2.4.1/isubrip.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      663 2023-05-25 09:09:54.000000 isubrip-2.4.1/isubrip.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 09:09:54.000000 isubrip-2.4.1/isubrip.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-25 09:09:54.000000 isubrip-2.4.1/isubrip.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       38 2023-05-25 09:09:54.000000 isubrip-2.4.1/isubrip.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-25 09:09:54.000000 isubrip-2.4.1/isubrip.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       83 2023-05-24 22:34:46.000000 isubrip-2.4.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-25 09:09:54.720051 isubrip-2.4.1/setup.cfg
--rw-rw-rw-   0        0        0     2815 2023-05-24 22:34:46.000000 isubrip-2.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:34:52.664036 isubrip-2.4.2/
+-rw-rw-rw-   0        0        0     1093 2022-01-28 09:13:22.000000 isubrip-2.4.2/LICENSE
+-rw-rw-rw-   0        0        0     3536 2023-06-02 18:34:52.663036 isubrip-2.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2411 2023-06-02 18:33:22.000000 isubrip-2.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 18:34:52.646516 isubrip-2.4.2/isubrip/
+-rw-rw-rw-   0        0        0       23 2023-06-02 18:33:22.000000 isubrip-2.4.2/isubrip/__init__.py
+-rw-rw-rw-   0        0        0    13093 2023-06-02 18:33:22.000000 isubrip-2.4.2/isubrip/__main__.py
+-rw-rw-rw-   0        0        0    11888 2023-06-02 14:55:15.000000 isubrip-2.4.2/isubrip/config.py
+-rw-rw-rw-   0        0        0     2175 2023-06-02 18:33:16.000000 isubrip-2.4.2/isubrip/constants.py
+-rw-rw-rw-   0        0        0     6053 2023-05-26 11:44:57.000000 isubrip-2.4.2/isubrip/data_structures.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:34:52.653522 isubrip-2.4.2/isubrip/resources/
+-rw-rw-rw-   0        0        0      595 2023-05-23 20:01:27.000000 isubrip-2.4.2/isubrip/resources/default_config.toml
+drwxrwxrwx   0        0        0        0 2023-06-02 18:34:52.656522 isubrip-2.4.2/isubrip/scrapers/
+-rw-rw-rw-   0        0        0        0 2023-05-26 10:40:55.000000 isubrip-2.4.2/isubrip/scrapers/__init__.py
+-rw-rw-rw-   0        0        0    15845 2023-05-30 20:51:32.000000 isubrip-2.4.2/isubrip/scrapers/appletv_scraper.py
+-rw-rw-rw-   0        0        0     4334 2023-06-02 14:55:15.000000 isubrip-2.4.2/isubrip/scrapers/itunes_scraper.py
+-rw-rw-rw-   0        0        0    22271 2023-06-02 18:33:16.000000 isubrip-2.4.2/isubrip/scrapers/scraper.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:34:52.660525 isubrip-2.4.2/isubrip/subtitle_formats/
+-rw-rw-rw-   0        0        0        0 2023-05-24 22:34:46.000000 isubrip-2.4.2/isubrip/subtitle_formats/__init__.py
+-rw-rw-rw-   0        0        0     1383 2023-05-26 11:44:57.000000 isubrip-2.4.2/isubrip/subtitle_formats/subrip.py
+-rw-rw-rw-   0        0        0     7909 2023-05-26 11:44:57.000000 isubrip-2.4.2/isubrip/subtitle_formats/subtitles.py
+-rw-rw-rw-   0        0        0     9220 2023-05-26 11:44:57.000000 isubrip-2.4.2/isubrip/subtitle_formats/webvtt.py
+-rw-rw-rw-   0        0        0    13341 2023-06-02 14:19:57.000000 isubrip-2.4.2/isubrip/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-02 18:34:52.652525 isubrip-2.4.2/isubrip.egg-info/
+-rw-rw-rw-   0        0        0     3536 2023-06-02 18:34:52.000000 isubrip-2.4.2/isubrip.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      663 2023-06-02 18:34:52.000000 isubrip-2.4.2/isubrip.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 18:34:52.000000 isubrip-2.4.2/isubrip.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-02 18:34:52.000000 isubrip-2.4.2/isubrip.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       38 2023-06-02 18:34:52.000000 isubrip-2.4.2/isubrip.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-02 18:34:52.000000 isubrip-2.4.2/isubrip.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       83 2023-05-26 11:45:14.000000 isubrip-2.4.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-02 18:34:52.664036 isubrip-2.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     2815 2023-05-26 11:44:57.000000 isubrip-2.4.2/setup.py
```

### Comparing `isubrip-2.4.1/LICENSE` & `isubrip-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `isubrip-2.4.1/PKG-INFO` & `isubrip-2.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isubrip
-Version: 2.4.1
+Version: 2.4.2
 Summary: A Python package for scraping and downloading subtitles from iTunes movie pages.
 Home-page: https://github.com/MichaelYochpaz/iSubRip
 Author: Michael Yochpaz
 License: MIT
 Project-URL: Bug Reports, https://github.com/MichaelYochpaz/iSubRip/issues
 Project-URL: Source, https://github.com/MichaelYochpaz/iSubRip
 Keywords: iTunes,AppleTV,movies,subtitles,scrape,scraper,download,m3u8
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # iSubRip
 A Python package for scraping and downloading subtitles from AppleTV / iTunes movie pages.  
-Latest version: 2.4.1 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))  
+Latest version: 2.4.2 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))  
 
 <br/>
   
 [![PyPI - Version](https://img.shields.io/pypi/v/isubrip)](https://python.org/pypi/isubrip)
 [![PyPI - Monthly Downloads](https://pepy.tech/badge/isubrip/month)](https://python.org/pypi/isubrip)
 [![PyPI - Total Downloads](https://pepy.tech/badge/isubrip)](https://python.org/pypi/isubrip)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/isubrip)](https://python.org/pypi/isubrip)
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: isubrip Version: 2.4.1 Summary: A Python package
+Metadata-Version: 2.1 Name: isubrip Version: 2.4.2 Summary: A Python package
 for scraping and downloading subtitles from iTunes movie pages. Home-page:
 https://github.com/MichaelYochpaz/iSubRip Author: Michael Yochpaz License: MIT
 Project-URL: Bug Reports, https://github.com/MichaelYochpaz/iSubRip/issues
 Project-URL: Source, https://github.com/MichaelYochpaz/iSubRip Keywords:
 iTunes,AppleTV,movies,subtitles,scrape,scraper,download,m3u8 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 End Users/Desktop Classifier: Intended Audience :: Developers Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Python: >=3.8 Description-Content-Type:
 text/markdown License-File: LICENSE # iSubRip A Python package for scraping and
-downloading subtitles from AppleTV / iTunes movie pages. Latest version: 2.4.1
+downloading subtitles from AppleTV / iTunes movie pages. Latest version: 2.4.2
 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))
 
 [![PyPI - Version](https://img.shields.io/pypi/v/isubrip)](https://python.org/
 pypi/isubrip) [![PyPI - Monthly Downloads](https://pepy.tech/badge/isubrip/
 month)](https://python.org/pypi/isubrip) [![PyPI - Total Downloads](https://
 pepy.tech/badge/isubrip)](https://python.org/pypi/isubrip) [![PyPI - Python
 Version](https://img.shields.io/pypi/pyversions/isubrip)](https://python.org/
```

### Comparing `isubrip-2.4.1/README.md` & `isubrip-2.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # iSubRip
 A Python package for scraping and downloading subtitles from AppleTV / iTunes movie pages.  
-Latest version: 2.4.1 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))  
+Latest version: 2.4.2 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))  
 
 <br/>
   
 [![PyPI - Version](https://img.shields.io/pypi/v/isubrip)](https://python.org/pypi/isubrip)
 [![PyPI - Monthly Downloads](https://pepy.tech/badge/isubrip/month)](https://python.org/pypi/isubrip)
 [![PyPI - Total Downloads](https://pepy.tech/badge/isubrip)](https://python.org/pypi/isubrip)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/isubrip)](https://python.org/pypi/isubrip)
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # iSubRip A Python package for scraping and downloading subtitles from AppleTV
-/ iTunes movie pages. Latest version: 2.4.1 ([changelog](https://github.com/
+/ iTunes movie pages. Latest version: 2.4.2 ([changelog](https://github.com/
 MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))
 [![PyPI - Version](https://img.shields.io/pypi/v/isubrip)](https://python.org/
 pypi/isubrip) [![PyPI - Monthly Downloads](https://pepy.tech/badge/isubrip/
 month)](https://python.org/pypi/isubrip) [![PyPI - Total Downloads](https://
 pepy.tech/badge/isubrip)](https://python.org/pypi/isubrip) [![PyPI - Python
 Version](https://img.shields.io/pypi/pyversions/isubrip)](https://python.org/
 pypi/isubrip) [![GitHub - License](https://img.shields.io/github/license/
```

### Comparing `isubrip-2.4.1/isubrip/__main__.py` & `isubrip-2.4.2/isubrip/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 from pathlib import Path
 
 import requests
 from requests.utils import default_user_agent
 
 from isubrip.config import Config, ConfigException
-from isubrip.constants import ARCHIVE_FORMAT, DATA_FOLDER_PATH, DEFAULT_CONFIG_PATH, DEFAULT_CONFIG_SETTINGS, \
+from isubrip.constants import ARCHIVE_FORMAT, DATA_FOLDER_PATH, DEFAULT_CONFIG_PATH, BASE_CONFIG_SETTINGS, \
     PACKAGE_NAME, TEMP_FOLDER_PATH, USER_CONFIG_FILE
 from isubrip.data_structures import EpisodeData,  MediaData, MovieData, SubtitlesDownloadResults, SubtitlesData
 from isubrip.scrapers.scraper import Scraper, ScraperFactory
 from isubrip.utils import download_subtitles_to_file, generate_non_conflicting_path, generate_release_name, \
     single_to_list
 
 
@@ -87,23 +87,25 @@
                             print(message)
                             continue
 
                         results = download_subtitles(media_data=media_item,
                                                      **download_media_subtitles_args)
 
                         success_count = len(results.successful_subtitles)
+                        failed_count = len(results.failed_subtitles)
 
-                        if not success_count:
-                            print("No matching subtitles were found.")
-                            continue
+                        if success_count:
+                            print(f"\n{success_count}/{success_count + failed_count} matching subtitles "
+                                  f"have been successfully downloaded.")
+
+                        elif failed_count:
+                            print(f"\n{failed_count} subtitles were matched, but failed to download.")
 
                         else:
-                            failed_count = len(results.failed_subtitles)
-                            print(f"\n{success_count}/{success_count + failed_count} matching subtitles "
-                                  f"have been successfully downloaded.", sep='')
+                            print("\nNo matching subtitles were found.")
 
                     except Exception as e:
                         if multiple_media_items:
                             print(f"Error: Encountered an error while scraping playlist for {media_id}: {e}")
                             continue
 
                         else:
@@ -183,58 +185,59 @@
     temp_downloads: list[Path] = []
 
     playlist = single_to_list(media_data.playlist)[0]
 
     for subtitles_data in media_data.scraper.get_subtitles(main_playlist=playlist.data,
                                                            language_filter=language_filter,
                                                            subrip_conversion=convert_to_srt):
+        language_data = f"{subtitles_data.language_name} ({subtitles_data.language_code})"
+
         try:
             temp_downloads.append(download_subtitles_to_file(
                 media_data=media_data,
                 subtitles_data=subtitles_data,
                 output_path=temp_download_path,
                 overwrite=overwrite_existing,
             ))
 
-            successful_downloads.append(subtitles_data)
-            language_data = f"{subtitles_data.language_name} ({subtitles_data.language_code})"
-
             print(f"{language_data} subtitles were successfully downloaded.")
+            successful_downloads.append(subtitles_data)
 
-        except Exception:
+        except Exception as e:
+            print(f"Error: Failed to download '{language_data}' subtitles: {e}")
             failed_downloads.append(subtitles_data)
             continue
 
     if not zip_files or len(temp_downloads) == 1:
         for file_path in temp_downloads:
             if overwrite_existing:
                 new_path = download_path / file_path.name
 
             else:
                 new_path = generate_non_conflicting_path(download_path / file_path.name)
 
-            # str conversion needed only for Python 3.8 - https://github.com/python/cpython/issues/76870
+            # str conversion needed only for Python <= 3.8 - https://github.com/python/cpython/issues/76870
             shutil.move(src=str(file_path), dst=new_path)
 
-    else:
+    elif len(temp_downloads) > 0:
         archive_path = Path(shutil.make_archive(
             base_name=str(temp_download_path.parent / temp_download_path.name),
             format=ARCHIVE_FORMAT,
             root_dir=temp_download_path,
         ))
 
         file_name = generate_media_folder_name(media_data=media_data) + f".{ARCHIVE_FORMAT}"
 
         if overwrite_existing:
             destination_path = download_path / file_name
 
         else:
             destination_path = generate_non_conflicting_path(download_path / file_name)
 
-        archive_path.replace(destination_path)
+        shutil.move(src=str(archive_path), dst=destination_path)
 
     shutil.rmtree(temp_download_path)
     atexit.unregister(shutil.rmtree)
 
     return SubtitlesDownloadResults(
         media_data=media_data,
         successful_subtitles=successful_downloads,
@@ -265,15 +268,15 @@
         DATA_FOLDER_PATH.mkdir(parents=True, exist_ok=True)
 
     else:
         # If a user config file exists, add it to config_files
         if USER_CONFIG_FILE.is_file():
             config_files.append(USER_CONFIG_FILE)
 
-    config = Config(config_settings=DEFAULT_CONFIG_SETTINGS)
+    config = Config(config_settings=BASE_CONFIG_SETTINGS)
 
     for file_path in config_files:
         with open(file_path, 'r') as data:
             config.loads(config_data=data.read(), check_config=True)
 
     config.check()
     return config
```

### Comparing `isubrip-2.4.1/isubrip/config.py` & `isubrip-2.4.2/isubrip/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,27 +128,28 @@
         """
         return self._config_data.get(key, default)
 
     @property
     def data(self):
         return self._config_data
 
-    def add_settings(self, config_settings: list[ConfigSetting],
+    def add_settings(self, config_settings: ConfigSetting | list[ConfigSetting],
                      duplicate_behavior: DuplicateBehavior = DuplicateBehavior.OVERWRITE,
                      check_config: bool = True) -> None:
         """
         Add new config settings to the config.
 
         Args:
-            config_settings (list[ConfigSetting]): A list of ConfigSettings objects to add to the config.
+            config_settings (ConfigSetting | list[ConfigSetting]): A ConfigSetting object or a list of ConfigSetting
+                objects to add to the config.
             duplicate_behavior (DuplicateBehavior, optional): Behaviour to apply if a duplicate is found.
                 Defaults to DuplicateBehavior.OVERWRITE.
             check_config (bool, optional): Whether to check the config after loading it. Defaults to True.
         """
-        config_settings_copy = deepcopy(config_settings)
+        config_settings_copy = deepcopy(single_to_list(config_settings))
 
         for config_setting in config_settings_copy:
             if config_setting in self._config_settings:
                 if duplicate_behavior == DuplicateBehavior.OVERWRITE:
                     self._config_settings.remove(config_setting)
                     self._config_settings.append(config_setting)
```

### Comparing `isubrip-2.4.1/isubrip/constants.py` & `isubrip-2.4.2/isubrip/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 DATA_FOLDER_PATH = Path.home() / f".{PACKAGE_NAME}"
 SCRAPER_MODULES_SUFFIX = "_scraper"
 USER_CONFIG_FILE_NAME = "config.toml"
 USER_CONFIG_FILE = DATA_FOLDER_PATH / USER_CONFIG_FILE_NAME
 TEMP_FOLDER_PATH = Path(gettempdir()) / PACKAGE_NAME
 
 # Config
-DEFAULT_CONFIG_SETTINGS = [
+BASE_CONFIG_SETTINGS = [
     ConfigSetting(
         key="check-for-updates",
         type=bool,
         category="general",
         required=False,
     ),
     ConfigSetting(
```

### Comparing `isubrip-2.4.1/isubrip/data_structures.py` & `isubrip-2.4.2/isubrip/data_structures.py`

 * *Files identical despite different names*

### Comparing `isubrip-2.4.1/isubrip/resources/default_config.toml` & `isubrip-2.4.2/isubrip/resources/default_config.toml`

 * *Files identical despite different names*

### Comparing `isubrip-2.4.1/isubrip/scrapers/appletv_scraper.py` & `isubrip-2.4.2/isubrip/scrapers/appletv_scraper.py`

 * *Files identical despite different names*

### Comparing `isubrip-2.4.1/isubrip/scrapers/itunes_scraper.py` & `isubrip-2.4.2/isubrip/scrapers/itunes_scraper.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     url_regex = r"(?P<base_url>https?://itunes\.apple\.com/(?:(?P<country_code>[a-z]{2})/)?(?P<media_type>movie|tv-show|tv-season|show)/(?:(?P<media_name>[\w\-%]+)/)?(?P<media_id>id\d{9,10}))(?:\?(?P<url_params>(?:).*))?"  # noqa: E501
     subtitles_class = WebVTTSubtitles
     is_movie_scraper = True
     uses_scrapers = ["appletv"]
 
     def __init__(self, config_data: dict | None = None):
         super().__init__(config_data=config_data)
-        self._config_data = config_data
         self._appletv_scraper = ScraperFactory().get_scraper_instance(scraper_id="appletv",
                                                                       config_data=self._config_data,
                                                                       raise_error=True)
 
     def get_data(self, url: str) -> MovieData:
         """
         Scrape iTunes to find info about a movie, and it's M3U8 main_playlist.
```

### Comparing `isubrip-2.4.1/isubrip/scrapers/scraper.py` & `isubrip-2.4.2/isubrip/scrapers/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
         """
         Initialize a Scraper object.
 
         Args:
             config_data (dict | None, optional): A dictionary containing scraper's configuration data. Defaults to None.
         """
         self._session = requests.Session()
+        self._config_data = config_data
         self.config = Config(config_data=config_data.get(self.id) if config_data else None)
 
         self.config.add_settings([
             ConfigSetting(
                 key="user-agent",
                 type=str,
                 required=False,
```

### Comparing `isubrip-2.4.1/isubrip/subtitle_formats/subrip.py` & `isubrip-2.4.2/isubrip/subtitle_formats/subrip.py`

 * *Files identical despite different names*

### Comparing `isubrip-2.4.1/isubrip/subtitle_formats/subtitles.py` & `isubrip-2.4.2/isubrip/subtitle_formats/subtitles.py`

 * *Files identical despite different names*

### Comparing `isubrip-2.4.1/isubrip/subtitle_formats/webvtt.py` & `isubrip-2.4.2/isubrip/subtitle_formats/webvtt.py`

 * *Files identical despite different names*

### Comparing `isubrip-2.4.1/isubrip/utils.py` & `isubrip-2.4.2/isubrip/utils.py`

 * *Files identical despite different names*

### Comparing `isubrip-2.4.1/isubrip.egg-info/PKG-INFO` & `isubrip-2.4.2/isubrip.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isubrip
-Version: 2.4.1
+Version: 2.4.2
 Summary: A Python package for scraping and downloading subtitles from iTunes movie pages.
 Home-page: https://github.com/MichaelYochpaz/iSubRip
 Author: Michael Yochpaz
 License: MIT
 Project-URL: Bug Reports, https://github.com/MichaelYochpaz/iSubRip/issues
 Project-URL: Source, https://github.com/MichaelYochpaz/iSubRip
 Keywords: iTunes,AppleTV,movies,subtitles,scrape,scraper,download,m3u8
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # iSubRip
 A Python package for scraping and downloading subtitles from AppleTV / iTunes movie pages.  
-Latest version: 2.4.1 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))  
+Latest version: 2.4.2 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))  
 
 <br/>
   
 [![PyPI - Version](https://img.shields.io/pypi/v/isubrip)](https://python.org/pypi/isubrip)
 [![PyPI - Monthly Downloads](https://pepy.tech/badge/isubrip/month)](https://python.org/pypi/isubrip)
 [![PyPI - Total Downloads](https://pepy.tech/badge/isubrip)](https://python.org/pypi/isubrip)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/isubrip)](https://python.org/pypi/isubrip)
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: isubrip Version: 2.4.1 Summary: A Python package
+Metadata-Version: 2.1 Name: isubrip Version: 2.4.2 Summary: A Python package
 for scraping and downloading subtitles from iTunes movie pages. Home-page:
 https://github.com/MichaelYochpaz/iSubRip Author: Michael Yochpaz License: MIT
 Project-URL: Bug Reports, https://github.com/MichaelYochpaz/iSubRip/issues
 Project-URL: Source, https://github.com/MichaelYochpaz/iSubRip Keywords:
 iTunes,AppleTV,movies,subtitles,scrape,scraper,download,m3u8 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 End Users/Desktop Classifier: Intended Audience :: Developers Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Python: >=3.8 Description-Content-Type:
 text/markdown License-File: LICENSE # iSubRip A Python package for scraping and
-downloading subtitles from AppleTV / iTunes movie pages. Latest version: 2.4.1
+downloading subtitles from AppleTV / iTunes movie pages. Latest version: 2.4.2
 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))
 
 [![PyPI - Version](https://img.shields.io/pypi/v/isubrip)](https://python.org/
 pypi/isubrip) [![PyPI - Monthly Downloads](https://pepy.tech/badge/isubrip/
 month)](https://python.org/pypi/isubrip) [![PyPI - Total Downloads](https://
 pepy.tech/badge/isubrip)](https://python.org/pypi/isubrip) [![PyPI - Python
 Version](https://img.shields.io/pypi/pyversions/isubrip)](https://python.org/
```

### Comparing `isubrip-2.4.1/isubrip.egg-info/SOURCES.txt` & `isubrip-2.4.2/isubrip.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `isubrip-2.4.1/setup.py` & `isubrip-2.4.2/setup.py`

 * *Files identical despite different names*

