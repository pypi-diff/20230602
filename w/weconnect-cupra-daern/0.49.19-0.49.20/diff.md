# Comparing `tmp/weconnect-cupra-daern-0.49.19.tar.gz` & `tmp/weconnect-cupra-daern-0.49.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weconnect-cupra-daern-0.49.19.tar", last modified: Fri Jun  2 08:25:10 2023, max compression
+gzip compressed data, was "weconnect-cupra-daern-0.49.20.tar", last modified: Fri Jun  2 08:46:43 2023, max compression
```

## Comparing `weconnect-cupra-daern-0.49.19.tar` & `weconnect-cupra-daern-0.49.20.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:25:10.617677 weconnect-cupra-daern-0.49.19/
--rw-r--r--   0 daern     (1000) daern     (1000)       51 2023-03-23 10:39:07.000000 weconnect-cupra-daern-0.49.19/MANIFEST.in
--rw-r--r--   0 daern     (1000) daern     (1000)     5580 2023-06-02 08:25:10.617677 weconnect-cupra-daern-0.49.19/PKG-INFO
--rw-r--r--   0 daern     (1000) daern     (1000)     4046 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/README.md
--rw-r--r--   0 daern     (1000) daern     (1000)     2998 2023-06-02 08:25:10.617677 weconnect-cupra-daern-0.49.19/setup.cfg
--rw-r--r--   0 daern     (1000) daern     (1000)     1924 2023-03-23 09:54:10.000000 weconnect-cupra-daern-0.49.19/setup.py
-drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:25:10.597677 weconnect-cupra-daern-0.49.19/tests/
--rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:24.000000 weconnect-cupra-daern-0.49.19/tests/__init__.py
--rw-r--r--   0 daern     (1000) daern     (1000)     8774 2023-01-12 20:52:24.000000 weconnect-cupra-daern-0.49.19/tests/test_addressable.py
--rw-r--r--   0 daern     (1000) daern     (1000)    13494 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/tests/test_cupra.py
--rw-r--r--   0 daern     (1000) daern     (1000)     1002 2023-01-12 20:52:24.000000 weconnect-cupra-daern-0.49.19/tests/test_elements.py
-drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:25:10.597677 weconnect-cupra-daern-0.49.19/weconnect/
--rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:24.000000 weconnect-cupra-daern-0.49.19/weconnect/__init__.py
--rw-r--r--   0 daern     (1000) daern     (1000)       24 2023-06-02 08:24:54.000000 weconnect-cupra-daern-0.49.19/weconnect/__version.py
--rw-r--r--   0 daern     (1000) daern     (1000)    25432 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/addressable.py
-drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:25:10.597677 weconnect-cupra-daern-0.49.19/weconnect/api/
--rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/__init__.py
-drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:25:10.597677 weconnect-cupra-daern-0.49.19/weconnect/api/cupra/
--rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/cupra/__init__.py
--rw-r--r--   0 daern     (1000) daern     (1000)     3885 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/cupra/api.py
-drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:25:10.597677 weconnect-cupra-daern-0.49.19/weconnect/api/cupra/auth/
--rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/cupra/auth/__init__.py
--rw-r--r--   0 daern     (1000) daern     (1000)    17224 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/cupra/auth/my_cupra_session.py
--rw-r--r--   0 daern     (1000) daern     (1000)      362 2023-03-09 16:56:41.000000 weconnect-cupra-daern-0.49.19/weconnect/api/cupra/domain.py
-drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:25:10.607677 weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/
--rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/__init__.py
--rw-r--r--   0 daern     (1000) daern     (1000)    12708 2023-03-10 15:19:25.000000 weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/access_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)     2670 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/battery_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)     4483 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/charging_settings.py
--rw-r--r--   0 daern     (1000) daern     (1000)    14443 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/charging_station.py
--rw-r--r--   0 daern     (1000) daern     (1000)     7736 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/charging_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)     8558 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/climatization_settings.py
--rw-r--r--   0 daern     (1000) daern     (1000)     2762 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/climatization_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)    12294 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/controls.py
--rw-r--r--   0 daern     (1000) daern     (1000)     2228 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/engine_state.py
--rw-r--r--   0 daern     (1000) daern     (1000)      796 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/enums.py
--rw-r--r--   0 daern     (1000) daern     (1000)     3424 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/error.py
--rw-r--r--   0 daern     (1000) daern     (1000)     3387 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/generic_capability.py
--rw-r--r--   0 daern     (1000) daern     (1000)     5260 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/generic_settings.py
-drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:25:10.607677 weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/helpers/
--rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/helpers/__init__.py
--rw-r--r--   0 daern     (1000) daern     (1000)     3492 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/helpers/request_tracker.py
--rw-r--r--   0 daern     (1000) daern     (1000)     2235 2023-01-12 20:57:33.000000 weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/odometer_measurement.py
--rw-r--r--   0 daern     (1000) daern     (1000)     1500 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/parking_position.py
--rw-r--r--   0 daern     (1000) daern     (1000)    22369 2023-03-28 15:48:23.000000 weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/vehicle.py
-drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:25:10.607677 weconnect-cupra-daern-0.49.19/weconnect/api/vw/
--rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/__init__.py
--rw-r--r--   0 daern     (1000) daern     (1000)     7626 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/api.py
-drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:25:10.607677 weconnect-cupra-daern-0.49.19/weconnect/api/vw/auth/
--rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/auth/__init__.py
--rw-r--r--   0 daern     (1000) daern     (1000)    16437 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/auth/we_charge_session.py
--rw-r--r--   0 daern     (1000) daern     (1000)    17759 2023-01-12 20:58:10.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/auth/we_connect_session.py
-drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:25:10.607677 weconnect-cupra-daern-0.49.19/weconnect/api/vw/badges/
--rw-r--r--   0 daern     (1000) daern     (1000)     5504 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/badges/charging.png
--rw-r--r--   0 daern     (1000) daern     (1000)     7170 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/badges/connected.png
--rw-r--r--   0 daern     (1000) daern     (1000)     9627 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/badges/cooling.png
--rw-r--r--   0 daern     (1000) daern     (1000)     7549 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/badges/heating.png
--rw-r--r--   0 daern     (1000) daern     (1000)     7022 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/badges/locked.png
--rw-r--r--   0 daern     (1000) daern     (1000)     5710 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/badges/parking.png
--rw-r--r--   0 daern     (1000) daern     (1000)     6941 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/badges/unlocked.png
--rw-r--r--   0 daern     (1000) daern     (1000)     8409 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/badges/ventilating.png
--rw-r--r--   0 daern     (1000) daern     (1000)     8199 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/badges/warning.png
--rw-r--r--   0 daern     (1000) daern     (1000)      659 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/domain.py
-drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:25:10.617677 weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/
--rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/__init__.py
--rw-r--r--   0 daern     (1000) daern     (1000)    10015 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/access_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)     2443 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/battery_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)     1970 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/capability_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)     3692 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/charge_mode.py
--rw-r--r--   0 daern     (1000) daern     (1000)    11793 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/charging_profiles.py
--rw-r--r--   0 daern     (1000) daern     (1000)     4295 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/charging_settings.py
--rw-r--r--   0 daern     (1000) daern     (1000)    19151 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/charging_station.py
--rw-r--r--   0 daern     (1000) daern     (1000)     7701 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/charging_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)     8079 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/climatization_settings.py
--rw-r--r--   0 daern     (1000) daern     (1000)     2868 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/climatization_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)     2691 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/climatization_timer.py
--rw-r--r--   0 daern     (1000) daern     (1000)     9402 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/controls.py
--rw-r--r--   0 daern     (1000) daern     (1000)      562 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/enums.py
--rw-r--r--   0 daern     (1000) daern     (1000)     3391 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/generic_capability.py
--rw-r--r--   0 daern     (1000) daern     (1000)     2083 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/generic_request_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)     3104 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/generic_settings.py
-drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:25:10.617677 weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/helpers/
--rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/helpers/__init__.py
--rw-r--r--   0 daern     (1000) daern     (1000)     3486 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/helpers/request_tracker.py
--rw-r--r--   0 daern     (1000) daern     (1000)     3331 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/lights_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)     1639 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/lv_battery_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)     3760 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/maintenance_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)     2319 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/odometer_measurement.py
--rw-r--r--   0 daern     (1000) daern     (1000)     1661 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/parking_position.py
--rw-r--r--   0 daern     (1000) daern     (1000)     1610 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/range_measurements.py
--rw-r--r--   0 daern     (1000) daern     (1000)     5078 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/range_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)     6696 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/readiness_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)     7627 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/timer.py
--rw-r--r--   0 daern     (1000) daern     (1000)    46165 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/vehicle.py
--rw-r--r--   0 daern     (1000) daern     (1000)     7969 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/warning_lights_status.py
-drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:25:10.617677 weconnect-cupra-daern-0.49.19/weconnect/auth/
--rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:24.000000 weconnect-cupra-daern-0.49.19/weconnect/auth/__init__.py
--rw-r--r--   0 daern     (1000) daern     (1000)      142 2023-01-12 20:52:24.000000 weconnect-cupra-daern-0.49.19/weconnect/auth/auth_util.py
--rw-r--r--   0 daern     (1000) daern     (1000)     7234 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/auth/openid_session.py
--rw-r--r--   0 daern     (1000) daern     (1000)     3101 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/auth/session_manager.py
--rw-r--r--   0 daern     (1000) daern     (1000)      232 2023-01-12 20:52:24.000000 weconnect-cupra-daern-0.49.19/weconnect/auth/vw_web_session.py
-drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:25:10.617677 weconnect-cupra-daern-0.49.19/weconnect/elements/
--rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:24.000000 weconnect-cupra-daern-0.49.19/weconnect/elements/__init__.py
--rw-r--r--   0 daern     (1000) daern     (1000)      880 2023-03-10 15:22:13.000000 weconnect-cupra-daern-0.49.19/weconnect/elements/access_control_state.py
--rw-r--r--   0 daern     (1000) daern     (1000)      927 2023-01-12 20:52:24.000000 weconnect-cupra-daern-0.49.19/weconnect/elements/control_operation.py
--rw-r--r--   0 daern     (1000) daern     (1000)     3426 2023-01-12 20:52:24.000000 weconnect-cupra-daern-0.49.19/weconnect/elements/error.py
--rw-r--r--   0 daern     (1000) daern     (1000)     9952 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/elements/generic_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)     3437 2023-01-12 20:58:26.000000 weconnect-cupra-daern-0.49.19/weconnect/elements/plug_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)     3818 2023-01-12 20:58:33.000000 weconnect-cupra-daern-0.49.19/weconnect/elements/window_heating_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)     2338 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/errors.py
--rw-r--r--   0 daern     (1000) daern     (1000)     7387 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/fetch.py
--rw-r--r--   0 daern     (1000) daern     (1000)      182 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/service.py
--rw-r--r--   0 daern     (1000) daern     (1000)     3695 2023-01-12 20:57:00.000000 weconnect-cupra-daern-0.49.19/weconnect/util.py
--rw-r--r--   0 daern     (1000) daern     (1000)     9001 2023-01-12 20:57:09.000000 weconnect-cupra-daern-0.49.19/weconnect/weconnect.py
--rw-r--r--   0 daern     (1000) daern     (1000)      184 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.19/weconnect/weconnect_errors.py
-drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:25:10.617677 weconnect-cupra-daern-0.49.19/weconnect_cupra_daern.egg-info/
--rw-r--r--   0 daern     (1000) daern     (1000)     5580 2023-06-02 08:25:10.000000 weconnect-cupra-daern-0.49.19/weconnect_cupra_daern.egg-info/PKG-INFO
--rw-r--r--   0 daern     (1000) daern     (1000)     3995 2023-06-02 08:25:10.000000 weconnect-cupra-daern-0.49.19/weconnect_cupra_daern.egg-info/SOURCES.txt
--rw-r--r--   0 daern     (1000) daern     (1000)        1 2023-06-02 08:25:10.000000 weconnect-cupra-daern-0.49.19/weconnect_cupra_daern.egg-info/dependency_links.txt
--rw-r--r--   0 daern     (1000) daern     (1000)        1 2023-03-23 10:05:32.000000 weconnect-cupra-daern-0.49.19/weconnect_cupra_daern.egg-info/not-zip-safe
--rw-r--r--   0 daern     (1000) daern     (1000)       76 2023-06-02 08:25:10.000000 weconnect-cupra-daern-0.49.19/weconnect_cupra_daern.egg-info/requires.txt
--rw-r--r--   0 daern     (1000) daern     (1000)       16 2023-06-02 08:25:10.000000 weconnect-cupra-daern-0.49.19/weconnect_cupra_daern.egg-info/top_level.txt
+drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:46:43.897645 weconnect-cupra-daern-0.49.20/
+-rw-r--r--   0 daern     (1000) daern     (1000)       51 2023-03-23 10:39:07.000000 weconnect-cupra-daern-0.49.20/MANIFEST.in
+-rw-r--r--   0 daern     (1000) daern     (1000)     5580 2023-06-02 08:46:43.897645 weconnect-cupra-daern-0.49.20/PKG-INFO
+-rw-r--r--   0 daern     (1000) daern     (1000)     4046 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/README.md
+-rw-r--r--   0 daern     (1000) daern     (1000)     2998 2023-06-02 08:46:43.897645 weconnect-cupra-daern-0.49.20/setup.cfg
+-rw-r--r--   0 daern     (1000) daern     (1000)     1924 2023-03-23 09:54:10.000000 weconnect-cupra-daern-0.49.20/setup.py
+drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:46:43.887645 weconnect-cupra-daern-0.49.20/tests/
+-rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:24.000000 weconnect-cupra-daern-0.49.20/tests/__init__.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     8774 2023-01-12 20:52:24.000000 weconnect-cupra-daern-0.49.20/tests/test_addressable.py
+-rw-r--r--   0 daern     (1000) daern     (1000)    13494 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/tests/test_cupra.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     1002 2023-01-12 20:52:24.000000 weconnect-cupra-daern-0.49.20/tests/test_elements.py
+drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:46:43.887645 weconnect-cupra-daern-0.49.20/weconnect/
+-rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:24.000000 weconnect-cupra-daern-0.49.20/weconnect/__init__.py
+-rw-r--r--   0 daern     (1000) daern     (1000)       24 2023-06-02 08:46:17.000000 weconnect-cupra-daern-0.49.20/weconnect/__version.py
+-rw-r--r--   0 daern     (1000) daern     (1000)    25432 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/addressable.py
+drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:46:43.887645 weconnect-cupra-daern-0.49.20/weconnect/api/
+-rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/__init__.py
+drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:46:43.887645 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/
+-rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/__init__.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     3885 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/api.py
+drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:46:43.887645 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/auth/
+-rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/auth/__init__.py
+-rw-r--r--   0 daern     (1000) daern     (1000)    17224 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/auth/my_cupra_session.py
+-rw-r--r--   0 daern     (1000) daern     (1000)      362 2023-03-09 16:56:41.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/domain.py
+drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:46:43.887645 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/
+-rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/__init__.py
+-rw-r--r--   0 daern     (1000) daern     (1000)    12708 2023-03-10 15:19:25.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/access_status.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     2670 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/battery_status.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     4483 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/charging_settings.py
+-rw-r--r--   0 daern     (1000) daern     (1000)    14443 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/charging_station.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     7736 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/charging_status.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     8558 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/climatization_settings.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     2762 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/climatization_status.py
+-rw-r--r--   0 daern     (1000) daern     (1000)    12294 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/controls.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     2228 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/engine_state.py
+-rw-r--r--   0 daern     (1000) daern     (1000)      796 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/enums.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     3424 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/error.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     3387 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/generic_capability.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     5260 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/generic_settings.py
+drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:46:43.887645 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/helpers/
+-rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/helpers/__init__.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     3492 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/helpers/request_tracker.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     2235 2023-01-12 20:57:33.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/odometer_measurement.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     1500 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/parking_position.py
+-rw-r--r--   0 daern     (1000) daern     (1000)    22369 2023-03-28 15:48:23.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/vehicle.py
+drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:46:43.887645 weconnect-cupra-daern-0.49.20/weconnect/api/vw/
+-rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/__init__.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     7626 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/api.py
+drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:46:43.887645 weconnect-cupra-daern-0.49.20/weconnect/api/vw/auth/
+-rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/auth/__init__.py
+-rw-r--r--   0 daern     (1000) daern     (1000)    16437 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/auth/we_charge_session.py
+-rw-r--r--   0 daern     (1000) daern     (1000)    17759 2023-01-12 20:58:10.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/auth/we_connect_session.py
+drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:46:43.887645 weconnect-cupra-daern-0.49.20/weconnect/api/vw/badges/
+-rw-r--r--   0 daern     (1000) daern     (1000)     5504 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/badges/charging.png
+-rw-r--r--   0 daern     (1000) daern     (1000)     7170 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/badges/connected.png
+-rw-r--r--   0 daern     (1000) daern     (1000)     9627 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/badges/cooling.png
+-rw-r--r--   0 daern     (1000) daern     (1000)     7549 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/badges/heating.png
+-rw-r--r--   0 daern     (1000) daern     (1000)     7022 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/badges/locked.png
+-rw-r--r--   0 daern     (1000) daern     (1000)     5710 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/badges/parking.png
+-rw-r--r--   0 daern     (1000) daern     (1000)     6941 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/badges/unlocked.png
+-rw-r--r--   0 daern     (1000) daern     (1000)     8409 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/badges/ventilating.png
+-rw-r--r--   0 daern     (1000) daern     (1000)     8199 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/badges/warning.png
+-rw-r--r--   0 daern     (1000) daern     (1000)      659 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/domain.py
+drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:46:43.887645 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/
+-rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/__init__.py
+-rw-r--r--   0 daern     (1000) daern     (1000)    10015 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/access_status.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     2443 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/battery_status.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     1970 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/capability_status.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     3692 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/charge_mode.py
+-rw-r--r--   0 daern     (1000) daern     (1000)    11793 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/charging_profiles.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     4295 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/charging_settings.py
+-rw-r--r--   0 daern     (1000) daern     (1000)    19151 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/charging_station.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     7701 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/charging_status.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     8079 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/climatization_settings.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     2868 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/climatization_status.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     2691 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/climatization_timer.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     9402 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/controls.py
+-rw-r--r--   0 daern     (1000) daern     (1000)      562 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/enums.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     3391 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/generic_capability.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     2083 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/generic_request_status.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     3104 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/generic_settings.py
+drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:46:43.887645 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/helpers/
+-rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/helpers/__init__.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     3486 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/helpers/request_tracker.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     3331 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/lights_status.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     1639 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/lv_battery_status.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     3760 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/maintenance_status.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     2319 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/odometer_measurement.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     1661 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/parking_position.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     1610 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/range_measurements.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     5078 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/range_status.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     6696 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/readiness_status.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     7627 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/timer.py
+-rw-r--r--   0 daern     (1000) daern     (1000)    46165 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/vehicle.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     7969 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/warning_lights_status.py
+drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:46:43.887645 weconnect-cupra-daern-0.49.20/weconnect/auth/
+-rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:24.000000 weconnect-cupra-daern-0.49.20/weconnect/auth/__init__.py
+-rw-r--r--   0 daern     (1000) daern     (1000)      142 2023-01-12 20:52:24.000000 weconnect-cupra-daern-0.49.20/weconnect/auth/auth_util.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     7234 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/auth/openid_session.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     3101 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/auth/session_manager.py
+-rw-r--r--   0 daern     (1000) daern     (1000)      232 2023-01-12 20:52:24.000000 weconnect-cupra-daern-0.49.20/weconnect/auth/vw_web_session.py
+drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:46:43.897645 weconnect-cupra-daern-0.49.20/weconnect/elements/
+-rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:24.000000 weconnect-cupra-daern-0.49.20/weconnect/elements/__init__.py
+-rw-r--r--   0 daern     (1000) daern     (1000)      880 2023-03-10 15:22:13.000000 weconnect-cupra-daern-0.49.20/weconnect/elements/access_control_state.py
+-rw-r--r--   0 daern     (1000) daern     (1000)      927 2023-01-12 20:52:24.000000 weconnect-cupra-daern-0.49.20/weconnect/elements/control_operation.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     3426 2023-01-12 20:52:24.000000 weconnect-cupra-daern-0.49.20/weconnect/elements/error.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     9952 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/elements/generic_status.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     3437 2023-01-12 20:58:26.000000 weconnect-cupra-daern-0.49.20/weconnect/elements/plug_status.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     3818 2023-01-12 20:58:33.000000 weconnect-cupra-daern-0.49.20/weconnect/elements/window_heating_status.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     2338 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/errors.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     7387 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/fetch.py
+-rw-r--r--   0 daern     (1000) daern     (1000)      182 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/service.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     3695 2023-01-12 20:57:00.000000 weconnect-cupra-daern-0.49.20/weconnect/util.py
+-rw-r--r--   0 daern     (1000) daern     (1000)     9001 2023-01-12 20:57:09.000000 weconnect-cupra-daern-0.49.20/weconnect/weconnect.py
+-rw-r--r--   0 daern     (1000) daern     (1000)      184 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/weconnect_errors.py
+drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:46:43.897645 weconnect-cupra-daern-0.49.20/weconnect_cupra_daern.egg-info/
+-rw-r--r--   0 daern     (1000) daern     (1000)     5580 2023-06-02 08:46:43.000000 weconnect-cupra-daern-0.49.20/weconnect_cupra_daern.egg-info/PKG-INFO
+-rw-r--r--   0 daern     (1000) daern     (1000)     3995 2023-06-02 08:46:43.000000 weconnect-cupra-daern-0.49.20/weconnect_cupra_daern.egg-info/SOURCES.txt
+-rw-r--r--   0 daern     (1000) daern     (1000)        1 2023-06-02 08:46:43.000000 weconnect-cupra-daern-0.49.20/weconnect_cupra_daern.egg-info/dependency_links.txt
+-rw-r--r--   0 daern     (1000) daern     (1000)        1 2023-03-23 10:05:32.000000 weconnect-cupra-daern-0.49.20/weconnect_cupra_daern.egg-info/not-zip-safe
+-rw-r--r--   0 daern     (1000) daern     (1000)       76 2023-06-02 08:46:43.000000 weconnect-cupra-daern-0.49.20/weconnect_cupra_daern.egg-info/requires.txt
+-rw-r--r--   0 daern     (1000) daern     (1000)       16 2023-06-02 08:46:43.000000 weconnect-cupra-daern-0.49.20/weconnect_cupra_daern.egg-info/top_level.txt
```

### Comparing `weconnect-cupra-daern-0.49.19/PKG-INFO` & `weconnect-cupra-daern-0.49.20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weconnect-cupra-daern
-Version: 0.49.19
+Version: 0.49.20
 Summary: Fork of Python API for the Volkswagen WeConnect Services to support Cupra Born
 Home-page: https://github.com/daernsinstantfortress/WeConnect-python
 Author: Till Steinbach / Alan Gibson / Stuart Hall
 License: MIT
 Project-URL: Funding, https://github.com/sponsors/tillsteinbach
 Project-URL: Source, https://github.com/daernsinstantfortress/WeConnect-python
 Project-URL: Bug Tracker, https://github.com/tillsteinbach/WeConnect-python/issues
```

### Comparing `weconnect-cupra-daern-0.49.19/README.md` & `weconnect-cupra-daern-0.49.20/README.md`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/setup.cfg` & `weconnect-cupra-daern-0.49.20/setup.cfg`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/setup.py` & `weconnect-cupra-daern-0.49.20/setup.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/tests/test_addressable.py` & `weconnect-cupra-daern-0.49.20/tests/test_addressable.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/tests/test_cupra.py` & `weconnect-cupra-daern-0.49.20/tests/test_cupra.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/tests/test_elements.py` & `weconnect-cupra-daern-0.49.20/tests/test_elements.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/addressable.py` & `weconnect-cupra-daern-0.49.20/weconnect/addressable.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/cupra/api.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/api.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/cupra/auth/my_cupra_session.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/auth/my_cupra_session.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/access_status.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/access_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/battery_status.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/battery_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/charging_settings.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/charging_settings.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/charging_station.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/charging_station.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/charging_status.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/charging_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/climatization_settings.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/climatization_settings.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/climatization_status.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/climatization_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/controls.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/controls.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/engine_state.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/engine_state.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/enums.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/enums.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/error.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/error.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/generic_capability.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/generic_capability.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/generic_settings.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/generic_settings.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/helpers/request_tracker.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/helpers/request_tracker.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/odometer_measurement.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/odometer_measurement.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/parking_position.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/parking_position.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/cupra/elements/vehicle.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/vehicle.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/api.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/api.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/auth/we_charge_session.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/auth/we_charge_session.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/auth/we_connect_session.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/auth/we_connect_session.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/badges/charging.png` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/badges/charging.png`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/badges/connected.png` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/badges/connected.png`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/badges/cooling.png` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/badges/cooling.png`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/badges/heating.png` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/badges/heating.png`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/badges/locked.png` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/badges/locked.png`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/badges/parking.png` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/badges/parking.png`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/badges/unlocked.png` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/badges/unlocked.png`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/badges/ventilating.png` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/badges/ventilating.png`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/badges/warning.png` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/badges/warning.png`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/domain.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/domain.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/access_status.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/access_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/battery_status.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/battery_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/capability_status.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/capability_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/charge_mode.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/charge_mode.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/charging_profiles.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/charging_profiles.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/charging_settings.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/charging_settings.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/charging_station.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/charging_station.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/charging_status.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/charging_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/climatization_settings.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/climatization_settings.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/climatization_status.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/climatization_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/climatization_timer.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/climatization_timer.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/controls.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/controls.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/enums.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/enums.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/generic_capability.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/generic_capability.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/generic_request_status.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/generic_request_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/generic_settings.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/generic_settings.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/helpers/request_tracker.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/helpers/request_tracker.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/lights_status.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/lights_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/lv_battery_status.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/lv_battery_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/maintenance_status.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/maintenance_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/odometer_measurement.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/odometer_measurement.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/parking_position.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/parking_position.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/range_measurements.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/range_measurements.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/range_status.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/range_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/readiness_status.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/readiness_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/timer.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/timer.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/vehicle.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/vehicle.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/api/vw/elements/warning_lights_status.py` & `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/warning_lights_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/auth/openid_session.py` & `weconnect-cupra-daern-0.49.20/weconnect/auth/openid_session.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/auth/session_manager.py` & `weconnect-cupra-daern-0.49.20/weconnect/auth/session_manager.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/elements/access_control_state.py` & `weconnect-cupra-daern-0.49.20/weconnect/elements/access_control_state.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/elements/control_operation.py` & `weconnect-cupra-daern-0.49.20/weconnect/elements/control_operation.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/elements/error.py` & `weconnect-cupra-daern-0.49.20/weconnect/elements/error.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/elements/generic_status.py` & `weconnect-cupra-daern-0.49.20/weconnect/elements/generic_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/elements/plug_status.py` & `weconnect-cupra-daern-0.49.20/weconnect/elements/plug_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/elements/window_heating_status.py` & `weconnect-cupra-daern-0.49.20/weconnect/elements/window_heating_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/errors.py` & `weconnect-cupra-daern-0.49.20/weconnect/errors.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/fetch.py` & `weconnect-cupra-daern-0.49.20/weconnect/fetch.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/util.py` & `weconnect-cupra-daern-0.49.20/weconnect/util.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect/weconnect.py` & `weconnect-cupra-daern-0.49.20/weconnect/weconnect.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.19/weconnect_cupra_daern.egg-info/PKG-INFO` & `weconnect-cupra-daern-0.49.20/weconnect_cupra_daern.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weconnect-cupra-daern
-Version: 0.49.19
+Version: 0.49.20
 Summary: Fork of Python API for the Volkswagen WeConnect Services to support Cupra Born
 Home-page: https://github.com/daernsinstantfortress/WeConnect-python
 Author: Till Steinbach / Alan Gibson / Stuart Hall
 License: MIT
 Project-URL: Funding, https://github.com/sponsors/tillsteinbach
 Project-URL: Source, https://github.com/daernsinstantfortress/WeConnect-python
 Project-URL: Bug Tracker, https://github.com/tillsteinbach/WeConnect-python/issues
```

### Comparing `weconnect-cupra-daern-0.49.19/weconnect_cupra_daern.egg-info/SOURCES.txt` & `weconnect-cupra-daern-0.49.20/weconnect_cupra_daern.egg-info/SOURCES.txt`

 * *Files identical despite different names*

