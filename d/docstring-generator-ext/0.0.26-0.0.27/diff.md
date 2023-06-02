# Comparing `tmp/docstring_generator_ext-0.0.26.tar.gz` & `tmp/docstring_generator_ext-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docstring_generator_ext-0.0.26.tar", max compression
+gzip compressed data, was "docstring_generator_ext-0.0.27.tar", max compression
```

## Comparing `docstring_generator_ext-0.0.26.tar` & `docstring_generator_ext-0.0.27.tar`

### file list

```diff
@@ -1,255 +1,255 @@
--rw-r--r--   0        0        0      212 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/README.md
--rw-r--r--   0        0        0      797 2023-05-27 21:00:15.813005 docstring_generator_ext-0.0.26/pyproject.toml
--rw-r--r--   0        0        0     1395 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/CMakeLists.txt
--rw-r--r--   0        0        0    17478 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/docstringFormat.cpp
--rw-r--r--   0        0        0    16321 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/docstringFormat.hpp
--rw-r--r--   0        0        0        0 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/__init__.py
--rw-r--r--   0        0        0     1271 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/.appveyor.yml
--rw-r--r--   0        0        0      996 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/.clang-format
--rw-r--r--   0        0        0     2605 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/.clang-tidy
--rw-r--r--   0        0        0     2196 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/.cmake-format.yaml
--rw-r--r--   0        0        0     1308 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/.codespell-ignore-lines
--rw-r--r--   0        0        0       18 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/.gitattributes
--rw-r--r--   0        0        0      182 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/.github/CODEOWNERS
--rw-r--r--   0        0        0    15271 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0     2561 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0        0        0      328 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      162 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/.github/dependabot.yml
--rw-r--r--   0        0        0      116 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/.github/labeler.yml
--rw-r--r--   0        0        0       50 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/.github/labeler_merged.yml
--rw-r--r--   0        0        0      668 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/.github/matchers/pylint.json
--rw-r--r--   0        0        0      645 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/.github/pull_request_template.md
--rw-r--r--   0        0        0    32023 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2127 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/.github/workflows/configure.yml
--rw-r--r--   0        0        0     1447 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/.github/workflows/format.yml
--rw-r--r--   0        0        0      559 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/.github/workflows/labeler.yml
--rw-r--r--   0        0        0     2558 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/.github/workflows/pip.yml
--rw-r--r--   0        0        0     2865 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/.github/workflows/upstream.yml
--rw-r--r--   0        0        0      512 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/.gitignore
--rw-r--r--   0        0        0     4330 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/.pre-commit-config.yaml
--rw-r--r--   0        0        0       62 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/.readthedocs.yml
--rw-r--r--   0        0        0    11883 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/CMakeLists.txt
--rw-r--r--   0        0        0     1684 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/LICENSE
--rw-r--r--   0        0        0      235 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/MANIFEST.in
--rw-r--r--   0        0        0     7686 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/README.rst
--rw-r--r--   0        0        0        0 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/__init__.py
--rw-r--r--   0        0        0      607 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/Doxyfile
--rw-r--r--   0        0        0       37 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/_static/css/custom.css
--rw-r--r--   0        0        0     3937 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/cast/chrono.rst
--rw-r--r--   0        0        0     3429 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/cast/custom.rst
--rw-r--r--   0        0        0    14283 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/cast/eigen.rst
--rw-r--r--   0        0        0     3889 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/cast/functional.rst
--rw-r--r--   0        0        0     1556 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/cast/index.rst
--rw-r--r--   0        0        0    12371 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/cast/overview.rst
--rw-r--r--   0        0        0     9586 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/cast/stl.rst
--rw-r--r--   0        0        0     8863 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/cast/strings.rst
--rw-r--r--   0        0        0    47796 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/classes.rst
--rw-r--r--   0        0        0     8453 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/embedding.rst
--rw-r--r--   0        0        0    17796 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/exceptions.rst
--rw-r--r--   0        0        0    26729 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/functions.rst
--rw-r--r--   0        0        0    15651 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/misc.rst
--rw-r--r--   0        0        0      278 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/pycpp/index.rst
--rw-r--r--   0        0        0    17161 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/pycpp/numpy.rst
--rw-r--r--   0        0        0     9030 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/pycpp/object.rst
--rw-r--r--   0        0        0     5710 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/pycpp/utilities.rst
--rw-r--r--   0        0        0     6377 2023-05-27 20:39:34.534200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/smart_ptrs.rst
--rw-r--r--   0        0        0     9240 2023-05-27 20:39:34.538200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/basics.rst
--rw-r--r--   0        0        0     2856 2023-05-27 20:39:34.538200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/benchmark.py
--rw-r--r--   0        0        0     3168 2023-05-27 20:39:34.538200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/benchmark.rst
--rw-r--r--   0        0        0   115476 2023-05-27 20:39:34.538200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/changelog.rst
--rw-r--r--   0        0        0    16380 2023-05-27 20:39:34.538200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/classes.rst
--rw-r--r--   0        0        0      273 2023-05-27 20:39:34.538200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/cmake/index.rst
--rw-r--r--   0        0        0    25777 2023-05-27 20:39:34.538200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/compiling.rst
--rw-r--r--   0        0        0    11558 2023-05-27 20:39:34.538200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/conf.py
--rw-r--r--   0        0        0    13177 2023-05-27 20:39:34.538200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/faq.rst
--rw-r--r--   0        0        0      613 2023-05-27 20:39:34.538200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/index.rst
--rw-r--r--   0        0        0     3277 2023-05-27 20:39:34.538200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/installing.rst
--rw-r--r--   0        0        0     3079 2023-05-27 20:39:34.538200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/limitations.rst
--rw-r--r--   0        0        0    61034 2023-05-27 20:39:34.538200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/pybind11-logo.png
--rw-r--r--   0        0        0    44653 2023-05-27 20:39:34.538200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/pybind11_vs_boost_python1.png
--rw-r--r--   0        0        0    87708 2023-05-27 20:39:34.538200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/pybind11_vs_boost_python1.svg
--rw-r--r--   0        0        0    41121 2023-05-27 20:39:34.538200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/pybind11_vs_boost_python2.png
--rw-r--r--   0        0        0    85853 2023-05-27 20:39:34.538200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/pybind11_vs_boost_python2.svg
--rw-r--r--   0        0        0     2647 2023-05-27 20:39:34.538200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/reference.rst
--rw-r--r--   0        0        0     4414 2023-05-27 20:39:34.538200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/release.rst
--rw-r--r--   0        0        0      149 2023-05-27 20:39:34.538200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/requirements.txt
--rw-r--r--   0        0        0    23489 2023-05-27 20:39:34.538200 docstring_generator_ext-0.0.26/src/extern/pybind11/docs/upgrade.rst
--rw-r--r--   0        0        0    23959 2023-05-27 20:39:34.538200 docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/attr.h
--rw-r--r--   0        0        0     7069 2023-05-27 20:39:34.538200 docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0        0        0    65660 2023-05-27 20:39:34.538200 docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/cast.h
--rw-r--r--   0        0        0     8458 2023-05-27 20:39:34.542200 docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/chrono.h
--rw-r--r--   0        0        0      120 2023-05-27 20:39:34.542200 docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/common.h
--rw-r--r--   0        0        0     2096 2023-05-27 20:39:34.542200 docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/complex.h
--rw-r--r--   0        0        0    28518 2023-05-27 20:39:34.542200 docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0        0        0    52930 2023-05-27 20:39:34.542200 docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0        0        0     5491 2023-05-27 20:39:34.542200 docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0        0        0    17869 2023-05-27 20:39:34.542200 docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0        0        0    26305 2023-05-27 20:39:34.542200 docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0        0        0    42613 2023-05-27 20:39:34.542200 docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0        0        0     1625 2023-05-27 20:39:34.542200 docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0        0        0    31450 2023-05-27 20:39:34.542200 docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/eigen/matrix.h
--rw-r--r--   0        0        0    18140 2023-05-27 20:39:34.542200 docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/eigen/tensor.h
--rw-r--r--   0        0        0      316 2023-05-27 20:39:34.542200 docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/eigen.h
--rw-r--r--   0        0        0    13471 2023-05-27 20:39:34.542200 docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/embed.h
--rw-r--r--   0        0        0     4731 2023-05-27 20:39:34.542200 docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/eval.h
--rw-r--r--   0        0        0     5002 2023-05-27 20:39:34.542200 docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/functional.h
--rw-r--r--   0        0        0     8262 2023-05-27 20:39:34.542200 docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/gil.h
--rw-r--r--   0        0        0     8862 2023-05-27 20:39:34.542200 docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/iostream.h
--rw-r--r--   0        0        0    79416 2023-05-27 20:39:34.542200 docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/numpy.h
--rw-r--r--   0        0        0     9103 2023-05-27 20:39:34.542200 docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/operators.h
--rw-r--r--   0        0        0     2734 2023-05-27 20:39:34.542200 docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/options.h
--rw-r--r--   0        0        0   126420 2023-05-27 20:39:34.542200 docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0        0        0    94641 2023-05-27 20:39:34.542200 docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/pytypes.h
--rw-r--r--   0        0        0     4185 2023-05-27 20:39:34.542200 docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0        0        0    15337 2023-05-27 20:39:34.542200 docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/stl.h
--rw-r--r--   0        0        0    29747 2023-05-27 20:39:34.542200 docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/stl_bind.h
--rw-r--r--   0        0        0     2765 2023-05-27 20:39:34.542200 docstring_generator_ext-0.0.26/src/extern/pybind11/noxfile.py
--rw-r--r--   0        0        0      414 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/pybind11/__init__.py
--rw-r--r--   0        0        0     1544 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/pybind11/__main__.py
--rw-r--r--   0        0        0      228 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/pybind11/_version.py
--rw-r--r--   0        0        0     1226 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/pybind11/commands.py
--rw-r--r--   0        0        0        0 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/pybind11/py.typed
--rw-r--r--   0        0        0    17650 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/pybind11/setup_helpers.py
--rw-r--r--   0        0        0     1261 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/pyproject.toml
--rw-r--r--   0        0        0     1618 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/setup.cfg
--rw-r--r--   0        0        0     4877 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/setup.py
--rw-r--r--   0        0        0    21509 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/CMakeLists.txt
--rw-r--r--   0        0        0     5876 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/conftest.py
--rw-r--r--   0        0        0    11736 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/constructor_stats.h
--rw-r--r--   0        0        0     3578 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/cross_module_gil_utils.cpp
--rw-r--r--   0        0        0     1776 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/cross_module_interleaved_error_already_set.cpp
--rw-r--r--   0        0        0      396 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/eigen_tensor_avoid_stl_array.cpp
--rw-r--r--   0        0        0      940 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/env.py
--rw-r--r--   0        0        0        0 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/extra_python_package/pytest.ini
--rw-r--r--   0        0        0     8294 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/extra_python_package/test_files.py
--rw-r--r--   0        0        0        0 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/extra_setuptools/pytest.ini
--rw-r--r--   0        0        0     4153 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/extra_setuptools/test_setuphelper.py
--rw-r--r--   0        0        0     2847 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/local_bindings.h
--rw-r--r--   0        0        0     5743 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/object.h
--rw-r--r--   0        0        0     6264 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/pybind11_cross_module_tests.cpp
--rw-r--r--   0        0        0     4517 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/pybind11_tests.cpp
--rw-r--r--   0        0        0     2685 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/pybind11_tests.h
--rw-r--r--   0        0        0      768 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/pytest.ini
--rw-r--r--   0        0        0      600 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/requirements.txt
--rw-r--r--   0        0        0      855 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_async.cpp
--rw-r--r--   0        0        0      534 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_async.py
--rw-r--r--   0        0        0     8567 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_buffers.cpp
--rw-r--r--   0        0        0     4841 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_buffers.py
--rw-r--r--   0        0        0    16025 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_builtin_casters.cpp
--rw-r--r--   0        0        0    17245 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_builtin_casters.py
--rw-r--r--   0        0        0     4118 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_call_policies.cpp
--rw-r--r--   0        0        0     6549 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_call_policies.py
--rw-r--r--   0        0        0    10858 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_callbacks.cpp
--rw-r--r--   0        0        0     6246 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_callbacks.py
--rw-r--r--   0        0        0     3370 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_chrono.cpp
--rw-r--r--   0        0        0     5691 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_chrono.py
--rw-r--r--   0        0        0    24874 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_class.cpp
--rw-r--r--   0        0        0    14814 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_class.py
--rw-r--r--   0        0        0     2639 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_cmake_build/CMakeLists.txt
--rw-r--r--   0        0        0      673 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_cmake_build/embed.cpp
--rw-r--r--   0        0        0     1171 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
--rw-r--r--   0        0        0     1293 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
--rw-r--r--   0        0        0     1685 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
--rw-r--r--   0        0        0      152 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_cmake_build/main.cpp
--rw-r--r--   0        0        0     1353 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
--rw-r--r--   0        0        0     1163 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
--rw-r--r--   0        0        0     1368 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
--rw-r--r--   0        0        0      198 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_cmake_build/test.py
--rw-r--r--   0        0        0     3831 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_const_name.cpp
--rw-r--r--   0        0        0      589 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_const_name.py
--rw-r--r--   0        0        0     5615 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_constants_and_functions.cpp
--rw-r--r--   0        0        0     1498 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_constants_and_functions.py
--rw-r--r--   0        0        0    10886 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_copy_move.cpp
--rw-r--r--   0        0        0     4796 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_copy_move.py
--rw-r--r--   0        0        0     7280 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_custom_type_casters.cpp
--rw-r--r--   0        0        0     3985 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_custom_type_casters.py
--rw-r--r--   0        0        0     1259 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_custom_type_setup.cpp
--rw-r--r--   0        0        0     1089 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_custom_type_setup.py
--rw-r--r--   0        0        0     4557 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_docstring_options.cpp
--rw-r--r--   0        0        0     2423 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_docstring_options.py
--rw-r--r--   0        0        0    19350 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_eigen_matrix.cpp
--rw-r--r--   0        0        0    28867 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_eigen_matrix.py
--rw-r--r--   0        0        0      473 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_eigen_tensor.cpp
--rw-r--r--   0        0        0    10590 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_eigen_tensor.inl
--rw-r--r--   0        0        0     9450 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_eigen_tensor.py
--rw-r--r--   0        0        0     1798 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_embed/CMakeLists.txt
--rw-r--r--   0        0        0     1315 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_embed/catch.cpp
--rw-r--r--   0        0        0      543 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_embed/external_module.cpp
--rw-r--r--   0        0        0    16535 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_embed/test_interpreter.cpp
--rw-r--r--   0        0        0      237 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_embed/test_interpreter.py
--rw-r--r--   0        0        0      275 2023-05-27 20:39:34.546200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_embed/test_trampoline.py
--rw-r--r--   0        0        0     5722 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_enum.cpp
--rw-r--r--   0        0        0     8903 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_enum.py
--rw-r--r--   0        0        0     3168 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_eval.cpp
--rw-r--r--   0        0        0     1143 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_eval.py
--rw-r--r--   0        0        0      119 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_eval_call.py
--rw-r--r--   0        0        0    11904 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_exceptions.cpp
--rw-r--r--   0        0        0      399 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_exceptions.h
--rw-r--r--   0        0        0    12774 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_exceptions.py
--rw-r--r--   0        0        0    18155 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_factory_constructors.cpp
--rw-r--r--   0        0        0    16519 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_factory_constructors.py
--rw-r--r--   0        0        0     5311 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_gil_scoped.cpp
--rw-r--r--   0        0        0     8540 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_gil_scoped.py
--rw-r--r--   0        0        0     3960 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_iostream.cpp
--rw-r--r--   0        0        0     7286 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_iostream.py
--rw-r--r--   0        0        0     9444 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_kwargs_and_defaults.cpp
--rw-r--r--   0        0        0    13757 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_kwargs_and_defaults.py
--rw-r--r--   0        0        0     4401 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_local_bindings.cpp
--rw-r--r--   0        0        0     8054 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_local_bindings.py
--rw-r--r--   0        0        0    21388 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_methods_and_attributes.cpp
--rw-r--r--   0        0        0    18134 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_methods_and_attributes.py
--rw-r--r--   0        0        0     4121 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_modules.cpp
--rw-r--r--   0        0        0     4209 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_modules.py
--rw-r--r--   0        0        0    12305 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_multiple_inheritance.cpp
--rw-r--r--   0        0        0    11874 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_multiple_inheritance.py
--rw-r--r--   0        0        0    19861 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_numpy_array.cpp
--rw-r--r--   0        0        0    20356 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_numpy_array.py
--rw-r--r--   0        0        0    21114 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_numpy_dtypes.cpp
--rw-r--r--   0        0        0    14394 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_numpy_dtypes.py
--rw-r--r--   0        0        0     4487 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_numpy_vectorize.cpp
--rw-r--r--   0        0        0     9686 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_numpy_vectorize.py
--rw-r--r--   0        0        0     2777 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_opaque_types.cpp
--rw-r--r--   0        0        0     1847 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_opaque_types.py
--rw-r--r--   0        0        0     9132 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_operator_overloading.cpp
--rw-r--r--   0        0        0     4332 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_operator_overloading.py
--rw-r--r--   0        0        0     6719 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_pickling.cpp
--rw-r--r--   0        0        0     2720 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_pickling.py
--rw-r--r--   0        0        0    30750 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_pytypes.cpp
--rw-r--r--   0        0        0    23630 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_pytypes.py
--rw-r--r--   0        0        0    21153 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_sequences_and_iterators.cpp
--rw-r--r--   0        0        0     8021 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_sequences_and_iterators.py
--rw-r--r--   0        0        0    18898 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_smart_ptr.cpp
--rw-r--r--   0        0        0     9530 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_smart_ptr.py
--rw-r--r--   0        0        0    21587 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_stl.cpp
--rw-r--r--   0        0        0    12235 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_stl.py
--rw-r--r--   0        0        0     4622 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_stl_binders.cpp
--rw-r--r--   0        0        0     9174 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_stl_binders.py
--rw-r--r--   0        0        0     4617 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_tagbased_polymorphic.cpp
--rw-r--r--   0        0        0      741 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_tagbased_polymorphic.py
--rw-r--r--   0        0        0     1855 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_thread.cpp
--rw-r--r--   0        0        0      826 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_thread.py
--rw-r--r--   0        0        0      603 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_union.cpp
--rw-r--r--   0        0        0      148 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_union.py
--rw-r--r--   0        0        0    22991 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_virtual_functions.cpp
--rw-r--r--   0        0        0    12919 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_virtual_functions.py
--rw-r--r--   0        0        0     3226 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/valgrind-numpy-scipy.supp
--rw-r--r--   0        0        0     2657 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tests/valgrind-python.supp
--rw-r--r--   0        0        0     2350 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tools/FindCatch.cmake
--rw-r--r--   0        0        0     3105 2023-05-27 20:39:34.550200 docstring_generator_ext-0.0.26/src/extern/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0        0        0    11190 2023-05-27 20:39:34.554200 docstring_generator_ext-0.0.26/src/extern/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0        0        0      817 2023-05-27 20:39:34.554200 docstring_generator_ext-0.0.26/src/extern/pybind11/tools/JoinPaths.cmake
--rwxr-xr-x   0        0        0     1423 2023-05-27 20:39:34.554200 docstring_generator_ext-0.0.26/src/extern/pybind11/tools/check-style.sh
--rw-r--r--   0        0        0      952 2023-05-27 20:39:34.554200 docstring_generator_ext-0.0.26/src/extern/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0        0        0     1040 2023-05-27 20:39:34.554200 docstring_generator_ext-0.0.26/src/extern/pybind11/tools/codespell_ignore_lines_from_errors.py
--rw-r--r--   0        0        0     1031 2023-05-27 20:39:34.554200 docstring_generator_ext-0.0.26/src/extern/pybind11/tools/libsize.py
--rwxr-xr-x   0        0        0     1311 2023-05-27 20:39:34.554200 docstring_generator_ext-0.0.26/src/extern/pybind11/tools/make_changelog.py
--rw-r--r--   0        0        0      196 2023-05-27 20:39:34.554200 docstring_generator_ext-0.0.26/src/extern/pybind11/tools/pybind11.pc.in
--rw-r--r--   0        0        0    13981 2023-05-27 20:39:34.554200 docstring_generator_ext-0.0.26/src/extern/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0        0        0     6930 2023-05-27 20:39:34.554200 docstring_generator_ext-0.0.26/src/extern/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0        0        0     8960 2023-05-27 20:39:34.554200 docstring_generator_ext-0.0.26/src/extern/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0        0        0     8337 2023-05-27 20:39:34.554200 docstring_generator_ext-0.0.26/src/extern/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0        0        0       94 2023-05-27 20:39:34.554200 docstring_generator_ext-0.0.26/src/extern/pybind11/tools/pyproject.toml
--rw-r--r--   0        0        0     2104 2023-05-27 20:39:34.554200 docstring_generator_ext-0.0.26/src/extern/pybind11/tools/setup_global.py.in
--rw-r--r--   0        0        0     1234 2023-05-27 20:39:34.554200 docstring_generator_ext-0.0.26/src/extern/pybind11/tools/setup_main.py.in
--rw-r--r--   0        0        0       97 2023-05-27 20:39:34.554200 docstring_generator_ext-0.0.26/src/main.cpp
--rw-r--r--   0        0        0     1202 1970-01-01 00:00:00.000000 docstring_generator_ext-0.0.26/PKG-INFO
+-rw-r--r--   0        0        0      212 2023-06-02 06:58:02.286426 docstring_generator_ext-0.0.27/README.md
+-rw-r--r--   0        0        0      842 2023-06-02 07:16:39.902413 docstring_generator_ext-0.0.27/pyproject.toml
+-rw-r--r--   0        0        0     1395 2023-06-02 06:58:02.286426 docstring_generator_ext-0.0.27/src/CMakeLists.txt
+-rw-r--r--   0        0        0    17478 2023-06-02 06:58:02.286426 docstring_generator_ext-0.0.27/src/docstringFormat.cpp
+-rw-r--r--   0        0        0    16321 2023-06-02 06:58:02.286426 docstring_generator_ext-0.0.27/src/docstringFormat.hpp
+-rw-r--r--   0        0        0        0 2023-06-02 06:58:02.286426 docstring_generator_ext-0.0.27/src/extern/__init__.py
+-rw-r--r--   0        0        0     1271 2023-06-02 06:58:02.286426 docstring_generator_ext-0.0.27/src/extern/pybind11/.appveyor.yml
+-rw-r--r--   0        0        0      996 2023-06-02 06:58:02.286426 docstring_generator_ext-0.0.27/src/extern/pybind11/.clang-format
+-rw-r--r--   0        0        0     2605 2023-06-02 06:58:02.286426 docstring_generator_ext-0.0.27/src/extern/pybind11/.clang-tidy
+-rw-r--r--   0        0        0     2196 2023-06-02 06:58:02.286426 docstring_generator_ext-0.0.27/src/extern/pybind11/.cmake-format.yaml
+-rw-r--r--   0        0        0     1308 2023-06-02 06:58:02.286426 docstring_generator_ext-0.0.27/src/extern/pybind11/.codespell-ignore-lines
+-rw-r--r--   0        0        0       18 2023-06-02 06:58:02.286426 docstring_generator_ext-0.0.27/src/extern/pybind11/.gitattributes
+-rw-r--r--   0        0        0      182 2023-06-02 06:58:02.286426 docstring_generator_ext-0.0.27/src/extern/pybind11/.github/CODEOWNERS
+-rw-r--r--   0        0        0    15271 2023-06-02 06:58:02.286426 docstring_generator_ext-0.0.27/src/extern/pybind11/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2561 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0      328 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      162 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/.github/dependabot.yml
+-rw-r--r--   0        0        0      116 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/.github/labeler.yml
+-rw-r--r--   0        0        0       50 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/.github/labeler_merged.yml
+-rw-r--r--   0        0        0      668 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      645 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/.github/pull_request_template.md
+-rw-r--r--   0        0        0    32023 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2127 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/.github/workflows/configure.yml
+-rw-r--r--   0        0        0     1447 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/.github/workflows/format.yml
+-rw-r--r--   0        0        0      559 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/.github/workflows/labeler.yml
+-rw-r--r--   0        0        0     2558 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/.github/workflows/pip.yml
+-rw-r--r--   0        0        0     2865 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/.github/workflows/upstream.yml
+-rw-r--r--   0        0        0      512 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/.gitignore
+-rw-r--r--   0        0        0     4330 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       62 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/.readthedocs.yml
+-rw-r--r--   0        0        0    11883 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/CMakeLists.txt
+-rw-r--r--   0        0        0     1684 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/LICENSE
+-rw-r--r--   0        0        0      235 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/MANIFEST.in
+-rw-r--r--   0        0        0     7686 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/README.rst
+-rw-r--r--   0        0        0        0 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/__init__.py
+-rw-r--r--   0        0        0      607 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/Doxyfile
+-rw-r--r--   0        0        0       37 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/_static/css/custom.css
+-rw-r--r--   0        0        0     3937 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/cast/chrono.rst
+-rw-r--r--   0        0        0     3429 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/cast/custom.rst
+-rw-r--r--   0        0        0    14283 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/cast/eigen.rst
+-rw-r--r--   0        0        0     3889 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/cast/functional.rst
+-rw-r--r--   0        0        0     1556 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/cast/index.rst
+-rw-r--r--   0        0        0    12371 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/cast/overview.rst
+-rw-r--r--   0        0        0     9586 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/cast/stl.rst
+-rw-r--r--   0        0        0     8863 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/cast/strings.rst
+-rw-r--r--   0        0        0    47796 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/classes.rst
+-rw-r--r--   0        0        0     8453 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/embedding.rst
+-rw-r--r--   0        0        0    17796 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/exceptions.rst
+-rw-r--r--   0        0        0    26729 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/functions.rst
+-rw-r--r--   0        0        0    15651 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/misc.rst
+-rw-r--r--   0        0        0      278 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/pycpp/index.rst
+-rw-r--r--   0        0        0    17161 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/pycpp/numpy.rst
+-rw-r--r--   0        0        0     9030 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/pycpp/object.rst
+-rw-r--r--   0        0        0     5710 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/pycpp/utilities.rst
+-rw-r--r--   0        0        0     6377 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/smart_ptrs.rst
+-rw-r--r--   0        0        0     9240 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/basics.rst
+-rw-r--r--   0        0        0     2856 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/benchmark.py
+-rw-r--r--   0        0        0     3168 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/benchmark.rst
+-rw-r--r--   0        0        0   115476 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/changelog.rst
+-rw-r--r--   0        0        0    16380 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/classes.rst
+-rw-r--r--   0        0        0      273 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/cmake/index.rst
+-rw-r--r--   0        0        0    25777 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/compiling.rst
+-rw-r--r--   0        0        0    11558 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/conf.py
+-rw-r--r--   0        0        0    13177 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/faq.rst
+-rw-r--r--   0        0        0      613 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/index.rst
+-rw-r--r--   0        0        0     3277 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/installing.rst
+-rw-r--r--   0        0        0     3079 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/limitations.rst
+-rw-r--r--   0        0        0    61034 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/pybind11-logo.png
+-rw-r--r--   0        0        0    44653 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/pybind11_vs_boost_python1.png
+-rw-r--r--   0        0        0    87708 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/pybind11_vs_boost_python1.svg
+-rw-r--r--   0        0        0    41121 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/pybind11_vs_boost_python2.png
+-rw-r--r--   0        0        0    85853 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/pybind11_vs_boost_python2.svg
+-rw-r--r--   0        0        0     2647 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/reference.rst
+-rw-r--r--   0        0        0     4414 2023-06-02 06:58:02.310426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/release.rst
+-rw-r--r--   0        0        0      149 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/requirements.txt
+-rw-r--r--   0        0        0    23489 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/docs/upgrade.rst
+-rw-r--r--   0        0        0    23959 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/attr.h
+-rw-r--r--   0        0        0     7069 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0        0        0    65660 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/cast.h
+-rw-r--r--   0        0        0     8458 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0        0        0      120 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/common.h
+-rw-r--r--   0        0        0     2096 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/complex.h
+-rw-r--r--   0        0        0    28518 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0        0        0    52930 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0        0        0     5491 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0        0        0    17869 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0        0        0    26305 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0        0        0    42613 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0        0        0     1625 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0        0        0    31450 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/eigen/matrix.h
+-rw-r--r--   0        0        0    18140 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/eigen/tensor.h
+-rw-r--r--   0        0        0      316 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0        0        0    13471 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/embed.h
+-rw-r--r--   0        0        0     4731 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/eval.h
+-rw-r--r--   0        0        0     5002 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/functional.h
+-rw-r--r--   0        0        0     8262 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/gil.h
+-rw-r--r--   0        0        0     8862 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0        0        0    79416 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0        0        0     9103 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/operators.h
+-rw-r--r--   0        0        0     2734 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/options.h
+-rw-r--r--   0        0        0   126420 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0        0        0    94641 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/pytypes.h
+-rw-r--r--   0        0        0     4185 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0        0        0    15337 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/stl.h
+-rw-r--r--   0        0        0    29747 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/stl_bind.h
+-rw-r--r--   0        0        0     2765 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/noxfile.py
+-rw-r--r--   0        0        0      414 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/pybind11/__init__.py
+-rw-r--r--   0        0        0     1544 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/pybind11/__main__.py
+-rw-r--r--   0        0        0      228 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/pybind11/_version.py
+-rw-r--r--   0        0        0     1226 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/pybind11/commands.py
+-rw-r--r--   0        0        0        0 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/pybind11/py.typed
+-rw-r--r--   0        0        0    17650 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/pybind11/setup_helpers.py
+-rw-r--r--   0        0        0     1261 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/pyproject.toml
+-rw-r--r--   0        0        0     1618 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/setup.cfg
+-rw-r--r--   0        0        0     4877 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/setup.py
+-rw-r--r--   0        0        0    21509 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/CMakeLists.txt
+-rw-r--r--   0        0        0     5876 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/conftest.py
+-rw-r--r--   0        0        0    11736 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/constructor_stats.h
+-rw-r--r--   0        0        0     3578 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/cross_module_gil_utils.cpp
+-rw-r--r--   0        0        0     1776 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/cross_module_interleaved_error_already_set.cpp
+-rw-r--r--   0        0        0      396 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/eigen_tensor_avoid_stl_array.cpp
+-rw-r--r--   0        0        0      940 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/env.py
+-rw-r--r--   0        0        0        0 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/extra_python_package/pytest.ini
+-rw-r--r--   0        0        0     8294 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/extra_python_package/test_files.py
+-rw-r--r--   0        0        0        0 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/extra_setuptools/pytest.ini
+-rw-r--r--   0        0        0     4153 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/extra_setuptools/test_setuphelper.py
+-rw-r--r--   0        0        0     2847 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/local_bindings.h
+-rw-r--r--   0        0        0     5743 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/object.h
+-rw-r--r--   0        0        0     6264 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/pybind11_cross_module_tests.cpp
+-rw-r--r--   0        0        0     4517 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/pybind11_tests.cpp
+-rw-r--r--   0        0        0     2685 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/pybind11_tests.h
+-rw-r--r--   0        0        0      768 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/pytest.ini
+-rw-r--r--   0        0        0      600 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/requirements.txt
+-rw-r--r--   0        0        0      855 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_async.cpp
+-rw-r--r--   0        0        0      534 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_async.py
+-rw-r--r--   0        0        0     8567 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_buffers.cpp
+-rw-r--r--   0        0        0     4841 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_buffers.py
+-rw-r--r--   0        0        0    16025 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_builtin_casters.cpp
+-rw-r--r--   0        0        0    17245 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_builtin_casters.py
+-rw-r--r--   0        0        0     4118 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_call_policies.cpp
+-rw-r--r--   0        0        0     6549 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_call_policies.py
+-rw-r--r--   0        0        0    10858 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_callbacks.cpp
+-rw-r--r--   0        0        0     6246 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_callbacks.py
+-rw-r--r--   0        0        0     3370 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_chrono.cpp
+-rw-r--r--   0        0        0     5691 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_chrono.py
+-rw-r--r--   0        0        0    24874 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_class.cpp
+-rw-r--r--   0        0        0    14814 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_class.py
+-rw-r--r--   0        0        0     2639 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_cmake_build/CMakeLists.txt
+-rw-r--r--   0        0        0      673 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_cmake_build/embed.cpp
+-rw-r--r--   0        0        0     1171 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+-rw-r--r--   0        0        0     1293 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+-rw-r--r--   0        0        0     1685 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+-rw-r--r--   0        0        0      152 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_cmake_build/main.cpp
+-rw-r--r--   0        0        0     1353 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+-rw-r--r--   0        0        0     1163 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+-rw-r--r--   0        0        0     1368 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+-rw-r--r--   0        0        0      198 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_cmake_build/test.py
+-rw-r--r--   0        0        0     3831 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_const_name.cpp
+-rw-r--r--   0        0        0      589 2023-06-02 06:58:02.314426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_const_name.py
+-rw-r--r--   0        0        0     5615 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_constants_and_functions.cpp
+-rw-r--r--   0        0        0     1498 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_constants_and_functions.py
+-rw-r--r--   0        0        0    10886 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_copy_move.cpp
+-rw-r--r--   0        0        0     4796 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_copy_move.py
+-rw-r--r--   0        0        0     7280 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_custom_type_casters.cpp
+-rw-r--r--   0        0        0     3985 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_custom_type_casters.py
+-rw-r--r--   0        0        0     1259 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_custom_type_setup.cpp
+-rw-r--r--   0        0        0     1089 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_custom_type_setup.py
+-rw-r--r--   0        0        0     4557 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_docstring_options.cpp
+-rw-r--r--   0        0        0     2423 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_docstring_options.py
+-rw-r--r--   0        0        0    19350 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_eigen_matrix.cpp
+-rw-r--r--   0        0        0    28867 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_eigen_matrix.py
+-rw-r--r--   0        0        0      473 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_eigen_tensor.cpp
+-rw-r--r--   0        0        0    10590 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_eigen_tensor.inl
+-rw-r--r--   0        0        0     9450 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_eigen_tensor.py
+-rw-r--r--   0        0        0     1798 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_embed/CMakeLists.txt
+-rw-r--r--   0        0        0     1315 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_embed/catch.cpp
+-rw-r--r--   0        0        0      543 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_embed/external_module.cpp
+-rw-r--r--   0        0        0    16535 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_embed/test_interpreter.cpp
+-rw-r--r--   0        0        0      237 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_embed/test_interpreter.py
+-rw-r--r--   0        0        0      275 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_embed/test_trampoline.py
+-rw-r--r--   0        0        0     5722 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_enum.cpp
+-rw-r--r--   0        0        0     8903 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_enum.py
+-rw-r--r--   0        0        0     3168 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_eval.cpp
+-rw-r--r--   0        0        0     1143 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_eval.py
+-rw-r--r--   0        0        0      119 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_eval_call.py
+-rw-r--r--   0        0        0    11904 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_exceptions.cpp
+-rw-r--r--   0        0        0      399 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_exceptions.h
+-rw-r--r--   0        0        0    12774 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_exceptions.py
+-rw-r--r--   0        0        0    18155 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_factory_constructors.cpp
+-rw-r--r--   0        0        0    16519 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_factory_constructors.py
+-rw-r--r--   0        0        0     5311 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_gil_scoped.cpp
+-rw-r--r--   0        0        0     8540 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_gil_scoped.py
+-rw-r--r--   0        0        0     3960 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_iostream.cpp
+-rw-r--r--   0        0        0     7286 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_iostream.py
+-rw-r--r--   0        0        0     9444 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_kwargs_and_defaults.cpp
+-rw-r--r--   0        0        0    13757 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_kwargs_and_defaults.py
+-rw-r--r--   0        0        0     4401 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_local_bindings.cpp
+-rw-r--r--   0        0        0     8054 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_local_bindings.py
+-rw-r--r--   0        0        0    21388 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_methods_and_attributes.cpp
+-rw-r--r--   0        0        0    18134 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_methods_and_attributes.py
+-rw-r--r--   0        0        0     4121 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_modules.cpp
+-rw-r--r--   0        0        0     4209 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_modules.py
+-rw-r--r--   0        0        0    12305 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_multiple_inheritance.cpp
+-rw-r--r--   0        0        0    11874 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_multiple_inheritance.py
+-rw-r--r--   0        0        0    19861 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_numpy_array.cpp
+-rw-r--r--   0        0        0    20356 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_numpy_array.py
+-rw-r--r--   0        0        0    21114 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_numpy_dtypes.cpp
+-rw-r--r--   0        0        0    14394 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_numpy_dtypes.py
+-rw-r--r--   0        0        0     4487 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_numpy_vectorize.cpp
+-rw-r--r--   0        0        0     9686 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_numpy_vectorize.py
+-rw-r--r--   0        0        0     2777 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_opaque_types.cpp
+-rw-r--r--   0        0        0     1847 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_opaque_types.py
+-rw-r--r--   0        0        0     9132 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_operator_overloading.cpp
+-rw-r--r--   0        0        0     4332 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_operator_overloading.py
+-rw-r--r--   0        0        0     6719 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_pickling.cpp
+-rw-r--r--   0        0        0     2720 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_pickling.py
+-rw-r--r--   0        0        0    30750 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_pytypes.cpp
+-rw-r--r--   0        0        0    23630 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_pytypes.py
+-rw-r--r--   0        0        0    21153 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_sequences_and_iterators.cpp
+-rw-r--r--   0        0        0     8021 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_sequences_and_iterators.py
+-rw-r--r--   0        0        0    18898 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_smart_ptr.cpp
+-rw-r--r--   0        0        0     9530 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_smart_ptr.py
+-rw-r--r--   0        0        0    21587 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_stl.cpp
+-rw-r--r--   0        0        0    12235 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_stl.py
+-rw-r--r--   0        0        0     4622 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_stl_binders.cpp
+-rw-r--r--   0        0        0     9174 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_stl_binders.py
+-rw-r--r--   0        0        0     4617 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_tagbased_polymorphic.cpp
+-rw-r--r--   0        0        0      741 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_tagbased_polymorphic.py
+-rw-r--r--   0        0        0     1855 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_thread.cpp
+-rw-r--r--   0        0        0      826 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_thread.py
+-rw-r--r--   0        0        0      603 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_union.cpp
+-rw-r--r--   0        0        0      148 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_union.py
+-rw-r--r--   0        0        0    22991 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_virtual_functions.cpp
+-rw-r--r--   0        0        0    12919 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_virtual_functions.py
+-rw-r--r--   0        0        0     3226 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/valgrind-numpy-scipy.supp
+-rw-r--r--   0        0        0     2657 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tests/valgrind-python.supp
+-rw-r--r--   0        0        0     2350 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0        0        0     3105 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0        0        0    11190 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0        0        0      817 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tools/JoinPaths.cmake
+-rwxr-xr-x   0        0        0     1423 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tools/check-style.sh
+-rw-r--r--   0        0        0      952 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0        0        0     1040 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-r--r--   0        0        0     1031 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tools/libsize.py
+-rwxr-xr-x   0        0        0     1311 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tools/make_changelog.py
+-rw-r--r--   0        0        0      196 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tools/pybind11.pc.in
+-rw-r--r--   0        0        0    13981 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0        0        0     6930 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0        0        0     8960 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0        0        0     8337 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0        0        0       94 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tools/pyproject.toml
+-rw-r--r--   0        0        0     2104 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tools/setup_global.py.in
+-rw-r--r--   0        0        0     1234 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/extern/pybind11/tools/setup_main.py.in
+-rw-r--r--   0        0        0       97 2023-06-02 06:58:02.318426 docstring_generator_ext-0.0.27/src/main.cpp
+-rw-r--r--   0        0        0     1103 1970-01-01 00:00:00.000000 docstring_generator_ext-0.0.27/PKG-INFO
```

### Comparing `docstring_generator_ext-0.0.26/pyproject.toml` & `docstring_generator_ext-0.0.27/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [tool.poetry]
 name = "docstring_generator_ext"
-version = "0.0.26"
+version = "0.0.27"
 description = "Auto generate docstring from type-hints."
 authors = ["FelixTheC <felixeisenmenger@gmx.net>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/FelixTheC/docstring_generator"
 packages = [{include = "src"}]
 classifiers=[
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Utilities",
     "Topic :: Software Development :: Documentation",
     "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.8"
 pybind11 = "^2.8"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `docstring_generator_ext-0.0.26/src/CMakeLists.txt` & `docstring_generator_ext-0.0.27/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/docstringFormat.cpp` & `docstring_generator_ext-0.0.27/src/docstringFormat.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/docstringFormat.hpp` & `docstring_generator_ext-0.0.27/src/docstringFormat.hpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/.appveyor.yml` & `docstring_generator_ext-0.0.27/src/extern/pybind11/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/.clang-format` & `docstring_generator_ext-0.0.27/src/extern/pybind11/.clang-format`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/.clang-tidy` & `docstring_generator_ext-0.0.27/src/extern/pybind11/.clang-tidy`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/.cmake-format.yaml` & `docstring_generator_ext-0.0.27/src/extern/pybind11/.cmake-format.yaml`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/.codespell-ignore-lines` & `docstring_generator_ext-0.0.27/src/extern/pybind11/.codespell-ignore-lines`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/.github/CONTRIBUTING.md` & `docstring_generator_ext-0.0.27/src/extern/pybind11/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml` & `docstring_generator_ext-0.0.27/src/extern/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/.github/matchers/pylint.json` & `docstring_generator_ext-0.0.27/src/extern/pybind11/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/.github/pull_request_template.md` & `docstring_generator_ext-0.0.27/src/extern/pybind11/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/.github/workflows/ci.yml` & `docstring_generator_ext-0.0.27/src/extern/pybind11/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/.github/workflows/configure.yml` & `docstring_generator_ext-0.0.27/src/extern/pybind11/.github/workflows/configure.yml`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/.github/workflows/format.yml` & `docstring_generator_ext-0.0.27/src/extern/pybind11/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/.github/workflows/labeler.yml` & `docstring_generator_ext-0.0.27/src/extern/pybind11/.github/workflows/labeler.yml`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/.github/workflows/pip.yml` & `docstring_generator_ext-0.0.27/src/extern/pybind11/.github/workflows/pip.yml`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/.github/workflows/upstream.yml` & `docstring_generator_ext-0.0.27/src/extern/pybind11/.github/workflows/upstream.yml`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/.gitignore` & `docstring_generator_ext-0.0.27/src/extern/pybind11/.gitignore`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/.pre-commit-config.yaml` & `docstring_generator_ext-0.0.27/src/extern/pybind11/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/CMakeLists.txt` & `docstring_generator_ext-0.0.27/src/extern/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/LICENSE` & `docstring_generator_ext-0.0.27/src/extern/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/README.rst` & `docstring_generator_ext-0.0.27/src/extern/pybind11/README.rst`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/Doxyfile` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/cast/chrono.rst` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/cast/chrono.rst`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/cast/custom.rst` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/cast/custom.rst`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/cast/eigen.rst` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/cast/eigen.rst`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/cast/functional.rst` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/cast/functional.rst`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/cast/index.rst` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/cast/index.rst`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/cast/overview.rst` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/cast/overview.rst`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/cast/stl.rst` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/cast/stl.rst`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/cast/strings.rst` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/cast/strings.rst`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/classes.rst` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/classes.rst`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/embedding.rst` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/embedding.rst`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/exceptions.rst` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/exceptions.rst`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/functions.rst` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/functions.rst`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/misc.rst` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/misc.rst`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/pycpp/numpy.rst` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/pycpp/numpy.rst`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/pycpp/object.rst` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/pycpp/object.rst`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/pycpp/utilities.rst` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/pycpp/utilities.rst`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/advanced/smart_ptrs.rst` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/advanced/smart_ptrs.rst`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/basics.rst` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/basics.rst`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/benchmark.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/benchmark.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/benchmark.rst` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/benchmark.rst`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/changelog.rst` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/classes.rst` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/classes.rst`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/compiling.rst` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/compiling.rst`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/conf.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/conf.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/faq.rst` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/index.rst` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/index.rst`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/installing.rst` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/limitations.rst` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/limitations.rst`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/pybind11-logo.png` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/pybind11-logo.png`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/pybind11_vs_boost_python1.png` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/pybind11_vs_boost_python1.png`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/pybind11_vs_boost_python1.svg` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/pybind11_vs_boost_python1.svg`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/pybind11_vs_boost_python2.png` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/pybind11_vs_boost_python2.png`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/pybind11_vs_boost_python2.svg` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/pybind11_vs_boost_python2.svg`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/reference.rst` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/release.rst` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/release.rst`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/docs/upgrade.rst` & `docstring_generator_ext-0.0.27/src/extern/pybind11/docs/upgrade.rst`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/attr.h` & `docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/buffer_info.h` & `docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/cast.h` & `docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/chrono.h` & `docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/complex.h` & `docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/detail/class.h` & `docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/detail/common.h` & `docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/detail/descr.h` & `docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/detail/init.h` & `docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/detail/internals.h` & `docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/detail/type_caster_base.h` & `docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/detail/typeid.h` & `docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/eigen/matrix.h` & `docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/eigen/matrix.h`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/eigen/tensor.h` & `docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/eigen/tensor.h`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/embed.h` & `docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/eval.h` & `docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/functional.h` & `docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/gil.h` & `docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/iostream.h` & `docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/numpy.h` & `docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/operators.h` & `docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/options.h` & `docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/pybind11.h` & `docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/pytypes.h` & `docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/stl/filesystem.h` & `docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/stl.h` & `docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/include/pybind11/stl_bind.h` & `docstring_generator_ext-0.0.27/src/extern/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/noxfile.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/noxfile.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/pybind11/__main__.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/pybind11/__main__.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/pybind11/commands.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/pybind11/commands.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/pybind11/setup_helpers.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/pybind11/setup_helpers.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/pyproject.toml` & `docstring_generator_ext-0.0.27/src/extern/pybind11/pyproject.toml`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/setup.cfg` & `docstring_generator_ext-0.0.27/src/extern/pybind11/setup.cfg`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/setup.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/setup.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/CMakeLists.txt` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/conftest.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/constructor_stats.h` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/constructor_stats.h`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/cross_module_gil_utils.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/cross_module_gil_utils.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/cross_module_interleaved_error_already_set.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/cross_module_interleaved_error_already_set.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/env.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/env.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/extra_python_package/test_files.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/extra_python_package/test_files.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/extra_setuptools/test_setuphelper.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/extra_setuptools/test_setuphelper.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/local_bindings.h` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/local_bindings.h`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/object.h` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/object.h`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/pybind11_cross_module_tests.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/pybind11_cross_module_tests.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/pybind11_tests.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/pybind11_tests.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/pybind11_tests.h` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/pybind11_tests.h`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/pytest.ini` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/pytest.ini`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/requirements.txt` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/requirements.txt`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_async.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_async.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_async.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_buffers.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_buffers.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_buffers.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_builtin_casters.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_builtin_casters.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_builtin_casters.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_builtin_casters.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_call_policies.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_call_policies.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_call_policies.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_call_policies.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_callbacks.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_callbacks.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_callbacks.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_chrono.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_chrono.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_chrono.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_chrono.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_class.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_class.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_class.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_cmake_build/CMakeLists.txt` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_cmake_build/embed.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_cmake_build/embed.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_const_name.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_const_name.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_const_name.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_const_name.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_constants_and_functions.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_constants_and_functions.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_constants_and_functions.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_constants_and_functions.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_copy_move.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_copy_move.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_copy_move.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_copy_move.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_custom_type_casters.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_custom_type_casters.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_custom_type_casters.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_custom_type_casters.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_custom_type_setup.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_custom_type_setup.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_custom_type_setup.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_custom_type_setup.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_docstring_options.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_docstring_options.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_docstring_options.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_docstring_options.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_eigen_matrix.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_eigen_matrix.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_eigen_matrix.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_eigen_matrix.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_eigen_tensor.inl` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_eigen_tensor.inl`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_eigen_tensor.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_eigen_tensor.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_embed/CMakeLists.txt` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_embed/catch.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_embed/catch.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_embed/external_module.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_embed/external_module.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_embed/test_interpreter.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_embed/test_interpreter.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_enum.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_enum.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_enum.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_eval.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_eval.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_eval.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_exceptions.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_exceptions.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_exceptions.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_factory_constructors.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_factory_constructors.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_factory_constructors.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_factory_constructors.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_gil_scoped.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_gil_scoped.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_gil_scoped.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_gil_scoped.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_iostream.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_iostream.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_iostream.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_iostream.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_kwargs_and_defaults.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_kwargs_and_defaults.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_kwargs_and_defaults.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_kwargs_and_defaults.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_local_bindings.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_local_bindings.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_local_bindings.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_local_bindings.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_methods_and_attributes.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_methods_and_attributes.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_methods_and_attributes.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_methods_and_attributes.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_modules.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_modules.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_modules.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_multiple_inheritance.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_multiple_inheritance.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_multiple_inheritance.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_multiple_inheritance.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_numpy_array.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_numpy_array.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_numpy_array.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_numpy_array.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_numpy_dtypes.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_numpy_dtypes.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_numpy_dtypes.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_numpy_dtypes.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_numpy_vectorize.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_numpy_vectorize.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_numpy_vectorize.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_numpy_vectorize.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_opaque_types.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_opaque_types.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_opaque_types.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_opaque_types.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_operator_overloading.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_operator_overloading.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_operator_overloading.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_operator_overloading.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_pickling.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_pickling.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_pickling.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_pytypes.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_pytypes.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_pytypes.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_pytypes.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_sequences_and_iterators.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_sequences_and_iterators.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_sequences_and_iterators.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_sequences_and_iterators.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_smart_ptr.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_smart_ptr.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_smart_ptr.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_smart_ptr.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_stl.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_stl.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_stl.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_stl.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_stl_binders.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_stl_binders.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_stl_binders.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_stl_binders.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_tagbased_polymorphic.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_tagbased_polymorphic.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_tagbased_polymorphic.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_tagbased_polymorphic.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_thread.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_thread.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_thread.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_union.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_union.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_virtual_functions.cpp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_virtual_functions.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/test_virtual_functions.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/test_virtual_functions.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/valgrind-numpy-scipy.supp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/valgrind-numpy-scipy.supp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tests/valgrind-python.supp` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tests/valgrind-python.supp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tools/FindCatch.cmake` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tools/FindEigen3.cmake` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tools/FindPythonLibsNew.cmake` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tools/JoinPaths.cmake` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tools/check-style.sh` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tools/cmake_uninstall.cmake.in` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tools/codespell_ignore_lines_from_errors.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tools/codespell_ignore_lines_from_errors.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tools/libsize.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tools/make_changelog.py` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tools/pybind11Common.cmake` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tools/pybind11Config.cmake.in` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tools/pybind11NewTools.cmake` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tools/pybind11Tools.cmake` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tools/setup_global.py.in` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/extern/pybind11/tools/setup_main.py.in` & `docstring_generator_ext-0.0.27/src/extern/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/PKG-INFO` & `docstring_generator_ext-0.0.27/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: docstring-generator-ext
-Version: 0.0.26
+Version: 0.0.27
 Summary: Auto generate docstring from type-hints.
 Home-page: https://github.com/FelixTheC/docstring_generator
 License: MIT
 Author: FelixTheC
 Author-email: felixeisenmenger@gmx.net
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: pybind11 (>=2.8,<3.0)
 Project-URL: Repository, https://github.com/FelixTheC/docstring_generator
 Description-Content-Type: text/markdown
```

