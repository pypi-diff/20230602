# Comparing `tmp/tidy_tweet-1.0.0a1.tar.gz` & `tmp/tidy_tweet-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidy_tweet-1.0.0a1.tar", last modified: Thu May 25 00:46:45 2023, max compression
+gzip compressed data, was "tidy_tweet-1.0.0a2.tar", last modified: Fri Jun  2 05:18:21 2023, max compression
```

## Comparing `tidy_tweet-1.0.0a1.tar` & `tidy_tweet-1.0.0a2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:46:45.739817 tidy_tweet-1.0.0a1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:46:45.731817 tidy_tweet-1.0.0a1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:46:45.735818 tidy_tweet-1.0.0a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/.github/workflows/pypi_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-05-25 00:46:45.739817 tidy_tweet-1.0.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:46:45.735818 tidy_tweet-1.0.0a1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    14737 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/docs/data_model.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    39299 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/docs/data_model.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/docs/schema.md
--rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/generate_schema_diagram.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-25 00:46:45.739817 tidy_tweet-1.0.0a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:46:45.731817 tidy_tweet-1.0.0a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:46:45.735818 tidy_tweet-1.0.0a1/src/tidy_tweet/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/src/tidy_tweet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/src/tidy_tweet/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-25 00:46:45.000000 tidy_tweet-1.0.0a1/src/tidy_tweet/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/src/tidy_tweet/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/src/tidy_tweet/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    16794 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/src/tidy_tweet/tweet_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/src/tidy_tweet/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:46:45.735818 tidy_tweet-1.0.0a1/src/tidy_tweet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-05-25 00:46:45.000000 tidy_tweet-1.0.0a1/src/tidy_tweet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-25 00:46:45.000000 tidy_tweet-1.0.0a1/src/tidy_tweet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 00:46:45.000000 tidy_tweet-1.0.0a1/src/tidy_tweet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-25 00:46:45.000000 tidy_tweet-1.0.0a1/src/tidy_tweet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-25 00:46:45.000000 tidy_tweet-1.0.0a1/src/tidy_tweet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 00:46:45.000000 tidy_tweet-1.0.0a1/src/tidy_tweet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:46:45.735818 tidy_tweet-1.0.0a1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:46:45.739817 tidy_tweet-1.0.0a1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   586918 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/tests/data/ObservatoryTeam.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-25 00:46:27.000000 tidy_tweet-1.0.0a1/tests/test_overall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:18:21.278354 tidy_tweet-1.0.0a2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:18:21.270354 tidy_tweet-1.0.0a2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:18:21.274354 tidy_tweet-1.0.0a2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/.github/workflows/pypi_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-06-02 05:18:21.278354 tidy_tweet-1.0.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:18:21.274354 tidy_tweet-1.0.0a2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    14737 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/docs/data_model.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    39299 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/docs/data_model.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/docs/schema.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/generate_schema_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-02 05:18:21.278354 tidy_tweet-1.0.0a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:18:21.270354 tidy_tweet-1.0.0a2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:18:21.274354 tidy_tweet-1.0.0a2/src/tidy_tweet/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/src/tidy_tweet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/src/tidy_tweet/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-02 05:18:21.000000 tidy_tweet-1.0.0a2/src/tidy_tweet/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/src/tidy_tweet/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/src/tidy_tweet/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17759 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/src/tidy_tweet/tweet_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/src/tidy_tweet/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:18:21.274354 tidy_tweet-1.0.0a2/src/tidy_tweet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-06-02 05:18:21.000000 tidy_tweet-1.0.0a2/src/tidy_tweet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-02 05:18:21.000000 tidy_tweet-1.0.0a2/src/tidy_tweet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 05:18:21.000000 tidy_tweet-1.0.0a2/src/tidy_tweet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-02 05:18:21.000000 tidy_tweet-1.0.0a2/src/tidy_tweet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-02 05:18:21.000000 tidy_tweet-1.0.0a2/src/tidy_tweet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-02 05:18:21.000000 tidy_tweet-1.0.0a2/src/tidy_tweet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:18:21.274354 tidy_tweet-1.0.0a2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:18:21.274354 tidy_tweet-1.0.0a2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   586918 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/tests/data/ObservatoryTeam.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/tests/test_overall.py
```

### Comparing `tidy_tweet-1.0.0a1/.github/workflows/pypi_publish.yml` & `tidy_tweet-1.0.0a2/.github/workflows/pypi_publish.yml`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a1/.github/workflows/tests.yml` & `tidy_tweet-1.0.0a2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a1/LICENSE` & `tidy_tweet-1.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a1/PKG-INFO` & `tidy_tweet-1.0.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy_tweet
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Tidies Twitter json collected with Twarc into relational tables
 Home-page: https://github.com/QUT-Digital-Observatory/tidy_tweet
 Author: QUT Digital Observatory
 Author-email: digitalobservatory@qut.edu.au
 Project-URL: Bug Tracker, https://github.com/QUT-Digital-Observatory/tidy_tweet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidy_tweet-1.0.0a1/README.md` & `tidy_tweet-1.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a1/contributing.md` & `tidy_tweet-1.0.0a2/contributing.md`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a1/docs/data_model.drawio` & `tidy_tweet-1.0.0a2/docs/data_model.drawio`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a1/docs/data_model.svg` & `tidy_tweet-1.0.0a2/docs/data_model.svg`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a1/docs/schema.md` & `tidy_tweet-1.0.0a2/docs/schema.md`

 * *Files 10% similar despite different names*

```diff
@@ -47,30 +47,30 @@
         integer width
         text type
         integer duration_ms
         integer view_count
         string alt_text
         text media_key PK
     }
-    "user" {
+    "user_by_page" {
         text name
         text profile_image_url
         text id PK
         text created_at
         text protected
         text description
         text location
         text pinned_tweet_id
         integer verified
         text url
         text username
         integer page_id PK, FK
         text source_file FK
     }
-    "tweet" {
+    "tweet_by_page" {
         text id PK
         integer page_id PK, FK
         text reply_settings
         text conversation_id
         text created_at
         text retweeted_tweet_id FK
         text quoted_tweet_id FK
@@ -103,23 +103,23 @@
     }
     tweet_url |o--o{ tweet : "tweet"
     user_url |o--o{ user : "user"
     tweet_hashtag |o--o{ tweet : "tweet"
     user_hashtag |o--o{ user : "user"
     tweet_mention |o--o{ tweet : "tweet"
     user_mention |o--o{ user : "user"
-    user |o--o{ results_page : "page"
-    user |o--o{ results_page : "source file"
-    tweet |o--o{ results_page : "page"
-    tweet |o--o{ tweet : "retweeted tweet"
-    tweet |o--o{ tweet : "quoted tweet"
-    tweet |o--o{ tweet : "replied to tweet"
-    tweet |o--o{ user : "in reply to user"
-    tweet |o--o{ user : "author"
-    tweet |o--o{ results_page : "source file"
+    user_by_page |o--o{ results_page : "page"
+    user_by_page |o--o{ results_page : "source file"
+    tweet_by_page |o--o{ results_page : "page"
+    tweet_by_page |o--o{ tweet : "retweeted tweet"
+    tweet_by_page |o--o{ tweet : "quoted tweet"
+    tweet_by_page |o--o{ tweet : "replied to tweet"
+    tweet_by_page |o--o{ user : "in reply to user"
+    tweet_by_page |o--o{ user : "author"
+    tweet_by_page |o--o{ results_page : "source file"
 ```
 
 Table **tweet_url**:
 
 - **tweet_id** (text primary key references tweet (id))
 - **field** (text not null): e.g. "description", "text" - which field of the source object the URL is in
 - **url** (text primary key not null): t.co shortened URL
@@ -187,15 +187,15 @@
 - **type** (text)
 - **duration_ms** (integer)
 - **view_count** (integer)
 - **alt_text** (string)
 - **media_key** (text primary key)
 
 
-Table **user**:
+Table **user_by_page**:
 
 - **name** (text)
 - **profile_image_url** (text)
 - **id** (text primary key )
 - **created_at** (text)
 - **protected** (text)
 - **description** (text)
@@ -206,15 +206,15 @@
 - **username** (text)
 - **page_id** (integer primary key references results_page (id))
 - **source_file** (text references results_page (filename))
 
 primary key 
 
 
-Table **tweet**:
+Table **tweet_by_page**:
 
 - **id** (text primary key )
 - **page_id** (integer primary key references results_page (id))
 - **reply_settings** (text)
 - **conversation_id** (text)
 - **created_at** (text)
 - **retweeted_tweet_id** (text references tweet (id))
```

### Comparing `tidy_tweet-1.0.0a1/generate_schema_diagram.py` & `tidy_tweet-1.0.0a2/generate_schema_diagram.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a1/setup.cfg` & `tidy_tweet-1.0.0a2/setup.cfg`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a1/src/tidy_tweet/__main__.py` & `tidy_tweet-1.0.0a2/src/tidy_tweet/__main__.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a1/src/tidy_tweet/database.py` & `tidy_tweet-1.0.0a2/src/tidy_tweet/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,18 @@
             assert len(created_tables) == len(mapping.create_table_statements)
             cursor.execute("create table schema_version (schema_version text)")
             cursor.execute(
                 "insert into schema_version values (:version)",
                 {"version": mapping.SCHEMA_VERSION},
             )
 
+        # Create views
+        for view_sql in mapping.sql_views.values():
+            cursor.execute(view_sql)
+
         logger.info("The database schema has been initialised")
 
 
 def check_database_version(db_name):
     """
     Checks the given pre-existing database is valid for use with this version
     of the tidy_tweet library.
```

### Comparing `tidy_tweet-1.0.0a1/src/tidy_tweet/processing.py` & `tidy_tweet-1.0.0a2/src/tidy_tweet/processing.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a1/src/tidy_tweet/tweet_mapping.py` & `tidy_tweet-1.0.0a2/src/tidy_tweet/tweet_mapping.py`

 * *Files 9% similar despite different names*

```diff
@@ -301,17 +301,17 @@
 
 
 # places - TODO
 
 # users
 # TODO: Fields not included yet:
 # - public_metrics
-sql_by_table["user"] = {
+sql_by_table["user_by_page"] = {
     "create": """
-create table user (
+create table user_by_page (
     name text,
     profile_image_url text,
     id text,
     created_at text,
     protected text,
     description text,
     location text,
@@ -321,31 +321,49 @@
     username text,
     page_id integer references results_page (id),
     source_file text references results_page (filename),
     primary key (id, page_id)
 )
     """,
     "insert": """
-insert or ignore into user (
+insert or ignore into user_by_page (
     id, username, name, url,
     profile_image_url, description,
     created_at,
     protected, verified,
     location,
-    pinned_tweet_id
+    pinned_tweet_id,
+    page_id, source_file
 ) values (
     :id, :username, :name, :url,
     :profile_image_url, :description,
     :created_at,
     :protected, :verified,
     :location,
-    :pinned_tweet_id
+    :pinned_tweet_id,
+    :page_id, :source_file
 )
     """,
 }
+sql_views[
+    "user"
+] = """
+create view user as
+select
+    id, username, name, url,
+    profile_image_url, description,
+    created_at,
+    protected, verified,
+    location,
+    pinned_tweet_id,
+    max(retrieved_at) as retrieved_at
+from user_by_page
+left join results_page on user_by_page.page_id = results_page.id
+group by user_by_page.id
+"""
 
 
 def map_user(user_json, source_file, page_id) -> Dict[str, List[Dict]]:
     user_map = {
         "id": user_json["id"],
         "username": user_json["username"],
         "name": user_json["name"],
@@ -357,15 +375,15 @@
         "verified": user_json["verified"],
         "location": user_json.get("location", None),
         "pinned_tweet_id": user_json.get("pinned_tweet_id", None),
         "source_file": source_file,
         "page_id": page_id,
     }
 
-    mappings = {"user": [user_map]}
+    mappings = {"user_by_page": [user_map]}
 
     # Entities
     if "entities" in user_json:
         for field, entities in user_json["entities"].items():
             add_mappings(
                 mappings, map_entities(user_json["id"], "user", field, entities)
             )
@@ -374,17 +392,17 @@
 
 
 # --- tweet tables ---
 # TODO: fields not yet included:
 # - entities
 # - context_annotations
 
-sql_by_table["tweet"] = {
+sql_by_table["tweet_by_page"] = {
     "create": """
-create table tweet (
+create table tweet_by_page (
     id text,
     page_id integer references results_page (id),
     reply_settings text,
     conversation_id text,
     created_at text,
     retweeted_tweet_id text references tweet (id),
     quoted_tweet_id text references tweet (id),
@@ -401,15 +419,15 @@
     retweet_count integer,
     source_file text references results_page (filename),
     directly_collected integer, -- boolean
     primary key (id, page_id)
 )
     """,
     "insert": """
-insert or ignore into tweet (
+insert or ignore into tweet_by_page (
     id, author_id,
     text, lang, source,
     possibly_sensitive, reply_settings,
     created_at,
     conversation_id,
     retweeted_tweet_id,
     quoted_tweet_id,
@@ -428,14 +446,34 @@
     :replied_to_tweet_id,
     :in_reply_to_user_id,
     :like_count, :quote_count, :reply_count, :retweet_count,
     :directly_collected, :source_file, :page_id
 )
     """,
 }
+sql_views[
+    "tweet"
+] = """
+create view tweet as
+select
+    tweet_by_page.id, author_id,
+    text, lang, source,
+    possibly_sensitive, reply_settings,
+    created_at,
+    conversation_id,
+    retweeted_tweet_id,
+    quoted_tweet_id,
+    replied_to_tweet_id,
+    in_reply_to_user_id,
+    like_count, quote_count, reply_count, retweet_count,
+    max(retrieved_at) as retrieved_at
+from tweet_by_page
+left join results_page on tweet_by_page.page_id = results_page.id
+group by tweet_by_page.id
+"""
 
 
 def map_tweet(
     tweet_json, directly_collected: bool, source_file: str, page_id
 ) -> Dict[str, List[Dict]]:
     tweet_map = {
         "id": tweet_json["id"],
@@ -475,15 +513,15 @@
                 qt_id = t["id"]
             elif t["type"] == "replied_to":
                 replied_to_id = t["id"]
     tweet_map["retweeted_tweet_id"] = rt_id
     tweet_map["quoted_tweet_id"] = qt_id
     tweet_map["replied_to_tweet_id"] = replied_to_id
 
-    mappings = {"tweet": [tweet_map]}
+    mappings = {"tweet_by_page": [tweet_map]}
 
     # Entities
     if "entities" in tweet_json:
         add_mappings(
             mappings,
             map_entities(tweet_json["id"], "tweet", "text", tweet_json["entities"]),
         )
@@ -553,15 +591,15 @@
     metadata["tidy_tweet_version"] = version
 
     # Twitter result page metadata
     key_columns = ["oldest_id", "newest_id", "result_count"]
     for key in key_columns:
         metadata[key] = page_metadata_json.pop(key, None)
 
-    # Twarc metadata
+    # Twarc metadatas
     metadata["twarc_version"] = twarc_metadata_json.pop("version", None)
     metadata["request_url"] = twarc_metadata_json.pop("url", None)
     metadata["retrieved_at"] = twarc_metadata_json.pop("retrieved_at")
 
     # Any unexpected items in either metadata should be retained
     extras = {}
```

### Comparing `tidy_tweet-1.0.0a1/src/tidy_tweet/utilities.py` & `tidy_tweet-1.0.0a2/src/tidy_tweet/utilities.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a1/src/tidy_tweet.egg-info/PKG-INFO` & `tidy_tweet-1.0.0a2/src/tidy_tweet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy-tweet
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Tidies Twitter json collected with Twarc into relational tables
 Home-page: https://github.com/QUT-Digital-Observatory/tidy_tweet
 Author: QUT Digital Observatory
 Author-email: digitalobservatory@qut.edu.au
 Project-URL: Bug Tracker, https://github.com/QUT-Digital-Observatory/tidy_tweet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidy_tweet-1.0.0a1/src/tidy_tweet.egg-info/SOURCES.txt` & `tidy_tweet-1.0.0a2/src/tidy_tweet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a1/tests/data/ObservatoryTeam.jsonl` & `tidy_tweet-1.0.0a2/tests/data/ObservatoryTeam.jsonl`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a1/tests/test_cli.py` & `tidy_tweet-1.0.0a2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a1/tests/test_overall.py` & `tidy_tweet-1.0.0a2/tests/test_overall.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     with sqlite3.connect(db_path) as conn:
         db = conn.cursor()
 
         # Check number of tweets
         db.execute(
             """
             select directly_collected, count(*)
-            from tweet
+            from tweet_by_page
             group by directly_collected;
          """
         )
 
         for directly_collected, num_tweets in db:
             if directly_collected == 0:
                 assert num_tweets == 177
```

