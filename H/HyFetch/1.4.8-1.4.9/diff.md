# Comparing `tmp/HyFetch-1.4.8.tar.gz` & `tmp/HyFetch-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HyFetch-1.4.8.tar", last modified: Sun Apr  2 01:16:40 2023, max compression
+gzip compressed data, was "HyFetch-1.4.9.tar", last modified: Fri Jun  2 07:31:03 2023, max compression
```

## Comparing `HyFetch-1.4.8.tar` & `HyFetch-1.4.9.tar`

### file list

```diff
@@ -1,401 +1,387 @@
-drwxr-xr-x   0 azalea    (1000) azalea    (1000)        0 2023-04-02 01:16:40.013063 HyFetch-1.4.8/
--rw-r--r--   0 azalea    (1000) azalea    (1000)       66 2022-08-06 02:38:59.000000 HyFetch-1.4.8/.gitattributes
-drwxr-xr-x   0 azalea    (1000) azalea    (1000)        0 2023-04-02 01:16:39.513058 HyFetch-1.4.8/.github/
--rw-r--r--   0 azalea    (1000) azalea    (1000)      355 2023-02-12 04:32:19.000000 HyFetch-1.4.8/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 azalea    (1000) azalea    (1000)       93 2023-02-12 04:32:19.000000 HyFetch-1.4.8/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 azalea    (1000) azalea    (1000)        0 2023-04-02 01:16:39.513058 HyFetch-1.4.8/.github/workflows/
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1836 2022-08-14 04:01:03.000000 HyFetch-1.4.8/.github/workflows/arch_package.yml
--rw-r--r--   0 azalea    (1000) azalea    (1000)     3639 2022-08-18 04:59:31.000000 HyFetch-1.4.8/.github/workflows/release.yml
--rw-r--r--   0 azalea    (1000) azalea    (1000)      460 2022-08-12 03:31:22.000000 HyFetch-1.4.8/.github/workflows/shellcheck.yml
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1325 2023-01-21 00:38:29.000000 HyFetch-1.4.8/.gitignore
-drwxr-xr-x   0 azalea    (1000) azalea    (1000)        0 2023-04-02 01:16:39.516391 HyFetch-1.4.8/.vscode/
--rw-r--r--   0 azalea    (1000) azalea    (1000)      443 2023-02-07 23:20:38.000000 HyFetch-1.4.8/.vscode/launch.json
--rw-r--r--   0 azalea    (1000) azalea    (1000)     3877 2023-02-12 04:32:19.000000 HyFetch-1.4.8/CONTRIBUTING.md
-drwxr-xr-x   0 azalea    (1000) azalea    (1000)        0 2023-04-02 01:16:39.516391 HyFetch-1.4.8/HyFetch.egg-info/
--rwxrwxr-x   0 azalea    (1000) azalea    (1000)    30431 2023-04-02 01:16:39.000000 HyFetch-1.4.8/HyFetch.egg-info/PKG-INFO
--rwxrwxr-x   0 azalea    (1000) azalea    (1000)    10670 2023-04-02 01:16:39.000000 HyFetch-1.4.8/HyFetch.egg-info/SOURCES.txt
--rwxrwxr-x   0 azalea    (1000) azalea    (1000)        1 2023-04-02 01:16:39.000000 HyFetch-1.4.8/HyFetch.egg-info/dependency_links.txt
--rwxrwxr-x   0 azalea    (1000) azalea    (1000)       45 2023-04-02 01:16:39.000000 HyFetch-1.4.8/HyFetch.egg-info/entry_points.txt
--rwxrwxr-x   0 azalea    (1000) azalea    (1000)       85 2023-04-02 01:16:39.000000 HyFetch-1.4.8/HyFetch.egg-info/requires.txt
--rwxrwxr-x   0 azalea    (1000) azalea    (1000)       25 2023-04-02 01:16:39.000000 HyFetch-1.4.8/HyFetch.egg-info/top_level.txt
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1083 2023-02-12 04:32:19.000000 HyFetch-1.4.8/LICENSE.md
--rw-r--r--   0 azalea    (1000) azalea    (1000)       26 2022-08-06 02:38:59.000000 HyFetch-1.4.8/MANIFEST.in
--rw-r--r--   0 azalea    (1000) azalea    (1000)      418 2023-02-12 04:32:19.000000 HyFetch-1.4.8/Makefile
--rw-r--r--   0 azalea    (1000) azalea    (1000)    30431 2023-04-02 01:16:40.013063 HyFetch-1.4.8/PKG-INFO
--rw-r--r--   0 azalea    (1000) azalea    (1000)    29821 2023-04-02 01:13:29.000000 HyFetch-1.4.8/README.md
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1283 2022-05-02 07:33:01.000000 HyFetch-1.4.8/default.nix
-drwxr-xr-x   0 azalea    (1000) azalea    (1000)        0 2023-04-02 01:16:39.516391 HyFetch-1.4.8/hyfetch/
--rw-r--r--   0 azalea    (1000) azalea    (1000)      143 2022-08-14 04:02:38.000000 HyFetch-1.4.8/hyfetch/__init__.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)       68 2022-08-23 15:01:05.000000 HyFetch-1.4.8/hyfetch/__main__.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)       18 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/__version__.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     2063 2022-08-06 02:38:59.000000 HyFetch-1.4.8/hyfetch/color_scale.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     7258 2023-03-21 03:30:16.000000 HyFetch-1.4.8/hyfetch/color_util.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1272 2023-04-02 01:10:55.000000 HyFetch-1.4.8/hyfetch/constants.py
-drwxr-xr-x   0 azalea    (1000) azalea    (1000)        0 2023-04-02 01:16:40.009729 HyFetch-1.4.8/hyfetch/distros/
--rw-r--r--   0 azalea    (1000) azalea    (1000)      510 2022-12-12 02:30:50.000000 HyFetch-1.4.8/hyfetch/distros/__init__.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      910 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/aix.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1023 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/almalinux.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      941 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/alpine.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      284 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/alpine_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      849 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/alter.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      906 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/amazon.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      756 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/amogos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1698 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/anarchy.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      699 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/android.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      293 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/android_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1070 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/antergos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      527 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/antix.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      911 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/aosc_os.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      954 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/aosc_os_retro.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      423 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/aoscosretro_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      238 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/aperio_gnu_linux.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      911 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/aperture.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      669 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/apricity.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      782 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/arch.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      761 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/arch_old.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      265 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/arch_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      913 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/archbox.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     3001 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/archcraft.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      846 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/archcraft_ascii.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1413 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/archcraft_minimal.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1030 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/archlabs.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      796 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/archmerge.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      919 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/archstrike.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      876 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/arcolinux.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      402 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/arcolinux_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1753 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/arselinux.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      776 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/artix.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      441 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/artix_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      813 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/arya.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1054 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/asahi.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      748 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/aster.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      810 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/asteroidos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      921 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/astos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      942 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/bedrock.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      904 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/biglinux.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      408 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/bitrig.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1021 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/blackarch.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     2631 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/blackpanther.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      599 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/blag.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1033 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/blankon.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1102 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/bluelight.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1170 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/bodhi.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      578 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/bonsai.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      746 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/bsd.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      495 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/bunsenlabs.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1617 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/cachyos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1068 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/calculate.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     3962 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/calinixos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1583 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/calinixos_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      538 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/carbs.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      737 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/cbl_mariner.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1114 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/celos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      485 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/center.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      969 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/centos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      344 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/centos_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      735 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/chakra.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      913 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/chaletos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      834 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/chapeau.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      949 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/chonkysealos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1026 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/chrom.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      824 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/cleanjaro.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      425 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/cleanjaro_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      752 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/clear_linux_os.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      901 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/clearos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      871 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/clover.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      887 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/cobalt.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1105 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/condres.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1094 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/container_linux_by_coreos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      748 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/crux.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      340 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/crux_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      833 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/crystal_linux.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1104 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/cucumber.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      510 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/cutefishos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      724 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/cuteos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      799 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/cyberos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      726 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/dahlia.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     2786 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/darkos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      664 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/darwin.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      574 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/debian.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      225 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/debian_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      795 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/deepin.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1274 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/desaos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      547 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/devuan.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      842 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/dietpi.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)    38316 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/distro_detector.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      531 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/dracos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      662 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/dragonfly.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      865 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/dragonfly_old.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      286 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/dragonfly_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      692 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/drauger.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      529 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/droidian.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      745 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/elementary.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      257 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/elementary_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1108 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/elive.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      608 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/encryptos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      908 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/endeavouros.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      923 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/endless.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      874 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/enso.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      741 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/eurolinux.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1137 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/exherbo.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1159 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/exodia_predator_os.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1025 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/fedora.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      876 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/fedora_old.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      300 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/fedora_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      652 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/feren.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      699 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/finnix.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     2114 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/floflis.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      775 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/freebsd.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      263 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/freebsd_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      608 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/freemint.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1220 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/frugalware.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      568 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/funtoo.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1024 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/galliumos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      895 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/garuda.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      280 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/garuda_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      888 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/gentoo.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      252 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/gentoo_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      363 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/ghostbsd.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      580 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/glaucus.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      713 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/gnewsense.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      846 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/gnome.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      691 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/gnu.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      314 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/gobolinux.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1005 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/grapheneos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      897 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/grombyang.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      442 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/guix.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      289 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/guix_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      619 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/haiku.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      299 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/haiku_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1066 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/hamonikr.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1144 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/hardclanz.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      441 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/hash.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      755 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/huayra.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      918 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/hybrid.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      478 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/hydroos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      693 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/hyperbola.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      261 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/hyperbola_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      365 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/iglunix.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      829 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/instantos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      866 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/irix.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      654 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/itc.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1117 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/januslinux.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      816 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/kaisen.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      950 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/kali.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      406 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/kali_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      645 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/kaos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      860 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/kde.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      729 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/kibojoe.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      710 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/kogaion.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      822 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/korora.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1373 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/krassos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      424 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/kslinux.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1192 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/kubuntu.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      617 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/langitketujuh.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      803 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/langitketujuh_old.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      798 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/laxeros.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      320 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/lede.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1164 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/libreelec.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1018 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/linspire.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      589 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/linux.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      521 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/linux_lite.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1060 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/linux_mint.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      890 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/linux_mint_old.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      275 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/linuxlite_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      327 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/linuxmint_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      742 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/live_raizo.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      714 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/lmde.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1200 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/lubuntu.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      590 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/lunar.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      669 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/mac.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      293 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/mac_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      606 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/mageia.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      235 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/mageia_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      898 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/magpieos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      795 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/mandriva.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1247 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/manjaro.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      286 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/manjaro_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      700 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/massos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     2715 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/matuusos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      895 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/maui.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1073 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/mer.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      815 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/minix.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      546 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/miracle_linux.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      858 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/mx.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      247 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/mx_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      927 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/namib.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1020 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/nekos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      804 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/neptune.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      577 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/netbsd.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      323 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/netbsd_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      928 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/netrunner.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      504 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/nitrux.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1825 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/nixos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     2066 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/nixos_old.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      267 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/nixos_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      497 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/nomadbsd.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      765 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/nurunner.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      883 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/nutyx.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      679 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/obarun.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      560 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/obrevenge.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      489 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/omnios.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      962 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/open_source_media_center.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1010 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/openbsd.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      298 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/openbsd_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1213 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/openeuler.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      761 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/openindiana.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      990 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/openmamba.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      999 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/openmandriva.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      694 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/openstage.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      999 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/opensuse.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      714 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/opensuse_leap.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      279 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/opensuse_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      878 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/opensuse_tumbleweed.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      369 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/openwrt.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1053 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/opnsense.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      545 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/oracle.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1541 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/orchid.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      890 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/orchid_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1063 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/os_elbrus.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1123 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/pacbsd.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      718 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/parabola.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      265 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/parabola_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1671 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/parch.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      851 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/pardus.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      898 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/parrot.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1167 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/parsix.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1130 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/pcbsd.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      888 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/pclinuxos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      744 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/pearos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      696 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/pengwin.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1074 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/pentoo.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1609 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/peppermint.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      699 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/pikaos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1038 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/pisi.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1184 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/pnm_linux.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1176 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/pop__os.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      316 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/popos_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      669 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/porteus.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      692 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/postmarketos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      325 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/postmarketos_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      890 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/profelis_sambabox.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1113 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/proxmox.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      518 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/puffos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      829 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/puppy.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      661 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/pureos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      276 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/pureos_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      895 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/q4os.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      946 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/qubes.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1007 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/qubyt.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      860 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/quibian.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      538 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/radix.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      924 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/raspbian.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      309 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/raspbian_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      885 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/ravynos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      951 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/reborn_os.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      793 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/red_star.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      725 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/redcore.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      829 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/redhat.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      748 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/redhat_old.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      759 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/refracted_devuan.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1222 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/regata.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      769 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/regolith.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      604 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/rhaymos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      781 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/rocky.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      464 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/rocky_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      901 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/rosa.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      878 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/sabayon.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      562 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/sabotage.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      442 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/sailfish.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1175 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/salentos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      927 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/salient_os.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1006 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/sasanqua.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      893 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/scientific.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      338 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/semc.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1134 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/septor.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      965 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/serene.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      682 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/sharklinux.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      798 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/shastraos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      806 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/siduction.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      591 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/skiffos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1217 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/slackware.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      277 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/slackware_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      803 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/slitaz.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      781 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/smartos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      709 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/soda.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      872 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/solus.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      748 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/source_mage.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      891 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/sparky.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      781 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/star.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      797 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/steamos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      789 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/stock_linux.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      832 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/sulin.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      421 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/sunos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      307 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/sunos_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      857 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/swagarch.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      287 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/t2.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      635 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/tails.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      935 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/tearch.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1946 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/torizoncore.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      748 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/trisquel.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1671 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/twister.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      996 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/ubuntu.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      958 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/ubuntu_budgie.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1244 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/ubuntu_cinnamon.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      722 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/ubuntu_gnome.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1305 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/ubuntu_kylin.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1414 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/ubuntu_mate.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1184 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/ubuntu_old.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      989 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/ubuntu_old02.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      406 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/ubuntu_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1320 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/ubuntu_studio.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1345 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/ubuntu_sway.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      410 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/ubuntu_touch.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1066 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/ultramarine_linux.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      816 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/univalent.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1244 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/univention.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1091 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/uos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1156 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/urukos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1171 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/uwuntu.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1016 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/vanilla.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      531 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/venom.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      933 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/vnux.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1704 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/void.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      266 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/void_small.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      921 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/vzlinux.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1271 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/wii_linux_ngx.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      839 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/windows.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      905 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/windows_10.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      724 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/windows_11.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      818 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/xferience.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1140 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/xubuntu.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      871 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/yiffos.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      654 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/distros/zorin.py
--rwxr-xr-x   0 azalea    (1000) azalea    (1000)    14187 2023-03-21 03:30:18.000000 HyFetch-1.4.8/hyfetch/main.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      856 2023-03-21 03:30:16.000000 HyFetch-1.4.8/hyfetch/models.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)    12607 2023-03-21 03:30:18.000000 HyFetch-1.4.8/hyfetch/neofetch_util.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)    14720 2023-03-21 19:57:23.000000 HyFetch-1.4.8/hyfetch/presets.py
-drwxr-xr-x   0 azalea    (1000) azalea    (1000)        0 2023-04-02 01:16:40.013063 HyFetch-1.4.8/hyfetch/scripts/
--rwxr-xr-x   0 azalea    (1000) azalea    (1000)   494485 2023-04-02 01:13:29.000000 HyFetch-1.4.8/hyfetch/scripts/neowofetch
--rw-r--r--   0 azalea    (1000) azalea    (1000)     1353 2022-08-06 02:38:59.000000 HyFetch-1.4.8/hyfetch/serializer.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     4729 2022-12-05 05:46:28.000000 HyFetch-1.4.8/hyfetch/termenv.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      284 2022-12-12 02:30:50.000000 HyFetch-1.4.8/hyfetch/types.py
--rwxr-xr-x   0 azalea    (1000) azalea    (1000)   494485 2023-04-02 01:13:29.000000 HyFetch-1.4.8/neofetch
--rw-r--r--   0 azalea    (1000) azalea    (1000)    13972 2023-04-02 01:13:29.000000 HyFetch-1.4.8/neofetch.1
--rw-r--r--   0 azalea    (1000) azalea    (1000)      569 2023-04-02 01:13:29.000000 HyFetch-1.4.8/package.json
--rwxr-xr-x   0 azalea    (1000) azalea    (1000)       90 2022-08-06 02:38:59.000000 HyFetch-1.4.8/runner.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)       38 2023-04-02 01:16:40.013063 HyFetch-1.4.8/setup.cfg
--rwxr-xr-x   0 azalea    (1000) azalea    (1000)     1513 2023-03-24 03:58:17.000000 HyFetch-1.4.8/setup.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     2183 2022-10-26 14:33:08.000000 HyFetch-1.4.8/test.py
-drwxr-xr-x   0 azalea    (1000) azalea    (1000)        0 2023-04-02 01:16:40.013063 HyFetch-1.4.8/tools/
--rwxr-xr-x   0 azalea    (1000) azalea    (1000)     3440 2023-02-02 17:38:01.000000 HyFetch-1.4.8/tools/accept_upstream.py
--rwxr-xr-x   0 azalea    (1000) azalea    (1000)     1034 2023-03-21 03:30:16.000000 HyFetch-1.4.8/tools/colors_test.py
--rwxr-xr-x   0 azalea    (1000) azalea    (1000)     5303 2023-04-02 01:16:17.000000 HyFetch-1.4.8/tools/deploy-release.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      625 2022-09-06 15:41:47.000000 HyFetch-1.4.8/tools/deploy.md
--rwxr-xr-x   0 azalea    (1000) azalea    (1000)      206 2022-10-04 17:09:48.000000 HyFetch-1.4.8/tools/deploy.sh
--rwxr-xr-x   0 azalea    (1000) azalea    (1000)      988 2022-12-05 05:46:28.000000 HyFetch-1.4.8/tools/issue_fixed.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)      580 2023-01-14 21:25:02.000000 HyFetch-1.4.8/tools/issue_whitelist.py
--rwxr-xr-x   0 azalea    (1000) azalea    (1000)     5243 2023-02-11 04:29:44.000000 HyFetch-1.4.8/tools/list_distros.py
--rwxr-xr-x   0 azalea    (1000) azalea    (1000)     2640 2022-08-12 03:11:03.000000 HyFetch-1.4.8/tools/list_unresolved.py
--rw-r--r--   0 azalea    (1000) azalea    (1000)     2259 2022-12-05 05:46:28.000000 HyFetch-1.4.8/tools/pull_request_markings.yaml
--rwxr-xr-x   0 azalea    (1000) azalea    (1000)      641 2023-02-21 14:54:52.000000 HyFetch-1.4.8/tools/reformat_readme.py
+drwxr-xr-x   0 azalea    (1000) azalea    (1000)        0 2023-06-02 07:31:03.034356 HyFetch-1.4.9/
+drwxr-xr-x   0 azalea    (1000) azalea    (1000)        0 2023-06-02 07:31:03.004356 HyFetch-1.4.9/HyFetch.egg-info/
+-rw-r--r--   0 azalea    (1000) azalea    (1000)    32011 2023-06-02 07:31:02.000000 HyFetch-1.4.9/HyFetch.egg-info/PKG-INFO
+-rw-r--r--   0 azalea    (1000) azalea    (1000)    10559 2023-06-02 07:31:02.000000 HyFetch-1.4.9/HyFetch.egg-info/SOURCES.txt
+-rw-r--r--   0 azalea    (1000) azalea    (1000)        1 2023-06-02 07:31:02.000000 HyFetch-1.4.9/HyFetch.egg-info/dependency_links.txt
+-rw-r--r--   0 azalea    (1000) azalea    (1000)       45 2023-06-02 07:31:02.000000 HyFetch-1.4.9/HyFetch.egg-info/entry_points.txt
+-rw-r--r--   0 azalea    (1000) azalea    (1000)       85 2023-06-02 07:31:02.000000 HyFetch-1.4.9/HyFetch.egg-info/requires.txt
+-rw-r--r--   0 azalea    (1000) azalea    (1000)       25 2023-06-02 07:31:02.000000 HyFetch-1.4.9/HyFetch.egg-info/top_level.txt
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1083 2023-05-16 03:13:08.000000 HyFetch-1.4.9/LICENSE.md
+-rw-r--r--   0 azalea    (1000) azalea    (1000)       26 2022-09-24 20:22:01.000000 HyFetch-1.4.9/MANIFEST.in
+-rw-r--r--   0 azalea    (1000) azalea    (1000)    32011 2023-06-02 07:31:03.034356 HyFetch-1.4.9/PKG-INFO
+-rw-r--r--   0 azalea    (1000) azalea    (1000)    31401 2023-06-02 07:26:04.000000 HyFetch-1.4.9/README.md
+drwxr-xr-x   0 azalea    (1000) azalea    (1000)        0 2023-06-02 07:31:03.004356 HyFetch-1.4.9/hyfetch/
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      143 2022-09-24 20:22:01.000000 HyFetch-1.4.9/hyfetch/__init__.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)       68 2022-09-24 20:22:01.000000 HyFetch-1.4.9/hyfetch/__main__.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)       18 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/__version__.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     2063 2022-09-24 20:22:01.000000 HyFetch-1.4.9/hyfetch/color_scale.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     7605 2023-06-02 04:54:20.000000 HyFetch-1.4.9/hyfetch/color_util.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1313 2023-06-02 06:55:43.000000 HyFetch-1.4.9/hyfetch/constants.py
+drwxr-xr-x   0 azalea    (1000) azalea    (1000)        0 2023-06-02 07:31:03.034356 HyFetch-1.4.9/hyfetch/distros/
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      510 2022-12-12 19:58:21.000000 HyFetch-1.4.9/hyfetch/distros/__init__.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      910 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/aix.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1023 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/almalinux.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      941 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/alpine.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      284 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/alpine_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      849 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/alter.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      906 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/amazon.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      756 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/amogos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1698 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/anarchy.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      699 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/android.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      293 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/android_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1070 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/antergos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      527 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/antix.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      911 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/aosc_os.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      954 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/aosc_os_retro.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      423 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/aoscosretro_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      238 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/aperio_gnu_linux.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      911 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/aperture.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      669 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/apricity.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      782 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/arch.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      761 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/arch_old.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      265 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/arch_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      913 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/archbox.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     3001 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/archcraft.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      846 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/archcraft_ascii.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1413 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/archcraft_minimal.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1030 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/archlabs.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      796 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/archmerge.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      919 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/archstrike.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      876 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/arcolinux.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      402 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/arcolinux_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1753 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/arselinux.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      776 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/artix.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      441 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/artix_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      813 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/arya.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1054 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/asahi.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      748 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/aster.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      810 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/asteroidos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      921 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/astos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1594 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/astra_linux.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      942 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/bedrock.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      904 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/biglinux.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      408 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/bitrig.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1021 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/blackarch.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     2631 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/blackpanther.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      599 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/blag.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1033 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/blankon.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1102 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/bluelight.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1170 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/bodhi.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      578 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/bonsai.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      746 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/bsd.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      495 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/bunsenlabs.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1617 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/cachyos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1068 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/calculate.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     3962 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/calinixos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1583 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/calinixos_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      538 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/carbs.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      737 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/cbl_mariner.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1114 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/celos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      485 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/center.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      969 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/centos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      344 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/centos_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      735 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/chakra.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      913 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/chaletos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      834 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/chapeau.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      949 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/chonkysealos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1026 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/chrom.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      824 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/cleanjaro.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      425 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/cleanjaro_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      752 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/clear_linux_os.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      901 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/clearos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      871 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/clover.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      887 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/cobalt.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1105 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/condres.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1094 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/container_linux_by_coreos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      748 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/crux.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      340 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/crux_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      833 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/crystal_linux.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1104 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/cucumber.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      510 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/cutefishos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      724 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/cuteos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      799 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/cyberos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      726 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/dahlia.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     2786 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/darkos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      664 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/darwin.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      574 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/debian.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      225 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/debian_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      795 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/deepin.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1274 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/desaos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      547 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/devuan.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      842 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/dietpi.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)    38632 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/distro_detector.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      531 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/dracos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      662 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/dragonfly.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      865 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/dragonfly_old.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      286 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/dragonfly_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      692 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/drauger.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      529 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/droidian.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      745 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/elementary.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      257 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/elementary_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1108 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/elive.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      608 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/encryptos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      908 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/endeavouros.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      923 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/endless.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      874 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/enso.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      741 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/eurolinux.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1137 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/exherbo.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1159 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/exodia_predator_os.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1025 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/fedora.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      876 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/fedora_old.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      300 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/fedora_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      989 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/femboyos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      652 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/feren.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      699 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/finnix.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     2114 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/floflis.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      775 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/freebsd.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      263 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/freebsd_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      608 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/freemint.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1220 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/frugalware.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      568 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/funtoo.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1024 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/galliumos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      895 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/garuda.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      280 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/garuda_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      888 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/gentoo.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      252 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/gentoo_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      363 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/ghostbsd.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      580 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/glaucus.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      713 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/gnewsense.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      846 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/gnome.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      691 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/gnu.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      314 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/gobolinux.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1005 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/grapheneos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      897 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/grombyang.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      442 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/guix.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      289 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/guix_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      619 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/haiku.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      299 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/haiku_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1066 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/hamonikr.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1144 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/hardclanz.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      441 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/hash.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      755 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/huayra.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      918 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/hybrid.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      478 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/hydroos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      693 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/hyperbola.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      261 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/hyperbola_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      365 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/iglunix.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      829 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/instantos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      866 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/irix.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      654 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/itc.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1117 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/januslinux.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      816 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/kaisen.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      950 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/kali.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      406 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/kali_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      645 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/kaos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      860 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/kde.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      729 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/kibojoe.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      710 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/kogaion.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      822 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/korora.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1373 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/krassos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      424 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/kslinux.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1192 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/kubuntu.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      617 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/langitketujuh.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      803 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/langitketujuh_old.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      798 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/laxeros.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      320 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/lede.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1164 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/libreelec.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1018 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/linspire.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      589 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/linux.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      521 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/linux_lite.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1060 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/linux_mint.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      890 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/linux_mint_old.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      275 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/linuxlite_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      327 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/linuxmint_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      742 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/live_raizo.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      714 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/lmde.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1200 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/lubuntu.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      590 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/lunar.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      669 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/mac.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      293 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/mac_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      606 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/mageia.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      235 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/mageia_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      898 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/magpieos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      795 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/mandriva.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1247 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/manjaro.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      286 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/manjaro_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      700 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/massos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     2715 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/matuusos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      895 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/maui.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1073 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/mer.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      815 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/minix.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      546 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/miracle_linux.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      858 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/mx.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      247 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/mx_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      927 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/namib.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1020 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/nekos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      804 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/neptune.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      577 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/netbsd.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      323 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/netbsd_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      928 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/netrunner.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      504 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/nitrux.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1825 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/nixos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     2066 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/nixos_old.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      267 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/nixos_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     2359 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/nobara.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      497 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/nomadbsd.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      765 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/nurunner.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      883 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/nutyx.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      679 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/obarun.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      560 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/obrevenge.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      489 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/omnios.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      962 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/open_source_media_center.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1010 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/openbsd.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      298 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/openbsd_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1213 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/openeuler.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      761 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/openindiana.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      990 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/openmamba.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      999 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/openmandriva.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      694 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/openstage.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      999 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/opensuse.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      714 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/opensuse_leap.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      279 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/opensuse_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      878 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/opensuse_tumbleweed.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      369 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/openwrt.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1053 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/opnsense.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      545 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/oracle.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1541 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/orchid.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      890 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/orchid_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1063 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/os_elbrus.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1123 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/pacbsd.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      718 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/parabola.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      265 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/parabola_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1671 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/parch.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      851 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/pardus.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      898 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/parrot.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1167 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/parsix.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1130 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/pcbsd.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      888 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/pclinuxos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      744 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/pearos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      696 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/pengwin.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1074 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/pentoo.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1609 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/peppermint.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      699 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/pikaos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1038 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/pisi.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1184 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/pnm_linux.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1176 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/pop__os.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      316 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/popos_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      669 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/porteus.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      692 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/postmarketos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      325 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/postmarketos_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      890 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/profelis_sambabox.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1113 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/proxmox.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      518 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/puffos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      829 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/puppy.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      661 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/pureos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      276 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/pureos_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      895 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/q4os.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      946 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/qubes.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1007 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/qubyt.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      860 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/quibian.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      538 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/radix.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      924 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/raspbian.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      309 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/raspbian_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      885 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/ravynos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      951 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/reborn_os.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      793 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/red_star.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      725 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/redcore.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      829 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/redhat.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      748 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/redhat_old.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      759 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/refracted_devuan.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1222 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/regata.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      769 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/regolith.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      604 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/rhaymos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      781 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/rocky.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      464 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/rocky_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      901 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/rosa.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      878 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/sabayon.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      562 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/sabotage.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      442 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/sailfish.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1175 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/salentos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      927 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/salient_os.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1006 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/sasanqua.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      893 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/scientific.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      338 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/semc.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1134 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/septor.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      965 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/serene.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      682 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/sharklinux.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      798 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/shastraos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      806 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/siduction.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      591 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/skiffos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1217 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/slackware.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      277 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/slackware_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      803 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/slitaz.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      781 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/smartos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      709 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/soda.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      872 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/solus.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      748 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/source_mage.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      891 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/sparky.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      781 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/star.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      797 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/steamos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      789 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/stock_linux.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      832 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/sulin.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      421 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/sunos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      307 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/sunos_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      857 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/swagarch.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      287 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/t2.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      635 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/tails.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      935 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/tearch.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1946 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/torizoncore.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      748 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/trisquel.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1671 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/twister.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      996 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/ubuntu.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      958 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/ubuntu_budgie.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1244 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/ubuntu_cinnamon.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      722 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/ubuntu_gnome.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1305 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/ubuntu_kylin.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1414 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/ubuntu_mate.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1184 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/ubuntu_old.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      989 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/ubuntu_old02.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      406 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/ubuntu_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1320 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/ubuntu_studio.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1345 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/ubuntu_sway.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      410 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/ubuntu_touch.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1066 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/ultramarine_linux.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      816 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/univalent.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1244 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/univention.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1091 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/uos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1156 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/urukos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1171 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/uwuntu.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1016 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/vanilla.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      531 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/venom.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      933 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/vnux.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1704 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/void.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      266 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/void_small.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      921 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/vzlinux.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1271 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/wii_linux_ngx.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      839 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/windows.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      905 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/windows_10.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      724 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/windows_11.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      818 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/xferience.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1140 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/xubuntu.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      871 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/yiffos.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      654 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/distros/zorin.py
+-rwxr-xr-x   0 azalea    (1000) azalea    (1000)    15363 2023-06-02 07:16:42.000000 HyFetch-1.4.9/hyfetch/main.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      919 2023-06-02 06:39:07.000000 HyFetch-1.4.9/hyfetch/models.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)    12844 2023-06-02 07:16:03.000000 HyFetch-1.4.9/hyfetch/neofetch_util.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)    15154 2023-06-02 06:56:19.000000 HyFetch-1.4.9/hyfetch/presets.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     4002 2023-06-02 06:38:22.000000 HyFetch-1.4.9/hyfetch/pride_month.py
+drwxr-xr-x   0 azalea    (1000) azalea    (1000)        0 2023-06-02 07:31:03.034356 HyFetch-1.4.9/hyfetch/scripts/
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     5706 2023-05-16 03:13:08.000000 HyFetch-1.4.9/hyfetch/scripts/autocomplete.bash
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1505 2023-05-16 03:13:08.000000 HyFetch-1.4.9/hyfetch/scripts/autocomplete.csh
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1950 2023-05-16 03:13:08.000000 HyFetch-1.4.9/hyfetch/scripts/autocomplete.zsh
+-rwxr-xr-x   0 azalea    (1000) azalea    (1000)     1420 2023-05-16 03:13:08.000000 HyFetch-1.4.9/hyfetch/scripts/install-autocomplete.sh
+-rwxr-xr-x   0 azalea    (1000) azalea    (1000)   504946 2023-06-02 07:26:04.000000 HyFetch-1.4.9/hyfetch/scripts/neowofetch
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     1353 2022-09-24 20:22:01.000000 HyFetch-1.4.9/hyfetch/serializer.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     4729 2022-12-11 10:26:18.000000 HyFetch-1.4.9/hyfetch/termenv.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)      284 2022-12-11 10:26:18.000000 HyFetch-1.4.9/hyfetch/types.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)       38 2023-06-02 07:31:03.034356 HyFetch-1.4.9/setup.cfg
+-rwxr-xr-x   0 azalea    (1000) azalea    (1000)     1513 2023-05-16 03:13:08.000000 HyFetch-1.4.9/setup.py
+drwxr-xr-x   0 azalea    (1000) azalea    (1000)        0 2023-06-02 07:31:03.034356 HyFetch-1.4.9/tools/
+-rwxr-xr-x   0 azalea    (1000) azalea    (1000)     3502 2023-05-16 03:13:08.000000 HyFetch-1.4.9/tools/accept_upstream.py
+-rwxr-xr-x   0 azalea    (1000) azalea    (1000)     1034 2023-05-16 03:13:08.000000 HyFetch-1.4.9/tools/colors_test.py
+-rwxr-xr-x   0 azalea    (1000) azalea    (1000)     5303 2023-05-16 03:13:08.000000 HyFetch-1.4.9/tools/deploy-release.py
+-rw-r--r--   0 azalea    (1000) azalea    (1000)     5304 2023-05-16 03:13:08.000000 HyFetch-1.4.9/tools/gh_moderator.py
+-rwxr-xr-x   0 azalea    (1000) azalea    (1000)      988 2022-12-11 10:26:18.000000 HyFetch-1.4.9/tools/issue_fixed.py
+-rwxr-xr-x   0 azalea    (1000) azalea    (1000)     5246 2023-06-02 07:23:24.000000 HyFetch-1.4.9/tools/list_distros.py
+-rwxr-xr-x   0 azalea    (1000) azalea    (1000)     2640 2022-09-24 20:22:01.000000 HyFetch-1.4.9/tools/list_unresolved.py
+-rwxr-xr-x   0 azalea    (1000) azalea    (1000)      641 2023-05-16 03:13:08.000000 HyFetch-1.4.9/tools/reformat_readme.py
```

### Comparing `HyFetch-1.4.8/HyFetch.egg-info/PKG-INFO` & `HyFetch-1.4.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: HyFetch
-Version: 1.4.8
-Summary: neofetch with flags <3
-Home-page: https://github.com/hykilpikonna/HyFetch
-Author: Azalea Gui
-Author-email: me@hydev.org
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # HyFetch
 
 neofetch with pride flags <3
 
 <img alt="screenshot" src="https://user-images.githubusercontent.com/22280294/197708447-ddee6db2-1017-48f2-b507-8ddf85acef0d.png">
 
 ### Running Updated Original Neofetch
@@ -46,14 +28,15 @@
 
 Currently, these distributions have existing packages for HyFetch:
 
 * Arch Linux: `sudo pacman -S hyfetch` (Thanks to [@Aleksana](https://github.com/Aleksanaa) and [@Antiz96](https://github.com/Antiz96))
 * Nix: `nix-env -i hyfetch` (Thanks to [@YisuiDenghua](https://github.com/YisuiDenghua))
 * Guix: `guix install hyfetch` (Thanks to [@WammKD](https://github.com/WammKD))
 * Slackware `sbopkg -b hyfetch` Slackware [Slackbuild](https://slackbuilds.org/repository/15.0/desktop/hyfetch/?search=hyfetch) (Thanks to [@bittin](https://github.com/bittin) and Urchlay)
+* Nix Profile `nix profile install nixpkgs#hyfetch`
 
 
 ### Method 3: Install the latest developmental version using git
 
 Install Python >= 3.7 first. Then run the following commands:
 
 ```sh
@@ -103,34 +86,53 @@
 Updates to HyFetch begins with the emoji 🌈  
 Updates to `neowofetch` begins with the emoji 🖼️
 
 ### TODO
 
 * [ ] (Important!) Refactor flag storage & coloring to support non-stride patterns
 * [ ] Config menu: Allow left-right arrow keys for pagination
-* [ ] Neofetch argument pass through
 
 ### Nightly
 
 Note: You can install the latest nightly version by using:
 
 ```sh
 pip install git+https://github.com/hykilpikonna/hyfetch.git@master
 ```
 
 <!-- CHANGELOG STARTS HERE --->
 
+### 1.4.9
+
+* 🌈 Add pride month easter-egg animation! ⭐️
+* 🌈 Autocompletion for bash, zsh, tcsh ([#96](https://github.com/hykilpikonna/hyfetch/pull/96))
+* 🌈 Add nix profile installation method ([#114](https://github.com/hykilpikonna/hyfetch/pull/114))
+* 🌈 Add experimental color overlay function for more accurate lightness adjusting (using `--c-overlay`)
+* 🌈 Allow neofetch argument passthrough (using `--args='...'`)
+* 🌈 Show recommended terminal size ([#129](https://github.com/hykilpikonna/hyfetch/pull/129))
+* 🌈 Update issue & pull request templates
+* 🖼 Hostname - Fix FQDN substitution
+* 🖼 Version - Fix Windows version detection ([dylanaraps#2309](https://github.com/dylanaraps/neofetch/pull/2309))
+* 🖼 Packages - Fix winget stuck on agreement ([#82](https://github.com/hykilpikonna/hyfetch/pull/82))
+* 🖼 Distro - Fix Windows text encoding ([#115](https://github.com/hykilpikonna/hyfetch/pull/115))
+* 🖼 Distro - Add Astra Linux ([dylanaraps#2313](https://github.com/dylanaraps/neofetch/pull/2313))
+* 🖼 Distro - Add FemboyOS ([#121](https://github.com/hykilpikonna/hyfetch/pull/121))
+* 🖼 Distro - Add Nobara Linux ([dylanaraps#2326](https://github.com/dylanaraps/neofetch/pull/2326))
+* 🖼 Font - Fix Konsole ppid detection ([#116](https://github.com/hykilpikonna/hyfetch/pull/116))
+* 🖼 Font - Fix Konsole terminal font detection ([#127](https://github.com/hykilpikonna/hyfetch/pull/127))
+* 🖼 Image - Optimize sixel image display ([dylanaraps#2316](https://github.com/dylanaraps/neofetch/pull/2316))
+
 ### 1.4.8
 
 * 🌈 Improved Windows git bash detection ([#99](https://github.com/hykilpikonna/hyfetch/pull/99))
 * 🌈 Improved color formatting codes ([#101](https://github.com/hykilpikonna/hyfetch/pull/101))
 * 🌈 Allow specifying distro in config ([#102](https://github.com/hykilpikonna/hyfetch/pull/102))
 * 🌈 Allow specifying custom ascii files ([#104](https://github.com/hykilpikonna/hyfetch/pull/104))
-* 🌈 Add omniromantic and pangender ([#106](https://github.com/hykilpikonna/hyfetch/pull/106))
-* 🌈 Now officially packaged for ArchLinux Community & Slackware! ([#112](https://github.com/hykilpikonna/hyfetch/pull/112)) ([#109](https://github.com/hykilpikonna/hyfetch/pull/109))
+* 🌈 Add omniromantic and pangender flags ([#106](https://github.com/hykilpikonna/hyfetch/pull/106))
+* 🌈 Now officially packaged for ArchLinux Community & Slackware! ([#112](https://github.com/hykilpikonna/hyfetch/pull/112) | [#109](https://github.com/hykilpikonna/hyfetch/pull/109))
 * 🖼 Host - Update Apple device model detection. ([#111](https://github.com/hykilpikonna/hyfetch/pull/111))
 * 🖼 Distro - Add Salient OS. ([dylanaraps#2301](https://github.com/dylanaraps/neofetch/pull/2301))
 * 🖼 Distro - Add PikaOS. ([#105](https://github.com/hykilpikonna/hyfetch/pull/105))
 * 🖼 Distro - Add Archcraft minimal variant. ([#108](https://github.com/hykilpikonna/hyfetch/pull/108))
 * 🖼 Distro - Update Vanilla logo. ([#98](https://github.com/hykilpikonna/hyfetch/pull/98))
 * 🖼 Distro - ChromeOS version improvements. ([dylanaraps#2305](https://github.com/dylanaraps/neofetch/pull/2305))
 * 🖼 CPU - Improved multi-cpu ARM chip detection. ([#97](https://github.com/hykilpikonna/hyfetch/pull/97))
```

### Comparing `HyFetch-1.4.8/HyFetch.egg-info/SOURCES.txt` & `HyFetch-1.4.9/HyFetch.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,11 @@
-.gitattributes
-.gitignore
-CONTRIBUTING.md
 LICENSE.md
 MANIFEST.in
-Makefile
 README.md
-default.nix
-neofetch
-neofetch.1
-package.json
-runner.py
 setup.py
-test.py
-.github/ISSUE_TEMPLATE.md
-.github/PULL_REQUEST_TEMPLATE.md
-.github/workflows/arch_package.yml
-.github/workflows/release.yml
-.github/workflows/shellcheck.yml
-.vscode/launch.json
 HyFetch.egg-info/PKG-INFO
 HyFetch.egg-info/SOURCES.txt
 HyFetch.egg-info/dependency_links.txt
 HyFetch.egg-info/entry_points.txt
 HyFetch.egg-info/requires.txt
 HyFetch.egg-info/top_level.txt
 hyfetch/__init__.py
@@ -30,14 +14,15 @@
 hyfetch/color_scale.py
 hyfetch/color_util.py
 hyfetch/constants.py
 hyfetch/main.py
 hyfetch/models.py
 hyfetch/neofetch_util.py
 hyfetch/presets.py
+hyfetch/pride_month.py
 hyfetch/serializer.py
 hyfetch/termenv.py
 hyfetch/types.py
 hyfetch/distros/__init__.py
 hyfetch/distros/aix.py
 hyfetch/distros/almalinux.py
 hyfetch/distros/alpine.py
@@ -72,14 +57,15 @@
 hyfetch/distros/artix.py
 hyfetch/distros/artix_small.py
 hyfetch/distros/arya.py
 hyfetch/distros/asahi.py
 hyfetch/distros/aster.py
 hyfetch/distros/asteroidos.py
 hyfetch/distros/astos.py
+hyfetch/distros/astra_linux.py
 hyfetch/distros/bedrock.py
 hyfetch/distros/biglinux.py
 hyfetch/distros/bitrig.py
 hyfetch/distros/blackarch.py
 hyfetch/distros/blackpanther.py
 hyfetch/distros/blag.py
 hyfetch/distros/blankon.py
@@ -143,14 +129,15 @@
 hyfetch/distros/enso.py
 hyfetch/distros/eurolinux.py
 hyfetch/distros/exherbo.py
 hyfetch/distros/exodia_predator_os.py
 hyfetch/distros/fedora.py
 hyfetch/distros/fedora_old.py
 hyfetch/distros/fedora_small.py
+hyfetch/distros/femboyos.py
 hyfetch/distros/feren.py
 hyfetch/distros/finnix.py
 hyfetch/distros/floflis.py
 hyfetch/distros/freebsd.py
 hyfetch/distros/freebsd_small.py
 hyfetch/distros/freemint.py
 hyfetch/distros/frugalware.py
@@ -234,14 +221,15 @@
 hyfetch/distros/netbsd.py
 hyfetch/distros/netbsd_small.py
 hyfetch/distros/netrunner.py
 hyfetch/distros/nitrux.py
 hyfetch/distros/nixos.py
 hyfetch/distros/nixos_old.py
 hyfetch/distros/nixos_small.py
+hyfetch/distros/nobara.py
 hyfetch/distros/nomadbsd.py
 hyfetch/distros/nurunner.py
 hyfetch/distros/nutyx.py
 hyfetch/distros/obarun.py
 hyfetch/distros/obrevenge.py
 hyfetch/distros/omnios.py
 hyfetch/distros/open_source_media_center.py
@@ -372,19 +360,20 @@
 hyfetch/distros/windows.py
 hyfetch/distros/windows_10.py
 hyfetch/distros/windows_11.py
 hyfetch/distros/xferience.py
 hyfetch/distros/xubuntu.py
 hyfetch/distros/yiffos.py
 hyfetch/distros/zorin.py
+hyfetch/scripts/autocomplete.bash
+hyfetch/scripts/autocomplete.csh
+hyfetch/scripts/autocomplete.zsh
+hyfetch/scripts/install-autocomplete.sh
 hyfetch/scripts/neowofetch
 tools/accept_upstream.py
 tools/colors_test.py
 tools/deploy-release.py
-tools/deploy.md
-tools/deploy.sh
+tools/gh_moderator.py
 tools/issue_fixed.py
-tools/issue_whitelist.py
 tools/list_distros.py
 tools/list_unresolved.py
-tools/pull_request_markings.yaml
 tools/reformat_readme.py
```

### Comparing `HyFetch-1.4.8/LICENSE.md` & `HyFetch-1.4.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/PKG-INFO` & `HyFetch-1.4.9/HyFetch.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HyFetch
-Version: 1.4.8
+Version: 1.4.9
 Summary: neofetch with flags <3
 Home-page: https://github.com/hykilpikonna/HyFetch
 Author: Azalea Gui
 Author-email: me@hydev.org
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -46,14 +46,15 @@
 
 Currently, these distributions have existing packages for HyFetch:
 
 * Arch Linux: `sudo pacman -S hyfetch` (Thanks to [@Aleksana](https://github.com/Aleksanaa) and [@Antiz96](https://github.com/Antiz96))
 * Nix: `nix-env -i hyfetch` (Thanks to [@YisuiDenghua](https://github.com/YisuiDenghua))
 * Guix: `guix install hyfetch` (Thanks to [@WammKD](https://github.com/WammKD))
 * Slackware `sbopkg -b hyfetch` Slackware [Slackbuild](https://slackbuilds.org/repository/15.0/desktop/hyfetch/?search=hyfetch) (Thanks to [@bittin](https://github.com/bittin) and Urchlay)
+* Nix Profile `nix profile install nixpkgs#hyfetch`
 
 
 ### Method 3: Install the latest developmental version using git
 
 Install Python >= 3.7 first. Then run the following commands:
 
 ```sh
@@ -103,34 +104,53 @@
 Updates to HyFetch begins with the emoji 🌈  
 Updates to `neowofetch` begins with the emoji 🖼️
 
 ### TODO
 
 * [ ] (Important!) Refactor flag storage & coloring to support non-stride patterns
 * [ ] Config menu: Allow left-right arrow keys for pagination
-* [ ] Neofetch argument pass through
 
 ### Nightly
 
 Note: You can install the latest nightly version by using:
 
 ```sh
 pip install git+https://github.com/hykilpikonna/hyfetch.git@master
 ```
 
 <!-- CHANGELOG STARTS HERE --->
 
+### 1.4.9
+
+* 🌈 Add pride month easter-egg animation! ⭐️
+* 🌈 Autocompletion for bash, zsh, tcsh ([#96](https://github.com/hykilpikonna/hyfetch/pull/96))
+* 🌈 Add nix profile installation method ([#114](https://github.com/hykilpikonna/hyfetch/pull/114))
+* 🌈 Add experimental color overlay function for more accurate lightness adjusting (using `--c-overlay`)
+* 🌈 Allow neofetch argument passthrough (using `--args='...'`)
+* 🌈 Show recommended terminal size ([#129](https://github.com/hykilpikonna/hyfetch/pull/129))
+* 🌈 Update issue & pull request templates
+* 🖼 Hostname - Fix FQDN substitution
+* 🖼 Version - Fix Windows version detection ([dylanaraps#2309](https://github.com/dylanaraps/neofetch/pull/2309))
+* 🖼 Packages - Fix winget stuck on agreement ([#82](https://github.com/hykilpikonna/hyfetch/pull/82))
+* 🖼 Distro - Fix Windows text encoding ([#115](https://github.com/hykilpikonna/hyfetch/pull/115))
+* 🖼 Distro - Add Astra Linux ([dylanaraps#2313](https://github.com/dylanaraps/neofetch/pull/2313))
+* 🖼 Distro - Add FemboyOS ([#121](https://github.com/hykilpikonna/hyfetch/pull/121))
+* 🖼 Distro - Add Nobara Linux ([dylanaraps#2326](https://github.com/dylanaraps/neofetch/pull/2326))
+* 🖼 Font - Fix Konsole ppid detection ([#116](https://github.com/hykilpikonna/hyfetch/pull/116))
+* 🖼 Font - Fix Konsole terminal font detection ([#127](https://github.com/hykilpikonna/hyfetch/pull/127))
+* 🖼 Image - Optimize sixel image display ([dylanaraps#2316](https://github.com/dylanaraps/neofetch/pull/2316))
+
 ### 1.4.8
 
 * 🌈 Improved Windows git bash detection ([#99](https://github.com/hykilpikonna/hyfetch/pull/99))
 * 🌈 Improved color formatting codes ([#101](https://github.com/hykilpikonna/hyfetch/pull/101))
 * 🌈 Allow specifying distro in config ([#102](https://github.com/hykilpikonna/hyfetch/pull/102))
 * 🌈 Allow specifying custom ascii files ([#104](https://github.com/hykilpikonna/hyfetch/pull/104))
-* 🌈 Add omniromantic and pangender ([#106](https://github.com/hykilpikonna/hyfetch/pull/106))
-* 🌈 Now officially packaged for ArchLinux Community & Slackware! ([#112](https://github.com/hykilpikonna/hyfetch/pull/112)) ([#109](https://github.com/hykilpikonna/hyfetch/pull/109))
+* 🌈 Add omniromantic and pangender flags ([#106](https://github.com/hykilpikonna/hyfetch/pull/106))
+* 🌈 Now officially packaged for ArchLinux Community & Slackware! ([#112](https://github.com/hykilpikonna/hyfetch/pull/112) | [#109](https://github.com/hykilpikonna/hyfetch/pull/109))
 * 🖼 Host - Update Apple device model detection. ([#111](https://github.com/hykilpikonna/hyfetch/pull/111))
 * 🖼 Distro - Add Salient OS. ([dylanaraps#2301](https://github.com/dylanaraps/neofetch/pull/2301))
 * 🖼 Distro - Add PikaOS. ([#105](https://github.com/hykilpikonna/hyfetch/pull/105))
 * 🖼 Distro - Add Archcraft minimal variant. ([#108](https://github.com/hykilpikonna/hyfetch/pull/108))
 * 🖼 Distro - Update Vanilla logo. ([#98](https://github.com/hykilpikonna/hyfetch/pull/98))
 * 🖼 Distro - ChromeOS version improvements. ([dylanaraps#2305](https://github.com/dylanaraps/neofetch/pull/2305))
 * 🖼 CPU - Improved multi-cpu ARM chip detection. ([#97](https://github.com/hykilpikonna/hyfetch/pull/97))
```

### Comparing `HyFetch-1.4.8/README.md` & `HyFetch-1.4.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: HyFetch
+Version: 1.4.9
+Summary: neofetch with flags <3
+Home-page: https://github.com/hykilpikonna/HyFetch
+Author: Azalea Gui
+Author-email: me@hydev.org
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 # HyFetch
 
 neofetch with pride flags <3
 
 <img alt="screenshot" src="https://user-images.githubusercontent.com/22280294/197708447-ddee6db2-1017-48f2-b507-8ddf85acef0d.png">
 
 ### Running Updated Original Neofetch
@@ -28,14 +46,15 @@
 
 Currently, these distributions have existing packages for HyFetch:
 
 * Arch Linux: `sudo pacman -S hyfetch` (Thanks to [@Aleksana](https://github.com/Aleksanaa) and [@Antiz96](https://github.com/Antiz96))
 * Nix: `nix-env -i hyfetch` (Thanks to [@YisuiDenghua](https://github.com/YisuiDenghua))
 * Guix: `guix install hyfetch` (Thanks to [@WammKD](https://github.com/WammKD))
 * Slackware `sbopkg -b hyfetch` Slackware [Slackbuild](https://slackbuilds.org/repository/15.0/desktop/hyfetch/?search=hyfetch) (Thanks to [@bittin](https://github.com/bittin) and Urchlay)
+* Nix Profile `nix profile install nixpkgs#hyfetch`
 
 
 ### Method 3: Install the latest developmental version using git
 
 Install Python >= 3.7 first. Then run the following commands:
 
 ```sh
@@ -85,34 +104,53 @@
 Updates to HyFetch begins with the emoji 🌈  
 Updates to `neowofetch` begins with the emoji 🖼️
 
 ### TODO
 
 * [ ] (Important!) Refactor flag storage & coloring to support non-stride patterns
 * [ ] Config menu: Allow left-right arrow keys for pagination
-* [ ] Neofetch argument pass through
 
 ### Nightly
 
 Note: You can install the latest nightly version by using:
 
 ```sh
 pip install git+https://github.com/hykilpikonna/hyfetch.git@master
 ```
 
 <!-- CHANGELOG STARTS HERE --->
 
+### 1.4.9
+
+* 🌈 Add pride month easter-egg animation! ⭐️
+* 🌈 Autocompletion for bash, zsh, tcsh ([#96](https://github.com/hykilpikonna/hyfetch/pull/96))
+* 🌈 Add nix profile installation method ([#114](https://github.com/hykilpikonna/hyfetch/pull/114))
+* 🌈 Add experimental color overlay function for more accurate lightness adjusting (using `--c-overlay`)
+* 🌈 Allow neofetch argument passthrough (using `--args='...'`)
+* 🌈 Show recommended terminal size ([#129](https://github.com/hykilpikonna/hyfetch/pull/129))
+* 🌈 Update issue & pull request templates
+* 🖼 Hostname - Fix FQDN substitution
+* 🖼 Version - Fix Windows version detection ([dylanaraps#2309](https://github.com/dylanaraps/neofetch/pull/2309))
+* 🖼 Packages - Fix winget stuck on agreement ([#82](https://github.com/hykilpikonna/hyfetch/pull/82))
+* 🖼 Distro - Fix Windows text encoding ([#115](https://github.com/hykilpikonna/hyfetch/pull/115))
+* 🖼 Distro - Add Astra Linux ([dylanaraps#2313](https://github.com/dylanaraps/neofetch/pull/2313))
+* 🖼 Distro - Add FemboyOS ([#121](https://github.com/hykilpikonna/hyfetch/pull/121))
+* 🖼 Distro - Add Nobara Linux ([dylanaraps#2326](https://github.com/dylanaraps/neofetch/pull/2326))
+* 🖼 Font - Fix Konsole ppid detection ([#116](https://github.com/hykilpikonna/hyfetch/pull/116))
+* 🖼 Font - Fix Konsole terminal font detection ([#127](https://github.com/hykilpikonna/hyfetch/pull/127))
+* 🖼 Image - Optimize sixel image display ([dylanaraps#2316](https://github.com/dylanaraps/neofetch/pull/2316))
+
 ### 1.4.8
 
 * 🌈 Improved Windows git bash detection ([#99](https://github.com/hykilpikonna/hyfetch/pull/99))
 * 🌈 Improved color formatting codes ([#101](https://github.com/hykilpikonna/hyfetch/pull/101))
 * 🌈 Allow specifying distro in config ([#102](https://github.com/hykilpikonna/hyfetch/pull/102))
 * 🌈 Allow specifying custom ascii files ([#104](https://github.com/hykilpikonna/hyfetch/pull/104))
-* 🌈 Add omniromantic and pangender ([#106](https://github.com/hykilpikonna/hyfetch/pull/106))
-* 🌈 Now officially packaged for ArchLinux Community & Slackware! ([#112](https://github.com/hykilpikonna/hyfetch/pull/112)) ([#109](https://github.com/hykilpikonna/hyfetch/pull/109))
+* 🌈 Add omniromantic and pangender flags ([#106](https://github.com/hykilpikonna/hyfetch/pull/106))
+* 🌈 Now officially packaged for ArchLinux Community & Slackware! ([#112](https://github.com/hykilpikonna/hyfetch/pull/112) | [#109](https://github.com/hykilpikonna/hyfetch/pull/109))
 * 🖼 Host - Update Apple device model detection. ([#111](https://github.com/hykilpikonna/hyfetch/pull/111))
 * 🖼 Distro - Add Salient OS. ([dylanaraps#2301](https://github.com/dylanaraps/neofetch/pull/2301))
 * 🖼 Distro - Add PikaOS. ([#105](https://github.com/hykilpikonna/hyfetch/pull/105))
 * 🖼 Distro - Add Archcraft minimal variant. ([#108](https://github.com/hykilpikonna/hyfetch/pull/108))
 * 🖼 Distro - Update Vanilla logo. ([#98](https://github.com/hykilpikonna/hyfetch/pull/98))
 * 🖼 Distro - ChromeOS version improvements. ([dylanaraps#2305](https://github.com/dylanaraps/neofetch/pull/2305))
 * 🖼 CPU - Improved multi-cpu ARM chip detection. ([#97](https://github.com/hykilpikonna/hyfetch/pull/97))
```

### Comparing `HyFetch-1.4.8/hyfetch/color_scale.py` & `HyFetch-1.4.9/hyfetch/color_scale.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/color_util.py` & `HyFetch-1.4.9/hyfetch/color_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -235,7 +235,17 @@
                 hsl.l = max(hsl.l, light)
 
         # Convert back to RGB
         return hsl.rgb()
 
     def is_light(self):
         return self.hsl().l > 0.5
+
+    def overlay(self, color: 'RGB', alpha: float) -> 'RGB':
+        """
+        Overlay a color on top of this color
+
+        :param color: Overlay color
+        :param alpha: Overlay alpha
+        :return: New color (original isn't modified)
+        """
+        return RGB(*[round((1 - alpha) * v1 + alpha * v2) for v1, v2 in zip(self, color)])
```

### Comparing `HyFetch-1.4.8/hyfetch/constants.py` & `HyFetch-1.4.9/hyfetch/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,20 +31,21 @@
 @dataclass
 class GlobalConfig:
     # Global color mode default to 8-bit for compatibility
     color_mode: str
     override_distro: str | None
     debug: bool
     is_light: bool
+    use_overlay: bool
 
     def light_dark(self) -> LightDark:
         return 'light' if self.is_light else 'dark'
 
     def default_lightness(self, term: LightDark | None = None) -> float:
         if term is None:
             term = self.light_dark()
         return 0.65 if term.lower() == 'dark' else 0.4
 
 
-GLOBAL_CFG = GlobalConfig(color_mode='8bit', override_distro=None, debug=False, is_light=False)
+GLOBAL_CFG = GlobalConfig(color_mode='8bit', override_distro=None, debug=False, is_light=False, use_overlay=False)
 
 MINGIT_URL = 'https://github.com/git-for-windows/git/releases/download/v2.37.2.windows.2/MinGit-2.37.2.2-busybox-32-bit.zip'
```

### Comparing `HyFetch-1.4.8/hyfetch/distros/aix.py` & `HyFetch-1.4.9/hyfetch/distros/aix.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/almalinux.py` & `HyFetch-1.4.9/hyfetch/distros/almalinux.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/alpine.py` & `HyFetch-1.4.9/hyfetch/distros/alpine.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/alter.py` & `HyFetch-1.4.9/hyfetch/distros/alter.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/amazon.py` & `HyFetch-1.4.9/hyfetch/distros/amazon.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/amogos.py` & `HyFetch-1.4.9/hyfetch/distros/amogos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/anarchy.py` & `HyFetch-1.4.9/hyfetch/distros/anarchy.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/android.py` & `HyFetch-1.4.9/hyfetch/distros/android.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/antergos.py` & `HyFetch-1.4.9/hyfetch/distros/antergos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/antix.py` & `HyFetch-1.4.9/hyfetch/distros/antix.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/aosc_os.py` & `HyFetch-1.4.9/hyfetch/distros/aosc_os.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/aosc_os_retro.py` & `HyFetch-1.4.9/hyfetch/distros/aosc_os_retro.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/aperture.py` & `HyFetch-1.4.9/hyfetch/distros/aperture.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/apricity.py` & `HyFetch-1.4.9/hyfetch/distros/apricity.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/arch.py` & `HyFetch-1.4.9/hyfetch/distros/arch.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/arch_old.py` & `HyFetch-1.4.9/hyfetch/distros/arch_old.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/archbox.py` & `HyFetch-1.4.9/hyfetch/distros/archbox.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/archcraft.py` & `HyFetch-1.4.9/hyfetch/distros/archcraft.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/archcraft_ascii.py` & `HyFetch-1.4.9/hyfetch/distros/archcraft_ascii.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/archcraft_minimal.py` & `HyFetch-1.4.9/hyfetch/distros/archcraft_minimal.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/archlabs.py` & `HyFetch-1.4.9/hyfetch/distros/archlabs.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/archmerge.py` & `HyFetch-1.4.9/hyfetch/distros/archmerge.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/archstrike.py` & `HyFetch-1.4.9/hyfetch/distros/archstrike.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/arcolinux.py` & `HyFetch-1.4.9/hyfetch/distros/arcolinux.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/arselinux.py` & `HyFetch-1.4.9/hyfetch/distros/arselinux.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/artix.py` & `HyFetch-1.4.9/hyfetch/distros/artix.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/arya.py` & `HyFetch-1.4.9/hyfetch/distros/arya.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/asahi.py` & `HyFetch-1.4.9/hyfetch/distros/asahi.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/aster.py` & `HyFetch-1.4.9/hyfetch/distros/aster.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/asteroidos.py` & `HyFetch-1.4.9/hyfetch/distros/asteroidos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/astos.py` & `HyFetch-1.4.9/hyfetch/distros/astos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/bedrock.py` & `HyFetch-1.4.9/hyfetch/distros/bedrock.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/biglinux.py` & `HyFetch-1.4.9/hyfetch/distros/biglinux.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/blackarch.py` & `HyFetch-1.4.9/hyfetch/distros/blackarch.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/blackpanther.py` & `HyFetch-1.4.9/hyfetch/distros/blackpanther.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/blag.py` & `HyFetch-1.4.9/hyfetch/distros/blag.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/blankon.py` & `HyFetch-1.4.9/hyfetch/distros/blankon.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/bluelight.py` & `HyFetch-1.4.9/hyfetch/distros/bluelight.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/bodhi.py` & `HyFetch-1.4.9/hyfetch/distros/bodhi.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/bonsai.py` & `HyFetch-1.4.9/hyfetch/distros/bonsai.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/bsd.py` & `HyFetch-1.4.9/hyfetch/distros/bsd.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/cachyos.py` & `HyFetch-1.4.9/hyfetch/distros/cachyos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/calculate.py` & `HyFetch-1.4.9/hyfetch/distros/calculate.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/calinixos.py` & `HyFetch-1.4.9/hyfetch/distros/calinixos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/calinixos_small.py` & `HyFetch-1.4.9/hyfetch/distros/calinixos_small.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/carbs.py` & `HyFetch-1.4.9/hyfetch/distros/carbs.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/cbl_mariner.py` & `HyFetch-1.4.9/hyfetch/distros/cbl_mariner.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/celos.py` & `HyFetch-1.4.9/hyfetch/distros/celos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/centos.py` & `HyFetch-1.4.9/hyfetch/distros/centos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/chakra.py` & `HyFetch-1.4.9/hyfetch/distros/chakra.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/chaletos.py` & `HyFetch-1.4.9/hyfetch/distros/chaletos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/chapeau.py` & `HyFetch-1.4.9/hyfetch/distros/chapeau.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/chonkysealos.py` & `HyFetch-1.4.9/hyfetch/distros/chonkysealos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/chrom.py` & `HyFetch-1.4.9/hyfetch/distros/chrom.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/cleanjaro.py` & `HyFetch-1.4.9/hyfetch/distros/cleanjaro.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/clear_linux_os.py` & `HyFetch-1.4.9/hyfetch/distros/clear_linux_os.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/clearos.py` & `HyFetch-1.4.9/hyfetch/distros/clearos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/clover.py` & `HyFetch-1.4.9/hyfetch/distros/clover.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/cobalt.py` & `HyFetch-1.4.9/hyfetch/distros/cobalt.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/condres.py` & `HyFetch-1.4.9/hyfetch/distros/condres.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/container_linux_by_coreos.py` & `HyFetch-1.4.9/hyfetch/distros/container_linux_by_coreos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/crux.py` & `HyFetch-1.4.9/hyfetch/distros/crux.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/crystal_linux.py` & `HyFetch-1.4.9/hyfetch/distros/crystal_linux.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/cucumber.py` & `HyFetch-1.4.9/hyfetch/distros/cucumber.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/cuteos.py` & `HyFetch-1.4.9/hyfetch/distros/cuteos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/cyberos.py` & `HyFetch-1.4.9/hyfetch/distros/cyberos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/dahlia.py` & `HyFetch-1.4.9/hyfetch/distros/dahlia.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/darkos.py` & `HyFetch-1.4.9/hyfetch/distros/darkos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/darwin.py` & `HyFetch-1.4.9/hyfetch/distros/darwin.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/debian.py` & `HyFetch-1.4.9/hyfetch/distros/debian.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/deepin.py` & `HyFetch-1.4.9/hyfetch/distros/deepin.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/desaos.py` & `HyFetch-1.4.9/hyfetch/distros/desaos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/devuan.py` & `HyFetch-1.4.9/hyfetch/distros/devuan.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/dietpi.py` & `HyFetch-1.4.9/hyfetch/distros/dietpi.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/distro_detector.py` & `HyFetch-1.4.9/hyfetch/distros/distro_detector.py`

 * *Files 0% similar despite different names*

```diff
@@ -464,14 +464,18 @@
         from .fedora import fedora
         return fedora
     
     if name.startswith('feren'):
         from .feren import feren
         return feren
     
+    if name.startswith('femboyos'):
+        from .femboyos import femboyos
+        return femboyos
+    
     if name.startswith('finnix'):
         from .finnix import finnix
         return finnix
     
     if name == 'freebsd_small':
         from .freebsd_small import freebsd_small
         return freebsd_small
@@ -796,14 +800,18 @@
         from .nixos_old import nixos_old
         return nixos_old
     
     if name.startswith('nixos'):
         from .nixos import nixos
         return nixos
     
+    if name.startswith('nobara'):
+        from .nobara import nobara
+        return nobara
+    
     if name.startswith('nomadbsd'):
         from .nomadbsd import nomadbsd
         return nomadbsd
     
     if name.startswith('ghostbsd'):
         from .ghostbsd import ghostbsd
         return ghostbsd
@@ -1052,14 +1060,18 @@
         from .rocky import rocky
         return rocky
     
     if name.startswith('rosa'):
         from .rosa import rosa
         return rosa
     
+    if name.startswith('astra linux'):
+        from .astra_linux import astra_linux
+        return astra_linux
+    
     if name.startswith('sabotage'):
         from .sabotage import sabotage
         return sabotage
     
     if name.startswith('sabayon'):
         from .sabayon import sabayon
         return sabayon
```

### Comparing `HyFetch-1.4.8/hyfetch/distros/dracos.py` & `HyFetch-1.4.9/hyfetch/distros/dracos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/dragonfly.py` & `HyFetch-1.4.9/hyfetch/distros/dragonfly.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/dragonfly_old.py` & `HyFetch-1.4.9/hyfetch/distros/dragonfly_old.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/drauger.py` & `HyFetch-1.4.9/hyfetch/distros/drauger.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/droidian.py` & `HyFetch-1.4.9/hyfetch/distros/droidian.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/elementary.py` & `HyFetch-1.4.9/hyfetch/distros/elementary.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/elive.py` & `HyFetch-1.4.9/hyfetch/distros/elive.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/encryptos.py` & `HyFetch-1.4.9/hyfetch/distros/encryptos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/endeavouros.py` & `HyFetch-1.4.9/hyfetch/distros/endeavouros.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/endless.py` & `HyFetch-1.4.9/hyfetch/distros/endless.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/enso.py` & `HyFetch-1.4.9/hyfetch/distros/enso.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/eurolinux.py` & `HyFetch-1.4.9/hyfetch/distros/eurolinux.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/exherbo.py` & `HyFetch-1.4.9/hyfetch/distros/exherbo.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/exodia_predator_os.py` & `HyFetch-1.4.9/hyfetch/distros/exodia_predator_os.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/fedora.py` & `HyFetch-1.4.9/hyfetch/distros/fedora.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/fedora_old.py` & `HyFetch-1.4.9/hyfetch/distros/fedora_old.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/feren.py` & `HyFetch-1.4.9/hyfetch/distros/feren.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/finnix.py` & `HyFetch-1.4.9/hyfetch/distros/finnix.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/floflis.py` & `HyFetch-1.4.9/hyfetch/distros/floflis.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/freebsd.py` & `HyFetch-1.4.9/hyfetch/distros/freebsd.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/freemint.py` & `HyFetch-1.4.9/hyfetch/distros/freemint.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/frugalware.py` & `HyFetch-1.4.9/hyfetch/distros/frugalware.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/funtoo.py` & `HyFetch-1.4.9/hyfetch/distros/funtoo.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/galliumos.py` & `HyFetch-1.4.9/hyfetch/distros/galliumos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/garuda.py` & `HyFetch-1.4.9/hyfetch/distros/garuda.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/gentoo.py` & `HyFetch-1.4.9/hyfetch/distros/gentoo.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/glaucus.py` & `HyFetch-1.4.9/hyfetch/distros/glaucus.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/gnewsense.py` & `HyFetch-1.4.9/hyfetch/distros/gnewsense.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/gnome.py` & `HyFetch-1.4.9/hyfetch/distros/gnome.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/gnu.py` & `HyFetch-1.4.9/hyfetch/distros/gnu.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/grapheneos.py` & `HyFetch-1.4.9/hyfetch/distros/grapheneos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/grombyang.py` & `HyFetch-1.4.9/hyfetch/distros/grombyang.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/haiku.py` & `HyFetch-1.4.9/hyfetch/distros/haiku.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/hamonikr.py` & `HyFetch-1.4.9/hyfetch/distros/hamonikr.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/hardclanz.py` & `HyFetch-1.4.9/hyfetch/distros/hardclanz.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/huayra.py` & `HyFetch-1.4.9/hyfetch/distros/huayra.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/hybrid.py` & `HyFetch-1.4.9/hyfetch/distros/hybrid.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/hyperbola.py` & `HyFetch-1.4.9/hyfetch/distros/hyperbola.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/instantos.py` & `HyFetch-1.4.9/hyfetch/distros/instantos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/irix.py` & `HyFetch-1.4.9/hyfetch/distros/irix.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/itc.py` & `HyFetch-1.4.9/hyfetch/distros/itc.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/januslinux.py` & `HyFetch-1.4.9/hyfetch/distros/januslinux.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/kaisen.py` & `HyFetch-1.4.9/hyfetch/distros/kaisen.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/kali.py` & `HyFetch-1.4.9/hyfetch/distros/kali.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/kaos.py` & `HyFetch-1.4.9/hyfetch/distros/kaos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/kde.py` & `HyFetch-1.4.9/hyfetch/distros/kde.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/kibojoe.py` & `HyFetch-1.4.9/hyfetch/distros/kibojoe.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/kogaion.py` & `HyFetch-1.4.9/hyfetch/distros/kogaion.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/korora.py` & `HyFetch-1.4.9/hyfetch/distros/korora.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/krassos.py` & `HyFetch-1.4.9/hyfetch/distros/krassos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/kubuntu.py` & `HyFetch-1.4.9/hyfetch/distros/kubuntu.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/langitketujuh.py` & `HyFetch-1.4.9/hyfetch/distros/langitketujuh.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/langitketujuh_old.py` & `HyFetch-1.4.9/hyfetch/distros/langitketujuh_old.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/laxeros.py` & `HyFetch-1.4.9/hyfetch/distros/laxeros.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/libreelec.py` & `HyFetch-1.4.9/hyfetch/distros/libreelec.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/linspire.py` & `HyFetch-1.4.9/hyfetch/distros/linspire.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/linux.py` & `HyFetch-1.4.9/hyfetch/distros/linux.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/linux_lite.py` & `HyFetch-1.4.9/hyfetch/distros/linux_lite.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/linux_mint.py` & `HyFetch-1.4.9/hyfetch/distros/linux_mint.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/linux_mint_old.py` & `HyFetch-1.4.9/hyfetch/distros/linux_mint_old.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/live_raizo.py` & `HyFetch-1.4.9/hyfetch/distros/live_raizo.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/lmde.py` & `HyFetch-1.4.9/hyfetch/distros/lmde.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/lubuntu.py` & `HyFetch-1.4.9/hyfetch/distros/lubuntu.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/lunar.py` & `HyFetch-1.4.9/hyfetch/distros/lunar.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/mac.py` & `HyFetch-1.4.9/hyfetch/distros/mac.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/mageia.py` & `HyFetch-1.4.9/hyfetch/distros/mageia.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/magpieos.py` & `HyFetch-1.4.9/hyfetch/distros/magpieos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/mandriva.py` & `HyFetch-1.4.9/hyfetch/distros/mandriva.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/manjaro.py` & `HyFetch-1.4.9/hyfetch/distros/manjaro.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/massos.py` & `HyFetch-1.4.9/hyfetch/distros/massos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/matuusos.py` & `HyFetch-1.4.9/hyfetch/distros/matuusos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/maui.py` & `HyFetch-1.4.9/hyfetch/distros/maui.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/mer.py` & `HyFetch-1.4.9/hyfetch/distros/mer.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/minix.py` & `HyFetch-1.4.9/hyfetch/distros/minix.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/miracle_linux.py` & `HyFetch-1.4.9/hyfetch/distros/miracle_linux.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/mx.py` & `HyFetch-1.4.9/hyfetch/distros/mx.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/namib.py` & `HyFetch-1.4.9/hyfetch/distros/namib.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/nekos.py` & `HyFetch-1.4.9/hyfetch/distros/nekos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/neptune.py` & `HyFetch-1.4.9/hyfetch/distros/neptune.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/netbsd.py` & `HyFetch-1.4.9/hyfetch/distros/netbsd.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/netrunner.py` & `HyFetch-1.4.9/hyfetch/distros/netrunner.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/nixos.py` & `HyFetch-1.4.9/hyfetch/distros/nixos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/nixos_old.py` & `HyFetch-1.4.9/hyfetch/distros/nixos_old.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/nurunner.py` & `HyFetch-1.4.9/hyfetch/distros/nurunner.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/nutyx.py` & `HyFetch-1.4.9/hyfetch/distros/nutyx.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/obarun.py` & `HyFetch-1.4.9/hyfetch/distros/obarun.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/obrevenge.py` & `HyFetch-1.4.9/hyfetch/distros/obrevenge.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/open_source_media_center.py` & `HyFetch-1.4.9/hyfetch/distros/open_source_media_center.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/openbsd.py` & `HyFetch-1.4.9/hyfetch/distros/openbsd.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/openeuler.py` & `HyFetch-1.4.9/hyfetch/distros/openeuler.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/openindiana.py` & `HyFetch-1.4.9/hyfetch/distros/openindiana.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/openmamba.py` & `HyFetch-1.4.9/hyfetch/distros/openmamba.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/openmandriva.py` & `HyFetch-1.4.9/hyfetch/distros/openmandriva.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/openstage.py` & `HyFetch-1.4.9/hyfetch/distros/openstage.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/opensuse.py` & `HyFetch-1.4.9/hyfetch/distros/opensuse.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/opensuse_leap.py` & `HyFetch-1.4.9/hyfetch/distros/opensuse_leap.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/opensuse_tumbleweed.py` & `HyFetch-1.4.9/hyfetch/distros/opensuse_tumbleweed.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/opnsense.py` & `HyFetch-1.4.9/hyfetch/distros/opnsense.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/oracle.py` & `HyFetch-1.4.9/hyfetch/distros/oracle.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/orchid.py` & `HyFetch-1.4.9/hyfetch/distros/orchid.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/orchid_small.py` & `HyFetch-1.4.9/hyfetch/distros/orchid_small.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/os_elbrus.py` & `HyFetch-1.4.9/hyfetch/distros/os_elbrus.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/pacbsd.py` & `HyFetch-1.4.9/hyfetch/distros/pacbsd.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/parabola.py` & `HyFetch-1.4.9/hyfetch/distros/parabola.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/parch.py` & `HyFetch-1.4.9/hyfetch/distros/parch.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/pardus.py` & `HyFetch-1.4.9/hyfetch/distros/pardus.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/parrot.py` & `HyFetch-1.4.9/hyfetch/distros/parrot.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/parsix.py` & `HyFetch-1.4.9/hyfetch/distros/parsix.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/pcbsd.py` & `HyFetch-1.4.9/hyfetch/distros/pcbsd.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/pclinuxos.py` & `HyFetch-1.4.9/hyfetch/distros/pclinuxos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/pearos.py` & `HyFetch-1.4.9/hyfetch/distros/pearos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/pengwin.py` & `HyFetch-1.4.9/hyfetch/distros/pengwin.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/pentoo.py` & `HyFetch-1.4.9/hyfetch/distros/pentoo.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/peppermint.py` & `HyFetch-1.4.9/hyfetch/distros/peppermint.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/pikaos.py` & `HyFetch-1.4.9/hyfetch/distros/pikaos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/pisi.py` & `HyFetch-1.4.9/hyfetch/distros/pisi.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/pnm_linux.py` & `HyFetch-1.4.9/hyfetch/distros/pnm_linux.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/pop__os.py` & `HyFetch-1.4.9/hyfetch/distros/pop__os.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/porteus.py` & `HyFetch-1.4.9/hyfetch/distros/porteus.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/postmarketos.py` & `HyFetch-1.4.9/hyfetch/distros/postmarketos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/profelis_sambabox.py` & `HyFetch-1.4.9/hyfetch/distros/profelis_sambabox.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/proxmox.py` & `HyFetch-1.4.9/hyfetch/distros/proxmox.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/puffos.py` & `HyFetch-1.4.9/hyfetch/distros/puffos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/puppy.py` & `HyFetch-1.4.9/hyfetch/distros/puppy.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/pureos.py` & `HyFetch-1.4.9/hyfetch/distros/pureos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/q4os.py` & `HyFetch-1.4.9/hyfetch/distros/q4os.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/qubes.py` & `HyFetch-1.4.9/hyfetch/distros/qubes.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/qubyt.py` & `HyFetch-1.4.9/hyfetch/distros/qubyt.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/quibian.py` & `HyFetch-1.4.9/hyfetch/distros/quibian.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/radix.py` & `HyFetch-1.4.9/hyfetch/distros/radix.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/raspbian.py` & `HyFetch-1.4.9/hyfetch/distros/raspbian.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/ravynos.py` & `HyFetch-1.4.9/hyfetch/distros/ravynos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/reborn_os.py` & `HyFetch-1.4.9/hyfetch/distros/reborn_os.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/red_star.py` & `HyFetch-1.4.9/hyfetch/distros/red_star.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/redcore.py` & `HyFetch-1.4.9/hyfetch/distros/redcore.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/redhat.py` & `HyFetch-1.4.9/hyfetch/distros/redhat.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/redhat_old.py` & `HyFetch-1.4.9/hyfetch/distros/redhat_old.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/refracted_devuan.py` & `HyFetch-1.4.9/hyfetch/distros/refracted_devuan.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/regata.py` & `HyFetch-1.4.9/hyfetch/distros/regata.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/regolith.py` & `HyFetch-1.4.9/hyfetch/distros/regolith.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/rhaymos.py` & `HyFetch-1.4.9/hyfetch/distros/rhaymos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/rocky.py` & `HyFetch-1.4.9/hyfetch/distros/rocky.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/rosa.py` & `HyFetch-1.4.9/hyfetch/distros/rosa.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/sabayon.py` & `HyFetch-1.4.9/hyfetch/distros/sabayon.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/sabotage.py` & `HyFetch-1.4.9/hyfetch/distros/sabotage.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/salentos.py` & `HyFetch-1.4.9/hyfetch/distros/salentos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/salient_os.py` & `HyFetch-1.4.9/hyfetch/distros/salient_os.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/sasanqua.py` & `HyFetch-1.4.9/hyfetch/distros/sasanqua.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/scientific.py` & `HyFetch-1.4.9/hyfetch/distros/scientific.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/septor.py` & `HyFetch-1.4.9/hyfetch/distros/septor.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/serene.py` & `HyFetch-1.4.9/hyfetch/distros/serene.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/sharklinux.py` & `HyFetch-1.4.9/hyfetch/distros/sharklinux.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/shastraos.py` & `HyFetch-1.4.9/hyfetch/distros/shastraos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/siduction.py` & `HyFetch-1.4.9/hyfetch/distros/siduction.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/skiffos.py` & `HyFetch-1.4.9/hyfetch/distros/skiffos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/slackware.py` & `HyFetch-1.4.9/hyfetch/distros/slackware.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/slitaz.py` & `HyFetch-1.4.9/hyfetch/distros/slitaz.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/smartos.py` & `HyFetch-1.4.9/hyfetch/distros/smartos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/soda.py` & `HyFetch-1.4.9/hyfetch/distros/soda.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/solus.py` & `HyFetch-1.4.9/hyfetch/distros/solus.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/source_mage.py` & `HyFetch-1.4.9/hyfetch/distros/source_mage.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/sparky.py` & `HyFetch-1.4.9/hyfetch/distros/sparky.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/star.py` & `HyFetch-1.4.9/hyfetch/distros/star.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/steamos.py` & `HyFetch-1.4.9/hyfetch/distros/steamos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/stock_linux.py` & `HyFetch-1.4.9/hyfetch/distros/stock_linux.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/sulin.py` & `HyFetch-1.4.9/hyfetch/distros/sulin.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/swagarch.py` & `HyFetch-1.4.9/hyfetch/distros/swagarch.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/tails.py` & `HyFetch-1.4.9/hyfetch/distros/tails.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/tearch.py` & `HyFetch-1.4.9/hyfetch/distros/tearch.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/torizoncore.py` & `HyFetch-1.4.9/hyfetch/distros/torizoncore.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/trisquel.py` & `HyFetch-1.4.9/hyfetch/distros/trisquel.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/twister.py` & `HyFetch-1.4.9/hyfetch/distros/twister.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/ubuntu.py` & `HyFetch-1.4.9/hyfetch/distros/ubuntu.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/ubuntu_budgie.py` & `HyFetch-1.4.9/hyfetch/distros/ubuntu_budgie.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/ubuntu_cinnamon.py` & `HyFetch-1.4.9/hyfetch/distros/ubuntu_cinnamon.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/ubuntu_gnome.py` & `HyFetch-1.4.9/hyfetch/distros/ubuntu_gnome.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/ubuntu_kylin.py` & `HyFetch-1.4.9/hyfetch/distros/ubuntu_kylin.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/ubuntu_mate.py` & `HyFetch-1.4.9/hyfetch/distros/ubuntu_mate.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/ubuntu_old.py` & `HyFetch-1.4.9/hyfetch/distros/ubuntu_old.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/ubuntu_old02.py` & `HyFetch-1.4.9/hyfetch/distros/ubuntu_old02.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/ubuntu_studio.py` & `HyFetch-1.4.9/hyfetch/distros/ubuntu_studio.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/ubuntu_sway.py` & `HyFetch-1.4.9/hyfetch/distros/ubuntu_sway.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/ultramarine_linux.py` & `HyFetch-1.4.9/hyfetch/distros/ultramarine_linux.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/univalent.py` & `HyFetch-1.4.9/hyfetch/distros/univalent.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/univention.py` & `HyFetch-1.4.9/hyfetch/distros/univention.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/uos.py` & `HyFetch-1.4.9/hyfetch/distros/uos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/urukos.py` & `HyFetch-1.4.9/hyfetch/distros/urukos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/uwuntu.py` & `HyFetch-1.4.9/hyfetch/distros/uwuntu.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/vanilla.py` & `HyFetch-1.4.9/hyfetch/distros/vanilla.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/venom.py` & `HyFetch-1.4.9/hyfetch/distros/venom.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/vnux.py` & `HyFetch-1.4.9/hyfetch/distros/vnux.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/void.py` & `HyFetch-1.4.9/hyfetch/distros/void.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/vzlinux.py` & `HyFetch-1.4.9/hyfetch/distros/vzlinux.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/wii_linux_ngx.py` & `HyFetch-1.4.9/hyfetch/distros/wii_linux_ngx.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/windows.py` & `HyFetch-1.4.9/hyfetch/distros/windows.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/windows_10.py` & `HyFetch-1.4.9/hyfetch/distros/windows_10.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/windows_11.py` & `HyFetch-1.4.9/hyfetch/distros/windows_11.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/xferience.py` & `HyFetch-1.4.9/hyfetch/distros/xferience.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/xubuntu.py` & `HyFetch-1.4.9/hyfetch/distros/xubuntu.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/yiffos.py` & `HyFetch-1.4.9/hyfetch/distros/yiffos.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/distros/zorin.py` & `HyFetch-1.4.9/hyfetch/distros/zorin.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/main.py` & `HyFetch-1.4.9/hyfetch/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
 import argparse
+import datetime
 import json
 import random
 import traceback
 from itertools import permutations
 from math import ceil
 
-from . import termenv, neofetch_util
+from . import termenv, neofetch_util, pride_month
 from .color_scale import Scale
 from .color_util import clear_screen
 from .constants import *
 from .models import Config
 from .neofetch_util import *
 from .presets import PRESETS
 
@@ -28,14 +29,15 @@
         try:
             return Config.from_dict(json.loads(CONFIG_PATH.read_text('utf-8')))
         except KeyError:
             return create_config()
 
     return create_config()
 
+
 def create_config() -> Config:
     """
     Create config interactively
 
     :return: Config object (automatically stored)
     """
     # Detect terminal environment (doesn't work on Windows)
@@ -60,18 +62,20 @@
     def print_title_prompt(prompt: str):
         printc(f'&a{option_counter}. {prompt}')
 
     ##############################
     # 0. Check term size
     try:
         term_len, term_lines = os.get_terminal_size().columns, os.get_terminal_size().lines
-        if term_len < 2 * asc_width + 4 or term_lines < 30:
+        term_len_min = 2 * asc_width + 4
+        term_lines_min = 30
+        if term_len < term_len_min or term_lines < term_lines_min:
             printc(f'&cWarning: Your terminal is too small ({term_len} * {term_lines}). \n'
-                   f'Please resize it for better experience.')
-            input('Press any key to ignore...')
+                   f'Please resize it to at least ({term_len_min} * {term_lines_min}) for better experience.')
+            input('Press enter to ignore...')
     except:
         # print('Warning: We cannot detect your terminal size.')
         pass
 
     ##############################
     # 1. Select color system
     def select_color_system():
@@ -291,51 +295,63 @@
     save = literal_input(f'Save config?', ['y', 'n'], 'y')
     if save == 'y':
         c.save()
 
     return c
 
 
-def run():
-    # Optional: Import readline
-    try:
-        import readline
-    except ModuleNotFoundError:
-        pass
-
-    # On Windows: Try to fix color rendering if not in git bash
-    if IS_WINDOWS:
-        import colorama
-        colorama.just_fix_windows_console()
-
+def create_parser() -> argparse.ArgumentParser:
     # Create CLI
     hyfetch = color('&l&bhyfetch&~&L')
-    parser = argparse.ArgumentParser(description=color(f'{hyfetch} - neofetch with flags <3'))
+    parser = argparse.ArgumentParser(description=color(f'{hyfetch} - neofetch with flags <3'), prog="hyfetch")
 
-    parser.add_argument('-c', '--config', action='store_true', help=color(f'Configure {hyfetch}'))
+    parser.add_argument('-c', '--config', action='store_true', help=color(f'Configure hyfetch'))
     parser.add_argument('-C', '--config-file', dest='config_file', default=CONFIG_PATH, help=f'Use another config file')
-    parser.add_argument('-p', '--preset', help=f'Use preset', choices=PRESETS.keys())
+    parser.add_argument('-p', '--preset', help=f'Use preset', choices=list(PRESETS.keys()))
     parser.add_argument('-m', '--mode', help=f'Color mode', choices=['8bit', 'rgb'])
     parser.add_argument('-b', '--backend', help=f'Choose a *fetch backend', choices=['neofetch', 'fastfetch', 'fastfetch-old'])
+    parser.add_argument('--args', help=f'Additional arguments pass-through to backend')
     parser.add_argument('--c-scale', dest='scale', help=f'Lighten colors by a multiplier', type=float)
     parser.add_argument('--c-set-l', dest='light', help=f'Set lightness value of the colors', type=float)
+    parser.add_argument('--c-overlay', action='store_true', dest='overlay', help=f'Use experimental overlay color adjusting instead of HSL lightness')
     parser.add_argument('-V', '--version', dest='version', action='store_true', help=f'Check version')
+    parser.add_argument('--june', action='store_true', help=f'Show pride month easter egg')
     parser.add_argument('--debug', action='store_true', help=f'Debug mode')
 
     parser.add_argument('--distro', '--test-distro', dest='distro', help=f'Test for a specific distro')
     parser.add_argument('--ascii-file', help='Use a specific file for the ascii art')
 
     # Hidden debug arguments
     # --test-print: Print the ascii distro and exit
     parser.add_argument('--test-print', action='store_true', help=argparse.SUPPRESS)
     # --ask-exit: Ask for input before exiting
     parser.add_argument('--ask-exit', action='store_true', help=argparse.SUPPRESS)
 
+    return parser
+
+
+def run():
+    # Optional: Import readline
+    try:
+        import readline
+    except ModuleNotFoundError:
+        pass
+
+    # On Windows: Try to fix color rendering if not in git bash
+    if IS_WINDOWS:
+        import colorama
+        colorama.just_fix_windows_console()
+
+    parser = create_parser()
     args = parser.parse_args()
 
+    # Use a custom distro
+    GLOBAL_CFG.override_distro = args.distro
+    GLOBAL_CFG.use_overlay = args.overlay
+
     if args.version:
         print(f'Version is {VERSION}')
         return
 
     # Ensure git bash for windows
     ensure_git_bash()
     check_windows_cmd()
@@ -354,14 +370,28 @@
         # If provided file does not exist use default config
         if not args.config_file.is_file():
             args.config_file = CONFIG_PATH
 
     # Load config or create config
     config = create_config() if args.config else check_config(args.config_file)
 
+    # Check if it's June (pride month)
+    now = datetime.datetime.now()
+    if now.month == 6 and now.year not in config.pride_month_shown:
+        args.june = True
+
+    if args.june:
+        pride_month.start_animation()
+        print()
+        print("Happy pride month!")
+        print("(You can always view the animation again with `hyfetch --june`)")
+        print()
+        config.pride_month_shown.append(now.year)
+        config.save()
+
     # Use a custom distro
     GLOBAL_CFG.override_distro = args.distro or config.distro
 
     # Param overwrite config
     if args.preset:
         config.preset = args.preset
     if args.mode:
@@ -384,14 +414,14 @@
     else:
         preset = preset.set_light_dl(config.lightness or GLOBAL_CFG.default_lightness())
 
     # Run
     try:
         asc = get_distro_ascii() if not args.ascii_file else Path(args.ascii_file).read_text("utf-8")
         asc = config.color_align.recolor_ascii(asc, preset)
-        neofetch_util.run(asc, config.backend)
+        neofetch_util.run(asc, config.backend, args.args or '')
     except Exception as e:
         print(f'Error: {e}')
         traceback.print_exc()
 
     if args.ask_exit:
         input('Press any key to exit...')
```

### Comparing `HyFetch-1.4.8/hyfetch/models.py` & `HyFetch-1.4.9/hyfetch/models.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     preset: str
     mode: AnsiMode
     light_dark: LightDark = 'dark'
     lightness: float | None = None
     color_align: ColorAlignment = field(default_factory=lambda: ColorAlignment('horizontal'))
     backend: BackendLiteral = "neofetch"
     distro: str | None = None
+    pride_month_shown: list[int] = field(default_factory=list)
 
     @classmethod
     def from_dict(cls, d: dict):
         d['color_align'] = ColorAlignment.from_dict(d['color_align'])
         return from_dict(cls, d)
 
     def save(self):
```

### Comparing `HyFetch-1.4.8/hyfetch/neofetch_util.py` & `HyFetch-1.4.9/hyfetch/neofetch_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from .distros import distro_detector
 from .presets import ColorProfile
 from .serializer import from_dict
 from .types import BackendLiteral, ColorAlignMode
 
 RE_NEOFETCH_COLOR = re.compile('\\${c[0-9]}')
 
+
 def literal_input(prompt: str, options: Iterable[str], default: str, show_ops: bool = True) -> str:
     """
     Ask the user to provide an input among a list of options
 
     :param prompt: Input prompt
     :param options: Options
     :param default: Default option
@@ -64,14 +65,15 @@
         print(f'Invalid selection! {selection} is not one of {"|".join(options)}')
         selection = input('> ').lower() or default
 
     print()
 
     return find_selection(selection)
 
+
 def term_size() -> tuple[int, int]:
     """
     Get terminal size
     :return:
     """
     try:
         return os.get_terminal_size().columns, os.get_terminal_size().lines
@@ -332,57 +334,61 @@
     return normalize_ascii(asc)
 
 
 def get_distro_name():
     return run_neofetch_cmd('ascii_distro_name', True)
 
 
-def run(asc: str, backend: BackendLiteral):
+def run(asc: str, backend: BackendLiteral, args: str = ''):
     if backend == "neofetch":
-        return run_neofetch(asc)
+        return run_neofetch(asc, args)
     if backend == "fastfetch":
-        return run_fastfetch(asc)
+        return run_fastfetch(asc, args)
     if backend == "fastfetch-old":
-        return run_fastfetch(asc, legacy=True)
+        return run_fastfetch(asc, args, legacy=True)
 
 
-def run_neofetch(asc: str):
+def run_neofetch(asc: str, args: str = ''):
     """
     Run neofetch with colors
 
     :param asc: Ascii art
+    :param args: Additional arguments to pass to neofetch
     """
     # Escape backslashes here because backslashes are escaped in neofetch for printf
     asc = asc.replace('\\', '\\\\')
 
     # Write temp file
     with TemporaryDirectory() as tmp_dir:
         tmp_dir = Path(tmp_dir)
         path = tmp_dir / 'ascii.txt'
         path.write_text(asc)
 
         # Call neofetch with the temp file
-        run_neofetch_cmd(f'--ascii --source {path.absolute()} --ascii-colors')
+        if args:
+            args = ' ' + args
+        run_neofetch_cmd(f'--ascii --source {path.absolute()} --ascii-colors' + args)
 
 
-def run_fastfetch(asc: str, legacy: bool = False):
+def run_fastfetch(asc: str, args: str = '', legacy: bool = False):
     """
     Run neofetch with colors
 
     :param asc: Ascii art
+    :param args: Additional arguments to pass to fastfetch
     :param legacy: Set true when using fastfetch < 1.8.0
     """
     # Write temp file
     with TemporaryDirectory() as tmp_dir:
         tmp_dir = Path(tmp_dir)
         path = tmp_dir / 'ascii.txt'
         path.write_text(asc)
 
         # Call fastfetch with the temp file
-        proc = subprocess.run(['fastfetch', '--raw' if legacy else '--file-raw', path.absolute()])
+        proc = subprocess.run(['fastfetch', '--raw' if legacy else '--file-raw', path.absolute(), *shlex.split(args)])
         if proc.returncode == 144:
             printc("&6Error code 144 detected: Please upgrade fastfetch to >=1.8.0 or use the 'fastfetch-old' backend")
 
 
 def get_fore_back(distro: str | None = None) -> tuple[int, int] | None:
     """
     Get recommended foreground-background configuration for distro, or None if the distro ascii is
@@ -400,15 +406,14 @@
             return v
     return None
 
 
 # Foreground-background recommendation
 fore_back = {
     'fedora': (2, 1),
-    'ubuntu': (2, 1),
     'kubuntu': (2, 1),
     'lubuntu': (2, 1),
     'xubuntu': (2, 1),
     'ubuntu-cinnamon': (2, 1),
     'ubuntu-kylin': (2, 1),
     'ubuntu-mate': (2, 1),
     'ubuntu-studio': (2, 1),
```

### Comparing `HyFetch-1.4.8/hyfetch/presets.py` & `HyFetch-1.4.9/hyfetch/presets.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,19 +115,43 @@
         """
         Set HSL lightness value with respect to dark/light terminals
 
         :param light: Lightness value (0-1)
         :param term: Terminal color (can be "dark" or "light")
         :return: New color profile (original isn't modified)
         """
+        if GLOBAL_CFG.use_overlay:
+            return self.overlay_dl(light, term)
+
         term = term or GLOBAL_CFG.light_dark()
         assert term.lower() in ['light', 'dark']
         at_least, at_most = (True, None) if term.lower() == 'dark' else (None, True)
         return self.set_light_raw(light, at_least, at_most)
 
+    def overlay_raw(self, color: RGB, alpha: float) -> 'ColorProfile':
+        """
+        Overlay a color on top of the color profile
+
+        :param color: Color to overlay
+        :param alpha: Alpha value (0-1)
+        :return: New color profile (original isn't modified)
+        """
+        return ColorProfile([c.overlay(color, alpha) for c in self.colors])
+
+    def overlay_dl(self, light: float, term: LightDark | None = None):
+        """
+        Same as set_light_dl except that this function uses RGB overlaying instead of HSL lightness change
+        """
+        term = term or GLOBAL_CFG.light_dark()
+        assert term.lower() in ['light', 'dark']
+
+        # If it's light bg, overlay black, else overlay white
+        overlay_color = RGB.from_hex('#000000' if term.lower() == 'light' else '#FFFFFF')
+        return self.overlay_raw(overlay_color, abs(light - 0.5) * 2)
+
     def set_light_dl_def(self, term: LightDark | None = None):
         """
         Set default lightness with respect to dark/light terminals
 
         :param term: Terminal color (can be "dark" or "light")
         :return: New color profile (original isn't modified)
         """
@@ -474,61 +498,30 @@
         '#AEB1AA',
         '#740194',
     ]),
 
     'autoromantic': ColorProfile([ # symbol interpreted
         '#99D9EA',
         '#99D9EA',
-        '#99D9EA',
-        '#99D9EA',
-        '#99D9EA',
-        '#000000',
-        '#3DA542',
         '#3DA542',
-        '#000000',
-        '#7F7F7F',
-        '#7F7F7F',
-        '#7F7F7F',
         '#7F7F7F',
         '#7F7F7F',
     ]),
 
     # i didn't expect this one to work. cool!
-    'boyflux2': ColorProfile([
+    'boyflux2': ColorProfile(ColorProfile([
         '#E48AE4',
         '#9A81B4',
         '#55BFAB',
         '#FFFFFF',
         '#A8A8A8',
         '#81D5EF',
-        '#81D5EF',
-        '#81D5EF',
-        '#81D5EF',
-        '#81D5EF',
-        '#69ABE5',
-        '#69ABE5',
-        '#69ABE5',
-        '#69ABE5',
-        '#69ABE5',
-        '#69ABE5',
-        '#69ABE5',
-        '#69ABE5',
         '#69ABE5',
-        '#69ABE5',
-        '#5276D4',
-        '#5276D4',
-        '#5276D4',
-        '#5276D4',
-        '#5276D4',
         '#5276D4',
-        '#5276D4',
-        '#5276D4',
-        '#5276D4',
-        '#5276D4',
-    ]),
+    ]).with_weights([1, 1, 1, 1, 1, 5, 5, 5])),
 
     "finsexual": ColorProfile([
         "#B18EDF",
         "#D7B1E2",
         "#F7CDE9",
         "#F39FCE",
         "#EA7BB3",
```

### Comparing `HyFetch-1.4.8/hyfetch/scripts/neowofetch` & `HyFetch-1.4.9/hyfetch/scripts/neowofetch`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-version=7.3.8
+version=7.3.9
 
 # Fallback to a value of '5' for shells which support bash
 # but do not set the 'BASH_' shell variables (osh).
 bash_version=${BASH_VERSINFO[0]:-5}
 shopt -s eval_unsafe_arith &>/dev/null
 
 sys_locale=${LANG:-C}
@@ -832,29 +832,29 @@
 # Default: 'auto'
 # Values:  'auto', 'distro_name'
 # Flag:    --ascii_distro
 #
 # NOTE: AIX, AlmaLinux, Alpine, Alter, Amazon, AmogOS, Anarchy, Android, Antergos, antiX, AOSC OS,
 # AOSC OS/Retro, Aperio GNU/Linux, Aperture, Apricity, Arch, ArchBox, Archcraft, archcraft_ascii,
 # archcraft_minimal, ARCHlabs, ArchMerge, ArchStrike, ArcoLinux, ArseLinux, Artix, Arya, Asahi,
-# Aster, AsteroidOS, astOS, Bedrock, BigLinux, Bitrig, BlackArch, blackPanther, BLAG, BlankOn,
-# BlueLight, Bodhi, bonsai, BSD, BunsenLabs, CachyOS, Calculate, CalinixOS, Carbs, CBL-Mariner,
-# CelOS, Center, CentOS, Chakra, ChaletOS, Chapeau, ChonkySealOS, Chrom, Cleanjaro, Clear Linux OS,
-# ClearOS, Clover, Cobalt, Condres, Container Linux by CoreOS, CRUX, Crystal Linux, Cucumber,
-# CutefishOS, CuteOS, CyberOS, dahlia, DarkOs, Darwin, Debian, Deepin, DesaOS, Devuan, DietPi,
-# DracOS, DragonFly, Drauger, Droidian, Elementary, Elive, EncryptOS, EndeavourOS, Endless, Enso,
-# EuroLinux, Exherbo, Exodia Predator OS, Fedora, Feren, Finnix, Floflis, FreeBSD, FreeMiNT,
-# Frugalware, Funtoo, GalliumOS, Garuda, Gentoo, GhostBSD, glaucus, gNewSense, GNOME, GNU,
+# Aster, AsteroidOS, astOS, Astra Linux, Bedrock, BigLinux, Bitrig, BlackArch, blackPanther, BLAG,
+# BlankOn, BlueLight, Bodhi, bonsai, BSD, BunsenLabs, CachyOS, Calculate, CalinixOS, Carbs, CBL-
+# Mariner, CelOS, Center, CentOS, Chakra, ChaletOS, Chapeau, ChonkySealOS, Chrom, Cleanjaro, Clear
+# Linux OS, ClearOS, Clover, Cobalt, Condres, Container Linux by CoreOS, CRUX, Crystal Linux,
+# Cucumber, CutefishOS, CuteOS, CyberOS, dahlia, DarkOs, Darwin, Debian, Deepin, DesaOS, Devuan,
+# DietPi, DracOS, DragonFly, Drauger, Droidian, Elementary, Elive, EncryptOS, EndeavourOS, Endless,
+# Enso, EuroLinux, Exherbo, Exodia Predator OS, Fedora, FemboyOS, Feren, Finnix, Floflis, FreeBSD,
+# FreeMiNT, Frugalware, Funtoo, GalliumOS, Garuda, Gentoo, GhostBSD, glaucus, gNewSense, GNOME, GNU,
 # GoboLinux, GrapheneOS, Grombyang, Guix, Haiku, HamoniKR, HarDClanZ, Hash, Huayra, Hybrid, HydroOS,
 # Hyperbola, iglunix, instantOS, IRIX, Itc, januslinux, Kaisen, Kali, KaOS, KDE, Kibojoe, Kogaion,
 # Korora, KrassOS, KSLinux, Kubuntu, LangitKetujuh, LaxerOS, LEDE, LibreELEC, Linspire, Linux, Linux
 # Lite, Linux Mint, Linux Mint Old, Live Raizo, LMDE, Lubuntu, Lunar, mac, Mageia, MagpieOS,
 # Mandriva, Manjaro, MassOS, MatuusOS, Maui, Mer, Minix, MIRACLE LINUX, MX, Namib, NekOS, Neptune,
-# NetBSD, Netrunner, Nitrux, NixOS, NomadBSD, Nurunner, NuTyX, Obarun, OBRevenge, OmniOS, Open
-# Source Media Center, OpenBSD, openEuler, OpenIndiana, openmamba, OpenMandriva, OpenStage,
+# NetBSD, Netrunner, Nitrux, NixOS, Nobara, NomadBSD, Nurunner, NuTyX, Obarun, OBRevenge, OmniOS,
+# Open Source Media Center, OpenBSD, openEuler, OpenIndiana, openmamba, OpenMandriva, OpenStage,
 # openSUSE, openSUSE Leap, openSUSE Tumbleweed, OpenWrt, OPNsense, Oracle, orchid, OS Elbrus,
 # PacBSD, Parabola, parch, Pardus, Parrot, Parsix, PCBSD, PCLinuxOS, pearOS, Pengwin, Pentoo,
 # Peppermint, PikaOS, Pisi, PNM Linux, Pop!_OS, Porteus, PostMarketOS, Profelis SambaBOX, Proxmox,
 # PuffOS, Puppy, PureOS, Q4OS, Qubes, Qubyt, Quibian, Radix, Raspbian, ravynOS, Reborn OS, Red Star,
 # Redcore, Redhat, Refracted Devuan, Regata, Regolith, RhaymOS, rocky, Rosa, Sabayon, sabotage,
 # Sailfish, SalentOS, Salient OS, Sasanqua, Scientific, semc, Septor, Serene, SharkLinux, ShastraOS,
 # Siduction, SkiffOS, Slackware, SliTaz, SmartOS, Soda, Solus, Source Mage, Sparky, Star, SteamOS,
@@ -1096,14 +1096,27 @@
                 esac
 
             elif [[ -f /etc/lindowsos-version ]]; then
                 case $distro_shorthand in
                     on|tiny) distro="LindowsOS" ;;
                     *) distro="$(awk '/Version/ {print $2,$3}' /etc/lindowsos-version)"
                 esac
+        
+            elif [[ -f /etc/astra_version ]]; then
+                distro="Astra Linux"
+                distro_version="$(sed -nr 's/^[^0-9]*(([0-9]+\.)*[0-9]+).*/\1/p' < /etc/astra_version)"
+                if [[ $distro_version == "2.12"* ]]; then
+                    distro_codename="ALCE"
+                else
+                    distro_codename="ALSE"
+                fi
+                case $distro_shorthand in
+                    on|tiny) ;;
+                    *) distro="${distro} ${distro_version} ${distro_codename}"
+                esac
 
             elif type -p pveversion >/dev/null; then
                 case $distro_shorthand in
                     on|tiny) distro="Proxmox VE" ;;
                     *)
                         distro=$(pveversion)
                         distro=${distro#pve-manager/}
@@ -1241,22 +1254,48 @@
                                 distro=$(<"/usr/local/opnsense/version/opnsense")
                                 distro="OPNsense ${distro%-*}"
                         esac
                     fi
                 fi
             fi
 
+            # Gets the windows tag caption (ie `Microsoft Windows 11 Pro Insider Preview`)
+            #
+            # Then removes the `Microsoft` and `Windows` part and gets the current
+            # version of Windows (old code reported Windows 10 even if host runs Windows 11).
+            #
+            # Finally, we decline it in three versions :
+            #
+            # - The `on`   version (ie `[Windows 11.0.25330]`)
+            # - The `tiny` version (ie `Windows 11`)
+            # - The `any`  version (ie `on Windows 11 Pro Insider Preview`)
             if [[ $(< /proc/version) == *Microsoft* || $kernel_version == *Microsoft* ]]; then
-                windows_version=$(wmic.exe os get Version)
-                windows_version=$(trim "${windows_version/Version}")
+
+                windows_version_verbose=$(reg query "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion" -v ProductName | grep REG_)
+                windows_version_verbose=$(trim "${windows_version_verbose/ProductName}")
+                windows_version_verbose=$(trim "${windows_version_verbose/REG_SZ}")buildnumber=$(reg query "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion" -v CurrentBuildNumber | grep REG_)
+                windows_version_verbose=$(trim "${windows_version_verbose/Windows}")
+                windows_buildnumber=$(reg query "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion" -v CurrentBuildNumber | grep REG_)               
+                windows_buildnumber=${buildnumber/CurrentBuildNumber}
+                windows_buildnumber=${buildnumber/REG_SZ}
+                if [[ "$windows_version_verbose" == *"10"* ]] && (( windows_buildnumber >= 22000 )); then
+                    windows_version_verbose=${windows_version_verbose/10/11}
+                fi
+
+                windows_version_current=${windows_version_verbose//[^[:digit:]]/}
+
+                windows_version_number_long=$(wmic.exe os get Version)
+                windows_version_number_long=$(trim "${windows_version_number_long/Version}")
+                windows_version_number_long=$(trim "${windows_version_number_long}")
+                windows_version_number_long="${windows_version_current}${windows_version_number_long:2}"
 
                 case $distro_shorthand in
-                    on)   distro+=" [Windows $windows_version]" ;;
-                    tiny) distro="Windows ${windows_version::2}" ;;
-                    *)    distro+=" on Windows $windows_version" ;;
+                    on)   distro+=" [Windows $windows_version_number_long]" ;;
+                    tiny) distro=" Windows $windows_version_current" ;;
+                    *)    distro+=" on Windows $windows_version_verbose" ;;
                 esac
 
             # Chrome OS doesn't conform to the /etc/*-release standard.
             # While the file is a series of variables they can't be sourced
             # by the shell since the values aren't quoted.
             elif [[ -f /etc/lsb-release && $(< /etc/lsb-release) == *CHROMEOS* ]]; then
                 distro='Chrome OS'
@@ -1345,17 +1384,25 @@
             distro="iOS $osx_version"
 
             # "uname -m" doesn't print architecture on iOS.
             os_arch=off
         ;;
 
         Windows)
-            distro=$(wmic os get Caption)
-            distro=${distro/Caption}
-            distro=${distro/Microsoft }
+            distro=$(reg query "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion" -v ProductName | grep REG_)
+            distro=${distro/ProductName}
+            distro=${distro/REG_SZ}
+            buildnumber=$(reg query "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion" -v CurrentBuildNumber | grep REG_)
+            buildnumber=${buildnumber/CurrentBuildNumber}
+            buildnumber=${buildnumber/REG_SZ}
+
+            # If the value of "ProductName" obtained is Windows 10 and the value of "CurrentBuildNumber" is greater than 22000, then the actual operating system version is Windows 11.
+            if [[ "$distro" == *"Windows 10"* ]] && (( buildnumber >= 22000 )); then
+                distro=${distro/Windows 10/Windows 11}
+            fi
         ;;
 
         Solaris|illumos)
             case $distro_shorthand in
                 on|tiny) distro=$(awk 'NR==1 {print $1,$3}' /etc/release) ;;
                 *)       distro=$(awk 'NR==1 {print $1,$2,$3}' /etc/release) ;;
             esac
@@ -1714,15 +1761,15 @@
                 *)
                     hostname=$(hostname -f)
                 ;;
             esac
         ;;
         *)
             hostname=${HOSTNAME:-$(hostname)}
-            hostname=${hostname%.*}
+            hostname=${hostname%%.*}
         ;;
     esac
 
     title=${title_color}${bold}${user}${at_color}@${title_color}${bold}${hostname}
     length=$((${#user} + ${#hostname} + 1))
 }
 
@@ -2053,15 +2100,15 @@
             # Count chocolatey packages.
             # [[ -d /c/ProgramData/chocolatey/lib ]] && \
             #     dir /c/ProgramData/chocolatey/lib/*
             # has choco && tot choco list --localonly
             has choco && dir "$ProgramData"/chocolatey/lib/*
 
             # Count winget
-            has winget && tot winget list
+            has winget && tot winget list --accept-source-agreements
         ;;
 
         Haiku)
             has pkgman && dir /boot/system/package-links/*
             packages=${packages/pkgman/depot}
         ;;
 
@@ -2220,14 +2267,18 @@
         *)
             ((wm_run != 1)) && get_wm
 
             # Temporary support for Regolith Linux
             if [[ $DESKTOP_SESSION == *regolith ]]; then
                 de=Regolith
 
+            # Added support Fly for Astra Linux
+            elif [[ $DESKTOP_SESSION == fly ]]; then
+                de=Fly
+
             elif [[ $XDG_CURRENT_DESKTOP ]]; then
                 de=${XDG_CURRENT_DESKTOP/X\-}
                 de=${de/Budgie:GNOME/Budgie}
                 de=${de/:Unity7:ubuntu}
 
             elif [[ $DESKTOP_SESSION ]]; then
                 de=${DESKTOP_SESSION##*/}
@@ -2613,14 +2664,24 @@
 
         LeftWM*)
             if command -v leftwm-theme &> /dev/null
             then
                 wm_theme=$(leftwm-theme status | grep "Your current theme" | sed -e 's/Your current theme is //g' -e 's/\,.*$//g')
             fi
         ;;
+        
+        fly-wm)
+            fly_config_file
+            if grep -q 'DecorTheme' "${fly_config_file}" 2>/dev/null; then
+                wm_theme=$(awk -F'=' '/^DecorTheme/{print $2}' "${fly_config_file}")
+            fi
+            if [ -z "$wm_theme" ] || [ "$wm_theme" = "Not Found" ]; then
+                wm_theme=Default
+            fi
+        ;;
     esac
 
     wm_theme=$(trim_quotes "$wm_theme")
 }
 
 get_cpu() {
     case $os in
@@ -3876,14 +3937,36 @@
                 ' {/etc/xdg,/etc/xdg/*,"$XDG_CONFIG_HOME"}/lxqt/lxqt.con?); then
                     err "Theme: Can't read LXQt config files. Unsetting Qt theme."
                     unset qt_theme
                 fi
                 shopt -u nullglob
             ;;
 
+            "Fly")
+                fly_config_file
+                if [[ $fly == "ColorScheme" ]]; then
+                    fly_theme="$(
+                        basename "$(
+                            awk -F '=' '/^'"${fly}"'/{print $2}' "${HOME}/.fly/paletterc"
+                        )"
+                    )"
+                    if [[ $wm_theme == "Default" && $fly_theme != *"FlyDefault"* ]]; then
+                        fly_theme=$(awk -F '=' '/^'"${fly}"'/{print $2}'\
+                                        "${HOME}/.config/fly-admin-themerc")
+                    fi
+                elif [[ $fly == "IconTheme" ]]; then
+                     fly_theme=$(awk -F '=' '/^'"${fly}"'/{print $2}' "${fly_config_file}")
+                elif [[ $fly == "DefaultFont" ]]; then
+                    fly_theme=$(awk -F'=' '/^'"${fly}"'/\
+                                    {gsub(/"/, "", $2); \
+                                    sub(/-.*/, "", $2); \
+                                    print $2}' "${fly_config_file}")
+                fi
+                fly_theme+=" [$de], "
+            ;;
         esac
 
         # Check for general GTK2 Theme.
         if [[ -z "$gtk2_theme" ]]; then
             if [[ -n "$GTK2_RC_FILES" ]]; then
                 IFS=: read -ra rc_files <<< "$GTK2_RC_FILES"
                 gtk2_theme="$(grep "^[^#]*${name}" "${rc_files[@]}")"
@@ -4005,14 +4088,15 @@
                     theme+="], $1 [$2"
                     cur_theme="$1"
                 fi
             fi
         }
         theme=''
         local cur_theme=''
+        append_theme "$fly_theme" 'Fly'
         append_theme "$qt_theme" 'Qt'
         append_theme "$gtk2_theme" 'GTK2'
         append_theme "$gtk3_theme" 'GTK3'
 
         # Final string.
         if [[ -n "$theme" ]]; then
           theme+=']'
@@ -4032,41 +4116,42 @@
     name="gtk-theme-name"
     gsettings="gtk-theme"
     gconf="gtk_theme"
     xfconf="/Net/ThemeName"
     kde="widgetStyle"
     lxqt="style"
     qt5ct="style=" # There is a property called 'stylesheets'.
-
+    fly="ColorScheme"
 
     get_style
 }
 
 get_icons() {
     name="gtk-icon-theme-name"
     gsettings="icon-theme"
     gconf="icon_theme"
     xfconf="/Net/IconThemeName"
     kde="Theme"
     lxqt="icon_theme"
     qt5ct="icon_theme"
-
+    fly="IconTheme"
 
     get_style
     icons="$theme"
 }
 
 get_font() {
     name="gtk-font-name"
     gsettings="font-name"
     gconf="font_theme"
     xfconf="/Gtk/FontName"
     kde="font"
     lxqt="font"
     qt5ct="general"
+    fly="DefaultFont"
 
     get_style
     font="$theme"
 }
 
 get_cursor() {
     name="gtk-cursor-theme-name"
@@ -4278,14 +4363,25 @@
             term_font="${term_font//\'}"
         ;;
 
         "konsole" | "yakuake")
             # Get Process ID of current konsole window / tab
             child="$(get_ppid "$$")"
 
+            # Loop while the process name is not "konsole"
+            while [[ "$(ps -p "$(get_ppid "$child")" -o comm=)" != "konsole" ]]; do
+                # Get the parent process ID
+                child="$(get_ppid "$child")"
+
+                # Exit the loop if the parent process ID is 1 (i.e., init)
+                if [[ "$child" == "1" ]]; then
+                    break
+                fi
+            done
+
             QT_BINDIR="$(qtpaths --binaries-dir)" && PATH+=":$QT_BINDIR"
 
             IFS=$'\n' read -d "" -ra konsole_instances \
                 <<< "$(qdbus | awk '/org.kde.'"$term"'/ {print $1}')"
 
             for i in "${konsole_instances[@]}"; do
                 IFS=$'\n' read -d "" -ra konsole_sessions <<< "$(qdbus "$i" | grep -F '/Sessions/')"
@@ -4304,15 +4400,15 @@
             [[ $profile ]] || return
 
             # We could have two profile files for the same profile name, take first match
             profile_filename="$(grep -l "Name=${profile}" "$HOME"/.local/share/konsole/*.profile)"
             profile_filename="${profile_filename/$'\n'*}"
 
             [[ $profile_filename ]] && \
-                term_font="$(awk -F '=|,' '/Font=/ {print $2,$3}' "$profile_filename")"
+                term_font="$(awk -F '=|,' '/^Font=/ {print $2,$3}' "$profile_filename")"
         ;;
 
         "lxterminal"*)
             term_font="$(awk -F '=' '/fontname=/ {print $2; exit}' \
                          "${XDG_CONFIG_HOME}/lxterminal/lxterminal.conf")"
         ;;
 
@@ -5402,15 +5498,15 @@
             pixterm \
                 -tc "$((width / font_width))" \
                 -tr "$((height / font_height))" \
             "$image"
         ;;
 
         "sixel")
-            img2sixel \
+            img2sixel -I \
                 -w "$width" \
                 -h "$height" \
             "$image"
         ;;
 
         "termpix")
             termpix \
@@ -5781,14 +5877,19 @@
         tde_config_dir="${HOME}/.configtde"
 
     fi
 
     tde_config_dir="${tde_config_dir/$'/:'*}"
 }
 
+fly_config_file() {
+    # Return main path the fly config file
+    fly_config_file=${HOME}/.fly/theme/current.themerc
+}
+
 term_padding() {
     # Get terminal padding to properly align cursor.
     [[ -z "$term" ]] && get_term
 
     case $term in
         urxvt*|rxvt-unicode)
             [[ $xrdb ]] || xrdb=$(xrdb -query)
@@ -6075,53 +6176,54 @@
     --ascii_colors x x x x x x  Colors to print the ascii art
     --ascii_distro distro       Which Distro's ascii art to print
 
                                 NOTE: AIX, AlmaLinux, Alpine, Alter, Amazon, AmogOS, Anarchy,
                                 Android, Antergos, antiX, AOSC OS, AOSC OS/Retro, Aperio GNU/Linux,
                                 Aperture, Apricity, Arch, ArchBox, Archcraft, archcraft_ascii,
                                 archcraft_minimal, ARCHlabs, ArchMerge, ArchStrike, ArcoLinux,
-                                ArseLinux, Artix, Arya, Asahi, Aster, AsteroidOS, astOS, Bedrock,
-                                BigLinux, Bitrig, BlackArch, blackPanther, BLAG, BlankOn, BlueLight,
-                                Bodhi, bonsai, BSD, BunsenLabs, CachyOS, Calculate, CalinixOS,
-                                Carbs, CBL-Mariner, CelOS, Center, CentOS, Chakra, ChaletOS,
-                                Chapeau, ChonkySealOS, Chrom, Cleanjaro, Clear Linux OS, ClearOS,
-                                Clover, Cobalt, Condres, Container Linux by CoreOS, CRUX, Crystal
-                                Linux, Cucumber, CutefishOS, CuteOS, CyberOS, dahlia, DarkOs,
-                                Darwin, Debian, Deepin, DesaOS, Devuan, DietPi, DracOS, DragonFly,
-                                Drauger, Droidian, Elementary, Elive, EncryptOS, EndeavourOS,
-                                Endless, Enso, EuroLinux, Exherbo, Exodia Predator OS, Fedora,
-                                Feren, Finnix, Floflis, FreeBSD, FreeMiNT, Frugalware, Funtoo,
-                                GalliumOS, Garuda, Gentoo, GhostBSD, glaucus, gNewSense, GNOME, GNU,
-                                GoboLinux, GrapheneOS, Grombyang, Guix, Haiku, HamoniKR, HarDClanZ,
-                                Hash, Huayra, Hybrid, HydroOS, Hyperbola, iglunix, instantOS, IRIX,
-                                Itc, januslinux, Kaisen, Kali, KaOS, KDE, Kibojoe, Kogaion, Korora,
-                                KrassOS, KSLinux, Kubuntu, LangitKetujuh, LaxerOS, LEDE, LibreELEC,
-                                Linspire, Linux, Linux Lite, Linux Mint, Linux Mint Old, Live Raizo,
-                                LMDE, Lubuntu, Lunar, mac, Mageia, MagpieOS, Mandriva, Manjaro,
-                                MassOS, MatuusOS, Maui, Mer, Minix, MIRACLE LINUX, MX, Namib, NekOS,
-                                Neptune, NetBSD, Netrunner, Nitrux, NixOS, NomadBSD, Nurunner,
-                                NuTyX, Obarun, OBRevenge, OmniOS, Open Source Media Center, OpenBSD,
-                                openEuler, OpenIndiana, openmamba, OpenMandriva, OpenStage,
-                                openSUSE, openSUSE Leap, openSUSE Tumbleweed, OpenWrt, OPNsense,
-                                Oracle, orchid, OS Elbrus, PacBSD, Parabola, parch, Pardus, Parrot,
-                                Parsix, PCBSD, PCLinuxOS, pearOS, Pengwin, Pentoo, Peppermint,
-                                PikaOS, Pisi, PNM Linux, Pop!_OS, Porteus, PostMarketOS, Profelis
-                                SambaBOX, Proxmox, PuffOS, Puppy, PureOS, Q4OS, Qubes, Qubyt,
-                                Quibian, Radix, Raspbian, ravynOS, Reborn OS, Red Star, Redcore,
-                                Redhat, Refracted Devuan, Regata, Regolith, RhaymOS, rocky, Rosa,
-                                Sabayon, sabotage, Sailfish, SalentOS, Salient OS, Sasanqua,
-                                Scientific, semc, Septor, Serene, SharkLinux, ShastraOS, Siduction,
-                                SkiffOS, Slackware, SliTaz, SmartOS, Soda, Solus, Source Mage,
-                                Sparky, Star, SteamOS, Stock Linux, Sulin, SunOS, SwagArch, t2,
-                                Tails, TeArch, TorizonCore, Trisquel, Twister, Ubuntu, Ubuntu
-                                Budgie, Ubuntu Cinnamon, Ubuntu Kylin, Ubuntu MATE, Ubuntu Studio,
-                                Ubuntu Sway, Ubuntu Touch, Ubuntu-GNOME, ubuntu_old02, Ultramarine
-                                Linux, Univalent, Univention, Uos, UrukOS, uwuntu, Vanilla, Venom,
-                                VNux, Void, VzLinux, wii-linux-ngx, Windows, Windows 10, Windows 11,
-                                XFerience, Xubuntu, yiffOS, Zorin have ascii logos.
+                                ArseLinux, Artix, Arya, Asahi, Aster, AsteroidOS, astOS, Astra
+                                Linux, Bedrock, BigLinux, Bitrig, BlackArch, blackPanther, BLAG,
+                                BlankOn, BlueLight, Bodhi, bonsai, BSD, BunsenLabs, CachyOS,
+                                Calculate, CalinixOS, Carbs, CBL-Mariner, CelOS, Center, CentOS,
+                                Chakra, ChaletOS, Chapeau, ChonkySealOS, Chrom, Cleanjaro, Clear
+                                Linux OS, ClearOS, Clover, Cobalt, Condres, Container Linux by
+                                CoreOS, CRUX, Crystal Linux, Cucumber, CutefishOS, CuteOS, CyberOS,
+                                dahlia, DarkOs, Darwin, Debian, Deepin, DesaOS, Devuan, DietPi,
+                                DracOS, DragonFly, Drauger, Droidian, Elementary, Elive, EncryptOS,
+                                EndeavourOS, Endless, Enso, EuroLinux, Exherbo, Exodia Predator OS,
+                                Fedora, FemboyOS, Feren, Finnix, Floflis, FreeBSD, FreeMiNT,
+                                Frugalware, Funtoo, GalliumOS, Garuda, Gentoo, GhostBSD, glaucus,
+                                gNewSense, GNOME, GNU, GoboLinux, GrapheneOS, Grombyang, Guix,
+                                Haiku, HamoniKR, HarDClanZ, Hash, Huayra, Hybrid, HydroOS,
+                                Hyperbola, iglunix, instantOS, IRIX, Itc, januslinux, Kaisen, Kali,
+                                KaOS, KDE, Kibojoe, Kogaion, Korora, KrassOS, KSLinux, Kubuntu,
+                                LangitKetujuh, LaxerOS, LEDE, LibreELEC, Linspire, Linux, Linux
+                                Lite, Linux Mint, Linux Mint Old, Live Raizo, LMDE, Lubuntu, Lunar,
+                                mac, Mageia, MagpieOS, Mandriva, Manjaro, MassOS, MatuusOS, Maui,
+                                Mer, Minix, MIRACLE LINUX, MX, Namib, NekOS, Neptune, NetBSD,
+                                Netrunner, Nitrux, NixOS, Nobara, NomadBSD, Nurunner, NuTyX, Obarun,
+                                OBRevenge, OmniOS, Open Source Media Center, OpenBSD, openEuler,
+                                OpenIndiana, openmamba, OpenMandriva, OpenStage, openSUSE, openSUSE
+                                Leap, openSUSE Tumbleweed, OpenWrt, OPNsense, Oracle, orchid, OS
+                                Elbrus, PacBSD, Parabola, parch, Pardus, Parrot, Parsix, PCBSD,
+                                PCLinuxOS, pearOS, Pengwin, Pentoo, Peppermint, PikaOS, Pisi, PNM
+                                Linux, Pop!_OS, Porteus, PostMarketOS, Profelis SambaBOX, Proxmox,
+                                PuffOS, Puppy, PureOS, Q4OS, Qubes, Qubyt, Quibian, Radix, Raspbian,
+                                ravynOS, Reborn OS, Red Star, Redcore, Redhat, Refracted Devuan,
+                                Regata, Regolith, RhaymOS, rocky, Rosa, Sabayon, sabotage, Sailfish,
+                                SalentOS, Salient OS, Sasanqua, Scientific, semc, Septor, Serene,
+                                SharkLinux, ShastraOS, Siduction, SkiffOS, Slackware, SliTaz,
+                                SmartOS, Soda, Solus, Source Mage, Sparky, Star, SteamOS, Stock
+                                Linux, Sulin, SunOS, SwagArch, t2, Tails, TeArch, TorizonCore,
+                                Trisquel, Twister, Ubuntu, Ubuntu Budgie, Ubuntu Cinnamon, Ubuntu
+                                Kylin, Ubuntu MATE, Ubuntu Studio, Ubuntu Sway, Ubuntu Touch,
+                                Ubuntu-GNOME, ubuntu_old02, Ultramarine Linux, Univalent,
+                                Univention, Uos, UrukOS, uwuntu, Vanilla, Venom, VNux, Void,
+                                VzLinux, wii-linux-ngx, Windows, Windows 10, Windows 11, XFerience,
+                                Xubuntu, yiffOS, Zorin have ascii logos.
 
                                 NOTE: arch, dragonfly, Fedora, LangitKetujuh, nixos, redhat, Ubuntu
                                 have 'old' logo variants, use {distro}_old to use them.
 
                                 NOTE: alpine, android, aoscosretro, arch, arcolinux, artix,
                                 CalinixOS, centos, cleanjaro, crux, debian, dragonfly, elementary,
                                 fedora, freebsd, garuda, gentoo, guix, haiku, hyperbola, kali,
@@ -9138,14 +9240,40 @@
            .:++++++++//////////-
              `-++++++---:::://///.
            `.:///+++.             `
           `.........
 EOF
         ;;
 
+        "FemboyOS"*)
+            set_colors 4
+            read -rd '' ascii_data <<'EOF'
+${c1}MMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMM
+MMMMWKkxkKWMMMMMMMMMMMMMMMMMMMMWKkxkKWMM
+MMMMXo. .;xKWMMMMMMMMMMMMMMMMMMXo. .oXMM
+MMWXx,..'..oXMMMMMMMMMMMMMMMMWKx,  .lXMM
+MMNo. .cOc.,xKWMMMMMMMMMMMMWXx;.....cXMM
+MMXl..;kKl. .oXMMMMMMMMMMWKx;..,ok:.'o0W
+WKx,.cKWNk;..lXMMMMMMMMWKx;..,o0NXl. .oN
+No. .lXMMWKc.,dKWMMMMMMNo..;d0NWMNx,..lX
+Nk:,:kNMMMNk:,ckNMMMMMMNxcxXWMMMMMN0ockN
+MWNNNWMMMMMWNNNWMMMMMMMMWWWMMMMMMMMMWWWM
+MMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMM
+MMMMMMMNXKXNWMMMMMMMMMMMWNKOKWMMMMMMMMMM
+MMMMMMWKdccxXMMMMMMMMMMW0o'.oXMMMMMMMMMM
+MMMMMMMNO:.'o0NKkkkkkOXXo. .lXMMMMMMMMMM
+MMMMMMMMNx,..;o;.    .:o,..;kNMMMMMMMMMM
+MMMMMMMMMNO:     ...     .cKWMMMMMMMMMMM
+MMMMMMMMMMNx,. .;dk:.   .;kNMMMMMMMMMMMM
+MMMMMMMMMMMN0ocxXWNkl:,:xXWMMMMMMMMMMMMM
+MMMMMMMMMMMMMWNWMMMWWNNNWMMMMMMMMMMMMMMM
+MMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMM
+EOF
+        ;;
+
         "Finnix"*)
             set_colors 4 7 7
             read -rd '' ascii_data <<'EOF'
 ${c1}            ,,:;;;;:,,
         ,;*%S########S%*;,
       ;?#################S?:
     :%######################?:
@@ -10931,14 +11059,38 @@
 ${c1}           ▟██████▙       ${c2}▜███▙
 ${c1}          ▟███▛▜███▙       ${c2}▜███▙
 ${c1}         ▟███▛  ▜███▙       ${c2}▜███▙
 ${c1}         ▝▀▀▀    ▀▀▀▀▘       ${c2}▀▀▀▘
 EOF
         ;;
 
+        "Nobara"*)
+            set_colors "#999999" "#d80a0a" "#e5b90b"
+
+            read -rd '' ascii_data <<'EOF'
+${c1}      ⢀⣤⣴⣶⣶⣶⣦⣤⡀⠀⣀⣠⣤⣴⣶⣶⣶⣶⣶⣶⣶⣶⣤⣤⣀⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
+    ⠀⣰⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣶⣤⡀⠀⠀⠀⠀⠀⠀⠀⠀
+    ⠀⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣷⣄⠀⠀⠀⠀⠀⠀
+    ⠀⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣷⣄⠀⠀⠀⠀
+    ⠀⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣧⠀⠀⠀
+    ⠀⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⠟⠋⠉⠁⠀⠀⠉⠉⠛⠿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣧⠀⠀
+    ⠀⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⠟⠁⠀⠀⠀${c3}⢀⣀⣀⡀${c1}⠀⠀⠀⠈⢻⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⡇⠀
+    ⠀⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⡏⠀⠀⠀${c3}⢠⣾⣿⣿⣿⣿⣷⡄${c1}⠀⠀⠀⠻⠿⢿⣿⣿⣿⣿⣿⣿⣿⣿⣿⠀
+    ⠀⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⠁⠀⠀⠀${c3}⣿⣿⣿⣿⣿⣿⣿⡇${c1}⠀⠀⠀⠀⠀⣀⣀⣬⣽⣿⣿⣿⣿⣿⣿⠀
+    ⠀⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⠀⠀⠀⠀${c3}⠈⠻⢿⣿⣿⡿⠟⠁${c1}⠀⠀⠀⢸⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⠀
+    ⠀⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⠀
+    ${c2} ⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣷⣤⣤⣄⣀⡀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⠀
+    ${c2} ⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣷⣄⠀⠀⠀⠀⠀⠀⢸⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⠀
+    ${c2} ⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣇⠀⠀⠀⠀⠀⢸⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⠀
+    ${c2} ⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⡿⠟⠛⠉⠉⠛⠛⢿⣿⣿⠀⠀⠀⠀⠀⠸⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⡿⠀
+    ${c2} ⠘⢿⣿⣿⣿⣿⣿⣿⣿⡿⠋⠀⠀⠀⠀⠀⠀⠀⠀⠈⢿⠀⠀⠀⠀⠀⠀⠙⢿⣿⣿⣿⣿⣿⣿⣿⠟⠁⠀
+      ${c2} ⠈⠙⠛⠛⠛⠋⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠉⠛⠛⠛⠛⠉⠁
+EOF
+        ;;
+
         "NomadBSD"*)
             set_colors 4
             read -rd '' ascii_data <<'EOF'
 ${c1}         _======__
      (===============\\
    (===================\\
    _              _---__
@@ -12407,14 +12559,46 @@
     RO   AROSAROS   AROSAROSAR   RO
      AROS   AROSAROSAROSARO   AROS
         ROSA               SARO
            ROSAROSAROSAROSAR
 EOF
         ;;
 
+        "Astra Linux"*)
+            if [[ $ascii_distro == *"ALCE"* ]]; then
+                set_colors 160 231
+            else
+                set_colors 32 231
+            fi
+            read -rd '' ascii_data <<'EOF'
+${c1}                   AA
+${c1}                  AaaA
+${c1}                 Aa${c2}/\\${c1}aA
+${c1}                Aa${c2}/${c1}aa${c2}\\${c1}aA
+${c1}               Aa${c2}/${c1}aAAa${c2}\\${c1}aA
+${c1}              aA${c2}/${c1}aaAAaa${c2}\\${c1}Aa
+${c1}             aA${c2}/${c1}aaAAAAaa${c2}\\${c1}Aa
+${c1}   aaaaaaAAAAa${c2}/${c1}aaAAAAAAaa${c2}\\${c1}aAAAAaaaaa
+${c1} aAAa${c2}-----${c1}aaaaaAAAAAAAAAAaaaaa${c2}-----${c1}aAAa
+${c1}   aAA${c2}\ ${c1}aAAAAAAAAAAAAAAAAAAAAAAa${c2} /${c1}AAa
+${c1}     aAa${c2}\\${c1}aAAA${c2}\\${c1}AAAA${c2}\\${c1}AAAA${c2}\\${c1}AAA${c2}\\${c1}AAa${c2}/${c1}aAa
+${c1}       aAa${c2}\\${c1}aA${c2}\\\\${c1}AAA${c2}\\\\${c1}AAA${c2}\\\\${c1}AA${c2}\\\\/${c1}aAa
+${c1}        aAA${c2}\\${c1}aA${c2}\\\\${c1}AAA${c2}\\\\${c1}AAA${c2}\\\\${c1}Aa${c2}/${c1}AAa
+${c1}          aA${c2}\\${c1}aA${c2}\\\\${c1}AAA${c2}\\\\${c1}AAA${c2}\\\\/${c1}Aa
+${c1}          aA${c2}/${c1}AA${c2}\\\\\\${c1}AA${c2}\\\\\\${c1}AA${c2}\\\\\\${c1}Aa
+${c1}         aA${c2}/\\${c1}AAa${c2}\\\\\\${c1}Aa${c2}\\\\\\${c1}Aa${c2}\\\\\\${c1}Aa
+${c1}         aA${c2}/\\\\${c1}AAa${c2}\\\\/\\${c1}a${c2}\\\\\\${c1}Aa${c2}\\\\${c1}Aa
+${c1}        aA${c2}/${c1}a${c2}\\\\\\${c1}Aa${c2}\\/${c1}AA${c2}\\\\\\\\\\${c1}Aa${c2}\\\\${c1}Aa
+${c1}        aA${c2}/${c1}aA${c2}\\\\/${c1}aAa  aAa${c2}\\\\\\${c1}Aa${c2}\\${c1}Aa
+${c1}       aA${c2}/\\${c1}A${c2}\\/${c1}Aa        aA${c2}\\\\${c1}A${c2}\\\\${c1}Aa
+${c1}       A${c2}|/${c1}aaAa            aAaa${c2}\\|${c1}A
+${c1}      aAaa                    aaAa
+EOF
+        ;;
+
         "sabotage"*)
             set_colors 4 7 1
             read -rd '' ascii_data <<'EOF'
 ${c2} .|'''.|      |     '||''|.    ..|''||
  ||..  '     |||     ||   ||  .|'    ||
   ''|||.    |  ||    ||'''|.  ||      ||
 .     '||  .''''|.   ||    || '|.     ||
```

### Comparing `HyFetch-1.4.8/hyfetch/serializer.py` & `HyFetch-1.4.9/hyfetch/serializer.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/hyfetch/termenv.py` & `HyFetch-1.4.9/hyfetch/termenv.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/setup.py` & `HyFetch-1.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/tools/accept_upstream.py` & `HyFetch-1.4.9/tools/accept_upstream.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python3
 import argparse
+import json
 import os
 import shlex
 from subprocess import check_output
 
 import pyperclip
 import requests
 from github import Github
@@ -48,15 +49,15 @@
 
     # Fetch original pr's information
     info = http.get(f'https://api.github.com/repos/{upstream}/pulls/{pr}').json()
     user = info['user']['login']
 
     # Fetch commit information
     commits = http.get(f'https://api.github.com/repos/{upstream}/pulls/{pr}/commits').json()
-    author = commits[0]['commit']['author']
+    author = json.loads(os.environ.get("override_author")) or commits[-1]['commit']['author']
 
     # Create commit message
     title = info["title"].replace('"', '\\"')
     msg = (f'-m "[PR] {upstream}#{pr} from {user} - {title}" '
            f'-m "Upstream PR: https://github.com/{upstream}/pull/{pr}  \n'
            f'Thanks to @{user}\n\n'
            f'Co-authored-by: {author["name"]} <{author["email"]}>"')
```

### Comparing `HyFetch-1.4.8/tools/colors_test.py` & `HyFetch-1.4.9/tools/colors_test.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/tools/deploy-release.py` & `HyFetch-1.4.9/tools/deploy-release.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/tools/issue_fixed.py` & `HyFetch-1.4.9/tools/issue_fixed.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/tools/list_distros.py` & `HyFetch-1.4.9/tools/list_distros.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import regex
 from hypy_utils import write
 
 from hyfetch.distros import AsciiArt
 
 RE_SPLIT = regex.compile('EOF[ \n]*?;;')
-RE_COLORS = regex.compile("""(?<=set_colors )[a-z\\d ]+(?=\n)""")
+RE_COLORS = regex.compile("""(?<=set_colors )[\"#a-z\\d ]+(?=\n)""")
 
 
 def substr(s: str, start: str, end: str | None = None):
     """
     Get substring between start and end
     """
     start = s.index(start) + len(start)
```

### Comparing `HyFetch-1.4.8/tools/list_unresolved.py` & `HyFetch-1.4.9/tools/list_unresolved.py`

 * *Files identical despite different names*

### Comparing `HyFetch-1.4.8/tools/reformat_readme.py` & `HyFetch-1.4.9/tools/reformat_readme.py`

 * *Files identical despite different names*

