# Comparing `tmp/april_vision-1.0.2.tar.gz` & `tmp/april_vision-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "april_vision-1.0.2.tar", last modified: Sat Jan  7 12:21:17 2023, max compression
+gzip compressed data, was "april_vision-2.0.0.tar", last modified: Thu Jun  1 22:06:15 2023, max compression
```

## Comparing `april_vision-1.0.2.tar` & `april_vision-2.0.0.tar`

### file list

```diff
@@ -1,63 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 12:21:17.236678 april_vision-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-01-07 12:20:36.000000 april_vision-1.0.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 12:21:17.224678 april_vision-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 12:21:17.228678 april_vision-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-01-07 12:20:36.000000 april_vision-1.0.2/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-01-07 12:20:36.000000 april_vision-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-07 12:20:36.000000 april_vision-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-01-07 12:20:36.000000 april_vision-1.0.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-01-07 12:21:17.236678 april_vision-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-01-07 12:20:36.000000 april_vision-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 12:21:17.228678 april_vision-1.0.2/april_vision/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-01-07 12:20:36.000000 april_vision-1.0.2/april_vision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-07 12:21:17.000000 april_vision-1.0.2/april_vision/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 12:21:17.232678 april_vision-1.0.2/april_vision/calibrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-01-07 12:20:36.000000 april_vision-1.0.2/april_vision/calibrations/FaceTime HD Camera.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-01-07 12:20:36.000000 april_vision-1.0.2/april_vision/calibrations/Logitech B500.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-01-07 12:20:36.000000 april_vision-1.0.2/april_vision/calibrations/Logitech C270.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-01-07 12:20:36.000000 april_vision-1.0.2/april_vision/calibrations/Logitech C905.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-01-07 12:20:36.000000 april_vision-1.0.2/april_vision/calibrations/Logitech C920.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-01-07 12:20:36.000000 april_vision-1.0.2/april_vision/calibrations/Microdia Integrated_Webcam_HD.xml
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-01-07 12:20:36.000000 april_vision-1.0.2/april_vision/calibrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 12:21:17.232678 april_vision-1.0.2/april_vision/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-01-07 12:20:36.000000 april_vision-1.0.2/april_vision/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-01-07 12:20:36.000000 april_vision-1.0.2/april_vision/cli/annotate_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-01-07 12:20:36.000000 april_vision-1.0.2/april_vision/cli/annotate_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-01-07 12:20:36.000000 april_vision-1.0.2/april_vision/cli/calibrate.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-01-07 12:20:36.000000 april_vision-1.0.2/april_vision/cli/camera_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-01-07 12:20:36.000000 april_vision-1.0.2/april_vision/cli/live.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-01-07 12:20:36.000000 april_vision-1.0.2/april_vision/cli/marker_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-01-07 12:20:36.000000 april_vision-1.0.2/april_vision/cli/vision_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     9493 2023-01-07 12:20:36.000000 april_vision-1.0.2/april_vision/detect_cameras.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-01-07 12:20:36.000000 april_vision-1.0.2/april_vision/frame_sources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 12:21:17.232678 april_vision-1.0.2/april_vision/j5/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-01-07 12:20:36.000000 april_vision-1.0.2/april_vision/j5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8386 2023-01-07 12:20:36.000000 april_vision-1.0.2/april_vision/j5/april_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-01-07 12:20:36.000000 april_vision-1.0.2/april_vision/j5/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15748 2023-01-07 12:20:36.000000 april_vision-1.0.2/april_vision/marker.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-01-07 12:20:36.000000 april_vision-1.0.2/april_vision/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-01-07 12:20:36.000000 april_vision-1.0.2/april_vision/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-01-07 12:20:36.000000 april_vision-1.0.2/april_vision/vision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 12:21:17.228678 april_vision-1.0.2/april_vision.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-01-07 12:21:17.000000 april_vision-1.0.2/april_vision.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-01-07 12:21:17.000000 april_vision-1.0.2/april_vision.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-07 12:21:17.000000 april_vision-1.0.2/april_vision.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-01-07 12:21:17.000000 april_vision-1.0.2/april_vision.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-01-07 12:21:17.000000 april_vision-1.0.2/april_vision.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-07 12:21:17.000000 april_vision-1.0.2/april_vision.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-01-07 12:20:36.000000 april_vision-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-01-07 12:21:17.236678 april_vision-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-07 12:20:36.000000 april_vision-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 12:21:17.224678 april_vision-1.0.2/stubs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 12:21:17.236678 april_vision-1.0.2/stubs/cv2/
--rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-01-07 12:20:36.000000 april_vision-1.0.2/stubs/cv2/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 12:21:17.236678 april_vision-1.0.2/stubs/libusb_package/
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-01-07 12:20:36.000000 april_vision-1.0.2/stubs/libusb_package/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 12:21:17.236678 april_vision-1.0.2/stubs/pyquaternion/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-07 12:20:36.000000 april_vision-1.0.2/stubs/pyquaternion/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-01-07 12:20:36.000000 april_vision-1.0.2/stubs/pyquaternion/quaternion.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 12:21:17.236678 april_vision-1.0.2/stubs/usb/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-01-07 12:20:36.000000 april_vision-1.0.2/stubs/usb/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 12:21:17.236678 april_vision-1.0.2/stubs/usb/backend/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-07 12:20:36.000000 april_vision-1.0.2/stubs/usb/backend/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-01-07 12:20:36.000000 april_vision-1.0.2/stubs/usb/core.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:06:15.159263 april_vision-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-01 22:05:46.000000 april_vision-2.0.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:06:15.155263 april_vision-2.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:06:15.155263 april_vision-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-01 22:05:46.000000 april_vision-2.0.0/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-01 22:05:46.000000 april_vision-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-01 22:05:46.000000 april_vision-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-01 22:05:46.000000 april_vision-2.0.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-01 22:06:15.159263 april_vision-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-01 22:05:46.000000 april_vision-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:06:15.155263 april_vision-2.0.0/april_vision/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-01 22:06:15.000000 april_vision-2.0.0/april_vision/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:06:15.159263 april_vision-2.0.0/april_vision/calibrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/calibrations/FaceTime HD Camera.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/calibrations/Logitech B500.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/calibrations/Logitech C270.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/calibrations/Logitech C905.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/calibrations/Logitech C920.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/calibrations/Microdia Integrated_Webcam_HD.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/calibrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:06:15.159263 april_vision-2.0.0/april_vision/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/cli/annotate_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/cli/annotate_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/cli/calibrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/cli/camera_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/cli/live.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/cli/marker_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17640 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/cli/marker_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:06:15.159263 april_vision-2.0.0/april_vision/cli/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/cli/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/cli/tools/family_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/cli/tools/list_cameras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/cli/vision_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/detect_cameras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:06:15.159263 april_vision-2.0.0/april_vision/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/examples/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/examples/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/frame_sources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:06:15.159263 april_vision-2.0.0/april_vision/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/helpers/markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/helpers/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/helpers/sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11797 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/vision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:06:15.155263 april_vision-2.0.0/april_vision.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-01 22:06:15.000000 april_vision-2.0.0/april_vision.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-01 22:06:15.000000 april_vision-2.0.0/april_vision.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 22:06:15.000000 april_vision-2.0.0/april_vision.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-01 22:06:15.000000 april_vision-2.0.0/april_vision.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-01 22:06:15.000000 april_vision-2.0.0/april_vision.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-01 22:06:15.000000 april_vision-2.0.0/april_vision.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-01 22:05:46.000000 april_vision-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-01 22:06:15.159263 april_vision-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-01 22:05:46.000000 april_vision-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:06:15.155263 april_vision-2.0.0/stubs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:06:15.159263 april_vision-2.0.0/stubs/cv2/
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-06-01 22:05:46.000000 april_vision-2.0.0/stubs/cv2/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:06:15.159263 april_vision-2.0.0/stubs/pyquaternion/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-01 22:05:46.000000 april_vision-2.0.0/stubs/pyquaternion/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-06-01 22:05:46.000000 april_vision-2.0.0/stubs/pyquaternion/quaternion.pyi
```

### Comparing `april_vision-1.0.2/.github/workflows/check.yml` & `april_vision-2.0.0/.github/workflows/check.yml`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
       uses: actions/setup-python@v4
       with:
         python-version: "3.8"
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install .[dev,j5]
+        python -m pip install pypdf
     - name: Lint
       run: |
         make lint
     - name: Isort
       run: |
         make isort-check
     - name: Typecheck
```

### Comparing `april_vision-1.0.2/.gitignore` & `april_vision-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `april_vision-1.0.2/LICENSE` & `april_vision-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `april_vision-1.0.2/PKG-INFO` & `april_vision-2.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: april_vision
-Version: 1.0.2
+Version: 2.0.0
 Summary: An AprilTags wrapper with camera discovery and axis conversion.
 Home-page: https://github.com/WillB97/april_vision
 Author: "Will Barber, Joshua Perriman"
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-Provides-Extra: j5
 Provides-Extra: cli
 Provides-Extra: opencv
 License-File: LICENSE
 
 # april_vision
 
 A fiducial marker system used by Student Robotics.
@@ -39,59 +38,40 @@
 ```
 
 If you need to run the calibration feature in the CLI you will need to install the `opencv-contrib-python` module. All the versions of OpenCV clash so you should only have one installed.
 
 ## Example
 
 ```python
-from april_vision import Processor, USBCamera, calibrations, find_cameras
+from april_vision.examples.camera import setup_cameras
 
-cameras = find_cameras(calibrations)
+# Markers 0-100 are 80mm in size
+tag_sizes = {
+    range(0, 100): 80
+}
 
-try:
-    camera = cameras[0]
-except IndexError:
-    print("No cameras found")
-    exit()
+# Returns a dict of index and camera
+cameras = setup_cameras(tag_sizes)
 
-source = USBCamera.from_calibration_file(
-    camera.index,
-    camera.calibration,
-    camera.vidpid
-)
-
-cam = Processor(
-    source,
-    tag_family='tag36h11',
-    quad_decimate=2.0,
-    tag_sizes=0.08,
-    calibration=source.calibration
-)
+if len(cameras) == 0:
+    print("No cameras found")
 
-markers = cam.see_ids()
-print(markers)
+for name, cam in cameras.items():
+    print(name)
+    print(cam.see())
 ```
 
 ## Tools
 
-When installed april_vision can be used on the command line providing a few useful tools. Each of the tools listed below contain help text on correct usage accessed via the `-h` argument.
+When installed april_vision can be used on the command line providing the following list of useful tools. Each of the tools contain help text on correct usage accessed via the `-h` argument.
 
-```
-april_vision annotate_image
-    Annotate an image file with the detected markers
-```
-```
-april_vision annotate_video
-    Annotate a video file with the detected markers
-```
-```
-april_vision calibrate
-    Generate camera calibration using a ChArUco board
-```
-```
-april_vision live
-    Live camera demonstration with marker annotation
-```
-```
-april_vision vision_debug
-    Generate the debug images of the vision processing steps
+```bash
+annotate_image
+annotate_video
+calibrate
+live
+marker_generator
+vision_debug
+tools
+    family_details
+    list_cameras
 ```
```

### Comparing `april_vision-1.0.2/README.md` & `april_vision-2.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -24,59 +24,40 @@
 ```
 
 If you need to run the calibration feature in the CLI you will need to install the `opencv-contrib-python` module. All the versions of OpenCV clash so you should only have one installed.
 
 ## Example
 
 ```python
-from april_vision import Processor, USBCamera, calibrations, find_cameras
+from april_vision.examples.camera import setup_cameras
 
-cameras = find_cameras(calibrations)
+# Markers 0-100 are 80mm in size
+tag_sizes = {
+    range(0, 100): 80
+}
 
-try:
-    camera = cameras[0]
-except IndexError:
-    print("No cameras found")
-    exit()
+# Returns a dict of index and camera
+cameras = setup_cameras(tag_sizes)
 
-source = USBCamera.from_calibration_file(
-    camera.index,
-    camera.calibration,
-    camera.vidpid
-)
-
-cam = Processor(
-    source,
-    tag_family='tag36h11',
-    quad_decimate=2.0,
-    tag_sizes=0.08,
-    calibration=source.calibration
-)
+if len(cameras) == 0:
+    print("No cameras found")
 
-markers = cam.see_ids()
-print(markers)
+for name, cam in cameras.items():
+    print(name)
+    print(cam.see())
 ```
 
 ## Tools
 
-When installed april_vision can be used on the command line providing a few useful tools. Each of the tools listed below contain help text on correct usage accessed via the `-h` argument.
+When installed april_vision can be used on the command line providing the following list of useful tools. Each of the tools contain help text on correct usage accessed via the `-h` argument.
 
-```
-april_vision annotate_image
-    Annotate an image file with the detected markers
-```
-```
-april_vision annotate_video
-    Annotate a video file with the detected markers
-```
-```
-april_vision calibrate
-    Generate camera calibration using a ChArUco board
-```
-```
-april_vision live
-    Live camera demonstration with marker annotation
-```
-```
-april_vision vision_debug
-    Generate the debug images of the vision processing steps
+```bash
+annotate_image
+annotate_video
+calibrate
+live
+marker_generator
+vision_debug
+tools
+    family_details
+    list_cameras
 ```
```

### Comparing `april_vision-1.0.2/april_vision/__init__.py` & `april_vision-2.0.0/april_vision/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 """An AprilTags wrapper with camera discovery and axis conversion."""
+import os
+
+os.environ["OPENCV_VIDEOIO_MSMF_ENABLE_HW_TRANSFORMS"] = "0"
+
 from ._version import __version__
 from .calibrations import calibrations
-from .detect_cameras import find_cameras
+from .detect_cameras import CalibratedCamera, find_cameras
 from .frame_sources import FrameSource, USBCamera
+from .helpers import generate_marker_size_mapping
 from .marker import (CartesianCoordinates, Marker, Orientation,
                      PixelCoordinates, SphericalCoordinate)
+from .utils import Frame
 from .vision import Processor
 
 __all__ = [
     '__version__',
+    'CalibratedCamera',
     'CartesianCoordinates',
+    'Frame',
     'FrameSource',
     'Marker',
     'Orientation',
     'PixelCoordinates',
     'Processor',
     'SphericalCoordinate',
     'USBCamera',
     'calibrations',
     'find_cameras',
+    'generate_marker_size_mapping',
 ]
```

### Comparing `april_vision-1.0.2/april_vision/calibrations/FaceTime HD Camera.xml` & `april_vision-2.0.0/april_vision/calibrations/FaceTime HD Camera.xml`

 * *Files identical despite different names*

### Comparing `april_vision-1.0.2/april_vision/calibrations/Logitech B500.xml` & `april_vision-2.0.0/april_vision/calibrations/Logitech B500.xml`

 * *Files identical despite different names*

### Comparing `april_vision-1.0.2/april_vision/calibrations/Logitech C270.xml` & `april_vision-2.0.0/april_vision/calibrations/Logitech C270.xml`

 * *Files identical despite different names*

### Comparing `april_vision-1.0.2/april_vision/calibrations/Logitech C905.xml` & `april_vision-2.0.0/april_vision/calibrations/Logitech C905.xml`

 * *Files identical despite different names*

### Comparing `april_vision-1.0.2/april_vision/calibrations/Logitech C920.xml` & `april_vision-2.0.0/april_vision/calibrations/Logitech C920.xml`

 * *Files identical despite different names*

### Comparing `april_vision-1.0.2/april_vision/calibrations/Microdia Integrated_Webcam_HD.xml` & `april_vision-2.0.0/april_vision/calibrations/Microdia Integrated_Webcam_HD.xml`

 * *Files identical despite different names*

### Comparing `april_vision-1.0.2/april_vision/cli/__init__.py` & `april_vision-2.0.0/april_vision/cli/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 import argparse
 import importlib
 import logging
 
 from april_vision._version import version
 
 subcommands = [
+    "tools",
     "annotate_image",
     "annotate_video",
     "calibrate",
     # "camera_benchmark",
     "live",
     # "marker_benchmark",
-    # "marker_generator",
+    "marker_generator",
     "vision_debug",
 ]
 
 
-def build_argparser():
+def build_argparser() -> argparse.ArgumentParser:
     """Load subparsers from available subcommands."""
     parser = argparse.ArgumentParser()
 
     subparsers = parser.add_subparsers(required=True)
     for command in subcommands:
         mod_name = f"{__package__}.{command}"
         importlib.import_module(mod_name).create_subparser(subparsers)
@@ -29,15 +30,15 @@
     parser.add_argument(
         '--version', action='version', version=version, help="Print package version")
     parser.add_argument('--debug', action='store_true', help="Enable debug logging")
 
     return parser
 
 
-def setup_logger(debug=False):
+def setup_logger(debug: bool = False) -> None:
     """Output all loggers to console with custom format at level INFO or DEBUG."""
     formatter = logging.Formatter('%(asctime)s - %(levelname)s - %(message)s')
 
     console_handler = logging.StreamHandler()
     console_handler.setFormatter(formatter)
 
     # log from all loggers to stdout
@@ -45,15 +46,15 @@
     root_logger.setLevel(logging.INFO)
     root_logger.addHandler(console_handler)
 
     if debug:
         root_logger.setLevel(logging.DEBUG)
 
 
-def main():
+def main() -> None:
     """CLI entry-point."""
     parser = build_argparser()
     args = parser.parse_args()
     setup_logger(debug=args.debug)
 
     if "func" in args:
         args.func(args)
```

### Comparing `april_vision-1.0.2/april_vision/cli/annotate_image.py` & `april_vision-2.0.0/april_vision/cli/annotate_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from ..marker import MarkerType
 from ..utils import annotate_text, load_calibration, normalise_marker_text
 from ..vision import Processor
 
 LOGGER = logging.getLogger(__name__)
 
 
-def main(args: argparse.Namespace):
+def main(args: argparse.Namespace) -> None:
     """Annotate an image file using the provided args."""
     input_file = Path(args.input_file)
     if not input_file.exists():
         LOGGER.fatal("Input file does not exist.")
         return
 
     calibration = None
@@ -47,16 +47,16 @@
             for marker in markers:
                 # Check we have pose data
                 _ = marker.cartesian
 
                 text_scale = normalise_marker_text(marker)
 
                 loc = (
-                    int(marker.pixel_centre[0] - 80 * text_scale),
-                    int(marker.pixel_centre[1] + 40 * text_scale),
+                    int(marker.pixel_centre.x - 80 * text_scale),
+                    int(marker.pixel_centre.y + 40 * text_scale),
                 )
                 frame = annotate_text(
                     frame, f"dist={marker.distance}mm", loc,
                     text_scale=0.8 * text_scale,
                     text_colour=(255, 191, 0),  # deep sky blue
                 )
         except RuntimeError:
@@ -68,15 +68,15 @@
     if args.preview:
         cv2.imshow('image', frame.colour_frame)
         LOGGER.info("Press any key to close window.")
         _ = cv2.waitKey(0)
         cv2.destroyAllWindows()
 
 
-def create_subparser(subparsers: argparse._SubParsersAction):
+def create_subparser(subparsers: argparse._SubParsersAction) -> None:
     """Annotate_image command parser."""
     parser = subparsers.add_parser(
         "annotate_image",
         description="Annotate an image file with its markers",
         help="Annotate an image file with its markers",
     )
```

### Comparing `april_vision-1.0.2/april_vision/cli/annotate_video.py` & `april_vision-2.0.0/april_vision/cli/annotate_video.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     height = int(source._video.get(cv2.CAP_PROP_FRAME_HEIGHT))
     calibration = None
     if args.calibration:
         _, calibration = load_calibration(args.calibration)
 
     processer = Processor(
         source,
-        tag_family=args.tag_family.value,
+        tag_family=args.tag_family,
         quad_decimate=args.quad_decimate,
         tag_sizes=float(args.tag_size) / 1000,
         calibration=calibration,
     )
     output = cv2.VideoWriter(
         args.output_file, cv2.VideoWriter_fourcc(*'mp4v'), fps, (width, height))
     while True:
@@ -60,16 +60,16 @@
                 for marker in markers:
                     # Check we have pose data
                     _ = marker.cartesian
 
                     text_scale = normalise_marker_text(marker)
 
                     loc = (
-                        int(marker.pixel_centre[0] - 80 * text_scale),
-                        int(marker.pixel_centre[1] + 40 * text_scale),
+                        int(marker.pixel_centre.x - 80 * text_scale),
+                        int(marker.pixel_centre.y + 40 * text_scale),
                     )
                     frame = annotate_text(
                         frame, f"dist={marker.distance}mm", loc,
                         text_scale=0.8 * text_scale,
                         text_colour=(255, 191, 0),  # deep sky blue
                     )
             except RuntimeError:
```

### Comparing `april_vision-1.0.2/april_vision/cli/calibrate.py` & `april_vision-2.0.0/april_vision/cli/calibrate.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,22 +2,28 @@
 A charuco calibration script.
 
 From: https://gist.github.com/naoki-mizuno/d25cbc3c59228291cabe50529d70894c
 """
 import argparse
 import logging
 import sys
+from datetime import datetime
+from typing import Any, Iterable, List, Tuple
 
 import cv2
-import numpy as np
+from numpy.typing import NDArray
 
 LOGGER = logging.getLogger(__name__)
 
 
-def read_chessboards(frames, aruco_dict, board):
+def read_chessboards(
+    frames: Iterable[NDArray],
+    aruco_dict: Any,
+    board: Any,
+) -> Tuple[Any, Any, Any]:
     """Charuco base pose estimation."""
     all_corners = []
     all_ids = []
 
     for frame in frames:
         gray = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
         corners, ids, rejectedImgPoints = cv2.aruco.detectMarkers(gray, aruco_dict)
@@ -26,68 +32,54 @@
             ret, c_corners, c_ids = cv2.aruco.interpolateCornersCharuco(
                 corners, ids, gray, board)
             # ret is the number of detected corners
             if ret > 0:
                 all_corners.append(c_corners)
                 all_ids.append(c_ids)
         else:
-            LOGGER.error('Failed!')
+            LOGGER.error("Failed!")
 
     imsize = gray.shape
     return all_corners, all_ids, imsize
 
 
-def capture_camera(cap, num=1, mirror=False, size=None):
+def capture_camera(
+    cap: cv2.VideoCapture,
+    num: int = 1,
+    mirror: bool = False,
+    size: Tuple[int, int] = None,
+) -> List[NDArray]:
     """Capture frames to be used for calibration."""
     frames = []
     LOGGER.info("Press space to capture frame.")
 
     while True:
         ret, frame = cap.read()
 
         if mirror is True:
             frame = cv2.flip(frame, 1)
 
         if size is not None and len(size) == 2:
             frame = cv2.resize(frame, size)
 
-        cv2.imshow('Frame', frame)
+        cv2.imshow("Frame", frame)
 
         k = cv2.waitKey(1)
         if k == 27:  # Esc
             break
         elif k == 10 or k == 32:  # Enter or Space
             frames.append(frame)
-            LOGGER.info('Frame captured!')
+            LOGGER.info("Frame captured!")
             if len(frames) == num:
                 break
 
     return frames
 
 
-def draw_axis(frame, camera_matrix, dist_coeff, aruco_dict, board):
-    """Annotate charuco marker target using calibration parameters."""
-    corners, ids, rejected_points = cv2.aruco.detectMarkers(frame, aruco_dict)
-    ret, c_corners, c_ids = cv2.aruco.interpolateCornersCharuco(
-        corners, ids, frame, board)
-    ret, p_rvec, p_tvec = cv2.aruco.estimatePoseCharucoBoard(
-        c_corners, c_ids, board, camera_matrix, dist_coeff, None, None)
-    cv2.drawFrameAxes(
-        frame, camera_matrix, dist_coeff,  p_rvec, p_tvec, 0.1)
-    # cv2.aruco.drawDetectedCornersCharuco(frame, c_corners, c_ids)
-    # cv2.aruco.drawDetectedMarkers(frame, corners, ids)
-    # cv2.aruco.drawDetectedMarkers(frame, rejected_points, borderColor=(100, 0, 240))
-    LOGGER.info('Translation : {0}'.format(p_tvec))
-    LOGGER.info('Rotation    : {0}'.format(p_rvec))
-    LOGGER.info('Distance from camera: {0} m'.format(np.linalg.norm(p_tvec)))
-
-    return frame
-
-
-def main(args: argparse.Namespace):
+def main(args: argparse.Namespace) -> None:
     """Charuco calibration."""
     try:
         import cv2.aruco  # type: ignore
     except ImportError:
         LOGGER.critical("Calibration requires the opencv-contrib-python package")
         sys.exit(1)
 
@@ -99,52 +91,76 @@
 
     if args.resolution:
         video_dev.set(cv2.CAP_PROP_FRAME_WIDTH, args.resolution[0])
         video_dev.set(cv2.CAP_PROP_FRAME_HEIGHT, args.resolution[1])
 
     frames = capture_camera(video_dev, args.frame_count)
     if len(frames) == 0:
-        LOGGER.error('No frame captured')
+        LOGGER.error("No frame captured")
         sys.exit(1)
     all_corners, all_ids, imsize = read_chessboards(frames, aruco_dict, board)
     ret, camera_matrix, dist_coeff, rvec, tvec = cv2.aruco.calibrateCameraCharuco(
         all_corners, all_ids, board, imsize, None, None,
     )
 
     LOGGER.info(f"> Camera matrix\n{camera_matrix}")
     LOGGER.info(f"> Distortion coefficients\n{dist_coeff}")
 
-    height = int(video_dev.get(cv2.CAP_PROP_FRAME_WIDTH))
-    width = int(video_dev.get(cv2.CAP_PROP_FRAME_HEIGHT))
-    LOGGER.info(f"> Resolution\n{height}x{width}")
-
-    LOGGER.info("Capture frame to test calibration.")
-    test_frame = capture_camera(video_dev, 1)[0]
-    test_frame = draw_axis(test_frame, camera_matrix, dist_coeff, aruco_dict, board)
-
-    cv2.imshow('Frame', test_frame)
-    cv2.waitKey(0)
+    width = int(video_dev.get(cv2.CAP_PROP_FRAME_WIDTH))
+    height = int(video_dev.get(cv2.CAP_PROP_FRAME_HEIGHT))
+    LOGGER.info(f"> Resolution\n{width}x{height}")
 
     video_dev.release()
 
+    LOGGER.info("Generating calibration XML file")
+    output_filename = args.cal_filename
+    if not args.cal_filename.lower().endswith(".xml"):
+        output_filename += ".xml"
+
+    file = cv2.FileStorage(args.cal_filename, cv2.FILE_STORAGE_WRITE)
+
+    calibrationDate = datetime.now().strftime("%a %d %b %Y %H:%M:%S")
+    file.write("calibrationDate", calibrationDate)
+
+    file.write("framesCount", args.frame_count)
 
-def create_subparser(subparsers: argparse._SubParsersAction):
+    file.startWriteStruct("cameraResolution", cv2.FILE_NODE_SEQ)
+    file.write("", width)
+    file.write("", height)
+    file.endWriteStruct()
+
+    file.write("cameraMatrix", camera_matrix)
+    file.write("dist_coeffs", dist_coeff)
+
+    if args.vidpid is not None:
+        # Wrap the str in quotes so it is outputed and loaded correctly
+        file.write("vidpid", f'"{args.vidpid}"')
+
+    file.release()
+
+
+def create_subparser(subparsers: argparse._SubParsersAction) -> None:
     """Calibrate command parser."""
     parser = subparsers.add_parser(
         "calibrate",
         help="Generate camera calibration",
         description="""
         Generate camera calibration using a ChArUco board.
 
         Generate a board with:
         https://calib.io/pages/camera-calibration-pattern-generator
         260x200mm, 6x8 squares, 30mm checkers.
         """)
-    parser.add_argument('camera', type=int, help="The camera index")
+    parser.add_argument("camera", type=int, help="The camera index")
     parser.add_argument(
-        '--resolution', type=int, nargs=2, default=None,
+        "--resolution", type=int, nargs=2, default=None,
+        metavar=("WIDTH", "HEIGHT"),
         help="Force camera resolution")
     parser.add_argument(
-        '-n', '--frame_count', type=int, default=15,
-        help="Number of frames to use for calbration.")
+        "-n", "--frame_count", type=int, default=15,
+        help="Number of frames to use for calbration")
+    parser.add_argument(
+        "--vidpid", type=str, default=None,
+        help="VID and PID to be put on the calibration file")
+    parser.add_argument("cal_filename", type=str, help="Filename of output calibration file")
 
     parser.set_defaults(func=main)
```

### Comparing `april_vision-1.0.2/april_vision/cli/live.py` & `april_vision-2.0.0/april_vision/cli/live.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,29 +4,30 @@
 Opens the camera and does live marker detection.
 Can add overlays of fps, marker annotation, marker distance, etc..
 Option to save the current view of the camera.
 """
 import argparse
 import logging
 import os
+from math import degrees
 from time import perf_counter
 
 import cv2
 
 from ..calibrations import calibrations
 from ..detect_cameras import find_cameras
 from ..frame_sources import USBCamera
 from ..marker import MarkerType
 from ..utils import RollingAverage, annotate_text, normalise_marker_text
 from ..vision import Processor
 
 LOGGER = logging.getLogger(__name__)
 
 
-def main(args: argparse.Namespace):
+def main(args: argparse.Namespace) -> None:
     """Live camera demonstration."""
     avg_fps = RollingAverage(50)
     prev_frame_time: float = 0
     file_num = 1
     if args.id is None:
         cameras = find_cameras(calibrations, include_uncalibrated=True)
         try:
@@ -61,60 +62,86 @@
         avg_fps.new_data(fps)
         if args.fps:
             frame = annotate_text(
                 frame, f"{avg_fps.average():.0f}", (7, 70),
                 text_scale=3, text_colour=(100, 255, 0))
 
         if args.distance:
-            try:
-                for marker in markers:
-                    # Check we have pose data
-                    _ = marker.cartesian
-
+            for marker in markers:
+                if marker.has_pose():
                     text_scale = normalise_marker_text(marker)
 
                     loc = (
                         int(marker.pixel_centre[0] - 80 * text_scale),
                         int(marker.pixel_centre[1] + 40 * text_scale),
                     )
                     frame = annotate_text(
                         frame, f"dist={marker.distance}mm", loc,
                         text_scale=0.8 * text_scale,
                         text_colour=(255, 191, 0),  # deep sky blue
                     )
-            except RuntimeError:
-                pass
+
+        for marker in markers:
+            output = "#{}, {}, ({}, {})".format(
+                marker.id,
+                marker.marker_type.value.strip('tag'),
+                int(marker.pixel_centre.x),
+                int(marker.pixel_centre.y),
+            )
+
+            if marker.has_pose():
+                output += (
+                    ", | b={} | r={}, θ={}, φ={} | "
+                    "x={}, y={}, z={} | r={}, p={}, y={}"
+                ).format(
+                    int(marker.bearing),
+                    int(marker.spherical.r),
+                    int(degrees(marker.spherical.theta)),
+                    int(degrees(marker.spherical.phi)),
+                    int(marker.cartesian.x),
+                    int(marker.cartesian.y),
+                    int(marker.cartesian.z),
+                    int(degrees(marker.orientation.roll)),
+                    int(degrees(marker.orientation.pitch)),
+                    int(degrees(marker.orientation.yaw)),
+                )
+            else:
+                output += ", no values for pose estimation"
+
+            LOGGER.info(output)
 
         cv2.imshow('image', frame.colour_frame)
 
         button = cv2.waitKey(1) & 0xFF
-        if button == ord('q'):
+        if (button == ord('q')) or (button == 27):
+            # Quit on q or ESC key
             break
         elif button == ord('s'):
             filename = f'saved_image{file_num:03d}.jpg'
             while os.path.exists(filename):
                 file_num += 1
                 filename = f'saved_image{file_num:03d}.jpg'
 
             cv2.imwrite(filename, frame.colour_frame)
             file_num += 1
 
 
-def create_subparser(subparsers: argparse._SubParsersAction):
+def create_subparser(subparsers: argparse._SubParsersAction) -> None:
     """Live command parser."""
     parser = subparsers.add_parser(
         "live",
         description="Live camera demonstration with marker annotation.",
         help="Live camera demonstration with marker annotation.",
     )
 
     parser.add_argument(
         "--id", type=int, default=None, help="Override the camera index to use.")
     parser.add_argument(
-        "--annotate", action='store_true', help="Annotate detected markers in the frames.")
+        "--no_annotate", action='store_false', dest='annotate',
+        help="Turn off marker annotation for detected markers.")
     parser.add_argument(
         '--fps', action='store_true',
         help="Display the frames per second that the preview is running at.")
 
     parser.add_argument(
         '--tag_family', default=MarkerType.APRILTAG_36H11.value,
         choices=[marker.value for marker in MarkerType],
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `april_vision-1.0.2/april_vision/cli/marker_benchmark.py` & `april_vision-2.0.0/april_vision/cli/marker_benchmark.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 # TODO impliment
 # marker_benchmark
 #     folder of test images
 # 	provide list of actual answers to check against
 #     give performance result
 
 
-def main(args: argparse.Namespace):
+def main(args: argparse.Namespace) -> None:
     """Iterate over images doing marker detection."""
     raise NotImplementedError("Marker benchmark is not implemented.")
 
 
-def create_subparser(subparsers: argparse._SubParsersAction):
+def create_subparser(subparsers: argparse._SubParsersAction) -> None:
     """Marker_benchmark command parser."""
     parser = subparsers.add_parser("marker_benchmark")
 
     parser.set_defaults(func=main)
```

### Comparing `april_vision-1.0.2/april_vision/cli/vision_debug.py` & `april_vision-2.0.0/april_vision/cli/vision_debug.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 of the vision processing steps.
 """
 import argparse
 import logging
 import os
 from contextlib import contextmanager
 from pathlib import Path
+from typing import Generator, List
 
 import cv2
 from PIL import Image
 from pyapriltags import Detector
 
 LOGGER = logging.getLogger(__name__)
 
@@ -31,25 +32,25 @@
     "debug_lines.ps",
     "debug_output.ps",
     "debug_quads.ps",
 ]
 
 
 @contextmanager
-def pushd(new_dir):
+def pushd(new_dir: str) -> Generator[None, None, None]:
     """Enter a directory for the context and return to the previous on exiting."""
     previous_dir = os.getcwd()
     os.chdir(new_dir)
     try:
         yield
     finally:
         os.chdir(previous_dir)
 
 
-def process_debug(preserve=True, collage=True, clean=False):
+def process_debug(preserve: bool = True, collage: bool = True, clean: bool = False) -> None:
     """Convert debug outputs to PNG and optionally collage the images."""
     new_files = []
 
     for index, file in enumerate(pnm_files):
         LOGGER.info(f"Generating PNG for {file}.")
         with Image.open(file) as im:
             new_filename = f"{index}_{file.split('.')[0]}.png"
@@ -70,15 +71,15 @@
             for file in new_files:
                 try:
                     os.remove(file)
                 except FileNotFoundError:
                     pass
 
 
-def create_collage(files, out):
+def create_collage(files: List[str], out: str) -> None:
     """Create a collage of the debug images."""
     LOGGER.info("Generating debug collage.")
     img = Image.open(files[-1])
     width, height = img.size
 
     target_img = Image.new("RGB", (width*4, height*2))
     for k, png in enumerate(files):
@@ -87,15 +88,15 @@
         img.thumbnail((width, height))
         target_img.paste(img, (width*row, height*col))
 
     target_img.save(out)
     LOGGER.info("Generated debug collage.")
 
 
-def main(args: argparse.Namespace):
+def main(args: argparse.Namespace) -> None:
     """Generate the debug images of the vision processing steps."""
     if not args.input_file.exists():
         LOGGER.fatal("Input file does not exist.")
         return
 
     detector = Detector(quad_decimate=1.0, debug=True)
 
@@ -110,15 +111,15 @@
 
         process_debug(
             preserve=not args.cleanup,
             collage=args.collage,
             clean=args.collage_only)
 
 
-def create_subparser(subparsers: argparse._SubParsersAction):
+def create_subparser(subparsers: argparse._SubParsersAction) -> None:
     """Vision_debug command parser."""
     parser = subparsers.add_parser(
         "vision_debug",
         description="Generate the debug images of the vision processing steps.",
         help="Generate the debug images of the vision processing steps.",
     )
```

### Comparing `april_vision-1.0.2/april_vision/detect_cameras.py` & `april_vision-2.0.0/april_vision/detect_cameras.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """OS-specific and generic methods for detecting attached USB cameras."""
 import json
 import logging
 import re
 import subprocess
 import sys
 from pathlib import Path
-from typing import Dict, List, NamedTuple, Optional, Tuple
+from typing import Dict, List, NamedTuple, Optional
 
 import cv2
 
 LOGGER = logging.getLogger(__name__)
 
 
 class CameraIdentifier(NamedTuple):
@@ -39,16 +39,15 @@
     calibration_map = generate_calibration_file_map(calibration_locations)
 
     if platform.startswith("linux"):
         cameras = linux_discovery()
     elif platform.startswith("darwin"):
         cameras = mac_discovery()
     elif platform == "win32":
-        valid_cameras = windows_discovery(calibration_map, include_uncalibrated)
-        return valid_cameras
+        cameras = windows_discovery()
     else:
         cameras = default_discovery()
 
     valid_cameras = match_calibrations(cameras, calibration_map, include_uncalibrated)
 
     return valid_cameras
 
@@ -109,35 +108,14 @@
                     name=camera.name,
                     vidpid=camera.vidpid,
                 ))
 
     return calibrated_cameras + uncalibrated_cameras
 
 
-def usable_present_devices(calibration_map: Dict[str, Path]) -> List[Tuple[str, Path, str]]:
-    """Use PyUSB to detect any supported USB VID/PID combinations connected to the system."""
-    import libusb_package
-    try:
-        usb_devices = libusb_package.find(find_all=True)
-    except ValueError:
-        LOGGER.warning("libusb_package failed to find a libusb backend.")
-        return []
-
-    usable_devices: List[Tuple[str, Path, str]] = []
-
-    for dev in usb_devices:
-        vidpid = f"{dev.idVendor:04x}:{dev.idProduct:04x}"
-        calibration = calibration_map.get(vidpid)
-        if calibration is not None:
-            usable_devices.append((vidpid, calibration, calibration.stem))
-
-    LOGGER.debug(f"Found calibration for the devices: {[dev[0] for dev in usable_devices]}")
-    return usable_devices
-
-
 def linux_discovery() -> List[CameraIdentifier]:
     """
     Discovery method for Linux using Video4Linux.
 
     This matches camera indexes to their USB VID & PID and omits indexes
     that are not the actual camera.
     """
@@ -216,61 +194,52 @@
             cameras.append(CameraIdentifier(index=index, name=name, vidpid=vidpid))
         except KeyError:
             LOGGER.warning(f"Camera {index} had missing fields: {camera}")
 
     return cameras
 
 
-def windows_discovery(
-    calibration_map: Dict[str, Path],
-    include_uncalibrated: bool,
-) -> List[CalibratedCamera]:
+def windows_discovery() -> List[CameraIdentifier]:
     """
-    Discovery method for Windows using PyUSB and the fallback discovery method.
+    Discovery method for Windows using windowsRT API.
 
-    This cannot identify which index corresponds to the found USB VID & PID
-    so is unable to provide a useful output when more than one USB camera with
-    calibration is connected.
-    The returned camera is a combination of the found USB VID & PID and the
-    first openable camera index.
+    Results are only valid for the MSMF opencv backend.
+    This matches camera indexes to their USB VID & PID and omits indexes
+    that are not USB cameras.
     """
-    found_cameras = default_discovery()
-    if include_uncalibrated:
-        # We lack the information to match which camera is which so treat them
-        # all as uncalibrated
-        LOGGER.debug("Assuming all cameras are uncalibrated")
-        return [
-            CalibratedCamera(
-                index=camera.index,
-                name=camera.name,
-                vidpid=camera.vidpid,
-            ) for camera in found_cameras
-        ]
+    import asyncio
 
-    if len(found_cameras) == 0:
-        return []
+    import winsdk.windows.devices.enumeration as windows_devices  # type: ignore
 
-    selected_camera = found_cameras[0]
-    LOGGER.debug(f"Selecting camera index {selected_camera.index}")
+    async def get_camera_info():  # type: ignore
+        device_class = windows_devices.DeviceClass.VIDEO_CAPTURE
+        return await windows_devices.DeviceInformation.find_all_async(device_class)
 
-    usable_cameras = usable_present_devices(calibration_map)
-    if len(usable_cameras) > 1:
-        raise RuntimeError(
-            "Naive calibration selection is only supported when a single compatible "
-            "device is connected")
-    elif len(usable_cameras) == 1:
-        usable_camera = usable_cameras[0]
-        return [CalibratedCamera(
-            index=selected_camera.index,
-            name=usable_camera[2],
-            vidpid=usable_camera[0],
-            calibration=usable_camera[1],
-        )]
-    else:
-        return []
+    connected_cameras = asyncio.run(get_camera_info())  # type: ignore
+
+    cameras = []
+    for index, device in enumerate(connected_cameras):
+        m = re.search(r'USB#VID_([0-9,A-F]{4})&PID_([0-9,A-F]{4})', device.id)
+        if m is None:
+            continue
+
+        vid = int(m.groups()[0], 16)
+        pid = int(m.groups()[1], 16)
+
+        vidpid = f'{vid:04x}:{pid:04x}'
+
+        LOGGER.debug(f"Found camera at index {index}: {device.name}")
+
+        cameras.append(CameraIdentifier(
+            index=index,
+            name=device.name,
+            vidpid=vidpid,
+        ))
+
+    return cameras
 
 
 def default_discovery() -> List[CameraIdentifier]:
     """
     A fallback discovery method for when there is not an OS specific one available.
 
     This cannot identify the USB VID & PID of the camera and only provides
```

### Comparing `april_vision-1.0.2/april_vision/frame_sources.py` & `april_vision-2.0.0/april_vision/frame_sources.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
     def _get_resolution(self) -> Tuple[int, int]:
         """Get the camera resolution active in opencv."""
         return (
             int(self._camera.get(cv2.CAP_PROP_FRAME_WIDTH)),
             int(self._camera.get(cv2.CAP_PROP_FRAME_HEIGHT)),
         )
 
-    def _optimise_camera(self, vidpid: str):
+    def _optimise_camera(self, vidpid: str) -> None:
         """Tweak the camera's image type and framerate to achieve the minimum frame time."""
         verified_vidpid = {'046d:0825', '046d:0807'}
         if not platform.startswith("linux"):
             # All current optimisations are for linux
             return
 
         # These may not improve frame time on all cameras
```

### Comparing `april_vision-1.0.2/april_vision/utils.py` & `april_vision-2.0.0/april_vision/utils.py`

 * *Files identical despite different names*

### Comparing `april_vision-1.0.2/april_vision/vision.py` & `april_vision-2.0.0/april_vision/vision.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from .marker import Marker
 from .utils import Frame, normalise_marker_text
 
 LOGGER = logging.getLogger(__name__)
 
 
 class Processor:
-    """A pyaprilTags wrapper for fiducial detection from frame sources."""
+    """A pyapriltags wrapper for fiducial detection from frame sources."""
 
     capture_filter: Callable[[NDArray], NDArray]
     marker_filter: Callable[[List[Marker]], List[Marker]]
     detection_hook: Callable[[Frame, List[Marker]], None]
 
     def __init__(
         self,
@@ -30,14 +30,15 @@
         *,
         tag_family: str = 'tag36h11',
         threads: int = 4,
         quad_decimate: float = 2,
         aruco_orientation: bool = True,
         name: str = "Camera",
         vidpid: str = "",
+        mask_unknown_size_tags: bool = False,
     ) -> None:
         self.capture_filter = lambda frame: frame
         self.marker_filter = lambda markers: markers
         self.detection_hook = lambda frame, markers: None
 
         self._aruco_orientation = aruco_orientation
         self.calibration = calibration
@@ -47,14 +48,15 @@
         if frame_source is None:
             frame_source = FrameSource()
         self._frame_source = frame_source
 
         if tag_sizes is None:
             tag_sizes = {}
         self.tag_sizes = tag_sizes
+        self.mask_unknown_size_tags = mask_unknown_size_tags
 
         self.detector = Detector(
             families=tag_family,
             nthreads=threads,
             quad_decimate=quad_decimate,
         )
 
@@ -77,15 +79,19 @@
                 estimate_tag_pose=True,
                 camera_params=self.calibration,
                 tag_size=self.tag_sizes,
             )
 
         markers: List[Marker] = []
         for detection in detections:
-            markers.append(Marker(
+            if self.mask_unknown_size_tags and isinstance(self.tag_sizes, dict):
+                # remove detections of marker ids we don't have a size for
+                if detection.tag_id not in self.tag_sizes:
+                    continue
+            markers.append(Marker.from_detection(
                 detection,
                 aruco_orientation=self._aruco_orientation,
             ))
 
         # hook to filter and modify markers
         markers = self.marker_filter(markers)
 
@@ -195,15 +201,20 @@
         if frame is None:
             frames = self._capture()
         else:
             frames = Frame.from_colour_frame(frame)
         markers = self._detect(frames)
         return [marker.id for marker in markers]
 
-    def save(self, name: Union[str, Path], *, frame: Optional[NDArray] = None) -> None:
+    def save(
+        self,
+        name: Union[str, Path],
+        *,
+        frame: Optional[NDArray] = None,
+    ) -> None:
         """Save an annotated image to a file."""
         if frame is None:
             frames = self._capture()
         else:
             frames = Frame.from_colour_frame(frame)
         markers = self._detect(frames)
         frames = self._annotate(
@@ -211,7 +222,18 @@
             markers,
         )
         self._save(frames, name)
 
     def close(self) -> None:
         """Close the underlying capture device."""
         self._frame_source.close()
+
+    def set_marker_sizes(
+        self,
+        tag_sizes: Union[float, Dict[int, float]],
+    ) -> None:
+        """
+        Set the size of tags that are used by pyapriltags for pose estimation.
+
+        Sizes are in meters.
+        """
+        self.tag_sizes = tag_sizes
```

### Comparing `april_vision-1.0.2/april_vision.egg-info/PKG-INFO` & `april_vision-2.0.0/april_vision.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: april-vision
-Version: 1.0.2
+Version: 2.0.0
 Summary: An AprilTags wrapper with camera discovery and axis conversion.
 Home-page: https://github.com/WillB97/april_vision
 Author: "Will Barber, Joshua Perriman"
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-Provides-Extra: j5
 Provides-Extra: cli
 Provides-Extra: opencv
 License-File: LICENSE
 
 # april_vision
 
 A fiducial marker system used by Student Robotics.
@@ -39,59 +38,40 @@
 ```
 
 If you need to run the calibration feature in the CLI you will need to install the `opencv-contrib-python` module. All the versions of OpenCV clash so you should only have one installed.
 
 ## Example
 
 ```python
-from april_vision import Processor, USBCamera, calibrations, find_cameras
+from april_vision.examples.camera import setup_cameras
 
-cameras = find_cameras(calibrations)
+# Markers 0-100 are 80mm in size
+tag_sizes = {
+    range(0, 100): 80
+}
 
-try:
-    camera = cameras[0]
-except IndexError:
-    print("No cameras found")
-    exit()
+# Returns a dict of index and camera
+cameras = setup_cameras(tag_sizes)
 
-source = USBCamera.from_calibration_file(
-    camera.index,
-    camera.calibration,
-    camera.vidpid
-)
-
-cam = Processor(
-    source,
-    tag_family='tag36h11',
-    quad_decimate=2.0,
-    tag_sizes=0.08,
-    calibration=source.calibration
-)
+if len(cameras) == 0:
+    print("No cameras found")
 
-markers = cam.see_ids()
-print(markers)
+for name, cam in cameras.items():
+    print(name)
+    print(cam.see())
 ```
 
 ## Tools
 
-When installed april_vision can be used on the command line providing a few useful tools. Each of the tools listed below contain help text on correct usage accessed via the `-h` argument.
+When installed april_vision can be used on the command line providing the following list of useful tools. Each of the tools contain help text on correct usage accessed via the `-h` argument.
 
-```
-april_vision annotate_image
-    Annotate an image file with the detected markers
-```
-```
-april_vision annotate_video
-    Annotate a video file with the detected markers
-```
-```
-april_vision calibrate
-    Generate camera calibration using a ChArUco board
-```
-```
-april_vision live
-    Live camera demonstration with marker annotation
-```
-```
-april_vision vision_debug
-    Generate the debug images of the vision processing steps
+```bash
+annotate_image
+annotate_video
+calibrate
+live
+marker_generator
+vision_debug
+tools
+    family_details
+    list_cameras
 ```
```

### Comparing `april_vision-1.0.2/april_vision.egg-info/SOURCES.txt` & `april_vision-2.0.0/april_vision.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -31,18 +31,23 @@
 april_vision/cli/__init__.py
 april_vision/cli/annotate_image.py
 april_vision/cli/annotate_video.py
 april_vision/cli/calibrate.py
 april_vision/cli/camera_benchmark.py
 april_vision/cli/live.py
 april_vision/cli/marker_benchmark.py
+april_vision/cli/marker_generator.py
+april_vision/cli/utils.py
 april_vision/cli/vision_debug.py
-april_vision/j5/__init__.py
-april_vision/j5/april_camera.py
-april_vision/j5/py.typed
+april_vision/cli/tools/__init__.py
+april_vision/cli/tools/family_details.py
+april_vision/cli/tools/list_cameras.py
+april_vision/examples/__init__.py
+april_vision/examples/camera.py
+april_vision/examples/py.typed
+april_vision/helpers/__init__.py
+april_vision/helpers/markers.py
+april_vision/helpers/py.typed
+april_vision/helpers/sender.py
 stubs/cv2/__init__.pyi
-stubs/libusb_package/__init__.py
 stubs/pyquaternion/__init__.pyi
-stubs/pyquaternion/quaternion.pyi
-stubs/usb/__init__.pyi
-stubs/usb/core.pyi
-stubs/usb/backend/__init__.pyi
+stubs/pyquaternion/quaternion.pyi
```

### Comparing `april_vision-1.0.2/setup.cfg` & `april_vision-2.0.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -8,32 +8,32 @@
 url = https://github.com/WillB97/april_vision
 
 [options]
 python_requires = >=3.8
 packages = find:
 include_package_data = True
 install_requires = 
-	pyapriltags >=3.3.0.post1, <4
+	pyapriltags >=3.3.0.2, <4
 	numpy >= 1.21, <2
 	pyquaternion >=0.9.9, <1
-	Pillow
-	libusb-package >=1.0.26.1, <2; platform_system=='Windows'
-	pyusb >=1.2.1, <2; platform_system=='Windows'
+	winsdk >=1.0.0b7, <2; platform_system=='Windows'
 
 [options.extras_require]
 dev = 
 	flake8
 	isort
 	mypy
 	build
 	types-Pillow
-j5 = 
-	j5 >=1, <2
+	types-tabulate
 cli = 
 	opencv-python >=4, <5
+	Pillow >=9.4.0, <10
+	pypdf >=3.2.0, <4
+	tabulate >=0.9.0, <1
 opencv = 
 	opencv-python-headless >=4, <5
 
 [options.entry_points]
 console_scripts = 
 	april_vision = april_vision.cli:main
```

### Comparing `april_vision-1.0.2/stubs/cv2/__init__.pyi` & `april_vision-2.0.0/stubs/cv2/__init__.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import typing
+from typing import Any, Tuple
+
 import numpy as np
+from numpy.typing import NDArray
 
-Mat = np.ndarray[int, np.dtype[np.generic]]
+Mat = np.ndarray[int, np.dtype]
 
 FILE_STORAGE_APPEND: int
 FILE_STORAGE_BASE64: int
 FILE_STORAGE_FORMAT_AUTO: int
 FILE_STORAGE_FORMAT_JSON: int
 FILE_STORAGE_FORMAT_MASK: int
 FILE_STORAGE_FORMAT_XML: int
@@ -146,49 +149,69 @@
 IMREAD_REDUCED_COLOR_4: int
 IMREAD_REDUCED_COLOR_8: int
 IMREAD_REDUCED_GRAYSCALE_2: int
 IMREAD_REDUCED_GRAYSCALE_4: int
 IMREAD_REDUCED_GRAYSCALE_8: int
 IMREAD_UNCHANGED: int
 
+FILE_NODE_NONE: int
+FILE_NODE_INT: int
+FILE_NODE_REAL: int
+FILE_NODE_FLOAT: int
+FILE_NODE_STR: int
+FILE_NODE_STRING: int
+FILE_NODE_SEQ: int
+FILE_NODE_MAP: int
+FILE_NODE_TYPE_MASK: int
+FILE_NODE_FLOW: int
+FILE_NODE_UNIFORM: int
+FILE_NODE_EMPTY: int
+FILE_NODE_NAMED: int
+
 
 def cvtColor(src: Mat, code: int, dts: Mat = ..., dstCn: int = ...) -> Mat: ...
 def imread(filename: str, flags: int = ...) -> Mat: ...
 def imwrite(filename: str, img: Mat, params: typing.List[int] = ...) -> bool: ...
 def imencode(ext: str, img: Mat, params: typing.List[int] = ...) -> typing.Tuple[bool, Mat]: ...
-def polylines(img: Mat, pts: typing.List[np.ndarray], isClosed: bool, color: typing.Tuple[int, int, int], thickness: int = ..., lineType: int = ..., shift: int = ...) -> Mat: ...
-def putText(img: Mat, text: str, org: np.ndarray, fontFace: int, fontScale: float, color: typing.Tuple[int, int, int], thickness: int = ..., lineType: int = ..., bottomLeftOrigin: bool = ...) -> Mat: ...
-def VideoWriter_fourcc(c1, c2, c3, c4) -> typing.Any: ...
+def polylines(img: Mat, pts: typing.List[NDArray], isClosed: bool, color: typing.Tuple[int, int, int], thickness: int = ..., lineType: int = ..., shift: int = ...) -> Mat: ...
+def putText(img: Mat, text: str, org: NDArray, fontFace: int, fontScale: float, color: typing.Tuple[int, int, int], thickness: int = ..., lineType: int = ..., bottomLeftOrigin: bool = ...) -> Mat: ...
+def VideoWriter_fourcc(c1: str, c2: str, c3: str, c4: str) -> int: ...
 def imshow(winname: str, mat: Mat) -> None: ...
 def waitKey(delay: int = 0) -> int: ...
 def destroyAllWindows() -> None: ...
+def flip(src: Mat, flipCode: int) -> Mat: ...
+def resize(src: Mat, dsize: Tuple[int, int]) -> Mat: ...
 
 
 class Node:
-    def __init__(self, payload) -> None: ...
+    def __init__(self, payload: Any) -> None: ...
     def isSeq(self) -> bool: ...
     def isString(self) -> bool: ...
     def at(self, i0: int) -> 'Node': ...
     def size(self) -> int: ...
     def string(self) -> str: ...
     def mat(self) -> Mat: ...
     def real(self) -> float: ...
 
 
 class FileStorage:
     def __init__(self, filename: str, flags: int, encoding: str = ...) -> None: ...
     def getNode(self, nodename: str) -> Node: ...
+    def write(self, nodename: str, payload: typing.Any) -> None: ...
+    def release(self) -> None: ...
+    def startWriteStruct(self, nodename: str, flags: int) -> None: ...
+    def endWriteStruct(self) -> None: ...
 
 
 class VideoCapture:
     def __init__(self, index: typing.Union[str, int], apiPreference: int = ...) -> None: ...
     def set(self, propId: int, value: float) -> None: ...
     def get(self, propId: int) -> float: ...
     def release(self) -> None: ...
     def isOpened(self) -> bool: ...
     def read(self) -> typing.Tuple[bool, Mat]: ...
 
 
 class VideoWriter:
-    def __init__(self, filename: str, fourcc: typing.Any, fps: float, frameSize: typing.Tuple[int, int]) -> None: ...
+    def __init__(self, filename: str, fourcc: int, fps: float, frameSize: Tuple[int, int]) -> None: ...
     def write(self, frame: Mat) -> None: ...
     def release(self) -> None: ...
```

### Comparing `april_vision-1.0.2/stubs/pyquaternion/quaternion.pyi` & `april_vision-2.0.0/stubs/pyquaternion/quaternion.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,132 +1,136 @@
-from _typeshed import Incomplete
 from collections.abc import Generator
-from typing import Tuple, Optional
+from typing import Any, Optional, Tuple, Union
 
 import numpy as np
+from numpy.typing import NDArray
+from _typeshed import Incomplete
 
 ThreeTuple = Tuple[float, float, float]
 FourTuple = Tuple[float, float, float, float]
 
 
 class Quaternion:
     q: Incomplete
-    def __init__(self, *args, **kwargs) -> None: ...
+    def __init__(self, *args: Any, **kwargs: Any) -> None: ...
     def __hash__(self) -> int: ...
     @classmethod
     def random(cls) -> 'Quaternion': ...
     def __format__(self, formatstr: str) -> str: ...
     def __int__(self) -> int: ...
     def __float__(self) -> float: ...
     def __complex__(self) -> complex: ...
     def __bool__(self) -> bool: ...
     def __nonzero__(self) -> bool: ...
     def __invert__(self) -> bool: ...
-    def __eq__(self, other): ...
+    def __eq__(self, other: object) -> bool: ...
     def __neg__(self) -> 'Quaternion': ...
     def __abs__(self) -> float: ...
-    def __add__(self, other): ...
-    def __iadd__(self, other): ...
-    def __radd__(self, other): ...
-    def __sub__(self, other): ...
-    def __isub__(self, other): ...
-    def __rsub__(self, other): ...
-    def __mul__(self, other): ...
-    def __imul__(self, other): ...
-    def __rmul__(self, other): ...
-    def __matmul__(self, other): ...
-    def __imatmul__(self, other): ...
-    def __rmatmul__(self, other): ...
-    def __div__(self, other): ...
-    def __idiv__(self, other): ...
-    def __rdiv__(self, other): ...
-    def __truediv__(self, other): ...
-    def __itruediv__(self, other): ...
-    def __rtruediv__(self, other): ...
-    def __pow__(self, exponent): ...
-    def __ipow__(self, other): ...
-    def __rpow__(self, other): ...
+    def __add__(self, other: object) -> 'Quaternion': ...
+    def __iadd__(self, other: object) -> 'Quaternion': ...
+    def __radd__(self, other: object) -> 'Quaternion': ...
+    def __sub__(self, other: object) -> 'Quaternion': ...
+    def __isub__(self, other: object) -> 'Quaternion': ...
+    def __rsub__(self, other: object) -> 'Quaternion': ...
+    def __mul__(self, other: object) -> 'Quaternion': ...
+    def __imul__(self, other: object) -> 'Quaternion': ...
+    def __rmul__(self, other: object) -> 'Quaternion': ...
+    def __matmul__(self, other: object) -> 'Quaternion': ...
+    def __imatmul__(self, other: object) -> 'Quaternion': ...
+    def __rmatmul__(self, other: object) -> 'Quaternion': ...
+    def __div__(self, other: object) -> 'Quaternion': ...
+    def __idiv__(self, other: object) -> 'Quaternion': ...
+    def __rdiv__(self, other: object) -> 'Quaternion': ...
+    def __truediv__(self, other: object) -> 'Quaternion': ...
+    def __itruediv__(self, other: object) -> 'Quaternion': ...
+    def __rtruediv__(self, other: object) -> 'Quaternion': ...
+    def __pow__(self, exponent: float) -> 'Quaternion': ...
+    def __ipow__(self, other: object) -> 'Quaternion': ...
+    def __rpow__(self, other: object) -> 'Quaternion': ...
     @property
     def conjugate(self) -> 'Quaternion': ...
     @property
     def inverse(self) -> 'Quaternion': ...
     @property
     def norm(self) -> float: ...
     @property
     def magnitude(self) -> float: ...
     @property
     def normalised(self) -> 'Quaternion': ...
     @property
-    def polar_unit_vector(self): ...
+    def polar_unit_vector(self) -> NDArray: ...
     @property
     def polar_angle(self) -> float: ...
     @property
-    def polar_decomposition(self): ...
+    def polar_decomposition(self) -> Tuple[NDArray, float]: ...
     @property
     def unit(self) -> 'Quaternion': ...
-    def is_unit(self, tolerance: float = ...): ...
-    def rotate(self, vector): ...
+    def is_unit(self, tolerance: float = ...) -> bool: ...
+    def rotate(
+        self,
+        vector: Union[NDArray, 'Quaternion']
+    ) -> Union[NDArray, 'Quaternion']: ...
     @classmethod
     def exp(cls, q: 'Quaternion') -> 'Quaternion': ...
     @classmethod
     def log(cls, q: 'Quaternion') -> 'Quaternion': ...
     @classmethod
-    def exp_map(cls, q, eta): ...
+    def exp_map(cls, q: 'Quaternion', eta: 'Quaternion') -> 'Quaternion': ...
     @classmethod
-    def sym_exp_map(cls, q, eta): ...
+    def sym_exp_map(cls, q: 'Quaternion', eta: 'Quaternion') -> 'Quaternion': ...
     @classmethod
-    def log_map(cls, q, p): ...
+    def log_map(cls, q: 'Quaternion', p: 'Quaternion') -> 'Quaternion': ...
     @classmethod
-    def sym_log_map(cls, q, p): ...
+    def sym_log_map(cls, q: 'Quaternion', p: 'Quaternion') -> 'Quaternion': ...
     @classmethod
-    def absolute_distance(cls, q0: 'Quaternion', q1: 'Quaternion'): ...
+    def absolute_distance(cls, q0: 'Quaternion', q1: 'Quaternion') -> float: ...
     @classmethod
     def distance(cls, q0: 'Quaternion', q1: 'Quaternion') -> float: ...
     @classmethod
     def sym_distance(cls, q0: 'Quaternion', q1: 'Quaternion') -> float: ...
     @classmethod
     def slerp(cls, q0: 'Quaternion', q1: 'Quaternion', amount: float = ...) -> 'Quaternion': ...
     @classmethod
     def intermediates(cls, q0: 'Quaternion', q1: 'Quaternion', n: int, include_endpoints: bool = ...) -> Generator['Quaternion', None, None]: ...
-    def derivative(self, rate) -> 'Quaternion': ...
-    def integrate(self, rate, timestep) -> None: ...
+    def derivative(self, rate: NDArray) -> 'Quaternion': ...
+    def integrate(self, rate: NDArray, timestep: float) -> None: ...
     @property
-    def rotation_matrix(self) -> np.ndarray: ...
+    def rotation_matrix(self) -> NDArray: ...
     @property
-    def transformation_matrix(self) -> np.ndarray: ...
+    def transformation_matrix(self) -> NDArray: ...
     @property
     def yaw_pitch_roll(self) -> Tuple[float, float, float]: ...
-    def get_axis(self, undefined=...): ...
+    def get_axis(self, undefined: NDArray = ...) -> NDArray: ...
     @property
-    def axis(self): ...
+    def axis(self) -> NDArray: ...
     @property
     def angle(self) -> float: ...
     @property
     def degrees(self) -> float: ...
     @property
     def radians(self) -> float: ...
     @property
     def scalar(self) -> float: ...
     @property
-    def vector(self): ...
+    def vector(self) -> NDArray: ...
     @property
     def real(self) -> float: ...
     @property
-    def imaginary(self): ...
+    def imaginary(self) -> NDArray: ...
     @property
     def w(self) -> float: ...
     @property
     def x(self) -> float: ...
     @property
     def y(self) -> float: ...
     @property
     def z(self) -> float: ...
     @property
-    def elements(self): ...
+    def elements(self) -> NDArray: ...
     def __getitem__(self, index: int) -> float: ...
     def __setitem__(self, index: int, value: float) -> None: ...
     def __copy__(self) -> 'Quaternion': ...
-    def __deepcopy__(self, memo) -> 'Quaternion': ...
+    # def __deepcopy__(self, memo) -> 'Quaternion': ...
     @staticmethod
     def to_degrees(angle_rad: Optional[float]) -> Optional[float]: ...
     @staticmethod
     def to_radians(angle_deg: Optional[float]) -> Optional[float]: ...
```

