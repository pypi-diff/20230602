# Comparing `tmp/ebi_eva_common_pyutils-0.5.5.tar.gz` & `tmp/ebi_eva_common_pyutils-0.5.5.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebi_eva_common_pyutils-0.5.5.tar", last modified: Fri Jun  2 16:14:45 2023, max compression
+gzip compressed data, was "ebi_eva_common_pyutils-0.5.5.dev0.tar", last modified: Wed May 31 09:49:36 2023, max compression
```

## Comparing `ebi_eva_common_pyutils-0.5.5.tar` & `ebi_eva_common_pyutils-0.5.5.dev0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-06-02 16:14:45.687260 ebi_eva_common_pyutils-0.5.5/
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1706 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/CHANGELOG.md
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)    11357 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/LICENSE
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)       28 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/MANIFEST.in
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      540 2023-06-02 16:14:45.687260 ebi_eva_common_pyutils-0.5.5/PKG-INFO
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1434 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/README.md
-drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-06-02 16:14:45.683261 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)        0 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/__init__.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     4984 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/archive_directory.py
-drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-06-02 16:14:45.683261 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/assembly/
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)       66 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/assembly/__init__.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1570 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/assembly/assembly.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     2151 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/command_utils.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1192 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/common_utils.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     2242 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/config.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     7952 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/config_utils.py
-drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-06-02 16:14:45.683261 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/contig_alias/
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)        0 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/contig_alias/__init__.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     3056 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/contig_alias/contig_alias.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1452 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/ena_utils.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1375 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/file_utils.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     4990 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/logger.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)    14953 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/metadata_utils.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     3573 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/mongo_utils.py
-drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-06-02 16:14:45.683261 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/mongodb/
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)       72 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/mongodb/__init__.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     9676 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/mongodb/mongo_database.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     4859 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/ncbi_utils.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     2285 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/network_utils.py
-drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-06-02 16:14:45.683261 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/nextflow/
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      120 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/nextflow/__init__.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)    10114 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/nextflow/nextflow_pipeline.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     4398 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/pg_utils.py
-drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-06-02 16:14:45.683261 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/reference/
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      134 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/reference/__init__.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)    12162 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/reference/assembly.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     3911 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/reference/sequence.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)    14666 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/spring_properties.py
-drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-06-02 16:14:45.687260 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/taxonomy/
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)        0 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/taxonomy/__init__.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     2259 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/taxonomy/taxonomy.py
-drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-06-02 16:14:45.687260 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/variation/
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)        0 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/variation/__init__.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     3515 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/variation/assembly_utils.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     5230 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/variation/contig_utils.py
-drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-06-02 16:14:45.683261 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils.egg-info/
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      540 2023-06-02 16:14:45.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils.egg-info/PKG-INFO
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1703 2023-06-02 16:14:45.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils.egg-info/SOURCES.txt
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)        1 2023-06-02 16:14:45.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils.egg-info/dependency_links.txt
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)       81 2023-06-02 16:14:45.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils.egg-info/requires.txt
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)       23 2023-06-02 16:14:45.000000 ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils.egg-info/top_level.txt
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      225 2023-06-02 16:14:45.687260 ebi_eva_common_pyutils-0.5.5/setup.cfg
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      907 2023-06-02 16:14:44.000000 ebi_eva_common_pyutils-0.5.5/setup.py
+drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-05-31 09:49:36.015066 ebi_eva_common_pyutils-0.5.5.dev0/
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1706 2023-05-31 08:16:27.000000 ebi_eva_common_pyutils-0.5.5.dev0/CHANGELOG.md
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)    11357 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/LICENSE
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)       28 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/MANIFEST.in
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      545 2023-05-31 09:49:36.015066 ebi_eva_common_pyutils-0.5.5.dev0/PKG-INFO
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1434 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/README.md
+drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-05-31 09:49:36.011066 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)        0 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/__init__.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     4984 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/archive_directory.py
+drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-05-31 09:49:36.015066 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/assembly/
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)       66 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/assembly/__init__.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1570 2023-05-31 08:16:27.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/assembly/assembly.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     2151 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/command_utils.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1192 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/common_utils.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     2242 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/config.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     7960 2023-05-31 08:27:23.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/config_utils.py
+drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-05-31 09:49:36.015066 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/contig_alias/
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)        0 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/contig_alias/__init__.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     3056 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/contig_alias/contig_alias.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1452 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/ena_utils.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1375 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/file_utils.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     4990 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/logger.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)    14953 2023-05-31 08:16:27.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/metadata_utils.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     3573 2023-05-31 08:27:23.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/mongo_utils.py
+drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-05-31 09:49:36.015066 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/mongodb/
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)       72 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/mongodb/__init__.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     9676 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/mongodb/mongo_database.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     4859 2023-05-31 08:16:27.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/ncbi_utils.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     2285 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/network_utils.py
+drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-05-31 09:49:36.015066 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/nextflow/
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      120 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/nextflow/__init__.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)    10114 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/nextflow/nextflow_pipeline.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     4398 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/pg_utils.py
+drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-05-31 09:49:36.015066 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/reference/
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      134 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/reference/__init__.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)    12162 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/reference/assembly.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     3911 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/reference/sequence.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)    14666 2023-05-31 09:14:28.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/spring_properties.py
+drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-05-31 09:49:36.015066 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/taxonomy/
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)        0 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/taxonomy/__init__.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     2259 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/taxonomy/taxonomy.py
+drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-05-31 09:49:36.015066 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/variation/
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)        0 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/variation/__init__.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     3515 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/variation/assembly_utils.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     5230 2023-05-31 08:16:14.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/variation/contig_utils.py
+drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-05-31 09:49:36.011066 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils.egg-info/
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      545 2023-05-31 09:49:34.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils.egg-info/PKG-INFO
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1702 2023-05-31 09:49:34.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils.egg-info/SOURCES.txt
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)        1 2023-05-31 09:49:34.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils.egg-info/dependency_links.txt
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)       81 2023-05-31 09:49:34.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils.egg-info/requires.txt
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)       23 2023-05-31 09:49:34.000000 ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils.egg-info/top_level.txt
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      225 2023-05-31 09:49:36.019066 ebi_eva_common_pyutils-0.5.5.dev0/setup.cfg
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      911 2023-05-31 09:18:33.000000 ebi_eva_common_pyutils-0.5.5.dev0/setup.py
```

### Comparing `ebi_eva_common_pyutils-0.5.5/CHANGELOG.md` & `ebi_eva_common_pyutils-0.5.5.dev0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.5/LICENSE` & `ebi_eva_common_pyutils-0.5.5.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.5/PKG-INFO` & `ebi_eva_common_pyutils-0.5.5.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebi_eva_common_pyutils
-Version: 0.5.5
+Version: 0.5.5.dev0
 Summary: EBI EVA - Common Python Utilities
 Home-page: https://github.com/EBIVariation/eva-common-pyutils
 License: Apache
 Keywords: EBI,EVA,PYTHON,UTILITIES
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `ebi_eva_common_pyutils-0.5.5/README.md` & `ebi_eva_common_pyutils-0.5.5.dev0/README.md`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/archive_directory.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/archive_directory.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/assembly/assembly.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/assembly/assembly.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/command_utils.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/common_utils.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/common_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/config.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/config.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/config_utils.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/config_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     pg_user = properties['eva.evapro.user']
     pg_pass = properties['eva.evapro.password']
     return pg_url, pg_user, pg_pass
 
 
 def get_mongo_creds_for_profile(profile_name: str, settings_xml_file: str):
     """
-    Gets host, username, and password for mongo database.
+    Gets primary host, username, and password for mongo database.
     Useful for filling properties files, for connection purposes it is preferable to use
     `mongo_utils.get_mongo_connection_handle` as that will handle multiple hosts appropriately.
     """
     properties = get_properties_from_xml_file(profile_name, settings_xml_file)
     mongo_host = properties['eva.mongo.host']
     mongo_user = properties['eva.mongo.user']
     mongo_pass = properties['eva.mongo.passwd']
```

### Comparing `ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/contig_alias/contig_alias.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/contig_alias/contig_alias.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/ena_utils.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/ena_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/file_utils.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/file_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/logger.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/logger.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/metadata_utils.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/mongo_utils.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/mongo_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/mongodb/mongo_database.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/mongodb/mongo_database.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/ncbi_utils.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/ncbi_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/network_utils.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/network_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/nextflow/nextflow_pipeline.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/nextflow/nextflow_pipeline.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/pg_utils.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/pg_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/reference/assembly.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/reference/assembly.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/reference/sequence.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/reference/sequence.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/spring_properties.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/spring_properties.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/taxonomy/taxonomy.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/taxonomy/taxonomy.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/variation/assembly_utils.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/variation/assembly_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils/variation/contig_utils.py` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils/variation/contig_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils.egg-info/PKG-INFO` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebi-eva-common-pyutils
-Version: 0.5.5
+Version: 0.5.5.dev0
 Summary: EBI EVA - Common Python Utilities
 Home-page: https://github.com/EBIVariation/eva-common-pyutils
 License: Apache
 Keywords: EBI,EVA,PYTHON,UTILITIES
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `ebi_eva_common_pyutils-0.5.5/ebi_eva_common_pyutils.egg-info/SOURCES.txt` & `ebi_eva_common_pyutils-0.5.5.dev0/ebi_eva_common_pyutils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
-/tmp/ebi_eva_common_pyutils-v0.5.5-baxfx66g/gitclone/ebi_eva_common_pyutils/archive_directory.py
+/data/sundarvenkata_work/EVA3253/eva-common-pyutils/ebi_eva_common_pyutils/archive_directory.py
 ebi_eva_common_pyutils/__init__.py
 ebi_eva_common_pyutils/archive_directory.py
 ebi_eva_common_pyutils/command_utils.py
 ebi_eva_common_pyutils/common_utils.py
 ebi_eva_common_pyutils/config.py
 ebi_eva_common_pyutils/config_utils.py
 ebi_eva_common_pyutils/ena_utils.py
```

### Comparing `ebi_eva_common_pyutils-0.5.5/setup.py` & `ebi_eva_common_pyutils-0.5.5.dev0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import find_packages
 
 setup(
     name='ebi_eva_common_pyutils',
     scripts=[os.path.join(os.path.dirname(__file__), 'ebi_eva_common_pyutils', 'archive_directory.py')],
     packages=find_packages(),
-    version='0.5.5',
+    version='0.5.5-dev',
     license='Apache',
     description='EBI EVA - Common Python Utilities',
     url='https://github.com/EBIVariation/eva-common-pyutils',
     keywords=['EBI', 'EVA', 'PYTHON', 'UTILITIES'],
     install_requires=['psycopg2-binary', 'requests', 'pymongo', 'lxml', 'pyyaml', 'cached-property', 'retry',
                       'networkx<=2.5'],
     classifiers=[
```

