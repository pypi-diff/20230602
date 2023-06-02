# Comparing `tmp/qctrl_open_controls-9.1.7.tar.gz` & `tmp/qctrl_open_controls-9.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qctrl_open_controls-9.1.7.tar", max compression
+gzip compressed data, was "qctrl_open_controls-9.1.8.tar", max compression
```

## Comparing `qctrl_open_controls-9.1.7.tar` & `qctrl_open_controls-9.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    10141 2023-02-10 05:47:31.562919 qctrl_open_controls-9.1.7/LICENSE
--rw-r--r--   0        0        0      626 2023-02-10 05:47:31.562919 qctrl_open_controls-9.1.7/README.md
--rw-r--r--   0        0        0     2886 2023-02-10 05:47:45.667258 qctrl_open_controls-9.1.7/pyproject.toml
--rw-r--r--   0        0        0     2305 2023-02-10 05:47:45.679258 qctrl_open_controls-9.1.7/qctrlopencontrols/__init__.py
--rw-r--r--   0        0        0     1004 2023-02-10 05:47:31.562919 qctrl_open_controls-9.1.7/qctrlopencontrols/constants.py
--rw-r--r--   0        0        0      569 2023-02-10 05:47:45.675258 qctrl_open_controls-9.1.7/qctrlopencontrols/driven_controls/__init__.py
--rw-r--r--   0        0        0    23611 2023-02-10 05:47:31.562919 qctrl_open_controls-9.1.7/qctrlopencontrols/driven_controls/driven_control.py
--rw-r--r--   0        0        0    46134 2023-02-10 05:47:31.562919 qctrl_open_controls-9.1.7/qctrlopencontrols/driven_controls/predefined.py
--rw-r--r--   0        0        0      569 2023-02-10 05:47:45.675258 qctrl_open_controls-9.1.7/qctrlopencontrols/dynamic_decoupling_sequences/__init__.py
--rw-r--r--   0        0        0    20297 2023-02-10 05:47:31.562919 qctrl_open_controls-9.1.7/qctrlopencontrols/dynamic_decoupling_sequences/dynamic_decoupling_sequence.py
--rw-r--r--   0        0        0    40422 2023-02-10 05:47:31.566919 qctrl_open_controls-9.1.7/qctrlopencontrols/dynamic_decoupling_sequences/predefined.py
--rw-r--r--   0        0        0     2007 2023-02-10 05:47:31.566919 qctrl_open_controls-9.1.7/qctrlopencontrols/exceptions.py
--rw-r--r--   0        0        0     4242 2023-02-10 05:47:31.566919 qctrl_open_controls-9.1.7/qctrlopencontrols/utils.py
--rw-r--r--   0        0        0     1585 1970-01-01 00:00:00.000000 qctrl_open_controls-9.1.7/setup.py
--rw-r--r--   0        0        0     2953 1970-01-01 00:00:00.000000 qctrl_open_controls-9.1.7/PKG-INFO
+-rw-r--r--   0        0        0    10141 2023-03-02 05:33:13.279275 qctrl_open_controls-9.1.8/LICENSE
+-rw-r--r--   0        0        0      626 2023-03-02 05:33:13.279275 qctrl_open_controls-9.1.8/README.md
+-rw-r--r--   0        0        0     2886 2023-03-02 05:33:28.435287 qctrl_open_controls-9.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2305 2023-03-02 05:33:28.443287 qctrl_open_controls-9.1.8/qctrlopencontrols/__init__.py
+-rw-r--r--   0        0        0     1004 2023-03-02 05:33:13.279275 qctrl_open_controls-9.1.8/qctrlopencontrols/constants.py
+-rw-r--r--   0        0        0      569 2023-03-02 05:33:28.447287 qctrl_open_controls-9.1.8/qctrlopencontrols/driven_controls/__init__.py
+-rw-r--r--   0        0        0    23611 2023-03-02 05:33:13.283275 qctrl_open_controls-9.1.8/qctrlopencontrols/driven_controls/driven_control.py
+-rw-r--r--   0        0        0    46134 2023-03-02 05:33:13.283275 qctrl_open_controls-9.1.8/qctrlopencontrols/driven_controls/predefined.py
+-rw-r--r--   0        0        0      569 2023-03-02 05:33:28.443287 qctrl_open_controls-9.1.8/qctrlopencontrols/dynamic_decoupling_sequences/__init__.py
+-rw-r--r--   0        0        0    20297 2023-03-02 05:33:13.283275 qctrl_open_controls-9.1.8/qctrlopencontrols/dynamic_decoupling_sequences/dynamic_decoupling_sequence.py
+-rw-r--r--   0        0        0    40422 2023-03-02 05:33:13.283275 qctrl_open_controls-9.1.8/qctrlopencontrols/dynamic_decoupling_sequences/predefined.py
+-rw-r--r--   0        0        0     2007 2023-03-02 05:33:13.283275 qctrl_open_controls-9.1.8/qctrlopencontrols/exceptions.py
+-rw-r--r--   0        0        0     4242 2023-03-02 05:33:13.283275 qctrl_open_controls-9.1.8/qctrlopencontrols/utils.py
+-rw-r--r--   0        0        0     1585 1970-01-01 00:00:00.000000 qctrl_open_controls-9.1.8/setup.py
+-rw-r--r--   0        0        0     2953 1970-01-01 00:00:00.000000 qctrl_open_controls-9.1.8/PKG-INFO
```

### Comparing `qctrl_open_controls-9.1.7/LICENSE` & `qctrl_open_controls-9.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `qctrl_open_controls-9.1.7/README.md` & `qctrl_open_controls-9.1.8/README.md`

 * *Files identical despite different names*

### Comparing `qctrl_open_controls-9.1.7/pyproject.toml` & `qctrl_open_controls-9.1.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qctrl-open-controls"
-version = "9.1.7"
+version = "9.1.8"
 description = "Q-CTRL Python Open Controls"
 license = "Apache-2.0"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
 repository = "https://github.com/qctrl/python-open-controls"
@@ -72,15 +72,15 @@
 
 [tool.poetry.dev-dependencies]
 black = "^22.3.0"
 mypy = "^0.991"
 pytest = "^7.0"
 pylint = "^2.16.1"
 sphinx = "^5.0.0"
-qctrl-sphinx-theme = "~0.1.1"
+qctrl-sphinx-theme = "~0.1.2"
 isort = "^5.7.0"
 pre-commit = "^2.9.3"
 
 [tool.poetry.urls]
 GitHub = "https://github.com/qctrl"
 Twitter = "https://twitter.com/qctrlHQ"
```

### Comparing `qctrl_open_controls-9.1.7/qctrlopencontrols/__init__.py` & `qctrl_open_controls-9.1.8/qctrlopencontrols/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Top-level package for Q-CTRL Open Controls.
 """
 
-__version__ = "9.1.7"
+__version__ = "9.1.8"
 
 from .driven_controls.driven_control import DrivenControl
 from .driven_controls.predefined import (
     new_bb1_control,
     new_corpse_control,
     new_corpse_in_bb1_control,
     new_corpse_in_scrofulous_control,
```

### Comparing `qctrl_open_controls-9.1.7/qctrlopencontrols/constants.py` & `qctrl_open_controls-9.1.8/qctrlopencontrols/constants.py`

 * *Files identical despite different names*

### Comparing `qctrl_open_controls-9.1.7/qctrlopencontrols/driven_controls/__init__.py` & `qctrl_open_controls-9.1.8/qctrlopencontrols/driven_controls/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_open_controls-9.1.7/qctrlopencontrols/driven_controls/driven_control.py` & `qctrl_open_controls-9.1.8/qctrlopencontrols/driven_controls/driven_control.py`

 * *Files identical despite different names*

### Comparing `qctrl_open_controls-9.1.7/qctrlopencontrols/driven_controls/predefined.py` & `qctrl_open_controls-9.1.8/qctrlopencontrols/driven_controls/predefined.py`

 * *Files identical despite different names*

### Comparing `qctrl_open_controls-9.1.7/qctrlopencontrols/dynamic_decoupling_sequences/__init__.py` & `qctrl_open_controls-9.1.8/qctrlopencontrols/dynamic_decoupling_sequences/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_open_controls-9.1.7/qctrlopencontrols/dynamic_decoupling_sequences/dynamic_decoupling_sequence.py` & `qctrl_open_controls-9.1.8/qctrlopencontrols/dynamic_decoupling_sequences/dynamic_decoupling_sequence.py`

 * *Files identical despite different names*

### Comparing `qctrl_open_controls-9.1.7/qctrlopencontrols/dynamic_decoupling_sequences/predefined.py` & `qctrl_open_controls-9.1.8/qctrlopencontrols/dynamic_decoupling_sequences/predefined.py`

 * *Files identical despite different names*

### Comparing `qctrl_open_controls-9.1.7/qctrlopencontrols/exceptions.py` & `qctrl_open_controls-9.1.8/qctrlopencontrols/exceptions.py`

 * *Files identical despite different names*

### Comparing `qctrl_open_controls-9.1.7/qctrlopencontrols/utils.py` & `qctrl_open_controls-9.1.8/qctrlopencontrols/utils.py`

 * *Files identical despite different names*

### Comparing `qctrl_open_controls-9.1.7/setup.py` & `qctrl_open_controls-9.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 extras_require = \
 {':python_version >= "3.7" and python_version < "3.8"': ['numpy>=1.21.6,<2.0.0'],
  ':python_version >= "3.8"': ['numpy>=1.23.0,<2.0.0']}
 
 setup_kwargs = {
     'name': 'qctrl-open-controls',
-    'version': '9.1.7',
+    'version': '9.1.8',
     'description': 'Q-CTRL Python Open Controls',
     'long_description': '# Q-CTRL Open Controls\n\nQ-CTRL Open Controls is an open-source Python package that makes it easy to\ncreate and deploy established error-robust quantum control protocols from the\nopen literature. The aim of the package is to be the most comprehensive library\nof published and tested quantum control techniques developed by the community,\nwith easy to use export functions allowing users to deploy these controls on:\n\n- Custom quantum hardware\n- Publicly available cloud quantum computers\n- The [Q-CTRL product suite](https://q-ctrl.com/products/)\n\nAnyone interested in quantum control is welcome to contribute to this project.\n',
     'author': 'Q-CTRL',
     'author_email': 'support@q-ctrl.com',
     'maintainer': 'Q-CTRL',
     'maintainer_email': 'support@q-ctrl.com',
     'url': 'https://q-ctrl.com',
```

### Comparing `qctrl_open_controls-9.1.7/PKG-INFO` & `qctrl_open_controls-9.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qctrl-open-controls
-Version: 9.1.7
+Version: 9.1.8
 Summary: Q-CTRL Python Open Controls
 Home-page: https://q-ctrl.com
 License: Apache-2.0
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
```

