# Comparing `tmp/OpenLA-0.2.8.tar.gz` & `tmp/openla-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenLA-0.2.8.tar", max compression
+gzip compressed data, was "openla-0.2.9.tar", max compression
```

## Comparing `OpenLA-0.2.8.tar` & `openla-0.2.9.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1061 2022-04-08 07:14:44.505967 OpenLA-0.2.8/LICENSE
--rw-r--r--   0        0        0      134 2022-05-11 05:55:09.038661 OpenLA-0.2.8/OpenLA/__init__.py
--rw-r--r--   0        0        0     1662 2022-05-11 05:55:09.038488 OpenLA-0.2.8/OpenLA/check.py
--rw-r--r--   0        0        0    21300 2022-05-11 05:55:09.038285 OpenLA-0.2.8/OpenLA/course_information.py
--rw-r--r--   0        0        0     4356 2022-05-11 05:55:09.038054 OpenLA-0.2.8/OpenLA/data_classes/event_stream.py
--rw-r--r--   0        0        0     3347 2022-05-11 05:55:09.037864 OpenLA-0.2.8/OpenLA/data_classes/operation_count.py
--rw-r--r--   0        0        0    11368 2022-05-11 05:55:09.037640 OpenLA-0.2.8/OpenLA/data_classes/pagewise_aggregation.py
--rw-r--r--   0        0        0     3756 2022-05-11 05:55:09.037413 OpenLA-0.2.8/OpenLA/data_classes/time_range_aggregation.py
--rw-r--r--   0        0        0    30845 2022-05-11 05:55:09.037169 OpenLA-0.2.8/OpenLA/data_conversion.py
--rw-r--r--   0        0        0    13359 2022-05-11 05:55:09.036917 OpenLA-0.2.8/OpenLA/data_extraction.py
--rw-r--r--   0        0        0    21350 2022-05-11 05:55:09.036687 OpenLA-0.2.8/OpenLA/data_visualization.py
--rw-r--r--   0        0        0     4474 2022-05-30 01:32:58.558993 OpenLA-0.2.8/README.md
--rw-r--r--   0        0        0      629 2022-06-03 04:26:40.267540 OpenLA-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     5275 2022-06-03 05:17:06.032908 OpenLA-0.2.8/setup.py
--rw-r--r--   0        0        0     5092 2022-06-03 05:17:06.033089 OpenLA-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2022-04-08 07:14:44.505967 openla-0.2.9/LICENSE
+-rw-r--r--   0        0        0      134 2022-05-11 05:55:09.038661 openla-0.2.9/OpenLA/__init__.py
+-rw-r--r--   0        0        0     1662 2022-05-11 05:55:09.038488 openla-0.2.9/OpenLA/check.py
+-rw-r--r--   0        0        0    21404 2023-06-02 02:54:54.137634 openla-0.2.9/OpenLA/course_information.py
+-rw-r--r--   0        0        0     4356 2022-05-11 05:55:09.038054 openla-0.2.9/OpenLA/data_classes/event_stream.py
+-rw-r--r--   0        0        0     3347 2022-05-11 05:55:09.037864 openla-0.2.9/OpenLA/data_classes/operation_count.py
+-rw-r--r--   0        0        0    11368 2022-05-11 05:55:09.037640 openla-0.2.9/OpenLA/data_classes/pagewise_aggregation.py
+-rw-r--r--   0        0        0     3756 2022-05-11 05:55:09.037413 openla-0.2.9/OpenLA/data_classes/time_range_aggregation.py
+-rw-r--r--   0        0        0    30845 2022-05-11 05:55:09.037169 openla-0.2.9/OpenLA/data_conversion.py
+-rw-r--r--   0        0        0    13359 2022-05-11 05:55:09.036917 openla-0.2.9/OpenLA/data_extraction.py
+-rw-r--r--   0        0        0    21350 2022-05-11 05:55:09.036687 openla-0.2.9/OpenLA/data_visualization.py
+-rw-r--r--   0        0        0     4474 2022-05-30 01:32:58.558993 openla-0.2.9/README.md
+-rw-r--r--   0        0        0      629 2023-06-02 06:30:12.610139 openla-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     5143 1970-01-01 00:00:00.000000 openla-0.2.9/PKG-INFO
```

### Comparing `OpenLA-0.2.8/LICENSE` & `openla-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `OpenLA-0.2.8/OpenLA/check.py` & `openla-0.2.9/OpenLA/check.py`

 * *Files identical despite different names*

### Comparing `OpenLA-0.2.8/OpenLA/course_information.py` & `openla-0.2.9/OpenLA/course_information.py`

 * *Files 2% similar despite different names*

```diff
@@ -409,28 +409,31 @@
     def lecture_week_to_contents_id(self, lecture_week):
         """
         Get the content(s) id used in the lecture of the argument "lecture_week".
 
         :param lecture_week: The lecture week or list of lecture weeks
         :type lecture_week: int or list[int]
 
-        :return: The contents id corresponding to the lecture week.
+        :return: The contents id corresponding to the lecture week(s).
 
-                 If the argument “lecture_week” is given as a list, the function returns list of contents ids.
+                 If there is more than one relevant contents id, the function returns a list with them.
 
         :rtype: str or list[str]
         """
         assert _is_int(lecture_week) or _is_int_list(lecture_week), "please pass int-type or list[int]-type"
 
         df = self._lecturematerial.df
         df['lecture'] = df['lecture'].apply(int)  # column 'lecture' is float (e.g. 1.0), so converting to integer
         df = df.set_index('lecture')
 
         if _is_int(lecture_week):
-            return df.at[lecture_week, 'contentsid']
+            cid = df.at[lecture_week, 'contentsid']
+            if isinstance(cid, pd.Series):
+                return cid.tolist()
+            return cid
 
         elif _is_int_list(lecture_week):
             contents_ids = df.loc[lecture_week, 'contentsid'].tolist()
             return contents_ids
 
 
     def num_pages_of_contents(self, contents_id):
@@ -535,16 +538,16 @@
     :param lecture_time_file: If you want to specify the file path directly, use this argument.
     :type lecture_time_file: str or None
 
     :param quiz_score_file: If you want to specify the file path directly, use this argument.
     :type quiz_score_file: str or None
 
     :returns:
-    - course_info - Instances of class "CourseInformation"
-    - event_stream - Instances of class "EventStream"
+        - course_info - Instances of class "CourseInformation"
+        - event_stream - Instances of class "EventStream"
     """
 
     course_info = CourseInformation(course_id=course_id, files_dir=files_dir,
                                     event_stream_file=event_stream_file, lecture_material_file=lecture_material_file,
                                     lecture_time_file=lecture_time_file, quiz_score_file=quiz_score_file,
                                     grade_point_file=grade_point_file)
     event_stream = course_info.load_eventstream()
```

### Comparing `OpenLA-0.2.8/OpenLA/data_classes/event_stream.py` & `openla-0.2.9/OpenLA/data_classes/event_stream.py`

 * *Files identical despite different names*

### Comparing `OpenLA-0.2.8/OpenLA/data_classes/operation_count.py` & `openla-0.2.9/OpenLA/data_classes/operation_count.py`

 * *Files identical despite different names*

### Comparing `OpenLA-0.2.8/OpenLA/data_classes/pagewise_aggregation.py` & `openla-0.2.9/OpenLA/data_classes/pagewise_aggregation.py`

 * *Files identical despite different names*

### Comparing `OpenLA-0.2.8/OpenLA/data_classes/time_range_aggregation.py` & `openla-0.2.9/OpenLA/data_classes/time_range_aggregation.py`

 * *Files identical despite different names*

### Comparing `OpenLA-0.2.8/OpenLA/data_conversion.py` & `openla-0.2.9/OpenLA/data_conversion.py`

 * *Files identical despite different names*

### Comparing `OpenLA-0.2.8/OpenLA/data_extraction.py` & `openla-0.2.9/OpenLA/data_extraction.py`

 * *Files identical despite different names*

### Comparing `OpenLA-0.2.8/OpenLA/data_visualization.py` & `openla-0.2.9/OpenLA/data_visualization.py`

 * *Files identical despite different names*

### Comparing `OpenLA-0.2.8/README.md` & `openla-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `OpenLA-0.2.8/pyproject.toml` & `openla-0.2.9/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "OpenLA"
-version = "0.2.8"
+version = "0.2.9"
 description = "Open source library for e-Book log analysis"
 authors = ["LIMU <repository@limu.ait.kyushu-u.ac.jp>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "OpenLA"},
 ]
```

### Comparing `OpenLA-0.2.8/PKG-INFO` & `openla-0.2.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: openla
-Version: 0.2.8
+Version: 0.2.9
 Summary: Open source library for e-Book log analysis
 License: MIT
 Author: LIMU
 Author-email: repository@limu.ait.kyushu-u.ac.jp
 Requires-Python: >=3.7.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: matplotlib (>=3.3.2,<4.0.0)
 Requires-Dist: numpy (>=1.18.15,<2.0.0)
 Requires-Dist: pandas (>=1.3,<2.0)
 Description-Content-Type: text/markdown
 
 # OpenLA: open-source library for e-book log analysis
```

