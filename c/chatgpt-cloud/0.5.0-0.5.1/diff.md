# Comparing `tmp/chatgpt-cloud-0.5.0.tar.gz` & `tmp/chatgpt-cloud-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/chatgpt-cloud/chatgpt-cloud/dist/.tmp-z6mn3n76/chatgpt-cloud-0.5.0.tar", last modified: Fri Jun  2 03:59:33 2023, max compression
+gzip compressed data, was "/home/runner/work/chatgpt-cloud/chatgpt-cloud/dist/.tmp-88v2zgjn/chatgpt-cloud-0.5.1.tar", last modified: Fri Jun  2 04:39:08 2023, max compression
```

## Comparing `chatgpt-cloud-0.5.0.tar` & `chatgpt-cloud-0.5.1.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/chatgpt_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/chatgpt_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/chatgpt_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/chatgpt_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/chatgpt_cloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/
--rw-r--r--   0 runner    (1001) docker     (123)    69737 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/012ff928-bcfa62e3ac82441c.js
--rw-r--r--   0 runner    (1001) docker     (123)   262802 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/1f110208-cda4026aba1898fb.js
--rw-r--r--   0 runner    (1001) docker     (123)    16757 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/259-c6320349d8f3ff4a.js
--rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/58-87db5ef127e7d0b9.js
--rw-r--r--   0 runner    (1001) docker     (123)  1259345 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/686-7a99a2d97a992914.js
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/68a27ff6-a453fd719d5bf767.js
--rw-r--r--   0 runner    (1001) docker     (123)   337183 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/734-99309a157861fd83.js
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/bd26816a-981e1ddc27b37cc6.js
--rw-r--r--   0 runner    (1001) docker     (123)   141071 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/framework-e23f030857e925d4.js
--rw-r--r--   0 runner    (1001) docker     (123)   115058 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/main-2f10fecca4c74462.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/cancel-63cd9f049103272b.js
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/manage-6ac6d4f0510ced68.js
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/upgrade-d6b322741680e2b4.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/[pluginId]/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/[pluginId]/oauth/
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/[pluginId]/oauth/callback-389963a554a230d2.js
--rw-r--r--   0 runner    (1001) docker     (123)  1003292 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/app-878ac43f93e00b3f.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/error-c7951a77c5f4547f.js
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback-927659025ea31258.js
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback_refresh-478ebccc4055d75b.js
--rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/login-f4fdb51b436aaaf4.js
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/logout-47cc26eb7b585e67.js
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/mocked_login-d5fbb97bc5d39e59.js
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/bypass-338530f42d5b2105.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/c/
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/c/[chatId]-c0db665988dd1d67.js
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/error-433a1bbdb23dd341.js
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/index-1401d2c2b63d99cf.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/business-e449df976df219cb.js
--rw-r--r--   0 runner    (1001) docker     (123)    27863 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/success-66b11e86067b001d.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/share/
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/share/[[...shareParams]]-875a033295abd238.js
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/status-6557d60655b68492.js
--rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/webpack-c08a82b5c21eeb38.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   125366 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/css/df35a37d1f08004f.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/cx416mT2Lb0ZTj5FxFg1l/
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/cx416mT2Lb0ZTj5FxFg1l/buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/cx416mT2Lb0ZTj5FxFg1l/ssgManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/favicon-32x32.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/colfax/
--rw-r--r--   0 runner    (1001) docker     (123)    34336 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    27412 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    35956 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    28532 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    35268 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    28060 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    37480 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    29824 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/
--rw-r--r--   0 runner    (1001) docker     (123)    28076 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_AMS-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    11316 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    25324 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16780 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-BoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    26272 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-BoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16440 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    12028 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Script-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size1-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size2-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size3-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size4-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Typewriter-Regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/signifier/
--rw-r--r--   0 runner    (1001) docker     (123)    56682 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    56021 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    56456 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/signifier/signifier-light-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    53009 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/signifier/signifier-light.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/soehne/
--rw-r--r--   0 runner    (1001) docker     (123)    34084 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch-kursiv.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    33350 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    40456 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett-kursiv.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    37996 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    38746 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig-kursiv.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    35690 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    28148 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch-kursiv.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    27437 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    28285 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-halbfett.woff2
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/service-worker.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/ulp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/ulp/react-components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/
--rw-r--r--   0 runner    (1001) docker     (123)   233073 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/main.cdn.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:59:33.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/templates/chat.html
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/templates/detail.html
--rw-r--r--   0 runner    (1001) docker     (123)    17410 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/flask/templates/share.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17104 2023-06-02 03:59:22.000000 chatgpt-cloud-0.5.0/src/pandora_cloud/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/chatgpt_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/chatgpt_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/chatgpt_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/chatgpt_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/chatgpt_cloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/
+-rw-r--r--   0 runner    (1001) docker     (123)    69737 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/012ff928-bcfa62e3ac82441c.js
+-rw-r--r--   0 runner    (1001) docker     (123)   262802 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/1f110208-cda4026aba1898fb.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16757 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/259-c6320349d8f3ff4a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/58-87db5ef127e7d0b9.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1259345 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/686-7a99a2d97a992914.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/68a27ff6-a453fd719d5bf767.js
+-rw-r--r--   0 runner    (1001) docker     (123)   337152 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/734-99309a157861fd83.js
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/bd26816a-981e1ddc27b37cc6.js
+-rw-r--r--   0 runner    (1001) docker     (123)   141071 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/framework-e23f030857e925d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)   115058 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/main-2f10fecca4c74462.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/cancel-63cd9f049103272b.js
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/manage-6ac6d4f0510ced68.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/upgrade-d6b322741680e2b4.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/[pluginId]/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/[pluginId]/oauth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/[pluginId]/oauth/callback-389963a554a230d2.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1003292 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/app-878ac43f93e00b3f.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/error-c7951a77c5f4547f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback-927659025ea31258.js
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback_refresh-478ebccc4055d75b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/login-f4fdb51b436aaaf4.js
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/logout-47cc26eb7b585e67.js
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/mocked_login-d5fbb97bc5d39e59.js
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/bypass-338530f42d5b2105.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/c/
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/c/[chatId]-c0db665988dd1d67.js
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/error-433a1bbdb23dd341.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/index-1401d2c2b63d99cf.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/business-e449df976df219cb.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27863 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/success-66b11e86067b001d.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/share/
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/share/[[...shareParams]]-875a033295abd238.js
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/status-6557d60655b68492.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/webpack-c08a82b5c21eeb38.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   125366 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/css/df35a37d1f08004f.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/cx416mT2Lb0ZTj5FxFg1l/
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/cx416mT2Lb0ZTj5FxFg1l/buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/cx416mT2Lb0ZTj5FxFg1l/ssgManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/favicon-32x32.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/colfax/
+-rw-r--r--   0 runner    (1001) docker     (123)    34336 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    27412 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    35956 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    28532 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    35268 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    28060 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    37480 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    29824 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/
+-rw-r--r--   0 runner    (1001) docker     (123)    28076 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_AMS-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11316 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    25324 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16780 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-BoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    26272 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-BoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16440 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    12028 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Script-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size1-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size2-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size3-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size4-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Typewriter-Regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/signifier/
+-rw-r--r--   0 runner    (1001) docker     (123)    56682 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    56021 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    56456 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/signifier/signifier-light-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    53009 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/signifier/signifier-light.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/soehne/
+-rw-r--r--   0 runner    (1001) docker     (123)    34084 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch-kursiv.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    33350 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    40456 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett-kursiv.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    37996 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    38746 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig-kursiv.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    35690 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    28148 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch-kursiv.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    27437 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    28285 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-halbfett.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/service-worker.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/ulp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/ulp/react-components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   233073 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/main.cdn.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:39:08.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/templates/chat.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/templates/detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17410 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/flask/templates/share.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17846 2023-06-02 04:38:51.000000 chatgpt-cloud-0.5.1/src/pandora_cloud/server.py
```

### Comparing `chatgpt-cloud-0.5.0/LICENSE` & `chatgpt-cloud-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/PKG-INFO` & `chatgpt-cloud-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-cloud
-Version: 0.5.0
+Version: 0.5.1
 Summary: A package for Pandora-ChatGPT
 Home-page: https://github.com/catty223/chatgpt-cloud
 Author: Neo Peng
 Author-email: pengzhile@gmail.com
 Project-URL: Source, https://github.com/catty223/chatgpt-cloud
 Project-URL: Tracker, https://github.com/catty223/chatgpt-cloud/issues
 Keywords: OpenAI ChatGPT ChatGPT-Plus
@@ -37,8 +37,8 @@
 [![Issues](https://img.shields.io/github/issues-raw/pengzhile/pandora-cloud)](https://github.com/pengzhile/pandora-cloud/issues)
 [![Commits](https://img.shields.io/github/last-commit/pengzhile/pandora-cloud/master)](https://github.com/pengzhile/pandora-cloud/commits/master)
 [![PyPi](https://img.shields.io/pypi/v/pandora-cloud.svg)](https://pypi.python.org/pypi/pandora-cloud)
 [![Downloads](https://static.pepy.tech/badge/pandora-cloud)](https://pypi.python.org/pypi/pandora-cloud)
 
 [![PyPi workflow](https://github.com/pengzhile/pandora-cloud/actions/workflows/python-publish.yml/badge.svg)](https://github.com/pengzhile/pandora-cloud/actions/workflows/python-publish.yml)
 
-### A package for Pandora-ChatGPT.
+### A package for Pandora-ChatGPT
```

### Comparing `chatgpt-cloud-0.5.0/README.md` & `chatgpt-cloud-0.5.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,8 +4,8 @@
 [![Issues](https://img.shields.io/github/issues-raw/pengzhile/pandora-cloud)](https://github.com/pengzhile/pandora-cloud/issues)
 [![Commits](https://img.shields.io/github/last-commit/pengzhile/pandora-cloud/master)](https://github.com/pengzhile/pandora-cloud/commits/master)
 [![PyPi](https://img.shields.io/pypi/v/pandora-cloud.svg)](https://pypi.python.org/pypi/pandora-cloud)
 [![Downloads](https://static.pepy.tech/badge/pandora-cloud)](https://pypi.python.org/pypi/pandora-cloud)
 
 [![PyPi workflow](https://github.com/pengzhile/pandora-cloud/actions/workflows/python-publish.yml/badge.svg)](https://github.com/pengzhile/pandora-cloud/actions/workflows/python-publish.yml)
 
-### A package for Pandora-ChatGPT.
+### A package for Pandora-ChatGPT
```

### Comparing `chatgpt-cloud-0.5.0/chatgpt_cloud.egg-info/PKG-INFO` & `chatgpt-cloud-0.5.1/chatgpt_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-cloud
-Version: 0.5.0
+Version: 0.5.1
 Summary: A package for Pandora-ChatGPT
 Home-page: https://github.com/catty223/chatgpt-cloud
 Author: Neo Peng
 Author-email: pengzhile@gmail.com
 Project-URL: Source, https://github.com/catty223/chatgpt-cloud
 Project-URL: Tracker, https://github.com/catty223/chatgpt-cloud/issues
 Keywords: OpenAI ChatGPT ChatGPT-Plus
@@ -37,8 +37,8 @@
 [![Issues](https://img.shields.io/github/issues-raw/pengzhile/pandora-cloud)](https://github.com/pengzhile/pandora-cloud/issues)
 [![Commits](https://img.shields.io/github/last-commit/pengzhile/pandora-cloud/master)](https://github.com/pengzhile/pandora-cloud/commits/master)
 [![PyPi](https://img.shields.io/pypi/v/pandora-cloud.svg)](https://pypi.python.org/pypi/pandora-cloud)
 [![Downloads](https://static.pepy.tech/badge/pandora-cloud)](https://pypi.python.org/pypi/pandora-cloud)
 
 [![PyPi workflow](https://github.com/pengzhile/pandora-cloud/actions/workflows/python-publish.yml/badge.svg)](https://github.com/pengzhile/pandora-cloud/actions/workflows/python-publish.yml)
 
-### A package for Pandora-ChatGPT.
+### A package for Pandora-ChatGPT
```

### Comparing `chatgpt-cloud-0.5.0/chatgpt_cloud.egg-info/SOURCES.txt` & `chatgpt-cloud-0.5.1/chatgpt_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/setup.py` & `chatgpt-cloud-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/012ff928-bcfa62e3ac82441c.js` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/012ff928-bcfa62e3ac82441c.js`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/1f110208-cda4026aba1898fb.js` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/1f110208-cda4026aba1898fb.js`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/259-c6320349d8f3ff4a.js` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/259-c6320349d8f3ff4a.js`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/58-87db5ef127e7d0b9.js` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/58-87db5ef127e7d0b9.js`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/686-7a99a2d97a992914.js` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/686-7a99a2d97a992914.js`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/68a27ff6-a453fd719d5bf767.js` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/68a27ff6-a453fd719d5bf767.js`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/734-99309a157861fd83.js` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/734-99309a157861fd83.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -10995,15 +10995,15 @@
                 return lu = function() {
                     return e
                 }, e
             }
             var lc = (0, K.vU)({
                     helpAndFaq: {
                         id: "navigation.helpAndFaq",
-                        defaultMessage: "Pandora on GitHub",
+                        defaultMessage: "Powered by Tom",
                         description: "GitHub menu item"
                     },
                     confirmClearConversations: {
                         id: "navigation.confirmClearConversations",
                         defaultMessage: "Confirm clear conversations",
                         description: "Confirmation text for clearing conversations"
                     },
@@ -11182,15 +11182,15 @@
                         l(!1), a()
                     }, [a]),
                     c = oG().conversations.length > 0,
                     d = (0, P.hz)();
                 return (0, w.jsxs)("nav", {
                     children: [(0, w.jsx)(lv, {}), (0, w.jsxs)(lh, {
                         as: "a",
-                        href: "https://github.com/pengzhile/pandora",
+                        href: "https://getai.plus",
                         target: "_blank",
                         onClick: function() {
                             i(I.s6.clickFaqLink)
                         },
                         children: [(0, w.jsx)(ef.ZP, {
                             icon: X.AlO
                         }), (0, w.jsx)(et.Z, (0, b._)({}, lc.helpAndFaq))]
@@ -12561,20 +12561,20 @@
                 doNotShareSensitive: {
                     id: "thread.modal.onboarding.title",
                     defaultMessage: "Do not share sensitive materials with this application",
                     description: "Title for the onboarding warning modal"
                 },
                 freeResearchPreview: {
                     id: "thread.chatgptFreeResearchPreview",
-                    defaultMessage: "This service is not an official OpenAI service. Powered by <link>Pandora</link>",
+                    defaultMessage: "ChatGPT may produce inaccurate information about people, places, or facts. Powered by <link>Tom</link>",
                     description: "Free Research Preview disclaimer"
                 },
                 mayProduceInaccurateInformation: {
                     id: "thread.chatgptMayProduceInaccurateInformation",
-                    defaultMessage: "This service is not an official OpenAI service. Powered by <link>Pandora</link>",
+                    defaultMessage: "ChatGPT may produce inaccurate information about people, places, or facts. Powered by <link>Tom</link>",
                     description: "ChatGPT disclaimer for producing inaccurate information"
                 },
                 somethingWentWrong: {
                     id: "thread.modal.unrecoverableError.title",
                     defaultMessage: "Something went wrong",
                     description: "Title for the UnrecoverableErrorModal"
                 },
@@ -12621,30 +12621,30 @@
                 reportSharedConversation: {
                     id: "thread.reportSharedConversation",
                     defaultMessage: "Report content",
                     description: "Report shared conversation footer link text"
                 },
                 termsOfUse: {
                     id: "thread.termsOfUse",
-                    defaultMessage: "Pandora on GitHub",
+                    defaultMessage: "Powered by Tom",
                     description: "pandora footer link text"
                 },
                 privacyPolicy: {
                     id: "thread.privacyPolicy",
                     defaultMessage: "Privacy policy",
                     description: "Privacy policy footer link text"
                 }
             });
 
             function ui(e) {
                 var t = e.onClickReportSharedConversation;
                 return (0, w.jsxs)("div", {
                     className: "flex justify-center gap-3 text-gray-500",
                     children: [(0, w.jsx)("a", {
-                        href: "https://github.com/pengzhile/pandora",
+                        href: "https://getai.plus",
                         target: "_blank",
                         rel: "noreferrer",
                         children: (0, w.jsx)(et.Z, (0, b._)({}, ua.termsOfUse))
                     })]
                 })
             }
             var uo = function(e) {
@@ -13541,29 +13541,29 @@
                                                 ez(eZ), eF(!0)
                                             }
                                         }) : e3 ? (0, w.jsx)("span", {
                                             children: (0, w.jsx)(et.Z, (0, ep._)((0, b._)({}, ua.mayProduceInaccurateInformation), {
                                                 values: {
                                                     link: function(e) {
                                                         return (0, w.jsx)("a", {
-                                                            href: "https://github.com/pengzhile/pandora",
+                                                            href: "https://getai.plus",
                                                             target: "_blank",
                                                             rel: "noreferrer",
                                                             className: "underline",
                                                             children: e
                                                         })
                                                     }
                                                 }
                                             }))
                                         }) : (0, w.jsx)("span", {
                                             children: (0, w.jsx)(et.Z, (0, ep._)((0, b._)({}, ua.freeResearchPreview), {
                                                 values: {
                                                     link: function(e) {
                                                         return (0, w.jsx)("a", {
-                                                            href: "https://github.com/pengzhile/pandora",
+                                                            href: "https://getai.plus",
                                                             target: "_blank",
                                                             rel: "noreferrer",
                                                             className: "underline",
                                                             children: e
                                                         })
                                                     }
                                                 }
```

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/framework-e23f030857e925d4.js` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/framework-e23f030857e925d4.js`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/main-2f10fecca4c74462.js` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/main-2f10fecca4c74462.js`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/upgrade-d6b322741680e2b4.js` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/upgrade-d6b322741680e2b4.js`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/[pluginId]/oauth/callback-389963a554a230d2.js` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/[pluginId]/oauth/callback-389963a554a230d2.js`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/app-878ac43f93e00b3f.js` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/app-878ac43f93e00b3f.js`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/error-c7951a77c5f4547f.js` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/error-c7951a77c5f4547f.js`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback-927659025ea31258.js` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback-927659025ea31258.js`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback_refresh-478ebccc4055d75b.js` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback_refresh-478ebccc4055d75b.js`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/login-f4fdb51b436aaaf4.js` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/login-f4fdb51b436aaaf4.js`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/logout-47cc26eb7b585e67.js` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/logout-47cc26eb7b585e67.js`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/mocked_login-d5fbb97bc5d39e59.js` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/mocked_login-d5fbb97bc5d39e59.js`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/c/[chatId]-c0db665988dd1d67.js` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/c/[chatId]-c0db665988dd1d67.js`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/index-1401d2c2b63d99cf.js` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/index-1401d2c2b63d99cf.js`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/business-e449df976df219cb.js` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/business-e449df976df219cb.js`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/success-66b11e86067b001d.js` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/success-66b11e86067b001d.js`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/share/[[...shareParams]]-875a033295abd238.js` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/share/[[...shareParams]]-875a033295abd238.js`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/chunks/webpack-c08a82b5c21eeb38.js` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/chunks/webpack-c08a82b5c21eeb38.js`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/css/df35a37d1f08004f.css` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/css/df35a37d1f08004f.css`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/_next/static/cx416mT2Lb0ZTj5FxFg1l/buildManifest.js` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/_next/static/cx416mT2Lb0ZTj5FxFg1l/buildManifest.js`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/apple-touch-icon.png` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/favicon-16x16.png` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/favicon-32x32.png` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_AMS-Regular.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_AMS-Regular.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Bold.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Bold.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Regular.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Regular.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Bold.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Bold.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Regular.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Regular.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Bold.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Bold.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-BoldItalic.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Italic.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Italic.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Regular.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Regular.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-BoldItalic.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-Italic.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-Italic.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Bold.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Bold.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Italic.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Italic.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Regular.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Regular.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Script-Regular.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Script-Regular.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size1-Regular.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size1-Regular.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size2-Regular.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size2-Regular.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size3-Regular.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size3-Regular.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size4-Regular.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size4-Regular.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Typewriter-Regular.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Typewriter-Regular.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold-italic.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/signifier/signifier-light-italic.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/signifier/signifier-light-italic.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/signifier/signifier-light.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/signifier/signifier-light.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch-kursiv.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch-kursiv.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett-kursiv.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett-kursiv.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig-kursiv.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig-kursiv.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch-kursiv.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch-kursiv.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-halbfett.woff2` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-halbfett.woff2`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/service-worker.js` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/service-worker.js`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/main.cdn.min.css` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/main.cdn.min.css`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/templates/404.html` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/templates/404.html`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/templates/chat.html` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/templates/chat.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=no"/><link rel="manifest" href="/manifest.json"><meta property="og:title" content="ChatGPT"/><meta property="og:image" content="https://chat.openai.com/images/chatgpt-share-og.png"/><meta property="og:description" content="A conversational AI system that listens, learns, and challenges"/><meta property="og:url" content="https://chat.openai.com"/><title></title><meta name="next-head-count" content="8"/><link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png"/><link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png"/><link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png"/><link rel="preconnect" href="{{api_prefix|safe}}"/><link rel="preload" href="/fonts/soehne/soehne-buch.woff2" as="font" crossorigin=""/><link rel="preload" href="/fonts/soehne/soehne-halbfett.woff2" as="font" crossorigin=""/><link rel="preload" href="/fonts/soehne/soehne-mono-buch.woff2" as="font" crossorigin=""/><link rel="preload" href="/fonts/soehne/soehne-mono-halbfett.woff2" as="font" crossorigin=""/><link rel="preload" href="/_next/static/css/df35a37d1f08004f.css" as="style"/><link rel="stylesheet" href="/_next/static/css/df35a37d1f08004f.css" data-n-g=""/><noscript data-n-css=""></noscript><script>window.__pandora_sentry={{pandora_sentry|lower}};window.__api_prefix='{{api_prefix|safe}}';</script><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-c08a82b5c21eeb38.js" defer=""></script><script src="/_next/static/chunks/framework-e23f030857e925d4.js" defer=""></script><script src="/_next/static/chunks/main-2f10fecca4c74462.js" defer=""></script><script src="/_next/static/chunks/pages/app-878ac43f93e00b3f.js" defer=""></script><script src="/_next/static/chunks/bd26816a-981e1ddc27b37cc6.js" defer=""></script><script src="/_next/static/chunks/1f110208-cda4026aba1898fb.js" defer=""></script><script src="/_next/static/chunks/012ff928-bcfa62e3ac82441c.js" defer=""></script><script src="/_next/static/chunks/68a27ff6-a453fd719d5bf767.js" defer=""></script><script src="/_next/static/chunks/686-7a99a2d97a992914.js" defer=""></script><script src="/_next/static/chunks/58-87db5ef127e7d0b9.js" defer=""></script><script src="/_next/static/chunks/734-99309a157861fd83.js" defer=""></script><script src="/_next/static/chunks/pages/index-1401d2c2b63d99cf.js" defer=""></script><script src="/_next/static/cx416mT2Lb0ZTj5FxFg1l/buildManifest.js" defer=""></script><script src="/_next/static/cx416mT2Lb0ZTj5FxFg1l/ssgManifest.js" defer=""></script></head><body class="antialiased"><div id="__next"><script>!function(){try{var d=document.documentElement,c=d.classList;c.remove('light','dark');var e=localStorage.getItem('theme');if('system'===e||(!e&&true)){var t='(prefers-color-scheme: dark)',m=window.matchMedia(t);if(m.media!==t||m.matches){d.style.colorScheme = 'dark';c.add('dark')}else{d.style.colorScheme = 'light';c.add('light')}}else if(e){c.add(e|| '')}if(e==='light'||e==='dark')d.style.colorScheme=e}catch(e){}}()</script><div></div><div class="overflow-hidden w-full h-full relative flex z-0"><div class="relative flex h-full max-w-full flex-1 overflow-hidden"><div class="flex h-full max-w-full flex-1 flex-col"><main class="relative h-full w-full transition-width flex flex-col overflow-hidden items-stretch flex-1"><div class="absolute z-10 hidden flex-col gap-2 md:flex right-3 top-3"></div><div class="flex-1 overflow-hidden"></div><div class="absolute bottom-0 left-0 w-full border-t md:border-t-0 dark:border-white/20 md:border-transparent md:dark:border-transparent md:bg-vert-light-gradient bg-white dark:bg-gray-800 md:!bg-transparent dark:md:bg-vert-dark-gradient pt-2"><div class="px-3 pb-3 pt-2 text-center text-xs text-gray-600 dark:text-gray-300 md:px-4 md:pb-6 md:pt-3"><span>This service is not an official OpenAI service. Powered by <a href="https://github.com/pengzhile/pandora" target="_blank" rel="noreferrer" class="underline">Pandora</a></span></div></div></main></div></div></div><div class="absolute left-0 right-0 top-0 z-[2]"></div></div><script id="__NEXT_DATA__" type="application/json">{{props|tojson|safe}}</script><script>if('serviceWorker' in navigator){window.addEventListener('load',function(){navigator.serviceWorker.register('/service-worker.js',{scope:'/'}).then(function(reg){console.log('ServiceWorker registration successful with scope: ',reg.scope);},function(e){console.log('ServiceWorker registration failed: ',e);});});}</script></body></html>
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=no"/><link rel="manifest" href="/manifest.json"><meta property="og:title" content="ChatGPT"/><meta property="og:image" content="https://chat.openai.com/images/chatgpt-share-og.png"/><meta property="og:description" content="A conversational AI system that listens, learns, and challenges"/><meta property="og:url" content="https://chat.openai.com"/><title></title><meta name="next-head-count" content="8"/><link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png"/><link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png"/><link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png"/><link rel="preconnect" href="{{api_prefix|safe}}"/><link rel="preload" href="/fonts/soehne/soehne-buch.woff2" as="font" crossorigin=""/><link rel="preload" href="/fonts/soehne/soehne-halbfett.woff2" as="font" crossorigin=""/><link rel="preload" href="/fonts/soehne/soehne-mono-buch.woff2" as="font" crossorigin=""/><link rel="preload" href="/fonts/soehne/soehne-mono-halbfett.woff2" as="font" crossorigin=""/><link rel="preload" href="/_next/static/css/df35a37d1f08004f.css" as="style"/><link rel="stylesheet" href="/_next/static/css/df35a37d1f08004f.css" data-n-g=""/><noscript data-n-css=""></noscript><script>window.__pandora_sentry={{pandora_sentry|lower}};window.__api_prefix='{{api_prefix|safe}}';</script><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-c08a82b5c21eeb38.js" defer=""></script><script src="/_next/static/chunks/framework-e23f030857e925d4.js" defer=""></script><script src="/_next/static/chunks/main-2f10fecca4c74462.js" defer=""></script><script src="/_next/static/chunks/pages/app-878ac43f93e00b3f.js" defer=""></script><script src="/_next/static/chunks/bd26816a-981e1ddc27b37cc6.js" defer=""></script><script src="/_next/static/chunks/1f110208-cda4026aba1898fb.js" defer=""></script><script src="/_next/static/chunks/012ff928-bcfa62e3ac82441c.js" defer=""></script><script src="/_next/static/chunks/68a27ff6-a453fd719d5bf767.js" defer=""></script><script src="/_next/static/chunks/686-7a99a2d97a992914.js" defer=""></script><script src="/_next/static/chunks/58-87db5ef127e7d0b9.js" defer=""></script><script src="/_next/static/chunks/734-99309a157861fd83.js" defer=""></script><script src="/_next/static/chunks/pages/index-1401d2c2b63d99cf.js" defer=""></script><script src="/_next/static/cx416mT2Lb0ZTj5FxFg1l/buildManifest.js" defer=""></script><script src="/_next/static/cx416mT2Lb0ZTj5FxFg1l/ssgManifest.js" defer=""></script></head><body class="antialiased"><div id="__next"><script>!function(){try{var d=document.documentElement,c=d.classList;c.remove('light','dark');var e=localStorage.getItem('theme');if('system'===e||(!e&&true)){var t='(prefers-color-scheme: dark)',m=window.matchMedia(t);if(m.media!==t||m.matches){d.style.colorScheme = 'dark';c.add('dark')}else{d.style.colorScheme = 'light';c.add('light')}}else if(e){c.add(e|| '')}if(e==='light'||e==='dark')d.style.colorScheme=e}catch(e){}}()</script><div></div><div class="overflow-hidden w-full h-full relative flex z-0"><div class="relative flex h-full max-w-full flex-1 overflow-hidden"><div class="flex h-full max-w-full flex-1 flex-col"><main class="relative h-full w-full transition-width flex flex-col overflow-hidden items-stretch flex-1"><div class="absolute z-10 hidden flex-col gap-2 md:flex right-3 top-3"></div><div class="flex-1 overflow-hidden"></div><div class="absolute bottom-0 left-0 w-full border-t md:border-t-0 dark:border-white/20 md:border-transparent md:dark:border-transparent md:bg-vert-light-gradient bg-white dark:bg-gray-800 md:!bg-transparent dark:md:bg-vert-dark-gradient pt-2"><div class="px-3 pb-3 pt-2 text-center text-xs text-gray-600 dark:text-gray-300 md:px-4 md:pb-6 md:pt-3"><span>ChatGPT may produce inaccurate information about people, places, or facts. Powered by <a href="https://getai.plus" target="_blank" rel="noreferrer" class="underline">Lanny Chan</a></span></div></div></main></div></div></div><div class="absolute left-0 right-0 top-0 z-[2]"></div></div><script id="__NEXT_DATA__" type="application/json">{{props|tojson|safe}}</script><script>if('serviceWorker' in navigator){window.addEventListener('load',function(){navigator.serviceWorker.register('/service-worker.js',{scope:'/'}).then(function(reg){console.log('ServiceWorker registration successful with scope: ',reg.scope);},function(e){console.log('ServiceWorker registration failed: ',e);});});}</script></body></html>
```

#### html2text {}

```diff
@@ -1 +1,2 @@
-This service is not an official OpenAI service. Powered by Pandora
+ChatGPT may produce inaccurate information about people, places, or facts.
+Powered by Lanny_Chan
```

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/templates/detail.html` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/templates/detail.html`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/templates/login.html` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/templates/login.html`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/flask/templates/share.html` & `chatgpt-cloud-0.5.1/src/pandora_cloud/flask/templates/share.html`

 * *Files identical despite different names*

### Comparing `chatgpt-cloud-0.5.0/src/pandora_cloud/server.py` & `chatgpt-cloud-0.5.1/src/pandora_cloud/server.py`

 * *Files 7% similar despite different names*

```diff
@@ -87,29 +87,42 @@
 
         return sections[0], int(sections[1])
 
     @staticmethod
     def __set_cookie(resp, token, expires):
         resp.set_cookie('access-token', token, expires=expires, path='/', domain=None, httponly=True, samesite='Lax')
 
-    @staticmethod
-    async def __get_userinfo():
+    async def __get_userinfo(self):
         access_token = request.cookies.get('access-token')
         try:
             payload = check_access_token(access_token)
+            if True == payload:
+                ti = await self.__fetch_share_tokeninfo(access_token)
+                return False, ti['user_id'], ti['email'], access_token, {'exp': ti['expire_at']}
+
             if 'https://api.openai.com/auth' not in payload or 'https://api.openai.com/profile' not in payload:
                 raise Exception('invalid access token')
         except:
             return True, None, None, None, None
 
         user_id = payload['https://api.openai.com/auth']['user_id']
         email = payload['https://api.openai.com/profile']['email']
 
         return False, user_id, email, access_token, payload
 
+    async def __fetch_share_tokeninfo(self, share_token):
+        url = self.api_prefix + '/token/info/{}'.format(share_token)
+
+        async with httpx.AsyncClient(proxies=self.proxy, timeout=30) as client:
+            response = await client.get(url)
+            if response.status_code != 200:
+                raise Exception('failed to fetch share token info')
+
+            return response.json()
+
     async def __fetch_share_detail(self, share_id):
         url = self.api_prefix + '/api/share/{}'.format(share_id)
 
         async with httpx.AsyncClient(proxies=self.proxy, timeout=30) as client:
             response = await client.get(url)
             if response.status_code != 200:
                 raise Exception('failed to fetch share detail')
@@ -157,14 +170,17 @@
         access_token = request.form.get('access_token')
         next_url = request.form.get('next')
         error = None
 
         if access_token:
             try:
                 payload = check_access_token(access_token)
+                if True == payload:
+                    ti = await self.__fetch_share_tokeninfo(access_token)
+                    payload = {'exp': ti['expire_at']}
 
                 resp = jsonify({'code': 0, 'url': next_url if next_url else '/'})
                 self.__set_cookie(resp, access_token, payload['exp'])
 
                 return resp
             except Exception as e:
                 error = str(e)
@@ -313,15 +329,15 @@
             },
             '__N_SSP': True
         }
 
         return jsonify(props)
 
     async def share_continue_info(self, share_id):
-        err, user_id, email, access_token, _ = await self.__get_userinfo()
+        err, user_id, email, _, _ = await self.__get_userinfo()
         if err:
             return jsonify({
                 'pageProps': {
                     '__N_REDIRECT': '/auth/login?next=%2Fshare%2F{}%2Fcontinue'.format(share_id),
                     '__N_REDIRECT_STATUS': 307
                 },
                 '__N_SSP': True
```

