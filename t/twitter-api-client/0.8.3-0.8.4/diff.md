# Comparing `tmp/twitter-api-client-0.8.3.tar.gz` & `tmp/twitter-api-client-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.8.3.tar", last modified: Wed May 24 17:53:54 2023, max compression
+gzip compressed data, was "twitter-api-client-0.8.4.tar", last modified: Fri Jun  2 03:04:19 2023, max compression
```

## Comparing `twitter-api-client-0.8.3.tar` & `twitter-api-client-0.8.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-24 17:53:54.817295 twitter-api-client-0.8.3/
--rw-r--r--   0 x         (1000) x         (1000)     1075 2023-04-30 17:24:38.000000 twitter-api-client-0.8.3/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)     8728 2023-05-24 17:53:54.817295 twitter-api-client-0.8.3/PKG-INFO
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-24 17:53:54.813962 twitter-api-client-0.8.3/protonmail/
--rw-r--r--   0 x         (1000) x         (1000)       78 2023-04-13 08:11:01.000000 twitter-api-client-0.8.3/protonmail/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)    24269 2023-04-13 08:11:01.000000 twitter-api-client-0.8.3/protonmail/api.py
--rw-r--r--   0 x         (1000) x         (1000)     5579 2023-04-13 08:11:01.000000 twitter-api-client-0.8.3/protonmail/cert_pinning.py
--rw-r--r--   0 x         (1000) x         (1000)     1589 2023-04-13 08:11:01.000000 twitter-api-client-0.8.3/protonmail/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     1029 2023-04-13 08:11:01.000000 twitter-api-client-0.8.3/protonmail/exceptions.py
--rw-r--r--   0 x         (1000) x         (1000)     1397 2023-04-13 08:11:01.000000 twitter-api-client-0.8.3/protonmail/logger.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-24 17:53:54.813962 twitter-api-client-0.8.3/protonmail/metadata/
--rw-r--r--   0 x         (1000) x         (1000)      106 2023-04-13 08:11:01.000000 twitter-api-client-0.8.3/protonmail/metadata/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)     1225 2023-04-13 08:11:01.000000 twitter-api-client-0.8.3/protonmail/metadata/_base.py
--rw-r--r--   0 x         (1000) x         (1000)     3432 2023-04-13 08:11:01.000000 twitter-api-client-0.8.3/protonmail/metadata/textfile_metadata.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-24 17:53:54.813962 twitter-api-client-0.8.3/protonmail/srp/
--rw-r--r--   0 x         (1000) x         (1000)      172 2023-04-13 08:11:01.000000 twitter-api-client-0.8.3/protonmail/srp/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)     9305 2023-04-13 08:11:01.000000 twitter-api-client-0.8.3/protonmail/srp/_ctsrp.py
--rw-r--r--   0 x         (1000) x         (1000)     4426 2023-04-13 08:11:01.000000 twitter-api-client-0.8.3/protonmail/srp/_pysrp.py
--rw-r--r--   0 x         (1000) x         (1000)      684 2023-04-13 08:11:01.000000 twitter-api-client-0.8.3/protonmail/srp/pmhash.py
--rw-r--r--   0 x         (1000) x         (1000)     1482 2023-04-13 08:11:01.000000 twitter-api-client-0.8.3/protonmail/srp/util.py
--rw-r--r--   0 x         (1000) x         (1000)      962 2023-04-13 08:11:01.000000 twitter-api-client-0.8.3/protonmail/utils.py
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-05-24 17:53:54.817295 twitter-api-client-0.8.3/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)    10269 2023-05-24 17:53:36.000000 twitter-api-client-0.8.3/setup.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-24 17:53:54.817295 twitter-api-client-0.8.3/twitter/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-30 17:24:38.000000 twitter-api-client-0.8.3/twitter/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)    21961 2023-05-23 20:00:03.000000 twitter-api-client-0.8.3/twitter/account.py
--rw-r--r--   0 x         (1000) x         (1000)    27271 2023-04-30 17:24:38.000000 twitter-api-client-0.8.3/twitter/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     7170 2023-05-24 17:52:40.000000 twitter-api-client-0.8.3/twitter/login.py
--rw-r--r--   0 x         (1000) x         (1000)    11982 2023-05-23 19:56:12.000000 twitter-api-client-0.8.3/twitter/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)     5203 2023-05-23 20:00:03.000000 twitter-api-client-0.8.3/twitter/search.py
--rw-r--r--   0 x         (1000) x         (1000)     5805 2023-05-23 23:05:47.000000 twitter-api-client-0.8.3/twitter/util.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-24 17:53:54.817295 twitter-api-client-0.8.3/twitter_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)     8728 2023-05-24 17:53:54.000000 twitter-api-client-0.8.3/twitter_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      740 2023-05-24 17:53:54.000000 twitter-api-client-0.8.3/twitter_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-05-24 17:53:54.000000 twitter-api-client-0.8.3/twitter_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)      118 2023-05-24 17:53:54.000000 twitter-api-client-0.8.3/twitter_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)       19 2023-05-24 17:53:54.000000 twitter-api-client-0.8.3/twitter_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-02 03:04:19.553220 twitter-api-client-0.8.4/
+-rw-r--r--   0 x         (1000) x         (1000)     1075 2023-05-28 16:24:21.000000 twitter-api-client-0.8.4/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)    10964 2023-06-02 03:04:19.553220 twitter-api-client-0.8.4/PKG-INFO
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-02 03:04:19.551220 twitter-api-client-0.8.4/protonmail/
+-rw-r--r--   0 x         (1000) x         (1000)       78 2023-05-28 16:24:21.000000 twitter-api-client-0.8.4/protonmail/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)    24269 2023-05-28 16:24:21.000000 twitter-api-client-0.8.4/protonmail/api.py
+-rw-r--r--   0 x         (1000) x         (1000)     5579 2023-05-28 16:24:21.000000 twitter-api-client-0.8.4/protonmail/cert_pinning.py
+-rw-r--r--   0 x         (1000) x         (1000)     1589 2023-05-28 16:24:21.000000 twitter-api-client-0.8.4/protonmail/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     1029 2023-05-28 16:24:21.000000 twitter-api-client-0.8.4/protonmail/exceptions.py
+-rw-r--r--   0 x         (1000) x         (1000)     1397 2023-05-28 16:24:21.000000 twitter-api-client-0.8.4/protonmail/logger.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-02 03:04:19.551220 twitter-api-client-0.8.4/protonmail/metadata/
+-rw-r--r--   0 x         (1000) x         (1000)      106 2023-05-28 16:24:21.000000 twitter-api-client-0.8.4/protonmail/metadata/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)     1225 2023-05-28 16:24:21.000000 twitter-api-client-0.8.4/protonmail/metadata/_base.py
+-rw-r--r--   0 x         (1000) x         (1000)     3432 2023-05-28 16:24:21.000000 twitter-api-client-0.8.4/protonmail/metadata/textfile_metadata.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-02 03:04:19.551220 twitter-api-client-0.8.4/protonmail/srp/
+-rw-r--r--   0 x         (1000) x         (1000)      172 2023-05-28 16:24:21.000000 twitter-api-client-0.8.4/protonmail/srp/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)     9305 2023-05-28 16:24:21.000000 twitter-api-client-0.8.4/protonmail/srp/_ctsrp.py
+-rw-r--r--   0 x         (1000) x         (1000)     4426 2023-05-28 16:24:21.000000 twitter-api-client-0.8.4/protonmail/srp/_pysrp.py
+-rw-r--r--   0 x         (1000) x         (1000)      684 2023-05-28 16:24:21.000000 twitter-api-client-0.8.4/protonmail/srp/pmhash.py
+-rw-r--r--   0 x         (1000) x         (1000)     1482 2023-05-28 16:24:21.000000 twitter-api-client-0.8.4/protonmail/srp/util.py
+-rw-r--r--   0 x         (1000) x         (1000)      962 2023-05-28 16:24:21.000000 twitter-api-client-0.8.4/protonmail/utils.py
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-02 03:04:19.553220 twitter-api-client-0.8.4/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)    12852 2023-06-02 03:02:38.000000 twitter-api-client-0.8.4/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-02 03:04:19.552220 twitter-api-client-0.8.4/twitter/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-05-28 16:24:21.000000 twitter-api-client-0.8.4/twitter/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)    22968 2023-06-02 01:49:12.000000 twitter-api-client-0.8.4/twitter/account.py
+-rw-r--r--   0 x         (1000) x         (1000)    28454 2023-06-02 01:49:12.000000 twitter-api-client-0.8.4/twitter/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     7350 2023-06-02 01:49:12.000000 twitter-api-client-0.8.4/twitter/login.py
+-rw-r--r--   0 x         (1000) x         (1000)    27552 2023-06-02 01:49:12.000000 twitter-api-client-0.8.4/twitter/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     5960 2023-06-02 01:50:23.000000 twitter-api-client-0.8.4/twitter/search.py
+-rw-r--r--   0 x         (1000) x         (1000)     9198 2023-06-02 01:49:12.000000 twitter-api-client-0.8.4/twitter/util.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-02 03:04:19.553220 twitter-api-client-0.8.4/twitter_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)    10964 2023-06-02 03:04:19.000000 twitter-api-client-0.8.4/twitter_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      740 2023-06-02 03:04:19.000000 twitter-api-client-0.8.4/twitter_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-02 03:04:19.000000 twitter-api-client-0.8.4/twitter_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)      130 2023-06-02 03:04:19.000000 twitter-api-client-0.8.4/twitter_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)       19 2023-06-02 03:04:19.000000 twitter-api-client-0.8.4/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.8.3/LICENSE` & `twitter-api-client-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.3/PKG-INFO` & `twitter-api-client-0.8.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.8.3
+Version: 0.8.4
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-Implementation of Twitter's v1, v2, and GraphQL APIs
+
+## Implementation of Twitter's v1, v2, and GraphQL APIs
 
 Tools include: [Scraping](#scraping), [Account Automation](#automation), [Search](#search)
 
-Automated email challenge solvers are supported for Proton Mail accounts. See [here](#automated-solvers) for more information.
+Automated email challenge solvers are supported for **Proton Mail** accounts using [proton-python-client](https://github.com/ProtonMail/proton-python-client). See [here](#automated-solvers) for more information.
+
+## Table of Contents
 
 * [Installation](#installation)
 * [Automation](#automation)
 * [Scraping](#scraping)
-    * [Users/Tweets data](#get-all-usertweet-data)
-    * [Search](#search)
+  * [Get all user/tweet data](#get-all-usertweet-data)
+  * [Resume Pagination](#resume-pagination)
+  * [Search](#search)
+* [Spaces](#spaces)
+  * [Live Audio Capture](#live-audio-capture)
+  * [Live Transcript Capture](#live-transcript-capture)
+  * [Search and Metadata](#search-and-metadata)
 * [Automated Solvers](#automated-solvers)
 * [Example API Responses](#example-api-responses)
 
 ### Installation
 
 ```bash
 pip install twitter-api-client
@@ -193,15 +201,15 @@
 media = scraper.media([123, 234, 345])
 following = scraper.following([123, 234, 345])
 followers = scraper.followers([123, 234, 345])
 scraper.tweet_stats([111111, 222222, 333333])
 
 # get recommended users based on user
 scraper.recommended_users()
-scraper.recommended_users(123)
+scraper.recommended_users([123])
 
 # tweet data
 tweets_by_ids = scraper.tweets_by_id([987, 876, 754])
 tweets_details = scraper.tweets_details([987, 876, 754])
 retweeters = scraper.retweeters([987, 876, 754])
 favoriters = scraper.favoriters([987, 876, 754])
 
@@ -213,28 +221,26 @@
 ])
 
 # trends
 scraper.trends()
 ```
 
 #### Resume Pagination
-Pagination is already done by default, however there are circumstances where you may need to resume pagination from a specific cursor. For example, the `Followers` endpoint only allows for 50 requests every 15 minutes. In this case, we can resume from where we left off by providing a specific cursor value. This technique applies to any other endpoint defined in `twitter.constants.Operation`.
+**Pagination is already done by default**, however there are circumstances where you may need to resume pagination from a specific cursor. For example, the `Followers` endpoint only allows for 50 requests every 15 minutes. In this case, we can resume from where we left off by providing a specific cursor value.
 ```python
 from twitter.scraper import Scraper
-from twitter.constants import Operation
 
 email, username, password = ...,...,...
 scraper = Scraper(email, username, password, debug=1, save=True)
 
-operation = Operation.Followers
 user_id = 44196397
-cursor = '1765001818576065118|1654241854176100129' # example cursor
-limit = 250  # arbitrary limit for demonstration
+cursor = '1767341853908517597|1663601806447476672'  # example cursor
+limit = 100  # arbitrary limit for demonstration
+follower_subset, last_cursor = scraper.followers([user_id], limit=limit, cursor=cursor)
 
-follower_subset, last_cursor = scraper.resume_pagination(scraper.session, user_id, operation, limit=limit, cursor=cursor)
 # use last_cursor to resume pagination
 ```
 
 #### Search
 
 ```python   
 from twitter.search import Search
@@ -267,21 +273,98 @@
 
 **Search Operators Reference**
 
 https://developer.twitter.com/en/docs/twitter-api/v1/rules-and-filtering/search-operators
 
 https://developer.twitter.com/en/docs/twitter-api/tweets/search/integrate/build-a-query
 
+### Spaces
+
+#### Live Audio Capture
+
+Capture live audio for up to 500 streams per IP
+
+```python
+from twitter.scraper import Scraper
+from twitter.util import init_session
+
+session = init_session() # initialize guest session, no login required
+scraper = Scraper(session=session, debug=1, save=True)
+
+rooms = [...]
+scraper.spaces_live(rooms=rooms) # capture live audio from list of rooms
+```
+
+#### Live Transcript Capture
+
+**Raw transcript chunks**
+
+```python
+from twitter.scraper import Scraper
+from twitter.util import init_session
+
+session = init_session() # initialize guest session, no login required
+scraper = Scraper(session=session, debug=1, save=True)
+
+# room must be live, i.e. in "Running" state
+scraper.space_live_transcript('1zqKVPlQNApJB', frequency=2)  # word-level live transcript. (dirty, on-the-fly transcription before post-processing)
+```
+
+**Processed (final) transcript chunks**
+
+```python
+from twitter.scraper import Scraper
+from twitter.util import init_session
+
+session = init_session() # initialize guest session, no login required
+scraper = Scraper(session=session, debug=1, save=True)
+
+# room must be live, i.e. in "Running" state
+scraper.space_live_transcript('1zqKVPlQNApJB', frequency=1)  # finalized live transcript.  (clean)
+```
+
+#### Search and Metadata
+```python
+from twitter.scraper import Scraper
+from twitter.util import init_session
+from twitter.constants import SpaceCategory
+
+session = init_session() # initialize guest session, no login required
+scraper = Scraper(session=session, debug=1, save=True)
+
+# download audio and chat-log from space
+spaces = scraper.spaces(rooms=['1eaJbrAPnBVJX', '1eaJbrAlZjjJX'], audio=True, chat=True)
+
+# pull metadata only
+spaces = scraper.spaces(rooms=['1eaJbrAPnBVJX', '1eaJbrAlZjjJX'])
+
+# search for spaces in "Upcoming", "Top" and "Live" categories
+spaces = scraper.spaces(search=[
+    {
+        'filter': SpaceCategory.Upcoming,
+        'query': 'hello'
+    },
+    {
+        'filter': SpaceCategory.Top,
+        'query': 'world'
+    },
+    {
+        'filter': SpaceCategory.Live,
+        'query': 'foo bar'
+    }
+])
+```
 
 ### Automated Solvers
 To set up automated email confirmation/verification solvers, add your Proton Mail credentials below as shown.
 This removes the need to manually solve email challenges via the web app. These credentials can be used in `Scraper`, `Account`, and `Search` constructors.
 
 E.g.
 
 ```python
 from twitter.scraper import Scraper
 
 email, username, password = ..., ..., ...
 proton_email, proton_password = ..., ...
 account = Scraper(email, username, password, debug=1, save=True, protonmail={'email':proton_email, 'password':proton_password})
 ```
+
```

### Comparing `twitter-api-client-0.8.3/protonmail/api.py` & `twitter-api-client-0.8.4/protonmail/api.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.3/protonmail/cert_pinning.py` & `twitter-api-client-0.8.4/protonmail/cert_pinning.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.3/protonmail/constants.py` & `twitter-api-client-0.8.4/protonmail/constants.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.3/protonmail/exceptions.py` & `twitter-api-client-0.8.4/protonmail/exceptions.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.3/protonmail/logger.py` & `twitter-api-client-0.8.4/protonmail/logger.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.3/protonmail/metadata/_base.py` & `twitter-api-client-0.8.4/protonmail/metadata/_base.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.3/protonmail/metadata/textfile_metadata.py` & `twitter-api-client-0.8.4/protonmail/metadata/textfile_metadata.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.3/protonmail/srp/_ctsrp.py` & `twitter-api-client-0.8.4/protonmail/srp/_ctsrp.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.3/protonmail/srp/_pysrp.py` & `twitter-api-client-0.8.4/protonmail/srp/_pysrp.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.3/protonmail/srp/pmhash.py` & `twitter-api-client-0.8.4/protonmail/srp/pmhash.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.3/protonmail/srp/util.py` & `twitter-api-client-0.8.4/protonmail/srp/util.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.3/protonmail/utils.py` & `twitter-api-client-0.8.4/protonmail/utils.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.3/setup.py` & `twitter-api-client-0.8.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,50 @@
 from textwrap import dedent
 
 from setuptools import find_packages, setup
 
 install_requires = [
+    "aiofiles",
+    "websockets",
     "nest_asyncio",
-    "aiohttp",
     "httpx",
     "tqdm",
     "orjson",
-    "requests",
     "bcrypt",
     "python-gnupg",
     "pyopenssl",
+    "requests",
     'uvloop; platform_system != "Windows"',
 ]
 
 setup(
     name="twitter-api-client",
-    version="0.8.3",
+    version="0.8.4",
     python_requires=">=3.10.10",
     description="Twitter API",
     long_description=dedent('''
-    Implementation of Twitter's v1, v2, and GraphQL APIs
     
+    ## Implementation of Twitter's v1, v2, and GraphQL APIs
+
     Tools include: [Scraping](#scraping), [Account Automation](#automation), [Search](#search)
     
-    Automated email challenge solvers are supported for Proton Mail accounts. See [here](#automated-solvers) for more information.
+    Automated email challenge solvers are supported for **Proton Mail** accounts using [proton-python-client](https://github.com/ProtonMail/proton-python-client). See [here](#automated-solvers) for more information.
+    
+    ## Table of Contents
     
     * [Installation](#installation)
     * [Automation](#automation)
     * [Scraping](#scraping)
-        * [Users/Tweets data](#get-all-usertweet-data)
-        * [Search](#search)
+      * [Get all user/tweet data](#get-all-usertweet-data)
+      * [Resume Pagination](#resume-pagination)
+      * [Search](#search)
+    * [Spaces](#spaces)
+      * [Live Audio Capture](#live-audio-capture)
+      * [Live Transcript Capture](#live-transcript-capture)
+      * [Search and Metadata](#search-and-metadata)
     * [Automated Solvers](#automated-solvers)
     * [Example API Responses](#example-api-responses)
     
     ### Installation
     
     ```bash
     pip install twitter-api-client
@@ -203,15 +212,15 @@
     media = scraper.media([123, 234, 345])
     following = scraper.following([123, 234, 345])
     followers = scraper.followers([123, 234, 345])
     scraper.tweet_stats([111111, 222222, 333333])
     
     # get recommended users based on user
     scraper.recommended_users()
-    scraper.recommended_users(123)
+    scraper.recommended_users([123])
     
     # tweet data
     tweets_by_ids = scraper.tweets_by_id([987, 876, 754])
     tweets_details = scraper.tweets_details([987, 876, 754])
     retweeters = scraper.retweeters([987, 876, 754])
     favoriters = scraper.favoriters([987, 876, 754])
     
@@ -223,28 +232,26 @@
     ])
     
     # trends
     scraper.trends()
     ```
     
     #### Resume Pagination
-    Pagination is already done by default, however there are circumstances where you may need to resume pagination from a specific cursor. For example, the `Followers` endpoint only allows for 50 requests every 15 minutes. In this case, we can resume from where we left off by providing a specific cursor value. This technique applies to any other endpoint defined in `twitter.constants.Operation`.
+    **Pagination is already done by default**, however there are circumstances where you may need to resume pagination from a specific cursor. For example, the `Followers` endpoint only allows for 50 requests every 15 minutes. In this case, we can resume from where we left off by providing a specific cursor value.
     ```python
     from twitter.scraper import Scraper
-    from twitter.constants import Operation
     
     email, username, password = ...,...,...
     scraper = Scraper(email, username, password, debug=1, save=True)
     
-    operation = Operation.Followers
     user_id = 44196397
-    cursor = '1765001818576065118|1654241854176100129' # example cursor
-    limit = 250  # arbitrary limit for demonstration
+    cursor = '1767341853908517597|1663601806447476672'  # example cursor
+    limit = 100  # arbitrary limit for demonstration
+    follower_subset, last_cursor = scraper.followers([user_id], limit=limit, cursor=cursor)
     
-    follower_subset, last_cursor = scraper.resume_pagination(scraper.session, user_id, operation, limit=limit, cursor=cursor)
     # use last_cursor to resume pagination
     ```
     
     #### Search
     
     ```python   
     from twitter.search import Search
@@ -277,28 +284,105 @@
     
     **Search Operators Reference**
     
     https://developer.twitter.com/en/docs/twitter-api/v1/rules-and-filtering/search-operators
     
     https://developer.twitter.com/en/docs/twitter-api/tweets/search/integrate/build-a-query
     
+    ### Spaces
+    
+    #### Live Audio Capture
+    
+    Capture live audio for up to 500 streams per IP
+    
+    ```python
+    from twitter.scraper import Scraper
+    from twitter.util import init_session
+    
+    session = init_session() # initialize guest session, no login required
+    scraper = Scraper(session=session, debug=1, save=True)
+    
+    rooms = [...]
+    scraper.spaces_live(rooms=rooms) # capture live audio from list of rooms
+    ```
+    
+    #### Live Transcript Capture
+    
+    **Raw transcript chunks**
+    
+    ```python
+    from twitter.scraper import Scraper
+    from twitter.util import init_session
+    
+    session = init_session() # initialize guest session, no login required
+    scraper = Scraper(session=session, debug=1, save=True)
+    
+    # room must be live, i.e. in "Running" state
+    scraper.space_live_transcript('1zqKVPlQNApJB', frequency=2)  # word-level live transcript. (dirty, on-the-fly transcription before post-processing)
+    ```
+    
+    **Processed (final) transcript chunks**
+    
+    ```python
+    from twitter.scraper import Scraper
+    from twitter.util import init_session
+    
+    session = init_session() # initialize guest session, no login required
+    scraper = Scraper(session=session, debug=1, save=True)
+    
+    # room must be live, i.e. in "Running" state
+    scraper.space_live_transcript('1zqKVPlQNApJB', frequency=1)  # finalized live transcript.  (clean)
+    ```
+    
+    #### Search and Metadata
+    ```python
+    from twitter.scraper import Scraper
+    from twitter.util import init_session
+    from twitter.constants import SpaceCategory
+    
+    session = init_session() # initialize guest session, no login required
+    scraper = Scraper(session=session, debug=1, save=True)
+    
+    # download audio and chat-log from space
+    spaces = scraper.spaces(rooms=['1eaJbrAPnBVJX', '1eaJbrAlZjjJX'], audio=True, chat=True)
+    
+    # pull metadata only
+    spaces = scraper.spaces(rooms=['1eaJbrAPnBVJX', '1eaJbrAlZjjJX'])
+    
+    # search for spaces in "Upcoming", "Top" and "Live" categories
+    spaces = scraper.spaces(search=[
+        {
+            'filter': SpaceCategory.Upcoming,
+            'query': 'hello'
+        },
+        {
+            'filter': SpaceCategory.Top,
+            'query': 'world'
+        },
+        {
+            'filter': SpaceCategory.Live,
+            'query': 'foo bar'
+        }
+    ])
+    ```
     
     ### Automated Solvers
     To set up automated email confirmation/verification solvers, add your Proton Mail credentials below as shown.
     This removes the need to manually solve email challenges via the web app. These credentials can be used in `Scraper`, `Account`, and `Search` constructors.
     
     E.g.
     
     ```python
     from twitter.scraper import Scraper
     
     email, username, password = ..., ..., ...
     proton_email, proton_password = ..., ...
     account = Scraper(email, username, password, debug=1, save=True, protonmail={'email':proton_email, 'password':proton_password})
     ```
+    
     '''),
     long_description_content_type='text/markdown',
     author="Trevor Hobenshield",
     author_email="trevorhobenshield@gmail.com",
     url="https://github.com/trevorhobenshield/twitter-api-client",
     install_requires=install_requires,
     keywords="twitter api client async search automation bot scrape",
```

### Comparing `twitter-api-client-0.8.3/twitter/account.py` & `twitter-api-client-0.8.4/twitter/account.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,52 @@
 import hashlib
 import logging.config
 import math
 import mimetypes
 import random
-import time
 from copy import deepcopy
 from datetime import datetime
-from logging import Logger
-from pathlib import Path
-from urllib.parse import urlencode
+from string import ascii_letters
 from uuid import uuid1, getnode
 
-import orjson
-from httpx import Response
 from tqdm import tqdm
 
 from .constants import *
 from .login import login
-from .util import find_key, get_headers, fmt_status, get_cursor, save_data
+from .util import *
 
 
 class Account:
 
-    def __init__(self, email: str, username: str, password: str, **kwargs):
-        self.session = login(email, username, password, **kwargs)
+    def __init__(self, email: str = None, username: str = None, password: str = None, session: Client = None, **kwargs):
+        self.logger = self.init_logger(kwargs.get('log_config', False))
+        self.session = self.validate_session(email, username, password, session, **kwargs)
         self.gql_url = 'https://twitter.com/i/api/graphql'
         self.v1_url = 'https://api.twitter.com/1.1'
         self.save = kwargs.get('save', True)
         self.debug = kwargs.get('debug', 0)
-        self.logger = self.init_logger(kwargs.get('log_config', False))
 
     @staticmethod
     def init_logger(cfg: dict) -> Logger:
-        logging.config.dictConfig(cfg or log_config)
-        return logging.getLogger(__name__)
+        if cfg:
+            logging.config.dictConfig(cfg)
+            return logging.getLogger(__name__)
+        return logger
+
+    @staticmethod
+    def validate_session(*args, **kwargs):
+        email, username, password, session = args
+        if session and all(session.cookies.get(c) for c in {'ct0', 'auth_token'}):
+            # authenticated session provided
+            return session
+        if not session:
+            # no session provided, login to authenticate
+            return login(email, username, password, **kwargs)
+        raise Exception('Session not authenticated. '
+                        'Please use an authenticated session or remove the `session` argument and try again.')
 
     def gql(self, method: str, operation: tuple, variables: dict, features: dict = Operation.default_features) -> dict:
         qid, op = operation
         params = {
             'queryId': qid,
             'features': features,
             'variables': Operation.default_variables | variables
@@ -49,27 +58,23 @@
         r = self.session.request(
             method=method,
             url=f'{self.gql_url}/{qid}/{op}',
             headers=get_headers(self.session),
             **data
         )
         if self.debug:
-            self.log(r)
-        if self.save:
-            save_data(r.json(), op, self.session.cookies.get('username', '_'))
+            log(self.logger, self.debug, r)
         return r.json()
 
     def v1(self, path: str, params: dict) -> dict:
         headers = get_headers(self.session)
         headers['content-type'] = 'application/x-www-form-urlencoded'
         r = self.session.post(f'{self.v1_url}/{path}', headers=headers, data=urlencode(params))
         if self.debug:
-            self.log(r)
-        if self.save:
-            save_data(r.json(), '_', self.session.cookies.get('username', '_'))
+            log(self.logger, self.debug, r)
         return r.json()
 
     def create_poll(self, text: str, choices: list[str], poll_duration: int) -> dict:
         options = {
             "twitter:card": "poll4choice_text_only",
             "twitter:api:api:endpoint": "1",
             "twitter:long:duration_minutes": poll_duration  # max: 10080
@@ -92,15 +97,18 @@
             "target": {"participant_ids": receivers},
         }
         if media:
             media_id = self._upload_media(media, is_dm=True)
             variables['message']['media'] = {'id': media_id, 'text': text}
         else:
             variables['message']['text'] = {'text': text}
-        return self.gql('POST', Operation.useSendMessageMutation, variables)
+        res = self.gql('POST', Operation.useSendMessageMutation, variables)
+        if find_key(res, 'dm_validation_failure_type'):
+            logger.debug(f"{RED}Failed to send DM(s) to {receivers}{RESET}")
+        return res
 
     def tweet(self, text: str, *, media: any = None, **kwargs) -> dict:
         variables = {
             'tweet_text': text,
             'dark_request': False,
             'media': {
                 'media_entities': [],
@@ -167,24 +175,19 @@
                 media_id = self._upload_media(m['media'])
                 variables['post_tweet_request']['media_ids'].append(media_id)
                 if alt := m.get('alt'):
                     self._add_alt_text(media_id, alt)
         return self.gql('POST', Operation.CreateScheduledTweet, variables)
 
     def unschedule_tweet(self, tweet_id: int) -> dict:
-        variables = {
-            'scheduled_tweet_id': tweet_id,
-        }
+        variables = {'scheduled_tweet_id': tweet_id}
         return self.gql('POST', Operation.DeleteScheduledTweet, variables)
 
     def untweet(self, tweet_id: int) -> dict:
-        variables = {
-            'tweet_id': tweet_id,
-            'dark_request': False,
-        }
+        variables = {'tweet_id': tweet_id, 'dark_request': False}
         return self.gql('POST', Operation.DeleteTweet, variables)
 
     def reply(self, text: str, tweet_id: int) -> dict:
         variables = {
             'tweet_text': text,
             'reply': {
                 'in_reply_to_tweet_id': tweet_id,
@@ -211,25 +214,19 @@
                 'possibly_sensitive': False,
             },
             'semantic_annotation_ids': [],
         }
         return self.gql('POST', Operation.CreateTweet, variables)
 
     def retweet(self, tweet_id: int) -> dict:
-        variables = {
-            "tweet_id": tweet_id,
-            "dark_request": False
-        }
+        variables = {"tweet_id": tweet_id, "dark_request": False}
         return self.gql('POST', Operation.CreateRetweet, variables)
 
     def unretweet(self, tweet_id: int) -> dict:
-        variables = {
-            "source_tweet_id": tweet_id,
-            "dark_request": False
-        }
+        variables = {"source_tweet_id": tweet_id, "dark_request": False}
         return self.gql('POST', Operation.DeleteRetweet, variables)
 
     def like(self, tweet_id: int) -> dict:
         variables = {'tweet_id': tweet_id}
         return self.gql('POST', Operation.FavoriteTweet, variables)
 
     def unlike(self, tweet_id: int) -> dict:
@@ -291,64 +288,56 @@
         variables = {'listId': list_id, 'mediaId': media_id}
         return self.gql('POST', Operation.EditListBanner, variables)
 
     def delete_list_banner(self, list_id: int) -> dict:
         return self.gql('POST', Operation.DeleteListBanner, {'listId': list_id})
 
     def follow_topic(self, topic_id: int) -> dict:
-        variables = {'topicId': str(topic_id)}
-        return self.gql('POST', Operation.TopicFollow, variables)
+        return self.gql('POST', Operation.TopicFollow, {'topicId': str(topic_id)})
 
     def unfollow_topic(self, topic_id: int) -> dict:
-        variables = {'topicId': str(topic_id)}
-        return self.gql('POST', Operation.TopicUnfollow, variables)
+        return self.gql('POST', Operation.TopicUnfollow, {'topicId': str(topic_id)})
 
     def pin(self, tweet_id: int) -> dict:
-        params = {'tweet_mode': 'extended', 'id': tweet_id}
-        return self.v1('account/pin_tweet.json', params)
+        return self.v1('account/pin_tweet.json', {'tweet_mode': 'extended', 'id': tweet_id})
 
     def unpin(self, tweet_id: int) -> dict:
-        params = {'tweet_mode': 'extended', 'id': tweet_id}
-        return self.v1('account/unpin_tweet.json', params)
+        return self.v1('account/unpin_tweet.json', {'tweet_mode': 'extended', 'id': tweet_id})
 
     def follow(self, user_id: int) -> dict:
         settings = deepcopy(follow_settings)
         settings |= {"user_id": user_id}
         return self.v1('friendships/create.json', settings)
 
     def unfollow(self, user_id: int) -> dict:
         settings = deepcopy(follow_settings)
         settings |= {"user_id": user_id}
         return self.v1('friendships/destroy.json', settings)
 
     def mute(self, user_id: int) -> dict:
-        params = {'user_id': user_id}
-        return self.v1('mutes/users/create.json', params)
+        return self.v1('mutes/users/create.json', {'user_id': user_id})
 
     def unmute(self, user_id: int) -> dict:
-        params = {'user_id': user_id}
-        return self.v1('mutes/users/destroy.json', params)
+        return self.v1('mutes/users/destroy.json', {'user_id': user_id})
 
     def enable_notifications(self, user_id: int) -> dict:
         settings = deepcopy(notification_settings)
         settings |= {'id': user_id, 'device': 'true'}
         return self.v1('friendships/update.json', settings)
 
     def disable_notifications(self, user_id: int) -> dict:
         settings = deepcopy(notification_settings)
         settings |= {'id': user_id, 'device': 'false'}
         return self.v1('friendships/update.json', settings)
 
     def block(self, user_id: int) -> dict:
-        params = {'user_id': user_id}
-        return self.v1('blocks/create.json', params)
+        return self.v1('blocks/create.json', {'user_id': user_id})
 
     def unblock(self, user_id: int) -> dict:
-        params = {'user_id': user_id}
-        return self.v1('blocks/destroy.json', params)
+        return self.v1('blocks/destroy.json', {'user_id': user_id})
 
     def update_profile_image(self, media: str) -> Response:
         media_id = self._upload_media(media, is_profile=True)
         url = f'{self.v1_url}/account/update_profile_image.json'
         headers = get_headers(self.session)
         params = {'media_id': media_id}
         r = self.session.post(url, headers=headers, params=params)
@@ -372,15 +361,14 @@
         twid = int(self.session.cookies.get('twid').split('=')[-1].strip('"'))
         headers = get_headers(self.session)
         r = self.session.post(
             url=f'{self.v1_url}/strato/column/User/{twid}/search/searchSafety',
             headers=headers,
             json=settings,
         )
-        self.logger.debug(r)
         return r
 
     def update_settings(self, settings: dict) -> dict:
         return self.v1('account/settings.json', settings)
 
     def change_password(self, old: str, new: str) -> dict:
         params = {
@@ -456,98 +444,116 @@
             if prev_len == len(ids):
                 dups += 1
 
             res.append(data)
         return res
 
     def _upload_media(self, filename: str, is_dm: bool = False, is_profile=False) -> int | None:
+        """
+        https://developer.twitter.com/en/docs/twitter-api/v1/media/upload-media/uploading-media/media-best-practices
+        """
 
         def check_media(category: str, size: int) -> None:
             fmt = lambda x: f'{(x / 1e6):.2f} MB'
             msg = lambda x: f'cannot upload {fmt(size)} {category}, max size is {fmt(x)}'
             if category == 'image' and size > MAX_IMAGE_SIZE:
                 raise Exception(msg(MAX_IMAGE_SIZE))
             if category == 'gif' and size > MAX_GIF_SIZE:
                 raise Exception(msg(MAX_GIF_SIZE))
             if category == 'video' and size > MAX_VIDEO_SIZE:
                 raise Exception(msg(MAX_VIDEO_SIZE))
 
-        if is_profile:
-            url = 'https://upload.twitter.com/i/media/upload.json'
-        else:
-            url = 'https://upload.twitter.com/1.1/media/upload.json'
+        # if is_profile:
+        #     url = 'https://upload.twitter.com/i/media/upload.json'
+        # else:
+        #     url = 'https://upload.twitter.com/1.1/media/upload.json'
+
+        url = 'https://upload.twitter.com/i/media/upload.json'
 
         file = Path(filename)
         total_bytes = file.stat().st_size
         headers = get_headers(self.session)
 
         upload_type = 'dm' if is_dm else 'tweet'
         media_type = mimetypes.guess_type(file)[0]
         media_category = f'{upload_type}_gif' if 'gif' in media_type else f'{upload_type}_{media_type.split("/")[0]}'
 
         check_media(media_category, total_bytes)
 
-        data = {'command': 'INIT', 'media_type': media_type, 'total_bytes': total_bytes,
-                'media_category': media_category}
-        r = self.session.post(url=url, headers=headers, data=data)
+        params = {'command': 'INIT', 'media_type': media_type, 'total_bytes': total_bytes,
+                  'media_category': media_category}
+        r = self.session.post(url=url, headers=headers, params=params)
+
+        if r.status_code >= 400:
+            raise Exception(f'{r.text}')
+
         media_id = r.json()['media_id']
 
         desc = f"uploading: {file.name}"
         with tqdm(total=total_bytes, desc=desc, unit='B', unit_scale=True, unit_divisor=1024) as pbar:
-            with open(file, 'rb') as f:
+            with open(file, 'rb') as fp:
                 i = 0
-                while chunk := f.read(UPLOAD_CHUNK_SIZE):  # todo: arbitrary max size for now
-                    data = {'command': 'APPEND', 'media_id': media_id, 'segment_index': i}
-                    files = {'media': chunk}
-                    r = self.session.post(url=url, headers=headers, data=data, files=files)
+                while chunk := fp.read(UPLOAD_CHUNK_SIZE):
+                    params = {'command': 'APPEND', 'media_id': media_id, 'segment_index': i}
+                    try:
+                        pad = bytes(''.join(random.choices(ascii_letters, k=16)), encoding='utf-8')
+                        data = b''.join([
+                            b'------WebKitFormBoundary',
+                            pad,
+                            b'\r\nContent-Disposition: form-data; name="media"; filename="blob"',
+                            b'\r\nContent-Type: application/octet-stream',
+                            b'\r\n\r\n',
+                            chunk,
+                            b'\r\n------WebKitFormBoundary',
+                            pad,
+                            b'--\r\n',
+                        ])
+                        _headers = {b'content-type': b'multipart/form-data; boundary=----WebKitFormBoundary' + pad}
+                        r = self.session.post(url=url, headers=headers | _headers, params=params, content=data)
+                    except Exception as e:
+                        self.logger.error('Failed to upload chunk, trying alternative method')
+                        try:
+                            files = {'media': chunk}
+                            r = self.session.post(url=url, headers=headers, params=params, files=files)
+                        except Exception as e:
+                            self.logger.error(f'Failed to upload chunk: {e}')
+                            return
+
                     if r.status_code < 200 or r.status_code > 299:
-                        self.logger.debug(f'{r.status_code} {r.text}')
-                        raise Exception(f'[{RED}error{RESET}] upload failed')
+                        self.logger.debug(f'{RED}{r.status_code} {r.text}{RESET}')
+
                     i += 1
-                    pbar.update(f.tell() - pbar.n)
+                    pbar.update(fp.tell() - pbar.n)
 
-        data = {'command': 'FINALIZE', 'media_id': media_id, 'allow_async': 'true'}
+        params = {'command': 'FINALIZE', 'media_id': media_id, 'allow_async': 'true'}
         if is_dm:
-            data |= {'original_md5': hashlib.md5(file.read_bytes()).hexdigest()}
-        r = self.session.post(url=url, headers=headers, data=data)
+            params |= {'original_md5': hashlib.md5(file.read_bytes()).hexdigest()}
+        r = self.session.post(url=url, headers=headers, params=params)
+        if r.status_code == 400:
+            self.logger.debug(f'{RED}{r.status_code} {r.text}{RESET}')
+            return
 
         # self.logger.debug(f'processing, please wait...')
         processing_info = r.json().get('processing_info')
         while processing_info:
             state = processing_info['state']
             if error := processing_info.get("error"):
-                raise Exception(f'media upload failed: {error}')
+                self.logger.debug(f'{RED}{error}{RESET}')
+                return
             if state == MEDIA_UPLOAD_SUCCEED:
                 break
             if state == MEDIA_UPLOAD_FAIL:
-                raise Exception(f'[{RED}error{RESET}] media processing failed')
+                self.logger.debug(f'{RED}{r.status_code} {r.text} {RESET}')
+                return
             check_after_secs = processing_info.get('check_after_secs', random.randint(1, 5))
             time.sleep(check_after_secs)
             params = {'command': 'STATUS', 'media_id': media_id}
             r = self.session.get(url=url, headers=headers, params=params)
             processing_info = r.json().get('processing_info')
         # self.logger.debug('processing complete')
         return media_id
 
     def _add_alt_text(self, media_id: int, text: str) -> Response:
         params = {"media_id": media_id, "alt_text": {"text": text}}
         url = f'{self.v1_url}/media/metadata/create.json'
         r = self.session.post(url, headers=get_headers(self.session), json=params)
         return r
-
-    def log(self, response: Response):
-        status = fmt_status(response.status_code)
-        if 'json' in response.headers.get('content-type', ''):
-            if response.json().get('errors'):
-                self.logger.debug(f'[{RED}twitter error{RESET}]')
-                self.logger.debug(f'{response.url}')
-                self.logger.debug(f'{response.text}')
-                return
-        self.logger.debug(status)
-        if self.debug >= 1:
-            self.logger.debug(f'{response.url}')
-        if self.debug >= 2:
-            self.logger.debug(f'{response.text}')
-        if self.debug >= 3:
-            self.logger.debug(f'{response.headers}')
-        if self.debug >= 4:
-            self.logger.debug(f'{response.cookies}')
```

### Comparing `twitter-api-client-0.8.3/twitter/constants.py` & `twitter-api-client-0.8.4/twitter/constants.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from dataclasses import dataclass
+import logging
+import logging.config
 
 MAX_IMAGE_SIZE = 5_242_880  # ~5 MB
 MAX_GIF_SIZE = 15_728_640  # ~15 MB
 MAX_VIDEO_SIZE = 536_870_912  # ~530 MB
 
 UPLOAD_CHUNK_SIZE = 4 * 1024 * 1024
 MEDIA_UPLOAD_SUCCEED = 'succeeded'
@@ -15,77 +17,108 @@
 BLUE = '\x1b[34m'
 MAGENTA = '\x1b[35m'
 CYAN = '\x1b[36m'
 WHITE = '\x1b[37m'
 BOLD = '\x1b[1m'
 RESET = '\x1b[0m'
 
-log_config = {
-    "version": 1,
-    "formatters": {
-        "simple": {
-            "format": "%(asctime)s.%(msecs)03d %(levelname)s: %(message)s"
-        }
+DISABLE_LOG_PROPAGATION = [
+    'httpx',
+    'httpcore',
+    'aiofiles',
+    'websockets',
+    'nest_asyncio',
+    'orjson',
+    'tqdm',
+    'bcrypt',
+    'python-gnupg',
+    'pyopenssl',
+    'uvloop',
+]
+
+LOGGING_CONFIG = {
+    'version': 1,
+    'disable_existing_loggers': False,
+    'formatters': {
+        'standard': {
+            'format': '%(asctime)s.%(msecs)03d [%(levelname)s] :: %(message)s',
+            'datefmt': '%Y-%m-%d %H:%M:%S'
+        },
     },
-    "handlers": {
-        "console": {
-            "class": "logging.StreamHandler",
-            "level": "DEBUG",
-            "formatter": "simple",
-            "stream": "ext://sys.stdout"
+    'handlers': {
+        'console': {
+            'class': 'logging.StreamHandler',
+            'level': 'DEBUG',
+            'formatter': 'standard',
+            'stream': 'ext://sys.stdout',
+        },
+        'file': {
+            'class': 'logging.FileHandler',
+            'level': 'DEBUG',
+            'formatter': 'standard',
+            'filename': 'log.log',
+            'mode': 'a',
         },
-        "file": {
-            "class": "logging.FileHandler",
-            "level": "DEBUG",
-            "formatter": "simple",
-            "filename": "debug.log",
-            "encoding": "utf8",
-            "mode": "a"
-        }
     },
-    "loggers": {
-        "myLogger": {
-            "level": "DEBUG",
-            "handlers": [
-                "console"
-            ],
-            "propagate": "no"
+    'root': {
+        'handlers': ['console', 'file'],
+        'level': 'DEBUG',
+    },
+    'loggers': {
+        pkg: {
+            'handlers': ['console', 'file'],
+            'level': 'WARNING',
+            'propagate': False
         }
+        for pkg in DISABLE_LOG_PROPAGATION
     },
-    "root": {
-        "level": "DEBUG",
-        "handlers": [
-            "console",
-            "file"
-        ]
-    }
 }
 
+logging.config.dictConfig(LOGGING_CONFIG)
+logger = logging.getLogger(__name__)
+
+
+@dataclass
+class SpaceCategory:
+    Top = 'Top'
+    Live = 'Live'
+    Upcoming = 'Upcoming'
+
+
+@dataclass
+class SpaceState:
+    Ended = 'Ended'
+    Canceled = 'Canceled'
+    NotStarted = 'NotStarted'
+    PrePublished = 'PrePublished'
+    Running = 'Running'
+    TimedOut = 'TimedOut'
+
 
 @dataclass
 class Operation:
-    # Scraper Operations
-    ProfileSpotlightsQuery = '9zwVLJ48lmVUk8u_Gh9DmA', 'ProfileSpotlightsQuery', 'screen_name'
-    UserByScreenName = 'sLVLhk0bGj3MVFEKTdax1w', 'UserByScreenName', 'screen_name'
-    UserByRestId = 'GazOglcBvgLigl3ywt6b3Q', 'UserByRestId', 'userId'
-    UsersByRestIds = 'OJBgJQIrij6e3cjqQ3Zu1Q', 'UsersByRestIds', 'userIds'
-    UserTweets = 'HuTx74BxAnezK1gWvYY7zg', 'UserTweets', 'userId'
-    UserMedia = 'YqiE3JL1KNgf9nSljYdxaA', 'UserMedia', 'userId'
-    UserTweetsAndReplies = 'RIWc55YCNyUJ-U3HHGYkdg', 'UserTweetsAndReplies', 'userId'
-    TweetResultByRestId = 'D_jNhjWZeRZT5NURzfJZSQ', 'TweetResultByRestId', 'tweetId'
-    TweetDetail = 'zXaXQgfyR4GxE21uwYQSyA', 'TweetDetail', 'focalTweetId'
-    TweetStats = 'EvbTkPDT-xQCfupPu0rWMA', 'TweetStats', 'rest_id'
-
-    # auth required
-    Likes = 'nYrjBgnUWQFt_tRyCGatZA', 'Likes', 'userId'
-    Followers = 'pd8Tt1qUz1YWrICegqZ8cw', 'Followers', 'userId'
-    Following = 'wjvx62Hye2dGVvnvVco0xA', 'Following', 'userId'
-    Retweeters = '0BoJlKAxoNPQUHRftlwZ2w', 'Retweeters', 'tweetId'
-    Favoriters = 'XRRjv1-uj1HZn3o324etOQ', 'Favoriters', 'tweetId'
-    ConnectTabTimeline = 'lq02A-gEzbLefqTgD_PFzQ', 'ConnectTabTimeline', 'context'
+    # todo: dynamically update
+    AudioSpaceById = {'id': str}, 'fYAuJHiY3TmYdBmrRtIKhA', 'AudioSpaceById'
+    AudioSpaceSearch = {'filter': str, 'query': str}, 'NTq79TuSz6fHj8lQaferJw', 'AudioSpaceSearch',
+    UserByScreenName = {'screen_name': str}, 'sLVLhk0bGj3MVFEKTdax1w', 'UserByScreenName'
+    UserTweets = {'userId': int}, 'HuTx74BxAnezK1gWvYY7zg', 'UserTweets'
+    ProfileSpotlightsQuery = {'screen_name': str}, '9zwVLJ48lmVUk8u_Gh9DmA', 'ProfileSpotlightsQuery'
+    UserByRestId = {'userId': int}, 'GazOglcBvgLigl3ywt6b3Q', 'UserByRestId'
+    UsersByRestIds = {'userIds': list}, 'OJBgJQIrij6e3cjqQ3Zu1Q', 'UsersByRestIds'
+    UserMedia = {'userId': int}, 'YqiE3JL1KNgf9nSljYdxaA', 'UserMedia'
+    UserTweetsAndReplies = {'userId': int}, 'RIWc55YCNyUJ-U3HHGYkdg', 'UserTweetsAndReplies'
+    TweetResultByRestId = {'tweetId': int}, 'D_jNhjWZeRZT5NURzfJZSQ', 'TweetResultByRestId'
+    TweetDetail = {'focalTweetId': int}, 'zXaXQgfyR4GxE21uwYQSyA', 'TweetDetail'
+    TweetStats = {'rest_id': int}, 'EvbTkPDT-xQCfupPu0rWMA', 'TweetStats'
+    Likes = {'userId': int}, 'nXEl0lfN_XSznVMlprThgQ', 'Likes'
+    Followers = {'userId': int}, 'pd8Tt1qUz1YWrICegqZ8cw', 'Followers'
+    Following = {'userId': int}, 'wjvx62Hye2dGVvnvVco0xA', 'Following'
+    Retweeters = {'tweetId': int}, '0BoJlKAxoNPQUHRftlwZ2w', 'Retweeters'
+    Favoriters = {'tweetId': int}, 'XRRjv1-uj1HZn3o324etOQ', 'Favoriters'
+    ConnectTabTimeline = {'context': dict}, 'lq02A-gEzbLefqTgD_PFzQ', 'ConnectTabTimeline'
 
     # Account Operations
     useSendMessageMutation = 'MaxK2PKX1F9Z-9SwqwavTw', 'useSendMessageMutation'
     CreateTweet = '7TKRKCPuAGsmYde0CudbVg', 'CreateTweet'
     DeleteTweet = 'VaenaVgh5q5ih7kvyVjgtg', 'DeleteTweet'
     CreateScheduledTweet = 'LCVzRQGxOaGnOnYH01NQXg', 'CreateScheduledTweet'
     DeleteScheduledTweet = 'CTOVqej0JBXAZSwkp1US0g', 'DeleteScheduledTweet'
@@ -112,16 +145,14 @@
     Bookmarks = 'tmd4ifV8RHltzn8ymGg1aw', 'Bookmarks'
 
     # misc/not implemented
     AdAccounts = 'a8KxGfFQAmm3WxqemuqSRA', 'AdAccounts'
     ArticleTimeline = 'o9FyvnC-xg8mVBXqL4g-rg', 'ArticleTimeline'
     ArticleTweetsTimeline = 'x4ywSpvg6BesoDszkfbFQg', 'ArticleTweetsTimeline'
     AudienceEstimate = '1LYVUabJBYkPlUAWRabB3g', 'AudienceEstimate'
-    AudioSpaceById = 'QB5okPsUwVP3TefHBFItnw', 'AudioSpaceById'
-    AudioSpaceSearch = 'NTq79TuSz6fHj8lQaferJw', 'AudioSpaceSearch'
     AuthenticatedUserTFLists = 'QjN8ZdavFDqxUjNn3r9cig', 'AuthenticatedUserTFLists'
     BirdwatchAliasSelect = '3ss48WFwGokBH_gj8t_8aQ', 'BirdwatchAliasSelect'
     BirdwatchCreateAppeal = 'TKdL0YFsX4DMOpMKeneLvA', 'BirdwatchCreateAppeal'
     BirdwatchCreateNote = '36EUZZyaciVmNrq4CRZcmw', 'BirdwatchCreateNote'
     BirdwatchCreateRating = 'bD3AEK9BMCSpRods_ng2fA', 'BirdwatchCreateRating'
     BirdwatchDeleteNote = 'IKS_qrShkDyor6Ri1ahd9g', 'BirdwatchDeleteNote'
     BirdwatchDeleteRating = 'OpvCOyOoQClUND66zDzrnA', 'BirdwatchDeleteRating'
@@ -305,29 +336,31 @@
     getAltTextPromptPreference = 'PFIxTk8owMoZgiMccP0r4g', 'getAltTextPromptPreference'
     getCaptionsAlwaysDisplayPreference = 'BwgMOGpOViDS0ri7VUgglg', 'getCaptionsAlwaysDisplayPreference'
     timelinesFeedback = 'vfVbgvTPTQ-dF_PQ5lD1WQ', 'timelinesFeedback'
     updateAltTextPromptPreference = 'aQKrduk_DA46XfOQDkcEng', 'updateAltTextPromptPreference'
     updateCaptionsAlwaysDisplayPreference = 'uCUQhvZ5sJ9qHinRp6CFlQ', 'updateCaptionsAlwaysDisplayPreference'
 
     default_variables = {
-        "count": 1000,
-        "withSafetyModeUserFields": True,
-        "includePromotedContent": True,
-        "withQuickPromoteEligibilityTweetFields": True,
-        "withVoice": True,
-        "withV2Timeline": True,
-        "withDownvotePerspective": False,
-        "withBirdwatchNotes": True,
-        "withCommunity": True,
-        "withSuperFollowsUserFields": True,
-        "withReactionsMetadata": False,
-        "withReactionsPerspective": False,
-        "withSuperFollowsTweetFields": True
+        'count': 1000,
+        'withSafetyModeUserFields': True,
+        'includePromotedContent': True,
+        'withQuickPromoteEligibilityTweetFields': True,
+        'withVoice': True,
+        'withV2Timeline': True,
+        'withDownvotePerspective': False,
+        'withBirdwatchNotes': True,
+        'withCommunity': True,
+        'withSuperFollowsUserFields': True,
+        'withReactionsMetadata': False,
+        'withReactionsPerspective': False,
+        'withSuperFollowsTweetFields': True,
+        'isMetatagsQuery': False,
+        'withReplays': True,
+        'withClientEventToken': False,
     }
-
     default_features = {
         'blue_business_profile_image_shape_enabled': True,
         'responsive_web_graphql_exclude_directive_enabled': True,
         'verified_phone_label_enabled': False,
         'responsive_web_graphql_skip_user_profile_image_extensions_enabled': False,
         'responsive_web_graphql_timeline_navigation_enabled': True,
         'tweetypie_unmention_optimization_enabled': True, 'vibe_api_enabled': True,
@@ -335,191 +368,197 @@
         'graphql_is_translatable_rweb_tweet_is_translatable_enabled': True,
         'view_counts_everywhere_api_enabled': True,
         'longform_notetweets_consumption_enabled': True,
         'tweet_awards_web_tipping_enabled': False,
         'freedom_of_speech_not_reach_fetch_enabled': False,
         'standardized_nudges_misinfo': True,
         'tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled': False,
-        'interactive_text_enabled': True, 'responsive_web_text_conversations_enabled': False,
+        'interactive_text_enabled': True,
+        'responsive_web_text_conversations_enabled': False,
         'longform_notetweets_rich_text_read_enabled': True,
         'responsive_web_enhance_cards_enabled': False,
         'responsive_web_twitter_blue_verified_badge_is_enabled': True,
         'longform_notetweets_richtext_consumption_enabled': True,
         'profile_foundations_tweet_stats_enabled': True,
         'profile_foundations_tweet_stats_tweet_frequency': True,
         'graphql_timeline_v2_bookmark_timeline': True,
+        'spaces_2022_h2_clipping': True,
+        'spaces_2022_h2_spaces_communities': True,
+        'creator_subscriptions_tweet_preview_api_enabled': True,
+        'longform_notetweets_inline_media_enabled': False,
+        'rweb_lists_timeline_redesign_enabled': True,
     }
 
 
 trending_params = {
-    "include_profile_interstitial_type": "1",
-    "include_blocking": "1",
-    "include_blocked_by": "1",
-    "include_followed_by": "1",
-    "include_want_retweets": "1",
-    "include_mute_edge": "1",
-    "include_can_dm": "1",
-    "include_can_media_tag": "1",
-    "include_ext_has_nft_avatar": "1",
-    "include_ext_is_blue_verified": "1",
-    "include_ext_verified_type": "1",
-    "skip_status": "1",
-    "cards_platform": "Web-12",
-    "include_cards": "1",
-    "include_ext_alt_text": "true",
-    "include_ext_limited_action_results": "false",
-    "include_quote_count": "true",
-    "include_reply_count": "1",
-    "tweet_mode": "extended",
-    "include_ext_views": "true",
-    "include_entities": "true",
-    "include_user_entities": "true",
-    "include_ext_media_color": "true",
-    "include_ext_media_availability": "true",
-    "include_ext_sensitive_media_warning": "true",
-    "include_ext_trusted_friends_metadata": "true",
-    "send_error_codes": "true",
-    "simple_quoted_tweet": "true",
-    "count": 1000,
-    "requestContext": "launch",
-    "include_page_configuration": "true",
-    "initial_tab_id": "trending",
-    "entity_tokens": "false",
-    "ext": "mediaStats,highlightedLabel,hasNftAvatar,voiceInfo,birdwatchPivot,enrichments,superFollowMetadata,unmentionInfo,editControl,vibe"
+    'include_profile_interstitial_type': '1',
+    'include_blocking': '1',
+    'include_blocked_by': '1',
+    'include_followed_by': '1',
+    'include_want_retweets': '1',
+    'include_mute_edge': '1',
+    'include_can_dm': '1',
+    'include_can_media_tag': '1',
+    'include_ext_has_nft_avatar': '1',
+    'include_ext_is_blue_verified': '1',
+    'include_ext_verified_type': '1',
+    'skip_status': '1',
+    'cards_platform': 'Web-12',
+    'include_cards': '1',
+    'include_ext_alt_text': 'true',
+    'include_ext_limited_action_results': 'false',
+    'include_quote_count': 'true',
+    'include_reply_count': '1',
+    'tweet_mode': 'extended',
+    'include_ext_views': 'true',
+    'include_entities': 'true',
+    'include_user_entities': 'true',
+    'include_ext_media_color': 'true',
+    'include_ext_media_availability': 'true',
+    'include_ext_sensitive_media_warning': 'true',
+    'include_ext_trusted_friends_metadata': 'true',
+    'send_error_codes': 'true',
+    'simple_quoted_tweet': 'true',
+    'count': 1000,
+    'requestContext': 'launch',
+    'include_page_configuration': 'true',
+    'initial_tab_id': 'trending',
+    'entity_tokens': 'false',
+    'ext': 'mediaStats,highlightedLabel,hasNftAvatar,voiceInfo,birdwatchPivot,enrichments,superFollowMetadata,unmentionInfo,editControl,vibe'
 }
 
 account_settings = {
-    "address_book_live_sync_enabled": False,
-    "allow_ads_personalization": False,
-    "allow_authenticated_periscope_requests": True,
-    "allow_dm_groups_from": "following",
-    "allow_dms_from": "following",  # all
-    "allow_location_history_personalization": False,
-    "allow_logged_out_device_personalization": False,
-    "allow_media_tagging": "none",  # all, following
-    "allow_sharing_data_for_third_party_personalization": False,
-    "alt_text_compose_enabled": None,
-    "always_use_https": True,
-    "autoplay_disabled": False,
-    "country_code": "us",
-    "discoverable_by_email": False,
-    "discoverable_by_mobile_phone": False,
-    "display_sensitive_media": True,
-    "dm_quality_filter": "enabled",  # disabled
-    "dm_receipt_setting": "all_disabled",  # all_enabled
-    "geo_enabled": False,
-    "include_alt_text_compose": True,
-    "include_mention_filter": True,
-    "include_nsfw_admin_flag": True,
-    "include_nsfw_user_flag": True,
-    "include_ranked_timeline": True,
-    "language": "en",
-    "mention_filter": "unfiltered",
-    "nsfw_admin": False,
-    "nsfw_user": False,
-    "personalized_trends": True,
-    "protected": False,
-    "ranked_timeline_eligible": None,
-    "ranked_timeline_setting": None,
-    "require_password_login": False,
-    "requires_login_verification": False,
-    "settings_metadata": {},
-    "sleep_time": {
-        "enabled": False,
-        "end_time": None,
-        "start_time": None
+    'address_book_live_sync_enabled': False,
+    'allow_ads_personalization': False,
+    'allow_authenticated_periscope_requests': True,
+    'allow_dm_groups_from': 'following',
+    'allow_dms_from': 'following',  # all
+    'allow_location_history_personalization': False,
+    'allow_logged_out_device_personalization': False,
+    'allow_media_tagging': 'none',  # all, following
+    'allow_sharing_data_for_third_party_personalization': False,
+    'alt_text_compose_enabled': None,
+    'always_use_https': True,
+    'autoplay_disabled': False,
+    'country_code': 'us',
+    'discoverable_by_email': False,
+    'discoverable_by_mobile_phone': False,
+    'display_sensitive_media': True,
+    'dm_quality_filter': 'enabled',  # disabled
+    'dm_receipt_setting': 'all_disabled',  # all_enabled
+    'geo_enabled': False,
+    'include_alt_text_compose': True,
+    'include_mention_filter': True,
+    'include_nsfw_admin_flag': True,
+    'include_nsfw_user_flag': True,
+    'include_ranked_timeline': True,
+    'language': 'en',
+    'mention_filter': 'unfiltered',
+    'nsfw_admin': False,
+    'nsfw_user': False,
+    'personalized_trends': True,
+    'protected': False,
+    'ranked_timeline_eligible': None,
+    'ranked_timeline_setting': None,
+    'require_password_login': False,
+    'requires_login_verification': False,
+    'settings_metadata': {},
+    'sleep_time': {
+        'enabled': False,
+        'end_time': None,
+        'start_time': None
     },
-    "translator_type": "none",
-    "universal_quality_filtering_enabled": "enabled",
-    "use_cookie_personalization": False,
+    'translator_type': 'none',
+    'universal_quality_filtering_enabled': 'enabled',
+    'use_cookie_personalization': False,
     ## todo: not yet implemented - requires additional steps
-    # "allow_contributor_request": "all",
-    # "protect_password_reset": False,
+    # 'allow_contributor_request': 'all',
+    # 'protect_password_reset': False,
 }
 notification_settings = {
-    "cursor": "-1",
-    "include_profile_interstitial_type": "1",
-    "include_blocking": "1",
-    "include_blocked_by": "1",
-    "include_followed_by": "1",
-    "include_want_retweets": "1",
-    "include_mute_edge": "1",
-    "include_can_dm": "1",
-    "include_can_media_tag": "1",
-    "include_ext_has_nft_avatar": "1",
-    "include_ext_is_blue_verified": "1",
-    "include_ext_verified_type": "1",
-    "skip_status": "1",
+    'cursor': '-1',
+    'include_profile_interstitial_type': '1',
+    'include_blocking': '1',
+    'include_blocked_by': '1',
+    'include_followed_by': '1',
+    'include_want_retweets': '1',
+    'include_mute_edge': '1',
+    'include_can_dm': '1',
+    'include_can_media_tag': '1',
+    'include_ext_has_nft_avatar': '1',
+    'include_ext_is_blue_verified': '1',
+    'include_ext_verified_type': '1',
+    'skip_status': '1',
 }
 
 follow_settings = {
-    "include_profile_interstitial_type": "1",
-    "include_blocking": "1",
-    "include_blocked_by": "1",
-    "include_followed_by": "1",
-    "include_want_retweets": "1",
-    "include_mute_edge": "1",
-    "include_can_dm": "1",
-    "include_can_media_tag": "1",
-    "include_ext_has_nft_avatar": "1",
-    "include_ext_is_blue_verified": "1",
-    "include_ext_verified_type": "1",
-    "skip_status": "1",
+    'include_profile_interstitial_type': '1',
+    'include_blocking': '1',
+    'include_blocked_by': '1',
+    'include_followed_by': '1',
+    'include_want_retweets': '1',
+    'include_mute_edge': '1',
+    'include_can_dm': '1',
+    'include_can_media_tag': '1',
+    'include_ext_has_nft_avatar': '1',
+    'include_ext_is_blue_verified': '1',
+    'include_ext_verified_type': '1',
+    'skip_status': '1',
 }
 
 account_search_settings = {
-    "optInFiltering": True,  # filter out nsfw content
-    "optInBlocking": True,  # filter out blocked accounts
+    'optInFiltering': True,  # filter out nsfw content
+    'optInBlocking': True,  # filter out blocked accounts
 }
 
 profile_settings = {
-    "birthdate_day": int,
-    "birthdate_month": int,
-    "birthdate_year": int,  # 1985
-    "birthdate_visibility": str,  # "self",
-    "birthdate_year_visibility": str,  # "self",
-    "displayNameMaxLength": int,  # "50",
-    "url": str,  # "https://example.com",
-    "name": str,  # "foo",
-    "description": str,  # "bar",
-    "location": str,  # "world",
+    'birthdate_day': int,
+    'birthdate_month': int,
+    'birthdate_year': int,  # 1985
+    'birthdate_visibility': str,  # 'self',
+    'birthdate_year_visibility': str,  # 'self',
+    'displayNameMaxLength': int,  # '50',
+    'url': str,  # 'https://example.com',
+    'name': str,  # 'foo',
+    'description': str,  # 'bar',
+    'location': str,  # 'world',
 }
 
 search_config = {
-    "include_profile_interstitial_type": 1,
-    "include_blocking": 1,
-    "include_blocked_by": 1,
-    "include_followed_by": 1,
-    "include_want_retweets": 1,
-    "include_mute_edge": 1,
-    "include_can_dm": 1,
-    "include_can_media_tag": 1,
-    "include_ext_has_nft_avatar": 1,
-    "include_ext_is_blue_verified": 1,
-    "include_ext_verified_type": 1,
-    "skip_status": 1,
-    "cards_platform": "Web-12",
-    "include_cards": 1,
-    "include_ext_alt_text": "true",
-    "include_ext_limited_action_results": "false",
-    "include_quote_count": "true",
-    "include_reply_count": 1,
-    "tweet_mode": "extended",
-    "include_ext_collab_control": "true",
-    "include_ext_views": "true",
-    "include_entities": "true",
-    "include_user_entities": "true",
-    "include_ext_media_color": "true",
-    "include_ext_media_availability": "true",
-    "include_ext_sensitive_media_warning": "true",
-    "include_ext_trusted_friends_metadata": "true",
-    "send_error_codes": "true",
-    "simple_quoted_tweet": "true",
-    "query_source": "typed_query",
-    "count": 1000,
-    "q": "",
-    "requestContext": "launch",
-    "pc": 1,
-    "spelling_corrections": 1,
-    "include_ext_edit_control": "true",
-    "ext": "mediaStats,highlightedLabel,hasNftAvatar,voiceInfo,birdwatchPivot,enrichments,superFollowMetadata,unmentionInfo,editControl,collab_control,vibe"
+    'include_profile_interstitial_type': 1,
+    'include_blocking': 1,
+    'include_blocked_by': 1,
+    'include_followed_by': 1,
+    'include_want_retweets': 1,
+    'include_mute_edge': 1,
+    'include_can_dm': 1,
+    'include_can_media_tag': 1,
+    'include_ext_has_nft_avatar': 1,
+    'include_ext_is_blue_verified': 1,
+    'include_ext_verified_type': 1,
+    'skip_status': 1,
+    'cards_platform': 'Web-12',
+    'include_cards': 1,
+    'include_ext_alt_text': 'true',
+    'include_ext_limited_action_results': 'false',
+    'include_quote_count': 'true',
+    'include_reply_count': 1,
+    'tweet_mode': 'extended',
+    'include_ext_collab_control': 'true',
+    'include_ext_views': 'true',
+    'include_entities': 'true',
+    'include_user_entities': 'true',
+    'include_ext_media_color': 'true',
+    'include_ext_media_availability': 'true',
+    'include_ext_sensitive_media_warning': 'true',
+    'include_ext_trusted_friends_metadata': 'true',
+    'send_error_codes': 'true',
+    'simple_quoted_tweet': 'true',
+    'query_source': 'typed_query',
+    'count': 1000,
+    'q': '',
+    'requestContext': 'launch',
+    'pc': 1,
+    'spelling_corrections': 1,
+    'include_ext_edit_control': 'true',
+    'ext': 'mediaStats,highlightedLabel,hasNftAvatar,voiceInfo,birdwatchPivot,enrichments,superFollowMetadata,unmentionInfo,editControl,collab_control,vibe'
 }
```

### Comparing `twitter-api-client-0.8.3/twitter/login.py` & `twitter-api-client-0.8.4/twitter/login.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,168 +1,175 @@
 import sys
+import time
+
 from httpx import Client
 from .constants import GREEN, YELLOW, RED, BOLD, RESET
-from .util import find_key, get_confirmation_code, get_inbox, init_session
+from .util import find_key, get_confirmation_code, get_inbox, init_protonmail_session
 
 
-def update_token(session: Client, key: str, url: str, **kwargs) -> Client:
+def update_token(client: Client, key: str, url: str, **kwargs) -> Client:
     caller_name = sys._getframe(1).f_code.co_name
     try:
         headers = {
-            'authorization': 'Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs%3D1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA',
-            'content-type': 'application/json',
-            'user-agent': 'Mozilla/5.0 (Linux; Android 11; Nokia G20) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.88 Mobile Safari/537.36',
-            'x-guest-token': session.cookies.get('guest_token', ''),
-            'x-csrf-token': session.cookies.get('ct0', ''),
-            'x-twitter-auth-type': 'OAuth2Client' if session.cookies.get('auth_token') else '',
-            'x-twitter-active-user': 'yes',
-            'x-twitter-client-language': 'en',
+            'x-guest-token': client.cookies.get('guest_token', ''),
+            'x-csrf-token': client.cookies.get('ct0', ''),
+            'x-twitter-auth-type': 'OAuth2Client' if client.cookies.get('auth_token') else '',
         }
-        r = session.post(url, headers=headers, **kwargs)
+        client.headers.update(headers)
+        r = client.post(url, **kwargs)
         info = r.json()
 
         for task in info.get('subtasks', []):
             if task.get('enter_text', {}).get('keyboard_type') == 'email':
                 print(f"[{YELLOW}warning{RESET}] {' '.join(find_key(task, 'text'))}")
-                session.cookies.set('confirm_email', 'true')  # signal that email challenge must be solved
+                client.cookies.set('confirm_email', 'true')  # signal that email challenge must be solved
 
             if task.get('subtask_id') == 'LoginAcid':
                 if task['enter_text']['hint_text'].casefold() == 'confirmation code':
                     print(f"[{YELLOW}warning{RESET}] email confirmation code challenge.")
-                    session.cookies.set('confirmation_code', 'true')
+                    client.cookies.set('confirmation_code', 'true')
 
-        session.cookies.set(key, info[key])
+        client.cookies.set(key, info[key])
 
     except KeyError as e:
-        session.cookies.set('flow_errors', 'true')  # signal that an error occurred somewhere in the flow
+        client.cookies.set('flow_errors', 'true')  # signal that an error occurred somewhere in the flow
         print(f'[{RED}error{RESET}] failed to update token at {BOLD}{caller_name}{RESET}\n{e}')
-    return session
+    return client
 
 
-def init_guest_token(session: Client) -> Client:
-    return update_token(session, 'guest_token', 'https://api.twitter.com/1.1/guest/activate.json')
+def init_guest_token(client: Client) -> Client:
+    return update_token(client, 'guest_token', 'https://api.twitter.com/1.1/guest/activate.json')
 
 
-def flow_start(session: Client) -> Client:
-    return update_token(session, 'flow_token', 'https://api.twitter.com/1.1/onboarding/task.json',
+def flow_start(client: Client) -> Client:
+    return update_token(client, 'flow_token', 'https://api.twitter.com/1.1/onboarding/task.json',
                         params={'flow_name': 'login'},
                         json={
                             "input_flow_data": {
                                 "flow_context": {
                                     "debug_overrides": {},
                                     "start_location": {"location": "splash_screen"}
                                 }
                             }, "subtask_versions": {}
                         })
 
 
-def flow_instrumentation(session: Client) -> Client:
-    return update_token(session, 'flow_token', 'https://api.twitter.com/1.1/onboarding/task.json', json={
-        "flow_token": session.cookies.get('flow_token'),
+def flow_instrumentation(client: Client) -> Client:
+    return update_token(client, 'flow_token', 'https://api.twitter.com/1.1/onboarding/task.json', json={
+        "flow_token": client.cookies.get('flow_token'),
         "subtask_inputs": [{
             "subtask_id": "LoginJsInstrumentationSubtask",
             "js_instrumentation": {"response": "{}", "link": "next_link"}
         }],
     })
 
 
-def flow_username(session: Client) -> Client:
-    return update_token(session, 'flow_token', 'https://api.twitter.com/1.1/onboarding/task.json', json={
-        "flow_token": session.cookies.get('flow_token'),
+def flow_username(client: Client) -> Client:
+    return update_token(client, 'flow_token', 'https://api.twitter.com/1.1/onboarding/task.json', json={
+        "flow_token": client.cookies.get('flow_token'),
         "subtask_inputs": [{
             "subtask_id": "LoginEnterUserIdentifierSSO",
             "settings_list": {
                 "setting_responses": [{
                     "key": "user_identifier",
-                    "response_data": {"text_data": {"result": session.cookies.get('username')}}
+                    "response_data": {"text_data": {"result": client.cookies.get('username')}}
                 }], "link": "next_link"}}],
     })
 
 
-def flow_password(session: Client) -> Client:
-    return update_token(session, 'flow_token', 'https://api.twitter.com/1.1/onboarding/task.json', json={
-        "flow_token": session.cookies.get('flow_token'),
+def flow_password(client: Client) -> Client:
+    return update_token(client, 'flow_token', 'https://api.twitter.com/1.1/onboarding/task.json', json={
+        "flow_token": client.cookies.get('flow_token'),
         "subtask_inputs": [{
             "subtask_id": "LoginEnterPassword",
-            "enter_password": {"password": session.cookies.get('password'), "link": "next_link"}}]
+            "enter_password": {"password": client.cookies.get('password'), "link": "next_link"}}]
     })
 
 
-def flow_duplication_check(session: Client) -> Client:
-    return update_token(session, 'flow_token', 'https://api.twitter.com/1.1/onboarding/task.json', json={
-        "flow_token": session.cookies.get('flow_token'),
+def flow_duplication_check(client: Client) -> Client:
+    return update_token(client, 'flow_token', 'https://api.twitter.com/1.1/onboarding/task.json', json={
+        "flow_token": client.cookies.get('flow_token'),
         "subtask_inputs": [{
             "subtask_id": "AccountDuplicationCheck",
             "check_logged_in_account": {"link": "AccountDuplicationCheck_false"},
         }],
     })
 
 
-def confirm_email(session: Client) -> Client:
-    return update_token(session, 'flow_token', 'https://api.twitter.com/1.1/onboarding/task.json', json={
-        "flow_token": session.cookies.get('flow_token'),
+def confirm_email(client: Client) -> Client:
+    return update_token(client, 'flow_token', 'https://api.twitter.com/1.1/onboarding/task.json', json={
+        "flow_token": client.cookies.get('flow_token'),
         "subtask_inputs": [
             {
                 "subtask_id": "LoginAcid",
                 "enter_text": {
-                    "text": session.cookies.get('email'),
+                    "text": client.cookies.get('email'),
                     "link": "next_link"
                 }
             }]
     })
 
 
-def solve_confirmation_challenge(session: Client, email: str, password: str) -> Client:
-    proton_session = init_session(email, password)
+def solve_confirmation_challenge(client: Client, email: str, password: str) -> Client:
+    proton_session = init_protonmail_session(email, password)
     inbox = get_inbox(proton_session)
     confirmation_code = get_confirmation_code(inbox)
     print(f'{confirmation_code = }')
-    return update_token(session, 'flow_token', 'https://api.twitter.com/1.1/onboarding/task.json', json={
-        "flow_token": session.cookies.get('flow_token'),
+    return update_token(client, 'flow_token', 'https://api.twitter.com/1.1/onboarding/task.json', json={
+        "flow_token": client.cookies.get('flow_token'),
         'subtask_inputs': [
             {
                 'subtask_id': 'LoginAcid',
                 'enter_text': {
                     'text': confirmation_code,
                     'link': 'next_link',
                 },
             },
         ],
     })
 
 
-def execute_login_flow(session: Client) -> Client | None:
-    session = init_guest_token(session)
+def execute_login_flow(client: Client) -> Client | None:
+    client = init_guest_token(client)
     for fn in [flow_start, flow_instrumentation, flow_username, flow_password, flow_duplication_check]:
-        session = fn(session)
+        client = fn(client)
 
     # solve email challenge
-    if session.cookies.get('confirm_email') == 'true':
-        session = confirm_email(session)
+    if client.cookies.get('confirm_email') == 'true':
+        client = confirm_email(client)
 
     # solve confirmation challenge (Proton Mail only)
-    if session.cookies.get('confirmation_code') == 'true':
-        if not session.protonmail:
+    if client.cookies.get('confirmation_code') == 'true':
+        if not client.protonmail:
             print(f'[{RED}warning{RESET}] Please check your email for a confirmation code'
                   f' and log in again using the web app. If you wish to automatically solve'
                   f' email confirmation challenges, add a Proton Mail account in your account settings')
             return
-        session = solve_confirmation_challenge(session, *session.protonmail.values())
-    return session
+        time.sleep(10)  # todo: just poll the inbox until it arrives instead of waiting
+        client = solve_confirmation_challenge(client, *client.protonmail.values())
+    return client
 
 
 def login(email: str, username: str, password: str, **kwargs) -> Client:
-    session = Client()
-    session.cookies.update({
-        "email": email,
-        "username": username,
-        "password": password,
-        "guest_token": None,
-        "flow_token": None,
-    })
-    session.protonmail = kwargs.get('protonmail')
-    session = execute_login_flow(session)
-    if not session or session.cookies.get('flow_errors') == 'true':
-        print(f'[{RED}error{RESET}] {BOLD}{username}{RESET} login failed')
-    else:
-        print(f'[{GREEN}success{RESET}] {BOLD}{username}{RESET} login success')
-    return session
+    client = Client(
+        cookies={
+            "email": email,
+            "username": username,
+            "password": password,
+            "guest_token": None,
+            "flow_token": None,
+        },
+        headers={
+            'authorization': 'Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs%3D1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA',
+            'content-type': 'application/json',
+            'user-agent': 'Mozilla/5.0 (Linux; Android 11; Nokia G20) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.88 Mobile Safari/537.36',
+            'x-twitter-active-user': 'yes',
+            'x-twitter-client-language': 'en',
+        })
+    client.protonmail = kwargs.get('protonmail')
+    client = execute_login_flow(client)
+    if kwargs.get('debug', True):
+        if not client or client.cookies.get('flow_errors') == 'true':
+            print(f'[{RED}error{RESET}] {BOLD}{username}{RESET} login failed')
+        else:
+            print(f'[{GREEN}success{RESET}] {BOLD}{username}{RESET} login success')
+    return client
```

### Comparing `twitter-api-client-0.8.3/twitter/scraper.py` & `twitter-api-client-0.8.4/twitter/util.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,299 +1,281 @@
-import asyncio
-import logging.config
-import math
-import platform
+import re
 import time
-from concurrent.futures import ThreadPoolExecutor, as_completed
 from logging import Logger
 from pathlib import Path
-from urllib.parse import urlsplit
+from urllib.parse import urlsplit, urlencode, urlunsplit, parse_qs, quote
 
-import httpx
 import orjson
-from httpx import AsyncClient, Response
-from tqdm import tqdm
+import protonmail
+from httpx import Response, Client
 
-from .constants import *
-from .login import login
-from .util import find_key, save_data, get_cursor, get_headers, set_qs, fmt_status
-
-try:
-    if get_ipython().__class__.__name__ == 'ZMQInteractiveShell':
-        import nest_asyncio
-
-        nest_asyncio.apply()
-except:
-    ...
+from .constants import GREEN, MAGENTA, RED, RESET
 
-if platform.system() != 'Windows':
-    try:
-        import uvloop
-
-        uvloop.install()
-    except ImportError as e:
-        ...
-
-
-class Scraper:
-    def __init__(self, email: str, username: str, password: str, **kwargs):
-        self.session = login(email, username, password, **kwargs)
-        self.api = 'https://twitter.com/i/api/graphql'
-        self.save = kwargs.get('save', True)
-        self.debug = kwargs.get('debug', 0)
-        self.logger = self.init_logger(kwargs.get('log_config', False))
-
-    @staticmethod
-    def init_logger(cfg: dict) -> Logger:
-        logging.config.dictConfig(cfg or log_config)
-        return logging.getLogger(__name__)
-
-    def users(self, screen_names: list[str]) -> list:
-        return self._run(screen_names, Operation.UserByScreenName)
-
-    def tweets_by_id(self, tweet_ids: list[int]) -> list[dict]:
-        return self._run(tweet_ids, Operation.TweetResultByRestId)
-
-    def tweets_details(self, tweet_ids: list[int], limit=math.inf) -> list[dict]:
-        return self._run(tweet_ids, Operation.TweetDetail, limit)
-
-    def tweets(self, user_ids: list[int], limit=math.inf) -> list[dict]:
-        return self._run(user_ids, Operation.UserTweets, limit)
-
-    def tweets_and_replies(self, user_ids: list[int], limit=math.inf) -> list[dict]:
-        return self._run(user_ids, Operation.UserTweetsAndReplies, limit)
-
-    def media(self, user_ids: list[int], limit=math.inf) -> list[dict]:
-        return self._run(user_ids, Operation.UserMedia, limit)
-
-    def likes(self, user_ids: list[int], limit=math.inf) -> list[dict]:
-        return self._run(user_ids, Operation.Likes, limit)
-
-    def followers(self, user_ids: list[int], limit=math.inf) -> list[dict]:
-        return self._run(user_ids, Operation.Followers, limit)
-
-    # auth required
-    def following(self, user_ids: list[int], limit=math.inf) -> list[dict]:
-        return self._run(user_ids, Operation.Following, limit)
-
-    # auth required
-    def favoriters(self, tweet_ids: list[int], limit=math.inf) -> list[dict]:
-        return self._run(tweet_ids, Operation.Favoriters, limit)
-
-    # auth required
-    def retweeters(self, tweet_ids: list[int], limit=math.inf) -> list[dict]:
-        return self._run(tweet_ids, Operation.Retweeters, limit)
-
-    def profile_spotlights(self, screen_names: list[str]) -> list:
-        """
-        This endpoint is included for completeness only. It returns very few data points.
-        Use the batched query `users_by_ids` instead if you wish to pull user profile data.
-        """
-        return self._run(screen_names, Operation.ProfileSpotlightsQuery)
-
-    def users_by_id(self, user_ids: list[int]) -> list[dict]:
-        """
-        This endpoint is included for completeness only.
-        Use the batched query `users_by_ids` instead if you wish to pull user profile data.
-        """
-        return self._run(user_ids, Operation.UserByRestId)
-
-    def tweet_stats(self, user_ids: list[int]) -> list[dict]:
-        return self._run(user_ids, Operation.TweetStats)
-
-    def recommended_users(self, user_id: int = None) -> dict:
-        qid, op, key = Operation.ConnectTabTimeline
-        context = {"contextualUserId": user_id} if user_id else {}
-        params = {k: orjson.dumps(v).decode() for k, v in {
-            'variables': Operation.default_variables | {key: orjson.dumps(context).decode()},
-            'features': Operation.default_features,
-        }.items()}
-        r = self.session.get(f'{self.api}/{qid}/{op}', headers=get_headers(self.session), params=params)
-        txt = r.text
-        data = r.json()
-        if self.debug:
-            self.log(r, txt, data)
-        if self.save:
-            save_data(data, op, user_id)
-        return data
-
-    # special case, batch query
-    def users_by_ids(self, user_ids: list[int]) -> dict:
-        """
-        Get user data in batches
-
-        Batch-size limited to around 200-300 users
-        """
-        qid, op, key = Operation.UsersByRestIds
-        params = {k: orjson.dumps(v).decode() for k, v in {
-            'variables': Operation.default_variables | {key: user_ids},
-            'features': Operation.default_features,
-        }.items()}
-        r = self.session.get(f'{self.api}/{qid}/{op}', headers=get_headers(self.session), params=params)
-        txt = r.text
-        data = r.json()
-        if self.debug:
-            self.log(r, txt, data)
-        if self.save:
-            save_data(data, op, user_ids[0])
-        return data
-
-    def _run(self, ids: list[int | str], operation: tuple, limit=None):
-        return asyncio.run(self._process(ids, operation, limit))
-
-    async def _process(self, ids: list[int | str], op: tuple, limit: int | None) -> list:
-        async with AsyncClient(headers=get_headers(self.session)) as s:
-            return await asyncio.gather(*(self._paginate(s, _id, op, limit) for _id in ids))
-
-    async def _paginate(self, session: AsyncClient, _id: int | str, operation: tuple,
-                        limit: int | None, **kwargs) -> list[dict] | tuple[list[dict], str]:
-
-        cursor = kwargs.get('cursor')
-        is_resuming = False
-        dups = 0
-        DUP_LIMIT = 3
-
-        if cursor:
-            is_resuming = True
-            res = []
-            ids = set()
-        else:
-            r = await self._query(session, _id, operation)
-            initial_data = r.json()
-            res = [initial_data]
-            ids = set(find_key(initial_data, 'rest_id'))
-            cursor = get_cursor(initial_data)
-
-        while (dups < DUP_LIMIT) and cursor:
-            prev_len = len(ids)
-            if prev_len >= limit:
-                # return res
-                break
 
-            r = await self._query(session, _id, operation, cursor=cursor)
-            data = r.json()
+def init_session():
+    client = Client(headers={
+        'authorization': 'Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs=1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA',
+        'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36',
+    })
+    r = client.post('https://api.twitter.com/1.1/guest/activate.json').json()
+    client.headers.update({
+        'content-type': 'application/json',
+        'x-guest-token': r['guest_token'],
+        'x-twitter-active-user': 'yes',
+    })
+    return client
+
+
+def batch_ids(ids: list[int], char_limit: int = 4_500) -> list[dict]:
+    """ To avoid 431 errors """
+    length = 0
+    res, batch = [], []
+    for x in map(str, ids):
+        curr_length = len(x)
+        if length + curr_length > char_limit:
+            res.append(batch)
+            batch = []
+            length = 0
+        batch.append(x)
+        length += curr_length
+    if batch:
+        res.append(batch)
+    return res
 
-            cursor = get_cursor(data)
-            ids |= set(find_key(data, 'rest_id'))
 
-            if self.debug:
-                self.logger.debug(f'cursor: {cursor}\tunique results: {len(ids)}')
+def build_params(params: dict) -> dict:
+    return {k: orjson.dumps(v).decode() for k, v in params.items()}
 
-            if prev_len == len(ids):
-                dups += 1
 
-            res.append(data)
-
-        if is_resuming:
-            return res, cursor
-        return res
-
-    def resume_pagination(self, *args, **kwargs):
-        async def _resume(session: AsyncClient, _id: int | str, operation: tuple, limit=math.inf, **kwargs) -> tuple:
-            session = AsyncClient(headers=get_headers(session), cookies=self.session.cookies)
-            return await self._paginate(session, _id, operation, limit, **kwargs)
-
-        return asyncio.run(_resume(*args, **kwargs))
-
-    async def _query(self, session: AsyncClient, _id: int | str | list, operation: tuple, **kwargs) -> Response:
-        qid, op, k = operation
-        params = {k: orjson.dumps(v).decode() for k, v in {
-            'variables': {k: _id} | Operation.default_variables | kwargs,
-            'features': Operation.default_features,
-        }.items()}
-        r = await session.get(f'{self.api}/{qid}/{op}', params=params)
-        txt = r.text
+def save_json(r: Response, path: Path, name: str, **kwargs):
+    try:
         data = r.json()
-        if self.debug:
-            self.log(r, txt, data)
-        if self.save:
-            save_data(data, op, _id[0] if isinstance(_id, list) else _id)
-        return r
-
-    def download_media(self, ids: list[int], photos: bool = True, videos: bool = True) -> None:
-        tweets = self.tweets_by_id(ids)
-        urls = []
-        for tweet in tweets:
-            tweet_id = find_key(tweet, 'id_str')[0]
-            url = f'https://twitter.com/i/status/{tweet_id}'  # `i` evaluates to screen_name
-            media = [y for x in find_key(tweet, 'media') for y in x]
-            if photos:
-                photo_urls = list({u for m in media if 'ext_tw_video_thumb' not in (u := m['media_url_https'])})
-                [urls.append([url, photo]) for photo in photo_urls]
-            if videos:
-                video_urls = [x['variants'] for m in media if (x := m.get('video_info'))]
-                hq_videos = {sorted(v, key=lambda d: d.get('bitrate', 0))[-1]['url'] for v in video_urls}
-                [urls.append([url, video]) for video in hq_videos]
-
-        with tqdm(total=len(urls), desc='downloading media') as pbar:
-            with ThreadPoolExecutor(max_workers=32) as e:
-                for future in as_completed(e.submit(self._download, x, y) for x, y in urls):
-                    future.result()
-                    pbar.update()
-
-    def _download(self, post_url: str, cdn_url: str, path: str = 'media', chunk_size: int = 4096) -> None:
-        Path(path).mkdir(parents=True, exist_ok=True)
-        name = urlsplit(post_url).path.replace('/', '_')[1:]
-        ext = urlsplit(cdn_url).path.split('/')[-1]
+        kwargs.pop('cursor', None)
+        out = path / '_'.join(map(str, kwargs.values()))
+        out.mkdir(parents=True, exist_ok=True)
+        (out / f'{time.time_ns()}_{name}.json').write_bytes(orjson.dumps(data))
+    except Exception as e:
+        print(f'Failed to save data: {e}')
+
+
+def flatten(seq: list | tuple) -> list:
+    flat = []
+    for e in seq:
+        if isinstance(e, list | tuple):
+            flat.extend(flatten(e))
+        else:
+            flat.append(e)
+    return flat
+
+
+def get_json(res: list[Response], name: str, save=True, **kwargs) -> dict | tuple:
+    cursor = kwargs.get('cursor')
+    temp = res
+    if any(isinstance(r, (list, tuple)) for r in res):
+        temp = flatten(res)
+    for r in temp:
         try:
-            with httpx.stream('GET', cdn_url) as r:
-                with open(f'{path}/{name}_{ext}', 'wb') as f:
-                    for chunk in r.iter_bytes(chunk_size=chunk_size):
-                        f.write(chunk)
+            data = r.json()
+            # if save:
+            #     dump(data, name=name)
+
+            # parentheses very important
+            return (data, cursor) if cursor else data
         except Exception as e:
-            self.logger.debug(f'[{RED}error{RESET}] failed to download media: {post_url} {e}')
+            print('Cannot parse JSON response', e)
 
-    def trends(self) -> dict:
-        """Get trends for all UTC offsets"""
 
-        def get_trends(offset: str, url: str, headers: dict):
-            headers['x-twitter-utcoffset'] = offset
-            r = self.session.get(url, headers=headers)
-            trends = find_key(r.json(), 'item')
-            return {t['content']['trend']['name']: t for t in trends}
-
-        headers = get_headers(self.session)
-        url = set_qs('https://twitter.com/i/api/2/guide.json', trending_params)
-        offsets = [f"{str(i).zfill(3)}00" if i < 0 else f"+{str(i).zfill(2)}00" for i in range(-12, 15)]
-        trends = {}
-        with tqdm(total=len(offsets), desc='downloading trends') as pbar:
-            with ThreadPoolExecutor(max_workers=32) as e:
-                for future in as_completed(e.submit(get_trends, o, url, headers) for o in offsets):
-                    trends |= future.result()
-                    pbar.update()
-
-        path = Path(f'data/raw/trends')
-        path.mkdir(parents=True, exist_ok=True)
-        (path / f'{time.time_ns()}.json').write_text(
-            orjson.dumps(trends, option=orjson.OPT_INDENT_2).decode(),
-            encoding='utf-8'
+def set_qs(url: str, qs: dict, update=False, **kwargs) -> str:
+    *_, q, f = urlsplit(url)
+    return urlunsplit((*_, urlencode(qs | parse_qs(q) if update else qs, doseq=True, quote_via=quote,
+                                     safe=kwargs.get('safe', '')), f))
+
+
+def get_cursor(data: list | dict) -> str:
+    # inefficient, but need to deal with arbitrary schema
+    entries = find_key(data, 'entries')
+    if entries:
+        for entry in entries.pop():
+            entry_id = entry.get('entryId', '')
+            if ('cursor-bottom' in entry_id) or ('cursor-showmorethreads' in entry_id):
+                content = entry['content']
+                if itemContent := content.get('itemContent'):
+                    return itemContent['value']  # v2 cursor
+                return content['value']  # v1 cursor
+
+
+def get_headers(session, **kwargs) -> dict:
+    """
+    Get the headers required for authenticated requests
+    """
+    headers = kwargs | {
+        'authorization': 'Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs=1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA',
+        'cookie': '; '.join(f'{k}={v}' for k, v in session.cookies.items()),
+        'referer': 'https://twitter.com/',
+        'user-agent': 'Mozilla/5.0 (Linux; Android 11; Nokia G20) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.88 Mobile Safari/537.36',
+        'x-csrf-token': session.cookies.get('ct0', ''),
+        'x-guest-token': session.cookies.get('guest_token', ''),
+        'x-twitter-auth-type': 'OAuth2Session' if session.cookies.get('auth_token') else '',
+        'x-twitter-active-user': 'yes',
+        'x-twitter-client-language': 'en',
+    }
+    return dict(sorted({k.lower(): v for k, v in headers.items()}.items()))
+
+
+def find_key(obj: any, key: str) -> list:
+    """
+    Find all values of a given key within a nested dict or list of dicts
+
+    @param obj: dictionary or list of dictionaries
+    @param key: key to search for
+    @return: list of values
+    """
+
+    def helper(obj: any, key: str, L: list) -> list:
+        if not obj:
+            return L
+
+        if isinstance(obj, list):
+            for e in obj:
+                L.extend(helper(e, key, []))
+            return L
+
+        if isinstance(obj, dict) and obj.get(key):
+            L.append(obj[key])
+
+        if isinstance(obj, dict) and obj:
+            for k in obj:
+                L.extend(helper(obj[k], key, []))
+        return L
+
+    return helper(obj, key, [])
+
+
+def init_protonmail_session(email: str, password: str) -> protonmail.api.Session:
+    """
+    Create an authenticated Proton Mail session
+
+    @param email: your email. Can also use username
+    @param password: your password
+    @return: Proton Mail Session object
+    """
+    cwd = Path.cwd()
+    log_dir_path = cwd / 'protonmail_log'
+    cache_dir_path = cwd / 'protonmail_cache'
+    try:
+        session = protonmail.api.Session(
+            api_url="https://api.protonmail.ch",
+            log_dir_path=log_dir_path,
+            cache_dir_path=cache_dir_path,
+            user_agent="Ubuntu_20.04",
+            tls_pinning=False,
         )
-        return trends
+        session.enable_alternative_routing = False
+        session.authenticate(email, password)
+        return session
+    except Exception as e:
+        print('Failed to initialize Proton Mail Session:', e)
 
-    def log(self, r: Response | Response, txt: str, data: dict):
-        status = r.status_code
 
-        def stat(r):
-            if self.debug >= 1:
-                self.logger.debug(f'{r.url}')
-            if self.debug >= 2:
-                self.logger.debug(f'{txt}')
+def get_inbox(session: protonmail.api.Session) -> dict:
+    """
+    Get inbox
+
+    @param session: Proton Mail Session object
+    @return: inbox data
+    """
+    try:
+        return session.api_request(
+            "/api/mail/v4/conversations",
+            method="GET",
+            params={
+                'Page': 0,
+                'PageSize': 50,
+                'Limit': 100,
+                'LabelID': 0,
+                'Sort': 'Time',
+                'Desc': 1,
+            }
+        )
+    except Exception as e:
+        print('Failed to get inbox:', e)
+
 
+def get_verification_code(inbox: dict) -> str:
+    """
+    Get Twitter verification code from inbox.
+
+    Crude implementation. Subject line contains verification code, no need to decrypt message body.
+
+    @param inbox: inbox data
+    @return: Twitter verification code
+    """
+    try:
+        expr = '(\w+) is your Twitter verification code'
+        return list(filter(len, (re.findall(expr, conv['Subject']) for conv in inbox['Conversations'])))[0][0]
+    except Exception as e:
+        print('Failed to get Twitter verification code:', e)
+
+
+def get_confirmation_code(inbox: dict) -> str:
+    """
+    Get Twitter confirmation code from inbox.
+
+    Crude implementation. Subject line contains confirmation code, no need to decrypt message body.
+
+    @param inbox: inbox data
+    @return: Twitter confirmation code
+    """
+    try:
+        expr = 'Your Twitter confirmation code is (\w+)'
+        return list(filter(len, (re.findall(expr, conv['Subject']) for conv in inbox['Conversations'])))[0][0]
+    except Exception as e:
+        print('Failed to get Twitter confirmation code:', e)
+
+
+def log(logger: Logger, level: int, r: Response):
+    def stat(r, txt, data):
+        if level >= 1:
+            logger.debug(f'{r.url.path}')
+        if level >= 2:
+            logger.debug(f'{r.url}')
+        if level >= 3:
+            logger.debug(f'{txt}')
+        if level >= 4:
+            logger.debug(f'{data}')
+
+        try:
             limits = {k: v for k, v in r.headers.items() if 'x-rate-limit' in k}
             current_time = int(time.time())
             wait = int(r.headers.get('x-rate-limit-reset', current_time)) - current_time
-            self.logger.debug(
-                f"remaining: {MAGENTA}{limits['x-rate-limit-remaining']}/{limits['x-rate-limit-limit']}{RESET} requests")
-            self.logger.debug(f'reset:     {MAGENTA}{(wait / 60):.2f}{RESET} minutes')
+            remaining = limits.get('x-rate-limit-remaining')
+            limit = limits.get('x-rate-limit-limit')
+            logger.debug(f"remaining: {MAGENTA}{remaining}/{limit}{RESET} requests")
+            logger.debug(f'reset:     {MAGENTA}{(wait / 60):.2f}{RESET} minutes')
+        except Exception as e:
+            logger.error(f'Rate limit info unavailable: {e}')
 
-        try:
-            if 'json' in r.headers.get('content-type', ''):
-                if data.get('errors'):
-                    self.logger.debug(f'[{RED}error{RESET}] {status} {data}')
-                else:
-                    self.logger.debug(fmt_status(status))
-                    stat(r)
+    try:
+        status = r.status_code
+        txt, data, = r.text, r.json()
+        if 'json' in r.headers.get('content-type', ''):
+            if data.get('errors') and not find_key(data, 'instructions'):
+                logger.error(f'[{RED}error{RESET}] {status} {data}')
             else:
-                self.logger.debug(fmt_status(status))
-                stat(r)
-        except Exception as e:
-            self.logger.debug(f'failed to log: {e}')
+                logger.debug(fmt_status(status))
+                stat(r, txt, data)
+        else:
+            logger.debug(fmt_status(status))
+            stat(r, txt, {})
+    except Exception as e:
+        logger.error(f'Failed to log: {e}')
+
+
+def fmt_status(status: int) -> str:
+    color = None
+    if 200 <= status < 300:
+        color = GREEN
+    elif 300 <= status < 400:
+        color = MAGENTA
+    elif 400 <= status < 600:
+        color = RED
+    return f'[{color}{status}{RESET}]'
```

### Comparing `twitter-api-client-0.8.3/twitter/search.py` & `twitter-api-client-0.8.4/twitter/search.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import platform
 import random
 import time
 from logging import Logger
 from pathlib import Path
 
 import orjson
-from httpx import AsyncClient
+from httpx import AsyncClient, Client
 
 from .constants import *
 from .login import login
 from .util import set_qs, get_headers, find_key
 
 reset = '\u001b[0m'
 colors = [f'\u001b[{i}m' for i in range(30, 38)]
@@ -31,25 +31,40 @@
 
         uvloop.install()
     except ImportError as e:
         ...
 
 
 class Search:
-    def __init__(self, email: str, username: str, password: str, **kwargs):
-        self.session = login(email, username, password, **kwargs)
+    def __init__(self, email: str = None, username: str = None, password: str = None, session: Client = None, **kwargs):
+        self.logger = self.init_logger(kwargs.get('log_config', False))
+        self.session = self.validate_session(email, username, password, session, **kwargs)
         self.api = 'https://api.twitter.com/2/search/adaptive.json?'
         self.save = kwargs.get('save', True)
         self.debug = kwargs.get('debug', 0)
         self.logger = self.init_logger(kwargs.get('log_config', False))
 
     @staticmethod
     def init_logger(cfg: dict) -> Logger:
-        logging.config.dictConfig(cfg or log_config)
-        return logging.getLogger(__name__)
+        if cfg:
+            logging.config.dictConfig(cfg)
+            return logging.getLogger(__name__)
+        return logger
+
+    @staticmethod
+    def validate_session(*args, **kwargs):
+        email, username, password, session = args
+        if session and all(session.cookies.get(c) for c in {'ct0', 'auth_token'}):
+            # authenticated session provided
+            return session
+        if not session:
+            # no session provided, login to authenticate
+            return login(email, username, password, **kwargs)
+        raise Exception('Session not authenticated. '
+                        'Please use an authenticated session or remove the `session` argument and try again.')
 
     def run(self, *args, out: str = 'data', **kwargs):
         out_path = self.make_output_dirs(out)
         if kwargs.get('latest', False):
             search_config['tweet_search_mode'] = 'live'
         return asyncio.run(self.process(args, search_config, out_path, **kwargs))
```

### Comparing `twitter-api-client-0.8.3/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.8.4/twitter_api_client.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.8.3
+Version: 0.8.4
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-Implementation of Twitter's v1, v2, and GraphQL APIs
+
+## Implementation of Twitter's v1, v2, and GraphQL APIs
 
 Tools include: [Scraping](#scraping), [Account Automation](#automation), [Search](#search)
 
-Automated email challenge solvers are supported for Proton Mail accounts. See [here](#automated-solvers) for more information.
+Automated email challenge solvers are supported for **Proton Mail** accounts using [proton-python-client](https://github.com/ProtonMail/proton-python-client). See [here](#automated-solvers) for more information.
+
+## Table of Contents
 
 * [Installation](#installation)
 * [Automation](#automation)
 * [Scraping](#scraping)
-    * [Users/Tweets data](#get-all-usertweet-data)
-    * [Search](#search)
+  * [Get all user/tweet data](#get-all-usertweet-data)
+  * [Resume Pagination](#resume-pagination)
+  * [Search](#search)
+* [Spaces](#spaces)
+  * [Live Audio Capture](#live-audio-capture)
+  * [Live Transcript Capture](#live-transcript-capture)
+  * [Search and Metadata](#search-and-metadata)
 * [Automated Solvers](#automated-solvers)
 * [Example API Responses](#example-api-responses)
 
 ### Installation
 
 ```bash
 pip install twitter-api-client
@@ -193,15 +201,15 @@
 media = scraper.media([123, 234, 345])
 following = scraper.following([123, 234, 345])
 followers = scraper.followers([123, 234, 345])
 scraper.tweet_stats([111111, 222222, 333333])
 
 # get recommended users based on user
 scraper.recommended_users()
-scraper.recommended_users(123)
+scraper.recommended_users([123])
 
 # tweet data
 tweets_by_ids = scraper.tweets_by_id([987, 876, 754])
 tweets_details = scraper.tweets_details([987, 876, 754])
 retweeters = scraper.retweeters([987, 876, 754])
 favoriters = scraper.favoriters([987, 876, 754])
 
@@ -213,28 +221,26 @@
 ])
 
 # trends
 scraper.trends()
 ```
 
 #### Resume Pagination
-Pagination is already done by default, however there are circumstances where you may need to resume pagination from a specific cursor. For example, the `Followers` endpoint only allows for 50 requests every 15 minutes. In this case, we can resume from where we left off by providing a specific cursor value. This technique applies to any other endpoint defined in `twitter.constants.Operation`.
+**Pagination is already done by default**, however there are circumstances where you may need to resume pagination from a specific cursor. For example, the `Followers` endpoint only allows for 50 requests every 15 minutes. In this case, we can resume from where we left off by providing a specific cursor value.
 ```python
 from twitter.scraper import Scraper
-from twitter.constants import Operation
 
 email, username, password = ...,...,...
 scraper = Scraper(email, username, password, debug=1, save=True)
 
-operation = Operation.Followers
 user_id = 44196397
-cursor = '1765001818576065118|1654241854176100129' # example cursor
-limit = 250  # arbitrary limit for demonstration
+cursor = '1767341853908517597|1663601806447476672'  # example cursor
+limit = 100  # arbitrary limit for demonstration
+follower_subset, last_cursor = scraper.followers([user_id], limit=limit, cursor=cursor)
 
-follower_subset, last_cursor = scraper.resume_pagination(scraper.session, user_id, operation, limit=limit, cursor=cursor)
 # use last_cursor to resume pagination
 ```
 
 #### Search
 
 ```python   
 from twitter.search import Search
@@ -267,21 +273,98 @@
 
 **Search Operators Reference**
 
 https://developer.twitter.com/en/docs/twitter-api/v1/rules-and-filtering/search-operators
 
 https://developer.twitter.com/en/docs/twitter-api/tweets/search/integrate/build-a-query
 
+### Spaces
+
+#### Live Audio Capture
+
+Capture live audio for up to 500 streams per IP
+
+```python
+from twitter.scraper import Scraper
+from twitter.util import init_session
+
+session = init_session() # initialize guest session, no login required
+scraper = Scraper(session=session, debug=1, save=True)
+
+rooms = [...]
+scraper.spaces_live(rooms=rooms) # capture live audio from list of rooms
+```
+
+#### Live Transcript Capture
+
+**Raw transcript chunks**
+
+```python
+from twitter.scraper import Scraper
+from twitter.util import init_session
+
+session = init_session() # initialize guest session, no login required
+scraper = Scraper(session=session, debug=1, save=True)
+
+# room must be live, i.e. in "Running" state
+scraper.space_live_transcript('1zqKVPlQNApJB', frequency=2)  # word-level live transcript. (dirty, on-the-fly transcription before post-processing)
+```
+
+**Processed (final) transcript chunks**
+
+```python
+from twitter.scraper import Scraper
+from twitter.util import init_session
+
+session = init_session() # initialize guest session, no login required
+scraper = Scraper(session=session, debug=1, save=True)
+
+# room must be live, i.e. in "Running" state
+scraper.space_live_transcript('1zqKVPlQNApJB', frequency=1)  # finalized live transcript.  (clean)
+```
+
+#### Search and Metadata
+```python
+from twitter.scraper import Scraper
+from twitter.util import init_session
+from twitter.constants import SpaceCategory
+
+session = init_session() # initialize guest session, no login required
+scraper = Scraper(session=session, debug=1, save=True)
+
+# download audio and chat-log from space
+spaces = scraper.spaces(rooms=['1eaJbrAPnBVJX', '1eaJbrAlZjjJX'], audio=True, chat=True)
+
+# pull metadata only
+spaces = scraper.spaces(rooms=['1eaJbrAPnBVJX', '1eaJbrAlZjjJX'])
+
+# search for spaces in "Upcoming", "Top" and "Live" categories
+spaces = scraper.spaces(search=[
+    {
+        'filter': SpaceCategory.Upcoming,
+        'query': 'hello'
+    },
+    {
+        'filter': SpaceCategory.Top,
+        'query': 'world'
+    },
+    {
+        'filter': SpaceCategory.Live,
+        'query': 'foo bar'
+    }
+])
+```
 
 ### Automated Solvers
 To set up automated email confirmation/verification solvers, add your Proton Mail credentials below as shown.
 This removes the need to manually solve email challenges via the web app. These credentials can be used in `Scraper`, `Account`, and `Search` constructors.
 
 E.g.
 
 ```python
 from twitter.scraper import Scraper
 
 email, username, password = ..., ..., ...
 proton_email, proton_password = ..., ...
 account = Scraper(email, username, password, debug=1, save=True, protonmail={'email':proton_email, 'password':proton_password})
 ```
+
```

### Comparing `twitter-api-client-0.8.3/twitter_api_client.egg-info/SOURCES.txt` & `twitter-api-client-0.8.4/twitter_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

