# Comparing `tmp/mkdocs-dsfr-0.0.3.tar.gz` & `tmp/mkdocs_dsfr-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-dsfr-0.0.3.tar", last modified: Fri Jun  2 15:46:04 2023, max compression
+gzip compressed data, was "mkdocs_dsfr-0.0.4.tar", last modified: Fri Jun  2 15:58:56 2023, max compression
```

## Comparing `mkdocs-dsfr-0.0.3.tar` & `mkdocs_dsfr-0.0.4.tar`

### file list

```diff
@@ -1,915 +1,881 @@
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.340980 mkdocs-dsfr-0.0.3/
--rw-r--r--   0 geoffrey   (501) staff       (20)     1096 2023-05-31 09:02:27.000000 mkdocs-dsfr-0.0.3/LICENSE
--rw-r--r--   0 geoffrey   (501) staff       (20)      180 2023-05-31 09:02:27.000000 mkdocs-dsfr-0.0.3/MANIFEST.in
--rw-r--r--   0 geoffrey   (501) staff       (20)      305 2023-06-02 15:46:04.340786 mkdocs-dsfr-0.0.3/PKG-INFO
--rw-r--r--   0 geoffrey   (501) staff       (20)      433 2023-06-02 15:45:48.000000 mkdocs-dsfr-0.0.3/README.md
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.112247 mkdocs-dsfr-0.0.3/dsfr/
--rw-r--r--   0 geoffrey   (501) staff       (20)        0 2023-05-31 09:02:27.000000 mkdocs-dsfr-0.0.3/dsfr/__init__.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     2851 2023-06-02 13:44:34.000000 mkdocs-dsfr-0.0.3/dsfr/base.html
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.112343 mkdocs-dsfr-0.0.3/dsfr/css/
--rw-r--r--   0 geoffrey   (501) staff       (20)     5366 2023-05-31 09:02:27.000000 mkdocs-dsfr-0.0.3/dsfr/css/theme.css
--rw-r--r--   0 geoffrey   (501) staff       (20)   516291 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/dsfr.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    68681 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/dsfr.module.min.js
--rw-r--r--   0 geoffrey   (501) staff       (20)   218391 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/dsfr.nomodule.min.js
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.113159 mkdocs-dsfr-0.0.3/dsfr/favicon/
--rw-r--r--   0 geoffrey   (501) staff       (20)     3631 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/favicon/android-chrome-192x192.png
--rw-r--r--   0 geoffrey   (501) staff       (20)     9190 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/favicon/android-chrome-512x512.png
--rw-r--r--   0 geoffrey   (501) staff       (20)     3448 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/favicon/apple-touch-icon.png
--rw-r--r--   0 geoffrey   (501) staff       (20)     7406 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/favicon/favicon.ico
--rw-r--r--   0 geoffrey   (501) staff       (20)     6360 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/favicon/favicon.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      292 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/favicon/manifest.webmanifest
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.118953 mkdocs-dsfr-0.0.3/dsfr/fonts/
--rwxr-xr-x   0 geoffrey   (501) staff       (20)    52216 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/fonts/Marianne-Bold.woff
--rwxr-xr-x   0 geoffrey   (501) staff       (20)    42092 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/fonts/Marianne-Bold.woff2
--rwxr-xr-x   0 geoffrey   (501) staff       (20)    56436 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/fonts/Marianne-Bold_Italic.woff
--rwxr-xr-x   0 geoffrey   (501) staff       (20)    45300 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/fonts/Marianne-Bold_Italic.woff2
--rwxr-xr-x   0 geoffrey   (501) staff       (20)    50440 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/fonts/Marianne-Light.woff
--rwxr-xr-x   0 geoffrey   (501) staff       (20)    41368 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/fonts/Marianne-Light.woff2
--rwxr-xr-x   0 geoffrey   (501) staff       (20)    54492 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/fonts/Marianne-Light_Italic.woff
--rwxr-xr-x   0 geoffrey   (501) staff       (20)    43916 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/fonts/Marianne-Light_Italic.woff2
--rwxr-xr-x   0 geoffrey   (501) staff       (20)    51292 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/fonts/Marianne-Medium.woff
--rwxr-xr-x   0 geoffrey   (501) staff       (20)    41940 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/fonts/Marianne-Medium.woff2
--rwxr-xr-x   0 geoffrey   (501) staff       (20)    54680 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/fonts/Marianne-Medium_Italic.woff
--rwxr-xr-x   0 geoffrey   (501) staff       (20)    44572 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/fonts/Marianne-Medium_Italic.woff2
--rwxr-xr-x   0 geoffrey   (501) staff       (20)    51140 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/fonts/Marianne-Regular.woff
--rwxr-xr-x   0 geoffrey   (501) staff       (20)    41328 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/fonts/Marianne-Regular.woff2
--rwxr-xr-x   0 geoffrey   (501) staff       (20)    54328 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/fonts/Marianne-Regular_Italic.woff
--rwxr-xr-x   0 geoffrey   (501) staff       (20)    44284 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/fonts/Marianne-Regular_Italic.woff2
--rw-r--r--   0 geoffrey   (501) staff       (20)   114508 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/fonts/Spectral-ExtraBold.woff
--rw-r--r--   0 geoffrey   (501) staff       (20)    80368 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/fonts/Spectral-ExtraBold.woff2
--rw-r--r--   0 geoffrey   (501) staff       (20)   114016 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/fonts/Spectral-Regular.woff
--rw-r--r--   0 geoffrey   (501) staff       (20)    79472 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/fonts/Spectral-Regular.woff2
--rw-r--r--   0 geoffrey   (501) staff       (20)     2819 2023-05-31 09:02:28.000000 mkdocs-dsfr-0.0.3/dsfr/footer.html
--rw-r--r--   0 geoffrey   (501) staff       (20)     2213 2023-05-31 09:02:28.000000 mkdocs-dsfr-0.0.3/dsfr/header.html
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.106367 mkdocs-dsfr-0.0.3/dsfr/icons/
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.122199 mkdocs-dsfr-0.0.3/dsfr/icons/buildings/
--rw-r--r--   0 geoffrey   (501) staff       (20)      397 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/buildings/ancient-gate-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      789 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/buildings/ancient-gate-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      280 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/buildings/ancient-pavilion-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      416 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/buildings/ancient-pavilion-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      232 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/buildings/bank-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      262 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/buildings/bank-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      204 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/buildings/building-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      225 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/buildings/building-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      316 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/buildings/community-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      388 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/buildings/community-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      232 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/buildings/government-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      227 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/buildings/government-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      209 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/buildings/home-4-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      239 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/buildings/home-4-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      212 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/buildings/hospital-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      228 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/buildings/hospital-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      224 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/buildings/hotel-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      243 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/buildings/hotel-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      437 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/buildings/store-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      546 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/buildings/store-line.svg
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.130617 mkdocs-dsfr-0.0.3/dsfr/icons/business/
--rw-r--r--   0 geoffrey   (501) staff       (20)      254 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/archive-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      288 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/archive-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      330 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/attachment-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      241 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/attachment-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      289 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/award-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      338 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/award-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      218 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/bar-chart-box-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      234 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/bar-chart-box-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      208 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/bookmark-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      242 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/bookmark-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      253 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/briefcase-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      267 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/briefcase-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      248 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/calendar-2-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      281 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/calendar-2-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      218 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/calendar-event-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      251 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/calendar-event-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      203 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/calendar-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      244 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/calendar-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      254 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/cloud-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      356 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/cloud-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      290 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/copyright-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      346 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/copyright-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      341 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/customer-service-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      375 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/customer-service-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      210 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/flag-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      255 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/flag-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      540 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/global-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      607 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/global-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      200 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/line-chart-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      218 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/line-chart-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      409 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/links-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      418 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/links-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      260 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/mail-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      247 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/mail-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      318 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/mail-open-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      359 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/mail-open-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      355 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/medal-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      389 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/medal-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      248 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/pie-chart-2-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      378 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/pie-chart-2-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      273 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/pie-chart-box-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      289 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/pie-chart-box-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      256 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/printer-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      341 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/printer-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      296 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/profil-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      312 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/profil-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      356 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/projector-2-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      350 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/projector-2-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      248 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/send-plane-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      301 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/send-plane-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      226 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/slideshow-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      241 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/slideshow-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      215 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/window-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      230 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/business/window-line.svg
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.133871 mkdocs-dsfr-0.0.3/dsfr/icons/communication/
--rw-r--r--   0 geoffrey   (501) staff       (20)      199 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/communication/chat-2-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      237 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/communication/chat-2-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      236 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/communication/chat-3-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      360 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/communication/chat-3-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      256 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/communication/chat-check-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      283 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/communication/chat-check-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      321 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/communication/chat-delete-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      348 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/communication/chat-delete-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      243 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/communication/chat-poll-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      214 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/communication/chat-poll-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      236 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/communication/discuss-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      282 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/communication/discuss-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      201 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/communication/feedback-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      229 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/communication/feedback-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      215 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/communication/message-2-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      245 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/communication/message-2-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      231 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/communication/question-answer-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      260 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/communication/question-answer-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      263 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/communication/questionnaire-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      327 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/communication/questionnaire-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      206 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/communication/video-chat-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      234 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/communication/video-chat-line.svg
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.140221 mkdocs-dsfr-0.0.3/dsfr/icons/design/
--rw-r--r--   0 geoffrey   (501) staff       (20)      318 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/ball-pen-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      372 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/ball-pen-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      252 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/brush-3-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      266 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/brush-3-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      449 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/brush-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      689 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/brush-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      195 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/contrast-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      230 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/contrast-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      173 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/crop-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      184 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/crop-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      399 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/drag-move-2-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      178 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/drag-move-2-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      153 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/drop-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      190 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/drop-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      275 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/edit-box-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      255 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/edit-box-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      206 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/edit-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      258 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/edit-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      266 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/ink-bottle-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      323 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/ink-bottle-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      241 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/layout-grid-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      232 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/layout-grid-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      401 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/mark-pen-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      503 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/mark-pen-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      292 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/paint-brush-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      305 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/paint-brush-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      339 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/paint-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      362 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/paint-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      437 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/palette-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      584 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/palette-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      386 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/pantone-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      505 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/pantone-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      389 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/pen-nib-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      510 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/pen-nib-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      254 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/pencil-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      310 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/pencil-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      234 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/pencil-ruler-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      255 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/pencil-ruler-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      302 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/sip-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      352 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/sip-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      221 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/table-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      234 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/design/table-line.svg
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.144936 mkdocs-dsfr-0.0.3/dsfr/icons/development/
--rw-r--r--   0 geoffrey   (501) staff       (20)      500 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/development/bug-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      632 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/development/bug-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      360 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/development/code-box-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      374 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/development/code-box-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      281 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/development/code-s-slash-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      197 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/development/cursor-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      283 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/development/cursor-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      307 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/development/git-branch-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      425 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/development/git-branch-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      187 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/development/git-commit-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      250 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/development/git-commit-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      330 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/development/git-merge-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      455 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/development/git-merge-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      233 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/development/git-pull-request-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      356 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/development/git-pull-request-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      294 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/development/git-repository-commits-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      320 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/development/git-repository-commits-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      285 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/development/git-repository-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      328 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/development/git-repository-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      288 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/development/git-repository-private-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      304 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/development/git-repository-private-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      260 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/development/terminal-box-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      287 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/development/terminal-box-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      186 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/development/terminal-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      230 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/development/terminal-window-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      245 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/development/terminal-window-line.svg
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.150580 mkdocs-dsfr-0.0.3/dsfr/icons/device/
--rw-r--r--   0 geoffrey   (501) staff       (20)      343 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/device/bluetooth-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      343 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/device/bluetooth-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      256 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/device/computer-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      275 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/device/computer-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      514 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/device/dashboard-3-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      552 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/device/dashboard-3-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      266 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/device/database-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      296 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/device/database-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      250 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/device/device-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      260 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/device/device-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      206 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/device/hard-drive-2-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      222 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/device/hard-drive-2-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      290 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/device/mac-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      288 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/device/mac-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      485 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/device/phone-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      719 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/device/phone-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      272 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/device/qr-code-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      315 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/device/qr-code-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      229 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/device/rss-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      230 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/device/rss-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      234 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/device/save-3-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      250 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/device/save-3-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      195 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/device/save-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      219 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/device/save-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      219 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/device/server-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      234 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/device/server-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      208 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/device/smartphone-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      224 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/device/smartphone-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      208 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/device/tablet-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      224 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/device/tablet-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      285 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/device/tv-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      304 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/device/tv-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      618 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/device/wifi-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      630 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/device/wifi-line.svg
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.154613 mkdocs-dsfr-0.0.3/dsfr/icons/document/
--rw-r--r--   0 geoffrey   (501) staff       (20)      233 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/document/article-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      249 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/document/article-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      181 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/document/book-2-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      227 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/document/book-2-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      226 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/document/booklet-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      242 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/document/booklet-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      250 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/document/clipboard-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      274 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/document/clipboard-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      317 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/document/draft-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      303 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/document/draft-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      234 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/document/file-add-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      251 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/document/file-add-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      227 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/document/file-download-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      245 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/document/file-download-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      230 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/document/file-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      225 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/document/file-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      255 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/document/file-pdf-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      273 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/document/file-pdf-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      281 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/document/file-text-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      272 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/document/file-text-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      198 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/document/folder-2-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      234 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/document/folder-2-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      262 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/document/newspaper-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      290 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/document/newspaper-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      292 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/document/survey-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      317 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/document/survey-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      217 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/document/todo-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      250 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/document/todo-line.svg
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.158511 mkdocs-dsfr-0.0.3/dsfr/icons/editor/
--rw-r--r--   0 geoffrey   (501) staff       (20)      250 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/editor/code-view.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      250 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/editor/font-size.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      314 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/editor/fr--bold.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      160 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/editor/fr--highlight.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      278 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/editor/fr--quote-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      344 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/editor/fr--quote-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      223 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/editor/h-1.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      387 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/editor/h-2.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      542 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/editor/h-3.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      268 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/editor/h-4.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      393 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/editor/h-5.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      538 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/editor/h-6.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      298 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/editor/hashtag.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      158 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/editor/italic.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      468 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/editor/link-unlink.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      408 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/editor/link.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      246 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/editor/list-ordered.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      275 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/editor/list-unordered.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      341 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/editor/question-mark.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      147 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/editor/separator.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      151 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/editor/space.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      317 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/editor/subscript.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      315 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/editor/superscript.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      263 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/editor/table-2.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      505 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/editor/translate-2.svg
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.161106 mkdocs-dsfr-0.0.3/dsfr/icons/finance/
--rw-r--r--   0 geoffrey   (501) staff       (20)      206 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/finance/bank-card-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      220 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/finance/bank-card-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      277 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/finance/coin-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      393 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/finance/gift-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      406 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/finance/gift-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      366 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/finance/money-euro-box-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      344 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/finance/money-euro-box-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      365 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/finance/money-euro-circle-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      362 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/finance/money-euro-circle-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      397 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/finance/secure-payment-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      427 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/finance/secure-payment-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      348 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/finance/shopping-bag-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      282 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/finance/shopping-bag-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      311 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/finance/shopping-cart-2-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      343 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/finance/shopping-cart-2-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      200 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/finance/trophy-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      222 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/finance/trophy-line.svg
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.173705 mkdocs-dsfr-0.0.3/dsfr/icons/health/
--rw-r--r--   0 geoffrey   (501) staff       (20)      289 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/capsule-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      379 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/capsule-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      336 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/dislike-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      543 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/dislike-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      243 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/dossier-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      265 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/dossier-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      269 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/first-aid-kit-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      283 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/first-aid-kit-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      317 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/hand-sanitizer-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      359 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/hand-sanitizer-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      258 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/health-book-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      273 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/health-book-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      209 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/heart-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      365 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/heart-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      331 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/heart-pulse-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      661 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/heart-pulse-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      476 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/lungs-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      909 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/lungs-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      241 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/medicine-bottle-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      293 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/medicine-bottle-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      395 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/mental-health-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      503 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/mental-health-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      519 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/microscope-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      618 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/microscope-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      370 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/psychotherapy-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      504 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/psychotherapy-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      181 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/pulse-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      311 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/stethoscope-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      346 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/stethoscope-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      446 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/surgical-mask-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      567 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/surgical-mask-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      466 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/syringe-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      486 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/syringe-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      237 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/test-tube-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      264 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/test-tube-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      484 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/thermometer-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      576 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/thermometer-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)     1055 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/virus-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)     1112 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/health/virus-line.svg
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.205600 mkdocs-dsfr-0.0.3/dsfr/icons/logo/
--rw-r--r--   0 geoffrey   (501) staff       (20)      552 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/chrome-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      594 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/chrome-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      591 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/edge-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      411 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/edge-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      368 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/facebook-circle-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      458 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/facebook-circle-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      708 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/firefox-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)     1003 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/firefox-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      685 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/fr--dailymotion-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      806 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/fr--dailymotion-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      561 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/fr--tiktok-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      428 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/fr--tiktok-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      790 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/github-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)     1485 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/github-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      530 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/google-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      371 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/google-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      965 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/ie-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      796 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/ie-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      917 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/instagram-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)     2014 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/instagram-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      552 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/linkedin-box-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      366 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/linkedin-box-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      948 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/mastodon-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)     1259 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/mastodon-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      202 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/npmjs-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      220 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/npmjs-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      331 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/remixicon-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      391 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/remixicon-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      972 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/safari-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      574 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/safari-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)     1133 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/slack-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      514 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/slack-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)     1494 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/snapchat-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)     1848 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/snapchat-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      398 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/telegram-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      440 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/telegram-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      332 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/twitch-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      241 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/twitch-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      586 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/twitter-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      690 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/twitter-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      726 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/vimeo-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)     1001 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/vimeo-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      178 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/vuejs-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      198 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/vuejs-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      418 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/youtube-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      899 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/logo/youtube-line.svg
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.230242 mkdocs-dsfr-0.0.3/dsfr/icons/map/
--rw-r--r--   0 geoffrey   (501) staff       (20)      385 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/anchor-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      350 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/anchor-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      359 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/bike-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      359 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/bike-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      284 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/bus-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      299 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/bus-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      372 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/car-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      387 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/car-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      317 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/caravan-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      383 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/caravan-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      253 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/charging-pile-2-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      265 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/charging-pile-2-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      246 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/compass-3-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      281 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/compass-3-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      222 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/cup-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      264 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/cup-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      945 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/earth-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      905 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/earth-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)     2305 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/france-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)     4459 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/france-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      303 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/gas-station-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      318 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/gas-station-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      179 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/goblet-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      208 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/goblet-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      214 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/map-pin-2-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      280 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/map-pin-2-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      277 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/map-pin-user-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      363 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/map-pin-user-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      378 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/motorbike-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      447 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/motorbike-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      256 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/passport-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      272 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/passport-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      221 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/restaurant-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      257 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/restaurant-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      381 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/road-map-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      405 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/road-map-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      278 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/sailboat-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      333 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/sailboat-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      580 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/ship-2-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      562 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/ship-2-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      351 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/signal-tower-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      348 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/signal-tower-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      271 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/suitcase-2-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      286 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/suitcase-2-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      374 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/taxi-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      386 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/taxi-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      251 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/train-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      293 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/map/train-line.svg
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.237629 mkdocs-dsfr-0.0.3/dsfr/icons/media/
--rw-r--r--   0 geoffrey   (501) staff       (20)      160 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/align-left.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      253 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/camera-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      311 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/camera-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      294 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/clapperboard-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      312 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/clapperboard-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      334 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/equalizer-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      505 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/equalizer-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      340 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/film-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      355 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/film-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      184 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/fullscreen-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      388 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/gallery-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      466 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/gallery-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      261 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/headphone-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      300 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/headphone-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      394 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/image-add-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      316 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/image-add-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      398 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/image-edit-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      415 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/image-edit-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      307 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/image-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      334 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/image-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      394 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/live-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      408 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/live-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      269 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/mic-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      320 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/mic-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      158 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/music-2-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      226 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/music-2-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      154 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/notification-3-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      208 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/notification-3-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      201 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/pause-circle-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      236 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/pause-circle-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      281 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/play-circle-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      313 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/play-circle-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      186 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/stop-circle-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      221 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/stop-circle-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      403 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/volume-down-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      489 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/volume-down-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      407 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/volume-mute-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      490 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/volume-mute-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      551 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/volume-up-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      630 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/media/volume-up-line.svg
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.242180 mkdocs-dsfr-0.0.3/dsfr/icons/others/
--rw-r--r--   0 geoffrey   (501) staff       (20)      334 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/others/leaf-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      467 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/others/leaf-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      253 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/others/lightbulb-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      406 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/others/lightbulb-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      277 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/others/plant-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      362 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/others/plant-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      573 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/others/recycle-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      558 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/others/recycle-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      454 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/others/scales-3-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      552 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/others/scales-3-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      258 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/others/seedling-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      326 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/others/seedling-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      232 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/others/umbrella-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      315 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/others/umbrella-line.svg
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.277846 mkdocs-dsfr-0.0.3/dsfr/icons/system/
--rw-r--r--   0 geoffrey   (501) staff       (20)      209 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/add-circle-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      260 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/add-circle-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      136 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/add-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      319 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/alarm-warning-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      360 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/alarm-warning-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      224 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/alert-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      257 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/alert-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      127 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/arrow-down-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      188 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/arrow-down-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      120 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/arrow-down-s-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      173 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/arrow-down-s-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      159 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/arrow-go-back-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      213 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/arrow-go-back-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      161 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/arrow-go-forward-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      218 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/arrow-go-forward-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      128 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/arrow-left-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      184 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/arrow-left-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      119 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/arrow-left-s-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      173 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/arrow-left-s-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      128 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/arrow-right-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      189 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/arrow-right-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      118 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/arrow-right-s-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      175 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/arrow-right-s-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      197 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/arrow-right-up-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      129 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/arrow-up-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      186 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/arrow-up-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      117 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/arrow-up-s-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      173 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/arrow-up-s-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      177 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/check-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      252 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/checkbox-circle-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      288 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/checkbox-circle-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      252 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/checkbox-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      288 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/checkbox-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      321 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/close-circle-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      342 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/close-circle-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      210 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/close-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      189 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/delete-bin-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      203 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/delete-bin-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      142 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/download-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      198 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/download-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      203 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/error-warning-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      238 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/error-warning-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      228 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/external-link-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      230 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/external-link-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      281 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/eye-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      380 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/eye-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      481 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/eye-off-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      678 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/eye-off-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      136 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/filter-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      187 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/filter-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      196 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/fr--arrow-left-s-first-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      197 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/fr--arrow-left-s-line-double.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      377 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/fr--arrow-right-down-circle-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      201 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/fr--arrow-right-s-last-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      201 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/fr--arrow-right-s-line-double.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      377 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/fr--arrow-right-up-circle-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      327 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/fr--capslock-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      329 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/fr--equal-circle-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      260 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/fr--error-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      309 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/fr--error-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      237 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/fr--info-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      328 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/fr--info-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      253 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/fr--success-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      289 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/fr--success-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      482 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/fr--theme-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      225 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/fr--warning-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      258 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/fr--warning-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      205 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/information-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      239 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/information-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      238 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/lock-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      252 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/lock-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      252 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/lock-unlock-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      268 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/lock-unlock-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      197 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/logout-box-r-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      219 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/logout-box-r-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      145 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/menu-2-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      145 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/menu-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      248 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/more-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      348 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/more-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      220 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/notification-badge-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      288 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/notification-badge-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      311 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/question-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      325 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/question-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      280 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/refresh-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      244 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/refresh-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      247 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/search-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      382 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/search-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      864 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/settings-5-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)     1599 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/settings-5-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      241 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/shield-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      332 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/shield-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      217 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/star-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      333 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/star-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      203 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/star-s-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      325 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/star-s-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      117 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/subtract-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      341 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/thumb-down-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      442 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/thumb-down-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      340 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/thumb-up-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      459 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/thumb-up-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      193 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/time-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      226 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/time-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      201 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/timer-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      236 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/timer-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      180 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/upload-2-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      180 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/upload-2-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      144 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/upload-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      206 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/upload-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      279 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/zoom-in-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      407 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/zoom-in-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      260 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/zoom-out-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      388 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/system/zoom-out-line.svg
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.281807 mkdocs-dsfr-0.0.3/dsfr/icons/user/
--rw-r--r--   0 geoffrey   (501) staff       (20)      337 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/user/account-circle-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      462 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/user/account-circle-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      383 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/user/account-pin-circle-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      575 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/user/account-pin-circle-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      279 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/user/admin-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      349 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/user/admin-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      357 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/user/group-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      462 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/user/group-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      279 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/user/parent-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      413 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/user/parent-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      424 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/user/team-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      750 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/user/team-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      235 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/user/user-add-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      316 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/user/user-add-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      186 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/user/user-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      314 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/user/user-heart-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      439 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/user/user-heart-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      275 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/user/user-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      314 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/user/user-search-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      384 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/user/user-search-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      529 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/user/user-setting-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      462 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/user/user-setting-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      298 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/user/user-star-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      367 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/user/user-star-line.svg
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.283717 mkdocs-dsfr-0.0.3/dsfr/icons/weather/
--rw-r--r--   0 geoffrey   (501) staff       (20)      167 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/weather/cloudy-2-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      291 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/weather/cloudy-2-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      128 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/weather/flashlight-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      172 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/weather/flashlight-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      226 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/weather/moon-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      286 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/weather/moon-line.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      449 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/weather/sun-fill.svg
--rw-r--r--   0 geoffrey   (501) staff       (20)      482 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/icons/weather/sun-line.svg
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.285121 mkdocs-dsfr-0.0.3/dsfr/js/
--rw-r--r--   0 geoffrey   (501) staff       (20)     1221 2023-05-31 09:02:28.000000 mkdocs-dsfr-0.0.3/dsfr/js/base.js
--rw-r--r--   0 geoffrey   (501) staff       (20)    58073 2023-05-31 09:02:28.000000 mkdocs-dsfr-0.0.3/dsfr/js/bootstrap.min.js
--rw-r--r--   0 geoffrey   (501) staff       (20)    93107 2023-05-31 09:02:28.000000 mkdocs-dsfr-0.0.3/dsfr/js/jquery-1.10.2.min.js
--rw-r--r--   0 geoffrey   (501) staff       (20)     1553 2023-05-31 09:02:28.000000 mkdocs-dsfr-0.0.3/dsfr/lateral.html
--rw-r--r--   0 geoffrey   (501) staff       (20)       25 2023-05-31 09:02:28.000000 mkdocs-dsfr-0.0.3/dsfr/main.html
--rw-r--r--   0 geoffrey   (501) staff       (20)     1068 2023-05-31 09:02:28.000000 mkdocs-dsfr-0.0.3/dsfr/nav.html
--rw-r--r--   0 geoffrey   (501) staff       (20)      743 2023-05-31 09:02:28.000000 mkdocs-dsfr-0.0.3/dsfr/prev-next-nav.html
--rw-r--r--   0 geoffrey   (501) staff       (20)      575 2023-05-31 09:02:28.000000 mkdocs-dsfr-0.0.3/dsfr/search.html
--rw-r--r--   0 geoffrey   (501) staff       (20)        0 2023-05-31 09:05:29.000000 mkdocs-dsfr-0.0.3/dsfr/tabs.html
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.106530 mkdocs-dsfr-0.0.3/dsfr/utility/
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.292916 mkdocs-dsfr-0.0.3/dsfr/utility/icons/
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.295932 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-buildings/
--rw-r--r--   0 geoffrey   (501) staff       (20)     8218 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-buildings/icons-buildings.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    18287 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-buildings/icons-buildings.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     3542 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-buildings/icons-buildings.legacy.css
--rw-r--r--   0 geoffrey   (501) staff       (20)     8457 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-buildings/icons-buildings.legacy.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     3036 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-buildings/icons-buildings.legacy.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)     8332 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-buildings/icons-buildings.legacy.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     4916 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-buildings/icons-buildings.main.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    12037 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-buildings/icons-buildings.main.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     4370 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-buildings/icons-buildings.main.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    11358 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-buildings/icons-buildings.main.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     7178 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-buildings/icons-buildings.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    17475 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-buildings/icons-buildings.min.css.map
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.300536 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-business/
--rw-r--r--   0 geoffrey   (501) staff       (20)    22912 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-business/icons-business.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    36228 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-business/icons-business.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     9504 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-business/icons-business.legacy.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    15589 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-business/icons-business.legacy.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     8088 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-business/icons-business.legacy.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    15215 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-business/icons-business.legacy.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)    13648 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-business/icons-business.main.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    22829 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-business/icons-business.main.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)    12243 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-business/icons-business.main.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    21852 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-business/icons-business.main.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)    20103 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-business/icons-business.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    34868 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-business/icons-business.min.css.map
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.303072 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-communication/
--rw-r--r--   0 geoffrey   (501) staff       (20)     8770 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-communication/icons-communication.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    18782 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-communication/icons-communication.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     3786 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-communication/icons-communication.legacy.css
--rw-r--r--   0 geoffrey   (501) staff       (20)     8627 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-communication/icons-communication.legacy.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     3272 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-communication/icons-communication.legacy.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)     8500 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-communication/icons-communication.legacy.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     5224 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-communication/icons-communication.main.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    12366 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-communication/icons-communication.main.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     4674 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-communication/icons-communication.main.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    11670 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-communication/icons-communication.main.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     7718 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-communication/icons-communication.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    17951 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-communication/icons-communication.min.css.map
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.305493 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-design/
--rw-r--r--   0 geoffrey   (501) staff       (20)    15237 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-design/icons-design.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    26942 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-design/icons-design.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     6494 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-design/icons-design.legacy.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    12000 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-design/icons-design.legacy.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     5504 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-design/icons-design.legacy.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    11743 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-design/icons-design.legacy.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     8983 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-design/icons-design.main.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    17146 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-design/icons-design.main.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     8000 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-design/icons-design.main.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    16324 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-design/icons-design.main.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)    13276 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-design/icons-design.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    25855 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-design/icons-design.min.css.map
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.309653 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-development/
--rw-r--r--   0 geoffrey   (501) staff       (20)    10584 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-development/icons-development.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    20888 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-development/icons-development.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     4556 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-development/icons-development.legacy.css
--rw-r--r--   0 geoffrey   (501) staff       (20)     9503 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-development/icons-development.legacy.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     3954 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-development/icons-development.legacy.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)     9352 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-development/icons-development.legacy.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     6268 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-development/icons-development.main.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    13594 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-development/icons-development.main.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     5638 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-development/icons-development.main.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    12876 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-development/icons-development.main.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     9364 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-development/icons-development.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    20011 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-development/icons-development.min.css.map
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.313002 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-device/
--rw-r--r--   0 geoffrey   (501) staff       (20)    13498 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-device/icons-device.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    24915 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-device/icons-device.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     5696 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-device/icons-device.legacy.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    11099 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-device/icons-device.legacy.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     4810 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-device/icons-device.legacy.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    10870 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-device/icons-device.legacy.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     8042 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-device/icons-device.main.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    16020 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-device/icons-device.main.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     7132 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-device/icons-device.main.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    15219 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-device/icons-device.main.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)    11714 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-device/icons-device.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    23877 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-device/icons-device.min.css.map
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.314947 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-document/
--rw-r--r--   0 geoffrey   (501) staff       (20)    12044 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-document/icons-document.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    23019 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-document/icons-document.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     5060 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-document/icons-document.legacy.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    10303 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-document/icons-document.legacy.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     4306 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-document/icons-document.legacy.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    10110 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-document/icons-document.legacy.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     7224 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-document/icons-document.main.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    14922 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-document/icons-document.main.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     6434 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-document/icons-document.main.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    14157 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-document/icons-document.main.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)    10512 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-document/icons-document.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    22053 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-document/icons-document.min.css.map
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.317185 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-editor/
--rw-r--r--   0 geoffrey   (501) staff       (20)    10188 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-editor/icons-editor.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    21006 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-editor/icons-editor.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     4282 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-editor/icons-editor.legacy.css
--rw-r--r--   0 geoffrey   (501) staff       (20)     9470 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-editor/icons-editor.legacy.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     3576 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-editor/icons-editor.legacy.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)     9290 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-editor/icons-editor.legacy.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     6146 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-editor/icons-editor.main.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    13740 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-editor/icons-editor.main.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     5396 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-editor/icons-editor.main.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    12995 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-editor/icons-editor.main.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     8744 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-editor/icons-editor.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    20073 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-editor/icons-editor.min.css.map
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.319138 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-finance/
--rw-r--r--   0 geoffrey   (501) staff       (20)     6775 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-finance/icons-finance.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    16388 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-finance/icons-finance.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     2988 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-finance/icons-finance.legacy.css
--rw-r--r--   0 geoffrey   (501) staff       (20)     7688 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-finance/icons-finance.legacy.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     2584 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-finance/icons-finance.legacy.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)     7591 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-finance/icons-finance.legacy.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     4027 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-finance/icons-finance.main.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    10905 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-finance/icons-finance.main.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     3577 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-finance/icons-finance.main.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    10262 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-finance/icons-finance.main.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     5933 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-finance/icons-finance.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    15640 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-finance/icons-finance.min.css.map
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.321708 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-health/
--rw-r--r--   0 geoffrey   (501) staff       (20)    14367 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-health/icons-health.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    25626 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-health/icons-health.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     6168 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-health/icons-health.legacy.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    11461 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-health/icons-health.legacy.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     5280 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-health/icons-health.legacy.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    11232 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-health/icons-health.legacy.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     8439 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-health/icons-health.main.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    16369 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-health/icons-health.main.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     7549 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-health/icons-health.main.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    15575 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-health/icons-health.main.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)    12601 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-health/icons-health.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    24595 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-health/icons-health.min.css.map
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.324351 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-logo/
--rw-r--r--   0 geoffrey   (501) staff       (20)    24122 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-logo/icons-logo.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    38165 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-logo/icons-logo.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     9746 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-logo/icons-logo.legacy.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    16087 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-logo/icons-logo.legacy.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     8200 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-logo/icons-logo.legacy.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    15676 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-logo/icons-logo.legacy.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)    14616 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-logo/icons-logo.main.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    24218 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-logo/icons-logo.main.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)    13026 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-logo/icons-logo.main.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    23185 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-logo/icons-logo.main.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)    20998 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-logo/icons-logo.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    36712 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-logo/icons-logo.min.css.map
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.327487 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-map/
--rw-r--r--   0 geoffrey   (501) staff       (20)    17550 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-map/icons-map.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    29852 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-map/icons-map.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     7456 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-map/icons-map.legacy.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    13177 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-map/icons-map.legacy.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     6298 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-map/icons-map.legacy.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    12874 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-map/icons-map.legacy.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)    10334 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-map/icons-map.main.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    18876 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-map/icons-map.main.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     9184 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-map/icons-map.main.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    18000 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-map/icons-map.main.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)    15254 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-map/icons-map.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    28665 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-map/icons-map.min.css.map
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.330052 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-media/
--rw-r--r--   0 geoffrey   (501) staff       (20)    19301 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-media/icons-media.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    31920 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-media/icons-media.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     7999 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-media/icons-media.legacy.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    13839 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-media/icons-media.legacy.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     6785 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-media/icons-media.legacy.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    13520 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-media/icons-media.legacy.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)    11542 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-media/icons-media.main.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    20284 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-media/icons-media.main.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)    10312 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-media/icons-media.main.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    19374 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-media/icons-media.main.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)    16869 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-media/icons-media.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    30683 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-media/icons-media.min.css.map
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.332007 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-others/
--rw-r--r--   0 geoffrey   (501) staff       (20)     5250 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-others/icons-others.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    14634 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-others/icons-others.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     2350 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-others/icons-others.legacy.css
--rw-r--r--   0 geoffrey   (501) staff       (20)     6968 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-others/icons-others.legacy.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     2012 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-others/icons-others.legacy.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)     6889 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-others/icons-others.legacy.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     3140 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-others/icons-others.main.css
--rw-r--r--   0 geoffrey   (501) staff       (20)     9870 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-others/icons-others.main.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     2750 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-others/icons-others.main.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)     9251 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-others/icons-others.main.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     4534 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-others/icons-others.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    13928 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-others/icons-others.min.css.map
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.334744 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-system/
--rw-r--r--   0 geoffrey   (501) staff       (20)    61210 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-system/icons-system.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    83686 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-system/icons-system.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)    24507 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-system/icons-system.legacy.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    33766 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-system/icons-system.legacy.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)    20773 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-system/icons-system.legacy.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    32754 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-system/icons-system.legacy.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)    36943 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-system/icons-system.main.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    51783 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-system/icons-system.main.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)    33240 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-system/icons-system.main.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    50018 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-system/icons-system.main.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)    53785 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-system/icons-system.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    80902 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-system/icons-system.min.css.map
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.337315 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-user/
--rw-r--r--   0 geoffrey   (501) staff       (20)    10694 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-user/icons-user.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    21349 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-user/icons-user.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     4602 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-user/icons-user.legacy.css
--rw-r--r--   0 geoffrey   (501) staff       (20)     9729 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-user/icons-user.legacy.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     3920 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-user/icons-user.legacy.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)     9556 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-user/icons-user.legacy.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     6332 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-user/icons-user.main.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    13822 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-user/icons-user.main.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     5622 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-user/icons-user.main.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    13097 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-user/icons-user.main.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     9314 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-user/icons-user.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    20443 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-user/icons-user.min.css.map
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.339175 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-weather/
--rw-r--r--   0 geoffrey   (501) staff       (20)     3858 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-weather/icons-weather.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    13024 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-weather/icons-weather.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     1726 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-weather/icons-weather.legacy.css
--rw-r--r--   0 geoffrey   (501) staff       (20)     6315 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-weather/icons-weather.legacy.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     1484 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-weather/icons-weather.legacy.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)     6262 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-weather/icons-weather.legacy.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     2372 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-weather/icons-weather.main.css
--rw-r--r--   0 geoffrey   (501) staff       (20)     8914 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-weather/icons-weather.main.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     2062 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-weather/icons-weather.main.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)     8320 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-weather/icons-weather.main.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)     3318 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-weather/icons-weather.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)    12369 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-weather/icons-weather.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)   252525 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons.css
--rw-r--r--   0 geoffrey   (501) staff       (20)   338301 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)   103243 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons.legacy.css
--rw-r--r--   0 geoffrey   (501) staff       (20)   134266 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons.legacy.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)    87075 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons.legacy.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)   129807 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons.legacy.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)   149522 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons.main.css
--rw-r--r--   0 geoffrey   (501) staff       (20)   204422 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons.main.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)   133091 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons.main.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)   190288 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons.main.min.css.map
--rw-r--r--   0 geoffrey   (501) staff       (20)   219938 2023-06-02 13:12:06.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons.min.css
--rw-r--r--   0 geoffrey   (501) staff       (20)   318184 2023-06-02 13:12:07.000000 mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons.min.css.map
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-02 15:46:04.340506 mkdocs-dsfr-0.0.3/mkdocs_dsfr.egg-info/
--rw-r--r--   0 geoffrey   (501) staff       (20)      305 2023-06-02 15:46:04.000000 mkdocs-dsfr-0.0.3/mkdocs_dsfr.egg-info/PKG-INFO
--rw-r--r--   0 geoffrey   (501) staff       (20)    35907 2023-06-02 15:46:04.000000 mkdocs-dsfr-0.0.3/mkdocs_dsfr.egg-info/SOURCES.txt
--rw-r--r--   0 geoffrey   (501) staff       (20)        1 2023-06-02 15:46:04.000000 mkdocs-dsfr-0.0.3/mkdocs_dsfr.egg-info/dependency_links.txt
--rw-r--r--   0 geoffrey   (501) staff       (20)       28 2023-06-02 15:46:04.000000 mkdocs-dsfr-0.0.3/mkdocs_dsfr.egg-info/entry_points.txt
--rw-r--r--   0 geoffrey   (501) staff       (20)        1 2023-06-02 15:38:26.000000 mkdocs-dsfr-0.0.3/mkdocs_dsfr.egg-info/not-zip-safe
--rw-r--r--   0 geoffrey   (501) staff       (20)       12 2023-06-02 15:46:04.000000 mkdocs-dsfr-0.0.3/mkdocs_dsfr.egg-info/requires.txt
--rw-r--r--   0 geoffrey   (501) staff       (20)        5 2023-06-02 15:46:04.000000 mkdocs-dsfr-0.0.3/mkdocs_dsfr.egg-info/top_level.txt
--rw-r--r--   0 geoffrey   (501) staff       (20)       38 2023-06-02 15:46:04.341026 mkdocs-dsfr-0.0.3/setup.cfg
--rw-r--r--   0 geoffrey   (501) staff       (20)      587 2023-06-02 15:45:41.000000 mkdocs-dsfr-0.0.3/setup.py
+-rw-r--r--   0        0        0     1096 2023-05-31 09:02:27.963069 mkdocs_dsfr-0.0.4/LICENSE
+-rw-r--r--   0        0        0      433 2023-06-02 15:45:48.776491 mkdocs_dsfr-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 09:02:27.964132 mkdocs_dsfr-0.0.4/dsfr/__init__.py
+-rw-r--r--   0        0        0     2851 2023-06-02 13:44:34.400540 mkdocs_dsfr-0.0.4/dsfr/base.html
+-rw-r--r--   0        0        0     5366 2023-05-31 09:02:27.964627 mkdocs_dsfr-0.0.4/dsfr/css/theme.css
+-rw-r--r--   0        0        0   516291 2023-06-02 13:12:06.507999 mkdocs_dsfr-0.0.4/dsfr/dsfr.min.css
+-rw-r--r--   0        0        0    68681 2023-06-02 13:12:06.859999 mkdocs_dsfr-0.0.4/dsfr/dsfr.module.min.js
+-rw-r--r--   0        0        0   218391 2023-06-02 13:12:06.865000 mkdocs_dsfr-0.0.4/dsfr/dsfr.nomodule.min.js
+-rw-r--r--   0        0        0     3631 2023-06-02 13:12:07.177000 mkdocs_dsfr-0.0.4/dsfr/favicon/android-chrome-192x192.png
+-rw-r--r--   0        0        0     9190 2023-06-02 13:12:07.177000 mkdocs_dsfr-0.0.4/dsfr/favicon/android-chrome-512x512.png
+-rw-r--r--   0        0        0     3448 2023-06-02 13:12:07.177999 mkdocs_dsfr-0.0.4/dsfr/favicon/apple-touch-icon.png
+-rw-r--r--   0        0        0     7406 2023-06-02 13:12:06.809999 mkdocs_dsfr-0.0.4/dsfr/favicon/favicon.ico
+-rw-r--r--   0        0        0     6360 2023-06-02 13:12:07.460000 mkdocs_dsfr-0.0.4/dsfr/favicon/favicon.svg
+-rw-r--r--   0        0        0      292 2023-06-02 13:12:07.661999 mkdocs_dsfr-0.0.4/dsfr/favicon/manifest.webmanifest
+-rwxr-xr-x   0        0        0    52216 2023-06-02 13:12:07.664000 mkdocs_dsfr-0.0.4/dsfr/fonts/Marianne-Bold.woff
+-rwxr-xr-x   0        0        0    42092 2023-06-02 13:12:07.674999 mkdocs_dsfr-0.0.4/dsfr/fonts/Marianne-Bold.woff2
+-rwxr-xr-x   0        0        0    56436 2023-06-02 13:12:07.661999 mkdocs_dsfr-0.0.4/dsfr/fonts/Marianne-Bold_Italic.woff
+-rwxr-xr-x   0        0        0    45300 2023-06-02 13:12:07.674000 mkdocs_dsfr-0.0.4/dsfr/fonts/Marianne-Bold_Italic.woff2
+-rwxr-xr-x   0        0        0    50440 2023-06-02 13:12:07.665999 mkdocs_dsfr-0.0.4/dsfr/fonts/Marianne-Light.woff
+-rwxr-xr-x   0        0        0    41368 2023-06-02 13:12:07.677000 mkdocs_dsfr-0.0.4/dsfr/fonts/Marianne-Light.woff2
+-rwxr-xr-x   0        0        0    54492 2023-06-02 13:12:07.664999 mkdocs_dsfr-0.0.4/dsfr/fonts/Marianne-Light_Italic.woff
+-rwxr-xr-x   0        0        0    43916 2023-06-02 13:12:07.676000 mkdocs_dsfr-0.0.4/dsfr/fonts/Marianne-Light_Italic.woff2
+-rwxr-xr-x   0        0        0    51292 2023-06-02 13:12:07.667999 mkdocs_dsfr-0.0.4/dsfr/fonts/Marianne-Medium.woff
+-rwxr-xr-x   0        0        0    41940 2023-06-02 13:12:07.678999 mkdocs_dsfr-0.0.4/dsfr/fonts/Marianne-Medium.woff2
+-rwxr-xr-x   0        0        0    54680 2023-06-02 13:12:07.667000 mkdocs_dsfr-0.0.4/dsfr/fonts/Marianne-Medium_Italic.woff
+-rwxr-xr-x   0        0        0    44572 2023-06-02 13:12:07.677999 mkdocs_dsfr-0.0.4/dsfr/fonts/Marianne-Medium_Italic.woff2
+-rwxr-xr-x   0        0        0    51140 2023-06-02 13:12:07.670000 mkdocs_dsfr-0.0.4/dsfr/fonts/Marianne-Regular.woff
+-rwxr-xr-x   0        0        0    41328 2023-06-02 13:12:07.680999 mkdocs_dsfr-0.0.4/dsfr/fonts/Marianne-Regular.woff2
+-rwxr-xr-x   0        0        0    54328 2023-06-02 13:12:07.668999 mkdocs_dsfr-0.0.4/dsfr/fonts/Marianne-Regular_Italic.woff
+-rwxr-xr-x   0        0        0    44284 2023-06-02 13:12:07.680000 mkdocs_dsfr-0.0.4/dsfr/fonts/Marianne-Regular_Italic.woff2
+-rw-r--r--   0        0        0   114508 2023-06-02 13:12:07.671000 mkdocs_dsfr-0.0.4/dsfr/fonts/Spectral-ExtraBold.woff
+-rw-r--r--   0        0        0    80368 2023-06-02 13:12:07.681999 mkdocs_dsfr-0.0.4/dsfr/fonts/Spectral-ExtraBold.woff2
+-rw-r--r--   0        0        0   114016 2023-06-02 13:12:07.673000 mkdocs_dsfr-0.0.4/dsfr/fonts/Spectral-Regular.woff
+-rw-r--r--   0        0        0    79472 2023-06-02 13:12:07.684000 mkdocs_dsfr-0.0.4/dsfr/fonts/Spectral-Regular.woff2
+-rw-r--r--   0        0        0     2819 2023-05-31 09:02:28.010334 mkdocs_dsfr-0.0.4/dsfr/footer.html
+-rw-r--r--   0        0        0     2213 2023-05-31 09:02:28.010420 mkdocs_dsfr-0.0.4/dsfr/header.html
+-rw-r--r--   0        0        0      397 2023-06-02 13:12:07.378000 mkdocs_dsfr-0.0.4/dsfr/icons/buildings/ancient-gate-fill.svg
+-rw-r--r--   0        0        0      789 2023-06-02 13:12:07.378000 mkdocs_dsfr-0.0.4/dsfr/icons/buildings/ancient-gate-line.svg
+-rw-r--r--   0        0        0      280 2023-06-02 13:12:07.378000 mkdocs_dsfr-0.0.4/dsfr/icons/buildings/ancient-pavilion-fill.svg
+-rw-r--r--   0        0        0      416 2023-06-02 13:12:07.378999 mkdocs_dsfr-0.0.4/dsfr/icons/buildings/ancient-pavilion-line.svg
+-rw-r--r--   0        0        0      232 2023-06-02 13:12:07.392999 mkdocs_dsfr-0.0.4/dsfr/icons/buildings/bank-fill.svg
+-rw-r--r--   0        0        0      262 2023-06-02 13:12:07.392999 mkdocs_dsfr-0.0.4/dsfr/icons/buildings/bank-line.svg
+-rw-r--r--   0        0        0      204 2023-06-02 13:12:07.403000 mkdocs_dsfr-0.0.4/dsfr/icons/buildings/building-fill.svg
+-rw-r--r--   0        0        0      225 2023-06-02 13:12:07.404000 mkdocs_dsfr-0.0.4/dsfr/icons/buildings/building-line.svg
+-rw-r--r--   0        0        0      316 2023-06-02 13:12:07.427000 mkdocs_dsfr-0.0.4/dsfr/icons/buildings/community-fill.svg
+-rw-r--r--   0        0        0      388 2023-06-02 13:12:07.427000 mkdocs_dsfr-0.0.4/dsfr/icons/buildings/community-line.svg
+-rw-r--r--   0        0        0      232 2023-06-02 13:12:07.502000 mkdocs_dsfr-0.0.4/dsfr/icons/buildings/government-fill.svg
+-rw-r--r--   0        0        0      227 2023-06-02 13:12:07.502000 mkdocs_dsfr-0.0.4/dsfr/icons/buildings/government-line.svg
+-rw-r--r--   0        0        0      209 2023-06-02 13:12:07.513999 mkdocs_dsfr-0.0.4/dsfr/icons/buildings/home-4-fill.svg
+-rw-r--r--   0        0        0      239 2023-06-02 13:12:07.513999 mkdocs_dsfr-0.0.4/dsfr/icons/buildings/home-4-line.svg
+-rw-r--r--   0        0        0      212 2023-06-02 13:12:07.515000 mkdocs_dsfr-0.0.4/dsfr/icons/buildings/hospital-fill.svg
+-rw-r--r--   0        0        0      228 2023-06-02 13:12:07.515000 mkdocs_dsfr-0.0.4/dsfr/icons/buildings/hospital-line.svg
+-rw-r--r--   0        0        0      224 2023-06-02 13:12:07.516000 mkdocs_dsfr-0.0.4/dsfr/icons/buildings/hotel-fill.svg
+-rw-r--r--   0        0        0      243 2023-06-02 13:12:07.516000 mkdocs_dsfr-0.0.4/dsfr/icons/buildings/hotel-line.svg
+-rw-r--r--   0        0        0      437 2023-06-02 13:12:07.615000 mkdocs_dsfr-0.0.4/dsfr/icons/buildings/store-fill.svg
+-rw-r--r--   0        0        0      546 2023-06-02 13:12:07.615000 mkdocs_dsfr-0.0.4/dsfr/icons/buildings/store-line.svg
+-rw-r--r--   0        0        0      254 2023-06-02 13:12:07.380000 mkdocs_dsfr-0.0.4/dsfr/icons/business/archive-fill.svg
+-rw-r--r--   0        0        0      288 2023-06-02 13:12:07.380000 mkdocs_dsfr-0.0.4/dsfr/icons/business/archive-line.svg
+-rw-r--r--   0        0        0      330 2023-06-02 13:12:07.390000 mkdocs_dsfr-0.0.4/dsfr/icons/business/attachment-fill.svg
+-rw-r--r--   0        0        0      241 2023-06-02 13:12:07.390000 mkdocs_dsfr-0.0.4/dsfr/icons/business/attachment-line.svg
+-rw-r--r--   0        0        0      289 2023-06-02 13:12:07.391000 mkdocs_dsfr-0.0.4/dsfr/icons/business/award-fill.svg
+-rw-r--r--   0        0        0      338 2023-06-02 13:12:07.391000 mkdocs_dsfr-0.0.4/dsfr/icons/business/award-line.svg
+-rw-r--r--   0        0        0      218 2023-06-02 13:12:07.394000 mkdocs_dsfr-0.0.4/dsfr/icons/business/bar-chart-box-fill.svg
+-rw-r--r--   0        0        0      234 2023-06-02 13:12:07.394000 mkdocs_dsfr-0.0.4/dsfr/icons/business/bar-chart-box-line.svg
+-rw-r--r--   0        0        0      208 2023-06-02 13:12:07.398999 mkdocs_dsfr-0.0.4/dsfr/icons/business/bookmark-fill.svg
+-rw-r--r--   0        0        0      242 2023-06-02 13:12:07.398999 mkdocs_dsfr-0.0.4/dsfr/icons/business/bookmark-line.svg
+-rw-r--r--   0        0        0      253 2023-06-02 13:12:07.400000 mkdocs_dsfr-0.0.4/dsfr/icons/business/briefcase-fill.svg
+-rw-r--r--   0        0        0      267 2023-06-02 13:12:07.400000 mkdocs_dsfr-0.0.4/dsfr/icons/business/briefcase-line.svg
+-rw-r--r--   0        0        0      248 2023-06-02 13:12:07.404999 mkdocs_dsfr-0.0.4/dsfr/icons/business/calendar-2-fill.svg
+-rw-r--r--   0        0        0      281 2023-06-02 13:12:07.405999 mkdocs_dsfr-0.0.4/dsfr/icons/business/calendar-2-line.svg
+-rw-r--r--   0        0        0      218 2023-06-02 13:12:07.405999 mkdocs_dsfr-0.0.4/dsfr/icons/business/calendar-event-fill.svg
+-rw-r--r--   0        0        0      251 2023-06-02 13:12:07.405999 mkdocs_dsfr-0.0.4/dsfr/icons/business/calendar-event-line.svg
+-rw-r--r--   0        0        0      203 2023-06-02 13:12:07.407000 mkdocs_dsfr-0.0.4/dsfr/icons/business/calendar-fill.svg
+-rw-r--r--   0        0        0      244 2023-06-02 13:12:07.407999 mkdocs_dsfr-0.0.4/dsfr/icons/business/calendar-line.svg
+-rw-r--r--   0        0        0      254 2023-06-02 13:12:07.423000 mkdocs_dsfr-0.0.4/dsfr/icons/business/cloud-fill.svg
+-rw-r--r--   0        0        0      356 2023-06-02 13:12:07.423000 mkdocs_dsfr-0.0.4/dsfr/icons/business/cloud-line.svg
+-rw-r--r--   0        0        0      290 2023-06-02 13:12:07.431999 mkdocs_dsfr-0.0.4/dsfr/icons/business/copyright-fill.svg
+-rw-r--r--   0        0        0      346 2023-06-02 13:12:07.431999 mkdocs_dsfr-0.0.4/dsfr/icons/business/copyright-line.svg
+-rw-r--r--   0        0        0      341 2023-06-02 13:12:07.436000 mkdocs_dsfr-0.0.4/dsfr/icons/business/customer-service-fill.svg
+-rw-r--r--   0        0        0      375 2023-06-02 13:12:07.436000 mkdocs_dsfr-0.0.4/dsfr/icons/business/customer-service-line.svg
+-rw-r--r--   0        0        0      210 2023-06-02 13:12:07.469000 mkdocs_dsfr-0.0.4/dsfr/icons/business/flag-fill.svg
+-rw-r--r--   0        0        0      255 2023-06-02 13:12:07.469000 mkdocs_dsfr-0.0.4/dsfr/icons/business/flag-line.svg
+-rw-r--r--   0        0        0      540 2023-06-02 13:12:07.499000 mkdocs_dsfr-0.0.4/dsfr/icons/business/global-fill.svg
+-rw-r--r--   0        0        0      607 2023-06-02 13:12:07.500000 mkdocs_dsfr-0.0.4/dsfr/icons/business/global-line.svg
+-rw-r--r--   0        0        0      200 2023-06-02 13:12:07.529000 mkdocs_dsfr-0.0.4/dsfr/icons/business/line-chart-fill.svg
+-rw-r--r--   0        0        0      218 2023-06-02 13:12:07.529000 mkdocs_dsfr-0.0.4/dsfr/icons/business/line-chart-line.svg
+-rw-r--r--   0        0        0      409 2023-06-02 13:12:07.530999 mkdocs_dsfr-0.0.4/dsfr/icons/business/links-fill.svg
+-rw-r--r--   0        0        0      418 2023-06-02 13:12:07.532000 mkdocs_dsfr-0.0.4/dsfr/icons/business/links-line.svg
+-rw-r--r--   0        0        0      260 2023-06-02 13:12:07.539999 mkdocs_dsfr-0.0.4/dsfr/icons/business/mail-fill.svg
+-rw-r--r--   0        0        0      247 2023-06-02 13:12:07.540999 mkdocs_dsfr-0.0.4/dsfr/icons/business/mail-line.svg
+-rw-r--r--   0        0        0      318 2023-06-02 13:12:07.540999 mkdocs_dsfr-0.0.4/dsfr/icons/business/mail-open-fill.svg
+-rw-r--r--   0        0        0      359 2023-06-02 13:12:07.540999 mkdocs_dsfr-0.0.4/dsfr/icons/business/mail-open-line.svg
+-rw-r--r--   0        0        0      355 2023-06-02 13:12:07.546999 mkdocs_dsfr-0.0.4/dsfr/icons/business/medal-fill.svg
+-rw-r--r--   0        0        0      389 2023-06-02 13:12:07.546999 mkdocs_dsfr-0.0.4/dsfr/icons/business/medal-line.svg
+-rw-r--r--   0        0        0      248 2023-06-02 13:12:07.573999 mkdocs_dsfr-0.0.4/dsfr/icons/business/pie-chart-2-fill.svg
+-rw-r--r--   0        0        0      378 2023-06-02 13:12:07.575000 mkdocs_dsfr-0.0.4/dsfr/icons/business/pie-chart-2-line.svg
+-rw-r--r--   0        0        0      273 2023-06-02 13:12:07.575000 mkdocs_dsfr-0.0.4/dsfr/icons/business/pie-chart-box-fill.svg
+-rw-r--r--   0        0        0      289 2023-06-02 13:12:07.575000 mkdocs_dsfr-0.0.4/dsfr/icons/business/pie-chart-box-line.svg
+-rw-r--r--   0        0        0      256 2023-06-02 13:12:07.579999 mkdocs_dsfr-0.0.4/dsfr/icons/business/printer-fill.svg
+-rw-r--r--   0        0        0      341 2023-06-02 13:12:07.579999 mkdocs_dsfr-0.0.4/dsfr/icons/business/printer-line.svg
+-rw-r--r--   0        0        0      296 2023-06-02 13:12:07.581000 mkdocs_dsfr-0.0.4/dsfr/icons/business/profil-fill.svg
+-rw-r--r--   0        0        0      312 2023-06-02 13:12:07.581000 mkdocs_dsfr-0.0.4/dsfr/icons/business/profil-line.svg
+-rw-r--r--   0        0        0      356 2023-06-02 13:12:07.581000 mkdocs_dsfr-0.0.4/dsfr/icons/business/projector-2-fill.svg
+-rw-r--r--   0        0        0      350 2023-06-02 13:12:07.582000 mkdocs_dsfr-0.0.4/dsfr/icons/business/projector-2-line.svg
+-rw-r--r--   0        0        0      248 2023-06-02 13:12:07.598999 mkdocs_dsfr-0.0.4/dsfr/icons/business/send-plane-fill.svg
+-rw-r--r--   0        0        0      301 2023-06-02 13:12:07.599999 mkdocs_dsfr-0.0.4/dsfr/icons/business/send-plane-line.svg
+-rw-r--r--   0        0        0      226 2023-06-02 13:12:07.608000 mkdocs_dsfr-0.0.4/dsfr/icons/business/slideshow-fill.svg
+-rw-r--r--   0        0        0      241 2023-06-02 13:12:07.608000 mkdocs_dsfr-0.0.4/dsfr/icons/business/slideshow-line.svg
+-rw-r--r--   0        0        0      215 2023-06-02 13:12:07.657999 mkdocs_dsfr-0.0.4/dsfr/icons/business/window-fill.svg
+-rw-r--r--   0        0        0      230 2023-06-02 13:12:07.658999 mkdocs_dsfr-0.0.4/dsfr/icons/business/window-line.svg
+-rw-r--r--   0        0        0      199 2023-06-02 13:12:07.413000 mkdocs_dsfr-0.0.4/dsfr/icons/communication/chat-2-fill.svg
+-rw-r--r--   0        0        0      237 2023-06-02 13:12:07.414000 mkdocs_dsfr-0.0.4/dsfr/icons/communication/chat-2-line.svg
+-rw-r--r--   0        0        0      236 2023-06-02 13:12:07.414000 mkdocs_dsfr-0.0.4/dsfr/icons/communication/chat-3-fill.svg
+-rw-r--r--   0        0        0      360 2023-06-02 13:12:07.414000 mkdocs_dsfr-0.0.4/dsfr/icons/communication/chat-3-line.svg
+-rw-r--r--   0        0        0      256 2023-06-02 13:12:07.414999 mkdocs_dsfr-0.0.4/dsfr/icons/communication/chat-check-fill.svg
+-rw-r--r--   0        0        0      283 2023-06-02 13:12:07.414999 mkdocs_dsfr-0.0.4/dsfr/icons/communication/chat-check-line.svg
+-rw-r--r--   0        0        0      321 2023-06-02 13:12:07.414999 mkdocs_dsfr-0.0.4/dsfr/icons/communication/chat-delete-fill.svg
+-rw-r--r--   0        0        0      348 2023-06-02 13:12:07.415999 mkdocs_dsfr-0.0.4/dsfr/icons/communication/chat-delete-line.svg
+-rw-r--r--   0        0        0      243 2023-06-02 13:12:07.415999 mkdocs_dsfr-0.0.4/dsfr/icons/communication/chat-poll-fill.svg
+-rw-r--r--   0        0        0      214 2023-06-02 13:12:07.415999 mkdocs_dsfr-0.0.4/dsfr/icons/communication/chat-poll-line.svg
+-rw-r--r--   0        0        0      236 2023-06-02 13:12:07.441999 mkdocs_dsfr-0.0.4/dsfr/icons/communication/discuss-fill.svg
+-rw-r--r--   0        0        0      282 2023-06-02 13:12:07.441999 mkdocs_dsfr-0.0.4/dsfr/icons/communication/discuss-line.svg
+-rw-r--r--   0        0        0      201 2023-06-02 13:12:07.460000 mkdocs_dsfr-0.0.4/dsfr/icons/communication/feedback-fill.svg
+-rw-r--r--   0        0        0      229 2023-06-02 13:12:07.460000 mkdocs_dsfr-0.0.4/dsfr/icons/communication/feedback-line.svg
+-rw-r--r--   0        0        0      215 2023-06-02 13:12:07.549999 mkdocs_dsfr-0.0.4/dsfr/icons/communication/message-2-fill.svg
+-rw-r--r--   0        0        0      245 2023-06-02 13:12:07.551000 mkdocs_dsfr-0.0.4/dsfr/icons/communication/message-2-line.svg
+-rw-r--r--   0        0        0      231 2023-06-02 13:12:07.584000 mkdocs_dsfr-0.0.4/dsfr/icons/communication/question-answer-fill.svg
+-rw-r--r--   0        0        0      260 2023-06-02 13:12:07.585000 mkdocs_dsfr-0.0.4/dsfr/icons/communication/question-answer-line.svg
+-rw-r--r--   0        0        0      263 2023-06-02 13:12:07.585999 mkdocs_dsfr-0.0.4/dsfr/icons/communication/questionnaire-fill.svg
+-rw-r--r--   0        0        0      327 2023-06-02 13:12:07.585999 mkdocs_dsfr-0.0.4/dsfr/icons/communication/questionnaire-line.svg
+-rw-r--r--   0        0        0      206 2023-06-02 13:12:07.651000 mkdocs_dsfr-0.0.4/dsfr/icons/communication/video-chat-fill.svg
+-rw-r--r--   0        0        0      234 2023-06-02 13:12:07.651000 mkdocs_dsfr-0.0.4/dsfr/icons/communication/video-chat-line.svg
+-rw-r--r--   0        0        0      318 2023-06-02 13:12:07.391000 mkdocs_dsfr-0.0.4/dsfr/icons/design/ball-pen-fill.svg
+-rw-r--r--   0        0        0      372 2023-06-02 13:12:07.391999 mkdocs_dsfr-0.0.4/dsfr/icons/design/ball-pen-line.svg
+-rw-r--r--   0        0        0      252 2023-06-02 13:12:07.401000 mkdocs_dsfr-0.0.4/dsfr/icons/design/brush-3-fill.svg
+-rw-r--r--   0        0        0      266 2023-06-02 13:12:07.401000 mkdocs_dsfr-0.0.4/dsfr/icons/design/brush-3-line.svg
+-rw-r--r--   0        0        0      449 2023-06-02 13:12:07.401999 mkdocs_dsfr-0.0.4/dsfr/icons/design/brush-fill.svg
+-rw-r--r--   0        0        0      689 2023-06-02 13:12:07.401999 mkdocs_dsfr-0.0.4/dsfr/icons/design/brush-line.svg
+-rw-r--r--   0        0        0      195 2023-06-02 13:12:07.430999 mkdocs_dsfr-0.0.4/dsfr/icons/design/contrast-fill.svg
+-rw-r--r--   0        0        0      230 2023-06-02 13:12:07.430999 mkdocs_dsfr-0.0.4/dsfr/icons/design/contrast-line.svg
+-rw-r--r--   0        0        0      173 2023-06-02 13:12:07.431999 mkdocs_dsfr-0.0.4/dsfr/icons/design/crop-fill.svg
+-rw-r--r--   0        0        0      184 2023-06-02 13:12:07.433000 mkdocs_dsfr-0.0.4/dsfr/icons/design/crop-line.svg
+-rw-r--r--   0        0        0      399 2023-06-02 13:12:07.447000 mkdocs_dsfr-0.0.4/dsfr/icons/design/drag-move-2-fill.svg
+-rw-r--r--   0        0        0      178 2023-06-02 13:12:07.447000 mkdocs_dsfr-0.0.4/dsfr/icons/design/drag-move-2-line.svg
+-rw-r--r--   0        0        0      153 2023-06-02 13:12:07.448999 mkdocs_dsfr-0.0.4/dsfr/icons/design/drop-fill.svg
+-rw-r--r--   0        0        0      190 2023-06-02 13:12:07.448999 mkdocs_dsfr-0.0.4/dsfr/icons/design/drop-line.svg
+-rw-r--r--   0        0        0      275 2023-06-02 13:12:07.451999 mkdocs_dsfr-0.0.4/dsfr/icons/design/edit-box-fill.svg
+-rw-r--r--   0        0        0      255 2023-06-02 13:12:07.451999 mkdocs_dsfr-0.0.4/dsfr/icons/design/edit-box-line.svg
+-rw-r--r--   0        0        0      206 2023-06-02 13:12:07.453000 mkdocs_dsfr-0.0.4/dsfr/icons/design/edit-fill.svg
+-rw-r--r--   0        0        0      258 2023-06-02 13:12:07.453000 mkdocs_dsfr-0.0.4/dsfr/icons/design/edit-line.svg
+-rw-r--r--   0        0        0      266 2023-06-02 13:12:07.522000 mkdocs_dsfr-0.0.4/dsfr/icons/design/ink-bottle-fill.svg
+-rw-r--r--   0        0        0      323 2023-06-02 13:12:07.522000 mkdocs_dsfr-0.0.4/dsfr/icons/design/ink-bottle-line.svg
+-rw-r--r--   0        0        0      241 2023-06-02 13:12:07.525000 mkdocs_dsfr-0.0.4/dsfr/icons/design/layout-grid-fill.svg
+-rw-r--r--   0        0        0      232 2023-06-02 13:12:07.526000 mkdocs_dsfr-0.0.4/dsfr/icons/design/layout-grid-line.svg
+-rw-r--r--   0        0        0      401 2023-06-02 13:12:07.545000 mkdocs_dsfr-0.0.4/dsfr/icons/design/mark-pen-fill.svg
+-rw-r--r--   0        0        0      503 2023-06-02 13:12:07.546000 mkdocs_dsfr-0.0.4/dsfr/icons/design/mark-pen-line.svg
+-rw-r--r--   0        0        0      292 2023-06-02 13:12:07.565000 mkdocs_dsfr-0.0.4/dsfr/icons/design/paint-brush-fill.svg
+-rw-r--r--   0        0        0      305 2023-06-02 13:12:07.565000 mkdocs_dsfr-0.0.4/dsfr/icons/design/paint-brush-line.svg
+-rw-r--r--   0        0        0      339 2023-06-02 13:12:07.565999 mkdocs_dsfr-0.0.4/dsfr/icons/design/paint-fill.svg
+-rw-r--r--   0        0        0      362 2023-06-02 13:12:07.565999 mkdocs_dsfr-0.0.4/dsfr/icons/design/paint-line.svg
+-rw-r--r--   0        0        0      437 2023-06-02 13:12:07.566999 mkdocs_dsfr-0.0.4/dsfr/icons/design/palette-fill.svg
+-rw-r--r--   0        0        0      584 2023-06-02 13:12:07.566999 mkdocs_dsfr-0.0.4/dsfr/icons/design/palette-line.svg
+-rw-r--r--   0        0        0      386 2023-06-02 13:12:07.568000 mkdocs_dsfr-0.0.4/dsfr/icons/design/pantone-fill.svg
+-rw-r--r--   0        0        0      505 2023-06-02 13:12:07.568000 mkdocs_dsfr-0.0.4/dsfr/icons/design/pantone-line.svg
+-rw-r--r--   0        0        0      389 2023-06-02 13:12:07.571000 mkdocs_dsfr-0.0.4/dsfr/icons/design/pen-nib-fill.svg
+-rw-r--r--   0        0        0      510 2023-06-02 13:12:07.572000 mkdocs_dsfr-0.0.4/dsfr/icons/design/pen-nib-line.svg
+-rw-r--r--   0        0        0      254 2023-06-02 13:12:07.572000 mkdocs_dsfr-0.0.4/dsfr/icons/design/pencil-fill.svg
+-rw-r--r--   0        0        0      310 2023-06-02 13:12:07.572999 mkdocs_dsfr-0.0.4/dsfr/icons/design/pencil-line.svg
+-rw-r--r--   0        0        0      234 2023-06-02 13:12:07.572999 mkdocs_dsfr-0.0.4/dsfr/icons/design/pencil-ruler-fill.svg
+-rw-r--r--   0        0        0      255 2023-06-02 13:12:07.572999 mkdocs_dsfr-0.0.4/dsfr/icons/design/pencil-ruler-line.svg
+-rw-r--r--   0        0        0      302 2023-06-02 13:12:07.605999 mkdocs_dsfr-0.0.4/dsfr/icons/design/sip-fill.svg
+-rw-r--r--   0        0        0      352 2023-06-02 13:12:07.607000 mkdocs_dsfr-0.0.4/dsfr/icons/design/sip-line.svg
+-rw-r--r--   0        0        0      221 2023-06-02 13:12:07.622999 mkdocs_dsfr-0.0.4/dsfr/icons/design/table-fill.svg
+-rw-r--r--   0        0        0      234 2023-06-02 13:12:07.624000 mkdocs_dsfr-0.0.4/dsfr/icons/design/table-line.svg
+-rw-r--r--   0        0        0      500 2023-06-02 13:12:07.401999 mkdocs_dsfr-0.0.4/dsfr/icons/development/bug-fill.svg
+-rw-r--r--   0        0        0      632 2023-06-02 13:12:07.403000 mkdocs_dsfr-0.0.4/dsfr/icons/development/bug-line.svg
+-rw-r--r--   0        0        0      360 2023-06-02 13:12:07.424000 mkdocs_dsfr-0.0.4/dsfr/icons/development/code-box-fill.svg
+-rw-r--r--   0        0        0      374 2023-06-02 13:12:07.424999 mkdocs_dsfr-0.0.4/dsfr/icons/development/code-box-line.svg
+-rw-r--r--   0        0        0      281 2023-06-02 13:12:07.424999 mkdocs_dsfr-0.0.4/dsfr/icons/development/code-s-slash-line.svg
+-rw-r--r--   0        0        0      197 2023-06-02 13:12:07.434999 mkdocs_dsfr-0.0.4/dsfr/icons/development/cursor-fill.svg
+-rw-r--r--   0        0        0      283 2023-06-02 13:12:07.436000 mkdocs_dsfr-0.0.4/dsfr/icons/development/cursor-line.svg
+-rw-r--r--   0        0        0      307 2023-06-02 13:12:07.490000 mkdocs_dsfr-0.0.4/dsfr/icons/development/git-branch-fill.svg
+-rw-r--r--   0        0        0      425 2023-06-02 13:12:07.490999 mkdocs_dsfr-0.0.4/dsfr/icons/development/git-branch-line.svg
+-rw-r--r--   0        0        0      187 2023-06-02 13:12:07.490999 mkdocs_dsfr-0.0.4/dsfr/icons/development/git-commit-fill.svg
+-rw-r--r--   0        0        0      250 2023-06-02 13:12:07.494999 mkdocs_dsfr-0.0.4/dsfr/icons/development/git-commit-line.svg
+-rw-r--r--   0        0        0      330 2023-06-02 13:12:07.494999 mkdocs_dsfr-0.0.4/dsfr/icons/development/git-merge-fill.svg
+-rw-r--r--   0        0        0      455 2023-06-02 13:12:07.494999 mkdocs_dsfr-0.0.4/dsfr/icons/development/git-merge-line.svg
+-rw-r--r--   0        0        0      233 2023-06-02 13:12:07.496000 mkdocs_dsfr-0.0.4/dsfr/icons/development/git-pull-request-fill.svg
+-rw-r--r--   0        0        0      356 2023-06-02 13:12:07.496000 mkdocs_dsfr-0.0.4/dsfr/icons/development/git-pull-request-line.svg
+-rw-r--r--   0        0        0      294 2023-06-02 13:12:07.496000 mkdocs_dsfr-0.0.4/dsfr/icons/development/git-repository-commits-fill.svg
+-rw-r--r--   0        0        0      320 2023-06-02 13:12:07.496999 mkdocs_dsfr-0.0.4/dsfr/icons/development/git-repository-commits-line.svg
+-rw-r--r--   0        0        0      285 2023-06-02 13:12:07.496999 mkdocs_dsfr-0.0.4/dsfr/icons/development/git-repository-fill.svg
+-rw-r--r--   0        0        0      328 2023-06-02 13:12:07.496999 mkdocs_dsfr-0.0.4/dsfr/icons/development/git-repository-line.svg
+-rw-r--r--   0        0        0      288 2023-06-02 13:12:07.497999 mkdocs_dsfr-0.0.4/dsfr/icons/development/git-repository-private-fill.svg
+-rw-r--r--   0        0        0      304 2023-06-02 13:12:07.497999 mkdocs_dsfr-0.0.4/dsfr/icons/development/git-repository-private-line.svg
+-rw-r--r--   0        0        0      260 2023-06-02 13:12:07.628999 mkdocs_dsfr-0.0.4/dsfr/icons/development/terminal-box-fill.svg
+-rw-r--r--   0        0        0      287 2023-06-02 13:12:07.628999 mkdocs_dsfr-0.0.4/dsfr/icons/development/terminal-box-line.svg
+-rw-r--r--   0        0        0      186 2023-06-02 13:12:07.630000 mkdocs_dsfr-0.0.4/dsfr/icons/development/terminal-line.svg
+-rw-r--r--   0        0        0      230 2023-06-02 13:12:07.630000 mkdocs_dsfr-0.0.4/dsfr/icons/development/terminal-window-fill.svg
+-rw-r--r--   0        0        0      245 2023-06-02 13:12:07.631000 mkdocs_dsfr-0.0.4/dsfr/icons/development/terminal-window-line.svg
+-rw-r--r--   0        0        0      343 2023-06-02 13:12:07.395999 mkdocs_dsfr-0.0.4/dsfr/icons/device/bluetooth-fill.svg
+-rw-r--r--   0        0        0      343 2023-06-02 13:12:07.395999 mkdocs_dsfr-0.0.4/dsfr/icons/device/bluetooth-line.svg
+-rw-r--r--   0        0        0      256 2023-06-02 13:12:07.428999 mkdocs_dsfr-0.0.4/dsfr/icons/device/computer-fill.svg
+-rw-r--r--   0        0        0      275 2023-06-02 13:12:07.428999 mkdocs_dsfr-0.0.4/dsfr/icons/device/computer-line.svg
+-rw-r--r--   0        0        0      514 2023-06-02 13:12:07.437000 mkdocs_dsfr-0.0.4/dsfr/icons/device/dashboard-3-fill.svg
+-rw-r--r--   0        0        0      552 2023-06-02 13:12:07.437999 mkdocs_dsfr-0.0.4/dsfr/icons/device/dashboard-3-line.svg
+-rw-r--r--   0        0        0      266 2023-06-02 13:12:07.438999 mkdocs_dsfr-0.0.4/dsfr/icons/device/database-fill.svg
+-rw-r--r--   0        0        0      296 2023-06-02 13:12:07.438999 mkdocs_dsfr-0.0.4/dsfr/icons/device/database-line.svg
+-rw-r--r--   0        0        0      250 2023-06-02 13:12:07.440000 mkdocs_dsfr-0.0.4/dsfr/icons/device/device-fill.svg
+-rw-r--r--   0        0        0      260 2023-06-02 13:12:07.440000 mkdocs_dsfr-0.0.4/dsfr/icons/device/device-line.svg
+-rw-r--r--   0        0        0      206 2023-06-02 13:12:07.509000 mkdocs_dsfr-0.0.4/dsfr/icons/device/hard-drive-2-fill.svg
+-rw-r--r--   0        0        0      222 2023-06-02 13:12:07.509000 mkdocs_dsfr-0.0.4/dsfr/icons/device/hard-drive-2-line.svg
+-rw-r--r--   0        0        0      290 2023-06-02 13:12:07.539999 mkdocs_dsfr-0.0.4/dsfr/icons/device/mac-fill.svg
+-rw-r--r--   0        0        0      288 2023-06-02 13:12:07.539999 mkdocs_dsfr-0.0.4/dsfr/icons/device/mac-line.svg
+-rw-r--r--   0        0        0      485 2023-06-02 13:12:07.573999 mkdocs_dsfr-0.0.4/dsfr/icons/device/phone-fill.svg
+-rw-r--r--   0        0        0      719 2023-06-02 13:12:07.573999 mkdocs_dsfr-0.0.4/dsfr/icons/device/phone-line.svg
+-rw-r--r--   0        0        0      272 2023-06-02 13:12:07.582999 mkdocs_dsfr-0.0.4/dsfr/icons/device/qr-code-fill.svg
+-rw-r--r--   0        0        0      315 2023-06-02 13:12:07.584000 mkdocs_dsfr-0.0.4/dsfr/icons/device/qr-code-line.svg
+-rw-r--r--   0        0        0      229 2023-06-02 13:12:07.591000 mkdocs_dsfr-0.0.4/dsfr/icons/device/rss-fill.svg
+-rw-r--r--   0        0        0      230 2023-06-02 13:12:07.592000 mkdocs_dsfr-0.0.4/dsfr/icons/device/rss-line.svg
+-rw-r--r--   0        0        0      234 2023-06-02 13:12:07.592999 mkdocs_dsfr-0.0.4/dsfr/icons/device/save-3-fill.svg
+-rw-r--r--   0        0        0      250 2023-06-02 13:12:07.594000 mkdocs_dsfr-0.0.4/dsfr/icons/device/save-3-line.svg
+-rw-r--r--   0        0        0      195 2023-06-02 13:12:07.594000 mkdocs_dsfr-0.0.4/dsfr/icons/device/save-fill.svg
+-rw-r--r--   0        0        0      219 2023-06-02 13:12:07.595000 mkdocs_dsfr-0.0.4/dsfr/icons/device/save-line.svg
+-rw-r--r--   0        0        0      219 2023-06-02 13:12:07.599999 mkdocs_dsfr-0.0.4/dsfr/icons/device/server-fill.svg
+-rw-r--r--   0        0        0      234 2023-06-02 13:12:07.601000 mkdocs_dsfr-0.0.4/dsfr/icons/device/server-line.svg
+-rw-r--r--   0        0        0      208 2023-06-02 13:12:07.608999 mkdocs_dsfr-0.0.4/dsfr/icons/device/smartphone-fill.svg
+-rw-r--r--   0        0        0      224 2023-06-02 13:12:07.608999 mkdocs_dsfr-0.0.4/dsfr/icons/device/smartphone-line.svg
+-rw-r--r--   0        0        0      208 2023-06-02 13:12:07.624000 mkdocs_dsfr-0.0.4/dsfr/icons/device/tablet-fill.svg
+-rw-r--r--   0        0        0      224 2023-06-02 13:12:07.625000 mkdocs_dsfr-0.0.4/dsfr/icons/device/tablet-line.svg
+-rw-r--r--   0        0        0      285 2023-06-02 13:12:07.638999 mkdocs_dsfr-0.0.4/dsfr/icons/device/tv-fill.svg
+-rw-r--r--   0        0        0      304 2023-06-02 13:12:07.640000 mkdocs_dsfr-0.0.4/dsfr/icons/device/tv-line.svg
+-rw-r--r--   0        0        0      618 2023-06-02 13:12:07.657000 mkdocs_dsfr-0.0.4/dsfr/icons/device/wifi-fill.svg
+-rw-r--r--   0        0        0      630 2023-06-02 13:12:07.657999 mkdocs_dsfr-0.0.4/dsfr/icons/device/wifi-line.svg
+-rw-r--r--   0        0        0      233 2023-06-02 13:12:07.388000 mkdocs_dsfr-0.0.4/dsfr/icons/document/article-fill.svg
+-rw-r--r--   0        0        0      249 2023-06-02 13:12:07.388999 mkdocs_dsfr-0.0.4/dsfr/icons/document/article-line.svg
+-rw-r--r--   0        0        0      181 2023-06-02 13:12:07.397000 mkdocs_dsfr-0.0.4/dsfr/icons/document/book-2-fill.svg
+-rw-r--r--   0        0        0      227 2023-06-02 13:12:07.397000 mkdocs_dsfr-0.0.4/dsfr/icons/document/book-2-line.svg
+-rw-r--r--   0        0        0      226 2023-06-02 13:12:07.398000 mkdocs_dsfr-0.0.4/dsfr/icons/document/booklet-fill.svg
+-rw-r--r--   0        0        0      242 2023-06-02 13:12:07.398999 mkdocs_dsfr-0.0.4/dsfr/icons/document/booklet-line.svg
+-rw-r--r--   0        0        0      250 2023-06-02 13:12:07.421000 mkdocs_dsfr-0.0.4/dsfr/icons/document/clipboard-fill.svg
+-rw-r--r--   0        0        0      274 2023-06-02 13:12:07.421000 mkdocs_dsfr-0.0.4/dsfr/icons/document/clipboard-line.svg
+-rw-r--r--   0        0        0      317 2023-06-02 13:12:07.446000 mkdocs_dsfr-0.0.4/dsfr/icons/document/draft-fill.svg
+-rw-r--r--   0        0        0      303 2023-06-02 13:12:07.447000 mkdocs_dsfr-0.0.4/dsfr/icons/document/draft-line.svg
+-rw-r--r--   0        0        0      234 2023-06-02 13:12:07.460999 mkdocs_dsfr-0.0.4/dsfr/icons/document/file-add-fill.svg
+-rw-r--r--   0        0        0      251 2023-06-02 13:12:07.460999 mkdocs_dsfr-0.0.4/dsfr/icons/document/file-add-line.svg
+-rw-r--r--   0        0        0      227 2023-06-02 13:12:07.460999 mkdocs_dsfr-0.0.4/dsfr/icons/document/file-download-fill.svg
+-rw-r--r--   0        0        0      245 2023-06-02 13:12:07.461999 mkdocs_dsfr-0.0.4/dsfr/icons/document/file-download-line.svg
+-rw-r--r--   0        0        0      230 2023-06-02 13:12:07.461999 mkdocs_dsfr-0.0.4/dsfr/icons/document/file-fill.svg
+-rw-r--r--   0        0        0      225 2023-06-02 13:12:07.463000 mkdocs_dsfr-0.0.4/dsfr/icons/document/file-line.svg
+-rw-r--r--   0        0        0      255 2023-06-02 13:12:07.463000 mkdocs_dsfr-0.0.4/dsfr/icons/document/file-pdf-fill.svg
+-rw-r--r--   0        0        0      273 2023-06-02 13:12:07.463000 mkdocs_dsfr-0.0.4/dsfr/icons/document/file-pdf-line.svg
+-rw-r--r--   0        0        0      281 2023-06-02 13:12:07.463999 mkdocs_dsfr-0.0.4/dsfr/icons/document/file-text-fill.svg
+-rw-r--r--   0        0        0      272 2023-06-02 13:12:07.463999 mkdocs_dsfr-0.0.4/dsfr/icons/document/file-text-line.svg
+-rw-r--r--   0        0        0      198 2023-06-02 13:12:07.470000 mkdocs_dsfr-0.0.4/dsfr/icons/document/folder-2-fill.svg
+-rw-r--r--   0        0        0      234 2023-06-02 13:12:07.470999 mkdocs_dsfr-0.0.4/dsfr/icons/document/folder-2-line.svg
+-rw-r--r--   0        0        0      262 2023-06-02 13:12:07.559999 mkdocs_dsfr-0.0.4/dsfr/icons/document/newspaper-fill.svg
+-rw-r--r--   0        0        0      290 2023-06-02 13:12:07.559999 mkdocs_dsfr-0.0.4/dsfr/icons/document/newspaper-line.svg
+-rw-r--r--   0        0        0      292 2023-06-02 13:12:07.619999 mkdocs_dsfr-0.0.4/dsfr/icons/document/survey-fill.svg
+-rw-r--r--   0        0        0      317 2023-06-02 13:12:07.619999 mkdocs_dsfr-0.0.4/dsfr/icons/document/survey-line.svg
+-rw-r--r--   0        0        0      217 2023-06-02 13:12:07.635999 mkdocs_dsfr-0.0.4/dsfr/icons/document/todo-fill.svg
+-rw-r--r--   0        0        0      250 2023-06-02 13:12:07.635999 mkdocs_dsfr-0.0.4/dsfr/icons/document/todo-line.svg
+-rw-r--r--   0        0        0      250 2023-06-02 13:12:07.426000 mkdocs_dsfr-0.0.4/dsfr/icons/editor/code-view.svg
+-rw-r--r--   0        0        0      250 2023-06-02 13:12:07.470999 mkdocs_dsfr-0.0.4/dsfr/icons/editor/font-size.svg
+-rw-r--r--   0        0        0      314 2023-06-02 13:12:07.473999 mkdocs_dsfr-0.0.4/dsfr/icons/editor/fr--bold.svg
+-rw-r--r--   0        0        0      160 2023-06-02 13:12:07.476000 mkdocs_dsfr-0.0.4/dsfr/icons/editor/fr--highlight.svg
+-rw-r--r--   0        0        0      278 2023-06-02 13:12:07.477999 mkdocs_dsfr-0.0.4/dsfr/icons/editor/fr--quote-fill.svg
+-rw-r--r--   0        0        0      344 2023-06-02 13:12:07.477999 mkdocs_dsfr-0.0.4/dsfr/icons/editor/fr--quote-line.svg
+-rw-r--r--   0        0        0      223 2023-06-02 13:12:07.505000 mkdocs_dsfr-0.0.4/dsfr/icons/editor/h-1.svg
+-rw-r--r--   0        0        0      387 2023-06-02 13:12:07.505000 mkdocs_dsfr-0.0.4/dsfr/icons/editor/h-2.svg
+-rw-r--r--   0        0        0      542 2023-06-02 13:12:07.505000 mkdocs_dsfr-0.0.4/dsfr/icons/editor/h-3.svg
+-rw-r--r--   0        0        0      268 2023-06-02 13:12:07.506000 mkdocs_dsfr-0.0.4/dsfr/icons/editor/h-4.svg
+-rw-r--r--   0        0        0      393 2023-06-02 13:12:07.506999 mkdocs_dsfr-0.0.4/dsfr/icons/editor/h-5.svg
+-rw-r--r--   0        0        0      538 2023-06-02 13:12:07.506999 mkdocs_dsfr-0.0.4/dsfr/icons/editor/h-6.svg
+-rw-r--r--   0        0        0      298 2023-06-02 13:12:07.509000 mkdocs_dsfr-0.0.4/dsfr/icons/editor/hashtag.svg
+-rw-r--r--   0        0        0      158 2023-06-02 13:12:07.525000 mkdocs_dsfr-0.0.4/dsfr/icons/editor/italic.svg
+-rw-r--r--   0        0        0      468 2023-06-02 13:12:07.529999 mkdocs_dsfr-0.0.4/dsfr/icons/editor/link-unlink.svg
+-rw-r--r--   0        0        0      408 2023-06-02 13:12:07.529999 mkdocs_dsfr-0.0.4/dsfr/icons/editor/link.svg
+-rw-r--r--   0        0        0      246 2023-06-02 13:12:07.532000 mkdocs_dsfr-0.0.4/dsfr/icons/editor/list-ordered.svg
+-rw-r--r--   0        0        0      275 2023-06-02 13:12:07.532999 mkdocs_dsfr-0.0.4/dsfr/icons/editor/list-unordered.svg
+-rw-r--r--   0        0        0      341 2023-06-02 13:12:07.585999 mkdocs_dsfr-0.0.4/dsfr/icons/editor/question-mark.svg
+-rw-r--r--   0        0        0      147 2023-06-02 13:12:07.599999 mkdocs_dsfr-0.0.4/dsfr/icons/editor/separator.svg
+-rw-r--r--   0        0        0      151 2023-06-02 13:12:07.611000 mkdocs_dsfr-0.0.4/dsfr/icons/editor/space.svg
+-rw-r--r--   0        0        0      317 2023-06-02 13:12:07.615999 mkdocs_dsfr-0.0.4/dsfr/icons/editor/subscript.svg
+-rw-r--r--   0        0        0      315 2023-06-02 13:12:07.618999 mkdocs_dsfr-0.0.4/dsfr/icons/editor/superscript.svg
+-rw-r--r--   0        0        0      263 2023-06-02 13:12:07.622999 mkdocs_dsfr-0.0.4/dsfr/icons/editor/table-2.svg
+-rw-r--r--   0        0        0      505 2023-06-02 13:12:07.638000 mkdocs_dsfr-0.0.4/dsfr/icons/editor/translate-2.svg
+-rw-r--r--   0        0        0      206 2023-06-02 13:12:07.391999 mkdocs_dsfr-0.0.4/dsfr/icons/finance/bank-card-fill.svg
+-rw-r--r--   0        0        0      220 2023-06-02 13:12:07.392999 mkdocs_dsfr-0.0.4/dsfr/icons/finance/bank-card-line.svg
+-rw-r--r--   0        0        0      277 2023-06-02 13:12:07.426000 mkdocs_dsfr-0.0.4/dsfr/icons/finance/coin-fill.svg
+-rw-r--r--   0        0        0      393 2023-06-02 13:12:07.487999 mkdocs_dsfr-0.0.4/dsfr/icons/finance/gift-fill.svg
+-rw-r--r--   0        0        0      406 2023-06-02 13:12:07.489000 mkdocs_dsfr-0.0.4/dsfr/icons/finance/gift-line.svg
+-rw-r--r--   0        0        0      366 2023-06-02 13:12:07.552999 mkdocs_dsfr-0.0.4/dsfr/icons/finance/money-euro-box-fill.svg
+-rw-r--r--   0        0        0      344 2023-06-02 13:12:07.552999 mkdocs_dsfr-0.0.4/dsfr/icons/finance/money-euro-box-line.svg
+-rw-r--r--   0        0        0      365 2023-06-02 13:12:07.552999 mkdocs_dsfr-0.0.4/dsfr/icons/finance/money-euro-circle-fill.svg
+-rw-r--r--   0        0        0      362 2023-06-02 13:12:07.553999 mkdocs_dsfr-0.0.4/dsfr/icons/finance/money-euro-circle-line.svg
+-rw-r--r--   0        0        0      397 2023-06-02 13:12:07.598000 mkdocs_dsfr-0.0.4/dsfr/icons/finance/secure-payment-fill.svg
+-rw-r--r--   0        0        0      427 2023-06-02 13:12:07.598000 mkdocs_dsfr-0.0.4/dsfr/icons/finance/secure-payment-line.svg
+-rw-r--r--   0        0        0      348 2023-06-02 13:12:07.604000 mkdocs_dsfr-0.0.4/dsfr/icons/finance/shopping-bag-fill.svg
+-rw-r--r--   0        0        0      282 2023-06-02 13:12:07.604000 mkdocs_dsfr-0.0.4/dsfr/icons/finance/shopping-bag-line.svg
+-rw-r--r--   0        0        0      311 2023-06-02 13:12:07.605000 mkdocs_dsfr-0.0.4/dsfr/icons/finance/shopping-cart-2-fill.svg
+-rw-r--r--   0        0        0      343 2023-06-02 13:12:07.605000 mkdocs_dsfr-0.0.4/dsfr/icons/finance/shopping-cart-2-line.svg
+-rw-r--r--   0        0        0      200 2023-06-02 13:12:07.638000 mkdocs_dsfr-0.0.4/dsfr/icons/finance/trophy-fill.svg
+-rw-r--r--   0        0        0      222 2023-06-02 13:12:07.638999 mkdocs_dsfr-0.0.4/dsfr/icons/finance/trophy-line.svg
+-rw-r--r--   0        0        0      289 2023-06-02 13:12:07.410000 mkdocs_dsfr-0.0.4/dsfr/icons/health/capsule-fill.svg
+-rw-r--r--   0        0        0      379 2023-06-02 13:12:07.410000 mkdocs_dsfr-0.0.4/dsfr/icons/health/capsule-line.svg
+-rw-r--r--   0        0        0      336 2023-06-02 13:12:07.441999 mkdocs_dsfr-0.0.4/dsfr/icons/health/dislike-fill.svg
+-rw-r--r--   0        0        0      543 2023-06-02 13:12:07.443000 mkdocs_dsfr-0.0.4/dsfr/icons/health/dislike-line.svg
+-rw-r--r--   0        0        0      243 2023-06-02 13:12:07.444999 mkdocs_dsfr-0.0.4/dsfr/icons/health/dossier-fill.svg
+-rw-r--r--   0        0        0      265 2023-06-02 13:12:07.444999 mkdocs_dsfr-0.0.4/dsfr/icons/health/dossier-line.svg
+-rw-r--r--   0        0        0      269 2023-06-02 13:12:07.467999 mkdocs_dsfr-0.0.4/dsfr/icons/health/first-aid-kit-fill.svg
+-rw-r--r--   0        0        0      283 2023-06-02 13:12:07.469000 mkdocs_dsfr-0.0.4/dsfr/icons/health/first-aid-kit-line.svg
+-rw-r--r--   0        0        0      317 2023-06-02 13:12:07.507999 mkdocs_dsfr-0.0.4/dsfr/icons/health/hand-sanitizer-fill.svg
+-rw-r--r--   0        0        0      359 2023-06-02 13:12:07.507999 mkdocs_dsfr-0.0.4/dsfr/icons/health/hand-sanitizer-line.svg
+-rw-r--r--   0        0        0      258 2023-06-02 13:12:07.509999 mkdocs_dsfr-0.0.4/dsfr/icons/health/health-book-fill.svg
+-rw-r--r--   0        0        0      273 2023-06-02 13:12:07.510999 mkdocs_dsfr-0.0.4/dsfr/icons/health/health-book-line.svg
+-rw-r--r--   0        0        0      209 2023-06-02 13:12:07.512000 mkdocs_dsfr-0.0.4/dsfr/icons/health/heart-fill.svg
+-rw-r--r--   0        0        0      365 2023-06-02 13:12:07.513000 mkdocs_dsfr-0.0.4/dsfr/icons/health/heart-line.svg
+-rw-r--r--   0        0        0      331 2023-06-02 13:12:07.513000 mkdocs_dsfr-0.0.4/dsfr/icons/health/heart-pulse-fill.svg
+-rw-r--r--   0        0        0      661 2023-06-02 13:12:07.513000 mkdocs_dsfr-0.0.4/dsfr/icons/health/heart-pulse-line.svg
+-rw-r--r--   0        0        0      476 2023-06-02 13:12:07.538000 mkdocs_dsfr-0.0.4/dsfr/icons/health/lungs-fill.svg
+-rw-r--r--   0        0        0      909 2023-06-02 13:12:07.539000 mkdocs_dsfr-0.0.4/dsfr/icons/health/lungs-line.svg
+-rw-r--r--   0        0        0      241 2023-06-02 13:12:07.548000 mkdocs_dsfr-0.0.4/dsfr/icons/health/medicine-bottle-fill.svg
+-rw-r--r--   0        0        0      293 2023-06-02 13:12:07.548000 mkdocs_dsfr-0.0.4/dsfr/icons/health/medicine-bottle-line.svg
+-rw-r--r--   0        0        0      395 2023-06-02 13:12:07.548000 mkdocs_dsfr-0.0.4/dsfr/icons/health/mental-health-fill.svg
+-rw-r--r--   0        0        0      503 2023-06-02 13:12:07.549000 mkdocs_dsfr-0.0.4/dsfr/icons/health/mental-health-line.svg
+-rw-r--r--   0        0        0      519 2023-06-02 13:12:07.552000 mkdocs_dsfr-0.0.4/dsfr/icons/health/microscope-fill.svg
+-rw-r--r--   0        0        0      618 2023-06-02 13:12:07.552000 mkdocs_dsfr-0.0.4/dsfr/icons/health/microscope-line.svg
+-rw-r--r--   0        0        0      370 2023-06-02 13:12:07.582000 mkdocs_dsfr-0.0.4/dsfr/icons/health/psychotherapy-fill.svg
+-rw-r--r--   0        0        0      504 2023-06-02 13:12:07.582999 mkdocs_dsfr-0.0.4/dsfr/icons/health/psychotherapy-line.svg
+-rw-r--r--   0        0        0      181 2023-06-02 13:12:07.582999 mkdocs_dsfr-0.0.4/dsfr/icons/health/pulse-line.svg
+-rw-r--r--   0        0        0      311 2023-06-02 13:12:07.612999 mkdocs_dsfr-0.0.4/dsfr/icons/health/stethoscope-fill.svg
+-rw-r--r--   0        0        0      346 2023-06-02 13:12:07.614000 mkdocs_dsfr-0.0.4/dsfr/icons/health/stethoscope-line.svg
+-rw-r--r--   0        0        0      446 2023-06-02 13:12:07.618999 mkdocs_dsfr-0.0.4/dsfr/icons/health/surgical-mask-fill.svg
+-rw-r--r--   0        0        0      567 2023-06-02 13:12:07.619999 mkdocs_dsfr-0.0.4/dsfr/icons/health/surgical-mask-line.svg
+-rw-r--r--   0        0        0      466 2023-06-02 13:12:07.621000 mkdocs_dsfr-0.0.4/dsfr/icons/health/syringe-fill.svg
+-rw-r--r--   0        0        0      486 2023-06-02 13:12:07.621000 mkdocs_dsfr-0.0.4/dsfr/icons/health/syringe-line.svg
+-rw-r--r--   0        0        0      237 2023-06-02 13:12:07.631000 mkdocs_dsfr-0.0.4/dsfr/icons/health/test-tube-fill.svg
+-rw-r--r--   0        0        0      264 2023-06-02 13:12:07.631000 mkdocs_dsfr-0.0.4/dsfr/icons/health/test-tube-line.svg
+-rw-r--r--   0        0        0      484 2023-06-02 13:12:07.631999 mkdocs_dsfr-0.0.4/dsfr/icons/health/thermometer-fill.svg
+-rw-r--r--   0        0        0      576 2023-06-02 13:12:07.631999 mkdocs_dsfr-0.0.4/dsfr/icons/health/thermometer-line.svg
+-rw-r--r--   0        0        0     1055 2023-06-02 13:12:07.651999 mkdocs_dsfr-0.0.4/dsfr/icons/health/virus-fill.svg
+-rw-r--r--   0        0        0     1112 2023-06-02 13:12:07.653000 mkdocs_dsfr-0.0.4/dsfr/icons/health/virus-line.svg
+-rw-r--r--   0        0        0      552 2023-06-02 13:12:07.418999 mkdocs_dsfr-0.0.4/dsfr/icons/logo/chrome-fill.svg
+-rw-r--r--   0        0        0      594 2023-06-02 13:12:07.418999 mkdocs_dsfr-0.0.4/dsfr/icons/logo/chrome-line.svg
+-rw-r--r--   0        0        0      591 2023-06-02 13:12:07.450999 mkdocs_dsfr-0.0.4/dsfr/icons/logo/edge-fill.svg
+-rw-r--r--   0        0        0      411 2023-06-02 13:12:07.450999 mkdocs_dsfr-0.0.4/dsfr/icons/logo/edge-line.svg
+-rw-r--r--   0        0        0      368 2023-06-02 13:12:07.457999 mkdocs_dsfr-0.0.4/dsfr/icons/logo/facebook-circle-fill.svg
+-rw-r--r--   0        0        0      458 2023-06-02 13:12:07.459000 mkdocs_dsfr-0.0.4/dsfr/icons/logo/facebook-circle-line.svg
+-rw-r--r--   0        0        0      708 2023-06-02 13:12:07.467000 mkdocs_dsfr-0.0.4/dsfr/icons/logo/firefox-fill.svg
+-rw-r--r--   0        0        0     1003 2023-06-02 13:12:07.467999 mkdocs_dsfr-0.0.4/dsfr/icons/logo/firefox-line.svg
+-rw-r--r--   0        0        0      685 2023-06-02 13:12:07.474999 mkdocs_dsfr-0.0.4/dsfr/icons/logo/fr--dailymotion-fill.svg
+-rw-r--r--   0        0        0      806 2023-06-02 13:12:07.474999 mkdocs_dsfr-0.0.4/dsfr/icons/logo/fr--dailymotion-line.svg
+-rw-r--r--   0        0        0      561 2023-06-02 13:12:07.480000 mkdocs_dsfr-0.0.4/dsfr/icons/logo/fr--tiktok-fill.svg
+-rw-r--r--   0        0        0      428 2023-06-02 13:12:07.480000 mkdocs_dsfr-0.0.4/dsfr/icons/logo/fr--tiktok-line.svg
+-rw-r--r--   0        0        0      790 2023-06-02 13:12:07.497999 mkdocs_dsfr-0.0.4/dsfr/icons/logo/github-fill.svg
+-rw-r--r--   0        0        0     1485 2023-06-02 13:12:07.499000 mkdocs_dsfr-0.0.4/dsfr/icons/logo/github-line.svg
+-rw-r--r--   0        0        0      530 2023-06-02 13:12:07.500999 mkdocs_dsfr-0.0.4/dsfr/icons/logo/google-fill.svg
+-rw-r--r--   0        0        0      371 2023-06-02 13:12:07.500999 mkdocs_dsfr-0.0.4/dsfr/icons/logo/google-line.svg
+-rw-r--r--   0        0        0      965 2023-06-02 13:12:07.516999 mkdocs_dsfr-0.0.4/dsfr/icons/logo/ie-fill.svg
+-rw-r--r--   0        0        0      796 2023-06-02 13:12:07.517999 mkdocs_dsfr-0.0.4/dsfr/icons/logo/ie-line.svg
+-rw-r--r--   0        0        0      917 2023-06-02 13:12:07.523000 mkdocs_dsfr-0.0.4/dsfr/icons/logo/instagram-fill.svg
+-rw-r--r--   0        0        0     2014 2023-06-02 13:12:07.523000 mkdocs_dsfr-0.0.4/dsfr/icons/logo/instagram-line.svg
+-rw-r--r--   0        0        0      552 2023-06-02 13:12:07.530999 mkdocs_dsfr-0.0.4/dsfr/icons/logo/linkedin-box-fill.svg
+-rw-r--r--   0        0        0      366 2023-06-02 13:12:07.530999 mkdocs_dsfr-0.0.4/dsfr/icons/logo/linkedin-box-line.svg
+-rw-r--r--   0        0        0      948 2023-06-02 13:12:07.546000 mkdocs_dsfr-0.0.4/dsfr/icons/logo/mastodon-fill.svg
+-rw-r--r--   0        0        0     1259 2023-06-02 13:12:07.546999 mkdocs_dsfr-0.0.4/dsfr/icons/logo/mastodon-line.svg
+-rw-r--r--   0        0        0      202 2023-06-02 13:12:07.562000 mkdocs_dsfr-0.0.4/dsfr/icons/logo/npmjs-fill.svg
+-rw-r--r--   0        0        0      220 2023-06-02 13:12:07.562000 mkdocs_dsfr-0.0.4/dsfr/icons/logo/npmjs-line.svg
+-rw-r--r--   0        0        0      331 2023-06-02 13:12:07.588000 mkdocs_dsfr-0.0.4/dsfr/icons/logo/remixicon-fill.svg
+-rw-r--r--   0        0        0      391 2023-06-02 13:12:07.588999 mkdocs_dsfr-0.0.4/dsfr/icons/logo/remixicon-line.svg
+-rw-r--r--   0        0        0      972 2023-06-02 13:12:07.592000 mkdocs_dsfr-0.0.4/dsfr/icons/logo/safari-fill.svg
+-rw-r--r--   0        0        0      574 2023-06-02 13:12:07.592000 mkdocs_dsfr-0.0.4/dsfr/icons/logo/safari-line.svg
+-rw-r--r--   0        0        0     1133 2023-06-02 13:12:07.607000 mkdocs_dsfr-0.0.4/dsfr/icons/logo/slack-fill.svg
+-rw-r--r--   0        0        0      514 2023-06-02 13:12:07.607000 mkdocs_dsfr-0.0.4/dsfr/icons/logo/slack-line.svg
+-rw-r--r--   0        0        0     1494 2023-06-02 13:12:07.609999 mkdocs_dsfr-0.0.4/dsfr/icons/logo/snapchat-fill.svg
+-rw-r--r--   0        0        0     1848 2023-06-02 13:12:07.611000 mkdocs_dsfr-0.0.4/dsfr/icons/logo/snapchat-line.svg
+-rw-r--r--   0        0        0      398 2023-06-02 13:12:07.628000 mkdocs_dsfr-0.0.4/dsfr/icons/logo/telegram-fill.svg
+-rw-r--r--   0        0        0      440 2023-06-02 13:12:07.628999 mkdocs_dsfr-0.0.4/dsfr/icons/logo/telegram-line.svg
+-rw-r--r--   0        0        0      332 2023-06-02 13:12:07.640000 mkdocs_dsfr-0.0.4/dsfr/icons/logo/twitch-fill.svg
+-rw-r--r--   0        0        0      241 2023-06-02 13:12:07.641000 mkdocs_dsfr-0.0.4/dsfr/icons/logo/twitch-line.svg
+-rw-r--r--   0        0        0      586 2023-06-02 13:12:07.641000 mkdocs_dsfr-0.0.4/dsfr/icons/logo/twitter-fill.svg
+-rw-r--r--   0        0        0      690 2023-06-02 13:12:07.641999 mkdocs_dsfr-0.0.4/dsfr/icons/logo/twitter-line.svg
+-rw-r--r--   0        0        0      726 2023-06-02 13:12:07.651999 mkdocs_dsfr-0.0.4/dsfr/icons/logo/vimeo-fill.svg
+-rw-r--r--   0        0        0     1001 2023-06-02 13:12:07.651999 mkdocs_dsfr-0.0.4/dsfr/icons/logo/vimeo-line.svg
+-rw-r--r--   0        0        0      178 2023-06-02 13:12:07.655999 mkdocs_dsfr-0.0.4/dsfr/icons/logo/vuejs-fill.svg
+-rw-r--r--   0        0        0      198 2023-06-02 13:12:07.657000 mkdocs_dsfr-0.0.4/dsfr/icons/logo/vuejs-line.svg
+-rw-r--r--   0        0        0      418 2023-06-02 13:12:07.658999 mkdocs_dsfr-0.0.4/dsfr/icons/logo/youtube-fill.svg
+-rw-r--r--   0        0        0      899 2023-06-02 13:12:07.660000 mkdocs_dsfr-0.0.4/dsfr/icons/logo/youtube-line.svg
+-rw-r--r--   0        0        0      385 2023-06-02 13:12:07.377000 mkdocs_dsfr-0.0.4/dsfr/icons/map/anchor-fill.svg
+-rw-r--r--   0        0        0      350 2023-06-02 13:12:07.377000 mkdocs_dsfr-0.0.4/dsfr/icons/map/anchor-line.svg
+-rw-r--r--   0        0        0      359 2023-06-02 13:12:07.394000 mkdocs_dsfr-0.0.4/dsfr/icons/map/bike-fill.svg
+-rw-r--r--   0        0        0      359 2023-06-02 13:12:07.394999 mkdocs_dsfr-0.0.4/dsfr/icons/map/bike-line.svg
+-rw-r--r--   0        0        0      284 2023-06-02 13:12:07.404000 mkdocs_dsfr-0.0.4/dsfr/icons/map/bus-fill.svg
+-rw-r--r--   0        0        0      299 2023-06-02 13:12:07.404999 mkdocs_dsfr-0.0.4/dsfr/icons/map/bus-line.svg
+-rw-r--r--   0        0        0      372 2023-06-02 13:12:07.411000 mkdocs_dsfr-0.0.4/dsfr/icons/map/car-fill.svg
+-rw-r--r--   0        0        0      387 2023-06-02 13:12:07.411000 mkdocs_dsfr-0.0.4/dsfr/icons/map/car-line.svg
+-rw-r--r--   0        0        0      317 2023-06-02 13:12:07.411999 mkdocs_dsfr-0.0.4/dsfr/icons/map/caravan-fill.svg
+-rw-r--r--   0        0        0      383 2023-06-02 13:12:07.411999 mkdocs_dsfr-0.0.4/dsfr/icons/map/caravan-line.svg
+-rw-r--r--   0        0        0      253 2023-06-02 13:12:07.411999 mkdocs_dsfr-0.0.4/dsfr/icons/map/charging-pile-2-fill.svg
+-rw-r--r--   0        0        0      265 2023-06-02 13:12:07.413000 mkdocs_dsfr-0.0.4/dsfr/icons/map/charging-pile-2-line.svg
+-rw-r--r--   0        0        0      246 2023-06-02 13:12:07.427999 mkdocs_dsfr-0.0.4/dsfr/icons/map/compass-3-fill.svg
+-rw-r--r--   0        0        0      281 2023-06-02 13:12:07.427999 mkdocs_dsfr-0.0.4/dsfr/icons/map/compass-3-line.svg
+-rw-r--r--   0        0        0      222 2023-06-02 13:12:07.434000 mkdocs_dsfr-0.0.4/dsfr/icons/map/cup-fill.svg
+-rw-r--r--   0        0        0      264 2023-06-02 13:12:07.434999 mkdocs_dsfr-0.0.4/dsfr/icons/map/cup-line.svg
+-rw-r--r--   0        0        0      945 2023-06-02 13:12:07.450000 mkdocs_dsfr-0.0.4/dsfr/icons/map/earth-fill.svg
+-rw-r--r--   0        0        0      905 2023-06-02 13:12:07.450000 mkdocs_dsfr-0.0.4/dsfr/icons/map/earth-line.svg
+-rw-r--r--   0        0        0     2305 2023-06-02 13:12:07.480999 mkdocs_dsfr-0.0.4/dsfr/icons/map/france-fill.svg
+-rw-r--r--   0        0        0     4459 2023-06-02 13:12:07.482000 mkdocs_dsfr-0.0.4/dsfr/icons/map/france-line.svg
+-rw-r--r--   0        0        0      303 2023-06-02 13:12:07.483000 mkdocs_dsfr-0.0.4/dsfr/icons/map/gas-station-fill.svg
+-rw-r--r--   0        0        0      318 2023-06-02 13:12:07.483999 mkdocs_dsfr-0.0.4/dsfr/icons/map/gas-station-line.svg
+-rw-r--r--   0        0        0      179 2023-06-02 13:12:07.500000 mkdocs_dsfr-0.0.4/dsfr/icons/map/goblet-fill.svg
+-rw-r--r--   0        0        0      208 2023-06-02 13:12:07.500000 mkdocs_dsfr-0.0.4/dsfr/icons/map/goblet-line.svg
+-rw-r--r--   0        0        0      214 2023-06-02 13:12:07.542000 mkdocs_dsfr-0.0.4/dsfr/icons/map/map-pin-2-fill.svg
+-rw-r--r--   0        0        0      280 2023-06-02 13:12:07.542999 mkdocs_dsfr-0.0.4/dsfr/icons/map/map-pin-2-line.svg
+-rw-r--r--   0        0        0      277 2023-06-02 13:12:07.542999 mkdocs_dsfr-0.0.4/dsfr/icons/map/map-pin-user-fill.svg
+-rw-r--r--   0        0        0      363 2023-06-02 13:12:07.543999 mkdocs_dsfr-0.0.4/dsfr/icons/map/map-pin-user-line.svg
+-rw-r--r--   0        0        0      378 2023-06-02 13:12:07.556999 mkdocs_dsfr-0.0.4/dsfr/icons/map/motorbike-fill.svg
+-rw-r--r--   0        0        0      447 2023-06-02 13:12:07.558000 mkdocs_dsfr-0.0.4/dsfr/icons/map/motorbike-line.svg
+-rw-r--r--   0        0        0      256 2023-06-02 13:12:07.569000 mkdocs_dsfr-0.0.4/dsfr/icons/map/passport-fill.svg
+-rw-r--r--   0        0        0      272 2023-06-02 13:12:07.569999 mkdocs_dsfr-0.0.4/dsfr/icons/map/passport-line.svg
+-rw-r--r--   0        0        0      221 2023-06-02 13:12:07.588999 mkdocs_dsfr-0.0.4/dsfr/icons/map/restaurant-fill.svg
+-rw-r--r--   0        0        0      257 2023-06-02 13:12:07.588999 mkdocs_dsfr-0.0.4/dsfr/icons/map/restaurant-line.svg
+-rw-r--r--   0        0        0      381 2023-06-02 13:12:07.589999 mkdocs_dsfr-0.0.4/dsfr/icons/map/road-map-fill.svg
+-rw-r--r--   0        0        0      405 2023-06-02 13:12:07.591000 mkdocs_dsfr-0.0.4/dsfr/icons/map/road-map-line.svg
+-rw-r--r--   0        0        0      278 2023-06-02 13:12:07.592999 mkdocs_dsfr-0.0.4/dsfr/icons/map/sailboat-fill.svg
+-rw-r--r--   0        0        0      333 2023-06-02 13:12:07.592999 mkdocs_dsfr-0.0.4/dsfr/icons/map/sailboat-line.svg
+-rw-r--r--   0        0        0      580 2023-06-02 13:12:07.602999 mkdocs_dsfr-0.0.4/dsfr/icons/map/ship-2-fill.svg
+-rw-r--r--   0        0        0      562 2023-06-02 13:12:07.604000 mkdocs_dsfr-0.0.4/dsfr/icons/map/ship-2-line.svg
+-rw-r--r--   0        0        0      351 2023-06-02 13:12:07.605000 mkdocs_dsfr-0.0.4/dsfr/icons/map/signal-tower-fill.svg
+-rw-r--r--   0        0        0      348 2023-06-02 13:12:07.605999 mkdocs_dsfr-0.0.4/dsfr/icons/map/signal-tower-line.svg
+-rw-r--r--   0        0        0      271 2023-06-02 13:12:07.617000 mkdocs_dsfr-0.0.4/dsfr/icons/map/suitcase-2-fill.svg
+-rw-r--r--   0        0        0      286 2023-06-02 13:12:07.617000 mkdocs_dsfr-0.0.4/dsfr/icons/map/suitcase-2-line.svg
+-rw-r--r--   0        0        0      374 2023-06-02 13:12:07.625999 mkdocs_dsfr-0.0.4/dsfr/icons/map/taxi-fill.svg
+-rw-r--r--   0        0        0      386 2023-06-02 13:12:07.627000 mkdocs_dsfr-0.0.4/dsfr/icons/map/taxi-line.svg
+-rw-r--r--   0        0        0      251 2023-06-02 13:12:07.637000 mkdocs_dsfr-0.0.4/dsfr/icons/map/train-fill.svg
+-rw-r--r--   0        0        0      293 2023-06-02 13:12:07.637000 mkdocs_dsfr-0.0.4/dsfr/icons/map/train-line.svg
+-rw-r--r--   0        0        0      160 2023-06-02 13:12:07.375999 mkdocs_dsfr-0.0.4/dsfr/icons/media/align-left.svg
+-rw-r--r--   0        0        0      253 2023-06-02 13:12:07.408999 mkdocs_dsfr-0.0.4/dsfr/icons/media/camera-fill.svg
+-rw-r--r--   0        0        0      311 2023-06-02 13:12:07.408999 mkdocs_dsfr-0.0.4/dsfr/icons/media/camera-line.svg
+-rw-r--r--   0        0        0      294 2023-06-02 13:12:07.420000 mkdocs_dsfr-0.0.4/dsfr/icons/media/clapperboard-fill.svg
+-rw-r--r--   0        0        0      312 2023-06-02 13:12:07.421000 mkdocs_dsfr-0.0.4/dsfr/icons/media/clapperboard-line.svg
+-rw-r--r--   0        0        0      334 2023-06-02 13:12:07.453999 mkdocs_dsfr-0.0.4/dsfr/icons/media/equalizer-fill.svg
+-rw-r--r--   0        0        0      505 2023-06-02 13:12:07.454999 mkdocs_dsfr-0.0.4/dsfr/icons/media/equalizer-line.svg
+-rw-r--r--   0        0        0      340 2023-06-02 13:12:07.463999 mkdocs_dsfr-0.0.4/dsfr/icons/media/film-fill.svg
+-rw-r--r--   0        0        0      355 2023-06-02 13:12:07.464999 mkdocs_dsfr-0.0.4/dsfr/icons/media/film-line.svg
+-rw-r--r--   0        0        0      184 2023-06-02 13:12:07.482000 mkdocs_dsfr-0.0.4/dsfr/icons/media/fullscreen-line.svg
+-rw-r--r--   0        0        0      388 2023-06-02 13:12:07.483000 mkdocs_dsfr-0.0.4/dsfr/icons/media/gallery-fill.svg
+-rw-r--r--   0        0        0      466 2023-06-02 13:12:07.483000 mkdocs_dsfr-0.0.4/dsfr/icons/media/gallery-line.svg
+-rw-r--r--   0        0        0      261 2023-06-02 13:12:07.509999 mkdocs_dsfr-0.0.4/dsfr/icons/media/headphone-fill.svg
+-rw-r--r--   0        0        0      300 2023-06-02 13:12:07.509999 mkdocs_dsfr-0.0.4/dsfr/icons/media/headphone-line.svg
+-rw-r--r--   0        0        0      394 2023-06-02 13:12:07.517999 mkdocs_dsfr-0.0.4/dsfr/icons/media/image-add-fill.svg
+-rw-r--r--   0        0        0      316 2023-06-02 13:12:07.519000 mkdocs_dsfr-0.0.4/dsfr/icons/media/image-add-line.svg
+-rw-r--r--   0        0        0      398 2023-06-02 13:12:07.519000 mkdocs_dsfr-0.0.4/dsfr/icons/media/image-edit-fill.svg
+-rw-r--r--   0        0        0      415 2023-06-02 13:12:07.519000 mkdocs_dsfr-0.0.4/dsfr/icons/media/image-edit-line.svg
+-rw-r--r--   0        0        0      307 2023-06-02 13:12:07.519999 mkdocs_dsfr-0.0.4/dsfr/icons/media/image-fill.svg
+-rw-r--r--   0        0        0      334 2023-06-02 13:12:07.519999 mkdocs_dsfr-0.0.4/dsfr/icons/media/image-line.svg
+-rw-r--r--   0        0        0      394 2023-06-02 13:12:07.532999 mkdocs_dsfr-0.0.4/dsfr/icons/media/live-fill.svg
+-rw-r--r--   0        0        0      408 2023-06-02 13:12:07.532999 mkdocs_dsfr-0.0.4/dsfr/icons/media/live-line.svg
+-rw-r--r--   0        0        0      269 2023-06-02 13:12:07.551000 mkdocs_dsfr-0.0.4/dsfr/icons/media/mic-fill.svg
+-rw-r--r--   0        0        0      320 2023-06-02 13:12:07.551000 mkdocs_dsfr-0.0.4/dsfr/icons/media/mic-line.svg
+-rw-r--r--   0        0        0      158 2023-06-02 13:12:07.559000 mkdocs_dsfr-0.0.4/dsfr/icons/media/music-2-fill.svg
+-rw-r--r--   0        0        0      226 2023-06-02 13:12:07.559000 mkdocs_dsfr-0.0.4/dsfr/icons/media/music-2-line.svg
+-rw-r--r--   0        0        0      154 2023-06-02 13:12:07.559999 mkdocs_dsfr-0.0.4/dsfr/icons/media/notification-3-fill.svg
+-rw-r--r--   0        0        0      208 2023-06-02 13:12:07.561000 mkdocs_dsfr-0.0.4/dsfr/icons/media/notification-3-line.svg
+-rw-r--r--   0        0        0      201 2023-06-02 13:12:07.571000 mkdocs_dsfr-0.0.4/dsfr/icons/media/pause-circle-fill.svg
+-rw-r--r--   0        0        0      236 2023-06-02 13:12:07.571000 mkdocs_dsfr-0.0.4/dsfr/icons/media/pause-circle-line.svg
+-rw-r--r--   0        0        0      281 2023-06-02 13:12:07.578000 mkdocs_dsfr-0.0.4/dsfr/icons/media/play-circle-fill.svg
+-rw-r--r--   0        0        0      313 2023-06-02 13:12:07.578000 mkdocs_dsfr-0.0.4/dsfr/icons/media/play-circle-line.svg
+-rw-r--r--   0        0        0      186 2023-06-02 13:12:07.614000 mkdocs_dsfr-0.0.4/dsfr/icons/media/stop-circle-fill.svg
+-rw-r--r--   0        0        0      221 2023-06-02 13:12:07.614000 mkdocs_dsfr-0.0.4/dsfr/icons/media/stop-circle-line.svg
+-rw-r--r--   0        0        0      403 2023-06-02 13:12:07.654000 mkdocs_dsfr-0.0.4/dsfr/icons/media/volume-down-fill.svg
+-rw-r--r--   0        0        0      489 2023-06-02 13:12:07.654000 mkdocs_dsfr-0.0.4/dsfr/icons/media/volume-down-line.svg
+-rw-r--r--   0        0        0      407 2023-06-02 13:12:07.654999 mkdocs_dsfr-0.0.4/dsfr/icons/media/volume-mute-fill.svg
+-rw-r--r--   0        0        0      490 2023-06-02 13:12:07.654999 mkdocs_dsfr-0.0.4/dsfr/icons/media/volume-mute-line.svg
+-rw-r--r--   0        0        0      551 2023-06-02 13:12:07.654999 mkdocs_dsfr-0.0.4/dsfr/icons/media/volume-up-fill.svg
+-rw-r--r--   0        0        0      630 2023-06-02 13:12:07.655999 mkdocs_dsfr-0.0.4/dsfr/icons/media/volume-up-line.svg
+-rw-r--r--   0        0        0      334 2023-06-02 13:12:07.526000 mkdocs_dsfr-0.0.4/dsfr/icons/others/leaf-fill.svg
+-rw-r--r--   0        0        0      467 2023-06-02 13:12:07.526999 mkdocs_dsfr-0.0.4/dsfr/icons/others/leaf-line.svg
+-rw-r--r--   0        0        0      253 2023-06-02 13:12:07.528000 mkdocs_dsfr-0.0.4/dsfr/icons/others/lightbulb-fill.svg
+-rw-r--r--   0        0        0      406 2023-06-02 13:12:07.528000 mkdocs_dsfr-0.0.4/dsfr/icons/others/lightbulb-line.svg
+-rw-r--r--   0        0        0      277 2023-06-02 13:12:07.575999 mkdocs_dsfr-0.0.4/dsfr/icons/others/plant-fill.svg
+-rw-r--r--   0        0        0      362 2023-06-02 13:12:07.576999 mkdocs_dsfr-0.0.4/dsfr/icons/others/plant-line.svg
+-rw-r--r--   0        0        0      573 2023-06-02 13:12:07.586999 mkdocs_dsfr-0.0.4/dsfr/icons/others/recycle-fill.svg
+-rw-r--r--   0        0        0      558 2023-06-02 13:12:07.586999 mkdocs_dsfr-0.0.4/dsfr/icons/others/recycle-line.svg
+-rw-r--r--   0        0        0      454 2023-06-02 13:12:07.595000 mkdocs_dsfr-0.0.4/dsfr/icons/others/scales-3-fill.svg
+-rw-r--r--   0        0        0      552 2023-06-02 13:12:07.595999 mkdocs_dsfr-0.0.4/dsfr/icons/others/scales-3-line.svg
+-rw-r--r--   0        0        0      258 2023-06-02 13:12:07.598000 mkdocs_dsfr-0.0.4/dsfr/icons/others/seedling-fill.svg
+-rw-r--r--   0        0        0      326 2023-06-02 13:12:07.598999 mkdocs_dsfr-0.0.4/dsfr/icons/others/seedling-line.svg
+-rw-r--r--   0        0        0      232 2023-06-02 13:12:07.641999 mkdocs_dsfr-0.0.4/dsfr/icons/others/umbrella-fill.svg
+-rw-r--r--   0        0        0      315 2023-06-02 13:12:07.641999 mkdocs_dsfr-0.0.4/dsfr/icons/others/umbrella-line.svg
+-rw-r--r--   0        0        0      209 2023-06-02 13:12:07.369999 mkdocs_dsfr-0.0.4/dsfr/icons/system/add-circle-fill.svg
+-rw-r--r--   0        0        0      260 2023-06-02 13:12:07.371000 mkdocs_dsfr-0.0.4/dsfr/icons/system/add-circle-line.svg
+-rw-r--r--   0        0        0      136 2023-06-02 13:12:07.371000 mkdocs_dsfr-0.0.4/dsfr/icons/system/add-line.svg
+-rw-r--r--   0        0        0      319 2023-06-02 13:12:07.372999 mkdocs_dsfr-0.0.4/dsfr/icons/system/alarm-warning-fill.svg
+-rw-r--r--   0        0        0      360 2023-06-02 13:12:07.374000 mkdocs_dsfr-0.0.4/dsfr/icons/system/alarm-warning-line.svg
+-rw-r--r--   0        0        0      224 2023-06-02 13:12:07.374000 mkdocs_dsfr-0.0.4/dsfr/icons/system/alert-fill.svg
+-rw-r--r--   0        0        0      257 2023-06-02 13:12:07.375000 mkdocs_dsfr-0.0.4/dsfr/icons/system/alert-line.svg
+-rw-r--r--   0        0        0      127 2023-06-02 13:12:07.380000 mkdocs_dsfr-0.0.4/dsfr/icons/system/arrow-down-fill.svg
+-rw-r--r--   0        0        0      188 2023-06-02 13:12:07.381000 mkdocs_dsfr-0.0.4/dsfr/icons/system/arrow-down-line.svg
+-rw-r--r--   0        0        0      120 2023-06-02 13:12:07.381000 mkdocs_dsfr-0.0.4/dsfr/icons/system/arrow-down-s-fill.svg
+-rw-r--r--   0        0        0      173 2023-06-02 13:12:07.381000 mkdocs_dsfr-0.0.4/dsfr/icons/system/arrow-down-s-line.svg
+-rw-r--r--   0        0        0      159 2023-06-02 13:12:07.381999 mkdocs_dsfr-0.0.4/dsfr/icons/system/arrow-go-back-fill.svg
+-rw-r--r--   0        0        0      213 2023-06-02 13:12:07.382999 mkdocs_dsfr-0.0.4/dsfr/icons/system/arrow-go-back-line.svg
+-rw-r--r--   0        0        0      161 2023-06-02 13:12:07.382999 mkdocs_dsfr-0.0.4/dsfr/icons/system/arrow-go-forward-fill.svg
+-rw-r--r--   0        0        0      218 2023-06-02 13:12:07.382999 mkdocs_dsfr-0.0.4/dsfr/icons/system/arrow-go-forward-line.svg
+-rw-r--r--   0        0        0      128 2023-06-02 13:12:07.382999 mkdocs_dsfr-0.0.4/dsfr/icons/system/arrow-left-fill.svg
+-rw-r--r--   0        0        0      184 2023-06-02 13:12:07.384000 mkdocs_dsfr-0.0.4/dsfr/icons/system/arrow-left-line.svg
+-rw-r--r--   0        0        0      119 2023-06-02 13:12:07.384000 mkdocs_dsfr-0.0.4/dsfr/icons/system/arrow-left-s-fill.svg
+-rw-r--r--   0        0        0      173 2023-06-02 13:12:07.384999 mkdocs_dsfr-0.0.4/dsfr/icons/system/arrow-left-s-line.svg
+-rw-r--r--   0        0        0      128 2023-06-02 13:12:07.384999 mkdocs_dsfr-0.0.4/dsfr/icons/system/arrow-right-fill.svg
+-rw-r--r--   0        0        0      189 2023-06-02 13:12:07.384999 mkdocs_dsfr-0.0.4/dsfr/icons/system/arrow-right-line.svg
+-rw-r--r--   0        0        0      118 2023-06-02 13:12:07.385999 mkdocs_dsfr-0.0.4/dsfr/icons/system/arrow-right-s-fill.svg
+-rw-r--r--   0        0        0      175 2023-06-02 13:12:07.385999 mkdocs_dsfr-0.0.4/dsfr/icons/system/arrow-right-s-line.svg
+-rw-r--r--   0        0        0      197 2023-06-02 13:12:07.385999 mkdocs_dsfr-0.0.4/dsfr/icons/system/arrow-right-up-line.svg
+-rw-r--r--   0        0        0      129 2023-06-02 13:12:07.387000 mkdocs_dsfr-0.0.4/dsfr/icons/system/arrow-up-fill.svg
+-rw-r--r--   0        0        0      186 2023-06-02 13:12:07.387000 mkdocs_dsfr-0.0.4/dsfr/icons/system/arrow-up-line.svg
+-rw-r--r--   0        0        0      117 2023-06-02 13:12:07.387000 mkdocs_dsfr-0.0.4/dsfr/icons/system/arrow-up-s-fill.svg
+-rw-r--r--   0        0        0      173 2023-06-02 13:12:07.388000 mkdocs_dsfr-0.0.4/dsfr/icons/system/arrow-up-s-line.svg
+-rw-r--r--   0        0        0      177 2023-06-02 13:12:07.417000 mkdocs_dsfr-0.0.4/dsfr/icons/system/check-line.svg
+-rw-r--r--   0        0        0      252 2023-06-02 13:12:07.417000 mkdocs_dsfr-0.0.4/dsfr/icons/system/checkbox-circle-fill.svg
+-rw-r--r--   0        0        0      288 2023-06-02 13:12:07.417999 mkdocs_dsfr-0.0.4/dsfr/icons/system/checkbox-circle-line.svg
+-rw-r--r--   0        0        0      252 2023-06-02 13:12:07.417999 mkdocs_dsfr-0.0.4/dsfr/icons/system/checkbox-fill.svg
+-rw-r--r--   0        0        0      288 2023-06-02 13:12:07.417999 mkdocs_dsfr-0.0.4/dsfr/icons/system/checkbox-line.svg
+-rw-r--r--   0        0        0      321 2023-06-02 13:12:07.421999 mkdocs_dsfr-0.0.4/dsfr/icons/system/close-circle-fill.svg
+-rw-r--r--   0        0        0      342 2023-06-02 13:12:07.421999 mkdocs_dsfr-0.0.4/dsfr/icons/system/close-circle-line.svg
+-rw-r--r--   0        0        0      210 2023-06-02 13:12:07.421999 mkdocs_dsfr-0.0.4/dsfr/icons/system/close-line.svg
+-rw-r--r--   0        0        0      189 2023-06-02 13:12:07.438999 mkdocs_dsfr-0.0.4/dsfr/icons/system/delete-bin-fill.svg
+-rw-r--r--   0        0        0      203 2023-06-02 13:12:07.440000 mkdocs_dsfr-0.0.4/dsfr/icons/system/delete-bin-line.svg
+-rw-r--r--   0        0        0      142 2023-06-02 13:12:07.446000 mkdocs_dsfr-0.0.4/dsfr/icons/system/download-fill.svg
+-rw-r--r--   0        0        0      198 2023-06-02 13:12:07.446000 mkdocs_dsfr-0.0.4/dsfr/icons/system/download-line.svg
+-rw-r--r--   0        0        0      203 2023-06-02 13:12:07.454999 mkdocs_dsfr-0.0.4/dsfr/icons/system/error-warning-fill.svg
+-rw-r--r--   0        0        0      238 2023-06-02 13:12:07.454999 mkdocs_dsfr-0.0.4/dsfr/icons/system/error-warning-line.svg
+-rw-r--r--   0        0        0      228 2023-06-02 13:12:07.456000 mkdocs_dsfr-0.0.4/dsfr/icons/system/external-link-fill.svg
+-rw-r--r--   0        0        0      230 2023-06-02 13:12:07.456000 mkdocs_dsfr-0.0.4/dsfr/icons/system/external-link-line.svg
+-rw-r--r--   0        0        0      281 2023-06-02 13:12:07.457000 mkdocs_dsfr-0.0.4/dsfr/icons/system/eye-fill.svg
+-rw-r--r--   0        0        0      380 2023-06-02 13:12:07.457000 mkdocs_dsfr-0.0.4/dsfr/icons/system/eye-line.svg
+-rw-r--r--   0        0        0      481 2023-06-02 13:12:07.457000 mkdocs_dsfr-0.0.4/dsfr/icons/system/eye-off-fill.svg
+-rw-r--r--   0        0        0      678 2023-06-02 13:12:07.457999 mkdocs_dsfr-0.0.4/dsfr/icons/system/eye-off-line.svg
+-rw-r--r--   0        0        0      136 2023-06-02 13:12:07.464999 mkdocs_dsfr-0.0.4/dsfr/icons/system/filter-fill.svg
+-rw-r--r--   0        0        0      187 2023-06-02 13:12:07.466000 mkdocs_dsfr-0.0.4/dsfr/icons/system/filter-line.svg
+-rw-r--r--   0        0        0      196 2023-06-02 13:12:07.471999 mkdocs_dsfr-0.0.4/dsfr/icons/system/fr--arrow-left-s-first-line.svg
+-rw-r--r--   0        0        0      197 2023-06-02 13:12:07.471999 mkdocs_dsfr-0.0.4/dsfr/icons/system/fr--arrow-left-s-line-double.svg
+-rw-r--r--   0        0        0      377 2023-06-02 13:12:07.473000 mkdocs_dsfr-0.0.4/dsfr/icons/system/fr--arrow-right-down-circle-fill.svg
+-rw-r--r--   0        0        0      201 2023-06-02 13:12:07.473000 mkdocs_dsfr-0.0.4/dsfr/icons/system/fr--arrow-right-s-last-line.svg
+-rw-r--r--   0        0        0      201 2023-06-02 13:12:07.473000 mkdocs_dsfr-0.0.4/dsfr/icons/system/fr--arrow-right-s-line-double.svg
+-rw-r--r--   0        0        0      377 2023-06-02 13:12:07.473999 mkdocs_dsfr-0.0.4/dsfr/icons/system/fr--arrow-right-up-circle-fill.svg
+-rw-r--r--   0        0        0      327 2023-06-02 13:12:07.473999 mkdocs_dsfr-0.0.4/dsfr/icons/system/fr--capslock-line.svg
+-rw-r--r--   0        0        0      329 2023-06-02 13:12:07.474999 mkdocs_dsfr-0.0.4/dsfr/icons/system/fr--equal-circle-fill.svg
+-rw-r--r--   0        0        0      260 2023-06-02 13:12:07.476000 mkdocs_dsfr-0.0.4/dsfr/icons/system/fr--error-fill.svg
+-rw-r--r--   0        0        0      309 2023-06-02 13:12:07.476000 mkdocs_dsfr-0.0.4/dsfr/icons/system/fr--error-line.svg
+-rw-r--r--   0        0        0      237 2023-06-02 13:12:07.476999 mkdocs_dsfr-0.0.4/dsfr/icons/system/fr--info-fill.svg
+-rw-r--r--   0        0        0      328 2023-06-02 13:12:07.476999 mkdocs_dsfr-0.0.4/dsfr/icons/system/fr--info-line.svg
+-rw-r--r--   0        0        0      253 2023-06-02 13:12:07.477999 mkdocs_dsfr-0.0.4/dsfr/icons/system/fr--success-fill.svg
+-rw-r--r--   0        0        0      289 2023-06-02 13:12:07.479000 mkdocs_dsfr-0.0.4/dsfr/icons/system/fr--success-line.svg
+-rw-r--r--   0        0        0      482 2023-06-02 13:12:07.479000 mkdocs_dsfr-0.0.4/dsfr/icons/system/fr--theme-fill.svg
+-rw-r--r--   0        0        0      225 2023-06-02 13:12:07.480999 mkdocs_dsfr-0.0.4/dsfr/icons/system/fr--warning-fill.svg
+-rw-r--r--   0        0        0      258 2023-06-02 13:12:07.480999 mkdocs_dsfr-0.0.4/dsfr/icons/system/fr--warning-line.svg
+-rw-r--r--   0        0        0      205 2023-06-02 13:12:07.520999 mkdocs_dsfr-0.0.4/dsfr/icons/system/information-fill.svg
+-rw-r--r--   0        0        0      239 2023-06-02 13:12:07.520999 mkdocs_dsfr-0.0.4/dsfr/icons/system/information-line.svg
+-rw-r--r--   0        0        0      238 2023-06-02 13:12:07.535000 mkdocs_dsfr-0.0.4/dsfr/icons/system/lock-fill.svg
+-rw-r--r--   0        0        0      252 2023-06-02 13:12:07.535000 mkdocs_dsfr-0.0.4/dsfr/icons/system/lock-line.svg
+-rw-r--r--   0        0        0      252 2023-06-02 13:12:07.536000 mkdocs_dsfr-0.0.4/dsfr/icons/system/lock-unlock-fill.svg
+-rw-r--r--   0        0        0      268 2023-06-02 13:12:07.536000 mkdocs_dsfr-0.0.4/dsfr/icons/system/lock-unlock-line.svg
+-rw-r--r--   0        0        0      197 2023-06-02 13:12:07.536999 mkdocs_dsfr-0.0.4/dsfr/icons/system/logout-box-r-fill.svg
+-rw-r--r--   0        0        0      219 2023-06-02 13:12:07.538000 mkdocs_dsfr-0.0.4/dsfr/icons/system/logout-box-r-line.svg
+-rw-r--r--   0        0        0      145 2023-06-02 13:12:07.549000 mkdocs_dsfr-0.0.4/dsfr/icons/system/menu-2-fill.svg
+-rw-r--r--   0        0        0      145 2023-06-02 13:12:07.549999 mkdocs_dsfr-0.0.4/dsfr/icons/system/menu-fill.svg
+-rw-r--r--   0        0        0      248 2023-06-02 13:12:07.555999 mkdocs_dsfr-0.0.4/dsfr/icons/system/more-fill.svg
+-rw-r--r--   0        0        0      348 2023-06-02 13:12:07.555999 mkdocs_dsfr-0.0.4/dsfr/icons/system/more-line.svg
+-rw-r--r--   0        0        0      220 2023-06-02 13:12:07.561000 mkdocs_dsfr-0.0.4/dsfr/icons/system/notification-badge-fill.svg
+-rw-r--r--   0        0        0      288 2023-06-02 13:12:07.561000 mkdocs_dsfr-0.0.4/dsfr/icons/system/notification-badge-line.svg
+-rw-r--r--   0        0        0      311 2023-06-02 13:12:07.585000 mkdocs_dsfr-0.0.4/dsfr/icons/system/question-fill.svg
+-rw-r--r--   0        0        0      325 2023-06-02 13:12:07.585000 mkdocs_dsfr-0.0.4/dsfr/icons/system/question-line.svg
+-rw-r--r--   0        0        0      280 2023-06-02 13:12:07.586999 mkdocs_dsfr-0.0.4/dsfr/icons/system/refresh-fill.svg
+-rw-r--r--   0        0        0      244 2023-06-02 13:12:07.588000 mkdocs_dsfr-0.0.4/dsfr/icons/system/refresh-line.svg
+-rw-r--r--   0        0        0      247 2023-06-02 13:12:07.596999 mkdocs_dsfr-0.0.4/dsfr/icons/system/search-fill.svg
+-rw-r--r--   0        0        0      382 2023-06-02 13:12:07.596999 mkdocs_dsfr-0.0.4/dsfr/icons/system/search-line.svg
+-rw-r--r--   0        0        0      864 2023-06-02 13:12:07.601000 mkdocs_dsfr-0.0.4/dsfr/icons/system/settings-5-fill.svg
+-rw-r--r--   0        0        0     1599 2023-06-02 13:12:07.601999 mkdocs_dsfr-0.0.4/dsfr/icons/system/settings-5-line.svg
+-rw-r--r--   0        0        0      241 2023-06-02 13:12:07.601999 mkdocs_dsfr-0.0.4/dsfr/icons/system/shield-fill.svg
+-rw-r--r--   0        0        0      332 2023-06-02 13:12:07.601999 mkdocs_dsfr-0.0.4/dsfr/icons/system/shield-line.svg
+-rw-r--r--   0        0        0      217 2023-06-02 13:12:07.611999 mkdocs_dsfr-0.0.4/dsfr/icons/system/star-fill.svg
+-rw-r--r--   0        0        0      333 2023-06-02 13:12:07.611999 mkdocs_dsfr-0.0.4/dsfr/icons/system/star-line.svg
+-rw-r--r--   0        0        0      203 2023-06-02 13:12:07.611999 mkdocs_dsfr-0.0.4/dsfr/icons/system/star-s-fill.svg
+-rw-r--r--   0        0        0      325 2023-06-02 13:12:07.612999 mkdocs_dsfr-0.0.4/dsfr/icons/system/star-s-line.svg
+-rw-r--r--   0        0        0      117 2023-06-02 13:12:07.615999 mkdocs_dsfr-0.0.4/dsfr/icons/system/subtract-line.svg
+-rw-r--r--   0        0        0      341 2023-06-02 13:12:07.631999 mkdocs_dsfr-0.0.4/dsfr/icons/system/thumb-down-fill.svg
+-rw-r--r--   0        0        0      442 2023-06-02 13:12:07.632999 mkdocs_dsfr-0.0.4/dsfr/icons/system/thumb-down-line.svg
+-rw-r--r--   0        0        0      340 2023-06-02 13:12:07.632999 mkdocs_dsfr-0.0.4/dsfr/icons/system/thumb-up-fill.svg
+-rw-r--r--   0        0        0      459 2023-06-02 13:12:07.634000 mkdocs_dsfr-0.0.4/dsfr/icons/system/thumb-up-line.svg
+-rw-r--r--   0        0        0      193 2023-06-02 13:12:07.634000 mkdocs_dsfr-0.0.4/dsfr/icons/system/time-fill.svg
+-rw-r--r--   0        0        0      226 2023-06-02 13:12:07.634000 mkdocs_dsfr-0.0.4/dsfr/icons/system/time-line.svg
+-rw-r--r--   0        0        0      201 2023-06-02 13:12:07.634999 mkdocs_dsfr-0.0.4/dsfr/icons/system/timer-fill.svg
+-rw-r--r--   0        0        0      236 2023-06-02 13:12:07.634999 mkdocs_dsfr-0.0.4/dsfr/icons/system/timer-line.svg
+-rw-r--r--   0        0        0      180 2023-06-02 13:12:07.642999 mkdocs_dsfr-0.0.4/dsfr/icons/system/upload-2-fill.svg
+-rw-r--r--   0        0        0      180 2023-06-02 13:12:07.642999 mkdocs_dsfr-0.0.4/dsfr/icons/system/upload-2-line.svg
+-rw-r--r--   0        0        0      144 2023-06-02 13:12:07.644000 mkdocs_dsfr-0.0.4/dsfr/icons/system/upload-fill.svg
+-rw-r--r--   0        0        0      206 2023-06-02 13:12:07.644000 mkdocs_dsfr-0.0.4/dsfr/icons/system/upload-line.svg
+-rw-r--r--   0        0        0      279 2023-06-02 13:12:07.660000 mkdocs_dsfr-0.0.4/dsfr/icons/system/zoom-in-fill.svg
+-rw-r--r--   0        0        0      407 2023-06-02 13:12:07.660000 mkdocs_dsfr-0.0.4/dsfr/icons/system/zoom-in-line.svg
+-rw-r--r--   0        0        0      260 2023-06-02 13:12:07.661000 mkdocs_dsfr-0.0.4/dsfr/icons/system/zoom-out-fill.svg
+-rw-r--r--   0        0        0      388 2023-06-02 13:12:07.661000 mkdocs_dsfr-0.0.4/dsfr/icons/system/zoom-out-line.svg
+-rw-r--r--   0        0        0      337 2023-06-02 13:12:07.368999 mkdocs_dsfr-0.0.4/dsfr/icons/user/account-circle-fill.svg
+-rw-r--r--   0        0        0      462 2023-06-02 13:12:07.368999 mkdocs_dsfr-0.0.4/dsfr/icons/user/account-circle-line.svg
+-rw-r--r--   0        0        0      383 2023-06-02 13:12:07.368999 mkdocs_dsfr-0.0.4/dsfr/icons/user/account-pin-circle-fill.svg
+-rw-r--r--   0        0        0      575 2023-06-02 13:12:07.369999 mkdocs_dsfr-0.0.4/dsfr/icons/user/account-pin-circle-line.svg
+-rw-r--r--   0        0        0      279 2023-06-02 13:12:07.371000 mkdocs_dsfr-0.0.4/dsfr/icons/user/admin-fill.svg
+-rw-r--r--   0        0        0      349 2023-06-02 13:12:07.371999 mkdocs_dsfr-0.0.4/dsfr/icons/user/admin-line.svg
+-rw-r--r--   0        0        0      357 2023-06-02 13:12:07.503000 mkdocs_dsfr-0.0.4/dsfr/icons/user/group-fill.svg
+-rw-r--r--   0        0        0      462 2023-06-02 13:12:07.503999 mkdocs_dsfr-0.0.4/dsfr/icons/user/group-line.svg
+-rw-r--r--   0        0        0      279 2023-06-02 13:12:07.568000 mkdocs_dsfr-0.0.4/dsfr/icons/user/parent-fill.svg
+-rw-r--r--   0        0        0      413 2023-06-02 13:12:07.569000 mkdocs_dsfr-0.0.4/dsfr/icons/user/parent-line.svg
+-rw-r--r--   0        0        0      424 2023-06-02 13:12:07.627000 mkdocs_dsfr-0.0.4/dsfr/icons/user/team-fill.svg
+-rw-r--r--   0        0        0      750 2023-06-02 13:12:07.628000 mkdocs_dsfr-0.0.4/dsfr/icons/user/team-line.svg
+-rw-r--r--   0        0        0      235 2023-06-02 13:12:07.644000 mkdocs_dsfr-0.0.4/dsfr/icons/user/user-add-fill.svg
+-rw-r--r--   0        0        0      316 2023-06-02 13:12:07.644999 mkdocs_dsfr-0.0.4/dsfr/icons/user/user-add-line.svg
+-rw-r--r--   0        0        0      186 2023-06-02 13:12:07.644999 mkdocs_dsfr-0.0.4/dsfr/icons/user/user-fill.svg
+-rw-r--r--   0        0        0      314 2023-06-02 13:12:07.645999 mkdocs_dsfr-0.0.4/dsfr/icons/user/user-heart-fill.svg
+-rw-r--r--   0        0        0      439 2023-06-02 13:12:07.645999 mkdocs_dsfr-0.0.4/dsfr/icons/user/user-heart-line.svg
+-rw-r--r--   0        0        0      275 2023-06-02 13:12:07.647000 mkdocs_dsfr-0.0.4/dsfr/icons/user/user-line.svg
+-rw-r--r--   0        0        0      314 2023-06-02 13:12:07.647000 mkdocs_dsfr-0.0.4/dsfr/icons/user/user-search-fill.svg
+-rw-r--r--   0        0        0      384 2023-06-02 13:12:07.647000 mkdocs_dsfr-0.0.4/dsfr/icons/user/user-search-line.svg
+-rw-r--r--   0        0        0      529 2023-06-02 13:12:07.648000 mkdocs_dsfr-0.0.4/dsfr/icons/user/user-setting-fill.svg
+-rw-r--r--   0        0        0      462 2023-06-02 13:12:07.648000 mkdocs_dsfr-0.0.4/dsfr/icons/user/user-setting-line.svg
+-rw-r--r--   0        0        0      298 2023-06-02 13:12:07.648000 mkdocs_dsfr-0.0.4/dsfr/icons/user/user-star-fill.svg
+-rw-r--r--   0        0        0      367 2023-06-02 13:12:07.648999 mkdocs_dsfr-0.0.4/dsfr/icons/user/user-star-line.svg
+-rw-r--r--   0        0        0      167 2023-06-02 13:12:07.424000 mkdocs_dsfr-0.0.4/dsfr/icons/weather/cloudy-2-fill.svg
+-rw-r--r--   0        0        0      291 2023-06-02 13:12:07.424000 mkdocs_dsfr-0.0.4/dsfr/icons/weather/cloudy-2-line.svg
+-rw-r--r--   0        0        0      128 2023-06-02 13:12:07.470000 mkdocs_dsfr-0.0.4/dsfr/icons/weather/flashlight-fill.svg
+-rw-r--r--   0        0        0      172 2023-06-02 13:12:07.470000 mkdocs_dsfr-0.0.4/dsfr/icons/weather/flashlight-line.svg
+-rw-r--r--   0        0        0      226 2023-06-02 13:12:07.555000 mkdocs_dsfr-0.0.4/dsfr/icons/weather/moon-fill.svg
+-rw-r--r--   0        0        0      286 2023-06-02 13:12:07.555000 mkdocs_dsfr-0.0.4/dsfr/icons/weather/moon-line.svg
+-rw-r--r--   0        0        0      449 2023-06-02 13:12:07.618000 mkdocs_dsfr-0.0.4/dsfr/icons/weather/sun-fill.svg
+-rw-r--r--   0        0        0      482 2023-06-02 13:12:07.618000 mkdocs_dsfr-0.0.4/dsfr/icons/weather/sun-line.svg
+-rw-r--r--   0        0        0     1221 2023-05-31 09:02:28.010861 mkdocs_dsfr-0.0.4/dsfr/js/base.js
+-rw-r--r--   0        0        0    58073 2023-05-31 09:02:28.011124 mkdocs_dsfr-0.0.4/dsfr/js/bootstrap.min.js
+-rw-r--r--   0        0        0    93107 2023-05-31 09:02:28.011514 mkdocs_dsfr-0.0.4/dsfr/js/jquery-1.10.2.min.js
+-rw-r--r--   0        0        0     1553 2023-05-31 09:02:28.011584 mkdocs_dsfr-0.0.4/dsfr/lateral.html
+-rw-r--r--   0        0        0       25 2023-05-31 09:02:28.011646 mkdocs_dsfr-0.0.4/dsfr/main.html
+-rw-r--r--   0        0        0      174 2023-05-31 09:02:28.011702 mkdocs_dsfr-0.0.4/dsfr/mkdocs_theme.yml
+-rw-r--r--   0        0        0     1068 2023-05-31 09:02:28.011760 mkdocs_dsfr-0.0.4/dsfr/nav.html
+-rw-r--r--   0        0        0      743 2023-05-31 09:02:28.011819 mkdocs_dsfr-0.0.4/dsfr/prev-next-nav.html
+-rw-r--r--   0        0        0      575 2023-05-31 09:02:28.011878 mkdocs_dsfr-0.0.4/dsfr/search.html
+-rw-r--r--   0        0        0        0 2023-05-31 09:05:29.657662 mkdocs_dsfr-0.0.4/dsfr/tabs.html
+-rw-r--r--   0        0        0      748 2023-06-02 13:12:07.173000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/README.md
+-rw-r--r--   0        0        0      794 2023-06-02 13:12:07.171000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-buildings/README.md
+-rw-r--r--   0        0        0     8218 2023-06-02 13:12:06.513999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-buildings/icons-buildings.css
+-rw-r--r--   0        0        0    18287 2023-06-02 13:12:07.059999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-buildings/icons-buildings.css.map
+-rw-r--r--   0        0        0     3542 2023-06-02 13:12:06.513999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-buildings/icons-buildings.legacy.css
+-rw-r--r--   0        0        0     8457 2023-06-02 13:12:07.059999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-buildings/icons-buildings.legacy.css.map
+-rw-r--r--   0        0        0     3036 2023-06-02 13:12:06.513999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-buildings/icons-buildings.legacy.min.css
+-rw-r--r--   0        0        0     8332 2023-06-02 13:12:07.059999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-buildings/icons-buildings.legacy.min.css.map
+-rw-r--r--   0        0        0     4916 2023-06-02 13:12:06.513999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-buildings/icons-buildings.main.css
+-rw-r--r--   0        0        0    12037 2023-06-02 13:12:07.059999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-buildings/icons-buildings.main.css.map
+-rw-r--r--   0        0        0     4370 2023-06-02 13:12:06.513999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-buildings/icons-buildings.main.min.css
+-rw-r--r--   0        0        0    11358 2023-06-02 13:12:07.059999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-buildings/icons-buildings.main.min.css.map
+-rw-r--r--   0        0        0     7178 2023-06-02 13:12:06.513999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-buildings/icons-buildings.min.css
+-rw-r--r--   0        0        0    17475 2023-06-02 13:12:07.061000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-buildings/icons-buildings.min.css.map
+-rw-r--r--   0        0        0      788 2023-06-02 13:12:07.171000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-business/README.md
+-rw-r--r--   0        0        0    22912 2023-06-02 13:12:06.513999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-business/icons-business.css
+-rw-r--r--   0        0        0    36228 2023-06-02 13:12:07.061000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-business/icons-business.css.map
+-rw-r--r--   0        0        0     9504 2023-06-02 13:12:06.515000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-business/icons-business.legacy.css
+-rw-r--r--   0        0        0    15589 2023-06-02 13:12:07.061000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-business/icons-business.legacy.css.map
+-rw-r--r--   0        0        0     8088 2023-06-02 13:12:06.515000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-business/icons-business.legacy.min.css
+-rw-r--r--   0        0        0    15215 2023-06-02 13:12:07.061000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-business/icons-business.legacy.min.css.map
+-rw-r--r--   0        0        0    13648 2023-06-02 13:12:06.515000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-business/icons-business.main.css
+-rw-r--r--   0        0        0    22829 2023-06-02 13:12:07.062000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-business/icons-business.main.css.map
+-rw-r--r--   0        0        0    12243 2023-06-02 13:12:06.515000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-business/icons-business.main.min.css
+-rw-r--r--   0        0        0    21852 2023-06-02 13:12:07.062000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-business/icons-business.main.min.css.map
+-rw-r--r--   0        0        0    20103 2023-06-02 13:12:06.516000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-business/icons-business.min.css
+-rw-r--r--   0        0        0    34868 2023-06-02 13:12:07.062000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-business/icons-business.min.css.map
+-rw-r--r--   0        0        0      818 2023-06-02 13:12:07.171000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-communication/README.md
+-rw-r--r--   0        0        0     8770 2023-06-02 13:12:06.516000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-communication/icons-communication.css
+-rw-r--r--   0        0        0    18782 2023-06-02 13:12:07.062000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-communication/icons-communication.css.map
+-rw-r--r--   0        0        0     3786 2023-06-02 13:12:06.516000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-communication/icons-communication.legacy.css
+-rw-r--r--   0        0        0     8627 2023-06-02 13:12:07.062000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-communication/icons-communication.legacy.css.map
+-rw-r--r--   0        0        0     3272 2023-06-02 13:12:06.516000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-communication/icons-communication.legacy.min.css
+-rw-r--r--   0        0        0     8500 2023-06-02 13:12:07.062000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-communication/icons-communication.legacy.min.css.map
+-rw-r--r--   0        0        0     5224 2023-06-02 13:12:06.516000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-communication/icons-communication.main.css
+-rw-r--r--   0        0        0    12366 2023-06-02 13:12:07.062999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-communication/icons-communication.main.css.map
+-rw-r--r--   0        0        0     4674 2023-06-02 13:12:06.516999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-communication/icons-communication.main.min.css
+-rw-r--r--   0        0        0    11670 2023-06-02 13:12:07.062999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-communication/icons-communication.main.min.css.map
+-rw-r--r--   0        0        0     7718 2023-06-02 13:12:06.516999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-communication/icons-communication.min.css
+-rw-r--r--   0        0        0    17951 2023-06-02 13:12:07.062999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-communication/icons-communication.min.css.map
+-rw-r--r--   0        0        0      776 2023-06-02 13:12:07.171000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-design/README.md
+-rw-r--r--   0        0        0    15237 2023-06-02 13:12:06.516999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-design/icons-design.css
+-rw-r--r--   0        0        0    26942 2023-06-02 13:12:07.062999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-design/icons-design.css.map
+-rw-r--r--   0        0        0     6494 2023-06-02 13:12:06.516999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-design/icons-design.legacy.css
+-rw-r--r--   0        0        0    12000 2023-06-02 13:12:07.062999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-design/icons-design.legacy.css.map
+-rw-r--r--   0        0        0     5504 2023-06-02 13:12:06.516999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-design/icons-design.legacy.min.css
+-rw-r--r--   0        0        0    11743 2023-06-02 13:12:07.062999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-design/icons-design.legacy.min.css.map
+-rw-r--r--   0        0        0     8983 2023-06-02 13:12:06.516999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-design/icons-design.main.css
+-rw-r--r--   0        0        0    17146 2023-06-02 13:12:07.062999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-design/icons-design.main.css.map
+-rw-r--r--   0        0        0     8000 2023-06-02 13:12:06.516999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-design/icons-design.main.min.css
+-rw-r--r--   0        0        0    16324 2023-06-02 13:12:07.063999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-design/icons-design.main.min.css.map
+-rw-r--r--   0        0        0    13276 2023-06-02 13:12:06.516999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-design/icons-design.min.css
+-rw-r--r--   0        0        0    25855 2023-06-02 13:12:07.063999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-design/icons-design.min.css.map
+-rw-r--r--   0        0        0      806 2023-06-02 13:12:07.171000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-development/README.md
+-rw-r--r--   0        0        0    10584 2023-06-02 13:12:06.516999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-development/icons-development.css
+-rw-r--r--   0        0        0    20888 2023-06-02 13:12:07.063999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-development/icons-development.css.map
+-rw-r--r--   0        0        0     4556 2023-06-02 13:12:06.516999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-development/icons-development.legacy.css
+-rw-r--r--   0        0        0     9503 2023-06-02 13:12:07.063999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-development/icons-development.legacy.css.map
+-rw-r--r--   0        0        0     3954 2023-06-02 13:12:06.517999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-development/icons-development.legacy.min.css
+-rw-r--r--   0        0        0     9352 2023-06-02 13:12:07.063999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-development/icons-development.legacy.min.css.map
+-rw-r--r--   0        0        0     6268 2023-06-02 13:12:06.517999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-development/icons-development.main.css
+-rw-r--r--   0        0        0    13594 2023-06-02 13:12:07.065000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-development/icons-development.main.css.map
+-rw-r--r--   0        0        0     5638 2023-06-02 13:12:06.517999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-development/icons-development.main.min.css
+-rw-r--r--   0        0        0    12876 2023-06-02 13:12:07.065000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-development/icons-development.main.min.css.map
+-rw-r--r--   0        0        0     9364 2023-06-02 13:12:06.517999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-development/icons-development.min.css
+-rw-r--r--   0        0        0    20011 2023-06-02 13:12:07.065000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-development/icons-development.min.css.map
+-rw-r--r--   0        0        0      776 2023-06-02 13:12:07.171000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-device/README.md
+-rw-r--r--   0        0        0    13498 2023-06-02 13:12:06.517999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-device/icons-device.css
+-rw-r--r--   0        0        0    24915 2023-06-02 13:12:07.065000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-device/icons-device.css.map
+-rw-r--r--   0        0        0     5696 2023-06-02 13:12:06.517999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-device/icons-device.legacy.css
+-rw-r--r--   0        0        0    11099 2023-06-02 13:12:07.065000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-device/icons-device.legacy.css.map
+-rw-r--r--   0        0        0     4810 2023-06-02 13:12:06.517999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-device/icons-device.legacy.min.css
+-rw-r--r--   0        0        0    10870 2023-06-02 13:12:07.065000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-device/icons-device.legacy.min.css.map
+-rw-r--r--   0        0        0     8042 2023-06-02 13:12:06.517999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-device/icons-device.main.css
+-rw-r--r--   0        0        0    16020 2023-06-02 13:12:07.065000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-device/icons-device.main.css.map
+-rw-r--r--   0        0        0     7132 2023-06-02 13:12:06.517999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-device/icons-device.main.min.css
+-rw-r--r--   0        0        0    15219 2023-06-02 13:12:07.065999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-device/icons-device.main.min.css.map
+-rw-r--r--   0        0        0    11714 2023-06-02 13:12:06.517999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-device/icons-device.min.css
+-rw-r--r--   0        0        0    23877 2023-06-02 13:12:07.065999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-device/icons-device.min.css.map
+-rw-r--r--   0        0        0      788 2023-06-02 13:12:07.171999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-document/README.md
+-rw-r--r--   0        0        0    12044 2023-06-02 13:12:06.519000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-document/icons-document.css
+-rw-r--r--   0        0        0    23019 2023-06-02 13:12:07.065999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-document/icons-document.css.map
+-rw-r--r--   0        0        0     5060 2023-06-02 13:12:06.519000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-document/icons-document.legacy.css
+-rw-r--r--   0        0        0    10303 2023-06-02 13:12:07.065999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-document/icons-document.legacy.css.map
+-rw-r--r--   0        0        0     4306 2023-06-02 13:12:06.519000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-document/icons-document.legacy.min.css
+-rw-r--r--   0        0        0    10110 2023-06-02 13:12:07.065999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-document/icons-document.legacy.min.css.map
+-rw-r--r--   0        0        0     7224 2023-06-02 13:12:06.519000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-document/icons-document.main.css
+-rw-r--r--   0        0        0    14922 2023-06-02 13:12:07.066999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-document/icons-document.main.css.map
+-rw-r--r--   0        0        0     6434 2023-06-02 13:12:06.519000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-document/icons-document.main.min.css
+-rw-r--r--   0        0        0    14157 2023-06-02 13:12:07.066999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-document/icons-document.main.min.css.map
+-rw-r--r--   0        0        0    10512 2023-06-02 13:12:06.519000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-document/icons-document.min.css
+-rw-r--r--   0        0        0    22053 2023-06-02 13:12:07.066999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-document/icons-document.min.css.map
+-rw-r--r--   0        0        0      776 2023-06-02 13:12:07.171999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-editor/README.md
+-rw-r--r--   0        0        0    10188 2023-06-02 13:12:06.519000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-editor/icons-editor.css
+-rw-r--r--   0        0        0    21006 2023-06-02 13:12:07.066999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-editor/icons-editor.css.map
+-rw-r--r--   0        0        0     4282 2023-06-02 13:12:06.519000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-editor/icons-editor.legacy.css
+-rw-r--r--   0        0        0     9470 2023-06-02 13:12:07.066999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-editor/icons-editor.legacy.css.map
+-rw-r--r--   0        0        0     3576 2023-06-02 13:12:06.519000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-editor/icons-editor.legacy.min.css
+-rw-r--r--   0        0        0     9290 2023-06-02 13:12:07.068000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-editor/icons-editor.legacy.min.css.map
+-rw-r--r--   0        0        0     6146 2023-06-02 13:12:06.519000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-editor/icons-editor.main.css
+-rw-r--r--   0        0        0    13740 2023-06-02 13:12:07.068000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-editor/icons-editor.main.css.map
+-rw-r--r--   0        0        0     5396 2023-06-02 13:12:06.519999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-editor/icons-editor.main.min.css
+-rw-r--r--   0        0        0    12995 2023-06-02 13:12:07.068000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-editor/icons-editor.main.min.css.map
+-rw-r--r--   0        0        0     8744 2023-06-02 13:12:06.519999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-editor/icons-editor.min.css
+-rw-r--r--   0        0        0    20073 2023-06-02 13:12:07.068000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-editor/icons-editor.min.css.map
+-rw-r--r--   0        0        0      782 2023-06-02 13:12:07.171999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-finance/README.md
+-rw-r--r--   0        0        0     6775 2023-06-02 13:12:06.519999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-finance/icons-finance.css
+-rw-r--r--   0        0        0    16388 2023-06-02 13:12:07.068000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-finance/icons-finance.css.map
+-rw-r--r--   0        0        0     2988 2023-06-02 13:12:06.519999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-finance/icons-finance.legacy.css
+-rw-r--r--   0        0        0     7688 2023-06-02 13:12:07.069000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-finance/icons-finance.legacy.css.map
+-rw-r--r--   0        0        0     2584 2023-06-02 13:12:06.519999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-finance/icons-finance.legacy.min.css
+-rw-r--r--   0        0        0     7591 2023-06-02 13:12:07.069000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-finance/icons-finance.legacy.min.css.map
+-rw-r--r--   0        0        0     4027 2023-06-02 13:12:06.519999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-finance/icons-finance.main.css
+-rw-r--r--   0        0        0    10905 2023-06-02 13:12:07.069000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-finance/icons-finance.main.css.map
+-rw-r--r--   0        0        0     3577 2023-06-02 13:12:06.519999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-finance/icons-finance.main.min.css
+-rw-r--r--   0        0        0    10262 2023-06-02 13:12:07.069000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-finance/icons-finance.main.min.css.map
+-rw-r--r--   0        0        0     5933 2023-06-02 13:12:06.519999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-finance/icons-finance.min.css
+-rw-r--r--   0        0        0    15640 2023-06-02 13:12:07.069000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-finance/icons-finance.min.css.map
+-rw-r--r--   0        0        0      776 2023-06-02 13:12:07.171999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-health/README.md
+-rw-r--r--   0        0        0    14367 2023-06-02 13:12:06.519999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-health/icons-health.css
+-rw-r--r--   0        0        0    25626 2023-06-02 13:12:07.069000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-health/icons-health.css.map
+-rw-r--r--   0        0        0     6168 2023-06-02 13:12:06.519999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-health/icons-health.legacy.css
+-rw-r--r--   0        0        0    11461 2023-06-02 13:12:07.069999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-health/icons-health.legacy.css.map
+-rw-r--r--   0        0        0     5280 2023-06-02 13:12:06.520999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-health/icons-health.legacy.min.css
+-rw-r--r--   0        0        0    11232 2023-06-02 13:12:07.069999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-health/icons-health.legacy.min.css.map
+-rw-r--r--   0        0        0     8439 2023-06-02 13:12:06.520999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-health/icons-health.main.css
+-rw-r--r--   0        0        0    16369 2023-06-02 13:12:07.069999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-health/icons-health.main.css.map
+-rw-r--r--   0        0        0     7549 2023-06-02 13:12:06.520999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-health/icons-health.main.min.css
+-rw-r--r--   0        0        0    15575 2023-06-02 13:12:07.069999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-health/icons-health.main.min.css.map
+-rw-r--r--   0        0        0    12601 2023-06-02 13:12:06.520999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-health/icons-health.min.css
+-rw-r--r--   0        0        0    24595 2023-06-02 13:12:07.069999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-health/icons-health.min.css.map
+-rw-r--r--   0        0        0      764 2023-06-02 13:12:07.171999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-logo/README.md
+-rw-r--r--   0        0        0    24122 2023-06-02 13:12:06.522000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-logo/icons-logo.css
+-rw-r--r--   0        0        0    38165 2023-06-02 13:12:07.069999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-logo/icons-logo.css.map
+-rw-r--r--   0        0        0     9746 2023-06-02 13:12:06.522000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-logo/icons-logo.legacy.css
+-rw-r--r--   0        0        0    16087 2023-06-02 13:12:07.071000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-logo/icons-logo.legacy.css.map
+-rw-r--r--   0        0        0     8200 2023-06-02 13:12:06.522000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-logo/icons-logo.legacy.min.css
+-rw-r--r--   0        0        0    15676 2023-06-02 13:12:07.071000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-logo/icons-logo.legacy.min.css.map
+-rw-r--r--   0        0        0    14616 2023-06-02 13:12:06.522000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-logo/icons-logo.main.css
+-rw-r--r--   0        0        0    24218 2023-06-02 13:12:07.071000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-logo/icons-logo.main.css.map
+-rw-r--r--   0        0        0    13026 2023-06-02 13:12:06.522000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-logo/icons-logo.main.min.css
+-rw-r--r--   0        0        0    23185 2023-06-02 13:12:07.071000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-logo/icons-logo.main.min.css.map
+-rw-r--r--   0        0        0    20998 2023-06-02 13:12:06.522000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-logo/icons-logo.min.css
+-rw-r--r--   0        0        0    36712 2023-06-02 13:12:07.071000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-logo/icons-logo.min.css.map
+-rw-r--r--   0        0        0      758 2023-06-02 13:12:07.171999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-map/README.md
+-rw-r--r--   0        0        0    17550 2023-06-02 13:12:06.522000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-map/icons-map.css
+-rw-r--r--   0        0        0    29852 2023-06-02 13:12:07.072000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-map/icons-map.css.map
+-rw-r--r--   0        0        0     7456 2023-06-02 13:12:06.522000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-map/icons-map.legacy.css
+-rw-r--r--   0        0        0    13177 2023-06-02 13:12:07.072000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-map/icons-map.legacy.css.map
+-rw-r--r--   0        0        0     6298 2023-06-02 13:12:06.522000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-map/icons-map.legacy.min.css
+-rw-r--r--   0        0        0    12874 2023-06-02 13:12:07.072000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-map/icons-map.legacy.min.css.map
+-rw-r--r--   0        0        0    10334 2023-06-02 13:12:06.523000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-map/icons-map.main.css
+-rw-r--r--   0        0        0    18876 2023-06-02 13:12:07.072000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-map/icons-map.main.css.map
+-rw-r--r--   0        0        0     9184 2023-06-02 13:12:06.523000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-map/icons-map.main.min.css
+-rw-r--r--   0        0        0    18000 2023-06-02 13:12:07.072999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-map/icons-map.main.min.css.map
+-rw-r--r--   0        0        0    15254 2023-06-02 13:12:06.523000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-map/icons-map.min.css
+-rw-r--r--   0        0        0    28665 2023-06-02 13:12:07.072999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-map/icons-map.min.css.map
+-rw-r--r--   0        0        0      770 2023-06-02 13:12:07.173000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-media/README.md
+-rw-r--r--   0        0        0    19301 2023-06-02 13:12:06.523000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-media/icons-media.css
+-rw-r--r--   0        0        0    31920 2023-06-02 13:12:07.072999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-media/icons-media.css.map
+-rw-r--r--   0        0        0     7999 2023-06-02 13:12:06.523000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-media/icons-media.legacy.css
+-rw-r--r--   0        0        0    13839 2023-06-02 13:12:07.072999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-media/icons-media.legacy.css.map
+-rw-r--r--   0        0        0     6785 2023-06-02 13:12:06.523000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-media/icons-media.legacy.min.css
+-rw-r--r--   0        0        0    13520 2023-06-02 13:12:07.072999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-media/icons-media.legacy.min.css.map
+-rw-r--r--   0        0        0    11542 2023-06-02 13:12:06.523000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-media/icons-media.main.css
+-rw-r--r--   0        0        0    20284 2023-06-02 13:12:07.073999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-media/icons-media.main.css.map
+-rw-r--r--   0        0        0    10312 2023-06-02 13:12:06.523000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-media/icons-media.main.min.css
+-rw-r--r--   0        0        0    19374 2023-06-02 13:12:07.073999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-media/icons-media.main.min.css.map
+-rw-r--r--   0        0        0    16869 2023-06-02 13:12:06.523000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-media/icons-media.min.css
+-rw-r--r--   0        0        0    30683 2023-06-02 13:12:07.073999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-media/icons-media.min.css.map
+-rw-r--r--   0        0        0      776 2023-06-02 13:12:07.173000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-others/README.md
+-rw-r--r--   0        0        0     5250 2023-06-02 13:12:06.523999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-others/icons-others.css
+-rw-r--r--   0        0        0    14634 2023-06-02 13:12:07.073999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-others/icons-others.css.map
+-rw-r--r--   0        0        0     2350 2023-06-02 13:12:06.523999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-others/icons-others.legacy.css
+-rw-r--r--   0        0        0     6968 2023-06-02 13:12:07.073999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-others/icons-others.legacy.css.map
+-rw-r--r--   0        0        0     2012 2023-06-02 13:12:06.523999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-others/icons-others.legacy.min.css
+-rw-r--r--   0        0        0     6889 2023-06-02 13:12:07.075000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-others/icons-others.legacy.min.css.map
+-rw-r--r--   0        0        0     3140 2023-06-02 13:12:06.523999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-others/icons-others.main.css
+-rw-r--r--   0        0        0     9870 2023-06-02 13:12:07.075000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-others/icons-others.main.css.map
+-rw-r--r--   0        0        0     2750 2023-06-02 13:12:06.523999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-others/icons-others.main.min.css
+-rw-r--r--   0        0        0     9251 2023-06-02 13:12:07.075000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-others/icons-others.main.min.css.map
+-rw-r--r--   0        0        0     4534 2023-06-02 13:12:06.523999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-others/icons-others.min.css
+-rw-r--r--   0        0        0    13928 2023-06-02 13:12:07.075000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-others/icons-others.min.css.map
+-rw-r--r--   0        0        0      776 2023-06-02 13:12:07.173000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-system/README.md
+-rw-r--r--   0        0        0    61210 2023-06-02 13:12:06.525000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-system/icons-system.css
+-rw-r--r--   0        0        0    83686 2023-06-02 13:12:07.075999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-system/icons-system.css.map
+-rw-r--r--   0        0        0    24507 2023-06-02 13:12:06.525000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-system/icons-system.legacy.css
+-rw-r--r--   0        0        0    33766 2023-06-02 13:12:07.075999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-system/icons-system.legacy.css.map
+-rw-r--r--   0        0        0    20773 2023-06-02 13:12:06.525000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-system/icons-system.legacy.min.css
+-rw-r--r--   0        0        0    32754 2023-06-02 13:12:07.075999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-system/icons-system.legacy.min.css.map
+-rw-r--r--   0        0        0    36943 2023-06-02 13:12:06.525000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-system/icons-system.main.css
+-rw-r--r--   0        0        0    51783 2023-06-02 13:12:07.075999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-system/icons-system.main.css.map
+-rw-r--r--   0        0        0    33240 2023-06-02 13:12:06.525000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-system/icons-system.main.min.css
+-rw-r--r--   0        0        0    50018 2023-06-02 13:12:07.076999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-system/icons-system.main.min.css.map
+-rw-r--r--   0        0        0    53785 2023-06-02 13:12:06.525000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-system/icons-system.min.css
+-rw-r--r--   0        0        0    80902 2023-06-02 13:12:07.076999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-system/icons-system.min.css.map
+-rw-r--r--   0        0        0      764 2023-06-02 13:12:07.173000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-user/README.md
+-rw-r--r--   0        0        0    10694 2023-06-02 13:12:06.526000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-user/icons-user.css
+-rw-r--r--   0        0        0    21349 2023-06-02 13:12:07.076999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-user/icons-user.css.map
+-rw-r--r--   0        0        0     4602 2023-06-02 13:12:06.526000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-user/icons-user.legacy.css
+-rw-r--r--   0        0        0     9729 2023-06-02 13:12:07.078000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-user/icons-user.legacy.css.map
+-rw-r--r--   0        0        0     3920 2023-06-02 13:12:06.526000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-user/icons-user.legacy.min.css
+-rw-r--r--   0        0        0     9556 2023-06-02 13:12:07.078000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-user/icons-user.legacy.min.css.map
+-rw-r--r--   0        0        0     6332 2023-06-02 13:12:06.526000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-user/icons-user.main.css
+-rw-r--r--   0        0        0    13822 2023-06-02 13:12:07.078000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-user/icons-user.main.css.map
+-rw-r--r--   0        0        0     5622 2023-06-02 13:12:06.526000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-user/icons-user.main.min.css
+-rw-r--r--   0        0        0    13097 2023-06-02 13:12:07.078000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-user/icons-user.main.min.css.map
+-rw-r--r--   0        0        0     9314 2023-06-02 13:12:06.526000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-user/icons-user.min.css
+-rw-r--r--   0        0        0    20443 2023-06-02 13:12:07.078999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-user/icons-user.min.css.map
+-rw-r--r--   0        0        0      782 2023-06-02 13:12:07.173000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-weather/README.md
+-rw-r--r--   0        0        0     3858 2023-06-02 13:12:06.526000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-weather/icons-weather.css
+-rw-r--r--   0        0        0    13024 2023-06-02 13:12:07.078999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-weather/icons-weather.css.map
+-rw-r--r--   0        0        0     1726 2023-06-02 13:12:06.526000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-weather/icons-weather.legacy.css
+-rw-r--r--   0        0        0     6315 2023-06-02 13:12:07.078999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-weather/icons-weather.legacy.css.map
+-rw-r--r--   0        0        0     1484 2023-06-02 13:12:06.526000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-weather/icons-weather.legacy.min.css
+-rw-r--r--   0        0        0     6262 2023-06-02 13:12:07.078999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-weather/icons-weather.legacy.min.css.map
+-rw-r--r--   0        0        0     2372 2023-06-02 13:12:06.526000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-weather/icons-weather.main.css
+-rw-r--r--   0        0        0     8914 2023-06-02 13:12:07.078999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-weather/icons-weather.main.css.map
+-rw-r--r--   0        0        0     2062 2023-06-02 13:12:06.526000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-weather/icons-weather.main.min.css
+-rw-r--r--   0        0        0     8320 2023-06-02 13:12:07.079999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-weather/icons-weather.main.min.css.map
+-rw-r--r--   0        0        0     3318 2023-06-02 13:12:06.526999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-weather/icons-weather.min.css
+-rw-r--r--   0        0        0    12369 2023-06-02 13:12:07.079999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-weather/icons-weather.min.css.map
+-rw-r--r--   0        0        0   252525 2023-06-02 13:12:06.528000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons.css
+-rw-r--r--   0        0        0   338301 2023-06-02 13:12:07.081000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons.css.map
+-rw-r--r--   0        0        0   103243 2023-06-02 13:12:06.528000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons.legacy.css
+-rw-r--r--   0        0        0   134266 2023-06-02 13:12:07.081000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons.legacy.css.map
+-rw-r--r--   0        0        0    87075 2023-06-02 13:12:06.528000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons.legacy.min.css
+-rw-r--r--   0        0        0   129807 2023-06-02 13:12:07.082000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons.legacy.min.css.map
+-rw-r--r--   0        0        0   149522 2023-06-02 13:12:06.529000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons.main.css
+-rw-r--r--   0        0        0   204422 2023-06-02 13:12:07.082999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons.main.css.map
+-rw-r--r--   0        0        0   133091 2023-06-02 13:12:06.529000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons.main.min.css
+-rw-r--r--   0        0        0   190288 2023-06-02 13:12:07.082999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons.main.min.css.map
+-rw-r--r--   0        0        0   219938 2023-06-02 13:12:06.529999 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons.min.css
+-rw-r--r--   0        0        0   318184 2023-06-02 13:12:07.084000 mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons.min.css.map
+-rw-r--r--   0        0        0      583 2023-06-02 15:58:56.155844 mkdocs_dsfr-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      830 1970-01-01 00:00:00.000000 mkdocs_dsfr-0.0.4/PKG-INFO
```

### Comparing `mkdocs-dsfr-0.0.3/LICENSE` & `mkdocs_dsfr-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/base.html` & `mkdocs_dsfr-0.0.4/dsfr/base.html`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/css/theme.css` & `mkdocs_dsfr-0.0.4/dsfr/css/theme.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/dsfr.min.css` & `mkdocs_dsfr-0.0.4/dsfr/dsfr.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/dsfr.module.min.js` & `mkdocs_dsfr-0.0.4/dsfr/dsfr.module.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/dsfr.nomodule.min.js` & `mkdocs_dsfr-0.0.4/dsfr/dsfr.nomodule.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/favicon/android-chrome-192x192.png` & `mkdocs_dsfr-0.0.4/dsfr/favicon/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/favicon/android-chrome-512x512.png` & `mkdocs_dsfr-0.0.4/dsfr/favicon/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/favicon/apple-touch-icon.png` & `mkdocs_dsfr-0.0.4/dsfr/favicon/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/favicon/favicon.ico` & `mkdocs_dsfr-0.0.4/dsfr/favicon/favicon.ico`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/favicon/favicon.svg` & `mkdocs_dsfr-0.0.4/dsfr/favicon/favicon.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/fonts/Marianne-Bold.woff` & `mkdocs_dsfr-0.0.4/dsfr/fonts/Marianne-Bold.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/fonts/Marianne-Bold.woff2` & `mkdocs_dsfr-0.0.4/dsfr/fonts/Marianne-Bold.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/fonts/Marianne-Bold_Italic.woff` & `mkdocs_dsfr-0.0.4/dsfr/fonts/Marianne-Bold_Italic.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/fonts/Marianne-Bold_Italic.woff2` & `mkdocs_dsfr-0.0.4/dsfr/fonts/Marianne-Bold_Italic.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/fonts/Marianne-Light.woff` & `mkdocs_dsfr-0.0.4/dsfr/fonts/Marianne-Light.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/fonts/Marianne-Light.woff2` & `mkdocs_dsfr-0.0.4/dsfr/fonts/Marianne-Light.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/fonts/Marianne-Light_Italic.woff` & `mkdocs_dsfr-0.0.4/dsfr/fonts/Marianne-Light_Italic.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/fonts/Marianne-Light_Italic.woff2` & `mkdocs_dsfr-0.0.4/dsfr/fonts/Marianne-Light_Italic.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/fonts/Marianne-Medium.woff` & `mkdocs_dsfr-0.0.4/dsfr/fonts/Marianne-Medium.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/fonts/Marianne-Medium.woff2` & `mkdocs_dsfr-0.0.4/dsfr/fonts/Marianne-Medium.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/fonts/Marianne-Medium_Italic.woff` & `mkdocs_dsfr-0.0.4/dsfr/fonts/Marianne-Medium_Italic.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/fonts/Marianne-Medium_Italic.woff2` & `mkdocs_dsfr-0.0.4/dsfr/fonts/Marianne-Medium_Italic.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/fonts/Marianne-Regular.woff` & `mkdocs_dsfr-0.0.4/dsfr/fonts/Marianne-Regular.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/fonts/Marianne-Regular.woff2` & `mkdocs_dsfr-0.0.4/dsfr/fonts/Marianne-Regular.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/fonts/Marianne-Regular_Italic.woff` & `mkdocs_dsfr-0.0.4/dsfr/fonts/Marianne-Regular_Italic.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/fonts/Marianne-Regular_Italic.woff2` & `mkdocs_dsfr-0.0.4/dsfr/fonts/Marianne-Regular_Italic.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/fonts/Spectral-ExtraBold.woff` & `mkdocs_dsfr-0.0.4/dsfr/fonts/Spectral-ExtraBold.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/fonts/Spectral-ExtraBold.woff2` & `mkdocs_dsfr-0.0.4/dsfr/fonts/Spectral-ExtraBold.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/fonts/Spectral-Regular.woff` & `mkdocs_dsfr-0.0.4/dsfr/fonts/Spectral-Regular.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/fonts/Spectral-Regular.woff2` & `mkdocs_dsfr-0.0.4/dsfr/fonts/Spectral-Regular.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/footer.html` & `mkdocs_dsfr-0.0.4/dsfr/footer.html`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/header.html` & `mkdocs_dsfr-0.0.4/dsfr/header.html`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/buildings/ancient-gate-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/buildings/ancient-gate-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/buildings/store-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/buildings/store-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/business/global-fill.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/business/global-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/business/global-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/business/global-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/design/brush-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/design/brush-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/design/palette-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/design/palette-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/development/bug-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/development/bug-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/device/dashboard-3-fill.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/device/dashboard-3-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/device/dashboard-3-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/device/dashboard-3-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/device/phone-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/device/phone-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/device/wifi-fill.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/device/wifi-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/device/wifi-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/device/wifi-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/editor/h-3.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/editor/h-3.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/editor/h-6.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/editor/h-6.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/health/dislike-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/health/dislike-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/health/heart-pulse-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/health/heart-pulse-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/health/lungs-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/health/lungs-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/health/microscope-fill.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/health/microscope-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/health/microscope-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/health/microscope-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/health/surgical-mask-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/health/surgical-mask-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/health/thermometer-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/health/thermometer-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/health/virus-fill.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/health/virus-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/health/virus-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/health/virus-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/logo/chrome-fill.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/logo/chrome-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/logo/chrome-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/logo/chrome-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/logo/edge-fill.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/logo/edge-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/logo/firefox-fill.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/logo/firefox-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/logo/firefox-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/logo/firefox-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/logo/fr--dailymotion-fill.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/logo/fr--dailymotion-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/logo/fr--dailymotion-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/logo/fr--dailymotion-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/logo/fr--tiktok-fill.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/logo/fr--tiktok-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/logo/github-fill.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/logo/github-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/logo/github-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/logo/github-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/logo/google-fill.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/logo/google-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/logo/ie-fill.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/logo/ie-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/logo/ie-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/logo/ie-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/logo/instagram-fill.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/logo/instagram-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/logo/instagram-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/logo/instagram-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/logo/linkedin-box-fill.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/logo/linkedin-box-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/logo/mastodon-fill.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/logo/mastodon-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/logo/mastodon-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/logo/mastodon-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/logo/safari-fill.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/logo/safari-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/logo/safari-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/logo/safari-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/logo/slack-fill.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/logo/slack-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/logo/slack-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/logo/slack-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/logo/snapchat-fill.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/logo/snapchat-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/logo/snapchat-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/logo/snapchat-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/logo/twitter-fill.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/logo/twitter-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/logo/twitter-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/logo/twitter-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/logo/vimeo-fill.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/logo/vimeo-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/logo/vimeo-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/logo/vimeo-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/logo/youtube-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/logo/youtube-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/map/earth-fill.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/map/earth-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/map/earth-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/map/earth-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/map/france-fill.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/map/france-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/map/france-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/map/france-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/map/ship-2-fill.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/map/ship-2-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/map/ship-2-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/map/ship-2-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/media/volume-up-fill.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/media/volume-up-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/media/volume-up-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/media/volume-up-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/others/recycle-fill.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/others/recycle-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/others/recycle-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/others/recycle-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/others/scales-3-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/others/scales-3-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/system/eye-off-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/system/eye-off-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/system/settings-5-fill.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/system/settings-5-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/system/settings-5-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/system/settings-5-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/user/account-pin-circle-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/user/account-pin-circle-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/user/team-line.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/user/team-line.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/icons/user/user-setting-fill.svg` & `mkdocs_dsfr-0.0.4/dsfr/icons/user/user-setting-fill.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/js/base.js` & `mkdocs_dsfr-0.0.4/dsfr/js/base.js`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/js/bootstrap.min.js` & `mkdocs_dsfr-0.0.4/dsfr/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/js/jquery-1.10.2.min.js` & `mkdocs_dsfr-0.0.4/dsfr/js/jquery-1.10.2.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/lateral.html` & `mkdocs_dsfr-0.0.4/dsfr/lateral.html`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/nav.html` & `mkdocs_dsfr-0.0.4/dsfr/nav.html`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/prev-next-nav.html` & `mkdocs_dsfr-0.0.4/dsfr/prev-next-nav.html`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/search.html` & `mkdocs_dsfr-0.0.4/dsfr/search.html`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-buildings/icons-buildings.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-buildings/icons-buildings.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-buildings/icons-buildings.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-buildings/icons-buildings.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-buildings/icons-buildings.legacy.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-buildings/icons-buildings.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-buildings/icons-buildings.legacy.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-buildings/icons-buildings.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-buildings/icons-buildings.legacy.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-buildings/icons-buildings.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-buildings/icons-buildings.legacy.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-buildings/icons-buildings.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-buildings/icons-buildings.main.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-buildings/icons-buildings.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-buildings/icons-buildings.main.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-buildings/icons-buildings.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-buildings/icons-buildings.main.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-buildings/icons-buildings.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-buildings/icons-buildings.main.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-buildings/icons-buildings.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-buildings/icons-buildings.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-buildings/icons-buildings.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-buildings/icons-buildings.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-buildings/icons-buildings.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-business/icons-business.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-business/icons-business.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-business/icons-business.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-business/icons-business.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-business/icons-business.legacy.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-business/icons-business.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-business/icons-business.legacy.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-business/icons-business.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-business/icons-business.legacy.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-business/icons-business.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-business/icons-business.legacy.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-business/icons-business.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-business/icons-business.main.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-business/icons-business.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-business/icons-business.main.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-business/icons-business.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-business/icons-business.main.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-business/icons-business.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-business/icons-business.main.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-business/icons-business.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-business/icons-business.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-business/icons-business.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-business/icons-business.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-business/icons-business.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-communication/icons-communication.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-communication/icons-communication.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-communication/icons-communication.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-communication/icons-communication.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-communication/icons-communication.legacy.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-communication/icons-communication.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-communication/icons-communication.legacy.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-communication/icons-communication.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-communication/icons-communication.legacy.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-communication/icons-communication.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-communication/icons-communication.legacy.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-communication/icons-communication.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-communication/icons-communication.main.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-communication/icons-communication.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-communication/icons-communication.main.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-communication/icons-communication.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-communication/icons-communication.main.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-communication/icons-communication.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-communication/icons-communication.main.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-communication/icons-communication.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-communication/icons-communication.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-communication/icons-communication.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-communication/icons-communication.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-communication/icons-communication.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-design/icons-design.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-design/icons-design.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-design/icons-design.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-design/icons-design.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-design/icons-design.legacy.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-design/icons-design.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-design/icons-design.legacy.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-design/icons-design.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-design/icons-design.legacy.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-design/icons-design.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-design/icons-design.legacy.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-design/icons-design.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-design/icons-design.main.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-design/icons-design.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-design/icons-design.main.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-design/icons-design.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-design/icons-design.main.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-design/icons-design.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-design/icons-design.main.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-design/icons-design.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-design/icons-design.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-design/icons-design.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-design/icons-design.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-design/icons-design.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-development/icons-development.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-development/icons-development.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-development/icons-development.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-development/icons-development.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-development/icons-development.legacy.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-development/icons-development.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-development/icons-development.legacy.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-development/icons-development.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-development/icons-development.legacy.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-development/icons-development.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-development/icons-development.legacy.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-development/icons-development.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-development/icons-development.main.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-development/icons-development.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-development/icons-development.main.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-development/icons-development.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-development/icons-development.main.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-development/icons-development.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-development/icons-development.main.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-development/icons-development.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-development/icons-development.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-development/icons-development.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-development/icons-development.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-development/icons-development.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-device/icons-device.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-device/icons-device.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-device/icons-device.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-device/icons-device.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-device/icons-device.legacy.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-device/icons-device.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-device/icons-device.legacy.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-device/icons-device.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-device/icons-device.legacy.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-device/icons-device.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-device/icons-device.legacy.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-device/icons-device.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-device/icons-device.main.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-device/icons-device.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-device/icons-device.main.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-device/icons-device.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-device/icons-device.main.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-device/icons-device.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-device/icons-device.main.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-device/icons-device.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-device/icons-device.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-device/icons-device.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-device/icons-device.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-device/icons-device.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-document/icons-document.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-document/icons-document.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-document/icons-document.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-document/icons-document.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-document/icons-document.legacy.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-document/icons-document.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-document/icons-document.legacy.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-document/icons-document.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-document/icons-document.legacy.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-document/icons-document.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-document/icons-document.legacy.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-document/icons-document.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-document/icons-document.main.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-document/icons-document.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-document/icons-document.main.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-document/icons-document.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-document/icons-document.main.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-document/icons-document.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-document/icons-document.main.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-document/icons-document.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-document/icons-document.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-document/icons-document.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-document/icons-document.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-document/icons-document.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-editor/icons-editor.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-editor/icons-editor.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-editor/icons-editor.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-editor/icons-editor.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-editor/icons-editor.legacy.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-editor/icons-editor.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-editor/icons-editor.legacy.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-editor/icons-editor.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-editor/icons-editor.legacy.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-editor/icons-editor.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-editor/icons-editor.legacy.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-editor/icons-editor.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-editor/icons-editor.main.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-editor/icons-editor.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-editor/icons-editor.main.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-editor/icons-editor.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-editor/icons-editor.main.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-editor/icons-editor.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-editor/icons-editor.main.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-editor/icons-editor.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-editor/icons-editor.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-editor/icons-editor.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-editor/icons-editor.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-editor/icons-editor.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-finance/icons-finance.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-finance/icons-finance.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-finance/icons-finance.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-finance/icons-finance.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-finance/icons-finance.legacy.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-finance/icons-finance.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-finance/icons-finance.legacy.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-finance/icons-finance.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-finance/icons-finance.legacy.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-finance/icons-finance.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-finance/icons-finance.legacy.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-finance/icons-finance.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-finance/icons-finance.main.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-finance/icons-finance.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-finance/icons-finance.main.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-finance/icons-finance.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-finance/icons-finance.main.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-finance/icons-finance.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-finance/icons-finance.main.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-finance/icons-finance.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-finance/icons-finance.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-finance/icons-finance.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-finance/icons-finance.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-finance/icons-finance.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-health/icons-health.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-health/icons-health.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-health/icons-health.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-health/icons-health.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-health/icons-health.legacy.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-health/icons-health.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-health/icons-health.legacy.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-health/icons-health.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-health/icons-health.legacy.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-health/icons-health.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-health/icons-health.legacy.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-health/icons-health.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-health/icons-health.main.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-health/icons-health.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-health/icons-health.main.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-health/icons-health.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-health/icons-health.main.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-health/icons-health.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-health/icons-health.main.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-health/icons-health.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-health/icons-health.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-health/icons-health.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-health/icons-health.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-health/icons-health.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-logo/icons-logo.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-logo/icons-logo.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-logo/icons-logo.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-logo/icons-logo.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-logo/icons-logo.legacy.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-logo/icons-logo.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-logo/icons-logo.legacy.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-logo/icons-logo.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-logo/icons-logo.legacy.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-logo/icons-logo.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-logo/icons-logo.legacy.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-logo/icons-logo.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-logo/icons-logo.main.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-logo/icons-logo.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-logo/icons-logo.main.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-logo/icons-logo.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-logo/icons-logo.main.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-logo/icons-logo.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-logo/icons-logo.main.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-logo/icons-logo.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-logo/icons-logo.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-logo/icons-logo.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-logo/icons-logo.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-logo/icons-logo.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-map/icons-map.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-map/icons-map.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-map/icons-map.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-map/icons-map.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-map/icons-map.legacy.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-map/icons-map.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-map/icons-map.legacy.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-map/icons-map.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-map/icons-map.legacy.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-map/icons-map.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-map/icons-map.legacy.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-map/icons-map.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-map/icons-map.main.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-map/icons-map.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-map/icons-map.main.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-map/icons-map.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-map/icons-map.main.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-map/icons-map.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-map/icons-map.main.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-map/icons-map.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-map/icons-map.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-map/icons-map.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-map/icons-map.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-map/icons-map.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-media/icons-media.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-media/icons-media.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-media/icons-media.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-media/icons-media.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-media/icons-media.legacy.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-media/icons-media.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-media/icons-media.legacy.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-media/icons-media.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-media/icons-media.legacy.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-media/icons-media.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-media/icons-media.legacy.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-media/icons-media.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-media/icons-media.main.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-media/icons-media.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-media/icons-media.main.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-media/icons-media.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-media/icons-media.main.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-media/icons-media.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-media/icons-media.main.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-media/icons-media.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-media/icons-media.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-media/icons-media.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-media/icons-media.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-media/icons-media.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-others/icons-others.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-others/icons-others.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-others/icons-others.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-others/icons-others.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-others/icons-others.legacy.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-others/icons-others.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-others/icons-others.legacy.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-others/icons-others.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-others/icons-others.legacy.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-others/icons-others.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-others/icons-others.legacy.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-others/icons-others.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-others/icons-others.main.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-others/icons-others.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-others/icons-others.main.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-others/icons-others.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-others/icons-others.main.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-others/icons-others.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-others/icons-others.main.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-others/icons-others.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-others/icons-others.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-others/icons-others.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-others/icons-others.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-others/icons-others.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-system/icons-system.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-system/icons-system.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-system/icons-system.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-system/icons-system.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-system/icons-system.legacy.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-system/icons-system.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-system/icons-system.legacy.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-system/icons-system.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-system/icons-system.legacy.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-system/icons-system.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-system/icons-system.legacy.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-system/icons-system.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-system/icons-system.main.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-system/icons-system.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-system/icons-system.main.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-system/icons-system.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-system/icons-system.main.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-system/icons-system.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-system/icons-system.main.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-system/icons-system.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-system/icons-system.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-system/icons-system.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-system/icons-system.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-system/icons-system.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-user/icons-user.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-user/icons-user.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-user/icons-user.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-user/icons-user.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-user/icons-user.legacy.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-user/icons-user.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-user/icons-user.legacy.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-user/icons-user.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-user/icons-user.legacy.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-user/icons-user.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-user/icons-user.legacy.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-user/icons-user.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-user/icons-user.main.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-user/icons-user.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-user/icons-user.main.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-user/icons-user.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-user/icons-user.main.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-user/icons-user.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-user/icons-user.main.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-user/icons-user.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-user/icons-user.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-user/icons-user.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-user/icons-user.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-user/icons-user.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-weather/icons-weather.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-weather/icons-weather.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-weather/icons-weather.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-weather/icons-weather.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-weather/icons-weather.legacy.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-weather/icons-weather.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-weather/icons-weather.legacy.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-weather/icons-weather.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-weather/icons-weather.legacy.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-weather/icons-weather.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-weather/icons-weather.legacy.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-weather/icons-weather.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-weather/icons-weather.main.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-weather/icons-weather.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-weather/icons-weather.main.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-weather/icons-weather.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-weather/icons-weather.main.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-weather/icons-weather.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-weather/icons-weather.main.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-weather/icons-weather.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-weather/icons-weather.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-weather/icons-weather.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons-weather/icons-weather.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons-weather/icons-weather.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons.legacy.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons.legacy.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons.legacy.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons.legacy.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons.legacy.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons.legacy.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons.legacy.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons.legacy.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons.main.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons.main.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons.main.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons.main.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons.main.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons.main.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons.main.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons.main.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons.min.css` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-dsfr-0.0.3/dsfr/utility/icons/icons.min.css.map` & `mkdocs_dsfr-0.0.4/dsfr/utility/icons/icons.min.css.map`

 * *Files identical despite different names*

