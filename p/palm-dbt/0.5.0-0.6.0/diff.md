# Comparing `tmp/palm-dbt-0.5.0.tar.gz` & `tmp/palm-dbt-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "palm-dbt-0.5.0.tar", last modified: Thu Mar 16 16:53:31 2023, max compression
+gzip compressed data, was "palm-dbt-0.6.0.tar", last modified: Fri Jun  2 15:08:03 2023, max compression
```

## Comparing `palm-dbt-0.5.0.tar` & `palm-dbt-0.6.0.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:53:31.705548 palm-dbt-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-03-16 16:53:31.701548 palm-dbt-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:53:31.697548 palm-dbt-0.5.0/palm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:53:31.697548 palm-dbt-0.5.0/palm/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:53:31.697548 palm-dbt-0.5.0/palm/plugins/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:53:31.701548 palm-dbt-0.5.0/palm/plugins/dbt/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/commands/cmd_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/commands/cmd_compile.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/commands/cmd_containerize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/commands/cmd_cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/commands/cmd_dbt-docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/commands/cmd_dbt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/commands/cmd_install.py
--rw-r--r--   0 runner    (1001) docker     (123)     9595 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/commands/cmd_model-doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/commands/cmd_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/commands/cmd_prod-artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/commands/cmd_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/commands/cmd_shell.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/commands/cmd_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/commands/cmd_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/dbt_containerizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/dbt_palm_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/dbt_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/local_user_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:53:31.701548 palm-dbt-0.5.0/palm/plugins/dbt/macros/
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/macros/drop_branch_schemas.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/macros/generate_schema_name.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:53:31.697548 palm-dbt-0.5.0/palm/plugins/dbt/model_template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:53:31.701548 palm-dbt-0.5.0/palm/plugins/dbt/model_template/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/model_template/docs/base_model.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/model_template/docs/template-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:53:31.701548 palm-dbt-0.5.0/palm/plugins/dbt/model_template/model/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/model_template/model/base_model.sql
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/model_template/model/base_model.yml
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/model_template/model/template-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:53:31.701548 palm-dbt-0.5.0/palm/plugins/dbt/model_template/ref_files/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/model_template/ref_files/ref_file.sql
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/model_template/ref_files/ref_file_readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:53:31.701548 palm-dbt-0.5.0/palm/plugins/dbt/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/parsers/project_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/plugin_config.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/sql_to_dbt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:53:31.697548 palm-dbt-0.5.0/palm/plugins/dbt/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:53:31.701548 palm-dbt-0.5.0/palm/plugins/dbt/templates/containerize/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/templates/containerize/Dockerfile.txt
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/templates/containerize/docker-compose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/templates/containerize/entrypoint.sh.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/templates/containerize/template-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:53:31.701548 palm-dbt-0.5.0/palm/plugins/dbt/templates/model_docs/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/templates/model_docs/model_doc.tpl.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/palm/plugins/dbt/templates/model_docs/template-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:53:31.701548 palm-dbt-0.5.0/palm_dbt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-03-16 16:53:31.000000 palm-dbt-0.5.0/palm_dbt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-03-16 16:53:31.000000 palm-dbt-0.5.0/palm_dbt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 16:53:31.000000 palm-dbt-0.5.0/palm_dbt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-16 16:53:31.000000 palm-dbt-0.5.0/palm_dbt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-16 16:53:31.000000 palm-dbt-0.5.0/palm_dbt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 16:53:31.705548 palm-dbt-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-03-16 16:53:21.000000 palm-dbt-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:08:03.135712 palm-dbt-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-06-02 15:08:03.135712 palm-dbt-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:08:03.119712 palm-dbt-0.6.0/palm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:08:03.119712 palm-dbt-0.6.0/palm/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:08:03.123712 palm-dbt-0.6.0/palm/plugins/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:08:03.127713 palm-dbt-0.6.0/palm/plugins/dbt/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_containerize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_dbt-docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_dbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9595 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_model-doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_prod-artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/dbt_containerizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/dbt_palm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/dbt_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/local_user_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:08:03.127713 palm-dbt-0.6.0/palm/plugins/dbt/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/macros/drop_branch_schemas.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/macros/generate_schema_name.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:08:03.119712 palm-dbt-0.6.0/palm/plugins/dbt/model_template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:08:03.131713 palm-dbt-0.6.0/palm/plugins/dbt/model_template/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/model_template/docs/base_model.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/model_template/docs/template-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:08:03.131713 palm-dbt-0.6.0/palm/plugins/dbt/model_template/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/model_template/model/base_model.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/model_template/model/base_model.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/model_template/model/template-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:08:03.131713 palm-dbt-0.6.0/palm/plugins/dbt/model_template/ref_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/model_template/ref_files/ref_file.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/model_template/ref_files/ref_file_readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:08:03.131713 palm-dbt-0.6.0/palm/plugins/dbt/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/parsers/project_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/plugin_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/sql_to_dbt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:08:03.119712 palm-dbt-0.6.0/palm/plugins/dbt/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:08:03.131713 palm-dbt-0.6.0/palm/plugins/dbt/templates/containerize/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/templates/containerize/Dockerfile.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/templates/containerize/docker-compose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/templates/containerize/entrypoint.sh.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/templates/containerize/template-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:08:03.135712 palm-dbt-0.6.0/palm/plugins/dbt/templates/model_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/templates/model_docs/model_doc.tpl.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/palm/plugins/dbt/templates/model_docs/template-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:08:03.135712 palm-dbt-0.6.0/palm_dbt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-06-02 15:08:03.000000 palm-dbt-0.6.0/palm_dbt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-02 15:08:03.000000 palm-dbt-0.6.0/palm_dbt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 15:08:03.000000 palm-dbt-0.6.0/palm_dbt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-02 15:08:03.000000 palm-dbt-0.6.0/palm_dbt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-02 15:08:03.000000 palm-dbt-0.6.0/palm_dbt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 15:08:03.135712 palm-dbt-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-02 15:07:53.000000 palm-dbt-0.6.0/setup.py
```

### Comparing `palm-dbt-0.5.0/LICENSE` & `palm-dbt-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.5.0/PKG-INFO` & `palm-dbt-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palm-dbt
-Version: 0.5.0
+Version: 0.6.0
 Summary: dbt extension for Palm CLI
 Home-page: https://github.com/palmetto/palm-dbt
 Author: Palmetto - Data & Analytics team
 Author-email: data-analytics-team@palmetto.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `palm-dbt-0.5.0/README.md` & `palm-dbt-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.5.0/palm/plugins/dbt/commands/cmd_cleanup.py` & `palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_cleanup.py`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.5.0/palm/plugins/dbt/commands/cmd_compile.py` & `palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_compile.py`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.5.0/palm/plugins/dbt/commands/cmd_containerize.py` & `palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_containerize.py`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.5.0/palm/plugins/dbt/commands/cmd_cycle.py` & `palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_cycle.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 @click.command("cycle")
 @click.argument("count", type=int, default=2)
 @click.option(
     "--persist", is_flag=True, help="will not drop the test schema at the end"
 )
 @click.option("--models", multiple=True, help="see dbt docs on models flag")
 @click.option("--select", multiple=True, help="see dbt docs on select flag")
-@click.option("--no-seed", is_flag=True, help="will skip seed full refresh")
+@click.option("--seed", is_flag=True, help="will skip seed full refresh")
 @click.pass_context
 def cli(
     ctx,
     count: int,
     persist: bool,
-    no_seed: bool,
+    seed: bool,
     models: Optional[Tuple] = tuple(),
     select: Optional[Tuple] = tuple(),
 ):
     """Consecutive run-test of the DBT repo. `count` is the number of run/test cycles to execute, defaults to 2"""
 
     def add_models(command: str) -> str:
         if models:
@@ -42,15 +42,15 @@
                 add_models("dbt test"),
             )
             * count
         )
 
     def make_cmd():
         commands = []
-        if not no_seed:
+        if seed:
             seed_cmd = "dbt seed --full-refresh"
             commands.append(add_select(seed_cmd))
 
         commands.append(run_test())
 
         if not persist:
             commands.append("dbt run-operation drop_branch_schemas")
```

### Comparing `palm-dbt-0.5.0/palm/plugins/dbt/commands/cmd_dbt.py` & `palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_dbt.py`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.5.0/palm/plugins/dbt/commands/cmd_install.py` & `palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_install.py`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.5.0/palm/plugins/dbt/commands/cmd_model-doc.py` & `palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_model-doc.py`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.5.0/palm/plugins/dbt/commands/cmd_model.py` & `palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_model.py`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.5.0/palm/plugins/dbt/commands/cmd_prod-artifacts.py` & `palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_prod-artifacts.py`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.5.0/palm/plugins/dbt/commands/cmd_run.py` & `palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_run.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,24 +17,24 @@
 @click.option("--defer", is_flag=True, help="See dbt docs on defer flag")
 @click.option("--iterative", is_flag=True, help="Iterative stateful dbt run")
 @click.option(
     "--full-refresh",
     is_flag=True,
     help="Will perform a full refresh on incremental models",
 )
-@click.option("--no-seed", is_flag=True, help="Will skip seed full refresh")
+@click.option("--seed", is_flag=True, help="Run dbt seed before dbt run")
 @click.pass_obj
 def cli(
     environment,
     no_fail_fast: bool,
     clean: bool,
     full_refresh: bool,
     iterative: bool,
     defer: bool,
-    no_seed: bool,
+    seed: bool,
     models: Optional[Tuple] = tuple(),
     select: Optional[Tuple] = tuple(),
     exclude: Optional[Tuple] = tuple(),
     vars: Optional[str] = None,
 ):
     """Runs the DBT repo."""
     stateful = iterative or defer
@@ -58,15 +58,15 @@
 
     # --select and --models are interchangeable on dbt >= v1, combine the lists of selections
     targets = list(set(models + select))
 
     run_cmd = build_run_command(
         # Is there a better way to pass these args in?
         full_refresh=full_refresh,
-        no_seed=(no_seed or defer),
+        seed=seed,
         no_fail_fast=(no_fail_fast or iterative),
         targets=targets,
         exclude=exclude,
         defer=defer,
         vars=vars,
     )
 
@@ -79,15 +79,15 @@
 
             if not cycle:
                 break
 
             env_vars = set_env_vars(environment, stateful)
             stateful_run_cmd = build_run_command(
                 targets=["result:error", "result:skipped"],
-                no_seed=iterative,
+                seed=False,
                 no_fail_fast=iterative,
             )
             success, msg = environment.run_in_docker(stateful_run_cmd, env_vars)
 
     click.secho(msg, fg="green" if success else "red")
 
     if clean:
@@ -95,26 +95,26 @@
             "dbt run-operation drop_branch_schemas && dbt clean", env_vars
         )
         click.secho(msg, fg="green" if success else "red")
 
 
 def build_run_command(
     full_refresh: bool = False,
-    no_seed: bool = True,
+    seed: bool = True,
     no_fail_fast: bool = False,
     targets: Optional[list] = None,
     exclude: Optional[Tuple] = None,
     defer: bool = False,
     vars: Optional[str] = None,
 ) -> str:
     cmd = []
     full_refresh_option = " --full-refresh" if full_refresh else ""
 
-    if not no_seed:
-        cmd.append(f"dbt seed{full_refresh_option}")
+    if seed:
+        cmd.append(f"dbt seed --full-refresh")
         cmd.append("&&")
 
     cmd.append(f"dbt run{full_refresh_option}")
     if targets:
         cmd.append("--select")
         cmd.extend(targets)
     if exclude:
```

### Comparing `palm-dbt-0.5.0/palm/plugins/dbt/commands/cmd_snapshot.py` & `palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_snapshot.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import click
 from typing import Optional, Tuple
 from palm.plugins.dbt.dbt_palm_utils import dbt_env_vars
 
 
 @click.command("snapshot")
-@click.option(
-    "--persist", is_flag=True, help="will not drop the test schema at the end"
-)
+@click.option("--clean", is_flag=True, help="Drop the test schema after the run")
 @click.option("--select", multiple=True)
 @click.pass_context
-def cli(ctx, persist: bool, select: Optional[Tuple] = tuple()):
+def cli(ctx, clean: bool, select: Optional[Tuple] = tuple()):
     """Executes the DBT snapshots."""
 
     cmd = "dbt snapshot"
     if select:
         cmd += f" --select " + " ".join(select)
-    if not persist:
+    if clean:
         cmd += " && dbt run-operation drop_branch_schemas"
 
     env_vars = dbt_env_vars(ctx.obj.palm.branch)
     success, msg = ctx.obj.run_in_docker(cmd, env_vars)
     click.secho(msg, fg="green" if success else "red")
```

### Comparing `palm-dbt-0.5.0/palm/plugins/dbt/commands/cmd_test.py` & `palm-dbt-0.6.0/palm/plugins/dbt/commands/cmd_test.py`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.5.0/palm/plugins/dbt/dbt_containerizer.py` & `palm-dbt-0.6.0/palm/plugins/dbt/dbt_containerizer.py`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.5.0/palm/plugins/dbt/dbt_palm_utils.py` & `palm-dbt-0.6.0/palm/plugins/dbt/dbt_palm_utils.py`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.5.0/palm/plugins/dbt/dbt_plugin.py` & `palm-dbt-0.6.0/palm/plugins/dbt/dbt_plugin.py`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.5.0/palm/plugins/dbt/macros/drop_branch_schemas.sql` & `palm-dbt-0.6.0/palm/plugins/dbt/macros/drop_branch_schemas.sql`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.5.0/palm/plugins/dbt/macros/generate_schema_name.sql` & `palm-dbt-0.6.0/palm/plugins/dbt/macros/generate_schema_name.sql`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.5.0/palm/plugins/dbt/model_template/ref_files/ref_file_readme.md` & `palm-dbt-0.6.0/palm/plugins/dbt/model_template/ref_files/ref_file_readme.md`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.5.0/palm/plugins/dbt/parsers/__init__.py` & `palm-dbt-0.6.0/palm/plugins/dbt/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.5.0/palm/plugins/dbt/parsers/project_parser.py` & `palm-dbt-0.6.0/palm/plugins/dbt/parsers/project_parser.py`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.5.0/palm/plugins/dbt/plugin_config.py` & `palm-dbt-0.6.0/palm/plugins/dbt/plugin_config.py`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.5.0/palm/plugins/dbt/sql_to_dbt.py` & `palm-dbt-0.6.0/palm/plugins/dbt/sql_to_dbt.py`

 * *Files identical despite different names*

### Comparing `palm-dbt-0.5.0/palm_dbt.egg-info/PKG-INFO` & `palm-dbt-0.6.0/palm_dbt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palm-dbt
-Version: 0.5.0
+Version: 0.6.0
 Summary: dbt extension for Palm CLI
 Home-page: https://github.com/palmetto/palm-dbt
 Author: Palmetto - Data & Analytics team
 Author-email: data-analytics-team@palmetto.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `palm-dbt-0.5.0/palm_dbt.egg-info/SOURCES.txt` & `palm-dbt-0.6.0/palm_dbt.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 palm/plugins/dbt/commands/cmd_dbt-docs.py
 palm/plugins/dbt/commands/cmd_dbt.py
 palm/plugins/dbt/commands/cmd_install.py
 palm/plugins/dbt/commands/cmd_model-doc.py
 palm/plugins/dbt/commands/cmd_model.py
 palm/plugins/dbt/commands/cmd_prod-artifacts.py
 palm/plugins/dbt/commands/cmd_run.py
+palm/plugins/dbt/commands/cmd_seed.py
 palm/plugins/dbt/commands/cmd_shell.py
 palm/plugins/dbt/commands/cmd_snapshot.py
 palm/plugins/dbt/commands/cmd_test.py
 palm/plugins/dbt/macros/drop_branch_schemas.sql
 palm/plugins/dbt/macros/generate_schema_name.sql
 palm/plugins/dbt/model_template/docs/base_model.md
 palm/plugins/dbt/model_template/docs/template-config.yaml
```

### Comparing `palm-dbt-0.5.0/setup.py` & `palm-dbt-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 # User-friendly description from README.md
 this_directory = Path(__file__).parent
 long_description = Path(this_directory, 'README.md').read_text()
 
 setup(
     name='palm-dbt',
-    version='0.5.0',
+    version='0.6.0',
     description='dbt extension for Palm CLI',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Palmetto - Data & Analytics team',
     author_email='data-analytics-team@palmetto.com',
     url='https://github.com/palmetto/palm-dbt',
     packages=find_namespace_packages(include=['palm', 'palm.*']),
```

