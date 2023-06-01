# Comparing `tmp/vissim2geojson-1.3.0.tar.gz` & `tmp/vissim2geojson-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vissim2geojson-1.3.0.tar", last modified: Wed Jun 15 00:21:33 2022, max compression
+gzip compressed data, was "vissim2geojson-1.5.0.tar", last modified: Thu Jun  1 22:11:56 2023, max compression
```

## Comparing `vissim2geojson-1.3.0.tar` & `vissim2geojson-1.5.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-06-15 00:21:33.821671 vissim2geojson-1.3.0/
--rw-rw-rw-   0        0        0     1083 2022-06-14 17:24:15.000000 vissim2geojson-1.3.0/LICENSE
--rw-rw-rw-   0        0        0     3471 2022-06-15 00:21:33.819663 vissim2geojson-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2866 2022-06-14 23:34:53.000000 vissim2geojson-1.3.0/README.md
--rw-rw-rw-   0        0        0       94 2022-06-14 23:44:59.000000 vissim2geojson-1.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-06-15 00:21:33.823666 vissim2geojson-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1606 2022-06-15 00:20:09.000000 vissim2geojson-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-06-15 00:21:33.803673 vissim2geojson-1.3.0/vissim2geojson/
--rw-rw-rw-   0        0        0      299 2022-06-15 00:12:58.000000 vissim2geojson-1.3.0/vissim2geojson/__init__.py
--rw-rw-rw-   0        0        0      320 2022-06-15 00:12:24.000000 vissim2geojson-1.3.0/vissim2geojson/_model.py
--rw-rw-rw-   0        0        0    13419 2022-06-15 00:16:44.000000 vissim2geojson-1.3.0/vissim2geojson/vissim2geojson.py
-drwxrwxrwx   0        0        0        0 2022-06-15 00:21:33.814667 vissim2geojson-1.3.0/vissim2geojson.egg-info/
--rw-rw-rw-   0        0        0     3471 2022-06-15 00:21:33.000000 vissim2geojson-1.3.0/vissim2geojson.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2022-06-15 00:21:33.000000 vissim2geojson-1.3.0/vissim2geojson.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-15 00:21:33.000000 vissim2geojson-1.3.0/vissim2geojson.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2022-06-15 00:21:33.000000 vissim2geojson-1.3.0/vissim2geojson.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 22:11:56.701382 vissim2geojson-1.5.0/
+-rw-rw-rw-   0        0        0     1083 2022-06-14 17:24:15.000000 vissim2geojson-1.5.0/LICENSE
+-rw-rw-rw-   0        0        0     3420 2023-06-01 22:11:56.701382 vissim2geojson-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2856 2023-06-01 22:11:23.000000 vissim2geojson-1.5.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-01 22:11:56.701382 vissim2geojson-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1660 2023-06-01 21:59:22.000000 vissim2geojson-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:11:56.667174 vissim2geojson-1.5.0/vissim2geojson/
+-rw-rw-rw-   0        0        0      326 2023-06-01 22:04:23.000000 vissim2geojson-1.5.0/vissim2geojson/__init__.py
+-rw-rw-rw-   0        0        0      320 2022-06-15 00:12:24.000000 vissim2geojson-1.5.0/vissim2geojson/_model.py
+-rw-rw-rw-   0        0        0    13617 2023-06-01 22:10:12.000000 vissim2geojson-1.5.0/vissim2geojson/vissim2geojson.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:11:56.701382 vissim2geojson-1.5.0/vissim2geojson.egg-info/
+-rw-rw-rw-   0        0        0     3420 2023-06-01 22:11:56.000000 vissim2geojson-1.5.0/vissim2geojson.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-06-01 22:11:56.000000 vissim2geojson-1.5.0/vissim2geojson.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 22:11:56.000000 vissim2geojson-1.5.0/vissim2geojson.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-01 22:11:56.000000 vissim2geojson-1.5.0/vissim2geojson.egg-info/top_level.txt
```

### Comparing `vissim2geojson-1.3.0/LICENSE` & `vissim2geojson-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vissim2geojson-1.3.0/PKG-INFO` & `vissim2geojson-1.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: vissim2geojson
-Version: 1.3.0
+Version: 1.5.0
 Summary: Convert vissim files(.inpx and .fzp to geojson, .fhz to csv). This tool help user to convert vissim files to wgs1984 and csv files.
 Home-page: https://github.com/Xiangyongluo/vissim2wgs1984
 Author: Xiangyong Luo
 Author-email: luoxiangyong01@gamil.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # vissim2wgs1984
 
 Convert vissim files (.inpx and .fzp to geojson, .fhz to csv).
 
-This tool help user to convert vissim files to wgs1984 and csv files.
+This tool help user convert vissim files to wgs1984 and csv files.
 
 specifically,
 
 1. convert **.inpx** to .geojson file
 2. convert **.fzp** file to .geojson and csv files.  comment: will return two files, one is geojson file and anther is csv file.
 3. convert **.fhz** file to csv file.
 
@@ -30,21 +28,21 @@
 
 1. **Vissim Simulation**
    This tool is to conver files geneated by PTV Vissim. You design you own network or get network from other sources.
 
    You will get the layer file (.inpx). the .inpx can only open by PTV Vissim and you can use this tool to convert layer file to wgs1984 so that you can see your layer at different platform (QGIS, Kepler.gl, ArcMap...)
 
    You will get simulation results (.fzp and .fhz). you can open these files by PTV Vissim but you can not other platform. you can use this tool to convert .fzp file to (.geojson and .csv),  .fhz file to .geojson.
-2. **Prepare data in need for this tool**
+2. **Prepare data for this tool**
 
    In order to use this tool , you need to prepare several data for the map conversion.
 
    There are for digital nubmers from Background maps:
 
-   every time you are using PTV Vissim, the software will generate these nubmers at Base Data -> Network settings -> Display
+   Everytime you are using PTV Vissim, the software will generate these nubmers at Base Data -> Network settings -> Display
 
    **Reference point in map**: (-9772791.018, 5317836.791)                  you will need to replace these numbers by yours
 
    **Reference point in network**: (0.000, 0.000)                                     you will need to replace these numbers by yours
 
    ![1655246139117](image/README/1655246139117.png)
 
@@ -72,17 +70,18 @@
    if__name__=="main":
 
        file_inpx ="./vissim_data/xl_002.inpx"
        file_fhz ="./vissim_data/xl_002_001.fhz"
        file_fzp ="./vissim_data/xl_002_001.fzp"
        file_folder ="./vissim_data"
 
-       # prepare map reference data from Vissim
+       # prepare map reference info from Vissim
        x_refmap =-9772791.018
        y_refmap =5317836.791
+
        x_refnet =0
        y_refnet =0
 
        # for covert fzp files, if you don't need to convert fzp file, leave these value to default values.
        x_col_name ="POS"
        y_col_name ="POSLAT"
 
@@ -90,9 +89,7 @@
        # all result files will save to the same folder as the input folder.
 
        vissim2wgs1984(file_folder, x_refmap, y_refmap, x_refnet, y_refnet, x_col_name, y_col_name).main()
 
    ```
 
 Enjoy it!
-
-
```

### Comparing `vissim2geojson-1.3.0/README.md` & `vissim2geojson-1.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # vissim2wgs1984
 
 Convert vissim files (.inpx and .fzp to geojson, .fhz to csv).
 
-This tool help user to convert vissim files to wgs1984 and csv files.
+This tool help user convert vissim files to wgs1984 and csv files.
 
 specifically,
 
 1. convert **.inpx** to .geojson file
 2. convert **.fzp** file to .geojson and csv files.  comment: will return two files, one is geojson file and anther is csv file.
 3. convert **.fhz** file to csv file.
 
@@ -14,21 +14,21 @@
 
 1. **Vissim Simulation**
    This tool is to conver files geneated by PTV Vissim. You design you own network or get network from other sources.
 
    You will get the layer file (.inpx). the .inpx can only open by PTV Vissim and you can use this tool to convert layer file to wgs1984 so that you can see your layer at different platform (QGIS, Kepler.gl, ArcMap...)
 
    You will get simulation results (.fzp and .fhz). you can open these files by PTV Vissim but you can not other platform. you can use this tool to convert .fzp file to (.geojson and .csv),  .fhz file to .geojson.
-2. **Prepare data in need for this tool**
+2. **Prepare data for this tool**
 
    In order to use this tool , you need to prepare several data for the map conversion.
 
    There are for digital nubmers from Background maps:
 
-   every time you are using PTV Vissim, the software will generate these nubmers at Base Data -> Network settings -> Display
+   Everytime you are using PTV Vissim, the software will generate these nubmers at Base Data -> Network settings -> Display
 
    **Reference point in map**: (-9772791.018, 5317836.791)                  you will need to replace these numbers by yours
 
    **Reference point in network**: (0.000, 0.000)                                     you will need to replace these numbers by yours
 
    ![1655246139117](image/README/1655246139117.png)
 
@@ -56,17 +56,18 @@
    if__name__=="main":
 
        file_inpx ="./vissim_data/xl_002.inpx"
        file_fhz ="./vissim_data/xl_002_001.fhz"
        file_fzp ="./vissim_data/xl_002_001.fzp"
        file_folder ="./vissim_data"
 
-       # prepare map reference data from Vissim
+       # prepare map reference info from Vissim
        x_refmap =-9772791.018
        y_refmap =5317836.791
+
        x_refnet =0
        y_refnet =0
 
        # for covert fzp files, if you don't need to convert fzp file, leave these value to default values.
        x_col_name ="POS"
        y_col_name ="POSLAT"
```

### Comparing `vissim2geojson-1.3.0/setup.py` & `vissim2geojson-1.5.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     with open("requirements.txt", "r", encoding="utf-8") as f:
         modules_needed = [i.strip() for i in fh.readlines()]
 except Exception:
     modules_needed = []
 
 setuptools.setup(
     name="vissim2geojson",  # Replace with your own username
-    version="1.3.0",
+    version="1.5.0",
     author="Xiangyong Luo",
     author_email="luoxiangyong01@gamil.com",
     description="Convert vissim files(.inpx and .fzp to geojson, .fhz to csv). This tool help user to convert vissim files to wgs1984 and csv files.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Xiangyongluo/vissim2wgs1984",
 
@@ -36,9 +36,10 @@
     python_requires='>=3.6',
 
     install_requires=modules_needed,
     packages=setuptools.find_packages(),
     include_package_data=True,
 
     package_data={'': ['*.txt', '*.xls', '*.xlsx', '*.csv', '*.png', "*.inpx", "*.fhz", "*.fzp"],
-                  "test_data": ['*.txt', '*.png', "*.inpx", "*.fhz", "*.fzp"]}
+                  "test_data": ['*.txt', '*.png', "*.inpx", "*.fhz", "*.fzp"]},
+    data_files=[("vissim_data", ["vissim_data/*"])]
 )
```

### Comparing `vissim2geojson-1.3.0/vissim2geojson/vissim2geojson.py` & `vissim2geojson-1.5.0/vissim2geojson/vissim2geojson.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,65 +17,73 @@
 import math
 
 
 class vissim2wgs1984:
 
     print("Please check and correctly input x_refmap, y_refmap, x_refnet and y_refnet from your vissim software!")
 
-    def __init__(self, vissim_file_path, x_refmap=-9772674.016, y_refmap=5317775.409, x_refnet=0, y_refnet=0, x_col_name="POS", y_col_name="POSLAT"):
+    def __init__(self,
+                 vissim_file_path: str,
+                 x_refmap: float = -9772674.016,
+                 y_refmap: float = 5317775.409,
+                 x_refnet: float = 0,
+                 y_refnet: float = 0,
+                 x_col_name:str = "POS",
+                 y_col_name: str = "POSLAT"):
+
         """A tool to convert vissim files to geojson and csv.
             specifically:
                 convert .inpx file to geojson file
                 convert .fzp file to geojson and csv files
                 convert .fhz file to csv file
         Args:
             vissim_file_path (_type_): the folder or file path to the vissim file
             x_refmap (float, optional): coordinates of the reference point of the background map(Mercator). Defaults to -9772674.016.
             y_refmap (float, optional): coordinates of the reference point of the background map(Mercator). Defaults to 5317775.409.
             x_refnet (int, optional): coordinates of the reference point of the network(Cartesian Vissim System). Defaults to 0.
             y_refnet (int, optional): coordinates of the reference point of the network(Cartesian Vissim System). Defaults to 0.
             x_col_name (str, optional): the longitude column name in fzp file to convert fzp file to geojson. Defaults to "POS".
             y_col_name (str, optional):the latitude column name in fzp file to convert fzp file to geojson. Defaults to "POSLAT".
         """
-        
+
         self.vissim_file_path = self.__allFiles(vissim_file_path)
         print("Input files: ", self.vissim_file_path)
-        
+
         self.x_refmap = x_refmap
         self.y_refmap = y_refmap
         self.x_refnet = x_refnet
         self.y_refnet = y_refnet
         self.x_col_name = x_col_name
         self.y_col_name = y_col_name
 
         # The class automatically return files in certain folder
         # self.main()
 
     # This return all files in a folder or subfolder or single file
-    def __allFiles(self, path, SeeFiles=False):
-        
+    def __allFiles(self, path: str, view_files=False) -> list:
+
         files = []
 
         def readFiles(path):
             if isfile(path):
                 files.append(path)
             elif isdir(path):
                 for f in listdir(path):
                     if isfile(join(path, f)):
                         files.append(join(path, f))
                     if isdir(join(path, f)):
                         readFiles(join(path, f))
             else:
                 print("Invalid Input Path!")
             return files
-        if SeeFiles:
+        if view_files:
             print(readFiles(path))
         return readFiles(path)
 
-    def __vissim2wgs1984(self, x_vissim, y_vissim):
+    def __vissim2wgs1984(self, x_vissim: float, y_vissim: float) -> list:
 
         # ##This is a function that transfer a single vissim x,y coordinate date into wgs1984 x,y format######
 
         # Local coordinates in PTV Vissim use a cartesian coordinate system with a reference to a background position in Mercator coordinates.
 
         # coordinates of the point to be converted(Cartesian Vissim System)
         # x_vissim , y_vissim = -0.255, 39.368
@@ -111,52 +119,52 @@
         # a_cor and r represents ???   经度
         Longitude = a_cor * MercatorX / (Pi * r / 180)
         Latitude = (2 * math.atan(math.exp(CorrectionFactorMercator *
                                            MercatorY / EarthRadius)) - Pi / 2) / (Pi / 180)  # 维度
 
         return [Longitude, Latitude]
 
-    def __get_link(self, path_vissim_inpx):
+    def __get_link(self, path_vissim_inpx: str) -> list:
         with open(path_vissim_inpx, "r") as f:
             xmlstring = f.read()
         f.close()
 
         tree = ET.ElementTree(ET.fromstring(xmlstring))
         root = tree.getroot()
         return root.findall("links")[0]
 
-    def __link_vissim2wgs(self): 
+    def __link_vissim2wgs(self):
         link_data = []
         link_data1 = []  # original x,   y multistring data
         link_data2 = []  # transfered x, y multistring data
-        
-        for i in range(len(self.link)): 
+
+        for i in range(len(self.link)):
             temp = []
             temp1 = []  # original single x,   y data
             temp2 = []  # transfered single x, y data
-            for j in range(len(self.link[i])): 
-                for k in range(len(self.link[i][j])): 
+            for j in range(len(self.link[i])):
+                for k in range(len(self.link[i][j])):
                     with contextlib.suppress(Exception):
-                        for m in range(len(self.link[i][j][k])): 
+                        for m in range(len(self.link[i][j][k])):
                             temp.extend((self.link[i][j][k][m].attrib["x"], self.link[i][j][k][m].attrib["y"], self.link[i][j][k][m].attrib["zOffset"]))
                             temp1.append((float(self.link[i][j][k][m].attrib["x"]), float(self.link[i][j][k][m].attrib["y"])))
                             temp2.append(self.__vissim2wgs1984(float(self.link[i][j][k][m].attrib["x"]), float(self.link[i][j][k][m].attrib["y"])))
                     with contextlib.suppress(Exception):
                         temp.append(self.link[i][j][k].attrib["width"])
             link_data.append(temp)
             link_data1.append(temp1)  # link original
             link_data2.append(temp2)  # link transfered
         # df = pd.DataFrame(link_data)
         return link_data, link_data1, link_data2
 
     def main(self):
         # #####save geojson data to geojson file ######
 
-        for i in self.vissim_file_path: 
-            if ".inpx" in i: 
+        for i in self.vissim_file_path:
+            if ".inpx" in i:
                 print("############## Begin to process inpx file! ######################\n")
                 self.output_filename = i + ".geojson"
                 self.link = self.__get_link(i)
                 self.vissimLayer, self.vissim_xy, self.wgs1984_lonlat = self.__link_vissim2wgs()
 
                 self.__multilines = MultiLineString([[(3.75, 9.25), (-130.95, 1.52)], [(
                     23.15, -34.25), (-1.35, -4.65), (3.45, 77.95)]])  # doctest: +ELLIPSIS
@@ -165,119 +173,122 @@
                 feature = Feature(geometry=self.__multilines)
                 feature_collection = FeatureCollection([feature])
                 with open(self.output_filename, 'w') as f:
                     dump(feature_collection, f)
                     # f.write(str(self.__multilines))
                 f.close()
                 print("\nSuccessfully Save inpx file to geojson\n", self.output_filename)
-            elif ".fzp" in i: 
+
+            elif ".fzp" in i:
                 print("############## Begin to process fzp file! ######################\n")
                 self.output_filename = i + ".geojson"
                 self.vissim_fzp(i, self.x_col_name, self.y_col_name)
                 self.dataframe2geojson()
                 print("\nSuccessfully Save fzp file to geojson\n", self.output_filename)
-            elif ".fhz" in i: 
+
+            elif ".fhz" in i:
                 print("############## Begin to process fhz file! ######################\n")
                 self.output_filename = i + ".csv"
                 self.vissim_fhz(i)
                 self.fhz_data.to_csv(
                     self.output_filename, header=True, index=False, encoding="utf_8_sig")
 
                 # df.to_csv(self.output_filename,header=False,index = False,encoding="utf_8_sig")
                 print("\nSuccessfully Save fhz file to csv\n", "fhz file is a vissim output file need no to transfer to geojson\n", self.output_filename)
-            else: 
+
+            else:
                 warnings.warn(f"Invalid Input File or Folder: {i}.")
-        
-    def vissim_fzp(self, path_vissim_fzp, x_col_name="POS", y_col_name="POSLAT"): 
+
+    def vissim_fzp(self, path_vissim_fzp: str, x_col_name: str = "POS", y_col_name: str = "POSLAT") -> None:
         df_fzp = ""
-        with open(path_vissim_fzp, 'rb') as ff: 
+        with open(path_vissim_fzp, 'rb') as ff:
             df_fzp = pd.DataFrame(ff.readlines())
         ff.close()
         fzp_date = str(df_fzp.iloc[3, :])  # Get the vissim running time(date)
 
         start_fzp = next((i for i in range(len(df_fzp)) if str(df_fzp.iloc[i, 0])[3:10] == "VEHICLE"), 0)
 
         # fzp file starts from start_fzp(row 28)
         vissim_fzpdata = df_fzp.iloc[start_fzp:]
         fzp_data = pd.DataFrame([str(jj).split(';') for jj in vissim_fzpdata.iloc[:, 0]])
 
         columns_pre = []
         columns_pre = list(fzp_data.iloc[0])
-        for i in columns_pre: 
-            if "\\r\\n'" in i: 
+        for i in columns_pre:
+            if "\\r\\n'" in i:
                 columns_pre[columns_pre.index(i)] = i[:-5]
 
         fzp_data.columns = columns_pre
-        
+
         fzp_data = fzp_data.iloc[1:]
         fzp_data = fzp_data.reset_index(drop=True)
         fzp_data.iloc[:, 0] = [i.split("'")[1] for i in fzp_data.iloc[:, 0]]
 
         fzp_data.iloc[:, 0] = fzp_data.iloc[:, 0].astype(float)
 
         fzp_data["datetime"] = pd.to_datetime(fzp_date.split("\\")[0].split(
             "Date: ")[1]) + pd.to_timedelta(fzp_data.iloc[:, 0], unit='s')
-        
+
         fzp_data[y_col_name] = fzp_data[y_col_name].apply(lambda x: x[:-5])
         # print(fzp_data.head(10))
 
-        for coor in range(len(fzp_data[x_col_name])): 
+        for coor in range(len(fzp_data[x_col_name])):
             # "COORDREARX"
             with contextlib.suppress(Exception):
                 fzp_data.loc[coor, f"{x_col_name}_wgs"], fzp_data.loc[coor, f"{y_col_name}_wgs"] = self.__vissim2wgs1984(float(fzp_data.loc[coor, x_col_name]), float(fzp_data.loc[coor, y_col_name]))
 
         self.fzp_data = fzp_data
         self.x_col_name_lonlat = f"{x_col_name}_wgs"
         self.y_col_name_lonlat = f"{y_col_name}_wgs"
 
-    def dataframe2geojson(self):
+    def dataframe2geojson(self) -> None:
         df = self.fzp_data
         geometry = [Point(xy) for xy in zip(df[self.x_col_name_lonlat], df[self.y_col_name_lonlat])]
         # http: //www.spatialreference.org/ref/epsg/2263/
-        
+
         geo_df = GeoDataFrame(df, crs="EPSG:4326", geometry=geometry)  # geometry=geometry
         geo_df.to_file(self.output_filename, driver="GeoJSON")
         df.to_csv(self.output_filename + ".csv", index=False)
         # geo_df.to_file(driver='ESRI Shapefile', filename='data.shp')
 
-    def vissim_fhz(self, path_vissim_fhz): 
+    def vissim_fhz(self, path_vissim_fhz: str) -> None:
 
-        with open(path_vissim_fhz, 'rb') as f: 
+        with open(path_vissim_fhz, 'rb') as f:
             df_fhz = pd.DataFrame(f.readlines())
         f.close()
         fhz_date = str(df_fhz.iloc[5, :])
         start_fhz = next((i for i in range(len(df_fhz)) if str(df_fhz.iloc[i, :])[11:15] == "Time"), 0)
 
         vissim_fhzdata = df_fhz.iloc[start_fhz:]  # fhz file starts from row 8
         fhz_data = pd.DataFrame([str(jj).split(';') for jj in vissim_fhzdata.iloc[:, 0]])
         fhz_data.columns = fhz_data.iloc[0]
         fhz_data = fhz_data.iloc[1:]
         fhz_data = fhz_data.reset_index(drop=True)
-        for j in range(len(fhz_data.iloc[:, 0])): 
+        for j in range(len(fhz_data.iloc[:, 0])):
             fhz_data.iloc[j, 0] = str(fhz_data.iloc[j, 0]).split("'")[1]
 
         fhz_data.iloc[:, 0] = fhz_data.iloc[:, 0].astype(float)
         fhz_data["datetime"] = pd.to_datetime(fhz_date.split("Name")[0].split(
             "Date:")[1].lstrip()) + pd.to_timedelta(fhz_data.iloc[:, 0], unit="s")
 
         self.fhz_data = fhz_data
 
 
 if __name__ == "__main__":
     file_inpx = "./vissim_data/xl_002.inpx"
     file_fhz = "./vissim_data/xl_002_001.fhz"
     file_fzp = "./vissim_data/xl_002_001.fzp"
     file_folder = "./vissim_data"
-    
+
     # prepare map reference data from Vissim
     x_refmap = -9772791.018
     y_refmap = 5317836.791
     x_refnet = 0
     y_refnet = 0
-    
+
     # for covert fzp files, if you don't need to convert fzp file, leave these value to default values.
     x_col_name = "POS"
     y_col_name = "POSLAT"
 
     # using vissim folder as input path, will generate four files: inpx.geojson, fzp.geojson, fzp.csv, fhz.csv.
     # all result files will save to the same folder as the input folder.
     vissim2wgs1984(file_folder, x_refmap, y_refmap, x_refnet, y_refnet, x_col_name, y_col_name).main()
```

### Comparing `vissim2geojson-1.3.0/vissim2geojson.egg-info/PKG-INFO` & `vissim2geojson-1.5.0/vissim2geojson.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: vissim2geojson
-Version: 1.3.0
+Version: 1.5.0
 Summary: Convert vissim files(.inpx and .fzp to geojson, .fhz to csv). This tool help user to convert vissim files to wgs1984 and csv files.
 Home-page: https://github.com/Xiangyongluo/vissim2wgs1984
 Author: Xiangyong Luo
 Author-email: luoxiangyong01@gamil.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # vissim2wgs1984
 
 Convert vissim files (.inpx and .fzp to geojson, .fhz to csv).
 
-This tool help user to convert vissim files to wgs1984 and csv files.
+This tool help user convert vissim files to wgs1984 and csv files.
 
 specifically,
 
 1. convert **.inpx** to .geojson file
 2. convert **.fzp** file to .geojson and csv files.  comment: will return two files, one is geojson file and anther is csv file.
 3. convert **.fhz** file to csv file.
 
@@ -30,21 +28,21 @@
 
 1. **Vissim Simulation**
    This tool is to conver files geneated by PTV Vissim. You design you own network or get network from other sources.
 
    You will get the layer file (.inpx). the .inpx can only open by PTV Vissim and you can use this tool to convert layer file to wgs1984 so that you can see your layer at different platform (QGIS, Kepler.gl, ArcMap...)
 
    You will get simulation results (.fzp and .fhz). you can open these files by PTV Vissim but you can not other platform. you can use this tool to convert .fzp file to (.geojson and .csv),  .fhz file to .geojson.
-2. **Prepare data in need for this tool**
+2. **Prepare data for this tool**
 
    In order to use this tool , you need to prepare several data for the map conversion.
 
    There are for digital nubmers from Background maps:
 
-   every time you are using PTV Vissim, the software will generate these nubmers at Base Data -> Network settings -> Display
+   Everytime you are using PTV Vissim, the software will generate these nubmers at Base Data -> Network settings -> Display
 
    **Reference point in map**: (-9772791.018, 5317836.791)                  you will need to replace these numbers by yours
 
    **Reference point in network**: (0.000, 0.000)                                     you will need to replace these numbers by yours
 
    ![1655246139117](image/README/1655246139117.png)
 
@@ -72,17 +70,18 @@
    if__name__=="main":
 
        file_inpx ="./vissim_data/xl_002.inpx"
        file_fhz ="./vissim_data/xl_002_001.fhz"
        file_fzp ="./vissim_data/xl_002_001.fzp"
        file_folder ="./vissim_data"
 
-       # prepare map reference data from Vissim
+       # prepare map reference info from Vissim
        x_refmap =-9772791.018
        y_refmap =5317836.791
+
        x_refnet =0
        y_refnet =0
 
        # for covert fzp files, if you don't need to convert fzp file, leave these value to default values.
        x_col_name ="POS"
        y_col_name ="POSLAT"
 
@@ -90,9 +89,7 @@
        # all result files will save to the same folder as the input folder.
 
        vissim2wgs1984(file_folder, x_refmap, y_refmap, x_refnet, y_refnet, x_col_name, y_col_name).main()
 
    ```
 
 Enjoy it!
-
-
```

