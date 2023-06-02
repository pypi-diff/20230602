# Comparing `tmp/docstring_generator_ext-0.0.26.tar.gz` & `tmp/docstring_generator_ext-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docstring_generator_ext-0.0.26.tar", max compression
+gzip compressed data, was "docstring_generator_ext-0.0.28.tar", last modified: Fri Jun  2 08:53:06 2023, max compression
```

## Comparing `docstring_generator_ext-0.0.26.tar` & `docstring_generator_ext-0.0.28.tar`

### file list

```diff
@@ -1,255 +1,16 @@
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
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-06-02 08:53:06.579650 docstring_generator_ext-0.0.28/
+-rw-rw-r--   0 felix     (1000) felix     (1000)      902 2023-06-02 08:53:06.579650 docstring_generator_ext-0.0.28/PKG-INFO
+-rw-rw-r--   0 felix     (1000) felix     (1000)      212 2023-06-02 07:53:42.000000 docstring_generator_ext-0.0.28/README.md
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-06-02 08:53:06.579650 docstring_generator_ext-0.0.28/docstring_generator_ext.egg-info/
+-rw-rw-r--   0 felix     (1000) felix     (1000)      902 2023-06-02 08:53:06.000000 docstring_generator_ext-0.0.28/docstring_generator_ext.egg-info/PKG-INFO
+-rw-rw-r--   0 felix     (1000) felix     (1000)      361 2023-06-02 08:53:06.000000 docstring_generator_ext-0.0.28/docstring_generator_ext.egg-info/SOURCES.txt
+-rw-rw-r--   0 felix     (1000) felix     (1000)        1 2023-06-02 08:53:06.000000 docstring_generator_ext-0.0.28/docstring_generator_ext.egg-info/dependency_links.txt
+-rw-rw-r--   0 felix     (1000) felix     (1000)        1 2023-06-02 08:16:06.000000 docstring_generator_ext-0.0.28/docstring_generator_ext.egg-info/not-zip-safe
+-rw-rw-r--   0 felix     (1000) felix     (1000)       15 2023-06-02 08:53:06.000000 docstring_generator_ext-0.0.28/docstring_generator_ext.egg-info/requires.txt
+-rw-rw-r--   0 felix     (1000) felix     (1000)       24 2023-06-02 08:53:06.000000 docstring_generator_ext-0.0.28/docstring_generator_ext.egg-info/top_level.txt
+-rw-rw-r--   0 felix     (1000) felix     (1000)      864 2023-06-02 07:55:25.000000 docstring_generator_ext-0.0.28/pyproject.toml
+-rw-rw-r--   0 felix     (1000) felix     (1000)       38 2023-06-02 08:53:06.579650 docstring_generator_ext-0.0.28/setup.cfg
+-rw-rw-r--   0 felix     (1000) felix     (1000)     1959 2023-06-02 08:53:01.000000 docstring_generator_ext-0.0.28/setup.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-06-02 08:53:06.579650 docstring_generator_ext-0.0.28/src/
+-rw-rw-r--   0 felix     (1000) felix     (1000)    17478 2023-06-02 07:53:42.000000 docstring_generator_ext-0.0.28/src/docstringFormat.cpp
+-rw-rw-r--   0 felix     (1000) felix     (1000)    16324 2023-06-02 08:40:40.000000 docstring_generator_ext-0.0.28/src/docstringFormat.hpp
```

### Comparing `docstring_generator_ext-0.0.26/pyproject.toml` & `docstring_generator_ext-0.0.28/pyproject.toml`

 * *Files 21% similar despite different names*

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
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+requires = ["setuptools>=42", "wheel", "pybind11~=2.6.1"]
+build-backend = "setuptools.build_meta"
```

### Comparing `docstring_generator_ext-0.0.26/src/docstringFormat.cpp` & `docstring_generator_ext-0.0.28/src/docstringFormat.cpp`

 * *Files identical despite different names*

### Comparing `docstring_generator_ext-0.0.26/src/docstringFormat.hpp` & `docstring_generator_ext-0.0.28/src/docstringFormat.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,15 @@
         }
         
         return 0;
     }
     
     void update_descriptions(DocstringFormatStyle &formatStyle)
     {
-        for (int idx = 0; idx < args.size(); ++idx)
+        for (size_t idx = 0; idx < args.size(); ++idx)
         {
             size_t start_pos;
             
             if (formatStyle == DocstringFormatStyle::reST)
             {
                 start_pos = docstring.docstring.find(":param " + args[idx].name + ":");
             }
```

### Comparing `docstring_generator_ext-0.0.26/PKG-INFO` & `docstring_generator_ext-0.0.28/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,27 @@
 Metadata-Version: 2.1
-Name: docstring-generator-ext
-Version: 0.0.26
-Summary: Auto generate docstring from type-hints.
+Name: docstring_generator_ext
+Version: 0.0.28
+Summary: Generate Docstrings with type-hint information
 Home-page: https://github.com/FelixTheC/docstring_generator
-License: MIT
 Author: FelixTheC
-Author-email: felixeisenmenger@gmx.net
-Requires-Python: >=3.9,<4.0
+Author-email: fberndt87@gmail.com
+License: MIT
+Description: #### Versioning
+        - For the versions available, see the tags on this repository.
+        
+        ### Authors
+        - Felix Eisenmenger
+        
+        ### License
+        - This project is licensed under the MIT License - see the LICENSE.md file for details
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Utilities
+Classifier: Topic :: Software Development :: Documentation
 Classifier: Typing :: Typed
-Requires-Dist: pybind11 (>=2.8,<3.0)
-Project-URL: Repository, https://github.com/FelixTheC/docstring_generator
+Requires-Python: <=3.11
 Description-Content-Type: text/markdown
-
-#### Versioning
-- For the versions available, see the tags on this repository.
-
-### Authors
-- Felix Eisenmenger
-
-### License
-- This project is licensed under the MIT License - see the LICENSE.md file for details
-
+Provides-Extra: test
```

