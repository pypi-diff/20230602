# Comparing `tmp/st-clickable-img-gallery-0.0.5.tar.gz` & `tmp/st-clickable-img-gallery-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/st-clickable-img-gallery-0.0.5.tar", last modified: Fri Jun  2 03:59:22 2023, max compression
+gzip compressed data, was "dist/st-clickable-img-gallery-0.0.6.tar", last modified: Fri Jun  2 04:36:27 2023, max compression
```

## Comparing `st-clickable-img-gallery-0.0.5.tar` & `st-clickable-img-gallery-0.0.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 CTI        (502) staff       (20)        0 2023-06-02 03:59:22.984858 st-clickable-img-gallery-0.0.5/
--rw-r--r--   0 CTI        (502) staff       (20)     1063 2023-05-25 08:36:25.000000 st-clickable-img-gallery-0.0.5/LICENSE
--rw-r--r--   0 CTI        (502) staff       (20)       60 2023-05-25 10:12:12.000000 st-clickable-img-gallery-0.0.5/MANIFEST.in
--rw-r--r--   0 CTI        (502) staff       (20)      378 2023-06-02 03:59:22.984524 st-clickable-img-gallery-0.0.5/PKG-INFO
--rw-r--r--   0 CTI        (502) staff       (20)     2750 2023-05-25 10:12:12.000000 st-clickable-img-gallery-0.0.5/README.md
--rw-r--r--   0 CTI        (502) staff       (20)       38 2023-06-02 03:59:22.984955 st-clickable-img-gallery-0.0.5/setup.cfg
--rw-r--r--   0 CTI        (502) staff       (20)      717 2023-06-02 03:57:35.000000 st-clickable-img-gallery-0.0.5/setup.py
-drwxr-xr-x   0 CTI        (502) staff       (20)        0 2023-06-02 03:59:22.959164 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/
--rw-r--r--   0 CTI        (502) staff       (20)     2811 2023-06-02 03:57:16.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/__init__.py
-drwxr-xr-x   0 CTI        (502) staff       (20)        0 2023-06-02 03:59:22.956468 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/
-drwxr-xr-x   0 CTI        (502) staff       (20)        0 2023-06-02 03:59:22.966979 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/
--rw-r--r--   0 CTI        (502) staff       (20)      859 2023-06-02 03:58:48.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/asset-manifest.json
--rw-r--r--   0 CTI        (502) staff       (20)   197459 2023-06-02 03:58:44.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/bootstrap.min.css
--rw-r--r--   0 CTI        (502) staff       (20)     2080 2023-06-02 03:58:48.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/index.html
--rw-r--r--   0 CTI        (502) staff       (20)      564 2023-06-02 03:58:48.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/precache-manifest.0a644e34e8c91feca024ba003e7a6372.js
--rw-r--r--   0 CTI        (502) staff       (20)     1183 2023-06-02 03:58:48.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/service-worker.js
-drwxr-xr-x   0 CTI        (502) staff       (20)        0 2023-06-02 03:59:22.956802 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/static/
-drwxr-xr-x   0 CTI        (502) staff       (20)        0 2023-06-02 03:59:22.984068 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/static/js/
--rw-r--r--   0 CTI        (502) staff       (20)   334667 2023-06-02 03:58:48.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/static/js/2.60f28383.chunk.js
--rw-r--r--   0 CTI        (502) staff       (20)     1158 2023-06-02 03:58:48.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/static/js/2.60f28383.chunk.js.LICENSE.txt
--rw-r--r--   0 CTI        (502) staff       (20)  1283638 2023-06-02 03:58:48.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/static/js/2.60f28383.chunk.js.map
--rw-r--r--   0 CTI        (502) staff       (20)     1180 2023-06-02 03:58:48.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/static/js/main.53f69541.chunk.js
--rw-r--r--   0 CTI        (502) staff       (20)     6071 2023-06-02 03:58:48.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/static/js/main.53f69541.chunk.js.map
--rw-r--r--   0 CTI        (502) staff       (20)     1598 2023-06-02 03:58:48.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/static/js/runtime-main.11ec9aca.js
--rw-r--r--   0 CTI        (502) staff       (20)     8317 2023-06-02 03:58:48.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/static/js/runtime-main.11ec9aca.js.map
-drwxr-xr-x   0 CTI        (502) staff       (20)        0 2023-06-02 03:59:22.964066 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery.egg-info/
--rw-r--r--   0 CTI        (502) staff       (20)      378 2023-06-02 03:59:22.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery.egg-info/PKG-INFO
--rw-r--r--   0 CTI        (502) staff       (20)     1165 2023-06-02 03:59:22.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery.egg-info/SOURCES.txt
--rw-r--r--   0 CTI        (502) staff       (20)        1 2023-06-02 03:59:22.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery.egg-info/dependency_links.txt
--rw-r--r--   0 CTI        (502) staff       (20)       16 2023-06-02 03:59:22.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery.egg-info/requires.txt
--rw-r--r--   0 CTI        (502) staff       (20)       25 2023-06-02 03:59:22.000000 st-clickable-img-gallery-0.0.5/st_clickable_img_gallery.egg-info/top_level.txt
+drwxr-xr-x   0 CTI        (502) staff       (20)        0 2023-06-02 04:36:27.794886 st-clickable-img-gallery-0.0.6/
+-rw-r--r--   0 CTI        (502) staff       (20)     1063 2023-05-25 08:36:25.000000 st-clickable-img-gallery-0.0.6/LICENSE
+-rw-r--r--   0 CTI        (502) staff       (20)       60 2023-05-25 10:12:12.000000 st-clickable-img-gallery-0.0.6/MANIFEST.in
+-rw-r--r--   0 CTI        (502) staff       (20)      378 2023-06-02 04:36:27.794536 st-clickable-img-gallery-0.0.6/PKG-INFO
+-rw-r--r--   0 CTI        (502) staff       (20)     2750 2023-05-25 10:12:12.000000 st-clickable-img-gallery-0.0.6/README.md
+-rw-r--r--   0 CTI        (502) staff       (20)       38 2023-06-02 04:36:27.795001 st-clickable-img-gallery-0.0.6/setup.cfg
+-rw-r--r--   0 CTI        (502) staff       (20)      717 2023-06-02 04:35:26.000000 st-clickable-img-gallery-0.0.6/setup.py
+drwxr-xr-x   0 CTI        (502) staff       (20)        0 2023-06-02 04:36:27.773886 st-clickable-img-gallery-0.0.6/st_clickable_img_gallery/
+-rw-r--r--   0 CTI        (502) staff       (20)     2945 2023-06-02 04:35:18.000000 st-clickable-img-gallery-0.0.6/st_clickable_img_gallery/__init__.py
+drwxr-xr-x   0 CTI        (502) staff       (20)        0 2023-06-02 04:36:27.770946 st-clickable-img-gallery-0.0.6/st_clickable_img_gallery/frontend/
+drwxr-xr-x   0 CTI        (502) staff       (20)        0 2023-06-02 04:36:27.779758 st-clickable-img-gallery-0.0.6/st_clickable_img_gallery/frontend/build/
+-rw-r--r--   0 CTI        (502) staff       (20)      859 2023-06-02 04:35:51.000000 st-clickable-img-gallery-0.0.6/st_clickable_img_gallery/frontend/build/asset-manifest.json
+-rw-r--r--   0 CTI        (502) staff       (20)   197459 2023-06-02 04:35:47.000000 st-clickable-img-gallery-0.0.6/st_clickable_img_gallery/frontend/build/bootstrap.min.css
+-rw-r--r--   0 CTI        (502) staff       (20)     2080 2023-06-02 04:35:51.000000 st-clickable-img-gallery-0.0.6/st_clickable_img_gallery/frontend/build/index.html
+-rw-r--r--   0 CTI        (502) staff       (20)      564 2023-06-02 04:35:51.000000 st-clickable-img-gallery-0.0.6/st_clickable_img_gallery/frontend/build/precache-manifest.9bad0753763e9c65a26561a891d47387.js
+-rw-r--r--   0 CTI        (502) staff       (20)     1183 2023-06-02 04:35:51.000000 st-clickable-img-gallery-0.0.6/st_clickable_img_gallery/frontend/build/service-worker.js
+drwxr-xr-x   0 CTI        (502) staff       (20)        0 2023-06-02 04:36:27.771287 st-clickable-img-gallery-0.0.6/st_clickable_img_gallery/frontend/build/static/
+drwxr-xr-x   0 CTI        (502) staff       (20)        0 2023-06-02 04:36:27.794046 st-clickable-img-gallery-0.0.6/st_clickable_img_gallery/frontend/build/static/js/
+-rw-r--r--   0 CTI        (502) staff       (20)   334667 2023-06-02 04:35:51.000000 st-clickable-img-gallery-0.0.6/st_clickable_img_gallery/frontend/build/static/js/2.60f28383.chunk.js
+-rw-r--r--   0 CTI        (502) staff       (20)     1158 2023-06-02 04:35:51.000000 st-clickable-img-gallery-0.0.6/st_clickable_img_gallery/frontend/build/static/js/2.60f28383.chunk.js.LICENSE.txt
+-rw-r--r--   0 CTI        (502) staff       (20)  1283638 2023-06-02 04:35:51.000000 st-clickable-img-gallery-0.0.6/st_clickable_img_gallery/frontend/build/static/js/2.60f28383.chunk.js.map
+-rw-r--r--   0 CTI        (502) staff       (20)     1235 2023-06-02 04:35:51.000000 st-clickable-img-gallery-0.0.6/st_clickable_img_gallery/frontend/build/static/js/main.1bc8d89a.chunk.js
+-rw-r--r--   0 CTI        (502) staff       (20)     6086 2023-06-02 04:35:51.000000 st-clickable-img-gallery-0.0.6/st_clickable_img_gallery/frontend/build/static/js/main.1bc8d89a.chunk.js.map
+-rw-r--r--   0 CTI        (502) staff       (20)     1598 2023-06-02 04:35:51.000000 st-clickable-img-gallery-0.0.6/st_clickable_img_gallery/frontend/build/static/js/runtime-main.11ec9aca.js
+-rw-r--r--   0 CTI        (502) staff       (20)     8317 2023-06-02 04:35:51.000000 st-clickable-img-gallery-0.0.6/st_clickable_img_gallery/frontend/build/static/js/runtime-main.11ec9aca.js.map
+drwxr-xr-x   0 CTI        (502) staff       (20)        0 2023-06-02 04:36:27.776470 st-clickable-img-gallery-0.0.6/st_clickable_img_gallery.egg-info/
+-rw-r--r--   0 CTI        (502) staff       (20)      378 2023-06-02 04:36:27.000000 st-clickable-img-gallery-0.0.6/st_clickable_img_gallery.egg-info/PKG-INFO
+-rw-r--r--   0 CTI        (502) staff       (20)     1165 2023-06-02 04:36:27.000000 st-clickable-img-gallery-0.0.6/st_clickable_img_gallery.egg-info/SOURCES.txt
+-rw-r--r--   0 CTI        (502) staff       (20)        1 2023-06-02 04:36:27.000000 st-clickable-img-gallery-0.0.6/st_clickable_img_gallery.egg-info/dependency_links.txt
+-rw-r--r--   0 CTI        (502) staff       (20)       16 2023-06-02 04:36:27.000000 st-clickable-img-gallery-0.0.6/st_clickable_img_gallery.egg-info/requires.txt
+-rw-r--r--   0 CTI        (502) staff       (20)       25 2023-06-02 04:36:27.000000 st-clickable-img-gallery-0.0.6/st_clickable_img_gallery.egg-info/top_level.txt
```

### Comparing `st-clickable-img-gallery-0.0.5/LICENSE` & `st-clickable-img-gallery-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `st-clickable-img-gallery-0.0.5/README.md` & `st-clickable-img-gallery-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `st-clickable-img-gallery-0.0.5/setup.py` & `st-clickable-img-gallery-0.0.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="st-clickable-img-gallery",
-    version="0.0.5",
+    version="0.0.6",
     author="",
     author_email="",
     description="A Streamlit component to display clickable images",
     long_description="A Streamlit component to display images and retrieve the indices of the images that were clicked on",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/__init__.py` & `st-clickable-img-gallery-0.0.6/st_clickable_img_gallery/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,27 +11,29 @@
     parent_dir = os.path.dirname(os.path.abspath(__file__))
     build_dir = os.path.join(parent_dir, "frontend/build")
     _component_func = components.declare_component(
         "st_clickable_img_gallery", path=build_dir
     )
 
 
-def clickable_images(paths, titles=[], links=[], div_style={}, img_style={}, key=None):
+def clickable_images(paths, titles=[], links=[], isActive=[], div_style={}, img_style={}, key=None):
     """Display one or several images that can be clicked on".
 
     Parameters
     ----------
     paths: list
         The list of URLS of the images
     
     titles: list
         The (optional) titles of the images
 
     links: list
         The (optional) links for the clicks
+    isActive:list
+        The (optional) state for the clicks
 
     div_style: dict
         A dict with the CSS property/value pairs for the div container
 
     img_style: dict
         A dict with the CSS property/value pairs for the images
 
@@ -46,14 +48,15 @@
         The index of the last image clicked on (or -1 before any click)
 
     """
     component_value = _component_func(
         paths=paths,
         titles=titles,
         links=links,
+        isActive=isActive,
         div_style=div_style,
         img_style=img_style,
         key=key,
         default=-1,
     )
 
     return component_value
@@ -72,12 +75,13 @@
         titles=[f"Image #{str(i)}" for i in range(5)],
         links=["https://images.unsplash.com/photo-1565130838609-c3a86655db61?w=700",
             "https://images.unsplash.com/photo-1565372195458-9de0b320ef04?w=700",
             "https://images.unsplash.com/photo-1582550945154-66ea8fff25e1?w=700",
             "https://images.unsplash.com/photo-1591797442444-039f23ddcc14?w=700",
             "https://images.unsplash.com/photo-1518727818782-ed5341dbd476?w=700",
                 ],
+        isActive = [1,0,0,0,0],
         div_style={"display": "flex", "justify-content": "center", "flex-wrap": "wrap"},
         img_style={"margin": "5px", "height": "200px"},
     )
 
     st.markdown(f"Image #{clicked} clicked" if clicked > -1 else "No image clicked")
```

### Comparing `st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/asset-manifest.json` & `st-clickable-img-gallery-0.0.6/st_clickable_img_gallery/frontend/build/asset-manifest.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8068181818181819%*

 * *Differences: {"'entrypoints'": "{insert: [(2, 'static/js/main.1bc8d89a.chunk.js')], delete: [2]}",*

 * * "'files'": "{'main.js': './static/js/main.1bc8d89a.chunk.js', 'main.js.map': "*

 * *            "'./static/js/main.1bc8d89a.chunk.js.map', "*

 * *            "'precache-manifest.9bad0753763e9c65a26561a891d47387.js': "*

 * *            "'./precache-manifest.9bad0753763e9c65a26561a891d47387.js', delete: "*

 * *            "['precache-manifest.0a644e34e8c91feca024ba003e7a6372.js']}"}*

```diff
@@ -1,18 +1,18 @@
 {
     "entrypoints": [
         "static/js/runtime-main.11ec9aca.js",
         "static/js/2.60f28383.chunk.js",
-        "static/js/main.53f69541.chunk.js"
+        "static/js/main.1bc8d89a.chunk.js"
     ],
     "files": {
         "index.html": "./index.html",
-        "main.js": "./static/js/main.53f69541.chunk.js",
-        "main.js.map": "./static/js/main.53f69541.chunk.js.map",
-        "precache-manifest.0a644e34e8c91feca024ba003e7a6372.js": "./precache-manifest.0a644e34e8c91feca024ba003e7a6372.js",
+        "main.js": "./static/js/main.1bc8d89a.chunk.js",
+        "main.js.map": "./static/js/main.1bc8d89a.chunk.js.map",
+        "precache-manifest.9bad0753763e9c65a26561a891d47387.js": "./precache-manifest.9bad0753763e9c65a26561a891d47387.js",
         "runtime-main.js": "./static/js/runtime-main.11ec9aca.js",
         "runtime-main.js.map": "./static/js/runtime-main.11ec9aca.js.map",
         "service-worker.js": "./service-worker.js",
         "static/js/2.60f28383.chunk.js": "./static/js/2.60f28383.chunk.js",
         "static/js/2.60f28383.chunk.js.LICENSE.txt": "./static/js/2.60f28383.chunk.js.LICENSE.txt",
         "static/js/2.60f28383.chunk.js.map": "./static/js/2.60f28383.chunk.js.map"
     }
```

### Comparing `st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/bootstrap.min.css` & `st-clickable-img-gallery-0.0.6/st_clickable_img_gallery/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/index.html` & `st-clickable-img-gallery-0.0.6/st_clickable_img_gallery/frontend/build/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/></head><body><noscript>You need to enable JavaScript to run this app.</noscript><script>!function(e){function t(t){for(var n,l,a=t[0],p=t[1],i=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in p)Object.prototype.hasOwnProperty.call(p,n)&&(e[n]=p[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var p=r[a];0!==o[p]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],p=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var f=p;r()}([])</script><script src="./static/js/2.60f28383.chunk.js"></script><script src="./static/js/main.53f69541.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/></head><body><noscript>You need to enable JavaScript to run this app.</noscript><script>!function(e){function t(t){for(var n,l,a=t[0],p=t[1],i=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in p)Object.prototype.hasOwnProperty.call(p,n)&&(e[n]=p[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var p=r[a];0!==o[p]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],p=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var f=p;r()}([])</script><script src="./static/js/2.60f28383.chunk.js"></script><script src="./static/js/main.1bc8d89a.chunk.js"></script></body></html>
```

### Comparing `st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/service-worker.js` & `st-clickable-img-gallery-0.0.6/st_clickable_img_gallery/frontend/build/service-worker.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -10,15 +10,15 @@
  * and re-run your build process.
  * See https://goo.gl/2aRDsh
  */
 
 importScripts("https://storage.googleapis.com/workbox-cdn/releases/4.3.1/workbox-sw.js");
 
 importScripts(
-    "./precache-manifest.0a644e34e8c91feca024ba003e7a6372.js"
+    "./precache-manifest.9bad0753763e9c65a26561a891d47387.js"
 );
 
 self.addEventListener('message', (event) => {
     if (event.data && event.data.type === 'SKIP_WAITING') {
         self.skipWaiting();
     }
 });
```

### Comparing `st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/static/js/2.60f28383.chunk.js` & `st-clickable-img-gallery-0.0.6/st_clickable_img_gallery/frontend/build/static/js/2.60f28383.chunk.js`

 * *Files identical despite different names*

### Comparing `st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/static/js/2.60f28383.chunk.js.LICENSE.txt` & `st-clickable-img-gallery-0.0.6/st_clickable_img_gallery/frontend/build/static/js/2.60f28383.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/static/js/2.60f28383.chunk.js.map` & `st-clickable-img-gallery-0.0.6/st_clickable_img_gallery/frontend/build/static/js/2.60f28383.chunk.js.map`

 * *Files identical despite different names*

### Comparing `st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/static/js/main.53f69541.chunk.js` & `st-clickable-img-gallery-0.0.6/st_clickable_img_gallery/frontend/build/static/js/main.1bc8d89a.chunk.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -1,36 +1,37 @@
 (this.webpackJsonpstreamlit_component_template = this.webpackJsonpstreamlit_component_template || []).push([
     [0], {
-        4: function(e, t, a) {
-            e.exports = a(5)
+        4: function(e, t, n) {
+            e.exports = n(5)
         },
-        5: function(e, t, a) {
+        5: function(e, t, n) {
             "use strict";
-            a.r(t);
-            var n = a(2);
-            n.a.events.addEventListener(n.a.RENDER_EVENT, (function(e) {
-                for (var t = e.detail, a = document.body.lastElementChild; a;) document.body.removeChild(a), a = document.body.lastElementChild;
-                var r = document.body.appendChild(document.createElement("div"));
-                for (var s in t.args.div_style) r.style[s] = t.args.div_style[s];
-                for (var l = 0, d = 0; d < t.args.paths.length; d++) {
-                    var i = r.appendChild(document.createElement("div"));
-                    i.style.border = "1px solid black", i.style.padding = "10px", i.style.cursor = "pointer";
-                    var o = i.appendChild(document.createElement("a"));
-                    o.href = t.args.links[d], o.target = "_blank";
-                    var p = o.appendChild(document.createElement("img"));
-                    for (var m in t.args.img_style) p.style[m] = t.args.img_style[m];
-                    if (p.src = t.args.paths[d], t.args.titles.length > d) {
-                        var c = i.appendChild(document.createElement("p"));
-                        c.innerText = t.args.titles[d], c.style.paddingLeft = "8px"
-                    }
-                    p.onload = function() {
-                        ++l === t.args.paths.length && n.a.setFrameHeight()
-                    }
-                }
-            })), n.a.setComponentReady()
+            n.r(t);
+            var a = n(2);
+            a.a.events.addEventListener(a.a.RENDER_EVENT, (function(e) {
+                for (var t = e.detail, n = document.body.lastElementChild; n;) document.body.removeChild(n), n = document.body.lastElementChild;
+                var s = document.body.appendChild(document.createElement("div"));
+                for (var i in t.args.div_style) s.style[i] = t.args.div_style[i];
+                for (var o = 0, l = function(e) {
+                        var n = s.appendChild(document.createElement("div"));
+                        n.style.border = "1px solid black", n.style.padding = "10px", n.style.cursor = "pointer";
+                        var i = n.appendChild(document.createElement("img"));
+                        for (var l in t.args.img_style) i.style[l] = t.args.img_style[l];
+                        if (i.src = t.args.paths[e], i.onload = function() {
+                                ++o === t.args.paths.length && a.a.setFrameHeight()
+                            }, t.args.isActive[e] ? n.onclick = function() {
+                                window.open(t.args.links[e], "_blank")
+                            } : n.onclick = function() {
+                                a.a.setComponentValue(e)
+                            }, t.args.titles.length > e) {
+                            var r = n.appendChild(document.createElement("p"));
+                            r.innerText = t.args.titles[e], r.style.paddingLeft = "8px"
+                        }
+                    }, r = 0; r < t.args.paths.length; r++) l(r)
+            })), a.a.setComponentReady()
         }
     },
     [
         [4, 1, 2]
     ]
 ]);
-//# sourceMappingURL=main.53f69541.chunk.js.map
+//# sourceMappingURL=main.1bc8d89a.chunk.js.map
```

### Comparing `st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/static/js/main.53f69541.chunk.js.map` & `st-clickable-img-gallery-0.0.6/st_clickable_img_gallery/frontend/build/static/js/main.1bc8d89a.chunk.js.map`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7641196013289037%*

 * *Differences: {"'file'": "'static/js/main.1bc8d89a.chunk.js'",*

 * * "'mappings'": "'8KAAA,kBAoHAA,IAAUC,OAAOC,iBAAiBF,IAAUG,cAvD5C,SAAkBC,GAKhB,IAJA,IAAMC,EAAQD,EAAkCE,OAG5CC,EAAQC,SAASC,KAAKC,iBACnBH,GACLC,SAASC,KAAKE,YAAYJ,GAC1BA,EAAQC,SAASC,KAAKC,iBAIxB,IAAIE,EAAMJ,SAASC,KAAKI,YAAYL,SAASM,cAAc,QAC3D,IAAK,IAAIC,KAAOV,EAAKW,KAAL,UACdJ,EAAIK,MAAMF,GAAcV,EAAKW,KAAL,UAAuBD,GAKjD,IADA,IAAIG,EAAe,EAjBiB,WAkB3BC,GACP,IAAIC,EAASR,EAAIC,YAAYL,SAASM,cAAc,QACpDM,EAAOH,MAAMI,OAAS,kBACtBD,EAAOH,MAAMK,QAAU,OACvBF,EAAOH,MAAMM,OAAS,UAEtB, […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.53f69541.chunk.js",
-    "mappings": "8KAAA,kBA6GAA,IAAUC,OAAOC,iBAAiBF,IAAUG,cAhD5C,SAAkBC,GAKhB,IAJA,IAAMC,EAAQD,EAAkCE,OAG5CC,EAAQC,SAASC,KAAKC,iBACnBH,GACLC,SAASC,KAAKE,YAAYJ,GAC1BA,EAAQC,SAASC,KAAKC,iBAIxB,IAAIE,EAAMJ,SAASC,KAAKI,YAAYL,SAASM,cAAc,QAC3D,IAAK,IAAIC,KAAOV,EAAKW,KAAL,UACdJ,EAAIK,MAAMF,GAAcV,EAAKW,KAAL,UAAuBD,GAKjD,IADA,IAAIG,EAAe,EACVC,EAAI,EAAGA,EAAId,EAAKW,KAAL,MAAmBI,OAAQD,IAAK,CAClD,IAAIE,EAAST,EAAIC,YAAYL,SAASM,cAAc,QACpDO,EAAOJ,MAAMK,OAAS,kBACtBD,EAAOJ,MAAMM,QAAU,OACvBF,EAAOJ,MAAMO,OAAS,UAEtB,IAAIC,EAAOJ,EAAOR,YAAYL,SAASM,cAAc,MACrDW,EAAKC,KAAOrB,EAAKW,KAAL,MAAmBG,GAC/BM,EAAKE,OAAS,SAEd,IAAIC,EAAMH,EAAKZ,YAAYL,SAASM,cAAc,QAClD,IAAK,IAAIC,KAAOV,EAAKW,KAAL,UACdY,EAAIX,MAAMF,GAAcV,EAAKW,KAAL,UAAuBD,GAGjD,GADAa,EAAIC,IAAMxB,EAAKW,KAAL,MAAmBG,GACzBd,EAAKW,KAAL,OAAoBI,OAASD,EAAG,CAClC,IAAIW,EAAWT,EAAOR,YAAYL,SAASM,cAAc,MACzDgB,EAASC,UAAY1B,EAAKW,KAAL,OAAoBG,GACzCW,EAASb,MAAMe,YAAc,MAG/BJ,EAAIK,OAAS,aACXf,IACqBb,EAAKW,KAAL,MAAmBI,QACtCpB,IAAUkC,sBAOlBlC,IAAUmC,sB",
+    "file": "static/js/main.1bc8d89a.chunk.js",
+    "mappings": "8KAAA,kBAoHAA,IAAUC,OAAOC,iBAAiBF,IAAUG,cAvD5C,SAAkBC,GAKhB,IAJA,IAAMC,EAAQD,EAAkCE,OAG5CC,EAAQC,SAASC,KAAKC,iBACnBH,GACLC,SAASC,KAAKE,YAAYJ,GAC1BA,EAAQC,SAASC,KAAKC,iBAIxB,IAAIE,EAAMJ,SAASC,KAAKI,YAAYL,SAASM,cAAc,QAC3D,IAAK,IAAIC,KAAOV,EAAKW,KAAL,UACdJ,EAAIK,MAAMF,GAAcV,EAAKW,KAAL,UAAuBD,GAKjD,IADA,IAAIG,EAAe,EAjBiB,WAkB3BC,GACP,IAAIC,EAASR,EAAIC,YAAYL,SAASM,cAAc,QACpDM,EAAOH,MAAMI,OAAS,kBACtBD,EAAOH,MAAMK,QAAU,OACvBF,EAAOH,MAAMM,OAAS,UAEtB,IAAIC,EAAMJ,EAAOP,YAAYL,SAASM,cAAc,QACpD,IAAK,IAAIC,KAAOV,EAAKW,KAAL,UACdQ,EAAIP,MAAMF,GAAcV,EAAKW,KAAL,UAAuBD,GAqBjD,GAnBAS,EAAIC,IAAMpB,EAAKW,KAAL,MAAmBG,GAE7BK,EAAIE,OAAS,aACXR,IACqBb,EAAKW,KAAL,MAAmBW,QACtC3B,IAAU4B,kBAIVvB,EAAKW,KAAL,SAAsBG,GACxBC,EAAOS,QAAU,WACfC,OAAOC,KAAK1B,EAAKW,KAAL,MAAmBG,GAAI,WAGrCC,EAAOS,QAAU,WACf7B,IAAUgC,kBAAkBb,IAI5Bd,EAAKW,KAAL,OAAoBW,OAASR,EAAG,CAClC,IAAIc,EAAWb,EAAOP,YAAYL,SAASM,cAAc,MACzDmB,EAASC,UAAY7B,EAAKW,KAAL,OAAoBG,GACzCc,EAAShB,MAAMkB,YAAc,QAhCxBhB,EAAI,EAAGA,EAAId,EAAKW,KAAL,MAAmBW,OAAQR,IAAM,EAA5CA,MAsCXnB,IAAUoC,sB",
     "names": [
         "Streamlit",
         "events",
         "addEventListener",
         "RENDER_EVENT",
         "event",
         "data",
@@ -18,33 +18,34 @@
         "appendChild",
         "createElement",
         "key",
         "args",
         "style",
         "imagesLoaded",
         "i",
-        "length",
         "imgDiv",
         "border",
         "padding",
         "cursor",
-        "link",
-        "href",
-        "target",
         "img",
         "src",
+        "onload",
+        "length",
+        "setFrameHeight",
+        "onclick",
+        "window",
+        "open",
+        "setComponentValue",
         "imgTitle",
         "innerText",
         "paddingLeft",
-        "onload",
-        "setFrameHeight",
         "setComponentReady"
     ],
     "sourceRoot": "",
     "sources": [
         "index.tsx"
     ],
     "sourcesContent": [
-        "// import { Streamlit, RenderData } from \"streamlit-component-lib\"\n\n// function onRender(event: Event): void {\n//   const data = (event as CustomEvent<RenderData>).detail\n\n//   // Remove existing content\n//   let child = document.body.lastElementChild;\n//   if (child) {\n//     document.body.removeChild(child)\n//   }\n\n//   // Add and style the image container\n//   let div = document.body.appendChild(document.createElement(\"div\"))\n//   for (let key in data.args[\"div_style\"]) {\n//     div.style[key as any] = data.args[\"div_style\"][key]\n//   }\n\n//   // Add and style all images\n//   let imagesLoaded = 0\n//   for (let i = 0; i < data.args[\"paths\"].length; i++) {\n//     let imgDiv = div.appendChild(document.createElement(\"div\")) // Create a new div for each image and its title\n//     imgDiv.style.border = \"1px solid black\"; // Add a border to the div\n//     imgDiv.style.padding = \"10px\"; // Add some padding to the div\n//     imgDiv.style.cursor = \"pointer\";\n//     imgDiv.onclick = function (): void { // Move the onclick event to the div\n//       Streamlit.setComponentValue(i)\n//     }\n//     imgDiv.onmouseover = function (): void { // Add a mouseover event to darken the image\n//       img.style.opacity = \"0.7\";\n//     }\n//     imgDiv.onmouseout = function (): void { // Add a mouseout event to lighten the image\n//       img.style.opacity = \"1.0\";\n//     }\n//     let img = imgDiv.appendChild(document.createElement(\"img\"))\n//     for (let key in data.args[\"img_style\"]) {\n//       img.style[key as any] = data.args[\"img_style\"][key]\n//     }\n//     img.src = data.args[\"paths\"][i]\n//     if (data.args[\"titles\"].length > i) {\n//       let imgTitle = imgDiv.appendChild(document.createElement(\"p\")) // Create a new p element for the title\n//       imgTitle.innerText = data.args[\"titles\"][i] // Set the innerText of the p element to the title\n//       imgTitle.style.paddingLeft = \"8px\"\n//     }\n//     // img.onclick = function (): void {\n//     //   Streamlit.setComponentValue(i)\n//     // }\n//     // eslint-disable-next-line\n//     img.onload = function (): void {\n//       imagesLoaded++\n//       if (imagesLoaded === data.args[\"paths\"].length) {\n//         Streamlit.setFrameHeight()\n//       }\n//     }\n//   }\n// }\n\n// Streamlit.events.addEventListener(Streamlit.RENDER_EVENT, onRender)\n// Streamlit.setComponentReady()\n\nimport { Streamlit, RenderData } from \"streamlit-component-lib\"\n\nfunction onRender(event: Event): void {\n  const data = (event as CustomEvent<RenderData>).detail\n\n  // Remove existing content\n  let child = document.body.lastElementChild;\n  while (child) {\n    document.body.removeChild(child);\n    child = document.body.lastElementChild;\n  }\n\n  // Add and style the image container\n  let div = document.body.appendChild(document.createElement(\"div\"))\n  for (let key in data.args[\"div_style\"]) {\n    div.style[key as any] = data.args[\"div_style\"][key]\n  }\n\n  // Add and style all images\n  let imagesLoaded = 0\n  for (let i = 0; i < data.args[\"paths\"].length; i++) {\n    let imgDiv = div.appendChild(document.createElement(\"div\")) // Create a new div for each image and its title\n    imgDiv.style.border = \"1px solid black\"; // Add a border to the div\n    imgDiv.style.padding = \"10px\"; // Add some padding to the div\n    imgDiv.style.cursor = \"pointer\";\n\n    let link = imgDiv.appendChild(document.createElement(\"a\")) // Create a new link element\n    link.href = data.args[\"links\"][i] // Set the href to the link from the \"links\" array\n    link.target = \"_blank\" // Open the link in a new tab\n\n    let img = link.appendChild(document.createElement(\"img\")) // Append the img element to the link instead of the div\n    for (let key in data.args[\"img_style\"]) {\n      img.style[key as any] = data.args[\"img_style\"][key]\n    }\n    img.src = data.args[\"paths\"][i]\n    if (data.args[\"titles\"].length > i) {\n      let imgTitle = imgDiv.appendChild(document.createElement(\"p\")) // Create a new p element for the title\n      imgTitle.innerText = data.args[\"titles\"][i] // Set the innerText of the p element to the title\n      imgTitle.style.paddingLeft = \"8px\"\n    }\n    // eslint-disable-next-line\n    img.onload = function (): void {\n      imagesLoaded++\n      if (imagesLoaded === data.args[\"paths\"].length) {\n        Streamlit.setFrameHeight()\n      }\n    }\n  }\n}\n\nStreamlit.events.addEventListener(Streamlit.RENDER_EVENT, onRender)\nStreamlit.setComponentReady()\n\n"
+        "// import { Streamlit, RenderData } from \"streamlit-component-lib\"\n\n// function onRender(event: Event): void {\n//   const data = (event as CustomEvent<RenderData>).detail\n\n//   // Remove existing content\n//   let child = document.body.lastElementChild;\n//   if (child) {\n//     document.body.removeChild(child)\n//   }\n\n//   // Add and style the image container\n//   let div = document.body.appendChild(document.createElement(\"div\"))\n//   for (let key in data.args[\"div_style\"]) {\n//     div.style[key as any] = data.args[\"div_style\"][key]\n//   }\n\n//   // Add and style all images\n//   let imagesLoaded = 0\n//   for (let i = 0; i < data.args[\"paths\"].length; i++) {\n//     let imgDiv = div.appendChild(document.createElement(\"div\")) // Create a new div for each image and its title\n//     imgDiv.style.border = \"1px solid black\"; // Add a border to the div\n//     imgDiv.style.padding = \"10px\"; // Add some padding to the div\n//     imgDiv.style.cursor = \"pointer\";\n//     imgDiv.onclick = function (): void { // Move the onclick event to the div\n//       Streamlit.setComponentValue(i)\n//     }\n//     imgDiv.onmouseover = function (): void { // Add a mouseover event to darken the image\n//       img.style.opacity = \"0.7\";\n//     }\n//     imgDiv.onmouseout = function (): void { // Add a mouseout event to lighten the image\n//       img.style.opacity = \"1.0\";\n//     }\n//     let img = imgDiv.appendChild(document.createElement(\"img\"))\n//     for (let key in data.args[\"img_style\"]) {\n//       img.style[key as any] = data.args[\"img_style\"][key]\n//     }\n//     img.src = data.args[\"paths\"][i]\n//     if (data.args[\"titles\"].length > i) {\n//       let imgTitle = imgDiv.appendChild(document.createElement(\"p\")) // Create a new p element for the title\n//       imgTitle.innerText = data.args[\"titles\"][i] // Set the innerText of the p element to the title\n//       imgTitle.style.paddingLeft = \"8px\"\n//     }\n//     // img.onclick = function (): void {\n//     //   Streamlit.setComponentValue(i)\n//     // }\n//     // eslint-disable-next-line\n//     img.onload = function (): void {\n//       imagesLoaded++\n//       if (imagesLoaded === data.args[\"paths\"].length) {\n//         Streamlit.setFrameHeight()\n//       }\n//     }\n//   }\n// }\n\n// Streamlit.events.addEventListener(Streamlit.RENDER_EVENT, onRender)\n// Streamlit.setComponentReady()\n\nimport { Streamlit, RenderData } from \"streamlit-component-lib\"\n\nfunction onRender(event: Event): void {\n  const data = (event as CustomEvent<RenderData>).detail\n\n  // Remove existing content\n  let child = document.body.lastElementChild;\n  while (child) {\n    document.body.removeChild(child);\n    child = document.body.lastElementChild;\n  }\n\n  // Add and style the image container\n  let div = document.body.appendChild(document.createElement(\"div\"))\n  for (let key in data.args[\"div_style\"]) {\n    div.style[key as any] = data.args[\"div_style\"][key]\n  }\n\n  // Add and style all images\n  let imagesLoaded = 0\n  for (let i = 0; i < data.args[\"paths\"].length; i++) {\n    let imgDiv = div.appendChild(document.createElement(\"div\")) // Create a new div for each image and its title\n    imgDiv.style.border = \"1px solid black\"; // Add a border to the div\n    imgDiv.style.padding = \"10px\"; // Add some padding to the div\n    imgDiv.style.cursor = \"pointer\";\n\n    let img = imgDiv.appendChild(document.createElement(\"img\"))\n    for (let key in data.args[\"img_style\"]) {\n      img.style[key as any] = data.args[\"img_style\"][key]\n    }\n    img.src = data.args[\"paths\"][i]\n\n    img.onload = function (): void {\n      imagesLoaded++\n      if (imagesLoaded === data.args[\"paths\"].length) {\n        Streamlit.setFrameHeight()\n      }\n    }\n\n    if (data.args[\"isActive\"][i]) {\n      imgDiv.onclick = function (): void { \n        window.open(data.args[\"links\"][i], \"_blank\")\n      }\n    } else {\n      imgDiv.onclick = function (): void { \n        Streamlit.setComponentValue(i)\n      }\n    }\n\n    if (data.args[\"titles\"].length > i) {\n      let imgTitle = imgDiv.appendChild(document.createElement(\"p\")) // Create a new p element for the title\n      imgTitle.innerText = data.args[\"titles\"][i] // Set the innerText of the p element to the title\n      imgTitle.style.paddingLeft = \"8px\"\n    }\n  }\n}\n\nStreamlit.events.addEventListener(Streamlit.RENDER_EVENT, onRender)\nStreamlit.setComponentReady()\n\n\n"
     ],
     "version": 3
 }
```

### Comparing `st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/static/js/runtime-main.11ec9aca.js` & `st-clickable-img-gallery-0.0.6/st_clickable_img_gallery/frontend/build/static/js/runtime-main.11ec9aca.js`

 * *Files identical despite different names*

### Comparing `st-clickable-img-gallery-0.0.5/st_clickable_img_gallery/frontend/build/static/js/runtime-main.11ec9aca.js.map` & `st-clickable-img-gallery-0.0.6/st_clickable_img_gallery/frontend/build/static/js/runtime-main.11ec9aca.js.map`

 * *Files identical despite different names*

### Comparing `st-clickable-img-gallery-0.0.5/st_clickable_img_gallery.egg-info/SOURCES.txt` & `st-clickable-img-gallery-0.0.6/st_clickable_img_gallery.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 st_clickable_img_gallery.egg-info/SOURCES.txt
 st_clickable_img_gallery.egg-info/dependency_links.txt
 st_clickable_img_gallery.egg-info/requires.txt
 st_clickable_img_gallery.egg-info/top_level.txt
 st_clickable_img_gallery/frontend/build/asset-manifest.json
 st_clickable_img_gallery/frontend/build/bootstrap.min.css
 st_clickable_img_gallery/frontend/build/index.html
-st_clickable_img_gallery/frontend/build/precache-manifest.0a644e34e8c91feca024ba003e7a6372.js
+st_clickable_img_gallery/frontend/build/precache-manifest.9bad0753763e9c65a26561a891d47387.js
 st_clickable_img_gallery/frontend/build/service-worker.js
 st_clickable_img_gallery/frontend/build/static/js/2.60f28383.chunk.js
 st_clickable_img_gallery/frontend/build/static/js/2.60f28383.chunk.js.LICENSE.txt
 st_clickable_img_gallery/frontend/build/static/js/2.60f28383.chunk.js.map
-st_clickable_img_gallery/frontend/build/static/js/main.53f69541.chunk.js
-st_clickable_img_gallery/frontend/build/static/js/main.53f69541.chunk.js.map
+st_clickable_img_gallery/frontend/build/static/js/main.1bc8d89a.chunk.js
+st_clickable_img_gallery/frontend/build/static/js/main.1bc8d89a.chunk.js.map
 st_clickable_img_gallery/frontend/build/static/js/runtime-main.11ec9aca.js
 st_clickable_img_gallery/frontend/build/static/js/runtime-main.11ec9aca.js.map
```

