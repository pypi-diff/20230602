# Comparing `tmp/consumableai-0.1.1-py3-none-any.whl.zip` & `tmp/consumableai-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6763 bytes, number of entries: 9
+Zip file size: 6588 bytes, number of entries: 9
 -rw-r--r--  2.0 unx        0 b- defN 23-May-29 10:28 consumableai/__init__.py
 -rw-r--r--  2.0 unx     4772 b- defN 23-Jun-01 15:59 consumableai/cli.py
--rwxr-xr-x  2.0 unx     4772 b- defN 23-Jun-01 15:59 consumableai-0.1.1.data/scripts/cli.py
--rw-r--r--  2.0 unx     1070 b- defN 23-Jun-02 08:17 consumableai-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2239 b- defN 23-Jun-02 08:17 consumableai-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-02 08:17 consumableai-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       55 b- defN 23-Jun-02 08:17 consumableai-0.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 23-Jun-02 08:17 consumableai-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      760 b- defN 23-Jun-02 08:17 consumableai-0.1.1.dist-info/RECORD
-9 files, 13773 bytes uncompressed, 5437 bytes compressed:  60.5%
+-rwxr-xr-x  2.0 unx     4772 b- defN 23-Jun-01 15:59 consumableai-1.0.0.data/scripts/cli.py
+-rw-r--r--  2.0 unx     1070 b- defN 23-Jun-02 08:23 consumableai-1.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1880 b- defN 23-Jun-02 08:23 consumableai-1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-02 08:23 consumableai-1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-02 08:23 consumableai-1.0.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-02 08:23 consumableai-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      760 b- defN 23-Jun-02 08:23 consumableai-1.0.0.dist-info/RECORD
+9 files, 13414 bytes uncompressed, 5262 bytes compressed:  60.8%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: consumableai/__init__.py
 Comment: 
 
 Filename: consumableai/cli.py
 Comment: 
 
-Filename: consumableai-0.1.1.data/scripts/cli.py
+Filename: consumableai-1.0.0.data/scripts/cli.py
 Comment: 
 
-Filename: consumableai-0.1.1.dist-info/LICENSE
+Filename: consumableai-1.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: consumableai-0.1.1.dist-info/METADATA
+Filename: consumableai-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: consumableai-0.1.1.dist-info/WHEEL
+Filename: consumableai-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: consumableai-0.1.1.dist-info/entry_points.txt
+Filename: consumableai-1.0.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: consumableai-0.1.1.dist-info/top_level.txt
+Filename: consumableai-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: consumableai-0.1.1.dist-info/RECORD
+Filename: consumableai-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `consumableai-0.1.1.data/scripts/cli.py` & `consumableai-1.0.0.data/scripts/cli.py`

 * *Files identical despite different names*

## Comparing `consumableai-0.1.1.dist-info/LICENSE` & `consumableai-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `consumableai-0.1.1.dist-info/METADATA` & `consumableai-1.0.0.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consumableai
-Version: 0.1.1
+Version: 1.0.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: pyyaml
 Requires-Dist: click
 Requires-Dist: psycopg2
 Requires-Dist: requests
@@ -16,51 +16,33 @@
 
 Consumable AI is an SDK that can be easily integrated into the self hosted BI tools which gives enterprises the power to talk to the databases in natural language. This will make exploratory data analyses easy to perform and remove the barrier of acquiring SQL skills and database know-how.
 
 ## Installation
 
 A Python library for seamless integration with ConsumableAI platform.
 
+> Right now we only support postgresql database, soon will update other databases as well
+
 To get started, follow these steps:
 
-1. Set up a virtual environment for your project:
+1. Set up a virtual environment in your aws which has access to database:
 
    $ python3 -m venv myenv
    $ source myenv/bin/activate
 
 2. Install the ConsumableAI library using pip:
 
    $ pip install consumableai
 
-   Please ensure you have a working internet connection.
-
 3. Obtain an API key by visiting [https://platform.consumableai.com](https://platform.consumableai.com) and creating an account. The API key will be used to authenticate your requests.
 
 4. Initialize the ConsumableAI library:
 
    $ consumableai init
 
    This command will prompt you to enter various database-related values. The library will create the table schema for your data. Please note that ConsumableAI does not store your data directly. Instead, it creates the table schema and shares a link to a spreadsheet. You can make changes to the spreadsheet, and when you're ready, inform us to update the schema accordingly.
 
    The spreadsheet link will be provided after initialization.
 
-5. Start utilizing the ConsumableAI library in your Python code to interact with the platform and access your data.
-
-   Example usage:
-
-   ```python
-   import consumableai
-
-   # Initialize the ConsumableAI client
-   client = consumableai.Client(api_key='YOUR_API_KEY')
-
-   # Perform operations with the client
-   ...
-   ```
-
-Replace 'YOUR_API_KEY' with the API key you obtained.
-
-For more information and documentation, please visit our website at example.com.
+For more information and documentation, please visit our website at [https://platform.consumableai.com](https://platform.consumableai.com).
 
 Happy data exploration with ConsumableAI!
-
-Feel free to modify and adapt this description to fit your specific library and instructions.
```

## Comparing `consumableai-0.1.1.dist-info/RECORD` & `consumableai-1.0.0.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 consumableai/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 consumableai/cli.py,sha256=_AnPe3MBwrK3REZYr0MJzgwxG_KSKmKWwUFCOH4PYCs,4772
-consumableai-0.1.1.data/scripts/cli.py,sha256=_AnPe3MBwrK3REZYr0MJzgwxG_KSKmKWwUFCOH4PYCs,4772
-consumableai-0.1.1.dist-info/LICENSE,sha256=-0N0XH5wv6NVSsgpJyirk1cMAGPdxSFvwryunqM5PgM,1070
-consumableai-0.1.1.dist-info/METADATA,sha256=jKfNGAvNMKeZFN_5A7HRqAJgoc4dKBpoeEaz94caVEk,2239
-consumableai-0.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-consumableai-0.1.1.dist-info/entry_points.txt,sha256=kgcQDEaQKnyao6xlJZJZT85aXHJ4mmDpOkNzAUH0lvQ,55
-consumableai-0.1.1.dist-info/top_level.txt,sha256=SCBbxRjx2Ua6WKjSn1lWC7Yel-8srL-DenNfJmWFZ9U,13
-consumableai-0.1.1.dist-info/RECORD,,
+consumableai-1.0.0.data/scripts/cli.py,sha256=_AnPe3MBwrK3REZYr0MJzgwxG_KSKmKWwUFCOH4PYCs,4772
+consumableai-1.0.0.dist-info/LICENSE,sha256=-0N0XH5wv6NVSsgpJyirk1cMAGPdxSFvwryunqM5PgM,1070
+consumableai-1.0.0.dist-info/METADATA,sha256=XHmBddlv6Q98LAdSyTe2ZXJQWxKkjjWq1Dk-fr8ERTc,1880
+consumableai-1.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+consumableai-1.0.0.dist-info/entry_points.txt,sha256=kgcQDEaQKnyao6xlJZJZT85aXHJ4mmDpOkNzAUH0lvQ,55
+consumableai-1.0.0.dist-info/top_level.txt,sha256=SCBbxRjx2Ua6WKjSn1lWC7Yel-8srL-DenNfJmWFZ9U,13
+consumableai-1.0.0.dist-info/RECORD,,
```

