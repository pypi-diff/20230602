# Comparing `tmp/starvote-1.5.1.tar.gz` & `tmp/starvote-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starvote-1.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "starvote-2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `starvote-1.5.1.tar` & `starvote-2.0.tar`

### file list

```diff
@@ -1,56 +1,161 @@
--rw-r--r--   0        0        0       19 2023-05-20 12:58:10.568731 starvote-1.5.1/.gitignore
--rw-r--r--   0        0        0     1087 2023-05-20 12:48:55.372092 starvote-1.5.1/LICENSE
--rw-r--r--   0        0        0    12872 2023-05-24 18:58:45.035781 starvote-1.5.1/README.md
--rw-r--r--   0        0        0      267 2023-05-20 12:47:55.671593 starvote-1.5.1/example.py
--rw-r--r--   0        0        0      502 2023-05-20 12:55:16.755279 starvote-1.5.1/pyproject.toml
--rw-r--r--   0        0        0      406 2023-05-21 11:19:31.211412 starvote-1.5.1/sample_polls/README.md
--rw-r--r--   0        0        0      169 2023-05-20 12:17:24.308288 starvote-1.5.1/sample_polls/sample_poll_automatic_runoff_breakable_tie.csv
--rw-r--r--   0        0        0      321 2023-05-21 14:36:07.812513 starvote-1.5.1/sample_polls/sample_poll_automatic_runoff_breakable_tie.result.txt
--rw-r--r--   0        0        0      169 2023-05-20 12:16:12.379686 starvote-1.5.1/sample_polls/sample_poll_automatic_runoff_unbreakable_tie.csv
--rw-r--r--   0        0        0      412 2023-05-21 14:36:10.524536 starvote-1.5.1/sample_polls/sample_poll_automatic_runoff_unbreakable_tie.result.txt
--rw-r--r--   0        0        0      226 2023-05-21 13:55:36.270675 starvote-1.5.1/sample_polls/sample_poll_proportional_star_3_seats_breakable_tie.csv
--rw-r--r--   0        0        0      883 2023-05-21 14:46:04.809533 starvote-1.5.1/sample_polls/sample_poll_proportional_star_3_seats_breakable_tie.result.txt
--rw-r--r--   0        0        0      226 2023-05-21 13:52:36.109138 starvote-1.5.1/sample_polls/sample_poll_proportional_star_3_seats_unbreakable_tie.csv
--rw-r--r--   0        0        0      390 2023-05-21 14:45:20.721162 starvote-1.5.1/sample_polls/sample_poll_proportional_star_3_seats_unbreakable_tie.result.txt
--rw-r--r--   0        0        0     4689 2023-05-22 05:48:56.428345 starvote-1.5.1/sample_polls/sample_poll_reweighted_range_3_seats_max-score_10.csv
--rw-r--r--   0        0        0     5899 2023-05-22 07:24:36.945502 starvote-1.5.1/sample_polls/sample_poll_reweighted_range_3_seats_max-score_10.result.html
--rw-r--r--   0        0        0      520 2023-05-22 07:23:43.629054 starvote-1.5.1/sample_polls/sample_poll_reweighted_range_3_seats_max-score_10.result.txt
--rw-r--r--   0        0        0      169 2023-05-20 12:27:44.977476 starvote-1.5.1/sample_polls/sample_poll_score_round_breakable_tie_between_second_and_third.csv
--rw-r--r--   0        0        0      340 2023-05-21 14:36:12.440552 starvote-1.5.1/sample_polls/sample_poll_score_round_breakable_tie_between_second_and_third.result.txt
--rw-r--r--   0        0        0      169 2023-05-20 12:14:18.630735 starvote-1.5.1/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_first.csv
--rw-r--r--   0        0        0      234 2023-05-21 14:36:15.004573 starvote-1.5.1/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_first.result.txt
--rw-r--r--   0        0        0      226 2023-05-20 14:20:22.817978 starvote-1.5.1/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_second.csv
--rw-r--r--   0        0        0      267 2023-05-21 14:36:17.328593 starvote-1.5.1/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_second.result.txt
--rw-r--r--   0        0        0      169 2023-05-20 12:30:43.458967 starvote-1.5.1/sample_polls/sample_poll_score_round_unbreakable_tie_between_second_and_third.csv
--rw-r--r--   0        0        0      374 2023-05-21 14:36:20.268617 starvote-1.5.1/sample_polls/sample_poll_score_round_unbreakable_tie_between_second_and_third.result.txt
--rw-r--r--   0        0        0   115109 2023-05-20 12:04:19.133723 starvote-1.5.1/sample_polls/starvote_ballots_2020_democratic_presidential_primary.csv
--rw-r--r--   0        0        0   696161 2023-05-20 14:36:00.553825 starvote-1.5.1/sample_polls/starvote_ballots_2020_democratic_presidential_primary.result.pdf
--rw-r--r--   0        0        0     2642 2023-05-21 14:36:26.092666 starvote-1.5.1/sample_polls/starvote_ballots_2020_democratic_presidential_primary.result.txt
--rw-r--r--   0        0        0    57750 2023-05-20 12:04:29.149807 starvote-1.5.1/sample_polls/starvote_ballots_2020_libertarian_party_presidential_nomination.csv
--rw-r--r--   0        0        0   575556 2023-05-20 14:35:00.177319 starvote-1.5.1/sample_polls/starvote_ballots_2020_libertarian_party_presidential_nomination.result.pdf
--rw-r--r--   0        0        0      961 2023-05-21 14:36:28.876690 starvote-1.5.1/sample_polls/starvote_ballots_2020_libertarian_party_presidential_nomination.result.txt
--rw-r--r--   0        0        0    49711 2023-05-20 12:04:34.029848 starvote-1.5.1/sample_polls/starvote_ballots_best_akali_skins.csv
--rw-r--r--   0        0        0   538128 2023-05-20 14:33:25.560528 starvote-1.5.1/sample_polls/starvote_ballots_best_akali_skins.result.pdf
--rw-r--r--   0        0        0      876 2023-05-21 14:36:32.040716 starvote-1.5.1/sample_polls/starvote_ballots_best_akali_skins.result.txt
--rw-r--r--   0        0        0     1812 2023-05-20 10:35:18.365110 starvote-1.5.1/sample_polls/starvote_ballots_eurovision_song_contest_2023.csv
--rw-r--r--   0        0        0   807144 2023-05-20 14:33:51.120742 starvote-1.5.1/sample_polls/starvote_ballots_eurovision_song_contest_2023.result.pdf
--rw-r--r--   0        0        0     2418 2023-05-21 14:36:34.744739 starvote-1.5.1/sample_polls/starvote_ballots_eurovision_song_contest_2023.result.txt
--rw-r--r--   0        0        0   250538 2023-05-20 10:34:04.044490 starvote-1.5.1/sample_polls/starvote_ballots_libertarian_party_2020_presidential_nomination_may.csv
--rw-r--r--   0        0        0   643536 2023-05-20 14:35:41.153662 starvote-1.5.1/sample_polls/starvote_ballots_libertarian_party_2020_presidential_nomination_may.result.pdf
--rw-r--r--   0        0        0     1091 2023-05-21 14:36:37.344761 starvote-1.5.1/sample_polls/starvote_ballots_libertarian_party_2020_presidential_nomination_may.result.txt
--rw-r--r--   0        0        0    31534 2023-05-20 12:04:38.493885 starvote-1.5.1/sample_polls/starvote_ballots_presidential_candidates.csv
--rw-r--r--   0        0        0   325033 2023-05-20 14:34:17.572963 starvote-1.5.1/sample_polls/starvote_ballots_presidential_candidates.result.pdf
--rw-r--r--   0        0        0      408 2023-05-21 14:36:39.896782 starvote-1.5.1/sample_polls/starvote_ballots_presidential_candidates.result.txt
--rw-r--r--   0        0        0    48454 2023-05-20 12:04:25.689778 starvote-1.5.1/sample_polls/starvote_ballots_presidential_poll_july_2020.csv
--rw-r--r--   0        0        0   360427 2023-05-20 14:36:25.050030 starvote-1.5.1/sample_polls/starvote_ballots_presidential_poll_july_2020.result.pdf
--rw-r--r--   0        0        0      419 2023-05-21 14:36:42.084801 starvote-1.5.1/sample_polls/starvote_ballots_presidential_poll_july_2020.result.txt
--rw-r--r--   0        0        0   123039 2023-05-20 12:04:13.781679 starvote-1.5.1/sample_polls/starvote_ballots_updated_2020_libertarian_presidential_candidate.csv
--rw-r--r--   0        0        0   584998 2023-05-20 14:35:22.465506 starvote-1.5.1/sample_polls/starvote_ballots_updated_2020_libertarian_presidential_candidate.result.pdf
--rw-r--r--   0        0        0      961 2023-05-21 14:36:44.284819 starvote-1.5.1/sample_polls/starvote_ballots_updated_2020_libertarian_presidential_candidate.result.txt
--rw-r--r--   0        0        0    52870 2023-05-20 12:04:22.533752 starvote-1.5.1/sample_polls/starvote_ballots_wa_governor_2020_republican_party_straw_poll.csv
--rw-r--r--   0        0        0   354740 2023-05-20 14:36:48.550226 starvote-1.5.1/sample_polls/starvote_ballots_wa_governor_2020_republican_party_straw_poll.result.pdf
--rw-r--r--   0        0        0      377 2023-05-21 14:36:46.788840 starvote-1.5.1/sample_polls/starvote_ballots_wa_governor_2020_republican_party_straw_poll.result.txt
--rw-r--r--   0        0        0    23647 2023-05-24 18:58:25.987616 starvote-1.5.1/starvote/__init__.py
--rw-r--r--   0        0        0       84 2023-05-21 14:27:54.116361 starvote-1.5.1/starvote/__main__.py
--rw-r--r--   0        0        0     2705 2023-05-24 18:54:16.761465 starvote-1.5.1/tests/run_tests.py
--rw-r--r--   0        0        0    13292 1970-01-01 00:00:00.000000 starvote-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0       38 2023-05-27 15:21:37.716345 starvote-2.0/.gitignore
+-rw-r--r--   0        0        0     1087 2023-05-20 12:48:55.372092 starvote-2.0/LICENSE
+-rw-r--r--   0        0        0    32170 2023-06-02 19:51:22.344081 starvote-2.0/README.md
+-rw-r--r--   0        0        0    15825 2023-06-01 10:48:31.686649 starvote-2.0/docs/clarifying_star_voting.md
+-rw-r--r--   0        0        0     2743 2023-05-31 19:56:48.827782 starvote-2.0/docs/formatting_fractions_in_columns_of_text.txt
+-rw-r--r--   0        0        0      217 2023-05-31 21:13:55.136896 starvote-2.0/example.py
+-rw-r--r--   0        0        0      583 2023-06-02 19:49:52.947305 starvote-2.0/pyproject.toml
+-rw-r--r--   0        0        0    90421 2023-06-02 19:29:39.644773 starvote-2.0/starvote/__init__.py
+-rw-r--r--   0        0        0      106 2023-06-02 00:43:16.709978 starvote-2.0/starvote/__main__.py
+-rw-r--r--   0        0        0     5809 2023-06-02 18:28:35.340765 starvote-2.0/starvote/reference.py
+-rw-r--r--   0        0        0     1051 2023-06-02 01:09:12.579780 starvote-2.0/test_elections/README.md
+-rw-r--r--   0        0        0       84 2023-06-01 23:43:37.846114 starvote-2.0/test_elections/bad_syntax_ballot_pragma_as_last_line.starvote
+-rw-r--r--   0        0        0     1358 2023-06-02 19:23:34.765586 starvote-2.0/test_elections/bad_syntax_ballot_pragma_as_last_line.txt
+-rw-r--r--   0        0        0       68 2023-06-01 23:24:50.800081 starvote-2.0/test_elections/bad_syntax_change_section_in_list.starvote
+-rw-r--r--   0        0        0     1395 2023-06-02 19:23:34.765586 starvote-2.0/test_elections/bad_syntax_change_section_in_list.txt
+-rw-r--r--   0        0        0       68 2023-06-01 23:23:06.267150 starvote-2.0/test_elections/bad_syntax_fussy_wrong_ballots_1.starvote
+-rw-r--r--   0        0        0     1404 2023-06-02 19:23:34.769586 starvote-2.0/test_elections/bad_syntax_fussy_wrong_ballots_1.txt
+-rw-r--r--   0        0        0       67 2023-06-01 23:23:00.095096 starvote-2.0/test_elections/bad_syntax_fussy_wrong_ballots_2.starvote
+-rw-r--r--   0        0        0     1402 2023-06-02 19:23:34.769586 starvote-2.0/test_elections/bad_syntax_fussy_wrong_ballots_2.txt
+-rw-r--r--   0        0        0       35 2023-06-02 19:31:20.821653 starvote-2.0/test_elections/bad_syntax_invalid_method.starvote
+-rw-r--r--   0        0        0     1375 2023-06-02 19:31:54.613947 starvote-2.0/test_elections/bad_syntax_invalid_method.txt
+-rw-r--r--   0        0        0       40 2023-06-01 23:17:55.140381 starvote-2.0/test_elections/bad_syntax_invalid_option.starvote
+-rw-r--r--   0        0        0     1374 2023-06-02 19:23:34.769586 starvote-2.0/test_elections/bad_syntax_invalid_option.txt
+-rw-r--r--   0        0        0       44 2023-06-01 23:16:35.203670 starvote-2.0/test_elections/bad_syntax_invalid_pragma.starvote
+-rw-r--r--   0        0        0     1376 2023-06-02 19:23:34.769586 starvote-2.0/test_elections/bad_syntax_invalid_pragma.txt
+-rw-r--r--   0        0        0       89 2023-06-01 23:37:41.946945 starvote-2.0/test_elections/bad_syntax_invalid_start_of_line_mode.starvote
+-rw-r--r--   0        0        0     1335 2023-06-02 19:23:34.769586 starvote-2.0/test_elections/bad_syntax_invalid_start_of_line_mode.txt
+-rw-r--r--   0        0        0       50 2023-06-01 23:14:06.126343 starvote-2.0/test_elections/bad_syntax_invalid_starvote_path_1.starvote
+-rw-r--r--   0        0        0     1331 2023-06-02 19:23:34.769586 starvote-2.0/test_elections/bad_syntax_invalid_starvote_path_1.txt
+-rw-r--r--   0        0        0       70 2023-06-01 23:28:17.369920 starvote-2.0/test_elections/bad_syntax_invalid_starvote_path_2.starvote
+-rw-r--r--   0        0        0     1360 2023-06-02 19:23:34.769586 starvote-2.0/test_elections/bad_syntax_invalid_starvote_path_2.txt
+-rw-r--r--   0        0        0       38 2023-06-01 23:13:26.765992 starvote-2.0/test_elections/bad_syntax_invalid_tiebreaker.starvote
+-rw-r--r--   0        0        0     1382 2023-06-02 19:23:34.769586 starvote-2.0/test_elections/bad_syntax_invalid_tiebreaker.txt
+-rw-r--r--   0        0        0       59 2023-06-02 02:02:11.939956 starvote-2.0/test_elections/bad_syntax_malformed_section.starvote
+-rw-r--r--   0        0        0     1371 2023-06-02 19:23:34.769586 starvote-2.0/test_elections/bad_syntax_malformed_section.txt
+-rw-r--r--   0        0        0       41 2023-06-01 23:44:44.538707 starvote-2.0/test_elections/bad_syntax_no_ballots.starvote
+-rw-r--r--   0        0        0     1314 2023-06-02 19:23:34.769586 starvote-2.0/test_elections/bad_syntax_no_ballots.txt
+-rw-r--r--   0        0        0       44 2023-06-01 23:34:09.385053 starvote-2.0/test_elections/bad_syntax_no_equals.starvote
+-rw-r--r--   0        0        0     1346 2023-06-02 19:23:34.769586 starvote-2.0/test_elections/bad_syntax_no_equals.txt
+-rw-r--r--   0        0        0       59 2023-06-02 01:03:50.036922 starvote-2.0/test_elections/bad_syntax_no_method.starvote
+-rw-r--r--   0        0        0     1409 2023-06-02 19:23:34.769586 starvote-2.0/test_elections/bad_syntax_no_method.txt
+-rw-r--r--   0        0        0       46 2023-06-01 23:32:02.351922 starvote-2.0/test_elections/bad_syntax_no_section.starvote
+-rw-r--r--   0        0        0     1364 2023-06-02 19:23:34.769586 starvote-2.0/test_elections/bad_syntax_no_section.txt
+-rw-r--r--   0        0        0       47 2023-06-01 23:21:20.118206 starvote-2.0/test_elections/bad_syntax_pragma_in_options.starvote
+-rw-r--r--   0        0        0     1375 2023-06-02 19:23:34.769586 starvote-2.0/test_elections/bad_syntax_pragma_in_options.txt
+-rw-r--r--   0        0        0      103 2023-06-01 23:32:48.848336 starvote-2.0/test_elections/bad_syntax_pragma_inside_list.starvote
+-rw-r--r--   0        0        0     1387 2023-06-02 19:23:34.769586 starvote-2.0/test_elections/bad_syntax_pragma_inside_list.txt
+-rw-r--r--   0        0        0       47 2023-06-01 23:18:10.564519 starvote-2.0/test_elections/bad_syntax_repeated_option.starvote
+-rw-r--r--   0        0        0     1380 2023-06-02 19:23:34.769586 starvote-2.0/test_elections/bad_syntax_repeated_option.txt
+-rw-r--r--   0        0        0       60 2023-06-01 23:31:08.239441 starvote-2.0/test_elections/bad_syntax_repeated_section.starvote
+-rw-r--r--   0        0        0     1383 2023-06-02 19:23:34.769586 starvote-2.0/test_elections/bad_syntax_repeated_section.txt
+-rw-r--r--   0        0        0    57750 2023-05-20 12:04:29.149807 starvote-2.0/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.csv
+-rw-r--r--   0        0        0   575556 2023-05-20 14:35:00.177319 starvote-2.0/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.pdf
+-rw-r--r--   0        0        0     1403 2023-06-02 19:23:34.773586 starvote-2.0/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.txt
+-rw-r--r--   0        0        0   115221 2023-05-27 14:48:58.735061 starvote-2.0/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.csv
+-rw-r--r--   0        0        0   410807 2023-05-27 14:59:16.160516 starvote-2.0/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.pdf
+-rw-r--r--   0        0        0     3193 2023-06-02 19:23:34.785586 starvote-2.0/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.txt
+-rw-r--r--   0        0        0    49711 2023-05-20 12:04:34.029848 starvote-2.0/test_elections/starvote_ballots_best_akali_skins.csv
+-rw-r--r--   0        0        0   538128 2023-05-20 14:33:25.560528 starvote-2.0/test_elections/starvote_ballots_best_akali_skins.pdf
+-rw-r--r--   0        0        0     1331 2023-06-02 19:23:34.789586 starvote-2.0/test_elections/starvote_ballots_best_akali_skins.txt
+-rw-r--r--   0        0        0     1812 2023-05-20 10:35:18.365110 starvote-2.0/test_elections/starvote_ballots_eurovision_song_contest_2023.csv
+-rw-r--r--   0        0        0   807144 2023-05-20 14:33:51.120742 starvote-2.0/test_elections/starvote_ballots_eurovision_song_contest_2023.pdf
+-rw-r--r--   0        0        0     2879 2023-06-02 19:23:34.789586 starvote-2.0/test_elections/starvote_ballots_eurovision_song_contest_2023.txt
+-rw-r--r--   0        0        0   250538 2023-05-20 10:34:04.044490 starvote-2.0/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.csv
+-rw-r--r--   0        0        0   643536 2023-05-20 14:35:41.153662 starvote-2.0/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.pdf
+-rw-r--r--   0        0        0     1596 2023-06-02 19:23:34.809586 starvote-2.0/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.txt
+-rw-r--r--   0        0        0      175 2023-06-02 19:18:28.166907 starvote-2.0/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_bloc_star.starvote
+-rw-r--r--   0        0        0    12586 2023-06-02 19:23:35.117589 starvote-2.0/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_bloc_star.txt
+-rw-r--r--   0        0        0      141 2023-06-02 19:18:26.038889 starvote-2.0/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_star_pr.starvote
+-rw-r--r--   0        0        0    12586 2023-06-02 19:23:35.429592 starvote-2.0/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_star_pr.txt
+-rw-r--r--   0        0        0    31534 2023-05-20 12:04:38.493885 starvote-2.0/test_elections/starvote_ballots_presidential_candidates.csv
+-rw-r--r--   0        0        0   325033 2023-05-20 14:34:17.572963 starvote-2.0/test_elections/starvote_ballots_presidential_candidates.pdf
+-rw-r--r--   0        0        0      814 2023-06-02 19:23:35.433591 starvote-2.0/test_elections/starvote_ballots_presidential_candidates.txt
+-rw-r--r--   0        0        0    48454 2023-05-20 12:04:25.689778 starvote-2.0/test_elections/starvote_ballots_presidential_poll_july_2020.csv
+-rw-r--r--   0        0        0   360427 2023-05-20 14:36:25.050030 starvote-2.0/test_elections/starvote_ballots_presidential_poll_july_2020.pdf
+-rw-r--r--   0        0        0      799 2023-06-02 19:23:35.433591 starvote-2.0/test_elections/starvote_ballots_presidential_poll_july_2020.txt
+-rw-r--r--   0        0        0   123039 2023-05-20 12:04:13.781679 starvote-2.0/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.csv
+-rw-r--r--   0        0        0   584998 2023-05-20 14:35:22.465506 starvote-2.0/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.pdf
+-rw-r--r--   0        0        0     1434 2023-06-02 19:23:35.441592 starvote-2.0/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.txt
+-rw-r--r--   0        0        0    52870 2023-05-20 12:04:22.533752 starvote-2.0/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.csv
+-rw-r--r--   0        0        0   354740 2023-05-20 14:36:48.550226 starvote-2.0/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.pdf
+-rw-r--r--   0        0        0      747 2023-06-02 19:23:35.445592 starvote-2.0/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.txt
+-rw-r--r--   0        0        0      146 2023-06-01 14:23:14.825743 starvote-2.0/test_elections/test_election_all_fives_bloc_star.starvote
+-rw-r--r--   0        0        0     1080 2023-06-02 19:23:35.445592 starvote-2.0/test_elections/test_election_all_fives_bloc_star.txt
+-rw-r--r--   0        0        0      145 2023-06-01 14:23:10.941709 starvote-2.0/test_elections/test_election_all_fives_rrv.starvote
+-rw-r--r--   0        0        0      484 2023-06-02 19:23:35.445592 starvote-2.0/test_elections/test_election_all_fives_rrv.txt
+-rw-r--r--   0        0        0      151 2023-06-02 19:18:20.314839 starvote-2.0/test_elections/test_election_all_fives_star-pr.starvote
+-rw-r--r--   0        0        0      476 2023-06-02 19:23:35.445592 starvote-2.0/test_elections/test_election_all_fives_star-pr.txt
+-rw-r--r--   0        0        0      132 2023-06-01 14:23:02.245634 starvote-2.0/test_elections/test_election_all_fives_star.starvote
+-rw-r--r--   0        0        0     1030 2023-06-02 19:23:35.445592 starvote-2.0/test_elections/test_election_all_fives_star.txt
+-rw-r--r--   0        0        0      146 2023-06-01 14:23:30.837882 starvote-2.0/test_elections/test_election_all_threes_bloc_star.starvote
+-rw-r--r--   0        0        0     1080 2023-06-02 19:23:35.445592 starvote-2.0/test_elections/test_election_all_threes_bloc_star.txt
+-rw-r--r--   0        0        0       92 2023-06-01 22:34:03.536957 starvote-2.0/test_elections/test_election_all_threes_rrv.starvote
+-rw-r--r--   0        0        0      484 2023-06-02 19:23:35.449592 starvote-2.0/test_elections/test_election_all_threes_rrv.txt
+-rw-r--r--   0        0        0       98 2023-06-02 19:18:18.286821 starvote-2.0/test_elections/test_election_all_threes_star-pr.starvote
+-rw-r--r--   0        0        0      476 2023-06-02 19:23:35.449592 starvote-2.0/test_elections/test_election_all_threes_star-pr.txt
+-rw-r--r--   0        0        0      132 2023-06-01 14:23:19.233781 starvote-2.0/test_elections/test_election_all_threes_star.starvote
+-rw-r--r--   0        0        0     1030 2023-06-02 19:23:35.449592 starvote-2.0/test_elections/test_election_all_threes_star.txt
+-rw-r--r--   0        0        0      146 2023-06-01 14:19:42.607904 starvote-2.0/test_elections/test_election_all_zeroes_bloc_star.starvote
+-rw-r--r--   0        0        0     1077 2023-06-02 19:23:35.449592 starvote-2.0/test_elections/test_election_all_zeroes_bloc_star.txt
+-rw-r--r--   0        0        0      145 2023-06-01 14:19:40.835888 starvote-2.0/test_elections/test_election_all_zeroes_rrv.starvote
+-rw-r--r--   0        0        0      481 2023-06-02 19:23:35.449592 starvote-2.0/test_elections/test_election_all_zeroes_rrv.txt
+-rw-r--r--   0        0        0      151 2023-06-02 19:18:15.894800 starvote-2.0/test_elections/test_election_all_zeroes_star-pr.starvote
+-rw-r--r--   0        0        0      473 2023-06-02 19:23:35.449592 starvote-2.0/test_elections/test_election_all_zeroes_star-pr.txt
+-rw-r--r--   0        0        0      132 2023-06-01 14:19:46.079934 starvote-2.0/test_elections/test_election_all_zeroes_star.starvote
+-rw-r--r--   0        0        0     1027 2023-06-02 19:23:35.449592 starvote-2.0/test_elections/test_election_all_zeroes_star.txt
+-rw-r--r--   0        0        0     2660 2023-05-31 22:55:06.890838 starvote-2.0/test_elections/test_election_bloc_star_and_electowiki.starvote
+-rw-r--r--   0        0        0     3383 2023-06-02 19:23:35.449592 starvote-2.0/test_elections/test_election_bloc_star_and_electowiki.txt
+-rw-r--r--   0        0        0      989 2023-05-31 14:32:27.710655 starvote-2.0/test_elections/test_election_bloc_star_unbreakable_tie_for_first.starvote
+-rw-r--r--   0        0        0     1606 2023-06-02 19:23:35.449592 starvote-2.0/test_elections/test_election_bloc_star_unbreakable_tie_for_first.txt
+-rw-r--r--   0        0        0      201 2023-05-31 14:32:09.618494 starvote-2.0/test_elections/test_election_breakable_tie_for_second_in_score_round.starvote
+-rw-r--r--   0        0        0      831 2023-06-02 19:23:35.449592 starvote-2.0/test_elections/test_election_breakable_tie_for_second_in_score_round.txt
+-rw-r--r--   0        0        0      204 2023-05-31 14:31:42.454252 starvote-2.0/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.starvote
+-rw-r--r--   0        0        0      965 2023-06-02 19:23:35.449592 starvote-2.0/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.txt
+-rw-r--r--   0        0        0      203 2023-05-31 14:31:18.974043 starvote-2.0/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_score_round.starvote
+-rw-r--r--   0        0        0      744 2023-06-02 19:23:35.453592 starvote-2.0/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_score_round.txt
+-rw-r--r--   0        0        0      838 2023-05-31 14:31:04.393913 starvote-2.0/test_elections/test_election_demonstrate_cloneproofness_1.starvote
+-rw-r--r--   0        0        0      542 2023-06-02 19:23:35.453592 starvote-2.0/test_elections/test_election_demonstrate_cloneproofness_1.txt
+-rw-r--r--   0        0        0      830 2023-05-31 14:09:22.654324 starvote-2.0/test_elections/test_election_demonstrate_cloneproofness_2.starvote
+-rw-r--r--   0        0        0     1087 2023-06-02 19:23:35.453592 starvote-2.0/test_elections/test_election_demonstrate_cloneproofness_2.txt
+-rw-r--r--   0        0        0      194 2023-06-01 16:45:03.487305 starvote-2.0/test_elections/test_election_extra_candidates_in_permutation.starvote
+-rw-r--r--   0        0        0      142 2023-06-02 19:23:35.453592 starvote-2.0/test_elections/test_election_extra_candidates_in_permutation.txt
+-rw-r--r--   0        0        0      165 2023-06-01 16:45:09.147349 starvote-2.0/test_elections/test_election_incomplete_permutation.starvote
+-rw-r--r--   0        0        0      138 2023-06-02 19:23:35.453592 starvote-2.0/test_elections/test_election_incomplete_permutation.txt
+-rw-r--r--   0        0        0      132 2023-06-02 01:44:01.610291 starvote-2.0/test_elections/test_election_no_output.starvote
+-rw-r--r--   0        0        0       17 2023-06-02 19:23:35.453592 starvote-2.0/test_elections/test_election_no_output.txt
+-rw-r--r--   0        0        0      130 2023-06-01 16:34:20.926370 starvote-2.0/test_elections/test_election_no_permuted_candidates_tiebreaker.starvote
+-rw-r--r--   0        0        0     1329 2023-06-02 19:23:35.453592 starvote-2.0/test_elections/test_election_no_permuted_candidates_tiebreaker.txt
+-rw-r--r--   0        0        0      131 2023-06-01 17:57:44.689602 starvote-2.0/test_elections/test_election_only_one_candidate_star.starvote
+-rw-r--r--   0        0        0      505 2023-06-02 19:23:35.453592 starvote-2.0/test_elections/test_election_only_one_candidate_star.txt
+-rw-r--r--   0        0        0      177 2023-06-01 17:57:23.633416 starvote-2.0/test_elections/test_election_only_two_candidates_bloc_star.starvote
+-rw-r--r--   0        0        0      487 2023-06-02 19:23:35.453592 starvote-2.0/test_elections/test_election_only_two_candidates_bloc_star.txt
+-rw-r--r--   0        0        0      176 2023-06-01 17:57:20.909392 starvote-2.0/test_elections/test_election_only_two_candidates_rrv.starvote
+-rw-r--r--   0        0        0      523 2023-06-02 19:23:35.453592 starvote-2.0/test_elections/test_election_only_two_candidates_rrv.txt
+-rw-r--r--   0        0        0      182 2023-06-02 19:18:13.310778 starvote-2.0/test_elections/test_election_only_two_candidates_star-pr.starvote
+-rw-r--r--   0        0        0      545 2023-06-02 19:23:35.453592 starvote-2.0/test_elections/test_election_only_two_candidates_star-pr.txt
+-rw-r--r--   0        0        0      319 2023-06-02 19:18:05.042705 starvote-2.0/test_elections/test_election_proportional_star_unbreakable_tie.starvote
+-rw-r--r--   0        0        0      480 2023-06-02 19:23:35.453592 starvote-2.0/test_elections/test_election_proportional_star_unbreakable_tie.txt
+-rw-r--r--   0        0        0     5899 2023-05-22 07:24:36.945502 starvote-2.0/test_elections/test_election_reweighted_range_sample_election.html
+-rw-r--r--   0        0        0      450 2023-05-31 14:05:31.788268 starvote-2.0/test_elections/test_election_reweighted_range_sample_election.starvote
+-rw-r--r--   0        0        0     1150 2023-06-02 19:23:35.457592 starvote-2.0/test_elections/test_election_reweighted_range_sample_election.txt
+-rw-r--r--   0        0        0      203 2023-05-31 14:05:02.452007 starvote-2.0/test_elections/test_election_unbreakable_three_way_tie_for_first_in_score_round.starvote
+-rw-r--r--   0        0        0     1023 2023-06-02 19:23:35.457592 starvote-2.0/test_elections/test_election_unbreakable_three_way_tie_for_first_in_score_round.txt
+-rw-r--r--   0        0        0      306 2023-06-01 18:06:23.106174 starvote-2.0/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round.starvote
+-rw-r--r--   0        0        0     1788 2023-06-02 19:23:35.457592 starvote-2.0/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round.txt
+-rw-r--r--   0        0        0      143 2023-06-02 19:18:03.054688 starvote-2.0/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_star-pr.starvote
+-rw-r--r--   0        0        0     2029 2023-06-02 19:23:35.457592 starvote-2.0/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_star-pr.txt
+-rw-r--r--   0        0        0      203 2023-05-31 14:04:09.035532 starvote-2.0/test_elections/test_election_unbreakable_tie_for_second_in_score_round.starvote
+-rw-r--r--   0        0        0      938 2023-06-02 19:23:35.457592 starvote-2.0/test_elections/test_election_unbreakable_tie_for_second_in_score_round.txt
+-rw-r--r--   0        0        0      155 2023-05-28 20:58:05.118365 starvote-2.0/test_elections/test_election_unbreakable_tie_in_automatic_runoff_round.starvote
+-rw-r--r--   0        0        0     1081 2023-06-02 19:23:35.457592 starvote-2.0/test_elections/test_election_unbreakable_tie_in_automatic_runoff_round.txt
+-rw-r--r--   0        0        0      150 2023-06-01 14:49:33.615373 starvote-2.0/test_elections/test_election_use_just_raise_tiebreaker.starvote
+-rw-r--r--   0        0        0     1197 2023-06-02 19:23:35.457592 starvote-2.0/test_elections/test_election_use_just_raise_tiebreaker.txt
+-rw-r--r--   0        0        0      154 2023-06-01 16:06:23.349484 starvote-2.0/test_elections/test_election_use_no_description_tiebreaker.starvote
+-rw-r--r--   0        0        0     1030 2023-06-02 19:23:35.457592 starvote-2.0/test_elections/test_election_use_no_description_tiebreaker.txt
+-rw-r--r--   0        0        0      152 2023-06-01 16:08:48.230596 starvote-2.0/test_elections/test_election_use_only_heading_tiebreaker.starvote
+-rw-r--r--   0        0        0      152 2023-06-02 19:23:35.457592 starvote-2.0/test_elections/test_election_use_only_heading_tiebreaker.txt
+-rw-r--r--   0        0        0    35726 2023-06-02 19:26:39.999204 starvote-2.0/tests/run_tests.py
+-rwxr-xr-x   0        0        0     2211 2023-06-02 19:34:15.379168 starvote-2.0/tools/is_ok
+-rwxr-xr-x   0        0        0     1827 2023-06-02 18:03:13.135277 starvote-2.0/tools/remake_test_elections_output
+-rw-r--r--   0        0        0    32738 1970-01-01 00:00:00.000000 starvote-2.0/PKG-INFO
```

### Comparing `starvote-1.5.1/LICENSE` & `starvote-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `starvote-1.5.1/sample_polls/sample_poll_reweighted_range_3_seats_max-score_10.result.html` & `starvote-2.0/test_elections/test_election_reweighted_range_sample_election.html`

 * *Files identical despite different names*

### Comparing `starvote-1.5.1/sample_polls/starvote_ballots_2020_democratic_presidential_primary.csv` & `starvote-2.0/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.csv`

 * *Files 0% similar despite different names*

```diff
@@ -1016,7 +1016,8 @@
 phw3rc4x5c,"2023-03-05 06:15:21",p4rs6xn4,4,4,0,4,0,3,0,4,0,0,0,0,0,3,3,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0
 mar752262f,"2023-03-11 20:04:01",p4rs6xn4,5,2,0,1,4,0,2,2,0,0,0,0,0,0,2,3,0,2,0,0,0,0,0,1,0,5,0,0,0,2,0,2,0,5,4
 sdshhzrsxa,"2023-03-28 17:34:48",p4rs6xn4,5,4,2,5,4,3,2,5,1,2,3,2,3,4,3,1,1,1,1,1,1,1,1,1,1,1,1,1,1,2,1,1,1,1,1
 s27khpch9n,"2023-04-11 12:18:21",p4rs6xn4,1,1,0,2,0,3,2,2,0,2,0,3,2,0,3,3,0,0,3,3,5,0,3,0,0,0,3,0,0,0,0,0,0,0,0
 55dx95zrc7,"2023-04-13 16:15:10",p4rs6xn4,4,4,0,0,4,0,0,0,0,0,2,5,0,2,5,5,0,0,0,0,0,0,0,0,0,0,0,0,0,5,0,0,0,5,0
 p7r9y3n2w1,"2023-04-20 17:14:27",p4rs6xn4,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0
 57x43t61xf,"2023-04-29 18:17:33",p4rs6xn4,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,5,0,0,0,5,5,5,5,5,5,5,5,0,0,0,0,0,0
+3zphk1t7kw,"2023-05-25 02:01:13",p4rs6xn4,5,1,1,1,1,1,1,2,1,1,1,1,1,1,3,1,0,1,0,0,0,0,0,0,0,0,0,1,0,1,1,1,1,1,1
```

### Comparing `starvote-1.5.1/sample_polls/starvote_ballots_2020_democratic_presidential_primary.result.pdf` & `starvote-2.0/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 12% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,699 +1,363 @@
 5/20/23, 7:35 AM
 
-★.✓ - 2020 Democratic Presidential Primary
+★.✓ - Libertarian Party 2020 Presidential Nomination - Star Voting Poll: May
 
 .vote
 
 More
 
 Learn
 
 Login
 
 You may score as many candidates as you like from 0 (no support) to 5 (max support).
 You may give the same score to multiple candidates.
 The two highest-scoring candidates are finalists.
 The finalist scored higher by more voters wins.
+Votes are limited to one per IP address.
 
-Vote on "2020 Democratic Presidential Primary"
-Jay Inslee
-0
+Vote on "Libertarian Party 2020 Presidential Nomination - Star Voting
+Poll: May"
+Ended: 2020-05-31 23:59:00
 
-Andrew Yang
+Vermin Supreme
 0
 
-Kamala Harris
+Phil Gray
 0
 
-Julian Castro
+Brian Ellison
 0
 
-Cory Booker
+John Monds
 0
 
-Amy Klobuchar
+Jedidiah Hill
 0
 
-Beto O'Rourke
+James Ogle
 0
 
-Marriane Williamson
+Jacob Hornberger
 0
 
-Tulsi Gabbard
+Louis Vanacore
 0
 
-John Kerry
-https://star.vote/demprimary2020/
+Keenan Dunham
+https://star.vote/lp2020presmay/
 
 1/5
 
 5/20/23, 7:35 AM
 
-★.✓ - 2020 Democratic Presidential Primary
+★.✓ - Libertarian Party 2020 Presidential Nomination - Star Voting Poll: May
 
 0
 
-John Delaney
+Daniel Behrman
 0
 
-Kirsten Gillibrand
+Sam Robb
 0
 
-Joe Biden
+Mark Whitney
 0
 
-Bernie Sanders
+Erik Gerhardt
 0
 
-Elizabeth Warren
+Sorinne Ardeleanu
 0
 
-John Hickenlooper
+Arvin Vohra
 0
 
-Pete Buttigieg
+Jo Jorgensen
 0
 
-Vote!
-
-Show Results
-
-Results for "2020 Democratic Presidential Primary"
-Selection Phase (Top two advance):
-10013 voters
-# Option
-
-Points
-
-Average
-
-1 Andrew Yang
-
-26220
-
-2.6
-
-20267
-
-2.0
-
-16861
-
-1.7
+Kenneth Blevins
+0
 
-→
+Justin Amash
+0
 
-52.3%
-52.3% (2.6/5)
+Adam Kokesh
+0
 
-2 Bernie Sanders
-40.4%
-40.4% (2.0/5)
+Judge Jim Gray
+0
 
-3 Pete Buttigieg
-https://star.vote/demprimary2020/
+Steve Richey
+https://star.vote/lp2020presmay/
 
 2/5
 
 5/20/23, 7:35 AM
-33.6%
-33.6% (1.7/5)
 
-★.✓ - 2020 Democratic Presidential Primary
+★.✓ - Libertarian Party 2020 Presidential Nomination - Star Voting Poll: May
 
-Runoff Phase (Single winner):
+0
 
-13000
+Rhett Smith
+0
 
-Runoff Phase (Single winner):
-1.3
+Vote!
 
-11317
+Show Results
 
-1.1
+Results for "Libertarian Party 2020 Presidential Nomination - Star
+Voting Poll: May"
+Selection Phase (Top two advance):
+2909 voters
 
-6037
+→ 1 Justin Amash
+# Option
 
-0.6
+# Option
 
-5872
+Points Average
 
-0.6
+1 Justin Amash
 
-8 Marriane Williamson 5260
+8018
 
-0.5
+2.8
 
-4 Tulsi Gabbard
+55.1%
+55.1% (2.8/5)
 
-25.9%
-25.9% (1.3/5)
+2 Vermin Supreme 7200
 
-5 Elizabeth Warren
-22.6%
-22.6% (1.1/5)
+2.5
 
-6 Cory Booker
-12.0%
-12.0% (0.6/5)
+49.5%
+49.5% (2.5/5)
 
-7 Kamala Harris
-11.7%
-11.7% (0.6/5)
+3826
 
-# Option
+1.3
 
-Votes
+4 Jacob Hornberger 3193
 
-1 Andrew Yang
+1.1
 
-4329
+3 Judge Jim Gray
 
-43.23% (4329/10013)
+Runoff Phase (Single winner):
+Votes
 
-2 Bernie Sanders 2912
-29.08% (2912/10013)
+1404
 
-No Preference 2772
-27.68% (2772/10013)
+48.26% (1404/2909)
 
-10.5%
-10.5% (0.5/5)
+2 Vermin Supreme 1138
+39.12% (1138/2909)
 
-9 Amy Klobuchar
+No Preference
 
-4340
+367
 
-0.4
+12.62% (367/2909)
 
-4311
+26.3%
+26.3% (1.3/5)
 
-0.4
+22.0%
+22.0% (1.1/5)
 
-4181
+2625
 
-0.4
+0.9
 
-3231
+2324
 
-0.3
+0.8
 
-2912
+1941
 
-0.3
+0.7
 
-2722
+1707
 
-0.3
+0.6
 
-2138
+1315
 
-0.2
+0.5
 
-1993
+10 Sorinne Ardeleanu 929
 
-0.2
+0.3
 
-1771
+5 Jo Jorgensen
+18.0%
+18.0% (0.9/5)
+
+6 Adam Kokesh
+16.0%
+16.0% (0.8/5)
+
+7 Daniel Behrman
+13.3%
+13.3% (0.7/5)
 
-0.2
+8 John Monds
+11.7%
+11.7% (0.6/5)
 
-8.7%
-8.7% (0.4/5)
-(0.4/5)
-
-10 Beto O'Rourke
-8.6%
-8.6% (0.4/5)
-(0.4/5)
-
-11 Joe Biden
-8.3%
-8.3% (0.4/5)
-(0.4/5)
+9 Sam Robb
+9.0%
+9.0% (0.5/5)
+(0.5/5)
 
-12 Jay Inslee
 6.4%
 6.4% (0.3/5)
 (0.3/5)
 
-13 Julian Castro
-5.8%
-5.8% (0.3/5)
-(0.3/5)
+11 Arvin Vohra
 
-14 Kirsten Gillibrand
-5.4%
-5.4% (0.3/5)
-(0.3/5)
+919
 
-15 John Kerry
-4.3%
-4.3% (0.2/5)
-(0.2/5)
+0.3
 
-16 John Hickenlooper
-4.0%
-4.0% (0.2/5)
-(0.2/5)
+830
 
-17 John Delaney
-3.5%
-3.5% (0.2/5)
-(0.2/5)
+0.3
 
-STAR elected the Condorcet winner.
-Update Results
+6.3%
+6.3% (0.3/5)
+(0.3/5)
 
-Share
-https://star.vote/demprimary2020/
+12 Brian Ellison
+5.7%
+5.7% (0.3/5)
+(0.3/5)
 
-https://star.vote/demprimary2020/
+https://star.vote/lp2020presmay/
 
 3/5
 
 5/20/23, 7:35 AM
 
-★.✓ - 2020 Democratic Presidential Primary
-
-Runoff Matrix
-Show
-
-Ballot Record
-Download Full CVR:
-
-CSV
-
-Most recent 20 votes:
-Andrew
-Cory
-Pete
-Bernie Elizabeth
-Marriane
-J
-B
-Booker Buttigieg Sanders Warren Williamson
-Yang
-
-Voter ID
-
-Timestamp
-
-Poll ID
-
-f3e9prr5zy
-
-2023-05-17
-14:00:14
-
-ceftnf46 0
-
-2
-
-5
-
-4
-
-1
-
-2
-
-3
-
-kzcy4am69e
-
-2023-05-14
-12:05:52
-
-ceftnf46 4
-
-5
-
-5
-
-5
-
-2
-
-4
-
-1
-
-6fw45edaz9
-
-2023-05-11
-22:26:37
-
-ceftnf46 0
-
-0
-
-5
-
-0
-
-0
-
-0
-
-0
-
-4racn62d6t
-
-2023-05-09
-15:16:09
-
-ceftnf46 5
-
-4
-
-5
-
-4
-
-0
-
-2
-
-3
-
-nf7nndfnrs
-
-2023-05-08
-12:04:44
-
-ceftnf46 5
-
-5
-
-3
-
-3
-
-0
-
-0
-
-4
-
-wmtpaz4z2x
-
-2023-05-06
-21:35:32
-
-ceftnf46 0
-
-2
-
-5
-
-4
-
-2
-
-1
-
-0
-
-n47tetk5x4
+13 Mark Whitney
 
-2023-04-29
-09:30:48
+★.✓ - Libertarian Party 2020 Presidential Nomination - Star Voting Poll: May
 
-ceftnf46 1
+807
 
-0
-
-5
-
-3
-
-3
-
-0
-
-0
-
-c31nr116wy
-
-2023-04-25
-11:00:37
-
-ceftnf46 4
-
-4
-
-5
-
-3
-
-0
-
-1
-
-4
-
-c412zt6rny
-
-2023-04-23
-18:49:43
-
-ceftnf46 0
-
-0
-
-5
-
-4
-
-4
-
-0
-
-1
-
-p7r9y3n2w1
-
-2023-04-20
-17:13:24
-
-ceftnf46 0
-
-1
-
-5
-
-0
-
-4
-
-4
-
-0
-
-tw9y2ymda9
-
-2023-04-18
-06:29:50
-
-ceftnf46 5
-
-0
-
-5
-
-1
-
-0
-
-3
-
-3
-
-55dx95zrc7
-
-2023-04-13
-16:08:22
-
-ceftnf46 3
-
-2
-
-4
-
-4
-
-5
-
-5
-
-0
-
-c456a5x564
-
-2023-04-11
-23:41:42
-
-ceftnf46 1
-
-2
+0.3
 
-5
+687
 
-4
+0.2
 
-5
+660
 
-4
+0.2
 
-1
+613
 
-nza3fm66t9
+0.2
 
-2023-04-11
-12:16:24
+572
 
-ceftnf46 2
+0.2
 
-3
+559
 
-1
+0.2
 
-1
+557
 
-3
+0.2
 
-3
+557
 
-2
+0.2
 
-aen1awrh7e
+546
 
-2023-04-09
-01:59:15
+0.2
 
-ceftnf46 0
+519
 
-0
+0.2
 
-5
+5.5%
+5.5% (0.3/5)
+(0.3/5)
 
-3
+14 Phil Gray
+4.7%
+4.7% (0.2/5)
+(0.2/5)
 
-0
+15 Kenneth Blevins
+4.5%
+4.5% (0.2/5)
+(0.2/5)
 
-4
+16 Jedidiah Hill
+4.2%
+4.2% (0.2/5)
+(0.2/5)
 
-5
+17 Steve Richey
+3.9%
+3.9% (0.2/5)
+(0.2/5)
 
-9cd6acxrxf
+18 Keenan Dunham
+3.8%
+3.8% (0.2/5)
+(0.2/5)
 
-2023-04-07
-08:44:21
+19 Erik Gerhardt
+3.8%
+3.8% (0.2/5)
+(0.2/5)
 
-ceftnf46 2
+20 James Ogle
+3.8%
+3.8% (0.2/5)
+(0.2/5)
 
-5
+21 Rhett Smith
+3.8%
+3.8% (0.2/5)
+(0.2/5)
 
-1
+22 Louis Vanacore
+3.6%
+3.6% (0.2/5)
+(0.2/5)
 
-1
+STAR elected the Condorcet winner.
+Update Results
 
-0
+Share
+https://star.vote/lp2020presmay/
 
-1
+Runoff Matrix
+Show
 
-4
+Ballot Record
 
-https://star.vote/demprimary2020/
+https://star.vote/lp2020presmay/
 
 4/5
 
 5/20/23, 7:35 AM
 
-★.✓ - 2020 Democratic Presidential Primary
-
-sdshhzrsxa
-
-2023-03-28
-17:31:22
-
-ceftnf46 3
-
-4
-
-5
-
-4
-
-1
-
-2
-
-5
-
-pxp4zh1pfm
+★.✓ - Libertarian Party 2020 Presidential Nomination - Star Voting Poll: May
 
-2023-03-27
-18:02:33
-
-ceftnf46 0
-
-1
-
-1
-
-0
-
-0
-
-5
-
-3
-
-1pryxztht9
-
-2023-03-19
-08:08:30
-
-ceftnf46 0
-
-2
-
-5
-
-3
-
-0
-
-3
-
-3
-
-h13e45fsrt
-
-2023-03-14
-13:55:49
-
-ceftnf46 0
-
-5
-
-0
-
-0
-
-0
-
-0
-
-0
+Show
 
 Learn more at starvoting.us
 
-https://star.vote/demprimary2020/
+https://star.vote/lp2020presmay/
 
 5/5
```

### Comparing `starvote-1.5.1/sample_polls/starvote_ballots_2020_libertarian_party_presidential_nomination.csv` & `starvote-2.0/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.5.1/sample_polls/starvote_ballots_2020_libertarian_party_presidential_nomination.result.pdf` & `starvote-2.0/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.pdf`

 * *Files identical despite different names*

### Comparing `starvote-1.5.1/sample_polls/starvote_ballots_best_akali_skins.csv` & `starvote-2.0/test_elections/starvote_ballots_best_akali_skins.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.5.1/sample_polls/starvote_ballots_best_akali_skins.result.pdf` & `starvote-2.0/test_elections/starvote_ballots_best_akali_skins.pdf`

 * *Files identical despite different names*

### Comparing `starvote-1.5.1/sample_polls/starvote_ballots_eurovision_song_contest_2023.csv` & `starvote-2.0/test_elections/starvote_ballots_eurovision_song_contest_2023.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.5.1/sample_polls/starvote_ballots_eurovision_song_contest_2023.result.pdf` & `starvote-2.0/test_elections/starvote_ballots_eurovision_song_contest_2023.pdf`

 * *Files identical despite different names*

### Comparing `starvote-1.5.1/sample_polls/starvote_ballots_libertarian_party_2020_presidential_nomination_may.csv` & `starvote-2.0/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.5.1/sample_polls/starvote_ballots_libertarian_party_2020_presidential_nomination_may.result.pdf` & `starvote-2.0/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 10% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,10 +1,10 @@
 5/20/23, 7:35 AM
 
-★.✓ - Libertarian Party 2020 Presidential Nomination - Star Voting Poll: May
+★.✓ - UPDATED 2020 Libertarian Presidential Candidate
 
 .vote
 
 More
 
 Learn
 
@@ -12,352 +12,304 @@
 
 You may score as many candidates as you like from 0 (no support) to 5 (max support).
 You may give the same score to multiple candidates.
 The two highest-scoring candidates are finalists.
 The finalist scored higher by more voters wins.
 Votes are limited to one per IP address.
 
-Vote on "Libertarian Party 2020 Presidential Nomination - Star Voting
-Poll: May"
-Ended: 2020-05-31 23:59:00
+Vote on "UPDATED 2020 Libertarian Presidential Candidate"
+Ended: 2020-05-26 00:00:00
 
-Vermin Supreme
+Keenan Dunham
 0
 
-Phil Gray
+Judge Jim Gray
 0
 
-Brian Ellison
+Erik Gerhardt
 0
 
-John Monds
+Jo Jorgensen
 0
 
-Jedidiah Hill
+Phil Gray
 0
 
-James Ogle
+Sorinne Ardeleanu
 0
 
-Jacob Hornberger
+Sam Robb
 0
 
 Louis Vanacore
 0
 
-Keenan Dunham
-https://star.vote/lp2020presmay/
+Steve Richey
+0
+https://star.vote/dd1wc4yx/
 
-1/5
+1/4
 
 5/20/23, 7:35 AM
 
-★.✓ - Libertarian Party 2020 Presidential Nomination - Star Voting Poll: May
-
-0
-
-Daniel Behrman
-0
+★.✓ - UPDATED 2020 Libertarian Presidential Candidate
 
-Sam Robb
+Brian Ellison
 0
 
-Mark Whitney
+Dan Behrman
 0
 
-Erik Gerhardt
+Vermin Supreme
 0
 
-Sorinne Ardeleanu
+Adam Kokesh
 0
 
 Arvin Vohra
 0
 
-Jo Jorgensen
+Jedidiah Hill
 0
 
-Kenneth Blevins
+Souraya Faas
 0
 
-Justin Amash
+Kenneth Blevins
 0
 
-Adam Kokesh
+Jacob Hornberger
 0
 
-Judge Jim Gray
+John Monds
 0
 
-Steve Richey
-https://star.vote/lp2020presmay/
-
-2/5
-
-5/20/23, 7:35 AM
+Vote!
 
-★.✓ - Libertarian Party 2020 Presidential Nomination - Star Voting Poll: May
+Show Results
 
-0
+Results for "UPDATED 2020 Libertarian Presidential Candidate"
+https://star.vote/dd1wc4yx/
 
-Rhett Smith
-0
+2/4
 
-Vote!
+5/20/23, 7:35 AM
 
-Show Results
+★.✓ - UPDATED 2020 Libertarian Presidential Candidate
 
-Results for "Libertarian Party 2020 Presidential Nomination - Star
-Voting Poll: May"
 Selection Phase (Top two advance):
-2909 voters
-
-→ 1 Justin Amash
-# Option
-
+1534 voters
 # Option
 
 Points Average
 
-1 Justin Amash
+3.0
 
-8018
+60.7%
+60.7% (3.0/5)
 
-2.8
+3008
 
-55.1%
-55.1% (2.8/5)
+2.0
 
-2 Vermin Supreme 7200
+2012
 
-2.5
-
-49.5%
-49.5% (2.5/5)
+1.3
 
-3826
+4 Jacob Hornberger 2011
 
 1.3
 
-4 Jacob Hornberger 3193
+39.2%
+39.2% (2.0/5)
+
+3 Jo Jorgensen
 
-1.1
+→ 1 Vermin Supreme 830
+# Option
 
-3 Judge Jim Gray
+1 Vermin Supreme 4653
+2 Judge Jim Gray
 
 Runoff Phase (Single winner):
 Votes
 
-1404
+54.11% (830/1534)
+
+2 Judge Jim Gray
 
-48.26% (1404/2909)
+519
 
-2 Vermin Supreme 1138
-39.12% (1138/2909)
+33.83% (519/1534)
 
 No Preference
 
-367
+185
 
-12.62% (367/2909)
+12.06% (185/1534)
 
-26.3%
-26.3% (1.3/5)
+26.2%
+26.2% (1.3/5)
 
-22.0%
-22.0% (1.1/5)
+26.2%
+26.2% (1.3/5)
 
-2625
+1403
 
 0.9
 
-2324
-
-0.8
-
-1941
+1132
 
 0.7
 
-1707
-
-0.6
-
-1315
+1050
 
-0.5
-
-10 Sorinne Ardeleanu 929
-
-0.3
-
-5 Jo Jorgensen
-18.0%
-18.0% (0.9/5)
-
-6 Adam Kokesh
-16.0%
-16.0% (0.8/5)
-
-7 Daniel Behrman
-13.3%
-13.3% (0.7/5)
-
-8 John Monds
-11.7%
-11.7% (0.6/5)
-
-9 Sam Robb
-9.0%
-9.0% (0.5/5)
-(0.5/5)
+0.7
 
-6.4%
-6.4% (0.3/5)
-(0.3/5)
+596
 
-11 Arvin Vohra
+0.4
 
-919
+9 Sorinne Ardeleanu 483
 
 0.3
 
-830
-
-0.3
+5 Adam Kokesh
+18.3%
+18.3% (0.9/5)
+
+6 John Monds
+14.8%
+14.8% (0.7/5)
+
+7 Dan Behrman
+13.7%
+13.7% (0.7/5)
+
+8 Sam Robb
+7.8%
+7.8% (0.4/5)
+(0.4/5)
 
 6.3%
 6.3% (0.3/5)
 (0.3/5)
 
-12 Brian Ellison
-5.7%
-5.7% (0.3/5)
-(0.3/5)
-
-https://star.vote/lp2020presmay/
-
-3/5
-
-5/20/23, 7:35 AM
+10 Arvin Vohra
 
-13 Mark Whitney
-
-★.✓ - Libertarian Party 2020 Presidential Nomination - Star Voting Poll: May
-
-807
+477
 
 0.3
 
-687
+450
 
-0.2
+0.3
 
-660
+390
 
-0.2
+0.3
 
-613
+383
 
 0.2
 
-572
+376
 
 0.2
 
-559
+299
 
 0.2
 
-557
+296
 
 0.2
 
-557
+293
 
 0.2
 
-546
+292
 
 0.2
 
-519
+6.2%
+6.2% (0.3/5)
+(0.3/5)
 
-0.2
+11 Brian Ellison
+5.9%
+5.9% (0.3/5)
+(0.3/5)
 
-5.5%
-5.5% (0.3/5)
+12 Kenneth Blevins
+5.1%
+5.1% (0.3/5)
 (0.3/5)
 
-14 Phil Gray
-4.7%
-4.7% (0.2/5)
+13 Phil Gray
+5.0%
+5.0% (0.2/5)
 (0.2/5)
 
-15 Kenneth Blevins
-4.5%
-4.5% (0.2/5)
+14 Souraya Faas
+4.9%
+4.9% (0.2/5)
 (0.2/5)
 
-16 Jedidiah Hill
-4.2%
-4.2% (0.2/5)
+15 Erik Gerhardt
+3.9%
+3.9% (0.2/5)
 (0.2/5)
 
-17 Steve Richey
+16 Steve Richey
 3.9%
 3.9% (0.2/5)
 (0.2/5)
 
-18 Keenan Dunham
+17 Keenan Dunham
 3.8%
 3.8% (0.2/5)
 (0.2/5)
 
-19 Erik Gerhardt
+18 Jedidiah Hill
 3.8%
 3.8% (0.2/5)
 (0.2/5)
 
-20 James Ogle
-3.8%
-3.8% (0.2/5)
-(0.2/5)
+https://star.vote/dd1wc4yx/
 
-21 Rhett Smith
-3.8%
-3.8% (0.2/5)
-(0.2/5)
+3/4
 
-22 Louis Vanacore
-3.6%
-3.6% (0.2/5)
+5/20/23, 7:35 AM
+
+19 Louis Vanacore
+
+★.✓ - UPDATED 2020 Libertarian Presidential Candidate
+
+263
+
+0.2
+
+3.4%
+3.4% (0.2/5)
 (0.2/5)
 
 STAR elected the Condorcet winner.
 Update Results
 
 Share
-https://star.vote/lp2020presmay/
+https://star.vote/dd1wc4yx/
 
 Runoff Matrix
 Show
 
 Ballot Record
-
-https://star.vote/lp2020presmay/
-
-4/5
-
-5/20/23, 7:35 AM
-
-★.✓ - Libertarian Party 2020 Presidential Nomination - Star Voting Poll: May
-
 Show
 
 Learn more at starvoting.us
 
-https://star.vote/lp2020presmay/
+https://star.vote/dd1wc4yx/
 
-5/5
+4/4
```

### Comparing `starvote-1.5.1/sample_polls/starvote_ballots_presidential_candidates.csv` & `starvote-2.0/test_elections/starvote_ballots_presidential_candidates.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.5.1/sample_polls/starvote_ballots_presidential_candidates.result.pdf` & `starvote-2.0/test_elections/starvote_ballots_presidential_candidates.pdf`

 * *Files identical despite different names*

### Comparing `starvote-1.5.1/sample_polls/starvote_ballots_presidential_poll_july_2020.csv` & `starvote-2.0/test_elections/starvote_ballots_presidential_poll_july_2020.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.5.1/sample_polls/starvote_ballots_presidential_poll_july_2020.result.pdf` & `starvote-2.0/test_elections/starvote_ballots_presidential_poll_july_2020.pdf`

 * *Files identical despite different names*

### Comparing `starvote-1.5.1/sample_polls/starvote_ballots_updated_2020_libertarian_presidential_candidate.csv` & `starvote-2.0/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.5.1/sample_polls/starvote_ballots_updated_2020_libertarian_presidential_candidate.result.txt` & `starvote-2.0/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,33 @@
-[STAR]
-[Score round]
-  Vermin Supreme    -- 4653 (average 3.03)
-  Judge Jim Gray    -- 3008 (average 1.96)
-  Jo Jorgensen      -- 2012 (average 1.31)
-  Jacob Hornberger  -- 2011 (average 1.31)
-  Adam Kokesh       -- 1403 (average 0.91)
-  John Monds        -- 1132 (average 0.74)
-  Dan Behrman       -- 1050 (average 0.68)
-  Sam Robb          --  596 (average 0.39)
-  Sorinne Ardeleanu --  483 (average 0.31)
-  Arvin Vohra       --  477 (average 0.31)
-  Brian Ellison     --  450 (average 0.29)
-  Kenneth Blevins   --  390 (average 0.25)
-  Phil Gray         --  383 (average 0.25)
-  Souraya Faas      --  376 (average 0.25)
-  Erik Gerhardt     --  299 (average 0.19)
-  Steve Richey      --  296 (average 0.19)
-  Keenan Dunham     --  293 (average 0.19)
-  Jedidiah Hill     --  292 (average 0.19)
-  Louis Vanacore    --  263 (average 0.17)
-[Automatic runoff round]
-  Vermin Supreme -- 830
-  Judge Jim Gray -- 519
-  No preference  -- 185
-[Winner]
+[STAR Voting]
+  Tabulating 718 ballots.
+  Maximum score is 5.
+[STAR Voting: Scoring Round]
+  The two highest-scoring candidates advance to the next round.
+    Vermin Supreme    -- 2865 (average 3+711/718) -- First place
+    Dan Behrman       --  708 (average 354/359)   -- Second place
+    Jacob Hornberger  --  703 (average 703/718)
+    John McAfee       --  584 (average 292/359)
+    Lincoln Chafee    --  340 (average 170/359)
+    Jo Jorgensen      --  333 (average 333/718)
+    John Monds        --  299 (average 299/718)
+    Ken Armstrong     --  263 (average 263/718)
+    Mark Whitney      --  259 (average 259/718)
+    Arvin Vohra       --  186 (average  93/359)
+    Max Abramson      --  184 (average  92/359)
+    Sam Robb          --  170 (average  85/359)
+    Jedi Hill         --  136 (average  68/359)
+    Souraya Fass      --  128 (average  64/359)
+    Sorinne Ardeleanu --  112 (average  56/359)
+    Ben Leder         --   97 (average  97/718)
+    Keenan Dunham     --   96 (average  48/359)
+    Erik Gerhardt     --   95 (average  95/718)
+    James Ogle        --   86 (average  43/359)
+  Vermin Supreme and Dan Behrman advance.
+[STAR Voting: Automatic Runoff Round]
+  The candidate preferred in the most head-to-head matchups wins.
+    Vermin Supreme -- 541 -- First place
+    Dan Behrman    --  77
+    No Preference  -- 100
+  Vermin Supreme wins.
+[STAR Voting: Winner]
   Vermin Supreme
```

### Comparing `starvote-1.5.1/sample_polls/starvote_ballots_wa_governor_2020_republican_party_straw_poll.csv` & `starvote-2.0/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.5.1/sample_polls/starvote_ballots_wa_governor_2020_republican_party_straw_poll.result.pdf` & `starvote-2.0/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.pdf`

 * *Files identical despite different names*

