# Comparing `tmp/mebuex-1.1.4.tar.gz` & `tmp/mebuex-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mebuex-1.1.4.tar", last modified: Thu May  4 10:04:30 2023, max compression
+gzip compressed data, was "mebuex-1.1.5.tar", last modified: Fri Jun  2 11:30:43 2023, max compression
```

## Comparing `mebuex-1.1.4.tar` & `mebuex-1.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2023-05-04 10:04:30.501773 mebuex-1.1.4/
--rw-r--r--   0 phd       (1000) phd       (1000)     1056 2022-07-13 11:17:33.000000 mebuex-1.1.4/LICENSE
--rw-r--r--   0 phd       (1000) phd       (1000)     3397 2023-05-04 10:04:30.501773 mebuex-1.1.4/PKG-INFO
--rw-r--r--   0 phd       (1000) phd       (1000)     2654 2023-05-04 10:01:39.000000 mebuex-1.1.4/README.md
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2023-05-04 10:04:30.501773 mebuex-1.1.4/mebuex/
--rw-r--r--   0 phd       (1000) phd       (1000)      213 2022-07-13 11:31:24.000000 mebuex-1.1.4/mebuex/__init__.py
--rw-r--r--   0 phd       (1000) phd       (1000)     4150 2023-05-04 09:59:53.000000 mebuex-1.1.4/mebuex/build_ext.py
--rw-r--r--   0 phd       (1000) phd       (1000)      799 2022-07-13 13:28:44.000000 mebuex-1.1.4/mebuex/extension.py
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2023-05-04 10:04:30.501773 mebuex-1.1.4/mebuex.egg-info/
--rw-r--r--   0 phd       (1000) phd       (1000)     3397 2023-05-04 10:04:30.000000 mebuex-1.1.4/mebuex.egg-info/PKG-INFO
--rw-r--r--   0 phd       (1000) phd       (1000)      240 2023-05-04 10:04:30.000000 mebuex-1.1.4/mebuex.egg-info/SOURCES.txt
--rw-r--r--   0 phd       (1000) phd       (1000)        1 2023-05-04 10:04:30.000000 mebuex-1.1.4/mebuex.egg-info/dependency_links.txt
--rw-r--r--   0 phd       (1000) phd       (1000)        6 2023-05-04 10:04:30.000000 mebuex-1.1.4/mebuex.egg-info/requires.txt
--rw-r--r--   0 phd       (1000) phd       (1000)        7 2023-05-04 10:04:30.000000 mebuex-1.1.4/mebuex.egg-info/top_level.txt
--rw-r--r--   0 phd       (1000) phd       (1000)      829 2023-05-04 10:01:46.000000 mebuex-1.1.4/pyproject.toml
--rw-r--r--   0 phd       (1000) phd       (1000)       38 2023-05-04 10:04:30.501773 mebuex-1.1.4/setup.cfg
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2023-06-02 11:30:43.298753 mebuex-1.1.5/
+-rw-r--r--   0 phd       (1000) phd       (1000)     1056 2022-07-13 11:17:33.000000 mebuex-1.1.5/LICENSE
+-rw-r--r--   0 phd       (1000) phd       (1000)     3537 2023-06-02 11:30:43.298753 mebuex-1.1.5/PKG-INFO
+-rw-r--r--   0 phd       (1000) phd       (1000)     2794 2023-06-02 11:26:18.000000 mebuex-1.1.5/README.md
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2023-06-02 11:30:43.298753 mebuex-1.1.5/mebuex/
+-rw-r--r--   0 phd       (1000) phd       (1000)      213 2022-07-13 11:31:24.000000 mebuex-1.1.5/mebuex/__init__.py
+-rw-r--r--   0 phd       (1000) phd       (1000)     4936 2023-06-02 11:25:53.000000 mebuex-1.1.5/mebuex/build_ext.py
+-rw-r--r--   0 phd       (1000) phd       (1000)      799 2022-07-13 13:28:44.000000 mebuex-1.1.5/mebuex/extension.py
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2023-06-02 11:30:43.298753 mebuex-1.1.5/mebuex.egg-info/
+-rw-r--r--   0 phd       (1000) phd       (1000)     3537 2023-06-02 11:30:43.000000 mebuex-1.1.5/mebuex.egg-info/PKG-INFO
+-rw-r--r--   0 phd       (1000) phd       (1000)      240 2023-06-02 11:30:43.000000 mebuex-1.1.5/mebuex.egg-info/SOURCES.txt
+-rw-r--r--   0 phd       (1000) phd       (1000)        1 2023-06-02 11:30:43.000000 mebuex-1.1.5/mebuex.egg-info/dependency_links.txt
+-rw-r--r--   0 phd       (1000) phd       (1000)        6 2023-06-02 11:30:43.000000 mebuex-1.1.5/mebuex.egg-info/requires.txt
+-rw-r--r--   0 phd       (1000) phd       (1000)        7 2023-06-02 11:30:43.000000 mebuex-1.1.5/mebuex.egg-info/top_level.txt
+-rw-r--r--   0 phd       (1000) phd       (1000)      829 2023-06-02 11:12:42.000000 mebuex-1.1.5/pyproject.toml
+-rw-r--r--   0 phd       (1000) phd       (1000)       38 2023-06-02 11:30:43.298753 mebuex-1.1.5/setup.cfg
```

### Comparing `mebuex-1.1.4/LICENSE` & `mebuex-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mebuex-1.1.4/PKG-INFO` & `mebuex-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mebuex
-Version: 1.1.4
+Version: 1.1.5
 Summary: Combining build_ext with the Meson build system
 Author-email: "Malte J. Ziebarth" <mjz.science@fmvkb.de>
 License: MIT
 Project-URL: Homepage, https://github.com/mjziebarth/Mebuex
 Project-URL: Bug Tracker, https://github.com/mjziebarth/Mebuex/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -71,14 +71,19 @@
 ## License
 Mebuex is licensed under the MIT license (see the LICENSE file).
 
 ## Changelog
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+### [1.1.5] - 2023-06-02
+#### Changed
+ - Try wiping the build directory if compilation within a previously setup
+   build directory fails.
+
 ### [1.1.4] - 2023-05-04
 #### Changed
  - Be more verbose on `destpath` error in `build_ext.build_extension`.
 
 ### [1.1.3] - 2023-04-14
 #### Added
  - Add example project in `example/` subfolder.
```

### Comparing `mebuex-1.1.4/README.md` & `mebuex-1.1.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -52,14 +52,19 @@
 ## License
 Mebuex is licensed under the MIT license (see the LICENSE file).
 
 ## Changelog
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+### [1.1.5] - 2023-06-02
+#### Changed
+ - Try wiping the build directory if compilation within a previously setup
+   build directory fails.
+
 ### [1.1.4] - 2023-05-04
 #### Changed
  - Be more verbose on `destpath` error in `build_ext.build_extension`.
 
 ### [1.1.3] - 2023-04-14
 #### Added
  - Add example project in `example/` subfolder.
```

### Comparing `mebuex-1.1.4/mebuex/build_ext.py` & `mebuex-1.1.5/mebuex/build_ext.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,21 +18,38 @@
     """
     def build_extension(self, ext):
         if isinstance(ext, MesonExtension):
             # Meson build.
             # First ensure that the build directory is set up:
             currentpath = Path().resolve()
             buildpath = (Path(ext.sourcepath) / ext.builddir).resolve()
+            first_setup = False
             if not Path(buildpath).is_dir():
                 os.chdir(ext.sourcepath)
                 subprocess.run(["meson","setup",ext.builddir], check=True)
+                first_setup = True
 
             # Compile within the build directory:
             os.chdir(buildpath)
-            subprocess.run(["meson","compile"], check=True)
+            try:
+                subprocess.run(["meson","compile"], check=True,
+                               capture_output=True)
+            except subprocess.CalledProcessError as e:
+                # Check if the build files have been generated by an old version
+                # of meson and need to be wiped:
+                if "--wipe" not in str(e.output) or first_setup:
+                    # Likely a true compilation error.
+                    raise e
+
+                # Try to wipe the build dir and try again:
+                os.chdir(currentpath)
+                subprocess.run(["meson","setup",ext.builddir,"--wipe"],
+                               check=True)
+                os.chdir(buildpath)
+                subprocess.run(["meson","compile"], check=True)
             os.chdir(currentpath)
 
             # Copy the file.
             #
             # This following code to compute the relevant path and file names,
             # is, up to the comment marking the end, adapted from
             # setuptools/command/build_ext.py, released under MIT license.
```

### Comparing `mebuex-1.1.4/mebuex/extension.py` & `mebuex-1.1.5/mebuex/extension.py`

 * *Files identical despite different names*

### Comparing `mebuex-1.1.4/mebuex.egg-info/PKG-INFO` & `mebuex-1.1.5/mebuex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mebuex
-Version: 1.1.4
+Version: 1.1.5
 Summary: Combining build_ext with the Meson build system
 Author-email: "Malte J. Ziebarth" <mjz.science@fmvkb.de>
 License: MIT
 Project-URL: Homepage, https://github.com/mjziebarth/Mebuex
 Project-URL: Bug Tracker, https://github.com/mjziebarth/Mebuex/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -71,14 +71,19 @@
 ## License
 Mebuex is licensed under the MIT license (see the LICENSE file).
 
 ## Changelog
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+### [1.1.5] - 2023-06-02
+#### Changed
+ - Try wiping the build directory if compilation within a previously setup
+   build directory fails.
+
 ### [1.1.4] - 2023-05-04
 #### Changed
  - Be more verbose on `destpath` error in `build_ext.build_extension`.
 
 ### [1.1.3] - 2023-04-14
 #### Added
  - Add example project in `example/` subfolder.
```

