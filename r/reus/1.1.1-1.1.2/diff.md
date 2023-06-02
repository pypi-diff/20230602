# Comparing `tmp/reus-1.1.1.tar.gz` & `tmp/reus-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reus-1.1.1.tar", last modified: Sat May 13 14:51:18 2023, max compression
+gzip compressed data, was "reus-1.1.2.tar", last modified: Fri Jun  2 19:53:16 2023, max compression
```

## Comparing `reus-1.1.1.tar` & `reus-1.1.2.tar`

### file list

```diff
@@ -1,74 +1,83 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 14:51:18.872095 reus-1.1.1/
--rw-rw-rw-   0        0        0     1090 2022-05-11 22:07:30.000000 reus-1.1.1/LICENSE
--rw-rw-rw-   0        0        0      616 2023-05-13 14:51:18.872095 reus-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1978 2023-05-13 14:44:11.000000 reus-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-13 14:51:18.804095 reus-1.1.1/reus/
--rw-rw-rw-   0        0        0      100 2022-10-09 22:38:33.000000 reus-1.1.1/reus/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-13 14:51:18.855096 reus-1.1.1/reus/fbref/
--rw-rw-rw-   0        0        0     1866 2022-10-09 22:38:44.000000 reus-1.1.1/reus/fbref/__init__.py
--rw-rw-rw-   0        0        0     3075 2023-05-10 20:47:21.000000 reus-1.1.1/reus/fbref/fb_league_table.py
--rw-rw-rw-   0        0        0     4728 2023-05-12 15:42:41.000000 reus-1.1.1/reus/fbref/fb_match_data.py
--rw-rw-rw-   0        0        0     5262 2023-05-11 14:36:50.000000 reus-1.1.1/reus/fbref/fb_match_defensive_actions_stats.py
--rw-rw-rw-   0        0        0     6747 2023-05-11 14:36:55.000000 reus-1.1.1/reus/fbref/fb_match_keeper_stats.py
--rw-rw-rw-   0        0        0     2215 2023-05-11 14:38:13.000000 reus-1.1.1/reus/fbref/fb_match_lineups.py
--rw-rw-rw-   0        0        0     8210 2023-05-10 17:45:31.000000 reus-1.1.1/reus/fbref/fb_match_metadata.py
--rw-rw-rw-   0        0        0     4753 2023-05-11 14:41:39.000000 reus-1.1.1/reus/fbref/fb_match_misc_stats.py
--rw-rw-rw-   0        0        0     6569 2023-05-11 14:43:26.000000 reus-1.1.1/reus/fbref/fb_match_passing_stats.py
--rw-rw-rw-   0        0        0     4564 2023-05-11 14:43:49.000000 reus-1.1.1/reus/fbref/fb_match_passing_type_stats.py
--rw-rw-rw-   0        0        0     6370 2023-05-11 14:44:03.000000 reus-1.1.1/reus/fbref/fb_match_possession_stats.py
--rw-rw-rw-   0        0        0     3793 2023-05-10 17:59:04.000000 reus-1.1.1/reus/fbref/fb_match_shots.py
--rw-rw-rw-   0        0        0     3262 2023-05-06 14:21:55.000000 reus-1.1.1/reus/fbref/fb_match_summary.py
--rw-rw-rw-   0        0        0     6007 2023-05-11 14:46:36.000000 reus-1.1.1/reus/fbref/fb_match_summary_stats.py
--rw-rw-rw-   0        0        0     9203 2023-05-10 18:01:05.000000 reus-1.1.1/reus/fbref/fb_match_team_stats.py
--rw-rw-rw-   0        0        0      869 2022-09-09 21:55:47.000000 reus-1.1.1/reus/fbref/fb_match_urls.py
--rw-rw-rw-   0        0        0     3176 2023-05-10 18:19:13.000000 reus-1.1.1/reus/fbref/fb_season_fixture_urls.py
--rw-rw-rw-   0        0        0     3161 2023-05-10 18:16:40.000000 reus-1.1.1/reus/fbref/fb_season_urls.py
--rw-rw-rw-   0        0        0     6142 2023-05-11 14:56:35.000000 reus-1.1.1/reus/fbref/fb_team_advanced_keeper_stats.py
--rw-rw-rw-   0        0        0     4206 2023-05-11 15:22:22.000000 reus-1.1.1/reus/fbref/fb_team_data.py
--rw-rw-rw-   0        0        0     4591 2023-05-11 14:56:06.000000 reus-1.1.1/reus/fbref/fb_team_defensive_actions_stats.py
--rw-rw-rw-   0        0        0     4227 2023-05-11 15:11:09.000000 reus-1.1.1/reus/fbref/fb_team_goal_sca_stats.py
--rw-rw-rw-   0        0        0     4272 2023-05-11 15:11:12.000000 reus-1.1.1/reus/fbref/fb_team_keeper_stats.py
--rw-rw-rw-   0        0        0     4048 2023-05-11 15:11:14.000000 reus-1.1.1/reus/fbref/fb_team_misc_stats.py
--rw-rw-rw-   0        0        0     6112 2023-05-11 15:11:17.000000 reus-1.1.1/reus/fbref/fb_team_passing_stats.py
--rw-rw-rw-   0        0        0     3870 2023-05-11 15:11:20.000000 reus-1.1.1/reus/fbref/fb_team_passing_type_stats.py
--rw-rw-rw-   0        0        0     5794 2023-05-10 20:37:39.000000 reus-1.1.1/reus/fbref/fb_team_player_advanced_keeper_stats.py
--rw-rw-rw-   0        0        0     3149 2023-05-11 15:22:18.000000 reus-1.1.1/reus/fbref/fb_team_player_data.py
--rw-rw-rw-   0        0        0     4366 2023-05-10 19:09:34.000000 reus-1.1.1/reus/fbref/fb_team_player_defensive_actions_stats.py
--rw-rw-rw-   0        0        0     4156 2023-05-10 19:15:49.000000 reus-1.1.1/reus/fbref/fb_team_player_goal_sca_stats.py
--rw-rw-rw-   0        0        0     4123 2023-05-10 19:26:43.000000 reus-1.1.1/reus/fbref/fb_team_player_keeper_stats.py
--rw-rw-rw-   0        0        0     3930 2023-05-10 19:41:13.000000 reus-1.1.1/reus/fbref/fb_team_player_misc_stats.py
--rw-rw-rw-   0        0        0     5823 2023-05-10 19:53:16.000000 reus-1.1.1/reus/fbref/fb_team_player_passing_stats.py
--rw-rw-rw-   0        0        0     3807 2023-05-10 19:57:40.000000 reus-1.1.1/reus/fbref/fb_team_player_passing_type_stats.py
--rw-rw-rw-   0        0        0     4870 2023-05-10 20:06:02.000000 reus-1.1.1/reus/fbref/fb_team_player_playing_time_stats.py
--rw-rw-rw-   0        0        0     5548 2023-05-10 20:08:44.000000 reus-1.1.1/reus/fbref/fb_team_player_possession_stats.py
--rw-rw-rw-   0        0        0     4208 2023-05-10 20:14:01.000000 reus-1.1.1/reus/fbref/fb_team_player_shooting_stats.py
--rw-rw-rw-   0        0        0     5299 2023-05-10 20:28:25.000000 reus-1.1.1/reus/fbref/fb_team_player_summary_stats.py
--rw-rw-rw-   0        0        0     4221 2023-05-10 22:30:19.000000 reus-1.1.1/reus/fbref/fb_team_playing_time_stats.py
--rw-rw-rw-   0        0        0     5696 2023-05-11 15:11:25.000000 reus-1.1.1/reus/fbref/fb_team_possession_stats.py
--rw-rw-rw-   0        0        0     4397 2023-05-11 15:11:27.000000 reus-1.1.1/reus/fbref/fb_team_shooting_stats.py
--rw-rw-rw-   0        0        0     5217 2023-05-11 15:11:28.000000 reus-1.1.1/reus/fbref/fb_team_summary_stats.py
-drwxrwxrwx   0        0        0        0 2023-05-13 14:51:18.861096 reus-1.1.1/reus/fotmob/
--rw-rw-rw-   0        0        0      143 2022-10-09 22:38:39.000000 reus-1.1.1/reus/fotmob/__init__.py
--rw-rw-rw-   0        0        0     1466 2023-05-11 15:29:50.000000 reus-1.1.1/reus/fotmob/fm_leagues.py
--rw-rw-rw-   0        0        0    14744 2023-05-12 15:42:45.000000 reus-1.1.1/reus/fotmob/fm_match_data.py
--rw-rw-rw-   0        0        0     1340 2022-10-16 18:56:44.000000 reus-1.1.1/reus/fotmob/fm_match_ids.py
--rw-rw-rw-   0        0        0     3768 2023-04-22 23:43:18.000000 reus-1.1.1/reus/fotmob/util.py
-drwxrwxrwx   0        0        0        0 2023-05-13 14:51:18.871095 reus-1.1.1/reus/transfermarkt/
--rw-rw-rw-   0        0        0      387 2023-05-11 17:36:53.000000 reus-1.1.1/reus/transfermarkt/__init__.py
--rw-rw-rw-   0        0        0     1522 2023-05-12 15:42:49.000000 reus-1.1.1/reus/transfermarkt/tm_player_data.py
--rw-rw-rw-   0        0        0     1660 2023-05-12 16:18:21.000000 reus-1.1.1/reus/transfermarkt/tm_player_injury.py
--rw-rw-rw-   0        0        0     1843 2023-05-12 16:09:28.000000 reus-1.1.1/reus/transfermarkt/tm_player_market_value.py
--rw-rw-rw-   0        0        0     8087 2023-05-12 16:18:15.000000 reus-1.1.1/reus/transfermarkt/tm_player_metadata.py
--rw-rw-rw-   0        0        0     3460 2023-05-12 16:18:09.000000 reus-1.1.1/reus/transfermarkt/tm_player_transfers.py
--rw-rw-rw-   0        0        0     5796 2023-05-12 16:06:28.000000 reus-1.1.1/reus/transfermarkt/tm_team_player_data.py
--rw-rw-rw-   0        0        0     9782 2023-05-12 16:04:59.000000 reus-1.1.1/reus/transfermarkt/tm_team_transfers.py
--rw-rw-rw-   0        0        0     2092 2023-05-12 16:07:09.000000 reus-1.1.1/reus/transfermarkt/util.py
--rw-rw-rw-   0        0        0     1052 2023-04-30 18:07:32.000000 reus-1.1.1/reus/util.py
-drwxrwxrwx   0        0        0        0 2023-05-13 14:51:18.812095 reus-1.1.1/reus.egg-info/
--rw-rw-rw-   0        0        0      616 2023-05-13 14:51:18.000000 reus-1.1.1/reus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2259 2023-05-13 14:51:18.000000 reus-1.1.1/reus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 14:51:18.000000 reus-1.1.1/reus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-13 14:51:18.000000 reus-1.1.1/reus.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-13 14:51:18.000000 reus-1.1.1/reus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-13 14:51:18.873096 reus-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      883 2022-10-09 22:40:20.000000 reus-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:53:16.213519 reus-1.1.2/
+-rw-rw-rw-   0        0        0     1090 2023-06-02 19:45:44.000000 reus-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0      616 2023-06-02 19:53:16.212519 reus-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2502 2023-06-02 19:44:43.000000 reus-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 19:53:16.144521 reus-1.1.2/reus/
+-rw-rw-rw-   0        0        0      178 2023-06-02 18:52:15.000000 reus-1.1.2/reus/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:53:16.190519 reus-1.1.2/reus/fbref/
+-rw-rw-rw-   0        0        0     1866 2023-06-02 18:51:51.000000 reus-1.1.2/reus/fbref/__init__.py
+-rw-rw-rw-   0        0        0     3075 2023-05-10 20:47:21.000000 reus-1.1.2/reus/fbref/fb_league_table.py
+-rw-rw-rw-   0        0        0     4728 2023-05-12 15:42:41.000000 reus-1.1.2/reus/fbref/fb_match_data.py
+-rw-rw-rw-   0        0        0     5262 2023-05-11 14:36:50.000000 reus-1.1.2/reus/fbref/fb_match_defensive_actions_stats.py
+-rw-rw-rw-   0        0        0     6747 2023-05-11 14:36:55.000000 reus-1.1.2/reus/fbref/fb_match_keeper_stats.py
+-rw-rw-rw-   0        0        0     2215 2023-05-11 14:38:13.000000 reus-1.1.2/reus/fbref/fb_match_lineups.py
+-rw-rw-rw-   0        0        0     8210 2023-05-10 17:45:31.000000 reus-1.1.2/reus/fbref/fb_match_metadata.py
+-rw-rw-rw-   0        0        0     4753 2023-05-11 14:41:39.000000 reus-1.1.2/reus/fbref/fb_match_misc_stats.py
+-rw-rw-rw-   0        0        0     6569 2023-05-11 14:43:26.000000 reus-1.1.2/reus/fbref/fb_match_passing_stats.py
+-rw-rw-rw-   0        0        0     4564 2023-05-11 14:43:49.000000 reus-1.1.2/reus/fbref/fb_match_passing_type_stats.py
+-rw-rw-rw-   0        0        0     6370 2023-05-11 14:44:03.000000 reus-1.1.2/reus/fbref/fb_match_possession_stats.py
+-rw-rw-rw-   0        0        0     3793 2023-05-10 17:59:04.000000 reus-1.1.2/reus/fbref/fb_match_shots.py
+-rw-rw-rw-   0        0        0     3262 2023-05-06 14:21:55.000000 reus-1.1.2/reus/fbref/fb_match_summary.py
+-rw-rw-rw-   0        0        0     6007 2023-05-11 14:46:36.000000 reus-1.1.2/reus/fbref/fb_match_summary_stats.py
+-rw-rw-rw-   0        0        0     9203 2023-05-10 18:01:05.000000 reus-1.1.2/reus/fbref/fb_match_team_stats.py
+-rw-rw-rw-   0        0        0      869 2022-09-09 21:55:47.000000 reus-1.1.2/reus/fbref/fb_match_urls.py
+-rw-rw-rw-   0        0        0     3945 2023-06-02 18:46:50.000000 reus-1.1.2/reus/fbref/fb_season_fixture_urls.py
+-rw-rw-rw-   0        0        0     3930 2023-06-02 18:46:25.000000 reus-1.1.2/reus/fbref/fb_season_urls.py
+-rw-rw-rw-   0        0        0     6142 2023-05-11 14:56:35.000000 reus-1.1.2/reus/fbref/fb_team_advanced_keeper_stats.py
+-rw-rw-rw-   0        0        0     4206 2023-05-11 15:22:22.000000 reus-1.1.2/reus/fbref/fb_team_data.py
+-rw-rw-rw-   0        0        0     4591 2023-05-11 14:56:06.000000 reus-1.1.2/reus/fbref/fb_team_defensive_actions_stats.py
+-rw-rw-rw-   0        0        0     4227 2023-05-11 15:11:09.000000 reus-1.1.2/reus/fbref/fb_team_goal_sca_stats.py
+-rw-rw-rw-   0        0        0     4272 2023-05-11 15:11:12.000000 reus-1.1.2/reus/fbref/fb_team_keeper_stats.py
+-rw-rw-rw-   0        0        0     4048 2023-05-11 15:11:14.000000 reus-1.1.2/reus/fbref/fb_team_misc_stats.py
+-rw-rw-rw-   0        0        0     6112 2023-05-11 15:11:17.000000 reus-1.1.2/reus/fbref/fb_team_passing_stats.py
+-rw-rw-rw-   0        0        0     3870 2023-05-11 15:11:20.000000 reus-1.1.2/reus/fbref/fb_team_passing_type_stats.py
+-rw-rw-rw-   0        0        0     5794 2023-05-10 20:37:39.000000 reus-1.1.2/reus/fbref/fb_team_player_advanced_keeper_stats.py
+-rw-rw-rw-   0        0        0     3149 2023-05-11 15:22:18.000000 reus-1.1.2/reus/fbref/fb_team_player_data.py
+-rw-rw-rw-   0        0        0     4366 2023-05-10 19:09:34.000000 reus-1.1.2/reus/fbref/fb_team_player_defensive_actions_stats.py
+-rw-rw-rw-   0        0        0     4156 2023-05-10 19:15:49.000000 reus-1.1.2/reus/fbref/fb_team_player_goal_sca_stats.py
+-rw-rw-rw-   0        0        0     4123 2023-05-10 19:26:43.000000 reus-1.1.2/reus/fbref/fb_team_player_keeper_stats.py
+-rw-rw-rw-   0        0        0     3930 2023-05-10 19:41:13.000000 reus-1.1.2/reus/fbref/fb_team_player_misc_stats.py
+-rw-rw-rw-   0        0        0     5823 2023-05-10 19:53:16.000000 reus-1.1.2/reus/fbref/fb_team_player_passing_stats.py
+-rw-rw-rw-   0        0        0     3807 2023-05-10 19:57:40.000000 reus-1.1.2/reus/fbref/fb_team_player_passing_type_stats.py
+-rw-rw-rw-   0        0        0     4870 2023-05-10 20:06:02.000000 reus-1.1.2/reus/fbref/fb_team_player_playing_time_stats.py
+-rw-rw-rw-   0        0        0     5548 2023-05-10 20:08:44.000000 reus-1.1.2/reus/fbref/fb_team_player_possession_stats.py
+-rw-rw-rw-   0        0        0     4208 2023-05-10 20:14:01.000000 reus-1.1.2/reus/fbref/fb_team_player_shooting_stats.py
+-rw-rw-rw-   0        0        0     5299 2023-05-10 20:28:25.000000 reus-1.1.2/reus/fbref/fb_team_player_summary_stats.py
+-rw-rw-rw-   0        0        0     4221 2023-05-10 22:30:19.000000 reus-1.1.2/reus/fbref/fb_team_playing_time_stats.py
+-rw-rw-rw-   0        0        0     5696 2023-05-11 15:11:25.000000 reus-1.1.2/reus/fbref/fb_team_possession_stats.py
+-rw-rw-rw-   0        0        0     4397 2023-05-11 15:11:27.000000 reus-1.1.2/reus/fbref/fb_team_shooting_stats.py
+-rw-rw-rw-   0        0        0     5217 2023-05-11 15:11:28.000000 reus-1.1.2/reus/fbref/fb_team_summary_stats.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:53:16.199519 reus-1.1.2/reus/fotmob/
+-rw-rw-rw-   0        0        0      557 2023-06-02 18:52:01.000000 reus-1.1.2/reus/fotmob/__init__.py
+-rw-rw-rw-   0        0        0     2462 2023-06-02 18:47:27.000000 reus-1.1.2/reus/fotmob/fm_league_ids.py
+-rw-rw-rw-   0        0        0     1304 2023-05-15 20:41:21.000000 reus-1.1.2/reus/fotmob/fm_league_matches.py
+-rw-rw-rw-   0        0        0     1452 2023-06-02 19:20:19.000000 reus-1.1.2/reus/fotmob/fm_league_table.py
+-rw-rw-rw-   0        0        0     2496 2023-06-02 18:43:54.000000 reus-1.1.2/reus/fotmob/fm_league_urls.py
+-rw-rw-rw-   0        0        0     1466 2023-05-11 15:29:50.000000 reus-1.1.2/reus/fotmob/fm_leagues.py
+-rw-rw-rw-   0        0        0    14981 2023-05-26 15:31:04.000000 reus-1.1.2/reus/fotmob/fm_match_data.py
+-rw-rw-rw-   0        0        0     1340 2022-10-16 18:56:44.000000 reus-1.1.2/reus/fotmob/fm_match_ids.py
+-rw-rw-rw-   0        0        0     1689 2023-06-02 18:20:03.000000 reus-1.1.2/reus/fotmob/fm_season_stat_leaders.py
+-rw-rw-rw-   0        0        0     1738 2023-06-02 18:23:50.000000 reus-1.1.2/reus/fotmob/fm_season_stats.py
+-rw-rw-rw-   0        0        0     3768 2023-04-22 23:43:18.000000 reus-1.1.2/reus/fotmob/util.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:53:16.209520 reus-1.1.2/reus/transfermarkt/
+-rw-rw-rw-   0        0        0      387 2023-06-02 18:52:23.000000 reus-1.1.2/reus/transfermarkt/__init__.py
+-rw-rw-rw-   0        0        0     1522 2023-05-12 15:42:49.000000 reus-1.1.2/reus/transfermarkt/tm_player_data.py
+-rw-rw-rw-   0        0        0     1660 2023-05-12 16:18:21.000000 reus-1.1.2/reus/transfermarkt/tm_player_injury.py
+-rw-rw-rw-   0        0        0     1843 2023-05-12 16:09:28.000000 reus-1.1.2/reus/transfermarkt/tm_player_market_value.py
+-rw-rw-rw-   0        0        0     8087 2023-05-12 16:18:15.000000 reus-1.1.2/reus/transfermarkt/tm_player_metadata.py
+-rw-rw-rw-   0        0        0     3460 2023-05-12 16:18:09.000000 reus-1.1.2/reus/transfermarkt/tm_player_transfers.py
+-rw-rw-rw-   0        0        0     5796 2023-05-12 16:06:28.000000 reus-1.1.2/reus/transfermarkt/tm_team_player_data.py
+-rw-rw-rw-   0        0        0     9782 2023-05-12 16:04:59.000000 reus-1.1.2/reus/transfermarkt/tm_team_transfers.py
+-rw-rw-rw-   0        0        0     2092 2023-05-12 16:07:09.000000 reus-1.1.2/reus/transfermarkt/util.py
+-rw-rw-rw-   0        0        0     1052 2023-06-02 18:48:58.000000 reus-1.1.2/reus/util.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:53:16.211520 reus-1.1.2/reus/utils/
+-rw-rw-rw-   0        0        0       91 2023-06-02 18:52:20.000000 reus-1.1.2/reus/utils/__init__.py
+-rw-rw-rw-   0        0        0     3972 2023-06-02 19:35:18.000000 reus-1.1.2/reus/utils/generate_standings.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:53:16.156519 reus-1.1.2/reus.egg-info/
+-rw-rw-rw-   0        0        0      616 2023-06-02 19:53:16.000000 reus-1.1.2/reus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2507 2023-06-02 19:53:16.000000 reus-1.1.2/reus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 19:53:16.000000 reus-1.1.2/reus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-02 19:53:16.000000 reus-1.1.2/reus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-02 19:53:16.000000 reus-1.1.2/reus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 19:53:16.213519 reus-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      883 2023-06-02 19:53:12.000000 reus-1.1.2/setup.py
```

### Comparing `reus-1.1.1/LICENSE` & `reus-1.1.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 ian-shepherd
+Copyright (c) 2023 ian-shepherd
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `reus-1.1.1/PKG-INFO` & `reus-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reus
-Version: 1.1.1
+Version: 1.1.2
 Summary: A package that allows you to soccer information
 Home-page: https://github.com/ian-shepherd/reus
 Author: Ian Shepherd
 License: UNKNOWN
 Keywords: python,fbref,fotmob,transfermarkt,soccer,football
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `reus-1.1.1/README.md` & `reus-1.1.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 [![PyPI version fury.io](https://badge.fury.io/py/reus.svg)](https://pypi.org/project/reus/) [![Lifecycle:
 experimental](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://www.tidyverse.org/lifecycle/#experimental) [![Twitter
 Follow](https://img.shields.io/twitter/follow/ishep123?style=social)](https://twitter.com/ishep123) [![Twitter
 Follow](https://img.shields.io/twitter/follow/theFirmAISports?style=social)](https://twitter.com/theFirmAISports)
 
 
-## Soccer/Football Team Information
+# Overview
 
-This package is designed to extract match statistics and league information from fbref in addition to player and team information from transfermarkt. Specific shoutout to [worldfootballR](https://github.com/JaseZiv/worldfootballR) and their associated [dataset](https://github.com/JaseZiv/worldfootballR_data) that provided the inspiration to build the python version.
+Reus is a Python library that provides a convenient way to scrape soccer data from various sources, including FBref, FotMob, and Transfermarkt. It aims to simplify the process of accessing and analyzing soccer-related information for data enthusiasts and sports analysts.
+
+## Features
+
+- Retrieve detailed soccer statistics, including player and team performance metrics.
+- Fetch fixture information for specific seasons and competitions.
+- Access transfer market data, including player transfers, contract details, and market values.
+
+## Inspiration
+
+Reus takes inspiration from the R package [worldfootballR](https://github.com/JaseZiv/worldfootballR), and their associated [dataset](https://github.com/JaseZiv/worldfootballR_data), which is known for its extensive soccer data scraping capabilities. While Reus mimics some of the functionalities of worldfootballR, it is designed specifically for Python users, providing similar functionality and ease of use.
 
 ## Installation
 
 You can install reus from [PyPi](https://pypi.org/project/reus/) with:
 
 ``` python
 pip install reus
@@ -26,18 +36,17 @@
 
 ```python
 time.sleep(4)
 ```
 
 It is a minor inconvenience to you but lets us all keep accessing the data.
 
-Additional documentation is provided [here](https://ian-shepherd.github.io/reus/)
+More detailed documentation is provided [here](https://ian-shepherd.github.io/reus/)
 
 ## Roadmap
-  - add fotmob league table and statistics functionality
   - translation function for players and teams
   - change outputs of fbref functions from lists and tuples to dictionaries
   - fbref player scouting reports
   - transfermarkt team staff
   - transfermarkt staff history
   - understat data
```

### Comparing `reus-1.1.1/reus/fbref/__init__.py` & `reus-1.1.2/reus/fbref/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.1.1"
+__version__ = "1.1.2"
 
 from .fb_season_fixture_urls import fb_season_fixture_urls
 from .fb_season_urls import fb_season_urls
 from .fb_league_table import fb_league_table
 from .fb_match_urls import fb_match_urls
 from .fb_match_data import fb_match_data
 from .fb_match_metadata import fb_match_metadata
```

### Comparing `reus-1.1.1/reus/fbref/fb_league_table.py` & `reus-1.1.2/reus/fbref/fb_league_table.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_match_data.py` & `reus-1.1.2/reus/fbref/fb_match_data.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_match_defensive_actions_stats.py` & `reus-1.1.2/reus/fbref/fb_match_defensive_actions_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_match_keeper_stats.py` & `reus-1.1.2/reus/fbref/fb_match_keeper_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_match_lineups.py` & `reus-1.1.2/reus/fbref/fb_match_lineups.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_match_metadata.py` & `reus-1.1.2/reus/fbref/fb_match_metadata.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_match_misc_stats.py` & `reus-1.1.2/reus/fbref/fb_match_misc_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_match_passing_stats.py` & `reus-1.1.2/reus/fbref/fb_match_passing_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_match_passing_type_stats.py` & `reus-1.1.2/reus/fbref/fb_match_passing_type_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_match_possession_stats.py` & `reus-1.1.2/reus/fbref/fb_match_possession_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_match_shots.py` & `reus-1.1.2/reus/fbref/fb_match_shots.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_match_summary.py` & `reus-1.1.2/reus/fbref/fb_match_summary.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_match_summary_stats.py` & `reus-1.1.2/reus/fbref/fb_match_summary_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_match_team_stats.py` & `reus-1.1.2/reus/fbref/fb_match_team_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_match_urls.py` & `reus-1.1.2/reus/fbref/fb_match_urls.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_season_fixture_urls.py` & `reus-1.1.2/reus/fotmob/fm_league_urls.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 import pandas as pd
 
 
-def fb_season_fixture_urls(
+def fm_league_urls(
     competition_type: str = None,
     competition_name: str = None,
+    ccode: str = None,
     country: str = None,
     gender: str = None,
-    governing_body: str = None,
-    tier: str = None,
-    season_end_year: int = None,
-    advanced: str = None,
 ) -> pd.Series:
-    """Returns a series of urls for fixture section of a season
+    """Returns a series of league urls for the current season
 
     Args:
-        competition_type (str or list, optional): type of competition. Defaults to None.
+        competition_type (str or list, optional): type of competition. Defaults to None. \n
+            'Domestic Leagues - 1st Tier' \n
+            'Domestic Leagues - 2nd Tier' \n
+            'Domestic Leagues - 3rd Tier and Lower' \n
+            'Domestic Cups' \n
+            'Domestic Youth Leagues' \n
+            'Club International Cups' \n
+            'National Team Competitions' \n
+            'National Team Qualification'
         competition_name (str or list, optional): name of competition. Defaults to None.
+        ccode (str or list, optional): country code of competition. Defaults to None.
         country (str or list, optional): country of competition. Defaults to None.
-        gender (str or list, optional): gender of competition. Defaults to None.
-        governing_body (str or list, optional): governing body of competition. Defaults to None.
-        tier (str or list, optional): tier of competition. Defaults to None.
-        season_end_year (int or list, optional): year at end of competition. Defaults to None.
-        advanced (str or list, optional): flag for if advanced data is available. Defaults to None.
+        gender (str or list, optional): gender of competition. Defaults to None. \n
+            'M' \n
+            'W'
 
     Returns:
-        series: season fixture urls
+        series: league urls
     """
 
     df = pd.read_csv(
-        "https://raw.githubusercontent.com/ian-shepherd/reus_data/main/raw-data/all_competitions.csv",
+        "https://raw.githubusercontent.com/ian-shepherd/reus_data/main/raw-data/fotmob_leagues.csv",
         keep_default_na=False,
+        encoding_errors="ignore",
     )
 
     # Competition type
     if competition_type is None:
         competition_type = df.competition_type.unique()
     elif not isinstance(competition_type, list):
         competition_type = [competition_type]
@@ -44,14 +49,22 @@
     if competition_name is None:
         competition_name = df.competition_name.unique()
     elif not isinstance(competition_name, list):
         competition_name = [competition_name]
 
     df = df[df.competition_name.isin(competition_name)]
 
+    # Country code
+    if ccode is None:
+        ccode = df.ccode.unique()
+    elif not isinstance(ccode, list):
+        ccode = [ccode]
+
+    df = df[df.ccode.isin(ccode)]
+
     # Country
     if country is None:
         country = df.country.unique()
     elif not isinstance(country, list):
         country = [country]
 
     df = df[df.country.isin(country)]
@@ -60,40 +73,8 @@
     if gender is None:
         gender = df.gender.unique()
     elif not isinstance(gender, list):
         gender = [gender]
 
     df = df[df.gender.isin(gender)]
 
-    # Governing body
-    if governing_body is None:
-        governing_body = df.governing_body.unique()
-    elif not isinstance(governing_body, list):
-        governing_body = [governing_body]
-
-    df = df[df.governing_body.isin(governing_body)]
-
-    # Tier
-    if tier is None:
-        tier = df.tier.unique()
-    elif not isinstance(tier, list):
-        tier = [tier]
-
-    df = df[df.tier.isin(tier)]
-
-    # Season end
-    if season_end_year is None:
-        season_end_year = df.season_end_year.unique()
-    elif not isinstance(season_end_year, list):
-        season_end_year = [season_end_year]
-
-    df = df[df.season_end_year.isin(season_end_year)]
-
-    # Advanced stats
-    if advanced is None:
-        advanced = df.advanced.unique()
-    elif not isinstance(advanced, list):
-        advanced = [advanced]
-
-    df = df[df.advanced.isin(advanced)]
-
-    return df["fixtures_url"]
+    return df.league_url
```

### Comparing `reus-1.1.1/reus/fbref/fb_season_urls.py` & `reus-1.1.2/reus/fotmob/fm_league_ids.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 import pandas as pd
 
 
-def fb_season_urls(
+def fm_league_ids(
     competition_type: str = None,
     competition_name: str = None,
+    ccode: str = None,
     country: str = None,
     gender: str = None,
-    governing_body: str = None,
-    tier: str = None,
-    season_end_year: int = None,
-    advanced: str = None,
 ) -> pd.Series:
-    """Returns a series of urls for overview section of a season
+    """Returns a series of league ids
 
     Args:
-        competition_type (str or list, optional): type of competition. Defaults to None.
+        competition_type (str or list, optional): type of competition. Defaults to None. \n
+            'Domestic Leagues - 1st Tier' \n
+            'Domestic Leagues - 2nd Tier' \n
+            'Domestic Leagues - 3rd Tier and Lower' \n
+            'Domestic Cups' \n
+            'Domestic Youth Leagues' \n
+            'Club International Cups' \n
+            'National Team Competitions' \n
+            'National Team Qualification'
         competition_name (str or list, optional): name of competition. Defaults to None.
+        ccode (str or list, optional): country code of competition. Defaults to None.
         country (str or list, optional): country of competition. Defaults to None.
-        gender (str or list, optional): gender of competition. Defaults to None.
-        governing_body (str or list, optional): governing body of competition. Defaults to None.
-        tier (str or list, optional): tier of competition. Defaults to None.
-        season_end_year (int or list, optional): year at end of competition. Defaults to None.
-        advanced (str or list, optional): flag for if advanced data is available. Defaults to None.
+        gender (str or list, optional): gender of competition. Defaults to None. \n
+            'M' \n
+            'W'
 
     Returns:
-        series: season urls
+        series: league ids
     """
 
     df = pd.read_csv(
-        "https://raw.githubusercontent.com/ian-shepherd/reus_data/main/raw-data/all_competitions.csv",
+        "https://raw.githubusercontent.com/ian-shepherd/reus_data/main/raw-data/fotmob_leagues.csv",
         keep_default_na=False,
+        encoding_errors="ignore",
     )
 
     # Competition type
     if competition_type is None:
         competition_type = df.competition_type.unique()
     elif not isinstance(competition_type, list):
         competition_type = [competition_type]
@@ -44,14 +49,22 @@
     if competition_name is None:
         competition_name = df.competition_name.unique()
     elif not isinstance(competition_name, list):
         competition_name = [competition_name]
 
     df = df[df.competition_name.isin(competition_name)]
 
+    # Country code
+    if ccode is None:
+        ccode = df.ccode.unique()
+    elif not isinstance(ccode, list):
+        ccode = [ccode]
+
+    df = df[df.ccode.isin(ccode)]
+
     # Country
     if country is None:
         country = df.country.unique()
     elif not isinstance(country, list):
         country = [country]
 
     df = df[df.country.isin(country)]
@@ -60,40 +73,8 @@
     if gender is None:
         gender = df.gender.unique()
     elif not isinstance(gender, list):
         gender = [gender]
 
     df = df[df.gender.isin(gender)]
 
-    # Governing body
-    if governing_body is None:
-        governing_body = df.governing_body.unique()
-    elif not isinstance(governing_body, list):
-        governing_body = [governing_body]
-
-    df = df[df.governing_body.isin(governing_body)]
-
-    # Tier
-    if tier is None:
-        tier = df.tier.unique()
-    elif not isinstance(tier, list):
-        tier = [tier]
-
-    df = df[df.tier.isin(tier)]
-
-    # Season end
-    if season_end_year is None:
-        season_end_year = df.season_end_year.unique()
-    elif not isinstance(season_end_year, list):
-        season_end_year = [season_end_year]
-
-    df = df[df.season_end_year.isin(season_end_year)]
-
-    # Advanced stats
-    if advanced is None:
-        advanced = df.advanced.unique()
-    elif not isinstance(advanced, list):
-        advanced = [advanced]
-
-    df = df[df.advanced.isin(advanced)]
-
-    return df["seasons_urls"]
+    return df.id
```

### Comparing `reus-1.1.1/reus/fbref/fb_team_advanced_keeper_stats.py` & `reus-1.1.2/reus/fbref/fb_team_advanced_keeper_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_team_data.py` & `reus-1.1.2/reus/fbref/fb_team_data.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_team_defensive_actions_stats.py` & `reus-1.1.2/reus/fbref/fb_team_defensive_actions_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_team_goal_sca_stats.py` & `reus-1.1.2/reus/fbref/fb_team_goal_sca_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_team_keeper_stats.py` & `reus-1.1.2/reus/fbref/fb_team_keeper_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_team_misc_stats.py` & `reus-1.1.2/reus/fbref/fb_team_misc_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_team_passing_stats.py` & `reus-1.1.2/reus/fbref/fb_team_passing_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_team_passing_type_stats.py` & `reus-1.1.2/reus/fbref/fb_team_passing_type_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_team_player_advanced_keeper_stats.py` & `reus-1.1.2/reus/fbref/fb_team_player_advanced_keeper_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_team_player_data.py` & `reus-1.1.2/reus/fbref/fb_team_player_data.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_team_player_defensive_actions_stats.py` & `reus-1.1.2/reus/fbref/fb_team_player_defensive_actions_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_team_player_goal_sca_stats.py` & `reus-1.1.2/reus/fbref/fb_team_player_goal_sca_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_team_player_keeper_stats.py` & `reus-1.1.2/reus/fbref/fb_team_player_keeper_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_team_player_misc_stats.py` & `reus-1.1.2/reus/fbref/fb_team_player_misc_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_team_player_passing_stats.py` & `reus-1.1.2/reus/fbref/fb_team_player_passing_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_team_player_passing_type_stats.py` & `reus-1.1.2/reus/fbref/fb_team_player_passing_type_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_team_player_playing_time_stats.py` & `reus-1.1.2/reus/fbref/fb_team_player_playing_time_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_team_player_possession_stats.py` & `reus-1.1.2/reus/fbref/fb_team_player_possession_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_team_player_shooting_stats.py` & `reus-1.1.2/reus/fbref/fb_team_player_shooting_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_team_player_summary_stats.py` & `reus-1.1.2/reus/fbref/fb_team_player_summary_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_team_playing_time_stats.py` & `reus-1.1.2/reus/fbref/fb_team_playing_time_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_team_possession_stats.py` & `reus-1.1.2/reus/fbref/fb_team_possession_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_team_shooting_stats.py` & `reus-1.1.2/reus/fbref/fb_team_shooting_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fbref/fb_team_summary_stats.py` & `reus-1.1.2/reus/fbref/fb_team_summary_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fotmob/fm_leagues.py` & `reus-1.1.2/reus/fotmob/fm_leagues.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fotmob/fm_match_data.py` & `reus-1.1.2/reus/fotmob/fm_match_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,22 +8,24 @@
 def fm_match_data(
     match_id: str, save_json: bool = False, json_file: json = None
 ) -> tuple:
     """Returns metadata and match data for a given match id
 
     Args:
         match_id (str): id of a match
+        save_json (bool, optional): whether to save json file. Defaults to False.
+        json_file (json, optional): json file of match data. Defaults to None.
 
     Returns:
         tuple: match data
             dict: metadata information
             list: events
             list: shots
             list: bench players
-            list starters
+            list: starters
             list: players not available
             list: shootout
             json: json file (if save_json=True)
     """
 
     assert isinstance(match_id, str), "match_id must be a string"
 
@@ -279,15 +281,16 @@
 
         for j in i.get("players"):
             for k in j:
                 mydict = {}
                 mydict["team_id"] = team_id
                 mydict["opta_id"] = k.get("usingOptaId")
                 mydict["player_id"] = k.get("id")
-                mydict["player_name"] = " ".join(k.get("name").values())
+                # mydict["player_name"] = " ".join(k.get("name").values())
+                mydict["player_name"] = k.get("name").get("fullName")
                 mydict["player_url"] = k.get("pageUrl")
                 mydict["shirt_number"] = k.get("shirt")
                 mydict["time_subbed_on"] = k.get("timeSubbedOn")
                 mydict["time_subbed_off"] = k.get("timeSubbedOff")
                 mydict["minutes_played"] = k.get("minutesPlayed")
                 mydict["position"] = k.get("positionStringShort")
                 mydict["usual_position"] = k.get("usualPosition")
```

### Comparing `reus-1.1.1/reus/fotmob/fm_match_ids.py` & `reus-1.1.2/reus/fotmob/fm_match_ids.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/fotmob/util.py` & `reus-1.1.2/reus/fotmob/util.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/transfermarkt/tm_player_data.py` & `reus-1.1.2/reus/transfermarkt/tm_player_data.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/transfermarkt/tm_player_injury.py` & `reus-1.1.2/reus/transfermarkt/tm_player_injury.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/transfermarkt/tm_player_market_value.py` & `reus-1.1.2/reus/transfermarkt/tm_player_market_value.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/transfermarkt/tm_player_metadata.py` & `reus-1.1.2/reus/transfermarkt/tm_player_metadata.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/transfermarkt/tm_player_transfers.py` & `reus-1.1.2/reus/transfermarkt/tm_player_transfers.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/transfermarkt/tm_team_player_data.py` & `reus-1.1.2/reus/transfermarkt/tm_team_player_data.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/transfermarkt/tm_team_transfers.py` & `reus-1.1.2/reus/transfermarkt/tm_team_transfers.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/transfermarkt/util.py` & `reus-1.1.2/reus/transfermarkt/util.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus/util.py` & `reus-1.1.2/reus/util.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.1/reus.egg-info/PKG-INFO` & `reus-1.1.2/reus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reus
-Version: 1.1.1
+Version: 1.1.2
 Summary: A package that allows you to soccer information
 Home-page: https://github.com/ian-shepherd/reus
 Author: Ian Shepherd
 License: UNKNOWN
 Keywords: python,fbref,fotmob,transfermarkt,soccer,football
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `reus-1.1.1/reus.egg-info/SOURCES.txt` & `reus-1.1.2/reus.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -47,20 +47,28 @@
 reus/fbref/fb_team_player_shooting_stats.py
 reus/fbref/fb_team_player_summary_stats.py
 reus/fbref/fb_team_playing_time_stats.py
 reus/fbref/fb_team_possession_stats.py
 reus/fbref/fb_team_shooting_stats.py
 reus/fbref/fb_team_summary_stats.py
 reus/fotmob/__init__.py
+reus/fotmob/fm_league_ids.py
+reus/fotmob/fm_league_matches.py
+reus/fotmob/fm_league_table.py
+reus/fotmob/fm_league_urls.py
 reus/fotmob/fm_leagues.py
 reus/fotmob/fm_match_data.py
 reus/fotmob/fm_match_ids.py
+reus/fotmob/fm_season_stat_leaders.py
+reus/fotmob/fm_season_stats.py
 reus/fotmob/util.py
 reus/transfermarkt/__init__.py
 reus/transfermarkt/tm_player_data.py
 reus/transfermarkt/tm_player_injury.py
 reus/transfermarkt/tm_player_market_value.py
 reus/transfermarkt/tm_player_metadata.py
 reus/transfermarkt/tm_player_transfers.py
 reus/transfermarkt/tm_team_player_data.py
 reus/transfermarkt/tm_team_transfers.py
-reus/transfermarkt/util.py
+reus/transfermarkt/util.py
+reus/utils/__init__.py
+reus/utils/generate_standings.py
```

### Comparing `reus-1.1.1/setup.py` & `reus-1.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-VERSION = "1.1.1"
+VERSION = "1.1.2"
 DESCRIPTION = "A package that allows you to soccer information"
 LONG_DESCRIPTION = """
     A package that allows you to pull soccer statistics, player market values, and
      transfer information, primarily from FBref, Fotmob, and Transfermarkt"""
 
 setuptools.setup(
     name="reus",
```

