# Comparing `tmp/streamlit-reveal-slides-0.1.5.tar.gz` & `tmp/streamlit-reveal-slides-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-reveal-slides-0.1.5.tar", last modified: Fri Jun  2 08:29:19 2023, max compression
+gzip compressed data, was "streamlit-reveal-slides-0.1.6.tar", last modified: Fri Jun  2 08:37:53 2023, max compression
```

## Comparing `streamlit-reveal-slides-0.1.5.tar` & `streamlit-reveal-slides-0.1.6.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:29:19.412422 streamlit-reveal-slides-0.1.5/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1063 2023-05-23 07:31:54.000000 streamlit-reveal-slides-0.1.5/LICENSE
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       49 2023-05-23 07:31:54.000000 streamlit-reveal-slides-0.1.5/MANIFEST.in
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      393 2023-06-02 08:29:19.402422 streamlit-reveal-slides-0.1.5/PKG-INFO
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2218 2023-05-23 23:10:19.000000 streamlit-reveal-slides-0.1.5/README.md
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:29:19.252422 streamlit-reveal-slides-0.1.5/reveal_slides/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    15014 2023-06-02 08:23:32.000000 streamlit-reveal-slides-0.1.5/reveal_slides/__init__.py
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:29:19.252422 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:29:19.262422 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6479 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/asset-manifest.json
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   197459 2023-06-02 08:25:55.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/bootstrap.min.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4356 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/index.html
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:29:19.252422 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:29:19.272422 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7201 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/10.1f3244e3.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11924 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/10.1f3244e3.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7253 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/11.cb699f02.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11744 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/11.cb699f02.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6477 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/12.158b51eb.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20354 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/12.158b51eb.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7194 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/13.74908590.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11911 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/13.74908590.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7194 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/14.e64fc659.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11713 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/14.e64fc659.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7184 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/15.3adba626.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11931 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/15.3adba626.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6719 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/16.b573d318.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11404 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/16.b573d318.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      405 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/17.10a8300f.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      580 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/17.10a8300f.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1666 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/18.4eb3e38a.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1954 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/18.4eb3e38a.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5699 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/19.74b97645.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    10009 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/19.74b97645.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    47158 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/2.5029ddca.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    60673 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/2.5029ddca.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6543 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/3.11f8848d.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20560 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/3.11f8848d.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6560 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/4.2fe0cb1b.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20701 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/4.2fe0cb1b.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6057 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/5.5a2b8ee3.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    19287 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/5.5a2b8ee3.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5695 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/6.1b9cee33.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    18239 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/6.1b9cee33.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5701 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/7.4e275de2.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    18662 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/7.4e275de2.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5826 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/8.eb5abf62.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    19077 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/8.eb5abf62.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5825 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/9.1253a161.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    18776 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/9.1253a161.chunk.css.map
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:29:19.372422 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/10.18fc5a6d.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/10.18fc5a6d.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/11.e2b8452b.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/11.e2b8452b.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/12.6c6d4448.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/12.6c6d4448.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/13.c5f703d1.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/13.c5f703d1.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/14.39efed4e.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/14.39efed4e.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/15.7665d197.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/15.7665d197.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/16.4a5a2671.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/16.4a5a2671.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/17.e0e3c073.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/17.e0e3c073.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/18.b265fc2b.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/18.b265fc2b.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/19.5ba3da56.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/19.5ba3da56.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)  1847219 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/2.5c1e1a04.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2767 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/2.5c1e1a04.chunk.js.LICENSE.txt
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)  3896922 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/2.5c1e1a04.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/3.d30f1cfd.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/3.d30f1cfd.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/4.ec7a53ea.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/4.ec7a53ea.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/5.e42b3133.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/5.e42b3133.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/6.e9192981.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/6.e9192981.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/7.be794506.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/7.be794506.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/8.15dd3b20.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/8.15dd3b20.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/9.119f08fa.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/9.119f08fa.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4645 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/main.3837bbb6.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20363 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/main.3837bbb6.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3774 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/runtime-main.eaac28ce.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    17321 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/runtime-main.eaac28ce.js.map
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:29:19.402422 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/media/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    30764 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/media/league-gothic.080eee2a.woff
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    25696 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/media/league-gothic.12baac5d.eot
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    64256 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/media/league-gothic.6ae91382.ttf
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   238084 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/media/source-sans-pro-italic.10a5cb40.ttf
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    75720 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/media/source-sans-pro-italic.97e79d3e.eot
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    98556 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/media/source-sans-pro-italic.983d97ca.woff
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    88070 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/media/source-sans-pro-regular.36443d24.eot
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   288008 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/media/source-sans-pro-regular.45c54810.ttf
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   114324 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/media/source-sans-pro-regular.d1653550.woff
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   284640 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.6ebea875.ttf
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    89897 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.83db537e.eot
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   115648 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.f11ba60a.woff
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   240944 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.522a9ee9.ttf
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    98816 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.a43f56ac.woff
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    75706 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.fb03c660.eot
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       38 2023-06-02 08:29:19.412422 streamlit-reveal-slides-0.1.5/setup.cfg
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      764 2023-06-02 08:25:48.000000 streamlit-reveal-slides-0.1.5/setup.py
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:29:19.402422 streamlit-reveal-slides-0.1.5/streamlit_reveal_slides.egg-info/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      393 2023-06-02 08:29:18.000000 streamlit-reveal-slides-0.1.5/streamlit_reveal_slides.egg-info/PKG-INFO
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6450 2023-06-02 08:29:19.000000 streamlit-reveal-slides-0.1.5/streamlit_reveal_slides.egg-info/SOURCES.txt
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)        1 2023-06-02 08:29:18.000000 streamlit-reveal-slides-0.1.5/streamlit_reveal_slides.egg-info/dependency_links.txt
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       16 2023-06-02 08:29:18.000000 streamlit-reveal-slides-0.1.5/streamlit_reveal_slides.egg-info/requires.txt
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       14 2023-06-02 08:29:18.000000 streamlit-reveal-slides-0.1.5/streamlit_reveal_slides.egg-info/top_level.txt
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:37:53.932431 streamlit-reveal-slides-0.1.6/
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1063 2023-05-23 07:31:54.000000 streamlit-reveal-slides-0.1.6/LICENSE
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       49 2023-05-23 07:31:54.000000 streamlit-reveal-slides-0.1.6/MANIFEST.in
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      393 2023-06-02 08:37:53.932431 streamlit-reveal-slides-0.1.6/PKG-INFO
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2218 2023-05-23 23:10:19.000000 streamlit-reveal-slides-0.1.6/README.md
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:37:53.722431 streamlit-reveal-slides-0.1.6/reveal_slides/
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    15013 2023-06-02 08:36:26.000000 streamlit-reveal-slides-0.1.6/reveal_slides/__init__.py
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:37:53.722431 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:37:53.732431 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6479 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/asset-manifest.json
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   197459 2023-06-02 08:25:55.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/bootstrap.min.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4356 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/index.html
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:37:53.722431 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:37:53.762431 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7201 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/10.1f3244e3.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11924 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/10.1f3244e3.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7253 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/11.cb699f02.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11744 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/11.cb699f02.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6477 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/12.158b51eb.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20354 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/12.158b51eb.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7194 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/13.74908590.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11911 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/13.74908590.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7194 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/14.e64fc659.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11713 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/14.e64fc659.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7184 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/15.3adba626.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11931 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/15.3adba626.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6719 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/16.b573d318.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11404 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/16.b573d318.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      405 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/17.10a8300f.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      580 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/17.10a8300f.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1666 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/18.4eb3e38a.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1954 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/18.4eb3e38a.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5699 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/19.74b97645.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    10009 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/19.74b97645.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    47158 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/2.5029ddca.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    60673 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/2.5029ddca.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6543 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/3.11f8848d.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20560 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/3.11f8848d.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6560 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/4.2fe0cb1b.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20701 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/4.2fe0cb1b.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6057 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/5.5a2b8ee3.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    19287 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/5.5a2b8ee3.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5695 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/6.1b9cee33.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    18239 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/6.1b9cee33.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5701 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/7.4e275de2.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    18662 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/7.4e275de2.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5826 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/8.eb5abf62.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    19077 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/8.eb5abf62.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5825 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/9.1253a161.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    18776 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/9.1253a161.chunk.css.map
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:37:53.882431 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/10.18fc5a6d.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/10.18fc5a6d.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/11.e2b8452b.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/11.e2b8452b.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/12.6c6d4448.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/12.6c6d4448.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/13.c5f703d1.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/13.c5f703d1.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/14.39efed4e.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/14.39efed4e.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/15.7665d197.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/15.7665d197.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/16.4a5a2671.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/16.4a5a2671.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/17.e0e3c073.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/17.e0e3c073.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/18.b265fc2b.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/18.b265fc2b.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/19.5ba3da56.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/19.5ba3da56.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)  1847219 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/2.5c1e1a04.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2767 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/2.5c1e1a04.chunk.js.LICENSE.txt
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)  3896922 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/2.5c1e1a04.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/3.d30f1cfd.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/3.d30f1cfd.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/4.ec7a53ea.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/4.ec7a53ea.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/5.e42b3133.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/5.e42b3133.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/6.e9192981.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/6.e9192981.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/7.be794506.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/7.be794506.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/8.15dd3b20.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/8.15dd3b20.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/9.119f08fa.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/9.119f08fa.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4645 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/main.3837bbb6.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20363 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/main.3837bbb6.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3774 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/runtime-main.eaac28ce.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    17321 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/runtime-main.eaac28ce.js.map
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:37:53.922431 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    30764 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/league-gothic.080eee2a.woff
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    25696 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/league-gothic.12baac5d.eot
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    64256 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/league-gothic.6ae91382.ttf
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   238084 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-italic.10a5cb40.ttf
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    75720 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-italic.97e79d3e.eot
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    98556 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-italic.983d97ca.woff
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    88070 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-regular.36443d24.eot
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   288008 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-regular.45c54810.ttf
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   114324 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-regular.d1653550.woff
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   284640 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.6ebea875.ttf
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    89897 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.83db537e.eot
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   115648 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.f11ba60a.woff
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   240944 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.522a9ee9.ttf
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    98816 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.a43f56ac.woff
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    75706 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.fb03c660.eot
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       38 2023-06-02 08:37:53.932431 streamlit-reveal-slides-0.1.6/setup.cfg
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      764 2023-06-02 08:37:04.000000 streamlit-reveal-slides-0.1.6/setup.py
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:37:53.932431 streamlit-reveal-slides-0.1.6/streamlit_reveal_slides.egg-info/
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      393 2023-06-02 08:37:53.000000 streamlit-reveal-slides-0.1.6/streamlit_reveal_slides.egg-info/PKG-INFO
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6450 2023-06-02 08:37:53.000000 streamlit-reveal-slides-0.1.6/streamlit_reveal_slides.egg-info/SOURCES.txt
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)        1 2023-06-02 08:37:53.000000 streamlit-reveal-slides-0.1.6/streamlit_reveal_slides.egg-info/dependency_links.txt
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       16 2023-06-02 08:37:53.000000 streamlit-reveal-slides-0.1.6/streamlit_reveal_slides.egg-info/requires.txt
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       14 2023-06-02 08:37:53.000000 streamlit-reveal-slides-0.1.6/streamlit_reveal_slides.egg-info/top_level.txt
```

### Comparing `streamlit-reveal-slides-0.1.5/LICENSE` & `streamlit-reveal-slides-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/README.md` & `streamlit-reveal-slides-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/__init__.py` & `streamlit-reveal-slides-0.1.6/reveal_slides/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import streamlit.components.v1 as components
 
 # Create a _RELEASE constant. We'll set this to False while we're developing
 # the component, and True when we're ready to package and distribute it.
 # (This is, of course, optional - there are innumerable ways to manage your
 # release process.)
-_RELEASE = False
+_RELEASE = True
 
 # Declare a Streamlit component. `declare_component` returns a function
 # that is used to create instances of the component. We're naming this
 # function "_component_func", with an underscore prefix, because we don't want
 # to expose it directly to users. Instead, we will create a custom wrapper
 # function, below, that will serve as our component's public API.
```

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/asset-manifest.json` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/bootstrap.min.css` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/index.html` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/10.1f3244e3.chunk.css` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/10.1f3244e3.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/10.1f3244e3.chunk.css.map` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/10.1f3244e3.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/11.cb699f02.chunk.css` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/11.cb699f02.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/11.cb699f02.chunk.css.map` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/11.cb699f02.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/12.158b51eb.chunk.css` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/12.158b51eb.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/12.158b51eb.chunk.css.map` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/12.158b51eb.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/13.74908590.chunk.css` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/13.74908590.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/13.74908590.chunk.css.map` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/13.74908590.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/14.e64fc659.chunk.css` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/14.e64fc659.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/14.e64fc659.chunk.css.map` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/14.e64fc659.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/15.3adba626.chunk.css` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/15.3adba626.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/15.3adba626.chunk.css.map` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/15.3adba626.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/16.b573d318.chunk.css` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/16.b573d318.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/16.b573d318.chunk.css.map` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/16.b573d318.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/17.10a8300f.chunk.css.map` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/17.10a8300f.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/18.4eb3e38a.chunk.css` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/18.4eb3e38a.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/18.4eb3e38a.chunk.css.map` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/18.4eb3e38a.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/19.74b97645.chunk.css` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/19.74b97645.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/19.74b97645.chunk.css.map` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/19.74b97645.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/2.5029ddca.chunk.css` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/2.5029ddca.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/2.5029ddca.chunk.css.map` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/2.5029ddca.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/3.11f8848d.chunk.css` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/3.11f8848d.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/3.11f8848d.chunk.css.map` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/3.11f8848d.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/4.2fe0cb1b.chunk.css` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/4.2fe0cb1b.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/4.2fe0cb1b.chunk.css.map` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/4.2fe0cb1b.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/5.5a2b8ee3.chunk.css` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/5.5a2b8ee3.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/5.5a2b8ee3.chunk.css.map` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/5.5a2b8ee3.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/6.1b9cee33.chunk.css` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/6.1b9cee33.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/6.1b9cee33.chunk.css.map` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/6.1b9cee33.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/7.4e275de2.chunk.css` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/7.4e275de2.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/7.4e275de2.chunk.css.map` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/7.4e275de2.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/8.eb5abf62.chunk.css` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/8.eb5abf62.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/8.eb5abf62.chunk.css.map` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/8.eb5abf62.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/9.1253a161.chunk.css` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/9.1253a161.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/css/9.1253a161.chunk.css.map` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/9.1253a161.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/2.5c1e1a04.chunk.js` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/2.5c1e1a04.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/2.5c1e1a04.chunk.js.LICENSE.txt` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/2.5c1e1a04.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/2.5c1e1a04.chunk.js.map` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/2.5c1e1a04.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/main.3837bbb6.chunk.js` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/main.3837bbb6.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/main.3837bbb6.chunk.js.map` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/main.3837bbb6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/runtime-main.eaac28ce.js` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/runtime-main.eaac28ce.js`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/js/runtime-main.eaac28ce.js.map` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/runtime-main.eaac28ce.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/media/league-gothic.080eee2a.woff` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/league-gothic.080eee2a.woff`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/media/league-gothic.12baac5d.eot` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/league-gothic.12baac5d.eot`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/media/league-gothic.6ae91382.ttf` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/league-gothic.6ae91382.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/media/source-sans-pro-italic.10a5cb40.ttf` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-italic.10a5cb40.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/media/source-sans-pro-italic.97e79d3e.eot` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-italic.97e79d3e.eot`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/media/source-sans-pro-italic.983d97ca.woff` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-italic.983d97ca.woff`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/media/source-sans-pro-regular.36443d24.eot` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-regular.36443d24.eot`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/media/source-sans-pro-regular.45c54810.ttf` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-regular.45c54810.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/media/source-sans-pro-regular.d1653550.woff` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-regular.d1653550.woff`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.6ebea875.ttf` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.6ebea875.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.83db537e.eot` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.83db537e.eot`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.f11ba60a.woff` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.f11ba60a.woff`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.522a9ee9.ttf` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.522a9ee9.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.a43f56ac.woff` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.a43f56ac.woff`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.fb03c660.eot` & `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.fb03c660.eot`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.5/setup.py` & `streamlit-reveal-slides-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit-reveal-slides",
-    version="0.1.5",
+    version="0.1.6",
     author="Anas Bouzid",
     author_email="",
     description="reveal.js HTML presentations for streamlit",
     long_description="create and add reveal.js HTML presentations to your streamlit app",
     long_description_content_type="text/plain",
     url="https://github.com/bouzidanas/streamlit.io/tree/master/streamlit-reveal-slides",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-reveal-slides-0.1.5/streamlit_reveal_slides.egg-info/SOURCES.txt` & `streamlit-reveal-slides-0.1.6/streamlit_reveal_slides.egg-info/SOURCES.txt`

 * *Files identical despite different names*

