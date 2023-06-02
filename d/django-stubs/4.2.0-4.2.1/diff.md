# Comparing `tmp/django-stubs-4.2.0.tar.gz` & `tmp/django-stubs-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-stubs-4.2.0.tar", last modified: Thu Apr 27 12:47:56 2023, max compression
+gzip compressed data, was "django-stubs-4.2.1.tar", last modified: Fri Jun  2 14:11:31 2023, max compression
```

## Comparing `django-stubs-4.2.0.tar` & `django-stubs-4.2.1.tar`

### file list

```diff
@@ -1,826 +1,833 @@
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.786592 django-stubs-4.2.0/
--rw-r--r--   0 marti     (1000) marti      (121)     1075 2023-03-15 16:53:32.000000 django-stubs-4.2.0/LICENSE.txt
--rw-r--r--   0 marti     (1000) marti      (121)    14046 2023-04-27 12:47:56.786592 django-stubs-4.2.0/PKG-INFO
--rw-r--r--   0 marti     (1000) marti      (121)    12881 2023-04-27 12:45:58.000000 django-stubs-4.2.0/README.md
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.669926 django-stubs-4.2.0/django-stubs/
--rw-r--r--   0 marti     (1000) marti      (121)      157 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.669926 django-stubs-4.2.0/django-stubs/apps/
--rw-r--r--   0 marti     (1000) marti      (121)       78 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/apps/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      855 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/apps/config.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1963 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/apps/registry.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.669926 django-stubs-4.2.0/django-stubs/conf/
--rw-r--r--   0 marti     (1000) marti      (121)     1387 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/conf/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    16655 2023-04-27 12:45:58.000000 django-stubs-4.2.0/django-stubs/conf/global_settings.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.669926 django-stubs-4.2.0/django-stubs/conf/locale/
--rw-r--r--   0 marti     (1000) marti      (121)       50 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/conf/locale/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.669926 django-stubs-4.2.0/django-stubs/conf/urls/
--rw-r--r--   0 marti     (1000) marti      (121)     1073 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/conf/urls/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      231 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/conf/urls/i18n.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      193 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/conf/urls/static.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.669926 django-stubs-4.2.0/django-stubs/contrib/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.676593 django-stubs-4.2.0/django-stubs/contrib/admin/
--rw-r--r--   0 marti     (1000) marti      (121)     1157 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/admin/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      313 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/admin/actions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      136 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/admin/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1075 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/admin/checks.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2208 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/admin/decorators.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      175 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/admin/exceptions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3887 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/admin/filters.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      237 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/admin/forms.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5562 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/admin/helpers.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.676593 django-stubs-4.2.0/django-stubs/contrib/admin/migrations/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/admin/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1032 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/admin/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    16126 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/admin/options.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4081 2023-04-27 12:45:58.000000 django-stubs-4.2.0/django-stubs/contrib/admin/sites.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.676593 django-stubs-4.2.0/django-stubs/contrib/admin/templatetags/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/admin/templatetags/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1981 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/admin/templatetags/admin_list.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      690 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/admin/templatetags/admin_modify.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      503 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/admin/templatetags/admin_urls.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      605 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/admin/templatetags/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      441 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/admin/templatetags/log.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1629 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/admin/tests.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3662 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/admin/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.676593 django-stubs-4.2.0/django-stubs/contrib/admin/views/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/admin/views/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      374 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/admin/views/autocomplete.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      383 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/admin/views/decorators.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3104 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/admin/views/main.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5455 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/admin/widgets.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.679926 django-stubs-4.2.0/django-stubs/contrib/admindocs/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/admindocs/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      129 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/admindocs/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      478 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/admindocs/middleware.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       60 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/admindocs/urls.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      840 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/admindocs/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1018 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/admindocs/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.679926 django-stubs-4.2.0/django-stubs/contrib/auth/
--rw-r--r--   0 marti     (1000) marti      (121)     1272 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/auth/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      496 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/auth/admin.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       68 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/auth/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1891 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/auth/backends.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1532 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/auth/base_user.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      398 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/auth/checks.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      662 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/auth/context_processors.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      934 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/auth/decorators.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3937 2023-04-27 12:45:58.000000 django-stubs-4.2.0/django-stubs/contrib/auth/forms.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.683259 django-stubs-4.2.0/django-stubs/contrib/auth/handlers/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/auth/handlers/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      198 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/auth/handlers/modwsgi.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1962 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/auth/hashers.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.683259 django-stubs-4.2.0/django-stubs/contrib/auth/management/
--rw-r--r--   0 marti     (1000) marti      (121)      405 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/auth/management/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.683259 django-stubs-4.2.0/django-stubs/contrib/auth/management/commands/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/auth/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      125 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/auth/management/commands/changepassword.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      208 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/auth/management/commands/createsuperuser.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      739 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/auth/middleware.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.683259 django-stubs-4.2.0/django-stubs/contrib/auth/migrations/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/auth/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1228 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/auth/mixins.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4613 2023-04-27 12:45:58.000000 django-stubs-4.2.0/django-stubs/contrib/auth/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2081 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/auth/password_validation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      120 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/auth/signals.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      728 2023-04-27 12:45:58.000000 django-stubs-4.2.0/django-stubs/contrib/auth/tokens.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       60 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/auth/urls.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      153 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/auth/validators.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2387 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/auth/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.683259 django-stubs-4.2.0/django-stubs/contrib/contenttypes/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/contenttypes/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      655 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/contenttypes/admin.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       76 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/contenttypes/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      414 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/contenttypes/checks.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3850 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/contenttypes/fields.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1420 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/contenttypes/forms.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.683259 django-stubs-4.2.0/django-stubs/contrib/contenttypes/management/
--rw-r--r--   0 marti     (1000) marti      (121)     1297 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/contenttypes/management/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.683259 django-stubs-4.2.0/django-stubs/contrib/contenttypes/management/commands/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/contenttypes/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      467 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/contenttypes/management/commands/remove_stale_contenttypes.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.683259 django-stubs-4.2.0/django-stubs/contrib/contenttypes/migrations/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/contenttypes/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1020 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/contenttypes/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      213 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/contenttypes/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.686593 django-stubs-4.2.0/django-stubs/contrib/flatpages/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/flatpages/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      196 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/flatpages/admin.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      129 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/flatpages/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      136 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/flatpages/forms.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      293 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/flatpages/middleware.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.686593 django-stubs-4.2.0/django-stubs/contrib/flatpages/migrations/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/flatpages/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      402 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/flatpages/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       81 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/flatpages/sitemaps.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.686593 django-stubs-4.2.0/django-stubs/contrib/flatpages/templatetags/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/flatpages/templatetags/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      484 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/flatpages/templatetags/flatpages.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       60 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/flatpages/urls.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      309 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/flatpages/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.686593 django-stubs-4.2.0/django-stubs/contrib/gis/
--rw-r--r--   0 marti     (1000) marti      (121)       24 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.689926 django-stubs-4.2.0/django-stubs/contrib/gis/admin/
--rw-r--r--   0 marti     (1000) marti      (121)      872 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/admin/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1174 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/admin/options.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      272 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/admin/widgets.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       67 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/apps.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.689926 django-stubs-4.2.0/django-stubs/contrib/gis/db/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.689926 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.689926 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/base/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/base/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      200 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/base/adapter.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1443 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/base/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      836 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/base/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1348 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/base/operations.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.689926 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/mysql/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/mysql/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      251 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/mysql/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      781 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/mysql/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      333 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/mysql/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1134 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/mysql/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      699 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/mysql/schema.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.693259 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/oracle/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/oracle/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      226 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/oracle/adapter.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      254 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/oracle/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      444 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/oracle/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      287 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/oracle/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      729 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/oracle/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1440 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/oracle/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      826 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/oracle/schema.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.693259 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/postgis/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/postgis/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      399 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/postgis/adapter.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      351 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/postgis/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      189 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/postgis/const.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      407 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/postgis/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      360 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/postgis/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      798 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/postgis/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2218 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/postgis/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      247 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/postgis/pgraster.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      340 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/postgis/schema.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.696593 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/spatialite/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/spatialite/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      182 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/spatialite/adapter.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      477 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/spatialite/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      127 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/spatialite/client.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      358 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/spatialite/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      451 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/spatialite/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      808 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/spatialite/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1286 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/spatialite/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1103 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/spatialite/schema.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      656 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.696593 django-stubs-4.2.0/django-stubs/contrib/gis/db/models/
--rw-r--r--   0 marti     (1000) marti      (121)      847 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/models/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      800 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/models/aggregates.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5021 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/models/fields.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     6016 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/models/functions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2955 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/models/lookups.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      345 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/models/proxy.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.696593 django-stubs-4.2.0/django-stubs/contrib/gis/db/models/sql/
--rw-r--r--   0 marti     (1000) marti      (121)      166 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/models/sql/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      829 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/db/models/sql/conversion.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      866 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/feeds.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.696593 django-stubs-4.2.0/django-stubs/contrib/gis/forms/
--rw-r--r--   0 marti     (1000) marti      (121)      642 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/forms/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      840 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/forms/fields.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      951 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/forms/widgets.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.699926 django-stubs-4.2.0/django-stubs/contrib/gis/gdal/
--rw-r--r--   0 marti     (1000) marti      (121)     1070 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/gdal/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      137 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/gdal/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      574 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/gdal/datasource.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      324 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/gdal/driver.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      688 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/gdal/envelope.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      200 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/gdal/error.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      947 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/gdal/feature.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1460 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/gdal/field.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4844 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/gdal/geometries.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      304 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/gdal/geomtype.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1721 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/gdal/layer.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      510 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/gdal/libgdal.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.699926 django-stubs-4.2.0/django-stubs/contrib/gis/gdal/prototypes/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/gdal/prototypes/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1036 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/gdal/prototypes/ds.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      961 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/gdal/prototypes/errcheck.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1077 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/gdal/prototypes/generation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      970 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/gdal/prototypes/geom.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1053 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/gdal/prototypes/raster.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      614 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/gdal/prototypes/srs.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.699926 django-stubs-4.2.0/django-stubs/contrib/gis/gdal/raster/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/gdal/raster/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1594 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/gdal/raster/band.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      225 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/gdal/raster/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      252 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/gdal/raster/const.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2180 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/gdal/raster/source.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2191 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/gdal/srs.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.703259 django-stubs-4.2.0/django-stubs/contrib/gis/geoip2/
--rw-r--r--   0 marti     (1000) marti      (121)      106 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/geoip2/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1202 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/geoip2/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       99 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/geoip2/resources.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       97 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/geometry.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.703259 django-stubs-4.2.0/django-stubs/contrib/gis/geos/
--rw-r--r--   0 marti     (1000) marti      (121)      883 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/geos/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      185 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/geos/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      604 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/geos/collections.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1250 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/geos/coordseq.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       36 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/geos/error.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      276 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/geos/factory.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5258 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/geos/geometry.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      491 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/geos/io.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      896 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/geos/libgeos.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      766 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/geos/linestring.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1148 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/geos/mutable_list.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      816 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/geos/point.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      713 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/geos/polygon.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      737 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/geos/prepared.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.706592 django-stubs-4.2.0/django-stubs/contrib/gis/geos/prototypes/
--rw-r--r--   0 marti     (1000) marti      (121)     4249 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/geos/prototypes/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      795 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/geos/prototypes/coordseq.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      474 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/geos/prototypes/errcheck.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      792 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/geos/prototypes/geom.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2975 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/geos/prototypes/io.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      232 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/geos/prototypes/misc.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      553 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/geos/prototypes/predicates.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      434 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/geos/prototypes/prepared.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      496 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/geos/prototypes/threadsafe.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      609 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/geos/prototypes/topology.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1418 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/measure.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      252 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/ptr.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.706592 django-stubs-4.2.0/django-stubs/contrib/gis/serializers/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/serializers/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      493 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/serializers/geojson.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      244 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/shortcuts.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.706592 django-stubs-4.2.0/django-stubs/contrib/gis/sitemaps/
--rw-r--r--   0 marti     (1000) marti      (121)      138 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/sitemaps/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      328 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/sitemaps/kml.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      352 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/sitemaps/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.706592 django-stubs-4.2.0/django-stubs/contrib/gis/utils/
--rw-r--r--   0 marti     (1000) marti      (121)      436 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/utils/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2526 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/utils/layermapping.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      153 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/utils/ogrinfo.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      320 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/utils/ogrinspect.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      199 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/utils/srs.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      202 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/gis/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.709926 django-stubs-4.2.0/django-stubs/contrib/humanize/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/humanize/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/humanize/apps.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.709926 django-stubs-4.2.0/django-stubs/contrib/humanize/templatetags/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/humanize/templatetags/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      859 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/humanize/templatetags/humanize.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.709926 django-stubs-4.2.0/django-stubs/contrib/messages/
--rw-r--r--   0 marti     (1000) marti      (121)      715 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/messages/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1294 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/messages/api.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/messages/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      120 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/messages/constants.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      225 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/messages/context_processors.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      349 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/messages/middleware.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.709926 django-stubs-4.2.0/django-stubs/contrib/messages/storage/
--rw-r--r--   0 marti     (1000) marti      (121)      192 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/messages/storage/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      906 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/messages/storage/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      463 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/messages/storage/cookie.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      228 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/messages/storage/fallback.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      468 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/messages/storage/session.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       44 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/messages/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      347 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/messages/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.713259 django-stubs-4.2.0/django-stubs/contrib/postgres/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/postgres/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.713259 django-stubs-4.2.0/django-stubs/contrib/postgres/aggregates/
--rw-r--r--   0 marti     (1000) marti      (121)      826 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/postgres/aggregates/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      357 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/postgres/aggregates/general.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       29 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/postgres/aggregates/mixins.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      470 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/postgres/aggregates/statistics.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      270 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/postgres/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      846 2023-04-27 12:45:58.000000 django-stubs-4.2.0/django-stubs/contrib/postgres/constraints.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.716592 django-stubs-4.2.0/django-stubs/contrib/postgres/fields/
--rw-r--r--   0 marti     (1000) marti      (121)      759 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/postgres/fields/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1897 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/postgres/fields/array.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      216 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/postgres/fields/citext.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      573 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/postgres/fields/hstore.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      376 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/postgres/fields/jsonb.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3038 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/postgres/fields/ranges.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      106 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/postgres/fields/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.716592 django-stubs-4.2.0/django-stubs/contrib/postgres/forms/
--rw-r--r--   0 marti     (1000) marti      (121)       86 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/postgres/forms/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2340 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/postgres/forms/array.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      462 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/postgres/forms/hstore.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1486 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/postgres/forms/ranges.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       95 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/postgres/functions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3972 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/postgres/indexes.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      532 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/postgres/lookups.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2055 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/postgres/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3627 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/postgres/search.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      152 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/postgres/serializers.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      230 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/postgres/signals.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      177 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/postgres/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      635 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/postgres/validators.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.716592 django-stubs-4.2.0/django-stubs/contrib/redirects/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/redirects/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      185 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/redirects/admin.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      129 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/redirects/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      379 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/redirects/middleware.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.716592 django-stubs-4.2.0/django-stubs/contrib/redirects/migrations/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/redirects/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      150 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/redirects/models.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.716592 django-stubs-4.2.0/django-stubs/contrib/sessions/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/sessions/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/sessions/apps.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.719926 django-stubs-4.2.0/django-stubs/contrib/sessions/backends/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/sessions/backends/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1770 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/sessions/backends/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      280 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/sessions/backends/cache.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      286 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/sessions/backends/cached_db.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      547 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/sessions/backends/db.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      239 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/sessions/backends/file.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      100 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/sessions/backends/signed_cookies.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      676 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/sessions/base_session.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      156 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/sessions/exceptions.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.719926 django-stubs-4.2.0/django-stubs/contrib/sessions/management/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/sessions/management/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.719926 django-stubs-4.2.0/django-stubs/contrib/sessions/management/commands/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/sessions/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       85 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/sessions/management/commands/clearsessions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      447 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/sessions/middleware.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.719926 django-stubs-4.2.0/django-stubs/contrib/sessions/migrations/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/sessions/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      243 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/sessions/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      337 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/sessions/serializers.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.719926 django-stubs-4.2.0/django-stubs/contrib/sitemaps/
--rw-r--r--   0 marti     (1000) marti      (121)     1697 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/sitemaps/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/sitemaps/apps.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.719926 django-stubs-4.2.0/django-stubs/contrib/sitemaps/management/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/sitemaps/management/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.719926 django-stubs-4.2.0/django-stubs/contrib/sitemaps/management/commands/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/sitemaps/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       85 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/sitemaps/management/commands/ping_google.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      710 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/sitemaps/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.723259 django-stubs-4.2.0/django-stubs/contrib/sites/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/sites/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      138 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/sites/admin.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       69 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/sites/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      288 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/sites/management.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      247 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/sites/managers.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      209 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/sites/middleware.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.723259 django-stubs-4.2.0/django-stubs/contrib/sites/migrations/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/sites/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      585 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/sites/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      292 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/sites/requests.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      221 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/sites/shortcuts.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.723259 django-stubs-4.2.0/django-stubs/contrib/staticfiles/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/staticfiles/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      120 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/staticfiles/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      263 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/staticfiles/checks.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2742 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/staticfiles/finders.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1674 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/staticfiles/handlers.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.723259 django-stubs-4.2.0/django-stubs/contrib/staticfiles/management/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/staticfiles/management/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.723259 django-stubs-4.2.0/django-stubs/contrib/staticfiles/management/commands/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/staticfiles/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1055 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/staticfiles/management/commands/collectstatic.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       87 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/staticfiles/management/commands/findstatic.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      120 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/staticfiles/management/commands/runserver.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2152 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/staticfiles/storage.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      100 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/staticfiles/testing.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      152 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/staticfiles/urls.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      345 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/staticfiles/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      216 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/staticfiles/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.723259 django-stubs-4.2.0/django-stubs/contrib/syndication/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/syndication/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      131 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/contrib/syndication/apps.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1924 2023-04-27 12:45:58.000000 django-stubs-4.2.0/django-stubs/contrib/syndication/views.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.726592 django-stubs-4.2.0/django-stubs/core/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       98 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/asgi.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.726592 django-stubs-4.2.0/django-stubs/core/cache/
--rw-r--r--   0 marti     (1000) marti      (121)      624 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/cache/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.726592 django-stubs-4.2.0/django-stubs/core/cache/backends/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/cache/backends/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4052 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/cache/backends/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      593 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/cache/backends/db.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      182 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/cache/backends/dummy.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      204 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/cache/backends/filebased.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      180 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/cache/backends/locmem.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      782 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/cache/backends/memcached.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      198 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/cache/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.729926 django-stubs-4.2.0/django-stubs/core/checks/
--rw-r--r--   0 marti     (1000) marti      (121)      652 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/checks/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      265 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/checks/async_checks.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      529 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/checks/caches.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.729926 django-stubs-4.2.0/django-stubs/core/checks/compatibility/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/checks/compatibility/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      229 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/checks/database.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1084 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/checks/messages.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      389 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/checks/model_checks.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1799 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/checks/registry.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.729926 django-stubs-4.2.0/django-stubs/core/checks/security/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/checks/security/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1847 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/checks/security/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      399 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/checks/security/csrf.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      577 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/checks/security/sessions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      407 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/checks/templates.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      625 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/checks/translation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      706 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/checks/urls.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1912 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/exceptions.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.733259 django-stubs-4.2.0/django-stubs/core/files/
--rw-r--r--   0 marti     (1000) marti      (121)       68 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/files/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1606 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/files/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      359 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/files/images.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      296 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/files/locks.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      130 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/files/move.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1872 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/files/storage.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      100 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/files/temp.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1459 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/files/uploadedfile.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3017 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/files/uploadhandler.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      736 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/files/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.733259 django-stubs-4.2.0/django-stubs/core/handlers/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/handlers/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2043 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/handlers/asgi.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1220 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/handlers/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      770 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/handlers/exception.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1405 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/handlers/wsgi.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.733259 django-stubs-4.2.0/django-stubs/core/mail/
--rw-r--r--   0 marti     (1000) marti      (121)     1707 2023-04-27 12:45:58.000000 django-stubs-4.2.0/django-stubs/core/mail/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.733259 django-stubs-4.2.0/django-stubs/core/mail/backends/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/mail/backends/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      668 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/mail/backends/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      189 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/mail/backends/console.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      103 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/mail/backends/dummy.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/mail/backends/filebased.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      103 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/mail/backends/locmem.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      395 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/mail/backends/smtp.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5032 2023-04-27 12:45:58.000000 django-stubs-4.2.0/django-stubs/core/mail/message.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       95 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/mail/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.733259 django-stubs-4.2.0/django-stubs/core/management/
--rw-r--r--   0 marti     (1000) marti      (121)      829 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/management/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3646 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/management/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1099 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/management/color.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.739925 django-stubs-4.2.0/django-stubs/core/management/commands/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      179 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/management/commands/check.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      430 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/management/commands/compilemessages.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      284 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/management/commands/createcachetable.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       85 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/management/commands/dbshell.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      519 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/management/commands/diffsettings.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      123 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/management/commands/dumpdata.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      177 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/management/commands/flush.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      789 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/management/commands/inspectdb.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1140 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/management/commands/loaddata.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1227 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/management/commands/makemessages.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      467 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/management/commands/makemigrations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      643 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/management/commands/migrate.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      515 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/management/commands/runserver.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      111 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/management/commands/sendtestemail.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      268 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/management/commands/shell.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      371 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/management/commands/showmigrations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      110 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/management/commands/sqlflush.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      203 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/management/commands/sqlmigrate.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       83 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/management/commands/sqlsequencereset.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      330 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/management/commands/squashmigrations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      124 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/management/commands/startapp.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      124 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/management/commands/startproject.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      232 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/management/commands/test.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       85 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/management/commands/testserver.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      488 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/management/sql.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      964 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/management/templates.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      850 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/management/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2313 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/paginator.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.739925 django-stubs-4.2.0/django-stubs/core/serializers/
--rw-r--r--   0 marti     (1000) marti      (121)     1437 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/serializers/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3192 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/serializers/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      577 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/serializers/json.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      398 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/serializers/jsonl.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      490 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/serializers/python.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      831 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/serializers/pyyaml.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2320 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/serializers/xml_serializer.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.739925 django-stubs-4.2.0/django-stubs/core/servers/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/servers/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1165 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/servers/basehttp.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      139 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/signals.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1846 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/signing.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4397 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/validators.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       98 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/core/wsgi.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.739925 django-stubs-4.2.0/django-stubs/db/
--rw-r--r--   0 marti     (1000) marti      (121)     1047 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.739925 django-stubs-4.2.0/django-stubs/db/backends/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.743259 django-stubs-4.2.0/django-stubs/db/backends/base/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/base/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5274 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/base/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      555 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/base/client.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1132 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/base/creation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5147 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/base/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1826 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/base/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     6660 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/base/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3557 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/base/schema.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      389 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/base/validation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3134 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/ddl_references.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.743259 django-stubs-4.2.0/django-stubs/db/backends/dummy/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/dummy/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      949 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/dummy/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      176 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/dummy/features.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.746592 django-stubs-4.2.0/django-stubs/db/backends/mysql/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/mysql/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2522 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/mysql/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      483 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/mysql/client.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      734 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/mysql/compiler.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      255 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/mysql/creation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3434 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/mysql/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1159 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/mysql/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2760 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/mysql/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      902 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/mysql/schema.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      354 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/mysql/validation.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.746592 django-stubs-4.2.0/django-stubs/db/backends/oracle/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/oracle/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2711 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/oracle/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      546 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/oracle/client.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      373 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/oracle/creation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1923 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/oracle/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      398 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/oracle/functions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1004 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/oracle/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3888 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/oracle/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      924 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/oracle/schema.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      511 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/oracle/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      308 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/oracle/validation.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.746592 django-stubs-4.2.0/django-stubs/db/backends/postgresql/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/postgresql/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1382 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/postgresql/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      524 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/postgresql/client.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      208 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/postgresql/creation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2197 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/postgresql/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      820 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/postgresql/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      216 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/postgresql/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      809 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/postgresql/schema.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       63 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/signals.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.749925 django-stubs-4.2.0/django-stubs/db/backends/sqlite3/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/sqlite3/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1052 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/sqlite3/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      441 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/sqlite3/client.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      322 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/sqlite3/creation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      205 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/sqlite3/features.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      432 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/sqlite3/introspection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      125 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/sqlite3/operations.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      215 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/sqlite3/schema.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2876 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/backends/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.749925 django-stubs-4.2.0/django-stubs/db/migrations/
--rw-r--r--   0 marti     (1000) marti      (121)      265 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2830 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/migrations/autodetector.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      664 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/migrations/exceptions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1739 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/migrations/executor.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2420 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/migrations/graph.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1960 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/migrations/loader.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1111 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/migrations/migration.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.753259 django-stubs-4.2.0/django-stubs/db/migrations/operations/
--rw-r--r--   0 marti     (1000) marti      (121)     1090 2023-04-27 12:45:58.000000 django-stubs-4.2.0/django-stubs/db/migrations/operations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1426 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/migrations/operations/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1171 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/migrations/operations/fields.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4451 2023-04-27 12:45:58.000000 django-stubs-4.2.0/django-stubs/db/migrations/operations/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1977 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/migrations/operations/special.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      985 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/migrations/operations/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      290 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/migrations/optimizer.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1109 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/migrations/questioner.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      755 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/migrations/recorder.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1835 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/migrations/serializer.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2939 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/migrations/state.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      195 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/migrations/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1235 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/migrations/writer.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.756592 django-stubs-4.2.0/django-stubs/db/models/
--rw-r--r--   0 marti     (1000) marti      (121)     5016 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/models/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      684 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/models/aggregates.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3728 2023-04-27 12:45:58.000000 django-stubs-4.2.0/django-stubs/db/models/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       16 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/models/constants.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2255 2023-04-27 12:45:58.000000 django-stubs-4.2.0/django-stubs/db/models/constraints.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3487 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/models/deletion.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1008 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/models/enums.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     9496 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/models/expressions.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.756592 django-stubs-4.2.0/django-stubs/db/models/fields/
--rw-r--r--   0 marti     (1000) marti      (121)    20451 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/models/fields/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3963 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/models/fields/files.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3142 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/models/fields/json.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      515 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/models/fields/mixins.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      161 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/models/fields/proxy.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    10535 2023-04-27 12:45:58.000000 django-stubs-4.2.0/django-stubs/db/models/fields/related.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3546 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/models/fields/related_descriptors.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1393 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/models/fields/related_lookups.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4605 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/models/fields/reverse_related.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.756592 django-stubs-4.2.0/django-stubs/db/models/functions/
--rw-r--r--   0 marti     (1000) marti      (121)     3378 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/models/functions/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      547 2023-04-27 12:45:58.000000 django-stubs-4.2.0/django-stubs/db/models/functions/comparison.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1343 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/models/functions/datetime.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1222 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/models/functions/math.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      100 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/models/functions/mixins.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4623 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/models/functions/text.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      918 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/models/functions/window.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2228 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/models/indexes.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5904 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/models/lookups.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     8468 2023-04-27 12:45:58.000000 django-stubs-4.2.0/django-stubs/db/models/manager.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5334 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/models/options.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    10808 2023-04-27 12:45:58.000000 django-stubs-4.2.0/django-stubs/db/models/query.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3326 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/models/query_utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      911 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/models/signals.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.759925 django-stubs-4.2.0/django-stubs/db/models/sql/
--rw-r--r--   0 marti     (1000) marti      (121)      284 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/models/sql/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     6464 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/models/sql/compiler.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      344 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/models/sql/constants.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1791 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/models/sql/datastructures.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     9565 2023-04-27 12:45:58.000000 django-stubs-4.2.0/django-stubs/db/models/sql/query.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1663 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/models/sql/subqueries.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2075 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/models/sql/where.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      473 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/models/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2146 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/transaction.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2061 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/db/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.759925 django-stubs-4.2.0/django-stubs/dispatch/
--rw-r--r--   0 marti     (1000) marti      (121)      116 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/dispatch/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      930 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/dispatch/dispatcher.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.759925 django-stubs-4.2.0/django-stubs/forms/
--rw-r--r--   0 marti     (1000) marti      (121)     4083 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/forms/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2874 2023-04-27 12:45:58.000000 django-stubs-4.2.0/django-stubs/forms/boundfield.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    20436 2023-04-27 12:45:58.000000 django-stubs-4.2.0/django-stubs/forms/fields.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3196 2023-04-27 12:45:58.000000 django-stubs-4.2.0/django-stubs/forms/forms.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3777 2023-04-27 12:45:58.000000 django-stubs-4.2.0/django-stubs/forms/formsets.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    12234 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/forms/models.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1125 2023-04-27 12:45:58.000000 django-stubs-4.2.0/django-stubs/forms/renderers.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2337 2023-04-27 12:45:58.000000 django-stubs-4.2.0/django-stubs/forms/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    10456 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/forms/widgets.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.763259 django-stubs-4.2.0/django-stubs/http/
--rw-r--r--   0 marti     (1000) marti      (121)     1332 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/http/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       96 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/http/cookie.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2076 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/http/multipartparser.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     8346 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/http/request.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5624 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/http/response.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.763259 django-stubs-4.2.0/django-stubs/middleware/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/middleware/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1062 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/middleware/cache.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      387 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/middleware/clickjacking.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      968 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/middleware/common.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1098 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/middleware/csrf.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      339 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/middleware/gzip.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      369 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/middleware/http.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      417 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/middleware/locale.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      645 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/middleware/security.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1543 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/shortcuts.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.766592 django-stubs-4.2.0/django-stubs/template/
--rw-r--r--   0 marti     (1000) marti      (121)      756 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/template/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.766592 django-stubs-4.2.0/django-stubs/template/backends/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/template/backends/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      925 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/template/backends/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1062 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/template/backends/django.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      432 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/template/backends/dummy.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      575 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/template/backends/jinja2.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      215 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/template/backends/utils.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     5673 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/template/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3410 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/template/context.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      631 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/template/context_processors.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3483 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/template/defaultfilters.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     6912 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/template/defaulttags.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2158 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/template/engine.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      511 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/template/exceptions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3244 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/template/library.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      684 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/template/loader.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2266 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/template/loader_tags.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.766592 django-stubs-4.2.0/django-stubs/template/loaders/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/template/loaders/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       88 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/template/loaders/app_directories.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      488 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/template/loaders/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      554 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/template/loaders/cached.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      518 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/template/loaders/filesystem.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      323 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/template/loaders/locmem.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2564 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/template/response.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1246 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/template/smartif.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      589 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/template/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.769925 django-stubs-4.2.0/django-stubs/templatetags/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/templatetags/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      629 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/templatetags/cache.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3492 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/templatetags/i18n.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      410 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/templatetags/l10n.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1123 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/templatetags/static.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1076 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/templatetags/tz.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.769925 django-stubs-4.2.0/django-stubs/test/
--rw-r--r--   0 marti     (1000) marti      (121)      848 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/test/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     7476 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/test/client.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1148 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/test/html.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     6619 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/test/runner.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      539 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/test/selenium.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      905 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/test/signals.pyi
--rw-r--r--   0 marti     (1000) marti      (121)    10511 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/test/testcases.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     6313 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/test/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.769925 django-stubs-4.2.0/django-stubs/urls/
--rw-r--r--   0 marti     (1000) marti      (121)     1576 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/urls/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      886 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/urls/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1349 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/urls/conf.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      778 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/urls/converters.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      102 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/urls/exceptions.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4497 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/urls/resolvers.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      157 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/urls/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.776592 django-stubs-4.2.0/django-stubs/utils/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      286 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/_os.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1485 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/archive.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      235 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/asyncio.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2830 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/autoreload.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      591 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/baseconv.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1287 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/cache.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1173 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/connection.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      557 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/crypto.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4498 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/datastructures.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2062 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/dateformat.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      525 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/dateparse.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      156 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/dates.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      386 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/datetime_safe.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      325 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/deconstruct.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1195 2023-04-27 12:45:58.000000 django-stubs-4.2.0/django-stubs/utils/decorators.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1361 2023-04-27 12:45:58.000000 django-stubs-4.2.0/django-stubs/utils/deprecation.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      198 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/duration.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3255 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/encoding.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2622 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/feedgenerator.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1804 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/formats.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4146 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/functional.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       66 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/hashable.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1399 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/html.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1766 2023-04-27 12:45:58.000000 django-stubs-4.2.0/django-stubs/utils/http.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      483 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/inspect.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      175 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/ipv6.pyi
--rw-r--r--   0 marti     (1000) marti      (121)       61 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/itercompat.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      714 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/jslex.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1691 2023-04-27 12:45:58.000000 django-stubs-4.2.0/django-stubs/utils/log.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      242 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/lorem_ipsum.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      247 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/module_loading.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      319 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/numberformat.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      917 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/regex_helper.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      616 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/safestring.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      557 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/termcolors.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1969 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/text.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      387 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/timesince.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2011 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/timezone.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      309 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/topological_sort.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.779925 django-stubs-4.2.0/django-stubs/utils/translation/
--rw-r--r--   0 marti     (1000) marti      (121)     2914 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/translation/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      286 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/translation/reloader.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      298 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/translation/template.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      825 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/translation/trans_null.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2929 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/translation/trans_real.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      800 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/tree.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      499 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/version.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      379 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/utils/xmlutils.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.779925 django-stubs-4.2.0/django-stubs/views/
--rw-r--r--   0 marti     (1000) marti      (121)       39 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/views/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      274 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/views/csrf.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2691 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/views/debug.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.783259 django-stubs-4.2.0/django-stubs/views/decorators/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/views/decorators/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      321 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/views/decorators/cache.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      274 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/views/decorators/clickjacking.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      162 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/views/decorators/common.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      427 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/views/decorators/csrf.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      184 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/views/decorators/debug.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      146 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/views/decorators/gzip.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      614 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/views/decorators/http.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      218 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/views/decorators/vary.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      782 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/views/defaults.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.783259 django-stubs-4.2.0/django-stubs/views/generic/
--rw-r--r--   0 marti     (1000) marti      (121)      797 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/views/generic/__init__.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     2272 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/views/generic/base.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     4525 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/views/generic/dates.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1109 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/views/generic/detail.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     3422 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/views/generic/edit.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1818 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/views/generic/list.pyi
--rw-r--r--   0 marti     (1000) marti      (121)     1035 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/views/i18n.pyi
--rw-r--r--   0 marti     (1000) marti      (121)      482 2023-03-15 16:53:32.000000 django-stubs-4.2.0/django-stubs/views/static.pyi
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.783259 django-stubs-4.2.0/django_stubs.egg-info/
--rw-r--r--   0 marti     (1000) marti      (121)    14046 2023-04-27 12:47:56.000000 django-stubs-4.2.0/django_stubs.egg-info/PKG-INFO
--rw-r--r--   0 marti     (1000) marti      (121)    29999 2023-04-27 12:47:56.000000 django-stubs-4.2.0/django_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 marti     (1000) marti      (121)        1 2023-04-27 12:47:56.000000 django-stubs-4.2.0/django_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 marti     (1000) marti      (121)      155 2023-04-27 12:47:56.000000 django-stubs-4.2.0/django_stubs.egg-info/requires.txt
--rw-r--r--   0 marti     (1000) marti      (121)       32 2023-04-27 12:47:56.000000 django-stubs-4.2.0/django_stubs.egg-info/top_level.txt
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.783259 django-stubs-4.2.0/mypy_django_plugin/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/mypy_django_plugin/__init__.py
--rw-r--r--   0 marti     (1000) marti      (121)     3484 2023-04-27 12:45:58.000000 django-stubs-4.2.0/mypy_django_plugin/config.py
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.783259 django-stubs-4.2.0/mypy_django_plugin/django/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/mypy_django_plugin/django/__init__.py
--rw-r--r--   0 marti     (1000) marti      (121)    20596 2023-04-27 12:45:58.000000 django-stubs-4.2.0/mypy_django_plugin/django/context.py
--rw-r--r--   0 marti     (1000) marti      (121)      227 2023-03-15 16:53:32.000000 django-stubs-4.2.0/mypy_django_plugin/errorcodes.py
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.783259 django-stubs-4.2.0/mypy_django_plugin/lib/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/mypy_django_plugin/lib/__init__.py
--rw-r--r--   0 marti     (1000) marti      (121)     2289 2023-04-27 12:45:58.000000 django-stubs-4.2.0/mypy_django_plugin/lib/fullnames.py
--rw-r--r--   0 marti     (1000) marti      (121)    13031 2023-04-27 12:45:58.000000 django-stubs-4.2.0/mypy_django_plugin/lib/helpers.py
--rw-r--r--   0 marti     (1000) marti      (121)    15645 2023-03-15 16:53:32.000000 django-stubs-4.2.0/mypy_django_plugin/main.py
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/mypy_django_plugin/py.typed
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.786592 django-stubs-4.2.0/mypy_django_plugin/transformers/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.0/mypy_django_plugin/transformers/__init__.py
--rw-r--r--   0 marti     (1000) marti      (121)     9647 2023-03-15 16:53:32.000000 django-stubs-4.2.0/mypy_django_plugin/transformers/fields.py
--rw-r--r--   0 marti     (1000) marti      (121)     1809 2023-03-15 16:53:32.000000 django-stubs-4.2.0/mypy_django_plugin/transformers/forms.py
--rw-r--r--   0 marti     (1000) marti      (121)     1335 2023-03-15 16:53:32.000000 django-stubs-4.2.0/mypy_django_plugin/transformers/functional.py
--rw-r--r--   0 marti     (1000) marti      (121)     3104 2023-03-15 16:53:32.000000 django-stubs-4.2.0/mypy_django_plugin/transformers/init_create.py
--rw-r--r--   0 marti     (1000) marti      (121)    20908 2023-03-15 16:53:32.000000 django-stubs-4.2.0/mypy_django_plugin/transformers/managers.py
--rw-r--r--   0 marti     (1000) marti      (121)     1960 2023-03-15 16:53:32.000000 django-stubs-4.2.0/mypy_django_plugin/transformers/meta.py
--rw-r--r--   0 marti     (1000) marti      (121)    32471 2023-04-27 12:45:58.000000 django-stubs-4.2.0/mypy_django_plugin/transformers/models.py
--rw-r--r--   0 marti     (1000) marti      (121)     2659 2023-03-15 16:53:32.000000 django-stubs-4.2.0/mypy_django_plugin/transformers/orm_lookups.py
--rw-r--r--   0 marti     (1000) marti      (121)    13195 2023-04-27 12:45:58.000000 django-stubs-4.2.0/mypy_django_plugin/transformers/querysets.py
--rw-r--r--   0 marti     (1000) marti      (121)     2070 2023-03-15 16:53:32.000000 django-stubs-4.2.0/mypy_django_plugin/transformers/request.py
--rw-r--r--   0 marti     (1000) marti      (121)     2003 2023-03-15 16:53:32.000000 django-stubs-4.2.0/mypy_django_plugin/transformers/settings.py
--rw-r--r--   0 marti     (1000) marti      (121)      227 2023-03-15 16:53:32.000000 django-stubs-4.2.0/pyproject.toml
--rw-r--r--   0 marti     (1000) marti      (121)      272 2023-04-27 12:47:56.786592 django-stubs-4.2.0/setup.cfg
--rw-r--r--   0 marti     (1000) marti      (121)     2293 2023-04-27 12:45:58.000000 django-stubs-4.2.0/setup.py
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:56.786592 django-stubs-4.2.0/tests/
--rw-r--r--   0 marti     (1000) marti      (121)     4735 2023-03-15 16:53:32.000000 django-stubs-4.2.0/tests/test_error_handling.py
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.264431 django-stubs-4.2.1/
+-rw-r--r--   0 marti     (1000) marti      (121)     1075 2023-06-02 14:08:54.000000 django-stubs-4.2.1/LICENSE.md
+-rw-r--r--   0 marti     (1000) marti      (121)    13907 2023-06-02 14:11:31.264431 django-stubs-4.2.1/PKG-INFO
+-rw-r--r--   0 marti     (1000) marti      (121)    12832 2023-06-02 14:08:54.000000 django-stubs-4.2.1/README.md
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.141099 django-stubs-4.2.1/django-stubs/
+-rw-r--r--   0 marti     (1000) marti      (121)      157 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.141099 django-stubs-4.2.1/django-stubs/apps/
+-rw-r--r--   0 marti     (1000) marti      (121)       78 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/apps/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      855 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/apps/config.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1963 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/apps/registry.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.141099 django-stubs-4.2.1/django-stubs/conf/
+-rw-r--r--   0 marti     (1000) marti      (121)     1453 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/conf/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)    16655 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/conf/global_settings.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.141099 django-stubs-4.2.1/django-stubs/conf/locale/
+-rw-r--r--   0 marti     (1000) marti      (121)       50 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/conf/locale/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.144432 django-stubs-4.2.1/django-stubs/conf/urls/
+-rw-r--r--   0 marti     (1000) marti      (121)     1073 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/conf/urls/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      231 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/conf/urls/i18n.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      193 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/conf/urls/static.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.144432 django-stubs-4.2.1/django-stubs/contrib/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.147765 django-stubs-4.2.1/django-stubs/contrib/admin/
+-rw-r--r--   0 marti     (1000) marti      (121)     1157 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      313 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/actions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      136 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1075 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/checks.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2208 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/decorators.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      175 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/exceptions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3887 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/filters.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      237 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/forms.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     5562 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/helpers.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.147765 django-stubs-4.2.1/django-stubs/contrib/admin/migrations/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/migrations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1032 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)    16126 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/options.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4087 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/contrib/admin/sites.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.147765 django-stubs-4.2.1/django-stubs/contrib/admin/templatetags/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/templatetags/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1981 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/templatetags/admin_list.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      690 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/templatetags/admin_modify.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      503 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/templatetags/admin_urls.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      605 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/templatetags/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      441 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/templatetags/log.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1629 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/tests.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3665 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/contrib/admin/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.147765 django-stubs-4.2.1/django-stubs/contrib/admin/views/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/views/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      374 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/views/autocomplete.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      383 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/views/decorators.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3104 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admin/views/main.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     5670 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/contrib/admin/widgets.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.147765 django-stubs-4.2.1/django-stubs/contrib/admindocs/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admindocs/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      129 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admindocs/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      478 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admindocs/middleware.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       60 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admindocs/urls.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      840 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admindocs/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1018 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/admindocs/views.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.157765 django-stubs-4.2.1/django-stubs/contrib/auth/
+-rw-r--r--   0 marti     (1000) marti      (121)     1272 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      496 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/admin.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       68 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1891 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/backends.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1532 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/base_user.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      398 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/checks.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      662 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/context_processors.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      934 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/decorators.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3944 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/contrib/auth/forms.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.157765 django-stubs-4.2.1/django-stubs/contrib/auth/handlers/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/handlers/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      198 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/handlers/modwsgi.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1962 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/hashers.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.157765 django-stubs-4.2.1/django-stubs/contrib/auth/management/
+-rw-r--r--   0 marti     (1000) marti      (121)      405 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/management/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.157765 django-stubs-4.2.1/django-stubs/contrib/auth/management/commands/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/management/commands/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      125 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/management/commands/changepassword.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      208 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/management/commands/createsuperuser.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      739 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/middleware.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.157765 django-stubs-4.2.1/django-stubs/contrib/auth/migrations/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/migrations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1228 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/mixins.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4613 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/contrib/auth/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2081 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/password_validation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      120 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/signals.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      735 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/contrib/auth/tokens.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       60 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/urls.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      153 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/validators.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2387 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/auth/views.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.157765 django-stubs-4.2.1/django-stubs/contrib/contenttypes/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/contenttypes/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      655 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/contenttypes/admin.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       76 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/contenttypes/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      414 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/contenttypes/checks.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3850 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/contenttypes/fields.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1420 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/contenttypes/forms.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.157765 django-stubs-4.2.1/django-stubs/contrib/contenttypes/management/
+-rw-r--r--   0 marti     (1000) marti      (121)     1297 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/contenttypes/management/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.157765 django-stubs-4.2.1/django-stubs/contrib/contenttypes/management/commands/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/contenttypes/management/commands/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      467 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/contenttypes/management/commands/remove_stale_contenttypes.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.157765 django-stubs-4.2.1/django-stubs/contrib/contenttypes/migrations/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/contenttypes/migrations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1020 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/contenttypes/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      213 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/contenttypes/views.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.161098 django-stubs-4.2.1/django-stubs/contrib/flatpages/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/flatpages/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      196 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/flatpages/admin.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      129 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/flatpages/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      136 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/flatpages/forms.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      293 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/flatpages/middleware.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.161098 django-stubs-4.2.1/django-stubs/contrib/flatpages/migrations/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/flatpages/migrations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      402 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/flatpages/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       81 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/flatpages/sitemaps.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.161098 django-stubs-4.2.1/django-stubs/contrib/flatpages/templatetags/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/flatpages/templatetags/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      484 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/flatpages/templatetags/flatpages.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       60 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/flatpages/urls.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      309 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/flatpages/views.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.161098 django-stubs-4.2.1/django-stubs/contrib/gis/
+-rw-r--r--   0 marti     (1000) marti      (121)       24 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.164432 django-stubs-4.2.1/django-stubs/contrib/gis/admin/
+-rw-r--r--   0 marti     (1000) marti      (121)      872 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/admin/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1174 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/admin/options.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      272 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/admin/widgets.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       67 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/apps.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.164432 django-stubs-4.2.1/django-stubs/contrib/gis/db/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.164432 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.164432 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/base/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/base/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      200 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/base/adapter.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1443 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/base/features.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      836 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/base/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1348 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/base/operations.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.164432 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/mysql/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/mysql/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      251 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/mysql/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      781 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/mysql/features.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      333 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/mysql/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1134 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/mysql/operations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      699 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/mysql/schema.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.167765 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/oracle/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/oracle/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      226 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/oracle/adapter.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      254 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/oracle/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      444 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/oracle/features.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      287 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/oracle/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      729 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/oracle/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1440 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/oracle/operations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      826 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/oracle/schema.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.167765 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/postgis/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/postgis/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      399 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/postgis/adapter.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      351 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/postgis/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      189 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/postgis/const.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      407 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/postgis/features.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      360 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/postgis/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      798 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/postgis/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2218 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/postgis/operations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      247 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/postgis/pgraster.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      340 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/postgis/schema.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.167765 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/spatialite/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/spatialite/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      182 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/spatialite/adapter.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      477 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/spatialite/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      127 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/spatialite/client.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      358 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/spatialite/features.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      451 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/spatialite/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      808 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/spatialite/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1286 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/spatialite/operations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1103 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/spatialite/schema.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      656 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.171098 django-stubs-4.2.1/django-stubs/contrib/gis/db/models/
+-rw-r--r--   0 marti     (1000) marti      (121)      847 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/models/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      800 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/models/aggregates.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     6077 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/models/fields.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     6016 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/models/functions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2955 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/models/lookups.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      345 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/models/proxy.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.171098 django-stubs-4.2.1/django-stubs/contrib/gis/db/models/sql/
+-rw-r--r--   0 marti     (1000) marti      (121)      166 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/models/sql/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      829 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/db/models/sql/conversion.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      866 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/feeds.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.171098 django-stubs-4.2.1/django-stubs/contrib/gis/forms/
+-rw-r--r--   0 marti     (1000) marti      (121)      642 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/forms/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      840 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/forms/fields.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      951 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/forms/widgets.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.171098 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/
+-rw-r--r--   0 marti     (1000) marti      (121)     1070 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      137 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      574 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/datasource.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      324 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/driver.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      688 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/envelope.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      200 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/error.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      947 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/feature.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1460 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/field.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4844 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/geometries.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      304 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/geomtype.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1721 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/layer.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      510 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/libgdal.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.174432 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/prototypes/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/prototypes/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1036 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/prototypes/ds.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      961 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/prototypes/errcheck.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1077 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/prototypes/generation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      970 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/prototypes/geom.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1053 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/prototypes/raster.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      614 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/prototypes/srs.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.174432 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/raster/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/raster/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1594 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/raster/band.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      225 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/raster/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      252 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/raster/const.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2180 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/raster/source.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2191 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/gdal/srs.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.174432 django-stubs-4.2.1/django-stubs/contrib/gis/geoip2/
+-rw-r--r--   0 marti     (1000) marti      (121)      106 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geoip2/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1202 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geoip2/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       99 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geoip2/resources.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       97 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geometry.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.177765 django-stubs-4.2.1/django-stubs/contrib/gis/geos/
+-rw-r--r--   0 marti     (1000) marti      (121)      883 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      185 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      604 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/collections.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1250 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/coordseq.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       36 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/error.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      276 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/factory.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     5258 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/geometry.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      491 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/io.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      896 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/libgeos.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      766 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/linestring.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1148 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/mutable_list.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      816 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/point.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      713 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/polygon.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      737 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/prepared.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.177765 django-stubs-4.2.1/django-stubs/contrib/gis/geos/prototypes/
+-rw-r--r--   0 marti     (1000) marti      (121)     4249 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/prototypes/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      795 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/prototypes/coordseq.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      474 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/prototypes/errcheck.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      792 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/prototypes/geom.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2975 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/prototypes/io.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      232 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/prototypes/misc.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      553 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/prototypes/predicates.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      434 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/prototypes/prepared.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      496 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/prototypes/threadsafe.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      609 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/geos/prototypes/topology.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1418 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/measure.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      252 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/ptr.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.177765 django-stubs-4.2.1/django-stubs/contrib/gis/serializers/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/serializers/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      493 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/serializers/geojson.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      244 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/shortcuts.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.181098 django-stubs-4.2.1/django-stubs/contrib/gis/sitemaps/
+-rw-r--r--   0 marti     (1000) marti      (121)      138 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/sitemaps/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      328 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/sitemaps/kml.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      352 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/sitemaps/views.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.181098 django-stubs-4.2.1/django-stubs/contrib/gis/utils/
+-rw-r--r--   0 marti     (1000) marti      (121)      436 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/utils/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2526 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/utils/layermapping.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      153 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/utils/ogrinfo.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      320 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/utils/ogrinspect.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      199 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/utils/srs.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      202 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/gis/views.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.181098 django-stubs-4.2.1/django-stubs/contrib/humanize/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/humanize/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/humanize/apps.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.181098 django-stubs-4.2.1/django-stubs/contrib/humanize/templatetags/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/humanize/templatetags/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      859 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/humanize/templatetags/humanize.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.181098 django-stubs-4.2.1/django-stubs/contrib/messages/
+-rw-r--r--   0 marti     (1000) marti      (121)      715 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/messages/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1294 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/messages/api.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/messages/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      120 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/messages/constants.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      225 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/messages/context_processors.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      349 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/messages/middleware.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.184431 django-stubs-4.2.1/django-stubs/contrib/messages/storage/
+-rw-r--r--   0 marti     (1000) marti      (121)      192 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/messages/storage/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      906 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/messages/storage/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      463 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/messages/storage/cookie.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      228 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/messages/storage/fallback.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      468 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/messages/storage/session.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       44 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/messages/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      347 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/messages/views.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.184431 django-stubs-4.2.1/django-stubs/contrib/postgres/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.184431 django-stubs-4.2.1/django-stubs/contrib/postgres/aggregates/
+-rw-r--r--   0 marti     (1000) marti      (121)      826 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/aggregates/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      357 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/aggregates/general.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       29 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/aggregates/mixins.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      470 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/aggregates/statistics.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      270 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      846 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/constraints.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.187765 django-stubs-4.2.1/django-stubs/contrib/postgres/fields/
+-rw-r--r--   0 marti     (1000) marti      (121)      759 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/fields/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1897 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/fields/array.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      216 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/fields/citext.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      573 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/fields/hstore.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      376 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/fields/jsonb.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3038 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/fields/ranges.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      106 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/fields/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.187765 django-stubs-4.2.1/django-stubs/contrib/postgres/forms/
+-rw-r--r--   0 marti     (1000) marti      (121)       86 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/forms/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2340 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/forms/array.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      462 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/forms/hstore.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      207 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/forms/jsonb.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1486 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/forms/ranges.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       95 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/functions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3972 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/indexes.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      532 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/lookups.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2055 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/operations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3627 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/search.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      152 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/serializers.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      230 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/signals.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      177 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      635 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/postgres/validators.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.187765 django-stubs-4.2.1/django-stubs/contrib/redirects/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/redirects/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      185 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/redirects/admin.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      129 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/redirects/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      379 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/redirects/middleware.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.187765 django-stubs-4.2.1/django-stubs/contrib/redirects/migrations/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/redirects/migrations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      150 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/redirects/models.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.191098 django-stubs-4.2.1/django-stubs/contrib/sessions/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/apps.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.191098 django-stubs-4.2.1/django-stubs/contrib/sessions/backends/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/backends/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1869 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/backends/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      280 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/backends/cache.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      286 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/backends/cached_db.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      508 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/backends/db.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      239 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/backends/file.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      100 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/backends/signed_cookies.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      676 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/base_session.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      156 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/exceptions.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.191098 django-stubs-4.2.1/django-stubs/contrib/sessions/management/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/management/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.191098 django-stubs-4.2.1/django-stubs/contrib/sessions/management/commands/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/management/commands/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       85 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/management/commands/clearsessions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      447 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/middleware.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.191098 django-stubs-4.2.1/django-stubs/contrib/sessions/migrations/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/migrations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      243 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      337 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sessions/serializers.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.191098 django-stubs-4.2.1/django-stubs/contrib/sitemaps/
+-rw-r--r--   0 marti     (1000) marti      (121)     1697 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sitemaps/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sitemaps/apps.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.191098 django-stubs-4.2.1/django-stubs/contrib/sitemaps/management/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sitemaps/management/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.191098 django-stubs-4.2.1/django-stubs/contrib/sitemaps/management/commands/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sitemaps/management/commands/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       85 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sitemaps/management/commands/ping_google.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      710 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sitemaps/views.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.194431 django-stubs-4.2.1/django-stubs/contrib/sites/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sites/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      138 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sites/admin.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       69 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sites/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      288 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sites/management.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      247 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sites/managers.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      209 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sites/middleware.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.194431 django-stubs-4.2.1/django-stubs/contrib/sites/migrations/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sites/migrations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      585 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sites/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      292 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sites/requests.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      221 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/sites/shortcuts.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.194431 django-stubs-4.2.1/django-stubs/contrib/staticfiles/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/staticfiles/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      120 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/staticfiles/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      263 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/staticfiles/checks.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2742 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/staticfiles/finders.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1674 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/staticfiles/handlers.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.194431 django-stubs-4.2.1/django-stubs/contrib/staticfiles/management/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/staticfiles/management/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.194431 django-stubs-4.2.1/django-stubs/contrib/staticfiles/management/commands/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/staticfiles/management/commands/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1055 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/staticfiles/management/commands/collectstatic.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       87 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/staticfiles/management/commands/findstatic.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      120 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/staticfiles/management/commands/runserver.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2152 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/staticfiles/storage.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      100 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/staticfiles/testing.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      152 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/staticfiles/urls.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      345 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/staticfiles/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      216 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/staticfiles/views.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.197765 django-stubs-4.2.1/django-stubs/contrib/syndication/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/syndication/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      131 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/contrib/syndication/apps.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1924 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/contrib/syndication/views.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.197765 django-stubs-4.2.1/django-stubs/core/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       98 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/asgi.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.197765 django-stubs-4.2.1/django-stubs/core/cache/
+-rw-r--r--   0 marti     (1000) marti      (121)      624 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/cache/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.197765 django-stubs-4.2.1/django-stubs/core/cache/backends/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/cache/backends/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4052 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/cache/backends/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      593 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/cache/backends/db.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      182 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/cache/backends/dummy.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      204 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/cache/backends/filebased.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      180 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/cache/backends/locmem.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      782 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/cache/backends/memcached.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      198 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/cache/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.201098 django-stubs-4.2.1/django-stubs/core/checks/
+-rw-r--r--   0 marti     (1000) marti      (121)      652 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/checks/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      265 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/checks/async_checks.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      529 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/checks/caches.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.201098 django-stubs-4.2.1/django-stubs/core/checks/compatibility/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/checks/compatibility/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      229 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/checks/database.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1084 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/checks/messages.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      389 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/checks/model_checks.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1799 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/checks/registry.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.201098 django-stubs-4.2.1/django-stubs/core/checks/security/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/checks/security/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1847 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/checks/security/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      399 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/checks/security/csrf.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      577 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/checks/security/sessions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      407 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/checks/templates.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      625 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/checks/translation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      706 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/checks/urls.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1912 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/exceptions.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.204431 django-stubs-4.2.1/django-stubs/core/files/
+-rw-r--r--   0 marti     (1000) marti      (121)       68 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/files/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1606 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/files/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      359 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/files/images.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      296 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/files/locks.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      130 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/files/move.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.204431 django-stubs-4.2.1/django-stubs/core/files/storage/
+-rw-r--r--   0 marti     (1000) marti      (121)      634 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/core/files/storage/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1073 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/core/files/storage/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      751 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/core/files/storage/filesystem.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      450 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/core/files/storage/handler.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      725 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/core/files/storage/memory.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      337 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/core/files/storage/mixins.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      100 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/files/temp.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1459 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/files/uploadedfile.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3017 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/files/uploadhandler.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      736 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/files/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.204431 django-stubs-4.2.1/django-stubs/core/handlers/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/handlers/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2043 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/handlers/asgi.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1220 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/handlers/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      770 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/handlers/exception.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1405 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/handlers/wsgi.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.204431 django-stubs-4.2.1/django-stubs/core/mail/
+-rw-r--r--   0 marti     (1000) marti      (121)     1714 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/core/mail/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.207765 django-stubs-4.2.1/django-stubs/core/mail/backends/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/mail/backends/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      668 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/mail/backends/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      189 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/mail/backends/console.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      103 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/mail/backends/dummy.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      128 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/mail/backends/filebased.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      103 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/mail/backends/locmem.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      395 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/mail/backends/smtp.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4639 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/core/mail/message.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       95 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/mail/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.207765 django-stubs-4.2.1/django-stubs/core/management/
+-rw-r--r--   0 marti     (1000) marti      (121)      829 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3646 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1099 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/color.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.211098 django-stubs-4.2.1/django-stubs/core/management/commands/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      179 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/check.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      430 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/compilemessages.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      284 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/createcachetable.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       85 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/dbshell.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      519 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/diffsettings.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      123 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/dumpdata.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      177 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/flush.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      789 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/inspectdb.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1140 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/loaddata.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1227 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/makemessages.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      467 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/makemigrations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      643 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/migrate.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      515 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/runserver.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      111 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/sendtestemail.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      268 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/shell.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      371 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/showmigrations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      110 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/sqlflush.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      203 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/sqlmigrate.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       83 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/sqlsequencereset.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      330 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/squashmigrations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      124 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/startapp.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      124 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/startproject.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      232 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/test.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       85 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/commands/testserver.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      488 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/sql.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      964 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/templates.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      850 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/management/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2313 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/paginator.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.211098 django-stubs-4.2.1/django-stubs/core/serializers/
+-rw-r--r--   0 marti     (1000) marti      (121)     1437 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/serializers/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3192 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/serializers/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      577 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/serializers/json.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      398 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/serializers/jsonl.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      490 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/serializers/python.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      831 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/serializers/pyyaml.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2320 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/serializers/xml_serializer.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.211098 django-stubs-4.2.1/django-stubs/core/servers/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/servers/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1165 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/servers/basehttp.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      139 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/signals.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1846 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/signing.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4397 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/validators.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       98 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/core/wsgi.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.214431 django-stubs-4.2.1/django-stubs/db/
+-rw-r--r--   0 marti     (1000) marti      (121)     1047 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.214431 django-stubs-4.2.1/django-stubs/db/backends/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.214431 django-stubs-4.2.1/django-stubs/db/backends/base/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/base/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     5296 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/db/backends/base/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      555 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/base/client.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1132 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/base/creation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     5147 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/base/features.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1826 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/base/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     6660 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/base/operations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3557 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/base/schema.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      389 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/base/validation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3134 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/ddl_references.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.214431 django-stubs-4.2.1/django-stubs/db/backends/dummy/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/dummy/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      949 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/dummy/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      176 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/dummy/features.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.217764 django-stubs-4.2.1/django-stubs/db/backends/mysql/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/mysql/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2522 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/mysql/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      483 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/mysql/client.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      734 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/mysql/compiler.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      255 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/mysql/creation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3434 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/mysql/features.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1159 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/mysql/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2760 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/mysql/operations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      902 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/mysql/schema.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      354 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/mysql/validation.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.217764 django-stubs-4.2.1/django-stubs/db/backends/oracle/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/oracle/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2711 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/oracle/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      546 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/oracle/client.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      373 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/oracle/creation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1923 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/oracle/features.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      398 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/oracle/functions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1004 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/oracle/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3888 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/oracle/operations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      924 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/oracle/schema.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      511 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/oracle/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      308 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/oracle/validation.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.221098 django-stubs-4.2.1/django-stubs/db/backends/postgresql/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/postgresql/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1382 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/postgresql/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      524 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/postgresql/client.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      208 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/postgresql/creation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2197 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/postgresql/features.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      820 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/postgresql/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      216 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/postgresql/operations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      809 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/postgresql/schema.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       63 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/signals.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.221098 django-stubs-4.2.1/django-stubs/db/backends/sqlite3/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/sqlite3/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1052 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/sqlite3/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      441 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/sqlite3/client.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      322 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/sqlite3/creation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      205 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/sqlite3/features.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      432 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/sqlite3/introspection.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      125 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/sqlite3/operations.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      215 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/sqlite3/schema.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2876 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/backends/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.224431 django-stubs-4.2.1/django-stubs/db/migrations/
+-rw-r--r--   0 marti     (1000) marti      (121)      265 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2830 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/autodetector.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      664 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/exceptions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1739 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/executor.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2420 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/graph.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1960 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/loader.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1111 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/migration.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.224431 django-stubs-4.2.1/django-stubs/db/migrations/operations/
+-rw-r--r--   0 marti     (1000) marti      (121)     1090 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/db/migrations/operations/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1426 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/operations/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1171 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/operations/fields.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4451 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/db/migrations/operations/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1977 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/operations/special.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      985 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/operations/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      290 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/optimizer.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1109 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/questioner.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      755 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/recorder.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1835 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/serializer.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2939 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/state.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      195 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1235 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/migrations/writer.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.227764 django-stubs-4.2.1/django-stubs/db/models/
+-rw-r--r--   0 marti     (1000) marti      (121)     5016 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      684 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/aggregates.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3728 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/db/models/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       16 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/constants.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2255 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/db/models/constraints.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3487 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/deletion.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1008 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/enums.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     9496 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/expressions.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.231098 django-stubs-4.2.1/django-stubs/db/models/fields/
+-rw-r--r--   0 marti     (1000) marti      (121)    21253 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/db/models/fields/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4001 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/db/models/fields/files.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3142 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/fields/json.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      515 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/fields/mixins.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      161 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/fields/proxy.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)    10684 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/db/models/fields/related.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3554 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/db/models/fields/related_descriptors.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1393 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/fields/related_lookups.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4605 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/fields/reverse_related.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.231098 django-stubs-4.2.1/django-stubs/db/models/functions/
+-rw-r--r--   0 marti     (1000) marti      (121)     3378 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/functions/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      547 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/db/models/functions/comparison.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1343 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/functions/datetime.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1222 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/functions/math.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      100 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/functions/mixins.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4623 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/functions/text.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      918 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/functions/window.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2228 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/indexes.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     5904 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/lookups.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     8468 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/db/models/manager.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     5334 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/options.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)    10808 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/db/models/query.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3306 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/db/models/query_utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      911 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/signals.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.234431 django-stubs-4.2.1/django-stubs/db/models/sql/
+-rw-r--r--   0 marti     (1000) marti      (121)      284 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/sql/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     6464 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/sql/compiler.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      344 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/sql/constants.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1791 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/sql/datastructures.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     9565 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/db/models/sql/query.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1663 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/sql/subqueries.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2075 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/sql/where.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      473 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/models/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2178 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/db/transaction.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2061 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/db/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.234431 django-stubs-4.2.1/django-stubs/dispatch/
+-rw-r--r--   0 marti     (1000) marti      (121)      116 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/dispatch/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      930 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/dispatch/dispatcher.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.234431 django-stubs-4.2.1/django-stubs/forms/
+-rw-r--r--   0 marti     (1000) marti      (121)     4083 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/forms/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2874 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/forms/boundfield.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)    20436 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/forms/fields.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3196 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/forms/forms.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3777 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/forms/formsets.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)    12234 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/forms/models.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1125 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/forms/renderers.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2337 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/forms/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)    10456 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/forms/widgets.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.237764 django-stubs-4.2.1/django-stubs/http/
+-rw-r--r--   0 marti     (1000) marti      (121)     1332 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/http/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       96 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/http/cookie.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2076 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/http/multipartparser.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     8346 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/http/request.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     5847 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/http/response.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.237764 django-stubs-4.2.1/django-stubs/middleware/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/middleware/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1062 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/middleware/cache.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      387 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/middleware/clickjacking.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      968 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/middleware/common.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1098 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/middleware/csrf.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      339 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/middleware/gzip.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      369 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/middleware/http.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      417 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/middleware/locale.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      645 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/middleware/security.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1543 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/shortcuts.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.241098 django-stubs-4.2.1/django-stubs/template/
+-rw-r--r--   0 marti     (1000) marti      (121)      756 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/__init__.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.241098 django-stubs-4.2.1/django-stubs/template/backends/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/backends/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      925 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/backends/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1062 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/backends/django.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      432 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/backends/dummy.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      575 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/backends/jinja2.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      215 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/backends/utils.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     5673 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3410 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/context.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      631 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/context_processors.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3483 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/defaultfilters.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     6912 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/defaulttags.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2158 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/engine.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      511 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/exceptions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3244 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/library.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      684 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/loader.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2266 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/loader_tags.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.244431 django-stubs-4.2.1/django-stubs/template/loaders/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/loaders/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       88 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/loaders/app_directories.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      488 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/loaders/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      554 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/loaders/cached.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      518 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/loaders/filesystem.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      323 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/loaders/locmem.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2564 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/response.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1246 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/smartif.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      589 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/template/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.244431 django-stubs-4.2.1/django-stubs/templatetags/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/templatetags/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      629 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/templatetags/cache.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3492 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/templatetags/i18n.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      410 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/templatetags/l10n.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1123 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/templatetags/static.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1076 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/templatetags/tz.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.244431 django-stubs-4.2.1/django-stubs/test/
+-rw-r--r--   0 marti     (1000) marti      (121)      848 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/test/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     7476 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/test/client.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1148 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/test/html.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     6619 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/test/runner.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      539 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/test/selenium.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      905 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/test/signals.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)    10511 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/test/testcases.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     6313 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/test/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.247764 django-stubs-4.2.1/django-stubs/urls/
+-rw-r--r--   0 marti     (1000) marti      (121)     1576 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/urls/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      886 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/urls/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1349 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/urls/conf.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      778 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/urls/converters.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      102 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/urls/exceptions.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4497 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/urls/resolvers.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      157 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/urls/utils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.254431 django-stubs-4.2.1/django-stubs/utils/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      286 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/_os.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1485 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/archive.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      235 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/asyncio.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2830 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/autoreload.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      591 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/baseconv.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1287 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/cache.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1173 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/connection.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      557 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/crypto.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4498 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/datastructures.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2062 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/dateformat.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      525 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/dateparse.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      156 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/dates.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      386 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/datetime_safe.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      325 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/deconstruct.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1185 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/utils/decorators.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1361 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/utils/deprecation.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      198 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/duration.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3255 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/encoding.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2622 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/feedgenerator.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1804 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/formats.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4146 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/functional.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       66 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/hashable.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1399 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/html.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1766 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/utils/http.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      483 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/inspect.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      175 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/ipv6.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)       61 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/itercompat.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      714 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/jslex.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1691 2023-04-27 12:45:58.000000 django-stubs-4.2.1/django-stubs/utils/log.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      242 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/lorem_ipsum.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      247 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/module_loading.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      319 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/numberformat.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      917 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/regex_helper.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      616 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/safestring.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      557 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/termcolors.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1969 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/text.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      387 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/timesince.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2011 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/timezone.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      309 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/topological_sort.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.254431 django-stubs-4.2.1/django-stubs/utils/translation/
+-rw-r--r--   0 marti     (1000) marti      (121)     2914 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/translation/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      286 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/translation/reloader.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      298 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/translation/template.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      825 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/translation/trans_null.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2929 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/translation/trans_real.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      800 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/tree.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      499 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/version.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      379 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/utils/xmlutils.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.257764 django-stubs-4.2.1/django-stubs/views/
+-rw-r--r--   0 marti     (1000) marti      (121)       39 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      274 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/csrf.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2691 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/debug.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.257764 django-stubs-4.2.1/django-stubs/views/decorators/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/decorators/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      347 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/views/decorators/cache.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      274 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/decorators/clickjacking.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      162 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/decorators/common.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      427 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/decorators/csrf.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      259 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/views/decorators/debug.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      146 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/decorators/gzip.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      718 2023-06-02 14:08:54.000000 django-stubs-4.2.1/django-stubs/views/decorators/http.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      218 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/decorators/vary.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      782 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/defaults.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.257764 django-stubs-4.2.1/django-stubs/views/generic/
+-rw-r--r--   0 marti     (1000) marti      (121)      797 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/generic/__init__.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     2272 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/generic/base.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     4525 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/generic/dates.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1109 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/generic/detail.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     3422 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/generic/edit.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1818 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/generic/list.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)     1035 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/i18n.pyi
+-rw-r--r--   0 marti     (1000) marti      (121)      482 2023-03-15 16:53:32.000000 django-stubs-4.2.1/django-stubs/views/static.pyi
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.261098 django-stubs-4.2.1/django_stubs.egg-info/
+-rw-r--r--   0 marti     (1000) marti      (121)    13907 2023-06-02 14:11:31.000000 django-stubs-4.2.1/django_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 marti     (1000) marti      (121)    30271 2023-06-02 14:11:31.000000 django-stubs-4.2.1/django_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 marti     (1000) marti      (121)        1 2023-06-02 14:11:31.000000 django-stubs-4.2.1/django_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 marti     (1000) marti      (121)      155 2023-06-02 14:11:31.000000 django-stubs-4.2.1/django_stubs.egg-info/requires.txt
+-rw-r--r--   0 marti     (1000) marti      (121)       32 2023-06-02 14:11:31.000000 django-stubs-4.2.1/django_stubs.egg-info/top_level.txt
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.261098 django-stubs-4.2.1/mypy_django_plugin/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/mypy_django_plugin/__init__.py
+-rw-r--r--   0 marti     (1000) marti      (121)     3484 2023-06-02 14:08:54.000000 django-stubs-4.2.1/mypy_django_plugin/config.py
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.261098 django-stubs-4.2.1/mypy_django_plugin/django/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/mypy_django_plugin/django/__init__.py
+-rw-r--r--   0 marti     (1000) marti      (121)    20567 2023-06-02 14:08:54.000000 django-stubs-4.2.1/mypy_django_plugin/django/context.py
+-rw-r--r--   0 marti     (1000) marti      (121)      227 2023-03-15 16:53:32.000000 django-stubs-4.2.1/mypy_django_plugin/errorcodes.py
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.261098 django-stubs-4.2.1/mypy_django_plugin/lib/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/mypy_django_plugin/lib/__init__.py
+-rw-r--r--   0 marti     (1000) marti      (121)     2289 2023-04-27 12:45:58.000000 django-stubs-4.2.1/mypy_django_plugin/lib/fullnames.py
+-rw-r--r--   0 marti     (1000) marti      (121)    13031 2023-04-27 12:45:58.000000 django-stubs-4.2.1/mypy_django_plugin/lib/helpers.py
+-rw-r--r--   0 marti     (1000) marti      (121)    15645 2023-03-15 16:53:32.000000 django-stubs-4.2.1/mypy_django_plugin/main.py
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/mypy_django_plugin/py.typed
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.264431 django-stubs-4.2.1/mypy_django_plugin/transformers/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-4.2.1/mypy_django_plugin/transformers/__init__.py
+-rw-r--r--   0 marti     (1000) marti      (121)     9647 2023-03-15 16:53:32.000000 django-stubs-4.2.1/mypy_django_plugin/transformers/fields.py
+-rw-r--r--   0 marti     (1000) marti      (121)     1809 2023-03-15 16:53:32.000000 django-stubs-4.2.1/mypy_django_plugin/transformers/forms.py
+-rw-r--r--   0 marti     (1000) marti      (121)     1335 2023-03-15 16:53:32.000000 django-stubs-4.2.1/mypy_django_plugin/transformers/functional.py
+-rw-r--r--   0 marti     (1000) marti      (121)     3104 2023-03-15 16:53:32.000000 django-stubs-4.2.1/mypy_django_plugin/transformers/init_create.py
+-rw-r--r--   0 marti     (1000) marti      (121)    20879 2023-06-02 14:08:54.000000 django-stubs-4.2.1/mypy_django_plugin/transformers/managers.py
+-rw-r--r--   0 marti     (1000) marti      (121)     1960 2023-03-15 16:53:32.000000 django-stubs-4.2.1/mypy_django_plugin/transformers/meta.py
+-rw-r--r--   0 marti     (1000) marti      (121)    32471 2023-04-27 12:45:58.000000 django-stubs-4.2.1/mypy_django_plugin/transformers/models.py
+-rw-r--r--   0 marti     (1000) marti      (121)     2659 2023-03-15 16:53:32.000000 django-stubs-4.2.1/mypy_django_plugin/transformers/orm_lookups.py
+-rw-r--r--   0 marti     (1000) marti      (121)    13195 2023-04-27 12:45:58.000000 django-stubs-4.2.1/mypy_django_plugin/transformers/querysets.py
+-rw-r--r--   0 marti     (1000) marti      (121)     2070 2023-03-15 16:53:32.000000 django-stubs-4.2.1/mypy_django_plugin/transformers/request.py
+-rw-r--r--   0 marti     (1000) marti      (121)     2003 2023-03-15 16:53:32.000000 django-stubs-4.2.1/mypy_django_plugin/transformers/settings.py
+-rw-r--r--   0 marti     (1000) marti      (121)      227 2023-03-15 16:53:32.000000 django-stubs-4.2.1/pyproject.toml
+-rw-r--r--   0 marti     (1000) marti      (121)      308 2023-06-02 14:11:31.264431 django-stubs-4.2.1/setup.cfg
+-rw-r--r--   0 marti     (1000) marti      (121)     2262 2023-06-02 14:08:54.000000 django-stubs-4.2.1/setup.py
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:31.264431 django-stubs-4.2.1/tests/
+-rw-r--r--   0 marti     (1000) marti      (121)     4735 2023-06-02 14:08:54.000000 django-stubs-4.2.1/tests/test_error_handling.py
```

### Comparing `django-stubs-4.2.0/LICENSE.txt` & `django-stubs-4.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/PKG-INFO` & `django-stubs-4.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,38 @@
 Metadata-Version: 2.1
 Name: django-stubs
-Version: 4.2.0
+Version: 4.2.1
 Summary: Mypy stubs for Django
 Home-page: https://github.com/typeddjango/django-stubs
 Author: Maksim Kurnikov
 Author-email: maxim.kurnikov@gmail.com
 Maintainer: Marti Raudsepp
 Maintainer-email: marti@juffo.org
 License: MIT
 Project-URL: Release notes, https://github.com/typeddjango/django-stubs/releases
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: compatible-mypy
-License-File: LICENSE.txt
+License-File: LICENSE.md
 
-<img src="http://mypy-lang.org/static/mypy_light.svg" alt="mypy logo" width="300px"/>
-
-# pep484 stubs for Django
+<img src="https://raw.githubusercontent.com/typeddjango/django-stubs/master/logo.svg" alt="django-stubs">
 
 [![Build status](https://github.com/typeddjango/django-stubs/workflows/test/badge.svg?branch=master&event=push)](https://github.com/typeddjango/django-stubs/actions?query=workflow%3Atest)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Gitter](https://badges.gitter.im/mypy-django/Lobby.svg)](https://gitter.im/mypy-django/Lobby)
 [![StackOverflow](https://shields.io/badge/ask-stackoverflow-orange?logo=stackoverflow)](https://stackoverflow.com/questions/tagged/django-stubs)
 
 This package contains [type stubs](https://www.python.org/dev/peps/pep-0561/) and a custom mypy plugin to provide more precise static types and type inference for Django framework. Django uses some Python "magic" that makes having precise types for some code patterns problematic. This is why we need this project. The final goal is to be able to get precise types for most common patterns.
@@ -77,20 +73,21 @@
 
 This fully working [typed boilerplate](https://github.com/wemake-services/wemake-django-template) can serve you as an example.
 
 ## Version compatibility
 
 We rely on different `django` and `mypy` versions:
 
-| django-stubs | Mypy version | Django version | Django partial support | Python version |
-|--------------|--------------|----------------|------------------------|----------------|
-| 4.2.0        | 1.2.x        | 4.2            | 4.1, 4.0, 3.2          | 3.7 - 3.11     |
-| 1.16.0       | 1.1.x        | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
-| 1.15.0       | 1.0.x        | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
-| 1.14.0       | 0.990+       | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
+| django-stubs   | Mypy version | Django version | Django partial support | Python version |
+|----------------|--------------|----------------|------------------------|----------------|
+| 4.2.1          | 1.3.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
+| 4.2.0          | 1.2.x        | 4.2            | 4.1, 4.0, 3.2          | 3.7 - 3.11     |
+| 1.16.0         | 1.1.x        | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
+| 1.15.0         | 1.0.x        | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
+| 1.14.0         | 0.990+       | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
 
 ## Features
 
 ### Type checking of Model Meta attributes
 
 By inheriting from the `TypedModelMeta` class, you can ensure you're using correct types for
 attributes:
@@ -152,16 +149,14 @@
 
    ```python
    import django_stubs_ext
 
    django_stubs_ext.monkeypatch()
    ```
 
-   Note: This monkey patching approach will only work when using Python 3.7 and higher, when the `__class_getitem__` magic method was introduced.
-
    You can add extra types to patch with `django_stubs_ext.monkeypatch(extra_classes=[YourDesiredType])`
 
 2. You can use strings instead: `'QuerySet[MyModel]'` and `'Manager[MyModel]'`, this way it will work as a type for `mypy` and as a regular `str` in runtime.
 
 ### How can I create a HttpRequest that's guaranteed to have an authenticated user?
 
 Django's built in [`HttpRequest`](https://docs.djangoproject.com/en/4.1/ref/request-response/#django.http.HttpRequest) has the attribute `user` that resolves to the type
```

### Comparing `django-stubs-4.2.0/README.md` & `django-stubs-4.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-<img src="http://mypy-lang.org/static/mypy_light.svg" alt="mypy logo" width="300px"/>
-
-# pep484 stubs for Django
+<img src="https://raw.githubusercontent.com/typeddjango/django-stubs/master/logo.svg" alt="django-stubs">
 
 [![Build status](https://github.com/typeddjango/django-stubs/workflows/test/badge.svg?branch=master&event=push)](https://github.com/typeddjango/django-stubs/actions?query=workflow%3Atest)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Gitter](https://badges.gitter.im/mypy-django/Lobby.svg)](https://gitter.im/mypy-django/Lobby)
 [![StackOverflow](https://shields.io/badge/ask-stackoverflow-orange?logo=stackoverflow)](https://stackoverflow.com/questions/tagged/django-stubs)
 
 This package contains [type stubs](https://www.python.org/dev/peps/pep-0561/) and a custom mypy plugin to provide more precise static types and type inference for Django framework. Django uses some Python "magic" that makes having precise types for some code patterns problematic. This is why we need this project. The final goal is to be able to get precise types for most common patterns.
@@ -45,20 +43,21 @@
 
 This fully working [typed boilerplate](https://github.com/wemake-services/wemake-django-template) can serve you as an example.
 
 ## Version compatibility
 
 We rely on different `django` and `mypy` versions:
 
-| django-stubs | Mypy version | Django version | Django partial support | Python version |
-|--------------|--------------|----------------|------------------------|----------------|
-| 4.2.0        | 1.2.x        | 4.2            | 4.1, 4.0, 3.2          | 3.7 - 3.11     |
-| 1.16.0       | 1.1.x        | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
-| 1.15.0       | 1.0.x        | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
-| 1.14.0       | 0.990+       | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
+| django-stubs   | Mypy version | Django version | Django partial support | Python version |
+|----------------|--------------|----------------|------------------------|----------------|
+| 4.2.1          | 1.3.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
+| 4.2.0          | 1.2.x        | 4.2            | 4.1, 4.0, 3.2          | 3.7 - 3.11     |
+| 1.16.0         | 1.1.x        | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
+| 1.15.0         | 1.0.x        | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
+| 1.14.0         | 0.990+       | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
 
 ## Features
 
 ### Type checking of Model Meta attributes
 
 By inheriting from the `TypedModelMeta` class, you can ensure you're using correct types for
 attributes:
@@ -120,16 +119,14 @@
 
    ```python
    import django_stubs_ext
 
    django_stubs_ext.monkeypatch()
    ```
 
-   Note: This monkey patching approach will only work when using Python 3.7 and higher, when the `__class_getitem__` magic method was introduced.
-
    You can add extra types to patch with `django_stubs_ext.monkeypatch(extra_classes=[YourDesiredType])`
 
 2. You can use strings instead: `'QuerySet[MyModel]'` and `'Manager[MyModel]'`, this way it will work as a type for `mypy` and as a regular `str` in runtime.
 
 ### How can I create a HttpRequest that's guaranteed to have an authenticated user?
 
 Django's built in [`HttpRequest`](https://docs.djangoproject.com/en/4.1/ref/request-response/#django.http.HttpRequest) has the attribute `user` that resolves to the type
```

### Comparing `django-stubs-4.2.0/django-stubs/apps/config.pyi` & `django-stubs-4.2.1/django-stubs/apps/config.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/apps/registry.pyi` & `django-stubs-4.2.1/django-stubs/apps/registry.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/conf/__init__.pyi` & `django-stubs-4.2.1/django-stubs/conf/__init__.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from typing import Any
 
 from _typeshed import Self
 from django.utils.functional import LazyObject
+from typing_extensions import Literal
 
 # explicit dependency on standard settings to make it loaded
 from . import global_settings
 
-ENVIRONMENT_VARIABLE: str
-PASSWORD_RESET_TIMEOUT_DAYS_DEPRECATED_MSG: str
-DEFAULT_HASHING_ALGORITHM_DEPRECATED_MSG: str
+ENVIRONMENT_VARIABLE: Literal["DJANGO_SETTINGS_MODULE"]
+DEFAULT_STORAGE_ALIAS: Literal["default"]
+STATICFILES_STORAGE_ALIAS: Literal["staticfiles"]
 
 # required for plugin to be able to distinguish this specific instance of LazySettings from others
 class _DjangoConfLazyObject(LazyObject):
     def __getattr__(self, item: Any) -> Any: ...
 
 class LazySettings(_DjangoConfLazyObject):
     SETTINGS_MODULE: str
```

### Comparing `django-stubs-4.2.0/django-stubs/conf/global_settings.pyi` & `django-stubs-4.2.1/django-stubs/conf/global_settings.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/conf/urls/__init__.pyi` & `django-stubs-4.2.1/django-stubs/conf/urls/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/admin/__init__.pyi` & `django-stubs-4.2.1/django-stubs/contrib/admin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/admin/checks.pyi` & `django-stubs-4.2.1/django-stubs/contrib/admin/checks.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/admin/decorators.pyi` & `django-stubs-4.2.1/django-stubs/contrib/admin/decorators.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/admin/filters.pyi` & `django-stubs-4.2.1/django-stubs/contrib/admin/filters.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/admin/helpers.pyi` & `django-stubs-4.2.1/django-stubs/contrib/admin/helpers.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/admin/models.pyi` & `django-stubs-4.2.1/django-stubs/contrib/admin/models.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/admin/options.pyi` & `django-stubs-4.2.1/django-stubs/contrib/admin/options.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/admin/sites.pyi` & `django-stubs-4.2.1/django-stubs/contrib/admin/sites.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     def password_change_done(
         self, request: HttpRequest, extra_context: dict[str, Any] | None = ...
     ) -> TemplateResponse: ...
     def i18n_javascript(self, request: HttpRequest, extra_context: dict[str, Any] | None = ...) -> HttpResponse: ...
     def logout(self, request: HttpRequest, extra_context: dict[str, Any] | None = ...) -> TemplateResponse: ...
     def login(self, request: HttpRequest, extra_context: dict[str, Any] | None = ...) -> HttpResponse: ...
     def _build_app_dict(self, request: HttpRequest, label: _StrOrPromise | None = ...) -> dict[str, Any]: ...
-    def get_app_list(self, request: HttpRequest, app_label: str | None) -> list[Any]: ...
+    def get_app_list(self, request: HttpRequest, app_label: str | None = ...) -> list[Any]: ...
     def index(self, request: HttpRequest, extra_context: dict[str, Any] | None = ...) -> TemplateResponse: ...
     def app_index(
         self, request: HttpRequest, app_label: str, extra_context: dict[str, Any] | None = ...
     ) -> TemplateResponse: ...
     def autocomplete_view(self, request: HttpRequest) -> HttpResponse: ...
     def catch_all_view(self, request: HttpRequest, url: str) -> HttpResponse: ...
```

### Comparing `django-stubs-4.2.0/django-stubs/contrib/admin/templatetags/admin_list.pyi` & `django-stubs-4.2.1/django-stubs/contrib/admin/templatetags/admin_list.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/admin/templatetags/admin_modify.pyi` & `django-stubs-4.2.1/django-stubs/contrib/admin/templatetags/admin_modify.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/admin/templatetags/base.pyi` & `django-stubs-4.2.1/django-stubs/contrib/admin/templatetags/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/admin/tests.pyi` & `django-stubs-4.2.1/django-stubs/contrib/admin/tests.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/admin/utils.pyi` & `django-stubs-4.2.1/django-stubs/contrib/admin/utils.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from django.forms.formsets import BaseFormSet
 from django.http.request import HttpRequest
 from django.utils.datastructures import _IndexableCollection
 from typing_extensions import Literal, TypedDict
 
 class FieldIsAForeignKeyColumnName(Exception): ...
 
-def lookup_needs_distinct(opts: Options, lookup_path: str) -> bool: ...
+def lookup_spawns_duplicates(opts: Options, lookup_path: str) -> bool: ...
 def prepare_lookup_value(key: str, value: datetime.datetime | str) -> bool | datetime.datetime | str: ...
 def quote(s: int | str | UUID) -> str: ...
 def unquote(s: str) -> str: ...
 def flatten(fields: Any) -> list[Callable | str]: ...
 def flatten_fieldsets(fieldsets: Any) -> list[Callable | str]: ...
 def get_deleted_objects(
     objs: Sequence[Model | None] | QuerySet[Model], request: HttpRequest, admin_site: AdminSite
```

### Comparing `django-stubs-4.2.0/django-stubs/contrib/admin/views/main.pyi` & `django-stubs-4.2.1/django-stubs/contrib/admin/views/main.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/admin/widgets.pyi` & `django-stubs-4.2.1/django-stubs/contrib/admin/widgets.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -38,23 +38,34 @@
 def url_params_from_lookup_dict(lookups: Any) -> dict[str, str]: ...
 
 class ForeignKeyRawIdWidget(forms.TextInput):
     rel: ManyToOneRel
     admin_site: AdminSite
     db: str | None
     def __init__(
-        self, rel: ManyToOneRel, admin_site: AdminSite, attrs: _OptAttrs | None = ..., using: str | None = ...
+        self,
+        rel: ManyToOneRel,
+        admin_site: AdminSite,
+        attrs: _OptAttrs | None = ...,
+        using: str | None = ...,
     ) -> None: ...
     def base_url_parameters(self) -> dict[str, str]: ...
     def get_context(self, name: str, value: Any, attrs: _OptAttrs | None) -> dict[str, Any]: ...
     def url_parameters(self) -> dict[str, str]: ...
     def label_and_url_for_value(self, value: Any) -> tuple[str, str]: ...
 
 class ManyToManyRawIdWidget(ForeignKeyRawIdWidget):
     rel: ManyToManyRel  # type: ignore
+    def __init__(
+        self,
+        rel: ManyToManyRel,
+        admin_site: AdminSite,
+        attrs: _OptAttrs | None = ...,
+        using: str | None = ...,
+    ) -> None: ...
     def get_context(self, name: str, value: Any, attrs: _OptAttrs | None) -> dict[str, Any]: ...
     def url_parameters(self) -> dict[str, str]: ...
     def label_and_url_for_value(self, value: Any) -> tuple[str, str]: ...
     def format_value(self, value: Any) -> str | None: ...
     def value_from_datadict(self, data: Mapping[str, Any], files: Mapping[str, Iterable[File]], name: str) -> Any: ...
 
 class RelatedFieldWidgetWrapper(forms.Widget):
```

### Comparing `django-stubs-4.2.0/django-stubs/contrib/admindocs/utils.pyi` & `django-stubs-4.2.1/django-stubs/contrib/admindocs/utils.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/admindocs/views.pyi` & `django-stubs-4.2.1/django-stubs/contrib/admindocs/views.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/auth/__init__.pyi` & `django-stubs-4.2.1/django-stubs/contrib/auth/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/auth/backends.pyi` & `django-stubs-4.2.1/django-stubs/contrib/auth/backends.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/auth/base_user.pyi` & `django-stubs-4.2.1/django-stubs/contrib/auth/base_user.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/auth/context_processors.pyi` & `django-stubs-4.2.1/django-stubs/contrib/auth/context_processors.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/auth/decorators.pyi` & `django-stubs-4.2.1/django-stubs/contrib/auth/decorators.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/auth/forms.pyi` & `django-stubs-4.2.1/django-stubs/contrib/auth/forms.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     error_messages: _ErrorMessagesT
     password1: forms.Field
     password2: forms.Field
     def __init__(self, *args: Any, **kwargs: Any) -> None: ...
     def clean_password2(self) -> str: ...
     def save(self, commit: bool = ...) -> _User: ...
 
-class UserCreationForm(BaseUserCreationForm):
+class UserCreationForm(BaseUserCreationForm[_User]):
     def clean_username(self) -> str: ...
 
 class UserChangeForm(forms.ModelForm[_User]):
     password: forms.Field
     def __init__(self, *args: Any, **kwargs: Any) -> None: ...
 
 class AuthenticationForm(forms.Form):
```

### Comparing `django-stubs-4.2.0/django-stubs/contrib/auth/hashers.pyi` & `django-stubs-4.2.1/django-stubs/contrib/auth/hashers.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/auth/middleware.pyi` & `django-stubs-4.2.1/django-stubs/contrib/auth/middleware.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/auth/mixins.pyi` & `django-stubs-4.2.1/django-stubs/contrib/auth/mixins.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/auth/models.pyi` & `django-stubs-4.2.1/django-stubs/contrib/auth/models.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/auth/password_validation.pyi` & `django-stubs-4.2.1/django-stubs/contrib/auth/password_validation.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/auth/tokens.pyi` & `django-stubs-4.2.1/django-stubs/contrib/auth/tokens.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 class PasswordResetTokenGenerator:
     key_salt: str
     secret: str | bytes
     secret_fallbacks: list[str | bytes]
     algorithm: str
     def make_token(self, user: AbstractBaseUser) -> str: ...
     def check_token(self, user: AbstractBaseUser | None, token: str | None) -> bool: ...
-    def _make_token_with_timestamp(self, user: AbstractBaseUser, timestamp: int, legacy: bool = ...) -> str: ...
+    def _make_token_with_timestamp(self, user: AbstractBaseUser, timestamp: int, secret: str | bytes = ...) -> str: ...
     def _make_hash_value(self, user: AbstractBaseUser, timestamp: int) -> str: ...
     def _num_seconds(self, dt: datetime | date) -> int: ...
     def _now(self) -> datetime: ...
 
 default_token_generator: Any
```

### Comparing `django-stubs-4.2.0/django-stubs/contrib/auth/views.pyi` & `django-stubs-4.2.1/django-stubs/contrib/auth/views.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/contenttypes/admin.pyi` & `django-stubs-4.2.1/django-stubs/contrib/contenttypes/admin.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/contenttypes/fields.pyi` & `django-stubs-4.2.1/django-stubs/contrib/contenttypes/fields.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/contenttypes/forms.pyi` & `django-stubs-4.2.1/django-stubs/contrib/contenttypes/forms.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/contenttypes/management/__init__.pyi` & `django-stubs-4.2.1/django-stubs/contrib/contenttypes/management/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/contenttypes/models.pyi` & `django-stubs-4.2.1/django-stubs/contrib/contenttypes/models.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/admin/__init__.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/admin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/admin/options.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/admin/options.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/base/features.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/base/features.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/base/models.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/base/models.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/base/operations.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/base/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/mysql/features.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/mysql/features.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/mysql/operations.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/mysql/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/mysql/schema.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/mysql/schema.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/oracle/models.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/oracle/models.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/oracle/operations.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/oracle/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/oracle/schema.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/oracle/schema.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/postgis/models.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/postgis/models.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/postgis/operations.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/postgis/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/spatialite/models.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/spatialite/models.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/spatialite/operations.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/spatialite/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/spatialite/schema.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/spatialite/schema.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/db/backends/utils.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/db/backends/utils.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/db/models/__init__.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/db/models/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/db/models/aggregates.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/db/models/aggregates.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/db/models/fields.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/db/models/fields.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     MultiLineString,
     MultiPoint,
     MultiPolygon,
     Point,
     Polygon,
 )
 from django.core.validators import _ValidatorCallable
+from django.db.models.expressions import Combinable
 from django.db.models.fields import Field, _ErrorMessagesT, _FieldChoices
 from django.utils.functional import _StrOrPromise
 
 # __set__ value type
 _ST = TypeVar("_ST")
 # __get__ return type
 _GT = TypeVar("_GT")
@@ -71,15 +72,15 @@
     def geodetic(self, connection: Any) -> Any: ...
     def get_placeholder(self, value: Any, compiler: Any, connection: Any) -> Any: ...
     def get_srid(self, obj: Any) -> Any: ...
     def get_db_prep_value(self, value: Any, connection: Any, *args: Any, **kwargs: Any) -> Any: ...
     def get_raster_prep_value(self, value: Any, is_candidate: Any) -> Any: ...
     def get_prep_value(self, value: Any) -> Any: ...
 
-class GeometryField(BaseSpatialField):
+class GeometryField(BaseSpatialField[_ST, _GT]):
     dim: int
     def __init__(
         self,
         verbose_name: _StrOrPromise | None = ...,
         dim: int = ...,
         geography: bool = ...,
         *,
@@ -108,39 +109,67 @@
         validators: Iterable[_ValidatorCallable] = ...,
         error_messages: _ErrorMessagesT | None = ...,
     ) -> None: ...
     def deconstruct(self) -> Any: ...
     def formfield(self, **kwargs: Any) -> Any: ...  # type: ignore[override]
     def select_format(self, compiler: Any, sql: Any, params: Any) -> Any: ...
 
-class PointField(GeometryField):
+class PointField(GeometryField[_ST, _GT]):
+    _pyi_private_set_type: Point | Combinable
+    _pyi_private_get_type: Point
+    _pyi_lookup_exact_type: Point
+
     geom_class: type[Point]
     form_class: type[forms.PointField]
 
-class LineStringField(GeometryField):
+class LineStringField(GeometryField[_ST, _GT]):
+    _pyi_private_set_type: LineString | Combinable
+    _pyi_private_get_type: LineString
+    _pyi_lookup_exact_type: LineString
+
     geom_class: type[LineString]
     form_class: type[forms.LineStringField]
 
-class PolygonField(GeometryField):
+class PolygonField(GeometryField[_ST, _GT]):
+    _pyi_private_set_type: Polygon | Combinable
+    _pyi_private_get_type: Polygon
+    _pyi_lookup_exact_type: Polygon
+
     geom_class: type[Polygon]
     form_class: type[forms.PolygonField]
 
-class MultiPointField(GeometryField):
+class MultiPointField(GeometryField[_ST, _GT]):
+    _pyi_private_set_type: MultiPoint | Combinable
+    _pyi_private_get_type: MultiPoint
+    _pyi_lookup_exact_type: MultiPoint
+
     geom_class: type[MultiPoint]
     form_class: type[forms.MultiPointField]
 
-class MultiLineStringField(GeometryField):
+class MultiLineStringField(GeometryField[_ST, _GT]):
+    _pyi_private_set_type: MultiLineString | Combinable
+    _pyi_private_get_type: MultiLineString
+    _pyi_lookup_exact_type: MultiLineString
+
     geom_class: type[MultiLineString]
     form_class: type[forms.MultiLineStringField]
 
-class MultiPolygonField(GeometryField):
+class MultiPolygonField(GeometryField[_ST, _GT]):
+    _pyi_private_set_type: MultiPolygon | Combinable
+    _pyi_private_get_type: MultiPolygon
+    _pyi_lookup_exact_type: MultiPolygon
+
     geom_class: type[MultiPolygon]
     form_class: type[forms.MultiPolygonField]
 
-class GeometryCollectionField(GeometryField):
+class GeometryCollectionField(GeometryField[_ST, _GT]):
+    _pyi_private_set_type: GeometryCollection | Combinable
+    _pyi_private_get_type: GeometryCollection
+    _pyi_lookup_exact_type: GeometryCollection
+
     geom_class: type[GeometryCollection]
     form_class: type[forms.GeometryCollectionField]
 
 class ExtentField(Field):
     def get_internal_type(self) -> Any: ...
     def select_format(self, compiler: Any, sql: Any, params: Any) -> Any: ...
```

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/db/models/functions.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/db/models/functions.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/db/models/lookups.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/db/models/lookups.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/db/models/sql/conversion.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/db/models/sql/conversion.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/feeds.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/feeds.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/forms/__init__.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/forms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/forms/fields.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/forms/fields.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/forms/widgets.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/forms/widgets.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/gdal/__init__.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/gdal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/gdal/datasource.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/gdal/datasource.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/gdal/envelope.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/gdal/envelope.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/gdal/feature.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/gdal/feature.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/gdal/field.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/gdal/field.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/gdal/geometries.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/gdal/geometries.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/gdal/layer.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/gdal/layer.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/gdal/prototypes/ds.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/gdal/prototypes/ds.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/gdal/prototypes/errcheck.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/gdal/prototypes/errcheck.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/gdal/prototypes/generation.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/gdal/prototypes/generation.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/gdal/prototypes/geom.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/gdal/prototypes/geom.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/gdal/prototypes/raster.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/gdal/prototypes/raster.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/gdal/prototypes/srs.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/gdal/prototypes/srs.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/gdal/raster/band.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/gdal/raster/band.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/gdal/raster/source.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/gdal/raster/source.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/gdal/srs.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/gdal/srs.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/geoip2/base.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/geoip2/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/geos/__init__.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/geos/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/geos/collections.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/geos/collections.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/geos/coordseq.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/geos/coordseq.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/geos/geometry.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/geos/geometry.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/geos/libgeos.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/geos/libgeos.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/geos/linestring.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/geos/linestring.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/geos/mutable_list.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/geos/mutable_list.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/geos/point.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/geos/point.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/geos/polygon.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/geos/polygon.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/geos/prepared.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/geos/prepared.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/geos/prototypes/__init__.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/geos/prototypes/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/geos/prototypes/coordseq.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/geos/prototypes/coordseq.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/geos/prototypes/geom.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/geos/prototypes/geom.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/geos/prototypes/io.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/geos/prototypes/io.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/geos/prototypes/predicates.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/geos/prototypes/predicates.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/geos/prototypes/topology.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/geos/prototypes/topology.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/measure.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/measure.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/gis/utils/layermapping.pyi` & `django-stubs-4.2.1/django-stubs/contrib/gis/utils/layermapping.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/humanize/templatetags/humanize.pyi` & `django-stubs-4.2.1/django-stubs/contrib/humanize/templatetags/humanize.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/messages/__init__.pyi` & `django-stubs-4.2.1/django-stubs/contrib/messages/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/messages/api.pyi` & `django-stubs-4.2.1/django-stubs/contrib/messages/api.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/messages/storage/base.pyi` & `django-stubs-4.2.1/django-stubs/contrib/messages/storage/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/postgres/aggregates/__init__.pyi` & `django-stubs-4.2.1/django-stubs/contrib/postgres/aggregates/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/postgres/constraints.pyi` & `django-stubs-4.2.1/django-stubs/contrib/postgres/constraints.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/postgres/fields/__init__.pyi` & `django-stubs-4.2.1/django-stubs/contrib/postgres/fields/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/postgres/fields/array.pyi` & `django-stubs-4.2.1/django-stubs/contrib/postgres/fields/array.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/postgres/fields/hstore.pyi` & `django-stubs-4.2.1/django-stubs/contrib/postgres/fields/hstore.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/postgres/fields/ranges.pyi` & `django-stubs-4.2.1/django-stubs/contrib/postgres/fields/ranges.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/postgres/forms/array.pyi` & `django-stubs-4.2.1/django-stubs/contrib/postgres/forms/array.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/postgres/forms/ranges.pyi` & `django-stubs-4.2.1/django-stubs/contrib/postgres/forms/ranges.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/postgres/indexes.pyi` & `django-stubs-4.2.1/django-stubs/contrib/postgres/indexes.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/postgres/lookups.pyi` & `django-stubs-4.2.1/django-stubs/contrib/postgres/lookups.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/postgres/operations.pyi` & `django-stubs-4.2.1/django-stubs/contrib/postgres/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/postgres/search.pyi` & `django-stubs-4.2.1/django-stubs/contrib/postgres/search.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/postgres/validators.pyi` & `django-stubs-4.2.1/django-stubs/contrib/postgres/validators.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/sessions/backends/base.pyi` & `django-stubs-4.2.1/django-stubs/contrib/sessions/backends/base.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -9,33 +9,36 @@
 class SessionBase(dict[str, Any]):
     TEST_COOKIE_NAME: str
     TEST_COOKIE_VALUE: str
     accessed: bool
     modified: bool
     serializer: Any
     def __init__(self, session_key: str | None = ...) -> None: ...
+    @property
+    def key_salt(self) -> str: ...
     def set_test_cookie(self) -> None: ...
     def test_cookie_worked(self) -> bool: ...
     def delete_test_cookie(self) -> None: ...
     def encode(self, session_dict: dict[str, Any]) -> str: ...
     def decode(self, session_data: bytes | str) -> dict[str, Any]: ...
-    def has_key(self, key: Any) -> Any: ...
+    def has_key(self, key: Any) -> bool: ...
     def keys(self) -> Any: ...
     def values(self) -> Any: ...
     def items(self) -> Any: ...
     def clear(self) -> None: ...
     def is_empty(self) -> bool: ...
     def _get_session_key(self) -> str | None: ...
     def _set_session_key(self, value: str | None) -> None: ...
     @property
     def session_key(self) -> str | None: ...
     @property
     def _session_key(self) -> str | None: ...
     @_session_key.setter
     def _session_key(self, value: str | None) -> None: ...
+    def get_session_cookie_age(self) -> int: ...
     def get_expiry_age(self, **kwargs: Any) -> int: ...
     def get_expiry_date(self, **kwargs: Any) -> datetime: ...
     def set_expiry(self, value: datetime | int | None) -> None: ...
     def get_expire_at_browser_close(self) -> bool: ...
     def flush(self) -> None: ...
     def cycle_key(self) -> None: ...
     def exists(self, session_key: str) -> bool: ...
```

### Comparing `django-stubs-4.2.0/django-stubs/contrib/sessions/backends/db.pyi` & `django-stubs-4.2.1/django-stubs/db/models/functions/comparison.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,22 @@
-from django.contrib.sessions.backends.base import SessionBase
-from django.contrib.sessions.base_session import AbstractBaseSession
-from django.contrib.sessions.models import Session
-from django.db.models.base import Model
-
-class SessionStore(SessionBase):
-    def __init__(self, session_key: str | None = ...) -> None: ...
-    @classmethod
-    def get_model_class(cls) -> type[Session]: ...
-    @property
-    def model(self) -> type[AbstractBaseSession]: ...
-    def create_model_instance(self, data: dict[str, Model]) -> AbstractBaseSession: ...
+from typing import Any
+
+from django.db.models import Func
+from django.db.models.fields import Field
+from django.db.models.fields.json import JSONField
+
+class Cast(Func):
+    def __init__(self, expression: Any, output_field: str | Field) -> None: ...
+
+class Coalesce(Func): ...
+
+class Collate(Func):
+    def __init__(self, expression: Any, collation: str) -> None: ...
+
+class Greatest(Func): ...
+
+class JSONObject(Func):
+    def __init__(self, **fields: Any) -> None: ...
+    output_field: JSONField
+
+class Least(Func): ...
+class NullIf(Func): ...
```

### Comparing `django-stubs-4.2.0/django-stubs/contrib/sessions/base_session.pyi` & `django-stubs-4.2.1/django-stubs/contrib/sessions/base_session.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/sitemaps/__init__.pyi` & `django-stubs-4.2.1/django-stubs/contrib/sitemaps/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/sitemaps/views.pyi` & `django-stubs-4.2.1/django-stubs/contrib/sitemaps/views.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/sites/models.pyi` & `django-stubs-4.2.1/django-stubs/contrib/sites/models.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/staticfiles/finders.pyi` & `django-stubs-4.2.1/django-stubs/contrib/staticfiles/finders.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/staticfiles/handlers.pyi` & `django-stubs-4.2.1/django-stubs/contrib/staticfiles/handlers.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/staticfiles/management/commands/collectstatic.pyi` & `django-stubs-4.2.1/django-stubs/contrib/staticfiles/management/commands/collectstatic.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/staticfiles/storage.pyi` & `django-stubs-4.2.1/django-stubs/contrib/staticfiles/storage.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/contrib/syndication/views.pyi` & `django-stubs-4.2.1/django-stubs/contrib/syndication/views.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/cache/__init__.pyi` & `django-stubs-4.2.1/django-stubs/core/cache/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/cache/backends/base.pyi` & `django-stubs-4.2.1/django-stubs/core/cache/backends/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/cache/backends/db.pyi` & `django-stubs-4.2.1/django-stubs/core/cache/backends/db.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/cache/backends/memcached.pyi` & `django-stubs-4.2.1/django-stubs/core/cache/backends/memcached.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/checks/__init__.pyi` & `django-stubs-4.2.1/django-stubs/core/checks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/checks/caches.pyi` & `django-stubs-4.2.1/django-stubs/core/checks/caches.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/checks/messages.pyi` & `django-stubs-4.2.1/django-stubs/core/checks/messages.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/checks/registry.pyi` & `django-stubs-4.2.1/django-stubs/core/checks/registry.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/checks/security/base.pyi` & `django-stubs-4.2.1/django-stubs/core/checks/security/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/checks/security/sessions.pyi` & `django-stubs-4.2.1/django-stubs/core/checks/security/sessions.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/checks/translation.pyi` & `django-stubs-4.2.1/django-stubs/core/checks/translation.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/checks/urls.pyi` & `django-stubs-4.2.1/django-stubs/core/checks/urls.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/exceptions.pyi` & `django-stubs-4.2.1/django-stubs/core/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/files/base.pyi` & `django-stubs-4.2.1/django-stubs/core/files/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/files/storage.pyi` & `django-stubs-4.2.1/django-stubs/core/management/templates.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,49 +1,22 @@
-from datetime import datetime
-from typing import IO, Any
-
-from django.core.files.base import File
-from django.utils._os import _PathCompatible
-from django.utils.functional import LazyObject
-
-class Storage:
-    def open(self, name: str, mode: str = ...) -> File: ...
-    def save(self, name: str | None, content: IO[Any], max_length: int | None = ...) -> str: ...
-    def get_valid_name(self, name: str) -> str: ...
-    def get_alternative_name(self, file_root: str, file_ext: str) -> str: ...
-    def get_available_name(self, name: str, max_length: int | None = ...) -> str: ...
-    def generate_filename(self, filename: _PathCompatible) -> str: ...
-    def path(self, name: str) -> str: ...
-    def delete(self, name: str) -> None: ...
-    def exists(self, name: str) -> bool: ...
-    def listdir(self, path: str) -> tuple[list[str], list[str]]: ...
-    def size(self, name: str) -> int: ...
-    def url(self, name: str | None) -> str: ...
-    def get_accessed_time(self, name: str) -> datetime: ...
-    def get_created_time(self, name: str) -> datetime: ...
-    def get_modified_time(self, name: str) -> datetime: ...
-
-class FileSystemStorage(Storage):
-    OS_OPEN_FLAGS: int
-    def __init__(
-        self,
-        location: _PathCompatible | None = ...,
-        base_url: str | None = ...,
-        file_permissions_mode: int | None = ...,
-        directory_permissions_mode: int | None = ...,
-    ) -> None: ...
-    @property
-    def base_location(self) -> _PathCompatible: ...
-    @property
-    def location(self) -> _PathCompatible: ...
-    @property
-    def base_url(self) -> str: ...
-    @property
-    def file_permissions_mode(self) -> int | None: ...
-    @property
-    def directory_permissions_mode(self) -> int | None: ...
-
-class DefaultStorage(LazyObject): ...
-
-default_storage: Any
-
-def get_storage_class(import_path: str | None = ...) -> type[Storage]: ...
+from argparse import ArgumentParser
+from collections.abc import Sequence
+from typing import Any
+
+from django.core.management.base import BaseCommand
+
+class TemplateCommand(BaseCommand):
+    url_schemes: Sequence[str]
+    rewrite_template_suffixes: Sequence[tuple[str, str]]
+    app_or_project: str
+    a_or_an: str
+    paths_to_remove: Sequence[Any]
+    verbosity: Any
+    def add_arguments(self, parser: ArgumentParser) -> None: ...
+    def handle(self, app_or_project: str, name: str, target: str | None = ..., **options: Any) -> None: ...
+    def handle_template(self, template: str | None, subdir: str | None) -> str: ...
+    def validate_name(self, name: str, name_or_dir: str = ...) -> None: ...
+    def download(self, url: str) -> str: ...
+    def splitext(self, the_path: str) -> tuple[str, str]: ...
+    def extract(self, filename: str) -> str: ...
+    def is_url(self, template: str) -> bool: ...
+    def make_writeable(self, filename: str) -> None: ...
```

### Comparing `django-stubs-4.2.0/django-stubs/core/files/uploadedfile.pyi` & `django-stubs-4.2.1/django-stubs/core/files/uploadedfile.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/files/uploadhandler.pyi` & `django-stubs-4.2.1/django-stubs/core/files/uploadhandler.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/files/utils.pyi` & `django-stubs-4.2.1/django-stubs/core/files/utils.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/handlers/asgi.pyi` & `django-stubs-4.2.1/django-stubs/core/handlers/asgi.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/handlers/base.pyi` & `django-stubs-4.2.1/django-stubs/core/handlers/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/handlers/exception.pyi` & `django-stubs-4.2.1/django-stubs/core/handlers/exception.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/handlers/wsgi.pyi` & `django-stubs-4.2.1/django-stubs/core/handlers/wsgi.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/mail/__init__.pyi` & `django-stubs-4.2.1/django-stubs/core/mail/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     fail_silently: bool = ...,
     auth_user: str | None = ...,
     auth_password: str | None = ...,
     connection: Any | None = ...,
     html_message: str | None = ...,
 ) -> int: ...
 def send_mass_mail(
-    datatuple: Iterable[tuple[str, str, str, list[str]]],
+    datatuple: Iterable[tuple[str, str, str | None, list[str]]],
     fail_silently: bool = ...,
     auth_user: str | None = ...,
     auth_password: str | None = ...,
     connection: Any | None = ...,
 ) -> int: ...
 def mail_admins(
     subject: _StrOrPromise,
```

### Comparing `django-stubs-4.2.0/django-stubs/core/mail/backends/base.pyi` & `django-stubs-4.2.1/django-stubs/core/mail/backends/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/mail/message.pyi` & `django-stubs-4.2.1/django-stubs/core/mail/message.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -2,18 +2,15 @@
 from email import charset as Charset
 from email._policybase import Policy
 from email.message import Message
 from email.mime.base import MIMEBase
 from email.mime.message import MIMEMessage
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
-
-# switch to tuple once https://github.com/python/mypy/issues/11098 is fixed
-# remove Optional once python 3.7 is dropped (Tuple[str | None, ...] works with mypy on py3.10)
-from typing import Any, Optional, Tuple, overload  # noqa: Y022, Y037
+from typing import Any, overload
 
 from django.utils.functional import _StrOrPromise
 from typing_extensions import TypeAlias
 
 utf8_charset: Any
 utf8_charset_qp: Any
 DEFAULT_ATTACHMENT_MIME_TYPE: str
@@ -62,20 +59,16 @@
         _subparts: Any | None = ...,
         encoding: str = ...,
         **_params: Any
     ) -> None: ...
     def __setitem__(self, name: str, val: str) -> None: ...
 
 _AttachmentContent: TypeAlias = bytes | EmailMessage | Message | SafeMIMEText | str
-# switch to tuple once https://github.com/python/mypy/issues/11098 is fixed
-# remove Optional once python 3.7 is dropped (Tuple[str | None, ...] works with mypy on py3.10)
 _AttachmentTuple: TypeAlias = (
-    Tuple[str, _AttachmentContent]
-    | Tuple[Optional[str], _AttachmentContent, str]
-    | Tuple[str, _AttachmentContent, None]
+    tuple[str, _AttachmentContent] | tuple[str | None, _AttachmentContent, str] | tuple[str, _AttachmentContent, None]
 )
 
 class EmailMessage:
     content_subtype: str
     mixed_subtype: str
     encoding: Any
     to: list[str]
```

### Comparing `django-stubs-4.2.0/django-stubs/core/management/__init__.pyi` & `django-stubs-4.2.1/django-stubs/core/management/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/management/base.pyi` & `django-stubs-4.2.1/django-stubs/core/management/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/management/color.pyi` & `django-stubs-4.2.1/django-stubs/core/management/color.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/management/commands/diffsettings.pyi` & `django-stubs-4.2.1/django-stubs/core/management/commands/diffsettings.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/management/commands/inspectdb.pyi` & `django-stubs-4.2.1/django-stubs/core/management/commands/inspectdb.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/management/commands/loaddata.pyi` & `django-stubs-4.2.1/django-stubs/core/management/commands/loaddata.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/management/commands/makemessages.pyi` & `django-stubs-4.2.1/django-stubs/core/management/commands/makemessages.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/management/commands/migrate.pyi` & `django-stubs-4.2.1/django-stubs/core/management/commands/migrate.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/management/commands/runserver.pyi` & `django-stubs-4.2.1/django-stubs/core/management/commands/runserver.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/management/utils.pyi` & `django-stubs-4.2.1/django-stubs/core/management/utils.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/paginator.pyi` & `django-stubs-4.2.1/django-stubs/core/paginator.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/serializers/__init__.pyi` & `django-stubs-4.2.1/django-stubs/core/serializers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/serializers/base.pyi` & `django-stubs-4.2.1/django-stubs/core/serializers/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/serializers/json.pyi` & `django-stubs-4.2.1/django-stubs/core/serializers/json.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/serializers/pyyaml.pyi` & `django-stubs-4.2.1/django-stubs/core/serializers/pyyaml.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/serializers/xml_serializer.pyi` & `django-stubs-4.2.1/django-stubs/core/serializers/xml_serializer.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/servers/basehttp.pyi` & `django-stubs-4.2.1/django-stubs/core/servers/basehttp.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/signing.pyi` & `django-stubs-4.2.1/django-stubs/core/signing.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/core/validators.pyi` & `django-stubs-4.2.1/django-stubs/core/validators.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/__init__.pyi` & `django-stubs-4.2.1/django-stubs/db/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/backends/base/base.pyi` & `django-stubs-4.2.1/django-stubs/db/backends/base/base.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -111,12 +111,12 @@
     def make_debug_cursor(self, cursor: CursorWrapper) -> CursorDebugWrapper: ...
     def make_cursor(self, cursor: CursorWrapper) -> CursorWrapper: ...
     @contextmanager
     def temporary_connection(self) -> Generator[CursorWrapper, None, None]: ...
     @contextmanager
     def _nodb_cursor(self) -> Generator[CursorWrapper, None, None]: ...
     def schema_editor(self, *args: Any, **kwargs: Any) -> BaseDatabaseSchemaEditor: ...
-    def on_commit(self, func: Callable[[], None]) -> None: ...
+    def on_commit(self, func: Callable[[], object], robust: bool = ...) -> None: ...
     def run_and_clear_commit_hooks(self) -> None: ...
     @contextmanager
     def execute_wrapper(self, wrapper: _ExecuteWrapper) -> Generator[None, None, None]: ...
     def copy(self: Self, alias: str | None = ...) -> Self: ...
```

### Comparing `django-stubs-4.2.0/django-stubs/db/backends/base/client.pyi` & `django-stubs-4.2.1/django-stubs/db/backends/base/client.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/backends/base/creation.pyi` & `django-stubs-4.2.1/django-stubs/db/backends/base/creation.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/backends/base/features.pyi` & `django-stubs-4.2.1/django-stubs/db/backends/base/features.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/backends/base/introspection.pyi` & `django-stubs-4.2.1/django-stubs/db/backends/base/introspection.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/backends/base/operations.pyi` & `django-stubs-4.2.1/django-stubs/db/backends/base/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/backends/base/schema.pyi` & `django-stubs-4.2.1/django-stubs/db/backends/base/schema.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/backends/ddl_references.pyi` & `django-stubs-4.2.1/django-stubs/db/backends/ddl_references.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/backends/dummy/base.pyi` & `django-stubs-4.2.1/django-stubs/db/backends/dummy/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/backends/mysql/base.pyi` & `django-stubs-4.2.1/django-stubs/db/backends/mysql/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/backends/mysql/compiler.pyi` & `django-stubs-4.2.1/django-stubs/db/backends/mysql/compiler.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/backends/mysql/features.pyi` & `django-stubs-4.2.1/django-stubs/db/backends/mysql/features.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/backends/mysql/introspection.pyi` & `django-stubs-4.2.1/django-stubs/db/backends/mysql/introspection.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/backends/mysql/operations.pyi` & `django-stubs-4.2.1/django-stubs/db/backends/mysql/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/backends/mysql/schema.pyi` & `django-stubs-4.2.1/django-stubs/db/backends/mysql/schema.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/backends/oracle/base.pyi` & `django-stubs-4.2.1/django-stubs/db/backends/oracle/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/backends/oracle/client.pyi` & `django-stubs-4.2.1/django-stubs/db/backends/oracle/client.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/backends/oracle/features.pyi` & `django-stubs-4.2.1/django-stubs/db/backends/oracle/features.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/backends/oracle/introspection.pyi` & `django-stubs-4.2.1/django-stubs/db/backends/oracle/introspection.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/backends/oracle/operations.pyi` & `django-stubs-4.2.1/django-stubs/db/backends/oracle/operations.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/backends/oracle/schema.pyi` & `django-stubs-4.2.1/django-stubs/db/backends/oracle/schema.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/backends/postgresql/base.pyi` & `django-stubs-4.2.1/django-stubs/db/backends/postgresql/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/backends/postgresql/client.pyi` & `django-stubs-4.2.1/django-stubs/db/backends/postgresql/client.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/backends/postgresql/features.pyi` & `django-stubs-4.2.1/django-stubs/db/backends/postgresql/features.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/backends/postgresql/introspection.pyi` & `django-stubs-4.2.1/django-stubs/db/backends/postgresql/introspection.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/backends/postgresql/schema.pyi` & `django-stubs-4.2.1/django-stubs/db/backends/postgresql/schema.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/backends/sqlite3/base.pyi` & `django-stubs-4.2.1/django-stubs/db/backends/sqlite3/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/backends/utils.pyi` & `django-stubs-4.2.1/django-stubs/db/backends/utils.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/migrations/autodetector.pyi` & `django-stubs-4.2.1/django-stubs/db/migrations/autodetector.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/migrations/exceptions.pyi` & `django-stubs-4.2.1/django-stubs/db/migrations/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/migrations/executor.pyi` & `django-stubs-4.2.1/django-stubs/db/migrations/executor.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/migrations/graph.pyi` & `django-stubs-4.2.1/django-stubs/db/migrations/graph.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/migrations/loader.pyi` & `django-stubs-4.2.1/django-stubs/db/migrations/loader.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/migrations/migration.pyi` & `django-stubs-4.2.1/django-stubs/db/migrations/migration.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/migrations/operations/__init__.pyi` & `django-stubs-4.2.1/django-stubs/db/migrations/operations/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/migrations/operations/base.pyi` & `django-stubs-4.2.1/django-stubs/db/migrations/operations/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/migrations/operations/fields.pyi` & `django-stubs-4.2.1/django-stubs/db/migrations/operations/fields.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/migrations/operations/models.pyi` & `django-stubs-4.2.1/django-stubs/db/migrations/operations/models.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/migrations/operations/special.pyi` & `django-stubs-4.2.1/django-stubs/db/migrations/operations/special.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/migrations/operations/utils.pyi` & `django-stubs-4.2.1/django-stubs/db/migrations/operations/utils.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/migrations/questioner.pyi` & `django-stubs-4.2.1/django-stubs/db/migrations/questioner.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/migrations/recorder.pyi` & `django-stubs-4.2.1/django-stubs/db/migrations/recorder.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/migrations/serializer.pyi` & `django-stubs-4.2.1/django-stubs/db/migrations/serializer.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/migrations/state.pyi` & `django-stubs-4.2.1/django-stubs/db/migrations/state.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/migrations/writer.pyi` & `django-stubs-4.2.1/django-stubs/db/migrations/writer.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/models/__init__.pyi` & `django-stubs-4.2.1/django-stubs/db/models/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/models/aggregates.pyi` & `django-stubs-4.2.1/django-stubs/db/models/aggregates.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/models/base.pyi` & `django-stubs-4.2.1/django-stubs/db/models/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/models/constraints.pyi` & `django-stubs-4.2.1/django-stubs/db/models/constraints.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/models/deletion.pyi` & `django-stubs-4.2.1/django-stubs/db/models/deletion.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/models/enums.pyi` & `django-stubs-4.2.1/django-stubs/db/models/enums.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/models/expressions.pyi` & `django-stubs-4.2.1/django-stubs/db/models/expressions.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/models/fields/__init__.pyi` & `django-stubs-4.2.1/django-stubs/db/models/fields/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,44 +2,54 @@
 import uuid
 from collections.abc import Callable, Iterable, Sequence
 from datetime import date
 from datetime import datetime as real_datetime
 from datetime import time, timedelta
 from typing import Any, Generic, Protocol, TypeVar, overload
 
-from _typeshed import Self
 from django.core import validators  # due to weird mypy.stubtest error
 from django.core.checks import CheckMessage
 from django.core.exceptions import FieldDoesNotExist as FieldDoesNotExist
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models import Model
 from django.db.models.expressions import Col, Combinable
 from django.db.models.fields.reverse_related import ForeignObjectRel
 from django.db.models.query_utils import Q, RegisterLookupMixin
 from django.forms import Field as FormField
 from django.forms import Widget
 from django.utils.datastructures import DictWrapper
 from django.utils.functional import _Getter, _StrOrPromise
-from typing_extensions import TypeAlias
+from typing_extensions import Self, TypeAlias
 
 class Empty: ...
 class NOT_PROVIDED: ...
 
 BLANK_CHOICE_DASH: list[tuple[str, str]]
 
 _Choice: TypeAlias = tuple[Any, Any]
 
 _ChoiceNamedGroup: TypeAlias = tuple[str, Iterable[_Choice]]
 _FieldChoices: TypeAlias = Iterable[_Choice | _ChoiceNamedGroup]
 _ChoicesList: TypeAlias = Sequence[_Choice] | Sequence[_ChoiceNamedGroup]
 _LimitChoicesTo: TypeAlias = Q | dict[str, Any]
 
+_F = TypeVar("_F", bound=Field, covariant=True)
+
 class _ChoicesCallable(Protocol):
     def __call__(self) -> _FieldChoices: ...
 
+class _FieldDescriptor(Protocol[_F]):
+    """
+    Accessing fields of a model class (not instance) returns an object conforming to this protocol.
+    Depending on field type this could be DeferredAttribute, ForwardManyToOneDescriptor, FileDescriptor, etc.
+    """
+
+    @property
+    def field(self) -> _F: ...
+
 _AllLimitChoicesTo: TypeAlias = _LimitChoicesTo | _ChoicesCallable  # noqa: Y047
 _ErrorMessagesT: TypeAlias = dict[str, Any]
 
 # __set__ value type
 _ST = TypeVar("_ST", contravariant=True)
 # __get__ return type
 _GT = TypeVar("_GT", covariant=True)
@@ -127,14 +137,15 @@
     blank: bool
     null: bool
     unique: bool
     editable: bool
     empty_strings_allowed: bool
     choices: _ChoicesList | None
     db_column: str | None
+    db_comment: str | None
     column: str
     concrete: bool
     default: Any
     error_messages: _ErrorMessagesT
     empty_values: Sequence[Any]
     creation_counter: int
     auto_creation_counter: int
@@ -160,23 +171,24 @@
         serialize: bool = ...,
         unique_for_date: str | None = ...,
         unique_for_month: str | None = ...,
         unique_for_year: str | None = ...,
         choices: _FieldChoices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
+        db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         auto_created: bool = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesT | None = ...,
     ) -> None: ...
     def __set__(self, instance: Any, value: _ST) -> None: ...
     # class access
     @overload
-    def __get__(self: Self, instance: None, owner: Any) -> Self: ...
+    def __get__(self: Self, instance: None, owner: Any) -> _FieldDescriptor[Self]: ...
     # Model instance access
     @overload
     def __get__(self, instance: Model, owner: Any) -> _GT: ...
     # non-Model instances
     @overload
     def __get__(self: Self, instance: Any, owner: Any) -> Self: ...
     def deconstruct(self) -> Any: ...
@@ -261,14 +273,15 @@
         default: Any = ...,
         editable: bool = ...,
         auto_created: bool = ...,
         serialize: bool = ...,
         choices: _FieldChoices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
+        db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesT | None = ...,
     ) -> None: ...
 
 class CharField(Field[_ST, _GT]):
     _pyi_private_set_type: str | int | Combinable
@@ -291,14 +304,15 @@
         serialize: bool = ...,
         unique_for_date: str | None = ...,
         unique_for_month: str | None = ...,
         unique_for_year: str | None = ...,
         choices: _FieldChoices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
+        db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesT | None = ...,
         *,
         db_collation: str | None = ...,
     ) -> None: ...
 
@@ -319,14 +333,15 @@
         serialize: bool = ...,
         unique_for_date: str | None = ...,
         unique_for_month: str | None = ...,
         unique_for_year: str | None = ...,
         choices: _FieldChoices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
+        db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesT | None = ...,
         *,
         max_length: int | None = ...,
         db_index: bool = ...,
         allow_unicode: bool = ...,
@@ -352,14 +367,15 @@
         serialize: bool = ...,
         unique_for_date: str | None = ...,
         unique_for_month: str | None = ...,
         unique_for_year: str | None = ...,
         choices: _FieldChoices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
+        db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         auto_created: bool = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesT | None = ...,
     ) -> None: ...
 
 class TextField(Field[_ST, _GT]):
@@ -383,14 +399,15 @@
         serialize: bool = ...,
         unique_for_date: str | None = ...,
         unique_for_month: str | None = ...,
         unique_for_year: str | None = ...,
         choices: _FieldChoices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
+        db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesT | None = ...,
         *,
         db_collation: str | None = ...,
     ) -> None: ...
 
@@ -429,14 +446,15 @@
         default: Any = ...,
         editable: bool = ...,
         auto_created: bool = ...,
         serialize: bool = ...,
         choices: _FieldChoices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
+        db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesT | None = ...,
     ) -> None: ...
 
 class DateTimeCheckMixin: ...
 
@@ -462,14 +480,15 @@
         default: Any = ...,
         editable: bool = ...,
         auto_created: bool = ...,
         serialize: bool = ...,
         choices: _FieldChoices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
+        db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesT | None = ...,
     ) -> None: ...
 
 class TimeField(DateTimeCheckMixin, Field[_ST, _GT]):
     _pyi_private_set_type: str | time | real_datetime | Combinable
@@ -491,14 +510,15 @@
         default: Any = ...,
         editable: bool = ...,
         auto_created: bool = ...,
         serialize: bool = ...,
         choices: _FieldChoices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
+        db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesT | None = ...,
     ) -> None: ...
 
 class DateTimeField(DateField[_ST, _GT]):
     _pyi_private_set_type: str | real_datetime | date | Combinable
@@ -526,14 +546,15 @@
         serialize: bool = ...,
         unique_for_date: str | None = ...,
         unique_for_month: str | None = ...,
         unique_for_year: str | None = ...,
         choices: _FieldChoices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
+        db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         auto_created: bool = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesT | None = ...,
     ) -> None: ...
 
 class FilePathField(Field[_ST, _GT]):
@@ -561,14 +582,15 @@
         default: Any = ...,
         editable: bool = ...,
         auto_created: bool = ...,
         serialize: bool = ...,
         choices: _FieldChoices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
+        db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesT | None = ...,
     ) -> None: ...
 
 class BinaryField(Field[_ST, _GT]):
     _pyi_private_get_type: bytes | memoryview
```

### Comparing `django-stubs-4.2.0/django-stubs/db/models/fields/files.pyi` & `django-stubs-4.2.1/django-stubs/db/models/fields/files.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,15 @@
         serialize: bool = ...,
         unique_for_date: str | None = ...,
         unique_for_month: str | None = ...,
         unique_for_year: str | None = ...,
         choices: _FieldChoices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
+        db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesT | None = ...,
     ) -> None: ...
     # class access
     @overload
     def __get__(self, instance: None, owner: Any) -> FileDescriptor: ...
```

### Comparing `django-stubs-4.2.0/django-stubs/db/models/fields/json.pyi` & `django-stubs-4.2.1/django-stubs/db/models/fields/json.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/models/fields/mixins.pyi` & `django-stubs-4.2.1/django-stubs/db/models/fields/mixins.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/models/fields/related.pyi` & `django-stubs-4.2.1/django-stubs/db/models/fields/related.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from collections.abc import Callable, Iterable, Sequence
 from typing import Any, TypeVar, overload
 from uuid import UUID
 
-from _typeshed import Self
 from django.core import validators  # due to weird mypy.stubtest error
 from django.db.models.base import Model
 from django.db.models.expressions import Combinable
 from django.db.models.fields import Field, _AllLimitChoicesTo, _ErrorMessagesT, _FieldChoices, _LimitChoicesTo
 from django.db.models.fields.mixins import FieldCacheMixin
 from django.db.models.fields.related_descriptors import ForwardManyToOneDescriptor as ForwardManyToOneDescriptor
 from django.db.models.fields.related_descriptors import (  # noqa: F401
@@ -18,15 +17,15 @@
 from django.db.models.fields.reverse_related import ForeignObjectRel as ForeignObjectRel  # noqa: F401
 from django.db.models.fields.reverse_related import ManyToManyRel as ManyToManyRel
 from django.db.models.fields.reverse_related import ManyToOneRel as ManyToOneRel
 from django.db.models.fields.reverse_related import OneToOneRel as OneToOneRel
 from django.db.models.manager import RelatedManager
 from django.db.models.query_utils import FilteredRelation, PathInfo, Q
 from django.utils.functional import _StrOrPromise
-from typing_extensions import Literal
+from typing_extensions import Literal, Self
 
 RECURSIVE_RELATIONSHIP_CONSTANT: Literal["self"]
 
 def resolve_relation(scope_model: type[Model], relation: str | type[Model]) -> str | type[Model]: ...
 
 # __set__ value type
 _ST = TypeVar("_ST")
@@ -86,18 +85,28 @@
         default: Any = ...,
         editable: bool = ...,
         auto_created: bool = ...,
         serialize: bool = ...,
         choices: _FieldChoices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
+        db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesT | None = ...,
     ) -> None: ...
+    # class access
+    @overload
+    def __get__(self, instance: None, owner: Any) -> ForwardManyToOneDescriptor[Self]: ...
+    # Model instance access
+    @overload
+    def __get__(self, instance: Model, owner: Any) -> _GT: ...
+    # non-Model instances
+    @overload
+    def __get__(self: Self, instance: Any, owner: Any) -> Self: ...
     def resolve_related_fields(self) -> list[tuple[Field, Field]]: ...
     @property
     def related_fields(self) -> list[tuple[Field, Field]]: ...
     @property
     def reverse_related_fields(self) -> list[tuple[Field, Field]]: ...
     @property
     def local_related_fields(self) -> tuple[Field, ...]: ...
@@ -135,27 +144,19 @@
         serialize: bool = ...,
         unique_for_date: str | None = ...,
         unique_for_month: str | None = ...,
         unique_for_year: str | None = ...,
         choices: _FieldChoices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
+        db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesT | None = ...,
     ) -> None: ...
-    # class access
-    @overload
-    def __get__(self, instance: None, owner: Any) -> ForwardManyToOneDescriptor: ...
-    # Model instance access
-    @overload
-    def __get__(self, instance: Model, owner: Any) -> _GT: ...
-    # non-Model instances
-    @overload
-    def __get__(self: Self, instance: Any, owner: Any) -> Self: ...
 
 class OneToOneField(ForeignKey[_ST, _GT]):
     _pyi_private_set_type: Any | Combinable
     _pyi_private_get_type: Any
 
     remote_field: OneToOneRel
     rel_class: type[OneToOneRel]
@@ -184,21 +185,22 @@
         serialize: bool = ...,
         unique_for_date: str | None = ...,
         unique_for_month: str | None = ...,
         unique_for_year: str | None = ...,
         choices: _FieldChoices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
+        db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesT | None = ...,
     ) -> None: ...
     # class access
     @overload
-    def __get__(self, instance: None, owner: Any) -> ForwardOneToOneDescriptor: ...
+    def __get__(self, instance: None, owner: Any) -> ForwardOneToOneDescriptor[Self]: ...
     # Model instance access
     @overload
     def __get__(self, instance: Model, owner: Any) -> _GT: ...
     # non-Model instances
     @overload
     def __get__(self: Self, instance: Any, owner: Any) -> Self: ...
 
@@ -244,21 +246,22 @@
         serialize: bool = ...,
         unique_for_date: str | None = ...,
         unique_for_month: str | None = ...,
         unique_for_year: str | None = ...,
         choices: _FieldChoices | None = ...,
         help_text: _StrOrPromise = ...,
         db_column: str | None = ...,
+        db_comment: str | None = ...,
         db_tablespace: str | None = ...,
         validators: Iterable[validators._ValidatorCallable] = ...,
         error_messages: _ErrorMessagesT | None = ...,
     ) -> None: ...
     # class access
     @overload
-    def __get__(self, instance: None, owner: Any) -> ManyToManyDescriptor: ...
+    def __get__(self, instance: None, owner: Any) -> ManyToManyDescriptor[Self]: ...
     # Model instance access
     @overload
     def __get__(self, instance: Model, owner: Any) -> _GT: ...
     # non-Model instances
     @overload
     def __get__(self: Self, instance: Any, owner: Any) -> Self: ...
     def get_path_info(self, filtered_relation: FilteredRelation | None = ...) -> list[PathInfo]: ...
```

### Comparing `django-stubs-4.2.0/django-stubs/db/models/fields/related_descriptors.pyi` & `django-stubs-4.2.1/django-stubs/db/models/fields/related_descriptors.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -8,37 +8,37 @@
 from django.db.models.fields.related import ForeignKey, ManyToManyField, OneToOneField, RelatedField
 from django.db.models.fields.reverse_related import ManyToManyRel, ManyToOneRel, OneToOneRel
 from django.db.models.manager import RelatedManager
 from django.db.models.query import QuerySet
 from django.db.models.query_utils import DeferredAttribute
 
 _T = TypeVar("_T")
+_F = TypeVar("_F", bound=Field)
 
 class ForeignKeyDeferredAttribute(DeferredAttribute):
     field: RelatedField
 
-class ForwardManyToOneDescriptor:
-    field: ForeignKey
-    def __init__(self, field_with_rel: ForeignKey) -> None: ...
+class ForwardManyToOneDescriptor(Generic[_F]):
+    field: _F
+    def __init__(self, field_with_rel: _F) -> None: ...
     @property
     def RelatedObjectDoesNotExist(self) -> type[ObjectDoesNotExist]: ...
     def is_cached(self, instance: Model) -> bool: ...
     def get_queryset(self, **hints: Any) -> QuerySet: ...
     def get_prefetch_queryset(
         self, instances: list[Model], queryset: QuerySet | None = ...
     ) -> tuple[QuerySet, Callable, Callable, bool, str, bool]: ...
     def get_object(self, instance: Model) -> Model: ...
     def __get__(
         self, instance: Model | None, cls: type[Model] | None = ...
     ) -> Model | ForwardManyToOneDescriptor | None: ...
     def __set__(self, instance: Model, value: Model | None) -> None: ...
     def __reduce__(self) -> tuple[Callable, tuple[type[Model], str]]: ...
 
-class ForwardOneToOneDescriptor(ForwardManyToOneDescriptor):
-    field: OneToOneField
+class ForwardOneToOneDescriptor(ForwardManyToOneDescriptor[_F]):
     def get_object(self, instance: Model) -> Model: ...
 
 class ReverseOneToOneDescriptor:
     related: OneToOneRel
     def __init__(self, related: OneToOneRel) -> None: ...
     @property
     def RelatedObjectDoesNotExist(self) -> type[ObjectDoesNotExist]: ...
@@ -58,16 +58,16 @@
     @property
     def related_manager_cls(self) -> type[RelatedManager]: ...
     def __get__(self, instance: Model | None, cls: type[Model] | None = ...) -> ReverseManyToOneDescriptor: ...
     def __set__(self, instance: Model, value: list[Model]) -> Any: ...
 
 def create_reverse_many_to_one_manager(superclass: type, rel: Any) -> type[RelatedManager]: ...
 
-class ManyToManyDescriptor(ReverseManyToOneDescriptor):
-    field: ManyToManyField  # type: ignore[assignment]
+class ManyToManyDescriptor(ReverseManyToOneDescriptor, Generic[_F]):
+    field: _F  # type: ignore[assignment]
     rel: ManyToManyRel  # type: ignore[assignment]
     reverse: bool
     def __init__(self, rel: ManyToManyRel, reverse: bool = ...) -> None: ...
     @property
     def through(self) -> type[Model]: ...
     @property
     def related_manager_cls(self) -> type[Any]: ...  # ManyRelatedManager
```

### Comparing `django-stubs-4.2.0/django-stubs/db/models/fields/related_lookups.pyi` & `django-stubs-4.2.1/django-stubs/db/models/fields/related_lookups.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/models/fields/reverse_related.pyi` & `django-stubs-4.2.1/django-stubs/db/models/fields/reverse_related.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/models/functions/__init__.pyi` & `django-stubs-4.2.1/django-stubs/db/models/functions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/models/functions/comparison.pyi` & `django-stubs-4.2.1/django-stubs/db/models/functions/window.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,35 @@
 from typing import Any
 
-from django.db.models import Func
-from django.db.models.fields import Field
-from django.db.models.fields.json import JSONField
+from django.db import models
+from django.db.models.expressions import Func
 
-class Cast(Func):
-    def __init__(self, expression: Any, output_field: str | Field) -> None: ...
+class CumeDist(Func):
+    output_field: models.FloatField
 
-class Coalesce(Func): ...
+class DenseRank(Func):
+    output_field: models.IntegerField
 
-class Collate(Func):
-    def __init__(self, expression: Any, collation: str) -> None: ...
+class FirstValue(Func): ...
 
-class Greatest(Func): ...
+class LagLeadFunction(Func):
+    def __init__(self, expression: str | None, offset: int = ..., default: int | None = ..., **extra: Any) -> None: ...
 
-class JSONObject(Func):
-    def __init__(self, **fields: Any) -> None: ...
-    output_field: JSONField
+class Lag(LagLeadFunction): ...
+class LastValue(Func): ...
+class Lead(LagLeadFunction): ...
 
-class Least(Func): ...
-class NullIf(Func): ...
+class NthValue(Func):
+    def __init__(self, expression: str | None, nth: int = ..., **extra: Any) -> None: ...
+
+class Ntile(Func):
+    def __init__(self, num_buckets: int = ..., **extra: Any) -> None: ...
+    output_field: models.IntegerField
+
+class PercentRank(Func):
+    output_field: models.FloatField
+
+class Rank(Func):
+    output_field: models.IntegerField
+
+class RowNumber(Func):
+    output_field: models.IntegerField
```

### Comparing `django-stubs-4.2.0/django-stubs/db/models/functions/datetime.pyi` & `django-stubs-4.2.1/django-stubs/db/models/functions/datetime.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/models/functions/math.pyi` & `django-stubs-4.2.1/django-stubs/db/models/functions/math.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/models/functions/text.pyi` & `django-stubs-4.2.1/django-stubs/db/models/functions/text.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/models/indexes.pyi` & `django-stubs-4.2.1/django-stubs/db/models/indexes.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/models/lookups.pyi` & `django-stubs-4.2.1/django-stubs/db/models/lookups.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/models/manager.pyi` & `django-stubs-4.2.1/django-stubs/db/models/manager.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/models/options.pyi` & `django-stubs-4.2.1/django-stubs/db/models/options.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/models/query.pyi` & `django-stubs-4.2.1/django-stubs/db/models/query.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/models/query_utils.pyi` & `django-stubs-4.2.1/django-stubs/db/models/query_utils.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,14 @@
         reuse: set[str] | None = ...,
         summarize: bool = ...,
         for_save: bool = ...,
     ) -> WhereNode: ...
     def deconstruct(self) -> tuple[str, tuple, dict[str, str]]: ...
 
 class DeferredAttribute:
-    field_name: str
     field: Field
     def __init__(self, field: Field) -> None: ...
 
 _R = TypeVar("_R", bound=type)
 
 class RegisterLookupMixin:
     class_lookups: list[dict[Any, Any]]
```

### Comparing `django-stubs-4.2.0/django-stubs/db/models/signals.pyi` & `django-stubs-4.2.1/django-stubs/db/models/signals.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/models/sql/compiler.pyi` & `django-stubs-4.2.1/django-stubs/db/models/sql/compiler.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/models/sql/datastructures.pyi` & `django-stubs-4.2.1/django-stubs/db/models/sql/datastructures.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/models/sql/query.pyi` & `django-stubs-4.2.1/django-stubs/db/models/sql/query.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/models/sql/subqueries.pyi` & `django-stubs-4.2.1/django-stubs/db/models/sql/subqueries.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/models/sql/where.pyi` & `django-stubs-4.2.1/django-stubs/db/models/sql/where.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/db/transaction.pyi` & `django-stubs-4.2.1/django-stubs/db/transaction.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 def savepoint_rollback(sid: str, using: str | None = ...) -> None: ...
 def savepoint_commit(sid: str, using: str | None = ...) -> None: ...
 def clean_savepoints(using: str | None = ...) -> None: ...
 def get_rollback(using: str | None = ...) -> bool: ...
 def set_rollback(rollback: bool, using: str | None = ...) -> None: ...
 @contextmanager
 def mark_for_rollback_on_error(using: str | None = ...) -> Iterator[None]: ...
-def on_commit(func: Callable, using: str | None = ...) -> None: ...
+def on_commit(func: Callable[[], object], using: str | None = ..., robust: bool = ...) -> None: ...
 
 _C = TypeVar("_C", bound=Callable)  # Any callable
 
 # Don't inherit from ContextDecorator, so we can provide a more specific signature for __call__
 class Atomic:
     using: str | None
     savepoint: bool
```

### Comparing `django-stubs-4.2.0/django-stubs/db/utils.pyi` & `django-stubs-4.2.1/django-stubs/db/utils.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/dispatch/dispatcher.pyi` & `django-stubs-4.2.1/django-stubs/dispatch/dispatcher.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/forms/__init__.pyi` & `django-stubs-4.2.1/django-stubs/forms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/forms/boundfield.pyi` & `django-stubs-4.2.1/django-stubs/forms/boundfield.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/forms/fields.pyi` & `django-stubs-4.2.1/django-stubs/forms/fields.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/forms/forms.pyi` & `django-stubs-4.2.1/django-stubs/forms/forms.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/forms/formsets.pyi` & `django-stubs-4.2.1/django-stubs/forms/formsets.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/forms/models.pyi` & `django-stubs-4.2.1/django-stubs/forms/models.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/forms/renderers.pyi` & `django-stubs-4.2.1/django-stubs/forms/renderers.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/forms/utils.pyi` & `django-stubs-4.2.1/django-stubs/forms/utils.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/forms/widgets.pyi` & `django-stubs-4.2.1/django-stubs/forms/widgets.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/http/__init__.pyi` & `django-stubs-4.2.1/django-stubs/http/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/http/multipartparser.pyi` & `django-stubs-4.2.1/django-stubs/http/multipartparser.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/http/request.pyi` & `django-stubs-4.2.1/django-stubs/http/request.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/http/response.pyi` & `django-stubs-4.2.1/django-stubs/http/response.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import datetime
-from collections.abc import Iterable, Iterator
+from collections.abc import AsyncIterable, AsyncIterator, Iterable, Iterator
 from io import BytesIO
 from json import JSONEncoder
 from typing import Any, TypeVar, overload, type_check_only
 
 from django.http.cookie import SimpleCookie
 from django.utils.datastructures import CaseInsensitiveMapping, _PropertyDescriptor
 from typing_extensions import Literal
@@ -100,18 +100,24 @@
     xframe_options_exempt: bool
     def __init__(self, content: object = ..., *args: Any, **kwargs: Any) -> None: ...
     def serialize(self) -> bytes: ...
     __bytes__ = serialize
     def __iter__(self) -> Iterator[bytes]: ...
     def getvalue(self) -> bytes: ...
 
-class StreamingHttpResponse(HttpResponseBase, Iterable[bytes]):
-    streaming_content = _PropertyDescriptor[Iterable[object], Iterator[bytes]]()
-    def __init__(self, streaming_content: Iterable[object] = ..., *args: Any, **kwargs: Any) -> None: ...
+class StreamingHttpResponse(HttpResponseBase, Iterable[bytes], AsyncIterable[bytes]):
+    is_async: bool
+    streaming_content = _PropertyDescriptor[
+        Iterable[object] | AsyncIterable[object], Iterator[bytes] | AsyncIterator[bytes]
+    ]()
+    def __init__(
+        self, streaming_content: Iterable[object] | AsyncIterable[object] = ..., *args: Any, **kwargs: Any
+    ) -> None: ...
     def __iter__(self) -> Iterator[bytes]: ...
+    def __aiter__(self) -> AsyncIterator[bytes]: ...
     def getvalue(self) -> bytes: ...
 
 class FileResponse(StreamingHttpResponse):
     file_to_stream: BytesIO | None
     block_size: int
     as_attachment: bool
     filename: str
```

### Comparing `django-stubs-4.2.0/django-stubs/middleware/cache.pyi` & `django-stubs-4.2.1/django-stubs/middleware/cache.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/middleware/common.pyi` & `django-stubs-4.2.1/django-stubs/middleware/common.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/middleware/csrf.pyi` & `django-stubs-4.2.1/django-stubs/middleware/csrf.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/middleware/security.pyi` & `django-stubs-4.2.1/django-stubs/middleware/security.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/shortcuts.pyi` & `django-stubs-4.2.1/django-stubs/shortcuts.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/template/__init__.pyi` & `django-stubs-4.2.1/django-stubs/template/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/template/backends/base.pyi` & `django-stubs-4.2.1/django-stubs/template/backends/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/template/backends/django.pyi` & `django-stubs-4.2.1/django-stubs/template/backends/django.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/template/backends/jinja2.pyi` & `django-stubs-4.2.1/django-stubs/template/backends/jinja2.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/template/base.pyi` & `django-stubs-4.2.1/django-stubs/template/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/template/context.pyi` & `django-stubs-4.2.1/django-stubs/template/context.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/template/context_processors.pyi` & `django-stubs-4.2.1/django-stubs/template/context_processors.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/template/defaultfilters.pyi` & `django-stubs-4.2.1/django-stubs/template/defaultfilters.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/template/defaulttags.pyi` & `django-stubs-4.2.1/django-stubs/template/defaulttags.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/template/engine.pyi` & `django-stubs-4.2.1/django-stubs/template/engine.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/template/library.pyi` & `django-stubs-4.2.1/django-stubs/template/library.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/template/loader.pyi` & `django-stubs-4.2.1/django-stubs/template/loader.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/template/loader_tags.pyi` & `django-stubs-4.2.1/django-stubs/template/loader_tags.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/template/loaders/cached.pyi` & `django-stubs-4.2.1/django-stubs/template/loaders/cached.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/template/loaders/filesystem.pyi` & `django-stubs-4.2.1/django-stubs/template/loaders/filesystem.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/template/response.pyi` & `django-stubs-4.2.1/django-stubs/template/response.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/template/smartif.pyi` & `django-stubs-4.2.1/django-stubs/template/smartif.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/template/utils.pyi` & `django-stubs-4.2.1/django-stubs/template/utils.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/templatetags/cache.pyi` & `django-stubs-4.2.1/django-stubs/templatetags/cache.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/templatetags/i18n.pyi` & `django-stubs-4.2.1/django-stubs/templatetags/i18n.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/templatetags/static.pyi` & `django-stubs-4.2.1/django-stubs/templatetags/static.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/templatetags/tz.pyi` & `django-stubs-4.2.1/django-stubs/templatetags/tz.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/test/__init__.pyi` & `django-stubs-4.2.1/django-stubs/test/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/test/client.pyi` & `django-stubs-4.2.1/django-stubs/test/client.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/test/html.pyi` & `django-stubs-4.2.1/django-stubs/test/html.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/test/runner.pyi` & `django-stubs-4.2.1/django-stubs/test/runner.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/test/selenium.pyi` & `django-stubs-4.2.1/django-stubs/test/selenium.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/test/signals.pyi` & `django-stubs-4.2.1/django-stubs/test/signals.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/test/testcases.pyi` & `django-stubs-4.2.1/django-stubs/test/testcases.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/test/utils.pyi` & `django-stubs-4.2.1/django-stubs/test/utils.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/urls/__init__.pyi` & `django-stubs-4.2.1/django-stubs/urls/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/urls/base.pyi` & `django-stubs-4.2.1/django-stubs/urls/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/urls/conf.pyi` & `django-stubs-4.2.1/django-stubs/urls/conf.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/urls/converters.pyi` & `django-stubs-4.2.1/django-stubs/urls/converters.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/urls/resolvers.pyi` & `django-stubs-4.2.1/django-stubs/urls/resolvers.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/utils/archive.pyi` & `django-stubs-4.2.1/django-stubs/utils/archive.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/utils/autoreload.pyi` & `django-stubs-4.2.1/django-stubs/utils/autoreload.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/utils/baseconv.pyi` & `django-stubs-4.2.1/django-stubs/utils/baseconv.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/utils/cache.pyi` & `django-stubs-4.2.1/django-stubs/utils/cache.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/utils/connection.pyi` & `django-stubs-4.2.1/django-stubs/utils/connection.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/utils/crypto.pyi` & `django-stubs-4.2.1/django-stubs/utils/crypto.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/utils/datastructures.pyi` & `django-stubs-4.2.1/django-stubs/utils/datastructures.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/utils/dateformat.pyi` & `django-stubs-4.2.1/django-stubs/utils/dateformat.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/utils/dateparse.pyi` & `django-stubs-4.2.1/django-stubs/utils/dateparse.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/utils/decorators.pyi` & `django-stubs-4.2.1/django-stubs/utils/decorators.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from django.utils.deprecation import MiddlewareMixin
 from django.utils.functional import classproperty as classproperty
 from django.views.generic.base import View
 
 _T = TypeVar("_T", bound=View | Callable)  # Any callable
 _CallableType = TypeVar("_CallableType", bound=Callable)
 
-class classonlymethod(classmethod): ...
+classonlymethod = classmethod
 
 def method_decorator(decorator: Callable | Iterable[Callable], name: str = ...) -> Callable[[_T], _T]: ...
 def decorator_from_middleware_with_args(middleware_class: type) -> Callable: ...
 def decorator_from_middleware(middleware_class: type) -> Callable: ...
 def make_middleware_decorator(middleware_class: type[MiddlewareMixin]) -> Callable: ...
 
 class AsyncGetResponseCallable(Protocol):
```

### Comparing `django-stubs-4.2.0/django-stubs/utils/deprecation.pyi` & `django-stubs-4.2.1/django-stubs/utils/deprecation.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/utils/encoding.pyi` & `django-stubs-4.2.1/django-stubs/utils/encoding.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/utils/feedgenerator.pyi` & `django-stubs-4.2.1/django-stubs/utils/feedgenerator.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/utils/formats.pyi` & `django-stubs-4.2.1/django-stubs/utils/formats.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/utils/functional.pyi` & `django-stubs-4.2.1/django-stubs/utils/functional.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/utils/html.pyi` & `django-stubs-4.2.1/django-stubs/utils/html.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/utils/http.pyi` & `django-stubs-4.2.1/django-stubs/utils/http.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/utils/jslex.pyi` & `django-stubs-4.2.1/django-stubs/utils/jslex.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/utils/log.pyi` & `django-stubs-4.2.1/django-stubs/utils/log.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/utils/regex_helper.pyi` & `django-stubs-4.2.1/django-stubs/utils/regex_helper.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/utils/safestring.pyi` & `django-stubs-4.2.1/django-stubs/utils/safestring.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/utils/termcolors.pyi` & `django-stubs-4.2.1/django-stubs/utils/termcolors.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/utils/text.pyi` & `django-stubs-4.2.1/django-stubs/utils/text.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/utils/timezone.pyi` & `django-stubs-4.2.1/django-stubs/utils/timezone.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/utils/translation/__init__.pyi` & `django-stubs-4.2.1/django-stubs/utils/translation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/utils/translation/trans_null.pyi` & `django-stubs-4.2.1/django-stubs/utils/translation/trans_null.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/utils/translation/trans_real.pyi` & `django-stubs-4.2.1/django-stubs/utils/translation/trans_real.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/utils/tree.pyi` & `django-stubs-4.2.1/django-stubs/utils/tree.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/views/debug.pyi` & `django-stubs-4.2.1/django-stubs/views/debug.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/views/defaults.pyi` & `django-stubs-4.2.1/django-stubs/views/defaults.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/views/generic/__init__.pyi` & `django-stubs-4.2.1/django-stubs/views/generic/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/views/generic/base.pyi` & `django-stubs-4.2.1/django-stubs/views/generic/base.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/views/generic/dates.pyi` & `django-stubs-4.2.1/django-stubs/views/generic/dates.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/views/generic/detail.pyi` & `django-stubs-4.2.1/django-stubs/views/generic/detail.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/views/generic/edit.pyi` & `django-stubs-4.2.1/django-stubs/views/generic/edit.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/views/generic/list.pyi` & `django-stubs-4.2.1/django-stubs/views/generic/list.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django-stubs/views/i18n.pyi` & `django-stubs-4.2.1/django-stubs/views/i18n.pyi`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/django_stubs.egg-info/PKG-INFO` & `django-stubs-4.2.1/django_stubs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,38 @@
 Metadata-Version: 2.1
 Name: django-stubs
-Version: 4.2.0
+Version: 4.2.1
 Summary: Mypy stubs for Django
 Home-page: https://github.com/typeddjango/django-stubs
 Author: Maksim Kurnikov
 Author-email: maxim.kurnikov@gmail.com
 Maintainer: Marti Raudsepp
 Maintainer-email: marti@juffo.org
 License: MIT
 Project-URL: Release notes, https://github.com/typeddjango/django-stubs/releases
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: compatible-mypy
-License-File: LICENSE.txt
+License-File: LICENSE.md
 
-<img src="http://mypy-lang.org/static/mypy_light.svg" alt="mypy logo" width="300px"/>
-
-# pep484 stubs for Django
+<img src="https://raw.githubusercontent.com/typeddjango/django-stubs/master/logo.svg" alt="django-stubs">
 
 [![Build status](https://github.com/typeddjango/django-stubs/workflows/test/badge.svg?branch=master&event=push)](https://github.com/typeddjango/django-stubs/actions?query=workflow%3Atest)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Gitter](https://badges.gitter.im/mypy-django/Lobby.svg)](https://gitter.im/mypy-django/Lobby)
 [![StackOverflow](https://shields.io/badge/ask-stackoverflow-orange?logo=stackoverflow)](https://stackoverflow.com/questions/tagged/django-stubs)
 
 This package contains [type stubs](https://www.python.org/dev/peps/pep-0561/) and a custom mypy plugin to provide more precise static types and type inference for Django framework. Django uses some Python "magic" that makes having precise types for some code patterns problematic. This is why we need this project. The final goal is to be able to get precise types for most common patterns.
@@ -77,20 +73,21 @@
 
 This fully working [typed boilerplate](https://github.com/wemake-services/wemake-django-template) can serve you as an example.
 
 ## Version compatibility
 
 We rely on different `django` and `mypy` versions:
 
-| django-stubs | Mypy version | Django version | Django partial support | Python version |
-|--------------|--------------|----------------|------------------------|----------------|
-| 4.2.0        | 1.2.x        | 4.2            | 4.1, 4.0, 3.2          | 3.7 - 3.11     |
-| 1.16.0       | 1.1.x        | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
-| 1.15.0       | 1.0.x        | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
-| 1.14.0       | 0.990+       | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
+| django-stubs   | Mypy version | Django version | Django partial support | Python version |
+|----------------|--------------|----------------|------------------------|----------------|
+| 4.2.1          | 1.3.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
+| 4.2.0          | 1.2.x        | 4.2            | 4.1, 4.0, 3.2          | 3.7 - 3.11     |
+| 1.16.0         | 1.1.x        | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
+| 1.15.0         | 1.0.x        | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
+| 1.14.0         | 0.990+       | 4.1            | 4.0, 3.2               | 3.7 - 3.11     |
 
 ## Features
 
 ### Type checking of Model Meta attributes
 
 By inheriting from the `TypedModelMeta` class, you can ensure you're using correct types for
 attributes:
@@ -152,16 +149,14 @@
 
    ```python
    import django_stubs_ext
 
    django_stubs_ext.monkeypatch()
    ```
 
-   Note: This monkey patching approach will only work when using Python 3.7 and higher, when the `__class_getitem__` magic method was introduced.
-
    You can add extra types to patch with `django_stubs_ext.monkeypatch(extra_classes=[YourDesiredType])`
 
 2. You can use strings instead: `'QuerySet[MyModel]'` and `'Manager[MyModel]'`, this way it will work as a type for `mypy` and as a regular `str` in runtime.
 
 ### How can I create a HttpRequest that's guaranteed to have an authenticated user?
 
 Django's built in [`HttpRequest`](https://docs.djangoproject.com/en/4.1/ref/request-response/#django.http.HttpRequest) has the attribute `user` that resolves to the type
```

### Comparing `django-stubs-4.2.0/django_stubs.egg-info/SOURCES.txt` & `django-stubs-4.2.1/django_stubs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-LICENSE.txt
+LICENSE.md
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 django-stubs/__init__.pyi
 django-stubs/shortcuts.pyi
 django-stubs/apps/__init__.pyi
@@ -261,14 +261,15 @@
 django-stubs/contrib/postgres/fields/hstore.pyi
 django-stubs/contrib/postgres/fields/jsonb.pyi
 django-stubs/contrib/postgres/fields/ranges.pyi
 django-stubs/contrib/postgres/fields/utils.pyi
 django-stubs/contrib/postgres/forms/__init__.pyi
 django-stubs/contrib/postgres/forms/array.pyi
 django-stubs/contrib/postgres/forms/hstore.pyi
+django-stubs/contrib/postgres/forms/jsonb.pyi
 django-stubs/contrib/postgres/forms/ranges.pyi
 django-stubs/contrib/redirects/__init__.pyi
 django-stubs/contrib/redirects/admin.pyi
 django-stubs/contrib/redirects/apps.pyi
 django-stubs/contrib/redirects/middleware.pyi
 django-stubs/contrib/redirects/models.pyi
 django-stubs/contrib/redirects/migrations/__init__.pyi
@@ -357,19 +358,24 @@
 django-stubs/core/checks/security/csrf.pyi
 django-stubs/core/checks/security/sessions.pyi
 django-stubs/core/files/__init__.pyi
 django-stubs/core/files/base.pyi
 django-stubs/core/files/images.pyi
 django-stubs/core/files/locks.pyi
 django-stubs/core/files/move.pyi
-django-stubs/core/files/storage.pyi
 django-stubs/core/files/temp.pyi
 django-stubs/core/files/uploadedfile.pyi
 django-stubs/core/files/uploadhandler.pyi
 django-stubs/core/files/utils.pyi
+django-stubs/core/files/storage/__init__.pyi
+django-stubs/core/files/storage/base.pyi
+django-stubs/core/files/storage/filesystem.pyi
+django-stubs/core/files/storage/handler.pyi
+django-stubs/core/files/storage/memory.pyi
+django-stubs/core/files/storage/mixins.pyi
 django-stubs/core/handlers/__init__.pyi
 django-stubs/core/handlers/asgi.pyi
 django-stubs/core/handlers/base.pyi
 django-stubs/core/handlers/exception.pyi
 django-stubs/core/handlers/wsgi.pyi
 django-stubs/core/mail/__init__.pyi
 django-stubs/core/mail/message.pyi
```

### Comparing `django-stubs-4.2.0/mypy_django_plugin/config.py` & `django-stubs-4.2.1/mypy_django_plugin/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     import tomllib
 else:
     import tomli as tomllib
 
 INI_USAGE = """
 (config)
 ...
-[mypy.plugins.django_stubs]
+[mypy.plugins.django-stubs]
     django_settings_module: str (required)
 ...
 """
 TOML_USAGE = """
 (config)
 ...
 [tool.django-stubs]
```

### Comparing `django-stubs-4.2.0/mypy_django_plugin/django/context.py` & `django-stubs-4.2.1/mypy_django_plugin/django/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import sys
 from collections import defaultdict
 from contextlib import contextmanager
-from typing import TYPE_CHECKING, Any, Dict, Iterable, Iterator, Optional, Sequence, Set, Tuple, Type, Union
+from typing import TYPE_CHECKING, Any, Dict, Iterable, Iterator, Literal, Optional, Sequence, Set, Tuple, Type, Union
 
 from django.core.exceptions import FieldDoesNotExist, FieldError
 from django.db import models
 from django.db.models.base import Model
 from django.db.models.expressions import Expression
 from django.db.models.fields import AutoField, CharField, Field
 from django.db.models.fields.related import ForeignKey, RelatedField
@@ -16,15 +16,14 @@
 from django.utils.functional import cached_property
 from mypy.checker import TypeChecker
 from mypy.nodes import TypeInfo
 from mypy.plugin import MethodContext
 from mypy.types import AnyType, Instance
 from mypy.types import Type as MypyType
 from mypy.types import TypeOfAny, UnionType
-from typing_extensions import Literal
 
 from mypy_django_plugin.lib import fullnames, helpers
 from mypy_django_plugin.lib.fullnames import WITH_ANNOTATIONS_FULLNAME
 
 try:
     from django.contrib.postgres.fields import ArrayField
 except ImportError:
```

### Comparing `django-stubs-4.2.0/mypy_django_plugin/lib/fullnames.py` & `django-stubs-4.2.1/mypy_django_plugin/lib/fullnames.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/mypy_django_plugin/lib/helpers.py` & `django-stubs-4.2.1/mypy_django_plugin/lib/helpers.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/mypy_django_plugin/main.py` & `django-stubs-4.2.1/mypy_django_plugin/main.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/mypy_django_plugin/transformers/fields.py` & `django-stubs-4.2.1/mypy_django_plugin/transformers/fields.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/mypy_django_plugin/transformers/forms.py` & `django-stubs-4.2.1/mypy_django_plugin/transformers/forms.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/mypy_django_plugin/transformers/functional.py` & `django-stubs-4.2.1/mypy_django_plugin/transformers/functional.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/mypy_django_plugin/transformers/init_create.py` & `django-stubs-4.2.1/mypy_django_plugin/transformers/init_create.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/mypy_django_plugin/transformers/managers.py` & `django-stubs-4.2.1/mypy_django_plugin/transformers/managers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union
+from typing import Final, Optional, Union
 
 from mypy.checker import TypeChecker
 from mypy.nodes import (
     GDEF,
     CallExpr,
     Decorator,
     FuncBase,
@@ -18,15 +18,14 @@
 from mypy.plugin import AttributeContext, ClassDefContext, DynamicClassDefContext
 from mypy.semanal import SemanticAnalyzer
 from mypy.semanal_shared import has_placeholder
 from mypy.types import AnyType, CallableType, Instance, ProperType
 from mypy.types import Type as MypyType
 from mypy.types import TypeOfAny
 from mypy.typevars import fill_typevars
-from typing_extensions import Final
 
 from mypy_django_plugin.lib import fullnames, helpers
 
 MANAGER_METHODS_RETURNING_QUERYSET: Final = frozenset(
     (
         "alias",
         "all",
```

### Comparing `django-stubs-4.2.0/mypy_django_plugin/transformers/meta.py` & `django-stubs-4.2.1/mypy_django_plugin/transformers/meta.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/mypy_django_plugin/transformers/models.py` & `django-stubs-4.2.1/mypy_django_plugin/transformers/models.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/mypy_django_plugin/transformers/orm_lookups.py` & `django-stubs-4.2.1/mypy_django_plugin/transformers/orm_lookups.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/mypy_django_plugin/transformers/querysets.py` & `django-stubs-4.2.1/mypy_django_plugin/transformers/querysets.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/mypy_django_plugin/transformers/request.py` & `django-stubs-4.2.1/mypy_django_plugin/transformers/request.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/mypy_django_plugin/transformers/settings.py` & `django-stubs-4.2.1/mypy_django_plugin/transformers/settings.py`

 * *Files identical despite different names*

### Comparing `django-stubs-4.2.0/setup.py` & `django-stubs-4.2.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#!/usr/bin/env python
 import os
 from typing import List
 
 from setuptools import find_packages, setup
 
 
 def find_stub_files(name: str) -> List[str]:
@@ -16,64 +17,63 @@
     return result
 
 
 with open("README.md") as f:
     readme = f.read()
 
 dependencies = [
-    "mypy>=0.980",
+    "mypy>=1.0.0",
     "django",
-    "django-stubs-ext>=4.2.0",
+    "django-stubs-ext>=4.2.1",
     "tomli; python_version < '3.11'",
     # Types:
     "typing-extensions",
     "types-pytz",
     "types-PyYAML",
 ]
 
 extras_require = {
-    "compatible-mypy": ["mypy>=1.2.0,<1.3"],
+    "compatible-mypy": ["mypy>=1.3.0,<1.4"],
 }
 
 setup(
     name="django-stubs",
-    version="4.2.0",
+    version="4.2.1",
     description="Mypy stubs for Django",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="MIT",
+    license_files=["LICENSE.md"],
     url="https://github.com/typeddjango/django-stubs",
     author="Maksim Kurnikov",
     author_email="maxim.kurnikov@gmail.com",
     maintainer="Marti Raudsepp",
     maintainer_email="marti@juffo.org",
     py_modules=[],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=dependencies,
     extras_require=extras_require,
     packages=["django-stubs", *find_packages(exclude=["scripts"])],
     package_data={
         "django-stubs": find_stub_files("django-stubs"),
         "mypy_django_plugin": ["py.typed"],
     },
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Framework :: Django",
         "Framework :: Django :: 2.2",
         "Framework :: Django :: 3.0",
         "Framework :: Django :: 3.1",
         "Framework :: Django :: 3.2",
-        "Framework :: Django :: 4.0",
         "Framework :: Django :: 4.1",
         "Framework :: Django :: 4.2",
     ],
     project_urls={
         "Release notes": "https://github.com/typeddjango/django-stubs/releases",
     },
 )
```

### Comparing `django-stubs-4.2.0/tests/test_error_handling.py` & `django-stubs-4.2.1/tests/test_error_handling.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pytest
 
 from mypy_django_plugin.config import DjangoPluginConfig
 
 TEMPLATE = """
 (config)
 ...
-[mypy.plugins.django_stubs]
+[mypy.plugins.django-stubs]
     django_settings_module: str (required)
 ...
 (django-stubs) mypy: error: {}
 """
 
 TEMPLATE_TOML = """
 (config)
```

