# Comparing `tmp/amazon-textract-prettyprinter-0.1.2.tar.gz` & `tmp/amazon-textract-prettyprinter-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-textract-prettyprinter-0.1.2.tar", last modified: Tue Mar 21 23:44:46 2023, max compression
+gzip compressed data, was "amazon-textract-prettyprinter-0.1.3.tar", last modified: Fri Jun  2 00:17:49 2023, max compression
```

## Comparing `amazon-textract-prettyprinter-0.1.2.tar` & `amazon-textract-prettyprinter-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 schadem    (504) staff       (20)        0 2023-03-21 23:44:46.291658 amazon-textract-prettyprinter-0.1.2/
--rw-r--r--   0 schadem    (504) staff       (20)    10142 2022-09-08 17:40:40.000000 amazon-textract-prettyprinter-0.1.2/LICENSE
--rw-r--r--   0 schadem    (504) staff       (20)      161 2022-09-08 17:40:40.000000 amazon-textract-prettyprinter-0.1.2/MANIFEST.in
--rw-r--r--   0 schadem    (504) staff       (20)     3092 2023-03-21 23:44:46.291745 amazon-textract-prettyprinter-0.1.2/PKG-INFO
--rw-r--r--   0 schadem    (504) staff       (20)     1835 2023-03-14 19:55:05.000000 amazon-textract-prettyprinter-0.1.2/README.md
-drwxr-xr-x   0 schadem    (504) staff       (20)        0 2023-03-21 23:44:46.290594 amazon-textract-prettyprinter-0.1.2/amazon_textract_prettyprinter.egg-info/
--rw-r--r--   0 schadem    (504) staff       (20)     3092 2023-03-21 23:44:46.000000 amazon-textract-prettyprinter-0.1.2/amazon_textract_prettyprinter.egg-info/PKG-INFO
--rw-r--r--   0 schadem    (504) staff       (20)      468 2023-03-21 23:44:46.000000 amazon-textract-prettyprinter-0.1.2/amazon_textract_prettyprinter.egg-info/SOURCES.txt
--rw-r--r--   0 schadem    (504) staff       (20)        1 2023-03-21 23:44:46.000000 amazon-textract-prettyprinter-0.1.2/amazon_textract_prettyprinter.egg-info/dependency_links.txt
--rw-r--r--   0 schadem    (504) staff       (20)       71 2023-03-21 23:44:46.000000 amazon-textract-prettyprinter-0.1.2/amazon_textract_prettyprinter.egg-info/requires.txt
--rw-r--r--   0 schadem    (504) staff       (20)       22 2023-03-21 23:44:46.000000 amazon-textract-prettyprinter-0.1.2/amazon_textract_prettyprinter.egg-info/top_level.txt
--rw-r--r--   0 schadem    (504) staff       (20)      406 2023-03-21 23:44:46.292079 amazon-textract-prettyprinter-0.1.2/setup.cfg
--rw-r--r--   0 schadem    (504) staff       (20)     1938 2023-03-21 23:42:08.000000 amazon-textract-prettyprinter-0.1.2/setup.py
-drwxr-xr-x   0 schadem    (504) staff       (20)        0 2023-03-21 23:44:46.291346 amazon-textract-prettyprinter-0.1.2/textractprettyprinter/
--rw-r--r--   0 schadem    (504) staff       (20)      220 2022-12-20 03:08:04.000000 amazon-textract-prettyprinter-0.1.2/textractprettyprinter/__init__.py
--rw-r--r--   0 schadem    (504) staff       (20)       23 2023-03-21 23:42:08.000000 amazon-textract-prettyprinter-0.1.2/textractprettyprinter/_version.py
--rw-r--r--   0 schadem    (504) staff       (20)    24989 2023-03-21 23:41:48.000000 amazon-textract-prettyprinter-0.1.2/textractprettyprinter/t_pretty_print.py
--rw-r--r--   0 schadem    (504) staff       (20)    10901 2022-12-20 03:08:04.000000 amazon-textract-prettyprinter-0.1.2/textractprettyprinter/t_pretty_print_expense.py
+drwxr-xr-x   0 schadem    (504) staff       (20)        0 2023-06-02 00:17:49.918577 amazon-textract-prettyprinter-0.1.3/
+-rw-r--r--   0 schadem    (504) staff       (20)    10142 2022-09-08 17:40:40.000000 amazon-textract-prettyprinter-0.1.3/LICENSE
+-rw-r--r--   0 schadem    (504) staff       (20)      161 2022-09-08 17:40:40.000000 amazon-textract-prettyprinter-0.1.3/MANIFEST.in
+-rw-r--r--   0 schadem    (504) staff       (20)     3092 2023-06-02 00:17:49.918668 amazon-textract-prettyprinter-0.1.3/PKG-INFO
+-rw-r--r--   0 schadem    (504) staff       (20)     1835 2023-03-14 19:55:05.000000 amazon-textract-prettyprinter-0.1.3/README.md
+drwxr-xr-x   0 schadem    (504) staff       (20)        0 2023-06-02 00:17:49.917545 amazon-textract-prettyprinter-0.1.3/amazon_textract_prettyprinter.egg-info/
+-rw-r--r--   0 schadem    (504) staff       (20)     3092 2023-06-02 00:17:49.000000 amazon-textract-prettyprinter-0.1.3/amazon_textract_prettyprinter.egg-info/PKG-INFO
+-rw-r--r--   0 schadem    (504) staff       (20)      468 2023-06-02 00:17:49.000000 amazon-textract-prettyprinter-0.1.3/amazon_textract_prettyprinter.egg-info/SOURCES.txt
+-rw-r--r--   0 schadem    (504) staff       (20)        1 2023-06-02 00:17:49.000000 amazon-textract-prettyprinter-0.1.3/amazon_textract_prettyprinter.egg-info/dependency_links.txt
+-rw-r--r--   0 schadem    (504) staff       (20)       71 2023-06-02 00:17:49.000000 amazon-textract-prettyprinter-0.1.3/amazon_textract_prettyprinter.egg-info/requires.txt
+-rw-r--r--   0 schadem    (504) staff       (20)       22 2023-06-02 00:17:49.000000 amazon-textract-prettyprinter-0.1.3/amazon_textract_prettyprinter.egg-info/top_level.txt
+-rw-r--r--   0 schadem    (504) staff       (20)      406 2023-06-02 00:17:49.918969 amazon-textract-prettyprinter-0.1.3/setup.cfg
+-rw-r--r--   0 schadem    (504) staff       (20)     1938 2023-06-02 00:17:44.000000 amazon-textract-prettyprinter-0.1.3/setup.py
+drwxr-xr-x   0 schadem    (504) staff       (20)        0 2023-06-02 00:17:49.918319 amazon-textract-prettyprinter-0.1.3/textractprettyprinter/
+-rw-r--r--   0 schadem    (504) staff       (20)      220 2022-12-20 03:08:04.000000 amazon-textract-prettyprinter-0.1.3/textractprettyprinter/__init__.py
+-rw-r--r--   0 schadem    (504) staff       (20)       23 2023-06-02 00:17:44.000000 amazon-textract-prettyprinter-0.1.3/textractprettyprinter/_version.py
+-rw-r--r--   0 schadem    (504) staff       (20)    25965 2023-06-02 00:17:28.000000 amazon-textract-prettyprinter-0.1.3/textractprettyprinter/t_pretty_print.py
+-rw-r--r--   0 schadem    (504) staff       (20)    10901 2022-12-20 03:08:04.000000 amazon-textract-prettyprinter-0.1.3/textractprettyprinter/t_pretty_print_expense.py
```

### Comparing `amazon-textract-prettyprinter-0.1.2/LICENSE` & `amazon-textract-prettyprinter-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon-textract-prettyprinter-0.1.2/PKG-INFO` & `amazon-textract-prettyprinter-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-textract-prettyprinter
-Version: 0.1.2
+Version: 0.1.3
 Summary: Amazon Textract Helper tools for pretty printing
 Home-page: https://github.com/aws-samples/amazon-textract-textractor/tree/master/prettyprinter
 Author: Amazon Rekognition Textract Demoes
 Author-email: rekognition-textract-demos@amazon.com
 License: Apache License Version 2.0
 Description: # Textract-PrettyPrinter
```

### Comparing `amazon-textract-prettyprinter-0.1.2/README.md` & `amazon-textract-prettyprinter-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `amazon-textract-prettyprinter-0.1.2/amazon_textract_prettyprinter.egg-info/PKG-INFO` & `amazon-textract-prettyprinter-0.1.3/amazon_textract_prettyprinter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-textract-prettyprinter
-Version: 0.1.2
+Version: 0.1.3
 Summary: Amazon Textract Helper tools for pretty printing
 Home-page: https://github.com/aws-samples/amazon-textract-textractor/tree/master/prettyprinter
 Author: Amazon Rekognition Textract Demoes
 Author-email: rekognition-textract-demos@amazon.com
 License: Apache License Version 2.0
 Description: # Textract-PrettyPrinter
```

### Comparing `amazon-textract-prettyprinter-0.1.2/setup.py` & `amazon-textract-prettyprinter-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
-requirements = ['boto3', 'botocore', 'amazon-textract-response-parser>=0.1.44', 'tabulate==0.9.*']
+requirements = ['boto3', 'botocore', 'amazon-textract-response-parser>=0.1.48', 'tabulate==0.9.*']
 
 if sys.argv[-1] == 'publish-test':
     os.system(f"cd {os.path.dirname(__file__)}")
     os.system('rm -rf dist/ build/ amazon_textract_prettyprinter.egg-info/')
     os.system('python setup.py sdist bdist_wheel')
     os.system('twine check dist/*')
     os.system('twine upload --repository pypitest dist/*')
@@ -23,15 +23,15 @@
     os.system('python setup.py sdist bdist_wheel')
     os.system('twine check dist/*')
     os.system('twine upload --repository pypi dist/*')
     sys.exit()
 
 setup(name='amazon-textract-prettyprinter',
       packages=['textractprettyprinter'],
-      version='0.1.2',
+      version='0.1.3',
       description='Amazon Textract Helper tools for pretty printing',
       install_requires=requirements,
       long_description_content_type='text/markdown',
       long_description=read('README.md'),
       author='Amazon Rekognition Textract Demoes',
       author_email='rekognition-textract-demos@amazon.com',
       url='https://github.com/aws-samples/amazon-textract-textractor/tree/master/prettyprinter',
```

### Comparing `amazon-textract-prettyprinter-0.1.2/textractprettyprinter/t_pretty_print.py` & `amazon-textract-prettyprinter-0.1.3/textractprettyprinter/t_pretty_print.py`

 * *Files 4% similar despite different names*

```diff
@@ -133,22 +133,22 @@
                     key_value = ""
                     value_geometry = TGeometry(TBoundingBox(width=0, height=0, top=0, left=0), polygon=[TPoint(0, 0)])
                     value_confidence = 1
                 page_keys.append([
                     str(idx + 1), key_name,
                     str(key_confidence), key_value,
                     str(value_confidence),
-                    str(key_geometry.bounding_box.top),
-                    str(key_geometry.bounding_box.height),
-                    str(key_geometry.bounding_box.width),
-                    str(key_geometry.bounding_box.left),
-                    str(value_geometry.bounding_box.top),
-                    str(value_geometry.bounding_box.height),
-                    str(value_geometry.bounding_box.width),
-                    str(value_geometry.bounding_box.left)
+                    str(key_geometry.bounding_box.top) if key_geometry and key_geometry.bounding_box else "0",
+                    str(key_geometry.bounding_box.height) if key_geometry and key_geometry.bounding_box else "0",
+                    str(key_geometry.bounding_box.width) if key_geometry and key_geometry.bounding_box else "0",
+                    str(key_geometry.bounding_box.left) if key_geometry and key_geometry.bounding_box else "0",
+                    str(value_geometry.bounding_box.top) if value_geometry and value_geometry.bounding_box else "0",
+                    str(value_geometry.bounding_box.height) if value_geometry and value_geometry.bounding_box else "0",
+                    str(value_geometry.bounding_box.width) if value_geometry and value_geometry.bounding_box else "0",
+                    str(value_geometry.bounding_box.left) if value_geometry and value_geometry.bounding_box else "0"
                 ])
         page_list.append(page_keys)
     return page_list
 
 
 def convert_queries_to_list_trp2(trp2_doc: TDocument) -> List[List[List[str]]]:
     '''return List[List[List[str]]]
@@ -166,18 +166,20 @@
             answer_blocks: List[TBlock] = [x for x in trp2_doc.get_answers_for_query(block=query)]
             if answer_blocks:
                 for answer in answer_blocks:
                     value_geometry = TDocument.create_geometry_from_blocks([answer])
                     page_keys.append([
                         str(idx + 1), key, "1", answer.text,
                         str(answer.confidence), "0", "0", "0", "0",
-                        str(value_geometry.bounding_box.top),
-                        str(value_geometry.bounding_box.height),
-                        str(value_geometry.bounding_box.width),
-                        str(value_geometry.bounding_box.left)
+                        str(value_geometry.bounding_box.top) if value_geometry and value_geometry.bounding_box else "0",
+                        str(value_geometry.bounding_box.height)
+                        if value_geometry and value_geometry.bounding_box else "0",
+                        str(value_geometry.bounding_box.width)
+                        if value_geometry and value_geometry.bounding_box else "0",
+                        str(value_geometry.bounding_box.left) if value_geometry and value_geometry.bounding_box else "0"
                     ])
             else:
                 # no answer found
                 page_keys.append([str(idx + 1), key, "1", "", "1", "0", "0", "0", "0", "0", "0", "0", "0 "])
         page_list.append(page_keys)
     return page_list
 
@@ -190,18 +192,18 @@
     for idx, page_block in enumerate(trp2_doc.pages):
         page_signatures: List[List[str]] = list()
         for signature in trp2_doc.signatures(page=page_block):
             value_geometry = TDocument.create_geometry_from_blocks([signature])
             page_signatures.append([
                 str(idx + 1), "SIGNATURE", "1", "exists",
                 str(signature.confidence), "0", "0", "0", "0",
-                str(value_geometry.bounding_box.top),
-                str(value_geometry.bounding_box.height),
-                str(value_geometry.bounding_box.width),
-                str(value_geometry.bounding_box.left)
+                str(value_geometry.bounding_box.top) if value_geometry and value_geometry.bounding_box else "0",
+                str(value_geometry.bounding_box.height) if value_geometry and value_geometry.bounding_box else "0",
+                str(value_geometry.bounding_box.width) if value_geometry and value_geometry.bounding_box else "0",
+                str(value_geometry.bounding_box.left) if value_geometry and value_geometry.bounding_box else "0"
             ])
         page_list.append(page_signatures)
     return page_list
 
 
 def convert_form_to_list(trp_form: trp.Form,
                          with_confidence: bool = False,
```

### Comparing `amazon-textract-prettyprinter-0.1.2/textractprettyprinter/t_pretty_print_expense.py` & `amazon-textract-prettyprinter-0.1.3/textractprettyprinter/t_pretty_print_expense.py`

 * *Files identical despite different names*

