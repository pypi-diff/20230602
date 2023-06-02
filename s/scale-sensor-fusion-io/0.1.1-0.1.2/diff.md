# Comparing `tmp/scale_sensor_fusion_io-0.1.1.tar.gz` & `tmp/scale_sensor_fusion_io-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scale_sensor_fusion_io-0.1.1.tar", max compression
+gzip compressed data, was "scale_sensor_fusion_io-0.1.2.tar", max compression
```

## Comparing `scale_sensor_fusion_io-0.1.1.tar` & `scale_sensor_fusion_io-0.1.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     2945 2023-06-02 02:48:06.569388 scale_sensor_fusion_io-0.1.1/docs/README.md
--rw-r--r--   0        0        0      883 2023-06-02 15:32:30.284496 scale_sensor_fusion_io-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       98 2023-06-02 02:48:06.569388 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/__init__.py
--rw-r--r--   0        0        0       52 2023-05-25 07:12:37.457890 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/loaders/__init__.py
--rw-r--r--   0        0        0     2716 2023-05-22 20:30:40.190095 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/loaders/bs5_loader.py
--rw-r--r--   0        0        0     3088 2023-06-02 02:48:06.569388 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/loaders/sfs_loader.py
--rw-r--r--   0        0        0       19 2023-06-02 02:48:06.569388 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/model_converters/__init__.py
--rw-r--r--   0        0        0     8163 2023-06-02 15:31:56.196184 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/model_converters/sfs.py
--rw-r--r--   0        0        0       96 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/__init__.py
--rw-r--r--   0        0        0      456 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/annotations/__init__.py
--rw-r--r--   0        0        0      512 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/annotations/attributes.py
--rw-r--r--   0        0        0      626 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/annotations/box_2d.py
--rw-r--r--   0        0        0     1129 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/annotations/cuboid.py
--rw-r--r--   0        0        0      520 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/annotations/event.py
--rw-r--r--   0        0        0      690 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/annotations/labeled_points.py
--rw-r--r--   0        0        0      924 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/annotations/localization_adjustment.py
--rw-r--r--   0        0        0      425 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/annotations/object.py
--rw-r--r--   0        0        0      638 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/annotations/polygon.py
--rw-r--r--   0        0        0      509 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/common.py
--rw-r--r--   0        0        0      109 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/paths/__init__.py
--rw-r--r--   0        0        0      291 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/paths/attribute_path.py
--rw-r--r--   0        0        0     5350 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/paths/cuboid_path.py
--rw-r--r--   0        0        0    16186 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/paths/pose_path.py
--rw-r--r--   0        0        0      577 2023-06-02 02:48:06.573388 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/scene.py
--rw-r--r--   0        0        0      253 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/sensors/__init__.py
--rw-r--r--   0        0        0       94 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/sensors/camera/__init__.py
--rw-r--r--   0        0        0     6340 2023-06-02 02:48:06.573388 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/sensors/camera/camera_distortion.py
--rw-r--r--   0        0        0      310 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/sensors/camera/camera_intrinsics.py
--rw-r--r--   0        0        0      896 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/sensors/camera/camera_sensor.py
--rw-r--r--   0        0        0       27 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/sensors/lidar/__init__.py
--rw-r--r--   0        0        0      931 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/sensors/lidar/lidar_sensor.py
--rw-r--r--   0        0        0       28 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/sensors/radar/__init__.py
--rw-r--r--   0        0        0      825 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/sensors/radar/radar_sensor.py
--rw-r--r--   0        0        0        0 2023-03-29 20:56:32.935581 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/py.typed
--rw-r--r--   0        0        0       91 2023-05-22 20:08:31.172592 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/spec/__init__.py
--rw-r--r--   0        0        0       21 2023-05-22 20:07:37.044396 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/spec/sfs/__init__.py
--rw-r--r--   0        0        0     7837 2023-05-22 20:08:31.172592 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/spec/sfs/types.py
--rw-r--r--   0        0        0       21 2023-05-22 20:07:37.044396 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/spec/v5/__init__.py
--rw-r--r--   0        0        0     3001 2023-05-22 20:08:31.172592 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/spec/v5/types.py
--rw-r--r--   0        0        0        0 2023-05-22 20:07:37.044396 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/utils/__init__.py
--rw-r--r--   0        0        0     2005 2023-05-22 20:07:37.044396 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/utils/downsample.py
--rw-r--r--   0        0        0     2730 2023-06-02 02:48:06.573388 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/utils/generate_video.py
--rw-r--r--   0        0        0      899 2023-06-02 02:48:06.573388 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/validation/__init__.py
--rw-r--r--   0        0        0     1069 2023-06-02 02:48:06.841389 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/validation/dacite_internal/LICENSE
--rw-r--r--   0        0        0      297 2023-06-02 02:48:06.841389 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/validation/dacite_internal/README.md
--rw-r--r--   0        0        0      135 2023-06-02 02:48:06.841389 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/validation/dacite_internal/__init__.py
--rw-r--r--   0        0        0      502 2023-06-02 02:48:06.841389 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/validation/dacite_internal/config.py
--rw-r--r--   0        0        0     7388 2023-06-02 02:48:06.841389 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/validation/dacite_internal/core.py
--rw-r--r--   0        0        0       90 2023-06-02 02:48:06.837389 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/validation/dacite_internal/data.py
--rw-r--r--   0        0        0     1121 2023-06-02 02:48:06.837389 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/validation/dacite_internal/dataclasses.py
--rw-r--r--   0        0        0     2949 2023-06-02 02:48:06.837389 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/validation/dacite_internal/exceptions.py
--rw-r--r--   0        0        0     8189 2023-06-02 02:48:06.837389 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/validation/dacite_internal/types.py
--rw-r--r--   0        0        0     2802 2023-06-02 02:48:06.573388 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/validation/error.py
--rw-r--r--   0        0        0      965 2023-06-02 02:48:06.573388 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/validation/helpers.py
--rw-r--r--   0        0        0       19 2023-06-02 02:48:06.573388 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/validation/parser/__init__.py
--rw-r--r--   0        0        0     7530 2023-06-02 02:48:06.573388 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/validation/parser/sfs.py
--rw-r--r--   0        0        0     6932 2023-06-02 02:48:06.573388 scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/validation/validate.py
--rw-r--r--   0        0        0     3756 1970-01-01 00:00:00.000000 scale_sensor_fusion_io-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2945 2023-06-02 02:48:06.569388 scale_sensor_fusion_io-0.1.2/docs/README.md
+-rw-r--r--   0        0        0      883 2023-06-02 17:34:42.069959 scale_sensor_fusion_io-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-06-02 02:48:06.569388 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/__init__.py
+-rw-r--r--   0        0        0       52 2023-05-25 07:12:37.457890 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/loaders/__init__.py
+-rw-r--r--   0        0        0     2716 2023-05-22 20:30:40.190095 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/loaders/bs5_loader.py
+-rw-r--r--   0        0        0     3088 2023-06-02 02:48:06.569388 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/loaders/sfs_loader.py
+-rw-r--r--   0        0        0       19 2023-06-02 02:48:06.569388 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/model_converters/__init__.py
+-rw-r--r--   0        0        0     8163 2023-06-02 16:33:35.150043 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/model_converters/sfs.py
+-rw-r--r--   0        0        0       96 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/__init__.py
+-rw-r--r--   0        0        0      456 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/annotations/__init__.py
+-rw-r--r--   0        0        0      512 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/annotations/attributes.py
+-rw-r--r--   0        0        0      626 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/annotations/box_2d.py
+-rw-r--r--   0        0        0     1129 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/annotations/cuboid.py
+-rw-r--r--   0        0        0      520 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/annotations/event.py
+-rw-r--r--   0        0        0      690 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/annotations/labeled_points.py
+-rw-r--r--   0        0        0      924 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/annotations/localization_adjustment.py
+-rw-r--r--   0        0        0      425 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/annotations/object.py
+-rw-r--r--   0        0        0      638 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/annotations/polygon.py
+-rw-r--r--   0        0        0      509 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/common.py
+-rw-r--r--   0        0        0      109 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/paths/__init__.py
+-rw-r--r--   0        0        0      291 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/paths/attribute_path.py
+-rw-r--r--   0        0        0     5350 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/paths/cuboid_path.py
+-rw-r--r--   0        0        0    16186 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/paths/pose_path.py
+-rw-r--r--   0        0        0      577 2023-06-02 02:48:06.573388 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/scene.py
+-rw-r--r--   0        0        0      253 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/sensors/__init__.py
+-rw-r--r--   0        0        0       94 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/sensors/camera/__init__.py
+-rw-r--r--   0        0        0     6340 2023-06-02 02:48:06.573388 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/sensors/camera/camera_distortion.py
+-rw-r--r--   0        0        0      310 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/sensors/camera/camera_intrinsics.py
+-rw-r--r--   0        0        0      896 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/sensors/camera/camera_sensor.py
+-rw-r--r--   0        0        0       27 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/sensors/lidar/__init__.py
+-rw-r--r--   0        0        0      931 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/sensors/lidar/lidar_sensor.py
+-rw-r--r--   0        0        0       28 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/sensors/radar/__init__.py
+-rw-r--r--   0        0        0      825 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/sensors/radar/radar_sensor.py
+-rw-r--r--   0        0        0        0 2023-03-29 20:56:32.935581 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/py.typed
+-rw-r--r--   0        0        0       91 2023-05-22 20:08:31.172592 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/spec/__init__.py
+-rw-r--r--   0        0        0       21 2023-05-22 20:07:37.044396 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/spec/sfs/__init__.py
+-rw-r--r--   0        0        0     7837 2023-05-22 20:08:31.172592 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/spec/sfs/types.py
+-rw-r--r--   0        0        0       21 2023-05-22 20:07:37.044396 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/spec/v5/__init__.py
+-rw-r--r--   0        0        0     3001 2023-05-22 20:08:31.172592 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/spec/v5/types.py
+-rw-r--r--   0        0        0        0 2023-05-22 20:07:37.044396 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/utils/__init__.py
+-rw-r--r--   0        0        0     2005 2023-05-22 20:07:37.044396 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/utils/downsample.py
+-rw-r--r--   0        0        0     2730 2023-06-02 02:48:06.573388 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/utils/generate_video.py
+-rw-r--r--   0        0        0      899 2023-06-02 02:48:06.573388 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/validation/__init__.py
+-rw-r--r--   0        0        0     1069 2023-06-02 02:48:06.841389 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/validation/dacite_internal/LICENSE
+-rw-r--r--   0        0        0      297 2023-06-02 02:48:06.841389 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/validation/dacite_internal/README.md
+-rw-r--r--   0        0        0      135 2023-06-02 02:48:06.841389 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/validation/dacite_internal/__init__.py
+-rw-r--r--   0        0        0      502 2023-06-02 02:48:06.841389 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/validation/dacite_internal/config.py
+-rw-r--r--   0        0        0     7388 2023-06-02 02:48:06.841389 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/validation/dacite_internal/core.py
+-rw-r--r--   0        0        0       90 2023-06-02 02:48:06.837389 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/validation/dacite_internal/data.py
+-rw-r--r--   0        0        0     1121 2023-06-02 02:48:06.837389 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/validation/dacite_internal/dataclasses.py
+-rw-r--r--   0        0        0     2949 2023-06-02 02:48:06.837389 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/validation/dacite_internal/exceptions.py
+-rw-r--r--   0        0        0     8189 2023-06-02 02:48:06.837389 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/validation/dacite_internal/types.py
+-rw-r--r--   0        0        0     2802 2023-06-02 02:48:06.573388 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/validation/error.py
+-rw-r--r--   0        0        0      965 2023-06-02 02:48:06.573388 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/validation/helpers.py
+-rw-r--r--   0        0        0       19 2023-06-02 02:48:06.573388 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/validation/parser/__init__.py
+-rw-r--r--   0        0        0     7530 2023-06-02 02:48:06.573388 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/validation/parser/sfs.py
+-rw-r--r--   0        0        0     8006 2023-06-02 17:44:19.436053 scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/validation/validate.py
+-rw-r--r--   0        0        0     3756 1970-01-01 00:00:00.000000 scale_sensor_fusion_io-0.1.2/PKG-INFO
```

### Comparing `scale_sensor_fusion_io-0.1.1/docs/README.md` & `scale_sensor_fusion_io-0.1.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.1/pyproject.toml` & `scale_sensor_fusion_io-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scale_sensor_fusion_io"
-version = "0.1.1"
+version = "0.1.2"
 description = "Library for working with timestamp-based sensor fusion scenes"
 authors = [
     "Michael Choi <michael.choi@scale.com>", 
     "Rodrigo Belfiore <rodrigo.belfiore@scale.com>"
 ]
 readme = ["docs/README.md"]
```

### Comparing `scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/loaders/bs5_loader.py` & `scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/loaders/bs5_loader.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/loaders/sfs_loader.py` & `scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/loaders/sfs_loader.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/model_converters/sfs.py` & `scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/model_converters/sfs.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/annotations/attributes.py` & `scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/annotations/attributes.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/annotations/box_2d.py` & `scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/annotations/box_2d.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/annotations/cuboid.py` & `scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/annotations/cuboid.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/annotations/event.py` & `scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/annotations/event.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/annotations/labeled_points.py` & `scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/annotations/labeled_points.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/annotations/localization_adjustment.py` & `scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/annotations/localization_adjustment.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/annotations/polygon.py` & `scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/annotations/polygon.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/paths/cuboid_path.py` & `scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/paths/cuboid_path.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/paths/pose_path.py` & `scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/paths/pose_path.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/scene.py` & `scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/scene.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/sensors/camera/camera_distortion.py` & `scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/sensors/camera/camera_distortion.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/sensors/camera/camera_sensor.py` & `scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/sensors/camera/camera_sensor.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/sensors/lidar/lidar_sensor.py` & `scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/sensors/lidar/lidar_sensor.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/models/sensors/radar/radar_sensor.py` & `scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/models/sensors/radar/radar_sensor.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/spec/sfs/types.py` & `scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/spec/sfs/types.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/spec/v5/types.py` & `scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/spec/v5/types.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/utils/downsample.py` & `scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/utils/downsample.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/utils/generate_video.py` & `scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/utils/generate_video.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/validation/__init__.py` & `scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/validation/dacite_internal/LICENSE` & `scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/validation/dacite_internal/LICENSE`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/validation/dacite_internal/core.py` & `scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/validation/dacite_internal/core.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/validation/dacite_internal/dataclasses.py` & `scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/validation/dacite_internal/dataclasses.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/validation/dacite_internal/exceptions.py` & `scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/validation/dacite_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/validation/dacite_internal/types.py` & `scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/validation/dacite_internal/types.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/validation/error.py` & `scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/validation/error.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/validation/helpers.py` & `scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/validation/helpers.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/validation/parser/sfs.py` & `scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/validation/parser/sfs.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.1/scale_sensor_fusion_io/validation/validate.py` & `scale_sensor_fusion_io-0.1.2/scale_sensor_fusion_io/validation/validate.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     ErrorDetails,
     PathField,
     ValidationResult,
 )
 from .helpers import is_monotonically_increasing
 
 MICRO_IN_SEC = 1e6
+MAX_FPS = 100
+MIN_FPS = 1
 
 
 def _handle_result(
     res: ValidationResult, error_details: List[ErrorDetails], path: List[PathField] = []
 ) -> None:
     if res:
         error_details.extend(
@@ -46,14 +48,20 @@
     content_timestamps = [frame.timestamp for frame in sensor.frames]
 
     _handle_result(
         validate_timestamps(content_timestamps), error_details, path=["frames"]
     )
     _handle_result(validate_fps(content_timestamps), error_details)
 
+    # pose validation
+    _handle_result(
+        validate_pose_path(sensor.poses),
+        error_details,
+    )
+
     if len(error_details) > 0:
         return DataValidationError(details=error_details)
 
     return None
 
 
 def validate_timestamps(timestamps: List[int]) -> ValidationResult:
@@ -66,20 +74,30 @@
         )
     if not is_monotonically_increasing(timestamps):
         error_details.append(
             ErrorDetails.from_msg(
                 "timestamps be monotonically increasing",
             )
         )
+
+    max_ts_diff = MICRO_IN_SEC / MIN_FPS
+    max_init_frame_ts = max_ts_diff * 100  # allow a padding of 100 frames
+    if timestamps[0] > max_init_frame_ts:
+        error_details.append(
+            ErrorDetails.from_msg(
+                f"timestamps must be normalized: {timestamps[0]} > {max_init_frame_ts}",
+            )
+        )
+
     if len(error_details) > 0:
         return DataValidationError(details=error_details)
     return None
 
 
-def validate_fps(timestamps: List[int], max_fps: int = 100) -> ValidationResult:
+def validate_fps(timestamps: List[int], max_fps: int = MAX_FPS) -> ValidationResult:
     error_details: List[ErrorDetails] = []
 
     # compute approximate fps from timestamps
     avg_ts_diffs = np.mean([t2 - t1 for t1, t2 in zip(timestamps, timestamps[1:])])
     fps = MICRO_IN_SEC / avg_ts_diffs
 
     if fps > max_fps:
@@ -101,14 +119,20 @@
     content_timestamps = [frame.timestamp for frame in sensor.frames]
 
     _handle_result(
         validate_timestamps(content_timestamps), error_details, path=["frames"]
     )
     _handle_result(validate_fps(content_timestamps), error_details)
 
+    # pose validation
+    _handle_result(
+        validate_pose_path(sensor.poses),
+        error_details,
+    )
+
     for frame in sensor.frames:
         ### validate all fields of points have same length
         pos_length = len(frame.points.positions)
         if (
             frame.points.intensities is not None
             and len(frame.points.intensities) != pos_length
         ):
@@ -137,14 +161,26 @@
 
     if len(error_details) > 0:
         return DataValidationError(details=error_details)
 
     return None
 
 
+def validate_pose_path(pose_path: PosePath) -> ValidationResult:
+    error_details: List[ErrorDetails] = []
+
+    pose_timestamps: List[int] = pose_path.index.tolist()
+    _handle_result(validate_timestamps(pose_timestamps), error_details, path=["poses"])
+
+    if len(error_details) > 0:
+        return DataValidationError(details=error_details)
+
+    return None
+
+
 def validate_camera(sensor: CameraSensor) -> ValidationResult:
     """Validate camera sensor"""
     error_details: List[ErrorDetails] = []
 
     # camera content
     content_timestamps: List[int] = []
     content_timestamps_path: List[PathField] = []
@@ -165,14 +201,20 @@
         path=content_timestamps_path,
     )
     _handle_result(
         validate_fps(content_timestamps),
         error_details,
     )
 
+    # pose validation
+    _handle_result(
+        validate_pose_path(sensor.poses),
+        error_details,
+    )
+
     if len(error_details) > 0:
         return DataValidationError(details=error_details)
 
     return None
 
 
 def validate_sensor(sensor: Sensor) -> ValidationResult:
```

### Comparing `scale_sensor_fusion_io-0.1.1/PKG-INFO` & `scale_sensor_fusion_io-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scale-sensor-fusion-io
-Version: 0.1.1
+Version: 0.1.2
 Summary: Library for working with timestamp-based sensor fusion scenes
 Author: Michael Choi
 Author-email: michael.choi@scale.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

