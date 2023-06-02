# Comparing `tmp/docstring-generator-0.3.0.tar.gz` & `tmp/docstring-generator-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docstring-generator-0.3.0.tar", max compression
+gzip compressed data, was "docstring-generator-0.3.1.tar", max compression
```

## Comparing `docstring-generator-0.3.0.tar` & `docstring-generator-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,7 @@
--rw-r--r--   0        0        0     1066 2023-05-27 21:10:19.698153 docstring-generator-0.3.0/LICENSE
--rw-r--r--   0        0        0     1818 2023-05-27 21:10:19.698153 docstring-generator-0.3.0/README.md
--rw-r--r--   0        0        0       89 2023-05-27 21:10:19.698153 docstring-generator-0.3.0/docstring_generator/__init__.py
--rw-r--r--   0        0        0      143 2023-05-27 21:10:19.698153 docstring-generator-0.3.0/docstring_generator/__main__.py
--rw-r--r--   0        0        0      126 2023-05-27 21:10:19.698153 docstring-generator-0.3.0/docstring_generator/config.py
--rw-r--r--   0        0        0     2708 2023-05-27 21:10:19.698153 docstring-generator-0.3.0/docstring_generator/docstring_generator.py
--rw-r--r--   0        0        0     2323 2023-05-27 21:10:19.698153 docstring-generator-0.3.0/docstring_generator/docstring_utils.py
--rw-r--r--   0        0        0     4828 2023-05-27 21:10:19.698153 docstring-generator-0.3.0/docstring_generator/function_cache.py
--rw-r--r--   0        0        0     8255 2023-05-27 21:10:19.698153 docstring-generator-0.3.0/docstring_generator/gen_docs.py
--rw-r--r--   0        0        0      954 2023-05-27 21:10:19.698153 docstring-generator-0.3.0/docstring_generator/new_gen_docs.py
--rw-r--r--   0        0        0     1281 2023-05-27 21:10:19.702153 docstring-generator-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2898 1970-01-01 00:00:00.000000 docstring-generator-0.3.0/setup.py
--rw-r--r--   0        0        0     2941 1970-01-01 00:00:00.000000 docstring-generator-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-02 09:18:13.626272 docstring-generator-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1818 2023-06-02 09:18:13.626272 docstring-generator-0.3.1/README.md
+-rw-r--r--   0        0        0       89 2023-06-02 09:18:13.626272 docstring-generator-0.3.1/docstring_generator/__init__.py
+-rw-r--r--   0        0        0      954 2023-06-02 09:18:13.626272 docstring-generator-0.3.1/docstring_generator/new_gen_docs.py
+-rw-r--r--   0        0        0     1177 2023-06-02 09:18:13.630272 docstring-generator-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2764 1970-01-01 00:00:00.000000 docstring-generator-0.3.1/setup.py
+-rw-r--r--   0        0        0     2898 1970-01-01 00:00:00.000000 docstring-generator-0.3.1/PKG-INFO
```

### Comparing `docstring-generator-0.3.0/LICENSE` & `docstring-generator-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `docstring-generator-0.3.0/README.md` & `docstring-generator-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `docstring-generator-0.3.0/docstring_generator/new_gen_docs.py` & `docstring-generator-0.3.1/docstring_generator/new_gen_docs.py`

 * *Files identical despite different names*

### Comparing `docstring-generator-0.3.0/pyproject.toml` & `docstring-generator-0.3.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.isort]
 combine_as_imports = true
 line_length = 100
 profile = "black"
 
 [tool.poetry]
 name = "docstring-generator"
-version = "0.3.0"
+version = "0.3.1"
 description = "Auto generate docstring from type-hints."
 authors = ["FelixTheC <felixeisenmenger@gmx.net>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/FelixTheC/docstring_generator"
 packages = [{include = "docstring_generator"}]
 classifiers=[
@@ -25,23 +25,20 @@
     "Programming Language :: Python :: 3.10",
     "Topic :: Utilities",
     "Topic :: Software Development :: Documentation",
     "Typing :: Typed",
 ]
 
 [tool.poetry.scripts]
-gendocs = "docstring_generator.__main__:main"
 gendocs_new = "docstring_generator.new_gen_docs:main"
 
 [tool.poetry.dependencies]
-python = ">=3.9,<=3.11"
-strongtyping = "^3.9.2"
-strongtyping-pyoverload = "^0.3.0"
+python = ">=3.8,<=3.11"
 click = "^8.1.3"
-docstring-generator-ext = "0.0.26"
+docstring-generator-ext = "^0.0.28"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.8.0"
 isort = "^5.10.1"
 pytest = "^7.1.3"
 
 [build-system]
```

### Comparing `docstring-generator-0.3.0/setup.py` & `docstring-generator-0.3.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,35 +4,31 @@
 packages = \
 ['docstring_generator']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['click>=8.1.3,<9.0.0',
- 'docstring-generator-ext==0.0.26',
- 'strongtyping-pyoverload>=0.3.0,<0.4.0',
- 'strongtyping>=3.9.2,<4.0.0']
+['click>=8.1.3,<9.0.0', 'docstring-generator-ext>=0.0.28,<0.0.29']
 
 entry_points = \
-{'console_scripts': ['gendocs = docstring_generator.__main__:main',
-                     'gendocs_new = docstring_generator.new_gen_docs:main']}
+{'console_scripts': ['gendocs_new = docstring_generator.new_gen_docs:main']}
 
 setup_kwargs = {
     'name': 'docstring-generator',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'Auto generate docstring from type-hints.',
     'long_description': '# docstring_generator\nAuto generate docstring from type-hints for python functions and class methods.\n\n## How to use it\n```shell\ngendocs_new file.py\n```\n\n```shell\ngendocs_new mydir/\n```\n\n## Options\n\n### style\n- `--style`\n- Docstring style [numpy, google, rest].  [default: numpy]\n\n### Add additional information before running `gendocs_new` \n- when adding `$<num>` into your docstring these will then be replaced with parameter at this index\n- Example:\n```python\nfrom typing import List\n\n\ndef foo(val_a: int, val_b: List[int]):\n    """\n    Lorem ipsum dolor sit amet, consetetur sadipscing elitr,\n    sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam\n\n    $1 Lorem ipsum dolor sit amet\n    $2 nonumy eirmod tempor invidun\n    """\n```\nwill become (here with numpy style)\n```python\nfrom typing import List\n\n\ndef foo(val_a: int, val_b: List[int]):\n    """\n    Lorem ipsum dolor sit amet, consetetur sadipscing elitr,\n    sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam\n    \n    Parameters\n    ----------\n    val_a : argument of type int\n        Lorem ipsum dolor sit amet\n    val_b : argument of type List(int)\n        nonumy eirmod tempor invidun\n\n    """\n```\n\n## FAQ\n#### what happens if I re-run the docstring creation?\n- nothing if all stays the same, changed parameter descriptions will be ignored only changes of the function header will be used\n\n## Examples\n- An example can be found under examples\n\n### Installing\n\n- pip install docstring-generator\n\n#### Versioning\n- For the versions available, see the tags on this repository.\n\n### Support for older version\n- the previous command `gendocs` is still supported for this version.\n\n### Authors\n- Felix Eisenmenger\n\n### License\n- This project is licensed under the MIT License - see the LICENSE.md file for details\n',
     'author': 'FelixTheC',
     'author_email': 'felixeisenmenger@gmx.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/FelixTheC/docstring_generator',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.9,<=3.11',
+    'python_requires': '>=3.8,<=3.11',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `docstring-generator-0.3.0/PKG-INFO` & `docstring-generator-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: docstring-generator
-Version: 0.3.0
+Version: 0.3.1
 Summary: Auto generate docstring from type-hints.
 Home-page: https://github.com/FelixTheC/docstring_generator
 License: MIT
 Author: FelixTheC
 Author-email: felixeisenmenger@gmx.net
-Requires-Python: >=3.9,<=3.11
+Requires-Python: >=3.8,<=3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: docstring-generator-ext (==0.0.26)
-Requires-Dist: strongtyping (>=3.9.2,<4.0.0)
-Requires-Dist: strongtyping-pyoverload (>=0.3.0,<0.4.0)
+Requires-Dist: docstring-generator-ext (>=0.0.28,<0.0.29)
 Project-URL: Repository, https://github.com/FelixTheC/docstring_generator
 Description-Content-Type: text/markdown
 
 # docstring_generator
 Auto generate docstring from type-hints for python functions and class methods.
 
 ## How to use it
```

