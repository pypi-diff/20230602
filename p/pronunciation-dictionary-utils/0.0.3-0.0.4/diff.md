# Comparing `tmp/pronunciation-dictionary-utils-0.0.3.tar.gz` & `tmp/pronunciation-dictionary-utils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pronunciation-dictionary-utils-0.0.3.tar", last modified: Thu Jan 12 13:13:11 2023, max compression
+gzip compressed data, was "pronunciation-dictionary-utils-0.0.4.tar", last modified: Fri Jun  2 11:37:49 2023, max compression
```

## Comparing `pronunciation-dictionary-utils-0.0.3.tar` & `pronunciation-dictionary-utils-0.0.4.tar`

### file list

```diff
@@ -1,76 +1,84 @@
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 13:13:11.869576 pronunciation-dictionary-utils-0.0.3/
--rw-rw-r--   0 mi        (1000) mi        (1000)     1071 2022-04-26 08:04:00.000000 pronunciation-dictionary-utils-0.0.3/LICENSE
--rw-rw-r--   0 mi        (1000) mi        (1000)     9251 2023-01-12 13:13:11.869576 pronunciation-dictionary-utils-0.0.3/PKG-INFO
--rw-rw-r--   0 mi        (1000) mi        (1000)     7914 2023-01-12 13:12:43.000000 pronunciation-dictionary-utils-0.0.3/README.md
--rw-rw-r--   0 mi        (1000) mi        (1000)     2765 2023-01-12 13:08:52.000000 pronunciation-dictionary-utils-0.0.3/pyproject.toml
--rw-rw-r--   0 mi        (1000) mi        (1000)       38 2023-01-12 13:13:11.869576 pronunciation-dictionary-utils-0.0.3/setup.cfg
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 13:13:11.865576 pronunciation-dictionary-utils-0.0.3/src/
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 13:13:11.865576 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils/
--rw-rw-r--   0 mi        (1000) mi        (1000)      940 2022-11-10 10:33:02.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils/__init__.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     3618 2022-11-10 10:33:01.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils/common.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2474 2022-11-10 10:33:01.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils/merging.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     5751 2023-01-10 14:46:28.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils/pronunciations_map_symbols.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     5429 2022-10-19 09:24:09.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils/pronunciations_remove_symbols.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2801 2022-10-25 12:21:02.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils/pronunciations_sorting.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     4020 2022-12-01 15:31:06.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils/single_pronunciation_selection.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2685 2022-11-23 09:51:43.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils/subset_extraction.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1808 2022-12-02 14:22:47.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils/validation.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2633 2022-10-14 11:17:03.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils/vocabulary_remove_symbols.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2375 2022-11-10 10:33:02.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils/weights_normalization.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2135 2022-11-10 10:33:01.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils/words_casing_adjustment.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2961 2022-11-10 10:33:02.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils/words_remove_symbols.py
--rw-rw-r--   0 mi        (1000) mi        (1000)      855 2022-10-25 13:11:45.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils/words_sorting.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 13:13:11.865576 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils.egg-info/
--rw-rw-r--   0 mi        (1000) mi        (1000)     9251 2023-01-12 13:13:11.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils.egg-info/PKG-INFO
--rw-rw-r--   0 mi        (1000) mi        (1000)     4164 2023-01-12 13:13:11.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 mi        (1000) mi        (1000)        1 2023-01-12 13:13:11.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 mi        (1000) mi        (1000)       72 2023-01-12 13:13:11.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils.egg-info/entry_points.txt
--rw-rw-r--   0 mi        (1000) mi        (1000)       56 2023-01-12 13:13:11.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils.egg-info/requires.txt
--rw-rw-r--   0 mi        (1000) mi        (1000)      103 2023-01-12 13:13:11.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils.egg-info/top_level.txt
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 13:13:11.865576 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/
--rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-04-26 08:04:34.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/__init__.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     7862 2022-10-14 13:43:01.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/argparse_helper.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     8815 2023-01-12 12:58:03.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/cli.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1980 2022-10-14 13:41:38.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/formatting_adjustment.py
--rw-rw-r--   0 mi        (1000) mi        (1000)      152 2022-11-23 10:14:42.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/globals.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1246 2022-05-23 08:56:43.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/io.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     5165 2022-11-23 08:31:48.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/logging_configuration.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2807 2022-11-10 10:51:28.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/merging.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2769 2022-10-14 13:43:20.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/phoneme_set_extraction.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2820 2023-01-10 14:47:03.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/pronunciations_map_symbols.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     4474 2023-01-10 13:11:07.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/pronunciations_map_symbols_json.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     4337 2022-12-19 12:35:07.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/pronunciations_remove_symbols.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2267 2022-10-25 12:22:37.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/pronunciations_sorting.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2942 2022-12-01 14:57:18.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/single_pronunciation_selection.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     4075 2022-10-14 13:44:29.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/subset_extraction.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2641 2022-10-14 13:44:51.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/vocabulary_extraction.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     3878 2022-11-10 10:33:01.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/vocabulary_remove_symbols.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1843 2022-10-25 12:31:40.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/weights_normalization.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2059 2022-11-10 10:33:01.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/words_casing_adjustment.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     3866 2022-11-10 10:33:01.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/words_remove_symbols.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2018 2022-10-25 13:10:50.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/words_sorting.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 13:13:11.865576 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_tests/
--rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-11-10 10:35:39.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_tests/__init__.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 13:13:11.869576 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_tests/test_common_py/
--rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-11-10 10:35:28.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_tests/test_common_py/__init__.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1834 2022-12-02 12:33:02.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_tests/test_common_py/test_merge_pronunciations.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 13:13:11.869576 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_tests/test_pronunciations_map_symbols_py/
--rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-11-10 10:35:30.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_tests/test_pronunciations_map_symbols_py/__init__.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1351 2023-01-12 13:02:50.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_tests/test_pronunciations_map_symbols_py/test_process_map_pronunciations_full.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1362 2022-11-23 09:14:35.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_tests/test_pronunciations_map_symbols_py/test_process_map_pronunciations_partial.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 13:13:11.869576 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_tests/test_pronunciations_remove_symbols_py/
--rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-11-10 10:35:37.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_tests/test_pronunciations_remove_symbols_py/__init__.py
--rw-rw-r--   0 mi        (1000) mi        (1000)      277 2022-10-19 09:11:52.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_tests/test_pronunciations_remove_symbols_py/test_remove_symbols_all.py
--rw-rw-r--   0 mi        (1000) mi        (1000)      284 2022-10-19 09:09:34.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_tests/test_pronunciations_remove_symbols_py/test_remove_symbols_both.py
--rw-rw-r--   0 mi        (1000) mi        (1000)      292 2022-10-19 09:08:21.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_tests/test_pronunciations_remove_symbols_py/test_remove_symbols_end.py
--rw-rw-r--   0 mi        (1000) mi        (1000)      599 2022-10-19 09:26:18.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_tests/test_pronunciations_remove_symbols_py/test_remove_symbols_from_pronunciations_entry.py
--rw-rw-r--   0 mi        (1000) mi        (1000)      296 2022-10-19 09:07:52.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_tests/test_pronunciations_remove_symbols_py/test_remove_symbols_start.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 13:13:11.869576 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_tests/test_pronunciations_sorting_py/
--rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-11-10 10:35:34.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_tests/test_pronunciations_sorting_py/__init__.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1871 2022-10-19 11:38:18.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_tests/test_pronunciations_sorting_py/test_sort_pronunciations_entry.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 13:13:11.869576 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_tests/test_validation_py/
--rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-12-02 14:18:24.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_tests/test_validation_py/__init__.py
--rw-rw-r--   0 mi        (1000) mi        (1000)      164 2022-05-23 08:27:25.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_tests/test_validation_py/test_validate_dictionary.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 13:13:11.869576 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_tests/test_words_sorting_py/
--rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-11-10 10:35:33.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_tests/test_words_sorting_py/__init__.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2699 2022-10-19 10:47:02.000000 pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_tests/test_words_sorting_py/test_sort_words.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-06-02 11:37:49.932561 pronunciation-dictionary-utils-0.0.4/
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1071 2023-06-02 11:35:32.000000 pronunciation-dictionary-utils-0.0.4/LICENSE
+-rw-rw-r--   0 mi        (1000) mi        (1000)     9713 2023-06-02 11:37:49.932561 pronunciation-dictionary-utils-0.0.4/PKG-INFO
+-rw-rw-r--   0 mi        (1000) mi        (1000)     8380 2023-06-02 11:35:32.000000 pronunciation-dictionary-utils-0.0.4/README.md
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2762 2023-06-02 11:37:39.000000 pronunciation-dictionary-utils-0.0.4/pyproject.toml
+-rw-rw-r--   0 mi        (1000) mi        (1000)       38 2023-06-02 11:37:49.932561 pronunciation-dictionary-utils-0.0.4/setup.cfg
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-06-02 11:37:49.924561 pronunciation-dictionary-utils-0.0.4/src/
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-06-02 11:37:49.928562 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils/
+-rw-rw-r--   0 mi        (1000) mi        (1000)      940 2022-11-10 10:33:02.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils/__init__.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     3618 2022-11-10 10:33:01.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils/common.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2474 2022-11-10 10:33:01.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils/merging.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     5761 2023-06-02 11:19:57.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils/pronunciations_map_symbols.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     5429 2022-10-19 09:24:09.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils/pronunciations_remove_symbols.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2801 2022-10-25 12:21:02.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils/pronunciations_sorting.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     4020 2022-12-01 15:31:06.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils/single_pronunciation_selection.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2685 2022-11-23 09:51:43.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils/subset_extraction.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1808 2022-12-02 14:22:47.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils/validation.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2633 2022-10-14 11:17:03.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils/vocabulary_remove_symbols.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2375 2022-11-10 10:33:02.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils/weights_normalization.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2135 2022-11-10 10:33:01.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils/words_casing_adjustment.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2961 2022-11-10 10:33:02.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils/words_remove_symbols.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)      855 2022-10-25 13:11:45.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils/words_sorting.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-06-02 11:37:49.928562 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils.egg-info/
+-rw-rw-r--   0 mi        (1000) mi        (1000)     9713 2023-06-02 11:37:49.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 mi        (1000) mi        (1000)     4945 2023-06-02 11:37:49.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 mi        (1000) mi        (1000)        1 2023-06-02 11:37:49.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 mi        (1000) mi        (1000)       72 2023-06-02 11:37:49.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils.egg-info/entry_points.txt
+-rw-rw-r--   0 mi        (1000) mi        (1000)       56 2023-06-02 11:37:49.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils.egg-info/requires.txt
+-rw-rw-r--   0 mi        (1000) mi        (1000)      103 2023-06-02 11:37:49.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils.egg-info/top_level.txt
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-06-02 11:37:49.932561 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/
+-rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-04-26 08:04:34.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/__init__.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     7862 2022-10-14 13:43:01.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/argparse_helper.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     8815 2023-01-12 12:58:03.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/cli.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1980 2022-10-14 13:41:38.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/formatting_adjustment.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)      152 2022-11-23 10:14:42.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/globals.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1246 2022-05-23 08:56:43.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/io.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     5165 2022-11-23 08:31:48.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/logging_configuration.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2806 2023-06-02 11:19:57.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/merging.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2769 2022-10-14 13:43:20.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/phoneme_set_extraction.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2819 2023-06-02 11:19:57.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/pronunciations_map_symbols.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     8281 2023-06-02 11:19:57.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/pronunciations_map_symbols_json.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     4336 2023-06-02 11:19:57.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/pronunciations_remove_symbols.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2266 2023-06-02 11:19:57.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/pronunciations_sorting.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2941 2023-06-02 11:19:57.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/single_pronunciation_selection.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     4075 2022-10-14 13:44:29.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/subset_extraction.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2641 2022-10-14 13:44:51.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/vocabulary_extraction.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     3877 2023-06-02 11:19:57.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/vocabulary_remove_symbols.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1842 2023-06-02 11:19:57.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/weights_normalization.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2058 2023-06-02 11:19:57.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/words_casing_adjustment.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     3865 2023-06-02 11:19:57.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/words_remove_symbols.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2017 2023-06-02 11:19:57.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/words_sorting.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-06-02 11:37:49.932561 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/
+-rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-11-10 10:35:39.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/__init__.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-06-02 11:37:49.932561 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_common_py/
+-rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-11-10 10:35:28.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_common_py/__init__.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1834 2022-12-02 12:33:02.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_common_py/test_merge_pronunciations.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-06-02 11:37:49.932561 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_pronunciations_map_symbols_json_py/
+-rw-rw-r--   0 mi        (1000) mi        (1000)        2 2023-06-02 11:19:57.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_pronunciations_map_symbols_json_py/__init__.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1234 2023-06-02 11:19:57.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_pronunciations_map_symbols_json_py/test_apply_mapping_full.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1239 2023-06-02 11:19:57.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_pronunciations_map_symbols_json_py/test_apply_mapping_partial.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1004 2023-06-02 11:19:57.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_pronunciations_map_symbols_json_py/test_get_mappable_symbols.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1006 2023-06-02 11:19:57.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_pronunciations_map_symbols_json_py/test_get_unmappable_symbols.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     3926 2023-06-02 11:19:57.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_pronunciations_map_symbols_json_py/test_identify_and_apply_mappings_full.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     3447 2023-06-02 11:19:57.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_pronunciations_map_symbols_json_py/test_identify_and_apply_mappings_partial.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-06-02 11:37:49.932561 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_pronunciations_map_symbols_py/
+-rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-11-10 10:35:30.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_pronunciations_map_symbols_py/__init__.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1351 2023-01-12 13:02:50.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_pronunciations_map_symbols_py/test_process_map_pronunciations_full.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1362 2022-11-23 09:14:35.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_pronunciations_map_symbols_py/test_process_map_pronunciations_partial.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-06-02 11:37:49.932561 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_pronunciations_remove_symbols_py/
+-rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-11-10 10:35:37.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_pronunciations_remove_symbols_py/__init__.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)      277 2022-10-19 09:11:52.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_pronunciations_remove_symbols_py/test_remove_symbols_all.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)      284 2022-10-19 09:09:34.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_pronunciations_remove_symbols_py/test_remove_symbols_both.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)      292 2022-10-19 09:08:21.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_pronunciations_remove_symbols_py/test_remove_symbols_end.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)      599 2022-10-19 09:26:18.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_pronunciations_remove_symbols_py/test_remove_symbols_from_pronunciations_entry.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)      296 2022-10-19 09:07:52.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_pronunciations_remove_symbols_py/test_remove_symbols_start.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-06-02 11:37:49.932561 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_pronunciations_sorting_py/
+-rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-11-10 10:35:34.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_pronunciations_sorting_py/__init__.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1871 2022-10-19 11:38:18.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_pronunciations_sorting_py/test_sort_pronunciations_entry.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-06-02 11:37:49.932561 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_validation_py/
+-rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-12-02 14:18:24.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_validation_py/__init__.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)      164 2022-05-23 08:27:25.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_validation_py/test_validate_dictionary.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-06-02 11:37:49.932561 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_words_sorting_py/
+-rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-11-10 10:35:33.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_words_sorting_py/__init__.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2699 2022-10-19 10:47:02.000000 pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_words_sorting_py/test_sort_words.py
```

### Comparing `pronunciation-dictionary-utils-0.0.3/LICENSE` & `pronunciation-dictionary-utils-0.0.4/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Stefan Taubert
+Copyright (c) 2023 Stefan Taubert
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pronunciation-dictionary-utils-0.0.3/PKG-INFO` & `pronunciation-dictionary-utils-0.0.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pronunciation-dictionary-utils
-Version: 0.0.3
+Version: 0.0.4
 Summary: CLI and library to modify pronunciation dictionaries (any language).
 Author-email: Stefan Taubert <pypi@stefantaubert.com>
 Maintainer-email: Stefan Taubert <pypi@stefantaubert.com>
 License: MIT
 Project-URL: Homepage, https://github.com/stefantaubert/pronunciation-dictionary-utils
 Project-URL: Issues, https://github.com/stefantaubert/pronunciation-dictionary-utils/issues
 Keywords: ARPAbet,IPA,X-SAMPA,CMU,TTS,Text-to-speech,Speech synthesis,Language,Linguistics
@@ -19,35 +19,36 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: <=3.11,>=3.8
+Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pronunciation-dictionary-utils
 
 [![PyPI](https://img.shields.io/pypi/v/pronunciation-dictionary-utils.svg)](https://pypi.python.org/pypi/pronunciation-dictionary-utils)
 [![PyPI](https://img.shields.io/pypi/pyversions/pronunciation-dictionary-utils.svg)](https://pypi.python.org/pypi/pronunciation-dictionary-utils)
 [![MIT](https://img.shields.io/github/license/stefantaubert/pronunciation-dictionary-utils.svg)](LICENSE)
 [![PyPI](https://img.shields.io/github/commits-since/stefantaubert/pronunciation-dictionary-utils/latest/master.svg)](https://pypi.python.org/pypi/pronunciation-dictionary-utils)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7529307.svg)](https://doi.org/10.5281/zenodo.7529307)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7997799.svg)](https://doi.org/10.5281/zenodo.7997799)
 
 Library and CLI to modify pronunciation dictionaries (any language).
 
 ## Features
 
 - `export-vocabulary`: export vocabulary from dictionaries
 - `export-phonemes`: export phoneme set from dictionaries
 - `merge`: merge dictionaries together
 - `extract`: extract subset of dictionary vocabulary
 - `map-symbols-in-pronunciations`: map phonemes/symbols in pronunciations to another phoneme/symbol, e.g., mapping ARPAbet to IPA
+- `map-symbols-in-pronunciations-json`: map phonemes/symbols in pronunciations to phoneme/symbol specified in file
 - `remove-symbols-from-vocabulary`: remove phonemes/symbols from vocabulary
 - `remove-symbols-from-pronunciations`: remove phonemes/symbols from pronunciations
 - `remove-symbols-from-words`: remove characters/symbols from words
 - `change-formatting`: change formatting of dictionaries
 - `select-single-pronunciation`: select single pronunciation
 - `change-word-casing`: transform all words to upper- or lower-case
 - `sort-words`: sort dictionary after words
@@ -186,14 +187,22 @@
 
 ## Citation
 
 If you want to cite this repo, you can use this BibTeX-entry generated by GitHub (see *About => Cite this repository*).
 
 ## Changelog
 
+- v0.0.4 (2023-06-02)
+  - Bugfixes:
+    - Support for Python 3.11 was not correctly defined
+    - Adjusted return value for `map_symbols` in `pronunciations_map_symbols`
+    - Corrected log messages
+  - Added:
+    - Support for partial mapping in `map-symbols-in-pronunciations-json`
+    - Added testing units for `map-symbols-in-pronunciations-json`
 - v0.0.3 (2023-01-12)
   - Added:
     - Added `sort-words` to support sorting of words
     - Added `sort-pronunciations` to support sorting of pronunciations
     - Added `normalize-weights` to support normalization of pronunciation weights
     - Added `map-symbols-in-pronunciations-json` to map phonemes/symbols in pronunciations to phonemes/symbols specified in json file
     - Added `--mode` to symbol removal in pronunciations
```

### Comparing `pronunciation-dictionary-utils-0.0.3/README.md` & `pronunciation-dictionary-utils-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # pronunciation-dictionary-utils
 
 [![PyPI](https://img.shields.io/pypi/v/pronunciation-dictionary-utils.svg)](https://pypi.python.org/pypi/pronunciation-dictionary-utils)
 [![PyPI](https://img.shields.io/pypi/pyversions/pronunciation-dictionary-utils.svg)](https://pypi.python.org/pypi/pronunciation-dictionary-utils)
 [![MIT](https://img.shields.io/github/license/stefantaubert/pronunciation-dictionary-utils.svg)](LICENSE)
 [![PyPI](https://img.shields.io/github/commits-since/stefantaubert/pronunciation-dictionary-utils/latest/master.svg)](https://pypi.python.org/pypi/pronunciation-dictionary-utils)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7529307.svg)](https://doi.org/10.5281/zenodo.7529307)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7997799.svg)](https://doi.org/10.5281/zenodo.7997799)
 
 Library and CLI to modify pronunciation dictionaries (any language).
 
 ## Features
 
 - `export-vocabulary`: export vocabulary from dictionaries
 - `export-phonemes`: export phoneme set from dictionaries
 - `merge`: merge dictionaries together
 - `extract`: extract subset of dictionary vocabulary
 - `map-symbols-in-pronunciations`: map phonemes/symbols in pronunciations to another phoneme/symbol, e.g., mapping ARPAbet to IPA
+- `map-symbols-in-pronunciations-json`: map phonemes/symbols in pronunciations to phoneme/symbol specified in file
 - `remove-symbols-from-vocabulary`: remove phonemes/symbols from vocabulary
 - `remove-symbols-from-pronunciations`: remove phonemes/symbols from pronunciations
 - `remove-symbols-from-words`: remove characters/symbols from words
 - `change-formatting`: change formatting of dictionaries
 - `select-single-pronunciation`: select single pronunciation
 - `change-word-casing`: transform all words to upper- or lower-case
 - `sort-words`: sort dictionary after words
@@ -157,14 +158,22 @@
 
 ## Citation
 
 If you want to cite this repo, you can use this BibTeX-entry generated by GitHub (see *About => Cite this repository*).
 
 ## Changelog
 
+- v0.0.4 (2023-06-02)
+  - Bugfixes:
+    - Support for Python 3.11 was not correctly defined
+    - Adjusted return value for `map_symbols` in `pronunciations_map_symbols`
+    - Corrected log messages
+  - Added:
+    - Support for partial mapping in `map-symbols-in-pronunciations-json`
+    - Added testing units for `map-symbols-in-pronunciations-json`
 - v0.0.3 (2023-01-12)
   - Added:
     - Added `sort-words` to support sorting of words
     - Added `sort-pronunciations` to support sorting of pronunciations
     - Added `normalize-weights` to support normalization of pronunciation weights
     - Added `map-symbols-in-pronunciations-json` to map phonemes/symbols in pronunciations to phonemes/symbols specified in json file
     - Added `--mode` to symbol removal in pronunciations
```

### Comparing `pronunciation-dictionary-utils-0.0.3/pyproject.toml` & `pronunciation-dictionary-utils-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,21 +3,21 @@
   "setuptools >= 40.9.0",
   "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pronunciation-dictionary-utils"
-version = "0.0.3"
+version = "0.0.4"
 description = "CLI and library to modify pronunciation dictionaries (any language)."
 readme = "README.md"
-requires-python = ">=3.8, <=3.11"
+requires-python = ">=3.8, <4"
 license = {text = "MIT"}
 authors = [
-  {name = "Stefan Taubert", email = "pypi@stefantaubert.com"}
+  {name = "Stefan Taubert", email = "pypi@stefantaubert.com"},
 ]
 maintainers = [
   {name = "Stefan Taubert", email = "pypi@stefantaubert.com"},
 ]
 keywords = [
   "ARPAbet",
   "IPA",
```

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils/__init__.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils/common.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils/common.py`

 * *Files identical despite different names*

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils/merging.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils/merging.py`

 * *Files identical despite different names*

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils/pronunciations_map_symbols.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils/pronunciations_map_symbols.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from collections import OrderedDict
 from functools import partial
 from multiprocessing.pool import Pool
-from typing import List, Optional, Tuple, Union
+from typing import List, Optional, Set, Tuple, Union
 
 from ordered_set import OrderedSet
 from pronunciation_dictionary import (MultiprocessingOptions, PronunciationDict, Pronunciations,
                                       Symbol, Word)
 from tqdm import tqdm
 
 from pronunciation_dictionary_utils.validation import (validate_dictionary, validate_mp_options,
@@ -15,15 +15,15 @@
 def __validate_symbol(symbol: str) -> Optional[str]:
   if not isinstance(symbol, str):
     return "Value needs of type 'str'!"
   assert len(symbol) > 0
   return None
 
 
-def map_symbols(dictionary: PronunciationDict, symbols: OrderedSet[Symbol], map_to: Union[List[Symbol], Symbol], partial_mapping: bool, mp_options: MultiprocessingOptions, use_tqdm: bool = True) -> int:
+def map_symbols(dictionary: PronunciationDict, symbols: OrderedSet[Symbol], map_to: Union[List[Symbol], Symbol], partial_mapping: bool, mp_options: MultiprocessingOptions, use_tqdm: bool = True) -> Set[str]:
   if msg := validate_dictionary(dictionary):
     raise ValueError(f"Parameter 'dictionary': {msg}")
   if msg := validate_type(symbols, OrderedSet):
     raise ValueError(f"Parameter 'symbols': {msg}")
   for symbol in symbols:
     if msg := __validate_symbol(symbol):
       raise ValueError(f"Parameter 'symbols': {msg}")
```

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils/pronunciations_remove_symbols.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils/pronunciations_remove_symbols.py`

 * *Files identical despite different names*

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils/pronunciations_sorting.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils/pronunciations_sorting.py`

 * *Files identical despite different names*

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils/single_pronunciation_selection.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils/single_pronunciation_selection.py`

 * *Files identical despite different names*

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils/subset_extraction.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils/subset_extraction.py`

 * *Files identical despite different names*

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils/validation.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils/validation.py`

 * *Files identical despite different names*

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils/vocabulary_remove_symbols.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils/vocabulary_remove_symbols.py`

 * *Files identical despite different names*

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils/weights_normalization.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils/weights_normalization.py`

 * *Files identical despite different names*

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils/words_casing_adjustment.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils/words_casing_adjustment.py`

 * *Files identical despite different names*

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils/words_remove_symbols.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils/words_remove_symbols.py`

 * *Files identical despite different names*

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils/words_sorting.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils/words_sorting.py`

 * *Files identical despite different names*

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils.egg-info/PKG-INFO` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pronunciation-dictionary-utils
-Version: 0.0.3
+Version: 0.0.4
 Summary: CLI and library to modify pronunciation dictionaries (any language).
 Author-email: Stefan Taubert <pypi@stefantaubert.com>
 Maintainer-email: Stefan Taubert <pypi@stefantaubert.com>
 License: MIT
 Project-URL: Homepage, https://github.com/stefantaubert/pronunciation-dictionary-utils
 Project-URL: Issues, https://github.com/stefantaubert/pronunciation-dictionary-utils/issues
 Keywords: ARPAbet,IPA,X-SAMPA,CMU,TTS,Text-to-speech,Speech synthesis,Language,Linguistics
@@ -19,35 +19,36 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: <=3.11,>=3.8
+Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pronunciation-dictionary-utils
 
 [![PyPI](https://img.shields.io/pypi/v/pronunciation-dictionary-utils.svg)](https://pypi.python.org/pypi/pronunciation-dictionary-utils)
 [![PyPI](https://img.shields.io/pypi/pyversions/pronunciation-dictionary-utils.svg)](https://pypi.python.org/pypi/pronunciation-dictionary-utils)
 [![MIT](https://img.shields.io/github/license/stefantaubert/pronunciation-dictionary-utils.svg)](LICENSE)
 [![PyPI](https://img.shields.io/github/commits-since/stefantaubert/pronunciation-dictionary-utils/latest/master.svg)](https://pypi.python.org/pypi/pronunciation-dictionary-utils)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7529307.svg)](https://doi.org/10.5281/zenodo.7529307)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7997799.svg)](https://doi.org/10.5281/zenodo.7997799)
 
 Library and CLI to modify pronunciation dictionaries (any language).
 
 ## Features
 
 - `export-vocabulary`: export vocabulary from dictionaries
 - `export-phonemes`: export phoneme set from dictionaries
 - `merge`: merge dictionaries together
 - `extract`: extract subset of dictionary vocabulary
 - `map-symbols-in-pronunciations`: map phonemes/symbols in pronunciations to another phoneme/symbol, e.g., mapping ARPAbet to IPA
+- `map-symbols-in-pronunciations-json`: map phonemes/symbols in pronunciations to phoneme/symbol specified in file
 - `remove-symbols-from-vocabulary`: remove phonemes/symbols from vocabulary
 - `remove-symbols-from-pronunciations`: remove phonemes/symbols from pronunciations
 - `remove-symbols-from-words`: remove characters/symbols from words
 - `change-formatting`: change formatting of dictionaries
 - `select-single-pronunciation`: select single pronunciation
 - `change-word-casing`: transform all words to upper- or lower-case
 - `sort-words`: sort dictionary after words
@@ -186,14 +187,22 @@
 
 ## Citation
 
 If you want to cite this repo, you can use this BibTeX-entry generated by GitHub (see *About => Cite this repository*).
 
 ## Changelog
 
+- v0.0.4 (2023-06-02)
+  - Bugfixes:
+    - Support for Python 3.11 was not correctly defined
+    - Adjusted return value for `map_symbols` in `pronunciations_map_symbols`
+    - Corrected log messages
+  - Added:
+    - Support for partial mapping in `map-symbols-in-pronunciations-json`
+    - Added testing units for `map-symbols-in-pronunciations-json`
 - v0.0.3 (2023-01-12)
   - Added:
     - Added `sort-words` to support sorting of words
     - Added `sort-pronunciations` to support sorting of pronunciations
     - Added `normalize-weights` to support normalization of pronunciation weights
     - Added `map-symbols-in-pronunciations-json` to map phonemes/symbols in pronunciations to phonemes/symbols specified in json file
     - Added `--mode` to symbol removal in pronunciations
```

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils.egg-info/SOURCES.txt` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -42,14 +42,21 @@
 src/pronunciation_dictionary_utils_cli/weights_normalization.py
 src/pronunciation_dictionary_utils_cli/words_casing_adjustment.py
 src/pronunciation_dictionary_utils_cli/words_remove_symbols.py
 src/pronunciation_dictionary_utils_cli/words_sorting.py
 src/pronunciation_dictionary_utils_tests/__init__.py
 src/pronunciation_dictionary_utils_tests/test_common_py/__init__.py
 src/pronunciation_dictionary_utils_tests/test_common_py/test_merge_pronunciations.py
+src/pronunciation_dictionary_utils_tests/test_pronunciations_map_symbols_json_py/__init__.py
+src/pronunciation_dictionary_utils_tests/test_pronunciations_map_symbols_json_py/test_apply_mapping_full.py
+src/pronunciation_dictionary_utils_tests/test_pronunciations_map_symbols_json_py/test_apply_mapping_partial.py
+src/pronunciation_dictionary_utils_tests/test_pronunciations_map_symbols_json_py/test_get_mappable_symbols.py
+src/pronunciation_dictionary_utils_tests/test_pronunciations_map_symbols_json_py/test_get_unmappable_symbols.py
+src/pronunciation_dictionary_utils_tests/test_pronunciations_map_symbols_json_py/test_identify_and_apply_mappings_full.py
+src/pronunciation_dictionary_utils_tests/test_pronunciations_map_symbols_json_py/test_identify_and_apply_mappings_partial.py
 src/pronunciation_dictionary_utils_tests/test_pronunciations_map_symbols_py/__init__.py
 src/pronunciation_dictionary_utils_tests/test_pronunciations_map_symbols_py/test_process_map_pronunciations_full.py
 src/pronunciation_dictionary_utils_tests/test_pronunciations_map_symbols_py/test_process_map_pronunciations_partial.py
 src/pronunciation_dictionary_utils_tests/test_pronunciations_remove_symbols_py/__init__.py
 src/pronunciation_dictionary_utils_tests/test_pronunciations_remove_symbols_py/test_remove_symbols_all.py
 src/pronunciation_dictionary_utils_tests/test_pronunciations_remove_symbols_py/test_remove_symbols_both.py
 src/pronunciation_dictionary_utils_tests/test_pronunciations_remove_symbols_py/test_remove_symbols_end.py
```

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/argparse_helper.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/argparse_helper.py`

 * *Files identical despite different names*

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/cli.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/cli.py`

 * *Files identical despite different names*

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/formatting_adjustment.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/formatting_adjustment.py`

 * *Files identical despite different names*

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/io.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/io.py`

 * *Files identical despite different names*

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/logging_configuration.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/logging_configuration.py`

 * *Files identical despite different names*

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/merging.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/merging.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     dictionary_instance = try_load_dict(dictionary, ns.encoding, lp_options, mp_options, logger)
     if dictionary_instance is None:
       return False
     changed_anything |= merge_dictionaries(
       resulting_dictionary, dictionary_instance, ns.duplicate_handling)
 
   if not changed_anything:
-    logger.info("Didn't changed anything.")
+    logger.info("Didn't change anything.")
     return True
 
   success = try_save_dict(resulting_dictionary, ns.dictionary,
                           ns.encoding, s_options, logger)
   if not success:
     return False
```

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/phoneme_set_extraction.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/phoneme_set_extraction.py`

 * *Files identical despite different names*

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/pronunciations_map_symbols.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/pronunciations_map_symbols.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     return False
 
   to_symbol = ns.to_symbol if ns.partial_mapping else [ns.to_symbol]
   changed_words = map_symbols(
     dictionary_instance, ns.from_symbols, to_symbol, ns.partial_mapping, mp_options)
 
   if len(changed_words) == 0:
-    logger.info("Didn't changed anything.")
+    logger.info("Didn't change anything.")
     return True
 
   logger.info(f"Changed pronunciations of {len(changed_words)} word(s).")
 
   success = try_save_dict(dictionary_instance, ns.dictionary, ns.encoding, s_options, logger)
   if not success:
     return False
```

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/pronunciations_remove_symbols.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/pronunciations_remove_symbols.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
   if dictionary_instance is None:
     return False
 
   removed_words, changed_counter = remove_symbols_from_pronunciations(
     dictionary_instance, ns.symbols, ns.mode, ns.keep_empty, ns.empty_symbol, mp_options)
 
   if changed_counter == 0:
-    logger.info("Didn't changed anything.")
+    logger.info("Didn't change anything.")
     return True
 
   logger.info(f"Changed pronunciations of {changed_counter} word(s).")
 
   success = try_save_dict(dictionary_instance, ns.dictionary, ns.encoding, s_options, logger)
   if not success:
     return False
```

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/pronunciations_sorting.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/pronunciations_sorting.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
   changed_counter = sort_pronunciations(
     dictionary_instance, ns.descending, ns.ignore_weight, mp_options)
 
   changed_anything = changed_counter > 0
 
   if not changed_anything:
-    logger.info("Didn't changed anything.")
+    logger.info("Didn't change anything.")
     return True
 
   success = try_save_dict(dictionary_instance, ns.dictionary, ns.encoding, s_options, logger)
   if not success:
     return False
 
   logger.info(f"Written dictionary to: \"{ns.dictionary.absolute()}\".")
```

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/single_pronunciation_selection.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/single_pronunciation_selection.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
   if dictionary_instance is None:
     return False
 
   changed_counter = select_single_pronunciation(
     dictionary_instance, ns.mode, ns.seed, mp_options)
 
   if changed_counter == 0:
-    logger.info("Didn't changed anything.")
+    logger.info("Didn't change anything.")
     return True
 
   logger.info(f"Changed pronunciations of {changed_counter} word(s).")
 
   success = try_save_dict(dictionary_instance, ns.dictionary, ns.encoding, s_options, logger)
   if not success:
     return False
```

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/subset_extraction.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/subset_extraction.py`

 * *Files identical despite different names*

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/vocabulary_extraction.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/vocabulary_extraction.py`

 * *Files identical despite different names*

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/vocabulary_remove_symbols.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/vocabulary_remove_symbols.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
   mp_options = MultiprocessingOptions(ns.n_jobs, ns.maxtasksperchild, ns.chunksize)
 
   removed_words_entirely, changed_words = remove_symbols_from_vocabulary(
     vocabulary, symbols_str, ns.mode, mp_options)
 
   if len(changed_words) == 0:
-    logger.info("Didn't changed anything.")
+    logger.info("Didn't change anything.")
     return True
 
   logger.info(f"Changed {len(changed_words)} word(s).")
 
   new_vocabulary_content = "\n".join(vocabulary)
   try:
     ns.vocabulary.write_text(new_vocabulary_content, ns.encoding)
```

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/weights_normalization.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/weights_normalization.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     return False
 
   changed_counter = normalize_weights(dictionary_instance, mp_options)
 
   changed_anything = changed_counter > 0
 
   if not changed_anything:
-    logger.info("Didn't changed anything.")
+    logger.info("Didn't change anything.")
     return True
 
   success = try_save_dict(dictionary_instance, ns.dictionary, ns.encoding, s_options, logger)
   if not success:
     return False
 
   logger.info(f"Written dictionary to: \"{ns.dictionary.absolute()}\".")
```

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/words_casing_adjustment.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/words_casing_adjustment.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
   dictionary_instance = try_load_dict(ns.dictionary, ns.encoding, lp_options, mp_options, logger)
   if dictionary_instance is None:
     return False
 
   removed_words, created_words = change_word_casing(dictionary_instance, ns.mode, mp_options)
 
   if len(removed_words) == 0:
-    logger.info("Didn't changed anything.")
+    logger.info("Didn't change anything.")
     return True
 
   logger.info(f"Replaced {len(removed_words)} with {len(created_words)} word spelling(s).")
 
   success = try_save_dict(dictionary_instance, ns.dictionary, ns.encoding, s_options, logger)
   if not success:
     return False
```

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/words_remove_symbols.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/words_remove_symbols.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
   if dictionary_instance is None:
     return False
 
   removed_words_entirely, removed_words = remove_symbols_from_words(
     dictionary_instance, symbols_str, ns.mode, mp_options)
 
   if len(removed_words) == 0:
-    logger.info("Didn't changed anything.")
+    logger.info("Didn't change anything.")
     return True
 
   logger.info(f"Renamed {len(removed_words)} word(s).")
 
   success = try_save_dict(dictionary_instance, ns.dictionary, ns.encoding, s_options, logger)
   if not success:
     return False
```

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_cli/words_sorting.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_cli/words_sorting.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     return False
 
   new_dictionary = sort_words(dictionary_instance, ns.descending, ns.consider_case)
 
   changed_anything = new_dictionary != dictionary_instance
 
   if not changed_anything:
-    logger.info("Didn't changed anything.")
+    logger.info("Didn't change anything.")
     return True
 
   success = try_save_dict(new_dictionary, ns.dictionary, ns.encoding, s_options, logger)
   if not success:
     return False
 
   logger.info(f"Written dictionary to: \"{ns.dictionary.absolute()}\".")
```

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_tests/test_common_py/test_merge_pronunciations.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_common_py/test_merge_pronunciations.py`

 * *Files identical despite different names*

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_tests/test_pronunciations_map_symbols_py/test_process_map_pronunciations_full.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_pronunciations_map_symbols_py/test_process_map_pronunciations_full.py`

 * *Files identical despite different names*

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_tests/test_pronunciations_map_symbols_py/test_process_map_pronunciations_partial.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_pronunciations_map_symbols_py/test_process_map_pronunciations_partial.py`

 * *Files identical despite different names*

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_tests/test_pronunciations_remove_symbols_py/test_remove_symbols_from_pronunciations_entry.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_pronunciations_remove_symbols_py/test_remove_symbols_from_pronunciations_entry.py`

 * *Files identical despite different names*

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_tests/test_pronunciations_sorting_py/test_sort_pronunciations_entry.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_pronunciations_sorting_py/test_sort_pronunciations_entry.py`

 * *Files identical despite different names*

### Comparing `pronunciation-dictionary-utils-0.0.3/src/pronunciation_dictionary_utils_tests/test_words_sorting_py/test_sort_words.py` & `pronunciation-dictionary-utils-0.0.4/src/pronunciation_dictionary_utils_tests/test_words_sorting_py/test_sort_words.py`

 * *Files identical despite different names*

