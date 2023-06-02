# Comparing `tmp/eptools-8.6.3.tar.gz` & `tmp/eptools-8.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c:\EasypostLibrary\eptools\dist\tmpw_orzyci\eptools-8.6.3.tar", last modified: Wed May 17 12:38:42 2023, max compression
+gzip compressed data, was "C:\EasypostLibrary\eptools\dist\tmpeocs2leq\eptools-8.6.4.tar", last modified: Fri Jun  2 09:01:11 2023, max compression
```

## Comparing `eptools-8.6.3.tar` & `eptools-8.6.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 12:38:42.000000 eptools-8.6.3/
-drwxrwxrwx   0        0        0        0 2023-05-17 12:38:41.000000 eptools-8.6.3/eptools/
--rw-rw-rw-   0        0        0      792 2023-04-27 15:46:33.000000 eptools-8.6.3/eptools/configuration.py
--rw-rw-rw-   0        0        0     6347 2023-05-16 11:39:59.000000 eptools-8.6.3/eptools/InvoiceDate.py
--rw-rw-rw-   0        0        0     9497 2023-05-11 09:45:44.000000 eptools-8.6.3/eptools/logger.py
--rw-rw-rw-   0        0        0     2401 2023-03-20 16:11:43.000000 eptools-8.6.3/eptools/mail_factory.py
--rw-rw-rw-   0        0        0    16595 2023-05-16 11:35:52.000000 eptools-8.6.3/eptools/SalesForceApiIntegration.py
--rw-rw-rw-   0        0        0     2305 2023-04-20 09:00:19.000000 eptools-8.6.3/eptools/sf_factory.py
--rw-rw-rw-   0        0        0    12808 2023-02-23 18:24:58.000000 eptools-8.6.3/eptools/slacker.py
--rw-rw-rw-   0        0        0    10443 2023-04-20 15:28:40.000000 eptools-8.6.3/eptools/slack_factory.py
--rw-rw-rw-   0        0        0    12446 2023-05-16 10:03:29.000000 eptools-8.6.3/eptools/SQLFactory.py
--rw-rw-rw-   0        0        0    31114 2023-05-17 12:36:14.000000 eptools-8.6.3/eptools/WindowsServiceBase.py
--rw-rw-rw-   0        0        0        0 2021-06-30 13:43:34.000000 eptools-8.6.3/eptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 12:38:41.000000 eptools-8.6.3/eptools.egg-info/
--rw-rw-rw-   0        0        0        1 2023-05-17 12:38:41.000000 eptools-8.6.3/eptools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      929 2023-05-17 12:38:41.000000 eptools-8.6.3/eptools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       92 2023-05-17 12:38:41.000000 eptools-8.6.3/eptools.egg-info/requires.txt
--rw-rw-rw-   0        0        0      469 2023-05-17 12:38:41.000000 eptools-8.6.3/eptools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-05-17 12:38:41.000000 eptools-8.6.3/eptools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1069 2021-03-05 11:50:38.000000 eptools-8.6.3/LICENSE
--rw-rw-rw-   0        0        0      929 2023-05-17 12:38:42.000000 eptools-8.6.3/PKG-INFO
--rw-rw-rw-   0        0        0      108 2021-03-05 11:44:12.000000 eptools-8.6.3/pyproject.toml
--rw-rw-rw-   0        0        0      485 2023-05-16 11:41:56.000000 eptools-8.6.3/README.md
--rw-rw-rw-   0        0        0      588 2023-05-17 12:38:42.000000 eptools-8.6.3/setup.cfg
--rw-rw-rw-   0        0        0       39 2021-03-05 11:49:21.000000 eptools-8.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 09:01:10.000000 eptools-8.6.4/
+drwxrwxrwx   0        0        0        0 2023-06-02 09:01:10.000000 eptools-8.6.4/eptools/
+-rw-rw-rw-   0        0        0      792 2023-04-27 15:46:33.000000 eptools-8.6.4/eptools/configuration.py
+-rw-rw-rw-   0        0        0     6347 2023-05-16 11:39:59.000000 eptools-8.6.4/eptools/InvoiceDate.py
+-rw-rw-rw-   0        0        0     9497 2023-05-11 09:45:44.000000 eptools-8.6.4/eptools/logger.py
+-rw-rw-rw-   0        0        0     2401 2023-03-20 16:11:43.000000 eptools-8.6.4/eptools/mail_factory.py
+-rw-rw-rw-   0        0        0    19373 2023-06-02 08:54:32.000000 eptools-8.6.4/eptools/SalesForceApiIntegration.py
+-rw-rw-rw-   0        0        0     2305 2023-04-20 09:00:19.000000 eptools-8.6.4/eptools/sf_factory.py
+-rw-rw-rw-   0        0        0    12808 2023-02-23 18:24:58.000000 eptools-8.6.4/eptools/slacker.py
+-rw-rw-rw-   0        0        0    10443 2023-04-20 15:28:40.000000 eptools-8.6.4/eptools/slack_factory.py
+-rw-rw-rw-   0        0        0    12474 2023-05-30 11:48:54.000000 eptools-8.6.4/eptools/SQLFactory.py
+-rw-rw-rw-   0        0        0    31114 2023-05-17 12:36:14.000000 eptools-8.6.4/eptools/WindowsServiceBase.py
+-rw-rw-rw-   0        0        0        0 2021-06-30 13:43:34.000000 eptools-8.6.4/eptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 09:01:10.000000 eptools-8.6.4/eptools.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-02 09:01:10.000000 eptools-8.6.4/eptools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      929 2023-06-02 09:01:10.000000 eptools-8.6.4/eptools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       92 2023-06-02 09:01:10.000000 eptools-8.6.4/eptools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      469 2023-06-02 09:01:10.000000 eptools-8.6.4/eptools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-06-02 09:01:10.000000 eptools-8.6.4/eptools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1069 2021-03-05 11:50:38.000000 eptools-8.6.4/LICENSE
+-rw-rw-rw-   0        0        0      929 2023-06-02 09:01:10.000000 eptools-8.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0      108 2021-03-05 11:44:12.000000 eptools-8.6.4/pyproject.toml
+-rw-rw-rw-   0        0        0      485 2023-05-16 11:41:56.000000 eptools-8.6.4/README.md
+-rw-rw-rw-   0        0        0      588 2023-06-02 09:01:10.000000 eptools-8.6.4/setup.cfg
+-rw-rw-rw-   0        0        0       39 2021-03-05 11:49:21.000000 eptools-8.6.4/setup.py
```

### Comparing `eptools-8.6.3/eptools/configuration.py` & `eptools-8.6.4/eptools/configuration.py`

 * *Files identical despite different names*

### Comparing `eptools-8.6.3/eptools/InvoiceDate.py` & `eptools-8.6.4/eptools/InvoiceDate.py`

 * *Files identical despite different names*

### Comparing `eptools-8.6.3/eptools/logger.py` & `eptools-8.6.4/eptools/logger.py`

 * *Files identical despite different names*

### Comparing `eptools-8.6.3/eptools/mail_factory.py` & `eptools-8.6.4/eptools/mail_factory.py`

 * *Files identical despite different names*

### Comparing `eptools-8.6.3/eptools/SalesForceApiIntegration.py` & `eptools-8.6.4/eptools/SalesForceApiIntegration.py`

 * *Files 12% similar despite different names*

```diff
@@ -379,15 +379,94 @@
             columns = [column[0] for column in sql_factory.cursor.description]
             for row in sql_factory.fetchall():
                 results.append(dict(zip(columns, row)))
         return results
     except Exception as ex:
         print(ex)
 
-if __name__ == "__main__":
+def getEmail(client_nr):
+    reset_query = """IF OBJECT_ID('tempdb..#TempContacts') IS NOT NULL
+                    BEGIN
+                        DROP TABLE #TempContacts;
+                    END
+                    SET NOCOUNT ON;"""
+    sql_query1 = """
+         DECLARE @CustomerIdPost INT = {};
+        WITH Contacts AS (
+            SELECT Email, '1' as priority, Role
+            FROM EasyPost.dbo.SFContacts
+            WHERE SFPickupLocationId = (
+                SELECT TOP 1 SFId
+                FROM EasyPost.dbo.SFPickupLocations
+                WHERE CustomerIdPost = @CustomerIdPost
+            )
+            AND (Role LIKE '%Contactpersoon Postkamer%' OR Role LIKE '%Hoofd Postkamer%')
+
+            UNION ALL
+
+            SELECT Email, '2' as priority, Role
+            FROM EasyPost.dbo.SFContacts
+            WHERE SFDepartmentId = (
+                SELECT TOP 1 SFId
+                FROM EasyPost.dbo.SFDepartments
+                WHERE CustomerIdPost = @CustomerIdPost
+            )
+            AND (Role LIKE '%Contactpersoon Postkamer%' OR Role LIKE '%Hoofd Postkamer%')
+
+            UNION ALL
+
+            
+            SELECT Email, '3' as priority, Role
+            FROM EasyPost.dbo.SFContacts
+            WHERE SFId in (
+                SELECT SFContactId
+                FROM [EasyPost].[dbo].[SFAccountContactRelations]
+                WHERE SFAccountId = ( 
+                    SELECT TOP 1 SFId
+                    FROM EasyPost.dbo.SFAccounts
+                    WHERE CustomerIdPost = @CustomerIdPost)
+            )
+            AND (Role LIKE '%Contactpersoon Postkamer%' OR Role LIKE '%Hoofd Postkamer%')
+        )
 
-    print(getHubAndRound(15555))
+        SELECT *
+        INTO #TempContacts
+        FROM Contacts
+
+        IF EXISTS (
+            SELECT *
+            FROM #TempContacts
+            WHERE Role LIKE '%Hoofd Postkamer%'
+        )
+        BEGIN
+            SELECT *
+            FROM #TempContacts
+            WHERE Role LIKE '%Hoofd Postkamer%'
+        END
+        ELSE
+        BEGIN
+            SELECT *
+            FROM #TempContacts
+            WHERE Role LIKE '%Contactpersoon Postkamer%'
+        END
+        """.format(client_nr)
+    results = []
+    with SQLFactory(SQLConnection.PRINTDB, config_path='c:\Software\Configs\eptools.json', logger = logs) as sql_factory:
+        sql_factory.execute(reset_query)
+        sql_factory.commit()
+        sql_factory.execute(sql_query1)
+        columns = [column[0] for column in sql_factory.cursor.description]
+        for row in sql_factory.fetchall():
+            results.append(dict(zip(columns, row)))
+    unique_emails = list(set(item['Email'] for item in results))
+
+    return unique_emails
+
+if __name__ == "__main__":
+    getEmail(1499)
+    getEmail(1627)
+    # print(getHubAndRound(15555))
     # print(getIdByName('BVBA Gdw Legia'))
     # print(AddressFromDB(7255))
 
     # print(getParentAccountEmail(7255))
     # print(getEmailFromDB(7255))
```

### Comparing `eptools-8.6.3/eptools/sf_factory.py` & `eptools-8.6.4/eptools/sf_factory.py`

 * *Files identical despite different names*

### Comparing `eptools-8.6.3/eptools/slacker.py` & `eptools-8.6.4/eptools/slacker.py`

 * *Files identical despite different names*

### Comparing `eptools-8.6.3/eptools/slack_factory.py` & `eptools-8.6.4/eptools/slack_factory.py`

 * *Files identical despite different names*

### Comparing `eptools-8.6.3/eptools/SQLFactory.py` & `eptools-8.6.4/eptools/SQLFactory.py`

 * *Files 1% similar despite different names*

```diff
@@ -357,16 +357,16 @@
 
     with SQLFactory(SQLConnection.PRINTDB, config_path='c:\Software\Configs\eptools.json') as conn:
         conn.execute("Select * from sysdatabases;")
         data = conn.fetchall(withColumns=True)
         print(data)
 
     # test without with
-
-    sqlf = SQLFactory(SQLConnection.PRINTDB, config_path='c:\Software\Configs\eptools.json')
+    logs = None
+    sqlf = SQLFactory(SQLConnection.PRINTDB, config_path='c:\Software\Configs\eptools.json', logger=logs)
     sqlf.createConnection()
     conn = sqlf.connection
     cursor = conn.cursor()
     cursor.execute("Select * from sysdatabases;")
     result = cursor.fetchall()
     for x in result:
         print(x)
```

### Comparing `eptools-8.6.3/eptools/WindowsServiceBase.py` & `eptools-8.6.4/eptools/WindowsServiceBase.py`

 * *Files identical despite different names*

### Comparing `eptools-8.6.3/eptools.egg-info/PKG-INFO` & `eptools-8.6.4/eptools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eptools
-Version: 8.6.3
+Version: 8.6.4
 Summary: EasyPost Tools
 Home-page: UNKNOWN
 Author: Arno De Decker
 Author-email: arno.dedecker@easypost.eu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eptools-8.6.3/LICENSE` & `eptools-8.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eptools-8.6.3/PKG-INFO` & `eptools-8.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eptools
-Version: 8.6.3
+Version: 8.6.4
 Summary: EasyPost Tools
 Home-page: UNKNOWN
 Author: Arno De Decker
 Author-email: arno.dedecker@easypost.eu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eptools-8.6.3/setup.cfg` & `eptools-8.6.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 7074 6f6f 6c73 0d0a 7665 7273   = eptools..vers
-00000020: 696f 6e20 3d20 382e 362e 330d 0a61 7574  ion = 8.6.3..aut
+00000020: 696f 6e20 3d20 382e 362e 340d 0a61 7574  ion = 8.6.4..aut
 00000030: 686f 7220 3d20 4172 6e6f 2044 6520 4465  hor = Arno De De
 00000040: 636b 6572 0d0a 6175 7468 6f72 5f65 6d61  cker..author_ema
 00000050: 696c 203d 2061 726e 6f2e 6465 6465 636b  il = arno.dedeck
 00000060: 6572 4065 6173 7970 6f73 742e 6575 0d0a  er@easypost.eu..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 4561  description = Ea
 00000080: 7379 506f 7374 2054 6f6f 6c73 0d0a 6c6f  syPost Tools..lo
 00000090: 6e67 5f64 6573 6372 6970 7469 6f6e 203d  ng_description =
```

