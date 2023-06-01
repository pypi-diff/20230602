# Comparing `tmp/mssql-django-1.2.tar.gz` & `tmp/mssql-django-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mssql-django-1.2.tar", last modified: Thu Dec  8 23:07:28 2022, max compression
+gzip compressed data, was "mssql-django-1.3.tar", last modified: Thu Jun  1 21:00:14 2023, max compression
```

## Comparing `mssql-django-1.2.tar` & `mssql-django-1.3.tar`

### file list

```diff
@@ -1,74 +1,76 @@
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2022-12-08 23:07:28.872338 mssql-django-1.2/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1673 2022-12-08 23:07:13.000000 mssql-django-1.2/LICENSE.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      114 2022-12-08 23:07:13.000000 mssql-django-1.2/MANIFEST.in
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1791 2022-12-08 23:07:13.000000 mssql-django-1.2/NOTICE.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11596 2022-12-08 23:07:28.872338 mssql-django-1.2/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10594 2022-12-08 23:07:13.000000 mssql-django-1.2/README.md
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2022-12-08 23:07:28.864338 mssql-django-1.2/mssql/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      105 2022-12-08 23:07:13.000000 mssql-django-1.2/mssql/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    25598 2022-12-08 23:07:13.000000 mssql-django-1.2/mssql/base.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1926 2022-12-08 23:07:13.000000 mssql-django-1.2/mssql/client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    27461 2022-12-08 23:07:13.000000 mssql-django-1.2/mssql/compiler.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4554 2022-12-08 23:07:13.000000 mssql-django-1.2/mssql/creation.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2699 2022-12-08 23:07:13.000000 mssql-django-1.2/mssql/features.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    19206 2022-12-08 23:07:13.000000 mssql-django-1.2/mssql/functions.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    16597 2022-12-08 23:07:13.000000 mssql-django-1.2/mssql/introspection.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2022-12-08 23:07:28.864338 mssql-django-1.2/mssql/management/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2022-12-08 23:07:13.000000 mssql-django-1.2/mssql/management/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2022-12-08 23:07:28.864338 mssql-django-1.2/mssql/management/commands/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2022-12-08 23:07:13.000000 mssql-django-1.2/mssql/management/commands/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      656 2022-12-08 23:07:13.000000 mssql-django-1.2/mssql/management/commands/inspectdb.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      850 2022-12-08 23:07:13.000000 mssql-django-1.2/mssql/management/commands/install_regex_clr.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    28254 2022-12-08 23:07:13.000000 mssql-django-1.2/mssql/operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4608 2022-03-02 21:19:22.000000 mssql-django-1.2/mssql/regex_clr.dll
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    66233 2022-12-08 23:07:13.000000 mssql-django-1.2/mssql/schema.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2022-12-08 23:07:28.864338 mssql-django-1.2/mssql_django.egg-info/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11596 2022-12-08 23:07:28.000000 mssql-django-1.2/mssql_django.egg-info/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2286 2022-12-08 23:07:28.000000 mssql-django-1.2/mssql_django.egg-info/SOURCES.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2022-12-08 23:07:28.000000 mssql-django-1.2/mssql_django.egg-info/dependency_links.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       34 2022-12-08 23:07:28.000000 mssql-django-1.2/mssql_django.egg-info/requires.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       14 2022-12-08 23:07:28.000000 mssql-django-1.2/mssql_django.egg-info/top_level.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      122 2022-12-08 23:07:28.872338 mssql-django-1.2/setup.cfg
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1513 2022-12-08 23:07:13.000000 mssql-django-1.2/setup.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2022-12-08 23:07:28.864338 mssql-django-1.2/testapp/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2022-12-08 23:07:28.868338 mssql-django-1.2/testapp/migrations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2392 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/migrations/0001_initial.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      772 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/migrations/0002_test_unique_nullable_part1.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      810 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/migrations/0003_test_unique_nullable_part2.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1023 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/migrations/0004_test_unique_type_change_part1.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1407 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/migrations/0005_test_unique_type_change_part2.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      743 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/migrations/0006_test_remove_onetoone_field_part1.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      376 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/migrations/0007_test_remove_onetoone_field_part2.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      584 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/migrations/0008_test_drop_table_with_foreign_key_reference_part1.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      477 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/migrations/0009_test_drop_table_with_foreign_key_reference_part2.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      761 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/migrations/0010_pizza_topping.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2380 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/migrations/0011_test_unique_constraints.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      678 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/migrations/0012_test_indexes_retained_part1.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      797 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/migrations/0013_test_indexes_retained_part2.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      887 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/migrations/0014_test_rename_m2mfield_part1.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      597 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/migrations/0015_test_rename_m2mfield_part2.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      774 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/migrations/0016_jsonmodel.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1335 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/migrations/0017_binarydata_testcheckconstraintwithunicode_and_more.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1252 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/migrations/0018_choice_question.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1161 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/migrations/0019_customer_name_customer_address.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      418 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/migrations/0020_autofield_to_bigautofield.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      790 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/migrations/0021_multiple_autofield_to_bigauto.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      579 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/migrations/0022_timezone.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      703 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/migrations/0023_number.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/migrations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7601 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/models.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1390 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/runners.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    17098 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/settings.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2022-12-08 23:07:28.872338 mssql-django-1.2/testapp/tests/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      461 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/tests/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      868 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/tests/test_bitshift.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11269 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/tests/test_constraints.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3137 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/tests/test_expressions.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1324 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/tests/test_fields.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9762 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/tests/test_indexes.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2008 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/tests/test_jsonfield.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      484 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/tests/test_lookups.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3679 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/tests/test_multiple_databases.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1101 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/tests/test_queries.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4172 2022-12-08 23:07:13.000000 mssql-django-1.2/testapp/tests/test_timezones.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-06-01 21:00:14.745409 mssql-django-1.3/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1673 2023-06-01 21:00:01.000000 mssql-django-1.3/LICENSE.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      114 2023-06-01 21:00:01.000000 mssql-django-1.3/MANIFEST.in
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1791 2023-06-01 21:00:01.000000 mssql-django-1.3/NOTICE.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11651 2023-06-01 21:00:14.745409 mssql-django-1.3/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10610 2023-06-01 21:00:01.000000 mssql-django-1.3/README.md
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-06-01 21:00:14.737409 mssql-django-1.3/mssql/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      105 2023-06-01 21:00:01.000000 mssql-django-1.3/mssql/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    25669 2023-06-01 21:00:01.000000 mssql-django-1.3/mssql/base.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1926 2023-06-01 21:00:01.000000 mssql-django-1.3/mssql/client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    28291 2023-06-01 21:00:01.000000 mssql-django-1.3/mssql/compiler.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4554 2023-06-01 21:00:01.000000 mssql-django-1.3/mssql/creation.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2741 2023-06-01 21:00:01.000000 mssql-django-1.3/mssql/features.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    20148 2023-06-01 21:00:01.000000 mssql-django-1.3/mssql/functions.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    16597 2023-06-01 21:00:01.000000 mssql-django-1.3/mssql/introspection.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-06-01 21:00:14.737409 mssql-django-1.3/mssql/management/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2023-06-01 21:00:01.000000 mssql-django-1.3/mssql/management/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-06-01 21:00:14.737409 mssql-django-1.3/mssql/management/commands/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2023-06-01 21:00:01.000000 mssql-django-1.3/mssql/management/commands/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      656 2023-06-01 21:00:01.000000 mssql-django-1.3/mssql/management/commands/inspectdb.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      850 2023-06-01 21:00:01.000000 mssql-django-1.3/mssql/management/commands/install_regex_clr.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    28404 2023-06-01 21:00:01.000000 mssql-django-1.3/mssql/operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4608 2022-03-02 21:19:22.000000 mssql-django-1.3/mssql/regex_clr.dll
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    67327 2023-06-01 21:00:01.000000 mssql-django-1.3/mssql/schema.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-06-01 21:00:14.737409 mssql-django-1.3/mssql_django.egg-info/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11651 2023-06-01 21:00:14.000000 mssql-django-1.3/mssql_django.egg-info/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2362 2023-06-01 21:00:14.000000 mssql-django-1.3/mssql_django.egg-info/SOURCES.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2023-06-01 21:00:14.000000 mssql-django-1.3/mssql_django.egg-info/dependency_links.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       34 2023-06-01 21:00:14.000000 mssql-django-1.3/mssql_django.egg-info/requires.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       14 2023-06-01 21:00:14.000000 mssql-django-1.3/mssql_django.egg-info/top_level.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      122 2023-06-01 21:00:14.745409 mssql-django-1.3/setup.cfg
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1547 2023-06-01 21:00:01.000000 mssql-django-1.3/setup.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-06-01 21:00:14.737409 mssql-django-1.3/testapp/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-06-01 21:00:14.745409 mssql-django-1.3/testapp/migrations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2392 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/migrations/0001_initial.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      772 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/migrations/0002_test_unique_nullable_part1.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      810 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/migrations/0003_test_unique_nullable_part2.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1023 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/migrations/0004_test_unique_type_change_part1.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1407 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/migrations/0005_test_unique_type_change_part2.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      743 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/migrations/0006_test_remove_onetoone_field_part1.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      376 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/migrations/0007_test_remove_onetoone_field_part2.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      584 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/migrations/0008_test_drop_table_with_foreign_key_reference_part1.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      477 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/migrations/0009_test_drop_table_with_foreign_key_reference_part2.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      761 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/migrations/0010_pizza_topping.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2380 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/migrations/0011_test_unique_constraints.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      678 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/migrations/0012_test_indexes_retained_part1.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      797 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/migrations/0013_test_indexes_retained_part2.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      887 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/migrations/0014_test_rename_m2mfield_part1.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      597 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/migrations/0015_test_rename_m2mfield_part2.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      774 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/migrations/0016_jsonmodel.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1335 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/migrations/0017_binarydata_testcheckconstraintwithunicode_and_more.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1252 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/migrations/0018_choice_question.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1161 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/migrations/0019_customer_name_customer_address.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      418 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/migrations/0020_autofield_to_bigautofield.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      790 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/migrations/0021_multiple_autofield_to_bigauto.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      579 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/migrations/0022_timezone.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      703 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/migrations/0023_number.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1744 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/migrations/0024_publisher_book.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/migrations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8022 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/models.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1390 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/runners.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    17526 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/settings.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-06-01 21:00:14.745409 mssql-django-1.3/testapp/tests/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      461 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/tests/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      868 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/tests/test_bitshift.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11269 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/tests/test_constraints.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3137 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/tests/test_expressions.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1324 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/tests/test_fields.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1739 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/tests/test_getorcreate.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9762 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/tests/test_indexes.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2008 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/tests/test_jsonfield.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      484 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/tests/test_lookups.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3679 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/tests/test_multiple_databases.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1101 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/tests/test_queries.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4172 2023-06-01 21:00:01.000000 mssql-django-1.3/testapp/tests/test_timezones.py
```

### Comparing `mssql-django-1.2/LICENSE.txt` & `mssql-django-1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/NOTICE.md` & `mssql-django-1.3/NOTICE.md`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/PKG-INFO` & `mssql-django-1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mssql-django
-Version: 1.2
+Version: 1.3
 Summary: Django backend for Microsoft SQL Server
 Home-page: https://github.com/microsoft/mssql-django
 Author: Microsoft
 Author-email: opencode@microsoft.com
 License: BSD
 Project-URL: Release Notes, https://github.com/microsoft/mssql-django/releases
 Keywords: django
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: NOTICE.md
 
 # SQL Server backend for Django
 
 Welcome to the MSSQL-Django 3rd party backend project!
@@ -33,16 +34,16 @@
 
 We'd like to give thanks to the community that made this project possible, with particular recognition of the contributors: OskarPersson, michiya, dlo and the original Google Code django-pyodbc team. Moving forward we encourage partipation in this project from both old and new contributors!
 
 We hope you enjoy using the MSSQL-Django 3rd party backend.
 
 ## Features
 
--  Supports Django 3.2 and 4.0
--  Tested on Microsoft SQL Server 2016, 2017, 2019
+-  Supports Django 3.2, 4.0, 4.1 and 4.2
+-  Tested on Microsoft SQL Server 2016, 2017, 2019, 2022
 -  Passes most of the tests of the Django test suite
 -  Compatible with
    [Micosoft ODBC Driver for SQL Server](https://docs.microsoft.com/en-us/sql/connect/odbc/microsoft-odbc-driver-for-sql-server),
    [SQL Server Native Client](https://msdn.microsoft.com/en-us/library/ms131321(v=sql.120).aspx),
    and [FreeTDS](https://www.freetds.org/) ODBC drivers
 
 ## Dependencies
```

### Comparing `mssql-django-1.2/README.md` & `mssql-django-1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 We'd like to give thanks to the community that made this project possible, with particular recognition of the contributors: OskarPersson, michiya, dlo and the original Google Code django-pyodbc team. Moving forward we encourage partipation in this project from both old and new contributors!
 
 We hope you enjoy using the MSSQL-Django 3rd party backend.
 
 ## Features
 
--  Supports Django 3.2 and 4.0
--  Tested on Microsoft SQL Server 2016, 2017, 2019
+-  Supports Django 3.2, 4.0, 4.1 and 4.2
+-  Tested on Microsoft SQL Server 2016, 2017, 2019, 2022
 -  Passes most of the tests of the Django test suite
 -  Compatible with
    [Micosoft ODBC Driver for SQL Server](https://docs.microsoft.com/en-us/sql/connect/odbc/microsoft-odbc-driver-for-sql-server),
    [SQL Server Native Client](https://msdn.microsoft.com/en-us/library/ms131321(v=sql.120).aspx),
    and [FreeTDS](https://www.freetds.org/) ODBC drivers
 
 ## Dependencies
```

### Comparing `mssql-django-1.2/mssql/base.py` & `mssql-django-1.3/mssql/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import os
 import re
 import time
 import struct
 import datetime
 
 from django.core.exceptions import ImproperlyConfigured
+from django.utils.functional import cached_property
 
 try:
     import pyodbc as Database
 except ImportError as e:
     raise ImproperlyConfigured("Error loading pyodbc module: %s" % e)
 
 from django.utils.version import get_version_tuple  # noqa
@@ -426,27 +427,28 @@
         cursor.execute('SET DATEFORMAT ymd; SET DATEFIRST %s' % datefirst)
 
         # Let user choose if driver can return rows from bulk insert since
         # inserting into tables with triggers causes errors. See issue #130
         if (options.get('return_rows_bulk_insert', False)):
             self.features_class.can_return_rows_from_bulk_insert = True
 
-        val = self.get_system_datetime()
+        val = self.get_system_datetime
         if isinstance(val, str):
             raise ImproperlyConfigured(
                 "The database driver doesn't support modern datatime types.")
 
     def is_usable(self):
         try:
             self.create_cursor().execute("SELECT 1")
         except Database.Error:
             return False
         else:
             return True
 
+    @cached_property
     def get_system_datetime(self):
         # http://blogs.msdn.com/b/sqlnativeclient/archive/2008/02/27/microsoft-sql-server-native-client-and-microsoft-sql-server-2008-native-client.aspx
         with self.temporary_connection() as cursor:
             if self.sql_server_version <= 2005:
                 return cursor.execute('SELECT GETDATE()').fetchone()[0]
             else:
                 return cursor.execute('SELECT SYSDATETIME()').fetchone()[0]
```

### Comparing `mssql-django-1.2/mssql/client.py` & `mssql-django-1.3/mssql/client.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/mssql/compiler.py` & `mssql-django-1.3/mssql/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     Chr, ConcatPair, Greatest, Least, Length, LPad, Random, Repeat, RPad, StrIndex, Substr, Trim
 )
 from django.db.models.sql import compiler
 from django.db.transaction import TransactionManagementError
 from django.db.utils import NotSupportedError
 if django.VERSION >= (3, 1):
     from django.db.models.fields.json import compile_json_path, KeyTransform as json_KeyTransform
+if django.VERSION >= (4, 2):
+    from django.core.exceptions import FullResultSet
 
 def _as_sql_agv(self, compiler, connection):
     return self.as_sql(compiler, connection, template='%(function)s(CONVERT(float, %(field)s))')
 
 
 def _as_sql_chr(self, compiler, connection):
     return self.as_sql(compiler, connection, function='NCHAR')
@@ -72,16 +74,17 @@
     params.extend(fill_text_arg)
     params.extend(length_arg)
     params.extend(length_arg)
     params.extend(expression_arg)
     params.extend(length_arg)
     params.extend(expression_arg)
     params.extend(expression_arg)
-    template = ('LEFT(REPLICATE(%(fill_text)s, %(length)s), CASE WHEN %(length)s > LEN(%(expression)s) '
-                'THEN %(length)s - LEN(%(expression)s) ELSE 0 END) + %(expression)s')
+    params.extend(length_arg)
+    template = ('LEFT(LEFT(REPLICATE(%(fill_text)s, %(length)s), CASE WHEN %(length)s > LEN(%(expression)s) '
+                'THEN %(length)s - LEN(%(expression)s) ELSE 0 END) + %(expression)s, %(length)s)')
     return template % {'expression': expression, 'length': length, 'fill_text': fill_text}, params
 
 
 def _as_sql_repeat(self, compiler, connection):
     return self.as_sql(compiler, connection, function='REPLICATE')
 
 
@@ -223,21 +226,34 @@
             supports_offset_clause = self.connection.sql_server_version >= 2012
             do_offset_emulation = do_offset and not supports_offset_clause
 
             if combinator:
                 if not getattr(features, 'supports_select_{}'.format(combinator)):
                     raise NotSupportedError('{} is not supported on this database backend.'.format(combinator))
                 result, params = self.get_combinator_sql(combinator, self.query.combinator_all)
+            elif django.VERSION >= (4, 2) and self.qualify:
+                result, params = self.get_qualify_sql()
+                order_by = None
             else:
                 distinct_fields, distinct_params = self.get_distinct()
                 # This must come after 'select', 'ordering', and 'distinct' -- see
                 # docstring of get_from_clause() for details.
                 from_, f_params = self.get_from_clause()
-                where, w_params = self.compile(self.where) if self.where is not None else ("", [])
-                having, h_params = self.compile(self.having) if self.having is not None else ("", [])
+                if django.VERSION >= (4, 2):
+                    try:
+                        where, w_params = self.compile(self.where) if self.where is not None else ("", [])
+                    except FullResultSet:
+                        where, w_params = "", []
+                    try:
+                        having, h_params = self.compile(self.having) if self.having is not None else ("", [])
+                    except FullResultSet:
+                        having, h_params = "", []
+                else:
+                    where, w_params = self.compile(self.where) if self.where is not None else ("", [])
+                    having, h_params = self.compile(self.having) if self.having is not None else ("", [])
                 params = []
                 result = ['SELECT']
 
                 if self.query.distinct:
                     distinct_result, distinct_params = self.connection.ops.distinct_sql(
                         distinct_fields,
                         distinct_params,
@@ -360,15 +376,15 @@
                 result.append('ORDER BY %s' % ', '.join(ordering))
 
                 # For subqueres with an ORDER BY clause, SQL Server also
                 # requires a TOP or OFFSET clause which is not generated for
                 # Django 2.x.  See https://github.com/microsoft/mssql-django/issues/12
                 # Add OFFSET for all Django versions.
                 # https://github.com/microsoft/mssql-django/issues/109
-                if not (do_offset or do_limit):
+                if not (do_offset or do_limit) and supports_offset_clause:
                     result.append("OFFSET 0 ROWS")
 
             # SQL Server requires the backend-specific emulation (2008 or earlier)
             # or an offset clause (2012 or newer) for offsetting
             if do_offset:
                 if do_offset_emulation:
                     # Construct the final SQL clause, using the initial select SQL
```

### Comparing `mssql-django-1.2/mssql/creation.py` & `mssql-django-1.3/mssql/creation.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/mssql/features.py` & `mssql-django-1.3/mssql/features.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Licensed under the BSD license.
 
 from django.db.backends.base.features import BaseDatabaseFeatures
 from django.utils.functional import cached_property
 
 
 class DatabaseFeatures(BaseDatabaseFeatures):
+    allows_group_by_select_index = False
     allow_sliced_subqueries_with_in = False
     can_introspect_autofield = True
     can_introspect_json_field = False
     can_introspect_small_integer_field = True
     can_return_columns_from_insert = True
     can_return_id_from_insert = True
     can_return_rows_from_bulk_insert = False
@@ -67,8 +68,8 @@
         return self.connection.sql_server_version >= 2016 or self.connection.to_azure_sql_db
 
     @cached_property
     def introspected_field_types(self):
         return {
             **super().introspected_field_types,
             "DurationField": "BigIntegerField",
-        }
+        }
```

### Comparing `mssql-django-1.2/mssql/functions.py` & `mssql-django-1.3/mssql/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 from django import VERSION
 from django.core import validators
 from django.db import NotSupportedError, connections, transaction
 from django.db.models import BooleanField, CheckConstraint, Value
 from django.db.models.expressions import Case, Exists, Expression, OrderBy, When, Window
 from django.db.models.fields import BinaryField, Field
 from django.db.models.functions import Cast, NthValue, MD5, SHA1, SHA224, SHA256, SHA384, SHA512
+from django.db.models.functions.datetime import Now
 from django.db.models.functions.math import ATan2, Ln, Log, Mod, Round, Degrees, Radians, Power
+from django.db.models.functions.text import Replace
 from django.db.models.lookups import In, Lookup
 from django.db.models.query import QuerySet
 from django.db.models.sql.query import Query
 
 if VERSION >= (3, 1):
     from django.db.models.fields.json import (
         KeyTransform, KeyTransformIn, KeyTransformExact,
@@ -40,14 +42,27 @@
     clone.set_source_expressions(self.get_source_expressions()[::-1])
     return clone.as_sql(compiler, connection, **extra_context)
 
 
 def sqlserver_ln(self, compiler, connection, **extra_context):
     return self.as_sql(compiler, connection, function='LOG', **extra_context)
 
+
+def sqlserver_replace(self, compiler, connection, **extra_context):
+    current_db = "CONVERT(varchar, (SELECT DB_NAME()))"
+    with connection.cursor() as cursor:
+        cursor.execute("SELECT CONVERT(varchar, DATABASEPROPERTYEX(%s, 'collation'))" % current_db)
+        default_collation = cursor.fetchone()[0]
+    current_collation = default_collation.replace('_CI', '_CS')
+    return self.as_sql(
+            compiler, connection, function='REPLACE',
+            template = 'REPLACE(%s COLLATE %s)' % ('%(expressions)s', current_collation),
+            **extra_context
+        )
+
 def sqlserver_degrees(self, compiler, connection, **extra_context):
     return self.as_sql(
             compiler, connection, function='DEGREES',
             template= 'DEGREES(CONVERT(float, %(expressions)s))',
             **extra_context
         )
 
@@ -105,14 +120,18 @@
     # MS SQL doesn't allow EXISTS() in the SELECT list, so wrap it with a
     # CASE WHEN expression. Change the template since the When expression
     # requires a left hand side (column) to compare against.
     sql, params = self.as_sql(compiler, connection, template, **extra_context)
     sql = 'CASE WHEN {} THEN 1 ELSE 0 END'.format(sql)
     return sql, params
 
+def sqlserver_now(self, compiler, connection, **extra_context):
+        return self.as_sql(
+            compiler, connection, template="SYSDATETIME()", **extra_context
+        )
 
 def sqlserver_lookup(self, compiler, connection):
     # MSSQL doesn't allow EXISTS() to be compared to another expression
     # unless it's wrapped in a CASE WHEN.
     wrapped = False
     exprs = []
     for expr in (self.lhs, self.rhs):
@@ -269,15 +288,15 @@
     """
         Update the given fields in each of the given objects in the database.
 
         When bulk_update all fields to null,
         SQL Server require that at least one of the result expressions in a CASE specification must be an expression other than the NULL constant.
         Patched with a default value 0. The user can also pass a custom default value for CASE statement.
     """
-    if batch_size is not None and batch_size < 0:
+    if batch_size is not None and batch_size <= 0:
         raise ValueError('Batch size must be a positive integer.')
     if not fields:
         raise ValueError('Field names must be given to bulk_update().')
     objs = tuple(objs)
     if any(obj.pk is None for obj in objs):
         raise ValueError('All bulk_update() objects must have a primary key set.')
     fields = [self.model._meta.get_field(name) for name in fields]
@@ -437,14 +456,16 @@
 Power.as_microsoft = sqlserver_power
 Ln.as_microsoft = sqlserver_ln
 Log.as_microsoft = sqlserver_log
 Mod.as_microsoft = sqlserver_mod
 NthValue.as_microsoft = sqlserver_nth_value
 Round.as_microsoft = sqlserver_round
 Window.as_microsoft = sqlserver_window
+Replace.as_microsoft = sqlserver_replace
+Now.as_microsoft = sqlserver_now
 MD5.as_microsoft = sqlserver_md5
 SHA1.as_microsoft = sqlserver_sha1
 SHA224.as_microsoft = sqlserver_sha224
 SHA256.as_microsoft = sqlserver_sha256
 SHA384.as_microsoft = sqlserver_sha384
 SHA512.as_microsoft = sqlserver_sha512
 BinaryField.__init__ = BinaryField_init
```

### Comparing `mssql-django-1.2/mssql/introspection.py` & `mssql-django-1.3/mssql/introspection.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         of SQL_AUTOFIELD, which maps to the 'AutoField' value in the DATA_TYPES_REVERSE dict.
 
         When a bigint field is found with an IDENTITY property, it is given a custom field number
         of SQL_BIGAUTOFIELD, which maps to the 'BigAutoField' value in the DATA_TYPES_REVERSE dict.
         """
 
         # map pyodbc's cursor.columns to db-api cursor description
-        columns = [[c[3], c[4], None, c[6], c[6], c[8], c[10], c[12]] for c in cursor.columns(table=table_name)]
+        columns = [[c[3], c[4], c[6], c[6], c[6], c[8], c[10], c[12]] for c in cursor.columns(table=table_name)]
 
         if not columns:
             raise DatabaseError(f"Table {table_name} does not exist.")
             
         items = []
         for column in columns:
             if VERSION >= (3, 2):
```

### Comparing `mssql-django-1.2/mssql/management/commands/inspectdb.py` & `mssql-django-1.3/mssql/management/commands/inspectdb.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/mssql/management/commands/install_regex_clr.py` & `mssql-django-1.3/mssql/management/commands/install_regex_clr.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/mssql/operations.py` & `mssql-django-1.3/mssql/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -400,29 +400,35 @@
         match_option = {'iregex': 0, 'regex': 1}[lookup_type]
         return "dbo.REGEXP_LIKE(%%s, %%s, %s)=1" % (match_option,)
 
     def limit_offset_sql(self, low_mark, high_mark):
         """Return LIMIT/OFFSET SQL clause."""
         limit, offset = self._get_limit_offset_params(low_mark, high_mark)
         return '%s%s' % (
-            (' OFFSET %d ROWS' % offset) if offset else '',
+            (' OFFSET %d ROWS' % offset) if offset else ' OFFSET 0 ROWS',
             (' FETCH FIRST %d ROWS ONLY' % limit) if limit else '',
         )
 
     def last_executed_query(self, cursor, sql, params):
         """
         Returns a string of the query last executed by the given cursor, with
         placeholders replaced with actual values.
 
         `sql` is the raw query containing placeholders, and `params` is the
         sequence of parameters. These are used by default, but this method
         exists for database backends to provide a better implementation
         according to their own quoting schemes.
         """
-        return super().last_executed_query(cursor, cursor.last_sql, cursor.last_params)
+        if params:
+            if isinstance(params, list):
+                params = tuple(params)
+            return sql % params
+        # Just return sql when there are no parameters.
+        else:
+            return sql
 
     def savepoint_create_sql(self, sid):
         """
         Returns the SQL for starting a new savepoint. Only required if the
         "uses_savepoints" feature is True. The "sid" parameter is a string
         for the savepoint id.
         """
```

### Comparing `mssql-django-1.2/mssql/regex_clr.dll` & `mssql-django-1.3/mssql/regex_clr.dll`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/mssql/schema.py` & `mssql-django-1.3/mssql/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,17 +157,22 @@
                 sql % {
                     'column': self.quote_name(new_field.column),
                     'type': new_db_params['type'],
                 },
                 [],
             )
 
-    def _alter_column_type_sql(self, model, old_field, new_field, new_type):
-        new_type = self._set_field_new_type_null_status(old_field, new_type)
-        return super()._alter_column_type_sql(model, old_field, new_field, new_type)
+    if django_version >= (4, 2):
+        def _alter_column_type_sql(self, model, old_field, new_field, new_type, old_collation, new_collation):
+            new_type = self._set_field_new_type_null_status(old_field, new_type)
+            return super()._alter_column_type_sql(model, old_field, new_field, new_type, old_collation, new_collation)
+    else:
+        def _alter_column_type_sql(self, model, old_field, new_field, new_type):
+            new_type = self._set_field_new_type_null_status(old_field, new_type)
+            return super()._alter_column_type_sql(model, old_field, new_field, new_type)
 
     def alter_unique_together(self, model, old_unique_together, new_unique_together):
         """
         Deal with a model changing its unique_together. The input
         unique_togethers must be doubly-nested, not the single-nested
         ["foo", "bar"] format.
         """
@@ -439,15 +444,20 @@
 
         # Next, start accumulating actions to do
         actions = []
         null_actions = []
         post_actions = []
         # Type change?
         if old_type != new_type:
-            fragment, other_actions = self._alter_column_type_sql(model, old_field, new_field, new_type)
+            if django_version >= (4, 2):
+                fragment, other_actions = self._alter_column_type_sql(
+                    model, old_field, new_field, new_type, old_collation=None, new_collation=None
+                )
+            else:
+                fragment, other_actions =  self._alter_column_type_sql(model, old_field, new_field, new_type)
             actions.append(fragment)
             post_actions.extend(other_actions)
             # Drop unique constraint, SQL Server requires explicit deletion
             self._delete_unique_constraints(model, old_field, new_field, strict)
             # Drop indexes, SQL Server requires explicit deletion
             self._delete_indexes(model, old_field, new_field)
         # When changing a column NULL constraint to NOT NULL with a given
@@ -679,17 +689,22 @@
             )
             # Update all referencing columns
             rels_to_update.extend(_related_non_m2m_objects(old_field, new_field))
         # Handle our type alters on the other end of rels from the PK stuff above
         for old_rel, new_rel in rels_to_update:
             rel_db_params = new_rel.field.db_parameters(connection=self.connection)
             rel_type = rel_db_params['type']
-            fragment, other_actions = self._alter_column_type_sql(
-                new_rel.related_model, old_rel.field, new_rel.field, rel_type
-            )
+            if django_version >= (4, 2):
+                fragment, other_actions = self._alter_column_type_sql(
+                    new_rel.related_model, old_rel.field, new_rel.field, rel_type, old_collation=None, new_collation=None
+                )
+            else:
+                fragment, other_actions = self._alter_column_type_sql(
+                    new_rel.related_model, old_rel.field, new_rel.field, rel_type
+                )
             # Drop related_model indexes, so it can be altered
             index_names = self._db_table_constraint_names(old_rel.related_model._meta.db_table, index=True)
             for index_name in index_names:
                 self.execute(self._db_table_delete_constraint_sql(
                     self.sql_delete_index, old_rel.related_model._meta.db_table, index_name))
             self.execute(
                 self.sql_alter_column % {
@@ -1258,16 +1273,20 @@
 
     def add_constraint(self, model, constraint):
         if isinstance(constraint, UniqueConstraint) and constraint.condition and constraint.condition.connector != AND:
             raise NotImplementedError("The backend does not support %s conditions on unique constraint %s." %
                                       (constraint.condition.connector, constraint.name))
         super().add_constraint(model, constraint)
 
-    def _collate_sql(self, collation):
-        return ' COLLATE ' + collation
+    if django_version >= (4, 2):
+        def _collate_sql(self, collation, old_collation=None, table_name=None):
+            return ' COLLATE ' + collation if collation else ""
+    else:
+        def _collate_sql(self, collation):
+            return ' COLLATE ' + collation
 
     def _create_index_name(self, table_name, column_names, suffix=""):
         index_name = super()._create_index_name(table_name, column_names, suffix)
         # Check if the db_table specified a user-defined schema
         if('].[' in index_name):
             new_index_name = index_name.replace('[', '').replace(']', '').replace('.', '_')
             return new_index_name
```

### Comparing `mssql-django-1.2/mssql_django.egg-info/PKG-INFO` & `mssql-django-1.3/mssql_django.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mssql-django
-Version: 1.2
+Version: 1.3
 Summary: Django backend for Microsoft SQL Server
 Home-page: https://github.com/microsoft/mssql-django
 Author: Microsoft
 Author-email: opencode@microsoft.com
 License: BSD
 Project-URL: Release Notes, https://github.com/microsoft/mssql-django/releases
 Keywords: django
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: NOTICE.md
 
 # SQL Server backend for Django
 
 Welcome to the MSSQL-Django 3rd party backend project!
@@ -33,16 +34,16 @@
 
 We'd like to give thanks to the community that made this project possible, with particular recognition of the contributors: OskarPersson, michiya, dlo and the original Google Code django-pyodbc team. Moving forward we encourage partipation in this project from both old and new contributors!
 
 We hope you enjoy using the MSSQL-Django 3rd party backend.
 
 ## Features
 
--  Supports Django 3.2 and 4.0
--  Tested on Microsoft SQL Server 2016, 2017, 2019
+-  Supports Django 3.2, 4.0, 4.1 and 4.2
+-  Tested on Microsoft SQL Server 2016, 2017, 2019, 2022
 -  Passes most of the tests of the Django test suite
 -  Compatible with
    [Micosoft ODBC Driver for SQL Server](https://docs.microsoft.com/en-us/sql/connect/odbc/microsoft-odbc-driver-for-sql-server),
    [SQL Server Native Client](https://msdn.microsoft.com/en-us/library/ms131321(v=sql.120).aspx),
    and [FreeTDS](https://www.freetds.org/) ODBC drivers
 
 ## Dependencies
```

### Comparing `mssql-django-1.2/mssql_django.egg-info/SOURCES.txt` & `mssql-django-1.3/mssql_django.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -47,19 +47,21 @@
 testapp/migrations/0017_binarydata_testcheckconstraintwithunicode_and_more.py
 testapp/migrations/0018_choice_question.py
 testapp/migrations/0019_customer_name_customer_address.py
 testapp/migrations/0020_autofield_to_bigautofield.py
 testapp/migrations/0021_multiple_autofield_to_bigauto.py
 testapp/migrations/0022_timezone.py
 testapp/migrations/0023_number.py
+testapp/migrations/0024_publisher_book.py
 testapp/migrations/__init__.py
 testapp/tests/__init__.py
 testapp/tests/test_bitshift.py
 testapp/tests/test_constraints.py
 testapp/tests/test_expressions.py
 testapp/tests/test_fields.py
+testapp/tests/test_getorcreate.py
 testapp/tests/test_indexes.py
 testapp/tests/test_jsonfield.py
 testapp/tests/test_lookups.py
 testapp/tests/test_multiple_databases.py
 testapp/tests/test_queries.py
 testapp/tests/test_timezones.py
```

### Comparing `mssql-django-1.2/setup.py` & `mssql-django-1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,36 +14,37 @@
     'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Framework :: Django :: 3.2',
     'Framework :: Django :: 4.0',
     'Framework :: Django :: 4.1',
+    'Framework :: Django :: 4.2',
 ]
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='mssql-django',
-    version='1.2',
+    version='1.3',
     description='Django backend for Microsoft SQL Server',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Microsoft',
     author_email='opencode@microsoft.com',
     url='https://github.com/microsoft/mssql-django',
     project_urls={
     'Release Notes': 'https://github.com/microsoft/mssql-django/releases',
     },
     license='BSD',
     packages=find_packages(),
     install_requires=[
-        'django>=2.2,<4.2',
+        'django>=3.2,<4.3',
         'pyodbc>=3.0',
         'pytz',
     ],
     package_data={'mssql': ['regex_clr.dll']},
     classifiers=CLASSIFIERS,
     keywords='django',
 )
```

### Comparing `mssql-django-1.2/testapp/migrations/0001_initial.py` & `mssql-django-1.3/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/testapp/migrations/0002_test_unique_nullable_part1.py` & `mssql-django-1.3/testapp/migrations/0002_test_unique_nullable_part1.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/testapp/migrations/0003_test_unique_nullable_part2.py` & `mssql-django-1.3/testapp/migrations/0003_test_unique_nullable_part2.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/testapp/migrations/0004_test_unique_type_change_part1.py` & `mssql-django-1.3/testapp/migrations/0004_test_unique_type_change_part1.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/testapp/migrations/0005_test_unique_type_change_part2.py` & `mssql-django-1.3/testapp/migrations/0005_test_unique_type_change_part2.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/testapp/migrations/0006_test_remove_onetoone_field_part1.py` & `mssql-django-1.3/testapp/migrations/0006_test_remove_onetoone_field_part1.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/testapp/migrations/0008_test_drop_table_with_foreign_key_reference_part1.py` & `mssql-django-1.3/testapp/migrations/0008_test_drop_table_with_foreign_key_reference_part1.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/testapp/migrations/0010_pizza_topping.py` & `mssql-django-1.3/testapp/migrations/0010_pizza_topping.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/testapp/migrations/0011_test_unique_constraints.py` & `mssql-django-1.3/testapp/migrations/0011_test_unique_constraints.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/testapp/migrations/0012_test_indexes_retained_part1.py` & `mssql-django-1.3/testapp/migrations/0012_test_indexes_retained_part1.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/testapp/migrations/0013_test_indexes_retained_part2.py` & `mssql-django-1.3/testapp/migrations/0013_test_indexes_retained_part2.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/testapp/migrations/0014_test_rename_m2mfield_part1.py` & `mssql-django-1.3/testapp/migrations/0014_test_rename_m2mfield_part1.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/testapp/migrations/0015_test_rename_m2mfield_part2.py` & `mssql-django-1.3/testapp/migrations/0015_test_rename_m2mfield_part2.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/testapp/migrations/0016_jsonmodel.py` & `mssql-django-1.3/testapp/migrations/0016_jsonmodel.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/testapp/migrations/0017_binarydata_testcheckconstraintwithunicode_and_more.py` & `mssql-django-1.3/testapp/migrations/0017_binarydata_testcheckconstraintwithunicode_and_more.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/testapp/migrations/0018_choice_question.py` & `mssql-django-1.3/testapp/migrations/0018_choice_question.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/testapp/migrations/0019_customer_name_customer_address.py` & `mssql-django-1.3/testapp/migrations/0019_customer_name_customer_address.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/testapp/migrations/0021_multiple_autofield_to_bigauto.py` & `mssql-django-1.3/testapp/migrations/0021_multiple_autofield_to_bigauto.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/testapp/migrations/0022_timezone.py` & `mssql-django-1.3/testapp/migrations/0022_timezone.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/testapp/migrations/0023_number.py` & `mssql-django-1.3/testapp/migrations/0023_number.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/testapp/models.py` & `mssql-django-1.3/testapp/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import uuid
 
 from django import VERSION
 from django.db import models
 from django.db.models import Q
 from django.utils import timezone
 
-# We are using this Mixin to test casting of BigAuto and Auto fields 
+# We are using this Mixin to test casting of BigAuto and Auto fields
 class BigAutoFieldMixin(models.Model):
     id = models.BigAutoField(primary_key=True)
 
     class Meta:
         abstract = True
 
 class Author(models.Model):
@@ -225,8 +225,24 @@
 
 class Number(models.Model):
     integer = models.BigIntegerField(db_column="the_integer")
     float = models.FloatField(null=True, db_column="the_float")
     decimal_value = models.DecimalField(max_digits=20, decimal_places=17, null=True)
 
     def __str__(self):
-        return "%i, %.3f, %.17f" % (self.integer, self.float, self.decimal_value)
+        return "%i, %.3f, %.17f" % (self.integer, self.float, self.decimal_value)
+
+
+class Publisher(models.Model):
+    name = models.CharField(max_length=100)
+
+
+class Book(models.Model):
+    name = models.CharField(max_length=100)
+    authors = models.ManyToManyField(Author, related_name="books")
+    publisher = models.ForeignKey(
+        Publisher,
+        models.CASCADE,
+        related_name="books",
+        db_column="publisher_id_column",
+    )
+    updated = models.DateTimeField(auto_now=True)
```

### Comparing `mssql-django-1.2/testapp/runners.py` & `mssql-django-1.3/testapp/runners.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/testapp/settings.py` & `mssql-django-1.3/testapp/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -95,16 +95,14 @@
 DEFAULT_AUTO_FIELD = 'django.db.models.AutoField'
 
 ENABLE_REGEX_TESTS = False
 USE_TZ = False
 
 TEST_RUNNER = "testapp.runners.ExcludedTestSuiteRunner"
 EXCLUDED_TESTS = [
-    'aggregation.tests.AggregateTestCase.test_expression_on_aggregation',
-    'aggregation_regress.tests.AggregationTests.test_annotated_conditional_aggregate',
     'aggregation_regress.tests.AggregationTests.test_annotation_with_value',
     'aggregation.tests.AggregateTestCase.test_distinct_on_aggregate',
     'annotations.tests.NonAggregateAnnotationTestCase.test_annotate_exists',
     'custom_lookups.tests.BilateralTransformTests.test_transform_order_by',
     'expressions.tests.BasicExpressionsTests.test_filtering_on_annotate_that_uses_q',
     'expressions.tests.BasicExpressionsTests.test_order_by_exists',
     'expressions.tests.ExpressionOperatorTests.test_righthand_power',
@@ -115,15 +113,14 @@
     'expressions_window.tests.WindowFunctionTests.test_nth_returns_null',
     'expressions_window.tests.WindowFunctionTests.test_nthvalue',
     'expressions_window.tests.WindowFunctionTests.test_range_n_preceding_and_following',
     'field_deconstruction.tests.FieldDeconstructionTests.test_binary_field',
     'ordering.tests.OrderingTests.test_orders_nulls_first_on_filtered_subquery',
     'get_or_create.tests.UpdateOrCreateTransactionTests.test_creation_in_transaction',
     'indexes.tests.PartialIndexTests.test_multiple_conditions',
-    'introspection.tests.IntrospectionTests.test_get_constraints',
     'migrations.test_executor.ExecutorTests.test_alter_id_type_with_fk',
     'migrations.test_operations.OperationTests.test_add_constraint_percent_escaping',
     'migrations.test_operations.OperationTests.test_alter_field_pk',
     'migrations.test_operations.OperationTests.test_alter_field_reloads_state_on_fk_with_to_field_target_changes',
     'schema.tests.SchemaTests.test_alter_auto_field_to_char_field',
     'schema.tests.SchemaTests.test_alter_auto_field_to_integer_field',
     'schema.tests.SchemaTests.test_alter_implicit_id_to_explicit',
@@ -133,32 +130,28 @@
     'schema.tests.SchemaTests.test_remove_field_check_does_not_remove_meta_constraints',
     'schema.tests.SchemaTests.test_remove_field_unique_does_not_remove_meta_constraints',
     'schema.tests.SchemaTests.test_text_field_with_db_index',
     'schema.tests.SchemaTests.test_unique_together_with_fk',
     'schema.tests.SchemaTests.test_unique_together_with_fk_with_existing_index',
     'aggregation.tests.AggregateTestCase.test_count_star',
     'aggregation_regress.tests.AggregationTests.test_values_list_annotation_args_ordering',
-    'db_functions.text.test_pad.PadTests.test_pad',
-    'db_functions.text.test_replace.ReplaceTests.test_case_sensitive',
     'expressions.tests.FTimeDeltaTests.test_invalid_operator',
     'fixtures_regress.tests.TestFixtures.test_loaddata_raises_error_when_fixture_has_invalid_foreign_key',
     'invalid_models_tests.test_ordinary_fields.TextFieldTests.test_max_length_warning',
     'model_indexes.tests.IndexesTests.test_db_tablespace',
     'ordering.tests.OrderingTests.test_deprecated_values_annotate',
     'queries.test_qs_combinators.QuerySetSetOperationTests.test_limits',
     'backends.tests.BackendTestCase.test_unicode_password',
-    'introspection.tests.IntrospectionTests.test_get_table_description_types',
     'migrations.test_commands.MigrateTests.test_migrate_syncdb_app_label',
     'migrations.test_commands.MigrateTests.test_migrate_syncdb_deferred_sql_executed_with_schemaeditor',
     'migrations.test_operations.OperationTests.test_alter_field_pk_fk',
     'schema.tests.SchemaTests.test_add_foreign_key_quoted_db_table',
     'schema.tests.SchemaTests.test_unique_and_reverse_m2m',
     'schema.tests.SchemaTests.test_unique_no_unnecessary_fk_drops',
     'select_for_update.tests.SelectForUpdateTests.test_for_update_after_from',
-    'backends.tests.LastExecutedQueryTest.test_last_executed_query',
     'db_functions.datetime.test_extract_trunc.DateFunctionTests.test_extract_year_exact_lookup',
     'db_functions.datetime.test_extract_trunc.DateFunctionTests.test_extract_year_greaterthan_lookup',
     'db_functions.datetime.test_extract_trunc.DateFunctionTests.test_extract_year_lessthan_lookup',
     'db_functions.datetime.test_extract_trunc.DateFunctionWithTimeZoneTests.test_extract_year_exact_lookup',
     'db_functions.datetime.test_extract_trunc.DateFunctionWithTimeZoneTests.test_extract_year_greaterthan_lookup',
     'db_functions.datetime.test_extract_trunc.DateFunctionWithTimeZoneTests.test_extract_year_lessthan_lookup',
     'db_functions.datetime.test_extract_trunc.DateFunctionWithTimeZoneTests.test_trunc_ambiguous_and_invalid_times',
@@ -172,17 +165,15 @@
     'aggregation.tests.AggregateTestCase.test_aggregation_subquery_annotation_values_collision',
     'db_functions.datetime.test_extract_trunc.DateFunctionWithTimeZoneTests.test_extract_func_with_timezone',
     'expressions.tests.FTimeDeltaTests.test_date_subquery_subtraction',
     'expressions.tests.FTimeDeltaTests.test_datetime_subquery_subtraction',
     'expressions.tests.FTimeDeltaTests.test_time_subquery_subtraction',
     'migrations.test_operations.OperationTests.test_alter_field_reloads_state_on_fk_with_to_field_target_type_change',
     'schema.tests.SchemaTests.test_alter_smallint_pk_to_smallautofield_pk',
-    
     'annotations.tests.NonAggregateAnnotationTestCase.test_combined_expression_annotation_with_aggregation',
-    'db_functions.comparison.test_cast.CastTests.test_cast_to_integer',
     'db_functions.datetime.test_extract_trunc.DateFunctionTests.test_extract_func',
     'db_functions.datetime.test_extract_trunc.DateFunctionTests.test_extract_iso_weekday_func',
     'db_functions.datetime.test_extract_trunc.DateFunctionWithTimeZoneTests.test_extract_func',
     'db_functions.datetime.test_extract_trunc.DateFunctionWithTimeZoneTests.test_extract_iso_weekday_func',
     'datetimes.tests.DateTimesTests.test_datetimes_ambiguous_and_invalid_times',
     'inspectdb.tests.InspectDBTestCase.test_number_field_types',
     'inspectdb.tests.InspectDBTestCase.test_json_field',
@@ -214,15 +205,14 @@
     'expressions.tests.FTimeDeltaTests.test_exclude',
     'expressions.tests.FTimeDeltaTests.test_mixed_comparisons1',
     'expressions.tests.FTimeDeltaTests.test_negative_timedelta_update',
     'inspectdb.tests.InspectDBTestCase.test_field_types',
     'lookup.tests.LookupTests.test_in_ignore_none',
     'lookup.tests.LookupTests.test_in_ignore_none_with_unhashable_items',
     'queries.test_qs_combinators.QuerySetSetOperationTests.test_exists_union',
-    'introspection.tests.IntrospectionTests.test_get_constraints_unique_indexes_orders',
     'schema.tests.SchemaTests.test_ci_cs_db_collation',
     'select_for_update.tests.SelectForUpdateTests.test_unsuported_no_key_raises_error',
 
     # Django 4.0
     'aggregation.tests.AggregateTestCase.test_aggregation_default_using_date_from_database',
     'aggregation.tests.AggregateTestCase.test_aggregation_default_using_datetime_from_database',
     'aggregation.tests.AggregateTestCase.test_aggregation_default_using_time_from_database',
@@ -292,14 +282,27 @@
     'queries.test_qs_combinators.QuerySetSetOperationTests.test_union_in_subquery_related_outerref',
     # These tests pass on SQL Server 2022 or newer
     'model_fields.test_jsonfield.TestQuerying.test_has_key_list',
     'model_fields.test_jsonfield.TestQuerying.test_has_key_null_value',
     'model_fields.test_jsonfield.TestQuerying.test_lookups_with_key_transform',
     'model_fields.test_jsonfield.TestQuerying.test_ordering_grouping_by_count',
     'model_fields.test_jsonfield.TestQuerying.test_has_key_number',
+
+    # Django 4.2
+    'get_or_create.tests.UpdateOrCreateTests.test_update_only_defaults_and_pre_save_fields_when_local_fields',
+    'aggregation.test_filter_argument.FilteredAggregateTests.test_filtered_aggregate_empty_condition',
+    'aggregation.test_filter_argument.FilteredAggregateTests.test_filtered_aggregate_ref_multiple_subquery_annotation',
+    'aggregation.test_filter_argument.FilteredAggregateTests.test_filtered_aggregate_ref_subquery_annotation',
+    "aggregation.tests.AggregateAnnotationPruningTests.test_referenced_group_by_annotation_kept",
+    'aggregation.tests.AggregateTestCase.test_group_by_nested_expression_with_params',
+    'expressions.tests.BasicExpressionsTests.test_aggregate_subquery_annotation',
+    'queries.test_qs_combinators.QuerySetSetOperationTests.test_union_order_with_null_first_last',
+    'queries.test_qs_combinators.QuerySetSetOperationTests.test_union_with_select_related_and_order',
+    'expressions_window.tests.WindowFunctionTests.test_limited_filter',
+    'schema.tests.SchemaTests.test_remove_ignored_unique_constraint_not_create_fk_index',
 ]
 
 REGEX_TESTS = [
     'lookup.tests.LookupTests.test_regex',
     'lookup.tests.LookupTests.test_regex_backreferencing',
     'lookup.tests.LookupTests.test_regex_non_ascii',
     'lookup.tests.LookupTests.test_regex_non_string',
```

### Comparing `mssql-django-1.2/testapp/tests/test_bitshift.py` & `mssql-django-1.3/testapp/tests/test_bitshift.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/testapp/tests/test_constraints.py` & `mssql-django-1.3/testapp/tests/test_constraints.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/testapp/tests/test_expressions.py` & `mssql-django-1.3/testapp/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/testapp/tests/test_fields.py` & `mssql-django-1.3/testapp/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/testapp/tests/test_indexes.py` & `mssql-django-1.3/testapp/tests/test_indexes.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/testapp/tests/test_jsonfield.py` & `mssql-django-1.3/testapp/tests/test_jsonfield.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/testapp/tests/test_multiple_databases.py` & `mssql-django-1.3/testapp/tests/test_multiple_databases.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/testapp/tests/test_queries.py` & `mssql-django-1.3/testapp/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `mssql-django-1.2/testapp/tests/test_timezones.py` & `mssql-django-1.3/testapp/tests/test_timezones.py`

 * *Files identical despite different names*

