# Comparing `tmp/quartodoc-0.3.1.tar.gz` & `tmp/quartodoc-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quartodoc-0.3.1.tar", last modified: Mon May 15 17:26:31 2023, max compression
+gzip compressed data, was "quartodoc-0.3.3.tar", last modified: Fri Jun  2 14:27:05 2023, max compression
```

## Comparing `quartodoc-0.3.1.tar` & `quartodoc-0.3.3.tar`

### file list

```diff
@@ -1,130 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.040083 quartodoc-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.000081 quartodoc-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.012081 quartodoc-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-05-15 17:26:15.000000 quartodoc-0.3.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-15 17:26:15.000000 quartodoc-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-15 17:26:15.000000 quartodoc-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-15 17:26:15.000000 quartodoc-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-15 17:26:15.000000 quartodoc-0.3.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-15 17:26:31.040083 quartodoc-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-15 17:26:15.000000 quartodoc-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-15 17:26:15.000000 quartodoc-0.3.1/README.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.000081 quartodoc-0.3.1/_extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.012081 quartodoc-0.3.1/_extensions/interlinks/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 17:26:15.000000 quartodoc-0.3.1/_extensions/interlinks/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-15 17:26:15.000000 quartodoc-0.3.1/_extensions/interlinks/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-15 17:26:15.000000 quartodoc-0.3.1/_extensions/interlinks/_extension.yml
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-15 17:26:15.000000 quartodoc-0.3.1/_extensions/interlinks/example.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-05-15 17:26:15.000000 quartodoc-0.3.1/_extensions/interlinks/interlinks.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-15 17:26:15.000000 quartodoc-0.3.1/_extensions/interlinks/objects_siuba.json
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-15 17:26:15.000000 quartodoc-0.3.1/_extensions/interlinks/objects_vetiver.inv
--rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-05-15 17:26:15.000000 quartodoc-0.3.1/_extensions/interlinks/objects_vetiver.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.012081 quartodoc-0.3.1/case_studies/
--rw-r--r--   0 runner    (1001) docker     (123)    66407 2023-05-15 17:26:15.000000 quartodoc-0.3.1/case_studies/objects_sqla.inv
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-15 17:26:15.000000 quartodoc-0.3.1/case_studies/parsing.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-15 17:26:15.000000 quartodoc-0.3.1/case_studies/some_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-15 17:26:15.000000 quartodoc-0.3.1/case_studies/sphinx-inventory.md
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-15 17:26:15.000000 quartodoc-0.3.1/case_studies/sphinx-inventory.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.016082 quartodoc-0.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/about.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.016082 quartodoc-0.3.1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/examples/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.020082 quartodoc-0.3.1/docs/get-started/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/advanced-layouts.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/architecture.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/basic-building.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/basic-content.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/basic-docs.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/crossrefs.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/dev-big-picture.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/dev-dataclasses.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/dev-docstrings.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/dev-prepare.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/dev-renderers.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/docstring-examples.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/docstring-style.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/extending.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/extra-build-sequence.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/interlinks.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/overview.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/get-started/sidebar.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-15 17:26:15.000000 quartodoc-0.3.1/docs/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.020082 quartodoc-0.3.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.024082 quartodoc-0.3.1/examples/dascore/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/dascore/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/dascore/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/dascore/generate_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/dascore/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.024082 quartodoc-0.3.1/examples/pkgdown/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/pkgdown/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/pkgdown/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/pkgdown/objects.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.024082 quartodoc-0.3.1/examples/pkgdown/reference/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/pkgdown/reference/Builder.build.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/pkgdown/reference/Builder.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/pkgdown/reference/get_object.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/pkgdown/reference/index.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/pkgdown/reference/preview.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.028082 quartodoc-0.3.1/examples/single-page/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/single-page/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/single-page/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/single-page/objects.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.028082 quartodoc-0.3.1/examples/single-page/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/single-page/reference/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.028082 quartodoc-0.3.1/examples/weird-install/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/weird-install/_quarto.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.028082 quartodoc-0.3.1/examples/weird-install/src/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-15 17:26:15.000000 quartodoc-0.3.1/examples/weird-install/src/some_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-15 17:26:15.000000 quartodoc-0.3.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.028082 quartodoc-0.3.1/quartodoc/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)    18446 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/autosummary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.032082 quartodoc-0.3.1/quartodoc/builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/builder/_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/builder/blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/builder/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/builder/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/builder/write.py
--rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/interlinks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)    10134 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/layout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.036083 quartodoc-0.3.1/quartodoc/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/renderers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19557 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/renderers/md_renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.040083 quartodoc-0.3.1/quartodoc/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/example.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/example_alias_target.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/example_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/example_dynamic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.040083 quartodoc-0.3.1/quartodoc/tests/example_interlinks/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/example_interlinks/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.040083 quartodoc-0.3.1/quartodoc/tests/example_interlinks/_inv/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/example_interlinks/_inv/other_objects.json
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/example_interlinks/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/example_interlinks/objects.json
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/example_interlinks/spec.yml
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/example_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/test_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/test_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/test_builder_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/test_interlinks.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/test_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-15 17:26:15.000000 quartodoc-0.3.1/quartodoc/tests/test_renderers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:26:31.032082 quartodoc-0.3.1/quartodoc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-15 17:26:30.000000 quartodoc-0.3.1/quartodoc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-05-15 17:26:30.000000 quartodoc-0.3.1/quartodoc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 17:26:30.000000 quartodoc-0.3.1/quartodoc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-15 17:26:30.000000 quartodoc-0.3.1/quartodoc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-15 17:26:30.000000 quartodoc-0.3.1/quartodoc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 17:26:30.000000 quartodoc-0.3.1/quartodoc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-05-15 17:26:15.000000 quartodoc-0.3.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-15 17:26:31.040083 quartodoc-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.784204 quartodoc-0.3.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.764204 quartodoc-0.3.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-02 14:26:52.000000 quartodoc-0.3.3/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.764204 quartodoc-0.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-06-02 14:26:52.000000 quartodoc-0.3.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-02 14:26:52.000000 quartodoc-0.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-02 14:26:52.000000 quartodoc-0.3.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-02 14:26:52.000000 quartodoc-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-02 14:26:52.000000 quartodoc-0.3.3/MAINTAINERS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-02 14:26:52.000000 quartodoc-0.3.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-06-02 14:27:05.784204 quartodoc-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-02 14:26:52.000000 quartodoc-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-02 14:26:52.000000 quartodoc-0.3.3/README.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.760203 quartodoc-0.3.3/_extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.764204 quartodoc-0.3.3/_extensions/interlinks/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 14:26:52.000000 quartodoc-0.3.3/_extensions/interlinks/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-02 14:26:52.000000 quartodoc-0.3.3/_extensions/interlinks/_extension.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-06-02 14:26:52.000000 quartodoc-0.3.3/_extensions/interlinks/interlinks.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.764204 quartodoc-0.3.3/case_studies/
+-rw-r--r--   0 runner    (1001) docker     (123)    66407 2023-06-02 14:26:52.000000 quartodoc-0.3.3/case_studies/objects_sqla.inv
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-02 14:26:52.000000 quartodoc-0.3.3/case_studies/parsing.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-02 14:26:52.000000 quartodoc-0.3.3/case_studies/some_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-02 14:26:52.000000 quartodoc-0.3.3/case_studies/sphinx-inventory.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-02 14:26:52.000000 quartodoc-0.3.3/case_studies/sphinx-inventory.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.768204 quartodoc-0.3.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/about.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.768204 quartodoc-0.3.3/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/examples/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.772204 quartodoc-0.3.3/docs/get-started/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/advanced-layouts.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/architecture.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/basic-building.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/basic-content.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/basic-docs.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/crossrefs.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/dev-big-picture.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/dev-dataclasses.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/dev-docstrings.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/dev-prepare.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/dev-renderers.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/docstring-examples.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/docstring-style.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/extending.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/extra-build-sequence.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/interlinks.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/overview.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/get-started/sidebar.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-02 14:26:52.000000 quartodoc-0.3.3/docs/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.772204 quartodoc-0.3.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.772204 quartodoc-0.3.3/examples/dascore/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/dascore/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/dascore/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/dascore/generate_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/dascore/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.772204 quartodoc-0.3.3/examples/pkgdown/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/pkgdown/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/pkgdown/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/pkgdown/objects.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.772204 quartodoc-0.3.3/examples/pkgdown/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/pkgdown/reference/Builder.build.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/pkgdown/reference/Builder.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/pkgdown/reference/get_object.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/pkgdown/reference/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/pkgdown/reference/preview.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.772204 quartodoc-0.3.3/examples/single-page/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/single-page/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/single-page/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/single-page/objects.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.772204 quartodoc-0.3.3/examples/single-page/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/single-page/reference/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.772204 quartodoc-0.3.3/examples/weird-install/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/weird-install/_quarto.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.776203 quartodoc-0.3.3/examples/weird-install/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-02 14:26:52.000000 quartodoc-0.3.3/examples/weird-install/src/some_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-02 14:26:52.000000 quartodoc-0.3.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.776203 quartodoc-0.3.3/quartodoc/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19909 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/autosummary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.776203 quartodoc-0.3.3/quartodoc/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/builder/_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/builder/blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/builder/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/builder/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/builder/write.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/interlinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10266 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/layout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.780204 quartodoc-0.3.3/quartodoc/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/renderers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19955 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/renderers/md_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.780204 quartodoc-0.3.3/quartodoc/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/example_alias_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/example_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/example_dynamic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.784204 quartodoc-0.3.3/quartodoc/tests/example_interlinks/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/example_interlinks/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/example_interlinks/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.784204 quartodoc-0.3.3/quartodoc/tests/example_interlinks/_inv/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/example_interlinks/_inv/other_objects.json
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/example_interlinks/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/example_interlinks/interlinks.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/example_interlinks/objects.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/example_interlinks/spec.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/example_interlinks/test.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/example_interlinks/test.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/example_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/test_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/test_builder_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/test_interlinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/test_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-02 14:26:52.000000 quartodoc-0.3.3/quartodoc/tests/test_renderers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.776203 quartodoc-0.3.3/quartodoc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-06-02 14:27:05.000000 quartodoc-0.3.3/quartodoc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-06-02 14:27:05.000000 quartodoc-0.3.3/quartodoc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:27:05.000000 quartodoc-0.3.3/quartodoc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-02 14:27:05.000000 quartodoc-0.3.3/quartodoc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-02 14:27:05.000000 quartodoc-0.3.3/quartodoc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-02 14:27:05.000000 quartodoc-0.3.3/quartodoc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-06-02 14:26:52.000000 quartodoc-0.3.3/requirements-dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.760203 quartodoc-0.3.3/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:27:05.784204 quartodoc-0.3.3/scripts/filter-spec/
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-02 14:26:52.000000 quartodoc-0.3.3/scripts/filter-spec/generate_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-02 14:26:52.000000 quartodoc-0.3.3/scripts/filter-spec/generate_test_qmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-02 14:27:05.784204 quartodoc-0.3.3/setup.cfg
```

### Comparing `quartodoc-0.3.1/.github/workflows/ci.yml` & `quartodoc-0.3.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/.gitignore` & `quartodoc-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/LICENSE` & `quartodoc-0.3.3/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Michael Chow
+Copyright (c) 2023 quartodoc authors
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `quartodoc-0.3.1/PKG-INFO` & `quartodoc-0.3.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: quartodoc
-Version: 0.3.1
+Version: 0.3.3
 Summary: Generate API documentation with quarto.
 Home-page: https://github.com/machow/quartodoc
 Author: Michael Chow
-Author-email: mc_al_github@fastmail.com
+Author-email: michael.chow@posit.co
 License: MIT
 Keywords: documentation,quarto
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `quartodoc-0.3.1/README.md` & `quartodoc-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/README.qmd` & `quartodoc-0.3.3/README.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/case_studies/objects_sqla.inv` & `quartodoc-0.3.3/case_studies/objects_sqla.inv`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/case_studies/parsing.qmd` & `quartodoc-0.3.3/case_studies/parsing.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/case_studies/some_package.py` & `quartodoc-0.3.3/case_studies/some_package.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/case_studies/sphinx-inventory.md` & `quartodoc-0.3.3/case_studies/sphinx-inventory.md`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/case_studies/sphinx-inventory.qmd` & `quartodoc-0.3.3/case_studies/sphinx-inventory.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/docs/_quarto.yml` & `quartodoc-0.3.3/docs/_quarto.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/docs/examples/index.qmd` & `quartodoc-0.3.3/docs/examples/index.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/docs/get-started/architecture.qmd` & `quartodoc-0.3.3/docs/get-started/architecture.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/docs/get-started/basic-building.qmd` & `quartodoc-0.3.3/docs/get-started/basic-building.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/docs/get-started/basic-content.qmd` & `quartodoc-0.3.3/docs/get-started/basic-content.qmd`

 * *Files 11% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 ```yaml
 contents:
   - name: MdRenderer
     members:
       - render
 ```
 
-Behind the scenes, quartodoc represents each content entry as a [](`quartodoc.Auto`) element, since it specifies how to automatically document some object.
+In the following sections, we'll discuss different options for configuring content.
+
 
 ## Looking up objects
 
 Finding Python objects to document involves two pieces of configuration:
 
 * the package name.
 * a list of objects for content.
@@ -160,23 +161,33 @@
   sections:
     - title: Cool functions
       desc: ""
 
       # contents with a page grouping ----
       contents:
         - kind: page
+          path: some_funcs
           contents:
             - get_object
             - name: MdRenderer
               members: ["render"]
 ```
 
 :::
 ::::::
 
+Note these three important pieces of the page entry:
+
+* `kind: page` - indicates that we are creating a page
+* `path:` - specifies what the name of the page will be in the generated docs.
+  For example, `path: some_funcs` in the config above produces a file called
+  `some_funcs.qmd` in the API reference folder.
+* `contents:` - lists out the contents of the page.
+
+
 
 ## Setting default package path
 
 Different levels of configuration let you set the `package` option.
 This controls the package path that quartodoc will try to import control content from.
 
 The example below shows three different places it can be set:
@@ -200,14 +211,18 @@
         - preview            # quartodoc.ast.preview
 
         # (3) package set on a page
         - kind: page
           package: pandas
           contents:
             - DataFrame     # pandas.DataFrame
+        
+        # (4) package set on individual content entry
+        - package: pandas
+          name: Series
 ```
 
 Use `package: null` to unset the package option. This enables you to specify objects using their full name.
 
 ```yaml
 quartodoc:
   package: quartodoc
@@ -228,8 +243,8 @@
 
 In this case, you can set the dynamic option on a piece of content.
 
 ```yaml
 contents:
   - name: get_object
     dynamic: true
-```
+```
```

### Comparing `quartodoc-0.3.1/docs/get-started/basic-docs.qmd` & `quartodoc-0.3.3/docs/get-started/basic-docs.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/docs/get-started/crossrefs.qmd` & `quartodoc-0.3.3/docs/get-started/crossrefs.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/docs/get-started/dev-big-picture.qmd` & `quartodoc-0.3.3/docs/get-started/dev-big-picture.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/docs/get-started/dev-docstrings.qmd` & `quartodoc-0.3.3/docs/get-started/dev-docstrings.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/docs/get-started/dev-prepare.qmd` & `quartodoc-0.3.3/docs/get-started/dev-prepare.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/docs/get-started/dev-renderers.qmd` & `quartodoc-0.3.3/docs/get-started/dev-renderers.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/docs/get-started/docstring-examples.qmd` & `quartodoc-0.3.3/docs/get-started/docstring-examples.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/docs/get-started/extending.qmd` & `quartodoc-0.3.3/docs/get-started/extending.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/docs/get-started/extra-build-sequence.qmd` & `quartodoc-0.3.3/docs/get-started/extra-build-sequence.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/docs/get-started/interlinks.qmd` & `quartodoc-0.3.3/docs/get-started/interlinks.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/docs/get-started/overview.qmd` & `quartodoc-0.3.3/docs/get-started/overview.qmd`

 * *Files 3% similar despite different names*

```diff
@@ -42,17 +42,26 @@
 
 First, create a `_quarto.yml` file with the following:
 
 ```yaml
 project:
   type: website
 
+# tell quarto to read the generated sidebar
+metadata-files:
+  - _sidebar.yml
+
+
 quartodoc:
   # the name used to import the package
   package: quartodoc
+
+  # write sidebar data to this file
+  sidebar: _sidebar.yml
+
   sections:
     - title: Some functions
       desc: Functions to inspect docstrings.
       contents:
         # the functions being documented in the package.
         # you can refer to anything: class methods, modules, etc..
         - get_object
```

### Comparing `quartodoc-0.3.1/docs/get-started/sidebar.qmd` & `quartodoc-0.3.3/docs/get-started/sidebar.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/docs/styles.css` & `quartodoc-0.3.3/docs/styles.css`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/examples/dascore/_quarto.yml` & `quartodoc-0.3.3/examples/dascore/_quarto.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/examples/dascore/generate_api.py` & `quartodoc-0.3.3/examples/dascore/generate_api.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/examples/pkgdown/_quarto.yml` & `quartodoc-0.3.3/examples/pkgdown/_quarto.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/examples/pkgdown/objects.json` & `quartodoc-0.3.3/examples/pkgdown/objects.json`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/examples/pkgdown/reference/Builder.qmd` & `quartodoc-0.3.3/examples/pkgdown/reference/Builder.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/examples/pkgdown/reference/get_object.qmd` & `quartodoc-0.3.3/examples/pkgdown/reference/get_object.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/examples/single-page/_quarto.yml` & `quartodoc-0.3.3/examples/single-page/_quarto.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/examples/single-page/objects.json` & `quartodoc-0.3.3/examples/single-page/objects.json`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/examples/single-page/reference/index.qmd` & `quartodoc-0.3.3/examples/single-page/reference/index.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/quartodoc/__main__.py` & `quartodoc-0.3.3/quartodoc/__main__.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/quartodoc/ast.py` & `quartodoc-0.3.3/quartodoc/ast.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         try:
             return tuple_to_data(el)
         except ValueError:
             pass
 
     # patch a list of docstring sections. note that this has to happen on the
     # list, since we replace single nodes on the tree (the list is the node).
-    elif isinstance(el, list) and len(el) and isinstance(el[0], dc.DocstringSection):
+    elif isinstance(el, list) and len(el) and isinstance(el[0], ds.DocstringSection):
         return _DocstringSectionPatched.transform_all(el)
 
     return el
 
 
 # Patch DocstringSection ------------------------------------------------------
 
@@ -43,16 +43,16 @@
     warnings = "warnings"
 
 
 class _DocstringSectionPatched(ds.DocstringSection):
     _registry: "dict[Enum, _DocstringSectionPatched]" = {}
 
     def __init__(self, value: str, title: "str | None" = None):
-        self.value = value
         super().__init__(title)
+        self.value = value
 
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
 
         if cls.kind.value in cls._registry:
             raise KeyError(f"A section for kind {cls.kind} already exists")
 
@@ -156,17 +156,25 @@
 
 
 # Tree previewer ==============================================================
 
 
 @dispatch
 def fields(el: BaseModel):
+    # TODO: this is the only quartodoc specific code.
+    # pydantic seems to copy MISSING() when it's a default, so we can't
+    # whether a MISSING() is the default MISSING(). Instead, we'll just
+    # use isinstance for this particular class
+    from .layout import MISSING
+
     # return fields whose values were not set to the default
     field_defaults = {mf.name: mf.default for mf in el.__fields__.values()}
-    return [k for k, v in el if field_defaults[k] is not v]
+    return [
+        k for k, v in el if field_defaults[k] is not v if not isinstance(v, MISSING)
+    ]
 
 
 @dispatch
 def fields(el: dc.Object):
     options = [
         "name",
         "canonical_path",
@@ -329,15 +337,20 @@
         connector = "\n" + " " * pad + connector
         prefix = "\n" + " " * pad + prefix
         # NOTE: because visiting is depth first, this is essentially prepending
         # the text to the left.
         return prefix + connector.join(x.splitlines())
 
 
-def preview(ast: "dc.Object | ds.Docstring | object", max_depth=999, compact=False):
+def preview(
+    ast: "dc.Object | ds.Docstring | object",
+    max_depth=999,
+    compact=False,
+    as_string: bool = False,
+):
     """Print a friendly representation of a griffe object (e.g. function, docstring)
 
     Examples
     --------
 
     >>> from quartodoc import get_object
     >>> obj = get_object("quartodoc", "get_object")
@@ -345,8 +358,14 @@
     >>> preview(obj.docstring.parsed)
      ...
 
     >>> preview(obj)
      ...
 
     """
-    print(Formatter(max_depth=max_depth, compact=compact).format(ast))
+
+    res = Formatter(max_depth=max_depth, compact=compact).format(ast)
+
+    if as_string:
+        return res
+
+    print(res)
```

### Comparing `quartodoc-0.3.1/quartodoc/autosummary.py` & `quartodoc-0.3.3/quartodoc/autosummary.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,14 +95,18 @@
 
     Examples
     --------
 
     >>> get_function("quartodoc", "get_function")
     <Function('get_function', ...
 
+    Returns
+    -------
+    x:
+        abc
     """
 
     if object_name is not None:
         warnings.warn(
             "object_name argument is deprecated in get_object", DeprecationWarning
         )
 
@@ -198,15 +202,22 @@
         for child_obj in obj.members.values():
             replace_docstring(child_obj)
 
     if f is None:
         mod = importlib.import_module(obj.module.canonical_path)
 
         if isinstance(obj.parent, dc.Class):
-            f = getattr(getattr(mod, obj.parent.name), obj.name)
+            parent_obj = getattr(mod, obj.parent.name)
+
+            # we might fail to get the attribute if it is only a type annotation,
+            # and in that case need to bail out of the docstring replacement
+            try:
+                f = getattr(parent_obj, obj.name)
+            except AttributeError:
+                return
         else:
             f = getattr(mod, obj.name)
 
     # if no docstring on the dynamically loaded function, then stop
     # since there's nothing to update.
     # TODO: A static docstring could have been detected erroneously
     if f.__doc__ is None:
@@ -266,23 +277,40 @@
         parts = []
         crnt_part = mod
         for ii, attr_name in enumerate(splits):
             try:
                 crnt_part = getattr(crnt_part, attr_name)
                 if not isinstance(crnt_part, ModuleType) and not canonical_path:
                     canonical_path = crnt_part.__module__ + ":" + ".".join(splits[ii:])
+                elif isinstance(crnt_part, ModuleType) and ii == (len(splits) - 1):
+                    # final object is module
+                    canonical_path = crnt_part.__name__
 
                 parts.append(crnt_part)
             except AttributeError:
+                # Fetching the attribute can fail if it is purely a type hint,
+                # and has no value. This can be an issue if you have added a
+                # docstring below the annotation
+                if canonical_path:
+                    # See if we can return the static object for a value-less attr
+                    try:
+                        obj = get_object(canonical_path, loader=loader)
+                        print(obj)
+                        if _is_valueless(obj):
+                            return obj
+                    except Exception as e:
+                        # TODO: should we fail silently, so the error below triggers?
+                        raise e
+
                 raise AttributeError(
                     f"No attribute named `{attr_name}` in the path `{path}`."
                 )
 
         if canonical_path is None:
-            raise ValueError("Cannot find canonical path for `{path}`")
+            raise ValueError(f"Cannot find canonical path for `{path}`")
 
         attr = crnt_part
 
     # start loading object with griffe ----
 
     if target:
         obj = get_object(target, loader=loader)
@@ -305,14 +333,24 @@
         else:
             parent_path = mod_name.rsplit(".", 1)[0]
 
         parent = get_object(parent_path, loader=loader)
         return dc.Alias(attr_name, obj, parent=parent)
 
 
+def _is_valueless(obj: dc.Object):
+    if isinstance(obj, dc.Attribute):
+        if "class-attribute" in obj.labels and obj.value is None:
+            return True
+        elif "instance-attribute" in obj.labels:
+            return True
+
+    return False
+
+
 # pkgdown =====================================================================
 
 # TODO: styles -- pkgdown, single-page, many-pages
 class Builder:
     """Base class for building API docs.
 
     Parameters
```

### Comparing `quartodoc-0.3.1/quartodoc/builder/blueprint.py` & `quartodoc-0.3.3/quartodoc/builder/blueprint.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/quartodoc/builder/collect.py` & `quartodoc-0.3.3/quartodoc/builder/collect.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/quartodoc/builder/utils.py` & `quartodoc-0.3.3/quartodoc/builder/utils.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/quartodoc/interlinks.py` & `quartodoc-0.3.3/quartodoc/interlinks.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/quartodoc/inventory.py` & `quartodoc-0.3.3/quartodoc/inventory.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/quartodoc/layout.py` & `quartodoc-0.3.3/quartodoc/layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,25 +199,29 @@
         (Not implemented). A list of members to exclude.
     dynamic:
         Whether to dynamically load docstring. By default docstrings are loaded
         using static analysis. dynamic may be a string pointing to another object,
         to return an alias for that object.
     children:
         Style for presenting members. Either separate, embedded, or flat.
+    package:
+        If specified, object lookup will be relative to this path.
+
 
     """
 
     kind: Literal["auto"] = "auto"
     name: str
     members: Optional[list[str]] = None
     include_private: bool = False
     include: Optional[str] = None
     exclude: Optional[str] = None
     dynamic: Union[bool, str] = False
     children: ChoicesChildren = ChoicesChildren.embedded
+    package: Union[str, None, MISSING] = MISSING()
 
 
 # TODO: rename to Default or something
 class _AutoDefault(_Base):
     """This hacky class allows creating Auto as a default option in Pages and Sections."""
 
     __root__: Union[str, dict]
```

### Comparing `quartodoc-0.3.1/quartodoc/renderers/base.py` & `quartodoc-0.3.3/quartodoc/renderers/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,21 +6,24 @@
 # utils -----------------------------------------------------------------------
 
 
 def escape(val: str):
     return f"`{val}`"
 
 
-def sanitize(val: str):
-    return (
-        val.replace("\n", " ")
-        .replace("|", "\\|")
-        .replace("[", "\\[")
-        .replace("]", "\\]")
-    )
+def sanitize(val: str, allow_markdown=False):
+    # sanitize common tokens that break tables
+    res = val.replace("\n", " ").replace("|", "\\|")
+
+    # sanitize elements that can get interpreted as markdown links
+    # or citations
+    if not allow_markdown:
+        return res.replace("[", "\\[").replace("]", "\\]")
+
+    return res
 
 
 def convert_rst_link_to_md(rst):
     expr = (
         r"((:external(\+[a-zA-Z\._]+))?(:[a-zA-Z\._]+)?:[a-zA-Z\._]+:`~?[a-zA-Z\._]+`)"
     )
```

### Comparing `quartodoc-0.3.1/quartodoc/renderers/md_renderer.py` & `quartodoc-0.3.3/quartodoc/renderers/md_renderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,21 @@
 from plum import dispatch
 from typing import Tuple, Union, Optional
 from quartodoc import layout
 
 from .base import Renderer, escape, sanitize, convert_rst_link_to_md
 
 
+try:
+    # Name and Expression were moved to expressions in v0.28
+    from griffe import expressions as expr
+except ImportError:
+    from griffe import dataclasses as expr
+
+
 def _has_attr_section(el: dc.Docstring | None):
     if el is None:
         return False
 
     return any([isinstance(x, ds.DocstringSectionAttributes) for x in el.parsed])
 
 
@@ -91,30 +98,30 @@
             return el.path
 
         elif self.display_name == "canonical":
             return el.canonical_path
 
         raise ValueError(f"Unsupported display_name: `{self.display_name}`")
 
-    def render_annotation(self, el: "str | dc.Name | dc.Expression | None"):
+    def render_annotation(self, el: "str | expr.Name | expr.Expression | None"):
         """Special hook for rendering a type annotation.
 
         Parameters
         ----------
         el:
             An object representing a type annotation.
             
         """
 
         if isinstance(el, (type(None), str)):
             return el
 
         # TODO: maybe there is a way to get tabulate to handle this?
         # unescaped pipes screw up table formatting
-        if isinstance(el, dc.Name):
+        if isinstance(el, expr.Name):
             return sanitize(el.source)
 
         return sanitize(el.full)
 
     # signature method --------------------------------------------------------
 
     @dispatch
@@ -408,29 +415,35 @@
 
     @dispatch
     def render(self, el: ds.DocstringParameter) -> Tuple[str]:
         # TODO: if default is not, should return the word "required" (unescaped)
         default = "required" if el.default is None else escape(el.default)
 
         annotation = self.render_annotation(el.annotation)
-        return (escape(el.name), annotation, sanitize(el.description), default)
+        clean_desc = sanitize(el.description, allow_markdown=True)
+        return (escape(el.name), annotation, clean_desc, default)
 
     # attributes ----
 
     @dispatch
     def render(self, el: ds.DocstringSectionAttributes):
         header = ["Name", "Type", "Description"]
         rows = list(map(self.render, el.value))
 
         return tabulate(rows, header, tablefmt="github")
 
     @dispatch
     def render(self, el: ds.DocstringAttribute):
         annotation = self.render_annotation(el.annotation)
-        return el.name, self.render_annotation(annotation), el.description
+        row = [
+            sanitize(el.name),
+            self.render_annotation(annotation),
+            sanitize(el.description or "", allow_markdown=True)
+        ]
+        return row
 
     # warnings ----
 
     @dispatch
     def render(self, el: qast.DocstringSectionWarnings):
         return el.value
 
@@ -474,15 +487,15 @@
 
         return tabulate(rows, header, tablefmt="github")
 
     @dispatch
     def render(self, el: Union[ds.DocstringReturn, ds.DocstringRaise]):
         # similar to DocstringParameter, but no name or default
         annotation = self.render_annotation(el.annotation)
-        return (annotation, el.description)
+        return (annotation, sanitize(el.description, allow_markdown=True))
 
     # unsupported parts ----
 
     @dispatch.multi(
         (ds.DocstringAdmonition,),
         (ds.DocstringDeprecated,),
         (ds.DocstringWarn,),
@@ -496,15 +509,15 @@
     
     # Summarize ===============================================================
     # this method returns a summary description, such as a table summarizing a
     # layout.Section, or a row in the table for layout.Page or layout.DocFunction.
 
     @staticmethod
     def _summary_row(link, description):
-        return f"| {link} | {sanitize(description)} |"
+        return f"| {link} | {sanitize(description, allow_markdown=True)} |"
 
     @dispatch
     def summarize(self, el):
         """Produce a summary table."""
 
         raise NotImplementedError("Unsupported type: {type(el)}")
```

### Comparing `quartodoc-0.3.1/quartodoc/tests/example_dynamic.py` & `quartodoc-0.3.3/quartodoc/tests/example_dynamic.py`

 * *Files 23% similar despite different names*

```diff
@@ -22,7 +22,17 @@
 
     dynamic_doc.__doc__ = """A dynamic method"""
 
     # note that we could use the partialmethod, but I am not sure how to
     # correctly set its __doc__ attribute in that case.
     dynamic_create = partial(dynamic_doc, x=1)
     dynamic_create.__doc__ = dynamic_doc.__doc__
+
+
+class InstanceAttrs:
+    z: int
+    """The z attribute"""
+
+    def __init__(self, a: int, b: str):
+        self.a = a
+        self.b = b
+        """The b attribute"""
```

### Comparing `quartodoc-0.3.1/quartodoc/tests/example_interlinks/objects.json` & `quartodoc-0.3.3/quartodoc/tests/example_interlinks/objects.json`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/quartodoc/tests/example_interlinks/spec.yml` & `quartodoc-0.3.3/quartodoc/tests/example_interlinks/spec.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/quartodoc/tests/test_ast.py` & `quartodoc-0.3.3/quartodoc/tests/test_ast.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/quartodoc/tests/test_basic.py` & `quartodoc-0.3.3/quartodoc/tests/test_basic.py`

 * *Files 8% similar despite different names*

```diff
@@ -80,7 +80,19 @@
 
 
 def test_get_object_dynamic_class_method_doc():
     obj = get_object("quartodoc.tests.example_dynamic:AClass", dynamic=True)
 
     meth = obj.members["dynamic_create"]
     assert meth.docstring.value == "A dynamic method"
+
+
+def test_get_object_dynamic_class_instance_attr_doc():
+    obj = get_object("quartodoc.tests.example_dynamic:InstanceAttrs", dynamic=True)
+
+    assert obj.members["b"].docstring.value == "The b attribute"
+
+
+def test_get_object_dynamic_class_instance_attr_doc():
+    obj = get_object("quartodoc.tests.example_dynamic:InstanceAttrs", dynamic=True)
+
+    assert obj.members["z"].docstring.value == "The z attribute"
```

### Comparing `quartodoc-0.3.1/quartodoc/tests/test_builder.py` & `quartodoc-0.3.3/quartodoc/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/quartodoc/tests/test_builder_blueprint.py` & `quartodoc-0.3.3/quartodoc/tests/test_builder_blueprint.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,7 +66,16 @@
     auto = lo.Auto(name=path, members=["a_func"], dynamic=dynamic)
     res = bp.visit(auto)
 
     assert isinstance(res, lo.DocModule)
     assert len(res.members) == 1
     assert res.members[0].name == "a_func"
     assert res.members[0].obj.path == path.replace(":", ".") + ".a_func"
+
+
+def test_blueprint_auto_package(bp):
+    auto = lo.Auto(name="a_func", package="quartodoc.tests.example")
+    res = bp.visit(auto)
+
+    assert isinstance(res, lo.DocFunction)
+    assert res.name == "a_func"
+    assert res.anchor == "quartodoc.tests.example.a_func"
```

### Comparing `quartodoc-0.3.1/quartodoc/tests/test_interlinks.py` & `quartodoc-0.3.3/quartodoc/tests/test_interlinks.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     parse_md_style_link,
     Link,
 )
 from importlib_resources import files
 
 # load test spec at import time, so that we can feed each spec entry
 # as an individual test case using parametrize
-_raw = yaml.safe_load(open("quartodoc/tests/example_interlinks/spec.yml"))
+_raw = yaml.safe_load(open(files("quartodoc") / "tests/example_interlinks/spec.yml"))
 spec = TestSpec(__root__=_raw).__root__
 
 
 @pytest.fixture
 def invs():
     invs = Inventories.from_quarto_config(
         str(files("quartodoc") / "tests/example_interlinks/_quarto.yml")
```

### Comparing `quartodoc-0.3.1/quartodoc/tests/test_layout.py` & `quartodoc-0.3.3/quartodoc/tests/test_layout.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/quartodoc.egg-info/PKG-INFO` & `quartodoc-0.3.3/quartodoc.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: quartodoc
-Version: 0.3.1
+Version: 0.3.3
 Summary: Generate API documentation with quarto.
 Home-page: https://github.com/machow/quartodoc
 Author: Michael Chow
-Author-email: mc_al_github@fastmail.com
+Author-email: michael.chow@posit.co
 License: MIT
 Keywords: documentation,quarto
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `quartodoc-0.3.1/quartodoc.egg-info/SOURCES.txt` & `quartodoc-0.3.3/quartodoc.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 .gitignore
 .pre-commit-config.yaml
 LICENSE
+MAINTAINERS.md
 Makefile
 README.md
 README.qmd
 pyproject.toml
 requirements-dev.txt
 setup.cfg
+.github/CODE_OF_CONDUCT.md
 .github/workflows/ci.yml
 _extensions/interlinks/.gitignore
-_extensions/interlinks/README.md
 _extensions/interlinks/_extension.yml
-_extensions/interlinks/example.qmd
-_extensions/interlinks/interlinks.py
-_extensions/interlinks/objects_siuba.json
-_extensions/interlinks/objects_vetiver.inv
-_extensions/interlinks/objects_vetiver.json
+_extensions/interlinks/interlinks.lua
 case_studies/objects_sqla.inv
 case_studies/parsing.qmd
 case_studies/some_package.py
 case_studies/sphinx-inventory.md
 case_studies/sphinx-inventory.qmd
 docs/.gitignore
 docs/_quarto.yml
@@ -94,12 +91,18 @@
 quartodoc/tests/test_ast.py
 quartodoc/tests/test_basic.py
 quartodoc/tests/test_builder.py
 quartodoc/tests/test_builder_blueprint.py
 quartodoc/tests/test_interlinks.py
 quartodoc/tests/test_layout.py
 quartodoc/tests/test_renderers.py
+quartodoc/tests/example_interlinks/.gitignore
 quartodoc/tests/example_interlinks/README.md
 quartodoc/tests/example_interlinks/_quarto.yml
+quartodoc/tests/example_interlinks/interlinks.lua
 quartodoc/tests/example_interlinks/objects.json
 quartodoc/tests/example_interlinks/spec.yml
-quartodoc/tests/example_interlinks/_inv/other_objects.json
+quartodoc/tests/example_interlinks/test.md
+quartodoc/tests/example_interlinks/test.qmd
+quartodoc/tests/example_interlinks/_inv/other_objects.json
+scripts/filter-spec/generate_files.py
+scripts/filter-spec/generate_test_qmd.py
```

### Comparing `quartodoc-0.3.1/requirements-dev.txt` & `quartodoc-0.3.3/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `quartodoc-0.3.1/setup.cfg` & `quartodoc-0.3.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -2,38 +2,36 @@
 name = quartodoc
 version = dynamic
 description = Generate API documentation with quarto.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/machow/quartodoc
 author = Michael Chow
-author_email = mc_al_github@fastmail.com
+author_email = michael.chow@posit.co
 license = MIT
 keywords = documentation, quarto
 classifiers = 
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 
 [options]
 packages = find:
 include_package_data = True
 zipsafe = False
 python_requires = >=3.9
 install_requires = 
-	griffe==0.25
+	griffe
 	plum-dispatch<2.0.0;python_version<'3.10'
 	plum-dispatch;python_version>='3.10'
-	sphobjinv
-	tabulate
-	importlib-metadata
-	importlib-resources
-	panflute
-	pydantic
-	typing-extensions
+	sphobjinv>=2.3.1
+	tabulate>=0.9.0
+	importlib-metadata>=5.1.0
+	importlib-resources>=5.10.2
+	pydantic>=1.9.2
+	typing-extensions>=4.4.0
 
 [options.extras_require]
 dev = 
 	pytest
 	jupyterlab
 	jupytext
```

