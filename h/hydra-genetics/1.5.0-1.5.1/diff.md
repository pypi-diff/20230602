# Comparing `tmp/hydra-genetics-1.5.0.tar.gz` & `tmp/hydra-genetics-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydra-genetics-1.5.0.tar", last modified: Tue May 30 14:38:31 2023, max compression
+gzip compressed data, was "hydra-genetics-1.5.1.tar", last modified: Fri Jun  2 13:01:10 2023, max compression
```

## Comparing `hydra-genetics-1.5.0.tar` & `hydra-genetics-1.5.1.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.712339 hydra-genetics-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34961 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-30 14:38:31.712339 hydra-genetics-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.712339 hydra-genetics-1.5.0/hydra_genetics/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-30 14:38:31.712339 hydra-genetics-1.5.0/hydra_genetics/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.704339 hydra-genetics-1.5.0/hydra_genetics/commands/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33247 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/commands/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/commands/prep_pipeline_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/commands/references.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.704339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.704339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.704339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.704339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/linters/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/linters/.snakefmt.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.704339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/linters/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/linters/report/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.704339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/workflows/conventional-prs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/workflows/integration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/workflows/pycodestyle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/workflows/release-please.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/workflows/snakefmt.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/workflows/snakemake-dry-run.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.700339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.708339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.tests/integration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.708339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.tests/integration/config/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.tests/integration/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.tests/integration/config/resources.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.tests/integration/samples.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.tests/integration/units.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    34961 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.708339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/config/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/config/output_files.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/config/resources.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/config/samples.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/config/units.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.708339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/docs/extra.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.708339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/docs/includes/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/docs/includes/abbreviations.md
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/docs/intro.md
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/docs/softwares.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.708339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/images/
--rw-r--r--   0 runner    (1001) docker     (123)    61275 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/images/hydragenetics.png
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/mkdocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/requirements.test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.708339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/Snakefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.708339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/notebooks/describe_jupyter_notebook.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.708339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/rules/
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/rules/common.smk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.708339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/schemas/config.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/schemas/output_files.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/schemas/resources.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/schemas/rules.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/schemas/samples.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/schemas/units.schema.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.708339 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/scripts/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/scripts/test_dummy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.708339 hydra-genetics-1.5.0/hydra_genetics/rule-template/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/rule-template/config.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/rule-template/resources.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/rule-template/rules.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/rule-template/skeleton_rule.smk
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/rule-template/softwares.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.708339 hydra-genetics-1.5.0/hydra_genetics/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.712339 hydra-genetics-1.5.0/hydra_genetics/utils/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/utils/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/utils/io/chr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/utils/io/hotspot.py
--rw-r--r--   0 runner    (1001) docker     (123)    18291 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/utils/io/hotspot_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/utils/io/multibp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/utils/io/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/utils/io/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/utils/io/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.712339 hydra-genetics-1.5.0/hydra_genetics/utils/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/utils/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/utils/models/hotspot.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/utils/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/utils/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/hydra_genetics/utils/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.704339 hydra-genetics-1.5.0/hydra_genetics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-30 14:38:31.000000 hydra-genetics-1.5.0/hydra_genetics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-30 14:38:31.000000 hydra-genetics-1.5.0/hydra_genetics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:38:31.000000 hydra-genetics-1.5.0/hydra_genetics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-30 14:38:31.000000 hydra-genetics-1.5.0/hydra_genetics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:38:31.000000 hydra-genetics-1.5.0/hydra_genetics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-30 14:38:31.000000 hydra-genetics-1.5.0/hydra_genetics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-30 14:38:31.000000 hydra-genetics-1.5.0/hydra_genetics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-30 14:38:31.712339 hydra-genetics-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.712339 hydra-genetics-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.712339 hydra-genetics-1.5.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/tests/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.712339 hydra-genetics-1.5.0/tests/utils/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/tests/utils/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/tests/utils/io/test_hotspot.py
--rw-r--r--   0 runner    (1001) docker     (123)    67196 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/tests/utils/io/test_mutations_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:31.712339 hydra-genetics-1.5.0/tests/utils/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/tests/utils/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/tests/utils/models/test_hotspot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/tests/utils/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/tests/utils/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/tests/utils/test_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    28006 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/tests/utils/test_units.py
--rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-05-30 14:38:24.000000 hydra-genetics-1.5.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:10.645204 hydra-genetics-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34961 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-06-02 13:01:10.645204 hydra-genetics-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:10.645204 hydra-genetics-1.5.1/hydra_genetics/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-02 13:01:10.645204 hydra-genetics-1.5.1/hydra_genetics/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:10.637204 hydra-genetics-1.5.1/hydra_genetics/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33247 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/commands/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/commands/prep_pipeline_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/commands/references.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:10.637204 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:10.637204 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:10.637204 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:10.637204 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.github/linters/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.github/linters/.snakefmt.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:10.637204 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.github/linters/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.github/linters/report/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:10.641203 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.github/workflows/conventional-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.github/workflows/integration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.github/workflows/pycodestyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.github/workflows/release-please.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.github/workflows/snakefmt.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.github/workflows/snakemake-dry-run.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:10.633203 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:10.641203 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.tests/integration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:10.641203 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.tests/integration/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.tests/integration/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.tests/integration/config/resources.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.tests/integration/samples.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.tests/integration/units.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    34961 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:10.641203 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/config/output_files.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/config/resources.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/config/samples.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/config/units.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:10.641203 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/docs/extra.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:10.641203 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/docs/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/docs/includes/abbreviations.md
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/docs/intro.md
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/docs/softwares.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:10.641203 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    61275 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/images/hydragenetics.png
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/mkdocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/requirements.test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:10.641203 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/workflow/Snakefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:10.641203 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/workflow/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/workflow/notebooks/describe_jupyter_notebook.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:10.641203 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/workflow/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/workflow/rules/common.smk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:10.641203 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/workflow/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/workflow/schemas/config.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/workflow/schemas/output_files.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/workflow/schemas/resources.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/workflow/schemas/rules.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/workflow/schemas/samples.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/workflow/schemas/units.schema.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:10.641203 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/workflow/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/workflow/scripts/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/pipeline-template/workflow/scripts/test_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:10.641203 hydra-genetics-1.5.1/hydra_genetics/rule-template/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/rule-template/config.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/rule-template/resources.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/rule-template/rules.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/rule-template/skeleton_rule.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/rule-template/softwares.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:10.641203 hydra-genetics-1.5.1/hydra_genetics/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:10.645204 hydra-genetics-1.5.1/hydra_genetics/utils/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/utils/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/utils/io/chr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/utils/io/hotspot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18291 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/utils/io/hotspot_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/utils/io/multibp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/utils/io/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/utils/io/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/utils/io/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:10.645204 hydra-genetics-1.5.1/hydra_genetics/utils/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/utils/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/utils/models/hotspot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/utils/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/utils/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/hydra_genetics/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:10.637204 hydra-genetics-1.5.1/hydra_genetics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-06-02 13:01:10.000000 hydra-genetics-1.5.1/hydra_genetics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-06-02 13:01:10.000000 hydra-genetics-1.5.1/hydra_genetics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 13:01:10.000000 hydra-genetics-1.5.1/hydra_genetics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-02 13:01:10.000000 hydra-genetics-1.5.1/hydra_genetics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 13:01:10.000000 hydra-genetics-1.5.1/hydra_genetics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-02 13:01:10.000000 hydra-genetics-1.5.1/hydra_genetics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-02 13:01:10.000000 hydra-genetics-1.5.1/hydra_genetics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-02 13:01:10.645204 hydra-genetics-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:10.645204 hydra-genetics-1.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:10.645204 hydra-genetics-1.5.1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/tests/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:10.645204 hydra-genetics-1.5.1/tests/utils/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/tests/utils/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/tests/utils/io/test_hotspot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67196 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/tests/utils/io/test_mutations_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:10.645204 hydra-genetics-1.5.1/tests/utils/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/tests/utils/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/tests/utils/models/test_hotspot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/tests/utils/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/tests/utils/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/tests/utils/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28006 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/tests/utils/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-06-02 13:01:05.000000 hydra-genetics-1.5.1/versioneer.py
```

### Comparing `hydra-genetics-1.5.0/LICENSE.md` & `hydra-genetics-1.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/PKG-INFO` & `hydra-genetics-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydra-genetics
-Version: 1.5.0
+Version: 1.5.1
 Summary: Helper tools for use with hydra-genetics pipelines.
 Home-page: https://github.com/hydra-genetics/tools
 Author: Patrik Smeds
 Author-email: patrik.smeds@scilifelab.uu.se
 License: GPL-3
 Keywords: hydra-genetics,snakemake,bioinformatics,workflow,pipeline,clinical,biology,sequencing,NGS,next generation sequencing
 Description-Content-Type: text/markdown
```

### Comparing `hydra-genetics-1.5.0/README.md` & `hydra-genetics-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/__init__.py` & `hydra-genetics-1.5.1/hydra_genetics/__init__.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/__main__.py` & `hydra-genetics-1.5.1/hydra_genetics/__main__.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/commands/create.py` & `hydra-genetics-1.5.1/hydra_genetics/commands/create.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/commands/prep_pipeline_env.py` & `hydra-genetics-1.5.1/hydra_genetics/commands/prep_pipeline_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,44 +73,44 @@
     "--new-configfile",
     prompt="path",
     required=True,
     type=str,
     help="path to update config file",
 )
 @click.option(
-    "--reference-paths",
+    "--reference-path",
     multiple=True,
     prompt="path",
     required=True,
     type=str,
     help=(
         "format oldpath:newpath, will iterate over the provided config"
         " file and replace all occurrences of oldpath with new path"
     ),
 )
-def reference_path_update(configfile, new_configfile, reference_paths):
+def reference_path_update(configfile, new_configfile, reference_path):
     def process_yaml_data(yaml_data, reference_path):
         for key in yaml_data:
             if isinstance(yaml_data[key], dict):
                 yaml_data[key] = process_yaml_data(yaml_data[key], reference_path)
             else:
                 if isinstance(yaml_data[key], str):
                     for old_path, new_path in reference_path:
                         if old_path in yaml_data[key]:
                             yaml_data[key] = yaml_data[key].replace(old_path, new_path)
         return yaml_data
-    reference_paths = [r.split(":") for r in reference_paths]
+    reference_paths = [r.split(":") for r in reference_path]
     with open(configfile, "r") as stream:
         try:
             yaml_data = yaml.safe_load(stream)
         except yaml.YAMLError as exc:
             print(exc)
             exit(1)
 
-    yaml_data = process_yaml_data(yaml_data, reference_path)
+    yaml_data = process_yaml_data(yaml_data, reference_paths)
 
     with open(new_configfile, 'w') as file:
         for key, value in yaml_data.items():
             file.write(yaml.dump({key: value}))
             file.write("\n")
```

### Comparing `hydra-genetics-1.5.0/hydra_genetics/commands/references.py` & `hydra-genetics-1.5.1/hydra_genetics/commands/references.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,22 +70,23 @@
             return False
 
         if re.match("^[0-9.]+$", possible_file):
             return False
 
         extension = pathlib.Path(possible_file)
         # docker container aren't files
-        if ":" in possible_file:
+        if ":" in possible_file or possible_file.endswith(".sif"):
             return False
         # Skip files that are configured per analysis/site
         if possible_file.endswith("samples.tsv") \
            or possible_file.endswith("resources.yaml") \
            or possible_file.endswith("units.tsv") \
            or possible_file.endswith("output_list.yaml") \
-           or possible_file.endswith("output_list.json"):
+           or possible_file.endswith("output_list.json") \
+           or possible_file.endswith("snakemake-wrappers"):
             logging.debug(f"Ignore: {possible_file}")
             return False
         # If a extension can be found we consider it as a file
         if extension.suffix:
             # File
             return True
         else:
```

### Comparing `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/bug_report.md` & `hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/feature_request.md` & `hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md` & `hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/workflows/integration.yaml` & `hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.github/workflows/integration.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/workflows/lint.yaml` & `hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.github/workflows/lint.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/workflows/pycodestyle.yaml` & `hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.github/workflows/pycodestyle.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/workflows/pytest.yaml` & `hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/workflows/snakefmt.yaml` & `hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.github/workflows/snakefmt.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/.github/workflows/snakemake-dry-run.yaml` & `hydra-genetics-1.5.1/hydra_genetics/pipeline-template/.github/workflows/snakemake-dry-run.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/LICENSE.md` & `hydra-genetics-1.5.1/hydra_genetics/pipeline-template/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/README.md` & `hydra-genetics-1.5.1/hydra_genetics/pipeline-template/README.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/docs/extra.css` & `hydra-genetics-1.5.1/hydra_genetics/pipeline-template/docs/extra.css`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/docs/index.md` & `hydra-genetics-1.5.1/hydra_genetics/pipeline-template/docs/index.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/images/hydragenetics.png` & `hydra-genetics-1.5.1/hydra_genetics/pipeline-template/images/hydragenetics.png`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/mkdocs.yaml` & `hydra-genetics-1.5.1/hydra_genetics/pipeline-template/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/rules/common.smk` & `hydra-genetics-1.5.1/hydra_genetics/pipeline-template/workflow/rules/common.smk`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/schemas/config.schema.yaml` & `hydra-genetics-1.5.1/hydra_genetics/pipeline-template/workflow/schemas/config.schema.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/schemas/output_files.schema.yaml` & `hydra-genetics-1.5.1/hydra_genetics/pipeline-template/workflow/schemas/output_files.schema.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/schemas/resources.schema.yaml` & `hydra-genetics-1.5.1/hydra_genetics/pipeline-template/workflow/schemas/resources.schema.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/pipeline-template/workflow/schemas/units.schema.yaml` & `hydra-genetics-1.5.1/hydra_genetics/pipeline-template/workflow/schemas/units.schema.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/rule-template/config.schema.yaml` & `hydra-genetics-1.5.1/hydra_genetics/rule-template/config.schema.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/rule-template/resources.schema.yaml` & `hydra-genetics-1.5.1/hydra_genetics/rule-template/resources.schema.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/rule-template/rules.schema.yaml` & `hydra-genetics-1.5.1/hydra_genetics/rule-template/rules.schema.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/rule-template/skeleton_rule.smk` & `hydra-genetics-1.5.1/hydra_genetics/rule-template/skeleton_rule.smk`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/utils/io/chr.py` & `hydra-genetics-1.5.1/hydra_genetics/utils/io/chr.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/utils/io/hotspot.py` & `hydra-genetics-1.5.1/hydra_genetics/utils/io/hotspot.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/utils/io/hotspot_report.py` & `hydra-genetics-1.5.1/hydra_genetics/utils/io/hotspot_report.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/utils/io/multibp.py` & `hydra-genetics-1.5.1/hydra_genetics/utils/io/multibp.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/utils/io/reference.py` & `hydra-genetics-1.5.1/hydra_genetics/utils/io/reference.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
             if not os.path.exists(file_path):
                 counter_fail += 1
                 logging.error(f"Could not locate: {file_path}")
                 file_list, not_found_in_config, found = track_files(item['path'], file_list, not_found_in_config, found)
             else:
                 if 'checksum' not in item:
                     counter_pass += 1
-                    logging.debug(f"{item[path]} found, no checksum validation!")
+                    logging.debug(f"{item['path']} found, no checksum validation!")
                 else:
                     calculated_md5 = hashlib.md5(open(file_path, 'rb').read()).hexdigest()
                     if not calculated_md5 == item['checksum']:
                         counter_fail += 1
                         logging.error(f"Incorrect checksum for {file_path}, expected"
                                       f" {validation_data[k]['checksum']}, got {calculated_md5}")
                     else:
```

### Comparing `hydra-genetics-1.5.0/hydra_genetics/utils/io/utils.py` & `hydra-genetics-1.5.1/hydra_genetics/utils/io/utils.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/utils/misc.py` & `hydra-genetics-1.5.1/hydra_genetics/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/utils/models/hotspot.py` & `hydra-genetics-1.5.1/hydra_genetics/utils/models/hotspot.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/utils/samples.py` & `hydra-genetics-1.5.1/hydra_genetics/utils/samples.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics/utils/units.py` & `hydra-genetics-1.5.1/hydra_genetics/utils/units.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/hydra_genetics.egg-info/PKG-INFO` & `hydra-genetics-1.5.1/hydra_genetics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydra-genetics
-Version: 1.5.0
+Version: 1.5.1
 Summary: Helper tools for use with hydra-genetics pipelines.
 Home-page: https://github.com/hydra-genetics/tools
 Author: Patrik Smeds
 Author-email: patrik.smeds@scilifelab.uu.se
 License: GPL-3
 Keywords: hydra-genetics,snakemake,bioinformatics,workflow,pipeline,clinical,biology,sequencing,NGS,next generation sequencing
 Description-Content-Type: text/markdown
```

### Comparing `hydra-genetics-1.5.0/hydra_genetics.egg-info/SOURCES.txt` & `hydra-genetics-1.5.1/hydra_genetics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/setup.py` & `hydra-genetics-1.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/tests/utils/io/test_hotspot.py` & `hydra-genetics-1.5.1/tests/utils/io/test_hotspot.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/tests/utils/io/test_mutations_report.py` & `hydra-genetics-1.5.1/tests/utils/io/test_mutations_report.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/tests/utils/models/test_hotspot.py` & `hydra-genetics-1.5.1/tests/utils/models/test_hotspot.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/tests/utils/test_misc.py` & `hydra-genetics-1.5.1/tests/utils/test_misc.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/tests/utils/test_resources.py` & `hydra-genetics-1.5.1/tests/utils/test_resources.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/tests/utils/test_samples.py` & `hydra-genetics-1.5.1/tests/utils/test_samples.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/tests/utils/test_units.py` & `hydra-genetics-1.5.1/tests/utils/test_units.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.5.0/versioneer.py` & `hydra-genetics-1.5.1/versioneer.py`

 * *Files identical despite different names*

