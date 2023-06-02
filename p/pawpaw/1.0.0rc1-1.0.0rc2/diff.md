# Comparing `tmp/pawpaw-1.0.0rc1.tar.gz` & `tmp/pawpaw-1.0.0rc2.tar.gz`

## Comparing `pawpaw-1.0.0rc1.tar` & `pawpaw-1.0.0rc2.tar`

### file list

```diff
@@ -1,117 +1,117 @@
--rw-r--r--   0        0        0     5236 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/CONTRIBUTING.md
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/SECURITY.md
--rw-r--r--   0        0        0     9502 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tinker.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/.idea/.gitignore
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/.idea/misc.xml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/.idea/modules.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/.idea/pawpaw.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/.idea/vcs.xml
--rw-r--r--   0        0        0    37396 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     9184 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/0. Introduction.md
--rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/1. Segment and Span.md
--rw-r--r--   0        0        0    23527 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/2. In Text Object.md
--rw-r--r--   0        0        0     9237 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/3. Visualization.md
--rw-r--r--   0        0        0    22226 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/4. Arborform.md
--rw-r--r--   0        0        0    15140 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/5. Traversal & Query.md
--rw-r--r--   0        0        0    13200 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/6. Xml.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/7. NLP.md
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/8. Serialization.md
--rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/Pawpaw Cookbook.md
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/Using Pawpaw with nltk.md
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/demos/Q&A/description.md
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/demos/Q&A/solution.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/demos/class_grades/description.md
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/demos/class_grades/input.txt
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/demos/class_grades/parser_compact.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/demos/class_grades/parser_verbose.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/demos/class_grades/solution.py
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/demos/gettysburg_address/gettysburg_address.txt
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/demos/us_constitution/description.md
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/demos/us_constitution/us_constitution.py
--rw-r--r--   0        0        0    26246 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/docs/demos/us_constitution/us_constitution.txt
--rw-r--r--   0        0        0   940341 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/images/pawpaw.png
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/__init__.py
--rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/_type_magic.py
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/_version.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/errors.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/infix.py
--rw-r--r--   0        0        0    53884 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/ito.py
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/span.py
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/util.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/arborform/__init__.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/arborform/itorator/__init__.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/arborform/itorator/desc.py
--rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/arborform/itorator/extract.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/arborform/itorator/filter.py
--rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/arborform/itorator/itorator.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/arborform/itorator/reflect.py
--rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/arborform/itorator/split.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/arborform/itorator/value_func.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/arborform/postorator/__init__.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/arborform/postorator/postorator.py
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/arborform/postorator/stacked_reduce.py
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/arborform/postorator/windowed_join.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/nlp/__init__.py
--rw-r--r--   0        0        0    15793 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/nlp/nlp.py
--rw-r--r--   0        0        0     3661 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/nlp/table.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/query/__init__.py
--rw-r--r--   0        0        0    27949 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/query/_query.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/visualization/__init__.py
--rw-r--r--   0        0        0    51546 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/visualization/ascii_box.py
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/visualization/highlighter.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/visualization/pepo/__init__.py
--rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/visualization/pepo/pepo.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/visualization/sgr/__init__.py
--rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/visualization/sgr/sgr.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/visualization/sgr/palettes/__init__.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/visualization/sgr/palettes/palettes.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/xml/__init__.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/xml/descriptors.py
--rw-r--r--   0        0        0     9818 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/xml/xml_helper.py
--rw-r--r--   0        0        0     8147 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pawpaw/xml/xml_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/__init__.py
--rw-r--r--   0        0        0    12004 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/test_child_itos.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/test_invoke_func.py
--rw-r--r--   0        0        0    20727 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/test_ito.py
--rw-r--r--   0        0        0    20370 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/test_ito_ctor.py
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/test_ito_descend.py
--rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/test_ito_regex_equivalence_methods.py
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/test_ito_serialization.py
--rw-r--r--   0        0        0    17476 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/test_ito_str_equivalence_methods.py
--rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/test_nlp.py
--rw-r--r--   0        0        0    41635 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/test_query_and_traversal.py
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/test_span.py
--rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/test_type_magic.py
--rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/test_util.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/test_version.py
--rw-r--r--   0        0        0     5333 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/test_xml_helper.py
--rw-r--r--   0        0        0     6838 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/test_xml_parser.py
--rw-r--r--   0        0        0     7560 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/util.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/arborform/__init__.py
--rw-r--r--   0        0        0    10053 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/arborform/test_connectors.py
--rw-r--r--   0        0        0    14065 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/arborform/test_itorator.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/arborform/test_itorator_desc.py
--rw-r--r--   0        0        0     7467 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/arborform/test_itorator_extract.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/arborform/test_itorator_filter.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/arborform/test_itorator_reflect.py
--rw-r--r--   0        0        0     5571 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/arborform/test_itorator_split.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/arborform/test_itorator_value_func.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/arborform/test_postorator.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/arborform/test_postorator_windowed_join.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/visualization/__init__.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/visualization/test_sgr.py
--rw-r--r--   0        0        0     5907 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/tests/visualization/test_visualization_ascii_box.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/LICENSE
--rw-r--r--   0        0        0    15670 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/README.md
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0    16264 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     5236 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/CONTRIBUTING.md
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/SECURITY.md
+-rw-r--r--   0        0        0    14348 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tinker.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/.idea/.gitignore
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/.idea/misc.xml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/.idea/modules.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/.idea/pawpaw.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/.idea/vcs.xml
+-rw-r--r--   0        0        0    37655 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     9184 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/0. Introduction.md
+-rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/1. Segment and Span.md
+-rw-r--r--   0        0        0    23527 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/2. In Text Object.md
+-rw-r--r--   0        0        0    21169 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/3. Visualization.md
+-rw-r--r--   0        0        0    22995 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/4. Arborform.md
+-rw-r--r--   0        0        0    15852 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/5. Traversal & Query.md
+-rw-r--r--   0        0        0    13200 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/6. Xml.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/7. NLP.md
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/8. Serialization.md
+-rw-r--r--   0        0        0     5042 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/Pawpaw Cookbook.md
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/Using Pawpaw with nltk.md
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/demos/Q&A/description.md
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/demos/Q&A/solution.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/demos/class_grades/description.md
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/demos/class_grades/input.txt
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/demos/class_grades/parser_compact.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/demos/class_grades/parser_verbose.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/demos/class_grades/solution.py
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/demos/gettysburg_address/gettysburg_address.txt
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/demos/us_constitution/description.md
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/demos/us_constitution/us_constitution.py
+-rw-r--r--   0        0        0    26246 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/docs/demos/us_constitution/us_constitution.txt
+-rw-r--r--   0        0        0   940341 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/images/pawpaw.png
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/__init__.py
+-rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/_type_magic.py
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/_version.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/errors.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/infix.py
+-rw-r--r--   0        0        0    53966 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/ito.py
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/span.py
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/util.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/arborform/__init__.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/arborform/itorator/__init__.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/arborform/itorator/desc.py
+-rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/arborform/itorator/extract.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/arborform/itorator/filter.py
+-rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/arborform/itorator/itorator.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/arborform/itorator/reflect.py
+-rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/arborform/itorator/split.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/arborform/itorator/value_func.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/arborform/postorator/__init__.py
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/arborform/postorator/postorator.py
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/arborform/postorator/stacked_reduce.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/arborform/postorator/windowed_join.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/nlp/__init__.py
+-rw-r--r--   0        0        0    15793 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/nlp/nlp.py
+-rw-r--r--   0        0        0     3661 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/nlp/table.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/query/__init__.py
+-rw-r--r--   0        0        0    27949 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/query/_query.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/visualization/__init__.py
+-rw-r--r--   0        0        0    51546 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/visualization/ascii_box.py
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/visualization/highlighter.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/visualization/pepo/__init__.py
+-rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/visualization/pepo/pepo.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/visualization/sgr/__init__.py
+-rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/visualization/sgr/sgr.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/visualization/sgr/palettes/__init__.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/visualization/sgr/palettes/palettes.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/xml/__init__.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/xml/descriptors.py
+-rw-r--r--   0        0        0     9818 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/xml/xml_helper.py
+-rw-r--r--   0        0        0     8147 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pawpaw/xml/xml_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/__init__.py
+-rw-r--r--   0        0        0    12004 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/test_child_itos.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/test_invoke_func.py
+-rw-r--r--   0        0        0    20727 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/test_ito.py
+-rw-r--r--   0        0        0    20370 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/test_ito_ctor.py
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/test_ito_descend.py
+-rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/test_ito_regex_equivalence_methods.py
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/test_ito_serialization.py
+-rw-r--r--   0        0        0    17476 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/test_ito_str_equivalence_methods.py
+-rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/test_nlp.py
+-rw-r--r--   0        0        0    41635 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/test_query_and_traversal.py
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/test_span.py
+-rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/test_type_magic.py
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/test_util.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/test_version.py
+-rw-r--r--   0        0        0     5333 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/test_xml_helper.py
+-rw-r--r--   0        0        0     6838 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/test_xml_parser.py
+-rw-r--r--   0        0        0     7560 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/util.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/arborform/__init__.py
+-rw-r--r--   0        0        0    10053 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/arborform/test_connectors.py
+-rw-r--r--   0        0        0    14065 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/arborform/test_itorator.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/arborform/test_itorator_desc.py
+-rw-r--r--   0        0        0     7467 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/arborform/test_itorator_extract.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/arborform/test_itorator_filter.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/arborform/test_itorator_reflect.py
+-rw-r--r--   0        0        0     5571 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/arborform/test_itorator_split.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/arborform/test_itorator_value_func.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/arborform/test_postorator.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/arborform/test_postorator_windowed_join.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/visualization/__init__.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/visualization/test_sgr.py
+-rw-r--r--   0        0        0     5907 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/tests/visualization/test_visualization_ascii_box.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/LICENSE
+-rw-r--r--   0        0        0    15670 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/README.md
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/pyproject.toml
+-rw-r--r--   0        0        0    16264 2020-02-02 00:00:00.000000 pawpaw-1.0.0rc2/PKG-INFO
```

### Comparing `pawpaw-1.0.0rc1/CODE_OF_CONDUCT.md` & `pawpaw-1.0.0rc2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/CONTRIBUTING.md` & `pawpaw-1.0.0rc2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/SECURITY.md` & `pawpaw-1.0.0rc2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/.github/ISSUE_TEMPLATE/bug_report.md` & `pawpaw-1.0.0rc2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/.github/ISSUE_TEMPLATE/feature_request.md` & `pawpaw-1.0.0rc2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/.idea/workspace.xml` & `pawpaw-1.0.0rc2/.idea/workspace.xml`

 * *Files 1% similar despite different names*

#### Comparing `pawpaw-1.0.0rc1/.idea/workspace.xml` & `pawpaw-1.0.0rc2/.idea/workspace.xml`

```diff
@@ -51,14 +51,35 @@
     <key name="MoveFile.RECENT_KEYS">
       <recent name="C:\Users\rlaye\Documents\PycharmProjects\pawpaw\tests\arborform"/>
       <recent name="C:\Users\rlaye\Documents\PycharmProjects\pawpaw\tests\visualization"/>
       <recent name="C:\Users\rlaye\Documents\PycharmProjects\pawpaw\pawpaw\arborform\itorator"/>
     </key>
   </component>
   <component name="RunManager" selected="Python tests. All Unittests">
+    <configuration name="parser_verbose" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
+      <module name="pawpaw"/>
+      <option name="INTERPRETER_OPTIONS" value=""/>
+      <option name="PARENT_ENVS" value="true"/>
+      <envs>
+        <env name="PYTHONUNBUFFERED" value="1"/>
+      </envs>
+      <option name="SDK_HOME" value=""/>
+      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/docs/demos/class_grades"/>
+      <option name="IS_MODULE_SDK" value="true"/>
+      <option name="ADD_CONTENT_ROOTS" value="true"/>
+      <option name="ADD_SOURCE_ROOTS" value="true"/>
+      <option name="SCRIPT_NAME" value="$PROJECT_DIR$/docs/demos/class_grades/parser_verbose.py"/>
+      <option name="PARAMETERS" value=""/>
+      <option name="SHOW_COMMAND_LINE" value="false"/>
+      <option name="EMULATE_TERMINAL" value="false"/>
+      <option name="MODULE_MODE" value="false"/>
+      <option name="REDIRECT_INPUT" value="false"/>
+      <option name="INPUT_FILE" value=""/>
+      <method v="2"/>
+    </configuration>
     <configuration name="solution (1)" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
       <module name="pawpaw"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs>
         <env name="PYTHONUNBUFFERED" value="1"/>
       </envs>
@@ -150,28 +171,14 @@
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <option name="_new_pattern" value="&quot;&quot;"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
       <option name="_new_target" value="&quot;$PROJECT_DIR$/tests&quot;"/>
       <option name="_new_targetType" value="&quot;PATH&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="Python tests in test_child_itos.py" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
-      <module name="pawpaw"/>
-      <option name="INTERPRETER_OPTIONS" value=""/>
-      <option name="PARENT_ENVS" value="true"/>
-      <option name="SDK_HOME" value=""/>
-      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
-      <option name="IS_MODULE_SDK" value="true"/>
-      <option name="ADD_CONTENT_ROOTS" value="true"/>
-      <option name="ADD_SOURCE_ROOTS" value="true"/>
-      <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;$PROJECT_DIR$/tests/test_child_itos.py&quot;"/>
-      <option name="_new_targetType" value="&quot;PATH&quot;"/>
-      <method v="2"/>
-    </configuration>
     <configuration name="Python tests in test_nlp.py" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="pawpaw"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
       <option name="IS_MODULE_SDK" value="true"/>
@@ -195,62 +202,41 @@
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
       <option name="_new_target" value="&quot;test_type_magic.TestTypeMagic.test_is_callable_exact&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
     <list>
       <item itemvalue="Python.tinker"/>
+      <item itemvalue="Python.parser_verbose"/>
       <item itemvalue="Python.solution"/>
       <item itemvalue="Python.solution (1)"/>
       <item itemvalue="Python.us_constitution"/>
       <item itemvalue="Python tests.Unittests for test_type_magic.TestTypeMagic.test_is_callable_exact"/>
       <item itemvalue="Python tests. All Unittests"/>
       <item itemvalue="Python tests.Python tests in test_nlp.py"/>
-      <item itemvalue="Python tests.Python tests in test_child_itos.py"/>
     </list>
     <recent_temporary>
       <list>
-        <item itemvalue="Python tests.Python tests in test_nlp.py"/>
+        <item itemvalue="Python.solution (1)"/>
+        <item itemvalue="Python.parser_verbose"/>
         <item itemvalue="Python.us_constitution"/>
         <item itemvalue="Python.solution"/>
-        <item itemvalue="Python.solution (1)"/>
-        <item itemvalue="Python tests.Python tests in test_child_itos.py"/>
+        <item itemvalue="Python tests.Python tests in test_nlp.py"/>
       </list>
     </recent_temporary>
   </component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="60f56f5e-2b22-4441-9568-072b306fbfd2" name="Changes" comment=""/>
       <created>1668472305766</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1668472305766</updated>
     </task>
-    <task id="LOCAL-00033" summary="__version__ = '1.0.0.a7'">
-      <created>1671850838352</created>
-      <option name="number" value="00033"/>
-      <option name="presentableId" value="LOCAL-00033"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1671850838352</updated>
-    </task>
-    <task id="LOCAL-00034" summary="__version__ = '1.0.0.a7'">
-      <created>1671850917519</created>
-      <option name="number" value="00034"/>
-      <option name="presentableId" value="LOCAL-00034"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1671850917519</updated>
-    </task>
-    <task id="LOCAL-00035" summary="ascii_box updates">
-      <created>1673232354514</created>
-      <option name="number" value="00035"/>
-      <option name="presentableId" value="LOCAL-00035"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1673232354514</updated>
-    </task>
     <task id="LOCAL-00036" summary="peduncle -&gt; pepo">
       <created>1673395183314</created>
       <option name="number" value="00036"/>
       <option name="presentableId" value="LOCAL-00036"/>
       <option name="project" value="LOCAL"/>
       <updated>1673395183314</updated>
     </task>
@@ -565,21 +551,39 @@
     <task id="LOCAL-00081" summary="Unit test count update">
       <created>1682384148587</created>
       <option name="number" value="00081"/>
       <option name="presentableId" value="LOCAL-00081"/>
       <option name="project" value="LOCAL"/>
       <updated>1682384148587</updated>
     </task>
-    <option name="localTasksCounter" value="82"/>
+    <task id="LOCAL-00082" summary="Visualization sample fixes; added outputs">
+      <created>1682563516561</created>
+      <option name="number" value="00082"/>
+      <option name="presentableId" value="LOCAL-00082"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1682563516561</updated>
+    </task>
+    <task id="LOCAL-00083" summary="Bumped version">
+      <created>1682563802065</created>
+      <option name="number" value="00083"/>
+      <option name="presentableId" value="LOCAL-00083"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1682563802065</updated>
+    </task>
+    <task id="LOCAL-00084" summary="import cleanup &amp; typehint corrections">
+      <created>1683944502477</created>
+      <option name="number" value="00084"/>
+      <option name="presentableId" value="LOCAL-00084"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1683944502477</updated>
+    </task>
+    <option name="localTasksCounter" value="85"/>
     <servers/>
   </component>
   <component name="VcsManagerConfiguration">
-    <MESSAGE value="Whitespace"/>
-    <MESSAGE value="Arborform .itor_next &amp; .itor_children now are monads (i.e., class Furcation)"/>
-    <MESSAGE value="Unit test fix"/>
     <MESSAGE value="Format string typo"/>
     <MESSAGE value="Concrete Itorators all return new or clones"/>
     <MESSAGE value="Cleanup + tags"/>
     <MESSAGE value="Itorator refactor; postorator roll-back"/>
     <MESSAGE value="Itorator function decorations"/>
     <MESSAGE value="Grammer, whitespace, and table-formatting"/>
     <MESSAGE value="import directive cleanups"/>
@@ -594,15 +598,18 @@
     <MESSAGE value="Comment updates"/>
     <MESSAGE value="Minor arborform refactoring"/>
     <MESSAGE value="Doc whitespace updates"/>
     <MESSAGE value="Example cleanups"/>
     <MESSAGE value="Whitespace and comment spelling fixes"/>
     <MESSAGE value="Minor PEP cleanups"/>
     <MESSAGE value="Unit test count update"/>
-    <option name="LAST_COMMIT_MESSAGE" value="Unit test count update"/>
+    <MESSAGE value="Visualization sample fixes; added outputs"/>
+    <MESSAGE value="Bumped version"/>
+    <MESSAGE value="import cleanup &amp; typehint corrections"/>
+    <option name="LAST_COMMIT_MESSAGE" value="import cleanup &amp; typehint corrections"/>
   </component>
   <component name="XDebuggerManager">
     <breakpoint-manager>
       <breakpoints>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/tests/test_xml_parser.py</url>
           <line>15</line>
@@ -671,15 +678,15 @@
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/tests/x_test_itorator.py</url>
           <line>97</line>
           <option name="timeStamp" value="134"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/pawpaw/ito.py</url>
-          <line>1418</line>
+          <line>1420</line>
           <option name="timeStamp" value="137"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/docs/demos/us_constitution/us_constitution.py</url>
           <line>77</line>
           <option name="timeStamp" value="138"/>
         </line-breakpoint>
@@ -751,15 +758,15 @@
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/tests/test_ito_ctor.py</url>
           <line>177</line>
           <option name="timeStamp" value="166"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/pawpaw/ito.py</url>
-          <line>696</line>
+          <line>698</line>
           <option name="timeStamp" value="169"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/tests/test_child_itos.py</url>
           <line>78</line>
           <option name="timeStamp" value="175"/>
         </line-breakpoint>
```

### Comparing `pawpaw-1.0.0rc1/docs/0. Introduction.md` & `pawpaw-1.0.0rc2/docs/0. Introduction.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/docs/1. Segment and Span.md` & `pawpaw-1.0.0rc2/docs/1. Segment and Span.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/docs/2. In Text Object.md` & `pawpaw-1.0.0rc2/docs/2. In Text Object.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/docs/4. Arborform.md` & `pawpaw-1.0.0rc2/docs/4. Arborform.md`

 * *Files 19% similar despite different names*

```diff
@@ -14,72 +14,91 @@
 
 For example, NLP processing typically comprises multiple smaller tasks.  A typically scneario might involve processing a segment by performing these three actions:
 
 1. Split paragraphs
 2. Split sentences
 3. Split words
 
-It might be possible to perform all of these tasks using a single regular expression.  On the other hand, NLP boundary detection tasks are non-trivial.  For reasonable precision and accuracy, a singular regular expression will quickly become too unweildy.
+It might be possible to perform all of these tasks using a single regular expression:
 
-Alternatively, each of these tasks could be performed in a pipeline:
+```mermaid
+flowchart LR
+  text[/text/]
+  text --> re["complex re"]
+  re --> words[/words/]
+```
+Although feasible, NLP boundary detection tasks are non-trivial.  A singular regular expression will quickly become unweildy in the pursuit of reasonable precision and accuracy.
 
+An alternative technique involves isolating each task in a pipeline:
+  
 ```mermaid
 flowchart LR
-  trim --> psplit["paragraph split"]
-  psplit --> wsplit["word split"]
+  text[/text/]
+  text --> psplit["para split"]
+  psplit --> ssplit["sent split"]
+  ssplit --> wsplit["word split"]
+  wsplit --> words[/words/]
 ```
 
-Lateral...
+This technique offers many advantages:
+
+1. Unexpected-side effects are minimized
+2. Tasks can be polymorphic, with run-time delegation 
+3. Additional tasks can be easily inserted as needed
+
+The arborform framework is designed around pipelined parser framework development.  Individual tasks are expressed as ``Itorator`` objects, which can be connected together in both top-down and lateral pipelines:
+
+#### Top Down
 
 ```python
->>> from pawpaw import arborform
+>>> from pawpaw.arborform import Connectors
 >>> itor_para, itor_sent, itor_word = ...
->>> con = aborform.Connectors.Recurse(itor_sent)
->>> itor_para.connections.append(con))
->>> con = aborform.Connectors.Recurse(itor_word)
->>> itor_sent.connections.append(con))
+>>> itor_para.connections.append(Connectors.Recurse(itor_sent))
+>>> itor_para.connections.append(Connectors.Recurse(itor_word))
 ```
 
-Top-down... alternatively:
+#### Lateral
 
 ```python
+>>> from pawpaw.arborform import Connectors
+>>> itor_para, itor_sent, itor_word = ...
 >>> itor_para.connections.append(Connectors.Recurse(itor_sent))
->>> itor_para.connections.append(Connectors.Recurse(itor_word))
+>>> itor_sent.connections.append(Connectors.Recurse(itor_word))
 ```
 
-### Overview
+Pipelines can incorporate *both* top-down and lateral flows, and connections can be predicate-based (for conditional branching), as well as support parent-to-child relationships.  
 
-Pipelines are implemented in arborform using the Python generator/iterator[^python_iter_gen] idiom and achieve a reasonable mixture of performance and memory conservation.  The resulting architecture is highly flexible and scalable, and is highly flexible and scalable for your needs.  The key classes in arborform are:
+Pipeline implementation in arborform makes extensive use of the the Python generator/iterator[^python_iter_gen] idiom, and achieve a reasonable mixture of performance and memory conservation.  The resulting architecture is highly flexible and scalable.  The key classes in arborform are:
 
 * ``Itorator``[^itorator_name]: Generator-based ``Ito`` transformation
 * ``Connector``: Defines connection type between itorators
 * ``Postorator``: Generator-based ``Iterable[Ito]`` consolidation
 
 ## Itorator
 
-The ``Itorator`` class encapsulates a single *transformation* step in a parser pipeline, whereby a given ``Ito`` is transformed into zero, one, or more itos, represented by a ``typing.Iterable[Ito]``.  Examples of transformations you may wish to perform are:
+The ``Itorator`` class encapsulates a single *transformation* step in a parser pipeline, whereby a given ``Ito`` is transformed into zero, one, or more itos, represented by a ``typing.Iterable[Ito]``.  Some examples of transformations include:
 
 * Use ``.str_strip`` to get a shortened ito
 * Split an ito into multiple itos
-* Filter out an ito so that it doesn't show in the final output
+* Exclude (i.e. filter) an ito from the final output
 
-Itorators are callable objects[^callable_object], which allows you to invoke them using simple function syntax.  The single input parameter is an ``Ito``, and the return type is a generator, which you can iterate over, unpack into a container, etc:
+Itorators are callable objects[^callable_object] are are invoked using simple function syntax.  The single input parameter is an ``Ito``, and the return type is a generator, which you can iterate over, unpack into a container, etc:
 
 ```python
 >>> from pawpaw import Ito, arborform
 >>> s = 'Hello, world!'
 >>> i = Ito(s)
 >>> i  # Starting ito has no .desc
 Ito('Hello, world!', 0, 13, None)
 >>> itor_desc = arborform.Desc('changed')  # Desc itorator: changes .desc property
 >>> next(itor_desc(i))  # Invoke itorator and get first item from pipeline
 Ito('Hello, world!', 0, 13, 'changed')
 ```
 
-When invoked, an itorator clones the input Ito, ensured that it is left unaltered:
+When invoked, an itorator clones the input Ito, which guarrantees that it is unaltered by the pipeline:
 
 ```python
 >>> i  # Original remains unmodified
 Ito('Hello, world!', 0, 13, None)
 ```
 
 Transformations are performed in the ``._transform`` method, which is abstract for the base class ``Itorator``.  The ``._transform`` method is not intended to be called directly, rather, it is available for you to override in derived classes.  Several concrete itorators with implementations for ``._transform`` are available:
@@ -152,14 +171,202 @@
   Itorator <|-- Filter
   Itorator <|-- Desc
   Itorator <|-- ValueFunc
   Itorator <|-- Split
   Itorator <|-- Extract
 ```
 
+## Concrete Itorator Types
+
+### Reflect
+
+The ``Reflect`` itorator uncondintionally reflects back an input ito:
+
+```python
+def _transform(self, ito: Ito) -> Types.C_IT_ITOS:
+    yield ito
+```
+
+### Filter
+
+The ``Filter`` itorator reflects back the input ito when it matches a given predicate filter:
+
+```python
+def _transform(self, ito: Ito) -> Types.C_IT_ITOS:
+    if self._filter(ito):
+        yield ito
+```
+
+The predicate filter is specified in the ctor:
+
+```python
+>>> from pawpaw import arborform, Ito
+>>> ito_filter = arborform.Filter(lambda ito: str(ito).>>> >>> isnumeric())
+>>> for ito in Ito('1a2'):
+        for r in ito_filter(ito):
+          print(r)
+1
+2
+```
+
+### Desc
+
+The ``Desc`` itorator changes the .desc of an ito and reflects it back:
+
+```python
+def _transform(self, ito: Ito) -> Types.C_IT_ITOS:
+    if self._filter(ito):
+        ito.desc = self._desc_func(ito)
+        yield ito
+```
+
+The value for the assignment is specified in the ctor:
+
+```python
+>>> from pawpaw import arborform, Ito
+>>> ito_desc = arborform.Desc('changed')
+>>> ito = Ito('abc', desc='original')
+>>> rv = next(ito_desc(ito))
+>>> print(rv.desc)
+changed
+```
+
+### ValueFunc
+
+The ``ValueFunc`` itorator changes the .value_func of an ito and reflects it back:
+
+```python
+def _transform(self, ito: Ito) -> Types.C_IT_ITOS:
+    if self._filter(ito):
+        ito.value_func = self.f
+        yield ito
+```
+
+The value for the assignment is specified in the ctor:
+
+```python
+>>> from pawpaw import arborform, Ito
+>>> ito_vf = arborform.ValueFunc(lambda ito: int(str(ito)))
+>>> ito = Ito('2')
+>>> rv = next(ito_vf(ito))
+>>> print(rv.value() + 3)
+5
+```
+
+### Split
+
+***This documentation has not yet been written***
+
+### Extract
+
+The ``Extract`` itorator applies a regular expression to an ito via ``.regex_finditer``.  Each match is returned back as a pawpaw tree:
+
+```python
+import regex 
+from pawpaw import arborform, Ito, visualization
+s = 'nine 9 ten 10 eleven 11 TWELVE 12 thirteen 13'
+pat = r"""
+(?:
+    (?P<phrase>
+        (?P<word>
+            (?P<char>\w)+
+        )
+        \ 
+        (?P<number>
+            (?P<digit>\d)+
+        )
+    )\s*
+)+
+"""
+re = regex.compile(pat, regex.VERBOSE)
+ito_extract = arborform.Extract(re)
+rv = next(ito_extract(Ito(s)))
+tree_vis = visualization.pepo.Tree()
+print(tree_vis.dumps(rv))
+```
+
+results in:
+
+```
+(0, 6) 'phrase' : 'nine 9'
+├──(0, 4) 'word' : 'nine'
+│  ├──(0, 1) 'char' : 'n'
+│  ├──(1, 2) 'char' : 'i'
+│  ├──(2, 3) 'char' : 'n'
+│  └──(3, 4) 'char' : 'e'
+└──(5, 6) 'number' : '9'
+   └──(5, 6) 'digit' : '9'
+
+(7, 13) 'phrase' : 'ten 10'
+├──(7, 10) 'word' : 'ten'
+│  ├──(7, 8) 'char' : 't'
+│  ├──(8, 9) 'char' : 'e'
+│  └──(9, 10) 'char' : 'n'
+└──(11, 13) 'number' : '10'
+   ├──(11, 12) 'digit' : '1'
+   └──(12, 13) 'digit' : '0'
+
+(14, 23) 'phrase' : 'eleven 11'
+├──(14, 20) 'word' : 'eleven'
+│  ├──(14, 15) 'char' : 'e'
+│  ├──(15, 16) 'char' : 'l'
+│  ├──(16, 17) 'char' : 'e'
+│  ├──(17, 18) 'char' : 'v'
+│  ├──(18, 19) 'char' : 'e'
+│  └──(19, 20) 'char' : 'n'
+└──(21, 23) 'number' : '11'
+   ├──(21, 22) 'digit' : '1'
+   └──(22, 23) 'digit' : '1'
+
+(24, 33) 'phrase' : 'TWELVE 12'
+├──(24, 30) 'word' : 'TWELVE'
+│  ├──(24, 25) 'char' : 'T'
+│  ├──(25, 26) 'char' : 'W'
+│  ├──(26, 27) 'char' : 'E'
+│  ├──(27, 28) 'char' : 'L'
+│  ├──(28, 29) 'char' : 'V'
+│  └──(29, 30) 'char' : 'E'
+└──(31, 33) 'number' : '12'
+   ├──(31, 32) 'digit' : '1'
+   └──(32, 33) 'digit' : '2'
+
+(34, 45) 'phrase' : 'thirteen 13'
+├──(34, 42) 'word' : 'thirteen'
+│  ├──(34, 35) 'char' : 't'
+│  ├──(35, 36) 'char' : 'h'
+│  ├──(36, 37) 'char' : 'i'
+│  ├──(37, 38) 'char' : 'r'
+│  ├──(38, 39) 'char' : 't'
+│  ├──(39, 40) 'char' : 'e'
+│  ├──(40, 41) 'char' : 'e'
+│  └──(41, 42) 'char' : 'n'
+└──(43, 45) 'number' : '13'
+   ├──(43, 44) 'digit' : '1'
+   └──(44, 45) 'digit' : '3'
+```
+
+Notes:
+
+* group_filter defaults to only **named** groups, but it can be set to nothing (i.e., allow *all* groups.)  Note that if all groups are allowed, then the output will always consist of a tree whose root is the entire match (group 0), with all other sub-groups present as descendants
+
+* If a group has a name, it will be used as the group key.  Otherwise, its index will be used.
+
+* Even if you filter groups (named or otherwise) in your output, you can still access them them in the match:
+
+```python
+>>> import regex
+>>> from pawpaw import Ito, arborform
+>>> s = 'AB'
+>>> re = regex.compile(r'(.)(?<foo>.)')
+>>> d = lambda ito, match, group: match.group(1)  # Used first (unnamed) group as descriptor for 'foo'
+>>> extract = arborform.Extract(re, desc_func=d)
+>>> next(extract(Ito(s)))
+Ito('AB', 1, 2, 'A')
+```
+
 ## Connector
 
 Data flow between Itorators is indicated through ``Connector`` objects.  
 
 A connector object consists of a single ``Itorator`` and an optional predicate[^predicate]:
 
 ```mermaid
@@ -247,17 +454,36 @@
 | ``Connectors.Children.Add`` | 1. Caches result of ``f(cur)``<br>2. Adds cached result to cur.children<br>3. Yields cached result<br>4. Breaks out of inner loop | adding children |
 | ``Connectors.Children.AddHierarchical`` |  1. Caches result of ``f(cur)``<br>2. Adds cached result hierarchically to cur.children<br>3. Yields cached result<br>4. Breaks out of inner loop | adding children  hierarchically |
 | ``Connectors.Children.Replace`` | 1. Caches result of ``f(cur)``<br>2. Clears cur.children<br>3. Adds cached result to cur.children<br>4. Yields cached result<br>5. Breaks out of inner loop | adding or replacing children |
 | ``Connectors.Children.Delete`` | 1. Caches result of ``f(cur)``<br>2. Calls ``cur.children.delete`` for each item in cached result<br>3. Yield cached result<br>4. Breaks out of inner loop | deleting children |
 
 If an itorator has a ``.postorator``, the result the entire flow is wrapped in an iterator and passed to it.
 
+### ``Connectors.Recurse``
+
+The ``Recurse`` connector passes a flow to a second itorator.  The results of the second are then fed to the next itorator in the pipeline.
+
+Note that the ``Recurse`` connector is useful when designing a *sub-pipeline* that has multiple end-points and whose output needs to be sent to another itorator:
+
+```mermaid
+flowchart LR
+  A["A()"] -->|"Connectors.Recurse"| sub-pipeline
+  subgraph sub-pipeline
+    direction LR
+    B["B()"] --> C["C()"]
+    B --> D["D()"]
+  end
+  sub-pipeline -.-> E[...]
+```
+
+By using a ``Sub`` connector, the output of both C and D will be fed into the next itorator in a connections list.
+
 ### ``Connectors.Delegate``
 
-YieldBreak is the cannonical connector type in that it delegates all subsequent flow processing to another itorator and yields the results.
+The ``Delegate`` connector passes flow to a second itorator.  The results of the second are then immediately yielded, *without passing them to any subsequent itorators* in the pipeline.
 
 ```python
 >>> from pawpaw import Ito, arborform, visualization
 >>> s = 'Hello, world!'
 >>> i = Ito(s)
 >>> itor_reflect = arborform.Reflect()  # Reflects current ito (no transformation)
 >>> vis_compact = visualization.pepo.Compact()
@@ -269,40 +495,32 @@
 >>> con = arborform.Connectors.Delegate(itor_desc)
 >>> itor_reflect.connections.append(con)
 >>> for result in itor_reflect(i):
 ...    print(vis_compact.dumps(result))
 1: (0, 13) 'Changed' : 'Hello, world!'
 ```
 
-### ``Connectors.Recurse``
-
-The ``Recurse`` connector is useful when designing a *sub-pipeline* that has multiple end-points and whose output needs to be sent to another itorator:
-
-```mermaid
-flowchart LR
-  A["A()"] -->|"Connectors.Recurse"| sub-pipeline
-  subgraph sub-pipeline
-    direction LR
-    B["B()"] --> C["C()"]
-    B --> D["D()"]
-  end
-  sub-pipeline -.-> E[...]
-```
-
-By using a ``Sub`` connector, the output of both C and D will be fed into the next itorator in a connections list.
-
 ### ``Connectors.Subroutine``
 
-This type is also aliases as ``Sub``...
+The ``Subroutine`` connector passes flow to an itorator but does *nothing* with the results.  The incoming flow is then then fed to the next itorator in the pipeline.  This type of connection is useful for diagnostic purposes.  For example, the flow could be passed to a visualization routine that displays the current flow status.
 
-TODO
+Alternatively, the receiving itorator can perform operations on the flow Itos in a trasnparant manner.
 
 ### ``Connectors.Children``
 
-Several connections apply results to the child of a given ito.  For example, an ``Itorator`` that performs a word split can pass its output to another ``Itorator`` that performs a char split.  The overall output will consist of *trees* whose roots are words and leaves are chars:
+When you need to apply the output of an itorator *to the children* of a given input Ito, several connections types are available:
+
+| Connectors.Children Type | Description | Pseudocode |
+|:---:|:---:|:---|
+| Add | Adds the results to the input ito's children | input_ito.children.add(*results) |
+| AddHierarchical | Adds the results hierarchically to the input ito's children | input_ito.children.add_hierarchical(*results) |
+| Replace | Replaces the results to the input ito's children | input_ito.children.clear()<br/>input_ito.children.add(*results)|
+| Delete | Removes the results from the input ito's children | for r in results:<br/>&nbsp;&nbsp;&nbsp;&nbsp;input_ito.children.remove(r)|
+
+#### Example:
 
 ```python
 >>> from pawpaw import Ito, arborform, visualization
 >>> s = 'Hello, world!'
 >>> i = Ito(s)
 >>> split_words = arborform.Itorator.wrap(lambda ito: ito.str_split())  # str split
 >>> split_chars = arborform.Itorator.wrap(lambda ito: [*ito])  # extract char itos
@@ -324,134 +542,29 @@
 ├──(8, 9) 'None' : 'o'
 ├──(9, 10) 'None' : 'r'
 ├──(10, 11) 'None' : 'l'
 ├──(11, 12) 'None' : 'd'
 └──(12, 13) 'None' : '!'
 ```
 
-## DOCUMENTATION BEYOND THIS POINT IS NOW DEPRECATED
-
-The ``.itor_next`` property is feeds an ito sequence as a *lateral* flow.  This is the most basic type of pipeline connection:
-
-```mermaid
-flowchart LR
-  A["A()"] -->|".iter_next"| B["B()"]
-  B -.-> C[...]
-```
-
-## Concrete Itorator Types
-
-### Extract
-
-Notes:
-
-* group_filter defaults to only **named** groups, but it can be set to nothing (i.e., allow *all* groups.)  Note that if all groups are allowed, then the output will always consist of a tree whose root is the entire match (group 0), with all other sub-groups present as descendants
-
-* If a group has a name, it will be used as the group key.  Otherwise, its index will be used.
-
-* Even if you filter groups (named or otherwise) in your output, you can still access them them in the match:
-
-```python
->>> import regex
->>> from pawpaw import Ito, arborform
->>> s = 'AB'
->>> re = regex.compile(r'(.)(?<foo>.)')
->>> d = lambda ito, match, group: match.group(1)  # Used first (unnamed) group as descriptor for 'foo'
->>> extract = arborform.Extract(re, desc_func=d)
->>> next(extract(Ito(s)))
-Ito('AB', 1, 2, 'A')
-```
-
 ## Advanced Chaining
 
-### Simple Pipeline Conections
-
-The most frequent pipeline connections are a) unconditional flow to a single ``Itorator`` and b) conditional flow to a single ``Itorator`` (otherwise None.)  The ``.itor_next`` and ``.itor_children` properties are highly overloaded, and directly support setting these two connection types:
-
-```python
->>> itor_1.itor_next = itor_2  # unconditional lateral flow (itor_1 → itor_2)
->>> itor_1.itor_child = lambda ito: ito.desc = 'parent', itor_3  # conditional downward flow (itor_1 ↓ itor_2)
-```
-
-### Chaining Internals
-
-Internally, the ``.itor_next`` and ``.itor_children`` properties have overloaded setters that support this type of varied syntax.  The underlying data for both of these is a specialized list of *monad-like* predicate-value pairs.  Each pair is modeled in Pawpaw as the class ``PredicatedValue``.  Predicates are Python callable objects with a single parameter, ``Ito``, and which return a ``bool``.  Values are either an ``Itorator`` or ``None``.
-
-```mermaid
-classDiagram
-  class PredicatedValue{
-      +predicate typing.Callable[[Ito], bool]
-      +value Itorator | None
-  }
-```
-
-The specialized list of ``PredicatedValue`` is modeled in Pawpaw as class ``Furcation``[^furcation_name].  Evaluation of a ``Furcation`` for a given ``Ito`` is done by evaluating each predicate in sequential order until a value of ``True`` is obtained, at which point the associated value (an ``Itorator`` or ``None``) is returned.  If no predicate returns ``True``, then ``None`` is returned.
-
-```mermaid
-flowchart LR
-  ito --> count[i = 0]
-  subgraph "furcation(ito)"
-    direction TB
-    count --> loop{"i #10875; len(pvs)"}
-    loop --->|True| None
-    loop -->|False| p{"pvs[i].predicate(ito)"}
-    p --> |True| v["pvs[i].value"]
-    p --> |False| inc["i += 1"]
-    inc --> loop
-  end
-  None --> return
-  v --> return
-```
-
-Although complex, this furcation-based architecture has several key advantages:
-
-* Better run-time type checks
-* Pipeline visualization
-
-The ``.itor_next`` and ``.itor_children` properties setters actually perform a transformation based on the value type passed, and initialize the furcation list with the result:
-
-|         Value Type         |               Transformation               |  len(Furcation)  |
-|:--------------------------:|:------------------------------------------:|:----------------:|
-|            None            |                    N/A                     |        0         |
-|          Itorator          | PredicateValue(Furcation.tautology, value) |        1         |
-| tuple(Predicate, Itorator) |     PredicateValue(value[0], value[1])     |        1         |
-|         Predicate          |        PredicateValue(value, None)         |        1         |
-|       PredicateValue       |                   value                    |        1         |
-
-Note that ``PredicateValue`` with a ``.value`` of None is perfectly valid.  When only an itorator is passed, a placeholder predicate, ``Furcation.tautology``, is used[^tautology].  In such a case, the furcation evaluation always returns the given ``Itorator``.
-
-For more complex, multi-predicate control flows, simply use standard list accessors methods (e.g. ``.append``, ``.extend``, ``.insert``, etc.) of the ``Furcation`` object.  These methods are also overloaded, allowing you to pass either:
-
-1. ``Predicate``
-2. ``Itorator``
-3. ``tuple[Predicate, Itorator]``
-4. ``PredicatedValue``
-
-Example:
-
-```python
->>> itor_1.itor_next = itor_2  # init
->>> itor_1.itor_next.append((func_1, itor_3)) # append tuple
->>> itor_1.itor_next.append(func_2) # append predicate
->>> itor_1.itor_next.append(itor_4) # append itorator
-```
-
 ### Sub-pipelines
 
 Complex connections will result in an ``Itorator`` having *multiple* flow paths.  For example:
 
 ```mermaid
 flowchart LR
   A --> B
   B --> C_1
   B --> C_2
   A --> D_1
   D_1 --> D_2
 ```
-If this is your entire pipeline, then calling ``.traverse`` on A yield the output of either C_1, C_2, or D_2, as expected, and nothing more need be done.
+If this is your entire pipeline, then invoking A will yield the output of either C_1, C_2, or D_2, as expected, and nothing more need be done.
 
 Alternatively, sometimes you'll need to *merge* flow paths.  For example, you might need a final processing step, Z, be performed on all three paths:
 
 ```mermaid
 flowchart LR
   A --> B
   B --> C_1
@@ -459,76 +572,40 @@
   A --> D_1
   D_1 --> D_2
   C_1 --> Z
   C_2 --> Z
   D_2 --> Z
 ```
 
-You can do this by adding Z to each of the three itorators' ``.itor_next`` furcations:
+You can do this by making A a ``Sub`` to it's parent.  The output, whether from C_1, C_2, or D_2 will be returned back up to the stack to A's parent.  Alternatively, if A has no parent, a stub ``Reflect`` itorator can be used instead:
 
 ```python
->>> A.itor_next = F1, B
->>> A.itor_next.append(D_1)
->>> B.itor_next = F2, C_1
->>> B.itor_next.append(C_2)
->>> D_1.itor_next = D_2
->>> # Merge all three branches
->>> C_1.itor_next = Z
->>> C_2.itor_next = Z
->>> D_2.itor_next = Z
+>>> itor_A = ...
+>>> itor_reflect = arborform.Reflect(...)
+>>> con = arborform.Connectors.Sub(itor_reflect)
+>>> itor_A.connections.append(con)
+>>> itor_B = ...
+>>> con = arborform.Connectors.Delegate(itor_B, some_predicate)
+>>> itor_reflect.connections.append(con)
+>>> ...
 ```
 
-Although valid, this approach can problematic for complex pipelines.  As you develop your pipelines, and paths are being added, altered, and deleted, you will need to be vigilant about removing and re-adding the final merge step for all affected branches.  More than likely, you will overlook one and your pipeline will be incorrect.
-
-Alternatively, these complex chains can be managed using ``.itor_sub``, which is used to define a encapsulated *sub-pipeline* with a **single output**:
-
 ```mermaid
 flowchart LR
-A -->|.itor_sub| S
-  S -->|.itor_sub| B
-  S -->|.itor_sub| D.1
-subgraph S[sub-pipeline]
-  direction LR
-  A.1(["."]) --> B
-  A.1(["."]) --> D.1
-  B -->|.itor_next| C.1
-  B -->|.itor_next| C.2
-  D.1 -->|.itor_next| D.2
-end
-  S -->|.itor_next| Z
-  ```
-
-The code for this is as follows:
-
-```python
->>> A.itor_sub = F1, B
->>> A.itor_sub.append(D_1)
->>> B.itor_next = F2, C_1
->>> B.itor_next.append(C_2)
->>> D_1.itor_next = D_2
->>> A.itor_next = Z
-```
-
-Creating a wrapped ``Itorator`` results in a single end-point to which you can connect to.  As you revise the sub-pipeline, the final merged connection is unaffected, and you are relieved from having to manage the merge code for each and every sub-path:
-
-```python
->>> A.itor_next = F1, B
->>> A.itor_next.append(D_1)
->>> B.itor_next = F2, C_1
->>> B.itor_next.append(C_2)
->>> C_2.itor_next = C_3  # new node
->>> D_1.itor_next = D_2
->>> # Wrap
->>> wrapped = Itorator.wrap(A)
->>> wrapped.itor_next = Z  # revised sub-pipeline still merged correctly
+  A --> Stub
+  Stub --> B
+  B --> C_1
+  B --> C_2
+  Stub --> D_1
+  D_1 --> D_2
 ```
 
 ## Postorator
 
-Coming soon...
+***This documentation has not yet been written***
 
 ### Postorator Class Diagram
 
 ```mermaid
 classDiagram
   class Postorator{
     +tag str | None
```

### Comparing `pawpaw-1.0.0rc1/docs/5. Traversal & Query.md` & `pawpaw-1.0.0rc2/docs/5. Traversal & Query.md`

 * *Files 3% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 | ``'**'``       | descendants    | All descendants of the current node, starting with the children and ending with leaves |
 | ``'***'``      | leaves         | Descendants of the current node that have no descendants themselves |
 | ``'<<<'``      | preceeding     | Nodes that are *before* the current node, *includes* prior siblings and *excludes* ancestors & descendants |
 | ``'<<'``       | prior siblings | Nodes *before* the current node that have the same parent |
 | ``'<'``        | prior sibling  | The nearest node *before* the current node that has the same parent |
 | ``'>'``        | next sibling   |  The nearest node *after* the current node that has the same parent |
 | ``'>>'``       | next siblings  |  Nodes *after* the current node that have the same parent |
-| ``'>>>'``      | following      | Nodes that are *after* the current node, *includes* prior siblings and *excludes* ancestors & descendants |
+| ``'>>>'``      | following      | Nodes that are *after* the current node, *includes* next siblings and *excludes* ancestors & descendants |
 
 #### Examples
 
 ```python
  '*'    # all children; equivalent to iter(i.children)
  '*/*'  # all grandchildren; equivalent to iter(gc for c in i.children for gc in c.children)
  '../*' # all siblings and self: equivalent to i.parent.children
@@ -196,27 +196,54 @@
 | Key                   |          Alt Keys(s)          | Meaning                                                                 | Example(s)                             |
 | :----:                |:-----------------------------:| :---                                                                    | :---                                   |
 | ``'desc'``            |            ``'d'``            | One or more ``str`` values used to match againss ``.desc`` of axis; values must be separated with commas, literal commas must be escaped | ``[d:number]``<br />``[d:word,char]`` |
 | ``'str'``          |            ``'s'``            | A ``str`` used to match against ``str()`` of axis | ``[s:foo]``<br />``[s:foo,goo]``|
 | ``'str-casefold'`` |   ``'scf'``,<br />``'lcs'``   | Checks if casefolded ``str()`` of axis matches casefolded value | ``[scf:FoO,GoO]`` |
 | ``'str-casefold-ew'`` | ``'scfew'``,<br />``'lcsew'`` | Checks if casefolded ``str()`` of axis ends with with casefolded value | ``[scfew:a,1]`` |
 | ``'str-casefold-sw'`` | ``'scfsw'``,<br />``'lcssw'`` | Checks if casefolded ``str()`` of axis starts with with casefolded value | ``[scfsw:a,1]`` |
-| ``'str-ew'`` |           ``'sew'``           | Checks if ``str()`` of axis starts with value | ``[scfew:a,1]`` |
-| ``'str-sw'`` |           ``'ssw'``           | Checks if ``str()`` of axis ends with with value | ``[scfsw:a,1]`` |
-| ``'index'`` |            ``'v'``            | One or more ``int`` tuples consisting of a *start* and optional *stop* values; matches against the enumeration index(ices) of the axis; start and stop must be non-negative integers; start and stop behave like a *slice*, i.e., stop should be *one more than* the last desired value; tuples must be separated with commas; *start* and *stop* must be separated with hyphens; a start followed by a hypen *without* a stop will be intepreted as ≥ , e.g. ``[i:5-]`` means *index(ices) greater than or equal to 5* | ``[i:1]``<br />``[i:2,3,4]``<br />``[i:2-3]``<br />``[i:2,5-7]``<br />``[i:0,5-,3]`` |
-| ``'predicate'`` |            ``'p'``            | Key for filter function used to match against axis A ``str`` used as a key to entry in dictionary of type:     typing.Dict[str, typing.Callable[[int, Ito], bool]  The value retrieved from the ``dict`` use used as a filter against the axis | ``[p:key1]``<br />``[p:key1,key2]`` |
+| ``'str-ew'`` |           ``'sew'``           | Checks if ``str()`` of axis ends with value | ``[scfew:a,1]`` |
+| ``'str-sw'`` |           ``'ssw'``           | Checks if ``str()`` of axis starts with with value | ``[scfsw:a,1]`` |
+| ``'index'`` |            ``'i'``            | One or more ``int`` tuples consisting of a *start* and optional *stop* values; matches against the enumeration index(ices) of the axis; start and stop must be non-negative integers; start and stop behave like a *slice*, i.e., stop should be *one more than* the last desired value; tuples must be separated with commas; *start* and *stop* must be separated with hyphens; a start followed by a hypen *without* a stop will be intepreted as ≥ , e.g. ``[i:5-]`` means *index(ices) greater than or equal to 5* | ``[i:1]``<br />``[i:2,3,4]``<br />``[i:2-3]``<br />``[i:2,5-7]``<br />``[i:0,5-,3]`` |
+| ``'predicate'`` |            ``'p'``            | Key for filter function used to match against axis A ``str`` used as a key to entry in dictionary of type: ``typing.Dict[str, typing.Callable[pawpaw.Types.C_EITO, bool]]``  The value retrieved from the ``dict`` use used as a filter against the axis | ``[p:key1]``<br />``[p:key1,key2]`` |
 | ``'value'`` |            ``'v'``            | A ``str`` used as a key to entry in dictionary of type::      typing.Dict[str, typing.Any]  The value retrieved from the ``dict`` is used to match against the ``.value()`` of the axis | ``[p:key]``<br />``[p:key1, key2]`` |
 
-Parentheses are allowed to perform logical grouping:
+#### Parentheses
 
-#### Examples
+Plumule supports parentheses for to perform logical grouping:
+
+```python
+# all children having .desc equal to 'word' or 'number'
+'*[d:word,number]'  
+
+# all descendants with .desc not 'word', or with
+# .desc 'word' and .__str__() 'ten'
+'**[~d:word] | ([d:word] & [s:ten])'  
+```
+
+#### Predicates
+
+Plumule supports arbitrary predicates as part of a query.  Predicates are refererred to in a plumule query via the ``'predicate'`` (or ``'p'``) key, whose associated value(s) are keys in a dictionary of type:
+
+```python
+typing.Dict[str, typing.Callable[pawpaw.Types.C_EITO, bool]] 
+```
+
+Predicates allow you to use your own code as part of a query filter:
 
 ```python
-'*[d:word,number]'  # all children having .desc equal to 'word' or 'number'
-'**[~d:word] | ([d:word] & [s:ten])'  # all descendants with .desc not 'word', or with .desc 'word and .__str__() 'ten'
+>>> import pawpaw
+>>> ito = pawpaw.Ito('ABcd12Ef')
+>>> ito.children.add(*ito)
+>>> query = '*[p:isnumeric]'
+>>> predicates = {}
+>>> predicates['isnumeric'] = lambda ei: ei.ito.str_isnumeric()
+>>> for i in ito.find_all(query, predicates=predicates):
+...     print(i)
+1
+2
 ```
 
 ### Subqueries
 
 The subqueries component of a phrase consists of one or more subquery expressions, separated with the same logical operators used for filters, and grouped as needed with parentheses:
 
 ```
```

### Comparing `pawpaw-1.0.0rc1/docs/6. Xml.md` & `pawpaw-1.0.0rc2/docs/6. Xml.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/docs/7. NLP.md` & `pawpaw-1.0.0rc2/docs/7. NLP.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/docs/8. Serialization.md` & `pawpaw-1.0.0rc2/docs/8. Serialization.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/docs/Pawpaw Cookbook.md` & `pawpaw-1.0.0rc2/docs/Pawpaw Cookbook.md`

 * *Files 25% similar despite different names*

```diff
@@ -69,14 +69,64 @@
    ├──(46, 52) 'Word' : 'Sleepy'
    ├──(53, 59) 'Word' : 'Hollow'
    ├──(61, 63) 'Word' : 'by'
    ├──(64, 74) 'Word' : 'Washington'
    └──(75, 81) 'Word' : 'Irving'
 ```
 
+### Extract children and then extract a second set of children based on the leftover space
+
+**Code:**
+
+```python
+from pawpaw import Ito, arborform, visualization
+import regex
+
+s = 'It measures 10 <!--inches--> long <!--front to back-->'
+
+itor_self = arborform.Reflect()
+
+pat = r"""
+(?<comment>\<\!\-\-
+    (?<value>.*?)
+\-\-\>)
+"""
+re = regex.compile(pat, regex.VERBOSE | regex.DOTALL)
+itor_comment = arborform.Extract(re)
+con = arborform.Connectors.Children.Add(itor_comment)
+itor_self.connections.append(con)
+
+itor_invert_children = arborform.Itorator.wrap(lambda ito: Ito.from_gaps(ito, ito.children, False))
+con = arborform.Connectors.Children.Add(itor_invert_children)
+itor_self.connections.append(con)
+
+re = regex.compile(r'(?<token>\S+)', regex.DOTALL)
+itor_token = arborform.Extract(re)
+con = arborform.Connectors.Delegate(itor_token)
+itor_invert_children.connections.append(con)
+
+ito = Ito(s, desc='phrase')
+v_tree = visualization.pepo.Tree()
+print(v_tree.dumps(next(itor_self(ito))))
+```
+
+**Output:**
+
+```
+(0, 54) 'phrase' : 'It measures 10 <!--i…!--front to back-->'
+├──(0, 2) 'token' : 'It'
+├──(3, 11) 'token' : 'measures'
+├──(12, 14) 'token' : '10'
+├──(15, 28) 'comment' : '<!--inches-->'
+│  └──(19, 25) 'value' : 'inches'
+├──(29, 33) 'token' : 'long'
+└──(34, 54) 'comment' : '<!--front to back-->'
+   └──(38, 51) 'value' : 'front to back'
+```
+
 ## XML
 
 ### Get spans for elements:
 
 **Code:**
 
 ```python
```

### Comparing `pawpaw-1.0.0rc1/docs/Using Pawpaw with nltk.md` & `pawpaw-1.0.0rc2/docs/Using Pawpaw with nltk.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/docs/demos/Q&A/description.md` & `pawpaw-1.0.0rc2/docs/demos/Q&A/description.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/docs/demos/Q&A/solution.py` & `pawpaw-1.0.0rc2/docs/demos/Q&A/solution.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/docs/demos/class_grades/description.md` & `pawpaw-1.0.0rc2/docs/demos/class_grades/description.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/docs/demos/class_grades/input.txt` & `pawpaw-1.0.0rc2/docs/demos/class_grades/input.txt`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/docs/demos/class_grades/parser_verbose.py` & `pawpaw-1.0.0rc2/docs/demos/class_grades/parser_verbose.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/docs/demos/class_grades/solution.py` & `pawpaw-1.0.0rc2/docs/demos/class_grades/solution.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/docs/demos/gettysburg_address/gettysburg_address.txt` & `pawpaw-1.0.0rc2/docs/demos/gettysburg_address/gettysburg_address.txt`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/docs/demos/us_constitution/us_constitution.py` & `pawpaw-1.0.0rc2/docs/demos/us_constitution/us_constitution.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/docs/demos/us_constitution/us_constitution.txt` & `pawpaw-1.0.0rc2/docs/demos/us_constitution/us_constitution.txt`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/images/pawpaw.png` & `pawpaw-1.0.0rc2/images/pawpaw.png`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/pawpaw/__init__.py` & `pawpaw-1.0.0rc2/pawpaw/__init__.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/pawpaw/_type_magic.py` & `pawpaw-1.0.0rc2/pawpaw/_type_magic.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/pawpaw/_version.py` & `pawpaw-1.0.0rc2/pawpaw/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import string
 import typing
 
 import regex
 
-__version__ = '1.0.0rc1'
+__version__ = '1.0.0rc2'
 """The str literal that build, setup, documentation, and other tools typically want."""
 
 class Version:
     _canonical_re = regex.compile(r'^([1-9][0-9]*!)?(0|[1-9][0-9]*)(\.(0|[1-9][0-9]*))*((a|b|rc)(0|[1-9][0-9]*))?(\.post(0|[1-9][0-9]*))?(\.dev(0|[1-9][0-9]*))?(?:\+[a-z0-9]+(?:[-_\.][a-z0-9]+)*)?$')
     """This pattern taken from https://peps.python.org/pep-0440/#appendix-b-parsing-version-strings-with-regular-expressions
     and expanded to support optional "local version identifier" (see https://peps.python.org/pep-0440/#local-version-identifiers)."""
```

### Comparing `pawpaw-1.0.0rc1/pawpaw/errors.py` & `pawpaw-1.0.0rc2/pawpaw/errors.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/pawpaw/infix.py` & `pawpaw-1.0.0rc2/pawpaw/infix.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/pawpaw/ito.py` & `pawpaw-1.0.0rc2/pawpaw/ito.py`

 * *Files 0% similar despite different names*

```diff
@@ -393,32 +393,34 @@
             child._parent = self
 
     # endregion
 
     # region JSON
 
     class JsonEncoderStringless(json.JSONEncoder):
-        def default(self, o: typing.Any) -> typing.Dict:
+        @classmethod
+        def default(cls, o: typing.Any) -> dict[str, typing.Any]:
             return {
                 '__type__': 'Ito',
                 'span': o._span,
                 'desc': o.desc,
-                'children': [self.default(c) for c in o.children]
+                'children': [cls.default(c) for c in o.children]
             }
 
     class JsonEncoder(json.JSONEncoder):
-        def default(self, o: typing.Any) -> typing.Dict:
+        @classmethod
+        def default(cls, o: typing.Any) -> dict[str, typing.Any]:
             return {
                 '__type__': 'typing.Tuple[str, Ito]',
                 'string': o.string,
                 'ito': Ito.JsonEncoderStringless().default(o)
             }
 
     @classmethod
-    def _json_decoder_stringless(cls, obj: typing.Dict) -> pawpaw.Ito | typing.Dict:
+    def _json_decoder_stringless(cls, obj: typing.Dict) -> pawpaw.Ito | dict[str, typing.Any]:
         if (t := obj.get('__type__')) is not None and t == 'Ito':
             rv = cls('', desc=obj['desc'])
             rv._span = Span(*obj['span'])
             rv.children.add(*obj['children'])
             return rv
         else:
             return obj
@@ -426,15 +428,15 @@
     @classmethod
     def json_decode_stringless(cls, string: str, json_data: str) -> pawpaw.Ito:
         rv = json.loads(json_data, object_hook=cls._json_decoder_stringless)
         rv._set_string(string)
         return rv
 
     @classmethod
-    def json_decoder(cls, obj: typing.Dict) -> pawpaw.Ito | typing.Dict:
+    def json_decoder(cls, obj: typing.Dict) -> pawpaw.Ito |  dict[str, typing.Any]:
         if (t := obj.get('__type__')) is not None:
             if t == 'typing.Tuple[str, Ito]':
                 rv = obj['ito']
                 rv._string = obj['string']
                 return rv
             elif t == 'Ito':
                 return cls._json_decoder_stringless(obj)
```

### Comparing `pawpaw-1.0.0rc1/pawpaw/span.py` & `pawpaw-1.0.0rc2/pawpaw/span.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/pawpaw/util.py` & `pawpaw-1.0.0rc2/pawpaw/util.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/pawpaw/arborform/itorator/desc.py` & `pawpaw-1.0.0rc2/pawpaw/arborform/itorator/desc.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/pawpaw/arborform/itorator/extract.py` & `pawpaw-1.0.0rc2/pawpaw/arborform/itorator/extract.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/pawpaw/arborform/itorator/filter.py` & `pawpaw-1.0.0rc2/pawpaw/arborform/itorator/filter.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/pawpaw/arborform/itorator/itorator.py` & `pawpaw-1.0.0rc2/pawpaw/arborform/itorator/itorator.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/pawpaw/arborform/itorator/split.py` & `pawpaw-1.0.0rc2/pawpaw/arborform/itorator/split.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/pawpaw/arborform/itorator/value_func.py` & `pawpaw-1.0.0rc2/pawpaw/arborform/itorator/value_func.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/pawpaw/arborform/postorator/postorator.py` & `pawpaw-1.0.0rc2/pawpaw/arborform/postorator/postorator.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/pawpaw/arborform/postorator/stacked_reduce.py` & `pawpaw-1.0.0rc2/pawpaw/arborform/postorator/stacked_reduce.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/pawpaw/arborform/postorator/windowed_join.py` & `pawpaw-1.0.0rc2/pawpaw/arborform/postorator/windowed_join.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/pawpaw/nlp/nlp.py` & `pawpaw-1.0.0rc2/pawpaw/nlp/nlp.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/pawpaw/nlp/table.py` & `pawpaw-1.0.0rc2/pawpaw/nlp/table.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/pawpaw/query/_query.py` & `pawpaw-1.0.0rc2/pawpaw/query/_query.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/pawpaw/visualization/ascii_box.py` & `pawpaw-1.0.0rc2/pawpaw/visualization/ascii_box.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/pawpaw/visualization/highlighter.py` & `pawpaw-1.0.0rc2/pawpaw/visualization/highlighter.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pawpaw.visualization import sgr
 
 
 class Highlighter:
     '''
     - Guarrantee differing color across any Ito boundaries
     - An Ito parent might not have the same color for sub spans, because it is not always possible to do so.
-      Consider a two-color palete with this nesting:
+      Consider a two-color palette with this nesting:
         A-------------A     Prefix and suffix get color 1
             B------B        Assign color 2 so that boundary AB and BA are visible
             C---C           If color 1, boundary AC is invisible.  If color 2, boundary CB invisible)
     '''
 
     def __init__(self, palette: sgr.C_PALETTE):
         self._backs = tuple(sgr.Back.from_color(col) for col in palette)
```

### Comparing `pawpaw-1.0.0rc1/pawpaw/visualization/pepo/pepo.py` & `pawpaw-1.0.0rc2/pawpaw/visualization/pepo/pepo.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/pawpaw/visualization/sgr/sgr.py` & `pawpaw-1.0.0rc2/pawpaw/visualization/sgr/sgr.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-from dataclasses import dataclass, field
+from dataclasses import dataclass
 import enum
 import typing
 
 from pawpaw import Errors
 
 
 """
@@ -131,15 +131,15 @@
 
     class Rgb(typing.NamedTuple):
         red: int
         green: int
         blue: int
 
         @classmethod
-        def from_24_bit(cls, val: int) -> Rgb:
+        def from_24_bit(cls, val: int) -> _Colors.Rgb:
             return cls(val >> 16, (val >> 8) & 0xFF, val & 0xFF)
 
 
     class EightBit(int):
         """
             0-  7:  standard colors (as in ESC [ 30–37 m)
             8- 15:  high intensity colors (as in ESC [ 90–97 m)
@@ -158,33 +158,33 @@
 @dataclass(frozen=True)
 class Fore(_Sgr):
     _NAMED_OFFSET: int = 30
     _BY_IDX      : int = 38
     RESET        : str = encode(39)
 
     @classmethod
-    def from_color(cls, src: Color) -> str:
+    def from_color(cls, src: C_COLOR) -> str:
         if isinstance(src, Colors.Named):
             nc = getattr(Colors.Named, src.name)
             return encode(nc.value + cls._NAMED_OFFSET)
         elif isinstance(src, Colors.Rgb):
             return encode(cls._BY_IDX, 2, *src)
         elif isinstance(src, Colors.EightBit):
             return encode(cls._BY_IDX, 5, src)
         else:
-            raise Errors.parameter_invalid_type('src', src, Color)
+            raise Errors.parameter_invalid_type('src', src, Colors.Named, Colors.Rgb, Colors.EightBit)
         
-    def __init__(self, src: Color):
+    def __init__(self, src: C_COLOR):
         object.__setattr__(self, '_value', self.from_color(src))
         
     def __str__(self) -> str:
         return self._value
 
 
 @dataclass(frozen=True)
 class Back(Fore):
     _NAMED_OFFSET: int = Fore._NAMED_OFFSET + 10
     _BY_IDX      : int = Fore._BY_IDX + 10
     RESET        : str = encode(49)
 
-    def __init__(self, src: Color):
+    def __init__(self, src: C_COLOR):
         super().__init__(src)
```

### Comparing `pawpaw-1.0.0rc1/pawpaw/xml/xml_helper.py` & `pawpaw-1.0.0rc2/pawpaw/xml/xml_helper.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/pawpaw/xml/xml_parser.py` & `pawpaw-1.0.0rc2/pawpaw/xml/xml_parser.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/tests/test_child_itos.py` & `pawpaw-1.0.0rc2/tests/test_child_itos.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/tests/test_invoke_func.py` & `pawpaw-1.0.0rc2/tests/test_invoke_func.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/tests/test_ito.py` & `pawpaw-1.0.0rc2/tests/test_ito.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/tests/test_ito_ctor.py` & `pawpaw-1.0.0rc2/tests/test_ito_ctor.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/tests/test_ito_descend.py` & `pawpaw-1.0.0rc2/tests/test_ito_descend.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/tests/test_ito_regex_equivalence_methods.py` & `pawpaw-1.0.0rc2/tests/test_ito_regex_equivalence_methods.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/tests/test_ito_serialization.py` & `pawpaw-1.0.0rc2/tests/test_ito_serialization.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/tests/test_ito_str_equivalence_methods.py` & `pawpaw-1.0.0rc2/tests/test_ito_str_equivalence_methods.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/tests/test_nlp.py` & `pawpaw-1.0.0rc2/tests/test_nlp.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/tests/test_query_and_traversal.py` & `pawpaw-1.0.0rc2/tests/test_query_and_traversal.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/tests/test_span.py` & `pawpaw-1.0.0rc2/tests/test_span.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/tests/test_type_magic.py` & `pawpaw-1.0.0rc2/tests/test_type_magic.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/tests/test_util.py` & `pawpaw-1.0.0rc2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/tests/test_version.py` & `pawpaw-1.0.0rc2/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/tests/test_xml_helper.py` & `pawpaw-1.0.0rc2/tests/test_xml_helper.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/tests/test_xml_parser.py` & `pawpaw-1.0.0rc2/tests/test_xml_parser.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/tests/util.py` & `pawpaw-1.0.0rc2/tests/util.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/tests/arborform/test_connectors.py` & `pawpaw-1.0.0rc2/tests/arborform/test_connectors.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/tests/arborform/test_itorator.py` & `pawpaw-1.0.0rc2/tests/arborform/test_itorator.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/tests/arborform/test_itorator_extract.py` & `pawpaw-1.0.0rc2/tests/arborform/test_itorator_extract.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/tests/arborform/test_itorator_filter.py` & `pawpaw-1.0.0rc2/tests/arborform/test_itorator_filter.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/tests/arborform/test_itorator_split.py` & `pawpaw-1.0.0rc2/tests/arborform/test_itorator_split.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/tests/arborform/test_itorator_value_func.py` & `pawpaw-1.0.0rc2/tests/arborform/test_itorator_value_func.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/tests/arborform/test_postorator.py` & `pawpaw-1.0.0rc2/tests/arborform/test_postorator.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/tests/arborform/test_postorator_windowed_join.py` & `pawpaw-1.0.0rc2/tests/arborform/test_postorator_windowed_join.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/tests/visualization/test_sgr.py` & `pawpaw-1.0.0rc2/tests/visualization/test_sgr.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/tests/visualization/test_visualization_ascii_box.py` & `pawpaw-1.0.0rc2/tests/visualization/test_visualization_ascii_box.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/LICENSE` & `pawpaw-1.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/README.md` & `pawpaw-1.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/pyproject.toml` & `pawpaw-1.0.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0rc1/PKG-INFO` & `pawpaw-1.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pawpaw
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: High Performance Text Processing & Segmentation Framework
 Project-URL: Homepage, https://github.com/rlayers/pawpaw
 Project-URL: Bug Tracker, https://github.com/rlayers/pawpaw/issues
 Author-email: "Robert L. Ayers" <rlayers@yahoo.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: extract-text,hierarchical-text-segmentation,information-extraction,knowledge-graph,nlp,python,text-processing,text-segmentation,xml-parser
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pawpaw Version: 1.0.0rc1 Summary: High Performance
+Metadata-Version: 2.1 Name: pawpaw Version: 1.0.0rc2 Summary: High Performance
 Text Processing & Segmentation Framework Project-URL: Homepage, https://
 github.com/rlayers/pawpaw Project-URL: Bug Tracker, https://github.com/rlayers/
 pawpaw/issues Author-email: "Robert L. Ayers"
 yahoo.com> License-Expression: MIT License-File: LICENSE Keywords: extract-
 text,hierarchical-text-segmentation,information-extraction,knowledge-
 graph,nlp,python,text-processing,text-segmentation,xml-parser Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
```

