# Comparing `tmp/lamindb_setup-0.46a2.tar.gz` & `tmp/lamindb_setup-0.46a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamindb_setup-0.46a2.tar", last modified: Thu Jun  1 11:35:10 2023, max compression
+gzip compressed data, was "lamindb_setup-0.46a3.tar", last modified: Fri Jun  2 16:03:58 2023, max compression
```

## Comparing `lamindb_setup-0.46a2.tar` & `lamindb_setup-0.46a3.tar`

### file list

```diff
@@ -1,166 +1,171 @@
--rw-r--r--   0        0        0     3304 2023-06-01 11:33:10.497771 lamindb_setup-0.46a2/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-05-26 12:29:21.559431 lamindb_setup-0.46a2/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-05-26 12:29:21.559519 lamindb_setup-0.46a2/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-05-26 12:29:21.559614 lamindb_setup-0.46a2/.gitignore
--rw-r--r--   0        0        0      100 2023-05-31 13:45:54.309833 lamindb_setup-0.46a2/.gitmodules
--rw-r--r--   0        0        0     1793 2023-06-01 11:33:10.497933 lamindb_setup-0.46a2/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-05-26 12:29:21.559824 lamindb_setup-0.46a2/LICENSE
--rw-r--r--   0        0        0      182 2023-06-01 11:33:49.258270 lamindb_setup-0.46a2/README.md
--rw-r--r--   0        0        0       52 2023-05-26 12:29:21.559991 lamindb_setup-0.46a2/docs/api.md
--rw-r--r--   0        0        0    50186 2023-06-01 11:34:50.925480 lamindb_setup-0.46a2/docs/changelog.md
--rw-r--r--   0        0        0     5356 2023-06-01 11:33:10.498487 lamindb_setup-0.46a2/docs/faq/check-synchronization.ipynb
--rw-r--r--   0        0        0     3553 2023-06-01 11:33:10.498687 lamindb_setup-0.46a2/docs/faq/clone.ipynb
--rw-r--r--   0        0        0     6339 2023-06-01 11:33:10.498876 lamindb_setup-0.46a2/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0      166 2023-05-26 12:29:21.560682 lamindb_setup-0.46a2/docs/faq/index.md
--rw-r--r--   0        0        0     1244 2023-06-01 11:33:10.499064 lamindb_setup-0.46a2/docs/faq/manage-migrations.ipynb
--rw-r--r--   0        0        0     3323 2023-06-01 11:33:10.499233 lamindb_setup-0.46a2/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     2880 2023-06-01 11:33:10.499418 lamindb_setup-0.46a2/docs/faq/test-migrations-e2e.ipynb
--rw-r--r--   0        0        0     2144 2023-06-01 11:33:10.499589 lamindb_setup-0.46a2/docs/faq/test-migrations-unit.ipynb
--rw-r--r--   0        0        0     8821 2023-06-01 11:33:10.499805 lamindb_setup-0.46a2/docs/guide/00-index.ipynb
--rw-r--r--   0        0        0     5037 2023-06-01 11:33:10.499992 lamindb_setup-0.46a2/docs/guide/01-setup-user.ipynb
--rw-r--r--   0        0        0     8081 2023-06-01 11:33:10.500188 lamindb_setup-0.46a2/docs/guide/02-init-instance.ipynb
--rw-r--r--   0        0        0     4342 2023-06-01 11:33:10.500381 lamindb_setup-0.46a2/docs/guide/03-load-instance.ipynb
--rw-r--r--   0        0        0     6104 2023-06-01 11:33:10.500592 lamindb_setup-0.46a2/docs/guide/04-set-storage.ipynb
--rw-r--r--   0        0        0     3329 2023-06-01 11:33:10.500807 lamindb_setup-0.46a2/docs/guide/05-schema-modules.ipynb
--rw-r--r--   0        0        0     3331 2023-05-26 12:29:21.561700 lamindb_setup-0.46a2/docs/guide/migrate.md
--rw-r--r--   0        0        0      126 2023-05-26 12:29:21.561778 lamindb_setup-0.46a2/docs/index.md
--rw-r--r--   0        0        0      365 2023-05-31 19:23:44.384942 lamindb_setup-0.46a2/docs/test_notebooks.py
--rw-r--r--   0        0        0      118 2023-05-26 12:29:21.561849 lamindb_setup-0.46a2/lamin-project.yaml
--rw-r--r--   0        0        0     2799 2023-06-01 11:34:40.733326 lamindb_setup-0.46a2/lamindb_setup/__init__.py
--rw-r--r--   0        0        0     5268 2023-06-01 11:33:10.501041 lamindb_setup-0.46a2/lamindb_setup/__main__.py
--rw-r--r--   0        0        0      100 2023-06-01 11:33:10.501383 lamindb_setup-0.46a2/lamindb_setup/_assets/__init__.py
--rw-r--r--   0        0        0     1606 2023-06-01 11:33:10.501615 lamindb_setup-0.46a2/lamindb_setup/_check_instance_setup.py
--rw-r--r--   0        0        0      221 2023-06-01 11:33:10.501769 lamindb_setup-0.46a2/lamindb_setup/_check_versions.py
--rw-r--r--   0        0        0      567 2023-06-01 11:33:10.501880 lamindb_setup-0.46a2/lamindb_setup/_close.py
--rw-r--r--   0        0        0     2182 2023-06-01 11:33:10.502044 lamindb_setup-0.46a2/lamindb_setup/_delete.py
--rw-r--r--   0        0        0      329 2023-06-01 11:33:10.502137 lamindb_setup-0.46a2/lamindb_setup/_info.py
--rw-r--r--   0        0        0     7302 2023-06-01 11:33:10.502357 lamindb_setup-0.46a2/lamindb_setup/_init_instance.py
--rw-r--r--   0        0        0     7291 2023-06-01 11:33:10.502702 lamindb_setup-0.46a2/lamindb_setup/_load_instance.py
--rw-r--r--   0        0        0      135 2023-06-01 11:33:10.502811 lamindb_setup-0.46a2/lamindb_setup/_migrate/__init__.py
--rw-r--r--   0        0        0      723 2023-06-01 11:33:10.503004 lamindb_setup-0.46a2/lamindb_setup/_migrate/alembic.ini
--rw-r--r--   0        0        0     3731 2023-06-01 11:33:10.503365 lamindb_setup-0.46a2/lamindb_setup/_migrate/core.py
--rw-r--r--   0        0        0     7656 2023-06-01 11:33:10.503596 lamindb_setup-0.46a2/lamindb_setup/_migrate/deploy.py
--rw-r--r--   0        0        0     3179 2023-06-01 11:33:10.503705 lamindb_setup-0.46a2/lamindb_setup/_migrate/env.py
--rw-r--r--   0        0        0      334 2023-06-01 11:33:10.503790 lamindb_setup-0.46a2/lamindb_setup/_migrate/script.py.mako
--rw-r--r--   0        0        0     4849 2023-06-01 11:33:10.503950 lamindb_setup-0.46a2/lamindb_setup/_migrate/utils.py
--rw-r--r--   0        0        0      790 2023-06-01 11:33:10.504025 lamindb_setup-0.46a2/lamindb_setup/_notebook.py
--rw-r--r--   0        0        0      803 2023-06-01 11:33:10.504108 lamindb_setup-0.46a2/lamindb_setup/_register_instance.py
--rw-r--r--   0        0        0     1020 2023-06-01 11:33:10.504188 lamindb_setup-0.46a2/lamindb_setup/_schema.py
--rw-r--r--   0        0        0     1848 2023-06-01 11:33:10.504348 lamindb_setup-0.46a2/lamindb_setup/_set.py
--rw-r--r--   0        0        0     2247 2023-06-01 11:33:10.504569 lamindb_setup-0.46a2/lamindb_setup/_settings.py
--rw-r--r--   0        0        0       87 2023-06-01 11:33:10.504660 lamindb_setup-0.46a2/lamindb_setup/_settings_load.py
--rw-r--r--   0        0        0       72 2023-06-01 11:33:10.504736 lamindb_setup-0.46a2/lamindb_setup/_settings_store.py
--rw-r--r--   0        0        0     3488 2023-06-01 11:33:10.504859 lamindb_setup-0.46a2/lamindb_setup/_setup_user.py
--rw-r--r--   0        0        0      456 2023-06-01 11:33:10.505005 lamindb_setup-0.46a2/lamindb_setup/dev/__init__.py
--rw-r--r--   0        0        0     3886 2023-06-01 11:33:10.505126 lamindb_setup-0.46a2/lamindb_setup/dev/_clone.py
--rw-r--r--   0        0        0     7299 2023-06-01 11:33:10.505212 lamindb_setup-0.46a2/lamindb_setup/dev/_db.py
--rw-r--r--   0        0        0     2491 2023-06-01 11:33:10.505290 lamindb_setup-0.46a2/lamindb_setup/dev/_deprecated.py
--rw-r--r--   0        0        0     1693 2023-06-01 11:33:10.505393 lamindb_setup-0.46a2/lamindb_setup/dev/_django.py
--rw-r--r--   0        0        0      240 2023-06-01 11:33:10.505462 lamindb_setup-0.46a2/lamindb_setup/dev/_docs.py
--rw-r--r--   0        0        0     5317 2023-06-01 11:33:10.505542 lamindb_setup-0.46a2/lamindb_setup/dev/_exclusion.py
--rw-r--r--   0        0        0     9126 2023-06-01 11:33:10.505691 lamindb_setup-0.46a2/lamindb_setup/dev/_settings_instance.py
--rw-r--r--   0        0        0     2597 2023-06-01 11:33:10.505847 lamindb_setup-0.46a2/lamindb_setup/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-06-01 11:33:10.505931 lamindb_setup-0.46a2/lamindb_setup/dev/_settings_save.py
--rw-r--r--   0        0        0     2314 2023-06-01 11:33:10.506008 lamindb_setup-0.46a2/lamindb_setup/dev/_settings_store.py
--rw-r--r--   0        0        0     1088 2023-06-01 11:33:10.506112 lamindb_setup-0.46a2/lamindb_setup/dev/_settings_user.py
--rw-r--r--   0        0        0     2728 2023-06-01 11:33:10.506321 lamindb_setup-0.46a2/lamindb_setup/dev/_setup_knowledge.py
--rw-r--r--   0        0        0     4371 2023-06-01 11:33:10.506456 lamindb_setup-0.46a2/lamindb_setup/dev/_setup_schema.py
--rw-r--r--   0        0        0     5536 2023-06-01 11:33:10.506569 lamindb_setup-0.46a2/lamindb_setup/dev/_storage.py
--rw-r--r--   0        0        0     2536 2023-06-01 11:33:10.506639 lamindb_setup-0.46a2/lamindb_setup/dev/upath.py
--rw-r--r--   0        0        0      356 2023-06-01 11:33:10.506745 lamindb_setup-0.46a2/lamindb_setup/test/__init__.py
--rw-r--r--   0        0        0       50 2023-06-01 11:33:10.506814 lamindb_setup-0.46a2/lamindb_setup/test/_env.py
--rw-r--r--   0        0        0     3949 2023-06-01 11:33:10.507074 lamindb_setup-0.46a2/lamindb_setup/test/_migrations_e2e.py
--rw-r--r--   0        0        0     6673 2023-06-01 11:33:10.507279 lamindb_setup-0.46a2/lamindb_setup/test/_migrations_unit.py
--rw-r--r--   0        0        0      254 2023-06-01 11:33:10.507525 lamindb_setup-0.46a2/lamindb_setup/test/_nox.py
--rw-r--r--   0        0        0      188 2023-06-01 11:33:10.507620 lamindb_setup-0.46a2/lamindb_setup/test/nox.py
--rw-r--r--   0        0        0     2802 2023-05-31 19:24:00.352440 lamindb_setup-0.46a2/lnschema-core/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-05-30 14:21:30.384240 lamindb_setup-0.46a2/lnschema-core/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-05-30 14:21:30.384364 lamindb_setup-0.46a2/lnschema-core/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1381 2023-05-30 14:21:30.384442 lamindb_setup-0.46a2/lnschema-core/.gitignore
--rw-r--r--   0        0        0       82 2023-06-01 10:22:45.426042 lamindb_setup-0.46a2/lnschema-core/.gitmodules
--rw-r--r--   0        0        0     1836 2023-05-30 14:21:30.384687 lamindb_setup-0.46a2/lnschema-core/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-05-30 14:21:30.384784 lamindb_setup-0.46a2/lnschema-core/LICENSE
--rw-r--r--   0        0        0      364 2023-05-30 14:21:30.384850 lamindb_setup-0.46a2/lnschema-core/README.md
--rw-r--r--   0        0        0        0 2023-05-30 14:21:30.384908 lamindb_setup-0.46a2/lnschema-core/django_project/__init__.py
--rw-r--r--   0        0        0      404 2023-05-30 14:21:30.384975 lamindb_setup-0.46a2/lnschema-core/django_project/asgi.py
--rw-r--r--   0        0        0     3572 2023-05-30 14:21:30.385044 lamindb_setup-0.46a2/lnschema-core/django_project/settings.py
--rw-r--r--   0        0        0      770 2023-05-30 14:21:30.385110 lamindb_setup-0.46a2/lnschema-core/django_project/urls.py
--rw-r--r--   0        0        0      404 2023-05-30 14:21:30.385276 lamindb_setup-0.46a2/lnschema-core/django_project/wsgi.py
--rw-r--r--   0        0        0    24348 2023-05-31 19:31:21.507267 lamindb_setup-0.46a2/lnschema-core/docs/changelog.md
--rw-r--r--   0        0        0     1485 2023-05-31 12:00:39.299258 lamindb_setup-0.46a2/lnschema-core/docs/guide/0-core-schema.ipynb
--rw-r--r--   0        0        0     8386 2023-05-31 12:00:39.320747 lamindb_setup-0.46a2/lnschema-core/docs/guide/1-data-validation.ipynb
--rw-r--r--   0        0        0       68 2023-05-30 14:21:30.385923 lamindb_setup-0.46a2/lnschema-core/docs/guide/index.md
--rw-r--r--   0        0        0      112 2023-05-30 14:21:30.386018 lamindb_setup-0.46a2/lnschema-core/docs/index.md
--rw-r--r--   0        0        0      202 2023-05-30 14:21:30.386086 lamindb_setup-0.46a2/lnschema-core/lamin-project.yaml
-drwxr-xr-x   0        0        0        0 2023-06-01 10:22:39.772570 lamindb_setup-0.46a2/lnschema-core/lamindb-setup/
--rw-r--r--   0        0        0      913 2023-06-01 10:21:24.511583 lamindb_setup-0.46a2/lnschema-core/lnschema_core/__init__.py
--rw-r--r--   0        0        0    24693 2023-06-01 10:21:24.525208 lamindb_setup-0.46a2/lnschema-core/lnschema_core/_core.py
--rw-r--r--   0        0        0     1514 2023-05-30 14:21:30.386812 lamindb_setup-0.46a2/lnschema-core/lnschema_core/_link.py
--rw-r--r--   0        0        0      228 2023-05-30 14:21:30.386885 lamindb_setup-0.46a2/lnschema-core/lnschema_core/_timestamps.py
--rw-r--r--   0        0        0      932 2023-06-01 10:20:04.411718 lamindb_setup-0.46a2/lnschema-core/lnschema_core/_types.py
--rw-r--r--   0        0        0      349 2023-06-01 10:20:04.411658 lamindb_setup-0.46a2/lnschema-core/lnschema_core/_users.py
--rw-r--r--   0        0        0      100 2023-05-30 14:21:30.387077 lamindb_setup-0.46a2/lnschema-core/lnschema_core/apps.py
--rw-r--r--   0        0        0      313 2023-05-30 14:21:30.387173 lamindb_setup-0.46a2/lnschema-core/lnschema_core/dev/__init__.py
--rw-r--r--   0        0        0     2477 2023-05-30 14:21:30.387427 lamindb_setup-0.46a2/lnschema-core/lnschema_core/dev/_id.py
--rw-r--r--   0        0        0     1075 2023-05-30 14:21:30.387523 lamindb_setup-0.46a2/lnschema-core/lnschema_core/dev/_versions.py
--rw-r--r--   0        0        0      579 2023-05-30 14:21:30.387597 lamindb_setup-0.46a2/lnschema-core/lnschema_core/dev/id.py
--rw-r--r--   0        0        0    14717 2023-06-01 10:20:04.431436 lamindb_setup-0.46a2/lnschema-core/lnschema_core/dev/sqlmodel.py
--rw-r--r--   0        0        0      227 2023-05-30 14:21:30.387777 lamindb_setup-0.46a2/lnschema-core/lnschema_core/link.py
--rwxr-xr-x   0        0        0      640 2023-05-30 14:21:30.387839 lamindb_setup-0.46a2/lnschema-core/lnschema_core/manage.py
--rw-r--r--   0        0        0     9699 2023-05-31 19:24:00.354344 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-05-30 14:21:30.387900 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/__init__.py
--rw-r--r--   0        0        0     3694 2023-05-30 14:21:30.388217 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-07-21-0560ee3d73dc-jupynb.py
--rw-r--r--   0        0        0     6580 2023-05-30 14:21:30.388467 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-08-08-8c78543d1c5b-v0_3_0.py
--rw-r--r--   0        0        0     2073 2023-05-30 14:21:30.388554 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-08-19-1c531ea346cf-storage.py
--rw-r--r--   0        0        0     4358 2023-05-30 14:21:30.388622 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-08-22-01fcb82dafd4-v0_4_0.py
--rw-r--r--   0        0        0     3333 2023-05-30 14:21:30.388701 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-08-26-3badf20f18c8-v0_5_0.py
--rw-r--r--   0        0        0      817 2023-05-30 14:21:30.388767 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-08-29-d1b3e5da6391-v0_5_1.py
--rw-r--r--   0        0        0      536 2023-05-30 14:21:30.388831 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-09-15-5fa54c55c3bf-v0_6_0.py
--rw-r--r--   0        0        0      976 2023-05-30 14:21:30.388893 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-09-18-049d7dfc80a8-v0_7_1.py
--rw-r--r--   0        0        0     6332 2023-05-30 14:21:30.388963 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-09-18-3b60b87450c0-v0_7_0.py
--rw-r--r--   0        0        0     2886 2023-05-30 14:21:30.389027 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-09-24-1f29517759b7-v0_7_3.py
--rw-r--r--   0        0        0      762 2023-05-30 14:21:30.389088 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-09-25-7e8f7b30792e-v0_8_0.py
--rw-r--r--   0        0        0      668 2023-05-30 14:21:30.389149 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-09-26-1190648443cb-v0_8_1.py
--rw-r--r--   0        0        0     1082 2023-05-30 14:21:30.389209 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-09-30-439c4ee0a22a-v0_9_0.py
--rw-r--r--   0        0        0     1725 2023-05-30 14:21:30.389276 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-10-07-0c819d33ca9b-v0_10_0.py
--rw-r--r--   0        0        0      613 2023-05-30 14:21:30.389356 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-10-10-3d244a8d3148-v0_11_0.py
--rw-r--r--   0        0        0      646 2023-05-30 14:21:30.389424 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-10-11-2ddcb037e3ea-v0_12_0.py
--rw-r--r--   0        0        0     3507 2023-05-30 14:21:30.389485 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-10-19-cf5913791674-v0_14_0.py
--rw-r--r--   0        0        0     2344 2023-05-30 14:21:30.389548 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-10-31-98da12fc80a8-v0_15_0.py
--rw-r--r--   0        0        0     8560 2023-05-30 14:21:30.389626 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-11-10-4ee426b656bb-v0_16_0.py
--rw-r--r--   0        0        0     4792 2023-05-30 14:21:30.389844 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-11-11-66bfd6cf2e2d-v0_17_0.py
--rw-r--r--   0        0        0     4603 2023-05-30 14:21:30.389927 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-11-28-4b4005b7841c-v0_21_1.py
--rw-r--r--   0        0        0     1209 2023-05-30 14:21:30.390122 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-12-07-9d94f3b9566d-v0_21_3.py
--rw-r--r--   0        0        0     2202 2023-05-30 14:21:30.390229 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-12-07-db1df7b2aaad-v0_22_0.py
--rw-r--r--   0        0        0     1098 2023-05-30 14:21:30.390300 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-01-09-f6b6b85cdffc-v0_24_0.py
--rw-r--r--   0        0        0     1229 2023-05-30 14:21:30.390371 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-02-02-9d283a1685a5-v0_25_6.py
--rw-r--r--   0        0        0     3580 2023-05-30 14:21:30.390448 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-02-07-8bf788467d0a-v0_25_9.py
--rw-r--r--   0        0        0      593 2023-05-30 14:21:30.390525 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-02-10-ff3b5b3ec913-v0_26_1.py
--rw-r--r--   0        0        0      973 2023-05-30 14:21:30.390584 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-02-14-8280855a5064-v0_26_2.py
--rw-r--r--   0        0        0     1120 2023-05-30 14:21:30.390641 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-02-21-1dafcf0b22aa-v0_28_0.py
--rw-r--r--   0        0        0     1067 2023-05-30 14:21:30.390699 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-02-22-6952574e2d49-v0_28_1.py
--rw-r--r--   0        0        0     1712 2023-05-30 14:21:30.390788 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-02-23-24e55331f27c-v0_28_2.py
--rw-r--r--   0        0        0      483 2023-05-30 14:21:30.390866 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-02-23-3dd9f8d41861-v0_28_3.py
--rw-r--r--   0        0        0      581 2023-05-30 14:21:30.390932 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-02-24-873683a29806-v0_28_7.py
--rw-r--r--   0        0        0      778 2023-05-30 14:21:30.390997 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-03-21-9640062eefee-v0_30rc1.py
--rw-r--r--   0        0        0     5367 2023-05-30 14:21:30.391066 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-03-23-ebafd37fd6e1-v0_30rc2.py
--rw-r--r--   0        0        0     6957 2023-05-30 14:21:30.391136 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-03-24-5846a15d9241-0_30rc3.py
--rw-r--r--   0        0        0     1658 2023-05-30 14:21:30.391214 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-04-05-6de59093e378-v0_32_0.py
--rw-r--r--   0        0        0      780 2023-05-30 14:21:30.391283 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-04-13-d161a14a12e3-v0_32_1.py
--rw-r--r--   0        0        0     4440 2023-05-30 14:21:30.391353 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-04-16-6a73c00555b4-v0_33_0.py
--rw-r--r--   0        0        0     3782 2023-05-30 14:21:30.391419 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-05-24-c3f38ffe9e03-v0_34a1.py
--rw-r--r--   0        0        0     8841 2023-05-30 14:21:30.391507 lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-05-28-1c49c9f9a982-v0_34a2.py
--rw-r--r--   0        0        0    16456 2023-06-01 10:21:24.519640 lamindb_setup-0.46a2/lnschema-core/lnschema_core/models.py
--rw-r--r--   0        0        0      205 2023-05-30 14:21:30.391658 lamindb_setup-0.46a2/lnschema-core/lnschema_core/types.py
--rwxr-xr-x   0        0        0      640 2023-05-30 14:21:30.391734 lamindb_setup-0.46a2/lnschema-core/manage.py
--rw-r--r--   0        0        0     1020 2023-06-01 10:49:38.723231 lamindb_setup-0.46a2/lnschema-core/noxfile.py
--rw-r--r--   0        0        0      966 2023-06-01 10:45:58.473413 lamindb_setup-0.46a2/lnschema-core/pyproject.toml
--rw-r--r--   0        0        0     1212 2023-06-01 10:20:18.519334 lamindb_setup-0.46a2/lnschema-core/tests/test_migrations.py
--rw-r--r--   0        0        0      475 2023-05-30 14:21:30.392155 lamindb_setup-0.46a2/lnschema-core/tests/test_notebooks.py
--rw-r--r--   0        0        0     2112 2023-06-01 11:33:10.507865 lamindb_setup-0.46a2/noxfile.py
--rw-r--r--   0        0        0     1399 2023-06-01 11:33:10.508034 lamindb_setup-0.46a2/pyproject.toml
--rw-r--r--   0        0        0      658 2023-06-01 11:33:10.508216 lamindb_setup-0.46a2/tests/test_bionty.py
--rw-r--r--   0        0        0     3041 2023-06-01 11:33:10.508406 lamindb_setup-0.46a2/tests/test_init_instance.py
--rw-r--r--   0        0        0      655 2023-06-01 11:33:10.508620 lamindb_setup-0.46a2/tests/test_load_instance.py
--rw-r--r--   0        0        0      243 2023-06-01 11:33:10.508784 lamindb_setup-0.46a2/tests/test_set_storage.py
--rw-r--r--   0        0        0     1215 1970-01-01 00:00:00.000000 lamindb_setup-0.46a2/PKG-INFO
+-rw-r--r--   0        0        0     3304 2023-06-01 11:33:10.497771 lamindb_setup-0.46a3/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-05-26 12:29:21.559431 lamindb_setup-0.46a3/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-05-26 12:29:21.559519 lamindb_setup-0.46a3/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-05-26 12:29:21.559614 lamindb_setup-0.46a3/.gitignore
+-rw-r--r--   0        0        0      100 2023-05-31 13:45:54.309833 lamindb_setup-0.46a3/.gitmodules
+-rw-r--r--   0        0        0     1793 2023-06-01 11:33:10.497933 lamindb_setup-0.46a3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-05-26 12:29:21.559824 lamindb_setup-0.46a3/LICENSE
+-rw-r--r--   0        0        0      182 2023-06-01 11:33:49.258270 lamindb_setup-0.46a3/README.md
+-rw-r--r--   0        0        0       52 2023-05-26 12:29:21.559991 lamindb_setup-0.46a3/docs/api.md
+-rw-r--r--   0        0        0    50353 2023-06-02 16:03:38.945364 lamindb_setup-0.46a3/docs/changelog.md
+-rw-r--r--   0        0        0     5356 2023-06-01 11:33:10.498487 lamindb_setup-0.46a3/docs/faq/check-synchronization.ipynb
+-rw-r--r--   0        0        0     3553 2023-06-01 11:33:10.498687 lamindb_setup-0.46a3/docs/faq/clone.ipynb
+-rw-r--r--   0        0        0     6339 2023-06-01 11:33:10.498876 lamindb_setup-0.46a3/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0      166 2023-05-26 12:29:21.560682 lamindb_setup-0.46a3/docs/faq/index.md
+-rw-r--r--   0        0        0     1244 2023-06-01 11:33:10.499064 lamindb_setup-0.46a3/docs/faq/manage-migrations.ipynb
+-rw-r--r--   0        0        0     3323 2023-06-01 11:33:10.499233 lamindb_setup-0.46a3/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     2880 2023-06-01 11:33:10.499418 lamindb_setup-0.46a3/docs/faq/test-migrations-e2e.ipynb
+-rw-r--r--   0        0        0     2144 2023-06-01 11:33:10.499589 lamindb_setup-0.46a3/docs/faq/test-migrations-unit.ipynb
+-rw-r--r--   0        0        0     8821 2023-06-01 11:33:10.499805 lamindb_setup-0.46a3/docs/guide/00-index.ipynb
+-rw-r--r--   0        0        0     5037 2023-06-01 11:33:10.499992 lamindb_setup-0.46a3/docs/guide/01-setup-user.ipynb
+-rw-r--r--   0        0        0     8081 2023-06-01 11:33:10.500188 lamindb_setup-0.46a3/docs/guide/02-init-instance.ipynb
+-rw-r--r--   0        0        0     4342 2023-06-01 11:33:10.500381 lamindb_setup-0.46a3/docs/guide/03-load-instance.ipynb
+-rw-r--r--   0        0        0     6104 2023-06-01 11:33:10.500592 lamindb_setup-0.46a3/docs/guide/04-set-storage.ipynb
+-rw-r--r--   0        0        0     3329 2023-06-01 11:33:10.500807 lamindb_setup-0.46a3/docs/guide/05-schema-modules.ipynb
+-rw-r--r--   0        0        0     3331 2023-05-26 12:29:21.561700 lamindb_setup-0.46a3/docs/guide/migrate.md
+-rw-r--r--   0        0        0      126 2023-05-26 12:29:21.561778 lamindb_setup-0.46a3/docs/index.md
+-rw-r--r--   0        0        0      365 2023-05-31 19:23:44.384942 lamindb_setup-0.46a3/docs/test_notebooks.py
+-rw-r--r--   0        0        0      118 2023-05-26 12:29:21.561849 lamindb_setup-0.46a3/lamin-project.yaml
+-rw-r--r--   0        0        0     2794 2023-06-02 16:03:32.990491 lamindb_setup-0.46a3/lamindb_setup/__init__.py
+-rw-r--r--   0        0        0     5268 2023-06-01 11:33:10.501041 lamindb_setup-0.46a3/lamindb_setup/__main__.py
+-rw-r--r--   0        0        0      100 2023-06-01 11:33:10.501383 lamindb_setup-0.46a3/lamindb_setup/_assets/__init__.py
+-rw-r--r--   0        0        0     1813 2023-06-02 16:02:42.978369 lamindb_setup-0.46a3/lamindb_setup/_check_instance_setup.py
+-rw-r--r--   0        0        0      221 2023-06-01 11:33:10.501769 lamindb_setup-0.46a3/lamindb_setup/_check_versions.py
+-rw-r--r--   0        0        0      567 2023-06-01 11:33:10.501880 lamindb_setup-0.46a3/lamindb_setup/_close.py
+-rw-r--r--   0        0        0     2182 2023-06-01 11:33:10.502044 lamindb_setup-0.46a3/lamindb_setup/_delete.py
+-rw-r--r--   0        0        0      329 2023-06-01 11:33:10.502137 lamindb_setup-0.46a3/lamindb_setup/_info.py
+-rw-r--r--   0        0        0     7275 2023-06-02 16:02:42.978682 lamindb_setup-0.46a3/lamindb_setup/_init_instance.py
+-rw-r--r--   0        0        0     7291 2023-06-01 11:33:10.502702 lamindb_setup-0.46a3/lamindb_setup/_load_instance.py
+-rw-r--r--   0        0        0      135 2023-06-01 11:33:10.502811 lamindb_setup-0.46a3/lamindb_setup/_migrate/__init__.py
+-rw-r--r--   0        0        0      723 2023-06-01 11:33:10.503004 lamindb_setup-0.46a3/lamindb_setup/_migrate/alembic.ini
+-rw-r--r--   0        0        0     3731 2023-06-01 11:33:10.503365 lamindb_setup-0.46a3/lamindb_setup/_migrate/core.py
+-rw-r--r--   0        0        0     7656 2023-06-01 11:33:10.503596 lamindb_setup-0.46a3/lamindb_setup/_migrate/deploy.py
+-rw-r--r--   0        0        0     3179 2023-06-01 11:33:10.503705 lamindb_setup-0.46a3/lamindb_setup/_migrate/env.py
+-rw-r--r--   0        0        0      334 2023-06-01 11:33:10.503790 lamindb_setup-0.46a3/lamindb_setup/_migrate/script.py.mako
+-rw-r--r--   0        0        0     4849 2023-06-01 11:33:10.503950 lamindb_setup-0.46a3/lamindb_setup/_migrate/utils.py
+-rw-r--r--   0        0        0      790 2023-06-01 11:33:10.504025 lamindb_setup-0.46a3/lamindb_setup/_notebook.py
+-rw-r--r--   0        0        0      803 2023-06-01 11:33:10.504108 lamindb_setup-0.46a3/lamindb_setup/_register_instance.py
+-rw-r--r--   0        0        0     1020 2023-06-01 11:33:10.504188 lamindb_setup-0.46a3/lamindb_setup/_schema.py
+-rw-r--r--   0        0        0     1848 2023-06-01 11:33:10.504348 lamindb_setup-0.46a3/lamindb_setup/_set.py
+-rw-r--r--   0        0        0     2247 2023-06-01 11:33:10.504569 lamindb_setup-0.46a3/lamindb_setup/_settings.py
+-rw-r--r--   0        0        0       87 2023-06-01 11:33:10.504660 lamindb_setup-0.46a3/lamindb_setup/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-06-01 11:33:10.504736 lamindb_setup-0.46a3/lamindb_setup/_settings_store.py
+-rw-r--r--   0        0        0     3488 2023-06-01 11:33:10.504859 lamindb_setup-0.46a3/lamindb_setup/_setup_user.py
+-rw-r--r--   0        0        0      456 2023-06-01 11:33:10.505005 lamindb_setup-0.46a3/lamindb_setup/dev/__init__.py
+-rw-r--r--   0        0        0     3886 2023-06-01 11:33:10.505126 lamindb_setup-0.46a3/lamindb_setup/dev/_clone.py
+-rw-r--r--   0        0        0     7299 2023-06-01 11:33:10.505212 lamindb_setup-0.46a3/lamindb_setup/dev/_db.py
+-rw-r--r--   0        0        0     2491 2023-06-01 11:33:10.505290 lamindb_setup-0.46a3/lamindb_setup/dev/_deprecated.py
+-rw-r--r--   0        0        0     1693 2023-06-01 11:33:10.505393 lamindb_setup-0.46a3/lamindb_setup/dev/_django.py
+-rw-r--r--   0        0        0      240 2023-06-01 11:33:10.505462 lamindb_setup-0.46a3/lamindb_setup/dev/_docs.py
+-rw-r--r--   0        0        0     5317 2023-06-01 11:33:10.505542 lamindb_setup-0.46a3/lamindb_setup/dev/_exclusion.py
+-rw-r--r--   0        0        0     9422 2023-06-02 16:02:42.978976 lamindb_setup-0.46a3/lamindb_setup/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2597 2023-06-01 11:33:10.505847 lamindb_setup-0.46a3/lamindb_setup/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-06-01 11:33:10.505931 lamindb_setup-0.46a3/lamindb_setup/dev/_settings_save.py
+-rw-r--r--   0        0        0     2314 2023-06-01 11:33:10.506008 lamindb_setup-0.46a3/lamindb_setup/dev/_settings_store.py
+-rw-r--r--   0        0        0     1088 2023-06-01 11:33:10.506112 lamindb_setup-0.46a3/lamindb_setup/dev/_settings_user.py
+-rw-r--r--   0        0        0     2728 2023-06-01 11:33:10.506321 lamindb_setup-0.46a3/lamindb_setup/dev/_setup_knowledge.py
+-rw-r--r--   0        0        0     4115 2023-06-02 16:02:42.979223 lamindb_setup-0.46a3/lamindb_setup/dev/_setup_schema.py
+-rw-r--r--   0        0        0     5536 2023-06-01 11:33:10.506569 lamindb_setup-0.46a3/lamindb_setup/dev/_storage.py
+-rw-r--r--   0        0        0     2536 2023-06-01 11:33:10.506639 lamindb_setup-0.46a3/lamindb_setup/dev/upath.py
+-rw-r--r--   0        0        0      356 2023-06-01 11:33:10.506745 lamindb_setup-0.46a3/lamindb_setup/test/__init__.py
+-rw-r--r--   0        0        0       50 2023-06-01 11:33:10.506814 lamindb_setup-0.46a3/lamindb_setup/test/_env.py
+-rw-r--r--   0        0        0     3949 2023-06-01 11:33:10.507074 lamindb_setup-0.46a3/lamindb_setup/test/_migrations_e2e.py
+-rw-r--r--   0        0        0     6673 2023-06-01 11:33:10.507279 lamindb_setup-0.46a3/lamindb_setup/test/_migrations_unit.py
+-rw-r--r--   0        0        0      254 2023-06-01 11:33:10.507525 lamindb_setup-0.46a3/lamindb_setup/test/_nox.py
+-rw-r--r--   0        0        0      188 2023-06-01 11:33:10.507620 lamindb_setup-0.46a3/lamindb_setup/test/nox.py
+-rw-r--r--   0        0        0     2811 2023-06-02 12:28:18.951248 lamindb_setup-0.46a3/lnschema-core/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-05-30 14:21:30.384240 lamindb_setup-0.46a3/lnschema-core/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-05-30 14:21:30.384364 lamindb_setup-0.46a3/lnschema-core/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1381 2023-05-30 14:21:30.384442 lamindb_setup-0.46a3/lnschema-core/.gitignore
+-rw-r--r--   0        0        0        0 2023-06-02 12:28:18.951387 lamindb_setup-0.46a3/lnschema-core/.gitmodules
+-rw-r--r--   0        0        0     1836 2023-05-30 14:21:30.384687 lamindb_setup-0.46a3/lnschema-core/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-05-30 14:21:30.384784 lamindb_setup-0.46a3/lnschema-core/LICENSE
+-rw-r--r--   0        0        0      364 2023-05-30 14:21:30.384850 lamindb_setup-0.46a3/lnschema-core/README.md
+-rw-r--r--   0        0        0        0 2023-05-30 14:21:30.384908 lamindb_setup-0.46a3/lnschema-core/django_project/__init__.py
+-rw-r--r--   0        0        0      404 2023-05-30 14:21:30.384975 lamindb_setup-0.46a3/lnschema-core/django_project/asgi.py
+-rw-r--r--   0        0        0     3572 2023-05-30 14:21:30.385044 lamindb_setup-0.46a3/lnschema-core/django_project/settings.py
+-rw-r--r--   0        0        0      770 2023-05-30 14:21:30.385110 lamindb_setup-0.46a3/lnschema-core/django_project/urls.py
+-rw-r--r--   0        0        0      404 2023-05-30 14:21:30.385276 lamindb_setup-0.46a3/lnschema-core/django_project/wsgi.py
+-rw-r--r--   0        0        0    24509 2023-06-02 12:28:18.952040 lamindb_setup-0.46a3/lnschema-core/docs/changelog.md
+-rw-r--r--   0        0        0     1485 2023-05-31 12:00:39.299258 lamindb_setup-0.46a3/lnschema-core/docs/guide/0-core-schema.ipynb
+-rw-r--r--   0        0        0     8386 2023-05-31 12:00:39.320747 lamindb_setup-0.46a3/lnschema-core/docs/guide/1-data-validation.ipynb
+-rw-r--r--   0        0        0       68 2023-05-30 14:21:30.385923 lamindb_setup-0.46a3/lnschema-core/docs/guide/index.md
+-rw-r--r--   0        0        0      112 2023-05-30 14:21:30.386018 lamindb_setup-0.46a3/lnschema-core/docs/index.md
+-rw-r--r--   0        0        0      202 2023-05-30 14:21:30.386086 lamindb_setup-0.46a3/lnschema-core/lamin-project.yaml
+-rw-r--r--   0        0        0     1033 2023-06-02 12:28:39.298653 lamindb_setup-0.46a3/lnschema-core/lnschema_core/__init__.py
+-rw-r--r--   0        0        0    24693 2023-06-02 12:28:18.952953 lamindb_setup-0.46a3/lnschema-core/lnschema_core/_core.py
+-rw-r--r--   0        0        0     1514 2023-05-30 14:21:30.386812 lamindb_setup-0.46a3/lnschema-core/lnschema_core/_link.py
+-rw-r--r--   0        0        0     1652 2023-06-02 15:54:27.350134 lamindb_setup-0.46a3/lnschema-core/lnschema_core/_lookup.py
+-rw-r--r--   0        0        0      228 2023-05-30 14:21:30.386885 lamindb_setup-0.46a3/lnschema-core/lnschema_core/_timestamps.py
+-rw-r--r--   0        0        0      932 2023-06-02 12:28:18.953448 lamindb_setup-0.46a3/lnschema-core/lnschema_core/_types.py
+-rw-r--r--   0        0        0      349 2023-06-02 12:28:18.953894 lamindb_setup-0.46a3/lnschema-core/lnschema_core/_users.py
+-rw-r--r--   0        0        0      100 2023-05-30 14:21:30.387077 lamindb_setup-0.46a3/lnschema-core/lnschema_core/apps.py
+-rw-r--r--   0        0        0      313 2023-05-30 14:21:30.387173 lamindb_setup-0.46a3/lnschema-core/lnschema_core/dev/__init__.py
+-rw-r--r--   0        0        0     2477 2023-05-30 14:21:30.387427 lamindb_setup-0.46a3/lnschema-core/lnschema_core/dev/_id.py
+-rw-r--r--   0        0        0     1075 2023-05-30 14:21:30.387523 lamindb_setup-0.46a3/lnschema-core/lnschema_core/dev/_versions.py
+-rw-r--r--   0        0        0      579 2023-05-30 14:21:30.387597 lamindb_setup-0.46a3/lnschema-core/lnschema_core/dev/id.py
+-rw-r--r--   0        0        0    13429 2023-06-02 15:54:27.350430 lamindb_setup-0.46a3/lnschema-core/lnschema_core/dev/sqlmodel.py
+-rw-r--r--   0        0        0      227 2023-05-30 14:21:30.387777 lamindb_setup-0.46a3/lnschema-core/lnschema_core/link.py
+-rwxr-xr-x   0        0        0      640 2023-05-30 14:21:30.387839 lamindb_setup-0.46a3/lnschema-core/lnschema_core/manage.py
+-rw-r--r--   0        0        0     9699 2023-05-31 19:24:00.354344 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/0001_initial.py
+-rw-r--r--   0        0        0      409 2023-06-02 12:28:39.298909 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/0002_alter_file_id.py
+-rw-r--r--   0        0        0      417 2023-06-02 12:28:39.299082 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/0003_alter_folder_id.py
+-rw-r--r--   0        0        0      661 2023-06-02 12:28:39.299271 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/0004_alter_folder_created_at_alter_folder_updated_at.py
+-rw-r--r--   0        0        0     1368 2023-06-02 12:28:39.299452 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/0005_alter_project_id_alter_run_id_alter_storage_id_and_more.py
+-rw-r--r--   0        0        0     2831 2023-06-02 12:28:39.299634 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/0006_transform_hash_alter_features_created_by_and_more.py
+-rw-r--r--   0        0        0        0 2023-05-30 14:21:30.387900 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/__init__.py
+-rw-r--r--   0        0        0     3694 2023-05-30 14:21:30.388217 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-07-21-0560ee3d73dc-jupynb.py
+-rw-r--r--   0        0        0     6580 2023-05-30 14:21:30.388467 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-08-08-8c78543d1c5b-v0_3_0.py
+-rw-r--r--   0        0        0     2073 2023-05-30 14:21:30.388554 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-08-19-1c531ea346cf-storage.py
+-rw-r--r--   0        0        0     4358 2023-05-30 14:21:30.388622 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-08-22-01fcb82dafd4-v0_4_0.py
+-rw-r--r--   0        0        0     3333 2023-05-30 14:21:30.388701 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-08-26-3badf20f18c8-v0_5_0.py
+-rw-r--r--   0        0        0      817 2023-05-30 14:21:30.388767 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-08-29-d1b3e5da6391-v0_5_1.py
+-rw-r--r--   0        0        0      536 2023-05-30 14:21:30.388831 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-09-15-5fa54c55c3bf-v0_6_0.py
+-rw-r--r--   0        0        0      976 2023-05-30 14:21:30.388893 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-09-18-049d7dfc80a8-v0_7_1.py
+-rw-r--r--   0        0        0     6332 2023-05-30 14:21:30.388963 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-09-18-3b60b87450c0-v0_7_0.py
+-rw-r--r--   0        0        0     2886 2023-05-30 14:21:30.389027 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-09-24-1f29517759b7-v0_7_3.py
+-rw-r--r--   0        0        0      762 2023-05-30 14:21:30.389088 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-09-25-7e8f7b30792e-v0_8_0.py
+-rw-r--r--   0        0        0      668 2023-05-30 14:21:30.389149 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-09-26-1190648443cb-v0_8_1.py
+-rw-r--r--   0        0        0     1082 2023-05-30 14:21:30.389209 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-09-30-439c4ee0a22a-v0_9_0.py
+-rw-r--r--   0        0        0     1725 2023-05-30 14:21:30.389276 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-10-07-0c819d33ca9b-v0_10_0.py
+-rw-r--r--   0        0        0      613 2023-05-30 14:21:30.389356 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-10-10-3d244a8d3148-v0_11_0.py
+-rw-r--r--   0        0        0      646 2023-05-30 14:21:30.389424 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-10-11-2ddcb037e3ea-v0_12_0.py
+-rw-r--r--   0        0        0     3507 2023-05-30 14:21:30.389485 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-10-19-cf5913791674-v0_14_0.py
+-rw-r--r--   0        0        0     2344 2023-05-30 14:21:30.389548 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-10-31-98da12fc80a8-v0_15_0.py
+-rw-r--r--   0        0        0     8560 2023-05-30 14:21:30.389626 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-11-10-4ee426b656bb-v0_16_0.py
+-rw-r--r--   0        0        0     4792 2023-05-30 14:21:30.389844 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-11-11-66bfd6cf2e2d-v0_17_0.py
+-rw-r--r--   0        0        0     4603 2023-05-30 14:21:30.389927 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-11-28-4b4005b7841c-v0_21_1.py
+-rw-r--r--   0        0        0     1209 2023-05-30 14:21:30.390122 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-12-07-9d94f3b9566d-v0_21_3.py
+-rw-r--r--   0        0        0     2202 2023-05-30 14:21:30.390229 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-12-07-db1df7b2aaad-v0_22_0.py
+-rw-r--r--   0        0        0     1098 2023-05-30 14:21:30.390300 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-01-09-f6b6b85cdffc-v0_24_0.py
+-rw-r--r--   0        0        0     1229 2023-05-30 14:21:30.390371 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-02-02-9d283a1685a5-v0_25_6.py
+-rw-r--r--   0        0        0     3580 2023-05-30 14:21:30.390448 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-02-07-8bf788467d0a-v0_25_9.py
+-rw-r--r--   0        0        0      593 2023-05-30 14:21:30.390525 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-02-10-ff3b5b3ec913-v0_26_1.py
+-rw-r--r--   0        0        0      973 2023-05-30 14:21:30.390584 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-02-14-8280855a5064-v0_26_2.py
+-rw-r--r--   0        0        0     1120 2023-05-30 14:21:30.390641 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-02-21-1dafcf0b22aa-v0_28_0.py
+-rw-r--r--   0        0        0     1067 2023-05-30 14:21:30.390699 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-02-22-6952574e2d49-v0_28_1.py
+-rw-r--r--   0        0        0     1712 2023-05-30 14:21:30.390788 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-02-23-24e55331f27c-v0_28_2.py
+-rw-r--r--   0        0        0      483 2023-05-30 14:21:30.390866 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-02-23-3dd9f8d41861-v0_28_3.py
+-rw-r--r--   0        0        0      581 2023-05-30 14:21:30.390932 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-02-24-873683a29806-v0_28_7.py
+-rw-r--r--   0        0        0      778 2023-05-30 14:21:30.390997 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-03-21-9640062eefee-v0_30rc1.py
+-rw-r--r--   0        0        0     5367 2023-05-30 14:21:30.391066 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-03-23-ebafd37fd6e1-v0_30rc2.py
+-rw-r--r--   0        0        0     6957 2023-05-30 14:21:30.391136 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-03-24-5846a15d9241-0_30rc3.py
+-rw-r--r--   0        0        0     1658 2023-05-30 14:21:30.391214 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-04-05-6de59093e378-v0_32_0.py
+-rw-r--r--   0        0        0      780 2023-05-30 14:21:30.391283 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-04-13-d161a14a12e3-v0_32_1.py
+-rw-r--r--   0        0        0     4440 2023-05-30 14:21:30.391353 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-04-16-6a73c00555b4-v0_33_0.py
+-rw-r--r--   0        0        0     3782 2023-05-30 14:21:30.391419 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-05-24-c3f38ffe9e03-v0_34a1.py
+-rw-r--r--   0        0        0     8841 2023-05-30 14:21:30.391507 lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-05-28-1c49c9f9a982-v0_34a2.py
+-rw-r--r--   0        0        0    18194 2023-06-02 15:54:27.350739 lamindb_setup-0.46a3/lnschema-core/lnschema_core/models.py
+-rw-r--r--   0        0        0      205 2023-05-30 14:21:30.391658 lamindb_setup-0.46a3/lnschema-core/lnschema_core/types.py
+-rwxr-xr-x   0        0        0      640 2023-05-30 14:21:30.391734 lamindb_setup-0.46a3/lnschema-core/manage.py
+-rw-r--r--   0        0        0     1281 2023-06-02 12:28:18.955047 lamindb_setup-0.46a3/lnschema-core/noxfile.py
+-rw-r--r--   0        0        0      966 2023-06-02 12:28:18.955511 lamindb_setup-0.46a3/lnschema-core/pyproject.toml
+-rw-r--r--   0        0        0     1212 2023-06-02 12:28:18.955860 lamindb_setup-0.46a3/lnschema-core/tests/test_migrations.py
+-rw-r--r--   0        0        0      475 2023-05-30 14:21:30.392155 lamindb_setup-0.46a3/lnschema-core/tests/test_notebooks.py
+-rw-r--r--   0        0        0     2112 2023-06-01 11:33:10.507865 lamindb_setup-0.46a3/noxfile.py
+-rw-r--r--   0        0        0     1399 2023-06-01 11:33:10.508034 lamindb_setup-0.46a3/pyproject.toml
+-rw-r--r--   0        0        0      658 2023-06-01 11:33:10.508216 lamindb_setup-0.46a3/tests/test_bionty.py
+-rw-r--r--   0        0        0     3041 2023-06-01 11:33:10.508406 lamindb_setup-0.46a3/tests/test_init_instance.py
+-rw-r--r--   0        0        0      655 2023-06-01 11:33:10.508620 lamindb_setup-0.46a3/tests/test_load_instance.py
+-rw-r--r--   0        0        0      243 2023-06-01 11:33:10.508784 lamindb_setup-0.46a3/tests/test_set_storage.py
+-rw-r--r--   0        0        0     1215 1970-01-01 00:00:00.000000 lamindb_setup-0.46a3/PKG-INFO
```

### Comparing `lamindb_setup-0.46a2/.github/workflows/build.yml` & `lamindb_setup-0.46a3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/.github/workflows/latest-changes.yml` & `lamindb_setup-0.46a3/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/.gitignore` & `lamindb_setup-0.46a3/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/.pre-commit-config.yaml` & `lamindb_setup-0.46a3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/LICENSE` & `lamindb_setup-0.46a3/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/docs/changelog.md` & `lamindb_setup-0.46a3/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🏗️ Enable Django backend (lamindb) | [390](https://github.com/laminlabs/lamindb-setup/pull/390) | [falexwolf](https://github.com/falexwolf) | 2023-06-02 | 0.46a3
 🚚 Rename package to `lamindb_setup` | [389](https://github.com/laminlabs/lamindb-setup/pull/389) | [falexwolf](https://github.com/falexwolf) | 2023-06-01 | 0.46a2
 🏗️ Add Django backend | [388](https://github.com/laminlabs/lndb/pull/388) | [falexwolf](https://github.com/falexwolf) | 2023-05-31 | 0.46a1
 ♻️ Refactor CI | [387](https://github.com/laminlabs/lndb/pull/387) | [falexwolf](https://github.com/falexwolf) | 2023-05-30 | 0.45.0
 🐛 Unlock on uncaught exceptions in ipython | [386](https://github.com/laminlabs/lndb/pull/386) | [Koncopd](https://github.com/Koncopd) | 2023-05-30 |
 ⬆️ Upgrade to lnhub-rest 0.9.8 | [384](https://github.com/laminlabs/lndb/pull/384) | [falexwolf](https://github.com/falexwolf) | 2023-05-28 | 0.45a4
 ⬆️ Upgrade lnhub-rest to 0.9.7 | [383](https://github.com/laminlabs/lndb/pull/383) | [falexwolf](https://github.com/falexwolf) | 2023-05-28 | 0.45a3
 📝 Add setup overview from lamindb | [382](https://github.com/laminlabs/lndb/pull/382) | [falexwolf](https://github.com/falexwolf) | 2023-05-27 |
```

### Comparing `lamindb_setup-0.46a2/docs/faq/check-synchronization.ipynb` & `lamindb_setup-0.46a3/docs/faq/check-synchronization.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/docs/faq/clone.ipynb` & `lamindb_setup-0.46a3/docs/faq/clone.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/docs/faq/edge-cases-login-init.ipynb` & `lamindb_setup-0.46a3/docs/faq/edge-cases-login-init.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/docs/faq/manage-migrations.ipynb` & `lamindb_setup-0.46a3/docs/faq/manage-migrations.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/docs/faq/switch-environment.ipynb` & `lamindb_setup-0.46a3/docs/faq/switch-environment.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/docs/faq/test-migrations-e2e.ipynb` & `lamindb_setup-0.46a3/docs/faq/test-migrations-e2e.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/docs/faq/test-migrations-unit.ipynb` & `lamindb_setup-0.46a3/docs/faq/test-migrations-unit.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/docs/guide/00-index.ipynb` & `lamindb_setup-0.46a3/docs/guide/00-index.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/docs/guide/01-setup-user.ipynb` & `lamindb_setup-0.46a3/docs/guide/01-setup-user.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/docs/guide/02-init-instance.ipynb` & `lamindb_setup-0.46a3/docs/guide/02-init-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/docs/guide/03-load-instance.ipynb` & `lamindb_setup-0.46a3/docs/guide/03-load-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/docs/guide/04-set-storage.ipynb` & `lamindb_setup-0.46a3/docs/guide/04-set-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/docs/guide/05-schema-modules.ipynb` & `lamindb_setup-0.46a3/docs/guide/05-schema-modules.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/docs/guide/migrate.md` & `lamindb_setup-0.46a3/docs/guide/migrate.md`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lamindb_setup/__init__.py` & `lamindb_setup-0.46a3/lamindb_setup/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,16 +49,16 @@
    :toctree:
 
    dev
 """
 
 import os
 
-__version__ = "0.46a2"  # denote a release candidate for 0.1.0 with 0.1rc1
-_USE_DJANGO = os.getenv("LAMINDB_USE_DJANGO") is not None
+__version__ = "0.46a3"  # denote a release candidate for 0.1.0 with 0.1rc1
+_USE_DJANGO = os.getenv("LAMINDB_USE_DJANGO") == "1"
 # _USE_DJANGO = True
 if _USE_DJANGO:
     print("using django backend")
 
 import builtins
 import sys
 from os import name as _os_name
```

### Comparing `lamindb_setup-0.46a2/lamindb_setup/__main__.py` & `lamindb_setup-0.46a3/lamindb_setup/__main__.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lamindb_setup/_check_instance_setup.py` & `lamindb_setup-0.46a3/lamindb_setup/_check_instance_setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,33 @@
+import importlib
+
 from lamin_logger import logger
 
 from . import _USE_DJANGO
 from .dev._settings_store import current_instance_settings_file
 
 
 def check_instance_setup(from_lamindb: bool = False):
     if current_instance_settings_file().exists():
         try:
             # attempt loading the settings file
             from .dev._settings_load import load_instance_settings
 
-            load_instance_settings()
+            isettings = load_instance_settings()
 
             if _USE_DJANGO:
-                from .dev._django import IS_SETUP
+                from .dev._django import IS_SETUP, setup_django
 
-                if not IS_SETUP:
-                    return False
+                if from_lamindb:
+                    setup_django(isettings)
+                    import lnschema_core
+
+                    importlib.reload(lnschema_core)
+                else:
+                    return IS_SETUP
 
             # if importing from lamindb, also ensure migrations are correct
             if from_lamindb and not _USE_DJANGO:
                 # attempt accessing settings and migrating the instance
                 from . import settings
                 from ._migrate import check_deploy_migration
```

### Comparing `lamindb_setup-0.46a2/lamindb_setup/_close.py` & `lamindb_setup-0.46a3/lamindb_setup/_close.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lamindb_setup/_delete.py` & `lamindb_setup-0.46a3/lamindb_setup/_delete.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lamindb_setup/_init_instance.py` & `lamindb_setup-0.46a3/lamindb_setup/_init_instance.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,32 +27,32 @@
 
 def register(isettings: InstanceSettings, usettings):
     """Register user & storage in DB."""
     if _USE_DJANGO:
         from lnschema_core.models import Storage, User
 
         user, created = User.objects.update_or_create(
-            id=usettings.get_id_as_int(),
+            id=usettings.id,
             defaults=dict(
                 handle=usettings.handle,
                 name=usettings.name,
                 email=usettings.email,
             ),
         )
+        if created:
+            logger.success(f"Saved: {user}")
         storage, created = Storage.objects.update_or_create(
             root=isettings.storage.root_as_str,
             defaults=dict(
                 root=isettings.storage.root_as_str,
                 region=isettings.storage.region,
             ),
         )
         if created:
-            logger.success(
-                f"Added storage root {storage.id}:  {isettings.storage.root_as_str}"
-            )
+            logger.success(f"Saved: {storage}")
     else:
         upsert.user(usettings.email, usettings.id, usettings.handle, usettings.name)
         insert_if_not_exists.storage(isettings.storage)
 
 
 def reload_lamindb(isettings: InstanceSettings):
     # only touch lamindb if we're operating from lamindb
```

### Comparing `lamindb_setup-0.46a2/lamindb_setup/_load_instance.py` & `lamindb_setup-0.46a3/lamindb_setup/_load_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lamindb_setup/_migrate/alembic.ini` & `lamindb_setup-0.46a3/lamindb_setup/_migrate/alembic.ini`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lamindb_setup/_migrate/core.py` & `lamindb_setup-0.46a3/lamindb_setup/_migrate/core.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lamindb_setup/_migrate/deploy.py` & `lamindb_setup-0.46a3/lamindb_setup/_migrate/deploy.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lamindb_setup/_migrate/env.py` & `lamindb_setup-0.46a3/lamindb_setup/_migrate/env.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lamindb_setup/_migrate/utils.py` & `lamindb_setup-0.46a3/lamindb_setup/_migrate/utils.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lamindb_setup/_notebook.py` & `lamindb_setup-0.46a3/lamindb_setup/_notebook.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lamindb_setup/_register_instance.py` & `lamindb_setup-0.46a3/lamindb_setup/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lamindb_setup/_schema.py` & `lamindb_setup-0.46a3/lamindb_setup/_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lamindb_setup/_set.py` & `lamindb_setup-0.46a3/lamindb_setup/_set.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lamindb_setup/_settings.py` & `lamindb_setup-0.46a3/lamindb_setup/_settings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lamindb_setup/_setup_user.py` & `lamindb_setup-0.46a3/lamindb_setup/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lamindb_setup/dev/_clone.py` & `lamindb_setup-0.46a3/lamindb_setup/dev/_clone.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lamindb_setup/dev/_db.py` & `lamindb_setup-0.46a3/lamindb_setup/dev/_db.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lamindb_setup/dev/_deprecated.py` & `lamindb_setup-0.46a3/lamindb_setup/dev/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lamindb_setup/dev/_django.py` & `lamindb_setup-0.46a3/lamindb_setup/dev/_django.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lamindb_setup/dev/_exclusion.py` & `lamindb_setup-0.46a3/lamindb_setup/dev/_exclusion.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lamindb_setup/dev/_settings_instance.py` & `lamindb_setup-0.46a3/lamindb_setup/dev/_settings_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import sqlalchemy as sa
 import sqlmodel as sqm
 from lamin_logger import logger
 from pydantic import PostgresDsn
 from sqlalchemy.future import Engine
 
+from .. import _USE_DJANGO
 from ._exclusion import empty_locker, get_locker
 from ._settings_save import save_instance_settings
 from ._settings_store import current_instance_settings_file, instance_settings_file
 from ._storage import StorageSettings
 from .upath import UPath
 
 # leave commented out until we understand more how to deal with
@@ -26,14 +27,28 @@
 # def _set_sqlite_pragma(dbapi_connection, connection_record):
 #     if isinstance(dbapi_connection, SQLite3Connection):
 #         cursor = dbapi_connection.cursor()
 #         cursor.execute("PRAGMA foreign_keys=ON;")
 #         cursor.close()
 
 
+class DjangoSession:
+    def delete(self, record):
+        record.delete()
+
+    def commit(self):
+        pass
+
+    def close(self):
+        pass
+
+    def refresh(self, record):
+        pass
+
+
 class InstanceSettings:
     """Instance settings."""
 
     def __init__(
         self,
         owner: str,  # owner handle
         name: str,  # instance name
@@ -150,16 +165,18 @@
 
     def session(self) -> sqm.Session:
         """Database session.
 
         In case of remote sqlite, updates the local sqlite file first.
         """
         self._update_local_sqlite_file()
-
-        return sqm.Session(self.engine, expire_on_commit=False)
+        if _USE_DJANGO:
+            return DjangoSession()
+        else:
+            return sqm.Session(self.engine, expire_on_commit=False)
 
     @property
     def is_cloud_sqlite(self) -> bool:
         # can we make this a private property, Sergei?
         # as it's not relevant to the user
         """Is this a cloud instance with sqlite db."""
         return self.dialect == "sqlite" and self.storage.is_cloud
```

### Comparing `lamindb_setup-0.46a2/lamindb_setup/dev/_settings_load.py` & `lamindb_setup-0.46a3/lamindb_setup/dev/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lamindb_setup/dev/_settings_save.py` & `lamindb_setup-0.46a3/lamindb_setup/dev/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lamindb_setup/dev/_settings_store.py` & `lamindb_setup-0.46a3/lamindb_setup/dev/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lamindb_setup/dev/_settings_user.py` & `lamindb_setup-0.46a3/lamindb_setup/dev/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lamindb_setup/dev/_setup_knowledge.py` & `lamindb_setup-0.46a3/lamindb_setup/dev/_setup_knowledge.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lamindb_setup/dev/_setup_schema.py` & `lamindb_setup-0.46a3/lamindb_setup/dev/_setup_schema.py`

 * *Files 18% similar despite different names*

```diff
@@ -74,25 +74,14 @@
         insert.user(
             email=usettings.email,
             user_id=usettings.id,
             handle=usettings.handle,
             name=usettings.name,
         )
 
-    else:
-        from lnschema_core.models import User
-
-        user = User(
-            id=usettings.get_id_as_int(),
-            email=usettings.email,
-            handle=usettings.handle,
-            name=usettings.name,
-        )
-        user.save()
-
     if not _USE_DJANGO:
         for schema_name in schema_names:
             schema_module = importlib.import_module(get_schema_module_name(schema_name))
             insert.version(
                 schema_module=schema_module,
                 user_id=usettings.id,  # type: ignore
                 cloud_sqlite=False,
```

### Comparing `lamindb_setup-0.46a2/lamindb_setup/dev/_storage.py` & `lamindb_setup-0.46a3/lamindb_setup/dev/_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lamindb_setup/dev/upath.py` & `lamindb_setup-0.46a3/lamindb_setup/dev/upath.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lamindb_setup/test/_migrations_e2e.py` & `lamindb_setup-0.46a3/lamindb_setup/test/_migrations_e2e.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lamindb_setup/test/_migrations_unit.py` & `lamindb_setup-0.46a3/lamindb_setup/test/_migrations_unit.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/.github/workflows/build.yml` & `lamindb_setup-0.46a3/lnschema-core/.github/workflows/build.yml`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         run: docker pull postgres:latest && docker image save postgres:latest --output ~/postgres.tar
       - name: cache postgres use
         if: steps.cache-postgres.outputs.cache-hit == 'true'
         run: docker image load --input ~/postgres.tar
       - name: install Python deps
         run: |
           python -m pip install -U pip
-          pip install laminci
+          pip install laminci requests
       - name: install apt-get deps
         run: |
           sudo apt-get -y install graphviz
           sudo apt-get install libpq-dev
       - name: Configure AWS
         uses: aws-actions/configure-aws-credentials@v1
         with:
```

### Comparing `lamindb_setup-0.46a2/lnschema-core/.github/workflows/latest-changes.yml` & `lamindb_setup-0.46a3/lnschema-core/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/.gitignore` & `lamindb_setup-0.46a3/lnschema-core/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/.pre-commit-config.yaml` & `lamindb_setup-0.46a3/lnschema-core/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/LICENSE` & `lamindb_setup-0.46a3/lnschema-core/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/django_project/settings.py` & `lamindb_setup-0.46a3/lnschema-core/django_project/settings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/django_project/urls.py` & `lamindb_setup-0.46a3/lnschema-core/django_project/urls.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/docs/changelog.md` & `lamindb_setup-0.46a3/lnschema-core/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🚚 Rename lndb to lamindb-setup | [176](https://github.com/laminlabs/lnschema-core/pull/176) | [falexwolf](https://github.com/falexwolf) | 2023-06-01 | 0.35a2
 🏗️ Add Django backend | [175](https://github.com/laminlabs/lnschema-core/pull/175) | [falexwolf](https://github.com/falexwolf) | 2023-05-31 | 0.35a1
 👷 Refactor CI | [174](https://github.com/laminlabs/lnschema-core/pull/174) | [falexwolf](https://github.com/falexwolf) | 2023-05-30 |
 🏗️ Remove SQL-level schema modules | [172](https://github.com/laminlabs/lnschema-core/pull/172) | [falexwolf](https://github.com/falexwolf) | 2023-05-25 | 0.34.0
 🏗️ Introduce Django skeleton | [171](https://github.com/laminlabs/lnschema-core/pull/171) | [falexwolf](https://github.com/falexwolf) | 2023-05-24 |
 ♻️ Refactor types | [170](https://github.com/laminlabs/lnschema-core/pull/170) | [falexwolf](https://github.com/falexwolf) | 2023-05-23 |
 ♻️ Refactor `BaseORM` | [169](https://github.com/laminlabs/lnschema-core/pull/169) | [falexwolf](https://github.com/falexwolf) | 2023-05-17 | 0.33.8
 🚸 Add `lazy="joined"` to some cheap joins | [168](https://github.com/laminlabs/lnschema-core/pull/168) | [falexwolf](https://github.com/falexwolf) | 2023-05-16 | 0.33.7
```

### Comparing `lamindb_setup-0.46a2/lnschema-core/docs/guide/0-core-schema.ipynb` & `lamindb_setup-0.46a3/lnschema-core/docs/guide/0-core-schema.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/docs/guide/1-data-validation.ipynb` & `lamindb_setup-0.46a3/lnschema-core/docs/guide/1-data-validation.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/_core.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/_core.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/_link.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/_link.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/_types.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/_types.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/dev/_id.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/dev/_id.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/dev/_versions.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/dev/_versions.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/dev/id.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/dev/id.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/dev/sqlmodel.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/dev/sqlmodel.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 
    BaseORM
 """
 
 import importlib
 import re
 import typing
-from collections import namedtuple
-from typing import Any, Iterable, Optional, Sequence, Tuple, Union
+from typing import Any, NamedTuple, Optional, Sequence, Tuple, Union
 
 import sqlmodel as sqm
 from pydantic import create_model
 from sqlalchemy.orm import declared_attr
 from sqlalchemy.orm import relationship as sa_relationship
 from sqlalchemy.orm.relationships import RelationshipProperty
 from sqlalchemy.orm.session import object_session
 from typeguard import check_type
 
 from .. import __name__
+from .._lookup import lookup as _lookup
 
 MODULE_NAME = __name__
 
 # add naming convention for alembic
 sqm.SQLModel.metadata.naming_convention = {
     "ix": "ix_%(column_0_label)s",
     "uq": "uq_%(table_name)s_%(column_0_name)s",
@@ -57,34 +57,16 @@
     def __init__(self, **user_kwargs):
         # pydantic does not enforce strict type checking for complex types, only their attributes
         validate_relationship_types(self, user_kwargs)
         super().__init__(**user_kwargs)
         validate_with_pydantic(self, user_kwargs)
 
     @classmethod
-    def lookup(cls, field: Optional[str] = None):
-        """Lookup rows by field."""
-        import lamindb as ln
-
-        if field is None:
-            # by default use the name field
-            if "name" in cls.__fields__:
-                field = "name"
-            else:
-                non_ids = [i for i in cls.__fields__.keys() if "id" not in i]
-                if len(non_ids) > 0:
-                    # the first field isn't named with id
-                    field = non_ids[0]
-                else:
-                    # the first field
-                    field = next(iter(cls.__fields__.keys()))
-        df = ln.select(cls).df()
-        values = set(df[field].values)
-        keys = _to_lookup_keys(values, padding=cls.__name__)
-        return _namedtuple_from_dict(d=dict(zip(keys, values)), name=cls.__name__)
+    def lookup(cls, field: Optional[str] = None) -> NamedTuple:
+        return _lookup(cls, field)
 
     @declared_attr
     def __tablename__(cls) -> str:  # type: ignore
         """Prefix table name with module name as in Django."""
         return f"{MODULE_NAME}_{cls.__name__.lower()}"
 
 
@@ -369,22 +351,7 @@
 #             return lookup_field
 
 #         sqlmodel_class.df = df
 #         sqlmodel_class.lookup = lookup
 #         return sqlmodel_class
 
 #     return wrapper
-
-
-def _to_lookup_keys(x: Iterable[str], padding: str = "LOOKUP") -> list:
-    """Convert a list of strings to tab-completion allowed formats."""
-    lookup = [re.sub("[^0-9a-zA-Z]+", "_", str(i)) for i in x]
-    for i, value in enumerate(lookup):
-        if value == "" or (not value[0].isalpha()):
-            lookup[i] = f"{padding}_{value}"
-    return lookup
-
-
-def _namedtuple_from_dict(d: dict, name: str = "entity") -> tuple:
-    """Create a namedtuple from a dict to allow autocompletion."""
-    nt = namedtuple(name, d.keys())  # type:ignore
-    return nt(**d)
```

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/manage.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/manage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/0001_initial.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-07-21-0560ee3d73dc-jupynb.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-07-21-0560ee3d73dc-jupynb.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-08-08-8c78543d1c5b-v0_3_0.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-08-08-8c78543d1c5b-v0_3_0.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-08-19-1c531ea346cf-storage.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-08-19-1c531ea346cf-storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-08-22-01fcb82dafd4-v0_4_0.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-08-22-01fcb82dafd4-v0_4_0.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-08-26-3badf20f18c8-v0_5_0.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-08-26-3badf20f18c8-v0_5_0.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-08-29-d1b3e5da6391-v0_5_1.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-08-29-d1b3e5da6391-v0_5_1.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-09-15-5fa54c55c3bf-v0_6_0.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-09-15-5fa54c55c3bf-v0_6_0.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-09-18-049d7dfc80a8-v0_7_1.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-09-18-049d7dfc80a8-v0_7_1.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-09-18-3b60b87450c0-v0_7_0.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-09-18-3b60b87450c0-v0_7_0.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-09-24-1f29517759b7-v0_7_3.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-09-24-1f29517759b7-v0_7_3.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-09-25-7e8f7b30792e-v0_8_0.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-09-25-7e8f7b30792e-v0_8_0.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-09-26-1190648443cb-v0_8_1.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-09-26-1190648443cb-v0_8_1.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-09-30-439c4ee0a22a-v0_9_0.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-09-30-439c4ee0a22a-v0_9_0.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-10-07-0c819d33ca9b-v0_10_0.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-10-07-0c819d33ca9b-v0_10_0.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-10-10-3d244a8d3148-v0_11_0.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-10-10-3d244a8d3148-v0_11_0.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-10-11-2ddcb037e3ea-v0_12_0.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-10-11-2ddcb037e3ea-v0_12_0.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-10-19-cf5913791674-v0_14_0.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-10-19-cf5913791674-v0_14_0.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-10-31-98da12fc80a8-v0_15_0.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-10-31-98da12fc80a8-v0_15_0.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-11-10-4ee426b656bb-v0_16_0.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-11-10-4ee426b656bb-v0_16_0.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-11-11-66bfd6cf2e2d-v0_17_0.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-11-11-66bfd6cf2e2d-v0_17_0.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-11-28-4b4005b7841c-v0_21_1.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-11-28-4b4005b7841c-v0_21_1.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-12-07-9d94f3b9566d-v0_21_3.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-12-07-9d94f3b9566d-v0_21_3.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2022-12-07-db1df7b2aaad-v0_22_0.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2022-12-07-db1df7b2aaad-v0_22_0.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-01-09-f6b6b85cdffc-v0_24_0.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-01-09-f6b6b85cdffc-v0_24_0.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-02-02-9d283a1685a5-v0_25_6.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-02-02-9d283a1685a5-v0_25_6.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-02-07-8bf788467d0a-v0_25_9.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-02-07-8bf788467d0a-v0_25_9.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-02-10-ff3b5b3ec913-v0_26_1.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-02-10-ff3b5b3ec913-v0_26_1.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-02-14-8280855a5064-v0_26_2.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-02-14-8280855a5064-v0_26_2.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-02-21-1dafcf0b22aa-v0_28_0.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-02-21-1dafcf0b22aa-v0_28_0.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-02-22-6952574e2d49-v0_28_1.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-02-22-6952574e2d49-v0_28_1.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-02-23-24e55331f27c-v0_28_2.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-02-23-24e55331f27c-v0_28_2.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-02-24-873683a29806-v0_28_7.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-02-24-873683a29806-v0_28_7.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-03-21-9640062eefee-v0_30rc1.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-03-21-9640062eefee-v0_30rc1.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-03-23-ebafd37fd6e1-v0_30rc2.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-03-23-ebafd37fd6e1-v0_30rc2.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-03-24-5846a15d9241-0_30rc3.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-03-24-5846a15d9241-0_30rc3.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-04-05-6de59093e378-v0_32_0.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-04-05-6de59093e378-v0_32_0.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-04-13-d161a14a12e3-v0_32_1.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-04-13-d161a14a12e3-v0_32_1.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-04-16-6a73c00555b4-v0_33_0.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-04-16-6a73c00555b4-v0_33_0.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-05-24-c3f38ffe9e03-v0_34a1.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-05-24-c3f38ffe9e03-v0_34a1.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/migrations/versions/2023-05-28-1c49c9f9a982-v0_34a2.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/migrations/versions/2023-05-28-1c49c9f9a982-v0_34a2.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/lnschema_core/models.py` & `lamindb_setup-0.46a3/lnschema-core/lnschema_core/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,92 +1,153 @@
 from pathlib import Path, PurePosixPath
-from typing import Any, List, Optional, Union
+from typing import Any, List, NamedTuple, Optional, Union
 
+import pandas as pd
 from django.db import models
-from django.db.models import Model as BaseORM
 from lamin_logger import logger
 from nbproject._is_run_from_ipython import is_run_from_ipython
 from upath import UPath
 
-from ._users import current_user_id_as_int
+from ._lookup import lookup as _lookup
+from ._users import current_user_id
+from .dev import id as idg
 from .types import DataLike, ListLike, PathLike, TransformType
 
 
-class RunInput(models.Model):
+class NoResultFound(Exception):
+    pass
+
+
+class MultipleResultsFound(Exception):
+    pass
+
+
+class LaminQuerySet(models.QuerySet):
+    def df(self):
+        return pd.DataFrame(self.values())
+
+    def list(self):
+        return list(self)
+
+    def first(self):
+        if len(self) == 0:
+            return None
+        return self[0]
+
+    def one(self):
+        if len(self) == 0:
+            raise NoResultFound
+        elif len(self) > 1:
+            raise MultipleResultsFound
+        else:
+            return self[0]
+
+    def one_or_none(self):
+        if len(self) == 0:
+            return None
+        elif len(self) == 1:
+            return self[0]
+        else:
+            raise MultipleResultsFound
+
+
+class BaseORM(models.Model):
+    def __repr__(self) -> str:
+        fields = ", ".join([f"{k.name}={getattr(self, k.name)}" for k in self._meta.fields])
+        return f"{self.__class__.__name__}({fields})"
+
+    @classmethod
+    def lookup(cls, field: Optional[str] = None) -> NamedTuple:
+        return _lookup(cls, field)
+
+    def __str__(self) -> str:
+        return self.__repr__()
+
+    class Meta:
+        abstract = True
+
+
+class RunInput(BaseORM):
     run = models.ForeignKey("Run", on_delete=models.CASCADE)
     file = models.ForeignKey("File", on_delete=models.CASCADE)
 
     class Meta:
         managed = True
 
 
 class User(BaseORM):
+    id = models.CharField(max_length=8, primary_key=True)
     email = models.CharField(max_length=64, unique=True)
     handle = models.CharField(max_length=64, unique=True)
     name = models.CharField(max_length=64, blank=True, null=True)
     created_at = models.DateTimeField(auto_now_add=True)
     updated_at = models.DateTimeField(auto_now=True)
 
     class Meta:
         managed = True
 
 
 class Storage(BaseORM):
+    id = models.CharField(max_length=8, default=idg.storage, primary_key=True)
     root = models.CharField(max_length=255)
     type = models.CharField(max_length=63, blank=True, null=True)
     region = models.CharField(max_length=63, blank=True, null=True)
     created_at = models.DateTimeField(auto_now_add=True)
     updated_at = models.DateTimeField(auto_now=True)
-    created_by = models.ForeignKey(User, models.DO_NOTHING, blank=True, null=True, default=current_user_id_as_int)
+    created_by = models.ForeignKey(User, models.DO_NOTHING, blank=True, null=True, default=current_user_id)
 
     class Meta:
         managed = True
 
 
 class Project(BaseORM):
+    id = models.CharField(max_length=8, default=idg.project, primary_key=True)
     name = models.CharField(max_length=64)
     folders = models.ManyToManyField("Folder")
     files = models.ManyToManyField("File")
-    created_by = models.ForeignKey(User, models.DO_NOTHING, default=current_user_id_as_int)
+    created_by = models.ForeignKey(User, models.DO_NOTHING, default=current_user_id)
     created_at = models.DateTimeField(auto_now_add=True)
     updated_at = models.DateTimeField(auto_now=True)
 
     class Meta:
         managed = True
 
 
-class Transform(models.Model):
-    name = models.CharField(max_length=63)
-    version = models.CharField(max_length=63)
+class Transform(BaseORM):
+    name = models.CharField(max_length=127)
+    hash = models.CharField(max_length=12, default=idg.transform)
+    version = models.CharField(max_length=10, default="0")
     type = models.CharField(max_length=63, choices=TransformType.choices(), db_index=True, default=(TransformType.notebook if is_run_from_ipython else TransformType.pipeline))
     title = models.CharField(max_length=63, blank=True, null=True)
     reference = models.CharField(max_length=63, blank=True, null=True)
-    created_by = models.ForeignKey(User, models.DO_NOTHING)
+    created_by = models.ForeignKey(User, models.DO_NOTHING, default=current_user_id)
     created_at = models.DateTimeField(auto_now_add=True)
     updated_at = models.DateTimeField(auto_now=True)
 
     class Meta:
         managed = True
         unique_together = (("name", "version"),)
 
 
-class Run(models.Model):
+class Run(BaseORM):
+    id = models.CharField(max_length=12, default=idg.run, primary_key=True)
     name = models.CharField(max_length=255, blank=True, null=True)
     external_id = models.CharField(max_length=255, blank=True, null=True)
     transform = models.ForeignKey(Transform, models.DO_NOTHING)
     inputs = models.ManyToManyField("File", through=RunInput, related_name="input_of")
     # outputs on File
-    created_by = models.ForeignKey(User, models.DO_NOTHING)
+    created_by = models.ForeignKey(User, models.DO_NOTHING, default=current_user_id)
     created_at = models.DateTimeField(auto_now_add=True)
 
     class Meta:
         managed = True
 
-    def __init__(  # type: ignore
-        self,
+    @classmethod
+    def create(  # type: ignore
+        cls,
         *,
         id: Optional[str] = None,
         name: Optional[str] = None,
         load_latest: bool = False,
         external_id: Optional[str] = None,
         transform: Optional[Transform] = None,
         inputs: List["File"] = None,
@@ -105,50 +166,47 @@
                 raise ValueError("Either call `ln.Run(transform=transform)` or `ln.track(transform=...)`.")
 
         if not isinstance(transform, Transform):
             raise TypeError("transform needs to be of type Transform")
 
         run = None
         if load_latest:
-            run = (
-                ln.select(
-                    ln.Run,
-                    transform_id=transform.id,
-                    transform_version=transform.version,
-                )
-                .order_by(ln.Run.created_at.desc())
-                .first()
-            )
+            run = ln.select(ln.Run, transform=transform).order_by("-created_at").first()
             if run is not None:
                 logger.info(f"Loaded: {run}")
         elif id is not None:
             run = ln.select(ln.Run, id=id).one_or_none()
             if run is None:
                 raise NotImplementedError("You can currently only pass existing ids")
 
         if run is None:
-            kwargs.update(dict(transform_id=transform.id, transform_version=transform.version))
-            super().__init__(**kwargs)
-            self._ln_identity_key = None
+            kwargs["transform_id"] = transform.id
+            if "load_latest" in kwargs:
+                del kwargs["load_latest"]
+            del kwargs["cls"]
+            run = cls(**kwargs)
+            run._ln_identity_key = None
         else:
-            super().__init__(**run.dict())
-            self._ln_identity_key = run.id  # simulate query result
+            run = cls(**run.dict())
+            run._ln_identity_key = run.id  # simulate query result
 
         if global_context:
             if run is None:
-                added_self = ln.add(self)
-                self._ln_identity_key = added_self.id
-                logger.success(f"Added: {self}")
-            ln.context.run = self
+                added_self = ln.add(run)
+                run._ln_identity_key = added_self.id  # type: ignore
+                logger.success(f"Saved: {run}")
+            ln.context.run = run
+
+        return run
 
 
-class Features(models.Model):
+class Features(BaseORM):
     id = models.CharField(max_length=63, primary_key=True)
     type = models.CharField(max_length=63)
-    created_by = models.ForeignKey(User, models.DO_NOTHING, default=current_user_id_as_int)
+    created_by = models.ForeignKey(User, models.DO_NOTHING, default=current_user_id)
     created_at = models.DateTimeField(auto_now=True)
     files = models.ManyToManyField("File")
 
     class Meta:
         managed = True
 
     def __init__(  # type: ignore
@@ -193,22 +251,23 @@
                 **map_kwargs,
             )
         else:
             features = super().__new__(cls)
         return features
 
 
-class Folder(models.Model):
+class Folder(BaseORM):
+    id = models.CharField(max_length=20, primary_key=True)
     name = models.CharField(max_length=255)
     key = models.CharField(max_length=255, blank=True, null=True)
     storage = models.ForeignKey(Storage, models.DO_NOTHING)
     files = models.ManyToManyField("File")
-    created_by = models.ForeignKey(User, models.DO_NOTHING, default=current_user_id_as_int)
-    created_at = models.DateTimeField()
-    updated_at = models.DateTimeField(blank=True, null=True)
+    created_by = models.ForeignKey(User, models.DO_NOTHING, default=current_user_id)
+    created_at = models.DateTimeField(auto_now_add=True)
+    updated_at = models.DateTimeField(auto_now=True)
 
     class Meta:
         managed = True
         unique_together = (("storage", "key"),)
 
     @property
     def __name__(cls) -> str:
@@ -230,59 +289,63 @@
         return tree(
             dir_path=self.path(),
             level=level,
             limit_to_directories=limit_to_directories,
             length_limit=length_limit,
         )
 
-    def __init__(  # type: ignore
-        self,
+    @classmethod
+    def create(  # type: ignore
+        cls,
         path: Optional[Union[Path, UPath, str]] = None,
         *,
         # continue with fields
-        id: Optional[str] = None,
         name: Optional[str] = None,
         key: Optional[str] = None,
         storage_id: Optional[str] = None,
         files: List["File"] = [],
     ):
         if path is not None:
             from lamindb._folder import get_folder_kwargs_from_data
 
             kwargs, privates = get_folder_kwargs_from_data(
                 path=path,
                 name=name,
                 key=key,
             )
-            if id is not None:
-                kwargs["id"] = id
         else:
             kwargs = {k: v for k, v in locals().items() if v and k != "self"}
+        kwargs["id"] = idg.folder()
 
-        super().__init__(**kwargs)
+        files = kwargs.pop("files")
+
+        folder = cls(**kwargs)
         if path is not None:
-            self._local_filepath = privates["local_filepath"]
-            self._cloud_filepath = privates["cloud_filepath"]
+            folder._local_filepath = privates["local_filepath"]
+            folder._cloud_filepath = privates["cloud_filepath"]
+            folder._files = files
+        return folder
 
 
-class File(models.Model):
+class File(BaseORM):
+    id = models.CharField(max_length=20, primary_key=True)
     name = models.CharField(max_length=255, blank=True, null=True)
     suffix = models.CharField(max_length=63, blank=True, null=True)
     size = models.BigIntegerField(blank=True, null=True)
     hash = models.CharField(max_length=63, blank=True, null=True)
     key = models.CharField(max_length=255, blank=True, null=True)
     run = models.ForeignKey(Run, models.DO_NOTHING, blank=True, null=True, related_name="outputs")
     transform = models.ForeignKey(Transform, models.DO_NOTHING, blank=True, null=True)
     storage = models.ForeignKey(Storage, models.DO_NOTHING)
     # folders from Folders.files
     # features from Features.files
     # input_of from Run.inputs
     created_at = models.DateTimeField(auto_now_add=True)
     updated_at = models.DateTimeField(auto_now=True)
-    created_by = models.ForeignKey(User, models.DO_NOTHING, default=current_user_id_as_int)
+    created_by = models.ForeignKey(User, models.DO_NOTHING, default=current_user_id)
 
     class Meta:
         managed = True
         unique_together = (("storage", "key"),)
 
     def path(self) -> Union[Path, UPath]:
         """Path on storage."""
@@ -342,16 +405,17 @@
         self._memory_rep = privates["memory_rep"]
         self._to_store = not privates["check_path_in_storage"]  # no need to upload if new file is already in storage
 
     @property
     def __name__(cls) -> str:
         return "File"
 
-    def __init__(  # type: ignore
-        self,
+    @classmethod
+    def create(  # type: ignore
+        cls,
         data: Union[PathLike, DataLike] = None,
         *,
         key: Optional[str] = None,
         name: Optional[str] = None,
         run: Optional[Run] = None,
         format: Optional[str] = None,
         features: List[Features] = None,
@@ -381,14 +445,15 @@
         kwargs, privates = get_file_kwargs_from_data(
             data=data,
             name=name,
             key=key,
             run=run,
             format=format,
         )
+        kwargs["id"] = idg.file()
         if features is not None:
             kwargs["features"] = features
         log_hint(
             check_path_in_storage=privates["check_path_in_storage"],
             key=kwargs["key"],
             id=kwargs["id"],
             suffix=kwargs["suffix"],
@@ -396,29 +461,35 @@
 
         # transform cannot be directly passed, just via run
         # it's directly stored in the file table to avoid another join
         # mediate by the run table
         if kwargs["run"] is not None:
             if kwargs["run"].transform_id is not None:
                 kwargs["transform_id"] = kwargs["run"].transform_id
-                assert kwargs["run"].transform_version is not None
-                kwargs["transform_version"] = kwargs["run"].transform_version
             else:
                 # accessing the relationship should always be possible if
                 # the above if clause was false as then, we should have a fresh
                 # Transform object that is not queried from the DB
                 assert kwargs["run"].transform is not None
                 kwargs["transform"] = kwargs["run"].transform
 
-        super().__init__(**kwargs)
+        file = cls(**kwargs)
         if data is not None:
-            self._local_filepath = privates["local_filepath"]
-            self._cloud_filepath = privates["cloud_filepath"]
-            self._memory_rep = privates["memory_rep"]
-            self._to_store = not privates["check_path_in_storage"]
+            file._local_filepath = privates["local_filepath"]
+            file._cloud_filepath = privates["cloud_filepath"]
+            file._memory_rep = privates["memory_rep"]
+            file._to_store = not privates["check_path_in_storage"]
+        return file
+
+    def save(self, *args, **kwargs):
+        if self.transform is not None:
+            self.transform.save()
+        if self.run is not None:
+            self.run.save()
+        super().save(*args, **kwargs)
 
 
 # add type annotations back asap when re-organizing the module
 def storage_key_from_file(file: File):
     if file.key is None:
         return f"{file.id}{file.suffix}"
     else:
```

### Comparing `lamindb_setup-0.46a2/lnschema-core/manage.py` & `lamindb_setup-0.46a3/lnschema-core/manage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/pyproject.toml` & `lamindb_setup-0.46a3/lnschema-core/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/lnschema-core/tests/test_migrations.py` & `lamindb_setup-0.46a3/lnschema-core/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/noxfile.py` & `lamindb_setup-0.46a3/noxfile.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/pyproject.toml` & `lamindb_setup-0.46a3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/tests/test_bionty.py` & `lamindb_setup-0.46a3/tests/test_bionty.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/tests/test_init_instance.py` & `lamindb_setup-0.46a3/tests/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/tests/test_load_instance.py` & `lamindb_setup-0.46a3/tests/test_load_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a2/PKG-INFO` & `lamindb_setup-0.46a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamindb_setup
-Version: 0.46a2
+Version: 0.46a3
 Summary: LaminDB setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnhub_rest==0.9.8
 Requires-Dist: lndb
 Requires-Dist: laminci>=0.3.0
 Requires-Dist: lnschema_core>=0.35a1
```

