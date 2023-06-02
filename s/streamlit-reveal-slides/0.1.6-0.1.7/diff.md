# Comparing `tmp/streamlit-reveal-slides-0.1.6.tar.gz` & `tmp/streamlit-reveal-slides-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-reveal-slides-0.1.6.tar", last modified: Fri Jun  2 08:37:53 2023, max compression
+gzip compressed data, was "streamlit-reveal-slides-0.1.7.tar", last modified: Fri Jun  2 08:46:15 2023, max compression
```

## Comparing `streamlit-reveal-slides-0.1.6.tar` & `streamlit-reveal-slides-0.1.7.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:37:53.932431 streamlit-reveal-slides-0.1.6/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1063 2023-05-23 07:31:54.000000 streamlit-reveal-slides-0.1.6/LICENSE
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       49 2023-05-23 07:31:54.000000 streamlit-reveal-slides-0.1.6/MANIFEST.in
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      393 2023-06-02 08:37:53.932431 streamlit-reveal-slides-0.1.6/PKG-INFO
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2218 2023-05-23 23:10:19.000000 streamlit-reveal-slides-0.1.6/README.md
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:37:53.722431 streamlit-reveal-slides-0.1.6/reveal_slides/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    15013 2023-06-02 08:36:26.000000 streamlit-reveal-slides-0.1.6/reveal_slides/__init__.py
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:37:53.722431 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:37:53.732431 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6479 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/asset-manifest.json
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   197459 2023-06-02 08:25:55.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/bootstrap.min.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4356 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/index.html
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:37:53.722431 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:37:53.762431 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7201 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/10.1f3244e3.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11924 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/10.1f3244e3.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7253 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/11.cb699f02.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11744 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/11.cb699f02.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6477 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/12.158b51eb.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20354 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/12.158b51eb.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7194 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/13.74908590.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11911 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/13.74908590.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7194 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/14.e64fc659.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11713 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/14.e64fc659.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7184 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/15.3adba626.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11931 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/15.3adba626.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6719 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/16.b573d318.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11404 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/16.b573d318.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      405 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/17.10a8300f.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      580 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/17.10a8300f.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1666 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/18.4eb3e38a.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1954 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/18.4eb3e38a.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5699 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/19.74b97645.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    10009 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/19.74b97645.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    47158 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/2.5029ddca.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    60673 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/2.5029ddca.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6543 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/3.11f8848d.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20560 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/3.11f8848d.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6560 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/4.2fe0cb1b.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20701 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/4.2fe0cb1b.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6057 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/5.5a2b8ee3.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    19287 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/5.5a2b8ee3.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5695 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/6.1b9cee33.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    18239 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/6.1b9cee33.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5701 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/7.4e275de2.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    18662 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/7.4e275de2.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5826 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/8.eb5abf62.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    19077 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/8.eb5abf62.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5825 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/9.1253a161.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    18776 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/9.1253a161.chunk.css.map
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:37:53.882431 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/10.18fc5a6d.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/10.18fc5a6d.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/11.e2b8452b.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/11.e2b8452b.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/12.6c6d4448.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/12.6c6d4448.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/13.c5f703d1.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/13.c5f703d1.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/14.39efed4e.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/14.39efed4e.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/15.7665d197.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/15.7665d197.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/16.4a5a2671.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/16.4a5a2671.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/17.e0e3c073.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/17.e0e3c073.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/18.b265fc2b.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/18.b265fc2b.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/19.5ba3da56.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/19.5ba3da56.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)  1847219 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/2.5c1e1a04.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2767 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/2.5c1e1a04.chunk.js.LICENSE.txt
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)  3896922 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/2.5c1e1a04.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/3.d30f1cfd.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/3.d30f1cfd.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/4.ec7a53ea.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/4.ec7a53ea.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/5.e42b3133.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/5.e42b3133.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/6.e9192981.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/6.e9192981.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/7.be794506.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/7.be794506.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/8.15dd3b20.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/8.15dd3b20.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/9.119f08fa.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/9.119f08fa.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4645 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/main.3837bbb6.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20363 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/main.3837bbb6.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3774 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/runtime-main.eaac28ce.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    17321 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/runtime-main.eaac28ce.js.map
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:37:53.922431 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    30764 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/league-gothic.080eee2a.woff
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    25696 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/league-gothic.12baac5d.eot
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    64256 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/league-gothic.6ae91382.ttf
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   238084 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-italic.10a5cb40.ttf
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    75720 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-italic.97e79d3e.eot
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    98556 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-italic.983d97ca.woff
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    88070 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-regular.36443d24.eot
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   288008 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-regular.45c54810.ttf
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   114324 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-regular.d1653550.woff
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   284640 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.6ebea875.ttf
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    89897 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.83db537e.eot
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   115648 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.f11ba60a.woff
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   240944 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.522a9ee9.ttf
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    98816 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.a43f56ac.woff
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    75706 2023-06-02 08:26:28.000000 streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.fb03c660.eot
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       38 2023-06-02 08:37:53.932431 streamlit-reveal-slides-0.1.6/setup.cfg
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      764 2023-06-02 08:37:04.000000 streamlit-reveal-slides-0.1.6/setup.py
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:37:53.932431 streamlit-reveal-slides-0.1.6/streamlit_reveal_slides.egg-info/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      393 2023-06-02 08:37:53.000000 streamlit-reveal-slides-0.1.6/streamlit_reveal_slides.egg-info/PKG-INFO
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6450 2023-06-02 08:37:53.000000 streamlit-reveal-slides-0.1.6/streamlit_reveal_slides.egg-info/SOURCES.txt
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)        1 2023-06-02 08:37:53.000000 streamlit-reveal-slides-0.1.6/streamlit_reveal_slides.egg-info/dependency_links.txt
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       16 2023-06-02 08:37:53.000000 streamlit-reveal-slides-0.1.6/streamlit_reveal_slides.egg-info/requires.txt
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       14 2023-06-02 08:37:53.000000 streamlit-reveal-slides-0.1.6/streamlit_reveal_slides.egg-info/top_level.txt
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:46:15.224335 streamlit-reveal-slides-0.1.7/
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1063 2023-05-23 07:31:54.000000 streamlit-reveal-slides-0.1.7/LICENSE
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       49 2023-05-23 07:31:54.000000 streamlit-reveal-slides-0.1.7/MANIFEST.in
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      393 2023-06-02 08:46:15.224335 streamlit-reveal-slides-0.1.7/PKG-INFO
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2218 2023-05-23 23:10:19.000000 streamlit-reveal-slides-0.1.7/README.md
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:46:15.184335 streamlit-reveal-slides-0.1.7/reveal_slides/
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    15013 2023-06-02 08:36:26.000000 streamlit-reveal-slides-0.1.7/reveal_slides/__init__.py
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:46:15.184335 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:46:15.184335 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6479 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/asset-manifest.json
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   197459 2023-06-02 08:45:23.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/bootstrap.min.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4356 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/index.html
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:46:15.184335 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:46:15.194335 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7201 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/10.1f3244e3.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11924 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/10.1f3244e3.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7253 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/11.cb699f02.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11744 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/11.cb699f02.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6477 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/12.158b51eb.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20354 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/12.158b51eb.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7194 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/13.74908590.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11911 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/13.74908590.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7194 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/14.e64fc659.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11713 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/14.e64fc659.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7184 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/15.3adba626.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11931 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/15.3adba626.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6719 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/16.b573d318.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11404 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/16.b573d318.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      405 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/17.10a8300f.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      580 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/17.10a8300f.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1666 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/18.4eb3e38a.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1954 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/18.4eb3e38a.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5699 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/19.74b97645.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    10009 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/19.74b97645.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    47158 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/2.5029ddca.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    60673 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/2.5029ddca.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6543 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/3.11f8848d.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20560 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/3.11f8848d.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6560 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/4.2fe0cb1b.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20701 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/4.2fe0cb1b.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6057 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/5.5a2b8ee3.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    19287 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/5.5a2b8ee3.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5695 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/6.1b9cee33.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    18239 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/6.1b9cee33.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5701 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/7.4e275de2.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    18662 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/7.4e275de2.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5826 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/8.eb5abf62.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    19077 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/8.eb5abf62.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5825 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/9.1253a161.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    18776 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/9.1253a161.chunk.css.map
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:46:15.224335 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/10.18fc5a6d.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/10.18fc5a6d.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/11.e2b8452b.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/11.e2b8452b.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/12.6c6d4448.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/12.6c6d4448.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/13.c5f703d1.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/13.c5f703d1.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/14.39efed4e.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/14.39efed4e.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/15.7665d197.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/15.7665d197.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/16.4a5a2671.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/16.4a5a2671.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/17.e0e3c073.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/17.e0e3c073.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/18.b265fc2b.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/18.b265fc2b.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/19.5ba3da56.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/19.5ba3da56.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)  1847219 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/2.5c1e1a04.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2767 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/2.5c1e1a04.chunk.js.LICENSE.txt
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)  3896922 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/2.5c1e1a04.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/3.d30f1cfd.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/3.d30f1cfd.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/4.ec7a53ea.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/4.ec7a53ea.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/5.e42b3133.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/5.e42b3133.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/6.e9192981.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/6.e9192981.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/7.be794506.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/7.be794506.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/8.15dd3b20.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/8.15dd3b20.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/9.119f08fa.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/9.119f08fa.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4645 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/main.befe19ba.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20365 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/main.befe19ba.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3774 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/runtime-main.eaac28ce.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    17321 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/runtime-main.eaac28ce.js.map
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:46:15.224335 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/media/
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    30764 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/media/league-gothic.080eee2a.woff
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    25696 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/media/league-gothic.12baac5d.eot
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    64256 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/media/league-gothic.6ae91382.ttf
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   238084 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/media/source-sans-pro-italic.10a5cb40.ttf
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    75720 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/media/source-sans-pro-italic.97e79d3e.eot
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    98556 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/media/source-sans-pro-italic.983d97ca.woff
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    88070 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/media/source-sans-pro-regular.36443d24.eot
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   288008 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/media/source-sans-pro-regular.45c54810.ttf
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   114324 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/media/source-sans-pro-regular.d1653550.woff
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   284640 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.6ebea875.ttf
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    89897 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.83db537e.eot
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   115648 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.f11ba60a.woff
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   240944 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.522a9ee9.ttf
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    98816 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.a43f56ac.woff
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    75706 2023-06-02 08:45:40.000000 streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.fb03c660.eot
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       38 2023-06-02 08:46:15.224335 streamlit-reveal-slides-0.1.7/setup.cfg
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      764 2023-06-02 08:40:31.000000 streamlit-reveal-slides-0.1.7/setup.py
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-02 08:46:15.224335 streamlit-reveal-slides-0.1.7/streamlit_reveal_slides.egg-info/
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      393 2023-06-02 08:46:15.000000 streamlit-reveal-slides-0.1.7/streamlit_reveal_slides.egg-info/PKG-INFO
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6450 2023-06-02 08:46:15.000000 streamlit-reveal-slides-0.1.7/streamlit_reveal_slides.egg-info/SOURCES.txt
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)        1 2023-06-02 08:46:15.000000 streamlit-reveal-slides-0.1.7/streamlit_reveal_slides.egg-info/dependency_links.txt
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       16 2023-06-02 08:46:15.000000 streamlit-reveal-slides-0.1.7/streamlit_reveal_slides.egg-info/requires.txt
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       14 2023-06-02 08:46:15.000000 streamlit-reveal-slides-0.1.7/streamlit_reveal_slides.egg-info/top_level.txt
```

### Comparing `streamlit-reveal-slides-0.1.6/LICENSE` & `streamlit-reveal-slides-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/README.md` & `streamlit-reveal-slides-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/__init__.py` & `streamlit-reveal-slides-0.1.7/reveal_slides/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/asset-manifest.json` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/asset-manifest.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8968750000000001%*

 * *Differences: {"'entrypoints'": "{insert: [(3, 'static/js/main.befe19ba.chunk.js')], delete: [3]}",*

 * * "'files'": "{'main.js': './static/js/main.befe19ba.chunk.js', 'main.js.map': "*

 * *            "'./static/js/main.befe19ba.chunk.js.map'}"}*

```diff
@@ -1,18 +1,18 @@
 {
     "entrypoints": [
         "static/js/runtime-main.eaac28ce.js",
         "static/css/2.5029ddca.chunk.css",
         "static/js/2.5c1e1a04.chunk.js",
-        "static/js/main.3837bbb6.chunk.js"
+        "static/js/main.befe19ba.chunk.js"
     ],
     "files": {
         "index.html": "./index.html",
-        "main.js": "./static/js/main.3837bbb6.chunk.js",
-        "main.js.map": "./static/js/main.3837bbb6.chunk.js.map",
+        "main.js": "./static/js/main.befe19ba.chunk.js",
+        "main.js.map": "./static/js/main.befe19ba.chunk.js.map",
         "runtime-main.js": "./static/js/runtime-main.eaac28ce.js",
         "runtime-main.js.map": "./static/js/runtime-main.eaac28ce.js.map",
         "static/css/10.1f3244e3.chunk.css": "./static/css/10.1f3244e3.chunk.css",
         "static/css/10.1f3244e3.chunk.css.map": "./static/css/10.1f3244e3.chunk.css.map",
         "static/css/11.cb699f02.chunk.css": "./static/css/11.cb699f02.chunk.css",
         "static/css/11.cb699f02.chunk.css.map": "./static/css/11.cb699f02.chunk.css.map",
         "static/css/12.158b51eb.chunk.css": "./static/css/12.158b51eb.chunk.css",
```

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/bootstrap.min.css` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/index.html` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/><link href="./static/css/2.5029ddca.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root" class="reveal"></div><script>!function(e){function t(t){for(var n,o,c=t[0],i=t[1],f=t[2],l=0,d=[];l<c.length;l++)o=c[l],Object.prototype.hasOwnProperty.call(a,o)&&a[o]&&d.push(a[o][0]),a[o]=0;for(n in i)Object.prototype.hasOwnProperty.call(i,n)&&(e[n]=i[n]);for(s&&s(t);d.length;)d.shift()();return u.push.apply(u,f||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,o=1;o<r.length;o++){var i=r[o];0!==a[i]&&(n=!1)}n&&(u.splice(t--,1),e=c(c.s=r[0]))}return e}var n={},o={1:0},a={1:0},u=[];function c(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,c),r.l=!0,r.exports}c.e=function(e){var t=[];o[e]?t.push(o[e]):0!==o[e]&&{3:1,4:1,5:1,6:1,7:1,8:1,9:1,10:1,11:1,12:1,13:1,14:1,15:1,16:1,17:1,18:1,19:1}[e]&&t.push(o[e]=new Promise((function(t,r){for(var n="static/css/"+({}[e]||e)+"."+{3:"11f8848d",4:"2fe0cb1b",5:"5a2b8ee3",6:"1b9cee33",7:"4e275de2",8:"eb5abf62",9:"1253a161",10:"1f3244e3",11:"cb699f02",12:"158b51eb",13:"74908590",14:"e64fc659",15:"3adba626",16:"b573d318",17:"10a8300f",18:"4eb3e38a",19:"74b97645"}[e]+".chunk.css",a=c.p+n,u=document.getElementsByTagName("link"),i=0;i<u.length;i++){var f=(s=u[i]).getAttribute("data-href")||s.getAttribute("href");if("stylesheet"===s.rel&&(f===n||f===a))return t()}var l=document.getElementsByTagName("style");for(i=0;i<l.length;i++){var s;if((f=(s=l[i]).getAttribute("data-href"))===n||f===a)return t()}var d=document.createElement("link");d.rel="stylesheet",d.type="text/css",d.onload=t,d.onerror=function(t){var n=t&&t.target&&t.target.src||a,u=new Error("Loading CSS chunk "+e+" failed.\n("+n+")");u.code="CSS_CHUNK_LOAD_FAILED",u.request=n,delete o[e],d.parentNode.removeChild(d),r(u)},d.href=a,document.getElementsByTagName("head")[0].appendChild(d)})).then((function(){o[e]=0})));var r=a[e];if(0!==r)if(r)t.push(r[2]);else{var n=new Promise((function(t,n){r=a[e]=[t,n]}));t.push(r[2]=n);var u,i=document.createElement("script");i.charset="utf-8",i.timeout=120,c.nc&&i.setAttribute("nonce",c.nc),i.src=function(e){return c.p+"static/js/"+({}[e]||e)+"."+{3:"d30f1cfd",4:"ec7a53ea",5:"e42b3133",6:"e9192981",7:"be794506",8:"15dd3b20",9:"119f08fa",10:"18fc5a6d",11:"e2b8452b",12:"6c6d4448",13:"c5f703d1",14:"39efed4e",15:"7665d197",16:"4a5a2671",17:"e0e3c073",18:"b265fc2b",19:"5ba3da56"}[e]+".chunk.js"}(e);var f=new Error;u=function(t){i.onerror=i.onload=null,clearTimeout(l);var r=a[e];if(0!==r){if(r){var n=t&&("load"===t.type?"missing":t.type),o=t&&t.target&&t.target.src;f.message="Loading chunk "+e+" failed.\n("+n+": "+o+")",f.name="ChunkLoadError",f.type=n,f.request=o,r[1](f)}a[e]=void 0}};var l=setTimeout((function(){u({type:"timeout",target:i})}),12e4);i.onerror=i.onload=u,document.head.appendChild(i)}return Promise.all(t)},c.m=e,c.c=n,c.d=function(e,t,r){c.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},c.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},c.t=function(e,t){if(1&t&&(e=c(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(c.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)c.d(r,n,function(t){return e[t]}.bind(null,n));return r},c.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return c.d(t,"a",t),t},c.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},c.p="./",c.oe=function(e){throw console.error(e),e};var i=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],f=i.push.bind(i);i.push=t,i=i.slice();for(var l=0;l<i.length;l++)t(i[l]);var s=f;r()}([])</script><script src="./static/js/2.5c1e1a04.chunk.js"></script><script src="./static/js/main.3837bbb6.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/><link href="./static/css/2.5029ddca.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root" class="reveal"></div><script>!function(e){function t(t){for(var n,o,c=t[0],i=t[1],f=t[2],l=0,d=[];l<c.length;l++)o=c[l],Object.prototype.hasOwnProperty.call(a,o)&&a[o]&&d.push(a[o][0]),a[o]=0;for(n in i)Object.prototype.hasOwnProperty.call(i,n)&&(e[n]=i[n]);for(s&&s(t);d.length;)d.shift()();return u.push.apply(u,f||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,o=1;o<r.length;o++){var i=r[o];0!==a[i]&&(n=!1)}n&&(u.splice(t--,1),e=c(c.s=r[0]))}return e}var n={},o={1:0},a={1:0},u=[];function c(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,c),r.l=!0,r.exports}c.e=function(e){var t=[];o[e]?t.push(o[e]):0!==o[e]&&{3:1,4:1,5:1,6:1,7:1,8:1,9:1,10:1,11:1,12:1,13:1,14:1,15:1,16:1,17:1,18:1,19:1}[e]&&t.push(o[e]=new Promise((function(t,r){for(var n="static/css/"+({}[e]||e)+"."+{3:"11f8848d",4:"2fe0cb1b",5:"5a2b8ee3",6:"1b9cee33",7:"4e275de2",8:"eb5abf62",9:"1253a161",10:"1f3244e3",11:"cb699f02",12:"158b51eb",13:"74908590",14:"e64fc659",15:"3adba626",16:"b573d318",17:"10a8300f",18:"4eb3e38a",19:"74b97645"}[e]+".chunk.css",a=c.p+n,u=document.getElementsByTagName("link"),i=0;i<u.length;i++){var f=(s=u[i]).getAttribute("data-href")||s.getAttribute("href");if("stylesheet"===s.rel&&(f===n||f===a))return t()}var l=document.getElementsByTagName("style");for(i=0;i<l.length;i++){var s;if((f=(s=l[i]).getAttribute("data-href"))===n||f===a)return t()}var d=document.createElement("link");d.rel="stylesheet",d.type="text/css",d.onload=t,d.onerror=function(t){var n=t&&t.target&&t.target.src||a,u=new Error("Loading CSS chunk "+e+" failed.\n("+n+")");u.code="CSS_CHUNK_LOAD_FAILED",u.request=n,delete o[e],d.parentNode.removeChild(d),r(u)},d.href=a,document.getElementsByTagName("head")[0].appendChild(d)})).then((function(){o[e]=0})));var r=a[e];if(0!==r)if(r)t.push(r[2]);else{var n=new Promise((function(t,n){r=a[e]=[t,n]}));t.push(r[2]=n);var u,i=document.createElement("script");i.charset="utf-8",i.timeout=120,c.nc&&i.setAttribute("nonce",c.nc),i.src=function(e){return c.p+"static/js/"+({}[e]||e)+"."+{3:"d30f1cfd",4:"ec7a53ea",5:"e42b3133",6:"e9192981",7:"be794506",8:"15dd3b20",9:"119f08fa",10:"18fc5a6d",11:"e2b8452b",12:"6c6d4448",13:"c5f703d1",14:"39efed4e",15:"7665d197",16:"4a5a2671",17:"e0e3c073",18:"b265fc2b",19:"5ba3da56"}[e]+".chunk.js"}(e);var f=new Error;u=function(t){i.onerror=i.onload=null,clearTimeout(l);var r=a[e];if(0!==r){if(r){var n=t&&("load"===t.type?"missing":t.type),o=t&&t.target&&t.target.src;f.message="Loading chunk "+e+" failed.\n("+n+": "+o+")",f.name="ChunkLoadError",f.type=n,f.request=o,r[1](f)}a[e]=void 0}};var l=setTimeout((function(){u({type:"timeout",target:i})}),12e4);i.onerror=i.onload=u,document.head.appendChild(i)}return Promise.all(t)},c.m=e,c.c=n,c.d=function(e,t,r){c.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},c.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},c.t=function(e,t){if(1&t&&(e=c(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(c.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)c.d(r,n,function(t){return e[t]}.bind(null,n));return r},c.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return c.d(t,"a",t),t},c.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},c.p="./",c.oe=function(e){throw console.error(e),e};var i=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],f=i.push.bind(i);i.push=t,i=i.slice();for(var l=0;l<i.length;l++)t(i[l]);var s=f;r()}([])</script><script src="./static/js/2.5c1e1a04.chunk.js"></script><script src="./static/js/main.befe19ba.chunk.js"></script></body></html>
```

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/10.1f3244e3.chunk.css` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/10.1f3244e3.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/10.1f3244e3.chunk.css.map` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/10.1f3244e3.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/11.cb699f02.chunk.css` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/11.cb699f02.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/11.cb699f02.chunk.css.map` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/11.cb699f02.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/12.158b51eb.chunk.css` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/12.158b51eb.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/12.158b51eb.chunk.css.map` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/12.158b51eb.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/13.74908590.chunk.css` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/13.74908590.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/13.74908590.chunk.css.map` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/13.74908590.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/14.e64fc659.chunk.css` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/14.e64fc659.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/14.e64fc659.chunk.css.map` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/14.e64fc659.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/15.3adba626.chunk.css` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/15.3adba626.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/15.3adba626.chunk.css.map` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/15.3adba626.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/16.b573d318.chunk.css` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/16.b573d318.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/16.b573d318.chunk.css.map` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/16.b573d318.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/17.10a8300f.chunk.css.map` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/17.10a8300f.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/18.4eb3e38a.chunk.css` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/18.4eb3e38a.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/18.4eb3e38a.chunk.css.map` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/18.4eb3e38a.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/19.74b97645.chunk.css` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/19.74b97645.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/19.74b97645.chunk.css.map` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/19.74b97645.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/2.5029ddca.chunk.css` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/2.5029ddca.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/2.5029ddca.chunk.css.map` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/2.5029ddca.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/3.11f8848d.chunk.css` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/3.11f8848d.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/3.11f8848d.chunk.css.map` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/3.11f8848d.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/4.2fe0cb1b.chunk.css` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/4.2fe0cb1b.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/4.2fe0cb1b.chunk.css.map` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/4.2fe0cb1b.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/5.5a2b8ee3.chunk.css` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/5.5a2b8ee3.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/5.5a2b8ee3.chunk.css.map` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/5.5a2b8ee3.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/6.1b9cee33.chunk.css` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/6.1b9cee33.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/6.1b9cee33.chunk.css.map` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/6.1b9cee33.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/7.4e275de2.chunk.css` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/7.4e275de2.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/7.4e275de2.chunk.css.map` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/7.4e275de2.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/8.eb5abf62.chunk.css` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/8.eb5abf62.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/8.eb5abf62.chunk.css.map` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/8.eb5abf62.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/9.1253a161.chunk.css` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/9.1253a161.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/css/9.1253a161.chunk.css.map` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/css/9.1253a161.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/2.5c1e1a04.chunk.js` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/2.5c1e1a04.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/2.5c1e1a04.chunk.js.LICENSE.txt` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/2.5c1e1a04.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/2.5c1e1a04.chunk.js.map` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/2.5c1e1a04.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/main.3837bbb6.chunk.js` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/main.befe19ba.chunk.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -56,27 +56,27 @@
                 v = n(36),
                 j = n.n(v),
                 b = n(37),
                 O = n.n(b),
                 y = n(38),
                 x = n.n(y),
                 w = (n(67), n(68), n(9)),
-                S = {
+                S = Object(r.a)(["", ""], (function(e) {
+                    return e.inject
+                })),
+                _ = {
                     markdown: h.a,
                     highlight: d.a,
                     katex: p.a.KaTeX,
                     mathjax2: p.a.MathJax2,
                     mathjax3: p.a.MathJax3,
                     search: j.a,
                     notes: O.a,
                     zoom: x.a
                 },
-                _ = Object(r.a)(["", ""], (function(e) {
-                    return e.inject
-                })),
                 k = {
                     width: 900,
                     height: 860,
                     margin: .05,
                     minScale: .1,
                     maxScale: 3,
                     controlsTutorial: !0,
@@ -89,15 +89,15 @@
                         o = JSON.stringify(t.initial_state),
                         r = function(e) {
                             var n = Object(c.a)(Object(c.a)({}, k), JSON.parse(i));
                             if (t.allow_unsafe_html);
                             else if ("plugins" in n) {
                                 var a = n.plugins;
                                 a.forEach((function(e, t) {
-                                    a[t] = e in S ? S[e] : null
+                                    a[t] = e in _ ? _[e] : null
                                 })), n.plugins = a.filter((function(e) {
                                     return !!e
                                 })), n.plugins.includes(h.a) || n.plugins.push(h.a)
                             } else n.plugins = [h.a];
                             return n
                         };
                     Object(a.useMemo)((function() {
@@ -157,15 +157,15 @@
                     }), []), Object(a.useEffect)((function() {
                         var e = u.a.getPlugins(),
                             n = r(),
                             a = Object.values(e).map((function(e) {
                                 return e.id
                             }));
                         "plugins" in t.config && t.config.plugins.forEach((function(e) {
-                            e && -1 === a.indexOf(e) && u.a.registerPlugin(S[e])
+                            e && -1 === a.indexOf(e) && u.a.registerPlugin(_[e])
                         }));
                         u.a.configure(n)
                     }), [i, t.allow_unsafe_html]), Object(a.useEffect)((function() {
                         var e = JSON.parse(o);
                         u.a.isReady() && 0 !== Object.keys(e).length && u.a.setState(e)
                     }), [o]), Object(a.useEffect)((function() {
                         if (u.a.isReady())
@@ -183,25 +183,25 @@
                             var n;
                             "auto" === t.height || "number" !== typeof t.height ? (l.a.setFrameHeight(null !== (n = e[0].contentBoxSize.blockSize) && void 0 !== n ? n : e[0].contentRect.height), u.a.isReady() && u.a.layout()) : (l.a.setFrameHeight(t.height), u.a.isReady() && u.a.layout())
                         })),
                         g = function(e) {
                             e ? f.observe(e) : f.disconnect()
                         };
                     return t.allow_unsafe_html ? Object(w.jsxs)(w.Fragment, {
-                        children: [Object(w.jsx)(_, {
+                        children: [Object(w.jsx)(S, {
                             inject: t.css
                         }), Object(w.jsx)("div", {
                             ref: g,
                             className: "slides",
                             dangerouslySetInnerHTML: {
                                 __html: t.content
                             }
                         })]
                     }) : Object(w.jsxs)(w.Fragment, {
-                        children: [Object(w.jsx)(_, {
+                        children: [Object(w.jsx)(S, {
                             inject: t.css
                         }), Object(w.jsx)("div", {
                             ref: g,
                             className: "slides",
                             children: Object(w.jsx)("section", Object(c.a)(Object(c.a)({
                                 "data-markdown": ""
                             }, t.markdown_props), {}, {
@@ -218,8 +218,8 @@
             }), document.getElementById("root"))
         }
     },
     [
         [72, 1, 2]
     ]
 ]);
-//# sourceMappingURL=main.3837bbb6.chunk.js.map
+//# sourceMappingURL=main.befe19ba.chunk.js.map
```

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/main.3837bbb6.chunk.js.map` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/main.befe19ba.chunk.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8172268907563025%*

 * *Differences: {"'file'": "'static/js/main.befe19ba.chunk.js'",*

 * * "'mappings'": "'gIAAA,IAAIA,EAAM,CACT,cAAe,CACd,GACA,GAED,uBAAwB,CACvB,GACA,IAED,cAAe,CACd,GACA,IAED,cAAe,CACd,GACA,IAED,gBAAiB,CAChB,GACA,IAED,0CAA2C,CAC1C,GACA,IAED,8CAA+C,CAC9C,GACA,IAED,eAAgB,CACf,GACA,GAED,aAAc,CACb,GACA,GAED,cAAe,CACd,GACA,GAED,cAAe,CACd,GACA,IAED,eAAgB,CACf,GACA,GAED,YAAa,CACZ,GACA,GAED,kBAAmB,CAClB,GACA,GAED,uBAAwB,CACvB,GACA,IAED,cAAe,CACd,GACA,IAED,gDAAiD,CAChD,GACA,KAGF,SAASC,EAAoBC,GAC5B,IAAIC,EAAoBC,EAAEJ,EAAKE,GAC9B,OAAOG,QAAQC […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.3837bbb6.chunk.js",
-    "mappings": "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",
+    "file": "static/js/main.befe19ba.chunk.js",
+    "mappings": "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",
     "names": [
         "map",
         "webpackAsyncContext",
         "req",
         "__webpack_require__",
         "o",
         "Promise",
@@ -16,28 +16,28 @@
         "ids",
         "id",
         "t",
         "keys",
         "Object",
         "module",
         "exports",
+        "GlobalCSS",
+        "createGlobalStyle",
+        "props",
+        "inject",
         "includedPlugins",
         "RevealMarkdown",
         "RevealHighlight",
         "RevealMath",
         "KaTeX",
         "MathJax2",
         "MathJax3",
         "RevealSearch",
         "RevealNotes",
         "RevealZoom",
-        "GlobalCSS",
-        "createGlobalStyle",
-        "props",
-        "inject",
         "defaultConfig",
         "width",
         "height",
         "margin",
         "minScale",
         "maxScale",
         "controlsTutorial",
@@ -139,12 +139,12 @@
     "sources": [
         "../node_modules/reveal.js/dist/theme lazy /^/.//.*/.css$/ groupOptions: {} namespace object",
         "RevealSlides.tsx",
         "index.tsx"
     ],
     "sourcesContent": [
         "var map = {\n\t\"./beige.css\": [\n\t\t73,\n\t\t3\n\t],\n\t\"./black-contrast.css\": [\n\t\t74,\n\t\t10\n\t],\n\t\"./black.css\": [\n\t\t75,\n\t\t11\n\t],\n\t\"./blood.css\": [\n\t\t76,\n\t\t12\n\t],\n\t\"./dracula.css\": [\n\t\t77,\n\t\t16\n\t],\n\t\"./fonts/league-gothic/league-gothic.css\": [\n\t\t78,\n\t\t17\n\t],\n\t\"./fonts/source-sans-pro/source-sans-pro.css\": [\n\t\t79,\n\t\t18\n\t],\n\t\"./league.css\": [\n\t\t80,\n\t\t4\n\t],\n\t\"./moon.css\": [\n\t\t81,\n\t\t5\n\t],\n\t\"./night.css\": [\n\t\t82,\n\t\t6\n\t],\n\t\"./serif.css\": [\n\t\t83,\n\t\t19\n\t],\n\t\"./simple.css\": [\n\t\t84,\n\t\t7\n\t],\n\t\"./sky.css\": [\n\t\t85,\n\t\t8\n\t],\n\t\"./solarized.css\": [\n\t\t86,\n\t\t9\n\t],\n\t\"./white-contrast.css\": [\n\t\t87,\n\t\t13\n\t],\n\t\"./white.css\": [\n\t\t88,\n\t\t14\n\t],\n\t\"./white_contrast_compact_verbatim_headers.css\": [\n\t\t89,\n\t\t15\n\t]\n};\nfunction webpackAsyncContext(req) {\n\tif(!__webpack_require__.o(map, req)) {\n\t\treturn Promise.resolve().then(function() {\n\t\t\tvar e = new Error(\"Cannot find module '\" + req + \"'\");\n\t\t\te.code = 'MODULE_NOT_FOUND';\n\t\t\tthrow e;\n\t\t});\n\t}\n\n\tvar ids = map[req], id = ids[0];\n\treturn __webpack_require__.e(ids[1]).then(function() {\n\t\treturn __webpack_require__.t(id, 7);\n\t});\n}\nwebpackAsyncContext.keys = function webpackAsyncContextKeys() {\n\treturn Object.keys(map);\n};\nwebpackAsyncContext.id = 71;\nmodule.exports = webpackAsyncContext;",
-        "import {\n  Streamlit,\n  ComponentProps,\n  withStreamlitConnection,\n  Theme,\n} from \"streamlit-component-lib\"\nimport { useEffect, useMemo } from \"react\"\nimport { createGlobalStyle } from \"styled-components/macro\"\n\n\nimport Reveal from 'reveal.js';\nimport RevealMarkdown from 'reveal.js/plugin/markdown/markdown';\nimport RevealHighlight from 'reveal.js/plugin/highlight/highlight';\nimport RevealMath from 'reveal.js/plugin/math/math';\nimport RevealSearch from 'reveal.js/plugin/search/search';\nimport RevealNotes from 'reveal.js/plugin/notes/notes';\nimport RevealZoom from 'reveal.js/plugin/zoom/zoom';\n\n\nimport 'reveal.js/dist/reveal.css';\nimport 'reveal.js/plugin/highlight/monokai.css';\n\ninterface RevealSlidesProps extends ComponentProps {\n  args: any\n  width: number\n  disabled: boolean\n  theme?: Theme\n}\n\nconst includedPlugins = {\"markdown\": RevealMarkdown, \"highlight\": RevealHighlight, \"katex\": RevealMath.KaTeX, \"mathjax2\": RevealMath.MathJax2, \"mathjax3\": RevealMath.MathJax3, \"search\": RevealSearch, \"notes\": RevealNotes, \"zoom\": RevealZoom}\n// const simpleCommands = {\"left\": Reveal.left, \"right\": () => {Reveal.right()}, \"up\": Reveal.up, \"down\": Reveal.down, \"prev\": Reveal.prev, \"next\": Reveal.next, \"prevFragment\": Reveal.prevFragment, \"nextFragment\": Reveal.nextFragment, \"togglePause\": Reveal.togglePause, \"toggleAutoSlide\": Reveal.toggleAutoSlide, \"toggleHelp\": Reveal.toggleHelp, \"toggleOverview\": Reveal.toggleOverview, \"shuffle\": Reveal.shuffle}\n// const commandsWithArgs = {slide: Reveal.slide, togglePause: Reveal.togglePause, toggleAutoSlide: Reveal.toggleAutoSlide, toggleHelp: Reveal.toggleHelp, toggleOverview: Reveal.toggleOverview}\n\nconst GlobalCSS = createGlobalStyle<{ inject: string}>`\n  ${props => props.inject}\n`\n\nconst defaultConfig = {\n  // The \"normal\" size of the presentation, aspect ratio will be preserved\n\t// when the presentation is scaled to fit different resolutions\n\twidth: 900,\n\theight: 860,\n\t\n\t// Factor of the display size that should remain empty around the content\n\tmargin: 0.05,\n\n\t// Bounds for smallest/largest possible scale to apply to content\n\tminScale: 0.1,\n\tmaxScale: 3.0,\n\n\t// Help the user learn the controls by providing hints, for example by\n\t// bouncing the down arrow when they first encounter a vertical slide\n\tcontrolsTutorial: true,\n\n\t// Determines where controls appear, \"edges\" or \"bottom-right\"\n\tcontrolsLayout: 'edges',\n}\n\n/**\n * This is a React-based component template. The `render()` function is called\n * automatically when your component should be re-rendered.\n */\nconst RevealSlides = ({ args, disabled }: RevealSlidesProps) => {   \n\n  let configStr = JSON.stringify(args[\"config\"])\n  let initStateStr = JSON.stringify(args[\"initial_state\"])\n  // const commandStr = JSON.stringify(args[\"commands\"])\n\n  const setupConfig = (configString: string) : object => {\n    const config = {...defaultConfig, ...JSON.parse(configStr)}\n    // code to run after render goes here\n    if (args[\"allow_unsafe_html\"]) {\n      // do nothing\n    }\n    else {\n      if ('plugins' in config){\n        var arr = config['plugins'];\n        arr.forEach(function(moduleName: string, index: number) {\n          if (moduleName in includedPlugins){\n            arr[index] = (includedPlugins as any)[moduleName];\n          }\n          else {\n            arr[index] = null;\n          }\n        });\n        config['plugins'] = arr.filter((x:any) => !!x) as any[];\n        if(!config['plugins'].includes(RevealMarkdown)){\n          config['plugins'].push(RevealMarkdown);\n        }\n      }\n      else {\n        config['plugins'] = [RevealMarkdown];\n      }\n    }\n    return config;\n  }\n\n  useMemo(()=>{\n    // code to run on component mount goes here\n\n    // To do: remove or disable previously imported css. When the list of\n    // css imports exceed about 25, the page no longer updates.\n    import('../node_modules/reveal.js/dist/theme/' + args.theme + '.css').then((css) => {\n\n      try{\n        Reveal.layout();\n      }\n      catch (e){\n        console.warn(\"Reveal.layout() call failed.\")\n      }\n    \n    }).catch((err) => {\n      console.warn(\"Failed CSS import: \", err);\n    });\n\n  }, [args.theme]);\n\n  useEffect(() => {\n    const config = setupConfig(configStr)\n    \n    try {\n      Reveal.destroy();\n    }\n    catch (e) {\n    }\n    Reveal.initialize(config).then(() => {\n      // reveal.js is ready\n      \n      // For some yet to be determined reason, the highlight plugin is not initialized.\n      // Setting highlight config option highlightOnLoad to true (before passing to initialize function)\n      // does not work\n      // To Do: make sure the highlight plugin only changes the HTML involving the code once instead of many times.\n      // Possible solution is to make a change to the plugin init function.\n      let highlighter = Reveal.getPlugin('highlight') as any;\n      if (highlighter){\n        highlighter.init(Reveal);\n      }\n      \n      const initState = JSON.parse(initStateStr);\n      if(Object.keys(initState).length !== 0){\n        Reveal.setState(initState);\n      }\n\n      if(!args['display_only']){\n        // Send slide position indecies back to Streamlit on initialization and on slide change\n        const currState = Reveal.getState();\n        Streamlit.setComponentValue(currState);\n        Reveal.on( 'slidechanged', event => {\n\n          const tempState = Reveal.getState();\n          Streamlit.setComponentValue({indexh: (event as any).indexh, indexv: (event as any).indexv, indexf: tempState.indexf, paused: tempState.paused, overview: tempState.overview});\n        });\n        \n        Reveal.on( 'fragmentshown', event => {\n          // event.fragment = the fragment DOM element\n          const tempState = Reveal.getState();\n          Streamlit.setComponentValue(tempState);\n        } );\n        Reveal.on( 'fragmenthidden', event => {\n          // event.fragment = the fragment DOM element\n          const tempState = Reveal.getState();\n          Streamlit.setComponentValue(tempState);\n        } );\n        Reveal.on( 'overviewshown', event => {\n          // event.overview = the overview DOM element\n          const tempState = Reveal.getState();\n          Streamlit.setComponentValue(tempState);\n        } );\n        Reveal.on( 'overviewhidden', event => {\n          // event.overview = the overview DOM element\n          const tempState = Reveal.getState();\n          Streamlit.setComponentValue(tempState);\n        } );\n        Reveal.on( 'paused', event => {\n          // event.fragment = the fragment DOM element\n          const tempState = Reveal.getState();\n          Streamlit.setComponentValue(tempState);\n        } );\n        Reveal.on( 'resumed', event => {\n          // event.fragment = the fragment DOM element\n          const tempState = Reveal.getState();\n          Streamlit.setComponentValue(tempState);\n        } );\n      }\n    });\n\n    return () => {\n      // code to run on component unmount goes here\n      Reveal.destroy();  \n    }\n  }, []);\n\n  // Reconfigure reveal.js if config changes\n  useEffect(() => {\n    const existingPlugins = Reveal.getPlugins();\n    const config = setupConfig(configStr)\n\n    // Add and register plugins that are not already loaded\n    let existingPluginsList : string[] = Object.values(existingPlugins).map((plugin: any) => plugin.id);\n    if('plugins' in args[\"config\"]){\n      const plugins = args[\"config\"][\"plugins\"];\n      (plugins as string[]).forEach((plugin: string) => {\n        if (plugin && existingPluginsList.indexOf(plugin) === -1){\n          Reveal.registerPlugin((includedPlugins as any)[plugin]);\n        }\n      });\n\n      //// Remove plugins that are no longer in the list (does not work yet..some signs there is a bug in Reveal.Plugin)\n      // Object.values(existingPlugins as {[id: string]: Reveal.Plugin;}).forEach((plugin: any) => {\n      //   if (plugin.id && plugin.id !=='markdown' && plugins.indexOf(plugin.id) === -1){\n      //     console.log(\"destroy plugin: \" + plugin.id);\n      //     if( typeof plugin.destroy === 'function' ) {\n      //       plugin.destroy();\n      //     }\n      //   }\n      // });\n    }\n    // Reconfigure reveal.js\n    Reveal.configure(config);\n  }, [configStr, args[\"allow_unsafe_html\"]]);\n\n  useEffect(() => {\n    const initState = JSON.parse(initStateStr);\n    if (Reveal.isReady() && Object.keys(initState).length !== 0){\n      Reveal.setState(initState);\n    }\n  }, [initStateStr]);\n\n  useEffect(() => {\n    if (Reveal.isReady()){\n      if (disabled){\n        Reveal.togglePause(true);\n        let viewport = Reveal.getViewportElement();\n        if (viewport){\n          viewport.style.pointerEvents = \"none\";\n        }\n      }\n      else {  \n        Reveal.togglePause(false);\n        let viewport = Reveal.getViewportElement();\n        if (viewport){\n          viewport.style.pointerEvents = \"auto\";\n        }\n      }\n    }\n  }, [disabled]);\n\n  //To do: add support for commands (i.e. control slides from Streamlit)\n  //-----------------\n  // useEffect(() => {\n  //   const commands = JSON.parse(commandStr)\n  //   if (Array.isArray(commands) && commands.length > 0 && Reveal.isReady()){\n  //     commands.forEach((command: any) => {\n  //       if (typeof command === \"string\" && command in simpleCommands){\n  //         (simpleCommands as any)[command]();\n  //       }\n  //       else if (Array.isArray(command) && command.length > 0 && typeof command[0] === \"string\" && command[0] in commandsWithArgs){\n  //         if (command[0] === \"slide\"){\n  //           if (command.length === 3){\n  //             Reveal.slide(command[1], command[2]);\n  //           }\n  //           else if (command.length === 4){\n  //             Reveal.slide(command[1], command[2], command[3]);\n  //           }\n  //           else {\n  //             console.warn(\"Invalid slide command: slide command array must have 3 or 4 elements.\");\n  //           }\n  //         }\n  //         else {\n  //           (commandsWithArgs as any)[command[0]](command[1]);\n  //         }\n  //       }\n  //       else {\n  //         console.warn(\"Invalid command: command must be a string or an array containing a string as its first element.\");\n  //       }\n  //     });\n  //   }\n  //   else if (!Array.isArray(args[\"commands\"])) {\n  //     console.warn(\"Invalid commands property value: commands must be an array containing at least one command.\");\n  //   }\n  // }, [commandStr]);\n\n  /**\n   * resizeObserver observes changes in elements its given to observe and is used here\n   * to communicate to streamlit the height of the component that has changed\n   * so that streamlit can adjust the iframe containing the component accordingly.\n   */\n  const resizeObserver = new ResizeObserver((entries: any) => {\n    // If we know that the body will always fully contain our component (without cutting it off)\n    // then we can use docuemnt.body height instead\n    if (args[\"height\"] === \"auto\" || typeof args[\"height\"] !== \"number\"){\n      Streamlit.setFrameHeight((entries[0].contentBoxSize.blockSize ?? entries[0].contentRect.height)); \n      if (Reveal.isReady()){\n        Reveal.layout();\n      }\n    }\n    else {\n      Streamlit.setFrameHeight(args[\"height\"]);\n      if (Reveal.isReady()){\n        Reveal.layout();\n      }\n    }\n    \n  })\n\n  const observe = (divElem: any) => {\n    divElem ? resizeObserver.observe(divElem as HTMLDivElement) : resizeObserver.disconnect();\n  }\n\n  if (args[\"allow_unsafe_html\"]) {\n    return (\n      <>\n        <GlobalCSS inject={args.css}/>\n        <div ref={observe} className=\"slides\" dangerouslySetInnerHTML={{__html: args[\"content\"]}}>\n        </div>\n      </>\n    )\n  }\n  else {\n    return (\n      <>\n        <GlobalCSS inject={args.css}/>\n        <div ref={observe} className=\"slides\">\n          <section data-markdown={\"\"} {...args[\"markdown_props\"]}>\n            <script type={\"text/template\"}>\n              {args[\"content\"]}\n            </script>\n          </section>\n        </div>\n      </>\n    )\n  }\n}\n\n// \"withStreamlitConnection\" is a wrapper function. It bootstraps the\n// connection between your component and the Streamlit app, and handles\n// passing arguments from Python -> Component.\n//\n// You don't need to edit withStreamlitConnection (but you're welcome to!).\nexport default withStreamlitConnection(RevealSlides)\n",
+        "import {\n  Streamlit,\n  ComponentProps,\n  withStreamlitConnection,\n  Theme,\n} from \"streamlit-component-lib\"\nimport { useEffect, useMemo } from \"react\"\nimport { createGlobalStyle } from \"styled-components/macro\"\n\n\nimport Reveal from 'reveal.js';\nimport RevealMarkdown from 'reveal.js/plugin/markdown/markdown';\nimport RevealHighlight from 'reveal.js/plugin/highlight/highlight';\nimport RevealMath from 'reveal.js/plugin/math/math';\nimport RevealSearch from 'reveal.js/plugin/search/search';\nimport RevealNotes from 'reveal.js/plugin/notes/notes';\nimport RevealZoom from 'reveal.js/plugin/zoom/zoom';\n\n\nimport 'reveal.js/dist/reveal.css';\nimport 'reveal.js/plugin/highlight/monokai.css';\n\ninterface RevealSlidesProps extends ComponentProps {\n  args: any\n  width: number\n  disabled: boolean\n  theme?: Theme\n}\n\nconst GlobalCSS = createGlobalStyle<{ inject: string}>`\n  ${props => props.inject}\n`\n\nconst includedPlugins = {\"markdown\": RevealMarkdown, \"highlight\": RevealHighlight, \"katex\": RevealMath.KaTeX, \"mathjax2\": RevealMath.MathJax2, \"mathjax3\": RevealMath.MathJax3, \"search\": RevealSearch, \"notes\": RevealNotes, \"zoom\": RevealZoom}\n// const simpleCommands = {\"left\": Reveal.left, \"right\": () => {Reveal.right()}, \"up\": Reveal.up, \"down\": Reveal.down, \"prev\": Reveal.prev, \"next\": Reveal.next, \"prevFragment\": Reveal.prevFragment, \"nextFragment\": Reveal.nextFragment, \"togglePause\": Reveal.togglePause, \"toggleAutoSlide\": Reveal.toggleAutoSlide, \"toggleHelp\": Reveal.toggleHelp, \"toggleOverview\": Reveal.toggleOverview, \"shuffle\": Reveal.shuffle}\n// const commandsWithArgs = {slide: Reveal.slide, togglePause: Reveal.togglePause, toggleAutoSlide: Reveal.toggleAutoSlide, toggleHelp: Reveal.toggleHelp, toggleOverview: Reveal.toggleOverview}\n\nconst defaultConfig = {\n  // The \"normal\" size of the presentation, aspect ratio will be preserved\n\t// when the presentation is scaled to fit different resolutions\n\twidth: 900,\n\theight: 860,\n\t\n\t// Factor of the display size that should remain empty around the content\n\tmargin: 0.05,\n\n\t// Bounds for smallest/largest possible scale to apply to content\n\tminScale: 0.1,\n\tmaxScale: 3.0,\n\n\t// Help the user learn the controls by providing hints, for example by\n\t// bouncing the down arrow when they first encounter a vertical slide\n\tcontrolsTutorial: true,\n\n\t// Determines where controls appear, \"edges\" or \"bottom-right\"\n\tcontrolsLayout: 'edges',\n}\n\n/**\n * This is a React-based component template. The `render()` function is called\n * automatically when your component should be re-rendered.\n */\nconst RevealSlides = ({ args, disabled }: RevealSlidesProps) => {   \n\n  let configStr = JSON.stringify(args[\"config\"])\n  let initStateStr = JSON.stringify(args[\"initial_state\"])\n  // const commandStr = JSON.stringify(args[\"commands\"])\n\n  const setupConfig = (configString: string) : object => {\n    const config = {...defaultConfig, ...JSON.parse(configStr)}\n    // code to run after render goes here\n    if (args[\"allow_unsafe_html\"]) {\n      // do nothing\n    }\n    else {\n      if ('plugins' in config){\n        var arr = config['plugins'];\n        arr.forEach(function(moduleName: string, index: number) {\n          if (moduleName in includedPlugins){\n            arr[index] = (includedPlugins as any)[moduleName];\n          }\n          else {\n            arr[index] = null;\n          }\n        });\n        config['plugins'] = arr.filter((x:any) => !!x) as any[];\n        if(!config['plugins'].includes(RevealMarkdown)){\n          config['plugins'].push(RevealMarkdown);\n        }\n      }\n      else {\n        config['plugins'] = [RevealMarkdown];\n      }\n    }\n    return config;\n  }\n\n  useMemo(()=>{\n    // code to run on component mount goes here\n\n    // To do: remove or disable previously imported css. When the list of\n    // css imports exceed about 25, the page no longer updates.\n    import('../node_modules/reveal.js/dist/theme/' + args.theme + '.css').then((css) => {\n\n      try{\n        Reveal.layout();\n      }\n      catch (e){\n        console.warn(\"Reveal.layout() call failed.\")\n      }\n    \n    }).catch((err) => {\n      console.warn(\"Failed CSS import: \", err);\n    });\n\n  }, [args.theme]);\n\n  useEffect(() => {\n    const config = setupConfig(configStr)\n    \n    try {\n      Reveal.destroy();\n    }\n    catch (e) {\n    }\n    Reveal.initialize(config).then(() => {\n      // reveal.js is ready\n      \n      // For some yet to be determined reason, the highlight plugin is not initialized.\n      // Setting highlight config option highlightOnLoad to true (before passing to initialize function)\n      // does not work\n      // To Do: make sure the highlight plugin only changes the HTML involving the code once instead of many times.\n      // Possible solution is to make a change to the plugin init function.\n      let highlighter = Reveal.getPlugin('highlight') as any;\n      if (highlighter){\n        highlighter.init(Reveal);\n      }\n      \n      const initState = JSON.parse(initStateStr);\n      if(Object.keys(initState).length !== 0){\n        Reveal.setState(initState);\n      }\n\n      if(!args['display_only']){\n        // Send slide position indecies back to Streamlit on initialization and on slide change\n        const currState = Reveal.getState();\n        Streamlit.setComponentValue(currState);\n        Reveal.on( 'slidechanged', event => {\n\n          const tempState = Reveal.getState();\n          Streamlit.setComponentValue({indexh: (event as any).indexh, indexv: (event as any).indexv, indexf: tempState.indexf, paused: tempState.paused, overview: tempState.overview});\n        });\n        \n        Reveal.on( 'fragmentshown', event => {\n          // event.fragment = the fragment DOM element\n          const tempState = Reveal.getState();\n          Streamlit.setComponentValue(tempState);\n        } );\n        Reveal.on( 'fragmenthidden', event => {\n          // event.fragment = the fragment DOM element\n          const tempState = Reveal.getState();\n          Streamlit.setComponentValue(tempState);\n        } );\n        Reveal.on( 'overviewshown', event => {\n          // event.overview = the overview DOM element\n          const tempState = Reveal.getState();\n          Streamlit.setComponentValue(tempState);\n        } );\n        Reveal.on( 'overviewhidden', event => {\n          // event.overview = the overview DOM element\n          const tempState = Reveal.getState();\n          Streamlit.setComponentValue(tempState);\n        } );\n        Reveal.on( 'paused', event => {\n          // event.fragment = the fragment DOM element\n          const tempState = Reveal.getState();\n          Streamlit.setComponentValue(tempState);\n        } );\n        Reveal.on( 'resumed', event => {\n          // event.fragment = the fragment DOM element\n          const tempState = Reveal.getState();\n          Streamlit.setComponentValue(tempState);\n        } );\n      }\n    });\n\n    return () => {\n      // code to run on component unmount goes here\n      Reveal.destroy();  \n    }\n  }, []);\n\n  // Reconfigure reveal.js if config changes\n  useEffect(() => {\n    const existingPlugins = Reveal.getPlugins();\n    const config = setupConfig(configStr)\n\n    // Add and register plugins that are not already loaded\n    let existingPluginsList : string[] = Object.values(existingPlugins).map((plugin: any) => plugin.id);\n    if('plugins' in args[\"config\"]){\n      const plugins = args[\"config\"][\"plugins\"];\n      (plugins as string[]).forEach((plugin: string) => {\n        if (plugin && existingPluginsList.indexOf(plugin) === -1){\n          Reveal.registerPlugin((includedPlugins as any)[plugin]);\n        }\n      });\n\n      //// Remove plugins that are no longer in the list (does not work yet..some signs there is a bug in Reveal.Plugin)\n      // Object.values(existingPlugins as {[id: string]: Reveal.Plugin;}).forEach((plugin: any) => {\n      //   if (plugin.id && plugin.id !=='markdown' && plugins.indexOf(plugin.id) === -1){\n      //     console.log(\"destroy plugin: \" + plugin.id);\n      //     if( typeof plugin.destroy === 'function' ) {\n      //       plugin.destroy();\n      //     }\n      //   }\n      // });\n    }\n    // Reconfigure reveal.js\n    Reveal.configure(config);\n  }, [configStr, args[\"allow_unsafe_html\"]]);\n\n  useEffect(() => {\n    const initState = JSON.parse(initStateStr);\n    if (Reveal.isReady() && Object.keys(initState).length !== 0){\n      Reveal.setState(initState);\n    }\n  }, [initStateStr]);\n\n  useEffect(() => {\n    if (Reveal.isReady()){\n      if (disabled){\n        Reveal.togglePause(true);\n        let viewport = Reveal.getViewportElement();\n        if (viewport){\n          viewport.style.pointerEvents = \"none\";\n        }\n      }\n      else {  \n        Reveal.togglePause(false);\n        let viewport = Reveal.getViewportElement();\n        if (viewport){\n          viewport.style.pointerEvents = \"auto\";\n        }\n      }\n    }\n  }, [disabled]);\n\n  //To do: add support for commands (i.e. control slides from Streamlit)\n  //-----------------\n  // useEffect(() => {\n  //   const commands = JSON.parse(commandStr)\n  //   if (Array.isArray(commands) && commands.length > 0 && Reveal.isReady()){\n  //     commands.forEach((command: any) => {\n  //       if (typeof command === \"string\" && command in simpleCommands){\n  //         (simpleCommands as any)[command]();\n  //       }\n  //       else if (Array.isArray(command) && command.length > 0 && typeof command[0] === \"string\" && command[0] in commandsWithArgs){\n  //         if (command[0] === \"slide\"){\n  //           if (command.length === 3){\n  //             Reveal.slide(command[1], command[2]);\n  //           }\n  //           else if (command.length === 4){\n  //             Reveal.slide(command[1], command[2], command[3]);\n  //           }\n  //           else {\n  //             console.warn(\"Invalid slide command: slide command array must have 3 or 4 elements.\");\n  //           }\n  //         }\n  //         else {\n  //           (commandsWithArgs as any)[command[0]](command[1]);\n  //         }\n  //       }\n  //       else {\n  //         console.warn(\"Invalid command: command must be a string or an array containing a string as its first element.\");\n  //       }\n  //     });\n  //   }\n  //   else if (!Array.isArray(args[\"commands\"])) {\n  //     console.warn(\"Invalid commands property value: commands must be an array containing at least one command.\");\n  //   }\n  // }, [commandStr]);\n\n  /**\n   * resizeObserver observes changes in elements its given to observe and is used here\n   * to communicate to streamlit the height of the component that has changed\n   * so that streamlit can adjust the iframe containing the component accordingly.\n   */\n  const resizeObserver = new ResizeObserver((entries: any) => {\n    // If we know that the body will always fully contain our component (without cutting it off)\n    // then we can use docuemnt.body height instead\n    if (args[\"height\"] === \"auto\" || typeof args[\"height\"] !== \"number\"){\n      Streamlit.setFrameHeight((entries[0].contentBoxSize.blockSize ?? entries[0].contentRect.height)); \n      if (Reveal.isReady()){\n        Reveal.layout();\n      }\n    }\n    else {\n      Streamlit.setFrameHeight(args[\"height\"]);\n      if (Reveal.isReady()){\n        Reveal.layout();\n      }\n    }\n    \n  })\n\n  const observe = (divElem: any) => {\n    divElem ? resizeObserver.observe(divElem as HTMLDivElement) : resizeObserver.disconnect();\n  }\n\n  if (args[\"allow_unsafe_html\"]) {\n    return (\n      <>\n        <GlobalCSS inject={args.css}/>\n        <div ref={observe} className=\"slides\" dangerouslySetInnerHTML={{__html: args[\"content\"]}}>\n        </div>\n      </>\n    )\n  }\n  else {\n    return (\n      <>\n        <GlobalCSS inject={args.css}/>\n        <div ref={observe} className=\"slides\">\n          <section data-markdown={\"\"} {...args[\"markdown_props\"]}>\n            <script type={\"text/template\"}>\n              {args[\"content\"]}\n            </script>\n          </section>\n        </div>\n      </>\n    )\n  }\n}\n\n// \"withStreamlitConnection\" is a wrapper function. It bootstraps the\n// connection between your component and the Streamlit app, and handles\n// passing arguments from Python -> Component.\n//\n// You don't need to edit withStreamlitConnection (but you're welcome to!).\nexport default withStreamlitConnection(RevealSlides)\n",
         "import React from \"react\"\nimport ReactDOM from \"react-dom\"\nimport RevealSlides from \"./RevealSlides\"\n\nReactDOM.render(\n  <React.StrictMode>\n    <RevealSlides />\n  </React.StrictMode>,\n  document.getElementById(\"root\")\n)\n"
     ],
     "version": 3
 }
```

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/runtime-main.eaac28ce.js` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/runtime-main.eaac28ce.js`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/js/runtime-main.eaac28ce.js.map` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/js/runtime-main.eaac28ce.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/league-gothic.080eee2a.woff` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/media/league-gothic.080eee2a.woff`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/league-gothic.12baac5d.eot` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/media/league-gothic.12baac5d.eot`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/league-gothic.6ae91382.ttf` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/media/league-gothic.6ae91382.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-italic.10a5cb40.ttf` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/media/source-sans-pro-italic.10a5cb40.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-italic.97e79d3e.eot` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/media/source-sans-pro-italic.97e79d3e.eot`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-italic.983d97ca.woff` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/media/source-sans-pro-italic.983d97ca.woff`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-regular.36443d24.eot` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/media/source-sans-pro-regular.36443d24.eot`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-regular.45c54810.ttf` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/media/source-sans-pro-regular.45c54810.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-regular.d1653550.woff` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/media/source-sans-pro-regular.d1653550.woff`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.6ebea875.ttf` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.6ebea875.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.83db537e.eot` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.83db537e.eot`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.f11ba60a.woff` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.f11ba60a.woff`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.522a9ee9.ttf` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.522a9ee9.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.a43f56ac.woff` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.a43f56ac.woff`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.fb03c660.eot` & `streamlit-reveal-slides-0.1.7/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.fb03c660.eot`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.6/setup.py` & `streamlit-reveal-slides-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit-reveal-slides",
-    version="0.1.6",
+    version="0.1.7",
     author="Anas Bouzid",
     author_email="",
     description="reveal.js HTML presentations for streamlit",
     long_description="create and add reveal.js HTML presentations to your streamlit app",
     long_description_content_type="text/plain",
     url="https://github.com/bouzidanas/streamlit.io/tree/master/streamlit-reveal-slides",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-reveal-slides-0.1.6/streamlit_reveal_slides.egg-info/SOURCES.txt` & `streamlit-reveal-slides-0.1.7/streamlit_reveal_slides.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -75,16 +75,16 @@
 reveal_slides/frontend/build/static/js/6.e9192981.chunk.js.map
 reveal_slides/frontend/build/static/js/7.be794506.chunk.js
 reveal_slides/frontend/build/static/js/7.be794506.chunk.js.map
 reveal_slides/frontend/build/static/js/8.15dd3b20.chunk.js
 reveal_slides/frontend/build/static/js/8.15dd3b20.chunk.js.map
 reveal_slides/frontend/build/static/js/9.119f08fa.chunk.js
 reveal_slides/frontend/build/static/js/9.119f08fa.chunk.js.map
-reveal_slides/frontend/build/static/js/main.3837bbb6.chunk.js
-reveal_slides/frontend/build/static/js/main.3837bbb6.chunk.js.map
+reveal_slides/frontend/build/static/js/main.befe19ba.chunk.js
+reveal_slides/frontend/build/static/js/main.befe19ba.chunk.js.map
 reveal_slides/frontend/build/static/js/runtime-main.eaac28ce.js
 reveal_slides/frontend/build/static/js/runtime-main.eaac28ce.js.map
 reveal_slides/frontend/build/static/media/league-gothic.080eee2a.woff
 reveal_slides/frontend/build/static/media/league-gothic.12baac5d.eot
 reveal_slides/frontend/build/static/media/league-gothic.6ae91382.ttf
 reveal_slides/frontend/build/static/media/source-sans-pro-italic.10a5cb40.ttf
 reveal_slides/frontend/build/static/media/source-sans-pro-italic.97e79d3e.eot
```

