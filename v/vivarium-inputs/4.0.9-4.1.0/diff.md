# Comparing `tmp/vivarium_inputs-4.0.9.tar.gz` & `tmp/vivarium_inputs-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vivarium_inputs-4.0.9.tar", last modified: Mon Nov 28 20:53:03 2022, max compression
+gzip compressed data, was "vivarium_inputs-4.1.0.tar", last modified: Fri Jun  2 00:21:01 2023, max compression
```

## Comparing `vivarium_inputs-4.0.9.tar` & `vivarium_inputs-4.1.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 20:53:03.042199 vivarium_inputs-4.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5164 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)      837 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2022-11-28 20:53:03.042199 vivarium_inputs-4.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      696 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 20:53:03.030198 vivarium_inputs-4.0.9/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      290 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/docs/nitpick-exceptions
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 20:53:03.030198 vivarium_inputs-4.0.9/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 20:53:03.030198 vivarium_inputs-4.0.9/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/docs/source/_static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 20:53:03.034198 vivarium_inputs-4.0.9/docs/source/api_reference/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/docs/source/api_reference/core.rst
--rw-r--r--   0 runner    (1001) docker     (123)      107 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/docs/source/api_reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       63 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/docs/source/api_reference/interface.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/docs/source/api_reference/mapping_extension.rst
--rw-r--r--   0 runner    (1001) docker     (123)       63 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/docs/source/api_reference/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7803 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 20:53:03.034198 vivarium_inputs-4.0.9/docs/source/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/docs/source/tutorials/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15442 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/docs/source/tutorials/pulling_data.rst
--rw-r--r--   0 runner    (1001) docker     (123)      205 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-11-28 20:53:03.042199 vivarium_inputs-4.0.9/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1615 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 20:53:03.026198 vivarium_inputs-4.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 20:53:03.034198 vivarium_inputs-4.0.9/src/vivarium_inputs/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/src/vivarium_inputs/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/src/vivarium_inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19647 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/src/vivarium_inputs/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9540 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/src/vivarium_inputs/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     6983 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/src/vivarium_inputs/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7861 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/src/vivarium_inputs/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 20:53:03.038199 vivarium_inputs-4.0.9/src/vivarium_inputs/mapping_extension/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/src/vivarium_inputs/mapping_extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/src/vivarium_inputs/mapping_extension/alternative_risk_factor.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/src/vivarium_inputs/mapping_extension/alternative_risk_factor_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/src/vivarium_inputs/mapping_extension/health_technology.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/src/vivarium_inputs/mapping_extension/health_technology_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/src/vivarium_inputs/mapping_extension/healthcare_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/src/vivarium_inputs/mapping_extension/healthcare_entity_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 20:53:03.038199 vivarium_inputs-4.0.9/src/vivarium_inputs/testing/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/src/vivarium_inputs/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/src/vivarium_inputs/testing/test_load.py
--rw-r--r--   0 runner    (1001) docker     (123)    18148 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/src/vivarium_inputs/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/src/vivarium_inputs/utility_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 20:53:03.038199 vivarium_inputs-4.0.9/src/vivarium_inputs/validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/src/vivarium_inputs/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    84399 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/src/vivarium_inputs/validation/raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/src/vivarium_inputs/validation/shared.py
--rw-r--r--   0 runner    (1001) docker     (123)    57659 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/src/vivarium_inputs/validation/sim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 20:53:03.038199 vivarium_inputs-4.0.9/src/vivarium_inputs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2022-11-28 20:53:02.000000 vivarium_inputs-4.0.9/src/vivarium_inputs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2022-11-28 20:53:02.000000 vivarium_inputs-4.0.9/src/vivarium_inputs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-28 20:53:02.000000 vivarium_inputs-4.0.9/src/vivarium_inputs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-28 20:53:02.000000 vivarium_inputs-4.0.9/src/vivarium_inputs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      329 2022-11-28 20:53:02.000000 vivarium_inputs-4.0.9/src/vivarium_inputs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-11-28 20:53:02.000000 vivarium_inputs-4.0.9/src/vivarium_inputs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 20:53:03.038199 vivarium_inputs-4.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 20:53:03.042199 vivarium_inputs-4.0.9/tests/extract/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/tests/extract/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     6345 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/tests/extract/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/tests/extract/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/tests/extract/test_get_measure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/tests/extract/test_utility_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/tests/test_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-28 20:53:03.042199 vivarium_inputs-4.0.9/tests/validation/
--rw-r--r--   0 runner    (1001) docker     (123)    15435 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/tests/validation/test_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/tests/validation/test_shared.py
--rw-r--r--   0 runner    (1001) docker     (123)    10484 2022-11-28 20:52:53.000000 vivarium_inputs-4.0.9/tests/validation/test_sim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:21:01.486185 vivarium_inputs-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-02 00:21:01.486185 vivarium_inputs-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:21:01.482185 vivarium_inputs-4.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/docs/nitpick-exceptions
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:21:01.482185 vivarium_inputs-4.1.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:21:01.482185 vivarium_inputs-4.1.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/docs/source/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:21:01.482185 vivarium_inputs-4.1.0/docs/source/api_reference/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/docs/source/api_reference/core.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/docs/source/api_reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/docs/source/api_reference/interface.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/docs/source/api_reference/mapping_extension.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/docs/source/api_reference/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7821 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:21:01.482185 vivarium_inputs-4.1.0/docs/source/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/docs/source/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15442 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/docs/source/tutorials/pulling_data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 00:21:01.486185 vivarium_inputs-4.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1613 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:21:01.482185 vivarium_inputs-4.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:21:01.486185 vivarium_inputs-4.1.0/src/vivarium_inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19647 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6983 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:21:01.486185 vivarium_inputs-4.1.0/src/vivarium_inputs/mapping_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/mapping_extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/mapping_extension/alternative_risk_factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/mapping_extension/alternative_risk_factor_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/mapping_extension/health_technology.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/mapping_extension/health_technology_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/mapping_extension/healthcare_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/mapping_extension/healthcare_entity_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:21:01.486185 vivarium_inputs-4.1.0/src/vivarium_inputs/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/testing/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18148 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/utility_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:21:01.486185 vivarium_inputs-4.1.0/src/vivarium_inputs/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84467 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/validation/raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/validation/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57659 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/validation/sim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:21:01.486185 vivarium_inputs-4.1.0/src/vivarium_inputs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-02 00:21:01.000000 vivarium_inputs-4.1.0/src/vivarium_inputs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-02 00:21:01.000000 vivarium_inputs-4.1.0/src/vivarium_inputs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 00:21:01.000000 vivarium_inputs-4.1.0/src/vivarium_inputs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 00:21:01.000000 vivarium_inputs-4.1.0/src/vivarium_inputs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-02 00:21:01.000000 vivarium_inputs-4.1.0/src/vivarium_inputs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-02 00:21:01.000000 vivarium_inputs-4.1.0/src/vivarium_inputs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:21:01.486185 vivarium_inputs-4.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:21:01.486185 vivarium_inputs-4.1.0/tests/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/tests/extract/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/tests/extract/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/tests/extract/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/tests/extract/test_get_measure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/tests/extract/test_utility_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:21:01.486185 vivarium_inputs-4.1.0/tests/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)    15435 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/tests/validation/test_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/tests/validation/test_shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/tests/validation/test_sim.py
```

### Comparing `vivarium_inputs-4.0.9/CHANGELOG.rst` & `vivarium_inputs-4.1.0/CHANGELOG.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+**4.1.0 - 06/01/23**
+
+ - Update pins
+ - Bugfix PAF validation
+ - Support Python 3.8-3.11
+
+**4.0.10 - 12/27/22**
+
+ - Update CI to build with python 3.8-3.10
+ - Update codeowners
+
 **4.0.9 - 11/28/22**
 
  - Add BMI in adults to list of known risk factors with negative PAFs
 
 **4.0.8 - 07/25/22**
 
  - Remove unneeded column when loading PAFs
```

### Comparing `vivarium_inputs-4.0.9/CODE_OF_CONDUCT.rst` & `vivarium_inputs-4.1.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.0.9/CONTRIBUTING.rst` & `vivarium_inputs-4.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.0.9/LICENSE.txt` & `vivarium_inputs-4.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.0.9/PKG-INFO` & `vivarium_inputs-4.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: vivarium_inputs
-Version: 4.0.9
+Version: 4.1.0
 Summary: Transformations and artifact building for the vivarium microsimulation project.
 Home-page: https://github.com/ihmeuw/vivarium_inputs
 Author: The vivarium developers
 Author-email: vivarium.dev@gmail.com
-License: UNKNOWN
-Description: Vivarium Inputs
-        ===============
-        
-        .. image:: https://badge.fury.io/py/vivarium-inputs.svg
-            :target: https://badge.fury.io/py/vivarium-inputs
-        
-        .. image:: https://travis-ci.org/ihmeuw/vivarium_inputs.svg?branch=master
-            :target: https://travis-ci.org/ihmeuw/vivarium_inputs
-            :alt: Latest Version
-        
-        .. image:: https://readthedocs.org/projects/vivarium_inputs/badge/?version=latest
-            :target: https://vivarium_inputs.readthedocs.io/en/latest/?badge=latest
-            :alt: Latest Docs
-        
-        
-        This package is used to transform Global Burden of Disease data and package it into data artifacts
-        used as inputs into vivarium simulations.
-        
-        It requires access to the IHME cluster for use (but not for testing).
-        
-Platform: UNKNOWN
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: data
 Provides-Extra: dev
+License-File: LICENSE.txt
+License-File: AUTHORS.rst
+
+Vivarium Inputs
+===============
+
+.. image:: https://badge.fury.io/py/vivarium-inputs.svg
+    :target: https://badge.fury.io/py/vivarium-inputs
+
+.. image:: https://travis-ci.org/ihmeuw/vivarium_inputs.svg?branch=master
+    :target: https://travis-ci.org/ihmeuw/vivarium_inputs
+    :alt: Latest Version
+
+.. image:: https://readthedocs.org/projects/vivarium_inputs/badge/?version=latest
+    :target: https://vivarium_inputs.readthedocs.io/en/latest/?badge=latest
+    :alt: Latest Docs
+
+
+This package is used to transform Global Burden of Disease data and package it into data artifacts
+used as inputs into vivarium simulations.
+
+It requires access to the IHME cluster for use (but not for testing).
```

### Comparing `vivarium_inputs-4.0.9/README.rst` & `vivarium_inputs-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.0.9/docs/Makefile` & `vivarium_inputs-4.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.0.9/docs/source/conf.py` & `vivarium_inputs-4.1.0/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,15 @@
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3.8", None),
     "pandas": ("https://pandas.pydata.org/pandas-docs/stable/", None),
     "tables": ("https://www.pytables.org/", None),
     "numpy": ("https://numpy.org/doc/stable/", None),
     "networkx": ("https://networkx.org/documentation/stable/", None),
     "vivarium": ("https://vivarium.readthedocs.io/en/latest/", None),
-    "gbd_mapping": ("https://gbd_mapping.readthedocs.io/en/latest/", None),
+    "gbd_mapping": ("https://vivarium.readthedocs.io/projects/gbd-mapping/en/latest/", None),
 }
 
 
 # -- Autodoc configuration ------------------------------------------------
 
 autodoc_default_options = {
     # Automatically document members (e.g. classes in a module,
```

### Comparing `vivarium_inputs-4.0.9/docs/source/tutorials/pulling_data.rst` & `vivarium_inputs-4.1.0/docs/source/tutorials/pulling_data.rst`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.0.9/setup.py` & `vivarium_inputs-4.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,20 +17,20 @@
     install_requirements = [
         "numpy",
         "scipy",
         "pandas",
         "click",
         "joblib",
         "tables",
-        "vivarium>=0.10.16",
-        "gbd_mapping>=3.0.6, <4.0.0",
+        "vivarium>=1.2.0",
+        "gbd_mapping>=3.1.0, <4.0.0",
         "loguru",
     ]
 
-    data_requires = ["vivarium-gbd-access>=3.0.5, <4.0.0", "core-maths"]
+    data_requires = ["vivarium-gbd-access>=3.0.7, <4.0.0", "core-maths"]
 
     test_requirements = [
         "pytest",
         "pytest-mock",
         "hypothesis",
     ]
```

### Comparing `vivarium_inputs-4.0.9/src/vivarium_inputs/__about__.py` & `vivarium_inputs-4.1.0/src/vivarium_inputs/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,14 @@
 
 __title__ = "vivarium_inputs"
 __summary__ = (
     "Transformations and artifact building for the vivarium microsimulation project."
 )
 __uri__ = "https://github.com/ihmeuw/vivarium_inputs"
 
-__version__ = "4.0.9"
+__version__ = "4.1.0"
 
 __author__ = "The vivarium developers"
 __email__ = "vivarium.dev@gmail.com"
 
 __license__ = "BSD-3-Clause"
 __copyright__ = f"Copyright 2022 {__author__}"
```

### Comparing `vivarium_inputs-4.0.9/src/vivarium_inputs/core.py` & `vivarium_inputs-4.1.0/src/vivarium_inputs/core.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.0.9/src/vivarium_inputs/extract.py` & `vivarium_inputs-4.1.0/src/vivarium_inputs/extract.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.0.9/src/vivarium_inputs/globals.py` & `vivarium_inputs-4.1.0/src/vivarium_inputs/globals.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.0.9/src/vivarium_inputs/interface.py` & `vivarium_inputs-4.1.0/src/vivarium_inputs/interface.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.0.9/src/vivarium_inputs/mapping_extension/alternative_risk_factor.py` & `vivarium_inputs-4.1.0/src/vivarium_inputs/mapping_extension/alternative_risk_factor.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.0.9/src/vivarium_inputs/mapping_extension/alternative_risk_factor_template.py` & `vivarium_inputs-4.1.0/src/vivarium_inputs/mapping_extension/alternative_risk_factor_template.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.0.9/src/vivarium_inputs/mapping_extension/healthcare_entity_template.py` & `vivarium_inputs-4.1.0/src/vivarium_inputs/mapping_extension/healthcare_entity_template.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.0.9/src/vivarium_inputs/utilities.py` & `vivarium_inputs-4.1.0/src/vivarium_inputs/utilities.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.0.9/src/vivarium_inputs/utility_data.py` & `vivarium_inputs-4.1.0/src/vivarium_inputs/utility_data.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.0.9/src/vivarium_inputs/validation/raw.py` & `vivarium_inputs-4.1.0/src/vivarium_inputs/validation/raw.py`

 * *Files 0% similar despite different names*

```diff
@@ -1150,29 +1150,29 @@
     check_measure_id(data, ["YLLs", "YLDs"], single_only=False)
     check_metric_id(data, "percent")
 
     check_years(data, context, "annual")
     check_location(data, context)
 
     restrictions = entity.restrictions
-    male_expected = not restrictions.female_only
-    female_expected = not restrictions.male_only
+    risk_male_expected = not restrictions.female_only
+    risk_female_expected = not restrictions.male_only
 
     grouped = data.groupby(["cause_id", "measure_id"])
 
     for (c_id, _), g in grouped:
         cause = [c for c in causes if c.gbd_id == c_id][0]
-        male_expected = male_expected and not cause.restrictions.female_only
-        female_expected = female_expected and not cause.restrictions.male_only
+        cause_male_expected = risk_male_expected and not cause.restrictions.female_only
+        cause_female_expected = risk_female_expected and not cause.restrictions.male_only
 
         check_age_group_ids(g, context, None, None)
-        check_sex_ids(g, context, male_expected, female_expected)
+        check_sex_ids(g, context, cause_male_expected, cause_female_expected)
         #  check only if there is a sex restriction (male only or female only).
-        if not male_expected or not female_expected:
-            check_sex_restrictions(g, context, male_expected, female_expected)
+        if not cause_male_expected or not cause_female_expected:
+            check_sex_restrictions(g, context, cause_male_expected, cause_female_expected)
         check_paf_rr_exposure_age_groups(g, context, entity)
 
     protective_causes = (
         PROTECTIVE_CAUSE_RISK_PAIRS[entity.name]
         if entity.name in PROTECTIVE_CAUSE_RISK_PAIRS
         else []
     )
```

### Comparing `vivarium_inputs-4.0.9/src/vivarium_inputs/validation/shared.py` & `vivarium_inputs-4.1.0/src/vivarium_inputs/validation/shared.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.0.9/src/vivarium_inputs/validation/sim.py` & `vivarium_inputs-4.1.0/src/vivarium_inputs/validation/sim.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.0.9/src/vivarium_inputs.egg-info/PKG-INFO` & `vivarium_inputs-4.1.0/src/vivarium_inputs.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: vivarium-inputs
-Version: 4.0.9
+Version: 4.1.0
 Summary: Transformations and artifact building for the vivarium microsimulation project.
 Home-page: https://github.com/ihmeuw/vivarium_inputs
 Author: The vivarium developers
 Author-email: vivarium.dev@gmail.com
-License: UNKNOWN
-Description: Vivarium Inputs
-        ===============
-        
-        .. image:: https://badge.fury.io/py/vivarium-inputs.svg
-            :target: https://badge.fury.io/py/vivarium-inputs
-        
-        .. image:: https://travis-ci.org/ihmeuw/vivarium_inputs.svg?branch=master
-            :target: https://travis-ci.org/ihmeuw/vivarium_inputs
-            :alt: Latest Version
-        
-        .. image:: https://readthedocs.org/projects/vivarium_inputs/badge/?version=latest
-            :target: https://vivarium_inputs.readthedocs.io/en/latest/?badge=latest
-            :alt: Latest Docs
-        
-        
-        This package is used to transform Global Burden of Disease data and package it into data artifacts
-        used as inputs into vivarium simulations.
-        
-        It requires access to the IHME cluster for use (but not for testing).
-        
-Platform: UNKNOWN
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: data
 Provides-Extra: dev
+License-File: LICENSE.txt
+License-File: AUTHORS.rst
+
+Vivarium Inputs
+===============
+
+.. image:: https://badge.fury.io/py/vivarium-inputs.svg
+    :target: https://badge.fury.io/py/vivarium-inputs
+
+.. image:: https://travis-ci.org/ihmeuw/vivarium_inputs.svg?branch=master
+    :target: https://travis-ci.org/ihmeuw/vivarium_inputs
+    :alt: Latest Version
+
+.. image:: https://readthedocs.org/projects/vivarium_inputs/badge/?version=latest
+    :target: https://vivarium_inputs.readthedocs.io/en/latest/?badge=latest
+    :alt: Latest Docs
+
+
+This package is used to transform Global Burden of Disease data and package it into data artifacts
+used as inputs into vivarium simulations.
+
+It requires access to the IHME cluster for use (but not for testing).
```

### Comparing `vivarium_inputs-4.0.9/src/vivarium_inputs.egg-info/SOURCES.txt` & `vivarium_inputs-4.1.0/src/vivarium_inputs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.0.9/tests/conftest.py` & `vivarium_inputs-4.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.0.9/tests/extract/test_core.py` & `vivarium_inputs-4.1.0/tests/extract/test_core.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.0.9/tests/extract/test_extract.py` & `vivarium_inputs-4.1.0/tests/extract/test_extract.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.0.9/tests/extract/test_get_measure.py` & `vivarium_inputs-4.1.0/tests/extract/test_get_measure.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.0.9/tests/extract/test_utility_data.py` & `vivarium_inputs-4.1.0/tests/extract/test_utility_data.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.0.9/tests/test_utilities.py` & `vivarium_inputs-4.1.0/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.0.9/tests/validation/test_raw.py` & `vivarium_inputs-4.1.0/tests/validation/test_raw.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.0.9/tests/validation/test_shared.py` & `vivarium_inputs-4.1.0/tests/validation/test_shared.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.0.9/tests/validation/test_sim.py` & `vivarium_inputs-4.1.0/tests/validation/test_sim.py`

 * *Files identical despite different names*

