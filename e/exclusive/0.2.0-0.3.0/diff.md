# Comparing `tmp/exclusive-0.2.0.tar.gz` & `tmp/exclusive-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exclusive-0.2.0.tar", last modified: Tue Aug 23 01:36:11 2022, max compression
+gzip compressed data, was "exclusive-0.3.0.tar", last modified: Fri Jun  2 05:33:31 2023, max compression
```

## Comparing `exclusive-0.2.0.tar` & `exclusive-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-08-23 01:36:11.072958 exclusive-0.2.0/
--rw-rw-rw-   0        0        0     1093 2022-05-24 18:04:26.000000 exclusive-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     7305 2022-08-23 01:36:11.073349 exclusive-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     6673 2022-07-27 05:43:25.000000 exclusive-0.2.0/README.rst
--rw-rw-rw-   0        0        0     1070 2022-07-17 04:52:36.000000 exclusive-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-08-23 01:36:11.075544 exclusive-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-08-23 01:36:11.063686 exclusive-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2022-08-23 01:36:11.065207 exclusive-0.2.0/src/exclusive/
--rw-rw-rw-   0        0        0      111 2022-05-24 18:04:26.000000 exclusive-0.2.0/src/exclusive/__init__.py
--rw-rw-rw-   0        0        0     6231 2022-07-17 07:26:56.000000 exclusive-0.2.0/src/exclusive/exclusive.py
-drwxrwxrwx   0        0        0        0 2022-08-23 01:36:11.072958 exclusive-0.2.0/src/exclusive.egg-info/
--rw-rw-rw-   0        0        0     7305 2022-08-23 01:36:10.000000 exclusive-0.2.0/src/exclusive.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2022-08-23 01:36:11.000000 exclusive-0.2.0/src/exclusive.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-23 01:36:10.000000 exclusive-0.2.0/src/exclusive.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      181 2022-08-23 01:36:10.000000 exclusive-0.2.0/src/exclusive.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-08-23 01:36:11.000000 exclusive-0.2.0/src/exclusive.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 05:33:31.687009 exclusive-0.3.0/
+-rw-rw-rw-   0        0        0     1093 2022-05-24 18:04:26.000000 exclusive-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     7690 2023-06-02 05:33:31.687009 exclusive-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7058 2023-06-01 19:21:33.000000 exclusive-0.3.0/README.rst
+-rw-rw-rw-   0        0        0     1071 2023-06-01 19:22:42.000000 exclusive-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-02 05:33:31.687009 exclusive-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-02 05:33:31.671004 exclusive-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-02 05:33:31.675507 exclusive-0.3.0/src/exclusive/
+-rw-rw-rw-   0        0        0      111 2022-05-24 18:04:26.000000 exclusive-0.3.0/src/exclusive/__init__.py
+-rw-rw-rw-   0        0        0     6231 2022-07-17 07:26:56.000000 exclusive-0.3.0/src/exclusive/exclusive.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:33:31.686009 exclusive-0.3.0/src/exclusive.egg-info/
+-rw-rw-rw-   0        0        0     7690 2023-06-02 05:33:31.000000 exclusive-0.3.0/src/exclusive.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-06-02 05:33:31.000000 exclusive-0.3.0/src/exclusive.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 05:33:31.000000 exclusive-0.3.0/src/exclusive.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      182 2023-06-02 05:33:31.000000 exclusive-0.3.0/src/exclusive.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-02 05:33:31.000000 exclusive-0.3.0/src/exclusive.egg-info/top_level.txt
```

### Comparing `exclusive-0.2.0/LICENSE` & `exclusive-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exclusive-0.2.0/PKG-INFO` & `exclusive-0.3.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: exclusive
-Version: 0.2.0
-Summary: Data structure for representing secret shares of byte vectors based on bitwise XOR, designed for use within secure multi-party computation (MPC) protocol implementations.
-Author: Andrei Lapets
-Author-email: a@lapets.io
-License: MIT
-Project-URL: Repository, https://github.com/nthparty/exclusive
-Project-URL: Documentation, https://exclusive.readthedocs.io
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: docs
-Provides-Extra: test
-Provides-Extra: lint
-Provides-Extra: coveralls
-Provides-Extra: publish
-License-File: LICENSE
-
 =========
 exclusive
 =========
 
 Data structure for representing secret shares of byte vectors based on bitwise XOR, designed for use within secure multi-party computation (MPC) protocol implementations.
 
 |pypi| |readthedocs| |actions| |coveralls|
@@ -46,113 +28,145 @@
 .. |bytes| replace:: ``bytes``
 .. _bytes: https://docs.python.org/3/library/stdtypes.html#bytes
 
 This library provides a data structure and methods that make it possible to work with *n*-out-of-*n* XOR-based `secret shares <https://en.wikipedia.org/wiki/Secret_sharing>`__ of bytes-like objects within secure multi-party computation (MPC) protocol implementations. Secret shares are represented using instances of class derived from |bytes|_, and functions are provided both for splitting bytes-like objects into shares and for reconstructing |bytes|_ objects from shares.
 
 Installation and Usage
 ----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/exclusive>`__::
+This library is available as a `package on PyPI <https://pypi.org/project/exclusive>`__:
+
+.. code-block:: bash
 
     python -m pip install exclusive
 
-The library can be imported in the usual ways::
+The library can be imported in the usual ways:
+
+.. code-block:: python
 
     import exclusive
     from exclusive import *
 
 Examples
 ^^^^^^^^
-This library makes it possible to concisely construct multiple XOR-based secret shares from a bytes-like object::
+This library makes it possible to concisely construct multiple XOR-based secret shares from a bytes-like object:
+
+.. code-block:: python
 
     >>> from exclusive import shares, xor
     >>> (a, b) = shares(bytes([1, 2, 3]))
     >>> (c, d) = shares(bytes([4, 5, 6]))
     >>> ((a ^ c) ^ (b ^ d)) == xor([bytes([1, 2, 3]), bytes([4, 5, 6])])
     True
 
-The number of shares can be specified explicitly (the default is two shares)::
+The number of shares can be specified explicitly (the default is two shares):
+
+.. code-block:: python
 
     >>> (r, s, t) = shares(bytes([1, 2, 3]), quantity=3)
 
 .. |xor| replace:: ``xor``
-.. _xor: https://exclusive.readthedocs.io/en/0.2.0/_source/exclusive.html#exclusive.exclusive.xor
+.. _xor: https://exclusive.readthedocs.io/en/0.3.0/_source/exclusive.html#exclusive.exclusive.xor
 
 .. |sum| replace:: ``sum``
 .. _sum: https://docs.python.org/3/library/functions.html#sum
 
-For convenience, an |xor|_ operator that is analogous to Python's built-in |sum|_ function is provided::
+For convenience, an |xor|_ operator that is analogous to Python's built-in |sum|_ function is provided:
+
+.. code-block:: python
 
     >>> xor([bytes([1, 2, 3]), bytes([4, 5, 6])]).hex()
     '050705
 
 .. |share| replace:: ``share``
-.. _share: https://exclusive.readthedocs.io/en/0.2.0/_source/exclusive.html#exclusive.exclusive.share
+.. _share: https://exclusive.readthedocs.io/en/0.3.0/_source/exclusive.html#exclusive.exclusive.share
+
+The |share|_ class is derived from the |bytes|_ class. Thus, all methods, operators, and functions that operate on bytes-like objects are supported for |share|_ objects. The |xor|_ operator provided by the library relies on Python's `built-in exclusive or operator <https://docs.python.org/3/reference/expressions.html#binary-bitwise-operations>`__ and can be used for concise reconstruction of values from a collection of secret shares:
 
-The |share|_ class is derived from the |bytes|_ class. Thus, all methods, operators, and functions that operate on bytes-like objects are supported for |share|_ objects. The |xor|_ operator provided by the library relies on Python's `built-in exclusive or operator <https://docs.python.org/3/reference/expressions.html#binary-bitwise-operations>`__ and can be used for concise reconstruction of values from a collection of secret shares::
+.. code-block:: python
 
     >>> xor([r, s, t]) == bytes([1, 2, 3])
     True
 
-In addition, conversion methods for Base64 strings are included to support encoding and decoding of |share|_ objects::
+In addition, conversion methods for Base64 strings are included to support encoding and decoding of |share|_ objects:
+
+.. code-block:: python
 
     >>> share.from_base64('HgEA').hex()
     '1e0100'
     >>> [s.to_base64() for s in shares(bytes([1, 2, 3]))]
     ['mB6G', 'mRyF']
 
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
 
     python src/exclusive/exclusive.py -v
 
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
 
     python -m pip install .[lint]
     python -m pylint src/exclusive
 
 Contributions
 ^^^^^^^^^^^^^
 In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/exclusive>`__ for this library.
 
 Versioning
 ^^^^^^^^^^
 The version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
 
 Publishing
 ^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/exclusive>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
+This library can be published as a `package on PyPI <https://pypi.org/project/exclusive>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
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

### Comparing `exclusive-0.2.0/pyproject.toml` & `exclusive-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "exclusive"
-version = "0.2.0"
+version = "0.3.0"
 description = """\
     Data structure for representing secret shares of byte vectors based on \
     bitwise XOR, designed for use within secure multi-party computation (MPC) \
     protocol implementations.\
     """
 license = {text = "MIT"}
 authors = [
@@ -21,29 +21,29 @@
 [project.optional-dependencies]
 docs = [
     "toml~=0.10.2",
     "sphinx~=4.2.0",
     "sphinx-rtd-theme~=1.0.0"
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
 addopts = "--doctest-modules --ignore=docs --cov=exclusive --cov-report term-missing"
```

### Comparing `exclusive-0.2.0/src/exclusive/exclusive.py` & `exclusive-0.3.0/src/exclusive/exclusive.py`

 * *Files identical despite different names*

### Comparing `exclusive-0.2.0/src/exclusive.egg-info/PKG-INFO` & `exclusive-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exclusive
-Version: 0.2.0
+Version: 0.3.0
 Summary: Data structure for representing secret shares of byte vectors based on bitwise XOR, designed for use within secure multi-party computation (MPC) protocol implementations.
 Author: Andrei Lapets
 Author-email: a@lapets.io
 License: MIT
 Project-URL: Repository, https://github.com/nthparty/exclusive
 Project-URL: Documentation, https://exclusive.readthedocs.io
 Requires-Python: >=3.7
@@ -46,113 +46,145 @@
 .. |bytes| replace:: ``bytes``
 .. _bytes: https://docs.python.org/3/library/stdtypes.html#bytes
 
 This library provides a data structure and methods that make it possible to work with *n*-out-of-*n* XOR-based `secret shares <https://en.wikipedia.org/wiki/Secret_sharing>`__ of bytes-like objects within secure multi-party computation (MPC) protocol implementations. Secret shares are represented using instances of class derived from |bytes|_, and functions are provided both for splitting bytes-like objects into shares and for reconstructing |bytes|_ objects from shares.
 
 Installation and Usage
 ----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/exclusive>`__::
+This library is available as a `package on PyPI <https://pypi.org/project/exclusive>`__:
+
+.. code-block:: bash
 
     python -m pip install exclusive
 
-The library can be imported in the usual ways::
+The library can be imported in the usual ways:
+
+.. code-block:: python
 
     import exclusive
     from exclusive import *
 
 Examples
 ^^^^^^^^
-This library makes it possible to concisely construct multiple XOR-based secret shares from a bytes-like object::
+This library makes it possible to concisely construct multiple XOR-based secret shares from a bytes-like object:
+
+.. code-block:: python
 
     >>> from exclusive import shares, xor
     >>> (a, b) = shares(bytes([1, 2, 3]))
     >>> (c, d) = shares(bytes([4, 5, 6]))
     >>> ((a ^ c) ^ (b ^ d)) == xor([bytes([1, 2, 3]), bytes([4, 5, 6])])
     True
 
-The number of shares can be specified explicitly (the default is two shares)::
+The number of shares can be specified explicitly (the default is two shares):
+
+.. code-block:: python
 
     >>> (r, s, t) = shares(bytes([1, 2, 3]), quantity=3)
 
 .. |xor| replace:: ``xor``
-.. _xor: https://exclusive.readthedocs.io/en/0.2.0/_source/exclusive.html#exclusive.exclusive.xor
+.. _xor: https://exclusive.readthedocs.io/en/0.3.0/_source/exclusive.html#exclusive.exclusive.xor
 
 .. |sum| replace:: ``sum``
 .. _sum: https://docs.python.org/3/library/functions.html#sum
 
-For convenience, an |xor|_ operator that is analogous to Python's built-in |sum|_ function is provided::
+For convenience, an |xor|_ operator that is analogous to Python's built-in |sum|_ function is provided:
+
+.. code-block:: python
 
     >>> xor([bytes([1, 2, 3]), bytes([4, 5, 6])]).hex()
     '050705
 
 .. |share| replace:: ``share``
-.. _share: https://exclusive.readthedocs.io/en/0.2.0/_source/exclusive.html#exclusive.exclusive.share
+.. _share: https://exclusive.readthedocs.io/en/0.3.0/_source/exclusive.html#exclusive.exclusive.share
+
+The |share|_ class is derived from the |bytes|_ class. Thus, all methods, operators, and functions that operate on bytes-like objects are supported for |share|_ objects. The |xor|_ operator provided by the library relies on Python's `built-in exclusive or operator <https://docs.python.org/3/reference/expressions.html#binary-bitwise-operations>`__ and can be used for concise reconstruction of values from a collection of secret shares:
 
-The |share|_ class is derived from the |bytes|_ class. Thus, all methods, operators, and functions that operate on bytes-like objects are supported for |share|_ objects. The |xor|_ operator provided by the library relies on Python's `built-in exclusive or operator <https://docs.python.org/3/reference/expressions.html#binary-bitwise-operations>`__ and can be used for concise reconstruction of values from a collection of secret shares::
+.. code-block:: python
 
     >>> xor([r, s, t]) == bytes([1, 2, 3])
     True
 
-In addition, conversion methods for Base64 strings are included to support encoding and decoding of |share|_ objects::
+In addition, conversion methods for Base64 strings are included to support encoding and decoding of |share|_ objects:
+
+.. code-block:: python
 
     >>> share.from_base64('HgEA').hex()
     '1e0100'
     >>> [s.to_base64() for s in shares(bytes([1, 2, 3]))]
     ['mB6G', 'mRyF']
 
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
 
     python src/exclusive/exclusive.py -v
 
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
 
     python -m pip install .[lint]
     python -m pylint src/exclusive
 
 Contributions
 ^^^^^^^^^^^^^
 In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/exclusive>`__ for this library.
 
 Versioning
 ^^^^^^^^^^
 The version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
 
 Publishing
 ^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/exclusive>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
+This library can be published as a `package on PyPI <https://pypi.org/project/exclusive>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
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

