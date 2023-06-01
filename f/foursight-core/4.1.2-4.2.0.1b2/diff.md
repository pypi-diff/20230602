# Comparing `tmp/foursight_core-4.1.2.tar.gz` & `tmp/foursight_core-4.2.0.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_core-4.1.2.tar", max compression
+gzip compressed data, was "foursight_core-4.2.0.1b2.tar", max compression
```

## Comparing `foursight_core-4.1.2.tar` & `foursight_core-4.2.0.1b2.tar`

### file list

```diff
@@ -1,76 +1,77 @@
--rw-r--r--   0        0        0     1083 2023-05-15 19:31:49.591048 foursight_core-4.1.2/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-05-15 19:31:49.599048 foursight_core-4.1.2/foursight_core/__init__.py
--rw-r--r--   0        0        0     1901 2023-05-15 19:31:49.599048 foursight_core-4.1.2/foursight_core/abstract_connection.py
--rw-r--r--   0        0        0       69 2023-05-15 19:31:49.599048 foursight_core-4.1.2/foursight_core/app.py
--rw-r--r--   0        0        0   105128 2023-05-15 19:31:49.599048 foursight_core-4.1.2/foursight_core/app_utils.py
--rw-r--r--   0        0        0     2571 2023-05-15 19:31:49.599048 foursight_core-4.1.2/foursight_core/buckets.py
--rw-r--r--   0        0        0      638 2023-05-15 19:31:49.599048 foursight_core-4.1.2/foursight_core/check_schema.py
--rw-r--r--   0        0        0        3 2023-05-15 19:31:49.599048 foursight_core-4.1.2/foursight_core/check_setup.json
--rw-r--r--   0        0        0    22858 2023-05-15 19:31:49.599048 foursight_core-4.1.2/foursight_core/check_utils.py
--rw-r--r--   0        0        0      270 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/checks/__init__.py
--rw-r--r--   0        0        0     4476 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/checks/access_key_expiration_detection.py
--rw-r--r--   0        0        0     2899 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/checks/codebuild_checks.py
--rw-r--r--   0        0        0     3305 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/checks/ecs_checks.py
--rw-r--r--   0        0        0     4683 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/checks/ecs_recovery_check.py
--rw-r--r--   0        0        0        0 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/checks/helpers/__init__.py
--rw-r--r--   0        0        0      348 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/checks/helpers/confchecks.py
--rw-r--r--   0        0        0     3519 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/checks/helpers/sys_utils.py
--rw-r--r--   0        0        0     2055 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0     8375 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/checks/scaling_checks.py
--rw-r--r--   0        0        0     2658 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/checks/test_checks.py
--rw-r--r--   0        0        0    11929 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/decorators.py
--rw-r--r--   0        0        0    15050 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/deploy.py
--rw-r--r--   0        0        0     8302 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/environment.py
--rw-r--r--   0        0        0    11792 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/es_connection.py
--rw-r--r--   0        0        0     1176 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/exceptions.py
--rw-r--r--   0        0        0     5146 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/fs_connection.py
--rw-r--r--   0        0        0     8423 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/identity.py
--rw-r--r--   0        0        0     3082 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/mapping.json
--rw-r--r--   0        0        0     1014 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/package.py
--rw-r--r--   0        0        0    16912 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/auth.py
--rw-r--r--   0        0        0     6629 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/auth0_config.py
--rw-r--r--   0        0        0    22994 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/aws_network.py
--rw-r--r--   0        0        0     3038 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/aws_s3.py
--rw-r--r--   0        0        0     6116 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/aws_stacks.py
--rw-r--r--   0        0        0    28009 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/checks.py
--rw-r--r--   0        0        0    20464 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/cognito.py
--rw-r--r--   0        0        0     3952 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/cookie_utils.py
--rw-r--r--   0        0        0     6189 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/datetime_utils.py
--rw-r--r--   0        0        0     1841 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/encoding_utils.py
--rw-r--r--   0        0        0     3649 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/encryption.py
--rw-r--r--   0        0        0     4720 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/envs.py
--rw-r--r--   0        0        0     3196 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/gac.py
--rw-r--r--   0        0        0     3516 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/jwt_utils.py
--rw-r--r--   0        0        0     9466 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/misc_utils.py
--rw-r--r--   0        0        0     5164 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/portal_access_key_utils.py
--rw-r--r--   0        0        0    78954 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/react_api.py
--rw-r--r--   0        0        0    11210 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/react_api_base.py
--rw-r--r--   0        0        0     8025 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/react_route_decorator.py
--rw-r--r--   0        0        0    33872 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/react_routes.py
--rw-r--r--   0        0        0     4805 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/react_ui.py
--rw-r--r--   0        0        0      806 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/api/yaml_utils.py
--rw-r--r--   0        0        0      234 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/ui/asset-manifest.json
--rw-r--r--   0        0        0     1681 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/ui/index.html
--rw-r--r--   0        0        0        3 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/ui/manifest.json
--rw-r--r--   0        0        0    11735 2023-05-15 19:31:49.603048 foursight_core-4.1.2/foursight_core/react/ui/static/css/main.css
--rw-r--r--   0        0        0  1932518 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/react/ui/static/js/main.js
--rw-r--r--   0        0        0      597 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/route_prefixes.py
--rw-r--r--   0        0        0    10496 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/routes.py
--rw-r--r--   0        0        0    22442 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/run_result.py
--rw-r--r--   0        0        0     6330 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/s3_connection.py
--rw-r--r--   0        0        0     5282 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/schedule_decorator.py
--rw-r--r--   0        0        0     1402 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/scripts/decrypt_accounts_file.py
--rw-r--r--   0        0        0     1406 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/scripts/encrypt_accounts_file.py
--rw-r--r--   0        0        0     5370 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/sqs_utils.py
--rw-r--r--   0        0        0     1715 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/stage.py
--rw-r--r--   0        0        0     7763 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/templates/base.html
--rw-r--r--   0        0        0    20532 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/templates/header.html
--rw-r--r--   0        0        0     4090 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/templates/history.html
--rw-r--r--   0        0        0    19634 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/templates/info.html
--rw-r--r--   0        0        0     1297 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/templates/unused.html
--rw-r--r--   0        0        0     2259 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/templates/user.html
--rw-r--r--   0        0        0     1669 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/templates/users.html
--rw-r--r--   0        0        0      572 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/templates/view_checks.html
--rw-r--r--   0        0        0     2248 2023-05-15 19:31:49.615048 foursight_core-4.1.2/foursight_core/templates/view_groups.html
--rw-r--r--   0        0        0     1603 2023-05-15 19:31:49.615048 foursight_core-4.1.2/pyproject.toml
--rw-r--r--   0        0        0     1189 1970-01-01 00:00:00.000000 foursight_core-4.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-06-01 22:56:44.423182 foursight_core-4.2.0.1b2/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-06-01 22:56:44.428854 foursight_core-4.2.0.1b2/foursight_core/__init__.py
+-rw-r--r--   0        0        0     1901 2023-06-01 22:56:44.428926 foursight_core-4.2.0.1b2/foursight_core/abstract_connection.py
+-rw-r--r--   0        0        0       69 2023-06-01 22:56:44.428975 foursight_core-4.2.0.1b2/foursight_core/app.py
+-rw-r--r--   0        0        0   105128 2023-06-01 22:56:44.429358 foursight_core-4.2.0.1b2/foursight_core/app_utils.py
+-rw-r--r--   0        0        0     2571 2023-06-01 22:56:44.429443 foursight_core-4.2.0.1b2/foursight_core/buckets.py
+-rw-r--r--   0        0        0      638 2023-06-01 22:56:44.429510 foursight_core-4.2.0.1b2/foursight_core/check_schema.py
+-rw-r--r--   0        0        0        3 2023-06-01 22:56:44.429564 foursight_core-4.2.0.1b2/foursight_core/check_setup.json
+-rw-r--r--   0        0        0    22858 2023-06-01 22:56:44.429683 foursight_core-4.2.0.1b2/foursight_core/check_utils.py
+-rw-r--r--   0        0        0      270 2023-06-01 22:56:44.429780 foursight_core-4.2.0.1b2/foursight_core/checks/__init__.py
+-rw-r--r--   0        0        0     4476 2023-06-01 22:56:44.429859 foursight_core-4.2.0.1b2/foursight_core/checks/access_key_expiration_detection.py
+-rw-r--r--   0        0        0     2899 2023-06-01 22:56:44.429921 foursight_core-4.2.0.1b2/foursight_core/checks/codebuild_checks.py
+-rw-r--r--   0        0        0     3305 2023-06-01 22:56:44.429986 foursight_core-4.2.0.1b2/foursight_core/checks/ecs_checks.py
+-rw-r--r--   0        0        0     4683 2023-06-01 22:56:44.430060 foursight_core-4.2.0.1b2/foursight_core/checks/ecs_recovery_check.py
+-rw-r--r--   0        0        0        0 2023-06-01 22:56:44.430116 foursight_core-4.2.0.1b2/foursight_core/checks/helpers/__init__.py
+-rw-r--r--   0        0        0      348 2023-06-01 22:56:44.430181 foursight_core-4.2.0.1b2/foursight_core/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0     3519 2023-06-01 22:56:44.430250 foursight_core-4.2.0.1b2/foursight_core/checks/helpers/sys_utils.py
+-rw-r--r--   0        0        0     2055 2023-06-01 22:56:44.430319 foursight_core-4.2.0.1b2/foursight_core/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0     8375 2023-06-01 22:56:44.430396 foursight_core-4.2.0.1b2/foursight_core/checks/scaling_checks.py
+-rw-r--r--   0        0        0     2658 2023-06-01 22:56:44.430459 foursight_core-4.2.0.1b2/foursight_core/checks/test_checks.py
+-rw-r--r--   0        0        0    11929 2023-06-01 22:56:44.430544 foursight_core-4.2.0.1b2/foursight_core/decorators.py
+-rw-r--r--   0        0        0    15050 2023-06-01 22:56:44.430637 foursight_core-4.2.0.1b2/foursight_core/deploy.py
+-rw-r--r--   0        0        0     8302 2023-06-01 22:56:44.430719 foursight_core-4.2.0.1b2/foursight_core/environment.py
+-rw-r--r--   0        0        0    11792 2023-06-01 22:56:44.430804 foursight_core-4.2.0.1b2/foursight_core/es_connection.py
+-rw-r--r--   0        0        0     1176 2023-06-01 22:56:44.430943 foursight_core-4.2.0.1b2/foursight_core/exceptions.py
+-rw-r--r--   0        0        0     5146 2023-06-01 22:56:44.431016 foursight_core-4.2.0.1b2/foursight_core/fs_connection.py
+-rw-r--r--   0        0        0     8423 2023-06-01 22:56:44.431090 foursight_core-4.2.0.1b2/foursight_core/identity.py
+-rw-r--r--   0        0        0     3082 2023-06-01 22:56:44.431156 foursight_core-4.2.0.1b2/foursight_core/mapping.json
+-rw-r--r--   0        0        0     1014 2023-06-01 22:56:44.431211 foursight_core-4.2.0.1b2/foursight_core/package.py
+-rw-r--r--   0        0        0    16912 2023-06-01 22:56:44.431385 foursight_core-4.2.0.1b2/foursight_core/react/api/auth.py
+-rw-r--r--   0        0        0     6629 2023-06-01 22:56:44.431609 foursight_core-4.2.0.1b2/foursight_core/react/api/auth0_config.py
+-rw-r--r--   0        0        0    22994 2023-06-01 22:56:44.431723 foursight_core-4.2.0.1b2/foursight_core/react/api/aws_network.py
+-rw-r--r--   0        0        0     3038 2023-06-01 22:56:44.431939 foursight_core-4.2.0.1b2/foursight_core/react/api/aws_s3.py
+-rw-r--r--   0        0        0     6116 2023-06-01 22:56:44.432016 foursight_core-4.2.0.1b2/foursight_core/react/api/aws_stacks.py
+-rw-r--r--   0        0        0    28009 2023-06-01 22:56:44.432132 foursight_core-4.2.0.1b2/foursight_core/react/api/checks.py
+-rw-r--r--   0        0        0    20464 2023-06-01 22:56:44.432264 foursight_core-4.2.0.1b2/foursight_core/react/api/cognito.py
+-rw-r--r--   0        0        0     3952 2023-06-01 22:56:44.432340 foursight_core-4.2.0.1b2/foursight_core/react/api/cookie_utils.py
+-rw-r--r--   0        0        0     6189 2023-06-01 22:56:44.432411 foursight_core-4.2.0.1b2/foursight_core/react/api/datetime_utils.py
+-rw-r--r--   0        0        0     1841 2023-06-01 22:56:44.432474 foursight_core-4.2.0.1b2/foursight_core/react/api/encoding_utils.py
+-rw-r--r--   0        0        0     3649 2023-06-01 22:56:44.432538 foursight_core-4.2.0.1b2/foursight_core/react/api/encryption.py
+-rw-r--r--   0        0        0     4720 2023-06-01 22:56:44.432603 foursight_core-4.2.0.1b2/foursight_core/react/api/envs.py
+-rw-r--r--   0        0        0     3196 2023-06-01 22:56:44.432670 foursight_core-4.2.0.1b2/foursight_core/react/api/gac.py
+-rw-r--r--   0        0        0     3516 2023-06-01 22:56:44.432733 foursight_core-4.2.0.1b2/foursight_core/react/api/jwt_utils.py
+-rw-r--r--   0        0        0     9466 2023-06-01 22:56:44.432818 foursight_core-4.2.0.1b2/foursight_core/react/api/misc_utils.py
+-rw-r--r--   0        0        0     5164 2023-06-01 22:56:44.432903 foursight_core-4.2.0.1b2/foursight_core/react/api/portal_access_key_utils.py
+-rw-r--r--   0        0        0    79982 2023-06-01 22:56:51.122411 foursight_core-4.2.0.1b2/foursight_core/react/api/react_api.py
+-rw-r--r--   0        0        0    11210 2023-06-01 22:56:44.433257 foursight_core-4.2.0.1b2/foursight_core/react/api/react_api_base.py
+-rw-r--r--   0        0        0     8025 2023-06-01 22:56:44.433344 foursight_core-4.2.0.1b2/foursight_core/react/api/react_route_decorator.py
+-rw-r--r--   0        0        0    34216 2023-06-01 22:56:51.122756 foursight_core-4.2.0.1b2/foursight_core/react/api/react_routes.py
+-rw-r--r--   0        0        0     4805 2023-06-01 22:56:44.433545 foursight_core-4.2.0.1b2/foursight_core/react/api/react_ui.py
+-rw-r--r--   0        0        0      806 2023-06-01 22:56:44.433609 foursight_core-4.2.0.1b2/foursight_core/react/api/yaml_utils.py
+-rw-r--r--   0        0        0      234 2023-06-01 22:56:44.433696 foursight_core-4.2.0.1b2/foursight_core/react/ui/asset-manifest.json
+-rw-r--r--   0        0        0     1681 2023-06-01 22:56:44.433762 foursight_core-4.2.0.1b2/foursight_core/react/ui/index.html
+-rw-r--r--   0        0        0        3 2023-06-01 22:56:44.433809 foursight_core-4.2.0.1b2/foursight_core/react/ui/manifest.json
+-rw-r--r--   0        0        0    11735 2023-06-01 22:56:44.434363 foursight_core-4.2.0.1b2/foursight_core/react/ui/static/css/main.css
+-rw-r--r--   0        0        0  1933280 2023-06-01 22:56:51.139496 foursight_core-4.2.0.1b2/foursight_core/react/ui/static/js/main.js
+-rw-r--r--   0        0        0      597 2023-06-01 22:56:44.444816 foursight_core-4.2.0.1b2/foursight_core/route_prefixes.py
+-rw-r--r--   0        0        0    10496 2023-06-01 22:56:44.444904 foursight_core-4.2.0.1b2/foursight_core/routes.py
+-rw-r--r--   0        0        0    22442 2023-06-01 22:56:44.444966 foursight_core-4.2.0.1b2/foursight_core/run_result.py
+-rw-r--r--   0        0        0     6330 2023-06-01 22:56:44.445073 foursight_core-4.2.0.1b2/foursight_core/s3_connection.py
+-rw-r--r--   0        0        0     5282 2023-06-01 22:56:44.445156 foursight_core-4.2.0.1b2/foursight_core/schedule_decorator.py
+-rw-r--r--   0        0        0     1402 2023-06-01 22:56:44.445259 foursight_core-4.2.0.1b2/foursight_core/scripts/decrypt_accounts_file.py
+-rw-r--r--   0        0        0     1406 2023-06-01 22:56:44.445320 foursight_core-4.2.0.1b2/foursight_core/scripts/encrypt_accounts_file.py
+-rw-r--r--   0        0        0     5370 2023-06-01 22:56:44.445402 foursight_core-4.2.0.1b2/foursight_core/sqs_utils.py
+-rw-r--r--   0        0        0     1715 2023-06-01 22:56:44.445471 foursight_core-4.2.0.1b2/foursight_core/stage.py
+-rw-r--r--   0        0        0     7763 2023-06-01 22:56:44.445653 foursight_core-4.2.0.1b2/foursight_core/templates/base.html
+-rw-r--r--   0        0        0    20532 2023-06-01 22:56:44.445766 foursight_core-4.2.0.1b2/foursight_core/templates/header.html
+-rw-r--r--   0        0        0     4090 2023-06-01 22:56:44.445844 foursight_core-4.2.0.1b2/foursight_core/templates/history.html
+-rw-r--r--   0        0        0    19634 2023-06-01 22:56:44.445927 foursight_core-4.2.0.1b2/foursight_core/templates/info.html
+-rw-r--r--   0        0        0     1297 2023-06-01 22:56:44.445997 foursight_core-4.2.0.1b2/foursight_core/templates/unused.html
+-rw-r--r--   0        0        0     2259 2023-06-01 22:56:44.446057 foursight_core-4.2.0.1b2/foursight_core/templates/user.html
+-rw-r--r--   0        0        0     1669 2023-06-01 22:56:44.446124 foursight_core-4.2.0.1b2/foursight_core/templates/users.html
+-rw-r--r--   0        0        0      572 2023-06-01 22:56:44.446212 foursight_core-4.2.0.1b2/foursight_core/templates/view_checks.html
+-rw-r--r--   0        0        0     2248 2023-06-01 22:56:44.446266 foursight_core-4.2.0.1b2/foursight_core/templates/view_groups.html
+-rw-r--r--   0        0        0     1626 2023-06-01 22:56:51.140511 foursight_core-4.2.0.1b2/pyproject.toml
+-rw-r--r--   0        0        0     1943 1970-01-01 00:00:00.000000 foursight_core-4.2.0.1b2/setup.py
+-rw-r--r--   0        0        0     1193 1970-01-01 00:00:00.000000 foursight_core-4.2.0.1b2/PKG-INFO
```

### Comparing `foursight_core-4.1.2/LICENSE.txt` & `foursight_core-4.2.0.1b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/abstract_connection.py` & `foursight_core-4.2.0.1b2/foursight_core/abstract_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/app_utils.py` & `foursight_core-4.2.0.1b2/foursight_core/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/buckets.py` & `foursight_core-4.2.0.1b2/foursight_core/buckets.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/check_schema.py` & `foursight_core-4.2.0.1b2/foursight_core/check_schema.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/check_utils.py` & `foursight_core-4.2.0.1b2/foursight_core/check_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/checks/access_key_expiration_detection.py` & `foursight_core-4.2.0.1b2/foursight_core/checks/access_key_expiration_detection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/checks/codebuild_checks.py` & `foursight_core-4.2.0.1b2/foursight_core/checks/codebuild_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/checks/ecs_checks.py` & `foursight_core-4.2.0.1b2/foursight_core/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/checks/ecs_recovery_check.py` & `foursight_core-4.2.0.1b2/foursight_core/checks/ecs_recovery_check.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/checks/helpers/sys_utils.py` & `foursight_core-4.2.0.1b2/foursight_core/checks/helpers/sys_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/checks/helpers/wrangler_utils.py` & `foursight_core-4.2.0.1b2/foursight_core/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/checks/scaling_checks.py` & `foursight_core-4.2.0.1b2/foursight_core/checks/scaling_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/checks/test_checks.py` & `foursight_core-4.2.0.1b2/foursight_core/checks/test_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/decorators.py` & `foursight_core-4.2.0.1b2/foursight_core/decorators.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/deploy.py` & `foursight_core-4.2.0.1b2/foursight_core/deploy.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/environment.py` & `foursight_core-4.2.0.1b2/foursight_core/environment.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/es_connection.py` & `foursight_core-4.2.0.1b2/foursight_core/es_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/exceptions.py` & `foursight_core-4.2.0.1b2/foursight_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/fs_connection.py` & `foursight_core-4.2.0.1b2/foursight_core/fs_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/identity.py` & `foursight_core-4.2.0.1b2/foursight_core/identity.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/mapping.json` & `foursight_core-4.2.0.1b2/foursight_core/mapping.json`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/package.py` & `foursight_core-4.2.0.1b2/foursight_core/package.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/react/api/auth.py` & `foursight_core-4.2.0.1b2/foursight_core/react/api/auth.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/react/api/auth0_config.py` & `foursight_core-4.2.0.1b2/foursight_core/react/api/auth0_config.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/react/api/aws_network.py` & `foursight_core-4.2.0.1b2/foursight_core/react/api/aws_network.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/react/api/aws_s3.py` & `foursight_core-4.2.0.1b2/foursight_core/react/api/aws_s3.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/react/api/aws_stacks.py` & `foursight_core-4.2.0.1b2/foursight_core/react/api/aws_stacks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/react/api/checks.py` & `foursight_core-4.2.0.1b2/foursight_core/react/api/checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/react/api/cognito.py` & `foursight_core-4.2.0.1b2/foursight_core/react/api/cognito.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/react/api/cookie_utils.py` & `foursight_core-4.2.0.1b2/foursight_core/react/api/cookie_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/react/api/datetime_utils.py` & `foursight_core-4.2.0.1b2/foursight_core/react/api/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/react/api/encoding_utils.py` & `foursight_core-4.2.0.1b2/foursight_core/react/api/encoding_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/react/api/encryption.py` & `foursight_core-4.2.0.1b2/foursight_core/react/api/encryption.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/react/api/envs.py` & `foursight_core-4.2.0.1b2/foursight_core/react/api/envs.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/react/api/gac.py` & `foursight_core-4.2.0.1b2/foursight_core/react/api/gac.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/react/api/jwt_utils.py` & `foursight_core-4.2.0.1b2/foursight_core/react/api/jwt_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/react/api/misc_utils.py` & `foursight_core-4.2.0.1b2/foursight_core/react/api/misc_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/react/api/portal_access_key_utils.py` & `foursight_core-4.2.0.1b2/foursight_core/react/api/portal_access_key_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/react/api/react_api.py` & `foursight_core-4.2.0.1b2/foursight_core/react/api/react_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1106,14 +1106,33 @@
         Called from react_routes for endpoint: GET /{env}/checks_registry
         Returns the content of the checks registry collected for the check_function
         decorator in decorators.py. For troubleshooting only.
         """
         ignored(request, env)
         return self.create_success_response(self._checks.get_registry())
 
+    def reactapi_checks_validation(self, request: dict, env: str) -> Response:
+        """
+        Called from react_routes for endpoint: GET /{env}/checks_validation
+        Returns information about any problems with the checks setup.
+        """
+        ignored(request, env)
+        checks_actions_registry = self._checks.get_registry()
+        actions_with_no_assocated_check = [name for name in checks_actions_registry
+                                           if checks_actions_registry[name].get("kind") == "action"
+                                           and not checks_actions_registry[name].get("checks")]
+        response = {}
+        if actions_with_no_assocated_check:
+            response["actions_with_no_associated_check"] = [
+                checks_actions_registry[item]
+                for item in checks_actions_registry
+                if checks_actions_registry[item]["kind"] == "action" and item in actions_with_no_assocated_check
+            ]
+        return self.create_success_response(response)
+
     def reactapi_lambdas(self, request: dict, env: str) -> Response:
         """
         Called from react_routes for endpoint: GET /{env}/lambdas
         Returns a summary (list) of all defined AWS lambdas for the current AWS environment.
         """
         ignored(request, env)
         # TODO: Filter out checks of lambas not in the env.
```

### Comparing `foursight_core-4.1.2/foursight_core/react/api/react_api_base.py` & `foursight_core-4.2.0.1b2/foursight_core/react/api/react_api_base.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/react/api/react_route_decorator.py` & `foursight_core-4.2.0.1b2/foursight_core/react/api/react_route_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/react/api/react_routes.py` & `foursight_core-4.2.0.1b2/foursight_core/react/api/react_routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,14 +361,21 @@
     @route("/{env}/checks_registry", authorize=True)
     def reactapi_route_checks_registry(env: str) -> Response:  # noqa: implicit @staticmethod via @route
         """
         Returns detailed registered checks functions.
         """
         return app.core.reactapi_checks_registry(app.current_request.to_dict(), env)
 
+    @route("/{env}/checks_validation", authorize=True)
+    def reactapi_route_checks_validation(env: str) -> Response:  # noqa: implicit @staticmethod via @route
+        """
+        Returns information about any problems with the checks setup.
+        """
+        return app.core.reactapi_checks_validation(app.current_request.to_dict(), env)
+
     @route("/{env}/lambdas", authorize=True)
     def reactapi_route_lambdas(env: str) -> Response:  # noqa: implicit @staticmethod via @route
         """
         Returns detailed info on defined lambdas.
         """
         return app.core.reactapi_lambdas(app.current_request.to_dict(), env)
```

### Comparing `foursight_core-4.1.2/foursight_core/react/api/react_ui.py` & `foursight_core-4.2.0.1b2/foursight_core/react/api/react_ui.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/react/api/yaml_utils.py` & `foursight_core-4.2.0.1b2/foursight_core/react/api/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/react/ui/index.html` & `foursight_core-4.2.0.1b2/foursight_core/react/ui/index.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/react/ui/static/css/main.css` & `foursight_core-4.2.0.1b2/foursight_core/react/ui/static/css/main.css`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/react/ui/static/js/main.js` & `foursight_core-4.2.0.1b2/foursight_core/react/ui/static/js/main.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.6f828eef.js.LICENSE.txt */
+/*! For license information please see main.62ec1490.js.LICENSE.txt */
 (function() {
     var __webpack_modules__ = {
             4189: function(e, t) {
                 "use strict";
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 })
@@ -52282,15 +52282,85 @@
                 var e = a(Yi(ya), 2),
                     t = e[0],
                     n = e[1];
                 return [t, function(e) {
                     n(e), bt.SetReadOnlyMode(e)
                 }]
             },
-            va = {
+            va = function() {
+                var e, t = null === (e = Xi("/checks_validation").data) || void 0 === e ? void 0 : e.actions_with_no_associated_check;
+                return t ? (0, Kr.jsxs)(Kr.Fragment, {
+                    children: [(0, Kr.jsxs)("div", {
+                        className: "box error thickborder",
+                        style: {
+                            width: "60%",
+                            fontSize: "small"
+                        },
+                        children: [(0, Kr.jsx)("b", {
+                            children: "The following defined action functions have no assocated check"
+                        }), ": ", (0, Kr.jsx)("br", {}), (0, Kr.jsx)(ji, {
+                            top: "6",
+                            bottom: "6",
+                            color: "darkred",
+                            thick: !0
+                        }), t.map((function(e) {
+                            return (0, Kr.jsxs)(Kr.Fragment, {
+                                children: [Fr.RightArrow, " ", (0, Kr.jsx)("a", {
+                                    href: e.github_url,
+                                    target: "_blank",
+                                    children: (0, Kr.jsx)("span", {
+                                        style: {
+                                            color: "darkred"
+                                        },
+                                        children: e.name
+                                    })
+                                }), (0, Kr.jsx)("br", {})]
+                            })
+                        }))]
+                    }), (0, Kr.jsx)("br", {})]
+                }) : (0, Kr.jsx)(Kr.Fragment, {})
+            },
+            Ma = function(e) {
+                var t, n = e.status;
+                return function(e) {
+                    return "ok" == e || "done" == e || e.includes("pass") || e.includes("success")
+                }(n = (null === (t = n) || void 0 === t ? void 0 : t.toLowerCase(n).trim()) || "") ? (0, Kr.jsx)("b", {
+                    style: {
+                        color: Ft.GetForegroundColor()
+                    },
+                    children: "OK"
+                }) : function(e) {
+                    return "warn" == e || "warning" == e
+                }(n) ? (0, Kr.jsx)("b", {
+                    style: {
+                        color: Ft.GetForegroundColor()
+                    },
+                    children: "WARNING"
+                }) : function(e) {
+                    return e.includes("error") || e.includes("fail") || e.includes("exception")
+                }(n) ? (0, Kr.jsx)("b", {
+                    style: {
+                        color: "darkred"
+                    },
+                    children: "ERROR"
+                }) : function(e) {
+                    return !it.HasValue(e)
+                }(n) ? (0, Kr.jsx)("b", {
+                    style: {
+                        color: "red"
+                    },
+                    children: "UNKNOWN"
+                }) : (0, Kr.jsx)("b", {
+                    style: {
+                        color: "black"
+                    },
+                    children: n
+                })
+            },
+            ba = {
                 FormatDateTime: function(e) {
                     var n = e.verbose,
                         r = void 0 !== n && n,
                         o = e.timezone,
                         i = void 0 === o || o,
                         s = a((0, t.useState)(new Date), 2),
                         u = s[0],
@@ -52340,143 +52410,143 @@
                                 id: "tooltip-timestamp-".concat(r || i),
                                 text: Pr.FormatDateTime(r || i)
                             })]
                         })
                     })
                 }
             },
-            Ma = va;
+            ja = ba;
 
-        function ba(e) {
+        function wa(e) {
             e.update()
         }
 
-        function ja(e) {
+        function xa(e) {
             e.update()
         }
 
-        function wa(e) {
+        function Na(e) {
             e.update()
         }
 
-        function xa(e, t) {
-            e.__showingResults = !1, ba(t)
+        function Ia(e, t) {
+            e.__showingResults = !1, wa(t)
         }
 
-        function Na(e, t, n) {
-            e.__showingResults = !0, ba(n)
+        function Da(e, t, n) {
+            e.__showingResults = !0, wa(n)
         }
 
-        function Ia(e, t, n) {
-            Sa(e, n) || (n.prepend(e), ba(n))
+        function Sa(e, t, n) {
+            ka(e, n) || (n.prepend(e), wa(n))
         }
 
-        function Da(e, t, n) {
+        function La(e, t, n) {
             e.checks.map((function(e) {
-                return Ca(e, n)
+                return _a(e, n)
             }));
             var r = function(e, t) {
                 for (var n = 0; n < t.length; n++) {
                     if (t.get(n).group === e.group) return n
                 }
                 return -1
             }(e, t);
             t.remove(r)
         }
 
-        function Sa(e, t) {
+        function ka(e, t) {
             for (var n = 0; n < t.length; n++) {
                 if (t.get(n).group === e.group) return !0
             }
             return !1
         }
 
-        function La(e) {
+        function Ca(e) {
             return null === e || void 0 === e ? void 0 : e.__showingResults
         }
 
-        function ka(e) {
+        function Ea(e) {
             Object.keys(e.kwargs).forEach((function(t) {
                 if (!st.IsBoolean(e.kwargs[t]) && !st.IsNonEmptyArray(e.kwargs[t])) {
                     var n = "".concat(e.name, ".").concat(t),
                         r = document.getElementById(n),
                         o = null === r || void 0 === r ? void 0 : r.value;
                     e.kwargs[t] = o
                 }
             }))
         }
 
-        function Ca(e, t) {
+        function _a(e, t) {
             if (e.__showingHistory) {
                 e.__showingHistory = !1;
                 var n = function(e, t) {
                     for (var n = 0; n < t.length; n++) {
                         if (t.get(n).name === e.name) return n
                     }
                     return -1
                 }(e, t);
                 t.remove(n)
             }
         }
 
-        function Ea(e, t, n) {
+        function Ta(e, t, n) {
             ! function(e, t, n) {
-                e.__showingHistory ? Ca(e, n) : _a(e, t, n)
+                e.__showingHistory ? _a(e, n) : Aa(e, t, n)
             }(e, t, n)
         }
 
-        function _a(e, t, n) {
+        function Aa(e, t, n) {
             e.__showingHistory || (e.__showingHistory = !0, n.prepend(e))
         }
 
-        function Ta(e, t, n, r, o) {
+        function Oa(e, t, n, r, o) {
             var i = e.kwargs,
                 a = Tr.Str(i),
                 s = btoa(a);
-            Oa(e, n), wa(n), e.__queueingCheckRun = !0, o({
+            Ua(e, n), Na(n), e.__queueingCheckRun = !0, o({
                     url: zt.Url("/checks/".concat(e.name, "/run?args=").concat(s), t),
                     onData: function(t) {
                         return e.__queueingCheckRun = !1, e.__queuedCheckRun = t.uuid, setTimeout((function() {
                             ! function(e) {
                                 e.__resultHistory && e.__resultHistory.refresh()
-                            }(e), wa(n)
+                            }(e), Na(n)
                         }), 4e3), t.uuid
                     }
                 }), e.__queuedCheckRun = null,
                 function(e, t) {
-                    e.showingCheckRunningBox = !0, wa(t)
-                }(e, n), _a(e, 0, r)
+                    e.showingCheckRunningBox = !0, Na(t)
+                }(e, n), Aa(e, 0, r)
         }
 
-        function Aa(e, t, n, r, o) {
+        function za(e, t, n, r, o) {
             var i, a = {
                     check_name: e.name,
                     called_by: null === (i = e.__result) || void 0 === i ? void 0 : i.get("uuid")
                 },
                 s = Tr.Str(a),
                 u = btoa(s);
-            za(e, r), wa(r), e.__queueingActionRun = !0, o({
+            Pa(e, r), Na(r), e.__queueingActionRun = !0, o({
                     url: zt.Url("/action/".concat(t, "/run?args=").concat(u), n),
                     onData: function(t) {
                         return e.__queueingActionRun = !1, e.__queuedActionRun = t.uuid, t.uuid
                     }
                 }), e.__queuedActionRun = null,
                 function(e, t) {
-                    e.__showingActionRunningBox = !0, wa(t)
+                    e.__showingActionRunningBox = !0, Na(t)
                 }(e, r)
         }
 
-        function Oa(e, t) {
-            e.showingCheckRunningBox = !1, wa(t)
+        function Ua(e, t) {
+            e.showingCheckRunningBox = !1, Na(t)
         }
 
-        function za(e, t) {
-            e.__showingActionRunningBox = !1, wa(t)
+        function Pa(e, t) {
+            e.__showingActionRunningBox = !1, Na(t)
         }
-        var Ua = function(e) {
+        var Ra = function(e) {
                 var t = e.groupList,
                     n = e.env,
                     r = e.historyList,
                     o = e.info,
                     i = e.toggleShowingChecksSearch;
                 return t.error ? (0, Kr.jsx)(xi, {
                     error: t.error,
@@ -52502,45 +52572,45 @@
                                 id: "tooltip-search",
                                 position: "right",
                                 shape: "squared",
                                 size: "small",
                                 text: "Click to search for checks."
                             })]
                         }), t.map((function(e, i) {
-                            return (0, Kr.jsx)(Pa, {
+                            return (0, Kr.jsx)(Ba, {
                                 group: e,
                                 env: n,
                                 groupList: t,
                                 historyList: r,
                                 info: o,
                                 style: {
                                     paddingBottom: "6pt"
                                 }
                             }, e.group)
                         }))]
                     }) : (0, Kr.jsx)(Kr.Fragment, {})
                 })
             },
-            Pa = function(e) {
+            Ba = function(e) {
                 var t, n = e.group,
                     r = e.groupList,
                     o = e.historyList,
                     i = e.env,
                     a = e.info,
                     s = e.style,
                     u = void 0 === s ? {} : s;
 
                 function l(e, t) {
                     c(e) ? function(e, t) {
                         e.map((function(e) {
-                            return e.__showingResults && xa(e, t)
+                            return e.__showingResults && Ia(e, t)
                         }))
                     }(e, t) : function(e, t, n) {
                         e.map((function(e) {
-                            return !e.__showingResults && Na(e, 0, n)
+                            return !e.__showingResults && Da(e, 0, n)
                         }))
                     }(e, 0, t)
                 }
 
                 function c(e) {
                     for (var t = 0; t < (null === e || void 0 === e ? void 0 : e.length); t++)
                         if (e[t].__showingResults) return !0;
@@ -52574,15 +52644,15 @@
                                 })]
                             }), (0, Kr.jsx)("span", {
                                 style: {
                                     float: "right",
                                     cursor: "pointer"
                                 },
                                 onClick: function() {
-                                    Da(n, r, o)
+                                    La(n, r, o)
                                 },
                                 children: (0, Kr.jsx)("b", {
                                     children: Fr.X
                                 })
                             })]
                         }), (0, Kr.jsx)("div", {
                             style: {
@@ -52592,27 +52662,27 @@
                             return e.title > t.title ? 1 : e.title < t.title ? -1 : 0
                         })).map((function(e, t) {
                             return (0, Kr.jsxs)("div", {
                                 children: [t > 0 && (0, Kr.jsx)("div", {
                                     style: {
                                         marginBottom: "12px"
                                     }
-                                }), (0, Kr.jsx)(Ra, {
+                                }), (0, Kr.jsx)(Fa, {
                                     check: e,
                                     env: i,
                                     groupList: r,
                                     historyList: o,
                                     info: a
                                 })]
                             }, t)
                         }))]
                     })
                 })
             },
-            Ra = function(e) {
+            Fa = function(e) {
                 var n, r = e.check,
                     o = e.env,
                     i = e.groupList,
                     s = e.historyList,
                     u = e.info,
                     l = (0, t.useState)(!1);
 
@@ -52685,19 +52755,19 @@
                                         style: {
                                             verticalAlign: "top",
                                             width: "1%",
                                             cursor: "pointer"
                                         },
                                         onClick: function() {
                                             ! function(e, t, n) {
-                                                e.__showingResults ? xa(e, n) : (Na(e, 0, n), g(!0))
+                                                e.__showingResults ? Ia(e, n) : (Da(e, 0, n), g(!0))
                                             }(r, 0, i)
                                         },
                                         children: (0, Kr.jsxs)("b", {
-                                            children: [La(r) ? (0, Kr.jsx)("small", {
+                                            children: [Ca(r) ? (0, Kr.jsx)("small", {
                                                 children: Fr.DownArrowHollow
                                             }) : (0, Kr.jsx)("small", {
                                                 children: Fr.RightArrowHollow
                                             }), "\xa0"]
                                         })
                                     }), (0, Kr.jsxs)("td", {
                                         style: {
@@ -52712,15 +52782,15 @@
                                                     id: "tooltip-configure ".concat(r.name),
                                                     className: r.__configuringCheckRun ? "check-config-button" : "check-run-button",
                                                     style: {
                                                         marginTop: "-2pt",
                                                         float: "right"
                                                     },
                                                     onClick: function() {
-                                                        r.__configuringCheckRun ? (ka(r), r.__configuringCheckRun = !1) : r.__configuringCheckRun = !0, wa(i), g(!0)
+                                                        r.__configuringCheckRun ? (Ea(r), r.__configuringCheckRun = !1) : r.__configuringCheckRun = !0, Na(i), g(!0)
                                                     },
                                                     children: [(0, Kr.jsx)("span", {
                                                         style: {
                                                             fontSize: "small"
                                                         },
                                                         children: Fr.DownArrowFat
                                                     }), "\xa0Configure"]
@@ -52732,15 +52802,15 @@
                                             })
                                         }) : (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("div", {
                                                 style: {
                                                     marginLeft: "10pt",
                                                     float: "right"
                                                 },
-                                                children: (0, Kr.jsx)(Qa, {
+                                                children: (0, Kr.jsx)(Wa, {
                                                     check: r,
                                                     env: o,
                                                     groupList: i,
                                                     historyList: s,
                                                     style: {
                                                         marginTop: "-1pt"
                                                     }
@@ -52750,19 +52820,19 @@
                                             style: {
                                                 whiteSpace: "nowrap"
                                             },
                                             children: [(0, Kr.jsx)("u", {
                                                 id: "tooltip-check-info ".concat(r.name),
                                                 style: {
                                                     cursor: "pointer",
-                                                    fontWeight: La(r) ? "bold" : "normal",
+                                                    fontWeight: Ca(r) ? "bold" : "normal",
                                                     whiteSpace: "break-spaces"
                                                 },
                                                 onClick: function() {
-                                                    Ea(r, o, s)
+                                                    Ta(r, o, s)
                                                 },
                                                 children: (null === (n = r.title) || void 0 === n ? void 0 : n.length) > 70 ? r.title.substring(0, 69) + " ..." : r.title
                                             }), (0, Kr.jsx)(Mi, {
                                                 id: "tooltip-check-info ".concat(r.name),
                                                 text: "Check: ".concat(r.name, ". Module: ").concat(r.module, ".")
                                             }), r.__result.get("action") && (0, Kr.jsx)("u", {
                                                 children: l[0] ? (0, Kr.jsxs)(Kr.Fragment, {
@@ -52820,15 +52890,15 @@
                                                         height: "18"
                                                     })
                                                 }), (0, Kr.jsx)(Mi, {
                                                     id: "tooltip-view-source ".concat(r.name),
                                                     text: "Click to view source code for this check (in new tab)."
                                                 })]
                                             })]
-                                        }), (0, Kr.jsx)(Ba, {
+                                        }), (0, Kr.jsx)(Ya, {
                                             check: r,
                                             env: o,
                                             historyList: s
                                         }), Object.keys(null === r || void 0 === r ? void 0 : r.schedule).map((function(e, t) {
                                             var n, o;
                                             return (0, Kr.jsx)("div", {
                                                 children: it.HasValue(null === (n = r.schedule[e]) || void 0 === n ? void 0 : n.cron_description) ? (0, Kr.jsxs)("div", {
@@ -52850,42 +52920,42 @@
                                                     })]
                                                 }, t) : (0, Kr.jsx)("small", {
                                                     children: (0, Kr.jsx)("i", {
                                                         children: "Not scheduled."
                                                     })
                                                 })
                                             }, e)
-                                        })), (0, Kr.jsx)(Ga, {
+                                        })), (0, Kr.jsx)(Ha, {
                                             check: r,
                                             env: o,
                                             groupList: i,
                                             historyList: s,
                                             update: function() {
-                                                return wa(i)
+                                                return Na(i)
                                             },
                                             showDependenciesBox: h,
                                             setShowDependenciesBox: g
-                                        }), (0, Kr.jsx)(Wa, {
+                                        }), (0, Kr.jsx)(Za, {
                                             check: r,
                                             groupList: i,
                                             info: u
-                                        }), (0, Kr.jsx)(Ka, {
+                                        }), (0, Kr.jsx)($a, {
                                             check: r,
                                             env: o,
                                             groupList: i,
                                             update: function() {
                                                 return i.update()
                                             },
                                             fetchResult: c,
                                             runActionAllowedState: l
-                                        }), (0, Kr.jsx)(Ha, {
+                                        }), (0, Kr.jsx)(Va, {
                                             check: r,
                                             groupList: i,
                                             info: u
-                                        }), (0, Kr.jsx)(Fa, {
+                                        }), (0, Kr.jsx)(Qa, {
                                             check: r,
                                             env: o,
                                             groupList: i,
                                             fetchResult: c,
                                             runActionAllowedState: l
                                         })]
                                     })]
@@ -52896,25 +52966,25 @@
                                     children: (0, Kr.jsx)("td", {})
                                 })]
                             })
                         })
                     })
                 })
             },
-            Ba = function(e) {
+            Ya = function(e) {
                 var t = e.check,
                     n = e.env,
                     r = e.historyList,
                     o = e.style;
                 return (0, Kr.jsxs)("span", {
                     style: Ye(Ye({}, o), {}, {
                         cursor: "pointer"
                     }),
                     onClick: function() {
-                        return Ea(t, n, r)
+                        return Ta(t, n, r)
                     },
                     children: [(0, Kr.jsx)("span", {
                         id: "tooltip-recent-history ".concat(t.name),
                         children: (0, Kr.jsx)("img", {
                             alt: "history",
                             onClick: function(e) {},
                             src: Ut.History(),
@@ -52928,15 +52998,15 @@
                         id: "tooltip-recent-history ".concat(t.name),
                         text: "Click to " + (t.__showingHistory ? "hide" : "show") + " recent history of check runs."
                     }), t.__showingHistory ? (0, Kr.jsx)("span", {
                         children: Fr.RightArrow
                     }) : (0, Kr.jsx)(Kr.Fragment, {})]
                 })
             },
-            Fa = function(e) {
+            Qa = function(e) {
                 var n, r, o, i = e.check,
                     s = e.env,
                     u = e.groupList,
                     l = e.fetchResult,
                     c = (e.runActionAllowedState, a((0, t.useState)(!1), 2)),
                     d = c[0],
                     f = c[1],
@@ -52953,15 +53023,15 @@
                 }
 
                 function v(e, t) {
                     f(!1), g(!0)
                 }
 
                 function M(e, t) {
-                    e.__showingResultDetails = !e.__showingResultDetails, ja(t)
+                    e.__showingResultDetails = !e.__showingResultDetails, xa(t)
                 }
                 var b = function(e) {
                     var t, n = e.check,
                         r = e.env,
                         o = (e.checkUuid, e.groupList);
                     return t = d ? n.__resultByUuid.loading ? "Fetching latest result: ".concat(n.__result.get("uuid")) : "Click to fetch latest result: ".concat(n.__result.get("uuid")) : n.__result.loading ? "Fetching latest result." : "Click to fetch latest result.", (0, Kr.jsxs)("span", {
                         style: {
@@ -53268,24 +53338,24 @@
                             })]
                         })
                     }), i.__showingResultDetails && (!i.__result.empty || !i.__resultByUuid.empty || !i.__resultByAction.empty) && (0, Kr.jsxs)(Kr.Fragment, {
                         children: [(0, Kr.jsx)("div", {
                             style: {
                                 height: "2pt"
                             }
-                        }), (0, Kr.jsx)(Ya, {
+                        }), (0, Kr.jsx)(Ga, {
                             check: i,
                             groupList: u,
                             showResultByUuid: d,
                             showResultByAction: h
                         })]
                     })]
                 })
             },
-            Ya = function(e) {
+            Ga = function(e) {
                 var t, n = e.check,
                     r = e.groupList,
                     o = e.showResultByUuid,
                     i = e.showResultByAction;
                 e.style;
                 return n.__showingResults ? o ? (0, Kr.jsxs)("pre", {
                     className: "box lighten",
@@ -53326,15 +53396,15 @@
                         }), "\xa0", (0, Kr.jsx)("span", {
                             style: {
                                 fontSize: "large",
                                 cursor: "pointer",
                                 color: "black"
                             },
                             onClick: function() {
-                                n.__showingResultDetails = !1, ja(r)
+                                n.__showingResultDetails = !1, xa(r)
                             },
                             children: "X"
                         })]
                     }), n.__result.loading || n.__resultByUuid.loading || n.__resultByAction.loading ? (0, Kr.jsx)(Kr.Fragment, {
                         children: (0, Kr.jsx)(no, {
                             condition: n.__result.loading || n.__resultByUuid.loading || n.__resultByAction.loading,
                             color: Ft.GetForegroundColor(),
@@ -53382,15 +53452,15 @@
                         }), "\xa0", (0, Kr.jsx)("span", {
                             style: {
                                 fontSize: "large",
                                 cursor: "pointer",
                                 color: "black"
                             },
                             onClick: function() {
-                                n.__showingResultDetails = !1, ja(r)
+                                n.__showingResultDetails = !1, xa(r)
                             },
                             children: "X"
                         })]
                     }), n.__result.loading || n.__resultByUuid.loading || n.__resultByAction.loading ? (0, Kr.jsx)(Kr.Fragment, {
                         children: (0, Kr.jsx)(no, {
                             condition: n.__result.loading || n.__resultByUuid.loading || n.__resultByAction.loading,
                             color: Ft.GetForegroundColor(),
@@ -53439,30 +53509,30 @@
                         }), "\xa0", (0, Kr.jsx)("span", {
                             style: {
                                 fontSize: "x-large",
                                 cursor: "pointer",
                                 color: "black"
                             },
                             onClick: function() {
-                                n.showingResultDetailsFull = !n.showingResultDetailsFull, ja(r)
+                                n.showingResultDetailsFull = !n.showingResultDetailsFull, xa(r)
                             },
                             children: n.showingResultDetailsFull ? (0, Kr.jsx)("span", {
                                 title: "Show full result output.",
                                 children: Fr.UpArrow
                             }) : (0, Kr.jsx)("span", {
                                 children: Fr.DownArrow
                             })
                         }), "\xa0", (0, Kr.jsx)("span", {
                             style: {
                                 fontSize: "large",
                                 cursor: "pointer",
                                 color: "black"
                             },
                             onClick: function() {
-                                n.__showingResultDetails = !1, ja(r)
+                                n.__showingResultDetails = !1, xa(r)
                             },
                             children: "X"
                         })]
                     }), n.__result.loading || n.__resultByUuid.loading || n.__resultByAction.loading ? (0, Kr.jsx)(no, {
                         condition: n.__result.loading || n.__resultByUuid.loading || n.__resultByAction.loading,
                         color: Ft.GetForegroundColor(),
                         label: "Loading latest result "
@@ -53470,15 +53540,15 @@
                         style: {
                             marginTop: "1pt"
                         },
                         children: "No result."
                     }) : Bi.Format(n.showingResultDetailsFull ? n.__result.get("full_output") : n.__result.get())]
                 }) : (0, Kr.jsx)(Kr.Fragment, {})
             },
-            Qa = function(e) {
+            Wa = function(e) {
                 var t = e.check,
                     n = e.env,
                     r = e.groupList,
                     o = e.historyList,
                     i = e.style,
                     s = a(ma(), 1)[0],
                     u = la();
@@ -53506,15 +53576,15 @@
                         className: "check-run-button" + (t.__configuringCheckRun, ""),
                         style: Ye(Ye({}, i), {}, {
                             cursor: s && t.__configuringCheckRun ? "not-allowed" : "",
                             background: s && t.__configuringCheckRun ? "#888888" : "",
                             color: t.__configuringCheckRun ? "yellow" : ""
                         }),
                         onClick: function(e) {
-                            t.__configuringCheckRun ? s || (ka(t), Ta(t, n, r, o, u)) : (t.__configuringCheckRun = !0, wa(r))
+                            t.__configuringCheckRun ? s || (Ea(t), Oa(t, n, r, o, u)) : (t.__configuringCheckRun = !0, Na(r))
                         },
                         children: (0, Kr.jsx)("span", {
                             children: s ? (0, Kr.jsx)(Kr.Fragment, {
                                 children: t.__configuringCheckRun ? (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsxs)("span", {
                                         style: {
                                             fontSize: "",
@@ -53551,15 +53621,15 @@
                                     })
                                 })
                             })
                         })
                     })]
                 })
             },
-            Ga = function(e) {
+            Ha = function(e) {
                 var n = e.check,
                     r = e.env,
                     o = e.groupList,
                     i = e.historyList,
                     a = (e.update, e.showDependenciesBox),
                     s = e.setShowDependenciesBox;
 
@@ -53656,15 +53726,15 @@
                         },
                         children: st.IsNonEmptyObject(n.kwargs) ? (0, Kr.jsxs)(Kr.Fragment, {
                             children: [(0, Kr.jsx)("div", {
                                 style: {
                                     marginTop: "-2pt",
                                     float: "right"
                                 },
-                                children: (0, Kr.jsx)(Qa, {
+                                children: (0, Kr.jsx)(Wa, {
                                     check: n,
                                     env: r,
                                     groupList: o,
                                     historyList: i,
                                     style: {
                                         float: "right"
                                     }
@@ -53695,15 +53765,15 @@
                                                     defaultValue: n.kwargs[e] ? "true" : "false",
                                                     style: {
                                                         background: "lightyellow",
                                                         border: "1px solid lightgray",
                                                         borderRadius: "4pt"
                                                     },
                                                     onChange: function(t) {
-                                                        n.kwargs[e] = "true" === t.target.value, wa(o)
+                                                        n.kwargs[e] = "true" === t.target.value, Na(o)
                                                     },
                                                     children: (n.kwargs[e], (0, Kr.jsxs)(Kr.Fragment, {
                                                         children: [(0, Kr.jsx)("option", {
                                                             children: "true"
                                                         }), (0, Kr.jsx)("option", {
                                                             children: "false"
                                                         })]
@@ -53711,28 +53781,28 @@
                                                 }), st.IsNonEmptyArray(n.kwargs[e]) && (0, Kr.jsx)("select", {
                                                     defaultValue: null === (t = n.kwargs[e]) || void 0 === t ? void 0 : t.__selected,
                                                     style: {
                                                         background: "lightyellow",
                                                         border: "1px solid lightgray"
                                                     },
                                                     onChange: function(t) {
-                                                        n.kwargs[e].__selected = t.target.value, wa(o)
+                                                        n.kwargs[e].__selected = t.target.value, Na(o)
                                                     },
                                                     children: n.kwargs[e].map((function(e) {
                                                         return (0, Kr.jsx)("option", {
                                                             children: e
                                                         }, Dr()())
                                                     }))
                                                 }, Dr()()), !st.IsBoolean(n.kwargs[e]) && !st.IsNonEmptyArray(n.kwargs[e]) && (0, Kr.jsx)(Kr.Fragment, {
                                                     children: (0, Kr.jsx)("input", {
                                                         id: "".concat(n.name, ".").concat(e),
                                                         defaultValue: n.kwargs[e],
                                                         placeholder: "Empty",
                                                         onBlur: function() {
-                                                            ka(n)
+                                                            Ea(n)
                                                         },
                                                         style: {
                                                             marginLeft: "0pt",
                                                             height: "14pt",
                                                             background: "lightyellow",
                                                             border: "1px solid lightgray",
                                                             borderRadius: "2pt"
@@ -53746,29 +53816,29 @@
                             })]
                         }) : (0, Kr.jsxs)(Kr.Fragment, {
                             children: [(0, Kr.jsx)("div", {
                                 style: {
                                     marginTop: "-3pt",
                                     float: "right"
                                 },
-                                children: (0, Kr.jsx)(Qa, {
+                                children: (0, Kr.jsx)(Wa, {
                                     check: n,
                                     env: r,
                                     groupList: o,
                                     historyList: i,
                                     style: {
                                         float: "right"
                                     }
                                 })
                             }), "No arguments."]
                         })
                     })]
                 })
             },
-            Wa = function(e) {
+            Za = function(e) {
                 var n = e.check,
                     r = e.groupList,
                     o = e.info,
                     i = a((0, t.useState)(!1), 2),
                     s = i[0],
                     u = i[1];
                 return n.showingCheckRunningBox && n.__configuringCheckRun ? (0, Kr.jsx)("div", {
@@ -53846,15 +53916,15 @@
                                 }), (0, Kr.jsxs)("div", {
                                     style: {
                                         float: "right",
                                         marginTop: "-0pt",
                                         cursor: "pointer"
                                     },
                                     onClick: function() {
-                                        Oa(n, r)
+                                        Ua(n, r)
                                     },
                                     children: ["\xa0", (0, Kr.jsx)("b", {
                                         children: Fr.X
                                     }), "\xa0"]
                                 })]
                             })
                         }), !n.__queuedCheckRun && (0, Kr.jsx)("div", {
@@ -53866,15 +53936,15 @@
                                 label: " Queueing check run",
                                 color: "darkred"
                             })
                         })]
                     })
                 }) : (0, Kr.jsx)("span", {})
             },
-            Ha = function(e) {
+            Va = function(e) {
                 var n = e.check,
                     r = e.groupList,
                     o = e.info,
                     i = a((0, t.useState)(!1), 2),
                     s = i[0],
                     u = i[1];
                 return n.__showingActionRunningBox && n.__configuringCheckRun ? (0, Kr.jsx)("div", {
@@ -53953,15 +54023,15 @@
                                 }), (0, Kr.jsxs)("div", {
                                     style: {
                                         float: "right",
                                         marginTop: "-0pt",
                                         cursor: "pointer"
                                     },
                                     onClick: function() {
-                                        za(n, r)
+                                        Pa(n, r)
                                     },
                                     children: ["\xa0", Fr.X]
                                 })]
                             })
                         }), !n.__queuedActionRun && (0, Kr.jsx)("div", {
                             style: {
                                 marginTop: "-2pt"
@@ -53971,15 +54041,15 @@
                                 label: " Queueing action run",
                                 color: "darkred"
                             })
                         })]
                     })
                 }) : (0, Kr.jsx)("span", {})
             },
-            Za = function(e) {
+            qa = function(e) {
                 var t = e.env,
                     n = e.historyList;
                 if (n.error) return (0, Kr.jsx)(xi, {
                     error: n.error,
                     message: "Error loading check history from Foursight API"
                 });
                 var r = n.filter((function(e) {
@@ -53992,24 +54062,24 @@
                         },
                         children: "Recent Results"
                     }), null === r || void 0 === r ? void 0 : r.map((function(e, r) {
                         return (0, Kr.jsx)("div", {
                             style: {
                                 marginTop: "3pt"
                             },
-                            children: (0, Kr.jsx)(Va, {
+                            children: (0, Kr.jsx)(Ja, {
                                 check: e,
                                 env: t,
                                 historyList: n
                             })
                         }, e.name)
                     }))]
                 })
             },
-            Va = function(e) {
+            Ja = function(e) {
                 var n, r, o, i = e.check,
                     a = (e.env, e.historyList);
 
                 function s(e, t) {
                     e.__resultShowing = !1, e.__result = null, e.__resultLoading = !1, t.update()
                 }
 
@@ -54145,15 +54215,15 @@
                             })]
                         }), (0, Kr.jsxs)("span", {
                             style: {
                                 float: "right",
                                 cursor: "pointer"
                             },
                             onClick: function() {
-                                Ca(i, a)
+                                _a(i, a)
                             },
                             children: ["\xa0\xa0", (0, Kr.jsx)("b", {
                                 children: Fr.X
                             })]
                         })]
                     }), (0, Kr.jsx)("div", {
                         style: {
@@ -54244,28 +54314,16 @@
                                                             children: (0, Kr.jsx)("b", {
                                                                 style: {
                                                                     color: "inherit"
                                                                 },
                                                                 children: "OK"
                                                             })
                                                         }) : (0, Kr.jsx)(Kr.Fragment, {
-                                                            children: "WARN" === c(e) ? (0, Kr.jsx)(Kr.Fragment, {
-                                                                children: (0, Kr.jsx)("b", {
-                                                                    style: {
-                                                                        color: "black"
-                                                                    },
-                                                                    children: "WARNING"
-                                                                })
-                                                            }) : (0, Kr.jsx)(Kr.Fragment, {
-                                                                children: (0, Kr.jsx)("b", {
-                                                                    style: {
-                                                                        color: "darkred"
-                                                                    },
-                                                                    children: "ERROR"
-                                                                })
+                                                            children: (0, Kr.jsx)(Ma, {
+                                                                status: c(e)
                                                             })
                                                         }), "\xa0\xa0"]
                                                     }), (0, Kr.jsxs)("td", {
                                                         style: {
                                                             textAlign: "right"
                                                         },
                                                         children: [f(e), "\xa0\xa0"]
@@ -54390,15 +54448,15 @@
                                     })
                                 })
                             })
                         })
                     })]
                 })
             },
-            qa = function(e) {
+            Ka = function(e) {
                 return (0, Kr.jsxs)(Kr.Fragment, {
                     children: ["\xa0", (0, Kr.jsxs)("span", {
                         style: {
                             fontWeight: e.showingChecksSearch ? "bold" : "normal"
                         },
                         onClick: e.toggleShowingChecksSearch,
                         children: [(0, Kr.jsx)("span", {
@@ -54416,15 +54474,15 @@
                             },
                             src: Ut.NewIcon(),
                             height: "42"
                         })]
                     }), " ", (0, Kr.jsx)("br", {})]
                 })
             },
-            Ja = function(e) {
+            Xa = function(e) {
                 var n = a((0, t.useState)(""), 2),
                     r = n[0],
                     o = n[1],
                     i = a((0, t.useState)([]), 2),
                     s = i[0],
                     l = i[1];
                 (0, t.useEffect)((function() {
@@ -54611,15 +54669,15 @@
                                     children: "No results."
                                 })
                             })]
                         })
                     })]
                 })
             },
-            Ka = function(e) {
+            $a = function(e) {
                 var n, r = e.check,
                     o = e.env,
                     i = e.groupList,
                     s = e.fetchResult,
                     u = e.runActionAllowedState,
                     l = a((0, t.useState)(!1), 2),
                     c = l[0],
@@ -54628,15 +54686,15 @@
                     p = la();
 
                 function h() {
                     if (c) {
                         var e;
                         d(!1);
                         var t = null === (e = r.__result) || void 0 === e ? void 0 : e.get("action");
-                        t && (Aa(r, t, o, i, p), u[1](!1))
+                        t && (za(r, t, o, i, p), u[1](!1))
                     } else d(!0)
                 }
                 return (0, t.useEffect)((function() {
                     d(!1)
                 }), []), (0, Kr.jsx)(Kr.Fragment, {
                     children: r.__configuringCheckRun && (null === (n = r.__result) || void 0 === n ? void 0 : n.get("action")) && (0, Kr.jsx)(Kr.Fragment, {
                         children: (0, Kr.jsxs)("div", {
@@ -54788,15 +54846,15 @@
                                     })]
                                 })]
                             })]
                         })
                     })
                 })
             },
-            Xa = function(e) {
+            es = function(e) {
                 var n = pe().environ,
                     r = Xi({
                         initial: []
                     }),
                     o = Xi({
                         initial: []
                     }),
@@ -54807,15 +54865,15 @@
                 var c = Xi({
                         url: zt.Url("/checks/grouped/schedule", n),
                         nofetch: !0,
                         cache: !0,
                         onData: function(e) {
                             return e.sort((function(e, t) {
                                 return e.group > t.group ? 1 : e.group < t.group ? -1 : 0
-                            })), e.length > 0 && Ia(function(e) {
+                            })), e.length > 0 && Sa(function(e) {
                                 for (var t = null, n = 0; n < (null === e || void 0 === e ? void 0 : e.length); n++) {
                                     var r, o;
                                     (!t || (null === (r = e[n]) || void 0 === r || null === (o = r.checks) || void 0 === o ? void 0 : o.length) < t.checks.length) && (t = e[n])
                                 }
                                 return t
                             }(e), 0, o), e
                         }
@@ -54835,15 +54893,15 @@
                 var f = Xi();
 
                 function p() {
                     f.refresh(zt.Url("/checks_status", n))
                 }
 
                 function h(e, t, n, r) {
-                    Sa(e, n) ? Da(e, n, r) : Ia(e, 0, n)
+                    ka(e, n) ? La(e, n, r) : Sa(e, 0, n)
                 }
 
                 function g() {
                     l(!u), o.update([])
                 }
                 var y = function(e) {
                         e.props;
@@ -54960,15 +55018,15 @@
                                 },
                                 children: c.map((function(e, t) {
                                     var n;
                                     return (0, Kr.jsxs)("div", {
                                         children: [(0, Kr.jsxs)("span", {
                                             id: "tooltip-group-count-".concat(t),
                                             style: {
-                                                fontWeight: Sa(e, o) ? "bold" : "normal",
+                                                fontWeight: ka(e, o) ? "bold" : "normal",
                                                 cursor: "pointer"
                                             },
                                             onClick: function() {
                                                 return h(e, 0, o, r)
                                             },
                                             children: [e.group.replace(/ checks$/i, ""), " \xa0", (0, Kr.jsxs)("small", {
                                                 children: ["(", e.checks.length, ")"]
@@ -55198,15 +55256,15 @@
                                             children: [(0, Kr.jsx)("b", {
                                                 children: "Most Recent"
                                             }), ":\xa0"]
                                         }) : (0, Kr.jsxs)(Kr.Fragment, {
                                             children: [(0, Kr.jsx)("b", {
                                                 children: "Top"
                                             }), ":\xa0"]
-                                        }), (0, Kr.jsx)(Ma.FormatDuration, {
+                                        }), (0, Kr.jsx)(ja.FormatDuration, {
                                             start: null === C || void 0 === C || null === (u = C.data[0]) || void 0 === u ? void 0 : u.timestamp,
                                             verbose: !0,
                                             fallback: "just now",
                                             suffix: "ago",
                                             tooltip: !0
                                         })]
                                     }), (0, Kr.jsx)("b", {
@@ -55318,15 +55376,15 @@
                                                                 width: "45%"
                                                             },
                                                             children: [(0, Kr.jsx)("b", {
                                                                 style: {
                                                                     cursor: "pointer"
                                                                 },
                                                                 onClick: function() {
-                                                                    return Ea(P(e.check, e.group), n, r)
+                                                                    return Ta(P(e.check, e.group), n, r)
                                                                 },
                                                                 children: e.title
                                                             }), "\xa0\xa0", (0, Kr.jsxs)(Oe, {
                                                                 to: kr.Path("/checks/".concat(e.check, "/history")),
                                                                 rel: "noreferrer",
                                                                 target: "_blank",
                                                                 children: [(0, Kr.jsx)("small", {
@@ -55353,28 +55411,16 @@
                                                                     children: e.group
                                                                 })
                                                             }), "\xa0 \xa0\xa0"]
                                                         }), (0, Kr.jsxs)("td", {
                                                             style: {
                                                                 width: "10%"
                                                             },
-                                                            children: ["\xa0", "PASS" === e.status ? (0, Kr.jsx)(Kr.Fragment, {
-                                                                children: (0, Kr.jsx)("b", {
-                                                                    style: {
-                                                                        color: Ft.GetForegroundColor()
-                                                                    },
-                                                                    children: "OK"
-                                                                })
-                                                            }) : (0, Kr.jsx)(Kr.Fragment, {
-                                                                children: (0, Kr.jsx)("b", {
-                                                                    style: {
-                                                                        color: "darkred"
-                                                                    },
-                                                                    children: "ERROR"
-                                                                })
+                                                            children: ["\xa0", (0, Kr.jsx)(Ma, {
+                                                                status: e.status
                                                             }), "\xa0\xa0"]
                                                         }), (0, Kr.jsxs)("td", {
                                                             align: "right",
                                                             style: {
                                                                 width: "10%"
                                                             },
                                                             children: [e.duration, "\xa0\xa0"]
@@ -55792,15 +55838,15 @@
                                                                             children: [(0, Kr.jsx)("b", {
                                                                                 id: "tooltip-lambda-check-".concat(e.check_name),
                                                                                 style: {
                                                                                     color: Ft.GetForegroundColor(),
                                                                                     cursor: "pointer"
                                                                                 },
                                                                                 onClick: function() {
-                                                                                    return Ea(P(e.check_name, e.check_group), n, r)
+                                                                                    return Ta(P(e.check_name, e.check_group), n, r)
                                                                                 },
                                                                                 children: e.check_title
                                                                             }), " ", (0, Kr.jsx)("br", {}), (0, Kr.jsx)("i", {
                                                                                 id: "tooltip-lambda-check-group-".concat(e.check_name),
                                                                                 style: {
                                                                                     color: Ft.GetForegroundColor(),
                                                                                     cursor: "pointer"
@@ -55854,16 +55900,16 @@
                         },
                         children: (0, Kr.jsx)(Xr, {
                             loading: c.loading,
                             color: Ft.GetForegroundColor(),
                             size: 90
                         })
                     })
-                }) : (0, Kr.jsx)(Kr.Fragment, {
-                    children: (0, Kr.jsx)("div", {
+                }) : (0, Kr.jsxs)(Kr.Fragment, {
+                    children: [(0, Kr.jsx)(va, {}), (0, Kr.jsx)("div", {
                         children: (0, Kr.jsx)("table", {
                             children: (0, Kr.jsx)("tbody", {
                                 children: (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsxs)("td", {
                                         style: {
                                             paddingLeft: "4pt",
                                             verticalAlign: "top"
@@ -55883,60 +55929,60 @@
                                             }), (0, Kr.jsx)(N, {}), (0, Kr.jsx)("div", {
                                                 style: {
                                                     marginTop: "3pt",
                                                     marginBottom: "3pt",
                                                     height: "1px",
                                                     backgroundColor: "var(--box-fg)"
                                                 }
-                                            }), (0, Kr.jsx)(qa, {
+                                            }), (0, Kr.jsx)(Ka, {
                                                 showingChecksSearch: D,
                                                 toggleShowingChecksSearch: L
                                             })]
                                         }), (0, Kr.jsx)(F, {}), (0, Kr.jsx)(H, {})]
                                     }), (0, Kr.jsxs)("td", {
                                         style: {
                                             paddingLeft: "8pt",
                                             verticalAlign: "top"
                                         },
                                         children: [(0, Kr.jsx)(k, {
                                             info: i
-                                        }), (0, Kr.jsx)(Ua, {
+                                        }), (0, Kr.jsx)(Ra, {
                                             env: n,
                                             groupList: o,
                                             historyList: r,
                                             info: i,
                                             toggleShowingChecksSearch: L
                                         })]
                                     }), (0, Kr.jsxs)("td", {
                                         style: {
                                             paddingLeft: (null === o || void 0 === o ? void 0 : o.length) > 0 || o.error || j() ? "8pt" : "0",
                                             verticalAlign: "top"
                                         },
-                                        children: [(0, Kr.jsx)(Ja, {
+                                        children: [(0, Kr.jsx)(Xa, {
                                             checks: c,
                                             groupList: o,
                                             environ: n,
                                             findGroup: U,
                                             toggleShowGroup: h,
                                             showingChecksSearch: D,
                                             toggleShowingChecksSearch: L
-                                        }), (0, Kr.jsx)(Z, {}), (0, Kr.jsx)(B, {}), (0, Kr.jsx)(Za, {
+                                        }), (0, Kr.jsx)(Z, {}), (0, Kr.jsx)(B, {}), (0, Kr.jsx)(qa, {
                                             env: n,
                                             historyList: r
                                         })]
                                     })]
                                 })
                             })
                         })
-                    })
+                    })]
                 })
             },
-            $a = __webpack_require__(8145),
-            es = __webpack_require__.n($a),
-            ts = function(e) {
+            ts = __webpack_require__(8145),
+            ns = __webpack_require__.n(ts),
+            rs = function(e) {
                 var t = e.pages,
                     n = e.page,
                     r = e.onChange,
                     o = e.refresh,
                     i = e.loading,
                     a = e.spinner;
                 return (0, Kr.jsx)("table", {
@@ -55951,15 +55997,15 @@
                                         style: {
                                             pointerEvents: i ? "none" : "",
                                             opacity: i ? "0.4" : "",
                                             fontSize: "8pt",
                                             fontWeight: "bold"
                                         },
                                         className: "pagination-control",
-                                        children: (0, Kr.jsx)(es(), {
+                                        children: (0, Kr.jsx)(ns(), {
                                             nextLabel: "NEXT",
                                             onPageChange: r,
                                             pageRangeDisplayed: 2,
                                             initialPage: n,
                                             disableInitialCallback: !0,
                                             marginPagesDisplayed: 2,
                                             pageCount: t,
@@ -56014,23 +56060,23 @@
                                 })
                             })]
                         })
                     })
                 })
             };
 
-        function ns(e) {
+        function os(e) {
             var t;
             return null === e || void 0 === e || null === (t = e.split("/")) || void 0 === t ? void 0 : t.reverse()[0]
         }
 
-        function rs(e) {
+        function is(e) {
             return null === e || void 0 === e ? void 0 : e.substring(0, null === e || void 0 === e ? void 0 : e.lastIndexOf("/"))
         }
-        var os = function(e) {
+        var as = function(e) {
                 var t = e.check,
                     n = e.checkInfo;
                 return (0, Kr.jsx)(Kr.Fragment, {
                     children: (0, Kr.jsx)("div", {
                         className: "box",
                         children: (0, Kr.jsx)("table", {
                             children: (0, Kr.jsxs)("tbody", {
@@ -56145,16 +56191,16 @@
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsxs)("td", {
                                         children: [(0, Kr.jsx)("b", {
                                             children: "Code"
                                         }), ":"]
                                     }), (0, Kr.jsxs)("td", {
-                                        children: [ns(n.get("file")), " ", (0, Kr.jsx)("br", {}), (0, Kr.jsx)("small", {
-                                            children: rs(n.get("file"))
+                                        children: [os(n.get("file")), " ", (0, Kr.jsx)("br", {}), (0, Kr.jsx)("small", {
+                                            children: is(n.get("file"))
                                         })]
                                     })]
                                 }), (0, Kr.jsx)("tr", {
                                     children: (0, Kr.jsx)("td", {
                                         style: {
                                             paddingTop: "2px"
                                         }
@@ -56247,15 +56293,15 @@
                                     })]
                                 })]
                             })
                         })
                     })
                 })
             },
-            is = function(e) {
+            ss = function(e) {
                 var n, r = e.check,
                     o = e.checkInfo;
 
                 function i(e) {
                     var t = e.get("schedule");
                     if (t) {
                         var n = Object.values(t);
@@ -56519,16 +56565,16 @@
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsxs)("td", {
                                         children: [(0, Kr.jsx)("b", {
                                             children: "Code"
                                         }), ":"]
                                     }), (0, Kr.jsxs)("td", {
-                                        children: [ns(o.get("registered_file")), " ", (0, Kr.jsx)("br", {}), (0, Kr.jsx)("small", {
-                                            children: rs(o.get("registered_file"))
+                                        children: [os(o.get("registered_file")), " ", (0, Kr.jsx)("br", {}), (0, Kr.jsx)("small", {
+                                            children: is(o.get("registered_file"))
                                         })]
                                     })]
                                 }), (0, Kr.jsx)("tr", {
                                     children: (0, Kr.jsx)("td", {
                                         style: {
                                             paddingTop: "3px"
                                         }
@@ -56735,16 +56781,16 @@
                                             style: {
                                                 paddingRight: "8pt"
                                             },
                                             children: [(0, Kr.jsx)("b", {
                                                 children: "Code"
                                             }), ":"]
                                         }), (0, Kr.jsxs)("td", {
-                                            children: [ns(o.get("registered_action.file")), " ", (0, Kr.jsx)("br", {}), (0, Kr.jsx)("small", {
-                                                children: rs(o.get("registered_action.file"))
+                                            children: [os(o.get("registered_action.file")), " ", (0, Kr.jsx)("br", {}), (0, Kr.jsx)("small", {
+                                                children: is(o.get("registered_action.file"))
                                             })]
                                         })]
                                     }), (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             style: {
                                                 paddingTop: "3px"
                                             }
@@ -56844,15 +56890,15 @@
                                     })]
                                 })
                             })
                         })]
                     })]
                 })
             },
-            as = function(e) {
+            us = function(e) {
                 var n, r = pe(),
                     o = r.environ,
                     i = r.check,
                     s = a(Re(), 2),
                     u = s[0],
                     l = s[1],
                     c = a((0, t.useState)(parseInt(u.get("limit")) || 25), 2),
@@ -57109,34 +57155,16 @@
                                                     children: [a(e), "\xa0\xa0"]
                                                 }), (0, Kr.jsxs)("td", {
                                                     id: "tooltip-status-".concat(n),
                                                     style: {
                                                         verticalAlign: "top",
                                                         whiteSpace: "break-spaces"
                                                     },
-                                                    children: ["PASS" === s(e) ? (0, Kr.jsx)(Kr.Fragment, {
-                                                        children: (0, Kr.jsx)("b", {
-                                                            children: "OK"
-                                                        })
-                                                    }) : (0, Kr.jsx)(Kr.Fragment, {
-                                                        children: "FAIL" === s(e) ? (0, Kr.jsx)(Kr.Fragment, {
-                                                            children: (0, Kr.jsx)("b", {
-                                                                style: {
-                                                                    color: "darkred"
-                                                                },
-                                                                children: "FAILURE"
-                                                            })
-                                                        }) : (0, Kr.jsx)(Kr.Fragment, {
-                                                            children: (0, Kr.jsx)("b", {
-                                                                style: {
-                                                                    color: "darkred"
-                                                                },
-                                                                children: "ERROR"
-                                                            })
-                                                        })
+                                                    children: [(0, Kr.jsx)(Ma, {
+                                                        status: s(e)
                                                     }), (0, Kr.jsx)(Mi, {
                                                         id: "tooltip-status-".concat(n),
                                                         text: s(e),
                                                         position: "right",
                                                         shape: "squared",
                                                         offset: -12
                                                     }), "\xa0\xa0"]
@@ -57265,15 +57293,15 @@
                                         },
                                         children: (0, Kr.jsx)("tbody", {
                                             children: (0, Kr.jsxs)("tr", {
                                                 children: [(0, Kr.jsx)("td", {
                                                     style: {
                                                         width: "90%"
                                                     },
-                                                    children: (0, Kr.jsx)(ts, {
+                                                    children: (0, Kr.jsx)(rs, {
                                                         pages: x,
                                                         onChange: function(e) {
                                                             var t = e.selected * d % I.get("paging.total");
                                                             S(d, t, m)
                                                         },
                                                         refresh: function() {
                                                             return L(d, h, m)
@@ -57389,43 +57417,43 @@
                                     children: (0, Kr.jsx)(_, {
                                         history: I
                                     })
                                 }), (0, Kr.jsx)("td", {
                                     style: {
                                         verticalAlign: "top"
                                     },
-                                    children: "action" === D.get("type") ? (0, Kr.jsx)(os, {
+                                    children: "action" === D.get("type") ? (0, Kr.jsx)(as, {
                                         check: i,
                                         checkInfo: D
-                                    }) : (0, Kr.jsx)(is, {
+                                    }) : (0, Kr.jsx)(ss, {
                                         check: i,
                                         checkInfo: D
                                     })
                                 })]
                             })]
                         })
                     })
                 })
             },
-            ss = function() {
+            ls = function() {
                 var e = a((0, t.useContext)(ea), 2),
                     n = (e[0], e[1]),
                     r = $i();
                 return function(e) {
                     return r.refresh(zt.Url("/header", e), {
                         onData: function(e) {
                             return n(e)
                         },
                         cache: !0
                     })
                 }
             },
-            us = function(e) {
+            cs = function(e) {
                 var t, n, r = ta(),
-                    o = ss(),
+                    o = ls(),
                     i = Xi(Br.IsLoggedIn() ? zt.Url("/info") : null);
                 Ui.NoteLastUrl(r);
                 var a = fe();
 
                 function s() {
                     return At.IsKnown(At.Current(), r)
                 }
@@ -57760,15 +57788,15 @@
                             style: {
                                 marginTop: "8pt"
                             }
                         })]
                     })
                 })
             },
-            ls = function(e) {
+            ds = function(e) {
                 var t = ta();
                 return t.loading ? null : (0, Kr.jsxs)(Kr.Fragment, {
                     children: [(0, Kr.jsx)("br", {}), (0, Kr.jsx)("table", {
                         width: "100%",
                         children: (0, Kr.jsxs)("tbody", {
                             children: [(0, Kr.jsx)("tr", {
                                 style: {
@@ -57801,15 +57829,15 @@
                                 },
                                 children: (0, Kr.jsx)("td", {})
                             })]
                         })
                     })]
                 })
             },
-            cs = function(e) {
+            fs = function(e) {
                 var t = ta();
                 return (0, Kr.jsx)(Kr.Fragment, {
                     children: (0, Kr.jsx)("div", {
                         className: "container",
                         id: "login_container",
                         children: (0, Kr.jsxs)("div", {
                             className: "boxstyle check-error",
@@ -57848,15 +57876,15 @@
                                     })
                                 }), " page."]
                             })]
                         })
                     })
                 })
             },
-            ds = function() {
+            ps = function() {
                 var e = a(ma(), 2),
                     t = e[0],
                     n = e[1];
                 return (0, Kr.jsxs)(Kr.Fragment, {
                     children: [(0, Kr.jsx)("img", {
                         id: "tooltip-readonly",
                         alt: "lock",
@@ -57871,74 +57899,74 @@
                     }), (0, Kr.jsx)(Mi, {
                         id: "tooltip-readonly",
                         position: "bottom",
                         text: "You are in ".concat(t ? "readonly" : "read/write", " mode. Click to enter ").concat(t ? "read/write" : "readonly", " mode.")
                     })]
                 })
             },
-            fs = function(e) {
+            hs = function(e) {
                 var t = e.header;
                 return (0, Kr.jsxs)(Kr.Fragment, {
-                    children: [(0, Kr.jsx)(ps, {
+                    children: [(0, Kr.jsx)(gs, {
                         header: t
-                    }), (0, Kr.jsx)(hs, {
+                    }), (0, Kr.jsx)(ys, {
                         header: t
                     })]
                 })
             },
-            ps = function() {
+            gs = function() {
                 a(Re(), 1)[0];
                 var e = Xi("/certificates");
                 if (e.loading) return (0, Kr.jsx)(Kr.Fragment, {});
                 var t = e.find((function(e) {
                     return "Portal" === e.name
                 }));
-                return t && t.expires_soon ? (0, Kr.jsxs)(gs, {
+                return t && t.expires_soon ? (0, Kr.jsxs)(ms, {
                     children: [(0, Kr.jsx)("b", {
                         children: "Warning: SSL certificate for associated Portal will expire soon"
                     }), "\xa0", Fr.RightArrow, "\xa0 ", t.expires_at, " \xa0", Fr.RightArrow, "\xa0", Pr.FromNow(t.expires_at, !0, !1), "\xa0", Fr.RightArrow, "\xa0", (0, Kr.jsx)(Oe, {
                         to: kr.Path("/certificates"),
                         style: {
                             color: "inherit"
                         },
                         children: "View"
                     })]
                 }) : void 0
             },
-            hs = function(e) {
+            ys = function(e) {
                 e.header;
                 var t = Xi("/portal_access_key");
                 if (t.loading) return (0, Kr.jsx)(Kr.Fragment, {});
                 if (t) {
                     var n, r;
-                    if (null !== t && void 0 !== t && null !== (n = t.data) && void 0 !== n && n.expires_soon) return (0, Kr.jsxs)(gs, {
+                    if (null !== t && void 0 !== t && null !== (n = t.data) && void 0 !== n && n.expires_soon) return (0, Kr.jsxs)(ms, {
                         children: [(0, Kr.jsx)("b", {
                             children: "Warning: Access key for associated Portal will expire soon"
                         }), "\xa0", Fr.RightArrow, "\xa0 ", t.data.expires_at, " \xa0", Fr.RightArrow, "\xa0", Pr.FromNow(t.data.expires_at, !0, !1), "\xa0", Fr.RightArrow, "\xa0", (0, Kr.jsx)(Oe, {
                             to: kr.Path("/portal_access_key"),
                             style: {
                                 color: "inherit"
                             },
                             children: "View"
                         })]
                     });
-                    if (null !== (r = t.data) && void 0 !== r && r.invalid) return (0, Kr.jsxs)(gs, {
+                    if (null !== (r = t.data) && void 0 !== r && r.invalid) return (0, Kr.jsxs)(ms, {
                         children: [(0, Kr.jsxs)("b", {
                             children: ["Warning: Access key for associated Portal ", t.data.expired ? "has expired" : "is invalid"]
                         }), "\xa0", Fr.RightArrow, "\xa0", (0, Kr.jsx)(Oe, {
                             to: kr.Path("/portal_access_key"),
                             style: {
                                 color: "inherit"
                             },
                             children: "View"
                         })]
                     })
                 }
             },
-            gs = function(e) {
+            ms = function(e) {
                 var t = e.children;
                 return (0, Kr.jsxs)(Kr.Fragment, {
                     children: [(0, Kr.jsx)("tr", {
                         children: (0, Kr.jsx)("td", {
                             style: {
                                 background: "black",
                                 height: "2px"
@@ -57963,15 +57991,15 @@
                                 height: "1px"
                             },
                             colSpan: "3"
                         })
                     })]
                 })
             },
-            ys = function(e) {
+            vs = function(e) {
                 var t = e.header,
                     n = Ft.LightenDarkenColor(Ft.GetBackgroundColor(), -10),
                     r = function(e) {
                         var t = e.path,
                             n = e.label;
                         return (0, Kr.jsx)(Kr.Fragment, {
                             children: kr.CurrentLogicalPath() === t ? (0, Kr.jsxs)("span", {
@@ -58045,15 +58073,15 @@
                                 path: "/login",
                                 label: Br.IsLoggedIn(t) ? "Session" : "Login"
                             })]
                         })]
                     })
                 })
             },
-            ms = function(e) {
+            Ms = function(e) {
                 var t, n, r, o, i = e.header;
 
                 function a(e) {
                     return e ? {
                         textDecoration: "none",
                         color: "black",
                         fontWeight: "bold"
@@ -58129,29 +58157,29 @@
                     }), (0, Kr.jsx)(Mi, {
                         id: "tooltip-header-aws",
                         position: "bottom",
                         text: "Open AWS console for (".concat(null !== (n = i.app) && void 0 !== n && n.credentials.aws_account_name ? (null === (r = i.app) || void 0 === r ? void 0 : r.credentials.aws_account_name) + "/" : "").concat(null === (o = i.app) || void 0 === o ? void 0 : o.credentials.aws_account_number, ") account (in new tab).")
                     })]
                 })
             },
-            vs = function(e) {
+            bs = function(e) {
                 var t = e.header;
                 return (0, Kr.jsxs)("span", {
-                    children: [(0, Kr.jsx)(ys, {
+                    children: [(0, Kr.jsx)(vs, {
                         header: t
                     }), (0, Kr.jsx)(Kr.Fragment, {
                         children: "\xa0|\xa0"
-                    }), (0, Kr.jsx)(ms, {
+                    }), (0, Kr.jsx)(Ms, {
                         header: t
                     })]
                 })
             },
-            Ms = function(e) {
+            js = function(e) {
                 var n, r, o, i, s, u, l, c, d, f, p, h, g, y, m, v, M, b, j, w, x, N, I, D, S, L, k = ta(),
-                    C = ss(),
+                    C = ls(),
                     E = fe(),
                     _ = a(na(), 1)[0],
                     T = At.IsFoursightFourfront(k) ? "#14533C" : "#143C53",
                     A = Ft.LightenDarkenColor(Ft.GetBackgroundColor(), -10);
                 return (0, Kr.jsx)(Kr.Fragment, {
                     children: k.loading ? (0, Kr.jsxs)("div", {
                         style: {
@@ -58432,15 +58460,15 @@
                                             style: {
                                                 paddingRight: "10pt",
                                                 whiteSpace: "nowrap",
                                                 color: "#D6EAF8"
                                             },
                                             align: "right",
                                             children: [(0, Kr.jsx)("small", {
-                                                children: (0, Kr.jsx)(Ma.FormatDateTime, {
+                                                children: (0, Kr.jsx)(ja.FormatDateTime, {
                                                     verbose: !0,
                                                     timezone: !1
                                                 })
                                             }), (null === (c = k.app) || void 0 === c || null === (d = c.credentials) || void 0 === d ? void 0 : d.aws_account_name) && (0, Kr.jsxs)(Kr.Fragment, {
                                                 children: ["\xa0|\xa0", (0, Kr.jsx)(Oe, {
                                                     id: "tooltip-header-account",
                                                     to: kr.Path("/login"),
@@ -58498,15 +58526,15 @@
                                             width: "49%",
                                             style: {
                                                 paddingLeft: "10pt",
                                                 paddingTop: "3pt",
                                                 paddingBottom: "3pt",
                                                 whiteSpace: "nowrap"
                                             },
-                                            children: (0, Kr.jsx)(vs, {
+                                            children: (0, Kr.jsx)(bs, {
                                                 header: k
                                             })
                                         }), (0, Kr.jsx)("td", {
                                             width: "2%",
                                             align: "center",
                                             style: {
                                                 whiteSpace: "nowrap",
@@ -58828,15 +58856,15 @@
                                                                 })]
                                                             })
                                                         })]
                                                     })
                                                 })
                                             })
                                         })]
-                                    }), (0, Kr.jsx)(fs, {
+                                    }), (0, Kr.jsx)(hs, {
                                         header: k
                                     }), (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             style: {
                                                 height: "1px",
                                                 background: "darkblue"
                                             }
@@ -58854,25 +58882,25 @@
                                 children: (0, Kr.jsx)("table", {
                                     children: (0, Kr.jsx)("tbody", {
                                         children: (0, Kr.jsx)("tr", {
                                             children: (0, Kr.jsx)("td", {
                                                 style: {
                                                     paddingLeft: "10pt"
                                                 },
-                                                children: (0, Kr.jsx)(ds, {})
+                                                children: (0, Kr.jsx)(ps, {})
                                             })
                                         })
                                     })
                                 })
                             })]
                         })]
                     })
                 })
             },
-            bs = function(e) {
+            ws = function(e) {
                 var n = e.children,
                     r = a((0, t.useState)({
                         loading: !0
                     }), 2),
                     o = r[0],
                     i = r[1];
                 return Xi("/header", {
@@ -58888,15 +58916,15 @@
                     },
                     cache: !0
                 }), (0, Kr.jsx)(ea.Provider, {
                     value: [o, i],
                     children: n
                 })
             },
-            js = function(e) {
+            xs = function(e) {
                 var n, r, o, i, s, u, l, c, d, f, p, h, g, y, m, v, M, b, j, w = ta(),
                     x = (At.IsFoursightFourfront(w) ? "foursight" : "foursight-cgap") + ": " + (null === w || void 0 === w || null === (n = w.versions) || void 0 === n ? void 0 : n.foursight_core) + " | foursight-core: " + (null === w || void 0 === w || null === (r = w.versions) || void 0 === r ? void 0 : r.foursight) + " | dcicutils: " + (null === w || void 0 === w || null === (o = w.versions) || void 0 === o ? void 0 : o.dcicutils),
                     N = {
                         id: "".concat(null === (i = w.app) || void 0 === i || null === (s = i.credentials) || void 0 === s ? void 0 : s.aws_account_name, ":").concat(null === w || void 0 === w || null === (u = w.app) || void 0 === u ? void 0 : u.stage),
                         name: null === (l = w.app) || void 0 === l || null === (c = l.credentials) || void 0 === c ? void 0 : c.aws_account_name,
                         stage: null === (d = w.app) || void 0 === d ? void 0 : d.stage
                     },
@@ -59171,15 +59199,15 @@
                                     }
                                 })]
                             })
                         })]
                     })
                 })
             },
-            ws = function(e) {
+            Ns = function(e) {
                 var n = e.title,
                     r = e.show,
                     o = void 0 === r || r,
                     i = e.info,
                     s = e.children,
                     u = a((0, t.useState)(o), 2),
                     l = u[0],
@@ -59268,15 +59296,15 @@
                                     children: "show"
                                 }), "."]
                             })]
                         })
                     })
                 })
             },
-            xs = function(e) {
+            Is = function(e) {
                 var t = e.name,
                     n = e.value,
                     r = e.monospace,
                     o = void 0 !== r && r,
                     i = e.copy,
                     a = void 0 === i || i,
                     s = e.size,
@@ -59433,15 +59461,15 @@
                                     })]
                                 }), E]
                             }))]
                         }) : (0, Kr.jsx)("span", {})
                     })
                 })
             },
-            Ns = function() {
+            Ds = function() {
                 var e, n, r, o, i, s, u, l, c, d, f, p, h, g, y, m, v, M, b, j, w, x, N, I, D, S, L, k, C, E, _, T, A, O, z, U, P, R = ta(),
                     B = Xi("/info"),
                     F = a((0, t.useState)(!1), 2),
                     Y = F[0],
                     Q = F[1],
                     G = a((0, t.useState)(!1), 2),
                     W = G[0],
@@ -59452,238 +59480,238 @@
                     J = Xi("/portal_access_key"),
                     K = la();
                 return B.error ? (0, Kr.jsx)(xi, {
                     error: B.error,
                     message: "Error loading info from Foursight API"
                 }) : (0, Kr.jsxs)("div", {
                     className: "container",
-                    children: [(0, Kr.jsxs)(ws, {
+                    children: [(0, Kr.jsxs)(Ns, {
                         info: B,
                         title: "Versions",
-                        children: [(0, Kr.jsx)(xs, {
+                        children: [(0, Kr.jsx)(Is, {
                             name: null === (e = R.app) || void 0 === e ? void 0 : e.package,
                             value: null === (n = R.versions) || void 0 === n ? void 0 : n.foursight,
                             monospace: !0,
                             copy: !0,
                             pypi: !0,
                             github: At.IsFoursightFourfront(R) ? "4dn-dcic" : "dbmi-bgm",
                             size: "2"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "foursight-core",
                             value: null === (r = R.versions) || void 0 === r ? void 0 : r.foursight_core,
                             monospace: !0,
                             copy: !0,
                             pypi: !0,
                             github: "4dn-dcic",
                             size: "2"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "dcicutils",
                             value: null === (o = R.versions) || void 0 === o ? void 0 : o.dcicutils,
                             monospace: !0,
                             copy: !0,
                             pypi: !0,
                             github: "4dn-dcic",
                             size: "2"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "tibanna",
                             value: null === (i = R.versions) || void 0 === i ? void 0 : i.tibanna,
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             pypi: !0
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "tibanna-ff",
                             value: null === (s = R.versions) || void 0 === s ? void 0 : s.tibanna_ff,
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             pypi: !0
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "chalice",
                             value: null === (u = R.versions) || void 0 === u ? void 0 : u.chalice,
                             monospace: !0,
                             copy: !0,
                             chalice: !0,
                             size: "2",
                             pypi: !0,
                             github: "aws"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "python",
                             value: null === (l = R.versions) || void 0 === l ? void 0 : l.python,
                             monospace: !0,
                             copy: !0,
                             python: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "elasticsearch-server",
                             value: (null === (c = R.versions) || void 0 === c ? void 0 : c.elasticsearch_server) || (null === (d = B.data) || void 0 === d || null === (f = d.versions) || void 0 === f ? void 0 : f.elasticsearch_server),
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             elasticsearch: !0
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "elasticsearch",
                             value: null === (p = R.versions) || void 0 === p ? void 0 : p.elasticsearch,
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             pypi: !0
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "elasticsearch-dsl",
                             value: null === (h = R.versions) || void 0 === h ? void 0 : h.elasticsearch_dsl,
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             pypi: !0
                         })]
-                    }), (0, Kr.jsxs)(ws, {
+                    }), (0, Kr.jsxs)(Ns, {
                         info: B,
                         title: "Credentials Info",
-                        children: [(0, Kr.jsx)(xs, {
+                        children: [(0, Kr.jsx)(Is, {
                             name: "AWS Account Number",
                             value: B.get("app.credentials.aws_account_number"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "AWS Region Name",
                             value: B.get("app.credentials.aws_region"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "AWS User ARN",
                             value: B.get("app.credentials.aws_user_arn"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "AWS Access Key ID",
                             value: B.get("app.credentials.aws_access_key_id"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), B.get("environ.S3_AWS_ACCESS_KEY_ID") && (0, Kr.jsx)(xs, {
+                        }), B.get("environ.S3_AWS_ACCESS_KEY_ID") && (0, Kr.jsx)(Is, {
                             name: "AWS S3 Access Key ID",
                             value: B.get("environ.S3_AWS_ACCESS_KEY_ID"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "Portal Access Key",
                             value: J.get("key"),
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             portalAccessKey: !0
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "Auth0 Client ID",
                             value: B.get("app.credentials.auth0_client_id"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         })]
-                    }), (0, Kr.jsxs)(ws, {
+                    }), (0, Kr.jsxs)(Ns, {
                         info: B,
                         title: "Resources",
-                        children: [(0, Kr.jsx)(xs, {
+                        children: [(0, Kr.jsx)(Is, {
                             name: "Foursight Server",
                             value: B.get("server.foursight"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "Portal Server",
                             value: B.get("server.portal"),
                             monospace: !0,
                             copy: !0,
                             size: "2",
                             portalCertificate: !0
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "ElasticSearch Server",
                             value: B.get("server.es"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "RDS Server",
                             value: B.get("server.rds"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "SQS Server",
                             value: B.get("server.sqs"),
                             monospace: !0,
                             copy: !0,
                             size: "2"
                         })]
-                    }), (0, Kr.jsxs)(ws, {
+                    }), (0, Kr.jsxs)(Ns, {
                         info: B,
                         title: "Environment Names",
-                        children: [(0, Kr.jsx)(xs, {
+                        children: [(0, Kr.jsx)(Is, {
                             name: "Environment Name",
                             value: At.RegularName(At.Current(), R),
                             monospace: !0,
                             copy: !0,
                             size: "3"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "Environment Name (Full)",
                             value: At.FullName(At.Current(), R),
                             monospace: !0,
                             copy: !0,
                             size: "3"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "Environment Name (Short)",
                             value: At.ShortName(At.Current(), R),
                             monospace: !0,
                             copy: !0,
                             size: "3"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "Environment Name (Public)",
                             value: At.PublicName(At.Current(), R),
                             monospace: !0,
                             copy: !0,
                             size: "3"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "Environment Name (Foursight)",
                             value: At.FoursightName(At.Current(), R),
                             monospace: !0,
                             copy: !0,
                             size: "3"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "Environment Name (Preferred)",
                             value: At.PreferredName(At.Current(R), R),
                             monospace: !0,
                             copy: !0,
                             size: "3"
                         })]
-                    }), (0, Kr.jsxs)(ws, {
+                    }), (0, Kr.jsxs)(Ns, {
                         info: B,
                         title: "Bucket Names",
-                        children: [(0, Kr.jsx)(xs, {
+                        children: [(0, Kr.jsx)(Is, {
                             name: "Global Environment Bucket",
                             value: B.get("buckets.env"),
                             monospace: !0,
                             copy: !0,
                             size: "3"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "Foursight Bucket Name",
                             value: B.get("buckets.foursight"),
                             monospace: !0,
                             copy: !0,
                             size: "3"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "Foursight Bucket Prefix",
                             value: B.get("buckets.foursight_prefix"),
                             monospace: !0,
                             copy: !0,
                             size: "3"
                         })]
-                    }), (0, Kr.jsx)(ws, {
+                    }), (0, Kr.jsx)(Ns, {
                         info: B,
                         title: "Environment & Bucket Names",
                         children: (0, Kr.jsx)("pre", {
                             className: "box",
                             style: {
                                 border: "0",
                                 margin: "0",
@@ -59698,84 +59726,84 @@
                                         marginTop: "6px",
                                         marginBottom: "6px",
                                         background: "black"
                                     }
                                 }) : (0, Kr.jsx)("span", {})]
                             }, Dr()())
                         })
-                    }), (0, Kr.jsx)(ws, {
+                    }), (0, Kr.jsx)(Ns, {
                         info: B,
                         title: "Ecosystem",
                         show: !1,
                         children: (0, Kr.jsx)("pre", {
                             className: "box",
                             style: {
                                 border: "0",
                                 margin: "0",
                                 paddingTop: "8",
                                 paddingBottom: "8",
                                 marginTop: "0"
                             },
                             children: Bi.Format(B.get("buckets.ecosystem"))
                         })
-                    }), (0, Kr.jsxs)(ws, {
+                    }), (0, Kr.jsxs)(Ns, {
                         info: B,
                         title: "Authentication/Authorization Info",
                         show: !1,
-                        children: [(0, Kr.jsx)(xs, {
+                        children: [(0, Kr.jsx)(Is, {
                             name: "Email",
                             value: null === (y = Br.Token()) || void 0 === y ? void 0 : y.user,
                             monospace: !0,
                             copy: !0,
                             check: null === (m = Br.Token()) || void 0 === m ? void 0 : m.user_verified,
                             link: kr.Path("/users/" + Br.LoggedInUser(R), !0),
                             size: "2"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "First Name",
                             value: null === (v = Br.Token()) || void 0 === v ? void 0 : v.first_name,
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "Last Name",
                             value: null === (M = Br.Token()) || void 0 === M ? void 0 : M.last_name,
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "Environments",
                             value: null === (b = Br.Token()) || void 0 === b ? void 0 : b.allowed_envs.join(", "),
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "Audience",
                             value: null === (j = Br.Token()) || void 0 === j ? void 0 : j.aud,
                             monospace: !0,
                             copy: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "Issued At",
                             monospace: !0,
                             copy: !0,
                             size: "2",
-                            value: (0, Kr.jsx)(Ma.FormatDuration, {
+                            value: (0, Kr.jsx)(ja.FormatDuration, {
                                 start: null === (w = Br.Token()) || void 0 === w ? void 0 : w.authenticated_at,
                                 verbose: !0,
                                 fallback: "just now",
                                 suffix: "ago",
                                 tooltip: !0,
                                 prefix: "datetime"
                             })
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "Expires At",
                             monospace: !0,
                             copy: !0,
                             size: "2",
-                            value: (0, Kr.jsx)(Ma.FormatDuration, {
+                            value: (0, Kr.jsx)(ja.FormatDuration, {
                                 end: null === (x = Br.Token()) || void 0 === x ? void 0 : x.authenticated_until,
                                 verbose: !0,
                                 fallback: "now",
                                 suffix: "from now",
                                 tooltip: !0,
                                 prefix: "datetime"
                             })
@@ -59840,70 +59868,70 @@
                                     children: [(0, Kr.jsx)("u", {
                                         children: "AuthToken"
                                     }), "\xa0", Fr.UpArrow]
                                 })
                             }), (0, Kr.jsx)("br", {})]
                         })]
                     }), B.get("environ.AWS_LAMBDA_LOG_GROUP_NAME") && B.get("environ.AWS_LAMBDA_LOG_STREAM_NAME") && (0, Kr.jsx)(Kr.Fragment, {
-                        children: (0, Kr.jsxs)(ws, {
+                        children: (0, Kr.jsxs)(Ns, {
                             info: B,
                             title: "Logs",
-                            children: [(0, Kr.jsx)(xs, {
+                            children: [(0, Kr.jsx)(Is, {
                                 name: "Log Group",
                                 value: B.get("environ.AWS_LAMBDA_LOG_GROUP_NAME"),
                                 monospace: !0,
                                 size: "2"
-                            }), (0, Kr.jsx)(xs, {
+                            }), (0, Kr.jsx)(Is, {
                                 name: "Log Stream",
                                 value: B.get("environ.AWS_LAMBDA_LOG_STREAM_NAME"),
                                 monospace: !0,
                                 size: "2"
                             })]
                         })
-                    }), B.get("app.lambda") && (0, Kr.jsxs)(ws, {
+                    }), B.get("app.lambda") && (0, Kr.jsxs)(Ns, {
                         info: B,
                         title: "Lambda",
                         show: !1,
-                        children: [(0, Kr.jsx)(xs, {
+                        children: [(0, Kr.jsx)(Is, {
                             name: "Name",
                             value: B.get("app.lambda.lambda_name"),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "Function",
                             value: B.get("app.lambda.lambda_function_name"),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "ARN",
                             value: B.get("app.lambda.lambda_function_arn"),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "S3 Location",
                             value: B.get("app.lambda.lambda_code_s3_bucket") + "/" + B.get("app.lambda.lambda_code_s3_bucket_key"),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "Size",
                             value: B.get("app.lambda.lambda_code_size"),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "Modified",
                             value: Pr.FormatDateTime(B.get("app.lambda.lambda_modified")),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "Role",
                             value: B.get("app.lambda.lambda_role"),
                             monospace: !0,
                             size: "2"
                         })]
-                    }), (0, Kr.jsxs)(ws, {
+                    }), (0, Kr.jsxs)(Ns, {
                         info: B,
                         title: "Miscellany",
                         children: [V ? (0, Kr.jsxs)(Kr.Fragment, {
                             children: [(0, Kr.jsx)("div", {
                                 id: "tooltip-info-reloading",
                                 style: {
                                     float: "right"
@@ -59957,114 +59985,114 @@
                                 }
                             })]
                         }), (0, Kr.jsx)(Mi, {
                             id: "tooltip-info-clear",
                             position: "bottom",
                             size: "small",
                             text: "Click to clear any server-side caches."
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "App Deployed At",
                             value: zt.IsLocal() ? "running locally" + (Je.IsLocalCrossOrigin() ? " (cross-origin)" : "") : (null === (N = R.app) || void 0 === N ? void 0 : N.deployed) + Pr.FormatDuration(null === (I = R.app) || void 0 === I ? void 0 : I.deployed, new Date, !0, "just now", "|", "ago"),
                             monospace: !0,
                             copy: !0,
                             optional: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "App Launched At",
                             value: (null === (D = R.app) || void 0 === D ? void 0 : D.launched) + Pr.FormatDuration(null === (S = R.app) || void 0 === S ? void 0 : S.launched, new Date, !0, "just now", "|", "ago"),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "Page Loaded At",
                             value: B.get("page.loaded") + Pr.FormatDuration(B.get("page.loaded"), new Date, !0, "just now", "|", "ago"),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "Package",
                             value: null === (L = R.app) || void 0 === L ? void 0 : L.package,
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "Stage",
                             value: null === (k = R.app) || void 0 === k ? void 0 : k.stage,
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "Environment",
                             value: At.Current(),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "Domain",
                             value: null === (C = R.app) || void 0 === C ? void 0 : C.domain,
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "Context",
                             value: null === (E = R.app) || void 0 === E ? void 0 : E.context,
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "Path",
                             value: B.get("page.path"),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "Endpoint",
                             value: B.get("page.endpoint"),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "Client (React UI)",
                             value: kr.BaseUrl(),
                             monospace: !0,
                             size: "2"
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "Server (React API)",
                             value: zt.BaseUrl(),
                             monospace: !0,
                             size: "2",
                             apiCache: !0
-                        }), (0, Kr.jsx)(xs, {
+                        }), (0, Kr.jsx)(Is, {
                             name: "Checks File",
                             value: null === (_ = B.data) || void 0 === _ || null === (T = _.checks) || void 0 === T ? void 0 : T.file,
                             monospace: !0,
                             size: "2"
-                        }), (null === (A = R.app) || void 0 === A ? void 0 : A.accounts_file) && (0, Kr.jsx)(xs, {
+                        }), (null === (A = R.app) || void 0 === A ? void 0 : A.accounts_file) && (0, Kr.jsx)(Is, {
                             name: "Accounts File",
                             value: null === (O = R.app) || void 0 === O ? void 0 : O.accounts_file,
                             monospace: !0,
                             size: "2"
-                        }), (null === (z = R.app) || void 0 === z ? void 0 : z.accounts_file_from_s3) && (0, Kr.jsx)(xs, {
+                        }), (null === (z = R.app) || void 0 === z ? void 0 : z.accounts_file_from_s3) && (0, Kr.jsx)(Is, {
                             name: "Accounts File (S3)",
                             value: null === (U = R.app) || void 0 === U ? void 0 : U.accounts_file_from_s3,
                             monospace: !0,
                             size: "2"
                         })]
-                    }), (0, Kr.jsx)(ws, {
+                    }), (0, Kr.jsx)(Ns, {
                         info: B,
                         title: "GAC: ".concat(B.get("gac.name")),
                         show: !1,
                         children: B.get("gac.values") ? (0, Kr.jsx)("span", {
                             children: Object.keys(B.get("gac.values")).map((function(e) {
-                                return (0, Kr.jsx)(xs, {
+                                return (0, Kr.jsx)(Is, {
                                     name: e,
                                     value: B.get("gac.values")[e],
                                     monospace: !0,
                                     copy: !0
                                 }, e)
                             }))
                         }) : (0, Kr.jsx)("span", {})
-                    }), (0, Kr.jsx)(ws, {
+                    }), (0, Kr.jsx)(Ns, {
                         info: B,
                         title: "Environment Variables",
                         show: !1,
                         children: B.get("environ") ? (0, Kr.jsx)("span", {
                             children: Object.keys(B.get("environ")).map((function(e) {
-                                return (0, Kr.jsx)(xs, {
+                                return (0, Kr.jsx)(Is, {
                                     name: e,
                                     value: B.get("environ")[e],
                                     monospace: !0,
                                     copy: !0
                                 }, e)
                             }))
                         }) : (0, Kr.jsx)("span", {})
@@ -60104,40 +60132,40 @@
                                     children: "show"
                                 }), "."]
                             })]
                         })
                     })]
                 })
             },
-            Is = function(e, t) {
-                return Is = Object.setPrototypeOf || {
+            Ss = function(e, t) {
+                return Ss = Object.setPrototypeOf || {
                     __proto__: []
                 }
                 instanceof Array && function(e, t) {
                     e.__proto__ = t
                 } || function(e, t) {
                     for (var n in t) t.hasOwnProperty(n) && (e[n] = t[n])
-                }, Is(e, t)
+                }, Ss(e, t)
             };
 
-        function Ds(e, t) {
+        function Ls(e, t) {
             function n() {
                 this.constructor = e
             }
-            Is(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
+            Ss(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
         }
-        var Ss, Ls, ks, Cs = function() {
-            return Cs = Object.assign || function(e) {
+        var ks, Cs, Es, _s = function() {
+            return _s = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, Cs.apply(this, arguments)
+            }, _s.apply(this, arguments)
         };
 
-        function Es(e, t, n, r) {
+        function Ts(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -60157,15 +60185,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function _s(e, t) {
+        function As(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -60233,15 +60261,15 @@
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
 
-        function Ts(e, t) {
+        function Os(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -60255,50 +60283,50 @@
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
 
-        function As(e) {
+        function zs(e) {
             return e && !!["provider"].find((function(t) {
                 return e.hasOwnProperty(t)
             }))
         }
 
-        function Os(e) {
+        function Us(e) {
             return void 0 !== e.redirectSignIn
         }! function(e) {
             e.Cognito = "COGNITO", e.Google = "Google", e.Facebook = "Facebook", e.Amazon = "LoginWithAmazon", e.Apple = "SignInWithApple"
-        }(Ss || (Ss = {})),
+        }(ks || (ks = {})),
         function(e) {
             e.NoConfig = "noConfig", e.MissingAuthConfig = "missingAuthConfig", e.EmptyUsername = "emptyUsername", e.InvalidUsername = "invalidUsername", e.EmptyPassword = "emptyPassword", e.EmptyCode = "emptyCode", e.SignUpError = "signUpError", e.NoMFA = "noMFA", e.InvalidMFA = "invalidMFA", e.EmptyChallengeResponse = "emptyChallengeResponse", e.NoUserSession = "noUserSession", e.Default = "default", e.DeviceConfig = "deviceConfig", e.NetworkError = "networkError", e.AutoSignInError = "autoSignInError"
-        }(Ls || (Ls = {})),
+        }(Cs || (Cs = {})),
         function(e) {
             e.API_KEY = "API_KEY", e.AWS_IAM = "AWS_IAM", e.OPENID_CONNECT = "OPENID_CONNECT", e.AMAZON_COGNITO_USER_POOLS = "AMAZON_COGNITO_USER_POOLS", e.AWS_LAMBDA = "AWS_LAMBDA"
-        }(ks || (ks = {}));
-        var zs = function(e, t) {
-            return zs = Object.setPrototypeOf || {
+        }(Es || (Es = {}));
+        var Ps = function(e, t) {
+            return Ps = Object.setPrototypeOf || {
                 __proto__: []
             }
             instanceof Array && function(e, t) {
                 e.__proto__ = t
             } || function(e, t) {
                 for (var n in t) t.hasOwnProperty(n) && (e[n] = t[n])
-            }, zs(e, t)
+            }, Ps(e, t)
         };
-        var Us = function() {
-            return Us = Object.assign || function(e) {
+        var Rs = function() {
+            return Rs = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, Us.apply(this, arguments)
+            }, Rs.apply(this, arguments)
         };
 
-        function Ps(e, t, n, r) {
+        function Bs(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -60318,15 +60346,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function Rs(e, t) {
+        function Fs(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -60394,15 +60422,15 @@
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
 
-        function Bs(e) {
+        function Ys(e) {
             var t = "function" === typeof Symbol && Symbol.iterator,
                 n = t && e[t],
                 r = 0;
             if (n) return n.call(e);
             if (e && "number" === typeof e.length) return {
                 next: function() {
                     return e && r >= e.length && (e = void 0), {
@@ -60410,15 +60438,15 @@
                         done: !e
                     }
                 }
             };
             throw new TypeError(t ? "Object is not iterable." : "Symbol.iterator is not defined.")
         }
 
-        function Fs(e, t) {
+        function Qs(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -60432,58 +60460,58 @@
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
 
-        function Ys() {
-            for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(Fs(arguments[t]));
+        function Gs() {
+            for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(Qs(arguments[t]));
             return e
         }
-        var Qs, Gs = {
+        var Ws, Hs = {
             VERBOSE: 1,
             DEBUG: 2,
             INFO: 3,
             WARN: 4,
             ERROR: 5
         };
         ! function(e) {
             e.DEBUG = "DEBUG", e.ERROR = "ERROR", e.INFO = "INFO", e.WARN = "WARN", e.VERBOSE = "VERBOSE"
-        }(Qs || (Qs = {}));
-        var Ws = function() {
+        }(Ws || (Ws = {}));
+        var Zs = function() {
                 function e(e, t) {
-                    void 0 === t && (t = Qs.WARN), this.name = e, this.level = t, this._pluggables = []
+                    void 0 === t && (t = Ws.WARN), this.name = e, this.level = t, this._pluggables = []
                 }
                 return e.prototype._padding = function(e) {
                     return e < 10 ? "0" + e : "" + e
                 }, e.prototype._ts = function() {
                     var e = new Date;
                     return [this._padding(e.getMinutes()), this._padding(e.getSeconds())].join(":") + "." + e.getMilliseconds()
                 }, e.prototype.configure = function(e) {
                     return e ? (this._config = e, this._config) : this._config
                 }, e.prototype._log = function(t) {
                     for (var n, r, o = [], i = 1; i < arguments.length; i++) o[i - 1] = arguments[i];
                     var a = this.level;
                     e.LOG_LEVEL && (a = e.LOG_LEVEL), "undefined" !== typeof window && window.LOG_LEVEL && (a = window.LOG_LEVEL);
-                    var s = Gs[a],
-                        u = Gs[t];
+                    var s = Hs[a],
+                        u = Hs[t];
                     if (u >= s) {
                         var l = console.log.bind(console);
-                        t === Qs.ERROR && console.error && (l = console.error.bind(console)), t === Qs.WARN && console.warn && (l = console.warn.bind(console));
+                        t === Ws.ERROR && console.error && (l = console.error.bind(console)), t === Ws.WARN && console.warn && (l = console.warn.bind(console));
                         var c = "[" + t + "] " + this._ts() + " " + this.name,
                             d = "";
                         if (1 === o.length && "string" === typeof o[0]) l(d = c + " - " + o[0]);
                         else if (1 === o.length) d = c + " " + o[0], l(c, o[0]);
                         else if ("string" === typeof o[0]) {
                             var f = o.slice(1);
                             1 === f.length && (f = f[0]), d = c + " - " + o[0] + " " + f, l(c + " - " + o[0], f)
                         } else d = c + " " + o, l(c, o);
                         try {
-                            for (var p = Bs(this._pluggables), h = p.next(); !h.done; h = p.next()) {
+                            for (var p = Ys(this._pluggables), h = p.next(); !h.done; h = p.next()) {
                                 var g = h.value,
                                     y = {
                                         message: d,
                                         timestamp: Date.now()
                                     };
                                 g.pushLogs([y])
                             }
@@ -60497,78 +60525,78 @@
                             } finally {
                                 if (n) throw n.error
                             }
                         }
                     }
                 }, e.prototype.log = function() {
                     for (var e = [], t = 0; t < arguments.length; t++) e[t] = arguments[t];
-                    this._log.apply(this, Ys([Qs.INFO], e))
+                    this._log.apply(this, Gs([Ws.INFO], e))
                 }, e.prototype.info = function() {
                     for (var e = [], t = 0; t < arguments.length; t++) e[t] = arguments[t];
-                    this._log.apply(this, Ys([Qs.INFO], e))
+                    this._log.apply(this, Gs([Ws.INFO], e))
                 }, e.prototype.warn = function() {
                     for (var e = [], t = 0; t < arguments.length; t++) e[t] = arguments[t];
-                    this._log.apply(this, Ys([Qs.WARN], e))
+                    this._log.apply(this, Gs([Ws.WARN], e))
                 }, e.prototype.error = function() {
                     for (var e = [], t = 0; t < arguments.length; t++) e[t] = arguments[t];
-                    this._log.apply(this, Ys([Qs.ERROR], e))
+                    this._log.apply(this, Gs([Ws.ERROR], e))
                 }, e.prototype.debug = function() {
                     for (var e = [], t = 0; t < arguments.length; t++) e[t] = arguments[t];
-                    this._log.apply(this, Ys([Qs.DEBUG], e))
+                    this._log.apply(this, Gs([Ws.DEBUG], e))
                 }, e.prototype.verbose = function() {
                     for (var e = [], t = 0; t < arguments.length; t++) e[t] = arguments[t];
-                    this._log.apply(this, Ys([Qs.VERBOSE], e))
+                    this._log.apply(this, Gs([Ws.VERBOSE], e))
                 }, e.prototype.addPluggable = function(e) {
                     e && "Logging" === e.getCategoryName() && (this._pluggables.push(e), e.configure(this._config))
                 }, e.prototype.listPluggables = function() {
                     return this._pluggables
                 }, e.LOG_LEVEL = null, e
             }(),
-            Hs = new Ws("Hub"),
-            Zs = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default";
-        var Vs = function() {
+            Vs = new Zs("Hub"),
+            qs = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default";
+        var Js = function() {
                 function e(e) {
                     this.listeners = [], this.patterns = [], this.protectedChannels = ["core", "auth", "api", "analytics", "interactions", "pubsub", "storage", "ui", "xr"], this.name = e
                 }
                 return e.prototype._remove = function(e, t) {
                     if (e instanceof RegExp) {
                         var n = this.patterns.find((function(t) {
                             return t.pattern.source === e.source
                         }));
-                        if (!n) return void Hs.warn("No listeners for " + e);
-                        this.patterns = Ys(this.patterns.filter((function(e) {
+                        if (!n) return void Vs.warn("No listeners for " + e);
+                        this.patterns = Gs(this.patterns.filter((function(e) {
                             return e !== n
                         })))
                     } else {
                         var r = this.listeners[e];
-                        if (!r) return void Hs.warn("No listeners for " + e);
-                        this.listeners[e] = Ys(r.filter((function(e) {
+                        if (!r) return void Vs.warn("No listeners for " + e);
+                        this.listeners[e] = Gs(r.filter((function(e) {
                             return e.callback !== t
                         })))
                     }
                 }, e.prototype.remove = function(e, t) {
                     this._remove(e, t)
                 }, e.prototype.dispatch = function(e, t, n, r) {
-                    (void 0 === n && (n = ""), this.protectedChannels.indexOf(e) > -1) && (r === Zs || Hs.warn("WARNING: " + e + " is protected and dispatching on it can have unintended consequences"));
+                    (void 0 === n && (n = ""), this.protectedChannels.indexOf(e) > -1) && (r === qs || Vs.warn("WARNING: " + e + " is protected and dispatching on it can have unintended consequences"));
                     var o = {
                         channel: e,
-                        payload: Us({}, t),
+                        payload: Rs({}, t),
                         source: n,
                         patternInfo: []
                     };
                     try {
                         this._toListeners(o)
                     } catch (i) {
-                        Hs.error(i)
+                        Vs.error(i)
                     }
                 }, e.prototype.listen = function(e, t, n) {
                     var r, o = this;
                     if (void 0 === n && (n = "noname"), function(e) {
                             return void 0 !== e.onHubCapsule
-                        }(t)) Hs.warn("WARNING onHubCapsule is Deprecated. Please pass in a callback."), r = t.onHubCapsule.bind(t);
+                        }(t)) Vs.warn("WARNING onHubCapsule is Deprecated. Please pass in a callback."), r = t.onHubCapsule.bind(t);
                     else {
                         if ("function" !== typeof t) throw new Error("No callback supplied to Hub");
                         r = t
                     }
                     if (e instanceof RegExp) this.patterns.push({
                         pattern: e,
                         callback: r
@@ -60584,115 +60612,115 @@
                         o._remove(e, r)
                     }
                 }, e.prototype._toListeners = function(e) {
                     var t = e.channel,
                         n = e.payload,
                         r = this.listeners[t];
                     if (r && r.forEach((function(r) {
-                            Hs.debug("Dispatching to " + t + " with ", n);
+                            Vs.debug("Dispatching to " + t + " with ", n);
                             try {
                                 r.callback(e)
                             } catch (o) {
-                                Hs.error(o)
+                                Vs.error(o)
                             }
                         })), this.patterns.length > 0) {
-                        if (!n.message) return void Hs.warn("Cannot perform pattern matching without a message key");
+                        if (!n.message) return void Vs.warn("Cannot perform pattern matching without a message key");
                         var o = n.message;
                         this.patterns.forEach((function(t) {
                             var n = o.match(t.pattern);
                             if (n) {
-                                var r = Fs(n).slice(1),
-                                    i = Us(Us({}, e), {
+                                var r = Qs(n).slice(1),
+                                    i = Rs(Rs({}, e), {
                                         patternInfo: r
                                     });
                                 try {
                                     t.callback(i)
                                 } catch (a) {
-                                    Hs.error(a)
+                                    Vs.error(a)
                                 }
                             }
                         }))
                     }
                 }, e
             }(),
-            qs = new Vs("__default__"),
-            Js = {},
-            Ks = function() {
+            Ks = new Js("__default__"),
+            Xs = {},
+            $s = function() {
                 function e() {}
                 return e.setItem = function(e, t) {
-                    return Js[e] = t, Js[e]
+                    return Xs[e] = t, Xs[e]
                 }, e.getItem = function(e) {
-                    return Object.prototype.hasOwnProperty.call(Js, e) ? Js[e] : void 0
+                    return Object.prototype.hasOwnProperty.call(Xs, e) ? Xs[e] : void 0
                 }, e.removeItem = function(e) {
-                    return delete Js[e]
+                    return delete Xs[e]
                 }, e.clear = function() {
-                    return Js = {}
+                    return Xs = {}
                 }, e
             }(),
-            Xs = function() {
+            eu = function() {
                 function e() {
                     try {
                         this.storageWindow = window.localStorage, this.storageWindow.setItem("aws.amplify.test-ls", 1), this.storageWindow.removeItem("aws.amplify.test-ls")
                     } catch (e) {
-                        this.storageWindow = Ks
+                        this.storageWindow = $s
                     }
                 }
                 return e.prototype.getStorage = function() {
                     return this.storageWindow
                 }, e
             }(),
-            $s = function() {
+            tu = function() {
                 return {
                     isBrowser: "undefined" !== typeof window && "undefined" !== typeof window.document,
                     isNode: "undefined" !== typeof process && null != process.versions && null != process.versions.node
                 }
             },
-            eu = new Ws("Util"),
-            tu = function(e) {
+            nu = new Zs("Util"),
+            ru = function(e) {
                 function t(t) {
                     var n = e.call(this, t) || this;
                     return n.nonRetryable = !0, n
                 }
                 return function(e, t) {
                     function n() {
                         this.constructor = e
                     }
-                    zs(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
+                    Ps(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
                 }(t, e), t
             }(Error);
-        var nu = 3e5;
-        var ru = function(e, t, n, r) {
-                return void 0 === n && (n = nu),
+        var ou = 3e5;
+        var iu = function(e, t, n, r) {
+                return void 0 === n && (n = ou),
                     function(e, t, n, r) {
-                        return Ps(this, void 0, void 0, (function() {
+                        return Bs(this, void 0, void 0, (function() {
                             var o = this;
-                            return Rs(this, (function(i) {
+                            return Fs(this, (function(i) {
                                 if ("function" !== typeof e) throw Error("functionToRetry must be a function");
                                 return [2, new Promise((function(i, a) {
-                                    return Ps(o, void 0, void 0, (function() {
+                                    return Bs(o, void 0, void 0, (function() {
                                         var o, s, u, l, c, d, f;
-                                        return Rs(this, (function(p) {
+                                        return Fs(this, (function(p) {
                                             switch (p.label) {
                                                 case 0:
                                                     o = 0, s = !1, l = function() {}, r && r.then((function() {
                                                         s = !0, clearTimeout(u), l()
                                                     })), d = function() {
                                                         var r, d, f, p;
-                                                        return Rs(this, (function(h) {
+                                                        return Fs(this, (function(h) {
                                                             switch (h.label) {
                                                                 case 0:
-                                                                    o++, eu.debug(e.name + " attempt #" + o + " with this vars: " + JSON.stringify(t)), h.label = 1;
+                                                                    o++, nu.debug(e.name + " attempt #" + o + " with this vars: " + JSON.stringify(t)), h.label = 1;
                                                                 case 1:
-                                                                    return h.trys.push([1, 3, , 7]), r = {}, d = i, [4, e.apply(void 0, Ys(t))];
+                                                                    return h.trys.push([1, 3, , 7]), r = {}, d = i, [4, e.apply(void 0, Gs(t))];
                                                                 case 2:
                                                                     return [2, (r.value = d.apply(void 0, [h.sent()]), r)];
                                                                 case 3:
-                                                                    return f = h.sent(), c = f, eu.debug("error on " + e.name, f), (g = f) && g.nonRetryable ? (eu.debug(e.name + " non retryable error", f), [2, {
+                                                                    return f = h.sent(), c = f, nu.debug("error on " + e.name, f), (g = f) && g.nonRetryable ? (nu.debug(e.name + " non retryable error", f), [2, {
                                                                         value: a(f)
-                                                                    }]) : (p = n(o, t, f), eu.debug(e.name + " retrying in " + p + " ms"), !1 === p || s ? [2, {
+                                                                    }]) : (p = n(o, t, f), nu.debug(e.name + " retrying in " + p + " ms"), !1 === p || s ? [2, {
                                                                         value: a(f)
                                                                     }] : [3, 4]);
                                                                 case 4:
                                                                     return [4, new Promise((function(e) {
                                                                         l = e, u = setTimeout(l, p)
                                                                     }))];
                                                                 case 5:
@@ -60714,147 +60742,147 @@
                                             }
                                         }))
                                     }))
                                 }))]
                             }))
                         }))
                     }(e, t, function(e) {
-                        return void 0 === e && (e = nu),
+                        return void 0 === e && (e = ou),
                             function(t) {
                                 var n = 100 * Math.pow(2, t) + 100 * Math.random();
                                 return !(n > e) && n
                             }
                     }(n), r)
             },
-            ou = new Ws("CognitoCredentials"),
-            iu = new Promise((function(e, t) {
-                return $s().isBrowser ? (window.gapi && window.gapi.auth2 ? window.gapi.auth2 : null) ? (ou.debug("google api already loaded"), e()) : void setTimeout((function() {
+            au = new Zs("CognitoCredentials"),
+            su = new Promise((function(e, t) {
+                return tu().isBrowser ? (window.gapi && window.gapi.auth2 ? window.gapi.auth2 : null) ? (au.debug("google api already loaded"), e()) : void setTimeout((function() {
                     return e()
-                }), 2e3) : (ou.debug("not in the browser, directly resolved"), e())
+                }), 2e3) : (au.debug("not in the browser, directly resolved"), e())
             })),
-            au = function() {
+            uu = function() {
                 function e() {
                     this.initialized = !1, this.refreshGoogleToken = this.refreshGoogleToken.bind(this), this._refreshGoogleTokenImpl = this._refreshGoogleTokenImpl.bind(this)
                 }
                 return e.prototype.refreshGoogleToken = function() {
-                    return Ps(this, void 0, void 0, (function() {
-                        return Rs(this, (function(e) {
+                    return Bs(this, void 0, void 0, (function() {
+                        return Fs(this, (function(e) {
                             switch (e.label) {
                                 case 0:
-                                    return this.initialized ? [3, 2] : (ou.debug("need to wait for the Google SDK loaded"), [4, iu]);
+                                    return this.initialized ? [3, 2] : (au.debug("need to wait for the Google SDK loaded"), [4, su]);
                                 case 1:
-                                    e.sent(), this.initialized = !0, ou.debug("finish waiting"), e.label = 2;
+                                    e.sent(), this.initialized = !0, au.debug("finish waiting"), e.label = 2;
                                 case 2:
                                     return [2, this._refreshGoogleTokenImpl()]
                             }
                         }))
                     }))
                 }, e.prototype._refreshGoogleTokenImpl = function() {
                     var e = null;
-                    return $s().isBrowser && (e = window.gapi && window.gapi.auth2 ? window.gapi.auth2 : null), e ? new Promise((function(t, n) {
+                    return tu().isBrowser && (e = window.gapi && window.gapi.auth2 ? window.gapi.auth2 : null), e ? new Promise((function(t, n) {
                         e.getAuthInstance().then((function(e) {
-                            e || (ou.debug("google Auth undefined"), n(new tu("google Auth undefined")));
+                            e || (au.debug("google Auth undefined"), n(new ru("google Auth undefined")));
                             var r = e.currentUser.get();
-                            r.isSignedIn() ? (ou.debug("refreshing the google access token"), r.reloadAuthResponse().then((function(e) {
+                            r.isSignedIn() ? (au.debug("refreshing the google access token"), r.reloadAuthResponse().then((function(e) {
                                 var n = e.id_token,
                                     r = e.expires_at;
                                 t({
                                     token: n,
                                     expires_at: r
                                 })
                             })).catch((function(e) {
-                                e && "network_error" === e.error ? n("Network error reloading google auth response") : n(new tu("Failed to reload google auth response"))
-                            }))) : n(new tu("User is not signed in with Google"))
+                                e && "network_error" === e.error ? n("Network error reloading google auth response") : n(new ru("Failed to reload google auth response"))
+                            }))) : n(new ru("User is not signed in with Google"))
                         })).catch((function(e) {
-                            ou.debug("Failed to refresh google token", e), n(new tu("Failed to refresh google token"))
+                            au.debug("Failed to refresh google token", e), n(new ru("Failed to refresh google token"))
                         }))
-                    })) : (ou.debug("no gapi auth2 available"), Promise.reject("no gapi auth2 available"))
+                    })) : (au.debug("no gapi auth2 available"), Promise.reject("no gapi auth2 available"))
                 }, e
             }(),
-            su = new Ws("CognitoCredentials"),
-            uu = new Promise((function(e, t) {
-                return $s().isBrowser ? window.FB ? (su.debug("FB SDK already loaded"), e()) : void setTimeout((function() {
+            lu = new Zs("CognitoCredentials"),
+            cu = new Promise((function(e, t) {
+                return tu().isBrowser ? window.FB ? (lu.debug("FB SDK already loaded"), e()) : void setTimeout((function() {
                     return e()
-                }), 2e3) : (su.debug("not in the browser, directly resolved"), e())
+                }), 2e3) : (lu.debug("not in the browser, directly resolved"), e())
             })),
-            lu = function() {
+            du = function() {
                 function e() {
                     this.initialized = !1, this.refreshFacebookToken = this.refreshFacebookToken.bind(this), this._refreshFacebookTokenImpl = this._refreshFacebookTokenImpl.bind(this)
                 }
                 return e.prototype.refreshFacebookToken = function() {
-                    return Ps(this, void 0, void 0, (function() {
-                        return Rs(this, (function(e) {
+                    return Bs(this, void 0, void 0, (function() {
+                        return Fs(this, (function(e) {
                             switch (e.label) {
                                 case 0:
-                                    return this.initialized ? [3, 2] : (su.debug("need to wait for the Facebook SDK loaded"), [4, uu]);
+                                    return this.initialized ? [3, 2] : (lu.debug("need to wait for the Facebook SDK loaded"), [4, cu]);
                                 case 1:
-                                    e.sent(), this.initialized = !0, su.debug("finish waiting"), e.label = 2;
+                                    e.sent(), this.initialized = !0, lu.debug("finish waiting"), e.label = 2;
                                 case 2:
                                     return [2, this._refreshFacebookTokenImpl()]
                             }
                         }))
                     }))
                 }, e.prototype._refreshFacebookTokenImpl = function() {
                     var e = null;
-                    if ($s().isBrowser && (e = window.FB), !e) {
+                    if (tu().isBrowser && (e = window.FB), !e) {
                         var t = "no fb sdk available";
-                        return su.debug(t), Promise.reject(new tu(t))
+                        return lu.debug(t), Promise.reject(new ru(t))
                     }
                     return new Promise((function(t, n) {
                         e.getLoginStatus((function(e) {
                             if (e && e.authResponse) {
                                 var r = e.authResponse,
                                     o = r.accessToken,
                                     i = 1e3 * r.expiresIn + (new Date).getTime();
                                 if (!o) {
                                     a = "the jwtToken is undefined";
-                                    su.debug(a), n(new tu(a))
+                                    lu.debug(a), n(new ru(a))
                                 }
                                 t({
                                     token: o,
                                     expires_at: i
                                 })
                             } else {
                                 var a = "no response from facebook when refreshing the jwt token";
-                                su.debug(a), n(new tu(a))
+                                lu.debug(a), n(new ru(a))
                             }
                         }), {
                             scope: "public_profile,email"
                         })
                     }))
                 }, e
             }(),
-            cu = new au,
-            du = new lu,
-            fu = new Ws("Amplify"),
-            pu = new(function() {
+            fu = new uu,
+            pu = new du,
+            hu = new Zs("Amplify"),
+            gu = new(function() {
                 function e() {
-                    this._components = [], this._config = {}, this._modules = {}, this.Auth = null, this.Analytics = null, this.API = null, this.Credentials = null, this.Storage = null, this.I18n = null, this.Cache = null, this.PubSub = null, this.Interactions = null, this.Pushnotification = null, this.UI = null, this.XR = null, this.Predictions = null, this.DataStore = null, this.Geo = null, this.Notifications = null, this.Logger = Ws, this.ServiceWorker = null
+                    this._components = [], this._config = {}, this._modules = {}, this.Auth = null, this.Analytics = null, this.API = null, this.Credentials = null, this.Storage = null, this.I18n = null, this.Cache = null, this.PubSub = null, this.Interactions = null, this.Pushnotification = null, this.UI = null, this.XR = null, this.Predictions = null, this.DataStore = null, this.Geo = null, this.Notifications = null, this.Logger = Zs, this.ServiceWorker = null
                 }
                 return e.prototype.register = function(e) {
-                    fu.debug("component registered in amplify", e), this._components.push(e), "function" === typeof e.getModuleName ? (this._modules[e.getModuleName()] = e, this[e.getModuleName()] = e) : fu.debug("no getModuleName method for component", e), e.configure(this._config)
+                    hu.debug("component registered in amplify", e), this._components.push(e), "function" === typeof e.getModuleName ? (this._modules[e.getModuleName()] = e, this[e.getModuleName()] = e) : hu.debug("no getModuleName method for component", e), e.configure(this._config)
                 }, e.prototype.configure = function(e) {
                     var t = this;
-                    return e ? (this._config = Object.assign(this._config, e), fu.debug("amplify config", this._config), Object.entries(this._modules).forEach((function(e) {
-                        var n = Fs(e, 2),
+                    return e ? (this._config = Object.assign(this._config, e), hu.debug("amplify config", this._config), Object.entries(this._modules).forEach((function(e) {
+                        var n = Qs(e, 2),
                             r = (n[0], n[1]);
                         Object.keys(r).forEach((function(e) {
                             t._modules[e] && (r[e] = t._modules[e])
                         }))
                     })), this._components.map((function(e) {
                         e.configure(t._config)
                     })), this._config) : this._config
                 }, e.prototype.addPluggable = function(e) {
                     e && e.getCategory && "function" === typeof e.getCategory && this._components.map((function(t) {
                         t.addPluggable && "function" === typeof t.addPluggable && t.addPluggable(e)
                     }))
                 }, e
             }());
 
-        function hu(e, t, n, r) {
+        function yu(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -60874,15 +60902,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function gu(e, t) {
+        function mu(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -60950,15 +60978,15 @@
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
 
-        function yu(e, t) {
+        function vu(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -60971,42 +60999,42 @@
                     r && !r.done && (n = i.return) && n.call(i)
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
-        var mu = function(e, t) {
-            return mu = Object.setPrototypeOf || {
+        var Mu = function(e, t) {
+            return Mu = Object.setPrototypeOf || {
                 __proto__: []
             }
             instanceof Array && function(e, t) {
                 e.__proto__ = t
             } || function(e, t) {
                 for (var n in t) Object.prototype.hasOwnProperty.call(t, n) && (e[n] = t[n])
-            }, mu(e, t)
+            }, Mu(e, t)
         };
 
-        function vu(e, t) {
+        function bu(e, t) {
             if ("function" !== typeof t && null !== t) throw new TypeError("Class extends value " + String(t) + " is not a constructor or null");
 
             function n() {
                 this.constructor = e
             }
-            mu(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
+            Mu(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
         }
-        var Mu = function() {
-            return Mu = Object.assign || function(e) {
+        var ju = function() {
+            return ju = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, Mu.apply(this, arguments)
+            }, ju.apply(this, arguments)
         };
 
-        function bu(e, t, n, r) {
+        function wu(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -61026,15 +61054,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function ju(e, t) {
+        function xu(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -61103,15 +61131,15 @@
                         }
                     }([i, s])
                 }
             }
         }
         Object.create;
 
-        function wu(e, t) {
+        function Nu(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -61124,312 +61152,312 @@
                     r && !r.done && (n = i.return) && n.call(i)
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
-        var xu, Nu, Iu, Du, Su, Lu, ku, Cu, Eu, _u, Tu, Au, Ou, zu, Uu, Pu, Ru, Bu, Fu, Yu, Qu, Gu, Wu, Hu, Zu, Vu, qu, Ju, Ku, Xu, $u, el, tl, nl, rl, ol, il, al, sl, ul, ll, cl, dl, fl, pl, hl, gl, yl, ml, vl, Ml, bl, jl, wl, xl, Nl, Il;
+        var Iu, Du, Su, Lu, ku, Cu, Eu, _u, Tu, Au, Ou, zu, Uu, Pu, Ru, Bu, Fu, Yu, Qu, Gu, Wu, Hu, Zu, Vu, qu, Ju, Ku, Xu, $u, el, tl, nl, rl, ol, il, al, sl, ul, ll, cl, dl, fl, pl, hl, gl, yl, ml, vl, Ml, bl, jl, wl, xl, Nl, Il, Dl, Sl;
         Object.create;
         ! function(e) {
             e.AUTHENTICATED_ROLE = "AuthenticatedRole", e.DENY = "Deny"
-        }(xu || (xu = {})),
-        function(e) {
-            e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
-            }
-        }(Nu || (Nu = {})),
-        function(e) {
-            e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
-            }
         }(Iu || (Iu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(Du || (Du = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(Su || (Su = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(Lu || (Lu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(ku || (ku = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(Cu || (Cu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(Eu || (Eu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(_u || (_u = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(Tu || (Tu = {})),
         function(e) {
-            e.ACCESS_DENIED = "AccessDenied", e.INTERNAL_SERVER_ERROR = "InternalServerError"
+            e.filterSensitiveLog = function(e) {
+                return ju({}, e)
+            }
         }(Au || (Au = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(Ou || (Ou = {})),
         function(e) {
-            e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
-            }
+            e.ACCESS_DENIED = "AccessDenied", e.INTERNAL_SERVER_ERROR = "InternalServerError"
         }(zu || (zu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(Uu || (Uu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(Pu || (Pu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(Ru || (Ru = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(Bu || (Bu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(Fu || (Fu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(Yu || (Yu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(Qu || (Qu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(Gu || (Gu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(Wu || (Wu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(Hu || (Hu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(Zu || (Zu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(Vu || (Vu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(qu || (qu = {})),
         function(e) {
-            e.CONTAINS = "Contains", e.EQUALS = "Equals", e.NOT_EQUAL = "NotEqual", e.STARTS_WITH = "StartsWith"
+            e.filterSensitiveLog = function(e) {
+                return ju({}, e)
+            }
         }(Ju || (Ju = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(Ku || (Ku = {})),
         function(e) {
-            e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
-            }
+            e.CONTAINS = "Contains", e.EQUALS = "Equals", e.NOT_EQUAL = "NotEqual", e.STARTS_WITH = "StartsWith"
         }(Xu || (Xu = {})),
         function(e) {
-            e.RULES = "Rules", e.TOKEN = "Token"
+            e.filterSensitiveLog = function(e) {
+                return ju({}, e)
+            }
         }($u || ($u = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(el || (el = {})),
         function(e) {
-            e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
-            }
+            e.RULES = "Rules", e.TOKEN = "Token"
         }(tl || (tl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(nl || (nl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(rl || (rl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(ol || (ol = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(il || (il = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(al || (al = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(sl || (sl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(ul || (ul = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(ll || (ll = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(cl || (cl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(dl || (dl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(fl || (fl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(pl || (pl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(hl || (hl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(gl || (gl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(yl || (yl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(ml || (ml = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(vl || (vl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(Ml || (Ml = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(bl || (bl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(jl || (jl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(wl || (wl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(xl || (xl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
         }(Nl || (Nl = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return Mu({}, e)
+                return ju({}, e)
             }
-        }(Il || (Il = {}));
-        var Dl = function() {
+        }(Il || (Il = {})),
+        function(e) {
+            e.filterSensitiveLog = function(e) {
+                return ju({}, e)
+            }
+        }(Dl || (Dl = {})),
+        function(e) {
+            e.filterSensitiveLog = function(e) {
+                return ju({}, e)
+            }
+        }(Sl || (Sl = {}));
+        var Ll = function() {
             function e(e) {
                 this.statusCode = e.statusCode, this.headers = e.headers || {}, this.body = e.body
             }
             return e.isInstance = function(e) {
                 if (!e) return !1;
                 var t = e;
                 return "number" === typeof t.statusCode && "object" === typeof t.headers
             }, e
         }();
-        var Sl = function() {
-            return Sl = Object.assign || function(e) {
+        var kl = function() {
+            return kl = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, Sl.apply(this, arguments)
+            }, kl.apply(this, arguments)
         };
 
-        function Ll(e, t) {
+        function Cl(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -61442,44 +61470,44 @@
                     r && !r.done && (n = i.return) && n.call(i)
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
-        var kl = function() {
+        var El = function() {
             function e(e) {
                 this.method = e.method || "GET", this.hostname = e.hostname || "localhost", this.port = e.port, this.query = e.query || {}, this.headers = e.headers || {}, this.body = e.body, this.protocol = e.protocol ? ":" !== e.protocol.substr(-1) ? e.protocol + ":" : e.protocol : "https:", this.path = e.path ? "/" !== e.path.charAt(0) ? "/" + e.path : e.path : "/"
             }
             return e.isInstance = function(e) {
                 if (!e) return !1;
                 var t = e;
                 return "method" in t && "protocol" in t && "hostname" in t && "path" in t && "object" === typeof t.query && "object" === typeof t.headers
             }, e.prototype.clone = function() {
-                var t, n = new e(Sl(Sl({}, this), {
-                    headers: Sl({}, this.headers)
+                var t, n = new e(kl(kl({}, this), {
+                    headers: kl({}, this.headers)
                 }));
                 return n.query && (n.query = (t = n.query, Object.keys(t).reduce((function(e, n) {
                     var r, o = t[n];
-                    return Sl(Sl({}, e), ((r = {})[n] = Array.isArray(o) ? function() {
-                        for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(Ll(arguments[t]));
+                    return kl(kl({}, e), ((r = {})[n] = Array.isArray(o) ? function() {
+                        for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(Cl(arguments[t]));
                         return e
                     }(o) : o, r))
                 }), {}))), n
             }, e
         }();
-        var Cl = function(e, t) {
-                return bu(void 0, void 0, void 0, (function() {
+        var _l = function(e, t) {
+                return wu(void 0, void 0, void 0, (function() {
                     var n, r, o, i, a, s, u, l, c, d, f, p, h, g, y;
-                    return ju(this, (function(m) {
+                    return xu(this, (function(m) {
                         switch (m.label) {
                             case 0:
-                                return r = [Mu({}, e)], y = {}, [4, ic(e.body, t)];
+                                return r = [ju({}, e)], y = {}, [4, sc(e.body, t)];
                             case 1:
-                                switch (n = Mu.apply(void 0, r.concat([(y.body = m.sent(), y)])), i = "UnknownError", i = ac(e, n.body), i) {
+                                switch (n = ju.apply(void 0, r.concat([(y.body = m.sent(), y)])), i = "UnknownError", i = uc(e, n.body), i) {
                                     case "ExternalServiceException":
                                     case "com.amazonaws.cognitoidentity#ExternalServiceException":
                                         return [3, 2];
                                     case "InternalErrorException":
                                     case "com.amazonaws.cognitoidentity#InternalErrorException":
                                         return [3, 4];
                                     case "InvalidIdentityPoolConfigurationException":
@@ -61499,91 +61527,91 @@
                                         return [3, 14];
                                     case "TooManyRequestsException":
                                     case "com.amazonaws.cognitoidentity#TooManyRequestsException":
                                         return [3, 16]
                                 }
                                 return [3, 18];
                             case 2:
-                                return a = [{}], [4, _l(n, t)];
+                                return a = [{}], [4, Al(n, t)];
                             case 3:
-                                return o = Mu.apply(void 0, [Mu.apply(void 0, a.concat([m.sent()])), {
+                                return o = ju.apply(void 0, [ju.apply(void 0, a.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: nc(e)
+                                    $metadata: oc(e)
                                 }]), [3, 19];
                             case 4:
-                                return s = [{}], [4, Tl(n, t)];
+                                return s = [{}], [4, Ol(n, t)];
                             case 5:
-                                return o = Mu.apply(void 0, [Mu.apply(void 0, s.concat([m.sent()])), {
+                                return o = ju.apply(void 0, [ju.apply(void 0, s.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: nc(e)
+                                    $metadata: oc(e)
                                 }]), [3, 19];
                             case 6:
-                                return u = [{}], [4, Al(n, t)];
+                                return u = [{}], [4, zl(n, t)];
                             case 7:
-                                return o = Mu.apply(void 0, [Mu.apply(void 0, u.concat([m.sent()])), {
+                                return o = ju.apply(void 0, [ju.apply(void 0, u.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: nc(e)
+                                    $metadata: oc(e)
                                 }]), [3, 19];
                             case 8:
-                                return l = [{}], [4, Ol(n, t)];
+                                return l = [{}], [4, Ul(n, t)];
                             case 9:
-                                return o = Mu.apply(void 0, [Mu.apply(void 0, l.concat([m.sent()])), {
+                                return o = ju.apply(void 0, [ju.apply(void 0, l.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: nc(e)
+                                    $metadata: oc(e)
                                 }]), [3, 19];
                             case 10:
-                                return c = [{}], [4, Ul(n, t)];
+                                return c = [{}], [4, Rl(n, t)];
                             case 11:
-                                return o = Mu.apply(void 0, [Mu.apply(void 0, c.concat([m.sent()])), {
+                                return o = ju.apply(void 0, [ju.apply(void 0, c.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: nc(e)
+                                    $metadata: oc(e)
                                 }]), [3, 19];
                             case 12:
-                                return d = [{}], [4, Pl(n, t)];
+                                return d = [{}], [4, Bl(n, t)];
                             case 13:
-                                return o = Mu.apply(void 0, [Mu.apply(void 0, d.concat([m.sent()])), {
+                                return o = ju.apply(void 0, [ju.apply(void 0, d.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: nc(e)
+                                    $metadata: oc(e)
                                 }]), [3, 19];
                             case 14:
-                                return f = [{}], [4, Rl(n, t)];
+                                return f = [{}], [4, Fl(n, t)];
                             case 15:
-                                return o = Mu.apply(void 0, [Mu.apply(void 0, f.concat([m.sent()])), {
+                                return o = ju.apply(void 0, [ju.apply(void 0, f.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: nc(e)
+                                    $metadata: oc(e)
                                 }]), [3, 19];
                             case 16:
-                                return p = [{}], [4, Bl(n, t)];
+                                return p = [{}], [4, Yl(n, t)];
                             case 17:
-                                return o = Mu.apply(void 0, [Mu.apply(void 0, p.concat([m.sent()])), {
+                                return o = ju.apply(void 0, [ju.apply(void 0, p.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: nc(e)
+                                    $metadata: oc(e)
                                 }]), [3, 19];
                             case 18:
-                                h = n.body, i = h.code || h.Code || i, o = Mu(Mu({}, h), {
+                                h = n.body, i = h.code || h.Code || i, o = ju(ju({}, h), {
                                     name: "" + i,
                                     message: h.message || h.Message || i,
                                     $fault: "client",
-                                    $metadata: nc(e)
+                                    $metadata: oc(e)
                                 }), m.label = 19;
                             case 19:
                                 return g = o.message || o.Message || i, o.message = g, delete o.Message, [2, Promise.reject(Object.assign(new Error(g), o))]
                         }
                     }))
                 }))
             },
-            El = function(e, t) {
-                return bu(void 0, void 0, void 0, (function() {
+            Tl = function(e, t) {
+                return wu(void 0, void 0, void 0, (function() {
                     var n, r, o, i, a, s, u, l, c, d, f, p, h, g, y;
-                    return ju(this, (function(m) {
+                    return xu(this, (function(m) {
                         switch (m.label) {
                             case 0:
-                                return r = [Mu({}, e)], y = {}, [4, ic(e.body, t)];
+                                return r = [ju({}, e)], y = {}, [4, sc(e.body, t)];
                             case 1:
-                                switch (n = Mu.apply(void 0, r.concat([(y.body = m.sent(), y)])), i = "UnknownError", i = ac(e, n.body), i) {
+                                switch (n = ju.apply(void 0, r.concat([(y.body = m.sent(), y)])), i = "UnknownError", i = uc(e, n.body), i) {
                                     case "ExternalServiceException":
                                     case "com.amazonaws.cognitoidentity#ExternalServiceException":
                                         return [3, 2];
                                     case "InternalErrorException":
                                     case "com.amazonaws.cognitoidentity#InternalErrorException":
                                         return [3, 4];
                                     case "InvalidParameterException":
@@ -61603,340 +61631,340 @@
                                         return [3, 14];
                                     case "TooManyRequestsException":
                                     case "com.amazonaws.cognitoidentity#TooManyRequestsException":
                                         return [3, 16]
                                 }
                                 return [3, 18];
                             case 2:
-                                return a = [{}], [4, _l(n, t)];
+                                return a = [{}], [4, Al(n, t)];
                             case 3:
-                                return o = Mu.apply(void 0, [Mu.apply(void 0, a.concat([m.sent()])), {
+                                return o = ju.apply(void 0, [ju.apply(void 0, a.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: nc(e)
+                                    $metadata: oc(e)
                                 }]), [3, 19];
                             case 4:
-                                return s = [{}], [4, Tl(n, t)];
+                                return s = [{}], [4, Ol(n, t)];
                             case 5:
-                                return o = Mu.apply(void 0, [Mu.apply(void 0, s.concat([m.sent()])), {
+                                return o = ju.apply(void 0, [ju.apply(void 0, s.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: nc(e)
+                                    $metadata: oc(e)
                                 }]), [3, 19];
                             case 6:
-                                return u = [{}], [4, Ol(n, t)];
+                                return u = [{}], [4, Ul(n, t)];
                             case 7:
-                                return o = Mu.apply(void 0, [Mu.apply(void 0, u.concat([m.sent()])), {
+                                return o = ju.apply(void 0, [ju.apply(void 0, u.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: nc(e)
+                                    $metadata: oc(e)
                                 }]), [3, 19];
                             case 8:
-                                return l = [{}], [4, zl(n, t)];
+                                return l = [{}], [4, Pl(n, t)];
                             case 9:
-                                return o = Mu.apply(void 0, [Mu.apply(void 0, l.concat([m.sent()])), {
+                                return o = ju.apply(void 0, [ju.apply(void 0, l.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: nc(e)
+                                    $metadata: oc(e)
                                 }]), [3, 19];
                             case 10:
-                                return c = [{}], [4, Ul(n, t)];
+                                return c = [{}], [4, Rl(n, t)];
                             case 11:
-                                return o = Mu.apply(void 0, [Mu.apply(void 0, c.concat([m.sent()])), {
+                                return o = ju.apply(void 0, [ju.apply(void 0, c.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: nc(e)
+                                    $metadata: oc(e)
                                 }]), [3, 19];
                             case 12:
-                                return d = [{}], [4, Pl(n, t)];
+                                return d = [{}], [4, Bl(n, t)];
                             case 13:
-                                return o = Mu.apply(void 0, [Mu.apply(void 0, d.concat([m.sent()])), {
+                                return o = ju.apply(void 0, [ju.apply(void 0, d.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: nc(e)
+                                    $metadata: oc(e)
                                 }]), [3, 19];
                             case 14:
-                                return f = [{}], [4, Rl(n, t)];
+                                return f = [{}], [4, Fl(n, t)];
                             case 15:
-                                return o = Mu.apply(void 0, [Mu.apply(void 0, f.concat([m.sent()])), {
+                                return o = ju.apply(void 0, [ju.apply(void 0, f.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: nc(e)
+                                    $metadata: oc(e)
                                 }]), [3, 19];
                             case 16:
-                                return p = [{}], [4, Bl(n, t)];
+                                return p = [{}], [4, Yl(n, t)];
                             case 17:
-                                return o = Mu.apply(void 0, [Mu.apply(void 0, p.concat([m.sent()])), {
+                                return o = ju.apply(void 0, [ju.apply(void 0, p.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: nc(e)
+                                    $metadata: oc(e)
                                 }]), [3, 19];
                             case 18:
-                                h = n.body, i = h.code || h.Code || i, o = Mu(Mu({}, h), {
+                                h = n.body, i = h.code || h.Code || i, o = ju(ju({}, h), {
                                     name: "" + i,
                                     message: h.message || h.Message || i,
                                     $fault: "client",
-                                    $metadata: nc(e)
+                                    $metadata: oc(e)
                                 }), m.label = 19;
                             case 19:
                                 return g = o.message || o.Message || i, o.message = g, delete o.Message, [2, Promise.reject(Object.assign(new Error(g), o))]
                         }
                     }))
                 }))
             },
-            _l = function(e, t) {
-                return bu(void 0, void 0, void 0, (function() {
+            Al = function(e, t) {
+                return wu(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return ju(this, (function(o) {
-                        return n = e.body, r = Wl(n, t), [2, Mu({
+                    return xu(this, (function(o) {
+                        return n = e.body, r = Zl(n, t), [2, ju({
                             name: "ExternalServiceException",
                             $fault: "client",
-                            $metadata: nc(e)
+                            $metadata: oc(e)
                         }, r)]
                     }))
                 }))
             },
-            Tl = function(e, t) {
-                return bu(void 0, void 0, void 0, (function() {
+            Ol = function(e, t) {
+                return wu(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return ju(this, (function(o) {
-                        return n = e.body, r = Vl(n, t), [2, Mu({
+                    return xu(this, (function(o) {
+                        return n = e.body, r = Jl(n, t), [2, ju({
                             name: "InternalErrorException",
                             $fault: "server",
-                            $metadata: nc(e)
+                            $metadata: oc(e)
                         }, r)]
                     }))
                 }))
             },
-            Al = function(e, t) {
-                return bu(void 0, void 0, void 0, (function() {
+            zl = function(e, t) {
+                return wu(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return ju(this, (function(o) {
-                        return n = e.body, r = ql(n, t), [2, Mu({
+                    return xu(this, (function(o) {
+                        return n = e.body, r = Kl(n, t), [2, ju({
                             name: "InvalidIdentityPoolConfigurationException",
                             $fault: "client",
-                            $metadata: nc(e)
+                            $metadata: oc(e)
                         }, r)]
                     }))
                 }))
             },
-            Ol = function(e, t) {
-                return bu(void 0, void 0, void 0, (function() {
+            Ul = function(e, t) {
+                return wu(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return ju(this, (function(o) {
-                        return n = e.body, r = Jl(n, t), [2, Mu({
+                    return xu(this, (function(o) {
+                        return n = e.body, r = Xl(n, t), [2, ju({
                             name: "InvalidParameterException",
                             $fault: "client",
-                            $metadata: nc(e)
+                            $metadata: oc(e)
                         }, r)]
                     }))
                 }))
             },
-            zl = function(e, t) {
-                return bu(void 0, void 0, void 0, (function() {
+            Pl = function(e, t) {
+                return wu(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return ju(this, (function(o) {
-                        return n = e.body, r = Kl(n, t), [2, Mu({
+                    return xu(this, (function(o) {
+                        return n = e.body, r = $l(n, t), [2, ju({
                             name: "LimitExceededException",
                             $fault: "client",
-                            $metadata: nc(e)
+                            $metadata: oc(e)
                         }, r)]
                     }))
                 }))
             },
-            Ul = function(e, t) {
-                return bu(void 0, void 0, void 0, (function() {
+            Rl = function(e, t) {
+                return wu(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return ju(this, (function(o) {
-                        return n = e.body, r = Xl(n, t), [2, Mu({
+                    return xu(this, (function(o) {
+                        return n = e.body, r = ec(n, t), [2, ju({
                             name: "NotAuthorizedException",
                             $fault: "client",
-                            $metadata: nc(e)
+                            $metadata: oc(e)
                         }, r)]
                     }))
                 }))
             },
-            Pl = function(e, t) {
-                return bu(void 0, void 0, void 0, (function() {
+            Bl = function(e, t) {
+                return wu(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return ju(this, (function(o) {
-                        return n = e.body, r = $l(n, t), [2, Mu({
+                    return xu(this, (function(o) {
+                        return n = e.body, r = tc(n, t), [2, ju({
                             name: "ResourceConflictException",
                             $fault: "client",
-                            $metadata: nc(e)
+                            $metadata: oc(e)
                         }, r)]
                     }))
                 }))
             },
-            Rl = function(e, t) {
-                return bu(void 0, void 0, void 0, (function() {
+            Fl = function(e, t) {
+                return wu(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return ju(this, (function(o) {
-                        return n = e.body, r = ec(n, t), [2, Mu({
+                    return xu(this, (function(o) {
+                        return n = e.body, r = nc(n, t), [2, ju({
                             name: "ResourceNotFoundException",
                             $fault: "client",
-                            $metadata: nc(e)
+                            $metadata: oc(e)
                         }, r)]
                     }))
                 }))
             },
-            Bl = function(e, t) {
-                return bu(void 0, void 0, void 0, (function() {
+            Yl = function(e, t) {
+                return wu(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return ju(this, (function(o) {
-                        return n = e.body, r = tc(n, t), [2, Mu({
+                    return xu(this, (function(o) {
+                        return n = e.body, r = rc(n, t), [2, ju({
                             name: "TooManyRequestsException",
                             $fault: "client",
-                            $metadata: nc(e)
+                            $metadata: oc(e)
                         }, r)]
                     }))
                 }))
             },
-            Fl = function(e, t) {
-                return Mu(Mu(Mu({}, void 0 !== e.CustomRoleArn && null !== e.CustomRoleArn && {
+            Ql = function(e, t) {
+                return ju(ju(ju({}, void 0 !== e.CustomRoleArn && null !== e.CustomRoleArn && {
                     CustomRoleArn: e.CustomRoleArn
                 }), void 0 !== e.IdentityId && null !== e.IdentityId && {
                     IdentityId: e.IdentityId
                 }), void 0 !== e.Logins && null !== e.Logins && {
-                    Logins: Ql(e.Logins, t)
+                    Logins: Wl(e.Logins, t)
                 })
             },
-            Yl = function(e, t) {
-                return Mu(Mu(Mu({}, void 0 !== e.AccountId && null !== e.AccountId && {
+            Gl = function(e, t) {
+                return ju(ju(ju({}, void 0 !== e.AccountId && null !== e.AccountId && {
                     AccountId: e.AccountId
                 }), void 0 !== e.IdentityPoolId && null !== e.IdentityPoolId && {
                     IdentityPoolId: e.IdentityPoolId
                 }), void 0 !== e.Logins && null !== e.Logins && {
-                    Logins: Ql(e.Logins, t)
+                    Logins: Wl(e.Logins, t)
                 })
             },
-            Ql = function(e, t) {
+            Wl = function(e, t) {
                 return Object.entries(e).reduce((function(e, t) {
-                    var n, r = wu(t, 2),
+                    var n, r = Nu(t, 2),
                         o = r[0],
                         i = r[1];
-                    return null === i ? e : Mu(Mu({}, e), ((n = {})[o] = i, n))
+                    return null === i ? e : ju(ju({}, e), ((n = {})[o] = i, n))
                 }), {})
             },
-            Gl = function(e, t) {
+            Hl = function(e, t) {
                 return {
                     AccessKeyId: void 0 !== e.AccessKeyId && null !== e.AccessKeyId ? e.AccessKeyId : void 0,
                     Expiration: void 0 !== e.Expiration && null !== e.Expiration ? new Date(Math.round(1e3 * e.Expiration)) : void 0,
                     SecretKey: void 0 !== e.SecretKey && null !== e.SecretKey ? e.SecretKey : void 0,
                     SessionToken: void 0 !== e.SessionToken && null !== e.SessionToken ? e.SessionToken : void 0
                 }
             },
-            Wl = function(e, t) {
+            Zl = function(e, t) {
                 return {
                     message: void 0 !== e.message && null !== e.message ? e.message : void 0
                 }
             },
-            Hl = function(e, t) {
+            Vl = function(e, t) {
                 return {
-                    Credentials: void 0 !== e.Credentials && null !== e.Credentials ? Gl(e.Credentials) : void 0,
+                    Credentials: void 0 !== e.Credentials && null !== e.Credentials ? Hl(e.Credentials) : void 0,
                     IdentityId: void 0 !== e.IdentityId && null !== e.IdentityId ? e.IdentityId : void 0
                 }
             },
-            Zl = function(e, t) {
+            ql = function(e, t) {
                 return {
                     IdentityId: void 0 !== e.IdentityId && null !== e.IdentityId ? e.IdentityId : void 0
                 }
             },
-            Vl = function(e, t) {
+            Jl = function(e, t) {
                 return {
                     message: void 0 !== e.message && null !== e.message ? e.message : void 0
                 }
             },
-            ql = function(e, t) {
+            Kl = function(e, t) {
                 return {
                     message: void 0 !== e.message && null !== e.message ? e.message : void 0
                 }
             },
-            Jl = function(e, t) {
+            Xl = function(e, t) {
                 return {
                     message: void 0 !== e.message && null !== e.message ? e.message : void 0
                 }
             },
-            Kl = function(e, t) {
+            $l = function(e, t) {
                 return {
                     message: void 0 !== e.message && null !== e.message ? e.message : void 0
                 }
             },
-            Xl = function(e, t) {
+            ec = function(e, t) {
                 return {
                     message: void 0 !== e.message && null !== e.message ? e.message : void 0
                 }
             },
-            $l = function(e, t) {
+            tc = function(e, t) {
                 return {
                     message: void 0 !== e.message && null !== e.message ? e.message : void 0
                 }
             },
-            ec = function(e, t) {
+            nc = function(e, t) {
                 return {
                     message: void 0 !== e.message && null !== e.message ? e.message : void 0
                 }
             },
-            tc = function(e, t) {
+            rc = function(e, t) {
                 return {
                     message: void 0 !== e.message && null !== e.message ? e.message : void 0
                 }
             },
-            nc = function(e) {
+            oc = function(e) {
                 var t;
                 return {
                     httpStatusCode: e.statusCode,
                     requestId: null !== (t = e.headers["x-amzn-requestid"]) && void 0 !== t ? t : e.headers["x-amzn-request-id"],
                     extendedRequestId: e.headers["x-amz-id-2"],
                     cfId: e.headers["x-amz-cf-id"]
                 }
             },
-            rc = function(e, t) {
+            ic = function(e, t) {
                 return void 0 === e && (e = new Uint8Array), e instanceof Uint8Array ? Promise.resolve(e) : t.streamCollector(e) || Promise.resolve(new Uint8Array)
             },
-            oc = function(e, t, n, r, o) {
-                return bu(void 0, void 0, void 0, (function() {
+            ac = function(e, t, n, r, o) {
+                return wu(void 0, void 0, void 0, (function() {
                     var i, a, s, u, l, c;
-                    return ju(this, (function(d) {
+                    return xu(this, (function(d) {
                         switch (d.label) {
                             case 0:
                                 return [4, e.endpoint()];
                             case 1:
                                 return i = d.sent(), a = i.hostname, s = i.protocol, u = void 0 === s ? "https" : s, l = i.port, c = {
                                     protocol: u,
                                     hostname: a,
                                     port: l,
                                     method: "POST",
                                     path: n,
                                     headers: t
-                                }, void 0 !== r && (c.hostname = r), void 0 !== o && (c.body = o), [2, new kl(c)]
+                                }, void 0 !== r && (c.hostname = r), void 0 !== o && (c.body = o), [2, new El(c)]
                         }
                     }))
                 }))
             },
-            ic = function(e, t) {
+            sc = function(e, t) {
                 return function(e, t) {
-                    return rc(e, t).then((function(e) {
+                    return ic(e, t).then((function(e) {
                         return t.utf8Encoder(e)
                     }))
                 }(e, t).then((function(e) {
                     return e.length ? JSON.parse(e) : {}
                 }))
             },
-            ac = function(e, t) {
+            uc = function(e, t) {
                 var n, r, o = function(e) {
                         var t = e;
                         return t.indexOf(":") >= 0 && (t = t.split(":")[0]), t.indexOf("#") >= 0 && (t = t.split("#")[1]), t
                     },
                     i = (n = e.headers, r = "x-amzn-errortype", Object.keys(n).find((function(e) {
                         return e.toLowerCase() === r.toLowerCase()
                     })));
                 return void 0 !== i ? o(e.headers[i]) : void 0 !== t.code ? o(t.code) : void 0 !== t.__type ? o(t.__type) : ""
             };
-        var sc = function() {
-            return sc = Object.assign || function(e) {
+        var lc = function() {
+            return lc = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, sc.apply(this, arguments)
+            }, lc.apply(this, arguments)
         };
 
-        function uc(e, t, n, r) {
+        function cc(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -61956,15 +61984,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function lc(e, t) {
+        function dc(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -62031,36 +62059,36 @@
                             value: i[0] ? i[1] : void 0,
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
-        var cc = {
+        var fc = {
                 name: "deserializerMiddleware",
                 step: "deserialize",
                 tags: ["DESERIALIZER"],
                 override: !0
             },
-            dc = {
+            pc = {
                 name: "serializerMiddleware",
                 step: "serialize",
                 tags: ["SERIALIZER"],
                 override: !0
             };
 
-        function fc(e, t, n) {
+        function hc(e, t, n) {
             return {
                 applyToStack: function(r) {
                     r.add(function(e, t) {
                         return function(n, r) {
                             return function(r) {
-                                return uc(void 0, void 0, void 0, (function() {
+                                return cc(void 0, void 0, void 0, (function() {
                                     var o, i;
-                                    return lc(this, (function(a) {
+                                    return dc(this, (function(a) {
                                         switch (a.label) {
                                             case 0:
                                                 return [4, n(r)];
                                             case 1:
                                                 return o = a.sent().response, [4, t(o, e)];
                                             case 2:
                                                 return i = a.sent(), [2, {
@@ -62068,45 +62096,45 @@
                                                     output: i
                                                 }]
                                         }
                                     }))
                                 }))
                             }
                         }
-                    }(e, n), cc), r.add(function(e, t) {
+                    }(e, n), fc), r.add(function(e, t) {
                         return function(n, r) {
                             return function(r) {
-                                return uc(void 0, void 0, void 0, (function() {
+                                return cc(void 0, void 0, void 0, (function() {
                                     var o;
-                                    return lc(this, (function(i) {
+                                    return dc(this, (function(i) {
                                         switch (i.label) {
                                             case 0:
                                                 return [4, t(r.input, e)];
                                             case 1:
-                                                return o = i.sent(), [2, n(sc(sc({}, r), {
+                                                return o = i.sent(), [2, n(lc(lc({}, r), {
                                                     request: o
                                                 }))]
                                         }
                                     }))
                                 }))
                             }
                         }
-                    }(e, t), dc)
+                    }(e, t), pc)
                 }
             }
         }
-        var pc = function() {
-            return pc = Object.assign || function(e) {
+        var gc = function() {
+            return gc = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, pc.apply(this, arguments)
+            }, gc.apply(this, arguments)
         };
 
-        function hc(e) {
+        function yc(e) {
             var t = "function" === typeof Symbol && Symbol.iterator,
                 n = t && e[t],
                 r = 0;
             if (n) return n.call(e);
             if (e && "number" === typeof e.length) return {
                 next: function() {
                     return e && r >= e.length && (e = void 0), {
@@ -62114,15 +62142,15 @@
                         done: !e
                     }
                 }
             };
             throw new TypeError(t ? "Object is not iterable." : "Symbol.iterator is not defined.")
         }
 
-        function gc(e, t) {
+        function mc(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -62136,75 +62164,75 @@
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
 
-        function yc() {
-            for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(gc(arguments[t]));
+        function vc() {
+            for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(mc(arguments[t]));
             return e
         }
-        var mc = function e() {
+        var Mc = function e() {
                 var t = [],
                     n = [],
                     r = new Set,
                     o = function(e) {
                         return t.forEach((function(t) {
-                            e.add(t.middleware, pc({}, t))
+                            e.add(t.middleware, gc({}, t))
                         })), n.forEach((function(t) {
-                            e.addRelativeTo(t.middleware, pc({}, t))
+                            e.addRelativeTo(t.middleware, gc({}, t))
                         })), e
                     },
                     i = function e(t) {
                         var n = [];
                         return t.before.forEach((function(t) {
-                            0 === t.before.length && 0 === t.after.length ? n.push(t) : n.push.apply(n, yc(e(t)))
+                            0 === t.before.length && 0 === t.after.length ? n.push(t) : n.push.apply(n, vc(e(t)))
                         })), n.push(t), t.after.reverse().forEach((function(t) {
-                            0 === t.before.length && 0 === t.after.length ? n.push(t) : n.push.apply(n, yc(e(t)))
+                            0 === t.before.length && 0 === t.after.length ? n.push(t) : n.push.apply(n, vc(e(t)))
                         })), n
                     },
                     a = function() {
                         var e = [],
                             r = [],
                             o = {};
                         t.forEach((function(t) {
-                            var n = pc(pc({}, t), {
+                            var n = gc(gc({}, t), {
                                 before: [],
                                 after: []
                             });
                             n.name && (o[n.name] = n), e.push(n)
                         })), n.forEach((function(e) {
-                            var t = pc(pc({}, e), {
+                            var t = gc(gc({}, e), {
                                 before: [],
                                 after: []
                             });
                             t.name && (o[t.name] = t), r.push(t)
                         })), r.forEach((function(e) {
                             if (e.toMiddleware) {
                                 var t = o[e.toMiddleware];
                                 if (void 0 === t) throw new Error(e.toMiddleware + " is not found when adding " + (e.name || "anonymous") + " middleware " + e.relation + " " + e.toMiddleware);
                                 "after" === e.relation && t.after.push(e), "before" === e.relation && t.before.push(e)
                             }
                         }));
                         var a, s = (a = e, a.sort((function(e, t) {
-                            return vc[t.step] - vc[e.step] || Mc[t.priority || "normal"] - Mc[e.priority || "normal"]
+                            return bc[t.step] - bc[e.step] || jc[t.priority || "normal"] - jc[e.priority || "normal"]
                         }))).map(i).reduce((function(e, t) {
-                            return e.push.apply(e, yc(t)), e
+                            return e.push.apply(e, vc(t)), e
                         }), []);
                         return s.map((function(e) {
                             return e.middleware
                         }))
                     },
                     s = {
                         add: function(e, n) {
                             void 0 === n && (n = {});
                             var o = n.name,
                                 i = n.override,
-                                a = pc({
+                                a = gc({
                                     step: "initialize",
                                     priority: "normal",
                                     middleware: e
                                 }, n);
                             if (o) {
                                 if (r.has(o)) {
                                     if (!i) throw new Error("Duplicate middleware name '" + o + "'");
@@ -62218,15 +62246,15 @@
                                 r.add(o)
                             }
                             t.push(a)
                         },
                         addRelativeTo: function(e, t) {
                             var o = t.name,
                                 i = t.override,
-                                a = pc({
+                                a = gc({
                                     middleware: e
                                 }, t);
                             if (o) {
                                 if (r.has(o)) {
                                     if (!i) throw new Error("Duplicate middleware name '" + o + "'");
                                     var s = n.findIndex((function(e) {
                                             return e.name === o
@@ -62273,15 +62301,15 @@
                             var n = o(e());
                             return n.use(t), n
                         },
                         applyToStack: o,
                         resolve: function(e, t) {
                             var n, r;
                             try {
-                                for (var o = hc(a().reverse()), i = o.next(); !i.done; i = o.next()) {
+                                for (var o = yc(a().reverse()), i = o.next(); !i.done; i = o.next()) {
                                     e = (0, i.value)(e, t)
                                 }
                             } catch (s) {
                                 n = {
                                     error: s
                                 }
                             } finally {
@@ -62292,29 +62320,29 @@
                                 }
                             }
                             return e
                         }
                     };
                 return s
             },
-            vc = {
+            bc = {
                 initialize: 5,
                 serialize: 4,
                 build: 3,
                 finalizeRequest: 2,
                 deserialize: 1
             },
-            Mc = {
+            jc = {
                 high: 3,
                 normal: 2,
                 low: 1
             },
-            bc = function() {
+            wc = function() {
                 function e(e) {
-                    this.middlewareStack = mc(), this.config = e
+                    this.middlewareStack = Mc(), this.config = e
                 }
                 return e.prototype.send = function(e, t, n) {
                     var r = "function" !== typeof t ? t : void 0,
                         o = "function" === typeof t ? t : n,
                         i = e.resolveMiddleware(this.middlewareStack, this.config, r);
                     if (!o) return i(e).then((function(e) {
                         return e.output
@@ -62324,29 +62352,29 @@
                     }), (function(e) {
                         return o(e)
                     })).catch((function() {}))
                 }, e.prototype.destroy = function() {
                     this.config.requestHandler.destroy && this.config.requestHandler.destroy()
                 }, e
             }(),
-            jc = function() {
-                this.middlewareStack = mc()
+            xc = function() {
+                this.middlewareStack = Mc()
             },
-            wc = function(e, t) {
-                return wc = Object.setPrototypeOf || {
+            Nc = function(e, t) {
+                return Nc = Object.setPrototypeOf || {
                     __proto__: []
                 }
                 instanceof Array && function(e, t) {
                     e.__proto__ = t
                 } || function(e, t) {
                     for (var n in t) t.hasOwnProperty(n) && (e[n] = t[n])
-                }, wc(e, t)
+                }, Nc(e, t)
             };
 
-        function xc(e, t) {
+        function Ic(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -62360,225 +62388,225 @@
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
 
-        function Nc() {
-            for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(xc(arguments[t]));
+        function Dc() {
+            for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(Ic(arguments[t]));
             return e
         }
-        var Ic = function() {
+        var Sc = function() {
             var e = Object.getPrototypeOf(this).constructor,
-                t = Function.bind.apply(String, Nc([null], arguments)),
+                t = Function.bind.apply(String, Dc([null], arguments)),
                 n = new t;
             return Object.setPrototypeOf(n, e.prototype), n
         };
-        Ic.prototype = Object.create(String.prototype, {
+        Sc.prototype = Object.create(String.prototype, {
             constructor: {
-                value: Ic,
+                value: Sc,
                 enumerable: !1,
                 writable: !0,
                 configurable: !0
             }
-        }), Object.setPrototypeOf(Ic, String);
+        }), Object.setPrototypeOf(Sc, String);
         ! function(e) {
             function t() {
                 return null !== e && e.apply(this, arguments) || this
             }(function(e, t) {
                 function n() {
                     this.constructor = e
                 }
-                wc(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
+                Nc(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
             })(t, e), t.prototype.deserializeJSON = function() {
                 return JSON.parse(e.prototype.toString.call(this))
             }, t.prototype.toJSON = function() {
                 return e.prototype.toString.call(this)
             }, t.fromObject = function(e) {
                 return e instanceof t ? e : new t(e instanceof String || "string" === typeof e ? e : JSON.stringify(e))
             }
-        }(Ic);
-        var Dc = function(e) {
+        }(Sc);
+        var Lc = function(e) {
                 function t(t) {
                     var n = e.call(this) || this;
                     return n.input = t, n
                 }
-                return vu(t, e), t.prototype.resolveMiddleware = function(e, t, n) {
-                    this.middlewareStack.use(fc(t, this.serialize, this.deserialize));
+                return bu(t, e), t.prototype.resolveMiddleware = function(e, t, n) {
+                    this.middlewareStack.use(hc(t, this.serialize, this.deserialize));
                     var r = e.concat(this.middlewareStack),
                         o = {
                             logger: t.logger,
                             clientName: "CognitoIdentityClient",
                             commandName: "GetCredentialsForIdentityCommand",
-                            inputFilterSensitiveLog: Qu.filterSensitiveLog,
-                            outputFilterSensitiveLog: Wu.filterSensitiveLog
+                            inputFilterSensitiveLog: Wu.filterSensitiveLog,
+                            outputFilterSensitiveLog: Zu.filterSensitiveLog
                         },
                         i = t.requestHandler;
                     return r.resolve((function(e) {
                         return i.handle(e.request, n || {})
                     }), o)
                 }, t.prototype.serialize = function(e, t) {
                     return function(e, t) {
-                        return bu(void 0, void 0, void 0, (function() {
+                        return wu(void 0, void 0, void 0, (function() {
                             var n, r;
-                            return ju(this, (function(o) {
+                            return xu(this, (function(o) {
                                 return n = {
                                     "content-type": "application/x-amz-json-1.1",
                                     "x-amz-target": "AWSCognitoIdentityService.GetCredentialsForIdentity"
-                                }, r = JSON.stringify(Fl(e, t)), [2, oc(t, n, "/", void 0, r)]
+                                }, r = JSON.stringify(Ql(e, t)), [2, ac(t, n, "/", void 0, r)]
                             }))
                         }))
                     }(e, t)
                 }, t.prototype.deserialize = function(e, t) {
                     return function(e, t) {
-                        return bu(void 0, void 0, void 0, (function() {
+                        return wu(void 0, void 0, void 0, (function() {
                             var n, r, o;
-                            return ju(this, (function(i) {
+                            return xu(this, (function(i) {
                                 switch (i.label) {
                                     case 0:
-                                        return e.statusCode >= 300 ? [2, Cl(e, t)] : [4, ic(e.body, t)];
+                                        return e.statusCode >= 300 ? [2, _l(e, t)] : [4, sc(e.body, t)];
                                     case 1:
-                                        return n = i.sent(), r = Hl(n, t), o = Mu({
-                                            $metadata: nc(e)
+                                        return n = i.sent(), r = Vl(n, t), o = ju({
+                                            $metadata: oc(e)
                                         }, r), [2, Promise.resolve(o)]
                                 }
                             }))
                         }))
                     }(e, t)
                 }, t
-            }(jc),
-            Sc = function(e, t) {
-                return Sc = Object.setPrototypeOf || {
+            }(xc),
+            kc = function(e, t) {
+                return kc = Object.setPrototypeOf || {
                     __proto__: []
                 }
                 instanceof Array && function(e, t) {
                     e.__proto__ = t
                 } || function(e, t) {
                     for (var n in t) t.hasOwnProperty(n) && (e[n] = t[n])
-                }, Sc(e, t)
+                }, kc(e, t)
             };
-        var Lc = function(e) {
+        var Cc = function(e) {
             function t(t, n) {
                 void 0 === n && (n = !0);
                 var r = e.call(this, t) || this;
                 return r.tryNextLink = n, r
             }
             return function(e, t) {
                 function n() {
                     this.constructor = e
                 }
-                Sc(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
+                kc(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
             }(t, e), t
         }(Error);
 
-        function kc(e) {
+        function Ec(e) {
             return Promise.all(Object.keys(e).reduce((function(t, n) {
                 var r = e[n];
                 return "string" === typeof r ? t.push([n, r]) : t.push(r().then((function(e) {
                     return [n, e]
                 }))), t
             }), [])).then((function(e) {
                 return e.reduce((function(e, t) {
-                    var n = yu(t, 2),
+                    var n = vu(t, 2),
                         r = n[0],
                         o = n[1];
                     return e[r] = o, e
                 }), {})
             }))
         }
 
-        function Cc(e) {
+        function _c(e) {
             var t = this;
             return function() {
-                return hu(t, void 0, void 0, (function() {
+                return yu(t, void 0, void 0, (function() {
                     var t, n, r, o, i, a, s, u, l, c, d, f, p;
-                    return gu(this, (function(h) {
+                    return mu(this, (function(h) {
                         switch (h.label) {
                             case 0:
-                                return c = (l = e.client).send, d = Dc.bind, p = {
+                                return c = (l = e.client).send, d = Lc.bind, p = {
                                     CustomRoleArn: e.customRoleArn,
                                     IdentityId: e.identityId
-                                }, e.logins ? [4, kc(e.logins)] : [3, 2];
+                                }, e.logins ? [4, Ec(e.logins)] : [3, 2];
                             case 1:
                                 return f = h.sent(), [3, 3];
                             case 2:
                                 f = void 0, h.label = 3;
                             case 3:
-                                return [4, c.apply(l, [new(d.apply(Dc, [void 0, (p.Logins = f, p)]))])];
+                                return [4, c.apply(l, [new(d.apply(Lc, [void 0, (p.Logins = f, p)]))])];
                             case 4:
                                 return t = h.sent().Credentials, n = void 0 === t ? function() {
-                                    throw new Lc("Response from Amazon Cognito contained no credentials")
+                                    throw new Cc("Response from Amazon Cognito contained no credentials")
                                 }() : t, r = n.AccessKeyId, o = void 0 === r ? function() {
-                                    throw new Lc("Response from Amazon Cognito contained no access key ID")
+                                    throw new Cc("Response from Amazon Cognito contained no access key ID")
                                 }() : r, i = n.Expiration, a = n.SecretKey, s = void 0 === a ? function() {
-                                    throw new Lc("Response from Amazon Cognito contained no secret key")
+                                    throw new Cc("Response from Amazon Cognito contained no secret key")
                                 }() : a, u = n.SessionToken, [2, {
                                     identityId: e.identityId,
                                     accessKeyId: o,
                                     secretAccessKey: s,
                                     sessionToken: u,
                                     expiration: i
                                 }]
                         }
                     }))
                 }))
             }
         }
-        var Ec = function(e) {
+        var Tc = function(e) {
                 function t(t) {
                     var n = e.call(this) || this;
                     return n.input = t, n
                 }
-                return vu(t, e), t.prototype.resolveMiddleware = function(e, t, n) {
-                    this.middlewareStack.use(fc(t, this.serialize, this.deserialize));
+                return bu(t, e), t.prototype.resolveMiddleware = function(e, t, n) {
+                    this.middlewareStack.use(hc(t, this.serialize, this.deserialize));
                     var r = e.concat(this.middlewareStack),
                         o = {
                             logger: t.logger,
                             clientName: "CognitoIdentityClient",
                             commandName: "GetIdCommand",
-                            inputFilterSensitiveLog: Zu.filterSensitiveLog,
-                            outputFilterSensitiveLog: Vu.filterSensitiveLog
+                            inputFilterSensitiveLog: qu.filterSensitiveLog,
+                            outputFilterSensitiveLog: Ju.filterSensitiveLog
                         },
                         i = t.requestHandler;
                     return r.resolve((function(e) {
                         return i.handle(e.request, n || {})
                     }), o)
                 }, t.prototype.serialize = function(e, t) {
                     return function(e, t) {
-                        return bu(void 0, void 0, void 0, (function() {
+                        return wu(void 0, void 0, void 0, (function() {
                             var n, r;
-                            return ju(this, (function(o) {
+                            return xu(this, (function(o) {
                                 return n = {
                                     "content-type": "application/x-amz-json-1.1",
                                     "x-amz-target": "AWSCognitoIdentityService.GetId"
-                                }, r = JSON.stringify(Yl(e, t)), [2, oc(t, n, "/", void 0, r)]
+                                }, r = JSON.stringify(Gl(e, t)), [2, ac(t, n, "/", void 0, r)]
                             }))
                         }))
                     }(e, t)
                 }, t.prototype.deserialize = function(e, t) {
                     return function(e, t) {
-                        return bu(void 0, void 0, void 0, (function() {
+                        return wu(void 0, void 0, void 0, (function() {
                             var n, r, o;
-                            return ju(this, (function(i) {
+                            return xu(this, (function(i) {
                                 switch (i.label) {
                                     case 0:
-                                        return e.statusCode >= 300 ? [2, El(e, t)] : [4, ic(e.body, t)];
+                                        return e.statusCode >= 300 ? [2, Tl(e, t)] : [4, sc(e.body, t)];
                                     case 1:
-                                        return n = i.sent(), r = Zl(n, t), o = Mu({
-                                            $metadata: nc(e)
+                                        return n = i.sent(), r = ql(n, t), o = ju({
+                                            $metadata: oc(e)
                                         }, r), [2, Promise.resolve(o)]
                                 }
                             }))
                         }))
                     }(e, t)
                 }, t
-            }(jc),
-            _c = "IdentityIds",
-            Tc = function() {
+            }(xc),
+            Ac = "IdentityIds",
+            Oc = function() {
                 function e(e) {
                     void 0 === e && (e = "aws:cognito-identity-ids"), this.dbName = e
                 }
                 return e.prototype.getItem = function(e) {
                     return this.withObjectStore("readonly", (function(t) {
                         var n = t.get(e);
                         return new Promise((function(e) {
@@ -62625,106 +62653,106 @@
                             n(e.error)
                         }, e.onblocked = function() {
                             n(new Error("Unable to access DB"))
                         }, e.onupgradeneeded = function() {
                             var t = e.result;
                             t.onerror = function() {
                                 n(new Error("Failed to create object store"))
-                            }, t.createObjectStore(_c, {
+                            }, t.createObjectStore(Ac, {
                                 keyPath: "id"
                             })
                         }
                     }))
                 }, e.prototype.withObjectStore = function(e, t) {
                     return this.getDb().then((function(n) {
-                        var r = n.transaction(_c, e);
+                        var r = n.transaction(Ac, e);
                         return r.oncomplete = function() {
                             return n.close()
                         }, new Promise((function(e, n) {
                             r.onerror = function() {
                                 return n(r.error)
-                            }, e(t(r.objectStore(_c)))
+                            }, e(t(r.objectStore(Ac)))
                         })).catch((function(e) {
                             throw n.close(), e
                         }))
                     }))
                 }, e
             }(),
-            Ac = new(function() {
+            zc = new(function() {
                 function e(e) {
                     void 0 === e && (e = {}), this.store = e
                 }
                 return e.prototype.getItem = function(e) {
                     return e in this.store ? this.store[e] : null
                 }, e.prototype.removeItem = function(e) {
                     delete this.store[e]
                 }, e.prototype.setItem = function(e, t) {
                     this.store[e] = t
                 }, e
             }());
 
-        function Oc(e) {
+        function Uc(e) {
             var t = this,
                 n = e.accountId,
                 r = e.cache,
-                o = void 0 === r ? "object" === typeof self && self.indexedDB ? new Tc : "object" === typeof window && window.localStorage ? window.localStorage : Ac : r,
+                o = void 0 === r ? "object" === typeof self && self.indexedDB ? new Oc : "object" === typeof window && window.localStorage ? window.localStorage : zc : r,
                 i = e.client,
                 a = e.customRoleArn,
                 s = e.identityPoolId,
                 u = e.logins,
                 l = e.userIdentifier,
                 c = void 0 === l ? u && 0 !== Object.keys(u).length ? void 0 : "ANONYMOUS" : l,
                 d = c ? "aws:cognito-identity-credentials:" + s + ":" + c : void 0,
                 f = function() {
-                    return hu(t, void 0, void 0, (function() {
+                    return yu(t, void 0, void 0, (function() {
                         var e, t, r, l, c, p, h, g, y;
-                        return gu(this, (function(m) {
+                        return mu(this, (function(m) {
                             switch (m.label) {
                                 case 0:
                                     return (t = d) ? [4, o.getItem(d)] : [3, 2];
                                 case 1:
                                     t = m.sent(), m.label = 2;
                                 case 2:
-                                    return (e = t) ? [3, 7] : (p = (c = i).send, h = Ec.bind, y = {
+                                    return (e = t) ? [3, 7] : (p = (c = i).send, h = Tc.bind, y = {
                                         AccountId: n,
                                         IdentityPoolId: s
-                                    }, u ? [4, kc(u)] : [3, 4]);
+                                    }, u ? [4, Ec(u)] : [3, 4]);
                                 case 3:
                                     return g = m.sent(), [3, 5];
                                 case 4:
                                     g = void 0, m.label = 5;
                                 case 5:
-                                    return [4, p.apply(c, [new(h.apply(Ec, [void 0, (y.Logins = g, y)]))])];
+                                    return [4, p.apply(c, [new(h.apply(Tc, [void 0, (y.Logins = g, y)]))])];
                                 case 6:
                                     r = m.sent().IdentityId, l = void 0 === r ? function() {
-                                        throw new Lc("Response from Amazon Cognito contained no identity ID")
+                                        throw new Cc("Response from Amazon Cognito contained no identity ID")
                                     }() : r, e = l, d && Promise.resolve(o.setItem(d, e)).catch((function() {})), m.label = 7;
                                 case 7:
-                                    return [2, (f = Cc({
+                                    return [2, (f = _c({
                                         client: i,
                                         customRoleArn: a,
                                         logins: u,
                                         identityId: e
                                     }))()]
                             }
                         }))
                     }))
                 };
             return function() {
                 return f().catch((function(e) {
-                    return hu(t, void 0, void 0, (function() {
-                        return gu(this, (function(t) {
+                    return yu(t, void 0, void 0, (function() {
+                        return mu(this, (function(t) {
                             throw d && Promise.resolve(o.removeItem(d)).catch((function() {})), e
                         }))
                     }))
                 }))
             }
         }
-        var zc = new Ws("Parser"),
-            Uc = function(e) {
+        var Pc = new Zs("Parser"),
+            Rc = function(e) {
                 var t, n = {};
                 if (e.aws_mobile_analytics_app_id) {
                     var r = {
                         AWSPinpoint: {
                             appId: e.aws_mobile_analytics_app_id,
                             region: e.aws_mobile_analytics_app_region
                         }
@@ -62741,23 +62769,23 @@
                     signUpVerificationMethod: e.aws_cognito_sign_up_verification_method || "code"
                 }), t = e.aws_user_files_s3_bucket ? {
                     AWSS3: {
                         bucket: e.aws_user_files_s3_bucket,
                         region: e.aws_user_files_s3_bucket_region,
                         dangerouslyConnectToHttpEndpointForTesting: e.aws_user_files_s3_dangerously_connect_to_http_endpoint_for_testing
                     }
-                } : e ? e.Storage || e : {}, e.Logging && (n.Logging = Us(Us({}, e.Logging), {
+                } : e ? e.Storage || e : {}, e.Logging && (n.Logging = Rs(Rs({}, e.Logging), {
                     region: e.aws_project_region
                 })), e.geo && (n.Geo = Object.assign({}, e.geo), e.geo.amazon_location_service && (n.Geo = {
                     AmazonLocationService: e.geo.amazon_location_service
-                })), n.Analytics = Object.assign({}, n.Analytics, e.Analytics), n.Auth = Object.assign({}, n.Auth, e.Auth), n.Storage = Object.assign({}, t), n.Logging = Object.assign({}, n.Logging, e.Logging), zc.debug("parse config", e, "to amplifyconfig", n), n
+                })), n.Analytics = Object.assign({}, n.Analytics, e.Analytics), n.Auth = Object.assign({}, n.Auth, e.Auth), n.Storage = Object.assign({}, t), n.Logging = Object.assign({}, n.Logging, e.Logging), Pc.debug("parse config", e, "to amplifyconfig", n), n
             },
-            Pc = __webpack_require__(3219);
+            Bc = __webpack_require__(3219);
 
-        function Rc(e, t, n, r) {
+        function Fc(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -62777,15 +62805,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function Bc(e, t) {
+        function Yc(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -62853,15 +62881,15 @@
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
 
-        function Fc(e) {
+        function Qc(e) {
             var t = "function" === typeof Symbol && Symbol.iterator,
                 n = t && e[t],
                 r = 0;
             if (n) return n.call(e);
             if (e && "number" === typeof e.length) return {
                 next: function() {
                     return e && r >= e.length && (e = void 0), {
@@ -62869,36 +62897,36 @@
                         done: !e
                     }
                 }
             };
             throw new TypeError(t ? "Object is not iterable." : "Symbol.iterator is not defined.")
         }
 
-        function Yc(e) {
+        function Gc(e) {
             var t = "function" === typeof Symbol && Symbol.iterator,
                 n = t && e[t],
                 r = 0;
             if (n) return n.call(e);
             if (e && "number" === typeof e.length) return {
                 next: function() {
                     return e && r >= e.length && (e = void 0), {
                         value: e && e[r++],
                         done: !e
                     }
                 }
             };
             throw new TypeError(t ? "Object is not iterable." : "Symbol.iterator is not defined.")
         }
-        var Qc = function(e) {
-                return encodeURIComponent(e).replace(/[!'()*]/g, Gc)
+        var Wc = function(e) {
+                return encodeURIComponent(e).replace(/[!'()*]/g, Hc)
             },
-            Gc = function(e) {
+            Hc = function(e) {
                 return "%" + e.charCodeAt(0).toString(16).toUpperCase()
             };
-        for (var Wc = function() {
+        for (var Zc = function() {
                 function e(e) {
                     var t = (void 0 === e ? {} : e).requestTimeout;
                     this.requestTimeout = t
                 }
                 return e.prototype.destroy = function() {}, e.prototype.handle = function(e, t) {
                     var n = (void 0 === t ? {} : t).abortSignal,
                         r = this.requestTimeout;
@@ -62907,22 +62935,22 @@
                         return o.name = "AbortError", Promise.reject(o)
                     }
                     var i = e.path;
                     if (e.query) {
                         var a = function(e) {
                             var t, n, r = [];
                             try {
-                                for (var o = Yc(Object.keys(e).sort()), i = o.next(); !i.done; i = o.next()) {
+                                for (var o = Gc(Object.keys(e).sort()), i = o.next(); !i.done; i = o.next()) {
                                     var a = i.value,
                                         s = e[a];
-                                    if (a = Qc(a), Array.isArray(s))
-                                        for (var u = 0, l = s.length; u < l; u++) r.push(a + "=" + Qc(s[u]));
+                                    if (a = Wc(a), Array.isArray(s))
+                                        for (var u = 0, l = s.length; u < l; u++) r.push(a + "=" + Wc(s[u]));
                                     else {
                                         var c = a;
-                                        (s || "string" === typeof s) && (c += "=" + Qc(s)), r.push(c)
+                                        (s || "string" === typeof s) && (c += "=" + Wc(s)), r.push(c)
                                     }
                                 }
                             } catch (d) {
                                 t = {
                                     error: d
                                 }
                             } finally {
@@ -62946,15 +62974,15 @@
                         };
                     "undefined" !== typeof AbortController && (c.signal = n);
                     var d, f = new Request(l, c),
                         p = [fetch(f).then((function(e) {
                             var t, n, r = e.headers,
                                 o = {};
                             try {
-                                for (var i = Fc(r.entries()), a = i.next(); !a.done; a = i.next()) {
+                                for (var i = Qc(r.entries()), a = i.next(); !a.done; a = i.next()) {
                                     var s = a.value;
                                     o[s[0]] = s[1]
                                 }
                             } catch (u) {
                                 t = {
                                     error: u
                                 }
@@ -62962,22 +62990,22 @@
                                 try {
                                     a && !a.done && (n = i.return) && n.call(i)
                                 } finally {
                                     if (t) throw t.error
                                 }
                             }
                             return void 0 !== e.body ? {
-                                response: new Dl({
+                                response: new Ll({
                                     headers: o,
                                     statusCode: e.status,
                                     body: e.body
                                 })
                             } : e.blob().then((function(t) {
                                 return {
-                                    response: new Dl({
+                                    response: new Ll({
                                         headers: o,
                                         statusCode: e.status,
                                         body: t
                                     })
                                 }
                             }))
                         })), (d = r, void 0 === d && (d = 0), new Promise((function(e, t) {
@@ -62989,46 +63017,46 @@
                     return n && p.push(new Promise((function(e, t) {
                         n.onabort = function() {
                             var e = new Error("Request aborted");
                             e.name = "AbortError", t(e)
                         }
                     }))), Promise.race(p)
                 }, e
-            }(), Hc = {}, Zc = new Array(64), Vc = 0, qc = "A".charCodeAt(0), Jc = "Z".charCodeAt(0); Vc + qc <= Jc; Vc++) {
-            var Kc = String.fromCharCode(Vc + qc);
-            Hc[Kc] = Vc, Zc[Vc] = Kc
-        }
-        for (Vc = 0, qc = "a".charCodeAt(0), Jc = "z".charCodeAt(0); Vc + qc <= Jc; Vc++) {
-            Kc = String.fromCharCode(Vc + qc);
-            var Xc = Vc + 26;
-            Hc[Kc] = Xc, Zc[Xc] = Kc
-        }
-        for (Vc = 0; Vc < 10; Vc++) {
-            Hc[Vc.toString(10)] = Vc + 52;
-            Kc = Vc.toString(10), Xc = Vc + 52;
-            Hc[Kc] = Xc, Zc[Xc] = Kc
+            }(), Vc = {}, qc = new Array(64), Jc = 0, Kc = "A".charCodeAt(0), Xc = "Z".charCodeAt(0); Jc + Kc <= Xc; Jc++) {
+            var $c = String.fromCharCode(Jc + Kc);
+            Vc[$c] = Jc, qc[Jc] = $c
+        }
+        for (Jc = 0, Kc = "a".charCodeAt(0), Xc = "z".charCodeAt(0); Jc + Kc <= Xc; Jc++) {
+            $c = String.fromCharCode(Jc + Kc);
+            var ed = Jc + 26;
+            Vc[$c] = ed, qc[ed] = $c
+        }
+        for (Jc = 0; Jc < 10; Jc++) {
+            Vc[Jc.toString(10)] = Jc + 52;
+            $c = Jc.toString(10), ed = Jc + 52;
+            Vc[$c] = ed, qc[ed] = $c
         }
-        Hc["+"] = 62, Zc[62] = "+", Hc["/"] = 63, Zc[63] = "/";
+        Vc["+"] = 62, qc[62] = "+", Vc["/"] = 63, qc[63] = "/";
 
-        function $c(e) {
+        function td(e) {
             var t = e.length / 4 * 3;
             "==" === e.substr(-2) ? t -= 2 : "=" === e.substr(-1) && t--;
             for (var n = new ArrayBuffer(t), r = new DataView(n), o = 0; o < e.length; o += 4) {
-                for (var i = 0, a = 0, s = o, u = o + 3; s <= u; s++) "=" !== e[s] ? (i |= Hc[e[s]] << 6 * (u - s), a += 6) : i >>= 6;
+                for (var i = 0, a = 0, s = o, u = o + 3; s <= u; s++) "=" !== e[s] ? (i |= Vc[e[s]] << 6 * (u - s), a += 6) : i >>= 6;
                 var l = o / 4 * 3;
                 i >>= a % 8;
                 for (var c = Math.floor(a / 8), d = 0; d < c; d++) {
                     var f = 8 * (c - d - 1);
                     r.setUint8(l + d, (i & 255 << f) >> f)
                 }
             }
             return new Uint8Array(n)
         }
 
-        function ed(e) {
+        function nd(e) {
             return new Promise((function(t, n) {
                 var r = new FileReader;
                 r.onloadend = function() {
                     var e;
                     if (2 !== r.readyState) return n(new Error("Reader aborted too early"));
                     var o = null !== (e = r.result) && void 0 !== e ? e : "",
                         i = o.indexOf(","),
@@ -63037,23 +63065,23 @@
                 }, r.onabort = function() {
                     return n(new Error("Read aborted"))
                 }, r.onerror = function() {
                     return n(r.error)
                 }, r.readAsDataURL(e)
             }))
         }
-        var td = function() {
-            return td = Object.assign || function(e) {
+        var rd = function() {
+            return rd = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, td.apply(this, arguments)
+            }, rd.apply(this, arguments)
         };
 
-        function nd(e, t, n, r) {
+        function od(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -63073,15 +63101,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function rd(e, t) {
+        function id(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -63149,15 +63177,15 @@
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
 
-        function od(e, t) {
+        function ad(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -63170,65 +63198,65 @@
                     r && !r.done && (n = i.return) && n.call(i)
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
-        var id = function(e) {
+        var sd = function(e) {
                 return function(t, n) {
                     return function(r) {
-                        return nd(void 0, void 0, void 0, (function() {
+                        return od(void 0, void 0, void 0, (function() {
                             var o;
-                            return rd(this, (function(i) {
+                            return id(this, (function(i) {
                                 return (null === (o = null === e || void 0 === e ? void 0 : e.retryStrategy) || void 0 === o ? void 0 : o.mode) && (n.userAgent = function() {
-                                    for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(od(arguments[t]));
+                                    for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(ad(arguments[t]));
                                     return e
                                 }(n.userAgent || [], [
                                     ["cfg/retry-mode", e.retryStrategy.mode]
                                 ])), [2, e.retryStrategy.retry(t, r)]
                             }))
                         }))
                     }
                 }
             },
-            ad = {
+            ud = {
                 name: "retryMiddleware",
                 tags: ["RETRY"],
                 step: "finalizeRequest",
                 priority: "high",
                 override: !0
             },
-            sd = ["AuthFailure", "InvalidSignatureException", "RequestExpired", "RequestInTheFuture", "RequestTimeTooSkewed", "SignatureDoesNotMatch"],
-            ud = ["BandwidthLimitExceeded", "EC2ThrottledException", "LimitExceededException", "PriorRequestNotComplete", "ProvisionedThroughputExceededException", "RequestLimitExceeded", "RequestThrottled", "RequestThrottledException", "SlowDown", "ThrottledException", "Throttling", "ThrottlingException", "TooManyRequestsException", "TransactionInProgressException"],
-            ld = ["AbortError", "TimeoutError", "RequestTimeout", "RequestTimeoutException"],
-            cd = [500, 502, 503, 504],
-            dd = function(e) {
+            ld = ["AuthFailure", "InvalidSignatureException", "RequestExpired", "RequestInTheFuture", "RequestTimeTooSkewed", "SignatureDoesNotMatch"],
+            cd = ["BandwidthLimitExceeded", "EC2ThrottledException", "LimitExceededException", "PriorRequestNotComplete", "ProvisionedThroughputExceededException", "RequestLimitExceeded", "RequestThrottled", "RequestThrottledException", "SlowDown", "ThrottledException", "Throttling", "ThrottlingException", "TooManyRequestsException", "TransactionInProgressException"],
+            dd = ["AbortError", "TimeoutError", "RequestTimeout", "RequestTimeoutException"],
+            fd = [500, 502, 503, 504],
+            pd = function(e) {
                 var t, n;
-                return 429 === (null === (t = e.$metadata) || void 0 === t ? void 0 : t.httpStatusCode) || ud.includes(e.name) || 1 == (null === (n = e.$retryable) || void 0 === n ? void 0 : n.throttling)
+                return 429 === (null === (t = e.$metadata) || void 0 === t ? void 0 : t.httpStatusCode) || cd.includes(e.name) || 1 == (null === (n = e.$retryable) || void 0 === n ? void 0 : n.throttling)
             },
-            fd = __webpack_require__(6231),
-            pd = function(e, t) {
+            hd = __webpack_require__(6231),
+            gd = function(e, t) {
                 return Math.floor(Math.min(2e4, Math.random() * Math.pow(2, t) * e))
             },
-            hd = function(e) {
+            yd = function(e) {
                 return !!e && (function(e) {
                     return void 0 !== e.$retryable
                 }(e) || function(e) {
-                    return sd.includes(e.name)
-                }(e) || dd(e) || function(e) {
+                    return ld.includes(e.name)
+                }(e) || pd(e) || function(e) {
                     var t;
-                    return ld.includes(e.name) || cd.includes((null === (t = e.$metadata) || void 0 === t ? void 0 : t.httpStatusCode) || 0)
+                    return dd.includes(e.name) || fd.includes((null === (t = e.$metadata) || void 0 === t ? void 0 : t.httpStatusCode) || 0)
                 }(e))
             },
-            gd = "standard",
-            yd = function() {
+            md = "standard",
+            vd = function() {
                 function e(e, t) {
                     var n, r, o;
-                    this.maxAttemptsProvider = e, this.mode = gd, this.retryDecider = null !== (n = null === t || void 0 === t ? void 0 : t.retryDecider) && void 0 !== n ? n : hd, this.delayDecider = null !== (r = null === t || void 0 === t ? void 0 : t.delayDecider) && void 0 !== r ? r : pd, this.retryQuota = null !== (o = null === t || void 0 === t ? void 0 : t.retryQuota) && void 0 !== o ? o : function(e) {
+                    this.maxAttemptsProvider = e, this.mode = md, this.retryDecider = null !== (n = null === t || void 0 === t ? void 0 : t.retryDecider) && void 0 !== n ? n : yd, this.delayDecider = null !== (r = null === t || void 0 === t ? void 0 : t.delayDecider) && void 0 !== r ? r : gd, this.retryQuota = null !== (o = null === t || void 0 === t ? void 0 : t.retryQuota) && void 0 !== o ? o : function(e) {
                         var t = e,
                             n = e,
                             r = function(e) {
                                 return "TimeoutError" === e.name ? 10 : 5
                             },
                             o = function(e) {
                                 return r(e) <= n
@@ -63245,52 +63273,52 @@
                             }
                         })
                     }(500)
                 }
                 return e.prototype.shouldRetry = function(e, t, n) {
                     return t < n && this.retryDecider(e) && this.retryQuota.hasRetryTokens(e)
                 }, e.prototype.getMaxAttempts = function() {
-                    return nd(this, void 0, void 0, (function() {
+                    return od(this, void 0, void 0, (function() {
                         var e;
-                        return rd(this, (function(t) {
+                        return id(this, (function(t) {
                             switch (t.label) {
                                 case 0:
                                     return t.trys.push([0, 2, , 3]), [4, this.maxAttemptsProvider()];
                                 case 1:
                                     return e = t.sent(), [3, 3];
                                 case 2:
                                     return t.sent(), e = 3, [3, 3];
                                 case 3:
                                     return [2, e]
                             }
                         }))
                     }))
                 }, e.prototype.retry = function(e, t) {
-                    return nd(this, void 0, void 0, (function() {
+                    return od(this, void 0, void 0, (function() {
                         var n, r, o, i, a, s, u, l;
-                        return rd(this, (function(c) {
+                        return id(this, (function(c) {
                             switch (c.label) {
                                 case 0:
                                     return r = 0, o = 0, [4, this.getMaxAttempts()];
                                 case 1:
-                                    i = c.sent(), a = t.request, kl.isInstance(a) && (a.headers["amz-sdk-invocation-id"] = (0, fd.v4)()), s = function() {
+                                    i = c.sent(), a = t.request, El.isInstance(a) && (a.headers["amz-sdk-invocation-id"] = (0, hd.v4)()), s = function() {
                                         var s, l, c, d, f;
-                                        return rd(this, (function(p) {
+                                        return id(this, (function(p) {
                                             switch (p.label) {
                                                 case 0:
-                                                    return p.trys.push([0, 2, , 5]), kl.isInstance(a) && (a.headers["amz-sdk-request"] = "attempt=" + (r + 1) + "; max=" + i), [4, e(t)];
+                                                    return p.trys.push([0, 2, , 5]), El.isInstance(a) && (a.headers["amz-sdk-request"] = "attempt=" + (r + 1) + "; max=" + i), [4, e(t)];
                                                 case 1:
                                                     return s = p.sent(), l = s.response, c = s.output, u.retryQuota.releaseRetryTokens(n), c.$metadata.attempts = r + 1, c.$metadata.totalRetryDelay = o, [2, {
                                                         value: {
                                                             response: l,
                                                             output: c
                                                         }
                                                     }];
                                                 case 2:
-                                                    return d = p.sent(), r++, u.shouldRetry(d, r, i) ? (n = u.retryQuota.retrieveRetryTokens(d), f = u.delayDecider(dd(d) ? 500 : 100, r), o += f, [4, new Promise((function(e) {
+                                                    return d = p.sent(), r++, u.shouldRetry(d, r, i) ? (n = u.retryQuota.retrieveRetryTokens(d), f = u.delayDecider(pd(d) ? 500 : 100, r), o += f, [4, new Promise((function(e) {
                                                         return setTimeout(e, f)
                                                     }))]) : [3, 4];
                                                 case 3:
                                                     return p.sent(), [2, "continue"];
                                                 case 4:
                                                     throw d.$metadata || (d.$metadata = {}), d.$metadata.attempts = r, d.$metadata.totalRetryDelay = o, d;
                                                 case 5:
@@ -63305,25 +63333,25 @@
                                 case 4:
                                     return [2]
                             }
                         }))
                     }))
                 }, e
             }(),
-            md = function(e) {
+            Md = function(e) {
                 if (void 0 === e && (e = 3), "number" === typeof e) {
                     var t = Promise.resolve(e);
                     return function() {
                         return t
                     }
                 }
                 return e
             };
 
-        function vd(e, t, n, r) {
+        function bd(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -63343,15 +63371,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function Md(e, t) {
+        function jd(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -63418,25 +63446,25 @@
                             value: i[0] ? i[1] : void 0,
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
-        var bd = __webpack_require__(984),
-            jd = __webpack_require__.n(bd),
-            wd = __webpack_require__(5863),
-            xd = "cognito-identity.{region}.amazonaws.com",
-            Nd = new Set(["af-south-1", "ap-east-1", "ap-northeast-1", "ap-northeast-2", "ap-south-1", "ap-southeast-1", "ap-southeast-2", "ca-central-1", "eu-central-1", "eu-north-1", "eu-south-1", "eu-west-1", "eu-west-2", "eu-west-3", "me-south-1", "sa-east-1", "us-east-1", "us-east-2", "us-west-1", "us-west-2"]),
-            Id = new Set(["cn-north-1", "cn-northwest-1"]),
-            Dd = new Set(["us-iso-east-1"]),
-            Sd = new Set(["us-isob-east-1"]),
-            Ld = new Set(["us-gov-east-1", "us-gov-west-1"]);
+        var wd = __webpack_require__(984),
+            xd = __webpack_require__.n(wd),
+            Nd = __webpack_require__(5863),
+            Id = "cognito-identity.{region}.amazonaws.com",
+            Dd = new Set(["af-south-1", "ap-east-1", "ap-northeast-1", "ap-northeast-2", "ap-south-1", "ap-southeast-1", "ap-southeast-2", "ca-central-1", "eu-central-1", "eu-north-1", "eu-south-1", "eu-west-1", "eu-west-2", "eu-west-3", "me-south-1", "sa-east-1", "us-east-1", "us-east-2", "us-west-1", "us-west-2"]),
+            Sd = new Set(["cn-north-1", "cn-northwest-1"]),
+            Ld = new Set(["us-iso-east-1"]),
+            kd = new Set(["us-isob-east-1"]),
+            Cd = new Set(["us-gov-east-1", "us-gov-west-1"]);
 
-        function kd(e) {
+        function Ed(e) {
             var t = "function" === typeof Symbol && Symbol.iterator,
                 n = t && e[t],
                 r = 0;
             if (n) return n.call(e);
             if (e && "number" === typeof e.length) return {
                 next: function() {
                     return e && r >= e.length && (e = void 0), {
@@ -63444,15 +63472,15 @@
                         done: !e
                     }
                 }
             };
             throw new TypeError(t ? "Object is not iterable." : "Symbol.iterator is not defined.")
         }
 
-        function Cd(e, t) {
+        function _d(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -63465,15 +63493,15 @@
                     r && !r.done && (n = i.return) && n.call(i)
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
-        var Ed, _d = {
+        var Td, Ad = {
                 apiVersion: "2014-06-30",
                 disableHostPrefix: !1,
                 logger: {},
                 regionInfoProvider: function(e, t) {
                     var n = void 0;
                     switch (e) {
                         case "ap-northeast-1":
@@ -63609,51 +63637,51 @@
                         case "us-west-2":
                             n = {
                                 hostname: "cognito-identity.us-west-2.amazonaws.com",
                                 partition: "aws"
                             };
                             break;
                         default:
-                            Nd.has(e) && (n = {
-                                hostname: xd.replace("{region}", e),
+                            Dd.has(e) && (n = {
+                                hostname: Id.replace("{region}", e),
                                 partition: "aws"
-                            }), Id.has(e) && (n = {
+                            }), Sd.has(e) && (n = {
                                 hostname: "cognito-identity.{region}.amazonaws.com.cn".replace("{region}", e),
                                 partition: "aws-cn"
-                            }), Dd.has(e) && (n = {
+                            }), Ld.has(e) && (n = {
                                 hostname: "cognito-identity.{region}.c2s.ic.gov".replace("{region}", e),
                                 partition: "aws-iso"
-                            }), Sd.has(e) && (n = {
+                            }), kd.has(e) && (n = {
                                 hostname: "cognito-identity.{region}.sc2s.sgov.gov".replace("{region}", e),
                                 partition: "aws-iso-b"
-                            }), Ld.has(e) && (n = {
+                            }), Cd.has(e) && (n = {
                                 hostname: "cognito-identity.{region}.amazonaws.com".replace("{region}", e),
                                 partition: "aws-us-gov"
                             }), void 0 === n && (n = {
-                                hostname: xd.replace("{region}", e),
+                                hostname: Id.replace("{region}", e),
                                 partition: "aws"
                             })
                     }
-                    return Promise.resolve(Mu({
+                    return Promise.resolve(ju({
                         signingService: "cognito-identity"
                     }, n))
                 },
                 serviceId: "Cognito Identity",
                 urlParser: function(e) {
                     var t, n = new URL(e),
                         r = n.hostname,
                         o = n.pathname,
                         i = n.port,
                         a = n.protocol,
                         s = n.search;
                     return s && (t = function(e) {
                         var t, n, r = {};
                         if (e = e.replace(/^\?/, "")) try {
-                            for (var o = kd(e.split("&")), i = o.next(); !i.done; i = o.next()) {
-                                var a = Cd(i.value.split("="), 2),
+                            for (var o = Ed(e.split("&")), i = o.next(); !i.done; i = o.next()) {
+                                var a = _d(i.value.split("="), 2),
                                     s = a[0],
                                     u = a[1],
                                     l = void 0 === u ? null : u;
                                 s = decodeURIComponent(s), l && (l = decodeURIComponent(l)), s in r ? Array.isArray(r[s]) ? r[s].push(l) : r[s] = [r[s], l] : r[s] = l
                             }
                         } catch (c) {
                             t = {
@@ -63672,25 +63700,25 @@
                         port: i ? parseInt(i) : void 0,
                         protocol: a,
                         path: o,
                         query: t
                     }
                 }
             },
-            Td = Mu(Mu({}, _d), {
+            Od = ju(ju({}, Ad), {
                 runtime: "browser",
-                base64Decoder: $c,
+                base64Decoder: td,
                 base64Encoder: function(e) {
                     for (var t = "", n = 0; n < e.length; n += 3) {
                         for (var r = 0, o = 0, i = n, a = Math.min(n + 3, e.length); i < a; i++) r |= e[i] << 8 * (a - i - 1), o += 8;
                         var s = Math.ceil(o / 6);
                         r <<= 6 * s - o;
                         for (var u = 1; u <= s; u++) {
                             var l = 6 * (s - u);
-                            t += Zc[(r & 63 << l) >> l]
+                            t += qc[(r & 63 << l) >> l]
                         }
                         t += "==".slice(0, 4 - s)
                     }
                     return t
                 },
                 bodyLengthChecker: function(e) {
                     if ("string" === typeof e) {
@@ -63707,79 +63735,79 @@
                         return Promise.reject(new Error("Credential is missing"))
                     }
                 },
                 defaultUserAgentProvider: function(e) {
                     var t = e.serviceId,
                         n = e.clientVersion;
                     return function() {
-                        return vd(void 0, void 0, void 0, (function() {
+                        return bd(void 0, void 0, void 0, (function() {
                             var e, r, o, i, a, s, u, l, c;
-                            return Md(this, (function(d) {
-                                return e = (null === (o = null === window || void 0 === window ? void 0 : window.navigator) || void 0 === o ? void 0 : o.userAgent) ? jd().parse(window.navigator.userAgent) : void 0, r = [
+                            return jd(this, (function(d) {
+                                return e = (null === (o = null === window || void 0 === window ? void 0 : window.navigator) || void 0 === o ? void 0 : o.userAgent) ? xd().parse(window.navigator.userAgent) : void 0, r = [
                                     ["aws-sdk-js", n],
                                     ["os/" + ((null === (i = null === e || void 0 === e ? void 0 : e.os) || void 0 === i ? void 0 : i.name) || "other"), null === (a = null === e || void 0 === e ? void 0 : e.os) || void 0 === a ? void 0 : a.version],
                                     ["lang/js"],
                                     ["md/browser", (null !== (u = null === (s = null === e || void 0 === e ? void 0 : e.browser) || void 0 === s ? void 0 : s.name) && void 0 !== u ? u : "unknown") + "_" + (null !== (c = null === (l = null === e || void 0 === e ? void 0 : e.browser) || void 0 === l ? void 0 : l.version) && void 0 !== c ? c : "unknown")]
                                 ], t && r.push(["api/" + t, n]), [2, r]
                             }))
                         }))
                     }
                 }({
-                    serviceId: _d.serviceId,
+                    serviceId: Ad.serviceId,
                     clientVersion: "3.6.1"
                 }),
                 maxAttempts: 3,
-                region: (Ed = "Region is missing", function() {
-                    return Promise.reject(Ed)
+                region: (Td = "Region is missing", function() {
+                    return Promise.reject(Td)
                 }),
-                requestHandler: new Wc,
-                sha256: Pc.Sha256,
+                requestHandler: new Zc,
+                sha256: Bc.Sha256,
                 streamCollector: function(e) {
                     return "function" === typeof Blob && e instanceof Blob ? function(e) {
-                        return Rc(this, void 0, void 0, (function() {
+                        return Fc(this, void 0, void 0, (function() {
                             var t, n;
-                            return Bc(this, (function(r) {
+                            return Yc(this, (function(r) {
                                 switch (r.label) {
                                     case 0:
-                                        return [4, ed(e)];
+                                        return [4, nd(e)];
                                     case 1:
-                                        return t = r.sent(), n = $c(t), [2, new Uint8Array(n)]
+                                        return t = r.sent(), n = td(t), [2, new Uint8Array(n)]
                                 }
                             }))
                         }))
                     }(e) : function(e) {
-                        return Rc(this, void 0, void 0, (function() {
+                        return Fc(this, void 0, void 0, (function() {
                             var t, n, r, o, i, a, s;
-                            return Bc(this, (function(u) {
+                            return Yc(this, (function(u) {
                                 switch (u.label) {
                                     case 0:
                                         t = new Uint8Array(0), n = e.getReader(), r = !1, u.label = 1;
                                     case 1:
                                         return r ? [3, 3] : [4, n.read()];
                                     case 2:
                                         return o = u.sent(), i = o.done, (a = o.value) && (s = t, (t = new Uint8Array(s.length + a.length)).set(s), t.set(a, s.length)), r = i, [3, 1];
                                     case 3:
                                         return [2, t]
                                 }
                             }))
                         }))
                     }(e)
                 },
-                utf8Decoder: wd.fromUtf8,
-                utf8Encoder: wd.toUtf8
+                utf8Decoder: Nd.fromUtf8,
+                utf8Encoder: Nd.toUtf8
             });
-        var Ad = function() {
-            return Ad = Object.assign || function(e) {
+        var zd = function() {
+            return zd = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, Ad.apply(this, arguments)
+            }, zd.apply(this, arguments)
         };
 
-        function Od(e, t, n, r) {
+        function Ud(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -63799,15 +63827,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function zd(e, t) {
+        function Pd(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -63874,15 +63902,15 @@
                             value: i[0] ? i[1] : void 0,
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
-        var Ud = function(e) {
+        var Rd = function(e) {
                 var t = e.endpoint,
                     n = e.urlParser;
                 if ("string" === typeof t) {
                     var r = Promise.resolve(n(t));
                     return function() {
                         return r
                     }
@@ -63891,49 +63919,49 @@
                     var o = Promise.resolve(t);
                     return function() {
                         return o
                     }
                 }
                 return t
             },
-            Pd = function(e) {
-                return Od(void 0, void 0, void 0, (function() {
+            Bd = function(e) {
+                return Ud(void 0, void 0, void 0, (function() {
                     var t, n, r, o, i;
-                    return zd(this, (function(a) {
+                    return Pd(this, (function(a) {
                         switch (a.label) {
                             case 0:
                                 return t = e.tls, n = void 0 === t || t, [4, e.region()];
                             case 1:
                                 if (r = a.sent(), !new RegExp(/^([a-zA-Z0-9]|[a-zA-Z0-9][a-zA-Z0-9-]{0,61}[a-zA-Z0-9])$/).test(r)) throw new Error("Invalid region in client config");
                                 return [4, e.regionInfoProvider(r)];
                             case 2:
                                 if (!(o = (null !== (i = a.sent()) && void 0 !== i ? i : {}).hostname)) throw new Error("Cannot resolve hostname from client config");
                                 return [2, e.urlParser((n ? "https:" : "http:") + "//" + o)]
                         }
                     }))
                 }))
             },
-            Rd = function(e) {
+            Fd = function(e) {
                 if ("string" === typeof e) {
                     var t = Promise.resolve(e);
                     return function() {
                         return t
                     }
                 }
                 return e
             };
-        var Bd = function() {
-            return Bd = Object.assign || function(e) {
+        var Yd = function() {
+            return Yd = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, Bd.apply(this, arguments)
+            }, Yd.apply(this, arguments)
         };
 
-        function Fd(e, t, n, r) {
+        function Qd(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -63953,15 +63981,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function Yd(e, t) {
+        function Gd(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -64028,46 +64056,46 @@
                             value: i[0] ? i[1] : void 0,
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
-        var Qd = "content-length";
-        var Gd = {
+        var Wd = "content-length";
+        var Hd = {
                 step: "build",
                 tags: ["SET_CONTENT_LENGTH", "CONTENT_LENGTH"],
                 name: "contentLengthMiddleware",
                 override: !0
             },
-            Wd = function(e) {
+            Zd = function(e) {
                 return {
                     applyToStack: function(t) {
                         t.add(function(e) {
                             var t = this;
                             return function(n) {
                                 return function(r) {
-                                    return Fd(t, void 0, void 0, (function() {
+                                    return Qd(t, void 0, void 0, (function() {
                                         var t, o, i, a, s;
-                                        return Yd(this, (function(u) {
-                                            return t = r.request, kl.isInstance(t) && (o = t.body, i = t.headers, o && -1 === Object.keys(i).map((function(e) {
+                                        return Gd(this, (function(u) {
+                                            return t = r.request, El.isInstance(t) && (o = t.body, i = t.headers, o && -1 === Object.keys(i).map((function(e) {
                                                 return e.toLowerCase()
-                                            })).indexOf(Qd) && void 0 !== (a = e(o)) && (t.headers = Bd(Bd({}, t.headers), ((s = {})["content-length"] = String(a), s)))), [2, n(Bd(Bd({}, r), {
+                                            })).indexOf(Wd) && void 0 !== (a = e(o)) && (t.headers = Yd(Yd({}, t.headers), ((s = {})["content-length"] = String(a), s)))), [2, n(Yd(Yd({}, r), {
                                                 request: t
                                             }))]
                                         }))
                                     }))
                                 }
                             }
-                        }(e.bodyLengthChecker), Gd)
+                        }(e.bodyLengthChecker), Hd)
                     }
                 }
             };
 
-        function Hd(e, t, n, r) {
+        function Vd(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -64087,15 +64115,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function Zd(e, t) {
+        function qd(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -64162,41 +64190,41 @@
                             value: i[0] ? i[1] : void 0,
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
-        var Vd = {
+        var Jd = {
                 name: "hostHeaderMiddleware",
                 step: "build",
                 priority: "low",
                 tags: ["HOST"],
                 override: !0
             },
-            qd = function(e) {
+            Kd = function(e) {
                 return {
                     applyToStack: function(t) {
                         t.add(function(e) {
                             return function(t) {
                                 return function(n) {
-                                    return Hd(void 0, void 0, void 0, (function() {
+                                    return Vd(void 0, void 0, void 0, (function() {
                                         var r, o;
-                                        return Zd(this, (function(i) {
-                                            return kl.isInstance(n.request) ? (r = n.request, (void 0 === (o = (e.requestHandler.metadata || {}).handlerProtocol) ? "" : o).indexOf("h2") >= 0 && !r.headers[":authority"] ? (delete r.headers.host, r.headers[":authority"] = "") : r.headers.host || (r.headers.host = r.hostname), [2, t(n)]) : [2, t(n)]
+                                        return qd(this, (function(i) {
+                                            return El.isInstance(n.request) ? (r = n.request, (void 0 === (o = (e.requestHandler.metadata || {}).handlerProtocol) ? "" : o).indexOf("h2") >= 0 && !r.headers[":authority"] ? (delete r.headers.host, r.headers[":authority"] = "") : r.headers.host || (r.headers.host = r.hostname), [2, t(n)]) : [2, t(n)]
                                         }))
                                     }))
                                 }
                             }
-                        }(e), Vd)
+                        }(e), Jd)
                     }
                 }
             };
 
-        function Jd(e, t, n, r) {
+        function Xd(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -64216,15 +64244,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function Kd(e, t) {
+        function $d(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -64291,20 +64319,20 @@
                             value: i[0] ? i[1] : void 0,
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
-        var Xd = function() {
+        var ef = function() {
                 return function(e, t) {
                     return function(n) {
-                        return Jd(void 0, void 0, void 0, (function() {
+                        return Xd(void 0, void 0, void 0, (function() {
                             var r, o, i, a, s, u, l, c, d;
-                            return Kd(this, (function(f) {
+                            return $d(this, (function(f) {
                                 switch (f.label) {
                                     case 0:
                                         return r = t.clientName, o = t.commandName, i = t.inputFilterSensitiveLog, a = t.logger, s = t.outputFilterSensitiveLog, [4, e(n)];
                                     case 1:
                                         return u = f.sent(), a ? ("function" === typeof a.info && (l = u.output, c = l.$metadata, d = function(e, t) {
                                             var n = {};
                                             for (var r in e) Object.prototype.hasOwnProperty.call(e, r) && t.indexOf(r) < 0 && (n[r] = e[r]);
@@ -64322,29 +64350,29 @@
                                         })), [2, u]) : [2, u]
                                 }
                             }))
                         }))
                     }
                 }
             },
-            $d = {
+            tf = {
                 name: "loggerMiddleware",
                 tags: ["LOGGER"],
                 step: "initialize",
                 override: !0
             };
-        var ef = function() {
-            return ef = Object.assign || function(e) {
+        var nf = function() {
+            return nf = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, ef.apply(this, arguments)
+            }, nf.apply(this, arguments)
         };
 
-        function tf(e, t, n, r) {
+        function rf(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -64364,15 +64392,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function nf(e, t) {
+        function of(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -64440,15 +64468,15 @@
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
 
-        function rf(e, t) {
+        function af(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -64461,23 +64489,23 @@
                     r && !r.done && (n = i.return) && n.call(i)
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
-        var of = function() {
-            return of = Object.assign || function(e) {
+        var sf = function() {
+            return sf = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, of.apply(this, arguments)
+            }, sf.apply(this, arguments)
         };
 
-        function af(e, t, n, r) {
+        function uf(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -64497,15 +64525,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function sf(e, t) {
+        function lf(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -64573,15 +64601,15 @@
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
 
-        function uf(e) {
+        function cf(e) {
             var t = "function" === typeof Symbol && Symbol.iterator,
                 n = t && e[t],
                 r = 0;
             if (n) return n.call(e);
             if (e && "number" === typeof e.length) return {
                 next: function() {
                     return e && r >= e.length && (e = void 0), {
@@ -64589,15 +64617,15 @@
                         done: !e
                     }
                 }
             };
             throw new TypeError(t ? "Object is not iterable." : "Symbol.iterator is not defined.")
         }
 
-        function lf(e, t) {
+        function df(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -64610,33 +64638,33 @@
                     r && !r.done && (n = i.return) && n.call(i)
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
-        for (var cf = {}, df = {}, ff = 0; ff < 256; ff++) {
-            var pf = ff.toString(16).toLowerCase();
-            1 === pf.length && (pf = "0" + pf), cf[ff] = pf, df[pf] = ff
+        for (var ff = {}, pf = {}, hf = 0; hf < 256; hf++) {
+            var gf = hf.toString(16).toLowerCase();
+            1 === gf.length && (gf = "0" + gf), ff[hf] = gf, pf[gf] = hf
         }
 
-        function hf(e) {
-            for (var t = "", n = 0; n < e.byteLength; n++) t += cf[e[n]];
+        function yf(e) {
+            for (var t = "", n = 0; n < e.byteLength; n++) t += ff[e[n]];
             return t
         }
-        var gf = "X-Amz-Date",
-            yf = "X-Amz-Signature",
-            mf = "X-Amz-Security-Token",
-            vf = "authorization",
-            Mf = gf.toLowerCase(),
-            bf = [vf, Mf, "date"],
-            jf = yf.toLowerCase(),
-            wf = "x-amz-content-sha256",
-            xf = mf.toLowerCase(),
-            Nf = {
+        var mf = "X-Amz-Date",
+            vf = "X-Amz-Signature",
+            Mf = "X-Amz-Security-Token",
+            bf = "authorization",
+            jf = mf.toLowerCase(),
+            wf = [bf, jf, "date"],
+            xf = vf.toLowerCase(),
+            Nf = "x-amz-content-sha256",
+            If = Mf.toLowerCase(),
+            Df = {
                 authorization: !0,
                 "cache-control": !0,
                 connection: !0,
                 expect: !0,
                 from: !0,
                 "keep-alive": !0,
                 "max-forwards": !0,
@@ -64645,39 +64673,39 @@
                 te: !0,
                 trailer: !0,
                 "transfer-encoding": !0,
                 upgrade: !0,
                 "user-agent": !0,
                 "x-amzn-trace-id": !0
             },
-            If = /^proxy-/,
-            Df = /^sec-/,
-            Sf = "AWS4-HMAC-SHA256",
-            Lf = "AWS4-HMAC-SHA256-PAYLOAD",
-            kf = "aws4_request",
-            Cf = {},
-            Ef = [];
+            Sf = /^proxy-/,
+            Lf = /^sec-/,
+            kf = "AWS4-HMAC-SHA256",
+            Cf = "AWS4-HMAC-SHA256-PAYLOAD",
+            Ef = "aws4_request",
+            _f = {},
+            Tf = [];
 
-        function _f(e, t, n) {
-            return e + "/" + t + "/" + n + "/" + kf
+        function Af(e, t, n) {
+            return e + "/" + t + "/" + n + "/" + Ef
         }
 
-        function Tf(e, t, n) {
+        function Of(e, t, n) {
             var r = new e(t);
             return r.update(n), r.digest()
         }
 
-        function Af(e, t, n) {
+        function zf(e, t, n) {
             var r, o, i = e.headers,
                 a = {};
             try {
-                for (var s = uf(Object.keys(i).sort()), u = s.next(); !u.done; u = s.next()) {
+                for (var s = cf(Object.keys(i).sort()), u = s.next(); !u.done; u = s.next()) {
                     var l = u.value,
                         c = l.toLowerCase();
-                    (c in Nf || (null === t || void 0 === t ? void 0 : t.has(c)) || If.test(c) || Df.test(c)) && (!n || n && !n.has(c)) || (a[c] = i[l].trim().replace(/\s+/g, " "))
+                    (c in Df || (null === t || void 0 === t ? void 0 : t.has(c)) || Sf.test(c) || Lf.test(c)) && (!n || n && !n.has(c)) || (a[c] = i[l].trim().replace(/\s+/g, " "))
                 }
             } catch (d) {
                 r = {
                     error: d
                 }
             } finally {
                 try {
@@ -64685,84 +64713,84 @@
                 } finally {
                     if (r) throw r.error
                 }
             }
             return a
         }
 
-        function Of(e, t) {
+        function Uf(e, t) {
             var n = e.headers,
                 r = e.body;
-            return af(this, void 0, void 0, (function() {
+            return uf(this, void 0, void 0, (function() {
                 var e, o, i, a, s, u, l;
-                return sf(this, (function(c) {
+                return lf(this, (function(c) {
                     switch (c.label) {
                         case 0:
                             try {
-                                for (e = uf(Object.keys(n)), o = e.next(); !o.done; o = e.next())
-                                    if ((i = o.value).toLowerCase() === wf) return [2, n[i]]
+                                for (e = cf(Object.keys(n)), o = e.next(); !o.done; o = e.next())
+                                    if ((i = o.value).toLowerCase() === Nf) return [2, n[i]]
                             } catch (f) {
                                 u = {
                                     error: f
                                 }
                             } finally {
                                 try {
                                     o && !o.done && (l = e.return) && l.call(e)
                                 } finally {
                                     if (u) throw u.error
                                 }
                             }
                             return void 0 != r ? [3, 1] : [2, "e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855"];
                         case 1:
-                            return "string" === typeof r || ArrayBuffer.isView(r) || (d = r, "function" === typeof ArrayBuffer && d instanceof ArrayBuffer || "[object ArrayBuffer]" === Object.prototype.toString.call(d)) ? ((a = new t).update(r), s = hf, [4, a.digest()]) : [3, 3];
+                            return "string" === typeof r || ArrayBuffer.isView(r) || (d = r, "function" === typeof ArrayBuffer && d instanceof ArrayBuffer || "[object ArrayBuffer]" === Object.prototype.toString.call(d)) ? ((a = new t).update(r), s = yf, [4, a.digest()]) : [3, 3];
                         case 2:
                             return [2, s.apply(void 0, [c.sent()])];
                         case 3:
                             return [2, "UNSIGNED-PAYLOAD"]
                     }
                     var d
                 }))
             }))
         }
 
-        function zf(e) {
+        function Pf(e) {
             var t = e.headers,
                 n = e.query,
                 r = function(e, t) {
                     var n = {};
                     for (var r in e) Object.prototype.hasOwnProperty.call(e, r) && t.indexOf(r) < 0 && (n[r] = e[r]);
                     if (null != e && "function" === typeof Object.getOwnPropertySymbols) {
                         var o = 0;
                         for (r = Object.getOwnPropertySymbols(e); o < r.length; o++) t.indexOf(r[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, r[o]) && (n[r[o]] = e[r[o]])
                     }
                     return n
                 }(e, ["headers", "query"]);
-            return of(of({}, r), {
-                headers: of({}, t),
-                query: n ? Uf(n) : void 0
+            return sf(sf({}, r), {
+                headers: sf({}, t),
+                query: n ? Rf(n) : void 0
             })
         }
 
-        function Uf(e) {
+        function Rf(e) {
             return Object.keys(e).reduce((function(t, n) {
                 var r, o = e[n];
-                return of(of({}, t), ((r = {})[n] = Array.isArray(o) ? function() {
-                    for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(lf(arguments[t]));
+                return sf(sf({}, t), ((r = {})[n] = Array.isArray(o) ? function() {
+                    for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(df(arguments[t]));
                     return e
                 }(o) : o, r))
             }), {})
         }
 
-        function Pf(e) {
+        function Bf(e) {
             var t, n;
-            e = "function" === typeof e.clone ? e.clone() : zf(e);
+            e = "function" === typeof e.clone ? e.clone() : Pf(e);
             try {
-                for (var r = uf(Object.keys(e.headers)), o = r.next(); !o.done; o = r.next()) {
+                for (var r = cf(Object.keys(e.headers)), o = r.next(); !o.done; o = r.next()) {
                     var i = o.value;
-                    bf.indexOf(i.toLowerCase()) > -1 && delete e.headers[i]
+                    wf.indexOf(i.toLowerCase()) > -1 && delete e.headers[i]
                 }
             } catch (a) {
                 t = {
                     error: a
                 }
             } finally {
                 try {
@@ -64770,55 +64798,55 @@
                 } finally {
                     if (t) throw t.error
                 }
             }
             return e
         }
 
-        function Rf(e) {
+        function Ff(e) {
             return function(e) {
                 if ("number" === typeof e) return new Date(1e3 * e);
                 if ("string" === typeof e) return Number(e) ? new Date(1e3 * Number(e)) : new Date(e);
                 return e
             }(e).toISOString().replace(/\.\d{3}Z$/, "Z")
         }
-        var Bf = function() {
+        var Yf = function() {
                 function e(e) {
                     var t = e.applyChecksum,
                         n = e.credentials,
                         r = e.region,
                         o = e.service,
                         i = e.sha256,
                         a = e.uriEscapePath,
                         s = void 0 === a || a;
-                    this.service = o, this.sha256 = i, this.uriEscapePath = s, this.applyChecksum = "boolean" !== typeof t || t, this.regionProvider = Qf(r), this.credentialProvider = Gf(n)
+                    this.service = o, this.sha256 = i, this.uriEscapePath = s, this.applyChecksum = "boolean" !== typeof t || t, this.regionProvider = Wf(r), this.credentialProvider = Hf(n)
                 }
                 return e.prototype.presign = function(e, t) {
-                    return void 0 === t && (t = {}), af(this, void 0, void 0, (function() {
+                    return void 0 === t && (t = {}), uf(this, void 0, void 0, (function() {
                         var n, r, o, i, a, s, u, l, c, d, f, p, h, g, y, m, v, M, b, j, w, x, N, I;
-                        return sf(this, (function(D) {
+                        return lf(this, (function(D) {
                             switch (D.label) {
                                 case 0:
                                     return n = t.signingDate, r = void 0 === n ? new Date : n, o = t.expiresIn, i = void 0 === o ? 3600 : o, a = t.unsignableHeaders, s = t.unhoistableHeaders, u = t.signableHeaders, l = t.signingRegion, c = t.signingService, [4, this.credentialProvider()];
                                 case 1:
                                     return d = D.sent(), null === l || void 0 === l ? [3, 2] : (p = l, [3, 4]);
                                 case 2:
                                     return [4, this.regionProvider()];
                                 case 3:
                                     p = D.sent(), D.label = 4;
                                 case 4:
-                                    return f = p, h = Ff(r), g = h.longDate, y = h.shortDate, i > 604800 ? [2, Promise.reject("Signature version 4 presigned URLs must have an expiration date less than one week in the future")] : (m = _f(y, f, null !== c && void 0 !== c ? c : this.service), v = function(e, t) {
+                                    return f = p, h = Qf(r), g = h.longDate, y = h.shortDate, i > 604800 ? [2, Promise.reject("Signature version 4 presigned URLs must have an expiration date less than one week in the future")] : (m = Af(y, f, null !== c && void 0 !== c ? c : this.service), v = function(e, t) {
                                         var n, r, o;
                                         void 0 === t && (t = {});
-                                        var i = "function" === typeof e.clone ? e.clone() : zf(e),
+                                        var i = "function" === typeof e.clone ? e.clone() : Pf(e),
                                             a = i.headers,
                                             s = i.query,
                                             u = void 0 === s ? {} : s;
                                         try {
-                                            for (var l = uf(Object.keys(a)), c = l.next(); !c.done; c = l.next()) {
+                                            for (var l = cf(Object.keys(a)), c = l.next(); !c.done; c = l.next()) {
                                                 var d = c.value,
                                                     f = d.toLowerCase();
                                                 "x-amz-" !== f.substr(0, 6) || (null === (o = t.unhoistableHeaders) || void 0 === o ? void 0 : o.has(f)) || (u[d] = a[d], delete a[d])
                                             }
                                         } catch (p) {
                                             n = {
                                                 error: p
@@ -64826,159 +64854,159 @@
                                         } finally {
                                             try {
                                                 c && !c.done && (r = l.return) && r.call(l)
                                             } finally {
                                                 if (n) throw n.error
                                             }
                                         }
-                                        return of(of({}, e), {
+                                        return sf(sf({}, e), {
                                             headers: a,
                                             query: u
                                         })
-                                    }(Pf(e), {
+                                    }(Bf(e), {
                                         unhoistableHeaders: s
-                                    }), d.sessionToken && (v.query[mf] = d.sessionToken), v.query["X-Amz-Algorithm"] = Sf, v.query["X-Amz-Credential"] = d.accessKeyId + "/" + m, v.query["X-Amz-Date"] = g, v.query["X-Amz-Expires"] = i.toString(10), M = Af(v, a, u), v.query["X-Amz-SignedHeaders"] = Yf(M), b = v.query, j = yf, w = this.getSignature, x = [g, m, this.getSigningKey(d, f, y, c)], N = this.createCanonicalRequest, I = [v, M], [4, Of(e, this.sha256)]);
+                                    }), d.sessionToken && (v.query[Mf] = d.sessionToken), v.query["X-Amz-Algorithm"] = kf, v.query["X-Amz-Credential"] = d.accessKeyId + "/" + m, v.query["X-Amz-Date"] = g, v.query["X-Amz-Expires"] = i.toString(10), M = zf(v, a, u), v.query["X-Amz-SignedHeaders"] = Gf(M), b = v.query, j = vf, w = this.getSignature, x = [g, m, this.getSigningKey(d, f, y, c)], N = this.createCanonicalRequest, I = [v, M], [4, Uf(e, this.sha256)]);
                                 case 5:
                                     return [4, w.apply(this, x.concat([N.apply(this, I.concat([D.sent()]))]))];
                                 case 6:
                                     return b[j] = D.sent(), [2, v]
                             }
                         }))
                     }))
                 }, e.prototype.sign = function(e, t) {
-                    return af(this, void 0, void 0, (function() {
-                        return sf(this, (function(n) {
+                    return uf(this, void 0, void 0, (function() {
+                        return lf(this, (function(n) {
                             return "string" === typeof e ? [2, this.signString(e, t)] : e.headers && e.payload ? [2, this.signEvent(e, t)] : [2, this.signRequest(e, t)]
                         }))
                     }))
                 }, e.prototype.signEvent = function(e, t) {
                     var n = e.headers,
                         r = e.payload,
                         o = t.signingDate,
                         i = void 0 === o ? new Date : o,
                         a = t.priorSignature,
                         s = t.signingRegion,
                         u = t.signingService;
-                    return af(this, void 0, void 0, (function() {
+                    return uf(this, void 0, void 0, (function() {
                         var e, t, o, l, c, d, f, p, h, g, y;
-                        return sf(this, (function(m) {
+                        return lf(this, (function(m) {
                             switch (m.label) {
                                 case 0:
                                     return null === s || void 0 === s ? [3, 1] : (t = s, [3, 3]);
                                 case 1:
                                     return [4, this.regionProvider()];
                                 case 2:
                                     t = m.sent(), m.label = 3;
                                 case 3:
-                                    return e = t, o = Ff(i), l = o.shortDate, c = o.longDate, d = _f(l, e, null !== u && void 0 !== u ? u : this.service), [4, Of({
+                                    return e = t, o = Qf(i), l = o.shortDate, c = o.longDate, d = Af(l, e, null !== u && void 0 !== u ? u : this.service), [4, Uf({
                                         headers: {},
                                         body: r
                                     }, this.sha256)];
                                 case 4:
-                                    return f = m.sent(), (p = new this.sha256).update(n), g = hf, [4, p.digest()];
+                                    return f = m.sent(), (p = new this.sha256).update(n), g = yf, [4, p.digest()];
                                 case 5:
-                                    return h = g.apply(void 0, [m.sent()]), y = [Lf, c, d, a, h, f].join("\n"), [2, this.signString(y, {
+                                    return h = g.apply(void 0, [m.sent()]), y = [Cf, c, d, a, h, f].join("\n"), [2, this.signString(y, {
                                         signingDate: i,
                                         signingRegion: e,
                                         signingService: u
                                     })]
                             }
                         }))
                     }))
                 }, e.prototype.signString = function(e, t) {
                     var n = void 0 === t ? {} : t,
                         r = n.signingDate,
                         o = void 0 === r ? new Date : r,
                         i = n.signingRegion,
                         a = n.signingService;
-                    return af(this, void 0, void 0, (function() {
+                    return uf(this, void 0, void 0, (function() {
                         var t, n, r, s, u, l, c, d;
-                        return sf(this, (function(f) {
+                        return lf(this, (function(f) {
                             switch (f.label) {
                                 case 0:
                                     return [4, this.credentialProvider()];
                                 case 1:
                                     return t = f.sent(), null === i || void 0 === i ? [3, 2] : (r = i, [3, 4]);
                                 case 2:
                                     return [4, this.regionProvider()];
                                 case 3:
                                     r = f.sent(), f.label = 4;
                                 case 4:
-                                    return n = r, s = Ff(o).shortDate, c = (l = this.sha256).bind, [4, this.getSigningKey(t, n, s, a)];
+                                    return n = r, s = Qf(o).shortDate, c = (l = this.sha256).bind, [4, this.getSigningKey(t, n, s, a)];
                                 case 5:
-                                    return (u = new(c.apply(l, [void 0, f.sent()]))).update(e), d = hf, [4, u.digest()];
+                                    return (u = new(c.apply(l, [void 0, f.sent()]))).update(e), d = yf, [4, u.digest()];
                                 case 6:
                                     return [2, d.apply(void 0, [f.sent()])]
                             }
                         }))
                     }))
                 }, e.prototype.signRequest = function(e, t) {
                     var n = void 0 === t ? {} : t,
                         r = n.signingDate,
                         o = void 0 === r ? new Date : r,
                         i = n.signableHeaders,
                         a = n.unsignableHeaders,
                         s = n.signingRegion,
                         u = n.signingService;
-                    return af(this, void 0, void 0, (function() {
+                    return uf(this, void 0, void 0, (function() {
                         var t, n, r, l, c, d, f, p, h, g, y;
-                        return sf(this, (function(m) {
+                        return lf(this, (function(m) {
                             switch (m.label) {
                                 case 0:
                                     return [4, this.credentialProvider()];
                                 case 1:
                                     return t = m.sent(), null === s || void 0 === s ? [3, 2] : (r = s, [3, 4]);
                                 case 2:
                                     return [4, this.regionProvider()];
                                 case 3:
                                     r = m.sent(), m.label = 4;
                                 case 4:
-                                    return n = r, l = Pf(e), c = Ff(o), d = c.longDate, f = c.shortDate, p = _f(f, n, null !== u && void 0 !== u ? u : this.service), l.headers[Mf] = d, t.sessionToken && (l.headers[xf] = t.sessionToken), [4, Of(l, this.sha256)];
+                                    return n = r, l = Bf(e), c = Qf(o), d = c.longDate, f = c.shortDate, p = Af(f, n, null !== u && void 0 !== u ? u : this.service), l.headers[jf] = d, t.sessionToken && (l.headers[If] = t.sessionToken), [4, Uf(l, this.sha256)];
                                 case 5:
                                     return h = m.sent(), ! function(e, t) {
                                         var n, r;
                                         e = e.toLowerCase();
                                         try {
-                                            for (var o = uf(Object.keys(t)), i = o.next(); !i.done; i = o.next())
+                                            for (var o = cf(Object.keys(t)), i = o.next(); !i.done; i = o.next())
                                                 if (e === i.value.toLowerCase()) return !0
                                         } catch (a) {
                                             n = {
                                                 error: a
                                             }
                                         } finally {
                                             try {
                                                 i && !i.done && (r = o.return) && r.call(o)
                                             } finally {
                                                 if (n) throw n.error
                                             }
                                         }
                                         return !1
-                                    }(wf, l.headers) && this.applyChecksum && (l.headers[wf] = h), g = Af(l, a, i), [4, this.getSignature(d, p, this.getSigningKey(t, n, f, u), this.createCanonicalRequest(l, g, h))];
+                                    }(Nf, l.headers) && this.applyChecksum && (l.headers[Nf] = h), g = zf(l, a, i), [4, this.getSignature(d, p, this.getSigningKey(t, n, f, u), this.createCanonicalRequest(l, g, h))];
                                 case 6:
-                                    return y = m.sent(), l.headers[vf] = "AWS4-HMAC-SHA256 Credential=" + t.accessKeyId + "/" + p + ", SignedHeaders=" + Yf(g) + ", Signature=" + y, [2, l]
+                                    return y = m.sent(), l.headers[bf] = "AWS4-HMAC-SHA256 Credential=" + t.accessKeyId + "/" + p + ", SignedHeaders=" + Gf(g) + ", Signature=" + y, [2, l]
                             }
                         }))
                     }))
                 }, e.prototype.createCanonicalRequest = function(e, t, n) {
                     var r = Object.keys(t).sort();
                     return e.method + "\n" + this.getCanonicalPath(e) + "\n" + function(e) {
                         var t, n, r = e.query,
                             o = void 0 === r ? {} : r,
                             i = [],
                             a = {},
                             s = function(e) {
-                                if (e.toLowerCase() === jf) return "continue";
+                                if (e.toLowerCase() === xf) return "continue";
                                 i.push(e);
                                 var t = o[e];
-                                "string" === typeof t ? a[e] = Qc(e) + "=" + Qc(t) : Array.isArray(t) && (a[e] = t.slice(0).sort().reduce((function(t, n) {
-                                    return t.concat([Qc(e) + "=" + Qc(n)])
+                                "string" === typeof t ? a[e] = Wc(e) + "=" + Wc(t) : Array.isArray(t) && (a[e] = t.slice(0).sort().reduce((function(t, n) {
+                                    return t.concat([Wc(e) + "=" + Wc(n)])
                                 }), []).join("&"))
                             };
                         try {
-                            for (var u = uf(Object.keys(o).sort()), l = u.next(); !l.done; l = u.next()) s(l.value)
+                            for (var u = cf(Object.keys(o).sort()), l = u.next(); !l.done; l = u.next()) s(l.value)
                         } catch (c) {
                             t = {
                                 error: c
                             }
                         } finally {
                             try {
                                 l && !l.done && (n = u.return) && n.call(u)
@@ -64991,60 +65019,60 @@
                         })).filter((function(e) {
                             return e
                         })).join("&")
                     }(e) + "\n" + r.map((function(e) {
                         return e + ":" + t[e]
                     })).join("\n") + "\n\n" + r.join(";") + "\n" + n
                 }, e.prototype.createStringToSign = function(e, t, n) {
-                    return af(this, void 0, void 0, (function() {
+                    return uf(this, void 0, void 0, (function() {
                         var r, o;
-                        return sf(this, (function(i) {
+                        return lf(this, (function(i) {
                             switch (i.label) {
                                 case 0:
                                     return (r = new this.sha256).update(n), [4, r.digest()];
                                 case 1:
-                                    return o = i.sent(), [2, "AWS4-HMAC-SHA256\n" + e + "\n" + t + "\n" + hf(o)]
+                                    return o = i.sent(), [2, "AWS4-HMAC-SHA256\n" + e + "\n" + t + "\n" + yf(o)]
                             }
                         }))
                     }))
                 }, e.prototype.getCanonicalPath = function(e) {
                     var t = e.path;
                     return this.uriEscapePath ? "/" + encodeURIComponent(t.replace(/^\//, "")).replace(/%2F/g, "/") : t
                 }, e.prototype.getSignature = function(e, t, n, r) {
-                    return af(this, void 0, void 0, (function() {
+                    return uf(this, void 0, void 0, (function() {
                         var o, i, a, s, u;
-                        return sf(this, (function(l) {
+                        return lf(this, (function(l) {
                             switch (l.label) {
                                 case 0:
                                     return [4, this.createStringToSign(e, t, r)];
                                 case 1:
                                     return o = l.sent(), s = (a = this.sha256).bind, [4, n];
                                 case 2:
-                                    return (i = new(s.apply(a, [void 0, l.sent()]))).update(o), u = hf, [4, i.digest()];
+                                    return (i = new(s.apply(a, [void 0, l.sent()]))).update(o), u = yf, [4, i.digest()];
                                 case 3:
                                     return [2, u.apply(void 0, [l.sent()])]
                             }
                         }))
                     }))
                 }, e.prototype.getSigningKey = function(e, t, n, r) {
                     return function(e, t, n, r, o) {
-                        return af(void 0, void 0, void 0, (function() {
+                        return uf(void 0, void 0, void 0, (function() {
                             var i, a, s, u, l, c, d, f, p;
-                            return sf(this, (function(h) {
+                            return lf(this, (function(h) {
                                 switch (h.label) {
                                     case 0:
-                                        return [4, Tf(e, t.secretAccessKey, t.accessKeyId)];
+                                        return [4, Of(e, t.secretAccessKey, t.accessKeyId)];
                                     case 1:
-                                        if (i = h.sent(), (a = n + ":" + r + ":" + o + ":" + hf(i) + ":" + t.sessionToken) in Cf) return [2, Cf[a]];
-                                        for (Ef.push(a); Ef.length > 50;) delete Cf[Ef.shift()];
+                                        if (i = h.sent(), (a = n + ":" + r + ":" + o + ":" + yf(i) + ":" + t.sessionToken) in _f) return [2, _f[a]];
+                                        for (Tf.push(a); Tf.length > 50;) delete _f[Tf.shift()];
                                         s = "AWS4" + t.secretAccessKey, h.label = 2;
                                     case 2:
-                                        h.trys.push([2, 7, 8, 9]), u = uf([n, r, o, kf]), l = u.next(), h.label = 3;
+                                        h.trys.push([2, 7, 8, 9]), u = cf([n, r, o, Ef]), l = u.next(), h.label = 3;
                                     case 3:
-                                        return l.done ? [3, 6] : (c = l.value, [4, Tf(e, s, c)]);
+                                        return l.done ? [3, 6] : (c = l.value, [4, Of(e, s, c)]);
                                     case 4:
                                         s = h.sent(), h.label = 5;
                                     case 5:
                                         return l = u.next(), [3, 3];
                                     case 6:
                                         return [3, 9];
                                     case 7:
@@ -65055,68 +65083,68 @@
                                         try {
                                             l && !l.done && (p = u.return) && p.call(u)
                                         } finally {
                                             if (f) throw f.error
                                         }
                                         return [7];
                                     case 9:
-                                        return [2, Cf[a] = s]
+                                        return [2, _f[a] = s]
                                 }
                             }))
                         }))
                     }(this.sha256, e, n, t, r || this.service)
                 }, e
             }(),
-            Ff = function(e) {
-                var t = Rf(e).replace(/[\-:]/g, "");
+            Qf = function(e) {
+                var t = Ff(e).replace(/[\-:]/g, "");
                 return {
                     longDate: t,
                     shortDate: t.substr(0, 8)
                 }
             },
-            Yf = function(e) {
+            Gf = function(e) {
                 return Object.keys(e).sort().join(";")
             },
-            Qf = function(e) {
+            Wf = function(e) {
                 if ("string" === typeof e) {
                     var t = Promise.resolve(e);
                     return function() {
                         return t
                     }
                 }
                 return e
             },
-            Gf = function(e) {
+            Hf = function(e) {
                 if ("object" === typeof e) {
                     var t = Promise.resolve(e);
                     return function() {
                         return t
                     }
                 }
                 return e
             };
 
-        function Wf(e) {
+        function Zf(e) {
             if ("object" === typeof e) {
                 var t = Promise.resolve(e);
                 return function() {
                     return t
                 }
             }
             return e
         }
-        var Hf = function() {
-            return Hf = Object.assign || function(e) {
+        var Vf = function() {
+            return Vf = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, Hf.apply(this, arguments)
+            }, Vf.apply(this, arguments)
         };
 
-        function Zf(e, t, n, r) {
+        function qf(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -65136,15 +65164,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function Vf(e, t) {
+        function Jf(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -65212,15 +65240,15 @@
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
 
-        function qf(e, t) {
+        function Kf(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -65234,213 +65262,213 @@
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
 
-        function Jf() {
-            for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(qf(arguments[t]));
+        function Xf() {
+            for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(Kf(arguments[t]));
             return e
         }
-        var Kf = "user-agent",
-            Xf = /[^\!\#\$\%\&\'\*\+\-\.\^\_\`\|\~\d\w]/g,
-            $f = function(e) {
-                var t = qf(e, 2),
+        var $f = "user-agent",
+            ep = /[^\!\#\$\%\&\'\*\+\-\.\^\_\`\|\~\d\w]/g,
+            tp = function(e) {
+                var t = Kf(e, 2),
                     n = t[0],
                     r = t[1],
                     o = n.indexOf("/"),
                     i = n.substring(0, o),
                     a = n.substring(o + 1);
                 return "api" === i && (a = a.toLowerCase()), [i, a, r].filter((function(e) {
                     return e && e.length > 0
                 })).map((function(e) {
-                    return null === e || void 0 === e ? void 0 : e.replace(Xf, "_")
+                    return null === e || void 0 === e ? void 0 : e.replace(ep, "_")
                 })).join("/")
             },
-            ep = {
+            np = {
                 name: "getUserAgentMiddleware",
                 step: "build",
                 priority: "low",
                 tags: ["SET_USER_AGENT", "USER_AGENT"],
                 override: !0
             },
-            tp = function(e) {
+            rp = function(e) {
                 return {
                     applyToStack: function(t) {
                         var n;
                         t.add((n = e, function(e, t) {
                             return function(r) {
-                                return Zf(void 0, void 0, void 0, (function() {
+                                return qf(void 0, void 0, void 0, (function() {
                                     var o, i, a, s, u, l, c, d;
-                                    return Vf(this, (function(f) {
+                                    return Jf(this, (function(f) {
                                         switch (f.label) {
                                             case 0:
-                                                return o = r.request, kl.isInstance(o) ? (i = o.headers, a = (null === (c = null === t || void 0 === t ? void 0 : t.userAgent) || void 0 === c ? void 0 : c.map($f)) || [], [4, n.defaultUserAgentProvider()]) : [2, e(r)];
+                                                return o = r.request, El.isInstance(o) ? (i = o.headers, a = (null === (c = null === t || void 0 === t ? void 0 : t.userAgent) || void 0 === c ? void 0 : c.map(tp)) || [], [4, n.defaultUserAgentProvider()]) : [2, e(r)];
                                             case 1:
-                                                return s = f.sent().map($f), u = (null === (d = null === n || void 0 === n ? void 0 : n.customUserAgent) || void 0 === d ? void 0 : d.map($f)) || [], i["x-amz-user-agent"] = Jf(s, a, u).join(" "), l = Jf(s.filter((function(e) {
+                                                return s = f.sent().map(tp), u = (null === (d = null === n || void 0 === n ? void 0 : n.customUserAgent) || void 0 === d ? void 0 : d.map(tp)) || [], i["x-amz-user-agent"] = Xf(s, a, u).join(" "), l = Xf(s.filter((function(e) {
                                                     return e.startsWith("aws-sdk-")
-                                                })), u).join(" "), "browser" !== n.runtime && l && (i[Kf] = i[Kf] ? i[Kf] + " " + l : l), [2, e(Hf(Hf({}, r), {
+                                                })), u).join(" "), "browser" !== n.runtime && l && (i[$f] = i[$f] ? i[$f] + " " + l : l), [2, e(Vf(Vf({}, r), {
                                                     request: o
                                                 }))]
                                         }
                                     }))
                                 }))
                             }
-                        }), ep)
+                        }), np)
                     }
                 }
             },
-            np = function(e) {
+            op = function(e) {
                 function t(t) {
                     var n, r, o = this,
                         i = function(e) {
                             if (!e.region) throw new Error("Region is missing");
-                            return Ad(Ad({}, e), {
-                                region: Rd(e.region)
+                            return zd(zd({}, e), {
+                                region: Fd(e.region)
                             })
-                        }(Mu(Mu({}, Td), t)),
+                        }(ju(ju({}, Od), t)),
                         a = function(e) {
                             var t;
-                            return Ad(Ad({}, e), {
+                            return zd(zd({}, e), {
                                 tls: null === (t = e.tls) || void 0 === t || t,
-                                endpoint: e.endpoint ? Ud(e) : function() {
-                                    return Pd(e)
+                                endpoint: e.endpoint ? Rd(e) : function() {
+                                    return Bd(e)
                                 },
                                 isCustomEndpoint: !!e.endpoint
                             })
                         }(i),
                         s = function(e) {
                             var t, n = this,
-                                r = Wf(e.credentials || e.credentialDefaultProvider(e)),
+                                r = Zf(e.credentials || e.credentialDefaultProvider(e)),
                                 o = e.signingEscapePath,
                                 i = void 0 === o || o,
                                 a = e.systemClockOffset,
                                 s = void 0 === a ? e.systemClockOffset || 0 : a,
                                 u = e.sha256;
-                            return t = e.signer ? Wf(e.signer) : function() {
-                                return Wf(e.region)().then((function(t) {
-                                    return tf(n, void 0, void 0, (function() {
-                                        return nf(this, (function(n) {
+                            return t = e.signer ? Zf(e.signer) : function() {
+                                return Zf(e.region)().then((function(t) {
+                                    return rf(n, void 0, void 0, (function() {
+                                        return of(this, (function(n) {
                                             switch (n.label) {
                                                 case 0:
                                                     return [4, e.regionInfoProvider(t)];
                                                 case 1:
                                                     return [2, [n.sent() || {}, t]]
                                             }
                                         }))
                                     }))
                                 })).then((function(t) {
-                                    var n = rf(t, 2),
+                                    var n = af(t, 2),
                                         o = n[0],
                                         a = n[1],
                                         s = o.signingRegion,
                                         l = o.signingService;
-                                    return e.signingRegion = e.signingRegion || s || a, e.signingName = e.signingName || l || e.serviceId, new Bf({
+                                    return e.signingRegion = e.signingRegion || s || a, e.signingName = e.signingName || l || e.serviceId, new Yf({
                                         credentials: r,
                                         region: e.signingRegion,
                                         service: e.signingName,
                                         sha256: u,
                                         uriEscapePath: i
                                     })
                                 }))
-                            }, ef(ef({}, e), {
+                            }, nf(nf({}, e), {
                                 systemClockOffset: s,
                                 signingEscapePath: i,
                                 credentials: r,
                                 signer: t
                             })
                         }(a),
                         u = function(e) {
-                            var t = md(e.maxAttempts);
-                            return td(td({}, e), {
+                            var t = Md(e.maxAttempts);
+                            return rd(rd({}, e), {
                                 maxAttempts: t,
-                                retryStrategy: e.retryStrategy || new yd(t)
+                                retryStrategy: e.retryStrategy || new vd(t)
                             })
                         }(s),
-                        l = Hf(Hf({}, n = u), {
+                        l = Vf(Vf({}, n = u), {
                             customUserAgent: "string" === typeof n.customUserAgent ? [
                                 [n.customUserAgent]
                             ] : n.customUserAgent
                         });
                     return (o = e.call(this, l) || this).config = l, o.middlewareStack.use((r = o.config, {
                         applyToStack: function(e) {
-                            e.add(id(r), ad)
+                            e.add(sd(r), ud)
                         }
-                    })), o.middlewareStack.use(Wd(o.config)), o.middlewareStack.use(qd(o.config)), o.middlewareStack.use((o.config, {
+                    })), o.middlewareStack.use(Zd(o.config)), o.middlewareStack.use(Kd(o.config)), o.middlewareStack.use((o.config, {
                         applyToStack: function(e) {
-                            e.add(Xd(), $d)
+                            e.add(ef(), tf)
                         }
-                    })), o.middlewareStack.use(tp(o.config)), o
+                    })), o.middlewareStack.use(rp(o.config)), o
                 }
-                return vu(t, e), t.prototype.destroy = function() {
+                return bu(t, e), t.prototype.destroy = function() {
                     e.prototype.destroy.call(this)
                 }, t
-            }(bc),
-            rp = "aws-amplify/5.0.10",
-            op = {
-                userAgent: rp + " js",
+            }(wc),
+            ip = "aws-amplify/5.0.10",
+            ap = {
+                userAgent: ip + " js",
                 product: "",
                 navigator: null,
                 isReactNative: !1
             };
         if ("undefined" !== typeof navigator && navigator.product)
-            if (op.product = navigator.product || "", op.navigator = navigator || null, "ReactNative" === navigator.product) op.userAgent = rp + " react-native", op.isReactNative = !0;
-            else op.userAgent = rp + " js", op.isReactNative = !1;
+            if (ap.product = navigator.product || "", ap.navigator = navigator || null, "ReactNative" === navigator.product) ap.userAgent = ip + " react-native", ap.isReactNative = !0;
+            else ap.userAgent = ip + " js", ap.isReactNative = !1;
 
-        function ip(e) {
-            var t, n = new np({
+        function sp(e) {
+            var t, n = new op({
                 region: e.region,
-                customUserAgent: "" + op.userAgent + (t || "")
+                customUserAgent: "" + ap.userAgent + (t || "")
             });
             return n.middlewareStack.add((function(e, t) {
                 return function(t) {
                     return e(function(e) {
-                        return Us(Us({}, e), {
-                            request: Us(Us({}, e.request), {
-                                headers: Us(Us({}, e.request.headers), {
+                        return Rs(Rs({}, e), {
+                            request: Rs(Rs({}, e.request), {
+                                headers: Rs(Rs({}, e.request.headers), {
                                     "cache-control": "no-store"
                                 })
                             })
                         })
                     }(t))
                 }
             }), {
                 step: "build",
                 name: "cacheControlMiddleWare"
             }), n
         }
-        var ap = new Ws("Credentials"),
-            sp = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default",
-            up = function() {
+        var up = new Zs("Credentials"),
+            lp = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default",
+            cp = function() {
                 function e(e) {
-                    this._gettingCredPromise = null, this._refreshHandlers = {}, this.Auth = void 0, this.configure(e), this._refreshHandlers.google = cu.refreshGoogleToken, this._refreshHandlers.facebook = du.refreshFacebookToken
+                    this._gettingCredPromise = null, this._refreshHandlers = {}, this.Auth = void 0, this.configure(e), this._refreshHandlers.google = fu.refreshGoogleToken, this._refreshHandlers.facebook = pu.refreshFacebookToken
                 }
                 return e.prototype.getModuleName = function() {
                     return "Credentials"
                 }, e.prototype.getCredSource = function() {
                     return this._credentials_source
                 }, e.prototype.configure = function(e) {
                     if (!e) return this._config || {};
                     this._config = Object.assign({}, this._config, e);
                     var t = this._config.refreshHandlers;
-                    return t && (this._refreshHandlers = Us(Us({}, this._refreshHandlers), t)), this._storage = this._config.storage, this._storage || (this._storage = (new Xs).getStorage()), this._storageSync = Promise.resolve(), "function" === typeof this._storage.sync && (this._storageSync = this._storage.sync()),
+                    return t && (this._refreshHandlers = Rs(Rs({}, this._refreshHandlers), t)), this._storage = this._config.storage, this._storage || (this._storage = (new eu).getStorage()), this._storageSync = Promise.resolve(), "function" === typeof this._storage.sync && (this._storageSync = this._storage.sync()),
                         function(e, t, n) {
-                            qs.dispatch("core", {
+                            Ks.dispatch("core", {
                                 event: e,
                                 data: t,
                                 message: n
-                            }, "Credentials", sp)
+                            }, "Credentials", lp)
                         }("credentials_configured", null, "Credentials has been configured successfully"), this._config
                 }, e.prototype.get = function() {
-                    return ap.debug("getting credentials"), this._pickupCredentials()
+                    return up.debug("getting credentials"), this._pickupCredentials()
                 }, e.prototype._getCognitoIdentityIdStorageKey = function(e) {
                     return "CognitoIdentityId-" + e
                 }, e.prototype._pickupCredentials = function() {
-                    return ap.debug("picking up credentials"), this._gettingCredPromise && this._gettingCredPromise.isPending() ? ap.debug("getting old cred promise") : (ap.debug("getting new cred promise"), this._gettingCredPromise = function(e) {
+                    return up.debug("picking up credentials"), this._gettingCredPromise && this._gettingCredPromise.isPending() ? up.debug("getting old cred promise") : (up.debug("getting new cred promise"), this._gettingCredPromise = function(e) {
                         if (e.isResolved) return e;
                         var t = !0,
                             n = !1,
                             r = !1,
                             o = e.then((function(e) {
                                 return r = !0, t = !1, e
                             }), (function(e) {
@@ -65451,152 +65479,152 @@
                         }, o.isPending = function() {
                             return t
                         }, o.isRejected = function() {
                             return n
                         }, o
                     }(this._keepAlive())), this._gettingCredPromise
                 }, e.prototype._keepAlive = function() {
-                    return Ps(this, void 0, void 0, (function() {
+                    return Bs(this, void 0, void 0, (function() {
                         var e, t, n, r, o, i, a;
-                        return Rs(this, (function(s) {
+                        return Fs(this, (function(s) {
                             switch (s.label) {
                                 case 0:
-                                    if (ap.debug("checking if credentials exists and not expired"), (e = this._credentials) && !this._isExpired(e) && !this._isPastTTL()) return ap.debug("credentials not changed and not expired, directly return"), [2, Promise.resolve(e)];
-                                    if (ap.debug("need to get a new credential or refresh the existing one"), t = this.Auth, !(n = void 0 === t ? pu.Auth : t) || "function" !== typeof n.currentUserCredentials) return [2, this._setCredentialsForGuest()];
+                                    if (up.debug("checking if credentials exists and not expired"), (e = this._credentials) && !this._isExpired(e) && !this._isPastTTL()) return up.debug("credentials not changed and not expired, directly return"), [2, Promise.resolve(e)];
+                                    if (up.debug("need to get a new credential or refresh the existing one"), t = this.Auth, !(n = void 0 === t ? gu.Auth : t) || "function" !== typeof n.currentUserCredentials) return [2, this._setCredentialsForGuest()];
                                     if (this._isExpired(e) || !this._isPastTTL()) return [3, 6];
-                                    ap.debug("ttl has passed but token is not yet expired"), s.label = 1;
+                                    up.debug("ttl has passed but token is not yet expired"), s.label = 1;
                                 case 1:
                                     return s.trys.push([1, 5, , 6]), [4, n.currentUserPoolUser()];
                                 case 2:
                                     return r = s.sent(), [4, n.currentSession()];
                                 case 3:
                                     return o = s.sent(), i = o.refreshToken, [4, new Promise((function(e, t) {
                                         r.refreshSession(i, (function(n, r) {
                                             return n ? t(n) : e(r)
                                         }))
                                     }))];
                                 case 4:
                                     return s.sent(), [3, 6];
                                 case 5:
-                                    return a = s.sent(), ap.debug("Error attempting to refreshing the session", a), [3, 6];
+                                    return a = s.sent(), up.debug("Error attempting to refreshing the session", a), [3, 6];
                                 case 6:
                                     return [2, n.currentUserCredentials()]
                             }
                         }))
                     }))
                 }, e.prototype.refreshFederatedToken = function(e) {
-                    ap.debug("Getting federated credentials");
+                    up.debug("Getting federated credentials");
                     var t = e.provider,
                         n = e.user,
                         r = e.token,
                         o = e.identity_id,
                         i = e.expires_at;
                     i = 1970 === new Date(i).getFullYear() ? 1e3 * i : i;
                     var a = this;
-                    return ap.debug("checking if federated jwt token expired"), i > (new Date).getTime() ? (ap.debug("token not expired"), this._setCredentialsFromFederation({
+                    return up.debug("checking if federated jwt token expired"), i > (new Date).getTime() ? (up.debug("token not expired"), this._setCredentialsFromFederation({
                         provider: t,
                         token: r,
                         user: n,
                         identity_id: o,
                         expires_at: i
-                    })) : a._refreshHandlers[t] && "function" === typeof a._refreshHandlers[t] ? (ap.debug("getting refreshed jwt token from federation provider"), this._providerRefreshWithRetry({
+                    })) : a._refreshHandlers[t] && "function" === typeof a._refreshHandlers[t] ? (up.debug("getting refreshed jwt token from federation provider"), this._providerRefreshWithRetry({
                         refreshHandler: a._refreshHandlers[t],
                         provider: t,
                         user: n
-                    })) : (ap.debug("no refresh handler for provider:", t), this.clear(), Promise.reject("no refresh handler for provider"))
+                    })) : (up.debug("no refresh handler for provider:", t), this.clear(), Promise.reject("no refresh handler for provider"))
                 }, e.prototype._providerRefreshWithRetry = function(e) {
                     var t = this,
                         n = e.refreshHandler,
                         r = e.provider,
                         o = e.user;
-                    return ru(n, [], 1e4).then((function(e) {
-                        return ap.debug("refresh federated token sucessfully", e), t._setCredentialsFromFederation({
+                    return iu(n, [], 1e4).then((function(e) {
+                        return up.debug("refresh federated token sucessfully", e), t._setCredentialsFromFederation({
                             provider: r,
                             token: e.token,
                             user: o,
                             identity_id: e.identity_id,
                             expires_at: e.expires_at
                         })
                     })).catch((function(e) {
-                        return "string" === typeof e && 0 === e.toLowerCase().lastIndexOf("network error", e.length) || t.clear(), ap.debug("refresh federated token failed", e), Promise.reject("refreshing federation token failed: " + e)
+                        return "string" === typeof e && 0 === e.toLowerCase().lastIndexOf("network error", e.length) || t.clear(), up.debug("refresh federated token failed", e), Promise.reject("refreshing federation token failed: " + e)
                     }))
                 }, e.prototype._isExpired = function(e) {
-                    if (!e) return ap.debug("no credentials for expiration check"), !0;
-                    ap.debug("are these credentials expired?", e);
+                    if (!e) return up.debug("no credentials for expiration check"), !0;
+                    up.debug("are these credentials expired?", e);
                     var t = Date.now();
                     return e.expiration.getTime() <= t
                 }, e.prototype._isPastTTL = function() {
                     return this._nextCredentialsRefresh <= Date.now()
                 }, e.prototype._setCredentialsForGuest = function() {
                     var e;
-                    return Ps(this, void 0, void 0, (function() {
+                    return Bs(this, void 0, void 0, (function() {
                         var t, n, r, o, i, a, s, u, l, c, d = this;
-                        return Rs(this, (function(f) {
+                        return Fs(this, (function(f) {
                             switch (f.label) {
                                 case 0:
-                                    return ap.debug("setting credentials for guest"), (null === (e = this._config) || void 0 === e ? void 0 : e.identityPoolId) || (this._config = Object.assign({}, this._config, Uc(this._config || {}).Auth)), t = this._config, n = t.identityPoolId, r = t.region, o = t.mandatorySignIn, i = t.identityPoolRegion, o ? [2, Promise.reject("cannot get guest credentials when mandatory signin enabled")] : n ? i || r ? (s = this, [4, this._getGuestIdentityId()]) : (ap.debug("region is not configured for getting the credentials"), [2, Promise.reject("region is not configured for getting the credentials")]) : (ap.debug("No Cognito Identity pool provided for unauthenticated access"), [2, Promise.reject("No Cognito Identity pool provided for unauthenticated access")]);
+                                    return up.debug("setting credentials for guest"), (null === (e = this._config) || void 0 === e ? void 0 : e.identityPoolId) || (this._config = Object.assign({}, this._config, Rc(this._config || {}).Auth)), t = this._config, n = t.identityPoolId, r = t.region, o = t.mandatorySignIn, i = t.identityPoolRegion, o ? [2, Promise.reject("cannot get guest credentials when mandatory signin enabled")] : n ? i || r ? (s = this, [4, this._getGuestIdentityId()]) : (up.debug("region is not configured for getting the credentials"), [2, Promise.reject("region is not configured for getting the credentials")]) : (up.debug("No Cognito Identity pool provided for unauthenticated access"), [2, Promise.reject("No Cognito Identity pool provided for unauthenticated access")]);
                                 case 1:
-                                    return a = s._identityId = f.sent(), u = ip({
+                                    return a = s._identityId = f.sent(), u = sp({
                                         region: i || r
-                                    }), l = void 0, a ? l = Cc({
+                                    }), l = void 0, a ? l = _c({
                                         identityId: a,
                                         client: u
                                     })() : (c = function() {
-                                        return Ps(d, void 0, void 0, (function() {
+                                        return Bs(d, void 0, void 0, (function() {
                                             var e;
-                                            return Rs(this, (function(t) {
+                                            return Fs(this, (function(t) {
                                                 switch (t.label) {
                                                     case 0:
-                                                        return [4, u.send(new Ec({
+                                                        return [4, u.send(new Tc({
                                                             IdentityPoolId: n
                                                         }))];
                                                     case 1:
-                                                        return e = t.sent().IdentityId, this._identityId = e, [2, Cc({
+                                                        return e = t.sent().IdentityId, this._identityId = e, [2, _c({
                                                             client: u,
                                                             identityId: e
                                                         })()]
                                                 }
                                             }))
                                         }))
                                     }, l = c().catch((function(e) {
-                                        return Ps(d, void 0, void 0, (function() {
-                                            return Rs(this, (function(t) {
+                                        return Bs(d, void 0, void 0, (function() {
+                                            return Fs(this, (function(t) {
                                                 throw e
                                             }))
                                         }))
                                     }))), [2, this._loadCredentials(l, "guest", !1, null).then((function(e) {
                                         return e
                                     })).catch((function(e) {
-                                        return Ps(d, void 0, void 0, (function() {
+                                        return Bs(d, void 0, void 0, (function() {
                                             var t, r = this;
-                                            return Rs(this, (function(o) {
+                                            return Fs(this, (function(o) {
                                                 switch (o.label) {
                                                     case 0:
-                                                        return "ResourceNotFoundException" !== e.name || e.message !== "Identity '" + a + "' not found." ? [3, 2] : (ap.debug("Failed to load guest credentials"), [4, this._removeGuestIdentityId()]);
+                                                        return "ResourceNotFoundException" !== e.name || e.message !== "Identity '" + a + "' not found." ? [3, 2] : (up.debug("Failed to load guest credentials"), [4, this._removeGuestIdentityId()]);
                                                     case 1:
                                                         return o.sent(), t = function() {
-                                                            return Ps(r, void 0, void 0, (function() {
+                                                            return Bs(r, void 0, void 0, (function() {
                                                                 var e;
-                                                                return Rs(this, (function(t) {
+                                                                return Fs(this, (function(t) {
                                                                     switch (t.label) {
                                                                         case 0:
-                                                                            return [4, u.send(new Ec({
+                                                                            return [4, u.send(new Tc({
                                                                                 IdentityPoolId: n
                                                                             }))];
                                                                         case 1:
-                                                                            return e = t.sent().IdentityId, this._identityId = e, [2, Cc({
+                                                                            return e = t.sent().IdentityId, this._identityId = e, [2, _c({
                                                                                 client: u,
                                                                                 identityId: e
                                                                             })()]
                                                                     }
                                                                 }))
                                                             }))
                                                         }, l = t().catch((function(e) {
-                                                            return Ps(r, void 0, void 0, (function() {
-                                                                return Rs(this, (function(t) {
+                                                            return Bs(r, void 0, void 0, (function() {
+                                                                return Fs(this, (function(t) {
                                                                     throw e
                                                                 }))
                                                             }))
                                                         })), [2, this._loadCredentials(l, "guest", !1, null)];
                                                     case 2:
                                                         return [2, e]
                                                 }
@@ -65619,191 +65647,191 @@
                     if (!o) return Promise.reject("You must specify a federated provider");
                     var i = {};
                     i[o] = n;
                     var a = this._config,
                         s = a.identityPoolId,
                         u = a.region,
                         l = a.identityPoolRegion;
-                    if (!s) return ap.debug("No Cognito Federated Identity pool provided"), Promise.reject("No Cognito Federated Identity pool provided");
-                    if (!l && !u) return ap.debug("region is not configured for getting the credentials"), Promise.reject("region is not configured for getting the credentials");
-                    var c = ip({
+                    if (!s) return up.debug("No Cognito Federated Identity pool provided"), Promise.reject("No Cognito Federated Identity pool provided");
+                    if (!l && !u) return up.debug("region is not configured for getting the credentials"), Promise.reject("region is not configured for getting the credentials");
+                    var c = sp({
                             region: l || u
                         }),
                         d = void 0;
-                    r ? d = Cc({
+                    r ? d = _c({
                         identityId: r,
                         logins: i,
                         client: c
-                    })() : d = Oc({
+                    })() : d = Uc({
                         logins: i,
                         identityPoolId: s,
                         client: c
                     })();
                     return this._loadCredentials(d, "federated", !0, e)
                 }, e.prototype._setCredentialsFromSession = function(e) {
                     var t = this;
-                    ap.debug("set credentials from session");
+                    up.debug("set credentials from session");
                     var n = e.getIdToken().getJwtToken(),
                         r = this._config,
                         o = r.region,
                         i = r.userPoolId,
                         a = r.identityPoolId,
                         s = r.identityPoolRegion;
-                    if (!a) return ap.debug("No Cognito Federated Identity pool provided"), Promise.reject("No Cognito Federated Identity pool provided");
-                    if (!s && !o) return ap.debug("region is not configured for getting the credentials"), Promise.reject("region is not configured for getting the credentials");
+                    if (!a) return up.debug("No Cognito Federated Identity pool provided"), Promise.reject("No Cognito Federated Identity pool provided");
+                    if (!s && !o) return up.debug("region is not configured for getting the credentials"), Promise.reject("region is not configured for getting the credentials");
                     var u = {};
                     u["cognito-idp." + o + ".amazonaws.com/" + i] = n;
-                    var l = ip({
+                    var l = sp({
                             region: s || o
                         }),
-                        c = Ps(t, void 0, void 0, (function() {
+                        c = Bs(t, void 0, void 0, (function() {
                             var e, t, n, r, o, i, s, c, d, f;
-                            return Rs(this, (function(p) {
+                            return Fs(this, (function(p) {
                                 switch (p.label) {
                                     case 0:
                                         return [4, this._getGuestIdentityId()];
                                     case 1:
-                                        return (e = p.sent()) ? [3, 3] : [4, l.send(new Ec({
+                                        return (e = p.sent()) ? [3, 3] : [4, l.send(new Tc({
                                             IdentityPoolId: a,
                                             Logins: u
                                         }))];
                                     case 2:
                                         n = p.sent().IdentityId, t = n, p.label = 3;
                                     case 3:
-                                        return [4, l.send(new Dc({
+                                        return [4, l.send(new Lc({
                                             IdentityId: e || t,
                                             Logins: u
                                         }))];
                                     case 4:
-                                        return r = p.sent(), o = r.Credentials, i = o.AccessKeyId, s = o.Expiration, c = o.SecretKey, d = o.SessionToken, f = r.IdentityId, this._identityId = f, e ? (ap.debug("The guest identity " + e + " has been successfully linked to the logins"), e === f && ap.debug("The guest identity " + e + " has become the primary identity"), [4, this._removeGuestIdentityId()]) : [3, 6];
+                                        return r = p.sent(), o = r.Credentials, i = o.AccessKeyId, s = o.Expiration, c = o.SecretKey, d = o.SessionToken, f = r.IdentityId, this._identityId = f, e ? (up.debug("The guest identity " + e + " has been successfully linked to the logins"), e === f && up.debug("The guest identity " + e + " has become the primary identity"), [4, this._removeGuestIdentityId()]) : [3, 6];
                                     case 5:
                                         p.sent(), p.label = 6;
                                     case 6:
                                         return [2, {
                                             accessKeyId: i,
                                             secretAccessKey: c,
                                             sessionToken: d,
                                             expiration: s,
                                             identityId: f
                                         }]
                                 }
                             }))
                         })).catch((function(e) {
-                            return Ps(t, void 0, void 0, (function() {
-                                return Rs(this, (function(t) {
+                            return Bs(t, void 0, void 0, (function() {
+                                return Fs(this, (function(t) {
                                     throw e
                                 }))
                             }))
                         }));
                     return this._loadCredentials(c, "userPool", !0, null)
                 }, e.prototype._loadCredentials = function(e, t, n, r) {
                     var o = this,
                         i = this;
                     return new Promise((function(a, s) {
                         e.then((function(e) {
-                            return Ps(o, void 0, void 0, (function() {
+                            return Bs(o, void 0, void 0, (function() {
                                 var o, s, u, l, c;
-                                return Rs(this, (function(d) {
+                                return Fs(this, (function(d) {
                                     switch (d.label) {
                                         case 0:
-                                            if (ap.debug("Load credentials successfully", e), this._identityId && !e.identityId && (e.identityId = this._identityId), i._credentials = e, i._credentials.authenticated = n, i._credentials_source = t, i._nextCredentialsRefresh = (new Date).getTime() + 3e6, "federated" === t) {
+                                            if (up.debug("Load credentials successfully", e), this._identityId && !e.identityId && (e.identityId = this._identityId), i._credentials = e, i._credentials.authenticated = n, i._credentials_source = t, i._nextCredentialsRefresh = (new Date).getTime() + 3e6, "federated" === t) {
                                                 o = Object.assign({
                                                     id: this._credentials.identityId
                                                 }, r.user), s = r.provider, u = r.token, l = r.expires_at, c = r.identity_id;
                                                 try {
                                                     this._storage.setItem("aws-amplify-federatedInfo", JSON.stringify({
                                                         provider: s,
                                                         token: u,
                                                         user: o,
                                                         expires_at: l,
                                                         identity_id: c
                                                     }))
                                                 } catch (f) {
-                                                    ap.debug("Failed to put federated info into auth storage", f)
+                                                    up.debug("Failed to put federated info into auth storage", f)
                                                 }
                                             }
                                             return "guest" !== t ? [3, 2] : [4, this._setGuestIdentityId(e.identityId)];
                                         case 1:
                                             d.sent(), d.label = 2;
                                         case 2:
                                             return a(i._credentials), [2]
                                     }
                                 }))
                             }))
                         })).catch((function(t) {
-                            if (t) return ap.debug("Failed to load credentials", e), ap.debug("Error loading credentials", t), void s(t)
+                            if (t) return up.debug("Failed to load credentials", e), up.debug("Error loading credentials", t), void s(t)
                         }))
                     }))
                 }, e.prototype.set = function(e, t) {
-                    return "session" === t ? this._setCredentialsFromSession(e) : "federation" === t ? this._setCredentialsFromFederation(e) : "guest" === t ? this._setCredentialsForGuest() : (ap.debug("no source specified for setting credentials"), Promise.reject("invalid source"))
+                    return "session" === t ? this._setCredentialsFromSession(e) : "federation" === t ? this._setCredentialsFromFederation(e) : "guest" === t ? this._setCredentialsForGuest() : (up.debug("no source specified for setting credentials"), Promise.reject("invalid source"))
                 }, e.prototype.clear = function() {
-                    return Ps(this, void 0, void 0, (function() {
-                        return Rs(this, (function(e) {
-                            return this._credentials = null, this._credentials_source = null, ap.debug("removing aws-amplify-federatedInfo from storage"), this._storage.removeItem("aws-amplify-federatedInfo"), [2]
+                    return Bs(this, void 0, void 0, (function() {
+                        return Fs(this, (function(e) {
+                            return this._credentials = null, this._credentials_source = null, up.debug("removing aws-amplify-federatedInfo from storage"), this._storage.removeItem("aws-amplify-federatedInfo"), [2]
                         }))
                     }))
                 }, e.prototype._getGuestIdentityId = function() {
-                    return Ps(this, void 0, void 0, (function() {
+                    return Bs(this, void 0, void 0, (function() {
                         var e, t;
-                        return Rs(this, (function(n) {
+                        return Fs(this, (function(n) {
                             switch (n.label) {
                                 case 0:
                                     e = this._config.identityPoolId, n.label = 1;
                                 case 1:
                                     return n.trys.push([1, 3, , 4]), [4, this._storageSync];
                                 case 2:
                                     return n.sent(), [2, this._storage.getItem(this._getCognitoIdentityIdStorageKey(e))];
                                 case 3:
-                                    return t = n.sent(), ap.debug("Failed to get the cached guest identityId", t), [3, 4];
+                                    return t = n.sent(), up.debug("Failed to get the cached guest identityId", t), [3, 4];
                                 case 4:
                                     return [2]
                             }
                         }))
                     }))
                 }, e.prototype._setGuestIdentityId = function(e) {
-                    return Ps(this, void 0, void 0, (function() {
+                    return Bs(this, void 0, void 0, (function() {
                         var t, n;
-                        return Rs(this, (function(r) {
+                        return Fs(this, (function(r) {
                             switch (r.label) {
                                 case 0:
                                     t = this._config.identityPoolId, r.label = 1;
                                 case 1:
                                     return r.trys.push([1, 3, , 4]), [4, this._storageSync];
                                 case 2:
                                     return r.sent(), this._storage.setItem(this._getCognitoIdentityIdStorageKey(t), e), [3, 4];
                                 case 3:
-                                    return n = r.sent(), ap.debug("Failed to cache guest identityId", n), [3, 4];
+                                    return n = r.sent(), up.debug("Failed to cache guest identityId", n), [3, 4];
                                 case 4:
                                     return [2]
                             }
                         }))
                     }))
                 }, e.prototype._removeGuestIdentityId = function() {
-                    return Ps(this, void 0, void 0, (function() {
+                    return Bs(this, void 0, void 0, (function() {
                         var e;
-                        return Rs(this, (function(t) {
-                            return e = this._config.identityPoolId, ap.debug("removing " + this._getCognitoIdentityIdStorageKey(e) + " from storage"), this._storage.removeItem(this._getCognitoIdentityIdStorageKey(e)), [2]
+                        return Fs(this, (function(t) {
+                            return e = this._config.identityPoolId, up.debug("removing " + this._getCognitoIdentityIdStorageKey(e) + " from storage"), this._storage.removeItem(this._getCognitoIdentityIdStorageKey(e)), [2]
                         }))
                     }))
                 }, e.prototype.shear = function(e) {
                     return {
                         accessKeyId: e.accessKeyId,
                         sessionToken: e.sessionToken,
                         secretAccessKey: e.secretAccessKey,
                         identityId: e.identityId,
                         authenticated: e.authenticated
                     }
                 }, e
             }(),
-            lp = new up(null);
-        pu.register(lp);
-        var cp = $s().isBrowser,
-            dp = function() {
+            dp = new cp(null);
+        gu.register(dp);
+        var fp = tu().isBrowser,
+            pp = function() {
                 function e(e) {
-                    void 0 === e && (e = {}), this.cookies = new tt, this.store = cp ? window.localStorage : Object.create(null), this.cookies = e.req ? new tt(e.req.headers.cookie) : new tt, Object.assign(this.store, this.cookies.getAll())
+                    void 0 === e && (e = {}), this.cookies = new tt, this.store = fp ? window.localStorage : Object.create(null), this.cookies = e.req ? new tt(e.req.headers.cookie) : new tt, Object.assign(this.store, this.cookies.getAll())
                 }
                 return Object.defineProperty(e.prototype, "length", {
                     get: function() {
                         return Object.entries(this.store).length
                     },
                     enumerable: !0,
                     configurable: !0
@@ -65835,22 +65863,22 @@
                     var n = e.split(".").pop();
                     ["LastAuthUser", "accessToken", "refreshToken", "idToken"].includes(null !== n && void 0 !== n ? n : "") && this.setUniversalItem(e, t, {
                         expires: new Date(Date.now() + 31536e6)
                     })
                 }, e.prototype.setLocalItem = function(e, t) {
                     this.store[e] = t
                 }, e.prototype.setUniversalItem = function(e, t, n) {
-                    void 0 === n && (n = {}), this.cookies.set(e, t, Us(Us({}, n), {
+                    void 0 === n && (n = {}), this.cookies.set(e, t, Rs(Rs({}, n), {
                         path: "/",
                         sameSite: !0,
-                        secure: !cp || "localhost" !== window.location.hostname
+                        secure: !fp || "localhost" !== window.location.hostname
                     }))
                 }, e
             }();
-        var fp, pp = function() {
+        var hp, gp = function() {
                 function e(e) {
                     var t = e || {},
                         n = t.ValidationData,
                         r = t.Username,
                         o = t.Password,
                         i = t.AuthParameters,
                         a = t.ClientMetadata;
@@ -65865,253 +65893,253 @@
                     return this.validationData
                 }, t.getAuthParameters = function() {
                     return this.authParameters
                 }, t.getClientMetadata = function() {
                     return this.clientMetadata
                 }, e
             }(),
-            hp = __webpack_require__(2890);
+            yp = __webpack_require__(2890);
 
-        function gp() {
-            if (fp) {
-                if ("function" === typeof fp.getRandomValues) try {
-                    return fp.getRandomValues(new Uint32Array(1))[0]
+        function mp() {
+            if (hp) {
+                if ("function" === typeof hp.getRandomValues) try {
+                    return hp.getRandomValues(new Uint32Array(1))[0]
                 } catch (e) {}
-                if ("function" === typeof fp.randomBytes) try {
-                    return fp.randomBytes(4).readInt32LE()
+                if ("function" === typeof hp.randomBytes) try {
+                    return hp.randomBytes(4).readInt32LE()
                 } catch (e) {}
             }
             throw new Error("Native crypto module could not be used to get secure random number.")
         }
-        "undefined" !== typeof window && window.crypto && (fp = window.crypto), !fp && "undefined" !== typeof window && window.msCrypto && (fp = window.msCrypto);
-        var yp, mp = function() {
+        "undefined" !== typeof window && window.crypto && (hp = window.crypto), !hp && "undefined" !== typeof window && window.msCrypto && (hp = window.msCrypto);
+        var vp, Mp = function() {
                 function e(e, t) {
                     e = this.words = e || [], this.sigBytes = void 0 != t ? t : 4 * e.length
                 }
                 var t = e.prototype;
                 return t.random = function(t) {
-                    for (var n = [], r = 0; r < t; r += 4) n.push(gp());
+                    for (var n = [], r = 0; r < t; r += 4) n.push(mp());
                     return new e(n, t)
                 }, t.toString = function() {
                     return function(e) {
                         for (var t = e.words, n = e.sigBytes, r = [], o = 0; o < n; o++) {
                             var i = t[o >>> 2] >>> 24 - o % 4 * 8 & 255;
                             r.push((i >>> 4).toString(16)), r.push((15 & i).toString(16))
                         }
                         return r.join("")
                     }(this)
                 }, e
             }(),
-            vp = __webpack_require__(6915),
-            Mp = bp;
+            bp = __webpack_require__(6915),
+            jp = wp;
 
-        function bp(e, t) {
+        function wp(e, t) {
             null != e && this.fromString(e, t)
         }
 
-        function jp() {
-            return new bp(null)
+        function xp() {
+            return new wp(null)
         }
-        var wp = "undefined" !== typeof navigator;
-        wp && "Microsoft Internet Explorer" == navigator.appName ? (bp.prototype.am = function(e, t, n, r, o, i) {
+        var Np = "undefined" !== typeof navigator;
+        Np && "Microsoft Internet Explorer" == navigator.appName ? (wp.prototype.am = function(e, t, n, r, o, i) {
             for (var a = 32767 & t, s = t >> 15; --i >= 0;) {
                 var u = 32767 & this[e],
                     l = this[e++] >> 15,
                     c = s * u + l * a;
                 o = ((u = a * u + ((32767 & c) << 15) + n[r] + (1073741823 & o)) >>> 30) + (c >>> 15) + s * l + (o >>> 30), n[r++] = 1073741823 & u
             }
             return o
-        }, yp = 30) : wp && "Netscape" != navigator.appName ? (bp.prototype.am = function(e, t, n, r, o, i) {
+        }, vp = 30) : Np && "Netscape" != navigator.appName ? (wp.prototype.am = function(e, t, n, r, o, i) {
             for (; --i >= 0;) {
                 var a = t * this[e++] + n[r] + o;
                 o = Math.floor(a / 67108864), n[r++] = 67108863 & a
             }
             return o
-        }, yp = 26) : (bp.prototype.am = function(e, t, n, r, o, i) {
+        }, vp = 26) : (wp.prototype.am = function(e, t, n, r, o, i) {
             for (var a = 16383 & t, s = t >> 14; --i >= 0;) {
                 var u = 16383 & this[e],
                     l = this[e++] >> 14,
                     c = s * u + l * a;
                 o = ((u = a * u + ((16383 & c) << 14) + n[r] + o) >> 28) + (c >> 14) + s * l, n[r++] = 268435455 & u
             }
             return o
-        }, yp = 28), bp.prototype.DB = yp, bp.prototype.DM = (1 << yp) - 1, bp.prototype.DV = 1 << yp;
-        bp.prototype.FV = Math.pow(2, 52), bp.prototype.F1 = 52 - yp, bp.prototype.F2 = 2 * yp - 52;
-        var xp, Np, Ip = new Array;
-        for (xp = "0".charCodeAt(0), Np = 0; Np <= 9; ++Np) Ip[xp++] = Np;
-        for (xp = "a".charCodeAt(0), Np = 10; Np < 36; ++Np) Ip[xp++] = Np;
-        for (xp = "A".charCodeAt(0), Np = 10; Np < 36; ++Np) Ip[xp++] = Np;
+        }, vp = 28), wp.prototype.DB = vp, wp.prototype.DM = (1 << vp) - 1, wp.prototype.DV = 1 << vp;
+        wp.prototype.FV = Math.pow(2, 52), wp.prototype.F1 = 52 - vp, wp.prototype.F2 = 2 * vp - 52;
+        var Ip, Dp, Sp = new Array;
+        for (Ip = "0".charCodeAt(0), Dp = 0; Dp <= 9; ++Dp) Sp[Ip++] = Dp;
+        for (Ip = "a".charCodeAt(0), Dp = 10; Dp < 36; ++Dp) Sp[Ip++] = Dp;
+        for (Ip = "A".charCodeAt(0), Dp = 10; Dp < 36; ++Dp) Sp[Ip++] = Dp;
 
-        function Dp(e) {
+        function Lp(e) {
             return "0123456789abcdefghijklmnopqrstuvwxyz".charAt(e)
         }
 
-        function Sp(e, t) {
-            var n = Ip[e.charCodeAt(t)];
+        function kp(e, t) {
+            var n = Sp[e.charCodeAt(t)];
             return null == n ? -1 : n
         }
 
-        function Lp(e) {
-            var t = jp();
+        function Cp(e) {
+            var t = xp();
             return t.fromInt(e), t
         }
 
-        function kp(e) {
+        function Ep(e) {
             var t, n = 1;
             return 0 != (t = e >>> 16) && (e = t, n += 16), 0 != (t = e >> 8) && (e = t, n += 8), 0 != (t = e >> 4) && (e = t, n += 4), 0 != (t = e >> 2) && (e = t, n += 2), 0 != (t = e >> 1) && (e = t, n += 1), n
         }
 
-        function Cp(e) {
+        function _p(e) {
             this.m = e, this.mp = e.invDigit(), this.mpl = 32767 & this.mp, this.mph = this.mp >> 15, this.um = (1 << e.DB - 15) - 1, this.mt2 = 2 * e.t
         }
 
-        function Ep(e) {
-            return hp.lW.from((new mp).random(e).toString(), "hex")
+        function Tp(e) {
+            return yp.lW.from((new Mp).random(e).toString(), "hex")
         }
-        Cp.prototype.convert = function(e) {
-            var t = jp();
-            return e.abs().dlShiftTo(this.m.t, t), t.divRemTo(this.m, null, t), e.s < 0 && t.compareTo(bp.ZERO) > 0 && this.m.subTo(t, t), t
-        }, Cp.prototype.revert = function(e) {
-            var t = jp();
+        _p.prototype.convert = function(e) {
+            var t = xp();
+            return e.abs().dlShiftTo(this.m.t, t), t.divRemTo(this.m, null, t), e.s < 0 && t.compareTo(wp.ZERO) > 0 && this.m.subTo(t, t), t
+        }, _p.prototype.revert = function(e) {
+            var t = xp();
             return e.copyTo(t), this.reduce(t), t
-        }, Cp.prototype.reduce = function(e) {
+        }, _p.prototype.reduce = function(e) {
             for (; e.t <= this.mt2;) e[e.t++] = 0;
             for (var t = 0; t < this.m.t; ++t) {
                 var n = 32767 & e[t],
                     r = n * this.mpl + ((n * this.mph + (e[t] >> 15) * this.mpl & this.um) << 15) & e.DM;
                 for (e[n = t + this.m.t] += this.m.am(0, r, e, t, 0, this.m.t); e[n] >= e.DV;) e[n] -= e.DV, e[++n]++
             }
             e.clamp(), e.drShiftTo(this.m.t, e), e.compareTo(this.m) >= 0 && e.subTo(this.m, e)
-        }, Cp.prototype.mulTo = function(e, t, n) {
+        }, _p.prototype.mulTo = function(e, t, n) {
             e.multiplyTo(t, n), this.reduce(n)
-        }, Cp.prototype.sqrTo = function(e, t) {
+        }, _p.prototype.sqrTo = function(e, t) {
             e.squareTo(t), this.reduce(t)
-        }, bp.prototype.copyTo = function(e) {
+        }, wp.prototype.copyTo = function(e) {
             for (var t = this.t - 1; t >= 0; --t) e[t] = this[t];
             e.t = this.t, e.s = this.s
-        }, bp.prototype.fromInt = function(e) {
+        }, wp.prototype.fromInt = function(e) {
             this.t = 1, this.s = e < 0 ? -1 : 0, e > 0 ? this[0] = e : e < -1 ? this[0] = e + this.DV : this.t = 0
-        }, bp.prototype.fromString = function(e, t) {
+        }, wp.prototype.fromString = function(e, t) {
             var n;
             if (16 == t) n = 4;
             else if (8 == t) n = 3;
             else if (2 == t) n = 1;
             else if (32 == t) n = 5;
             else {
                 if (4 != t) throw new Error("Only radix 2, 4, 8, 16, 32 are supported");
                 n = 2
             }
             this.t = 0, this.s = 0;
             for (var r = e.length, o = !1, i = 0; --r >= 0;) {
-                var a = Sp(e, r);
+                var a = kp(e, r);
                 a < 0 ? "-" == e.charAt(r) && (o = !0) : (o = !1, 0 == i ? this[this.t++] = a : i + n > this.DB ? (this[this.t - 1] |= (a & (1 << this.DB - i) - 1) << i, this[this.t++] = a >> this.DB - i) : this[this.t - 1] |= a << i, (i += n) >= this.DB && (i -= this.DB))
             }
-            this.clamp(), o && bp.ZERO.subTo(this, this)
-        }, bp.prototype.clamp = function() {
+            this.clamp(), o && wp.ZERO.subTo(this, this)
+        }, wp.prototype.clamp = function() {
             for (var e = this.s & this.DM; this.t > 0 && this[this.t - 1] == e;) --this.t
-        }, bp.prototype.dlShiftTo = function(e, t) {
+        }, wp.prototype.dlShiftTo = function(e, t) {
             var n;
             for (n = this.t - 1; n >= 0; --n) t[n + e] = this[n];
             for (n = e - 1; n >= 0; --n) t[n] = 0;
             t.t = this.t + e, t.s = this.s
-        }, bp.prototype.drShiftTo = function(e, t) {
+        }, wp.prototype.drShiftTo = function(e, t) {
             for (var n = e; n < this.t; ++n) t[n - e] = this[n];
             t.t = Math.max(this.t - e, 0), t.s = this.s
-        }, bp.prototype.lShiftTo = function(e, t) {
+        }, wp.prototype.lShiftTo = function(e, t) {
             var n, r = e % this.DB,
                 o = this.DB - r,
                 i = (1 << o) - 1,
                 a = Math.floor(e / this.DB),
                 s = this.s << r & this.DM;
             for (n = this.t - 1; n >= 0; --n) t[n + a + 1] = this[n] >> o | s, s = (this[n] & i) << r;
             for (n = a - 1; n >= 0; --n) t[n] = 0;
             t[a] = s, t.t = this.t + a + 1, t.s = this.s, t.clamp()
-        }, bp.prototype.rShiftTo = function(e, t) {
+        }, wp.prototype.rShiftTo = function(e, t) {
             t.s = this.s;
             var n = Math.floor(e / this.DB);
             if (n >= this.t) t.t = 0;
             else {
                 var r = e % this.DB,
                     o = this.DB - r,
                     i = (1 << r) - 1;
                 t[0] = this[n] >> r;
                 for (var a = n + 1; a < this.t; ++a) t[a - n - 1] |= (this[a] & i) << o, t[a - n] = this[a] >> r;
                 r > 0 && (t[this.t - n - 1] |= (this.s & i) << o), t.t = this.t - n, t.clamp()
             }
-        }, bp.prototype.subTo = function(e, t) {
+        }, wp.prototype.subTo = function(e, t) {
             for (var n = 0, r = 0, o = Math.min(e.t, this.t); n < o;) r += this[n] - e[n], t[n++] = r & this.DM, r >>= this.DB;
             if (e.t < this.t) {
                 for (r -= e.s; n < this.t;) r += this[n], t[n++] = r & this.DM, r >>= this.DB;
                 r += this.s
             } else {
                 for (r += this.s; n < e.t;) r -= e[n], t[n++] = r & this.DM, r >>= this.DB;
                 r -= e.s
             }
             t.s = r < 0 ? -1 : 0, r < -1 ? t[n++] = this.DV + r : r > 0 && (t[n++] = r), t.t = n, t.clamp()
-        }, bp.prototype.multiplyTo = function(e, t) {
+        }, wp.prototype.multiplyTo = function(e, t) {
             var n = this.abs(),
                 r = e.abs(),
                 o = n.t;
             for (t.t = o + r.t; --o >= 0;) t[o] = 0;
             for (o = 0; o < r.t; ++o) t[o + n.t] = n.am(0, r[o], t, o, 0, n.t);
-            t.s = 0, t.clamp(), this.s != e.s && bp.ZERO.subTo(t, t)
-        }, bp.prototype.squareTo = function(e) {
+            t.s = 0, t.clamp(), this.s != e.s && wp.ZERO.subTo(t, t)
+        }, wp.prototype.squareTo = function(e) {
             for (var t = this.abs(), n = e.t = 2 * t.t; --n >= 0;) e[n] = 0;
             for (n = 0; n < t.t - 1; ++n) {
                 var r = t.am(n, t[n], e, 2 * n, 0, 1);
                 (e[n + t.t] += t.am(n + 1, 2 * t[n], e, 2 * n + 1, r, t.t - n - 1)) >= t.DV && (e[n + t.t] -= t.DV, e[n + t.t + 1] = 1)
             }
             e.t > 0 && (e[e.t - 1] += t.am(n, t[n], e, 2 * n, 0, 1)), e.s = 0, e.clamp()
-        }, bp.prototype.divRemTo = function(e, t, n) {
+        }, wp.prototype.divRemTo = function(e, t, n) {
             var r = e.abs();
             if (!(r.t <= 0)) {
                 var o = this.abs();
                 if (o.t < r.t) return null != t && t.fromInt(0), void(null != n && this.copyTo(n));
-                null == n && (n = jp());
-                var i = jp(),
+                null == n && (n = xp());
+                var i = xp(),
                     a = this.s,
                     s = e.s,
-                    u = this.DB - kp(r[r.t - 1]);
+                    u = this.DB - Ep(r[r.t - 1]);
                 u > 0 ? (r.lShiftTo(u, i), o.lShiftTo(u, n)) : (r.copyTo(i), o.copyTo(n));
                 var l = i.t,
                     c = i[l - 1];
                 if (0 != c) {
                     var d = c * (1 << this.F1) + (l > 1 ? i[l - 2] >> this.F2 : 0),
                         f = this.FV / d,
                         p = (1 << this.F1) / d,
                         h = 1 << this.F2,
                         g = n.t,
                         y = g - l,
-                        m = null == t ? jp() : t;
-                    for (i.dlShiftTo(y, m), n.compareTo(m) >= 0 && (n[n.t++] = 1, n.subTo(m, n)), bp.ONE.dlShiftTo(l, m), m.subTo(i, i); i.t < l;) i[i.t++] = 0;
+                        m = null == t ? xp() : t;
+                    for (i.dlShiftTo(y, m), n.compareTo(m) >= 0 && (n[n.t++] = 1, n.subTo(m, n)), wp.ONE.dlShiftTo(l, m), m.subTo(i, i); i.t < l;) i[i.t++] = 0;
                     for (; --y >= 0;) {
                         var v = n[--g] == c ? this.DM : Math.floor(n[g] * f + (n[g - 1] + h) * p);
                         if ((n[g] += i.am(0, v, n, y, 0, l)) < v)
                             for (i.dlShiftTo(y, m), n.subTo(m, n); n[g] < --v;) n.subTo(m, n)
                     }
-                    null != t && (n.drShiftTo(l, t), a != s && bp.ZERO.subTo(t, t)), n.t = l, n.clamp(), u > 0 && n.rShiftTo(u, n), a < 0 && bp.ZERO.subTo(n, n)
+                    null != t && (n.drShiftTo(l, t), a != s && wp.ZERO.subTo(t, t)), n.t = l, n.clamp(), u > 0 && n.rShiftTo(u, n), a < 0 && wp.ZERO.subTo(n, n)
                 }
             }
-        }, bp.prototype.invDigit = function() {
+        }, wp.prototype.invDigit = function() {
             if (this.t < 1) return 0;
             var e = this[0];
             if (0 == (1 & e)) return 0;
             var t = 3 & e;
             return (t = (t = (t = (t = t * (2 - (15 & e) * t) & 15) * (2 - (255 & e) * t) & 255) * (2 - ((65535 & e) * t & 65535)) & 65535) * (2 - e * t % this.DV) % this.DV) > 0 ? this.DV - t : -t
-        }, bp.prototype.addTo = function(e, t) {
+        }, wp.prototype.addTo = function(e, t) {
             for (var n = 0, r = 0, o = Math.min(e.t, this.t); n < o;) r += this[n] + e[n], t[n++] = r & this.DM, r >>= this.DB;
             if (e.t < this.t) {
                 for (r += e.s; n < this.t;) r += this[n], t[n++] = r & this.DM, r >>= this.DB;
                 r += this.s
             } else {
                 for (r += this.s; n < e.t;) r += e[n], t[n++] = r & this.DM, r >>= this.DB;
                 r += e.s
             }
             t.s = r < 0 ? -1 : 0, r > 0 ? t[n++] = r : r < -1 && (t[n++] = this.DV + r), t.t = n, t.clamp()
-        }, bp.prototype.toString = function(e) {
+        }, wp.prototype.toString = function(e) {
             if (this.s < 0) return "-" + this.negate().toString(e);
             var t;
             if (16 == e) t = 4;
             else if (8 == e) t = 3;
             else if (2 == e) t = 1;
             else if (32 == e) t = 5;
             else {
@@ -66120,236 +66148,236 @@
             }
             var n, r = (1 << t) - 1,
                 o = !1,
                 i = "",
                 a = this.t,
                 s = this.DB - a * this.DB % t;
             if (a-- > 0)
-                for (s < this.DB && (n = this[a] >> s) > 0 && (o = !0, i = Dp(n)); a >= 0;) s < t ? (n = (this[a] & (1 << s) - 1) << t - s, n |= this[--a] >> (s += this.DB - t)) : (n = this[a] >> (s -= t) & r, s <= 0 && (s += this.DB, --a)), n > 0 && (o = !0), o && (i += Dp(n));
+                for (s < this.DB && (n = this[a] >> s) > 0 && (o = !0, i = Lp(n)); a >= 0;) s < t ? (n = (this[a] & (1 << s) - 1) << t - s, n |= this[--a] >> (s += this.DB - t)) : (n = this[a] >> (s -= t) & r, s <= 0 && (s += this.DB, --a)), n > 0 && (o = !0), o && (i += Lp(n));
             return o ? i : "0"
-        }, bp.prototype.negate = function() {
-            var e = jp();
-            return bp.ZERO.subTo(this, e), e
-        }, bp.prototype.abs = function() {
+        }, wp.prototype.negate = function() {
+            var e = xp();
+            return wp.ZERO.subTo(this, e), e
+        }, wp.prototype.abs = function() {
             return this.s < 0 ? this.negate() : this
-        }, bp.prototype.compareTo = function(e) {
+        }, wp.prototype.compareTo = function(e) {
             var t = this.s - e.s;
             if (0 != t) return t;
             var n = this.t;
             if (0 != (t = n - e.t)) return this.s < 0 ? -t : t;
             for (; --n >= 0;)
                 if (0 != (t = this[n] - e[n])) return t;
             return 0
-        }, bp.prototype.bitLength = function() {
-            return this.t <= 0 ? 0 : this.DB * (this.t - 1) + kp(this[this.t - 1] ^ this.s & this.DM)
-        }, bp.prototype.mod = function(e) {
-            var t = jp();
-            return this.abs().divRemTo(e, null, t), this.s < 0 && t.compareTo(bp.ZERO) > 0 && e.subTo(t, t), t
-        }, bp.prototype.equals = function(e) {
+        }, wp.prototype.bitLength = function() {
+            return this.t <= 0 ? 0 : this.DB * (this.t - 1) + Ep(this[this.t - 1] ^ this.s & this.DM)
+        }, wp.prototype.mod = function(e) {
+            var t = xp();
+            return this.abs().divRemTo(e, null, t), this.s < 0 && t.compareTo(wp.ZERO) > 0 && e.subTo(t, t), t
+        }, wp.prototype.equals = function(e) {
             return 0 == this.compareTo(e)
-        }, bp.prototype.add = function(e) {
-            var t = jp();
+        }, wp.prototype.add = function(e) {
+            var t = xp();
             return this.addTo(e, t), t
-        }, bp.prototype.subtract = function(e) {
-            var t = jp();
+        }, wp.prototype.subtract = function(e) {
+            var t = xp();
             return this.subTo(e, t), t
-        }, bp.prototype.multiply = function(e) {
-            var t = jp();
+        }, wp.prototype.multiply = function(e) {
+            var t = xp();
             return this.multiplyTo(e, t), t
-        }, bp.prototype.divide = function(e) {
-            var t = jp();
+        }, wp.prototype.divide = function(e) {
+            var t = xp();
             return this.divRemTo(e, t, null), t
-        }, bp.prototype.modPow = function(e, t, n) {
+        }, wp.prototype.modPow = function(e, t, n) {
             var r, o = e.bitLength(),
-                i = Lp(1),
-                a = new Cp(t);
+                i = Cp(1),
+                a = new _p(t);
             if (o <= 0) return i;
             r = o < 18 ? 1 : o < 48 ? 3 : o < 144 ? 4 : o < 768 ? 5 : 6;
             var s = new Array,
                 u = 3,
                 l = r - 1,
                 c = (1 << r) - 1;
             if (s[1] = a.convert(this), r > 1) {
-                var d = jp();
-                for (a.sqrTo(s[1], d); u <= c;) s[u] = jp(), a.mulTo(d, s[u - 2], s[u]), u += 2
+                var d = xp();
+                for (a.sqrTo(s[1], d); u <= c;) s[u] = xp(), a.mulTo(d, s[u - 2], s[u]), u += 2
             }
             var f, p, h = e.t - 1,
                 g = !0,
-                y = jp();
-            for (o = kp(e[h]) - 1; h >= 0;) {
+                y = xp();
+            for (o = Ep(e[h]) - 1; h >= 0;) {
                 for (o >= l ? f = e[h] >> o - l & c : (f = (e[h] & (1 << o + 1) - 1) << l - o, h > 0 && (f |= e[h - 1] >> this.DB + o - l)), u = r; 0 == (1 & f);) f >>= 1, --u;
                 if ((o -= u) < 0 && (o += this.DB, --h), g) s[f].copyTo(i), g = !1;
                 else {
                     for (; u > 1;) a.sqrTo(i, y), a.sqrTo(y, i), u -= 2;
                     u > 0 ? a.sqrTo(i, y) : (p = i, i = y, y = p), a.mulTo(y, s[f], i)
                 }
                 for (; h >= 0 && 0 == (e[h] & 1 << o);) a.sqrTo(i, y), p = i, i = y, y = p, --o < 0 && (o = this.DB - 1, --h)
             }
             var m = a.revert(i);
             return n(null, m), m
-        }, bp.ZERO = Lp(0), bp.ONE = Lp(1);
-        var _p = /^[89a-f]/i,
-            Tp = function() {
+        }, wp.ZERO = Cp(0), wp.ONE = Cp(1);
+        var Ap = /^[89a-f]/i,
+            Op = function() {
                 function e(e) {
-                    this.N = new Mp("FFFFFFFFFFFFFFFFC90FDAA22168C234C4C6628B80DC1CD129024E088A67CC74020BBEA63B139B22514A08798E3404DDEF9519B3CD3A431B302B0A6DF25F14374FE1356D6D51C245E485B576625E7EC6F44C42E9A637ED6B0BFF5CB6F406B7EDEE386BFB5A899FA5AE9F24117C4B1FE649286651ECE45B3DC2007CB8A163BF0598DA48361C55D39A69163FA8FD24CF5F83655D23DCA3AD961C62F356208552BB9ED529077096966D670C354E4ABC9804F1746C08CA18217C32905E462E36CE3BE39E772C180E86039B2783A2EC07A28FB5C55DF06F4C52C9DE2BCBF6955817183995497CEA956AE515D2261898FA051015728E5A8AAAC42DAD33170D04507A33A85521ABDF1CBA64ECFB850458DBEF0A8AEA71575D060C7DB3970F85A6E1E4C7ABF5AE8CDB0933D71E8C94E04A25619DCEE3D2261AD2EE6BF12FFA06D98A0864D87602733EC86A64521F2B18177B200CBBE117577A615D6C770988C0BAD946E208E24FA074E5AB3143DB5BFCE0FD108E4B82D120A93AD2CAFFFFFFFFFFFFFFFF", 16), this.g = new Mp("2", 16), this.k = new Mp(this.hexHash("" + this.padHex(this.N) + this.padHex(this.g)), 16), this.smallAValue = this.generateRandomSmallA(), this.getLargeAValue((function() {})), this.infoBits = hp.lW.from("Caldera Derived Key", "utf8"), this.poolName = e
+                    this.N = new jp("FFFFFFFFFFFFFFFFC90FDAA22168C234C4C6628B80DC1CD129024E088A67CC74020BBEA63B139B22514A08798E3404DDEF9519B3CD3A431B302B0A6DF25F14374FE1356D6D51C245E485B576625E7EC6F44C42E9A637ED6B0BFF5CB6F406B7EDEE386BFB5A899FA5AE9F24117C4B1FE649286651ECE45B3DC2007CB8A163BF0598DA48361C55D39A69163FA8FD24CF5F83655D23DCA3AD961C62F356208552BB9ED529077096966D670C354E4ABC9804F1746C08CA18217C32905E462E36CE3BE39E772C180E86039B2783A2EC07A28FB5C55DF06F4C52C9DE2BCBF6955817183995497CEA956AE515D2261898FA051015728E5A8AAAC42DAD33170D04507A33A85521ABDF1CBA64ECFB850458DBEF0A8AEA71575D060C7DB3970F85A6E1E4C7ABF5AE8CDB0933D71E8C94E04A25619DCEE3D2261AD2EE6BF12FFA06D98A0864D87602733EC86A64521F2B18177B200CBBE117577A615D6C770988C0BAD946E208E24FA074E5AB3143DB5BFCE0FD108E4B82D120A93AD2CAFFFFFFFFFFFFFFFF", 16), this.g = new jp("2", 16), this.k = new jp(this.hexHash("" + this.padHex(this.N) + this.padHex(this.g)), 16), this.smallAValue = this.generateRandomSmallA(), this.getLargeAValue((function() {})), this.infoBits = yp.lW.from("Caldera Derived Key", "utf8"), this.poolName = e
                 }
                 var t = e.prototype;
                 return t.getSmallAValue = function() {
                     return this.smallAValue
                 }, t.getLargeAValue = function(e) {
                     var t = this;
                     this.largeAValue ? e(null, this.largeAValue) : this.calculateA(this.smallAValue, (function(n, r) {
                         n && e(n, null), t.largeAValue = r, e(null, t.largeAValue)
                     }))
                 }, t.generateRandomSmallA = function() {
-                    var e = Ep(128).toString("hex");
-                    return new Mp(e, 16)
+                    var e = Tp(128).toString("hex");
+                    return new jp(e, 16)
                 }, t.generateRandomString = function() {
-                    return Ep(40).toString("base64")
+                    return Tp(40).toString("base64")
                 }, t.getRandomPassword = function() {
                     return this.randomPassword
                 }, t.getSaltDevices = function() {
                     return this.SaltToHashDevices
                 }, t.getVerifierDevices = function() {
                     return this.verifierDevices
                 }, t.generateHashDevice = function(e, t, n) {
                     var r = this;
                     this.randomPassword = this.generateRandomString();
                     var o = "" + e + t + ":" + this.randomPassword,
                         i = this.hash(o),
-                        a = Ep(16).toString("hex");
-                    this.SaltToHashDevices = this.padHex(new Mp(a, 16)), this.g.modPow(new Mp(this.hexHash(this.SaltToHashDevices + i), 16), this.N, (function(e, t) {
+                        a = Tp(16).toString("hex");
+                    this.SaltToHashDevices = this.padHex(new jp(a, 16)), this.g.modPow(new jp(this.hexHash(this.SaltToHashDevices + i), 16), this.N, (function(e, t) {
                         e && n(e, null), r.verifierDevices = r.padHex(t), n(null, null)
                     }))
                 }, t.calculateA = function(e, t) {
                     var n = this;
                     this.g.modPow(e, this.N, (function(e, r) {
-                        e && t(e, null), r.mod(n.N).equals(Mp.ZERO) && t(new Error("Illegal paramater. A mod N cannot be 0."), null), t(null, r)
+                        e && t(e, null), r.mod(n.N).equals(jp.ZERO) && t(new Error("Illegal paramater. A mod N cannot be 0."), null), t(null, r)
                     }))
                 }, t.calculateU = function(e, t) {
-                    return this.UHexHash = this.hexHash(this.padHex(e) + this.padHex(t)), new Mp(this.UHexHash, 16)
+                    return this.UHexHash = this.hexHash(this.padHex(e) + this.padHex(t)), new jp(this.UHexHash, 16)
                 }, t.hash = function(e) {
-                    var t = new vp.Sha256;
+                    var t = new bp.Sha256;
                     t.update(e);
                     var n = t.digestSync(),
-                        r = hp.lW.from(n).toString("hex");
+                        r = yp.lW.from(n).toString("hex");
                     return new Array(64 - r.length).join("0") + r
                 }, t.hexHash = function(e) {
-                    return this.hash(hp.lW.from(e, "hex"))
+                    return this.hash(yp.lW.from(e, "hex"))
                 }, t.computehkdf = function(e, t) {
-                    var n = hp.lW.concat([this.infoBits, hp.lW.from(String.fromCharCode(1), "utf8")]),
-                        r = new vp.Sha256(t);
+                    var n = yp.lW.concat([this.infoBits, yp.lW.from(String.fromCharCode(1), "utf8")]),
+                        r = new bp.Sha256(t);
                     r.update(e);
                     var o = r.digestSync(),
-                        i = new vp.Sha256(o);
+                        i = new bp.Sha256(o);
                     return i.update(n), i.digestSync().slice(0, 16)
                 }, t.getPasswordAuthenticationKey = function(e, t, n, r, o) {
                     var i = this;
-                    if (n.mod(this.N).equals(Mp.ZERO)) throw new Error("B cannot be zero.");
-                    if (this.UValue = this.calculateU(this.largeAValue, n), this.UValue.equals(Mp.ZERO)) throw new Error("U cannot be zero.");
+                    if (n.mod(this.N).equals(jp.ZERO)) throw new Error("B cannot be zero.");
+                    if (this.UValue = this.calculateU(this.largeAValue, n), this.UValue.equals(jp.ZERO)) throw new Error("U cannot be zero.");
                     var a = "" + this.poolName + e + ":" + t,
                         s = this.hash(a),
-                        u = new Mp(this.hexHash(this.padHex(r) + s), 16);
+                        u = new jp(this.hexHash(this.padHex(r) + s), 16);
                     this.calculateS(u, n, (function(e, t) {
                         e && o(e, null);
-                        var n = i.computehkdf(hp.lW.from(i.padHex(t), "hex"), hp.lW.from(i.padHex(i.UValue), "hex"));
+                        var n = i.computehkdf(yp.lW.from(i.padHex(t), "hex"), yp.lW.from(i.padHex(i.UValue), "hex"));
                         o(null, n)
                     }))
                 }, t.calculateS = function(e, t, n) {
                     var r = this;
                     this.g.modPow(e, this.N, (function(o, i) {
                         o && n(o, null), t.subtract(r.k.multiply(i)).modPow(r.smallAValue.add(r.UValue.multiply(e)), r.N, (function(e, t) {
                             e && n(e, null), n(null, t.mod(r.N))
                         }))
                     }))
                 }, t.getNewPasswordRequiredChallengeUserAttributePrefix = function() {
                     return "userAttributes."
                 }, t.padHex = function(e) {
-                    if (!(e instanceof Mp)) throw new Error("Not a BigInteger");
-                    var t = e.compareTo(Mp.ZERO) < 0,
+                    if (!(e instanceof jp)) throw new Error("Not a BigInteger");
+                    var t = e.compareTo(jp.ZERO) < 0,
                         n = e.abs().toString(16);
-                    if (n = n.length % 2 !== 0 ? "0" + n : n, n = _p.test(n) ? "00" + n : n, t) {
+                    if (n = n.length % 2 !== 0 ? "0" + n : n, n = Ap.test(n) ? "00" + n : n, t) {
                         var r = n.split("").map((function(e) {
                             var t = 15 & ~parseInt(e, 16);
                             return "0123456789ABCDEF".charAt(t)
                         })).join("");
-                        (n = new Mp(r, 16).add(Mp.ONE).toString(16)).toUpperCase().startsWith("FF8") && (n = n.substring(2))
+                        (n = new jp(r, 16).add(jp.ONE).toString(16)).toUpperCase().startsWith("FF8") && (n = n.substring(2))
                     }
                     return n
                 }, e
             }(),
-            Ap = function() {
+            zp = function() {
                 function e(e) {
                     this.jwtToken = e || "", this.payload = this.decodePayload()
                 }
                 var t = e.prototype;
                 return t.getJwtToken = function() {
                     return this.jwtToken
                 }, t.getExpiration = function() {
                     return this.payload.exp
                 }, t.getIssuedAt = function() {
                     return this.payload.iat
                 }, t.decodePayload = function() {
                     var e = this.jwtToken.split(".")[1];
                     try {
-                        return JSON.parse(hp.lW.from(e, "base64").toString("utf8"))
+                        return JSON.parse(yp.lW.from(e, "base64").toString("utf8"))
                     } catch (t) {
                         return {}
                     }
                 }, e
             }();
 
-        function Op(e, t) {
-            return Op = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
+        function Up(e, t) {
+            return Up = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
                 return e.__proto__ = t, e
-            }, Op(e, t)
+            }, Up(e, t)
         }
-        var zp = function(e) {
+        var Pp = function(e) {
             var t, n;
 
             function r(t) {
                 var n = (void 0 === t ? {} : t).AccessToken;
                 return e.call(this, n || "") || this
             }
-            return n = e, (t = r).prototype = Object.create(n.prototype), t.prototype.constructor = t, Op(t, n), r
-        }(Ap);
+            return n = e, (t = r).prototype = Object.create(n.prototype), t.prototype.constructor = t, Up(t, n), r
+        }(zp);
 
-        function Up(e, t) {
-            return Up = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
+        function Rp(e, t) {
+            return Rp = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
                 return e.__proto__ = t, e
-            }, Up(e, t)
+            }, Rp(e, t)
         }
-        var Pp = function(e) {
+        var Bp = function(e) {
                 var t, n;
 
                 function r(t) {
                     var n = (void 0 === t ? {} : t).IdToken;
                     return e.call(this, n || "") || this
                 }
-                return n = e, (t = r).prototype = Object.create(n.prototype), t.prototype.constructor = t, Up(t, n), r
-            }(Ap),
-            Rp = function() {
+                return n = e, (t = r).prototype = Object.create(n.prototype), t.prototype.constructor = t, Rp(t, n), r
+            }(zp),
+            Fp = function() {
                 function e(e) {
                     var t = (void 0 === e ? {} : e).RefreshToken;
                     this.token = t || ""
                 }
                 return e.prototype.getToken = function() {
                     return this.token
                 }, e
             }(),
-            Bp = {
+            Yp = {
                 userAgent: "aws-amplify/5.0.4 js",
                 product: "",
                 navigator: null,
                 isReactNative: !1
             };
         if ("undefined" !== typeof navigator && navigator.product)
-            if (Bp.product = navigator.product || "", Bp.navigator = navigator || null, "ReactNative" === navigator.product) Bp.userAgent = "aws-amplify/5.0.4 react-native", Bp.isReactNative = !0;
-            else Bp.userAgent = "aws-amplify/5.0.4 js", Bp.isReactNative = !1;
-        var Fp = function() {
+            if (Yp.product = navigator.product || "", Yp.navigator = navigator || null, "ReactNative" === navigator.product) Yp.userAgent = "aws-amplify/5.0.4 react-native", Yp.isReactNative = !0;
+            else Yp.userAgent = "aws-amplify/5.0.4 js", Yp.isReactNative = !1;
+        var Qp = function() {
                 function e(e) {
                     var t = void 0 === e ? {} : e,
                         n = t.IdToken,
                         r = t.RefreshToken,
                         o = t.AccessToken,
                         i = t.ClockDrift;
                     if (null == o || null == n) throw new Error("Id token and Access Token must be present.");
@@ -66367,32 +66395,32 @@
                 }, t.calculateClockDrift = function() {
                     return Math.floor(new Date / 1e3) - Math.min(this.accessToken.getIssuedAt(), this.idToken.getIssuedAt())
                 }, t.isValid = function() {
                     var e = Math.floor(new Date / 1e3) - this.clockDrift;
                     return e < this.accessToken.getExpiration() && e < this.idToken.getExpiration()
                 }, e
             }(),
-            Yp = ["Jan", "Feb", "Mar", "Apr", "May", "Jun", "Jul", "Aug", "Sep", "Oct", "Nov", "Dec"],
-            Qp = ["Sun", "Mon", "Tue", "Wed", "Thu", "Fri", "Sat"],
-            Gp = function() {
+            Gp = ["Jan", "Feb", "Mar", "Apr", "May", "Jun", "Jul", "Aug", "Sep", "Oct", "Nov", "Dec"],
+            Wp = ["Sun", "Mon", "Tue", "Wed", "Thu", "Fri", "Sat"],
+            Hp = function() {
                 function e() {}
                 return e.prototype.getNowString = function() {
                     var e = new Date,
-                        t = Qp[e.getUTCDay()],
-                        n = Yp[e.getUTCMonth()],
+                        t = Wp[e.getUTCDay()],
+                        n = Gp[e.getUTCMonth()],
                         r = e.getUTCDate(),
                         o = e.getUTCHours();
                     o < 10 && (o = "0" + o);
                     var i = e.getUTCMinutes();
                     i < 10 && (i = "0" + i);
                     var a = e.getUTCSeconds();
                     return a < 10 && (a = "0" + a), t + " " + n + " " + r + " " + o + ":" + i + ":" + a + " UTC " + e.getUTCFullYear()
                 }, e
             }(),
-            Wp = function() {
+            Zp = function() {
                 function e(e) {
                     var t = void 0 === e ? {} : e,
                         n = t.Name,
                         r = t.Value;
                     this.Name = n || "", this.Value = r || ""
                 }
                 var t = e.prototype;
@@ -66409,44 +66437,44 @@
                 }, t.toJSON = function() {
                     return {
                         Name: this.Name,
                         Value: this.Value
                     }
                 }, e
             }(),
-            Hp = {},
-            Zp = function() {
+            Vp = {},
+            qp = function() {
                 function e() {}
                 return e.setItem = function(e, t) {
-                    return Hp[e] = t, Hp[e]
+                    return Vp[e] = t, Vp[e]
                 }, e.getItem = function(e) {
-                    return Object.prototype.hasOwnProperty.call(Hp, e) ? Hp[e] : void 0
+                    return Object.prototype.hasOwnProperty.call(Vp, e) ? Vp[e] : void 0
                 }, e.removeItem = function(e) {
-                    return delete Hp[e]
+                    return delete Vp[e]
                 }, e.clear = function() {
-                    return Hp = {}
+                    return Vp = {}
                 }, e
             }(),
-            Vp = function() {
+            Jp = function() {
                 function e() {
                     try {
                         this.storageWindow = window.localStorage, this.storageWindow.setItem("aws.cognito.test-ls", 1), this.storageWindow.removeItem("aws.cognito.test-ls")
                     } catch (e) {
-                        this.storageWindow = Zp
+                        this.storageWindow = qp
                     }
                 }
                 return e.prototype.getStorage = function() {
                     return this.storageWindow
                 }, e
             }(),
-            qp = "undefined" !== typeof navigator ? Bp.isReactNative ? "react-native" : navigator.userAgent : "nodejs",
-            Jp = function() {
+            Kp = "undefined" !== typeof navigator ? Yp.isReactNative ? "react-native" : navigator.userAgent : "nodejs",
+            Xp = function() {
                 function e(e) {
                     if (null == e || null == e.Username || null == e.Pool) throw new Error("Username and Pool information are required.");
-                    this.username = e.Username || "", this.pool = e.Pool, this.Session = null, this.client = e.Pool.client, this.signInUserSession = null, this.authenticationFlowType = "USER_SRP_AUTH", this.storage = e.Storage || (new Vp).getStorage(), this.keyPrefix = "CognitoIdentityServiceProvider." + this.pool.getClientId(), this.userDataKey = this.keyPrefix + "." + this.username + ".userData"
+                    this.username = e.Username || "", this.pool = e.Pool, this.Session = null, this.client = e.Pool.client, this.signInUserSession = null, this.authenticationFlowType = "USER_SRP_AUTH", this.storage = e.Storage || (new Jp).getStorage(), this.keyPrefix = "CognitoIdentityServiceProvider." + this.pool.getClientId(), this.userDataKey = this.keyPrefix + "." + this.username + ".userData"
                 }
                 var t = e.prototype;
                 return t.setSignInUserSession = function(e) {
                     this.clearCachedUserData(), this.signInUserSession = e, this.cacheTokens()
                 }, t.getSignInUserSession = function() {
                     return this.signInUserSession
                 }, t.getUsername = function() {
@@ -66472,37 +66500,37 @@
                             i = r.ChallengeParameters;
                         return "CUSTOM_CHALLENGE" === o ? (n.Session = r.Session, t.customChallenge(i)) : (n.signInUserSession = n.getCognitoUserSession(r.AuthenticationResult), n.cacheTokens(), t.onSuccess(n.signInUserSession))
                     }))
                 }, t.authenticateUser = function(e, t) {
                     return "USER_PASSWORD_AUTH" === this.authenticationFlowType ? this.authenticateUserPlainUsernamePassword(e, t) : "USER_SRP_AUTH" === this.authenticationFlowType || "CUSTOM_AUTH" === this.authenticationFlowType ? this.authenticateUserDefaultAuth(e, t) : t.onFailure(new Error("Authentication flow type is invalid."))
                 }, t.authenticateUserDefaultAuth = function(e, t) {
                     var n, r, o = this,
-                        i = new Tp(this.pool.getUserPoolName()),
-                        a = new Gp,
+                        i = new Op(this.pool.getUserPoolName()),
+                        a = new Hp,
                         s = {};
                     null != this.deviceKey && (s.DEVICE_KEY = this.deviceKey), s.USERNAME = this.username, i.getLargeAValue((function(u, l) {
                         u && t.onFailure(u), s.SRP_A = l.toString(16), "CUSTOM_AUTH" === o.authenticationFlowType && (s.CHALLENGE_NAME = "SRP_A");
                         var c = 0 !== Object.keys(e.getValidationData()).length ? e.getValidationData() : e.getClientMetadata(),
                             d = {
                                 AuthFlow: o.authenticationFlowType,
                                 ClientId: o.pool.getClientId(),
                                 AuthParameters: s,
                                 ClientMetadata: c
                             };
                         o.getUserContextData(o.username) && (d.UserContextData = o.getUserContextData(o.username)), o.client.request("InitiateAuth", d, (function(s, u) {
                             if (s) return t.onFailure(s);
                             var l = u.ChallengeParameters;
-                            o.username = l.USER_ID_FOR_SRP, o.userDataKey = o.keyPrefix + "." + o.username + ".userData", n = new Mp(l.SRP_B, 16), r = new Mp(l.SALT, 16), o.getCachedDeviceKeyAndPassword(), i.getPasswordAuthenticationKey(o.username, e.getPassword(), n, r, (function(e, n) {
+                            o.username = l.USER_ID_FOR_SRP, o.userDataKey = o.keyPrefix + "." + o.username + ".userData", n = new jp(l.SRP_B, 16), r = new jp(l.SALT, 16), o.getCachedDeviceKeyAndPassword(), i.getPasswordAuthenticationKey(o.username, e.getPassword(), n, r, (function(e, n) {
                                 e && t.onFailure(e);
                                 var r = a.getNowString(),
-                                    s = hp.lW.concat([hp.lW.from(o.pool.getUserPoolName(), "utf8"), hp.lW.from(o.username, "utf8"), hp.lW.from(l.SECRET_BLOCK, "base64"), hp.lW.from(r, "utf8")]),
-                                    d = new vp.Sha256(n);
+                                    s = yp.lW.concat([yp.lW.from(o.pool.getUserPoolName(), "utf8"), yp.lW.from(o.username, "utf8"), yp.lW.from(l.SECRET_BLOCK, "base64"), yp.lW.from(r, "utf8")]),
+                                    d = new bp.Sha256(n);
                                 d.update(s);
                                 var f = d.digestSync(),
-                                    p = hp.lW.from(f).toString("base64"),
+                                    p = yp.lW.from(f).toString("base64"),
                                     h = {};
                                 h.USERNAME = o.username, h.PASSWORD_CLAIM_SECRET_BLOCK = l.SECRET_BLOCK, h.TIMESTAMP = r, h.PASSWORD_CLAIM_SIGNATURE = p, null != o.deviceKey && (h.DEVICE_KEY = o.deviceKey);
                                 var g = {
                                     ChallengeName: "PASSWORD_VERIFIER",
                                     ClientId: o.pool.getClientId(),
                                     ChallengeResponses: h,
                                     Session: u.Session,
@@ -66519,15 +66547,15 @@
                             }))
                         }))
                     }))
                 }, t.authenticateUserPlainUsernamePassword = function(e, t) {
                     var n = this,
                         r = {};
                     if (r.USERNAME = this.username, r.PASSWORD = e.getPassword(), r.PASSWORD) {
-                        var o = new Tp(this.pool.getUserPoolName());
+                        var o = new Op(this.pool.getUserPoolName());
                         this.getCachedDeviceKeyAndPassword(), null != this.deviceKey && (r.DEVICE_KEY = this.deviceKey);
                         var i = 0 !== Object.keys(e.getValidationData()).length ? e.getValidationData() : e.getClientMetadata(),
                             a = {
                                 AuthFlow: "USER_PASSWORD_AUTH",
                                 ClientId: this.pool.getClientId(),
                                 AuthParameters: r,
                                 ClientMetadata: i
@@ -66558,30 +66586,30 @@
                     if ("DEVICE_SRP_AUTH" === o) return this.Session = e.Session, void this.getDeviceResponse(n);
                     this.signInUserSession = this.getCognitoUserSession(e.AuthenticationResult), this.challengeName = o, this.cacheTokens();
                     var d = e.AuthenticationResult.NewDeviceMetadata;
                     if (null == d) return n.onSuccess(this.signInUserSession);
                     t.generateHashDevice(e.AuthenticationResult.NewDeviceMetadata.DeviceGroupKey, e.AuthenticationResult.NewDeviceMetadata.DeviceKey, (function(o) {
                         if (o) return n.onFailure(o);
                         var i = {
-                            Salt: hp.lW.from(t.getSaltDevices(), "hex").toString("base64"),
-                            PasswordVerifier: hp.lW.from(t.getVerifierDevices(), "hex").toString("base64")
+                            Salt: yp.lW.from(t.getSaltDevices(), "hex").toString("base64"),
+                            PasswordVerifier: yp.lW.from(t.getVerifierDevices(), "hex").toString("base64")
                         };
                         r.verifierDevices = i.PasswordVerifier, r.deviceGroupKey = d.DeviceGroupKey, r.randomPassword = t.getRandomPassword(), r.client.request("ConfirmDevice", {
                             DeviceKey: d.DeviceKey,
                             AccessToken: r.signInUserSession.getAccessToken().getJwtToken(),
                             DeviceSecretVerifierConfig: i,
-                            DeviceName: qp
+                            DeviceName: Kp
                         }, (function(t, o) {
                             return t ? n.onFailure(t) : (r.deviceKey = e.AuthenticationResult.NewDeviceMetadata.DeviceKey, r.cacheDeviceKeyAndPassword(), !0 === o.UserConfirmationNecessary ? n.onSuccess(r.signInUserSession, o.UserConfirmationNecessary) : n.onSuccess(r.signInUserSession))
                         }))
                     }))
                 }, t.completeNewPasswordChallenge = function(e, t, n, r) {
                     var o = this;
                     if (!e) return n.onFailure(new Error("New password is required."));
-                    var i = new Tp(this.pool.getUserPoolName()),
+                    var i = new Op(this.pool.getUserPoolName()),
                         a = i.getNewPasswordRequiredChallengeUserAttributePrefix(),
                         s = {};
                     t && Object.keys(t).forEach((function(e) {
                         s[a + e] = t[e]
                     })), s.NEW_PASSWORD = e, s.USERNAME = this.username;
                     var u = {
                         ChallengeName: "NEW_PASSWORD_REQUIRED",
@@ -66591,39 +66619,39 @@
                         ClientMetadata: r
                     };
                     this.getUserContextData() && (u.UserContextData = this.getUserContextData()), this.client.request("RespondToAuthChallenge", u, (function(e, t) {
                         return e ? n.onFailure(e) : o.authenticateUserInternal(t, i, n)
                     }))
                 }, t.getDeviceResponse = function(e, t) {
                     var n = this,
-                        r = new Tp(this.deviceGroupKey),
-                        o = new Gp,
+                        r = new Op(this.deviceGroupKey),
+                        o = new Hp,
                         i = {};
                     i.USERNAME = this.username, i.DEVICE_KEY = this.deviceKey, r.getLargeAValue((function(a, s) {
                         a && e.onFailure(a), i.SRP_A = s.toString(16);
                         var u = {
                             ChallengeName: "DEVICE_SRP_AUTH",
                             ClientId: n.pool.getClientId(),
                             ChallengeResponses: i,
                             ClientMetadata: t,
                             Session: n.Session
                         };
                         n.getUserContextData() && (u.UserContextData = n.getUserContextData()), n.client.request("RespondToAuthChallenge", u, (function(t, i) {
                             if (t) return e.onFailure(t);
                             var a = i.ChallengeParameters,
-                                s = new Mp(a.SRP_B, 16),
-                                u = new Mp(a.SALT, 16);
+                                s = new jp(a.SRP_B, 16),
+                                u = new jp(a.SALT, 16);
                             r.getPasswordAuthenticationKey(n.deviceKey, n.randomPassword, s, u, (function(t, r) {
                                 if (t) return e.onFailure(t);
                                 var s = o.getNowString(),
-                                    u = hp.lW.concat([hp.lW.from(n.deviceGroupKey, "utf8"), hp.lW.from(n.deviceKey, "utf8"), hp.lW.from(a.SECRET_BLOCK, "base64"), hp.lW.from(s, "utf8")]),
-                                    l = new vp.Sha256(r);
+                                    u = yp.lW.concat([yp.lW.from(n.deviceGroupKey, "utf8"), yp.lW.from(n.deviceKey, "utf8"), yp.lW.from(a.SECRET_BLOCK, "base64"), yp.lW.from(s, "utf8")]),
+                                    l = new bp.Sha256(r);
                                 l.update(u);
                                 var c = l.digestSync(),
-                                    d = hp.lW.from(c).toString("base64"),
+                                    d = yp.lW.from(c).toString("base64"),
                                     f = {};
                                 f.USERNAME = n.username, f.PASSWORD_CLAIM_SECRET_BLOCK = a.SECRET_BLOCK, f.TIMESTAMP = s, f.PASSWORD_CLAIM_SIGNATURE = d, f.DEVICE_KEY = n.deviceKey;
                                 var p = {
                                     ChallengeName: "DEVICE_PASSWORD_VERIFIER",
                                     ClientId: n.pool.getClientId(),
                                     ChallengeResponses: f,
                                     Session: i.Session
@@ -66645,15 +66673,15 @@
                     this.getUserContextData() && (o.UserContextData = this.getUserContextData()), this.client.request("ConfirmSignUp", o, (function(e) {
                         return e ? n(e, null) : n(null, "SUCCESS")
                     }))
                 }, t.sendCustomChallengeAnswer = function(e, t, n) {
                     var r = this,
                         o = {};
                     o.USERNAME = this.username, o.ANSWER = e;
-                    var i = new Tp(this.pool.getUserPoolName());
+                    var i = new Op(this.pool.getUserPoolName());
                     this.getCachedDeviceKeyAndPassword(), null != this.deviceKey && (o.DEVICE_KEY = this.deviceKey);
                     var a = {
                         ChallengeName: "CUSTOM_CHALLENGE",
                         ChallengeResponses: o,
                         ClientId: this.pool.getClientId(),
                         Session: this.Session,
                         ClientMetadata: n
@@ -66674,26 +66702,26 @@
                         Session: this.Session,
                         ClientMetadata: r
                     };
                     this.getUserContextData() && (s.UserContextData = this.getUserContextData()), this.client.request("RespondToAuthChallenge", s, (function(e, n) {
                         if (e) return t.onFailure(e);
                         if ("DEVICE_SRP_AUTH" !== n.ChallengeName) {
                             if (o.signInUserSession = o.getCognitoUserSession(n.AuthenticationResult), o.cacheTokens(), null == n.AuthenticationResult.NewDeviceMetadata) return t.onSuccess(o.signInUserSession);
-                            var r = new Tp(o.pool.getUserPoolName());
+                            var r = new Op(o.pool.getUserPoolName());
                             r.generateHashDevice(n.AuthenticationResult.NewDeviceMetadata.DeviceGroupKey, n.AuthenticationResult.NewDeviceMetadata.DeviceKey, (function(e) {
                                 if (e) return t.onFailure(e);
                                 var i = {
-                                    Salt: hp.lW.from(r.getSaltDevices(), "hex").toString("base64"),
-                                    PasswordVerifier: hp.lW.from(r.getVerifierDevices(), "hex").toString("base64")
+                                    Salt: yp.lW.from(r.getSaltDevices(), "hex").toString("base64"),
+                                    PasswordVerifier: yp.lW.from(r.getVerifierDevices(), "hex").toString("base64")
                                 };
                                 o.verifierDevices = i.PasswordVerifier, o.deviceGroupKey = n.AuthenticationResult.NewDeviceMetadata.DeviceGroupKey, o.randomPassword = r.getRandomPassword(), o.client.request("ConfirmDevice", {
                                     DeviceKey: n.AuthenticationResult.NewDeviceMetadata.DeviceKey,
                                     AccessToken: o.signInUserSession.getAccessToken().getJwtToken(),
                                     DeviceSecretVerifierConfig: i,
-                                    DeviceName: qp
+                                    DeviceName: Kp
                                 }, (function(e, r) {
                                     return e ? t.onFailure(e) : (o.deviceKey = n.AuthenticationResult.NewDeviceMetadata.DeviceKey, o.cacheDeviceKeyAndPassword(), !0 === r.UserConfirmationNecessary ? t.onSuccess(o.signInUserSession, r.UserConfirmationNecessary) : t.onSuccess(o.signInUserSession))
                                 }))
                             }))
                         } else o.getDeviceResponse(t)
                     }))
                 }, t.changePassword = function(e, t, n, r) {
@@ -66765,15 +66793,15 @@
                     }, (function(t, n) {
                         if (t) return e(t, null);
                         for (var r = [], o = 0; o < n.UserAttributes.length; o++) {
                             var i = {
                                     Name: n.UserAttributes[o].Name,
                                     Value: n.UserAttributes[o].Value
                                 },
-                                a = new Wp(i);
+                                a = new Zp(i);
                             r.push(a)
                         }
                         return e(null, r)
                     }))
                 }, t.getMFAOptions = function(e) {
                     if (null == this.signInUserSession || !this.signInUserSession.isValid()) return e(new Error("User is not authenticated"), null);
                     this.client.request("GetUser", {
@@ -66847,25 +66875,25 @@
                     if (null != this.signInUserSession && this.signInUserSession.isValid()) return e(null, this.signInUserSession);
                     var n = "CognitoIdentityServiceProvider." + this.pool.getClientId() + "." + this.username,
                         r = n + ".idToken",
                         o = n + ".accessToken",
                         i = n + ".refreshToken",
                         a = n + ".clockDrift";
                     if (this.storage.getItem(r)) {
-                        var s = new Pp({
+                        var s = new Bp({
                                 IdToken: this.storage.getItem(r)
                             }),
-                            u = new zp({
+                            u = new Pp({
                                 AccessToken: this.storage.getItem(o)
                             }),
-                            l = new Rp({
+                            l = new Fp({
                                 RefreshToken: this.storage.getItem(i)
                             }),
                             c = parseInt(this.storage.getItem(a), 0) || 0,
-                            d = new Fp({
+                            d = new Qp({
                                 IdToken: s,
                                 AccessToken: u,
                                 RefreshToken: l,
                                 ClockDrift: c
                             });
                         if (d.isValid()) return this.signInUserSession = d, e(null, this.signInUserSession);
                         if (!l.getToken()) return e(new Error("Cannot retrieve a new session. Please authenticate."), null);
@@ -66933,18 +66961,18 @@
                         t = e + "." + this.username + ".idToken",
                         n = e + "." + this.username + ".accessToken",
                         r = e + "." + this.username + ".refreshToken",
                         o = e + ".LastAuthUser",
                         i = e + "." + this.username + ".clockDrift";
                     this.storage.removeItem(t), this.storage.removeItem(n), this.storage.removeItem(r), this.storage.removeItem(o), this.storage.removeItem(i)
                 }, t.getCognitoUserSession = function(e) {
-                    var t = new Pp(e),
-                        n = new zp(e),
-                        r = new Rp(e);
-                    return new Fp({
+                    var t = new Bp(e),
+                        n = new Pp(e),
+                        r = new Fp(e);
+                    return new Qp({
                         IdToken: t,
                         AccessToken: n,
                         RefreshToken: r
                     })
                 }, t.forgotPassword = function(e, t) {
                     var n = {
                         ClientId: this.pool.getClientId(),
@@ -67131,106 +67159,106 @@
                             return e ? n.onFailure(e) : (r.signInUserSession = r.getCognitoUserSession(t.AuthenticationResult), r.cacheTokens(), n.onSuccess(r.signInUserSession))
                         }))
                     }))
                 }, e
             }();
         __webpack_require__(8117);
 
-        function Kp() {}
-        Kp.prototype.userAgent = Bp.userAgent;
-        var Xp = Kp;
+        function $p() {}
+        $p.prototype.userAgent = Yp.userAgent;
+        var eh = $p;
 
-        function $p(e, t) {
-            e.prototype = Object.create(t.prototype), e.prototype.constructor = e, rh(e, t)
+        function th(e, t) {
+            e.prototype = Object.create(t.prototype), e.prototype.constructor = e, ih(e, t)
         }
 
-        function eh(e) {
+        function nh(e) {
             var t = "function" === typeof Map ? new Map : void 0;
-            return eh = function(e) {
+            return nh = function(e) {
                 if (null === e || (n = e, -1 === Function.toString.call(n).indexOf("[native code]"))) return e;
                 var n;
                 if ("function" !== typeof e) throw new TypeError("Super expression must either be null or a function");
                 if ("undefined" !== typeof t) {
                     if (t.has(e)) return t.get(e);
                     t.set(e, r)
                 }
 
                 function r() {
-                    return th(e, arguments, oh(this).constructor)
+                    return rh(e, arguments, ah(this).constructor)
                 }
                 return r.prototype = Object.create(e.prototype, {
                     constructor: {
                         value: r,
                         enumerable: !1,
                         writable: !0,
                         configurable: !0
                     }
-                }), rh(r, e)
-            }, eh(e)
+                }), ih(r, e)
+            }, nh(e)
         }
 
-        function th(e, t, n) {
-            return th = nh() ? Reflect.construct.bind() : function(e, t, n) {
+        function rh(e, t, n) {
+            return rh = oh() ? Reflect.construct.bind() : function(e, t, n) {
                 var r = [null];
                 r.push.apply(r, t);
                 var o = new(Function.bind.apply(e, r));
-                return n && rh(o, n.prototype), o
-            }, th.apply(null, arguments)
+                return n && ih(o, n.prototype), o
+            }, rh.apply(null, arguments)
         }
 
-        function nh() {
+        function oh() {
             if ("undefined" === typeof Reflect || !Reflect.construct) return !1;
             if (Reflect.construct.sham) return !1;
             if ("function" === typeof Proxy) return !0;
             try {
                 return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
             } catch (e) {
                 return !1
             }
         }
 
-        function rh(e, t) {
-            return rh = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
+        function ih(e, t) {
+            return ih = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
                 return e.__proto__ = t, e
-            }, rh(e, t)
+            }, ih(e, t)
         }
 
-        function oh(e) {
-            return oh = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(e) {
+        function ah(e) {
+            return ah = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(e) {
                 return e.__proto__ || Object.getPrototypeOf(e)
-            }, oh(e)
+            }, ah(e)
         }
-        var ih = function(e) {
+        var sh = function(e) {
                 function t(t, n, r, o) {
                     var i;
                     return (i = e.call(this, t) || this).code = n, i.name = r, i.statusCode = o, i
                 }
-                return $p(t, e), t
-            }(eh(Error)),
-            ah = function() {
+                return th(t, e), t
+            }(nh(Error)),
+            uh = function() {
                 function e(e, t, n) {
                     this.endpoint = t || "https://cognito-idp." + e + ".amazonaws.com/";
                     var r = (n || {}).credentials;
                     this.fetchOptions = r ? {
                         credentials: r
                     } : {}
                 }
                 var t = e.prototype;
                 return t.promisifyRequest = function(e, t) {
                     var n = this;
                     return new Promise((function(r, o) {
                         n.request(e, t, (function(e, t) {
-                            e ? o(new ih(e.message, e.code, e.name, e.statusCode)) : r(t)
+                            e ? o(new sh(e.message, e.code, e.name, e.statusCode)) : r(t)
                         }))
                     }))
                 }, t.requestWithRetry = function(e, t, n) {
                     var r = this;
                     (function(e, t, n) {
-                        void 0 === n && (n = lh);
-                        return uh(e, t, function(e) {
+                        void 0 === n && (n = dh);
+                        return ch(e, t, function(e) {
                             var t = 100,
                                 n = 100;
                             return function(r) {
                                 var o = Math.pow(2, r) * t + n * Math.random();
                                 return !(o > e) && o
                             }
                         }(n))
@@ -67245,15 +67273,15 @@
                     })).catch((function(e) {
                         return n(e)
                     }))
                 }, t.request = function(e, t, n) {
                     var r, o = {
                             "Content-Type": "application/x-amz-json-1.1",
                             "X-Amz-Target": "AWSCognitoIdentityProviderService." + e,
-                            "X-Amz-User-Agent": Xp.prototype.userAgent,
+                            "X-Amz-User-Agent": eh.prototype.userAgent,
                             "Cache-Control": "no-store"
                         },
                         i = Object.assign({}, this.fetchOptions, {
                             headers: o,
                             method: "POST",
                             mode: "cors",
                             body: JSON.stringify(t)
@@ -67281,43 +67309,43 @@
                         } catch (i) {
                             return n(e)
                         } else e instanceof Error && "Network error" === e.message && (e.code = "NetworkError");
                         return n(e)
                     }))
                 }, e
             }(),
-            sh = function() {};
+            lh = function() {};
         Error;
 
-        function uh(e, t, n, r) {
+        function ch(e, t, n, r) {
             if (void 0 === r && (r = 1), "function" !== typeof e) throw Error("functionToRetry must be a function");
-            return sh(e.name + " attempt #" + r + " with args: " + JSON.stringify(t)), e.apply(void 0, t).catch((function(o) {
-                if (sh("error on " + e.name, o), (i = o) && i.nonRetryable) throw sh(e.name + " non retryable error", o), o;
+            return lh(e.name + " attempt #" + r + " with args: " + JSON.stringify(t)), e.apply(void 0, t).catch((function(o) {
+                if (lh("error on " + e.name, o), (i = o) && i.nonRetryable) throw lh(e.name + " non retryable error", o), o;
                 var i, a = n(r, t, o);
-                if (sh(e.name + " retrying in " + a + " ms"), !1 !== a) return new Promise((function(e) {
+                if (lh(e.name + " retrying in " + a + " ms"), !1 !== a) return new Promise((function(e) {
                     return setTimeout(e, a)
                 })).then((function() {
-                    return uh(e, t, n, r + 1)
+                    return ch(e, t, n, r + 1)
                 }));
                 throw o
             }))
         }
-        var lh = 3e5;
-        var ch, dh = function() {
+        var dh = 3e5;
+        var fh, ph = function() {
                 function e(e, t) {
                     var n = e || {},
                         r = n.UserPoolId,
                         o = n.ClientId,
                         i = n.endpoint,
                         a = n.fetchOptions,
                         s = n.AdvancedSecurityDataCollectionFlag;
                     if (!r || !o) throw new Error("Both UserPoolId and ClientId are required.");
                     if (r.length > 55 || !/^[\w-]+_[0-9a-zA-Z]+$/.test(r)) throw new Error("Invalid UserPoolId format.");
                     var u = r.split("_")[0];
-                    this.userPoolId = r, this.clientId = o, this.client = new ah(u, i, a), this.advancedSecurityDataCollectionFlag = !1 !== s, this.storage = e.Storage || (new Vp).getStorage(), t && (this.wrapRefreshSessionCallback = t)
+                    this.userPoolId = r, this.clientId = o, this.client = new uh(u, i, a), this.advancedSecurityDataCollectionFlag = !1 !== s, this.storage = e.Storage || (new Jp).getStorage(), t && (this.wrapRefreshSessionCallback = t)
                 }
                 var t = e.prototype;
                 return t.getUserPoolId = function() {
                     return this.userPoolId
                 }, t.getUserPoolName = function() {
                     return this.getUserPoolId().split("_")[1]
                 }, t.getClientId = function() {
@@ -67336,15 +67364,15 @@
                         if (t) return o(t, null);
                         var r = {
                                 Username: e,
                                 Pool: a,
                                 Storage: a.storage
                             },
                             i = {
-                                user: new Jp(r),
+                                user: new Xp(r),
                                 userConfirmed: n.UserConfirmed,
                                 userSub: n.UserSub,
                                 codeDeliveryDetails: n.CodeDeliveryDetails
                             };
                         return o(null, i)
                     }))
                 }, t.getCurrentUser = function() {
@@ -67352,15 +67380,15 @@
                         t = this.storage.getItem(e);
                     if (t) {
                         var n = {
                             Username: t,
                             Pool: this,
                             Storage: this.storage
                         };
-                        return new Jp(n)
+                        return new Xp(n)
                     }
                     return null
                 }, t.getUserContextData = function(e) {
                     if ("undefined" !== typeof AmazonCognitoAdvancedSecurityData) {
                         var t = AmazonCognitoAdvancedSecurityData;
                         if (this.advancedSecurityDataCollectionFlag) {
                             var n = t.getData(e, this.userPoolId, this.clientId);
@@ -67368,16 +67396,16 @@
                                 EncodedData: n
                             }
                         }
                         return {}
                     }
                 }, e
             }(),
-            fh = __webpack_require__(5943),
-            ph = function() {
+            hh = __webpack_require__(5943),
+            gh = function() {
                 function e(e) {
                     if (!e.domain) throw new Error("The domain of cookieStorage can not be undefined.");
                     if (this.domain = e.domain, e.path ? this.path = e.path : this.path = "/", Object.prototype.hasOwnProperty.call(e, "expires") ? this.expires = e.expires : this.expires = 365, Object.prototype.hasOwnProperty.call(e, "secure") ? this.secure = e.secure : this.secure = !0, Object.prototype.hasOwnProperty.call(e, "sameSite")) {
                         if (!["strict", "lax", "none"].includes(e.sameSite)) throw new Error('The sameSite value of cookieStorage must be "lax", "strict" or "none".');
                         if ("none" === e.sameSite && !this.secure) throw new Error("sameSite = None requires the Secure attribute in latest browser versions.");
                         this.sameSite = e.sameSite
                     } else this.sameSite = null
@@ -67386,116 +67414,116 @@
                 return t.setItem = function(e, t) {
                     var n = {
                         path: this.path,
                         expires: this.expires,
                         domain: this.domain,
                         secure: this.secure
                     };
-                    return this.sameSite && (n.sameSite = this.sameSite), fh.set(e, t, n), fh.get(e)
+                    return this.sameSite && (n.sameSite = this.sameSite), hh.set(e, t, n), hh.get(e)
                 }, t.getItem = function(e) {
-                    return fh.get(e)
+                    return hh.get(e)
                 }, t.removeItem = function(e) {
                     var t = {
                         path: this.path,
                         expires: this.expires,
                         domain: this.domain,
                         secure: this.secure
                     };
-                    return this.sameSite && (t.sameSite = this.sameSite), fh.remove(e, t)
+                    return this.sameSite && (t.sameSite = this.sameSite), hh.remove(e, t)
                 }, t.clear = function() {
-                    for (var e = fh.get(), t = Object.keys(e).length, n = 0; n < t; ++n) this.removeItem(Object.keys(e)[n]);
+                    for (var e = hh.get(), t = Object.keys(e).length, n = 0; n < t; ++n) this.removeItem(Object.keys(e)[n]);
                     return {}
                 }, e
             }(),
-            hh = __webpack_require__(2770),
-            gh = function(e) {
+            yh = __webpack_require__(2770),
+            mh = function(e) {
                 var t = window.open(e, "_self");
                 return t ? Promise.resolve(t) : Promise.reject()
             },
-            yh = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default",
-            mh = function(e, t, n) {
-                qs.dispatch("auth", {
+            vh = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default",
+            Mh = function(e, t, n) {
+                Ks.dispatch("auth", {
                     event: e,
                     data: t,
                     message: n
-                }, "Auth", yh)
+                }, "Auth", vh)
             },
-            vh = new Ws("OAuth"),
-            Mh = function() {
+            bh = new Zs("OAuth"),
+            jh = function() {
                 function e(e) {
                     var t = e.config,
                         n = e.cognitoClientId,
                         r = e.scopes,
                         o = void 0 === r ? [] : r;
-                    if (this._urlOpener = t.urlOpener || gh, this._config = t, this._cognitoClientId = n, !this.isValidScopes(o)) throw Error("scopes must be a String Array");
+                    if (this._urlOpener = t.urlOpener || mh, this._config = t, this._cognitoClientId = n, !this.isValidScopes(o)) throw Error("scopes must be a String Array");
                     this._scopes = o
                 }
                 return e.prototype.isValidScopes = function(e) {
                     return Array.isArray(e) && e.every((function(e) {
                         return "string" === typeof e
                     }))
                 }, e.prototype.oauthSignIn = function(e, t, n, r, o, i) {
-                    void 0 === e && (e = "code"), void 0 === o && (o = Ss.Cognito);
+                    void 0 === e && (e = "code"), void 0 === o && (o = ks.Cognito);
                     var a = this._generateState(32),
                         s = i ? a + "-" + i.split("").map((function(e) {
                             return e.charCodeAt(0).toString(16).padStart(2, "0")
                         })).join("") : a;
                     ! function(e) {
                         window.sessionStorage.setItem("oauth_state", e)
                     }(s);
                     var u, l = this._generateRandom(128);
                     u = l, window.sessionStorage.setItem("ouath_pkce_key", u);
                     var c = this._generateChallenge(l),
                         d = this._scopes.join(" "),
-                        f = Object.entries(Cs(Cs({
+                        f = Object.entries(_s(_s({
                             redirect_uri: n,
                             response_type: e,
                             client_id: r,
                             identity_provider: o,
                             scope: d,
                             state: s
                         }, "code" === e ? {
                             code_challenge: c
                         } : {}), "code" === e ? {
                             code_challenge_method: "S256"
                         } : {})).map((function(e) {
-                            var t = Ts(e, 2),
+                            var t = Os(e, 2),
                                 n = t[0],
                                 r = t[1];
                             return encodeURIComponent(n) + "=" + encodeURIComponent(r)
                         })).join("&"),
                         p = "https://" + t + "/oauth2/authorize?" + f;
-                    vh.debug("Redirecting to " + p), this._urlOpener(p, n)
+                    bh.debug("Redirecting to " + p), this._urlOpener(p, n)
                 }, e.prototype._handleCodeFlow = function(e) {
-                    return Es(this, void 0, void 0, (function() {
+                    return Ts(this, void 0, void 0, (function() {
                         var t, n, r, o, i, a, s, u, l, c, d, f, p, h;
-                        return _s(this, (function(g) {
+                        return As(this, (function(g) {
                             switch (g.label) {
                                 case 0:
-                                    return t = ((0, hh.Qc)(e).query || "").split("&").map((function(e) {
+                                    return t = ((0, yh.Qc)(e).query || "").split("&").map((function(e) {
                                         return e.split("=")
                                     })).reduce((function(e, t) {
-                                        var n, r = Ts(t, 2),
+                                        var n, r = Os(t, 2),
                                             o = r[0],
                                             i = r[1];
-                                        return Cs(Cs({}, e), ((n = {})[o] = i, n))
+                                        return _s(_s({}, e), ((n = {})[o] = i, n))
                                     }), {
                                         code: void 0
-                                    }).code, n = (0, hh.Qc)(e).pathname || "/", r = (0, hh.Qc)(this._config.redirectSignIn).pathname || "/", t && n === r ? (o = "https://" + this._config.domain + "/oauth2/token", mh("codeFlow", {}, "Retrieving tokens from " + o), i = Os(this._config) ? this._cognitoClientId : this._config.clientID, a = Os(this._config) ? this._config.redirectSignIn : this._config.redirectUri, s = function() {
+                                    }).code, n = (0, yh.Qc)(e).pathname || "/", r = (0, yh.Qc)(this._config.redirectSignIn).pathname || "/", t && n === r ? (o = "https://" + this._config.domain + "/oauth2/token", Mh("codeFlow", {}, "Retrieving tokens from " + o), i = Us(this._config) ? this._cognitoClientId : this._config.clientID, a = Us(this._config) ? this._config.redirectSignIn : this._config.redirectUri, s = function() {
                                         var e = window.sessionStorage.getItem("ouath_pkce_key");
                                         return window.sessionStorage.removeItem("ouath_pkce_key"), e
-                                    }(), u = Cs({
+                                    }(), u = _s({
                                         grant_type: "authorization_code",
                                         code: t,
                                         client_id: i,
                                         redirect_uri: a
                                     }, s ? {
                                         code_verifier: s
-                                    } : {}), vh.debug("Calling token endpoint: " + o + " with", u), l = Object.entries(u).map((function(e) {
-                                        var t = Ts(e, 2),
+                                    } : {}), bh.debug("Calling token endpoint: " + o + " with", u), l = Object.entries(u).map((function(e) {
+                                        var t = Os(e, 2),
                                             n = t[0],
                                             r = t[1];
                                         return encodeURIComponent(n) + "=" + encodeURIComponent(r)
                                     })).join("&"), [4, fetch(o, {
                                         method: "POST",
                                         headers: {
                                             "Content-Type": "application/x-www-form-urlencoded"
@@ -67511,70 +67539,70 @@
                                         refreshToken: f,
                                         idToken: p
                                     }]
                             }
                         }))
                     }))
                 }, e.prototype._handleImplicitFlow = function(e) {
-                    return Es(this, void 0, void 0, (function() {
+                    return Ts(this, void 0, void 0, (function() {
                         var t, n, r;
-                        return _s(this, (function(o) {
-                            return t = ((0, hh.Qc)(e).hash || "#").substr(1).split("&").map((function(e) {
+                        return As(this, (function(o) {
+                            return t = ((0, yh.Qc)(e).hash || "#").substr(1).split("&").map((function(e) {
                                 return e.split("=")
                             })).reduce((function(e, t) {
-                                var n, r = Ts(t, 2),
+                                var n, r = Os(t, 2),
                                     o = r[0],
                                     i = r[1];
-                                return Cs(Cs({}, e), ((n = {})[o] = i, n))
+                                return _s(_s({}, e), ((n = {})[o] = i, n))
                             }), {
                                 id_token: void 0,
                                 access_token: void 0
-                            }), n = t.id_token, r = t.access_token, mh("implicitFlow", {}, "Got tokens from " + e), vh.debug("Retrieving implicit tokens from " + e + " with"), [2, {
+                            }), n = t.id_token, r = t.access_token, Mh("implicitFlow", {}, "Got tokens from " + e), bh.debug("Retrieving implicit tokens from " + e + " with"), [2, {
                                 accessToken: r,
                                 idToken: n,
                                 refreshToken: null
                             }]
                         }))
                     }))
                 }, e.prototype.handleAuthResponse = function(e) {
-                    return Es(this, void 0, void 0, (function() {
+                    return Ts(this, void 0, void 0, (function() {
                         var t, n, r, o, i, a, s;
-                        return _s(this, (function(u) {
+                        return As(this, (function(u) {
                             switch (u.label) {
                                 case 0:
-                                    if (u.trys.push([0, 5, , 6]), t = e ? Cs(Cs({}, ((0, hh.Qc)(e).hash || "#").substr(1).split("&").map((function(e) {
+                                    if (u.trys.push([0, 5, , 6]), t = e ? _s(_s({}, ((0, yh.Qc)(e).hash || "#").substr(1).split("&").map((function(e) {
                                             return e.split("=")
                                         })).reduce((function(e, t) {
-                                            var n = Ts(t, 2),
+                                            var n = Os(t, 2),
                                                 r = n[0],
                                                 o = n[1];
                                             return e[r] = o, e
-                                        }), {})), ((0, hh.Qc)(e).query || "").split("&").map((function(e) {
+                                        }), {})), ((0, yh.Qc)(e).query || "").split("&").map((function(e) {
                                             return e.split("=")
                                         })).reduce((function(e, t) {
-                                            var n = Ts(t, 2),
+                                            var n = Os(t, 2),
                                                 r = n[0],
                                                 o = n[1];
                                             return e[r] = o, e
                                         }), {})) : {}, n = t.error, r = t.error_description, n) throw new Error(r);
-                                    return o = this._validateState(t), vh.debug("Starting " + this._config.responseType + " flow with " + e), "code" !== this._config.responseType ? [3, 2] : (i = [{}], [4, this._handleCodeFlow(e)]);
+                                    return o = this._validateState(t), bh.debug("Starting " + this._config.responseType + " flow with " + e), "code" !== this._config.responseType ? [3, 2] : (i = [{}], [4, this._handleCodeFlow(e)]);
                                 case 1:
-                                    return [2, Cs.apply(void 0, [Cs.apply(void 0, i.concat([u.sent()])), {
+                                    return [2, _s.apply(void 0, [_s.apply(void 0, i.concat([u.sent()])), {
                                         state: o
                                     }])];
                                 case 2:
                                     return a = [{}], [4, this._handleImplicitFlow(e)];
                                 case 3:
-                                    return [2, Cs.apply(void 0, [Cs.apply(void 0, a.concat([u.sent()])), {
+                                    return [2, _s.apply(void 0, [_s.apply(void 0, a.concat([u.sent()])), {
                                         state: o
                                     }])];
                                 case 4:
                                     return [3, 6];
                                 case 5:
-                                    throw s = u.sent(), vh.error("Error handling auth response.", s), s;
+                                    throw s = u.sent(), bh.error("Error handling auth response.", s), s;
                                 case 6:
                                     return [2]
                             }
                         }))
                     }))
                 }, e.prototype._validateState = function(e) {
                     if (e) {
@@ -67583,33 +67611,33 @@
                                 return window.sessionStorage.removeItem("oauth_state"), e
                             }(),
                             n = e.state;
                         if (t && t !== n) throw new Error("Invalid state in OAuth flow");
                         return n
                     }
                 }, e.prototype.signOut = function() {
-                    return Es(this, void 0, void 0, (function() {
+                    return Ts(this, void 0, void 0, (function() {
                         var e, t, n;
-                        return _s(this, (function(r) {
-                            return e = "https://" + this._config.domain + "/logout?", t = Os(this._config) ? this._cognitoClientId : this._config.oauth.clientID, n = Os(this._config) ? this._config.redirectSignOut : this._config.returnTo, e += Object.entries({
+                        return As(this, (function(r) {
+                            return e = "https://" + this._config.domain + "/logout?", t = Us(this._config) ? this._cognitoClientId : this._config.oauth.clientID, n = Us(this._config) ? this._config.redirectSignOut : this._config.returnTo, e += Object.entries({
                                 client_id: t,
                                 logout_uri: encodeURIComponent(n)
                             }).map((function(e) {
-                                var t = Ts(e, 2);
+                                var t = Os(e, 2);
                                 return t[0] + "=" + t[1]
-                            })).join("&"), mh("oAuthSignOut", {
+                            })).join("&"), Mh("oAuthSignOut", {
                                 oAuth: "signOut"
-                            }, "Signing out from " + e), vh.debug("Signing out from " + e), [2, this._urlOpener(e, n)]
+                            }, "Signing out from " + e), bh.debug("Signing out from " + e), [2, this._urlOpener(e, n)]
                         }))
                     }))
                 }, e.prototype._generateState = function(e) {
                     for (var t = "", n = e, r = "0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ"; n > 0; --n) t += r[Math.round(Math.random() * (r.length - 1))];
                     return t
                 }, e.prototype._generateChallenge = function(e) {
-                    var t = new vp.Sha256;
+                    var t = new bp.Sha256;
                     t.update(e);
                     var n = t.digestSync(),
                         r = nt.lW.from(n).toString("base64");
                     return this._base64URL(r)
                 }, e.prototype._base64URL = function(e) {
                     return e.replace(/=/g, "").replace(/\+/g, "-").replace(/\//g, "_")
                 }, e.prototype._generateRandom = function(e) {
@@ -67622,104 +67650,104 @@
                     for (var t = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789", n = [], r = 0; r < e.byteLength; r += 1) {
                         var o = e[r] % t.length;
                         n.push(t[o])
                     }
                     return n.join("")
                 }, e
             }(),
-            bh = Mh;
+            wh = jh;
         ! function(e) {
             e.DEFAULT_MSG = "Authentication Error", e.EMPTY_EMAIL = "Email cannot be empty", e.EMPTY_PHONE = "Phone number cannot be empty", e.EMPTY_USERNAME = "Username cannot be empty", e.INVALID_USERNAME = "The username should either be a string or one of the sign in types", e.EMPTY_PASSWORD = "Password cannot be empty", e.EMPTY_CODE = "Confirmation code cannot be empty", e.SIGN_UP_ERROR = "Error creating account", e.NO_MFA = "No valid MFA method provided", e.INVALID_MFA = "Invalid MFA type", e.EMPTY_CHALLENGE = "Challenge response cannot be empty", e.NO_USER_SESSION = "Failed to get the session because the user is empty", e.NETWORK_ERROR = "Network Error", e.DEVICE_CONFIG = "Device tracking has not been configured in this User Pool", e.AUTOSIGNIN_ERROR = "Please use your credentials to sign in"
-        }(ch || (ch = {}));
-        var jh = new Ws("AuthError"),
-            wh = function(e) {
+        }(fh || (fh = {}));
+        var xh = new Zs("AuthError"),
+            Nh = function(e) {
                 function t(n) {
                     var r = this,
-                        o = Nh[n],
+                        o = Dh[n],
                         i = o.message,
                         a = o.log;
-                    return (r = e.call(this, i) || this).constructor = t, Object.setPrototypeOf(r, t.prototype), r.name = "AuthError", r.log = a || i, jh.error(r.log), r
+                    return (r = e.call(this, i) || this).constructor = t, Object.setPrototypeOf(r, t.prototype), r.name = "AuthError", r.log = a || i, xh.error(r.log), r
                 }
-                return Ds(t, e), t
+                return Ls(t, e), t
             }(Error),
-            xh = function(e) {
+            Ih = function(e) {
                 function t(n) {
                     var r = e.call(this, n) || this;
                     return r.constructor = t, Object.setPrototypeOf(r, t.prototype), r.name = "NoUserPoolError", r
                 }
-                return Ds(t, e), t
-            }(wh),
-            Nh = {
+                return Ls(t, e), t
+            }(Nh),
+            Dh = {
                 noConfig: {
-                    message: ch.DEFAULT_MSG,
+                    message: fh.DEFAULT_MSG,
                     log: "\n            Error: Amplify has not been configured correctly.\n            This error is typically caused by one of the following scenarios:\n\n            1. Make sure you're passing the awsconfig object to Amplify.configure() in your app's entry point\n                See https://aws-amplify.github.io/docs/js/authentication#configure-your-app for more information\n            \n            2. There might be multiple conflicting versions of amplify packages in your node_modules.\n\t\t\t\tRefer to our docs site for help upgrading Amplify packages (https://docs.amplify.aws/lib/troubleshooting/upgrading/q/platform/js)\n        "
                 },
                 missingAuthConfig: {
-                    message: ch.DEFAULT_MSG,
+                    message: fh.DEFAULT_MSG,
                     log: "\n            Error: Amplify has not been configured correctly. \n            The configuration object is missing required auth properties.\n            This error is typically caused by one of the following scenarios:\n\n            1. Did you run `amplify push` after adding auth via `amplify add auth`?\n                See https://aws-amplify.github.io/docs/js/authentication#amplify-project-setup for more information\n\n            2. This could also be caused by multiple conflicting versions of amplify packages, see (https://docs.amplify.aws/lib/troubleshooting/upgrading/q/platform/js) for help upgrading Amplify packages.\n        "
                 },
                 emptyUsername: {
-                    message: ch.EMPTY_USERNAME
+                    message: fh.EMPTY_USERNAME
                 },
                 invalidUsername: {
-                    message: ch.INVALID_USERNAME
+                    message: fh.INVALID_USERNAME
                 },
                 emptyPassword: {
-                    message: ch.EMPTY_PASSWORD
+                    message: fh.EMPTY_PASSWORD
                 },
                 emptyCode: {
-                    message: ch.EMPTY_CODE
+                    message: fh.EMPTY_CODE
                 },
                 signUpError: {
-                    message: ch.SIGN_UP_ERROR,
+                    message: fh.SIGN_UP_ERROR,
                     log: "The first parameter should either be non-null string or object"
                 },
                 noMFA: {
-                    message: ch.NO_MFA
+                    message: fh.NO_MFA
                 },
                 invalidMFA: {
-                    message: ch.INVALID_MFA
+                    message: fh.INVALID_MFA
                 },
                 emptyChallengeResponse: {
-                    message: ch.EMPTY_CHALLENGE
+                    message: fh.EMPTY_CHALLENGE
                 },
                 noUserSession: {
-                    message: ch.NO_USER_SESSION
+                    message: fh.NO_USER_SESSION
                 },
                 deviceConfig: {
-                    message: ch.DEVICE_CONFIG
+                    message: fh.DEVICE_CONFIG
                 },
                 networkError: {
-                    message: ch.NETWORK_ERROR
+                    message: fh.NETWORK_ERROR
                 },
                 autoSignInError: {
-                    message: ch.AUTOSIGNIN_ERROR
+                    message: fh.AUTOSIGNIN_ERROR
                 },
                 default: {
-                    message: ch.DEFAULT_MSG
+                    message: fh.DEFAULT_MSG
                 }
             },
-            Ih = new Ws("AuthClass"),
-            Dh = "aws.cognito.signin.user.admin",
-            Sh = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default",
-            Lh = function(e, t, n) {
-                qs.dispatch("auth", {
+            Sh = new Zs("AuthClass"),
+            Lh = "aws.cognito.signin.user.admin",
+            kh = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default",
+            Ch = function(e, t, n) {
+                Ks.dispatch("auth", {
                     event: e,
                     data: t,
                     message: n
-                }, "Auth", Sh)
+                }, "Auth", kh)
             },
-            kh = function() {
+            Eh = function() {
                 function e(e) {
                     var t = this;
-                    this.userPool = null, this.user = null, this.oAuthFlowInProgress = !1, this.autoSignInInitiated = !1, this.inflightSessionPromise = null, this.inflightSessionPromiseCounter = 0, this.Credentials = lp, this.wrapRefreshSessionCallback = function(e) {
+                    this.userPool = null, this.user = null, this.oAuthFlowInProgress = !1, this.autoSignInInitiated = !1, this.inflightSessionPromise = null, this.inflightSessionPromiseCounter = 0, this.Credentials = dp, this.wrapRefreshSessionCallback = function(e) {
                         return function(t, n) {
-                            return n ? Lh("tokenRefresh", void 0, "New token retrieved") : Lh("tokenRefresh_failure", t, "Failed to retrieve new token"), e(t, n)
+                            return n ? Ch("tokenRefresh", void 0, "New token retrieved") : Ch("tokenRefresh_failure", t, "Failed to retrieve new token"), e(t, n)
                         }
-                    }, this.configure(e), this.currentCredentials = this.currentCredentials.bind(this), this.currentUserCredentials = this.currentUserCredentials.bind(this), qs.listen("auth", (function(e) {
+                    }, this.configure(e), this.currentCredentials = this.currentCredentials.bind(this), this.currentUserCredentials = this.currentUserCredentials.bind(this), Ks.listen("auth", (function(e) {
                         switch (e.payload.event) {
                             case "verify":
                             case "signIn":
                                 t._storage.setItem("amplify-signin-with-hostedUI", "false");
                                 break;
                             case "signOut":
                                 t._storage.removeItem("amplify-signin-with-hostedUI");
@@ -67730,80 +67758,80 @@
                     }))
                 }
                 return e.prototype.getModuleName = function() {
                     return "Auth"
                 }, e.prototype.configure = function(e) {
                     var t = this;
                     if (!e) return this._config || {};
-                    Ih.debug("configure Auth");
-                    var n = Object.assign({}, this._config, Uc(e).Auth, e);
+                    Sh.debug("configure Auth");
+                    var n = Object.assign({}, this._config, Rc(e).Auth, e);
                     this._config = n;
                     var r = this._config,
                         o = r.userPoolId,
                         i = r.userPoolWebClientId,
                         a = r.cookieStorage,
                         s = r.oauth,
                         u = r.region,
                         l = r.identityPoolId,
                         c = r.mandatorySignIn,
                         d = r.refreshHandlers,
                         f = r.identityPoolRegion,
                         p = r.clientMetadata,
                         h = r.endpoint;
                     if (this._config.storage) {
-                        if (!this._isValidAuthStorage(this._config.storage)) throw Ih.error("The storage in the Auth config is not valid!"), new Error("Empty storage object");
+                        if (!this._isValidAuthStorage(this._config.storage)) throw Sh.error("The storage in the Auth config is not valid!"), new Error("Empty storage object");
                         this._storage = this._config.storage
-                    } else this._storage = a ? new ph(a) : e.ssr ? new dp : (new Xs).getStorage();
+                    } else this._storage = a ? new gh(a) : e.ssr ? new pp : (new eu).getStorage();
                     if (this._storageSync = Promise.resolve(), "function" === typeof this._storage.sync && (this._storageSync = this._storage.sync()), o) {
                         var g = {
                             UserPoolId: o,
                             ClientId: i,
                             endpoint: h
                         };
-                        g.Storage = this._storage, this.userPool = new dh(g, this.wrapRefreshSessionCallback)
+                        g.Storage = this._storage, this.userPool = new ph(g, this.wrapRefreshSessionCallback)
                     }
                     this.Credentials.configure({
                         mandatorySignIn: c,
                         region: u,
                         userPoolId: o,
                         identityPoolId: l,
                         refreshHandlers: d,
                         storage: this._storage,
                         identityPoolRegion: f
                     });
-                    var y = s ? Os(this._config.oauth) ? s : s.awsCognito : void 0;
+                    var y = s ? Us(this._config.oauth) ? s : s.awsCognito : void 0;
                     if (y) {
                         var m = Object.assign({
                             cognitoClientId: i,
                             UserPoolId: o,
                             domain: y.domain,
                             scopes: y.scope,
                             redirectSignIn: y.redirectSignIn,
                             redirectSignOut: y.redirectSignOut,
                             responseType: y.responseType,
                             Storage: this._storage,
                             urlOpener: y.urlOpener,
                             clientMetadata: p
                         }, y.options);
-                        this._oAuthHandler = new bh({
+                        this._oAuthHandler = new wh({
                             scopes: m.scopes,
                             config: m,
                             cognitoClientId: m.cognitoClientId
                         });
                         var v = {};
                         ! function(e) {
-                            if ($s().isBrowser && window.location) e({
+                            if (tu().isBrowser && window.location) e({
                                 url: window.location.href
                             });
-                            else if (!$s().isNode) throw new Error("Not supported")
+                            else if (!tu().isNode) throw new Error("Not supported")
                         }((function(e) {
                             var n = e.url;
                             v[n] || (v[n] = !0, t._handleAuthResponse(n))
                         }))
-                    }(Lh("configured", null, "The Auth category has been configured successfully"), this.autoSignInInitiated || "function" !== typeof this._storage.getItem) || (this.isTrueStorageValue("amplify-polling-started") && (Lh("autoSignIn_failure", null, Ls.AutoSignInError), this._storage.removeItem("amplify-auto-sign-in")), this._storage.removeItem("amplify-polling-started"));
+                    }(Ch("configured", null, "The Auth category has been configured successfully"), this.autoSignInInitiated || "function" !== typeof this._storage.getItem) || (this.isTrueStorageValue("amplify-polling-started") && (Ch("autoSignIn_failure", null, Cs.AutoSignInError), this._storage.removeItem("amplify-auto-sign-in")), this._storage.removeItem("amplify-polling-started"));
                     return this._config
                 }, e.prototype.signUp = function(e) {
                     for (var t, n, r, o = this, i = [], a = 1; a < arguments.length; a++) i[a - 1] = arguments[a];
                     if (!this.userPool) return this.rejectNoUserPool();
                     var s, u = null,
                         l = null,
                         c = [],
@@ -67813,187 +67841,187 @@
                         },
                         p = {},
                         h = {};
                     if (e && "string" === typeof e) {
                         u = e, l = i ? i[0] : null;
                         var g = i ? i[1] : null,
                             y = i ? i[2] : null;
-                        g && c.push(new Wp({
+                        g && c.push(new Zp({
                             Name: "email",
                             Value: g
-                        })), y && c.push(new Wp({
+                        })), y && c.push(new Zp({
                             Name: "phone_number",
                             Value: y
                         }))
                     } else {
-                        if (!e || "object" !== typeof e) return this.rejectAuthError(Ls.SignUpError);
+                        if (!e || "object" !== typeof e) return this.rejectAuthError(Cs.SignUpError);
                         u = e.username, l = e.password, e && e.clientMetadata ? s = e.clientMetadata : this._config.clientMetadata && (s = this._config.clientMetadata);
                         var m = e.attributes;
                         m && Object.keys(m).map((function(e) {
-                            c.push(new Wp({
+                            c.push(new Zp({
                                 Name: e,
                                 Value: m[e]
                             }))
                         }));
                         var v = e.validationData;
                         v && (d = [], Object.keys(v).map((function(e) {
-                            d.push(new Wp({
+                            d.push(new Zp({
                                 Name: e,
                                 Value: v[e]
                             }))
                         }))), (f = null !== (t = e.autoSignIn) && void 0 !== t ? t : {
                             enabled: !1
                         }).enabled && (this._storage.setItem("amplify-auto-sign-in", "true"), p = null !== (n = f.validationData) && void 0 !== n ? n : {}, h = null !== (r = f.clientMetaData) && void 0 !== r ? r : {})
                     }
-                    return u ? l ? (Ih.debug("signUp attrs:", c), Ih.debug("signUp validation data:", d), new Promise((function(e, t) {
+                    return u ? l ? (Sh.debug("signUp attrs:", c), Sh.debug("signUp validation data:", d), new Promise((function(e, t) {
                         o.userPool.signUp(u, l, c, d, (function(n, r) {
-                            n ? (Lh("signUp_failure", n, u + " failed to signup"), t(n)) : (Lh("signUp", r, u + " has signed up successfully"), f.enabled && o.handleAutoSignIn(u, l, p, h, r), e(r))
+                            n ? (Ch("signUp_failure", n, u + " failed to signup"), t(n)) : (Ch("signUp", r, u + " has signed up successfully"), f.enabled && o.handleAutoSignIn(u, l, p, h, r), e(r))
                         }), s)
-                    }))) : this.rejectAuthError(Ls.EmptyPassword) : this.rejectAuthError(Ls.EmptyUsername)
+                    }))) : this.rejectAuthError(Cs.EmptyPassword) : this.rejectAuthError(Cs.EmptyUsername)
                 }, e.prototype.handleAutoSignIn = function(e, t, n, r, o) {
                     this.autoSignInInitiated = !0;
-                    var i = new pp({
+                    var i = new gp({
                         Username: e,
                         Password: t,
                         ValidationData: n,
                         ClientMetadata: r
                     });
                     o.userConfirmed ? this.signInAfterUserConfirmed(i) : "link" === this._config.signUpVerificationMethod ? this.handleLinkAutoSignIn(i) : this.handleCodeAutoSignIn(i)
                 }, e.prototype.handleCodeAutoSignIn = function(e) {
                     var t = this;
-                    qs.listen("auth", (function n(r) {
+                    Ks.listen("auth", (function n(r) {
                         "confirmSignUp" === r.payload.event && t.signInAfterUserConfirmed(e, n)
                     }))
                 }, e.prototype.handleLinkAutoSignIn = function(e) {
                     var t = this;
                     this._storage.setItem("amplify-polling-started", "true");
                     var n = Date.now(),
                         r = setInterval((function() {
-                            Date.now() - n > 18e4 ? (clearInterval(r), Lh("autoSignIn_failure", null, "Please confirm your account and use your credentials to sign in."), t._storage.removeItem("amplify-auto-sign-in")) : t.signInAfterUserConfirmed(e, null, r)
+                            Date.now() - n > 18e4 ? (clearInterval(r), Ch("autoSignIn_failure", null, "Please confirm your account and use your credentials to sign in."), t._storage.removeItem("amplify-auto-sign-in")) : t.signInAfterUserConfirmed(e, null, r)
                         }), 5e3)
                 }, e.prototype.signInAfterUserConfirmed = function(e, t, n) {
-                    return Es(this, void 0, void 0, (function() {
+                    return Ts(this, void 0, void 0, (function() {
                         var r, o, i = this;
-                        return _s(this, (function(a) {
+                        return As(this, (function(a) {
                             switch (a.label) {
                                 case 0:
                                     r = this.createCognitoUser(e.getUsername()), a.label = 1;
                                 case 1:
                                     return a.trys.push([1, 3, , 4]), [4, r.authenticateUser(e, this.authCallbacks(r, (function(r) {
-                                        Lh("autoSignIn", r, e.getUsername() + " has signed in successfully"), t && qs.remove("auth", t), n && (clearInterval(n), i._storage.removeItem("amplify-polling-started")), i._storage.removeItem("amplify-auto-sign-in")
+                                        Ch("autoSignIn", r, e.getUsername() + " has signed in successfully"), t && Ks.remove("auth", t), n && (clearInterval(n), i._storage.removeItem("amplify-polling-started")), i._storage.removeItem("amplify-auto-sign-in")
                                     }), (function(e) {
-                                        Ih.error(e), i._storage.removeItem("amplify-auto-sign-in")
+                                        Sh.error(e), i._storage.removeItem("amplify-auto-sign-in")
                                     })))];
                                 case 2:
                                     return a.sent(), [3, 4];
                                 case 3:
-                                    return o = a.sent(), Ih.error(o), [3, 4];
+                                    return o = a.sent(), Sh.error(o), [3, 4];
                                 case 4:
                                     return [2]
                             }
                         }))
                     }))
                 }, e.prototype.confirmSignUp = function(e, t, n) {
                     var r = this;
                     if (!this.userPool) return this.rejectNoUserPool();
-                    if (!e) return this.rejectAuthError(Ls.EmptyUsername);
-                    if (!t) return this.rejectAuthError(Ls.EmptyCode);
+                    if (!e) return this.rejectAuthError(Cs.EmptyUsername);
+                    if (!t) return this.rejectAuthError(Cs.EmptyCode);
                     var o, i = this.createCognitoUser(e),
                         a = !n || "boolean" !== typeof n.forceAliasCreation || n.forceAliasCreation;
                     return n && n.clientMetadata ? o = n.clientMetadata : this._config.clientMetadata && (o = this._config.clientMetadata), new Promise((function(n, s) {
                         i.confirmRegistration(t, a, (function(t, o) {
-                            t ? s(t) : (Lh("confirmSignUp", o, e + " has been confirmed successfully"), r.isTrueStorageValue("amplify-auto-sign-in") && !r.autoSignInInitiated && (Lh("autoSignIn_failure", null, Ls.AutoSignInError), r._storage.removeItem("amplify-auto-sign-in")), n(o))
+                            t ? s(t) : (Ch("confirmSignUp", o, e + " has been confirmed successfully"), r.isTrueStorageValue("amplify-auto-sign-in") && !r.autoSignInInitiated && (Ch("autoSignIn_failure", null, Cs.AutoSignInError), r._storage.removeItem("amplify-auto-sign-in")), n(o))
                         }), o)
                     }))
                 }, e.prototype.isTrueStorageValue = function(e) {
                     var t = this._storage.getItem(e);
                     return !!t && "true" === t
                 }, e.prototype.resendSignUp = function(e, t) {
                     if (void 0 === t && (t = this._config.clientMetadata), !this.userPool) return this.rejectNoUserPool();
-                    if (!e) return this.rejectAuthError(Ls.EmptyUsername);
+                    if (!e) return this.rejectAuthError(Cs.EmptyUsername);
                     var n = this.createCognitoUser(e);
                     return new Promise((function(e, r) {
                         n.resendConfirmationCode((function(t, n) {
                             t ? r(t) : e(n)
                         }), t)
                     }))
                 }, e.prototype.signIn = function(e, t, n) {
                     if (void 0 === n && (n = this._config.clientMetadata), !this.userPool) return this.rejectNoUserPool();
                     var r = null,
                         o = null,
                         i = {};
                     if ("string" === typeof e) r = e, o = t;
                     else {
-                        if (!e.username) return this.rejectAuthError(Ls.InvalidUsername);
-                        "undefined" !== typeof t && Ih.warn("The password should be defined under the first parameter object!"), r = e.username, o = e.password, i = e.validationData
+                        if (!e.username) return this.rejectAuthError(Cs.InvalidUsername);
+                        "undefined" !== typeof t && Sh.warn("The password should be defined under the first parameter object!"), r = e.username, o = e.password, i = e.validationData
                     }
-                    if (!r) return this.rejectAuthError(Ls.EmptyUsername);
-                    var a = new pp({
+                    if (!r) return this.rejectAuthError(Cs.EmptyUsername);
+                    var a = new gp({
                         Username: r,
                         Password: o,
                         ValidationData: i,
                         ClientMetadata: n
                     });
                     return o ? this.signInWithPassword(a) : this.signInWithoutPassword(a)
                 }, e.prototype.authCallbacks = function(e, t, n) {
                     var r = this,
                         o = this;
                     return {
                         onSuccess: function(i) {
-                            return Es(r, void 0, void 0, (function() {
+                            return Ts(r, void 0, void 0, (function() {
                                 var r, a, s, u;
-                                return _s(this, (function(l) {
+                                return As(this, (function(l) {
                                     switch (l.label) {
                                         case 0:
-                                            Ih.debug(i), delete e.challengeName, delete e.challengeParam, l.label = 1;
+                                            Sh.debug(i), delete e.challengeName, delete e.challengeParam, l.label = 1;
                                         case 1:
                                             return l.trys.push([1, 4, 5, 9]), [4, this.Credentials.clear()];
                                         case 2:
                                             return l.sent(), [4, this.Credentials.set(i, "session")];
                                         case 3:
-                                            return r = l.sent(), Ih.debug("succeed to get cognito credentials", r), [3, 9];
+                                            return r = l.sent(), Sh.debug("succeed to get cognito credentials", r), [3, 9];
                                         case 4:
-                                            return a = l.sent(), Ih.debug("cannot get cognito credentials", a), [3, 9];
+                                            return a = l.sent(), Sh.debug("cannot get cognito credentials", a), [3, 9];
                                         case 5:
                                             return l.trys.push([5, 7, , 8]), [4, this.currentUserPoolUser()];
                                         case 6:
-                                            return s = l.sent(), o.user = s, Lh("signIn", s, "A user " + e.getUsername() + " has been signed in"), t(s), [3, 8];
+                                            return s = l.sent(), o.user = s, Ch("signIn", s, "A user " + e.getUsername() + " has been signed in"), t(s), [3, 8];
                                         case 7:
-                                            return u = l.sent(), Ih.error("Failed to get the signed in user", u), n(u), [3, 8];
+                                            return u = l.sent(), Sh.error("Failed to get the signed in user", u), n(u), [3, 8];
                                         case 8:
                                             return [7];
                                         case 9:
                                             return [2]
                                     }
                                 }))
                             }))
                         },
                         onFailure: function(t) {
-                            Ih.debug("signIn failure", t), Lh("signIn_failure", t, e.getUsername() + " failed to signin"), n(t)
+                            Sh.debug("signIn failure", t), Ch("signIn_failure", t, e.getUsername() + " failed to signin"), n(t)
                         },
                         customChallenge: function(n) {
-                            Ih.debug("signIn custom challenge answer required"), e.challengeName = "CUSTOM_CHALLENGE", e.challengeParam = n, t(e)
+                            Sh.debug("signIn custom challenge answer required"), e.challengeName = "CUSTOM_CHALLENGE", e.challengeParam = n, t(e)
                         },
                         mfaRequired: function(n, r) {
-                            Ih.debug("signIn MFA required"), e.challengeName = n, e.challengeParam = r, t(e)
+                            Sh.debug("signIn MFA required"), e.challengeName = n, e.challengeParam = r, t(e)
                         },
                         mfaSetup: function(n, r) {
-                            Ih.debug("signIn mfa setup", n), e.challengeName = n, e.challengeParam = r, t(e)
+                            Sh.debug("signIn mfa setup", n), e.challengeName = n, e.challengeParam = r, t(e)
                         },
                         newPasswordRequired: function(n, r) {
-                            Ih.debug("signIn new password"), e.challengeName = "NEW_PASSWORD_REQUIRED", e.challengeParam = {
+                            Sh.debug("signIn new password"), e.challengeName = "NEW_PASSWORD_REQUIRED", e.challengeParam = {
                                 userAttributes: n,
                                 requiredAttributes: r
                             }, t(e)
                         },
                         totpRequired: function(n, r) {
-                            Ih.debug("signIn totpRequired"), e.challengeName = n, e.challengeParam = r, t(e)
+                            Sh.debug("signIn totpRequired"), e.challengeName = n, e.challengeParam = r, t(e)
                         },
                         selectMFAType: function(n, r) {
-                            Ih.debug("signIn selectMFAType", n), e.challengeName = n, e.challengeParam = r, t(e)
+                            Sh.debug("signIn selectMFAType", n), e.challengeName = n, e.challengeParam = r, t(e)
                         }
                     }
                 }, e.prototype.signInWithPassword = function(e) {
                     var t = this;
                     if (this.pendingSignIn) throw new Error("Pending sign-in attempt already in progress");
                     var n = this.createCognitoUser(e.getUsername());
                     return this.pendingSignIn = new Promise((function(r, o) {
@@ -68008,32 +68036,32 @@
                         n = this.createCognitoUser(e.getUsername());
                     return n.setAuthenticationFlowType("CUSTOM_AUTH"), new Promise((function(r, o) {
                         n.initiateAuth(e, t.authCallbacks(n, r, o))
                     }))
                 }, e.prototype.getMFAOptions = function(e) {
                     return new Promise((function(t, n) {
                         e.getMFAOptions((function(e, r) {
-                            if (e) return Ih.debug("get MFA Options failed", e), void n(e);
-                            Ih.debug("get MFA options success", r), t(r)
+                            if (e) return Sh.debug("get MFA Options failed", e), void n(e);
+                            Sh.debug("get MFA options success", r), t(r)
                         }))
                     }))
                 }, e.prototype.getPreferredMFA = function(e, t) {
                     var n = this,
                         r = this;
                     return new Promise((function(o, i) {
                         var a = n._config.clientMetadata,
                             s = !!t && t.bypassCache;
                         e.getUserData((function(t, a) {
-                            return Es(n, void 0, void 0, (function() {
+                            return Ts(n, void 0, void 0, (function() {
                                 var n, s;
-                                return _s(this, (function(u) {
+                                return As(this, (function(u) {
                                     switch (u.label) {
                                         case 0:
                                             if (!t) return [3, 5];
-                                            if (Ih.debug("getting preferred mfa failed", t), !this.isSessionInvalid(t)) return [3, 4];
+                                            if (Sh.debug("getting preferred mfa failed", t), !this.isSessionInvalid(t)) return [3, 4];
                                             u.label = 1;
                                         case 1:
                                             return u.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(e)];
                                         case 2:
                                             return u.sent(), [3, 4];
                                         case 3:
                                             return n = u.sent(), i(new Error("Session is invalid due to: " + t.message + " and failed to clean up invalid session: " + n.message)), [2];
@@ -68051,29 +68079,29 @@
                     }))
                 }, e.prototype._getMfaTypeFromUserData = function(e) {
                     var t = null,
                         n = e.PreferredMfaSetting;
                     if (n) t = n;
                     else {
                         var r = e.UserMFASettingList;
-                        if (r) 0 === r.length ? t = "NOMFA" : Ih.debug("invalid case for getPreferredMFA", e);
+                        if (r) 0 === r.length ? t = "NOMFA" : Sh.debug("invalid case for getPreferredMFA", e);
                         else t = e.MFAOptions ? "SMS_MFA" : "NOMFA"
                     }
                     return t
                 }, e.prototype._getUserData = function(e, t) {
                     var n = this;
                     return new Promise((function(r, o) {
                         e.getUserData((function(t, i) {
-                            return Es(n, void 0, void 0, (function() {
+                            return Ts(n, void 0, void 0, (function() {
                                 var n;
-                                return _s(this, (function(a) {
+                                return As(this, (function(a) {
                                     switch (a.label) {
                                         case 0:
                                             if (!t) return [3, 5];
-                                            if (Ih.debug("getting user data failed", t), !this.isSessionInvalid(t)) return [3, 4];
+                                            if (Sh.debug("getting user data failed", t), !this.isSessionInvalid(t)) return [3, 4];
                                             a.label = 1;
                                         case 1:
                                             return a.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(e)];
                                         case 2:
                                             return a.sent(), [3, 4];
                                         case 3:
                                             return n = a.sent(), o(new Error("Session is invalid due to: " + t.message + " and failed to clean up invalid session: " + n.message)), [2];
@@ -68085,17 +68113,17 @@
                                             return [2]
                                     }
                                 }))
                             }))
                         }), t)
                     }))
                 }, e.prototype.setPreferredMFA = function(e, t) {
-                    return Es(this, void 0, void 0, (function() {
+                    return Ts(this, void 0, void 0, (function() {
                         var n, r, o, i, a, s, u = this;
-                        return _s(this, (function(l) {
+                        return As(this, (function(l) {
                             switch (l.label) {
                                 case 0:
                                     return n = this._config.clientMetadata, [4, this._getUserData(e, {
                                         bypassCache: !0,
                                         clientMetadata: n
                                     })];
                                 case 1:
@@ -68125,15 +68153,15 @@
                                 case 5:
                                     if ("NOMFA" === (s = l.sent())) return [2, Promise.resolve("No change for mfa type")];
                                     if ("SMS_MFA" === s) o = {
                                         PreferredMfa: !1,
                                         Enabled: !1
                                     };
                                     else {
-                                        if ("SOFTWARE_TOKEN_MFA" !== s) return [2, this.rejectAuthError(Ls.InvalidMFA)];
+                                        if ("SOFTWARE_TOKEN_MFA" !== s) return [2, this.rejectAuthError(Cs.InvalidMFA)];
                                         i = {
                                             PreferredMfa: !1,
                                             Enabled: !1
                                         }
                                     }
                                     return a && 0 !== a.length && a.forEach((function(e) {
                                         "SMS_MFA" === e ? o = {
@@ -68141,27 +68169,27 @@
                                             Enabled: !1
                                         } : "SOFTWARE_TOKEN_MFA" === e && (i = {
                                             PreferredMfa: !1,
                                             Enabled: !1
                                         })
                                     })), [3, 7];
                                 case 6:
-                                    return Ih.debug("no validmfa method provided"), [2, this.rejectAuthError(Ls.NoMFA)];
+                                    return Sh.debug("no validmfa method provided"), [2, this.rejectAuthError(Cs.NoMFA)];
                                 case 7:
                                     return this, [2, new Promise((function(t, r) {
                                         e.setUserMfaPreference(o, i, (function(o, i) {
-                                            if (o) return Ih.debug("Set user mfa preference error", o), r(o);
-                                            Ih.debug("Set user mfa success", i), Ih.debug("Caching the latest user data into local"), e.getUserData((function(n, o) {
-                                                return Es(u, void 0, void 0, (function() {
+                                            if (o) return Sh.debug("Set user mfa preference error", o), r(o);
+                                            Sh.debug("Set user mfa success", i), Sh.debug("Caching the latest user data into local"), e.getUserData((function(n, o) {
+                                                return Ts(u, void 0, void 0, (function() {
                                                     var o;
-                                                    return _s(this, (function(a) {
+                                                    return As(this, (function(a) {
                                                         switch (a.label) {
                                                             case 0:
                                                                 if (!n) return [3, 5];
-                                                                if (Ih.debug("getting user data failed", n), !this.isSessionInvalid(n)) return [3, 4];
+                                                                if (Sh.debug("getting user data failed", n), !this.isSessionInvalid(n)) return [3, 4];
                                                                 a.label = 1;
                                                             case 1:
                                                                 return a.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(e)];
                                                             case 2:
                                                                 return a.sent(), [3, 4];
                                                             case 3:
                                                                 return o = a.sent(), r(new Error("Session is invalid due to: " + n.message + " and failed to clean up invalid session: " + o.message)), [2];
@@ -68180,195 +68208,195 @@
                                     }))]
                             }
                         }))
                     }))
                 }, e.prototype.disableSMS = function(e) {
                     return new Promise((function(t, n) {
                         e.disableMFA((function(e, r) {
-                            if (e) return Ih.debug("disable mfa failed", e), void n(e);
-                            Ih.debug("disable mfa succeed", r), t(r)
+                            if (e) return Sh.debug("disable mfa failed", e), void n(e);
+                            Sh.debug("disable mfa succeed", r), t(r)
                         }))
                     }))
                 }, e.prototype.enableSMS = function(e) {
                     return new Promise((function(t, n) {
                         e.enableMFA((function(e, r) {
-                            if (e) return Ih.debug("enable mfa failed", e), void n(e);
-                            Ih.debug("enable mfa succeed", r), t(r)
+                            if (e) return Sh.debug("enable mfa failed", e), void n(e);
+                            Sh.debug("enable mfa succeed", r), t(r)
                         }))
                     }))
                 }, e.prototype.setupTOTP = function(e) {
                     return new Promise((function(t, n) {
                         e.associateSoftwareToken({
                             onFailure: function(e) {
-                                Ih.debug("associateSoftwareToken failed", e), n(e)
+                                Sh.debug("associateSoftwareToken failed", e), n(e)
                             },
                             associateSecretCode: function(e) {
-                                Ih.debug("associateSoftwareToken sucess", e), t(e)
+                                Sh.debug("associateSoftwareToken sucess", e), t(e)
                             }
                         })
                     }))
                 }, e.prototype.verifyTotpToken = function(e, t) {
-                    return Ih.debug("verification totp token", e, t), new Promise((function(n, r) {
+                    return Sh.debug("verification totp token", e, t), new Promise((function(n, r) {
                         e.verifySoftwareToken(t, "My TOTP device", {
                             onFailure: function(e) {
-                                Ih.debug("verifyTotpToken failed", e), r(e)
+                                Sh.debug("verifyTotpToken failed", e), r(e)
                             },
                             onSuccess: function(t) {
-                                Lh("signIn", e, "A user " + e.getUsername() + " has been signed in"), Lh("verify", e, "A user " + e.getUsername() + " has been verified"), Ih.debug("verifyTotpToken success", t), n(t)
+                                Ch("signIn", e, "A user " + e.getUsername() + " has been signed in"), Ch("verify", e, "A user " + e.getUsername() + " has been verified"), Sh.debug("verifyTotpToken success", t), n(t)
                             }
                         })
                     }))
                 }, e.prototype.confirmSignIn = function(e, t, n, r) {
                     var o = this;
-                    if (void 0 === r && (r = this._config.clientMetadata), !t) return this.rejectAuthError(Ls.EmptyCode);
+                    if (void 0 === r && (r = this._config.clientMetadata), !t) return this.rejectAuthError(Cs.EmptyCode);
                     var i = this;
                     return new Promise((function(a, s) {
                         e.sendMFACode(t, {
                             onSuccess: function(t) {
-                                return Es(o, void 0, void 0, (function() {
+                                return Ts(o, void 0, void 0, (function() {
                                     var n, r;
-                                    return _s(this, (function(o) {
+                                    return As(this, (function(o) {
                                         switch (o.label) {
                                             case 0:
-                                                Ih.debug(t), o.label = 1;
+                                                Sh.debug(t), o.label = 1;
                                             case 1:
                                                 return o.trys.push([1, 4, 5, 6]), [4, this.Credentials.clear()];
                                             case 2:
                                                 return o.sent(), [4, this.Credentials.set(t, "session")];
                                             case 3:
-                                                return n = o.sent(), Ih.debug("succeed to get cognito credentials", n), [3, 6];
+                                                return n = o.sent(), Sh.debug("succeed to get cognito credentials", n), [3, 6];
                                             case 4:
-                                                return r = o.sent(), Ih.debug("cannot get cognito credentials", r), [3, 6];
+                                                return r = o.sent(), Sh.debug("cannot get cognito credentials", r), [3, 6];
                                             case 5:
-                                                return i.user = e, Lh("signIn", e, "A user " + e.getUsername() + " has been signed in"), a(e), [7];
+                                                return i.user = e, Ch("signIn", e, "A user " + e.getUsername() + " has been signed in"), a(e), [7];
                                             case 6:
                                                 return [2]
                                         }
                                     }))
                                 }))
                             },
                             onFailure: function(e) {
-                                Ih.debug("confirm signIn failure", e), s(e)
+                                Sh.debug("confirm signIn failure", e), s(e)
                             }
                         }, n, r)
                     }))
                 }, e.prototype.completeNewPassword = function(e, t, n, r) {
                     var o = this;
-                    if (void 0 === n && (n = {}), void 0 === r && (r = this._config.clientMetadata), !t) return this.rejectAuthError(Ls.EmptyPassword);
+                    if (void 0 === n && (n = {}), void 0 === r && (r = this._config.clientMetadata), !t) return this.rejectAuthError(Cs.EmptyPassword);
                     var i = this;
                     return new Promise((function(a, s) {
                         e.completeNewPasswordChallenge(t, n, {
                             onSuccess: function(t) {
-                                return Es(o, void 0, void 0, (function() {
+                                return Ts(o, void 0, void 0, (function() {
                                     var n, r;
-                                    return _s(this, (function(o) {
+                                    return As(this, (function(o) {
                                         switch (o.label) {
                                             case 0:
-                                                Ih.debug(t), o.label = 1;
+                                                Sh.debug(t), o.label = 1;
                                             case 1:
                                                 return o.trys.push([1, 4, 5, 6]), [4, this.Credentials.clear()];
                                             case 2:
                                                 return o.sent(), [4, this.Credentials.set(t, "session")];
                                             case 3:
-                                                return n = o.sent(), Ih.debug("succeed to get cognito credentials", n), [3, 6];
+                                                return n = o.sent(), Sh.debug("succeed to get cognito credentials", n), [3, 6];
                                             case 4:
-                                                return r = o.sent(), Ih.debug("cannot get cognito credentials", r), [3, 6];
+                                                return r = o.sent(), Sh.debug("cannot get cognito credentials", r), [3, 6];
                                             case 5:
-                                                return i.user = e, Lh("signIn", e, "A user " + e.getUsername() + " has been signed in"), a(e), [7];
+                                                return i.user = e, Ch("signIn", e, "A user " + e.getUsername() + " has been signed in"), a(e), [7];
                                             case 6:
                                                 return [2]
                                         }
                                     }))
                                 }))
                             },
                             onFailure: function(e) {
-                                Ih.debug("completeNewPassword failure", e), Lh("completeNewPassword_failure", e, o.user + " failed to complete the new password flow"), s(e)
+                                Sh.debug("completeNewPassword failure", e), Ch("completeNewPassword_failure", e, o.user + " failed to complete the new password flow"), s(e)
                             },
                             mfaRequired: function(t, n) {
-                                Ih.debug("signIn MFA required"), e.challengeName = t, e.challengeParam = n, a(e)
+                                Sh.debug("signIn MFA required"), e.challengeName = t, e.challengeParam = n, a(e)
                             },
                             mfaSetup: function(t, n) {
-                                Ih.debug("signIn mfa setup", t), e.challengeName = t, e.challengeParam = n, a(e)
+                                Sh.debug("signIn mfa setup", t), e.challengeName = t, e.challengeParam = n, a(e)
                             },
                             totpRequired: function(t, n) {
-                                Ih.debug("signIn mfa setup", t), e.challengeName = t, e.challengeParam = n, a(e)
+                                Sh.debug("signIn mfa setup", t), e.challengeName = t, e.challengeParam = n, a(e)
                             }
                         }, r)
                     }))
                 }, e.prototype.sendCustomChallengeAnswer = function(e, t, n) {
                     var r = this;
                     if (void 0 === n && (n = this._config.clientMetadata), !this.userPool) return this.rejectNoUserPool();
-                    if (!t) return this.rejectAuthError(Ls.EmptyChallengeResponse);
+                    if (!t) return this.rejectAuthError(Cs.EmptyChallengeResponse);
                     return new Promise((function(o, i) {
                         e.sendCustomChallengeAnswer(t, r.authCallbacks(e, o, i), n)
                     }))
                 }, e.prototype.deleteUserAttributes = function(e, t) {
                     var n = this;
                     return new Promise((function(r, o) {
                         n.userSession(e).then((function(n) {
                             e.deleteAttributes(t, (function(e, t) {
                                 return e ? o(e) : r(t)
                             }))
                         }))
                     }))
                 }, e.prototype.deleteUser = function() {
-                    return Es(this, void 0, void 0, (function() {
+                    return Ts(this, void 0, void 0, (function() {
                         var e, t, n = this;
-                        return _s(this, (function(r) {
+                        return As(this, (function(r) {
                             switch (r.label) {
                                 case 0:
                                     return r.trys.push([0, 2, , 3]), [4, this._storageSync];
                                 case 1:
                                     return r.sent(), [3, 3];
                                 case 2:
-                                    throw e = r.sent(), Ih.debug("Failed to sync cache info into memory", e), new Error(e);
+                                    throw e = r.sent(), Sh.debug("Failed to sync cache info into memory", e), new Error(e);
                                 case 3:
                                     return t = this._oAuthHandler && "true" === this._storage.getItem("amplify-signin-with-hostedUI"), [2, new Promise((function(e, r) {
-                                        return Es(n, void 0, void 0, (function() {
+                                        return Ts(n, void 0, void 0, (function() {
                                             var n, o = this;
-                                            return _s(this, (function(i) {
+                                            return As(this, (function(i) {
                                                 if (this.userPool) {
-                                                    if (!(n = this.userPool.getCurrentUser())) return Ih.debug("Failed to get user from user pool"), [2, r(new Error("No current user."))];
+                                                    if (!(n = this.userPool.getCurrentUser())) return Sh.debug("Failed to get user from user pool"), [2, r(new Error("No current user."))];
                                                     n.getSession((function(i, a) {
-                                                        return Es(o, void 0, void 0, (function() {
+                                                        return Ts(o, void 0, void 0, (function() {
                                                             var o, a = this;
-                                                            return _s(this, (function(s) {
+                                                            return As(this, (function(s) {
                                                                 switch (s.label) {
                                                                     case 0:
                                                                         if (!i) return [3, 5];
-                                                                        if (Ih.debug("Failed to get the user session", i), !this.isSessionInvalid(i)) return [3, 4];
+                                                                        if (Sh.debug("Failed to get the user session", i), !this.isSessionInvalid(i)) return [3, 4];
                                                                         s.label = 1;
                                                                     case 1:
                                                                         return s.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(n)];
                                                                     case 2:
                                                                         return s.sent(), [3, 4];
                                                                     case 3:
                                                                         return o = s.sent(), r(new Error("Session is invalid due to: " + i.message + " and failed to clean up invalid session: " + o.message)), [2];
                                                                     case 4:
                                                                         return [2, r(i)];
                                                                     case 5:
                                                                         n.deleteUser((function(o, i) {
                                                                             if (o) r(o);
                                                                             else {
-                                                                                Lh("userDeleted", i, "The authenticated user has been deleted."), n.signOut(), a.user = null;
+                                                                                Ch("userDeleted", i, "The authenticated user has been deleted."), n.signOut(), a.user = null;
                                                                                 try {
                                                                                     a.cleanCachedItems()
                                                                                 } catch (s) {
-                                                                                    Ih.debug("failed to clear cached items")
+                                                                                    Sh.debug("failed to clear cached items")
                                                                                 }
-                                                                                t ? a.oAuthSignOutRedirect(e, r) : (Lh("signOut", a.user, "A user has been signed out"), e(i))
+                                                                                t ? a.oAuthSignOutRedirect(e, r) : (Ch("signOut", a.user, "A user has been signed out"), e(i))
                                                                             }
                                                                         })), s.label = 6;
                                                                     case 6:
                                                                         return [2]
                                                                 }
                                                             }))
                                                         }))
                                                     }))
-                                                } else Ih.debug("no Congito User pool"), r(new Error("Cognito User pool does not exist"));
+                                                } else Sh.debug("no Congito User pool"), r(new Error("Cognito User pool does not exist"));
                                                 return [2]
                                             }))
                                         }))
                                     }))]
                             }
                         }))
                     }))
@@ -68383,17 +68411,17 @@
                                 if ("sub" !== u && u.indexOf("_verified") < 0) {
                                     var l = {
                                         Name: u,
                                         Value: t[u]
                                     };
                                     o.push(l)
                                 } e.updateAttributes(o, (function(e, n, o) {
-                                if (e) return Lh("updateUserAttributes_failure", e, "Failed to update attributes"), s(e);
+                                if (e) return Ch("updateUserAttributes_failure", e, "Failed to update attributes"), s(e);
                                 var i = r.createUpdateAttributesResultList(t, null === o || void 0 === o ? void 0 : o.CodeDeliveryDetailsList);
-                                return Lh("updateUserAttributes", i, "Attributes successfully updated"), a(n)
+                                return Ch("updateUserAttributes", i, "Attributes successfully updated"), a(n)
                             }), n)
                         }))
                     }))
                 }, e.prototype.createUpdateAttributesResultList = function(e, t) {
                     var n = {};
                     return Object.keys(e).forEach((function(e) {
                         n[e] = {
@@ -68437,73 +68465,73 @@
                 }, e.prototype.isRefreshTokenExpiredError = function(e) {
                     return this.isErrorWithMessage(e) && "Refresh Token has expired" === e.message
                 }, e.prototype.isSignedInHostedUI = function() {
                     return this._oAuthHandler && "true" === this._storage.getItem("amplify-signin-with-hostedUI")
                 }, e.prototype.isSessionInvalid = function(e) {
                     return this.isUserDisabledError(e) || this.isUserDoesNotExistError(e) || this.isTokenRevokedError(e) || this.isRefreshTokenRevokedError(e) || this.isRefreshTokenExpiredError(e)
                 }, e.prototype.cleanUpInvalidSession = function(e) {
-                    return Es(this, void 0, void 0, (function() {
+                    return Ts(this, void 0, void 0, (function() {
                         var t = this;
-                        return _s(this, (function(n) {
+                        return As(this, (function(n) {
                             switch (n.label) {
                                 case 0:
                                     e.signOut(), this.user = null, n.label = 1;
                                 case 1:
                                     return n.trys.push([1, 3, , 4]), [4, this.cleanCachedItems()];
                                 case 2:
                                     return n.sent(), [3, 4];
                                 case 3:
-                                    return n.sent(), Ih.debug("failed to clear cached items"), [3, 4];
+                                    return n.sent(), Sh.debug("failed to clear cached items"), [3, 4];
                                 case 4:
                                     return this.isSignedInHostedUI() ? [2, new Promise((function(e, n) {
                                         t.oAuthSignOutRedirect(e, n)
-                                    }))] : (Lh("signOut", this.user, "A user has been signed out"), [2])
+                                    }))] : (Ch("signOut", this.user, "A user has been signed out"), [2])
                             }
                         }))
                     }))
                 }, e.prototype.currentUserPoolUser = function(e) {
                     var t = this;
                     return this.userPool ? new Promise((function(n, r) {
                         t._storageSync.then((function() {
-                            return Es(t, void 0, void 0, (function() {
+                            return Ts(t, void 0, void 0, (function() {
                                 var t, o, i, a, s, u, l = this;
-                                return _s(this, (function(c) {
+                                return As(this, (function(c) {
                                     switch (c.label) {
                                         case 0:
-                                            return this.isOAuthInProgress() ? (Ih.debug("OAuth signIn in progress, waiting for resolution..."), [4, new Promise((function(e) {
+                                            return this.isOAuthInProgress() ? (Sh.debug("OAuth signIn in progress, waiting for resolution..."), [4, new Promise((function(e) {
                                                 var t = setTimeout((function() {
-                                                    Ih.debug("OAuth signIn in progress timeout"), qs.remove("auth", n), e()
+                                                    Sh.debug("OAuth signIn in progress timeout"), Ks.remove("auth", n), e()
                                                 }), 1e4);
 
                                                 function n(r) {
                                                     var o = r.payload.event;
-                                                    "cognitoHostedUI" !== o && "cognitoHostedUI_failure" !== o || (Ih.debug("OAuth signIn resolved: " + o), clearTimeout(t), qs.remove("auth", n), e())
+                                                    "cognitoHostedUI" !== o && "cognitoHostedUI_failure" !== o || (Sh.debug("OAuth signIn resolved: " + o), clearTimeout(t), Ks.remove("auth", n), e())
                                                 }
-                                                qs.listen("auth", n)
+                                                Ks.listen("auth", n)
                                             }))]) : [3, 2];
                                         case 1:
                                             c.sent(), c.label = 2;
                                         case 2:
-                                            if (!(t = this.userPool.getCurrentUser())) return Ih.debug("Failed to get user from user pool"), r("No current user"), [2];
+                                            if (!(t = this.userPool.getCurrentUser())) return Sh.debug("Failed to get user from user pool"), r("No current user"), [2];
                                             c.label = 3;
                                         case 3:
                                             return c.trys.push([3, 7, , 8]), [4, this._userSession(t)];
                                         case 4:
                                             return o = c.sent(), (i = !!e && e.bypassCache) ? [4, this.Credentials.clear()] : [3, 6];
                                         case 5:
                                             c.sent(), c.label = 6;
                                         case 6:
-                                            return a = this._config.clientMetadata, s = o.getAccessToken().decodePayload().scope, (void 0 === s ? "" : s).split(" ").includes(Dh) ? (t.getUserData((function(e, o) {
-                                                return Es(l, void 0, void 0, (function() {
+                                            return a = this._config.clientMetadata, s = o.getAccessToken().decodePayload().scope, (void 0 === s ? "" : s).split(" ").includes(Lh) ? (t.getUserData((function(e, o) {
+                                                return Ts(l, void 0, void 0, (function() {
                                                     var i, a, s, u, l, c, d;
-                                                    return _s(this, (function(f) {
+                                                    return As(this, (function(f) {
                                                         switch (f.label) {
                                                             case 0:
                                                                 if (!e) return [3, 7];
-                                                                if (Ih.debug("getting user data failed", e), !this.isSessionInvalid(e)) return [3, 5];
+                                                                if (Sh.debug("getting user data failed", e), !this.isSessionInvalid(e)) return [3, 5];
                                                                 f.label = 1;
                                                             case 1:
                                                                 return f.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(t)];
                                                             case 2:
                                                                 return f.sent(), [3, 4];
                                                             case 3:
                                                                 return i = f.sent(), r(new Error("Session is invalid due to: " + e.message + " and failed to clean up invalid session: " + i.message)), [2];
@@ -68513,114 +68541,114 @@
                                                                 n(t), f.label = 6;
                                                             case 6:
                                                                 return [2];
                                                             case 7:
                                                                 for (a = o.PreferredMfaSetting || "NOMFA", s = [], u = 0; u < o.UserAttributes.length; u++) l = {
                                                                     Name: o.UserAttributes[u].Name,
                                                                     Value: o.UserAttributes[u].Value
-                                                                }, c = new Wp(l), s.push(c);
+                                                                }, c = new Zp(l), s.push(c);
                                                                 return d = this.attributesToObject(s), Object.assign(t, {
                                                                     attributes: d,
                                                                     preferredMFA: a
                                                                 }), [2, n(t)]
                                                         }
                                                     }))
                                                 }))
                                             }), {
                                                 bypassCache: i,
                                                 clientMetadata: a
-                                            }), [3, 8]) : (Ih.debug("Unable to get the user data because the " + Dh + " is not in the scopes of the access token"), [2, n(t)]);
+                                            }), [3, 8]) : (Sh.debug("Unable to get the user data because the " + Lh + " is not in the scopes of the access token"), [2, n(t)]);
                                         case 7:
                                             return u = c.sent(), r(u), [3, 8];
                                         case 8:
                                             return [2]
                                     }
                                 }))
                             }))
                         })).catch((function(e) {
-                            return Ih.debug("Failed to sync cache info into memory", e), r(e)
+                            return Sh.debug("Failed to sync cache info into memory", e), r(e)
                         }))
                     })) : this.rejectNoUserPool()
                 }, e.prototype.isOAuthInProgress = function() {
                     return this.oAuthFlowInProgress
                 }, e.prototype.currentAuthenticatedUser = function(e) {
-                    return Es(this, void 0, void 0, (function() {
+                    return Ts(this, void 0, void 0, (function() {
                         var t, n, r, o, i;
-                        return _s(this, (function(a) {
+                        return As(this, (function(a) {
                             switch (a.label) {
                                 case 0:
-                                    Ih.debug("getting current authenticated user"), t = null, a.label = 1;
+                                    Sh.debug("getting current authenticated user"), t = null, a.label = 1;
                                 case 1:
                                     return a.trys.push([1, 3, , 4]), [4, this._storageSync];
                                 case 2:
                                     return a.sent(), [3, 4];
                                 case 3:
-                                    throw n = a.sent(), Ih.debug("Failed to sync cache info into memory", n), n;
+                                    throw n = a.sent(), Sh.debug("Failed to sync cache info into memory", n), n;
                                 case 4:
                                     try {
-                                        (r = JSON.parse(this._storage.getItem("aws-amplify-federatedInfo"))) && (t = Cs(Cs({}, r.user), {
+                                        (r = JSON.parse(this._storage.getItem("aws-amplify-federatedInfo"))) && (t = _s(_s({}, r.user), {
                                             token: r.token
                                         }))
                                     } catch (s) {
-                                        Ih.debug("cannot load federated user from auth storage")
+                                        Sh.debug("cannot load federated user from auth storage")
                                     }
-                                    return t ? (this.user = t, Ih.debug("get current authenticated federated user", this.user), [2, this.user]) : [3, 5];
+                                    return t ? (this.user = t, Sh.debug("get current authenticated federated user", this.user), [2, this.user]) : [3, 5];
                                 case 5:
-                                    Ih.debug("get current authenticated userpool user"), o = null, a.label = 6;
+                                    Sh.debug("get current authenticated userpool user"), o = null, a.label = 6;
                                 case 6:
                                     return a.trys.push([6, 8, , 9]), [4, this.currentUserPoolUser(e)];
                                 case 7:
                                     return o = a.sent(), [3, 9];
                                 case 8:
-                                    return "No userPool" === (i = a.sent()) && Ih.error("Cannot get the current user because the user pool is missing. Please make sure the Auth module is configured with a valid Cognito User Pool ID"), Ih.debug("The user is not authenticated by the error", i), [2, Promise.reject("The user is not authenticated")];
+                                    return "No userPool" === (i = a.sent()) && Sh.error("Cannot get the current user because the user pool is missing. Please make sure the Auth module is configured with a valid Cognito User Pool ID"), Sh.debug("The user is not authenticated by the error", i), [2, Promise.reject("The user is not authenticated")];
                                 case 9:
                                     return this.user = o, [2, this.user]
                             }
                         }))
                     }))
                 }, e.prototype.currentSession = function() {
                     var e = this;
-                    return Ih.debug("Getting current session"), this.userPool ? new Promise((function(t, n) {
+                    return Sh.debug("Getting current session"), this.userPool ? new Promise((function(t, n) {
                         e.currentUserPoolUser().then((function(r) {
                             e.userSession(r).then((function(e) {
                                 t(e)
                             })).catch((function(e) {
-                                Ih.debug("Failed to get the current session", e), n(e)
+                                Sh.debug("Failed to get the current session", e), n(e)
                             }))
                         })).catch((function(e) {
-                            Ih.debug("Failed to get the current user", e), n(e)
+                            Sh.debug("Failed to get the current user", e), n(e)
                         }))
                     })) : Promise.reject(new Error("No User Pool in the configuration."))
                 }, e.prototype._userSession = function(e) {
-                    return Es(this, void 0, void 0, (function() {
+                    return Ts(this, void 0, void 0, (function() {
                         var t, n, r = this;
-                        return _s(this, (function(o) {
+                        return As(this, (function(o) {
                             switch (o.label) {
                                 case 0:
-                                    if (!e) return Ih.debug("the user is null"), [2, this.rejectAuthError(Ls.NoUserSession)];
+                                    if (!e) return Sh.debug("the user is null"), [2, this.rejectAuthError(Cs.NoUserSession)];
                                     t = this._config.clientMetadata, 0 === this.inflightSessionPromiseCounter && (this.inflightSessionPromise = new Promise((function(n, o) {
                                         e.getSession((function(t, i) {
-                                            return Es(r, void 0, void 0, (function() {
+                                            return Ts(r, void 0, void 0, (function() {
                                                 var r;
-                                                return _s(this, (function(a) {
+                                                return As(this, (function(a) {
                                                     switch (a.label) {
                                                         case 0:
                                                             if (!t) return [3, 5];
-                                                            if (Ih.debug("Failed to get the session from user", e), !this.isSessionInvalid(t)) return [3, 4];
+                                                            if (Sh.debug("Failed to get the session from user", e), !this.isSessionInvalid(t)) return [3, 4];
                                                             a.label = 1;
                                                         case 1:
                                                             return a.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(e)];
                                                         case 2:
                                                             return a.sent(), [3, 4];
                                                         case 3:
                                                             return r = a.sent(), o(new Error("Session is invalid due to: " + t.message + " and failed to clean up invalid session: " + r.message)), [2];
                                                         case 4:
                                                             return o(t), [2];
                                                         case 5:
-                                                            return Ih.debug("Succeed to get the user session", i), n(i), [2]
+                                                            return Sh.debug("Succeed to get the user session", i), n(i), [2]
                                                     }
                                                 }))
                                             }))
                                         }), {
                                             clientMetadata: t
                                         })
                                     }))), this.inflightSessionPromiseCounter++, o.label = 1;
@@ -68634,43 +68662,43 @@
                                     return [2]
                             }
                         }))
                     }))
                 }, e.prototype.userSession = function(e) {
                     return this._userSession(e)
                 }, e.prototype.currentUserCredentials = function() {
-                    return Es(this, void 0, void 0, (function() {
+                    return Ts(this, void 0, void 0, (function() {
                         var e, t, n = this;
-                        return _s(this, (function(r) {
+                        return As(this, (function(r) {
                             switch (r.label) {
                                 case 0:
-                                    Ih.debug("Getting current user credentials"), r.label = 1;
+                                    Sh.debug("Getting current user credentials"), r.label = 1;
                                 case 1:
                                     return r.trys.push([1, 3, , 4]), [4, this._storageSync];
                                 case 2:
                                     return r.sent(), [3, 4];
                                 case 3:
-                                    throw e = r.sent(), Ih.debug("Failed to sync cache info into memory", e), e;
+                                    throw e = r.sent(), Sh.debug("Failed to sync cache info into memory", e), e;
                                 case 4:
                                     t = null;
                                     try {
                                         t = JSON.parse(this._storage.getItem("aws-amplify-federatedInfo"))
                                     } catch (o) {
-                                        Ih.debug("failed to get or parse item aws-amplify-federatedInfo", o)
+                                        Sh.debug("failed to get or parse item aws-amplify-federatedInfo", o)
                                     }
                                     return t ? [2, this.Credentials.refreshFederatedToken(t)] : [2, this.currentSession().then((function(e) {
-                                        return Ih.debug("getting session success", e), n.Credentials.set(e, "session")
+                                        return Sh.debug("getting session success", e), n.Credentials.set(e, "session")
                                     })).catch((function() {
-                                        return Ih.debug("getting guest credentials"), n.Credentials.set(null, "guest")
+                                        return Sh.debug("getting guest credentials"), n.Credentials.set(null, "guest")
                                     }))]
                             }
                         }))
                     }))
                 }, e.prototype.currentCredentials = function() {
-                    return Ih.debug("getting current credentials"), this.Credentials.get()
+                    return Sh.debug("getting current credentials"), this.Credentials.get()
                 }, e.prototype.verifyUserAttribute = function(e, t, n) {
                     return void 0 === n && (n = this._config.clientMetadata), new Promise((function(r, o) {
                         e.getAttributeVerificationCode(t, {
                             onSuccess: function(e) {
                                 return r(e)
                             },
                             onFailure: function(e) {
@@ -68684,289 +68712,289 @@
                             onSuccess: function(e) {
                                 r(e)
                             },
                             onFailure: function(e) {
                                 o(e)
                             }
                         })
-                    })) : this.rejectAuthError(Ls.EmptyCode)
+                    })) : this.rejectAuthError(Cs.EmptyCode)
                 }, e.prototype.verifyCurrentUserAttribute = function(e) {
                     var t = this;
                     return t.currentUserPoolUser().then((function(n) {
                         return t.verifyUserAttribute(n, e)
                     }))
                 }, e.prototype.verifyCurrentUserAttributeSubmit = function(e, t) {
                     var n = this;
                     return n.currentUserPoolUser().then((function(r) {
                         return n.verifyUserAttributeSubmit(r, e, t)
                     }))
                 }, e.prototype.cognitoIdentitySignOut = function(e, t) {
-                    return Es(this, void 0, void 0, (function() {
+                    return Ts(this, void 0, void 0, (function() {
                         var n, r, o = this;
-                        return _s(this, (function(i) {
+                        return As(this, (function(i) {
                             switch (i.label) {
                                 case 0:
                                     return i.trys.push([0, 2, , 3]), [4, this._storageSync];
                                 case 1:
                                     return i.sent(), [3, 3];
                                 case 2:
-                                    throw n = i.sent(), Ih.debug("Failed to sync cache info into memory", n), n;
+                                    throw n = i.sent(), Sh.debug("Failed to sync cache info into memory", n), n;
                                 case 3:
                                     return r = this._oAuthHandler && "true" === this._storage.getItem("amplify-signin-with-hostedUI"), [2, new Promise((function(n, i) {
                                         if (e && e.global) {
-                                            Ih.debug("user global sign out", t);
+                                            Sh.debug("user global sign out", t);
                                             var a = o._config.clientMetadata;
                                             t.getSession((function(e, a) {
-                                                return Es(o, void 0, void 0, (function() {
+                                                return Ts(o, void 0, void 0, (function() {
                                                     var o, a = this;
-                                                    return _s(this, (function(s) {
+                                                    return As(this, (function(s) {
                                                         switch (s.label) {
                                                             case 0:
                                                                 if (!e) return [3, 5];
-                                                                if (Ih.debug("failed to get the user session", e), !this.isSessionInvalid(e)) return [3, 4];
+                                                                if (Sh.debug("failed to get the user session", e), !this.isSessionInvalid(e)) return [3, 4];
                                                                 s.label = 1;
                                                             case 1:
                                                                 return s.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(t)];
                                                             case 2:
                                                                 return s.sent(), [3, 4];
                                                             case 3:
                                                                 return o = s.sent(), i(new Error("Session is invalid due to: " + e.message + " and failed to clean up invalid session: " + o.message)), [2];
                                                             case 4:
                                                                 return [2, i(e)];
                                                             case 5:
                                                                 return t.globalSignOut({
                                                                     onSuccess: function(e) {
-                                                                        if (Ih.debug("global sign out success"), !r) return n();
+                                                                        if (Sh.debug("global sign out success"), !r) return n();
                                                                         a.oAuthSignOutRedirect(n, i)
                                                                     },
                                                                     onFailure: function(e) {
-                                                                        return Ih.debug("global sign out failed", e), i(e)
+                                                                        return Sh.debug("global sign out failed", e), i(e)
                                                                     }
                                                                 }), [2]
                                                         }
                                                     }))
                                                 }))
                                             }), {
                                                 clientMetadata: a
                                             })
-                                        } else Ih.debug("user sign out", t), t.signOut((function() {
+                                        } else Sh.debug("user sign out", t), t.signOut((function() {
                                             if (!r) return n();
                                             o.oAuthSignOutRedirect(n, i)
                                         }))
                                     }))]
                             }
                         }))
                     }))
                 }, e.prototype.oAuthSignOutRedirect = function(e, t) {
-                    $s().isBrowser ? this.oAuthSignOutRedirectOrReject(t) : this.oAuthSignOutAndResolve(e)
+                    tu().isBrowser ? this.oAuthSignOutRedirectOrReject(t) : this.oAuthSignOutAndResolve(e)
                 }, e.prototype.oAuthSignOutAndResolve = function(e) {
                     this._oAuthHandler.signOut(), e()
                 }, e.prototype.oAuthSignOutRedirectOrReject = function(e) {
                     this._oAuthHandler.signOut(), setTimeout((function() {
                         return e(Error("Signout timeout fail"))
                     }), 3e3)
                 }, e.prototype.signOut = function(e) {
-                    return Es(this, void 0, void 0, (function() {
+                    return Ts(this, void 0, void 0, (function() {
                         var t;
-                        return _s(this, (function(n) {
+                        return As(this, (function(n) {
                             switch (n.label) {
                                 case 0:
                                     return n.trys.push([0, 2, , 3]), [4, this.cleanCachedItems()];
                                 case 1:
                                     return n.sent(), [3, 3];
                                 case 2:
-                                    return n.sent(), Ih.debug("failed to clear cached items"), [3, 3];
+                                    return n.sent(), Sh.debug("failed to clear cached items"), [3, 3];
                                 case 3:
                                     return this.userPool ? (t = this.userPool.getCurrentUser()) ? [4, this.cognitoIdentitySignOut(e, t)] : [3, 5] : [3, 7];
                                 case 4:
                                     return n.sent(), [3, 6];
                                 case 5:
-                                    Ih.debug("no current Cognito user"), n.label = 6;
+                                    Sh.debug("no current Cognito user"), n.label = 6;
                                 case 6:
                                     return [3, 8];
                                 case 7:
-                                    Ih.debug("no Cognito User pool"), n.label = 8;
+                                    Sh.debug("no Cognito User pool"), n.label = 8;
                                 case 8:
-                                    return Lh("signOut", this.user, "A user has been signed out"), this.user = null, [2]
+                                    return Ch("signOut", this.user, "A user has been signed out"), this.user = null, [2]
                             }
                         }))
                     }))
                 }, e.prototype.cleanCachedItems = function() {
-                    return Es(this, void 0, void 0, (function() {
-                        return _s(this, (function(e) {
+                    return Ts(this, void 0, void 0, (function() {
+                        return As(this, (function(e) {
                             switch (e.label) {
                                 case 0:
                                     return [4, this.Credentials.clear()];
                                 case 1:
                                     return e.sent(), [2]
                             }
                         }))
                     }))
                 }, e.prototype.changePassword = function(e, t, n, r) {
                     var o = this;
                     return void 0 === r && (r = this._config.clientMetadata), new Promise((function(i, a) {
                         o.userSession(e).then((function(o) {
                             e.changePassword(t, n, (function(e, t) {
-                                return e ? (Ih.debug("change password failure", e), a(e)) : i(t)
+                                return e ? (Sh.debug("change password failure", e), a(e)) : i(t)
                             }), r)
                         }))
                     }))
                 }, e.prototype.forgotPassword = function(e, t) {
                     if (void 0 === t && (t = this._config.clientMetadata), !this.userPool) return this.rejectNoUserPool();
-                    if (!e) return this.rejectAuthError(Ls.EmptyUsername);
+                    if (!e) return this.rejectAuthError(Cs.EmptyUsername);
                     var n = this.createCognitoUser(e);
                     return new Promise((function(r, o) {
                         n.forgotPassword({
                             onSuccess: function() {
                                 r()
                             },
                             onFailure: function(t) {
-                                Ih.debug("forgot password failure", t), Lh("forgotPassword_failure", t, e + " forgotPassword failed"), o(t)
+                                Sh.debug("forgot password failure", t), Ch("forgotPassword_failure", t, e + " forgotPassword failed"), o(t)
                             },
                             inputVerificationCode: function(t) {
-                                Lh("forgotPassword", n, e + " has initiated forgot password flow"), r(t)
+                                Ch("forgotPassword", n, e + " has initiated forgot password flow"), r(t)
                             }
                         }, t)
                     }))
                 }, e.prototype.forgotPasswordSubmit = function(e, t, n, r) {
                     if (void 0 === r && (r = this._config.clientMetadata), !this.userPool) return this.rejectNoUserPool();
-                    if (!e) return this.rejectAuthError(Ls.EmptyUsername);
-                    if (!t) return this.rejectAuthError(Ls.EmptyCode);
-                    if (!n) return this.rejectAuthError(Ls.EmptyPassword);
+                    if (!e) return this.rejectAuthError(Cs.EmptyUsername);
+                    if (!t) return this.rejectAuthError(Cs.EmptyCode);
+                    if (!n) return this.rejectAuthError(Cs.EmptyPassword);
                     var o = this.createCognitoUser(e);
                     return new Promise((function(i, a) {
                         o.confirmPassword(t, n, {
                             onSuccess: function(t) {
-                                Lh("forgotPasswordSubmit", o, e + " forgotPasswordSubmit successful"), i(t)
+                                Ch("forgotPasswordSubmit", o, e + " forgotPasswordSubmit successful"), i(t)
                             },
                             onFailure: function(t) {
-                                Lh("forgotPasswordSubmit_failure", t, e + " forgotPasswordSubmit failed"), a(t)
+                                Ch("forgotPasswordSubmit_failure", t, e + " forgotPasswordSubmit failed"), a(t)
                             }
                         }, r)
                     }))
                 }, e.prototype.currentUserInfo = function() {
-                    return Es(this, void 0, void 0, (function() {
+                    return Ts(this, void 0, void 0, (function() {
                         var e, t, n, r, o, i, a;
-                        return _s(this, (function(s) {
+                        return As(this, (function(s) {
                             switch (s.label) {
                                 case 0:
                                     return (e = this.Credentials.getCredSource()) && "aws" !== e && "userPool" !== e ? [3, 9] : [4, this.currentUserPoolUser().catch((function(e) {
-                                        return Ih.error(e)
+                                        return Sh.error(e)
                                     }))];
                                 case 1:
                                     if (!(a = s.sent())) return [2, null];
                                     s.label = 2;
                                 case 2:
                                     return s.trys.push([2, 8, , 9]), [4, this.userAttributes(a)];
                                 case 3:
                                     t = s.sent(), n = this.attributesToObject(t), r = null, s.label = 4;
                                 case 4:
                                     return s.trys.push([4, 6, , 7]), [4, this.currentCredentials()];
                                 case 5:
                                     return r = s.sent(), [3, 7];
                                 case 6:
-                                    return o = s.sent(), Ih.debug("Failed to retrieve credentials while getting current user info", o), [3, 7];
+                                    return o = s.sent(), Sh.debug("Failed to retrieve credentials while getting current user info", o), [3, 7];
                                 case 7:
                                     return [2, {
                                         id: r ? r.identityId : void 0,
                                         username: a.getUsername(),
                                         attributes: n
                                     }];
                                 case 8:
-                                    return i = s.sent(), Ih.error("currentUserInfo error", i), [2, {}];
+                                    return i = s.sent(), Sh.error("currentUserInfo error", i), [2, {}];
                                 case 9:
                                     return "federated" === e ? [2, (a = this.user) || {}] : [2]
                             }
                         }))
                     }))
                 }, e.prototype.federatedSignIn = function(e, t, n) {
-                    return Es(this, void 0, void 0, (function() {
+                    return Ts(this, void 0, void 0, (function() {
                         var r, o, i, a, s, u, l, c, d, f, p;
-                        return _s(this, (function(h) {
+                        return As(this, (function(h) {
                             switch (h.label) {
                                 case 0:
                                     if (!this._config.identityPoolId && !this._config.userPoolId) throw new Error("Federation requires either a User Pool or Identity Pool in config");
                                     if ("undefined" === typeof e && this._config.identityPoolId && !this._config.userPoolId) throw new Error("Federation with Identity Pools requires tokens passed as arguments");
-                                    return As(e) || (g = e) && ["customProvider"].find((function(e) {
+                                    return zs(e) || (g = e) && ["customProvider"].find((function(e) {
                                         return g.hasOwnProperty(e)
                                     })) || function(e) {
                                         return e && !!["customState"].find((function(t) {
                                             return e.hasOwnProperty(t)
                                         }))
                                     }(e) || "undefined" === typeof e ? (r = e || {
-                                        provider: Ss.Cognito
-                                    }, s = As(r) ? r.provider : r.customProvider, As(r), o = r.customState, this._config.userPoolId && (i = Os(this._config.oauth) ? this._config.userPoolWebClientId : this._config.oauth.clientID, a = Os(this._config.oauth) ? this._config.oauth.redirectSignIn : this._config.oauth.redirectUri, this._oAuthHandler.oauthSignIn(this._config.oauth.responseType, this._config.oauth.domain, a, i, s, o)), [3, 4]) : [3, 1];
+                                        provider: ks.Cognito
+                                    }, s = zs(r) ? r.provider : r.customProvider, zs(r), o = r.customState, this._config.userPoolId && (i = Us(this._config.oauth) ? this._config.userPoolWebClientId : this._config.oauth.clientID, a = Us(this._config.oauth) ? this._config.oauth.redirectSignIn : this._config.oauth.redirectUri, this._oAuthHandler.oauthSignIn(this._config.oauth.responseType, this._config.oauth.domain, a, i, s, o)), [3, 4]) : [3, 1];
                                 case 1:
                                     s = e;
                                     try {
-                                        (u = JSON.stringify(JSON.parse(this._storage.getItem("aws-amplify-federatedInfo")).user)) && Ih.warn("There is already a signed in user: " + u + " in your app.\n\t\t\t\t\t\t\t\t\t\t\t\t\t\t\t\t\tYou should not call Auth.federatedSignIn method again as it may cause unexpected behavior.")
+                                        (u = JSON.stringify(JSON.parse(this._storage.getItem("aws-amplify-federatedInfo")).user)) && Sh.warn("There is already a signed in user: " + u + " in your app.\n\t\t\t\t\t\t\t\t\t\t\t\t\t\t\t\t\tYou should not call Auth.federatedSignIn method again as it may cause unexpected behavior.")
                                     } catch (y) {}
                                     return l = t.token, c = t.identity_id, d = t.expires_at, [4, this.Credentials.set({
                                         provider: s,
                                         token: l,
                                         identity_id: c,
                                         user: n,
                                         expires_at: d
                                     }, "federation")];
                                 case 2:
                                     return f = h.sent(), [4, this.currentAuthenticatedUser()];
                                 case 3:
-                                    return p = h.sent(), Lh("signIn", p, "A user " + p.username + " has been signed in"), Ih.debug("federated sign in credentials", f), [2, f];
+                                    return p = h.sent(), Ch("signIn", p, "A user " + p.username + " has been signed in"), Sh.debug("federated sign in credentials", f), [2, f];
                                 case 4:
                                     return [2]
                             }
                             var g
                         }))
                     }))
                 }, e.prototype._handleAuthResponse = function(e) {
-                    return Es(this, void 0, void 0, (function() {
+                    return Ts(this, void 0, void 0, (function() {
                         var t, n, r, o, i, a, s, u, l, c, d, f, p, h;
-                        return _s(this, (function(g) {
+                        return As(this, (function(g) {
                             switch (g.label) {
                                 case 0:
-                                    if (this.oAuthFlowInProgress) return Ih.debug("Skipping URL " + e + " current flow in progress"), [2];
+                                    if (this.oAuthFlowInProgress) return Sh.debug("Skipping URL " + e + " current flow in progress"), [2];
                                     g.label = 1;
                                 case 1:
                                     if (g.trys.push([1, , 8, 9]), this.oAuthFlowInProgress = !0, !this._config.userPoolId) throw new Error("OAuth responses require a User Pool defined in config");
-                                    if (Lh("parsingCallbackUrl", {
+                                    if (Ch("parsingCallbackUrl", {
                                             url: e
-                                        }, "The callback url is being parsed"), t = e || ($s().isBrowser ? window.location.href : ""), n = !!((0, hh.Qc)(t).query || "").split("&").map((function(e) {
+                                        }, "The callback url is being parsed"), t = e || (tu().isBrowser ? window.location.href : ""), n = !!((0, yh.Qc)(t).query || "").split("&").map((function(e) {
                                             return e.split("=")
                                         })).find((function(e) {
-                                            var t = Ts(e, 1)[0];
+                                            var t = Os(e, 1)[0];
                                             return "code" === t || "error" === t
-                                        })), r = !!((0, hh.Qc)(t).hash || "#").substr(1).split("&").map((function(e) {
+                                        })), r = !!((0, yh.Qc)(t).hash || "#").substr(1).split("&").map((function(e) {
                                             return e.split("=")
                                         })).find((function(e) {
-                                            var t = Ts(e, 1)[0];
+                                            var t = Os(e, 1)[0];
                                             return "access_token" === t || "error" === t
                                         })), !n && !r) return [3, 7];
                                     this._storage.setItem("amplify-redirected-from-hosted-ui", "true"), g.label = 2;
                                 case 2:
                                     return g.trys.push([2, 6, , 7]), [4, this._oAuthHandler.handleAuthResponse(t)];
                                 case 3:
-                                    return o = g.sent(), i = o.accessToken, a = o.idToken, s = o.refreshToken, u = o.state, l = new Fp({
-                                        IdToken: new Pp({
+                                    return o = g.sent(), i = o.accessToken, a = o.idToken, s = o.refreshToken, u = o.state, l = new Qp({
+                                        IdToken: new Bp({
                                             IdToken: a
                                         }),
-                                        RefreshToken: new Rp({
+                                        RefreshToken: new Fp({
                                             RefreshToken: s
                                         }),
-                                        AccessToken: new zp({
+                                        AccessToken: new Pp({
                                             AccessToken: i
                                         })
                                     }), c = void 0, this._config.identityPoolId ? [4, this.Credentials.set(l, "session")] : [3, 5];
                                 case 4:
-                                    c = g.sent(), Ih.debug("AWS credentials", c), g.label = 5;
+                                    c = g.sent(), Sh.debug("AWS credentials", c), g.label = 5;
                                 case 5:
-                                    return d = /-/.test(u), (f = this.createCognitoUser(l.getIdToken().decodePayload()["cognito:username"])).setSignInUserSession(l), window && "undefined" !== typeof window.history && window.history.replaceState({}, null, this._config.oauth.redirectSignIn), Lh("signIn", f, "A user " + f.getUsername() + " has been signed in"), Lh("cognitoHostedUI", f, "A user " + f.getUsername() + " has been signed in via Cognito Hosted UI"), d && (p = u.split("-").splice(1).join("-"), Lh("customOAuthState", p.match(/.{2}/g).map((function(e) {
+                                    return d = /-/.test(u), (f = this.createCognitoUser(l.getIdToken().decodePayload()["cognito:username"])).setSignInUserSession(l), window && "undefined" !== typeof window.history && window.history.replaceState({}, null, this._config.oauth.redirectSignIn), Ch("signIn", f, "A user " + f.getUsername() + " has been signed in"), Ch("cognitoHostedUI", f, "A user " + f.getUsername() + " has been signed in via Cognito Hosted UI"), d && (p = u.split("-").splice(1).join("-"), Ch("customOAuthState", p.match(/.{2}/g).map((function(e) {
                                         return String.fromCharCode(parseInt(e, 16))
                                     })).join(""), "State for user " + f.getUsername())), [2, c];
                                 case 6:
-                                    return h = g.sent(), Ih.debug("Error in cognito hosted auth response", h), window && "undefined" !== typeof window.history && window.history.replaceState({}, null, this._config.oauth.redirectSignIn), Lh("signIn_failure", h, "The OAuth response flow failed"), Lh("cognitoHostedUI_failure", h, "A failure occurred when returning to the Cognito Hosted UI"), Lh("customState_failure", h, "A failure occurred when returning state"), [3, 7];
+                                    return h = g.sent(), Sh.debug("Error in cognito hosted auth response", h), window && "undefined" !== typeof window.history && window.history.replaceState({}, null, this._config.oauth.redirectSignIn), Ch("signIn_failure", h, "The OAuth response flow failed"), Ch("cognitoHostedUI_failure", h, "A failure occurred when returning to the Cognito Hosted UI"), Ch("customState_failure", h, "A failure occurred when returning state"), [3, 7];
                                 case 7:
                                     return [3, 9];
                                 case 8:
                                     return this.oAuthFlowInProgress = !1, [7];
                                 case 9:
                                     return [2]
                             }
@@ -68991,86 +69019,86 @@
                 }, e.prototype.createCognitoUser = function(e) {
                     var t = {
                         Username: e,
                         Pool: this.userPool
                     };
                     t.Storage = this._storage;
                     var n = this._config.authenticationFlowType,
-                        r = new Jp(t);
+                        r = new Xp(t);
                     return n && r.setAuthenticationFlowType(n), r
                 }, e.prototype._isValidAuthStorage = function(e) {
                     return !!e && "function" === typeof e.getItem && "function" === typeof e.setItem && "function" === typeof e.removeItem && "function" === typeof e.clear
                 }, e.prototype.noUserPoolErrorHandler = function(e) {
-                    return !e || e.userPoolId && e.identityPoolId ? Ls.NoConfig : Ls.MissingAuthConfig
+                    return !e || e.userPoolId && e.identityPoolId ? Cs.NoConfig : Cs.MissingAuthConfig
                 }, e.prototype.rejectAuthError = function(e) {
-                    return Promise.reject(new wh(e))
+                    return Promise.reject(new Nh(e))
                 }, e.prototype.rejectNoUserPool = function() {
                     var e = this.noUserPoolErrorHandler(this._config);
-                    return Promise.reject(new xh(e))
+                    return Promise.reject(new Ih(e))
                 }, e.prototype.rememberDevice = function() {
-                    return Es(this, void 0, void 0, (function() {
+                    return Ts(this, void 0, void 0, (function() {
                         var e, t;
-                        return _s(this, (function(n) {
+                        return As(this, (function(n) {
                             switch (n.label) {
                                 case 0:
                                     return n.trys.push([0, 2, , 3]), [4, this.currentUserPoolUser()];
                                 case 1:
                                     return e = n.sent(), [3, 3];
                                 case 2:
-                                    return t = n.sent(), Ih.debug("The user is not authenticated by the error", t), [2, Promise.reject("The user is not authenticated")];
+                                    return t = n.sent(), Sh.debug("The user is not authenticated by the error", t), [2, Promise.reject("The user is not authenticated")];
                                 case 3:
                                     return e.getCachedDeviceKeyAndPassword(), [2, new Promise((function(t, n) {
                                         e.setDeviceStatusRemembered({
                                             onSuccess: function(e) {
                                                 t(e)
                                             },
                                             onFailure: function(e) {
-                                                "InvalidParameterException" === e.code ? n(new wh(Ls.DeviceConfig)) : "NetworkError" === e.code ? n(new wh(Ls.NetworkError)) : n(e)
+                                                "InvalidParameterException" === e.code ? n(new Nh(Cs.DeviceConfig)) : "NetworkError" === e.code ? n(new Nh(Cs.NetworkError)) : n(e)
                                             }
                                         })
                                     }))]
                             }
                         }))
                     }))
                 }, e.prototype.forgetDevice = function() {
-                    return Es(this, void 0, void 0, (function() {
+                    return Ts(this, void 0, void 0, (function() {
                         var e, t;
-                        return _s(this, (function(n) {
+                        return As(this, (function(n) {
                             switch (n.label) {
                                 case 0:
                                     return n.trys.push([0, 2, , 3]), [4, this.currentUserPoolUser()];
                                 case 1:
                                     return e = n.sent(), [3, 3];
                                 case 2:
-                                    return t = n.sent(), Ih.debug("The user is not authenticated by the error", t), [2, Promise.reject("The user is not authenticated")];
+                                    return t = n.sent(), Sh.debug("The user is not authenticated by the error", t), [2, Promise.reject("The user is not authenticated")];
                                 case 3:
                                     return e.getCachedDeviceKeyAndPassword(), [2, new Promise((function(t, n) {
                                         e.forgetDevice({
                                             onSuccess: function(e) {
                                                 t(e)
                                             },
                                             onFailure: function(e) {
-                                                "InvalidParameterException" === e.code ? n(new wh(Ls.DeviceConfig)) : "NetworkError" === e.code ? n(new wh(Ls.NetworkError)) : n(e)
+                                                "InvalidParameterException" === e.code ? n(new Nh(Cs.DeviceConfig)) : "NetworkError" === e.code ? n(new Nh(Cs.NetworkError)) : n(e)
                                             }
                                         })
                                     }))]
                             }
                         }))
                     }))
                 }, e.prototype.fetchDevices = function() {
-                    return Es(this, void 0, void 0, (function() {
+                    return Ts(this, void 0, void 0, (function() {
                         var e, t;
-                        return _s(this, (function(n) {
+                        return As(this, (function(n) {
                             switch (n.label) {
                                 case 0:
                                     return n.trys.push([0, 2, , 3]), [4, this.currentUserPoolUser()];
                                 case 1:
                                     return e = n.sent(), [3, 3];
                                 case 2:
-                                    throw t = n.sent(), Ih.debug("The user is not authenticated by the error", t), new Error("The user is not authenticated");
+                                    throw t = n.sent(), Sh.debug("The user is not authenticated by the error", t), new Error("The user is not authenticated");
                                 case 3:
                                     return e.getCachedDeviceKeyAndPassword(), [2, new Promise((function(t, n) {
                                         var r = {
                                             onSuccess: function(e) {
                                                 var n = e.Devices.map((function(e) {
                                                     var t = e.DeviceAttributes.find((function(e) {
                                                         return "device_name" === e.Name
@@ -69079,28 +69107,28 @@
                                                         id: e.DeviceKey,
                                                         name: t.Value
                                                     }
                                                 }));
                                                 t(n)
                                             },
                                             onFailure: function(e) {
-                                                "InvalidParameterException" === e.code ? n(new wh(Ls.DeviceConfig)) : "NetworkError" === e.code ? n(new wh(Ls.NetworkError)) : n(e)
+                                                "InvalidParameterException" === e.code ? n(new Nh(Cs.DeviceConfig)) : "NetworkError" === e.code ? n(new Nh(Cs.NetworkError)) : n(e)
                                             }
                                         };
                                         e.listDevices(60, null, r)
                                     }))]
                             }
                         }))
                     }))
                 }, e
             }(),
-            Ch = new kh(null);
-        pu.register(Ch);
-        var Eh = "#FEFEFE",
-            _h = function(e) {
+            _h = new Eh(null);
+        gu.register(_h);
+        var Th = "#FEFEFE",
+            Ah = function(e) {
                 var t = e.hide,
                     n = pe().environ,
                     r = ta(),
                     o = Xi(zt.Url("/cognito_config", !1), {
                         cache: !0,
                         onData: function(e) {
                             var t = {
@@ -69112,15 +69140,15 @@
                                     domain: e.domain,
                                     scope: e.scope,
                                     prompt: "select_account",
                                     redirectSignIn: e.callback,
                                     responseType: "code"
                                 }
                             };
-                            Ch.configure(t)
+                            _h.configure(t)
                         }
                     });
                 var i = (0, Kr.jsx)("div", {
                     children: (0, Kr.jsxs)("div", {
                         className: "title-font",
                         style: {
                             marginTop: "4pt",
@@ -69148,52 +69176,52 @@
                 });
                 return (0, Kr.jsx)("div", {
                     style: {
                         transform: "scale(1.1)",
                         marginTop: "10pt",
                         marginBottom: "40pt"
                     },
-                    children: (0, Kr.jsx)(Th, {
+                    children: (0, Kr.jsx)(Oh, {
                         links: i,
                         children: o.loading ? (0, Kr.jsx)(Kr.Fragment, {
                             children: (0, Kr.jsx)(no, {
                                 condition: !0,
                                 color: Ft.GetForegroundColor(),
                                 bold: !1,
                                 size: "140px",
                                 label: "Loading configuration "
                             })
                         }) : (0, Kr.jsxs)(Kr.Fragment, {
                             children: [(0, Kr.jsx)("div", {
                                 style: {
                                     paddingTop: "0pt"
                                 }
-                            }), (0, Kr.jsx)(Ah, {
+                            }), (0, Kr.jsx)(zh, {
                                 signin: function() {
-                                    bt.Set("env", At.PreferredName(n, r)), bt.Set("signinvia", "Google"), Ch.federatedSignIn({
+                                    bt.Set("env", At.PreferredName(n, r)), bt.Set("signinvia", "Google"), _h.federatedSignIn({
                                         provider: "Google",
                                         prompt: "select_account"
                                     }, {
                                         prompt: "select_account"
                                     })
                                 }
                             }), (0, Kr.jsx)("div", {
                                 style: {
                                     paddingTop: "6pt"
                                 }
-                            }), (0, Kr.jsx)(Oh, {
+                            }), (0, Kr.jsx)(Uh, {
                                 signin: function() {
                                     window.alert("Sign in with GitHub via Cognito not supported.")
                                 }
                             })]
                         })
                     })
                 })
             },
-            Th = function(e) {
+            Oh = function(e) {
                 var t = e.links,
                     n = e.children;
                 return (0, Kr.jsx)("div", {
                     className: "container",
                     style: {
                         width: "265pt",
                         marginTop: "30pt"
@@ -69204,15 +69232,15 @@
                                 border: "2px solid var(--box-fg)",
                                 padding: "2px 2px 2px 2px",
                                 borderRadius: "6px",
                                 overflow: "hidden"
                             },
                             children: (0, Kr.jsxs)("div", {
                                 style: {
-                                    background: Eh,
+                                    background: Th,
                                     border: "1px solid var(--box-fg)",
                                     borderRadius: "6px",
                                     overflow: "hidden"
                                 },
                                 children: [(0, Kr.jsx)("div", {
                                     style: {
                                         background: "var(--box-fg)",
@@ -69237,17 +69265,17 @@
                             })
                         }), t && (0, Kr.jsx)(Kr.Fragment, {
                             children: t
                         })]
                     })
                 })
             },
-            Ah = function(e) {
+            zh = function(e) {
                 var t = e.signin;
-                return (0, Kr.jsxs)(zh, {
+                return (0, Kr.jsxs)(Ph, {
                     signin: t,
                     children: [(0, Kr.jsx)("img", {
                         alt: "google",
                         src: Ut.GoogleLoginLogo(),
                         style: {
                             position: "relative",
                             marginTop: "-2px"
@@ -69259,17 +69287,17 @@
                             fontSize: "12pt",
                             marginLeft: "10pt"
                         },
                         children: "Sign in with Google"
                     })]
                 })
             },
-            Oh = function(e) {
+            Uh = function(e) {
                 var t = e.signin;
-                return (0, Kr.jsxs)(zh, {
+                return (0, Kr.jsxs)(Ph, {
                     signin: t,
                     children: [(0, Kr.jsx)("img", {
                         alt: "github",
                         src: Ut.GitHubLoginLogo(),
                         style: {
                             position: "relative",
                             marginTop: "-2px",
@@ -69282,30 +69310,30 @@
                             fontSize: "12pt",
                             marginLeft: "7pt"
                         },
                         children: "Sign in with GitHub"
                     })]
                 })
             },
-            zh = function(e) {
+            Ph = function(e) {
                 var t = e.signin,
                     n = e.children;
                 return (0, Kr.jsx)("div", {
                     style: {
-                        background: Eh,
+                        background: Th,
                         padding: "0 10pt 0 10pt"
                     },
                     children: (0, Kr.jsx)("button", {
                         className: "signin-as-button",
                         onClick: t,
                         children: n
                     })
                 })
             },
-            Uh = function(e) {
+            Rh = function(e) {
                 var t = a(Re(), 1)[0],
                     n = t.get("code"),
                     r = t.get("state"),
                     o = sessionStorage.getItem("oauth_state"),
                     i = sessionStorage.getItem("ouath_pkce_key"),
                     s = fe(),
                     u = "".concat(zt.Url("/cognito/callback", !1), "?code=").concat(n, "&code_verifier=").concat(i, "&state=").concat(r, "&state_verifier=").concat(o),
@@ -69328,28 +69356,28 @@
                     var c = bt.Get("signinvia");
                     return (0, Kr.jsx)("div", {
                         style: {
                             transform: "scale(1.1)",
                             marginTop: "10pt",
                             marginBottom: "40pt"
                         },
-                        children: (0, Kr.jsx)(Th, {
+                        children: (0, Kr.jsx)(Oh, {
                             children: (0, Kr.jsx)(no, {
                                 condition: l.loading,
                                 color: Ft.GetForegroundColor(),
                                 bold: !1,
                                 size: 140,
                                 label: "Signing in via ".concat(c)
                             })
                         })
                     })
                 }
             },
-            Ph = __webpack_require__(9712),
-            Rh = function(e) {
+            Bh = __webpack_require__(9712),
+            Fh = function(e) {
                 var n, r, o, i, s, u, l, c, d, f, p, h, g = ta(),
                     y = a((0, t.useState)(!1), 2),
                     m = y[0],
                     v = y[1],
                     M = a((0, t.useState)(!1), 2),
                     b = M[0],
                     j = M[1],
@@ -69395,15 +69423,15 @@
                                 theme: {
                                     primaryColor: "blue",
                                     backgroundColor: "blue",
                                     logo: ""
                                 },
                                 allowedConnections: null === x || void 0 === x || null === (o = x.data) || void 0 === o ? void 0 : o.connections
                             };
-                            return new Ph.default(null === x || void 0 === x || null === (i = x.data) || void 0 === i ? void 0 : i.client, null === x || void 0 === x || null === (a = x.data) || void 0 === a ? void 0 : a.domain, s)
+                            return new Bh.default(null === x || void 0 === x || null === (i = x.data) || void 0 === i ? void 0 : i.client, null === x || void 0 === x || null === (a = x.data) || void 0 === a ? void 0 : a.domain, s)
                         }().show(), navigator.userAgent.toLowerCase().indexOf("firefox") > -1 && (document.getElementById("login_auth_container").style.height = "200", document.getElementById("login_auth_container").style.background = "white", document.getElementById("login_auth_container").style.borderStyle = "none"), document.getElementById("login_auth_container").firstChild.firstChild.style.paddingLeft = "1", document.getElementById("login_auth_container").firstChild.firstChild.style.paddingRight = "1", document.getElementById("login_auth_container").firstChild.firstChild.style.paddingTop = "1", document.getElementById("login_auth_container").firstChild.firstChild.style.paddingBottom = "1", document.getElementById("login_auth_container").firstChild.firstChild.style.fontWeight = "bold", document.getElementById("login_auth_container").firstChild.firstChild.style.fontWeight = "bold", v(!0)
                 }
                 if ((g.loading || x.loading) && !g.error) return (0, Kr.jsx)(Kr.Fragment, {
                     children: "Loading ..."
                 });
                 if (g.error) return (0, Kr.jsx)(xi, {
                     error: g.error,
@@ -69447,15 +69475,15 @@
                                     position: "bottom",
                                     text: "AWS Account Alias: ".concat(null === g || void 0 === g || null === (c = g.app) || void 0 === c || null === (d = c.credentials) || void 0 === d ? void 0 : d.aws_account_name)
                                 })]
                             }), (0, Kr.jsx)("br", {})]
                         })]
                     })
                 };
-                return I ? (0, Kr.jsx)(_h, {
+                return I ? (0, Kr.jsx)(Ah, {
                     hide: function() {
                         return D(!1)
                     }
                 }) : (0, Kr.jsx)(Kr.Fragment, {
                     children: Br.IsLoggedIn(g) ? (0, Kr.jsx)(t.Fragment, {
                         children: (0, Kr.jsxs)("div", {
                             className: "container",
@@ -69522,21 +69550,21 @@
                                                 }), (0, Kr.jsxs)("div", {
                                                     style: {
                                                         fontSize: "small",
                                                         marginTop: "6pt",
                                                         paddingTop: "5pt",
                                                         borderTop: "1px solid"
                                                     },
-                                                    children: ["Session started: ", (0, Kr.jsx)(Ma.FormatDuration, {
+                                                    children: ["Session started: ", (0, Kr.jsx)(ja.FormatDuration, {
                                                         start: Br.Token().authenticated_at,
                                                         verbose: !0,
                                                         fallback: "just now",
                                                         suffix: "ago",
                                                         tooltip: !0
-                                                    }), "\xa0", (0, Kr.jsx)("br", {}), "Session expires: ", (0, Kr.jsx)(Ma.FormatDuration, {
+                                                    }), "\xa0", (0, Kr.jsx)("br", {}), "Session expires: ", (0, Kr.jsx)(ja.FormatDuration, {
                                                         end: Br.Token().authenticated_until,
                                                         verbose: !0,
                                                         fallback: "now",
                                                         suffix: "from now",
                                                         tooltip: !0
                                                     }), "\xa0", (0, Kr.jsx)("br", {}), "Click ", (0, Kr.jsx)("span", {
                                                         style: {
@@ -70074,15 +70102,15 @@
                                     w && !m && T()
                                 }), 10), "")]
                             })]
                         })]
                     })
                 })
             },
-            Bh = function(e) {
+            Yh = function(e) {
                 var n = ta(),
                     r = pe().environCompare,
                     o = a((0, t.useState)(!1), 2),
                     i = o[0],
                     s = o[1],
                     u = a((0, t.useState)("all"), 2),
                     l = u[0],
@@ -70428,15 +70456,15 @@
                                 display: "none"
                             },
                             children: d.yaml()
                         })]
                     })
                 })
             },
-            Fh = function(e) {
+            Qh = function(e) {
                 return {
                     __get: function(t, n, r, o) {
                         var i = e.findIndex((function(e) {
                             return e.type === t
                         }));
                         if (i >= 0) {
                             var a = n ? "".concat(t, ".").concat(n) : t;
@@ -70449,16 +70477,16 @@
                                 }
                             }
                         }
                         return null
                     }
                 }
             },
-            Yh = function(e) {
-                e = Fh(e);
+            Gh = function(e) {
+                e = Qh(e);
                 var n = a((0, t.useState)([]), 2),
                     r = n[0],
                     o = n[1];
                 return (0, t.useState)({
                     count: function() {
                         return r.length
                     },
@@ -70503,23 +70531,23 @@
                     __unselect: function(e) {
                         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : null,
                             n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : null;
                         null == n && (n = this.__lookup(e, t)), n >= 0 && (r.splice(n, 1), o(u(r)))
                     }
                 })[0]
             },
-            Qh = function(e) {
+            Wh = function(e) {
                 var t;
                 return "function" == typeof e && (e = e()), (null === (t = e) || void 0 === t ? void 0 : t.constructor) === Object ? e : {}
             },
-            Gh = function(e, t) {
+            Hh = function(e, t) {
                 return "function" == typeof e && (e = e()), void 0 !== e ? e : {}
             };
 
-        function Wh(e) {
+        function Zh(e) {
             var t, n, r = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : void 0,
                 o = !(arguments.length > 2 && void 0 !== arguments[2]) || arguments[2];
             if (Object.is(e, r))
                 if ((null === (n = e) || void 0 === n ? void 0 : n.constructor) === Object) e = Ye({}, e);
                 else if (Array.isArray(e)) {
                 var i = function(e) {
                     var t = u(e),
@@ -70534,24 +70562,24 @@
                     return t
                 };
                 e = i(e)
             } else "function" === typeof e && (e = e(r));
             else(null === (t = e) || void 0 === t ? void 0 : t.constructor) === Object && (null === r || void 0 === r ? void 0 : r.constructor) === Object && o && (e = Ye(Ye({}, r), e));
             return e
         }
-        var Hh = function(e, n) {
+        var Vh = function(e, n) {
                 var r = !0 === (null === e || void 0 === e ? void 0 : e.__keyedState) ? !0 === e.__keyedStateUsage ? e : e.keyed("default") : null,
-                    o = r ? r.__state() ? r.__state() : Gh(n) : Qh(e),
+                    o = r ? r.__state() ? r.__state() : Hh(n) : Wh(e),
                     i = a((0, t.useState)(o), 2),
                     s = i[0],
                     u = i[1];
                 return (0, t.useEffect)((function() {
-                    o && r && !r.__state() && r.__updateState(Wh(o, s, !0))
+                    o && r && !r.__state() && r.__updateState(Zh(o, s, !0))
                 }), []), r ? [s, function(e) {
-                    e = Wh(e, s, !0), u(e), r.__updateState(e)
+                    e = Zh(e, s, !0), u(e), r.__updateState(e)
                 }] : {
                     __keyedState: !0,
                     key: null,
                     keyed: function(e) {
                         var t;
                         if (!0 === this.__keyedState) {
                             (null === (t = e) || void 0 === t ? void 0 : t.constructor) === String && 0 !== e.length || (e = "default");
@@ -70575,27 +70603,27 @@
                                     return s[e]
                                 }
                             }
                         }
                     }
                 }
             },
-            Zh = {
+            qh = {
                 color: "var(--box-fg)",
                 fontWeight: "bold",
                 paddingTop: "1pt",
                 verticalAlign: "top",
                 width: "5%",
                 paddingRight: "8pt",
                 whiteSpace: "nowrap"
             },
-            Vh = {
+            Jh = {
                 verticalAlign: "top"
             },
-            qh = function(e) {
+            Kh = function(e) {
                 var t = e.showVpcs,
                     n = e.toggleVpcs,
                     r = e.showSecurityGroups,
                     o = e.toggleSecurityGroups,
                     i = e.showSubnetsPublic,
                     a = e.toggleSubnetsPublic,
                     s = e.showSubnetsPrivate,
@@ -70648,15 +70676,15 @@
                             },
                             onClick: o,
                             children: "Security Groups"
                         })]
                     })]
                 })
             },
-            Jh = function(e) {
+            Xh = function(e) {
                 var t = e.showGac,
                     n = e.toggleGac,
                     r = e.showEcosystem,
                     o = e.toggleEcosystem;
                 return (0, Kr.jsx)(Kr.Fragment, {
                     children: (0, Kr.jsxs)("div", {
                         className: "box margin thickborder",
@@ -70681,15 +70709,15 @@
                             },
                             onClick: o,
                             children: "Ecosystem Definition"
                         })]
                     })
                 })
             },
-            Kh = function(e) {
+            $h = function(e) {
                 var t, n, r = e.keyedState,
                     o = e.hide,
                     i = "true" === (null === (t = Re()[0]) || void 0 === t || null === (n = t.get("all")) || void 0 === n ? void 0 : n.toLowerCase()),
                     a = Xi("/aws/vpcs".concat(i ? "/all" : ""), {
                         cache: !0
                     });
                 return (0, Kr.jsxs)("div", {
@@ -70728,27 +70756,27 @@
                                 marginTop: "2pt"
                             },
                             children: (0, Kr.jsx)(no, {
                                 label: "Loading VPCs"
                             })
                         }), a.map((function(e) {
                             return (0, Kr.jsx)("div", {
-                                children: (0, Kr.jsx)(Xh, {
+                                children: (0, Kr.jsx)(eg, {
                                     vpc: e,
                                     keyedState: null === r || void 0 === r ? void 0 : r.keyed(e.id)
                                 })
                             }, e.id)
                         }))]
                     })]
                 })
             },
-            Xh = function(e) {
+            eg = function(e) {
                 var t = e.vpc,
                     n = e.keyedState,
-                    r = a(Hh(n), 2),
+                    r = a(Vh(n), 2),
                     o = r[0],
                     i = r[1],
                     s = function(e) {
                         return o[e]
                     },
                     u = function(e) {
                         return i(Be({}, e, !o[e]))
@@ -70794,42 +70822,42 @@
                                 }
                             })]
                         }), (0, Kr.jsx)("table", {
                             width: "100%",
                             children: (0, Kr.jsxs)("tbody", {
                                 children: [(0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "ID:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Vh,
+                                        style: Jh,
                                         children: t.id
                                     })]
                                 }), (null === t || void 0 === t ? void 0 : t.stack) && (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "Stack:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Vh,
+                                        style: Jh,
                                         children: null === t || void 0 === t ? void 0 : t.stack
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "CIDR:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Vh,
+                                        style: Jh,
                                         children: null === t || void 0 === t ? void 0 : t.cidr
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "Status:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Vh,
+                                        style: Jh,
                                         children: null === t || void 0 === t ? void 0 : t.status
                                     })]
                                 }), (0, Kr.jsx)("tr", {
                                     children: (0, Kr.jsx)("td", {
                                         style: {
                                             height: "2pt"
                                         },
@@ -70852,15 +70880,15 @@
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     onClick: function() {
                                         return t.id, u("showSubnetsPublic")
                                     },
                                     className: "pointer",
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "Public Subnets:"
                                     }), (0, Kr.jsx)("td", {
                                         children: l() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("small", {
                                                 children: (0, Kr.jsxs)("u", {
                                                     children: ["Hide\xa0", Fr.DownArrowHollow]
                                                 })
@@ -70876,29 +70904,29 @@
                                 }), l() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             style: {
                                                 paddingTop: "2pt"
                                             },
                                             colSpan: "2",
-                                            children: (0, Kr.jsx)($h, {
+                                            children: (0, Kr.jsx)(tg, {
                                                 type: "public",
                                                 vpcId: null === t || void 0 === t ? void 0 : t.id,
                                                 notitle: !0,
                                                 keyedState: null === n || void 0 === n ? void 0 : n.keyed("subnets-public")
                                             })
                                         })
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     onClick: function() {
                                         return u("showSubnetsPrivate")
                                     },
                                     className: "pointer",
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "Private Subnets:"
                                     }), (0, Kr.jsx)("td", {
                                         children: c() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("small", {
                                                 children: (0, Kr.jsxs)("u", {
                                                     children: ["Hide\xa0", Fr.DownArrowHollow]
                                                 })
@@ -70914,29 +70942,29 @@
                                 }), c() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             style: {
                                                 paddingTop: "2pt"
                                             },
                                             colSpan: "2",
-                                            children: (0, Kr.jsx)($h, {
+                                            children: (0, Kr.jsx)(tg, {
                                                 type: "private",
                                                 vpcId: null === t || void 0 === t ? void 0 : t.id,
                                                 notitle: !0,
                                                 keyedState: null === n || void 0 === n ? void 0 : n.keyed("subnets-private")
                                             })
                                         })
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     onClick: function() {
                                         return u("showSecurityGroups")
                                     },
                                     className: "pointer",
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "Security Groups:"
                                     }), (0, Kr.jsx)("td", {
                                         children: d() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("small", {
                                                 children: (0, Kr.jsxs)("u", {
                                                     children: ["Hide\xa0", Fr.DownArrowHollow]
                                                 })
@@ -70952,28 +70980,28 @@
                                 }), d() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             style: {
                                                 paddingTop: "2pt"
                                             },
                                             colSpan: "2",
-                                            children: (0, Kr.jsx)(tg, {
+                                            children: (0, Kr.jsx)(rg, {
                                                 vpcId: null === t || void 0 === t ? void 0 : t.id,
                                                 notitle: !0,
                                                 keyedState: null === n || void 0 === n ? void 0 : n.keyed("security-groups")
                                             })
                                         })
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     onClick: function() {
                                         return u("showTags")
                                     },
                                     className: "pointer",
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "Tags:"
                                     }), (0, Kr.jsx)("td", {
                                         children: f() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("small", {
                                                 children: (0, Kr.jsxs)("u", {
                                                     children: ["Hide\xa0", Fr.DownArrowHollow]
                                                 })
@@ -70989,26 +71017,26 @@
                                 }), f() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             style: {
                                                 paddingTop: "2pt"
                                             },
                                             colSpan: "2",
-                                            children: (0, Kr.jsx)(ig, {
+                                            children: (0, Kr.jsx)(sg, {
                                                 tags: null === t || void 0 === t ? void 0 : t.tags
                                             })
                                         })
                                     })
                                 })]
                             })
                         })]
                     })
                 })
             },
-            $h = function(e) {
+            tg = function(e) {
                 var t, n, r = e.vpcId,
                     o = e.type,
                     i = e.hide,
                     a = e.notitle,
                     s = e.keyedState,
                     u = "true" === (null === (t = Re()[0].get("all")) || void 0 === t ? void 0 : t.toLowerCase()),
                     l = r ? "?vpc=".concat(r) : "",
@@ -71047,31 +71075,31 @@
                             children: (0, Kr.jsx)(no, {
                                 label: "Loading Subnets"
                             })
                         }), null === (n = c.filter((function(e) {
                             return !o || e.type === o
                         }))) || void 0 === n ? void 0 : n.map((function(e) {
                             return (0, Kr.jsxs)("div", {
-                                children: [(0, Kr.jsx)(eg, {
+                                children: [(0, Kr.jsx)(ng, {
                                     subnet: e,
                                     keyedState: null === s || void 0 === s ? void 0 : s.keyed(e.id)
                                 }), (0, Kr.jsx)("div", {
                                     style: {
                                         height: "4pt"
                                     }
                                 })]
                             }, e.id)
                         }))]
                     })]
                 })
             },
-            eg = function(e) {
+            ng = function(e) {
                 var t = e.subnet,
                     n = e.keyedState,
-                    r = a(Hh(n), 2),
+                    r = a(Vh(n), 2),
                     o = r[0],
                     i = r[1],
                     s = function() {
                         return o["showTags"]
                     };
                 return (0, Kr.jsx)(Kr.Fragment, {
                     children: (0, Kr.jsxs)("div", {
@@ -71119,60 +71147,60 @@
                                 })
                             })]
                         }), (0, Kr.jsx)("table", {
                             width: "100%",
                             children: (0, Kr.jsxs)("tbody", {
                                 children: [(0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "ID:"
                                     }), (0, Kr.jsxs)("td", {
-                                        style: Vh,
+                                        style: Jh,
                                         children: [null === t || void 0 === t ? void 0 : t.id, (0, Kr.jsx)("br", {}), (0, Kr.jsx)("small", {
                                             children: null === t || void 0 === t ? void 0 : t.subnet_arn
                                         })]
                                     })]
                                 }), (null === t || void 0 === t ? void 0 : t.stack) && (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "Stack:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Vh,
+                                        style: Jh,
                                         children: null === t || void 0 === t ? void 0 : t.stack
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "CIDR:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Vh,
+                                        style: Jh,
                                         children: null === t || void 0 === t ? void 0 : t.cidr
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "Zone:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Vh,
+                                        style: Jh,
                                         children: null === t || void 0 === t ? void 0 : t.zone
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "VPC:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Vh,
+                                        style: Jh,
                                         children: null === t || void 0 === t ? void 0 : t.vpc
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "Status:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Vh,
+                                        style: Jh,
                                         children: null === t || void 0 === t ? void 0 : t.status
                                     })]
                                 }), (0, Kr.jsx)("tr", {
                                     children: (0, Kr.jsx)("td", {
                                         style: {
                                             height: "4pt"
                                         },
@@ -71196,15 +71224,15 @@
                                 }), (0, Kr.jsxs)("tr", {
                                     onClick: function() {
                                         return i(Be({}, e = "showTags", !o[e]));
                                         var e
                                     },
                                     className: "pointer",
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "Tags:"
                                     }), (0, Kr.jsx)("td", {
                                         children: s() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("small", {
                                                 children: (0, Kr.jsxs)("u", {
                                                     children: ["Hide\xa0", Fr.DownArrowHollow]
                                                 })
@@ -71220,26 +71248,26 @@
                                 }), s() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             style: {
                                                 paddingTop: "2pt"
                                             },
                                             colSpan: "2",
-                                            children: (0, Kr.jsx)(ig, {
+                                            children: (0, Kr.jsx)(sg, {
                                                 tags: null === t || void 0 === t ? void 0 : t.tags
                                             })
                                         })
                                     })
                                 })]
                             })
                         })]
                     })
                 })
             },
-            tg = function(e) {
+            rg = function(e) {
                 var t, n = e.vpcId,
                     r = e.notitle,
                     o = e.keyedState,
                     i = e.hide,
                     a = "true" === (null === (t = Re()[0].get("all")) || void 0 === t ? void 0 : t.toLowerCase()),
                     s = n ? "?vpc=".concat(n) : "",
                     u = Xi("/aws/security_groups".concat(a ? "/all" : "").concat(s), {
@@ -71275,31 +71303,31 @@
                                 marginTop: "2pt"
                             },
                             children: (0, Kr.jsx)(no, {
                                 label: "Loading security groups"
                             })
                         }), u.map((function(e) {
                             return (0, Kr.jsxs)("div", {
-                                children: [(0, Kr.jsx)(ng, {
+                                children: [(0, Kr.jsx)(og, {
                                     securityGroup: e,
                                     keyedState: null === o || void 0 === o ? void 0 : o.keyed(e.id)
                                 }), (0, Kr.jsx)("div", {
                                     style: {
                                         height: "4pt"
                                     }
                                 })]
                             }, e.id)
                         }))]
                     })]
                 })
             },
-            ng = function(e) {
+            og = function(e) {
                 var t = e.securityGroup,
                     n = e.keyedState,
-                    r = a(Hh(n), 2),
+                    r = a(Vh(n), 2),
                     o = r[0],
                     i = r[1],
                     s = function(e) {
                         return o[e]
                     },
                     u = function(e) {
                         return i(Be({}, e, !o[e]))
@@ -71341,47 +71369,47 @@
                                 }
                             })]
                         }), (0, Kr.jsx)("table", {
                             width: "100%",
                             children: (0, Kr.jsxs)("tbody", {
                                 children: [(0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "ID:"
                                     }), (0, Kr.jsxs)("td", {
-                                        style: Vh,
+                                        style: Jh,
                                         children: [null === t || void 0 === t ? void 0 : t.id, (0, Kr.jsx)("br", {}), (0, Kr.jsx)("small", {
                                             children: null === t || void 0 === t ? void 0 : t.securityGroup
                                         })]
                                     })]
                                 }), (null === t || void 0 === t ? void 0 : t.stack) && (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "Stack:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Vh,
+                                        style: Jh,
                                         children: null === t || void 0 === t ? void 0 : t.stack
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "Description:"
                                     }), (0, Kr.jsx)("td", {
                                         style: {
                                             whiteSpace: "break-spaces",
                                             wordBreak: "break-all"
                                         },
                                         children: null === t || void 0 === t ? void 0 : t.description
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "VPC:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Vh,
+                                        style: Jh,
                                         children: null === t || void 0 === t ? void 0 : t.vpc
                                     })]
                                 }), (0, Kr.jsx)("tr", {
                                     children: (0, Kr.jsx)("td", {
                                         style: {
                                             height: "4pt"
                                         },
@@ -71404,15 +71432,15 @@
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     onClick: function() {
                                         return u("showInboundRules")
                                     },
                                     className: "pointer",
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "Inbound Rules:"
                                     }), (0, Kr.jsx)("td", {
                                         children: l() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsxs)("small", {
                                                 children: [(0, Kr.jsx)("u", {
                                                     children: "Hide"
                                                 }), "\xa0", Fr.DownArrowHollow]
@@ -71428,27 +71456,27 @@
                                 }), l() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             style: {
                                                 paddingTop: "2pt"
                                             },
                                             colSpan: "2",
-                                            children: (0, Kr.jsx)(rg, {
+                                            children: (0, Kr.jsx)(ig, {
                                                 securityGroupId: null === t || void 0 === t ? void 0 : t.id,
                                                 direction: "inbound"
                                             })
                                         })
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     onClick: function() {
                                         return u("showOutboundRules")
                                     },
                                     className: "pointer",
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "Outbound Rules:"
                                     }), (0, Kr.jsx)("td", {
                                         children: c() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("small", {
                                                 children: (0, Kr.jsxs)("u", {
                                                     children: ["Hide\xa0", Fr.DownArrowHollow]
                                                 })
@@ -71464,27 +71492,27 @@
                                 }), c() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             style: {
                                                 paddingTop: "2pt"
                                             },
                                             colSpan: "2",
-                                            children: (0, Kr.jsx)(rg, {
+                                            children: (0, Kr.jsx)(ig, {
                                                 securityGroupId: null === t || void 0 === t ? void 0 : t.id,
                                                 direction: "outbound"
                                             })
                                         })
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     onClick: function() {
                                         return u("showTags")
                                     },
                                     className: "pointer",
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "Tags:"
                                     }), (0, Kr.jsx)("td", {
                                         children: d() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("small", {
                                                 children: (0, Kr.jsxs)("u", {
                                                     children: ["Hide\xa0", Fr.DownArrowHollow]
                                                 })
@@ -71500,26 +71528,26 @@
                                 }), d() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             style: {
                                                 paddingTop: "2pt"
                                             },
                                             colSpan: "2",
-                                            children: (0, Kr.jsx)(ig, {
+                                            children: (0, Kr.jsx)(sg, {
                                                 tags: null === t || void 0 === t ? void 0 : t.tags
                                             })
                                         })
                                     })
                                 })]
                             })
                         })]
                     })
                 })
             },
-            rg = function(e) {
+            ig = function(e) {
                 var t = e.securityGroupId,
                     n = e.direction,
                     r = "inbound" === n ? "?direction=inbound" : "outbound" === n ? "?direction=outbound" : "",
                     o = Xi("/aws/security_group_rules/".concat(t).concat(r), {
                         cache: !0
                     });
                 return (0, Kr.jsxs)(Kr.Fragment, {
@@ -71529,26 +71557,26 @@
                             paddingBottom: "10pt"
                         },
                         children: (0, Kr.jsx)(no, {
                             label: "Loading security group rules"
                         })
                     }), null === o || void 0 === o ? void 0 : o.map((function(e) {
                         return (0, Kr.jsxs)("div", {
-                            children: [(0, Kr.jsx)(og, {
+                            children: [(0, Kr.jsx)(ag, {
                                 securityGroupRule: e
                             }), (0, Kr.jsx)("div", {
                                 style: {
                                     height: "4pt"
                                 }
                             })]
                         }, e.id)
                     }))]
                 })
             },
-            og = function(e) {
+            ag = function(e) {
                 var t = e.securityGroupRule;
 
                 function n(e) {
                     var t, n;
                     if ("TCP" === (null === e || void 0 === e || null === (t = e.protocol) || void 0 === t ? void 0 : t.toUpperCase())) {
                         if (22 === (null === e || void 0 === e ? void 0 : e.port_from) && 22 === (null === e || void 0 === e ? void 0 : e.port_thru)) return "SSH";
                         if (443 === (null === e || void 0 === e ? void 0 : e.port_from) && 443 === (null === e || void 0 === e ? void 0 : e.port_thru)) return "HTTPS";
@@ -71603,78 +71631,78 @@
                                 }
                             })]
                         }), (0, Kr.jsx)("table", {
                             width: "100%",
                             children: (0, Kr.jsxs)("tbody", {
                                 children: [(0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "Direction:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Vh,
+                                        style: Jh,
                                         children: null !== t && void 0 !== t && t.egress ? "Outbound" : "Inbound"
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "Protocol:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Vh,
+                                        style: Jh,
                                         children: r(t)
                                     })]
                                 }), n(t) !== r(t) && (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "Type:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Vh,
+                                        style: Jh,
                                         children: n(t)
                                     })]
                                 }), o(t) && (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "Port:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Vh,
+                                        style: Jh,
                                         children: o(t)
                                     })]
                                 }), (null === t || void 0 === t ? void 0 : t.cidr) && (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "CIDR:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Vh,
+                                        style: Jh,
                                         children: null === t || void 0 === t ? void 0 : t.cidr
                                     })]
                                 }), (null === t || void 0 === t ? void 0 : t.description) && (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "Description:"
                                     }), (0, Kr.jsx)("td", {
                                         style: {
                                             whiteSpace: "break-spaces",
                                             wordBreak: "break-all"
                                         },
                                         children: null === t || void 0 === t ? void 0 : t.description
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "Security Group:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Vh,
+                                        style: Jh,
                                         children: null === t || void 0 === t ? void 0 : t.security_group
                                     })]
                                 })]
                             })
                         })]
                     })
                 })
             },
-            ig = function(e) {
+            sg = function(e) {
                 var t;
                 return (0, Kr.jsx)("div", {
                     style: {
                         maxWidth: "480pt"
                     },
                     children: (0, Kr.jsx)("div", {
                         className: "box lighten",
@@ -71709,15 +71737,15 @@
                             children: (0, Kr.jsx)("li", {
                                 children: "No tags."
                             })
                         })
                     })
                 })
             },
-            ag = function(e) {
+            ug = function(e) {
                 var t = Xi("/aws/stacks", {
                         cache: !0
                     }),
                     n = {
                         cursor: "pointer"
                     },
                     r = Ye(Ye({}, n), {}, {
@@ -71748,19 +71776,19 @@
                                 },
                                 children: o.name
                             }, o.name)
                         }))]
                     })]
                 })
             },
-            sg = function(e) {
+            lg = function(e) {
                 var t, n, r, o, i, s, u, l, c, d, f, p, h = e.stackName,
                     g = e.keyedState,
                     y = e.hide,
-                    m = a(Hh(g), 2),
+                    m = a(Vh(g), 2),
                     v = m[0],
                     M = m[1],
                     b = Xi("/aws/stacks/".concat(h), {
                         cache: !0
                     }),
                     j = function(e) {
                         return v[e]
@@ -71812,56 +71840,56 @@
                         children: b.loading ? (0, Kr.jsx)(no, {
                             label: "Loading stack info"
                         }) : (0, Kr.jsx)("table", {
                             width: "100%",
                             children: (0, Kr.jsxs)("tbody", {
                                 children: [(0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "Name:"
                                     }), (0, Kr.jsxs)("td", {
-                                        style: Ye(Ye({}, Vh), {}, {
+                                        style: Ye(Ye({}, Jh), {}, {
                                             wordBreak: "break-all"
                                         }),
                                         children: [(0, Kr.jsx)("b", {
                                             style: {
                                                 float: "right",
                                                 cursor: "pointer",
                                                 marginTop: "-2pt"
                                             },
                                             onClick: y,
                                             children: Fr.X
                                         }), h]
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "ID:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Ye(Ye({}, Vh), {}, {
+                                        style: Ye(Ye({}, Jh), {}, {
                                             wordBreak: "break-all"
                                         }),
                                         children: (0, Kr.jsx)("small", {
                                             children: null === (n = b.data) || void 0 === n ? void 0 : n.id
                                         })
                                     })]
                                 }), (null === (r = b.data) || void 0 === r ? void 0 : r.role_arn) && (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "Role:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Vh,
+                                        style: Jh,
                                         children: (null === (o = b.data) || void 0 === o ? void 0 : o.role_arn) || Fr.EmptySet
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "Description:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Vh,
+                                        style: Jh,
                                         children: null === (i = b.data) || void 0 === i ? void 0 : i.description
                                     })]
                                 }), (0, Kr.jsx)("tr", {
                                     children: (0, Kr.jsx)("td", {
                                         style: {
                                             height: "2pt"
                                         },
@@ -71880,34 +71908,34 @@
                                         style: {
                                             height: "2pt"
                                         },
                                         colSpan: "2"
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "Status:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Vh,
+                                        style: Jh,
                                         children: null === (s = b.data) || void 0 === s ? void 0 : s.status
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "Created:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Vh,
+                                        style: Jh,
                                         children: null === (u = b.data) || void 0 === u ? void 0 : u.created
                                     })]
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "Updated:"
                                     }), (0, Kr.jsx)("td", {
-                                        style: Vh,
+                                        style: Jh,
                                         children: null === (l = b.data) || void 0 === l ? void 0 : l.updated
                                     })]
                                 }), (0, Kr.jsx)("tr", {
                                     children: (0, Kr.jsx)("td", {
                                         style: {
                                             height: "2pt"
                                         },
@@ -71926,18 +71954,18 @@
                                         style: {
                                             height: "2pt"
                                         },
                                         colSpan: "2"
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "Outputs:"
                                     }), (0, Kr.jsxs)("td", {
-                                        style: Vh,
+                                        style: Jh,
                                         children: [x() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("small", {
                                                 className: "pointer",
                                                 onClick: N,
                                                 children: (0, Kr.jsxs)("u", {
                                                     children: ["Hide\xa0", Fr.DownArrowHollow]
                                                 })
@@ -71962,25 +71990,25 @@
                                 }), x() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             colSpan: "2",
                                             style: {
                                                 paddingTop: "2pt"
                                             },
-                                            children: (0, Kr.jsx)(ug, {
+                                            children: (0, Kr.jsx)(cg, {
                                                 stackName: h
                                             })
                                         })
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "Parameters:"
                                     }), (0, Kr.jsxs)("td", {
-                                        style: Vh,
+                                        style: Jh,
                                         children: [I() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("small", {
                                                 className: "pointer",
                                                 onClick: D,
                                                 children: (0, Kr.jsxs)("u", {
                                                     children: ["Hide\xa0", Fr.DownArrowHollow]
                                                 })
@@ -72005,25 +72033,25 @@
                                 }), I() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             colSpan: "2",
                                             style: {
                                                 paddingTop: "2pt"
                                             },
-                                            children: (0, Kr.jsx)(lg, {
+                                            children: (0, Kr.jsx)(dg, {
                                                 stackName: h
                                             })
                                         })
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "Resources:"
                                     }), (0, Kr.jsxs)("td", {
-                                        style: Vh,
+                                        style: Jh,
                                         children: [S() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("small", {
                                                 className: "pointer",
                                                 onClick: L,
                                                 children: (0, Kr.jsxs)("u", {
                                                     children: ["Hide\xa0", Fr.DownArrowHollow]
                                                 })
@@ -72048,25 +72076,25 @@
                                 }), S() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             colSpan: "2",
                                             style: {
                                                 paddingTop: "2pt"
                                             },
-                                            children: (0, Kr.jsx)(cg, {
+                                            children: (0, Kr.jsx)(fg, {
                                                 stackName: h
                                             })
                                         })
                                     })
                                 }), (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
-                                        style: Zh,
+                                        style: qh,
                                         children: "Template:"
                                     }), (0, Kr.jsxs)("td", {
-                                        style: Vh,
+                                        style: Jh,
                                         children: [k() ? (0, Kr.jsx)(Kr.Fragment, {
                                             children: (0, Kr.jsx)("small", {
                                                 className: "pointer",
                                                 onClick: C,
                                                 children: (0, Kr.jsxs)("u", {
                                                     children: ["Hide\xa0", Fr.DownArrowHollow]
                                                 })
@@ -72091,26 +72119,26 @@
                                 }), k() && (0, Kr.jsx)(Kr.Fragment, {
                                     children: (0, Kr.jsx)("tr", {
                                         children: (0, Kr.jsx)("td", {
                                             colSpan: "2",
                                             style: {
                                                 paddingTop: "2pt"
                                             },
-                                            children: (0, Kr.jsx)(dg, {
+                                            children: (0, Kr.jsx)(pg, {
                                                 stackName: h
                                             })
                                         })
                                     })
                                 })]
                             })
                         })
                     })]
                 })
             },
-            ug = function(e) {
+            cg = function(e) {
                 var t, n = Xi("/aws/stacks/".concat(e.stackName, "/outputs"), {
                     cache: !0
                 });
                 return (0, Kr.jsx)("div", {
                     style: {
                         maxWidth: "480pt"
                     },
@@ -72153,15 +72181,15 @@
                                     }, e)
                                 })))
                             })
                         })
                     })
                 })
             },
-            lg = function(e) {
+            dg = function(e) {
                 var t, n = Xi("/aws/stacks/".concat(e.stackName, "/parameters"), {
                     cache: !0
                 });
                 return (0, Kr.jsx)("div", {
                     style: {
                         maxWidth: "480pt"
                     },
@@ -72204,15 +72232,15 @@
                                     }, e)
                                 })))
                             })
                         })
                     })
                 })
             },
-            cg = function(e) {
+            fg = function(e) {
                 var t, n = Xi("/aws/stacks/".concat(e.stackName, "/resources"), {
                     cache: !0
                 });
                 return (0, Kr.jsx)("div", {
                     style: {
                         maxWidth: "480pt"
                     },
@@ -72258,15 +72286,15 @@
                                     }, e)
                                 })))
                             })
                         })
                     })
                 })
             },
-            dg = function(e) {
+            pg = function(e) {
                 var t = Xi("/aws/stacks/".concat(e.stackName, "/template"), {
                     cache: !0
                 });
                 return (0, Kr.jsx)("div", {
                     style: {
                         maxWidth: "480pt"
                     },
@@ -72293,15 +72321,15 @@
                                 },
                                 children: st.IsObject(t.data) ? Bi.Format(t.data) : t.data
                             })
                         })
                     })
                 })
             },
-            fg = function(e) {
+            hg = function(e) {
                 var t, n, r, o, i, a, s = e.hide,
                     u = Xi("/info", {
                         cache: !0
                     });
                 return (0, Kr.jsxs)("div", {
                     style: {
                         maxWidth: "500pt",
@@ -72352,15 +72380,15 @@
                                     }) : u.data.gac.values[e]]
                                 }, e)
                             })))
                         })]
                     })]
                 })
             },
-            pg = function(e) {
+            gg = function(e) {
                 var t, n, r, o, i = e.hide,
                     a = Xi("/info", {
                         cache: !0
                     });
                 return (0, Kr.jsxs)("div", {
                     style: {
                         maxWidth: "500pt",
@@ -72386,81 +72414,81 @@
                         className: "box margin",
                         children: [a.loading && (0, Kr.jsx)(no, {
                             label: "Loading Ecosystem"
                         }), !a.loading && Bi.Format(null === (r = a.data) || void 0 === r || null === (o = r.buckets) || void 0 === o ? void 0 : o.ecosystem)]
                     })]
                 })
             },
-            hg = function() {
-                var e = Hh(),
+            yg = function() {
+                var e = Vh(),
                     n = [{
                         type: "stack",
                         create: function(e, t, n, r) {
                             var o = r.keyedState;
-                            return (0, Kr.jsx)(sg, {
+                            return (0, Kr.jsx)(lg, {
                                 stackName: e,
                                 keyedState: o.keyed(t),
                                 hide: n
                             })
                         }
                     }, {
                         type: "vpcs",
                         create: function(e, t, n, r) {
                             var o = r.keyedState;
-                            return (0, Kr.jsx)(Kh, {
+                            return (0, Kr.jsx)($h, {
                                 keyedState: o.keyed(t),
                                 hide: n
                             })
                         }
                     }, {
                         type: "subnets-public",
                         create: function(e, t, n, r) {
                             var o = r.keyedState;
-                            return (0, Kr.jsx)($h, {
+                            return (0, Kr.jsx)(tg, {
                                 type: "public",
                                 keyedState: o.keyed(t),
                                 hide: n
                             })
                         }
                     }, {
                         type: "subnets-private",
                         create: function(e, t, n, r) {
                             var o = r.keyedState;
-                            return (0, Kr.jsx)($h, {
+                            return (0, Kr.jsx)(tg, {
                                 type: "private",
                                 keyedState: o.keyed(t),
                                 hide: n
                             })
                         }
                     }, {
                         type: "security-groups",
                         create: function(e, t, n, r) {
                             var o = r.keyedState;
-                            return (0, Kr.jsx)(tg, {
+                            return (0, Kr.jsx)(rg, {
                                 keyedState: o.keyed(t),
                                 hide: n
                             })
                         }
                     }, {
                         type: "gac",
                         create: function(e, t, n, r) {
-                            return (0, Kr.jsx)(fg, {
+                            return (0, Kr.jsx)(hg, {
                                 hide: n
                             })
                         }
                     }, {
                         type: "ecosystem",
                         create: function(e, t, n, r) {
-                            return (0, Kr.jsx)(pg, {
+                            return (0, Kr.jsx)(gg, {
                                 hide: n
                             })
                         }
                     }],
-                    r = Yh(n),
-                    o = Yh(n);
+                    r = Gh(n),
+                    o = Gh(n);
                 var i = function() {
                         return r.toggle("vpcs")
                     },
                     a = function() {
                         return r.toggle("ecosystem")
                     };
                 return (0, t.useEffect)((function() {
@@ -72469,15 +72497,15 @@
                     children: (0, Kr.jsx)("tbody", {
                         children: (0, Kr.jsxs)("tr", {
                             children: [(0, Kr.jsxs)("td", {
                                 style: {
                                     verticalAlign: "top",
                                     paddingRight: "8pt"
                                 },
-                                children: [(0, Kr.jsx)(qh, {
+                                children: [(0, Kr.jsx)(Kh, {
                                     keyedState: e,
                                     showVpcs: function() {
                                         return r.selected("vpcs")
                                     },
                                     toggleVpcs: i,
                                     showSubnetsPublic: function() {
                                         return o.selected("subnets-public")
@@ -72493,26 +72521,26 @@
                                     },
                                     showSecurityGroups: function() {
                                         return o.selected("security-groups")
                                     },
                                     toggleSecurityGroups: function() {
                                         return o.toggle("security-groups")
                                     }
-                                }), (0, Kr.jsx)(Jh, {
+                                }), (0, Kr.jsx)(Xh, {
                                     showGac: function() {
                                         return r.selected("gac")
                                     },
                                     toggleGac: function() {
                                         return r.toggle("gac")
                                     },
                                     showEcosystem: function() {
                                         return r.selected("ecosystem")
                                     },
                                     toggleEcosystem: a
-                                }), (0, Kr.jsx)(ag, {
+                                }), (0, Kr.jsx)(ug, {
                                     toggleStack: function(e) {
                                         return r.toggle("stack", e)
                                     },
                                     selectedStack: function(e) {
                                         return r.selected("stack", e)
                                     }
                                 })]
@@ -72541,15 +72569,15 @@
                                     }, t.key)
                                 }))
                             })]
                         })
                     })
                 })
             },
-            gg = function(e) {
+            mg = function(e) {
                 var t = ta();
                 return (0, Kr.jsx)(Kr.Fragment, {
                     children: (0, Kr.jsx)("div", {
                         className: "container",
                         id: "login_container",
                         children: (0, Kr.jsxs)("div", {
                             className: "boxstyle check-warn",
@@ -72578,56 +72606,56 @@
                                     })
                                 }), " page."]
                             })]
                         })
                     })
                 })
             },
-            yg = function() {
+            vg = function() {
                 var e = ce().state.url;
                 return e.startsWith(window.location.origin) && (e = e.substring(window.location.origin.length)), (0, Kr.jsx)(xe, {
                     to: e,
                     replace: !0
                 })
             },
-            mg = function(e) {
+            Mg = function(e) {
                 return (0, Kr.jsx)(Kr.Fragment, {
                     children: (0, Kr.jsx)("div", {
                         className: "box thickborder",
                         style: {
                             marginBottom: "6pt"
                         },
                         children: (0, Kr.jsx)(Si, {
                             certificate: e.certificate
                         })
                     })
                 })
             },
-            vg = function(e) {
+            bg = function(e) {
                 var t, n = a(Re(), 1)[0].get("hostname"),
                     r = Xi("/certificates?hostname=".concat(n));
                 return (0, Kr.jsx)(Kr.Fragment, {
                     children: (0, Kr.jsxs)("div", {
                         className: "container",
                         style: {
                             width: "800pt"
                         },
                         children: [(0, Kr.jsx)("b", {
                             children: "SSL Certificates"
                         }), null === r || void 0 === r || null === (t = r.data) || void 0 === t ? void 0 : t.map((function(e) {
                             return (0, Kr.jsx)("div", {
-                                children: (0, Kr.jsx)(mg, {
+                                children: (0, Kr.jsx)(Mg, {
                                     certificate: e
                                 })
                             }, e.serial_number)
                         }))]
                     })
                 })
             },
-            Mg = function(e) {
+            jg = function(e) {
                 var t = Xi("/portal_access_key");
                 return (0, Kr.jsx)(Kr.Fragment, {
                     children: (0, Kr.jsxs)("div", {
                         className: "container",
                         style: {
                             width: "800pt"
                         },
@@ -72641,15 +72669,15 @@
                             children: (0, Kr.jsx)(Ii, {
                                 accessKey: t.data
                             })
                         })]
                     })
                 })
             },
-            bg = function() {
+            wg = function() {
                 var e = Xi("/users/projects", {
                         cache: !0
                     }),
                     t = Xi("/users/roles", {
                         cache: !0
                     }),
                     n = Xi("/users/institutions", {
@@ -72707,15 +72735,15 @@
                             return (null === e || void 0 === e ? void 0 : e.map((function(e) {
                                 return o.title(e)
                             })).join(", ")) || ""
                         }
                     };
                 return o
             },
-            jg = [{
+            xg = [{
                 name: "email",
                 label: "Email Address",
                 type: "email",
                 focus: !0,
                 required: !0
             }, {
                 name: "first_name",
@@ -72760,38 +72788,38 @@
                 label: "Updated",
                 readonly: !0
             }, {
                 name: "uuid",
                 label: "UUID",
                 readonly: !0
             }],
-            wg = {
+            Ng = {
                 PrincipalInvestigatorLine: function(e) {
                     var t, n, r = e.institution,
-                        o = bg();
+                        o = wg();
                     return (0, Kr.jsx)("div", {
                         style: e.style,
                         children: o.principleInvestigator(r) && (0, Kr.jsxs)("small", {
                             children: [(0, Kr.jsxs)("b", {
                                 children: ["Principle Investigator ", Fr.RightArrow]
                             }), " ", null === (t = o.principleInvestigator(r)) || void 0 === t ? void 0 : t.name, "\xa0", (0, Kr.jsx)(Ni, {
                                 href: kr.Path("/users/".concat(null === (n = o.principleInvestigator(r)) || void 0 === n ? void 0 : n.uuid))
                             })]
                         })
                     })
                 },
                 useUserInputs: function() {
                     var e = ta(),
-                        n = At.IsFoursightFourfront(e) ? jg.filter((function(e) {
+                        n = At.IsFoursightFourfront(e) ? xg.filter((function(e) {
                             return "project" !== e.name && "role" !== e.name && "institution" !== e.name
-                        })) : jg;
+                        })) : xg;
                     return (0, t.useState)(Tr.Clone(Tr.Clone(n)))
                 }
             },
-            xg = function(e) {
+            Ig = function(e) {
                 var t = Xi("/users/".concat(e.email, "?raw=true"));
                 return (0, Kr.jsxs)("pre", {
                     className: "box",
                     children: [(0, Kr.jsx)("span", {
                         style: {
                             float: "right",
                             marginTop: "-6pt",
@@ -72805,15 +72833,15 @@
                     }), t.loading ? (0, Kr.jsx)(Kr.Fragment, {
                         children: (0, Kr.jsx)(no, {})
                     }) : (0, Kr.jsx)(Kr.Fragment, {
                         children: Bi.Format(t.data)
                     })]
                 })
             },
-            Ng = function(e) {
+            Dg = function(e) {
                 var n = {
                         color: "var(--box-fg)",
                         fontWeight: "bold",
                         fontSize: "small",
                         paddingTop: "1pt",
                         verticalAlign: "top",
                         width: "5%",
@@ -72922,16 +72950,16 @@
                                     })]
                                 }, o.name)
                             }))
                         })
                     })
                 })
             },
-            Ig = function(e) {
-                var t = bg(),
+            Sg = function(e) {
+                var t = wg(),
                     n = [{
                         label: "Email",
                         name: "email"
                     }, {
                         label: "First Name",
                         name: "first_name"
                     }, {
@@ -72954,26 +72982,26 @@
                         name: "role",
                         map: function(n) {
                             return t.userRoleTitle(e.user, e.user.project)
                         }
                     }, {
                         label: "Roles",
                         name: "roles",
-                        ui: (0, Kr.jsx)(Dg, {
+                        ui: (0, Kr.jsx)(Lg, {
                             user: e.user
                         }),
                         toggle: !0
                     }, {
                         label: "Institution",
                         name: "institution",
                         map: function(e) {
                             return t.institutionTitle(e)
                         },
                         subComponent: function(e) {
-                            return (0, Kr.jsx)(wg.PrincipalInvestigatorLine, {
+                            return (0, Kr.jsx)(Ng.PrincipalInvestigatorLine, {
                                 institution: e
                             })
                         }
                     }, {
                         label: "Status",
                         name: "status",
                         map: function(e) {
@@ -72993,22 +73021,22 @@
                         }
                     }, {
                         label: "UUID",
                         name: "uuid"
                     }];
                 return At.IsFoursightFourfront(ta()) && (n = n.filter((function(e) {
                     return "institution" !== e.name && "project" !== e.name && "roles" !== e.name && "role" !== e.name
-                }))), (0, Kr.jsx)(Ng, {
+                }))), (0, Kr.jsx)(Dg, {
                     keys: n,
                     value: e.user,
                     separators: !0
                 })
             },
-            Dg = function(e) {
-                var t = bg();
+            Lg = function(e) {
+                var t = wg();
                 return (0, Kr.jsx)("div", {
                     className: "box lighten",
                     style: {
                         marginTop: "2pt",
                         marginBottom: "2pt"
                     },
                     children: (0, Kr.jsx)("table", {
@@ -73071,15 +73099,15 @@
                                     })]
                                 }, e.project)
                             }))]
                         })
                     })
                 })
             },
-            Sg = function(e) {
+            kg = function(e) {
                 var n, r, o, i = pe().email,
                     s = a((0, t.useState)(!1), 2),
                     u = s[0],
                     l = s[1],
                     c = fe();
                 var d = Xi({
                     url: "/users/".concat(i),
@@ -73195,25 +73223,25 @@
                                             float: "right",
                                             fontSize: "small",
                                             marginTop: "-1pt",
                                             marginRight: "2pt"
                                         },
                                         children: "Edit"
                                     })]
-                                }), u ? (0, Kr.jsx)(xg, {
+                                }), u ? (0, Kr.jsx)(Ig, {
                                     email: e.email
-                                }) : (0, Kr.jsx)(Ig, {
+                                }) : (0, Kr.jsx)(Sg, {
                                     user: e
                                 })]
                             }, e.uuid)
                         }))]
                     })
                 })
             },
-            Lg = function(e) {
+            Cg = function(e) {
                 var n = Xi(e.url, {
                         nofetch: !0,
                         cache: !0
                     }),
                     r = a((0, t.useState)(e.selected), 2),
                     o = r[0],
                     i = r[1];
@@ -73246,15 +73274,15 @@
                             }, e.id) : null
                         }))]
                     }), e.subComponent && (0, Kr.jsx)(Kr.Fragment, {
                         children: e.subComponent(o)
                     })]
                 })
             },
-            kg = function(e) {
+            Eg = function(e) {
                 var n = e.inputs,
                     r = (e.setInputs, e.title, e.loading),
                     o = e.onCreate,
                     i = e.onUpdate,
                     u = e.onDelete,
                     l = e.onCancel,
                     c = e.onRefresh,
@@ -73506,15 +73534,15 @@
                                                         }), (0, Kr.jsx)("option", {
                                                             value: !0,
                                                             children: "True"
                                                         })]
                                                     })
                                                 }) : (0, Kr.jsx)(Kr.Fragment, {
                                                     children: "select" === e.type ? (0, Kr.jsx)(Kr.Fragment, {
-                                                        children: (0, Kr.jsx)(Lg, {
+                                                        children: (0, Kr.jsx)(Cg, {
                                                             id: e.name,
                                                             url: e.url,
                                                             required: e.required,
                                                             selected: z(e),
                                                             onChange: T,
                                                             disabled: F() || e.readonly,
                                                             setLoadingCount: S,
@@ -73690,28 +73718,28 @@
                                     })]
                                 })
                             })
                         })
                     })
                 })
             },
-            Cg = function() {
+            _g = function() {
                 var e = Xi(zt.Url("/users"), {
                         method: "POST",
                         nofetch: !0
                     }),
-                    n = a(wg.useUserInputs(), 2),
+                    n = a(Ng.useUserInputs(), 2),
                     r = n[0],
                     o = (n[1], fe());
                 return (0, t.useEffect)((function() {
                     var e = r.find((function(e) {
                         return "institution" === e.name
                     }));
                     e && (e.subComponent = function(e) {
-                        return (0, Kr.jsx)(wg.PrincipalInvestigatorLine, {
+                        return (0, Kr.jsx)(Ng.PrincipalInvestigatorLine, {
                             institution: e
                         })
                     })
                 }), []), (0, Kr.jsx)("center", {
                     children: (0, Kr.jsx)("table", {
                         children: (0, Kr.jsxs)("tbody", {
                             children: [(0, Kr.jsx)("tr", {
@@ -73738,15 +73766,15 @@
                                                 children: "List"
                                             })
                                         })
                                     })]
                                 })
                             }), (0, Kr.jsx)("tr", {
                                 children: (0, Kr.jsx)("td", {
-                                    children: (0, Kr.jsx)(kg, {
+                                    children: (0, Kr.jsx)(Eg, {
                                         title: "Edit User",
                                         inputs: r,
                                         onCreate: function(t) {
                                             t.admin ? (delete t.admin, t = Ye(Ye({}, t), {}, {
                                                 groups: ["admin"]
                                             })) : (delete t.admin, t = Ye(Ye({}, t), {}, {
                                                 groups: []
@@ -73766,17 +73794,17 @@
                                     })
                                 })
                             })]
                         })
                     })
                 })
             },
-            Eg = function() {
+            Tg = function() {
                 var e = pe().uuid,
-                    n = a(wg.useUserInputs(), 2),
+                    n = a(Ng.useUserInputs(), 2),
                     r = n[0],
                     o = n[1],
                     i = a((0, t.useState)(!1), 2),
                     l = i[0],
                     c = i[1],
                     d = a(ma(), 1)[0],
                     f = Xi({
@@ -73800,27 +73828,27 @@
                                 return u(t)
                             }))
                         },
                         onError: function(e) {
                             404 === e.status && c(!0)
                         }
                     }),
-                    p = bg(),
+                    p = wg(),
                     h = fe();
 
                 function g() {
                     h(kr.Path("/users/".concat(e)))
                 }
                 return (0, t.useEffect)((function() {
                     f.fetch();
                     var e = r.find((function(e) {
                         return "institution" === e.name
                     }));
                     e && (e.subComponent = function(e) {
-                        return (0, Kr.jsx)(wg.PrincipalInvestigatorLine, {
+                        return (0, Kr.jsx)(Ng.PrincipalInvestigatorLine, {
                             institution: e
                         })
                     })
                 }), [e]), (0, Kr.jsx)("center", {
                     children: (0, Kr.jsx)("table", {
                         children: (0, Kr.jsxs)("tbody", {
                             children: [(0, Kr.jsx)("tr", {
@@ -73861,15 +73889,15 @@
                                             children: ["The specified user was not found: ", e, " ", (0, Kr.jsx)("p", {}), (0, Kr.jsx)("button", {
                                                 className: "button cancel",
                                                 onClick: g,
                                                 children: "Cancel"
                                             })]
                                         })
                                     }) : (0, Kr.jsx)(Kr.Fragment, {
-                                        children: (0, Kr.jsx)(kg, {
+                                        children: (0, Kr.jsx)(Eg, {
                                             title: "Edit User",
                                             inputs: r,
                                             setInputs: o,
                                             onUpdate: function(t) {
                                                 var n, r = (null === (n = f.get("groups")) || void 0 === n ? void 0 : n.filter((function(e) {
                                                     return "admin" !== e
                                                 }))) || [];
@@ -73904,15 +73932,15 @@
                                     })
                                 })
                             })]
                         })
                     })
                 })
             },
-            _g = function(e) {
+            Ag = function(e) {
                 var n, r = e.columns,
                     o = e.data,
                     i = e.update,
                     s = e.initialSort,
                     u = e.children,
                     l = a(Re(), 2),
                     c = l[0],
@@ -73993,15 +74021,15 @@
                         border: "0",
                         children: (0, Kr.jsx)("tbody", {
                             children: (0, Kr.jsxs)("tr", {
                                 children: [(0, Kr.jsx)("td", {
                                     style: {
                                         width: "90%"
                                     },
-                                    children: (0, Kr.jsx)(ts, {
+                                    children: (0, Kr.jsx)(rs, {
                                         pages: _,
                                         page: k,
                                         onChange: function(e) {
                                             var t = e.selected;
                                             m(t * p)
                                         },
                                         refresh: R,
@@ -74092,27 +74120,27 @@
                             }), (0, Kr.jsx)("tbody", {
                                 children: u
                             })]
                         })
                     })]
                 })
             },
-            Tg = function() {
+            Og = function() {
                 var e = pe().environ,
                     n = a(Re(), 2),
                     r = n[0],
                     o = n[1],
                     i = Xi(),
                     s = a((0, t.useState)(r.get("search") || ""), 2),
                     u = s[0],
                     l = s[1],
                     c = a((0, t.useState)(it.HasValue(u)), 2),
                     d = c[0],
                     f = c[1],
-                    p = bg();
+                    p = wg();
 
                 function h(t) {
                     var n = t.limit,
                         o = t.offset,
                         a = t.sort,
                         s = t.search,
                         u = t.onDone;
@@ -74239,15 +74267,15 @@
                                 style: {
                                     height: "1px",
                                     background: Ft.GetForegroundColor(),
                                     marginTop: "2pt",
                                     marginBottom: "4pt"
                                 }
                             })]
-                        }), (0, Kr.jsx)(_g, {
+                        }), (0, Kr.jsx)(Ag, {
                             columns: [{
                                 label: ""
                             }, {
                                 label: "User",
                                 key: "email"
                             }, {
                                 label: "Groups",
@@ -74376,30 +74404,30 @@
                                     })]
                                 }, e.uuid)
                             }))
                         })]
                     })
                 })
             },
-            Ag = function() {
+            zg = function() {
                 var e = ta();
 
                 function t() {
                     return "/api/react/".concat(At.PreferredName(At.Default(e)), "/login")
                 }
                 return (0, Kr.jsx)(Ae, {
-                    children: (0, Kr.jsxs)(bs, {
-                        children: [(0, Kr.jsx)(Ms, {}), (0, Kr.jsx)("div", {
+                    children: (0, Kr.jsxs)(ws, {
+                        children: [(0, Kr.jsx)(js, {}), (0, Kr.jsx)("div", {
                             style: {
                                 margin: "14pt"
                             },
                             children: (0, Kr.jsxs)(De, {
                                 children: [(0, Kr.jsx)(Ne, {
                                     path: "/api/react/cognito/callback",
-                                    element: (0, Kr.jsx)(Uh, {})
+                                    element: (0, Kr.jsx)(Rh, {})
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/",
                                     element: (0, Kr.jsx)(xe, {
                                         to: t()
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api",
@@ -74420,131 +74448,131 @@
                                     path: "/api/react/:environ/accounts",
                                     element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
                                         children: (0, Kr.jsx)(ua, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/env",
                                     element: (0, Kr.jsx)(Ui.KnownEnvRequired, {
-                                        children: (0, Kr.jsx)(us, {})
+                                        children: (0, Kr.jsx)(cs, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/env",
                                     element: (0, Kr.jsx)(Ui.KnownEnvRequired, {
-                                        children: (0, Kr.jsx)(us, {})
+                                        children: (0, Kr.jsx)(cs, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/login",
                                     element: (0, Kr.jsx)(Ui.KnownEnvRequired, {
-                                        children: (0, Kr.jsx)(Rh, {})
+                                        children: (0, Kr.jsx)(Fh, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/checks",
                                     element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(Xa, {})
+                                        children: (0, Kr.jsx)(es, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/checks/:check/history",
                                     element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(as, {})
+                                        children: (0, Kr.jsx)(us, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/home",
                                     element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(js, {})
+                                        children: (0, Kr.jsx)(xs, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/info",
                                     element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(Ns, {})
+                                        children: (0, Kr.jsx)(Ds, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/users",
                                     element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(Tg, {})
+                                        children: (0, Kr.jsx)(Og, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/users/:email",
                                     element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(Sg, {})
+                                        children: (0, Kr.jsx)(kg, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/users/edit/:uuid",
                                     element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(Eg, {})
+                                        children: (0, Kr.jsx)(Tg, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/users/create",
                                     element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(Cg, {})
+                                        children: (0, Kr.jsx)(_g, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/gac/:environCompare",
                                     element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(Bh, {})
+                                        children: (0, Kr.jsx)(Yh, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/aws/s3",
                                     element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
                                         children: (0, Kr.jsx)(ga, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/aws/infrastructure",
                                     element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(hg, {})
+                                        children: (0, Kr.jsx)(yg, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/certificates",
                                     element: (0, Kr.jsx)(Ui.KnownEnvRequired, {
-                                        children: (0, Kr.jsx)(vg, {})
+                                        children: (0, Kr.jsx)(bg, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/portal_access_key",
                                     element: (0, Kr.jsx)(Ui.KnownEnvRequired, {
-                                        children: (0, Kr.jsx)(Mg, {})
+                                        children: (0, Kr.jsx)(jg, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/apicache",
                                     element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
                                         children: (0, Kr.jsx)(pa, {})
                                     })
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/forbidden",
-                                    element: (0, Kr.jsx)(cs, {})
+                                    element: (0, Kr.jsx)(fs, {})
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/:environ/error",
                                     element: (0, Kr.jsx)(_i, {})
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/api/react/error",
                                     element: (0, Kr.jsx)(_i, {})
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "/redirect",
-                                    element: (0, Kr.jsx)(yg, {})
+                                    element: (0, Kr.jsx)(vg, {})
                                 }), (0, Kr.jsx)(Ne, {
                                     path: "*",
                                     element: (0, Kr.jsx)(Ui.AuthorizationRequired, {
-                                        children: (0, Kr.jsx)(gg, {})
+                                        children: (0, Kr.jsx)(mg, {})
                                     })
                                 })]
                             })
-                        }), (0, Kr.jsx)(ls, {})]
+                        }), (0, Kr.jsx)(ds, {})]
                     })
                 })
             },
-            Og = r.createRoot(document.getElementById("root"));
-        "1" === bt.Get("test_mode_strict_mode") ? Og.render((0, Kr.jsx)(t.StrictMode, {
-            children: (0, Kr.jsx)(Ag, {})
-        })) : Og.render((0, Kr.jsx)("table", {
+            Ug = r.createRoot(document.getElementById("root"));
+        "1" === bt.Get("test_mode_strict_mode") ? Ug.render((0, Kr.jsx)(t.StrictMode, {
+            children: (0, Kr.jsx)(zg, {})
+        })) : Ug.render((0, Kr.jsx)("table", {
             style: {
                 width: "100%"
             },
             cellPadding: "0",
             cellSpacing: "0",
             children: (0, Kr.jsx)("tbody", {
                 children: (0, Kr.jsx)("tr", {
                     children: (0, Kr.jsx)("td", {
-                        children: (0, Kr.jsx)(Ag, {})
+                        children: (0, Kr.jsx)(zg, {})
                     })
                 })
             })
         }))
     }()
 })();
```

### Comparing `foursight_core-4.1.2/foursight_core/route_prefixes.py` & `foursight_core-4.2.0.1b2/foursight_core/route_prefixes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/routes.py` & `foursight_core-4.2.0.1b2/foursight_core/routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/run_result.py` & `foursight_core-4.2.0.1b2/foursight_core/run_result.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/s3_connection.py` & `foursight_core-4.2.0.1b2/foursight_core/s3_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/schedule_decorator.py` & `foursight_core-4.2.0.1b2/foursight_core/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/scripts/decrypt_accounts_file.py` & `foursight_core-4.2.0.1b2/foursight_core/scripts/decrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/scripts/encrypt_accounts_file.py` & `foursight_core-4.2.0.1b2/foursight_core/scripts/encrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/sqs_utils.py` & `foursight_core-4.2.0.1b2/foursight_core/sqs_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/stage.py` & `foursight_core-4.2.0.1b2/foursight_core/stage.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/templates/base.html` & `foursight_core-4.2.0.1b2/foursight_core/templates/base.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/templates/header.html` & `foursight_core-4.2.0.1b2/foursight_core/templates/header.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/templates/history.html` & `foursight_core-4.2.0.1b2/foursight_core/templates/history.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/templates/info.html` & `foursight_core-4.2.0.1b2/foursight_core/templates/info.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/templates/unused.html` & `foursight_core-4.2.0.1b2/foursight_core/templates/unused.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/templates/user.html` & `foursight_core-4.2.0.1b2/foursight_core/templates/user.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/templates/users.html` & `foursight_core-4.2.0.1b2/foursight_core/templates/users.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/templates/view_checks.html` & `foursight_core-4.2.0.1b2/foursight_core/templates/view_checks.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/foursight_core/templates/view_groups.html` & `foursight_core-4.2.0.1b2/foursight_core/templates/view_groups.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.2/pyproject.toml` & `foursight_core-4.2.0.1b2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "foursight-core"
-version = "4.1.2"
+version = "4.2.0.1b2"  # to become 4.2.0
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "foursight_core" },
   { include = "checks", from = "foursight_core" },
   { include = "helpers", from = "foursight_core/checks" }
```

### Comparing `foursight_core-4.1.2/PKG-INFO` & `foursight_core-4.2.0.1b2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight-core
-Version: 4.1.2
+Version: 4.2.0.1b2
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

