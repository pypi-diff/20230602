# Comparing `tmp/voxcell-3.1.4.tar.gz` & `tmp/voxcell-3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voxcell-3.1.4.tar", last modified: Tue Mar 21 12:44:23 2023, max compression
+gzip compressed data, was "voxcell-3.1.5.tar", last modified: Fri Jun  2 07:57:21 2023, max compression
```

## Comparing `voxcell-3.1.4.tar` & `voxcell-3.1.5.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 12:44:23.610458 voxcell-3.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 12:44:23.602459 voxcell-3.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 12:44:23.602459 voxcell-3.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-03-21 12:44:15.000000 voxcell-3.1.4/.github/workflows/publish-sdist.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-03-21 12:44:15.000000 voxcell-3.1.4/.github/workflows/run-tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-21 12:44:15.000000 voxcell-3.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-03-21 12:44:15.000000 voxcell-3.1.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-03-21 12:44:15.000000 voxcell-3.1.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-21 12:44:15.000000 voxcell-3.1.4/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-03-21 12:44:15.000000 voxcell-3.1.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-03-21 12:44:15.000000 voxcell-3.1.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-21 12:44:15.000000 voxcell-3.1.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-21 12:44:15.000000 voxcell-3.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-03-21 12:44:23.610458 voxcell-3.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-03-21 12:44:15.000000 voxcell-3.1.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 12:44:23.602459 voxcell-3.1.4/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-03-21 12:44:15.000000 voxcell-3.1.4/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 12:44:23.606459 voxcell-3.1.4/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 12:44:23.606459 voxcell-3.1.4/doc/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 12:44:15.000000 voxcell-3.1.4/doc/source/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-03-21 12:44:15.000000 voxcell-3.1.4/doc/source/aibs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-03-21 12:44:15.000000 voxcell-3.1.4/doc/source/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 12:44:23.606459 voxcell-3.1.4/doc/source/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    45749 2023-03-21 12:44:15.000000 voxcell-3.1.4/doc/source/assets/combined_dist.png
--rw-r--r--   0 runner    (1001) docker     (123)    32876 2023-03-21 12:44:15.000000 voxcell-3.1.4/doc/source/assets/size_dist.png
--rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-03-21 12:44:15.000000 voxcell-3.1.4/doc/source/atlas.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-21 12:44:15.000000 voxcell-3.1.4/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-03-21 12:44:15.000000 voxcell-3.1.4/doc/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 12:44:23.602459 voxcell-3.1.4/doc/source/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 12:44:23.606459 voxcell-3.1.4/doc/source/extensions/bbp-table/
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-03-21 12:44:15.000000 voxcell-3.1.4/doc/source/extensions/bbp-table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-03-21 12:44:15.000000 voxcell-3.1.4/doc/source/extras.rst
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-21 12:44:15.000000 voxcell-3.1.4/doc/source/formats.rst
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-21 12:44:15.000000 voxcell-3.1.4/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-21 12:44:15.000000 voxcell-3.1.4/doc/source/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-03-21 12:44:15.000000 voxcell-3.1.4/doc/source/mask.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-03-21 12:44:15.000000 voxcell-3.1.4/doc/source/orientation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-03-21 12:44:15.000000 voxcell-3.1.4/doc/source/scalar.rst
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-21 12:44:15.000000 voxcell-3.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 12:44:23.610458 voxcell-3.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-03-21 12:44:15.000000 voxcell-3.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 12:44:23.606459 voxcell-3.1.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 12:44:23.606459 voxcell-3.1.4/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-03-21 12:44:15.000000 voxcell-3.1.4/tests/data/hierarchy.json
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-21 12:44:15.000000 voxcell-3.1.4/tests/data/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 12:44:23.606459 voxcell-3.1.4/tests/data/mvd2_mvd3/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-03-21 12:44:15.000000 voxcell-3.1.4/tests/data/mvd2_mvd3/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)   153026 2023-03-21 12:44:15.000000 voxcell-3.1.4/tests/data/mvd2_mvd3/circuit.mvd2
--rw-r--r--   0 runner    (1001) docker     (123)   175072 2023-03-21 12:44:15.000000 voxcell-3.1.4/tests/data/mvd2_mvd3/circuit.mvd3
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-21 12:44:15.000000 voxcell-3.1.4/tests/data/no_spacings_fail.nrrd
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-03-21 12:44:15.000000 voxcell-3.1.4/tests/data/region_map.json
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-21 12:44:15.000000 voxcell-3.1.4/tests/data/scalar.nrrd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 12:44:23.606459 voxcell-3.1.4/tests/data/sonata/
--rw-r--r--   0 runner    (1001) docker     (123)    40840 2023-03-21 12:44:15.000000 voxcell-3.1.4/tests/data/sonata/nodes_eulers.h5
--rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-03-21 12:44:15.000000 voxcell-3.1.4/tests/data/sonata/nodes_multi_types.h5
--rw-r--r--   0 runner    (1001) docker     (123)    12904 2023-03-21 12:44:15.000000 voxcell-3.1.4/tests/data/sonata/nodes_no_rotation.h5
--rw-r--r--   0 runner    (1001) docker     (123)    28912 2023-03-21 12:44:15.000000 voxcell-3.1.4/tests/data/sonata/nodes_quaternions.h5
--rw-r--r--   0 runner    (1001) docker     (123)    14224 2023-03-21 12:44:15.000000 voxcell-3.1.4/tests/data/sonata/nodes_quaternions_w_missing.h5
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-21 12:44:15.000000 voxcell-3.1.4/tests/data/space_directions.nrrd
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-21 12:44:15.000000 voxcell-3.1.4/tests/data/space_directions_fail.nrrd
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-21 12:44:15.000000 voxcell-3.1.4/tests/data/vector.nrrd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 12:44:23.606459 voxcell-3.1.4/tests/sonata/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-03-21 12:44:15.000000 voxcell-3.1.4/tests/sonata/test_node_population.py
--rw-r--r--   0 runner    (1001) docker     (123)    18393 2023-03-21 12:44:15.000000 voxcell-3.1.4/tests/test_cell_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    16706 2023-03-21 12:44:15.000000 voxcell-3.1.4/tests/test_math_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-03-21 12:44:15.000000 voxcell-3.1.4/tests/test_quaternion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-03-21 12:44:15.000000 voxcell-3.1.4/tests/test_region_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    13325 2023-03-21 12:44:15.000000 voxcell-3.1.4/tests/test_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-03-21 12:44:15.000000 voxcell-3.1.4/tests/test_vector_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    13760 2023-03-21 12:44:15.000000 voxcell-3.1.4/tests/test_voxel_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-03-21 12:44:15.000000 voxcell-3.1.4/tests/test_voxelbrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-03-21 12:44:15.000000 voxcell-3.1.4/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 12:44:23.610458 voxcell-3.1.4/voxcell/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-21 12:44:15.000000 voxcell-3.1.4/voxcell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20036 2023-03-21 12:44:15.000000 voxcell-3.1.4/voxcell/cell_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-21 12:44:15.000000 voxcell-3.1.4/voxcell/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8835 2023-03-21 12:44:15.000000 voxcell-3.1.4/voxcell/math_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 12:44:23.610458 voxcell-3.1.4/voxcell/nexus/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-21 12:44:15.000000 voxcell-3.1.4/voxcell/nexus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-03-21 12:44:15.000000 voxcell-3.1.4/voxcell/nexus/voxelbrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-03-21 12:44:15.000000 voxcell-3.1.4/voxcell/quaternion.py
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-03-21 12:44:15.000000 voxcell-3.1.4/voxcell/region_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 12:44:23.610458 voxcell-3.1.4/voxcell/sonata/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-21 12:44:15.000000 voxcell-3.1.4/voxcell/sonata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-21 12:44:15.000000 voxcell-3.1.4/voxcell/sonata/node_population.py
--rw-r--r--   0 runner    (1001) docker     (123)    12785 2023-03-21 12:44:15.000000 voxcell-3.1.4/voxcell/traits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 12:44:23.610458 voxcell-3.1.4/voxcell/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-21 12:44:15.000000 voxcell-3.1.4/voxcell/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-21 12:44:15.000000 voxcell-3.1.4/voxcell/utils/deprecate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-03-21 12:44:15.000000 voxcell-3.1.4/voxcell/vector_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    16742 2023-03-21 12:44:15.000000 voxcell-3.1.4/voxcell/voxel_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 12:44:23.610458 voxcell-3.1.4/voxcell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-03-21 12:44:23.000000 voxcell-3.1.4/voxcell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-03-21 12:44:23.000000 voxcell-3.1.4/voxcell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 12:44:23.000000 voxcell-3.1.4/voxcell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-21 12:44:23.000000 voxcell-3.1.4/voxcell.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-21 12:44:23.000000 voxcell-3.1.4/voxcell.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:57:21.206897 voxcell-3.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:57:21.194897 voxcell-3.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:57:21.198897 voxcell-3.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-02 07:57:13.000000 voxcell-3.1.5/.github/workflows/publish-sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-02 07:57:13.000000 voxcell-3.1.5/.github/workflows/run-tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-02 07:57:13.000000 voxcell-3.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-02 07:57:13.000000 voxcell-3.1.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-02 07:57:13.000000 voxcell-3.1.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-02 07:57:13.000000 voxcell-3.1.5/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-06-02 07:57:13.000000 voxcell-3.1.5/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-02 07:57:13.000000 voxcell-3.1.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-02 07:57:13.000000 voxcell-3.1.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-02 07:57:13.000000 voxcell-3.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-06-02 07:57:21.202897 voxcell-3.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-02 07:57:13.000000 voxcell-3.1.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:57:21.198897 voxcell-3.1.5/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-02 07:57:13.000000 voxcell-3.1.5/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:57:21.198897 voxcell-3.1.5/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:57:21.198897 voxcell-3.1.5/doc/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:57:13.000000 voxcell-3.1.5/doc/source/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-02 07:57:13.000000 voxcell-3.1.5/doc/source/aibs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-02 07:57:13.000000 voxcell-3.1.5/doc/source/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:57:21.198897 voxcell-3.1.5/doc/source/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    45749 2023-06-02 07:57:13.000000 voxcell-3.1.5/doc/source/assets/combined_dist.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32876 2023-06-02 07:57:13.000000 voxcell-3.1.5/doc/source/assets/size_dist.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-06-02 07:57:13.000000 voxcell-3.1.5/doc/source/atlas.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-02 07:57:13.000000 voxcell-3.1.5/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-06-02 07:57:13.000000 voxcell-3.1.5/doc/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:57:21.194897 voxcell-3.1.5/doc/source/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:57:21.198897 voxcell-3.1.5/doc/source/extensions/bbp-table/
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-06-02 07:57:13.000000 voxcell-3.1.5/doc/source/extensions/bbp-table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-06-02 07:57:13.000000 voxcell-3.1.5/doc/source/extras.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-02 07:57:13.000000 voxcell-3.1.5/doc/source/formats.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-02 07:57:13.000000 voxcell-3.1.5/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-02 07:57:13.000000 voxcell-3.1.5/doc/source/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-02 07:57:13.000000 voxcell-3.1.5/doc/source/mask.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-02 07:57:13.000000 voxcell-3.1.5/doc/source/orientation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-02 07:57:13.000000 voxcell-3.1.5/doc/source/scalar.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-02 07:57:13.000000 voxcell-3.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 07:57:21.206897 voxcell-3.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-02 07:57:13.000000 voxcell-3.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:57:21.198897 voxcell-3.1.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:57:21.202897 voxcell-3.1.5/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-02 07:57:13.000000 voxcell-3.1.5/tests/data/hierarchy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-02 07:57:13.000000 voxcell-3.1.5/tests/data/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:57:21.202897 voxcell-3.1.5/tests/data/mvd2_mvd3/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-02 07:57:13.000000 voxcell-3.1.5/tests/data/mvd2_mvd3/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   153026 2023-06-02 07:57:13.000000 voxcell-3.1.5/tests/data/mvd2_mvd3/circuit.mvd2
+-rw-r--r--   0 runner    (1001) docker     (123)   175072 2023-06-02 07:57:13.000000 voxcell-3.1.5/tests/data/mvd2_mvd3/circuit.mvd3
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-02 07:57:13.000000 voxcell-3.1.5/tests/data/no_spacings_fail.nrrd
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-02 07:57:13.000000 voxcell-3.1.5/tests/data/region_map.json
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-02 07:57:13.000000 voxcell-3.1.5/tests/data/scalar.nrrd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:57:21.202897 voxcell-3.1.5/tests/data/sonata/
+-rw-r--r--   0 runner    (1001) docker     (123)    40840 2023-06-02 07:57:13.000000 voxcell-3.1.5/tests/data/sonata/nodes_eulers.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-06-02 07:57:13.000000 voxcell-3.1.5/tests/data/sonata/nodes_multi_types.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    12904 2023-06-02 07:57:13.000000 voxcell-3.1.5/tests/data/sonata/nodes_no_rotation.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    28912 2023-06-02 07:57:13.000000 voxcell-3.1.5/tests/data/sonata/nodes_quaternions.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    14224 2023-06-02 07:57:13.000000 voxcell-3.1.5/tests/data/sonata/nodes_quaternions_w_missing.h5
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-02 07:57:13.000000 voxcell-3.1.5/tests/data/space_directions.nrrd
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-02 07:57:13.000000 voxcell-3.1.5/tests/data/space_directions_fail.nrrd
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-02 07:57:13.000000 voxcell-3.1.5/tests/data/vector.nrrd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:57:21.202897 voxcell-3.1.5/tests/sonata/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-02 07:57:13.000000 voxcell-3.1.5/tests/sonata/test_node_population.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18393 2023-06-02 07:57:13.000000 voxcell-3.1.5/tests/test_cell_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16706 2023-06-02 07:57:13.000000 voxcell-3.1.5/tests/test_math_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-06-02 07:57:13.000000 voxcell-3.1.5/tests/test_quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-06-02 07:57:13.000000 voxcell-3.1.5/tests/test_region_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13325 2023-06-02 07:57:13.000000 voxcell-3.1.5/tests/test_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-02 07:57:13.000000 voxcell-3.1.5/tests/test_vector_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-06-02 07:57:13.000000 voxcell-3.1.5/tests/test_voxel_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-06-02 07:57:13.000000 voxcell-3.1.5/tests/test_voxelbrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-02 07:57:13.000000 voxcell-3.1.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:57:21.202897 voxcell-3.1.5/voxcell/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-02 07:57:13.000000 voxcell-3.1.5/voxcell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20036 2023-06-02 07:57:13.000000 voxcell-3.1.5/voxcell/cell_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-02 07:57:13.000000 voxcell-3.1.5/voxcell/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8835 2023-06-02 07:57:13.000000 voxcell-3.1.5/voxcell/math_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:57:21.202897 voxcell-3.1.5/voxcell/nexus/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-02 07:57:13.000000 voxcell-3.1.5/voxcell/nexus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-06-02 07:57:13.000000 voxcell-3.1.5/voxcell/nexus/voxelbrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-06-02 07:57:13.000000 voxcell-3.1.5/voxcell/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-06-02 07:57:13.000000 voxcell-3.1.5/voxcell/region_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:57:21.202897 voxcell-3.1.5/voxcell/sonata/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-02 07:57:13.000000 voxcell-3.1.5/voxcell/sonata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-02 07:57:13.000000 voxcell-3.1.5/voxcell/sonata/node_population.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-06-02 07:57:13.000000 voxcell-3.1.5/voxcell/traits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:57:21.202897 voxcell-3.1.5/voxcell/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 07:57:13.000000 voxcell-3.1.5/voxcell/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-02 07:57:13.000000 voxcell-3.1.5/voxcell/utils/deprecate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-02 07:57:13.000000 voxcell-3.1.5/voxcell/vector_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16847 2023-06-02 07:57:13.000000 voxcell-3.1.5/voxcell/voxel_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:57:21.202897 voxcell-3.1.5/voxcell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-06-02 07:57:20.000000 voxcell-3.1.5/voxcell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-02 07:57:21.000000 voxcell-3.1.5/voxcell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 07:57:20.000000 voxcell-3.1.5/voxcell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-02 07:57:20.000000 voxcell-3.1.5/voxcell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 07:57:20.000000 voxcell-3.1.5/voxcell.egg-info/top_level.txt
```

### Comparing `voxcell-3.1.4/.github/workflows/publish-sdist.yml` & `voxcell-3.1.5/.github/workflows/publish-sdist.yml`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/.github/workflows/run-tox.yml` & `voxcell-3.1.5/.github/workflows/run-tox.yml`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/.pylintrc` & `voxcell-3.1.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/CHANGELOG.rst` & `voxcell-3.1.5/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+Version 3.1.5
+-------------
+
+- Fix outer value lookup with vector data (#19)
+- Fix compatibility with groupby from pandas 2.0
+
 Version 3.1.4
 -------------
 - switch hemisphere constants to be in line with Allen Institute
 
 Version 3.1.3
 -------------
 - Add a RegionMap conversion to Pandas DataFrame (#6)
```

### Comparing `voxcell-3.1.4/CONTRIBUTING.rst` & `voxcell-3.1.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/LICENSE.txt` & `voxcell-3.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/PKG-INFO` & `voxcell-3.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voxcell
-Version: 3.1.4
+Version: 3.1.5
 Summary: Voxcell is a small library to handle probability distributions that have a spatial component and to use them to build collection of cells in space.
 Home-page: https://github.com/BlueBrain/voxcell
 Author: Blue Brain Project, EPFL
 License: Apache-2
 Download-URL: https://github.com/BlueBrain/voxcell
 Description: Overview
         ========
```

### Comparing `voxcell-3.1.4/README.rst` & `voxcell-3.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/doc/Makefile` & `voxcell-3.1.5/doc/Makefile`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/doc/source/aibs.rst` & `voxcell-3.1.5/doc/source/aibs.rst`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/doc/source/api.rst` & `voxcell-3.1.5/doc/source/api.rst`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/doc/source/assets/combined_dist.png` & `voxcell-3.1.5/doc/source/assets/combined_dist.png`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/doc/source/assets/size_dist.png` & `voxcell-3.1.5/doc/source/assets/size_dist.png`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/doc/source/atlas.rst` & `voxcell-3.1.5/doc/source/atlas.rst`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/doc/source/conf.py` & `voxcell-3.1.5/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/doc/source/extensions/bbp-table/__init__.py` & `voxcell-3.1.5/doc/source/extensions/bbp-table/__init__.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/doc/source/extras.rst` & `voxcell-3.1.5/doc/source/extras.rst`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/doc/source/index.rst` & `voxcell-3.1.5/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/doc/source/mask.rst` & `voxcell-3.1.5/doc/source/mask.rst`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/doc/source/orientation.rst` & `voxcell-3.1.5/doc/source/orientation.rst`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/doc/source/scalar.rst` & `voxcell-3.1.5/doc/source/scalar.rst`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/setup.py` & `voxcell-3.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/tests/data/hierarchy.json` & `voxcell-3.1.5/tests/data/hierarchy.json`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/tests/data/mvd2_mvd3/circuit.mvd2` & `voxcell-3.1.5/tests/data/mvd2_mvd3/circuit.mvd2`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/tests/data/mvd2_mvd3/circuit.mvd3` & `voxcell-3.1.5/tests/data/mvd2_mvd3/circuit.mvd3`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/tests/data/region_map.json` & `voxcell-3.1.5/tests/data/region_map.json`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/tests/data/sonata/nodes_eulers.h5` & `voxcell-3.1.5/tests/data/sonata/nodes_eulers.h5`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/tests/data/sonata/nodes_multi_types.h5` & `voxcell-3.1.5/tests/data/sonata/nodes_multi_types.h5`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/tests/data/sonata/nodes_no_rotation.h5` & `voxcell-3.1.5/tests/data/sonata/nodes_no_rotation.h5`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/tests/data/sonata/nodes_quaternions.h5` & `voxcell-3.1.5/tests/data/sonata/nodes_quaternions.h5`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/tests/data/sonata/nodes_quaternions_w_missing.h5` & `voxcell-3.1.5/tests/data/sonata/nodes_quaternions_w_missing.h5`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/tests/test_cell_collection.py` & `voxcell-3.1.5/tests/test_cell_collection.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/tests/test_math_utils.py` & `voxcell-3.1.5/tests/test_math_utils.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/tests/test_quaternion.py` & `voxcell-3.1.5/tests/test_quaternion.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/tests/test_region_map.py` & `voxcell-3.1.5/tests/test_region_map.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/tests/test_traits.py` & `voxcell-3.1.5/tests/test_traits.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/tests/test_vector_fields.py` & `voxcell-3.1.5/tests/test_vector_fields.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/tests/test_voxel_data.py` & `voxcell-3.1.5/tests/test_voxel_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,18 +23,57 @@
     assert v.lookup([[2, 3]]) == [11]
     assert_array_equal(v.lookup([[2, 10], [1, 5]], outer_value=42), [42, 42])
     assert_array_equal(v.lookup([[2, 10], [1, 5], [4, 5]], outer_value=42), [42, 42, 22])
     assert_raises(VoxcellError, v.lookup, [[1, 5]])
     assert_raises(VoxcellError, v.lookup, [[2, 10]])
 
 
-def test_lookup_vector_data():
-    raw = np.array([[[11], [12]], [[21], [22]]])
-    v = test_module.VoxelData(raw, (2, 2))
-    assert_array_equal(v.lookup([[1, 1], [3, 3]]), [[11], [22]])
+@pytest.mark.parametrize(
+    "raw, voxel_dimensions, coordinates, outer_value, expected",
+    [
+        (
+            [[[11, 11], [12, 12]], [[21, 21], [22, 22]]],
+            (2, 2),
+            [[1, 1], [3, 3]],
+            None,
+            [[11, 11], [22, 22]],
+        ),
+        (
+            [[[11, 11], [12, 12]], [[21, 21], [22, 22]]],
+            (2, 2),
+            [[10, 1]],
+            [10, 10],
+            [[10, 10]],
+        ),
+        (
+            np.zeros((1, 1, 1)),
+            (1, 1, 1),
+            [(-1, -1, -1)],
+            0,
+            [0],
+        ),
+        (
+            np.zeros((1, 1, 1, 1)),
+            (1, 1, 1),
+            [(-1, -1, -1)],
+            0,
+            [(0,)],
+        ),
+        (
+            np.zeros((1, 1, 1, 2)),
+            (1, 1, 1),
+            [(-1, -1, -1)],
+            (0, 0),
+            [(0, 0)],
+        ),
+    ],
+)
+def test_lookup_vector_data(raw, voxel_dimensions, coordinates, outer_value, expected):
+    voxel_data = test_module.VoxelData(np.array(raw), voxel_dimensions)
+    assert_array_equal(voxel_data.lookup(coordinates, outer_value), expected)
 
 
 def test_positions_to_indices():
     raw = np.zeros(2)
     v = test_module.VoxelData(raw, voxel_dimensions=(10.0,), offset=(10.0,))
     assert_array_equal(v.positions_to_indices([15., 25.]), [0, 1])
     assert_array_equal(v.positions_to_indices([15., 25.], keep_fraction=True), [0.5, 1.5])
```

### Comparing `voxcell-3.1.4/tests/test_voxelbrain.py` & `voxcell-3.1.5/tests/test_voxelbrain.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/tox.ini` & `voxcell-3.1.5/tox.ini`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/voxcell/cell_collection.py` & `voxcell-3.1.5/voxcell/cell_collection.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/voxcell/math_utils.py` & `voxcell-3.1.5/voxcell/math_utils.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/voxcell/nexus/voxelbrain.py` & `voxcell-3.1.5/voxcell/nexus/voxelbrain.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/voxcell/quaternion.py` & `voxcell-3.1.5/voxcell/quaternion.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/voxcell/region_map.py` & `voxcell-3.1.5/voxcell/region_map.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/voxcell/traits.py` & `voxcell-3.1.5/voxcell/traits.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,20 +101,15 @@
         preassigned = preassigned.to_frame() if isinstance(preassigned, pd.Series) else preassigned
 
         subsections = self.split(list(preassigned.columns))
         chosen = np.ones(shape=(len(preassigned)), dtype=int) * -1
 
         unique_assigned = preassigned.drop_duplicates()
         for values_comb in unique_assigned.values:
-
-            if len(values_comb) == 1:
-                values_comb = values_comb[0]
-                hashable = values_comb
-            else:
-                hashable = tuple(values_comb)
+            hashable = tuple(values_comb)
 
             if hashable in subsections:
                 subdist = subsections[hashable]
                 mask = np.all(np.array(preassigned) == values_comb, axis=1)
                 chosen[mask] = subdist.assign(positions[mask])
 
         invalid_count = np.count_nonzero(chosen == -1)
@@ -175,14 +170,17 @@
 
         Returns:
             A dictionary where the keys are tuples with the values of the attributes found
             in the traits_collection and the values are the resulting SpatialDistribution objects.
         """
         grouped_distributions = {}
         for attr_values, traits in self.traits.groupby(attributes):
+            # this is backwards compatibility: https://github.com/pandas-dev/pandas/issues/42795
+            if len(attributes) == 1:
+                attr_values = tuple(attr_values)
 
             dists = self.distributions.iloc[traits.index]
 
             # remove dists that have become empty
             dists = dists[dists.columns[dists.sum() != 0]]
             dists /= dists.sum()
```

### Comparing `voxcell-3.1.4/voxcell/vector_fields.py` & `voxcell-3.1.5/voxcell/vector_fields.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.4/voxcell/voxel_data.py` & `voxcell-3.1.5/voxcell/voxel_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,19 @@
 
         Returns:
             Numpy array with the values of the voxels corresponding to each position.
         """
         voxel_idx = self.positions_to_indices(positions, strict=outer_value is None)
         outer_mask = np.any(voxel_idx == VoxelData.OUT_OF_BOUNDS, axis=-1)
         if np.any(outer_mask):
-            result = np.full(voxel_idx.shape[:-1], outer_value)
+            result = np.full(
+                voxel_idx.shape[:-1] + self.payload_shape,
+                outer_value,
+                dtype=self.raw.dtype
+            )
             inner_mask = np.logical_not(outer_mask)  # pylint: disable=assignment-from-no-return
             result[inner_mask] = self._lookup_by_indices(voxel_idx[inner_mask])
         else:
             result = self._lookup_by_indices(voxel_idx)
         return result
 
     def _lookup_by_indices(self, voxel_idx):
```

### Comparing `voxcell-3.1.4/voxcell.egg-info/PKG-INFO` & `voxcell-3.1.5/voxcell.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voxcell
-Version: 3.1.4
+Version: 3.1.5
 Summary: Voxcell is a small library to handle probability distributions that have a spatial component and to use them to build collection of cells in space.
 Home-page: https://github.com/BlueBrain/voxcell
 Author: Blue Brain Project, EPFL
 License: Apache-2
 Download-URL: https://github.com/BlueBrain/voxcell
 Description: Overview
         ========
```

### Comparing `voxcell-3.1.4/voxcell.egg-info/SOURCES.txt` & `voxcell-3.1.5/voxcell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

