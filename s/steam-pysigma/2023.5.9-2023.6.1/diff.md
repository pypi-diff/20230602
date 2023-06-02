# Comparing `tmp/steam-pysigma-2023.5.9.tar.gz` & `tmp/steam-pysigma-2023.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\steam-pysigma-2023.5.9.tar", last modified: Mon May 15 09:46:05 2023, max compression
+gzip compressed data, was "dist\steam-pysigma-2023.6.1.tar", last modified: Fri Jun  2 07:22:27 2023, max compression
```

## Comparing `steam-pysigma-2023.5.9.tar` & `steam-pysigma-2023.6.1.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 09:46:05.008297 steam-pysigma-2023.5.9/
--rw-rw-rw-   0        0        0     1030 2023-05-15 09:46:05.007296 steam-pysigma-2023.5.9/PKG-INFO
--rw-rw-rw-   0        0        0      616 2023-02-22 13:16:40.000000 steam-pysigma-2023.5.9/README.md
--rw-rw-rw-   0        0        0       42 2023-05-15 09:46:05.008297 steam-pysigma-2023.5.9/setup.cfg
--rw-rw-rw-   0        0        0      897 2023-05-15 09:38:17.000000 steam-pysigma-2023.5.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:46:04.965543 steam-pysigma-2023.5.9/steam_pysigma/
--rw-rw-rw-   0        0        0     2302 2023-05-15 09:37:50.000000 steam-pysigma-2023.5.9/steam_pysigma/MainSIGMA.py
--rw-rw-rw-   0        0        0        0 2023-02-02 13:16:25.000000 steam-pysigma-2023.5.9/steam_pysigma/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:46:04.980862 steam-pysigma-2023.5.9/steam_pysigma/comsol/
--rw-rw-rw-   0        0        0    14494 2023-05-15 09:35:20.000000 steam-pysigma-2023.5.9/steam_pysigma/comsol/BuildComsolModel.py
--rw-rw-rw-   0        0        0    14785 2023-05-09 13:02:54.000000 steam-pysigma-2023.5.9/steam_pysigma/comsol/BuildGlobalVariables.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.5.9/steam_pysigma/comsol/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:46:04.987007 steam-pysigma-2023.5.9/steam_pysigma/data/
--rw-rw-rw-   0        0        0     7899 2023-03-21 08:33:21.000000 steam-pysigma-2023.5.9/steam_pysigma/data/DataRoxieParser.py
--rw-rw-rw-   0        0        0     7220 2023-05-09 12:57:42.000000 steam-pysigma-2023.5.9/steam_pysigma/data/DataSIGMA.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.5.9/steam_pysigma/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:46:04.990007 steam-pysigma-2023.5.9/steam_pysigma/domain_generator/
--rw-rw-rw-   0        0        0    17382 2023-05-04 09:30:11.000000 steam-pysigma-2023.5.9/steam_pysigma/domain_generator/GeometryMultipole.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.5.9/steam_pysigma/domain_generator/__init__.py
--rw-rw-rw-   0        0        0    12500 2023-04-21 07:21:40.000000 steam-pysigma-2023.5.9/steam_pysigma/helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:46:04.993007 steam-pysigma-2023.5.9/steam_pysigma/parsers/
--rw-rw-rw-   0        0        0     1673 2023-05-02 10:05:01.000000 steam-pysigma-2023.5.9/steam_pysigma/parsers/ParserRoxie.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.5.9/steam_pysigma/parsers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:46:04.995007 steam-pysigma-2023.5.9/steam_pysigma/plotters/
--rw-rw-rw-   0        0        0    17437 2023-05-08 12:35:29.000000 steam-pysigma-2023.5.9/steam_pysigma/plotters/PlotterPysigma.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.5.9/steam_pysigma/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:46:04.998139 steam-pysigma-2023.5.9/steam_pysigma/postprocessing/
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.5.9/steam_pysigma/postprocessing/__init__.py
--rw-rw-rw-   0        0        0     3077 2023-05-08 12:18:35.000000 steam-pysigma-2023.5.9/steam_pysigma/postprocessing/postprocessing.py
--rw-rw-rw-   0        0        0    10147 2023-04-27 07:07:05.000000 steam-pysigma-2023.5.9/steam_pysigma/pysigma.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:46:05.005139 steam-pysigma-2023.5.9/steam_pysigma/utils/
--rw-rw-rw-   0        0        0     1945 2023-05-08 12:45:36.000000 steam-pysigma-2023.5.9/steam_pysigma/utils/Util.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.5.9/steam_pysigma/utils/__init__.py
--rw-rw-rw-   0        0        0      299 2022-11-02 10:29:42.000000 steam-pysigma-2023.5.9/steam_pysigma/utils/make_folder_if_not_existing.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:46:04.975652 steam-pysigma-2023.5.9/steam_pysigma.egg-info/
--rw-rw-rw-   0        0        0     1030 2023-05-15 09:46:01.000000 steam-pysigma-2023.5.9/steam_pysigma.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      966 2023-05-15 09:46:01.000000 steam-pysigma-2023.5.9/steam_pysigma.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 09:46:01.000000 steam-pysigma-2023.5.9/steam_pysigma.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      220 2023-05-15 09:46:01.000000 steam-pysigma-2023.5.9/steam_pysigma.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-15 09:46:01.000000 steam-pysigma-2023.5.9/steam_pysigma.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 07:22:27.712811 steam-pysigma-2023.6.1/
+-rw-rw-rw-   0        0        0     1030 2023-06-02 07:22:27.711811 steam-pysigma-2023.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0      616 2023-02-22 13:16:40.000000 steam-pysigma-2023.6.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-02 07:22:27.712811 steam-pysigma-2023.6.1/setup.cfg
+-rw-rw-rw-   0        0        0      897 2023-06-02 07:21:36.000000 steam-pysigma-2023.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 07:22:27.672141 steam-pysigma-2023.6.1/steam_pysigma/
+-rw-rw-rw-   0        0        0     2861 2023-05-23 07:10:27.000000 steam-pysigma-2023.6.1/steam_pysigma/MainSIGMA.py
+-rw-rw-rw-   0        0        0        0 2023-02-02 13:16:25.000000 steam-pysigma-2023.6.1/steam_pysigma/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 07:22:27.685712 steam-pysigma-2023.6.1/steam_pysigma/comsol/
+-rw-rw-rw-   0        0        0    17426 2023-05-25 12:24:48.000000 steam-pysigma-2023.6.1/steam_pysigma/comsol/BuildComsolModel.py
+-rw-rw-rw-   0        0        0    15166 2023-05-24 08:17:29.000000 steam-pysigma-2023.6.1/steam_pysigma/comsol/BuildGlobalVariables.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.1/steam_pysigma/comsol/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 07:22:27.692395 steam-pysigma-2023.6.1/steam_pysigma/data/
+-rw-rw-rw-   0        0        0     8068 2023-05-25 12:15:47.000000 steam-pysigma-2023.6.1/steam_pysigma/data/DataRoxieParser.py
+-rw-rw-rw-   0        0        0     7220 2023-06-01 09:48:39.000000 steam-pysigma-2023.6.1/steam_pysigma/data/DataSIGMA.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.1/steam_pysigma/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 07:22:27.694394 steam-pysigma-2023.6.1/steam_pysigma/domain_generator/
+-rw-rw-rw-   0        0        0    17229 2023-05-25 12:09:39.000000 steam-pysigma-2023.6.1/steam_pysigma/domain_generator/GeometryMultipole.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.1/steam_pysigma/domain_generator/__init__.py
+-rw-rw-rw-   0        0        0    12500 2023-04-21 07:21:40.000000 steam-pysigma-2023.6.1/steam_pysigma/helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-02 07:22:27.697395 steam-pysigma-2023.6.1/steam_pysigma/parsers/
+-rw-rw-rw-   0        0        0     1975 2023-05-25 12:04:31.000000 steam-pysigma-2023.6.1/steam_pysigma/parsers/ParserRoxie.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.1/steam_pysigma/parsers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 07:22:27.701505 steam-pysigma-2023.6.1/steam_pysigma/plotters/
+-rw-rw-rw-   0        0        0    17437 2023-05-08 12:35:29.000000 steam-pysigma-2023.6.1/steam_pysigma/plotters/PlotterPysigma.py
+-rw-rw-rw-   0        0        0     8879 2023-05-22 07:52:03.000000 steam-pysigma-2023.6.1/steam_pysigma/plotters/PlotterRoxie.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.1/steam_pysigma/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 07:22:27.705504 steam-pysigma-2023.6.1/steam_pysigma/postprocessing/
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.1/steam_pysigma/postprocessing/__init__.py
+-rw-rw-rw-   0        0        0     3077 2023-05-08 12:18:35.000000 steam-pysigma-2023.6.1/steam_pysigma/postprocessing/postprocessing.py
+-rw-rw-rw-   0        0        0    10147 2023-04-27 07:07:05.000000 steam-pysigma-2023.6.1/steam_pysigma/pysigma.py
+drwxrwxrwx   0        0        0        0 2023-06-02 07:22:27.710811 steam-pysigma-2023.6.1/steam_pysigma/utils/
+-rw-rw-rw-   0        0        0     1945 2023-05-08 12:45:36.000000 steam-pysigma-2023.6.1/steam_pysigma/utils/Util.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.1/steam_pysigma/utils/__init__.py
+-rw-rw-rw-   0        0        0      299 2022-11-02 10:29:42.000000 steam-pysigma-2023.6.1/steam_pysigma/utils/make_folder_if_not_existing.py
+drwxrwxrwx   0        0        0        0 2023-06-02 07:22:27.679710 steam-pysigma-2023.6.1/steam_pysigma.egg-info/
+-rw-rw-rw-   0        0        0     1030 2023-06-02 07:22:23.000000 steam-pysigma-2023.6.1/steam_pysigma.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1005 2023-06-02 07:22:23.000000 steam-pysigma-2023.6.1/steam_pysigma.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 07:22:23.000000 steam-pysigma-2023.6.1/steam_pysigma.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      315 2023-06-02 07:22:23.000000 steam-pysigma-2023.6.1/steam_pysigma.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-02 07:22:23.000000 steam-pysigma-2023.6.1/steam_pysigma.egg-info/top_level.txt
```

### Comparing `steam-pysigma-2023.5.9/PKG-INFO` & `steam-pysigma-2023.6.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-pysigma
-Version: 2023.5.9
+Version: 2023.6.1
 Summary: This is python wrapper of STEAM SIGMA code
 Home-page: https://gitlab.cern.ch/steam/steam_pysigma
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: SIGMA,STEAM,CERN
+Keywords: STEAM,SIGMA,CERN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM PySIGMA
```

### Comparing `steam-pysigma-2023.5.9/README.md` & `steam-pysigma-2023.6.1/README.md`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.5.9/setup.py` & `steam-pysigma-2023.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='steam-pysigma',
-    version="2023.5.9",
+    version="2023.6.1",
     author="STEAM Team",
     author_email="steam-team@cern.ch",
     description="This is python wrapper of STEAM SIGMA code",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://gitlab.cern.ch/steam/steam_pysigma",
     keywords={'STEAM', 'SIGMA', 'CERN'},
```

### Comparing `steam-pysigma-2023.5.9/steam_pysigma/comsol/BuildComsolModel.py` & `steam-pysigma-2023.6.1/steam_pysigma/comsol/BuildComsolModel.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,73 +2,90 @@
 from pathlib import Path
 
 import numpy as np
 
 from steam_pysigma.comsol.BuildGlobalVariables import BuildGlobalVariables
 from steam_pysigma import pysigma as ps
 from steam_pysigma.domain_generator.GeometryMultipole import GeometryMultipole
-
-
+from matplotlib import lines, pyplot as plt
+from steam_pysigma.plotters.PlotterPysigma import plot_multiple_areas
+from steam_pysigma.utils.Util import displayWaitAndClose
 class BuildComsolModel:
     """
     Class take in domains and a configuration and builds a functioning comsol model saved as java.
     """
 
-    def __init__(self, model_data, input_conductor_params, settings, output_path, roxie_data, bh_curve_database):
+    def __init__(self, model_data=None, input_conductor_params=None,output_path=None, settings=None,
+                 path_to_results=None, input_coordinates_path=None, roxie_data=None, bh_curve_database=None):
+        """
+        Class builds a comsol model.
+        :param model_data: data dict from magnet_name.yaml
+        :param input_conductor_params: magnet_name.set
+        :param output_path: Output path of java files and mph model.
+        :param settings: settings dict
+        :param path_to_results: location of comsol-generated results
+        :param input_coordinates_path: path to file with coordinates to evaluate B_field
+        :param roxie_data: roxie data
+        :param bh_curve_database: path to bh curve file
+        """
         self.g = ps.GatewaySIGMA()
         self.a = ps.ArraysSIGMA
         self.model_data = model_data
         self.output_path = output_path
         self.roxie_data = roxie_data.Roxie_Data
         self.settings_dict = dict(settings)
         self.input_conductor_params = input_conductor_params
         self.funlib_map = ps.FunLibCSVReader().read_csv_funclib_create_hashmap(self.g)
         self.COMSOL_exe_path = Path(self.settings_dict['comsolexe_path']).parent
         self.java_jdk_path = self.settings_dict['JAVA_jdk_path']
         self.COMSOL_compile_path = os.path.join(self.COMSOL_exe_path, 'comsolcompile.exe')  # Change os.join()
         self.COMSOL_batch_path = os.path.join(self.COMSOL_exe_path, 'comsolbatch.exe')
         self.COMSOL_version = os.path.basename(os.path.dirname(self.COMSOL_exe_path.parent.parent)).replace("COMSOL",
                                                                                                             "")
+        self.path_to_results = path_to_results if path_to_results != None else self.output_path
         self.bh_curve_database = bh_curve_database
         if self.COMSOL_version != "60" and self.COMSOL_version != "53a":
             raise Exception("Not supporting any other versions than 6.0 and 5.3a")
 
         self.model_name = f"{self.model_data.general_parameters.magnet_name}_Model"
 
         self.model_java_file_path = f"{os.path.join(self.output_path, self.model_name)}.java"
         self.compile_batch_file_path = f"{os.path.join(self.output_path, self.model_name)}_Compile_and_Open.bat"
         self.model_class_file_path = f"{os.path.join(self.output_path, self.model_name)}.class"
         self.split_java_file_path = []
         self.study_type = self.model_data.options_sigma.simulation.study_type
         self.num_qh = self.model_data.quench_protection.quench_heaters.N_strips
         self.make_batch_mode_executable = self.model_data.options_sigma.simulation.make_batch_mode_executable
         self.generate_study = self.model_data.options_sigma.simulation.generate_study
-        self.input_coordinates_path = str(self.model_data.options_sigma.postprocessing.out_2D_at_points.coordinate_source) if self.model_data.options_sigma.postprocessing.out_2D_at_points.coordinate_source!=None else None
+        self.input_coordinates_path = input_coordinates_path #str(self.model_data.options_sigma.postprocessing.out_2D_at_points.coordinate_source) if self.model_data.options_sigma.postprocessing.out_2D_at_points.coordinate_source!=None else None
 
         self.postprocessing_data = self.model_data.options_sigma.postprocessing
         self.variables2DConverted = self.postprocessing_data.out_2D_at_points.variables
         self.time2DConverted = self.postprocessing_data.out_2D_at_points.time  # List of all exported time
         self.variables1DvsTime = self.postprocessing_data.out_1D_vs_times.variables
         self.time1DConverted = self.postprocessing_data.out_1D_vs_times.time
         self.variables1DvsTimeVector = self.postprocessing_data.out_1D_vs_times.variables
         self.timeRange = ", ".join(["range(" + ", ".join(map(str, lst)) + ")" for lst in
                                     self.model_data.options_sigma.time_vector_solution.time_step])
 
         print(f"Comsol compile path {self.COMSOL_compile_path}")
         print(f"Comsol version {self.COMSOL_version}")
-
+        #bgv = BuildGlobalVariables(self.g, self.model_data)
+        #bgv.validate_sigma_model_data()
         self.cfg = self.setup_config_sigma()
         self.srv = self.g.TxtSigmaServer(self.cfg.getOutputModelPath(), self.cfg.getComsolBatchPath(),
                                          self.cfg.getComsolCompilePath())
 
-        bgv = BuildGlobalVariables(self.g, self.model_data)
-        bgv.validate_sigma_model_data()
-        geom_multipole = GeometryMultipole(self.g, self.roxie_data, model_data, self.input_conductor_params,
+
+        geom_multipole = GeometryMultipole(self.g, self.roxie_data, model_data, self.bh_curve_database, self.input_conductor_params,
                                            self.settings_dict)
+
         self.domains = geom_multipole.build_magnet()
+        self.wedge_areas = geom_multipole.wedge_areas
+        self.plot_magnet()
         self.connect_create_MPH_model(self.domains)
         self.save_files_java()
         self.save_compile_and_open_bat()
 
     def setup_config_sigma(self):
         cfg = self.g.ConfigSigma()
         cfg.setComsolVersion(self.COMSOL_version)  # for sigma_60
@@ -165,15 +182,15 @@
             builder_qh = self.g.QuenchHeaterMPHBuilder(self.cfg, self.srv)
             self.model.connectToServer()
             builder_qh.buildQuenchHeaterMPH()
         if self.generate_study:
             self.build_study()
             # Define result nodes
 
-            self.create_results(self.input_coordinates_path, self.output_path)
+            self.create_results(self.input_coordinates_path, self.path_to_results)
             self.srv.build(self.cfg.getOutputModelPath())
             self.model.save()
 
     def save_files_java(self):
         with open(self.model_java_file_path) as java_file:
 
             print("Java file splitting started.")
@@ -246,7 +263,39 @@
             f'"{self.COMSOL_batch_path}" -inputfile "{self.model_class_file_path}" '
             f'-outputfile "{os.path.join(self.output_path, self.model_data.general_parameters.magnet_name)}.mph"']
 
         with open(self.compile_batch_file_path, "w") as outfile:
             outfile.write("\n".join(str(line) for line in script_lines))
         print(f'BuilderSIGMA successfully saved: {self.compile_batch_file_path}')
         os.chdir(self.output_path)
+
+    def plot_magnet(self):
+        """
+        Plot blocks and halfturns for the roxie model data
+        :return: None
+        """
+        fig = plt.figure(figsize=(10, 10))
+        ax = plt.axes()
+        ax.set_xlim(0., 0.2)
+        ax.set_ylim(-.1, 0.1)
+        self.show_halfTurns = True
+        # p.plot_multiple_areas(ax, self.air_far_field_areas)  # air far field
+        # p.plot_multiple_areas(ax, self.air_areas)  # air
+        # p.plot_multiple_areas(ax, self.iron_yoke_areas)  # iron yoke
+        plot_multiple_areas(ax, self.wedge_areas)  # wedges
+        if self.show_halfTurns:
+            for coil_nr, coil in self.roxie_data.coil.coils.items():
+                for pole_nr, pole in coil.poles.items():
+                    for layer_nr, layer in pole.layers.items():
+                        for winding_key, winding in layer.windings.items():
+                            for block_key, block in winding.blocks.items():
+                                for halfTurn_nr, halfTurn in block.half_turns.items():
+                                    iH = halfTurn.corners.insulated.iH
+                                    iL = halfTurn.corners.insulated.iL
+                                    oH = halfTurn.corners.insulated.oH
+                                    oL = halfTurn.corners.insulated.oL
+                                    ax.add_line(lines.Line2D([iH.x, iL.x], [iH.y, iL.y], color='red'))
+                                    ax.add_line(lines.Line2D([oH.x, oL.x], [oH.y, oL.y], color='red'))
+                                    ax.add_line(lines.Line2D([oL.x, iL.x], [oL.y, iL.y], color='red'))
+                                    ax.add_line(lines.Line2D([iH.x, oH.x], [iH.y, oH.y], color='red'))
+        #p.plot_multiple_areas(ax, self.coil_areas)
+        displayWaitAndClose(waitTimeBeforeMessage=0.1, waitTimeAfterMessage=10)
```

### Comparing `steam-pysigma-2023.5.9/steam_pysigma/comsol/BuildGlobalVariables.py` & `steam-pysigma-2023.6.1/steam_pysigma/comsol/BuildGlobalVariables.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,15 @@
                 if key == "quench_stop_temp":
                     if value is None:
                         raise ValueError(f"{key} can't be none")
                     if value < 0:
                         raise ValueError("Tempereatur for initialize quench can't be negative")
 
         # Check options_sigma.postprocessing.out_2D_at_points
+        options_sigma.postprocessing.out_2D_at_points.coordinate_source = None
         for key, value in options_sigma.postprocessing.out_2D_at_points:
             if key == "coordinate_source":
                 # Check if source exists
                 if value is not None:
                     if not os.path.exists(value):
                         raise ValueError("Given coordinate file path does not exist")
 
@@ -120,17 +121,21 @@
                                     raise ValueError(
                                         f"options_sigma.postprocessing.out_1D_vs_times.time has invalid data for value {value}. Start value can not be larger than end value.")
                             else:
                                 raise ValueError(
                                     "options_sigma.postprocessing.out_1D_vs_times.time has invalid data. Three elements needed.")
 
         # options_sigma.quench_heaters
-        # th_coils = options_sigma.quench_heaters.th_coils
-        # if 0 in th_coils:
-        #     raise ValueError("List contains zero values")
+        if options_sigma.simulation.study_type == constants.LABEL_TRANSIENT:
+            th_coils = options_sigma.quench_heaters.th_coils
+            if 0 in th_coils:
+                raise ValueError("List contains zero values, change model_data.yaml to valid value.")
+
+            if self.model_data.quench_protection.quench_heaters.N_strips == None:
+                raise ValueError("N_strips can't be null. Edit the model_data.yaml file.")
 
     def helper_check_time_step_valid(self, time_step):
         if type(time_step) == list:
             if any(isinstance(el, list) for el in time_step):
                 # Check data in vector is valid;
                 for i in range(len(time_step)):
                     if len(time_step[i]) == 3:
```

### Comparing `steam-pysigma-2023.5.9/steam_pysigma/data/DataRoxieParser.py` & `steam-pysigma-2023.6.1/steam_pysigma/data/DataRoxieParser.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,17 +258,17 @@
 
 
 class Corner(BaseModel):
     """
         Class for corner positions
     """
     iH: Coord = Coord()  # inner left
-    iLA: Coord = Coord()  # inner right
+    iL: Coord = Coord()  # inner right
     oH: Coord = Coord()  # outer left
-    oLA: Coord = Coord()  # outer right
+    oL: Coord = Coord()  # outer right
 
 
 class HalfTurnCorner(BaseModel):
     """
         Class for corner type
     """
     insulated: Corner = Corner()
@@ -279,36 +279,51 @@
     """
         Class for half-turn data
     """
     corners: HalfTurnCorner = HalfTurnCorner()
     strand_groups: Dict[int, StrandGroup] = {}
 
 
+class Order(BaseModel):
+    """
+        Class for electrical order (block location)
+    """
+    coil: int = None
+    pole: int = None
+    layer: int = None
+    winding: int = None
+    block: int = None
+
+
 class CenterShift(BaseModel):
     """
         Class for bore center shift
     """
     inner: Coord = Coord()
     outer: Coord = Coord()
 
 
 class Wedge(BaseModel):
     """
         Class for wedge positions
     """
     corners: Corner = Corner()
+    corners_ins: Corner = Corner()
     corrected_center: CenterShift = CenterShift()
-    coil: int = None
+    corrected_center_ins: CenterShift = CenterShift()
+    order_l: Order = Order()
+    order_h: Order = Order()
 
 
 class BlockData(BaseModel):
     """
         Class for block data
     """
     block_corners: Corner = Corner()
+    block_corners_ins: Corner = Corner()
     current_sign: int = None
     half_turns: Dict[int, HalfTurn] = {}
 
 
 class WindingData(BaseModel):
     """
         Class for winding data
@@ -336,25 +351,14 @@
     """
         Class for poles
     """
     poles: Dict[int, Layer] = {}
     bore_center: Coord = Coord()
 
 
-class Order(BaseModel):
-    """
-        Class for electrical order (block location)
-    """
-    coil: int = None
-    pole: int = None
-    layer: int = None
-    winding: int = None
-    block: int = None
-
-
 class CoilData(BaseModel):
     """
         Class for coils
     """
     coils: Dict[int, Pole] = {}
     physical_order: List[Order] = []
```

### Comparing `steam-pysigma-2023.5.9/steam_pysigma/data/DataSIGMA.py` & `steam-pysigma-2023.6.1/steam_pysigma/data/DataSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.5.9/steam_pysigma/domain_generator/GeometryMultipole.py` & `steam-pysigma-2023.6.1/steam_pysigma/domain_generator/GeometryMultipole.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,21 @@
 class GeometryMultipole:
     """
     Class creates SIGMA domain objects
     IMPROVMENTS:
     No dependency on config sigma
     """
 
-    def __init__(self, g, input_roxie_data, input_model_data, input_conductor_params, settings_dict, flag_build=True,
+    def __init__(self, g, input_roxie_data, input_model_data, bh_curve_database, input_conductor_params, settings_dict, flag_build=True,
                  verbose=False):
 
         self.model_data = input_model_data
         self.roxie_data = input_roxie_data
         self.input_conductor_params = input_conductor_params
-        self.bh_curve_database = Path.joinpath(Path(__file__).parent,
-                                               input_model_data.sources.bh_curve_source).resolve()
-        print(self.bh_curve_database)
+        self.bh_curve_database = bh_curve_database
         self.settings_dict: dict = settings_dict
         self.verbose = verbose
         if (not self.model_data or not self.roxie_data) and flag_build:
             raise Exception('Cannot build model without providing DataModelMagnet and RoxieData')
         elif flag_build:
             self.g = g
             self.a = ps.ArraysSIGMA
@@ -73,25 +71,25 @@
                         areas = ()
                         currents = ()
                         for block_key, block in winding.blocks.items():
                             currents += (block.current_sign,)
                             # kp0 = self.g.Point.ofCartesian(coil.bore_center.x, coil.bore_center.y)
                             bore = coil.bore_center
                             if (
-                                    block.block_corners.iH.y > 0.0 and block.block_corners.oH.y > 0.0 and block.block_corners.iLA.y > 0.0 and block.block_corners.oLA.y > 0.0):  # ?
+                                    block.block_corners.iH.y > 0.0 and block.block_corners.oH.y > 0.0 and block.block_corners.iL.y > 0.0 and block.block_corners.oL.y > 0.0):  # ?
                                 inner, outer = arcCenter(bore, block.block_corners.iH, block.block_corners.oH
-                                                         , block.block_corners.iLA, block.block_corners.oLA,
+                                                         , block.block_corners.iL, block.block_corners.oL,
                                                          diff_radius=None)
                             else:
-                                inner, outer = arcCenter(bore, block.block_corners.iLA, block.block_corners.oLA,
+                                inner, outer = arcCenter(bore, block.block_corners.iL, block.block_corners.oL,
                                                          block.block_corners.iH,
                                                          block.block_corners.oH, diff_radius=None)
                             arg = [self.g.Point.ofCartesian(block.block_corners.iH.x, block.block_corners.iH.y),
-                                   self.g.Point.ofCartesian(block.block_corners.iLA.x, block.block_corners.iLA.y),
-                                   self.g.Point.ofCartesian(block.block_corners.oLA.x, block.block_corners.oLA.y),
+                                   self.g.Point.ofCartesian(block.block_corners.iL.x, block.block_corners.iL.y),
+                                   self.g.Point.ofCartesian(block.block_corners.oL.x, block.block_corners.oL.y),
                                    self.g.Point.ofCartesian(block.block_corners.oH.x, block.block_corners.oH.y)]
                             kp0_inner = self.g.Point.ofCartesian(inner[0], inner[1])
                             kp0_outer = self.g.Point.ofCartesian(outer[0], outer[1])
                             areas += (self.g.Area.ofHyperLines(
                                 self.a.create_hyper_line_array(self.g.gateway,
                                                                (self.g.Arc.ofEndPointsCenter(arg[1], arg[0], kp0_inner),
                                                                 self.g.Line.ofEndPoints(arg[1], arg[3]),
@@ -171,17 +169,17 @@
         wedges = self.roxie_data.wedges
 
         elements = []
         for i in wedges:
             kp0_inner = self.g.Point.ofCartesian(wedges[i].corrected_center.inner.x, wedges[i].corrected_center.inner.y)
             kp0_outer = self.g.Point.ofCartesian(wedges[i].corrected_center.outer.x, wedges[i].corrected_center.outer.y)
             arg = [self.g.Point.ofCartesian(wedges[i].corners.iH.x, wedges[i].corners.iH.y),
-                   self.g.Point.ofCartesian(wedges[i].corners.iLA.x, wedges[i].corners.iLA.y),
+                   self.g.Point.ofCartesian(wedges[i].corners.iL.x, wedges[i].corners.iL.y),
                    self.g.Point.ofCartesian(wedges[i].corners.oH.x, wedges[i].corners.oH.y),
-                   self.g.Point.ofCartesian(wedges[i].corners.oLA.x, wedges[i].corners.oLA.y)]
+                   self.g.Point.ofCartesian(wedges[i].corners.oL.x, wedges[i].corners.oL.y)]
 
             area = self.g.Area.ofHyperLines(self.a.create_hyper_line_array(
                 self.g.gateway, (self.g.Arc.ofEndPointsCenter(arg[0], arg[1], kp0_inner),
                                  self.g.Line.ofEndPoints(arg[1], arg[3]),
                                  self.g.Arc.ofEndPointsCenter(arg[3], arg[2], kp0_outer),
                                  self.g.Line.ofEndPoints(arg[0], arg[2]))))
             self.wedge_areas += [area]
```

### Comparing `steam-pysigma-2023.5.9/steam_pysigma/helpers.py` & `steam-pysigma-2023.6.1/steam_pysigma/helpers.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.5.9/steam_pysigma/plotters/PlotterPysigma.py` & `steam-pysigma-2023.6.1/steam_pysigma/plotters/PlotterPysigma.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.5.9/steam_pysigma/postprocessing/postprocessing.py` & `steam-pysigma-2023.6.1/steam_pysigma/postprocessing/postprocessing.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.5.9/steam_pysigma/pysigma.py` & `steam-pysigma-2023.6.1/steam_pysigma/pysigma.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.5.9/steam_pysigma/utils/Util.py` & `steam-pysigma-2023.6.1/steam_pysigma/utils/Util.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.5.9/steam_pysigma.egg-info/PKG-INFO` & `steam-pysigma-2023.6.1/steam_pysigma.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-pysigma
-Version: 2023.5.9
+Version: 2023.6.1
 Summary: This is python wrapper of STEAM SIGMA code
 Home-page: https://gitlab.cern.ch/steam/steam_pysigma
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: SIGMA,STEAM,CERN
+Keywords: STEAM,SIGMA,CERN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM PySIGMA
```

### Comparing `steam-pysigma-2023.5.9/steam_pysigma.egg-info/SOURCES.txt` & `steam-pysigma-2023.6.1/steam_pysigma.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -16,13 +16,14 @@
 steam_pysigma/data/DataSIGMA.py
 steam_pysigma/data/__init__.py
 steam_pysigma/domain_generator/GeometryMultipole.py
 steam_pysigma/domain_generator/__init__.py
 steam_pysigma/parsers/ParserRoxie.py
 steam_pysigma/parsers/__init__.py
 steam_pysigma/plotters/PlotterPysigma.py
+steam_pysigma/plotters/PlotterRoxie.py
 steam_pysigma/plotters/__init__.py
 steam_pysigma/postprocessing/__init__.py
 steam_pysigma/postprocessing/postprocessing.py
 steam_pysigma/utils/Util.py
 steam_pysigma/utils/__init__.py
 steam_pysigma/utils/make_folder_if_not_existing.py
```

