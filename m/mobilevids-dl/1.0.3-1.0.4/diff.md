# Comparing `tmp/mobilevids-dl-1.0.3.tar.gz` & `tmp/mobilevids-dl-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobilevids-dl-1.0.3.tar", last modified: Tue May 30 21:21:30 2023, max compression
+gzip compressed data, was "mobilevids-dl-1.0.4.tar", last modified: Fri Jun  2 08:10:50 2023, max compression
```

## Comparing `mobilevids-dl-1.0.3.tar` & `mobilevids-dl-1.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:21:30.175266 mobilevids-dl-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-30 21:21:13.000000 mobilevids-dl-1.0.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-30 21:21:13.000000 mobilevids-dl-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-30 21:21:13.000000 mobilevids-dl-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-05-30 21:21:30.171265 mobilevids-dl-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-05-30 21:21:13.000000 mobilevids-dl-1.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:21:30.171265 mobilevids-dl-1.0.3/mobilevids/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-30 21:21:13.000000 mobilevids-dl-1.0.3/mobilevids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-30 21:21:13.000000 mobilevids-dl-1.0.3/mobilevids/define.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1121 2023-05-30 21:21:13.000000 mobilevids-dl-1.0.3/mobilevids/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-05-30 21:21:13.000000 mobilevids-dl-1.0.3/mobilevids/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-30 21:21:13.000000 mobilevids-dl-1.0.3/mobilevids/imagetoascii.py
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-05-30 21:21:13.000000 mobilevids-dl-1.0.3/mobilevids/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-30 21:21:13.000000 mobilevids-dl-1.0.3/mobilevids/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:21:30.171265 mobilevids-dl-1.0.3/mobilevids_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-05-30 21:21:30.000000 mobilevids-dl-1.0.3/mobilevids_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-30 21:21:30.000000 mobilevids-dl-1.0.3/mobilevids_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 21:21:30.000000 mobilevids-dl-1.0.3/mobilevids_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-30 21:21:30.000000 mobilevids-dl-1.0.3/mobilevids_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-30 21:21:30.000000 mobilevids-dl-1.0.3/mobilevids_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-30 21:21:30.000000 mobilevids-dl-1.0.3/mobilevids_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-30 21:21:13.000000 mobilevids-dl-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 21:21:30.175266 mobilevids-dl-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-30 21:21:13.000000 mobilevids-dl-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:50.387296 mobilevids-dl-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-02 08:10:33.000000 mobilevids-dl-1.0.4/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-02 08:10:34.000000 mobilevids-dl-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-02 08:10:34.000000 mobilevids-dl-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-06-02 08:10:50.387296 mobilevids-dl-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-06-02 08:10:34.000000 mobilevids-dl-1.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:50.383296 mobilevids-dl-1.0.4/mobilevids/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-02 08:10:34.000000 mobilevids-dl-1.0.4/mobilevids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-02 08:10:34.000000 mobilevids-dl-1.0.4/mobilevids/define.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1121 2023-06-02 08:10:34.000000 mobilevids-dl-1.0.4/mobilevids/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-02 08:10:34.000000 mobilevids-dl-1.0.4/mobilevids/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-02 08:10:34.000000 mobilevids-dl-1.0.4/mobilevids/imagetoascii.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-06-02 08:10:34.000000 mobilevids-dl-1.0.4/mobilevids/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-02 08:10:34.000000 mobilevids-dl-1.0.4/mobilevids/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:10:50.387296 mobilevids-dl-1.0.4/mobilevids_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-06-02 08:10:50.000000 mobilevids-dl-1.0.4/mobilevids_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-02 08:10:50.000000 mobilevids-dl-1.0.4/mobilevids_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 08:10:50.000000 mobilevids-dl-1.0.4/mobilevids_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-02 08:10:50.000000 mobilevids-dl-1.0.4/mobilevids_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-02 08:10:50.000000 mobilevids-dl-1.0.4/mobilevids_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-02 08:10:50.000000 mobilevids-dl-1.0.4/mobilevids_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-02 08:10:34.000000 mobilevids-dl-1.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 08:10:50.387296 mobilevids-dl-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-02 08:10:34.000000 mobilevids-dl-1.0.4/setup.py
```

### Comparing `mobilevids-dl-1.0.3/AUTHORS.md` & `mobilevids-dl-1.0.4/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `mobilevids-dl-1.0.3/LICENSE` & `mobilevids-dl-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mobilevids-dl-1.0.3/PKG-INFO` & `mobilevids-dl-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobilevids-dl
-Version: 1.0.3
+Version: 1.0.4
 Summary: Script for downloading Movies and Shows from mobilevids.org
 Home-page: https://github.com/ahron-maslin/mobilevids-dl
 Maintainer: Aharon Maslin
 Maintainer-email: aronmas613@gmail.com
 License: LGPL
 Keywords: mpbilevids-dl,mobilevids,download,entertainment,video
 Platform: any
```

### Comparing `mobilevids-dl-1.0.3/README.rst` & `mobilevids-dl-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `mobilevids-dl-1.0.3/mobilevids/define.py` & `mobilevids-dl-1.0.4/mobilevids/define.py`

 * *Files identical despite different names*

### Comparing `mobilevids-dl-1.0.3/mobilevids/dispatcher.py` & `mobilevids-dl-1.0.4/mobilevids/dispatcher.py`

 * *Files identical despite different names*

### Comparing `mobilevids-dl-1.0.3/mobilevids/downloader.py` & `mobilevids-dl-1.0.4/mobilevids/downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,16 +121,14 @@
 			logging.info(f"Name: {movie_json['title']}\n"
 									 f"ID: {movie_json['id']}\n"
 									 f"Year: {movie_json['year']}\n"
 									 f"Description: {movie_json['plot']}")
 
 		logging.info(f'[*] Downloading {movie_json["title"]} ({movie_json["year"]})')
 		self.dl_obj = dl_wrapper(self.get_quality(movie_json), self.download_dir)
-		if self.dl_obj:
-			self.dl_obj.start()
 
 
 	def get_show_by_id(self, show_id: str, season_chosen=None):
 		"""
     Downloads the TV show with the given ID and prompts the user to select a season to download.
 
     Args:
@@ -166,39 +164,39 @@
         show_id (str): The ID of the TV show to download.
         season (str): The season number of the episode.
         episode (str): The episode number of the episode.
         path (str): The directory where the downloaded file will be saved.
     """
 		episode_info = get_json(self.session, GET_SINGLE_EPISODE_URL.format(self.user_id, self.auth_token, show_id, season, episode))
 		self.dl_obj = dl_wrapper(self.get_quality(episode_info), path)
-		if self.dl_obj:
-			self.dl_obj.start()
 
 
 	def signal_handler(self, sig, frame):
 		"""
     Handles keyboard interrupts during file downloads and removes incomplete downloads.
 
     Args:
         sig: The signal number.
         frame: The interrupted stack frame.
     """
 		logging.debug('SIGINT captured')
 		if self.dl_obj:
 			self.dl_obj.stop()
+		"""
 		for file in os.listdir(self.download_dir):
-			if file.endswith(".00", -4, -1):
+			if file.endswith(".part", -4, -1):
 				'''
-				  Smart_DL downloads file in chunks ending in ".00x" 
+				  pypdl downloads file in chunks ending in ".part" 
 					where x is a number corresponding to the thread that is being used
 				'''
 				filepath = os.path.join(self.download_dir, file)
 				os.remove(filepath)
 		if self.download_dir and len(os.listdir(self.download_dir)) == 0 and self.download_dir is not DOWNLOAD_DIRECTORY:
 			'''
 			remove download dir if not the default directory
 			'''
 			logging.debug(f'Removing {self.download_dir}')
 			os.rmdir(self.download_dir)
+		"""
 		logging.error('\n[!] CTRL-C pressed - exiting!')
 		exit(1)
```

### Comparing `mobilevids-dl-1.0.3/mobilevids/imagetoascii.py` & `mobilevids-dl-1.0.4/mobilevids/imagetoascii.py`

 * *Files identical despite different names*

### Comparing `mobilevids-dl-1.0.3/mobilevids/network.py` & `mobilevids-dl-1.0.4/mobilevids/network.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import requests
 import netrc
 import json
 from json import JSONDecodeError
 from wget import detect_filename
 import os
 import logging
-from pySmartDL import SmartDL
+from pypdl import Downloader as mtdl
 
 from .define import LOGIN_PAYLOAD, LOGIN_URL, HEADERS, AUTH_TOKEN_CACHE, GET_VIDEO_URL, NETRC_FILE_PATH
 
 
 def check_auth_cache(cached_auth_file):
 	"""
 	Check if cached auth file exists, and return its content as a string.
@@ -103,33 +103,34 @@
 	logging.debug(login_info)
 	logging.info('[*] Successfully logged in!')
 	return login_info['auth_token'], login_info['id']
 
 
 def dl_wrapper(video: str, folder):  
 	"""
-	Wrapper function for the SmartDL module.
+	Wrapper function for the pypdl module.
 
 	Args:
 		video: The URL of the video to download.
 		folder: The path to the folder in which to save the downloaded video.
 
 	Returns:
-		A SmartDL object that can be used to download the video.
+		A pypdl object that can be used to download the video.
 	"""
-	if not os.path.exists(folder): # remove this? smart_DL takes care of it
+	if not os.path.exists(folder): # remove this? pypdl takes care of it
 		os.mkdir(folder)
 
 	filename = detect_filename(video)
 	save_path = folder + filename
 
 	if not os.path.isfile(save_path):
 		logging.debug(f'Save path {save_path}')
 		logging.info(f'Downloading {filename} to {folder}')
-		dl_obj = SmartDL(video, save_path, threads=(os.cpu_count()-2))
+		dl_obj = mtdl()
+		dl_obj.start(url=video, filepath=save_path, num_connections=(os.cpu_count()-2), retries=3)
 		return dl_obj
 	
 	return None
 
 
 def get_json(session, url: str) -> dict:
 	"""
```

### Comparing `mobilevids-dl-1.0.3/mobilevids/options.py` & `mobilevids-dl-1.0.4/mobilevids/options.py`

 * *Files identical despite different names*

### Comparing `mobilevids-dl-1.0.3/mobilevids_dl.egg-info/PKG-INFO` & `mobilevids-dl-1.0.4/mobilevids_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobilevids-dl
-Version: 1.0.3
+Version: 1.0.4
 Summary: Script for downloading Movies and Shows from mobilevids.org
 Home-page: https://github.com/ahron-maslin/mobilevids-dl
 Maintainer: Aharon Maslin
 Maintainer-email: aronmas613@gmail.com
 License: LGPL
 Keywords: mpbilevids-dl,mobilevids,download,entertainment,video
 Platform: any
```

### Comparing `mobilevids-dl-1.0.3/setup.py` & `mobilevids-dl-1.0.4/setup.py`

 * *Files identical despite different names*

