# Comparing `tmp/cdktf-cdktf-provider-snowflake-6.0.3.tar.gz` & `tmp/cdktf-cdktf-provider-snowflake-6.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-snowflake-6.0.3.tar", last modified: Thu Jun  1 11:14:03 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-snowflake-6.0.4.tar", last modified: Fri Jun  2 14:21:19 2023, max compression
```

## Comparing `cdktf-cdktf-provider-snowflake-6.0.3.tar` & `cdktf-cdktf-provider-snowflake-6.0.4.tar`

### file list

```diff
@@ -1,243 +1,243 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.488927 cdktf-cdktf-provider-snowflake-6.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-06-01 11:14:03.488927 cdktf-cdktf-provider-snowflake-6.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 11:14:03.488927 cdktf-cdktf-provider-snowflake-6.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.456927 cdktf-cdktf-provider-snowflake-6.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.464927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.468927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   833322 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/_jsii/provider-snowflake@6.0.3.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.468927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/account/
--rw-r--r--   0 runner    (1001) docker     (123)    51486 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/account/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.468927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/account_grant/
--rw-r--r--   0 runner    (1001) docker     (123)    28660 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/account_grant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.468927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/account_parameter/
--rw-r--r--   0 runner    (1001) docker     (123)    20584 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/account_parameter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.468927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/alert/
--rw-r--r--   0 runner    (1001) docker     (123)    53003 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/alert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.468927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/api_integration/
--rw-r--r--   0 runner    (1001) docker     (123)    50596 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/api_integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.468927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_accounts/
--rw-r--r--   0 runner    (1001) docker     (123)    30561 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_accounts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.468927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_alerts/
--rw-r--r--   0 runner    (1001) docker     (123)    33105 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_alerts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.468927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_current_account/
--rw-r--r--   0 runner    (1001) docker     (123)    16458 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_current_account/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.468927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_current_role/
--rw-r--r--   0 runner    (1001) docker     (123)    16057 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_current_role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.468927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_database/
--rw-r--r--   0 runner    (1001) docker     (123)    19373 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.468927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_database_roles/
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_database_roles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.468927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_databases/
--rw-r--r--   0 runner    (1001) docker     (123)    36334 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_databases/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.468927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_external_functions/
--rw-r--r--   0 runner    (1001) docker     (123)    30799 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_external_functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.468927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_external_tables/
--rw-r--r--   0 runner    (1001) docker     (123)    30372 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_external_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.468927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_failover_groups/
--rw-r--r--   0 runner    (1001) docker     (123)    31015 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_failover_groups/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.472927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_file_formats/
--rw-r--r--   0 runner    (1001) docker     (123)    30296 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_file_formats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.472927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_functions/
--rw-r--r--   0 runner    (1001) docker     (123)    30330 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.472927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_grants/
--rw-r--r--   0 runner    (1001) docker     (123)    92827 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_grants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.472927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_masking_policies/
--rw-r--r--   0 runner    (1001) docker     (123)    30609 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_masking_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.472927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_materialized_views/
--rw-r--r--   0 runner    (1001) docker     (123)    30588 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_materialized_views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.472927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_parameters/
--rw-r--r--   0 runner    (1001) docker     (123)    40527 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_parameters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.472927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_pipes/
--rw-r--r--   0 runner    (1001) docker     (123)    29752 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_pipes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.472927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_procedures/
--rw-r--r--   0 runner    (1001) docker     (123)    30410 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_procedures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.472927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_resource_monitors/
--rw-r--r--   0 runner    (1001) docker     (123)    25984 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_resource_monitors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.472927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_role/
--rw-r--r--   0 runner    (1001) docker     (123)    17958 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.472927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_roles/
--rw-r--r--   0 runner    (1001) docker     (123)    27427 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_roles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.472927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_row_access_policies/
--rw-r--r--   0 runner    (1001) docker     (123)    30638 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_row_access_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.472927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_schemas/
--rw-r--r--   0 runner    (1001) docker     (123)    27417 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.472927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_sequences/
--rw-r--r--   0 runner    (1001) docker     (123)    29937 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_sequences/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.472927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_shares/
--rw-r--r--   0 runner    (1001) docker     (123)    27838 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_shares/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.472927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_stages/
--rw-r--r--   0 runner    (1001) docker     (123)    29854 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_stages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.472927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_storage_integrations/
--rw-r--r--   0 runner    (1001) docker     (123)    26196 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_storage_integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.472927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_streams/
--rw-r--r--   0 runner    (1001) docker     (123)    29917 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_streams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.472927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_system_generate_scim_access_token/
--rw-r--r--   0 runner    (1001) docker     (123)    19097 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_system_generate_scim_access_token/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.472927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_system_get_aws_sns_iam_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    19142 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_system_get_aws_sns_iam_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.472927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_system_get_privatelink_config/
--rw-r--r--   0 runner    (1001) docker     (123)    17956 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_system_get_privatelink_config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.472927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_system_get_snowflake_platform_info/
--rw-r--r--   0 runner    (1001) docker     (123)    16805 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_system_get_snowflake_platform_info/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.472927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_tables/
--rw-r--r--   0 runner    (1001) docker     (123)    29651 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.472927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_tasks/
--rw-r--r--   0 runner    (1001) docker     (123)    29746 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.472927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_users/
--rw-r--r--   0 runner    (1001) docker     (123)    29544 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_users/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.472927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_views/
--rw-r--r--   0 runner    (1001) docker     (123)    29571 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.476927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_warehouses/
--rw-r--r--   0 runner    (1001) docker     (123)    25882 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_warehouses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.476927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/database/
--rw-r--r--   0 runner    (1001) docker     (123)    68913 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.476927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/database_grant/
--rw-r--r--   0 runner    (1001) docker     (123)    36715 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/database_grant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.476927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/database_role/
--rw-r--r--   0 runner    (1001) docker     (123)    22457 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/database_role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.476927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/email_notification_integration/
--rw-r--r--   0 runner    (1001) docker     (123)    26164 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/email_notification_integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.476927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/external_function/
--rw-r--r--   0 runner    (1001) docker     (123)    91183 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/external_function/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.476927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/external_oauth_integration/
--rw-r--r--   0 runner    (1001) docker     (123)    63121 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/external_oauth_integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.476927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/external_table/
--rw-r--r--   0 runner    (1001) docker     (123)    87720 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/external_table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.476927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/external_table_grant/
--rw-r--r--   0 runner    (1001) docker     (123)    50996 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/external_table_grant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.476927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/failover_group/
--rw-r--r--   0 runner    (1001) docker     (123)    73668 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/failover_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.476927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/failover_group_grant/
--rw-r--r--   0 runner    (1001) docker     (123)    34768 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/failover_group_grant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.476927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/file_format/
--rw-r--r--   0 runner    (1001) docker     (123)   122928 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/file_format/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.476927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/file_format_grant/
--rw-r--r--   0 runner    (1001) docker     (123)    47803 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/file_format_grant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.476927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/function_grant/
--rw-r--r--   0 runner    (1001) docker     (123)    53654 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/function_grant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.476927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/function_resource/
--rw-r--r--   0 runner    (1001) docker     (123)    72237 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/function_resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.476927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/integration_grant/
--rw-r--r--   0 runner    (1001) docker     (123)    34494 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/integration_grant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.476927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/managed_account/
--rw-r--r--   0 runner    (1001) docker     (123)    28535 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/managed_account/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.476927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/masking_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    62887 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/masking_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.476927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/masking_policy_grant/
--rw-r--r--   0 runner    (1001) docker     (123)    39744 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/masking_policy_grant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.476927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/materialized_view/
--rw-r--r--   0 runner    (1001) docker     (123)    56899 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/materialized_view/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.476927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/materialized_view_grant/
--rw-r--r--   0 runner    (1001) docker     (123)    51780 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/materialized_view_grant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.476927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/network_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    26480 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/network_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.480927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/network_policy_attachment/
--rw-r--r--   0 runner    (1001) docker     (123)    26500 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/network_policy_attachment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.480927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/notification_integration/
--rw-r--r--   0 runner    (1001) docker     (123)    56592 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/notification_integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.480927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/oauth_integration/
--rw-r--r--   0 runner    (1001) docker     (123)    46460 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/oauth_integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.480927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/object_parameter/
--rw-r--r--   0 runner    (1001) docker     (123)    47387 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/object_parameter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.480927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/password_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    59456 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/password_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.480927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/pipe/
--rw-r--r--   0 runner    (1001) docker     (123)    38285 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/pipe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.480927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/pipe_grant/
--rw-r--r--   0 runner    (1001) docker     (123)    43200 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/pipe_grant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.480927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/procedure/
--rw-r--r--   0 runner    (1001) docker     (123)    68263 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/procedure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.480927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/procedure_grant/
--rw-r--r--   0 runner    (1001) docker     (123)    53539 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/procedure_grant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.480927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    68644 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.480927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/resource_monitor/
--rw-r--r--   0 runner    (1001) docker     (123)    53681 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/resource_monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.480927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/resource_monitor_grant/
--rw-r--r--   0 runner    (1001) docker     (123)    31199 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/resource_monitor_grant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.480927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/role/
--rw-r--r--   0 runner    (1001) docker     (123)    40187 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.480927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/role_grants/
--rw-r--r--   0 runner    (1001) docker     (123)    26777 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/role_grants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.480927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/role_ownership_grant/
--rw-r--r--   0 runner    (1001) docker     (123)    27050 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/role_ownership_grant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.480927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/row_access_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    31383 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/row_access_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.480927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/row_access_policy_grant/
--rw-r--r--   0 runner    (1001) docker     (123)    40049 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/row_access_policy_grant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.480927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/saml_integration/
--rw-r--r--   0 runner    (1001) docker     (123)    69478 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/saml_integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.480927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/schema/
--rw-r--r--   0 runner    (1001) docker     (123)    53281 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.480927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/schema_grant/
--rw-r--r--   0 runner    (1001) docker     (123)    46687 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/schema_grant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.484927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/scim_integration/
--rw-r--r--   0 runner    (1001) docker     (123)    27127 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/scim_integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.484927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/sequence/
--rw-r--r--   0 runner    (1001) docker     (123)    27376 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.484927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/sequence_grant/
--rw-r--r--   0 runner    (1001) docker     (123)    47401 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/sequence_grant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.484927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/session_parameter/
--rw-r--r--   0 runner    (1001) docker     (123)    26212 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/session_parameter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.484927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/share/
--rw-r--r--   0 runner    (1001) docker     (123)    23017 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/share/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.484927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/stage/
--rw-r--r--   0 runner    (1001) docker     (123)    68064 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/stage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.484927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/stage_grant/
--rw-r--r--   0 runner    (1001) docker     (123)    46831 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/stage_grant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.484927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/storage_integration/
--rw-r--r--   0 runner    (1001) docker     (123)    44003 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/storage_integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.484927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/stream/
--rw-r--r--   0 runner    (1001) docker     (123)    41531 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/stream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.484927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/stream_grant/
--rw-r--r--   0 runner    (1001) docker     (123)    47103 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/stream_grant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.484927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/table/
--rw-r--r--   0 runner    (1001) docker     (123)   110381 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.484927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/table_column_masking_policy_application/
--rw-r--r--   0 runner    (1001) docker     (123)    23627 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/table_column_masking_policy_application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.484927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/table_constraint/
--rw-r--r--   0 runner    (1001) docker     (123)    71299 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/table_constraint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.484927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/table_grant/
--rw-r--r--   0 runner    (1001) docker     (123)    49962 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/table_grant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.484927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/tag/
--rw-r--r--   0 runner    (1001) docker     (123)    26987 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/tag/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.484927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/tag_association/
--rw-r--r--   0 runner    (1001) docker     (123)    57674 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/tag_association/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.484927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/tag_grant/
--rw-r--r--   0 runner    (1001) docker     (123)    38475 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/tag_grant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.484927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/tag_masking_policy_association/
--rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/tag_masking_policy_association/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.484927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/task/
--rw-r--r--   0 runner    (1001) docker     (123)    58343 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.484927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/task_grant/
--rw-r--r--   0 runner    (1001) docker     (123)    46805 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/task_grant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.484927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/user/
--rw-r--r--   0 runner    (1001) docker     (123)    80645 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.484927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/user_grant/
--rw-r--r--   0 runner    (1001) docker     (123)    30140 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/user_grant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.484927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/user_ownership_grant/
--rw-r--r--   0 runner    (1001) docker     (123)    27050 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/user_ownership_grant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.484927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/user_public_keys/
--rw-r--r--   0 runner    (1001) docker     (123)    23946 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/user_public_keys/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.488927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/view/
--rw-r--r--   0 runner    (1001) docker     (123)    56582 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/view/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.488927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/view_grant/
--rw-r--r--   0 runner    (1001) docker     (123)    49813 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/view_grant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.488927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/warehouse/
--rw-r--r--   0 runner    (1001) docker     (123)    68315 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/warehouse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.488927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/warehouse_grant/
--rw-r--r--   0 runner    (1001) docker     (123)    34277 2023-06-01 11:13:52.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/warehouse_grant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:14:03.468927 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-06-01 11:14:03.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-06-01 11:14:03.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 11:14:03.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 11:14:03.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-01 11:14:03.000000 cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.925824 cdktf-cdktf-provider-snowflake-6.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-06-02 14:21:19.921824 cdktf-cdktf-provider-snowflake-6.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 14:21:19.925824 cdktf-cdktf-provider-snowflake-6.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.893823 cdktf-cdktf-provider-snowflake-6.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.901824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.905824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   833306 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/_jsii/provider-snowflake@6.0.4.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.905824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/account/
+-rw-r--r--   0 runner    (1001) docker     (123)    51486 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/account/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.905824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/account_grant/
+-rw-r--r--   0 runner    (1001) docker     (123)    28660 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/account_grant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.905824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/account_parameter/
+-rw-r--r--   0 runner    (1001) docker     (123)    20584 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/account_parameter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.905824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/alert/
+-rw-r--r--   0 runner    (1001) docker     (123)    53003 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/alert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.905824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/api_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)    50596 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/api_integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.905824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)    30561 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_accounts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.905824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_alerts/
+-rw-r--r--   0 runner    (1001) docker     (123)    33105 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_alerts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.905824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_current_account/
+-rw-r--r--   0 runner    (1001) docker     (123)    16458 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_current_account/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.905824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_current_role/
+-rw-r--r--   0 runner    (1001) docker     (123)    16057 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_current_role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.905824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_database/
+-rw-r--r--   0 runner    (1001) docker     (123)    19373 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.905824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_database_roles/
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_database_roles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.905824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_databases/
+-rw-r--r--   0 runner    (1001) docker     (123)    36334 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_databases/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.905824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_external_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)    30799 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_external_functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.905824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_external_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)    30372 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_external_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.905824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_failover_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)    31015 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_failover_groups/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.909824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_file_formats/
+-rw-r--r--   0 runner    (1001) docker     (123)    30296 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_file_formats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.909824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)    30330 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.909824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_grants/
+-rw-r--r--   0 runner    (1001) docker     (123)    92827 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_grants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.909824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_masking_policies/
+-rw-r--r--   0 runner    (1001) docker     (123)    30609 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_masking_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.909824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_materialized_views/
+-rw-r--r--   0 runner    (1001) docker     (123)    30588 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_materialized_views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.909824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)    40527 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_parameters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.909824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_pipes/
+-rw-r--r--   0 runner    (1001) docker     (123)    29752 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_pipes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.909824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_procedures/
+-rw-r--r--   0 runner    (1001) docker     (123)    30410 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_procedures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.909824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_resource_monitors/
+-rw-r--r--   0 runner    (1001) docker     (123)    25984 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_resource_monitors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.909824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_role/
+-rw-r--r--   0 runner    (1001) docker     (123)    17958 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.909824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_roles/
+-rw-r--r--   0 runner    (1001) docker     (123)    27427 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_roles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.909824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_row_access_policies/
+-rw-r--r--   0 runner    (1001) docker     (123)    30638 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_row_access_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.909824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)    27417 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.909824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_sequences/
+-rw-r--r--   0 runner    (1001) docker     (123)    29937 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_sequences/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.909824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_shares/
+-rw-r--r--   0 runner    (1001) docker     (123)    27838 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_shares/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.909824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_stages/
+-rw-r--r--   0 runner    (1001) docker     (123)    29854 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_stages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.909824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_storage_integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    26196 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_storage_integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.909824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_streams/
+-rw-r--r--   0 runner    (1001) docker     (123)    29917 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_streams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.909824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_system_generate_scim_access_token/
+-rw-r--r--   0 runner    (1001) docker     (123)    19097 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_system_generate_scim_access_token/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.909824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_system_get_aws_sns_iam_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    19142 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_system_get_aws_sns_iam_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.909824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_system_get_privatelink_config/
+-rw-r--r--   0 runner    (1001) docker     (123)    17956 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_system_get_privatelink_config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.909824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_system_get_snowflake_platform_info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16805 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_system_get_snowflake_platform_info/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.909824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)    29651 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.909824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)    29746 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.909824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_users/
+-rw-r--r--   0 runner    (1001) docker     (123)    29544 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_users/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.909824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_views/
+-rw-r--r--   0 runner    (1001) docker     (123)    29571 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.909824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_warehouses/
+-rw-r--r--   0 runner    (1001) docker     (123)    25882 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_warehouses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.913824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/database/
+-rw-r--r--   0 runner    (1001) docker     (123)    68913 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.913824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/database_grant/
+-rw-r--r--   0 runner    (1001) docker     (123)    36715 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/database_grant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.913824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/database_role/
+-rw-r--r--   0 runner    (1001) docker     (123)    22457 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/database_role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.913824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/email_notification_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)    26164 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/email_notification_integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.913824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/external_function/
+-rw-r--r--   0 runner    (1001) docker     (123)    91183 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/external_function/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.913824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/external_oauth_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)    63121 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/external_oauth_integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.913824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/external_table/
+-rw-r--r--   0 runner    (1001) docker     (123)    87720 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/external_table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.913824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/external_table_grant/
+-rw-r--r--   0 runner    (1001) docker     (123)    50996 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/external_table_grant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.913824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/failover_group/
+-rw-r--r--   0 runner    (1001) docker     (123)    73668 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/failover_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.913824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/failover_group_grant/
+-rw-r--r--   0 runner    (1001) docker     (123)    34768 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/failover_group_grant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.913824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/file_format/
+-rw-r--r--   0 runner    (1001) docker     (123)   122928 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/file_format/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.913824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/file_format_grant/
+-rw-r--r--   0 runner    (1001) docker     (123)    47803 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/file_format_grant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.913824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/function_grant/
+-rw-r--r--   0 runner    (1001) docker     (123)    53654 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/function_grant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.913824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/function_resource/
+-rw-r--r--   0 runner    (1001) docker     (123)    72237 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/function_resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.913824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/integration_grant/
+-rw-r--r--   0 runner    (1001) docker     (123)    34494 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/integration_grant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.913824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/managed_account/
+-rw-r--r--   0 runner    (1001) docker     (123)    28535 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/managed_account/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.913824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/masking_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    62887 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/masking_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.913824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/masking_policy_grant/
+-rw-r--r--   0 runner    (1001) docker     (123)    39744 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/masking_policy_grant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.913824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/materialized_view/
+-rw-r--r--   0 runner    (1001) docker     (123)    56899 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/materialized_view/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.913824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/materialized_view_grant/
+-rw-r--r--   0 runner    (1001) docker     (123)    51780 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/materialized_view_grant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.913824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/network_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    26480 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/network_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.913824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/network_policy_attachment/
+-rw-r--r--   0 runner    (1001) docker     (123)    26500 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/network_policy_attachment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.913824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/notification_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)    56592 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/notification_integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.917824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/oauth_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)    46460 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/oauth_integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.917824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/object_parameter/
+-rw-r--r--   0 runner    (1001) docker     (123)    47387 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/object_parameter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.917824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/password_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    59456 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/password_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.917824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/pipe/
+-rw-r--r--   0 runner    (1001) docker     (123)    38285 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/pipe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.917824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/pipe_grant/
+-rw-r--r--   0 runner    (1001) docker     (123)    43200 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/pipe_grant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.917824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/procedure/
+-rw-r--r--   0 runner    (1001) docker     (123)    68263 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/procedure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.917824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/procedure_grant/
+-rw-r--r--   0 runner    (1001) docker     (123)    53539 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/procedure_grant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.917824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    68644 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.917824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/resource_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)    53681 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/resource_monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.917824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/resource_monitor_grant/
+-rw-r--r--   0 runner    (1001) docker     (123)    31199 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/resource_monitor_grant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.917824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/role/
+-rw-r--r--   0 runner    (1001) docker     (123)    40187 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.917824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/role_grants/
+-rw-r--r--   0 runner    (1001) docker     (123)    26777 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/role_grants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.917824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/role_ownership_grant/
+-rw-r--r--   0 runner    (1001) docker     (123)    27050 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/role_ownership_grant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.917824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/row_access_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    31383 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/row_access_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.917824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/row_access_policy_grant/
+-rw-r--r--   0 runner    (1001) docker     (123)    40049 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/row_access_policy_grant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.917824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/saml_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)    69478 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/saml_integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.917824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)    53281 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.917824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/schema_grant/
+-rw-r--r--   0 runner    (1001) docker     (123)    46687 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/schema_grant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.917824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/scim_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)    27127 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/scim_integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.917824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/sequence/
+-rw-r--r--   0 runner    (1001) docker     (123)    27376 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.917824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/sequence_grant/
+-rw-r--r--   0 runner    (1001) docker     (123)    47401 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/sequence_grant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.917824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/session_parameter/
+-rw-r--r--   0 runner    (1001) docker     (123)    26212 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/session_parameter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.917824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/share/
+-rw-r--r--   0 runner    (1001) docker     (123)    23017 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/share/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.917824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/stage/
+-rw-r--r--   0 runner    (1001) docker     (123)    68064 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/stage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.921824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/stage_grant/
+-rw-r--r--   0 runner    (1001) docker     (123)    46831 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/stage_grant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.921824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/storage_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)    44003 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/storage_integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.921824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)    41531 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/stream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.921824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/stream_grant/
+-rw-r--r--   0 runner    (1001) docker     (123)    47103 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/stream_grant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.921824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/table/
+-rw-r--r--   0 runner    (1001) docker     (123)   110381 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.921824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/table_column_masking_policy_application/
+-rw-r--r--   0 runner    (1001) docker     (123)    23627 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/table_column_masking_policy_application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.921824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/table_constraint/
+-rw-r--r--   0 runner    (1001) docker     (123)    71299 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/table_constraint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.921824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/table_grant/
+-rw-r--r--   0 runner    (1001) docker     (123)    49962 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/table_grant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.921824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/tag/
+-rw-r--r--   0 runner    (1001) docker     (123)    26987 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/tag/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.921824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/tag_association/
+-rw-r--r--   0 runner    (1001) docker     (123)    57674 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/tag_association/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.921824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/tag_grant/
+-rw-r--r--   0 runner    (1001) docker     (123)    38475 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/tag_grant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.921824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/tag_masking_policy_association/
+-rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/tag_masking_policy_association/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.921824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/task/
+-rw-r--r--   0 runner    (1001) docker     (123)    58343 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.921824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/task_grant/
+-rw-r--r--   0 runner    (1001) docker     (123)    46805 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/task_grant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.921824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    80645 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.921824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/user_grant/
+-rw-r--r--   0 runner    (1001) docker     (123)    30140 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/user_grant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.921824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/user_ownership_grant/
+-rw-r--r--   0 runner    (1001) docker     (123)    27050 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/user_ownership_grant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.921824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/user_public_keys/
+-rw-r--r--   0 runner    (1001) docker     (123)    23946 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/user_public_keys/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.921824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/view/
+-rw-r--r--   0 runner    (1001) docker     (123)    56582 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/view/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.921824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/view_grant/
+-rw-r--r--   0 runner    (1001) docker     (123)    49813 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/view_grant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.921824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/warehouse/
+-rw-r--r--   0 runner    (1001) docker     (123)    68315 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/warehouse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.921824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/warehouse_grant/
+-rw-r--r--   0 runner    (1001) docker     (123)    34277 2023-06-02 14:21:08.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/warehouse_grant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:21:19.905824 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-06-02 14:21:19.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-06-02 14:21:19.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:21:19.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-02 14:21:19.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-02 14:21:19.000000 cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/LICENSE` & `cdktf-cdktf-provider-snowflake-6.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/PKG-INFO` & `cdktf-cdktf-provider-snowflake-6.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-snowflake
-Version: 6.0.3
+Version: 6.0.4
 Summary: Prebuilt snowflake Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-snowflake.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-snowflake.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/README.md` & `cdktf-cdktf-provider-snowflake-6.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/setup.py` & `cdktf-cdktf-provider-snowflake-6.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-snowflake",
-    "version": "6.0.3",
+    "version": "6.0.4",
     "description": "Prebuilt snowflake Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-snowflake.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -133,23 +133,23 @@
         "cdktf_cdktf_provider_snowflake.view",
         "cdktf_cdktf_provider_snowflake.view_grant",
         "cdktf_cdktf_provider_snowflake.warehouse",
         "cdktf_cdktf_provider_snowflake.warehouse_grant"
     ],
     "package_data": {
         "cdktf_cdktf_provider_snowflake._jsii": [
-            "provider-snowflake@6.0.3.jsii.tgz"
+            "provider-snowflake@6.0.4.jsii.tgz"
         ],
         "cdktf_cdktf_provider_snowflake": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "cdktf>=0.16.0, <0.17.0",
+        "cdktf>=0.16.3, <0.17.0",
         "constructs>=10.0.0, <11.0.0",
         "jsii>=1.81.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/account/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/account/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/account_grant/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/account_grant/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/account_parameter/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/account_parameter/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/alert/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/alert/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/api_integration/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/api_integration/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_accounts/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_alerts/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_alerts/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_current_account/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_current_account/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_current_role/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_current_role/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_database/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_database/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_database_roles/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_database_roles/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_databases/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_databases/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_external_functions/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_external_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_external_tables/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_external_tables/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_failover_groups/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_failover_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_file_formats/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_file_formats/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_functions/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_grants/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_grants/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_masking_policies/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_masking_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_materialized_views/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_materialized_views/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_parameters/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_pipes/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_pipes/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_procedures/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_procedures/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_resource_monitors/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_resource_monitors/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_role/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_role/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_roles/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_roles/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_row_access_policies/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_row_access_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_schemas/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_sequences/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_sequences/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_shares/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_shares/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_stages/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_stages/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_storage_integrations/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_storage_integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_streams/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_streams/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_system_generate_scim_access_token/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_system_generate_scim_access_token/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_system_get_aws_sns_iam_policy/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_system_get_aws_sns_iam_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_system_get_privatelink_config/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_system_get_privatelink_config/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_system_get_snowflake_platform_info/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_system_get_snowflake_platform_info/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_tables/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_tables/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_tasks/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_users/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_users/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_views/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_views/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/data_snowflake_warehouses/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/data_snowflake_warehouses/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/database/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/database/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/database_grant/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/database_grant/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/database_role/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/database_role/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/email_notification_integration/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/email_notification_integration/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/external_function/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/external_function/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/external_oauth_integration/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/external_oauth_integration/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/external_table/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/external_table/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/external_table_grant/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/external_table_grant/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/failover_group/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/failover_group/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/failover_group_grant/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/failover_group_grant/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/file_format/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/file_format/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/file_format_grant/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/file_format_grant/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/function_grant/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/function_grant/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/function_resource/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/function_resource/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/integration_grant/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/integration_grant/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/managed_account/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/managed_account/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/masking_policy/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/masking_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/masking_policy_grant/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/masking_policy_grant/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/materialized_view/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/materialized_view/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/materialized_view_grant/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/materialized_view_grant/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/network_policy/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/network_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/network_policy_attachment/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/network_policy_attachment/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/notification_integration/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/notification_integration/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/oauth_integration/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/oauth_integration/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/object_parameter/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/object_parameter/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/password_policy/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/password_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/pipe/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/pipe_grant/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/pipe_grant/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/procedure/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/procedure/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/procedure_grant/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/procedure_grant/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/provider/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/resource_monitor/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/resource_monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/resource_monitor_grant/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/resource_monitor_grant/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/role/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/role/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/role_grants/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/role_grants/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/role_ownership_grant/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/role_ownership_grant/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/row_access_policy/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/row_access_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/row_access_policy_grant/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/row_access_policy_grant/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/saml_integration/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/saml_integration/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/schema/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/schema_grant/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/schema_grant/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/scim_integration/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/scim_integration/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/sequence/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/sequence/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/sequence_grant/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/sequence_grant/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/session_parameter/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/session_parameter/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/share/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/share/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/stage/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/stage/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/stage_grant/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/stage_grant/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/storage_integration/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/storage_integration/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/stream/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/stream_grant/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/stream_grant/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/table/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/table/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/table_column_masking_policy_application/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/table_column_masking_policy_application/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/table_constraint/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/table_constraint/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/table_grant/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/table_grant/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/tag/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/tag/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/tag_association/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/tag_association/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/tag_grant/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/tag_grant/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/tag_masking_policy_association/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/tag_masking_policy_association/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/task/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/task/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/task_grant/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/task_grant/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/user/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/user/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/user_grant/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/user_grant/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/user_ownership_grant/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/user_ownership_grant/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/user_public_keys/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/user_public_keys/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/view/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/view/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/view_grant/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/view_grant/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/warehouse/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/warehouse/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake/warehouse_grant/__init__.py` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake/warehouse_grant/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake.egg-info/PKG-INFO` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-snowflake
-Version: 6.0.3
+Version: 6.0.4
 Summary: Prebuilt snowflake Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-snowflake.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-snowflake.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-snowflake-6.0.3/src/cdktf_cdktf_provider_snowflake.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-snowflake-6.0.4/src/cdktf_cdktf_provider_snowflake.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_snowflake/py.typed
 src/cdktf_cdktf_provider_snowflake.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_snowflake.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_snowflake.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_snowflake.egg-info/requires.txt
 src/cdktf_cdktf_provider_snowflake.egg-info/top_level.txt
 src/cdktf_cdktf_provider_snowflake/_jsii/__init__.py
-src/cdktf_cdktf_provider_snowflake/_jsii/provider-snowflake@6.0.3.jsii.tgz
+src/cdktf_cdktf_provider_snowflake/_jsii/provider-snowflake@6.0.4.jsii.tgz
 src/cdktf_cdktf_provider_snowflake/account/__init__.py
 src/cdktf_cdktf_provider_snowflake/account_grant/__init__.py
 src/cdktf_cdktf_provider_snowflake/account_parameter/__init__.py
 src/cdktf_cdktf_provider_snowflake/alert/__init__.py
 src/cdktf_cdktf_provider_snowflake/api_integration/__init__.py
 src/cdktf_cdktf_provider_snowflake/data_snowflake_accounts/__init__.py
 src/cdktf_cdktf_provider_snowflake/data_snowflake_alerts/__init__.py
```

