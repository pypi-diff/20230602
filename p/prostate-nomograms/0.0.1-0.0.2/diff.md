# Comparing `tmp/prostate-nomograms-0.0.1.tar.gz` & `tmp/prostate-nomograms-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prostate-nomograms-0.0.1.tar", last modified: Fri Jun  2 19:37:54 2023, max compression
+gzip compressed data, was "prostate-nomograms-0.0.2.tar", last modified: Fri Jun  2 19:46:06 2023, max compression
```

## Comparing `prostate-nomograms-0.0.1.tar` & `prostate-nomograms-0.0.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 19:37:54.379783 prostate-nomograms-0.0.1/
--rw-rw-rw-   0        0        0    11558 2023-05-09 17:06:15.000000 prostate-nomograms-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     3107 2023-06-02 19:37:54.379783 prostate-nomograms-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2497 2023-06-02 19:07:37.000000 prostate-nomograms-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 19:37:54.273211 prostate-nomograms-0.0.1/examples/
--rw-rw-rw-   0        0        0        0 2023-05-09 17:06:15.000000 prostate-nomograms-0.0.1/examples/__init__.py
--rw-rw-rw-   0        0        0      150 2023-05-09 17:06:15.000000 prostate-nomograms-0.0.1/examples/env_examples.py
--rw-rw-rw-   0        0        0     3569 2023-06-02 19:21:40.000000 prostate-nomograms-0.0.1/examples/ex01-mskcc.py
--rw-rw-rw-   0        0        0     3781 2023-06-02 19:21:40.000000 prostate-nomograms-0.0.1/examples/ex02-capra.py
--rw-rw-rw-   0        0        0     3914 2023-06-02 19:21:40.000000 prostate-nomograms-0.0.1/examples/ex03-custom.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:37:54.283135 prostate-nomograms-0.0.1/prostate_nomograms/
--rw-rw-rw-   0        0        0      185 2023-06-02 19:10:35.000000 prostate-nomograms-0.0.1/prostate_nomograms/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:37:54.306310 prostate-nomograms-0.0.1/prostate_nomograms/capra/
--rw-rw-rw-   0        0        0       34 2023-06-02 19:10:35.000000 prostate-nomograms-0.0.1/prostate_nomograms/capra/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:37:54.321847 prostate-nomograms-0.0.1/prostate_nomograms/capra/base/
--rw-rw-rw-   0        0        0      106 2023-05-31 14:34:11.000000 prostate-nomograms-0.0.1/prostate_nomograms/capra/base/__init__.py
--rw-rw-rw-   0        0        0     1336 2023-06-01 15:55:16.000000 prostate-nomograms-0.0.1/prostate_nomograms/capra/base/logistic_regression.py
--rw-rw-rw-   0        0        0     2273 2023-05-31 23:11:28.000000 prostate-nomograms-0.0.1/prostate_nomograms/capra/base/survival_regression.py
--rw-rw-rw-   0        0        0    12574 2023-06-02 19:10:35.000000 prostate-nomograms-0.0.1/prostate_nomograms/capra/capra.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:37:54.331935 prostate-nomograms-0.0.1/prostate_nomograms/custom/
--rw-rw-rw-   0        0        0       36 2023-05-31 19:54:31.000000 prostate-nomograms-0.0.1/prostate_nomograms/custom/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:37:54.342786 prostate-nomograms-0.0.1/prostate_nomograms/custom/base/
--rw-rw-rw-   0        0        0      106 2023-05-31 14:34:11.000000 prostate-nomograms-0.0.1/prostate_nomograms/custom/base/__init__.py
--rw-rw-rw-   0        0        0     1282 2023-06-01 15:55:16.000000 prostate-nomograms-0.0.1/prostate_nomograms/custom/base/logistic_regression.py
--rw-rw-rw-   0        0        0     2192 2023-05-31 15:13:00.000000 prostate-nomograms-0.0.1/prostate_nomograms/custom/base/survival_regression.py
--rw-rw-rw-   0        0        0     9078 2023-05-31 22:07:18.000000 prostate-nomograms-0.0.1/prostate_nomograms/custom/custom.py
--rw-rw-rw-   0        0        0     1162 2023-06-02 19:10:35.000000 prostate-nomograms-0.0.1/prostate_nomograms/enum.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:37:54.351786 prostate-nomograms-0.0.1/prostate_nomograms/mskcc/
--rw-rw-rw-   0        0        0       86 2023-06-02 19:10:35.000000 prostate-nomograms-0.0.1/prostate_nomograms/mskcc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:37:54.378782 prostate-nomograms-0.0.1/prostate_nomograms/mskcc/base/
--rw-rw-rw-   0        0        0       26 2023-05-31 14:34:11.000000 prostate-nomograms-0.0.1/prostate_nomograms/mskcc/base/__init__.py
--rw-rw-rw-   0        0        0     9792 2023-05-31 14:34:11.000000 prostate-nomograms-0.0.1/prostate_nomograms/mskcc/base/logistic_regression.py
--rw-rw-rw-   0        0        0    10577 2023-05-31 22:05:59.000000 prostate-nomograms-0.0.1/prostate_nomograms/mskcc/base/model.py
--rw-rw-rw-   0        0        0     2533 2023-05-31 14:34:11.000000 prostate-nomograms-0.0.1/prostate_nomograms/mskcc/base/survival_regression.py
--rw-rw-rw-   0        0        0     5490 2023-05-31 14:34:11.000000 prostate-nomograms-0.0.1/prostate_nomograms/mskcc/base/web_table_scraper.py
--rw-rw-rw-   0        0        0     2841 2023-06-02 19:10:35.000000 prostate-nomograms-0.0.1/prostate_nomograms/mskcc/pre_radical_prostatectomy_nomogram.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:37:54.296141 prostate-nomograms-0.0.1/prostate_nomograms.egg-info/
--rw-rw-rw-   0        0        0     3107 2023-06-02 19:37:54.000000 prostate-nomograms-0.0.1/prostate_nomograms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1191 2023-06-02 19:37:54.000000 prostate-nomograms-0.0.1/prostate_nomograms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 19:37:54.000000 prostate-nomograms-0.0.1/prostate_nomograms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-06-02 19:37:54.000000 prostate-nomograms-0.0.1/prostate_nomograms.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-06-02 19:37:54.000000 prostate-nomograms-0.0.1/prostate_nomograms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 19:37:54.380890 prostate-nomograms-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      986 2023-06-02 19:33:16.000000 prostate-nomograms-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:46:06.430377 prostate-nomograms-0.0.2/
+-rw-rw-rw-   0        0        0    11549 2023-06-02 19:44:39.000000 prostate-nomograms-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3522 2023-06-02 19:46:06.429376 prostate-nomograms-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2912 2023-06-02 19:42:50.000000 prostate-nomograms-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 19:46:06.340841 prostate-nomograms-0.0.2/examples/
+-rw-rw-rw-   0        0        0        0 2023-05-09 17:06:15.000000 prostate-nomograms-0.0.2/examples/__init__.py
+-rw-rw-rw-   0        0        0      150 2023-05-09 17:06:15.000000 prostate-nomograms-0.0.2/examples/env_examples.py
+-rw-rw-rw-   0        0        0     3569 2023-06-02 19:21:40.000000 prostate-nomograms-0.0.2/examples/ex01-mskcc.py
+-rw-rw-rw-   0        0        0     3781 2023-06-02 19:21:40.000000 prostate-nomograms-0.0.2/examples/ex02-capra.py
+-rw-rw-rw-   0        0        0     3914 2023-06-02 19:21:40.000000 prostate-nomograms-0.0.2/examples/ex03-custom.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:46:06.345853 prostate-nomograms-0.0.2/prostate_nomograms/
+-rw-rw-rw-   0        0        0      465 2023-06-02 19:44:39.000000 prostate-nomograms-0.0.2/prostate_nomograms/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:46:06.365376 prostate-nomograms-0.0.2/prostate_nomograms/capra/
+-rw-rw-rw-   0        0        0       34 2023-06-02 19:10:35.000000 prostate-nomograms-0.0.2/prostate_nomograms/capra/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:46:06.378377 prostate-nomograms-0.0.2/prostate_nomograms/capra/base/
+-rw-rw-rw-   0        0        0      106 2023-05-31 14:34:11.000000 prostate-nomograms-0.0.2/prostate_nomograms/capra/base/__init__.py
+-rw-rw-rw-   0        0        0     1336 2023-06-01 15:55:16.000000 prostate-nomograms-0.0.2/prostate_nomograms/capra/base/logistic_regression.py
+-rw-rw-rw-   0        0        0     2273 2023-05-31 23:11:28.000000 prostate-nomograms-0.0.2/prostate_nomograms/capra/base/survival_regression.py
+-rw-rw-rw-   0        0        0    12574 2023-06-02 19:10:35.000000 prostate-nomograms-0.0.2/prostate_nomograms/capra/capra.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:46:06.387377 prostate-nomograms-0.0.2/prostate_nomograms/custom/
+-rw-rw-rw-   0        0        0       36 2023-05-31 19:54:31.000000 prostate-nomograms-0.0.2/prostate_nomograms/custom/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:46:06.397376 prostate-nomograms-0.0.2/prostate_nomograms/custom/base/
+-rw-rw-rw-   0        0        0      106 2023-05-31 14:34:11.000000 prostate-nomograms-0.0.2/prostate_nomograms/custom/base/__init__.py
+-rw-rw-rw-   0        0        0     1282 2023-06-01 15:55:16.000000 prostate-nomograms-0.0.2/prostate_nomograms/custom/base/logistic_regression.py
+-rw-rw-rw-   0        0        0     2192 2023-05-31 15:13:00.000000 prostate-nomograms-0.0.2/prostate_nomograms/custom/base/survival_regression.py
+-rw-rw-rw-   0        0        0     9078 2023-05-31 22:07:18.000000 prostate-nomograms-0.0.2/prostate_nomograms/custom/custom.py
+-rw-rw-rw-   0        0        0     1162 2023-06-02 19:10:35.000000 prostate-nomograms-0.0.2/prostate_nomograms/enum.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:46:06.405377 prostate-nomograms-0.0.2/prostate_nomograms/mskcc/
+-rw-rw-rw-   0        0        0       86 2023-06-02 19:10:35.000000 prostate-nomograms-0.0.2/prostate_nomograms/mskcc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:46:06.428377 prostate-nomograms-0.0.2/prostate_nomograms/mskcc/base/
+-rw-rw-rw-   0        0        0       26 2023-05-31 14:34:11.000000 prostate-nomograms-0.0.2/prostate_nomograms/mskcc/base/__init__.py
+-rw-rw-rw-   0        0        0     9792 2023-05-31 14:34:11.000000 prostate-nomograms-0.0.2/prostate_nomograms/mskcc/base/logistic_regression.py
+-rw-rw-rw-   0        0        0    10577 2023-05-31 22:05:59.000000 prostate-nomograms-0.0.2/prostate_nomograms/mskcc/base/model.py
+-rw-rw-rw-   0        0        0     2533 2023-05-31 14:34:11.000000 prostate-nomograms-0.0.2/prostate_nomograms/mskcc/base/survival_regression.py
+-rw-rw-rw-   0        0        0     5490 2023-05-31 14:34:11.000000 prostate-nomograms-0.0.2/prostate_nomograms/mskcc/base/web_table_scraper.py
+-rw-rw-rw-   0        0        0     2841 2023-06-02 19:10:35.000000 prostate-nomograms-0.0.2/prostate_nomograms/mskcc/pre_radical_prostatectomy_nomogram.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:46:06.356364 prostate-nomograms-0.0.2/prostate_nomograms.egg-info/
+-rw-rw-rw-   0        0        0     3522 2023-06-02 19:46:06.000000 prostate-nomograms-0.0.2/prostate_nomograms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1191 2023-06-02 19:46:06.000000 prostate-nomograms-0.0.2/prostate_nomograms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 19:46:06.000000 prostate-nomograms-0.0.2/prostate_nomograms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-06-02 19:46:06.000000 prostate-nomograms-0.0.2/prostate_nomograms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-06-02 19:46:06.000000 prostate-nomograms-0.0.2/prostate_nomograms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 19:46:06.430377 prostate-nomograms-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      986 2023-06-02 19:44:39.000000 prostate-nomograms-0.0.2/setup.py
```

### Comparing `prostate-nomograms-0.0.1/LICENSE` & `prostate-nomograms-0.0.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright [2023] [Maxence Larose]
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `prostate-nomograms-0.0.1/PKG-INFO` & `prostate-nomograms-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: prostate-nomograms
-Version: 0.0.1
-Summary: Prediction tools based on existing prostate cancer nomograms.
-Home-page: https://github.com/MaxenceLarose/prostate-nomograms
-Author: Maxence Larose
-Author-email: maxence.larose.1@ulaval.ca
-License: Apache License 2.0
-Keywords: cancer medical nomogram prediction prostate python3
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Prostate Nomograms
 
 A simple implementation of prostate cancer nomograms.
 
 > Prostate cancer nomograms are prediction tools designed to help patients and their physicians understand the nature of their prostate cancer, assess risk based on specific characteristics of a patient and his disease, and predict the likely outcomes of treatment. <sup>[1][1]</sup>
 
 ## Installation
@@ -51,15 +35,29 @@
 
 Note that a custom nomogram is also implemented, i.e. a simple logistic regression or cox regression using arbitrary variables. 
 
 ## Getting started
 
 You can find examples [here](https://github.com/MaxenceLarose/ProstateCancerNomograms/tree/main/examples).
 
-## Contact
+## License
 
-Maxence Larose, B. Ing., [maxence.larose.1@ulaval.ca](mailto:maxence.larose.1@ulaval.ca)
+This code is provided under the [Apache License 2.0](https://github.com/MaxenceLarose/delia/blob/main/LICENSE).
 
+## Citation
 
+```
+@misc{prostate-nomograms,
+  title={prostate-nomograms: Prediction tools based on existing prostate cancer nomograms},
+  author={Maxence Larose},
+  year={2022},
+  publisher={Université Laval},
+  url={https://github.com/MaxenceLarose/prostate-nomograms},
+}
+```
+
+## Contact
+
+Maxence Larose, B. Ing., [maxence.larose.1@ulaval.ca](mailto:maxence.larose.1@ulaval.ca)
 
 [comment]: REFERENCES>
 [1]: <https://www.mskcc.org/nomograms/prostate> "MSKCC - Prostate Cancer Nomograms"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `prostate-nomograms-0.0.1/README.md` & `prostate-nomograms-0.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: prostate-nomograms
+Version: 0.0.2
+Summary: Prediction tools based on existing prostate cancer nomograms.
+Home-page: https://github.com/MaxenceLarose/prostate-nomograms
+Author: Maxence Larose
+Author-email: maxence.larose.1@ulaval.ca
+License: Apache License 2.0
+Keywords: cancer medical nomogram prediction prostate python3
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Prostate Nomograms
 
 A simple implementation of prostate cancer nomograms.
 
 > Prostate cancer nomograms are prediction tools designed to help patients and their physicians understand the nature of their prostate cancer, assess risk based on specific characteristics of a patient and his disease, and predict the likely outcomes of treatment. <sup>[1][1]</sup>
 
 ## Installation
@@ -35,15 +51,29 @@
 
 Note that a custom nomogram is also implemented, i.e. a simple logistic regression or cox regression using arbitrary variables. 
 
 ## Getting started
 
 You can find examples [here](https://github.com/MaxenceLarose/ProstateCancerNomograms/tree/main/examples).
 
-## Contact
+## License
 
-Maxence Larose, B. Ing., [maxence.larose.1@ulaval.ca](mailto:maxence.larose.1@ulaval.ca)
+This code is provided under the [Apache License 2.0](https://github.com/MaxenceLarose/delia/blob/main/LICENSE).
 
+## Citation
 
+```
+@misc{prostate-nomograms,
+  title={prostate-nomograms: Prediction tools based on existing prostate cancer nomograms},
+  author={Maxence Larose},
+  year={2022},
+  publisher={Université Laval},
+  url={https://github.com/MaxenceLarose/prostate-nomograms},
+}
+```
+
+## Contact
+
+Maxence Larose, B. Ing., [maxence.larose.1@ulaval.ca](mailto:maxence.larose.1@ulaval.ca)
 
 [comment]: REFERENCES>
 [1]: <https://www.mskcc.org/nomograms/prostate> "MSKCC - Prostate Cancer Nomograms"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `prostate-nomograms-0.0.1/examples/ex01-mskcc.py` & `prostate-nomograms-0.0.2/examples/ex01-mskcc.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.1/examples/ex02-capra.py` & `prostate-nomograms-0.0.2/examples/ex02-capra.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.1/examples/ex03-custom.py` & `prostate-nomograms-0.0.2/examples/ex03-custom.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.1/prostate_nomograms/capra/base/logistic_regression.py` & `prostate-nomograms-0.0.2/prostate_nomograms/capra/base/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.1/prostate_nomograms/capra/base/survival_regression.py` & `prostate-nomograms-0.0.2/prostate_nomograms/capra/base/survival_regression.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.1/prostate_nomograms/capra/capra.py` & `prostate-nomograms-0.0.2/prostate_nomograms/capra/capra.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.1/prostate_nomograms/custom/base/logistic_regression.py` & `prostate-nomograms-0.0.2/prostate_nomograms/custom/base/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.1/prostate_nomograms/custom/base/survival_regression.py` & `prostate-nomograms-0.0.2/prostate_nomograms/custom/base/survival_regression.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.1/prostate_nomograms/custom/custom.py` & `prostate-nomograms-0.0.2/prostate_nomograms/custom/custom.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.1/prostate_nomograms/enum.py` & `prostate-nomograms-0.0.2/prostate_nomograms/enum.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.1/prostate_nomograms/mskcc/base/logistic_regression.py` & `prostate-nomograms-0.0.2/prostate_nomograms/mskcc/base/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.1/prostate_nomograms/mskcc/base/model.py` & `prostate-nomograms-0.0.2/prostate_nomograms/mskcc/base/model.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.1/prostate_nomograms/mskcc/base/survival_regression.py` & `prostate-nomograms-0.0.2/prostate_nomograms/mskcc/base/survival_regression.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.1/prostate_nomograms/mskcc/base/web_table_scraper.py` & `prostate-nomograms-0.0.2/prostate_nomograms/mskcc/base/web_table_scraper.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.1/prostate_nomograms/mskcc/pre_radical_prostatectomy_nomogram.py` & `prostate-nomograms-0.0.2/prostate_nomograms/mskcc/pre_radical_prostatectomy_nomogram.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.1/prostate_nomograms.egg-info/PKG-INFO` & `prostate-nomograms-0.0.2/prostate_nomograms.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prostate-nomograms
-Version: 0.0.1
+Version: 0.0.2
 Summary: Prediction tools based on existing prostate cancer nomograms.
 Home-page: https://github.com/MaxenceLarose/prostate-nomograms
 Author: Maxence Larose
 Author-email: maxence.larose.1@ulaval.ca
 License: Apache License 2.0
 Keywords: cancer medical nomogram prediction prostate python3
 Classifier: Programming Language :: Python :: 3
@@ -51,15 +51,29 @@
 
 Note that a custom nomogram is also implemented, i.e. a simple logistic regression or cox regression using arbitrary variables. 
 
 ## Getting started
 
 You can find examples [here](https://github.com/MaxenceLarose/ProstateCancerNomograms/tree/main/examples).
 
-## Contact
+## License
 
-Maxence Larose, B. Ing., [maxence.larose.1@ulaval.ca](mailto:maxence.larose.1@ulaval.ca)
+This code is provided under the [Apache License 2.0](https://github.com/MaxenceLarose/delia/blob/main/LICENSE).
+
+## Citation
+
+```
+@misc{prostate-nomograms,
+  title={prostate-nomograms: Prediction tools based on existing prostate cancer nomograms},
+  author={Maxence Larose},
+  year={2022},
+  publisher={Université Laval},
+  url={https://github.com/MaxenceLarose/prostate-nomograms},
+}
+```
 
+## Contact
 
+Maxence Larose, B. Ing., [maxence.larose.1@ulaval.ca](mailto:maxence.larose.1@ulaval.ca)
 
 [comment]: REFERENCES>
 [1]: <https://www.mskcc.org/nomograms/prostate> "MSKCC - Prostate Cancer Nomograms"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `prostate-nomograms-0.0.1/prostate_nomograms.egg-info/SOURCES.txt` & `prostate-nomograms-0.0.2/prostate_nomograms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.1/setup.py` & `prostate-nomograms-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="prostate-nomograms",
-    version="0.0.1",
+    version="0.0.2",
     author="Maxence Larose",
     author_email="maxence.larose.1@ulaval.ca",
     description="Prediction tools based on existing prostate cancer nomograms.",
     long_description=open('README.md', "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/MaxenceLarose/prostate-nomograms",
     license="Apache License 2.0",
```

