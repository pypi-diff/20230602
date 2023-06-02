# Comparing `tmp/st-clickable-img-gallery-0.0.4.tar.gz` & `tmp/st-clickable-img-gallery-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/st-clickable-img-gallery-0.0.4.tar", last modified: Thu May 25 10:55:54 2023, max compression
+gzip compressed data, was "dist/st-clickable-img-gallery-0.0.5.tar", last modified: Fri Jun  2 03:59:22 2023, max compression
```

## Comparing `st-clickable-img-gallery-0.0.4.tar` & `st-clickable-img-gallery-0.0.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 CTI        (502) staff       (20)        0 2023-05-25 10:55:54.910577 st-clickable-img-gallery-0.0.4/
--rw-r--r--   0 CTI        (502) staff       (20)     1063 2023-05-25 08:36:25.000000 st-clickable-img-gallery-0.0.4/LICENSE
--rw-r--r--   0 CTI        (502) staff       (20)       60 2023-05-25 10:12:12.000000 st-clickable-img-gallery-0.0.4/MANIFEST.in
--rw-r--r--   0 CTI        (502) staff       (20)      346 2023-05-25 10:55:54.910016 st-clickable-img-gallery-0.0.4/PKG-INFO
--rw-r--r--   0 CTI        (502) staff       (20)     2750 2023-05-25 10:12:12.000000 st-clickable-img-gallery-0.0.4/README.md
--rw-r--r--   0 CTI        (502) staff       (20)       38 2023-05-25 10:55:54.910745 st-clickable-img-gallery-0.0.4/setup.cfg
--rw-r--r--   0 CTI        (502) staff       (20)      717 2023-05-25 10:55:04.000000 st-clickable-img-gallery-0.0.4/setup.py
-drwxr-xr-x   0 CTI        (502) staff       (20)        0 2023-05-25 10:55:54.897831 st-clickable-img-gallery-0.0.4/st_clickable_img_gallery/
--rw-r--r--   0 CTI        (502) staff       (20)     2291 2023-05-25 10:53:27.000000 st-clickable-img-gallery-0.0.4/st_clickable_img_gallery/__init__.py
-drwxr-xr-x   0 CTI        (502) staff       (20)        0 2023-05-25 10:55:54.894816 st-clickable-img-gallery-0.0.4/st_clickable_img_gallery/frontend/
-drwxr-xr-x   0 CTI        (502) staff       (20)        0 2023-05-25 10:55:54.902797 st-clickable-img-gallery-0.0.4/st_clickable_img_gallery/frontend/build/
--rw-r--r--   0 CTI        (502) staff       (20)      859 2023-05-25 10:53:56.000000 st-clickable-img-gallery-0.0.4/st_clickable_img_gallery/frontend/build/asset-manifest.json
--rw-r--r--   0 CTI        (502) staff       (20)   197459 2023-05-25 10:53:51.000000 st-clickable-img-gallery-0.0.4/st_clickable_img_gallery/frontend/build/bootstrap.min.css
--rw-r--r--   0 CTI        (502) staff       (20)     2080 2023-05-25 10:53:56.000000 st-clickable-img-gallery-0.0.4/st_clickable_img_gallery/frontend/build/index.html
--rw-r--r--   0 CTI        (502) staff       (20)      564 2023-05-25 10:53:56.000000 st-clickable-img-gallery-0.0.4/st_clickable_img_gallery/frontend/build/precache-manifest.65360b4608e046d15fda00ebfec33802.js
--rw-r--r--   0 CTI        (502) staff       (20)     1183 2023-05-25 10:53:56.000000 st-clickable-img-gallery-0.0.4/st_clickable_img_gallery/frontend/build/service-worker.js
-drwxr-xr-x   0 CTI        (502) staff       (20)        0 2023-05-25 10:55:54.895467 st-clickable-img-gallery-0.0.4/st_clickable_img_gallery/frontend/build/static/
-drwxr-xr-x   0 CTI        (502) staff       (20)        0 2023-05-25 10:55:54.909413 st-clickable-img-gallery-0.0.4/st_clickable_img_gallery/frontend/build/static/js/
--rw-r--r--   0 CTI        (502) staff       (20)   334667 2023-05-25 10:53:56.000000 st-clickable-img-gallery-0.0.4/st_clickable_img_gallery/frontend/build/static/js/2.60f28383.chunk.js
--rw-r--r--   0 CTI        (502) staff       (20)     1158 2023-05-25 10:53:56.000000 st-clickable-img-gallery-0.0.4/st_clickable_img_gallery/frontend/build/static/js/2.60f28383.chunk.js.LICENSE.txt
--rw-r--r--   0 CTI        (502) staff       (20)  1283638 2023-05-25 10:53:56.000000 st-clickable-img-gallery-0.0.4/st_clickable_img_gallery/frontend/build/static/js/2.60f28383.chunk.js.map
--rw-r--r--   0 CTI        (502) staff       (20)     1213 2023-05-25 10:53:56.000000 st-clickable-img-gallery-0.0.4/st_clickable_img_gallery/frontend/build/static/js/main.e9a8ee4d.chunk.js
--rw-r--r--   0 CTI        (502) staff       (20)     4616 2023-05-25 10:53:56.000000 st-clickable-img-gallery-0.0.4/st_clickable_img_gallery/frontend/build/static/js/main.e9a8ee4d.chunk.js.map
--rw-r--r--   0 CTI        (502) staff       (20)     1598 2023-05-25 10:53:56.000000 st-clickable-img-gallery-0.0.4/st_clickable_img_gallery/frontend/build/static/js/runtime-main.11ec9aca.js
--rw-r--r--   0 CTI        (502) staff       (20)     8317 2023-05-25 10:53:56.000000 st-clickable-img-gallery-0.0.4/st_clickable_img_gallery/frontend/build/static/js/runtime-main.11ec9aca.js.map
-drwxr-xr-x   0 CTI        (502) staff       (20)        0 2023-05-25 10:55:54.900208 st-clickable-img-gallery-0.0.4/st_clickable_img_gallery.egg-info/
--rw-r--r--   0 CTI        (502) staff       (20)      346 2023-05-25 10:55:54.000000 st-clickable-img-gallery-0.0.4/st_clickable_img_gallery.egg-info/PKG-INFO
--rw-r--r--   0 CTI        (502) staff       (20)     1165 2023-05-25 10:55:54.000000 st-clickable-img-gallery-0.0.4/st_clickable_img_gallery.egg-info/SOURCES.txt
--rw-r--r--   0 CTI        (502) staff       (20)        1 2023-05-25 10:55:54.000000 st-clickable-img-gallery-0.0.4/st_clickable_img_gallery.egg-info/dependency_links.txt
--rw-r--r--   0 CTI        (502) staff       (20)       16 2023-05-25 10:55:54.000000 st-clickable-img-gallery-0.0.4/st_clickable_img_gallery.egg-info/requires.txt
--rw-r--r--   0 CTI        (502) staff       (20)       25 2023-05-25 10:55:54.000000 st-clickable-img-gallery-0.0.4/st_clickable_img_gallery.egg-info/top_level.txt
+drwxr-xr-x   0 CTI        (502) staff       (20)        0 2023-06-02 03:59:22.984858 st-clickable-img-gallery-0.0.5/
+-rw-r--r--   0 CTI        (502) staff       (20)     1063 2023-05-25 08:36:25.000000 st-clickable-img-gallery-0.0.5/LICENSE
+-rw-r--r--   0 CTI        (502) staff       (20)       60 2023-05-25 10:12:12.000000 st-clickable-img-gallery-0.0.5/MANIFEST.in
+-rw-r--r--   0 CTI        (502) staff       (20)      378 2023-06-02 03:59:22.984524 st-clickable-img-gallery-0.0.5/PKG-INFO
+-rw-r--r--   0 CTI        (502) staff       (20)     2750 2023-05-25 10:12:12.000000 st-clickable-img-gallery-0.0.5/README.md
+-rw-r--r--   0 CTI        (502) staff       (20)       38 2023-06-02 03:59:22.984955 st-clickable-img-gallery-0.0.5/setup.cfg
+-rw-r--r--   0 CTI        (502) staff       (20)      717 2023-06-02 03:57:35.000000 st-clickable-img-gallery-0.0.5/setup.py
+drwxr-xr-x   0 CTI        (502) staff       (20)        0 2023-06-02 03:59:22.959164 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/
+-rw-r--r--   0 CTI        (502) staff       (20)     2811 2023-06-02 03:57:16.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/__init__.py
+drwxr-xr-x   0 CTI        (502) staff       (20)        0 2023-06-02 03:59:22.956468 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/
+drwxr-xr-x   0 CTI        (502) staff       (20)        0 2023-06-02 03:59:22.966979 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/
+-rw-r--r--   0 CTI        (502) staff       (20)      859 2023-06-02 03:58:48.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/asset-manifest.json
+-rw-r--r--   0 CTI        (502) staff       (20)   197459 2023-06-02 03:58:44.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/bootstrap.min.css
+-rw-r--r--   0 CTI        (502) staff       (20)     2080 2023-06-02 03:58:48.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/index.html
+-rw-r--r--   0 CTI        (502) staff       (20)      564 2023-06-02 03:58:48.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/precache-manifest.0a644e34e8c91feca024ba003e7a6372.js
+-rw-r--r--   0 CTI        (502) staff       (20)     1183 2023-06-02 03:58:48.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/service-worker.js
+drwxr-xr-x   0 CTI        (502) staff       (20)        0 2023-06-02 03:59:22.956802 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/static/
+drwxr-xr-x   0 CTI        (502) staff       (20)        0 2023-06-02 03:59:22.984068 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/static/js/
+-rw-r--r--   0 CTI        (502) staff       (20)   334667 2023-06-02 03:58:48.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/static/js/2.60f28383.chunk.js
+-rw-r--r--   0 CTI        (502) staff       (20)     1158 2023-06-02 03:58:48.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/static/js/2.60f28383.chunk.js.LICENSE.txt
+-rw-r--r--   0 CTI        (502) staff       (20)  1283638 2023-06-02 03:58:48.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/static/js/2.60f28383.chunk.js.map
+-rw-r--r--   0 CTI        (502) staff       (20)     1180 2023-06-02 03:58:48.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/static/js/main.53f69541.chunk.js
+-rw-r--r--   0 CTI        (502) staff       (20)     6071 2023-06-02 03:58:48.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/static/js/main.53f69541.chunk.js.map
+-rw-r--r--   0 CTI        (502) staff       (20)     1598 2023-06-02 03:58:48.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/static/js/runtime-main.11ec9aca.js
+-rw-r--r--   0 CTI        (502) staff       (20)     8317 2023-06-02 03:58:48.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/static/js/runtime-main.11ec9aca.js.map
+drwxr-xr-x   0 CTI        (502) staff       (20)        0 2023-06-02 03:59:22.964066 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery.egg-info/
+-rw-r--r--   0 CTI        (502) staff       (20)      378 2023-06-02 03:59:22.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery.egg-info/PKG-INFO
+-rw-r--r--   0 CTI        (502) staff       (20)     1165 2023-06-02 03:59:22.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery.egg-info/SOURCES.txt
+-rw-r--r--   0 CTI        (502) staff       (20)        1 2023-06-02 03:59:22.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery.egg-info/dependency_links.txt
+-rw-r--r--   0 CTI        (502) staff       (20)       16 2023-06-02 03:59:22.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery.egg-info/requires.txt
+-rw-r--r--   0 CTI        (502) staff       (20)       25 2023-06-02 03:59:22.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery.egg-info/top_level.txt
```

### Comparing `st-clickable-img-gallery-0.0.4/LICENSE` & `st-clickable-img-gallery-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `st-clickable-img-gallery-0.0.4/README.md` & `st-clickable-img-gallery-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `st-clickable-img-gallery-0.0.4/setup.py` & `st-clickable-img-gallery-0.0.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="st-clickable-img-gallery",
-    version="0.0.4",
+    version="0.0.5",
     author="",
     author_email="",
     description="A Streamlit component to display clickable images",
     long_description="A Streamlit component to display images and retrieve the indices of the images that were clicked on",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `st-clickable-img-gallery-0.0.4/st_clickable_img_gallery/__init__.py` & `st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,25 +11,28 @@
     parent_dir = os.path.dirname(os.path.abspath(__file__))
     build_dir = os.path.join(parent_dir, "frontend/build")
     _component_func = components.declare_component(
         "st_clickable_img_gallery", path=build_dir
     )
 
 
-def clickable_images(paths, titles=[], div_style={}, img_style={}, key=None):
+def clickable_images(paths, titles=[], links=[], div_style={}, img_style={}, key=None):
     """Display one or several images that can be clicked on".
 
     Parameters
     ----------
     paths: list
         The list of URLS of the images
     
     titles: list
         The (optional) titles of the images
-    
+
+    links: list
+        The (optional) links for the clicks
+
     div_style: dict
         A dict with the CSS property/value pairs for the div container
 
     img_style: dict
         A dict with the CSS property/value pairs for the images
 
     key: str or None
@@ -42,14 +45,15 @@
     int
         The index of the last image clicked on (or -1 before any click)
 
     """
     component_value = _component_func(
         paths=paths,
         titles=titles,
+        links=links,
         div_style=div_style,
         img_style=img_style,
         key=key,
         default=-1,
     )
 
     return component_value
@@ -62,12 +66,18 @@
             "https://images.unsplash.com/photo-1565130838609-c3a86655db61?w=700",
             "https://images.unsplash.com/photo-1565372195458-9de0b320ef04?w=700",
             "https://images.unsplash.com/photo-1582550945154-66ea8fff25e1?w=700",
             "https://images.unsplash.com/photo-1591797442444-039f23ddcc14?w=700",
             "https://images.unsplash.com/photo-1518727818782-ed5341dbd476?w=700",
         ],
         titles=[f"Image #{str(i)}" for i in range(5)],
+        links=["https://images.unsplash.com/photo-1565130838609-c3a86655db61?w=700",
+            "https://images.unsplash.com/photo-1565372195458-9de0b320ef04?w=700",
+            "https://images.unsplash.com/photo-1582550945154-66ea8fff25e1?w=700",
+            "https://images.unsplash.com/photo-1591797442444-039f23ddcc14?w=700",
+            "https://images.unsplash.com/photo-1518727818782-ed5341dbd476?w=700",
+                ],
         div_style={"display": "flex", "justify-content": "center", "flex-wrap": "wrap"},
         img_style={"margin": "5px", "height": "200px"},
     )
 
     st.markdown(f"Image #{clicked} clicked" if clicked > -1 else "No image clicked")
```

### Comparing `st-clickable-img-gallery-0.0.4/st_clickable_img_gallery/frontend/build/asset-manifest.json` & `st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/asset-manifest.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8068181818181819%*

 * *Differences: {"'entrypoints'": "{insert: [(2, 'static/js/main.53f69541.chunk.js')], delete: [2]}",*

 * * "'files'": "{'main.js': './static/js/main.53f69541.chunk.js', 'main.js.map': "*

 * *            "'./static/js/main.53f69541.chunk.js.map', "*

 * *            "'precache-manifest.0a644e34e8c91feca024ba003e7a6372.js': "*

 * *            "'./precache-manifest.0a644e34e8c91feca024ba003e7a6372.js', delete: "*

 * *            "['precache-manifest.65360b4608e046d15fda00ebfec33802.js']}"}*

```diff
@@ -1,18 +1,18 @@
 {
     "entrypoints": [
         "static/js/runtime-main.11ec9aca.js",
         "static/js/2.60f28383.chunk.js",
-        "static/js/main.e9a8ee4d.chunk.js"
+        "static/js/main.53f69541.chunk.js"
     ],
     "files": {
         "index.html": "./index.html",
-        "main.js": "./static/js/main.e9a8ee4d.chunk.js",
-        "main.js.map": "./static/js/main.e9a8ee4d.chunk.js.map",
-        "precache-manifest.65360b4608e046d15fda00ebfec33802.js": "./precache-manifest.65360b4608e046d15fda00ebfec33802.js",
+        "main.js": "./static/js/main.53f69541.chunk.js",
+        "main.js.map": "./static/js/main.53f69541.chunk.js.map",
+        "precache-manifest.0a644e34e8c91feca024ba003e7a6372.js": "./precache-manifest.0a644e34e8c91feca024ba003e7a6372.js",
         "runtime-main.js": "./static/js/runtime-main.11ec9aca.js",
         "runtime-main.js.map": "./static/js/runtime-main.11ec9aca.js.map",
         "service-worker.js": "./service-worker.js",
         "static/js/2.60f28383.chunk.js": "./static/js/2.60f28383.chunk.js",
         "static/js/2.60f28383.chunk.js.LICENSE.txt": "./static/js/2.60f28383.chunk.js.LICENSE.txt",
         "static/js/2.60f28383.chunk.js.map": "./static/js/2.60f28383.chunk.js.map"
     }
```

### Comparing `st-clickable-img-gallery-0.0.4/st_clickable_img_gallery/frontend/build/bootstrap.min.css` & `st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `st-clickable-img-gallery-0.0.4/st_clickable_img_gallery/frontend/build/index.html` & `st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/></head><body><noscript>You need to enable JavaScript to run this app.</noscript><script>!function(e){function t(t){for(var n,l,a=t[0],p=t[1],i=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in p)Object.prototype.hasOwnProperty.call(p,n)&&(e[n]=p[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var p=r[a];0!==o[p]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],p=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var f=p;r()}([])</script><script src="./static/js/2.60f28383.chunk.js"></script><script src="./static/js/main.e9a8ee4d.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/></head><body><noscript>You need to enable JavaScript to run this app.</noscript><script>!function(e){function t(t){for(var n,l,a=t[0],p=t[1],i=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in p)Object.prototype.hasOwnProperty.call(p,n)&&(e[n]=p[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var p=r[a];0!==o[p]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],p=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var f=p;r()}([])</script><script src="./static/js/2.60f28383.chunk.js"></script><script src="./static/js/main.53f69541.chunk.js"></script></body></html>
```

### Comparing `st-clickable-img-gallery-0.0.4/st_clickable_img_gallery/frontend/build/service-worker.js` & `st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/service-worker.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -10,15 +10,15 @@
  * and re-run your build process.
  * See https://goo.gl/2aRDsh
  */
 
 importScripts("https://storage.googleapis.com/workbox-cdn/releases/4.3.1/workbox-sw.js");
 
 importScripts(
-    "./precache-manifest.65360b4608e046d15fda00ebfec33802.js"
+    "./precache-manifest.0a644e34e8c91feca024ba003e7a6372.js"
 );
 
 self.addEventListener('message', (event) => {
     if (event.data && event.data.type === 'SKIP_WAITING') {
         self.skipWaiting();
     }
 });
```

### Comparing `st-clickable-img-gallery-0.0.4/st_clickable_img_gallery/frontend/build/static/js/2.60f28383.chunk.js` & `st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/static/js/2.60f28383.chunk.js`

 * *Files identical despite different names*

### Comparing `st-clickable-img-gallery-0.0.4/st_clickable_img_gallery/frontend/build/static/js/2.60f28383.chunk.js.LICENSE.txt` & `st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/static/js/2.60f28383.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st-clickable-img-gallery-0.0.4/st_clickable_img_gallery/frontend/build/static/js/2.60f28383.chunk.js.map` & `st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/static/js/2.60f28383.chunk.js.map`

 * *Files identical despite different names*

### Comparing `st-clickable-img-gallery-0.0.4/st_clickable_img_gallery/frontend/build/static/js/runtime-main.11ec9aca.js` & `st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/static/js/runtime-main.11ec9aca.js`

 * *Files identical despite different names*

### Comparing `st-clickable-img-gallery-0.0.4/st_clickable_img_gallery/frontend/build/static/js/runtime-main.11ec9aca.js.map` & `st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/static/js/runtime-main.11ec9aca.js.map`

 * *Files identical despite different names*

### Comparing `st-clickable-img-gallery-0.0.4/st_clickable_img_gallery.egg-info/SOURCES.txt` & `st-clickable-img-gallery-0.0.5/st_clickable_img_gallery.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 st_clickable_img_gallery.egg-info/SOURCES.txt
 st_clickable_img_gallery.egg-info/dependency_links.txt
 st_clickable_img_gallery.egg-info/requires.txt
 st_clickable_img_gallery.egg-info/top_level.txt
 st_clickable_img_gallery/frontend/build/asset-manifest.json
 st_clickable_img_gallery/frontend/build/bootstrap.min.css
 st_clickable_img_gallery/frontend/build/index.html
-st_clickable_img_gallery/frontend/build/precache-manifest.65360b4608e046d15fda00ebfec33802.js
+st_clickable_img_gallery/frontend/build/precache-manifest.0a644e34e8c91feca024ba003e7a6372.js
 st_clickable_img_gallery/frontend/build/service-worker.js
 st_clickable_img_gallery/frontend/build/static/js/2.60f28383.chunk.js
 st_clickable_img_gallery/frontend/build/static/js/2.60f28383.chunk.js.LICENSE.txt
 st_clickable_img_gallery/frontend/build/static/js/2.60f28383.chunk.js.map
-st_clickable_img_gallery/frontend/build/static/js/main.e9a8ee4d.chunk.js
-st_clickable_img_gallery/frontend/build/static/js/main.e9a8ee4d.chunk.js.map
+st_clickable_img_gallery/frontend/build/static/js/main.53f69541.chunk.js
+st_clickable_img_gallery/frontend/build/static/js/main.53f69541.chunk.js.map
 st_clickable_img_gallery/frontend/build/static/js/runtime-main.11ec9aca.js
 st_clickable_img_gallery/frontend/build/static/js/runtime-main.11ec9aca.js.map
```

