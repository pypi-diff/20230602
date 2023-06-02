# Comparing `tmp/SuperDuperMetroid-2.3.0.tar.gz` & `tmp/SuperDuperMetroid-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SuperDuperMetroid-2.3.0.tar", last modified: Mon Feb 28 05:20:58 2022, max compression
+gzip compressed data, was "SuperDuperMetroid-2.3.2.tar", last modified: Fri Jun  2 04:13:05 2023, max compression
```

## Comparing `SuperDuperMetroid-2.3.0.tar` & `SuperDuperMetroid-2.3.2.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-28 05:20:58.747832 SuperDuperMetroid-2.3.0/
--rw-r--r--   0 runner     (501) staff       (20)     1066 2022-02-28 05:18:31.000000 SuperDuperMetroid-2.3.0/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)       72 2022-02-28 05:18:31.000000 SuperDuperMetroid-2.3.0/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     2247 2022-02-28 05:20:58.748040 SuperDuperMetroid-2.3.0/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1704 2022-02-28 05:18:31.000000 SuperDuperMetroid-2.3.0/README.md
--rw-r--r--   0 runner     (501) staff       (20)      229 2022-02-28 05:18:34.000000 SuperDuperMetroid-2.3.0/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)      798 2022-02-28 05:20:58.749584 SuperDuperMetroid-2.3.0/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)      159 2022-02-28 05:18:34.000000 SuperDuperMetroid-2.3.0/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-28 05:20:58.707371 SuperDuperMetroid-2.3.0/src/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-28 05:20:58.716632 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-28 05:20:58.720618 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/BPSPatch/
--rw-r--r--   0 runner     (501) staff       (20)     9885 2022-02-28 05:18:34.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/BPSPatch/BPS_Patcher.pyx
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-02-28 05:18:34.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/BPSPatch/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3228 2022-02-28 05:18:34.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/IPS_Patcher.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-28 05:20:58.709548 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-28 05:20:58.720986 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Accessibility/
--rw-r--r--   0 runner     (501) staff       (20)     8995 2022-02-28 05:18:34.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Accessibility/colorblind.ips
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-28 05:20:58.726216 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Animals/
--rw-r--r--   0 runner     (501) staff       (20)      225 2022-02-28 05:18:34.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Animals/animal_enemies.ips
--rw-r--r--   0 runner     (501) staff       (20)      190 2022-02-28 05:18:34.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Animals/animals.ips
--rw-r--r--   0 runner     (501) staff       (20)      190 2022-02-28 05:18:34.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Animals/draygonimals.ips
--rw-r--r--   0 runner     (501) staff       (20)       69 2022-02-28 05:18:35.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Animals/escapimals.ips
--rw-r--r--   0 runner     (501) staff       (20)      209 2022-02-28 05:18:35.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Animals/grey_door_animals.ips
--rw-r--r--   0 runner     (501) staff       (20)       37 2022-02-28 05:18:35.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Animals/low_timer.ips
--rw-r--r--   0 runner     (501) staff       (20)      130 2022-02-28 05:18:35.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Animals/metalimals.ips
--rw-r--r--   0 runner     (501) staff       (20)      138 2022-02-28 05:18:35.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Animals/no_animals.ips
--rw-r--r--   0 runner     (501) staff       (20)      138 2022-02-28 05:18:35.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Animals/phantoonimals.ips
--rw-r--r--   0 runner     (501) staff       (20)      173 2022-02-28 05:18:35.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Animals/ridleyimals.ips
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-28 05:20:58.728357 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Fixes/
--rw-r--r--   0 runner     (501) staff       (20)       14 2022-02-28 05:18:35.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Fixes/disable_gt_code.ips
--rw-r--r--   0 runner     (501) staff       (20)       14 2022-02-28 05:18:35.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Fixes/fix_heat_echoes.ips
--rw-r--r--   0 runner     (501) staff       (20)       14 2022-02-28 05:18:35.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Fixes/fix_screw_attack_menu.ips
--rw-r--r--   0 runner     (501) staff       (20)       14 2022-02-28 05:18:35.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Fixes/fix_spacetime_beam.ips
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-28 05:20:58.730377 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Mandatory Patches/
--rw-r--r--   0 runner     (501) staff       (20)      145 2022-02-28 05:18:35.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Mandatory Patches/door_transition.ips
--rw-r--r--   0 runner     (501) staff       (20)      643 2022-02-28 05:18:35.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Mandatory Patches/seed_display.ips
--rw-r--r--   0 runner     (501) staff       (20)       36 2022-02-28 05:18:35.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Mandatory Patches/varia_rng.ips
--rw-r--r--   0 runner     (501) staff       (20)       52 2022-02-28 05:18:35.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Mandatory Patches/varia_timer_fix.ips
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-28 05:20:58.733795 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Map Changes/
--rw-r--r--   0 runner     (501) staff       (20)     2331 2022-02-28 05:18:35.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Map Changes/dachora_pit.ips
--rw-r--r--   0 runner     (501) staff       (20)      642 2022-02-28 05:18:36.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Map Changes/early_super_bridge.ips
--rw-r--r--   0 runner     (501) staff       (20)      689 2022-02-28 05:18:36.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Map Changes/moat.ips
--rw-r--r--   0 runner     (501) staff       (20)     1093 2022-02-28 05:18:36.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Map Changes/nova_boost_platform.ips
--rw-r--r--   0 runner     (501) staff       (20)      850 2022-02-28 05:18:36.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Map Changes/pre_high_jump.ips
--rw-r--r--   0 runner     (501) staff       (20)      660 2022-02-28 05:18:36.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Map Changes/pre_spazer.ips
--rw-r--r--   0 runner     (501) staff       (20)     2370 2022-02-28 05:18:36.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Map Changes/red_tower.ips
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-28 05:20:58.735586 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Music/
--rw-r--r--   0 runner     (501) staff       (20)      295 2022-02-28 05:18:36.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Music/custom_music.ips
--rw-r--r--   0 runner     (501) staff       (20)       14 2022-02-28 05:18:36.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Music/no_music.ips
--rw-r--r--   0 runner     (501) staff       (20)      288 2022-02-28 05:18:36.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Music/random_music.ips
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-28 05:20:58.739536 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/QoL/
--rw-r--r--   0 runner     (501) staff       (20)      169 2022-02-28 05:18:36.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/QoL/aim_any_button.ips
--rw-r--r--   0 runner     (501) staff       (20)      293 2022-02-28 05:18:36.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/QoL/better_decompress.ips
--rw-r--r--   0 runner     (501) staff       (20)       14 2022-02-28 05:18:36.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/QoL/enable_backup_saves.ips
--rw-r--r--   0 runner     (501) staff       (20)       14 2022-02-28 05:18:36.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/QoL/enable_moonwalk_by_default.ips
--rw-r--r--   0 runner     (501) staff       (20)      203 2022-02-28 05:18:36.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/QoL/fast_elevators_doors.ips
--rw-r--r--   0 runner     (501) staff       (20)       62 2022-02-28 05:18:36.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/QoL/g4_skip.ips
--rw-r--r--   0 runner     (501) staff       (20)      949 2022-02-28 05:18:36.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/QoL/max_ammo_display.ips
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-28 05:20:58.745521 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Tweaks/
--rw-r--r--   0 runner     (501) staff       (20)      179 2022-02-28 05:18:37.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Tweaks/cheap_charge.ips
--rw-r--r--   0 runner     (501) staff       (20)       15 2022-02-28 05:18:37.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Tweaks/infinite_space_jump.ips
--rw-r--r--   0 runner     (501) staff       (20)      217 2022-02-28 05:18:37.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Tweaks/mother_brain_cutscene_edits.ips
--rw-r--r--   0 runner     (501) staff       (20)       24 2022-02-28 05:18:37.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Tweaks/nerfed_rainbow_beam.ips
--rw-r--r--   0 runner     (501) staff       (20)       15 2022-02-28 05:18:37.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Tweaks/no_demo.ips
--rw-r--r--   0 runner     (501) staff       (20)       21 2022-02-28 05:18:37.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Tweaks/no_ln_chozo_inventory_check.ips
--rw-r--r--   0 runner     (501) staff       (20)      121 2022-02-28 05:18:37.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Tweaks/no_supers_on_red_doors.ips
--rw-r--r--   0 runner     (501) staff       (20)      177 2022-02-28 05:18:37.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Tweaks/refill_before_save.ips
--rw-r--r--   0 runner     (501) staff       (20)     3397 2022-02-28 05:18:37.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Tweaks/respin.ips
--rw-r--r--   0 runner     (501) staff       (20)      124 2022-02-28 05:18:37.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Tweaks/speed_keep.ips
--rw-r--r--   0 runner     (501) staff       (20)    60163 2022-02-28 05:18:37.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/ROM_Patcher.py
--rw-r--r--   0 runner     (501) staff       (20)    25236 2022-02-28 05:18:37.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/SM_Constants.py
--rw-r--r--   0 runner     (501) staff       (20)    45683 2022-02-28 05:18:37.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/SM_Interface.py
--rw-r--r--   0 runner     (501) staff       (20)    84426 2022-02-28 05:18:37.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/SM_Room_Header_Data.py
--rw-r--r--   0 runner     (501) staff       (20)     1024 2022-02-28 05:18:37.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/VramItems.bin
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-02-28 05:18:37.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-28 05:20:58.746899 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/__pyinstaller/
--rw-r--r--   0 runner     (501) staff       (20)      416 2022-02-28 05:18:37.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/__pyinstaller/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      218 2022-02-28 05:18:37.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/__pyinstaller/hook-SuperDuperMetroid.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-28 05:20:58.719688 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     2247 2022-02-28 05:20:58.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     3470 2022-02-28 05:20:58.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2022-02-28 05:20:58.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       74 2022-02-28 05:20:58.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid.egg-info/entry_points.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2022-02-28 05:20:20.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)       18 2022-02-28 05:20:58.000000 SuperDuperMetroid-2.3.0/src/SuperDuperMetroid.egg-info/top_level.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-28 05:20:58.747349 SuperDuperMetroid-2.3.0/test/
--rw-r--r--   0 runner     (501) staff       (20)     8930 2022-02-28 05:18:37.000000 SuperDuperMetroid-2.3.0/test/test_rom_patcher.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-02 04:13:05.771691 SuperDuperMetroid-2.3.2/
+-rw-r--r--   0 runner     (501) staff       (20)     1066 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)       72 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     2210 2023-06-02 04:13:05.771906 SuperDuperMetroid-2.3.2/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1704 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/README.md
+-rw-r--r--   0 runner     (501) staff       (20)      229 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)      798 2023-06-02 04:13:05.773015 SuperDuperMetroid-2.3.2/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)      159 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-02 04:13:05.724633 SuperDuperMetroid-2.3.2/src/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-02 04:13:05.736821 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-02 04:13:05.741324 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/BPSPatch/
+-rw-r--r--   0 runner     (501) staff       (20)     9885 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/BPSPatch/BPS_Patcher.pyx
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/BPSPatch/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3228 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/IPS_Patcher.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-02 04:13:05.727597 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-02 04:13:05.741781 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Accessibility/
+-rw-r--r--   0 runner     (501) staff       (20)     8995 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Accessibility/colorblind.ips
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-02 04:13:05.747983 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Animals/
+-rw-r--r--   0 runner     (501) staff       (20)      225 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Animals/animal_enemies.ips
+-rw-r--r--   0 runner     (501) staff       (20)      190 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Animals/animals.ips
+-rw-r--r--   0 runner     (501) staff       (20)      190 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Animals/draygonimals.ips
+-rw-r--r--   0 runner     (501) staff       (20)       69 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Animals/escapimals.ips
+-rw-r--r--   0 runner     (501) staff       (20)      209 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Animals/grey_door_animals.ips
+-rw-r--r--   0 runner     (501) staff       (20)       37 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Animals/low_timer.ips
+-rw-r--r--   0 runner     (501) staff       (20)      130 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Animals/metalimals.ips
+-rw-r--r--   0 runner     (501) staff       (20)      138 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Animals/no_animals.ips
+-rw-r--r--   0 runner     (501) staff       (20)      138 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Animals/phantoonimals.ips
+-rw-r--r--   0 runner     (501) staff       (20)      173 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Animals/ridleyimals.ips
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-02 04:13:05.750263 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Fixes/
+-rw-r--r--   0 runner     (501) staff       (20)       14 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Fixes/disable_gt_code.ips
+-rw-r--r--   0 runner     (501) staff       (20)       14 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Fixes/fix_heat_echoes.ips
+-rw-r--r--   0 runner     (501) staff       (20)       14 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Fixes/fix_screw_attack_menu.ips
+-rw-r--r--   0 runner     (501) staff       (20)       14 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Fixes/fix_spacetime_beam.ips
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-02 04:13:05.752626 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Mandatory Patches/
+-rw-r--r--   0 runner     (501) staff       (20)      145 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Mandatory Patches/door_transition.ips
+-rw-r--r--   0 runner     (501) staff       (20)      643 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Mandatory Patches/seed_display.ips
+-rw-r--r--   0 runner     (501) staff       (20)       36 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Mandatory Patches/varia_rng.ips
+-rw-r--r--   0 runner     (501) staff       (20)       52 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Mandatory Patches/varia_timer_fix.ips
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-02 04:13:05.756995 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Map Changes/
+-rw-r--r--   0 runner     (501) staff       (20)     2331 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Map Changes/dachora_pit.ips
+-rw-r--r--   0 runner     (501) staff       (20)      642 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Map Changes/early_super_bridge.ips
+-rw-r--r--   0 runner     (501) staff       (20)      689 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Map Changes/moat.ips
+-rw-r--r--   0 runner     (501) staff       (20)     1093 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Map Changes/nova_boost_platform.ips
+-rw-r--r--   0 runner     (501) staff       (20)      850 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Map Changes/pre_high_jump.ips
+-rw-r--r--   0 runner     (501) staff       (20)      660 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Map Changes/pre_spazer.ips
+-rw-r--r--   0 runner     (501) staff       (20)     2370 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Map Changes/red_tower.ips
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-02 04:13:05.758829 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Music/
+-rw-r--r--   0 runner     (501) staff       (20)      295 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Music/custom_music.ips
+-rw-r--r--   0 runner     (501) staff       (20)       14 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Music/no_music.ips
+-rw-r--r--   0 runner     (501) staff       (20)      288 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Music/random_music.ips
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-02 04:13:05.763093 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/QoL/
+-rw-r--r--   0 runner     (501) staff       (20)      169 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/QoL/aim_any_button.ips
+-rw-r--r--   0 runner     (501) staff       (20)      293 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/QoL/better_decompress.ips
+-rw-r--r--   0 runner     (501) staff       (20)       14 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/QoL/enable_backup_saves.ips
+-rw-r--r--   0 runner     (501) staff       (20)       14 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/QoL/enable_moonwalk_by_default.ips
+-rw-r--r--   0 runner     (501) staff       (20)      203 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/QoL/fast_elevators_doors.ips
+-rw-r--r--   0 runner     (501) staff       (20)       62 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/QoL/g4_skip.ips
+-rw-r--r--   0 runner     (501) staff       (20)      949 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/QoL/max_ammo_display.ips
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-02 04:13:05.769305 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Tweaks/
+-rw-r--r--   0 runner     (501) staff       (20)      179 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Tweaks/cheap_charge.ips
+-rw-r--r--   0 runner     (501) staff       (20)       15 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Tweaks/infinite_space_jump.ips
+-rw-r--r--   0 runner     (501) staff       (20)      217 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Tweaks/mother_brain_cutscene_edits.ips
+-rw-r--r--   0 runner     (501) staff       (20)       24 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Tweaks/nerfed_rainbow_beam.ips
+-rw-r--r--   0 runner     (501) staff       (20)       15 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Tweaks/no_demo.ips
+-rw-r--r--   0 runner     (501) staff       (20)       21 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Tweaks/no_ln_chozo_inventory_check.ips
+-rw-r--r--   0 runner     (501) staff       (20)      121 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Tweaks/no_supers_on_red_doors.ips
+-rw-r--r--   0 runner     (501) staff       (20)      177 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Tweaks/refill_before_save.ips
+-rw-r--r--   0 runner     (501) staff       (20)     3397 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Tweaks/respin.ips
+-rw-r--r--   0 runner     (501) staff       (20)      124 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Tweaks/speed_keep.ips
+-rw-r--r--   0 runner     (501) staff       (20)    60164 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/ROM_Patcher.py
+-rw-r--r--   0 runner     (501) staff       (20)    25236 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/SM_Constants.py
+-rw-r--r--   0 runner     (501) staff       (20)    45683 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/SM_Interface.py
+-rw-r--r--   0 runner     (501) staff       (20)    84426 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/SM_Room_Header_Data.py
+-rw-r--r--   0 runner     (501) staff       (20)     1024 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/VramItems.bin
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-02 04:13:05.770573 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/__pyinstaller/
+-rw-r--r--   0 runner     (501) staff       (20)      416 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/__pyinstaller/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      218 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/__pyinstaller/hook-SuperDuperMetroid.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-02 04:13:05.740086 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     2210 2023-06-02 04:13:05.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     3470 2023-06-02 04:13:05.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-06-02 04:13:05.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       74 2023-06-02 04:13:05.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid.egg-info/entry_points.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-06-02 04:12:25.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid.egg-info/not-zip-safe
+-rw-r--r--   0 runner     (501) staff       (20)       18 2023-06-02 04:13:05.000000 SuperDuperMetroid-2.3.2/src/SuperDuperMetroid.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-02 04:13:05.771216 SuperDuperMetroid-2.3.2/test/
+-rw-r--r--   0 runner     (501) staff       (20)     8931 2023-06-02 04:12:01.000000 SuperDuperMetroid-2.3.2/test/test_rom_patcher.py
```

### Comparing `SuperDuperMetroid-2.3.0/LICENSE` & `SuperDuperMetroid-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SuperDuperMetroid-2.3.0/PKG-INFO` & `SuperDuperMetroid-2.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: SuperDuperMetroid
-Version: 2.3.0
+Version: 2.3.2
 Summary: A Super Metroid patching utility
 Home-page: https://github.com/SolventMercury/Super-Duper-Metroid
 Author: Samuel Roy
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/SolventMercury/super-Duper-Metroid/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -36,9 +34,7 @@
 Credit goes to Samuel Roy for writing most of this code.  
 Kazuto wrote the More Efficient Item PLMs Hack, which is recreated in parts of this code.  
 Metroid Construction and Kejardon provided a lot of documentation which I made use of.  
 PHOSPHOTiDYL wrote the Skip Intro Saves hack, which is included in this program.  
 Smiley and Flo wrote the Cheap Charge IPS patch.  
 [n00btube](https://github.com/n00btube) wrote the Save Refill patch.  
 Total, Fusda, and Leodox were responsible for most of the other IPS patches.  
-
-
```

### Comparing `SuperDuperMetroid-2.3.0/README.md` & `SuperDuperMetroid-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `SuperDuperMetroid-2.3.0/setup.cfg` & `SuperDuperMetroid-2.3.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = SuperDuperMetroid
-version = 2.3.0
+version = 2.3.2
 author = Samuel Roy
 description = A Super Metroid patching utility
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/SolventMercury/Super-Duper-Metroid
 project_urls = 
 	Bug Tracker = https://github.com/SolventMercury/super-Duper-Metroid/issues
```

### Comparing `SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/BPSPatch/BPS_Patcher.pyx` & `SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/BPSPatch/BPS_Patcher.pyx`

 * *Files identical despite different names*

### Comparing `SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/IPS_Patcher.py` & `SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/IPS_Patcher.py`

 * *Files identical despite different names*

### Comparing `SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Accessibility/colorblind.ips` & `SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Accessibility/colorblind.ips`

 * *Files identical despite different names*

### Comparing `SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Mandatory Patches/seed_display.ips` & `SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Mandatory Patches/seed_display.ips`

 * *Files identical despite different names*

### Comparing `SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Map Changes/dachora_pit.ips` & `SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Map Changes/dachora_pit.ips`

 * *Files identical despite different names*

### Comparing `SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Map Changes/early_super_bridge.ips` & `SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Map Changes/early_super_bridge.ips`

 * *Files identical despite different names*

### Comparing `SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Map Changes/moat.ips` & `SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Map Changes/moat.ips`

 * *Files identical despite different names*

### Comparing `SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Map Changes/nova_boost_platform.ips` & `SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Map Changes/nova_boost_platform.ips`

 * *Files identical despite different names*

### Comparing `SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Map Changes/pre_high_jump.ips` & `SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Map Changes/pre_high_jump.ips`

 * *Files identical despite different names*

### Comparing `SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Map Changes/pre_spazer.ips` & `SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Map Changes/pre_spazer.ips`

 * *Files identical despite different names*

### Comparing `SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Map Changes/red_tower.ips` & `SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Map Changes/red_tower.ips`

 * *Files identical despite different names*

### Comparing `SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/QoL/max_ammo_display.ips` & `SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/QoL/max_ammo_display.ips`

 * *Files identical despite different names*

### Comparing `SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/Patches/Tweaks/respin.ips` & `SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/Patches/Tweaks/respin.ips`

 * *Files identical despite different names*

### Comparing `SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/ROM_Patcher.py` & `SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/ROM_Patcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,14 +315,15 @@
         self.owner_name = owner_name
         self.graphics_file_name = graphics_filename
         self.native_sprite_name = native_sprite_name
 
 
 # class PickupEffect(Enum):
 
+
 # Converts a hexadecimal string to a base 10 integer.
 def hex_to_int(hex_to_convert):
     return int(hex_to_convert, 16)
 
 
 # Converts an integer to a hexadecimal string.
 def int_to_hex(int_to_convert):
```

### Comparing `SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/SM_Constants.py` & `SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/SM_Constants.py`

 * *Files identical despite different names*

### Comparing `SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/SM_Interface.py` & `SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/SM_Interface.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 import sys
 import threading
 import time
 
 from SuperDuperMetroid.SM_Constants import SuperMetroidConstants
 from websocket import create_connection
 
+
 # Converts a hexadecimal string to a base 10 integer.
 def hex_to_int(hex_to_convert):
     return int(hex_to_convert, 16)
 
 
 # Converts an integer to a hexadecimal string.
 def int_to_hex(int_to_convert):
@@ -77,15 +78,14 @@
     return_hex = hex_to_pad
     while len(return_hex) < num_hex_characters:
         return_hex = "0" + return_hex
     return return_hex
 
 
 class SuperMetroidInterface:
-
     # These get imported dynamically from a JSON file created by the patcher.
     # This is necessary because these may not always be in the same place every game.
     itemRoutineDict = {
         "Energy Tank": None,
         "Missile Expansion": None,
         "Super Missile Expansion": None,
         "Power Bomb Expansion": None,
```

### Comparing `SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/SM_Room_Header_Data.py` & `SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/SM_Room_Header_Data.py`

 * *Files identical despite different names*

### Comparing `SuperDuperMetroid-2.3.0/src/SuperDuperMetroid/VramItems.bin` & `SuperDuperMetroid-2.3.2/src/SuperDuperMetroid/VramItems.bin`

 * *Files identical despite different names*

### Comparing `SuperDuperMetroid-2.3.0/src/SuperDuperMetroid.egg-info/PKG-INFO` & `SuperDuperMetroid-2.3.2/src/SuperDuperMetroid.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: SuperDuperMetroid
-Version: 2.3.0
+Version: 2.3.2
 Summary: A Super Metroid patching utility
 Home-page: https://github.com/SolventMercury/Super-Duper-Metroid
 Author: Samuel Roy
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/SolventMercury/super-Duper-Metroid/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -36,9 +34,7 @@
 Credit goes to Samuel Roy for writing most of this code.  
 Kazuto wrote the More Efficient Item PLMs Hack, which is recreated in parts of this code.  
 Metroid Construction and Kejardon provided a lot of documentation which I made use of.  
 PHOSPHOTiDYL wrote the Skip Intro Saves hack, which is included in this program.  
 Smiley and Flo wrote the Cheap Charge IPS patch.  
 [n00btube](https://github.com/n00btube) wrote the Save Refill patch.  
 Total, Fusda, and Leodox were responsible for most of the other IPS patches.  
-
-
```

### Comparing `SuperDuperMetroid-2.3.0/src/SuperDuperMetroid.egg-info/SOURCES.txt` & `SuperDuperMetroid-2.3.2/src/SuperDuperMetroid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SuperDuperMetroid-2.3.0/test/test_rom_patcher.py` & `SuperDuperMetroid-2.3.2/test/test_rom_patcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from SuperDuperMetroid import ROM_Patcher
 
 romSize = 3145728
 
+
 # endAddress is excluded
 def is_file_byte_range_empty(f, empty_byte, start_address, end_address):
     found_non_empty_byte = False
     f.seek(start_address)
     bytes = f.read(end_address - start_address)
     for byte in bytes:
         if byte != empty_byte[0]:
```

