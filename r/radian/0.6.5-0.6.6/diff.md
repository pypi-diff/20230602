# Comparing `tmp/radian-0.6.5.tar.gz` & `tmp/radian-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radian-0.6.5.tar", last modified: Wed Apr 12 16:36:27 2023, max compression
+gzip compressed data, was "radian-0.6.6.tar", last modified: Fri Jun  2 17:47:58 2023, max compression
```

## Comparing `radian-0.6.5.tar` & `radian-0.6.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:36:27.630395 radian-0.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-12 16:36:17.000000 radian-0.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 16:36:17.000000 radian-0.6.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-04-12 16:36:27.630395 radian-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10660 2023-04-12 16:36:17.000000 radian-0.6.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:36:27.630395 radian-0.6.5/radian/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-12 16:36:17.000000 radian-0.6.5/radian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-12 16:36:17.000000 radian-0.6.5/radian/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-04-12 16:36:17.000000 radian-0.6.5/radian/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-04-12 16:36:17.000000 radian-0.6.5/radian/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-04-12 16:36:17.000000 radian-0.6.5/radian/console.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-12 16:36:17.000000 radian-0.6.5/radian/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-12 16:36:17.000000 radian-0.6.5/radian/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 16:36:17.000000 radian-0.6.5/radian/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    15876 2023-04-12 16:36:17.000000 radian-0.6.5/radian/key_bindings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:36:27.630395 radian-0.6.5/radian/latex/
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-12 16:36:17.000000 radian-0.6.5/radian/latex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64127 2023-04-12 16:36:17.000000 radian-0.6.5/radian/latex/latex_symbols.py
--rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-04-12 16:36:17.000000 radian-0.6.5/radian/lexer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:36:27.630395 radian-0.6.5/radian/lineedit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:36:17.000000 radian-0.6.5/radian/lineedit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-04-12 16:36:17.000000 radian-0.6.5/radian/lineedit/buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-12 16:36:17.000000 radian-0.6.5/radian/lineedit/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-04-12 16:36:17.000000 radian-0.6.5/radian/lineedit/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-04-12 16:36:17.000000 radian-0.6.5/radian/prompt_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:36:27.630395 radian-0.6.5/radian/reticulate/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-12 16:36:17.000000 radian-0.6.5/radian/reticulate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-12 16:36:17.000000 radian-0.6.5/radian/reticulate/config.R
--rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-04-12 16:36:17.000000 radian-0.6.5/radian/reticulate/key_bindings.R
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-12 16:36:17.000000 radian-0.6.5/radian/rutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-12 16:36:17.000000 radian-0.6.5/radian/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-12 16:36:17.000000 radian-0.6.5/radian/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:36:27.630395 radian-0.6.5/radian.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-04-12 16:36:27.000000 radian-0.6.5/radian.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-12 16:36:27.000000 radian-0.6.5/radian.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:36:27.000000 radian-0.6.5/radian.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-12 16:36:27.000000 radian-0.6.5/radian.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-12 16:36:27.000000 radian-0.6.5/radian.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 16:36:27.000000 radian-0.6.5/radian.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-12 16:36:27.630395 radian-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-12 16:36:17.000000 radian-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:47:58.437547 radian-0.6.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-02 17:47:49.000000 radian-0.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-02 17:47:49.000000 radian-0.6.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13395 2023-06-02 17:47:58.437547 radian-0.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-06-02 17:47:49.000000 radian-0.6.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:47:58.437547 radian-0.6.6/radian/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-02 17:47:49.000000 radian-0.6.6/radian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-02 17:47:49.000000 radian-0.6.6/radian/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-06-02 17:47:49.000000 radian-0.6.6/radian/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-06-02 17:47:49.000000 radian-0.6.6/radian/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-06-02 17:47:49.000000 radian-0.6.6/radian/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-02 17:47:49.000000 radian-0.6.6/radian/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-02 17:47:49.000000 radian-0.6.6/radian/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-02 17:47:49.000000 radian-0.6.6/radian/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15876 2023-06-02 17:47:49.000000 radian-0.6.6/radian/key_bindings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:47:58.437547 radian-0.6.6/radian/latex/
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-02 17:47:49.000000 radian-0.6.6/radian/latex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64127 2023-06-02 17:47:49.000000 radian-0.6.6/radian/latex/latex_symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-06-02 17:47:49.000000 radian-0.6.6/radian/lexer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:47:58.437547 radian-0.6.6/radian/lineedit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:47:49.000000 radian-0.6.6/radian/lineedit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-06-02 17:47:49.000000 radian-0.6.6/radian/lineedit/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-06-02 17:47:49.000000 radian-0.6.6/radian/lineedit/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-06-02 17:47:49.000000 radian-0.6.6/radian/lineedit/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-06-02 17:47:49.000000 radian-0.6.6/radian/prompt_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:47:58.437547 radian-0.6.6/radian/reticulate/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-02 17:47:49.000000 radian-0.6.6/radian/reticulate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-02 17:47:49.000000 radian-0.6.6/radian/reticulate/config.R
+-rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-06-02 17:47:49.000000 radian-0.6.6/radian/reticulate/key_bindings.R
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-06-02 17:47:49.000000 radian-0.6.6/radian/rutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-02 17:47:49.000000 radian-0.6.6/radian/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-02 17:47:49.000000 radian-0.6.6/radian/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:47:58.437547 radian-0.6.6/radian.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13395 2023-06-02 17:47:58.000000 radian-0.6.6/radian.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-02 17:47:58.000000 radian-0.6.6/radian.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 17:47:58.000000 radian-0.6.6/radian.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-02 17:47:58.000000 radian-0.6.6/radian.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-02 17:47:58.000000 radian-0.6.6/radian.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-02 17:47:58.000000 radian-0.6.6/radian.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-02 17:47:58.437547 radian-0.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-02 17:47:49.000000 radian-0.6.6/setup.py
```

### Comparing `radian-0.6.5/LICENSE` & `radian-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `radian-0.6.5/PKG-INFO` & `radian-0.6.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radian
-Version: 0.6.5
+Version: 0.6.6
 Summary: A 21 century R console
 Home-page: https://github.com/randy3k/radian
 Author: Randy Lai
 License: UNKNOWN
 Description: # radian: A 21 century R console
         
         [![Main](https://github.com/randy3k/radian/actions/workflows/main.yml/badge.svg)](https://github.com/randy3k/radian/actions/workflows/main.yml)
@@ -242,14 +242,16 @@
         _radian_ maintains its own history file `.radian_history` and doesn't use the `.Rhistory` file. A local `.radian_history` is used if it is found in the launch directory. Otherwise, the global history file `~/.radian_history` would be used. To override the default behavior, you could launch _radian_ with the options: `radian --local-history`, `radian --global-history` or `radian --no-history`.
         
         
         #### Does it slow down my R program?
         
         _radian_ only provides a frontend to the R program, the actual running eventloop is the same as that of the traditional R console. There is no performance sacrifice (or gain) while using this modern command line interface. 
         
+        However, it was reported that radian may be slower when using parallel computation, specifially when using forking. User should take extra care in those cases.
+        
         #### Nvim-R support
         
         Put
         ```vim
         let R_app = "radian"
         let R_cmd = "R"
         let R_hl_term = 0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: radian Version: 0.6.5 Summary: A 21 century R
+Metadata-Version: 2.1 Name: radian Version: 0.6.6 Summary: A 21 century R
 console Home-page: https://github.com/randy3k/radian Author: Randy Lai License:
 UNKNOWN Description: # radian: A 21 century R console [![Main](https://
 github.com/randy3k/radian/actions/workflows/main.yml/badge.svg)](https://
 github.com/randy3k/radian/actions/workflows/main.yml) [![codecov](https://
 codecov.io/gh/randy3k/radian/branch/master/graph/badge.svg)](https://
 codecov.io/gh/randy3k/radian) [![](https://img.shields.io/pypi/v/radian.svg)]
 (https://pypi.org/project/radian/) [![Conda version](https://img.shields.io/
@@ -121,22 +121,24 @@
 is found in the launch directory. Otherwise, the global history file
 `~/.radian_history` would be used. To override the default behavior, you could
 launch _radian_ with the options: `radian --local-history`, `radian --global-
 history` or `radian --no-history`. #### Does it slow down my R program?
 _radian_ only provides a frontend to the R program, the actual running
 eventloop is the same as that of the traditional R console. There is no
 performance sacrifice (or gain) while using this modern command line interface.
-#### Nvim-R support Put ```vim let R_app = "radian" let R_cmd = "R" let
-R_hl_term = 0 let R_args = [] " if you had set any let R_bracketed_paste = 1
-``` in your vim config. #### `reticulate` Auto Completions To enable reticulate
-prompt completions, make sure that `jedi` is installed. ```sh pip install jedi
-``` Alternatively, if you use conda, ```sh conda install -c conda-forge jedi
-``` #### Prompt not shown inside a docker container It maybe caused by the
-invalid terminal size, try running `stty size` in your terminal to see if it
-returns a correct size. You could change the values of it from the
-environmental variables `$COLUMNS` and `$LINES` when you log-in the docker
-container. ``` docker exec -it  bash -c "stty cols $COLUMNS rows $LINES &&
-bash" ``` ## Why called _radian_? _radian_ is powered by (Ï)thon. ## Credits
-_radian_ wouldn't be possible without the creative work [prompt_toolkit](https:
-//github.com/jonathanslenders/python-prompt-toolkit/) by Jonathan Slenders.
-Platform: UNKNOWN Requires-Python: >=3.6 Description-Content-Type: text/
-markdown Provides-Extra: test
+However, it was reported that radian may be slower when using parallel
+computation, specifially when using forking. User should take extra care in
+those cases. #### Nvim-R support Put ```vim let R_app = "radian" let R_cmd =
+"R" let R_hl_term = 0 let R_args = [] " if you had set any let
+R_bracketed_paste = 1 ``` in your vim config. #### `reticulate` Auto
+Completions To enable reticulate prompt completions, make sure that `jedi` is
+installed. ```sh pip install jedi ``` Alternatively, if you use conda, ```sh
+conda install -c conda-forge jedi ``` #### Prompt not shown inside a docker
+container It maybe caused by the invalid terminal size, try running `stty size`
+in your terminal to see if it returns a correct size. You could change the
+values of it from the environmental variables `$COLUMNS` and `$LINES` when you
+log-in the docker container. ``` docker exec -it  bash -c "stty cols $COLUMNS
+rows $LINES && bash" ``` ## Why called _radian_? _radian_ is powered by
+(Ï)thon. ## Credits _radian_ wouldn't be possible without the creative work
+[prompt_toolkit](https://github.com/jonathanslenders/python-prompt-toolkit/) by
+Jonathan Slenders. Platform: UNKNOWN Requires-Python: >=3.6 Description-
+Content-Type: text/markdown Provides-Extra: test
```

### Comparing `radian-0.6.5/README.md` & `radian-0.6.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -235,14 +235,16 @@
 _radian_ maintains its own history file `.radian_history` and doesn't use the `.Rhistory` file. A local `.radian_history` is used if it is found in the launch directory. Otherwise, the global history file `~/.radian_history` would be used. To override the default behavior, you could launch _radian_ with the options: `radian --local-history`, `radian --global-history` or `radian --no-history`.
 
 
 #### Does it slow down my R program?
 
 _radian_ only provides a frontend to the R program, the actual running eventloop is the same as that of the traditional R console. There is no performance sacrifice (or gain) while using this modern command line interface. 
 
+However, it was reported that radian may be slower when using parallel computation, specifially when using forking. User should take extra care in those cases.
+
 #### Nvim-R support
 
 Put
 ```vim
 let R_app = "radian"
 let R_cmd = "R"
 let R_hl_term = 0
```

#### html2text {}

```diff
@@ -119,20 +119,23 @@
 is found in the launch directory. Otherwise, the global history file
 `~/.radian_history` would be used. To override the default behavior, you could
 launch _radian_ with the options: `radian --local-history`, `radian --global-
 history` or `radian --no-history`. #### Does it slow down my R program?
 _radian_ only provides a frontend to the R program, the actual running
 eventloop is the same as that of the traditional R console. There is no
 performance sacrifice (or gain) while using this modern command line interface.
-#### Nvim-R support Put ```vim let R_app = "radian" let R_cmd = "R" let
-R_hl_term = 0 let R_args = [] " if you had set any let R_bracketed_paste = 1
-``` in your vim config. #### `reticulate` Auto Completions To enable reticulate
-prompt completions, make sure that `jedi` is installed. ```sh pip install jedi
-``` Alternatively, if you use conda, ```sh conda install -c conda-forge jedi
-``` #### Prompt not shown inside a docker container It maybe caused by the
-invalid terminal size, try running `stty size` in your terminal to see if it
-returns a correct size. You could change the values of it from the
-environmental variables `$COLUMNS` and `$LINES` when you log-in the docker
-container. ``` docker exec -it  bash -c "stty cols $COLUMNS rows $LINES &&
-bash" ``` ## Why called _radian_? _radian_ is powered by (Ï)thon. ## Credits
-_radian_ wouldn't be possible without the creative work [prompt_toolkit](https:
-//github.com/jonathanslenders/python-prompt-toolkit/) by Jonathan Slenders.
+However, it was reported that radian may be slower when using parallel
+computation, specifially when using forking. User should take extra care in
+those cases. #### Nvim-R support Put ```vim let R_app = "radian" let R_cmd =
+"R" let R_hl_term = 0 let R_args = [] " if you had set any let
+R_bracketed_paste = 1 ``` in your vim config. #### `reticulate` Auto
+Completions To enable reticulate prompt completions, make sure that `jedi` is
+installed. ```sh pip install jedi ``` Alternatively, if you use conda, ```sh
+conda install -c conda-forge jedi ``` #### Prompt not shown inside a docker
+container It maybe caused by the invalid terminal size, try running `stty size`
+in your terminal to see if it returns a correct size. You could change the
+values of it from the environmental variables `$COLUMNS` and `$LINES` when you
+log-in the docker container. ``` docker exec -it  bash -c "stty cols $COLUMNS
+rows $LINES && bash" ``` ## Why called _radian_? _radian_ is powered by
+(Ï)thon. ## Credits _radian_ wouldn't be possible without the creative work
+[prompt_toolkit](https://github.com/jonathanslenders/python-prompt-toolkit/) by
+Jonathan Slenders.
```

### Comparing `radian-0.6.5/radian/__main__.py` & `radian-0.6.6/radian/__main__.py`

 * *Files identical despite different names*

### Comparing `radian-0.6.5/radian/app.py` & `radian-0.6.6/radian/app.py`

 * *Files identical despite different names*

### Comparing `radian-0.6.5/radian/completion.py` & `radian-0.6.6/radian/completion.py`

 * *Files identical despite different names*

### Comparing `radian-0.6.5/radian/console.py` & `radian-0.6.6/radian/console.py`

 * *Files identical despite different names*

### Comparing `radian-0.6.5/radian/document.py` & `radian-0.6.6/radian/document.py`

 * *Files identical despite different names*

### Comparing `radian-0.6.5/radian/io.py` & `radian-0.6.6/radian/io.py`

 * *Files identical despite different names*

### Comparing `radian-0.6.5/radian/key_bindings.py` & `radian-0.6.6/radian/key_bindings.py`

 * *Files identical despite different names*

### Comparing `radian-0.6.5/radian/latex/__init__.py` & `radian-0.6.6/radian/latex/__init__.py`

 * *Files identical despite different names*

### Comparing `radian-0.6.5/radian/latex/latex_symbols.py` & `radian-0.6.6/radian/latex/latex_symbols.py`

 * *Files identical despite different names*

### Comparing `radian-0.6.5/radian/lexer.py` & `radian-0.6.6/radian/lexer.py`

 * *Files identical despite different names*

### Comparing `radian-0.6.5/radian/lineedit/buffer.py` & `radian-0.6.6/radian/lineedit/buffer.py`

 * *Files identical despite different names*

### Comparing `radian-0.6.5/radian/lineedit/history.py` & `radian-0.6.6/radian/lineedit/history.py`

 * *Files identical despite different names*

### Comparing `radian-0.6.5/radian/lineedit/prompt.py` & `radian-0.6.6/radian/lineedit/prompt.py`

 * *Files identical despite different names*

### Comparing `radian-0.6.5/radian/prompt_session.py` & `radian-0.6.6/radian/prompt_session.py`

 * *Files identical despite different names*

### Comparing `radian-0.6.5/radian/reticulate/__init__.py` & `radian-0.6.6/radian/reticulate/__init__.py`

 * *Files identical despite different names*

### Comparing `radian-0.6.5/radian/reticulate/config.R` & `radian-0.6.6/radian/reticulate/config.R`

 * *Files identical despite different names*

### Comparing `radian-0.6.5/radian/reticulate/key_bindings.R` & `radian-0.6.6/radian/reticulate/key_bindings.R`

 * *Files identical despite different names*

### Comparing `radian-0.6.5/radian/rutils.py` & `radian-0.6.6/radian/rutils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import os
 import sys
 from rchitect import rcopy, reval, rcall
 from rchitect.interface import roption
 from .key_bindings import map_key
 
+def is_ascii(str):
+    return all(ord(c) < 128 for c in str)
 
 def is_long_non_ascii_multiline(text):
-    if text.isascii():
+    if is_ascii(text):
         return False
     if "\n" not in text:
         return False
     if len(text) < 1000:
         return False
     return True
```

### Comparing `radian-0.6.5/radian/settings.py` & `radian-0.6.6/radian/settings.py`

 * *Files identical despite different names*

### Comparing `radian-0.6.5/radian/shell.py` & `radian-0.6.6/radian/shell.py`

 * *Files identical despite different names*

### Comparing `radian-0.6.5/radian.egg-info/PKG-INFO` & `radian-0.6.6/radian.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radian
-Version: 0.6.5
+Version: 0.6.6
 Summary: A 21 century R console
 Home-page: https://github.com/randy3k/radian
 Author: Randy Lai
 License: UNKNOWN
 Description: # radian: A 21 century R console
         
         [![Main](https://github.com/randy3k/radian/actions/workflows/main.yml/badge.svg)](https://github.com/randy3k/radian/actions/workflows/main.yml)
@@ -242,14 +242,16 @@
         _radian_ maintains its own history file `.radian_history` and doesn't use the `.Rhistory` file. A local `.radian_history` is used if it is found in the launch directory. Otherwise, the global history file `~/.radian_history` would be used. To override the default behavior, you could launch _radian_ with the options: `radian --local-history`, `radian --global-history` or `radian --no-history`.
         
         
         #### Does it slow down my R program?
         
         _radian_ only provides a frontend to the R program, the actual running eventloop is the same as that of the traditional R console. There is no performance sacrifice (or gain) while using this modern command line interface. 
         
+        However, it was reported that radian may be slower when using parallel computation, specifially when using forking. User should take extra care in those cases.
+        
         #### Nvim-R support
         
         Put
         ```vim
         let R_app = "radian"
         let R_cmd = "R"
         let R_hl_term = 0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: radian Version: 0.6.5 Summary: A 21 century R
+Metadata-Version: 2.1 Name: radian Version: 0.6.6 Summary: A 21 century R
 console Home-page: https://github.com/randy3k/radian Author: Randy Lai License:
 UNKNOWN Description: # radian: A 21 century R console [![Main](https://
 github.com/randy3k/radian/actions/workflows/main.yml/badge.svg)](https://
 github.com/randy3k/radian/actions/workflows/main.yml) [![codecov](https://
 codecov.io/gh/randy3k/radian/branch/master/graph/badge.svg)](https://
 codecov.io/gh/randy3k/radian) [![](https://img.shields.io/pypi/v/radian.svg)]
 (https://pypi.org/project/radian/) [![Conda version](https://img.shields.io/
@@ -121,22 +121,24 @@
 is found in the launch directory. Otherwise, the global history file
 `~/.radian_history` would be used. To override the default behavior, you could
 launch _radian_ with the options: `radian --local-history`, `radian --global-
 history` or `radian --no-history`. #### Does it slow down my R program?
 _radian_ only provides a frontend to the R program, the actual running
 eventloop is the same as that of the traditional R console. There is no
 performance sacrifice (or gain) while using this modern command line interface.
-#### Nvim-R support Put ```vim let R_app = "radian" let R_cmd = "R" let
-R_hl_term = 0 let R_args = [] " if you had set any let R_bracketed_paste = 1
-``` in your vim config. #### `reticulate` Auto Completions To enable reticulate
-prompt completions, make sure that `jedi` is installed. ```sh pip install jedi
-``` Alternatively, if you use conda, ```sh conda install -c conda-forge jedi
-``` #### Prompt not shown inside a docker container It maybe caused by the
-invalid terminal size, try running `stty size` in your terminal to see if it
-returns a correct size. You could change the values of it from the
-environmental variables `$COLUMNS` and `$LINES` when you log-in the docker
-container. ``` docker exec -it  bash -c "stty cols $COLUMNS rows $LINES &&
-bash" ``` ## Why called _radian_? _radian_ is powered by (Ï)thon. ## Credits
-_radian_ wouldn't be possible without the creative work [prompt_toolkit](https:
-//github.com/jonathanslenders/python-prompt-toolkit/) by Jonathan Slenders.
-Platform: UNKNOWN Requires-Python: >=3.6 Description-Content-Type: text/
-markdown Provides-Extra: test
+However, it was reported that radian may be slower when using parallel
+computation, specifially when using forking. User should take extra care in
+those cases. #### Nvim-R support Put ```vim let R_app = "radian" let R_cmd =
+"R" let R_hl_term = 0 let R_args = [] " if you had set any let
+R_bracketed_paste = 1 ``` in your vim config. #### `reticulate` Auto
+Completions To enable reticulate prompt completions, make sure that `jedi` is
+installed. ```sh pip install jedi ``` Alternatively, if you use conda, ```sh
+conda install -c conda-forge jedi ``` #### Prompt not shown inside a docker
+container It maybe caused by the invalid terminal size, try running `stty size`
+in your terminal to see if it returns a correct size. You could change the
+values of it from the environmental variables `$COLUMNS` and `$LINES` when you
+log-in the docker container. ``` docker exec -it  bash -c "stty cols $COLUMNS
+rows $LINES && bash" ``` ## Why called _radian_? _radian_ is powered by
+(Ï)thon. ## Credits _radian_ wouldn't be possible without the creative work
+[prompt_toolkit](https://github.com/jonathanslenders/python-prompt-toolkit/) by
+Jonathan Slenders. Platform: UNKNOWN Requires-Python: >=3.6 Description-
+Content-Type: text/markdown Provides-Extra: test
```

### Comparing `radian-0.6.5/radian.egg-info/SOURCES.txt` & `radian-0.6.6/radian.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `radian-0.6.5/setup.py` & `radian-0.6.6/setup.py`

 * *Files identical despite different names*

