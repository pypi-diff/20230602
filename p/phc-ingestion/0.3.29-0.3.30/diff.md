# Comparing `tmp/phc-ingestion-0.3.29.tar.gz` & `tmp/phc-ingestion-0.3.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phc-ingestion-0.3.29.tar", last modified: Thu Jun  1 09:40:27 2023, max compression
+gzip compressed data, was "phc-ingestion-0.3.30.tar", last modified: Fri Jun  2 17:59:01 2023, max compression
```

## Comparing `phc-ingestion-0.3.29.tar` & `phc-ingestion-0.3.30.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0       16 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/PYPI.md
--rw-r--r--   0        0        0        0 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/__init__.py
--rw-r--r--   0        0        0       61 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/caris/__init__.py
--rw-r--r--   0        0        0     1603 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/caris/process.py
--rw-r--r--   0        0        0        0 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/caris/util/__init__.py
--rw-r--r--   0        0        0     4738 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/caris/util/cnv.py
--rw-r--r--   0        0        0     1325 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/caris/util/detect_genome_ref.py
--rw-r--r--   0        0        0      629 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/caris/util/ga4gh.py
--rw-r--r--   0        0        0      555 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/caris/util/interpretation.py
--rw-r--r--   0        0        0     4636 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/caris/util/json.py
--rw-r--r--   0        0        0    21500 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/caris/util/metadata.py
--rw-r--r--   0        0        0     4948 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/caris/util/structural.py
--rw-r--r--   0        0        0      482 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/caris/util/tar.py
--rw-r--r--   0        0        0     1771 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/caris/util/tsv.py
--rw-r--r--   0        0        0     5010 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/caris/util/vcf.py
--rw-r--r--   0        0        0       49 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/foundation/__init__.py
--rw-r--r--   0        0        0     3127 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/foundation/process.py
--rw-r--r--   0        0        0        0 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/foundation/util/__init__.py
--rw-r--r--   0        0        0     4215 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/foundation/util/cnv.py
--rw-r--r--   0        0        0     5937 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/foundation/util/fnv.py
--rw-r--r--   0        0        0     8876 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/foundation/util/ga4gh.py
--rw-r--r--   0        0        0      405 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/foundation/util/interpretation.py
--rw-r--r--   0        0        0     3187 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/foundation/util/vcf_etl.py
--rw-r--r--   0        0        0       46 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/nextgen/__init__.py
--rw-r--r--   0        0        0     2802 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/nextgen/process.py
--rw-r--r--   0        0        0      297 2023-06-01 09:40:03.343839 phc-ingestion-0.3.29/ingestion/nextgen/util/interpretation.py
--rw-r--r--   0        0        0     2111 2023-06-01 09:40:03.347839 phc-ingestion-0.3.29/ingestion/nextgen/util/process_cnv.py
--rw-r--r--   0        0        0     6525 2023-06-01 09:40:03.347839 phc-ingestion-0.3.29/ingestion/nextgen/util/process_manifest.py
--rw-r--r--   0        0        0     3576 2023-06-01 09:40:03.347839 phc-ingestion-0.3.29/ingestion/nextgen/util/process_structural.py
--rw-r--r--   0        0        0     5430 2023-06-01 09:40:03.347839 phc-ingestion-0.3.29/ingestion/nextgen/util/process_vcf.py
--rw-r--r--   0        0        0       22 2023-06-01 09:40:03.347839 phc-ingestion-0.3.29/ingestion/nextgen/util/types.py
--rw-r--r--   0        0        0     1923 2023-06-01 09:40:03.347839 phc-ingestion-0.3.29/ingestion/nextgen/util/variant_table.py
--rw-r--r--   0        0        0   408290 2023-06-01 09:40:03.347839 phc-ingestion-0.3.29/ingestion/resources/GRCh37_map.csv.gz
--rw-r--r--   0        0        0   612373 2023-06-01 09:40:03.347839 phc-ingestion-0.3.29/ingestion/resources/GRCh38_map.csv.gz
--rw-r--r--   0        0        0        0 2023-06-01 09:40:03.347839 phc-ingestion-0.3.29/ingestion/shared_util/__init__.py
--rw-r--r--   0        0        0     1669 2023-06-01 09:40:03.347839 phc-ingestion-0.3.29/ingestion/shared_util/coords_to_genes.py
--rw-r--r--   0        0        0      876 2023-06-01 09:40:03.347839 phc-ingestion-0.3.29/ingestion/shared_util/gene_to_coords.py
--rw-r--r--   0        0        0     1029 2023-06-01 09:40:03.347839 phc-ingestion-0.3.29/pyproject.toml
--rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.3.29/PKG-INFO
+-rw-r--r--   0        0        0       16 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/PYPI.md
+-rw-r--r--   0        0        0        0 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/caris/__init__.py
+-rw-r--r--   0        0        0     1603 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/caris/process.py
+-rw-r--r--   0        0        0        0 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/caris/util/__init__.py
+-rw-r--r--   0        0        0     4738 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/caris/util/cnv.py
+-rw-r--r--   0        0        0     1325 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/caris/util/detect_genome_ref.py
+-rw-r--r--   0        0        0      629 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/caris/util/ga4gh.py
+-rw-r--r--   0        0        0      555 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/caris/util/interpretation.py
+-rw-r--r--   0        0        0     4636 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/caris/util/json.py
+-rw-r--r--   0        0        0    21500 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/caris/util/metadata.py
+-rw-r--r--   0        0        0     4948 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/caris/util/structural.py
+-rw-r--r--   0        0        0      482 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/caris/util/tar.py
+-rw-r--r--   0        0        0     1771 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/caris/util/tsv.py
+-rw-r--r--   0        0        0     5010 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/caris/util/vcf.py
+-rw-r--r--   0        0        0       49 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/foundation/__init__.py
+-rw-r--r--   0        0        0     3127 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/foundation/process.py
+-rw-r--r--   0        0        0        0 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/foundation/util/__init__.py
+-rw-r--r--   0        0        0     4215 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/foundation/util/cnv.py
+-rw-r--r--   0        0        0     5937 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/foundation/util/fnv.py
+-rw-r--r--   0        0        0     8876 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/foundation/util/ga4gh.py
+-rw-r--r--   0        0        0      405 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/foundation/util/interpretation.py
+-rw-r--r--   0        0        0     3187 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/foundation/util/vcf_etl.py
+-rw-r--r--   0        0        0       46 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/nextgen/__init__.py
+-rw-r--r--   0        0        0     2924 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/nextgen/process.py
+-rw-r--r--   0        0        0      297 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/nextgen/util/interpretation.py
+-rw-r--r--   0        0        0     2214 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/nextgen/util/process_cnv.py
+-rw-r--r--   0        0        0     7359 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/nextgen/util/process_manifest.py
+-rw-r--r--   0        0        0     3675 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/nextgen/util/process_structural.py
+-rw-r--r--   0        0        0     5503 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/nextgen/util/process_vcf.py
+-rw-r--r--   0        0        0       22 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/nextgen/util/types.py
+-rw-r--r--   0        0        0     2222 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/nextgen/util/variant_table.py
+-rw-r--r--   0        0        0   408290 2023-06-02 17:58:31.454668 phc-ingestion-0.3.30/ingestion/resources/GRCh37_map.csv.gz
+-rw-r--r--   0        0        0   612373 2023-06-02 17:58:31.458668 phc-ingestion-0.3.30/ingestion/resources/GRCh38_map.csv.gz
+-rw-r--r--   0        0        0        0 2023-06-02 17:58:31.458668 phc-ingestion-0.3.30/ingestion/shared_util/__init__.py
+-rw-r--r--   0        0        0     1669 2023-06-02 17:58:31.458668 phc-ingestion-0.3.30/ingestion/shared_util/coords_to_genes.py
+-rw-r--r--   0        0        0      876 2023-06-02 17:58:31.458668 phc-ingestion-0.3.30/ingestion/shared_util/gene_to_coords.py
+-rw-r--r--   0        0        0     1029 2023-06-02 17:58:31.458668 phc-ingestion-0.3.30/pyproject.toml
+-rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.3.30/PKG-INFO
```

### Comparing `phc-ingestion-0.3.29/ingestion/caris/process.py` & `phc-ingestion-0.3.30/ingestion/caris/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.29/ingestion/caris/util/cnv.py` & `phc-ingestion-0.3.30/ingestion/caris/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.29/ingestion/caris/util/detect_genome_ref.py` & `phc-ingestion-0.3.30/ingestion/caris/util/detect_genome_ref.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.29/ingestion/caris/util/ga4gh.py` & `phc-ingestion-0.3.30/ingestion/caris/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.29/ingestion/caris/util/interpretation.py` & `phc-ingestion-0.3.30/ingestion/caris/util/interpretation.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.29/ingestion/caris/util/json.py` & `phc-ingestion-0.3.30/ingestion/caris/util/json.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.29/ingestion/caris/util/metadata.py` & `phc-ingestion-0.3.30/ingestion/caris/util/metadata.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.29/ingestion/caris/util/structural.py` & `phc-ingestion-0.3.30/ingestion/caris/util/structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.29/ingestion/caris/util/tsv.py` & `phc-ingestion-0.3.30/ingestion/caris/util/tsv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.29/ingestion/caris/util/vcf.py` & `phc-ingestion-0.3.30/ingestion/caris/util/vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.29/ingestion/foundation/process.py` & `phc-ingestion-0.3.30/ingestion/foundation/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.29/ingestion/foundation/util/cnv.py` & `phc-ingestion-0.3.30/ingestion/foundation/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.29/ingestion/foundation/util/fnv.py` & `phc-ingestion-0.3.30/ingestion/foundation/util/fnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.29/ingestion/foundation/util/ga4gh.py` & `phc-ingestion-0.3.30/ingestion/foundation/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.29/ingestion/foundation/util/vcf_etl.py` & `phc-ingestion-0.3.30/ingestion/foundation/util/vcf_etl.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.29/ingestion/nextgen/process.py` & `phc-ingestion-0.3.30/ingestion/nextgen/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,18 +29,21 @@
         cnv_path_name = process_cnv(
             pdf_in_file=vendor_files["pdfFile"],
             cnv_in_file=vendor_files["somaticCnvTxtFile"],
             root_path=local_output_dir,
             prefix=prefix,
             log=log,
         )
+
+        xml_pdf_prefix = vendor_files["pdfFile"].split("/")[-1].split(".")[0]
         manifest = process_manifest(
-            pdf_in_file=vendor_files["pdfFile"],
+            xml_in_file=vendor_files["xmlFile"],
             source_file_id=source_file_id,
             prefix=prefix,
+            xml_pdf_prefix=xml_pdf_prefix,
             log=log,
         )
         structural_path_name = process_structural(
             pdf_in_file=vendor_files["pdfFile"],
             sv_in_file=vendor_files["somaticSvVcfFile"],
             root_path=local_output_dir,
             prefix=prefix,
```

### Comparing `phc-ingestion-0.3.29/ingestion/nextgen/util/process_cnv.py` & `phc-ingestion-0.3.30/ingestion/nextgen/util/process_cnv.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 
 
 def process_cnv(pdf_in_file: str, cnv_in_file: str, root_path: str, prefix: str, log: Logger):
     copy_number_path_name = f"{root_path}/{prefix}.copynumber.csv"
     sample_id = prefix
 
     copy_number_variant_rows = []
-    copy_number_variant_table = extract_variant_table(pdf=pdf_in_file, variant_type="copy number")
+    copy_number_variant_table = extract_variant_table(
+        pdf=pdf_in_file, variant_type="copy number", log=log
+    )
 
     with open(cnv_in_file, "r") as f:
         cnv_rows = f.readlines()
 
     for row in cnv_rows[1:]:
         working = row.strip().split("\t")
 
@@ -30,23 +32,24 @@
         status = working[5]
 
         # Hard-code
         attributes = {}
 
         # Scrape interpretation
         interpretation = None
-        for index, row in copy_number_variant_table.iterrows():
-            ref_gene = row["gene"].split(" ")[0]
-            ref_coord = row["gene"].split(" ")[1]
-
-            if (
-                ref_gene == gene_id_only
-                and ref_coord == f"({chromosome}:{start_position}_{end_position})"
-            ):
-                interpretation = map_interpretation(row["info"], log)
+        if not copy_number_variant_table.empty:
+            for index, row in copy_number_variant_table.iterrows():
+                ref_gene = row["gene"].split(" ")[0]
+                ref_coord = row["gene"].split(" ")[1]
+
+                if (
+                    ref_gene == gene_id_only
+                    and ref_coord == f"({chromosome}:{start_position}_{end_position})"
+                ):
+                    interpretation = map_interpretation(row["info"], log)
 
         if not interpretation:
             interpretation = "unknown"
 
         copy_number_variant_rows.append(
             f"{sample_id},{gene_id_only},{copy_number},{status},{attributes},{chromosome},{start_position},{end_position},{interpretation}\n"
         )
```

### Comparing `phc-ingestion-0.3.29/ingestion/nextgen/util/process_manifest.py` & `phc-ingestion-0.3.30/ingestion/nextgen/util/process_manifest.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,90 @@
+import re
 from ruamel.yaml import YAML
 from logging import Logger
 from pdfminer.high_level import extract_pages
 from pdfminer.layout import LTTextBoxHorizontal
 
 
 def transform_date(date: str):
     """mm/dd/yyyy -> yyyy-mm-dd"""
     date_list = date.split("/")
     new_date = f"{date_list[2]}-{date_list[0]}-{date_list[1]}"
     return new_date
 
 
-def extract_pdf_text(pdf_in_file: str):
-    pdf_text = {}
-    for page_layout in extract_pages(pdf_in_file, maxpages=1):
-        for element in page_layout:
-            if isinstance(element, LTTextBoxHorizontal):
-                if "PCM Result" in element.get_text():
-                    return pdf_text
-
-                else:
-                    row_text = element.get_text().strip()
-                    row_text_lower = row_text.lower().strip()
-                    pdf_text[row_text_lower] = row_text
+def search_and_grab(array: list, search_item: str, grab_index: int):
+    """Searches through an array for a string, and returns the item at the specified index after the search item"""
+    return array[array.index([i for i in array if re.search(search_item, i)][0]) + grab_index]
+
+
+def extract_xml_text(xml_in_file: str):
+    with open(xml_in_file, "r") as f:
+        xml_lines = f.readlines()
+
+    in_range_trigger = False
+    patient_info_lines = []
+    for line in xml_lines:
+        if "Diagnostic Genomics Laboratory " in line:
+            in_range_trigger = True
+        if "PCM Result:" in line:
+            in_range_trigger = False
+            break
+        if in_range_trigger == True:
+            patient_info_lines.append(line.strip())
 
+    return patient_info_lines
 
-def extract_patient_data(pdf_text: dict):
+
+def extract_patient_data(patient_info_lines: list):
     patient_data = {}
     patient_data["patientInfo"] = {}
 
-    for row_text_lower, row_text in pdf_text.items():
-        if "patientLastName" not in patient_data and "Patient Name".lower() in row_text_lower:
-            patientNameArray = row_text.split(":")[1].strip().split(",")
-            first = patientNameArray[1].strip()
-            last = patientNameArray[0].strip()
+    for line in patient_info_lines:
+        if "patientLastName" not in patient_data and "Patient Name" in line:
+            patientNameArray = line.split(" ")
+            first = search_and_grab(patientNameArray, "Name:", 2)
+            last = search_and_grab(patientNameArray, "Name:", 1).strip(", ")
             patient_data["patientInfo"]["firstName"] = first
             patient_data["patientInfo"]["lastName"] = last
             patient_data["patientLastName"] = last
 
-        elif "patientDOB" not in patient_data and "Birthdate".lower() in row_text_lower:
-            dob = row_text.split(":")[1].strip()
+        if "patientDOB" not in patient_data and "Birthdate" in line:
+            dobArray = line.split(" ")
+            dob = search_and_grab(dobArray, "Birthdate:", 1)
             patient_data["patientDOB"] = transform_date(dob)
             patient_data["patientInfo"]["dob"] = transform_date(dob)
 
-        elif "mrn" not in patient_data and "MRN #".lower() in row_text_lower:
-            mrn = row_text.split(":")[1].strip()
+        if "mrn" not in patient_data and "MRN #" in line:
+            mrnArray = line.split(" ")
+            mrn = search_and_grab(mrnArray, "MRN", 2)
             patient_data["mrn"] = mrn
             patient_data["patientInfo"]["identifiers"] = [
                 {
                     "codingCode": "MR",
                     "codingSystem": "http://hl7.org/fhir/v2/0203",
                     "value": mrn,
                 }
             ]
 
-        elif "gender" not in patient_data["patientInfo"] and "Gender".lower() in row_text_lower:
-            gender = row_text.split(":")[1].strip()
+        if "gender" not in patient_data["patientInfo"] and "Gender" in line:
+            genderArray = line.split(" ")
+            gender = search_and_grab(genderArray, "Gender", 1)
             if gender == "F":
                 gender = "female"
             elif gender == "M":
                 gender = "male"
             else:
                 gender = "other"
             patient_data["patientInfo"]["gender"] = gender
 
     return patient_data
 
 
-def extract_test_data(pdf_text: dict):
+def extract_test_data(patient_info_lines: dict):
     # Initialize manifest and hard-code some values
     manifest = {}
     manifest["testType"] = "NextGen"
     manifest["name"] = "IU Diagnostic Genomics"
     manifest["reference"] = "GRCh38"
 
     manifest["ihcTests"] = []
@@ -80,68 +93,71 @@
 
     manifest["bodySiteSystem"] = "http://lifeomic.com/fhir/sequence-body-site"
     manifest["indicationSystem"] = "http://lifeomic.com/fhir/sequence-indication"
 
     manifest["medFacilID"] = ""
     manifest["medFacilName"] = "IU Health"
 
-    manifest["reportDate"] = transform_date(list(pdf_text)[1])
-
-    for row_text_lower, row_text in pdf_text.items():
-        if "collected" in row_text_lower:
-            coll_date = pdf_text.get(row_text_lower, "")
-            if coll_date != "":
-                coll_date = transform_date(coll_date.split(":")[1].strip())
-            manifest["collDate"] = coll_date
-
-        elif "received" in row_text_lower:
-            rec_date = pdf_text.get(row_text_lower, "")
-            if rec_date != "":
-                rec_date = transform_date(rec_date.split(":")[1].strip())
-            manifest["receivedDate"] = rec_date
-
-        elif "accession" in row_text_lower:
-            report_id = pdf_text.get(row_text_lower, "")
-            if report_id != "":
-                report_id = report_id.split(":")[1].strip()
+    for line in patient_info_lines:
+        if "reportDate" not in manifest and "Laboratory" in line:
+            reportArray = line.split(" ")
+            report_date = search_and_grab(reportArray, "Laboratory", 1)
+            manifest["reportDate"] = transform_date(report_date)
+
+        if "collDate" not in manifest and "Collected" in line:
+            collArray = line.split(" ")
+            coll_date = search_and_grab(collArray, "Collected", 1)
+            manifest["collDate"] = transform_date(coll_date)
+
+        if "receivedDate" not in manifest and "Received" in line:
+            recArray = line.split(" ")
+            rec_date = search_and_grab(recArray, "Received", 1)
+            manifest["receivedDate"] = transform_date(rec_date)
+
+        if "reportID" not in manifest and "Accession" in line:
+            reportArray = line.split(" ")
+            report_id = search_and_grab(reportArray, "Accession", 2)
             manifest["reportID"] = report_id
 
-        elif "physician" in row_text_lower:
-            phys_name = pdf_text.get(row_text_lower, "")
-            if phys_name != "":
-                phys_name = phys_name.split(":")[1].strip()
-            manifest["orderingMDName"] = phys_name
-
-        elif "reason for referral" in row_text_lower:
-            indication = pdf_text.get(row_text_lower, "")
-            if indication != "":
-                indication = indication.split(":")[1].strip()
+        if "orderingMDName" not in manifest and "Physician Name:" in line:
+            physArray = line.split(" ")
+            phys_last = search_and_grab(physArray, "Name:", 1)
+            phys_first = search_and_grab(physArray, "Name:", 2)
+            manifest["orderingMDName"] = f"{phys_last} {phys_first}"
+
+        if "indication" not in manifest and "Reason for Referral" in line:
+            indicationArray = line.split(" ")
+            indication = search_and_grab(indicationArray, "Referral", 1)
+            # Accounting for two-word indication
+            if "</" not in search_and_grab(indicationArray, "Referral", 2):
+                indication = f'{indication} {search_and_grab(indicationArray, "Referral", 2)}'
             manifest["indication"] = indication
             manifest["indicationDisplay"] = indication
 
-        elif "specimen" in row_text_lower:
-            body_site = pdf_text.get(row_text_lower, "")
-            if body_site != "":
-                body_site = body_site.split(":")[1].strip("\nAge").strip()
-            manifest["bodySite"] = body_site
-            manifest["bodySiteDisplay"] = body_site
+        if "bodySite" not in manifest and "Specimen:" in line:
+            bodySiteArray = line.split(" ")
+            body_site_one = search_and_grab(bodySiteArray, "Specimen:", 1)
+            body_site_two = search_and_grab(bodySiteArray, "Specimen:", 2)
+            manifest["bodySite"] = f"{body_site_one} {body_site_two}"
+            manifest["bodySiteDisplay"] = f"{body_site_one} {body_site_two}"
 
     return manifest
 
 
-def process_manifest(pdf_in_file: str, source_file_id: str, prefix: str, log: Logger):
-    pdf_text = extract_pdf_text(pdf_in_file)
-    manifest = extract_test_data(pdf_text)
-    manifest.update(extract_patient_data(pdf_text))
+def process_manifest(
+    xml_in_file: str, source_file_id: str, prefix: str, xml_pdf_prefix: str, log: Logger
+):
+    xml_text = extract_xml_text(xml_in_file)
+    manifest = extract_test_data(xml_text)
+    manifest.update(extract_patient_data(xml_text))
 
-    manifest["reportFile"] = f".lifeomic/nextgen/{prefix}/{prefix}.pdf"
+    manifest["reportFile"] = f".lifeomic/nextgen/{prefix}/{xml_pdf_prefix}.pdf"
     manifest["sourceFileId"] = source_file_id
     manifest["resources"] = [
-        {"fileName": f".lifeomic/nextgen/{prefix}/{prefix}.pdf"},
-        {"fileName": f".lifeomic/nextgen/{prefix}/{prefix}.xml"},
+        {"fileName": f".lifeomic/nextgen/{prefix}/{xml_pdf_prefix}.pdf"},
     ]
 
     manifest["files"] = [
         {
             "fileName": f".lifeomic/nextgen/{prefix}/{prefix}.copynumber.csv",
             "sequenceType": "somatic",
             "type": "copyNumberVariant",
```

### Comparing `phc-ingestion-0.3.29/ingestion/nextgen/util/process_structural.py` & `phc-ingestion-0.3.30/ingestion/nextgen/util/process_structural.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 
 from ingestion.shared_util.coords_to_genes import coords_to_genes
 from ingestion.nextgen.util.variant_table import extract_variant_table
 from ingestion.nextgen.util.interpretation import map_interpretation
 
 
 def process_structural(sv_in_file: str, pdf_in_file, root_path: str, prefix: str, log: Logger):
-    structural_variant_table = extract_variant_table(pdf=pdf_in_file, variant_type="structural")
+    structural_variant_table = extract_variant_table(
+        pdf=pdf_in_file, variant_type="structural", log=log
+    )
 
     structural_variant_path_name = f"{root_path}/{prefix}.structural.csv"
     sample_id = prefix
 
     with open(sv_in_file, "r") as f:
         variants = [line for line in f.readlines() if not line.startswith("#")]
 
@@ -32,43 +34,44 @@
             chromosome2 = chromosome1
             start_position2 = start_position1
             end_position2 = end_position2
             effect = "deletion" if working_variant[4] == "<DEL>" else "duplication"
 
             # Get genes from coordinates using center point of start and end positions
             gene1 = coords_to_genes(
-                "GRCh38", chromosome1, ((int(start_position1) + int(end_position1)) / 2), log
+                "GRCh38", chromosome1, int((int(start_position1) + int(end_position1)) / 2), log
             )
             gene2 = "N/A"
 
         else:
             alt = working_variant[4].strip("][TCGA").split(":")
 
             end_position1 = start_position1
             chromosome2 = f"chr{alt[0]}"
             start_position2 = alt[1]
             end_position2 = alt[1]
             effect = "translocation"
 
             # Get genes from coordinates using center point of start and end positions
             gene1 = coords_to_genes(
-                "GRCh38", chromosome1, ((int(start_position1) + int(end_position1)) / 2), log
+                "GRCh38", chromosome1, int((int(start_position1) + int(end_position1)) / 2), log
             )
             gene2 = coords_to_genes(
-                "GRCh38", chromosome2, ((int(start_position2) + int(end_position2)) / 2), log
+                "GRCh38", chromosome2, int((int(start_position2) + int(end_position2)) / 2), log
             )
 
         # Scrape interpretation
         interpretation = None
-        for index, row in structural_variant_table.iterrows():
-            ref_gene1 = row["gene"].split(" ")[0].split("-")[0]
-            ref_coord = row["gene"].split(" ")[1].split(";")[0].strip("(")
+        if not structural_variant_table.empty:
+            for index, row in structural_variant_table.iterrows():
+                ref_gene1 = row["gene"].split(" ")[0].split("-")[0]
+                ref_coord = row["gene"].split(" ")[1].split(";")[0].strip("(")
 
-            if ref_gene1 == gene1 and ref_coord == f"{chromosome1}:{start_position1}":
-                interpretation = map_interpretation(row["info"], log)
+                if ref_gene1 == gene1 and ref_coord == f"{chromosome1}:{start_position1}":
+                    interpretation = map_interpretation(row["info"], log)
 
         if not interpretation:
             interpretation = "unknown"
 
         # Hard-code
         sequence_type = "Somatic"
         in_frame = "Unknown"
```

### Comparing `phc-ingestion-0.3.29/ingestion/nextgen/util/process_vcf.py` & `phc-ingestion-0.3.30/ingestion/nextgen/util/process_vcf.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,18 @@
 
         ad_split = ad.split(",")
         total_dp = sum([int(i) for i in ad_split])
 
         afs = []
         # Start at the first REF allele
         for ad in ad_split[1:]:
-            af = float(int(ad) / total_dp)
+            if ad == "0":
+                af = 0.0
+            else:
+                af = float(int(ad) / total_dp)
             afs.append("{:.4f}".format(af))
 
         self.info.append(f'AF={",".join(afs)}')
 
     def prune_var(self):
         # Pruning FORMAT to only include GT, AD, and DP values.
         # Pruning VARIANT column to only include the corresponding values.
```

### Comparing `phc-ingestion-0.3.29/ingestion/nextgen/util/variant_table.py` & `phc-ingestion-0.3.30/ingestion/nextgen/util/variant_table.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from logging import Logger
 import pandas as pd
 from pdfminer.high_level import extract_pages
 from pdfminer.layout import LTTextBoxHorizontal
 
 
-def extract_variant_table(pdf: str, variant_type: str):
+def extract_variant_table(pdf: str, variant_type: str, log: Logger):
     # Narrow down to variant table entries
     in_range_trigger = False
     table_entries = []
     for page_layout in extract_pages(pdf, maxpages=2):
         for element in page_layout:
             if isinstance(element, LTTextBoxHorizontal):
                 if "Clinical\nInformation\n" in element.get_text():
@@ -31,14 +31,20 @@
     for coordinate in sorted(list(coordinate_set)):
         column = []
         for entry in table_entries:
             if round(int(entry.bbox[0]), -1) == coordinate:
                 column.append(entry.get_text().strip().replace("\n", " "))
         table_columns.append(column)
 
+    # If the test is negative we will have a table with only NA values
+    # We return an empty df which we check for later when scraping annotations
+    if set(table_columns[0]) == {"NA"}:
+        log.info(f"No variants present in {variant_type} table")
+        return pd.DataFrame()
+
     variant_df = pd.DataFrame(
         {
             "gene": table_columns[0],
             "type": table_columns[1],
             "description": table_columns[2],
             "vaf": table_columns[3],
             "info": table_columns[4],
```

### Comparing `phc-ingestion-0.3.29/ingestion/resources/GRCh37_map.csv.gz` & `phc-ingestion-0.3.30/ingestion/resources/GRCh37_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.29/ingestion/resources/GRCh38_map.csv.gz` & `phc-ingestion-0.3.30/ingestion/resources/GRCh38_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.29/ingestion/shared_util/coords_to_genes.py` & `phc-ingestion-0.3.30/ingestion/shared_util/coords_to_genes.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.29/ingestion/shared_util/gene_to_coords.py` & `phc-ingestion-0.3.30/ingestion/shared_util/gene_to_coords.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.29/pyproject.toml` & `phc-ingestion-0.3.30/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phc-ingestion"
-version = "0.3.29"
+version = "0.3.30"
 description = "Functions for LifeOmic PHC genomic ingestions"
 authors = [
     { name = "LifeOmic Development", email = "development@lifeomic.com" },
 ]
 dependencies = [
     "lifeomic-logging>=0.3.2,<0.4.0",
     "xmltodict==0.13.0",
```

