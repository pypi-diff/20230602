# Comparing `tmp/ipyvolume-0.6.2.tar.gz` & `tmp/ipyvolume-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyvolume-0.6.2.tar", last modified: Fri Jun  2 13:32:07 2023, max compression
+gzip compressed data, was "ipyvolume-0.6.3.tar", last modified: Fri Jun  2 14:33:03 2023, max compression
```

## Comparing `ipyvolume-0.6.2.tar` & `ipyvolume-0.6.3.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:32:07.288249 ipyvolume-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-02 13:29:46.000000 ipyvolume-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-02 13:29:46.000000 ipyvolume-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-02 13:32:07.288249 ipyvolume-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-06-02 13:29:46.000000 ipyvolume-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-02 13:29:46.000000 ipyvolume-0.6.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:32:07.272249 ipyvolume-0.6.2/etc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:32:07.272249 ipyvolume-0.6.2/etc/jupyter/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:32:07.272249 ipyvolume-0.6.2/etc/jupyter/nbconfig/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:32:07.276249 ipyvolume-0.6.2/etc/jupyter/nbconfig/notebook.d/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-02 13:29:47.000000 ipyvolume-0.6.2/etc/jupyter/nbconfig/notebook.d/ipyvolume.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:32:07.276249 ipyvolume-0.6.2/ipyvolume/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-02 13:29:47.000000 ipyvolume-0.6.2/ipyvolume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-02 13:29:47.000000 ipyvolume-0.6.2/ipyvolume/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-06-02 13:29:47.000000 ipyvolume-0.6.2/ipyvolume/astro.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-02 13:29:47.000000 ipyvolume-0.6.2/ipyvolume/bokeh.py
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-06-02 13:29:47.000000 ipyvolume-0.6.2/ipyvolume/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-06-02 13:29:47.000000 ipyvolume-0.6.2/ipyvolume/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-06-02 13:29:47.000000 ipyvolume-0.6.2/ipyvolume/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-02 13:29:47.000000 ipyvolume-0.6.2/ipyvolume/headless.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-02 13:29:47.000000 ipyvolume-0.6.2/ipyvolume/hotreload.py
--rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-06-02 13:29:47.000000 ipyvolume-0.6.2/ipyvolume/moviemaker.py
--rw-r--r--   0 runner    (1001) docker     (123)    69007 2023-06-02 13:29:47.000000 ipyvolume-0.6.2/ipyvolume/pylab.py
--rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-06-02 13:29:47.000000 ipyvolume-0.6.2/ipyvolume/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-02 13:29:47.000000 ipyvolume-0.6.2/ipyvolume/styles.py
--rw-r--r--   0 runner    (1001) docker     (123)    14319 2023-06-02 13:29:47.000000 ipyvolume-0.6.2/ipyvolume/test_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-02 13:29:47.000000 ipyvolume-0.6.2/ipyvolume/traittypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-06-02 13:29:47.000000 ipyvolume-0.6.2/ipyvolume/transferfunction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-02 13:29:47.000000 ipyvolume-0.6.2/ipyvolume/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    11205 2023-06-02 13:29:47.000000 ipyvolume-0.6.2/ipyvolume/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:32:07.280249 ipyvolume-0.6.2/ipyvolume/vue/
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-06-02 13:29:47.000000 ipyvolume-0.6.2/ipyvolume/vue/container.vue
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-02 13:29:47.000000 ipyvolume-0.6.2/ipyvolume/vue/legend.vue
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-02 13:29:47.000000 ipyvolume-0.6.2/ipyvolume/vue/popup.vue
--rw-r--r--   0 runner    (1001) docker     (123)    25405 2023-06-02 13:29:47.000000 ipyvolume-0.6.2/ipyvolume/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:32:07.276249 ipyvolume-0.6.2/ipyvolume.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-02 13:32:07.000000 ipyvolume-0.6.2/ipyvolume.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-02 13:32:07.000000 ipyvolume-0.6.2/ipyvolume.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 13:32:07.000000 ipyvolume-0.6.2/ipyvolume.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 13:32:07.000000 ipyvolume-0.6.2/ipyvolume.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-02 13:32:07.000000 ipyvolume-0.6.2/ipyvolume.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-02 13:32:07.000000 ipyvolume-0.6.2/ipyvolume.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:32:07.280249 ipyvolume-0.6.2/js/
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-02 13:29:47.000000 ipyvolume-0.6.2/js/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-02 13:29:47.000000 ipyvolume-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-02 13:32:07.288249 ipyvolume-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-02 13:29:47.000000 ipyvolume-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:32:07.272249 ipyvolume-0.6.2/share/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:32:07.272249 ipyvolume-0.6.2/share/jupyter/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:32:07.272249 ipyvolume-0.6.2/share/jupyter/labextensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:32:07.280249 ipyvolume-0.6.2/share/jupyter/labextensions/ipyvolume/
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-06-02 13:31:55.000000 ipyvolume-0.6.2/share/jupyter/labextensions/ipyvolume/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:32:07.280249 ipyvolume-0.6.2/share/jupyter/labextensions/ipyvolume/static/
--rw-r--r--   0 runner    (1001) docker     (123)   559918 2023-06-02 13:31:55.000000 ipyvolume-0.6.2/share/jupyter/labextensions/ipyvolume/static/212.b0149a14735c9b14c049.js
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-02 13:31:55.000000 ipyvolume-0.6.2/share/jupyter/labextensions/ipyvolume/static/212.b0149a14735c9b14c049.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-02 13:31:55.000000 ipyvolume-0.6.2/share/jupyter/labextensions/ipyvolume/static/261.a9c9630b28934bcbf1c3.js
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-06-02 13:31:55.000000 ipyvolume-0.6.2/share/jupyter/labextensions/ipyvolume/static/466.df53a5241872f78b6b60.js
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-02 13:31:55.000000 ipyvolume-0.6.2/share/jupyter/labextensions/ipyvolume/static/466.df53a5241872f78b6b60.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    70101 2023-06-02 13:31:55.000000 ipyvolume-0.6.2/share/jupyter/labextensions/ipyvolume/static/486.59ac5542d87a8f7709e9.js
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-02 13:31:55.000000 ipyvolume-0.6.2/share/jupyter/labextensions/ipyvolume/static/486.59ac5542d87a8f7709e9.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-02 13:31:55.000000 ipyvolume-0.6.2/share/jupyter/labextensions/ipyvolume/static/501.54c2baeab80ecb56ca08.js
--rw-r--r--   0 runner    (1001) docker     (123)   342388 2023-06-02 13:31:55.000000 ipyvolume-0.6.2/share/jupyter/labextensions/ipyvolume/static/568.5edc20b9bebeb1dddffc.js
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-02 13:31:55.000000 ipyvolume-0.6.2/share/jupyter/labextensions/ipyvolume/static/577.ef610ec4539ffe9cddc1.js
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-02 13:31:55.000000 ipyvolume-0.6.2/share/jupyter/labextensions/ipyvolume/static/577.ef610ec4539ffe9cddc1.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-06-02 13:31:55.000000 ipyvolume-0.6.2/share/jupyter/labextensions/ipyvolume/static/58.5dd767d4301576cee659.js
--rw-r--r--   0 runner    (1001) docker     (123)   249038 2023-06-02 13:31:55.000000 ipyvolume-0.6.2/share/jupyter/labextensions/ipyvolume/static/64.e6b27f39dcb5e033dca2.js
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-06-02 13:31:55.000000 ipyvolume-0.6.2/share/jupyter/labextensions/ipyvolume/static/861.845bccd8cacebe4b0886.js
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-02 13:31:55.000000 ipyvolume-0.6.2/share/jupyter/labextensions/ipyvolume/static/861.845bccd8cacebe4b0886.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10492 2023-06-02 13:31:55.000000 ipyvolume-0.6.2/share/jupyter/labextensions/ipyvolume/static/943.4d08ec41a49be026ca9f.js
--rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-06-02 13:31:55.000000 ipyvolume-0.6.2/share/jupyter/labextensions/ipyvolume/static/remoteEntry.f52c61a5425bd83d7ff9.js
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-02 13:31:40.000000 ipyvolume-0.6.2/share/jupyter/labextensions/ipyvolume/static/style.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:32:07.272249 ipyvolume-0.6.2/share/jupyter/nbextensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:32:07.284249 ipyvolume-0.6.2/share/jupyter/nbextensions/ipyvolume/
--rw-r--r--   0 runner    (1001) docker     (123)     9698 2023-06-02 13:31:56.000000 ipyvolume-0.6.2/share/jupyter/nbextensions/ipyvolume/extension.js
--rw-r--r--   0 runner    (1001) docker     (123)  3883902 2023-06-02 13:32:07.000000 ipyvolume-0.6.2/share/jupyter/nbextensions/ipyvolume/index.js
--rw-r--r--   0 runner    (1001) docker     (123)   571575 2023-06-02 13:31:58.000000 ipyvolume-0.6.2/share/jupyter/nbextensions/ipyvolume/three.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:03.346598 ipyvolume-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-02 14:30:42.000000 ipyvolume-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-02 14:30:42.000000 ipyvolume-0.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-02 14:33:03.346598 ipyvolume-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-06-02 14:30:42.000000 ipyvolume-0.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-02 14:30:42.000000 ipyvolume-0.6.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:03.334597 ipyvolume-0.6.3/etc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:03.334597 ipyvolume-0.6.3/etc/jupyter/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:03.334597 ipyvolume-0.6.3/etc/jupyter/nbconfig/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:03.338598 ipyvolume-0.6.3/etc/jupyter/nbconfig/notebook.d/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-02 14:30:42.000000 ipyvolume-0.6.3/etc/jupyter/nbconfig/notebook.d/ipyvolume.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:03.338598 ipyvolume-0.6.3/ipyvolume/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-02 14:30:42.000000 ipyvolume-0.6.3/ipyvolume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-02 14:30:42.000000 ipyvolume-0.6.3/ipyvolume/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-06-02 14:30:42.000000 ipyvolume-0.6.3/ipyvolume/astro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-02 14:30:42.000000 ipyvolume-0.6.3/ipyvolume/bokeh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-06-02 14:30:42.000000 ipyvolume-0.6.3/ipyvolume/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-06-02 14:30:42.000000 ipyvolume-0.6.3/ipyvolume/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-06-02 14:30:42.000000 ipyvolume-0.6.3/ipyvolume/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-02 14:30:42.000000 ipyvolume-0.6.3/ipyvolume/headless.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-02 14:30:42.000000 ipyvolume-0.6.3/ipyvolume/hotreload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-06-02 14:30:42.000000 ipyvolume-0.6.3/ipyvolume/moviemaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69007 2023-06-02 14:30:42.000000 ipyvolume-0.6.3/ipyvolume/pylab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-06-02 14:30:42.000000 ipyvolume-0.6.3/ipyvolume/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-02 14:30:42.000000 ipyvolume-0.6.3/ipyvolume/styles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14319 2023-06-02 14:30:42.000000 ipyvolume-0.6.3/ipyvolume/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-02 14:30:42.000000 ipyvolume-0.6.3/ipyvolume/traittypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-06-02 14:30:42.000000 ipyvolume-0.6.3/ipyvolume/transferfunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-02 14:30:42.000000 ipyvolume-0.6.3/ipyvolume/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11205 2023-06-02 14:30:42.000000 ipyvolume-0.6.3/ipyvolume/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:03.338598 ipyvolume-0.6.3/ipyvolume/vue/
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-06-02 14:30:42.000000 ipyvolume-0.6.3/ipyvolume/vue/container.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-02 14:30:42.000000 ipyvolume-0.6.3/ipyvolume/vue/legend.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-02 14:30:42.000000 ipyvolume-0.6.3/ipyvolume/vue/popup.vue
+-rw-r--r--   0 runner    (1001) docker     (123)    25405 2023-06-02 14:30:42.000000 ipyvolume-0.6.3/ipyvolume/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:03.338598 ipyvolume-0.6.3/ipyvolume.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-02 14:33:03.000000 ipyvolume-0.6.3/ipyvolume.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-02 14:33:03.000000 ipyvolume-0.6.3/ipyvolume.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:33:03.000000 ipyvolume-0.6.3/ipyvolume.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:33:03.000000 ipyvolume-0.6.3/ipyvolume.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-02 14:33:03.000000 ipyvolume-0.6.3/ipyvolume.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-02 14:33:03.000000 ipyvolume-0.6.3/ipyvolume.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:03.338598 ipyvolume-0.6.3/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-02 14:30:42.000000 ipyvolume-0.6.3/js/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-02 14:30:42.000000 ipyvolume-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-02 14:33:03.346598 ipyvolume-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-02 14:30:42.000000 ipyvolume-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:03.334597 ipyvolume-0.6.3/share/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:03.334597 ipyvolume-0.6.3/share/jupyter/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:03.334597 ipyvolume-0.6.3/share/jupyter/labextensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:03.338598 ipyvolume-0.6.3/share/jupyter/labextensions/ipyvolume/
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-06-02 14:32:51.000000 ipyvolume-0.6.3/share/jupyter/labextensions/ipyvolume/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:03.342598 ipyvolume-0.6.3/share/jupyter/labextensions/ipyvolume/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   559918 2023-06-02 14:32:51.000000 ipyvolume-0.6.3/share/jupyter/labextensions/ipyvolume/static/212.b0149a14735c9b14c049.js
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-02 14:32:51.000000 ipyvolume-0.6.3/share/jupyter/labextensions/ipyvolume/static/212.b0149a14735c9b14c049.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-02 14:32:51.000000 ipyvolume-0.6.3/share/jupyter/labextensions/ipyvolume/static/261.a9c9630b28934bcbf1c3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-06-02 14:32:51.000000 ipyvolume-0.6.3/share/jupyter/labextensions/ipyvolume/static/466.df53a5241872f78b6b60.js
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-02 14:32:51.000000 ipyvolume-0.6.3/share/jupyter/labextensions/ipyvolume/static/466.df53a5241872f78b6b60.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    70101 2023-06-02 14:32:51.000000 ipyvolume-0.6.3/share/jupyter/labextensions/ipyvolume/static/486.59ac5542d87a8f7709e9.js
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-02 14:32:51.000000 ipyvolume-0.6.3/share/jupyter/labextensions/ipyvolume/static/486.59ac5542d87a8f7709e9.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-02 14:32:51.000000 ipyvolume-0.6.3/share/jupyter/labextensions/ipyvolume/static/501.54c2baeab80ecb56ca08.js
+-rw-r--r--   0 runner    (1001) docker     (123)   342388 2023-06-02 14:32:51.000000 ipyvolume-0.6.3/share/jupyter/labextensions/ipyvolume/static/568.df354347cf6898d012c4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-02 14:32:51.000000 ipyvolume-0.6.3/share/jupyter/labextensions/ipyvolume/static/577.ef610ec4539ffe9cddc1.js
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-02 14:32:51.000000 ipyvolume-0.6.3/share/jupyter/labextensions/ipyvolume/static/577.ef610ec4539ffe9cddc1.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-06-02 14:32:51.000000 ipyvolume-0.6.3/share/jupyter/labextensions/ipyvolume/static/58.5dd767d4301576cee659.js
+-rw-r--r--   0 runner    (1001) docker     (123)   249038 2023-06-02 14:32:51.000000 ipyvolume-0.6.3/share/jupyter/labextensions/ipyvolume/static/64.e6b27f39dcb5e033dca2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-06-02 14:32:51.000000 ipyvolume-0.6.3/share/jupyter/labextensions/ipyvolume/static/861.845bccd8cacebe4b0886.js
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-02 14:32:51.000000 ipyvolume-0.6.3/share/jupyter/labextensions/ipyvolume/static/861.845bccd8cacebe4b0886.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10492 2023-06-02 14:32:51.000000 ipyvolume-0.6.3/share/jupyter/labextensions/ipyvolume/static/943.4d08ec41a49be026ca9f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-06-02 14:32:51.000000 ipyvolume-0.6.3/share/jupyter/labextensions/ipyvolume/static/remoteEntry.6b98305c8298015194ea.js
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-02 14:32:36.000000 ipyvolume-0.6.3/share/jupyter/labextensions/ipyvolume/static/style.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:03.334597 ipyvolume-0.6.3/share/jupyter/nbextensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:33:03.346598 ipyvolume-0.6.3/share/jupyter/nbextensions/ipyvolume/
+-rw-r--r--   0 runner    (1001) docker     (123)     9698 2023-06-02 14:32:52.000000 ipyvolume-0.6.3/share/jupyter/nbextensions/ipyvolume/extension.js
+-rw-r--r--   0 runner    (1001) docker     (123)  3883902 2023-06-02 14:33:03.000000 ipyvolume-0.6.3/share/jupyter/nbextensions/ipyvolume/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)   571575 2023-06-02 14:32:55.000000 ipyvolume-0.6.3/share/jupyter/nbextensions/ipyvolume/three.js
```

### Comparing `ipyvolume-0.6.2/LICENSE` & `ipyvolume-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyvolume-0.6.2/PKG-INFO` & `ipyvolume-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyvolume
-Version: 0.6.2
+Version: 0.6.3
 Summary: IPython widget for rendering 3d volumes
 Home-page: https://github.com/maartenbreddels/ipyvolume
 Author: Maarten A. Breddels
 Author-email: maartenbreddels@gmail.com
 License: MIT
 Keywords: ipython,jupyter,widgets,volume rendering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ipyvolume-0.6.2/README.md` & `ipyvolume-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `ipyvolume-0.6.2/README.rst` & `ipyvolume-0.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `ipyvolume-0.6.2/ipyvolume/__init__.py` & `ipyvolume-0.6.3/ipyvolume/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyvolume-0.6.2/ipyvolume/astro.py` & `ipyvolume-0.6.3/ipyvolume/astro.py`

 * *Files identical despite different names*

### Comparing `ipyvolume-0.6.2/ipyvolume/bokeh.py` & `ipyvolume-0.6.3/ipyvolume/bokeh.py`

 * *Files identical despite different names*

### Comparing `ipyvolume-0.6.2/ipyvolume/datasets.py` & `ipyvolume-0.6.3/ipyvolume/datasets.py`

 * *Files identical despite different names*

### Comparing `ipyvolume-0.6.2/ipyvolume/embed.py` & `ipyvolume-0.6.3/ipyvolume/embed.py`

 * *Files identical despite different names*

### Comparing `ipyvolume-0.6.2/ipyvolume/examples.py` & `ipyvolume-0.6.3/ipyvolume/examples.py`

 * *Files identical despite different names*

### Comparing `ipyvolume-0.6.2/ipyvolume/headless.py` & `ipyvolume-0.6.3/ipyvolume/headless.py`

 * *Files identical despite different names*

### Comparing `ipyvolume-0.6.2/ipyvolume/hotreload.py` & `ipyvolume-0.6.3/ipyvolume/hotreload.py`

 * *Files identical despite different names*

### Comparing `ipyvolume-0.6.2/ipyvolume/moviemaker.py` & `ipyvolume-0.6.3/ipyvolume/moviemaker.py`

 * *Files identical despite different names*

### Comparing `ipyvolume-0.6.2/ipyvolume/pylab.py` & `ipyvolume-0.6.3/ipyvolume/pylab.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -201,14 +201,15 @@
     :param int height:  .. height ..
     :param bool lighting: use lighting or not
     :param bool controls: show controls or not
     :param bool controls_vr: show controls for VR or not
     :param bool debug: show debug buttons or not
     :return: :any:`Figure`
     """
+    utils.colab_workarounds()
     if key is not None and key in current.figures:
         current.figure = current.figures[key]
         current.container = current.containers[key]
     elif isinstance(key, ipv.Figure) and key in current.figures.values():
         key_index = list(current.figures.values()).index(key)
         key = list(current.figures.keys())[key_index]
         current.figure = current.figures[key]
@@ -811,15 +812,14 @@
     fig.scatters = fig.scatters + [s]
     return s
 
 
 def show(extra_widgets=[]):
     """Display (like in IPython.display.dispay(...)) the current figure."""
     gcf()  # make sure we have something..
-    utils.colab_workarounds()
     display(gcc())
     for widget in extra_widgets:
         display(widget)
 
 
 def animate_glyphs(*args, **kwargs):
     """Deprecated: please use animation_control."""
```

### Comparing `ipyvolume-0.6.2/ipyvolume/serialize.py` & `ipyvolume-0.6.3/ipyvolume/serialize.py`

 * *Files identical despite different names*

### Comparing `ipyvolume-0.6.2/ipyvolume/styles.py` & `ipyvolume-0.6.3/ipyvolume/styles.py`

 * *Files identical despite different names*

### Comparing `ipyvolume-0.6.2/ipyvolume/test_all.py` & `ipyvolume-0.6.3/ipyvolume/test_all.py`

 * *Files identical despite different names*

### Comparing `ipyvolume-0.6.2/ipyvolume/transferfunction.py` & `ipyvolume-0.6.3/ipyvolume/transferfunction.py`

 * *Files identical despite different names*

### Comparing `ipyvolume-0.6.2/ipyvolume/ui.py` & `ipyvolume-0.6.3/ipyvolume/ui.py`

 * *Files identical despite different names*

### Comparing `ipyvolume-0.6.2/ipyvolume/utils.py` & `ipyvolume-0.6.3/ipyvolume/utils.py`

 * *Files identical despite different names*

### Comparing `ipyvolume-0.6.2/ipyvolume/vue/container.vue` & `ipyvolume-0.6.3/ipyvolume/vue/container.vue`

 * *Files identical despite different names*

### Comparing `ipyvolume-0.6.2/ipyvolume/vue/legend.vue` & `ipyvolume-0.6.3/ipyvolume/vue/legend.vue`

 * *Files identical despite different names*

### Comparing `ipyvolume-0.6.2/ipyvolume/vue/popup.vue` & `ipyvolume-0.6.3/ipyvolume/vue/popup.vue`

 * *Files identical despite different names*

### Comparing `ipyvolume-0.6.2/ipyvolume/widgets.py` & `ipyvolume-0.6.3/ipyvolume/widgets.py`

 * *Files identical despite different names*

### Comparing `ipyvolume-0.6.2/ipyvolume.egg-info/PKG-INFO` & `ipyvolume-0.6.3/ipyvolume.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyvolume
-Version: 0.6.2
+Version: 0.6.3
 Summary: IPython widget for rendering 3d volumes
 Home-page: https://github.com/maartenbreddels/ipyvolume
 Author: Maarten A. Breddels
 Author-email: maartenbreddels@gmail.com
 License: MIT
 Keywords: ipython,jupyter,widgets,volume rendering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ipyvolume-0.6.2/ipyvolume.egg-info/SOURCES.txt` & `ipyvolume-0.6.3/ipyvolume.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -40,20 +40,20 @@
 share/jupyter/labextensions/ipyvolume/static/212.b0149a14735c9b14c049.js.LICENSE.txt
 share/jupyter/labextensions/ipyvolume/static/261.a9c9630b28934bcbf1c3.js
 share/jupyter/labextensions/ipyvolume/static/466.df53a5241872f78b6b60.js
 share/jupyter/labextensions/ipyvolume/static/466.df53a5241872f78b6b60.js.LICENSE.txt
 share/jupyter/labextensions/ipyvolume/static/486.59ac5542d87a8f7709e9.js
 share/jupyter/labextensions/ipyvolume/static/486.59ac5542d87a8f7709e9.js.LICENSE.txt
 share/jupyter/labextensions/ipyvolume/static/501.54c2baeab80ecb56ca08.js
-share/jupyter/labextensions/ipyvolume/static/568.5edc20b9bebeb1dddffc.js
+share/jupyter/labextensions/ipyvolume/static/568.df354347cf6898d012c4.js
 share/jupyter/labextensions/ipyvolume/static/577.ef610ec4539ffe9cddc1.js
 share/jupyter/labextensions/ipyvolume/static/577.ef610ec4539ffe9cddc1.js.LICENSE.txt
 share/jupyter/labextensions/ipyvolume/static/58.5dd767d4301576cee659.js
 share/jupyter/labextensions/ipyvolume/static/64.e6b27f39dcb5e033dca2.js
 share/jupyter/labextensions/ipyvolume/static/861.845bccd8cacebe4b0886.js
 share/jupyter/labextensions/ipyvolume/static/861.845bccd8cacebe4b0886.js.LICENSE.txt
 share/jupyter/labextensions/ipyvolume/static/943.4d08ec41a49be026ca9f.js
-share/jupyter/labextensions/ipyvolume/static/remoteEntry.f52c61a5425bd83d7ff9.js
+share/jupyter/labextensions/ipyvolume/static/remoteEntry.6b98305c8298015194ea.js
 share/jupyter/labextensions/ipyvolume/static/style.js
 share/jupyter/nbextensions/ipyvolume/extension.js
 share/jupyter/nbextensions/ipyvolume/index.js
 share/jupyter/nbextensions/ipyvolume/three.js
```

### Comparing `ipyvolume-0.6.2/js/package.json` & `ipyvolume-0.6.3/js/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.6.3'"}*

```diff
@@ -101,9 +101,9 @@
         "test": "karma start --single-run",
         "watch": "npm-run-all -p watch:*",
         "watch:dev": "npm-run-all -p watch:lib watch:nbextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w --project .",
         "watch:nbextension": "webpack --watch --mode=development"
     },
-    "version": "0.6.2"
+    "version": "0.6.3"
 }
```

### Comparing `ipyvolume-0.6.2/setup.py` & `ipyvolume-0.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `ipyvolume-0.6.2/share/jupyter/labextensions/ipyvolume/package.json` & `ipyvolume-0.6.3/share/jupyter/labextensions/ipyvolume/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9603365384615384%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.6b98305c8298015194ea.js'}}",*

 * * "'version'": "'0.6.3'"}*

```diff
@@ -68,15 +68,15 @@
         "lib/three/*.js",
         "data/",
         "glsl/"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.f52c61a5425bd83d7ff9.js"
+            "load": "static/remoteEntry.6b98305c8298015194ea.js"
         },
         "extension": "lib/labplugin",
         "outputDir": "../share/jupyter/labextensions/ipyvolume",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -105,9 +105,9 @@
         "test": "karma start --single-run",
         "watch": "npm-run-all -p watch:*",
         "watch:dev": "npm-run-all -p watch:lib watch:nbextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w --project .",
         "watch:nbextension": "webpack --watch --mode=development"
     },
-    "version": "0.6.2"
+    "version": "0.6.3"
 }
```

### Comparing `ipyvolume-0.6.2/share/jupyter/labextensions/ipyvolume/static/212.b0149a14735c9b14c049.js` & `ipyvolume-0.6.3/share/jupyter/labextensions/ipyvolume/static/212.b0149a14735c9b14c049.js`

 * *Files identical despite different names*

### Comparing `ipyvolume-0.6.2/share/jupyter/labextensions/ipyvolume/static/261.a9c9630b28934bcbf1c3.js` & `ipyvolume-0.6.3/share/jupyter/labextensions/ipyvolume/static/261.a9c9630b28934bcbf1c3.js`

 * *Files identical despite different names*

### Comparing `ipyvolume-0.6.2/share/jupyter/labextensions/ipyvolume/static/466.df53a5241872f78b6b60.js` & `ipyvolume-0.6.3/share/jupyter/labextensions/ipyvolume/static/466.df53a5241872f78b6b60.js`

 * *Files identical despite different names*

### Comparing `ipyvolume-0.6.2/share/jupyter/labextensions/ipyvolume/static/486.59ac5542d87a8f7709e9.js` & `ipyvolume-0.6.3/share/jupyter/labextensions/ipyvolume/static/486.59ac5542d87a8f7709e9.js`

 * *Files identical despite different names*

### Comparing `ipyvolume-0.6.2/share/jupyter/labextensions/ipyvolume/static/501.54c2baeab80ecb56ca08.js` & `ipyvolume-0.6.3/share/jupyter/labextensions/ipyvolume/static/501.54c2baeab80ecb56ca08.js`

 * *Files identical despite different names*

### Comparing `ipyvolume-0.6.2/share/jupyter/labextensions/ipyvolume/static/568.5edc20b9bebeb1dddffc.js` & `ipyvolume-0.6.3/share/jupyter/labextensions/ipyvolume/static/568.df354347cf6898d012c4.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -3832,12 +3832,12 @@
                     return /^(#|data:|http:\/\/|https:\/\/|file:\/\/\/)/i.test(s) ? e : (a = 0 === s.indexOf("//") ? s : 0 === s.indexOf("/") ? n + s : i + s.replace(/^\.\//, ""), "url(" + JSON.stringify(a) + ")")
                 }))
             }
         },
         306: e => {
             "use strict";
             e.exports = {
-                version: "0.6.2"
+                version: "0.6.3"
             }
         }
     }
 ]);
```

### Comparing `ipyvolume-0.6.2/share/jupyter/labextensions/ipyvolume/static/577.ef610ec4539ffe9cddc1.js` & `ipyvolume-0.6.3/share/jupyter/labextensions/ipyvolume/static/577.ef610ec4539ffe9cddc1.js`

 * *Files identical despite different names*

### Comparing `ipyvolume-0.6.2/share/jupyter/labextensions/ipyvolume/static/58.5dd767d4301576cee659.js` & `ipyvolume-0.6.3/share/jupyter/labextensions/ipyvolume/static/58.5dd767d4301576cee659.js`

 * *Files identical despite different names*

### Comparing `ipyvolume-0.6.2/share/jupyter/labextensions/ipyvolume/static/64.e6b27f39dcb5e033dca2.js` & `ipyvolume-0.6.3/share/jupyter/labextensions/ipyvolume/static/64.e6b27f39dcb5e033dca2.js`

 * *Files identical despite different names*

### Comparing `ipyvolume-0.6.2/share/jupyter/labextensions/ipyvolume/static/861.845bccd8cacebe4b0886.js` & `ipyvolume-0.6.3/share/jupyter/labextensions/ipyvolume/static/861.845bccd8cacebe4b0886.js`

 * *Files identical despite different names*

### Comparing `ipyvolume-0.6.2/share/jupyter/labextensions/ipyvolume/static/943.4d08ec41a49be026ca9f.js` & `ipyvolume-0.6.3/share/jupyter/labextensions/ipyvolume/static/943.4d08ec41a49be026ca9f.js`

 * *Files identical despite different names*

### Comparing `ipyvolume-0.6.2/share/jupyter/labextensions/ipyvolume/static/remoteEntry.f52c61a5425bd83d7ff9.js` & `ipyvolume-0.6.3/share/jupyter/labextensions/ipyvolume/static/remoteEntry.6b98305c8298015194ea.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -45,28 +45,28 @@
         58: "5dd767d4301576cee659",
         64: "e6b27f39dcb5e033dca2",
         212: "b0149a14735c9b14c049",
         261: "a9c9630b28934bcbf1c3",
         466: "df53a5241872f78b6b60",
         486: "59ac5542d87a8f7709e9",
         501: "54c2baeab80ecb56ca08",
-        568: "5edc20b9bebeb1dddffc",
+        568: "df354347cf6898d012c4",
         577: "ef610ec4539ffe9cddc1",
         861: "845bccd8cacebe4b0886",
         936: "34edf02ccabe0274c00d",
         943: "4d08ec41a49be026ca9f"
     } [e] + ".js?v=" + {
         58: "5dd767d4301576cee659",
         64: "e6b27f39dcb5e033dca2",
         212: "b0149a14735c9b14c049",
         261: "a9c9630b28934bcbf1c3",
         466: "df53a5241872f78b6b60",
         486: "59ac5542d87a8f7709e9",
         501: "54c2baeab80ecb56ca08",
-        568: "5edc20b9bebeb1dddffc",
+        568: "df354347cf6898d012c4",
         577: "ef610ec4539ffe9cddc1",
         861: "845bccd8cacebe4b0886",
         936: "34edf02ccabe0274c00d",
         943: "4d08ec41a49be026ca9f"
     } [e], w.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
@@ -124,15 +124,15 @@
                             from: d,
                             eager: !!a
                         })
                     },
                     c = [];
                 switch (t) {
                     case "default":
-                        i("d3", "5.12.0", (() => w.e(64).then((() => () => w(64))))), i("ipyvolume", "0.6.2", (() => w.e(568).then((() => () => w(1568))))), i("is-typedarray", "1.0.0", (() => w.e(501).then((() => () => w(4501))))), i("lodash", "4.17.15", (() => w.e(486).then((() => () => w(6486))))), i("mustache", "2.3.2", (() => w.e(466).then((() => () => w(466))))), i("ndarray-pack", "1.2.1", (() => Promise.all([w.e(943), w.e(936)]).then((() => () => w(1943))))), i("ndarray", "1.0.18", (() => w.e(861).then((() => () => w(2861))))), i("screenfull", "3.3.3", (() => w.e(577).then((() => () => w(577))))), i("three-text2d", "0.4.1", (() => w.e(58).then((() => () => w(5058))))), i("three", "0.97.0", (() => w.e(212).then((() => () => w(2212)))))
+                        i("d3", "5.12.0", (() => w.e(64).then((() => () => w(64))))), i("ipyvolume", "0.6.3", (() => w.e(568).then((() => () => w(1568))))), i("is-typedarray", "1.0.0", (() => w.e(501).then((() => () => w(4501))))), i("lodash", "4.17.15", (() => w.e(486).then((() => () => w(6486))))), i("mustache", "2.3.2", (() => w.e(466).then((() => () => w(466))))), i("ndarray-pack", "1.2.1", (() => Promise.all([w.e(943), w.e(936)]).then((() => () => w(1943))))), i("ndarray", "1.0.18", (() => w.e(861).then((() => () => w(2861))))), i("screenfull", "3.3.3", (() => w.e(577).then((() => () => w(577))))), i("three-text2d", "0.4.1", (() => w.e(58).then((() => () => w(5058))))), i("three", "0.97.0", (() => w.e(212).then((() => () => w(2212)))))
                 }
                 return e[t] = c.length ? Promise.all(c).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
```

### Comparing `ipyvolume-0.6.2/share/jupyter/nbextensions/ipyvolume/extension.js` & `ipyvolume-0.6.3/share/jupyter/nbextensions/ipyvolume/extension.js`

 * *Files identical despite different names*

### Comparing `ipyvolume-0.6.2/share/jupyter/nbextensions/ipyvolume/index.js` & `ipyvolume-0.6.3/share/jupyter/nbextensions/ipyvolume/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -19808,15 +19808,15 @@
             return e instanceof Int8Array || e instanceof Int16Array || e instanceof Int32Array || e instanceof Uint8Array || e instanceof Uint8ClampedArray || e instanceof Uint16Array || e instanceof Uint32Array || e instanceof Float32Array || e instanceof Float64Array
         }
 
         function a(e) {
             return r[n.call(e)]
         }
     }, function(e) {
-        e.exports = JSON.parse('{"name":"ipyvolume","version":"0.6.2","description":"IPython widget for rendering 3d volumes","author":"Maarten A. Breddels","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/maartenbreddels/ipyvolume.git"},"keywords":["jupyter","widgets","ipython","ipywidgets"],"license":"MIT","scripts":{"install-test":"npm install && karma start --single-run","test":"karma start --single-run","build":"npm run build:lib && npm run build:labextension && webpack --mode=production","build:lib":"tsc --project .","build:labextension":"jupyter labextension build .","prepare":"npm run build","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w --project .","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch .","watch:dev":"npm-run-all -p watch:lib watch:nbextension"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../share/jupyter/labextensions/ipyvolume","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"devDependencies":{"@jupyterlab/builder":"^3.0.0","@types/chai":"^4.1.4","@types/d3":"^5.7.2","@types/expect.js":"^0.3.29","@types/mocha":"^2.2.48","@types/node":"^12.0.2","@types/requirejs":"^2.1.31","@types/three":"^0.93.4","bqplot":"^0.5.0","chai":"^4.1.2","eslint":"^5.13.0","eslint-config-standard":"^12.0.0","eslint-plugin-import":"^2.16.0","eslint-plugin-node":"^8.0.1","eslint-plugin-promise":"^4.0.1","eslint-plugin-standard":"^4.0.0","json-loader":"^0.5.4","jupyter-threejs":"^2.3.0","karma":"^4.0.0","karma-chai":"^0.1.0","karma-chrome-launcher":"^2.0.0","karma-mocha":"^1.3.0","karma-mocha-reporter":"^2.2.5","karma-sinon":"^1.0.5","karma-sourcemap-loader":"^0.3.7","karma-webpack":"^3.0.5","mocha":"^3.5.3","npm-run-all":"^4.1.3","raw-loader":"~3.0.0","sinon":"^2.4.1","sinon-chai":"^2.11.0","source-map-loader":"^0.2.4","typescript":"^3.5.2","url-loader":"^0.5.7","webpack":"^4.29.1","webpack-cli":"^3.2.3"},"dependencies":{"@jupyter-widgets/base":"^1 || ^2.0.2 || ^3 || ^4 || ^5 || ^6","@jupyter-widgets/controls":"^1 || ^2","css-loader":"^0.28.4","d3":"^5.7.0","gl-matrix":"^2.0.0","is-typedarray":"~1.0.0","jquery":"^3.1.1","jslink":"^1.1.3","lodash":"^4.17.15","mustache":"^2.3.1","ndarray":"~1.0.18","ndarray-pack":"^1.2.1","screenfull":"^3.3.1","style-loader":"^0.18.2","three":"^0.97.0","three-text2d":"~0.4.1","tslint":"^5.20.0","underscore":"^1.8.3","webrtc-adapter":"^4.2.2"},"files":["dist/","css/","src/","lib/*.js","lib/three/*.js","data/","glsl/"]}')
+        e.exports = JSON.parse('{"name":"ipyvolume","version":"0.6.3","description":"IPython widget for rendering 3d volumes","author":"Maarten A. Breddels","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/maartenbreddels/ipyvolume.git"},"keywords":["jupyter","widgets","ipython","ipywidgets"],"license":"MIT","scripts":{"install-test":"npm install && karma start --single-run","test":"karma start --single-run","build":"npm run build:lib && npm run build:labextension && webpack --mode=production","build:lib":"tsc --project .","build:labextension":"jupyter labextension build .","prepare":"npm run build","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w --project .","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch .","watch:dev":"npm-run-all -p watch:lib watch:nbextension"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../share/jupyter/labextensions/ipyvolume","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"devDependencies":{"@jupyterlab/builder":"^3.0.0","@types/chai":"^4.1.4","@types/d3":"^5.7.2","@types/expect.js":"^0.3.29","@types/mocha":"^2.2.48","@types/node":"^12.0.2","@types/requirejs":"^2.1.31","@types/three":"^0.93.4","bqplot":"^0.5.0","chai":"^4.1.2","eslint":"^5.13.0","eslint-config-standard":"^12.0.0","eslint-plugin-import":"^2.16.0","eslint-plugin-node":"^8.0.1","eslint-plugin-promise":"^4.0.1","eslint-plugin-standard":"^4.0.0","json-loader":"^0.5.4","jupyter-threejs":"^2.3.0","karma":"^4.0.0","karma-chai":"^0.1.0","karma-chrome-launcher":"^2.0.0","karma-mocha":"^1.3.0","karma-mocha-reporter":"^2.2.5","karma-sinon":"^1.0.5","karma-sourcemap-loader":"^0.3.7","karma-webpack":"^3.0.5","mocha":"^3.5.3","npm-run-all":"^4.1.3","raw-loader":"~3.0.0","sinon":"^2.4.1","sinon-chai":"^2.11.0","source-map-loader":"^0.2.4","typescript":"^3.5.2","url-loader":"^0.5.7","webpack":"^4.29.1","webpack-cli":"^3.2.3"},"dependencies":{"@jupyter-widgets/base":"^1 || ^2.0.2 || ^3 || ^4 || ^5 || ^6","@jupyter-widgets/controls":"^1 || ^2","css-loader":"^0.28.4","d3":"^5.7.0","gl-matrix":"^2.0.0","is-typedarray":"~1.0.0","jquery":"^3.1.1","jslink":"^1.1.3","lodash":"^4.17.15","mustache":"^2.3.1","ndarray":"~1.0.18","ndarray-pack":"^1.2.1","screenfull":"^3.3.1","style-loader":"^0.18.2","three":"^0.97.0","three-text2d":"~0.4.1","tslint":"^5.20.0","underscore":"^1.8.3","webrtc-adapter":"^4.2.2"},"files":["dist/","css/","src/","lib/*.js","lib/three/*.js","data/","glsl/"]}')
     }, function(e, t, n) {
         e.exports = n(36)({
             args: ["array", "scalar", "index"],
             pre: {
                 body: "{}",
                 args: [],
                 thisVars: [],
```

### Comparing `ipyvolume-0.6.2/share/jupyter/nbextensions/ipyvolume/three.js` & `ipyvolume-0.6.3/share/jupyter/nbextensions/ipyvolume/three.js`

 * *Files identical despite different names*

