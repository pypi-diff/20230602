# Comparing `tmp/itkwasm_dicom_emscripten-2.0.3.tar.gz` & `tmp/itkwasm_dicom_emscripten-2.1.0.tar.gz`

## Comparing `itkwasm_dicom_emscripten-2.0.3.tar` & `itkwasm_dicom_emscripten-2.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/itkwasm_dicom_emscripten/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/itkwasm_dicom_emscripten/_version.py
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/itkwasm_dicom_emscripten/apply_presentation_state_to_image_async.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/itkwasm_dicom_emscripten/js_package.py
--rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/itkwasm_dicom_emscripten/read_dicom_encapsulated_pdf_async.py
--rw-r--r--   0        0        0    10552 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/itkwasm_dicom_emscripten/structured_report_to_html_async.py
--rw-r--r--   0        0        0     5025 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/itkwasm_dicom_emscripten/structured_report_to_text_async.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/test/__init__.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/test/fixtures.py
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/test/test_apply_presentation_state_to_image_async.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/test/test_itkwasm_dicom.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/test/test_read_dicom_encapsulated_pdf_async.py
--rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/test/test_structured_report_to_html_async.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/test/test_structured_report_to_text_async.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/.gitignore
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/README.md
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.1.0/itkwasm_dicom_emscripten/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.1.0/itkwasm_dicom_emscripten/_version.py
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.1.0/itkwasm_dicom_emscripten/apply_presentation_state_to_image_async.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.1.0/itkwasm_dicom_emscripten/js_package.py
+-rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.1.0/itkwasm_dicom_emscripten/read_dicom_encapsulated_pdf_async.py
+-rw-r--r--   0        0        0    10552 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.1.0/itkwasm_dicom_emscripten/structured_report_to_html_async.py
+-rw-r--r--   0        0        0     5025 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.1.0/itkwasm_dicom_emscripten/structured_report_to_text_async.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.1.0/test/__init__.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.1.0/test/fixtures.py
+-rw-r--r--   0        0        0     4614 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.1.0/test/test_apply_presentation_state_to_image_async.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.1.0/test/test_itkwasm_dicom.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.1.0/test/test_read_dicom_encapsulated_pdf_async.py
+-rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.1.0/test/test_structured_report_to_html_async.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.1.0/test/test_structured_report_to_text_async.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.1.0/.gitignore
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.1.0/README.md
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.1.0/PKG-INFO
```

### Comparing `itkwasm_dicom_emscripten-2.0.3/itkwasm_dicom_emscripten/apply_presentation_state_to_image_async.py` & `itkwasm_dicom_emscripten-2.1.0/itkwasm_dicom_emscripten/apply_presentation_state_to_image_async.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,27 +16,31 @@
     BinaryFile,
     Image,
 )
 
 async def apply_presentation_state_to_image_async(
     image_in: os.PathLike,
     presentation_state_file: os.PathLike,
+    color_output: bool = False,
     config_file: str = "",
     frame: int = 1,
     no_presentation_state_output: bool = False,
     no_bitmap_output: bool = False,
 ) -> Tuple[Dict, Image]:
-    """Apply a presentation state to a given DICOM image and render output as pgm bitmap or dicom file.
+    """Apply a presentation state to a given DICOM image and render output as bitmap, or dicom file.
 
     :param image_in: Input DICOM file
     :type  image_in: os.PathLike
 
     :param presentation_state_file: Process using presentation state file
     :type  presentation_state_file: os.PathLike
 
+    :param color_output: output image as RGB (default: false)
+    :type  color_output: bool
+
     :param config_file: filename: string. Process using settings from configuration file
     :type  config_file: str
 
     :param frame: frame: integer. Process using image frame f (default: 1)
     :type  frame: int
 
     :param no_presentation_state_output: Do not get presentation state information in text stream.
@@ -51,14 +55,16 @@
     :return: Output image
     :rtype:  Image
     """
     js_module = await js_package.js_module
     web_worker = js_resources.web_worker
 
     kwargs = {}
+    if color_output:
+        kwargs["colorOutput"] = to_js(color_output)
     if config_file:
         kwargs["configFile"] = to_js(config_file)
     if frame:
         kwargs["frame"] = to_js(frame)
     if no_presentation_state_output:
         kwargs["noPresentationStateOutput"] = to_js(no_presentation_state_output)
     if no_bitmap_output:
```

### Comparing `itkwasm_dicom_emscripten-2.0.3/itkwasm_dicom_emscripten/read_dicom_encapsulated_pdf_async.py` & `itkwasm_dicom_emscripten-2.1.0/itkwasm_dicom_emscripten/read_dicom_encapsulated_pdf_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.3/itkwasm_dicom_emscripten/structured_report_to_html_async.py` & `itkwasm_dicom_emscripten-2.1.0/itkwasm_dicom_emscripten/structured_report_to_html_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.3/itkwasm_dicom_emscripten/structured_report_to_text_async.py` & `itkwasm_dicom_emscripten-2.1.0/itkwasm_dicom_emscripten/structured_report_to_text_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.3/test/test_itkwasm_dicom.py` & `itkwasm_dicom_emscripten-2.1.0/test/test_itkwasm_dicom.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.3/test/test_read_dicom_encapsulated_pdf_async.py` & `itkwasm_dicom_emscripten-2.1.0/test/test_read_dicom_encapsulated_pdf_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.3/test/test_structured_report_to_html_async.py` & `itkwasm_dicom_emscripten-2.1.0/test/test_structured_report_to_html_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.3/test/test_structured_report_to_text_async.py` & `itkwasm_dicom_emscripten-2.1.0/test/test_structured_report_to_text_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.3/pyproject.toml` & `itkwasm_dicom_emscripten-2.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
   "itkwasm",
   "webassembly",
   "emscripten",
 ]
 
 requires-python = ">=3.7"
 dependencies = [
-    "itkwasm >= 1.0.b103",
+    "itkwasm >= 1.0.b105",
 ]
 
 [tool.hatch.version]
 path = "itkwasm_dicom_emscripten/_version.py"
 
 [tool.hatch.envs.default]
 dependencies = [
```

### Comparing `itkwasm_dicom_emscripten-2.0.3/PKG-INFO` & `itkwasm_dicom_emscripten-2.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itkwasm-dicom-emscripten
-Version: 2.0.3
+Version: 2.1.0
 Project-URL: Home, https://itk-wasm-dicom-python-docs.on.fleek.co
 Project-URL: Source, https://github.com/InsightSoftwareConsortium/itk-wasm
 Project-URL: Issues, https://github.com/InsightSoftwareConsortium/itk-wasm/issues
 License-Expression: Apache-2.0
 Keywords: emscripten,itkwasm,webassembly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: WebAssembly
@@ -18,24 +18,39 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
-Requires-Dist: itkwasm>=1.0.b103
+Requires-Dist: itkwasm>=1.0.b105
 Description-Content-Type: text/markdown
 
 # itkwasm-dicom-emscripten
 
 [![PyPI version](https://badge.fury.io/py/itkwasm-dicom-emscripten.svg)](https://badge.fury.io/py/itkwasm-dicom-emscripten)
 
 Read files and images related to DICOM file format. Emscripten implementation.
 
 This package provides the Emscripten WebAssembly implementation. It is usually not called directly. Please use the [`itkwasm-dicom`](https://pypi.org/project/itkwasm-dicom/) instead.
 
 
 ## Installation
 
 ```sh
-pip install itkwasm-dicom-emscripten
+import micropip
+await micropip.install('itkwasm-dicom-emscripten')
+```
+
+## Development
+
+```sh
+# Download test data
+cd ../../../..
+npm ci
+npm run build:testData
+cd -
+
+pip install hatch
+hatch run download-pyodide
+hatch run test
 ```
```

