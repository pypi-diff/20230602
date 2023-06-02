# Comparing `tmp/afscgap-1.0.1.tar.gz` & `tmp/afscgap-1.0.2.tar.gz`

## Comparing `afscgap-1.0.1.tar` & `afscgap-1.0.2.tar`

### file list

```diff
@@ -1,39 +1,41 @@
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 afscgap-1.0.1/.gitattributes
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 afscgap-1.0.1/CONDUCT.md
--rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 afscgap-1.0.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 afscgap-1.0.1/build_docs.sh
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 afscgap-1.0.1/gruntfile.js
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 afscgap-1.0.1/install_browser.sh
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 afscgap-1.0.1/mkdocs.yml
--rw-r--r--   0        0        0   178220 2020-02-02 00:00:00.000000 afscgap-1.0.1/package-lock.json
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 afscgap-1.0.1/package.json
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 afscgap-1.0.1/setup.cfg
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 afscgap-1.0.1/afscgap/README.md
--rw-r--r--   0        0        0    58901 2020-02-02 00:00:00.000000 afscgap-1.0.1/afscgap/__init__.py
--rw-r--r--   0        0        0    42895 2020-02-02 00:00:00.000000 afscgap-1.0.1/afscgap/client.py
--rw-r--r--   0        0        0     9440 2020-02-02 00:00:00.000000 afscgap-1.0.1/afscgap/convert.py
--rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 afscgap-1.0.1/afscgap/cursor.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 afscgap-1.0.1/afscgap/http_util.py
--rw-r--r--   0        0        0    37009 2020-02-02 00:00:00.000000 afscgap-1.0.1/afscgap/inference.py
--rw-r--r--   0        0        0    37762 2020-02-02 00:00:00.000000 afscgap-1.0.1/afscgap/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 afscgap-1.0.1/afscgap/py.typed
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 afscgap-1.0.1/afscgap/query_util.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 afscgap-1.0.1/afscgap/typesdef.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 afscgap-1.0.1/docs/building.md
--rw-r--r--   0        0        0     5761 2020-02-02 00:00:00.000000 afscgap-1.0.1/docs/inference.md
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 afscgap-1.0.1/docs/limitations.md
--rw-r--r--   0        0        0    12988 2020-02-02 00:00:00.000000 afscgap-1.0.1/docs/model.md
--rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 afscgap-1.0.1/docs/objectives.md
--rw-r--r--   0        0        0    10255 2020-02-02 00:00:00.000000 afscgap-1.0.1/docs/usage.md
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 afscgap-1.0.1/paper/README.md
--rw-r--r--   0        0        0    13278 2020-02-02 00:00:00.000000 afscgap-1.0.1/paper/architecture.drawio
--rw-r--r--   0        0        0    87762 2020-02-02 00:00:00.000000 afscgap-1.0.1/paper/library.png
--rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 afscgap-1.0.1/paper/paper.bib
--rw-r--r--   0        0        0     7698 2020-02-02 00:00:00.000000 afscgap-1.0.1/paper/paper.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 afscgap-1.0.1/paper/preview_paper.sh
--rw-r--r--   0        0        0   173860 2020-02-02 00:00:00.000000 afscgap-1.0.1/paper/viz.png
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 afscgap-1.0.1/.gitignore
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 afscgap-1.0.1/LICENSE.md
--rw-r--r--   0        0        0    11252 2020-02-02 00:00:00.000000 afscgap-1.0.1/README.md
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 afscgap-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    12721 2020-02-02 00:00:00.000000 afscgap-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 afscgap-1.0.2/.gitattributes
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 afscgap-1.0.2/.zenodo.json
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 afscgap-1.0.2/CITATION.cff
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 afscgap-1.0.2/CONDUCT.md
+-rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 afscgap-1.0.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 afscgap-1.0.2/build_docs.sh
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 afscgap-1.0.2/gruntfile.js
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 afscgap-1.0.2/install_browser.sh
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 afscgap-1.0.2/mkdocs.yml
+-rw-r--r--   0        0        0   178220 2020-02-02 00:00:00.000000 afscgap-1.0.2/package-lock.json
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 afscgap-1.0.2/package.json
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 afscgap-1.0.2/setup.cfg
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 afscgap-1.0.2/afscgap/README.md
+-rw-r--r--   0        0        0    58901 2020-02-02 00:00:00.000000 afscgap-1.0.2/afscgap/__init__.py
+-rw-r--r--   0        0        0    42895 2020-02-02 00:00:00.000000 afscgap-1.0.2/afscgap/client.py
+-rw-r--r--   0        0        0     9440 2020-02-02 00:00:00.000000 afscgap-1.0.2/afscgap/convert.py
+-rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 afscgap-1.0.2/afscgap/cursor.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 afscgap-1.0.2/afscgap/http_util.py
+-rw-r--r--   0        0        0    37009 2020-02-02 00:00:00.000000 afscgap-1.0.2/afscgap/inference.py
+-rw-r--r--   0        0        0    37762 2020-02-02 00:00:00.000000 afscgap-1.0.2/afscgap/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 afscgap-1.0.2/afscgap/py.typed
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 afscgap-1.0.2/afscgap/query_util.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 afscgap-1.0.2/afscgap/typesdef.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 afscgap-1.0.2/docs/building.md
+-rw-r--r--   0        0        0     5761 2020-02-02 00:00:00.000000 afscgap-1.0.2/docs/inference.md
+-rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 afscgap-1.0.2/docs/limitations.md
+-rw-r--r--   0        0        0    12988 2020-02-02 00:00:00.000000 afscgap-1.0.2/docs/model.md
+-rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 afscgap-1.0.2/docs/objectives.md
+-rw-r--r--   0        0        0    10255 2020-02-02 00:00:00.000000 afscgap-1.0.2/docs/usage.md
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 afscgap-1.0.2/paper/README.md
+-rw-r--r--   0        0        0    13278 2020-02-02 00:00:00.000000 afscgap-1.0.2/paper/architecture.drawio
+-rw-r--r--   0        0        0    87762 2020-02-02 00:00:00.000000 afscgap-1.0.2/paper/library.png
+-rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 afscgap-1.0.2/paper/paper.bib
+-rw-r--r--   0        0        0     7649 2020-02-02 00:00:00.000000 afscgap-1.0.2/paper/paper.md
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 afscgap-1.0.2/paper/preview_paper.sh
+-rw-r--r--   0        0        0   173860 2020-02-02 00:00:00.000000 afscgap-1.0.2/paper/viz.png
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 afscgap-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 afscgap-1.0.2/LICENSE.md
+-rw-r--r--   0        0        0    11415 2020-02-02 00:00:00.000000 afscgap-1.0.2/README.md
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 afscgap-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    12884 2020-02-02 00:00:00.000000 afscgap-1.0.2/PKG-INFO
```

### Comparing `afscgap-1.0.1/CONDUCT.md` & `afscgap-1.0.2/CONDUCT.md`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.1/CONTRIBUTING.md` & `afscgap-1.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.1/gruntfile.js` & `afscgap-1.0.2/gruntfile.js`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.1/package-lock.json` & `afscgap-1.0.2/package-lock.json`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.1/afscgap/__init__.py` & `afscgap-1.0.2/afscgap/__init__.py`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.1/afscgap/client.py` & `afscgap-1.0.2/afscgap/client.py`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.1/afscgap/convert.py` & `afscgap-1.0.2/afscgap/convert.py`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.1/afscgap/cursor.py` & `afscgap-1.0.2/afscgap/cursor.py`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.1/afscgap/http_util.py` & `afscgap-1.0.2/afscgap/http_util.py`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.1/afscgap/inference.py` & `afscgap-1.0.2/afscgap/inference.py`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.1/afscgap/model.py` & `afscgap-1.0.2/afscgap/model.py`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.1/afscgap/query_util.py` & `afscgap-1.0.2/afscgap/query_util.py`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.1/afscgap/typesdef.py` & `afscgap-1.0.2/afscgap/typesdef.py`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.1/docs/building.md` & `afscgap-1.0.2/docs/building.md`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.1/docs/inference.md` & `afscgap-1.0.2/docs/inference.md`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.1/docs/limitations.md` & `afscgap-1.0.2/docs/limitations.md`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.1/docs/model.md` & `afscgap-1.0.2/docs/model.md`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.1/docs/objectives.md` & `afscgap-1.0.2/docs/objectives.md`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.1/docs/usage.md` & `afscgap-1.0.2/docs/usage.md`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.1/paper/README.md` & `afscgap-1.0.2/paper/README.md`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.1/paper/architecture.drawio` & `afscgap-1.0.2/paper/architecture.drawio`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.1/paper/library.png` & `afscgap-1.0.2/paper/library.png`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.1/paper/paper.bib` & `afscgap-1.0.2/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.1/paper/paper.md` & `afscgap-1.0.2/paper/paper.md`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
       institute:
         - ucberkeley
 affiliations:
  - name: University of California, Berkeley
    index: 1
 institute:
   - ucberkeley: University of California, Berkeley
-date: 4 April 2023
+date: 2 June 2023
 bibliography: paper.bib
 ---
 
 # Summary
 The Groundfish Assessment Program within NOAA's Alaska Fisheries Science Center produces longitudinal catch data for the region [@afscgap]. Supporting ocean health research and fisheries management, these "hauls" report where marine species are found during bottom trawl surveys and in what quantities [@example]. Increasing data usability for communities of diverse programming experience, Pyafscgap.org offers not just friendlier REST API operation for this economically and scientifically important dataset but query language compliation, memory-efficient algorithms for "zero-catch" inference, and interactive visual analytics. Altogether, this research toolset supports investigatory tasks not easily executable using the API service alone and broadens access through game and information design.
 
 # Statement of need
@@ -52,55 +52,55 @@
 The API struggles supporting some investigations as it provides "presence-only" data [@inport]. For example, the API may readily yield total mass of Pacific cod but not its geohash-aggregated catch per unit effort [@geohash].
 
 $$CPUE_{species} = \frac{m_{species}}{A_{swept}}$$
 
 Knowing CPUE (kg/ha) must also include "absence data" or hauls in which the speices was not recorded, this package can efficiently infer those hauls not easily returned from the API service [@notebook].
 
 ## Broad accessibility
-Though the `afscgap` Python package makes GAP catch data more accessible, the size and complexity of this dataset complicates comparative analysis between species, years, and/or geographic areas [@notebook]. Without deep developer experience, it may still be difficult to get started even with scientific background. To address a broader audience, this project also offers a no-code visualization tool sitting on top of `afscgap` with CSV and Python code export as a bridge to further analysis.
+Though the `afscgap` Python package makes GAP catch data more accessible, the size and complexity of this dataset complicates comparative analysis between species, years, and/or geographic areas [@notebook]. Without deep developer experience, it may still be difficult to get started even with scientific background. To address a broader audience, this project offers visualization on top of `afscgap` with CSV and Python code export as a bridge to further analysis.
 
 # Functions
-This project aims to improve accessibility of GAP catch data and offer approachable tools to kickstart analysis.
+This project improves accessibility of GAP catch data and offers approachable tools to kickstart analysis.
 
 ## Lazy querying facade
 The `afscgap` library manages significant complexity to offer a simple familiar interface to Python developers:
 
  - Lazy "generator iterables" increase accessibility by encapsulating logic for memory-efficient pagination and "data munging" behind Python-standard iterators [@lazy].
  - To support zero catch data, decorators adapt diverse structures to common interfaces, offering polymorphism [@decorators].
  - Offering a single object entry-point into the library, a "facade" frees users from needing deep understanding of the library's types, a goal furthered by compilation of "standard" Python types to Oracle REST Data Service queries [@facade].
 
 ![Diagram of afscgap.\label{fig:library}](library.png)
 
 ## Zero catch inference
 "Zero catch" inference enables a broader range of analysis with the following algorithm:
 
- - Paginate while records remain available from the API service.
+ - Lazily paginate while records remain available from the API service.
    - Record species and hauls observed from API-returned results.
    - Return records as available.
- - Generate inferred records after API exhaustion.
+ - Lazily generate inferred records after API exhaustion.
    - For each species observed in API results, check if it had a record for each haul in a hauls flat file [@flatfile].
    - For any hauls without the species, produce a record from the iterator.
 
-This library offers Python-emulation of ORDS filters for inferred records.
+Note `afscgap` performs Python-emulation of ORDS filters on inferred records.
 
 ## Visualization
 This complex dataset requires technical sophistication to navigate and, to further increase accessibility, visualization tools help start temporal, spatial, and species comparisons with deep linking, coordinated highlighting, separated color channels, summary statistics, and side-by-side display [@few].
 
 ![Visualization screenshot.\label{fig:viz}](viz.png)
 
-To support learning this UI, an optional introduction sequence tutorializes a "real" analysis via Hayashida^[Uses Mark Brown's formalization [@brown].] level design [@hayashida; @brown]:
+To support learning this UI, an optional introduction sequence tutorializes a "real" analysis via Hayashida level design [@hayashida; @brown]:
 
  - **Introduction**: The tool shows information about Pacific cod with pre-filled controls used to achieve that analysis gradually fading in, asking the user for minor modifications.
  - **Development**: Using the mechanics introduced moments prior, the tool invites the user to change the analysis to compare different regions.
  - **Twist**: Enabling overlays on the same display, the user leverages mechanics they just exercised in a now more complex interface.
  - **Conclusion**: The visualization invites the user to demonstrate skills acquired in a new problem.
 
 Note that this visualization also serves as a starting point for continued analysis by generating either CSV or Python code to take work into other tools.
 
-In addition to graduate classroom use, five individuals with relevant background offered feedback on this open source visualization. Though typically aided by a think-aloud prompt to help structure conversation, feedback was limited to needs assessment / quality improvement specific to this public web service^[IRB questionnaire indicates "project does not constitute human subjects research" and review is not required.] [@thinkaloud].
+In addition to use in a graduate classroom setting, five individuals with relevant background offered feedback on this open source visualization with four aided by a think-aloud prompt^[Discussion limited to tool-specific needs assessment / quality improvement, collecting information about the tool and not individuals. IRB questionnaire on file finds "project does not constitute human subjects research" and review is not required.] [@thinkaloud].
 
 ## Limitations
 As further documented in the repository [@readme], these tools:
 
  - Run single-threaded and synchoronous.
  - Represents hauls as points not areas in visualization aggregation due to dataset limitation.
  - Must exclude any hauls also excluded by NOAA from their dataset.
```

### Comparing `afscgap-1.0.1/paper/preview_paper.sh` & `afscgap-1.0.2/paper/preview_paper.sh`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.1/paper/viz.png` & `afscgap-1.0.2/paper/viz.png`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.1/LICENSE.md` & `afscgap-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.1/README.md` & `afscgap-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Python Tools for AFSC GAP
 | Group | Badges |
 |-------|--------|
 | Status | ![build workflow status](https://github.com/SchmidtDSE/afscgap/actions/workflows/build.yml/badge.svg?branch=main) ![docs workflow status](https://github.com/SchmidtDSE/afscgap/actions/workflows/docs.yml/badge.svg?branch=main) [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active) |
-| Usage | [![Python 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-370/) [![Pypi Badge](https://img.shields.io/pypi/v/afscgap)](https://pypi.org/project/afscgap/) [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause) |
-| Publication | [![pyOpenSci](https://tinyurl.com/y22nb8up)](https://github.com/pyOpenSci/software-submission/issues/93) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/SchmidtDSE/afscgap/main?urlpath=/tree/index.ipynb) [![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://codeocean.com/capsule/4905407/tree/v2) |
+| Usage | [![Python 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-370/) [![Pypi Badge](https://img.shields.io/pypi/v/afscgap)](https://pypi.org/project/afscgap/) [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/SchmidtDSE/afscgap/main?urlpath=/tree/index.ipynb) |
+| Publication | [![pyOpenSci](https://tinyurl.com/y22nb8up)](https://github.com/pyOpenSci/software-submission/issues/93) [![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://codeocean.com/capsule/4905407/tree/v2) [![DOI](https://zenodo.org/badge/603308264.svg)](https://zenodo.org/badge/latestdoi/603308264) |
 
 <br>
 
 Python-based tool chain ("Pyafscgap.org") for working with the public bottom trawl surveys data from the [NOAA AFSC GAP](https://www.fisheries.noaa.gov/contact/groundfish-assessment-program). This provides information about where certain species were seen and when under what conditions, information useful for research in ocean health.
 
 See [webpage](https://pyafscgap.org), [project Github](https://github.com/SchmidtDSE/afscgap), and [example notebook](https://mybinder.org/v2/gh/SchmidtDSE/afscgap/main?urlpath=/tree/index.ipynb).
 
@@ -113,15 +113,15 @@
 <br>
 <br>
 
 ## People
 [Sam Pottinger](https://github.com/sampottinger) is the primary contact with additional development from [Giulia Zarpellon](https://github.com/gizarp). Additionally some acknowledgements:
 
  - Thank you to [Carl Boettiger](https://github.com/cboettig) and [Fernando Perez](https://github.com/fperez) for advice in the Python library.
- - Thanks also to [Maya Weltman-Fahs](https://dse.berkeley.edu/people/maya-weltman-fahs), [Brookie Guzder-Williams](https://github.com/brookisme), Angela Hayes, and [Magali de Bruyn](https://github.com/magalidebruyn) for advice on the visual analytics tool.
+ - Thanks also to [Maya Weltman-Fahs](https://dse.berkeley.edu/people/maya-weltman-fahs), [Brookie Guzder-Williams](https://github.com/brookisme), Angela Hayes, David Joy, and [Magali de Bruyn](https://github.com/magalidebruyn) for advice on the visual analytics tool.
  - Lewis Barnett, Emily Markowitz, and Ciera Martinez for general guidance.
 
 This is a project of the [The Eric and Wendy Schmidt Center for Data Science and the Environment
 at UC Berkeley](https://dse.berkeley.edu) where [Kevin Koy](https://github.com/kevkoy) is Executive Director. Please contact us via dse@berkeley.edu.
 
 <br>
 <br>
@@ -153,14 +153,15 @@
 
 <br>
 <br>
 
 ## Version history
 Annotated version history:
 
+ - `1.0.2`: Minor documentation touch ups for pyopensci.
  - `1.0.1`: Minor documentation fix.
  - `1.0.0`: Release with pyopensci.
  - `0.0.9`: Fix with issue for certain import modalities and the `http` module.
  - `0.0.8`: New query syntax (builder / chaining) and units conversions.
  - `0.0.7`: Visual analytics tools.
  - `0.0.6`: Performance and size improvements.
  - `0.0.5`: Changes to documentation.
```

### Comparing `afscgap-1.0.1/pyproject.toml` & `afscgap-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "afscgap"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="A Samuel Pottinger", email="sam.pottinger@berkeley.edu" },
 ]
 description = "Tools for interacting with the public bottom trawl surveys data from the NOAA AFSC GAP."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `afscgap-1.0.1/PKG-INFO` & `afscgap-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afscgap
-Version: 1.0.1
+Version: 1.0.2
 Summary: Tools for interacting with the public bottom trawl surveys data from the NOAA AFSC GAP.
 Project-URL: Homepage, https://pyafscgap.org
 Project-URL: Documentation, https://pyafscgap.org/devdocs/afscgap.html
 Project-URL: Source, https://github.com/SchmidtDSE/afscgap
 Project-URL: Issue Tracker, https://github.com/SchmidtDSE/afscgap/issues
 Project-URL: Changelog, https://github.com/SchmidtDSE/afscgap#version-history
 Author-email: A Samuel Pottinger <sam.pottinger@berkeley.edu>
@@ -32,16 +32,16 @@
 Requires-Dist: types-requests; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # Python Tools for AFSC GAP
 | Group | Badges |
 |-------|--------|
 | Status | ![build workflow status](https://github.com/SchmidtDSE/afscgap/actions/workflows/build.yml/badge.svg?branch=main) ![docs workflow status](https://github.com/SchmidtDSE/afscgap/actions/workflows/docs.yml/badge.svg?branch=main) [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active) |
-| Usage | [![Python 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-370/) [![Pypi Badge](https://img.shields.io/pypi/v/afscgap)](https://pypi.org/project/afscgap/) [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause) |
-| Publication | [![pyOpenSci](https://tinyurl.com/y22nb8up)](https://github.com/pyOpenSci/software-submission/issues/93) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/SchmidtDSE/afscgap/main?urlpath=/tree/index.ipynb) [![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://codeocean.com/capsule/4905407/tree/v2) |
+| Usage | [![Python 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-370/) [![Pypi Badge](https://img.shields.io/pypi/v/afscgap)](https://pypi.org/project/afscgap/) [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/SchmidtDSE/afscgap/main?urlpath=/tree/index.ipynb) |
+| Publication | [![pyOpenSci](https://tinyurl.com/y22nb8up)](https://github.com/pyOpenSci/software-submission/issues/93) [![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://codeocean.com/capsule/4905407/tree/v2) [![DOI](https://zenodo.org/badge/603308264.svg)](https://zenodo.org/badge/latestdoi/603308264) |
 
 <br>
 
 Python-based tool chain ("Pyafscgap.org") for working with the public bottom trawl surveys data from the [NOAA AFSC GAP](https://www.fisheries.noaa.gov/contact/groundfish-assessment-program). This provides information about where certain species were seen and when under what conditions, information useful for research in ocean health.
 
 See [webpage](https://pyafscgap.org), [project Github](https://github.com/SchmidtDSE/afscgap), and [example notebook](https://mybinder.org/v2/gh/SchmidtDSE/afscgap/main?urlpath=/tree/index.ipynb).
 
@@ -147,15 +147,15 @@
 <br>
 <br>
 
 ## People
 [Sam Pottinger](https://github.com/sampottinger) is the primary contact with additional development from [Giulia Zarpellon](https://github.com/gizarp). Additionally some acknowledgements:
 
  - Thank you to [Carl Boettiger](https://github.com/cboettig) and [Fernando Perez](https://github.com/fperez) for advice in the Python library.
- - Thanks also to [Maya Weltman-Fahs](https://dse.berkeley.edu/people/maya-weltman-fahs), [Brookie Guzder-Williams](https://github.com/brookisme), Angela Hayes, and [Magali de Bruyn](https://github.com/magalidebruyn) for advice on the visual analytics tool.
+ - Thanks also to [Maya Weltman-Fahs](https://dse.berkeley.edu/people/maya-weltman-fahs), [Brookie Guzder-Williams](https://github.com/brookisme), Angela Hayes, David Joy, and [Magali de Bruyn](https://github.com/magalidebruyn) for advice on the visual analytics tool.
  - Lewis Barnett, Emily Markowitz, and Ciera Martinez for general guidance.
 
 This is a project of the [The Eric and Wendy Schmidt Center for Data Science and the Environment
 at UC Berkeley](https://dse.berkeley.edu) where [Kevin Koy](https://github.com/kevkoy) is Executive Director. Please contact us via dse@berkeley.edu.
 
 <br>
 <br>
@@ -187,14 +187,15 @@
 
 <br>
 <br>
 
 ## Version history
 Annotated version history:
 
+ - `1.0.2`: Minor documentation touch ups for pyopensci.
  - `1.0.1`: Minor documentation fix.
  - `1.0.0`: Release with pyopensci.
  - `0.0.9`: Fix with issue for certain import modalities and the `http` module.
  - `0.0.8`: New query syntax (builder / chaining) and units conversions.
  - `0.0.7`: Visual analytics tools.
  - `0.0.6`: Performance and size improvements.
  - `0.0.5`: Changes to documentation.
```

