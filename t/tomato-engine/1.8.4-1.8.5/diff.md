# Comparing `tmp/tomato-engine-1.8.4.tar.gz` & `tmp/tomato-engine-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomato-engine-1.8.4.tar", last modified: Tue May  9 12:32:31 2023, max compression
+gzip compressed data, was "tomato-engine-1.8.5.tar", last modified: Fri Jun  2 03:34:01 2023, max compression
```

## Comparing `tomato-engine-1.8.4.tar` & `tomato-engine-1.8.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 12:32:31.950858 tomato-engine-1.8.4/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)    35149 2022-05-23 23:00:31.000000 tomato-engine-1.8.4/LICENSE
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3049 2023-05-09 12:32:31.950858 tomato-engine-1.8.4/PKG-INFO
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2417 2022-10-20 06:23:30.000000 tomato-engine-1.8.4/README.md
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       61 2022-05-23 23:00:31.000000 tomato-engine-1.8.4/pyproject.toml
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      836 2023-05-09 12:32:31.950858 tomato-engine-1.8.4/setup.cfg
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1009 2023-05-04 22:54:50.000000 tomato-engine-1.8.4/setup.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 12:32:31.942858 tomato-engine-1.8.4/src/
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 12:32:31.942858 tomato-engine-1.8.4/src/tomato/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      116 2023-05-08 19:51:10.000000 tomato-engine-1.8.4/src/tomato/__init__.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 12:32:31.946858 tomato-engine-1.8.4/src/tomato/classes/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       93 2023-05-08 19:52:06.000000 tomato-engine-1.8.4/src/tomato/classes/__init__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)    10952 2022-10-20 06:23:30.000000 tomato-engine-1.8.4/src/tomato/classes/board.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)    13921 2022-10-20 06:23:30.000000 tomato-engine-1.8.4/src/tomato/classes/cell.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4569 2023-05-03 22:45:39.000000 tomato-engine-1.8.4/src/tomato/classes/cellmatrix.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3621 2023-05-08 19:51:41.000000 tomato-engine-1.8.4/src/tomato/classes/window.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 12:32:31.946858 tomato-engine-1.8.4/src/tomato/functions/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2022-05-23 23:00:31.000000 tomato-engine-1.8.4/src/tomato/functions/__init__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      842 2022-06-20 19:13:20.000000 tomato-engine-1.8.4/src/tomato/functions/display.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4192 2022-07-06 18:41:02.000000 tomato-engine-1.8.4/src/tomato/functions/file_io.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4163 2022-10-20 06:23:30.000000 tomato-engine-1.8.4/src/tomato/functions/utils.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 12:32:31.950858 tomato-engine-1.8.4/src/tomato/rules/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2022-05-23 23:00:31.000000 tomato-engine-1.8.4/src/tomato/rules/__init__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      660 2022-10-20 06:23:30.000000 tomato-engine-1.8.4/src/tomato/rules/colorful.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      273 2022-10-20 06:23:30.000000 tomato-engine-1.8.4/src/tomato/rules/colorful_demo.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      912 2022-10-20 06:23:30.000000 tomato-engine-1.8.4/src/tomato/rules/cyclic.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      316 2022-10-20 06:23:30.000000 tomato-engine-1.8.4/src/tomato/rules/cyclic_demo.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      872 2023-05-04 22:48:21.000000 tomato-engine-1.8.4/src/tomato/rules/game_of_life.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      274 2022-10-20 06:23:30.000000 tomato-engine-1.8.4/src/tomato/rules/game_of_life_demo.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      759 2022-10-20 06:23:30.000000 tomato-engine-1.8.4/src/tomato/rules/toothpick_fractal.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      297 2023-04-27 23:43:06.000000 tomato-engine-1.8.4/src/tomato/rules/toothpick_fractal_demo.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 12:32:31.950858 tomato-engine-1.8.4/src/tomato_engine.egg-info/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3049 2023-05-09 12:32:31.000000 tomato-engine-1.8.4/src/tomato_engine.egg-info/PKG-INFO
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      856 2023-05-09 12:32:31.000000 tomato-engine-1.8.4/src/tomato_engine.egg-info/SOURCES.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-05-09 12:32:31.000000 tomato-engine-1.8.4/src/tomato_engine.egg-info/dependency_links.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       53 2023-05-09 12:32:31.000000 tomato-engine-1.8.4/src/tomato_engine.egg-info/requires.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        7 2023-05-09 12:32:31.000000 tomato-engine-1.8.4/src/tomato_engine.egg-info/top_level.txt
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-02 03:34:01.003161 tomato-engine-1.8.5/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)    35149 2022-05-23 23:00:31.000000 tomato-engine-1.8.5/LICENSE
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3049 2023-06-02 03:34:01.003161 tomato-engine-1.8.5/PKG-INFO
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2417 2022-10-20 06:23:30.000000 tomato-engine-1.8.5/README.md
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       61 2022-05-23 23:00:31.000000 tomato-engine-1.8.5/pyproject.toml
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      836 2023-06-02 03:34:01.003161 tomato-engine-1.8.5/setup.cfg
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1009 2023-06-02 03:29:46.000000 tomato-engine-1.8.5/setup.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-02 03:34:00.999160 tomato-engine-1.8.5/src/
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-02 03:34:00.999160 tomato-engine-1.8.5/src/tomato/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      116 2023-05-08 19:51:10.000000 tomato-engine-1.8.5/src/tomato/__init__.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-02 03:34:01.003161 tomato-engine-1.8.5/src/tomato/classes/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       93 2023-05-08 19:52:06.000000 tomato-engine-1.8.5/src/tomato/classes/__init__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)    10952 2022-10-20 06:23:30.000000 tomato-engine-1.8.5/src/tomato/classes/board.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)    13921 2022-10-20 06:23:30.000000 tomato-engine-1.8.5/src/tomato/classes/cell.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5109 2023-06-02 03:25:30.000000 tomato-engine-1.8.5/src/tomato/classes/cellmatrix.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3621 2023-05-08 19:51:41.000000 tomato-engine-1.8.5/src/tomato/classes/window.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-02 03:34:01.003161 tomato-engine-1.8.5/src/tomato/functions/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2022-05-23 23:00:31.000000 tomato-engine-1.8.5/src/tomato/functions/__init__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      842 2022-06-20 19:13:20.000000 tomato-engine-1.8.5/src/tomato/functions/display.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4192 2022-07-06 18:41:02.000000 tomato-engine-1.8.5/src/tomato/functions/file_io.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4163 2022-10-20 06:23:30.000000 tomato-engine-1.8.5/src/tomato/functions/utils.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-02 03:34:01.003161 tomato-engine-1.8.5/src/tomato/rules/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2022-05-23 23:00:31.000000 tomato-engine-1.8.5/src/tomato/rules/__init__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      660 2022-10-20 06:23:30.000000 tomato-engine-1.8.5/src/tomato/rules/colorful.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      273 2022-10-20 06:23:30.000000 tomato-engine-1.8.5/src/tomato/rules/colorful_demo.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      912 2023-05-13 01:05:56.000000 tomato-engine-1.8.5/src/tomato/rules/cyclic.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      316 2022-10-20 06:23:30.000000 tomato-engine-1.8.5/src/tomato/rules/cyclic_demo.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      872 2023-05-04 22:48:21.000000 tomato-engine-1.8.5/src/tomato/rules/game_of_life.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      274 2022-10-20 06:23:30.000000 tomato-engine-1.8.5/src/tomato/rules/game_of_life_demo.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      759 2023-05-13 01:06:01.000000 tomato-engine-1.8.5/src/tomato/rules/toothpick_fractal.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      297 2023-04-27 23:43:06.000000 tomato-engine-1.8.5/src/tomato/rules/toothpick_fractal_demo.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-06-02 03:34:01.003161 tomato-engine-1.8.5/src/tomato_engine.egg-info/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3049 2023-06-02 03:34:00.000000 tomato-engine-1.8.5/src/tomato_engine.egg-info/PKG-INFO
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      856 2023-06-02 03:34:00.000000 tomato-engine-1.8.5/src/tomato_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-06-02 03:34:00.000000 tomato-engine-1.8.5/src/tomato_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       53 2023-06-02 03:34:00.000000 tomato-engine-1.8.5/src/tomato_engine.egg-info/requires.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        7 2023-06-02 03:34:00.000000 tomato-engine-1.8.5/src/tomato_engine.egg-info/top_level.txt
```

### Comparing `tomato-engine-1.8.4/LICENSE` & `tomato-engine-1.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.4/PKG-INFO` & `tomato-engine-1.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomato-engine
-Version: 1.8.4
+Version: 1.8.5
 Summary: Engine for prototyping and playing with cellular automata
 Home-page: https://codeberg.org/eduardotogpi/tomato-engine
 Author: Eduardo Lopes Dias, Murilo Melhem
 Author-email: eduardosprp@usp.br
 Project-URL: Bug Tracker, https://codeberg.org/eduardotogpi/tomato-engine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `tomato-engine-1.8.4/README.md` & `tomato-engine-1.8.5/README.md`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.4/setup.cfg` & `tomato-engine-1.8.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tomato-engine
-version = 1.8.4
+version = 1.8.5
 author = Eduardo Lopes Dias, Murilo Melhem
 author_email = eduardotogpi@usp.br
 description = Engine for prototyping and playing with cellular automata.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://codeberg.org/eduardotogpi/tomato-engine
 project_urls =
```

### Comparing `tomato-engine-1.8.4/setup.py` & `tomato-engine-1.8.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tomato-engine",
-    version="1.8.4",
+    version="1.8.5",
     author="Eduardo Lopes Dias, Murilo Melhem",
     author_email="eduardosprp@usp.br",
     description="Engine for prototyping and playing with cellular automata",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://codeberg.org/eduardotogpi/tomato-engine",
     project_urls={
```

### Comparing `tomato-engine-1.8.4/src/tomato/classes/board.py` & `tomato-engine-1.8.5/src/tomato/classes/board.py`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.4/src/tomato/classes/cell.py` & `tomato-engine-1.8.5/src/tomato/classes/cell.py`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.4/src/tomato/classes/cellmatrix.py` & `tomato-engine-1.8.5/src/tomato/classes/cellmatrix.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,32 +7,57 @@
 from .cell import CellTemplate
 
 """
 Estrutura de dados para a matriz que contém todos os autômatos.
 """
 
 
+def cell_from_rule(rule):
+    # {{{
+    """
+    A regra pode ser um módulo de Python contendo uma classe que herda de CellTemplate,
+    ou a própria classe. Esta função existe para que as demais funções deste módulo se
+    adequem a estes requisitos.
+    """
+
+    if rule in CellTemplate.__subclasses__():
+        return rule
+    elif isinstance(rule, ModuleType):
+        for name in dir(rule):
+            try:
+                attribute = rule.__dict__[name]
+                return cell_from_rule(attribute)
+            except TypeError:
+                pass
+
+        raise TypeError(
+            f"Tipo {type(rule)} inválido para o parâmetro rule. "
+            "Tipos válidos são 'CellTemplate' e 'module'"
+        )
+
+    else:
+        raise TypeError(
+            f"Tipo {type(rule)} inválido para o parâmetro rule. "
+            "Tipos válidos são 'CellTemplate' e 'module'"
+        )
+
+
+# }}}
+
+
 class CellMatrix:
     # {{{
     def __init__(self, state_matrix, rule, cell_args=None):
         # {{{
         """
         Cria a matriz de autômatos a partir de uma regra e a
         matriz de estado inicial.
         """
 
-        if isinstance(rule, ModuleType):
-            self.Cell = rule.Cell
-        elif rule in CellTemplate.__subclasses__():
-            self.Cell = rule
-        else:
-            raise TypeError(
-                f"Tipo {type(rule)} inválido para o parâmetro rule. "
-                "Tipos válidos são 'Cell' e 'module'"
-            )
+        self.Cell = cell_from_rule(rule)
 
         self.state_matrix = state_matrix.copy()
 
         if cell_args is not None:
             self.cell_matrix = np.array(
                 [
                     self.Cell(value, (lin_num, col_num), cell_args)
@@ -58,19 +83,18 @@
         # {{{
         """
         Inicializa a partir da matriz de valores RGB ou valor de
         escala monocromática extraídos de uma imagem. Essa
         provavelmente é a maneira mais lenta possível de se fazer
         isso.
         """
+    
+        cell = cell_from_rule(rule)
 
-        # Ugliest hack I've ever seen in my life
-        rule.Cell.simulation_start(display_matrix, cell_args)
-
-        cell_from_display = rule.Cell.from_display
+        cell_from_display = cell.from_display
         pixels_gen = (cell_from_display(col) for lin in display_matrix for col in lin)
 
         state_matrix = np.array(list(pixels_gen))
         state_matrix = state_matrix.reshape(display_matrix.shape[:2])
 
         return cls(state_matrix, rule, cell_args)
```

### Comparing `tomato-engine-1.8.4/src/tomato/classes/window.py` & `tomato-engine-1.8.5/src/tomato/classes/window.py`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.4/src/tomato/functions/display.py` & `tomato-engine-1.8.5/src/tomato/functions/display.py`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.4/src/tomato/functions/file_io.py` & `tomato-engine-1.8.5/src/tomato/functions/file_io.py`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.4/src/tomato/functions/utils.py` & `tomato-engine-1.8.5/src/tomato/functions/utils.py`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.4/src/tomato/rules/colorful.py` & `tomato-engine-1.8.5/src/tomato/rules/colorful.py`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.4/src/tomato/rules/cyclic.py` & `tomato-engine-1.8.5/src/tomato/rules/cyclic.py`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.4/src/tomato/rules/game_of_life.py` & `tomato-engine-1.8.5/src/tomato/rules/game_of_life.py`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.4/src/tomato/rules/toothpick_fractal.py` & `tomato-engine-1.8.5/src/tomato/rules/toothpick_fractal.py`

 * *Files identical despite different names*

### Comparing `tomato-engine-1.8.4/src/tomato_engine.egg-info/PKG-INFO` & `tomato-engine-1.8.5/src/tomato_engine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomato-engine
-Version: 1.8.4
+Version: 1.8.5
 Summary: Engine for prototyping and playing with cellular automata
 Home-page: https://codeberg.org/eduardotogpi/tomato-engine
 Author: Eduardo Lopes Dias, Murilo Melhem
 Author-email: eduardosprp@usp.br
 Project-URL: Bug Tracker, https://codeberg.org/eduardotogpi/tomato-engine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `tomato-engine-1.8.4/src/tomato_engine.egg-info/SOURCES.txt` & `tomato-engine-1.8.5/src/tomato_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

