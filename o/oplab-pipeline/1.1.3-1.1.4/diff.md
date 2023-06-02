# Comparing `tmp/oplab_pipeline-1.1.3.tar.gz` & `tmp/oplab_pipeline-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oplab_pipeline-1.1.3.tar", last modified: Tue Apr 25 16:16:41 2023, max compression
+gzip compressed data, was "oplab_pipeline-1.1.4.tar", last modified: Fri Jun  2 13:59:51 2023, max compression
```

## Comparing `oplab_pipeline-1.1.3.tar` & `oplab_pipeline-1.1.4.tar`

### file list

```diff
@@ -1,221 +1,221 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.880731 oplab_pipeline-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    20848 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-04-25 16:16:41.880731 oplab_pipeline-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 16:16:41.880731 oplab_pipeline-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.864730 oplab_pipeline-1.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.864730 oplab_pipeline-1.1.3/src/auv_cal/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_cal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_cal/auv_cal.py
--rw-r--r--   0 runner    (1001) docker     (123)    25715 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_cal/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)    57980 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_cal/camera_calibrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_cal/cone_fitting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.864730 oplab_pipeline-1.1.3/src/auv_cal/default_yaml/
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_cal/default_yaml/default_calibration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_cal/euler_angles_from_rotation_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    41020 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_cal/laser_calibrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_cal/plane_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_cal/plot_points_and_planes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_cal/ransac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.864730 oplab_pipeline-1.1.3/src/auv_nav/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10343 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/auv_nav.py
--rw-r--r--   0 runner    (1001) docker     (123)    14771 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.864730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.860730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ae2000/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.864730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ae2000/YK17-23C/
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ae2000/YK17-23C/camera.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ae2000/YK17-23C/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ae2000/YK17-23C/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.860730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/alr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.864730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/alr/dy152/
--rwxr-xr-x   0 runner    (1001) docker     (123)      444 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/alr/dy152/camera.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1468 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/alr/dy152/mission.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1736 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/alr/dy152/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.864730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/alr/insite/
--rwxr-xr-x   0 runner    (1001) docker     (123)      444 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/alr/insite/camera.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1757 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/alr/insite/mission.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1962 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/alr/insite/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.864730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/alr/jc220/
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/alr/jc220/camera.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.860730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/as6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.868730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/as6/DY109/
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/as6/DY109/camera.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/as6/DY109/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/as6/DY109/vehicle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/auv_nav.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.868730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/hybis/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/hybis/camera.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/hybis/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/hybis/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.868730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ntnu_rov/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ntnu_rov/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ntnu_rov/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.860730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ntnu_stereo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.868730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ntnu_stereo/tautra21/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ntnu_stereo/tautra21/camera.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ntnu_stereo/tautra21/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ntnu_stereo/tautra21/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.860730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/rosbag/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.868730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/rosbag/grassmap/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/rosbag/grassmap/camera.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/rosbag/grassmap/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/rosbag/grassmap/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.860730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/smarty200/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.868730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/smarty200/stereo_gopro/
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/smarty200/stereo_gopro/camera.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/smarty200/stereo_gopro/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/smarty200/stereo_gopro/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.860730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ts1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.868730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ts1/SSK17-01/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ts1/SSK17-01/camera.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ts1/SSK17-01/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ts1/SSK17-01/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.860730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ts2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.868730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ts2/SSK16-01/
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ts2/SSK16-01/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ts2/SSK16-01/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.868730 oplab_pipeline-1.1.3/src/auv_nav/localisation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/localisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/localisation/dead_reckoning.py
--rw-r--r--   0 runner    (1001) docker     (123)    43615 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/localisation/ekf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/localisation/particle.py
--rw-r--r--   0 runner    (1001) docker     (123)    31173 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/localisation/particle_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19387 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/localisation/pf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/localisation/usbl_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/localisation/usbl_offset.py
--rw-r--r--   0 runner    (1001) docker     (123)    26656 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.872731 oplab_pipeline-1.1.3/src/auv_nav/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/acfr_combined_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)    11598 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/acfr_stereo_pose.py
--rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/acfr_vehicle_pose.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/generic_csv_payload_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/hybis.py
--rw-r--r--   0 runner    (1001) docker     (123)    38968 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/koyo20rov.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/load_matlab_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_NOC_nmea.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_NOC_polpred.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_acfr_images.py
--rw-r--r--   0 runner    (1001) docker     (123)    17453 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_ae2000.py
--rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_alr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_autosub.py
--rw-r--r--   0 runner    (1001) docker     (123)    13242 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_biocam_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_eiva_navipac.py
--rw-r--r--   0 runner    (1001) docker     (123)    21692 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_gaps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_interlacer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_koyo21rov.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_ntnu_dvl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_ntnu_stereo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_phins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_rdi.py
--rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_rosbag.py
--rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_seaxerocks_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_stereo_gopro.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_tide_CTI.py
--rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_usbl_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parser_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.872731 oplab_pipeline-1.1.3/src/auv_nav/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/plot/plot_parse_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    60072 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/plot/plot_process_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    81521 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/process.py
--rw-r--r--   0 runner    (1001) docker     (123)    74413 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/sensors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.872731 oplab_pipeline-1.1.3/src/auv_nav/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/tools/body_to_inertial.py
--rw-r--r--   0 runner    (1001) docker     (123)    13377 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/tools/csv_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/tools/displayable_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/tools/dvl_level_arm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/tools/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/tools/inertial_to_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    18019 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/tools/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/tools/latlon_wgs84.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/tools/time_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)    58260 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/tools/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.872731 oplab_pipeline-1.1.3/src/correct_images/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20183 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/correct_images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.872731 oplab_pipeline-1.1.3/src/correct_images/corrections/
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/corrections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9515 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/corrections/attenuation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/corrections/debayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/corrections/gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/corrections/manual_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/corrections/pixel_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/corrections/rescale.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/corrections/undistort.py
--rw-r--r--   0 runner    (1001) docker     (123)    56562 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/corrector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.864730 oplab_pipeline-1.1.3/src/correct_images/default_yaml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.872731 oplab_pipeline-1.1.3/src/correct_images/default_yaml/acfr/
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/default_yaml/acfr/correct_images.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.872731 oplab_pipeline-1.1.3/src/correct_images/default_yaml/biocam/
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/default_yaml/biocam/correct_images.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.872731 oplab_pipeline-1.1.3/src/correct_images/default_yaml/biocam4000_15c/
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/default_yaml/biocam4000_15c/correct_images.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.872731 oplab_pipeline-1.1.3/src/correct_images/default_yaml/hybis/
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/default_yaml/hybis/correct_images.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.872731 oplab_pipeline-1.1.3/src/correct_images/default_yaml/ntnu_stereo/
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/default_yaml/ntnu_stereo/correct_images.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.876731 oplab_pipeline-1.1.3/src/correct_images/default_yaml/rosbag/
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/default_yaml/rosbag/correct_images.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.876731 oplab_pipeline-1.1.3/src/correct_images/default_yaml/stereo_gopro/
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/default_yaml/stereo_gopro/correct_images.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.876731 oplab_pipeline-1.1.3/src/correct_images/default_yaml/sx3/
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/default_yaml/sx3/correct_images.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.876731 oplab_pipeline-1.1.3/src/correct_images/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/loaders/default.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/loaders/depth_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/loaders/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/loaders/rosbag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/loaders/xviii.py
--rw-r--r--   0 runner    (1001) docker     (123)    13630 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.876731 oplab_pipeline-1.1.3/src/correct_images/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/tools/curve_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/tools/file_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/tools/joblib_tqdm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/tools/memmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/tools/numerical.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.876731 oplab_pipeline-1.1.3/src/oplab/
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/oplab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/oplab/camera_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11572 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/oplab/camera_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/oplab/console.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.864730 oplab_pipeline-1.1.3/src/oplab/default_yaml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.864730 oplab_pipeline-1.1.3/src/oplab/default_yaml/ae2000/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.876731 oplab_pipeline-1.1.3/src/oplab/default_yaml/ae2000/YK17-23C/
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/oplab/default_yaml/ae2000/YK17-23C/camera.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/oplab/default_yaml/ae2000/YK17-23C/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/oplab/default_yaml/ae2000/YK17-23C/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.864730 oplab_pipeline-1.1.3/src/oplab/default_yaml/as6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.876731 oplab_pipeline-1.1.3/src/oplab/default_yaml/as6/DY109/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/oplab/default_yaml/as6/DY109/camera.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/oplab/default_yaml/as6/DY109/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/oplab/default_yaml/as6/DY109/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.864730 oplab_pipeline-1.1.3/src/oplab/default_yaml/ts1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.876731 oplab_pipeline-1.1.3/src/oplab/default_yaml/ts1/SSK17-01/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/oplab/default_yaml/ts1/SSK17-01/camera.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/oplab/default_yaml/ts1/SSK17-01/mission.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.864730 oplab_pipeline-1.1.3/src/oplab/default_yaml/ts2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.876731 oplab_pipeline-1.1.3/src/oplab/default_yaml/ts2/SSK16-01/
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/oplab/default_yaml/ts2/SSK16-01/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/oplab/filename_to_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/oplab/folder_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)    19627 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/oplab/mission.py
--rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/oplab/vehicle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.876731 oplab_pipeline-1.1.3/src/oplab_pipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-04-25 16:16:41.000000 oplab_pipeline-1.1.3/src/oplab_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-04-25 16:16:41.000000 oplab_pipeline-1.1.3/src/oplab_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:16:41.000000 oplab_pipeline-1.1.3/src/oplab_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-25 16:16:41.000000 oplab_pipeline-1.1.3/src/oplab_pipeline.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-25 16:16:41.000000 oplab_pipeline-1.1.3/src/oplab_pipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-25 16:16:41.000000 oplab_pipeline-1.1.3/src/oplab_pipeline.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.880731 oplab_pipeline-1.1.3/src/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/scripts/auv_cd.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/scripts/debayer_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/scripts/extract_rosbag_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/scripts/merge_dataset_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/scripts/pixel_stats_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.668285 oplab_pipeline-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    20848 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-06-02 13:59:51.668285 oplab_pipeline-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 13:59:51.672285 oplab_pipeline-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.656285 oplab_pipeline-1.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.656285 oplab_pipeline-1.1.4/src/auv_cal/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_cal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_cal/auv_cal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25715 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_cal/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57980 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_cal/camera_calibrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_cal/cone_fitting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.656285 oplab_pipeline-1.1.4/src/auv_cal/default_yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_cal/default_yaml/default_calibration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_cal/euler_angles_from_rotation_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41020 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_cal/laser_calibrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_cal/plane_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_cal/plot_points_and_planes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_cal/ransac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.656285 oplab_pipeline-1.1.4/src/auv_nav/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10343 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/auv_nav.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14771 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.656285 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.656285 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/ae2000/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.660285 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/ae2000/YK17-23C/
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/ae2000/YK17-23C/camera.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/ae2000/YK17-23C/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/ae2000/YK17-23C/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.656285 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/alr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.660285 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/alr/dy152/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      444 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/alr/dy152/camera.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1468 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/alr/dy152/mission.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1736 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/alr/dy152/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.660285 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/alr/insite/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      444 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/alr/insite/camera.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1757 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/alr/insite/mission.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1962 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/alr/insite/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.660285 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/alr/jc220/
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/alr/jc220/camera.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.656285 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/as6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.660285 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/as6/DY109/
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/as6/DY109/camera.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/as6/DY109/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/as6/DY109/vehicle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/auv_nav.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.660285 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/hybis/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/hybis/camera.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/hybis/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/hybis/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.660285 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/ntnu_rov/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/ntnu_rov/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/ntnu_rov/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.656285 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/ntnu_stereo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.660285 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/ntnu_stereo/tautra21/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/ntnu_stereo/tautra21/camera.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/ntnu_stereo/tautra21/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/ntnu_stereo/tautra21/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.656285 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/rosbag/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.660285 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/rosbag/grassmap/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/rosbag/grassmap/camera.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/rosbag/grassmap/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/rosbag/grassmap/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.656285 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/smarty200/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.660285 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/smarty200/stereo_gopro/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/smarty200/stereo_gopro/camera.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/smarty200/stereo_gopro/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/smarty200/stereo_gopro/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.656285 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/ts1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.660285 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/ts1/SSK17-01/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/ts1/SSK17-01/camera.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/ts1/SSK17-01/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/ts1/SSK17-01/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.656285 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/ts2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.660285 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/ts2/SSK16-01/
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/ts2/SSK16-01/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/default_yaml/ts2/SSK16-01/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.660285 oplab_pipeline-1.1.4/src/auv_nav/localisation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/localisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/localisation/dead_reckoning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43615 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/localisation/ekf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/localisation/particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31173 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/localisation/particle_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19387 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/localisation/pf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/localisation/usbl_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/localisation/usbl_offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26656 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.664285 oplab_pipeline-1.1.4/src/auv_nav/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/parsers/acfr_combined_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11598 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/parsers/acfr_stereo_pose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/parsers/acfr_vehicle_pose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/parsers/generic_csv_payload_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/parsers/hybis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38968 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/parsers/koyo20rov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/parsers/load_matlab_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_NOC_nmea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_NOC_polpred.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_acfr_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17453 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_ae2000.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_alr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_autosub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13242 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_biocam_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_eiva_navipac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21692 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_gaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_interlacer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_koyo21rov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_ntnu_dvl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_ntnu_stereo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_phins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_rdi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_rosbag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_seaxerocks_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_stereo_gopro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_tide_CTI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_usbl_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/parsers/parser_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.664285 oplab_pipeline-1.1.4/src/auv_nav/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/plot/plot_parse_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60072 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/plot/plot_process_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81521 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74413 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/sensors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.664285 oplab_pipeline-1.1.4/src/auv_nav/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/tools/body_to_inertial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13377 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/tools/csv_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/tools/displayable_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/tools/dvl_level_arm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/tools/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/tools/inertial_to_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18019 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/tools/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/tools/latlon_wgs84.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/tools/time_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58260 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/auv_nav/tools/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.664285 oplab_pipeline-1.1.4/src/correct_images/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/correct_images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20183 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/correct_images/correct_images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.664285 oplab_pipeline-1.1.4/src/correct_images/corrections/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/correct_images/corrections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9515 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/correct_images/corrections/attenuation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/correct_images/corrections/debayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/correct_images/corrections/gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/correct_images/corrections/manual_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/correct_images/corrections/pixel_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/correct_images/corrections/rescale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/correct_images/corrections/undistort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56318 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/correct_images/corrector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.656285 oplab_pipeline-1.1.4/src/correct_images/default_yaml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.664285 oplab_pipeline-1.1.4/src/correct_images/default_yaml/acfr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/correct_images/default_yaml/acfr/correct_images.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.664285 oplab_pipeline-1.1.4/src/correct_images/default_yaml/biocam/
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/correct_images/default_yaml/biocam/correct_images.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.668285 oplab_pipeline-1.1.4/src/correct_images/default_yaml/biocam4000_15c/
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/correct_images/default_yaml/biocam4000_15c/correct_images.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.668285 oplab_pipeline-1.1.4/src/correct_images/default_yaml/hybis/
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/correct_images/default_yaml/hybis/correct_images.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.668285 oplab_pipeline-1.1.4/src/correct_images/default_yaml/ntnu_stereo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/correct_images/default_yaml/ntnu_stereo/correct_images.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.668285 oplab_pipeline-1.1.4/src/correct_images/default_yaml/rosbag/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/correct_images/default_yaml/rosbag/correct_images.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.668285 oplab_pipeline-1.1.4/src/correct_images/default_yaml/stereo_gopro/
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/correct_images/default_yaml/stereo_gopro/correct_images.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.668285 oplab_pipeline-1.1.4/src/correct_images/default_yaml/sx3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/correct_images/default_yaml/sx3/correct_images.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.668285 oplab_pipeline-1.1.4/src/correct_images/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/correct_images/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/correct_images/loaders/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/correct_images/loaders/depth_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/correct_images/loaders/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/correct_images/loaders/rosbag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/correct_images/loaders/xviii.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13630 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/correct_images/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.668285 oplab_pipeline-1.1.4/src/correct_images/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/correct_images/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/correct_images/tools/curve_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/correct_images/tools/file_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/correct_images/tools/joblib_tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/correct_images/tools/memmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/correct_images/tools/numerical.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.668285 oplab_pipeline-1.1.4/src/oplab/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/oplab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/oplab/camera_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11572 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/oplab/camera_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/oplab/console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.656285 oplab_pipeline-1.1.4/src/oplab/default_yaml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.656285 oplab_pipeline-1.1.4/src/oplab/default_yaml/ae2000/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.668285 oplab_pipeline-1.1.4/src/oplab/default_yaml/ae2000/YK17-23C/
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/oplab/default_yaml/ae2000/YK17-23C/camera.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/oplab/default_yaml/ae2000/YK17-23C/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/oplab/default_yaml/ae2000/YK17-23C/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.656285 oplab_pipeline-1.1.4/src/oplab/default_yaml/as6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.668285 oplab_pipeline-1.1.4/src/oplab/default_yaml/as6/DY109/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/oplab/default_yaml/as6/DY109/camera.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/oplab/default_yaml/as6/DY109/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/oplab/default_yaml/as6/DY109/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.656285 oplab_pipeline-1.1.4/src/oplab/default_yaml/ts1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.668285 oplab_pipeline-1.1.4/src/oplab/default_yaml/ts1/SSK17-01/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/oplab/default_yaml/ts1/SSK17-01/camera.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/oplab/default_yaml/ts1/SSK17-01/mission.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.656285 oplab_pipeline-1.1.4/src/oplab/default_yaml/ts2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.668285 oplab_pipeline-1.1.4/src/oplab/default_yaml/ts2/SSK16-01/
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/oplab/default_yaml/ts2/SSK16-01/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/oplab/filename_to_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/oplab/folder_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19627 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/oplab/mission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/oplab/vehicle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.668285 oplab_pipeline-1.1.4/src/oplab_pipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-06-02 13:59:51.000000 oplab_pipeline-1.1.4/src/oplab_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-06-02 13:59:51.000000 oplab_pipeline-1.1.4/src/oplab_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 13:59:51.000000 oplab_pipeline-1.1.4/src/oplab_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-02 13:59:51.000000 oplab_pipeline-1.1.4/src/oplab_pipeline.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-02 13:59:51.000000 oplab_pipeline-1.1.4/src/oplab_pipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-02 13:59:51.000000 oplab_pipeline-1.1.4/src/oplab_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:59:51.668285 oplab_pipeline-1.1.4/src/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/scripts/auv_cd.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/scripts/debayer_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/scripts/extract_rosbag_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/scripts/merge_dataset_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-06-02 13:59:31.000000 oplab_pipeline-1.1.4/src/scripts/pixel_stats_folder.py
```

### Comparing `oplab_pipeline-1.1.3/LICENSE` & `oplab_pipeline-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/PKG-INFO` & `oplab_pipeline-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oplab_pipeline
-Version: 1.1.3
+Version: 1.1.4
 Summary: Toolchain for AUV dive processing, camera calibration and image correction
 Home-page: https://github.com/ocean-perception/oplab_pipeline
 Author: Ocean Perception - University of Southampton
 Author-email: miquel.massot-campos@soton.ac.uk
 License: BSD
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `oplab_pipeline-1.1.3/README.md` & `oplab_pipeline-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/setup.py` & `oplab_pipeline-1.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_cal/auv_cal.py` & `oplab_pipeline-1.1.4/src/auv_cal/auv_cal.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_cal/calibration.py` & `oplab_pipeline-1.1.4/src/auv_cal/calibration.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_cal/camera_calibrator.py` & `oplab_pipeline-1.1.4/src/auv_cal/camera_calibrator.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_cal/cone_fitting.py` & `oplab_pipeline-1.1.4/src/auv_cal/cone_fitting.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_cal/default_yaml/default_calibration.yaml` & `oplab_pipeline-1.1.4/src/auv_cal/default_yaml/default_calibration.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_cal/euler_angles_from_rotation_matrix.py` & `oplab_pipeline-1.1.4/src/auv_cal/euler_angles_from_rotation_matrix.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_cal/laser_calibrator.py` & `oplab_pipeline-1.1.4/src/auv_cal/laser_calibrator.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_cal/plane_fitting.py` & `oplab_pipeline-1.1.4/src/auv_cal/plane_fitting.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_cal/plot_points_and_planes.py` & `oplab_pipeline-1.1.4/src/auv_cal/plot_points_and_planes.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_cal/ransac.py` & `oplab_pipeline-1.1.4/src/auv_cal/ransac.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/auv_nav.py` & `oplab_pipeline-1.1.4/src/auv_nav/auv_nav.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/convert.py` & `oplab_pipeline-1.1.4/src/auv_nav/convert.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ae2000/YK17-23C/camera.yaml` & `oplab_pipeline-1.1.4/src/auv_nav/default_yaml/ae2000/YK17-23C/camera.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ae2000/YK17-23C/mission.yaml` & `oplab_pipeline-1.1.4/src/auv_nav/default_yaml/ae2000/YK17-23C/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ae2000/YK17-23C/vehicle.yaml` & `oplab_pipeline-1.1.4/src/auv_nav/default_yaml/ae2000/YK17-23C/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/alr/dy152/mission.yaml` & `oplab_pipeline-1.1.4/src/auv_nav/default_yaml/alr/dy152/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/alr/dy152/vehicle.yaml` & `oplab_pipeline-1.1.4/src/auv_nav/default_yaml/alr/dy152/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/alr/insite/mission.yaml` & `oplab_pipeline-1.1.4/src/auv_nav/default_yaml/alr/insite/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/alr/insite/vehicle.yaml` & `oplab_pipeline-1.1.4/src/auv_nav/default_yaml/alr/insite/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/alr/jc220/camera.yaml` & `oplab_pipeline-1.1.4/src/auv_nav/default_yaml/alr/jc220/camera.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/as6/DY109/camera.yaml` & `oplab_pipeline-1.1.4/src/auv_nav/default_yaml/as6/DY109/camera.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/as6/DY109/mission.yaml` & `oplab_pipeline-1.1.4/src/auv_nav/default_yaml/as6/DY109/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/as6/DY109/vehicle.yaml` & `oplab_pipeline-1.1.4/src/auv_nav/default_yaml/as6/DY109/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/auv_nav.yaml` & `oplab_pipeline-1.1.4/src/auv_nav/default_yaml/auv_nav.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ntnu_rov/mission.yaml` & `oplab_pipeline-1.1.4/src/auv_nav/default_yaml/ntnu_rov/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ntnu_rov/vehicle.yaml` & `oplab_pipeline-1.1.4/src/auv_nav/default_yaml/ntnu_rov/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ntnu_stereo/tautra21/mission.yaml` & `oplab_pipeline-1.1.4/src/auv_nav/default_yaml/ntnu_stereo/tautra21/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ntnu_stereo/tautra21/vehicle.yaml` & `oplab_pipeline-1.1.4/src/auv_nav/default_yaml/ntnu_stereo/tautra21/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/rosbag/grassmap/mission.yaml` & `oplab_pipeline-1.1.4/src/auv_nav/default_yaml/rosbag/grassmap/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/rosbag/grassmap/vehicle.yaml` & `oplab_pipeline-1.1.4/src/auv_nav/default_yaml/rosbag/grassmap/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/smarty200/stereo_gopro/camera.yaml` & `oplab_pipeline-1.1.4/src/auv_nav/default_yaml/smarty200/stereo_gopro/camera.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/smarty200/stereo_gopro/mission.yaml` & `oplab_pipeline-1.1.4/src/auv_nav/default_yaml/smarty200/stereo_gopro/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/smarty200/stereo_gopro/vehicle.yaml` & `oplab_pipeline-1.1.4/src/auv_nav/default_yaml/smarty200/stereo_gopro/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ts1/SSK17-01/mission.yaml` & `oplab_pipeline-1.1.4/src/auv_nav/default_yaml/ts1/SSK17-01/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ts1/SSK17-01/vehicle.yaml` & `oplab_pipeline-1.1.4/src/auv_nav/default_yaml/ts1/SSK17-01/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ts2/SSK16-01/mission.yaml` & `oplab_pipeline-1.1.4/src/auv_nav/default_yaml/ts2/SSK16-01/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ts2/SSK16-01/vehicle.yaml` & `oplab_pipeline-1.1.4/src/auv_nav/default_yaml/ts2/SSK16-01/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/localisation/dead_reckoning.py` & `oplab_pipeline-1.1.4/src/auv_nav/localisation/dead_reckoning.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/localisation/ekf.py` & `oplab_pipeline-1.1.4/src/auv_nav/localisation/ekf.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/localisation/particle.py` & `oplab_pipeline-1.1.4/src/auv_nav/localisation/particle.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/localisation/particle_filter.py` & `oplab_pipeline-1.1.4/src/auv_nav/localisation/particle_filter.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/localisation/pf.py` & `oplab_pipeline-1.1.4/src/auv_nav/localisation/pf.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/localisation/usbl_filter.py` & `oplab_pipeline-1.1.4/src/auv_nav/localisation/usbl_filter.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/localisation/usbl_offset.py` & `oplab_pipeline-1.1.4/src/auv_nav/localisation/usbl_offset.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/parse.py` & `oplab_pipeline-1.1.4/src/auv_nav/parse.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/parsers/acfr_combined_raw.py` & `oplab_pipeline-1.1.4/src/auv_nav/parsers/acfr_combined_raw.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/parsers/acfr_stereo_pose.py` & `oplab_pipeline-1.1.4/src/auv_nav/parsers/acfr_stereo_pose.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/parsers/acfr_vehicle_pose.py` & `oplab_pipeline-1.1.4/src/auv_nav/parsers/acfr_vehicle_pose.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/parsers/generic_csv_payload_parser.py` & `oplab_pipeline-1.1.4/src/auv_nav/parsers/generic_csv_payload_parser.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/parsers/hybis.py` & `oplab_pipeline-1.1.4/src/auv_nav/parsers/hybis.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/parsers/koyo20rov.py` & `oplab_pipeline-1.1.4/src/auv_nav/parsers/koyo20rov.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/parsers/load_matlab_file.py` & `oplab_pipeline-1.1.4/src/auv_nav/parsers/load_matlab_file.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_NOC_nmea.py` & `oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_NOC_nmea.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_NOC_polpred.py` & `oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_NOC_polpred.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_acfr_images.py` & `oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_acfr_images.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_ae2000.py` & `oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_ae2000.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_alr.py` & `oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_alr.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_autosub.py` & `oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_autosub.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_biocam_images.py` & `oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_biocam_images.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_eiva_navipac.py` & `oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_eiva_navipac.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_gaps.py` & `oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_gaps.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_interlacer.py` & `oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_interlacer.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_koyo21rov.py` & `oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_koyo21rov.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_ntnu_dvl.py` & `oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_ntnu_dvl.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_ntnu_stereo.py` & `oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_ntnu_stereo.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_phins.py` & `oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_phins.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_rdi.py` & `oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_rdi.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_rosbag.py` & `oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_rosbag.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_seaxerocks_images.py` & `oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_seaxerocks_images.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_stereo_gopro.py` & `oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_stereo_gopro.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_tide_CTI.py` & `oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_tide_CTI.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_usbl_dump.py` & `oplab_pipeline-1.1.4/src/auv_nav/parsers/parse_usbl_dump.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/parsers/parser_template.py` & `oplab_pipeline-1.1.4/src/auv_nav/parsers/parser_template.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/plot/plot_parse_data.py` & `oplab_pipeline-1.1.4/src/auv_nav/plot/plot_parse_data.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/plot/plot_process_data.py` & `oplab_pipeline-1.1.4/src/auv_nav/plot/plot_process_data.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/process.py` & `oplab_pipeline-1.1.4/src/auv_nav/process.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/sensors.py` & `oplab_pipeline-1.1.4/src/auv_nav/sensors.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/tools/body_to_inertial.py` & `oplab_pipeline-1.1.4/src/auv_nav/tools/body_to_inertial.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/tools/csv_tools.py` & `oplab_pipeline-1.1.4/src/auv_nav/tools/csv_tools.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/tools/displayable_path.py` & `oplab_pipeline-1.1.4/src/auv_nav/tools/displayable_path.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/tools/dvl_level_arm.py` & `oplab_pipeline-1.1.4/src/auv_nav/tools/dvl_level_arm.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/tools/graph.py` & `oplab_pipeline-1.1.4/src/auv_nav/tools/graph.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/tools/inertial_to_body.py` & `oplab_pipeline-1.1.4/src/auv_nav/tools/inertial_to_body.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/tools/interpolate.py` & `oplab_pipeline-1.1.4/src/auv_nav/tools/interpolate.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/tools/latlon_wgs84.py` & `oplab_pipeline-1.1.4/src/auv_nav/tools/latlon_wgs84.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/tools/time_conversions.py` & `oplab_pipeline-1.1.4/src/auv_nav/tools/time_conversions.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/auv_nav/tools/transformations.py` & `oplab_pipeline-1.1.4/src/auv_nav/tools/transformations.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/correct_images/correct_images.py` & `oplab_pipeline-1.1.4/src/correct_images/correct_images.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/correct_images/corrections/__init__.py` & `oplab_pipeline-1.1.4/src/correct_images/corrections/__init__.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/correct_images/corrections/attenuation.py` & `oplab_pipeline-1.1.4/src/correct_images/corrections/attenuation.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/correct_images/corrections/debayer.py` & `oplab_pipeline-1.1.4/src/correct_images/corrections/debayer.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/correct_images/corrections/gamma.py` & `oplab_pipeline-1.1.4/src/correct_images/corrections/gamma.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/correct_images/corrections/manual_balance.py` & `oplab_pipeline-1.1.4/src/correct_images/corrections/manual_balance.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/correct_images/corrections/pixel_stat.py` & `oplab_pipeline-1.1.4/src/correct_images/corrections/pixel_stat.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/correct_images/corrections/rescale.py` & `oplab_pipeline-1.1.4/src/correct_images/corrections/rescale.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/correct_images/corrections/undistort.py` & `oplab_pipeline-1.1.4/src/correct_images/corrections/undistort.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/correct_images/corrector.py` & `oplab_pipeline-1.1.4/src/correct_images/corrector.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,20 +7,14 @@
 """
 
 import copy
 import os
 import random
 from pathlib import Path
 
-try:
-    # Try using the v2 API directly to avoid a warning from imageio >= 2.16.2
-    from imageio.v2 import imwrite
-except ImportError:
-    from imageio import imwrite
-
 import joblib
 import matplotlib
 import numpy as np
 import pandas as pd
 from matplotlib import pyplot as plt
 from tqdm import tqdm, trange
 
@@ -671,40 +665,40 @@
             Console.info("Null distance matrix created")
             self.depth_map_list = []
             return
         elif self.distance_metric == "depth_map":
             # Load depth maps
             path_depth = self.path_processed / "3d_reconstruction" / "depth_maps"
             if not path_depth.exists():
-                Console.quit(
-                    "Depth maps folder", path_depth, "does not exist."
-                )
+                Console.quit("Depth maps folder", path_depth, "does not exist.")
             images_to_drop = []
             for img_idx, image_path in enumerate(self.camera_image_list):
                 p = path_depth / os.path.relpath(image_path, self.path_raw)
                 p = p.with_name(p.stem + "_depthmap.npy")
                 if p.exists():
                     self.depth_map_list.append(p)
                 else:
                     images_to_drop.append(img_idx)
 
             # Drop images that do not have a corresponding depth map
             if len(images_to_drop) > 0:
                 if len(images_to_drop) == len(self.camera_image_list):
                     Console.quit(
-                        "No depth maps found in", path_depth,
-                        "\nLast path checked:", p
+                        "No depth maps found in", path_depth, "\nLast path checked:", p
                     )
                 Console.info(
-                    "Dropping", len(images_to_drop), "of", len(self.camera_image_list),
-                    "images for which no depth maps exists."
+                    "Dropping",
+                    len(images_to_drop),
+                    "of",
+                    len(self.camera_image_list),
+                    "images for which no depth maps exists.",
                 )
                 for idx in sorted(images_to_drop, reverse=True):
                     del self.camera_image_list[idx]
-            assert(len(self.camera_image_list) == len(self.depth_map_list))
+            assert len(self.camera_image_list) == len(self.depth_map_list)
 
             Console.info("Depth maps loaded")
             return
 
     # compute correction parameters either for attenuation correction or
     # static correction of images
     def generate_attenuation_correction_parameters(self):
@@ -763,17 +757,23 @@
 
         distance_vector = None
 
         if self.depth_map_list and self.distance_metric == "depth_map":
             Console.info("Computing depth map histogram with", hist_bins.size, "bins")
 
             distance_vector = np.zeros((len(self.depth_map_list), 1))
-            for i, dm_file in enumerate(self.depth_map_list):
-                dm_np = depth_map.loader(dm_file, self.image_width, self.image_height)
-                distance_vector[i] = dm_np.mean()
+            with tqdm(
+                desc="Computing depth map histogram", total=len(self.depth_map_list)
+            ) as pbar:
+                for i, dm_file in enumerate(self.depth_map_list):
+                    dm_np = depth_map.loader(
+                        dm_file, self.image_width, self.image_height
+                    )
+                    distance_vector[i] = dm_np.mean()
+                    pbar.update(1)
 
         elif self.altitude_list and self.distance_metric == "altitude":
             Console.info("Computing altitude histogram with", hist_bins.size, "bins")
             distance_vector = np.array(self.altitude_list)
 
         if distance_vector is not None:
             idxs = np.digitize(distance_vector, hist_bins) - 1
@@ -1029,23 +1029,14 @@
             # image_raw_std = np.load(self.raw_std_filepath)
 
             ch = image_raw_mean.shape[0]
             if ch == 3:
                 image_raw_mean = image_raw_mean.transpose((1, 2, 0))
                 image_raw_std = image_raw_std.transpose((1, 2, 0))
 
-            imwrite(
-                Path(self.attenuation_parameters_folder) / "image_raw_mean.png",
-                image_raw_mean,
-            )
-            imwrite(
-                Path(self.attenuation_parameters_folder) / "image_raw_std.png",
-                image_raw_std,
-            )
-
             corrections.save_attenuation_plots(
                 self.attenuation_parameters_folder,
                 img_mean=image_raw_mean,
                 img_std=image_raw_std,
             )
 
         Console.info("Correction parameters saved")
```

### Comparing `oplab_pipeline-1.1.3/src/correct_images/default_yaml/acfr/correct_images.yaml` & `oplab_pipeline-1.1.4/src/correct_images/default_yaml/acfr/correct_images.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/correct_images/default_yaml/biocam/correct_images.yaml` & `oplab_pipeline-1.1.4/src/correct_images/default_yaml/biocam/correct_images.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/correct_images/default_yaml/biocam4000_15c/correct_images.yaml` & `oplab_pipeline-1.1.4/src/correct_images/default_yaml/biocam4000_15c/correct_images.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/correct_images/default_yaml/hybis/correct_images.yaml` & `oplab_pipeline-1.1.4/src/correct_images/default_yaml/hybis/correct_images.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/correct_images/default_yaml/ntnu_stereo/correct_images.yaml` & `oplab_pipeline-1.1.4/src/correct_images/default_yaml/ntnu_stereo/correct_images.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/correct_images/default_yaml/rosbag/correct_images.yaml` & `oplab_pipeline-1.1.4/src/correct_images/default_yaml/rosbag/correct_images.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/correct_images/default_yaml/stereo_gopro/correct_images.yaml` & `oplab_pipeline-1.1.4/src/correct_images/default_yaml/stereo_gopro/correct_images.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/correct_images/default_yaml/sx3/correct_images.yaml` & `oplab_pipeline-1.1.4/src/correct_images/default_yaml/sx3/correct_images.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/correct_images/loaders/default.py` & `oplab_pipeline-1.1.4/src/correct_images/loaders/default.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/correct_images/loaders/depth_map.py` & `oplab_pipeline-1.1.4/src/correct_images/loaders/depth_map.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/correct_images/loaders/loader.py` & `oplab_pipeline-1.1.4/src/correct_images/loaders/loader.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/correct_images/loaders/rosbag.py` & `oplab_pipeline-1.1.4/src/correct_images/loaders/rosbag.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/correct_images/loaders/xviii.py` & `oplab_pipeline-1.1.4/src/correct_images/loaders/xviii.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/correct_images/parser.py` & `oplab_pipeline-1.1.4/src/correct_images/parser.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/correct_images/tools/curve_fitting.py` & `oplab_pipeline-1.1.4/src/correct_images/tools/curve_fitting.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/correct_images/tools/file_handlers.py` & `oplab_pipeline-1.1.4/src/correct_images/tools/file_handlers.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/correct_images/tools/joblib_tqdm.py` & `oplab_pipeline-1.1.4/src/correct_images/tools/joblib_tqdm.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/correct_images/tools/memmap.py` & `oplab_pipeline-1.1.4/src/correct_images/tools/memmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,18 @@
 
 
 def create_memmap_name() -> str:
     filename_map = (
         "memmap_"
         + datetime.now().strftime("%Y%m%d_%H%M%S_")
         + "correct_images_"
-        + Console.get_username() + "_"
-        + str(uuid.uuid4()) + ".map"
+        + Console.get_username()
+        + "_"
+        + str(uuid.uuid4())
+        + ".map"
     )
     return filename_map
 
 
 def create_memmap(image_list, dimensions, loader=default.loader):
     filename_map = create_memmap_name()
     Console.info("Creating memmap at", filename_map)
@@ -51,15 +53,15 @@
             image_list, image_memmap, idx, loader, dimensions[1], dimensions[0]
         )
     return filename_map, image_memmap
 
 
 def open_memmap(shape, dtype):
     filename_map = create_memmap_name()
-    Console.info("Creating memmap (open_mammap) at", filename_map)
+    Console.info("Creating memmap (open_memmap) at", filename_map)
     image_memmap = np.memmap(filename=filename_map, mode="w+", shape=shape, dtype=dtype)
     return filename_map, image_memmap
 
 
 def convert_to_memmap(array, loader=default.loader):
     filename_map = create_memmap_name()
     Console.info("Creating memmap (convert_to_memmap) at", filename_map)
```

### Comparing `oplab_pipeline-1.1.3/src/correct_images/tools/numerical.py` & `oplab_pipeline-1.1.4/src/correct_images/tools/numerical.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/oplab/__init__.py` & `oplab_pipeline-1.1.4/src/oplab/__init__.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/oplab/camera_models.py` & `oplab_pipeline-1.1.4/src/oplab/camera_models.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/oplab/camera_system.py` & `oplab_pipeline-1.1.4/src/oplab/camera_system.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/oplab/console.py` & `oplab_pipeline-1.1.4/src/oplab/console.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/oplab/default_yaml/ae2000/YK17-23C/camera.yaml` & `oplab_pipeline-1.1.4/src/oplab/default_yaml/ae2000/YK17-23C/camera.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/oplab/default_yaml/ae2000/YK17-23C/mission.yaml` & `oplab_pipeline-1.1.4/src/oplab/default_yaml/ae2000/YK17-23C/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/oplab/default_yaml/ae2000/YK17-23C/vehicle.yaml` & `oplab_pipeline-1.1.4/src/oplab/default_yaml/ae2000/YK17-23C/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/oplab/default_yaml/as6/DY109/camera.yaml` & `oplab_pipeline-1.1.4/src/oplab/default_yaml/as6/DY109/camera.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/oplab/default_yaml/as6/DY109/mission.yaml` & `oplab_pipeline-1.1.4/src/oplab/default_yaml/as6/DY109/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/oplab/default_yaml/as6/DY109/vehicle.yaml` & `oplab_pipeline-1.1.4/src/oplab/default_yaml/as6/DY109/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/oplab/default_yaml/ts1/SSK17-01/mission.yaml` & `oplab_pipeline-1.1.4/src/oplab/default_yaml/ts1/SSK17-01/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/oplab/default_yaml/ts2/SSK16-01/mission.yaml` & `oplab_pipeline-1.1.4/src/oplab/default_yaml/ts2/SSK16-01/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/oplab/filename_to_date.py` & `oplab_pipeline-1.1.4/src/oplab/filename_to_date.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,9 +189,10 @@
         for index, row in df.iterrows():
             row["epoch_timestamp"] = self.string_to_epoch(
                 row["combined"], row["combined_format"]
             )
 
         df = df.drop("combined", axis=1)
         df = df.drop("combined_format", axis=1)
-        df[df_index_name] = df[df_index_name].astype(int)
-        self.df = df.set_index(df_index_name)
+        if df_index_name:
+            df[df_index_name] = df[df_index_name].astype(int)
+            self.df = df.set_index(df_index_name)
```

### Comparing `oplab_pipeline-1.1.3/src/oplab/folder_structure.py` & `oplab_pipeline-1.1.4/src/oplab/folder_structure.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/oplab/mission.py` & `oplab_pipeline-1.1.4/src/oplab/mission.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/oplab/vehicle.py` & `oplab_pipeline-1.1.4/src/oplab/vehicle.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/oplab_pipeline.egg-info/PKG-INFO` & `oplab_pipeline-1.1.4/src/oplab_pipeline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oplab-pipeline
-Version: 1.1.3
+Version: 1.1.4
 Summary: Toolchain for AUV dive processing, camera calibration and image correction
 Home-page: https://github.com/ocean-perception/oplab_pipeline
 Author: Ocean Perception - University of Southampton
 Author-email: miquel.massot-campos@soton.ac.uk
 License: BSD
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `oplab_pipeline-1.1.3/src/oplab_pipeline.egg-info/SOURCES.txt` & `oplab_pipeline-1.1.4/src/oplab_pipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/scripts/auv_cd.sh` & `oplab_pipeline-1.1.4/src/scripts/auv_cd.sh`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/scripts/debayer_folder.py` & `oplab_pipeline-1.1.4/src/scripts/debayer_folder.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/scripts/extract_rosbag_images.py` & `oplab_pipeline-1.1.4/src/scripts/extract_rosbag_images.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/scripts/merge_dataset_csv.py` & `oplab_pipeline-1.1.4/src/scripts/merge_dataset_csv.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.3/src/scripts/pixel_stats_folder.py` & `oplab_pipeline-1.1.4/src/scripts/pixel_stats_folder.py`

 * *Files identical despite different names*

