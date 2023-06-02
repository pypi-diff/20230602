# Comparing `tmp/caosdb-0.8.0.tar.gz` & `tmp/caosdb-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caosdb-0.8.0.tar", last modified: Fri Jul 15 09:59:17 2022, max compression
+gzip compressed data, was "caosdb-0.9.0.tar", last modified: Mon Oct 24 19:00:07 2022, max compression
```

## Comparing `caosdb-0.8.0.tar` & `caosdb-0.9.0.tar`

### file list

```diff
@@ -1,157 +1,59 @@
-drwxr-xr-x   0 tf        (1000) tf        (1000)        0 2022-07-15 09:59:17.662940 caosdb-0.8.0/
--rw-r--r--   0 tf        (1000) tf        (1000)      197 2021-10-15 14:36:10.000000 caosdb-0.8.0/.gitignore
--rw-r--r--   0 tf        (1000) tf        (1000)     3203 2022-07-14 10:06:15.000000 caosdb-0.8.0/.gitlab-ci.yml
--rw-r--r--   0 tf        (1000) tf        (1000)    10487 2022-07-14 10:06:15.000000 caosdb-0.8.0/CHANGELOG.md
--rw-r--r--   0 tf        (1000) tf        (1000)      141 2022-07-14 10:06:15.000000 caosdb-0.8.0/DEPENDENCIES.md
--rw-r--r--   0 tf        (1000) tf        (1000)      398 2022-07-12 10:13:11.000000 caosdb-0.8.0/FEATURES.md
--rw-r--r--   0 tf        (1000) tf        (1000)    34283 2021-10-15 14:36:10.000000 caosdb-0.8.0/LICENSE.md
--rw-r--r--   0 tf        (1000) tf        (1000)     1346 2022-05-16 19:30:19.000000 caosdb-0.8.0/Makefile
--rw-r--r--   0 tf        (1000) tf        (1000)     2843 2022-07-15 09:59:17.663941 caosdb-0.8.0/PKG-INFO
--rw-r--r--   0 tf        (1000) tf        (1000)     2196 2022-05-16 19:30:05.000000 caosdb-0.8.0/README.md
--rw-r--r--   0 tf        (1000) tf        (1000)     3627 2022-07-14 10:06:15.000000 caosdb-0.8.0/README_SETUP.md
--rw-r--r--   0 tf        (1000) tf        (1000)     1644 2022-05-16 19:30:19.000000 caosdb-0.8.0/RELEASE_GUIDELINES.md
-drwxr-xr-x   0 tf        (1000) tf        (1000)        0 2022-07-15 09:59:17.590940 caosdb-0.8.0/examples/
--rw-r--r--   0 tf        (1000) tf        (1000)      161 2021-10-15 14:36:10.000000 caosdb-0.8.0/examples/caosdb_julia.jl
--rw-r--r--   0 tf        (1000) tf        (1000)     2587 2022-05-16 19:30:19.000000 caosdb-0.8.0/examples/pycaosdb.ini
--rwxr-xr-x   0 tf        (1000) tf        (1000)     1163 2021-10-15 14:36:10.000000 caosdb-0.8.0/examples/pycaosdb_example.py
--rwxr-xr-x   0 tf        (1000) tf        (1000)     2563 2021-10-15 14:36:10.000000 caosdb-0.8.0/examples/server_side_script.py
--rwxr-xr-x   0 tf        (1000) tf        (1000)     7600 2022-01-14 12:46:34.000000 caosdb-0.8.0/examples/set_permissions.py
--rw-r--r--   0 tf        (1000) tf        (1000)       57 2021-10-15 14:36:10.000000 caosdb-0.8.0/pytest.ini
--rwxr-xr-x   0 tf        (1000) tf        (1000)      106 2022-03-28 08:37:48.000000 caosdb-0.8.0/release.sh
--rw-r--r--   0 tf        (1000) tf        (1000)      131 2022-07-15 09:59:17.664940 caosdb-0.8.0/setup.cfg
--rwxr-xr-x   0 tf        (1000) tf        (1000)     6511 2022-07-14 10:06:15.000000 caosdb-0.8.0/setup.py
-drwxr-xr-x   0 tf        (1000) tf        (1000)        0 2022-07-15 09:59:17.578940 caosdb-0.8.0/src/
-drwxr-xr-x   0 tf        (1000) tf        (1000)        0 2022-07-15 09:59:17.596940 caosdb-0.8.0/src/caosdb/
--rw-r--r--   0 tf        (1000) tf        (1000)     2440 2022-05-16 19:30:05.000000 caosdb-0.8.0/src/caosdb/__init__.py
--rw-r--r--   0 tf        (1000) tf        (1000)    17102 2022-07-07 23:02:19.000000 caosdb-0.8.0/src/caosdb/apiutils.py
-drwxr-xr-x   0 tf        (1000) tf        (1000)        0 2022-07-15 09:59:17.599940 caosdb-0.8.0/src/caosdb/cert/
--rw-r--r--   0 tf        (1000) tf        (1000)     3495 2021-10-15 14:36:10.000000 caosdb-0.8.0/src/caosdb/cert/indiscale.ca.crt
-drwxr-xr-x   0 tf        (1000) tf        (1000)        0 2022-07-15 09:59:17.604941 caosdb-0.8.0/src/caosdb/common/
--rw-r--r--   0 tf        (1000) tf        (1000)       40 2021-10-15 14:36:10.000000 caosdb-0.8.0/src/caosdb/common/__init__.py
--rw-r--r--   0 tf        (1000) tf        (1000)    12523 2022-07-14 10:06:15.000000 caosdb-0.8.0/src/caosdb/common/administration.py
--rw-r--r--   0 tf        (1000) tf        (1000)     4632 2022-05-16 19:30:05.000000 caosdb-0.8.0/src/caosdb/common/datatype.py
--rw-r--r--   0 tf        (1000) tf        (1000)   153309 2022-07-14 10:06:15.000000 caosdb-0.8.0/src/caosdb/common/models.py
--rw-r--r--   0 tf        (1000) tf        (1000)     5698 2022-01-14 12:46:34.000000 caosdb-0.8.0/src/caosdb/common/state.py
--rw-r--r--   0 tf        (1000) tf        (1000)     1457 2022-07-14 10:06:15.000000 caosdb-0.8.0/src/caosdb/common/utils.py
--rw-r--r--   0 tf        (1000) tf        (1000)     9699 2021-10-15 14:36:10.000000 caosdb-0.8.0/src/caosdb/common/versioning.py
--rw-r--r--   0 tf        (1000) tf        (1000)     3549 2022-05-16 19:30:19.000000 caosdb-0.8.0/src/caosdb/configuration.py
-drwxr-xr-x   0 tf        (1000) tf        (1000)        0 2022-07-15 09:59:17.609940 caosdb-0.8.0/src/caosdb/connection/
--rw-r--r--   0 tf        (1000) tf        (1000)     9266 2021-10-15 14:36:10.000000 caosdb-0.8.0/src/caosdb/connection/SocksiPy.zip
--rw-r--r--   0 tf        (1000) tf        (1000)        0 2022-07-14 10:06:15.000000 caosdb-0.8.0/src/caosdb/connection/__init__.py
-drwxr-xr-x   0 tf        (1000) tf        (1000)        0 2022-07-15 09:59:17.615940 caosdb-0.8.0/src/caosdb/connection/authentication/
--rw-r--r--   0 tf        (1000) tf        (1000)        0 2021-10-15 14:36:10.000000 caosdb-0.8.0/src/caosdb/connection/authentication/__init__.py
--rw-r--r--   0 tf        (1000) tf        (1000)     3286 2021-10-15 14:36:10.000000 caosdb-0.8.0/src/caosdb/connection/authentication/auth_token.py
--rw-r--r--   0 tf        (1000) tf        (1000)     3350 2021-10-15 14:36:10.000000 caosdb-0.8.0/src/caosdb/connection/authentication/external_credentials_provider.py
--rw-r--r--   0 tf        (1000) tf        (1000)     2605 2021-10-15 14:36:10.000000 caosdb-0.8.0/src/caosdb/connection/authentication/input.py
--rw-r--r--   0 tf        (1000) tf        (1000)     7460 2022-05-16 19:30:05.000000 caosdb-0.8.0/src/caosdb/connection/authentication/interface.py
--rw-r--r--   0 tf        (1000) tf        (1000)     3256 2022-05-16 19:30:05.000000 caosdb-0.8.0/src/caosdb/connection/authentication/keyring.py
--rw-r--r--   0 tf        (1000) tf        (1000)     2818 2021-10-15 14:36:10.000000 caosdb-0.8.0/src/caosdb/connection/authentication/pass.py
--rw-r--r--   0 tf        (1000) tf        (1000)     2449 2021-10-15 14:36:10.000000 caosdb-0.8.0/src/caosdb/connection/authentication/plain.py
--rw-r--r--   0 tf        (1000) tf        (1000)     3265 2021-10-15 14:36:10.000000 caosdb-0.8.0/src/caosdb/connection/authentication/unauthenticated.py
--rw-r--r--   0 tf        (1000) tf        (1000)    20813 2022-07-14 10:06:15.000000 caosdb-0.8.0/src/caosdb/connection/connection.py
--rw-r--r--   0 tf        (1000) tf        (1000)    17222 2022-07-14 10:06:15.000000 caosdb-0.8.0/src/caosdb/connection/encode.py
--rw-r--r--   0 tf        (1000) tf        (1000)     2895 2021-10-15 14:36:10.000000 caosdb-0.8.0/src/caosdb/connection/interface.py
--rw-r--r--   0 tf        (1000) tf        (1000)     3620 2022-07-14 10:06:15.000000 caosdb-0.8.0/src/caosdb/connection/mockup.py
--rw-r--r--   0 tf        (1000) tf        (1000)     6206 2021-10-15 14:36:10.000000 caosdb-0.8.0/src/caosdb/connection/streaminghttp.py
--rw-r--r--   0 tf        (1000) tf        (1000)     5132 2022-07-14 10:06:15.000000 caosdb-0.8.0/src/caosdb/connection/utils.py
--rw-r--r--   0 tf        (1000) tf        (1000)    10817 2022-05-16 19:30:05.000000 caosdb-0.8.0/src/caosdb/exceptions.py
--rw-r--r--   0 tf        (1000) tf        (1000)    35442 2022-07-07 23:02:19.000000 caosdb-0.8.0/src/caosdb/high_level_api.py
--rw-r--r--   0 tf        (1000) tf        (1000)     4145 2022-05-16 19:30:19.000000 caosdb-0.8.0/src/caosdb/schema-pycaosdb-ini.yml
-drwxr-xr-x   0 tf        (1000) tf        (1000)        0 2022-07-15 09:59:17.619940 caosdb-0.8.0/src/caosdb/utils/
--rw-r--r--   0 tf        (1000) tf        (1000)        0 2021-10-15 14:36:10.000000 caosdb-0.8.0/src/caosdb/utils/__init__.py
--rwxr-xr-x   0 tf        (1000) tf        (1000)    22747 2022-05-16 19:30:05.000000 caosdb-0.8.0/src/caosdb/utils/caosdb_admin.py
--rwxr-xr-x   0 tf        (1000) tf        (1000)     3780 2021-10-15 14:36:10.000000 caosdb-0.8.0/src/caosdb/utils/checkFileSystemConsistency.py
--rw-r--r--   0 tf        (1000) tf        (1000)     3190 2021-10-15 14:36:10.000000 caosdb-0.8.0/src/caosdb/utils/create_revision.py
--rw-r--r--   0 tf        (1000) tf        (1000)    14527 2022-07-07 23:02:19.000000 caosdb-0.8.0/src/caosdb/utils/plantuml.py
--rw-r--r--   0 tf        (1000) tf        (1000)     4449 2021-10-15 14:36:10.000000 caosdb-0.8.0/src/caosdb/utils/server_side_scripting.py
--rw-r--r--   0 tf        (1000) tf        (1000)      231 2022-07-15 09:59:09.000000 caosdb-0.8.0/src/caosdb/version.py
--rw-r--r--   0 tf        (1000) tf        (1000)     6238 2022-05-16 19:30:05.000000 caosdb-0.8.0/src/caosdb/yamlapi.py
-drwxr-xr-x   0 tf        (1000) tf        (1000)        0 2022-07-15 09:59:17.599940 caosdb-0.8.0/src/caosdb.egg-info/
--rw-r--r--   0 tf        (1000) tf        (1000)     2843 2022-07-15 09:59:15.000000 caosdb-0.8.0/src/caosdb.egg-info/PKG-INFO
--rw-r--r--   0 tf        (1000) tf        (1000)     4281 2022-07-15 09:59:17.000000 caosdb-0.8.0/src/caosdb.egg-info/SOURCES.txt
--rw-r--r--   0 tf        (1000) tf        (1000)        1 2022-07-15 09:59:15.000000 caosdb-0.8.0/src/caosdb.egg-info/dependency_links.txt
--rw-r--r--   0 tf        (1000) tf        (1000)      105 2022-07-15 09:59:16.000000 caosdb-0.8.0/src/caosdb.egg-info/requires.txt
--rw-r--r--   0 tf        (1000) tf        (1000)        7 2022-07-15 09:59:16.000000 caosdb-0.8.0/src/caosdb.egg-info/top_level.txt
-drwxr-xr-x   0 tf        (1000) tf        (1000)        0 2022-07-15 09:59:17.625940 caosdb-0.8.0/src/doc/
--rw-r--r--   0 tf        (1000) tf        (1000)     1717 2022-05-16 19:30:05.000000 caosdb-0.8.0/src/doc/Makefile
--rw-r--r--   0 tf        (1000) tf        (1000)     3627 2022-07-14 10:06:15.000000 caosdb-0.8.0/src/doc/README_SETUP.md
--rw-r--r--   0 tf        (1000) tf        (1000)      498 2022-01-14 12:46:34.000000 caosdb-0.8.0/src/doc/administration.rst
--rw-r--r--   0 tf        (1000) tf        (1000)      111 2021-10-15 14:36:10.000000 caosdb-0.8.0/src/doc/concepts.rst
--rw-r--r--   0 tf        (1000) tf        (1000)     6597 2022-07-14 10:06:15.000000 caosdb-0.8.0/src/doc/conf.py
--rw-r--r--   0 tf        (1000) tf        (1000)     2996 2022-07-06 19:25:53.000000 caosdb-0.8.0/src/doc/configuration.md
--rw-r--r--   0 tf        (1000) tf        (1000)     7032 2022-07-06 19:25:53.000000 caosdb-0.8.0/src/doc/future_caosdb.md
-drwxr-xr-x   0 tf        (1000) tf        (1000)        0 2022-07-15 09:59:17.628940 caosdb-0.8.0/src/doc/gallery/
--rw-r--r--   0 tf        (1000) tf        (1000)      907 2022-05-16 19:30:19.000000 caosdb-0.8.0/src/doc/gallery/Makefile
--rw-r--r--   0 tf        (1000) tf        (1000)      414 2022-05-16 19:30:19.000000 caosdb-0.8.0/src/doc/gallery/index.rst
--rw-r--r--   0 tf        (1000) tf        (1000)     4715 2022-05-16 19:30:19.000000 caosdb-0.8.0/src/doc/gallery/simulation.py
--rw-r--r--   0 tf        (1000) tf        (1000)      379 2022-05-16 19:30:19.000000 caosdb-0.8.0/src/doc/gallery/simulation.rst
--rw-r--r--   0 tf        (1000) tf        (1000)     8079 2022-07-06 19:25:53.000000 caosdb-0.8.0/src/doc/high_level_api.org
--rw-r--r--   0 tf        (1000) tf        (1000)     5856 2022-07-06 19:25:53.000000 caosdb-0.8.0/src/doc/high_level_api.rst
--rw-r--r--   0 tf        (1000) tf        (1000)      743 2022-07-06 19:25:53.000000 caosdb-0.8.0/src/doc/index.rst
-drwxr-xr-x   0 tf        (1000) tf        (1000)        0 2022-07-15 09:59:17.633940 caosdb-0.8.0/src/doc/tutorials/
--rw-r--r--   0 tf        (1000) tf        (1000)     6413 2022-05-16 19:30:05.000000 caosdb-0.8.0/src/doc/tutorials/Data-Insertion.rst
--rw-r--r--   0 tf        (1000) tf        (1000)     1501 2021-10-15 14:36:10.000000 caosdb-0.8.0/src/doc/tutorials/basic_analysis.rst
--rw-r--r--   0 tf        (1000) tf        (1000)     3245 2022-05-16 19:30:05.000000 caosdb-0.8.0/src/doc/tutorials/complex_data_models.rst
--rw-r--r--   0 tf        (1000) tf        (1000)      856 2021-10-15 14:36:10.000000 caosdb-0.8.0/src/doc/tutorials/data-model-interface.md
--rw-r--r--   0 tf        (1000) tf        (1000)     6511 2022-01-14 12:46:34.000000 caosdb-0.8.0/src/doc/tutorials/errors.rst
--rw-r--r--   0 tf        (1000) tf        (1000)     4865 2022-01-14 12:46:34.000000 caosdb-0.8.0/src/doc/tutorials/first_steps.rst
--rw-r--r--   0 tf        (1000) tf        (1000)      343 2022-05-16 19:30:19.000000 caosdb-0.8.0/src/doc/tutorials/index.rst
--rw-r--r--   0 tf        (1000) tf        (1000)     1947 2022-05-16 19:30:19.000000 caosdb-0.8.0/src/doc/tutorials/serverside.rst
--rw-r--r--   0 tf        (1000) tf        (1000)      236 2022-07-14 10:06:15.000000 caosdb-0.8.0/tox.ini
-drwxr-xr-x   0 tf        (1000) tf        (1000)        0 2022-07-15 09:59:17.654940 caosdb-0.8.0/unittests/
--rw-r--r--   0 tf        (1000) tf        (1000)        0 2021-10-15 14:36:10.000000 caosdb-0.8.0/unittests/__init__.py
-drwxr-xr-x   0 tf        (1000) tf        (1000)        0 2022-07-15 09:59:17.656940 caosdb-0.8.0/unittests/broken_configs/
--rw-r--r--   0 tf        (1000) tf        (1000)      150 2022-05-16 19:30:05.000000 caosdb-0.8.0/unittests/broken_configs/pycaosdb1.ini
--rw-r--r--   0 tf        (1000) tf        (1000)      188 2022-05-16 19:30:05.000000 caosdb-0.8.0/unittests/broken_configs/pycaosdb2.ini
--rw-r--r--   0 tf        (1000) tf        (1000)      157 2022-05-16 19:30:05.000000 caosdb-0.8.0/unittests/broken_configs/pycaosdb3.ini
--rw-r--r--   0 tf        (1000) tf        (1000)      143 2022-05-16 19:30:05.000000 caosdb-0.8.0/unittests/broken_configs/pycaosdb4.ini
-drwxr-xr-x   0 tf        (1000) tf        (1000)        0 2022-07-15 09:59:17.656940 caosdb-0.8.0/unittests/data/
--rw-r--r--   0 tf        (1000) tf        (1000)      514 2022-05-16 19:30:19.000000 caosdb-0.8.0/unittests/data/list_in_value.xml
-drwxr-xr-x   0 tf        (1000) tf        (1000)        0 2022-07-15 09:59:17.657940 caosdb-0.8.0/unittests/docker/
--rw-r--r--   0 tf        (1000) tf        (1000)      359 2022-01-14 12:46:34.000000 caosdb-0.8.0/unittests/docker/Dockerfile
--rw-r--r--   0 tf        (1000) tf        (1000)     2052 2022-05-16 19:30:19.000000 caosdb-0.8.0/unittests/test_acl.py
--rw-r--r--   0 tf        (1000) tf        (1000)    10402 2022-05-16 19:30:05.000000 caosdb-0.8.0/unittests/test_add_property.py
--rw-r--r--   0 tf        (1000) tf        (1000)     2965 2021-10-15 14:36:10.000000 caosdb-0.8.0/unittests/test_administraction.py
--rw-r--r--   0 tf        (1000) tf        (1000)    11236 2022-07-06 19:25:53.000000 caosdb-0.8.0/unittests/test_apiutils.py
--rw-r--r--   0 tf        (1000) tf        (1000)     3525 2022-07-14 10:06:15.000000 caosdb-0.8.0/unittests/test_authentication_auth_token.py
--rw-r--r--   0 tf        (1000) tf        (1000)     1873 2021-10-15 14:36:10.000000 caosdb-0.8.0/unittests/test_authentication_external.py
--rw-r--r--   0 tf        (1000) tf        (1000)     1400 2021-10-15 14:36:10.000000 caosdb-0.8.0/unittests/test_authentication_keyring.py
--rw-r--r--   0 tf        (1000) tf        (1000)     1436 2021-10-15 14:36:10.000000 caosdb-0.8.0/unittests/test_authentication_pass.py
--rw-r--r--   0 tf        (1000) tf        (1000)     2575 2022-05-16 19:30:05.000000 caosdb-0.8.0/unittests/test_authentication_plain.py
--rw-r--r--   0 tf        (1000) tf        (1000)     2559 2022-07-14 10:06:15.000000 caosdb-0.8.0/unittests/test_authentication_unauthenticated.py
--rw-r--r--   0 tf        (1000) tf        (1000)     1688 2021-10-15 14:36:10.000000 caosdb-0.8.0/unittests/test_concrete_property.py
-drwxr-xr-x   0 tf        (1000) tf        (1000)        0 2022-07-15 09:59:17.662940 caosdb-0.8.0/unittests/test_configs/
--rw-r--r--   0 tf        (1000) tf        (1000)     1706 2022-05-16 19:30:19.000000 caosdb-0.8.0/unittests/test_configs/pycaosdb-IntegrationTests.ini
--rw-r--r--   0 tf        (1000) tf        (1000)        0 2022-05-16 19:30:19.000000 caosdb-0.8.0/unittests/test_configs/pycaosdb-empty.ini
--rw-r--r--   0 tf        (1000) tf        (1000)      166 2022-05-16 19:30:05.000000 caosdb-0.8.0/unittests/test_configs/pycaosdb-indiscale-demo.ini
--rw-r--r--   0 tf        (1000) tf        (1000)      416 2022-05-16 19:30:19.000000 caosdb-0.8.0/unittests/test_configs/pycaosdb-real-world-1.ini
--rw-r--r--   0 tf        (1000) tf        (1000)      446 2022-05-16 19:30:19.000000 caosdb-0.8.0/unittests/test_configs/pycaosdb-real-world-2.ini
--rw-r--r--   0 tf        (1000) tf        (1000)      228 2022-05-16 19:30:19.000000 caosdb-0.8.0/unittests/test_configs/pycaosdb-server-side-scripting.ini
--rw-r--r--   0 tf        (1000) tf        (1000)      185 2022-05-16 19:30:05.000000 caosdb-0.8.0/unittests/test_configs/pycaosdb1.ini
--rw-r--r--   0 tf        (1000) tf        (1000)      188 2022-05-16 19:30:05.000000 caosdb-0.8.0/unittests/test_configs/pycaosdb2.ini
--rw-r--r--   0 tf        (1000) tf        (1000)      157 2022-05-16 19:30:05.000000 caosdb-0.8.0/unittests/test_configs/pycaosdb3.ini
--rw-r--r--   0 tf        (1000) tf        (1000)       79 2022-05-16 19:30:19.000000 caosdb-0.8.0/unittests/test_configs/pycaosdb4.ini
--rw-r--r--   0 tf        (1000) tf        (1000)      108 2022-05-16 19:30:19.000000 caosdb-0.8.0/unittests/test_configs/pycaosdb5.ini
--rw-r--r--   0 tf        (1000) tf        (1000)     2456 2022-01-14 12:46:34.000000 caosdb-0.8.0/unittests/test_configuration.py
--rw-r--r--   0 tf        (1000) tf        (1000)    10438 2022-07-14 10:06:15.000000 caosdb-0.8.0/unittests/test_connection.py
--rw-r--r--   0 tf        (1000) tf        (1000)     2116 2021-10-15 14:36:10.000000 caosdb-0.8.0/unittests/test_connection_utils.py
--rw-r--r--   0 tf        (1000) tf        (1000)     5639 2022-05-16 19:30:05.000000 caosdb-0.8.0/unittests/test_container.py
--rw-r--r--   0 tf        (1000) tf        (1000)     3200 2021-10-15 14:36:10.000000 caosdb-0.8.0/unittests/test_datatype.py
--rw-r--r--   0 tf        (1000) tf        (1000)     3616 2022-07-06 19:32:15.000000 caosdb-0.8.0/unittests/test_entity.py
--rw-r--r--   0 tf        (1000) tf        (1000)    11695 2021-10-15 14:36:10.000000 caosdb-0.8.0/unittests/test_error_handling.py
--rw-r--r--   0 tf        (1000) tf        (1000)     1829 2021-10-15 14:36:10.000000 caosdb-0.8.0/unittests/test_file.py
--rw-r--r--   0 tf        (1000) tf        (1000)    21611 2022-07-06 19:25:53.000000 caosdb-0.8.0/unittests/test_high_level_api.py
--rw-r--r--   0 tf        (1000) tf        (1000)     1375 2022-05-16 19:30:19.000000 caosdb-0.8.0/unittests/test_issues.py
--rw-r--r--   0 tf        (1000) tf        (1000)     3949 2021-10-15 14:36:10.000000 caosdb-0.8.0/unittests/test_message.py
--rw-r--r--   0 tf        (1000) tf        (1000)     1912 2022-07-06 19:25:53.000000 caosdb-0.8.0/unittests/test_plantuml.py
--rw-r--r--   0 tf        (1000) tf        (1000)     4344 2022-05-16 19:30:05.000000 caosdb-0.8.0/unittests/test_property.py
--rw-r--r--   0 tf        (1000) tf        (1000)     1614 2022-01-14 12:46:34.000000 caosdb-0.8.0/unittests/test_query.py
--rw-r--r--   0 tf        (1000) tf        (1000)     2423 2021-10-15 14:36:10.000000 caosdb-0.8.0/unittests/test_record.py
--rw-r--r--   0 tf        (1000) tf        (1000)    10504 2021-10-15 14:36:10.000000 caosdb-0.8.0/unittests/test_record.xml
--rw-r--r--   0 tf        (1000) tf        (1000)     1718 2021-10-15 14:36:10.000000 caosdb-0.8.0/unittests/test_record_type.py
--rw-r--r--   0 tf        (1000) tf        (1000)     1772 2022-05-16 19:30:19.000000 caosdb-0.8.0/unittests/test_schema.py
--rw-r--r--   0 tf        (1000) tf        (1000)     4323 2021-10-15 14:36:10.000000 caosdb-0.8.0/unittests/test_server_side_scripting.py
--rw-r--r--   0 tf        (1000) tf        (1000)     2450 2022-01-14 12:46:34.000000 caosdb-0.8.0/unittests/test_state.py
--rw-r--r--   0 tf        (1000) tf        (1000)     1175 2021-10-15 14:36:10.000000 caosdb-0.8.0/unittests/test_utils.py
--rw-r--r--   0 tf        (1000) tf        (1000)     7103 2021-10-15 14:36:10.000000 caosdb-0.8.0/unittests/test_versioning.py
--rw-r--r--   0 tf        (1000) tf        (1000)     2957 2022-05-16 19:30:05.000000 caosdb-0.8.0/unittests/test_yamlapi.py
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2022-10-24 19:00:07.247152 caosdb-0.9.0/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    34283 2021-06-28 12:57:59.000000 caosdb-0.9.0/LICENSE.md
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2823 2022-10-24 19:00:07.247152 caosdb-0.9.0/PKG-INFO
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2196 2022-10-24 18:58:51.000000 caosdb-0.9.0/README.md
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      131 2022-10-24 19:00:07.250486 caosdb-0.9.0/setup.cfg
+-rwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     6513 2022-10-24 18:58:51.000000 caosdb-0.9.0/setup.py
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2022-10-24 19:00:07.240486 caosdb-0.9.0/src/
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2022-10-24 19:00:07.243819 caosdb-0.9.0/src/caosdb/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2440 2022-05-31 09:40:09.000000 caosdb-0.9.0/src/caosdb/__init__.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    17700 2022-10-24 18:58:51.000000 caosdb-0.9.0/src/caosdb/apiutils.py
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2022-10-24 19:00:07.243819 caosdb-0.9.0/src/caosdb/cert/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3495 2021-06-28 12:57:59.000000 caosdb-0.9.0/src/caosdb/cert/indiscale.ca.crt
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2022-10-24 19:00:07.243819 caosdb-0.9.0/src/caosdb/common/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)       40 2021-06-28 12:57:59.000000 caosdb-0.9.0/src/caosdb/common/__init__.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    12523 2022-10-24 18:58:51.000000 caosdb-0.9.0/src/caosdb/common/administration.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     4632 2022-05-31 09:40:09.000000 caosdb-0.9.0/src/caosdb/common/datatype.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)   153594 2022-10-24 18:58:51.000000 caosdb-0.9.0/src/caosdb/common/models.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     5698 2022-05-25 07:14:04.000000 caosdb-0.9.0/src/caosdb/common/state.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      444 2022-10-24 18:58:51.000000 caosdb-0.9.0/src/caosdb/common/timezone.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     1457 2022-10-24 18:58:51.000000 caosdb-0.9.0/src/caosdb/common/utils.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     9699 2021-06-28 12:57:59.000000 caosdb-0.9.0/src/caosdb/common/versioning.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3549 2022-05-31 09:40:09.000000 caosdb-0.9.0/src/caosdb/configuration.py
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2022-10-24 19:00:07.247152 caosdb-0.9.0/src/caosdb/connection/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2022-10-24 18:58:51.000000 caosdb-0.9.0/src/caosdb/connection/__init__.py
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2022-10-24 19:00:07.247152 caosdb-0.9.0/src/caosdb/connection/authentication/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2021-06-28 12:57:59.000000 caosdb-0.9.0/src/caosdb/connection/authentication/__init__.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3286 2021-06-28 12:57:59.000000 caosdb-0.9.0/src/caosdb/connection/authentication/auth_token.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3350 2021-06-28 12:57:59.000000 caosdb-0.9.0/src/caosdb/connection/authentication/external_credentials_provider.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2605 2021-06-28 12:57:59.000000 caosdb-0.9.0/src/caosdb/connection/authentication/input.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     7460 2022-05-31 09:40:09.000000 caosdb-0.9.0/src/caosdb/connection/authentication/interface.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3256 2022-05-31 09:40:09.000000 caosdb-0.9.0/src/caosdb/connection/authentication/keyring.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2818 2021-06-28 12:57:59.000000 caosdb-0.9.0/src/caosdb/connection/authentication/pass.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2449 2021-06-28 12:57:59.000000 caosdb-0.9.0/src/caosdb/connection/authentication/plain.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3265 2021-06-28 12:57:59.000000 caosdb-0.9.0/src/caosdb/connection/authentication/unauthenticated.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    20813 2022-10-24 18:58:51.000000 caosdb-0.9.0/src/caosdb/connection/connection.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    17222 2022-10-24 18:58:51.000000 caosdb-0.9.0/src/caosdb/connection/encode.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2895 2021-06-28 12:57:59.000000 caosdb-0.9.0/src/caosdb/connection/interface.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3620 2022-10-24 18:58:51.000000 caosdb-0.9.0/src/caosdb/connection/mockup.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     6206 2021-06-28 12:57:59.000000 caosdb-0.9.0/src/caosdb/connection/streaminghttp.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     5132 2022-10-24 18:58:51.000000 caosdb-0.9.0/src/caosdb/connection/utils.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    10817 2022-05-31 09:40:09.000000 caosdb-0.9.0/src/caosdb/exceptions.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    35442 2022-07-28 15:02:01.000000 caosdb-0.9.0/src/caosdb/high_level_api.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     4162 2022-10-24 18:58:51.000000 caosdb-0.9.0/src/caosdb/schema-pycaosdb-ini.yml
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2022-10-24 19:00:07.247152 caosdb-0.9.0/src/caosdb/utils/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2021-06-28 12:57:59.000000 caosdb-0.9.0/src/caosdb/utils/__init__.py
+-rwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    22747 2022-05-31 09:40:09.000000 caosdb-0.9.0/src/caosdb/utils/caosdb_admin.py
+-rwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3780 2021-06-28 12:57:59.000000 caosdb-0.9.0/src/caosdb/utils/checkFileSystemConsistency.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3190 2021-06-28 12:57:59.000000 caosdb-0.9.0/src/caosdb/utils/create_revision.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    14527 2022-07-28 15:02:01.000000 caosdb-0.9.0/src/caosdb/utils/plantuml.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     4916 2022-10-24 18:58:51.000000 caosdb-0.9.0/src/caosdb/utils/register_tests.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     4449 2021-06-28 12:57:59.000000 caosdb-0.9.0/src/caosdb/utils/server_side_scripting.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      231 2022-10-24 19:00:06.000000 caosdb-0.9.0/src/caosdb/version.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     6238 2022-05-31 09:40:09.000000 caosdb-0.9.0/src/caosdb/yamlapi.py
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2022-10-24 19:00:07.243819 caosdb-0.9.0/src/caosdb.egg-info/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2823 2022-10-24 19:00:07.000000 caosdb-0.9.0/src/caosdb.egg-info/PKG-INFO
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     1639 2022-10-24 19:00:07.000000 caosdb-0.9.0/src/caosdb.egg-info/SOURCES.txt
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        1 2022-10-24 19:00:07.000000 caosdb-0.9.0/src/caosdb.egg-info/dependency_links.txt
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      107 2022-10-24 19:00:07.000000 caosdb-0.9.0/src/caosdb.egg-info/requires.txt
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        7 2022-10-24 19:00:07.000000 caosdb-0.9.0/src/caosdb.egg-info/top_level.txt
```

### Comparing `caosdb-0.8.0/LICENSE.md` & `caosdb-0.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `caosdb-0.8.0/PKG-INFO` & `caosdb-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: caosdb
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python Interface for CaosDB
 Home-page: https://www.caosdb.org
 Author: Timm Fitschen
 Author-email: t.fitschen@indiscale.com
 License: AGPLv3+
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -63,13 +62,11 @@
   CaosDB community on
   [#caosdb:matrix.org](https://matrix.to/#/!unwwlTfOznjEnMMXxf:matrix.org).
 
 ## License
 
 * Copyright (C) 2018 Research Group Biomedical Physics, Max Planck Institute
   for Dynamics and Self-Organization Göttingen.
-* Copyright (C) 2020-2021 Indiscale GmbH <info@indiscale.com>
+* Copyright (C) 2020-2022 Indiscale GmbH <info@indiscale.com>
 
 All files in this repository are licensed under a [GNU Affero General Public
 License](LICENCE.md) (version 3 or later).
-
-
```

### Comparing `caosdb-0.8.0/README.md` & `caosdb-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -43,11 +43,11 @@
   CaosDB community on
   [#caosdb:matrix.org](https://matrix.to/#/!unwwlTfOznjEnMMXxf:matrix.org).
 
 ## License
 
 * Copyright (C) 2018 Research Group Biomedical Physics, Max Planck Institute
   for Dynamics and Self-Organization Göttingen.
-* Copyright (C) 2020-2021 Indiscale GmbH <info@indiscale.com>
+* Copyright (C) 2020-2022 Indiscale GmbH <info@indiscale.com>
 
 All files in this repository are licensed under a [GNU Affero General Public
 License](LICENCE.md) (version 3 or later).
```

### Comparing `caosdb-0.8.0/setup.py` & `caosdb-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 # THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 ########################################################################
 
 ISRELEASED = True
 MAJOR = 0
-MINOR = 8
+MINOR = 9
 MICRO = 0
 # Do not tag as pre-release until this commit
 # https://github.com/pypa/packaging/pull/515
 # has made it into a release. Probably we should wait for pypa/packaging>=21.4
 # https://github.com/pypa/packaging/releases
 PRE = "" # "dev"  # e.g. rc0, alpha.1, 0.beta-23
 
@@ -167,15 +167,15 @@
             "Topic :: Database",
             "Topic :: Scientific/Engineering :: Information Analysis",
         ],
         packages=find_packages('src'),
         python_requires='>=3.8',
         package_dir={'': 'src'},
         install_requires=['lxml>=4.6.3',
-                          'PyYAML>=6.0', 'future', 'PySocks>=1.6.7'],
+                          'PyYAML>=5.4.1', 'future', 'PySocks>=1.6.7'],
         extras_require={'keyring': ['keyring>=13.0.0'],
                         'jsonschema': ['jsonschema>=4.4.0']},
         setup_requires=["pytest-runner>=2.0,<3dev"],
         tests_require=["pytest", "pytest-cov", "coverage>=4.4.2",
                        "jsonschema>=4.4.0"],
         package_data={
             'caosdb': ['cert/indiscale.ca.crt', 'schema-pycaosdb-ini.yml'],
```

### Comparing `caosdb-0.8.0/src/caosdb/__init__.py` & `caosdb-0.9.0/src/caosdb/__init__.py`

 * *Files identical despite different names*

### Comparing `caosdb-0.8.0/src/caosdb/apiutils.py` & `caosdb-0.9.0/src/caosdb/apiutils.py`

 * *Files 5% similar despite different names*

```diff
@@ -334,19 +334,27 @@
                         diff_r2["properties"][key]["importance"]):
                     raise NotImplementedError()
             elif ("importance" in diff_r1["properties"][key] or
                   "importance" in diff_r2["properties"][key]):
                 raise NotImplementedError()
 
             for attribute in ("datatype", "unit", "value"):
-                if diff_r1["properties"][key][attribute] is None:
-                    setattr(entity_a.get_property(key), attribute,
-                            diff_r2["properties"][key][attribute])
-                else:
-                    raise RuntimeError("Merge conflict.")
+                if (attribute in diff_r2["properties"][key] and
+                        diff_r2["properties"][key][attribute] is not None):
+                    if (diff_r1["properties"][key][attribute] is None):
+                        setattr(entity_a.get_property(key), attribute,
+                                diff_r2["properties"][key][attribute])
+                    else:
+                        raise RuntimeError(
+                            f"Merge conflict:\nEntity a ({entity_a.id}, {entity_a.name}) "
+                            f"has a Property '{key}' with {attribute}="
+                            f"{diff_r2['properties'][key][attribute]}\n"
+                            f"Entity b ({entity_b.id}, {entity_b.name}) "
+                            f"has a Property '{key}' with {attribute}="
+                            f"{diff_r1['properties'][key][attribute]}")
         else:
             # TODO: This is a temporary FIX for
             #       https://gitlab.indiscale.com/caosdb/src/caosdb-pylib/-/issues/105
             entity_a.add_property(id=entity_b.get_property(key).id,
                                   name=entity_b.get_property(key).name,
                                   datatype=entity_b.get_property(key).datatype,
                                   value=entity_b.get_property(key).value,
```

### Comparing `caosdb-0.8.0/src/caosdb/cert/indiscale.ca.crt` & `caosdb-0.9.0/src/caosdb/cert/indiscale.ca.crt`

 * *Files identical despite different names*

### Comparing `caosdb-0.8.0/src/caosdb/common/administration.py` & `caosdb-0.9.0/src/caosdb/common/administration.py`

 * *Files identical despite different names*

### Comparing `caosdb-0.8.0/src/caosdb/common/datatype.py` & `caosdb-0.9.0/src/caosdb/common/datatype.py`

 * *Files identical despite different names*

### Comparing `caosdb-0.8.0/src/caosdb/common/models.py` & `caosdb-0.9.0/src/caosdb/common/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 from tempfile import NamedTemporaryFile
 from warnings import warn
 
 from caosdb.common.datatype import (BOOLEAN, DATETIME, DOUBLE, INTEGER, TEXT,
                                     is_list_datatype, is_reference)
 from caosdb.common.state import State
 from caosdb.common.utils import uuid, xml2str
+from caosdb.common.timezone import TimeZone
 from caosdb.common.versioning import Version
 from caosdb.configuration import get_config
 from caosdb.connection.connection import get_connection
 from caosdb.connection.encode import MultipartParam, multipart_encode
 from caosdb.exceptions import (AmbiguousEntityError, AuthorizationError,
                                CaosDBConnectionError, CaosDBException,
                                ConsistencyError, EmptyUniqueQueryError,
@@ -4323,14 +4324,16 @@
         xml = etree.fromstring(http_response.read())
 
         for e in xml:
             m = _parse_single_xml_element(e)
 
             if isinstance(m, UserInfo):
                 self.user_info = m
+            elif isinstance(m, TimeZone):
+                self.time_zone = m
             else:
                 self.messages.append(m)
 
     def __str__(self):
         if "counts" not in self.messages:
             return "caosdb.Info"
 
@@ -4456,14 +4459,17 @@
         return Message(type="Counts", body=counts.attrib)
     elif elem.tag == "EntityACL":
         return ACL(xml=elem)
     elif elem.tag == "Permissions":
         return Permissions(xml=elem)
     elif elem.tag == "UserInfo":
         return UserInfo(xml=elem)
+    elif elem.tag == "TimeZone":
+        return TimeZone(zone_id=elem.get("id"), offset=elem.get("offset"),
+                        display_name=elem.text.strip())
     else:
         return Message(type=elem.tag, code=elem.get(
             "code"), description=elem.get("description"), body=elem.text)
 
 
 def _evaluate_and_add_error(parent_error, ent):
     """Evaluate the error message(s) attached to entity and add a
```

### Comparing `caosdb-0.8.0/src/caosdb/common/state.py` & `caosdb-0.9.0/src/caosdb/common/state.py`

 * *Files identical despite different names*

### Comparing `caosdb-0.8.0/src/caosdb/common/utils.py` & `caosdb-0.9.0/src/caosdb/common/utils.py`

 * *Files identical despite different names*

### Comparing `caosdb-0.8.0/src/caosdb/common/versioning.py` & `caosdb-0.9.0/src/caosdb/common/versioning.py`

 * *Files identical despite different names*

### Comparing `caosdb-0.8.0/src/caosdb/configuration.py` & `caosdb-0.9.0/src/caosdb/configuration.py`

 * *Files identical despite different names*

### Comparing `caosdb-0.8.0/src/caosdb/connection/authentication/auth_token.py` & `caosdb-0.9.0/src/caosdb/connection/authentication/auth_token.py`

 * *Files identical despite different names*

### Comparing `caosdb-0.8.0/src/caosdb/connection/authentication/external_credentials_provider.py` & `caosdb-0.9.0/src/caosdb/connection/authentication/external_credentials_provider.py`

 * *Files identical despite different names*

### Comparing `caosdb-0.8.0/src/caosdb/connection/authentication/input.py` & `caosdb-0.9.0/src/caosdb/connection/authentication/input.py`

 * *Files identical despite different names*

### Comparing `caosdb-0.8.0/src/caosdb/connection/authentication/interface.py` & `caosdb-0.9.0/src/caosdb/connection/authentication/interface.py`

 * *Files identical despite different names*

### Comparing `caosdb-0.8.0/src/caosdb/connection/authentication/keyring.py` & `caosdb-0.9.0/src/caosdb/connection/authentication/keyring.py`

 * *Files identical despite different names*

### Comparing `caosdb-0.8.0/src/caosdb/connection/authentication/pass.py` & `caosdb-0.9.0/src/caosdb/connection/authentication/pass.py`

 * *Files identical despite different names*

### Comparing `caosdb-0.8.0/src/caosdb/connection/authentication/plain.py` & `caosdb-0.9.0/src/caosdb/connection/authentication/plain.py`

 * *Files identical despite different names*

### Comparing `caosdb-0.8.0/src/caosdb/connection/authentication/unauthenticated.py` & `caosdb-0.9.0/src/caosdb/connection/authentication/unauthenticated.py`

 * *Files identical despite different names*

### Comparing `caosdb-0.8.0/src/caosdb/connection/connection.py` & `caosdb-0.9.0/src/caosdb/connection/connection.py`

 * *Files identical despite different names*

### Comparing `caosdb-0.8.0/src/caosdb/connection/encode.py` & `caosdb-0.9.0/src/caosdb/connection/encode.py`

 * *Files identical despite different names*

### Comparing `caosdb-0.8.0/src/caosdb/connection/interface.py` & `caosdb-0.9.0/src/caosdb/connection/interface.py`

 * *Files identical despite different names*

### Comparing `caosdb-0.8.0/src/caosdb/connection/mockup.py` & `caosdb-0.9.0/src/caosdb/connection/mockup.py`

 * *Files identical despite different names*

### Comparing `caosdb-0.8.0/src/caosdb/connection/streaminghttp.py` & `caosdb-0.9.0/src/caosdb/connection/streaminghttp.py`

 * *Files identical despite different names*

### Comparing `caosdb-0.8.0/src/caosdb/connection/utils.py` & `caosdb-0.9.0/src/caosdb/connection/utils.py`

 * *Files identical despite different names*

### Comparing `caosdb-0.8.0/src/caosdb/exceptions.py` & `caosdb-0.9.0/src/caosdb/exceptions.py`

 * *Files identical despite different names*

### Comparing `caosdb-0.8.0/src/caosdb/high_level_api.py` & `caosdb-0.9.0/src/caosdb/high_level_api.py`

 * *Files identical despite different names*

### Comparing `caosdb-0.8.0/src/caosdb/schema-pycaosdb-ini.yml` & `caosdb-0.9.0/src/caosdb/schema-pycaosdb-ini.yml`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
           type: string
           description: User name used for authentication with the server
           examples: [admin]
         password_method:
           description: The password input method defines how the password is supplied that is used for authentication with the server.
           type: string
           default: input
-          enum: [input, plain, pass, keyring]
+          enum: [input, unauthenticated, plain, pass, keyring]
         password_identifier:
           type: string
         password:
           type: string
           examples: [caosdb]
         auth_token:
           type: string
```

### Comparing `caosdb-0.8.0/src/caosdb/utils/caosdb_admin.py` & `caosdb-0.9.0/src/caosdb/utils/caosdb_admin.py`

 * *Files identical despite different names*

### Comparing `caosdb-0.8.0/src/caosdb/utils/checkFileSystemConsistency.py` & `caosdb-0.9.0/src/caosdb/utils/checkFileSystemConsistency.py`

 * *Files identical despite different names*

### Comparing `caosdb-0.8.0/src/caosdb/utils/create_revision.py` & `caosdb-0.9.0/src/caosdb/utils/create_revision.py`

 * *Files identical despite different names*

### Comparing `caosdb-0.8.0/src/caosdb/utils/plantuml.py` & `caosdb-0.9.0/src/caosdb/utils/plantuml.py`

 * *Files identical despite different names*

### Comparing `caosdb-0.8.0/src/caosdb/utils/server_side_scripting.py` & `caosdb-0.9.0/src/caosdb/utils/server_side_scripting.py`

 * *Files identical despite different names*

### Comparing `caosdb-0.8.0/src/caosdb/yamlapi.py` & `caosdb-0.9.0/src/caosdb/yamlapi.py`

 * *Files identical despite different names*

### Comparing `caosdb-0.8.0/src/caosdb.egg-info/PKG-INFO` & `caosdb-0.9.0/src/caosdb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: caosdb
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python Interface for CaosDB
 Home-page: https://www.caosdb.org
 Author: Timm Fitschen
 Author-email: t.fitschen@indiscale.com
 License: AGPLv3+
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -63,13 +62,11 @@
   CaosDB community on
   [#caosdb:matrix.org](https://matrix.to/#/!unwwlTfOznjEnMMXxf:matrix.org).
 
 ## License
 
 * Copyright (C) 2018 Research Group Biomedical Physics, Max Planck Institute
   for Dynamics and Self-Organization Göttingen.
-* Copyright (C) 2020-2021 Indiscale GmbH <info@indiscale.com>
+* Copyright (C) 2020-2022 Indiscale GmbH <info@indiscale.com>
 
 All files in this repository are licensed under a [GNU Affero General Public
 License](LICENCE.md) (version 3 or later).
-
-
```

