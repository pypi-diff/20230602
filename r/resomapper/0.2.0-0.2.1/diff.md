# Comparing `tmp/resomapper-0.2.0.tar.gz` & `tmp/resomapper-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resomapper-0.2.0.tar", max compression
+gzip compressed data, was "resomapper-0.2.1.tar", max compression
```

## Comparing `resomapper-0.2.0.tar` & `resomapper-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     2817 2023-05-19 14:13:54.847958 resomapper-0.2.0/LICENSE
--rw-r--r--   0        0        0      857 2023-05-29 13:48:33.041389 resomapper-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2931 2023-05-24 10:04:14.557416 resomapper-0.2.0/README.md
--rw-r--r--   0        0        0      114 2023-05-05 11:04:10.117735 resomapper-0.2.0/resomapper/__init__.py
--rw-r--r--   0        0        0     5581 2023-05-29 13:46:36.947032 resomapper-0.2.0/resomapper/cli.py
--rw-r--r--   0        0        0    19722 2023-05-29 13:46:36.947032 resomapper-0.2.0/resomapper/file_system_functions.py
--rw-r--r--   0        0        0        2 2023-05-11 15:27:12.587903 resomapper-0.2.0/resomapper/myrelax/__init__.py
--rw-r--r--   0        0        0    29416 2023-04-18 15:08:27.862058 resomapper-0.2.0/resomapper/myrelax/getT1TR.py
--rw-r--r--   0        0        0    29826 2023-04-18 15:08:27.862058 resomapper-0.2.0/resomapper/myrelax/getT2T2star.py
--rw-r--r--   0        0        0     8166 2023-05-22 13:05:31.541382 resomapper-0.2.0/resomapper/preprocessing.py
--rw-r--r--   0        0        0    69042 2023-05-29 13:46:36.947032 resomapper-0.2.0/resomapper/processing.py
--rw-r--r--   0        0        0    19243 2023-05-29 13:46:36.962655 resomapper-0.2.0/resomapper/utils.py
--rw-r--r--   0        0        0     3978 1970-01-01 00:00:00.000000 resomapper-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2817 2023-05-19 14:13:54.847958 resomapper-0.2.1/LICENSE
+-rw-r--r--   0        0        0      857 2023-06-02 08:11:46.996757 resomapper-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2931 2023-05-24 10:04:14.557416 resomapper-0.2.1/README.md
+-rw-r--r--   0        0        0      114 2023-05-05 11:04:10.117735 resomapper-0.2.1/resomapper/__init__.py
+-rw-r--r--   0        0        0     5560 2023-06-02 07:25:26.661296 resomapper-0.2.1/resomapper/cli.py
+-rw-r--r--   0        0        0    25261 2023-05-31 14:19:33.655191 resomapper-0.2.1/resomapper/file_system_functions.py
+-rw-r--r--   0        0        0        2 2023-05-11 15:27:12.587903 resomapper-0.2.1/resomapper/myrelax/__init__.py
+-rw-r--r--   0        0        0    29416 2023-04-18 15:08:27.862058 resomapper-0.2.1/resomapper/myrelax/getT1TR.py
+-rw-r--r--   0        0        0    29826 2023-04-18 15:08:27.862058 resomapper-0.2.1/resomapper/myrelax/getT2T2star.py
+-rw-r--r--   0        0        0     7534 2023-06-02 08:09:40.236010 resomapper-0.2.1/resomapper/preprocessing.py
+-rw-r--r--   0        0        0    62382 2023-05-31 13:11:18.455517 resomapper-0.2.1/resomapper/processing.py
+-rw-r--r--   0        0        0    19972 2023-05-31 10:55:56.176706 resomapper-0.2.1/resomapper/utils.py
+-rw-r--r--   0        0        0     3978 1970-01-01 00:00:00.000000 resomapper-0.2.1/PKG-INFO
```

### Comparing `resomapper-0.2.0/LICENSE` & `resomapper-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `resomapper-0.2.0/pyproject.toml` & `resomapper-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "resomapper"
-version = "0.2.0"
+version = "0.2.1"
 description = "Pipeline for processing MR images and generating parametric maps."
 authors = ["Biomedical-MR"]
 license = "MIT"
 readme = "README.md"
 
 packages = [
     { include = "resomapper" }
```

### Comparing `resomapper-0.2.0/README.md` & `resomapper-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `resomapper-0.2.0/resomapper/cli.py` & `resomapper-0.2.1/resomapper/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# import click
 import multiprocessing
 import os
 import traceback
 import warnings
 
 from colorama import just_fix_windows_console
 
@@ -17,15 +16,15 @@
 from resomapper.utils import Headermsg as hmg
 from resomapper.utils import Mask, ask_user
 
 warnings.filterwarnings("ignore")
 
 
 def cli():
-    """Comand Line Interface of resomapper:
+    """Comand Line Interface of resomapper.
 
     1. Select root directory where studies are stored.
     2. Convert Bruker studies to nifti.
     3. Select of modalities to be processed.
     4. Process selected studies and save results.
     """
     # Ensure color text shows
@@ -95,50 +94,49 @@
         mode = masker.select_mask_mode()
         mask_path = masker.create_mask(mode)
 
         if study_name.startswith("DT"):
             dti_map_pro = DTIProcessor(root_path, study)
             ok_mask = dti_map_pro.check_DTI_data()
             while not ok_mask:
-                mode = masker.select_mask_mode()
+                mode = masker.select_mask_mode(again=True)
                 mask_path = masker.create_mask(mode)
                 ok_mask = dti_map_pro.check_DTI_data()
 
             if ask_user("¿Deseas realizar un preprocesado de este estudio?"):
                 Preprocessing([study]).preprocess()
             dti_map_pro.process_DTI()
 
         elif study_name.startswith("MT"):
             mt_map_pro = MTProcessor(study, mask_path)
             ok_mask = mt_map_pro.check_MT_data()
             while not ok_mask:
-                mode = masker.select_mask_mode()
+                mode = masker.select_mask_mode(again=True)
                 mask_path = masker.create_mask(mode)
                 ok_mask = mt_map_pro.check_MT_data()
 
             if ask_user("¿Deseas realizar un preprocesado de este estudio?"):
                 Preprocessing([study]).preprocess()
             mt_map_pro.process_MT()
 
         else:
             n_cpu = multiprocessing.cpu_count() - 1
             t_map_pro = TMapProcessor(
                 study, mask_path, n_cpu=n_cpu, fitting_mode="nonlinear"
             )
             ok_mask = t_map_pro.check_T_data()
             while not ok_mask:
-                mode = masker.select_mask_mode()
+                mode = masker.select_mask_mode(again=True)
                 mask_path = masker.create_mask(mode)
                 ok_mask = t_map_pro.check_T_data()
 
             if ask_user("¿Deseas realizar un preprocesado de este estudio?"):
                 Preprocessing([study]).preprocess()
             t_map_pro.process_T_map(f_time_paths)
 
-    fs_builder.empty_supplfiles()
     print(f"\n{hmg.success}Procesamiento terminado.")
 
 
 def run_cli():
     """Runs the CLI of resomapper, catching keyboard interruption to exit the program
     or any other errors during execution.
     """
```

### Comparing `resomapper-0.2.0/resomapper/file_system_functions.py` & `resomapper-0.2.1/resomapper/file_system_functions.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,27 +12,34 @@
 import resomapper.utils as ut
 from resomapper.utils import Headermsg as hmg
 
 warnings.filterwarnings("ignore")
 
 
 def select_directory():
-    """Allows selection of root directory showing a file explorer window."""
+    """Allows selection of root directory showing a file explorer window.
+
+    Returns:
+        Path: full path to the selected directory."""
 
     root = tk.Tk()
     root.withdraw()
     file_path = filedialog.askdirectory()
     root.destroy()
     root.mainloop()
 
     return Path(file_path)
 
 
 def select_file():
-    """Allows selection of a file."""
+    """Allows selection of a file showing a file explorer window.
+
+    Returns:
+        Path: full path to the selected file.
+    """
 
     root = tk.Tk()
     root.withdraw()
     file_path = filedialog.askopenfilename()
     root.destroy()
     # root.mainloop()
 
@@ -65,65 +72,79 @@
             except FileNotFoundError:
                 print(f"{hmg.error}Por favor, introduce un directorio válido.")
     if return_cwd:
         return Path().cwd()
 
 
 class FileSystemBuilder:
+    """File and folder organization workflow."""
+
     def __init__(self, root_path) -> None:
+        """Initialize a new instance of the FileSystemBuilder class.
+
+        Args:
+            root_path (str): The path of the working directory.
+        """
         self.root_path = root_path
 
     def create_dir(self):
-        """Creates 'convertidos' and 'procesados' folders."""
+        """Create 'convertidos' and 'procesados' folders."""
 
-        folders = ["convertidos", "procesados", "supplfiles"]
+        folders = ["convertidos", "procesados"]
         for folder_name in folders:
             if not (self.root_path / folder_name).exists():
                 (self.root_path / folder_name).mkdir(parents=True)
 
-        self.empty_supplfiles()
-
-    def empty_supplfiles(self):
-        supplfiles_path = self.root_path / "supplfiles"
-        if supplfiles_path.exists():
-            for f in os.listdir(supplfiles_path):
-                os.remove(self.root_path / "supplfiles" / f)
-
     def get_studies(self):
-        """Get only studies folders. Returns a list with the
-        name of the studies."""
+        """Get only studies folders present in the working directory. Returns a list
+        with the names of the studies folders.
+
+        Returns:
+            list: list of paths to the studies folders in the working directory.
+        """
 
         not_studies = ["procesados", "convertidos", "supplfiles", ".DS_Store"]
         return [s for s in os.listdir(self.root_path) if s not in not_studies]
 
     def convert_bru_to_nii(self):
-        """Convert from Bruker to Niftii. Get files to convert from
-        'convertidos' folder."""
+        """Convert all studies present in the workinf folder from Bruker to Niftii.
+        Converted files will be stored in the 'convertidos' folder.
+        """
 
         studies_names = self.get_studies()
         self.path_converted = self.root_path / "convertidos"
         converter = Bru2NiiConverter(self.root_path, self.path_converted, studies_names)
         converter.perform_conversion_bru2nii()
 
     def get_study_subfolders(self, directory: str):
-        """Get subfolders of a directory located in root_path."""
+        """Get subfolders of a directory located in root_path.
+
+        Args:
+            directory (str): Name of the directory.
+
+        Returns:
+            Generator: A generator that yields subfolder paths.
+        """
         directory = self.root_path / directory
         return directory.glob("*/*")
 
     def rename_sutudies(self):
         """Rename studies located in 'convertidos' adding a
         prefix depending on their modality."""
         conv_study_subfolders = self.get_study_subfolders("convertidos")
         for subfolder in conv_study_subfolders:
             if subfolder.parts[-1].startswith("convertido"):
                 self.add_method_to_subfolder(subfolder)
 
     def ask_preprocessing(self):
-        """Select from a checklist those modalities to be processed. Returns a
-        list of str with the selected modalities."""
+        """Select from a checklist those modalities to be processed.
+
+        Returns:
+            list: list of str with the selected modalities.
+        """
 
         print(
             f"\n{hmg.ask}Marca qué modalidades deseas procesar en la ventana emergente."
         )
 
         # init tkinter
         root = tk.Tk()
@@ -155,17 +176,21 @@
         return [
             modalities[idx]
             for idx in range(len(modalities))
             if selected_modals[idx].get() == 1
         ]
 
     def get_converted_files(self, known_modals=False):
-        """Get those files we want to transfer to 'procesados' folder.
-        Returns  a list including *method.txt, *.nii, *DwEffBval.txt and
-        *DwGradVec.txt files."""
+        """Get the files' names of those that we want to transfer from 'convertidos'
+        to 'procesados' folder.
+
+        Returns:
+            list: a list including *method.txt, *.nii, *DwEffBval.txt and
+                *DwGradVec.txt files.
+        """
 
         # add an uderscore to distingish T2 from T2E and change DTI per DT
         modals = []
         method_files = []
         nii_files = []
         dti_files = []
         # ask user for which modalities are desired to be processed
@@ -205,20 +230,19 @@
 
         return method_files + nii_files + dti_files
 
     def transfer_files(self, src_paths=None, dst_paths=None):
         """Transfer files from 'convertidos' to 'procesados' folder.
         If folder alredy exists in destiny, it will not be overwritten.
 
-        Parameters
-        ----------
-            src_paths : list(Path)
-                Paths to source folder
-            dst_paths : list(Path)
-                Paths to destination folder
+        Args:
+            src_paths (list(Path)): Paths to source folder.
+                Defaults to None (automatically selected).
+            dst_paths (list(Path)): Paths to destination folder.
+                Defaults to None (automatically selected).
         """
 
         # replicate the file directory from 'convertidos' to 'procesados' taking
         # into account those modalities that user wants to process. Get the files
         # we want to mirror in 'procesados' folder.
         if src_paths is None:
             src_paths = self.get_converted_files()  # path of converted files
@@ -244,84 +268,189 @@
                     shutil.copy(src_path, dst_path)
                 except Exception:
                     print(
                         f'{hmg.error}No se ha podido trasferir el \
                             archivo {src_path.split("/|//")[-1]}'
                     )
 
+    # def add_method_to_subfolder2(self, study_subfolder: str):
+    #     """Adds method (T1, T2, T2*, D, MTon, MToff) to study subfolder name.
+    #     It discriminates by adquisition and method.
+
+    #     Args:
+    #         study_subfolder (str): Name or path of the study subfolder.
+
+    #     The 'acquisition_method.txt' file located in the study subfolder to determine
+    #     the acquisition method.
+
+    #     The following acquisition methods are handled:
+    #     - "RAREVTR": T1 modality.
+    #     - "MGE": T2* modality.
+    #     - "DtiEpi": Diffusion (DT) modality.
+    #     - "MSME": T2, M0, or MT modality.
+
+    #     For "MSME" acquisition method, it additionally reads the '*method.txt' file in
+    #     the subfolder to determine the specific method.
+    #     - If the method contains "EffectiveTE" and its length is greater than 35, the
+    #       subfolder is renamed as T2.
+    #     - If the method contains "MagTransOnOff = On", the subfolder is
+    #       renamed as MTon.
+    #     - If the method contains "MagTransOnOff = Off" and
+    #       "DigFilter = Digital_Medium", the subfolder is renamed as MToff.
+    #     """
+
+    #     f_adq = "acquisition_method.txt"
+    #     path_adq = study_subfolder / f_adq
+
+    #     try:
+    #         with open(path_adq, "r") as f:
+    #             adq_lines = f.readlines()
+    #     except FileNotFoundError:
+    #         # patch to avoid 'variable referenced before assignment error'
+    #         adq_lines = [""]
+
+    #     # rename study subfolder
+    #     if adq_lines[0] == "RAREVTR":  # T1
+    #         r_study_subfolder = Path("/".join(study_subfolder.parts[:-1])) / (
+    #             "T1_" + study_subfolder.parts[-1]
+    #         )
+    #         os.rename(study_subfolder, r_study_subfolder)
+
+    #     elif adq_lines[0] == "MGE":  # T2STAR
+    #         r_study_subfolder = Path("/".join(study_subfolder.parts[:-1])) / (
+    #             "T2E_" + study_subfolder.parts[-1]
+    #         )
+    #         os.rename(study_subfolder, r_study_subfolder)
+
+    #     elif adq_lines[0] == "DtiEpi":  # DIFFUSION
+    #         r_study_subfolder = Path("/".join(study_subfolder.parts[:-1])) / (
+    #             "DT_" + study_subfolder.parts[-1]
+    #         )
+    #         os.rename(study_subfolder, r_study_subfolder)
+
+    #     elif adq_lines[0] == "MSME":  # T2, M0 or MT
+    #         f_method = study_subfolder.parts[-1] + "_method.txt"
+    #         path_met = study_subfolder / f_method  # path to *method.txt file
+
+    #         try:
+    #             with open(path_met, "r") as f:
+    #                 met_lines = f.readlines()
+    #         except FileNotFoundError:
+    #             print(f"{hmg.error}Archivo no encontrado.")
+
+    #         for line in met_lines:
+    #             if not line.startswith("EffectiveTE"):
+    #                 continue
+    #             elif len(line) > 35:
+    #                 r_study_subfolder = Path("/".join(study_subfolder.parts[:-1])) / (
+    #                     "T2_" + study_subfolder.parts[-1]
+    #                 )
+    #                 os.rename(study_subfolder, r_study_subfolder)
+    #                 return None
+    #             else:
+    #                 if "MagTransOnOff = On \n" in met_lines:
+    #                     r_study_subfolder = Path(
+    #                         "/".join(study_subfolder.parts[:-1])
+    #                     ) / ("MT_" + study_subfolder.parts[-1])
+    #                     os.rename(study_subfolder, r_study_subfolder)
+    #                 elif ("MagTransOnOff = Off \n" in met_lines) and (
+    #                     "DigFilter = Digital_Medium \n" in met_lines
+    #                 ):
+    #                     r_study_subfolder = Path(
+    #                         "/".join(study_subfolder.parts[:-1])
+    #                     ) / ("M0_" + study_subfolder.parts[-1])
+    #                     os.rename(study_subfolder, r_study_subfolder)
+    #                 return None
+
     def add_method_to_subfolder(self, study_subfolder: str):
         """Adds method (T1, T2, T2*, D, MTon, MToff) to study subfolder name.
-        It discriminates by adquisition and method."""
+        It discriminates by adquisition and method.
+
+        Args:
+            study_subfolder (str): Name or path of the study subfolder.
+
+        The 'acquisition_method.txt' file located in the study subfolder to determine
+        the acquisition method.
+
+        The following acquisition methods are handled:
+        - "RAREVTR": T1 modality.
+        - "MGE": T2* modality.
+        - "DtiEpi": Diffusion (DT) modality.
+        - "MSME": T2, M0, or MT modality.
+
+        For "MSME" acquisition method, it additionally reads the '*method.txt' file in
+        the subfolder to determine the specific method.
+        - If the method contains "EffectiveTE" and its length is greater than 35, the
+          subfolder is renamed as T2.
+        - If the method contains "MagTransOnOff = On", the subfolder is renamed as MTon.
+        - If the method contains "MagTransOnOff = Off" and "DigFilter = Digital_Medium",
+          the subfolder is renamed as MToff.
+        """
 
         f_adq = "acquisition_method.txt"
         path_adq = study_subfolder / f_adq
 
         try:
             with open(path_adq, "r") as f:
                 adq_lines = f.readlines()
         except FileNotFoundError:
             # patch to avoid 'variable referenced before assignment error'
             adq_lines = [""]
 
-        # rename study subfolder
-        if adq_lines[0] == "RAREVTR":  # T1
-            r_study_subfolder = Path("/".join(study_subfolder.parts[:-1])) / (
-                "T1_" + study_subfolder.parts[-1]
-            )
-            os.rename(study_subfolder, r_study_subfolder)
+        acquisition_method = adq_lines[0].strip()
 
-        elif adq_lines[0] == "MGE":  # T2STAR
-            r_study_subfolder = Path("/".join(study_subfolder.parts[:-1])) / (
-                "T2E_" + study_subfolder.parts[-1]
-            )
-            os.rename(study_subfolder, r_study_subfolder)
+        new_prefix = None
 
-        elif adq_lines[0] == "DtiEpi":  # DIFFUSION
-            r_study_subfolder = Path("/".join(study_subfolder.parts[:-1])) / (
-                "DT_" + study_subfolder.parts[-1]
-            )
-            os.rename(study_subfolder, r_study_subfolder)
-
-        elif adq_lines[0] == "MSME":  # T2, M0 or MT
+        # Rename study subfolder based on acquisition method
+        if acquisition_method == "RAREVTR":  # T1
+            new_prefix = "T1_"
+        elif acquisition_method == "MGE":  # T2STAR
+            new_prefix = "T2E_"
+        elif acquisition_method == "DtiEpi":  # DIFFUSION
+            new_prefix = "DT_"
+        elif acquisition_method == "MSME":  # T2, M0 or MT
             f_method = study_subfolder.parts[-1] + "_method.txt"
             path_met = study_subfolder / f_method  # path to *method.txt file
 
             try:
                 with open(path_met, "r") as f:
                     met_lines = f.readlines()
             except FileNotFoundError:
                 print(f"{hmg.error}Archivo no encontrado.")
+                return None
 
             for line in met_lines:
-                if not line.startswith("EffectiveTE"):
-                    continue
-                elif len(line) > 35:
-                    r_study_subfolder = Path("/".join(study_subfolder.parts[:-1])) / (
-                        "T2_" + study_subfolder.parts[-1]
-                    )
-                    os.rename(study_subfolder, r_study_subfolder)
-                    return None
-                else:
-                    if "MagTransOnOff = On \n" in met_lines:
-                        r_study_subfolder = Path(
-                            "/".join(study_subfolder.parts[:-1])
-                        ) / ("MT_" + study_subfolder.parts[-1])
-                        os.rename(study_subfolder, r_study_subfolder)
-                    elif ("MagTransOnOff = Off \n" in met_lines) and (
-                        "DigFilter = Digital_Medium \n" in met_lines
-                    ):
-                        r_study_subfolder = Path(
-                            "/".join(study_subfolder.parts[:-1])
-                        ) / ("M0_" + study_subfolder.parts[-1])
-                        os.rename(study_subfolder, r_study_subfolder)
-                    return None
+                if line.startswith("EffectiveTE") and len(line) > 35:
+                    new_prefix = "T2_"
+                    break
+                elif line == "MagTransOnOff = On \n":
+                    new_prefix = "MT_"
+                    break
+                elif (
+                    line == "MagTransOnOff = Off \n"
+                    and "DigFilter = Digital_Medium \n" in met_lines
+                ):
+                    new_prefix = "M0_"
+                    break
+
+        if new_prefix:
+            r_study_subfolder = Path("/".join(study_subfolder.parts[:-1])) / (
+                new_prefix + study_subfolder.parts[-1]
+            )
+            os.rename(study_subfolder, r_study_subfolder)
 
     def get_modality(self, study_subfolder_path: str):
         """Returns the modality of a subfolder path such as
         "C:// * //T2_convertidos*"
+
+        Args:
+            study_subfolder_path (str): Path to the subfolder.
+
+        Returns:
+            str: The modality of the subfolder.
         """
         if study_subfolder_path.parts[-1][:3] == "T1_":
             return "T1"
         elif study_subfolder_path.parts[-1][:3] == "T2_":
             return "T2"
         elif study_subfolder_path.parts[-1][:3] == "T2E":
             return "T2E"
@@ -331,22 +460,20 @@
             return "MT"
         else:
             return "M0"
 
     def get_selected_studies(self):
         """Returns those studies that will be processed. Checks if a modality
         has alredy been processed. In that case gives two options:
-            a) Remove it and processed again
-            b) Do not process it again.
+            - Remove it and processed again
+            - Do not process it again.
 
-        Returns
-        -------
-            subfolders_paths: list(Path)
-                path to modality subfolders that will be processed.
-            modals_to_process : list(str)
+        Returns:
+            subfolders_paths (list): Paths to modality subfolders to be processed.
+            modals_to_process (list): Modalities present in the studies to process.
         """
 
         self.proc_study_subfolders = self.get_study_subfolders("procesados")
 
         subfolders_paths = []
         if "DTI" in self.modals_to_process:
             self.modals_to_process[self.modals_to_process.index("DTI")] = "DT"
@@ -382,57 +509,65 @@
                                 )
                                 ready = input(msg)
                                 ready = ready.lower()
 
                     # remove folder and files contained in it
                     shutil.rmtree(str(subfolder))
                     # create folder again
-                    src_path = Path(
-                        str(subfolder)
-                        .replace("procesados", "convertidos")
-                        .replace("procesado", "convertido")
-                    )
-                    files_to_trasnfer = self.get_converted_files([processed_modal])
+                    # src_path = Path(
+                    #     str(subfolder)
+                    #     .replace("procesados", "convertidos")
+                    #     .replace("procesado", "convertido")
+                    # )
+                    files_to_transfer = self.get_converted_files([processed_modal])
                     dst_paths = [
                         Path(
                             str(f)
                             .replace("convertidos", "procesados")
                             .replace("convertido", "procesado")
                         )
-                        for f in files_to_trasnfer
+                        for f in files_to_transfer
                     ]
-                    self.transfer_files(files_to_trasnfer, dst_paths)
+                    self.transfer_files(files_to_transfer, dst_paths)
                     subfolders_paths.append(subfolder)
 
         return subfolders_paths, self.modals_to_process
 
 
 ###############################################################################
 # From Bruker to Nifti format
 ###############################################################################
 
 
 class Bru2NiiConverter:
+    """Conversion from Bruker files to NIfTI files workflow."""
+
     def __init__(self, root_path: str, converted_path: str, studies: list) -> None:
+        """Initialize a new instance of the Bru2NiiConverter class.
+
+        Args:
+            root_path (str): Path of the working directory.
+            converted_path (str): Path of the output folder ('convertidos').
+            studies (list): List of paths to the studies folders in the working dir.
+        """
         self.root_path = root_path
         self.converted_path = converted_path
         self.studies = studies
 
     def convert_bru_2_nii(self, study):
-        """Convert Bruker files to NIfTI
-        Parameters
-        ----------
-            study : str
-                Name of the study to convert
+        """Convert Bruker files of one study to NIfTI.
 
-        To understand the Bruker2Nifti converter, you can check a example in:
-            https://github.com/SebastianoF/bruker2nifti/wiki/
+        Args:
+            study (str): Name of the study to convert.
 
-        Setting get_method or save_human_readable to False is
-        extremely not recommended
+        Note:
+            To understand the Bruker2Nifti converter, you can check a example in:
+            https://github.com/SebastianoF/bruker2nifti/wiki/
+            Setting get_method or save_human_readable to False is
+            extremely not recommended
         """
         pfo_study_in = str(self.root_path / study)
         pfo_study_out = str(self.root_path / "convertidos")
 
         # instantiating the converter
         study_name = "convertido_" + study
         bru = Bruker2Nifti(pfo_study_in, pfo_study_out, study_name=study_name)
@@ -447,27 +582,30 @@
         bru.save_human_readable = True  # stores parameters in a .txt
         bru.save_b0_if_dwi = False
 
         # perform conversion
         bru.convert()
 
     def perform_conversion_bru2nii(self):
-        """Three cases:
+        """Check if any studies have already been converted and convert those that
+        haven't or those that the user wants to reconvert.
+
+        Three cases:
         1. No study has been converted
         2. All studies have been converted
         3. Some studies have been converted
         """
         conv_f = os.listdir(self.converted_path)  # converted folder
         # 1. If list is empty converts all raw data folders from bruker to nii
         if not conv_f:
             conv_studies = []
             for study in self.studies:
                 self.convert_bru_2_nii(study)
                 conv_studies.append(study)
-            df_conv_studies = pd.DataFrame(conv_studies)
+            # df_conv_studies = pd.DataFrame(conv_studies)
             print(f"\n{hmg.info}Ya se han convertido todos los estudios.")
 
         else:
             alredy_conv = []
             not_conv = []
             for study in self.studies:
                 if "convertido_" + study in conv_f:
```

### Comparing `resomapper-0.2.0/resomapper/myrelax/getT1TR.py` & `resomapper-0.2.1/resomapper/myrelax/getT1TR.py`

 * *Files identical despite different names*

### Comparing `resomapper-0.2.0/resomapper/myrelax/getT2T2star.py` & `resomapper-0.2.1/resomapper/myrelax/getT2T2star.py`

 * *Files identical despite different names*

### Comparing `resomapper-0.2.0/resomapper/preprocessing.py` & `resomapper-0.2.1/resomapper/preprocessing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 import tkinter as tk
 import warnings
 from math import trunc
-from tkinter.messagebox import askyesno
 
 import matplotlib.pyplot as plt
 import nibabel as nib
 import numpy as np
 
 # from scipy.ndimage import rotate
 from skimage.restoration import denoise_nl_means
 from skimage.transform import rotate
 
-from resomapper.utils import Headermsg as hmg  # Added by Raquel
+from resomapper.utils import Headermsg as hmg
 from resomapper.utils import ask_user
 
 warnings.filterwarnings("ignore")
 
 
 def get_preprocessing_params():
+    """Show a window to select the parameters to perform non local means denoising.
+
+    Returns:
+        list: Filtering parameters list [search distance, window size, h value]
+    """
     print(f"\n{hmg.ask}Indica los parámetros de preprocesado en la ventana emergente.")
 
     root = tk.Tk()
     root.title("MyX")
 
     # declaring string variable for storing values
     patch_s = tk.StringVar()
@@ -77,45 +81,14 @@
     root.mainloop()
     try:
         return entries
     except NameError:
         return ""
 
 
-def ask_yes_no_preprocessing():
-    """Creates a window to ask a question that has a yes/no answer."""
-
-    warnings.filterwarnings("ignore")
-
-    root = tk.Tk()
-    root.withdraw()
-    answer = askyesno(title="MyX", message="¿Quieres realizar un preprocesado?")
-    root.destroy()
-    # añadir root.quit para que funcione (creo)
-
-    root.mainloop()
-
-    return answer
-
-
-def ask_yes_no_mask():
-    """Creates a window to ask a question that has a yes/no answer."""
-    warnings.filterwarnings("ignore")
-
-    root = tk.Tk()
-    root.withdraw()
-    msg = "¿Quieres reutilizar la última máscara hecha para este sujeto?"
-    answer = askyesno(title="MyX", message=msg)
-    root.destroy()
-
-    root.mainloop()
-
-    return answer
-
-
 class Preprocessing:
     def __init__(self, studies_paths):
         self.studies_paths = studies_paths
 
     def load_nii(self, study_path, is_mt_study=False, scan=0):
         """Returns data in size x_dim x y_dim x num slices x rep times"""
```

### Comparing `resomapper-0.2.0/resomapper/processing.py` & `resomapper-0.2.1/resomapper/processing.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,16 @@
         study_path = list(study_path.glob("M0*"))[0]
         for f in list(study_path.glob("*.nii.gz")):
             new_filename = f.parts[-1].replace("convertido", "procesado_M0")
             shutil.copy(os.path.join(f), os.path.join(self.mt_study_path, new_filename))
         # return study_path
 
     def select_MT_acq(self):
-        n_mt = int(len(list(self.mt_study_path.glob("*.nii.gz"))) / 2)
+        # n_mt = int(len(list(self.mt_study_path.glob("*.nii.gz"))) / 2)
+        n_mt = len(list(self.mt_study_path.glob("*.nii.gz"))) // 2
 
         if n_mt == 1:
             mt_folders_list = [1]
         else:
             print(
                 f"\n{hmg.warn}Has adquirido imágenes de MT con diferentes slopes para "
                 f"este estudio ({n_mt})."
@@ -169,17 +170,14 @@
                 )[0]
 
             # from nifti to array
             mt_on, affine1 = load_nifti(f_mton_path)
             mt_off, _ = load_nifti(f_mtoff_path)  # affine matrix is the same
             mask, _ = load_nifti(self.mask_path)
 
-            # check_shapes(mt_on, mask)
-            # check_shapes(mt_off, mask)
-
             # apply mask
             mt_on = mt_on * mask
             mt_off = mt_off * mask
 
             if len(self.selected_mt_folders_list) > 1:
                 # get maps
                 print(f"\n{hmg.info}Generando mapa de MT (carpeta {i}).")
@@ -204,155 +202,14 @@
                 mt_map = self.compute_MT_map(mt_on, mt_off)
 
                 # save as .nii file and save heatmaps
                 saving_path = str(self.mt_study_path / "MT_map.nii")
                 save_nifti(saving_path, mt_map.astype(np.float32), affine1)
                 Heatmap().save_heatmap(mt_map, "MT", out_path=str(self.mt_study_path))
 
-        # n_mt = int(len(list(self.mt_study_path.glob("*.nii.gz"))) / 2)
-
-        # if n_mt == 1:
-        #     f_mton_path = list(self.mt_study_path.glob("procesado_MT_*.nii.gz"))[0]
-        #     f_mtoff_path = list(self.mt_study_path.glob("procesado_M0_*.nii.gz"))[0]
-
-        #     # from nifti to array
-        #     mt_on, affine1 = load_nifti(f_mton_path)
-        #     mt_off, _ = load_nifti(f_mtoff_path)  # affine matrix is the same
-        #     mask, _ = load_nifti(self.mask_path)
-
-        #     check_shapes(mt_on, mask)
-        #     check_shapes(mt_off, mask)
-
-        #     # apply mask
-        #     mt_on = mt_on * mask
-        #     mt_off = mt_off * mask
-
-        #     # get maps
-        #     print(f"\n{hmg.info}Generando mapa de MT.")
-        #     mt_map = self.compute_MT_map(mt_on, mt_off)
-
-        #     # save as .nii file and save heatmaps
-        #     saving_path = str(self.mt_study_path / "MT_map.nii")
-        #     save_nifti(saving_path, mt_map.astype(np.float32), affine1)
-        #     Heatmap().save_heatmap(mt_map, "MT", out_path=str(self.mt_study_path))
-        # else:
-        #     print(
-        #         f"\n{hmg.warn}Has adquirido imágenes de MT con diferentes slopes "
-        #         f"para este estudio ({n_mt})."
-        #     )
-
-        #     input_ready = False
-        #     while not input_ready:
-        #         mt_folders_input = input(
-        #             f"\n{hmg.ask}Indica el número de la carpeta de adquisición que "
-        #             f"desas procesar (entre 1 y {n_mt}). "
-        #             "Si deseas procesar más de una carpeta, introduce los diferentes "
-        #             f'números separados por ",".\n{hmg.pointer}'
-        #         )
-        #         mt_folders_input = mt_folders_input.split(",")
-        #         try:
-        #             mt_folders_list = [int(x.strip()) for x in mt_folders_input]
-        #             input_ready = True
-        #             for number in mt_folders_list:
-        #                 if (number > n_mt) or (number < 1):
-        #                     print(
-        #                         f"\n{hmg.error}Por favor, introduce números entre 1 y"
-        #                         f" {n_mt}."
-        #                     )
-        #                     input_ready = False
-        #                     break
-        #         except Exception:
-        #             print(
-        #                 f'\n{hmg.error}Por favor, introduce sólo números separados'
-        #                 f' por "," (si hay más de uno).'
-        #             )
-
-        #     mt_folders_list = [*set(mt_folders_list)]
-
-        #     if len(mt_folders_list) == 1:
-        #         subscan_index = mt_folders_list[0] - 1
-        #         f_mton_path = list(
-        #             self.mt_study_path.glob(
-        #                 f"procesado_MT_*subscan_{subscan_index}.nii*"
-        #             )
-        #         )[0]
-        #         f_mtoff_path = list(
-        #             self.mt_study_path.glob(
-        #                 f"procesado_M0_*subscan_{subscan_index}.nii*"
-        #             )
-        #         )[0]
-
-        #         # from nifti to array
-        #         mt_on, affine1 = load_nifti(f_mton_path)
-        #         mt_off, _ = load_nifti(f_mtoff_path)  # affine matrix is the same
-        #         mask, _ = load_nifti(self.mask_path)
-
-        #         check_shapes(mt_on, mask)
-        #         check_shapes(mt_off, mask)
-
-        #         # apply mask
-        #         mt_on = mt_on * mask
-        #         mt_off = mt_off * mask
-
-        #         # get maps
-        #         print(f"\n{hmg.info}Generando mapa de MT.")
-        #         mt_map = self.compute_MT_map(mt_on, mt_off)
-
-        #         # save as .nii file and save heatmaps
-        #         saving_path = str(self.mt_study_path / "MT_map.nii")
-        #         save_nifti(saving_path, mt_map.astype(np.float32), affine1)
-        #         Heatmap().save_heatmap(mt_map, "MT", out_path=str(self.mt_study_path))
-
-        #     else:
-        #         for i in mt_folders_list:
-        #             subscan_index = i - 1
-        #             f_mton_path = list(
-        #                 self.mt_study_path.glob(
-        #                     f"procesado_MT_*subscan_{subscan_index}.nii*"
-        #                 )
-        #             )[0]
-        #             f_mtoff_path = list(
-        #                 self.mt_study_path.glob(
-        #                     f"procesado_M0_*subscan_{subscan_index}.nii*"
-        #                 )
-        #             )[0]
-
-        #             # from nifti to array
-        #             mt_on, affine1 = load_nifti(f_mton_path)
-        #             mt_off, _ = load_nifti(f_mtoff_path)  # affine matrix is the same
-        #             mask, _ = load_nifti(self.mask_path)
-
-        #             check_shapes(mt_on, mask)
-        #             check_shapes(mt_off, mask)
-
-        #             # apply mask
-        #             mt_on = mt_on * mask
-        #             mt_off = mt_off * mask
-
-        #             # get maps
-        #             print(f"\n{hmg.info}Generando mapa de MT (carpeta {i}).")
-        #             mt_map = self.compute_MT_map(mt_on, mt_off)
-
-        #             try:
-        #                 os.mkdir(str(self.mt_study_path / str(i)))
-        #             except Exception:
-        #                 pass
-
-        #             # save as .nii file and save heatmaps
-        #             mt_map_filename = f"MT_map_{str(i)}.nii"
-        #             saving_path = os.path.join(
-        #                 str(self.mt_study_path), str(i), mt_map_filename
-        #             )
-        #             save_nifti(saving_path, mt_map.astype(np.float32), affine1)
-        #             Heatmap().save_heatmap(
-        #                 mt_map,
-        #                 "MT",
-        #                 out_path=os.path.join(str(self.mt_study_path), str(i)),
-        #             )
-
 
 ###############################################################################
 # DTI PROCESSING
 ###############################################################################
 class DTIProcessor:
     def __init__(self, root_path: str, study_path: str) -> None:
         self.root_path = root_path
@@ -397,21 +254,21 @@
 
         src_dirs = list(self.study_path.glob("*_DwGradVec.txt"))[0]
         src_bvals = list(self.study_path.glob("*_DwEffBval.txt"))[0]
 
         method_path = list(self.study_path.glob("procesado_*_method.txt"))[0]
         with open(method_path, "r") as f:
             lines = f.readlines()
-            for idx, line in enumerate(lines):
+            for line in lines:
                 if line.startswith("DwNDiffDir"):
-                    n_dirs_real = int(re.search("\d+", line).group(0))
+                    n_dirs_real = int(re.search("\d+", line)[0])
                 elif line.startswith("DwNDiffExpEach"):
-                    n_b_val_real = int(re.search("\d+", line).group(0))
+                    n_b_val_real = int(re.search("\d+", line)[0])
                 elif line.startswith("DwAoImages"):
-                    n_basal_real = int(re.search("\d+", line).group(0))
+                    n_basal_real = int(re.search("\d+", line)[0])
 
         if n_b_val != n_b_val_real:
             print(
                 f"\n{hmg.warn}Has introducido un número de b valores diferente "
                 "al adquirido."
             )
             print(
@@ -653,16 +510,19 @@
     def process_DTI(self):
         """Solves diffusion tensor using Non-Linear Least Squares (NLLS) and
         computes ADC, FA, MD, AD, RD and R^2 maps."""
 
         n_b_val, n_basal, n_dirs = self.ask_dti_info()
 
         # create B values and B dirs files
-        f_bvals = self.root_path / "supplfiles" / "Bvalues.bval"
-        f_dirs = self.root_path / "supplfiles" / "Bdirs.bvec"
+        # f_bvals = self.root_path / "supplfiles" / "Bvalues.bval"
+        # f_dirs = self.root_path / "supplfiles" / "Bdirs.bvec"
+
+        f_bvals = self.study_path / "Bvalues.bval"
+        f_dirs = self.study_path / "Bdirs.bvec"
 
         b_vals, dirs, n_b_val, n_basal, n_dirs, indexes_to_rm = self.get_bvals_n_dirs(
             n_b_val, n_basal, n_dirs
         )
 
         with open(f_bvals, "w") as f:
             for b_val in b_vals:
@@ -692,38 +552,21 @@
         try:
             mask, affine = load_nifti(self.study_path / "mask.nii")
         except FileNotFoundError:
             mask, affine = load_nifti(
                 Path("/".join(self.study_path.parts[:-1])) / "mask.nii"
             )
 
-        # check_shapes(
-        #     data, mask, callback_func=self.process_DTI, study_path=self.study_path
-        # )
-        # ok_mask = check_shapes(data, mask)
-        # while not ok_mask:
-        #     mode = self.masker.select_mask_mode()
-        #     self.masker.create_mask(mode)
-        #     # while True:
-        #     #     try:
-        #     #         masker.create_mask(mode)
-        #     #         break
-        #     #     except PermissionError:
-        #     #         print("retrying")
-        #     #         time.sleep(5)
-        #     mask, affine = load_nifti(self.study_path / "mask.nii")
-        #     ok_mask = check_shapes(data, mask)
-
         # apply mask
         for i in range(data.shape[3]):  # para cada imagen de cada slice
             data[:, :, :, i] = data[:, :, :, i] * mask
 
         # read b values (bvals) and gradient directions (bvecs)
-        bval_path = str(self.root_path / "supplfiles" / "bvalues.bval")
-        bvec_path = str(self.root_path / "supplfiles" / "Bdirs.bvec")
+        bval_path = str(self.study_path / "bvalues.bval")
+        bvec_path = str(self.study_path / "Bdirs.bvec")
         bvals, bvecs = read_bvals_bvecs(bval_path, bvec_path)
 
         # create gradient table. You can access gradients with gtab.gradients
         gtab = gradient_table(bvals, bvecs, atol=1e-0)
         # gtab contains bvec and bvals, such as
         # -0.066   0.9937   -0.089   421.46    Gradient direction and b_val_1
         # -0.066   0.9937   -0.089   1827.43   Gradient direction and b_val_2
@@ -976,18 +819,18 @@
             times = list(map(lambda x: x.rstrip("."), times))
 
             return times
 
         except FileNotFoundError:
             print(f"{hmg.error}El directorio no existe.")
 
-    def write_times(self, times: list, file_name: str):
+    def write_times(self, times: list, file_name: str, subfolder: str):
         """Write times, overwritting if file alredy exists."""
 
-        file_path = self.root_path / "supplfiles" / file_name
+        file_path = self.root_path / subfolder / file_name
         with open(file_path, "w") as f:
             f.write(" ".join([t for t in times]))
 
         return file_path
 
     def get_times_auto(self):
         """Read times (TR, TE, TEs) automatically from method.txt files
@@ -996,144 +839,151 @@
         Returns
         -------
         times_paths: list
             Contains TR in position 0, TE in position 1, and TEs in position 2.
             It has to be in this way as other functions expect a varible with
             times in this particular structure."""
 
-        times_paths = [[], [], []]  # empty list that will store times
+        times_paths = {}  # empty dictionary that will store times
         for subfolder in self.studies_to_process:
             study_name = subfolder.parts[-1]
             if (
                 study_name.startswith("T1_")
-                and study_name[:2] in self.modals_to_process
+                and "T1" in self.modals_to_process
+                # and study_name[:2] in self.modals_to_process
             ):
                 TR_times = self.read_times(subfolder, "MultiRepTime", 3)
-                TR_times_path = self.write_times(TR_times, "TiemposRepeticion.txt")
-                times_paths[0] = TR_times_path
+                TR_times_path = self.write_times(
+                    TR_times, "TiemposRepeticion.txt", subfolder
+                )
+                times_paths[subfolder] = TR_times_path
 
             elif (
                 study_name.startswith("T2_")
-                and study_name[:2] in self.modals_to_process
+                and "T2" in self.modals_to_process
+                # and study_name[:2] in self.modals_to_process
             ):
                 TE_times = self.read_times(subfolder, "EffectiveTE", 3)
-                TE_times_path = self.write_times(TE_times, "TiemposEco.txt")
-                times_paths[1] = TE_times_path
+                TE_times_path = self.write_times(TE_times, "TiemposEco.txt", subfolder)
+                times_paths[subfolder] = TE_times_path
 
             elif (
                 study_name.startswith("T2E_")
-                and study_name[:3] in self.modals_to_process
+                and "T2E" in self.modals_to_process
+                # and study_name[:3] in self.modals_to_process
             ):
                 TEs_times = self.read_times(subfolder, "EffectiveTE", 4)
-                TEs_times_path = self.write_times(TEs_times, "TiemposEcoStar.txt")
-                times_paths[2] = TEs_times_path
+                TEs_times_path = self.write_times(
+                    TEs_times, "TiemposEcoStar.txt", subfolder
+                )
+                times_paths[subfolder] = TEs_times_path
 
         return times_paths
 
     # GET TIMES MANUALLY
-    def get_TR(self):
-        trs = []
-        while True:
-            try:
-                n_tr = int(
-                    input(
-                        "¿Cuántos tiempos de repetición se usaron "
-                        "en la acquisición de T1?\n"
-                    )
-                )
-                break
-            except ValueError:
-                print("No has introducido un número correcto.")
+    # def get_TR(self):
+    #     trs = []
+    #     while True:
+    #         try:
+    #             n_tr = int(
+    #                 input(
+    #                     "¿Cuántos tiempos de repetición se usaron "
+    #                     "en la acquisición de T1?\n"
+    #                 )
+    #             )
+    #             break
+    #         except ValueError:
+    #             print("No has introducido un número correcto.")
+
+    #     print("Deberás introducir los TR de mayor a menor.\n")
+    #     for i in range(n_tr):
+    #         tr = input(f"Introduce el tiempo de repetición {i+1}.\n")
+    #         trs.append(tr)
+
+    #     return trs
+
+    # def get_TE(self):
+    #     init_te = int(input("¿Primer tiempo de eco en T2? "))
+    #     n_te = int(input("¿Cuántos tiempos de eco hay en T2? "))
+    #     interval = int(input("¿Separación entre tiempos de eco? "))
+
+    #     return list(range(init_te, interval * n_te + interval, interval))
+
+    # def get_TE_star(self):
+    #     init_te_star = float(input("¿Primer tiempo de eco en T2 estrella? "))
+    #     n_te_star = float(input("¿Cuántos tiempos de eco hay en T2 estrella? "))
+    #     interval_star = float(input("¿Separación entre tiempos de eco? "))
+
+    #     return list(np.arange(init_te_star, interval_star * n_te_star, interval_star))
+
+    # def get_requested_times(self, modal: str):
+    #     if modal == "T1":
+    #         return self.get_TR()
+    #     elif modal == "T2":
+    #         return self.get_TE()
+    #     elif modal == "T2E":
+    #         return self.get_TE_star()
+
+    # def get_selected_time(self, selected_modal: str):
+    #     """If it does not exists, fuction returns a file with sequence
+    #     times (TR, TE or TE*). If it alredy exists, returns that file, as
+    #     it will have the same times.
+
+    #     Parameters
+    #     ----------
+    #         selected_modal: str
+    #             selected modality to process (T1, T2 or T2*).
+    #     Returns
+    #     -------
+    #         file_path: str
+    #             path to the file with the written times.
+    #     """
+    #     # define modalities names and time files names
+    #     modals = ["T1", "T2", "T2E"]
+    #     time_file_names = [
+    #         "TiemposRepeticion.txt",
+    #         "TiemposEco.txt",
+    #         "TiemposEcoStar.txt",
+    #     ]
+
+    #     modal_idx = modals.index(selected_modal)
+    #     file_name = time_file_names[
+    #         modal_idx
+    #     ]  # get file name (str) associated to modality
+
+    #     file_path = str(self.root_path / "supplfiles" / file_name)
+    #     if not os.path.exists(file_path):
+    #         times = self.get_requested_times(selected_modal)  # collects times
+    #         with open(file_path, "w+") as f:  # creates file
+    #             f.write(" ".join([str(t) for t in times]))
+    #     else:
+    #         print("[INFO]: Usando archivo de sujeto anterior para tiempos de eco T2")
+
+    #     return file_path
+
+    # def get_times_manual(self):
+    #     """Manually, you get times associated to T1, T2, T2E modalities i.e.
+    #     TR, TE, TE*, respectively. If a modality has not been selected by
+    #     the user to be processed returns an empty string."""
+
+    #     times = []
+    #     for modal in ["T1", "T2", "T2E"]:  # orden de los tiempos: tr, te, ts
+    #         if modal in self.modals_to_process:
+    #             time = self.get_selected_time(modal)
+    #             times.append(time)
+    #         else:
+    #             times.append("")
 
-        print("Deberás introducir los TR de mayor a menor.\n")
-        for i in range(n_tr):
-            tr = input(f"Introduce el tiempo de repetición {i+1}.\n")
-            trs.append(tr)
-
-        return trs
-
-    def get_TE(self):
-        init_te = int(input("¿Primer tiempo de eco en T2? "))
-        n_te = int(input("¿Cuántos tiempos de eco hay en T2? "))
-        interval = int(input("¿Separación entre tiempos de eco? "))
-
-        return list(range(init_te, interval * n_te + interval, interval))
-
-    def get_TE_star(self):
-        init_te_star = float(input("¿Primer tiempo de eco en T2 estrella? "))
-        n_te_star = float(input("¿Cuántos tiempos de eco hay en T2 estrella? "))
-        interval_star = float(input("¿Separación entre tiempos de eco? "))
-
-        return list(np.arange(init_te_star, interval_star * n_te_star, interval_star))
-
-    def get_requested_times(self, modal: str):
-        if modal == "T1":
-            return self.get_TR()
-        elif modal == "T2":
-            return self.get_TE()
-        elif modal == "T2E":
-            return self.get_TE_star()
-
-    def get_selected_time(self, selected_modal: str):
-        """If it does not exists, fuction returns a file with sequence
-        times (TR, TE or TE*). If it alredy exists, returns that file, as
-        it will have the same times.
-
-        Parameters
-        ----------
-            selected_modal: str
-                selected modality to process (T1, T2 or T2*).
-        Returns
-        -------
-            file_path: str
-                path to the file with the written times.
-        """
-        # define modalities names and time files names
-        modals = ["T1", "T2", "T2E"]
-        time_file_names = [
-            "TiemposRepeticion.txt",
-            "TiemposEco.txt",
-            "TiemposEcoStar.txt",
-        ]
-
-        modal_idx = modals.index(selected_modal)
-        file_name = time_file_names[
-            modal_idx
-        ]  # get file name (str) associated to modality
-
-        file_path = str(self.root_path / "supplfiles" / file_name)
-        if not os.path.exists(file_path):
-            times = self.get_requested_times(selected_modal)  # collects times
-            with open(file_path, "w+") as f:  # creates file
-                f.write(" ".join([str(t) for t in times]))
-        else:
-            print("[INFO]: Usando archivo de sujeto anterior para tiempos de eco T2")
-
-        return file_path
-
-    def get_times_manual(self):
-        """Manually, you get times associated to T1, T2, T2E modalities i.e.
-        TR, TE, TE*, respectively. If a modality has not been selected by
-        the user to be processed returns an empty string."""
-
-        times = []
-        for modal in ["T1", "T2", "T2E"]:  # orden de los tiempos: tr, te, ts
-            if modal in self.modals_to_process:
-                time = self.get_selected_time(modal)
-                times.append(time)
-            else:
-                times.append("")
-
-        return times
+    #     return times
 
     def get_times(self, how="auto"):
         if how == "auto":
             time_paths = self.get_times_auto()
-        else:
-            time_paths = self.get_times_manual()
+        # else:
+        #     time_paths = self.get_times_manual()
 
         return time_paths
 
 
 class TMapProcessor:
     def __init__(
         self, study_path: str, mask_path: str, n_cpu: int, fitting_mode="nonlinear"
@@ -1169,103 +1019,91 @@
             method = "T2"
             print(f"\n{hmg.info}Generando mapa de T2.\n")
             try:
                 f_name = self.study_path.parts[-1][3:] + "_subscan_0.nii.gz"
                 f_path = str(self.study_path / f_name)
                 out_path = f_path[:-7]  # remove .nii
 
-                # check_shapes(f_path, self.mask_path)
-
                 getT2T2star.TxyFitME(
                     f_path,
-                    time_paths[1],
+                    time_paths[self.study_path],
                     out_path,
                     self.fitting_mode,
                     self.n_cpu,
                     self.mask_path,
                 )
 
             except (NameError, FileNotFoundError):
                 f_name = self.study_path.parts[-1][3:] + ".nii.gz"
                 f_path = str(self.study_path / f_name)
                 out_path = f_path[:-7]  # remove .nii
 
-                # check_shapes(f_path, self.mask_path)
-
                 getT2T2star.TxyFitME(
                     f_path,
-                    time_paths[1],
+                    time_paths[self.study_path],
                     out_path,
                     self.fitting_mode,
                     self.n_cpu,
                     self.mask_path,
                 )
 
         elif "T2E" in str(self.study_path):
             method = "T2E"
             print(f"\n{hmg.info}Generando mapa de T2E.\n")
             try:
                 f_name = self.study_path.parts[-1][4:] + "_subscan_0.nii.gz"
                 f_path = str(self.study_path / f_name)
                 out_path = f_path[:-7]  # remove .nii
 
-                # check_shapes(f_path, self.mask_path)
-
                 getT2T2star.TxyFitME(
                     f_path,
-                    time_paths[2],
+                    time_paths[self.study_path],
                     out_path,
                     self.fitting_mode,
                     self.n_cpu,
                     self.mask_path,
                 )
             except (NameError, FileNotFoundError):
                 f_name = self.study_path.parts[-1][4:] + ".nii.gz"
                 f_path = str(self.study_path / f_name)
                 out_path = f_path[:-7]  # remove .nii
 
-                # check_shapes(f_path, self.mask_path)
-
                 getT2T2star.TxyFitME(
                     f_path,
-                    time_paths[2],
+                    time_paths[self.study_path],
                     out_path,
                     self.fitting_mode,
                     self.n_cpu,
                     self.mask_path,
                 )
 
         elif "T1" in str(self.study_path):
             method = "T1"
             print(f"\n{hmg.info}Generando mapa de T1.\n")
             try:
                 f_name = self.study_path.parts[-1][3:] + "_subscan_0.nii.gz"
                 f_path = str(self.study_path / f_name)
                 out_path = f_path[:-7]  # remove .nii.gz
 
-                # check_shapes(f_path, self.mask_path)
-
                 getT1TR.TxyFitME(
                     f_path,
-                    time_paths[0],
+                    time_paths[self.study_path],
                     out_path,
                     self.fitting_mode,
                     self.n_cpu,
                     self.mask_path,
                 )
             except (NameError, FileNotFoundError):
                 f_name = self.study_path.parts[-1][3:] + ".nii.gz"
                 f_path = str(self.study_path / f_name)
                 out_path = f_path[:-7]  # remove .nii
 
-                # check_shapes(f_path, self.mask_path)
-
                 getT1TR.TxyFitME(
                     f_path,
-                    time_paths[0],
+                    time_paths[self.study_path],
                     out_path,
                     self.fitting_mode,
                     self.n_cpu,
                     self.mask_path,
                 )
 
         # create a folder to store useful files
@@ -1373,24 +1211,21 @@
 
 ##############################################################################
 # HEATMAPS
 ##############################################################################
 class Heatmap:
     def rotate(self, array_2d):
         list_of_tuples = zip(*array_2d[::-1])
-        rotated_element = [list(elem) for elem in list_of_tuples]
-
-        return rotated_element
+        return [list(elem) for elem in list_of_tuples]
 
     def change_colormap(self):
         while True:
             cmap_name = input("Introduce el nombre del mapa de colores.\n")
             try:
-                cmap = cm.get_cmap(cmap_name)
-                return cmap
+                return cm.get_cmap(cmap_name)
             except ValueError:
                 print(
                     f'Has introducido "{cmap_name}" y ese nombre no corresponde '
                     "con ningún mapa. Vuelve a intentarlo.\n"
                 )
 
     def change_vmin_vmax(self):
@@ -1638,19 +1473,18 @@
         vmax=None,
         cmap=None,
     ):
         """Opens a window to show the heatmaps per slice and allows to
         change color range and color map. Do not use for ADC maps, use
         save_ADC_heatmap function instead.
 
-        Parameters
-        ----------
-            maps: stack of maps (one map per slice)
-            map_type: name of the map
-            out_path: string path to save output maps
+        Args:
+            maps (numpy.array): stack of maps (one map per slice)
+            map_type (str): name of the map
+            out_path (str): string path to save output maps
         """
         cmap = plt.cm.turbo  # select default cmap
         # cmap.set_bad('black', 1)  # paints NaN values in black
 
         if map_type == "FA":
             vmin = 0.05  # min possible value of FA
             vmax = 0.95  # max possible value of FA
```

### Comparing `resomapper-0.2.0/resomapper/utils.py` & `resomapper-0.2.1/resomapper/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,36 @@
 import shutil
 from pathlib import Path
 
 import cv2
 import matplotlib.pyplot as plt
 import numpy as np
 from dipy.io.image import load_nifti, save_nifti
-from PIL import Image
 from scipy.ndimage import rotate
 
+# from PIL import Image
+
 import resomapper.file_system_functions as fs
 
 
 class Headermsg:
-    """Class containing headers for messages during execution of the CLI."""
+    """Headers for messages shown during execution of the CLI.
+
+    Attributes:
+        info (str): Header for information messages.
+        warn (str): Header for warning messages.
+        error (str): Header for error messages.
+        success (str): Header for success messages.
+        pointer (str): Header for pointer messages.
+        ask (str): Header for question messages.
+        welcome (str): Header for the welcome message.
+        new_patient1 (str): Header for new patient study message (part 1).
+        new_patient2 (str): Header for new patient study message (part 2).
+        new_modal (str): Header for new modal message.
+    """
 
     info = "\x1b[0;30;44m [INFO] \x1b[0m "
     warn = "\x1b[0;30;43m [WARNING] \x1b[0m "
     error = "\x1b[0;30;41m [ERROR] \x1b[0m "
     success = "\x1b[0;30;42m [SUCCESS] \x1b[0m "
     pointer = "\x1b[5;36;40m>>>\x1b[0m "
     ask = "\x1b[0;30;46m ? \x1b[0m "
@@ -82,15 +96,14 @@
         else:
             print(
                 f"\n{Headermsg.error}Por favor, introduce una de las opciones "
                 "especificadas.\n"
             )
 
 
-# def check_shapes(img, mask, callback_func=None, study_path=None):
 def check_shapes(img, mask):
     """Check if an image and mask have the same shapes (resolution and slices).
     If the input arguments are file paths, the 'load_nifti' function is used to load the
     respective NIfTI files. The program will terminate if the shapes of the image and
     mask do not match.
 
     Args:
@@ -114,39 +127,32 @@
             f"{img.shape[2]} slices.\n"
             f"- Mask: resolution {mask.shape[0]}x{mask.shape[1]}, "
             f"{mask.shape[2]} slices."
         )
         return False
     else:
         return True
-        # if (callback_func is not None) and (study_path is not None):
-        #     mask = Mask(study_path)
-        #     mode = mask.select_mask_mode()
-        #     mask.create_mask(mode)
-        #     callback_func()
-        # else:
-        #     exit()
-        # exit()
 
 
 ###############################################################################
 # Mask creation
 ###############################################################################
 class Mask:
+    """Mask creating workflow."""
+
     def __init__(self, study_subfolder: str) -> None:
         """Initialize a new instance of the Mask class.
 
         Args:
             study_subfolder (str): The path or name of the study subfolder.
         """
         self.study_subfolder = study_subfolder
 
     def prepare_vol(self, vol_3d):
-        """Some modifications are needed on the volume: 270 degrees
-        rotation and image flip.
+        """Some modifications on the volume: 270 degrees rotation and image flip.
 
         Args:
             vol_3d (ndarray): Input image.
 
         Returns:
             list: Transformed image ready for visualization.
         """
@@ -166,15 +172,15 @@
             dim = (width, height)
             ima = cv2.resize(ima, dim, interpolation=cv2.INTER_AREA)
             vol_prepared.append(ima)
 
         return vol_prepared
 
     def min_max_normalization(self, img):
-        """Applies min-max normalization to the input image. Creates a copy of the input
+        """Apply min-max normalization to the input image. Creates a copy of the input
         image and computes the minimum and maximum values. The image is normalized using
         the formula (img - min_val) / (max_val - min_val).
 
         Args:
             img (numpy.ndarray): Input image array.
 
         Returns:
@@ -223,15 +229,15 @@
             param[counter].append(click_pos)
         elif event == cv2.EVENT_RBUTTONDOWN:  # right click
             click_pos = [(x, y)]
             param[counter].append(click_pos)
             status = 0  # finish
 
     def itera(self, ima, refPT):
-        """Iteratively displays slices for masking.Left click adds a line and right
+        """Iteratively display slices for masking. Left click adds a line and right
         click closes the polygon. Next slice will be showed after right click.
 
         Args:
             ima (numpy.ndarray): Input image array.
             refPT (list): List to store the masked vertices for each slice.
 
         The 'click' event handler is used to handle mouse events and update the 'refPT'
@@ -284,29 +290,28 @@
                         break
             except IndexError:
                 cv2.destroyAllWindows()
                 break
         return refPT
 
     def draw_mask(self):
-        """Creates a binary mask for the roi where processing will take place and saves
+        """Create a binary mask for the roi where processing will take place and save
         it as a NIfTI file. The user is prompted to create the mask by selecting
         contours in a pop-up window.
 
         The function loads the appropriate input image based on the study type, prepares
         the volume and creates a list of lists, 'refPT', to store the vertexes of the
         masks for each slice. The user is then presented with the selected contours
         overlaid on the image slices, and the function saves the image files and waits
         for a keyboard enter from the user to proceed.
 
         Next, the function creates a binary mask by filling the contours with ones and
         resizing the mask to match the original image dimensions. The resulting masks
         are converted to a NIfTI format by transposing the axes to match the expected
-        shape. The mask is saved both in the method subfolder and the
-        subject folder for reusability.
+        shape. The mask is saved both in the method subfolder.
 
         Example:
             masker = Mask(study_path)
             mask.draw_mask()
         """
 
         study_name = self.study_subfolder.parts[-2]
@@ -366,16 +371,17 @@
         ax = ax.flatten()
         for i in range(n_slc):
             poly = np.array((refPT[i]), np.int32)
             img_copy = np.copy(images[i])
             img_poly = cv2.polylines(
                 img_copy, [poly], True, (255, 255, 255), thickness=3
             )
-            im = Image.fromarray(img_poly)
-            im.save(self.study_subfolder / f"shape_slice_{str(i+1)}.png")
+            # Removed saving png images - not needed
+            # im = Image.fromarray(img_poly)
+            # im.save(self.study_subfolder / f"shape_slice_{str(i+1)}.png")
 
             ax[i].imshow(img_poly, cmap="gray")
             ax[i].set_title(f"Slice {i+1}")
             ax[i].axis("off")
 
         plt.tight_layout()
         keyboardClick = False
@@ -392,22 +398,16 @@
             mask = cv2.resize(mask, (x_dim, y_dim), interpolation=cv2.INTER_NEAREST)
             mask = mask.astype(np.int32)
             masks.append(mask)
             # cv2.destroyAllWindows()
         masks = np.asarray(masks)
         masks = masks.transpose(2, 1, 0)
 
-        # saving mask in both method subfolder and subject folder
-        # (for reusing mask purposes)
+        # saving mask in method subfolder
         save_nifti(self.study_subfolder / "mask", masks.astype(np.float32), affine)
-        save_nifti(
-            Path("/".join(self.study_subfolder.parts[:-1])) / "mask",
-            masks.astype(np.float32),
-            affine,
-        )
 
     def create_mask(self, mode="manual"):
         """Create a mask for the study image. Implemented modes:
         - 'manual': manual drawing, allowing several tries if user is not satisfied.
         - 'reuse': reuse last mask used for the current patient.
         - 'file_selection': manually select a mask file already created.
 
@@ -416,52 +416,66 @@
                 Defaults to "manual".
 
         Returns:
             Path: Study's mask file path.
         """
         study_path = self.study_subfolder
         dst_mask_path = study_path / "mask.nii"
+        reusing_mask_path = Path("/".join(study_path.parts[:-1])) / "mask.nii"
         if mode == "manual":
             correct_selection = False
             while not correct_selection:
                 self.draw_mask()
                 correct_selection = ask_user(
                     "¿Es la previsualización de la selección lo que deseas?"
                 )
             print(f"\n{Headermsg.info}Máscara creada correctamente.")
+            shutil.copy(dst_mask_path, reusing_mask_path)
 
         elif mode == "reuse":
             src_path = Path("/".join(study_path.parts[:-1])) / "mask.nii"
-            if os.path.exists(dst_mask_path):
-                os.remove(dst_mask_path)
             shutil.copy(src_path, dst_mask_path)
 
         elif mode == "file_selection":
             src_path = fs.select_file()
+            ok_file = False
+            while not ok_file:
+                if src_path in [dst_mask_path, reusing_mask_path]:
+                    print(
+                        f"\n{Headermsg.error}You selected the same mask as before. "
+                        "Try again"
+                    )
+                    src_path = fs.select_file()
+                    ok_file = False
+                else:
+                    ok_file = True
             ext = os.path.splitext(src_path)[1]
             if src_path is not None and ext in [".nii", ".gz"]:
                 shutil.copy(src_path, dst_mask_path)
-                # if os.path.exists(dst_mask_path):
-                #     os.remove(dst_mask_path)
-                # shutil.copy(src_path, dst_mask_path)
+                shutil.copy(src_path, reusing_mask_path)
             else:
                 print(f"\n{Headermsg.error}You didn't select a NiFTI file.")
                 exit()
 
         else:
             print(f"\n{Headermsg.error}Invalid masking mode selected.")
             exit()
 
         return dst_mask_path
 
-    def select_mask_mode(self):
+    def select_mask_mode(self, again=False):
         """Prompt the user to select the mode for specifying the mask for the study.
         The function checks if a previous mask file exists in the subject's folder to
         determine if the reuse option is available.
 
+        Args:
+            again (bool, optional): whether we are calling this function the first time
+                or a second time after an error when checking the mask and image
+                resolutions. In that case, the reuse option is not available.
+
         Returns:
             str: The selected mask mode.
 
         Possible return values:
             - "reuse": The user selected to reuse the last created mask.
             - "manual": The user selected manual selection mode.
             - "file_selection": The user selected to select another file.
@@ -469,18 +483,18 @@
         study_path = self.study_subfolder
         options = {
             "m": "Selección manual de la máscara.",
             "s": "Seleccionar otro archivo (máscara en formato NiFTI).",
         }
 
         last_mask_path = Path("/".join(study_path.parts[:-1])) / "mask.nii"
-        if last_mask_path.exists():
+        if last_mask_path.exists() and not again:
             options["r"] = "Reutilizar la última máscara creada para este sujeto."
 
-        question = "Selecciona cómo quieres especificar la máscara para este estudio:"
+        question = "Selecciona cómo quieres especificar la máscara para este estudio."
         selected_option = ask_user_options(question, options)
         if selected_option == "r":
             return "reuse"
         elif selected_option == "m":
             return "manual"
         elif selected_option == "s":
             return "file_selection"
```

### Comparing `resomapper-0.2.0/PKG-INFO` & `resomapper-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resomapper
-Version: 0.2.0
+Version: 0.2.1
 Summary: Pipeline for processing MR images and generating parametric maps.
 License: MIT
 Author: Biomedical-MR
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

