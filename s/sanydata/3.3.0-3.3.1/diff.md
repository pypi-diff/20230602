# Comparing `tmp/sanydata-3.3.0.tar.gz` & `tmp/sanydata-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sanydata-3.3.0.tar", last modified: Tue May  9 02:31:34 2023, max compression
+gzip compressed data, was "sanydata-3.3.1.tar", last modified: Fri Jun  2 06:34:38 2023, max compression
```

## Comparing `sanydata-3.3.0.tar` & `sanydata-3.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-05-09 02:31:34.550407 sanydata-3.3.0/
--rw-r--r--   0 thao       (501) staff       (20)      302 2023-05-09 02:31:34.550186 sanydata-3.3.0/PKG-INFO
-drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-05-09 02:31:34.545909 sanydata-3.3.0/sanydata/
--rw-r--r--   0 thao       (501) staff       (20)      103 2022-04-09 07:48:22.000000 sanydata-3.3.0/sanydata/__init__.py
--rw-r--r--   0 thao       (501) staff       (20)   114500 2023-05-09 02:31:01.000000 sanydata-3.3.0/sanydata/datatools.py
--rw-r--r--   0 thao       (501) staff       (20)    20291 2022-08-29 10:08:03.000000 sanydata-3.3.0/sanydata/model_data_message_pb2.py
--rw-r--r--   0 thao       (501) staff       (20)    20370 2022-08-29 10:08:03.000000 sanydata-3.3.0/sanydata/model_data_message_pb2_grpc.py
-drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-05-09 02:31:34.547408 sanydata-3.3.0/sanydata.egg-info/
--rw-r--r--   0 thao       (501) staff       (20)      302 2023-05-09 02:31:33.000000 sanydata-3.3.0/sanydata.egg-info/PKG-INFO
--rw-r--r--   0 thao       (501) staff       (20)      371 2023-05-09 02:31:34.000000 sanydata-3.3.0/sanydata.egg-info/SOURCES.txt
--rw-r--r--   0 thao       (501) staff       (20)        1 2023-05-09 02:31:34.000000 sanydata-3.3.0/sanydata.egg-info/dependency_links.txt
--rw-r--r--   0 thao       (501) staff       (20)      130 2023-05-09 02:31:34.000000 sanydata-3.3.0/sanydata.egg-info/requires.txt
--rw-r--r--   0 thao       (501) staff       (20)       15 2023-05-09 02:31:34.000000 sanydata-3.3.0/sanydata.egg-info/top_level.txt
--rw-r--r--   0 thao       (501) staff       (20)       38 2023-05-09 02:31:34.550486 sanydata-3.3.0/setup.cfg
--rw-r--r--   0 thao       (501) staff       (20)      999 2023-05-09 02:31:14.000000 sanydata-3.3.0/setup.py
-drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-05-09 02:31:34.549447 sanydata-3.3.0/utils/
--rw-r--r--   0 thao       (501) staff       (20)      103 2022-04-09 07:48:22.000000 sanydata-3.3.0/utils/__init__.py
--rw-r--r--   0 thao       (501) staff       (20)     1328 2022-04-14 01:33:04.000000 sanydata-3.3.0/utils/cos_handler.py
--rw-r--r--   0 thao       (501) staff       (20)     1080 2022-04-13 10:48:13.000000 sanydata-3.3.0/utils/file_operation.py
--rw-r--r--   0 thao       (501) staff       (20)      667 2022-04-14 01:24:56.000000 sanydata-3.3.0/utils/local_handler.py
+drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-06-02 06:34:38.868323 sanydata-3.3.1/
+-rw-r--r--   0 thao       (501) staff       (20)      302 2023-06-02 06:34:38.868035 sanydata-3.3.1/PKG-INFO
+drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-06-02 06:34:38.864328 sanydata-3.3.1/sanydata/
+-rw-r--r--   0 thao       (501) staff       (20)      103 2022-04-09 07:48:22.000000 sanydata-3.3.1/sanydata/__init__.py
+-rw-r--r--   0 thao       (501) staff       (20)   117531 2023-06-02 06:32:38.000000 sanydata-3.3.1/sanydata/datatools.py
+-rw-r--r--   0 thao       (501) staff       (20)    20291 2022-08-29 10:08:03.000000 sanydata-3.3.1/sanydata/model_data_message_pb2.py
+-rw-r--r--   0 thao       (501) staff       (20)    20370 2022-08-29 10:08:03.000000 sanydata-3.3.1/sanydata/model_data_message_pb2_grpc.py
+drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-06-02 06:34:38.865989 sanydata-3.3.1/sanydata.egg-info/
+-rw-r--r--   0 thao       (501) staff       (20)      302 2023-06-02 06:34:38.000000 sanydata-3.3.1/sanydata.egg-info/PKG-INFO
+-rw-r--r--   0 thao       (501) staff       (20)      371 2023-06-02 06:34:38.000000 sanydata-3.3.1/sanydata.egg-info/SOURCES.txt
+-rw-r--r--   0 thao       (501) staff       (20)        1 2023-06-02 06:34:38.000000 sanydata-3.3.1/sanydata.egg-info/dependency_links.txt
+-rw-r--r--   0 thao       (501) staff       (20)      130 2023-06-02 06:34:38.000000 sanydata-3.3.1/sanydata.egg-info/requires.txt
+-rw-r--r--   0 thao       (501) staff       (20)       15 2023-06-02 06:34:38.000000 sanydata-3.3.1/sanydata.egg-info/top_level.txt
+-rw-r--r--   0 thao       (501) staff       (20)       38 2023-06-02 06:34:38.868407 sanydata-3.3.1/setup.cfg
+-rw-r--r--   0 thao       (501) staff       (20)      999 2023-06-02 06:30:09.000000 sanydata-3.3.1/setup.py
+drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-06-02 06:34:38.867409 sanydata-3.3.1/utils/
+-rw-r--r--   0 thao       (501) staff       (20)      103 2022-04-09 07:48:22.000000 sanydata-3.3.1/utils/__init__.py
+-rw-r--r--   0 thao       (501) staff       (20)     1328 2022-04-14 01:33:04.000000 sanydata-3.3.1/utils/cos_handler.py
+-rw-r--r--   0 thao       (501) staff       (20)     1080 2022-04-13 10:48:13.000000 sanydata-3.3.1/utils/file_operation.py
+-rw-r--r--   0 thao       (501) staff       (20)      667 2022-04-14 01:24:56.000000 sanydata-3.3.1/utils/local_handler.py
```

### Comparing `sanydata-3.3.0/sanydata/datatools.py` & `sanydata-3.3.1/sanydata/datatools.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,15 @@
                 airDensity
                 annualAverageWindSpeed
                 turbulenceIntensity
                 windShear
                 inflowAngle
                 windDistributionParameter
                 scadaVersion
+                turbineTag
                 }
                 }
                 """)
 key_map = dict(zip(
     [
         "turbineId",
         "innerTurbineName",
@@ -139,14 +140,15 @@
         "airDensity",
         "annualAverageWindSpeed",
         "turbulenceIntensity",
         "windShear",
         "inflowAngle",
         "windDistributionParameter",
         "scadaVersion",
+        "turbineTag"
     ],
     [
         "turbine_id",
         "inner_turbine_name",
         "type_id",
         "type_name",
         "inner_turbine_type",
@@ -191,15 +193,16 @@
         "wind_id",
         "air_density",
         "annual_average_wind_speed",
         "turbulence_intensity",
         "wind_shear",
         "inflow_angle",
         "wind_distribution_parameter",
-        "scada_version"
+        "scada_version",
+        "turbine_tag"
     ]
 ))
 options = [('grpc.max_message_length', 64 * 1024 * 1024), ('grpc.max_receive_message_length', 64 * 1024 * 1024),
            ('grpc.service_config', '{ "retryPolicy":{ "maxAttempts": 4, "initialBackoff": "0.3s", "maxBackoff": "2s", '
                                    '"backoffMutiplier": 2, "retryableStatusCodes": [ "UNAVAILABLE" ] } }')]
 
 
@@ -226,15 +229,15 @@
 
     return wrapper
 
 
 class DataTools(object):
     # This programme is to get data.
     PROGRAMME = 'DataTools'
-    VERSION = '3.3.0'
+    VERSION = '3.3.1'
 
     def __init__(self, stub=None, es_hosts='http://es.sanywind.net:9200/'):
         self.es = Elasticsearch(hosts=es_hosts)
 
         if stub:
             with grpc.insecure_channel(stub, options=options) as channel:
                 stub = model_data_message_pb2_grpc.ModelDataMessageStub(channel)
@@ -780,14 +783,16 @@
           （上述中**代表最终文件命名，命名时应尽可能避免多文件保存到本地时进行覆盖，建议采用当前时间戳）
 
         """
 
         model_end_time = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
         model_start_time = os.getenv('ModelStartTime')
         task_id = int(os.getenv('TaskId'))
+        data_start_time = str(data_start_time)[:10] + ' 00:00:01'
+        data_end_time = str(data_end_time)[:10] + ' 23:59:59'
         if not model_version:
             model_version = os.getenv('ProjectVersion')
 
         fig_fio = None
         log_fio = None
         file_fio = None
         # 本地图片处理
@@ -1680,14 +1685,90 @@
             if str(result) in ['nan', 'None']:
                 result = '数据库表df_wind_farm_turbine中缺少 {} 风场信息'.format(farm)
             else:
                 result = int(result)
 
         return result
 
+    def is_watercolling_by_turbine(self, farm, turbine):
+        """
+        :param farm: 需要查询的风场，例“TYSFCA”
+        :param turbine: 需要查询的机组号，例"001"
+        :return: 所查询机组是否为水冷机组，返回bool
+        """
+
+        df_turbine = self.df_wind_farm_turbine.query('pinyin_code == @farm & inner_turbine_name == @turbine')
+        if len(df_turbine) == 0:
+            result = False
+        else:
+            result = df_turbine['turbine_tag'].unique().tolist()[0]
+            if str(result) in ['nan', 'None']:
+                result = False
+            else:
+                result = 'waterColling' in result.split(',')
+
+        return result
+
+    def is_watercolling_open_by_turbine(self, farm, turbine):
+        """
+        :param farm: 需要查询的风场，例“TYSFCA”
+        :param turbine: 需要查询的机组号，例"001"
+        :return: 所查询机组是否为水冷机组，返回bool
+        """
+
+        df_turbine = self.df_wind_farm_turbine.query('pinyin_code == @farm & inner_turbine_name == @turbine')
+        if len(df_turbine) == 0:
+            result = False
+        else:
+            result = df_turbine['turbine_tag'].unique().tolist()[0]
+            if str(result) in ['nan', 'None']:
+                result = False
+            else:
+                result = 'waterColling-open' in result.split(',')
+
+        return result
+
+    def is_turnedbox_upward_by_turbine(self, farm, turbine):
+        """
+        :param farm: 需要查询的风场，例“TYSFCA”
+        :param turbine: 需要查询的机组号，例"001"
+        :return: 所查询机组是否为水冷机组，返回bool
+        """
+
+        df_turbine = self.df_wind_farm_turbine.query('pinyin_code == @farm & inner_turbine_name == @turbine')
+        if len(df_turbine) == 0:
+            result = False
+        else:
+            result = df_turbine['turbine_tag'].unique().tolist()[0]
+            if str(result) in ['nan', 'None']:
+                result = False
+            else:
+                result = 'turnedBoxUpward' in result.split(',')
+
+        return result
+
+    def is_kneading_tower_by_turbine(self, farm, turbine):
+        """
+        :param farm: 需要查询的风场，例“TYSFCA”
+        :param turbine: 需要查询的机组号，例"001"
+        :return: 所查询机组是否为水冷机组，返回bool
+        """
+
+        df_turbine = self.df_wind_farm_turbine.query('pinyin_code == @farm & inner_turbine_name == @turbine')
+        if len(df_turbine) == 0:
+            result = False
+        else:
+            result = df_turbine['turbine_tag'].unique().tolist()[0]
+            if str(result) in ['nan', 'None']:
+                result = False
+            else:
+                result = 'kneadingTower' in result.split(',')
+
+        return result
+
 
 class EsHandler(object):
     # This programme is to get label from es.
     PROGRAMME = 'EsHandler'
     VERSION = '1.0.1'
 
     """
```

### Comparing `sanydata-3.3.0/sanydata/model_data_message_pb2.py` & `sanydata-3.3.1/sanydata/model_data_message_pb2.py`

 * *Files identical despite different names*

### Comparing `sanydata-3.3.0/sanydata/model_data_message_pb2_grpc.py` & `sanydata-3.3.1/sanydata/model_data_message_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sanydata-3.3.0/setup.py` & `sanydata-3.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import sys
 import importlib
 
 importlib.reload(sys)
 
 setup(
     name="sanydata",
-    version="3.3.0",
+    version="3.3.1",
     keywords=["pip", "sanydata", "thao"],
     description="get data and get wind farm information",
     long_description="get data and get wind farm information",
     license="MIT Licence",
 
     url="http://gitlab.sanywind.net/sanydata/sanydata",
     author="thao",
```

### Comparing `sanydata-3.3.0/utils/cos_handler.py` & `sanydata-3.3.1/utils/cos_handler.py`

 * *Files identical despite different names*

### Comparing `sanydata-3.3.0/utils/file_operation.py` & `sanydata-3.3.1/utils/file_operation.py`

 * *Files identical despite different names*

### Comparing `sanydata-3.3.0/utils/local_handler.py` & `sanydata-3.3.1/utils/local_handler.py`

 * *Files identical despite different names*

