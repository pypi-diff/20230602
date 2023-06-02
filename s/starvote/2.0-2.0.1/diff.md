# Comparing `tmp/starvote-2.0.tar.gz` & `tmp/starvote-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starvote-2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "starvote-2.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `starvote-2.0.tar` & `starvote-2.0.1.tar`

### file list

```diff
@@ -1,161 +1,161 @@
--rw-r--r--   0        0        0       38 2023-05-27 15:21:37.716345 starvote-2.0/.gitignore
--rw-r--r--   0        0        0     1087 2023-05-20 12:48:55.372092 starvote-2.0/LICENSE
--rw-r--r--   0        0        0    32170 2023-06-02 19:51:22.344081 starvote-2.0/README.md
--rw-r--r--   0        0        0    15825 2023-06-01 10:48:31.686649 starvote-2.0/docs/clarifying_star_voting.md
--rw-r--r--   0        0        0     2743 2023-05-31 19:56:48.827782 starvote-2.0/docs/formatting_fractions_in_columns_of_text.txt
--rw-r--r--   0        0        0      217 2023-05-31 21:13:55.136896 starvote-2.0/example.py
--rw-r--r--   0        0        0      583 2023-06-02 19:49:52.947305 starvote-2.0/pyproject.toml
--rw-r--r--   0        0        0    90421 2023-06-02 19:29:39.644773 starvote-2.0/starvote/__init__.py
--rw-r--r--   0        0        0      106 2023-06-02 00:43:16.709978 starvote-2.0/starvote/__main__.py
--rw-r--r--   0        0        0     5809 2023-06-02 18:28:35.340765 starvote-2.0/starvote/reference.py
--rw-r--r--   0        0        0     1051 2023-06-02 01:09:12.579780 starvote-2.0/test_elections/README.md
--rw-r--r--   0        0        0       84 2023-06-01 23:43:37.846114 starvote-2.0/test_elections/bad_syntax_ballot_pragma_as_last_line.starvote
--rw-r--r--   0        0        0     1358 2023-06-02 19:23:34.765586 starvote-2.0/test_elections/bad_syntax_ballot_pragma_as_last_line.txt
--rw-r--r--   0        0        0       68 2023-06-01 23:24:50.800081 starvote-2.0/test_elections/bad_syntax_change_section_in_list.starvote
--rw-r--r--   0        0        0     1395 2023-06-02 19:23:34.765586 starvote-2.0/test_elections/bad_syntax_change_section_in_list.txt
--rw-r--r--   0        0        0       68 2023-06-01 23:23:06.267150 starvote-2.0/test_elections/bad_syntax_fussy_wrong_ballots_1.starvote
--rw-r--r--   0        0        0     1404 2023-06-02 19:23:34.769586 starvote-2.0/test_elections/bad_syntax_fussy_wrong_ballots_1.txt
--rw-r--r--   0        0        0       67 2023-06-01 23:23:00.095096 starvote-2.0/test_elections/bad_syntax_fussy_wrong_ballots_2.starvote
--rw-r--r--   0        0        0     1402 2023-06-02 19:23:34.769586 starvote-2.0/test_elections/bad_syntax_fussy_wrong_ballots_2.txt
--rw-r--r--   0        0        0       35 2023-06-02 19:31:20.821653 starvote-2.0/test_elections/bad_syntax_invalid_method.starvote
--rw-r--r--   0        0        0     1375 2023-06-02 19:31:54.613947 starvote-2.0/test_elections/bad_syntax_invalid_method.txt
--rw-r--r--   0        0        0       40 2023-06-01 23:17:55.140381 starvote-2.0/test_elections/bad_syntax_invalid_option.starvote
--rw-r--r--   0        0        0     1374 2023-06-02 19:23:34.769586 starvote-2.0/test_elections/bad_syntax_invalid_option.txt
--rw-r--r--   0        0        0       44 2023-06-01 23:16:35.203670 starvote-2.0/test_elections/bad_syntax_invalid_pragma.starvote
--rw-r--r--   0        0        0     1376 2023-06-02 19:23:34.769586 starvote-2.0/test_elections/bad_syntax_invalid_pragma.txt
--rw-r--r--   0        0        0       89 2023-06-01 23:37:41.946945 starvote-2.0/test_elections/bad_syntax_invalid_start_of_line_mode.starvote
--rw-r--r--   0        0        0     1335 2023-06-02 19:23:34.769586 starvote-2.0/test_elections/bad_syntax_invalid_start_of_line_mode.txt
--rw-r--r--   0        0        0       50 2023-06-01 23:14:06.126343 starvote-2.0/test_elections/bad_syntax_invalid_starvote_path_1.starvote
--rw-r--r--   0        0        0     1331 2023-06-02 19:23:34.769586 starvote-2.0/test_elections/bad_syntax_invalid_starvote_path_1.txt
--rw-r--r--   0        0        0       70 2023-06-01 23:28:17.369920 starvote-2.0/test_elections/bad_syntax_invalid_starvote_path_2.starvote
--rw-r--r--   0        0        0     1360 2023-06-02 19:23:34.769586 starvote-2.0/test_elections/bad_syntax_invalid_starvote_path_2.txt
--rw-r--r--   0        0        0       38 2023-06-01 23:13:26.765992 starvote-2.0/test_elections/bad_syntax_invalid_tiebreaker.starvote
--rw-r--r--   0        0        0     1382 2023-06-02 19:23:34.769586 starvote-2.0/test_elections/bad_syntax_invalid_tiebreaker.txt
--rw-r--r--   0        0        0       59 2023-06-02 02:02:11.939956 starvote-2.0/test_elections/bad_syntax_malformed_section.starvote
--rw-r--r--   0        0        0     1371 2023-06-02 19:23:34.769586 starvote-2.0/test_elections/bad_syntax_malformed_section.txt
--rw-r--r--   0        0        0       41 2023-06-01 23:44:44.538707 starvote-2.0/test_elections/bad_syntax_no_ballots.starvote
--rw-r--r--   0        0        0     1314 2023-06-02 19:23:34.769586 starvote-2.0/test_elections/bad_syntax_no_ballots.txt
--rw-r--r--   0        0        0       44 2023-06-01 23:34:09.385053 starvote-2.0/test_elections/bad_syntax_no_equals.starvote
--rw-r--r--   0        0        0     1346 2023-06-02 19:23:34.769586 starvote-2.0/test_elections/bad_syntax_no_equals.txt
--rw-r--r--   0        0        0       59 2023-06-02 01:03:50.036922 starvote-2.0/test_elections/bad_syntax_no_method.starvote
--rw-r--r--   0        0        0     1409 2023-06-02 19:23:34.769586 starvote-2.0/test_elections/bad_syntax_no_method.txt
--rw-r--r--   0        0        0       46 2023-06-01 23:32:02.351922 starvote-2.0/test_elections/bad_syntax_no_section.starvote
--rw-r--r--   0        0        0     1364 2023-06-02 19:23:34.769586 starvote-2.0/test_elections/bad_syntax_no_section.txt
--rw-r--r--   0        0        0       47 2023-06-01 23:21:20.118206 starvote-2.0/test_elections/bad_syntax_pragma_in_options.starvote
--rw-r--r--   0        0        0     1375 2023-06-02 19:23:34.769586 starvote-2.0/test_elections/bad_syntax_pragma_in_options.txt
--rw-r--r--   0        0        0      103 2023-06-01 23:32:48.848336 starvote-2.0/test_elections/bad_syntax_pragma_inside_list.starvote
--rw-r--r--   0        0        0     1387 2023-06-02 19:23:34.769586 starvote-2.0/test_elections/bad_syntax_pragma_inside_list.txt
--rw-r--r--   0        0        0       47 2023-06-01 23:18:10.564519 starvote-2.0/test_elections/bad_syntax_repeated_option.starvote
--rw-r--r--   0        0        0     1380 2023-06-02 19:23:34.769586 starvote-2.0/test_elections/bad_syntax_repeated_option.txt
--rw-r--r--   0        0        0       60 2023-06-01 23:31:08.239441 starvote-2.0/test_elections/bad_syntax_repeated_section.starvote
--rw-r--r--   0        0        0     1383 2023-06-02 19:23:34.769586 starvote-2.0/test_elections/bad_syntax_repeated_section.txt
--rw-r--r--   0        0        0    57750 2023-05-20 12:04:29.149807 starvote-2.0/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.csv
--rw-r--r--   0        0        0   575556 2023-05-20 14:35:00.177319 starvote-2.0/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.pdf
--rw-r--r--   0        0        0     1403 2023-06-02 19:23:34.773586 starvote-2.0/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.txt
--rw-r--r--   0        0        0   115221 2023-05-27 14:48:58.735061 starvote-2.0/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.csv
--rw-r--r--   0        0        0   410807 2023-05-27 14:59:16.160516 starvote-2.0/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.pdf
--rw-r--r--   0        0        0     3193 2023-06-02 19:23:34.785586 starvote-2.0/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.txt
--rw-r--r--   0        0        0    49711 2023-05-20 12:04:34.029848 starvote-2.0/test_elections/starvote_ballots_best_akali_skins.csv
--rw-r--r--   0        0        0   538128 2023-05-20 14:33:25.560528 starvote-2.0/test_elections/starvote_ballots_best_akali_skins.pdf
--rw-r--r--   0        0        0     1331 2023-06-02 19:23:34.789586 starvote-2.0/test_elections/starvote_ballots_best_akali_skins.txt
--rw-r--r--   0        0        0     1812 2023-05-20 10:35:18.365110 starvote-2.0/test_elections/starvote_ballots_eurovision_song_contest_2023.csv
--rw-r--r--   0        0        0   807144 2023-05-20 14:33:51.120742 starvote-2.0/test_elections/starvote_ballots_eurovision_song_contest_2023.pdf
--rw-r--r--   0        0        0     2879 2023-06-02 19:23:34.789586 starvote-2.0/test_elections/starvote_ballots_eurovision_song_contest_2023.txt
--rw-r--r--   0        0        0   250538 2023-05-20 10:34:04.044490 starvote-2.0/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.csv
--rw-r--r--   0        0        0   643536 2023-05-20 14:35:41.153662 starvote-2.0/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.pdf
--rw-r--r--   0        0        0     1596 2023-06-02 19:23:34.809586 starvote-2.0/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.txt
--rw-r--r--   0        0        0      175 2023-06-02 19:18:28.166907 starvote-2.0/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_bloc_star.starvote
--rw-r--r--   0        0        0    12586 2023-06-02 19:23:35.117589 starvote-2.0/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_bloc_star.txt
--rw-r--r--   0        0        0      141 2023-06-02 19:18:26.038889 starvote-2.0/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_star_pr.starvote
--rw-r--r--   0        0        0    12586 2023-06-02 19:23:35.429592 starvote-2.0/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_star_pr.txt
--rw-r--r--   0        0        0    31534 2023-05-20 12:04:38.493885 starvote-2.0/test_elections/starvote_ballots_presidential_candidates.csv
--rw-r--r--   0        0        0   325033 2023-05-20 14:34:17.572963 starvote-2.0/test_elections/starvote_ballots_presidential_candidates.pdf
--rw-r--r--   0        0        0      814 2023-06-02 19:23:35.433591 starvote-2.0/test_elections/starvote_ballots_presidential_candidates.txt
--rw-r--r--   0        0        0    48454 2023-05-20 12:04:25.689778 starvote-2.0/test_elections/starvote_ballots_presidential_poll_july_2020.csv
--rw-r--r--   0        0        0   360427 2023-05-20 14:36:25.050030 starvote-2.0/test_elections/starvote_ballots_presidential_poll_july_2020.pdf
--rw-r--r--   0        0        0      799 2023-06-02 19:23:35.433591 starvote-2.0/test_elections/starvote_ballots_presidential_poll_july_2020.txt
--rw-r--r--   0        0        0   123039 2023-05-20 12:04:13.781679 starvote-2.0/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.csv
--rw-r--r--   0        0        0   584998 2023-05-20 14:35:22.465506 starvote-2.0/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.pdf
--rw-r--r--   0        0        0     1434 2023-06-02 19:23:35.441592 starvote-2.0/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.txt
--rw-r--r--   0        0        0    52870 2023-05-20 12:04:22.533752 starvote-2.0/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.csv
--rw-r--r--   0        0        0   354740 2023-05-20 14:36:48.550226 starvote-2.0/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.pdf
--rw-r--r--   0        0        0      747 2023-06-02 19:23:35.445592 starvote-2.0/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.txt
--rw-r--r--   0        0        0      146 2023-06-01 14:23:14.825743 starvote-2.0/test_elections/test_election_all_fives_bloc_star.starvote
--rw-r--r--   0        0        0     1080 2023-06-02 19:23:35.445592 starvote-2.0/test_elections/test_election_all_fives_bloc_star.txt
--rw-r--r--   0        0        0      145 2023-06-01 14:23:10.941709 starvote-2.0/test_elections/test_election_all_fives_rrv.starvote
--rw-r--r--   0        0        0      484 2023-06-02 19:23:35.445592 starvote-2.0/test_elections/test_election_all_fives_rrv.txt
--rw-r--r--   0        0        0      151 2023-06-02 19:18:20.314839 starvote-2.0/test_elections/test_election_all_fives_star-pr.starvote
--rw-r--r--   0        0        0      476 2023-06-02 19:23:35.445592 starvote-2.0/test_elections/test_election_all_fives_star-pr.txt
--rw-r--r--   0        0        0      132 2023-06-01 14:23:02.245634 starvote-2.0/test_elections/test_election_all_fives_star.starvote
--rw-r--r--   0        0        0     1030 2023-06-02 19:23:35.445592 starvote-2.0/test_elections/test_election_all_fives_star.txt
--rw-r--r--   0        0        0      146 2023-06-01 14:23:30.837882 starvote-2.0/test_elections/test_election_all_threes_bloc_star.starvote
--rw-r--r--   0        0        0     1080 2023-06-02 19:23:35.445592 starvote-2.0/test_elections/test_election_all_threes_bloc_star.txt
--rw-r--r--   0        0        0       92 2023-06-01 22:34:03.536957 starvote-2.0/test_elections/test_election_all_threes_rrv.starvote
--rw-r--r--   0        0        0      484 2023-06-02 19:23:35.449592 starvote-2.0/test_elections/test_election_all_threes_rrv.txt
--rw-r--r--   0        0        0       98 2023-06-02 19:18:18.286821 starvote-2.0/test_elections/test_election_all_threes_star-pr.starvote
--rw-r--r--   0        0        0      476 2023-06-02 19:23:35.449592 starvote-2.0/test_elections/test_election_all_threes_star-pr.txt
--rw-r--r--   0        0        0      132 2023-06-01 14:23:19.233781 starvote-2.0/test_elections/test_election_all_threes_star.starvote
--rw-r--r--   0        0        0     1030 2023-06-02 19:23:35.449592 starvote-2.0/test_elections/test_election_all_threes_star.txt
--rw-r--r--   0        0        0      146 2023-06-01 14:19:42.607904 starvote-2.0/test_elections/test_election_all_zeroes_bloc_star.starvote
--rw-r--r--   0        0        0     1077 2023-06-02 19:23:35.449592 starvote-2.0/test_elections/test_election_all_zeroes_bloc_star.txt
--rw-r--r--   0        0        0      145 2023-06-01 14:19:40.835888 starvote-2.0/test_elections/test_election_all_zeroes_rrv.starvote
--rw-r--r--   0        0        0      481 2023-06-02 19:23:35.449592 starvote-2.0/test_elections/test_election_all_zeroes_rrv.txt
--rw-r--r--   0        0        0      151 2023-06-02 19:18:15.894800 starvote-2.0/test_elections/test_election_all_zeroes_star-pr.starvote
--rw-r--r--   0        0        0      473 2023-06-02 19:23:35.449592 starvote-2.0/test_elections/test_election_all_zeroes_star-pr.txt
--rw-r--r--   0        0        0      132 2023-06-01 14:19:46.079934 starvote-2.0/test_elections/test_election_all_zeroes_star.starvote
--rw-r--r--   0        0        0     1027 2023-06-02 19:23:35.449592 starvote-2.0/test_elections/test_election_all_zeroes_star.txt
--rw-r--r--   0        0        0     2660 2023-05-31 22:55:06.890838 starvote-2.0/test_elections/test_election_bloc_star_and_electowiki.starvote
--rw-r--r--   0        0        0     3383 2023-06-02 19:23:35.449592 starvote-2.0/test_elections/test_election_bloc_star_and_electowiki.txt
--rw-r--r--   0        0        0      989 2023-05-31 14:32:27.710655 starvote-2.0/test_elections/test_election_bloc_star_unbreakable_tie_for_first.starvote
--rw-r--r--   0        0        0     1606 2023-06-02 19:23:35.449592 starvote-2.0/test_elections/test_election_bloc_star_unbreakable_tie_for_first.txt
--rw-r--r--   0        0        0      201 2023-05-31 14:32:09.618494 starvote-2.0/test_elections/test_election_breakable_tie_for_second_in_score_round.starvote
--rw-r--r--   0        0        0      831 2023-06-02 19:23:35.449592 starvote-2.0/test_elections/test_election_breakable_tie_for_second_in_score_round.txt
--rw-r--r--   0        0        0      204 2023-05-31 14:31:42.454252 starvote-2.0/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.starvote
--rw-r--r--   0        0        0      965 2023-06-02 19:23:35.449592 starvote-2.0/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.txt
--rw-r--r--   0        0        0      203 2023-05-31 14:31:18.974043 starvote-2.0/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_score_round.starvote
--rw-r--r--   0        0        0      744 2023-06-02 19:23:35.453592 starvote-2.0/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_score_round.txt
--rw-r--r--   0        0        0      838 2023-05-31 14:31:04.393913 starvote-2.0/test_elections/test_election_demonstrate_cloneproofness_1.starvote
--rw-r--r--   0        0        0      542 2023-06-02 19:23:35.453592 starvote-2.0/test_elections/test_election_demonstrate_cloneproofness_1.txt
--rw-r--r--   0        0        0      830 2023-05-31 14:09:22.654324 starvote-2.0/test_elections/test_election_demonstrate_cloneproofness_2.starvote
--rw-r--r--   0        0        0     1087 2023-06-02 19:23:35.453592 starvote-2.0/test_elections/test_election_demonstrate_cloneproofness_2.txt
--rw-r--r--   0        0        0      194 2023-06-01 16:45:03.487305 starvote-2.0/test_elections/test_election_extra_candidates_in_permutation.starvote
--rw-r--r--   0        0        0      142 2023-06-02 19:23:35.453592 starvote-2.0/test_elections/test_election_extra_candidates_in_permutation.txt
--rw-r--r--   0        0        0      165 2023-06-01 16:45:09.147349 starvote-2.0/test_elections/test_election_incomplete_permutation.starvote
--rw-r--r--   0        0        0      138 2023-06-02 19:23:35.453592 starvote-2.0/test_elections/test_election_incomplete_permutation.txt
--rw-r--r--   0        0        0      132 2023-06-02 01:44:01.610291 starvote-2.0/test_elections/test_election_no_output.starvote
--rw-r--r--   0        0        0       17 2023-06-02 19:23:35.453592 starvote-2.0/test_elections/test_election_no_output.txt
--rw-r--r--   0        0        0      130 2023-06-01 16:34:20.926370 starvote-2.0/test_elections/test_election_no_permuted_candidates_tiebreaker.starvote
--rw-r--r--   0        0        0     1329 2023-06-02 19:23:35.453592 starvote-2.0/test_elections/test_election_no_permuted_candidates_tiebreaker.txt
--rw-r--r--   0        0        0      131 2023-06-01 17:57:44.689602 starvote-2.0/test_elections/test_election_only_one_candidate_star.starvote
--rw-r--r--   0        0        0      505 2023-06-02 19:23:35.453592 starvote-2.0/test_elections/test_election_only_one_candidate_star.txt
--rw-r--r--   0        0        0      177 2023-06-01 17:57:23.633416 starvote-2.0/test_elections/test_election_only_two_candidates_bloc_star.starvote
--rw-r--r--   0        0        0      487 2023-06-02 19:23:35.453592 starvote-2.0/test_elections/test_election_only_two_candidates_bloc_star.txt
--rw-r--r--   0        0        0      176 2023-06-01 17:57:20.909392 starvote-2.0/test_elections/test_election_only_two_candidates_rrv.starvote
--rw-r--r--   0        0        0      523 2023-06-02 19:23:35.453592 starvote-2.0/test_elections/test_election_only_two_candidates_rrv.txt
--rw-r--r--   0        0        0      182 2023-06-02 19:18:13.310778 starvote-2.0/test_elections/test_election_only_two_candidates_star-pr.starvote
--rw-r--r--   0        0        0      545 2023-06-02 19:23:35.453592 starvote-2.0/test_elections/test_election_only_two_candidates_star-pr.txt
--rw-r--r--   0        0        0      319 2023-06-02 19:18:05.042705 starvote-2.0/test_elections/test_election_proportional_star_unbreakable_tie.starvote
--rw-r--r--   0        0        0      480 2023-06-02 19:23:35.453592 starvote-2.0/test_elections/test_election_proportional_star_unbreakable_tie.txt
--rw-r--r--   0        0        0     5899 2023-05-22 07:24:36.945502 starvote-2.0/test_elections/test_election_reweighted_range_sample_election.html
--rw-r--r--   0        0        0      450 2023-05-31 14:05:31.788268 starvote-2.0/test_elections/test_election_reweighted_range_sample_election.starvote
--rw-r--r--   0        0        0     1150 2023-06-02 19:23:35.457592 starvote-2.0/test_elections/test_election_reweighted_range_sample_election.txt
--rw-r--r--   0        0        0      203 2023-05-31 14:05:02.452007 starvote-2.0/test_elections/test_election_unbreakable_three_way_tie_for_first_in_score_round.starvote
--rw-r--r--   0        0        0     1023 2023-06-02 19:23:35.457592 starvote-2.0/test_elections/test_election_unbreakable_three_way_tie_for_first_in_score_round.txt
--rw-r--r--   0        0        0      306 2023-06-01 18:06:23.106174 starvote-2.0/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round.starvote
--rw-r--r--   0        0        0     1788 2023-06-02 19:23:35.457592 starvote-2.0/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round.txt
--rw-r--r--   0        0        0      143 2023-06-02 19:18:03.054688 starvote-2.0/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_star-pr.starvote
--rw-r--r--   0        0        0     2029 2023-06-02 19:23:35.457592 starvote-2.0/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_star-pr.txt
--rw-r--r--   0        0        0      203 2023-05-31 14:04:09.035532 starvote-2.0/test_elections/test_election_unbreakable_tie_for_second_in_score_round.starvote
--rw-r--r--   0        0        0      938 2023-06-02 19:23:35.457592 starvote-2.0/test_elections/test_election_unbreakable_tie_for_second_in_score_round.txt
--rw-r--r--   0        0        0      155 2023-05-28 20:58:05.118365 starvote-2.0/test_elections/test_election_unbreakable_tie_in_automatic_runoff_round.starvote
--rw-r--r--   0        0        0     1081 2023-06-02 19:23:35.457592 starvote-2.0/test_elections/test_election_unbreakable_tie_in_automatic_runoff_round.txt
--rw-r--r--   0        0        0      150 2023-06-01 14:49:33.615373 starvote-2.0/test_elections/test_election_use_just_raise_tiebreaker.starvote
--rw-r--r--   0        0        0     1197 2023-06-02 19:23:35.457592 starvote-2.0/test_elections/test_election_use_just_raise_tiebreaker.txt
--rw-r--r--   0        0        0      154 2023-06-01 16:06:23.349484 starvote-2.0/test_elections/test_election_use_no_description_tiebreaker.starvote
--rw-r--r--   0        0        0     1030 2023-06-02 19:23:35.457592 starvote-2.0/test_elections/test_election_use_no_description_tiebreaker.txt
--rw-r--r--   0        0        0      152 2023-06-01 16:08:48.230596 starvote-2.0/test_elections/test_election_use_only_heading_tiebreaker.starvote
--rw-r--r--   0        0        0      152 2023-06-02 19:23:35.457592 starvote-2.0/test_elections/test_election_use_only_heading_tiebreaker.txt
--rw-r--r--   0        0        0    35726 2023-06-02 19:26:39.999204 starvote-2.0/tests/run_tests.py
--rwxr-xr-x   0        0        0     2211 2023-06-02 19:34:15.379168 starvote-2.0/tools/is_ok
--rwxr-xr-x   0        0        0     1827 2023-06-02 18:03:13.135277 starvote-2.0/tools/remake_test_elections_output
--rw-r--r--   0        0        0    32738 1970-01-01 00:00:00.000000 starvote-2.0/PKG-INFO
+-rw-r--r--   0        0        0       38 2023-05-27 15:21:37.716345 starvote-2.0.1/.gitignore
+-rw-r--r--   0        0        0     1087 2023-05-20 12:48:55.372092 starvote-2.0.1/LICENSE
+-rw-r--r--   0        0        0    32302 2023-06-02 20:05:55.863662 starvote-2.0.1/README.md
+-rw-r--r--   0        0        0    15825 2023-06-01 10:48:31.686649 starvote-2.0.1/docs/clarifying_star_voting.md
+-rw-r--r--   0        0        0     2743 2023-05-31 19:56:48.827782 starvote-2.0.1/docs/formatting_fractions_in_columns_of_text.txt
+-rw-r--r--   0        0        0      217 2023-05-31 21:13:55.136896 starvote-2.0.1/example.py
+-rw-r--r--   0        0        0      583 2023-06-02 19:49:52.947305 starvote-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0    90423 2023-06-02 20:04:35.358964 starvote-2.0.1/starvote/__init__.py
+-rw-r--r--   0        0        0      106 2023-06-02 00:43:16.709978 starvote-2.0.1/starvote/__main__.py
+-rw-r--r--   0        0        0     5781 2023-06-02 20:04:16.742802 starvote-2.0.1/starvote/reference.py
+-rw-r--r--   0        0        0     1051 2023-06-02 01:09:12.579780 starvote-2.0.1/test_elections/README.md
+-rw-r--r--   0        0        0       84 2023-06-01 23:43:37.846114 starvote-2.0.1/test_elections/bad_syntax_ballot_pragma_as_last_line.starvote
+-rw-r--r--   0        0        0     1358 2023-06-02 19:23:34.765586 starvote-2.0.1/test_elections/bad_syntax_ballot_pragma_as_last_line.txt
+-rw-r--r--   0        0        0       68 2023-06-01 23:24:50.800081 starvote-2.0.1/test_elections/bad_syntax_change_section_in_list.starvote
+-rw-r--r--   0        0        0     1395 2023-06-02 19:23:34.765586 starvote-2.0.1/test_elections/bad_syntax_change_section_in_list.txt
+-rw-r--r--   0        0        0       68 2023-06-01 23:23:06.267150 starvote-2.0.1/test_elections/bad_syntax_fussy_wrong_ballots_1.starvote
+-rw-r--r--   0        0        0     1404 2023-06-02 19:23:34.769586 starvote-2.0.1/test_elections/bad_syntax_fussy_wrong_ballots_1.txt
+-rw-r--r--   0        0        0       67 2023-06-01 23:23:00.095096 starvote-2.0.1/test_elections/bad_syntax_fussy_wrong_ballots_2.starvote
+-rw-r--r--   0        0        0     1402 2023-06-02 19:23:34.769586 starvote-2.0.1/test_elections/bad_syntax_fussy_wrong_ballots_2.txt
+-rw-r--r--   0        0        0       35 2023-06-02 19:31:20.821653 starvote-2.0.1/test_elections/bad_syntax_invalid_method.starvote
+-rw-r--r--   0        0        0     1375 2023-06-02 19:31:54.613947 starvote-2.0.1/test_elections/bad_syntax_invalid_method.txt
+-rw-r--r--   0        0        0       40 2023-06-01 23:17:55.140381 starvote-2.0.1/test_elections/bad_syntax_invalid_option.starvote
+-rw-r--r--   0        0        0     1374 2023-06-02 19:23:34.769586 starvote-2.0.1/test_elections/bad_syntax_invalid_option.txt
+-rw-r--r--   0        0        0       44 2023-06-01 23:16:35.203670 starvote-2.0.1/test_elections/bad_syntax_invalid_pragma.starvote
+-rw-r--r--   0        0        0     1376 2023-06-02 19:23:34.769586 starvote-2.0.1/test_elections/bad_syntax_invalid_pragma.txt
+-rw-r--r--   0        0        0       89 2023-06-01 23:37:41.946945 starvote-2.0.1/test_elections/bad_syntax_invalid_start_of_line_mode.starvote
+-rw-r--r--   0        0        0     1335 2023-06-02 19:23:34.769586 starvote-2.0.1/test_elections/bad_syntax_invalid_start_of_line_mode.txt
+-rw-r--r--   0        0        0       50 2023-06-01 23:14:06.126343 starvote-2.0.1/test_elections/bad_syntax_invalid_starvote_path_1.starvote
+-rw-r--r--   0        0        0     1331 2023-06-02 19:23:34.769586 starvote-2.0.1/test_elections/bad_syntax_invalid_starvote_path_1.txt
+-rw-r--r--   0        0        0       70 2023-06-01 23:28:17.369920 starvote-2.0.1/test_elections/bad_syntax_invalid_starvote_path_2.starvote
+-rw-r--r--   0        0        0     1360 2023-06-02 19:23:34.769586 starvote-2.0.1/test_elections/bad_syntax_invalid_starvote_path_2.txt
+-rw-r--r--   0        0        0       38 2023-06-01 23:13:26.765992 starvote-2.0.1/test_elections/bad_syntax_invalid_tiebreaker.starvote
+-rw-r--r--   0        0        0     1382 2023-06-02 19:23:34.769586 starvote-2.0.1/test_elections/bad_syntax_invalid_tiebreaker.txt
+-rw-r--r--   0        0        0       59 2023-06-02 02:02:11.939956 starvote-2.0.1/test_elections/bad_syntax_malformed_section.starvote
+-rw-r--r--   0        0        0     1371 2023-06-02 19:23:34.769586 starvote-2.0.1/test_elections/bad_syntax_malformed_section.txt
+-rw-r--r--   0        0        0       41 2023-06-01 23:44:44.538707 starvote-2.0.1/test_elections/bad_syntax_no_ballots.starvote
+-rw-r--r--   0        0        0     1314 2023-06-02 19:23:34.769586 starvote-2.0.1/test_elections/bad_syntax_no_ballots.txt
+-rw-r--r--   0        0        0       44 2023-06-01 23:34:09.385053 starvote-2.0.1/test_elections/bad_syntax_no_equals.starvote
+-rw-r--r--   0        0        0     1346 2023-06-02 19:23:34.769586 starvote-2.0.1/test_elections/bad_syntax_no_equals.txt
+-rw-r--r--   0        0        0       59 2023-06-02 01:03:50.036922 starvote-2.0.1/test_elections/bad_syntax_no_method.starvote
+-rw-r--r--   0        0        0     1409 2023-06-02 19:23:34.769586 starvote-2.0.1/test_elections/bad_syntax_no_method.txt
+-rw-r--r--   0        0        0       46 2023-06-01 23:32:02.351922 starvote-2.0.1/test_elections/bad_syntax_no_section.starvote
+-rw-r--r--   0        0        0     1364 2023-06-02 19:23:34.769586 starvote-2.0.1/test_elections/bad_syntax_no_section.txt
+-rw-r--r--   0        0        0       47 2023-06-01 23:21:20.118206 starvote-2.0.1/test_elections/bad_syntax_pragma_in_options.starvote
+-rw-r--r--   0        0        0     1375 2023-06-02 19:23:34.769586 starvote-2.0.1/test_elections/bad_syntax_pragma_in_options.txt
+-rw-r--r--   0        0        0      103 2023-06-01 23:32:48.848336 starvote-2.0.1/test_elections/bad_syntax_pragma_inside_list.starvote
+-rw-r--r--   0        0        0     1387 2023-06-02 19:23:34.769586 starvote-2.0.1/test_elections/bad_syntax_pragma_inside_list.txt
+-rw-r--r--   0        0        0       47 2023-06-01 23:18:10.564519 starvote-2.0.1/test_elections/bad_syntax_repeated_option.starvote
+-rw-r--r--   0        0        0     1380 2023-06-02 19:23:34.769586 starvote-2.0.1/test_elections/bad_syntax_repeated_option.txt
+-rw-r--r--   0        0        0       60 2023-06-01 23:31:08.239441 starvote-2.0.1/test_elections/bad_syntax_repeated_section.starvote
+-rw-r--r--   0        0        0     1383 2023-06-02 19:23:34.769586 starvote-2.0.1/test_elections/bad_syntax_repeated_section.txt
+-rw-r--r--   0        0        0    57750 2023-05-20 12:04:29.149807 starvote-2.0.1/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.csv
+-rw-r--r--   0        0        0   575556 2023-05-20 14:35:00.177319 starvote-2.0.1/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.pdf
+-rw-r--r--   0        0        0     1403 2023-06-02 19:23:34.773586 starvote-2.0.1/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.txt
+-rw-r--r--   0        0        0   115221 2023-05-27 14:48:58.735061 starvote-2.0.1/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.csv
+-rw-r--r--   0        0        0   410807 2023-05-27 14:59:16.160516 starvote-2.0.1/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.pdf
+-rw-r--r--   0        0        0     3193 2023-06-02 19:23:34.785586 starvote-2.0.1/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.txt
+-rw-r--r--   0        0        0    49711 2023-05-20 12:04:34.029848 starvote-2.0.1/test_elections/starvote_ballots_best_akali_skins.csv
+-rw-r--r--   0        0        0   538128 2023-05-20 14:33:25.560528 starvote-2.0.1/test_elections/starvote_ballots_best_akali_skins.pdf
+-rw-r--r--   0        0        0     1331 2023-06-02 19:23:34.789586 starvote-2.0.1/test_elections/starvote_ballots_best_akali_skins.txt
+-rw-r--r--   0        0        0     1812 2023-05-20 10:35:18.365110 starvote-2.0.1/test_elections/starvote_ballots_eurovision_song_contest_2023.csv
+-rw-r--r--   0        0        0   807144 2023-05-20 14:33:51.120742 starvote-2.0.1/test_elections/starvote_ballots_eurovision_song_contest_2023.pdf
+-rw-r--r--   0        0        0     2879 2023-06-02 19:23:34.789586 starvote-2.0.1/test_elections/starvote_ballots_eurovision_song_contest_2023.txt
+-rw-r--r--   0        0        0   250538 2023-05-20 10:34:04.044490 starvote-2.0.1/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.csv
+-rw-r--r--   0        0        0   643536 2023-05-20 14:35:41.153662 starvote-2.0.1/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.pdf
+-rw-r--r--   0        0        0     1596 2023-06-02 19:23:34.809586 starvote-2.0.1/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.txt
+-rw-r--r--   0        0        0      175 2023-06-02 19:18:28.166907 starvote-2.0.1/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_bloc_star.starvote
+-rw-r--r--   0        0        0    12586 2023-06-02 19:23:35.117589 starvote-2.0.1/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_bloc_star.txt
+-rw-r--r--   0        0        0      141 2023-06-02 19:18:26.038889 starvote-2.0.1/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_star_pr.starvote
+-rw-r--r--   0        0        0    12586 2023-06-02 19:23:35.429592 starvote-2.0.1/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_star_pr.txt
+-rw-r--r--   0        0        0    31534 2023-05-20 12:04:38.493885 starvote-2.0.1/test_elections/starvote_ballots_presidential_candidates.csv
+-rw-r--r--   0        0        0   325033 2023-05-20 14:34:17.572963 starvote-2.0.1/test_elections/starvote_ballots_presidential_candidates.pdf
+-rw-r--r--   0        0        0      814 2023-06-02 19:23:35.433591 starvote-2.0.1/test_elections/starvote_ballots_presidential_candidates.txt
+-rw-r--r--   0        0        0    48454 2023-05-20 12:04:25.689778 starvote-2.0.1/test_elections/starvote_ballots_presidential_poll_july_2020.csv
+-rw-r--r--   0        0        0   360427 2023-05-20 14:36:25.050030 starvote-2.0.1/test_elections/starvote_ballots_presidential_poll_july_2020.pdf
+-rw-r--r--   0        0        0      799 2023-06-02 19:23:35.433591 starvote-2.0.1/test_elections/starvote_ballots_presidential_poll_july_2020.txt
+-rw-r--r--   0        0        0   123039 2023-05-20 12:04:13.781679 starvote-2.0.1/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.csv
+-rw-r--r--   0        0        0   584998 2023-05-20 14:35:22.465506 starvote-2.0.1/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.pdf
+-rw-r--r--   0        0        0     1434 2023-06-02 19:23:35.441592 starvote-2.0.1/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.txt
+-rw-r--r--   0        0        0    52870 2023-05-20 12:04:22.533752 starvote-2.0.1/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.csv
+-rw-r--r--   0        0        0   354740 2023-05-20 14:36:48.550226 starvote-2.0.1/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.pdf
+-rw-r--r--   0        0        0      747 2023-06-02 19:23:35.445592 starvote-2.0.1/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.txt
+-rw-r--r--   0        0        0      146 2023-06-01 14:23:14.825743 starvote-2.0.1/test_elections/test_election_all_fives_bloc_star.starvote
+-rw-r--r--   0        0        0     1080 2023-06-02 19:23:35.445592 starvote-2.0.1/test_elections/test_election_all_fives_bloc_star.txt
+-rw-r--r--   0        0        0      145 2023-06-01 14:23:10.941709 starvote-2.0.1/test_elections/test_election_all_fives_rrv.starvote
+-rw-r--r--   0        0        0      484 2023-06-02 19:23:35.445592 starvote-2.0.1/test_elections/test_election_all_fives_rrv.txt
+-rw-r--r--   0        0        0      151 2023-06-02 19:18:20.314839 starvote-2.0.1/test_elections/test_election_all_fives_star-pr.starvote
+-rw-r--r--   0        0        0      476 2023-06-02 19:23:35.445592 starvote-2.0.1/test_elections/test_election_all_fives_star-pr.txt
+-rw-r--r--   0        0        0      132 2023-06-01 14:23:02.245634 starvote-2.0.1/test_elections/test_election_all_fives_star.starvote
+-rw-r--r--   0        0        0     1030 2023-06-02 19:23:35.445592 starvote-2.0.1/test_elections/test_election_all_fives_star.txt
+-rw-r--r--   0        0        0      146 2023-06-01 14:23:30.837882 starvote-2.0.1/test_elections/test_election_all_threes_bloc_star.starvote
+-rw-r--r--   0        0        0     1080 2023-06-02 19:23:35.445592 starvote-2.0.1/test_elections/test_election_all_threes_bloc_star.txt
+-rw-r--r--   0        0        0       92 2023-06-01 22:34:03.536957 starvote-2.0.1/test_elections/test_election_all_threes_rrv.starvote
+-rw-r--r--   0        0        0      484 2023-06-02 19:23:35.449592 starvote-2.0.1/test_elections/test_election_all_threes_rrv.txt
+-rw-r--r--   0        0        0       98 2023-06-02 19:18:18.286821 starvote-2.0.1/test_elections/test_election_all_threes_star-pr.starvote
+-rw-r--r--   0        0        0      476 2023-06-02 19:23:35.449592 starvote-2.0.1/test_elections/test_election_all_threes_star-pr.txt
+-rw-r--r--   0        0        0      132 2023-06-01 14:23:19.233781 starvote-2.0.1/test_elections/test_election_all_threes_star.starvote
+-rw-r--r--   0        0        0     1030 2023-06-02 19:23:35.449592 starvote-2.0.1/test_elections/test_election_all_threes_star.txt
+-rw-r--r--   0        0        0      146 2023-06-01 14:19:42.607904 starvote-2.0.1/test_elections/test_election_all_zeroes_bloc_star.starvote
+-rw-r--r--   0        0        0     1077 2023-06-02 19:23:35.449592 starvote-2.0.1/test_elections/test_election_all_zeroes_bloc_star.txt
+-rw-r--r--   0        0        0      145 2023-06-01 14:19:40.835888 starvote-2.0.1/test_elections/test_election_all_zeroes_rrv.starvote
+-rw-r--r--   0        0        0      481 2023-06-02 19:23:35.449592 starvote-2.0.1/test_elections/test_election_all_zeroes_rrv.txt
+-rw-r--r--   0        0        0      151 2023-06-02 19:18:15.894800 starvote-2.0.1/test_elections/test_election_all_zeroes_star-pr.starvote
+-rw-r--r--   0        0        0      473 2023-06-02 19:23:35.449592 starvote-2.0.1/test_elections/test_election_all_zeroes_star-pr.txt
+-rw-r--r--   0        0        0      132 2023-06-01 14:19:46.079934 starvote-2.0.1/test_elections/test_election_all_zeroes_star.starvote
+-rw-r--r--   0        0        0     1027 2023-06-02 19:23:35.449592 starvote-2.0.1/test_elections/test_election_all_zeroes_star.txt
+-rw-r--r--   0        0        0     2660 2023-05-31 22:55:06.890838 starvote-2.0.1/test_elections/test_election_bloc_star_and_electowiki.starvote
+-rw-r--r--   0        0        0     3383 2023-06-02 19:23:35.449592 starvote-2.0.1/test_elections/test_election_bloc_star_and_electowiki.txt
+-rw-r--r--   0        0        0      989 2023-05-31 14:32:27.710655 starvote-2.0.1/test_elections/test_election_bloc_star_unbreakable_tie_for_first.starvote
+-rw-r--r--   0        0        0     1606 2023-06-02 19:23:35.449592 starvote-2.0.1/test_elections/test_election_bloc_star_unbreakable_tie_for_first.txt
+-rw-r--r--   0        0        0      201 2023-05-31 14:32:09.618494 starvote-2.0.1/test_elections/test_election_breakable_tie_for_second_in_score_round.starvote
+-rw-r--r--   0        0        0      831 2023-06-02 19:23:35.449592 starvote-2.0.1/test_elections/test_election_breakable_tie_for_second_in_score_round.txt
+-rw-r--r--   0        0        0      204 2023-05-31 14:31:42.454252 starvote-2.0.1/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.starvote
+-rw-r--r--   0        0        0      965 2023-06-02 19:23:35.449592 starvote-2.0.1/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.txt
+-rw-r--r--   0        0        0      203 2023-05-31 14:31:18.974043 starvote-2.0.1/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_score_round.starvote
+-rw-r--r--   0        0        0      744 2023-06-02 19:23:35.453592 starvote-2.0.1/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_score_round.txt
+-rw-r--r--   0        0        0      838 2023-05-31 14:31:04.393913 starvote-2.0.1/test_elections/test_election_demonstrate_cloneproofness_1.starvote
+-rw-r--r--   0        0        0      542 2023-06-02 19:23:35.453592 starvote-2.0.1/test_elections/test_election_demonstrate_cloneproofness_1.txt
+-rw-r--r--   0        0        0      830 2023-05-31 14:09:22.654324 starvote-2.0.1/test_elections/test_election_demonstrate_cloneproofness_2.starvote
+-rw-r--r--   0        0        0     1087 2023-06-02 19:23:35.453592 starvote-2.0.1/test_elections/test_election_demonstrate_cloneproofness_2.txt
+-rw-r--r--   0        0        0      194 2023-06-01 16:45:03.487305 starvote-2.0.1/test_elections/test_election_extra_candidates_in_permutation.starvote
+-rw-r--r--   0        0        0      142 2023-06-02 19:23:35.453592 starvote-2.0.1/test_elections/test_election_extra_candidates_in_permutation.txt
+-rw-r--r--   0        0        0      165 2023-06-01 16:45:09.147349 starvote-2.0.1/test_elections/test_election_incomplete_permutation.starvote
+-rw-r--r--   0        0        0      138 2023-06-02 19:23:35.453592 starvote-2.0.1/test_elections/test_election_incomplete_permutation.txt
+-rw-r--r--   0        0        0      132 2023-06-02 01:44:01.610291 starvote-2.0.1/test_elections/test_election_no_output.starvote
+-rw-r--r--   0        0        0       17 2023-06-02 19:23:35.453592 starvote-2.0.1/test_elections/test_election_no_output.txt
+-rw-r--r--   0        0        0      130 2023-06-01 16:34:20.926370 starvote-2.0.1/test_elections/test_election_no_permuted_candidates_tiebreaker.starvote
+-rw-r--r--   0        0        0     1329 2023-06-02 19:23:35.453592 starvote-2.0.1/test_elections/test_election_no_permuted_candidates_tiebreaker.txt
+-rw-r--r--   0        0        0      131 2023-06-01 17:57:44.689602 starvote-2.0.1/test_elections/test_election_only_one_candidate_star.starvote
+-rw-r--r--   0        0        0      505 2023-06-02 19:23:35.453592 starvote-2.0.1/test_elections/test_election_only_one_candidate_star.txt
+-rw-r--r--   0        0        0      177 2023-06-01 17:57:23.633416 starvote-2.0.1/test_elections/test_election_only_two_candidates_bloc_star.starvote
+-rw-r--r--   0        0        0      487 2023-06-02 19:23:35.453592 starvote-2.0.1/test_elections/test_election_only_two_candidates_bloc_star.txt
+-rw-r--r--   0        0        0      176 2023-06-01 17:57:20.909392 starvote-2.0.1/test_elections/test_election_only_two_candidates_rrv.starvote
+-rw-r--r--   0        0        0      523 2023-06-02 19:23:35.453592 starvote-2.0.1/test_elections/test_election_only_two_candidates_rrv.txt
+-rw-r--r--   0        0        0      182 2023-06-02 19:18:13.310778 starvote-2.0.1/test_elections/test_election_only_two_candidates_star-pr.starvote
+-rw-r--r--   0        0        0      545 2023-06-02 19:23:35.453592 starvote-2.0.1/test_elections/test_election_only_two_candidates_star-pr.txt
+-rw-r--r--   0        0        0      319 2023-06-02 19:18:05.042705 starvote-2.0.1/test_elections/test_election_proportional_star_unbreakable_tie.starvote
+-rw-r--r--   0        0        0      480 2023-06-02 19:23:35.453592 starvote-2.0.1/test_elections/test_election_proportional_star_unbreakable_tie.txt
+-rw-r--r--   0        0        0     5899 2023-05-22 07:24:36.945502 starvote-2.0.1/test_elections/test_election_reweighted_range_sample_election.html
+-rw-r--r--   0        0        0      450 2023-05-31 14:05:31.788268 starvote-2.0.1/test_elections/test_election_reweighted_range_sample_election.starvote
+-rw-r--r--   0        0        0     1150 2023-06-02 19:23:35.457592 starvote-2.0.1/test_elections/test_election_reweighted_range_sample_election.txt
+-rw-r--r--   0        0        0      203 2023-05-31 14:05:02.452007 starvote-2.0.1/test_elections/test_election_unbreakable_three_way_tie_for_first_in_score_round.starvote
+-rw-r--r--   0        0        0     1023 2023-06-02 19:23:35.457592 starvote-2.0.1/test_elections/test_election_unbreakable_three_way_tie_for_first_in_score_round.txt
+-rw-r--r--   0        0        0      306 2023-06-01 18:06:23.106174 starvote-2.0.1/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round.starvote
+-rw-r--r--   0        0        0     1788 2023-06-02 19:23:35.457592 starvote-2.0.1/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round.txt
+-rw-r--r--   0        0        0      143 2023-06-02 19:18:03.054688 starvote-2.0.1/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_star-pr.starvote
+-rw-r--r--   0        0        0     2029 2023-06-02 19:23:35.457592 starvote-2.0.1/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_star-pr.txt
+-rw-r--r--   0        0        0      203 2023-05-31 14:04:09.035532 starvote-2.0.1/test_elections/test_election_unbreakable_tie_for_second_in_score_round.starvote
+-rw-r--r--   0        0        0      938 2023-06-02 19:23:35.457592 starvote-2.0.1/test_elections/test_election_unbreakable_tie_for_second_in_score_round.txt
+-rw-r--r--   0        0        0      155 2023-05-28 20:58:05.118365 starvote-2.0.1/test_elections/test_election_unbreakable_tie_in_automatic_runoff_round.starvote
+-rw-r--r--   0        0        0     1081 2023-06-02 19:23:35.457592 starvote-2.0.1/test_elections/test_election_unbreakable_tie_in_automatic_runoff_round.txt
+-rw-r--r--   0        0        0      150 2023-06-01 14:49:33.615373 starvote-2.0.1/test_elections/test_election_use_just_raise_tiebreaker.starvote
+-rw-r--r--   0        0        0     1197 2023-06-02 19:23:35.457592 starvote-2.0.1/test_elections/test_election_use_just_raise_tiebreaker.txt
+-rw-r--r--   0        0        0      154 2023-06-01 16:06:23.349484 starvote-2.0.1/test_elections/test_election_use_no_description_tiebreaker.starvote
+-rw-r--r--   0        0        0     1030 2023-06-02 19:23:35.457592 starvote-2.0.1/test_elections/test_election_use_no_description_tiebreaker.txt
+-rw-r--r--   0        0        0      152 2023-06-01 16:08:48.230596 starvote-2.0.1/test_elections/test_election_use_only_heading_tiebreaker.starvote
+-rw-r--r--   0        0        0      152 2023-06-02 19:23:35.457592 starvote-2.0.1/test_elections/test_election_use_only_heading_tiebreaker.txt
+-rw-r--r--   0        0        0    35726 2023-06-02 19:26:39.999204 starvote-2.0.1/tests/run_tests.py
+-rwxr-xr-x   0        0        0     2211 2023-06-02 19:34:15.379168 starvote-2.0.1/tools/is_ok
+-rwxr-xr-x   0        0        0     1827 2023-06-02 18:03:13.135277 starvote-2.0.1/tools/remake_test_elections_output
+-rw-r--r--   0        0        0    32872 1970-01-01 00:00:00.000000 starvote-2.0.1/PKG-INFO
```

### Comparing `starvote-2.0/LICENSE` & `starvote-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `starvote-2.0/README.md` & `starvote-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: starvote
+Version: 2.0.1
+Summary: An election tabulator for the STAR electoral system, and others
+Author-email: Larry Hastings <larry@hastings.org>
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Dist: numpy ; extra == "reference"
+Requires-Dist: pandas ; extra == "reference"
+Project-URL: Source, https://github.com/larryhastings/starvote/
+Provides-Extra: reference
+
 # starvote
 
 ## A simple STAR Voting tabulator
 
 ## Copyright 2023 by Larry Hastings
 
 [STAR voting](https://www.starvoting.org/) is a
@@ -650,15 +665,15 @@
 *starvote format* files should end with the file extension `.starvote`
 and contain a *starvote format election* in UTF-8 format.
 
 For example, you can run this from the root of the
 source-code repository:
 
 ```
-% python3 -m starvote test_elections/test_election_automatic_runoff_breakable_tie_using_5_score_count_round.starvote
+% python3 -m starvote test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.starvote
 ```
 
 to see how **starvote** handles ties during the automatic runoff round.
 
 
 ## Multiple-winner elections
 
@@ -726,14 +741,19 @@
 [`https://star.vote/`](https://star.vote/).  The licensing of these
 sample ballots is unclear, but they're assumed to be public-domain
 or otherwise freely redistributable.
 
 
 ## Changelog
 
+**2.0.1** - *2023/05/27*
+
+* Changed the nickname of the reference version of
+  Allocated Score Voting to "Allocated-R".
+
 **2.0** - *2023/05/27*
 
 A complete rewrite!  The 1.x code base was pretty smelly.
 This codebase is much, much cleaner--and I think I squashed
 one or two bugs too.
 
 `starvote` has an entirely new, functional API. `election`
@@ -879,7 +899,8 @@
 * Added sample output for every sample poll in `sample_polls/`.
   These outputs have been confirmed correct by inspection, and
   could in the future be used as part of an automated test suite.
 
 **1.0** - *2023/05/20*
 
 * Initial release.
+
```

### Comparing `starvote-2.0/docs/clarifying_star_voting.md` & `starvote-2.0.1/docs/clarifying_star_voting.md`

 * *Files identical despite different names*

### Comparing `starvote-2.0/docs/formatting_fractions_in_columns_of_text.txt` & `starvote-2.0.1/docs/formatting_fractions_in_columns_of_text.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/pyproject.toml` & `starvote-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `starvote-2.0/starvote/__init__.py` & `starvote-2.0.1/starvote/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 __doc__ = "An election tabulator for the STAR electoral system, and others"
 
-__version__ = "2.0"
+__version__ = "2.0.1"
 
 __all__ = [
     'Allocated_Score_Voting', # Method
     'Allocated', # Method (nickname)
     'allocated_score_voting', # function
     'Bloc_STAR_Voting', # Method
     'Bloc', # Method (nickname)
```

### Comparing `starvote-2.0/starvote/reference.py` & `starvote-2.0.1/starvote/reference.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,14 +155,14 @@
     """
     Adds the reference implementation of Proportional STAR from the STAR voting website
     to the available electoral systems provided by starvote, under the name
     'Reference Proportional STAR'.
     """
     for name in (
         'Allocated Score Voting (reference)',
-        'Reference Allocated Score',
-        'reference allocated score',
+        'Allocated-R',
+        'allocated-r',
         ):
         starvote.methods[name] = Allocated_Score_Voting_reference
     starvote.Allocated_Score_Voting_reference = Allocated_Score_Voting_reference
     starvote.allocated_score_voting_reference = allocated_score_voting_reference
     starvote.__all__.append('Allocated_Score_Voting_reference')
```

### Comparing `starvote-2.0/test_elections/README.md` & `starvote-2.0.1/test_elections/README.md`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/bad_syntax_ballot_pragma_as_last_line.txt` & `starvote-2.0.1/test_elections/bad_syntax_ballot_pragma_as_last_line.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/bad_syntax_change_section_in_list.txt` & `starvote-2.0.1/test_elections/bad_syntax_change_section_in_list.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/bad_syntax_fussy_wrong_ballots_1.txt` & `starvote-2.0.1/test_elections/bad_syntax_fussy_wrong_ballots_1.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/bad_syntax_fussy_wrong_ballots_2.txt` & `starvote-2.0.1/test_elections/bad_syntax_fussy_wrong_ballots_2.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/bad_syntax_invalid_method.txt` & `starvote-2.0.1/test_elections/bad_syntax_invalid_method.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/bad_syntax_invalid_option.txt` & `starvote-2.0.1/test_elections/bad_syntax_invalid_option.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/bad_syntax_invalid_pragma.txt` & `starvote-2.0.1/test_elections/bad_syntax_invalid_pragma.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/bad_syntax_invalid_start_of_line_mode.txt` & `starvote-2.0.1/test_elections/bad_syntax_invalid_start_of_line_mode.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/bad_syntax_invalid_starvote_path_1.txt` & `starvote-2.0.1/test_elections/bad_syntax_invalid_starvote_path_1.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/bad_syntax_invalid_starvote_path_2.txt` & `starvote-2.0.1/test_elections/bad_syntax_invalid_starvote_path_2.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/bad_syntax_invalid_tiebreaker.txt` & `starvote-2.0.1/test_elections/bad_syntax_invalid_tiebreaker.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/bad_syntax_malformed_section.txt` & `starvote-2.0.1/test_elections/bad_syntax_malformed_section.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/bad_syntax_no_ballots.txt` & `starvote-2.0.1/test_elections/bad_syntax_no_ballots.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/bad_syntax_no_equals.txt` & `starvote-2.0.1/test_elections/bad_syntax_no_equals.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/bad_syntax_no_method.txt` & `starvote-2.0.1/test_elections/bad_syntax_no_method.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/bad_syntax_no_section.txt` & `starvote-2.0.1/test_elections/bad_syntax_no_section.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/bad_syntax_pragma_in_options.txt` & `starvote-2.0.1/test_elections/bad_syntax_pragma_in_options.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/bad_syntax_pragma_inside_list.txt` & `starvote-2.0.1/test_elections/bad_syntax_pragma_inside_list.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/bad_syntax_repeated_option.txt` & `starvote-2.0.1/test_elections/bad_syntax_repeated_option.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/bad_syntax_repeated_section.txt` & `starvote-2.0.1/test_elections/bad_syntax_repeated_section.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.csv` & `starvote-2.0.1/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.pdf` & `starvote-2.0.1/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.txt` & `starvote-2.0.1/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.csv` & `starvote-2.0.1/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.pdf` & `starvote-2.0.1/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.txt` & `starvote-2.0.1/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/starvote_ballots_best_akali_skins.csv` & `starvote-2.0.1/test_elections/starvote_ballots_best_akali_skins.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/starvote_ballots_best_akali_skins.pdf` & `starvote-2.0.1/test_elections/starvote_ballots_best_akali_skins.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/starvote_ballots_best_akali_skins.txt` & `starvote-2.0.1/test_elections/starvote_ballots_best_akali_skins.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/starvote_ballots_eurovision_song_contest_2023.csv` & `starvote-2.0.1/test_elections/starvote_ballots_eurovision_song_contest_2023.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/starvote_ballots_eurovision_song_contest_2023.pdf` & `starvote-2.0.1/test_elections/starvote_ballots_eurovision_song_contest_2023.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/starvote_ballots_eurovision_song_contest_2023.txt` & `starvote-2.0.1/test_elections/starvote_ballots_eurovision_song_contest_2023.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.csv` & `starvote-2.0.1/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.pdf` & `starvote-2.0.1/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.txt` & `starvote-2.0.1/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_bloc_star.txt` & `starvote-2.0.1/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_bloc_star.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_star_pr.txt` & `starvote-2.0.1/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_star_pr.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/starvote_ballots_presidential_candidates.csv` & `starvote-2.0.1/test_elections/starvote_ballots_presidential_candidates.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/starvote_ballots_presidential_candidates.pdf` & `starvote-2.0.1/test_elections/starvote_ballots_presidential_candidates.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/starvote_ballots_presidential_candidates.txt` & `starvote-2.0.1/test_elections/starvote_ballots_presidential_candidates.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/starvote_ballots_presidential_poll_july_2020.csv` & `starvote-2.0.1/test_elections/starvote_ballots_presidential_poll_july_2020.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/starvote_ballots_presidential_poll_july_2020.pdf` & `starvote-2.0.1/test_elections/starvote_ballots_presidential_poll_july_2020.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/starvote_ballots_presidential_poll_july_2020.txt` & `starvote-2.0.1/test_elections/starvote_ballots_presidential_poll_july_2020.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.csv` & `starvote-2.0.1/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.pdf` & `starvote-2.0.1/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.txt` & `starvote-2.0.1/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.csv` & `starvote-2.0.1/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.pdf` & `starvote-2.0.1/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.txt` & `starvote-2.0.1/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/test_election_all_fives_bloc_star.txt` & `starvote-2.0.1/test_elections/test_election_all_fives_bloc_star.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/test_election_all_fives_star.txt` & `starvote-2.0.1/test_elections/test_election_all_fives_star.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/test_election_all_threes_bloc_star.txt` & `starvote-2.0.1/test_elections/test_election_all_threes_bloc_star.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/test_election_all_threes_star.txt` & `starvote-2.0.1/test_elections/test_election_all_threes_star.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/test_election_all_zeroes_bloc_star.txt` & `starvote-2.0.1/test_elections/test_election_all_zeroes_bloc_star.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/test_election_all_zeroes_star.txt` & `starvote-2.0.1/test_elections/test_election_all_zeroes_star.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/test_election_bloc_star_and_electowiki.starvote` & `starvote-2.0.1/test_elections/test_election_bloc_star_and_electowiki.starvote`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/test_election_bloc_star_and_electowiki.txt` & `starvote-2.0.1/test_elections/test_election_bloc_star_and_electowiki.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/test_election_bloc_star_unbreakable_tie_for_first.starvote` & `starvote-2.0.1/test_elections/test_election_bloc_star_unbreakable_tie_for_first.starvote`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/test_election_bloc_star_unbreakable_tie_for_first.txt` & `starvote-2.0.1/test_elections/test_election_bloc_star_unbreakable_tie_for_first.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/test_election_breakable_tie_for_second_in_score_round.txt` & `starvote-2.0.1/test_elections/test_election_breakable_tie_for_second_in_score_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.txt` & `starvote-2.0.1/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_score_round.txt` & `starvote-2.0.1/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_score_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/test_election_demonstrate_cloneproofness_1.starvote` & `starvote-2.0.1/test_elections/test_election_demonstrate_cloneproofness_1.starvote`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/test_election_demonstrate_cloneproofness_1.txt` & `starvote-2.0.1/test_elections/test_election_demonstrate_cloneproofness_1.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/test_election_demonstrate_cloneproofness_2.starvote` & `starvote-2.0.1/test_elections/test_election_demonstrate_cloneproofness_2.starvote`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/test_election_demonstrate_cloneproofness_2.txt` & `starvote-2.0.1/test_elections/test_election_demonstrate_cloneproofness_2.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/test_election_no_permuted_candidates_tiebreaker.txt` & `starvote-2.0.1/test_elections/test_election_no_permuted_candidates_tiebreaker.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/test_election_only_two_candidates_rrv.txt` & `starvote-2.0.1/test_elections/test_election_only_two_candidates_rrv.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/test_election_only_two_candidates_star-pr.txt` & `starvote-2.0.1/test_elections/test_election_only_two_candidates_star-pr.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/test_election_reweighted_range_sample_election.html` & `starvote-2.0.1/test_elections/test_election_reweighted_range_sample_election.html`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/test_election_reweighted_range_sample_election.txt` & `starvote-2.0.1/test_elections/test_election_reweighted_range_sample_election.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/test_election_unbreakable_three_way_tie_for_first_in_score_round.txt` & `starvote-2.0.1/test_elections/test_election_unbreakable_three_way_tie_for_first_in_score_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round.txt` & `starvote-2.0.1/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_star-pr.txt` & `starvote-2.0.1/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_star-pr.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/test_election_unbreakable_tie_for_second_in_score_round.txt` & `starvote-2.0.1/test_elections/test_election_unbreakable_tie_for_second_in_score_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/test_election_unbreakable_tie_in_automatic_runoff_round.txt` & `starvote-2.0.1/test_elections/test_election_unbreakable_tie_in_automatic_runoff_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/test_election_use_just_raise_tiebreaker.txt` & `starvote-2.0.1/test_elections/test_election_use_just_raise_tiebreaker.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/test_elections/test_election_use_no_description_tiebreaker.txt` & `starvote-2.0.1/test_elections/test_election_use_no_description_tiebreaker.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0/tests/run_tests.py` & `starvote-2.0.1/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `starvote-2.0/tools/is_ok` & `starvote-2.0.1/tools/is_ok`

 * *Files identical despite different names*

### Comparing `starvote-2.0/tools/remake_test_elections_output` & `starvote-2.0.1/tools/remake_test_elections_output`

 * *Files identical despite different names*

### Comparing `starvote-2.0/PKG-INFO` & `starvote-2.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: starvote
-Version: 2.0
-Summary: An election tabulator for the STAR electoral system, and others
-Author-email: Larry Hastings <larry@hastings.org>
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Dist: numpy ; extra == "reference"
-Requires-Dist: pandas ; extra == "reference"
-Project-URL: Source, https://github.com/larryhastings/starvote/
-Provides-Extra: reference
-
 # starvote
 
 ## A simple STAR Voting tabulator
 
 ## Copyright 2023 by Larry Hastings
 
 [STAR voting](https://www.starvoting.org/) is a
@@ -665,15 +650,15 @@
 *starvote format* files should end with the file extension `.starvote`
 and contain a *starvote format election* in UTF-8 format.
 
 For example, you can run this from the root of the
 source-code repository:
 
 ```
-% python3 -m starvote test_elections/test_election_automatic_runoff_breakable_tie_using_5_score_count_round.starvote
+% python3 -m starvote test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.starvote
 ```
 
 to see how **starvote** handles ties during the automatic runoff round.
 
 
 ## Multiple-winner elections
 
@@ -741,14 +726,19 @@
 [`https://star.vote/`](https://star.vote/).  The licensing of these
 sample ballots is unclear, but they're assumed to be public-domain
 or otherwise freely redistributable.
 
 
 ## Changelog
 
+**2.0.1** - *2023/05/27*
+
+* Changed the nickname of the reference version of
+  Allocated Score Voting to "Allocated-R".
+
 **2.0** - *2023/05/27*
 
 A complete rewrite!  The 1.x code base was pretty smelly.
 This codebase is much, much cleaner--and I think I squashed
 one or two bugs too.
 
 `starvote` has an entirely new, functional API. `election`
@@ -894,8 +884,7 @@
 * Added sample output for every sample poll in `sample_polls/`.
   These outputs have been confirmed correct by inspection, and
   could in the future be used as part of an automated test suite.
 
 **1.0** - *2023/05/20*
 
 * Initial release.
-
```

