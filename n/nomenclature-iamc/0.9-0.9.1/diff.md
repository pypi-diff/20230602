# Comparing `tmp/nomenclature-iamc-0.9.tar.gz` & `tmp/nomenclature-iamc-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomenclature-iamc-0.9.tar", last modified: Tue May  2 15:29:26 2023, max compression
+gzip compressed data, was "nomenclature-iamc-0.9.1.tar", last modified: Mon May 22 08:26:10 2023, max compression
```

## Comparing `nomenclature-iamc-0.9.tar` & `nomenclature-iamc-0.9.1.tar`

### file list

```diff
@@ -1,322 +1,329 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.464473 nomenclature-iamc-0.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.476473 nomenclature-iamc-0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/.github/workflows/build-docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/.github/workflows/nightly.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/.stickler.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/DEVELOPING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-05-02 15:29:26.500474 nomenclature-iamc-0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.476473 nomenclature-iamc-0.9/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.476473 nomenclature-iamc-0.9/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.476473 nomenclature-iamc-0.9/doc/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/_static/EU-logo-300x201.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)   172467 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/_static/iamc-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/_static/open_entrance-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.476473 nomenclature-iamc-0.9/doc/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/_templates/navigation.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.476473 nomenclature-iamc-0.9/doc/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/api/codelist.rst
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/api/datastructuredefinition.rst
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/api/nomenclature.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/api/regionprocessor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/api/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.480473 nomenclature-iamc-0.9/doc/source/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/user_guide/codelist.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/user_guide/directory-structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/user_guide/local-usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/user_guide/model-mapping.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/user_guide/model-registration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/user_guide/region.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/user_guide/variable.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/doc/source/user_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.480473 nomenclature-iamc-0.9/nomenclature/
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/code.py
--rw-r--r--   0 runner    (1001) docker     (123)    20645 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/codelist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.480473 nomenclature-iamc-0.9/nomenclature/error/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/error/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/error/codelist.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/error/region.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/error/required_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/error/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.480473 nomenclature-iamc-0.9/nomenclature/processor/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21941 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/processor/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/processor/required_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/processor/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.480473 nomenclature-iamc-0.9/nomenclature/validation_schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/validation_schemas/generic_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/validation_schemas/region_mapping_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/validation_schemas/region_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/validation_schemas/tag_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/nomenclature/validation_schemas/variable_schema.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.484474 nomenclature-iamc-0.9/nomenclature_iamc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-05-02 15:29:26.000000 nomenclature-iamc-0.9/nomenclature_iamc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-05-02 15:29:26.000000 nomenclature-iamc-0.9/nomenclature_iamc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:29:26.000000 nomenclature-iamc-0.9/nomenclature_iamc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-02 15:29:26.000000 nomenclature-iamc-0.9/nomenclature_iamc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-02 15:29:26.000000 nomenclature-iamc-0.9/nomenclature_iamc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-02 15:29:26.000000 nomenclature-iamc-0.9/nomenclature_iamc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-02 15:29:26.500474 nomenclature-iamc-0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.484474 nomenclature-iamc-0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.484474 nomenclature-iamc-0.9/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.464473 nomenclature-iamc-0.9/tests/data/check_aggregate/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.464473 nomenclature-iamc-0.9/tests/data/check_aggregate/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.484474 nomenclature-iamc-0.9/tests/data/check_aggregate/components/region/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/check_aggregate/components/region/regions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.484474 nomenclature-iamc-0.9/tests/data/check_aggregate/components/variable/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/check_aggregate/components/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.464473 nomenclature-iamc-0.9/tests/data/check_aggregate/components_dict/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.484474 nomenclature-iamc-0.9/tests/data/check_aggregate/components_dict/region/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/check_aggregate/components_dict/region/regions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.484474 nomenclature-iamc-0.9/tests/data/check_aggregate/components_dict/variable/
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/check_aggregate/components_dict/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.464473 nomenclature-iamc-0.9/tests/data/custom_dimension_nc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.484474 nomenclature-iamc-0.9/tests/data/custom_dimension_nc/region/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/custom_dimension_nc/region/regions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.484474 nomenclature-iamc-0.9/tests/data/custom_dimension_nc/scenario/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/custom_dimension_nc/scenario/scenarios.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.484474 nomenclature-iamc-0.9/tests/data/custom_dimension_nc/variable/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/custom_dimension_nc/variable/tag_fuel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/custom_dimension_nc/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.484474 nomenclature-iamc-0.9/tests/data/duplicate_code_raises/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/duplicate_code_raises/bar.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/duplicate_code_raises/foo.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.484474 nomenclature-iamc-0.9/tests/data/duplicate_tag_raises/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/duplicate_tag_raises/tag_1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/duplicate_tag_raises/tag_2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.464473 nomenclature-iamc-0.9/tests/data/empty_definitions_dir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.484474 nomenclature-iamc-0.9/tests/data/empty_definitions_dir/definitions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/empty_definitions_dir/definitions/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.468473 nomenclature-iamc-0.9/tests/data/end_whitespace/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.468473 nomenclature-iamc-0.9/tests/data/end_whitespace/definitions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.484474 nomenclature-iamc-0.9/tests/data/end_whitespace/definitions/scenario/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/end_whitespace/definitions/scenario/scenarios.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.468473 nomenclature-iamc-0.9/tests/data/extras_nc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/extras_nc/region/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/extras_nc/region/regions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/extras_nc/variable/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/extras_nc/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.468473 nomenclature-iamc-0.9/tests/data/failing_variable_codelist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.468473 nomenclature-iamc-0.9/tests/data/failing_variable_codelist/rename_arg_conflict/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/failing_variable_codelist/rename_arg_conflict/variable/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/failing_variable_codelist/rename_arg_conflict/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.468473 nomenclature-iamc-0.9/tests/data/failing_variable_codelist/rename_undefined_target/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/failing_variable_codelist/rename_undefined_target/variable/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/failing_variable_codelist/rename_undefined_target/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.468473 nomenclature-iamc-0.9/tests/data/failing_variable_codelist/unknown_weight/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/failing_variable_codelist/unknown_weight/variable/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/failing_variable_codelist/unknown_weight/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/general_filtering/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/general_filtering/basic_codelist.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.468473 nomenclature-iamc-0.9/tests/data/hidden_character/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.468473 nomenclature-iamc-0.9/tests/data/hidden_character/definitions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/hidden_character/definitions/scenario/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/hidden_character/definitions/scenario/scenarios.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/invalid_yaml/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/invalid_yaml/foo.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/multiple_unit_codelist/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/multiple_unit_codelist/variable.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.468473 nomenclature-iamc-0.9/tests/data/non-default_dimensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.468473 nomenclature-iamc-0.9/tests/data/non-default_dimensions/definitions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/non-default_dimensions/definitions/region/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/non-default_dimensions/definitions/region/regions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/non-default_dimensions/definitions/scenario/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/non-default_dimensions/definitions/scenario/scenarios.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/non-default_dimensions/definitions/variable/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/non-default_dimensions/definitions/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/non-default_dimensions/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/non-default_dimensions/mappings/mapping_1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/non-default_dimensions/mappings/mapping_2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.468473 nomenclature-iamc-0.9/tests/data/non-default_dimensions_one_empty/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.468473 nomenclature-iamc-0.9/tests/data/non-default_dimensions_one_empty/definitions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/non-default_dimensions_one_empty/definitions/empty/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/non-default_dimensions_one_empty/definitions/empty/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/non-default_dimensions_one_empty/definitions/region/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/non-default_dimensions_one_empty/definitions/region/regions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/non-default_dimensions_one_empty/definitions/variable/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/non-default_dimensions_one_empty/definitions/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/non-default_dimensions_one_empty/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/non-default_dimensions_one_empty/mappings/mapping_1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/non-default_dimensions_one_empty/mappings/mapping_2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.468473 nomenclature-iamc-0.9/tests/data/non-default_folders/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.468473 nomenclature-iamc-0.9/tests/data/non-default_folders/def/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/non-default_folders/def/region/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/non-default_folders/def/region/regions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/non-default_folders/def/variable/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/non-default_folders/def/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/non-default_folders/map/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/non-default_folders/map/mapping_1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/non-default_folders/map/mapping_2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.488474 nomenclature-iamc-0.9/tests/data/norway_as_bool/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/norway_as_bool/regions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_aggregation/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_aggregation/illegal_mapping_conflict_regions.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_aggregation/illegal_mapping_duplicate_common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_aggregation/illegal_mapping_illegal_attribute.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_aggregation/illegal_mapping_invalid_format_dict.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_aggregation/illegal_mapping_model_only.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_aggregation/illegal_mapping_native_duplicate_key.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_aggregation/illegal_mapping_native_rename_key_conflict.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_aggregation/illegal_mapping_native_rename_target_conflict_1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_aggregation/illegal_mapping_native_rename_target_conflict_2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_aggregation/working_mapping.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_codelist/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_codelist/region.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/region_processing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/aggregate_only/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/aggregate_only/aggregate_only.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/complete_processing/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/complete_processing/model_a.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/complete_processing_list/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/complete_processing_list/model_a.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.468473 nomenclature-iamc-0.9/tests/data/region_processing/dsd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/dsd/region/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/dsd/region/regions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/dsd/variable/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/dsd/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/empty_aggregation/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/empty_aggregation/model_a.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/empty_aggregation/model_b.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/no_mapping/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/no_mapping/.keep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/partial_aggregation/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/partial_aggregation/model_a.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/rename_only/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/rename_only/model_a.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/rename_only/model_b.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/rename_only/model_c.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/region_processing/skip_aggregation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/region_processing/skip_aggregation/dsd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/skip_aggregation/dsd/region/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/skip_aggregation/dsd/region/regions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/skip_aggregation/dsd/variable/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/skip_aggregation/dsd/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/skip_aggregation/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/skip_aggregation/mappings/model_a.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/skip_aggregation/mappings/model_b.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/region_processing/weighted_aggregation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/weighted_aggregation/aggregate/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/weighted_aggregation/aggregate/aggregate_only.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/region_processing/weighted_aggregation/dsd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/weighted_aggregation/dsd/region/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/weighted_aggregation/dsd/region/regions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/weighted_aggregation/dsd/variable/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/weighted_aggregation/dsd/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/region_processing/weighted_aggregation_rename/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/weighted_aggregation_rename/aggregate/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/weighted_aggregation_rename/aggregate/aggregate_only.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/region_processing/weighted_aggregation_rename/dsd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/weighted_aggregation_rename/dsd/region/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/weighted_aggregation_rename/dsd/region/regions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_processing/weighted_aggregation_rename/dsd/variable/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_processing/weighted_aggregation_rename/dsd/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/region_to_filter_codelist/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/region_to_filter_codelist/region_filtering.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/regionprocessor_duplicate/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/regionprocessor_duplicate/mapping_1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/regionprocessor_duplicate/mapping_2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/regionprocessor_exclude_region_overlap/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/regionprocessor_exclude_region_overlap/exclude_common_overlap.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/regionprocessor_exclude_region_overlap/exclude_native_overlap.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.492474 nomenclature-iamc-0.9/tests/data/regionprocessor_not_defined/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/regionprocessor_not_defined/mapping_1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/regionprocessor_not_defined/mapping_2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/regionprocessor_unexpected_region/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/regionprocessor_unexpected_region/model_a.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/regionprocessor_working/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/regionprocessor_working/mapping_1.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/regionprocessor_working/mapping_2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/required_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/required_data/definition/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/required_data/definition/region/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/required_data/definition/region/region.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/required_data/definition/variable/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/required_data/definition/variable/variable.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/required_data/required_data/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/required_data/required_data/requiredData.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/required_data/required_data/requiredData_apply_error.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/required_data/required_data/requiredData_apply_working.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/required_data/required_data/requiredData_unknown_region.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/required_data/required_data/requiredData_unknown_unit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/required_data/required_data/requiredData_unknown_variable.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/simple_codelist/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/simple_codelist/foo.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/stray_tag/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/stray_tag/definitions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/stray_tag/definitions/variable/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/stray_tag/definitions/variable/tag_fuel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/stray_tag/definitions/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/structure_validation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/structure_validation/definitions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/structure_validation/definitions/region/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/structure_validation/definitions/region/regions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/structure_validation/definitions/variable/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/structure_validation/definitions/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/structure_validation/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/structure_validation/mappings/mapping_1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/structure_validation/mappings/mapping_2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/structure_validation_fails/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/structure_validation_fails/definitions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/structure_validation_fails/definitions/region/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/structure_validation_fails/definitions/region/regions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/structure_validation_fails/definitions/variable/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/structure_validation_fails/definitions/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/structure_validation_fails/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/structure_validation_fails/mappings/mapping_1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/structure_validation_fails/mappings/mapping_2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/structure_validation_no_mappings/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/structure_validation_no_mappings/definitions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/structure_validation_no_mappings/definitions/region/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/structure_validation_no_mappings/definitions/region/regions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/structure_validation_no_mappings/definitions/variable/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/structure_validation_no_mappings/definitions/variable/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/tagged_codelist/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/tagged_codelist/foo.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/tagged_codelist/tag_sector.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/tagged_codelist/tag_source.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.472473 nomenclature-iamc-0.9/tests/data/validation_nc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/validation_nc/region/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/validation_nc/region/regions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/validation_nc/variable/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/validation_nc/variable/tag_fuel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/validation_nc/variable/variables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/validation_nc.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/validation_nc_duplicates.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/validation_nc_flat.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/validation_nc_list_arg.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:29:26.496474 nomenclature-iamc-0.9/tests/data/variable_codelist_complex_attr/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/data/variable_codelist_complex_attr/variable_complex_attr.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/test_check_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/test_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    10421 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/test_codelist.py
--rw-r--r--   0 runner    (1001) docker     (123)    15827 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/test_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/test_definition_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/test_region_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/test_required_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-05-02 15:29:13.000000 nomenclature-iamc-0.9/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.408842 nomenclature-iamc-0.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.332842 nomenclature-iamc-0.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.364842 nomenclature-iamc-0.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/.github/workflows/build-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/.github/workflows/nightly.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/.stickler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/DEVELOPING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-22 08:26:10.408842 nomenclature-iamc-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.364842 nomenclature-iamc-0.9.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.364842 nomenclature-iamc-0.9.1/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.368842 nomenclature-iamc-0.9.1/doc/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/doc/source/_static/EU-logo-300x201.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/doc/source/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)   172467 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/doc/source/_static/iamc-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/doc/source/_static/open_entrance-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.368842 nomenclature-iamc-0.9.1/doc/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/doc/source/_templates/navigation.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.368842 nomenclature-iamc-0.9.1/doc/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/doc/source/api/codelist.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/doc/source/api/datastructuredefinition.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/doc/source/api/nomenclature.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/doc/source/api/regionprocessor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/doc/source/api/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/doc/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/doc/source/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.372842 nomenclature-iamc-0.9.1/doc/source/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/doc/source/user_guide/codelist.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/doc/source/user_guide/directory-structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/doc/source/user_guide/local-usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/doc/source/user_guide/model-mapping.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/doc/source/user_guide/model-registration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/doc/source/user_guide/region.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/doc/source/user_guide/variable.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/doc/source/user_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.372842 nomenclature-iamc-0.9.1/nomenclature/
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/nomenclature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/nomenclature/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/nomenclature/code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20045 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/nomenclature/codelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/nomenclature/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/nomenclature/definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.372842 nomenclature-iamc-0.9.1/nomenclature/error/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/nomenclature/error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/nomenclature/error/codelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/nomenclature/error/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/nomenclature/error/required_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/nomenclature/error/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.376842 nomenclature-iamc-0.9.1/nomenclature/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/nomenclature/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/nomenclature/processor/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22360 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/nomenclature/processor/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/nomenclature/processor/required_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/nomenclature/processor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/nomenclature/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/nomenclature/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.376842 nomenclature-iamc-0.9.1/nomenclature/validation_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/nomenclature/validation_schemas/generic_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/nomenclature/validation_schemas/region_mapping_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/nomenclature/validation_schemas/region_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/nomenclature/validation_schemas/tag_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/nomenclature/validation_schemas/variable_schema.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.380842 nomenclature-iamc-0.9.1/nomenclature_iamc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-22 08:26:10.000000 nomenclature-iamc-0.9.1/nomenclature_iamc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9436 2023-05-22 08:26:10.000000 nomenclature-iamc-0.9.1/nomenclature_iamc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:26:10.000000 nomenclature-iamc-0.9.1/nomenclature_iamc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-22 08:26:10.000000 nomenclature-iamc-0.9.1/nomenclature_iamc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-22 08:26:10.000000 nomenclature-iamc-0.9.1/nomenclature_iamc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-22 08:26:10.000000 nomenclature-iamc-0.9.1/nomenclature_iamc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-22 08:26:10.408842 nomenclature-iamc-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.380842 nomenclature-iamc-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.360842 nomenclature-iamc-0.9.1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.336842 nomenclature-iamc-0.9.1/tests/data/check_aggregate/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.336842 nomenclature-iamc-0.9.1/tests/data/check_aggregate/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.380842 nomenclature-iamc-0.9.1/tests/data/check_aggregate/components/region/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/check_aggregate/components/region/regions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.380842 nomenclature-iamc-0.9.1/tests/data/check_aggregate/components/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/check_aggregate/components/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.336842 nomenclature-iamc-0.9.1/tests/data/check_aggregate/components_dict/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.380842 nomenclature-iamc-0.9.1/tests/data/check_aggregate/components_dict/region/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/check_aggregate/components_dict/region/regions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.384842 nomenclature-iamc-0.9.1/tests/data/check_aggregate/components_dict/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/check_aggregate/components_dict/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.336842 nomenclature-iamc-0.9.1/tests/data/custom_dimension_nc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.384842 nomenclature-iamc-0.9.1/tests/data/custom_dimension_nc/region/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/custom_dimension_nc/region/regions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.384842 nomenclature-iamc-0.9.1/tests/data/custom_dimension_nc/scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/custom_dimension_nc/scenario/scenarios.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.384842 nomenclature-iamc-0.9.1/tests/data/custom_dimension_nc/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/custom_dimension_nc/variable/tag_fuel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/custom_dimension_nc/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.384842 nomenclature-iamc-0.9.1/tests/data/duplicate_code_raises/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/duplicate_code_raises/bar.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/duplicate_code_raises/foo.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.384842 nomenclature-iamc-0.9.1/tests/data/duplicate_tag_raises/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/duplicate_tag_raises/tag_1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/duplicate_tag_raises/tag_2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.336842 nomenclature-iamc-0.9.1/tests/data/empty_definitions_dir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.384842 nomenclature-iamc-0.9.1/tests/data/empty_definitions_dir/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/empty_definitions_dir/definitions/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.340842 nomenclature-iamc-0.9.1/tests/data/end_whitespace/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.340842 nomenclature-iamc-0.9.1/tests/data/end_whitespace/definitions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.384842 nomenclature-iamc-0.9.1/tests/data/end_whitespace/definitions/scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/end_whitespace/definitions/scenario/scenarios.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.384842 nomenclature-iamc-0.9.1/tests/data/excel_io/
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/excel_io/validation_nc.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/excel_io/validation_nc_duplicates.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/excel_io/validation_nc_flat.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/excel_io/validation_nc_list_arg.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/excel_io/validation_nc_list_arg.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.340842 nomenclature-iamc-0.9.1/tests/data/extras_nc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.384842 nomenclature-iamc-0.9.1/tests/data/extras_nc/region/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/extras_nc/region/regions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.384842 nomenclature-iamc-0.9.1/tests/data/extras_nc/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/extras_nc/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.340842 nomenclature-iamc-0.9.1/tests/data/failing_variable_codelist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.340842 nomenclature-iamc-0.9.1/tests/data/failing_variable_codelist/rename_arg_conflict/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.388842 nomenclature-iamc-0.9.1/tests/data/failing_variable_codelist/rename_arg_conflict/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/failing_variable_codelist/rename_arg_conflict/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.340842 nomenclature-iamc-0.9.1/tests/data/failing_variable_codelist/rename_undefined_target/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.388842 nomenclature-iamc-0.9.1/tests/data/failing_variable_codelist/rename_undefined_target/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/failing_variable_codelist/rename_undefined_target/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.340842 nomenclature-iamc-0.9.1/tests/data/failing_variable_codelist/unknown_weight/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.388842 nomenclature-iamc-0.9.1/tests/data/failing_variable_codelist/unknown_weight/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/failing_variable_codelist/unknown_weight/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.388842 nomenclature-iamc-0.9.1/tests/data/general_filtering/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/general_filtering/basic_codelist.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.340842 nomenclature-iamc-0.9.1/tests/data/hidden_character/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.344842 nomenclature-iamc-0.9.1/tests/data/hidden_character/definitions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.388842 nomenclature-iamc-0.9.1/tests/data/hidden_character/definitions/scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/hidden_character/definitions/scenario/scenarios.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.388842 nomenclature-iamc-0.9.1/tests/data/invalid_yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/invalid_yaml/foo.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.388842 nomenclature-iamc-0.9.1/tests/data/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/meta/meta_indicators_allowed_values.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.388842 nomenclature-iamc-0.9.1/tests/data/multiple_unit_codelist/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/multiple_unit_codelist/variable.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.344842 nomenclature-iamc-0.9.1/tests/data/non-default_dimensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.344842 nomenclature-iamc-0.9.1/tests/data/non-default_dimensions/definitions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.388842 nomenclature-iamc-0.9.1/tests/data/non-default_dimensions/definitions/region/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/non-default_dimensions/definitions/region/regions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.388842 nomenclature-iamc-0.9.1/tests/data/non-default_dimensions/definitions/scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/non-default_dimensions/definitions/scenario/scenarios.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.388842 nomenclature-iamc-0.9.1/tests/data/non-default_dimensions/definitions/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/non-default_dimensions/definitions/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.388842 nomenclature-iamc-0.9.1/tests/data/non-default_dimensions/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/non-default_dimensions/mappings/mapping_1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/non-default_dimensions/mappings/mapping_2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.344842 nomenclature-iamc-0.9.1/tests/data/non-default_dimensions_one_empty/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.344842 nomenclature-iamc-0.9.1/tests/data/non-default_dimensions_one_empty/definitions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.388842 nomenclature-iamc-0.9.1/tests/data/non-default_dimensions_one_empty/definitions/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/non-default_dimensions_one_empty/definitions/empty/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.388842 nomenclature-iamc-0.9.1/tests/data/non-default_dimensions_one_empty/definitions/region/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/non-default_dimensions_one_empty/definitions/region/regions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.388842 nomenclature-iamc-0.9.1/tests/data/non-default_dimensions_one_empty/definitions/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/non-default_dimensions_one_empty/definitions/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.392842 nomenclature-iamc-0.9.1/tests/data/non-default_dimensions_one_empty/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/non-default_dimensions_one_empty/mappings/mapping_1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/non-default_dimensions_one_empty/mappings/mapping_2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.344842 nomenclature-iamc-0.9.1/tests/data/non-default_folders/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.344842 nomenclature-iamc-0.9.1/tests/data/non-default_folders/def/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.392842 nomenclature-iamc-0.9.1/tests/data/non-default_folders/def/region/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/non-default_folders/def/region/regions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.392842 nomenclature-iamc-0.9.1/tests/data/non-default_folders/def/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/non-default_folders/def/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.392842 nomenclature-iamc-0.9.1/tests/data/non-default_folders/map/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/non-default_folders/map/mapping_1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/non-default_folders/map/mapping_2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.392842 nomenclature-iamc-0.9.1/tests/data/norway_as_bool/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/norway_as_bool/regions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.392842 nomenclature-iamc-0.9.1/tests/data/region_aggregation/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/region_aggregation/illegal_mapping_conflict_regions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/region_aggregation/illegal_mapping_duplicate_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/region_aggregation/illegal_mapping_illegal_attribute.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/region_aggregation/illegal_mapping_invalid_format_dict.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/region_aggregation/illegal_mapping_model_only.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/region_aggregation/illegal_mapping_native_duplicate_key.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/region_aggregation/illegal_mapping_native_rename_key_conflict.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/region_aggregation/illegal_mapping_native_rename_target_conflict_1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/region_aggregation/illegal_mapping_native_rename_target_conflict_2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/region_aggregation/working_mapping.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.392842 nomenclature-iamc-0.9.1/tests/data/region_codelist/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/region_codelist/region.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.352842 nomenclature-iamc-0.9.1/tests/data/region_processing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.396842 nomenclature-iamc-0.9.1/tests/data/region_processing/aggregate_only/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/region_processing/aggregate_only/aggregate_only.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.396842 nomenclature-iamc-0.9.1/tests/data/region_processing/complete_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/region_processing/complete_processing/model_a.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.396842 nomenclature-iamc-0.9.1/tests/data/region_processing/complete_processing_list/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/region_processing/complete_processing_list/model_a.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.348842 nomenclature-iamc-0.9.1/tests/data/region_processing/dsd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.396842 nomenclature-iamc-0.9.1/tests/data/region_processing/dsd/region/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/region_processing/dsd/region/regions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.396842 nomenclature-iamc-0.9.1/tests/data/region_processing/dsd/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/region_processing/dsd/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.396842 nomenclature-iamc-0.9.1/tests/data/region_processing/empty_aggregation/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/region_processing/empty_aggregation/model_a.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/region_processing/empty_aggregation/model_b.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.396842 nomenclature-iamc-0.9.1/tests/data/region_processing/no_mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/region_processing/no_mapping/.keep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.396842 nomenclature-iamc-0.9.1/tests/data/region_processing/partial_aggregation/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/region_processing/partial_aggregation/model_a.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.396842 nomenclature-iamc-0.9.1/tests/data/region_processing/rename_only/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/region_processing/rename_only/model_a.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/region_processing/rename_only/model_b.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/region_processing/rename_only/model_c.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.352842 nomenclature-iamc-0.9.1/tests/data/region_processing/skip_aggregation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.352842 nomenclature-iamc-0.9.1/tests/data/region_processing/skip_aggregation/dsd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.396842 nomenclature-iamc-0.9.1/tests/data/region_processing/skip_aggregation/dsd/region/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/region_processing/skip_aggregation/dsd/region/regions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.396842 nomenclature-iamc-0.9.1/tests/data/region_processing/skip_aggregation/dsd/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/region_processing/skip_aggregation/dsd/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.396842 nomenclature-iamc-0.9.1/tests/data/region_processing/skip_aggregation/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/region_processing/skip_aggregation/mappings/model_a.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/region_processing/skip_aggregation/mappings/model_b.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.352842 nomenclature-iamc-0.9.1/tests/data/region_processing/weighted_aggregation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.396842 nomenclature-iamc-0.9.1/tests/data/region_processing/weighted_aggregation/aggregate/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/region_processing/weighted_aggregation/aggregate/aggregate_only.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.352842 nomenclature-iamc-0.9.1/tests/data/region_processing/weighted_aggregation/dsd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.400842 nomenclature-iamc-0.9.1/tests/data/region_processing/weighted_aggregation/dsd/region/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/region_processing/weighted_aggregation/dsd/region/regions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.400842 nomenclature-iamc-0.9.1/tests/data/region_processing/weighted_aggregation/dsd/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/region_processing/weighted_aggregation/dsd/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.352842 nomenclature-iamc-0.9.1/tests/data/region_processing/weighted_aggregation_rename/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.400842 nomenclature-iamc-0.9.1/tests/data/region_processing/weighted_aggregation_rename/aggregate/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/region_processing/weighted_aggregation_rename/aggregate/aggregate_only.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.352842 nomenclature-iamc-0.9.1/tests/data/region_processing/weighted_aggregation_rename/dsd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.400842 nomenclature-iamc-0.9.1/tests/data/region_processing/weighted_aggregation_rename/dsd/region/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/region_processing/weighted_aggregation_rename/dsd/region/regions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.400842 nomenclature-iamc-0.9.1/tests/data/region_processing/weighted_aggregation_rename/dsd/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/region_processing/weighted_aggregation_rename/dsd/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.400842 nomenclature-iamc-0.9.1/tests/data/region_to_filter_codelist/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/region_to_filter_codelist/region_filtering.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.400842 nomenclature-iamc-0.9.1/tests/data/regionprocessor_duplicate/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/regionprocessor_duplicate/mapping_1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/regionprocessor_duplicate/mapping_2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.400842 nomenclature-iamc-0.9.1/tests/data/regionprocessor_exclude_region_overlap/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/regionprocessor_exclude_region_overlap/exclude_common_overlap.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/regionprocessor_exclude_region_overlap/exclude_native_overlap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.400842 nomenclature-iamc-0.9.1/tests/data/regionprocessor_not_defined/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/regionprocessor_not_defined/mapping_1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/regionprocessor_not_defined/mapping_2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.400842 nomenclature-iamc-0.9.1/tests/data/regionprocessor_unexpected_region/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/regionprocessor_unexpected_region/model_a.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.400842 nomenclature-iamc-0.9.1/tests/data/regionprocessor_working/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/regionprocessor_working/mapping_1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/regionprocessor_working/mapping_2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.356842 nomenclature-iamc-0.9.1/tests/data/required_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.356842 nomenclature-iamc-0.9.1/tests/data/required_data/definition/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.400842 nomenclature-iamc-0.9.1/tests/data/required_data/definition/region/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/required_data/definition/region/region.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.400842 nomenclature-iamc-0.9.1/tests/data/required_data/definition/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/required_data/definition/variable/variable.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.404842 nomenclature-iamc-0.9.1/tests/data/required_data/required_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/required_data/required_data/requiredData.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/required_data/required_data/requiredData_any_unit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/required_data/required_data/requiredData_apply_error.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/required_data/required_data/requiredData_apply_working.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/required_data/required_data/requiredData_multiple_units_allowed.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/required_data/required_data/requiredData_unknown_region.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/required_data/required_data/requiredData_unknown_unit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/required_data/required_data/requiredData_unknown_variable.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.404842 nomenclature-iamc-0.9.1/tests/data/simple_codelist/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/simple_codelist/foo.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.356842 nomenclature-iamc-0.9.1/tests/data/stray_tag/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.356842 nomenclature-iamc-0.9.1/tests/data/stray_tag/definitions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.404842 nomenclature-iamc-0.9.1/tests/data/stray_tag/definitions/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/stray_tag/definitions/variable/tag_fuel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/stray_tag/definitions/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.360842 nomenclature-iamc-0.9.1/tests/data/structure_validation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.360842 nomenclature-iamc-0.9.1/tests/data/structure_validation/definitions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.404842 nomenclature-iamc-0.9.1/tests/data/structure_validation/definitions/region/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/structure_validation/definitions/region/regions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.404842 nomenclature-iamc-0.9.1/tests/data/structure_validation/definitions/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/structure_validation/definitions/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.404842 nomenclature-iamc-0.9.1/tests/data/structure_validation/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/structure_validation/mappings/mapping_1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/structure_validation/mappings/mapping_2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.360842 nomenclature-iamc-0.9.1/tests/data/structure_validation_fails/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.360842 nomenclature-iamc-0.9.1/tests/data/structure_validation_fails/definitions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.404842 nomenclature-iamc-0.9.1/tests/data/structure_validation_fails/definitions/region/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/structure_validation_fails/definitions/region/regions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.404842 nomenclature-iamc-0.9.1/tests/data/structure_validation_fails/definitions/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/structure_validation_fails/definitions/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.404842 nomenclature-iamc-0.9.1/tests/data/structure_validation_fails/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/structure_validation_fails/mappings/mapping_1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/structure_validation_fails/mappings/mapping_2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.360842 nomenclature-iamc-0.9.1/tests/data/structure_validation_no_mappings/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.360842 nomenclature-iamc-0.9.1/tests/data/structure_validation_no_mappings/definitions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.404842 nomenclature-iamc-0.9.1/tests/data/structure_validation_no_mappings/definitions/region/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/structure_validation_no_mappings/definitions/region/regions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.404842 nomenclature-iamc-0.9.1/tests/data/structure_validation_no_mappings/definitions/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/structure_validation_no_mappings/definitions/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.408842 nomenclature-iamc-0.9.1/tests/data/tagged_codelist/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/tagged_codelist/foo.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/tagged_codelist/tag_sector.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/tagged_codelist/tag_source.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.360842 nomenclature-iamc-0.9.1/tests/data/validation_nc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.408842 nomenclature-iamc-0.9.1/tests/data/validation_nc/region/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/validation_nc/region/regions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.408842 nomenclature-iamc-0.9.1/tests/data/validation_nc/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/validation_nc/variable/tag_fuel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/validation_nc/variable/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:10.408842 nomenclature-iamc-0.9.1/tests/data/variable_codelist_complex_attr/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/data/variable_codelist_complex_attr/variable_complex_attr.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/test_check_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/test_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/test_codelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15827 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/test_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/test_definition_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/test_region_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/test_required_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-05-22 08:25:55.000000 nomenclature-iamc-0.9.1/tests/test_validation.py
```

### Comparing `nomenclature-iamc-0.9/.github/workflows/build-docs.yml` & `nomenclature-iamc-0.9.1/.github/workflows/build-docs.yml`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/.github/workflows/nightly.yaml` & `nomenclature-iamc-0.9.1/.github/workflows/nightly.yaml`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/.github/workflows/publish.yaml` & `nomenclature-iamc-0.9.1/.github/workflows/publish.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Workflow created according to: https://packaging.python.org/en/latest/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/
 name: Publish to PyPI and TestPyPI
 
-on: 
+on:
   push:
     tags: ["v*"]
   release:
     types: ["published"]
 
 jobs:
   build-n-publish:
@@ -32,14 +32,14 @@
         --outdir dist/
     - name: Publish distribution to Test PyPI
       uses: pypa/gh-action-pypi-publish@release/v1
       # Only run for testing
       if: github.event_name != 'release'
       with:
         password: ${{ secrets.TESTPYPI_TOKEN }}
-        repository_url: https://test.pypi.org/legacy/
+        repository-url: https://test.pypi.org/legacy/
     - name: Publish distribution to PyPI
       uses: pypa/gh-action-pypi-publish@release/v1
       # Only run for actual release
       if: github.event_name == 'release'
       with:
         password: ${{ secrets.PYPI_TOKEN }}
```

### Comparing `nomenclature-iamc-0.9/.github/workflows/pytest.yml` & `nomenclature-iamc-0.9.1/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/.gitignore` & `nomenclature-iamc-0.9.1/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 nosetests.xml
 coverage.xml
 *.cover
 *.py,cover
 .hypothesis/
 .pytest_cache/
 # include xlsx files needed for testing
-!tests/data/*.xlsx
+!tests/data/**/*.xlsx
 
 # Translations
 *.mo
 *.pot
 
 # Django stuff:
 *.log
```

### Comparing `nomenclature-iamc-0.9/CITATION.cff` & `nomenclature-iamc-0.9.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/DEVELOPING.rst` & `nomenclature-iamc-0.9.1/DEVELOPING.rst`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/LICENSE` & `nomenclature-iamc-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/PKG-INFO` & `nomenclature-iamc-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomenclature-iamc
-Version: 0.9
+Version: 0.9.1
 Summary: Package for managing codelists & attributes for IAMC-format datasets
 Home-page: https://github.com/IAMconsortium/nomenclature
 Author: Scenario Services team, ECE program, IIASA
 Author-email: ece-scse@iiasa.ac.at
 License: APACHE-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `nomenclature-iamc-0.9/README.md` & `nomenclature-iamc-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/doc/Makefile` & `nomenclature-iamc-0.9.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/doc/make.bat` & `nomenclature-iamc-0.9.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/doc/source/_static/EU-logo-300x201.jpg` & `nomenclature-iamc-0.9.1/doc/source/_static/EU-logo-300x201.jpg`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/doc/source/_static/iamc-logo.png` & `nomenclature-iamc-0.9.1/doc/source/_static/iamc-logo.png`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/doc/source/_static/open_entrance-logo.png` & `nomenclature-iamc-0.9.1/doc/source/_static/open_entrance-logo.png`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/doc/source/_templates/navigation.html` & `nomenclature-iamc-0.9.1/doc/source/_templates/navigation.html`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/doc/source/cli.rst` & `nomenclature-iamc-0.9.1/doc/source/cli.rst`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/doc/source/conf.py` & `nomenclature-iamc-0.9.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/doc/source/index.rst` & `nomenclature-iamc-0.9.1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/doc/source/installation.rst` & `nomenclature-iamc-0.9.1/doc/source/installation.rst`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/doc/source/user_guide/codelist.rst` & `nomenclature-iamc-0.9.1/doc/source/user_guide/codelist.rst`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/doc/source/user_guide/directory-structure.rst` & `nomenclature-iamc-0.9.1/doc/source/user_guide/directory-structure.rst`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/doc/source/user_guide/local-usage.rst` & `nomenclature-iamc-0.9.1/doc/source/user_guide/local-usage.rst`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/doc/source/user_guide/model-mapping.rst` & `nomenclature-iamc-0.9.1/doc/source/user_guide/model-mapping.rst`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/doc/source/user_guide/model-registration.rst` & `nomenclature-iamc-0.9.1/doc/source/user_guide/model-registration.rst`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/doc/source/user_guide/variable.rst` & `nomenclature-iamc-0.9.1/doc/source/user_guide/variable.rst`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/doc/source/user_guide.rst` & `nomenclature-iamc-0.9.1/doc/source/user_guide.rst`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/nomenclature/__init__.py` & `nomenclature-iamc-0.9.1/nomenclature/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 # get version number either from git (preferred) or metadata
 try:
     __version__ = get_version(Path(__file__).parents[1])
 except LookupError:
     __version__ = version("nomenclature-iamc")
 
 
-def create_yaml_from_xlsx(source, target, sheet_name, col, attrs=[]):
+def create_yaml_from_xlsx(source, target, sheet_name, col, attrs=None):
     """Parses an xlsx file with a codelist and writes a yaml file
 
     Parameters
     ----------
     source : str, path, file-like object
         Path to Excel file with definitions (codelists).
     target : str, path, file-like object
@@ -42,10 +42,12 @@
     sheet_name : str
         Sheet name of `source`.
     col : str
         Column from `sheet_name` to use as codes.
     attrs : list, optional
         Columns from `sheet_name` to use as attributes.
     """
+    if attrs is None:
+        attrs = []
     SPECIAL_CODELIST.get(col.lower(), CodeList).read_excel(
         name="", source=source, sheet_name=sheet_name, col=col, attrs=attrs
     ).to_yaml(target)
```

### Comparing `nomenclature-iamc-0.9/nomenclature/cli.py` & `nomenclature-iamc-0.9.1/nomenclature/cli.py`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/nomenclature/code.py` & `nomenclature-iamc-0.9.1/nomenclature/code.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 import json
 import re
+import pycountry
 from keyword import iskeyword
+from pathlib import Path
 from typing import Any, Dict, List, Optional, Set, Union
 
 from pydantic import BaseModel, Field, validator
 
 
 class Code(BaseModel):
     """A simple class for a mapping of a "code" to its attributes"""
 
     name: str
     description: Optional[str]
+    file: Optional[Union[str, Path]] = None
     extra_attributes: Dict[str, Any] = {}
 
+    def __eq__(self, other) -> bool:
+        return {key: value for key, value in self.dict().items() if key != "file"} == {
+            key: value for key, value in other.dict().items() if key != "file"
+        }
+
     @validator("extra_attributes")
     def check_attribute_names(cls, v, values):
         # Check that attributes only contains keys which are valid identifiers
         if illegal_keys := [
             key for key in v.keys() if not key.isidentifier() or iskeyword(key)
         ]:
             raise ValueError(
@@ -67,19 +75,22 @@
 
     @property
     def tags(self):
         return re.findall("(?<={).*?(?=})", self.name)
 
     @property
     def flattened_dict(self):
+        fields_set_alias = {
+            self.__fields__[field].alias for field in self.__fields_set__
+        }
         return {
             **{
                 k: v
                 for k, v in self.dict(by_alias=True).items()
-                if k != "extra_attributes"
+                if k != "extra_attributes" and k in fields_set_alias
             },
             **self.extra_attributes,
         }
 
     @property
     def flattened_dict_serialized(self):
         return {
@@ -205,7 +216,35 @@
         Name of the RegionCode
     hierarchy : str
         Hierarchy of the RegionCode
 
     """
 
     hierarchy: str = None
+    countries: List[str] = None
+
+    @validator("countries")
+    def check_iso3_codes(cls, v, values) -> List[str]:
+        """Verifies that each ISO3 code is valid according to pycountry library."""
+        invalid_iso3_codes: List[str] = []
+        for country in v:
+            if pycountry.countries.get(alpha_3=country) is None:
+                invalid_iso3_codes.append(country)
+        if invalid_iso3_codes:
+            raise ValueError(
+                f"Region {values['name']} has invalid"
+                f" ISO3 country codes: {invalid_iso3_codes}"
+            )
+        return v
+
+
+class MetaCode(Code):
+    """Code object with allowed values list
+
+    Attributes
+    ----------
+    allowed_values : Optional(list[any])
+        An optional list of allowed values
+
+    """
+
+    allowed_values: Optional[List[Any]]
```

### Comparing `nomenclature-iamc-0.9/nomenclature/codelist.py` & `nomenclature-iamc-0.9.1/nomenclature/codelist.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,37 @@
+import logging
 from pathlib import Path
 from typing import ClassVar, Dict, List
 
-import pandas as pd
 import numpy as np
+import pandas as pd
 import yaml
-import logging
 from jsonschema import validate
 from pyam.utils import write_sheet
 from pydantic import BaseModel, validator
 
-from nomenclature.code import Code, VariableCode, RegionCode
+from nomenclature.code import Code, VariableCode, RegionCode, MetaCode
 from nomenclature.error.codelist import DuplicateCodeError
 from nomenclature.error.variable import (
     MissingWeightError,
     VariableRenameArgError,
     VariableRenameTargetError,
 )
 
-
 here = Path(__file__).parent.absolute()
 
 
-def read_validation_schema(i):
-    with open(here / "validation_schemas" / f"{i}_schema.yaml", "r") as f:
+def read_validation_schema(schema):
+    with open(here / "validation_schemas" / f"{schema}_schema.yaml", "r") as f:
         schema = yaml.safe_load(f)
     return schema
 
 
 SCHEMA_TYPES = ("variable", "tag", "region", "generic")
-SCHEMA_MAPPING = dict([(i, read_validation_schema(i)) for i in SCHEMA_TYPES])
+SCHEMA_MAPPING = {schema: read_validation_schema(schema) for schema in SCHEMA_TYPES}
 
 
 class CodeList(BaseModel):
     """A class for nomenclature codelists & attributes
 
     Attributes
     ----------
@@ -46,14 +45,17 @@
     name: str
     mapping: Dict[str, Code] = {}
 
     # class variable
     validation_schema: ClassVar[str] = "generic"
     code_basis: ClassVar = Code
 
+    def __eq__(self, other):
+        return self.name == other.name and self.mapping == other.mapping
+
     @validator("mapping")
     def check_stray_tag(cls, v):
         """Check that no '{' are left in codes after tag replacement"""
         for code in v:
             if "{" in code:
                 raise ValueError(
                     f"Unexpected {{}} in codelist: {code}."
@@ -216,15 +218,15 @@
         for code in code_list:
             if code.name in mapping:
                 raise DuplicateCodeError(name=name, code=code.name)
             mapping[code.name] = code
         return cls(name=name, mapping=mapping)
 
     @classmethod
-    def read_excel(cls, name, source, sheet_name, col, attrs=[]):
+    def read_excel(cls, name, source, sheet_name, col, attrs=None):
         """Parses an xlsx file with a codelist
 
         Parameters
         ----------
         name : str
             Name of the CodeList
         source : str, path, file-like object
@@ -232,14 +234,16 @@
         sheet_name : str
             Sheet name of `source`.
         col : str
             Column from `sheet_name` to use as codes.
         attrs : list, optional
             Columns from `sheet_name` to use as attributes.
         """
+        if attrs is None:
+            attrs = []
         codelist = pd.read_excel(source, sheet_name=sheet_name, usecols=[col] + attrs)
 
         # replace nan with None
         codelist = codelist.replace(np.nan, None)
 
         # check for duplicates in the codelist
         duplicate_rows = codelist[col].duplicated(keep=False).values
@@ -267,33 +271,32 @@
         Parameters
         ----------
         path : :class:`pathlib.Path` or str, optional
             Write to file path if not None, otherwise return as stream
         """
 
         class Dumper(yaml.Dumper):
-            def increase_indent(self, flow=False, *args, **kwargs):
-                return super().increase_indent(flow=flow, indentless=False)
+            def increase_indent(self, flow: bool = False, indentless: bool = False):
+                return super().increase_indent(flow=flow, indentless=indentless)
 
         # translate to list of nested dicts, replace None by empty field, write to file
         stream = (
             yaml.dump(
                 [{code: attrs} for code, attrs in self.codelist_repr().items()],
                 sort_keys=False,
                 Dumper=Dumper,
             )
             .replace(": null\n", ":\n")
             .replace(": nan\n", ":\n")
         )
 
-        if path is not None:
-            with open(path, "w") as file:
-                file.write(stream)
-        else:
+        if path is None:
             return stream
+        with open(path, "w") as file:
+            file.write(stream)
 
     def to_pandas(self, sort_by_code: bool = False) -> pd.DataFrame:
         """Export the CodeList to a :class:`pandas.DataFrame`
 
         Parameters
         ----------
         sort_by_code : bool, optional
@@ -375,21 +378,15 @@
         nice_dict = {}
         for name, code in self.mapping.items():
             code_dict = (
                 code.flattened_dict_serialized
                 if json_serialized
                 else code.flattened_dict
             )
-            code_dict = {
-                k: v
-                for k, v in code_dict.items()
-                if (v is not None and k != "name") or k == "unit"
-            }
-
-            nice_dict[name] = code_dict
+            nice_dict[name] = {k: v for k, v in code_dict.items() if k != "name"}
 
         return nice_dict
 
     def filter(self, **kwargs) -> "CodeList":
         """Filter a CodeList by any attribute-value pairs.
 
         Parameters
@@ -402,29 +399,29 @@
         CodeList
             CodeList with Codes that match attribute-value pairs.
         """
 
         # Returns True if code satisfies all filter parameters
         def _match_attribute(code, kwargs):
             return all(
-                hasattr(code, attribute) and getattr(code, attribute, None) == value
+                hasattr(code, attribute) and getattr(code, attribute) == value
                 for attribute, value in kwargs.items()
             )
 
-        filtered_codelist = CodeList(
+        filtered_codelist = self.__class__(
             name=self.name,
             mapping={
                 code.name: code
                 for code in self.mapping.values()
                 if _match_attribute(code, kwargs)
             },
         )
 
         if not filtered_codelist.mapping:
-            logging.warning("Formatted data is empty!")
+            logging.warning(f"Filtered {self.__class__.__name__} is empty!")
         return filtered_codelist
 
 
 class VariableCodeList(CodeList):
     """A subclass of CodeList specified for variables
 
     Attributes
@@ -584,43 +581,24 @@
         """Return the hierarchies defined in the RegionCodeList
 
         Returns
         -------
         List[str]
 
         """
-        return sorted(list(set(v.hierarchy for v in self.mapping.values())))
-
-    def filter(self, hierarchy: str) -> "RegionCodeList":
-        """Return a filtered RegionCodeList object
-
-        Parameters
-        ----------
-        hierarchy : str
-            String with filter parameter.
+        return sorted(list({v.hierarchy for v in self.mapping.values()}))
 
-        Raises
-        ------
-        ValueError
-            Provided hierarchy is not compatible with the given model.
 
-        Returns
-        -------
-        :class:'RegionCodeList'
-
-        Notes
-        -----
-        The following arguments are available for filtering:
+class MetaCodeList(CodeList):
+    """A subclass of CodeList specified for MetaCodes
 
-        - 'hierarchy': filter by the hierarchy of each region
+    Attributes
+    ----------
+    name : str
+        Name of the MetaCodeList
+    mapping : dict
+        Dictionary of `MetaCode` objects
 
-        """
+    """
 
-        mapping = {k: v for k, v in self.mapping.items() if v.hierarchy == hierarchy}
-        if mapping:
-            return RegionCodeList(name=self.name, mapping=mapping)
-        else:
-            msg: str = (
-                f"Filtered RegionCodeList is empty: hierarchy={hierarchy}\n"
-                "Use `RegionCodeList.hierarchy` method for available items."
-            )
-            raise ValueError(msg)
+    code_basis: ClassVar = MetaCode
+    validation_schema: ClassVar[str] = "generic"
```

### Comparing `nomenclature-iamc-0.9/nomenclature/core.py` & `nomenclature-iamc-0.9.1/nomenclature/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-import copy
 import logging
-from typing import List, Optional
+from typing import Optional, Union, List
 
 import pyam
 from pydantic import validate_arguments
 
 from nomenclature.definition import DataStructureDefinition
-from nomenclature.processor import RegionProcessor
+from nomenclature.processor import Processor, RegionProcessor
 
 logger = logging.getLogger(__name__)
 
 
-@validate_arguments(config=dict(arbitrary_types_allowed=True))
+@validate_arguments(config={"arbitrary_types_allowed": True})
 def process(
     df: pyam.IamDataFrame,
     dsd: DataStructureDefinition,
     dimensions: Optional[List[str]] = None,
-    processor: Optional[RegionProcessor] = None,
+    processor: Optional[Union[Processor, List[Processor]]] = None,
 ) -> pyam.IamDataFrame:
     """Function for validation and region aggregation in one step
 
     This function is the recommended way of using the nomenclature package. It performs
     the following operations:
 
     * Validation against the codelists of a DataStructureDefinition
@@ -48,29 +47,30 @@
         Processed scenario data
 
     Raises
     ------
     ValueError
         If the :class:`pyam.IamDataFrame` fails the validation.
     """
-    # The deep copy is needed so we don't alter dsd in dimensions.remove("region")
-    dimensions = copy.deepcopy(dimensions or dsd.dimensions)
 
-    # perform validation and region-processing (optional)
-    if processor is None:
-        dsd.validate(df, dimensions=dimensions)
-    else:
-        if "region" in dimensions:
-            dimensions.remove("region")
-            dsd.validate(df, dimensions=dimensions)
-            df = processor.apply(df)
-            dsd.validate(df, dimensions=["region"])
-        else:
-            dsd.validate(df, dimensions=dimensions)
-            df = processor.apply(df)
+    processor = processor or []
+    processor = processor if isinstance(processor, list) else [processor]
+
+    dimensions = dimensions or dsd.dimensions
+
+    if (
+        any(isinstance(p, RegionProcessor) for p in processor)
+        and "region" in dimensions
+    ):
+        dimensions.remove("region")
+
+    dsd.validate(df, dimensions=dimensions)
+
+    for p in processor:
+        df = p.apply(df)
 
     # check consistency across the variable hierarchy
     error = dsd.check_aggregate(df)
     if error is not None:
         logger.error(f"These variables are not the sum of their components:\n{error}")
         raise ValueError("The validation failed. Please check the log for details.")
```

### Comparing `nomenclature-iamc-0.9/nomenclature/definition.py` & `nomenclature-iamc-0.9.1/nomenclature/definition.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,139 +1,152 @@
-import logging
-from pathlib import Path
-
-import pandas as pd
-from pyam import IamDataFrame
-from pyam.index import replace_index_labels
-from pyam.logging import adjust_log_level
-
-from nomenclature.codelist import CodeList, RegionCodeList, VariableCodeList
-from nomenclature.validation import validate
-
-logger = logging.getLogger(__name__)
-SPECIAL_CODELIST = {"variable": VariableCodeList, "region": RegionCodeList}
-
-
-class DataStructureDefinition:
-    """Definition of datastructure codelists for dimensions used in the IAMC format"""
-
-    def __init__(self, path, dimensions=["region", "variable"]):
-        """
-
-        Parameters
-        ----------
-        path : str or path-like
-            The folder with the project definitions.
-        dimensions : list of str, optional
-            List of :meth:`CodeList` names. Each CodeList is initialized
-            from a sub-folder of `path` of that name.
-        """
-        if not isinstance(path, Path):
-            path = Path(path)
-
-        if not path.is_dir():
-            raise NotADirectoryError(f"Definitions directory not found: {path}")
-
-        self.dimensions = dimensions
-        for dim in self.dimensions:
-            self.__setattr__(
-                dim, SPECIAL_CODELIST.get(dim, CodeList).from_directory(dim, path / dim)
-            )
-
-        empty = [d for d in self.dimensions if not self.__getattribute__(d)]
-        if empty:
-            raise ValueError(f"Empty codelist: {', '.join(empty)}")
-
-    def validate(self, df: IamDataFrame, dimensions: list = None) -> None:
-        """Validate that the coordinates of `df` are defined in the codelists
-
-        Parameters
-        ----------
-        df : :class:`pyam.IamDataFrame`
-            Scenario data to be validated against the codelists of this instance.
-        dimensions : list of str, optional
-            Dimensions to perform validation (defaults to all dimensions of self)
-
-        Returns
-        -------
-        None
-
-        Raises
-        ------
-        ValueError
-            If `df` fails validation against any codelist.
-        """
-        validate(self, df, dimensions=dimensions or self.dimensions)
-
-    def check_aggregate(self, df: IamDataFrame, **kwargs) -> None:
-        """Check for consistency of scenario data along the variable hierarchy
-
-        Parameters
-        ----------
-        df : :class:`pyam.IamDataFrame`
-            Scenario data to be checked for consistency along the variable hierarchy.
-        kwargs : Tolerance arguments for comparison of values
-            Passed to :any:`numpy.isclose` via :any:`pyam.IamDataFrame.check_aggregate`.
-
-        Returns
-        -------
-        :class:`pandas.DataFrame` or None
-            Data where a variable and its computed aggregate does not match.
-
-        Raises
-        ------
-        ValueError
-            If the :any:`DataStructureDefinition` does not have a *variable* dimension.
-        """
-        if "variable" not in self.dimensions:
-            raise ValueError("Aggregation check requires 'variable' dimension.")
-
-        lst = []
-
-        with adjust_log_level(level="WARNING"):
-            for code in df.variable:
-                attr = self.variable.mapping[code]
-                if attr.check_aggregate:
-                    components = attr.components
-
-                    # check if multiple lists of components are given for a code
-                    if isinstance(components, dict):
-                        for name, _components in components.items():
-                            error = df.check_aggregate(code, _components, **kwargs)
-                            if error is not None:
-                                error.dropna(inplace=True)
-                                # append components-name to variable column
-                                error.index = replace_index_labels(
-                                    error.index, "variable", [f"{code} [{name}]"]
-                                )
-                                lst.append(error)
-
-                    # else use components provided as single list or pyam-default (None)
-                    else:
-                        error = df.check_aggregate(code, components, **kwargs)
-                        if error is not None:
-                            lst.append(error.dropna())
-
-        if lst:
-            # there may be empty dataframes due to `dropna()` above
-            error = pd.concat(lst)
-            return error if not error.empty else None
-
-    def to_excel(
-        self, excel_writer, sheet_name=None, sort_by_code: bool = False, **kwargs
-    ):
-        """Write the *variable* codelist to an Excel sheet
-
-        Parameters
-        ----------
-        excel_writer : path-like, file-like, or ExcelWriter object
-            File path as string or :class:`pathlib.Path`,
-            or existing :class:`pandas.ExcelWriter`.
-        sheet_name : str, optional
-            Name of sheet that will have the codelist. If *None*, use the codelist name.
-        sort_by_code : bool, optional
-            Sort the codelist before exporting to file.
-        **kwargs
-            Passed to :class:`pandas.ExcelWriter` (if *excel_writer* is path-like).
-        """
-        # TODO write all dimensions to the file
-        self.variable.to_excel(excel_writer, sheet_name, sort_by_code, **kwargs)
+import logging
+from pathlib import Path
+
+import pandas as pd
+from pyam import IamDataFrame
+from pyam.index import replace_index_labels
+from pyam.logging import adjust_log_level
+
+from nomenclature.codelist import (
+    CodeList,
+    RegionCodeList,
+    VariableCodeList,
+    MetaCodeList,
+)
+from nomenclature.validation import validate
+
+logger = logging.getLogger(__name__)
+SPECIAL_CODELIST = {
+    "variable": VariableCodeList,
+    "region": RegionCodeList,
+    "meta": MetaCodeList,
+}
+
+
+class DataStructureDefinition:
+    """Definition of datastructure codelists for dimensions used in the IAMC format"""
+
+    def __init__(self, path, dimensions=None):
+        """
+
+        Parameters
+        ----------
+        path : str or path-like
+            The folder with the project definitions.
+        dimensions : list of str, optional
+            List of :meth:`CodeList` names. Each CodeList is initialized
+            from a sub-folder of `path` of that name.
+        """
+
+        if dimensions is None:
+            dimensions = ["region", "variable"]
+
+        if not isinstance(path, Path):
+            path = Path(path)
+
+        if not path.is_dir():
+            raise NotADirectoryError(f"Definitions directory not found: {path}")
+
+        self.dimensions = dimensions
+        for dim in self.dimensions:
+            self.__setattr__(
+                dim, SPECIAL_CODELIST.get(dim, CodeList).from_directory(dim, path / dim)
+            )
+
+        empty = [d for d in self.dimensions if not self.__getattribute__(d)]
+        if empty:
+            raise ValueError(f"Empty codelist: {', '.join(empty)}")
+
+    def validate(self, df: IamDataFrame, dimensions: list = None) -> None:
+        """Validate that the coordinates of `df` are defined in the codelists
+
+        Parameters
+        ----------
+        df : :class:`pyam.IamDataFrame`
+            Scenario data to be validated against the codelists of this instance.
+        dimensions : list of str, optional
+            Dimensions to perform validation (defaults to all dimensions of self)
+
+        Returns
+        -------
+        None
+
+        Raises
+        ------
+        ValueError
+            If `df` fails validation against any codelist.
+        """
+        validate(self, df, dimensions=dimensions or self.dimensions)
+
+    def check_aggregate(self, df: IamDataFrame, **kwargs) -> None:
+        """Check for consistency of scenario data along the variable hierarchy
+
+        Parameters
+        ----------
+        df : :class:`pyam.IamDataFrame`
+            Scenario data to be checked for consistency along the variable hierarchy.
+        kwargs : Tolerance arguments for comparison of values
+            Passed to :any:`numpy.isclose` via :any:`pyam.IamDataFrame.check_aggregate`.
+
+        Returns
+        -------
+        :class:`pandas.DataFrame` or None
+            Data where a variable and its computed aggregate does not match.
+
+        Raises
+        ------
+        ValueError
+            If the :any:`DataStructureDefinition` does not have a *variable* dimension.
+        """
+        if "variable" not in self.dimensions:
+            raise ValueError("Aggregation check requires 'variable' dimension.")
+
+        lst = []
+
+        with adjust_log_level(level="WARNING"):
+            for code in df.variable:
+                attr = self.variable.mapping[code]
+                if attr.check_aggregate:
+                    components = attr.components
+
+                    # check if multiple lists of components are given for a code
+                    if isinstance(components, dict):
+                        for name, _components in components.items():
+                            error = df.check_aggregate(code, _components, **kwargs)
+                            if error is not None:
+                                error.dropna(inplace=True)
+                                # append components-name to variable column
+                                error.index = replace_index_labels(
+                                    error.index, "variable", [f"{code} [{name}]"]
+                                )
+                                lst.append(error)
+
+                    # else use components provided as single list or pyam-default (None)
+                    else:
+                        error = df.check_aggregate(code, components, **kwargs)
+                        if error is not None:
+                            lst.append(error.dropna())
+
+        if lst:
+            # there may be empty dataframes due to `dropna()` above
+            error = pd.concat(lst)
+            return error if not error.empty else None
+
+    def to_excel(
+        self, excel_writer, sheet_name=None, sort_by_code: bool = False, **kwargs
+    ):
+        """Write the *variable* codelist to an Excel sheet
+
+        Parameters
+        ----------
+        excel_writer : path-like, file-like, or ExcelWriter object
+            File path as string or :class:`pathlib.Path`,
+            or existing :class:`pandas.ExcelWriter`.
+        sheet_name : str, optional
+            Name of sheet that will have the codelist. If *None*, use the codelist name.
+        sort_by_code : bool, optional
+            Sort the codelist before exporting to file.
+        **kwargs
+            Passed to :class:`pandas.ExcelWriter` (if *excel_writer* is path-like).
+        """
+        # TODO write all dimensions to the file
+        self.variable.to_excel(excel_writer, sheet_name, sort_by_code, **kwargs)
```

### Comparing `nomenclature-iamc-0.9/nomenclature/error/region.py` & `nomenclature-iamc-0.9.1/nomenclature/error/region.py`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/nomenclature/error/variable.py` & `nomenclature-iamc-0.9.1/nomenclature/error/variable.py`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/nomenclature/processor/region.py` & `nomenclature-iamc-0.9.1/nomenclature/processor/region.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from nomenclature.definition import DataStructureDefinition
 from nomenclature.error.region import (
     ExcludeRegionOverlapError,
     ModelMappingCollisionError,
     RegionNameCollisionError,
     RegionNotDefinedError,
 )
+from nomenclature.processor import Processor
 from nomenclature.processor.utils import get_relative_path
 
 logger = logging.getLogger(__name__)
 
 here = Path(__file__).parent.absolute()
 
 
@@ -77,18 +78,17 @@
     def is_single_constituent_region(self):
         return len(self.constituent_regions) == 1
 
     @property
     def rename_dict(self):
         if self.is_single_constituent_region:
             return {self.constituent_regions[0]: self.name}
-        else:
-            raise AttributeError(
-                "rename_dict is only available for single constituent regions"
-            )
+        raise AttributeError(
+            "rename_dict is only available for single constituent regions"
+        )
 
 
 class RegionAggregationMapping(BaseModel):
     """Hold information for region processing on a per-model basis.
 
     Region processing is comprised of native region selection and potentially renaming
     as well as aggregation to "common regions" (regions used for reporting and
@@ -218,54 +218,57 @@
 
         Notes
         -----
 
         This function is used to convert a model mapping yaml file into a dictionary
         which is used to initialize a RegionAggregationMapping.
         """
-        SCHEMA_FILE = here / "../validation_schemas" / "region_mapping_schema.yaml"
+        schema_file = here / "../validation_schemas" / "region_mapping_schema.yaml"
         file = Path(file) if isinstance(file, str) else file
         with open(file, "r") as f:
             mapping_input = yaml.safe_load(f)
-        with open(SCHEMA_FILE, "r") as f:
+        with open(schema_file, "r") as f:
             schema = yaml.safe_load(f)
 
         # Validate the input data using jsonschema
         try:
             jsonschema.validate(mapping_input, schema)
-        except jsonschema.ValidationError as e:
+        except jsonschema.ValidationError as error:
             # Add file information in case of error
             raise jsonschema.ValidationError(
-                f"{e.message} in {get_relative_path(file)}"
+                f"{error.message} in {get_relative_path(file)}"
             )
 
         # Add the file name to mapping_input
         mapping_input["file"] = get_relative_path(file)
 
         # Reformat the "native_regions"
         if "native_regions" in mapping_input:
             native_region_list: List[Dict] = []
-            for nr in mapping_input["native_regions"]:
-                if isinstance(nr, str):
-                    native_region_list.append({"name": nr})
-                elif isinstance(nr, dict):
+            for native_region in mapping_input["native_regions"]:
+                if isinstance(native_region, str):
+                    native_region_list.append({"name": native_region})
+                elif isinstance(native_region, dict):
                     native_region_list.append(
-                        {"name": list(nr)[0], "rename": list(nr.values())[0]}
+                        {
+                            "name": list(native_region)[0],
+                            "rename": list(native_region.values())[0],
+                        }
                     )
             mapping_input["native_regions"] = native_region_list
 
         # Reformat the "common_regions"
         if "common_regions" in mapping_input:
             common_region_list: List[Dict[str, List[Dict[str, str]]]] = []
-            for cr in mapping_input["common_regions"]:
-                cr_name = list(cr)[0]
+            for common_region in mapping_input["common_regions"]:
+                common_region_name = list(common_region)[0]
                 common_region_list.append(
                     {
-                        "name": cr_name,
-                        "constituent_regions": cr[cr_name],
+                        "name": common_region_name,
+                        "constituent_regions": common_region[common_region_name],
                     }
                 )
             mapping_input["common_regions"] = common_region_list
         return cls(**mapping_input)
 
     @property
     def all_regions(self) -> List[str]:
@@ -309,15 +312,15 @@
                 "'common_regions' or 'exclude_regions' in model mapping for "
                 f"{self.model} in {self.file}. If they are not meant to be included "
                 "in the results add to the 'exclude_regions' section in the model "
                 "mapping to silence this error."
             )
 
 
-class RegionProcessor(BaseModel):
+class RegionProcessor(Processor):
     """Region aggregation mappings for scenario processing"""
 
     region_codelist: RegionCodeList
     variable_codelist: VariableCodeList
     mappings: Dict[str, RegionAggregationMapping]
 
     @classmethod
@@ -344,30 +347,30 @@
             Raised in case there are multiple mappings defined for the same model.
         """
         mapping_dict: Dict[str, RegionAggregationMapping] = {}
         errors: List[ErrorWrapper] = []
         for file in (f for f in path.glob("**/*") if f.suffix in {".yaml", ".yml"}):
             try:
                 mapping = RegionAggregationMapping.from_file(file)
-                for m in mapping.model:
-                    if m not in mapping_dict:
-                        mapping_dict[m] = mapping
+                for model in mapping.model:
+                    if model not in mapping_dict:
+                        mapping_dict[model] = mapping
                     else:
                         errors.append(
                             ErrorWrapper(
                                 ModelMappingCollisionError(
-                                    model=m,
+                                    model=model,
                                     file1=mapping.file,
-                                    file2=mapping_dict[m].file,
+                                    file2=mapping_dict[model].file,
                                 ),
                                 "__root__",
                             )
                         )
-            except (pydantic.ValidationError, jsonschema.ValidationError) as e:
-                errors.append(ErrorWrapper(e, "__root__"))
+            except (pydantic.ValidationError, jsonschema.ValidationError) as error:
+                errors.append(ErrorWrapper(error, "__root__"))
 
         if errors:
             raise pydantic.ValidationError(errors, model=RegionProcessor)
 
         if missing_dims := [
             dim for dim in ("region", "variable") if not hasattr(dsd, dim)
         ]:
@@ -404,31 +407,31 @@
         ------
         ValueError
             * If *df* contains regions that are not listed in the model mapping, or
             * If the region-processing results in an empty **IamDataFrame**.
         """
         processed_dfs: List[IamDataFrame] = []
         for model in df.model:
-
             model_df = df.filter(model=model)
 
             # if no mapping is defined the data frame is returned unchanged
             if model not in self.mappings:
                 logger.info(f"No model mapping found for model '{model}'")
                 processed_dfs.append(model_df)
 
             # otherwise we first rename, then aggregate
             else:
                 file = self.mappings[model].file
                 logger.info(
                     f"Applying region-processing for model '{model}' from '{file}'"
                 )
                 processed_dfs.append(self._apply_region_processing(model_df))
-
-        return pyam.concat(processed_dfs)
+        res = pyam.concat(processed_dfs)
+        self.region_codelist.validate_items(res.region)
+        return res
 
     def _apply_region_processing(self, model_df: IamDataFrame) -> IamDataFrame:
         """Apply the region processing for a single model"""
         if len(model_df.model) != 1:
             raise ValueError(
                 f"Must be called for a unique model, found: {model_df.model}"
             )
@@ -452,27 +455,26 @@
                 if not _df.empty:
                     _processed_data.append(
                         _df.rename(region=self.mappings[model].rename_mapping)._data
                     )
 
             # aggregate common regions
             if self.mappings[model].common_regions is not None:
-
-                for cr in self.mappings[model].common_regions:
+                for common_region in self.mappings[model].common_regions:
                     # if a common region is consists of a single native region, rename
-                    if cr.is_single_constituent_region:
-                        _df = model_df.filter(region=cr.constituent_regions[0]).rename(
-                            region=cr.rename_dict
-                        )
+                    if common_region.is_single_constituent_region:
+                        _df = model_df.filter(
+                            region=common_region.constituent_regions[0]
+                        ).rename(region=common_region.rename_dict)
                         if not _df.empty:
                             _processed_data.append(_df._data)
                         continue
 
                     # if there are multiple constituent regions, aggregate
-                    regions = [cr.name, cr.constituent_regions]
+                    regions = [common_region.name, common_region.constituent_regions]
 
                     # first, perform 'simple' aggregation (no arguments)
                     simple_vars = [
                         var.name
                         for var in self.variable_codelist.vars_default_args(
                             model_df.variable
                         )
@@ -536,21 +538,21 @@
         return IamDataFrame(_data, meta=model_df.meta)
 
 
 def _aggregate_region(df, var, *regions, **kwargs):
     """Perform region aggregation with kwargs catching inconsistent-index errors"""
     try:
         return df.aggregate_region(var, *regions, **kwargs)
-    except ValueError as e:
-        if str(e) == "Inconsistent index between variable and weight!":
+    except ValueError as error:
+        if str(error) == "Inconsistent index between variable and weight!":
             logger.info(
                 f"Could not aggregate '{var}' for region '{regions[0]}' ({kwargs})"
             )
         else:
-            raise e
+            raise error
 
 
 def _compare_and_merge(original: pd.Series, aggregated: pd.Series) -> IamDataFrame:
     """Compare and merge original and aggregated results"""
 
     # compare processed (aggregated) data and data provided at the common-region level
     compare = pd.merge(
```

### Comparing `nomenclature-iamc-0.9/nomenclature/testing.py` & `nomenclature-iamc-0.9.1/nomenclature/testing.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,42 +59,41 @@
             RegionProcessor.from_directory(path / "mappings", dsd)
     elif (path / mappings).is_dir():
         RegionProcessor.from_directory(path / mappings, dsd)
     else:
         raise FileNotFoundError(f"Mappings directory not found: {path / mappings}")
 
 
-def _collect_requiredData_errors(
-    requiredDatadir: Path, dsd: DataStructureDefinition
+def _collect_RequiredData_errors(
+    required_data_dir: Path, dsd: DataStructureDefinition
 ) -> None:
     errors: List[str] = []
-    for file in (requiredDatadir).iterdir():
+    for file in required_data_dir.iterdir():
         try:
             RequiredDataValidator.from_file(file).validate_with_definition(dsd)
         except pydantic.ValidationError as pve:
             errors.append(str(pve))
     if errors:
         all_errors = "\n".join(errors)
         raise ValueError(f"Found error(s) in required data files: {all_errors}")
 
 
-def _check_requiredData(
+def _check_RequiredData(
     path: Path,
     definitions: str = "definitions",
     dimensions: Optional[List[str]] = None,
     required_data: Optional[str] = None,
 ) -> None:
-
     dsd = DataStructureDefinition(path / definitions, dimensions)
     if required_data is None:
         if (path / "requiredData").is_dir():
-            _collect_requiredData_errors(path / "required_data", dsd)
+            _collect_RequiredData_errors(path / "required_data", dsd)
 
     elif (path / required_data).is_dir():
-        _collect_requiredData_errors(path / required_data, dsd)
+        _collect_RequiredData_errors(path / required_data, dsd)
     else:
         raise FileNotFoundError(
             f"Directory for required data not found at: {path / required_data}"
         )
 
 
 def assert_valid_structure(
@@ -140,11 +139,11 @@
     if dimensions is None:  # if "dimensions" were not specified
         dimensions = [x.stem for x in (path / definitions).iterdir() if x.is_dir()]
         if not dimensions:
             raise FileNotFoundError(
                 f"`definitions` directory is empty: {path / definitions}"
             )
     _check_mappings(path, definitions, dimensions, mappings)
-    _check_requiredData(path, definitions, dimensions, required_data)
+    _check_RequiredData(path, definitions, dimensions, required_data)
 
 
 # Todo: add function which runs `DataStructureDefinition(path).validate(scenario)`
```

### Comparing `nomenclature-iamc-0.9/nomenclature/validation.py` & `nomenclature-iamc-0.9.1/nomenclature/validation.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,48 +20,40 @@
     """Validation of an IamDataFrame against codelists of a DataStructureDefinition"""
 
     if not isinstance(df, IamDataFrame):
         df = IamDataFrame(df)
 
     error = False
 
+    for dim in dimensions:
+        if invalid := getattr(dsd, dim).validate_items(getattr(df, dim)):
+            log_error(dim, invalid)
+            error = True
+
     if "variable" in dimensions:
-        # combined validation of variables and units
-        invalid_vars, invalid_units = [], []
+        # validation of variable, unit combinations
+        invalid_units = []
         for variable, unit in df.unit_mapping.items():
-            if variable not in dsd.variable:
-                invalid_vars.append(variable)
-            else:
+            if variable in dsd.variable:
                 dsd_unit = dsd.variable[variable].unit
                 # fast-pass for unique units in df and the DataStructureDefinition
                 if dsd_unit == unit:
                     continue
                 # full-fledged subset validation
                 if is_subset(unit, dsd_unit):
                     continue
                 invalid_units.append((variable, unit, dsd_unit))
 
-        if invalid_vars:
-            log_error("variable", invalid_vars)
-            error = True
-
         if invalid_units:
             lst = [
                 f"'{v}' - expected: {'one of ' if isinstance(e, list) else ''}"
                 f"'{e}', found: '{u}'"
                 for v, u, e in invalid_units
             ]
             msg = "The following variable(s) are reported with the wrong unit:"
             logger.error("\n - ".join([msg] + lst))
             error = True
 
-    # validation of all other dimensions
-    for dim in [d for d in dimensions if d != "variable"]:
-        invalid = dsd.__getattribute__(dim).validate_items(df.__getattribute__(dim))
-        if invalid:
-            log_error(dim, invalid)
-            error = True
-
     if error:
         raise ValueError("The validation failed. Please check the log for details.")
 
     return True
```

### Comparing `nomenclature-iamc-0.9/nomenclature/validation_schemas/region_mapping_schema.yaml` & `nomenclature-iamc-0.9.1/nomenclature/validation_schemas/region_mapping_schema.yaml`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/nomenclature/validation_schemas/region_schema.yaml` & `nomenclature-iamc-0.9.1/nomenclature/validation_schemas/region_schema.yaml`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/nomenclature/validation_schemas/tag_schema.yaml` & `nomenclature-iamc-0.9.1/nomenclature/validation_schemas/tag_schema.yaml`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/nomenclature/validation_schemas/variable_schema.yaml` & `nomenclature-iamc-0.9.1/nomenclature/validation_schemas/variable_schema.yaml`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/nomenclature_iamc.egg-info/PKG-INFO` & `nomenclature-iamc-0.9.1/nomenclature_iamc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomenclature-iamc
-Version: 0.9
+Version: 0.9.1
 Summary: Package for managing codelists & attributes for IAMC-format datasets
 Home-page: https://github.com/IAMconsortium/nomenclature
 Author: Scenario Services team, ECE program, IIASA
 Author-email: ece-scse@iiasa.ac.at
 License: APACHE-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `nomenclature-iamc-0.9/nomenclature_iamc.egg-info/SOURCES.txt` & `nomenclature-iamc-0.9.1/nomenclature_iamc.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 nomenclature/validation.py
 nomenclature/error/__init__.py
 nomenclature/error/codelist.py
 nomenclature/error/region.py
 nomenclature/error/required_data.py
 nomenclature/error/variable.py
 nomenclature/processor/__init__.py
+nomenclature/processor/processor.py
 nomenclature/processor/region.py
 nomenclature/processor/required_data.py
 nomenclature/processor/utils.py
 nomenclature/validation_schemas/generic_schema.yaml
 nomenclature/validation_schemas/region_mapping_schema.yaml
 nomenclature/validation_schemas/region_schema.yaml
 nomenclature/validation_schemas/tag_schema.yaml
@@ -72,40 +73,42 @@
 tests/test_core.py
 tests/test_definition.py
 tests/test_definition_variable.py
 tests/test_region_aggregation.py
 tests/test_required_data.py
 tests/test_testing.py
 tests/test_validation.py
-tests/data/validation_nc.xlsx
-tests/data/validation_nc_duplicates.xlsx
-tests/data/validation_nc_flat.yaml
-tests/data/validation_nc_list_arg.xlsx
 tests/data/check_aggregate/components/region/regions.yaml
 tests/data/check_aggregate/components/variable/variables.yaml
 tests/data/check_aggregate/components_dict/region/regions.yaml
 tests/data/check_aggregate/components_dict/variable/variables.yaml
 tests/data/custom_dimension_nc/region/regions.yaml
 tests/data/custom_dimension_nc/scenario/scenarios.yaml
 tests/data/custom_dimension_nc/variable/tag_fuel.yaml
 tests/data/custom_dimension_nc/variable/variables.yaml
 tests/data/duplicate_code_raises/bar.yaml
 tests/data/duplicate_code_raises/foo.yaml
 tests/data/duplicate_tag_raises/tag_1.yaml
 tests/data/duplicate_tag_raises/tag_2.yaml
 tests/data/empty_definitions_dir/definitions/.gitkeep
 tests/data/end_whitespace/definitions/scenario/scenarios.yaml
+tests/data/excel_io/validation_nc.xlsx
+tests/data/excel_io/validation_nc_duplicates.xlsx
+tests/data/excel_io/validation_nc_flat.yaml
+tests/data/excel_io/validation_nc_list_arg.xlsx
+tests/data/excel_io/validation_nc_list_arg.yaml
 tests/data/extras_nc/region/regions.yaml
 tests/data/extras_nc/variable/variables.yaml
 tests/data/failing_variable_codelist/rename_arg_conflict/variable/variables.yaml
 tests/data/failing_variable_codelist/rename_undefined_target/variable/variables.yaml
 tests/data/failing_variable_codelist/unknown_weight/variable/variables.yaml
 tests/data/general_filtering/basic_codelist.yaml
 tests/data/hidden_character/definitions/scenario/scenarios.yaml
 tests/data/invalid_yaml/foo.yaml
+tests/data/meta/meta_indicators_allowed_values.yaml
 tests/data/multiple_unit_codelist/variable.yaml
 tests/data/non-default_dimensions/definitions/region/regions.yaml
 tests/data/non-default_dimensions/definitions/scenario/scenarios.yaml
 tests/data/non-default_dimensions/definitions/variable/variables.yaml
 tests/data/non-default_dimensions/mappings/mapping_1.yaml
 tests/data/non-default_dimensions/mappings/mapping_2.yaml
 tests/data/non-default_dimensions_one_empty/definitions/empty/.gitkeep
@@ -160,16 +163,18 @@
 tests/data/regionprocessor_not_defined/mapping_2.yaml
 tests/data/regionprocessor_unexpected_region/model_a.yaml
 tests/data/regionprocessor_working/mapping_1.yml
 tests/data/regionprocessor_working/mapping_2.yaml
 tests/data/required_data/definition/region/region.yaml
 tests/data/required_data/definition/variable/variable.yaml
 tests/data/required_data/required_data/requiredData.yaml
+tests/data/required_data/required_data/requiredData_any_unit.yaml
 tests/data/required_data/required_data/requiredData_apply_error.yaml
 tests/data/required_data/required_data/requiredData_apply_working.yaml
+tests/data/required_data/required_data/requiredData_multiple_units_allowed.yaml
 tests/data/required_data/required_data/requiredData_unknown_region.yaml
 tests/data/required_data/required_data/requiredData_unknown_unit.yaml
 tests/data/required_data/required_data/requiredData_unknown_variable.yaml
 tests/data/simple_codelist/foo.yaml
 tests/data/stray_tag/definitions/variable/tag_fuel.yaml
 tests/data/stray_tag/definitions/variable/variables.yaml
 tests/data/structure_validation/definitions/region/regions.yaml
```

### Comparing `nomenclature-iamc-0.9/setup.cfg` & `nomenclature-iamc-0.9.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 	setuptools >= 41
 	pydantic
 	pyyaml
 	jsonschema
 	setuptools_scm
 	pandas >= 1.5.2
 	numpy
+	pycountry
 setup_requires = 
 	setuptools >= 41
 	setuptools_scm
 
 [options.extras_require]
 tests = 
 	pytest
```

### Comparing `nomenclature-iamc-0.9/tests/conftest.py` & `nomenclature-iamc-0.9.1/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,14 +43,7 @@
     """Add simple meta indicators"""
     if len(df.index) == 1:
         df.set_meta([1.0], "number")
         df.set_meta(["foo"], "string")
     if len(df.index) == 2:
         df.set_meta([1.0, 2.0], "number")
         df.set_meta(["foo", np.nan], "string")
-
-
-def remove_file_from_mapping(mapping: Dict[str, Code]) -> List[Dict]:
-    return [
-        {key: value for key, value in code.flattened_dict.items() if key != "file"}
-        for code in mapping.values()
-    ]
```

### Comparing `nomenclature-iamc-0.9/tests/data/check_aggregate/components/variable/variables.yaml` & `nomenclature-iamc-0.9.1/tests/data/check_aggregate/components/variable/variables.yaml`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/tests/data/check_aggregate/components_dict/variable/variables.yaml` & `nomenclature-iamc-0.9.1/tests/data/check_aggregate/components_dict/variable/variables.yaml`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/tests/data/region_processing/dsd/variable/variables.yaml` & `nomenclature-iamc-0.9.1/tests/data/region_processing/dsd/variable/variables.yaml`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/tests/data/validation_nc.xlsx` & `nomenclature-iamc-0.9.1/tests/data/excel_io/validation_nc_list_arg.xlsx`

 * *Files 26% similar despite different names*

#### zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 6599 bytes, number of entries: 16
-drwx---     2.0 fat        0 b- stor 23-Jan-16 10:53 _rels/
--rw----     2.0 fat      586 b- defN 23-Jan-16 10:53 _rels/.rels
-drwx---     2.0 fat        0 b- stor 23-Jan-16 10:53 docProps/
-drwx---     2.0 fat        0 b- stor 23-Jan-16 10:53 xl/
-drwx---     2.0 fat        0 b- stor 23-Jan-16 10:53 xl/theme/
--rw----     2.0 fat     7029 b- defN 23-Jan-16 10:53 xl/theme/theme1.xml
--rw----     2.0 fat      568 b- defN 23-Jan-16 10:53 docProps/core.xml
-drwx---     2.0 fat        0 b- stor 23-Jan-16 10:53 xl/worksheets/
--rw----     2.0 fat     2052 b- defN 23-Jan-16 10:53 xl/worksheets/sheet1.xml
--rw----     2.0 fat     2690 b- defN 23-Jan-16 10:53 xl/styles.xml
--rw----     2.0 fat     1166 b- defN 23-Jan-16 10:53 [Content_Types].xml
--rw----     2.0 fat      813 b- defN 23-Jan-16 10:53 docProps/app.xml
-drwx---     2.0 fat        0 b- stor 23-Jan-16 10:53 xl/_rels/
--rw----     2.0 fat      696 b- defN 23-Jan-16 10:53 xl/_rels/workbook.xml.rels
--rw----     2.0 fat      593 b- defN 23-Jan-16 10:53 xl/sharedStrings.xml
--rw----     2.0 fat      532 b- defN 23-Jan-16 10:53 xl/workbook.xml
-16 files, 16725 bytes uncompressed, 4901 bytes compressed:  70.7%
+Zip file size: 6593 bytes, number of entries: 16
+drwx---     2.0 fat        0 b- stor 23-May-10 16:55 _rels/
+-rw----     2.0 fat      586 b- defN 23-May-10 16:55 _rels/.rels
+drwx---     2.0 fat        0 b- stor 23-May-10 16:55 docProps/
+drwx---     2.0 fat        0 b- stor 23-May-10 16:55 xl/
+drwx---     2.0 fat        0 b- stor 23-May-10 16:55 xl/theme/
+-rw----     2.0 fat     7029 b- defN 23-May-10 16:55 xl/theme/theme1.xml
+-rw----     2.0 fat      568 b- defN 23-May-10 16:55 docProps/core.xml
+drwx---     2.0 fat        0 b- stor 23-May-10 16:55 xl/worksheets/
+-rw----     2.0 fat     1793 b- defN 23-May-10 16:55 xl/worksheets/sheet1.xml
+-rw----     2.0 fat     2690 b- defN 23-May-10 16:55 xl/styles.xml
+-rw----     2.0 fat     1166 b- defN 23-May-10 16:55 [Content_Types].xml
+-rw----     2.0 fat      813 b- defN 23-May-10 16:55 docProps/app.xml
+drwx---     2.0 fat        0 b- stor 23-May-10 16:55 xl/_rels/
+-rw----     2.0 fat      696 b- defN 23-May-10 16:55 xl/_rels/workbook.xml.rels
+-rw----     2.0 fat      628 b- defN 23-May-10 16:55 xl/sharedStrings.xml
+-rw----     2.0 fat      532 b- defN 23-May-10 16:55 xl/workbook.xml
+16 files, 16501 bytes uncompressed, 4895 bytes compressed:  70.3%
```

#### docProps/core.xml

##### docProps/core.xml

```diff
@@ -1,7 +1,7 @@
 <?xml version="1.0" encoding="utf-8"?>
 <cp:coreProperties xmlns:cp="http://schemas.openxmlformats.org/package/2006/metadata/core-properties" xmlns:dc="http://purl.org/dc/elements/1.1/" xmlns:dcterms="http://purl.org/dc/terms/" xmlns:dcmitype="http://purl.org/dc/dcmitype/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
   <dc:creator/>
   <cp:lastModifiedBy/>
-  <dcterms:created xsi:type="dcterms:W3CDTF">2023-01-16T09:53:34.095Z</dcterms:created>
-  <dcterms:modified xsi:type="dcterms:W3CDTF">2023-01-16T09:53:34.095Z</dcterms:modified>
+  <dcterms:created xsi:type="dcterms:W3CDTF">2023-05-10T14:55:01.935Z</dcterms:created>
+  <dcterms:modified xsi:type="dcterms:W3CDTF">2023-05-10T14:55:01.935Z</dcterms:modified>
 </cp:coreProperties>
```

#### xl/worksheets/sheet1.xml

##### xl/worksheets/sheet1.xml

```diff
@@ -1,23 +1,22 @@
 <?xml version="1.0" encoding="utf-8"?>
 <worksheet xmlns="http://schemas.openxmlformats.org/spreadsheetml/2006/main" xmlns:r="http://schemas.openxmlformats.org/officeDocument/2006/relationships" xmlns:mc="http://schemas.openxmlformats.org/markup-compatibility/2006" xmlns:x14ac="http://schemas.microsoft.com/office/spreadsheetml/2009/9/ac" mc:Ignorable="x14ac">
   <sheetPr>
     <outlinePr summaryBelow="0"/>
   </sheetPr>
-  <dimension ref="A1:E4"/>
+  <dimension ref="A1:D4"/>
   <sheetViews>
     <sheetView workbookViewId="0" tabSelected="1"/>
   </sheetViews>
   <sheetFormatPr defaultRowHeight="15" x14ac:dyDescent="0.25"/>
   <cols>
     <col min="1" max="1" style="5" width="21.005" customWidth="1" bestFit="1"/>
     <col min="2" max="2" style="5" width="47.005" customWidth="1" bestFit="1"/>
     <col min="3" max="3" style="6" width="7.005" customWidth="1" bestFit="1"/>
-    <col min="4" max="4" style="7" width="21.576428571428572" customWidth="1" bestFit="1"/>
-    <col min="5" max="5" style="7" width="16.290714285714284" customWidth="1" bestFit="1"/>
+    <col min="4" max="4" style="7" width="49.29071428571429" customWidth="1" bestFit="1"/>
   </cols>
   <sheetData>
     <row x14ac:dyDescent="0.25" r="1" customHeight="1" ht="19.5">
       <c r="A1" s="1" t="s">
         <v>0</v>
       </c>
       <c r="B1" s="1" t="s">
@@ -25,63 +24,47 @@
       </c>
       <c r="C1" s="1" t="s">
         <v>2</v>
       </c>
       <c r="D1" s="2" t="s">
         <v>3</v>
       </c>
-      <c r="E1" s="2" t="s">
-        <v>4</v>
-      </c>
     </row>
     <row x14ac:dyDescent="0.25" r="2" customHeight="1" ht="18.75">
       <c r="A2" s="2" t="s">
-        <v>5</v>
+        <v>4</v>
       </c>
       <c r="B2" s="2" t="s">
-        <v>6</v>
+        <v>5</v>
       </c>
       <c r="C2" s="2" t="s">
-        <v>7</v>
+        <v>6</v>
       </c>
       <c r="D2" s="3" t="s">
-        <v>8</v>
-      </c>
-      <c r="E2" s="3" t="s">
-        <v>8</v>
+        <v>7</v>
       </c>
     </row>
     <row x14ac:dyDescent="0.25" r="3" customHeight="1" ht="18.75">
       <c r="A3" s="2" t="s">
-        <v>9</v>
+        <v>8</v>
       </c>
       <c r="B3" s="2" t="s">
-        <v>10</v>
+        <v>9</v>
       </c>
       <c r="C3" s="2" t="s">
-        <v>7</v>
-      </c>
-      <c r="D3" s="3" t="s">
-        <v>8</v>
-      </c>
-      <c r="E3" s="3" t="s">
-        <v>8</v>
+        <v>6</v>
       </c>
+      <c r="D3" s="3"/>
     </row>
     <row x14ac:dyDescent="0.25" r="4" customHeight="1" ht="18.75">
       <c r="A4" s="2" t="s">
-        <v>11</v>
+        <v>10</v>
       </c>
       <c r="B4" s="2" t="s">
-        <v>12</v>
+        <v>11</v>
       </c>
       <c r="C4" s="4"/>
-      <c r="D4" s="3" t="s">
-        <v>8</v>
-      </c>
-      <c r="E4" s="3" t="s">
-        <v>8</v>
-      </c>
+      <c r="D4" s="3"/>
     </row>
   </sheetData>
   <pageMargins left="0.7" right="0.7" top="0.75" bottom="0.75" header="0.3" footer="0.3"/>
 </worksheet>
```

#### xl/sharedStrings.xml

##### xl/sharedStrings.xml

```diff
@@ -1,41 +1,38 @@
 <?xml version="1.0" encoding="utf-8"?>
-<sst xmlns="http://schemas.openxmlformats.org/spreadsheetml/2006/main" count="19" uniqueCount="13">
+<sst xmlns="http://schemas.openxmlformats.org/spreadsheetml/2006/main" count="13" uniqueCount="12">
   <si>
     <t>Variable</t>
   </si>
   <si>
     <t>Description</t>
   </si>
   <si>
     <t>Unit</t>
   </si>
   <si>
-    <t>Skip-region-aggregation</t>
-  </si>
-  <si>
-    <t>Check-aggregate</t>
+    <t>Region-aggregation</t>
   </si>
   <si>
     <t>Primary Energy</t>
   </si>
   <si>
     <t>Total primary energy consumption</t>
   </si>
   <si>
     <t>EJ/yr</t>
   </si>
   <si>
-    <t>false</t>
+    <t>[{&quot;Primary Energy (mean)&quot;: {&quot;method&quot;: &quot;mean&quot;}}]</t>
   </si>
   <si>
-    <t>Primary Energy|Coal</t>
+    <t>Primary Energy (mean)</t>
   </si>
   <si>
-    <t>Primary energy consumption of coal</t>
+    <t>Mean primary energy consumption</t>
   </si>
   <si>
     <t>Share|Coal</t>
   </si>
   <si>
     <t>Share of coal in the total primary energy mix</t>
   </si>
```

### Comparing `nomenclature-iamc-0.9/tests/data/validation_nc_duplicates.xlsx` & `nomenclature-iamc-0.9.1/tests/data/excel_io/validation_nc_duplicates.xlsx`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/tests/test_check_aggregate.py` & `nomenclature-iamc-0.9.1/tests/test_check_aggregate.py`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/tests/test_cli.py` & `nomenclature-iamc-0.9.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/tests/test_codelist.py` & `nomenclature-iamc-0.9.1/tests/test_codelist.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 import pytest
 import pandas as pd
 import pandas.testing as pdt
 import logging
 
-from nomenclature.code import Code, RegionCode
-from nomenclature.codelist import CodeList, VariableCodeList, RegionCodeList
+from nomenclature.code import Code, RegionCode, MetaCode
+from nomenclature.codelist import (
+    CodeList,
+    VariableCodeList,
+    RegionCodeList,
+    MetaCodeList,
+)
 from nomenclature.error.codelist import DuplicateCodeError
 
-from conftest import TEST_DATA_DIR, remove_file_from_mapping
+from conftest import TEST_DATA_DIR
 
 
 def test_simple_codelist():
     """Import a simple codelist"""
     code = VariableCodeList.from_directory(
         "variable", TEST_DATA_DIR / "simple_codelist"
     )
@@ -26,19 +31,18 @@
     code = VariableCodeList.from_directory(
         "variable", TEST_DATA_DIR / "simple_codelist"
     )
 
     assert code.to_yaml() == (
         "- Some Variable:\n"
         "    description: Some basic variable\n"
+        "    file: simple_codelist/foo.yaml\n"
         "    unit:\n"
         "    skip-region-aggregation: false\n"
-        "    check-aggregate: false\n"
         "    bool: true\n"
-        "    file: simple_codelist/foo.yaml\n"
     )
 
 
 def test_duplicate_code_raises():
     """Check that code conflicts across different files raises"""
     match = "Duplicate item in variable codelist: Some Variable"
     with pytest.raises(DuplicateCodeError, match=match):
@@ -109,29 +113,28 @@
     (
         VariableCodeList.from_directory(
             "Variable", TEST_DATA_DIR / "validation_nc" / "variable"
         ).to_excel(file)
     )
 
     obs = pd.read_excel(file)
-    exp = pd.read_excel(TEST_DATA_DIR / "validation_nc.xlsx")
+    exp = pd.read_excel(TEST_DATA_DIR / "excel_io" / "validation_nc.xlsx")
 
     pdt.assert_frame_equal(obs, exp)
 
 
-@pytest.mark.parametrize("sort", (True, False))
-def test_to_csv(sort):
+def test_to_csv():
     """Check writing to csv"""
     obs = VariableCodeList.from_directory(
         "Variable", TEST_DATA_DIR / "simple_codelist"
-    ).to_csv(sort_by_code=sort, lineterminator="\n")
+    ).to_csv(lineterminator="\n")
 
     exp = (
-        "Variable,Description,Unit,Skip-region-aggregation,Check-aggregate,Bool\n"
-        "Some Variable,Some basic variable,,False,False,True\n"
+        "Variable,Description,Unit,Skip-region-aggregation,Bool\n"
+        "Some Variable,Some basic variable,,False,True\n"
     )
     assert obs == exp
 
 
 def test_stray_tag_fails():
     """Check that typos in a tag raises expected error"""
 
@@ -172,20 +175,15 @@
         "variable",
         tmpdir / "output.xlsx",
         "variable",
         "Variable",
         attrs=["Description", "Unit", "Region-aggregation"],
     )
 
-    assert obs.name == exp.name
-    # since the obs and exp are read from different files, the file attribute will be
-    # different. For comparison we remove it
-    assert remove_file_from_mapping(obs.mapping) == remove_file_from_mapping(
-        exp.mapping
-    )
+    assert obs == exp
 
 
 def test_to_yaml_from_directory(tmp_path):
     """Test that creating a codelist from a yaml file and writing it to yaml produces
     the same file"""
 
     # read VariableCodeList
@@ -193,68 +191,41 @@
         "variable", TEST_DATA_DIR / "variable_codelist_complex_attr"
     )
     exp.to_yaml(tmp_path / "variables.yaml")
 
     # read from temporary file
     obs = VariableCodeList.from_directory("variable", tmp_path)
 
-    assert obs.name == exp.name
-    # since the obs and exp are read from different files, the file attribute will be
-    # different. For comparison we remove it
-    assert remove_file_from_mapping(obs.mapping) == remove_file_from_mapping(
-        exp.mapping
-    )
+    assert obs == exp
 
 
 def test_RegionCodeList_filter():
     """Test that verifies the hierarchy filter can sort through list of regions and
     give list of regions contained in the given hierarchy"""
 
     # read RegionCodeList
     rcl = RegionCodeList.from_directory(
         "Region", TEST_DATA_DIR / "region_to_filter_codelist"
     )
-    obs = rcl.filter("countries")
-    extra_attributes = {
-        "file": "region_to_filter_codelist/region_filtering.yaml",
-    }
+    obs = rcl.filter(hierarchy="countries")
+
     mapping = {
         "Some Country": RegionCode(
-            name="Some Country",
-            description="some small country",
-            extra_attributes=extra_attributes,
-            hierarchy="countries",
+            name="Some Country", description="some small country", hierarchy="countries"
         ),
         "Another Country": RegionCode(
             name="Another Country",
             description="another small country",
-            extra_attributes=extra_attributes,
             hierarchy="countries",
         ),
     }
     exp = RegionCodeList(name=rcl.name, mapping=mapping)
     assert obs == exp
 
 
-def test_RegionCodeList_filter_ValueError():
-    """Test that verifies the filter gives error when user inputs an unrecognizeable
-    hierarchy"""
-
-    # read RegionCodeList
-    rcl = RegionCodeList.from_directory(
-        "Region", TEST_DATA_DIR / "region_to_filter_codelist"
-    )
-    match = (
-        "Filtered RegionCodeList is empty: hierarchy=R77\n"
-        "Use `RegionCodeList.hierarchy` method for available items."
-    )
-    with pytest.raises(ValueError, match=match):
-        rcl.filter("R77")
-
-
 def test_RegionCodeList_hierarchy():
     """Verifies that the hierarchy method returns a List[str]"""
 
     rcl = RegionCodeList.from_directory(
         "Region", TEST_DATA_DIR / "region_to_filter_codelist"
     )
     assert rcl.hierarchy == ["common", "countries"]
@@ -265,15 +236,14 @@
     obs = var.filter(required=True)
     mapping = {
         "Big Variable": Code(
             name="Big Variable",
             description="Some basic variable",
             extra_attributes={
                 "required": True,
-                "file": "general_filtering/basic_codelist.yaml",
             },
         )
     }
     exp = CodeList(name=var.name, mapping=mapping)
     assert obs == exp
 
 
@@ -283,15 +253,14 @@
     mapping = {
         "Another Variable": Code(
             name="Another Variable",
             description="some details",
             extra_attributes={
                 "some_attribute": True,
                 "another_attribute": "This is true",
-                "file": "general_filtering/basic_codelist.yaml",
             },
         )
     }
     exp = CodeList(name=var.name, mapping=mapping)
     assert obs == exp
 
 
@@ -301,8 +270,26 @@
     with caplog.at_level(logging.WARNING):
         obs = var.filter(
             some_attribute=True, another_attribute="This is true", required=False
         )
         assert obs == CodeList(name="Variable", mapping={})
         assert len(caplog.records) == 1
         assert caplog.records[0].levelname == "WARNING"
-        assert caplog.records[0].message == "Formatted data is empty!"
+        assert caplog.records[0].message == "Filtered CodeList is empty!"
+
+
+def test_MetaCodeList_from_directory():
+    obs = MetaCodeList.from_directory(name="Meta", path=TEST_DATA_DIR / "meta")
+    mapping = {
+        "Meta category with boolean values": MetaCode(
+            name="Meta category with boolean values",
+            description=None,
+            allowed_values=[True, False],
+        ),
+        "Meta cat with int values": MetaCode(
+            name="Meta cat with int values",
+            description=None,
+            allowed_values=[1, 2, 3],
+        ),
+    }
+    exp = MetaCodeList(name="Meta", mapping=mapping)
+    assert obs == exp
```

### Comparing `nomenclature-iamc-0.9/tests/test_core.py` & `nomenclature-iamc-0.9.1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/tests/test_definition.py` & `nomenclature-iamc-0.9.1/tests/test_definition.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,19 +17,17 @@
     # check that "standard" dimensions are identical to simple test definitions
     assert obs.region == simple_definition.region
     assert obs.variable == simple_definition.variable
 
     # check that "custom" dimensions are as expected
     file = "scenario/scenarios.yaml"
     assert obs.scenario["scen_a"] == Code(
-        name="scen_a", extra_attributes={"attribute": "value", "file": file}
-    )
-    assert obs.scenario["scen_b"] == Code(
-        name="scen_b", extra_attributes={"file": file}
+        name="scen_a", extra_attributes={"attribute": "value"}
     )
+    assert obs.scenario["scen_b"] == Code(name="scen_b")
 
 
 def test_nonexisting_path_raises():
     """Check that initializing a DataStructureDefinition with non-existing path fails"""
     match = "Definitions directory not found: foo"
     with pytest.raises(NotADirectoryError, match=match):
         DataStructureDefinition("foo")
@@ -45,48 +43,52 @@
 def test_to_excel(simple_definition, tmpdir):
     """Check writing a DataStructureDefinition to file"""
     file = tmpdir / "testing_export.xlsx"
 
     simple_definition.to_excel(file)
 
     obs = pd.read_excel(file)
-    exp = pd.read_excel(TEST_DATA_DIR / "validation_nc.xlsx")
+    exp = pd.read_excel(TEST_DATA_DIR / "excel_io" / "validation_nc.xlsx")
     pd.testing.assert_frame_equal(obs, exp)
 
 
 @pytest.mark.parametrize(
-    "input_file, attrs",
+    "input_file, attrs, exp_file",
     [
-        ("validation_nc.xlsx", ["Description", "Unit"]),
-        ("validation_nc_list_arg.xlsx", ["Description", "Unit", "Region-aggregation"]),
+        ("validation_nc.xlsx", ["Description", "Unit"], "validation_nc_flat.yaml"),
+        (
+            "validation_nc_list_arg.xlsx",
+            ["Description", "Unit", "Region-aggregation"],
+            "validation_nc_list_arg.yaml",
+        ),
     ],
 )
-def test_create_yaml_from_xlsx(input_file, attrs, tmpdir):
+def test_create_yaml_from_xlsx(input_file, attrs, exp_file, tmpdir):
     """Check that creating a yaml codelist from xlsx yields the expected output file"""
     file = tmpdir / "foo.yaml"
 
     create_yaml_from_xlsx(
-        source=TEST_DATA_DIR / input_file,
+        source=TEST_DATA_DIR / "excel_io" / input_file,
         target=file,
         sheet_name="variable_definitions",
         col="Variable",
         attrs=attrs,
     )
 
     with open(file, "r") as f:
         obs = f.read()
-    with open(TEST_DATA_DIR / "validation_nc_flat.yaml", "r") as f:
+    with open(TEST_DATA_DIR / "excel_io" / exp_file, "r") as f:
         exp = f.read()
 
     assert obs == exp
 
 
 def test_create_yaml_from_xlsx_duplicate():
     """Check that creating a yaml codelist from xlsx with duplicates raises"""
     with pytest.raises(ValueError, match="Duplicate values in the codelist:"):
         create_yaml_from_xlsx(
-            source=TEST_DATA_DIR / "validation_nc_duplicates.xlsx",
+            source=TEST_DATA_DIR / "excel_io" / "validation_nc_duplicates.xlsx",
             target="_",
             sheet_name="duplicate_index_raises",
             col="Variable",
             attrs=["Unit", "Description"],
         )
```

### Comparing `nomenclature-iamc-0.9/tests/test_definition_variable.py` & `nomenclature-iamc-0.9.1/tests/test_definition_variable.py`

 * *Files identical despite different names*

### Comparing `nomenclature-iamc-0.9/tests/test_region_aggregation.py` & `nomenclature-iamc-0.9.1/tests/test_region_aggregation.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,14 @@
     "region_processor_path",
     [
         TEST_DATA_DIR / "regionprocessor_working",
         (TEST_DATA_DIR / "regionprocessor_working").relative_to(Path.cwd()),
     ],
 )
 def test_region_processor_working(region_processor_path, simple_definition):
-
     obs = RegionProcessor.from_directory(region_processor_path, simple_definition)
     exp_data = [
         {
             "model": ["model_a"],
             "file": (
                 TEST_DATA_DIR / "regionprocessor_working/mapping_1.yml"
             ).relative_to(Path.cwd()),
@@ -206,15 +205,14 @@
     ):
         RegionProcessor.from_directory(
             TEST_DATA_DIR / "regionprocessor_exclude_region_overlap", simple_definition
         )
 
 
 def test_region_processor_unexpected_region_raises():
-
     test_df = IamDataFrame(
         pd.DataFrame(
             [
                 ["model_a", "scen_a", "region_A", "Primary Energy", "EJ/yr", 1],
                 ["model_a", "scen_a", "region_B", "Primary Energy", "EJ/yr", 0.5],
             ],
             columns=IAMC_IDX + [2005],
```

### Comparing `nomenclature-iamc-0.9/tests/test_testing.py` & `nomenclature-iamc-0.9.1/tests/test_testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     """Check that a non-printable character in any yaml file will raise an error"""
     match = "scenarios.yaml, line 3, col 12."
     with pytest.raises(AssertionError, match=match):
         assert_valid_yaml(TEST_DATA_DIR / "hidden_character")
 
 
 def test_assert_valid_structure_requiredData_raises():
-
     with pytest.raises(ValueError) as e:
         assert_valid_structure(
             path=TEST_DATA_DIR / "required_data",
             definitions="definition",
             required_data="required_data",
         )
     # assert that all issues with requiredData files are reported correctly
```

### Comparing `nomenclature-iamc-0.9/tests/test_validation.py` & `nomenclature-iamc-0.9.1/tests/test_validation.py`

 * *Files identical despite different names*

