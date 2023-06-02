# Comparing `tmp/jupyterlab_sparksql-0.2.0.tar.gz` & `tmp/jupyterlab_sparksql-1.1.0.tar.gz`

## Comparing `jupyterlab_sparksql-0.2.0.tar` & `jupyterlab_sparksql-1.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jupyterlab_sparksql-0.2.0/.prettierignore
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_sparksql-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 jupyterlab_sparksql-0.2.0/Dockerfile
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 jupyterlab_sparksql-0.2.0/Makefile
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 jupyterlab_sparksql-0.2.0/RELEASE.md
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 jupyterlab_sparksql-0.2.0/install.json
--rw-r--r--   0        0        0   538875 2020-02-02 00:00:00.000000 jupyterlab_sparksql-0.2.0/package-lock.json
--rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 jupyterlab_sparksql-0.2.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_sparksql-0.2.0/setup.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_sparksql-0.2.0/tsconfig.json
--rw-r--r--   0        0        0   190057 2020-02-02 00:00:00.000000 jupyterlab_sparksql-0.2.0/yarn.lock
--rw-r--r--   0        0        0    19228 2020-02-02 00:00:00.000000 jupyterlab_sparksql-0.2.0/example/Test.ipynb
--rw-r--r--   0        0        0     6113 2020-02-02 00:00:00.000000 jupyterlab_sparksql-0.2.0/example/Usage.ipynb
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 jupyterlab_sparksql-0.2.0/jupyterlab_sparksql/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_sparksql-0.2.0/jupyterlab_sparksql/_version.py
--rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 jupyterlab_sparksql-0.2.0/jupyterlab_sparksql/labextension/package.json
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 jupyterlab_sparksql-0.2.0/jupyterlab_sparksql/labextension/static/568.07bb5fea90bf1461a1c3.js
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 jupyterlab_sparksql-0.2.0/jupyterlab_sparksql/labextension/static/747.7ecba06e06bf4ca5847b.js
--rw-r--r--   0        0        0     6961 2020-02-02 00:00:00.000000 jupyterlab_sparksql-0.2.0/jupyterlab_sparksql/labextension/static/remoteEntry.23ec0fe6f1eb04f5f3f4.js
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 jupyterlab_sparksql-0.2.0/jupyterlab_sparksql/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyterlab_sparksql-0.2.0/jupyterlab_sparksql/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 jupyterlab_sparksql-0.2.0/jupyterlab_sparksql/magics/__init__.py
--rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 jupyterlab_sparksql-0.2.0/jupyterlab_sparksql/magics/sparksql.py
--rw-r--r--   0        0        0    13469 2020-02-02 00:00:00.000000 jupyterlab_sparksql-0.2.0/jupyterlab_sparksql/magics/widget.py
--rw-r--r--   0        0        0     4682 2020-02-02 00:00:00.000000 jupyterlab_sparksql-0.2.0/src/index.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_sparksql-0.2.0/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_sparksql-0.2.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_sparksql-0.2.0/style/index.js
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 jupyterlab_sparksql-0.2.0/.gitignore
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_sparksql-0.2.0/LICENSE
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 jupyterlab_sparksql-0.2.0/README.md
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 jupyterlab_sparksql-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 jupyterlab_sparksql-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jupyterlab_sparksql-1.1.0/.prettierignore
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_sparksql-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 jupyterlab_sparksql-1.1.0/Dockerfile
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 jupyterlab_sparksql-1.1.0/Makefile
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 jupyterlab_sparksql-1.1.0/RELEASE.md
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 jupyterlab_sparksql-1.1.0/install.json
+-rw-r--r--   0        0        0   538875 2020-02-02 00:00:00.000000 jupyterlab_sparksql-1.1.0/package-lock.json
+-rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 jupyterlab_sparksql-1.1.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_sparksql-1.1.0/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_sparksql-1.1.0/tsconfig.json
+-rw-r--r--   0        0        0   190057 2020-02-02 00:00:00.000000 jupyterlab_sparksql-1.1.0/yarn.lock
+-rw-r--r--   0        0        0    19228 2020-02-02 00:00:00.000000 jupyterlab_sparksql-1.1.0/example/Test.ipynb
+-rw-r--r--   0        0        0     6113 2020-02-02 00:00:00.000000 jupyterlab_sparksql-1.1.0/example/Usage.ipynb
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 jupyterlab_sparksql-1.1.0/jupyterlab_sparksql/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_sparksql-1.1.0/jupyterlab_sparksql/_version.py
+-rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 jupyterlab_sparksql-1.1.0/jupyterlab_sparksql/labextension/package.json
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 jupyterlab_sparksql-1.1.0/jupyterlab_sparksql/labextension/static/568.241643848d12210f39b0.js
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 jupyterlab_sparksql-1.1.0/jupyterlab_sparksql/labextension/static/747.7ecba06e06bf4ca5847b.js
+-rw-r--r--   0        0        0     6961 2020-02-02 00:00:00.000000 jupyterlab_sparksql-1.1.0/jupyterlab_sparksql/labextension/static/remoteEntry.cf84e0c5aa4d370967c0.js
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 jupyterlab_sparksql-1.1.0/jupyterlab_sparksql/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyterlab_sparksql-1.1.0/jupyterlab_sparksql/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 jupyterlab_sparksql-1.1.0/jupyterlab_sparksql/magics/__init__.py
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 jupyterlab_sparksql-1.1.0/jupyterlab_sparksql/magics/sparksql.py
+-rw-r--r--   0        0        0    19338 2020-02-02 00:00:00.000000 jupyterlab_sparksql-1.1.0/jupyterlab_sparksql/magics/widget.py
+-rw-r--r--   0        0        0     4682 2020-02-02 00:00:00.000000 jupyterlab_sparksql-1.1.0/src/index.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_sparksql-1.1.0/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_sparksql-1.1.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_sparksql-1.1.0/style/index.js
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 jupyterlab_sparksql-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_sparksql-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 jupyterlab_sparksql-1.1.0/README.md
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 jupyterlab_sparksql-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 jupyterlab_sparksql-1.1.0/PKG-INFO
```

### Comparing `jupyterlab_sparksql-0.2.0/RELEASE.md` & `jupyterlab_sparksql-1.1.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_sparksql-0.2.0/package-lock.json` & `jupyterlab_sparksql-1.1.0/package-lock.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_sparksql-0.2.0/package.json` & `jupyterlab_sparksql-1.1.0/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'1.1.0'"}*

```diff
@@ -163,9 +163,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.0"
+    "version": "1.1.0"
 }
```

### Comparing `jupyterlab_sparksql-0.2.0/tsconfig.json` & `jupyterlab_sparksql-1.1.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_sparksql-0.2.0/yarn.lock` & `jupyterlab_sparksql-1.1.0/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_sparksql-0.2.0/example/Test.ipynb` & `jupyterlab_sparksql-1.1.0/example/Test.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_sparksql-0.2.0/example/Usage.ipynb` & `jupyterlab_sparksql-1.1.0/example/Usage.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_sparksql-0.2.0/jupyterlab_sparksql/labextension/package.json` & `jupyterlab_sparksql-1.1.0/jupyterlab_sparksql/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9785879629629629%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.cf84e0c5aa4d370967c0.js'}}",*

 * * "'version'": "'1.1.0'"}*

```diff
@@ -96,15 +96,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/vule24/jupyterlab-sparksql",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.23ec0fe6f1eb04f5f3f4.js",
+            "load": "static/remoteEntry.cf84e0c5aa4d370967c0.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyterlab_sparksql/labextension"
     },
     "keywords": [
         "jupyter",
@@ -168,9 +168,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.0"
+    "version": "1.1.0"
 }
```

### Comparing `jupyterlab_sparksql-0.2.0/jupyterlab_sparksql/labextension/static/568.07bb5fea90bf1461a1c3.js` & `jupyterlab_sparksql-1.1.0/jupyterlab_sparksql/labextension/static/568.241643848d12210f39b0.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
 "use strict";
 (self.webpackChunkjupyterlab_sparksql = self.webpackChunkjupyterlab_sparksql || []).push([
     [568], {
         568: (t, e, i) => {
             i.r(e), i.d(e, {
                 default: () => c
             });
-            var n = i(123),
-                s = i(191);
+            var n = i(779),
+                s = i(872);
             const r = {
                 ipython: "text/x-ipython",
                 "%%sql": "text/x-pgsql",
                 "%%sh": "text/x-sh",
                 "%%bash": "text/x-sh",
                 "%%html": "text/html",
                 "%%javascript": "text/javascript",
```

### Comparing `jupyterlab_sparksql-0.2.0/jupyterlab_sparksql/labextension/static/747.7ecba06e06bf4ca5847b.js` & `jupyterlab_sparksql-1.1.0/jupyterlab_sparksql/labextension/static/747.7ecba06e06bf4ca5847b.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_sparksql-0.2.0/jupyterlab_sparksql/labextension/static/remoteEntry.23ec0fe6f1eb04f5f3f4.js` & `jupyterlab_sparksql-1.1.0/jupyterlab_sparksql/labextension/static/remoteEntry.cf84e0c5aa4d370967c0.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -43,18 +43,18 @@
         }), r
     }, S.d = (e, r) => {
         for (var t in r) S.o(r, t) && !S.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
-        568: "07bb5fea90bf1461a1c3",
+        568: "241643848d12210f39b0",
         747: "7ecba06e06bf4ca5847b"
     } [e] + ".js?v=" + {
-        568: "07bb5fea90bf1461a1c3",
+        568: "241643848d12210f39b0",
         747: "7ecba06e06bf4ca5847b"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
@@ -106,15 +106,15 @@
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => S.e(568).then((() => () => S(568))),
                         from: i,
                         eager: !1
                     })
-                })("jupyterlab-sparksql", "0.2.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("jupyterlab-sparksql", "1.1.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -216,18 +216,18 @@
         return "No satisfying version (" + o(n) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(a).map((e => e + " from " + a[e].from)).join(", ")
     }, c = (e, r, t, n) => {
         "undefined" != typeof console && console.warn && console.warn(p(e, r, t, n))
     }, h = e => (e.loaded = 1, e.get()), b = (v = e => function(r, t, n, o) {
         var a = S.I(r);
         return a && a.then ? a.then(e.bind(e, r, S.S[r], t, n, o)) : e(r, S.S[r], t, n, o)
     })(((e, r, t, n) => (i(e, t), h(d(r, t, n) || c(r, e, t, n) || u(r, t))))), g = v(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), y = {}, m = {
-        123: () => g("default", "@jupyterlab/notebook", [1, 3, 6, 3]),
-        191: () => b("default", "@jupyterlab/cells", [1, 3, 6, 3])
+        779: () => g("default", "@jupyterlab/notebook", [1, 3, 6, 4]),
+        872: () => b("default", "@jupyterlab/cells", [1, 3, 6, 4])
     }, w = {
-        568: [123, 191]
+        568: [779, 872]
     }, S.f.consumes = (e, r) => {
         S.o(w, e) && w[e].forEach((e => {
             if (S.o(y, e)) return r.push(y[e]);
             var t = r => {
                     y[e] = 0, S.m[e] = t => {
                         delete S.c[e], t.exports = r()
                     }
```

### Comparing `jupyterlab_sparksql-0.2.0/jupyterlab_sparksql/labextension/static/third-party-licenses.json` & `jupyterlab_sparksql-1.1.0/jupyterlab_sparksql/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_sparksql-0.2.0/jupyterlab_sparksql/magics/__init__.py` & `jupyterlab_sparksql-1.1.0/jupyterlab_sparksql/magics/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sparksql-0.2.0/jupyterlab_sparksql/magics/sparksql.py` & `jupyterlab_sparksql-1.1.0/jupyterlab_sparksql/magics/sparksql.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,54 @@
 from IPython.core.magic import Magics, magics_class, cell_magic, line_magic
 from IPython.core.magic_arguments import argument, magic_arguments, parse_argstring
 from pyspark.sql import SparkSession
 from pyspark.sql.dataframe import DataFrame
 from string import Formatter
 
-from .widget import generate_output_widget, generate_classic_table
+from .widget import generate_output_widget
 
 
 @magics_class
 class SparkSQL(Magics):
 
     @property
     def spark(self):
         return SparkSession._instantiatedSession
 
     @magic_arguments()
     @argument('dataframe', metavar='DF', type=str, nargs='?')
     @argument('-n', '--num-rows', type=int, default=100)
-    @argument('-c', '--classic', action='store_true', default=False)
     @cell_magic
     def sql(self, line, cell):
         self.create_temp_view_for_available_dataframe()
         
         args = parse_argstring(self.sql, line)
         query_str = rf'{self.format_fillin_pyvar(cell)}'
         
         sdf = self.spark.sql(query_str)
         if args.dataframe:
             self.shell.user_ns.update({args.dataframe: sdf})
-        if not args.classic:
-            return generate_output_widget(sdf, num_rows=args.num_rows, export_table_name=args.dataframe or None)
-        else:
-            return generate_classic_table(sdf, num_rows=args.num_rows)
+
+        return generate_output_widget(sdf, num_rows=args.num_rows, export_table_name=args.dataframe or None)
+
 
 
     @magic_arguments()
     @argument('dataframe', metavar='DF', type=str, nargs='?')
     @argument('-n', '--num-rows', type=int, default=20)
-    @argument('-c', '--classic', action='store_true', default=False)
     @line_magic
     def show(self, line):
         args = parse_argstring(self.sql, line)
         if not args.dataframe:
             raise ValueError('dataframe is required. Eg. `%show <dataframe>`')
         sdf = self.shell.user_ns.get(args.dataframe, None)
         if not sdf:
             raise NameError(f"Name '{args.dataframe}' is not defined")
-        if not args.classic:
-            return generate_output_widget(sdf, num_rows=args.num_rows, export_table_name=args.dataframe)
-        else:
-            return generate_classic_table(sdf, num_rows=args.num_rows)
+        
+        return generate_output_widget(sdf, num_rows=args.num_rows, export_table_name=args.dataframe)
 
 
     def create_temp_view_for_available_dataframe(self):
         for k, v in self.shell.user_ns.items():
             v.createOrReplaceTempView(k) if isinstance(v, DataFrame) else None
 
     def format_fillin_pyvar(self, source):
```

### Comparing `jupyterlab_sparksql-0.2.0/src/index.ts` & `jupyterlab_sparksql-1.1.0/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_sparksql-0.2.0/.gitignore` & `jupyterlab_sparksql-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_sparksql-0.2.0/LICENSE` & `jupyterlab_sparksql-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_sparksql-0.2.0/README.md` & `jupyterlab_sparksql-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_sparksql-0.2.0/pyproject.toml` & `jupyterlab_sparksql-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_sparksql-0.2.0/PKG-INFO` & `jupyterlab_sparksql-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_sparksql
-Version: 0.2.0
+Version: 1.1.0
 Summary: A JupyterLab extension that provides SparkSQL magic commands, a SparkSQL syntax highlighter, and visualization widgets.
 Project-URL: Homepage, https://github.com/vule24/jupyterlab-sparksql
 Project-URL: Bug Tracker, https://github.com/vule24/jupyterlab-sparksql/issues
 Project-URL: Repository, https://github.com/vule24/jupyterlab-sparksql.git
 Author-email: Vu Le <ltnv24@gmail.com>
 License: BSD 3-Clause License
```

