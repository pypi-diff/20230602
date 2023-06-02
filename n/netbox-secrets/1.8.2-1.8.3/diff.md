# Comparing `tmp/netbox-secrets-1.8.2.tar.gz` & `tmp/netbox-secrets-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-secrets-1.8.2.tar", last modified: Thu May 25 16:36:13 2023, max compression
+gzip compressed data, was "netbox-secrets-1.8.3.tar", last modified: Fri Jun  2 15:07:56 2023, max compression
```

## Comparing `netbox-secrets-1.8.2.tar` & `netbox-secrets-1.8.3.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:13.880566 netbox-secrets-1.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-25 16:36:13.880566 netbox-secrets-1.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:13.872565 netbox-secrets-1.8.2/netbox_secrets/
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:13.872565 netbox-secrets-1.8.2/netbox_secrets/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/api/nested_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    12415 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/filtersets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:13.876565 netbox-secrets-1.8.2/netbox_secrets/forms/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/forms/bulk_edit.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/forms/bulk_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/forms/filterset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/forms/model_forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:13.876565 netbox-secrets-1.8.2/netbox_secrets/graphql/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/graphql/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/graphql/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/hashers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:13.876565 netbox-secrets-1.8.2/netbox_secrets/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/migrations/0002_populate_userkeys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/migrations/0003_populate_secretroles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/migrations/0004_populate_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/migrations/0005_alter_secret_custom_field_data_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/migrations/0006_alter_userkey_created_alter_userkey_last_updated.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/migrations/0007_secret__object_repr_secret_comments_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:13.876565 netbox-secrets-1.8.2/netbox_secrets/models/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14680 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/models/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/querysets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:13.872565 netbox-secrets-1.8.2/netbox_secrets/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:13.876565 netbox-secrets-1.8.2/netbox_secrets/static/netbox_secrets/
--rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/static/netbox_secrets/secrets.js
--rw-r--r--   0 runner    (1001) docker     (123)    29495 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/static/netbox_secrets/secrets.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:13.872565 netbox-secrets-1.8.2/netbox_secrets/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:13.876565 netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/activate_keys.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:13.876565 netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/inc/
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/inc/private_key_modal.html
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/inc/secret_actions.html
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/inc/secret_add_button.html
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/inc/secrets_panel.html
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/inc/view_tab.html
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/secret.html
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/secret_edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/secretrole.html
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/userkey.html
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/userkey_edit.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:13.880566 netbox-secrets-1.8.2/netbox_secrets/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/tests/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/tests/test_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:13.880566 netbox-secrets-1.8.2/netbox_secrets/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/utils/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/utils/hashers.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:13.872565 netbox-secrets-1.8.2/netbox_secrets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-25 16:36:13.000000 netbox-secrets-1.8.2/netbox_secrets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-25 16:36:13.000000 netbox-secrets-1.8.2/netbox_secrets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:36:13.000000 netbox-secrets-1.8.2/netbox_secrets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:36:13.000000 netbox-secrets-1.8.2/netbox_secrets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-25 16:36:13.000000 netbox-secrets-1.8.2/netbox_secrets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-25 16:36:13.000000 netbox-secrets-1.8.2/netbox_secrets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 16:36:13.880566 netbox-secrets-1.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:56.495597 netbox-secrets-1.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-02 15:07:56.495597 netbox-secrets-1.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:56.487597 netbox-secrets-1.8.3/netbox_secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:56.491597 netbox-secrets-1.8.3/netbox_secrets/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/api/nested_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12415 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/filtersets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:56.491597 netbox-secrets-1.8.3/netbox_secrets/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/forms/bulk_edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/forms/bulk_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/forms/filterset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/forms/model_forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:56.491597 netbox-secrets-1.8.3/netbox_secrets/graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/graphql/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/graphql/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/hashers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:56.491597 netbox-secrets-1.8.3/netbox_secrets/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/migrations/0002_populate_userkeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/migrations/0003_populate_secretroles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/migrations/0004_populate_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/migrations/0005_alter_secret_custom_field_data_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/migrations/0006_alter_userkey_created_alter_userkey_last_updated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/migrations/0007_secret__object_repr_secret_comments_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:56.491597 netbox-secrets-1.8.3/netbox_secrets/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14680 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/models/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/querysets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:56.487597 netbox-secrets-1.8.3/netbox_secrets/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:56.491597 netbox-secrets-1.8.3/netbox_secrets/static/netbox_secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/static/netbox_secrets/secrets.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29495 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/static/netbox_secrets/secrets.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:56.487597 netbox-secrets-1.8.3/netbox_secrets/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:56.495597 netbox-secrets-1.8.3/netbox_secrets/templates/netbox_secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/templates/netbox_secrets/activate_keys.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:56.495597 netbox-secrets-1.8.3/netbox_secrets/templates/netbox_secrets/inc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/templates/netbox_secrets/inc/private_key_modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/templates/netbox_secrets/inc/secret_actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/templates/netbox_secrets/inc/secret_add_button.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/templates/netbox_secrets/inc/secrets_panel.html
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/templates/netbox_secrets/inc/view_tab.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/templates/netbox_secrets/secret.html
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/templates/netbox_secrets/secret_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/templates/netbox_secrets/secretrole.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/templates/netbox_secrets/userkey.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/templates/netbox_secrets/userkey_edit.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:56.495597 netbox-secrets-1.8.3/netbox_secrets/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/tests/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/tests/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:56.495597 netbox-secrets-1.8.3/netbox_secrets/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/utils/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/utils/hashers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/netbox_secrets/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:56.491597 netbox-secrets-1.8.3/netbox_secrets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-02 15:07:56.000000 netbox-secrets-1.8.3/netbox_secrets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-06-02 15:07:56.000000 netbox-secrets-1.8.3/netbox_secrets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 15:07:56.000000 netbox-secrets-1.8.3/netbox_secrets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 15:07:56.000000 netbox-secrets-1.8.3/netbox_secrets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 15:07:56.000000 netbox-secrets-1.8.3/netbox_secrets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-02 15:07:56.000000 netbox-secrets-1.8.3/netbox_secrets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 15:07:56.495597 netbox-secrets-1.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-02 15:07:41.000000 netbox-secrets-1.8.3/setup.py
```

### Comparing `netbox-secrets-1.8.2/LICENSE.md` & `netbox-secrets-1.8.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/README.md` & `netbox-secrets-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/__init__.py` & `netbox-secrets-1.8.3/netbox_secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/admin.py` & `netbox-secrets-1.8.3/netbox_secrets/admin.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/api/nested_serializers.py` & `netbox-secrets-1.8.3/netbox_secrets/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/api/serializers.py` & `netbox-secrets-1.8.3/netbox_secrets/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/api/urls.py` & `netbox-secrets-1.8.3/netbox_secrets/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/api/views.py` & `netbox-secrets-1.8.3/netbox_secrets/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/filtersets.py` & `netbox-secrets-1.8.3/netbox_secrets/filtersets.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 class SecretRoleFilterSet(NetBoxModelFilterSet):
     q = django_filters.CharFilter(
         method='search',
         label='Search',
     )
-    name = django_filters.ModelMultipleChoiceFilter(queryset=SecretRole.objects.all(), field_name='name')
+    name = MultiValueCharFilter(lookup_expr='iexact')
 
     class Meta:
         model = SecretRole
         fields = ['id', 'name', 'slug', 'description', 'comments']
 
     def search(self, queryset, name, value):
         if not value.strip():
```

### Comparing `netbox-secrets-1.8.2/netbox_secrets/forms/bulk_edit.py` & `netbox-secrets-1.8.3/netbox_secrets/forms/bulk_edit.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/forms/filterset.py` & `netbox-secrets-1.8.3/netbox_secrets/forms/filterset.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from django import forms
 from django.contrib.contenttypes.models import ContentType
 from django.utils.translation import gettext as _
+
 from netbox.forms import NetBoxModelFilterSetForm
 from utilities.forms.fields import (
     ContentTypeMultipleChoiceField,
     DynamicModelMultipleChoiceField,
     TagFilterField,
 )
-
 from ..constants import *
 from ..models import Secret, SecretRole
 
 __all__ = [
     'SecretRoleFilterForm',
     'SecretFilterForm',
 ]
 
 
 class SecretRoleFilterForm(NetBoxModelFilterSetForm):
     model = SecretRole
     q = forms.CharField(required=False, label=_('Search'))
-    name = DynamicModelMultipleChoiceField(queryset=SecretRole.objects.all(), required=False)
+    id = DynamicModelMultipleChoiceField(queryset=SecretRole.objects.all(), required=False, label=_('Roles'))
 
 
 class SecretFilterForm(NetBoxModelFilterSetForm):
     model = Secret
 
     fieldsets = (
         (None, ('q', 'filter_id', 'tag')),
```

### Comparing `netbox-secrets-1.8.2/netbox_secrets/forms/model_forms.py` & `netbox-secrets-1.8.3/netbox_secrets/forms/model_forms.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/graphql/types.py` & `netbox-secrets-1.8.3/netbox_secrets/graphql/types.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/migrations/0001_initial.py` & `netbox-secrets-1.8.3/netbox_secrets/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/migrations/0002_populate_userkeys.py` & `netbox-secrets-1.8.3/netbox_secrets/migrations/0002_populate_userkeys.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/migrations/0003_populate_secretroles.py` & `netbox-secrets-1.8.3/netbox_secrets/migrations/0003_populate_secretroles.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/migrations/0004_populate_secrets.py` & `netbox-secrets-1.8.3/netbox_secrets/migrations/0004_populate_secrets.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/migrations/0005_alter_secret_custom_field_data_and_more.py` & `netbox-secrets-1.8.3/netbox_secrets/migrations/0005_alter_secret_custom_field_data_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/migrations/0006_alter_userkey_created_alter_userkey_last_updated.py` & `netbox-secrets-1.8.3/netbox_secrets/migrations/0006_alter_userkey_created_alter_userkey_last_updated.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/models/secrets.py` & `netbox-secrets-1.8.3/netbox_secrets/models/secrets.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/navigation.py` & `netbox-secrets-1.8.3/netbox_secrets/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/static/netbox_secrets/secrets.js` & `netbox-secrets-1.8.3/netbox_secrets/static/netbox_secrets/secrets.js`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/static/netbox_secrets/secrets.js.map` & `netbox-secrets-1.8.3/netbox_secrets/static/netbox_secrets/secrets.js.map`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/tables.py` & `netbox-secrets-1.8.3/netbox_secrets/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/template_content.py` & `netbox-secrets-1.8.3/netbox_secrets/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/inc/private_key_modal.html` & `netbox-secrets-1.8.3/netbox_secrets/templates/netbox_secrets/inc/private_key_modal.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/inc/secret_actions.html` & `netbox-secrets-1.8.3/netbox_secrets/templates/netbox_secrets/inc/secret_actions.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/inc/secrets_panel.html` & `netbox-secrets-1.8.3/netbox_secrets/templates/netbox_secrets/inc/secrets_panel.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/inc/view_tab.html` & `netbox-secrets-1.8.3/netbox_secrets/templates/netbox_secrets/inc/view_tab.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/secret.html` & `netbox-secrets-1.8.3/netbox_secrets/templates/netbox_secrets/secret.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/secret_edit.html` & `netbox-secrets-1.8.3/netbox_secrets/templates/netbox_secrets/secret_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/secretrole.html` & `netbox-secrets-1.8.3/netbox_secrets/templates/netbox_secrets/secretrole.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/userkey.html` & `netbox-secrets-1.8.3/netbox_secrets/templates/netbox_secrets/userkey.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/userkey_edit.html` & `netbox-secrets-1.8.3/netbox_secrets/templates/netbox_secrets/userkey_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/tests/constants.py` & `netbox-secrets-1.8.3/netbox_secrets/tests/constants.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/tests/test_api.py` & `netbox-secrets-1.8.3/netbox_secrets/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/tests/test_filters.py` & `netbox-secrets-1.8.3/netbox_secrets/tests/test_filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from dcim.models import Device, DeviceRole, DeviceType, Manufacturer, Site
 from django.test import TestCase
-from virtualization.models import Cluster, ClusterType, VirtualMachine
 
+from dcim.models import Device, DeviceRole, DeviceType, Manufacturer, Site
 from netbox_secrets.filtersets import *
 from netbox_secrets.models import Secret, SecretRole
+from virtualization.models import Cluster, ClusterType, VirtualMachine
 
 
 class SecretRoleTestCase(TestCase):
     queryset = SecretRole.objects.all()
     filterset = SecretRoleFilterSet
 
     @classmethod
@@ -21,15 +21,15 @@
 
     def test_id(self):
         params = {'id': self.queryset.values_list('pk', flat=True)[:2]}
         self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
 
     def test_name(self):
         name = SecretRole.objects.all()
-        params = {'name': [name[0].pk, name[1].pk]}
+        params = {'name': [name[0].name, name[1].name]}
         self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
 
     def test_slug(self):
         params = {'slug': ['secret-role-1', 'secret-role-2']}
         self.assertEqual(self.filterset(params, self.queryset).qs.count(), 2)
```

### Comparing `netbox-secrets-1.8.2/netbox_secrets/tests/test_form.py` & `netbox-secrets-1.8.3/netbox_secrets/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/tests/test_models.py` & `netbox-secrets-1.8.3/netbox_secrets/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/tests/test_views.py` & `netbox-secrets-1.8.3/netbox_secrets/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/urls.py` & `netbox-secrets-1.8.3/netbox_secrets/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/utils/crypto.py` & `netbox-secrets-1.8.3/netbox_secrets/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets/views.py` & `netbox-secrets-1.8.3/netbox_secrets/views.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/netbox_secrets.egg-info/SOURCES.txt` & `netbox-secrets-1.8.3/netbox_secrets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.2/setup.py` & `netbox-secrets-1.8.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='netbox-secrets',
-    version='1.8.2',
+    version='1.8.3',
     description='Netbox Secrets',
     long_description='A Secret store for NetBox',
     url='https://github.com/Onemind-Services-LLC/netbox-secrets/',
     author='Daniel Sheppard',
     author_email='dans@dansheps.com',
     license='Apache 2.0',
     install_requires=[
```

