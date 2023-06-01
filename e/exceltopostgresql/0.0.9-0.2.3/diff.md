# Comparing `tmp/exceltopostgresql-0.0.9.tar.gz` & `tmp/exceltopostgresql-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exceltopostgresql-0.0.9.tar", last modified: Sat Dec  4 04:02:01 2021, max compression
+gzip compressed data, was "exceltopostgresql-0.2.3.tar", last modified: Thu Jun  1 21:57:38 2023, max compression
```

## Comparing `exceltopostgresql-0.0.9.tar` & `exceltopostgresql-0.2.3.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2021-12-04 04:02:01.310063 exceltopostgresql-0.0.9/
--rw-rw-rw-   0        0        0     1083 2021-12-04 02:19:58.000000 exceltopostgresql-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     2748 2021-12-04 04:02:01.309054 exceltopostgresql-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     2192 2021-12-04 03:59:56.000000 exceltopostgresql-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2021-12-04 04:02:01.282241 exceltopostgresql-0.0.9/exceltopostgresql/
--rw-rw-rw-   0        0        0      343 2021-12-04 03:14:38.000000 exceltopostgresql-0.0.9/exceltopostgresql/__init__.py
--rw-rw-rw-   0        0        0      407 2021-12-04 03:11:14.000000 exceltopostgresql-0.0.9/exceltopostgresql/_model.py
--rw-rw-rw-   0        0        0     3215 2021-12-04 04:01:13.000000 exceltopostgresql-0.0.9/exceltopostgresql/exceltopostgresql.py
-drwxrwxrwx   0        0        0        0 2021-12-04 04:02:01.306930 exceltopostgresql-0.0.9/exceltopostgresql.egg-info/
--rw-rw-rw-   0        0        0     2748 2021-12-04 04:02:01.000000 exceltopostgresql-0.0.9/exceltopostgresql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2021-12-04 04:02:01.000000 exceltopostgresql-0.0.9/exceltopostgresql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-12-04 04:02:01.000000 exceltopostgresql-0.0.9/exceltopostgresql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2021-12-04 04:02:01.000000 exceltopostgresql-0.0.9/exceltopostgresql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       94 2021-12-04 02:25:06.000000 exceltopostgresql-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2021-12-04 04:02:01.310063 exceltopostgresql-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1216 2021-12-04 04:01:38.000000 exceltopostgresql-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:57:38.274587 exceltopostgresql-0.2.3/
+-rw-rw-rw-   0        0        0     1082 2021-12-04 04:08:24.000000 exceltopostgresql-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     2743 2023-06-01 21:57:38.274587 exceltopostgresql-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2149 2023-06-01 21:56:06.000000 exceltopostgresql-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 21:57:38.240739 exceltopostgresql-0.2.3/exceltopostgresql/
+-rw-rw-rw-   0        0        0      365 2023-06-01 21:45:30.000000 exceltopostgresql-0.2.3/exceltopostgresql/__init__.py
+-rw-rw-rw-   0        0        0      407 2021-12-04 03:11:14.000000 exceltopostgresql-0.2.3/exceltopostgresql/_model.py
+-rw-rw-rw-   0        0        0     3210 2023-06-01 21:51:19.000000 exceltopostgresql-0.2.3/exceltopostgresql/exceltopostgresql.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:57:38.272287 exceltopostgresql-0.2.3/exceltopostgresql.egg-info/
+-rw-rw-rw-   0        0        0     2743 2023-06-01 21:57:37.000000 exceltopostgresql-0.2.3/exceltopostgresql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-06-01 21:57:38.000000 exceltopostgresql-0.2.3/exceltopostgresql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 21:57:37.000000 exceltopostgresql-0.2.3/exceltopostgresql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-01 21:57:37.000000 exceltopostgresql-0.2.3/exceltopostgresql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 21:57:38.274587 exceltopostgresql-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1203 2023-06-01 21:44:37.000000 exceltopostgresql-0.2.3/setup.py
```

### Comparing `exceltopostgresql-0.0.9/LICENSE` & `exceltopostgresql-0.2.3/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 MIT License
 
 Copyright (c) 2021 xyluo
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
@@ -15,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `exceltopostgresql-0.0.9/PKG-INFO` & `exceltopostgresql-0.2.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,98 +1,96 @@
 Metadata-Version: 2.1
 Name: exceltopostgresql
-Version: 0.0.9
-Summary: This package help to convert your excel files (xlsx,xls,csv) to Postgresql database.
+Version: 0.2.3
+Summary: This package help convert your excel files (xlsx,xls,csv) to Postgresql Database.
 Home-page: https://github.com/Xiangyongluo/exceltopostgresql
 Author: Xiangyong Luo
 Author-email: rochemay@163.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# exceltopostgresql
+
+A model to automatically save your local excel file (xlsx,xls,csv) onto your postgresql database
+
 # Introduction
 
 This package help to convert your excel files (xlsx,xls,csv) to postgresql database.
 
 # Installation
 
 exceltopostgresql can be installed as:
 
-```python
+```
 pip install exceltopostgresql
 ```
 
 # Dependency
 
-👍   [pandas](https://pandas.pydata.org/)
+👍 [pandas](https://pandas.pydata.org/)
 
-👍   [psycopg2](https://pypi.org/project/psycopg2/)
+👍 [psycopg2](https://pypi.org/project/psycopg2/)
 
-👍   [sqlalchemy](https://www.sqlalchemy.org/)
+👍 [sqlalchemy](https://www.sqlalchemy.org/)
 
 # QuickStart
 
-```python
+```
 import exceltosqlserver as ep
 # generate the class instance
 
 # STEP One, prepare your input pareameters
 
 yourFile  = "test01.xls"  # available for xlsx, xls,csv
-yourUsrID = ""  
+yourUsrID = ""
 yourPWD   = ""
 yourDBname= ""
-save2tableName = False  
-	# False: save your file name as table name onto posgtresql 
-	# or 
+rename_table = ""
+	# "": save your file name as table name onto posgtresql
+	# or
 	# customize your table, like: "test"
 
 # get your local host name
 # this will return your local computer name for your sql server database
-host_name = ep.hostname   
-or 
+host_name = ep.hostname
+or
 host_name = "localhost"
 
-# get your local ip address 
+# get your local ip address
 # this will return your local ip address (if your sql server can be accessed by DNS)
-ip = ep.local_ip  
+ip = ep.local_ip
 
 # you need to change your host if needed, dns: local ip address
-#yourHostORip  = "localhost"   
+#yourHostORip  = "localhost"
 # yourHostORip  = host_name
 yourHostORip  = ip
 
 
 # STEP Two  convert your data to sql server
 ep.exceltoDBtable(yourFile,yourHostORip,yourUsrID,yourPWD,yourDBname,save2tableName)
-
-
 ```
 
-```python
+```
 output:
 Successfully load excel data...
 Secessfully connected to SQL Server...
-Secessfully saved 'yourtable' onto Posggresql...
+Secessfully saved 'yourtable' to Posggresql...
 ```
 
 # API Reference
 
-exceltopostgresql.exceltoDBtable(`filePath,host_ip=False,usrID =False,pwd=False,database_name=False,port:str= "5432",save2tableName=False`)
+exceltopostgresql.exceltoDBtable(`filePath, host_ip="", usrID ="", pwd="", database_name="", port= "5432", rename_table=""`)
 
 ```
 Args:
             filePath (str): [path of your input file name]
-            host_ip (bool, optional): [description]. Defaults to False.
-            usrID (bool, optional): [description]. Defaults to False.
-            pwd (bool, optional): [description]. Defaults to False.
-            database_name (bool, optional): [description]. Defaults to False.
+            host_ip (bool, optional): [description]. Defaults to "".
+            usrID (bool, optional): [description]. Defaults to "".
+            pwd (bool, optional): [description]. Defaults to "".
+            database_name (bool, optional): [description]. Defaults to "".
             port (str, optional): [description]. Defaults to "5432".
-            save2tableName (bool, optional): [description]. Defaults to False.
+            save2tableName (bool, optional): [description]. Defaults to "".
 ```
-
-
```

### Comparing `exceltopostgresql-0.0.9/exceltopostgresql/exceltopostgresql.py` & `exceltopostgresql-0.2.3/exceltopostgresql/exceltopostgresql.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,81 +2,87 @@
 ##############################################################
 # Created Date: Friday, December 3rd 2021
 # Contact Info: luoxiangyong01@gmail.com
 # Author/Copyright: Mr. Xiangyong Luo
 ##############################################################
 
 
-import sqlalchemy
-import psycopg2
-import pandas as pd
 import socket
 
+import pandas as pd
+import psycopg2
+import sqlalchemy
+
 hostname = socket.gethostname()
 local_ip = socket.gethostbyname(hostname)
 
 
 class exceltoDBtable:
-    """This is a model to automatically save your local excel file (xlsx,xls,csv) onto your postgresql database
+    """This is a model to automatically save your local excel file (xlsx,xls,csv) to your Postgresql Database
         define inputs variables
 
         Args:
             filePath (str): [path of your input file name]
-            host_ip (bool, optional): [description]. Defaults to False.
-            usrID (bool, optional): [description]. Defaults to False.
-            pwd (bool, optional): [description]. Defaults to False.
-            database_name (bool, optional): [description]. Defaults to False.
+            host_ip (bool, optional): [description]. Defaults to "".
+            usrID (bool, optional): [description]. Defaults to "".
+            pwd (bool, optional): [description]. Defaults to "".
+            database_name (bool, optional): [description]. Defaults to "".
             port (str, optional): [description]. Defaults to "5432".
-            save2tableName (bool, optional): [description]. Defaults to False.
+            save2tableName (bool, optional): [description]. Defaults to "".
 
         Raises:
             Exception: [if the inputs in not correct then raise exceptions]
         """
-    
-    def __init__(self,filePath,host_ip=False,usrID =False,pwd=False,database_name=False,port:str= "5432",save2tableName=False):
-        
-        if not any([host_ip,database_name,usrID,pwd]):
+
+    def __init__(self,
+                 filePath: str,
+                 host_ip: str = "",
+                 usrID: str = "",
+                 pwd: str = "",
+                 database_name: str = "",
+                 port: str = "5432",
+                 rename_table: str = ""):
+
+        if not any([host_ip, database_name, usrID, pwd]):
             raise Exception("Partially inputs, please check your inputs...")
-        else:
-            self.filePath = filePath
-            self.host_ip = host_ip
-            self.database_name=database_name
-            self.usrID = usrID
-            self.pwd = pwd
-            self.port = port
-            self.save2tableName = save2tableName
-            
+
+        self.filePath = filePath
+        self.host_ip = host_ip
+        self.database_name = database_name
+        self.usrID = usrID
+        self.pwd = pwd
+        self.port = port
+        self.rename_table = rename_table
+
         self.postgresql_cur()
         self.readData()
         self.save2database()
-        
-        
+
     def postgresql_cur(self):
         db_url = f"postgresql+psycopg2://{self.usrID}:{self.pwd}@{self.host_ip}:{self.port}/{self.database_name}"
         self.engine = sqlalchemy.create_engine(db_url)
 
-    def readData(self) -> "DataFrame":
-        if self.filePath.split(".")[-1] in ["xlsx","xls"]:
+    def readData(self) -> None:
+        if self.filePath.split(".")[-1] in ["xlsx", "xls"]:
             self.file_data = pd.read_excel(self.filePath)
             print("Successfully load excel data...")
         elif self.filePath.split(".")[-1] in ["csv"]:
             self.file_data = pd.read_csv(self.filePath)
             print("Successfully load csv data...")
         else:
             raise Exception("Unable to load input file...")
-    
-    def save2database(self) ->"DataFrame to database":
-        # specificy the table name
-        if self.save2tableName:
-            tableName = self.save2tableName
+
+    def save2database(self) -> None:
+        # specify the table name
+        if self.rename_table:
+            tableName = self.rename_table
+        elif "/" in self.filePath:
+            tableName = self.filePath.split("/")[-1].split(".")[0]
         else:
-            if "/" in self.filePath:
-                tableName = self.filePath.split("/")[-1].split(".")[0]
-            else:
-                tableName = self.filePath.split(".")[0]
-                
+            tableName = self.filePath.split(".")[0]
+
         # using pandas to save table to database
         try:
-            self.file_data.to_sql(tableName,con=self.engine)
-            print("Successfully save %s into database..."%tableName)
+            self.file_data.to_sql(tableName, con=self.engine)
+            print("Successfully save %s into Postgresql Database..." % tableName)
         except Exception as e:
             raise Exception(e)
```

### Comparing `exceltopostgresql-0.0.9/exceltopostgresql.egg-info/PKG-INFO` & `exceltopostgresql-0.2.3/exceltopostgresql.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,98 +1,96 @@
 Metadata-Version: 2.1
 Name: exceltopostgresql
-Version: 0.0.9
-Summary: This package help to convert your excel files (xlsx,xls,csv) to Postgresql database.
+Version: 0.2.3
+Summary: This package help convert your excel files (xlsx,xls,csv) to Postgresql Database.
 Home-page: https://github.com/Xiangyongluo/exceltopostgresql
 Author: Xiangyong Luo
 Author-email: rochemay@163.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# exceltopostgresql
+
+A model to automatically save your local excel file (xlsx,xls,csv) onto your postgresql database
+
 # Introduction
 
 This package help to convert your excel files (xlsx,xls,csv) to postgresql database.
 
 # Installation
 
 exceltopostgresql can be installed as:
 
-```python
+```
 pip install exceltopostgresql
 ```
 
 # Dependency
 
-👍   [pandas](https://pandas.pydata.org/)
+👍 [pandas](https://pandas.pydata.org/)
 
-👍   [psycopg2](https://pypi.org/project/psycopg2/)
+👍 [psycopg2](https://pypi.org/project/psycopg2/)
 
-👍   [sqlalchemy](https://www.sqlalchemy.org/)
+👍 [sqlalchemy](https://www.sqlalchemy.org/)
 
 # QuickStart
 
-```python
+```
 import exceltosqlserver as ep
 # generate the class instance
 
 # STEP One, prepare your input pareameters
 
 yourFile  = "test01.xls"  # available for xlsx, xls,csv
-yourUsrID = ""  
+yourUsrID = ""
 yourPWD   = ""
 yourDBname= ""
-save2tableName = False  
-	# False: save your file name as table name onto posgtresql 
-	# or 
+rename_table = ""
+	# "": save your file name as table name onto posgtresql
+	# or
 	# customize your table, like: "test"
 
 # get your local host name
 # this will return your local computer name for your sql server database
-host_name = ep.hostname   
-or 
+host_name = ep.hostname
+or
 host_name = "localhost"
 
-# get your local ip address 
+# get your local ip address
 # this will return your local ip address (if your sql server can be accessed by DNS)
-ip = ep.local_ip  
+ip = ep.local_ip
 
 # you need to change your host if needed, dns: local ip address
-#yourHostORip  = "localhost"   
+#yourHostORip  = "localhost"
 # yourHostORip  = host_name
 yourHostORip  = ip
 
 
 # STEP Two  convert your data to sql server
 ep.exceltoDBtable(yourFile,yourHostORip,yourUsrID,yourPWD,yourDBname,save2tableName)
-
-
 ```
 
-```python
+```
 output:
 Successfully load excel data...
 Secessfully connected to SQL Server...
-Secessfully saved 'yourtable' onto Posggresql...
+Secessfully saved 'yourtable' to Posggresql...
 ```
 
 # API Reference
 
-exceltopostgresql.exceltoDBtable(`filePath,host_ip=False,usrID =False,pwd=False,database_name=False,port:str= "5432",save2tableName=False`)
+exceltopostgresql.exceltoDBtable(`filePath, host_ip="", usrID ="", pwd="", database_name="", port= "5432", rename_table=""`)
 
 ```
 Args:
             filePath (str): [path of your input file name]
-            host_ip (bool, optional): [description]. Defaults to False.
-            usrID (bool, optional): [description]. Defaults to False.
-            pwd (bool, optional): [description]. Defaults to False.
-            database_name (bool, optional): [description]. Defaults to False.
+            host_ip (bool, optional): [description]. Defaults to "".
+            usrID (bool, optional): [description]. Defaults to "".
+            pwd (bool, optional): [description]. Defaults to "".
+            database_name (bool, optional): [description]. Defaults to "".
             port (str, optional): [description]. Defaults to "5432".
-            save2tableName (bool, optional): [description]. Defaults to False.
+            save2tableName (bool, optional): [description]. Defaults to "".
 ```
-
-
```

### Comparing `exceltopostgresql-0.0.9/setup.py` & `exceltopostgresql-0.2.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
-    
+
 try:
     # if have requirements.txt file inside the folder
     with open("requirements.txt", "r", encoding="utf-8") as f:
-        modules_needed = [i.strip() for i in fh.readlines()]   
-except:
+        modules_needed = [i.strip() for i in fh.readlines()]
+except Exception:
     modules_needed = []
 
 setuptools.setup(
     name="exceltopostgresql", # Replace with your own username
-    version="0.0.9",
+    version="0.2.3",
     author="Xiangyong Luo",
     author_email="rochemay@163.com",
-    description="This package help to convert your excel files (xlsx,xls,csv) to Postgresql database.",
+    description="This package help convert your excel files (xlsx,xls,csv) to Postgresql Database.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Xiangyongluo/exceltopostgresql",
-    
-    
+
+
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
-    
+
     install_requires=modules_needed,
     packages=setuptools.find_packages(),
     include_package_data=True,
 
-    package_data= {'':['*.txt','*.xls','*.xlsx','*.csv'],
-                   "test_data":['*.txt']}
+    package_data={'': ['*.txt', '*.xls', '*.xlsx', '*.csv'],
+                  "test_data": ['*.txt']}
 )
-
-
```

