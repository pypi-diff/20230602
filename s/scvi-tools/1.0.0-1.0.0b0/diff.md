# Comparing `tmp/scvi_tools-1.0.0.tar.gz` & `tmp/scvi_tools-1.0.0b0.tar.gz`

## Comparing `scvi_tools-1.0.0.tar` & `scvi_tools-1.0.0b0.tar`

### file list

```diff
@@ -1,351 +1,345 @@
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/.editorconfig
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/.gitattributes
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/.gitmodules
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/codecov.yml
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/readthedocs.yml
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/setup.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/.devcontainer/Dockerfile
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/Makefile
--rw-r--r--   0        0        0     8380 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/conf.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/index.md
--rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/installation.md
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/make.bat
--rw-r--r--   0        0        0    10246 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/references.bib
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/references.md
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/_static/code-24px.svg
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/_static/computer-24px.svg
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/_static/library_books-24px.svg
--rw-r--r--   0        0        0     7800 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/_static/logo.png
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/_static/logo.svg
--rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/_static/old_logo.png
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/_static/play_circle_outline-24px.svg
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/_static/scvi-tools-horizontal.svg
--rw-r--r--   0        0        0  1898761 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/_static/scvi_team.jpg
--rw-r--r--   0        0        0   745458 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/_static/tasks-01.png
--rw-r--r--   0        0        0   678820 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/_static/tasks.png
--rw-r--r--   0        0        0    39665 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/_static/tasks.svg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/_static/css/override.css
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/_static/tutorials/ldvae.svg
--rw-r--r--   0        0        0   111585 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/_static/tutorials/overview.svg
--rw-r--r--   0        0        0   304447 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/_static/tutorials/scanvi_alt.svg
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/_static/tutorials/totalvi_cell.svg
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/_templates/class_no_inherited.rst
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/_templates/layout.html
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/api/datasets.md
--rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/api/developer.md
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/api/index.md
--rw-r--r--   0        0        0     3471 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/api/user.md
--rw-r--r--   0        0        0     9899 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/contributing/index.md
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/extensions/edit_colab_url.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/extensions/typed_returns.py
--rw-r--r--   0        0        0    78222 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/release_notes/index.md
--rw-r--r--   0        0        0     8723 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/release_notes/figures/anndata_manager_schematic.svg
--rw-r--r--   0        0        0   366878 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/release_notes/figures/setup_anndata_before_after.svg
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/tutorials/index.md
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/tutorials/index_atac.md
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/tutorials/index_dev.md
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/tutorials/index_hub.md
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/tutorials/index_multimodal.md
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/tutorials/index_quick_start.md
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/tutorials/index_scrna.md
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/tutorials/index_spatial.md
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/tutorials/index_tuning.md
--rw-r--r--   0        0        0     6213 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/user_guide/index.md
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/user_guide/background/codebase_overview.md
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/user_guide/background/counterfactual_prediction.md
--rw-r--r--   0        0        0     8528 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/user_guide/background/differential_expression.md
--rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/user_guide/background/transfer_learning.md
--rw-r--r--   0        0        0     6093 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/user_guide/background/variational_inference.md
--rw-r--r--   0        0        0   998853 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/user_guide/background/figures/codebase_overview.svg
--rw-r--r--   0        0        0    53944 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/user_guide/background/figures/fdr_control.png
--rw-r--r--   0        0        0    26304 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/user_guide/background/figures/vi_projection.svg
--rw-r--r--   0        0        0     5710 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/user_guide/models/amortizedlda.md
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/user_guide/models/autozi.md
--rw-r--r--   0        0        0     7576 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/user_guide/models/cellassign.md
--rw-r--r--   0        0        0    12095 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/user_guide/models/destvi.md
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/user_guide/models/gimvi.md
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/user_guide/models/linearscvi.md
--rw-r--r--   0        0        0    10046 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/user_guide/models/multivi.md
--rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/user_guide/models/peakvi.md
--rw-r--r--   0        0        0    10196 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/user_guide/models/scanvi.md
--rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/user_guide/models/scar.md
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/user_guide/models/scbasset.md
--rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/user_guide/models/scvi.md
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/user_guide/models/solo.md
--rw-r--r--   0        0        0     7560 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/user_guide/models/stereoscope.md
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/user_guide/models/tangram.md
--rw-r--r--   0        0        0     9922 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/user_guide/models/totalvi.md
--rw-r--r--   0        0        0    53944 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/user_guide/models/figures/fdr_control.png
--rw-r--r--   0        0        0    19339 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/user_guide/models/figures/scLVM_graphical_model.svg
--rw-r--r--   0        0        0   707043 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/user_guide/models/figures/scanvi_pgm.png
--rw-r--r--   0        0        0   379727 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/user_guide/models/figures/scvi_annotated_graphical_model.png
--rw-r--r--   0        0        0    23137 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/user_guide/models/figures/stLVM_graphical_model.svg
--rw-r--r--   0        0        0    19723 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/user_guide/models/figures/stsc_scLVM_graphical_model.svg
--rw-r--r--   0        0        0    26350 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/user_guide/models/figures/stsc_stLVM_graphical_model.svg
--rw-r--r--   0        0        0    38410 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/docs/user_guide/models/figures/totalvi_graphical_model.svg
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/__init__.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/_compat.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/_constants.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/_decorators.py
--rw-r--r--   0        0        0     8413 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/_settings.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/_types.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/autotune/__init__.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/autotune/_callbacks.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/autotune/_defaults.py
--rw-r--r--   0        0        0    23291 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/autotune/_manager.py
--rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/autotune/_tuner.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/autotune/_types.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/autotune/_utils.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/criticism/__init__.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/criticism/_constants.py
--rw-r--r--   0        0        0    16915 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/criticism/_ppc.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/data/__init__.py
--rw-r--r--   0        0        0     6483 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/data/_anntorchdataset.py
--rw-r--r--   0        0        0     7912 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/data/_compat.py
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/data/_constants.py
--rw-r--r--   0        0        0    21277 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/data/_datasets.py
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/data/_download.py
--rw-r--r--   0        0        0    19381 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/data/_manager.py
--rw-r--r--   0        0        0    17277 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/data/_preprocessing.py
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/data/_read.py
--rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/data/_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/data/_built_in_data/__init__.py
--rw-r--r--   0        0        0     4314 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/data/_built_in_data/_brain_large.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/data/_built_in_data/_cellxgene.py
--rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/data/_built_in_data/_cite_seq.py
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/data/_built_in_data/_cortex.py
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/data/_built_in_data/_csv.py
--rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/data/_built_in_data/_dataset_10x.py
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/data/_built_in_data/_heartcellatlas.py
--rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/data/_built_in_data/_loom.py
--rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/data/_built_in_data/_pbmc.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/data/_built_in_data/_smfish.py
--rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/data/_built_in_data/_synthetic.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/data/fields/__init__.py
--rw-r--r--   0        0        0    18246 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/data/fields/_arraylike_field.py
--rw-r--r--   0        0        0     5546 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/data/fields/_base_field.py
--rw-r--r--   0        0        0     9702 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/data/fields/_dataframe_field.py
--rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/data/fields/_layer_field.py
--rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/data/fields/_mudata.py
--rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/data/fields/_protein.py
--rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/data/fields/_scanvi.py
--rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/data/fields/_uns_field.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/dataloaders/__init__.py
--rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/dataloaders/_ann_dataloader.py
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/dataloaders/_concat_dataloader.py
--rw-r--r--   0        0        0    17784 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/dataloaders/_data_splitting.py
--rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/dataloaders/_semi_dataloader.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/distributions/__init__.py
--rw-r--r--   0        0        0    19906 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/distributions/_negative_binomial.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/distributions/_utils.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/external/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/external/cellassign/__init__.py
--rw-r--r--   0        0        0    10477 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/external/cellassign/_model.py
--rw-r--r--   0        0        0     8944 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/external/cellassign/_module.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/external/gimvi/__init__.py
--rw-r--r--   0        0        0    24696 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/external/gimvi/_model.py
--rw-r--r--   0        0        0    17576 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/external/gimvi/_module.py
--rw-r--r--   0        0        0     5485 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/external/gimvi/_task.py
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/external/gimvi/_utils.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/external/scar/__init__.py
--rw-r--r--   0        0        0    12966 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/external/scar/_model.py
--rw-r--r--   0        0        0    12717 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/external/scar/_module.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/external/scbasset/__init__.py
--rw-r--r--   0        0        0    17242 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/external/scbasset/_model.py
--rw-r--r--   0        0        0    13981 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/external/scbasset/_module.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/external/solo/__init__.py
--rw-r--r--   0        0        0    17365 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/external/solo/_model.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/external/stereoscope/__init__.py
--rw-r--r--   0        0        0    12590 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/external/stereoscope/_model.py
--rw-r--r--   0        0        0     8943 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/external/stereoscope/_module.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/external/tangram/__init__.py
--rw-r--r--   0        0        0    12807 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/external/tangram/_model.py
--rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/external/tangram/_module.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/hub/__init__.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/hub/_constants.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/hub/_url.py
--rw-r--r--   0        0        0    11291 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/hub/hub_metadata.py
--rw-r--r--   0        0        0    13124 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/hub/hub_model.py
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/hub/model_card_template.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/model/__init__.py
--rw-r--r--   0        0        0     8875 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/model/_amortizedlda.py
--rw-r--r--   0        0        0    11198 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/model/_autozi.py
--rw-r--r--   0        0        0    10284 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/model/_condscvi.py
--rw-r--r--   0        0        0    14198 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/model/_destvi.py
--rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/model/_jaxscvi.py
--rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/model/_linear_scvi.py
--rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/model/_metrics.py
--rw-r--r--   0        0        0    44227 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/model/_multivi.py
--rw-r--r--   0        0        0    22243 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/model/_peakvi.py
--rw-r--r--   0        0        0    21595 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/model/_scanvi.py
--rw-r--r--   0        0        0    10886 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/model/_scvi.py
--rw-r--r--   0        0        0    54399 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/model/_totalvi.py
--rw-r--r--   0        0        0    15529 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/model/_utils.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/model/base/__init__.py
--rw-r--r--   0        0        0    12311 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/model/base/_archesmixin.py
--rw-r--r--   0        0        0    33943 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/model/base/_base_model.py
--rw-r--r--   0        0        0    27924 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/model/base/_differential.py
--rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/model/base/_jaxmixin.py
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/model/base/_log_likelihood.py
--rwxr-xr-x   0        0        0    20650 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/model/base/_pyromixin.py
--rw-r--r--   0        0        0    29147 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/model/base/_rnamixin.py
--rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/model/base/_training_mixin.py
--rw-r--r--   0        0        0     9931 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/model/base/_utils.py
--rw-r--r--   0        0        0     7955 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/model/base/_vaemixin.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/model/utils/__init__.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/model/utils/_mde.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/model/utils/_minification.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/module/__init__.py
--rw-r--r--   0        0        0    12511 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/module/_amortizedlda.py
--rw-r--r--   0        0        0    16720 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/module/_autozivae.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/module/_classifier.py
--rw-r--r--   0        0        0     7000 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/module/_jaxvae.py
--rw-r--r--   0        0        0    15351 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/module/_mrdeconv.py
--rw-r--r--   0        0        0    40070 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/module/_multivae.py
--rw-r--r--   0        0        0    12716 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/module/_peakvae.py
--rw-r--r--   0        0        0    13210 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/module/_scanvae.py
--rw-r--r--   0        0        0    29749 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/module/_totalvae.py
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/module/_utils.py
--rw-r--r--   0        0        0    27427 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/module/_vae.py
--rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/module/_vaec.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/module/base/__init__.py
--rw-r--r--   0        0        0    27109 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/module/base/_base_module.py
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/module/base/_decorators.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/module/base/_pyro.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/nn/__init__.py
--rw-r--r--   0        0        0    35112 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/nn/_base_components.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/nn/_utils.py
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/train/__init__.py
--rw-r--r--   0        0        0     5510 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/train/_callbacks.py
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/train/_logger.py
--rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/train/_metrics.py
--rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/train/_progress.py
--rw-r--r--   0        0        0     8170 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/train/_trainer.py
--rw-r--r--   0        0        0    51888 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/train/_trainingplans.py
--rw-r--r--   0        0        0     5650 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/train/_trainrunner.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/utils/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/utils/_attrdict.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/utils/_decorators.py
--rw-r--r--   0        0        0     8881 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/utils/_docstrings.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/utils/_exceptions.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/utils/_jax.py
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/scvi/utils/_track.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/conftest.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/autotune/test_defaults.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/autotune/test_manager.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/autotune/test_tuner.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/autotune/test_types.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/autotune/test_utils.py
--rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/core/test_differential.py
--rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/core/test_distributions.py
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/criticism/test_criticism.py
--rw-r--r--   0        0        0    15546 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/Cortex.loom
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/GSE100866_CBMC_8K_13AB_10X-RNA_umi.csv.gz
--rw-r--r--   0        0        0   332396 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/Layer2_BC_count_matrix-1.tsv
--rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/Rep11_MOB_count_matrix-1.tsv
--rw-r--r--   0        0        0    55647 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/SeqFISH.xlsx
--rw-r--r--   0        0        0    20360 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/TM_droplet_mat.h5ad
--rw-r--r--   0        0        0    40943 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/brain_large.h5
--rw-r--r--   0        0        0     6885 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/brain_small_metadata.pickle
--rw-r--r--   0        0        0   181632 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/brainlarge_dataset_test.h5ad
--rw-r--r--   0        0        0   167626 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/expression.bin
--rw-r--r--   0        0        0    31092 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/fc-dropseq.loom
--rw-r--r--   0        0        0    22197 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/immune_control_expression_matrix.txt
--rw-r--r--   0        0        0    22269 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/immune_stimulated_expression_matrix.txt
--rw-r--r--   0        0        0   529817 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/mpfc-starmap.loom
--rw-r--r--   0        0        0    21859 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/osmFISH_SScortex_mouse_all_cell.loom
--rw-r--r--   0        0        0  2064068 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/pbmc_10k_protein_v3.h5ad
--rw-r--r--   0        0        0  2302990 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/pbmc_5k_protein_v3.h5ad
--rw-r--r--   0        0        0    38216 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/random_metadata.pickle
--rw-r--r--   0        0        0    28396 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/retina.loom
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/seqfishplus.zip
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/10X/gene_info_pbmc.csv
--rw-r--r--   0        0        0    33580 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/10X/pbmc_metadata.pickle
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/10X/b_cells/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/10X/cd14_monocytes/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/10X/cd34/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/10X/cd4_t_helper/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/10X/cd56_nk/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/10X/cytotoxic_t/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/10X/memory_t/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/10X/naive_cytotoxic/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/10X/naive_t/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/10X/neuron_9k/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/10X/neuron_9k/filtered_gene_bc_matrices/mm10/barcodes.tsv
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/10X/neuron_9k/filtered_gene_bc_matrices/mm10/genes.tsv
--rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/10X/neuron_9k/filtered_gene_bc_matrices/mm10/matrix.mtx
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/10X/pbmc4k/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/10X/pbmc8k/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0    86914 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/10X/pbmc_10k_protein_v3/filtered_feature_bc_matrix.tar.gz
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/10X/regulatory_t/filtered_gene_bc_matrices.tar.gz
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/HEMATO/bBM.filtered_gene_list.paper.txt
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/HEMATO/bBM.raw_umifm_counts.csv.gz
--rw-r--r--   0        0        0     4860 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/HEMATO/bBM.spring_and_pba.csv
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/HEMATO/data.zip
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/citeSeq/cbmc/cbmc_adt.csv.gz
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/citeSeq/cbmc/cbmc_adt_centered.csv.gz
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/citeSeq/cbmc/cbmc_rna.csv.gz
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/citeSeq/pbmc/pbmc_adt.csv.gz
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/citeSeq/pbmc/pbmc_adt_centered.csv.gz
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/citeSeq/pbmc/pbmc_rna.csv.gz
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/filtered_gene_bc_matrices/hg19/barcodes.tsv
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/filtered_gene_bc_matrices/hg19/genes.tsv
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/filtered_gene_bc_matrices/hg19/matrix.mtx
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/seqfishplus/sourcedata/cortex_svz_cellcentroids.csv
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/seqfishplus/sourcedata/cortex_svz_counts.csv
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/seqfishplus/sourcedata/ob_cellcentroids.csv
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/seqfishplus/sourcedata/ob_counts.csv
--rw-r--r--   0        0        0    18358 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/simulation/simulation_1.loom
--rw-r--r--   0        0        0    17127 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/simulation/simulation_2.loom
--rw-r--r--   0        0        0    17046 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/simulation/simulation_3.loom
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/test_genome/test_genome.fa
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/test_genome/test_genome.fa.fai
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/test_genome/test_genome.fa.sizes
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/data/test_genome/test_genome.gaps.bed
--rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/dataloaders/test_dataloaders.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/dataloaders/test_datasplitter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/dataset/__init__.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/dataset/conftest.py
--rw-r--r--   0        0        0    20282 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/dataset/test_anndata.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/dataset/test_built_in_data.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/dataset/test_dataset10X.py
--rw-r--r--   0        0        0    14177 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/dataset/test_mudata.py
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/dataset/test_preprocessing.py
--rw-r--r--   0        0        0     5186 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/dataset/utils.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/external/test_cellassign.py
--rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/external/test_gimvi.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/external/test_scar.py
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/external/test_scbasset.py
--rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/external/test_solo.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/external/test_stereoscope.py
--rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/external/test_tangram.py
--rw-r--r--   0        0        0     6049 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/hub/test_hub_metadata.py
--rw-r--r--   0        0        0     7326 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/hub/test_hub_model.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/hub/test_url.py
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/model/base/test_base_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/models/__init__.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/models/test_lightning.py
--rw-r--r--   0        0        0    57068 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/models/test_models.py
--rw-r--r--   0        0        0    15511 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/models/test_models_with_minified_data.py
--rw-r--r--   0        0        0    10424 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/models/test_mudata_models.py
--rw-r--r--   0        0        0    22689 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/models/test_pyro.py
--rw-r--r--   0        0        0    18983 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/models/test_scarches.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/notebooks/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/train/__init__.py
--rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/tests/train/test_trainingplans.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/.gitignore
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/LICENSE
--rw-r--r--   0        0        0     4763 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/README.md
--rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    10263 2020-02-02 00:00:00.000000 scvi_tools-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/.editorconfig
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/.gitattributes
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/.gitmodules
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/codecov.yml
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/readthedocs.yml
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/setup.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/Makefile
+-rw-r--r--   0        0        0     8380 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/conf.py
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/index.md
+-rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/installation.md
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/make.bat
+-rw-r--r--   0        0        0    10246 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/references.bib
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/references.md
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_static/code-24px.svg
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_static/computer-24px.svg
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_static/library_books-24px.svg
+-rw-r--r--   0        0        0     7800 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_static/logo.png
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_static/logo.svg
+-rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_static/old_logo.png
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_static/play_circle_outline-24px.svg
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_static/scvi-tools-horizontal.svg
+-rw-r--r--   0        0        0  1898761 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_static/scvi_team.jpg
+-rw-r--r--   0        0        0   745458 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_static/tasks-01.png
+-rw-r--r--   0        0        0   678820 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_static/tasks.png
+-rw-r--r--   0        0        0    39665 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_static/tasks.svg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_static/css/override.css
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_static/tutorials/ldvae.svg
+-rw-r--r--   0        0        0   111585 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_static/tutorials/overview.svg
+-rw-r--r--   0        0        0   304447 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_static/tutorials/scanvi_alt.svg
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_static/tutorials/totalvi_cell.svg
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_templates/class_no_inherited.rst
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_templates/layout.html
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/api/datasets.md
+-rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/api/developer.md
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/api/index.md
+-rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/api/user.md
+-rw-r--r--   0        0        0     9899 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/contributing/index.md
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/extensions/edit_colab_url.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/extensions/typed_returns.py
+-rw-r--r--   0        0        0    76851 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/release_notes/index.md
+-rw-r--r--   0        0        0     8723 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/release_notes/figures/anndata_manager_schematic.svg
+-rw-r--r--   0        0        0   366878 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/release_notes/figures/setup_anndata_before_after.svg
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/tutorials/index.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/tutorials/index_atac.md
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/tutorials/index_dev.md
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/tutorials/index_hub.md
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/tutorials/index_multimodal.md
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/tutorials/index_quick_start.md
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/tutorials/index_scrna.md
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/tutorials/index_spatial.md
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/tutorials/index_tuning.md
+-rw-r--r--   0        0        0     6213 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/index.md
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/background/codebase_overview.md
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/background/counterfactual_prediction.md
+-rw-r--r--   0        0        0     8528 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/background/differential_expression.md
+-rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/background/transfer_learning.md
+-rw-r--r--   0        0        0     6093 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/background/variational_inference.md
+-rw-r--r--   0        0        0   998853 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/background/figures/codebase_overview.svg
+-rw-r--r--   0        0        0    53944 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/background/figures/fdr_control.png
+-rw-r--r--   0        0        0    26304 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/background/figures/vi_projection.svg
+-rw-r--r--   0        0        0     5710 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/amortizedlda.md
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/autozi.md
+-rw-r--r--   0        0        0     7576 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/cellassign.md
+-rw-r--r--   0        0        0    12095 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/destvi.md
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/gimvi.md
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/linearscvi.md
+-rw-r--r--   0        0        0    10046 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/multivi.md
+-rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/peakvi.md
+-rw-r--r--   0        0        0    10196 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/scanvi.md
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/scar.md
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/scbasset.md
+-rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/scvi.md
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/solo.md
+-rw-r--r--   0        0        0     7560 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/stereoscope.md
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/tangram.md
+-rw-r--r--   0        0        0     9922 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/totalvi.md
+-rw-r--r--   0        0        0    53944 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/figures/fdr_control.png
+-rw-r--r--   0        0        0    19339 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/figures/scLVM_graphical_model.svg
+-rw-r--r--   0        0        0   707043 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/figures/scanvi_pgm.png
+-rw-r--r--   0        0        0   379727 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/figures/scvi_annotated_graphical_model.png
+-rw-r--r--   0        0        0    23137 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/figures/stLVM_graphical_model.svg
+-rw-r--r--   0        0        0    19723 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/figures/stsc_scLVM_graphical_model.svg
+-rw-r--r--   0        0        0    26350 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/figures/stsc_stLVM_graphical_model.svg
+-rw-r--r--   0        0        0    38410 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/docs/user_guide/models/figures/totalvi_graphical_model.svg
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/__init__.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/_compat.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/_constants.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/_decorators.py
+-rw-r--r--   0        0        0     8413 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/_settings.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/_types.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/autotune/__init__.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/autotune/_callbacks.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/autotune/_defaults.py
+-rw-r--r--   0        0        0    23291 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/autotune/_manager.py
+-rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/autotune/_tuner.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/autotune/_types.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/autotune/_utils.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/__init__.py
+-rw-r--r--   0        0        0     6483 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_anntorchdataset.py
+-rw-r--r--   0        0        0     7912 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_compat.py
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_constants.py
+-rw-r--r--   0        0        0    21277 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_datasets.py
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_download.py
+-rw-r--r--   0        0        0    19381 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_manager.py
+-rw-r--r--   0        0        0    17277 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_preprocessing.py
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_read.py
+-rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_built_in_data/__init__.py
+-rw-r--r--   0        0        0     4314 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_built_in_data/_brain_large.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_built_in_data/_cellxgene.py
+-rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_built_in_data/_cite_seq.py
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_built_in_data/_cortex.py
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_built_in_data/_csv.py
+-rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_built_in_data/_dataset_10x.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_built_in_data/_heartcellatlas.py
+-rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_built_in_data/_loom.py
+-rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_built_in_data/_pbmc.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_built_in_data/_smfish.py
+-rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/_built_in_data/_synthetic.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/fields/__init__.py
+-rw-r--r--   0        0        0    18246 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/fields/_arraylike_field.py
+-rw-r--r--   0        0        0     5546 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/fields/_base_field.py
+-rw-r--r--   0        0        0     9702 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/fields/_dataframe_field.py
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/fields/_layer_field.py
+-rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/fields/_mudata.py
+-rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/fields/_protein.py
+-rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/fields/_scanvi.py
+-rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/data/fields/_uns_field.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/dataloaders/__init__.py
+-rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/dataloaders/_ann_dataloader.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/dataloaders/_concat_dataloader.py
+-rw-r--r--   0        0        0    17784 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/dataloaders/_data_splitting.py
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/dataloaders/_semi_dataloader.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/distributions/__init__.py
+-rw-r--r--   0        0        0    19906 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/distributions/_negative_binomial.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/distributions/_utils.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/cellassign/__init__.py
+-rw-r--r--   0        0        0    10469 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/cellassign/_model.py
+-rw-r--r--   0        0        0     8944 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/cellassign/_module.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/gimvi/__init__.py
+-rw-r--r--   0        0        0    24696 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/gimvi/_model.py
+-rw-r--r--   0        0        0    17576 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/gimvi/_module.py
+-rw-r--r--   0        0        0     5485 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/gimvi/_task.py
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/gimvi/_utils.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/scar/__init__.py
+-rw-r--r--   0        0        0    12966 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/scar/_model.py
+-rw-r--r--   0        0        0    12717 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/scar/_module.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/scbasset/__init__.py
+-rw-r--r--   0        0        0    17242 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/scbasset/_model.py
+-rw-r--r--   0        0        0    13981 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/scbasset/_module.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/solo/__init__.py
+-rw-r--r--   0        0        0    15785 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/solo/_model.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/stereoscope/__init__.py
+-rw-r--r--   0        0        0    12590 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/stereoscope/_model.py
+-rw-r--r--   0        0        0     8943 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/stereoscope/_module.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/tangram/__init__.py
+-rw-r--r--   0        0        0    12807 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/tangram/_model.py
+-rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/external/tangram/_module.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/hub/__init__.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/hub/_constants.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/hub/_url.py
+-rw-r--r--   0        0        0    11291 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/hub/hub_metadata.py
+-rw-r--r--   0        0        0    13124 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/hub/hub_model.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/hub/model_card_template.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/__init__.py
+-rw-r--r--   0        0        0     8875 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/_amortizedlda.py
+-rw-r--r--   0        0        0    11198 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/_autozi.py
+-rw-r--r--   0        0        0    10284 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/_condscvi.py
+-rw-r--r--   0        0        0    14198 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/_destvi.py
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/_jaxscvi.py
+-rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/_linear_scvi.py
+-rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/_metrics.py
+-rw-r--r--   0        0        0    44227 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/_multivi.py
+-rw-r--r--   0        0        0    22243 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/_peakvi.py
+-rw-r--r--   0        0        0    21345 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/_scanvi.py
+-rw-r--r--   0        0        0    10886 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/_scvi.py
+-rw-r--r--   0        0        0    54416 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/_totalvi.py
+-rw-r--r--   0        0        0    13899 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/_utils.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/base/__init__.py
+-rw-r--r--   0        0        0    12311 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/base/_archesmixin.py
+-rw-r--r--   0        0        0    32259 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/base/_base_model.py
+-rw-r--r--   0        0        0    27924 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/base/_differential.py
+-rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/base/_jaxmixin.py
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/base/_log_likelihood.py
+-rwxr-xr-x   0        0        0    20652 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/base/_pyromixin.py
+-rw-r--r--   0        0        0    28358 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/base/_rnamixin.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/base/_training_mixin.py
+-rw-r--r--   0        0        0     9931 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/base/_utils.py
+-rw-r--r--   0        0        0     7955 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/base/_vaemixin.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/utils/__init__.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/utils/_mde.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/model/utils/_minification.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/module/__init__.py
+-rw-r--r--   0        0        0    12511 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/module/_amortizedlda.py
+-rw-r--r--   0        0        0    16720 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/module/_autozivae.py
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/module/_classifier.py
+-rw-r--r--   0        0        0     7000 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/module/_jaxvae.py
+-rw-r--r--   0        0        0    15351 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/module/_mrdeconv.py
+-rw-r--r--   0        0        0    40070 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/module/_multivae.py
+-rw-r--r--   0        0        0    12716 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/module/_peakvae.py
+-rw-r--r--   0        0        0    12861 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/module/_scanvae.py
+-rw-r--r--   0        0        0    29749 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/module/_totalvae.py
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/module/_utils.py
+-rw-r--r--   0        0        0    27427 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/module/_vae.py
+-rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/module/_vaec.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/module/base/__init__.py
+-rw-r--r--   0        0        0    27109 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/module/base/_base_module.py
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/module/base/_decorators.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/module/base/_pyro.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/nn/__init__.py
+-rw-r--r--   0        0        0    35112 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/nn/_base_components.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/nn/_utils.py
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/train/__init__.py
+-rw-r--r--   0        0        0     5510 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/train/_callbacks.py
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/train/_logger.py
+-rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/train/_metrics.py
+-rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/train/_progress.py
+-rw-r--r--   0        0        0     8170 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/train/_trainer.py
+-rw-r--r--   0        0        0    51487 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/train/_trainingplans.py
+-rw-r--r--   0        0        0     5650 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/train/_trainrunner.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/utils/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/utils/_attrdict.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/utils/_decorators.py
+-rw-r--r--   0        0        0     8881 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/utils/_docstrings.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/utils/_exceptions.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/utils/_jax.py
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/scvi/utils/_track.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/__init__.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/conftest.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/autotune/test_defaults.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/autotune/test_manager.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/autotune/test_tuner.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/autotune/test_types.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/autotune/test_utils.py
+-rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/core/test_differential.py
+-rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/core/test_distributions.py
+-rw-r--r--   0        0        0    15546 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/Cortex.loom
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/GSE100866_CBMC_8K_13AB_10X-RNA_umi.csv.gz
+-rw-r--r--   0        0        0   332396 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/Layer2_BC_count_matrix-1.tsv
+-rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/Rep11_MOB_count_matrix-1.tsv
+-rw-r--r--   0        0        0    55647 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/SeqFISH.xlsx
+-rw-r--r--   0        0        0    20360 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/TM_droplet_mat.h5ad
+-rw-r--r--   0        0        0    40943 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/brain_large.h5
+-rw-r--r--   0        0        0     6885 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/brain_small_metadata.pickle
+-rw-r--r--   0        0        0   181632 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/brainlarge_dataset_test.h5ad
+-rw-r--r--   0        0        0   167626 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/expression.bin
+-rw-r--r--   0        0        0    31092 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/fc-dropseq.loom
+-rw-r--r--   0        0        0    22197 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/immune_control_expression_matrix.txt
+-rw-r--r--   0        0        0    22269 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/immune_stimulated_expression_matrix.txt
+-rw-r--r--   0        0        0   529817 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/mpfc-starmap.loom
+-rw-r--r--   0        0        0    21859 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/osmFISH_SScortex_mouse_all_cell.loom
+-rw-r--r--   0        0        0  2064068 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/pbmc_10k_protein_v3.h5ad
+-rw-r--r--   0        0        0  2302990 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/pbmc_5k_protein_v3.h5ad
+-rw-r--r--   0        0        0    38216 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/random_metadata.pickle
+-rw-r--r--   0        0        0    28396 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/retina.loom
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/seqfishplus.zip
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/gene_info_pbmc.csv
+-rw-r--r--   0        0        0    33580 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/pbmc_metadata.pickle
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/b_cells/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/cd14_monocytes/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/cd34/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/cd4_t_helper/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/cd56_nk/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/cytotoxic_t/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/memory_t/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/naive_cytotoxic/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/naive_t/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/neuron_9k/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/neuron_9k/filtered_gene_bc_matrices/mm10/barcodes.tsv
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/neuron_9k/filtered_gene_bc_matrices/mm10/genes.tsv
+-rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/neuron_9k/filtered_gene_bc_matrices/mm10/matrix.mtx
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/pbmc4k/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/pbmc8k/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0    86914 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/pbmc_10k_protein_v3/filtered_feature_bc_matrix.tar.gz
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/10X/regulatory_t/filtered_gene_bc_matrices.tar.gz
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/HEMATO/bBM.filtered_gene_list.paper.txt
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/HEMATO/bBM.raw_umifm_counts.csv.gz
+-rw-r--r--   0        0        0     4860 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/HEMATO/bBM.spring_and_pba.csv
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/HEMATO/data.zip
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/citeSeq/cbmc/cbmc_adt.csv.gz
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/citeSeq/cbmc/cbmc_adt_centered.csv.gz
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/citeSeq/cbmc/cbmc_rna.csv.gz
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/citeSeq/pbmc/pbmc_adt.csv.gz
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/citeSeq/pbmc/pbmc_adt_centered.csv.gz
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/citeSeq/pbmc/pbmc_rna.csv.gz
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/filtered_gene_bc_matrices/hg19/barcodes.tsv
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/filtered_gene_bc_matrices/hg19/genes.tsv
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/filtered_gene_bc_matrices/hg19/matrix.mtx
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/seqfishplus/sourcedata/cortex_svz_cellcentroids.csv
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/seqfishplus/sourcedata/cortex_svz_counts.csv
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/seqfishplus/sourcedata/ob_cellcentroids.csv
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/seqfishplus/sourcedata/ob_counts.csv
+-rw-r--r--   0        0        0    18358 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/simulation/simulation_1.loom
+-rw-r--r--   0        0        0    17127 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/simulation/simulation_2.loom
+-rw-r--r--   0        0        0    17046 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/simulation/simulation_3.loom
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/test_genome/test_genome.fa
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/test_genome/test_genome.fa.fai
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/test_genome/test_genome.fa.sizes
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/data/test_genome/test_genome.gaps.bed
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/dataloaders/test_datasplitter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/dataset/__init__.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/dataset/conftest.py
+-rw-r--r--   0        0        0    20282 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/dataset/test_anndata.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/dataset/test_built_in_data.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/dataset/test_dataset10X.py
+-rw-r--r--   0        0        0    14177 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/dataset/test_mudata.py
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/dataset/test_preprocessing.py
+-rw-r--r--   0        0        0     5186 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/dataset/utils.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/external/test_cellassign.py
+-rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/external/test_gimvi.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/external/test_scar.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/external/test_scbasset.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/external/test_solo.py
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/external/test_stereoscope.py
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/external/test_tangram.py
+-rw-r--r--   0        0        0     6049 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/hub/test_hub_metadata.py
+-rw-r--r--   0        0        0     7326 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/hub/test_hub_model.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/hub/test_url.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/models/__init__.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/models/test_lightning.py
+-rw-r--r--   0        0        0    56424 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/models/test_models.py
+-rw-r--r--   0        0        0    15511 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/models/test_models_with_minified_data.py
+-rw-r--r--   0        0        0    10424 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/models/test_mudata_models.py
+-rw-r--r--   0        0        0    22689 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/models/test_pyro.py
+-rw-r--r--   0        0        0    18983 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/models/test_scarches.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/notebooks/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/train/__init__.py
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/tests/train/test_trainingplans.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/.gitignore
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/LICENSE
+-rw-r--r--   0        0        0     4763 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/README.md
+-rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/pyproject.toml
+-rw-r--r--   0        0        0    10225 2020-02-02 00:00:00.000000 scvi_tools-1.0.0b0/PKG-INFO
```

### Comparing `scvi_tools-1.0.0/.pre-commit-config.yaml` & `scvi_tools-1.0.0b0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/CODE_OF_CONDUCT.md` & `scvi_tools-1.0.0b0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/.devcontainer/devcontainer.json` & `scvi_tools-1.0.0b0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/.github/workflows/build.yml` & `scvi_tools-1.0.0b0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/.github/workflows/release.yml` & `scvi_tools-1.0.0b0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/.github/workflows/test.yml` & `scvi_tools-1.0.0b0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/Makefile` & `scvi_tools-1.0.0b0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/conf.py` & `scvi_tools-1.0.0b0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/index.md` & `scvi_tools-1.0.0b0/docs/index.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/installation.md` & `scvi_tools-1.0.0b0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/make.bat` & `scvi_tools-1.0.0b0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/references.bib` & `scvi_tools-1.0.0b0/docs/references.bib`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/_static/logo.png` & `scvi_tools-1.0.0b0/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/_static/logo.svg` & `scvi_tools-1.0.0b0/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/_static/old_logo.png` & `scvi_tools-1.0.0b0/docs/_static/old_logo.png`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/_static/scvi-tools-horizontal.svg` & `scvi_tools-1.0.0b0/docs/_static/scvi-tools-horizontal.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/_static/scvi_team.jpg` & `scvi_tools-1.0.0b0/docs/_static/scvi_team.jpg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/_static/tasks-01.png` & `scvi_tools-1.0.0b0/docs/_static/tasks-01.png`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/_static/tasks.png` & `scvi_tools-1.0.0b0/docs/_static/tasks.png`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/_static/tasks.svg` & `scvi_tools-1.0.0b0/docs/_static/tasks.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/_static/tutorials/ldvae.svg` & `scvi_tools-1.0.0b0/docs/_static/tutorials/ldvae.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/_static/tutorials/overview.svg` & `scvi_tools-1.0.0b0/docs/_static/tutorials/overview.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/_static/tutorials/scanvi_alt.svg` & `scvi_tools-1.0.0b0/docs/_static/tutorials/scanvi_alt.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/_static/tutorials/totalvi_cell.svg` & `scvi_tools-1.0.0b0/docs/_static/tutorials/totalvi_cell.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/_templates/class_no_inherited.rst` & `scvi_tools-1.0.0b0/docs/_templates/class_no_inherited.rst`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/_templates/layout.html` & `scvi_tools-1.0.0b0/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/_templates/autosummary/class.rst` & `scvi_tools-1.0.0b0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/api/datasets.md` & `scvi_tools-1.0.0b0/docs/api/datasets.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/api/developer.md` & `scvi_tools-1.0.0b0/docs/api/developer.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/api/user.md` & `scvi_tools-1.0.0b0/docs/api/user.md`

 * *Files 7% similar despite different names*

```diff
@@ -122,31 +122,25 @@
 ## Model hub
 
 We have a hub for pre-trained `scvi-tools` models that is hosted on [huggingface](https://huggingface.co/models).
 Using the functionality that `scvi-tools` provides, users can download pre-trained `scvi-tools` models (and datasets)
 from this platform, and model generators can upload their own pre-trained `scvi-tools` models to this platform.
 
 ```{eval-rst}
-.. autosummary::
-   :toctree: reference/
-   :nosignatures:
-
-   hub.HubMetadata
-   hub.HubModelCardHelper
-   hub.HubModel
+.. currentmodule:: scvi
 ```
 
-## Model criticism
-
 ```{eval-rst}
 .. autosummary::
    :toctree: reference/
    :nosignatures:
 
-   criticism.PosteriorPredictiveCheck
+   scvi.hub.HubMetadata
+   scvi.hub.HubModelCardHelper
+   scvi.hub.HubModel
 ```
 
 ## Utilities
 
 Here we maintain miscellaneous general methods.
 
 ```{eval-rst}
```

### Comparing `scvi_tools-1.0.0/docs/contributing/index.md` & `scvi_tools-1.0.0b0/docs/contributing/index.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/extensions/edit_colab_url.py` & `scvi_tools-1.0.0b0/docs/extensions/edit_colab_url.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/extensions/typed_returns.py` & `scvi_tools-1.0.0b0/docs/extensions/typed_returns.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/release_notes/index.md` & `scvi_tools-1.0.0b0/docs/release_notes/index.md`

 * *Files 0% similar despite different names*

```diff
@@ -13,43 +13,31 @@
 
 #### Removed
 
 -   Remove deprecated `use_gpu` in favor of PyTorch Lightning arguments `accelerator` and `devices` {pr}`xxxx`.
 
 ## Version 1.0
 
-### 1.0.0 (2023-06-02)
+### 1.0.0 (2023-MM-DD)
 
 #### Added
 
--   Add {class}`scvi.criticism.PosteriorPredictiveCheck` for model evaluation {pr}`2058`.
 -   Add {func}`scvi.data.reads_to_fragments` for scATAC data {pr}`1946`
 -   Add default `stacklevel` for `warnings` in `scvi.settings` {pr}`1971`.
 -   Add scBasset motif injection procedure {pr}`2010`.
 -   Add importance sampling based differential expression procedure {pr}`1872`.
--   Raise clearer error when initializing {class}`scvi.external.SOLO` from {class}`scvi.model.SCVI` with extra categorical or continuous covariates {pr}`2027`.
 -   Add option to generate {class}`mudata.MuData` in {meth}`scvi.data.synthetic_iid` {pr}`2028`.
 -   Add option for disabling shuffling prior to splitting data in {class}`scvi.dataloaders.DataSplitter` {pr}`2037`.
 -   Add {meth}`scvi.data.AnnDataManager.create_torch_dataset` and expose custom sampler ability {pr}`2036`.
--   Log training loss through Lightning's progress bar {pr}`2043`.
--   Filter Jax undetected GPU warnings {pr}`2044`.
--   Raise warning if MPS backend is selected for PyTorch, see https://github.com/pytorch/pytorch/issues/77764 {pr}`2045`.
--   Add `deregister_manager` function to {class}`scvi.model.base.BaseModelClass`, allowing to clear
-    {class}`scvi.data.AnnDataManager` instances from memory {pr}`2060`.
--   Add option to use a linear classifier in {class}`scvi.model.SCANVI` {pr}`2063`.
--   Add lower bound 0.12.1 for Numpyro dependency {pr}`2078`.
--   Add new section in scBasset tutorial for motif scoring {pr}`2079`.
 
 #### Fixed
 
 -   Fix creation of minified adata by copying original uns dict {pr}`2000`. This issue arises with anndata>=0.9.0.
 -   Fix {class}`scvi.model.TOTALVI` {class}`scvi.model.MULTIVI` handling of missing protein values {pr}`2009`.
 -   Fix bug in {meth}`scvi.distributions.NegativeBinomialMixture.sample` where `theta` and `mu` arguments were switched around {pr}`2024`.
--   Fix bug in {meth}`scvi.dataloaders.SemiSupervisedDataLoader.resample_labels` where the labeled dataloader was not being reinitialized on subsample {pr}`2032`.
--   Fix typo in {class}`scvi.model.JaxSCVI` example snippet {pr}`2075`.
 
 #### Changed
 
 -   Use sphinx book theme for documentation {pr}`1673`.
 -   {meth}`scvi.model.base.RNASeqMixin.posterior_predictive_sample` now outputs 3-d {class}`sparse.GCXS` matrices {pr}`1902`.
 -   Add an option to specify `dropout_ratio` in {meth}`scvi.data.synthetic_iid` {pr}`1920`.
 -   Update to lightning 2.0 {pr}`1961`
@@ -62,16 +50,14 @@
 -   Validate training data and code URLs for {class}`scvi.hub.HubMetadata` and {class}`scvi.hub.HubModelCardHelper` {pr}`1985`.
 -   Keyword arguments for encoders and decoders can now be passed in from the model level {pr}`1986`.
 -   Expose `local_dir` as a public property in {class}`scvi.hub.HubModel` {pr}`1994`.
 -   Use {func}`anndata.concat` internally inside {meth}`scvi.external.SOLO.from_scvi_model` {pr}`2013`.
 -   {class}`scvi.train.SemiSupervisedTrainingPlan` and {class}`scvi.train.ClassifierTrainingPlan` now log accuracy,
     F1 score, and AUROC metrics {pr}`2023`.
 -   Switch to cellxgene census for backend for cellxgene data function {pr}`2030`.
--   Change default `max_cells` and `truncation` in {meth}`scvi.model.base.RNASeqMixin._get_importance_weights` {pr}`2064`.
--   Refactor heuristic for default `max_epochs` as a separate function {meth}`scvi.model._utils.get_max_epochs_heuristic` {pr}`2083`.
 
 #### Removed
 
 -   Remove ability to set up ST data in {class}`~scvi.external.SpatialStereoscope.from_rna_model`, which was deprecated. ST data should be set up using {class}`~scvi.external.SpatialStereoscope.setup_anndata` {pr}`1949`.
 -   Remove custom reusable doc decorator which was used for de docs {pr}`1970`.
 -   Remove `drop_last` as an integer from {class}`~scvi.dataloaders.AnnDataLoader`, add typing and code cleanup {pr}`1975`.
 -   Remove seqfish and seqfish plus datasets {pr}`2017`.
```

### Comparing `scvi_tools-1.0.0/docs/release_notes/figures/anndata_manager_schematic.svg` & `scvi_tools-1.0.0b0/docs/release_notes/figures/anndata_manager_schematic.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/release_notes/figures/setup_anndata_before_after.svg` & `scvi_tools-1.0.0b0/docs/release_notes/figures/setup_anndata_before_after.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/tutorials/index.md` & `scvi_tools-1.0.0b0/docs/tutorials/index.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/tutorials/index_dev.md` & `scvi_tools-1.0.0b0/docs/tutorials/index_dev.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/user_guide/index.md` & `scvi_tools-1.0.0b0/docs/user_guide/index.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/user_guide/background/differential_expression.md` & `scvi_tools-1.0.0b0/docs/user_guide/background/differential_expression.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/user_guide/background/transfer_learning.md` & `scvi_tools-1.0.0b0/docs/user_guide/background/transfer_learning.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/user_guide/background/variational_inference.md` & `scvi_tools-1.0.0b0/docs/user_guide/background/variational_inference.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/user_guide/background/figures/codebase_overview.svg` & `scvi_tools-1.0.0b0/docs/user_guide/background/figures/codebase_overview.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/user_guide/background/figures/fdr_control.png` & `scvi_tools-1.0.0b0/docs/user_guide/background/figures/fdr_control.png`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/user_guide/background/figures/vi_projection.svg` & `scvi_tools-1.0.0b0/docs/user_guide/background/figures/vi_projection.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/user_guide/models/amortizedlda.md` & `scvi_tools-1.0.0b0/docs/user_guide/models/amortizedlda.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/user_guide/models/autozi.md` & `scvi_tools-1.0.0b0/docs/user_guide/models/autozi.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/user_guide/models/cellassign.md` & `scvi_tools-1.0.0b0/docs/user_guide/models/cellassign.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/user_guide/models/destvi.md` & `scvi_tools-1.0.0b0/docs/user_guide/models/destvi.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/user_guide/models/linearscvi.md` & `scvi_tools-1.0.0b0/docs/user_guide/models/linearscvi.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/user_guide/models/multivi.md` & `scvi_tools-1.0.0b0/docs/user_guide/models/multivi.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/user_guide/models/peakvi.md` & `scvi_tools-1.0.0b0/docs/user_guide/models/peakvi.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/user_guide/models/scanvi.md` & `scvi_tools-1.0.0b0/docs/user_guide/models/scanvi.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/user_guide/models/scar.md` & `scvi_tools-1.0.0b0/docs/user_guide/models/scar.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/user_guide/models/scbasset.md` & `scvi_tools-1.0.0b0/docs/user_guide/models/scbasset.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/user_guide/models/scvi.md` & `scvi_tools-1.0.0b0/docs/user_guide/models/scvi.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/user_guide/models/solo.md` & `scvi_tools-1.0.0b0/docs/user_guide/models/solo.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/user_guide/models/stereoscope.md` & `scvi_tools-1.0.0b0/docs/user_guide/models/stereoscope.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/user_guide/models/tangram.md` & `scvi_tools-1.0.0b0/docs/user_guide/models/tangram.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/user_guide/models/totalvi.md` & `scvi_tools-1.0.0b0/docs/user_guide/models/totalvi.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/user_guide/models/figures/fdr_control.png` & `scvi_tools-1.0.0b0/docs/user_guide/models/figures/fdr_control.png`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/user_guide/models/figures/scLVM_graphical_model.svg` & `scvi_tools-1.0.0b0/docs/user_guide/models/figures/scLVM_graphical_model.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/user_guide/models/figures/scanvi_pgm.png` & `scvi_tools-1.0.0b0/docs/user_guide/models/figures/scanvi_pgm.png`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/user_guide/models/figures/scvi_annotated_graphical_model.png` & `scvi_tools-1.0.0b0/docs/user_guide/models/figures/scvi_annotated_graphical_model.png`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/user_guide/models/figures/stLVM_graphical_model.svg` & `scvi_tools-1.0.0b0/docs/user_guide/models/figures/stLVM_graphical_model.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/user_guide/models/figures/stsc_scLVM_graphical_model.svg` & `scvi_tools-1.0.0b0/docs/user_guide/models/figures/stsc_scLVM_graphical_model.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/user_guide/models/figures/stsc_stLVM_graphical_model.svg` & `scvi_tools-1.0.0b0/docs/user_guide/models/figures/stsc_stLVM_graphical_model.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/docs/user_guide/models/figures/totalvi_graphical_model.svg` & `scvi_tools-1.0.0b0/docs/user_guide/models/figures/totalvi_graphical_model.svg`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/__init__.py` & `scvi_tools-1.0.0b0/scvi/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,33 @@
 """scvi-tools."""
 
 # Set default logging handler to avoid logging with logging.lastResort logger.
 import logging
-import warnings
 
 from ._constants import METRIC_KEYS, REGISTRY_KEYS
 from ._settings import settings
 
 # this import needs to come after prior imports to prevent circular import
-from . import autotune, data, model, external, utils, criticism
+from . import autotune, data, model, external, utils
 
 from importlib.metadata import version
 
 package_name = "scvi-tools"
 __version__ = version(package_name)
 
 settings.verbosity = logging.INFO
 test_var = "test"
 
 # Jax sets the root logger, this prevents double output.
 scvi_logger = logging.getLogger("scvi")
 scvi_logger.propagate = False
 
-# ignore Jax GPU warnings
-warnings.filterwarnings("ignore", message="No GPU/TPU found, falling back to CPU.")
-
 __all__ = [
     "settings",
     "REGISTRY_KEYS",
     "METRIC_KEYS",
     "autotune",
     "data",
     "model",
     "external",
     "utils",
-    "criticism",
 ]
```

### Comparing `scvi_tools-1.0.0/scvi/_constants.py` & `scvi_tools-1.0.0b0/scvi/_constants.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/_decorators.py` & `scvi_tools-1.0.0b0/scvi/_decorators.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/_settings.py` & `scvi_tools-1.0.0b0/scvi/_settings.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/autotune/_callbacks.py` & `scvi_tools-1.0.0b0/scvi/autotune/_callbacks.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/autotune/_defaults.py` & `scvi_tools-1.0.0b0/scvi/autotune/_defaults.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/autotune/_manager.py` & `scvi_tools-1.0.0b0/scvi/autotune/_manager.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/autotune/_tuner.py` & `scvi_tools-1.0.0b0/scvi/autotune/_tuner.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/autotune/_types.py` & `scvi_tools-1.0.0b0/scvi/autotune/_types.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/autotune/_utils.py` & `scvi_tools-1.0.0b0/scvi/autotune/_utils.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/criticism/_ppc.py` & `scvi_tools-1.0.0b0/scvi/external/solo/_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,435 +1,443 @@
-import json
+import io
+import logging
 import warnings
-from typing import Dict, List, Literal, Optional
+from contextlib import redirect_stdout
+from typing import List, Optional, Sequence, Union
 
+import anndata
 import numpy as np
 import pandas as pd
+import torch
 from anndata import AnnData
-from scipy.sparse import issparse
-from scipy.stats import pearsonr, spearmanr
-from sklearn.metrics import (
-    average_precision_score,
-    precision_recall_fscore_support,
-    roc_auc_score,
-)
-from sparse import GCXS, SparseArray
-from xarray import DataArray, Dataset
 
-from scvi._decorators import dependencies
+from scvi import REGISTRY_KEYS, settings
+from scvi.data import AnnDataManager
+from scvi.data.fields import CategoricalObsField, LayerField
+from scvi.dataloaders import DataSplitter
+from scvi.model import SCVI
 from scvi.model.base import BaseModelClass
+from scvi.module import Classifier
+from scvi.module.base import auto_move_data
+from scvi.train import ClassifierTrainingPlan, LoudEarlyStopping, TrainRunner
+from scvi.utils import setup_anndata_dsp
+from scvi.utils._docstrings import devices_dsp
 
-from ._constants import (
-    DATA_VAR_RAW,
-    DEFAULT_DE_N_TOP_GENES_OVERLAP,
-    DEFAULT_DE_P_VAL_THRESHOLD,
-    METRIC_CALIBRATION,
-    METRIC_CV_CELL,
-    METRIC_CV_GENE,
-    METRIC_DIFF_EXP,
-    METRIC_ZERO_FRACTION,
-    UNS_NAME_RGG_PPC,
-    UNS_NAME_RGG_RAW,
-)
-
-Dims = Literal["cells", "features"]
-
-
-def _make_dataset_dense(dataset: Dataset) -> Dataset:
-    """Make a dataset dense, converting sparse arrays to dense arrays."""
-    dataset = dataset.map(
-        lambda x: x.data.todense() if isinstance(x.data, SparseArray) else x
-    )
-    return dataset
-
-
-def _get_precision_recall_f1(ground_truth: np.ndarray, pred: np.ndarray):
-    precision, recall, f1, _ = precision_recall_fscore_support(
-        ground_truth, pred, average="binary"
-    )
-    return precision, recall, f1
+logger = logging.getLogger(__name__)
 
+LABELS_KEY = "_solo_doub_sim"
 
-class PosteriorPredictiveCheck:
-    """
-    EXPERIMENTAL Posterior predictive checks for comparing scRNA-seq generative models.
+
+class SOLO(BaseModelClass):
+    """Doublet detection in scRNA-seq :cite:p:`Bernstein20`.
+
+    Most users will initialize the model using the class method
+    :meth:`~scvi.external.SOLO.from_scvi_model`, which takes as
+    input a pre-trained :class:`~scvi.model.SCVI` object.
 
     Parameters
     ----------
     adata
-        AnnData object with raw counts.
-    models_dict
-        Dictionary of models to compare.
-    count_layer_key
-        Key in adata.layers to use as raw counts, if None, use adata.X.
-    n_samples
-        Number of posterior predictive samples to generate
+        AnnData object that has been registered via :meth:`~scvi.model.SCVI.setup_anndata`.
+        Object should contain latent representation of real cells and doublets as `adata.X`.
+        Object should also be registered, using `.X` and `labels_key="_solo_doub_sim"`.
+    **classifier_kwargs
+        Keyword args for :class:`~scvi.module.Classifier`
+
+    Examples
+    --------
+    In the case of scVI trained with multiple batches:
+
+    >>> adata = anndata.read_h5ad(path_to_anndata)
+    >>> scvi.model.SCVI.setup_anndata(adata, batch_key="batch")
+    >>> vae = scvi.model.SCVI(adata)
+    >>> vae.train()
+    >>> solo_batch_1 = scvi.external.SOLO.from_scvi_model(vae, restrict_to_batch="batch 1")
+    >>> solo_batch_1.train()
+    >>> solo_batch_1.predict()
+
+    Otherwise:
+
+    >>> adata = anndata.read_h5ad(path_to_anndata)
+    >>> scvi.model.SCVI.setup_anndata(adata)
+    >>> vae = scvi.model.SCVI(adata)
+    >>> vae.train()
+    >>> solo = scvi.external.SOLO.from_scvi_model(vae)
+    >>> solo.train()
+    >>> solo.predict()
+
+    Notes
+    -----
+    Solo should be trained on one lane of data at a time. An
+    :class:`~scvi.model.SCVI` instance that was trained with multiple
+    batches can be used as input, but Solo should be created and run
+    multiple times, each with a new `restrict_to_batch` in
+    :meth:`~scvi.external.SOLO.from_scvi_model`.
     """
 
     def __init__(
         self,
         adata: AnnData,
-        models_dict: Dict[str, BaseModelClass],
-        count_layer_key: Optional[str] = None,
-        n_samples: int = 10,
+        **classifier_kwargs,
     ):
-        self.adata = adata
-        self.count_layer_key = count_layer_key
-        raw_counts = (
-            adata.layers[count_layer_key] if count_layer_key is not None else adata.X
-        )
-        # Compressed axis is rows, like csr
-        if isinstance(raw_counts, np.ndarray):
-            self.raw_counts = GCXS.from_numpy(raw_counts, compressed_axes=(0,))
-        elif issparse(raw_counts):
-            self.raw_counts = GCXS.from_scipy_sparse(raw_counts).change_compressed_axes(
-                (0,)
-            )
-        else:
-            raise ValueError("raw_counts must be a numpy array or scipy sparse matrix")
-        self.samples_dataset = None
-        self.n_samples = n_samples
-        self.models = models_dict
-        self.metrics = {}
-
-        self._store_posterior_predictive_samples()
-
-    def __repr__(self) -> str:
-        return (
-            f"--- Posterior Predictive Checks ---\n"
-            f"n_samples = {self.n_samples}\n"
-            f"raw_counts shape = {self.raw_counts.shape}\n"
-            f"models: {list(self.models.keys())}\n"
-            f"metrics: \n{self._metrics_repr()}"
-        )
-
-    def _metrics_repr(self) -> str:
-        def custom_handle_unserializable(o):
-            if isinstance(o, AnnData):
-                return f"AnnData object with n_obs={o.n_obs}, n_vars={o.n_vars}"
-            elif isinstance(o, pd.DataFrame):
-                s = f"Pandas DataFrame with shape={o.shape}, "
-                n_cols = 5
-                if len(o.columns) > n_cols:
-                    return s + f"first {n_cols} columns={o.columns[:n_cols].to_list()}"
-                return s + f"columns={o.columns.to_list()}"
-            elif isinstance(o, pd.Series):
-                return f"Pandas Series with n_rows={len(o)}"
-            return f"ERROR unserializable type: {type(o)}"
-
-        return json.dumps(self.metrics, indent=4, default=custom_handle_unserializable)
+        # TODO, catch user warning here and logger warning
+        # about non count data
+        super().__init__(adata)
+
+        self.n_labels = 2
+        self.module = Classifier(
+            n_input=self.summary_stats.n_vars,
+            n_labels=self.n_labels,
+            logits=True,
+            **classifier_kwargs,
+        )
+        self._model_summary_string = "Solo model"
+        self.init_params_ = self._get_init_params(locals())
 
-    def _store_posterior_predictive_samples(
-        self,
-        batch_size: int = 32,
-        indices: List[int] = None,
+    @classmethod
+    def from_scvi_model(
+        cls,
+        scvi_model: SCVI,
+        adata: Optional[AnnData] = None,
+        restrict_to_batch: Optional[str] = None,
+        doublet_ratio: int = 2,
+        **classifier_kwargs,
     ):
-        """
-        Store posterior predictive samples for each model.
+        """Instantiate a SOLO model from an scvi model.
 
         Parameters
         ----------
-        models_dict
-            Dictionary of models to store posterior predictive samples for.
-        batch_size
-            Batch size for generating posterior predictive samples.
-        indices
-            Indices to generate posterior predictive samples for.
+        scvi_model
+            Pre-trained model of :class:`~scvi.model.SCVI`. The
+            adata object used to initialize this model should have only
+            been setup with count data, and optionally a `batch_key`;
+            i.e., no extra covariates or labels, etc.
+        adata
+            Optional anndata to use that is compatible with scvi_model.
+        restrict_to_batch
+            Batch category in `batch_key` used to setup adata for scvi_model
+            to restrict Solo model to. This allows to train a Solo model on
+            one batch of a scvi_model that was trained on multiple batches.
+        doublet_ratio
+            Ratio of generated doublets to produce relative to number of
+            cells in adata or length of indices, if not `None`.
+        **classifier_kwargs
+            Keyword args for :class:`~scvi.module.Classifier`
+
+        Returns
+        -------
+        SOLO model
         """
-        self.batch_size = batch_size
+        _validate_scvi_model(scvi_model, restrict_to_batch=restrict_to_batch)
+        orig_adata_manager = scvi_model.adata_manager
+        orig_batch_key = orig_adata_manager.get_state_registry(
+            REGISTRY_KEYS.BATCH_KEY
+        ).original_key
+        orig_labels_key = orig_adata_manager.get_state_registry(
+            REGISTRY_KEYS.LABELS_KEY
+        ).original_key
+
+        if adata is not None:
+            adata_manager = orig_adata_manager.transfer_fields(adata)
+            cls.register_manager(adata_manager)
+        else:
+            adata_manager = orig_adata_manager
+        adata = adata_manager.adata
 
-        samples_dict = {}
-        for m, model in self.models.items():
-            pp_counts = model.posterior_predictive_sample(
-                model.adata,
-                n_samples=self.n_samples,
-                batch_size=self.batch_size,
-                indices=indices,
-            )
-            samples_dict[m] = DataArray(
-                data=pp_counts,
-                coords={
-                    "cells": self.adata.obs_names,
-                    "features": model.adata.var_names,
-                    "samples": np.arange(self.n_samples),
-                },
-            )
-        samples_dict[DATA_VAR_RAW] = DataArray(
-            data=self.raw_counts,
-            coords={"cells": self.adata.obs_names, "features": self.adata.var_names},
+        if restrict_to_batch is not None:
+            batch_mask = adata.obs[orig_batch_key] == restrict_to_batch
+            if np.sum(batch_mask) == 0:
+                raise ValueError(
+                    "Batch category given to restrict_to_batch not found.\n"
+                    + "Available categories: {}".format(
+                        adata.obs[orig_batch_key].astype("category").cat.categories
+                    )
+                )
+            # indices in adata with restrict_to_batch category
+            batch_indices = np.where(batch_mask)[0]
+        else:
+            # use all indices
+            batch_indices = None
+
+        # anndata with only generated doublets
+        doublet_adata = cls.create_doublets(
+            adata_manager, indices=batch_indices, doublet_ratio=doublet_ratio
+        )
+        # if scvi wasn't trained with batch correction having the
+        # zeros here does nothing.
+        doublet_adata.obs[orig_batch_key] = (
+            restrict_to_batch if restrict_to_batch is not None else 0
         )
-        self.samples_dataset = Dataset(samples_dict)
 
-    def coefficient_of_variation(self, dim: Dims = "cells") -> None:
-        """
-        Calculate the coefficient of variation (CV) for each model and the raw counts.
+        # Create dummy labels column set to first label in adata (does not affect inference).
+        dummy_label = orig_adata_manager.get_state_registry(
+            REGISTRY_KEYS.LABELS_KEY
+        ).categorical_mapping[0]
+        doublet_adata.obs[orig_labels_key] = dummy_label
+
+        # if model is using observed lib size, needs to get lib sample
+        # which is just observed lib size on log scale
+        give_mean_lib = not scvi_model.module.use_observed_lib_size
+
+        # get latent representations and make input anndata
+        latent_rep = scvi_model.get_latent_representation(adata, indices=batch_indices)
+        lib_size = scvi_model.get_latent_library_size(
+            adata, indices=batch_indices, give_mean=give_mean_lib
+        )
+        latent_adata = AnnData(np.concatenate([latent_rep, np.log(lib_size)], axis=1))
+        latent_adata.obs[LABELS_KEY] = "singlet"
+        orig_obs_names = adata.obs_names
+        latent_adata.obs_names = (
+            orig_obs_names[batch_indices]
+            if batch_indices is not None
+            else orig_obs_names
+        )
 
-        The CV is computed over the cells or features dimension per sample. The mean CV is then
-        computed over all samples.
+        logger.info("Creating doublets, preparing SOLO model.")
+        f = io.StringIO()
+        with redirect_stdout(f):
+            doublet_latent_rep = scvi_model.get_latent_representation(doublet_adata)
+            doublet_lib_size = scvi_model.get_latent_library_size(
+                doublet_adata, give_mean=give_mean_lib
+            )
+            doublet_adata = AnnData(
+                np.concatenate([doublet_latent_rep, np.log(doublet_lib_size)], axis=1)
+            )
+            doublet_adata.obs[LABELS_KEY] = "doublet"
+
+            full_adata = anndata.concat([latent_adata, doublet_adata])
+            cls.setup_anndata(full_adata, labels_key=LABELS_KEY)
+        return cls(full_adata, **classifier_kwargs)
+
+    @classmethod
+    def create_doublets(
+        cls,
+        adata_manager: AnnDataManager,
+        doublet_ratio: int,
+        indices: Optional[Sequence[int]] = None,
+        seed: int = 1,
+    ) -> AnnData:
+        """Simulate doublets.
 
         Parameters
         ----------
-        dim
-            Dimension to compute CV over.
+        adata
+            AnnData object setup with setup_anndata.
+        doublet_ratio
+            Ratio of generated doublets to produce relative to number of
+            cells in adata or length of indices, if not `None`.
+        indices
+            Indices of cells in adata to use. If `None`, all cells are used.
+        seed
+            Seed for reproducibility
         """
-        identifier = METRIC_CV_CELL if dim == "features" else METRIC_CV_GENE
-        mean = self.samples_dataset.mean(dim=dim, skipna=False)
-        # we use a trick to compute the std to speed it up: std = E[X^2] - E[X]^2
-        # a square followed by a sqrt is ok here because this is counts data (no negative values)
-        self.samples_dataset = np.square(self.samples_dataset)
-        std = np.sqrt(
-            self.samples_dataset.mean(dim=dim, skipna=False) - np.square(mean)
-        )
-        self.samples_dataset = np.sqrt(self.samples_dataset)
-        # now compute the CV
-        cv = std / mean
-        # It's ok to make things dense here
-        cv = _make_dataset_dense(cv)
-        cv_mean = cv.mean(dim="samples", skipna=True)
-        cv_mean[DATA_VAR_RAW].data = np.nan_to_num(cv_mean[DATA_VAR_RAW].data)
-        self.metrics[identifier] = cv_mean.to_dataframe()
-
-    def zero_fraction(self) -> None:
-        """Fraction of zeros in raw counts for a specific gene"""
-        pp_samples = self.samples_dataset
-        mean = (
-            (pp_samples != 0)
-            .mean(dim="cells", skipna=False)
-            .mean(dim="samples", skipna=False)
-        )
-        mean = _make_dataset_dense(mean)
-        self.metrics[METRIC_ZERO_FRACTION] = mean.to_dataframe()
-
-    def calibration_error(
-        self, confidence_intervals: Optional[List[float]] = None
-    ) -> None:
-        """Calibration error for each observed count.
-
-        For a series of credible intervals of the samples, the fraction of observed counts that fall
-        within the credible interval is computed. The calibration error is then the squared difference
-        between the observed fraction and the true interval width.
+        adata = adata_manager.adata
+        n_obs = adata.n_obs if indices is None else len(indices)
+        num_doublets = doublet_ratio * n_obs
+
+        # counts can be in many locations, this uses where it was registered in setup
+        x = adata_manager.get_from_registry(REGISTRY_KEYS.X_KEY)
+        if indices is not None:
+            x = x[indices]
+
+        random_state = np.random.RandomState(seed=seed)
+        parent_inds = random_state.choice(n_obs, size=(num_doublets, 2))
+        doublets = x[parent_inds[:, 0]] + x[parent_inds[:, 1]]
+
+        doublets_ad = AnnData(doublets)
+        doublets_ad.var_names = adata.var_names
+        doublets_ad.obs_names = [f"sim_doublet_{i}" for i in range(num_doublets)]
+
+        # if adata setup with a layer, need to add layer to doublets adata
+        layer = adata_manager.data_registry[REGISTRY_KEYS.X_KEY].attr_key
+        if layer is not None:
+            doublets_ad.layers[layer] = doublets
 
-        For this metric, lower is better.
+        return doublets_ad
+
+    @devices_dsp.dedent
+    def train(
+        self,
+        max_epochs: int = 400,
+        lr: float = 1e-3,
+        use_gpu: Optional[Union[str, int, bool]] = None,
+        accelerator: str = "auto",
+        devices: Union[int, List[int], str] = "auto",
+        train_size: float = 0.9,
+        validation_size: Optional[float] = None,
+        shuffle_set_split: bool = True,
+        batch_size: int = 128,
+        plan_kwargs: Optional[dict] = None,
+        early_stopping: bool = True,
+        early_stopping_patience: int = 30,
+        early_stopping_min_delta: float = 0.0,
+        **kwargs,
+    ):
+        """Trains the model.
 
         Parameters
         ----------
-        confidence_intervals
-            List of confidence intervals to compute calibration error for.
-            E.g., [0.01, 0.02, 0.98, 0.99]
-
-        Notes
-        -----
-        This does not work on sparse data and can cause large memory usage.
+        max_epochs
+            Number of epochs to train for
+        lr
+            Learning rate for optimization.
+        %(param_use_gpu)s
+        %(param_accelerator)s
+        %(param_devices)s
+        train_size
+            Size of training set in the range [0.0, 1.0].
+        validation_size
+            Size of the test set. If `None`, defaults to 1 - `train_size`. If
+            `train_size + validation_size < 1`, the remaining cells belong to a test set.
+        shuffle_set_split
+            Whether to shuffle indices before splitting. If `False`, the val, train, and test set are split in the
+            sequential order of the data according to `validation_size` and `train_size` percentages.
+        batch_size
+            Minibatch size to use during training.
+        plan_kwargs
+            Keyword args for :class:`~scvi.train.ClassifierTrainingPlan`. Keyword arguments passed to
+        early_stopping
+            Adds callback for early stopping on validation_loss
+        early_stopping_patience
+            Number of times early stopping metric can not improve over early_stopping_min_delta
+        early_stopping_min_delta
+            Threshold for counting an epoch torwards patience
+            `train()` will overwrite values present in `plan_kwargs`, when appropriate.
+        **kwargs
+            Other keyword args for :class:`~scvi.train.Trainer`.
         """
-        if confidence_intervals is None:
-            ps = [2.5, 5, 7.5, 10, 12.5, 15, 17.5, 82.5, 85, 87.5, 90, 92.5, 95, 97.5]
-            ps = [p / 100 for p in ps]
+        update_dict = {
+            "lr": lr,
+        }
+        if plan_kwargs is not None:
+            plan_kwargs.update(update_dict)
         else:
-            if len(confidence_intervals) % 2 != 0:
-                raise ValueError("Confidence intervals must be even")
-            ps = confidence_intervals
-        pp_samples = self.samples_dataset
-        # TODO: Reimplement to work on sparse data
-        pp_samples = _make_dataset_dense(pp_samples)
-        # results in (quantiles, cells, features)
-        quants = pp_samples.quantile(q=ps, dim="samples", skipna=False)
-        credible_interval_indices = [
-            (i, len(ps) - (i + 1)) for i in range(len(ps) // 2)
-        ]
+            plan_kwargs = update_dict
 
-        model_cal = {}
-        for model in pp_samples.data_vars:
-            if model == DATA_VAR_RAW:
-                continue
-            cal_error_features = 0
-            for interval in credible_interval_indices:
-                start = interval[0]
-                end = interval[1]
-                true_width = ps[end] - ps[start]
-                greater_than = (
-                    quants[DATA_VAR_RAW] >= quants.model1.isel(quantile=start)
-                ).data
-                less_than = (
-                    quants[DATA_VAR_RAW] <= quants.model1.isel(quantile=end)
-                ).data
-                # Logical and
-                ci = greater_than * less_than
-                pci_features = ci.mean()
-                cal_error_features += (pci_features - true_width) ** 2
-            model_cal[model] = {
-                "features": cal_error_features,
-            }
-        self.metrics[METRIC_CALIBRATION] = pd.DataFrame.from_dict(model_cal)
-
-    @dependencies("scanpy")
-    def differential_expression(
-        self,
-        de_groupby: str,
-        de_method: str = "t-test",
-        n_samples: int = 1,
-        cell_scale_factor: float = 1e4,
-        p_val_thresh: float = DEFAULT_DE_P_VAL_THRESHOLD,
-        n_top_genes_fallback: int = DEFAULT_DE_N_TOP_GENES_OVERLAP,
-    ):
-        """
-        Compute differential expression (DE) metrics.
+        if early_stopping:
+            early_stopping_callback = [
+                LoudEarlyStopping(
+                    monitor="validation_loss" if train_size != 1.0 else "train_loss",
+                    min_delta=early_stopping_min_delta,
+                    patience=early_stopping_patience,
+                    mode="min",
+                )
+            ]
+            if "callbacks" in kwargs:
+                kwargs["callbacks"] += early_stopping_callback
+            else:
+                kwargs["callbacks"] = early_stopping_callback
+            kwargs["check_val_every_n_epoch"] = 1
+
+        if max_epochs is None:
+            n_cells = self.adata.n_obs
+            max_epochs = int(np.min([round((20000 / n_cells) * 400), 400]))
+
+        plan_kwargs = plan_kwargs if isinstance(plan_kwargs, dict) else {}
+
+        data_splitter = DataSplitter(
+            self.adata_manager,
+            train_size=train_size,
+            validation_size=validation_size,
+            shuffle_set_split=shuffle_set_split,
+            batch_size=batch_size,
+        )
+        training_plan = ClassifierTrainingPlan(
+            self.module, self.n_labels, **plan_kwargs
+        )
+        runner = TrainRunner(
+            self,
+            training_plan=training_plan,
+            data_splitter=data_splitter,
+            max_epochs=max_epochs,
+            use_gpu=use_gpu,
+            accelerator=accelerator,
+            devices=devices,
+            **kwargs,
+        )
+        return runner()
 
-        If n_samples > 1, all metrics are averaged over a posterior predictive dataset.
+    @torch.inference_mode()
+    def predict(
+        self, soft: bool = True, include_simulated_doublets: bool = False
+    ) -> pd.DataFrame:
+        """Return doublet predictions.
 
         Parameters
         ----------
-        de_groupby
-            The column name in `adata_obs_raw` that contains the groupby information.
-        de_method
-            The DE method to use. See :meth:`~scanpy.tl.rank_genes_groups` for more details.
-        n_samples
-            The number of posterior predictive samples to use for the DE analysis.
-        cell_scale_factor
-            The cell scale factor to use for normalization before DE.
-        p_val_thresh
-            The p-value threshold to use for the DE analysis.
-        n_top_genes_fallback
-            The number of top genes to use for the DE analysis if the number of genes
-            with a p-value < p_val_thresh is zero.
+        soft
+            Return probabilities instead of class label
+        include_simulated_doublets
+            Return probabilities for simulated doublets as well.
+
+        Returns
+        -------
+        DataFrame with prediction, index corresponding to cell barcode.
         """
-        import scanpy as sc
+        adata = self._validate_anndata(None)
 
-        if n_samples > self.n_samples:
-            raise ValueError(
-                f"n_samples={n_samples} is greater than the number of samples already recorded "
-                f"({self.n_samples})"
-            )
-        # run DE with the raw counts
-        adata_de = AnnData(
-            X=self.raw_counts.to_scipy_sparse().tocsr().copy(),
-            obs=self.adata.obs,
-            var=self.adata.var,
-        )
-        sc.pp.normalize_total(adata_de, target_sum=cell_scale_factor)
-        sc.pp.log1p(adata_de)
-        with warnings.catch_warnings():
-            warnings.simplefilter(
-                action="ignore", category=pd.errors.PerformanceWarning
-            )
-            sc.tl.rank_genes_groups(
-                adata_de,
-                de_groupby,
-                use_raw=False,
-                method=de_method,
-                key_added=UNS_NAME_RGG_RAW,
-            )
+        scdl = self._make_data_loader(
+            adata=adata,
+        )
 
-        # get posterior predictive samples from the model (aka approx counts)
-        pp_samples = self.samples_dataset
-        # create adata object to run DE on the approx counts
-        # X here will be overwritten
-        adata_approx = AnnData(X=adata_de.X, obs=adata_de.obs, var=adata_de.var)
-        de_keys = {}
-        models = [model for model in pp_samples.data_vars if model != DATA_VAR_RAW]
-        for model in models:
-            if model not in de_keys:
-                de_keys[model] = []
-            for k in range(n_samples):
-                one_sample = pp_samples[model].isel(samples=k)
-                # overwrite X with the posterior predictive sample
-                # This allows us to save all the DE results in the same adata object
-                one_sample_data = (
-                    one_sample.data.to_scipy_sparse().tocsr()
-                    if isinstance(one_sample.data, SparseArray)
-                    else one_sample
-                )
-                adata_approx.X = one_sample_data.copy()
-                sc.pp.normalize_total(adata_approx, target_sum=cell_scale_factor)
-                sc.pp.log1p(adata_approx)
-
-                # run DE with the imputed normalized data
-                with warnings.catch_warnings():
-                    warnings.simplefilter(
-                        action="ignore", category=pd.errors.PerformanceWarning
-                    )
-                    key_added = f"{UNS_NAME_RGG_PPC}_{model}_sample_{k}"
-                    de_keys[model].append(key_added)
-                    sc.tl.rank_genes_groups(
-                        adata_approx,
-                        de_groupby,
-                        use_raw=False,
-                        method=de_method,
-                        key_added=key_added,
-                    )
+        @auto_move_data
+        def auto_forward(module, x):
+            return module(x)
 
-        groups = self.adata.obs[de_groupby].astype("category").cat.categories
-        df = pd.DataFrame(
-            index=np.arange(len(groups) * len(models)),
-            columns=[
-                "gene_overlap_f1",
-                "lfc_mae",
-                "lfc_pearson",
-                "lfc_spearman",
-                "roc_auc",
-                "pr_auc",
-                "group",
-                "model",
-            ],
-        )
-        i = 0
-        for g in groups:
-            raw_group_data = sc.get.rank_genes_groups_df(
-                adata_de, group=g, key=UNS_NAME_RGG_RAW
-            )
-            raw_group_data.set_index("names", inplace=True)
-            for model in de_keys.keys():
-                gene_overlap_f1s = []
-                lfc_maes = []
-                lfc_pearsons = []
-                lfc_spearmans = []
-                roc_aucs = []
-                pr_aucs = []
-                # Now over potential samples
-                for de_key in de_keys[model]:
-                    sample_group_data = sc.get.rank_genes_groups_df(
-                        adata_approx, group=g, key=de_key
-                    )
-                    sample_group_data.set_index("names", inplace=True)
-                    # compute gene overlaps
-                    all_genes = raw_group_data.index  # order doesn't matter here
-                    top_genes_raw = raw_group_data[:n_top_genes_fallback].index
-                    top_genes_sample = sample_group_data[:n_top_genes_fallback].index
-                    true_genes = np.array(
-                        [0 if g not in top_genes_raw else 1 for g in all_genes]
-                    )
-                    pred_genes = np.array(
-                        [0 if g not in top_genes_sample else 1 for g in all_genes]
-                    )
-                    gene_overlap_f1s.append(
-                        _get_precision_recall_f1(true_genes, pred_genes)[2]
-                    )
-                    # compute lfc correlations
-                    sample_group_data = sample_group_data.loc[raw_group_data.index]
-                    rgd, sgd = (
-                        raw_group_data["logfoldchanges"],
-                        sample_group_data["logfoldchanges"],
-                    )
-                    lfc_maes.append(np.mean(np.abs(rgd - sgd)))
-                    lfc_pearsons.append(pearsonr(rgd, sgd)[0])
-                    lfc_spearmans.append(spearmanr(rgd, sgd)[0])
-                    # compute auPRC and auROC
-                    raw_adj_p_vals = raw_group_data["pvals_adj"]
-                    true = raw_adj_p_vals < p_val_thresh
-                    pred = sample_group_data["scores"]
-                    if true.sum() == 0:
-                        # if there are no true DE genes, just use the top n genes
-                        true = np.zeros_like(pred)
-                        true[np.argsort(raw_adj_p_vals)[:n_top_genes_fallback]] = 1
-                    roc_aucs.append(roc_auc_score(true, pred))
-                    pr_aucs.append(average_precision_score(true, pred))
-                # Mean here is over sampled datasets
-                df.loc[i, "model"] = model
-                df.loc[i, "group"] = g
-                df.loc[i, "gene_overlap_f1"] = np.mean(gene_overlap_f1s)
-                df.loc[i, "lfc_mae"] = np.mean(lfc_maes)
-                df.loc[i, "lfc_pearson"] = np.mean(lfc_pearsons)
-                df.loc[i, "lfc_spearman"] = np.mean(lfc_spearmans)
-                df.loc[i, "roc_auc"] = np.mean(roc_aucs)
-                df.loc[i, "pr_auc"] = np.mean(pr_aucs)
-                i += 1
+        y_pred = []
+        for _, tensors in enumerate(scdl):
+            x = tensors[REGISTRY_KEYS.X_KEY]
+            pred = auto_forward(self.module, x)
+            y_pred.append(pred.cpu())
 
-        self.metrics[METRIC_DIFF_EXP] = df
+        y_pred = torch.cat(y_pred).numpy()
+
+        label = self.adata.obs["_solo_doub_sim"].values.ravel()
+        mask = label == "singlet" if not include_simulated_doublets else slice(None)
+
+        preds = y_pred[mask]
+
+        cols = self.adata_manager.get_state_registry(
+            REGISTRY_KEYS.LABELS_KEY
+        ).categorical_mapping
+        preds_df = pd.DataFrame(preds, columns=cols, index=self.adata.obs_names[mask])
+
+        if not soft:
+            preds_df = preds_df.idxmax(axis=1)
+
+        return preds_df
+
+    @classmethod
+    @setup_anndata_dsp.dedent
+    def setup_anndata(
+        cls,
+        adata: AnnData,
+        labels_key: Optional[str] = None,
+        layer: Optional[str] = None,
+        **kwargs,
+    ):
+        """%(summary)s.
+
+        Parameters
+        ----------
+        %(param_labels_key)s
+        %(param_layer)s
+        """
+        setup_method_args = cls._get_setup_method_args(**locals())
+        anndata_fields = [
+            LayerField(REGISTRY_KEYS.X_KEY, layer, is_count_data=False),
+            CategoricalObsField(REGISTRY_KEYS.LABELS_KEY, labels_key),
+        ]
+        adata_manager = AnnDataManager(
+            fields=anndata_fields, setup_method_args=setup_method_args
+        )
+        adata_manager.register_fields(adata, **kwargs)
+        cls.register_manager(adata_manager)
+
+
+def _validate_scvi_model(scvi_model: SCVI, restrict_to_batch: str):
+    if scvi_model.summary_stats.n_batch > 1 and restrict_to_batch is None:
+        warnings.warn(
+            "Solo should only be trained on one lane of data using `restrict_to_batch`. Performance may suffer.",
+            UserWarning,
+            stacklevel=settings.warnings_stacklevel,
+        )
```

### Comparing `scvi_tools-1.0.0/scvi/data/__init__.py` & `scvi_tools-1.0.0b0/scvi/data/__init__.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/data/_anntorchdataset.py` & `scvi_tools-1.0.0b0/scvi/data/_anntorchdataset.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/data/_compat.py` & `scvi_tools-1.0.0b0/scvi/data/_compat.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/data/_constants.py` & `scvi_tools-1.0.0b0/scvi/data/_constants.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/data/_datasets.py` & `scvi_tools-1.0.0b0/scvi/data/_datasets.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/data/_download.py` & `scvi_tools-1.0.0b0/scvi/data/_download.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/data/_manager.py` & `scvi_tools-1.0.0b0/scvi/data/_manager.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/data/_preprocessing.py` & `scvi_tools-1.0.0b0/scvi/data/_preprocessing.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/data/_read.py` & `scvi_tools-1.0.0b0/scvi/data/_read.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/data/_utils.py` & `scvi_tools-1.0.0b0/scvi/data/_utils.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/data/_built_in_data/_brain_large.py` & `scvi_tools-1.0.0b0/scvi/data/_built_in_data/_brain_large.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/data/_built_in_data/_cellxgene.py` & `scvi_tools-1.0.0b0/scvi/data/_built_in_data/_cellxgene.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/data/_built_in_data/_cite_seq.py` & `scvi_tools-1.0.0b0/scvi/data/_built_in_data/_cite_seq.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/data/_built_in_data/_cortex.py` & `scvi_tools-1.0.0b0/scvi/data/_built_in_data/_cortex.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/data/_built_in_data/_csv.py` & `scvi_tools-1.0.0b0/scvi/data/_built_in_data/_csv.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/data/_built_in_data/_dataset_10x.py` & `scvi_tools-1.0.0b0/scvi/data/_built_in_data/_dataset_10x.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/data/_built_in_data/_heartcellatlas.py` & `scvi_tools-1.0.0b0/scvi/data/_built_in_data/_heartcellatlas.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/data/_built_in_data/_loom.py` & `scvi_tools-1.0.0b0/scvi/data/_built_in_data/_loom.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/data/_built_in_data/_pbmc.py` & `scvi_tools-1.0.0b0/scvi/data/_built_in_data/_pbmc.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/data/_built_in_data/_smfish.py` & `scvi_tools-1.0.0b0/scvi/data/_built_in_data/_smfish.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/data/_built_in_data/_synthetic.py` & `scvi_tools-1.0.0b0/scvi/data/_built_in_data/_synthetic.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/data/fields/__init__.py` & `scvi_tools-1.0.0b0/scvi/data/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/data/fields/_arraylike_field.py` & `scvi_tools-1.0.0b0/scvi/data/fields/_arraylike_field.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/data/fields/_base_field.py` & `scvi_tools-1.0.0b0/scvi/data/fields/_base_field.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/data/fields/_dataframe_field.py` & `scvi_tools-1.0.0b0/scvi/data/fields/_dataframe_field.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/data/fields/_layer_field.py` & `scvi_tools-1.0.0b0/scvi/data/fields/_layer_field.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/data/fields/_mudata.py` & `scvi_tools-1.0.0b0/scvi/data/fields/_mudata.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/data/fields/_protein.py` & `scvi_tools-1.0.0b0/scvi/data/fields/_protein.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/data/fields/_scanvi.py` & `scvi_tools-1.0.0b0/scvi/data/fields/_scanvi.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/data/fields/_uns_field.py` & `scvi_tools-1.0.0b0/scvi/data/fields/_uns_field.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/dataloaders/__init__.py` & `scvi_tools-1.0.0b0/scvi/dataloaders/__init__.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/dataloaders/_ann_dataloader.py` & `scvi_tools-1.0.0b0/scvi/dataloaders/_ann_dataloader.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/dataloaders/_concat_dataloader.py` & `scvi_tools-1.0.0b0/scvi/dataloaders/_concat_dataloader.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,32 +36,25 @@
         indices_list: List[List[int]],
         shuffle: bool = False,
         batch_size: int = 128,
         data_and_attributes: Optional[dict] = None,
         drop_last: Union[bool, int] = False,
         **data_loader_kwargs,
     ):
-        self.adata_manager = adata_manager
-        self.dataloader_kwargs = data_loader_kwargs
-        self.data_and_attributes = data_and_attributes
-        self._shuffle = shuffle
-        self._batch_size = batch_size
-        self._drop_last = drop_last
-
         self.dataloaders = []
         for indices in indices_list:
             self.dataloaders.append(
                 AnnDataLoader(
                     adata_manager,
                     indices=indices,
                     shuffle=shuffle,
                     batch_size=batch_size,
                     data_and_attributes=data_and_attributes,
                     drop_last=drop_last,
-                    **self.dataloader_kwargs,
+                    **data_loader_kwargs,
                 )
             )
         lens = [len(dl) for dl in self.dataloaders]
         self.largest_dl = self.dataloaders[np.argmax(lens)]
         super().__init__(self.largest_dl, **data_loader_kwargs)
 
     def __len__(self):
```

### Comparing `scvi_tools-1.0.0/scvi/dataloaders/_data_splitting.py` & `scvi_tools-1.0.0b0/scvi/dataloaders/_data_splitting.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/dataloaders/_semi_dataloader.py` & `scvi_tools-1.0.0b0/scvi/dataloaders/_semi_dataloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import numpy as np
 
 from scvi import REGISTRY_KEYS
 from scvi.data import AnnDataManager
 from scvi.data._utils import get_anndata_attribute
 
-from ._ann_dataloader import AnnDataLoader
 from ._concat_dataloader import ConcatDataLoader
 
 
 class SemiSupervisedDataLoader(ConcatDataLoader):
     """DataLoader that supports semisupervised training.
 
     Parameters
@@ -86,22 +85,15 @@
 
     def resample_labels(self):
         """Resamples the labeled data."""
         labelled_idx = self.subsample_labels()
         # self.dataloaders[0] iterates over full_indices
         # self.dataloaders[1] iterates over the labelled_indices
         # change the indices of the labelled set
-        self.dataloaders[1] = AnnDataLoader(
-            self.adata_manager,
-            indices=labelled_idx,
-            shuffle=self._shuffle,
-            batch_size=self._batch_size,
-            data_and_attributes=self.data_and_attributes,
-            drop_last=self._drop_last,
-        )
+        self.dataloaders[1].indices = labelled_idx
 
     def subsample_labels(self):
         """Subsamples each label class by taking up to n_samples_per_label samples per class."""
         if self.n_samples_per_label is None:
             return np.concatenate(self.labeled_locs)
 
         sample_idx = []
```

### Comparing `scvi_tools-1.0.0/scvi/distributions/_negative_binomial.py` & `scvi_tools-1.0.0b0/scvi/distributions/_negative_binomial.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/distributions/_utils.py` & `scvi_tools-1.0.0b0/scvi/distributions/_utils.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/external/cellassign/_model.py` & `scvi_tools-1.0.0b0/scvi/external/cellassign/_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     CategoricalObsField,
     LayerField,
     NumericalJointObsField,
     NumericalObsField,
 )
 from scvi.dataloaders import DataSplitter
 from scvi.external.cellassign._module import CellAssignModule
-from scvi.model._utils import get_max_epochs_heuristic
 from scvi.model.base import BaseModelClass, UnsupervisedTrainingMixin
 from scvi.train import LoudEarlyStopping, TrainingPlan, TrainRunner
 from scvi.utils import setup_anndata_dsp
 from scvi.utils._docstrings import devices_dsp
 
 logger = logging.getLogger(__name__)
 
@@ -202,15 +201,16 @@
             if "callbacks" in kwargs:
                 kwargs["callbacks"] += early_stopping_callback
             else:
                 kwargs["callbacks"] = early_stopping_callback
             kwargs["check_val_every_n_epoch"] = 1
 
         if max_epochs is None:
-            max_epochs = get_max_epochs_heuristic(self.adata.n_obs)
+            n_cells = self.adata.n_obs
+            max_epochs = int(np.min([round((20000 / n_cells) * 400), 400]))
 
         plan_kwargs = plan_kwargs if isinstance(plan_kwargs, dict) else {}
 
         data_splitter = DataSplitter(
             self.adata_manager,
             train_size=train_size,
             validation_size=validation_size,
```

### Comparing `scvi_tools-1.0.0/scvi/external/cellassign/_module.py` & `scvi_tools-1.0.0b0/scvi/external/cellassign/_module.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/external/gimvi/_model.py` & `scvi_tools-1.0.0b0/scvi/external/gimvi/_model.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/external/gimvi/_module.py` & `scvi_tools-1.0.0b0/scvi/external/gimvi/_module.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/external/gimvi/_task.py` & `scvi_tools-1.0.0b0/scvi/external/gimvi/_task.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/external/gimvi/_utils.py` & `scvi_tools-1.0.0b0/scvi/external/gimvi/_utils.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/external/scar/_model.py` & `scvi_tools-1.0.0b0/scvi/external/scar/_model.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/external/scar/_module.py` & `scvi_tools-1.0.0b0/scvi/external/scar/_module.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/external/scbasset/_model.py` & `scvi_tools-1.0.0b0/scvi/external/scbasset/_model.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/external/scbasset/_module.py` & `scvi_tools-1.0.0b0/scvi/external/scbasset/_module.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/external/solo/_model.py` & `scvi_tools-1.0.0b0/scvi/model/_destvi.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,312 +1,332 @@
-import io
 import logging
-import warnings
-from contextlib import redirect_stdout
-from typing import List, Optional, Sequence, Union
+from collections import OrderedDict
+from typing import Dict, List, Optional, Sequence, Union
 
-import anndata
 import numpy as np
 import pandas as pd
 import torch
 from anndata import AnnData
 
-from scvi import REGISTRY_KEYS, settings
+from scvi import REGISTRY_KEYS
 from scvi.data import AnnDataManager
-from scvi.data.fields import CategoricalObsField, LayerField
-from scvi.dataloaders import DataSplitter
-from scvi.model import SCVI
-from scvi.model._utils import get_max_epochs_heuristic
-from scvi.model.base import BaseModelClass
-from scvi.module import Classifier
-from scvi.module.base import auto_move_data
-from scvi.train import ClassifierTrainingPlan, LoudEarlyStopping, TrainRunner
+from scvi.data.fields import LayerField, NumericalObsField
+from scvi.model import CondSCVI
+from scvi.model.base import BaseModelClass, UnsupervisedTrainingMixin
+from scvi.module import MRDeconv
 from scvi.utils import setup_anndata_dsp
 from scvi.utils._docstrings import devices_dsp
 
 logger = logging.getLogger(__name__)
 
-LABELS_KEY = "_solo_doub_sim"
 
-
-class SOLO(BaseModelClass):
-    """Doublet detection in scRNA-seq :cite:p:`Bernstein20`.
-
-    Most users will initialize the model using the class method
-    :meth:`~scvi.external.SOLO.from_scvi_model`, which takes as
-    input a pre-trained :class:`~scvi.model.SCVI` object.
+class DestVI(UnsupervisedTrainingMixin, BaseModelClass):
+    """Multi-resolution deconvolution of Spatial Transcriptomics data (DestVI) :cite:p:`Lopez21`. Most users will use the alternate constructor (see example).
 
     Parameters
     ----------
-    adata
-        AnnData object that has been registered via :meth:`~scvi.model.SCVI.setup_anndata`.
-        Object should contain latent representation of real cells and doublets as `adata.X`.
-        Object should also be registered, using `.X` and `labels_key="_solo_doub_sim"`.
-    **classifier_kwargs
-        Keyword args for :class:`~scvi.module.Classifier`
+    st_adata
+        spatial transcriptomics AnnData object that has been registered via :meth:`~scvi.model.DestVI.setup_anndata`.
+    cell_type_mapping
+        mapping between numerals and cell type labels
+    decoder_state_dict
+        state_dict from the decoder of the CondSCVI model
+    px_decoder_state_dict
+        state_dict from the px_decoder of the CondSCVI model
+    px_r
+        parameters for the px_r tensor in the CondSCVI model
+    n_hidden
+        Number of nodes per hidden layer.
+    n_latent
+        Dimensionality of the latent space.
+    n_layers
+        Number of hidden layers used for encoder and decoder NNs.
+    **module_kwargs
+        Keyword args for :class:`~scvi.modules.MRDeconv`
 
     Examples
     --------
-    In the case of scVI trained with multiple batches:
-
-    >>> adata = anndata.read_h5ad(path_to_anndata)
-    >>> scvi.model.SCVI.setup_anndata(adata, batch_key="batch")
-    >>> vae = scvi.model.SCVI(adata)
-    >>> vae.train()
-    >>> solo_batch_1 = scvi.external.SOLO.from_scvi_model(vae, restrict_to_batch="batch 1")
-    >>> solo_batch_1.train()
-    >>> solo_batch_1.predict()
-
-    Otherwise:
-
-    >>> adata = anndata.read_h5ad(path_to_anndata)
-    >>> scvi.model.SCVI.setup_anndata(adata)
-    >>> vae = scvi.model.SCVI(adata)
-    >>> vae.train()
-    >>> solo = scvi.external.SOLO.from_scvi_model(vae)
-    >>> solo.train()
-    >>> solo.predict()
+    >>> sc_adata = anndata.read_h5ad(path_to_scRNA_anndata)
+    >>> scvi.model.CondSCVI.setup_anndata(sc_adata)
+    >>> sc_model = scvi.model.CondSCVI(sc_adata)
+    >>> st_adata = anndata.read_h5ad(path_to_ST_anndata)
+    >>> DestVI.setup_anndata(st_adata)
+    >>> spatial_model = DestVI.from_rna_model(st_adata, sc_model)
+    >>> spatial_model.train(max_epochs=2000)
+    >>> st_adata.obsm["proportions"] = spatial_model.get_proportions(st_adata)
+    >>> gamma = spatial_model.get_gamma(st_adata)
 
     Notes
     -----
-    Solo should be trained on one lane of data at a time. An
-    :class:`~scvi.model.SCVI` instance that was trained with multiple
-    batches can be used as input, but Solo should be created and run
-    multiple times, each with a new `restrict_to_batch` in
-    :meth:`~scvi.external.SOLO.from_scvi_model`.
+    See further usage examples in the following tutorials:
+
+    1. :doc:`/tutorials/notebooks/DestVI_tutorial`
     """
 
+    _module_cls = MRDeconv
+
     def __init__(
         self,
-        adata: AnnData,
-        **classifier_kwargs,
+        st_adata: AnnData,
+        cell_type_mapping: np.ndarray,
+        decoder_state_dict: OrderedDict,
+        px_decoder_state_dict: OrderedDict,
+        px_r: np.ndarray,
+        n_hidden: int,
+        n_latent: int,
+        n_layers: int,
+        dropout_decoder: float,
+        l1_reg: float,
+        **module_kwargs,
     ):
-        # TODO, catch user warning here and logger warning
-        # about non count data
-        super().__init__(adata)
-
-        self.n_labels = 2
-        self.module = Classifier(
-            n_input=self.summary_stats.n_vars,
-            n_labels=self.n_labels,
-            logits=True,
-            **classifier_kwargs,
+        super().__init__(st_adata)
+        self.module = self._module_cls(
+            n_spots=st_adata.n_obs,
+            n_labels=cell_type_mapping.shape[0],
+            decoder_state_dict=decoder_state_dict,
+            px_decoder_state_dict=px_decoder_state_dict,
+            px_r=px_r,
+            n_genes=st_adata.n_vars,
+            n_latent=n_latent,
+            n_layers=n_layers,
+            n_hidden=n_hidden,
+            dropout_decoder=dropout_decoder,
+            l1_reg=l1_reg,
+            **module_kwargs,
         )
-        self._model_summary_string = "Solo model"
+        self.cell_type_mapping = cell_type_mapping
+        self._model_summary_string = "DestVI Model"
         self.init_params_ = self._get_init_params(locals())
 
     @classmethod
-    def from_scvi_model(
+    def from_rna_model(
         cls,
-        scvi_model: SCVI,
-        adata: Optional[AnnData] = None,
-        restrict_to_batch: Optional[str] = None,
-        doublet_ratio: int = 2,
-        **classifier_kwargs,
+        st_adata: AnnData,
+        sc_model: CondSCVI,
+        vamp_prior_p: int = 15,
+        l1_reg: float = 0.0,
+        **module_kwargs,
     ):
-        """Instantiate a SOLO model from an scvi model.
+        """Alternate constructor for exploiting a pre-trained model on a RNA-seq dataset.
 
         Parameters
         ----------
-        scvi_model
-            Pre-trained :class:`~scvi.model.SCVI` model. The AnnData object used to
-            initialize this model should have only been setup with count data, and
-            optionally a `batch_key`. Extra categorical and continuous covariates are
-            currenty unsupported.
-        adata
-            Optional AnnData to use that is compatible with `scvi_model`.
-        restrict_to_batch
-            Batch category to restrict the SOLO model to if `scvi_model` was set up with
-            a `batch_key`. This allows the model to be trained on the subset of cells
-            belonging to `restrict_to_batch` when `scvi_model` was trained on multiple
-            batches. If `None`, all cells are used.
-        doublet_ratio
-            Ratio of generated doublets to produce relative to number of
-            cells in adata or length of indices, if not `None`.
-        **classifier_kwargs
-            Keyword args for :class:`~scvi.module.Classifier`
-
-        Returns
-        -------
-        SOLO model
+        st_adata
+            registered anndata object
+        sc_model
+            trained CondSCVI model
+        vamp_prior_p
+            number of mixture parameter for VampPrior calculations
+        l1_reg
+            Scalar parameter indicating the strength of L1 regularization on cell type proportions.
+            A value of 50 leads to sparser results.
+        **model_kwargs
+            Keyword args for :class:`~scvi.model.DestVI`
         """
-        _validate_scvi_model(scvi_model, restrict_to_batch=restrict_to_batch)
-        orig_adata_manager = scvi_model.adata_manager
-        orig_batch_key_registry = orig_adata_manager.get_state_registry(
-            REGISTRY_KEYS.BATCH_KEY
-        )
-        orig_labels_key_registry = orig_adata_manager.get_state_registry(
+        decoder_state_dict = sc_model.module.decoder.state_dict()
+        px_decoder_state_dict = sc_model.module.px_decoder.state_dict()
+        px_r = sc_model.module.px_r.detach().cpu().numpy()
+        mapping = sc_model.adata_manager.get_state_registry(
             REGISTRY_KEYS.LABELS_KEY
+        ).categorical_mapping
+        dropout_decoder = sc_model.module.dropout_rate
+        if vamp_prior_p is None:
+            mean_vprior = None
+            var_vprior = None
+        else:
+            mean_vprior, var_vprior, mp_vprior = sc_model.get_vamp_prior(
+                sc_model.adata, p=vamp_prior_p
+            )
+
+        return cls(
+            st_adata,
+            mapping,
+            decoder_state_dict,
+            px_decoder_state_dict,
+            px_r,
+            sc_model.module.n_hidden,
+            sc_model.module.n_latent,
+            sc_model.module.n_layers,
+            mean_vprior=mean_vprior,
+            var_vprior=var_vprior,
+            mp_vprior=mp_vprior,
+            dropout_decoder=dropout_decoder,
+            l1_reg=l1_reg,
+            **module_kwargs,
         )
-        orig_batch_key = orig_batch_key_registry.original_key
-        orig_labels_key = orig_labels_key_registry.original_key
 
-        if len(orig_adata_manager.get_state_registry(REGISTRY_KEYS.CONT_COVS_KEY)) > 0:
-            raise ValueError(
-                "Initializing a SOLO model from SCVI with registered continuous "
-                "covariates is currently unsupported."
-            )
-        if len(orig_adata_manager.get_state_registry(REGISTRY_KEYS.CAT_COVS_KEY)) > 0:
-            raise ValueError(
-                "Initializing a SOLO model from SCVI with registered categorical "
-                "covariates is currently unsupported."
-            )
-        scvi_trained_with_batch = len(orig_batch_key_registry.categorical_mapping) > 1
-        if not scvi_trained_with_batch and restrict_to_batch is not None:
-            raise ValueError(
-                "Cannot specify `restrict_to_batch` when initializing a SOLO model from SCVI "
-                "not trained with multiple batches."
-            )
-        if scvi_trained_with_batch > 1 and restrict_to_batch is None:
-            warnings.warn(
-                "`restrict_to_batch` not specified but `scvi_model` was trained with "
-                "multiple batches. Doublets will be simulated using the first batch.",
-                UserWarning,
-                stacklevel=settings.warnings_stacklevel,
-            )
+    def get_proportions(
+        self,
+        keep_noise: bool = False,
+        indices: Optional[Sequence[int]] = None,
+        batch_size: Optional[int] = None,
+    ) -> pd.DataFrame:
+        """Returns the estimated cell type proportion for the spatial data.
 
-        if adata is not None:
-            adata_manager = orig_adata_manager.transfer_fields(adata)
-            cls.register_manager(adata_manager)
-        else:
-            adata_manager = orig_adata_manager
-        adata = adata_manager.adata
+        Shape is n_cells x n_labels OR n_cells x (n_labels + 1) if keep_noise.
 
-        if restrict_to_batch is not None:
-            batch_mask = adata.obs[orig_batch_key] == restrict_to_batch
-            if np.sum(batch_mask) == 0:
-                raise ValueError(
-                    "Batch category given to restrict_to_batch not found.\n"
-                    + "Available categories: {}".format(
-                        adata.obs[orig_batch_key].astype("category").cat.categories
-                    )
+        Parameters
+        ----------
+        keep_noise
+            whether to account for the noise term as a standalone cell type in the proportion estimate.
+        indices
+            Indices of cells in adata to use. Only used if amortization. If `None`, all cells are used.
+        batch_size
+            Minibatch size for data loading into model. Only used if amortization. Defaults to `scvi.settings.batch_size`.
+        """
+        self._check_if_trained()
+
+        column_names = self.cell_type_mapping
+        index_names = self.adata.obs.index
+        if keep_noise:
+            column_names = np.append(column_names, "noise_term")
+
+        if self.module.amortization in ["both", "proportion"]:
+            stdl = self._make_data_loader(
+                adata=self.adata, indices=indices, batch_size=batch_size
+            )
+            prop_ = []
+            for tensors in stdl:
+                generative_inputs = self.module._get_generative_input(tensors, None)
+                prop_local = self.module.get_proportions(
+                    x=generative_inputs["x"], keep_noise=keep_noise
                 )
-            # indices in adata with restrict_to_batch category
-            batch_indices = np.where(batch_mask)[0]
+                prop_ += [prop_local.cpu()]
+            data = torch.cat(prop_).numpy()
+            if indices:
+                index_names = index_names[indices]
         else:
-            # use all indices
-            batch_indices = None
+            if indices is not None:
+                logger.info(
+                    "No amortization for proportions, ignoring indices and returning results for the full data"
+                )
+            data = self.module.get_proportions(keep_noise=keep_noise)
 
-        # anndata with only generated doublets
-        doublet_adata = cls.create_doublets(
-            adata_manager, indices=batch_indices, doublet_ratio=doublet_ratio
-        )
-        # if scvi wasn't trained with batch correction having the
-        # zeros here does nothing.
-        doublet_adata.obs[orig_batch_key] = (
-            restrict_to_batch
-            if restrict_to_batch is not None
-            else orig_adata_manager.get_state_registry(
-                REGISTRY_KEYS.BATCH_KEY
-            ).categorical_mapping[0]
+        return pd.DataFrame(
+            data=data,
+            columns=column_names,
+            index=index_names,
         )
 
-        # Create dummy labels column set to first label in adata (does not affect inference).
-        dummy_label = orig_labels_key_registry.categorical_mapping[0]
-        doublet_adata.obs[orig_labels_key] = dummy_label
-
-        # if model is using observed lib size, needs to get lib sample
-        # which is just observed lib size on log scale
-        give_mean_lib = not scvi_model.module.use_observed_lib_size
-
-        # get latent representations and make input anndata
-        latent_rep = scvi_model.get_latent_representation(adata, indices=batch_indices)
-        lib_size = scvi_model.get_latent_library_size(
-            adata, indices=batch_indices, give_mean=give_mean_lib
-        )
-        latent_adata = AnnData(np.concatenate([latent_rep, np.log(lib_size)], axis=1))
-        latent_adata.obs[LABELS_KEY] = "singlet"
-        orig_obs_names = adata.obs_names
-        latent_adata.obs_names = (
-            orig_obs_names[batch_indices]
-            if batch_indices is not None
-            else orig_obs_names
-        )
+    def get_gamma(
+        self,
+        indices: Optional[Sequence[int]] = None,
+        batch_size: Optional[int] = None,
+        return_numpy: bool = False,
+    ) -> Union[np.ndarray, Dict[str, pd.DataFrame]]:
+        """Returns the estimated cell-type specific latent space for the spatial data.
 
-        logger.info("Creating doublets, preparing SOLO model.")
-        f = io.StringIO()
-        with redirect_stdout(f):
-            doublet_latent_rep = scvi_model.get_latent_representation(doublet_adata)
-            doublet_lib_size = scvi_model.get_latent_library_size(
-                doublet_adata, give_mean=give_mean_lib
-            )
-            doublet_adata = AnnData(
-                np.concatenate([doublet_latent_rep, np.log(doublet_lib_size)], axis=1)
+        Parameters
+        ----------
+        indices
+            Indices of cells in adata to use. Only used if amortization. If `None`, all cells are used.
+        batch_size
+            Minibatch size for data loading into model. Only used if amortization. Defaults to `scvi.settings.batch_size`.
+        return_numpy
+            if activated, will return a numpy array of shape is n_spots x n_latent x n_labels.
+        """
+        self._check_if_trained()
+
+        column_names = np.arange(self.module.n_latent)
+        index_names = self.adata.obs.index
+
+        if self.module.amortization in ["both", "latent"]:
+            stdl = self._make_data_loader(
+                adata=self.adata, indices=indices, batch_size=batch_size
             )
-            doublet_adata.obs[LABELS_KEY] = "doublet"
+            gamma_ = []
+            for tensors in stdl:
+                generative_inputs = self.module._get_generative_input(tensors, None)
+                gamma_local = self.module.get_gamma(x=generative_inputs["x"])
+                gamma_ += [gamma_local.cpu()]
+            data = torch.cat(gamma_, dim=-1).numpy()
+            if indices is not None:
+                index_names = index_names[indices]
+        else:
+            if indices is not None:
+                logger.info(
+                    "No amortization for latent values, ignoring adata and returning results for the full data"
+                )
+            data = self.module.get_gamma()
 
-            full_adata = anndata.concat([latent_adata, doublet_adata])
-            cls.setup_anndata(full_adata, labels_key=LABELS_KEY)
-        return cls(full_adata, **classifier_kwargs)
+        data = np.transpose(data, (2, 0, 1))
+        if return_numpy:
+            return data
+        else:
+            res = {}
+            for i, ct in enumerate(self.cell_type_mapping):
+                res[ct] = pd.DataFrame(
+                    data=data[:, :, i], columns=column_names, index=index_names
+                )
+            return res
 
-    @classmethod
-    def create_doublets(
-        cls,
-        adata_manager: AnnDataManager,
-        doublet_ratio: int,
+    def get_scale_for_ct(
+        self,
+        label: str,
         indices: Optional[Sequence[int]] = None,
-        seed: int = 1,
-    ) -> AnnData:
-        """Simulate doublets.
+        batch_size: Optional[int] = None,
+    ) -> pd.DataFrame:
+        r"""Return the scaled parameter of the NB for every spot in queried cell types.
 
         Parameters
         ----------
-        adata
-            AnnData object setup with setup_anndata.
-        doublet_ratio
-            Ratio of generated doublets to produce relative to number of
-            cells in adata or length of indices, if not `None`.
+        label
+            cell type of interest
         indices
-            Indices of cells in adata to use. If `None`, all cells are used.
-        seed
-            Seed for reproducibility
-        """
-        adata = adata_manager.adata
-        n_obs = adata.n_obs if indices is None else len(indices)
-        num_doublets = doublet_ratio * n_obs
+            Indices of cells in self.adata to use. If `None`, all cells are used.
+        batch_size
+            Minibatch size for data loading into model. Defaults to `scvi.settings.batch_size`.
 
-        # counts can be in many locations, this uses where it was registered in setup
-        x = adata_manager.get_from_registry(REGISTRY_KEYS.X_KEY)
-        if indices is not None:
-            x = x[indices]
+        Returns
+        -------
+        Pandas dataframe of gene_expression
+        """
+        self._check_if_trained()
 
-        random_state = np.random.RandomState(seed=seed)
-        parent_inds = random_state.choice(n_obs, size=(num_doublets, 2))
-        doublets = x[parent_inds[:, 0]] + x[parent_inds[:, 1]]
-
-        doublets_ad = AnnData(doublets)
-        doublets_ad.var_names = adata.var_names
-        doublets_ad.obs_names = [f"sim_doublet_{i}" for i in range(num_doublets)]
-
-        # if adata setup with a layer, need to add layer to doublets adata
-        layer = adata_manager.data_registry[REGISTRY_KEYS.X_KEY].attr_key
-        if layer is not None:
-            doublets_ad.layers[layer] = doublets
+        if label not in self.cell_type_mapping:
+            raise ValueError("Unknown cell type")
+        y = np.where(label == self.cell_type_mapping)[0][0]
+
+        stdl = self._make_data_loader(
+            self.adata, indices=indices, batch_size=batch_size
+        )
+        scale = []
+        for tensors in stdl:
+            generative_inputs = self.module._get_generative_input(tensors, None)
+            x, ind_x = (
+                generative_inputs["x"],
+                generative_inputs["ind_x"],
+            )
+            px_scale = self.module.get_ct_specific_expression(x, ind_x, y)
+            scale += [px_scale.cpu()]
 
-        return doublets_ad
+        data = torch.cat(scale).numpy()
+        column_names = self.adata.var.index
+        index_names = self.adata.obs.index
+        if indices is not None:
+            index_names = index_names[indices]
+        return pd.DataFrame(data=data, columns=column_names, index=index_names)
 
     @devices_dsp.dedent
     def train(
         self,
-        max_epochs: int = 400,
-        lr: float = 1e-3,
+        max_epochs: int = 2000,
+        lr: float = 0.003,
         use_gpu: Optional[Union[str, int, bool]] = None,
         accelerator: str = "auto",
         devices: Union[int, List[int], str] = "auto",
-        train_size: float = 0.9,
+        train_size: float = 1.0,
         validation_size: Optional[float] = None,
         shuffle_set_split: bool = True,
         batch_size: int = 128,
+        n_epochs_kl_warmup: int = 200,
         plan_kwargs: Optional[dict] = None,
-        early_stopping: bool = True,
-        early_stopping_patience: int = 30,
-        early_stopping_min_delta: float = 0.0,
         **kwargs,
     ):
-        """Trains the model.
+        """Trains the model using MAP inference.
 
         Parameters
         ----------
         max_epochs
             Number of epochs to train for
         lr
             Learning rate for optimization.
@@ -319,154 +339,63 @@
             Size of the test set. If `None`, defaults to 1 - `train_size`. If
             `train_size + validation_size < 1`, the remaining cells belong to a test set.
         shuffle_set_split
             Whether to shuffle indices before splitting. If `False`, the val, train, and test set are split in the
             sequential order of the data according to `validation_size` and `train_size` percentages.
         batch_size
             Minibatch size to use during training.
+        n_epochs_kl_warmup
+            number of epochs needed to reach unit kl weight in the elbo
         plan_kwargs
-            Keyword args for :class:`~scvi.train.ClassifierTrainingPlan`. Keyword arguments passed to
-        early_stopping
-            Adds callback for early stopping on validation_loss
-        early_stopping_patience
-            Number of times early stopping metric can not improve over early_stopping_min_delta
-        early_stopping_min_delta
-            Threshold for counting an epoch torwards patience
+            Keyword args for :class:`~scvi.train.TrainingPlan`. Keyword arguments passed to
             `train()` will overwrite values present in `plan_kwargs`, when appropriate.
         **kwargs
             Other keyword args for :class:`~scvi.train.Trainer`.
         """
         update_dict = {
             "lr": lr,
+            "n_epochs_kl_warmup": n_epochs_kl_warmup,
         }
         if plan_kwargs is not None:
             plan_kwargs.update(update_dict)
         else:
             plan_kwargs = update_dict
-
-        if early_stopping:
-            early_stopping_callback = [
-                LoudEarlyStopping(
-                    monitor="validation_loss" if train_size != 1.0 else "train_loss",
-                    min_delta=early_stopping_min_delta,
-                    patience=early_stopping_patience,
-                    mode="min",
-                )
-            ]
-            if "callbacks" in kwargs:
-                kwargs["callbacks"] += early_stopping_callback
-            else:
-                kwargs["callbacks"] = early_stopping_callback
-            kwargs["check_val_every_n_epoch"] = 1
-
-        if max_epochs is None:
-            max_epochs = get_max_epochs_heuristic(self.adata.n_obs)
-
-        plan_kwargs = plan_kwargs if isinstance(plan_kwargs, dict) else {}
-
-        data_splitter = DataSplitter(
-            self.adata_manager,
-            train_size=train_size,
-            validation_size=validation_size,
-            shuffle_set_split=shuffle_set_split,
-            batch_size=batch_size,
-        )
-        training_plan = ClassifierTrainingPlan(
-            self.module, self.n_labels, **plan_kwargs
-        )
-        runner = TrainRunner(
-            self,
-            training_plan=training_plan,
-            data_splitter=data_splitter,
+        super().train(
             max_epochs=max_epochs,
             use_gpu=use_gpu,
             accelerator=accelerator,
             devices=devices,
+            train_size=train_size,
+            validation_size=validation_size,
+            shuffle_set_split=shuffle_set_split,
+            batch_size=batch_size,
+            plan_kwargs=plan_kwargs,
             **kwargs,
         )
-        return runner()
-
-    @torch.inference_mode()
-    def predict(
-        self, soft: bool = True, include_simulated_doublets: bool = False
-    ) -> pd.DataFrame:
-        """Return doublet predictions.
-
-        Parameters
-        ----------
-        soft
-            Return probabilities instead of class label
-        include_simulated_doublets
-            Return probabilities for simulated doublets as well.
-
-        Returns
-        -------
-        DataFrame with prediction, index corresponding to cell barcode.
-        """
-        adata = self._validate_anndata(None)
-
-        scdl = self._make_data_loader(
-            adata=adata,
-        )
-
-        @auto_move_data
-        def auto_forward(module, x):
-            return module(x)
-
-        y_pred = []
-        for _, tensors in enumerate(scdl):
-            x = tensors[REGISTRY_KEYS.X_KEY]
-            pred = auto_forward(self.module, x)
-            y_pred.append(pred.cpu())
-
-        y_pred = torch.cat(y_pred).numpy()
-
-        label = self.adata.obs["_solo_doub_sim"].values.ravel()
-        mask = label == "singlet" if not include_simulated_doublets else slice(None)
-
-        preds = y_pred[mask]
-
-        cols = self.adata_manager.get_state_registry(
-            REGISTRY_KEYS.LABELS_KEY
-        ).categorical_mapping
-        preds_df = pd.DataFrame(preds, columns=cols, index=self.adata.obs_names[mask])
-
-        if not soft:
-            preds_df = preds_df.idxmax(axis=1)
-
-        return preds_df
 
     @classmethod
     @setup_anndata_dsp.dedent
     def setup_anndata(
         cls,
         adata: AnnData,
-        labels_key: Optional[str] = None,
         layer: Optional[str] = None,
         **kwargs,
     ):
         """%(summary)s.
 
         Parameters
         ----------
-        %(param_labels_key)s
+        %(param_adata)s
         %(param_layer)s
         """
         setup_method_args = cls._get_setup_method_args(**locals())
+        # add index for each cell (provided to pyro plate for correct minibatching)
+        adata.obs["_indices"] = np.arange(adata.n_obs)
         anndata_fields = [
-            LayerField(REGISTRY_KEYS.X_KEY, layer, is_count_data=False),
-            CategoricalObsField(REGISTRY_KEYS.LABELS_KEY, labels_key),
+            LayerField(REGISTRY_KEYS.X_KEY, layer, is_count_data=True),
+            NumericalObsField(REGISTRY_KEYS.INDICES_KEY, "_indices"),
         ]
         adata_manager = AnnDataManager(
             fields=anndata_fields, setup_method_args=setup_method_args
         )
         adata_manager.register_fields(adata, **kwargs)
         cls.register_manager(adata_manager)
-
-
-def _validate_scvi_model(scvi_model: SCVI, restrict_to_batch: str):
-    if scvi_model.summary_stats.n_batch > 1 and restrict_to_batch is None:
-        warnings.warn(
-            "Solo should only be trained on one lane of data using `restrict_to_batch`. Performance may suffer.",
-            UserWarning,
-            stacklevel=settings.warnings_stacklevel,
-        )
```

### Comparing `scvi_tools-1.0.0/scvi/external/stereoscope/_model.py` & `scvi_tools-1.0.0b0/scvi/external/stereoscope/_model.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/external/stereoscope/_module.py` & `scvi_tools-1.0.0b0/scvi/external/stereoscope/_module.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/external/tangram/_model.py` & `scvi_tools-1.0.0b0/scvi/external/tangram/_model.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/external/tangram/_module.py` & `scvi_tools-1.0.0b0/scvi/external/tangram/_module.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/hub/_constants.py` & `scvi_tools-1.0.0b0/scvi/hub/_constants.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/hub/_url.py` & `scvi_tools-1.0.0b0/scvi/hub/_url.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/hub/hub_metadata.py` & `scvi_tools-1.0.0b0/scvi/hub/hub_metadata.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/hub/hub_model.py` & `scvi_tools-1.0.0b0/scvi/hub/hub_model.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/hub/model_card_template.py` & `scvi_tools-1.0.0b0/scvi/hub/model_card_template.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/model/__init__.py` & `scvi_tools-1.0.0b0/scvi/model/__init__.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/model/_amortizedlda.py` & `scvi_tools-1.0.0b0/scvi/model/_amortizedlda.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/model/_autozi.py` & `scvi_tools-1.0.0b0/scvi/model/_autozi.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/model/_condscvi.py` & `scvi_tools-1.0.0b0/scvi/model/_condscvi.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/model/_destvi.py` & `scvi_tools-1.0.0b0/scvi/module/_scanvae.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,401 +1,362 @@
-import logging
-from collections import OrderedDict
-from typing import Dict, List, Optional, Sequence, Union
+from typing import Iterable, Literal, Optional, Sequence
 
 import numpy as np
-import pandas as pd
 import torch
-from anndata import AnnData
+from torch.distributions import Categorical, Normal
+from torch.distributions import kl_divergence as kl
+from torch.nn import functional as F
 
 from scvi import REGISTRY_KEYS
-from scvi.data import AnnDataManager
-from scvi.data.fields import LayerField, NumericalObsField
-from scvi.model import CondSCVI
-from scvi.model.base import BaseModelClass, UnsupervisedTrainingMixin
-from scvi.module import MRDeconv
-from scvi.utils import setup_anndata_dsp
-from scvi.utils._docstrings import devices_dsp
+from scvi.autotune._types import Tunable
+from scvi.module.base import LossOutput, auto_move_data
+from scvi.nn import Decoder, Encoder
 
-logger = logging.getLogger(__name__)
+from ._classifier import Classifier
+from ._utils import broadcast_labels
+from ._vae import VAE
 
 
-class DestVI(UnsupervisedTrainingMixin, BaseModelClass):
-    """Multi-resolution deconvolution of Spatial Transcriptomics data (DestVI) :cite:p:`Lopez21`. Most users will use the alternate constructor (see example).
+class SCANVAE(VAE):
+    """Single-cell annotation using variational inference.
+
+    This is an implementation of the scANVI model described in :cite:p:`Xu21`,
+    inspired from M1 + M2 model, as described in (https://arxiv.org/pdf/1406.5298.pdf).
 
     Parameters
     ----------
-    st_adata
-        spatial transcriptomics AnnData object that has been registered via :meth:`~scvi.model.DestVI.setup_anndata`.
-    cell_type_mapping
-        mapping between numerals and cell type labels
-    decoder_state_dict
-        state_dict from the decoder of the CondSCVI model
-    px_decoder_state_dict
-        state_dict from the px_decoder of the CondSCVI model
-    px_r
-        parameters for the px_r tensor in the CondSCVI model
+    n_input
+        Number of input genes
+    n_batch
+        Number of batches
+    n_labels
+        Number of labels
     n_hidden
-        Number of nodes per hidden layer.
+        Number of nodes per hidden layer
     n_latent
-        Dimensionality of the latent space.
+        Dimensionality of the latent space
     n_layers
-        Number of hidden layers used for encoder and decoder NNs.
-    **module_kwargs
-        Keyword args for :class:`~scvi.modules.MRDeconv`
-
-    Examples
-    --------
-    >>> sc_adata = anndata.read_h5ad(path_to_scRNA_anndata)
-    >>> scvi.model.CondSCVI.setup_anndata(sc_adata)
-    >>> sc_model = scvi.model.CondSCVI(sc_adata)
-    >>> st_adata = anndata.read_h5ad(path_to_ST_anndata)
-    >>> DestVI.setup_anndata(st_adata)
-    >>> spatial_model = DestVI.from_rna_model(st_adata, sc_model)
-    >>> spatial_model.train(max_epochs=2000)
-    >>> st_adata.obsm["proportions"] = spatial_model.get_proportions(st_adata)
-    >>> gamma = spatial_model.get_gamma(st_adata)
-
-    Notes
-    -----
-    See further usage examples in the following tutorials:
-
-    1. :doc:`/tutorials/notebooks/DestVI_tutorial`
+        Number of hidden layers used for encoder and decoder NNs
+    n_continuous_cov
+        Number of continuous covarites
+    n_cats_per_cov
+        Number of categories for each extra categorical covariate
+    dropout_rate
+        Dropout rate for neural networks
+    dispersion
+        One of the following
+
+        * ``'gene'`` - dispersion parameter of NB is constant per gene across cells
+        * ``'gene-batch'`` - dispersion can differ between different batches
+        * ``'gene-label'`` - dispersion can differ between different labels
+        * ``'gene-cell'`` - dispersion can differ for every gene in every cell
+    log_variational
+        Log(data+1) prior to encoding for numerical stability. Not normalization.
+    gene_likelihood
+        One of:
+
+        * ``'nb'`` - Negative binomial distribution
+        * ``'zinb'`` - Zero-inflated negative binomial distribution
+    y_prior
+        If None, initialized to uniform probability over cell types
+    labels_groups
+        Label group designations
+    use_labels_groups
+        Whether to use the label groups
+    use_batch_norm
+        Whether to use batch norm in layers
+    use_layer_norm
+        Whether to use layer norm in layers
+    **vae_kwargs
+        Keyword args for :class:`~scvi.module.VAE`
     """
 
-    _module_cls = MRDeconv
-
     def __init__(
         self,
-        st_adata: AnnData,
-        cell_type_mapping: np.ndarray,
-        decoder_state_dict: OrderedDict,
-        px_decoder_state_dict: OrderedDict,
-        px_r: np.ndarray,
-        n_hidden: int,
-        n_latent: int,
-        n_layers: int,
-        dropout_decoder: float,
-        l1_reg: float,
-        **module_kwargs,
+        n_input: int,
+        n_batch: int = 0,
+        n_labels: int = 0,
+        n_hidden: Tunable[int] = 128,
+        n_latent: Tunable[int] = 10,
+        n_layers: Tunable[int] = 1,
+        n_continuous_cov: int = 0,
+        n_cats_per_cov: Optional[Iterable[int]] = None,
+        dropout_rate: Tunable[float] = 0.1,
+        dispersion: Tunable[
+            Literal["gene", "gene-batch", "gene-label", "gene-cell"]
+        ] = "gene",
+        log_variational: Tunable[bool] = True,
+        gene_likelihood: Tunable[Literal["zinb", "nb"]] = "zinb",
+        y_prior=None,
+        labels_groups: Sequence[int] = None,
+        use_labels_groups: bool = False,
+        classifier_parameters: Optional[dict] = None,
+        use_batch_norm: Tunable[Literal["encoder", "decoder", "none", "both"]] = "both",
+        use_layer_norm: Tunable[Literal["encoder", "decoder", "none", "both"]] = "none",
+        **vae_kwargs,
     ):
-        super().__init__(st_adata)
-        self.module = self._module_cls(
-            n_spots=st_adata.n_obs,
-            n_labels=cell_type_mapping.shape[0],
-            decoder_state_dict=decoder_state_dict,
-            px_decoder_state_dict=px_decoder_state_dict,
-            px_r=px_r,
-            n_genes=st_adata.n_vars,
+        super().__init__(
+            n_input,
+            n_hidden=n_hidden,
             n_latent=n_latent,
             n_layers=n_layers,
+            n_continuous_cov=n_continuous_cov,
+            n_cats_per_cov=n_cats_per_cov,
+            dropout_rate=dropout_rate,
+            n_batch=n_batch,
+            dispersion=dispersion,
+            log_variational=log_variational,
+            gene_likelihood=gene_likelihood,
+            use_batch_norm=use_batch_norm,
+            use_layer_norm=use_layer_norm,
+            **vae_kwargs,
+        )
+
+        classifier_parameters = classifier_parameters or {}
+        use_batch_norm_encoder = use_batch_norm == "encoder" or use_batch_norm == "both"
+        use_batch_norm_decoder = use_batch_norm == "decoder" or use_batch_norm == "both"
+        use_layer_norm_encoder = use_layer_norm == "encoder" or use_layer_norm == "both"
+        use_layer_norm_decoder = use_layer_norm == "decoder" or use_layer_norm == "both"
+
+        self.n_labels = n_labels
+        # Classifier takes n_latent as input
+        cls_parameters = {
+            "n_layers": n_layers,
+            "n_hidden": n_hidden,
+            "dropout_rate": dropout_rate,
+        }
+        cls_parameters.update(classifier_parameters)
+        self.classifier = Classifier(
+            n_latent,
+            n_labels=n_labels,
+            use_batch_norm=use_batch_norm_encoder,
+            use_layer_norm=use_layer_norm_encoder,
+            **cls_parameters,
+        )
+
+        self.encoder_z2_z1 = Encoder(
+            n_latent,
+            n_latent,
+            n_cat_list=[self.n_labels],
+            n_layers=n_layers,
             n_hidden=n_hidden,
-            dropout_decoder=dropout_decoder,
-            l1_reg=l1_reg,
-            **module_kwargs,
-        )
-        self.cell_type_mapping = cell_type_mapping
-        self._model_summary_string = "DestVI Model"
-        self.init_params_ = self._get_init_params(locals())
-
-    @classmethod
-    def from_rna_model(
-        cls,
-        st_adata: AnnData,
-        sc_model: CondSCVI,
-        vamp_prior_p: int = 15,
-        l1_reg: float = 0.0,
-        **module_kwargs,
-    ):
-        """Alternate constructor for exploiting a pre-trained model on a RNA-seq dataset.
+            dropout_rate=dropout_rate,
+            use_batch_norm=use_batch_norm_encoder,
+            use_layer_norm=use_layer_norm_encoder,
+            return_dist=True,
+        )
 
-        Parameters
-        ----------
-        st_adata
-            registered anndata object
-        sc_model
-            trained CondSCVI model
-        vamp_prior_p
-            number of mixture parameter for VampPrior calculations
-        l1_reg
-            Scalar parameter indicating the strength of L1 regularization on cell type proportions.
-            A value of 50 leads to sparser results.
-        **model_kwargs
-            Keyword args for :class:`~scvi.model.DestVI`
-        """
-        decoder_state_dict = sc_model.module.decoder.state_dict()
-        px_decoder_state_dict = sc_model.module.px_decoder.state_dict()
-        px_r = sc_model.module.px_r.detach().cpu().numpy()
-        mapping = sc_model.adata_manager.get_state_registry(
-            REGISTRY_KEYS.LABELS_KEY
-        ).categorical_mapping
-        dropout_decoder = sc_model.module.dropout_rate
-        if vamp_prior_p is None:
-            mean_vprior = None
-            var_vprior = None
-        else:
-            mean_vprior, var_vprior, mp_vprior = sc_model.get_vamp_prior(
-                sc_model.adata, p=vamp_prior_p
-            )
+        self.decoder_z1_z2 = Decoder(
+            n_latent,
+            n_latent,
+            n_cat_list=[self.n_labels],
+            n_layers=n_layers,
+            n_hidden=n_hidden,
+            use_batch_norm=use_batch_norm_decoder,
+            use_layer_norm=use_layer_norm_decoder,
+        )
 
-        return cls(
-            st_adata,
-            mapping,
-            decoder_state_dict,
-            px_decoder_state_dict,
-            px_r,
-            sc_model.module.n_hidden,
-            sc_model.module.n_latent,
-            sc_model.module.n_layers,
-            mean_vprior=mean_vprior,
-            var_vprior=var_vprior,
-            mp_vprior=mp_vprior,
-            dropout_decoder=dropout_decoder,
-            l1_reg=l1_reg,
-            **module_kwargs,
+        self.y_prior = torch.nn.Parameter(
+            y_prior
+            if y_prior is not None
+            else (1 / n_labels) * torch.ones(1, n_labels),
+            requires_grad=False,
+        )
+        self.use_labels_groups = use_labels_groups
+        self.labels_groups = (
+            np.array(labels_groups) if labels_groups is not None else None
         )
+        if self.use_labels_groups:
+            if labels_groups is None:
+                raise ValueError("Specify label groups")
+            unique_groups = np.unique(self.labels_groups)
+            self.n_groups = len(unique_groups)
+            if not (unique_groups == np.arange(self.n_groups)).all():
+                raise ValueError()
+            self.classifier_groups = Classifier(
+                n_latent, n_hidden, self.n_groups, n_layers, dropout_rate
+            )
+            self.groups_index = torch.nn.ParameterList(
+                [
+                    torch.nn.Parameter(
+                        torch.tensor(
+                            (self.labels_groups == i).astype(np.uint8),
+                            dtype=torch.uint8,
+                        ),
+                        requires_grad=False,
+                    )
+                    for i in range(self.n_groups)
+                ]
+            )
 
-    def get_proportions(
+    @auto_move_data
+    def classify(
         self,
-        keep_noise: bool = False,
-        indices: Optional[Sequence[int]] = None,
-        batch_size: Optional[int] = None,
-    ) -> pd.DataFrame:
-        """Returns the estimated cell type proportion for the spatial data.
-
-        Shape is n_cells x n_labels OR n_cells x (n_labels + 1) if keep_noise.
-
-        Parameters
-        ----------
-        keep_noise
-            whether to account for the noise term as a standalone cell type in the proportion estimate.
-        indices
-            Indices of cells in adata to use. Only used if amortization. If `None`, all cells are used.
-        batch_size
-            Minibatch size for data loading into model. Only used if amortization. Defaults to `scvi.settings.batch_size`.
-        """
-        self._check_if_trained()
-
-        column_names = self.cell_type_mapping
-        index_names = self.adata.obs.index
-        if keep_noise:
-            column_names = np.append(column_names, "noise_term")
-
-        if self.module.amortization in ["both", "proportion"]:
-            stdl = self._make_data_loader(
-                adata=self.adata, indices=indices, batch_size=batch_size
-            )
-            prop_ = []
-            for tensors in stdl:
-                generative_inputs = self.module._get_generative_input(tensors, None)
-                prop_local = self.module.get_proportions(
-                    x=generative_inputs["x"], keep_noise=keep_noise
-                )
-                prop_ += [prop_local.cpu()]
-            data = torch.cat(prop_).numpy()
-            if indices:
-                index_names = index_names[indices]
+        x: torch.Tensor,
+        batch_index: Optional[torch.Tensor] = None,
+        cont_covs: Optional[torch.Tensor] = None,
+        cat_covs: Optional[torch.Tensor] = None,
+    ) -> torch.Tensor:
+        """Classify cells into cell types."""
+        if self.log_variational:
+            x = torch.log(1 + x)
+
+        if cont_covs is not None and self.encode_covariates:
+            encoder_input = torch.cat((x, cont_covs), dim=-1)
         else:
-            if indices is not None:
-                logger.info(
-                    "No amortization for proportions, ignoring indices and returning results for the full data"
+            encoder_input = x
+        if cat_covs is not None and self.encode_covariates:
+            categorical_input = torch.split(cat_covs, 1, dim=1)
+        else:
+            categorical_input = ()
+
+        qz, z = self.z_encoder(encoder_input, batch_index, *categorical_input)
+        # We classify using the inferred mean parameter of z_1 in the latent space
+        z = qz.loc
+        if self.use_labels_groups:
+            w_g = self.classifier_groups(z)
+            unw_y = self.classifier(z)
+            w_y = torch.zeros_like(unw_y)
+            for i, group_index in enumerate(self.groups_index):
+                unw_y_g = unw_y[:, group_index]
+                w_y[:, group_index] = unw_y_g / (
+                    unw_y_g.sum(dim=-1, keepdim=True) + 1e-8
                 )
-            data = self.module.get_proportions(keep_noise=keep_noise)
+                w_y[:, group_index] *= w_g[:, [i]]
+        else:
+            w_y = self.classifier(z)
+        return w_y
 
-        return pd.DataFrame(
-            data=data,
-            columns=column_names,
-            index=index_names,
+    @auto_move_data
+    def classification_loss(self, labelled_dataset):
+        x = labelled_dataset[REGISTRY_KEYS.X_KEY]  # (n_obs, n_vars)
+        y = labelled_dataset[REGISTRY_KEYS.LABELS_KEY]  # (n_obs, 1)
+        batch_idx = labelled_dataset[REGISTRY_KEYS.BATCH_KEY]
+        cont_key = REGISTRY_KEYS.CONT_COVS_KEY
+        cont_covs = (
+            labelled_dataset[cont_key] if cont_key in labelled_dataset.keys() else None
+        )
+
+        cat_key = REGISTRY_KEYS.CAT_COVS_KEY
+        cat_covs = (
+            labelled_dataset[cat_key] if cat_key in labelled_dataset.keys() else None
+        )
+        logits = self.classify(
+            x, batch_index=batch_idx, cat_covs=cat_covs, cont_covs=cont_covs
+        )  # (n_obs, n_labels)
+        ce_loss = F.cross_entropy(
+            logits,
+            y.view(-1).long(),
         )
+        return ce_loss, y, logits
 
-    def get_gamma(
+    def loss(
         self,
-        indices: Optional[Sequence[int]] = None,
-        batch_size: Optional[int] = None,
-        return_numpy: bool = False,
-    ) -> Union[np.ndarray, Dict[str, pd.DataFrame]]:
-        """Returns the estimated cell-type specific latent space for the spatial data.
-
-        Parameters
-        ----------
-        indices
-            Indices of cells in adata to use. Only used if amortization. If `None`, all cells are used.
-        batch_size
-            Minibatch size for data loading into model. Only used if amortization. Defaults to `scvi.settings.batch_size`.
-        return_numpy
-            if activated, will return a numpy array of shape is n_spots x n_latent x n_labels.
-        """
-        self._check_if_trained()
-
-        column_names = np.arange(self.module.n_latent)
-        index_names = self.adata.obs.index
-
-        if self.module.amortization in ["both", "latent"]:
-            stdl = self._make_data_loader(
-                adata=self.adata, indices=indices, batch_size=batch_size
-            )
-            gamma_ = []
-            for tensors in stdl:
-                generative_inputs = self.module._get_generative_input(tensors, None)
-                gamma_local = self.module.get_gamma(x=generative_inputs["x"])
-                gamma_ += [gamma_local.cpu()]
-            data = torch.cat(gamma_, dim=-1).numpy()
-            if indices is not None:
-                index_names = index_names[indices]
+        tensors,
+        inference_outputs,
+        generative_ouputs,
+        feed_labels=False,
+        kl_weight=1,
+        labelled_tensors=None,
+        classification_ratio=None,
+    ):
+        """Compute the loss."""
+        px = generative_ouputs["px"]
+        qz1 = inference_outputs["qz"]
+        z1 = inference_outputs["z"]
+        x = tensors[REGISTRY_KEYS.X_KEY]
+        batch_index = tensors[REGISTRY_KEYS.BATCH_KEY]
+
+        if feed_labels:
+            y = tensors[REGISTRY_KEYS.LABELS_KEY]
         else:
-            if indices is not None:
-                logger.info(
-                    "No amortization for latent values, ignoring adata and returning results for the full data"
-                )
-            data = self.module.get_gamma()
+            y = None
+        is_labelled = False if y is None else True
 
-        data = np.transpose(data, (2, 0, 1))
-        if return_numpy:
-            return data
+        # Enumerate choices of label
+        ys, z1s = broadcast_labels(y, z1, n_broadcast=self.n_labels)
+        qz2, z2 = self.encoder_z2_z1(z1s, ys)
+        pz1_m, pz1_v = self.decoder_z1_z2(z2, ys)
+        reconst_loss = -px.log_prob(x).sum(-1)
+
+        # KL Divergence
+        mean = torch.zeros_like(qz2.loc)
+        scale = torch.ones_like(qz2.scale)
+
+        kl_divergence_z2 = kl(qz2, Normal(mean, scale)).sum(dim=1)
+        loss_z1_unweight = -Normal(pz1_m, torch.sqrt(pz1_v)).log_prob(z1s).sum(dim=-1)
+        loss_z1_weight = qz1.log_prob(z1).sum(dim=-1)
+        if not self.use_observed_lib_size:
+            ql = inference_outputs["ql"]
+            (
+                local_library_log_means,
+                local_library_log_vars,
+            ) = self._compute_local_library_params(batch_index)
+
+            kl_divergence_l = kl(
+                ql,
+                Normal(local_library_log_means, torch.sqrt(local_library_log_vars)),
+            ).sum(dim=1)
         else:
-            res = {}
-            for i, ct in enumerate(self.cell_type_mapping):
-                res[ct] = pd.DataFrame(
-                    data=data[:, :, i], columns=column_names, index=index_names
-                )
-            return res
+            kl_divergence_l = 0.0
 
-    def get_scale_for_ct(
-        self,
-        label: str,
-        indices: Optional[Sequence[int]] = None,
-        batch_size: Optional[int] = None,
-    ) -> pd.DataFrame:
-        r"""Return the scaled parameter of the NB for every spot in queried cell types.
-
-        Parameters
-        ----------
-        label
-            cell type of interest
-        indices
-            Indices of cells in self.adata to use. If `None`, all cells are used.
-        batch_size
-            Minibatch size for data loading into model. Defaults to `scvi.settings.batch_size`.
-
-        Returns
-        -------
-        Pandas dataframe of gene_expression
-        """
-        self._check_if_trained()
-
-        if label not in self.cell_type_mapping:
-            raise ValueError("Unknown cell type")
-        y = np.where(label == self.cell_type_mapping)[0][0]
-
-        stdl = self._make_data_loader(
-            self.adata, indices=indices, batch_size=batch_size
-        )
-        scale = []
-        for tensors in stdl:
-            generative_inputs = self.module._get_generative_input(tensors, None)
-            x, ind_x = (
-                generative_inputs["x"],
-                generative_inputs["ind_x"],
+        if is_labelled:
+            loss = reconst_loss + loss_z1_weight + loss_z1_unweight
+            kl_locals = {
+                "kl_divergence_z2": kl_divergence_z2,
+                "kl_divergence_l": kl_divergence_l,
+            }
+            if labelled_tensors is not None:
+                ce_loss, true_labels, logits = self.classification_loss(
+                    labelled_tensors
+                )
+                loss += ce_loss * classification_ratio
+                return LossOutput(
+                    loss=loss,
+                    reconstruction_loss=reconst_loss,
+                    kl_local=kl_locals,
+                    classification_loss=ce_loss,
+                    true_labels=true_labels,
+                    logits=logits,
+                    extra_metrics={
+                        "n_labelled_tensors": labelled_tensors[
+                            REGISTRY_KEYS.X_KEY
+                        ].shape[0],
+                    },
+                )
+            return LossOutput(
+                loss=loss,
+                reconstruction_loss=reconst_loss,
+                kl_local=kl_locals,
             )
-            px_scale = self.module.get_ct_specific_expression(x, ind_x, y)
-            scale += [px_scale.cpu()]
 
-        data = torch.cat(scale).numpy()
-        column_names = self.adata.var.index
-        index_names = self.adata.obs.index
-        if indices is not None:
-            index_names = index_names[indices]
-        return pd.DataFrame(data=data, columns=column_names, index=index_names)
+        probs = self.classifier(z1)
+        reconst_loss += loss_z1_weight + (
+            (loss_z1_unweight).view(self.n_labels, -1).t() * probs
+        ).sum(dim=1)
 
-    @devices_dsp.dedent
-    def train(
-        self,
-        max_epochs: int = 2000,
-        lr: float = 0.003,
-        use_gpu: Optional[Union[str, int, bool]] = None,
-        accelerator: str = "auto",
-        devices: Union[int, List[int], str] = "auto",
-        train_size: float = 1.0,
-        validation_size: Optional[float] = None,
-        shuffle_set_split: bool = True,
-        batch_size: int = 128,
-        n_epochs_kl_warmup: int = 200,
-        plan_kwargs: Optional[dict] = None,
-        **kwargs,
-    ):
-        """Trains the model using MAP inference.
+        kl_divergence = (kl_divergence_z2.view(self.n_labels, -1).t() * probs).sum(
+            dim=1
+        )
+        kl_divergence += kl(
+            Categorical(probs=probs),
+            Categorical(probs=self.y_prior.repeat(probs.size(0), 1)),
+        )
+        kl_divergence += kl_divergence_l
 
-        Parameters
-        ----------
-        max_epochs
-            Number of epochs to train for
-        lr
-            Learning rate for optimization.
-        %(param_use_gpu)s
-        %(param_accelerator)s
-        %(param_devices)s
-        train_size
-            Size of training set in the range [0.0, 1.0].
-        validation_size
-            Size of the test set. If `None`, defaults to 1 - `train_size`. If
-            `train_size + validation_size < 1`, the remaining cells belong to a test set.
-        shuffle_set_split
-            Whether to shuffle indices before splitting. If `False`, the val, train, and test set are split in the
-            sequential order of the data according to `validation_size` and `train_size` percentages.
-        batch_size
-            Minibatch size to use during training.
-        n_epochs_kl_warmup
-            number of epochs needed to reach unit kl weight in the elbo
-        plan_kwargs
-            Keyword args for :class:`~scvi.train.TrainingPlan`. Keyword arguments passed to
-            `train()` will overwrite values present in `plan_kwargs`, when appropriate.
-        **kwargs
-            Other keyword args for :class:`~scvi.train.Trainer`.
-        """
-        update_dict = {
-            "lr": lr,
-            "n_epochs_kl_warmup": n_epochs_kl_warmup,
-        }
-        if plan_kwargs is not None:
-            plan_kwargs.update(update_dict)
-        else:
-            plan_kwargs = update_dict
-        super().train(
-            max_epochs=max_epochs,
-            use_gpu=use_gpu,
-            accelerator=accelerator,
-            devices=devices,
-            train_size=train_size,
-            validation_size=validation_size,
-            shuffle_set_split=shuffle_set_split,
-            batch_size=batch_size,
-            plan_kwargs=plan_kwargs,
-            **kwargs,
-        )
-
-    @classmethod
-    @setup_anndata_dsp.dedent
-    def setup_anndata(
-        cls,
-        adata: AnnData,
-        layer: Optional[str] = None,
-        **kwargs,
-    ):
-        """%(summary)s.
+        loss = torch.mean(reconst_loss + kl_divergence * kl_weight)
 
-        Parameters
-        ----------
-        %(param_adata)s
-        %(param_layer)s
-        """
-        setup_method_args = cls._get_setup_method_args(**locals())
-        # add index for each cell (provided to pyro plate for correct minibatching)
-        adata.obs["_indices"] = np.arange(adata.n_obs)
-        anndata_fields = [
-            LayerField(REGISTRY_KEYS.X_KEY, layer, is_count_data=True),
-            NumericalObsField(REGISTRY_KEYS.INDICES_KEY, "_indices"),
-        ]
-        adata_manager = AnnDataManager(
-            fields=anndata_fields, setup_method_args=setup_method_args
+        if labelled_tensors is not None:
+            ce_loss, true_labels, logits = self.classification_loss(labelled_tensors)
+
+            loss += ce_loss * classification_ratio
+            return LossOutput(
+                loss=loss,
+                reconstruction_loss=reconst_loss,
+                kl_local=kl_divergence,
+                classification_loss=ce_loss,
+                true_labels=true_labels,
+                logits=logits,
+            )
+        return LossOutput(
+            loss=loss, reconstruction_loss=reconst_loss, kl_local=kl_divergence
         )
-        adata_manager.register_fields(adata, **kwargs)
-        cls.register_manager(adata_manager)
```

### Comparing `scvi_tools-1.0.0/scvi/model/_jaxscvi.py` & `scvi_tools-1.0.0b0/scvi/model/_jaxscvi.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     **model_kwargs
         Keyword args for :class:`~scvi.module.JaxVAE`
 
     Examples
     --------
     >>> adata = anndata.read_h5ad(path_to_anndata)
     >>> scvi.model.JaxSCVI.setup_anndata(adata, batch_key="batch")
-    >>> vae = scvi.model.JaxSCVI(adata)
+    >>> vae = scvi.model.SCVI(adata)
     >>> vae.train()
     >>> adata.obsm["X_scVI"] = vae.get_latent_representation()
     """
 
     _module_cls = JaxVAE
 
     def __init__(
```

### Comparing `scvi_tools-1.0.0/scvi/model/_linear_scvi.py` & `scvi_tools-1.0.0b0/scvi/model/_linear_scvi.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/model/_metrics.py` & `scvi_tools-1.0.0b0/scvi/model/_metrics.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/model/_multivi.py` & `scvi_tools-1.0.0b0/scvi/model/_multivi.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/model/_peakvi.py` & `scvi_tools-1.0.0b0/scvi/model/_peakvi.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/model/_scanvi.py` & `scvi_tools-1.0.0b0/scvi/model/_scanvi.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     LayerField,
     NumericalJointObsField,
     NumericalObsField,
     ObsmField,
     StringUnsField,
 )
 from scvi.dataloaders import SemiSupervisedDataSplitter
-from scvi.model._utils import _init_library_size, get_max_epochs_heuristic
+from scvi.model._utils import _init_library_size
 from scvi.model.utils import get_minified_adata_scrna
 from scvi.module import SCANVAE
 from scvi.train import SemiSupervisedTrainingPlan, TrainRunner
 from scvi.train._callbacks import SubSampleLabels
 from scvi.utils import setup_anndata_dsp
 from scvi.utils._docstrings import devices_dsp
 
@@ -73,17 +73,14 @@
         * ``'gene-cell'`` - dispersion can differ for every gene in every cell
     gene_likelihood
         One of:
 
         * ``'nb'`` - Negative binomial distribution
         * ``'zinb'`` - Zero-inflated negative binomial distribution
         * ``'poisson'`` - Poisson distribution
-    linear_classifier
-        If `True`, uses a single linear layer for classification instead of a
-        multi-layer perceptron.
     **model_kwargs
         Keyword args for :class:`~scvi.module.SCANVAE`
 
     Examples
     --------
     >>> adata = anndata.read_h5ad(path_to_anndata)
     >>> scvi.model.SCANVI.setup_anndata(adata, batch_key="batch", labels_key="labels")
@@ -98,26 +95,24 @@
 
     1. :doc:`/tutorials/notebooks/harmonization`
     2. :doc:`/tutorials/notebooks/scarches_scvi_tools`
     3. :doc:`/tutorials/notebooks/seed_labeling`
     """
 
     _module_cls = SCANVAE
-    _training_plan_cls = SemiSupervisedTrainingPlan
 
     def __init__(
         self,
         adata: AnnData,
         n_hidden: int = 128,
         n_latent: int = 10,
         n_layers: int = 1,
         dropout_rate: float = 0.1,
         dispersion: Literal["gene", "gene-batch", "gene-label", "gene-cell"] = "gene",
         gene_likelihood: Literal["zinb", "nb", "poisson"] = "zinb",
-        linear_classifier: bool = False,
         **model_kwargs,
     ):
         super().__init__(adata)
         scanvae_model_kwargs = dict(model_kwargs)
 
         self._set_indices_and_labels()
 
@@ -152,15 +147,14 @@
             n_layers=n_layers,
             dropout_rate=dropout_rate,
             dispersion=dispersion,
             gene_likelihood=gene_likelihood,
             use_size_factor_key=use_size_factor_key,
             library_log_means=library_log_means,
             library_log_vars=library_log_vars,
-            linear_classifier=linear_classifier,
             **scanvae_model_kwargs,
         )
         self.module.minified_data_type = self.minified_data_type
 
         self.unsupervised_history_ = None
         self.semisupervised_history_ = None
 
@@ -391,15 +385,16 @@
         plan_kwargs
             Keyword args for :class:`~scvi.train.SemiSupervisedTrainingPlan`. Keyword arguments passed to
             `train()` will overwrite values present in `plan_kwargs`, when appropriate.
         **trainer_kwargs
             Other keyword args for :class:`~scvi.train.Trainer`.
         """
         if max_epochs is None:
-            max_epochs = get_max_epochs_heuristic(self.adata.n_obs)
+            n_cells = self.adata.n_obs
+            max_epochs = int(np.min([round((20000 / n_cells) * 400), 400]))
 
             if self.was_pretrained:
                 max_epochs = int(np.min([10, np.max([2, round(max_epochs / 3.0)])]))
 
         logger.info(f"Training for {max_epochs} epochs.")
 
         plan_kwargs = {} if plan_kwargs is None else plan_kwargs
@@ -413,15 +408,15 @@
             adata_manager=self.adata_manager,
             train_size=train_size,
             validation_size=validation_size,
             shuffle_set_split=shuffle_set_split,
             n_samples_per_label=n_samples_per_label,
             batch_size=batch_size,
         )
-        training_plan = self._training_plan_cls(
+        training_plan = SemiSupervisedTrainingPlan(
             self.module, self.n_labels, **plan_kwargs
         )
         if "callbacks" in trainer_kwargs.keys():
             trainer_kwargs["callbacks"].concatenate(sampler_callback)
         else:
             trainer_kwargs["callbacks"] = sampler_callback
```

### Comparing `scvi_tools-1.0.0/scvi/model/_scvi.py` & `scvi_tools-1.0.0b0/scvi/model/_scvi.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/model/_totalvi.py` & `scvi_tools-1.0.0b0/scvi/model/_totalvi.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from scvi.data._utils import _check_nonnegative_integers
 from scvi.dataloaders import DataSplitter
 from scvi.model._utils import (
     _get_batch_code_from_category,
     _get_var_names_from_manager,
     _init_library_size,
     cite_seq_raw_counts_properties,
-    get_max_epochs_heuristic,
 )
 from scvi.model.base._utils import _de_core
 from scvi.module import TOTALVAE
 from scvi.train import AdversarialTrainingPlan, TrainRunner
 from scvi.utils._docstrings import de_dsp, devices_dsp, setup_anndata_dsp
 
 from .base import ArchesMixin, BaseModelClass, RNASeqMixin, VAEMixin
@@ -278,15 +277,16 @@
         }
         if plan_kwargs is not None:
             plan_kwargs.update(update_dict)
         else:
             plan_kwargs = update_dict
 
         if max_epochs is None:
-            max_epochs = get_max_epochs_heuristic(self.adata.n_obs)
+            n_cells = self.adata.n_obs
+            max_epochs = int(np.min([round((20000 / n_cells) * 400), 400]))
 
         plan_kwargs = plan_kwargs if isinstance(plan_kwargs, dict) else {}
 
         data_splitter = self._data_splitter_cls(
             self.adata_manager,
             train_size=train_size,
             validation_size=validation_size,
```

### Comparing `scvi_tools-1.0.0/scvi/model/_utils.py` & `scvi_tools-1.0.0b0/scvi/model/_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,52 +16,14 @@
 from scvi.data import AnnDataManager
 from scvi.utils._docstrings import devices_dsp
 from scvi.utils._exceptions import InvalidParameterError
 
 logger = logging.getLogger(__name__)
 
 
-def get_max_epochs_heuristic(
-    n_obs: int, epochs_cap: int = 400, decay_at_n_obs: int = 20000
-) -> int:
-    """Compute a heuristic for the default number of maximum epochs.
-
-    If `n_obs <= decay_at_n_obs`, the number of maximum epochs is set to
-    `epochs_cap`. Otherwise, the number of maximum epochs decays according to
-    `(decay_at_n_obs / n_obs) * epochs_cap`, with a minimum of 1.
-
-    Parameters
-    ----------
-    n_obs
-        The number of observations in the dataset.
-    epochs_cap
-        The maximum number of epochs for the heuristic.
-    decay_at_n_obs
-        The number of observations at which the heuristic starts decaying.
-
-    Returns
-    -------
-    `int`
-        A heuristic for the default number of maximum epochs.
-    """
-    max_epochs = min(round((decay_at_n_obs / n_obs) * epochs_cap), epochs_cap)
-    max_epochs = max(max_epochs, 1)
-
-    if max_epochs == 1:
-        warnings.warn(
-            "The default number of maximum epochs has been set to 1 due to the large"
-            "number of observations. Pass in `max_epochs` to the `train` function in "
-            "order to override this behavior.",
-            UserWarning,
-            stacklevel=settings.warnings_stacklevel,
-        )
-
-    return max_epochs
-
-
 @devices_dsp.dedent
 def parse_device_args(
     use_gpu: Optional[Union[str, int, bool]] = None,
     accelerator: str = "auto",
     devices: Union[int, List[int], str] = "auto",
     return_device: Optional[Literal["torch", "jax"]] = None,
     validate_single_device: bool = False,
@@ -102,29 +64,20 @@
 
     connector = _AcceleratorConnector(accelerator=accelerator, devices=devices)
     _accelerator = connector._accelerator_flag
     _devices = connector._devices_flag
 
     if _accelerator in ["tpu", "ipu", "hpu"]:
         warnings.warn(
-            f"The selected accelerator `{_accelerator}` has not been extensively "
+            f"The selected accelerator `{_accelerator}` has not been extensively ",
             "tested in scvi-tools. Please report any issues in the GitHub repo.",
             UserWarning,
             stacklevel=settings.warnings_stacklevel,
         )
 
-    if _accelerator == "mps":
-        warnings.warn(
-            "The accelerator has been set to `mps`. Please note that not all PyTorch "
-            "operations are supported with this backend. Refer to "
-            "https://github.com/pytorch/pytorch/issues/77764 for more details.",
-            UserWarning,
-            stacklevel=settings.warnings_stacklevel,
-        )
-
     # get the first device index
     if isinstance(_devices, list):
         device_idx = _devices[0]
     elif isinstance(_devices, str) and "," in _devices:
         device_idx = _devices.split(",")[0]
     else:
         device_idx = _devices
```

### Comparing `scvi_tools-1.0.0/scvi/model/base/__init__.py` & `scvi_tools-1.0.0b0/scvi/model/base/__init__.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/model/base/_archesmixin.py` & `scvi_tools-1.0.0b0/scvi/model/base/_archesmixin.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/model/base/_base_model.py` & `scvi_tools-1.0.0b0/scvi/model/base/_base_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -220,50 +220,14 @@
         if self.id not in self._per_instance_manager_store:
             self._per_instance_manager_store[self.id] = {}
 
         adata_id = adata_manager.adata_uuid
         instance_manager_store = self._per_instance_manager_store[self.id]
         instance_manager_store[adata_id] = adata_manager
 
-    def deregister_manager(self, adata: Optional[AnnData] = None):
-        """Deregisters the :class:`~scvi.data.AnnDataManager` instance associated with `adata`.
-
-        If `adata` is `None`, deregisters all :class:`~scvi.data.AnnDataManager` instances
-        in both the class and instance-specific manager stores, except for the one associated
-        with this model instance.
-        """
-        cls_manager_store = self._setup_adata_manager_store
-        instance_manager_store = self._per_instance_manager_store[self.id]
-
-        if adata is None:
-            instance_managers_to_clear = list(instance_manager_store.keys())
-            cls_managers_to_clear = list(cls_manager_store.keys())
-        else:
-            adata_manager = self._get_most_recent_anndata_manager(adata, required=True)
-            cls_managers_to_clear = [adata_manager.adata_uuid]
-            instance_managers_to_clear = [adata_manager.adata_uuid]
-
-        for adata_id in cls_managers_to_clear:
-            # don't clear the current manager by default
-            is_current_adata = (
-                adata is None and adata_id == self.adata_manager.adata_uuid
-            )
-            if is_current_adata or adata_id not in cls_manager_store:
-                continue
-            del cls_manager_store[adata_id]
-
-        for adata_id in instance_managers_to_clear:
-            # don't clear the current manager by default
-            is_current_adata = (
-                adata is None and adata_id == self.adata_manager.adata_uuid
-            )
-            if is_current_adata or adata_id not in instance_manager_store:
-                continue
-            del instance_manager_store[adata_id]
-
     @classmethod
     def _get_most_recent_anndata_manager(
         cls, adata: AnnOrMuData, required: bool = False
     ) -> Optional[AnnDataManager]:
         """Retrieves the :class:`~scvi.data.AnnDataManager` for a given AnnData object specific to this model class.
 
         Checks for the most recent :class:`~scvi.data.AnnDataManager` created for the given AnnData object via
```

### Comparing `scvi_tools-1.0.0/scvi/model/base/_differential.py` & `scvi_tools-1.0.0b0/scvi/model/base/_differential.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/model/base/_jaxmixin.py` & `scvi_tools-1.0.0b0/scvi/model/base/_jaxmixin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import warnings
 from typing import List, Optional, Union
 
 import jax
+import numpy as np
 
 from scvi.dataloaders import DataSplitter
-from scvi.model._utils import get_max_epochs_heuristic
 from scvi.train import JaxModuleInit, JaxTrainingPlan, TrainRunner
 from scvi.utils._docstrings import devices_dsp
 
 logger = logging.getLogger(__name__)
 
 
 class JaxTrainingMixin:
@@ -58,15 +58,16 @@
         plan_kwargs
             Keyword args for :class:`~scvi.train.JaxTrainingPlan`. Keyword arguments passed to
             `train()` will overwrite values present in `plan_kwargs`, when appropriate.
         **trainer_kwargs
             Other keyword args for :class:`~scvi.train.Trainer`.
         """
         if max_epochs is None:
-            max_epochs = get_max_epochs_heuristic(self.adata.n_obs)
+            n_cells = self.adata.n_obs
+            max_epochs = int(np.min([round((20000 / n_cells) * 400), 400]))
 
         if use_gpu is None or use_gpu is True:
             try:
                 self.module.to(jax.devices("gpu")[0])
                 logger.info(
                     "Jax module moved to GPU. "
                     "Note: Pytorch lightning will show GPU is not being used for the Trainer."
```

### Comparing `scvi_tools-1.0.0/scvi/model/base/_log_likelihood.py` & `scvi_tools-1.0.0b0/scvi/model/base/_log_likelihood.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/model/base/_pyromixin.py` & `scvi_tools-1.0.0b0/scvi/model/base/_pyromixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import numpy as np
 import torch
 from lightning.pytorch.callbacks import Callback
 from pyro import poutine
 
 from scvi import settings
 from scvi.dataloaders import AnnDataLoader, DataSplitter, DeviceBackedDataSplitter
-from scvi.model._utils import get_max_epochs_heuristic, parse_device_args
+from scvi.model._utils import parse_device_args
 from scvi.train import PyroTrainingPlan, TrainRunner
 from scvi.utils import track
 from scvi.utils._docstrings import devices_dsp
 
 logger = logging.getLogger(__name__)
 
 
@@ -130,15 +130,16 @@
         plan_kwargs
             Keyword args for :class:`~scvi.train.PyroTrainingPlan`. Keyword arguments passed to
             `train()` will overwrite values present in `plan_kwargs`, when appropriate.
         **trainer_kwargs
             Other keyword args for :class:`~scvi.train.Trainer`.
         """
         if max_epochs is None:
-            max_epochs = get_max_epochs_heuristic(self.adata.n_obs, epochs_cap=1000)
+            n_obs = self.adata.n_obs
+            max_epochs = int(np.min([round((20000 / n_obs) * 1000), 1000]))
 
         plan_kwargs = plan_kwargs if isinstance(plan_kwargs, dict) else {}
         if lr is not None and "optim" not in plan_kwargs.keys():
             plan_kwargs.update({"optim_kwargs": {"lr": lr}})
 
         if batch_size is None:
             # use data splitter which moves data to GPU once
```

### Comparing `scvi_tools-1.0.0/scvi/model/base/_rnamixin.py` & `scvi_tools-1.0.0b0/scvi/model/base/_rnamixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,16 +40,16 @@
     def _get_importance_weights(
         self,
         adata: Optional[AnnData],
         indices: Optional[Sequence[int]],
         qz: db.Distribution,
         px: db.Distribution,
         zs: torch.Tensor,
-        max_cells: int = 1024,
-        truncation: bool = False,
+        max_cells: int = 128,
+        truncation: bool = True,
         n_mc_samples: int = 500,
         n_mc_samples_per_pass: int = 250,
     ) -> np.ndarray:
         """Computes importance weights for the given samples.
 
         This method computes importance weights for every latent code in `zs` as a way to
         encourage latent codes providing high likelihoods across many cells in the considered
@@ -153,15 +153,14 @@
         library_size: Union[float, Literal["latent"]] = 1,
         n_samples: int = 1,
         n_samples_overall: int = None,
         weights: Optional[Literal["uniform", "importance"]] = None,
         batch_size: Optional[int] = None,
         return_mean: bool = True,
         return_numpy: Optional[bool] = None,
-        **importance_weighting_kwargs,
     ) -> Union[np.ndarray, pd.DataFrame]:
         r"""Returns the normalized (decoded) gene expression.
 
         This is denoted as :math:`\rho_n` in the scVI paper.
 
         Parameters
         ----------
@@ -194,16 +193,14 @@
             Minibatch size for data loading into model. Defaults to `scvi.settings.batch_size`.
         return_mean
             Whether to return the mean of the samples.
         return_numpy
             Return a :class:`~numpy.ndarray` instead of a :class:`~pandas.DataFrame`. DataFrame includes
             gene names as columns. If either `n_samples=1` or `return_mean=True`, defaults to `False`.
             Otherwise, it defaults to `True`.
-        importance_weighting_kwargs
-            Keyword arguments passed into :meth:`~scvi.model.base.RNASeqMixin._get_importance_weights`.
 
         Returns
         -------
         If `n_samples` is provided and `return_mean` is False,
         this method returns a 3d tensor of shape (n_samples, n_cells, n_genes).
         If `n_samples` is provided and `return_mean` is True, it returns a 2d tensor
         of shape (n_cells, n_genes).
@@ -295,15 +292,14 @@
                 px = px_store.get_concatenated_distributions(axis=x_axis)
                 p = self._get_importance_weights(
                     adata,
                     indices,
                     qz=qz,
                     px=px,
                     zs=zs,
-                    **importance_weighting_kwargs,
                 )
             ind_ = np.random.choice(n_samples_, n_samples_overall, p=p, replace=True)
             exprs = exprs[ind_]
         elif n_samples > 1 and return_mean:
             exprs = exprs.mean(0)
 
         if return_numpy is None or return_numpy is False:
@@ -331,15 +327,14 @@
         batch_correction: bool = False,
         batchid1: Optional[Iterable[str]] = None,
         batchid2: Optional[Iterable[str]] = None,
         fdr_target: float = 0.05,
         silent: bool = False,
         weights: Optional[Literal["uniform", "importance"]] = "uniform",
         filter_outlier_cells: bool = False,
-        importance_weighting_kwargs: Optional[dict] = None,
         **kwargs,
     ) -> pd.DataFrame:
         r"""A unified method for differential expression analysis.
 
         Implements ``'vanilla'`` DE :cite:p:`Lopez18` and ``'change'`` mode DE :cite:p:`Boyeau19`.
 
         Parameters
@@ -355,37 +350,29 @@
         %(de_batch_size)s
         %(de_all_stats)s
         %(de_batch_correction)s
         %(de_batchid1)s
         %(de_batchid2)s
         %(de_fdr_target)s
         %(de_silent)s
-        weights
-            Weights to use for sampling. If `None`, defaults to `"uniform"`.
-        filter_outlier_cells
-            Whether to filter outlier cells with :meth:`~scvi.model.base.DifferentialComputation.filter_outlier_cells`.
-        importance_weighting_kwargs
-            Keyword arguments passed into :meth:`~scvi.model.base.RNASeqMixin._get_importance_weights`.
         **kwargs
             Keyword args for :meth:`scvi.model.base.DifferentialComputation.get_bayes_factors`
 
         Returns
         -------
         Differential expression DataFrame.
         """
         adata = self._validate_anndata(adata)
         col_names = adata.var_names
-        importance_weighting_kwargs = importance_weighting_kwargs or {}
         model_fn = partial(
             self.get_normalized_expression,
             return_numpy=True,
             n_samples=1,
             batch_size=batch_size,
             weights=weights,
-            **importance_weighting_kwargs,
         )
         representation_fn = (
             self.get_latent_representation if filter_outlier_cells else None
         )
 
         result = _de_core(
             self.get_anndata_manager(adata, required=True),
```

### Comparing `scvi_tools-1.0.0/scvi/model/base/_training_mixin.py` & `scvi_tools-1.0.0b0/scvi/model/base/_training_mixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import List, Optional, Union
 
+import numpy as np
+
 from scvi.dataloaders import DataSplitter
-from scvi.model._utils import get_max_epochs_heuristic
 from scvi.train import TrainingPlan, TrainRunner
 from scvi.utils._docstrings import devices_dsp
 
 
 class UnsupervisedTrainingMixin:
     """General purpose unsupervised train method."""
 
@@ -53,16 +54,17 @@
             See :class:`~scvi.train.Trainer` for further options.
         plan_kwargs
             Keyword args for :class:`~scvi.train.TrainingPlan`. Keyword arguments passed to
             `train()` will overwrite values present in `plan_kwargs`, when appropriate.
         **trainer_kwargs
             Other keyword args for :class:`~scvi.train.Trainer`.
         """
+        n_cells = self.adata.n_obs
         if max_epochs is None:
-            max_epochs = get_max_epochs_heuristic(self.adata.n_obs)
+            max_epochs = int(np.min([round((20000 / n_cells) * 400), 400]))
 
         plan_kwargs = plan_kwargs if isinstance(plan_kwargs, dict) else {}
 
         data_splitter = self._data_splitter_cls(
             self.adata_manager,
             train_size=train_size,
             validation_size=validation_size,
```

### Comparing `scvi_tools-1.0.0/scvi/model/base/_utils.py` & `scvi_tools-1.0.0b0/scvi/model/base/_utils.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/model/base/_vaemixin.py` & `scvi_tools-1.0.0b0/scvi/model/base/_vaemixin.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/model/utils/_mde.py` & `scvi_tools-1.0.0b0/scvi/model/utils/_mde.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/model/utils/_minification.py` & `scvi_tools-1.0.0b0/scvi/model/utils/_minification.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/module/__init__.py` & `scvi_tools-1.0.0b0/scvi/module/__init__.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/module/_amortizedlda.py` & `scvi_tools-1.0.0b0/scvi/module/_amortizedlda.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/module/_autozivae.py` & `scvi_tools-1.0.0b0/scvi/module/_autozivae.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/module/_classifier.py` & `scvi_tools-1.0.0b0/scvi/module/_classifier.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,21 +7,19 @@
     """Basic fully-connected NN classifier.
 
     Parameters
     ----------
     n_input
         Number of input dimensions
     n_hidden
-        Number of nodes in hidden layer(s). If `0`, the classifier only consists of a
-        single linear layer.
+        Number of hidden nodes in hidden layer
     n_labels
         Numput of outputs dimensions
     n_layers
-        Number of hidden layers. If `0`, the classifier only consists of a single
-        linear layer.
+        Number of hidden layers
     dropout_rate
         dropout_rate for nodes
     logits
         Return logits or not
     use_batch_norm
         Whether to use batch norm in layers
     use_layer_norm
@@ -43,35 +41,28 @@
         use_batch_norm: bool = True,
         use_layer_norm: bool = False,
         activation_fn: nn.Module = nn.ReLU,
         **kwargs,
     ):
         super().__init__()
         self.logits = logits
-        layers = []
-
-        if n_hidden > 0 and n_layers > 0:
-            layers.append(
-                FCLayers(
-                    n_in=n_input,
-                    n_out=n_hidden,
-                    n_layers=n_layers,
-                    n_hidden=n_hidden,
-                    dropout_rate=dropout_rate,
-                    use_batch_norm=use_batch_norm,
-                    use_layer_norm=use_layer_norm,
-                    activation_fn=activation_fn,
-                    **kwargs,
-                )
-            )
-        else:
-            n_hidden = n_input
-
-        layers.append(nn.Linear(n_hidden, n_labels))
-
+        layers = [
+            FCLayers(
+                n_in=n_input,
+                n_out=n_hidden,
+                n_layers=n_layers,
+                n_hidden=n_hidden,
+                dropout_rate=dropout_rate,
+                use_batch_norm=use_batch_norm,
+                use_layer_norm=use_layer_norm,
+                activation_fn=activation_fn,
+                **kwargs,
+            ),
+            nn.Linear(n_hidden, n_labels),
+        ]
         if not logits:
             layers.append(nn.Softmax(dim=-1))
 
         self.classifier = nn.Sequential(*layers)
 
     def forward(self, x):
         """Forward computation."""
```

### Comparing `scvi_tools-1.0.0/scvi/module/_jaxvae.py` & `scvi_tools-1.0.0b0/scvi/module/_jaxvae.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/module/_mrdeconv.py` & `scvi_tools-1.0.0b0/scvi/module/_mrdeconv.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/module/_multivae.py` & `scvi_tools-1.0.0b0/scvi/module/_multivae.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/module/_peakvae.py` & `scvi_tools-1.0.0b0/scvi/module/_peakvae.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/module/_totalvae.py` & `scvi_tools-1.0.0b0/scvi/module/_totalvae.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/module/_utils.py` & `scvi_tools-1.0.0b0/scvi/module/_utils.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/module/_vae.py` & `scvi_tools-1.0.0b0/scvi/module/_vae.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/module/_vaec.py` & `scvi_tools-1.0.0b0/scvi/module/_vaec.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/module/base/_base_module.py` & `scvi_tools-1.0.0b0/scvi/module/base/_base_module.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/module/base/_decorators.py` & `scvi_tools-1.0.0b0/scvi/module/base/_decorators.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/nn/_base_components.py` & `scvi_tools-1.0.0b0/scvi/nn/_base_components.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/train/__init__.py` & `scvi_tools-1.0.0b0/scvi/train/__init__.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/train/_callbacks.py` & `scvi_tools-1.0.0b0/scvi/train/_callbacks.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/train/_logger.py` & `scvi_tools-1.0.0b0/scvi/train/_logger.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/train/_metrics.py` & `scvi_tools-1.0.0b0/scvi/train/_metrics.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/train/_progress.py` & `scvi_tools-1.0.0b0/scvi/train/_progress.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/train/_trainer.py` & `scvi_tools-1.0.0b0/scvi/train/_trainer.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/train/_trainingplans.py` & `scvi_tools-1.0.0b0/scvi/train/_trainingplans.py`

 * *Files 2% similar despite different names*

```diff
@@ -336,15 +336,15 @@
     def training_step(self, batch, batch_idx):
         """Training step for the model."""
         if "kl_weight" in self.loss_kwargs:
             kl_weight = self.kl_weight
             self.loss_kwargs.update({"kl_weight": kl_weight})
             self.log("kl_weight", kl_weight, on_step=True, on_epoch=False)
         _, _, scvi_loss = self.forward(batch, loss_kwargs=self.loss_kwargs)
-        self.log("train_loss", scvi_loss.loss, on_epoch=True, prog_bar=True)
+        self.log("train_loss", scvi_loss.loss, on_epoch=True)
         self.compute_and_log_metrics(scvi_loss, self.train_metrics, "train")
         return scvi_loss.loss
 
     def validation_step(self, batch, batch_idx):
         """Validation step for the model."""
         # loss kwargs here contains `n_obs` equal to n_training_obs
         # so when relevant, the actual loss value is rescaled to number
@@ -559,15 +559,15 @@
         z = inference_outputs["z"]
         loss = scvi_loss.loss
         # fool classifier if doing adversarial training
         if kappa > 0 and self.adversarial_classifier is not False:
             fool_loss = self.loss_adversarial_classifier(z, batch_tensor, False)
             loss += fool_loss * kappa
 
-        self.log("train_loss", loss, on_epoch=True, prog_bar=True)
+        self.log("train_loss", loss, on_epoch=True)
         self.compute_and_log_metrics(scvi_loss, self.train_metrics, "train")
         opt1.zero_grad()
         self.manual_backward(loss)
         opt1.step()
 
         # train adversarial classifier
         # this condition will not be met unless self.adversarial_classifier is not False
@@ -712,18 +712,17 @@
         )
         self.loss_kwargs.update({"classification_ratio": classification_ratio})
         self.initialize_metrics(n_classes)
 
     def initialize_metrics(self, n_classes: int):
         """Initialize metrics."""
         kwargs = {"task": "multiclass", "num_classes": n_classes}
-        self.train_accuracy = Accuracy(**kwargs)
-        self.train_f1 = F1Score(**kwargs)
-        self.val_accuracy = Accuracy(**kwargs)
-        self.val_f1 = F1Score(**kwargs)
+        self.accuracy = Accuracy(**kwargs)
+        self.f1 = F1Score(**kwargs)
+        self.auroc = AUROC(**kwargs)
 
     def log_with_mode(self, key: str, value: Any, mode: str, **kwargs):
         """Log with mode."""
         # TODO: Include this with a base training plan
         self.log(f"{mode}_{key}", value, **kwargs)
 
     def compute_and_log_metrics(
@@ -737,47 +736,38 @@
             return
 
         classification_loss = loss_output.classification_loss
         true_labels = loss_output.true_labels
         logits = loss_output.logits
         predicted_labels = torch.argmax(logits, dim=-1, keepdim=True)
 
-        if mode == "train":
-            accuracy = self.train_accuracy
-            f1 = self.train_f1
-        else:
-            accuracy = self.val_accuracy
-            f1 = self.val_f1
-
-        accuracy(predicted_labels, true_labels)
-        f1(predicted_labels, true_labels)
+        self.accuracy(predicted_labels, true_labels)
+        self.f1(predicted_labels, true_labels)
+        self.auroc(logits, true_labels.view(-1).long())
 
         self.log_with_mode(
             METRIC_KEYS.CLASSIFICATION_LOSS_KEY,
             classification_loss,
             mode,
             on_step=False,
             on_epoch=True,
-            batch_size=loss_output.n_obs_minibatch,
         )
         self.log_with_mode(
             METRIC_KEYS.ACCURACY_KEY,
-            accuracy,
+            self.accuracy,
             mode,
             on_step=False,
             on_epoch=True,
-            batch_size=loss_output.n_obs_minibatch,
         )
         self.log_with_mode(
             METRIC_KEYS.F1_SCORE_KEY,
-            f1,
+            self.f1,
             mode,
             on_step=False,
             on_epoch=True,
-            batch_size=loss_output.n_obs_minibatch,
         )
         # currently not logging auroc due to accumulation error
 
     def training_step(self, batch, batch_idx):
         """Training step for semi-supervised training."""
         # Potentially dangerous if batch is from a single dataloader with two keys
         if len(batch) == 2:
@@ -797,15 +787,14 @@
         _, _, loss_output = self.forward(full_dataset, loss_kwargs=input_kwargs)
         loss = loss_output.loss
         self.log(
             "train_loss",
             loss,
             on_epoch=True,
             batch_size=loss_output.n_obs_minibatch,
-            prog_bar=True,
         )
         self.compute_and_log_metrics(loss_output, self.train_metrics, "train")
         return loss
 
     def validation_step(self, batch, batch_idx):
         """Validation step for semi-supervised training."""
         # Potentially dangerous if batch is from a single dataloader with two keys
@@ -1163,15 +1152,15 @@
         self.log_with_mode(METRIC_KEYS.F1_SCORE_KEY, self.f1, mode)
         self.log_with_mode(METRIC_KEYS.AUROC_KEY, self.auroc, mode)
 
     def training_step(self, batch, batch_idx):
         """Training step for classifier training."""
         soft_prediction = self.forward(batch[self.data_key])
         loss = self.loss_fn(soft_prediction, batch[self.labels_key].view(-1).long())
-        self.log("train_loss", loss, on_epoch=True, prog_bar=True)
+        self.log("train_loss", loss, on_epoch=True)
         return loss
 
     def validation_step(self, batch, batch_idx):
         """Validation step for classifier training."""
         soft_prediction = self.forward(batch[self.data_key])
         loss = self.loss_fn(soft_prediction, batch[self.labels_key].view(-1).long())
         self.log("validation_loss", loss)
```

### Comparing `scvi_tools-1.0.0/scvi/train/_trainrunner.py` & `scvi_tools-1.0.0b0/scvi/train/_trainrunner.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/utils/_decorators.py` & `scvi_tools-1.0.0b0/scvi/utils/_decorators.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/utils/_docstrings.py` & `scvi_tools-1.0.0b0/scvi/utils/_docstrings.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/utils/_exceptions.py` & `scvi_tools-1.0.0b0/scvi/utils/_exceptions.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/scvi/utils/_track.py` & `scvi_tools-1.0.0b0/scvi/utils/_track.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/conftest.py` & `scvi_tools-1.0.0b0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/autotune/test_manager.py` & `scvi_tools-1.0.0b0/tests/autotune/test_manager.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/autotune/test_tuner.py` & `scvi_tools-1.0.0b0/tests/autotune/test_tuner.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/autotune/test_types.py` & `scvi_tools-1.0.0b0/tests/autotune/test_types.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/core/test_differential.py` & `scvi_tools-1.0.0b0/tests/core/test_differential.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/core/test_distributions.py` & `scvi_tools-1.0.0b0/tests/core/test_distributions.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/Cortex.loom` & `scvi_tools-1.0.0b0/tests/data/Cortex.loom`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/GSE100866_CBMC_8K_13AB_10X-RNA_umi.csv.gz` & `scvi_tools-1.0.0b0/tests/data/GSE100866_CBMC_8K_13AB_10X-RNA_umi.csv.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/Layer2_BC_count_matrix-1.tsv` & `scvi_tools-1.0.0b0/tests/data/Layer2_BC_count_matrix-1.tsv`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/Rep11_MOB_count_matrix-1.tsv` & `scvi_tools-1.0.0b0/tests/data/Rep11_MOB_count_matrix-1.tsv`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/SeqFISH.xlsx` & `scvi_tools-1.0.0b0/tests/data/SeqFISH.xlsx`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/TM_droplet_mat.h5ad` & `scvi_tools-1.0.0b0/tests/data/TM_droplet_mat.h5ad`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/brain_large.h5` & `scvi_tools-1.0.0b0/tests/data/brain_large.h5`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/brain_small_metadata.pickle` & `scvi_tools-1.0.0b0/tests/data/brain_small_metadata.pickle`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/brainlarge_dataset_test.h5ad` & `scvi_tools-1.0.0b0/tests/data/brainlarge_dataset_test.h5ad`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/expression.bin` & `scvi_tools-1.0.0b0/tests/data/expression.bin`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/fc-dropseq.loom` & `scvi_tools-1.0.0b0/tests/data/fc-dropseq.loom`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/immune_control_expression_matrix.txt` & `scvi_tools-1.0.0b0/tests/data/immune_control_expression_matrix.txt`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/immune_stimulated_expression_matrix.txt` & `scvi_tools-1.0.0b0/tests/data/immune_stimulated_expression_matrix.txt`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/mpfc-starmap.loom` & `scvi_tools-1.0.0b0/tests/data/mpfc-starmap.loom`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/osmFISH_SScortex_mouse_all_cell.loom` & `scvi_tools-1.0.0b0/tests/data/osmFISH_SScortex_mouse_all_cell.loom`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/pbmc_10k_protein_v3.h5ad` & `scvi_tools-1.0.0b0/tests/data/pbmc_10k_protein_v3.h5ad`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/pbmc_5k_protein_v3.h5ad` & `scvi_tools-1.0.0b0/tests/data/pbmc_5k_protein_v3.h5ad`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/random_metadata.pickle` & `scvi_tools-1.0.0b0/tests/data/random_metadata.pickle`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/retina.loom` & `scvi_tools-1.0.0b0/tests/data/retina.loom`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/seqfishplus.zip` & `scvi_tools-1.0.0b0/tests/data/seqfishplus.zip`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/10X/gene_info_pbmc.csv` & `scvi_tools-1.0.0b0/tests/data/10X/gene_info_pbmc.csv`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/10X/pbmc_metadata.pickle` & `scvi_tools-1.0.0b0/tests/data/10X/pbmc_metadata.pickle`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/10X/b_cells/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.0b0/tests/data/10X/b_cells/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/10X/cd14_monocytes/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.0b0/tests/data/10X/cd14_monocytes/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/10X/cd34/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.0b0/tests/data/10X/cd34/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/10X/cd4_t_helper/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.0b0/tests/data/10X/cd4_t_helper/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/10X/cd56_nk/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.0b0/tests/data/10X/cd56_nk/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/10X/cytotoxic_t/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.0b0/tests/data/10X/cytotoxic_t/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/10X/memory_t/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.0b0/tests/data/10X/memory_t/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/10X/naive_cytotoxic/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.0b0/tests/data/10X/naive_cytotoxic/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/10X/naive_t/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.0b0/tests/data/10X/naive_t/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/10X/neuron_9k/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.0b0/tests/data/10X/neuron_9k/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/10X/neuron_9k/filtered_gene_bc_matrices/mm10/barcodes.tsv` & `scvi_tools-1.0.0b0/tests/data/10X/neuron_9k/filtered_gene_bc_matrices/mm10/barcodes.tsv`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/10X/neuron_9k/filtered_gene_bc_matrices/mm10/matrix.mtx` & `scvi_tools-1.0.0b0/tests/data/10X/neuron_9k/filtered_gene_bc_matrices/mm10/matrix.mtx`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/10X/pbmc4k/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.0b0/tests/data/10X/pbmc4k/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/10X/pbmc8k/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.0b0/tests/data/10X/pbmc8k/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/10X/pbmc_10k_protein_v3/filtered_feature_bc_matrix.tar.gz` & `scvi_tools-1.0.0b0/tests/data/10X/pbmc_10k_protein_v3/filtered_feature_bc_matrix.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/10X/regulatory_t/filtered_gene_bc_matrices.tar.gz` & `scvi_tools-1.0.0b0/tests/data/10X/regulatory_t/filtered_gene_bc_matrices.tar.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/HEMATO/bBM.raw_umifm_counts.csv.gz` & `scvi_tools-1.0.0b0/tests/data/HEMATO/bBM.raw_umifm_counts.csv.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/HEMATO/bBM.spring_and_pba.csv` & `scvi_tools-1.0.0b0/tests/data/HEMATO/bBM.spring_and_pba.csv`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/citeSeq/cbmc/cbmc_adt_centered.csv.gz` & `scvi_tools-1.0.0b0/tests/data/citeSeq/cbmc/cbmc_adt_centered.csv.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/citeSeq/pbmc/pbmc_adt_centered.csv.gz` & `scvi_tools-1.0.0b0/tests/data/citeSeq/pbmc/pbmc_adt_centered.csv.gz`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/filtered_gene_bc_matrices/hg19/barcodes.tsv` & `scvi_tools-1.0.0b0/tests/data/filtered_gene_bc_matrices/hg19/barcodes.tsv`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/filtered_gene_bc_matrices/hg19/matrix.mtx` & `scvi_tools-1.0.0b0/tests/data/filtered_gene_bc_matrices/hg19/matrix.mtx`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/simulation/simulation_1.loom` & `scvi_tools-1.0.0b0/tests/data/simulation/simulation_1.loom`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/simulation/simulation_2.loom` & `scvi_tools-1.0.0b0/tests/data/simulation/simulation_2.loom`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/data/simulation/simulation_3.loom` & `scvi_tools-1.0.0b0/tests/data/simulation/simulation_3.loom`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/dataloaders/test_datasplitter.py` & `scvi_tools-1.0.0b0/tests/dataloaders/test_datasplitter.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/dataset/conftest.py` & `scvi_tools-1.0.0b0/tests/dataset/conftest.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/dataset/test_anndata.py` & `scvi_tools-1.0.0b0/tests/dataset/test_anndata.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/dataset/test_built_in_data.py` & `scvi_tools-1.0.0b0/tests/dataset/test_built_in_data.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/dataset/test_dataset10X.py` & `scvi_tools-1.0.0b0/tests/dataset/test_dataset10X.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/dataset/test_mudata.py` & `scvi_tools-1.0.0b0/tests/dataset/test_mudata.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/dataset/test_preprocessing.py` & `scvi_tools-1.0.0b0/tests/dataset/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/dataset/utils.py` & `scvi_tools-1.0.0b0/tests/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/external/test_cellassign.py` & `scvi_tools-1.0.0b0/tests/external/test_cellassign.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/external/test_gimvi.py` & `scvi_tools-1.0.0b0/tests/external/test_gimvi.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/external/test_scar.py` & `scvi_tools-1.0.0b0/tests/external/test_scar.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/external/test_scbasset.py` & `scvi_tools-1.0.0b0/tests/external/test_scbasset.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/external/test_stereoscope.py` & `scvi_tools-1.0.0b0/tests/external/test_stereoscope.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/external/test_tangram.py` & `scvi_tools-1.0.0b0/tests/external/test_tangram.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/hub/test_hub_metadata.py` & `scvi_tools-1.0.0b0/tests/hub/test_hub_metadata.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/hub/test_hub_model.py` & `scvi_tools-1.0.0b0/tests/hub/test_hub_model.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/models/test_lightning.py` & `scvi_tools-1.0.0b0/tests/models/test_lightning.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/models/test_models.py` & `scvi_tools-1.0.0b0/tests/models/test_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1108,32 +1108,14 @@
     m = SCVI(a, use_observed_lib_size=False)
     a2 = scvi.data.synthetic_iid()
     a2.obs["size_factor"] = np.random.randint(1, 5, size=(a2.shape[0],))
     scanvi_model = scvi.model.SCANVI.from_scvi_model(m, "label_0", adata=a2)
     scanvi_model.train(1)
 
 
-def test_linear_classifier_scanvi(n_latent: int = 10, n_labels: int = 5):
-    adata = synthetic_iid(n_labels=n_labels)
-    SCANVI.setup_anndata(
-        adata,
-        "labels",
-        "label_0",
-        batch_key="batch",
-    )
-    model = SCANVI(adata, linear_classifier=True, n_latent=n_latent)
-
-    assert len(model.module.classifier.classifier) == 2  # linear layer + softmax
-    assert isinstance(model.module.classifier.classifier[0], torch.nn.Linear)
-    assert model.module.classifier.classifier[0].in_features == n_latent
-    assert model.module.classifier.classifier[0].out_features == n_labels - 1
-
-    model.train(max_epochs=1)
-
-
 def test_linear_scvi(save_path):
     adata = synthetic_iid()
     adata = adata[:, :10].copy()
     LinearSCVI.setup_anndata(adata)
     model = LinearSCVI(adata, n_latent=10)
     model.train(1, check_val_every_n_epoch=1, train_size=0.5)
     assert len(model.history["elbo_train"]) == 1
```

### Comparing `scvi_tools-1.0.0/tests/models/test_models_with_minified_data.py` & `scvi_tools-1.0.0b0/tests/models/test_models_with_minified_data.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/models/test_mudata_models.py` & `scvi_tools-1.0.0b0/tests/models/test_mudata_models.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/models/test_pyro.py` & `scvi_tools-1.0.0b0/tests/models/test_pyro.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/models/test_scarches.py` & `scvi_tools-1.0.0b0/tests/models/test_scarches.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/tests/train/test_trainingplans.py` & `scvi_tools-1.0.0b0/tests/train/test_trainingplans.py`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/.gitignore` & `scvi_tools-1.0.0b0/.gitignore`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/LICENSE` & `scvi_tools-1.0.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/README.md` & `scvi_tools-1.0.0b0/README.md`

 * *Files identical despite different names*

### Comparing `scvi_tools-1.0.0/pyproject.toml` & `scvi_tools-1.0.0b0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 
 [project]
 name = "scvi-tools"
-version = "1.0.0"
+version = "1.0.0b0"
 description = "Deep probabilistic analysis of single-cell omics data."
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 authors = [
     {name = "The scvi-tools development team"},
 ]
@@ -46,19 +46,18 @@
     "h5py>=2.9.0",
     "torch>=1.8.0",
     "lightning>=2.0,<2.1",
     "torchmetrics>=0.11.0",
     "pyro-ppl>=1.6.0",
     "tqdm>=4.56.0",
     "scikit-learn>=0.21.2",
-    "numpyro>=0.12.1",
+    "numpyro",
     "ml-collections>=0.1.1",
     "mudata>=0.1.2",
     "sparse>=0.14.0",
-    "xarray>=2023.2.0",
 ]
 
 
 [project.optional-dependencies]
 dev = [
     "black",
     "pytest",
```

### Comparing `scvi_tools-1.0.0/PKG-INFO` & `scvi_tools-1.0.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scvi-tools
-Version: 1.0.0
+Version: 1.0.0b0
 Summary: Deep probabilistic analysis of single-cell omics data.
 Project-URL: Documentation, https://scvi-tools.org
 Project-URL: Source, https://github.com/scverse/scvi-tools
 Project-URL: Home-page, https://scvi-tools.org
 Author: The scvi-tools development team
 Maintainer-email: The scvi-tools development team <adamgayoso@berkeley.edu>
 License: BSD 3-Clause License
@@ -53,26 +53,25 @@
 Requires-Dist: h5py>=2.9.0
 Requires-Dist: jax>=0.4.4
 Requires-Dist: jaxlib>=0.4.3
 Requires-Dist: lightning<2.1,>=2.0
 Requires-Dist: ml-collections>=0.1.1
 Requires-Dist: mudata>=0.1.2
 Requires-Dist: numpy>=1.17.0
-Requires-Dist: numpyro>=0.12.1
+Requires-Dist: numpyro
 Requires-Dist: optax
 Requires-Dist: pandas>=1.0
 Requires-Dist: pyro-ppl>=1.6.0
 Requires-Dist: rich>=12.0.0
 Requires-Dist: scikit-learn>=0.21.2
 Requires-Dist: scipy
 Requires-Dist: sparse>=0.14.0
 Requires-Dist: torch>=1.8.0
 Requires-Dist: torchmetrics>=0.11.0
 Requires-Dist: tqdm>=4.56.0
-Requires-Dist: xarray>=2023.2.0
 Provides-Extra: autotune
 Requires-Dist: hyperopt>=0.2; extra == 'autotune'
 Requires-Dist: ipython; extra == 'autotune'
 Requires-Dist: ray[tune]>=2.2.0; extra == 'autotune'
 Requires-Dist: scib-metrics>=0.3; extra == 'autotune'
 Provides-Extra: census
 Requires-Dist: cellxgene-census; extra == 'census'
```

