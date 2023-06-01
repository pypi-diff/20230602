# Comparing `tmp/afscgap-1.0.0.tar.gz` & `tmp/afscgap-1.0.1.tar.gz`

## Comparing `afscgap-1.0.0.tar` & `afscgap-1.0.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 afscgap-1.0.0/.gitattributes
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 afscgap-1.0.0/CONDUCT.md
--rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 afscgap-1.0.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 afscgap-1.0.0/build_docs.sh
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 afscgap-1.0.0/gruntfile.js
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 afscgap-1.0.0/install_browser.sh
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 afscgap-1.0.0/mkdocs.yml
--rw-r--r--   0        0        0   178220 2020-02-02 00:00:00.000000 afscgap-1.0.0/package-lock.json
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 afscgap-1.0.0/package.json
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 afscgap-1.0.0/setup.cfg
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 afscgap-1.0.0/afscgap/README.md
--rw-r--r--   0        0        0    58901 2020-02-02 00:00:00.000000 afscgap-1.0.0/afscgap/__init__.py
--rw-r--r--   0        0        0    42895 2020-02-02 00:00:00.000000 afscgap-1.0.0/afscgap/client.py
--rw-r--r--   0        0        0     9440 2020-02-02 00:00:00.000000 afscgap-1.0.0/afscgap/convert.py
--rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 afscgap-1.0.0/afscgap/cursor.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 afscgap-1.0.0/afscgap/http_util.py
--rw-r--r--   0        0        0    37009 2020-02-02 00:00:00.000000 afscgap-1.0.0/afscgap/inference.py
--rw-r--r--   0        0        0    37762 2020-02-02 00:00:00.000000 afscgap-1.0.0/afscgap/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 afscgap-1.0.0/afscgap/py.typed
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 afscgap-1.0.0/afscgap/query_util.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 afscgap-1.0.0/afscgap/typesdef.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 afscgap-1.0.0/docs/building.md
--rw-r--r--   0        0        0     5761 2020-02-02 00:00:00.000000 afscgap-1.0.0/docs/inference.md
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 afscgap-1.0.0/docs/limitations.md
--rw-r--r--   0        0        0    12988 2020-02-02 00:00:00.000000 afscgap-1.0.0/docs/model.md
--rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 afscgap-1.0.0/docs/objectives.md
--rw-r--r--   0        0        0    10255 2020-02-02 00:00:00.000000 afscgap-1.0.0/docs/usage.md
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 afscgap-1.0.0/inst/README.md
--rw-r--r--   0        0        0    13278 2020-02-02 00:00:00.000000 afscgap-1.0.0/inst/architecture.drawio
--rw-r--r--   0        0        0    87762 2020-02-02 00:00:00.000000 afscgap-1.0.0/inst/library.png
--rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 afscgap-1.0.0/inst/paper.bib
--rw-r--r--   0        0        0     7572 2020-02-02 00:00:00.000000 afscgap-1.0.0/inst/paper.md
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 afscgap-1.0.0/inst/preview_paper.sh
--rw-r--r--   0        0        0   173860 2020-02-02 00:00:00.000000 afscgap-1.0.0/inst/viz.png
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 afscgap-1.0.0/.gitignore
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 afscgap-1.0.0/LICENSE.md
--rw-r--r--   0        0        0    11171 2020-02-02 00:00:00.000000 afscgap-1.0.0/README.md
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 afscgap-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    12640 2020-02-02 00:00:00.000000 afscgap-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 afscgap-1.0.1/.gitattributes
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 afscgap-1.0.1/CONDUCT.md
+-rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 afscgap-1.0.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 afscgap-1.0.1/build_docs.sh
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 afscgap-1.0.1/gruntfile.js
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 afscgap-1.0.1/install_browser.sh
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 afscgap-1.0.1/mkdocs.yml
+-rw-r--r--   0        0        0   178220 2020-02-02 00:00:00.000000 afscgap-1.0.1/package-lock.json
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 afscgap-1.0.1/package.json
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 afscgap-1.0.1/setup.cfg
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 afscgap-1.0.1/afscgap/README.md
+-rw-r--r--   0        0        0    58901 2020-02-02 00:00:00.000000 afscgap-1.0.1/afscgap/__init__.py
+-rw-r--r--   0        0        0    42895 2020-02-02 00:00:00.000000 afscgap-1.0.1/afscgap/client.py
+-rw-r--r--   0        0        0     9440 2020-02-02 00:00:00.000000 afscgap-1.0.1/afscgap/convert.py
+-rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 afscgap-1.0.1/afscgap/cursor.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 afscgap-1.0.1/afscgap/http_util.py
+-rw-r--r--   0        0        0    37009 2020-02-02 00:00:00.000000 afscgap-1.0.1/afscgap/inference.py
+-rw-r--r--   0        0        0    37762 2020-02-02 00:00:00.000000 afscgap-1.0.1/afscgap/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 afscgap-1.0.1/afscgap/py.typed
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 afscgap-1.0.1/afscgap/query_util.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 afscgap-1.0.1/afscgap/typesdef.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 afscgap-1.0.1/docs/building.md
+-rw-r--r--   0        0        0     5761 2020-02-02 00:00:00.000000 afscgap-1.0.1/docs/inference.md
+-rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 afscgap-1.0.1/docs/limitations.md
+-rw-r--r--   0        0        0    12988 2020-02-02 00:00:00.000000 afscgap-1.0.1/docs/model.md
+-rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 afscgap-1.0.1/docs/objectives.md
+-rw-r--r--   0        0        0    10255 2020-02-02 00:00:00.000000 afscgap-1.0.1/docs/usage.md
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 afscgap-1.0.1/paper/README.md
+-rw-r--r--   0        0        0    13278 2020-02-02 00:00:00.000000 afscgap-1.0.1/paper/architecture.drawio
+-rw-r--r--   0        0        0    87762 2020-02-02 00:00:00.000000 afscgap-1.0.1/paper/library.png
+-rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 afscgap-1.0.1/paper/paper.bib
+-rw-r--r--   0        0        0     7698 2020-02-02 00:00:00.000000 afscgap-1.0.1/paper/paper.md
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 afscgap-1.0.1/paper/preview_paper.sh
+-rw-r--r--   0        0        0   173860 2020-02-02 00:00:00.000000 afscgap-1.0.1/paper/viz.png
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 afscgap-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 afscgap-1.0.1/LICENSE.md
+-rw-r--r--   0        0        0    11252 2020-02-02 00:00:00.000000 afscgap-1.0.1/README.md
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 afscgap-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    12721 2020-02-02 00:00:00.000000 afscgap-1.0.1/PKG-INFO
```

### Comparing `afscgap-1.0.0/CONDUCT.md` & `afscgap-1.0.1/CONDUCT.md`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.0/CONTRIBUTING.md` & `afscgap-1.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.0/gruntfile.js` & `afscgap-1.0.1/gruntfile.js`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.0/package-lock.json` & `afscgap-1.0.1/package-lock.json`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.0/afscgap/__init__.py` & `afscgap-1.0.1/afscgap/__init__.py`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.0/afscgap/client.py` & `afscgap-1.0.1/afscgap/client.py`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.0/afscgap/convert.py` & `afscgap-1.0.1/afscgap/convert.py`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.0/afscgap/cursor.py` & `afscgap-1.0.1/afscgap/cursor.py`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.0/afscgap/http_util.py` & `afscgap-1.0.1/afscgap/http_util.py`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.0/afscgap/inference.py` & `afscgap-1.0.1/afscgap/inference.py`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.0/afscgap/model.py` & `afscgap-1.0.1/afscgap/model.py`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.0/afscgap/query_util.py` & `afscgap-1.0.1/afscgap/query_util.py`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.0/afscgap/typesdef.py` & `afscgap-1.0.1/afscgap/typesdef.py`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.0/docs/building.md` & `afscgap-1.0.1/docs/building.md`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.0/docs/inference.md` & `afscgap-1.0.1/docs/inference.md`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.0/docs/limitations.md` & `afscgap-1.0.1/docs/limitations.md`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.0/docs/model.md` & `afscgap-1.0.1/docs/model.md`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.0/docs/objectives.md` & `afscgap-1.0.1/docs/objectives.md`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.0/docs/usage.md` & `afscgap-1.0.1/docs/usage.md`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.0/inst/README.md` & `afscgap-1.0.1/paper/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Inst
+Paper
 ================================================================================
-Resources for the JOSS paper submission for the Pyafscgap.org project. See paper preview at https://pyafscgap.org/static/paper.pdf. Note that the paper preview uses the following open source tools:
+Resources for the JOSS paper submission for the Pyafscgap.org project. See paper preview at https://pyafscgap.org/static/paper_preview.pdf or the JOSS formatted version in the build artifact. Note that the paper preview uses the following open source tools:
 
  - [pandoc/luafilters](https://github.com/pandoc/lua-filters) by pandoc Lua filters contributors under the [MIT License](https://github.com/pandoc/lua-filters/blob/master/LICENSE)
  - [pandoc](https://pandoc.org/) (via call to OS package through shell script) by John MacFarlane, Albert Krewinkel, Jesse Rosenthal, and other contributors under the [GPL License](https://github.com/jgm/pandoc#license).
 
 The paper preview can be built by running `bash preview_paper.sh`.
```

### Comparing `afscgap-1.0.0/inst/architecture.drawio` & `afscgap-1.0.1/paper/architecture.drawio`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.0/inst/library.png` & `afscgap-1.0.1/paper/library.png`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.0/inst/paper.bib` & `afscgap-1.0.1/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.0/inst/paper.md` & `afscgap-1.0.1/paper/paper.md`

 * *Files 2% similar despite different names*

```diff
@@ -79,39 +79,41 @@
  - Generate inferred records after API exhaustion.
    - For each species observed in API results, check if it had a record for each haul in a hauls flat file [@flatfile].
    - For any hauls without the species, produce a record from the iterator.
 
 This library offers Python-emulation of ORDS filters for inferred records.
 
 ## Visualization
-This complex dataset requires technical sophistication to navigate and, to further increase accessibility, visualization tools help start temporal, spatial, and species comparisons with deep linking, coordinated highlighting, separated color channels, summary statistics, and side-by-side display [@few]. To support learning this UI, an optional introduction sequence tutorializes a "real" analysis via Hayashida^[Uses Mark Brown's formalization [@brown].] level design [@hayashida; @brown]:
+This complex dataset requires technical sophistication to navigate and, to further increase accessibility, visualization tools help start temporal, spatial, and species comparisons with deep linking, coordinated highlighting, separated color channels, summary statistics, and side-by-side display [@few].
+
+![Visualization screenshot.\label{fig:viz}](viz.png)
+
+To support learning this UI, an optional introduction sequence tutorializes a "real" analysis via Hayashida^[Uses Mark Brown's formalization [@brown].] level design [@hayashida; @brown]:
 
  - **Introduction**: The tool shows information about Pacific cod with pre-filled controls used to achieve that analysis gradually fading in, asking the user for minor modifications.
  - **Development**: Using the mechanics introduced moments prior, the tool invites the user to change the analysis to compare different regions.
  - **Twist**: Enabling overlays on the same display, the user leverages mechanics they just exercised in a now more complex interface.
  - **Conclusion**: The visualization invites the user to demonstrate skills acquired in a new problem.
 
 Note that this visualization also serves as a starting point for continued analysis by generating either CSV or Python code to take work into other tools.
 
-![Visualization screenshot.\label{fig:viz}](viz.png)
-
-In addition to graduate classroom use, five individuals with relevant background offered detailed feedback on this open source visualization. Though sometimes aided by a think-aloud prompt, feedback was limited to needs assessment / quality improvement specific to this publicly accessible web service [@thinkaloud].
+In addition to graduate classroom use, five individuals with relevant background offered feedback on this open source visualization. Though typically aided by a think-aloud prompt to help structure conversation, feedback was limited to needs assessment / quality improvement specific to this public web service^[IRB questionnaire indicates "project does not constitute human subjects research" and review is not required.] [@thinkaloud].
 
 ## Limitations
 As further documented in the repository [@readme], these tools:
 
  - Run single-threaded and synchoronous.
  - Represents hauls as points not areas in visualization aggregation due to dataset limitation.
  - Must exclude any hauls also excluded by NOAA from their dataset.
 
 # Acknowledgements
 Thanks to:
 
  - Runtime dependencies: ColorBrewer, D3, Flask, Geolib, Requests, Toolz, and Papa Parse [@colorbrewer; @d3; @flask; @geolib; @requests; @toolz; @papa].
  - Library advice: Carl Boettiger, Fernando Perez, and PyOpenSci reviewers.
- - Visualization advice: Lewis Barnett, Magali de Bruyn, Brookie Guzder-Williams, Angela Hayes, David Joy, Emily Markowitz, and Maya Weltman-Fahs.
- - Ciera Martinez for general guidance.
+ - Visualization advice: Magali de Bruyn, Brookie Guzder-Williams, Angela Hayes, David Joy, and Maya Weltman-Fahs.
+ - Lewis Barnett, Emily Markowitz, and Ciera Martinez for general guidance.
  - Draw.io for diagrams [@diagrams].
 
 Project of The Eric and Wendy Schmidt Center for Data Science and the Environment at UC Berkeley.
 
 # References
```

### Comparing `afscgap-1.0.0/inst/preview_paper.sh` & `afscgap-1.0.1/paper/preview_paper.sh`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 [[ ! -f author-info-blocks.lua ]] && wget https://raw.githubusercontent.com/pandoc/lua-filters/master/author-info-blocks/author-info-blocks.lua
 [[ ! -f scholarly-metadata.lua ]] && wget https://raw.githubusercontent.com/pandoc/lua-filters/master/scholarly-metadata/scholarly-metadata.lua
 
 sudo apt-get update
 
 sudo apt-get install pandoc pandoc-citeproc texlive-extra-utils texlive-fonts-recommended texlive-latex-base texlive-latex-extra
 
-pandoc paper.md --bibliography=paper.bib --lua-filter=scholarly-metadata.lua --lua-filter=author-info-blocks.lua -o ../website/static/paper.pdf
+pandoc paper.md --bibliography=paper.bib --lua-filter=scholarly-metadata.lua --lua-filter=author-info-blocks.lua -o ../website/static/paper_preview.pdf
```

### Comparing `afscgap-1.0.0/inst/viz.png` & `afscgap-1.0.1/paper/viz.png`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.0/LICENSE.md` & `afscgap-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `afscgap-1.0.0/README.md` & `afscgap-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,16 @@
 <br>
 <br>
 
 ## People
 [Sam Pottinger](https://github.com/sampottinger) is the primary contact with additional development from [Giulia Zarpellon](https://github.com/gizarp). Additionally some acknowledgements:
 
  - Thank you to [Carl Boettiger](https://github.com/cboettig) and [Fernando Perez](https://github.com/fperez) for advice in the Python library.
- - Thanks also to [Maya Weltman-Fahs](https://dse.berkeley.edu/people/maya-weltman-fahs), [Brookie Guzder-Williams](https://github.com/brookisme), Angela Hayes, Lewis Barnett, Emily Markowitz, and [Magali de Bruyn](https://github.com/magalidebruyn) for advice on the visual analytics tool.
+ - Thanks also to [Maya Weltman-Fahs](https://dse.berkeley.edu/people/maya-weltman-fahs), [Brookie Guzder-Williams](https://github.com/brookisme), Angela Hayes, and [Magali de Bruyn](https://github.com/magalidebruyn) for advice on the visual analytics tool.
+ - Lewis Barnett, Emily Markowitz, and Ciera Martinez for general guidance.
 
 This is a project of the [The Eric and Wendy Schmidt Center for Data Science and the Environment
 at UC Berkeley](https://dse.berkeley.edu) where [Kevin Koy](https://github.com/kevkoy) is Executive Director. Please contact us via dse@berkeley.edu.
 
 <br>
 <br>
 
@@ -152,14 +153,15 @@
 
 <br>
 <br>
 
 ## Version history
 Annotated version history:
 
+ - `1.0.1`: Minor documentation fix.
  - `1.0.0`: Release with pyopensci.
  - `0.0.9`: Fix with issue for certain import modalities and the `http` module.
  - `0.0.8`: New query syntax (builder / chaining) and units conversions.
  - `0.0.7`: Visual analytics tools.
  - `0.0.6`: Performance and size improvements.
  - `0.0.5`: Changes to documentation.
  - `0.0.4`: Negative / zero catch inference.
```

### Comparing `afscgap-1.0.0/pyproject.toml` & `afscgap-1.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "afscgap"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="A Samuel Pottinger", email="sam.pottinger@berkeley.edu" },
 ]
 description = "Tools for interacting with the public bottom trawl surveys data from the NOAA AFSC GAP."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `afscgap-1.0.0/PKG-INFO` & `afscgap-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afscgap
-Version: 1.0.0
+Version: 1.0.1
 Summary: Tools for interacting with the public bottom trawl surveys data from the NOAA AFSC GAP.
 Project-URL: Homepage, https://pyafscgap.org
 Project-URL: Documentation, https://pyafscgap.org/devdocs/afscgap.html
 Project-URL: Source, https://github.com/SchmidtDSE/afscgap
 Project-URL: Issue Tracker, https://github.com/SchmidtDSE/afscgap/issues
 Project-URL: Changelog, https://github.com/SchmidtDSE/afscgap#version-history
 Author-email: A Samuel Pottinger <sam.pottinger@berkeley.edu>
@@ -147,15 +147,16 @@
 <br>
 <br>
 
 ## People
 [Sam Pottinger](https://github.com/sampottinger) is the primary contact with additional development from [Giulia Zarpellon](https://github.com/gizarp). Additionally some acknowledgements:
 
  - Thank you to [Carl Boettiger](https://github.com/cboettig) and [Fernando Perez](https://github.com/fperez) for advice in the Python library.
- - Thanks also to [Maya Weltman-Fahs](https://dse.berkeley.edu/people/maya-weltman-fahs), [Brookie Guzder-Williams](https://github.com/brookisme), Angela Hayes, Lewis Barnett, Emily Markowitz, and [Magali de Bruyn](https://github.com/magalidebruyn) for advice on the visual analytics tool.
+ - Thanks also to [Maya Weltman-Fahs](https://dse.berkeley.edu/people/maya-weltman-fahs), [Brookie Guzder-Williams](https://github.com/brookisme), Angela Hayes, and [Magali de Bruyn](https://github.com/magalidebruyn) for advice on the visual analytics tool.
+ - Lewis Barnett, Emily Markowitz, and Ciera Martinez for general guidance.
 
 This is a project of the [The Eric and Wendy Schmidt Center for Data Science and the Environment
 at UC Berkeley](https://dse.berkeley.edu) where [Kevin Koy](https://github.com/kevkoy) is Executive Director. Please contact us via dse@berkeley.edu.
 
 <br>
 <br>
 
@@ -186,14 +187,15 @@
 
 <br>
 <br>
 
 ## Version history
 Annotated version history:
 
+ - `1.0.1`: Minor documentation fix.
  - `1.0.0`: Release with pyopensci.
  - `0.0.9`: Fix with issue for certain import modalities and the `http` module.
  - `0.0.8`: New query syntax (builder / chaining) and units conversions.
  - `0.0.7`: Visual analytics tools.
  - `0.0.6`: Performance and size improvements.
  - `0.0.5`: Changes to documentation.
  - `0.0.4`: Negative / zero catch inference.
```

