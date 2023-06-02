# Comparing `tmp/pybaseutils-0.8.1.tar.gz` & `tmp/pybaseutils-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pybaseutils-0.8.1.tar", last modified: Wed May 31 02:57:58 2023, max compression
+gzip compressed data, was "dist/pybaseutils-0.8.2.tar", last modified: Fri Jun  2 01:38:34 2023, max compression
```

## Comparing `pybaseutils-0.8.1.tar` & `pybaseutils-0.8.2.tar`

### file list

```diff
@@ -1,135 +1,136 @@
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1073 2021-12-28 07:55:19.000000 pybaseutils-0.8.1/LICENCE
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3952 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/PKG-INFO
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/pybaseutils/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5094 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/base64_utils.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/pybaseutils/base_audio/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4792 2023-05-16 07:29:26.000000 pybaseutils-0.8.1/pybaseutils/base_audio/audio_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      109 2023-05-11 02:35:54.000000 pybaseutils-0.8.1/pybaseutils/base_audio/__init__.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2155 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/batch_utils.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/pybaseutils/cluster/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1952 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/cluster/kmean.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3038 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/cluster/maxmin_distance.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2744 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/cluster/similarity.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/cluster/__init__.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7049 2022-11-16 02:12:19.000000 pybaseutils-0.8.1/pybaseutils/color_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5027 2022-06-14 03:12:10.000000 pybaseutils-0.8.1/pybaseutils/config_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    10076 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/coords_utils.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/pybaseutils/cvutils/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7528 2022-11-25 09:29:09.000000 pybaseutils-0.8.1/pybaseutils/cvutils/corner_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     8265 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/cvutils/mouse_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7804 2023-05-24 02:10:31.000000 pybaseutils-0.8.1/pybaseutils/cvutils/video_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      130 2022-11-25 02:19:14.000000 pybaseutils-0.8.1/pybaseutils/cvutils/__init__.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/pybaseutils/dataloader/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7363 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/dataloader/dataset.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    12136 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/dataloader/parser_labelme.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    11897 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/dataloader/parser_textdata.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    19470 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/dataloader/parser_voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/dataloader/__init__.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    32583 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/file_utils.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/pybaseutils/font_style/
--rwxrwxrwx   0 dm        (1000) dm        (1000)      537 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/font_style/__init__.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7786 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/font_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    13053 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/geometry_tools.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5306 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/heatmap_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    97144 2023-05-30 10:28:33.000000 pybaseutils-0.8.1/pybaseutils/image_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4255 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/json_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     6813 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/log.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1874 2022-10-10 02:04:07.000000 pybaseutils-0.8.1/pybaseutils/logger.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/pybaseutils/maker/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4645 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/maker/convert_labelme2voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4366 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/maker/convert_voc2voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     6204 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/maker/convert_voc2yolo.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3508 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/maker/convert_yolo2voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1651 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/maker/maker_labelme.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    17365 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/maker/maker_voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/maker/__init__.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/pybaseutils/metrics/
--rwxrwxrwx   0 dm        (1000) dm        (1000)      795 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/metrics/accuracy.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2191 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/metrics/average_meter.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5895 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/metrics/class_report.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5576 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/metrics/plot_pr.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5375 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/metrics/plot_roc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/metrics/__init__.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    19288 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/numpy_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2090 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/pandas_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7522 2023-05-26 03:47:33.000000 pybaseutils-0.8.1/pybaseutils/plot_utils.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/pybaseutils/pycpp/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1337 2022-10-26 09:40:02.000000 pybaseutils-0.8.1/pybaseutils/pycpp/demo.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4309 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/pycpp/main.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)        0 2022-10-25 08:09:00.000000 pybaseutils-0.8.1/pybaseutils/pycpp/__init__.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5027 2022-10-20 02:03:17.000000 pybaseutils-0.8.1/pybaseutils/setup_config.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7283 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/thread_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3306 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/time_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4985 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/tracemalloc_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4239 2023-02-24 10:15:12.000000 pybaseutils-0.8.1/pybaseutils/tracemalloc_utils2.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/pybaseutils/transforms/
--rwxrwxrwx   0 dm        (1000) dm        (1000)    24116 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/transforms/affine_transform.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/transforms/__init__.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    13662 2023-05-30 01:11:50.000000 pybaseutils-0.8.1/pybaseutils/word_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4090 2023-05-25 05:47:07.000000 pybaseutils-0.8.1/pybaseutils/worker.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1141 2020-04-15 02:17:42.000000 pybaseutils-0.8.1/pybaseutils/yaml_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      137 2023-05-31 02:57:56.000000 pybaseutils-0.8.1/pybaseutils/__init__.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/pybaseutils.egg-info/
--rwxrwxrwx   0 dm        (1000) dm        (1000)        1 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/pybaseutils.egg-info/dependency_links.txt
--rwxrwxrwx   0 dm        (1000) dm        (1000)        1 2022-04-01 01:42:31.000000 pybaseutils-0.8.1/pybaseutils.egg-info/not-zip-safe
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3952 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/pybaseutils.egg-info/PKG-INFO
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3460 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/pybaseutils.egg-info/SOURCES.txt
--rwxrwxrwx   0 dm        (1000) dm        (1000)       20 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/pybaseutils.egg-info/top_level.txt
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3374 2023-03-01 06:33:08.000000 pybaseutils-0.8.1/README.md
--rwxrwxrwx   0 dm        (1000) dm        (1000)       38 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/setup.cfg
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2213 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/setup.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/test_py/
--rwxrwxrwx   0 dm        (1000) dm        (1000)      790 2023-04-06 03:02:23.000000 pybaseutils-0.8.1/test_py/class_names.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/test_py/converter/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4473 2023-03-14 07:41:09.000000 pybaseutils-0.8.1/test_py/converter/AffectNet.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3472 2023-03-11 01:43:26.000000 pybaseutils-0.8.1/test_py/converter/AsianMovie.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3693 2022-12-13 08:38:36.000000 pybaseutils-0.8.1/test_py/converter/BITVehicle2voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4577 2022-12-13 08:38:36.000000 pybaseutils-0.8.1/test_py/converter/BSTLD2voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5580 2023-01-18 07:11:31.000000 pybaseutils-0.8.1/test_py/converter/CCPD.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7024 2023-01-18 07:11:16.000000 pybaseutils-0.8.1/test_py/converter/CCPD2voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1203 2023-04-12 08:06:30.000000 pybaseutils-0.8.1/test_py/converter/insects_for_aichallenger.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2568 2023-04-10 08:35:17.000000 pybaseutils-0.8.1/test_py/converter/TT100K.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     8806 2023-04-10 06:56:11.000000 pybaseutils-0.8.1/test_py/converter/tt100k_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7592 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/test_py/converter/ua_detrac2voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/test_py/converter/__init__.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1733 2023-05-11 03:26:39.000000 pybaseutils-0.8.1/test_py/demo1.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1189 2023-05-30 10:27:09.000000 pybaseutils-0.8.1/test_py/demo2.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      204 2023-05-25 03:47:34.000000 pybaseutils-0.8.1/test_py/demo_async_await1.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1194 2023-05-25 05:49:48.000000 pybaseutils-0.8.1/test_py/demo_async_await2.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4533 2023-04-15 03:49:32.000000 pybaseutils-0.8.1/test_py/demo_copy_files.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2132 2023-02-27 02:15:50.000000 pybaseutils-0.8.1/test_py/demo_copy_files_for_voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1342 2023-05-16 02:22:22.000000 pybaseutils-0.8.1/test_py/demo_ffmpy.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      174 2022-12-23 02:56:57.000000 pybaseutils-0.8.1/test_py/demo_for_trt.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2877 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/test_py/demo_get_file_list.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      667 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/test_py/demo_gif.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1745 2023-05-24 03:16:30.000000 pybaseutils-0.8.1/test_py/demo_gif_video.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2639 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/test_py/demo_metrics.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1675 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/test_py/demo_mouse.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2085 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/test_py/demo_pandas.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      731 2023-01-13 09:22:52.000000 pybaseutils-0.8.1/test_py/demo_plot.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1124 2023-03-28 00:52:07.000000 pybaseutils-0.8.1/test_py/demo_standard_image .py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      863 2023-04-19 10:05:09.000000 pybaseutils-0.8.1/test_py/demo_standard_video .py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      749 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/test_py/demo_taichi.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      669 2023-04-23 09:10:41.000000 pybaseutils-0.8.1/test_py/demo_video.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3267 2023-04-19 06:55:52.000000 pybaseutils-0.8.1/test_py/demo_voc_crop.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2374 2023-04-18 03:49:38.000000 pybaseutils-0.8.1/test_py/demo_voc_vis.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1323 2023-04-06 02:34:20.000000 pybaseutils-0.8.1/test_py/demo_word_similar.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2906 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/test_py/demo_worker1.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3151 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/test_py/demo_worker2.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/test_py/detector/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     6671 2023-05-04 08:11:18.000000 pybaseutils-0.8.1/test_py/detector/detect_face_person.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      130 2023-04-23 10:06:32.000000 pybaseutils-0.8.1/test_py/detector/__init__.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/test_py/flask_demo/
--rwxrwxrwx   0 dm        (1000) dm        (1000)      386 2023-05-16 00:55:43.000000 pybaseutils-0.8.1/test_py/flask_demo/func.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      990 2023-05-16 01:11:46.000000 pybaseutils-0.8.1/test_py/flask_demo/server.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      109 2023-05-16 00:53:07.000000 pybaseutils-0.8.1/test_py/flask_demo/__init__.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/test_py/image_correction/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7370 2022-11-26 02:52:34.000000 pybaseutils-0.8.1/test_py/image_correction/demo_correction_v1.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5657 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/test_py/image_correction/demo_correction_v2.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1558 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/test_py/image_correction/demo_correction_v3.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      130 2023-04-23 09:02:28.000000 pybaseutils-0.8.1/test_py/image_correction/__init__.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      575 2023-05-24 09:15:25.000000 pybaseutils-0.8.1/test_py/kafka_worker.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      665 2023-02-27 08:49:34.000000 pybaseutils-0.8.1/test_py/men_tracemalloc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2222 2023-01-05 06:46:58.000000 pybaseutils-0.8.1/test_py/performance.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/test_py/__init__.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1073 2021-12-28 07:55:19.000000 pybaseutils-0.8.2/LICENCE
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     3952 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/PKG-INFO
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/pybaseutils/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     5094 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/base64_utils.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/pybaseutils/base_audio/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     4792 2023-05-16 07:29:26.000000 pybaseutils-0.8.2/pybaseutils/base_audio/audio_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      109 2023-05-11 02:35:54.000000 pybaseutils-0.8.2/pybaseutils/base_audio/__init__.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2155 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/batch_utils.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/pybaseutils/cluster/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1952 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/cluster/kmean.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     3038 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/cluster/maxmin_distance.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2744 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/cluster/similarity.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/cluster/__init__.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     7049 2022-11-16 02:12:19.000000 pybaseutils-0.8.2/pybaseutils/color_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     5027 2022-06-14 03:12:10.000000 pybaseutils-0.8.2/pybaseutils/config_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)    10076 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/coords_utils.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/pybaseutils/cvutils/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     7528 2022-11-25 09:29:09.000000 pybaseutils-0.8.2/pybaseutils/cvutils/corner_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     6101 2023-06-01 06:52:32.000000 pybaseutils-0.8.2/pybaseutils/cvutils/monitor.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     8265 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/cvutils/mouse_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     9695 2023-06-01 07:00:45.000000 pybaseutils-0.8.2/pybaseutils/cvutils/video_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      130 2022-11-25 02:19:14.000000 pybaseutils-0.8.2/pybaseutils/cvutils/__init__.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/pybaseutils/dataloader/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     7363 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/dataloader/dataset.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)    12136 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/dataloader/parser_labelme.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)    11897 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/dataloader/parser_textdata.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)    19470 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/dataloader/parser_voc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/dataloader/__init__.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)    32583 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/file_utils.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/pybaseutils/font_style/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      537 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/font_style/__init__.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     7786 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/font_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)    13053 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/geometry_tools.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     5306 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/heatmap_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)    97190 2023-06-02 01:38:12.000000 pybaseutils-0.8.2/pybaseutils/image_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     4255 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/json_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     6813 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/log.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1874 2022-10-10 02:04:07.000000 pybaseutils-0.8.2/pybaseutils/logger.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/pybaseutils/maker/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     4645 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/maker/convert_labelme2voc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     4366 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/maker/convert_voc2voc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     6204 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/maker/convert_voc2yolo.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     3508 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/maker/convert_yolo2voc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1651 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/maker/maker_labelme.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)    17365 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/maker/maker_voc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/maker/__init__.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/pybaseutils/metrics/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      795 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/metrics/accuracy.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2191 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/metrics/average_meter.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     5895 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/metrics/class_report.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     5576 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/metrics/plot_pr.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     5375 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/metrics/plot_roc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/metrics/__init__.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)    19288 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/numpy_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2090 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/pandas_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     7522 2023-05-26 03:47:33.000000 pybaseutils-0.8.2/pybaseutils/plot_utils.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/pybaseutils/pycpp/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1337 2022-10-26 09:40:02.000000 pybaseutils-0.8.2/pybaseutils/pycpp/demo.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     4309 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/pycpp/main.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)        0 2022-10-25 08:09:00.000000 pybaseutils-0.8.2/pybaseutils/pycpp/__init__.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     5027 2022-10-20 02:03:17.000000 pybaseutils-0.8.2/pybaseutils/setup_config.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     7283 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/thread_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     3306 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/time_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     4985 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/tracemalloc_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     4239 2023-02-24 10:15:12.000000 pybaseutils-0.8.2/pybaseutils/tracemalloc_utils2.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/pybaseutils/transforms/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)    24116 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/pybaseutils/transforms/affine_transform.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/pybaseutils/transforms/__init__.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)    13662 2023-05-30 01:11:50.000000 pybaseutils-0.8.2/pybaseutils/word_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     4090 2023-05-25 05:47:07.000000 pybaseutils-0.8.2/pybaseutils/worker.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1141 2020-04-15 02:17:42.000000 pybaseutils-0.8.2/pybaseutils/yaml_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      137 2023-06-02 01:38:30.000000 pybaseutils-0.8.2/pybaseutils/__init__.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/pybaseutils.egg-info/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)        1 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/pybaseutils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dm        (1000) dm        (1000)        1 2022-04-01 01:42:31.000000 pybaseutils-0.8.2/pybaseutils.egg-info/not-zip-safe
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     3952 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/pybaseutils.egg-info/PKG-INFO
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     3491 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/pybaseutils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dm        (1000) dm        (1000)       20 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/pybaseutils.egg-info/top_level.txt
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     3374 2023-03-01 06:33:08.000000 pybaseutils-0.8.2/README.md
+-rwxrwxrwx   0 dm        (1000) dm        (1000)       38 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/setup.cfg
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2213 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/setup.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/test_py/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      790 2023-04-06 03:02:23.000000 pybaseutils-0.8.2/test_py/class_names.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/test_py/converter/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     4473 2023-03-14 07:41:09.000000 pybaseutils-0.8.2/test_py/converter/AffectNet.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     3472 2023-03-11 01:43:26.000000 pybaseutils-0.8.2/test_py/converter/AsianMovie.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     3693 2022-12-13 08:38:36.000000 pybaseutils-0.8.2/test_py/converter/BITVehicle2voc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     4577 2022-12-13 08:38:36.000000 pybaseutils-0.8.2/test_py/converter/BSTLD2voc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     5580 2023-01-18 07:11:31.000000 pybaseutils-0.8.2/test_py/converter/CCPD.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     7024 2023-01-18 07:11:16.000000 pybaseutils-0.8.2/test_py/converter/CCPD2voc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1203 2023-04-12 08:06:30.000000 pybaseutils-0.8.2/test_py/converter/insects_for_aichallenger.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2568 2023-04-10 08:35:17.000000 pybaseutils-0.8.2/test_py/converter/TT100K.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     8806 2023-04-10 06:56:11.000000 pybaseutils-0.8.2/test_py/converter/tt100k_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     7592 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/test_py/converter/ua_detrac2voc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/test_py/converter/__init__.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1733 2023-05-11 03:26:39.000000 pybaseutils-0.8.2/test_py/demo1.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1189 2023-05-30 10:27:09.000000 pybaseutils-0.8.2/test_py/demo2.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      204 2023-05-25 03:47:34.000000 pybaseutils-0.8.2/test_py/demo_async_await1.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1194 2023-05-25 05:49:48.000000 pybaseutils-0.8.2/test_py/demo_async_await2.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     4664 2023-06-01 07:22:44.000000 pybaseutils-0.8.2/test_py/demo_copy_files.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2132 2023-02-27 02:15:50.000000 pybaseutils-0.8.2/test_py/demo_copy_files_for_voc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1342 2023-05-16 02:22:22.000000 pybaseutils-0.8.2/test_py/demo_ffmpy.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      174 2022-12-23 02:56:57.000000 pybaseutils-0.8.2/test_py/demo_for_trt.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2877 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/test_py/demo_get_file_list.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      667 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/test_py/demo_gif.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1745 2023-05-24 03:16:30.000000 pybaseutils-0.8.2/test_py/demo_gif_video.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2639 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/test_py/demo_metrics.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1675 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/test_py/demo_mouse.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2085 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/test_py/demo_pandas.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      731 2023-01-13 09:22:52.000000 pybaseutils-0.8.2/test_py/demo_plot.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1124 2023-03-28 00:52:07.000000 pybaseutils-0.8.2/test_py/demo_standard_image .py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      863 2023-04-19 10:05:09.000000 pybaseutils-0.8.2/test_py/demo_standard_video .py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      749 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/test_py/demo_taichi.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      778 2023-06-01 07:11:31.000000 pybaseutils-0.8.2/test_py/demo_video.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     3267 2023-04-19 06:55:52.000000 pybaseutils-0.8.2/test_py/demo_voc_crop.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2374 2023-04-18 03:49:38.000000 pybaseutils-0.8.2/test_py/demo_voc_vis.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1323 2023-04-06 02:34:20.000000 pybaseutils-0.8.2/test_py/demo_word_similar.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2906 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/test_py/demo_worker1.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     3151 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/test_py/demo_worker2.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/test_py/detector/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     6671 2023-05-04 08:11:18.000000 pybaseutils-0.8.2/test_py/detector/detect_face_person.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      130 2023-04-23 10:06:32.000000 pybaseutils-0.8.2/test_py/detector/__init__.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/test_py/flask_demo/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      386 2023-05-16 00:55:43.000000 pybaseutils-0.8.2/test_py/flask_demo/func.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      990 2023-05-16 01:11:46.000000 pybaseutils-0.8.2/test_py/flask_demo/server.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      109 2023-05-16 00:53:07.000000 pybaseutils-0.8.2/test_py/flask_demo/__init__.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-06-02 01:38:34.000000 pybaseutils-0.8.2/test_py/image_correction/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     7370 2022-11-26 02:52:34.000000 pybaseutils-0.8.2/test_py/image_correction/demo_correction_v1.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     5657 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/test_py/image_correction/demo_correction_v2.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1558 2023-04-19 09:05:26.000000 pybaseutils-0.8.2/test_py/image_correction/demo_correction_v3.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      130 2023-04-23 09:02:28.000000 pybaseutils-0.8.2/test_py/image_correction/__init__.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      575 2023-05-24 09:15:25.000000 pybaseutils-0.8.2/test_py/kafka_worker.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      665 2023-02-27 08:49:34.000000 pybaseutils-0.8.2/test_py/men_tracemalloc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2222 2023-01-05 06:46:58.000000 pybaseutils-0.8.2/test_py/performance.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.2/test_py/__init__.py
```

### Comparing `pybaseutils-0.8.1/LICENCE` & `pybaseutils-0.8.2/LICENCE`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/PKG-INFO` & `pybaseutils-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybaseutils
-Version: 0.8.1
+Version: 0.8.2
 Summary: pybaseutils
 Home-page: https://github.com/PanJinquan/base-utils
 Author: PanJinquan
 Author-email: 390737991@qq.com
 License: MIT
 Platform: UNKNOWN
 License-File: LICENCE
```

### Comparing `pybaseutils-0.8.1/pybaseutils/base64_utils.py` & `pybaseutils-0.8.2/pybaseutils/base64_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/base_audio/audio_utils.py` & `pybaseutils-0.8.2/pybaseutils/base_audio/audio_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/batch_utils.py` & `pybaseutils-0.8.2/pybaseutils/batch_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/cluster/kmean.py` & `pybaseutils-0.8.2/pybaseutils/cluster/kmean.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/cluster/maxmin_distance.py` & `pybaseutils-0.8.2/pybaseutils/cluster/maxmin_distance.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/cluster/similarity.py` & `pybaseutils-0.8.2/pybaseutils/cluster/similarity.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/color_utils.py` & `pybaseutils-0.8.2/pybaseutils/color_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/config_utils.py` & `pybaseutils-0.8.2/pybaseutils/config_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/coords_utils.py` & `pybaseutils-0.8.2/pybaseutils/coords_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/cvutils/corner_utils.py` & `pybaseutils-0.8.2/pybaseutils/cvutils/corner_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/cvutils/mouse_utils.py` & `pybaseutils-0.8.2/pybaseutils/cvutils/mouse_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/cvutils/video_utils.py` & `pybaseutils-0.8.2/pybaseutils/cvutils/video_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     @Brief  :
 """
 import os
 import cv2
 import numpy as np
 from tqdm import tqdm
 from pybaseutils import image_utils, file_utils
+from pybaseutils.cvutils import monitor
 
 VIDEO_POSTFIX = ['*.mp4', '*.avi']
 
 get_video_capture = image_utils.get_video_capture
 get_video_info = image_utils.get_video_info
 get_video_writer = image_utils.get_video_writer
 
@@ -89,14 +90,57 @@
             frame_file = os.path.join(out_dir, "{}_{:0=4d}.jpg".format(name, count))
             cv2.imwrite(frame_file, frame)
         count += 1
     video_cap.release()
     cv2.destroyAllWindows()
 
 
+def video2frames_similarity(video_file, out_dir=None, func=None, interval=1, thresh=0.3, vis=True):
+    """
+    视频抽帧图像
+    :param video_file: 视频文件
+    :param out_dir: 保存抽帧图像的目录
+    :param func: 回调函数，对每一帧图像进行处理
+    :param interval: 保存间隔
+    :param vis: 是否可视化显示
+    :return:
+    """
+    sm = monitor.StatusMonitor()
+    name = os.path.basename(video_file).split(".")[0]
+    if not out_dir:  out_dir = os.path.join(os.path.dirname(video_file), name)
+    video_cap = get_video_capture(video_file)
+    width, height, num_frames, fps = get_video_info(video_cap)
+    if not os.path.exists(out_dir): os.makedirs(out_dir)
+    count = 0
+    last_frame = None
+    while count < num_frames:
+        if count % interval == 0:
+            # 设置抽帧的位置
+            video_cap.set(cv2.CAP_PROP_POS_FRAMES, count)
+            isSuccess, curr_frame = video_cap.read()
+            if not isSuccess:
+                break
+            if func: curr_frame = func(curr_frame)
+            if last_frame is None:
+                last_frame = curr_frame.copy()
+            diff = sm.get_frame_similarity(curr_frame, last_frame, size=(256, 256), vis=False)
+            if diff > thresh:
+                frame_file = os.path.join(out_dir, "{}_{:0=4d}.jpg".format(name, count))
+                last_frame = curr_frame.copy()
+                cv2.imwrite(frame_file, curr_frame)
+            if vis:
+                text = "TH={},diff={:3.3f}".format(thresh, diff)
+                image = image_utils.draw_text(curr_frame, point=(10, 70), color=(0, 255, 0),
+                                              text=text, drawType="simple")
+                image = image_utils.cv_show_image("image", image, delay=10)
+        count += 1
+    video_cap.release()
+    cv2.destroyAllWindows()
+
+
 def frames2video(image_dir, video_file=None, func=None, size=None, postfix=["*.png", "*.jpg"], interval=1, fps=30,
                  vis=True):
     """
     将抽帧图像转为视频文件(*.mp4)
     :param image_dir:抽帧图像路径
     :param video_file: 保存的视频文件
     :param func: 回调函数，对每一帧图像进行处理
```

### Comparing `pybaseutils-0.8.1/pybaseutils/dataloader/dataset.py` & `pybaseutils-0.8.2/pybaseutils/dataloader/dataset.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/dataloader/parser_labelme.py` & `pybaseutils-0.8.2/pybaseutils/dataloader/parser_labelme.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/dataloader/parser_textdata.py` & `pybaseutils-0.8.2/pybaseutils/dataloader/parser_textdata.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/dataloader/parser_voc.py` & `pybaseutils-0.8.2/pybaseutils/dataloader/parser_voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/file_utils.py` & `pybaseutils-0.8.2/pybaseutils/file_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/font_style/__init__.py` & `pybaseutils-0.8.2/pybaseutils/font_style/__init__.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/font_utils.py` & `pybaseutils-0.8.2/pybaseutils/font_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/geometry_tools.py` & `pybaseutils-0.8.2/pybaseutils/geometry_tools.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/heatmap_utils.py` & `pybaseutils-0.8.2/pybaseutils/heatmap_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/image_utils.py` & `pybaseutils-0.8.2/pybaseutils/image_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,20 +21,20 @@
 from typing import List, Dict, Tuple
 from PIL import ImageDraw, ImageFont
 from math import cos, sin
 from pybaseutils import file_utils
 from pybaseutils.coords_utils import *
 from pybaseutils.transforms import affine_transform
 
-color_map2 = [(0, 0, 0), (0, 0, 255), (0, 255, 0), (255, 0, 0),
-              (128, 0, 0), (0, 128, 0), (128, 128, 0),
-              (0, 0, 128), (128, 0, 128), (0, 128, 128), (128, 128, 128),
-              (64, 0, 0), (192, 0, 0), (64, 128, 0), (192, 128, 0),
-              (64, 0, 128), (192, 0, 128), (64, 128, 128), (192, 128, 128),
-              (0, 64, 0), (128, 64, 0), (0, 192, 0), (128, 192, 0), (0, 64, 128)] * 100
+color_table = [(0, 0, 0), (0, 0, 255), (0, 255, 0), (255, 0, 0),
+               (128, 0, 0), (0, 128, 0), (128, 128, 0),
+               (0, 0, 128), (128, 0, 128), (0, 128, 128), (128, 128, 128),
+               (64, 0, 0), (192, 0, 0), (64, 128, 0), (192, 128, 0),
+               (64, 0, 128), (192, 0, 128), (64, 128, 128), (192, 128, 128),
+               (0, 64, 0), (128, 64, 0), (0, 192, 0), (128, 192, 0), (0, 64, 128)] * 100
 
 color_map = [(0, 0, 0), (56, 56, 255), (151, 157, 255), (31, 112, 255), (29, 178, 255), (49, 210, 207),
              (10, 249, 72), (23, 204, 146), (134, 219, 61), (52, 147, 26), (187, 212, 0),
              (168, 153, 44), (255, 194, 0), (147, 69, 52), (255, 115, 100),
              (236, 24, 0), (255, 56, 132), (133, 0, 82), (255, 56, 203), (200, 149, 255), (199, 55, 255)] * 100
 
 root = os.path.dirname(__file__)
@@ -1307,25 +1307,25 @@
     :param drawType: custom or simple
     :return:
     """
     thickness, fontScale = get_linesize(max(image.shape), thickness=thickness, fontScale=fontScale)
     text_thickness = 1
     fontFace = cv2.FONT_HERSHEY_SIMPLEX
     # fontFace=cv2.FONT_HERSHEY_SIMPLEX
-    if drawType == "custom":
+    if drawType == "custom" or drawType == "en":
         text_size, baseline = cv2.getTextSize(str(text), fontFace, fontScale, thickness)
         text_loc = (point[0], point[1] + text_size[1])
         cv2.rectangle(image, (text_loc[0] - 2 // 2, text_loc[1] - 2 - baseline),
                       (text_loc[0] + text_size[0], text_loc[1] + text_size[1]), color=color, thickness=thickness)
         # draw score value
         cv2.putText(image, str(text), (text_loc[0], text_loc[1] + baseline), fontFace, fontScale,
                     (255, 255, 255), text_thickness, 2)
     elif drawType == "simple":
         cv2.putText(image, str(text), point, fontFace, fontScale, color=color, thickness=thickness)
-    if drawType == "chinese":
+    if drawType == "chinese" or drawType == "ch":
         cv2_putText(image, str(text), point, fontFace, fontScale, color=color, thickness=thickness)
     return image
 
 
 def draw_text_line(image, point, text_line: str, bg_color=(255, 0, 0), thickness=-1, fontScale=-1.0, drawType="custom"):
     """
     :param image:
```

### Comparing `pybaseutils-0.8.1/pybaseutils/json_utils.py` & `pybaseutils-0.8.2/pybaseutils/json_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/log.py` & `pybaseutils-0.8.2/pybaseutils/log.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/logger.py` & `pybaseutils-0.8.2/pybaseutils/logger.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/maker/convert_labelme2voc.py` & `pybaseutils-0.8.2/pybaseutils/maker/convert_labelme2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/maker/convert_voc2voc.py` & `pybaseutils-0.8.2/pybaseutils/maker/convert_voc2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/maker/convert_voc2yolo.py` & `pybaseutils-0.8.2/pybaseutils/maker/convert_voc2yolo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/maker/convert_yolo2voc.py` & `pybaseutils-0.8.2/pybaseutils/maker/convert_yolo2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/maker/maker_labelme.py` & `pybaseutils-0.8.2/pybaseutils/maker/maker_labelme.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/maker/maker_voc.py` & `pybaseutils-0.8.2/pybaseutils/maker/maker_voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/metrics/accuracy.py` & `pybaseutils-0.8.2/pybaseutils/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/metrics/average_meter.py` & `pybaseutils-0.8.2/pybaseutils/metrics/average_meter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/metrics/class_report.py` & `pybaseutils-0.8.2/pybaseutils/metrics/class_report.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/metrics/plot_pr.py` & `pybaseutils-0.8.2/pybaseutils/metrics/plot_pr.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/metrics/plot_roc.py` & `pybaseutils-0.8.2/pybaseutils/metrics/plot_roc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/numpy_utils.py` & `pybaseutils-0.8.2/pybaseutils/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/pandas_utils.py` & `pybaseutils-0.8.2/pybaseutils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/plot_utils.py` & `pybaseutils-0.8.2/pybaseutils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/pycpp/demo.py` & `pybaseutils-0.8.2/pybaseutils/pycpp/demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/pycpp/main.py` & `pybaseutils-0.8.2/pybaseutils/pycpp/main.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/setup_config.py` & `pybaseutils-0.8.2/pybaseutils/setup_config.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/thread_utils.py` & `pybaseutils-0.8.2/pybaseutils/thread_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/time_utils.py` & `pybaseutils-0.8.2/pybaseutils/time_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/tracemalloc_utils.py` & `pybaseutils-0.8.2/pybaseutils/tracemalloc_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/tracemalloc_utils2.py` & `pybaseutils-0.8.2/pybaseutils/tracemalloc_utils2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/transforms/affine_transform.py` & `pybaseutils-0.8.2/pybaseutils/transforms/affine_transform.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/word_utils.py` & `pybaseutils-0.8.2/pybaseutils/word_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/worker.py` & `pybaseutils-0.8.2/pybaseutils/worker.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils/yaml_utils.py` & `pybaseutils-0.8.2/pybaseutils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/pybaseutils.egg-info/PKG-INFO` & `pybaseutils-0.8.2/pybaseutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybaseutils
-Version: 0.8.1
+Version: 0.8.2
 Summary: pybaseutils
 Home-page: https://github.com/PanJinquan/base-utils
 Author: PanJinquan
 Author-email: 390737991@qq.com
 License: MIT
 Platform: UNKNOWN
 License-File: LICENCE
```

### Comparing `pybaseutils-0.8.1/pybaseutils.egg-info/SOURCES.txt` & `pybaseutils-0.8.2/pybaseutils.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 pybaseutils/base_audio/audio_utils.py
 pybaseutils/cluster/__init__.py
 pybaseutils/cluster/kmean.py
 pybaseutils/cluster/maxmin_distance.py
 pybaseutils/cluster/similarity.py
 pybaseutils/cvutils/__init__.py
 pybaseutils/cvutils/corner_utils.py
+pybaseutils/cvutils/monitor.py
 pybaseutils/cvutils/mouse_utils.py
 pybaseutils/cvutils/video_utils.py
 pybaseutils/dataloader/__init__.py
 pybaseutils/dataloader/dataset.py
 pybaseutils/dataloader/parser_labelme.py
 pybaseutils/dataloader/parser_textdata.py
 pybaseutils/dataloader/parser_voc.py
```

### Comparing `pybaseutils-0.8.1/README.md` & `pybaseutils-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/setup.py` & `pybaseutils-0.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/class_names.py` & `pybaseutils-0.8.2/test_py/class_names.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/converter/AffectNet.py` & `pybaseutils-0.8.2/test_py/converter/AffectNet.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/converter/AsianMovie.py` & `pybaseutils-0.8.2/test_py/converter/AsianMovie.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/converter/BITVehicle2voc.py` & `pybaseutils-0.8.2/test_py/converter/BITVehicle2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/converter/BSTLD2voc.py` & `pybaseutils-0.8.2/test_py/converter/BSTLD2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/converter/CCPD.py` & `pybaseutils-0.8.2/test_py/converter/CCPD.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/converter/CCPD2voc.py` & `pybaseutils-0.8.2/test_py/converter/CCPD2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/converter/insects_for_aichallenger.py` & `pybaseutils-0.8.2/test_py/converter/insects_for_aichallenger.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/converter/TT100K.py` & `pybaseutils-0.8.2/test_py/converter/TT100K.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/converter/tt100k_utils.py` & `pybaseutils-0.8.2/test_py/converter/tt100k_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/converter/ua_detrac2voc.py` & `pybaseutils-0.8.2/test_py/converter/ua_detrac2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/demo1.py` & `pybaseutils-0.8.2/test_py/demo1.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/demo2.py` & `pybaseutils-0.8.2/test_py/demo2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/demo_async_await2.py` & `pybaseutils-0.8.2/test_py/demo_async_await2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/demo_copy_files.py` & `pybaseutils-0.8.2/test_py/demo_copy_files.py`

 * *Files 11% similar despite different names*

```diff
@@ -56,17 +56,17 @@
     image_dir = "/home/dm/nasdata/dataset/tmp/Medicine/dataset/train"
     out_dir = "/home/dm/nasdata/dataset/tmp/Medicine/dataset/test"
     # file_utils.copy_move_dir_dir(image_dir, out_dir, sub_names=sub_names, per_nums=10, shuffle=True, move=True)
     file_utils.copy_move_file_dir(image_dir, out_dir, sub_names=None, max_nums=10000, move=True, shuffle=True)
 
 
 def demo_copy_move():
-    image_dir = "/home/dm/nasdata/dataset/tmp/Medicine/dataset1/train"
-    out_dir = "/home/dm/nasdata/dataset/tmp/Medicine/dataset1/test"
-    file_utils.copy_move_file_dir(image_dir, out_dir, sub_names=None, max_nums=7000, move=True, shuffle=True)
+    image_dir = "/home/dm/nasdata/dataset-dmai/handwriting/grid-det/grid_cross_points_images/grid_cross_points_v7/儿童C组"
+    out_dir = "/home/dm/nasdata/dataset-dmai/handwriting/grid-det/grid_cross_points_images/grid_cross_points_v7/images"
+    file_utils.copy_move_file_dir(image_dir, out_dir, sub_names=None, max_nums=1000, move=False, shuffle=True)
 
 
 def copy_files(shuffle=False):
     root = "/home/dm/nasdata/dataset/tmp/fall/Fall-detection-Dataset/train"
     out = "/home/dm/nasdata/dataset/tmp/fall/fall-v3"
     sub_list = file_utils.get_sub_paths(root)
     phase = os.path.basename(root)
@@ -95,8 +95,9 @@
 
 if __name__ == "__main__":
     # demo_copy_move()
     # demo_copy_move_by_sub_names_v1()
     # demo_copy_move_by_sub_names_v2()
     # demo_copy_move_by_sub_names_v2()
     # demo_copy_move_by_sub_names_v3()
-    copy_files()
+    # copy_files()
+    demo_copy_move()
```

### Comparing `pybaseutils-0.8.1/test_py/demo_copy_files_for_voc.py` & `pybaseutils-0.8.2/test_py/demo_copy_files_for_voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/demo_ffmpy.py` & `pybaseutils-0.8.2/test_py/demo_ffmpy.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/demo_get_file_list.py` & `pybaseutils-0.8.2/test_py/demo_get_file_list.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/demo_gif.py` & `pybaseutils-0.8.2/test_py/demo_gif.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/demo_gif_video.py` & `pybaseutils-0.8.2/test_py/demo_gif_video.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/demo_metrics.py` & `pybaseutils-0.8.2/test_py/demo_metrics.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/demo_mouse.py` & `pybaseutils-0.8.2/test_py/demo_mouse.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/demo_pandas.py` & `pybaseutils-0.8.2/test_py/demo_pandas.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/demo_plot.py` & `pybaseutils-0.8.2/test_py/demo_plot.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/demo_standard_image .py` & `pybaseutils-0.8.2/test_py/demo_standard_image .py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/demo_standard_video .py` & `pybaseutils-0.8.2/test_py/demo_standard_video .py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/demo_taichi.py` & `pybaseutils-0.8.2/test_py/demo_taichi.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/demo_video.py` & `pybaseutils-0.8.2/test_py/demo_video.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from pybaseutils.cvutils import video_utils
 
 
 def video2frames_demo(root, out):
     files = file_utils.get_files_list(root, postfix=["*.avi", "*.mp4"])
     for video_file in files:
         print(video_file)
-        video_utils.video2frames(video_file, out_dir=out, func=None, interval=20, vis=True)
+        video_utils.video2frames_similarity(video_file, out_dir=out, func=None, interval=50, vis=True)
+        # video_utils.video2frames(video_file, out_dir=out, func=None, interval=50, vis=True)
 
 
 if __name__ == "__main__":
-    root = "/home/dm/nasdata/dataset/tmp/smoking/videos/video1"
+    root = "/home/dm/nasdata/release/CSG/南方电网视频/videos"
     out = root + "-frame"
     video2frames_demo(root, out)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pybaseutils-0.8.1/test_py/demo_voc_crop.py` & `pybaseutils-0.8.2/test_py/demo_voc_crop.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/demo_voc_vis.py` & `pybaseutils-0.8.2/test_py/demo_voc_vis.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/demo_word_similar.py` & `pybaseutils-0.8.2/test_py/demo_word_similar.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/demo_worker1.py` & `pybaseutils-0.8.2/test_py/demo_worker1.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/demo_worker2.py` & `pybaseutils-0.8.2/test_py/demo_worker2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/detector/detect_face_person.py` & `pybaseutils-0.8.2/test_py/detector/detect_face_person.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/flask_demo/server.py` & `pybaseutils-0.8.2/test_py/flask_demo/server.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/image_correction/demo_correction_v1.py` & `pybaseutils-0.8.2/test_py/image_correction/demo_correction_v1.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/image_correction/demo_correction_v2.py` & `pybaseutils-0.8.2/test_py/image_correction/demo_correction_v2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/image_correction/demo_correction_v3.py` & `pybaseutils-0.8.2/test_py/image_correction/demo_correction_v3.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/kafka_worker.py` & `pybaseutils-0.8.2/test_py/kafka_worker.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/men_tracemalloc.py` & `pybaseutils-0.8.2/test_py/men_tracemalloc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.1/test_py/performance.py` & `pybaseutils-0.8.2/test_py/performance.py`

 * *Files identical despite different names*

