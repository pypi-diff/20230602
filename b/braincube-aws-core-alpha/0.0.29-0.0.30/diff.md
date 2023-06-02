# Comparing `tmp/braincube-aws-core-alpha-0.0.29.tar.gz` & `tmp/braincube-aws-core-alpha-0.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "braincube-aws-core-alpha-0.0.29.tar", last modified: Wed May 31 12:26:54 2023, max compression
+gzip compressed data, was "braincube-aws-core-alpha-0.0.30.tar", last modified: Fri Jun  2 06:36:15 2023, max compression
```

## Comparing `braincube-aws-core-alpha-0.0.29.tar` & `braincube-aws-core-alpha-0.0.30.tar`

### file list

```diff
@@ -1,35 +1,40 @@
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-31 12:26:54.287366 braincube-aws-core-alpha-0.0.29/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.29/LICENSE
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8896 2023-05-31 12:26:54.287642 braincube-aws-core-alpha-0.0.29/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8143 2023-05-23 10:50:40.000000 braincube-aws-core-alpha-0.0.29/README.md
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.29/pyproject.toml
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      933 2023-05-31 12:26:54.290181 braincube-aws-core-alpha-0.0.29/setup.cfg
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.29/setup.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-31 12:26:54.271682 braincube-aws-core-alpha-0.0.29/src/
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-31 12:26:54.276520 braincube-aws-core-alpha-0.0.29/src/braincube_aws_core_alpha.egg-info/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8896 2023-05-31 12:26:54.000000 braincube-aws-core-alpha-0.0.29/src/braincube_aws_core_alpha.egg-info/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      733 2023-05-31 12:26:54.000000 braincube-aws-core-alpha-0.0.29/src/braincube_aws_core_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-31 12:26:54.000000 braincube-aws-core-alpha-0.0.29/src/braincube_aws_core_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       48 2023-05-31 12:26:54.000000 braincube-aws-core-alpha-0.0.29/src/braincube_aws_core_alpha.egg-info/requires.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-31 12:26:54.000000 braincube-aws-core-alpha-0.0.29/src/braincube_aws_core_alpha.egg-info/top_level.txt
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-31 12:26:54.276889 braincube-aws-core-alpha-0.0.29/src/core/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.29/src/core/__init__.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-31 12:26:54.279478 braincube-aws-core-alpha-0.0.29/src/core/dal/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.29/src/core/dal/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1990 2023-05-15 18:52:22.000000 braincube-aws-core-alpha-0.0.29/src/core/dal/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      241 2023-05-11 10:53:14.000000 braincube-aws-core-alpha-0.0.29/src/core/dal/database_errors.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     4110 2023-05-23 08:56:40.000000 braincube-aws-core-alpha-0.0.29/src/core/dal/postgres_connection.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)    33020 2023-05-31 12:25:52.000000 braincube-aws-core-alpha-0.0.29/src/core/dal/postgres_repository.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-31 12:26:54.281857 braincube-aws-core-alpha-0.0.29/src/core/di/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.29/src/core/di/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      561 2023-05-11 10:50:19.000000 braincube-aws-core-alpha-0.0.29/src/core/di/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     4122 2023-05-11 10:51:25.000000 braincube-aws-core-alpha-0.0.29/src/core/di/injector.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-31 12:26:54.284627 braincube-aws-core-alpha-0.0.29/src/core/rest/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.29/src/core/rest/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     2793 2023-05-11 10:52:14.000000 braincube-aws-core-alpha-0.0.29/src/core/rest/app_controller.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3722 2023-05-11 10:52:31.000000 braincube-aws-core-alpha-0.0.29/src/core/rest/app_module.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3598 2023-05-11 17:50:46.000000 braincube-aws-core-alpha-0.0.29/src/core/rest/data.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-31 12:26:54.286753 braincube-aws-core-alpha-0.0.29/src/core/utils/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.29/src/core/utils/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      738 2023-05-15 14:42:55.000000 braincube-aws-core-alpha-0.0.29/src/core/utils/convert.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1377 2023-05-11 10:53:41.000000 braincube-aws-core-alpha-0.0.29/src/core/utils/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-02 06:36:15.654819 braincube-aws-core-alpha-0.0.30/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.30/LICENSE
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8820 2023-06-02 06:36:15.655113 braincube-aws-core-alpha-0.0.30/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8067 2023-06-01 08:04:11.000000 braincube-aws-core-alpha-0.0.30/README.md
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.30/pyproject.toml
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      953 2023-06-02 06:36:15.656479 braincube-aws-core-alpha-0.0.30/setup.cfg
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.30/setup.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-02 06:36:15.631394 braincube-aws-core-alpha-0.0.30/src/
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-02 06:36:15.638180 braincube-aws-core-alpha-0.0.30/src/braincube_aws_core_alpha.egg-info/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8820 2023-06-02 06:36:15.000000 braincube-aws-core-alpha-0.0.30/src/braincube_aws_core_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      871 2023-06-02 06:36:15.000000 braincube-aws-core-alpha-0.0.30/src/braincube_aws_core_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-06-02 06:36:15.000000 braincube-aws-core-alpha-0.0.30/src/braincube_aws_core_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       67 2023-06-02 06:36:15.000000 braincube-aws-core-alpha-0.0.30/src/braincube_aws_core_alpha.egg-info/requires.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-06-02 06:36:15.000000 braincube-aws-core-alpha-0.0.30/src/braincube_aws_core_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-02 06:36:15.638689 braincube-aws-core-alpha-0.0.30/src/core/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.30/src/core/__init__.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-02 06:36:15.641773 braincube-aws-core-alpha-0.0.30/src/core/dal/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.30/src/core/dal/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1990 2023-05-15 18:52:22.000000 braincube-aws-core-alpha-0.0.30/src/core/dal/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      241 2023-05-11 10:53:14.000000 braincube-aws-core-alpha-0.0.30/src/core/dal/database_errors.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     4110 2023-05-23 08:56:40.000000 braincube-aws-core-alpha-0.0.30/src/core/dal/postgres_connection.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)    33020 2023-05-31 12:25:52.000000 braincube-aws-core-alpha-0.0.30/src/core/dal/postgres_repository.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-02 06:36:15.644462 braincube-aws-core-alpha-0.0.30/src/core/di/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.30/src/core/di/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      561 2023-05-11 10:50:19.000000 braincube-aws-core-alpha-0.0.30/src/core/di/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     4122 2023-05-11 10:51:25.000000 braincube-aws-core-alpha-0.0.30/src/core/di/injector.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-02 06:36:15.647762 braincube-aws-core-alpha-0.0.30/src/core/rest/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.30/src/core/rest/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     2793 2023-05-11 10:52:14.000000 braincube-aws-core-alpha-0.0.30/src/core/rest/app_controller.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3722 2023-05-11 10:52:31.000000 braincube-aws-core-alpha-0.0.30/src/core/rest/app_module.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3598 2023-05-11 17:50:46.000000 braincube-aws-core-alpha-0.0.30/src/core/rest/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-02 06:36:15.651546 braincube-aws-core-alpha-0.0.30/src/core/rules_engine/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.30/src/core/rules_engine/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1017 2023-06-01 06:45:52.000000 braincube-aws-core-alpha-0.0.30/src/core/rules_engine/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      132 2023-06-01 06:45:21.000000 braincube-aws-core-alpha-0.0.30/src/core/rules_engine/exceptions.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     2752 2023-06-01 07:59:06.000000 braincube-aws-core-alpha-0.0.30/src/core/rules_engine/rule_manager.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-02 06:36:15.654096 braincube-aws-core-alpha-0.0.30/src/core/utils/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.30/src/core/utils/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      738 2023-05-15 14:42:55.000000 braincube-aws-core-alpha-0.0.30/src/core/utils/convert.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1377 2023-05-11 10:53:41.000000 braincube-aws-core-alpha-0.0.30/src/core/utils/data.py
```

### Comparing `braincube-aws-core-alpha-0.0.29/LICENSE` & `braincube-aws-core-alpha-0.0.30/LICENSE`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.29/PKG-INFO` & `braincube-aws-core-alpha-0.0.30/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core-alpha
-Version: 0.0.29
+Version: 0.0.30
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
@@ -117,40 +117,40 @@
 
 # schema definition
 equities = Schema(
     table="equities",
     alias="e",
     primary_key=["id"],
     columns=[
-        Column(name="id", updatable=False, insertable=False),
-        Column(name="name"),
-        Column(name="type"),
-        Column(name="issuer_id", alias="issuerId"),
-        Column(name="industry_sector", alias="industrySector"),
-        Column(name="isin"),
-        Column(name="reference"),
-        Column(name="bloomberg_code", alias="bloombergCode"),
-        Column(name="market_symbol", alias="marketSymbol"),
-        Column(name="currency"),
-        Column(name="country", ),
-        Column(name="min_amount", alias="minAmount"),
+        Column("id", updatable=False, insertable=False),
+        Column("name"),
+        Column("type"),
+        Column("issuer_id", alias="issuerId"),
+        Column("industry_sector", alias="industrySector"),
+        Column("isin"),
+        Column("reference"),
+        Column("bloomberg_code", alias="bloombergCode"),
+        Column("market_symbol", alias="marketSymbol"),
+        Column("currency"),
+        Column("country", ),
+        Column("min_amount", alias="minAmount"),
     ],
     statement_fields=[
-        StatementField(alias="isTypeOne", statement="CASE WHEN e.type = 1 then True else False END")
+        StatementField("isTypeOne", statement="CASE WHEN e.type = 1 then True else False END")
     ],
     order=[
         Order(type=OrderType.asc, alias="name")
     ],
     relations=[
         Relation(
             table="parties",
             alias="p",
             columns=[
-                SimpleColumn(name="name"),
-                SimpleColumn(name="short_name", alias="shortName"),
+                SimpleColumn("name"),
+                SimpleColumn("short_name", alias="shortName"),
             ],
             join_forced=False,
             join_type=JoinType.left,
             join_through=JoinThrough(from_column_name="issuer_id", to_column_name="id")
         )
     ]
 )
```

### Comparing `braincube-aws-core-alpha-0.0.29/README.md` & `braincube-aws-core-alpha-0.0.30/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -97,40 +97,40 @@
 
 # schema definition
 equities = Schema(
     table="equities",
     alias="e",
     primary_key=["id"],
     columns=[
-        Column(name="id", updatable=False, insertable=False),
-        Column(name="name"),
-        Column(name="type"),
-        Column(name="issuer_id", alias="issuerId"),
-        Column(name="industry_sector", alias="industrySector"),
-        Column(name="isin"),
-        Column(name="reference"),
-        Column(name="bloomberg_code", alias="bloombergCode"),
-        Column(name="market_symbol", alias="marketSymbol"),
-        Column(name="currency"),
-        Column(name="country", ),
-        Column(name="min_amount", alias="minAmount"),
+        Column("id", updatable=False, insertable=False),
+        Column("name"),
+        Column("type"),
+        Column("issuer_id", alias="issuerId"),
+        Column("industry_sector", alias="industrySector"),
+        Column("isin"),
+        Column("reference"),
+        Column("bloomberg_code", alias="bloombergCode"),
+        Column("market_symbol", alias="marketSymbol"),
+        Column("currency"),
+        Column("country", ),
+        Column("min_amount", alias="minAmount"),
     ],
     statement_fields=[
-        StatementField(alias="isTypeOne", statement="CASE WHEN e.type = 1 then True else False END")
+        StatementField("isTypeOne", statement="CASE WHEN e.type = 1 then True else False END")
     ],
     order=[
         Order(type=OrderType.asc, alias="name")
     ],
     relations=[
         Relation(
             table="parties",
             alias="p",
             columns=[
-                SimpleColumn(name="name"),
-                SimpleColumn(name="short_name", alias="shortName"),
+                SimpleColumn("name"),
+                SimpleColumn("short_name", alias="shortName"),
             ],
             join_forced=False,
             join_type=JoinType.left,
             join_through=JoinThrough(from_column_name="issuer_id", to_column_name="id")
         )
     ]
 )
```

### Comparing `braincube-aws-core-alpha-0.0.29/setup.cfg` & `braincube-aws-core-alpha-0.0.30/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = braincube-aws-core-alpha
-version = 0.0.29
+version = 0.0.30
 author = Braincube
 author_email = v.boudis@braincube.gr
 description = Microframework for python aws lambdas
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://bitbucket.org/braincube-common/core-aws.git
 license = MIT
@@ -24,14 +24,15 @@
 	= src
 packages = find:
 python_requires = >=3.10, <4
 install_requires = 
 	asyncpg==0.27.0
 	pypika==0.48.9
 	pydantic==1.10.7
+	rule-engine==3.5.1
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `braincube-aws-core-alpha-0.0.29/src/braincube_aws_core_alpha.egg-info/PKG-INFO` & `braincube-aws-core-alpha-0.0.30/src/braincube_aws_core_alpha.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core-alpha
-Version: 0.0.29
+Version: 0.0.30
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
@@ -117,40 +117,40 @@
 
 # schema definition
 equities = Schema(
     table="equities",
     alias="e",
     primary_key=["id"],
     columns=[
-        Column(name="id", updatable=False, insertable=False),
-        Column(name="name"),
-        Column(name="type"),
-        Column(name="issuer_id", alias="issuerId"),
-        Column(name="industry_sector", alias="industrySector"),
-        Column(name="isin"),
-        Column(name="reference"),
-        Column(name="bloomberg_code", alias="bloombergCode"),
-        Column(name="market_symbol", alias="marketSymbol"),
-        Column(name="currency"),
-        Column(name="country", ),
-        Column(name="min_amount", alias="minAmount"),
+        Column("id", updatable=False, insertable=False),
+        Column("name"),
+        Column("type"),
+        Column("issuer_id", alias="issuerId"),
+        Column("industry_sector", alias="industrySector"),
+        Column("isin"),
+        Column("reference"),
+        Column("bloomberg_code", alias="bloombergCode"),
+        Column("market_symbol", alias="marketSymbol"),
+        Column("currency"),
+        Column("country", ),
+        Column("min_amount", alias="minAmount"),
     ],
     statement_fields=[
-        StatementField(alias="isTypeOne", statement="CASE WHEN e.type = 1 then True else False END")
+        StatementField("isTypeOne", statement="CASE WHEN e.type = 1 then True else False END")
     ],
     order=[
         Order(type=OrderType.asc, alias="name")
     ],
     relations=[
         Relation(
             table="parties",
             alias="p",
             columns=[
-                SimpleColumn(name="name"),
-                SimpleColumn(name="short_name", alias="shortName"),
+                SimpleColumn("name"),
+                SimpleColumn("short_name", alias="shortName"),
             ],
             join_forced=False,
             join_type=JoinType.left,
             join_through=JoinThrough(from_column_name="issuer_id", to_column_name="id")
         )
     ]
 )
```

### Comparing `braincube-aws-core-alpha-0.0.29/src/braincube_aws_core_alpha.egg-info/SOURCES.txt` & `braincube-aws-core-alpha-0.0.30/src/braincube_aws_core_alpha.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -17,10 +17,14 @@
 src/core/di/__init__.py
 src/core/di/data.py
 src/core/di/injector.py
 src/core/rest/__init__.py
 src/core/rest/app_controller.py
 src/core/rest/app_module.py
 src/core/rest/data.py
+src/core/rules_engine/__init__.py
+src/core/rules_engine/data.py
+src/core/rules_engine/exceptions.py
+src/core/rules_engine/rule_manager.py
 src/core/utils/__init__.py
 src/core/utils/convert.py
 src/core/utils/data.py
```

### Comparing `braincube-aws-core-alpha-0.0.29/src/core/dal/data.py` & `braincube-aws-core-alpha-0.0.30/src/core/dal/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.29/src/core/dal/postgres_connection.py` & `braincube-aws-core-alpha-0.0.30/src/core/dal/postgres_connection.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.29/src/core/dal/postgres_repository.py` & `braincube-aws-core-alpha-0.0.30/src/core/dal/postgres_repository.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.29/src/core/di/data.py` & `braincube-aws-core-alpha-0.0.30/src/core/di/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.29/src/core/di/injector.py` & `braincube-aws-core-alpha-0.0.30/src/core/di/injector.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.29/src/core/rest/app_controller.py` & `braincube-aws-core-alpha-0.0.30/src/core/rest/app_controller.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.29/src/core/rest/app_module.py` & `braincube-aws-core-alpha-0.0.30/src/core/rest/app_module.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.29/src/core/rest/data.py` & `braincube-aws-core-alpha-0.0.30/src/core/rest/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.29/src/core/utils/convert.py` & `braincube-aws-core-alpha-0.0.30/src/core/utils/convert.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.29/src/core/utils/data.py` & `braincube-aws-core-alpha-0.0.30/src/core/utils/data.py`

 * *Files identical despite different names*

