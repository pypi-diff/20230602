# Comparing `tmp/specker-1.0.3.tar.gz` & `tmp/specker-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specker-1.0.3.tar", last modified: Tue Feb 28 08:27:20 2023, max compression
+gzip compressed data, was "specker-1.1.0.tar", last modified: Fri Jun  2 06:42:16 2023, max compression
```

## Comparing `specker-1.0.3.tar` & `specker-1.1.0.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 08:27:20.667819 specker-1.0.3/
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-02-28 08:26:25.000000 specker-1.0.3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      780 2023-02-28 08:26:25.000000 specker-1.0.3/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-02-28 08:26:25.000000 specker-1.0.3/.mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)    20971 2023-02-28 08:26:25.000000 specker-1.0.3/.pylintrc
--rw-rw-rw-   0 root         (0) root         (0)   115210 2023-02-28 08:26:25.000000 specker-1.0.3/Doxyfile
--rw-rw-rw-   0 root         (0) root         (0)    35149 2023-02-28 08:26:25.000000 specker-1.0.3/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)     2530 2023-02-28 08:26:25.000000 specker-1.0.3/Makefile
--rw-r--r--   0 root         (0) root         (0)     6194 2023-02-28 08:27:20.667819 specker-1.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5416 2023-02-28 08:26:25.000000 specker-1.0.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)      100 2023-02-28 08:26:25.000000 specker-1.0.3/build_requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)     2586 2023-02-28 08:26:25.000000 specker-1.0.3/git-tags.sh
--rw-rw-rw-   0 root         (0) root         (0)     1143 2023-02-28 08:27:13.000000 specker-1.0.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-28 08:27:20.667819 specker-1.0.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 08:27:20.658819 specker-1.0.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 08:27:20.663819 specker-1.0.3/src/specker/
--rw-rw-rw-   0 root         (0) root         (0)     3237 2023-02-28 08:26:25.000000 specker-1.0.3/src/specker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2457 2023-02-28 08:26:25.000000 specker-1.0.3/src/specker/content.py
--rw-rw-rw-   0 root         (0) root         (0)     4810 2023-02-28 08:26:25.000000 specker-1.0.3/src/specker/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 08:27:20.667819 specker-1.0.3/src/specker/specs/
--rw-rw-rw-   0 root         (0) root         (0)      751 2023-02-28 08:26:25.000000 specker-1.0.3/src/specker/specs/SPECFILES.md
--rw-rw-rw-   0 root         (0) root         (0)      769 2023-02-28 08:26:25.000000 specker-1.0.3/src/specker/specs/specker.spec
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 08:27:20.665819 specker-1.0.3/src/specker.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6194 2023-02-28 08:27:20.000000 specker-1.0.3/src/specker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      443 2023-02-28 08:27:20.000000 specker-1.0.3/src/specker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-28 08:27:20.000000 specker-1.0.3/src/specker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      114 2023-02-28 08:27:20.000000 specker-1.0.3/src/specker.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-02-28 08:27:20.000000 specker-1.0.3/src/specker.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 06:42:16.242685 specker-1.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-02 06:24:00.000000 specker-1.1.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      828 2023-06-02 06:34:14.000000 specker-1.1.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-02 06:24:00.000000 specker-1.1.0/.mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)    20971 2023-06-02 06:24:00.000000 specker-1.1.0/.pylintrc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 06:42:16.238685 specker-1.1.0/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      802 2023-06-02 06:24:00.000000 specker-1.1.0/.vscode/extensions.json
+-rw-rw-rw-   0 root         (0) root         (0)   115210 2023-06-02 06:24:00.000000 specker-1.1.0/Doxyfile
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2023-06-02 06:24:00.000000 specker-1.1.0/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)     2530 2023-06-02 06:24:00.000000 specker-1.1.0/Makefile
+-rw-r--r--   0 root         (0) root         (0)     6884 2023-06-02 06:42:16.242685 specker-1.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6106 2023-06-02 06:24:00.000000 specker-1.1.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-06-02 06:24:00.000000 specker-1.1.0/build_requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)     2586 2023-06-02 06:24:00.000000 specker-1.1.0/git-tags.sh
+-rwxrwxrwx   0 root         (0) root         (0)     7192 2023-06-02 06:24:00.000000 specker-1.1.0/icon.png
+-rw-rw-rw-   0 root         (0) root         (0)     1143 2023-06-02 06:42:10.000000 specker-1.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-02 06:42:16.242685 specker-1.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 06:42:16.238685 specker-1.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 06:42:16.242685 specker-1.1.0/src/specker/
+-rw-rw-rw-   0 root         (0) root         (0)     3237 2023-06-02 06:24:00.000000 specker-1.1.0/src/specker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2556 2023-06-02 06:24:00.000000 specker-1.1.0/src/specker/content.py
+-rw-rw-rw-   0 root         (0) root         (0)     5945 2023-06-02 06:24:00.000000 specker-1.1.0/src/specker/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 06:42:16.242685 specker-1.1.0/src/specker/specs/
+-rw-rw-rw-   0 root         (0) root         (0)      840 2023-06-02 06:24:00.000000 specker-1.1.0/src/specker/specs/SPECFILES.md
+-rw-rw-rw-   0 root         (0) root         (0)      890 2023-06-02 06:24:00.000000 specker-1.1.0/src/specker/specs/specker.spec
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 06:42:16.242685 specker-1.1.0/src/specker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6884 2023-06-02 06:42:16.000000 specker-1.1.0/src/specker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      476 2023-06-02 06:42:16.000000 specker-1.1.0/src/specker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 06:42:16.000000 specker-1.1.0/src/specker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-02 06:42:16.000000 specker-1.1.0/src/specker.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-02 06:42:16.000000 specker-1.1.0/src/specker.egg-info/top_level.txt
```

### Comparing `specker-1.0.3/.gitlab-ci.yml` & `specker-1.1.0/.gitlab-ci.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 image: debian:bullseye-slim
 
+default:
+  tags:
+    - atc-runner
+    - docker
+
 before_script:
   - apt update
   - DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true apt -y install make python3 python3-pip python3-venv git curl jq
   - make install_build_deps
 
 stages:
   - lint
@@ -28,14 +33,14 @@
     - tags
 
 dist:
   stage: dist
   script:
     - make DIST_PASSWORD="$PYPI_TOKEN" dist
   rules:
-    - if: $CI_COMMIT_BRANCH == $CI_DEFAULT_BRANCH && $CI_COMMIT_TITLE =~ /Merge branch.*/
+    - if: $CI_COMMIT_BRANCH == $CI_DEFAULT_BRANCH && $CI_COMMIT_MESSAGE  =~ /Merge Ref.*/
 tag:
   stage: dist
   script:
     - make DIST_PASSWORD="$TAG_TOKEN" tag
   rules:
-    - if: $CI_COMMIT_BRANCH == $CI_DEFAULT_BRANCH && $CI_COMMIT_TITLE =~ /Merge branch.*/
+    - if: $CI_COMMIT_BRANCH == $CI_DEFAULT_BRANCH && $CI_COMMIT_MESSAGE  =~ /Merge Ref.*/
```

### Comparing `specker-1.0.3/.pylintrc` & `specker-1.1.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `specker-1.0.3/Doxyfile` & `specker-1.1.0/Doxyfile`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 PROJECT_NAME           = "Specker JSON Specification Validator"
 
 # The PROJECT_NUMBER tag can be used to enter a project or revision number. This
 # could be handy for archiving the generated documentation or if some version
 # control system is used.
 
-PROJECT_NUMBER = "1.0.3"
+PROJECT_NUMBER = "1.1.0"
 
 # Using the PROJECT_BRIEF tag one can provide an optional one line description
 # for a project that appears at the top of each page and should give viewer a
 # quick idea about the purpose of the project. Keep the description short.
 
 PROJECT_BRIEF          =
```

### Comparing `specker-1.0.3/LICENSE.md` & `specker-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `specker-1.0.3/Makefile` & `specker-1.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `specker-1.0.3/PKG-INFO` & `specker-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specker
-Version: 1.0.3
+Version: 1.1.0
 Summary: Specker JSON Specification Validator
 Author-email: AccidentallyTheCable <cableninja@cableninja.net>
 License: GPLv3
 Project-URL: Homepage, https://gitlab.com/accidentallythecable-public/python-modules/python-specker/
 Project-URL: Bug Tracker, https://gitlab.com/accidentallythecable-public/python-modules/python-specker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -97,14 +97,21 @@
         "comment": "Time Configuration"
     },
     "environment": {
         "required": false,
         "default": {},
         "type": "dict",
         "comment": "Environment Variables to use during Command execution"
+    },
+    "visibility": {
+        "required": false,
+        "default": "hidden",
+        "type": "str",
+        "values": [ "hidden", "visible", "admin", "deleted" ],
+        "comment": "Visbility of Command Information"
     }
 }
 ```
 
 Given the above Spec, additional Specs sould be created for `time` and optionally `environment`, Note the `dict` value for `type`. This will validate that `time` is a `dict`, without caring what is in it. For that validation, you need the spec below.
 
 Spec: `myfile.json_time.spec`
@@ -160,12 +167,23 @@
     exit(1)
 spec_result = spec_loader.compare("myfile.json_time",config_content["time"])
 if not spec_result:
     exit(1)
 exit(0)
 ```
 
+We can additionally Gather any default values the Spec contains, with the `defaults` function:
+
+```
+# Initialize the Loader, and point it to your Spec directory
+spec_loader = SpecLoader(Path(__file__).resolve().parent.joinpath("specs")) # This would load `../specs/` from the location where SpecLoader was initialized
+
+# Load `myfile.json.spec` and gather any defaults from it
+spec_defaults = spec_loader.defaults("myfile.json")
+print(json.dumps(spec_defaults))
+```
+
 ## Utils
 
 To aid in documentation, Specker comes with `generate-spec-docs.py`, a script to generate a .md file from a directory of Spec files. (See `SPECFILES.md`, this is a generated document).
 
 You can additionally validate a Spec file using `validate-spec-file.py`, to ensure that your Spec file is built properly.
```

### Comparing `specker-1.0.3/README.md` & `specker-1.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -79,14 +79,21 @@
         "comment": "Time Configuration"
     },
     "environment": {
         "required": false,
         "default": {},
         "type": "dict",
         "comment": "Environment Variables to use during Command execution"
+    },
+    "visibility": {
+        "required": false,
+        "default": "hidden",
+        "type": "str",
+        "values": [ "hidden", "visible", "admin", "deleted" ],
+        "comment": "Visbility of Command Information"
     }
 }
 ```
 
 Given the above Spec, additional Specs sould be created for `time` and optionally `environment`, Note the `dict` value for `type`. This will validate that `time` is a `dict`, without caring what is in it. For that validation, you need the spec below.
 
 Spec: `myfile.json_time.spec`
@@ -142,12 +149,23 @@
     exit(1)
 spec_result = spec_loader.compare("myfile.json_time",config_content["time"])
 if not spec_result:
     exit(1)
 exit(0)
 ```
 
+We can additionally Gather any default values the Spec contains, with the `defaults` function:
+
+```
+# Initialize the Loader, and point it to your Spec directory
+spec_loader = SpecLoader(Path(__file__).resolve().parent.joinpath("specs")) # This would load `../specs/` from the location where SpecLoader was initialized
+
+# Load `myfile.json.spec` and gather any defaults from it
+spec_defaults = spec_loader.defaults("myfile.json")
+print(json.dumps(spec_defaults))
+```
+
 ## Utils
 
 To aid in documentation, Specker comes with `generate-spec-docs.py`, a script to generate a .md file from a directory of Spec files. (See `SPECFILES.md`, this is a generated document).
 
 You can additionally validate a Spec file using `validate-spec-file.py`, to ensure that your Spec file is built properly.
```

### Comparing `specker-1.0.3/git-tags.sh` & `specker-1.1.0/git-tags.sh`

 * *Files identical despite different names*

### Comparing `specker-1.0.3/pyproject.toml` & `specker-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "specker"
-version = "1.0.3"
+version = "1.1.0"
 authors = [
   { name="AccidentallyTheCable", email="cableninja@cableninja.net" },
 ]
 description = "Specker JSON Specification Validator"
 readme = "README.md"
 requires-python = ">=3.9"
 license = { text = "GPLv3" }
```

### Comparing `specker-1.0.3/src/specker/__init__.py` & `specker-1.1.0/src/specker/__init__.py`

 * *Files identical despite different names*

### Comparing `specker-1.0.3/src/specker/content.py` & `specker-1.1.0/src/specker/content.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
     _name:str
     _required:bool
     _default:typing.Any
     _type:str
     _comment:str
     _example:str
+    _values:list[typing.Any]
 
     def get(self,attr:str) -> typing.Any:
         """Get a Parameter
         @param str \c attr Attribute to Get
         @retval Any Value of Attribute if it exists
         @throws AttributeError Cannot find Requested Attribute (or not set)
         """
@@ -59,14 +60,16 @@
             self._required = False
         if not hasattr(self,"_default"):
             self._default = None
         if not hasattr(self,"_comment"):
             self._comment = ""
         if not hasattr(self,"_example"):
             self._example = ""
+        if not hasattr(self,"_values"):
+            self._values = []
 
     def __str__(self) -> str:
         """To String Generator
         @retval str Markdown Formatted Data about Spec
         """
         return f'''Option: `{self._name}` - {self._comment}
  - Type: {self._type}
```

### Comparing `specker-1.0.3/src/specker/loader.py` & `specker-1.1.0/src/specker/loader.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import os
 import re
 import json
 import typing
 import logging
 from pathlib import Path
 
+# from specker import content
+
 if __name__ == "loader":
     # pylint: disable=import-error
     from content import SpecContent
     # pylint: enable=import-error
 else:
     from .content import SpecContent
 
@@ -90,16 +92,42 @@
                 logging.debug(f"{k}: pass, not required, but is empty")
                 continue
             if spec.type != type(content[k]) and spec.type != typing.Any:
                 spec_pass = False
                 logging.error(f"{k}: fail, must be {str(spec.type)}, got: {str(type(content[k]))}")
             else:
                 logging.debug(f"{k}: pass, type match; need:{str(spec.type)}, got:{str(type(content[k]))}")
+            valid_values:list[typing.Any] = spec.get("values")
+            if len(valid_values) > 0:
+                values:str = ""
+                for v in valid_values:
+                    values += f",{str(v)}"
+                values = values.lstrip(",")
+                if content[k] not in valid_values:
+                    spec_pass = False
+                    logging.error(f"{k}: fail, invalid value; must be one of: {values}")
+                else:
+                    logging.debug(f"{k}: pass, value match, need:{values}, got:{str(content[k])}")
         return spec_pass
 
+    def defaults(self,spec_file_name:str) -> dict[typing.Any,typing.Any]:
+        """Get any Defined Defaults from a Spec
+        @param str \c spec_file_name Spec File Name to pull
+        @retval dict[Any,Any] Spec Defaults
+        """
+        spec_file:dict[str,SpecContent] = self.get(spec_file_name)
+        content:dict[typing.Any,typing.Any] = {}
+
+        for k,spec in spec_file.items():
+            try:
+                content[k] = spec.get("default")
+            except AttributeError:
+                continue
+        return content
+
     def get(self,spec_file_name:str) -> dict[str,SpecContent]:
         """Get Spec Content for a Config
         @param str \c spec_file_name Name of Spec to Get
         @retval dict[str,SpecContent] Configuration Spec
         """
         return self._specs[spec_file_name]
```

### Comparing `specker-1.0.3/src/specker/specs/SPECFILES.md` & `specker-1.1.0/src/specker/specs/SPECFILES.md`

 * *Files 25% similar despite different names*

```diff
@@ -2,32 +2,38 @@
 Auto generated from .spec files
 ## Spec for specker
 
 Option: `required` - Whether or not this Option is required
  - Type: bool
  - Required: False
  - Default: False
- - Example: None
+ - Example: 
 
 Option: `default` - Default Value if not required and not set
  - Type: any
  - Required: False
  - Default: None
- - Example: None
+ - Example: 
 
 Option: `type` - Type the Value must be. Must be one of: int, str, list, dict, bool, any
  - Type: str
  - Required: True
  - Default: any
- - Example: None
+ - Example: 
 
 Option: `comment` - Informational Comment about this Option and Value
  - Type: str
  - Required: False
  - Default: None
- - Example: None
+ - Example: 
 
 Option: `example` - Example Data for this Option and Value
  - Type: any
  - Required: False
  - Default: None
- - Example: None
+ - Example: 
+
+Option: `values` - List of Acceptable Values
+ - Type: list
+ - Required: False
+ - Default: None
+ - Example:
```

### Comparing `specker-1.0.3/src/specker/specs/specker.spec` & `specker-1.1.0/src/specker/specs/specker.spec`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'values'": "OrderedDict([('required', False), ('type', 'list'), ('comment', 'List of Acceptable "*

 * *             "Values')])"}*

```diff
@@ -21,9 +21,14 @@
         "type": "bool"
     },
     "type": {
         "comment": "Type the Value must be. Must be one of: int, str, list, dict, bool, any",
         "default": "any",
         "required": true,
         "type": "str"
+    },
+    "values": {
+        "comment": "List of Acceptable Values",
+        "required": false,
+        "type": "list"
     }
 }
```

### Comparing `specker-1.0.3/src/specker.egg-info/PKG-INFO` & `specker-1.1.0/src/specker.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specker
-Version: 1.0.3
+Version: 1.1.0
 Summary: Specker JSON Specification Validator
 Author-email: AccidentallyTheCable <cableninja@cableninja.net>
 License: GPLv3
 Project-URL: Homepage, https://gitlab.com/accidentallythecable-public/python-modules/python-specker/
 Project-URL: Bug Tracker, https://gitlab.com/accidentallythecable-public/python-modules/python-specker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -97,14 +97,21 @@
         "comment": "Time Configuration"
     },
     "environment": {
         "required": false,
         "default": {},
         "type": "dict",
         "comment": "Environment Variables to use during Command execution"
+    },
+    "visibility": {
+        "required": false,
+        "default": "hidden",
+        "type": "str",
+        "values": [ "hidden", "visible", "admin", "deleted" ],
+        "comment": "Visbility of Command Information"
     }
 }
 ```
 
 Given the above Spec, additional Specs sould be created for `time` and optionally `environment`, Note the `dict` value for `type`. This will validate that `time` is a `dict`, without caring what is in it. For that validation, you need the spec below.
 
 Spec: `myfile.json_time.spec`
@@ -160,12 +167,23 @@
     exit(1)
 spec_result = spec_loader.compare("myfile.json_time",config_content["time"])
 if not spec_result:
     exit(1)
 exit(0)
 ```
 
+We can additionally Gather any default values the Spec contains, with the `defaults` function:
+
+```
+# Initialize the Loader, and point it to your Spec directory
+spec_loader = SpecLoader(Path(__file__).resolve().parent.joinpath("specs")) # This would load `../specs/` from the location where SpecLoader was initialized
+
+# Load `myfile.json.spec` and gather any defaults from it
+spec_defaults = spec_loader.defaults("myfile.json")
+print(json.dumps(spec_defaults))
+```
+
 ## Utils
 
 To aid in documentation, Specker comes with `generate-spec-docs.py`, a script to generate a .md file from a directory of Spec files. (See `SPECFILES.md`, this is a generated document).
 
 You can additionally validate a Spec file using `validate-spec-file.py`, to ensure that your Spec file is built properly.
```

