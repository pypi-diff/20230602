# Comparing `tmp/pyvista-imgui-0.1.0.tar.gz` & `tmp/pyvista-imgui-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvista-imgui-0.1.0.tar", last modified: Fri Jun  2 11:34:11 2023, max compression
+gzip compressed data, was "pyvista-imgui-0.1.1.tar", last modified: Fri Jun  2 11:37:51 2023, max compression
```

## Comparing `pyvista-imgui-0.1.0.tar` & `pyvista-imgui-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:34:11.859407 pyvista-imgui-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:34:11.855407 pyvista-imgui-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:34:11.859407 pyvista-imgui-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-02 11:33:52.000000 pyvista-imgui-0.1.0/.github/workflows/python-package-build-and-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-02 11:33:52.000000 pyvista-imgui-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-02 11:33:52.000000 pyvista-imgui-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-02 11:33:52.000000 pyvista-imgui-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-02 11:34:11.859407 pyvista-imgui-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-02 11:33:52.000000 pyvista-imgui-0.1.0/PyVista.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-02 11:33:52.000000 pyvista-imgui-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:34:11.859407 pyvista-imgui-0.1.0/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-02 11:33:52.000000 pyvista-imgui-0.1.0/example/example_embedded.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-02 11:33:52.000000 pyvista-imgui-0.1.0/example/example_standalone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-02 11:33:52.000000 pyvista-imgui-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:34:11.859407 pyvista-imgui-0.1.0/pyvista_imgui/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-02 11:33:52.000000 pyvista-imgui-0.1.0/pyvista_imgui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-02 11:34:11.000000 pyvista-imgui-0.1.0/pyvista_imgui/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-06-02 11:33:52.000000 pyvista-imgui-0.1.0/pyvista_imgui/imgui_render_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-06-02 11:33:52.000000 pyvista-imgui-0.1.0/pyvista_imgui/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-06-02 11:33:52.000000 pyvista-imgui-0.1.0/pyvista_imgui/texture_render_window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:34:11.859407 pyvista-imgui-0.1.0/pyvista_imgui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-02 11:34:11.000000 pyvista-imgui-0.1.0/pyvista_imgui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-02 11:34:11.000000 pyvista-imgui-0.1.0/pyvista_imgui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 11:34:11.000000 pyvista-imgui-0.1.0/pyvista_imgui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-02 11:34:11.000000 pyvista-imgui-0.1.0/pyvista_imgui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 11:34:11.000000 pyvista-imgui-0.1.0/pyvista_imgui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 11:34:11.859407 pyvista-imgui-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-02 11:33:52.000000 pyvista-imgui-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:37:51.324796 pyvista-imgui-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:37:51.320796 pyvista-imgui-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:37:51.320796 pyvista-imgui-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-02 11:37:26.000000 pyvista-imgui-0.1.1/.github/workflows/python-package-build-and-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-02 11:37:26.000000 pyvista-imgui-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-02 11:37:26.000000 pyvista-imgui-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-02 11:37:26.000000 pyvista-imgui-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-06-02 11:37:51.324796 pyvista-imgui-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-02 11:37:26.000000 pyvista-imgui-0.1.1/PyVista.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-02 11:37:26.000000 pyvista-imgui-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:37:51.320796 pyvista-imgui-0.1.1/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-02 11:37:26.000000 pyvista-imgui-0.1.1/example/example_embedded.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-02 11:37:26.000000 pyvista-imgui-0.1.1/example/example_standalone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-02 11:37:26.000000 pyvista-imgui-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:37:51.320796 pyvista-imgui-0.1.1/pyvista_imgui/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-02 11:37:26.000000 pyvista-imgui-0.1.1/pyvista_imgui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-02 11:37:51.000000 pyvista-imgui-0.1.1/pyvista_imgui/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-06-02 11:37:26.000000 pyvista-imgui-0.1.1/pyvista_imgui/imgui_render_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-06-02 11:37:26.000000 pyvista-imgui-0.1.1/pyvista_imgui/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-06-02 11:37:26.000000 pyvista-imgui-0.1.1/pyvista_imgui/texture_render_window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:37:51.324796 pyvista-imgui-0.1.1/pyvista_imgui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-06-02 11:37:51.000000 pyvista-imgui-0.1.1/pyvista_imgui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-02 11:37:51.000000 pyvista-imgui-0.1.1/pyvista_imgui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 11:37:51.000000 pyvista-imgui-0.1.1/pyvista_imgui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-02 11:37:51.000000 pyvista-imgui-0.1.1/pyvista_imgui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 11:37:51.000000 pyvista-imgui-0.1.1/pyvista_imgui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 11:37:51.324796 pyvista-imgui-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-02 11:37:26.000000 pyvista-imgui-0.1.1/setup.py
```

### Comparing `pyvista-imgui-0.1.0/.github/workflows/python-package-build-and-publish.yaml` & `pyvista-imgui-0.1.1/.github/workflows/python-package-build-and-publish.yaml`

 * *Files identical despite different names*

### Comparing `pyvista-imgui-0.1.0/.gitignore` & `pyvista-imgui-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyvista-imgui-0.1.0/LICENSE` & `pyvista-imgui-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvista-imgui-0.1.0/PKG-INFO` & `pyvista-imgui-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvista-imgui
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pyvista imgui integration
 Author-email: Felix Igelbrink <felix.igelbrink@dfki.de>
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mortacious/pyvista-imgui/issues
 Project-URL: Source Code, https://github.com/mortacious/pyvista-imgui
 Keywords: vtk,imgui,plotting
 Classifier: Development Status :: 4 - Beta
@@ -19,25 +19,25 @@
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Pyvista-Imgui
 
-[![PyPi license](https://badgen.net/pypi/license/pip/)](https://pypi.org/project/pip/) [![PyPi version](https://badgen.net/pypi/v/pip/)](https://pypi.org/project/pip)
+[![PyPi license](https://badgen.net/pypi/license/pyvista-imgui/)](https://pypi.org/project/pyvista-imgui/) [![PyPi version](https://badgen.net/pypi/v/pyvista-imgui/)](https://pypi.org/project/pyvista-imgui/)
 
 `pyvista-imgui` is a small helper module for the [`pyvista`](https://github.com/pyvista/pyvista)-package to integrate it with the [imgui](https://github.com/ocornut/imgui)-library. 
 
 It integrates a fully interactive `pyvista`-Plotter as an imgui-widget, by utilizing VTK's `vtkGenericOpenGLRenderWindow` to first render the output into an OpenGL texture and displaying it as a regular imgui-Image widget.
 
 It currently utilizes the bindings provided by [`imgui-bundle`](https://github.com/ocornut/imgui), but the integration of other imgui-bindings is planned for a future release.
 
 This package is considered experimental at this moment, so expect issues.
 
-## Installation
+## Installation5
 
 To install this package using `pip` use:
 
 ```bash
 pip install pyvista-imgui
 ```
```

### Comparing `pyvista-imgui-0.1.0/README.md` & `pyvista-imgui-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Pyvista-Imgui
 
-[![PyPi license](https://badgen.net/pypi/license/pip/)](https://pypi.org/project/pip/) [![PyPi version](https://badgen.net/pypi/v/pip/)](https://pypi.org/project/pip)
+[![PyPi license](https://badgen.net/pypi/license/pyvista-imgui/)](https://pypi.org/project/pyvista-imgui/) [![PyPi version](https://badgen.net/pypi/v/pyvista-imgui/)](https://pypi.org/project/pyvista-imgui/)
 
 `pyvista-imgui` is a small helper module for the [`pyvista`](https://github.com/pyvista/pyvista)-package to integrate it with the [imgui](https://github.com/ocornut/imgui)-library. 
 
 It integrates a fully interactive `pyvista`-Plotter as an imgui-widget, by utilizing VTK's `vtkGenericOpenGLRenderWindow` to first render the output into an OpenGL texture and displaying it as a regular imgui-Image widget.
 
 It currently utilizes the bindings provided by [`imgui-bundle`](https://github.com/ocornut/imgui), but the integration of other imgui-bindings is planned for a future release.
 
 This package is considered experimental at this moment, so expect issues.
 
-## Installation
+## Installation5
 
 To install this package using `pip` use:
 
 ```bash
 pip install pyvista-imgui
 ```
```

### Comparing `pyvista-imgui-0.1.0/example/example_embedded.py` & `pyvista-imgui-0.1.1/example/example_embedded.py`

 * *Files identical despite different names*

### Comparing `pyvista-imgui-0.1.0/pyproject.toml` & `pyvista-imgui-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyvista-imgui-0.1.0/pyvista_imgui/imgui_render_window.py` & `pyvista-imgui-0.1.1/pyvista_imgui/imgui_render_window.py`

 * *Files identical despite different names*

### Comparing `pyvista-imgui-0.1.0/pyvista_imgui/plotting.py` & `pyvista-imgui-0.1.1/pyvista_imgui/plotting.py`

 * *Files identical despite different names*

### Comparing `pyvista-imgui-0.1.0/pyvista_imgui/texture_render_window.py` & `pyvista-imgui-0.1.1/pyvista_imgui/texture_render_window.py`

 * *Files identical despite different names*

### Comparing `pyvista-imgui-0.1.0/pyvista_imgui.egg-info/PKG-INFO` & `pyvista-imgui-0.1.1/pyvista_imgui.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvista-imgui
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pyvista imgui integration
 Author-email: Felix Igelbrink <felix.igelbrink@dfki.de>
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mortacious/pyvista-imgui/issues
 Project-URL: Source Code, https://github.com/mortacious/pyvista-imgui
 Keywords: vtk,imgui,plotting
 Classifier: Development Status :: 4 - Beta
@@ -19,25 +19,25 @@
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Pyvista-Imgui
 
-[![PyPi license](https://badgen.net/pypi/license/pip/)](https://pypi.org/project/pip/) [![PyPi version](https://badgen.net/pypi/v/pip/)](https://pypi.org/project/pip)
+[![PyPi license](https://badgen.net/pypi/license/pyvista-imgui/)](https://pypi.org/project/pyvista-imgui/) [![PyPi version](https://badgen.net/pypi/v/pyvista-imgui/)](https://pypi.org/project/pyvista-imgui/)
 
 `pyvista-imgui` is a small helper module for the [`pyvista`](https://github.com/pyvista/pyvista)-package to integrate it with the [imgui](https://github.com/ocornut/imgui)-library. 
 
 It integrates a fully interactive `pyvista`-Plotter as an imgui-widget, by utilizing VTK's `vtkGenericOpenGLRenderWindow` to first render the output into an OpenGL texture and displaying it as a regular imgui-Image widget.
 
 It currently utilizes the bindings provided by [`imgui-bundle`](https://github.com/ocornut/imgui), but the integration of other imgui-bindings is planned for a future release.
 
 This package is considered experimental at this moment, so expect issues.
 
-## Installation
+## Installation5
 
 To install this package using `pip` use:
 
 ```bash
 pip install pyvista-imgui
 ```
```

### Comparing `pyvista-imgui-0.1.0/pyvista_imgui.egg-info/SOURCES.txt` & `pyvista-imgui-0.1.1/pyvista_imgui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

