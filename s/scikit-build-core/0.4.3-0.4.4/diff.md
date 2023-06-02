# Comparing `tmp/scikit_build_core-0.4.3.tar.gz` & `tmp/scikit_build_core-0.4.4.tar.gz`

## Comparing `scikit_build_core-0.4.3.tar` & `scikit_build_core-0.4.4.tar`

### file list

```diff
@@ -1,237 +1,237 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.git_archival.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.gitattributes
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.packit.yaml
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.readthedocs.yml
--rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/noxfile.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.distro/packit.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.distro/python-scikit-build-core.rpmlintrc
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.distro/python-scikit-build-core.spec
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.distro/.fmf/version
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.distro/plans/main.fmf.dist-git
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.distro/plans/rpmlint.fmf
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.distro/plans/smoke.fmf
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.distro/tests/rpmlint.fmf
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.distro/tests/smoke.fmf
--rw-r--r--   0        0        0     9969 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.github/codecov.yml
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.github/matchers/pylint.json
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.github/workflows/cd.yml
--rw-r--r--   0        0        0     6827 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0    15372 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/changelog.md
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/cmakelists.md
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/conf.py
--rw-r--r--   0        0        0    12730 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/configuration.md
--rw-r--r--   0        0        0     9062 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/getting_started.md
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/index.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/api/scikit_build_core.build.rst
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/api/scikit_build_core.builder.rst
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/api/scikit_build_core.file_api.model.rst
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/api/scikit_build_core.file_api.rst
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/api/scikit_build_core.metadata.rst
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/api/scikit_build_core.resources.find_python.rst
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/api/scikit_build_core.resources.rst
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/api/scikit_build_core.rst
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/api/scikit_build_core.settings.rst
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/api/scikit_build_core.setuptools.rst
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/test.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/abi3/CMakeLists.txt
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/abi3/example.c
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/abi3/pyproject.toml
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/c/CMakeLists.txt
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/c/example.c
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/c/pyproject.toml
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/cython/CMakeLists.txt
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/cython/example.pyx
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/cython/pyproject.toml
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/fortran/CMakeLists.txt
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/fortran/example.f
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/fortran/pyproject.toml
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/pybind11/CMakeLists.txt
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/pybind11/example.cpp
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/pybind11/pyproject.toml
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/swig/CMakeLists.txt
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/swig/example.c
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/swig/example.i
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/swig/pyproject.toml
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/__init__.py
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/_logging.py
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/_shutil.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/_version.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/_version.pyi
--rw-r--r--   0        0        0     8594 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/cmake.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/errors.py
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/program_search.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/py.typed
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/_compat/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/_compat/builtins.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/_compat/tomllib.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/_compat/typing.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/_compat/importlib/__init__.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/_compat/importlib/metadata.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/_compat/importlib/resources.py
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/build/__init__.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/build/_file_processor.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/build/_init.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/build/_pathutil.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/build/_scripts.py
--rw-r--r--   0        0        0     8169 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/build/_wheelfile.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/build/sdist.py
--rw-r--r--   0        0        0     9882 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/build/wheel.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/builder/__init__.py
--rw-r--r--   0        0        0     7574 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/builder/builder.py
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/builder/generator.py
--rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/builder/get_requires.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/builder/macos.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/builder/sysconfig.py
--rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/builder/wheel_tag.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/file_api/__init__.py
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/file_api/_cattrs_converter.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/file_api/query.py
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/file_api/reply.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/file_api/model/__init__.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/file_api/model/cache.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/file_api/model/cmakefiles.py
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/file_api/model/codemodel.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/file_api/model/common.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/file_api/model/directory.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/file_api/model/index.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/file_api/model/toolchains.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/metadata/__init__.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/metadata/fancy_pypi_readme.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/metadata/setuptools_scm.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/resources/__init__.py
--rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/resources/_editable_redirect.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/resources/known_wheels.toml
--rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/resources/find_python/Copyright.txt
--rw-r--r--   0        0        0    23174 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake
--rw-r--r--   0        0        0    22536 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/resources/find_python/FindPython.cmake
--rw-r--r--   0        0        0    19036 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/resources/find_python/FindPython3.cmake
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/resources/find_python/__init__.py
--rw-r--r--   0        0        0   198528 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/resources/find_python/FindPython/Support.cmake
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/settings/__init__.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/settings/_load_provider.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/settings/metadata.py
--rw-r--r--   0        0        0     5642 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/settings/skbuild_model.py
--rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/settings/skbuild_read_settings.py
--rw-r--r--   0        0        0    18214 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/settings/sources.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/setuptools/__init__.py
--rw-r--r--   0        0        0     7759 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/setuptools/build_cmake.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/setuptools/build_meta.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/setuptools/wrapper.py
--rw-r--r--   0        0        0     9343 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/conftest.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/constraints.txt
--rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_builder.py
--rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_cmake_config.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_custom_modules.py
--rw-r--r--   0        0        0     8426 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_dynamic_metadata.py
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_fileapi.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_fortran.py
--rw-r--r--   0        0        0    15811 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_generator_default.py
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_get_requires.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_logging.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_module_dir.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_name_main.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_prepare_metadata.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_process_scripts.py
--rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_program_search.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_pyproject_abi3.py
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_pyproject_extra_dirs.py
--rw-r--r--   0        0        0     8248 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_pyproject_pep517.py
--rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_pyproject_pep518.py
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_pyproject_pep660.py
--rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_settings.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_setuptools_abi3.py
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_setuptools_pep517.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_setuptools_pep518.py
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_simple_pure.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_simplest_c.py
--rw-r--r--   0        0        0    12743 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_skbuild_settings.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_wheelfile_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/query/cache-v2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/query/cmakeFiles-v1
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/query/codemodel-v2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/query/toolchains-v1
--rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/abi3_pyproject_ext/CMakeLists.txt
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/abi3_pyproject_ext/abi3_example.c
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/abi3_pyproject_ext/pyproject.toml
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/abi3_setuptools_ext/CMakeLists.txt
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/abi3_setuptools_ext/abi3_example.c
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/abi3_setuptools_ext/pyproject.toml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/abi3_setuptools_ext/setup.cfg
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/abi3_setuptools_ext/setup.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/custom_cmake/CMakeLists.txt
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/custom_cmake/pyproject.toml
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/custom_cmake/extern/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/__init__.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/ExampleInclude.cmake
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/__init__.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/ExamplePkgConfig.cmake
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/__init__.py
--rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/custom_cmake/scripts/script1
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/dynamic_metadata/CMakeLists.txt
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/dynamic_metadata/dual_project.toml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/dynamic_metadata/faulty_dual_project.toml
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/dynamic_metadata/faulty_project.toml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/dynamic_metadata/local_pyproject.toml
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/dynamic_metadata/plugin_project.toml
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/dynamic_metadata/pyproject.toml
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/dynamic_metadata/warn_project.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/dynamic_metadata/plugins/local/version/__init__.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/dynamic_metadata/plugins/local/version/nested/__init__.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/dynamic_metadata/src/module.c
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/dynamic_metadata/src/dynamic/__init__.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/filepath_pure/CMakeLists.txt
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/filepath_pure/pyproject.toml
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/fortran_example/CMakeLists.txt
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/fortran_example/fib1.f
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/fortran_example/pyproject.toml
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/mixed_setuptools/CMakeLists.txt
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/mixed_setuptools/pyproject.toml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/mixed_setuptools/setup.cfg
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/mixed_setuptools/setup.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/mixed_setuptools/src/main.cpp
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/mixed_setuptools/src/mixed_setuptools/__init__.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/mixed_setuptools/src/mixed_setuptools/_core.pyi
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simple_pure/CMakeLists.txt
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simple_pure/simple_pure.cpp
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simple_pyproject_ext/CMakeLists.txt
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simple_pyproject_ext/LICENSE
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simple_pyproject_ext/pyproject.toml
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simple_pyproject_ext/src/main.cpp
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simple_pyproject_source_dir/LICENSE
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simple_pyproject_source_dir/pyproject.toml
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simple_pyproject_source_dir/src/CMakeLists.txt
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simple_pyproject_source_dir/src/main.cpp
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simple_setuptools_ext/CMakeLists.txt
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simple_setuptools_ext/LICENSE
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simple_setuptools_ext/pyproject.toml
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simple_setuptools_ext/setup.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simple_setuptools_ext/src/main.cpp
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simplest_c/.gitignore
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simplest_c/CMakeLists.txt
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simplest_c/pyproject.toml
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simplest_c/src/module.c
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simplest_c/src/not_a_package/simple.txt
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simplest_c/src/simplest/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simplest_c/src/simplest/_module.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simplest_c/src/simplest/artifact_ignored.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simplest_c/src/simplest/data.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simplest_c/src/simplest/excluded.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simplest_c/src/simplest/ignored.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simplest_c/src/simplest/ignored_included.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simplest_c/src/simplest/sdist_only.txt
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.gitignore
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/LICENSE
--rw-r--r--   0        0        0    10748 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/README.md
--rw-r--r--   0        0        0     8587 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/pyproject.toml
--rw-r--r--   0        0        0    13747 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.gitattributes
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.packit.yaml
+-rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.readthedocs.yml
+-rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/noxfile.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.distro/packit.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.distro/python-scikit-build-core.rpmlintrc
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.distro/python-scikit-build-core.spec
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.distro/.fmf/version
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.distro/plans/main.fmf.dist-git
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.distro/plans/rpmlint.fmf
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.distro/plans/smoke.fmf
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.distro/tests/rpmlint.fmf
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.distro/tests/smoke.fmf
+-rw-r--r--   0        0        0     9969 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.github/codecov.yml
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     6827 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0    15738 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/changelog.md
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/cmakelists.md
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/conf.py
+-rw-r--r--   0        0        0    12730 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/configuration.md
+-rw-r--r--   0        0        0     9062 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/getting_started.md
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/index.md
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/api/scikit_build_core.build.rst
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/api/scikit_build_core.builder.rst
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/api/scikit_build_core.file_api.model.rst
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/api/scikit_build_core.file_api.rst
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/api/scikit_build_core.metadata.rst
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/api/scikit_build_core.resources.find_python.rst
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/api/scikit_build_core.resources.rst
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/api/scikit_build_core.rst
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/api/scikit_build_core.settings.rst
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/api/scikit_build_core.setuptools.rst
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/test.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/abi3/CMakeLists.txt
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/abi3/example.c
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/abi3/pyproject.toml
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/c/CMakeLists.txt
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/c/example.c
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/c/pyproject.toml
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/cython/CMakeLists.txt
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/cython/example.pyx
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/cython/pyproject.toml
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/fortran/CMakeLists.txt
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/fortran/example.f
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/fortran/pyproject.toml
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/pybind11/CMakeLists.txt
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/pybind11/example.cpp
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/pybind11/pyproject.toml
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/swig/CMakeLists.txt
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/swig/example.c
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/swig/example.i
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/docs/examples/getting_started/swig/pyproject.toml
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/__init__.py
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/_logging.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/_shutil.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/_version.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/_version.pyi
+-rw-r--r--   0        0        0     8594 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/cmake.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/errors.py
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/program_search.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/py.typed
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/_compat/__init__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/_compat/builtins.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/_compat/tomllib.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/_compat/typing.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/_compat/importlib/metadata.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/_compat/importlib/resources.py
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/build/__init__.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/build/_file_processor.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/build/_init.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/build/_pathutil.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/build/_scripts.py
+-rw-r--r--   0        0        0     8169 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/build/_wheelfile.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/build/sdist.py
+-rw-r--r--   0        0        0    10438 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/build/wheel.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/builder/__init__.py
+-rw-r--r--   0        0        0     7854 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/builder/builder.py
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/builder/generator.py
+-rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/builder/get_requires.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/builder/macos.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/builder/sysconfig.py
+-rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/builder/wheel_tag.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/file_api/__init__.py
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/file_api/_cattrs_converter.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/file_api/query.py
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/file_api/reply.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/file_api/model/__init__.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/file_api/model/cache.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/file_api/model/cmakefiles.py
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/file_api/model/codemodel.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/file_api/model/common.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/file_api/model/directory.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/file_api/model/index.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/file_api/model/toolchains.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/metadata/__init__.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/metadata/fancy_pypi_readme.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/metadata/setuptools_scm.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/resources/__init__.py
+-rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/resources/_editable_redirect.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/resources/known_wheels.toml
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/resources/find_python/Copyright.txt
+-rw-r--r--   0        0        0    23174 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake
+-rw-r--r--   0        0        0    22536 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/resources/find_python/FindPython.cmake
+-rw-r--r--   0        0        0    19036 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/resources/find_python/FindPython3.cmake
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/resources/find_python/__init__.py
+-rw-r--r--   0        0        0   198528 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/resources/find_python/FindPython/Support.cmake
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/settings/__init__.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/settings/_load_provider.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/settings/metadata.py
+-rw-r--r--   0        0        0     5642 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/settings/skbuild_model.py
+-rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/settings/skbuild_read_settings.py
+-rw-r--r--   0        0        0    18214 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/settings/sources.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/setuptools/__init__.py
+-rw-r--r--   0        0        0     7759 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/setuptools/build_cmake.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/setuptools/build_meta.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/src/scikit_build_core/setuptools/wrapper.py
+-rw-r--r--   0        0        0     9343 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/conftest.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/constraints.txt
+-rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_builder.py
+-rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_cmake_config.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_custom_modules.py
+-rw-r--r--   0        0        0     8426 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_dynamic_metadata.py
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_fileapi.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_fortran.py
+-rw-r--r--   0        0        0    15811 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_generator_default.py
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_get_requires.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_logging.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_module_dir.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_name_main.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_prepare_metadata.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_process_scripts.py
+-rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_program_search.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_pyproject_abi3.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_pyproject_extra_dirs.py
+-rw-r--r--   0        0        0     8248 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_pyproject_pep517.py
+-rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_pyproject_pep518.py
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_pyproject_pep660.py
+-rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_settings.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_setuptools_abi3.py
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_setuptools_pep517.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_setuptools_pep518.py
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_simple_pure.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_simplest_c.py
+-rw-r--r--   0        0        0    12743 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_skbuild_settings.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/test_wheelfile_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/query/cache-v2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/query/cmakeFiles-v1
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/query/codemodel-v2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/query/toolchains-v1
+-rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/abi3_pyproject_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/abi3_pyproject_ext/abi3_example.c
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/abi3_pyproject_ext/pyproject.toml
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/abi3_setuptools_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/abi3_setuptools_ext/abi3_example.c
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/abi3_setuptools_ext/pyproject.toml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/abi3_setuptools_ext/setup.cfg
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/abi3_setuptools_ext/setup.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/custom_cmake/CMakeLists.txt
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/custom_cmake/pyproject.toml
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/custom_cmake/extern/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/__init__.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/ExampleInclude.cmake
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/__init__.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/ExamplePkgConfig.cmake
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/__init__.py
+-rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/custom_cmake/scripts/script1
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/dynamic_metadata/CMakeLists.txt
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/dynamic_metadata/dual_project.toml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/dynamic_metadata/faulty_dual_project.toml
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/dynamic_metadata/faulty_project.toml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/dynamic_metadata/local_pyproject.toml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/dynamic_metadata/plugin_project.toml
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/dynamic_metadata/pyproject.toml
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/dynamic_metadata/warn_project.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/dynamic_metadata/plugins/local/version/__init__.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/dynamic_metadata/plugins/local/version/nested/__init__.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/dynamic_metadata/src/module.c
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/dynamic_metadata/src/dynamic/__init__.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/filepath_pure/CMakeLists.txt
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/filepath_pure/pyproject.toml
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/fortran_example/CMakeLists.txt
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/fortran_example/fib1.f
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/fortran_example/pyproject.toml
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/mixed_setuptools/CMakeLists.txt
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/mixed_setuptools/pyproject.toml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/mixed_setuptools/setup.cfg
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/mixed_setuptools/setup.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/mixed_setuptools/src/main.cpp
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/mixed_setuptools/src/mixed_setuptools/__init__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/mixed_setuptools/src/mixed_setuptools/_core.pyi
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simple_pure/CMakeLists.txt
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simple_pure/simple_pure.cpp
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simple_pyproject_ext/CMakeLists.txt
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simple_pyproject_ext/LICENSE
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simple_pyproject_ext/pyproject.toml
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simple_pyproject_ext/src/main.cpp
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simple_pyproject_source_dir/LICENSE
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simple_pyproject_source_dir/pyproject.toml
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simple_pyproject_source_dir/src/CMakeLists.txt
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simple_pyproject_source_dir/src/main.cpp
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simple_setuptools_ext/CMakeLists.txt
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simple_setuptools_ext/LICENSE
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simple_setuptools_ext/pyproject.toml
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simple_setuptools_ext/setup.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simple_setuptools_ext/src/main.cpp
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simplest_c/.gitignore
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simplest_c/CMakeLists.txt
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simplest_c/pyproject.toml
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simplest_c/src/module.c
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simplest_c/src/not_a_package/simple.txt
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simplest_c/src/simplest/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simplest_c/src/simplest/_module.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simplest_c/src/simplest/artifact_ignored.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simplest_c/src/simplest/data.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simplest_c/src/simplest/excluded.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simplest_c/src/simplest/ignored.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simplest_c/src/simplest/ignored_included.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/tests/packages/simplest_c/src/simplest/sdist_only.txt
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/.gitignore
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/LICENSE
+-rw-r--r--   0        0        0    10816 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/README.md
+-rw-r--r--   0        0        0     8587 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0    13815 2020-02-02 00:00:00.000000 scikit_build_core-0.4.4/PKG-INFO
```

### Comparing `scikit_build_core-0.4.3/.packit.yaml` & `scikit_build_core-0.4.4/.packit.yaml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/.pre-commit-config.yaml` & `scikit_build_core-0.4.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/noxfile.py` & `scikit_build_core-0.4.4/noxfile.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/.distro/python-scikit-build-core.spec` & `scikit_build_core-0.4.4/.distro/python-scikit-build-core.spec`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/.github/CONTRIBUTING.md` & `scikit_build_core-0.4.4/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/.github/matchers/pylint.json` & `scikit_build_core-0.4.4/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/.github/workflows/cd.yml` & `scikit_build_core-0.4.4/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/.github/workflows/ci.yml` & `scikit_build_core-0.4.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/docs/changelog.md` & `scikit_build_core-0.4.4/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # Changelog
 
+## Version 0.4.4
+
+This version fixes some issues cross-compiling to Windows ARM when making
+Limited API / Stable ABI extensions, and supports multiple config generators in
+editable mode.
+
+- Conditional ABI3 logic fixed by @henryiii in #352
+- Set `Python_SABI_LIBRARY` by @henryiii in #352
+- Editable installs now support multiconfig generators by @henryiii in #353
+
 ## Version 0.4.3
 
 This adds support for CPython 3.12.0b1, and improves Stable ABI / Limited API
 support (supported by an upcoming nanobind for Python 3.12). An editable install
 fix allows running from any directory.
 
 Fixes:
```

### Comparing `scikit_build_core-0.4.3/docs/cmakelists.md` & `scikit_build_core-0.4.4/docs/cmakelists.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/docs/conf.py` & `scikit_build_core-0.4.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/docs/configuration.md` & `scikit_build_core-0.4.4/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/docs/getting_started.md` & `scikit_build_core-0.4.4/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/docs/index.md` & `scikit_build_core-0.4.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/docs/api/scikit_build_core.build.rst` & `scikit_build_core-0.4.4/docs/api/scikit_build_core.build.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/docs/api/scikit_build_core.builder.rst` & `scikit_build_core-0.4.4/docs/api/scikit_build_core.builder.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/docs/api/scikit_build_core.file_api.model.rst` & `scikit_build_core-0.4.4/docs/api/scikit_build_core.file_api.model.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/docs/api/scikit_build_core.file_api.rst` & `scikit_build_core-0.4.4/docs/api/scikit_build_core.file_api.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/docs/api/scikit_build_core.metadata.rst` & `scikit_build_core-0.4.4/docs/api/scikit_build_core.metadata.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/docs/api/scikit_build_core.rst` & `scikit_build_core-0.4.4/docs/api/scikit_build_core.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/docs/api/scikit_build_core.settings.rst` & `scikit_build_core-0.4.4/docs/api/scikit_build_core.settings.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/docs/api/scikit_build_core.setuptools.rst` & `scikit_build_core-0.4.4/docs/api/scikit_build_core.setuptools.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/docs/examples/getting_started/abi3/example.c` & `scikit_build_core-0.4.4/docs/examples/getting_started/abi3/example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/docs/examples/getting_started/c/example.c` & `scikit_build_core-0.4.4/docs/examples/getting_started/c/example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/docs/examples/getting_started/cython/CMakeLists.txt` & `scikit_build_core-0.4.4/docs/examples/getting_started/cython/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/docs/examples/getting_started/fortran/CMakeLists.txt` & `scikit_build_core-0.4.4/docs/examples/getting_started/fortran/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/docs/examples/getting_started/swig/CMakeLists.txt` & `scikit_build_core-0.4.4/docs/examples/getting_started/swig/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/_logging.py` & `scikit_build_core-0.4.4/src/scikit_build_core/_logging.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/_shutil.py` & `scikit_build_core-0.4.4/src/scikit_build_core/_shutil.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/cmake.py` & `scikit_build_core-0.4.4/src/scikit_build_core/cmake.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/errors.py` & `scikit_build_core-0.4.4/src/scikit_build_core/errors.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/program_search.py` & `scikit_build_core-0.4.4/src/scikit_build_core/program_search.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/_compat/typing.py` & `scikit_build_core-0.4.4/src/scikit_build_core/_compat/typing.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/_compat/importlib/metadata.py` & `scikit_build_core-0.4.4/src/scikit_build_core/_compat/importlib/metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/build/__init__.py` & `scikit_build_core-0.4.4/src/scikit_build_core/build/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/build/_file_processor.py` & `scikit_build_core-0.4.4/src/scikit_build_core/build/_file_processor.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/build/_init.py` & `scikit_build_core-0.4.4/src/scikit_build_core/build/_init.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/build/_pathutil.py` & `scikit_build_core-0.4.4/src/scikit_build_core/build/_pathutil.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/build/_scripts.py` & `scikit_build_core-0.4.4/src/scikit_build_core/build/_scripts.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/build/_wheelfile.py` & `scikit_build_core-0.4.4/src/scikit_build_core/build/_wheelfile.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/build/sdist.py` & `scikit_build_core-0.4.4/src/scikit_build_core/build/sdist.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/build/wheel.py` & `scikit_build_core-0.4.4/src/scikit_build_core/build/wheel.py`

 * *Files 6% similar despite different names*

```diff
@@ -253,15 +253,30 @@
                     for v in scantree(wheel_dirs["platlib"])
                 }
                 editable_py = resources / "_editable_redirect.py"
                 editable_txt = editable_py.read_text(encoding="utf-8")
                 reload_dir = (
                     os.fspath(build_dir.resolve()) if settings.build_dir else None
                 )
-                editable_txt += f"\n\ninstall({modules!r}, {installed!r}, {reload_dir!r}, {settings.editable.rebuild!r}, {settings.editable.verbose!r})\n"
+                options = []
+                if not builder.config.single_config and builder.config.build_type:
+                    options += ["--config", builder.config.build_type]
+                ext_build_opts = ["-v"] if builder.settings.cmake.verbose else []
+
+                arguments = (
+                    modules,
+                    installed,
+                    reload_dir,
+                    settings.editable.rebuild,
+                    settings.editable.verbose,
+                    options + ext_build_opts,
+                    options,
+                )
+                arguments_str = ", ".join(repr(x) for x in arguments)
+                editable_txt += f"\n\ninstall({arguments_str})\n"
 
                 wheel.writestr(
                     f"_{normalized_name}_editable.py",
                     editable_txt.encode("utf-8"),
                 )
                 wheel.writestr(
                     f"_{normalized_name}_editable.pth",
```

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/builder/builder.py` & `scikit_build_core-0.4.4/src/scikit_build_core/builder/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,19 +125,22 @@
             cache_config["SKBUILD_PROJECT_NAME"] = canonical_name
         if version is not None:
             cache_config["SKBUILD_PROJECT_VERSION"] = str(version)
 
         if limited_abi is None:
             if self.settings.wheel.py_api.startswith("cp3"):
                 target_minor_version = int(self.settings.wheel.py_api[3:])
-                limited_abi = target_minor_version >= sys.version_info.minor
+                limited_abi = target_minor_version <= sys.version_info.minor
             else:
                 limited_abi = False
 
-        python_library = get_python_library(self.config.env, abi3=limited_abi)
+        python_library = get_python_library(self.config.env, abi3=False)
+        python_sabi_library = (
+            get_python_library(self.config.env, abi3=True) if limited_abi else None
+        )
         python_include_dir = get_python_include_dir()
 
         # Classic Find Python
         cache_config["PYTHON_EXECUTABLE"] = sys.executable
         cache_config["PYTHON_INCLUDE_DIR"] = python_include_dir
         if python_library:
             cache_config["PYTHON_LIBRARY"] = python_library
@@ -147,14 +150,16 @@
             cache_config[f"{prefix}_EXECUTABLE"] = sys.executable
             cache_config[f"{prefix}_ROOT_DIR"] = sys.prefix
             cache_config[f"{prefix}_INCLUDE_DIR"] = python_include_dir
             cache_config[f"{prefix}_FIND_REGISTRY"] = "NEVER"
             # FindPython may break if this is set - only useful on Windows
             if python_library and sysconfig.get_platform().startswith("win"):
                 cache_config[f"{prefix}_LIBRARY"] = python_library
+            if python_sabi_library and sysconfig.get_platform().startswith("win"):
+                cache_config[f"{prefix}_SABI_LIBRARY"] = python_sabi_library
 
         if limited_abi:
             cache_config["SKBUILD_SOABI"] = (
                 "" if sysconfig.get_platform().startswith("win") else "abi3"
             )
         else:
             # Workaround for bug in PyPy and packaging that is not handled in CMake
```

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/builder/generator.py` & `scikit_build_core-0.4.4/src/scikit_build_core/builder/generator.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/builder/get_requires.py` & `scikit_build_core-0.4.4/src/scikit_build_core/builder/get_requires.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/builder/macos.py` & `scikit_build_core-0.4.4/src/scikit_build_core/builder/macos.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/builder/sysconfig.py` & `scikit_build_core-0.4.4/src/scikit_build_core/builder/sysconfig.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/builder/wheel_tag.py` & `scikit_build_core-0.4.4/src/scikit_build_core/builder/wheel_tag.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/file_api/_cattrs_converter.py` & `scikit_build_core-0.4.4/src/scikit_build_core/file_api/_cattrs_converter.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/file_api/query.py` & `scikit_build_core-0.4.4/src/scikit_build_core/file_api/query.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/file_api/reply.py` & `scikit_build_core-0.4.4/src/scikit_build_core/file_api/reply.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/file_api/model/codemodel.py` & `scikit_build_core-0.4.4/src/scikit_build_core/file_api/model/codemodel.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/file_api/model/directory.py` & `scikit_build_core-0.4.4/src/scikit_build_core/file_api/model/directory.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/file_api/model/index.py` & `scikit_build_core-0.4.4/src/scikit_build_core/file_api/model/index.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/file_api/model/toolchains.py` & `scikit_build_core-0.4.4/src/scikit_build_core/file_api/model/toolchains.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/metadata/fancy_pypi_readme.py` & `scikit_build_core-0.4.4/src/scikit_build_core/metadata/fancy_pypi_readme.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/metadata/setuptools_scm.py` & `scikit_build_core-0.4.4/src/scikit_build_core/metadata/setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/resources/_editable_redirect.py` & `scikit_build_core-0.4.4/src/scikit_build_core/resources/_editable_redirect.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,20 +22,24 @@
     def __init__(
         self,
         known_source_files: dict[str, str],
         known_wheel_files: dict[str, str],
         path: str | None,
         rebuild: bool,
         verbose: bool,
+        build_options: list[str],
+        install_options: list[str],
     ):
         self.known_source_files = known_source_files
         self.known_wheel_files = known_wheel_files
         self.path = path
         self.rebuild_flag = rebuild
         self.verbose = verbose
+        self.build_options = build_options
+        self.install_options = install_options
 
     def find_spec(
         self,
         fullname: str,
         path: object = None,
         target: object = None,
     ) -> importlib.machinery.ModuleSpec | None:
@@ -67,30 +71,30 @@
         verbose = self.verbose or bool(env.get(VERBOSE, ""))
         if env.get(VERBOSE, "") == "0":
             verbose = False
         if verbose:
             print(f"Running cmake --build & --install in {self.path}")  # noqa: T201
 
         result = subprocess.run(
-            ["cmake", "--build", "."],
+            ["cmake", "--build", ".", *self.build_options],
             cwd=self.path,
             stdout=sys.stderr if verbose else subprocess.PIPE,
             env=env,
             check=False,
             text=True,
         )
         if result.returncode and verbose:
             print(  # noqa: T201
                 f"ERROR: {result.stdout}",
                 file=sys.stderr,
             )
         result.check_returncode()
 
         result = subprocess.run(
-            ["cmake", "--install", ".", "--prefix", DIR],
+            ["cmake", "--install", ".", "--prefix", DIR, *self.install_options],
             cwd=self.path,
             stdout=sys.stderr if verbose else subprocess.PIPE,
             env=env,
             check=False,
             text=True,
         )
         if result.returncode and verbose:
@@ -103,24 +107,32 @@
 
 def install(
     known_source_files: dict[str, str],
     known_wheel_files: dict[str, str],
     path: str | None,
     rebuild: bool = False,
     verbose: bool = False,
+    build_options: list[str] | None = None,
+    install_options: list[str] | None = None,
 ) -> None:
     """
     Install a meta path finder that redirects imports to the source files, and
     optionally rebuilds if path is given.
 
     :param known_source_files: A mapping of module names to source files
     :param known_wheel_files: A mapping of module names to wheel files
     :param path: The path to the build directory, or None
     :param verbose: Whether to print the cmake commands (also controlled by the
                     SKBUILD_EDITABLE_VERBOSE environment variable)
     """
     sys.meta_path.insert(
         0,
         ScikitBuildRedirectingFinder(
-            known_source_files, known_wheel_files, path, rebuild, verbose
+            known_source_files,
+            known_wheel_files,
+            path,
+            rebuild,
+            verbose,
+            build_options or [],
+            install_options or [],
         ),
     )
```

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/resources/known_wheels.toml` & `scikit_build_core-0.4.4/src/scikit_build_core/resources/known_wheels.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/resources/find_python/Copyright.txt` & `scikit_build_core-0.4.4/src/scikit_build_core/resources/find_python/Copyright.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake` & `scikit_build_core-0.4.4/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake` & `scikit_build_core-0.4.4/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/resources/find_python/FindPython.cmake` & `scikit_build_core-0.4.4/src/scikit_build_core/resources/find_python/FindPython.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/resources/find_python/FindPython3.cmake` & `scikit_build_core-0.4.4/src/scikit_build_core/resources/find_python/FindPython3.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/resources/find_python/FindPython/Support.cmake` & `scikit_build_core-0.4.4/src/scikit_build_core/resources/find_python/FindPython/Support.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/settings/_load_provider.py` & `scikit_build_core-0.4.4/src/scikit_build_core/settings/_load_provider.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/settings/metadata.py` & `scikit_build_core-0.4.4/src/scikit_build_core/settings/metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/settings/skbuild_model.py` & `scikit_build_core-0.4.4/src/scikit_build_core/settings/skbuild_model.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/settings/skbuild_read_settings.py` & `scikit_build_core-0.4.4/src/scikit_build_core/settings/skbuild_read_settings.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/settings/sources.py` & `scikit_build_core-0.4.4/src/scikit_build_core/settings/sources.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/setuptools/build_cmake.py` & `scikit_build_core-0.4.4/src/scikit_build_core/setuptools/build_cmake.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/setuptools/build_meta.py` & `scikit_build_core-0.4.4/src/scikit_build_core/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/src/scikit_build_core/setuptools/wrapper.py` & `scikit_build_core-0.4.4/src/scikit_build_core/setuptools/wrapper.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/conftest.py` & `scikit_build_core-0.4.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/test_builder.py` & `scikit_build_core-0.4.4/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/test_cmake_config.py` & `scikit_build_core-0.4.4/tests/test_cmake_config.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/test_dynamic_metadata.py` & `scikit_build_core-0.4.4/tests/test_dynamic_metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/test_fileapi.py` & `scikit_build_core-0.4.4/tests/test_fileapi.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/test_fortran.py` & `scikit_build_core-0.4.4/tests/test_fortran.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/test_generator_default.py` & `scikit_build_core-0.4.4/tests/test_generator_default.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/test_get_requires.py` & `scikit_build_core-0.4.4/tests/test_get_requires.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/test_module_dir.py` & `scikit_build_core-0.4.4/tests/test_module_dir.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/test_name_main.py` & `scikit_build_core-0.4.4/tests/test_name_main.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/test_prepare_metadata.py` & `scikit_build_core-0.4.4/tests/test_prepare_metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/test_process_scripts.py` & `scikit_build_core-0.4.4/tests/test_process_scripts.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/test_program_search.py` & `scikit_build_core-0.4.4/tests/test_program_search.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/test_pyproject_abi3.py` & `scikit_build_core-0.4.4/tests/test_pyproject_abi3.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/test_pyproject_extra_dirs.py` & `scikit_build_core-0.4.4/tests/test_pyproject_extra_dirs.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/test_pyproject_pep517.py` & `scikit_build_core-0.4.4/tests/test_pyproject_pep517.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/test_pyproject_pep518.py` & `scikit_build_core-0.4.4/tests/test_pyproject_pep518.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/test_pyproject_pep660.py` & `scikit_build_core-0.4.4/tests/test_pyproject_pep660.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/test_settings.py` & `scikit_build_core-0.4.4/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/test_setuptools_abi3.py` & `scikit_build_core-0.4.4/tests/test_setuptools_abi3.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/test_setuptools_pep517.py` & `scikit_build_core-0.4.4/tests/test_setuptools_pep517.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/test_setuptools_pep518.py` & `scikit_build_core-0.4.4/tests/test_setuptools_pep518.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/test_simple_pure.py` & `scikit_build_core-0.4.4/tests/test_simple_pure.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/test_simplest_c.py` & `scikit_build_core-0.4.4/tests/test_simplest_c.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/test_skbuild_settings.py` & `scikit_build_core-0.4.4/tests/test_skbuild_settings.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/test_wheelfile_utils.py` & `scikit_build_core-0.4.4/tests/test_wheelfile_utils.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json` & `scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json` & `scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json` & `scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json` & `scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json` & `scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json` & `scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json` & `scikit_build_core-0.4.4/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/packages/abi3_pyproject_ext/abi3_example.c` & `scikit_build_core-0.4.4/tests/packages/abi3_pyproject_ext/abi3_example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/packages/abi3_setuptools_ext/abi3_example.c` & `scikit_build_core-0.4.4/tests/packages/abi3_setuptools_ext/abi3_example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/packages/dynamic_metadata/plugin_project.toml` & `scikit_build_core-0.4.4/tests/packages/dynamic_metadata/plugin_project.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/packages/dynamic_metadata/src/module.c` & `scikit_build_core-0.4.4/tests/packages/dynamic_metadata/src/module.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/packages/filepath_pure/CMakeLists.txt` & `scikit_build_core-0.4.4/tests/packages/filepath_pure/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/packages/fortran_example/CMakeLists.txt` & `scikit_build_core-0.4.4/tests/packages/fortran_example/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/packages/mixed_setuptools/CMakeLists.txt` & `scikit_build_core-0.4.4/tests/packages/mixed_setuptools/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/packages/simple_pyproject_ext/LICENSE` & `scikit_build_core-0.4.4/tests/packages/simple_pyproject_ext/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/packages/simple_pyproject_ext/src/main.cpp` & `scikit_build_core-0.4.4/tests/packages/simple_pyproject_ext/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/packages/simple_pyproject_source_dir/LICENSE` & `scikit_build_core-0.4.4/tests/packages/simple_pyproject_source_dir/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/packages/simple_pyproject_source_dir/src/main.cpp` & `scikit_build_core-0.4.4/tests/packages/simple_pyproject_source_dir/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/packages/simple_setuptools_ext/LICENSE` & `scikit_build_core-0.4.4/tests/packages/simple_setuptools_ext/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/packages/simple_setuptools_ext/src/main.cpp` & `scikit_build_core-0.4.4/tests/packages/simple_setuptools_ext/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/packages/simplest_c/CMakeLists.txt` & `scikit_build_core-0.4.4/tests/packages/simplest_c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/tests/packages/simplest_c/src/module.c` & `scikit_build_core-0.4.4/tests/packages/simplest_c/src/module.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/.gitignore` & `scikit_build_core-0.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/LICENSE` & `scikit_build_core-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/README.md` & `scikit_build_core-0.4.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -216,16 +216,16 @@
 backends:
 
 - [py-build-cmake][]: A different attempt at a standards compliant builder for
   CMake. Strong focus on cross-compilation. Uses Flit internals.
 - [meson-python][]: A meson-based build backend; has some maintainer overlap
   with scikit-build-core.
 - [maturin][]: A build backend for Rust projects, using Cargo.
-- [enscons][]: A SCons based backend, not very actively developed (it predates
-  all the others in modern standard support!)
+- [enscons][]: A SCons based backend, not very actively developed (but it
+  predates all the others in modern standard support!)
 
 If you don't need a binary build, you don't need to use a binary build backend!
 There are some very good Python build backends; we recommend [hatchling][] as a
 good balance between good defaults for beginners and good support for advanced
 use cases. This is the tool scikit-build-core itself uses.
 
 ## Acknowledgements
@@ -249,10 +249,11 @@
 [pypi-platforms]:           https://img.shields.io/pypi/pyversions/scikit-build-core
 [pypi-version]:             https://badge.fury.io/py/scikit-build-core.svg
 [rtd-badge]:                https://readthedocs.org/projects/scikit-build-core/badge/?version=latest
 [rtd-link]:                 https://scikit-build-core.readthedocs.io/en/latest/?badge=latest
 [OAC-2209877]:              https://www.nsf.gov/awardsearch/showAward?AWD_ID=2209877&HistoricalAwards=false
 [hatchling]:                https://hatch.pypa.io/latest
 [maturin]:                  https://www.maturin.rs
+[meson-python]:             https://meson-python.readthedocs.io
 [enscons]:                  https://pypi.org/project/enscons
 [py-build-cmake]:           https://tttapa.github.io/py-build-cmake
 <!-- prettier-ignore-end -->
```

### Comparing `scikit_build_core-0.4.3/pyproject.toml` & `scikit_build_core-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.3/PKG-INFO` & `scikit_build_core-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit_build_core
-Version: 0.4.3
+Version: 0.4.4
 Summary: Build backend for CMake based projects
 Project-URL: Homepage, https://github.com/scikit-build/scikit-build-core
 Project-URL: Documentation, https://scikit-build-core.readthedocs.io
 Project-URL: Discussions, https://github.com/orgs/scikit-build/discussions
 Project-URL: Issues, https://github.com/scikit-build/scikit-build-core/issues
 Project-URL: Changelog, https://scikit-build-core.readthedocs.io/en/latest/changelog.html
 Author-email: Henry Schreiner <henryfs@princeton.edu>
@@ -281,16 +281,16 @@
 backends:
 
 - [py-build-cmake][]: A different attempt at a standards compliant builder for
   CMake. Strong focus on cross-compilation. Uses Flit internals.
 - [meson-python][]: A meson-based build backend; has some maintainer overlap
   with scikit-build-core.
 - [maturin][]: A build backend for Rust projects, using Cargo.
-- [enscons][]: A SCons based backend, not very actively developed (it predates
-  all the others in modern standard support!)
+- [enscons][]: A SCons based backend, not very actively developed (but it
+  predates all the others in modern standard support!)
 
 If you don't need a binary build, you don't need to use a binary build backend!
 There are some very good Python build backends; we recommend [hatchling][] as a
 good balance between good defaults for beginners and good support for advanced
 use cases. This is the tool scikit-build-core itself uses.
 
 ## Acknowledgements
@@ -314,10 +314,11 @@
 [pypi-platforms]:           https://img.shields.io/pypi/pyversions/scikit-build-core
 [pypi-version]:             https://badge.fury.io/py/scikit-build-core.svg
 [rtd-badge]:                https://readthedocs.org/projects/scikit-build-core/badge/?version=latest
 [rtd-link]:                 https://scikit-build-core.readthedocs.io/en/latest/?badge=latest
 [OAC-2209877]:              https://www.nsf.gov/awardsearch/showAward?AWD_ID=2209877&HistoricalAwards=false
 [hatchling]:                https://hatch.pypa.io/latest
 [maturin]:                  https://www.maturin.rs
+[meson-python]:             https://meson-python.readthedocs.io
 [enscons]:                  https://pypi.org/project/enscons
 [py-build-cmake]:           https://tttapa.github.io/py-build-cmake
 <!-- prettier-ignore-end -->
```

