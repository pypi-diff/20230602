# Comparing `tmp/pretext-1.5.4.dev20230601.tar.gz` & `tmp/pretext-1.5.4.dev20230602.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretext-1.5.4.dev20230601.tar", max compression
+gzip compressed data, was "pretext-1.5.4.dev20230602.tar", max compression
```

## Comparing `pretext-1.5.4.dev20230601.tar` & `pretext-1.5.4.dev20230602.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35148 2023-06-01 06:19:12.025256 pretext-1.5.4.dev20230601/LICENSE
--rw-r--r--   0        0        0     9664 2023-06-01 06:19:12.025256 pretext-1.5.4.dev20230601/README.md
--rw-r--r--   0        0        0     1901 2023-06-01 06:19:39.885615 pretext-1.5.4.dev20230601/pretext/__init__.py
--rw-r--r--   0        0        0       61 2023-06-01 06:19:12.025256 pretext-1.5.4.dev20230601/pretext/__main__.py
--rw-r--r--   0        0        0     8170 2023-06-01 06:19:12.025256 pretext-1.5.4.dev20230601/pretext/build.py
--rw-r--r--   0        0        0    22798 2023-06-01 06:19:12.025256 pretext-1.5.4.dev20230601/pretext/cli.py
--rw-r--r--   0        0        0     5694 2023-06-01 06:19:12.025256 pretext-1.5.4.dev20230601/pretext/codechat.py
--rw-r--r--   0        0        0     5692 2023-06-01 06:19:12.025256 pretext-1.5.4.dev20230601/pretext/config/xml_overlay.py
--rw-r--r--   0        0        0      350 2023-06-01 06:19:12.025256 pretext-1.5.4.dev20230601/pretext/core/__init__.py
--rw-r--r--   0        0        0   172432 2023-06-01 06:19:44.849680 pretext-1.5.4.dev20230601/pretext/core/pretext.py
--rw-r--r--   0        0        0     1465 2023-06-01 06:19:12.025256 pretext-1.5.4.dev20230601/pretext/core/resources.py
--rw-r--r--   0        0        0  1031737 2023-06-01 06:19:44.849680 pretext-1.5.4.dev20230601/pretext/core/resources.zip
--rw-r--r--   0        0        0    15723 2023-06-01 06:19:12.025256 pretext-1.5.4.dev20230601/pretext/generate.py
--rw-r--r--   0        0        0    24666 2023-06-01 06:19:12.025256 pretext-1.5.4.dev20230601/pretext/project.py
--rw-r--r--   0        0        0      516 2023-06-01 06:19:12.025256 pretext-1.5.4.dev20230601/pretext/templates/__init__.py
--rw-r--r--   0        0        0     1676 2023-06-01 06:19:44.917681 pretext-1.5.4.dev20230601/pretext/templates/resources/.gitignore
--rw-r--r--   0        0        0        0 2023-06-01 06:19:44.917681 pretext-1.5.4.dev20230601/pretext/templates/resources/__init__.py
--rw-r--r--   0        0        0   160064 2023-06-01 06:19:44.897680 pretext-1.5.4.dev20230601/pretext/templates/resources/article.zip
--rw-r--r--   0        0        0     7570 2023-06-01 06:19:44.889680 pretext-1.5.4.dev20230601/pretext/templates/resources/book.zip
--rw-r--r--   0        0        0   173263 2023-06-01 06:19:44.917681 pretext-1.5.4.dev20230601/pretext/templates/resources/demo.zip
--rw-r--r--   0        0        0     2059 2023-06-01 06:19:44.917681 pretext-1.5.4.dev20230601/pretext/templates/resources/devcontainer.json
--rw-r--r--   0        0        0     4611 2023-06-01 06:19:44.901680 pretext-1.5.4.dev20230601/pretext/templates/resources/hello.zip
--rw-r--r--   0        0        0     1710 2023-06-01 06:19:44.917681 pretext-1.5.4.dev20230601/pretext/templates/resources/project.ptx
--rw-r--r--   0        0        0      242 2023-06-01 06:19:44.917681 pretext-1.5.4.dev20230601/pretext/templates/resources/publication.ptx
--rw-r--r--   0        0        0     8346 2023-06-01 06:19:44.905680 pretext-1.5.4.dev20230601/pretext/templates/resources/slideshow.zip
--rw-r--r--   0        0        0    18416 2023-06-01 06:19:12.025256 pretext-1.5.4.dev20230601/pretext/utils.py
--rw-r--r--   0        0        0     1143 2023-06-01 06:19:39.885615 pretext-1.5.4.dev20230601/pyproject.toml
--rw-r--r--   0        0        0    10761 1970-01-01 00:00:00.000000 pretext-1.5.4.dev20230601/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-06-02 06:18:09.908278 pretext-1.5.4.dev20230602/LICENSE
+-rw-r--r--   0        0        0     9664 2023-06-02 06:18:09.908278 pretext-1.5.4.dev20230602/README.md
+-rw-r--r--   0        0        0     1901 2023-06-02 06:18:39.301020 pretext-1.5.4.dev20230602/pretext/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-02 06:18:09.912279 pretext-1.5.4.dev20230602/pretext/__main__.py
+-rw-r--r--   0        0        0     8170 2023-06-02 06:18:09.912279 pretext-1.5.4.dev20230602/pretext/build.py
+-rw-r--r--   0        0        0    22798 2023-06-02 06:18:09.912279 pretext-1.5.4.dev20230602/pretext/cli.py
+-rw-r--r--   0        0        0     5694 2023-06-02 06:18:09.912279 pretext-1.5.4.dev20230602/pretext/codechat.py
+-rw-r--r--   0        0        0     5692 2023-06-02 06:18:09.912279 pretext-1.5.4.dev20230602/pretext/config/xml_overlay.py
+-rw-r--r--   0        0        0      350 2023-06-02 06:18:09.912279 pretext-1.5.4.dev20230602/pretext/core/__init__.py
+-rw-r--r--   0        0        0   172432 2023-06-02 06:18:44.257129 pretext-1.5.4.dev20230602/pretext/core/pretext.py
+-rw-r--r--   0        0        0     1465 2023-06-02 06:18:09.912279 pretext-1.5.4.dev20230602/pretext/core/resources.py
+-rw-r--r--   0        0        0  1031758 2023-06-02 06:18:44.257129 pretext-1.5.4.dev20230602/pretext/core/resources.zip
+-rw-r--r--   0        0        0    15723 2023-06-02 06:18:09.912279 pretext-1.5.4.dev20230602/pretext/generate.py
+-rw-r--r--   0        0        0    24666 2023-06-02 06:18:09.912279 pretext-1.5.4.dev20230602/pretext/project.py
+-rw-r--r--   0        0        0      516 2023-06-02 06:18:09.912279 pretext-1.5.4.dev20230602/pretext/templates/__init__.py
+-rw-r--r--   0        0        0     1676 2023-06-02 06:18:44.325131 pretext-1.5.4.dev20230602/pretext/templates/resources/.gitignore
+-rw-r--r--   0        0        0        0 2023-06-02 06:18:44.325131 pretext-1.5.4.dev20230602/pretext/templates/resources/__init__.py
+-rw-r--r--   0        0        0   160064 2023-06-02 06:18:44.305130 pretext-1.5.4.dev20230602/pretext/templates/resources/article.zip
+-rw-r--r--   0        0        0     7570 2023-06-02 06:18:44.305130 pretext-1.5.4.dev20230602/pretext/templates/resources/book.zip
+-rw-r--r--   0        0        0   173263 2023-06-02 06:18:44.321131 pretext-1.5.4.dev20230602/pretext/templates/resources/demo.zip
+-rw-r--r--   0        0        0     2059 2023-06-02 06:18:44.325131 pretext-1.5.4.dev20230602/pretext/templates/resources/devcontainer.json
+-rw-r--r--   0        0        0     4611 2023-06-02 06:18:44.321131 pretext-1.5.4.dev20230602/pretext/templates/resources/hello.zip
+-rw-r--r--   0        0        0     1710 2023-06-02 06:18:44.325131 pretext-1.5.4.dev20230602/pretext/templates/resources/project.ptx
+-rw-r--r--   0        0        0      242 2023-06-02 06:18:44.325131 pretext-1.5.4.dev20230602/pretext/templates/resources/publication.ptx
+-rw-r--r--   0        0        0     8346 2023-06-02 06:18:44.325131 pretext-1.5.4.dev20230602/pretext/templates/resources/slideshow.zip
+-rw-r--r--   0        0        0    18416 2023-06-02 06:18:09.912279 pretext-1.5.4.dev20230602/pretext/utils.py
+-rw-r--r--   0        0        0     1143 2023-06-02 06:18:39.305020 pretext-1.5.4.dev20230602/pyproject.toml
+-rw-r--r--   0        0        0    10761 1970-01-01 00:00:00.000000 pretext-1.5.4.dev20230602/PKG-INFO
```

### Comparing `pretext-1.5.4.dev20230601/LICENSE` & `pretext-1.5.4.dev20230602/LICENSE`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230601/README.md` & `pretext-1.5.4.dev20230602/README.md`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230601/pretext/__init__.py` & `pretext-1.5.4.dev20230602/pretext/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from pathlib import Path
 from single_version import get_version
 
 VERSION = get_version("pretext", Path(__file__).parent.parent)
 
-CORE_COMMIT = 'f468291d468dabd48557cb465125c1bc6b94b54c'
+CORE_COMMIT = '3024ffd91203498bc9fba1c16681c9817ccce93a'
 
 # List of templates, build formats, and assets that are supported by the CLI.
 NEW_TEMPLATES = ["book", "article", "demo", "hello", "slideshow"]
 BUILD_FORMATS = [
     "html",
     "pdf",
     "latex",
```

### Comparing `pretext-1.5.4.dev20230601/pretext/build.py` & `pretext-1.5.4.dev20230602/pretext/build.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230601/pretext/cli.py` & `pretext-1.5.4.dev20230602/pretext/cli.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230601/pretext/codechat.py` & `pretext-1.5.4.dev20230602/pretext/codechat.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230601/pretext/config/xml_overlay.py` & `pretext-1.5.4.dev20230602/pretext/config/xml_overlay.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230601/pretext/core/pretext.py` & `pretext-1.5.4.dev20230602/pretext/core/pretext.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230601/pretext/core/resources.py` & `pretext-1.5.4.dev20230602/pretext/core/resources.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230601/pretext/core/resources.zip` & `pretext-1.5.4.dev20230602/pretext/core/resources.zip`

 * *Files 12% similar despite different names*

#### zipinfo {}

```diff
@@ -1,142 +1,142 @@
-Zip file size: 1031737 bytes, number of entries: 140
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 06:19 css/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 06:19 pretext/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 06:19 schema/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 06:19 script/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 06:19 xsl/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 06:19 script/mjsre/
--rw-r--r--  2.0 unx      258 b- defN 23-Jun-01 06:19 script/README.md
--rw-r--r--  2.0 unx     2666 b- defN 23-Jun-01 06:19 script/mbx
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 06:19 script/mjsre/update-sre
--rw-r--r--  2.0 unx      481 b- defN 23-Jun-01 06:19 script/mjsre/README.md
--rw-r--r--  2.0 unx      116 b- defN 23-Jun-01 06:19 script/mjsre/package.json
--rw-r--r--  2.0 unx     9251 b- defN 23-Jun-01 06:19 script/mjsre/mj-sre-page.js
--rw-r--r--  2.0 unx    18421 b- defN 23-Jun-01 06:19 schema/pretext-schematron.xsl
--rw-r--r--  2.0 unx    58086 b- defN 23-Jun-01 06:19 schema/pretext.rnc
--rw-r--r--  2.0 unx    25290 b- defN 23-Jun-01 06:19 schema/pretext-validation-plus.xsl
--rw-r--r--  2.0 unx   134043 b- defN 23-Jun-01 06:19 schema/pretext.xml
--rw-r--r--  2.0 unx     1180 b- defN 23-Jun-01 06:19 schema/README.md
--rw-r--r--  2.0 unx   125135 b- defN 23-Jun-01 06:19 schema/pretext.xsd
--rw-r--r--  2.0 unx      326 b- defN 23-Jun-01 06:19 schema/xml.xsd
--rw-r--r--  2.0 unx    34210 b- defN 23-Jun-01 06:19 schema/pretext-dev.rng
--rw-r--r--  2.0 unx   101829 b- defN 23-Jun-01 06:19 schema/pretext.rng
--rw-r--r--  2.0 unx    17587 b- defN 23-Jun-01 06:19 schema/pretext-dev.rnc
--rw-r--r--  2.0 unx     3135 b- defN 23-Jun-01 06:19 schema/build.sh
--rw-r--r--  2.0 unx     1367 b- defN 23-Jun-01 06:19 pretext/README.md
--rw-r--r--  2.0 unx   172432 b- defN 23-Jun-01 06:19 pretext/pretext.py
--rw-r--r--  2.0 unx     1955 b- defN 23-Jun-01 06:19 pretext/module-test.py
--rw-r--r--  2.0 unx    30908 b- defN 23-Jun-01 06:19 pretext/pretext
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 06:19 pretext/__init__.py
--rw-r--r--  2.0 unx    35449 b- defN 23-Jun-01 06:19 pretext/braille_format.py
--rw-r--r--  2.0 unx     2566 b- defN 23-Jun-01 06:19 pretext/pretext.cfg
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 06:19 xsl/latex/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 06:19 xsl/localizations/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 06:19 xsl/support/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 06:19 xsl/utilities/
--rw-r--r--  2.0 unx     9787 b- defN 23-Jun-01 06:19 xsl/entities.ent
--rw-r--r--  2.0 unx     3239 b- defN 23-Jun-01 06:19 xsl/extract-interactive.xsl
--rw-r--r--  2.0 unx    13037 b- defN 23-Jun-01 06:19 xsl/pretext-text.xsl
--rw-r--r--  2.0 unx     1768 b- defN 23-Jun-01 06:19 xsl/README.md
--rw-r--r--  2.0 unx   139486 b- defN 23-Jun-01 06:19 xsl/extract-pg.xsl
--rw-r--r--  2.0 unx     6066 b- defN 23-Jun-01 06:19 xsl/pretext-json-manifest.xsl
--rw-r--r--  2.0 unx    22121 b- defN 23-Jun-01 06:19 xsl/pretext-revealjs.xsl
--rw-r--r--  2.0 unx     2846 b- defN 23-Jun-01 06:19 xsl/extract-datafile.xsl
--rw-r--r--  2.0 unx     8130 b- defN 23-Jun-01 06:19 xsl/extract-identity.xsl
--rw-r--r--  2.0 unx     8125 b- defN 23-Jun-01 06:19 xsl/extract-sageplot.xsl
--rw-r--r--  2.0 unx   263063 b- defN 23-Jun-01 06:19 xsl/publisher-variables.xsl
--rw-r--r--  2.0 unx   103661 b- defN 23-Jun-01 06:19 xsl/pretext-runestone.xsl
--rw-r--r--  2.0 unx    11766 b- defN 23-Jun-01 06:19 xsl/pretext-sage-doctest.xsl
--rw-r--r--  2.0 unx    39918 b- defN 23-Jun-01 06:19 xsl/pretext-runestone-static.xsl
--rw-r--r--  2.0 unx    17293 b- defN 23-Jun-01 06:19 xsl/pretext-ww-problem-sets.xsl
--rw-r--r--  2.0 unx   543735 b- defN 23-Jun-01 06:19 xsl/pretext-latex.xsl
--rw-r--r--  2.0 unx     2601 b- defN 23-Jun-01 06:19 xsl/pretext-merge.xsl
--rw-r--r--  2.0 unx     4571 b- defN 23-Jun-01 06:19 xsl/pretext-litprog.xsl
--rw-r--r--  2.0 unx    19072 b- defN 23-Jun-01 06:19 xsl/extract-latex-image.xsl
--rw-r--r--  2.0 unx    67275 b- defN 23-Jun-01 06:19 xsl/pretext-epub.xsl
--rw-r--r--  2.0 unx     8535 b- defN 23-Jun-01 06:19 xsl/pretext-view-source.xsl
--rw-r--r--  2.0 unx     6281 b- defN 23-Jun-01 06:19 xsl/pretext-numbers.xsl
--rw-r--r--  2.0 unx   111553 b- defN 23-Jun-01 06:19 xsl/pretext-assembly.xsl
--rw-r--r--  2.0 unx     2248 b- defN 23-Jun-01 06:19 xsl/extract-mom.xsl
--rw-r--r--  2.0 unx    21086 b- defN 23-Jun-01 06:19 xsl/pretext-smc.xsl
--rw-r--r--  2.0 unx   546938 b- defN 23-Jun-01 06:19 xsl/pretext-common.xsl
--rw-r--r--  2.0 unx     2740 b- defN 23-Jun-01 06:19 xsl/extract-youtube.xsl
--rw-r--r--  2.0 unx    41730 b- defN 23-Jun-01 06:19 xsl/pretext-beamer.xsl
--rw-r--r--  2.0 unx    13186 b- defN 23-Jun-01 06:19 xsl/pretext-solution-manual-latex.xsl
--rw-r--r--  2.0 unx    89128 b- defN 23-Jun-01 06:19 xsl/pretext-braille-preprint.xsl
--rw-r--r--  2.0 unx    10708 b- defN 23-Jun-01 06:19 xsl/pretext-units.xsl
--rw-r--r--  2.0 unx     3560 b- defN 23-Jun-01 06:19 xsl/pretext-basic-html.xsl
--rw-r--r--  2.0 unx     2725 b- defN 23-Jun-01 06:19 xsl/extract-asymptote.xsl
--rw-r--r--  2.0 unx   605806 b- defN 23-Jun-01 06:19 xsl/pretext-html.xsl
--rw-r--r--  2.0 unx     2597 b- defN 23-Jun-01 06:19 xsl/extract-trace.xsl
--rw-r--r--  2.0 unx    43020 b- defN 23-Jun-01 06:19 xsl/pretext-text-utilities.xsl
--rw-r--r--  2.0 unx    40230 b- defN 23-Jun-01 06:19 xsl/pretext-jupyter.xsl
--rw-r--r--  2.0 unx     2709 b- defN 23-Jun-01 06:19 xsl/extract-qrcode.xsl
--rw-r--r--  2.0 unx     7526 b- defN 23-Jun-01 06:19 xsl/latex/pretext-latex-CLP.xsl
--rw-r--r--  2.0 unx     3024 b- defN 23-Jun-01 06:19 xsl/latex/pretext-latex-dyslexic-font.xsl
--rw-r--r--  2.0 unx     2261 b- defN 23-Jun-01 06:19 xsl/latex/pretext-latex-AIM.xsl
--rw-r--r--  2.0 unx    14482 b- defN 23-Jun-01 06:19 xsl/latex/pretext-latex-chaos.xsl
--rw-r--r--  2.0 unx     5135 b- defN 23-Jun-01 06:19 xsl/latex/pretext-latex-guide.xsl
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 06:19 xsl/support/play-button/
--rw-r--r--  2.0 unx      504 b- defN 23-Jun-01 06:19 xsl/support/README.md
--rw-r--r--  2.0 unx    10306 b- defN 23-Jun-01 06:19 xsl/support/extract-math.xsl
--rw-r--r--  2.0 unx     5241 b- defN 23-Jun-01 06:19 xsl/support/pretext-pg-macros.xsl
--rw-r--r--  2.0 unx     5879 b- defN 23-Jun-01 06:19 xsl/support/package-math.xsl
--rw-r--r--  2.0 unx      486 b- defN 23-Jun-01 06:19 xsl/support/runestone-services.xml
--rw-r--r--  2.0 unx     5800 b- defN 23-Jun-01 06:19 xsl/support/tactile-svg.xsl
--rw-r--r--  2.0 unx     5065 b- defN 23-Jun-01 06:19 xsl/support/extract-latex-image-labels.xsl
--rw-r--r--  2.0 unx     2657 b- defN 23-Jun-01 06:19 xsl/support/play-button/README.md
--rw-r--r--  2.0 unx      722 b- defN 23-Jun-01 06:19 xsl/support/play-button/play-button.svg
--rw-r--r--  2.0 unx     6621 b- defN 23-Jun-01 06:19 xsl/support/play-button/play-button.png
--rw-r--r--  2.0 unx    16518 b- defN 23-Jun-01 06:19 xsl/localizations/es-ES.xml
--rw-r--r--  2.0 unx    16069 b- defN 23-Jun-01 06:19 xsl/localizations/hu-HU.xml
--rw-r--r--  2.0 unx    17215 b- defN 23-Jun-01 06:19 xsl/localizations/de-DE.xml
--rw-r--r--  2.0 unx    16333 b- defN 23-Jun-01 06:19 xsl/localizations/fr-FR.xml
--rw-r--r--  2.0 unx    17285 b- defN 23-Jun-01 06:19 xsl/localizations/fi-FI.xml
--rw-r--r--  2.0 unx     4708 b- defN 23-Jun-01 06:19 xsl/localizations/README.md
--rw-r--r--  2.0 unx    15938 b- defN 23-Jun-01 06:19 xsl/localizations/it-IT.xml
--rw-r--r--  2.0 unx    16821 b- defN 23-Jun-01 06:19 xsl/localizations/af-ZA.xml
--rw-r--r--  2.0 unx    16236 b- defN 23-Jun-01 06:19 xsl/localizations/ca-ES.xml
--rw-r--r--  2.0 unx    19049 b- defN 23-Jun-01 06:19 xsl/localizations/en-US.xml
--rw-r--r--  2.0 unx    19169 b- defN 23-Jun-01 06:19 xsl/localizations/nl-NL.xml
--rw-r--r--  2.0 unx     2227 b- defN 23-Jun-01 06:19 xsl/localizations/localizations.xml
--rw-r--r--  2.0 unx    15566 b- defN 23-Jun-01 06:19 xsl/localizations/cs-CZ.xml
--rw-r--r--  2.0 unx    17040 b- defN 23-Jun-01 06:19 xsl/localizations/bg-BG.xml
--rw-r--r--  2.0 unx    17065 b- defN 23-Jun-01 06:19 xsl/localizations/pt-PT.xml
--rw-r--r--  2.0 unx    16484 b- defN 23-Jun-01 06:19 xsl/localizations/fr-CA.xml
--rw-r--r--  2.0 unx    16296 b- defN 23-Jun-01 06:19 xsl/localizations/pt-BR.xml
--rw-r--r--  2.0 unx     1810 b- defN 23-Jun-01 06:19 xsl/utilities/README.md
--rw-r--r--  2.0 unx    30257 b- defN 23-Jun-01 06:19 xsl/utilities/fix-deprecations.xsl
--rw-r--r--  2.0 unx     4926 b- defN 23-Jun-01 06:19 xsl/utilities/pretext-enhanced-source.xsl
--rw-r--r--  2.0 unx      513 b- defN 23-Jun-01 06:19 xsl/utilities/deprecate-autoname.sed
--rw-r--r--  2.0 unx     4299 b- defN 23-Jun-01 06:19 xsl/utilities/author-report.xsl
--rw-r--r--  2.0 unx      787 b- defN 23-Jun-01 06:19 xsl/utilities/deprecate-index.sed
--rw-r--r--  2.0 unx     1276 b- defN 23-Jun-01 06:19 css/colors_maroon_grey.css
--rw-r--r--  2.0 unx     7761 b- defN 23-Jun-01 06:19 css/style_default.css
--rw-r--r--  2.0 unx     3473 b- defN 23-Jun-01 06:19 css/style_soundwriting.css
--rw-r--r--  2.0 unx    63664 b- defN 23-Jun-01 06:19 css/mathbook-add-on.css
--rw-r--r--  2.0 unx     1865 b- defN 23-Jun-01 06:19 css/README.md
--rw-r--r--  2.0 unx     1280 b- defN 23-Jun-01 06:19 css/colors_brown_gold.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-01 06:19 css/colors_blue_red.css
--rw-r--r--  2.0 unx   435680 b- defN 23-Jun-01 06:19 css/mathbook-3.css
--rw-r--r--  2.0 unx   146685 b- defN 23-Jun-01 06:19 css/mathbook-content.css
--rw-r--r--  2.0 unx    22438 b- defN 23-Jun-01 06:19 css/pretext.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-01 06:19 css/colors_green_plum.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-01 06:19 css/colors_ruby_turquoise.css
--rw-r--r--  2.0 unx     4308 b- defN 23-Jun-01 06:19 css/colors_blue_green.css
--rw-r--r--  2.0 unx    71198 b- defN 23-Jun-01 06:19 css/pretext_add_on.css
--rw-r--r--  2.0 unx     2608 b- defN 23-Jun-01 06:19 css/colors_default.css
--rw-r--r--  2.0 unx     2438 b- defN 23-Jun-01 06:19 css/colors_blue_grey.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-01 06:19 css/colors_green_blue.css
--rw-r--r--  2.0 unx     2446 b- defN 23-Jun-01 06:19 css/colors_darkmartiansands.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-01 06:19 css/colors_orange_navy.css
--rw-r--r--  2.0 unx    12567 b- defN 23-Jun-01 06:19 css/style_oscarlevin.css
--rw-r--r--  2.0 unx      691 b- defN 23-Jun-01 06:19 css/colors_pastel_blue_orange.css
--rw-r--r--  2.0 unx     1338 b- defN 23-Jun-01 06:19 css/colors_red_blue.css
--rw-r--r--  2.0 unx    14069 b- defN 23-Jun-01 06:19 css/setcolors.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-01 06:19 css/colors_ruby_amethyst.css
--rw-r--r--  2.0 unx     2446 b- defN 23-Jun-01 06:19 css/colors_martiansands.css
--rw-r--r--  2.0 unx     1362 b- defN 23-Jun-01 06:19 css/epub.css
--rw-r--r--  2.0 unx     2441 b- defN 23-Jun-01 06:19 css/kindle.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-01 06:19 css/colors_ruby_emerald.css
--rw-r--r--  2.0 unx     4021 b- defN 23-Jun-01 06:19 css/update_css
-140 files, 4820277 bytes uncompressed, 1014409 bytes compressed:  79.0%
+Zip file size: 1031758 bytes, number of entries: 140
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 06:18 css/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 06:18 pretext/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 06:18 schema/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 06:18 script/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 06:18 xsl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 06:18 xsl/latex/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 06:18 xsl/localizations/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 06:18 xsl/support/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 06:18 xsl/utilities/
+-rw-r--r--  2.0 unx   263063 b- defN 23-Jun-02 06:18 xsl/publisher-variables.xsl
+-rw-r--r--  2.0 unx   605964 b- defN 23-Jun-02 06:18 xsl/pretext-html.xsl
+-rw-r--r--  2.0 unx     6066 b- defN 23-Jun-02 06:18 xsl/pretext-json-manifest.xsl
+-rw-r--r--  2.0 unx     4571 b- defN 23-Jun-02 06:18 xsl/pretext-litprog.xsl
+-rw-r--r--  2.0 unx     2725 b- defN 23-Jun-02 06:18 xsl/extract-asymptote.xsl
+-rw-r--r--  2.0 unx   139486 b- defN 23-Jun-02 06:18 xsl/extract-pg.xsl
+-rw-r--r--  2.0 unx     9787 b- defN 23-Jun-02 06:18 xsl/entities.ent
+-rw-r--r--  2.0 unx    13186 b- defN 23-Jun-02 06:18 xsl/pretext-solution-manual-latex.xsl
+-rw-r--r--  2.0 unx     6281 b- defN 23-Jun-02 06:18 xsl/pretext-numbers.xsl
+-rw-r--r--  2.0 unx     2597 b- defN 23-Jun-02 06:18 xsl/extract-trace.xsl
+-rw-r--r--  2.0 unx     8535 b- defN 23-Jun-02 06:18 xsl/pretext-view-source.xsl
+-rw-r--r--  2.0 unx    10708 b- defN 23-Jun-02 06:18 xsl/pretext-units.xsl
+-rw-r--r--  2.0 unx     3239 b- defN 23-Jun-02 06:18 xsl/extract-interactive.xsl
+-rw-r--r--  2.0 unx    40230 b- defN 23-Jun-02 06:18 xsl/pretext-jupyter.xsl
+-rw-r--r--  2.0 unx   111553 b- defN 23-Jun-02 06:18 xsl/pretext-assembly.xsl
+-rw-r--r--  2.0 unx    43020 b- defN 23-Jun-02 06:18 xsl/pretext-text-utilities.xsl
+-rw-r--r--  2.0 unx    39918 b- defN 23-Jun-02 06:18 xsl/pretext-runestone-static.xsl
+-rw-r--r--  2.0 unx    13037 b- defN 23-Jun-02 06:18 xsl/pretext-text.xsl
+-rw-r--r--  2.0 unx    89128 b- defN 23-Jun-02 06:18 xsl/pretext-braille-preprint.xsl
+-rw-r--r--  2.0 unx     2846 b- defN 23-Jun-02 06:18 xsl/extract-datafile.xsl
+-rw-r--r--  2.0 unx     2601 b- defN 23-Jun-02 06:18 xsl/pretext-merge.xsl
+-rw-r--r--  2.0 unx    17293 b- defN 23-Jun-02 06:18 xsl/pretext-ww-problem-sets.xsl
+-rw-r--r--  2.0 unx   546938 b- defN 23-Jun-02 06:18 xsl/pretext-common.xsl
+-rw-r--r--  2.0 unx    21086 b- defN 23-Jun-02 06:18 xsl/pretext-smc.xsl
+-rw-r--r--  2.0 unx     8125 b- defN 23-Jun-02 06:18 xsl/extract-sageplot.xsl
+-rw-r--r--  2.0 unx     8130 b- defN 23-Jun-02 06:18 xsl/extract-identity.xsl
+-rw-r--r--  2.0 unx    41730 b- defN 23-Jun-02 06:18 xsl/pretext-beamer.xsl
+-rw-r--r--  2.0 unx   103793 b- defN 23-Jun-02 06:18 xsl/pretext-runestone.xsl
+-rw-r--r--  2.0 unx     3560 b- defN 23-Jun-02 06:18 xsl/pretext-basic-html.xsl
+-rw-r--r--  2.0 unx     2709 b- defN 23-Jun-02 06:18 xsl/extract-qrcode.xsl
+-rw-r--r--  2.0 unx     2248 b- defN 23-Jun-02 06:18 xsl/extract-mom.xsl
+-rw-r--r--  2.0 unx     2740 b- defN 23-Jun-02 06:18 xsl/extract-youtube.xsl
+-rw-r--r--  2.0 unx     1768 b- defN 23-Jun-02 06:18 xsl/README.md
+-rw-r--r--  2.0 unx    67275 b- defN 23-Jun-02 06:18 xsl/pretext-epub.xsl
+-rw-r--r--  2.0 unx    11766 b- defN 23-Jun-02 06:18 xsl/pretext-sage-doctest.xsl
+-rw-r--r--  2.0 unx    22121 b- defN 23-Jun-02 06:18 xsl/pretext-revealjs.xsl
+-rw-r--r--  2.0 unx   543735 b- defN 23-Jun-02 06:18 xsl/pretext-latex.xsl
+-rw-r--r--  2.0 unx    19072 b- defN 23-Jun-02 06:18 xsl/extract-latex-image.xsl
+-rw-r--r--  2.0 unx      513 b- defN 23-Jun-02 06:18 xsl/utilities/deprecate-autoname.sed
+-rw-r--r--  2.0 unx      787 b- defN 23-Jun-02 06:18 xsl/utilities/deprecate-index.sed
+-rw-r--r--  2.0 unx    30257 b- defN 23-Jun-02 06:18 xsl/utilities/fix-deprecations.xsl
+-rw-r--r--  2.0 unx     4299 b- defN 23-Jun-02 06:18 xsl/utilities/author-report.xsl
+-rw-r--r--  2.0 unx     4926 b- defN 23-Jun-02 06:18 xsl/utilities/pretext-enhanced-source.xsl
+-rw-r--r--  2.0 unx     1810 b- defN 23-Jun-02 06:18 xsl/utilities/README.md
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 06:18 xsl/support/play-button/
+-rw-r--r--  2.0 unx    10306 b- defN 23-Jun-02 06:18 xsl/support/extract-math.xsl
+-rw-r--r--  2.0 unx     5241 b- defN 23-Jun-02 06:18 xsl/support/pretext-pg-macros.xsl
+-rw-r--r--  2.0 unx      486 b- defN 23-Jun-02 06:18 xsl/support/runestone-services.xml
+-rw-r--r--  2.0 unx     5065 b- defN 23-Jun-02 06:18 xsl/support/extract-latex-image-labels.xsl
+-rw-r--r--  2.0 unx     5879 b- defN 23-Jun-02 06:18 xsl/support/package-math.xsl
+-rw-r--r--  2.0 unx      504 b- defN 23-Jun-02 06:18 xsl/support/README.md
+-rw-r--r--  2.0 unx     5800 b- defN 23-Jun-02 06:18 xsl/support/tactile-svg.xsl
+-rw-r--r--  2.0 unx      722 b- defN 23-Jun-02 06:18 xsl/support/play-button/play-button.svg
+-rw-r--r--  2.0 unx     2657 b- defN 23-Jun-02 06:18 xsl/support/play-button/README.md
+-rw-r--r--  2.0 unx     6621 b- defN 23-Jun-02 06:18 xsl/support/play-button/play-button.png
+-rw-r--r--  2.0 unx    16236 b- defN 23-Jun-02 06:18 xsl/localizations/ca-ES.xml
+-rw-r--r--  2.0 unx    16821 b- defN 23-Jun-02 06:18 xsl/localizations/af-ZA.xml
+-rw-r--r--  2.0 unx    16518 b- defN 23-Jun-02 06:18 xsl/localizations/es-ES.xml
+-rw-r--r--  2.0 unx    17215 b- defN 23-Jun-02 06:18 xsl/localizations/de-DE.xml
+-rw-r--r--  2.0 unx    15566 b- defN 23-Jun-02 06:18 xsl/localizations/cs-CZ.xml
+-rw-r--r--  2.0 unx    19169 b- defN 23-Jun-02 06:18 xsl/localizations/nl-NL.xml
+-rw-r--r--  2.0 unx    19049 b- defN 23-Jun-02 06:18 xsl/localizations/en-US.xml
+-rw-r--r--  2.0 unx    15938 b- defN 23-Jun-02 06:18 xsl/localizations/it-IT.xml
+-rw-r--r--  2.0 unx    17285 b- defN 23-Jun-02 06:18 xsl/localizations/fi-FI.xml
+-rw-r--r--  2.0 unx    16296 b- defN 23-Jun-02 06:18 xsl/localizations/pt-BR.xml
+-rw-r--r--  2.0 unx    16333 b- defN 23-Jun-02 06:18 xsl/localizations/fr-FR.xml
+-rw-r--r--  2.0 unx    17065 b- defN 23-Jun-02 06:18 xsl/localizations/pt-PT.xml
+-rw-r--r--  2.0 unx    16069 b- defN 23-Jun-02 06:18 xsl/localizations/hu-HU.xml
+-rw-r--r--  2.0 unx    16484 b- defN 23-Jun-02 06:18 xsl/localizations/fr-CA.xml
+-rw-r--r--  2.0 unx    17040 b- defN 23-Jun-02 06:18 xsl/localizations/bg-BG.xml
+-rw-r--r--  2.0 unx     2227 b- defN 23-Jun-02 06:18 xsl/localizations/localizations.xml
+-rw-r--r--  2.0 unx     4708 b- defN 23-Jun-02 06:18 xsl/localizations/README.md
+-rw-r--r--  2.0 unx    14482 b- defN 23-Jun-02 06:18 xsl/latex/pretext-latex-chaos.xsl
+-rw-r--r--  2.0 unx     2261 b- defN 23-Jun-02 06:18 xsl/latex/pretext-latex-AIM.xsl
+-rw-r--r--  2.0 unx     7526 b- defN 23-Jun-02 06:18 xsl/latex/pretext-latex-CLP.xsl
+-rw-r--r--  2.0 unx     3024 b- defN 23-Jun-02 06:18 xsl/latex/pretext-latex-dyslexic-font.xsl
+-rw-r--r--  2.0 unx     5135 b- defN 23-Jun-02 06:18 xsl/latex/pretext-latex-guide.xsl
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-02 06:18 css/colors_orange_navy.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-02 06:18 css/colors_green_blue.css
+-rw-r--r--  2.0 unx     2441 b- defN 23-Jun-02 06:18 css/kindle.css
+-rw-r--r--  2.0 unx     4021 b- defN 23-Jun-02 06:18 css/update_css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-02 06:18 css/colors_ruby_turquoise.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-02 06:18 css/colors_ruby_amethyst.css
+-rw-r--r--  2.0 unx     2608 b- defN 23-Jun-02 06:18 css/colors_default.css
+-rw-r--r--  2.0 unx     1338 b- defN 23-Jun-02 06:18 css/colors_red_blue.css
+-rw-r--r--  2.0 unx      691 b- defN 23-Jun-02 06:18 css/colors_pastel_blue_orange.css
+-rw-r--r--  2.0 unx     3473 b- defN 23-Jun-02 06:18 css/style_soundwriting.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-Jun-02 06:18 css/colors_darkmartiansands.css
+-rw-r--r--  2.0 unx     2438 b- defN 23-Jun-02 06:18 css/colors_blue_grey.css
+-rw-r--r--  2.0 unx     4308 b- defN 23-Jun-02 06:18 css/colors_blue_green.css
+-rw-r--r--  2.0 unx   146685 b- defN 23-Jun-02 06:18 css/mathbook-content.css
+-rw-r--r--  2.0 unx     1276 b- defN 23-Jun-02 06:18 css/colors_maroon_grey.css
+-rw-r--r--  2.0 unx    22438 b- defN 23-Jun-02 06:18 css/pretext.css
+-rw-r--r--  2.0 unx     1280 b- defN 23-Jun-02 06:18 css/colors_brown_gold.css
+-rw-r--r--  2.0 unx     1362 b- defN 23-Jun-02 06:18 css/epub.css
+-rw-r--r--  2.0 unx    63664 b- defN 23-Jun-02 06:18 css/mathbook-add-on.css
+-rw-r--r--  2.0 unx    14069 b- defN 23-Jun-02 06:18 css/setcolors.css
+-rw-r--r--  2.0 unx    71198 b- defN 23-Jun-02 06:18 css/pretext_add_on.css
+-rw-r--r--  2.0 unx   435680 b- defN 23-Jun-02 06:18 css/mathbook-3.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-02 06:18 css/colors_green_plum.css
+-rw-r--r--  2.0 unx    12567 b- defN 23-Jun-02 06:18 css/style_oscarlevin.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-02 06:18 css/colors_blue_red.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-Jun-02 06:18 css/colors_martiansands.css
+-rw-r--r--  2.0 unx     1865 b- defN 23-Jun-02 06:18 css/README.md
+-rw-r--r--  2.0 unx     7761 b- defN 23-Jun-02 06:18 css/style_default.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-02 06:18 css/colors_ruby_emerald.css
+-rw-r--r--  2.0 unx    35449 b- defN 23-Jun-02 06:18 pretext/braille_format.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 06:18 pretext/__init__.py
+-rw-r--r--  2.0 unx     2566 b- defN 23-Jun-02 06:18 pretext/pretext.cfg
+-rw-r--r--  2.0 unx    30908 b- defN 23-Jun-02 06:18 pretext/pretext
+-rw-r--r--  2.0 unx     1955 b- defN 23-Jun-02 06:18 pretext/module-test.py
+-rw-r--r--  2.0 unx   172432 b- defN 23-Jun-02 06:18 pretext/pretext.py
+-rw-r--r--  2.0 unx     1367 b- defN 23-Jun-02 06:18 pretext/README.md
+-rw-r--r--  2.0 unx      326 b- defN 23-Jun-02 06:18 schema/xml.xsd
+-rw-r--r--  2.0 unx    18421 b- defN 23-Jun-02 06:18 schema/pretext-schematron.xsl
+-rw-r--r--  2.0 unx    17587 b- defN 23-Jun-02 06:18 schema/pretext-dev.rnc
+-rw-r--r--  2.0 unx   134043 b- defN 23-Jun-02 06:18 schema/pretext.xml
+-rw-r--r--  2.0 unx    58086 b- defN 23-Jun-02 06:18 schema/pretext.rnc
+-rw-r--r--  2.0 unx   101829 b- defN 23-Jun-02 06:18 schema/pretext.rng
+-rw-r--r--  2.0 unx    34210 b- defN 23-Jun-02 06:18 schema/pretext-dev.rng
+-rw-r--r--  2.0 unx     3135 b- defN 23-Jun-02 06:18 schema/build.sh
+-rw-r--r--  2.0 unx   125135 b- defN 23-Jun-02 06:18 schema/pretext.xsd
+-rw-r--r--  2.0 unx     1180 b- defN 23-Jun-02 06:18 schema/README.md
+-rw-r--r--  2.0 unx    25290 b- defN 23-Jun-02 06:18 schema/pretext-validation-plus.xsl
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 06:18 script/mjsre/
+-rw-r--r--  2.0 unx     2666 b- defN 23-Jun-02 06:18 script/mbx
+-rw-r--r--  2.0 unx      258 b- defN 23-Jun-02 06:18 script/README.md
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-02 06:18 script/mjsre/update-sre
+-rw-r--r--  2.0 unx      116 b- defN 23-Jun-02 06:18 script/mjsre/package.json
+-rw-r--r--  2.0 unx      481 b- defN 23-Jun-02 06:18 script/mjsre/README.md
+-rw-r--r--  2.0 unx     9251 b- defN 23-Jun-02 06:18 script/mjsre/mj-sre-page.js
+140 files, 4820567 bytes uncompressed, 1014430 bytes compressed:  79.0%
```

#### zipnote {}

```diff
@@ -9,413 +9,413 @@
 
 Filename: script/
 Comment: 
 
 Filename: xsl/
 Comment: 
 
-Filename: script/mjsre/
+Filename: xsl/latex/
 Comment: 
 
-Filename: script/README.md
+Filename: xsl/localizations/
 Comment: 
 
-Filename: script/mbx
+Filename: xsl/support/
 Comment: 
 
-Filename: script/mjsre/update-sre
+Filename: xsl/utilities/
 Comment: 
 
-Filename: script/mjsre/README.md
+Filename: xsl/publisher-variables.xsl
 Comment: 
 
-Filename: script/mjsre/package.json
+Filename: xsl/pretext-html.xsl
 Comment: 
 
-Filename: script/mjsre/mj-sre-page.js
+Filename: xsl/pretext-json-manifest.xsl
 Comment: 
 
-Filename: schema/pretext-schematron.xsl
+Filename: xsl/pretext-litprog.xsl
 Comment: 
 
-Filename: schema/pretext.rnc
+Filename: xsl/extract-asymptote.xsl
 Comment: 
 
-Filename: schema/pretext-validation-plus.xsl
+Filename: xsl/extract-pg.xsl
 Comment: 
 
-Filename: schema/pretext.xml
+Filename: xsl/entities.ent
 Comment: 
 
-Filename: schema/README.md
+Filename: xsl/pretext-solution-manual-latex.xsl
 Comment: 
 
-Filename: schema/pretext.xsd
+Filename: xsl/pretext-numbers.xsl
 Comment: 
 
-Filename: schema/xml.xsd
+Filename: xsl/extract-trace.xsl
 Comment: 
 
-Filename: schema/pretext-dev.rng
+Filename: xsl/pretext-view-source.xsl
 Comment: 
 
-Filename: schema/pretext.rng
+Filename: xsl/pretext-units.xsl
 Comment: 
 
-Filename: schema/pretext-dev.rnc
+Filename: xsl/extract-interactive.xsl
 Comment: 
 
-Filename: schema/build.sh
+Filename: xsl/pretext-jupyter.xsl
 Comment: 
 
-Filename: pretext/README.md
+Filename: xsl/pretext-assembly.xsl
 Comment: 
 
-Filename: pretext/pretext.py
+Filename: xsl/pretext-text-utilities.xsl
 Comment: 
 
-Filename: pretext/module-test.py
+Filename: xsl/pretext-runestone-static.xsl
 Comment: 
 
-Filename: pretext/pretext
+Filename: xsl/pretext-text.xsl
 Comment: 
 
-Filename: pretext/__init__.py
+Filename: xsl/pretext-braille-preprint.xsl
 Comment: 
 
-Filename: pretext/braille_format.py
+Filename: xsl/extract-datafile.xsl
 Comment: 
 
-Filename: pretext/pretext.cfg
+Filename: xsl/pretext-merge.xsl
 Comment: 
 
-Filename: xsl/latex/
+Filename: xsl/pretext-ww-problem-sets.xsl
 Comment: 
 
-Filename: xsl/localizations/
+Filename: xsl/pretext-common.xsl
 Comment: 
 
-Filename: xsl/support/
+Filename: xsl/pretext-smc.xsl
 Comment: 
 
-Filename: xsl/utilities/
+Filename: xsl/extract-sageplot.xsl
 Comment: 
 
-Filename: xsl/entities.ent
+Filename: xsl/extract-identity.xsl
 Comment: 
 
-Filename: xsl/extract-interactive.xsl
+Filename: xsl/pretext-beamer.xsl
 Comment: 
 
-Filename: xsl/pretext-text.xsl
+Filename: xsl/pretext-runestone.xsl
 Comment: 
 
-Filename: xsl/README.md
+Filename: xsl/pretext-basic-html.xsl
 Comment: 
 
-Filename: xsl/extract-pg.xsl
+Filename: xsl/extract-qrcode.xsl
 Comment: 
 
-Filename: xsl/pretext-json-manifest.xsl
+Filename: xsl/extract-mom.xsl
 Comment: 
 
-Filename: xsl/pretext-revealjs.xsl
+Filename: xsl/extract-youtube.xsl
 Comment: 
 
-Filename: xsl/extract-datafile.xsl
+Filename: xsl/README.md
 Comment: 
 
-Filename: xsl/extract-identity.xsl
+Filename: xsl/pretext-epub.xsl
 Comment: 
 
-Filename: xsl/extract-sageplot.xsl
+Filename: xsl/pretext-sage-doctest.xsl
 Comment: 
 
-Filename: xsl/publisher-variables.xsl
+Filename: xsl/pretext-revealjs.xsl
 Comment: 
 
-Filename: xsl/pretext-runestone.xsl
+Filename: xsl/pretext-latex.xsl
 Comment: 
 
-Filename: xsl/pretext-sage-doctest.xsl
+Filename: xsl/extract-latex-image.xsl
 Comment: 
 
-Filename: xsl/pretext-runestone-static.xsl
+Filename: xsl/utilities/deprecate-autoname.sed
 Comment: 
 
-Filename: xsl/pretext-ww-problem-sets.xsl
+Filename: xsl/utilities/deprecate-index.sed
 Comment: 
 
-Filename: xsl/pretext-latex.xsl
+Filename: xsl/utilities/fix-deprecations.xsl
 Comment: 
 
-Filename: xsl/pretext-merge.xsl
+Filename: xsl/utilities/author-report.xsl
 Comment: 
 
-Filename: xsl/pretext-litprog.xsl
+Filename: xsl/utilities/pretext-enhanced-source.xsl
 Comment: 
 
-Filename: xsl/extract-latex-image.xsl
+Filename: xsl/utilities/README.md
 Comment: 
 
-Filename: xsl/pretext-epub.xsl
+Filename: xsl/support/play-button/
 Comment: 
 
-Filename: xsl/pretext-view-source.xsl
+Filename: xsl/support/extract-math.xsl
 Comment: 
 
-Filename: xsl/pretext-numbers.xsl
+Filename: xsl/support/pretext-pg-macros.xsl
 Comment: 
 
-Filename: xsl/pretext-assembly.xsl
+Filename: xsl/support/runestone-services.xml
 Comment: 
 
-Filename: xsl/extract-mom.xsl
+Filename: xsl/support/extract-latex-image-labels.xsl
 Comment: 
 
-Filename: xsl/pretext-smc.xsl
+Filename: xsl/support/package-math.xsl
 Comment: 
 
-Filename: xsl/pretext-common.xsl
+Filename: xsl/support/README.md
 Comment: 
 
-Filename: xsl/extract-youtube.xsl
+Filename: xsl/support/tactile-svg.xsl
 Comment: 
 
-Filename: xsl/pretext-beamer.xsl
+Filename: xsl/support/play-button/play-button.svg
 Comment: 
 
-Filename: xsl/pretext-solution-manual-latex.xsl
+Filename: xsl/support/play-button/README.md
 Comment: 
 
-Filename: xsl/pretext-braille-preprint.xsl
+Filename: xsl/support/play-button/play-button.png
 Comment: 
 
-Filename: xsl/pretext-units.xsl
+Filename: xsl/localizations/ca-ES.xml
 Comment: 
 
-Filename: xsl/pretext-basic-html.xsl
+Filename: xsl/localizations/af-ZA.xml
 Comment: 
 
-Filename: xsl/extract-asymptote.xsl
+Filename: xsl/localizations/es-ES.xml
 Comment: 
 
-Filename: xsl/pretext-html.xsl
+Filename: xsl/localizations/de-DE.xml
 Comment: 
 
-Filename: xsl/extract-trace.xsl
+Filename: xsl/localizations/cs-CZ.xml
 Comment: 
 
-Filename: xsl/pretext-text-utilities.xsl
+Filename: xsl/localizations/nl-NL.xml
 Comment: 
 
-Filename: xsl/pretext-jupyter.xsl
+Filename: xsl/localizations/en-US.xml
 Comment: 
 
-Filename: xsl/extract-qrcode.xsl
+Filename: xsl/localizations/it-IT.xml
 Comment: 
 
-Filename: xsl/latex/pretext-latex-CLP.xsl
+Filename: xsl/localizations/fi-FI.xml
 Comment: 
 
-Filename: xsl/latex/pretext-latex-dyslexic-font.xsl
+Filename: xsl/localizations/pt-BR.xml
 Comment: 
 
-Filename: xsl/latex/pretext-latex-AIM.xsl
+Filename: xsl/localizations/fr-FR.xml
 Comment: 
 
-Filename: xsl/latex/pretext-latex-chaos.xsl
+Filename: xsl/localizations/pt-PT.xml
 Comment: 
 
-Filename: xsl/latex/pretext-latex-guide.xsl
+Filename: xsl/localizations/hu-HU.xml
 Comment: 
 
-Filename: xsl/support/play-button/
+Filename: xsl/localizations/fr-CA.xml
 Comment: 
 
-Filename: xsl/support/README.md
+Filename: xsl/localizations/bg-BG.xml
 Comment: 
 
-Filename: xsl/support/extract-math.xsl
+Filename: xsl/localizations/localizations.xml
 Comment: 
 
-Filename: xsl/support/pretext-pg-macros.xsl
+Filename: xsl/localizations/README.md
 Comment: 
 
-Filename: xsl/support/package-math.xsl
+Filename: xsl/latex/pretext-latex-chaos.xsl
 Comment: 
 
-Filename: xsl/support/runestone-services.xml
+Filename: xsl/latex/pretext-latex-AIM.xsl
 Comment: 
 
-Filename: xsl/support/tactile-svg.xsl
+Filename: xsl/latex/pretext-latex-CLP.xsl
 Comment: 
 
-Filename: xsl/support/extract-latex-image-labels.xsl
+Filename: xsl/latex/pretext-latex-dyslexic-font.xsl
 Comment: 
 
-Filename: xsl/support/play-button/README.md
+Filename: xsl/latex/pretext-latex-guide.xsl
 Comment: 
 
-Filename: xsl/support/play-button/play-button.svg
+Filename: css/colors_orange_navy.css
 Comment: 
 
-Filename: xsl/support/play-button/play-button.png
+Filename: css/colors_green_blue.css
 Comment: 
 
-Filename: xsl/localizations/es-ES.xml
+Filename: css/kindle.css
 Comment: 
 
-Filename: xsl/localizations/hu-HU.xml
+Filename: css/update_css
 Comment: 
 
-Filename: xsl/localizations/de-DE.xml
+Filename: css/colors_ruby_turquoise.css
 Comment: 
 
-Filename: xsl/localizations/fr-FR.xml
+Filename: css/colors_ruby_amethyst.css
 Comment: 
 
-Filename: xsl/localizations/fi-FI.xml
+Filename: css/colors_default.css
 Comment: 
 
-Filename: xsl/localizations/README.md
+Filename: css/colors_red_blue.css
 Comment: 
 
-Filename: xsl/localizations/it-IT.xml
+Filename: css/colors_pastel_blue_orange.css
 Comment: 
 
-Filename: xsl/localizations/af-ZA.xml
+Filename: css/style_soundwriting.css
 Comment: 
 
-Filename: xsl/localizations/ca-ES.xml
+Filename: css/colors_darkmartiansands.css
 Comment: 
 
-Filename: xsl/localizations/en-US.xml
+Filename: css/colors_blue_grey.css
 Comment: 
 
-Filename: xsl/localizations/nl-NL.xml
+Filename: css/colors_blue_green.css
 Comment: 
 
-Filename: xsl/localizations/localizations.xml
+Filename: css/mathbook-content.css
 Comment: 
 
-Filename: xsl/localizations/cs-CZ.xml
+Filename: css/colors_maroon_grey.css
 Comment: 
 
-Filename: xsl/localizations/bg-BG.xml
+Filename: css/pretext.css
 Comment: 
 
-Filename: xsl/localizations/pt-PT.xml
+Filename: css/colors_brown_gold.css
 Comment: 
 
-Filename: xsl/localizations/fr-CA.xml
+Filename: css/epub.css
 Comment: 
 
-Filename: xsl/localizations/pt-BR.xml
+Filename: css/mathbook-add-on.css
 Comment: 
 
-Filename: xsl/utilities/README.md
+Filename: css/setcolors.css
 Comment: 
 
-Filename: xsl/utilities/fix-deprecations.xsl
+Filename: css/pretext_add_on.css
 Comment: 
 
-Filename: xsl/utilities/pretext-enhanced-source.xsl
+Filename: css/mathbook-3.css
 Comment: 
 
-Filename: xsl/utilities/deprecate-autoname.sed
+Filename: css/colors_green_plum.css
 Comment: 
 
-Filename: xsl/utilities/author-report.xsl
+Filename: css/style_oscarlevin.css
 Comment: 
 
-Filename: xsl/utilities/deprecate-index.sed
+Filename: css/colors_blue_red.css
 Comment: 
 
-Filename: css/colors_maroon_grey.css
+Filename: css/colors_martiansands.css
 Comment: 
 
-Filename: css/style_default.css
+Filename: css/README.md
 Comment: 
 
-Filename: css/style_soundwriting.css
+Filename: css/style_default.css
 Comment: 
 
-Filename: css/mathbook-add-on.css
+Filename: css/colors_ruby_emerald.css
 Comment: 
 
-Filename: css/README.md
+Filename: pretext/braille_format.py
 Comment: 
 
-Filename: css/colors_brown_gold.css
+Filename: pretext/__init__.py
 Comment: 
 
-Filename: css/colors_blue_red.css
+Filename: pretext/pretext.cfg
 Comment: 
 
-Filename: css/mathbook-3.css
+Filename: pretext/pretext
 Comment: 
 
-Filename: css/mathbook-content.css
+Filename: pretext/module-test.py
 Comment: 
 
-Filename: css/pretext.css
+Filename: pretext/pretext.py
 Comment: 
 
-Filename: css/colors_green_plum.css
+Filename: pretext/README.md
 Comment: 
 
-Filename: css/colors_ruby_turquoise.css
+Filename: schema/xml.xsd
 Comment: 
 
-Filename: css/colors_blue_green.css
+Filename: schema/pretext-schematron.xsl
 Comment: 
 
-Filename: css/pretext_add_on.css
+Filename: schema/pretext-dev.rnc
 Comment: 
 
-Filename: css/colors_default.css
+Filename: schema/pretext.xml
 Comment: 
 
-Filename: css/colors_blue_grey.css
+Filename: schema/pretext.rnc
 Comment: 
 
-Filename: css/colors_green_blue.css
+Filename: schema/pretext.rng
 Comment: 
 
-Filename: css/colors_darkmartiansands.css
+Filename: schema/pretext-dev.rng
 Comment: 
 
-Filename: css/colors_orange_navy.css
+Filename: schema/build.sh
 Comment: 
 
-Filename: css/style_oscarlevin.css
+Filename: schema/pretext.xsd
 Comment: 
 
-Filename: css/colors_pastel_blue_orange.css
+Filename: schema/README.md
 Comment: 
 
-Filename: css/colors_red_blue.css
+Filename: schema/pretext-validation-plus.xsl
 Comment: 
 
-Filename: css/setcolors.css
+Filename: script/mjsre/
 Comment: 
 
-Filename: css/colors_ruby_amethyst.css
+Filename: script/mbx
 Comment: 
 
-Filename: css/colors_martiansands.css
+Filename: script/README.md
 Comment: 
 
-Filename: css/epub.css
+Filename: script/mjsre/update-sre
 Comment: 
 
-Filename: css/kindle.css
+Filename: script/mjsre/package.json
 Comment: 
 
-Filename: css/colors_ruby_emerald.css
+Filename: script/mjsre/README.md
 Comment: 
 
-Filename: css/update_css
+Filename: script/mjsre/mj-sre-page.js
 Comment: 
 
 Zip file comment:
```

#### xsl/pretext-runestone.xsl

##### xsl/pretext-runestone.xsl

```diff
@@ -1562,15 +1562,19 @@
   <!-- TODO: are start/end attributes useful?      -->
   <xsl:template match="video[@youtube]" mode="runestone-youtube-embed">
     <xsl:param name="width"/>
     <xsl:param name="height"/>
     <xsl:variable name="hid">
       <xsl:apply-templates select="." mode="runestone-id"/>
     </xsl:variable>
-    <div id="{$hid}" data-component="youtube" class="align-left youtube-video" data-video-height="{$height}" data-video-width="{$width}" data-video-videoid="{@youtube}" data-video-divid="{$hid}" data-video-start="0" data-video-end="-1"/>
+    <div class="ptx-runestone-container">
+      <div class="runestone">
+        <div id="{$hid}" data-component="youtube" class="align-left youtube-video" data-video-height="{$height}" data-video-width="{$width}" data-video-videoid="{@youtube}" data-video-divid="{$hid}" data-video-start="0" data-video-end="-1"/>
+      </div>
+    </div>
   </xsl:template>
   <!-- ########### -->
   <!-- Active Code -->
   <!-- ########### -->
   <!-- Runestone has support for various languages.  Some    -->
   <!-- are "in-browser" while others are backed by "real"    -->
   <!-- compilers as part of a Runestone server.  For an      -->
```

#### xsl/pretext-html.xsl

##### xsl/pretext-html.xsl

```diff
@@ -10921,20 +10921,22 @@
       </xsl:choose>
       <!-- Button to show/hide the calculator -->
       <xsl:if test="$b-has-calculator">
         <xsl:call-template name="calculator-toggle"/>
         <xsl:call-template name="calculator"/>
       </xsl:if>
       <!-- Runestone user menu -->
-      <!-- Conditional on a build for Runestone hosting -->
-      <xsl:call-template name="runestone-bust-menu"/>
-      <!-- A scratch ActiveCode via a pencil icon, always -->
-      <xsl:call-template name="runestone-scratch-activecode"/>
-      <!-- The user-preferences-menu needs to be unified with the runestone-bust-menu -->
-      <xsl:call-template name="user-preferences-menu"/>
+      <xsl:if test="not($b-debug-react)">
+        <!-- Conditional on a build for Runestone hosting -->
+        <xsl:call-template name="runestone-bust-menu"/>
+        <!-- A scratch ActiveCode via a pencil icon, always -->
+        <xsl:call-template name="runestone-scratch-activecode"/>
+        <!-- The user-preferences-menu needs to be unified with the runestone-bust-menu -->
+        <xsl:call-template name="user-preferences-menu"/>
+      </xsl:if>
       <!-- Span to encase Prev/Up/Next buttons and float right    -->
       <!-- Each button gets an id for keypress recognition/action -->
       <span class="treebuttons">
         <xsl:apply-templates select="." mode="previous-button"/>
         <xsl:if test="$nav-upbutton='yes'">
           <xsl:apply-templates select="." mode="up-button"/>
         </xsl:if>
@@ -11853,24 +11855,24 @@
         </xsl:with-param>
         <xsl:with-param name="language-text">Singular</xsl:with-param>
       </xsl:call-template>
     </xsl:if>
   </xsl:template>
   <!-- Program Listings highlighted by Prism -->
   <xsl:template name="syntax-highlight">
-    <xsl:if test="$b-has-program">
+    <xsl:if test="$b-has-program and not($b-debug-react)">
       <link href="https://cdnjs.cloudflare.com/ajax/libs/prism/1.26.0/themes/prism.css" rel="stylesheet"/>
       <script src="https://cdnjs.cloudflare.com/ajax/libs/prism/1.26.0/components/prism-core.min.js"/>
       <script src="https://cdnjs.cloudflare.com/ajax/libs/prism/1.26.0/plugins/autoloader/prism-autoloader.min.js"/>
     </xsl:if>
   </xsl:template>
   <!-- JS setup for a Google Custom Search Engine box -->
   <!-- Empty if not enabled via presence of cx number -->
   <xsl:template name="google-search-box-js">
-    <xsl:if test="$b-google-cse">
+    <xsl:if test="$b-google-cse and not($b-debug-react)">
       <script async="">
         <xsl:attribute name="src">
           <xsl:text>https://cse.google.com/cse.js?cx=</xsl:text>
           <xsl:value-of select="$google-search-cx"/>
         </xsl:attribute>
       </script>
     </xsl:if>
@@ -11889,15 +11891,15 @@
   <!-- JS for native search -->
   <!-- The async attribute may help with slow downloads,  -->
   <!-- especially the project-specific search-file which  -->
   <!-- can be as large as several megabytes.              -->
   <!-- NB: async attribute also on Lunr and PTX-JS        -->
   <!-- resulted in console errors (2022-02-08)            -->
   <xsl:template name="native-search-box-js">
-    <xsl:if test="$has-native-search">
+    <xsl:if test="$has-native-search and not($b-debug-react)">
       <script src="https://cdnjs.cloudflare.com/ajax/libs/lunr.js/2.3.9/lunr.min.js" integrity="sha512-4xUl/d6D6THrAnXAwGajXkoWaeMNwEKK4iNfq5DotEbLPAfk6FSxSP3ydNxqDgCw1c/0Z1Jg6L8h2j+++9BZmg==" crossorigin="anonymous" referrerpolicy="no-referrer"/>
       <!-- document-specific variables with search documents -->
       <script src="{$lunr-search-file}" async=""/>
       <!-- PreTeXt Javascript and CSS to form and render results of a search -->
       <script src="{$html.js.server}/js/{$html.js.version}/pretext_search.js"/>
       <link href="{$html.css.server}/css/{$html.css.version}/pretext_search.css" rel="stylesheet" type="text/css"/>
     </xsl:if>
```

### Comparing `pretext-1.5.4.dev20230601/pretext/generate.py` & `pretext-1.5.4.dev20230602/pretext/generate.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230601/pretext/project.py` & `pretext-1.5.4.dev20230602/pretext/project.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230601/pretext/templates/__init__.py` & `pretext-1.5.4.dev20230602/pretext/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230601/pretext/templates/resources/.gitignore` & `pretext-1.5.4.dev20230602/pretext/templates/resources/.gitignore`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230601/pretext/templates/resources/article.zip` & `pretext-1.5.4.dev20230602/pretext/templates/resources/article.zip`

 * *Files 4% similar despite different names*

#### zipinfo {}

```diff
@@ -1,16 +1,16 @@
 Zip file size: 160064 bytes, number of entries: 14
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 06:19 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 06:19 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 06:19 source/
--rw-r--r--  2.0 unx       86 b- defN 23-Jun-01 06:19 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-Jun-01 06:19 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-01 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-01 06:19 .gitignore
--rw-r--r--  2.0 unx   154806 b- defN 23-Jun-01 06:19 assets/frog.jpg
--rw-r--r--  2.0 unx     2059 b- defN 23-Jun-01 06:19 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      242 b- defN 23-Jun-01 06:19 publication/publication.ptx
--rw-r--r--  2.0 unx      430 b- defN 23-Jun-01 06:19 source/main.ptx
--rw-r--r--  2.0 unx      449 b- defN 23-Jun-01 06:19 source/section-1.ptx
--rw-r--r--  2.0 unx      982 b- defN 23-Jun-01 06:19 source/section-2.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 06:18 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 06:18 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 06:18 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 06:18 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-02 06:18 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-02 06:18 codechat_config.yaml
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jun-02 06:18 project.ptx
+-rw-r--r--  2.0 unx       86 b- defN 23-Jun-02 06:18 README.md
+-rw-r--r--  2.0 unx   154806 b- defN 23-Jun-02 06:18 assets/frog.jpg
+-rw-r--r--  2.0 unx      242 b- defN 23-Jun-02 06:18 publication/publication.ptx
+-rw-r--r--  2.0 unx      430 b- defN 23-Jun-02 06:18 source/main.ptx
+-rw-r--r--  2.0 unx      449 b- defN 23-Jun-02 06:18 source/section-1.ptx
+-rw-r--r--  2.0 unx      982 b- defN 23-Jun-02 06:18 source/section-2.ptx
+-rw-r--r--  2.0 unx     2059 b- defN 23-Jun-02 06:18 .devcontainer/devcontainer.json
 14 files, 164708 bytes uncompressed, 158542 bytes compressed:  3.7%
```

#### zipnote {}

```diff
@@ -6,38 +6,38 @@
 
 Filename: publication/
 Comment: 
 
 Filename: source/
 Comment: 
 
-Filename: README.md
-Comment: 
-
-Filename: project.ptx
+Filename: .gitignore
 Comment: 
 
 Filename: codechat_config.yaml
 Comment: 
 
-Filename: .gitignore
+Filename: project.ptx
 Comment: 
 
-Filename: assets/frog.jpg
+Filename: README.md
 Comment: 
 
-Filename: .devcontainer/devcontainer.json
+Filename: assets/frog.jpg
 Comment: 
 
 Filename: publication/publication.ptx
 Comment: 
 
 Filename: source/main.ptx
 Comment: 
 
 Filename: source/section-1.ptx
 Comment: 
 
 Filename: source/section-2.ptx
 Comment: 
 
+Filename: .devcontainer/devcontainer.json
+Comment: 
+
 Zip file comment:
```

### Comparing `pretext-1.5.4.dev20230601/pretext/templates/resources/book.zip` & `pretext-1.5.4.dev20230602/pretext/templates/resources/book.zip`

 * *Files 11% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 7570 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 06:19 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 06:19 source/
--rw-r--r--  2.0 unx       82 b- defN 23-Jun-01 06:19 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-Jun-01 06:19 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-01 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-01 06:19 .gitignore
--rw-r--r--  2.0 unx     2059 b- defN 23-Jun-01 06:19 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx     6114 b- defN 23-Jun-01 06:19 publication/publication.ptx
--rw-r--r--  2.0 unx     1767 b- defN 23-Jun-01 06:19 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 06:18 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 06:18 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 06:18 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-02 06:18 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-02 06:18 codechat_config.yaml
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jun-02 06:18 project.ptx
+-rw-r--r--  2.0 unx       82 b- defN 23-Jun-02 06:18 README.md
+-rw-r--r--  2.0 unx     6114 b- defN 23-Jun-02 06:18 publication/publication.ptx
+-rw-r--r--  2.0 unx     1767 b- defN 23-Jun-02 06:18 source/main.ptx
+-rw-r--r--  2.0 unx     2059 b- defN 23-Jun-02 06:18 .devcontainer/devcontainer.json
 10 files, 15676 bytes uncompressed, 6476 bytes compressed:  58.7%
```

#### zipnote {}

```diff
@@ -3,29 +3,29 @@
 
 Filename: publication/
 Comment: 
 
 Filename: source/
 Comment: 
 
-Filename: README.md
-Comment: 
-
-Filename: project.ptx
+Filename: .gitignore
 Comment: 
 
 Filename: codechat_config.yaml
 Comment: 
 
-Filename: .gitignore
+Filename: project.ptx
 Comment: 
 
-Filename: .devcontainer/devcontainer.json
+Filename: README.md
 Comment: 
 
 Filename: publication/publication.ptx
 Comment: 
 
 Filename: source/main.ptx
 Comment: 
 
+Filename: .devcontainer/devcontainer.json
+Comment: 
+
 Zip file comment:
```

### Comparing `pretext-1.5.4.dev20230601/pretext/templates/resources/demo.zip` & `pretext-1.5.4.dev20230602/pretext/templates/resources/demo.zip`

 * *Files 7% similar despite different names*

#### zipinfo {}

```diff
@@ -1,36 +1,36 @@
 Zip file size: 173263 bytes, number of entries: 34
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 06:19 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 06:19 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 06:19 source/
--rw-r--r--  2.0 unx       82 b- defN 23-Jun-01 06:19 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-Jun-01 06:19 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-01 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-01 06:19 .gitignore
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 06:19 assets/jsxgraph/
--rw-r--r--  2.0 unx   154806 b- defN 23-Jun-01 06:19 assets/frog.jpg
--rw-r--r--  2.0 unx     1737 b- defN 23-Jun-01 06:19 assets/jsxgraph/infinity.js
--rw-r--r--  2.0 unx     2059 b- defN 23-Jun-01 06:19 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx     6092 b- defN 23-Jun-01 06:19 publication/publication.ptx
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 06:19 source/images/
--rw-r--r--  2.0 unx      847 b- defN 23-Jun-01 06:19 source/sec-first-intro.ptx
--rw-r--r--  2.0 unx     2517 b- defN 23-Jun-01 06:19 source/main.ptx
--rw-r--r--  2.0 unx     1697 b- defN 23-Jun-01 06:19 source/sec-first-examples.ptx
--rw-r--r--  2.0 unx      375 b- defN 23-Jun-01 06:19 source/fig-sage2d.ptx
--rw-r--r--  2.0 unx      381 b- defN 23-Jun-01 06:19 source/fig-tikz.ptx
--rw-r--r--  2.0 unx      411 b- defN 23-Jun-01 06:19 source/fig-sage3d.ptx
--rw-r--r--  2.0 unx      335 b- defN 23-Jun-01 06:19 source/fig-asymptote.ptx
--rw-r--r--  2.0 unx     2080 b- defN 23-Jun-01 06:19 source/frontmatter.ptx
--rw-r--r--  2.0 unx      339 b- defN 23-Jun-01 06:19 source/ch-features.ptx
--rw-r--r--  2.0 unx     3036 b- defN 23-Jun-01 06:19 source/ch-generate.ptx
--rw-r--r--  2.0 unx      867 b- defN 23-Jun-01 06:19 source/sec-features.ptx
--rw-r--r--  2.0 unx      885 b- defN 23-Jun-01 06:19 source/backmatter.ptx
--rw-r--r--  2.0 unx     1115 b- defN 23-Jun-01 06:19 source/ch-first with spaces.ptx
--rw-r--r--  2.0 unx      230 b- defN 23-Jun-01 06:19 source/ch-empty.ptx
--rw-r--r--  2.0 unx     1515 b- defN 23-Jun-01 06:19 source/ex-first.ptx
--rw-r--r--  2.0 unx     1616 b- defN 23-Jun-01 06:19 source/docinfo.ptx
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-01 06:19 source/images/sageplot2d.sage
--rw-r--r--  2.0 unx      835 b- defN 23-Jun-01 06:19 source/images/cflag.asy
--rw-r--r--  2.0 unx      357 b- defN 23-Jun-01 06:19 source/images/tikz.tex
--rw-r--r--  2.0 unx       93 b- defN 23-Jun-01 06:19 source/images/sageplot3d.sage
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 06:18 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 06:18 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 06:18 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 06:18 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-02 06:18 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-02 06:18 codechat_config.yaml
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jun-02 06:18 project.ptx
+-rw-r--r--  2.0 unx       82 b- defN 23-Jun-02 06:18 README.md
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 06:18 assets/jsxgraph/
+-rw-r--r--  2.0 unx   154806 b- defN 23-Jun-02 06:18 assets/frog.jpg
+-rw-r--r--  2.0 unx     1737 b- defN 23-Jun-02 06:18 assets/jsxgraph/infinity.js
+-rw-r--r--  2.0 unx     6092 b- defN 23-Jun-02 06:18 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 06:18 source/images/
+-rw-r--r--  2.0 unx      867 b- defN 23-Jun-02 06:18 source/sec-features.ptx
+-rw-r--r--  2.0 unx      411 b- defN 23-Jun-02 06:18 source/fig-sage3d.ptx
+-rw-r--r--  2.0 unx     2080 b- defN 23-Jun-02 06:18 source/frontmatter.ptx
+-rw-r--r--  2.0 unx     1515 b- defN 23-Jun-02 06:18 source/ex-first.ptx
+-rw-r--r--  2.0 unx     1115 b- defN 23-Jun-02 06:18 source/ch-first with spaces.ptx
+-rw-r--r--  2.0 unx     2517 b- defN 23-Jun-02 06:18 source/main.ptx
+-rw-r--r--  2.0 unx     3036 b- defN 23-Jun-02 06:18 source/ch-generate.ptx
+-rw-r--r--  2.0 unx      885 b- defN 23-Jun-02 06:18 source/backmatter.ptx
+-rw-r--r--  2.0 unx      375 b- defN 23-Jun-02 06:18 source/fig-sage2d.ptx
+-rw-r--r--  2.0 unx     1697 b- defN 23-Jun-02 06:18 source/sec-first-examples.ptx
+-rw-r--r--  2.0 unx      847 b- defN 23-Jun-02 06:18 source/sec-first-intro.ptx
+-rw-r--r--  2.0 unx      339 b- defN 23-Jun-02 06:18 source/ch-features.ptx
+-rw-r--r--  2.0 unx      335 b- defN 23-Jun-02 06:18 source/fig-asymptote.ptx
+-rw-r--r--  2.0 unx      381 b- defN 23-Jun-02 06:18 source/fig-tikz.ptx
+-rw-r--r--  2.0 unx      230 b- defN 23-Jun-02 06:18 source/ch-empty.ptx
+-rw-r--r--  2.0 unx     1616 b- defN 23-Jun-02 06:18 source/docinfo.ptx
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-02 06:18 source/images/sageplot2d.sage
+-rw-r--r--  2.0 unx      357 b- defN 23-Jun-02 06:18 source/images/tikz.tex
+-rw-r--r--  2.0 unx       93 b- defN 23-Jun-02 06:18 source/images/sageplot3d.sage
+-rw-r--r--  2.0 unx      835 b- defN 23-Jun-02 06:18 source/images/cflag.asy
+-rw-r--r--  2.0 unx     2059 b- defN 23-Jun-02 06:18 .devcontainer/devcontainer.json
 34 files, 189971 bytes uncompressed, 169307 bytes compressed:  10.9%
```

#### zipnote {}

```diff
@@ -6,98 +6,98 @@
 
 Filename: publication/
 Comment: 
 
 Filename: source/
 Comment: 
 
-Filename: README.md
+Filename: .gitignore
 Comment: 
 
-Filename: project.ptx
+Filename: codechat_config.yaml
 Comment: 
 
-Filename: codechat_config.yaml
+Filename: project.ptx
 Comment: 
 
-Filename: .gitignore
+Filename: README.md
 Comment: 
 
 Filename: assets/jsxgraph/
 Comment: 
 
 Filename: assets/frog.jpg
 Comment: 
 
 Filename: assets/jsxgraph/infinity.js
 Comment: 
 
-Filename: .devcontainer/devcontainer.json
-Comment: 
-
 Filename: publication/publication.ptx
 Comment: 
 
 Filename: source/images/
 Comment: 
 
-Filename: source/sec-first-intro.ptx
+Filename: source/sec-features.ptx
 Comment: 
 
-Filename: source/main.ptx
+Filename: source/fig-sage3d.ptx
 Comment: 
 
-Filename: source/sec-first-examples.ptx
+Filename: source/frontmatter.ptx
 Comment: 
 
-Filename: source/fig-sage2d.ptx
+Filename: source/ex-first.ptx
 Comment: 
 
-Filename: source/fig-tikz.ptx
+Filename: source/ch-first with spaces.ptx
 Comment: 
 
-Filename: source/fig-sage3d.ptx
+Filename: source/main.ptx
 Comment: 
 
-Filename: source/fig-asymptote.ptx
+Filename: source/ch-generate.ptx
 Comment: 
 
-Filename: source/frontmatter.ptx
+Filename: source/backmatter.ptx
 Comment: 
 
-Filename: source/ch-features.ptx
+Filename: source/fig-sage2d.ptx
 Comment: 
 
-Filename: source/ch-generate.ptx
+Filename: source/sec-first-examples.ptx
 Comment: 
 
-Filename: source/sec-features.ptx
+Filename: source/sec-first-intro.ptx
 Comment: 
 
-Filename: source/backmatter.ptx
+Filename: source/ch-features.ptx
 Comment: 
 
-Filename: source/ch-first with spaces.ptx
+Filename: source/fig-asymptote.ptx
 Comment: 
 
-Filename: source/ch-empty.ptx
+Filename: source/fig-tikz.ptx
 Comment: 
 
-Filename: source/ex-first.ptx
+Filename: source/ch-empty.ptx
 Comment: 
 
 Filename: source/docinfo.ptx
 Comment: 
 
 Filename: source/images/sageplot2d.sage
 Comment: 
 
-Filename: source/images/cflag.asy
-Comment: 
-
 Filename: source/images/tikz.tex
 Comment: 
 
 Filename: source/images/sageplot3d.sage
 Comment: 
 
+Filename: source/images/cflag.asy
+Comment: 
+
+Filename: .devcontainer/devcontainer.json
+Comment: 
+
 Zip file comment:
```

### Comparing `pretext-1.5.4.dev20230601/pretext/templates/resources/devcontainer.json` & `pretext-1.5.4.dev20230602/pretext/templates/resources/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230601/pretext/templates/resources/hello.zip` & `pretext-1.5.4.dev20230602/pretext/templates/resources/hello.zip`

 * *Files 11% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 4611 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 06:19 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 06:19 source/
--rw-r--r--  2.0 unx       69 b- defN 23-Jun-01 06:19 README.md
--rw-r--r--  2.0 unx     1217 b- defN 23-Jun-01 06:19 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-01 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-01 06:19 .gitignore
--rw-r--r--  2.0 unx     2059 b- defN 23-Jun-01 06:19 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      242 b- defN 23-Jun-01 06:19 publication/publication.ptx
--rw-r--r--  2.0 unx      156 b- defN 23-Jun-01 06:19 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 06:18 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 06:18 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 06:18 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-02 06:18 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-02 06:18 codechat_config.yaml
+-rw-r--r--  2.0 unx     1217 b- defN 23-Jun-02 06:18 project.ptx
+-rw-r--r--  2.0 unx       69 b- defN 23-Jun-02 06:18 README.md
+-rw-r--r--  2.0 unx      242 b- defN 23-Jun-02 06:18 publication/publication.ptx
+-rw-r--r--  2.0 unx      156 b- defN 23-Jun-02 06:18 source/main.ptx
+-rw-r--r--  2.0 unx     2059 b- defN 23-Jun-02 06:18 .devcontainer/devcontainer.json
 10 files, 7687 bytes uncompressed, 3517 bytes compressed:  54.2%
```

#### zipnote {}

```diff
@@ -3,29 +3,29 @@
 
 Filename: publication/
 Comment: 
 
 Filename: source/
 Comment: 
 
-Filename: README.md
-Comment: 
-
-Filename: project.ptx
+Filename: .gitignore
 Comment: 
 
 Filename: codechat_config.yaml
 Comment: 
 
-Filename: .gitignore
+Filename: project.ptx
 Comment: 
 
-Filename: .devcontainer/devcontainer.json
+Filename: README.md
 Comment: 
 
 Filename: publication/publication.ptx
 Comment: 
 
 Filename: source/main.ptx
 Comment: 
 
+Filename: .devcontainer/devcontainer.json
+Comment: 
+
 Zip file comment:
```

### Comparing `pretext-1.5.4.dev20230601/pretext/templates/resources/project.ptx` & `pretext-1.5.4.dev20230602/pretext/templates/resources/project.ptx`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230601/pretext/templates/resources/slideshow.zip` & `pretext-1.5.4.dev20230602/pretext/templates/resources/slideshow.zip`

 * *Files 8% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 8346 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 06:19 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 06:19 source/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 06:19 xsl/
--rw-r--r--  2.0 unx      784 b- defN 23-Jun-01 06:19 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-01 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-01 06:19 .gitignore
--rw-r--r--  2.0 unx     2059 b- defN 23-Jun-01 06:19 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      190 b- defN 23-Jun-01 06:19 xsl/slides.xsl
--rw-r--r--  2.0 unx     2097 b- defN 23-Jun-01 06:19 publication/publication.ptx
--rw-r--r--  2.0 unx    11200 b- defN 23-Jun-01 06:19 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 06:18 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 06:18 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 06:18 source/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 06:18 xsl/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-02 06:18 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-02 06:18 codechat_config.yaml
+-rw-r--r--  2.0 unx      784 b- defN 23-Jun-02 06:18 project.ptx
+-rw-r--r--  2.0 unx      190 b- defN 23-Jun-02 06:18 xsl/slides.xsl
+-rw-r--r--  2.0 unx     2097 b- defN 23-Jun-02 06:18 publication/publication.ptx
+-rw-r--r--  2.0 unx    11200 b- defN 23-Jun-02 06:18 source/main.ptx
+-rw-r--r--  2.0 unx     2059 b- defN 23-Jun-02 06:18 .devcontainer/devcontainer.json
 11 files, 20274 bytes uncompressed, 7158 bytes compressed:  64.7%
```

#### zipnote {}

```diff
@@ -6,29 +6,29 @@
 
 Filename: source/
 Comment: 
 
 Filename: xsl/
 Comment: 
 
-Filename: project.ptx
+Filename: .gitignore
 Comment: 
 
 Filename: codechat_config.yaml
 Comment: 
 
-Filename: .gitignore
-Comment: 
-
-Filename: .devcontainer/devcontainer.json
+Filename: project.ptx
 Comment: 
 
 Filename: xsl/slides.xsl
 Comment: 
 
 Filename: publication/publication.ptx
 Comment: 
 
 Filename: source/main.ptx
 Comment: 
 
+Filename: .devcontainer/devcontainer.json
+Comment: 
+
 Zip file comment:
```

### Comparing `pretext-1.5.4.dev20230601/pretext/utils.py` & `pretext-1.5.4.dev20230602/pretext/utils.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230601/pyproject.toml` & `pretext-1.5.4.dev20230602/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pretext"
-version = "1.5.4.dev20230601"
+version = "1.5.4.dev20230602"
 description = "A package to author, build, and deploy PreTeXt projects."
 readme = "README.md"
 homepage = "https://pretextbook.org"
 repository = "https://github.com/PreTeXtBook/pretext-cli"
 authors = ["Oscar Levin <oscar.levin@unco.edu>", "Steven Clontz <steven.clontz@gmail.com>",]
 license = "GPL-3.0-or-later"
 include = [
```

### Comparing `pretext-1.5.4.dev20230601/PKG-INFO` & `pretext-1.5.4.dev20230602/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretext
-Version: 1.5.4.dev20230601
+Version: 1.5.4.dev20230602
 Summary: A package to author, build, and deploy PreTeXt projects.
 Home-page: https://pretextbook.org
 License: GPL-3.0-or-later
 Author: Oscar Levin
 Author-email: oscar.levin@unco.edu
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

