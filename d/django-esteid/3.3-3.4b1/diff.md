# Comparing `tmp/django_esteid-3.3.tar.gz` & `tmp/django_esteid-3.4b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_esteid-3.3.tar", max compression
+gzip compressed data, was "django_esteid-3.4b1.tar", max compression
```

## Comparing `django_esteid-3.3.tar` & `django_esteid-3.4b1.tar`

### file list

```diff
@@ -1,85 +1,82 @@
--rw-r--r--   0        0        0      354 2023-03-07 13:21:45.275368 django_esteid-3.3/AUTHORS.md
--rw-r--r--   0        0        0     1477 2023-03-07 13:21:45.275368 django_esteid-3.3/LICENSE
--rw-r--r--   0        0        0     4901 2023-03-07 13:21:45.275368 django_esteid-3.3/README.md
--rw-r--r--   0        0        0       20 2023-03-07 13:21:45.275368 django_esteid-3.3/esteid/__init__.py
--rw-r--r--   0        0        0    16648 2023-03-07 13:21:45.275368 django_esteid-3.3/esteid/actions.py
--rw-r--r--   0        0        0     2685 2023-03-07 13:21:45.275368 django_esteid-3.3/esteid/authentication/README.md
--rw-r--r--   0        0        0      283 2023-03-07 13:21:45.275368 django_esteid-3.3/esteid/authentication/__init__.py
--rw-r--r--   0        0        0     6569 2023-03-07 13:21:45.275368 django_esteid-3.3/esteid/authentication/authenticator.py
--rw-r--r--   0        0        0      576 2023-03-07 13:21:45.275368 django_esteid-3.3/esteid/authentication/types.py
--rw-r--r--   0        0        0     3854 2023-03-07 13:21:45.275368 django_esteid-3.3/esteid/authentication/views.py
--rw-r--r--   0        0        0     6250 2023-03-07 13:21:45.275368 django_esteid-3.3/esteid/base_service.py
--rw-r--r--   0        0        0     1960 2023-03-07 13:21:45.275368 django_esteid-3.3/esteid/compat.py
--rw-r--r--   0        0        0     1912 2023-03-07 13:21:45.275368 django_esteid-3.3/esteid/constants.py
--rw-r--r--   0        0        0      410 2023-03-07 13:21:45.275368 django_esteid-3.3/esteid/context_processors.py
--rw-r--r--   0        0        0     5842 2023-03-07 13:21:45.275368 django_esteid-3.3/esteid/exceptions.py
--rw-r--r--   0        0        0       52 2023-03-07 13:21:45.275368 django_esteid-3.3/esteid/flowtest/README.md
--rw-r--r--   0        0        0        0 2023-03-07 13:21:45.275368 django_esteid-3.3/esteid/flowtest/__init__.py
--rw-r--r--   0        0        0     1155 2023-03-07 13:21:45.275368 django_esteid-3.3/esteid/flowtest/signer.py
--rw-r--r--   0        0        0     1390 2023-03-07 13:21:45.275368 django_esteid-3.3/esteid/flowtest/urls.py
--rw-r--r--   0        0        0     1938 2023-03-07 13:21:45.275368 django_esteid-3.3/esteid/flowtest/views.py
--rw-r--r--   0        0        0     1621 2023-03-07 13:21:45.275368 django_esteid-3.3/esteid/generic.py
--rw-r--r--   0        0        0     5265 2023-03-07 13:21:45.275368 django_esteid-3.3/esteid/idcard/README.md
--rw-r--r--   0        0        0      141 2023-03-07 13:21:45.275368 django_esteid-3.3/esteid/idcard/__init__.py
--rw-r--r--   0        0        0     3710 2023-03-07 13:21:45.275368 django_esteid-3.3/esteid/idcard/signer.py
--rw-r--r--   0        0        0      288 2023-03-07 13:21:45.275368 django_esteid-3.3/esteid/idcard/templates/iframe-error.html
--rw-r--r--   0        0        0      245 2023-03-07 13:21:45.275368 django_esteid-3.3/esteid/idcard/templates/iframe.html
--rw-r--r--   0        0        0     6413 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/idcard/views.py
--rw-r--r--   0        0        0      380 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2049 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1927 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/locale/et/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2743 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/locale/et/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      511 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/locale/lt/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2186 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/locale/lt/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2688 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3363 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6627 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/middleware.py
--rw-r--r--   0        0        0     4682 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/mixins.py
--rw-r--r--   0        0        0     1329 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/mobileid/README.md
--rw-r--r--   0        0        0      210 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/mobileid/__init__.py
--rw-r--r--   0        0        0     2440 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/mobileid/authenticator.py
--rw-r--r--   0        0        0    11547 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/mobileid/base.py
--rw-r--r--   0        0        0      518 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/mobileid/constants.py
--rw-r--r--   0        0        0      960 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/mobileid/i18n.py
--rw-r--r--   0        0        0     3133 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/mobileid/signer.py
--rw-r--r--   0        0        0     2083 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/mobileid/types.py
--rw-r--r--   0        0        0      960 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/mobileid/utils.py
--rw-r--r--   0        0        0     2568 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/ocsp.py
--rw-r--r--   0        0        0     1981 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/session.py
--rw-r--r--   0        0        0     4932 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/settings.py
--rw-r--r--   0        0        0    13575 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/signing/README.md
--rw-r--r--   0        0        0      294 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/signing/__init__.py
--rw-r--r--   0        0        0     9874 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/signing/signer.py
--rw-r--r--   0        0        0     2579 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/signing/types.py
--rw-r--r--   0        0        0     5865 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/signing/views.py
--rw-r--r--   0        0        0     3498 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/smartid/README.md
--rw-r--r--   0        0        0      204 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/smartid/__init__.py
--rw-r--r--   0        0        0      183 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/smartid/apps.py
--rw-r--r--   0        0        0     2253 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/smartid/authenticator.py
--rw-r--r--   0        0        0    14593 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/smartid/base.py
--rw-r--r--   0        0        0      729 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/smartid/constants.py
--rw-r--r--   0        0        0      882 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/smartid/i18n.py
--rw-r--r--   0        0        0     2986 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/smartid/signer.py
--rw-r--r--   0        0        0     1612 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/smartid/types.py
--rw-r--r--   0        0        0      727 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/smartid/utils.py
--rw-r--r--   0        0        0     5393 2023-03-07 13:21:45.279368 django_esteid-3.3/esteid/static/esteid-new/Esteid.main.js
--rw-r--r--   0        0        0    11979 2023-03-07 13:21:45.283368 django_esteid-3.3/esteid/static/esteid-new/hwcrypto.js
--rw-r--r--   0        0        0     5369 2023-03-07 13:21:45.283368 django_esteid-3.3/esteid/static/esteid-test/Esteid.main.js
--rw-r--r--   0        0        0    11979 2023-03-07 13:21:45.283368 django_esteid-3.3/esteid/static/esteid-test/hwcrypto.js
--rw-r--r--   0        0        0     3580 2023-03-07 13:21:45.283368 django_esteid-3.3/esteid/static/esteid-test/npo.js
--rw-r--r--   0        0        0    38052 2023-03-07 13:21:45.283368 django_esteid-3.3/esteid/static/esteid-test/typedarray.js
--rw-r--r--   0        0        0     1449 2023-03-07 13:21:45.283368 django_esteid-3.3/esteid/static/images/esteid/id-kaart-logo.gif
--rw-r--r--   0        0        0     1472 2023-03-07 13:21:45.283368 django_esteid-3.3/esteid/static/images/esteid/mid-logo.gif
--rw-r--r--   0        0        0     2458 2023-03-07 13:21:45.283368 django_esteid-3.3/esteid/static/images/esteid/smartID-logo-btn.png
--rw-r--r--   0        0        0     6894 2023-03-07 13:21:45.283368 django_esteid-3.3/esteid/static/images/esteid/smartID-logo.png
--rw-r--r--   0        0        0    17692 2023-03-07 13:21:45.283368 django_esteid-3.3/esteid/templates/esteid/auth-new.html
--rw-r--r--   0        0        0      320 2023-03-07 13:21:45.283368 django_esteid-3.3/esteid/templates/esteid/authenticate.html
--rw-r--r--   0        0        0    19016 2023-03-07 13:21:45.283368 django_esteid-3.3/esteid/templates/esteid/test-new.html
--rw-r--r--   0        0        0    15400 2023-03-07 13:21:45.283368 django_esteid-3.3/esteid/templates/esteid/test.html
--rw-r--r--   0        0        0    10314 2023-03-07 13:21:45.283368 django_esteid-3.3/esteid/types.py
--rw-r--r--   0        0        0     1899 2023-03-07 13:21:45.283368 django_esteid-3.3/esteid/urls.py
--rw-r--r--   0        0        0     3477 2023-03-07 13:21:45.283368 django_esteid-3.3/esteid/util.py
--rw-r--r--   0        0        0     2305 2023-03-07 13:21:45.283368 django_esteid-3.3/esteid/validators.py
--rw-r--r--   0        0        0     6326 2023-03-07 13:21:45.283368 django_esteid-3.3/esteid/views.py
--rw-r--r--   0        0        0     2629 2023-03-07 13:21:45.283368 django_esteid-3.3/pyproject.toml
--rw-r--r--   0        0        0     6476 1970-01-01 00:00:00.000000 django_esteid-3.3/PKG-INFO
+-rw-r--r--   0        0        0      354 2021-11-09 11:26:25.693390 django_esteid-3.4b1/AUTHORS.md
+-rw-r--r--   0        0        0     1477 2021-11-09 11:26:25.693390 django_esteid-3.4b1/LICENSE
+-rw-r--r--   0        0        0     4901 2021-11-15 15:18:14.832376 django_esteid-3.4b1/README.md
+-rw-r--r--   0        0        0       23 2023-06-02 10:09:24.263424 django_esteid-3.4b1/esteid/__init__.py
+-rw-r--r--   0        0        0    16980 2023-06-02 09:57:48.736038 django_esteid-3.4b1/esteid/actions.py
+-rw-r--r--   0        0        0     2685 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/authentication/README.md
+-rw-r--r--   0        0        0      283 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/authentication/__init__.py
+-rw-r--r--   0        0        0     6569 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/authentication/authenticator.py
+-rw-r--r--   0        0        0      576 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/authentication/types.py
+-rw-r--r--   0        0        0     3854 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/authentication/views.py
+-rw-r--r--   0        0        0     6250 2021-11-15 12:09:45.735139 django_esteid-3.4b1/esteid/base_service.py
+-rw-r--r--   0        0        0     1960 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/compat.py
+-rw-r--r--   0        0        0     1912 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/constants.py
+-rw-r--r--   0        0        0      410 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/context_processors.py
+-rw-r--r--   0        0        0     5842 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/exceptions.py
+-rw-r--r--   0        0        0       52 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/flowtest/README.md
+-rw-r--r--   0        0        0        0 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/flowtest/__init__.py
+-rw-r--r--   0        0        0     1155 2023-06-01 12:41:12.526823 django_esteid-3.4b1/esteid/flowtest/signer.py
+-rw-r--r--   0        0        0     1475 2023-06-02 10:16:36.944478 django_esteid-3.4b1/esteid/flowtest/urls.py
+-rw-r--r--   0        0        0     1938 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/flowtest/views.py
+-rw-r--r--   0        0        0     1621 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/generic.py
+-rw-r--r--   0        0        0     5336 2023-06-01 12:45:10.777134 django_esteid-3.4b1/esteid/idcard/README.md
+-rw-r--r--   0        0        0      141 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/idcard/__init__.py
+-rw-r--r--   0        0        0     3712 2023-06-01 13:16:41.695317 django_esteid-3.4b1/esteid/idcard/signer.py
+-rw-r--r--   0        0        0      288 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/idcard/templates/iframe-error.html
+-rw-r--r--   0        0        0      245 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/idcard/templates/iframe.html
+-rw-r--r--   0        0        0     6413 2023-06-01 12:41:27.213305 django_esteid-3.4b1/esteid/idcard/views.py
+-rw-r--r--   0        0        0      380 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2049 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1927 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/locale/et/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2743 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/locale/et/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      511 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/locale/lt/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2186 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/locale/lt/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2688 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3363 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6627 2021-11-15 14:09:18.303071 django_esteid-3.4b1/esteid/middleware.py
+-rw-r--r--   0        0        0     4682 2023-06-01 12:41:35.186538 django_esteid-3.4b1/esteid/mixins.py
+-rw-r--r--   0        0        0     1329 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/mobileid/README.md
+-rw-r--r--   0        0        0      210 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/mobileid/__init__.py
+-rw-r--r--   0        0        0     2440 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/mobileid/authenticator.py
+-rw-r--r--   0        0        0    11547 2021-11-15 12:09:45.738473 django_esteid-3.4b1/esteid/mobileid/base.py
+-rw-r--r--   0        0        0      518 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/mobileid/constants.py
+-rw-r--r--   0        0        0      960 2023-03-07 10:56:00.181576 django_esteid-3.4b1/esteid/mobileid/i18n.py
+-rw-r--r--   0        0        0     3133 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/mobileid/signer.py
+-rw-r--r--   0        0        0     2083 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/mobileid/types.py
+-rw-r--r--   0        0        0      960 2021-11-15 12:09:45.738473 django_esteid-3.4b1/esteid/mobileid/utils.py
+-rw-r--r--   0        0        0     2568 2023-03-07 11:40:15.776172 django_esteid-3.4b1/esteid/ocsp.py
+-rw-r--r--   0        0        0     1981 2021-11-15 12:09:45.738473 django_esteid-3.4b1/esteid/session.py
+-rw-r--r--   0        0        0     4932 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/settings.py
+-rw-r--r--   0        0        0    13575 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/signing/README.md
+-rw-r--r--   0        0        0      294 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/signing/__init__.py
+-rw-r--r--   0        0        0     9874 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/signing/signer.py
+-rw-r--r--   0        0        0     2579 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/signing/types.py
+-rw-r--r--   0        0        0     5865 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/signing/views.py
+-rw-r--r--   0        0        0     3498 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/smartid/README.md
+-rw-r--r--   0        0        0      204 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/smartid/__init__.py
+-rw-r--r--   0        0        0      183 2023-03-07 10:56:00.188243 django_esteid-3.4b1/esteid/smartid/apps.py
+-rw-r--r--   0        0        0     2253 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/smartid/authenticator.py
+-rw-r--r--   0        0        0    14593 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/smartid/base.py
+-rw-r--r--   0        0        0      729 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/smartid/constants.py
+-rw-r--r--   0        0        0      882 2023-03-07 10:56:00.191576 django_esteid-3.4b1/esteid/smartid/i18n.py
+-rw-r--r--   0        0        0     2986 2021-11-09 11:26:25.696724 django_esteid-3.4b1/esteid/smartid/signer.py
+-rw-r--r--   0        0        0     1612 2021-11-09 11:26:25.700057 django_esteid-3.4b1/esteid/smartid/types.py
+-rw-r--r--   0        0        0      727 2021-11-15 12:09:45.738473 django_esteid-3.4b1/esteid/smartid/utils.py
+-rw-r--r--   0        0        0    18710 2023-06-01 15:12:04.915485 django_esteid-3.4b1/esteid/static/esteid-helper/Esteid.main.web.js
+-rw-r--r--   0        0        0     9450 2023-06-01 14:18:55.478528 django_esteid-3.4b1/esteid/static/esteid-helper/Esteid.main.web.min.js
+-rw-r--r--   0        0        0    18301 2023-06-01 11:37:15.406641 django_esteid-3.4b1/esteid/static/esteid-helper/web-eid.js
+-rw-r--r--   0        0        0     1449 2021-11-09 11:26:25.700057 django_esteid-3.4b1/esteid/static/images/esteid/id-kaart-logo.gif
+-rw-r--r--   0        0        0     1472 2021-11-09 11:26:25.700057 django_esteid-3.4b1/esteid/static/images/esteid/mid-logo.gif
+-rw-r--r--   0        0        0     2458 2021-11-09 11:26:25.700057 django_esteid-3.4b1/esteid/static/images/esteid/smartID-logo-btn.png
+-rw-r--r--   0        0        0     6894 2021-11-09 11:26:25.700057 django_esteid-3.4b1/esteid/static/images/esteid/smartID-logo.png
+-rw-r--r--   0        0        0    17701 2023-06-01 13:22:35.750760 django_esteid-3.4b1/esteid/templates/esteid/auth-new.html
+-rw-r--r--   0        0        0      320 2021-11-09 11:26:25.700057 django_esteid-3.4b1/esteid/templates/esteid/authenticate.html
+-rw-r--r--   0        0        0    19018 2023-06-01 12:12:54.665282 django_esteid-3.4b1/esteid/templates/esteid/test-new.html
+-rw-r--r--   0        0        0    15435 2023-06-01 13:16:01.879157 django_esteid-3.4b1/esteid/templates/esteid/test.html
+-rw-r--r--   0        0        0    10255 2023-03-07 12:58:53.501536 django_esteid-3.4b1/esteid/types.py
+-rw-r--r--   0        0        0     1995 2023-06-02 10:16:24.981279 django_esteid-3.4b1/esteid/urls.py
+-rw-r--r--   0        0        0     3477 2023-03-07 11:38:29.734360 django_esteid-3.4b1/esteid/util.py
+-rw-r--r--   0        0        0     2305 2023-03-07 12:11:59.783677 django_esteid-3.4b1/esteid/validators.py
+-rw-r--r--   0        0        0     6326 2023-06-01 12:48:23.157992 django_esteid-3.4b1/esteid/views.py
+-rw-r--r--   0        0        0     2632 2023-06-02 10:09:33.583298 django_esteid-3.4b1/pyproject.toml
+-rw-r--r--   0        0        0     6326 1970-01-01 00:00:00.000000 django_esteid-3.4b1/PKG-INFO
```

### Comparing `django_esteid-3.3/LICENSE` & `django_esteid-3.4b1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/README.md` & `django_esteid-3.4b1/README.md`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/actions.py` & `django_esteid-3.4b1/esteid/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # pragma: no cover
+import base64
 import binascii
 import logging
 import typing
 import warnings
 from tempfile import NamedTemporaryFile
 
 from esteid_certificates import get_certificate
@@ -44,30 +45,36 @@
     def do_action(cls, view: "GenericDigitalSignViewMixin", params: dict = None, *, certificate: str = None):
         """
         The old API is to pass a dict of params (previously confusingly named `action_kwargs`),
         the keyword args are added here for clarity as to what the method accepts
 
         :param view:
         :param params:
-        :param certificate: HEX-encoded certificate from the ID card
+        :param certificate: DER-encoded certificate from the ID card
         :return:
         """
         request = view.request
         delete_esteid_session(request)
 
         if not certificate:
             certificate = (params or {}).get("certificate")
 
         if not certificate:
             return {
                 "success": False,
                 "code": "BAD_CERTIFICATE",
             }
 
-        certificate = binascii.a2b_hex(certificate)
+        try:
+            certificate = base64.b64decode(certificate)
+        except binascii.Error:
+            return {
+                "success": False,
+                "code": "BAD_CERTIFICATE",
+            }
 
         files = view.get_files()
         container_path = view.get_bdoc_container_file()
 
         if not (files or container_path):
             return {
                 "success": False,
@@ -93,28 +100,28 @@
             signed_hash=digest_hash_b64,  # we can take the hash from the signature XML, but it'd take time to compute
             temp_signature_file=temp_signature_file.name,
             temp_container_file=temp_container_file.name,
         )
 
         return {
             "success": True,
-            "digest": binascii.b2a_hex(signed_digest).decode(),
+            "digest": base64.b64encode(signed_digest).decode(),
         }
 
 
 class IdCardFinishAction(BaseAction):
     @classmethod
     def do_action(cls, view: "GenericDigitalSignViewMixin", params: dict = None, *, signature_value: str = None):
         """
         The old API is to pass a dict of params (previously confusingly named `action_kwargs`),
         the keyword args are added here for clarity as to what the method accepts
 
         :param view:
         :param params:
-        :param signature_value: a HEX encoded signature, as received from `hwcrypto.js`
+        :param signature_value: a DER encoded signature, as received from `web-eid.js`
         :return:
         """
         request = view.request
         session_data = get_esteid_session(request)
         if not session_data:
             return {
                 "success": False,
@@ -125,18 +132,25 @@
             signature_value = (params or {}).get("signature_value")
             if not signature_value:
                 return {
                     "success": False,
                     "code": "BAD_SIGNATURE",
                 }
 
-        logger.debug("Signature HEX: %s", signature_value)
+        logger.debug("Signature B64: %s", signature_value)
 
         signed_hash_b64 = session_data["signed_hash"]
-        signature_value = binascii.a2b_hex(signature_value)
+
+        try:
+            signature_value = base64.b64decode(signature_value)
+        except binascii.Error:
+            return {
+                "success": False,
+                "code": "BAD_SIGNATURE",
+            }
 
         temp_signature_file = session_data["temp_signature_file"]
         temp_container_file = session_data["temp_container_file"]
 
         with open(temp_signature_file, "rb") as f:
             xml_sig = XmlSignature(f.read())
```

### Comparing `django_esteid-3.3/esteid/authentication/README.md` & `django_esteid-3.4b1/esteid/authentication/README.md`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/authentication/authenticator.py` & `django_esteid-3.4b1/esteid/authentication/authenticator.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/authentication/types.py` & `django_esteid-3.4b1/esteid/authentication/types.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/authentication/views.py` & `django_esteid-3.4b1/esteid/authentication/views.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/base_service.py` & `django_esteid-3.4b1/esteid/base_service.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/compat.py` & `django_esteid-3.4b1/esteid/compat.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/constants.py` & `django_esteid-3.4b1/esteid/constants.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/exceptions.py` & `django_esteid-3.4b1/esteid/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/flowtest/signer.py` & `django_esteid-3.4b1/esteid/flowtest/signer.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/flowtest/urls.py` & `django_esteid-3.4b1/esteid/flowtest/urls.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-from django.urls import re_path
+try:
+    from django.urls import re_path
+except ImportError:  # noqa
+    from django.conf.urls import url as re_path
 
 from esteid.mobileid import MobileIdAuthenticator  # noqa
 from esteid.signing import Signer
 from esteid.smartid import SmartIdAuthenticator  # noqa
 
 from .views import AuthTestRestView, AuthTestView, IDCardAuthTestView, SigningTestRestView, SigningTestView
```

### Comparing `django_esteid-3.3/esteid/flowtest/views.py` & `django_esteid-3.4b1/esteid/flowtest/views.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/generic.py` & `django_esteid-3.4b1/esteid/generic.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/idcard/README.md` & `django_esteid-3.4b1/esteid/idcard/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 ## Signing with ID Card
 
 ### Process outline
 
 1. Fetch the user certificate from the ID Card
 
-   On the frontend, query the the `hwcrypto.js` API that interacts with the ID card,
+   On the frontend, query the the `web-eid.js` API that interacts with the ID card,
    to obtain the certificate that would be required for the initial XAdEs structure.  
 
 1. Initialization request to the backend 
 
    The backend creates a BDoc (Asic-E) container with files to be signed (or takes an existing container). 
    The files' digests, together with the user certificate received from the ID card on step 1,
    are embedded into a XAdEs structure which constitutes the value that is to be signed.
    This value is returned to the frontend.
    
    The container (if it is newly created), and the XAdEs structure, are stored in temporary files.
    
 1. Signature generation (frontend) 
 
-   The frontend passes the value for signing to the `hwcrypto.js` API, 
+   The frontend passes the value for signing to the `web-eid.js` API, 
    and passes on the obtained signature to the backend. 
    
 1. Finalization of the container (backend) 
 
    The backend picks up the XAdEs structure and container 
    from the temporary files created on step 2, 
    inserts the received signature into the XAdEs structure and packs it into the container.
@@ -45,14 +45,16 @@
 
 Since the previous service-based action implementation provided for a very long inheritance tree
 of action classes which all override the `do_action` method in some way but still make a call to a
 non-existent `service`, it's advised that all those "actions" be scrapped in favor of a simpler API. 
 
 ## Authentication with ID Card
 
+*TODO: Update this section based on the new id-card authentication flow*
+
 ### Process Outline
 
 The request to the client to enter PIN is initialized by a specifically configured web server,
 with an option similar to `ssl_verify_client` on nginx.
 
 On nginx, it is only possible to protect an entire `server` section with this option, which means that
 in order to keep the site generally accessible to unauthenticated clients we need to set up a separate domain
@@ -66,15 +68,15 @@
 
 Let's describe the key points of the ID card authentication process, based on the usual routine common for
 SmartID and MobileID. 
 
 The process thus should consist of the following steps:
 * While visiting the site (assuming `example.com` for this matter), the user clicks on a link to start the authentication process;
 * Instead of issuing a _start_ request to the backend (as in the usual routine), 
-  or a `hwcrypto` library call (as in the process of signing with ID card), the user is taken to a specifically configured
+  or a `web-eid` library call (as in the process of signing with ID card), the user is taken to a specifically configured
   domain (e.g. `UNIQUE.auth.example.com`) where they are asked for the ID Card's PIN code and 
   proceed to allow the site to access the certificate;
 * the certificate is validated via OCSP (see below as to why);
 * the certificate or data obtained from it is saved to the session;
 * user is redirected to the protected page on the `example.com` site.
 
 The process above is by and large impractical. One improvement that could be made to it is to use an iframe instead of
```

### Comparing `django_esteid-3.3/esteid/idcard/signer.py` & `django_esteid-3.4b1/esteid/idcard/signer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import base64
 import binascii
 import logging
 from typing import List
 
 from oscrypto.asymmetric import Certificate as OsCryptoCertificate
 from oscrypto.asymmetric import load_certificate
 
@@ -36,18 +37,18 @@
         """
         try:
             certificate_hex = initial_data["certificate"]
         except (TypeError, KeyError) as e:
             raise InvalidParameter("Missing required parameter 'certificate'", param="certificate") from e
 
         try:
-            certificate = binascii.a2b_hex(certificate_hex)
-        except (TypeError, ValueError) as e:
+            certificate = base64.b64decode(certificate_hex)
+        except binascii.Error as e:
             raise InvalidParameter(
-                "Failed to decode parameter `certificate` from hex-encoding", param="certificate"
+                "Failed to decode parameter `certificate` from DER encoding", param="certificate"
             ) from e
 
         try:
             self._certificate_handle = load_certificate(certificate)
         except ValueError as e:
             raise InvalidParameter(
                 "Failed to recognize `certificate` as a supported certificate format", param="certificate"
@@ -61,29 +62,29 @@
 
         # Note: uses default digest algorithm (sha256)
         signed_digest = xml_sig.digest()
 
         self.save_session_data(digest=signed_digest, container=container, xml_sig=xml_sig)
 
         return {
-            # hex-encoded digest to be consumed by the hwcrypto.js library
-            "digest": binascii.b2a_hex(signed_digest).decode(),
+            # hex-encoded digest to be consumed by the web-eid.js library
+            "digest": base64.b64encode(signed_digest).decode("utf-8"),
         }
 
     def finalize(self, data: dict = None) -> pyasice.Container:
         try:
             signature_value = data["signature_value"]
         except (TypeError, KeyError) as e:
             raise InvalidParameter("Missing required parameter 'signature_value'", param="signature_value") from e
 
         try:
-            signature_value = binascii.a2b_hex(signature_value)
-        except (TypeError, ValueError) as e:
+            signature_value = base64.b64decode(signature_value)
+        except binascii.Error as e:
             raise InvalidParameter(
-                "Failed to decode parameter `signature_value` from hex-encoding", param="signature_value"
+                "Failed to decode parameter `signature_value` from DER encoding", param="signature_value"
             ) from e
 
         temp_signature_file = self.session_data.temp_signature_file
         temp_container_file = self.session_data.temp_container_file
         digest = self.session_data.digest
 
         with open(temp_signature_file, "rb") as f:
```

### Comparing `django_esteid-3.3/esteid/idcard/views.py` & `django_esteid-3.4b1/esteid/idcard/views.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/locale/en/LC_MESSAGES/django.po` & `django_esteid-3.4b1/esteid/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/locale/et/LC_MESSAGES/django.mo` & `django_esteid-3.4b1/esteid/locale/et/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/locale/et/LC_MESSAGES/django.po` & `django_esteid-3.4b1/esteid/locale/et/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/locale/lt/LC_MESSAGES/django.po` & `django_esteid-3.4b1/esteid/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/locale/ru/LC_MESSAGES/django.mo` & `django_esteid-3.4b1/esteid/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/locale/ru/LC_MESSAGES/django.po` & `django_esteid-3.4b1/esteid/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/middleware.py` & `django_esteid-3.4b1/esteid/middleware.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/mixins.py` & `django_esteid-3.4b1/esteid/mixins.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/mobileid/README.md` & `django_esteid-3.4b1/esteid/mobileid/README.md`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/mobileid/authenticator.py` & `django_esteid-3.4b1/esteid/mobileid/authenticator.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/mobileid/base.py` & `django_esteid-3.4b1/esteid/mobileid/base.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/mobileid/constants.py` & `django_esteid-3.4b1/esteid/mobileid/constants.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/mobileid/i18n.py` & `django_esteid-3.4b1/esteid/mobileid/i18n.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/mobileid/signer.py` & `django_esteid-3.4b1/esteid/mobileid/signer.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/mobileid/types.py` & `django_esteid-3.4b1/esteid/mobileid/types.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/mobileid/utils.py` & `django_esteid-3.4b1/esteid/mobileid/utils.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/ocsp.py` & `django_esteid-3.4b1/esteid/ocsp.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/session.py` & `django_esteid-3.4b1/esteid/session.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/settings.py` & `django_esteid-3.4b1/esteid/settings.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/signing/README.md` & `django_esteid-3.4b1/esteid/signing/README.md`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/signing/signer.py` & `django_esteid-3.4b1/esteid/signing/signer.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/signing/types.py` & `django_esteid-3.4b1/esteid/signing/types.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/signing/views.py` & `django_esteid-3.4b1/esteid/signing/views.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/smartid/README.md` & `django_esteid-3.4b1/esteid/smartid/README.md`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/smartid/authenticator.py` & `django_esteid-3.4b1/esteid/smartid/authenticator.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/smartid/base.py` & `django_esteid-3.4b1/esteid/smartid/base.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/smartid/constants.py` & `django_esteid-3.4b1/esteid/smartid/constants.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/smartid/i18n.py` & `django_esteid-3.4b1/esteid/smartid/i18n.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/smartid/signer.py` & `django_esteid-3.4b1/esteid/smartid/signer.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/smartid/types.py` & `django_esteid-3.4b1/esteid/smartid/types.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/smartid/utils.py` & `django_esteid-3.4b1/esteid/smartid/utils.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/static/images/esteid/id-kaart-logo.gif` & `django_esteid-3.4b1/esteid/static/images/esteid/id-kaart-logo.gif`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/static/images/esteid/mid-logo.gif` & `django_esteid-3.4b1/esteid/static/images/esteid/mid-logo.gif`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/static/images/esteid/smartID-logo-btn.png` & `django_esteid-3.4b1/esteid/static/images/esteid/smartID-logo-btn.png`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/static/images/esteid/smartID-logo.png` & `django_esteid-3.4b1/esteid/static/images/esteid/smartID-logo.png`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/templates/esteid/auth-new.html` & `django_esteid-3.4b1/esteid/templates/esteid/auth-new.html`

 * *Files 1% similar despite different names*

```diff
@@ -262,16 +262,16 @@
         </div>
     </div>
 </div>
 
 <script src="//ajax.googleapis.com/ajax/libs/jquery/1.11.1/jquery.min.js"></script>
 <script src="//maxcdn.bootstrapcdn.com/bootstrap/3.3.4/js/bootstrap.min.js"></script>
 
-<script type="text/javascript" src="{% static 'esteid-new/hwcrypto.js' %}"></script>
-<script type="text/javascript" src="{% static 'esteid-new/Esteid.main.js' %}"></script>
+<script type="text/javascript" src="{% static 'esteid-helper/web-eid.js' %}"></script>
+<script type="text/javascript" src="{% static 'esteid-helper/Esteid.main.web.js' %}"></script>
 
 <script type="text/javascript">
     function startSpinner(form) {
         $("button", form).hide()
         $(".lds-dual-ring", form).css("display", "inline-block")
     }
```

### Comparing `django_esteid-3.3/esteid/templates/esteid/test-new.html` & `django_esteid-3.4b1/esteid/templates/esteid/test-new.html`

 * *Files 0% similar despite different names*

```diff
@@ -290,16 +290,17 @@
         </div>
     </div>
 </div>
 
 <script src="//ajax.googleapis.com/ajax/libs/jquery/1.11.1/jquery.min.js"></script>
 <script src="//maxcdn.bootstrapcdn.com/bootstrap/3.3.4/js/bootstrap.min.js"></script>
 
-<script type="text/javascript" src="{% static 'esteid-new/hwcrypto.js' %}"></script>
-<script type="text/javascript" src="{% static 'esteid-new/Esteid.main.js' %}"></script>
+
+<script type="text/javascript" src="{% static 'esteid-helper/web-eid.js' %}"></script>
+<script type="text/javascript" src="{% static 'esteid-helper/Esteid.main.web.js' %}"></script>
 
 <script type="text/javascript">
     function startSpinner(form) {
         $("button", form).hide()
         $(".lds-dual-ring", form).css("display", "inline-block")
     }
 
@@ -507,15 +508,15 @@
                     $('#id-modal').modal('hide')
                     onSigned()
                 },
 
                 function (res) {
                     if (res instanceof Error) {
                         console.log(res.message, res)
-                        res = manager.getError(res.message)
+                        res = manager.getError(res)
 
                         alert(res.message)
 
                         console.error('[Error code: ' + res.returnCode + '; Error: ' + res.message + ']')
                         $('#id-modal').modal('hide')
                     } else {
                         if (typeof res === 'string' || res.error_code) {
```

### Comparing `django_esteid-3.3/esteid/templates/esteid/test.html` & `django_esteid-3.4b1/esteid/templates/esteid/test.html`

 * *Files 2% similar despite different names*

```diff
@@ -217,22 +217,22 @@
         </div>
     </div>
 </div>
 
 <script src="//ajax.googleapis.com/ajax/libs/jquery/1.11.1/jquery.min.js"></script>
 <script src="//maxcdn.bootstrapcdn.com/bootstrap/3.3.4/js/bootstrap.min.js"></script>
 
-<script type="text/javascript" src="{% static 'esteid-test/hwcrypto.js' %}"></script>
-<script type="text/javascript" src="{% static 'esteid-test/Esteid.main.js' %}"></script>
+<script type="text/javascript" src="{% static 'esteid-helper/web-eid.js' %}"></script>
+<script type="text/javascript" src="{% static 'esteid-helper/Esteid.main.web.js' %}"></script>
 
 <script type="text/javascript">
     $(function () {
         var csrf_token = '{{ csrf_token }}'
         var downloadUrl = '{% url 'download_signed_container' %}'
-        var manager = new Esteid.IdentificationManager({
+        var manager = new Esteid.LegacyIdentificationManager({
             language: Esteid.Languages.ET,
 
             idEndpoints: {
                 start: '{% url 'test_id_start' %}',
                 finish: '{% url 'test_id_finish' %}',
             },
 
@@ -311,15 +311,15 @@
                             }
 
                             $('#challenge-modal').modal('hide')
                         }
                     )
 
                 }, function (res) {
-                    if (res.message) {
+                    if (res && res.message) {
                         alert('MID Response[' + res.error_code + ']: ' + res.message)
                     } else {
                         alert('Something went wrong, please try again')
                     }
                 })
         }
 
@@ -403,28 +403,28 @@
                     $('#id-modal').modal('hide')
                     onSigned()
                 },
 
                 function (res) {
                     if (res instanceof Error) {
                         console.log(res.message, res)
-                        res = manager.getError(res.message)
+                        res = manager.getError(res)
 
                         alert(res.message)
 
                         console.error('[Error code: ' + res.returnCode + '; Error: ' + res.message + ']')
                         $('#id-modal').modal('hide')
                     } else {
-                        if (typeof res === 'string' || res.error_code) {
-                            var msg = res.message !== undefined ? res.message : res
+                        if (typeof res === 'string' || (res && res.error_code)) {
+                            var msg = res && res.message !== undefined ? res.message : res
 
                             alert(msg + ', please try again')
                             $('#id-modal').modal('hide')
                         } else {
-                            console.error(res.message !== undefined ? res.message : res)
+                            console.error(res && res.message !== undefined ? res.message : res)
                             alert('Something went wrong, please refresh the page and try again')
                         }
                     }
                 }
             )
         })
```

### Comparing `django_esteid-3.3/esteid/types.py` & `django_esteid-3.4b1/esteid/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,19 +33,14 @@
 class CertificatePolicy(FromDictMixin):
     oid = attr.ib()
     url = attr.ib(default=None)
     description = attr.ib(default=None)
 
 
 @attr.s
-class CertificateIssuer(FromDictMixin):
-    pass
-
-
-@attr.s
 class Certificate(FromDictMixin):
     issuer = attr.ib()
     issuer_serial = attr.ib()
     subject = attr.ib()
     valid_from: datetime = attr.ib(converter=convert_time)
     valid_to: datetime = attr.ib(converter=convert_time)
     issuer_country = attr.ib(default=None)
```

### Comparing `django_esteid-3.3/esteid/urls.py` & `django_esteid-3.4b1/esteid/urls.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import os
 
 from django.conf import settings
 from django.conf.urls.static import static
-from django.urls import include, re_path
 from django.views.generic import TemplateView
 
 import esteid.flowtest.urls
 
+
+try:
+    from django.urls import include, re_path
+except ImportError:  # noqa
+    from django.conf.urls import include, url as re_path
+
 from .views import (
     SKTestView,
     TestDownloadContainerView,
     TestIdCardFinishView,
     TestIdCardSignView,
     TestMobileIdSignView,
     TestMobileIdStatusView,
```

### Comparing `django_esteid-3.3/esteid/util.py` & `django_esteid-3.4b1/esteid/util.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/validators.py` & `django_esteid-3.4b1/esteid/validators.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/esteid/views.py` & `django_esteid-3.4b1/esteid/views.py`

 * *Files identical despite different names*

### Comparing `django_esteid-3.3/pyproject.toml` & `django_esteid-3.4b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-esteid"
-version = "3.3"
+version = "3.4.b1"
 description = "Django-esteid is a package that provides Esteid based authentication for your Django applications."
 readme = "README.md"
 license = "BSD"
 authors = [
     "Thorgate <info@thorgate.eu>",
     "Jürno Ader <jyrno@thorgate.eu>",
     "Yuri Shatrov <yuriy@thorgate.eu>",
```

### Comparing `django_esteid-3.3/PKG-INFO` & `django_esteid-3.4b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-esteid
-Version: 3.3
+Version: 3.4b1
 Summary: Django-esteid is a package that provides Esteid based authentication for your Django applications.
 Home-page: https://github.com/thorgate/django-esteid
 License: BSD
 Keywords: esteid,django,smartid,mobile-id,idcard,asice
 Author: Thorgate
 Author-email: info@thorgate.eu
 Maintainer: Jyrno Ader
@@ -17,24 +17,21 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Django (>=1.11,!=2.1.0,!=2.1.1)
 Requires-Dist: attrs (>=19.2.0)
 Requires-Dist: backports.zoneinfo (==0.2.1) ; python_version < "3.9"
-Requires-Dist: esteid-certificates (>=1.0.0,<1.1.0)
-Requires-Dist: pyasice (>=1.0.1,<1.1.0)
+Requires-Dist: esteid-certificates (==1.0.*)
+Requires-Dist: pyasice (>=1.0.1,<1.1.dev0)
 Requires-Dist: requests (>=2.20)
 Project-URL: Repository, https://github.com/thorgate/django-esteid
 Description-Content-Type: text/markdown
 
 # django-esteid
 
 [![pypi Status](https://badge.fury.io/py/django-esteid.png)](https://badge.fury.io/py/django-esteid)
```

