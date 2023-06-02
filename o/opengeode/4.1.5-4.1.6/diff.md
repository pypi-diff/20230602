# Comparing `tmp/opengeode-4.1.5.tar.gz` & `tmp/opengeode-4.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opengeode-4.1.5.tar", last modified: Thu May 25 08:53:30 2023, max compression
+gzip compressed data, was "opengeode-4.1.6.tar", last modified: Fri Jun  2 09:04:34 2023, max compression
```

## Comparing `opengeode-4.1.5.tar` & `opengeode-4.1.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 taste     (1001) taste     (1001)        0 2023-05-25 08:53:30.980527 opengeode-4.1.5/
--rw-r--r--   0 taste     (1001) taste     (1001)     4673 2022-05-15 08:02:36.000000 opengeode-4.1.5/FONT-LICENCE.txt
--rw-r--r--   0 taste     (1001) taste     (1001)     7651 2022-05-15 08:02:36.000000 opengeode-4.1.5/LICENSE
--rw-r--r--   0 taste     (1001) taste     (1001)       54 2022-05-15 08:02:36.000000 opengeode-4.1.5/MANIFEST.in
--rw-r--r--   0 taste     (1001) taste     (1001)    44280 2023-05-25 08:53:30.980527 opengeode-4.1.5/PKG-INFO
--rw-r--r--   0 taste     (1001) taste     (1001)    34681 2023-05-25 08:53:21.000000 opengeode-4.1.5/README.md
-drwxr-xr-x   0 taste     (1001) taste     (1001)        0 2023-05-25 08:53:30.980527 opengeode-4.1.5/opengeode/
--rw-r--r--   0 taste     (1001) taste     (1001)   158021 2023-05-25 08:53:21.000000 opengeode-4.1.5/opengeode/AdaGenerator.py
--rwxr-xr-x   0 taste     (1001) taste     (1001)    13961 2023-05-25 08:53:21.000000 opengeode-4.1.5/opengeode/Asn1scc.py
--rw-r--r--   0 taste     (1001) taste     (1001)   116013 2022-11-13 15:59:02.000000 opengeode-4.1.5/opengeode/CGenerator.py
--rw-r--r--   0 taste     (1001) taste     (1001)    11750 2023-05-09 20:41:05.000000 opengeode-4.1.5/opengeode/Clipboard.py
--rw-r--r--   0 taste     (1001) taste     (1001)    29689 2022-12-08 11:28:57.000000 opengeode-4.1.5/opengeode/Connectors.py
--rw-r--r--   0 taste     (1001) taste     (1001)    38556 2023-05-25 08:53:21.000000 opengeode-4.1.5/opengeode/Helper.py
--rw-r--r--   0 taste     (1001) taste     (1001)    12719 2023-04-14 16:02:15.000000 opengeode-4.1.5/opengeode/Lander.py
--rw-r--r--   0 taste     (1001) taste     (1001)    82924 2023-01-22 14:09:04.000000 opengeode-4.1.5/opengeode/LlvmGenerator.py
--rw-r--r--   0 taste     (1001) taste     (1001)    18655 2023-05-10 20:42:44.000000 opengeode-4.1.5/opengeode/Pr.py
--rw-r--r--   0 taste     (1001) taste     (1001)     2462 2022-05-15 08:02:36.000000 opengeode-4.1.5/opengeode/QGenSDL.py
--rw-r--r--   0 taste     (1001) taste     (1001)    15873 2023-01-03 10:27:29.000000 opengeode-4.1.5/opengeode/Renderer.py
--rw-r--r--   0 taste     (1001) taste     (1001)    36467 2022-08-25 09:25:42.000000 opengeode-4.1.5/opengeode/Statechart.py
--rw-r--r--   0 taste     (1001) taste     (1001)    73348 2022-07-25 21:01:25.000000 opengeode-4.1.5/opengeode/StgBackend.py
--rw-r--r--   0 taste     (1001) taste     (1001)    18658 2022-11-04 15:55:28.000000 opengeode-4.1.5/opengeode/TextInteraction.py
--rw-r--r--   0 taste     (1001) taste     (1001)     1058 2022-05-15 08:02:36.000000 opengeode-4.1.5/opengeode/__init__.py
--rw-r--r--   0 taste     (1001) taste     (1001)    57607 2023-05-10 20:42:44.000000 opengeode-4.1.5/opengeode/genericSymbols.py
--rw-r--r--   0 taste     (1001) taste     (1001) 21475752 2023-02-01 06:37:57.000000 opengeode-4.1.5/opengeode/icons.py
--rw-r--r--   0 taste     (1001) taste     (1001)    45021 2023-05-25 08:53:21.000000 opengeode-4.1.5/opengeode/ogAST.py
--rw-r--r--   0 taste     (1001) taste     (1001)     9297 2023-05-25 08:53:21.000000 opengeode-4.1.5/opengeode/ogASTDumper.py
--rw-r--r--   0 taste     (1001) taste     (1001)   340546 2023-05-25 08:53:21.000000 opengeode-4.1.5/opengeode/ogParser.py
--rw-r--r--   0 taste     (1001) taste     (1001)   160565 2023-05-25 08:53:21.000000 opengeode-4.1.5/opengeode/opengeode.py
--rw-r--r--   0 taste     (1001) taste     (1001)   183270 2023-05-10 20:42:44.000000 opengeode-4.1.5/opengeode/sdl92Lexer.py
--rw-r--r--   0 taste     (1001) taste     (1001)  4922318 2023-05-10 20:42:44.000000 opengeode-4.1.5/opengeode/sdl92Parser.py
--rw-r--r--   0 taste     (1001) taste     (1001)     2077 2022-10-06 09:09:20.000000 opengeode-4.1.5/opengeode/sdlHelp.py
--rw-r--r--   0 taste     (1001) taste     (1001)    64900 2023-05-10 20:42:44.000000 opengeode-4.1.5/opengeode/sdlSymbols.py
--rw-r--r--   0 taste     (1001) taste     (1001)     9445 2022-07-25 21:01:25.000000 opengeode-4.1.5/opengeode/undoCommands.py
--rw-r--r--   0 taste     (1001) taste     (1001)      358 2023-05-25 08:53:21.000000 opengeode-4.1.5/opengeode/version.py
-drwxr-xr-x   0 taste     (1001) taste     (1001)        0 2023-05-25 08:53:30.980527 opengeode-4.1.5/opengeode.egg-info/
--rw-r--r--   0 taste     (1001) taste     (1001)    44280 2023-05-25 08:53:30.000000 opengeode-4.1.5/opengeode.egg-info/PKG-INFO
--rw-r--r--   0 taste     (1001) taste     (1001)      843 2023-05-25 08:53:30.000000 opengeode-4.1.5/opengeode.egg-info/SOURCES.txt
--rw-r--r--   0 taste     (1001) taste     (1001)        1 2023-05-25 08:53:30.000000 opengeode-4.1.5/opengeode.egg-info/dependency_links.txt
--rw-r--r--   0 taste     (1001) taste     (1001)       61 2023-05-25 08:53:30.000000 opengeode-4.1.5/opengeode.egg-info/entry_points.txt
--rw-r--r--   0 taste     (1001) taste     (1001)       10 2023-05-25 08:53:30.000000 opengeode-4.1.5/opengeode.egg-info/top_level.txt
--rw-r--r--   0 taste     (1001) taste     (1001)       38 2023-05-25 08:53:30.980527 opengeode-4.1.5/setup.cfg
--rwxr-xr-x   0 taste     (1001) taste     (1001)     1220 2023-01-22 14:13:21.000000 opengeode-4.1.5/setup.py
+drwxr-xr-x   0 taste     (1001) taste     (1001)        0 2023-06-02 09:04:34.401009 opengeode-4.1.6/
+-rw-r--r--   0 taste     (1001) taste     (1001)     4673 2022-05-15 08:02:36.000000 opengeode-4.1.6/FONT-LICENCE.txt
+-rw-r--r--   0 taste     (1001) taste     (1001)     7651 2022-05-15 08:02:36.000000 opengeode-4.1.6/LICENSE
+-rw-r--r--   0 taste     (1001) taste     (1001)       54 2022-05-15 08:02:36.000000 opengeode-4.1.6/MANIFEST.in
+-rw-r--r--   0 taste     (1001) taste     (1001)    44405 2023-06-02 09:04:34.401009 opengeode-4.1.6/PKG-INFO
+-rw-r--r--   0 taste     (1001) taste     (1001)    34782 2023-06-02 09:04:15.000000 opengeode-4.1.6/README.md
+drwxr-xr-x   0 taste     (1001) taste     (1001)        0 2023-06-02 09:04:34.401009 opengeode-4.1.6/opengeode/
+-rw-r--r--   0 taste     (1001) taste     (1001)   158021 2023-05-25 08:53:21.000000 opengeode-4.1.6/opengeode/AdaGenerator.py
+-rwxr-xr-x   0 taste     (1001) taste     (1001)    13961 2023-05-25 08:53:21.000000 opengeode-4.1.6/opengeode/Asn1scc.py
+-rw-r--r--   0 taste     (1001) taste     (1001)   116013 2022-11-13 15:59:02.000000 opengeode-4.1.6/opengeode/CGenerator.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    11750 2023-05-09 20:41:05.000000 opengeode-4.1.6/opengeode/Clipboard.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    29689 2022-12-08 11:28:57.000000 opengeode-4.1.6/opengeode/Connectors.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    38556 2023-05-25 08:53:21.000000 opengeode-4.1.6/opengeode/Helper.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    12719 2023-04-14 16:02:15.000000 opengeode-4.1.6/opengeode/Lander.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    82924 2023-01-22 14:09:04.000000 opengeode-4.1.6/opengeode/LlvmGenerator.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    18655 2023-05-10 20:42:44.000000 opengeode-4.1.6/opengeode/Pr.py
+-rw-r--r--   0 taste     (1001) taste     (1001)     2462 2022-05-15 08:02:36.000000 opengeode-4.1.6/opengeode/QGenSDL.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    15873 2023-01-03 10:27:29.000000 opengeode-4.1.6/opengeode/Renderer.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    36467 2022-08-25 09:25:42.000000 opengeode-4.1.6/opengeode/Statechart.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    73348 2022-07-25 21:01:25.000000 opengeode-4.1.6/opengeode/StgBackend.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    18658 2022-11-04 15:55:28.000000 opengeode-4.1.6/opengeode/TextInteraction.py
+-rw-r--r--   0 taste     (1001) taste     (1001)     1058 2022-05-15 08:02:36.000000 opengeode-4.1.6/opengeode/__init__.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    57607 2023-05-10 20:42:44.000000 opengeode-4.1.6/opengeode/genericSymbols.py
+-rw-r--r--   0 taste     (1001) taste     (1001) 21475752 2023-02-01 06:37:57.000000 opengeode-4.1.6/opengeode/icons.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    45021 2023-05-25 08:53:21.000000 opengeode-4.1.6/opengeode/ogAST.py
+-rw-r--r--   0 taste     (1001) taste     (1001)     9297 2023-05-25 08:53:21.000000 opengeode-4.1.6/opengeode/ogASTDumper.py
+-rw-r--r--   0 taste     (1001) taste     (1001)   340998 2023-06-02 09:04:15.000000 opengeode-4.1.6/opengeode/ogParser.py
+-rw-r--r--   0 taste     (1001) taste     (1001)   160565 2023-05-25 08:53:21.000000 opengeode-4.1.6/opengeode/opengeode.py
+-rw-r--r--   0 taste     (1001) taste     (1001)   183270 2023-05-10 20:42:44.000000 opengeode-4.1.6/opengeode/sdl92Lexer.py
+-rw-r--r--   0 taste     (1001) taste     (1001)  4922318 2023-05-10 20:42:44.000000 opengeode-4.1.6/opengeode/sdl92Parser.py
+-rw-r--r--   0 taste     (1001) taste     (1001)     2077 2022-10-06 09:09:20.000000 opengeode-4.1.6/opengeode/sdlHelp.py
+-rw-r--r--   0 taste     (1001) taste     (1001)    64900 2023-05-10 20:42:44.000000 opengeode-4.1.6/opengeode/sdlSymbols.py
+-rw-r--r--   0 taste     (1001) taste     (1001)     9445 2022-07-25 21:01:25.000000 opengeode-4.1.6/opengeode/undoCommands.py
+-rw-r--r--   0 taste     (1001) taste     (1001)      358 2023-06-02 09:04:15.000000 opengeode-4.1.6/opengeode/version.py
+drwxr-xr-x   0 taste     (1001) taste     (1001)        0 2023-06-02 09:04:34.401009 opengeode-4.1.6/opengeode.egg-info/
+-rw-r--r--   0 taste     (1001) taste     (1001)    44405 2023-06-02 09:04:34.000000 opengeode-4.1.6/opengeode.egg-info/PKG-INFO
+-rw-r--r--   0 taste     (1001) taste     (1001)      843 2023-06-02 09:04:34.000000 opengeode-4.1.6/opengeode.egg-info/SOURCES.txt
+-rw-r--r--   0 taste     (1001) taste     (1001)        1 2023-06-02 09:04:34.000000 opengeode-4.1.6/opengeode.egg-info/dependency_links.txt
+-rw-r--r--   0 taste     (1001) taste     (1001)       61 2023-06-02 09:04:34.000000 opengeode-4.1.6/opengeode.egg-info/entry_points.txt
+-rw-r--r--   0 taste     (1001) taste     (1001)       10 2023-06-02 09:04:34.000000 opengeode-4.1.6/opengeode.egg-info/top_level.txt
+-rw-r--r--   0 taste     (1001) taste     (1001)       38 2023-06-02 09:04:34.401009 opengeode-4.1.6/setup.cfg
+-rwxr-xr-x   0 taste     (1001) taste     (1001)     1220 2023-01-22 14:13:21.000000 opengeode-4.1.6/setup.py
```

### Comparing `opengeode-4.1.5/FONT-LICENCE.txt` & `opengeode-4.1.6/FONT-LICENCE.txt`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.5/LICENSE` & `opengeode-4.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.5/PKG-INFO` & `opengeode-4.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengeode
-Version: 4.1.5
+Version: 4.1.6
 Summary: A free SDL editor for TASTE
 Home-page: http://opengeode.net
 Author: Maxime Perrotin
 Author-email: maxime.perrotin@esa.int
 License: UNKNOWN
 Description: ![OpenGEODE Logo](icons/opengeode4.png)
         
@@ -129,14 +129,17 @@
         There is no runtime, and the generated code is not subject to any license.
         
         The fonts are the fonts from Ubuntu, check licence in file [FONT-LICENSE.TXT](https://github.com/esa/opengeode/blob/master/FONT-LICENCE.txt)
         The background pattern was downloaded from www.subtlepatterns.com
         
         Changelog
         =========
+        **4.1.6 (05/2023)**
+        - Fix more issues with  computation of modulo operator range (negative numbers)
+        
         **4.1.5 (05/2023)**
         - Fix computation of modulo operator range
         
         **4.1.4 (05/2023)**
         - Fix support for built-in operators (Val, To_Enum, etc) / Ada backend
         
         **4.1.3 (05/2023)**
```

### Comparing `opengeode-4.1.5/README.md` & `opengeode-4.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -121,14 +121,17 @@
 There is no runtime, and the generated code is not subject to any license.
 
 The fonts are the fonts from Ubuntu, check licence in file [FONT-LICENSE.TXT](https://github.com/esa/opengeode/blob/master/FONT-LICENCE.txt)
 The background pattern was downloaded from www.subtlepatterns.com
 
 Changelog
 =========
+**4.1.6 (05/2023)**
+- Fix more issues with  computation of modulo operator range (negative numbers)
+
 **4.1.5 (05/2023)**
 - Fix computation of modulo operator range
 
 **4.1.4 (05/2023)**
 - Fix support for built-in operators (Val, To_Enum, etc) / Ada backend
 
 **4.1.3 (05/2023)**
```

### Comparing `opengeode-4.1.5/opengeode/AdaGenerator.py` & `opengeode-4.1.6/opengeode/AdaGenerator.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.5/opengeode/Asn1scc.py` & `opengeode-4.1.6/opengeode/Asn1scc.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.5/opengeode/CGenerator.py` & `opengeode-4.1.6/opengeode/CGenerator.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.5/opengeode/Clipboard.py` & `opengeode-4.1.6/opengeode/Clipboard.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.5/opengeode/Connectors.py` & `opengeode-4.1.6/opengeode/Connectors.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.5/opengeode/Helper.py` & `opengeode-4.1.6/opengeode/Helper.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.5/opengeode/Lander.py` & `opengeode-4.1.6/opengeode/Lander.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.5/opengeode/LlvmGenerator.py` & `opengeode-4.1.6/opengeode/LlvmGenerator.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.5/opengeode/Pr.py` & `opengeode-4.1.6/opengeode/Pr.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.5/opengeode/QGenSDL.py` & `opengeode-4.1.6/opengeode/QGenSDL.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.5/opengeode/Renderer.py` & `opengeode-4.1.6/opengeode/Renderer.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.5/opengeode/Statechart.py` & `opengeode-4.1.6/opengeode/Statechart.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.5/opengeode/StgBackend.py` & `opengeode-4.1.6/opengeode/StgBackend.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.5/opengeode/TextInteraction.py` & `opengeode-4.1.6/opengeode/TextInteraction.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.5/opengeode/__init__.py` & `opengeode-4.1.6/opengeode/__init__.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.5/opengeode/genericSymbols.py` & `opengeode-4.1.6/opengeode/genericSymbols.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.5/opengeode/icons.py` & `opengeode-4.1.6/opengeode/icons.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.5/opengeode/ogAST.py` & `opengeode-4.1.6/opengeode/ogAST.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.5/opengeode/ogASTDumper.py` & `opengeode-4.1.6/opengeode/ogASTDumper.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.5/opengeode/ogParser.py` & `opengeode-4.1.6/opengeode/ogParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -2400,16 +2400,24 @@
                 msg = f'Modulo: range [{minR} .. {maxR}] allows division by zero'
                 errors.append(error(root, msg))
             else:
                 # no the following is wrong
                 #possible_values = [minL % minR, minL % maxR, maxL % minR, maxL % maxR]
                 #bounds["Min"] = min(possible_values)
                 #bounds["Max"] = max(possible_values)
-                bounds["Min"] = min([minL, minR - 1])
-                bounds["Max"] = min([maxL, maxR - 1])
+                if minL == maxL and minR == maxR:
+                    bounds["Min"] = bounds["Max"] = minL % minR
+                elif minL < 0 and minR > 0:
+                    # a bit tricky... but in minR is positive, result is always positive
+                    bounds["Min"] = 0
+                    # and e.g. -5 % 99 = 94 so  maxR + minL should be right
+                    bounds["Max"] = max([maxL, maxR + minL])
+                else:
+                    bounds["Min"] = min([minL, minR - 1])
+                    bounds["Max"] = min([maxL, maxR - 1])
         else:
             bounds = find_bounds(expr.op, minL, maxL, minR, maxR)
 
         if is_number(basic_right) or is_number(basic_left):
             is_signed = (not is_number(basic_right))   and minR < 0.0 \
                         or (not is_number(basic_left)) and minL < 0.0
```

### Comparing `opengeode-4.1.5/opengeode/opengeode.py` & `opengeode-4.1.6/opengeode/opengeode.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.5/opengeode/sdl92Lexer.py` & `opengeode-4.1.6/opengeode/sdl92Lexer.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.5/opengeode/sdl92Parser.py` & `opengeode-4.1.6/opengeode/sdl92Parser.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.5/opengeode/sdlHelp.py` & `opengeode-4.1.6/opengeode/sdlHelp.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.5/opengeode/sdlSymbols.py` & `opengeode-4.1.6/opengeode/sdlSymbols.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.5/opengeode/undoCommands.py` & `opengeode-4.1.6/opengeode/undoCommands.py`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.5/opengeode.egg-info/PKG-INFO` & `opengeode-4.1.6/opengeode.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengeode
-Version: 4.1.5
+Version: 4.1.6
 Summary: A free SDL editor for TASTE
 Home-page: http://opengeode.net
 Author: Maxime Perrotin
 Author-email: maxime.perrotin@esa.int
 License: UNKNOWN
 Description: ![OpenGEODE Logo](icons/opengeode4.png)
         
@@ -129,14 +129,17 @@
         There is no runtime, and the generated code is not subject to any license.
         
         The fonts are the fonts from Ubuntu, check licence in file [FONT-LICENSE.TXT](https://github.com/esa/opengeode/blob/master/FONT-LICENCE.txt)
         The background pattern was downloaded from www.subtlepatterns.com
         
         Changelog
         =========
+        **4.1.6 (05/2023)**
+        - Fix more issues with  computation of modulo operator range (negative numbers)
+        
         **4.1.5 (05/2023)**
         - Fix computation of modulo operator range
         
         **4.1.4 (05/2023)**
         - Fix support for built-in operators (Val, To_Enum, etc) / Ada backend
         
         **4.1.3 (05/2023)**
```

### Comparing `opengeode-4.1.5/opengeode.egg-info/SOURCES.txt` & `opengeode-4.1.6/opengeode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opengeode-4.1.5/setup.py` & `opengeode-4.1.6/setup.py`

 * *Files identical despite different names*

