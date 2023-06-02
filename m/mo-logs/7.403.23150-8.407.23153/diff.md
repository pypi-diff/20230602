# Comparing `tmp/mo_logs-7.403.23150-py2.py3-none-any.whl.zip` & `tmp/mo_logs-8.407.23153-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 42897 bytes, number of entries: 21
--rw-rw-rw-  2.0 fat    14729 b- defN 23-May-30 00:22 mo_logs/__init__.py
+Zip file size: 42724 bytes, number of entries: 21
+-rw-rw-rw-  2.0 fat    14801 b- defN 23-Jun-02 01:32 mo_logs/__init__.py
 -rw-rw-rw-  2.0 fat     2329 b- defN 23-Apr-30 18:00 mo_logs/constants.py
 -rw-rw-rw-  2.0 fat     2407 b- defN 23-May-30 00:22 mo_logs/convert.py
 -rw-rw-rw-  2.0 fat     8766 b- defN 23-May-30 00:22 mo_logs/exceptions.py
 -rw-rw-rw-  2.0 fat     3524 b- defN 23-Apr-30 18:00 mo_logs/log_usingEmail.py
 -rw-rw-rw-  2.0 fat     1099 b- defN 23-Apr-30 18:00 mo_logs/log_usingFile.py
 -rw-rw-rw-  2.0 fat     3301 b- defN 23-May-09 22:44 mo_logs/log_usingHandler.py
 -rw-rw-rw-  2.0 fat     2013 b- defN 23-Apr-30 18:00 mo_logs/log_usingLogger.py
@@ -11,13 +11,13 @@
 -rw-rw-rw-  2.0 fat     1454 b- defN 23-Apr-30 18:00 mo_logs/log_usingMulti.py
 -rw-rw-rw-  2.0 fat      450 b- defN 23-Apr-30 18:00 mo_logs/log_usingNothing.py
 -rw-rw-rw-  2.0 fat     4069 b- defN 23-Apr-30 18:00 mo_logs/log_usingSES.py
 -rw-rw-rw-  2.0 fat     1525 b- defN 23-May-30 00:22 mo_logs/log_usingStream.py
 -rw-rw-rw-  2.0 fat     2325 b- defN 23-Apr-30 18:00 mo_logs/log_usingThread.py
 -rw-rw-rw-  2.0 fat     6310 b- defN 23-May-30 00:22 mo_logs/startup.py
 -rw-rw-rw-  2.0 fat    24689 b- defN 23-May-30 00:22 mo_logs/strings.py
--rw-rw-rw-  2.0 fat    16725 b- defN 23-May-30 00:22 mo_logs-7.403.23150.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    18254 b- defN 23-May-30 00:22 mo_logs-7.403.23150.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-May-30 00:22 mo_logs-7.403.23150.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-30 00:22 mo_logs-7.403.23150.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1700 b- defN 23-May-30 00:22 mo_logs-7.403.23150.dist-info/RECORD
-21 files, 118376 bytes uncompressed, 40163 bytes compressed:  66.1%
+-rw-rw-rw-  2.0 fat    16725 b- defN 23-Jun-02 01:32 mo_logs-8.407.23153.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    17648 b- defN 23-Jun-02 01:32 mo_logs-8.407.23153.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-02 01:32 mo_logs-8.407.23153.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-02 01:32 mo_logs-8.407.23153.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1700 b- defN 23-Jun-02 01:32 mo_logs-8.407.23153.dist-info/RECORD
+21 files, 117842 bytes uncompressed, 39990 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -42,23 +42,23 @@
 
 Filename: mo_logs/startup.py
 Comment: 
 
 Filename: mo_logs/strings.py
 Comment: 
 
-Filename: mo_logs-7.403.23150.dist-info/LICENSE
+Filename: mo_logs-8.407.23153.dist-info/LICENSE
 Comment: 
 
-Filename: mo_logs-7.403.23150.dist-info/METADATA
+Filename: mo_logs-8.407.23153.dist-info/METADATA
 Comment: 
 
-Filename: mo_logs-7.403.23150.dist-info/WHEEL
+Filename: mo_logs-8.407.23153.dist-info/WHEEL
 Comment: 
 
-Filename: mo_logs-7.403.23150.dist-info/top_level.txt
+Filename: mo_logs-8.407.23153.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_logs-7.403.23150.dist-info/RECORD
+Filename: mo_logs-8.407.23153.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mo_logs/__init__.py

```diff
@@ -58,16 +58,17 @@
         https://fangpenlin.com/posts/2012/08/26/good-logging-practice-in-python/
 
         :param trace: SHOW MORE DETAILS IN EVERY LOG LINE (default False)
         :param cprofile: True==ENABLE THE C-PROFILER THAT COMES WITH PYTHON (default False)
                          USE THE LONG FORM TO SET THE FILENAME {"enabled": True, "filename": "cprofile.tab"}
         :param constants: UPDATE MODULE CONSTANTS AT STARTUP (PRIMARILY INTENDED TO CHANGE DEBUG STATE)
         :param logs: LIST OF PARAMETERS FOR LOGGER(S)
+        :param extra: ADDITIONAL DATA TO BE INCLUDED IN EVERY LOG LINE
         :param app_name: GIVE THIS APP A NAME, AND RETURN A CONTEXT MANAGER
-        :param settings: ALL THE ABOVE PARAMTERS
+        :param settings: ALL THE ABOVE PARAMETERS
         :return:
         """
         if app_name:
             return LoggingContext(app_name)
 
         Log.stop()
```

## Comparing `mo_logs-7.403.23150.dist-info/LICENSE` & `mo_logs-8.407.23153.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mo_logs-7.403.23150.dist-info/METADATA` & `mo_logs-8.407.23153.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-logs
-Version: 7.403.23150
+Version: 8.407.23153
 Summary: More Logs! Structured Logging and Exception Handling
 Home-page: https://github.com/klahnakoski/mo-logs
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
@@ -487,28 +487,18 @@
         }
     ]
 }}
 ```
 
 ## Capturing logs
 
-You can recieve a copy of all logs and send them to your own logging with 
+You can receive a copy of all logs and send them to your own logging with 
 
     logger.set_logger(myLogger)
     
 where `myLogger` is an instance that can accept a calls to `write(template, parameters)`. If your logging library can only handle strings, then use `message = expand_template(template, params)`.
 
 
-## Problems with Python 2.x Logging
-
-[Python's default `logging` module](https://docs.python.org/2/library/logging.html#logging.debug)
-comes close to doing the right thing, but fails:  
-
-  * It has keyword parameters, but they are expanded at call time so the values are lost in a string.  
-  * It has `extra` parameters, but they are lost if not used by the matching `Formatter`.  
-  * It even has stack trace with `exc_info` parameter, but only if an exception is being handled.
-  * Python 2.x has no builtin exception chaining, but [Python 3 does](https://www.python.org/dev/peps/pep-3134/)
-
-### More Reading
+## More Reading
 
 * **Structured Logging is Good** - https://sites.google.com/site/steveyegge2/the-emacs-problem
```

## Comparing `mo_logs-7.403.23150.dist-info/RECORD` & `mo_logs-8.407.23153.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-mo_logs/__init__.py,sha256=p2Uj4KNdl8Uh-T3H2zv5MZtPGSsJLOQDfvIJUQIdx8I,14729
+mo_logs/__init__.py,sha256=PZYfv6ooiGHmYppyksfFuXSsN5-qUcQyXd2HLD7_us8,14801
 mo_logs/constants.py,sha256=uYmXrreY2PJ4nXwFhRCySuqvBJmwRsrjFoTpy6dSf1I,2329
 mo_logs/convert.py,sha256=LjY9G-sgb64KctRkMQA2bYLMZj8iK226bwgS52wvMyA,2407
 mo_logs/exceptions.py,sha256=hrn-eoq8D69GiWw8t3O6V_lbTXySDt-ixI7kXhrtGWU,8766
 mo_logs/log_usingEmail.py,sha256=R2wxQX0KolEQt_qtkwhISICAAlSQSU1Xus9iWaoDaW8,3524
 mo_logs/log_usingFile.py,sha256=wDRvM45WarKZqAfTZKqPkO6fleGwZaM0M_qFPRVmC-k,1099
 mo_logs/log_usingHandler.py,sha256=h67fvo7PJCKx85TrE-QOMCZe2lLyCvBHBcr6BUo-2Gs,3301
 mo_logs/log_usingLogger.py,sha256=4OOsUZPemh27cUOYdLetHuI9KmF47Ut0IRmdRU0p7EM,2013
@@ -10,12 +10,12 @@
 mo_logs/log_usingMulti.py,sha256=2uUM3zHgpviKL5xJUIhi-5ReFEC51Zqv9-imi0xjBi0,1454
 mo_logs/log_usingNothing.py,sha256=RAJGGPwg4bw-eX4kDFT0kdEHH4hFsLicnJeq9Pf4Y3Q,450
 mo_logs/log_usingSES.py,sha256=hzfmQSiMnBudy4ptn73nGLUOXB-uhBXbOdUpv42HYjs,4069
 mo_logs/log_usingStream.py,sha256=t9q7Ju7F9wMKjReWXkUIcpkKRkiat2FHa---s8gdJ4s,1525
 mo_logs/log_usingThread.py,sha256=LbWlEBNGbjPBEFFIegmXhuT1_AA7H18Lv8YGDRVUpMc,2325
 mo_logs/startup.py,sha256=sMOxbRnsb-GPoMidGoTYAS9ooasv4BfwJRvyklY7fKM,6310
 mo_logs/strings.py,sha256=jo6J2Y5w2tjyOK2fMeIrfcSjBoMVgTFI6ZvY-80s2cc,24689
-mo_logs-7.403.23150.dist-info/LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
-mo_logs-7.403.23150.dist-info/METADATA,sha256=JE7rcD8Hc1X_HL0iCvDahb34e3ogdJ2a2r7PXDI3-b4,18254
-mo_logs-7.403.23150.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-mo_logs-7.403.23150.dist-info/top_level.txt,sha256=yqpeBBL3Yw2CDh1_FthlIK34KbT5cyZcAEjxlQ3MpDA,8
-mo_logs-7.403.23150.dist-info/RECORD,,
+mo_logs-8.407.23153.dist-info/LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
+mo_logs-8.407.23153.dist-info/METADATA,sha256=OEl8NQQKy4whgts9r4OihgY_Hlv3kllfcuIhnJjxVq4,17648
+mo_logs-8.407.23153.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+mo_logs-8.407.23153.dist-info/top_level.txt,sha256=yqpeBBL3Yw2CDh1_FthlIK34KbT5cyZcAEjxlQ3MpDA,8
+mo_logs-8.407.23153.dist-info/RECORD,,
```

