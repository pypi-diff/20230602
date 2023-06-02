# Comparing `tmp/oenv2config-1.0.0.tar.gz` & `tmp/oenv2config-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oenv2config-1.0.0.tar", last modified: Sat May  6 10:26:55 2023, max compression
+gzip compressed data, was "oenv2config-1.0.1.tar", last modified: Fri Jun  2 14:33:14 2023, max compression
```

## Comparing `oenv2config-1.0.0.tar` & `oenv2config-1.0.1.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:26:55.464344 oenv2config-1.0.0/
--rw-rw-rw-   0 root         (0) root         (0)     1885 2023-05-05 10:29:38.000000 oenv2config-1.0.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-05-06 10:18:20.000000 oenv2config-1.0.0/.gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:26:55.452344 oenv2config-1.0.0/.idea/
--rw-rw-rw-   0 root         (0) root         (0)      203 2023-05-02 08:56:52.000000 oenv2config-1.0.0/.idea/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      201 2023-05-02 08:56:52.000000 oenv2config-1.0.0/.idea/misc.xml
--rw-rw-rw-   0 root         (0) root         (0)      275 2023-05-02 08:56:52.000000 oenv2config-1.0.0/.idea/modules.xml
--rw-rw-rw-   0 root         (0) root         (0)      949 2023-05-02 08:56:52.000000 oenv2config-1.0.0/.idea/oenv2config.iml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:26:55.456344 oenv2config-1.0.0/.idea/runConfigurations/
--rw-rw-rw-   0 root         (0) root         (0)     1458 2023-05-05 10:29:38.000000 oenv2config-1.0.0/.idea/runConfigurations/Python_tests__no_Odoo_.xml
--rw-rw-rw-   0 root         (0) root         (0)     1565 2023-05-05 10:29:38.000000 oenv2config-1.0.0/.idea/runConfigurations/Python_tests_in_tests_odoo.xml
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-05-02 08:56:52.000000 oenv2config-1.0.0/.idea/vcs.xml
--rw-rw-rw-   0 root         (0) root         (0)      426 2023-05-02 08:56:52.000000 oenv2config-1.0.0/.local-antora-playbook.yml
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-05-05 10:29:38.000000 oenv2config-1.0.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 10:31:13.000000 oenv2config-1.0.0/.ruff
--rw-r--r--   0 root         (0) root         (0)      182 2023-05-06 10:26:55.464344 oenv2config-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      857 2023-05-02 08:56:52.000000 oenv2config-1.0.0/README.adoc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:26:55.456344 oenv2config-1.0.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-05-02 08:56:52.000000 oenv2config-1.0.0/docs/antora.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:26:55.456344 oenv2config-1.0.0/docs/mkdocs/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-05-02 08:56:52.000000 oenv2config-1.0.0/docs/mkdocs/cli.md
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-05-02 08:56:52.000000 oenv2config-1.0.0/docs/mkdocs/db_options.md
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-02 08:56:52.000000 oenv2config-1.0.0/docs/mkdocs/entry.md
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-02 08:56:52.000000 oenv2config-1.0.0/docs/mkdocs/index.md
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-05-02 08:56:52.000000 oenv2config-1.0.0/docs/mkdocs/mappers.md
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-05-02 08:56:52.000000 oenv2config-1.0.0/docs/mkdocs/options.md
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-05-02 08:56:52.000000 oenv2config-1.0.0/docs/mkdocs/reference.md
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-05-02 08:56:52.000000 oenv2config-1.0.0/docs/mkdocs/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-02 08:56:52.000000 oenv2config-1.0.0/docs/mkdocs/utils.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:26:55.452344 oenv2config-1.0.0/docs/modules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:26:55.456344 oenv2config-1.0.0/docs/modules/ROOT/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:26:55.456344 oenv2config-1.0.0/docs/modules/ROOT/images/
--rw-rw-rw-   0 root         (0) root         (0)    44111 2023-05-02 08:56:52.000000 oenv2config-1.0.0/docs/modules/ROOT/images/run_odoo_test.png
--rw-rw-rw-   0 root         (0) root         (0)    35877 2023-05-02 08:56:52.000000 oenv2config-1.0.0/docs/modules/ROOT/images/run_test.png
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-05-02 08:56:52.000000 oenv2config-1.0.0/docs/modules/ROOT/nav.adoc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:26:55.456344 oenv2config-1.0.0/docs/modules/ROOT/pages/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.0.0/docs/modules/ROOT/pages/antora.adoc
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.0.0/docs/modules/ROOT/pages/contribute.adoc
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-05-02 08:56:52.000000 oenv2config-1.0.0/docs/modules/ROOT/pages/index.adoc
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.0.0/docs/modules/ROOT/pages/mkdocs.adoc
--rw-rw-rw-   0 root         (0) root         (0)      754 2023-05-02 08:56:52.000000 oenv2config-1.0.0/docs/modules/ROOT/pages/tests.adoc
--rw-rw-rw-   0 root         (0) root         (0)     1872 2023-05-05 10:29:38.000000 oenv2config-1.0.0/docs/modules/ROOT/pages/tests_odoo.adoc
--rwxrwxrwx   0 root         (0) root         (0)      320 2023-05-05 10:29:38.000000 oenv2config-1.0.0/in_docker_test.sh
--rw-rw-rw-   0 root         (0) root         (0)       56 2023-05-02 08:56:52.000000 oenv2config-1.0.0/mkdocs-plugins.txt
--rw-rw-rw-   0 root         (0) root         (0)     1032 2023-05-02 08:56:52.000000 oenv2config-1.0.0/mkdocs.yml
--rw-rw-rw-   0 root         (0) root         (0)      753 2023-05-05 10:29:38.000000 oenv2config-1.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-06 10:26:55.464344 oenv2config-1.0.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      399 2023-05-02 08:56:52.000000 oenv2config-1.0.0/setup.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:26:55.452344 oenv2config-1.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:26:55.456344 oenv2config-1.0.0/src/odoo_env_config/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.0.0/src/odoo_env_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-05-06 10:26:55.000000 oenv2config-1.0.0/src/odoo_env_config/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     4690 2023-05-02 08:56:52.000000 oenv2config-1.0.0/src/odoo_env_config/api.py
--rw-rw-rw-   0 root         (0) root         (0)     3960 2023-05-02 08:56:52.000000 oenv2config-1.0.0/src/odoo_env_config/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2412 2023-05-02 08:56:52.000000 oenv2config-1.0.0/src/odoo_env_config/entry.py
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-05-02 08:56:52.000000 oenv2config-1.0.0/src/odoo_env_config/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4475 2023-05-02 08:56:52.000000 oenv2config-1.0.0/src/odoo_env_config/mappers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:26:55.452344 oenv2config-1.0.0/src/odoo_env_config/odoo_modules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:26:55.456344 oenv2config-1.0.0/src/odoo_env_config/odoo_modules/env2config/
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-05 10:31:13.000000 oenv2config-1.0.0/src/odoo_env_config/odoo_modules/env2config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2023-05-02 08:56:52.000000 oenv2config-1.0.0/src/odoo_env_config/odoo_modules/env2config/__manifest__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:26:55.456344 oenv2config-1.0.0/src/odoo_env_config/odoo_modules/env2config/cli/
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-05-02 08:56:52.000000 oenv2config-1.0.0/src/odoo_env_config/odoo_modules/env2config/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:26:55.460344 oenv2config-1.0.0/src/odoo_env_config/section/
--rw-rw-rw-   0 root         (0) root         (0)      802 2023-05-02 08:56:52.000000 oenv2config-1.0.0/src/odoo_env_config/section/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      659 2023-05-05 10:29:38.000000 oenv2config-1.0.0/src/odoo_env_config/section/addons_path_section.py
--rw-rw-rw-   0 root         (0) root         (0)     4172 2023-05-02 08:56:52.000000 oenv2config-1.0.0/src/odoo_env_config/section/db_section.py
--rw-rw-rw-   0 root         (0) root         (0)      961 2023-05-02 08:56:52.000000 oenv2config-1.0.0/src/odoo_env_config/section/http_section.py
--rw-rw-rw-   0 root         (0) root         (0)     2151 2023-05-02 08:56:52.000000 oenv2config-1.0.0/src/odoo_env_config/section/limit_section.py
--rw-rw-rw-   0 root         (0) root         (0)     1512 2023-05-02 08:56:52.000000 oenv2config-1.0.0/src/odoo_env_config/section/log_section.py
--rw-rw-rw-   0 root         (0) root         (0)      972 2023-05-02 08:56:52.000000 oenv2config-1.0.0/src/odoo_env_config/section/misc_section.py
--rw-rw-rw-   0 root         (0) root         (0)      861 2023-05-02 08:56:52.000000 oenv2config-1.0.0/src/odoo_env_config/section/test_section.py
--rw-rw-rw-   0 root         (0) root         (0)      611 2023-05-02 08:56:52.000000 oenv2config-1.0.0/src/odoo_env_config/section/update_init_section.py
--rw-rw-rw-   0 root         (0) root         (0)     1030 2023-05-02 08:56:52.000000 oenv2config-1.0.0/src/odoo_env_config/section/widemodule_section.py
--rw-rw-rw-   0 root         (0) root         (0)     2322 2023-05-02 08:56:52.000000 oenv2config-1.0.0/src/odoo_env_config/section/worker_section.py
--rw-rw-rw-   0 root         (0) root         (0)    10125 2023-05-02 08:56:52.000000 oenv2config-1.0.0/src/odoo_env_config/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:26:55.460344 oenv2config-1.0.0/src/oenv2config.egg-info/
--rw-r--r--   0 root         (0) root         (0)      182 2023-05-06 10:26:55.000000 oenv2config-1.0.0/src/oenv2config.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3205 2023-05-06 10:26:55.000000 oenv2config-1.0.0/src/oenv2config.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 10:26:55.000000 oenv2config-1.0.0/src/oenv2config.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2023-05-06 10:26:55.000000 oenv2config-1.0.0/src/oenv2config.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       72 2023-05-06 10:26:55.000000 oenv2config-1.0.0/src/oenv2config.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-06 10:26:55.000000 oenv2config-1.0.0/src/oenv2config.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:26:55.460344 oenv2config-1.0.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.0.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2148 2023-05-05 10:29:38.000000 oenv2config-1.0.0/tests/_decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     3154 2023-05-02 08:56:52.000000 oenv2config-1.0.0/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)      310 2023-05-02 08:56:52.000000 oenv2config-1.0.0/tests/test_doctests.py
--rw-rw-rw-   0 root         (0) root         (0)     1942 2023-05-02 08:56:52.000000 oenv2config-1.0.0/tests/test_entry.py
--rw-rw-rw-   0 root         (0) root         (0)      740 2023-05-02 08:56:52.000000 oenv2config-1.0.0/tests/test_libs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:26:55.460344 oenv2config-1.0.0/tests/test_mapper/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.0.0/tests/test_mapper/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7703 2023-05-05 10:29:38.000000 oenv2config-1.0.0/tests/test_mapper/test_mapper_clever_cloud_cellar.py
--rw-rw-rw-   0 root         (0) root         (0)    10835 2023-05-02 08:56:52.000000 oenv2config-1.0.0/tests/test_mapper/test_mapper_clever_cloud_postgres.py
--rw-rw-rw-   0 root         (0) root         (0)     6535 2023-05-02 08:56:52.000000 oenv2config-1.0.0/tests/test_mapper/test_mapper_odoo_compatibility.py
--rw-rw-rw-   0 root         (0) root         (0)     5002 2023-05-02 08:56:52.000000 oenv2config-1.0.0/tests/test_mapper/test_mapper_queue_job.py
--rw-rw-rw-   0 root         (0) root         (0)     3921 2023-05-02 08:56:52.000000 oenv2config-1.0.0/tests/test_mapper/test_mapper_redis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:26:55.460344 oenv2config-1.0.0/tests/test_section/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.0.0/tests/test_section/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1366 2023-05-05 10:29:38.000000 oenv2config-1.0.0/tests/test_section/test_addons_path_section.py
--rw-rw-rw-   0 root         (0) root         (0)     7581 2023-05-02 08:56:52.000000 oenv2config-1.0.0/tests/test_section/test_db_section.py
--rw-rw-rw-   0 root         (0) root         (0)     2339 2023-05-02 08:56:52.000000 oenv2config-1.0.0/tests/test_section/test_http_section.py
--rw-rw-rw-   0 root         (0) root         (0)     5567 2023-05-02 08:56:52.000000 oenv2config-1.0.0/tests/test_section/test_limit_section.py
--rw-rw-rw-   0 root         (0) root         (0)     2489 2023-05-02 08:56:52.000000 oenv2config-1.0.0/tests/test_section/test_log_section.py
--rw-rw-rw-   0 root         (0) root         (0)     1389 2023-05-02 08:56:52.000000 oenv2config-1.0.0/tests/test_section/test_misc_section.py
--rw-rw-rw-   0 root         (0) root         (0)     1989 2023-05-05 10:29:38.000000 oenv2config-1.0.0/tests/test_section/test_test_section.py
--rw-rw-rw-   0 root         (0) root         (0)     1259 2023-05-05 10:29:38.000000 oenv2config-1.0.0/tests/test_section/test_update_init_section.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2023-05-02 08:56:52.000000 oenv2config-1.0.0/tests/test_section/test_widemodule_section.py
--rw-rw-rw-   0 root         (0) root         (0)     6727 2023-05-02 08:56:52.000000 oenv2config-1.0.0/tests/test_section/test_worker_section.py
--rw-rw-rw-   0 root         (0) root         (0)     2436 2023-05-05 10:29:38.000000 oenv2config-1.0.0/tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:26:55.460344 oenv2config-1.0.0/tests/tests_odoo/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.0.0/tests/tests_odoo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4906 2023-05-05 10:29:38.000000 oenv2config-1.0.0/tests/tests_odoo/_helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 10:26:55.464344 oenv2config-1.0.0/tests/tests_odoo/profiles/
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-02 08:56:52.000000 oenv2config-1.0.0/tests/tests_odoo/profiles/filestore_s3.env
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-02 08:56:52.000000 oenv2config-1.0.0/tests/tests_odoo/profiles/filestore_s3_cellar.env
--rw-rw-rw-   0 root         (0) root         (0)      175 2023-05-02 08:56:52.000000 oenv2config-1.0.0/tests/tests_odoo/profiles/test_db_clever.env
--rw-rw-rw-   0 root         (0) root         (0)      217 2023-05-02 08:56:52.000000 oenv2config-1.0.0/tests/tests_odoo/profiles/test_db_clever_direct.env
--rw-rw-rw-   0 root         (0) root         (0)     4115 2023-05-05 10:29:38.000000 oenv2config-1.0.0/tests/tests_odoo/test_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.118942 oenv2config-1.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1885 2023-05-05 10:29:38.000000 oenv2config-1.0.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-05-06 10:18:20.000000 oenv2config-1.0.1/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.098942 oenv2config-1.0.1/.idea/
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-05-02 08:56:52.000000 oenv2config-1.0.1/.idea/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      201 2023-05-02 08:56:52.000000 oenv2config-1.0.1/.idea/misc.xml
+-rw-rw-rw-   0 root         (0) root         (0)      275 2023-05-02 08:56:52.000000 oenv2config-1.0.1/.idea/modules.xml
+-rw-rw-rw-   0 root         (0) root         (0)      949 2023-05-02 08:56:52.000000 oenv2config-1.0.1/.idea/oenv2config.iml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.098942 oenv2config-1.0.1/.idea/runConfigurations/
+-rw-rw-rw-   0 root         (0) root         (0)     1458 2023-05-05 10:29:38.000000 oenv2config-1.0.1/.idea/runConfigurations/Python_tests__no_Odoo_.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1565 2023-05-05 10:29:38.000000 oenv2config-1.0.1/.idea/runConfigurations/Python_tests_in_tests_odoo.xml
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-05-02 08:56:52.000000 oenv2config-1.0.1/.idea/vcs.xml
+-rw-rw-rw-   0 root         (0) root         (0)      426 2023-05-02 08:56:52.000000 oenv2config-1.0.1/.local-antora-playbook.yml
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-05-05 10:29:38.000000 oenv2config-1.0.1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 10:31:13.000000 oenv2config-1.0.1/.ruff
+-rw-r--r--   0 root         (0) root         (0)      182 2023-06-02 14:33:14.114942 oenv2config-1.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      857 2023-05-02 08:56:52.000000 oenv2config-1.0.1/README.adoc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.098942 oenv2config-1.0.1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-05-02 08:56:52.000000 oenv2config-1.0.1/docs/antora.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.098942 oenv2config-1.0.1/docs/mkdocs/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-05-02 08:56:52.000000 oenv2config-1.0.1/docs/mkdocs/cli.md
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-05-02 08:56:52.000000 oenv2config-1.0.1/docs/mkdocs/db_options.md
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-02 08:56:52.000000 oenv2config-1.0.1/docs/mkdocs/entry.md
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-02 08:56:52.000000 oenv2config-1.0.1/docs/mkdocs/index.md
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-05-02 08:56:52.000000 oenv2config-1.0.1/docs/mkdocs/mappers.md
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-05-02 08:56:52.000000 oenv2config-1.0.1/docs/mkdocs/options.md
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-05-02 08:56:52.000000 oenv2config-1.0.1/docs/mkdocs/reference.md
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-05-02 08:56:52.000000 oenv2config-1.0.1/docs/mkdocs/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-02 08:56:52.000000 oenv2config-1.0.1/docs/mkdocs/utils.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.090942 oenv2config-1.0.1/docs/modules/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.098942 oenv2config-1.0.1/docs/modules/ROOT/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.102942 oenv2config-1.0.1/docs/modules/ROOT/images/
+-rw-rw-rw-   0 root         (0) root         (0)    44111 2023-05-02 08:56:52.000000 oenv2config-1.0.1/docs/modules/ROOT/images/run_odoo_test.png
+-rw-rw-rw-   0 root         (0) root         (0)    35877 2023-05-02 08:56:52.000000 oenv2config-1.0.1/docs/modules/ROOT/images/run_test.png
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-05-02 08:56:52.000000 oenv2config-1.0.1/docs/modules/ROOT/nav.adoc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.102942 oenv2config-1.0.1/docs/modules/ROOT/pages/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.0.1/docs/modules/ROOT/pages/antora.adoc
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.0.1/docs/modules/ROOT/pages/contribute.adoc
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-05-02 08:56:52.000000 oenv2config-1.0.1/docs/modules/ROOT/pages/index.adoc
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.0.1/docs/modules/ROOT/pages/mkdocs.adoc
+-rw-rw-rw-   0 root         (0) root         (0)      754 2023-06-02 13:54:32.000000 oenv2config-1.0.1/docs/modules/ROOT/pages/tests.adoc
+-rw-rw-rw-   0 root         (0) root         (0)     1872 2023-06-02 13:54:32.000000 oenv2config-1.0.1/docs/modules/ROOT/pages/tests_odoo.adoc
+-rwxrwxrwx   0 root         (0) root         (0)      320 2023-05-05 10:29:38.000000 oenv2config-1.0.1/in_docker_test.sh
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-05-02 08:56:52.000000 oenv2config-1.0.1/mkdocs-plugins.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1032 2023-05-02 08:56:52.000000 oenv2config-1.0.1/mkdocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)      753 2023-05-05 10:29:38.000000 oenv2config-1.0.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-02 14:33:14.118942 oenv2config-1.0.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      399 2023-05-02 08:56:52.000000 oenv2config-1.0.1/setup.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.090942 oenv2config-1.0.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.102942 oenv2config-1.0.1/src/odoo_env_config/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.0.1/src/odoo_env_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-06-02 14:33:13.000000 oenv2config-1.0.1/src/odoo_env_config/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     4690 2023-06-02 13:54:32.000000 oenv2config-1.0.1/src/odoo_env_config/api.py
+-rw-rw-rw-   0 root         (0) root         (0)     4121 2023-06-02 13:54:32.000000 oenv2config-1.0.1/src/odoo_env_config/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2412 2023-06-02 13:54:32.000000 oenv2config-1.0.1/src/odoo_env_config/entry.py
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-05-02 08:56:52.000000 oenv2config-1.0.1/src/odoo_env_config/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4475 2023-06-02 13:54:32.000000 oenv2config-1.0.1/src/odoo_env_config/mappers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.090942 oenv2config-1.0.1/src/odoo_env_config/odoo_modules/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.106942 oenv2config-1.0.1/src/odoo_env_config/odoo_modules/env2config/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-05 10:31:13.000000 oenv2config-1.0.1/src/odoo_env_config/odoo_modules/env2config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-05-02 08:56:52.000000 oenv2config-1.0.1/src/odoo_env_config/odoo_modules/env2config/__manifest__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.106942 oenv2config-1.0.1/src/odoo_env_config/odoo_modules/env2config/cli/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-05-02 08:56:52.000000 oenv2config-1.0.1/src/odoo_env_config/odoo_modules/env2config/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.106942 oenv2config-1.0.1/src/odoo_env_config/section/
+-rw-rw-rw-   0 root         (0) root         (0)      802 2023-06-02 13:54:32.000000 oenv2config-1.0.1/src/odoo_env_config/section/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      659 2023-06-02 13:54:32.000000 oenv2config-1.0.1/src/odoo_env_config/section/addons_path_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     4172 2023-06-02 13:54:32.000000 oenv2config-1.0.1/src/odoo_env_config/section/db_section.py
+-rw-rw-rw-   0 root         (0) root         (0)      961 2023-06-02 13:54:32.000000 oenv2config-1.0.1/src/odoo_env_config/section/http_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     2151 2023-06-02 13:54:32.000000 oenv2config-1.0.1/src/odoo_env_config/section/limit_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     1512 2023-06-02 13:54:32.000000 oenv2config-1.0.1/src/odoo_env_config/section/log_section.py
+-rw-rw-rw-   0 root         (0) root         (0)      972 2023-06-02 13:54:32.000000 oenv2config-1.0.1/src/odoo_env_config/section/misc_section.py
+-rw-rw-rw-   0 root         (0) root         (0)      861 2023-06-02 13:54:32.000000 oenv2config-1.0.1/src/odoo_env_config/section/test_section.py
+-rw-rw-rw-   0 root         (0) root         (0)      611 2023-06-02 13:54:32.000000 oenv2config-1.0.1/src/odoo_env_config/section/update_init_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2023-06-02 13:54:32.000000 oenv2config-1.0.1/src/odoo_env_config/section/widemodule_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     2322 2023-06-02 13:54:32.000000 oenv2config-1.0.1/src/odoo_env_config/section/worker_section.py
+-rw-rw-rw-   0 root         (0) root         (0)    10125 2023-05-02 08:56:52.000000 oenv2config-1.0.1/src/odoo_env_config/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.110942 oenv2config-1.0.1/src/oenv2config.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      182 2023-06-02 14:33:14.000000 oenv2config-1.0.1/src/oenv2config.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3205 2023-06-02 14:33:14.000000 oenv2config-1.0.1/src/oenv2config.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 14:33:14.000000 oenv2config-1.0.1/src/oenv2config.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2023-06-02 14:33:14.000000 oenv2config-1.0.1/src/oenv2config.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       72 2023-06-02 14:33:14.000000 oenv2config-1.0.1/src/oenv2config.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-02 14:33:14.000000 oenv2config-1.0.1/src/oenv2config.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.110942 oenv2config-1.0.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2148 2023-05-05 10:29:38.000000 oenv2config-1.0.1/tests/_decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     3154 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      310 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/test_doctests.py
+-rw-rw-rw-   0 root         (0) root         (0)     1942 2023-06-02 13:54:32.000000 oenv2config-1.0.1/tests/test_entry.py
+-rw-rw-rw-   0 root         (0) root         (0)      740 2023-06-02 13:54:32.000000 oenv2config-1.0.1/tests/test_libs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.110942 oenv2config-1.0.1/tests/test_mapper/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/test_mapper/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7703 2023-06-02 13:54:32.000000 oenv2config-1.0.1/tests/test_mapper/test_mapper_clever_cloud_cellar.py
+-rw-rw-rw-   0 root         (0) root         (0)    10835 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/test_mapper/test_mapper_clever_cloud_postgres.py
+-rw-rw-rw-   0 root         (0) root         (0)     6535 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/test_mapper/test_mapper_odoo_compatibility.py
+-rw-rw-rw-   0 root         (0) root         (0)     5002 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/test_mapper/test_mapper_queue_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     3921 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/test_mapper/test_mapper_redis.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.114942 oenv2config-1.0.1/tests/test_section/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/test_section/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1366 2023-05-05 10:29:38.000000 oenv2config-1.0.1/tests/test_section/test_addons_path_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     7581 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/test_section/test_db_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     2339 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/test_section/test_http_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     5567 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/test_section/test_limit_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     2489 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/test_section/test_log_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     1389 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/test_section/test_misc_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     1989 2023-05-05 10:29:38.000000 oenv2config-1.0.1/tests/test_section/test_test_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     1259 2023-05-05 10:29:38.000000 oenv2config-1.0.1/tests/test_section/test_update_init_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/test_section/test_widemodule_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     6727 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/test_section/test_worker_section.py
+-rw-rw-rw-   0 root         (0) root         (0)     2436 2023-06-02 13:54:32.000000 oenv2config-1.0.1/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.114942 oenv2config-1.0.1/tests/tests_odoo/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/tests_odoo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4906 2023-05-05 10:29:38.000000 oenv2config-1.0.1/tests/tests_odoo/_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:33:14.114942 oenv2config-1.0.1/tests/tests_odoo/profiles/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/tests_odoo/profiles/filestore_s3.env
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/tests_odoo/profiles/filestore_s3_cellar.env
+-rw-rw-rw-   0 root         (0) root         (0)      175 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/tests_odoo/profiles/test_db_clever.env
+-rw-rw-rw-   0 root         (0) root         (0)      217 2023-05-02 08:56:52.000000 oenv2config-1.0.1/tests/tests_odoo/profiles/test_db_clever_direct.env
+-rw-rw-rw-   0 root         (0) root         (0)     4115 2023-05-05 10:29:38.000000 oenv2config-1.0.1/tests/tests_odoo/test_base.py
```

### Comparing `oenv2config-1.0.0/.gitignore` & `oenv2config-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/.gitlab-ci.yml` & `oenv2config-1.0.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/.idea/oenv2config.iml` & `oenv2config-1.0.1/.idea/oenv2config.iml`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/.idea/runConfigurations/Python_tests__no_Odoo_.xml` & `oenv2config-1.0.1/.idea/runConfigurations/Python_tests__no_Odoo_.xml`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/.idea/runConfigurations/Python_tests_in_tests_odoo.xml` & `oenv2config-1.0.1/.idea/runConfigurations/Python_tests_in_tests_odoo.xml`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/.pre-commit-config.yaml` & `oenv2config-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/README.adoc` & `oenv2config-1.0.1/README.adoc`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/docs/modules/ROOT/images/run_odoo_test.png` & `oenv2config-1.0.1/docs/modules/ROOT/images/run_odoo_test.png`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/docs/modules/ROOT/images/run_test.png` & `oenv2config-1.0.1/docs/modules/ROOT/images/run_test.png`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/docs/modules/ROOT/pages/tests.adoc` & `oenv2config-1.0.1/docs/modules/ROOT/pages/tests.adoc`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/docs/modules/ROOT/pages/tests_odoo.adoc` & `oenv2config-1.0.1/docs/modules/ROOT/pages/tests_odoo.adoc`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/mkdocs.yml` & `oenv2config-1.0.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/pyproject.toml` & `oenv2config-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/src/odoo_env_config/api.py` & `oenv2config-1.0.1/src/odoo_env_config/api.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/src/odoo_env_config/cli.py` & `oenv2config-1.0.1/src/odoo_env_config/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 from dotenv import dotenv_values
 
 from . import api, entry
 
 
 def get_odoo_cmd_parser() -> argparse.ArgumentParser:
     p = argparse.ArgumentParser()
-    p.add_argument("--profile", action="append", dest="profiles", default=[])
-    p.add_argument("--dest", dest="config_dest")
+    p.add_argument("--profile", action="append", dest="profiles", default=[], help="profile to use")
+    p.add_argument("--dest", dest="config_dest", help="Path to odoo configuration file")
     return p
 
 
 class OdooCommand:
     """
     This contains a new OdooCommand named `env2config`
     This class prupose is to use it inside an Odoo modules
@@ -81,23 +81,24 @@
     return extra_env
 
 
 load_profiles = _load_profiles
 
 
 def env_to_config():
-    parser = argparse.ArgumentParser(parents=[get_odoo_cmd_parser()])
+    # add_help=False otherwise conflict with -h parameter of parent parser
+    parser = argparse.ArgumentParser(parents=[get_odoo_cmd_parser()], add_help=False)
     parser.add_argument(
         "odoo_bin",
         default=api.Env().odoo_bin,
         nargs="?",
         help="Path to odoo-bin file, env:ODOO_BIN or /odoo/odoo-bin is used",
     )
     ns, other = parser.parse_known_args()
-    parser.exit(execute_odoo_cli_helper(ns.odoo_bin, ns.profiles, ns.dest, other))
+    parser.exit(execute_odoo_cli_helper(ns.odoo_bin, ns.profiles, ns.config_dest, other))
 
 
 def execute_odoo_cli_helper(odoo_bin: str, profiles: List[str], odoo_rc: str, extra_odoo_args: List[str] = None) -> int:
     return execute_odoo_cli(
         os.path.abspath(os.path.expanduser(odoo_bin)),
         ["--profile=" + profile for profile in profiles] + ["--dest=" + odoo_rc] + extra_odoo_args,
     )
```

### Comparing `oenv2config-1.0.0/src/odoo_env_config/entry.py` & `oenv2config-1.0.1/src/odoo_env_config/entry.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/src/odoo_env_config/mappers.py` & `oenv2config-1.0.1/src/odoo_env_config/mappers.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/src/odoo_env_config/odoo_modules/env2config/__manifest__.py` & `oenv2config-1.0.1/src/odoo_env_config/odoo_modules/env2config/__manifest__.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/src/odoo_env_config/section/__init__.py` & `oenv2config-1.0.1/src/odoo_env_config/section/__init__.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/src/odoo_env_config/section/addons_path_section.py` & `oenv2config-1.0.1/src/odoo_env_config/section/addons_path_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/src/odoo_env_config/section/db_section.py` & `oenv2config-1.0.1/src/odoo_env_config/section/db_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/src/odoo_env_config/section/http_section.py` & `oenv2config-1.0.1/src/odoo_env_config/section/http_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/src/odoo_env_config/section/limit_section.py` & `oenv2config-1.0.1/src/odoo_env_config/section/limit_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/src/odoo_env_config/section/log_section.py` & `oenv2config-1.0.1/src/odoo_env_config/section/log_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/src/odoo_env_config/section/misc_section.py` & `oenv2config-1.0.1/src/odoo_env_config/section/misc_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/src/odoo_env_config/section/test_section.py` & `oenv2config-1.0.1/src/odoo_env_config/section/test_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/src/odoo_env_config/section/update_init_section.py` & `oenv2config-1.0.1/src/odoo_env_config/section/update_init_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/src/odoo_env_config/section/widemodule_section.py` & `oenv2config-1.0.1/src/odoo_env_config/section/widemodule_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/src/odoo_env_config/section/worker_section.py` & `oenv2config-1.0.1/src/odoo_env_config/section/worker_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/src/odoo_env_config/utils.py` & `oenv2config-1.0.1/src/odoo_env_config/utils.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/src/oenv2config.egg-info/SOURCES.txt` & `oenv2config-1.0.1/src/oenv2config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/tests/_decorators.py` & `oenv2config-1.0.1/tests/_decorators.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/tests/test_cli.py` & `oenv2config-1.0.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/tests/test_entry.py` & `oenv2config-1.0.1/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/tests/test_libs.py` & `oenv2config-1.0.1/tests/test_libs.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/tests/test_mapper/test_mapper_clever_cloud_cellar.py` & `oenv2config-1.0.1/tests/test_mapper/test_mapper_clever_cloud_cellar.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/tests/test_mapper/test_mapper_clever_cloud_postgres.py` & `oenv2config-1.0.1/tests/test_mapper/test_mapper_clever_cloud_postgres.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/tests/test_mapper/test_mapper_odoo_compatibility.py` & `oenv2config-1.0.1/tests/test_mapper/test_mapper_odoo_compatibility.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/tests/test_mapper/test_mapper_queue_job.py` & `oenv2config-1.0.1/tests/test_mapper/test_mapper_queue_job.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/tests/test_mapper/test_mapper_redis.py` & `oenv2config-1.0.1/tests/test_mapper/test_mapper_redis.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/tests/test_section/test_addons_path_section.py` & `oenv2config-1.0.1/tests/test_section/test_addons_path_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/tests/test_section/test_db_section.py` & `oenv2config-1.0.1/tests/test_section/test_db_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/tests/test_section/test_http_section.py` & `oenv2config-1.0.1/tests/test_section/test_http_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/tests/test_section/test_limit_section.py` & `oenv2config-1.0.1/tests/test_section/test_limit_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/tests/test_section/test_log_section.py` & `oenv2config-1.0.1/tests/test_section/test_log_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/tests/test_section/test_misc_section.py` & `oenv2config-1.0.1/tests/test_section/test_misc_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/tests/test_section/test_test_section.py` & `oenv2config-1.0.1/tests/test_section/test_test_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/tests/test_section/test_update_init_section.py` & `oenv2config-1.0.1/tests/test_section/test_update_init_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/tests/test_section/test_widemodule_section.py` & `oenv2config-1.0.1/tests/test_section/test_widemodule_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/tests/test_section/test_worker_section.py` & `oenv2config-1.0.1/tests/test_section/test_worker_section.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/tests/test_utils.py` & `oenv2config-1.0.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/tests/tests_odoo/_helpers.py` & `oenv2config-1.0.1/tests/tests_odoo/_helpers.py`

 * *Files identical despite different names*

### Comparing `oenv2config-1.0.0/tests/tests_odoo/test_base.py` & `oenv2config-1.0.1/tests/tests_odoo/test_base.py`

 * *Files identical despite different names*

