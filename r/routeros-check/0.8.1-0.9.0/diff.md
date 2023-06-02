# Comparing `tmp/routeros-check-0.8.1.tar.gz` & `tmp/routeros-check-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routeros-check-0.8.1.tar", last modified: Wed Mar 29 21:15:42 2023, max compression
+gzip compressed data, was "routeros-check-0.9.0.tar", last modified: Fri Jun  2 11:14:55 2023, max compression
```

## Comparing `routeros-check-0.8.1.tar` & `routeros-check-0.9.0.tar`

### file list

```diff
@@ -1,73 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 21:15:42.369092 routeros-check-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-29 21:15:24.000000 routeros-check-0.8.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 21:15:42.361092 routeros-check-0.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 21:15:42.361092 routeros-check-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-03-29 21:15:24.000000 routeros-check-0.8.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-03-29 21:15:24.000000 routeros-check-0.8.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-03-29 21:15:24.000000 routeros-check-0.8.1/.github/workflows/icinga.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-03-29 21:15:24.000000 routeros-check-0.8.1/.github/workflows/pages.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-03-29 21:15:24.000000 routeros-check-0.8.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-03-29 21:15:24.000000 routeros-check-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-03-29 21:15:24.000000 routeros-check-0.8.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-03-29 21:15:24.000000 routeros-check-0.8.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-29 21:15:24.000000 routeros-check-0.8.1/CHANGELOG.md.license
--rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-03-29 21:15:24.000000 routeros-check-0.8.1/LICENSE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 21:15:42.361092 routeros-check-0.8.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-03-29 21:15:24.000000 routeros-check-0.8.1/LICENSES/CC0-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    34670 2023-03-29 21:15:24.000000 routeros-check-0.8.1/LICENSES/GPL-3.0-or-later.txt
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-03-29 21:15:24.000000 routeros-check-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    46952 2023-03-29 21:15:42.369092 routeros-check-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-03-29 21:15:24.000000 routeros-check-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-29 21:15:24.000000 routeros-check-0.8.1/README.md.license
--rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-03-29 21:15:24.000000 routeros-check-0.8.1/check_routeros.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 21:15:42.361092 routeros-check-0.8.1/config/
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-03-29 21:15:24.000000 routeros-check-0.8.1/config/check_routeros.icinga2.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 21:15:42.365092 routeros-check-0.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-03-29 21:15:24.000000 routeros-check-0.8.1/docs/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-29 21:15:24.000000 routeros-check-0.8.1/docs/cli.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-29 21:15:24.000000 routeros-check-0.8.1/docs/cli.md.license
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-03-29 21:15:24.000000 routeros-check-0.8.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-29 21:15:24.000000 routeros-check-0.8.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-03-29 21:15:24.000000 routeros-check-0.8.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-03-29 21:15:24.000000 routeros-check-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-29 21:15:24.000000 routeros-check-0.8.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 21:15:42.365092 routeros-check-0.8.1/routeros_check/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-29 21:15:24.000000 routeros-check-0.8.1/routeros_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-29 21:15:24.000000 routeros-check-0.8.1/routeros_check/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-29 21:15:42.000000 routeros-check-0.8.1/routeros_check/_scm_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 21:15:42.365092 routeros-check-0.8.1/routeros_check/check/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-29 21:15:24.000000 routeros-check-0.8.1/routeros_check/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-03-29 21:15:24.000000 routeros-check-0.8.1/routeros_check/check/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-03-29 21:15:24.000000 routeros-check-0.8.1/routeros_check/check/interface_gre.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-03-29 21:15:24.000000 routeros-check-0.8.1/routeros_check/check/interface_vrrp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-03-29 21:15:24.000000 routeros-check-0.8.1/routeros_check/check/routing_bgp_peer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-03-29 21:15:24.000000 routeros-check-0.8.1/routeros_check/check/routing_ospf_neighbor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-03-29 21:15:24.000000 routeros-check-0.8.1/routeros_check/check/system_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-03-29 21:15:24.000000 routeros-check-0.8.1/routeros_check/check/system_fan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-03-29 21:15:24.000000 routeros-check-0.8.1/routeros_check/check/system_license.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-03-29 21:15:24.000000 routeros-check-0.8.1/routeros_check/check/system_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-03-29 21:15:24.000000 routeros-check-0.8.1/routeros_check/check/system_power.py
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-03-29 21:15:24.000000 routeros-check-0.8.1/routeros_check/check/system_psu.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-03-29 21:15:24.000000 routeros-check-0.8.1/routeros_check/check/system_temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-03-29 21:15:24.000000 routeros-check-0.8.1/routeros_check/check/system_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-03-29 21:15:24.000000 routeros-check-0.8.1/routeros_check/check/system_uptime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-03-29 21:15:24.000000 routeros-check-0.8.1/routeros_check/check/tool_ping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-03-29 21:15:24.000000 routeros-check-0.8.1/routeros_check/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-03-29 21:15:24.000000 routeros-check-0.8.1/routeros_check/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-29 21:15:24.000000 routeros-check-0.8.1/routeros_check/exeption.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-03-29 21:15:24.000000 routeros-check-0.8.1/routeros_check/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    15137 2023-03-29 21:15:24.000000 routeros-check-0.8.1/routeros_check/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 21:15:42.365092 routeros-check-0.8.1/routeros_check.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    46952 2023-03-29 21:15:42.000000 routeros-check-0.8.1/routeros_check.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-03-29 21:15:42.000000 routeros-check-0.8.1/routeros_check.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 21:15:42.000000 routeros-check-0.8.1/routeros_check.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-29 21:15:42.000000 routeros-check-0.8.1/routeros_check.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-29 21:15:42.000000 routeros-check-0.8.1/routeros_check.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-29 21:15:42.000000 routeros-check-0.8.1/routeros_check.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 21:15:42.369092 routeros-check-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-29 21:15:24.000000 routeros-check-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 21:15:42.365092 routeros-check-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 21:15:24.000000 routeros-check-0.8.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-03-29 21:15:24.000000 routeros-check-0.8.1/tests/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-03-29 21:15:24.000000 routeros-check-0.8.1/tests/helpers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-29 21:15:24.000000 routeros-check-0.8.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:14:55.012930 routeros-check-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-02 11:14:36.000000 routeros-check-0.9.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:14:55.000930 routeros-check-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:14:55.004930 routeros-check-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-02 11:14:36.000000 routeros-check-0.9.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-02 11:14:36.000000 routeros-check-0.9.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-02 11:14:36.000000 routeros-check-0.9.0/.github/workflows/icinga.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-02 11:14:36.000000 routeros-check-0.9.0/.github/workflows/pages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-02 11:14:36.000000 routeros-check-0.9.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-02 11:14:36.000000 routeros-check-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-02 11:14:36.000000 routeros-check-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-02 11:14:36.000000 routeros-check-0.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-02 11:14:36.000000 routeros-check-0.9.0/CHANGELOG.md.license
+-rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-06-02 11:14:36.000000 routeros-check-0.9.0/LICENSE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:14:55.004930 routeros-check-0.9.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-06-02 11:14:36.000000 routeros-check-0.9.0/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    34670 2023-06-02 11:14:36.000000 routeros-check-0.9.0/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-02 11:14:36.000000 routeros-check-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    47174 2023-06-02 11:14:55.012930 routeros-check-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-06-02 11:14:36.000000 routeros-check-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-02 11:14:36.000000 routeros-check-0.9.0/README.md.license
+-rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-06-02 11:14:36.000000 routeros-check-0.9.0/check_routeros.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:14:55.004930 routeros-check-0.9.0/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-06-02 11:14:36.000000 routeros-check-0.9.0/config/check_routeros.icinga2.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:14:55.004930 routeros-check-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-06-02 11:14:36.000000 routeros-check-0.9.0/docs/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-02 11:14:36.000000 routeros-check-0.9.0/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-02 11:14:36.000000 routeros-check-0.9.0/docs/cli.md.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-06-02 11:14:36.000000 routeros-check-0.9.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-02 11:14:36.000000 routeros-check-0.9.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-02 11:14:36.000000 routeros-check-0.9.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-02 11:14:36.000000 routeros-check-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-02 11:14:36.000000 routeros-check-0.9.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:14:55.008930 routeros-check-0.9.0/routeros_check/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-02 11:14:54.000000 routeros-check-0.9.0/routeros_check/_scm_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:14:55.012930 routeros-check-0.9.0/routeros_check/check/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/interface_gre.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/interface_vrrp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/routing_bgp_peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/routing_ospf_neighbor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/system_clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/system_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/system_fan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/system_license.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/system_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9545 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/system_ntp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/system_power.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/system_psu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/system_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/system_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/system_uptime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/tool_ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/exeption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:14:55.008930 routeros-check-0.9.0/routeros_check.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    47174 2023-06-02 11:14:54.000000 routeros-check-0.9.0/routeros_check.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-02 11:14:55.000000 routeros-check-0.9.0/routeros_check.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 11:14:54.000000 routeros-check-0.9.0/routeros_check.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-02 11:14:54.000000 routeros-check-0.9.0/routeros_check.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-02 11:14:54.000000 routeros-check-0.9.0/routeros_check.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-02 11:14:54.000000 routeros-check-0.9.0/routeros_check.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 11:14:55.012930 routeros-check-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-02 11:14:36.000000 routeros-check-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:14:55.012930 routeros-check-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:14:36.000000 routeros-check-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-02 11:14:36.000000 routeros-check-0.9.0/tests/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-06-02 11:14:36.000000 routeros-check-0.9.0/tests/helpers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-02 11:14:36.000000 routeros-check-0.9.0/tox.ini
```

### Comparing `routeros-check-0.8.1/.github/workflows/ci.yml` & `routeros-check-0.9.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `routeros-check-0.8.1/.github/workflows/docs.yml` & `routeros-check-0.9.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `routeros-check-0.8.1/.github/workflows/icinga.yml` & `routeros-check-0.9.0/.github/workflows/icinga.yml`

 * *Files identical despite different names*

### Comparing `routeros-check-0.8.1/.github/workflows/pages.yml` & `routeros-check-0.9.0/.github/workflows/pages.yml`

 * *Files identical despite different names*

### Comparing `routeros-check-0.8.1/.github/workflows/pypi.yml` & `routeros-check-0.9.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `routeros-check-0.8.1/.gitignore` & `routeros-check-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `routeros-check-0.8.1/.pre-commit-config.yaml` & `routeros-check-0.9.0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     hooks:
       - id: flake8
         additional_dependencies:
           - flake8-bugbear
           - flake8-implicit-str-concat
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.1.1
+    rev: v1.3.0
     hooks:
       - id: mypy
         args: [--ignore-missing-imports]
         exclude: ^(docs/|setup.py)
 
   # Check for missing licensing and copyright information.
   # The REUSE helper tool assists with achieving and confirming REUSE compliance.
```

### Comparing `routeros-check-0.8.1/CHANGELOG.md` & `routeros-check-0.9.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Changelog
 =========
 
+0.9.0 - 2023-06-02
+------------------
+
+- Add checks
+  - system.clock
+  - system.ntp.client
+- Update checks to support RouterOS 7.x
+  - routing.ospf.neighbor
+
 0.8.1 - 2023-03-29
 ------------------
 
 - Fix issues introduced in 0.8.0
   - routing.bgp.peer
   - routing.ospf.neighbor
```

### Comparing `routeros-check-0.8.1/LICENSE.md` & `routeros-check-0.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `routeros-check-0.8.1/LICENSES/CC0-1.0.txt` & `routeros-check-0.9.0/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `routeros-check-0.8.1/LICENSES/GPL-3.0-or-later.txt` & `routeros-check-0.9.0/LICENSES/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `routeros-check-0.8.1/PKG-INFO` & `routeros-check-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routeros-check
-Version: 0.8.1
+Version: 0.9.0
 Summary: Monitoring plugin for MikroTik devices for Icinga-Nagios-... 
 Author: DinoTools
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
@@ -798,17 +798,19 @@
 | Subcommand             | Permissions | RouterOS | Description                                              |
 |------------------------|-------------|----------|----------------------------------------------------------|
 | interface              | -           | 6, 7     | Check interfaces                                         |
 | interface.gre          | -           | 6        | Check GRE interfaces/tunnels                             |
 | interface.vrrp         | -           | 6        | Check the state of an VRRP interface                     |
 | routing.bgp.peers      | -           | 6        | Check if connection to BGP peers is established          |
 | routing.ospf.neighbors | -           | 6        | Check if ospf neigbhors are reachable                    |
+| system.clock           | -           | 6, 7     | Check the time from RouterOS against local time          |
 | system.cpu             | -           | 6, 7     | Check the cpu load                                       |
 | system.fan             | -           | 6, 7     | Check the fans                                           |
 | system.memory          | -           | 6, 7     | Check system memory                                      |
+| system.ntp.client      | -           | 6, 7     | Check the ntp client, offset and stratum                 |
 | system.license         | -           | 6, 7     | Check the license level and deadline and renewal date    |
 | system.power           | -           | 6, 7     | Check the overall power consumption if available         |
 | system.psu             | -           | 6, 7     | Check the current, voltage and state of the power supply |
 | system.temperature     | -           | 6, 7     | Check the cpu, system, board and more temperatures.      |
 | system.update          | -           | 6, 7     | Check for updates                                        |
 | system.uptime          | -           | 6, 7     | Check the uptime                                         |
 | tool.ping              | test        | 6, 7     | Run the ping command on the device                       |
```

### Comparing `routeros-check-0.8.1/README.md` & `routeros-check-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -107,17 +107,19 @@
 | Subcommand             | Permissions | RouterOS | Description                                              |
 |------------------------|-------------|----------|----------------------------------------------------------|
 | interface              | -           | 6, 7     | Check interfaces                                         |
 | interface.gre          | -           | 6        | Check GRE interfaces/tunnels                             |
 | interface.vrrp         | -           | 6        | Check the state of an VRRP interface                     |
 | routing.bgp.peers      | -           | 6        | Check if connection to BGP peers is established          |
 | routing.ospf.neighbors | -           | 6        | Check if ospf neigbhors are reachable                    |
+| system.clock           | -           | 6, 7     | Check the time from RouterOS against local time          |
 | system.cpu             | -           | 6, 7     | Check the cpu load                                       |
 | system.fan             | -           | 6, 7     | Check the fans                                           |
 | system.memory          | -           | 6, 7     | Check system memory                                      |
+| system.ntp.client      | -           | 6, 7     | Check the ntp client, offset and stratum                 |
 | system.license         | -           | 6, 7     | Check the license level and deadline and renewal date    |
 | system.power           | -           | 6, 7     | Check the overall power consumption if available         |
 | system.psu             | -           | 6, 7     | Check the current, voltage and state of the power supply |
 | system.temperature     | -           | 6, 7     | Check the cpu, system, board and more temperatures.      |
 | system.update          | -           | 6, 7     | Check for updates                                        |
 | system.uptime          | -           | 6, 7     | Check the uptime                                         |
 | tool.ping              | test        | 6, 7     | Run the ping command on the device                       |
```

#### html2text {}

```diff
@@ -29,22 +29,24 @@
 documented in the table are additional permissions. | Subcommand | Permissions
 | RouterOS | Description | |------------------------|-------------|----------|-
 ---------------------------------------------------------| | interface | - | 6,
 7 | Check interfaces | | interface.gre | - | 6 | Check GRE interfaces/tunnels |
 | interface.vrrp | - | 6 | Check the state of an VRRP interface | |
 routing.bgp.peers | - | 6 | Check if connection to BGP peers is established | |
 routing.ospf.neighbors | - | 6 | Check if ospf neigbhors are reachable | |
+system.clock | - | 6, 7 | Check the time from RouterOS against local time | |
 system.cpu | - | 6, 7 | Check the cpu load | | system.fan | - | 6, 7 | Check
-the fans | | system.memory | - | 6, 7 | Check system memory | | system.license
-| - | 6, 7 | Check the license level and deadline and renewal date | |
-system.power | - | 6, 7 | Check the overall power consumption if available | |
-system.psu | - | 6, 7 | Check the current, voltage and state of the power
-supply | | system.temperature | - | 6, 7 | Check the cpu, system, board and
-more temperatures. | | system.update | - | 6, 7 | Check for updates | |
-system.uptime | - | 6, 7 | Check the uptime | | tool.ping | test | 6, 7 | Run
+the fans | | system.memory | - | 6, 7 | Check system memory | |
+system.ntp.client | - | 6, 7 | Check the ntp client, offset and stratum | |
+system.license | - | 6, 7 | Check the license level and deadline and renewal
+date | | system.power | - | 6, 7 | Check the overall power consumption if
+available | | system.psu | - | 6, 7 | Check the current, voltage and state of
+the power supply | | system.temperature | - | 6, 7 | Check the cpu, system,
+board and more temperatures. | | system.update | - | 6, 7 | Check for updates |
+| system.uptime | - | 6, 7 | Check the uptime | | tool.ping | test | 6, 7 | Run
 the ping command on the device | To get more information about the available
 subcommands/checks have a look at the [check_routeros Command Reference](https:
 //dinotools.github.io/monitoring-check_routeros/cli/) Resources --------- -
 Git-Repository: https://github.com/DinoTools/monitoring-check_routeros -
 Issues: https://github.com/DinoTools/monitoring-check_routeros/issues -
 Documentation: https://dinotools.github.io/monitoring-check_routeros License --
 ----- GPLv3+
```

### Comparing `routeros-check-0.8.1/config/check_routeros.icinga2.conf` & `routeros-check-0.9.0/config/check_routeros.icinga2.conf`

 * *Files identical despite different names*

### Comparing `routeros-check-0.8.1/docs/LICENSE.md` & `routeros-check-0.9.0/docs/LICENSE.md`

 * *Files identical despite different names*

### Comparing `routeros-check-0.8.1/docs/index.md` & `routeros-check-0.9.0/docs/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -107,17 +107,19 @@
 | Subcommand             | Permissions | RouterOS | Description                                              |
 |------------------------|-------------|----------|----------------------------------------------------------|
 | interface              | -           | 6, 7     | Check interfaces                                         |
 | interface.gre          | -           | 6        | Check GRE interfaces/tunnels                             |
 | interface.vrrp         | -           | 6        | Check the state of an VRRP interface                     |
 | routing.bgp.peers      | -           | 6        | Check if connection to BGP peers is established          |
 | routing.ospf.neighbors | -           | 6        | Check if ospf neigbhors are reachable                    |
+| system.clock           | -           | 6, 7     | Check the time from RouterOS against local time          |
 | system.cpu             | -           | 6, 7     | Check the cpu load                                       |
 | system.fan             | -           | 6, 7     | Check the fans                                           |
 | system.memory          | -           | 6, 7     | Check system memory                                      |
+| system.ntp.client      | -           | 6, 7     | Check the ntp client, offset and stratum                 |
 | system.license         | -           | 6, 7     | Check the license level and deadline and renewal date    |
 | system.power           | -           | 6, 7     | Check the overall power consumption if available         |
 | system.psu             | -           | 6, 7     | Check the current, voltage and state of the power supply |
 | system.temperature     | -           | 6, 7     | Check the cpu, system, board and more temperatures.      |
 | system.update          | -           | 6, 7     | Check for updates                                        |
 | system.uptime          | -           | 6, 7     | Check the uptime                                         |
 | tool.ping              | test        | 6, 7     | Run the ping command on the device                       |
```

#### html2text {}

```diff
@@ -29,22 +29,24 @@
 documented in the table are additional permissions. | Subcommand | Permissions
 | RouterOS | Description | |------------------------|-------------|----------|-
 ---------------------------------------------------------| | interface | - | 6,
 7 | Check interfaces | | interface.gre | - | 6 | Check GRE interfaces/tunnels |
 | interface.vrrp | - | 6 | Check the state of an VRRP interface | |
 routing.bgp.peers | - | 6 | Check if connection to BGP peers is established | |
 routing.ospf.neighbors | - | 6 | Check if ospf neigbhors are reachable | |
+system.clock | - | 6, 7 | Check the time from RouterOS against local time | |
 system.cpu | - | 6, 7 | Check the cpu load | | system.fan | - | 6, 7 | Check
-the fans | | system.memory | - | 6, 7 | Check system memory | | system.license
-| - | 6, 7 | Check the license level and deadline and renewal date | |
-system.power | - | 6, 7 | Check the overall power consumption if available | |
-system.psu | - | 6, 7 | Check the current, voltage and state of the power
-supply | | system.temperature | - | 6, 7 | Check the cpu, system, board and
-more temperatures. | | system.update | - | 6, 7 | Check for updates | |
-system.uptime | - | 6, 7 | Check the uptime | | tool.ping | test | 6, 7 | Run
+the fans | | system.memory | - | 6, 7 | Check system memory | |
+system.ntp.client | - | 6, 7 | Check the ntp client, offset and stratum | |
+system.license | - | 6, 7 | Check the license level and deadline and renewal
+date | | system.power | - | 6, 7 | Check the overall power consumption if
+available | | system.psu | - | 6, 7 | Check the current, voltage and state of
+the power supply | | system.temperature | - | 6, 7 | Check the cpu, system,
+board and more temperatures. | | system.update | - | 6, 7 | Check for updates |
+| system.uptime | - | 6, 7 | Check the uptime | | tool.ping | test | 6, 7 | Run
 the ping command on the device | To get more information about the available
 subcommands/checks have a look at the [check_routeros Command Reference](https:
 //dinotools.github.io/monitoring-check_routeros/cli/) Resources --------- -
 Git-Repository: https://github.com/DinoTools/monitoring-check_routeros -
 Issues: https://github.com/DinoTools/monitoring-check_routeros/issues -
 Documentation: https://dinotools.github.io/monitoring-check_routeros License --
 ----- GPLv3+
```

### Comparing `routeros-check-0.8.1/mkdocs.yml` & `routeros-check-0.9.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `routeros-check-0.8.1/pyproject.toml` & `routeros-check-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `routeros-check-0.8.1/routeros_check/check/interface.py` & `routeros-check-0.9.0/routeros_check/check/interface.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.8.1/routeros_check/check/interface_gre.py` & `routeros-check-0.9.0/routeros_check/check/interface_gre.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.8.1/routeros_check/check/interface_vrrp.py` & `routeros-check-0.9.0/routeros_check/check/interface_vrrp.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.8.1/routeros_check/check/routing_bgp_peer.py` & `routeros-check-0.9.0/routeros_check/check/routing_bgp_peer.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
         self._routeros_metric_values = [
             {"name": "disabled", "type": bool},
             {"name": "prefix-count", "dst": "prefix_count", "type": int},
             {"name": "state", "type": str},
             {"name": "updates-received", "dst": "updates_received", "type": int},
             {"name": "updates-sent", "dst": "updates_sent", "type": int},
-            {"name": "uptime", "type": self.parse_routeros_time, "min": 0, "uom": "s"},
+            {"name": "uptime", "type": self.parse_routeros_time_duration, "min": 0, "uom": "s"},
         ]
 
     def fetch_data(self) -> Dict[str, Dict]:
         if self._peer_data:
             return self._peer_data
 
         api = self._connect_api()
```

### Comparing `routeros-check-0.8.1/routeros_check/check/routing_ospf_neighbor.py` & `routeros-check-0.9.0/routeros_check/check/routing_ospf_neighbor.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import click
 import librouteros
 import librouteros.query
 import nagiosplugin
 
 from ..cli import cli
 from ..context import BooleanContext
-from ..helper import logger
+from ..helper import logger, RouterOSVersion
 from ..resource import RouterOSCheckResource
 
 
 class RoutingOSPFNeighborResource(RouterOSCheckResource):
     name = "OSPF NEIGHBOR"
 
     def __init__(
@@ -29,44 +29,59 @@
         self.area = area
         self.instance = instance
         self.router_id = router_id
 
         self.state: Optional[str] = None
 
         self._routeros_metric_values = [
-            {"name": "priority", "type": int},
-            {"name": "adjacency", "type": self.parse_routeros_time, "min": 0, "uom": "s"},
+            {"name": "adjacency", "type": self.parse_routeros_time_duration, "min": 0, "uom": "s"},
             {"name": "state", "type": None},
             {"name": "state-changes", "dst": "state_changes", "type": int},
-            {"name": "ls-retransmits", "dst": "ls_retransmits", "type": int},
-            {"name": "ls-requests", "dst": "ls_requests", "type": int},
-            {"name": "db-summaries", "dst": "db_summaries", "type": int},
         ]
+        if self.routeros_version < RouterOSVersion("7"):
+            self._routeros_metric_values += [
+                {"name": "priority", "type": int},
+                {"name": "ls-retransmits", "dst": "ls_retransmits", "type": int},
+                {"name": "ls-requests", "dst": "ls_requests", "type": int},
+                {"name": "db-summaries", "dst": "db_summaries", "type": int},
+            ]
 
     def probe(self):
         # ToDo: Only available in v7.x
-        # key_area = librouteros.query.Key("area")
+        key_area = librouteros.query.Key("area")
         key_instance = librouteros.query.Key("instance")
         key_router_id = librouteros.query.Key("router-id")
 
-        api = self._connect_api()
-
         logger.info("Fetching data ...")
 
-        call = api.path(
-            "/routing/ospf/neighbor"
-        ).select(
+        select_keys = [
             key_instance,
-            # key_area,
             key_router_id,
-            *self.get_routeros_select_keys()
-        ).where(
+        ] + self.get_routeros_select_keys()
+
+        if self.routeros_version >= RouterOSVersion("7"):
+            select_keys.append(key_area)
+
+        where = [
             key_instance == self.instance,
-            # key_area == self._area,
-            key_router_id == self.router_id
+            key_router_id == self.router_id,
+        ]
+
+        if self.area is not None:
+            if self.routeros_version >= RouterOSVersion("7"):
+                where.append(key_area == self.area)
+            else:
+                logger.warning("The area selector is only available on RouterOS 7.x")
+
+        call = self.api.path(
+            "/routing/ospf/neighbor"
+        ).select(
+            *select_keys
+        ).where(
+            *where
         )
         results = tuple(call)
         if len(results) == 0:
             return nagiosplugin.Metric(
                 name="state",
                 value=None
             )
@@ -75,22 +90,29 @@
 
         return self.get_routeros_metric_item(result)
 
 
 class RoutingOSPFNeighborState(BooleanContext):
     def evaluate(self, metric, resource: RoutingOSPFNeighborResource):
         if metric.value is None:
+            if resource.area is None:
+                hint = f"Neighbor for instance '{resource.instance}' and router-id '{resource.router_id}' not found"
+            else:
+                hint = (
+                    f"Neighbor for area '{resource.area}', instance '{resource.instance}' and "
+                    f"router-id '{resource.router_id}' not found"
+                )
             return nagiosplugin.Result(
                 state=nagiosplugin.state.Critical,
-                hint=f"Neighbor for instance '{resource.instance}' and router-id '{resource.router_id}' not found"
+                hint=hint
             )
         elif metric.value in ("Down",):
             return self.result_cls(
                 state=nagiosplugin.state.Critical,
-                hint="Linkt to neighbor down"
+                hint="Link to neighbor down"
             )
         elif metric.value in ("Full",):
             return self.result_cls(
                 state=nagiosplugin.state.Ok,
                 hint="Communicating with neighbor"
             )
         else:
@@ -98,28 +120,33 @@
                 state=nagiosplugin.state.Warn,
                 hint=f"Link to neighbor not fully up, state: {metric.value}"
             )
 
 
 @cli.command("routing.ospf.neighbors")
 @click.option(
+    "--area",
+    help="The area the neighbor router belongs to (only supported on RouterOS v7.x",
+)
+@click.option(
     "--instance",
     required=True,
     help="The name of the OSPF instance",
 )
 @click.option(
     "--router-id",
     required=True,
     help="The ID of the neighbor router",
 )
 @click.pass_context
-def routing_ospf_neighbors(ctx, instance, router_id):
+def routing_ospf_neighbors(ctx, area, instance, router_id):
     """Check the state of an OSPF neighbor"""
     resource = RoutingOSPFNeighborResource(
         cmd_options=ctx.obj,
+        area=area,
         instance=instance,
         router_id=router_id,
     )
     check = nagiosplugin.Check(
         resource,
         nagiosplugin.ScalarContext("priority"),
         nagiosplugin.ScalarContext("adjacency"),
```

### Comparing `routeros-check-0.8.1/routeros_check/check/system_cpu.py` & `routeros-check-0.9.0/routeros_check/check/system_cpu.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.8.1/routeros_check/check/system_fan.py` & `routeros-check-0.9.0/routeros_check/check/system_fan.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.8.1/routeros_check/check/system_license.py` & `routeros-check-0.9.0/routeros_check/check/system_license.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.8.1/routeros_check/check/system_memory.py` & `routeros-check-0.9.0/routeros_check/check/system_memory.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.8.1/routeros_check/check/system_power.py` & `routeros-check-0.9.0/routeros_check/check/system_power.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.8.1/routeros_check/check/system_psu.py` & `routeros-check-0.9.0/routeros_check/check/system_psu.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.8.1/routeros_check/check/system_temperature.py` & `routeros-check-0.9.0/routeros_check/check/system_temperature.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.8.1/routeros_check/check/system_update.py` & `routeros-check-0.9.0/routeros_check/check/system_update.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.8.1/routeros_check/check/system_uptime.py` & `routeros-check-0.9.0/routeros_check/check/system_uptime.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             librouteros.query.Key("uptime"),
         )
         results = tuple(call)
         result = results[0]
 
         yield nagiosplugin.Metric(
             name="uptime",
-            value=self.parse_routeros_time(result["uptime"]),
+            value=self.parse_routeros_time_duration(result["uptime"]),
             uom="s",
             min=0,
         )
 
 
 @cli.command("system.uptime")
 @click.pass_context
```

### Comparing `routeros-check-0.8.1/routeros_check/check/tool_ping.py` & `routeros-check-0.9.0/routeros_check/check/tool_ping.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.8.1/routeros_check/cli.py` & `routeros-check-0.9.0/routeros_check/cli.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.8.1/routeros_check/context.py` & `routeros-check-0.9.0/routeros_check/context.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,61 @@
 # SPDX-FileCopyrightText: PhiBo DinoTools (2021)
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import re
 from typing import Optional, Union
 
 import nagiosplugin
+from nagiosplugin.state import Ok as STATE_Ok, Warn as STATE_Warn, Critical as STATE_Critical
 
 
 class BooleanContext(nagiosplugin.Context):
     def performance(self, metric, resource):
         return nagiosplugin.performance.Performance(
             label=metric.name,
             value=1 if metric.value else 0
         )
 
 
+class PerfdataScalarContext(nagiosplugin.ScalarContext):
+    def evaluate(self, metric, resource):
+        return self.result_cls(STATE_Ok, None, metric)
+
+    def performance(self, metric, resource):
+        return super(PerfdataScalarContext, self).performance(metric, resource)
+
+
+class SimplePositiveFloatContext(nagiosplugin.ScalarContext):
+    def __init__(self, name, warning=None, critical=None, fmt_metric='{name} is {valueunit}',
+                 result_cls=nagiosplugin.Result):
+        super(SimplePositiveFloatContext, self).__init__(name, fmt_metric=fmt_metric, result_cls=result_cls)
+
+        self._warning = warning
+        self._critical = critical
+
+    def evaluate(self, metric, resource):
+        metric_value_abs = abs(metric.value)
+        if self._critical and metric_value_abs > self._critical:
+            return self.result_cls(
+                STATE_Critical,
+                None,
+                metric
+            )
+        if self._warning and metric_value_abs > self._warning:
+            return self.result_cls(
+                STATE_Warn,
+                None,
+                metric
+            )
+        return self.result_cls(STATE_Ok, None, metric)
+
+    def performance(self, metric, resource):
+        return super(SimplePositiveFloatContext, self).performance(metric, resource)
+
+
 class ScalarPercentContext(nagiosplugin.ScalarContext):
     def __init__(self, name, total_name: Optional[str] = None, total_value: Optional[Union[int, float]] = None,
                  warning=None, critical=None, fmt_metric='{name} is {valueunit}', result_cls=nagiosplugin.Result):
         super(ScalarPercentContext, self).__init__(name, fmt_metric=fmt_metric, result_cls=result_cls)
 
         self._warning = warning
         self._critical = critical
```

### Comparing `routeros-check-0.8.1/routeros_check/helper.py` & `routeros-check-0.9.0/routeros_check/helper.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.8.1/routeros_check/resource.py` & `routeros-check-0.9.0/routeros_check/resource.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,54 @@
 # SPDX-FileCopyrightText: PhiBo DinoTools (2021)
 # SPDX-License-Identifier: GPL-3.0-or-later
-from datetime import datetime
+from datetime import date, datetime, time
+from decimal import Decimal
 import re
 import ssl
 from typing import Any, Dict, List, Optional, Union
 
 import librouteros
 import librouteros.query
 import nagiosplugin
 
 from .helper import logger, RouterOSVersion
 from .exeption import MissingValue
 
 
 class RouterOSCheckResource(nagiosplugin.Resource):
+    month_mapping: Dict[str, int] = {
+        "jan": 1,
+        "feb": 2,
+        "mar": 3,
+        "apr": 4,
+        "may": 5,
+        "jun": 6,
+        "jul": 7,
+        "aug": 8,
+        "sep": 9,
+        "oct": 10,
+        "nov": 11,
+        "dec": 12,
+    }
+
     regex_datetime = re.compile(
         r"(?P<month>[a-z]{3})/(?P<day>\d+)/(?P<year>\d{4})\s+(?P<hour>\d+):(?P<minute>\d+):(?P<second>\d+)",
         flags=re.IGNORECASE
     )
 
+    regex_date = re.compile(
+        r"(?P<month>[a-z]{3})/(?P<day>\d+)/(?P<year>\d{4})",
+        flags=re.IGNORECASE
+    )
+
+    regex_time = re.compile(
+        r"(?P<hour>\d+):(?P<minute>\d+):(?P<second>\d+)",
+        flags=re.IGNORECASE
+    )
+
     def __init__(self, cmd_options: Dict[str, Any]):
         self._cmd_options = cmd_options
         self._routeros_metric_values: List[Dict[str, Any]] = []
         self._routeros_version: Optional[RouterOSVersion] = None
         self._api: Optional[librouteros.api.Api] = None
         self.current_time = datetime.now()
 
@@ -112,18 +138,15 @@
             result_items.append({
                 "name": name,
                 "value": value,
             })
         return result_items
 
     def _get_routeros_version(self) -> RouterOSVersion:
-        if self._api is None:
-            raise RuntimeWarning("Not connected to RouterOS device")
-
-        call = self._api.path(
+        call = self.api.path(
             "/system/resource"
         )
         results = tuple(call)
         result: Dict[str, str] = results[0]
         # version: 7.8 (stable)
         version_string = result["version"].partition(" ")[0]
         return RouterOSVersion(version_string)
@@ -131,37 +154,41 @@
     def connect_api(self) -> librouteros.api.Api:
         if self._api is None:
             self._api = self._connect_api()
 
         return self._api
 
     @classmethod
-    def parse_routeros_datetime(cls, datetime_string: str) -> datetime:
-        month_mapping: Dict[str, int] = {
-            "jan": 1,
-            "feb": 2,
-            "mar": 3,
-            "apr": 4,
-            "may": 5,
-            "jun": 6,
-            "jul": 7,
-            "aug": 8,
-            "sep": 9,
-            "oct": 10,
-            "nov": 11,
-            "dec": 12,
-        }
+    def parse_routeros_date(cls, date_string: str) -> date:
+        m = cls.regex_date.match(date_string)
+        if not m:
+            raise ValueError("Unable to parse datetime string")
 
+        return date(
+            year=int(m.group("year")),
+            month=cls.month_mapping[m.group("month").lower()],
+            day=int(m.group("day"))
+        )
+
+    @classmethod
+    def parse_routeros_date_time(cls, date_string: str, time_string: str) -> datetime:
+        parsed_date = cls.parse_routeros_date(date_string=date_string)
+        parsed_time = cls.parse_routeros_time(time_string=time_string)
+
+        return datetime.combine(parsed_date, parsed_time)
+
+    @classmethod
+    def parse_routeros_datetime(cls, datetime_string: str) -> datetime:
         m = cls.regex_datetime.match(datetime_string)
         if not m:
             raise ValueError("Unable to parse datetime string")
 
         return datetime(
             year=int(m.group("year")),
-            month=month_mapping[m.group("month").lower()],
+            month=cls.month_mapping[m.group("month").lower()],
             day=int(m.group("day")),
             hour=int(m.group("hour")),
             minute=int(m.group("minute")),
             second=int(m.group("second"))
         )
 
     @staticmethod
@@ -180,32 +207,52 @@
         factor = factors.get(m.group("factor"))
 
         if factor is None:
             raise ValueError(f"Unable to parse element '{m.group()}' of speed string: '{value_string}'")
 
         return int(m.group("value")) * factor
 
+    @classmethod
+    def parse_routeros_time(cls, time_string: str) -> time:
+        m = cls.regex_time.match(time_string)
+        if not m:
+            raise ValueError("Unable to parse datetime string")
+
+        return time(
+            hour=int(m.group("hour")),
+            minute=int(m.group("minute")),
+            second=int(m.group("second"))
+        )
+
     @staticmethod
-    def parse_routeros_time(time_string: str) -> int:
-        factors = {
+    def parse_routeros_time_duration(time_string: str) -> float:
+        factors: Dict[str, Union[int, Decimal]] = {
+            "us": Decimal(1e-6),
+            "ms": Decimal(0.001),
             "s": 1,
             "m": 60,
             "h": 60 * 60,
             "d": 24 * 60 * 60,
             "w": 7 * 24 * 60 * 60,
         }
 
-        seconds = 0
+        value_is_negativ = time_string.startswith("-")
+
+        seconds = Decimal(0)
         for m in re.compile(r"(?P<value>\d+)(?P<type>[a-z]+)").finditer(time_string):
             factor = factors.get(m.group("type"))
             if factor is None:
                 raise ValueError(f"Unable to parse element '{m.group()}' of time string: '{time_string}'")
             seconds += int(m.group("value")) * factor
 
-        return seconds
+        seconds_float = float(round(seconds, 6))
+
+        if value_is_negativ:
+            return -seconds_float
+        return seconds_float
 
     @staticmethod
     def prepare_override_values(override_values: List[str]) -> Dict[str, str]:
         results: Dict[str, str] = {}
         for override_value in override_values:
             name, _, value = override_value.partition(":")
             if value is None or value == "":
```

### Comparing `routeros-check-0.8.1/routeros_check.egg-info/PKG-INFO` & `routeros-check-0.9.0/routeros_check.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routeros-check
-Version: 0.8.1
+Version: 0.9.0
 Summary: Monitoring plugin for MikroTik devices for Icinga-Nagios-... 
 Author: DinoTools
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
@@ -798,17 +798,19 @@
 | Subcommand             | Permissions | RouterOS | Description                                              |
 |------------------------|-------------|----------|----------------------------------------------------------|
 | interface              | -           | 6, 7     | Check interfaces                                         |
 | interface.gre          | -           | 6        | Check GRE interfaces/tunnels                             |
 | interface.vrrp         | -           | 6        | Check the state of an VRRP interface                     |
 | routing.bgp.peers      | -           | 6        | Check if connection to BGP peers is established          |
 | routing.ospf.neighbors | -           | 6        | Check if ospf neigbhors are reachable                    |
+| system.clock           | -           | 6, 7     | Check the time from RouterOS against local time          |
 | system.cpu             | -           | 6, 7     | Check the cpu load                                       |
 | system.fan             | -           | 6, 7     | Check the fans                                           |
 | system.memory          | -           | 6, 7     | Check system memory                                      |
+| system.ntp.client      | -           | 6, 7     | Check the ntp client, offset and stratum                 |
 | system.license         | -           | 6, 7     | Check the license level and deadline and renewal date    |
 | system.power           | -           | 6, 7     | Check the overall power consumption if available         |
 | system.psu             | -           | 6, 7     | Check the current, voltage and state of the power supply |
 | system.temperature     | -           | 6, 7     | Check the cpu, system, board and more temperatures.      |
 | system.update          | -           | 6, 7     | Check for updates                                        |
 | system.uptime          | -           | 6, 7     | Check the uptime                                         |
 | tool.ping              | test        | 6, 7     | Run the ping command on the device                       |
```

### Comparing `routeros-check-0.8.1/routeros_check.egg-info/SOURCES.txt` & `routeros-check-0.9.0/routeros_check.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -42,18 +42,20 @@
 routeros_check.egg-info/top_level.txt
 routeros_check/check/__init__.py
 routeros_check/check/interface.py
 routeros_check/check/interface_gre.py
 routeros_check/check/interface_vrrp.py
 routeros_check/check/routing_bgp_peer.py
 routeros_check/check/routing_ospf_neighbor.py
+routeros_check/check/system_clock.py
 routeros_check/check/system_cpu.py
 routeros_check/check/system_fan.py
 routeros_check/check/system_license.py
 routeros_check/check/system_memory.py
+routeros_check/check/system_ntp_client.py
 routeros_check/check/system_power.py
 routeros_check/check/system_psu.py
 routeros_check/check/system_temperature.py
 routeros_check/check/system_update.py
 routeros_check/check/system_uptime.py
 routeros_check/check/tool_ping.py
 tests/__init__.py
```

### Comparing `routeros-check-0.8.1/tests/helpers_test.py` & `routeros-check-0.9.0/tests/helpers_test.py`

 * *Files identical despite different names*

