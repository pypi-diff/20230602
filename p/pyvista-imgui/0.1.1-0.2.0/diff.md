# Comparing `tmp/pyvista-imgui-0.1.1.tar.gz` & `tmp/pyvista-imgui-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvista-imgui-0.1.1.tar", last modified: Fri Jun  2 11:37:51 2023, max compression
+gzip compressed data, was "pyvista-imgui-0.2.0.tar", last modified: Fri Jun  2 19:42:38 2023, max compression
```

## Comparing `pyvista-imgui-0.1.1.tar` & `pyvista-imgui-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:37:51.324796 pyvista-imgui-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:37:51.320796 pyvista-imgui-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:37:51.320796 pyvista-imgui-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-02 11:37:26.000000 pyvista-imgui-0.1.1/.github/workflows/python-package-build-and-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-02 11:37:26.000000 pyvista-imgui-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-02 11:37:26.000000 pyvista-imgui-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-02 11:37:26.000000 pyvista-imgui-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-06-02 11:37:51.324796 pyvista-imgui-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-02 11:37:26.000000 pyvista-imgui-0.1.1/PyVista.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-02 11:37:26.000000 pyvista-imgui-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:37:51.320796 pyvista-imgui-0.1.1/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-02 11:37:26.000000 pyvista-imgui-0.1.1/example/example_embedded.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-02 11:37:26.000000 pyvista-imgui-0.1.1/example/example_standalone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-02 11:37:26.000000 pyvista-imgui-0.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:37:51.320796 pyvista-imgui-0.1.1/pyvista_imgui/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-02 11:37:26.000000 pyvista-imgui-0.1.1/pyvista_imgui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-02 11:37:51.000000 pyvista-imgui-0.1.1/pyvista_imgui/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-06-02 11:37:26.000000 pyvista-imgui-0.1.1/pyvista_imgui/imgui_render_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-06-02 11:37:26.000000 pyvista-imgui-0.1.1/pyvista_imgui/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-06-02 11:37:26.000000 pyvista-imgui-0.1.1/pyvista_imgui/texture_render_window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:37:51.324796 pyvista-imgui-0.1.1/pyvista_imgui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-06-02 11:37:51.000000 pyvista-imgui-0.1.1/pyvista_imgui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-02 11:37:51.000000 pyvista-imgui-0.1.1/pyvista_imgui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 11:37:51.000000 pyvista-imgui-0.1.1/pyvista_imgui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-02 11:37:51.000000 pyvista-imgui-0.1.1/pyvista_imgui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 11:37:51.000000 pyvista-imgui-0.1.1/pyvista_imgui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 11:37:51.324796 pyvista-imgui-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-02 11:37:26.000000 pyvista-imgui-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:42:38.731080 pyvista-imgui-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:42:38.723080 pyvista-imgui-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:42:38.727080 pyvista-imgui-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-02 19:42:19.000000 pyvista-imgui-0.2.0/.github/workflows/python-package-build-and-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-02 19:42:19.000000 pyvista-imgui-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-02 19:42:19.000000 pyvista-imgui-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-02 19:42:19.000000 pyvista-imgui-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-06-02 19:42:38.731080 pyvista-imgui-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-02 19:42:19.000000 pyvista-imgui-0.2.0/PyVista.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-02 19:42:19.000000 pyvista-imgui-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:42:38.727080 pyvista-imgui-0.2.0/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-02 19:42:19.000000 pyvista-imgui-0.2.0/example/example_embedded.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-02 19:42:19.000000 pyvista-imgui-0.2.0/example/example_standalone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-02 19:42:19.000000 pyvista-imgui-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:42:38.727080 pyvista-imgui-0.2.0/pyvista_imgui/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-02 19:42:19.000000 pyvista-imgui-0.2.0/pyvista_imgui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-02 19:42:38.000000 pyvista-imgui-0.2.0/pyvista_imgui/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-06-02 19:42:19.000000 pyvista-imgui-0.2.0/pyvista_imgui/imgui_render_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10132 2023-06-02 19:42:19.000000 pyvista-imgui-0.2.0/pyvista_imgui/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-06-02 19:42:19.000000 pyvista-imgui-0.2.0/pyvista_imgui/texture_render_window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:42:38.731080 pyvista-imgui-0.2.0/pyvista_imgui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-06-02 19:42:38.000000 pyvista-imgui-0.2.0/pyvista_imgui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-02 19:42:38.000000 pyvista-imgui-0.2.0/pyvista_imgui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 19:42:38.000000 pyvista-imgui-0.2.0/pyvista_imgui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-02 19:42:38.000000 pyvista-imgui-0.2.0/pyvista_imgui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 19:42:38.000000 pyvista-imgui-0.2.0/pyvista_imgui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 19:42:38.731080 pyvista-imgui-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-02 19:42:19.000000 pyvista-imgui-0.2.0/setup.py
```

### Comparing `pyvista-imgui-0.1.1/.github/workflows/python-package-build-and-publish.yaml` & `pyvista-imgui-0.2.0/.github/workflows/python-package-build-and-publish.yaml`

 * *Files identical despite different names*

### Comparing `pyvista-imgui-0.1.1/.gitignore` & `pyvista-imgui-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyvista-imgui-0.1.1/LICENSE` & `pyvista-imgui-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvista-imgui-0.1.1/PKG-INFO` & `pyvista-imgui-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvista-imgui
-Version: 0.1.1
+Version: 0.2.0
 Summary: Pyvista imgui integration
 Author-email: Felix Igelbrink <felix.igelbrink@dfki.de>
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mortacious/pyvista-imgui/issues
 Project-URL: Source Code, https://github.com/mortacious/pyvista-imgui
 Keywords: vtk,imgui,plotting
 Classifier: Development Status :: 4 - Beta
@@ -15,42 +15,52 @@
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: imgui-bundle
+Provides-Extra: imgui
 License-File: LICENSE
 
 # Pyvista-Imgui
 
 [![PyPi license](https://badgen.net/pypi/license/pyvista-imgui/)](https://pypi.org/project/pyvista-imgui/) [![PyPi version](https://badgen.net/pypi/v/pyvista-imgui/)](https://pypi.org/project/pyvista-imgui/)
 
 `pyvista-imgui` is a small helper module for the [`pyvista`](https://github.com/pyvista/pyvista)-package to integrate it with the [imgui](https://github.com/ocornut/imgui)-library. 
 
-It integrates a fully interactive `pyvista`-Plotter as an imgui-widget, by utilizing VTK's `vtkGenericOpenGLRenderWindow` to first render the output into an OpenGL texture and displaying it as a regular imgui-Image widget.
+It integrates a fully interactive `pyvista`-Plotter as an imgui-widget, by utilizing VTK's `vtkGenericOpenGLRenderWindow` to first render the output into an OpenGL texture and displaying it as a regular imgui-image widget.
 
-It currently utilizes the bindings provided by [`imgui-bundle`](https://github.com/ocornut/imgui), but the integration of other imgui-bindings is planned for a future release.
+It currently utilizes either the bindings provided by [`imgui-bundle`](https://github.com/ocornut/imgui), or by [`pyimgui`](https://github.com/pyimgui/pyimgui/tree/master).
 
 This package is considered experimental at this moment, so expect issues.
 
 ## Installation5
 
 To install this package using `pip` use:
 
 ```bash
-pip install pyvista-imgui
+pip install pyvista-imgui[imgui-bundle]
 ```
 
+for the `imgui-bundle` bindings or:
+
+```bash
+pip install pyvista-imgui[imgui]
+```
+
+for the `pyimgui` bindings.
+
 Alternatively the installation from source is also possible with:
 
 ```bash
 git clone https://github.com/mortacious/pyvista-imgui
 cd pyvista-imgui
-pip install [-e] .
+pip install [-e] .[imgui-bundle / imgui] 
 ```
 
 ## Usage
 
 The package includes the class `ImguiPlotter`, which can be used as a drop-in alternative to the regular `pyvista`-plotters:
 
 ```py
@@ -61,15 +71,15 @@
 
 plotter = ImguiPlotter()
 plotter.add_axes()
 plotter.add_mesh(sphere)
 plotter.show()
 ```
 
-Alternatively, an instance of `ImguiPlotter` can be integrated into an existing `imgui`-UI as a widget:
+Alternatively, an instance of `ImguiPlotter` can be integrated into an existing imgui-UI as a widget:
 
 ```py
 imgui.begin("Imgui Plotter")
 # render the plotter's contents here
 plotter.render()
 imgui.end()
 ```
```

### Comparing `pyvista-imgui-0.1.1/README.md` & `pyvista-imgui-0.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 # Pyvista-Imgui
 
 [![PyPi license](https://badgen.net/pypi/license/pyvista-imgui/)](https://pypi.org/project/pyvista-imgui/) [![PyPi version](https://badgen.net/pypi/v/pyvista-imgui/)](https://pypi.org/project/pyvista-imgui/)
 
 `pyvista-imgui` is a small helper module for the [`pyvista`](https://github.com/pyvista/pyvista)-package to integrate it with the [imgui](https://github.com/ocornut/imgui)-library. 
 
-It integrates a fully interactive `pyvista`-Plotter as an imgui-widget, by utilizing VTK's `vtkGenericOpenGLRenderWindow` to first render the output into an OpenGL texture and displaying it as a regular imgui-Image widget.
+It integrates a fully interactive `pyvista`-Plotter as an imgui-widget, by utilizing VTK's `vtkGenericOpenGLRenderWindow` to first render the output into an OpenGL texture and displaying it as a regular imgui-image widget.
 
-It currently utilizes the bindings provided by [`imgui-bundle`](https://github.com/ocornut/imgui), but the integration of other imgui-bindings is planned for a future release.
+It currently utilizes either the bindings provided by [`imgui-bundle`](https://github.com/ocornut/imgui), or by [`pyimgui`](https://github.com/pyimgui/pyimgui/tree/master).
 
 This package is considered experimental at this moment, so expect issues.
 
 ## Installation5
 
 To install this package using `pip` use:
 
 ```bash
-pip install pyvista-imgui
+pip install pyvista-imgui[imgui-bundle]
 ```
 
+for the `imgui-bundle` bindings or:
+
+```bash
+pip install pyvista-imgui[imgui]
+```
+
+for the `pyimgui` bindings.
+
 Alternatively the installation from source is also possible with:
 
 ```bash
 git clone https://github.com/mortacious/pyvista-imgui
 cd pyvista-imgui
-pip install [-e] .
+pip install [-e] .[imgui-bundle / imgui] 
 ```
 
 ## Usage
 
 The package includes the class `ImguiPlotter`, which can be used as a drop-in alternative to the regular `pyvista`-plotters:
 
 ```py
@@ -38,15 +46,15 @@
 
 plotter = ImguiPlotter()
 plotter.add_axes()
 plotter.add_mesh(sphere)
 plotter.show()
 ```
 
-Alternatively, an instance of `ImguiPlotter` can be integrated into an existing `imgui`-UI as a widget:
+Alternatively, an instance of `ImguiPlotter` can be integrated into an existing imgui-UI as a widget:
 
 ```py
 imgui.begin("Imgui Plotter")
 # render the plotter's contents here
 plotter.render()
 imgui.end()
 ```
```

### Comparing `pyvista-imgui-0.1.1/example/example_embedded.py` & `pyvista-imgui-0.2.0/example/example_embedded.py`

 * *Files identical despite different names*

### Comparing `pyvista-imgui-0.1.1/pyproject.toml` & `pyvista-imgui-0.2.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -23,20 +23,27 @@
     'Operating System :: Microsoft :: Windows',
     'Operating System :: POSIX',
     'Operating System :: MacOS',
 ]
 dependencies = [
     "pyvista>=0.39",
     'vtk', # without version
-    'imgui-bundle',
     'PyOpenGL',
     'importlib-metadata; python_version>"3.8"',
 ]
 dynamic = ["version"]
 
+[project.optional-dependencies]
+imgui-bundle = [
+  'imgui-bundle'
+]
+imgui = [
+  'imgui[glfw]'
+]
+
 [tool.setuptools_scm]
 write_to = "pyvista_imgui/_version.py"
 version_scheme = "release-branch-semver"
 
 [project.urls]
 "Bug Tracker" = 'https://github.com/mortacious/pyvista-imgui/issues'
 "Source Code" = 'https://github.com/mortacious/pyvista-imgui'
```

### Comparing `pyvista-imgui-0.1.1/pyvista_imgui/plotting.py` & `pyvista-imgui-0.2.0/pyvista_imgui/plotting.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import pyvista as pv
-from .imgui_render_window import VTKImguiRenderWindowInteractor
+from .imgui_render_window import VTKImguiRenderWindowInteractor, BACKEND_IMGUI_BUNDLE, BACKEND_PYIMGUI
 from pyvista import global_theme
 from pyvista.plotting.render_window_interactor import RenderWindowInteractor
 import typing as typ
 from functools import wraps
 
-
 __all__ = ['ImguiPlotter']
 
 
 class ImguiPlotter(VTKImguiRenderWindowInteractor, pv.BasePlotter):
     """
     This class extends pyvista's BasePlotter making it available
     as a DearImGui widget. 
@@ -68,27 +67,25 @@
                     renderer.enable_depth_peeling()
 
         self._setup_interactor()
 
         # Set some private attributes that let BasePlotter know
         # that this is safely rendering
         self._first_time = False  # Crucial!
-    
 
     def _setup_interactor(self) -> None:
         self.iren = RenderWindowInteractor(
             self, interactor=self.renwin.GetInteractor()
         )
         self.iren.interactor.RemoveObservers(
             "MouseMoveEvent"
         )  # slows window update?
         self.iren.initialize()
         self.enable_trackball_style()
 
-
     def __del__(self):
         # We have to check here if the plotter was only partially initialized
         self.deep_clean()
         if self._initialized:
             del self.renderers
 
     def close(self, render=False):
@@ -142,14 +139,112 @@
     def add_actor(self, *args, **kwargs):
         """
         Override to ignore the 'render' argument
         """
         kwargs["render"] = False # never render as this is not controlled by vtk any more
         pv.BasePlotter.add_actor(self, *args, **kwargs)
 
+    def _show_imgui_bundle(self, 
+                           title: typ.Optional[str] = None, 
+                           window_size: tuple[int, int] = (1400, 1080)):
+        """
+        show method for the imgui-bundle package.
+
+        Parameters
+        ----------
+        title, optional
+            The title of the window, if None, a default title is used.
+        window_size, optional
+            The size of the displayed window, by default (1400, 1080)
+        """
+
+        from imgui_bundle import immapp, hello_imgui, imgui     
+        runner_params = hello_imgui.RunnerParams()
+        runner_params.app_window_params.window_title = title or "ImguiPlotter"
+        runner_params.app_window_params.window_geometry.size = window_size
+        runner_params.imgui_window_params.show_status_bar = True
+
+        def gui():
+            hello_imgui.apply_theme(hello_imgui.ImGuiTheme_.imgui_colors_dark)
+            vec = imgui.get_main_viewport().pos
+            imgui.set_next_window_pos(vec, imgui.Cond_.once)
+            imgui.set_next_window_size(imgui.get_main_viewport().size)
+            imgui.set_next_window_bg_alpha(1.0)
+            imgui.begin("Vtk Viewer", flags=imgui.WindowFlags_.no_bring_to_front_on_focus | imgui.WindowFlags_.no_title_bar | imgui.WindowFlags_.no_decoration | imgui.WindowFlags_.no_resize | imgui.WindowFlags_.no_move)
+            self.render()
+            imgui.end()
+
+        runner_params.callbacks.show_gui = gui
+        runner_params.imgui_window_params.default_imgui_window_type = hello_imgui.DefaultImGuiWindowType.no_default_window
+        immapp.run(runner_params=runner_params)
+
+    def _show_pyimgui(self,
+                      title: typ.Optional[str] = None, 
+                      window_size: tuple[int, int] = (1400, 1080)):
+        """
+        Show method for the pyimgui package
+
+        Parameters
+        ----------
+        title, optional
+            The title of the window, if None, a default title is used.
+        window_size, optional
+            The size of the displayed window, by default (1400, 1080)
+        """
+        import glfw
+        import OpenGL.GL as GL
+        import imgui
+        from imgui.integrations.glfw import GlfwRenderer
+
+        if not glfw.init():
+            raise ValueError("Could not initialize OpenGL context")
+
+        # Create a window and its OpenGL context
+        window = glfw.create_window(int(window_size[0]), int(window_size[1]), title or "ImguiPlotter", None, None)
+        glfw.make_context_current(window)
+
+        if not window:
+            glfw.terminate()
+            raise ValueError("Could not initialize Window")
+        
+        background_color = (0.0, 0.0, 0.0, 1.0)
+        GL.glClearColor(*background_color)
+        imgui.create_context()
+
+        impl = GlfwRenderer(window)
+
+        while not glfw.window_should_close(window):
+            glfw.poll_events()
+            impl.process_inputs()
+            imgui.new_frame()
+            vec = imgui.get_main_viewport().pos
+            imgui.set_next_window_position(vec.x, vec.y, imgui.ONCE)
+            size = imgui.get_main_viewport().size
+            imgui.set_next_window_size(size.x, size.y)
+            imgui.set_next_window_bg_alpha(1.0)
+            window_flags = imgui.WINDOW_NO_BRING_TO_FRONT_ON_FOCUS | \
+                           imgui.WINDOW_NO_TITLE_BAR | \
+                           imgui.WINDOW_NO_DECORATION | \
+                           imgui.WINDOW_NO_RESIZE | \
+                           imgui.WINDOW_NO_MOVE
+                                 
+            imgui.begin("Vtk Viewer", flags=window_flags)
+            self.render()
+            imgui.end()
+
+            imgui.render()
+
+            GL.glClearColor(*background_color)
+            GL.glClear(GL.GL_COLOR_BUFFER_BIT)
+            impl.render(imgui.get_draw_data())
+            glfw.swap_buffers(window)
+
+        impl.shutdown()
+        glfw.terminate()
+
     def show(self, 
              title: typ.Optional[str] = None, 
              window_size: tuple[int, int] = (1400, 1080),
              before_close_callback: typ.Optional[typ.Callable] = None,
             **kwargs):
         """
         Show this plotter as a standalone imgui application. This call blocks until
@@ -168,27 +263,11 @@
         kwargs: Exists to ensure compatiblity with the BasePlotter interface. 
                 Any additional keywords are ignored for this plotter.
         """
         if before_close_callback is None:
             before_close_callback = global_theme._before_close_callback
         self._before_close_callback = before_close_callback
 
-
-        from imgui_bundle import immapp, imgui, hello_imgui     
-        runner_params = hello_imgui.RunnerParams()
-        runner_params.app_window_params.window_title = title or "ImguiPlotter"
-        runner_params.app_window_params.window_geometry.size = window_size
-        runner_params.imgui_window_params.show_status_bar = True
-
-        def gui():
-            hello_imgui.apply_theme(hello_imgui.ImGuiTheme_.imgui_colors_dark)
-            vec = imgui.get_main_viewport().pos
-            imgui.set_next_window_pos(vec, imgui.Cond_.once)
-            imgui.set_next_window_size(imgui.get_main_viewport().size)
-            imgui.set_next_window_bg_alpha(1.0)
-            imgui.begin("Vtk Viewer", flags=imgui.WindowFlags_.no_bring_to_front_on_focus | imgui.WindowFlags_.no_title_bar | imgui.WindowFlags_.no_decoration | imgui.WindowFlags_.no_resize | imgui.WindowFlags_.no_move)
-            self.render()
-            imgui.end()
-
-        runner_params.callbacks.show_gui = gui
-        runner_params.imgui_window_params.default_imgui_window_type = hello_imgui.DefaultImGuiWindowType.no_default_window
-        immapp.run(runner_params=runner_params)
+        if self.imgui_backed == BACKEND_IMGUI_BUNDLE:
+            self._show_imgui_bundle(title=title, window_size=window_size)
+        else:
+            self._show_pyimgui(title=title, window_size=window_size)
```

### Comparing `pyvista-imgui-0.1.1/pyvista_imgui/texture_render_window.py` & `pyvista-imgui-0.2.0/pyvista_imgui/texture_render_window.py`

 * *Files identical despite different names*

### Comparing `pyvista-imgui-0.1.1/pyvista_imgui.egg-info/PKG-INFO` & `pyvista-imgui-0.2.0/pyvista_imgui.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvista-imgui
-Version: 0.1.1
+Version: 0.2.0
 Summary: Pyvista imgui integration
 Author-email: Felix Igelbrink <felix.igelbrink@dfki.de>
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mortacious/pyvista-imgui/issues
 Project-URL: Source Code, https://github.com/mortacious/pyvista-imgui
 Keywords: vtk,imgui,plotting
 Classifier: Development Status :: 4 - Beta
@@ -15,42 +15,52 @@
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: imgui-bundle
+Provides-Extra: imgui
 License-File: LICENSE
 
 # Pyvista-Imgui
 
 [![PyPi license](https://badgen.net/pypi/license/pyvista-imgui/)](https://pypi.org/project/pyvista-imgui/) [![PyPi version](https://badgen.net/pypi/v/pyvista-imgui/)](https://pypi.org/project/pyvista-imgui/)
 
 `pyvista-imgui` is a small helper module for the [`pyvista`](https://github.com/pyvista/pyvista)-package to integrate it with the [imgui](https://github.com/ocornut/imgui)-library. 
 
-It integrates a fully interactive `pyvista`-Plotter as an imgui-widget, by utilizing VTK's `vtkGenericOpenGLRenderWindow` to first render the output into an OpenGL texture and displaying it as a regular imgui-Image widget.
+It integrates a fully interactive `pyvista`-Plotter as an imgui-widget, by utilizing VTK's `vtkGenericOpenGLRenderWindow` to first render the output into an OpenGL texture and displaying it as a regular imgui-image widget.
 
-It currently utilizes the bindings provided by [`imgui-bundle`](https://github.com/ocornut/imgui), but the integration of other imgui-bindings is planned for a future release.
+It currently utilizes either the bindings provided by [`imgui-bundle`](https://github.com/ocornut/imgui), or by [`pyimgui`](https://github.com/pyimgui/pyimgui/tree/master).
 
 This package is considered experimental at this moment, so expect issues.
 
 ## Installation5
 
 To install this package using `pip` use:
 
 ```bash
-pip install pyvista-imgui
+pip install pyvista-imgui[imgui-bundle]
 ```
 
+for the `imgui-bundle` bindings or:
+
+```bash
+pip install pyvista-imgui[imgui]
+```
+
+for the `pyimgui` bindings.
+
 Alternatively the installation from source is also possible with:
 
 ```bash
 git clone https://github.com/mortacious/pyvista-imgui
 cd pyvista-imgui
-pip install [-e] .
+pip install [-e] .[imgui-bundle / imgui] 
 ```
 
 ## Usage
 
 The package includes the class `ImguiPlotter`, which can be used as a drop-in alternative to the regular `pyvista`-plotters:
 
 ```py
@@ -61,15 +71,15 @@
 
 plotter = ImguiPlotter()
 plotter.add_axes()
 plotter.add_mesh(sphere)
 plotter.show()
 ```
 
-Alternatively, an instance of `ImguiPlotter` can be integrated into an existing `imgui`-UI as a widget:
+Alternatively, an instance of `ImguiPlotter` can be integrated into an existing imgui-UI as a widget:
 
 ```py
 imgui.begin("Imgui Plotter")
 # render the plotter's contents here
 plotter.render()
 imgui.end()
 ```
```

### Comparing `pyvista-imgui-0.1.1/pyvista_imgui.egg-info/SOURCES.txt` & `pyvista-imgui-0.2.0/pyvista_imgui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

