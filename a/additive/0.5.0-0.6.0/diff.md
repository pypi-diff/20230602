# Comparing `tmp/additive-0.5.0.tar.gz` & `tmp/additive-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "additive-0.5.0.tar", last modified: Tue Aug 23 01:37:36 2022, max compression
+gzip compressed data, was "additive-0.6.0.tar", last modified: Fri Jun  2 05:37:50 2023, max compression
```

## Comparing `additive-0.5.0.tar` & `additive-0.6.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-08-23 01:37:36.571284 additive-0.5.0/
--rw-rw-rw-   0        0        0     1093 2022-04-14 16:22:47.000000 additive-0.5.0/LICENSE
--rw-rw-rw-   0        0        0     6675 2022-08-23 01:37:36.571535 additive-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     6088 2022-07-27 05:44:03.000000 additive-0.5.0/README.rst
--rw-rw-rw-   0        0        0     1058 2022-07-17 07:30:55.000000 additive-0.5.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-08-23 01:37:36.571726 additive-0.5.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-08-23 01:37:36.550560 additive-0.5.0/src/
-drwxrwxrwx   0        0        0        0 2022-08-23 01:37:36.559888 additive-0.5.0/src/additive/
--rw-rw-rw-   0        0        0      104 2022-04-14 16:22:47.000000 additive-0.5.0/src/additive/__init__.py
--rw-rw-rw-   0        0        0    20038 2022-07-17 07:42:53.000000 additive-0.5.0/src/additive/additive.py
-drwxrwxrwx   0        0        0        0 2022-08-23 01:37:36.570535 additive-0.5.0/src/additive.egg-info/
--rw-rw-rw-   0        0        0     6675 2022-08-23 01:37:36.000000 additive-0.5.0/src/additive.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2022-08-23 01:37:36.000000 additive-0.5.0/src/additive.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-23 01:37:36.000000 additive-0.5.0/src/additive.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      214 2022-08-23 01:37:36.000000 additive-0.5.0/src/additive.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-08-23 01:37:36.000000 additive-0.5.0/src/additive.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 05:37:50.144641 additive-0.6.0/
+-rw-rw-rw-   0        0        0     1093 2022-10-06 21:17:14.000000 additive-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0     7060 2023-06-02 05:37:50.144641 additive-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6473 2023-06-02 03:53:11.000000 additive-0.6.0/README.rst
+-rw-rw-rw-   0        0        0     1059 2023-06-02 03:54:31.000000 additive-0.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-02 05:37:50.144641 additive-0.6.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-02 05:37:50.122287 additive-0.6.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-02 05:37:50.133031 additive-0.6.0/src/additive/
+-rw-rw-rw-   0        0        0      104 2022-10-06 21:17:14.000000 additive-0.6.0/src/additive/__init__.py
+-rw-rw-rw-   0        0        0    20038 2022-10-06 21:17:14.000000 additive-0.6.0/src/additive/additive.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:37:50.143641 additive-0.6.0/src/additive.egg-info/
+-rw-rw-rw-   0        0        0     7060 2023-06-02 05:37:50.000000 additive-0.6.0/src/additive.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-06-02 05:37:50.000000 additive-0.6.0/src/additive.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 05:37:50.000000 additive-0.6.0/src/additive.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      215 2023-06-02 05:37:50.000000 additive-0.6.0/src/additive.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-02 05:37:50.000000 additive-0.6.0/src/additive.egg-info/top_level.txt
```

### Comparing `additive-0.5.0/LICENSE` & `additive-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `additive-0.5.0/PKG-INFO` & `additive-0.6.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: additive
-Version: 0.5.0
+Version: 0.6.0
 Summary: Data structure for representing additive secret shares of integers, designed for use within secure MPC protocol implementations.
 Author: Andrei Lapets
 Author-email: a@lapets.io
 License: MIT
 Project-URL: Repository, https://github.com/nthparty/additive
 Project-URL: Documentation, https://additive.readthedocs.io
 Requires-Python: >=3.7
@@ -42,111 +42,143 @@
 
 Purpose
 -------
 This library provides a data structure and methods that make it possible work with *n*-out-of-*n* `additive secret shares <https://en.wikipedia.org/wiki/Secret_sharing>`__ of integers within secure multi-party computation (MPC) protocol implementations. Secret shares of signed and unsigned integers can be represented using elements from finite fields, with support currently limited to fields having a power-of-two order.
 
 Installation and Usage
 ----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/additive>`__::
+This library is available as a `package on PyPI <https://pypi.org/project/additive>`__:
+
+.. code-block:: bash
 
     python -m pip install additive
 
-The library can be imported in the usual ways::
+The library can be imported in the usual ways:
+
+.. code-block:: python
 
     import additive
     from additive import *
 
 Examples
 ^^^^^^^^
-This library makes it possible to concisely construct multiple secret shares from an integer::
+This library makes it possible to concisely construct multiple secret shares from an integer:
+
+.. code-block:: python
 
     >>> from additive import shares
     >>> (a, b) = shares(123)
     >>> (c, d) = shares(456)
     >>> ((a + c) + (b + d)).to_int()
     579
 
-It is possible to specify the exponent in the order of the finite field used to represent secret shares, as well as whether the encoding of the integer should support signed integers::
+It is possible to specify the exponent in the order of the finite field used to represent secret shares, as well as whether the encoding of the integer should support signed integers:
+
+.. code-block:: python
 
     >>> (s, t) = shares(-123, exponent=8, signed=True)
     >>> (s + t).to_int()
     -123
 
-The number of shares can be specified explicitly (the default is two shares)::
+The number of shares can be specified explicitly (the default is two shares):
+
+.. code-block:: python
 
     >>> (r, s, t) = shares(123, quantity=3)
 
 .. |share| replace:: ``share``
-.. _share: https://additive.readthedocs.io/en/0.5.0/_source/additive.html#additive.additive.share
+.. _share: https://additive.readthedocs.io/en/0.6.0/_source/additive.html#additive.additive.share
+
+The |share|_ data structure supports Python's built-in addition operators, enabling both operations on shares and concise reconstruction of values from a collection of shares:
 
-The |share|_ data structure supports Python's built-in addition operators, enabling both operations on shares and concise reconstruction of values from a collection of shares::
+.. code-block:: python
 
     >>> (r + s + t).to_int()
     123
     >>> sum([r, s, t]).to_int()
     123
 
-In addition, conversion methods for Base64 strings and bytes-like objects are included to support encoding and decoding of |share|_ objects::
+In addition, conversion methods for Base64 strings and bytes-like objects are included to support encoding and decoding of |share|_ objects:
+
+.. code-block:: python
 
     >>> from additive import share
     >>> share.from_base64('HgEA').to_bytes().hex()
     '1e0100'
     >>> [s.to_base64() for s in shares(123)]
     ['PvmKMG8=', 'PoJ1z5A=']
 
 Development
 -----------
-All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__::
+All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__:
+
+.. code-block:: bash
 
     python -m pip install .[docs,lint]
 
 Documentation
 ^^^^^^^^^^^^^
-The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__::
+The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__:
+
+.. code-block:: bash
 
     python -m pip install .[docs]
     cd docs
     sphinx-apidoc -f -E --templatedir=_templates -o _source .. && make html
 
 Testing and Conventions
 ^^^^^^^^^^^^^^^^^^^^^^^
-All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details)::
+All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details):
+
+.. code-block:: bash
 
     python -m pip install .[test]
     python -m pytest
 
-Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__::
+Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__:
+
+.. code-block:: bash
 
     python src/additive/additive.py -v
 
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
 
     python -m pip install .[lint]
     python -m pylint src/additive
 
 Contributions
 ^^^^^^^^^^^^^
 In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/additive>`__ for this library.
 
 Versioning
 ^^^^^^^^^^
 The version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
 
 Publishing
 ^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/additive>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
+This library can be published as a `package on PyPI <https://pypi.org/project/additive>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
+
+.. code-block:: bash
 
     python -m pip install .[publish]
 
-Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number)::
+Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number):
+
+.. code-block:: bash
 
     git tag ?.?.?
     git push origin ?.?.?
 
-Remove any old build/distribution files. Then, package the source into a distribution archive::
+Remove any old build/distribution files. Then, package the source into a distribution archive:
+
+.. code-block:: bash
 
     rm -rf build dist src/*.egg-info
     python -m build --sdist --wheel .
 
-Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__::
+Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__:
+
+.. code-block:: bash
 
     python -m twine upload dist/*
```

### Comparing `additive-0.5.0/README.rst` & `additive-0.6.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -24,111 +24,143 @@
 
 Purpose
 -------
 This library provides a data structure and methods that make it possible work with *n*-out-of-*n* `additive secret shares <https://en.wikipedia.org/wiki/Secret_sharing>`__ of integers within secure multi-party computation (MPC) protocol implementations. Secret shares of signed and unsigned integers can be represented using elements from finite fields, with support currently limited to fields having a power-of-two order.
 
 Installation and Usage
 ----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/additive>`__::
+This library is available as a `package on PyPI <https://pypi.org/project/additive>`__:
+
+.. code-block:: bash
 
     python -m pip install additive
 
-The library can be imported in the usual ways::
+The library can be imported in the usual ways:
+
+.. code-block:: python
 
     import additive
     from additive import *
 
 Examples
 ^^^^^^^^
-This library makes it possible to concisely construct multiple secret shares from an integer::
+This library makes it possible to concisely construct multiple secret shares from an integer:
+
+.. code-block:: python
 
     >>> from additive import shares
     >>> (a, b) = shares(123)
     >>> (c, d) = shares(456)
     >>> ((a + c) + (b + d)).to_int()
     579
 
-It is possible to specify the exponent in the order of the finite field used to represent secret shares, as well as whether the encoding of the integer should support signed integers::
+It is possible to specify the exponent in the order of the finite field used to represent secret shares, as well as whether the encoding of the integer should support signed integers:
+
+.. code-block:: python
 
     >>> (s, t) = shares(-123, exponent=8, signed=True)
     >>> (s + t).to_int()
     -123
 
-The number of shares can be specified explicitly (the default is two shares)::
+The number of shares can be specified explicitly (the default is two shares):
+
+.. code-block:: python
 
     >>> (r, s, t) = shares(123, quantity=3)
 
 .. |share| replace:: ``share``
-.. _share: https://additive.readthedocs.io/en/0.5.0/_source/additive.html#additive.additive.share
+.. _share: https://additive.readthedocs.io/en/0.6.0/_source/additive.html#additive.additive.share
+
+The |share|_ data structure supports Python's built-in addition operators, enabling both operations on shares and concise reconstruction of values from a collection of shares:
 
-The |share|_ data structure supports Python's built-in addition operators, enabling both operations on shares and concise reconstruction of values from a collection of shares::
+.. code-block:: python
 
     >>> (r + s + t).to_int()
     123
     >>> sum([r, s, t]).to_int()
     123
 
-In addition, conversion methods for Base64 strings and bytes-like objects are included to support encoding and decoding of |share|_ objects::
+In addition, conversion methods for Base64 strings and bytes-like objects are included to support encoding and decoding of |share|_ objects:
+
+.. code-block:: python
 
     >>> from additive import share
     >>> share.from_base64('HgEA').to_bytes().hex()
     '1e0100'
     >>> [s.to_base64() for s in shares(123)]
     ['PvmKMG8=', 'PoJ1z5A=']
 
 Development
 -----------
-All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__::
+All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__:
+
+.. code-block:: bash
 
     python -m pip install .[docs,lint]
 
 Documentation
 ^^^^^^^^^^^^^
-The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__::
+The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__:
+
+.. code-block:: bash
 
     python -m pip install .[docs]
     cd docs
     sphinx-apidoc -f -E --templatedir=_templates -o _source .. && make html
 
 Testing and Conventions
 ^^^^^^^^^^^^^^^^^^^^^^^
-All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details)::
+All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details):
+
+.. code-block:: bash
 
     python -m pip install .[test]
     python -m pytest
 
-Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__::
+Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__:
+
+.. code-block:: bash
 
     python src/additive/additive.py -v
 
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
 
     python -m pip install .[lint]
     python -m pylint src/additive
 
 Contributions
 ^^^^^^^^^^^^^
 In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/additive>`__ for this library.
 
 Versioning
 ^^^^^^^^^^
 The version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
 
 Publishing
 ^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/additive>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
+This library can be published as a `package on PyPI <https://pypi.org/project/additive>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
+
+.. code-block:: bash
 
     python -m pip install .[publish]
 
-Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number)::
+Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number):
+
+.. code-block:: bash
 
     git tag ?.?.?
     git push origin ?.?.?
 
-Remove any old build/distribution files. Then, package the source into a distribution archive::
+Remove any old build/distribution files. Then, package the source into a distribution archive:
+
+.. code-block:: bash
 
     rm -rf build dist src/*.egg-info
     python -m build --sdist --wheel .
 
-Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__::
+Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__:
+
+.. code-block:: bash
 
     python -m twine upload dist/*
```

### Comparing `additive-0.5.0/pyproject.toml` & `additive-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "additive"
-version = "0.5.0"
+version = "0.6.0"
 description = """\
     Data structure for representing additive secret shares of integers, \
     designed for use within secure MPC protocol implementations.\
     """
 license = {text = "MIT"}
 authors = [
     {name = "Andrei Lapets"},
@@ -21,29 +21,29 @@
 docs = [
     "toml~=0.10.2",
     "sphinx~=4.2.0",
     "sphinx-rtd-theme~=1.0.0",
     "sphinx-autodoc-typehints~=1.12.0"
 ]
 test = [
-    "pytest~=7.0",
-    "pytest-cov~=3.0"
+    "pytest~=7.2",
+    "pytest-cov~=4.0"
 ]
 lint = [
-    "pylint~=2.14.0"
+    "pylint~=2.17.0"
 ]
 coveralls = [
     "coveralls~=3.3.1"
 ]
 publish = [
-    "build~=0.8",
+    "build~=0.10",
     "twine~=4.0"
 ]
 
 [build-system]
 requires = [
-    "setuptools~=62.0"
+    "setuptools~=67.6"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules --ignore=docs --cov=additive --cov-report term-missing"
```

### Comparing `additive-0.5.0/src/additive/additive.py` & `additive-0.6.0/src/additive/additive.py`

 * *Files identical despite different names*

### Comparing `additive-0.5.0/src/additive.egg-info/PKG-INFO` & `additive-0.6.0/src/additive.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: additive
-Version: 0.5.0
+Version: 0.6.0
 Summary: Data structure for representing additive secret shares of integers, designed for use within secure MPC protocol implementations.
 Author: Andrei Lapets
 Author-email: a@lapets.io
 License: MIT
 Project-URL: Repository, https://github.com/nthparty/additive
 Project-URL: Documentation, https://additive.readthedocs.io
 Requires-Python: >=3.7
@@ -42,111 +42,143 @@
 
 Purpose
 -------
 This library provides a data structure and methods that make it possible work with *n*-out-of-*n* `additive secret shares <https://en.wikipedia.org/wiki/Secret_sharing>`__ of integers within secure multi-party computation (MPC) protocol implementations. Secret shares of signed and unsigned integers can be represented using elements from finite fields, with support currently limited to fields having a power-of-two order.
 
 Installation and Usage
 ----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/additive>`__::
+This library is available as a `package on PyPI <https://pypi.org/project/additive>`__:
+
+.. code-block:: bash
 
     python -m pip install additive
 
-The library can be imported in the usual ways::
+The library can be imported in the usual ways:
+
+.. code-block:: python
 
     import additive
     from additive import *
 
 Examples
 ^^^^^^^^
-This library makes it possible to concisely construct multiple secret shares from an integer::
+This library makes it possible to concisely construct multiple secret shares from an integer:
+
+.. code-block:: python
 
     >>> from additive import shares
     >>> (a, b) = shares(123)
     >>> (c, d) = shares(456)
     >>> ((a + c) + (b + d)).to_int()
     579
 
-It is possible to specify the exponent in the order of the finite field used to represent secret shares, as well as whether the encoding of the integer should support signed integers::
+It is possible to specify the exponent in the order of the finite field used to represent secret shares, as well as whether the encoding of the integer should support signed integers:
+
+.. code-block:: python
 
     >>> (s, t) = shares(-123, exponent=8, signed=True)
     >>> (s + t).to_int()
     -123
 
-The number of shares can be specified explicitly (the default is two shares)::
+The number of shares can be specified explicitly (the default is two shares):
+
+.. code-block:: python
 
     >>> (r, s, t) = shares(123, quantity=3)
 
 .. |share| replace:: ``share``
-.. _share: https://additive.readthedocs.io/en/0.5.0/_source/additive.html#additive.additive.share
+.. _share: https://additive.readthedocs.io/en/0.6.0/_source/additive.html#additive.additive.share
+
+The |share|_ data structure supports Python's built-in addition operators, enabling both operations on shares and concise reconstruction of values from a collection of shares:
 
-The |share|_ data structure supports Python's built-in addition operators, enabling both operations on shares and concise reconstruction of values from a collection of shares::
+.. code-block:: python
 
     >>> (r + s + t).to_int()
     123
     >>> sum([r, s, t]).to_int()
     123
 
-In addition, conversion methods for Base64 strings and bytes-like objects are included to support encoding and decoding of |share|_ objects::
+In addition, conversion methods for Base64 strings and bytes-like objects are included to support encoding and decoding of |share|_ objects:
+
+.. code-block:: python
 
     >>> from additive import share
     >>> share.from_base64('HgEA').to_bytes().hex()
     '1e0100'
     >>> [s.to_base64() for s in shares(123)]
     ['PvmKMG8=', 'PoJ1z5A=']
 
 Development
 -----------
-All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__::
+All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__:
+
+.. code-block:: bash
 
     python -m pip install .[docs,lint]
 
 Documentation
 ^^^^^^^^^^^^^
-The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__::
+The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__:
+
+.. code-block:: bash
 
     python -m pip install .[docs]
     cd docs
     sphinx-apidoc -f -E --templatedir=_templates -o _source .. && make html
 
 Testing and Conventions
 ^^^^^^^^^^^^^^^^^^^^^^^
-All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details)::
+All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details):
+
+.. code-block:: bash
 
     python -m pip install .[test]
     python -m pytest
 
-Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__::
+Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__:
+
+.. code-block:: bash
 
     python src/additive/additive.py -v
 
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
 
     python -m pip install .[lint]
     python -m pylint src/additive
 
 Contributions
 ^^^^^^^^^^^^^
 In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/additive>`__ for this library.
 
 Versioning
 ^^^^^^^^^^
 The version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
 
 Publishing
 ^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/additive>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
+This library can be published as a `package on PyPI <https://pypi.org/project/additive>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
+
+.. code-block:: bash
 
     python -m pip install .[publish]
 
-Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number)::
+Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number):
+
+.. code-block:: bash
 
     git tag ?.?.?
     git push origin ?.?.?
 
-Remove any old build/distribution files. Then, package the source into a distribution archive::
+Remove any old build/distribution files. Then, package the source into a distribution archive:
+
+.. code-block:: bash
 
     rm -rf build dist src/*.egg-info
     python -m build --sdist --wheel .
 
-Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__::
+Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__:
+
+.. code-block:: bash
 
     python -m twine upload dist/*
```

