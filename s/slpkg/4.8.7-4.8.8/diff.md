# Comparing `tmp/slpkg-4.8.7.tar.gz` & `tmp/slpkg-4.8.8.tar.gz`

## Comparing `slpkg-4.8.7.tar` & `slpkg-4.8.8.tar`

### file list

```diff
@@ -1,106 +1,107 @@
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-26 09:24:47.000000 slpkg-4.8.7/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/filelists/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/filelists/multilib/
--rw-r--r--   0 dslackw   (1000) users      (100)    15477 2023-05-26 09:20:22.000000 slpkg-4.8.7/filelists/multilib/README.ERIC
--rw-r--r--   0 dslackw   (1000) users      (100)      250 2023-05-26 09:20:22.000000 slpkg-4.8.7/filelists/multilib/glibc_packages.pkgs
--rw-r--r--   0 dslackw   (1000) users      (100)      831 2023-05-26 09:20:22.000000 slpkg-4.8.7/filelists/multilib/README
--rw-r--r--   0 dslackw   (1000) users      (100)     4508 2023-05-26 09:20:22.000000 slpkg-4.8.7/filelists/multilib/compat32.pkgs
--rw-r--r--   0 dslackw   (1000) users      (100)       88 2023-05-26 09:20:22.000000 slpkg-4.8.7/filelists/README
--rw-r--r--   0 dslackw   (1000) users      (100)     1189 2023-05-26 09:20:22.000000 slpkg-4.8.7/repositories.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/slackbuild/
--rw-r--r--   0 dslackw   (1000) users      (100)      941 2023-05-26 09:20:22.000000 slpkg-4.8.7/slackbuild/slack-desc
--rw-r--r--   0 dslackw   (1000) users      (100)      464 2023-05-26 09:20:22.000000 slpkg-4.8.7/slackbuild/doinst.sh
--rw-r--r--   0 dslackw   (1000) users      (100)      304 2023-05-26 09:20:22.000000 slpkg-4.8.7/slackbuild/README
--rwxr-xr-x   0 dslackw   (1000) users      (100)     4262 2023-05-26 09:20:22.000000 slpkg-4.8.7/slackbuild/slpkg.SlackBuild
--rwxr-xr-x   0 dslackw   (1000) users      (100)       70 2023-05-26 09:20:22.000000 slpkg-4.8.7/setup.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1520 2023-05-26 09:20:22.000000 slpkg-4.8.7/.pyproject.toml
--rw-r--r--   0 dslackw   (1000) users      (100)       84 2023-05-26 09:20:22.000000 slpkg-4.8.7/requirements.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/configs/
--rw-r--r--   0 dslackw   (1000) users      (100)     8802 2023-05-26 09:20:22.000000 slpkg-4.8.7/configs/repositories.toml
--rw-r--r--   0 dslackw   (1000) users      (100)      483 2023-05-26 09:20:22.000000 slpkg-4.8.7/configs/blacklist.toml
--rw-r--r--   0 dslackw   (1000) users      (100)     4129 2023-05-26 09:20:22.000000 slpkg-4.8.7/configs/slpkg.toml
--rw-r--r--   0 dslackw   (1000) users      (100)      381 2023-05-26 09:20:22.000000 slpkg-4.8.7/configs/rules.toml
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/tests/
--rw-r--r--   0 dslackw   (1000) users      (100)     2337 2023-05-26 09:20:22.000000 slpkg-4.8.7/tests/test_configs.py
--rw-r--r--   0 dslackw   (1000) users      (100)      765 2023-05-26 09:20:22.000000 slpkg-4.8.7/tests/test_checks.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1961 2023-05-26 09:20:22.000000 slpkg-4.8.7/tests/test_utilities.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1565 2023-05-26 09:20:22.000000 slpkg-4.8.7/tests/test_sbo_queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)      256 2023-05-26 09:20:22.000000 slpkg-4.8.7/tests/test_blacklist.py
--rw-r--r--   0 dslackw   (1000) users      (100)      898 2023-05-26 09:20:22.000000 slpkg-4.8.7/tests/test_colors.py
--rw-r--r--   0 dslackw   (1000) users      (100)      902 2023-05-26 09:20:22.000000 slpkg-4.8.7/tests/check_updates_test.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1460 2023-05-26 09:20:22.000000 slpkg-4.8.7/tests/test_upgrade.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1716 2023-05-26 09:20:22.000000 slpkg-4.8.7/tests/test_bin_queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1076 2023-05-26 09:20:22.000000 slpkg-4.8.7/LICENSE
--rwxr-xr-x   0 dslackw   (1000) users      (100)     1624 2023-05-26 09:20:22.000000 slpkg-4.8.7/install.sh
--rw-r--r--   0 dslackw   (1000) users      (100)    46862 2023-05-26 09:20:22.000000 slpkg-4.8.7/ChangeLog.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/man/
--rw-r--r--   0 dslackw   (1000) users      (100)     9677 2023-05-26 09:20:22.000000 slpkg-4.8.7/man/slpkg.1
--rw-r--r--   0 dslackw   (1000) users      (100)     9919 2023-05-26 09:20:22.000000 slpkg-4.8.7/man/slpkg-fr.1
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/completion/
--rw-r--r--   0 dslackw   (1000) users      (100)      910 2023-05-26 09:20:22.000000 slpkg-4.8.7/completion/slpkg
--rw-r--r--   0 dslackw   (1000) users      (100)       93 2023-05-26 09:20:22.000000 slpkg-4.8.7/.gitignore
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/
--rw-r--r--   0 dslackw   (1000) users      (100)     4289 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/dialog_configs.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/binaries/
--rw-r--r--   0 dslackw   (1000) users      (100)     1892 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/binaries/required.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1439 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/binaries/queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/binaries/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     7565 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/binaries/install.py
--rw-r--r--   0 dslackw   (1000) users      (100)    65376 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/install_data.py
--rw-r--r--   0 dslackw   (1000) users      (100)    31419 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/repositories.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4367 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/repo_info.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/sbos/
--rw-r--r--   0 dslackw   (1000) users      (100)     1605 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/sbos/queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)    11615 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/sbos/slackbuild.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1151 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/sbos/dependencies.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/sbos/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4483 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/sbos/sbo_generate.py
--rw-r--r--   0 dslackw   (1000) users      (100)    36482 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/update_repository.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2627 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/progress_bar.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3163 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/downloader.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/models/
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/models/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2655 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/models/models.py
--rw-r--r--   0 dslackw   (1000) users      (100)      887 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/rules.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/views/
--rw-r--r--   0 dslackw   (1000) users      (100)     6604 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/views/view_package.py
--rw-r--r--   0 dslackw   (1000) users      (100)      629 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/views/version.py
--rw-r--r--   0 dslackw   (1000) users      (100)     6335 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/views/cli_menu.py
--rw-r--r--   0 dslackw   (1000) users      (100)     5935 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/views/asciibox.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4110 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/views/help_commands.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/views/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)    10274 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/views/views.py
--rw-r--r--   0 dslackw   (1000) users      (100)      430 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/error_messages.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3637 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/checks.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1350 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/logging_deps.py
--rw-r--r--   0 dslackw   (1000) users      (100)    13634 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/new_configs.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2058 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/multi_process.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3211 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/cleanings.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1881 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/checksum.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1906 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/dialog_box.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4812 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/configs.py
--rw-r--r--   0 dslackw   (1000) users      (100)     7857 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/utilities.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3867 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/dependees.py
--rw-r--r--   0 dslackw   (1000) users      (100)      587 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/toml_error_message.py
--rw-r--r--   0 dslackw   (1000) users      (100)     6100 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/check_updates.py
--rw-r--r--   0 dslackw   (1000) users      (100)     6716 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/remove_packages.py
--rw-r--r--   0 dslackw   (1000) users      (100)      916 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/blacklist.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3481 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/download_only.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4147 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/tracking.py
--rw-r--r--   0 dslackw   (1000) users      (100)      514 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/logging_config.py
--rw-r--r--   0 dslackw   (1000) users      (100)    33380 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/main.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1609 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/find_installed.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4041 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/upgrade.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3428 2023-05-26 09:20:22.000000 slpkg-4.8.7/slpkg/search.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1466 2023-05-26 09:20:22.000000 slpkg-4.8.7/setup.cfg
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-26 09:24:43.000000 slpkg-4.8.7/slpkg.egg-info/
--rw-r--r--   0 dslackw   (1000) users      (100)       86 2023-05-26 09:24:43.000000 slpkg-4.8.7/slpkg.egg-info/entry_points.txt
--rw-r--r--   0 dslackw   (1000) users      (100)        1 2023-05-26 09:24:43.000000 slpkg-4.8.7/slpkg.egg-info/dependency_links.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     1301 2023-05-26 09:24:43.000000 slpkg-4.8.7/slpkg.egg-info/SOURCES.txt
--rw-r--r--   0 dslackw   (1000) users      (100)        6 2023-05-26 09:24:43.000000 slpkg-4.8.7/slpkg.egg-info/top_level.txt
--rw-r--r--   0 dslackw   (1000) users      (100)       77 2023-05-26 09:24:43.000000 slpkg-4.8.7/slpkg.egg-info/requires.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     1257 2023-05-26 09:24:43.000000 slpkg-4.8.7/slpkg.egg-info/PKG-INFO
--rw-r--r--   0 dslackw   (1000) users      (100)     8595 2023-05-26 09:20:22.000000 slpkg-4.8.7/README.md
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-26 09:20:22.000000 slpkg-4.8.7/tools/
--rwxr-xr-x   0 dslackw   (1000) users      (100)      787 2023-05-26 09:20:22.000000 slpkg-4.8.7/tools/gen_sbo_txt.sh
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-02 14:40:58.000000 slpkg-4.8.8/
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/filelists/
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/filelists/multilib/
+-rw-r--r--   0 dslackw   (1000) users      (100)    15477 2023-06-02 14:31:34.000000 slpkg-4.8.8/filelists/multilib/README.ERIC
+-rw-r--r--   0 dslackw   (1000) users      (100)      250 2023-06-02 14:31:34.000000 slpkg-4.8.8/filelists/multilib/glibc_packages.pkgs
+-rw-r--r--   0 dslackw   (1000) users      (100)      831 2023-06-02 14:31:34.000000 slpkg-4.8.8/filelists/multilib/README
+-rw-r--r--   0 dslackw   (1000) users      (100)     4508 2023-06-02 14:31:34.000000 slpkg-4.8.8/filelists/multilib/compat32.pkgs
+-rw-r--r--   0 dslackw   (1000) users      (100)       88 2023-06-02 14:31:34.000000 slpkg-4.8.8/filelists/README
+-rw-r--r--   0 dslackw   (1000) users      (100)     1189 2023-06-02 14:31:34.000000 slpkg-4.8.8/repositories.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/slackbuild/
+-rw-r--r--   0 dslackw   (1000) users      (100)      941 2023-06-02 14:31:34.000000 slpkg-4.8.8/slackbuild/slack-desc
+-rw-r--r--   0 dslackw   (1000) users      (100)      334 2023-06-02 14:31:34.000000 slpkg-4.8.8/slackbuild/doinst.sh
+-rw-r--r--   0 dslackw   (1000) users      (100)      304 2023-06-02 14:31:34.000000 slpkg-4.8.8/slackbuild/README
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     4112 2023-06-02 14:31:34.000000 slpkg-4.8.8/slackbuild/slpkg.SlackBuild
+-rwxr-xr-x   0 dslackw   (1000) users      (100)       70 2023-06-02 14:31:34.000000 slpkg-4.8.8/setup.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1520 2023-06-02 14:31:34.000000 slpkg-4.8.8/.pyproject.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)       84 2023-06-02 14:31:34.000000 slpkg-4.8.8/requirements.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/configs/
+-rw-r--r--   0 dslackw   (1000) users      (100)     8802 2023-06-02 14:31:34.000000 slpkg-4.8.8/configs/repositories.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)      483 2023-06-02 14:31:34.000000 slpkg-4.8.8/configs/blacklist.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)     4129 2023-06-02 14:31:34.000000 slpkg-4.8.8/configs/slpkg.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)      381 2023-06-02 14:31:34.000000 slpkg-4.8.8/configs/rules.toml
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/tests/
+-rw-r--r--   0 dslackw   (1000) users      (100)     2337 2023-06-02 14:31:34.000000 slpkg-4.8.8/tests/test_configs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      765 2023-06-02 14:31:34.000000 slpkg-4.8.8/tests/test_checks.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1961 2023-06-02 14:31:34.000000 slpkg-4.8.8/tests/test_utilities.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1565 2023-06-02 14:31:34.000000 slpkg-4.8.8/tests/test_sbo_queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      256 2023-06-02 14:31:34.000000 slpkg-4.8.8/tests/test_blacklist.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      898 2023-06-02 14:31:34.000000 slpkg-4.8.8/tests/test_colors.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      902 2023-06-02 14:31:34.000000 slpkg-4.8.8/tests/check_updates_test.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1460 2023-06-02 14:31:34.000000 slpkg-4.8.8/tests/test_upgrade.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1716 2023-06-02 14:31:34.000000 slpkg-4.8.8/tests/test_bin_queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1076 2023-06-02 14:31:34.000000 slpkg-4.8.8/LICENSE
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     1624 2023-06-02 14:31:34.000000 slpkg-4.8.8/install.sh
+-rw-r--r--   0 dslackw   (1000) users      (100)    47093 2023-06-02 14:31:34.000000 slpkg-4.8.8/ChangeLog.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/man/
+-rw-r--r--   0 dslackw   (1000) users      (100)     9677 2023-06-02 14:31:34.000000 slpkg-4.8.8/man/slpkg.1
+-rw-r--r--   0 dslackw   (1000) users      (100)    10867 2023-06-02 14:31:34.000000 slpkg-4.8.8/man/slpkg-fr.1
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/completion/
+-rw-r--r--   0 dslackw   (1000) users      (100)      910 2023-06-02 14:31:34.000000 slpkg-4.8.8/completion/slpkg
+-rw-r--r--   0 dslackw   (1000) users      (100)       93 2023-06-02 14:31:34.000000 slpkg-4.8.8/.gitignore
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/
+-rw-r--r--   0 dslackw   (1000) users      (100)     4289 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/dialog_configs.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/binaries/
+-rw-r--r--   0 dslackw   (1000) users      (100)     1892 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/binaries/required.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1439 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/binaries/queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/binaries/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     7698 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/binaries/install.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    65384 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/install_data.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    31419 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/repositories.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4367 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/repo_info.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/sbos/
+-rw-r--r--   0 dslackw   (1000) users      (100)     1605 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/sbos/queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    11675 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/sbos/slackbuild.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1151 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/sbos/dependencies.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/sbos/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4483 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/sbos/sbo_generate.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    36699 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/update_repository.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2627 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/progress_bar.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3510 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/downloader.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/models/
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/models/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2655 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/models/models.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      887 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/rules.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/views/
+-rw-r--r--   0 dslackw   (1000) users      (100)     6604 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/views/view_package.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      629 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/views/version.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     6335 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/views/cli_menu.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     5935 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/views/asciibox.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4110 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/views/help_commands.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/views/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    10274 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/views/views.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4004 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/choose_packages.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      430 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/error_messages.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3637 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/checks.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1350 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/logging_deps.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    13634 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/new_configs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2058 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/multi_process.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3211 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/cleanings.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1881 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/checksum.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1906 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/dialog_box.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4812 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/configs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     7857 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/utilities.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3867 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/dependees.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      587 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/toml_error_message.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     6100 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/check_updates.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     6716 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/remove_packages.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      916 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/blacklist.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3491 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/download_only.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4147 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/tracking.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      514 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/logging_config.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    29920 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/main.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1609 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/find_installed.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4041 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/upgrade.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3428 2023-06-02 14:31:34.000000 slpkg-4.8.8/slpkg/search.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1466 2023-06-02 14:31:34.000000 slpkg-4.8.8/setup.cfg
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-02 14:40:55.000000 slpkg-4.8.8/slpkg.egg-info/
+-rw-r--r--   0 dslackw   (1000) users      (100)       86 2023-06-02 14:40:55.000000 slpkg-4.8.8/slpkg.egg-info/entry_points.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)        1 2023-06-02 14:40:55.000000 slpkg-4.8.8/slpkg.egg-info/dependency_links.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     1326 2023-06-02 14:40:55.000000 slpkg-4.8.8/slpkg.egg-info/SOURCES.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)        6 2023-06-02 14:40:55.000000 slpkg-4.8.8/slpkg.egg-info/top_level.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)       77 2023-06-02 14:40:55.000000 slpkg-4.8.8/slpkg.egg-info/requires.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     1257 2023-06-02 14:40:55.000000 slpkg-4.8.8/slpkg.egg-info/PKG-INFO
+-rw-r--r--   0 dslackw   (1000) users      (100)     8595 2023-06-02 14:31:34.000000 slpkg-4.8.8/README.md
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-02 14:31:34.000000 slpkg-4.8.8/tools/
+-rwxr-xr-x   0 dslackw   (1000) users      (100)      787 2023-06-02 14:31:34.000000 slpkg-4.8.8/tools/gen_sbo_txt.sh
```

### Comparing `slpkg-4.8.7/filelists/multilib/README.ERIC` & `slpkg-4.8.8/filelists/multilib/README.ERIC`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/filelists/multilib/README` & `slpkg-4.8.8/filelists/multilib/README`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/filelists/multilib/compat32.pkgs` & `slpkg-4.8.8/filelists/multilib/compat32.pkgs`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/repositories.txt` & `slpkg-4.8.8/repositories.txt`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slackbuild/slack-desc` & `slpkg-4.8.8/slackbuild/slack-desc`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slackbuild/slpkg.SlackBuild` & `slpkg-4.8.8/slackbuild/slpkg.SlackBuild`

 * *Files 14% similar despite different names*

```diff
@@ -94,18 +94,18 @@
 rm -rf $PKG/usr/bin
 
 find $PKG -print0 | xargs -0 file | grep -e "executable" -e "shared object" | grep ELF \
   | cut -f 1 -d : | xargs strip --strip-unneeded 2> /dev/null || true
 
 # Install configuration files and creating lib directory
 mkdir -p $PKG/etc/$PRGNAM
-install -D -m0644 configs/slpkg.toml $PKG/etc/slpkg/slpkg.toml.new
-install -D -m0644 configs/repositories.toml $PKG/etc/slpkg/repositories.toml.new
-install -D -m0644 configs/blacklist.toml $PKG/etc/slpkg/blacklist.toml.new
-install -D -m0644 configs/rules.toml $PKG/etc/slpkg/rules.toml.new
+FILES="slpkg repositories blacklist rules"
+for file in $FILES; do
+  install -D -m0644 configs/$file.toml $PKG/etc/slpkg/$file.toml.new
+done
 
 mkdir -p $PKG/usr/man/man1 & mkdir -p $PKG/usr/man/fr/man1
 cp man/slpkg.1 $PKG/usr/man/man1
 cp man/slpkg-fr.1 $PKG/usr/man/fr/man1/slpkg.1
 
 find $PKG/usr/man -type f -exec gzip -9 {} \;
 for i in $( find $PKG/usr/man -type l ) ; do ln -s $( readlink $i ).gz $i.gz; rm $i ; done
```

### Comparing `slpkg-4.8.7/.pyproject.toml` & `slpkg-4.8.8/.pyproject.toml`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/configs/repositories.toml` & `slpkg-4.8.8/configs/repositories.toml`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/configs/slpkg.toml` & `slpkg-4.8.8/configs/slpkg.toml`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/tests/test_configs.py` & `slpkg-4.8.8/tests/test_configs.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/tests/test_checks.py` & `slpkg-4.8.8/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/tests/test_utilities.py` & `slpkg-4.8.8/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/tests/test_sbo_queries.py` & `slpkg-4.8.8/tests/test_sbo_queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/tests/test_colors.py` & `slpkg-4.8.8/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/tests/check_updates_test.py` & `slpkg-4.8.8/tests/check_updates_test.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/tests/test_upgrade.py` & `slpkg-4.8.8/tests/test_upgrade.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/tests/test_bin_queries.py` & `slpkg-4.8.8/tests/test_bin_queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/LICENSE` & `slpkg-4.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/install.sh` & `slpkg-4.8.8/install.sh`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/ChangeLog.txt` & `slpkg-4.8.8/ChangeLog.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+4.8.8 - 29/05/2023
+Updated:
+- France manpage
+Fixed:
+- Choose dependencies for upgraded packages
+- Build packages with the same source name:
+  (nvidia-driver and nvidia-kernel use the same source NVIDIA-Linux-x86_64-<VERSION>.run)
+
 4.8.7 - 23/05/2023
 Fixed:
 - Package tag for slack_patches and salixos_patches
 - Parallel download for slackbuilds repositories (sbo, ponce)
 
 4.8.6 - 21/05/2023
 Updated:
```

### Comparing `slpkg-4.8.7/man/slpkg.1` & `slpkg-4.8.8/man/slpkg.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH slpkg 1 "Orestiada, Greece" "slpkg 4.8.5" dslackw
+.TH slpkg 1 "Orestiada, Hellas" "slpkg 4.8.5" dslackw
 .SH NAME
 .P
 slpkg \- Package manager utility for Slackware.
 .SH SYNOPSIS
 .P
 slpkg \c
 [\fICOMMAND\fR] [\fIOPTIONS\fR] [\fIFILELIST|PACKAGES...\fR]
```

### Comparing `slpkg-4.8.7/man/slpkg-fr.1` & `slpkg-4.8.8/man/slpkg-fr.1`

 * *Files 21% similar despite different names*

```diff
@@ -1,255 +1,288 @@
-.TH slpkg 1 "Orestiada, Grèce" "slpkg 4.7.3" dslackw
+.TH slpkg 1 "Orestiada, Grèce" "slpkg 4.8.5" dslackw
 .SH NOM
 .P
-slpkg \- Package manager pour Slackware.
+slpkg \- Utilitaire de gestion de paquets pour Slackware.
 .SH SYNOPSIS
 .P
 slpkg \c
 [\fICOMMAND\fR] [\fIOPTIONS\fR] [\fIFILELIST|PACKAGES...\fR]
 .P
-slpkg [-h|-v] [-u, update] [-U, upgrade] [-c, check-updates] [-I, repo-info] [-g, configs] [-L, clean-logs]
-[-D, clean-tmp] [-T, clean-data] [-b, build] [-i, install] [-d, download]
-[-R, remove] [-f, find] [-w, view] [-s, search] [-e, dependees] [-t, tracking] -y, --yes, -j, --jobs, -o, --resolve-off,
--r, --reinstall, -k, --skip-installed, -E, --full-reverse, -S, --search, -n, --no-silent, -p, --pkg-version, -z,
--G, --generate-only, -P, --parallel, -B, --bin-repo=[\fIPATH\fR], -z, --directory=[\fIPATH\fR]
+slpkg [-h|-v] [-u, update] [-U, upgrade] [-c, check-updates] [-I, repo-info] [-g, configs]
+[-L, clean-logs] [-D, clean-tmp] [-T, clean-data] [-b, build] [-i, install] [-d, download]
+[-R, remove] [-f, find] [-w, view] [-s, search] [-e, dependees] [-t, tracking] -y, --yes, -j, --jobs, -O, --resolve-off,
+-r, --reinstall, -k, --skip-installed, -a, --install-data, -E, --full-reverse, -S, --search, -n, --no-silent, -p, --pkg-version,
+-P, --parallel, -o, --repository=\fINAME\fR, -z, --directory=\fIPATH\fR
 .SH DESCRIPTION
 .P
-\fBSlpkg\fP est un gestionnaire de paquets logiciels qui \fBinstalle\fP, \fBmet à jour\fP et \fBsupprime\fP les paquets pour les systèmes basés sur \fBSlackware\fP.
-Il calcule automatiquement \fBles dépendances\fP et détermine comment doit se dérouler l'installation des paquets.
-\fBSlpkg\fP facilite la maintenance de groupes de machines sans avoir à effectuer des mises à jour manuelles.
+Slpkg est un gestionnaire de paquets qui installe, met à jour et supprime les paquets sur les systèmes basés sur Slackware. 
+Il calcule automatiquement les dépendances et détermine ce qui doit se passer pour installer les paquets. 
+Slpkg facilite la maintenance de groupes de machines sans avoir à les mettre à jour manuellement. 
 .P
-\fBSlpkg\fP travaille en accord avec les standards du projet \fBSlackBuilds.org\fP pour construire des paquets.
-Il utilise également les instructions de \fBSlackware Linux\fP pour l'installation, la mise à jour ainsi que la suppression des paquets.
+Slpkg travaille en accord avec les standards de l'organisation SlackBuilds.org pour construire des paquets. 
+Il utilise également les instructions de Slackware Linux pour l'installation, la mise à jour ou la suppression des paquets. 
 .SH COMMANDES
 .P
 .B -u, update
 .RS
-Mettre à jour la liste des paquets et la base de données.
+Met à jour la liste des paquets et la base de données.
 .RE
 .P
 .B -U, upgrade
 .RS
-Mettre à niveau tous les paquets installés si une version plus récente existe dans le dépôt.
+Met à jour tous les paquets installés si une version plus récente existe dans le référentiel.
 .RE
 .P
 .B -c, check-updates
 .RS
-Vérifier si le fichier \fBChangeLog.txt\fP du SlackBuild contient des mises à jour.
+Vérifier s'il y a des nouvelles dans le fichier ChangeLog.txt du référentiel.
 .RE
 .P
 .B -I, repo-info
 .RS
-Afficher les informations relatives aux dépôts, telles que les dépôts actifs, la date de leur mise à jour et le nombre de paquets qu'ils contiennent.
+Affiche les informations relatives aux dépôts, telles que les dépôts actifs, la date de leur mise à jour, et le nombre de paquets qu'ils contiennent.
 .RE
 .P
 .B -L, clean-logs
 .RS
-Nettoyer les journaux de suivi de dépendances. \fBAttention\fP, après cette procédure vous devrez supprimer les dépendances à la main.
+Nettoie le suivi du journal des dépendances. Après cette procédure, vous devez supprimer les dépendances à la main.
 .RE
 .P
 .B -T, clean-data
 .RS
-Il est parfois nécessaire de nettoyer toutes les données des dépôts de la base de données.  Exécutez cette commande pour supprimer toutes les données et exécutez \fB'slpkg update'\fP pour les recréer.
+Il est parfois nécessaire de nettoyer toutes les données des référentiels de la base de données.
+Exécutez cette commande pour supprimer toutes les données et exécutez '\fIslpkg update\fR' pour les recréer.
 .RE
 .P
 .B -D, clean-tmp
 .RS
-Supprimer tous les scripts et sources des SlackBuilds téléchargés.
+Supprime tous les scripts et sources SlackBuilds téléchargés.
 .RE
 .P
 .B -g, configs
 .RS
-Modifier le fichier de configuration \fB/etc/slpkg/slpkg.toml\fP.
+Modifie le fichier de configuration /etc/slpkg/slpkg.toml.
 .RE
 .P
 .B -b, build
 .RS
-Construire les scripts des Slackbuilds et les ajouter au répertoire \fB/tmp\fP.
+Construit les scripts Slackbuilds et ajoute les paquets au répertoire '/tmp'.
 .RE
 .P
 .B -i, install
 .RS
-Construire et installer les paquets dans l'ordre adéquat et enregistre également les paquets avec les dépendances à utiliser pour la suppression.
+Construit et installe les paquets dans l'ordre correct, et enregistre également les paquets avec les dépendances pour les supprimer.
 .RE
 .P
 .B -d, download
 .RS
-Télécharger les scripts et les sources des SlackBuilds sans les construire ni les installer.
+Télécharge les scripts SlackBuilds actuels et les sources sans les construire ou les installer.
 .RE
 .P
 .B -R, remove
 .RS
-Supprimer les paquets avec leurs dépendances s'ils ont été installés avec la méthode \fB'slpkg install'\fP.
-Slpkg examine la configuration \fB'REPO_TAG'\fP pour trouver les paquets à supprimer.
+Supprime les paquets avec les dépendances si les paquets ont été installés avec la méthode '\fIslpkg install\fR'.
+Slpkg consulte la configuration 'REPO_TAG' pour trouver les paquets à supprimer par défaut, sauf si vous utilisez l'option \fB--file-pattern\fR.
 .RE
 .P
 .B -f, find
 .RS
-Trouver les paquets installés par \fBSBo\fP (taggés _SBo) sur votre distribution.
+Recherche les paquets installés sur votre système.
 .RE
 .P
 .B -w, view
 .RS
-Voir les paquets du dépôt et obtenir toutes les informations dans le terminal.
+Visualiser les paquets d'information du référentiel et tout obtenir dans votre terminal.
 .RE
 .P
 .B -s, search
 .RS
-Rechercher des paquets.
+Rechercher et faire correspondre les paquets
 .RE
 .P
 .B -e, dependees
 .RS
-Afficher les dépendances du paquet.
+Montrer de quels SlackBuilds dépendent.
 .RE
 .P
 .B -t, tracking
 .RS
-Suivre les dépendances des paquets.
+Suivi des dépendances des paquets.
 .RE
 .SH OPTIONS
 .P
 .B -y, --yes
 .RS
-Répondre \fBOui\fP à toutes les questions. (à utiliser avec: \fB-u, update, -U, upgrade, -L, clean-logs, -b, build,
--i, install, -R, remove, -d, download\fP)
+Répondre oui à toutes les questions. (à utiliser avec : -u, update, -U, upgrade, -b, build,
+-i, install, -R, remove, -d, download,)
 .RE
 .P
 .B -j, --jobs
 .RS
-Accélération des scripts SlackBuild. Lorsque l'indicateur \fB--jobs\fP est activé, slpkg détecte automatiquement le nombre de
-de processeurs et le saisit dans la variable \fBMAKEFLAGS\fP. Certains SlackBuilds échouent lorsque \fBMAKEFLAGS\fP est déclaré ou que
-le nombre de processeurs (-j) est supérieur à 1. (à utiliser avec: \fB-U, upgrade, build, -i, install\fP)
+Accélération des scripts SlackBuild. Lorsque l'option \fB--jobs\fR est activée, slpkg détecte automatiquement le nombre de processeurs et l'entre dans la variable MAKEFLAGS.
+Certains SlackBuilds échouent lorsque MAKEFLAGS est déclaré ou que le nombre de processeurs (-j) est supérieur à un. (à utiliser avec : -U, upgrade, -b, build, -i, install)
 .RE
 .P
-.B -o, --resolve-off
+.B -O, --resolve-off
 .RS
-Désactiver la résolution des dépendances. (à utiliser avec: \fB-U, upgrade, -b, build, -i, install\fP)
+Désactive la résolution des dépendances. (à utiliser avec : -U, upgrade, -b, build, -i, install)
 .RE
 .P
 .B -r, --reinstall
 .RS
-Utilisez cette option si vous voulez mettre à niveau tous les paquets même si la même version est déjà installée.
-Ne saute pas les paquets déjà installés. (à utiliser avec: \fB-U, upgrade, -i, install\fP)
+Utilisez cette option si vous souhaitez mettre à jour tous les paquets, même si la même version est déjà installée.
+Ne pas ignorer les paquets installés. (à utiliser avec : -U, upgrade, -i, install)
 .RE
 .P
 .B -k, --skip-installed
 .RS
-Utilisez cette option si vous voulez éviter de construire et de réinstaller des paquets.
-Remarque : Cette option n'affecte que les dépendances. (à utiliser avec: \fB-i, install\fP)
+Cette option est utile si vous souhaitez éviter de construire et de réinstaller des paquets.
+Remarque : cette option n'affecte que les dépendances. (à utiliser avec : -i, install)
+.RE
+.P
+.B -a, --install-data
+.RS
+Installe les données dans la base de données uniquement si vous ne souhaitez pas retélécharger ou resynchroniser les listes de paquets,
+et que vous avez déjà téléchargé le référentiel, vous pouvez appliquer cette option pour installer les données dans la base de données.
+Cette option est particulièrement utile pour les dépôts locaux et pour ceux qui téléchargent les dépôts manuellement.
+(à utiliser avec : -u, update)
 .RE
 .P
 .B -E, --full-reverse
 .RS
-Dépendances inverses complètes. Ne fonctionne qu'avec la commande \fB-e, dependees\fP et montre aussi les \fBRequires\fP.
-(à utiliser avec: -e, dependees)
+Dépendance inversée complète. Ne fonctionne qu'avec les commandes -e, dependees et affiche également les besoins.
+(à utiliser avec : -e, dependees)
 .RE
 .P
 .B -S, --search
 .RS
-Active l'utilitaire de dialogue pour rechercher des paquets dans le dépôt.
-Essayez par exemple : \fB`slpkg install python3 --search`\fP ou \fB`slpkg download python3 --search`\fP et ainsi de suite.
-(à utiliser avec: \fB-b, build, -i, install, -d, download, -R, remove, -f, find, -w, view,
--s, search, -e, dependees, -t, tracking\fP)
+Active l'utilitaire de dialogue pour rechercher des paquets dans le référentiel.
+Exemple : '\fIslpkg install python3 --search\fR' ou '\fIslpkg download python3 --search\fR', etc.
+(à utiliser avec : -b, build, -i, install, -d, download, -R, remove, -f, find, -w, view,
+-s, search, -e, dependees, -t, tracking)
 .RE
 .P
 .B -n, --no-silent
 .RS
-Désactiver le mode silencieux s'il est activé dans le fichier de configuration. (à utiliser avec: \fB-u, update, -U,upgrade, -b, build,
--i, install, -d, download, -R, remove\fP)
+Désactive le mode silencieux, s'il est activé dans le fichier de configuration. (à utiliser avec : -u, update, -U, upgrade, -b, build,
+-i, install, -R, remove)
 .RE
 .P
 .B -p, --pkg-version
 .RS
-Afficher la version du package du dépôt. (à utiliser avec: \fB-e, dependees, -t, tracking, -w, view\fP)
+Affiche la version du paquetage du référentiel. (à utiliser avec : -e, dependees, -t, tracking, -w, view)
 .RE
 .P
-.B -G, --generate-only
+.B -P, --parallèle
 .RS
-N'est utilisé qu'avec le dépôt ponce et lorsque vous souhaitez générer uniquement le fichier SLACKBUILDS.TXT
-et mettre à jour la base de données, sans re-télécharger l'ensemble du référentiel. (à utiliser avec : \fB-u, update\fP)
+Télécharger des fichiers en parallèle pour accélérer le processus.
+(à utiliser avec : -u, update, -U, upgrade, -b, build, -i, install, -d, download)
 .RE
 .P
-.B -P, --parallel
+.B -m, --no-case
 .RS
-Télécharger des fichiers en parallèle pour accélérer le processus.
-(à utiliser avec: \fB-u, update, -U, upgrade, -b, build, -i, install, -d, download\fP)
+Paquets de correspondance de motifs sensibles à la casse.
+(à utiliser avec : -b, build, -i, install, -d, download, -s, search, -f, find, -w, view, -t, tracking, -e, dependees)
 .RE
 .P
-.BI "-B," "" " \-\-bin-repo=[" REPO "]
+.BI "-o," "" " \-\--repository=" NAME "
 .RS
-Passer aux dépôts de binaires et sélectionner un dépôt.
-Exemple: '\fIslpkg -i audacity --bin=repo=alien\fR'.
-Les options update, check et search supportent l'astérisque '*' pour l'appliquer à tous les dépôts, comme rechercher un paquet dans tous les dépôts binaires 'slpkg -s libreoffice --bin-repo='*''.  (à utiliser avec : \fB-u, update, -c, check-updates, -U, upgrade, -i, install, -d, download, -s, search, -t, tracking, -e, dependees, -w, view\fP)
+Change le référentiel par défaut et définit le référentiel avec lequel vous voulez travailler.
+Assurez-vous d'avoir activé le référentiel dans le fichier '/etc/slpkg/repositories.toml'.
+Le modèle de référentiel '*' n'est supporté qu'avec l'option '-s, search'
+(à utiliser avec : -u, update, -U, upgrade, -c, check-updates, -I, repo-info, -b, build, -i, install, -d, download, -s, search,
+-t, tracking, -e, dependees, -w, view)
 .RE
 .P
-.B -z, --directory=[PATH]
+.BI "-z," "" " \-\-directory=" PATH "
 .RS
-Définir le répertoire où seront enregistrés les fichiers téléchargés. (à utiliser avec: \fB-d, download\fP)
+Le répertoire est le chemin où les fichiers seront enregistrés. (à utiliser avec : -d, download)
 .RE
 .P
 .B -h | --help
 .RS
-Afficher l'aide.
+Affiche les informations d'aide et quitte.
 .RE
 .P
 .B -v | --version
 .RS
-Afficher la version.
+Affiche la version et quitte.
 .RE
-.SH OPTION SYNTAX
+.SH SYNTAXE DES OPTIONS
 .P
-En plus de la façon classique, vous pouvez mettre ensemble plusieurs options qui ne nécessitent pas d'arguments, comme par exemple :
+En dehors de la manière classique, vous pouvez mettre plusieurs options qui ne nécessitent pas d'arguments ensemble, comme :
 .PP
 .Vb 1.
 \&       slpkg -iPny [\fIPACKAGES...\fR]
 .Ve
 .RE
 .SH FILELIST|PACKAGES
 .P
-Au lieu de paquets, vous pouvez passer un fichier texte avec le suffixe '.pkgs' et les noms des paquets.  Exemple : 'slpkg install list.pkgs'.
-Éditer la configuration '/etc/slpkg/slpkg.toml' pour changer le suffixe si vous le souhaitez. Vous pouvez utiliser des listes provenant d'autres sources, avec des fichiers '.sqf'.
+Au lieu de paquets, vous pouvez transmettre un fichier texte avec le suffixe '.pkgs' et les noms des paquets. 
+Exemple : '\fIslpkg install list.pkgs\fR'. 
+Editez le fichier de configuration '/etc/slpkg/slpkg.toml' pour changer le suffixe si vous le souhaitez. 
+Vous pouvez utiliser des listes provenant d'autres sources, comme les fichiers '.sqf'. 
 .RE
 .SH A SAVOIR
 .P
 Il y a cinq indicateurs lorsque certaines commandes sont utilisées, par exemple :
 
-Cyan : Installer, Jaune : Pour construire, Gris : C'est installé, Violet : Pour la mise à jour, Rouge : Pour supprimer.
+Cyan : Installer, Jaune : Construire, Gris : Installé, Violet : Installé Pour construire, Gris : C'est installé, Violet : Pour la mise à jour, Rouge : Pour supprimer.
 
-Lorsque vous utilisez les commandes install, build, upgrade ou remove, vous devez savoir que si le paquet est installé, 
-sa couleur passera au gris, si le paquet peut être mis à niveau, il devient violet. Et s'il n'est pas installé alors 
-sa couleur sera cyan. De même, si vous essayez de supprimer un paquet, la couleur du paquet devient rouge.
+Lorsque vous utilisez les commandes install, build, upgrade ou remove, vous devez savoir que si le paquet est installé, sa couleur passera au gris, 
+si le paquet peut être mis à jour, il devient violet, et s'il n'est pas installé, sa couleur est cyan.
+De même, si vous essayez de supprimer un paquet, la couleur du paquet devient rouge.
 
 Exemple : Si le paquet est déjà installé, que la couleur de l'indicateur est grise et que l'option '\fB-r, --reinstall\fR' n'est pas appliquée,
-le paquetage ne sera pas installé et le message "(already installed)" s'affichera.
-Si le paquet peut être mis à niveau, l'installation se poursuivra et le paquet passera à la mise à niveau.
+le paquet ne sera pas installé et le message "(déjà installé)" s'affichera.
+Si le paquet peut être mis à jour, l'installation se poursuivra et le paquet sera mis à jour.
 
-Pour la commande de mise à niveau, vous devez savoir que vous pouvez mettre à niveau des paquets provenant de différents dépôts, si vous éditez
+Pour la commande de mise à jour, vous devez savoir que vous pouvez mettre à jour des paquets provenant de différents dépôts, si vous éditez
 le fichier '\fI/etc/slpkg/repositories.toml\fR' et supprimez la balise repository. Le slpkg ne peut alors pas reconnaître le dépôt des paquets.
 
 Avec la commande remove, il va supprimer les dépendances si le paquet a été installé avec la commande '\fIslpkg install\fR',
 sinon, le slpkg ne connaît pas les dépendances qui sont installées avec les paquets qu'il va supprimer.
 
 Vous pouvez appliquer l'astérisque '*' à la place d'un paquet, pour faire correspondre tous les paquets d'un dépôt. Vous ne pouvez pas appliquer
-un astérisque à l'option '\fB-B, --bin-repos=\fR', sauf pour les commandes '\fB-s, search\fR', '\fB-u, update\fR' et '\fB-c, check-updates\fR'.
+un astérisque à l'option '\fB-o, --repository=\fR', sauf pour la commande '\fB-s, search\fR'.
 
-La commande clean-data supprime les données du référentiel local et de la base de données.
-
-Remarque : il n'existe actuellement aucune fonction permettant d'indiquer les paquets si les couleurs sont désactivées.
+Note : Il n'existe actuellement aucune fonction permettant d'indiquer les paquets si les couleurs sont désactivées.
+.RE
+.SH ÉTAT DE SORTIE
+.P
+0 Exécution réussie de slpkg.
+.P
+1 Une erreur s'est produite.
+.P
+20 Aucun paquetage n'a été trouvé pour être téléchargé, installé, réinstallé, mis à jour ou supprimé.
+.RE
+.SH CARACTÈRES D'EXPLICATION
+.P
+[État du traitement : Rouge est en cours de traitement, Vert est terminé.
+.P
+[✔️] Caractère terminé : Apparaît lorsque le traitement est terminé.
+.P
+[X] Caractère d'échec : Apparaît lorsque le traitement a échoué.
+.P
+[Caractère ignoré : Apparaît lorsque le traitement a été ignoré.
+.P
 .RE
 .SH FICHIERS DE CONFIGURATION
 .P
-Fichier de \fBconfiguration\fP : /etc/slpkg/slpkg.toml
+Fichier de configuration dans le fichier /etc/slpkg/slpkg.toml.
 .P
-Fichier des \fBdépôts\fP : /etc/slpkg/repositories.toml
+Fichier de référentiels dans le fichier /etc/slpkg/repositories.toml.
 .P
-Fichier \fBblacklist\fP : /etc/slpkg/blacklist.toml
+Fichier de liste noire dans le fichier /etc/slpkg/blacklist.toml.
 .P
-\fIslpkg_new-configs\fR permet de gérer les fichiers de configuration \fB.new\fP facilement et rapidement. Déplacez, copiez ou supprimez-les.
+Fichier de règles dans le fichier /etc/slpkg/rules.toml.
+.P
+\fIslpkg_new-configs\fR permet de gérer les fichiers de configuration .new facilement et rapidement. Déplacez-les, copiez-les ou supprimez-les.
 .RE
 .SH RAPPORT DE BOGUES
 .P
-Veuillez signaler tout bogue trouvé à \fBhttps://gitlab.com/dslackw/slpkg/-/issues\fP.
+Veuillez rapporter tout bug trouvé à : https://gitlab.com/dslackw/slpkg/-/issues.
+.P
+Note : Avec le problème, veuillez référencer le fichier journal que vous trouverez dans le chemin /tmp/slpkg/logs/slpkg.log et le coller également.
 .SH AUTEUR
 .P
-\fBDimitris Zlatanidis\fP <dslackw@gmail.com>
+Dimitris Zlatanidis <dslackw@gmail.com>
```

### Comparing `slpkg-4.8.7/completion/slpkg` & `slpkg-4.8.8/completion/slpkg`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/dialog_configs.py` & `slpkg-4.8.8/slpkg/dialog_configs.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/binaries/required.py` & `slpkg-4.8.8/slpkg/binaries/required.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/binaries/queries.py` & `slpkg-4.8.8/slpkg/binaries/queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/binaries/install.py` & `slpkg-4.8.8/slpkg/binaries/install.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,16 +108,17 @@
         packages: dict = {}
 
         for pkg in self.install_order:
             if self.continue_to_install(pkg):
                 package: str = self.data[pkg]['package']
                 mirror: str = self.data[pkg]['mirror']
                 location: str = self.data[pkg]['location']
+                url: list = [f'{mirror}{location}/{package}']
 
-                packages[f'{mirror}{location}/{package}'] = self.tmp_slpkg
+                packages[pkg] = (url, self.tmp_slpkg)
 
                 self.binary_packages.append(package)
                 self.utils.remove_file_if_exists(self.tmp_slpkg, package)
             else:
                 installed_package: str = self.utils.is_package_installed(pkg)
                 self.view_message.view_skipping_packages(installed_package)
 
@@ -155,15 +156,15 @@
             command: str = f'{self.slackware_command} {self.tmp_slpkg}/{package}'
             self.multi_proc.process(command, package, self.progress_message)
 
             if not self.option_for_resolve_off:
                 name: str = self.utils.split_package(Path(package).stem)['name']
                 self.logs_deps.logging(name)
 
-    def set_progress_message(self):
+    def set_progress_message(self) -> None:
         if self.mode == 'upgrade' or self.option_for_reinstall:
             self.progress_message: str = f'{self.cyan}Upgrading{self.endc}'
 
     def set_slackware_command(self) -> None:
         if self.mode == 'upgrade' or self.option_for_reinstall:
             self.slackware_command: str = self.reinstall
 
@@ -183,13 +184,16 @@
 
                 if installed:
                     status: bool = False
 
                 if self.option_for_reinstall:
                     status: bool = True
 
+                if self.mode == 'upgrade':
+                    status: bool = True
+
                 choices.extend([(package, repo_ver, status, help_text)])
 
             text: str = f'There are {len(choices)} dependencies:'
             code, self.dependencies = self.dialogbox.checklist(text, title, height, width, list_height, choices)
 
             os.system('clear')
```

### Comparing `slpkg-4.8.7/slpkg/install_data.py` & `slpkg-4.8.8/slpkg/install_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         """ Reads the first date of the changelog file."""
         lines: list = self.utils.read_text_file(changelog_file)
         days = ('Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun')
         for line in lines:
             if line.startswith(days):
                 return line.replace('\n', '')
 
-    def view_done_message(self):
+    def view_done_message(self) -> None:
         print(f'{self.yellow}{self.ascii.done}{self.endc}\n')
 
     def install_sbo_data(self) -> None:
         """ Install the data for SBo repository. """
         sbo_tags = [
             'SLACKBUILD NAME:',
             'SLACKBUILD LOCATION:',
```

### Comparing `slpkg-4.8.7/slpkg/repositories.py` & `slpkg-4.8.8/slpkg/repositories.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/repo_info.py` & `slpkg-4.8.8/slpkg/repo_info.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/sbos/queries.py` & `slpkg-4.8.8/slpkg/sbos/queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/sbos/slackbuild.py` & `slpkg-4.8.8/slpkg/sbos/slackbuild.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,19 +159,19 @@
                 # Copy slackbuilds to the build folder.
                 path_repo_package: Path = Path(self.repos.repositories[self.repository]['path'], location, sbo)
                 shutil.copytree(path_repo_package, build_path)
 
                 os.chmod(slackbuild, 0o775)
 
                 if self.os_arch == 'x86_64' and self.data[sbo]['download64']:
-                    sources: list = self.data[sbo]['download64'].split()
+                    sources: tuple = self.data[sbo]['download64'].split()
                 else:
-                    sources: list = self.data[sbo]['download'].split()
-                for source in sources:
-                    self.sources[source] = Path(self.build_path, sbo)
+                    sources: tuple = self.data[sbo]['download'].split()
+
+                self.sources[sbo] = (sources, Path(self.build_path, sbo))
 
     def download_the_sources(self) -> None:
         if self.sources:
             print(f'Started to download total ({self.cyan}{len(self.sources)}{self.endc}) sources:\n')
             self.download.download(self.sources)
             print()
 
@@ -241,15 +241,15 @@
         folder: Path = Path(path, name)
         filename: str = f'{name}.SlackBuild'
         command: str = f'{folder}/./{filename}'
         self.utils.change_owner_privileges(folder)
         progress_message: str = f'{self.red}Building{self.endc}'
         self.multi_proc.process(command, filename, progress_message)
 
-    def set_progress_message(self):
+    def set_progress_message(self) -> None:
         if self.mode == 'upgrade' or self.option_for_reinstall:
             self.progress_message: str = f'{self.cyan}Upgrading{self.endc}'
 
     def set_slackware_command(self) -> None:
         if self.mode == 'upgrade' or self.option_for_reinstall:
             self.slackware_command: str = self.reinstall
 
@@ -274,14 +274,17 @@
 
                 if installed:
                     status: bool = False
 
                 if self.option_for_reinstall:
                     status: bool = True
 
+                if self.mode == 'upgrade':
+                    status: bool = True
+
                 choices.extend(
                     [(package, repo_ver, status, help_text)]
                 )
             text: str = f'There are {len(choices)} dependencies:'
 
             code, self.dependencies = self.dialogbox.checklist(text, title, height, width, list_height, choices)
```

### Comparing `slpkg-4.8.7/slpkg/sbos/dependencies.py` & `slpkg-4.8.8/slpkg/sbos/dependencies.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/sbos/sbo_generate.py` & `slpkg-4.8.8/slpkg/sbos/sbo_generate.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/update_repository.py` & `slpkg-4.8.8/slpkg/update_repository.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,15 +89,15 @@
                     repositories[repo]()
         print()
 
     def view_downloading_message(self, repo: str) -> None:
         print(f"Downloading the '{self.green}{repo}{self.endc}' repository "
               f"in the '{self.repos.repositories[repo]['path']}' folder, please wait...\n")
 
-    def slack_repository(self):
+    def slack_repository(self) -> None:
         if not self.option_for_install_data:
             urls: dict = {}
             self.utils.create_directory(self.repos.slack_repo_path)
 
             self.utils.remove_file_if_exists(self.repos.slack_repo_path, self.repos.slack_repo_packages)
             self.utils.remove_file_if_exists(self.repos.slack_repo_path, self.repos.slack_repo_changelog)
             self.utils.remove_file_if_exists(self.repos.slack_repo_path, self.repos.slack_repo_checksums)
@@ -109,118 +109,115 @@
                 )
                 self.utils.process(lftp_command)
             else:
                 changelog: str = f'{self.repos.slack_repo_mirror[0]}{self.repos.slack_repo_changelog}'
                 packages: str = f'{self.repos.slack_repo_mirror[0]}{self.repos.slack_repo_packages}'
                 checksums: str = f'{self.repos.slack_repo_mirror[0]}{self.repos.slack_repo_checksums}'
 
-                urls[changelog] = self.repos.slack_repo_path
-                urls[packages] = self.repos.slack_repo_path
-                urls[checksums] = self.repos.slack_repo_path
+                urls[self.repos.slack_repo_name] = ((changelog, packages, checksums), self.repos.slack_repo_path)
 
                 self.download.download(urls)
                 print()
 
         self.delete_bin_database_data(self.repos.slack_repo_name)
         self.delete_last_updated(self.repos.slack_repo_name)
         self.data.install_slack_data()
 
-    def slack_extra_repository(self):
+    def slack_extra_repository(self) -> None:
         if not self.option_for_install_data:
             urls: dict = {}
             self.utils.create_directory(self.repos.slack_extra_repo_path)
 
             self.utils.remove_file_if_exists(self.repos.slack_extra_repo_path, self.repos.slack_extra_repo_changelog)
             self.utils.remove_file_if_exists(self.repos.slack_extra_repo_path, self.repos.slack_extra_repo_packages)
             self.utils.remove_file_if_exists(self.repos.slack_extra_repo_path, self.repos.slack_extra_repo_checksums)
 
             changelog: str = f'{self.repos.slack_extra_repo_mirror[0]}{self.repos.slack_extra_repo_changelog}'
-            urls[changelog] = self.repos.slack_extra_repo_path
 
             if self.repos.slack_extra_repo_local[0].startswith('file'):
+                urls[self.repos.slack_extra_repo_name] = ((changelog,), self.repos.slack_extra_repo_path)
                 lftp_command: str = (
                     f'lftp {self.lftp_mirror_options} {"".join(self.repos.slack_extra_repo_mirror)} '
                     f'{self.repos.slack_extra_repo_path}'
                 )
                 self.utils.process(lftp_command)
             else:
                 packages: str = f'{"".join(self.repos.slack_extra_repo_mirror)}{self.repos.slack_extra_repo_packages}'
                 checksums: str = f'{"".join(self.repos.slack_extra_repo_mirror)}{self.repos.slack_extra_repo_checksums}'
-
-                urls[packages] = self.repos.slack_extra_repo_path
-                urls[checksums] = self.repos.slack_extra_repo_path
+                urls[self.repos.slack_extra_repo_name] = ((changelog, packages, checksums),
+                                                          self.repos.slack_extra_repo_path)
 
             self.download.download(urls)
             print()
 
         self.delete_bin_database_data(self.repos.slack_extra_repo_name)
         self.delete_last_updated(self.repos.slack_extra_repo_name)
         self.data.install_slack_extra_data()
 
-    def slack_patches_repository(self):
+    def slack_patches_repository(self) -> None:
         if not self.option_for_install_data:
             urls: dict = {}
             self.utils.create_directory(self.repos.slack_patches_repo_path)
 
             self.utils.remove_file_if_exists(self.repos.slack_patches_repo_path,
                                              self.repos.slack_patches_repo_changelog)
             self.utils.remove_file_if_exists(self.repos.slack_patches_repo_path,
                                              self.repos.slack_patches_repo_packages)
             self.utils.remove_file_if_exists(self.repos.slack_patches_repo_path,
                                              self.repos.slack_patches_repo_checksums)
 
             changelog: str = f'{self.repos.slack_patches_repo_mirror[0]}{self.repos.slack_patches_repo_changelog}'
-            urls[changelog] = self.repos.slack_patches_repo_path
 
             if self.repos.slack_patches_repo_local[0].startswith('file'):
+                urls[self.repos.slack_patches_repo_name] = ((changelog,), self.repos.slack_patches_repo_path)
                 lftp_command: str = (
                     f'lftp {self.lftp_mirror_options} {"".join(self.repos.slack_patches_repo_mirror)} '
                     f'{self.repos.slack_patches_repo_path}'
                 )
                 self.utils.process(lftp_command)
             else:
                 packages: str = (f'{"".join(self.repos.slack_patches_repo_mirror)}'
                                  f'{self.repos.slack_patches_repo_packages}')
                 checksums: str = (f'{"".join(self.repos.slack_patches_repo_mirror)}'
                                   f'{self.repos.slack_patches_repo_checksums}')
 
-                urls[packages] = self.repos.slack_patches_repo_path
-                urls[checksums] = self.repos.slack_patches_repo_path
+                urls[self.repos.slack_patches_repo_name] = ((changelog, packages, checksums),
+                                                            self.repos.slack_patches_repo_path)
 
             self.download.download(urls)
             print()
 
         self.delete_bin_database_data(self.repos.slack_patches_repo_name)
         self.delete_last_updated(self.repos.slack_patches_repo_name)
         self.data.install_slack_patches_data()
 
-    def alien_repository(self):
+    def alien_repository(self) -> None:
         if not self.option_for_install_data:
             urls: dict = {}
             self.utils.create_directory(self.repos.alien_repo_path)
 
             self.utils.remove_file_if_exists(self.repos.alien_repo_path, self.repos.alien_repo_changelog)
             self.utils.remove_file_if_exists(self.repos.alien_repo_path, self.repos.alien_repo_packages)
             self.utils.remove_file_if_exists(self.repos.alien_repo_path, self.repos.alien_repo_checksums)
 
             changelog: str = f'{self.repos.alien_repo_mirror[0]}{self.repos.alien_repo_changelog}'
-            urls[changelog] = self.repos.alien_repo_path
 
             if self.repos.alien_repo_local[0].startswith('file'):
+                urls[self.repos.alien_repo_name] = ((changelog,), self.repos.alien_repo_path)
                 lftp_command: str = (
                     f'lftp {self.lftp_mirror_options} {"".join(self.repos.alien_repo_mirror)} '
                     f'{self.repos.alien_repo_path}'
                 )
                 self.utils.process(lftp_command)
             else:
                 packages: str = f'{"".join(self.repos.alien_repo_mirror)}{self.repos.alien_repo_packages}'
                 checksums: str = f'{"".join(self.repos.alien_repo_mirror)}{self.repos.alien_repo_checksums}'
 
-                urls[packages] = self.repos.alien_repo_path
-                urls[checksums] = self.repos.alien_repo_path
+                urls[self.repos.alien_repo_name] = ((changelog, packages, checksums),
+                                                    self.repos.alien_repo_path)
 
             self.download.download(urls)
             print()
 
         self.delete_bin_database_data(self.repos.alien_repo_name)
         self.delete_last_updated(self.repos.alien_repo_name)
         self.data.install_alien_data()
@@ -231,28 +228,28 @@
             self.utils.create_directory(self.repos.multilib_repo_path)
 
             self.utils.remove_file_if_exists(self.repos.multilib_repo_path, self.repos.multilib_repo_changelog)
             self.utils.remove_file_if_exists(self.repos.multilib_repo_path, self.repos.multilib_repo_packages)
             self.utils.remove_file_if_exists(self.repos.multilib_repo_path, self.repos.multilib_repo_checksums)
 
             changelog: str = f'{self.repos.multilib_repo_mirror[0]}{self.repos.multilib_repo_changelog}'
-            urls[changelog] = self.repos.multilib_repo_path
 
             if self.repos.multilib_repo_local[0].startswith('file'):
+                urls[self.repos.multilib_repo_name] = ((changelog,), self.repos.multilib_repo_path)
                 lftp_command: str = (
                     f'lftp {self.lftp_mirror_options} {"".join(self.repos.multilib_repo_mirror)} '
                     f'{self.repos.multilib_repo_path}'
                 )
                 self.utils.process(lftp_command)
             else:
                 packages: str = f'{"".join(self.repos.multilib_repo_mirror)}{self.repos.multilib_repo_packages}'
                 checksums: str = f'{"".join(self.repos.multilib_repo_mirror)}{self.repos.multilib_repo_checksums}'
 
-                urls[packages] = self.repos.multilib_repo_path
-                urls[checksums] = self.repos.multilib_repo_path
+                urls[self.repos.multilib_repo_name] = ((changelog, packages, checksums),
+                                                       self.repos.multilib_repo_path)
 
             self.download.download(urls)
             print()
 
         self.delete_bin_database_data(self.repos.multilib_repo_name)
         self.delete_last_updated(self.repos.multilib_repo_name)
         self.data.install_multilib_data()
@@ -263,28 +260,28 @@
             self.utils.create_directory(self.repos.restricted_repo_path)
 
             self.utils.remove_file_if_exists(self.repos.restricted_repo_path, self.repos.restricted_repo_changelog)
             self.utils.remove_file_if_exists(self.repos.restricted_repo_path, self.repos.restricted_repo_packages)
             self.utils.remove_file_if_exists(self.repos.restricted_repo_path, self.repos.restricted_repo_checksums)
 
             changelog: str = f'{self.repos.restricted_repo_mirror[0]}{self.repos.restricted_repo_changelog}'
-            urls[changelog] = self.repos.restricted_repo_path
 
             if self.repos.restricted_repo_local[0].startswith('file'):
+                urls[self.repos.restricted_repo_name] = ((changelog,), self.repos.restricted_repo_path)
                 lftp_command: str = (
                     f'lftp {self.lftp_mirror_options} {"".join(self.repos.restricted_repo_mirror)} '
                     f'{self.repos.restricted_repo_path}'
                 )
                 self.utils.process(lftp_command)
             else:
                 packages: str = f'{"".join(self.repos.restricted_repo_mirror)}{self.repos.restricted_repo_packages}'
                 checksums: str = f'{"".join(self.repos.restricted_repo_mirror)}{self.repos.restricted_repo_checksums}'
 
-                urls[packages] = self.repos.restricted_repo_path
-                urls[checksums] = self.repos.restricted_repo_path
+                urls[self.repos.restricted_repo_name] = ((changelog, packages, checksums),
+                                                         self.repos.restricted_repo_path)
 
             self.download.download(urls)
             print()
 
         self.delete_bin_database_data(self.repos.restricted_repo_name)
         self.delete_last_updated(self.repos.restricted_repo_name)
         self.data.install_restricted_data()
@@ -305,17 +302,15 @@
                 )
                 self.utils.process(lftp_command)
             else:
                 changelog: str = f'{self.repos.gnome_repo_mirror[0]}{self.repos.gnome_repo_changelog}'
                 packages: str = f'{self.repos.gnome_repo_mirror[0]}{self.repos.gnome_repo_packages}'
                 checksums: str = f'{self.repos.gnome_repo_mirror[0]}{self.repos.gnome_repo_checksums}'
 
-                urls[changelog] = self.repos.gnome_repo_path
-                urls[packages] = self.repos.gnome_repo_path
-                urls[checksums] = self.repos.gnome_repo_path
+                urls[self.repos.gnome_repo_name] = ((changelog, packages, checksums), self.repos.gnome_repo_path)
 
                 self.download.download(urls)
                 print()
 
         self.delete_bin_database_data(self.repos.gnome_repo_name)
         self.delete_last_updated(self.repos.gnome_repo_name)
         self.data.install_gnome_data()
@@ -326,28 +321,27 @@
             self.utils.create_directory(self.repos.msb_repo_path)
 
             self.utils.remove_file_if_exists(self.repos.msb_repo_path, self.repos.msb_repo_changelog)
             self.utils.remove_file_if_exists(self.repos.msb_repo_path, self.repos.msb_repo_packages)
             self.utils.remove_file_if_exists(self.repos.msb_repo_path, self.repos.msb_repo_checksums)
 
             changelog: str = f'{self.repos.msb_repo_mirror[0]}{self.repos.msb_repo_changelog}'
-            urls[changelog] = self.repos.msb_repo_path
 
             if self.repos.msb_repo_local[0].startswith('file'):
+                urls[self.repos.msb_repo_name] = ((changelog,), self.repos.msb_repo_path)
                 lftp_command: str = (
                     f'lftp {self.lftp_mirror_options} {"".join(self.repos.msb_repo_mirror)} '
                     f'{self.repos.msb_repo_path}'
                 )
                 self.utils.process(lftp_command)
             else:
                 packages: str = f'{"".join(self.repos.msb_repo_mirror)}{self.repos.msb_repo_packages}'
                 checksums: str = f'{"".join(self.repos.msb_repo_mirror)}{self.repos.msb_repo_checksums}'
 
-                urls[packages] = self.repos.msb_repo_path
-                urls[checksums] = self.repos.msb_repo_path
+                urls[self.repos.msb_repo_name] = ((changelog, packages, checksums), self.repos.msb_repo_path)
 
             self.download.download(urls)
             print()
 
         self.delete_bin_database_data(self.repos.msb_repo_name)
         self.delete_last_updated(self.repos.msb_repo_name)
         self.data.install_msb_data()
@@ -368,17 +362,15 @@
                 )
                 self.utils.process(lftp_command)
             else:
                 changelog: str = f'{"".join(self.repos.csb_repo_mirror)}{self.repos.csb_repo_changelog}'
                 packages: str = f'{"".join(self.repos.csb_repo_mirror)}{self.repos.csb_repo_packages}'
                 checksums: str = f'{"".join(self.repos.csb_repo_mirror)}{self.repos.csb_repo_checksums}'
 
-                urls[changelog] = self.repos.csb_repo_path
-                urls[packages] = self.repos.csb_repo_path
-                urls[checksums] = self.repos.csb_repo_path
+                urls[self.repos.csb_repo_name] = ((changelog, packages, checksums), self.repos.csb_repo_path)
 
                 self.download.download(urls)
                 print()
 
         self.delete_bin_database_data(self.repos.csb_repo_name)
         self.delete_last_updated(self.repos.csb_repo_name)
         self.data.install_csb_data()
@@ -399,17 +391,15 @@
                 )
                 self.utils.process(lftp_command)
             else:
                 changelog: str = f'{self.repos.conraid_repo_mirror[0]}{self.repos.conraid_repo_changelog}'
                 packages: str = f'{self.repos.conraid_repo_mirror[0]}{self.repos.conraid_repo_packages}'
                 checksums: str = f'{self.repos.conraid_repo_mirror[0]}{self.repos.conraid_repo_checksums}'
 
-                urls[changelog] = self.repos.conraid_repo_path
-                urls[packages] = self.repos.conraid_repo_path
-                urls[checksums] = self.repos.conraid_repo_path
+                urls[self.repos.conraid_repo_name] = ((changelog, packages, checksums), self.repos.conraid_repo_path)
 
                 self.download.download(urls)
                 print()
 
         self.delete_bin_database_data(self.repos.conraid_repo_name)
         self.delete_last_updated(self.repos.conraid_repo_name)
         self.data.install_conraid_data()
@@ -430,17 +420,16 @@
                 )
                 self.utils.process(lftp_command)
             else:
                 changelog: str = f'{self.repos.slackonly_repo_mirror[0]}{self.repos.slackonly_repo_changelog}'
                 packages: str = f'{self.repos.slackonly_repo_mirror[0]}{self.repos.slackonly_repo_packages}'
                 checksums: str = f'{self.repos.slackonly_repo_mirror[0]}{self.repos.slackonly_repo_checksums}'
 
-                urls[changelog] = self.repos.slackonly_repo_path
-                urls[packages] = self.repos.slackonly_repo_path
-                urls[checksums] = self.repos.slackonly_repo_path
+                urls[self.repos.slackonly_repo_name] = ((changelog, packages, checksums),
+                                                        self.repos.slackonly_repo_path)
 
                 self.download.download(urls)
                 print()
 
         self.delete_bin_database_data(self.repos.slackonly_repo_name)
         self.delete_last_updated(self.repos.slackonly_repo_name)
         self.data.install_slackonly_data()
@@ -461,17 +450,15 @@
                 )
                 self.utils.process(lftp_command)
             else:
                 changelog: str = f'{self.repos.salixos_repo_mirror[0]}{self.repos.salixos_repo_changelog}'
                 packages: str = f'{self.repos.salixos_repo_mirror[0]}{self.repos.salixos_repo_packages}'
                 checksums: str = f'{self.repos.salixos_repo_mirror[0]}{self.repos.salixos_repo_checksums}'
 
-                urls[changelog] = self.repos.salixos_repo_path
-                urls[packages] = self.repos.salixos_repo_path
-                urls[checksums] = self.repos.salixos_repo_path
+                urls[self.repos.salixos_repo_name] = ((changelog, packages, checksums), self.repos.salixos_repo_path)
 
                 self.download.download(urls)
                 print()
 
         self.delete_bin_database_data(self.repos.salixos_repo_name)
         self.delete_last_updated(self.repos.salixos_repo_name)
         self.data.install_salixos_data()
@@ -485,30 +472,30 @@
                                              self.repos.salixos_extra_repo_changelog)
             self.utils.remove_file_if_exists(self.repos.salixos_extra_repo_path,
                                              self.repos.salixos_extra_repo_packages)
             self.utils.remove_file_if_exists(self.repos.salixos_extra_repo_path,
                                              self.repos.salixos_extra_repo_checksums)
 
             changelog: str = f'{self.repos.salixos_extra_repo_mirror[0]}{self.repos.salixos_extra_repo_changelog}'
-            urls[changelog] = self.repos.salixos_extra_repo_path
 
             if self.repos.salixos_extra_repo_local[0].startswith('file'):
+                urls[self.repos.salixos_extra_repo_name] = ((changelog,), self.repos.salixos_extra_repo_path)
                 lftp_command: str = (
                     f'lftp {self.lftp_mirror_options} {"".join(self.repos.salixos_extra_repo_mirror)} '
                     f'{self.repos.salixos_extra_repo_path}'
                 )
                 self.utils.process(lftp_command)
             else:
                 packages: str = f'{"".join(self.repos.salixos_extra_repo_mirror)}' \
                                 f'{self.repos.salixos_extra_repo_packages}'
                 checksums: str = (f'{"".join(self.repos.salixos_extra_repo_mirror)}'
                                   f'{self.repos.salixos_extra_repo_checksums}')
 
-                urls[packages] = self.repos.salixos_extra_repo_path
-                urls[checksums] = self.repos.salixos_extra_repo_path
+                urls[self.repos.salixos_extra_repo_name] = ((changelog, packages, checksums),
+                                                            self.repos.salixos_extra_repo_path)
 
             self.download.download(urls)
             print()
 
         self.delete_bin_database_data(self.repos.salixos_extra_repo_name)
         self.delete_last_updated(self.repos.salixos_extra_repo_name)
         self.data.install_salixos_extra_data()
@@ -522,30 +509,30 @@
                                              self.repos.salixos_patches_repo_changelog)
             self.utils.remove_file_if_exists(self.repos.salixos_patches_repo_path,
                                              self.repos.salixos_patches_repo_packages)
             self.utils.remove_file_if_exists(self.repos.salixos_patches_repo_path,
                                              self.repos.salixos_patches_repo_checksums)
 
             changelog: str = f'{self.repos.salixos_patches_repo_mirror[0]}{self.repos.salixos_patches_repo_changelog}'
-            urls[changelog] = self.repos.salixos_patches_repo_path
 
             if self.repos.salixos_patches_repo_local[0].startswith('file'):
+                urls[self.repos.salixos_patches_repo_name] = ((changelog,), self.repos.salixos_patches_repo_path)
                 lftp_command: str = (
                     f'lftp {self.lftp_mirror_options} {"".join(self.repos.salixos_patches_repo_mirror)} '
                     f'{self.repos.salixos_patches_repo_path}'
                 )
                 self.utils.process(lftp_command)
             else:
                 packages: str = (f'{"".join(self.repos.salixos_patches_repo_mirror)}'
                                  f'{self.repos.salixos_patches_repo_packages}')
                 checksums: str = (f'{"".join(self.repos.salixos_patches_repo_mirror)}'
                                   f'{self.repos.salixos_patches_repo_checksums}')
 
-                urls[packages] = self.repos.salixos_patches_repo_path
-                urls[checksums] = self.repos.salixos_patches_repo_path
+                urls[self.repos.salixos_patches_repo_name] = ((changelog, packages, checksums),
+                                                              self.repos.salixos_patches_repo_path)
 
             self.download.download(urls)
             print()
 
         self.delete_bin_database_data(self.repos.salixos_patches_repo_name)
         self.delete_last_updated(self.repos.salixos_patches_repo_name)
         self.data.install_salixos_patches_data()
@@ -566,17 +553,15 @@
                 )
                 self.utils.process(lftp_command)
             else:
                 changelog: str = f'{self.repos.slackel_repo_mirror[0]}{self.repos.slackel_repo_changelog}'
                 packages: str = f'{self.repos.slackel_repo_mirror[0]}{self.repos.slackel_repo_packages}'
                 checksums: str = f'{self.repos.slackel_repo_mirror[0]}{self.repos.slackel_repo_checksums}'
 
-                urls[changelog] = self.repos.slackel_repo_path
-                urls[packages] = self.repos.slackel_repo_path
-                urls[checksums] = self.repos.slackel_repo_path
+                urls[self.repos.slackel_repo_name] = ((changelog, packages, checksums), self.repos.slackel_repo_path)
 
                 self.download.download(urls)
                 print()
 
         self.delete_bin_database_data(self.repos.slackel_repo_name)
         self.delete_last_updated(self.repos.slackel_repo_name)
         self.data.install_slackel_data()
@@ -597,17 +582,15 @@
                 )
                 self.utils.process(lftp_command)
             else:
                 changelog: str = f'{self.repos.slint_repo_mirror[0]}{self.repos.slint_repo_changelog}'
                 packages: str = f'{self.repos.slint_repo_mirror[0]}{self.repos.slint_repo_packages}'
                 checksums: str = f'{self.repos.slint_repo_mirror[0]}{self.repos.slint_repo_checksums}'
 
-                urls[changelog] = self.repos.slint_repo_path
-                urls[packages] = self.repos.slint_repo_path
-                urls[checksums] = self.repos.slint_repo_path
+                urls[self.repos.slint_repo_name] = ((changelog, packages, checksums), self.repos.slint_repo_path)
 
                 self.download.download(urls)
                 print()
 
         self.delete_bin_database_data(self.repos.slint_repo_name)
         self.delete_last_updated(self.repos.slint_repo_name)
         self.data.install_slint_data()
```

### Comparing `slpkg-4.8.7/slpkg/progress_bar.py` & `slpkg-4.8.8/slpkg/progress_bar.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/downloader.py` & `slpkg-4.8.8/slpkg/downloader.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,26 +29,35 @@
             'lftp': self.lftp_downloader
         }
         self.option_for_parallel: bool = self.utils.is_option(
             ('-P', '--parallel'), flags)
 
     def download(self, sources: dict) -> None:
         """ Starting the processing for downloading. """
-        processes: list = []
-
         if self.parallel_downloads or self.option_for_parallel:
-            for url, path in sources.items():
+            self.parallel_download(sources)
+        else:
+            self.normal_download(sources)
+
+    def parallel_download(self, sources: dict) -> None:
+        """ Download sources with parallel mode. """
+        processes: list = []
+        for urls, path in sources.values():
+            for url in urls:
                 proc = Process(target=self.tools, args=(url, path))
                 processes.append(proc)
                 proc.start()
 
-            for process in processes:
-                process.join()
-        else:
-            for url, path in sources.items():
+        for process in processes:
+            process.join()
+
+    def normal_download(self, sources: dict) -> None:
+        """ Download sources with normal mode. """
+        for urls, path in sources.values():
+            for url in urls:
                 self.tools(url, path)
 
     def tools(self, url: str, path: Path) -> None:
         url_parse: str = urlparse(url).path
         self.filename: str = unquote(Path(url_parse).name)
 
         if url.startswith('file'):
```

### Comparing `slpkg-4.8.7/slpkg/models/models.py` & `slpkg-4.8.8/slpkg/models/models.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/rules.py` & `slpkg-4.8.8/slpkg/rules.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/views/view_package.py` & `slpkg-4.8.8/slpkg/views/view_package.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/views/version.py` & `slpkg-4.8.8/slpkg/views/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 class Version:
     """ Print the version. """
 
     def __init__(self):
-        self.version_info: tuple = (4, 8, 7)
+        self.version_info: tuple = (4, 8, 8)
         self.version: str = '{0}.{1}.{2}'.format(*self.version_info)
         self.license: str = 'MIT License'
         self.author: str = 'Dimitris Zlatanidis (dslackw)'
         self.homepage: str = 'https://dslackw.gitlab.io/slpkg'
 
     def view(self) -> None:
         """ Prints the version. """
```

### Comparing `slpkg-4.8.7/slpkg/views/cli_menu.py` & `slpkg-4.8.8/slpkg/views/cli_menu.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/views/asciibox.py` & `slpkg-4.8.8/slpkg/views/asciibox.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/views/help_commands.py` & `slpkg-4.8.8/slpkg/views/help_commands.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/views/views.py` & `slpkg-4.8.8/slpkg/views/views.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/checks.py` & `slpkg-4.8.8/slpkg/checks.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/logging_deps.py` & `slpkg-4.8.8/slpkg/logging_deps.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/new_configs.py` & `slpkg-4.8.8/slpkg/new_configs.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/multi_process.py` & `slpkg-4.8.8/slpkg/multi_process.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/cleanings.py` & `slpkg-4.8.8/slpkg/cleanings.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/checksum.py` & `slpkg-4.8.8/slpkg/checksum.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/dialog_box.py` & `slpkg-4.8.8/slpkg/dialog_box.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/configs.py` & `slpkg-4.8.8/slpkg/configs.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/utilities.py` & `slpkg-4.8.8/slpkg/utilities.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/dependees.py` & `slpkg-4.8.8/slpkg/dependees.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/toml_error_message.py` & `slpkg-4.8.8/slpkg/toml_error_message.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/check_updates.py` & `slpkg-4.8.8/slpkg/check_updates.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/remove_packages.py` & `slpkg-4.8.8/slpkg/remove_packages.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/blacklist.py` & `slpkg-4.8.8/slpkg/blacklist.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/download_only.py` & `slpkg-4.8.8/slpkg/download_only.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,23 +66,23 @@
         if self.option_for_directory:
             self.download_path: Path = self.directory
 
     def save_binary_sources(self, name: str) -> None:
         package: str = self.data[name]['package']
         mirror: str = self.data[name]['mirror']
         location: str = self.data[name]['location']
-        self.urls[f'{mirror}{location}/{package}'] = self.tmp_slpkg
+        url: str = f'{mirror}{location}/{package}'
+        self.urls[name] = ((url,), self.tmp_slpkg)
 
     def save_slackbuild_sources(self, name: str) -> None:
         if self.os_arch == 'x86_64' and self.data[name]['download64']:
-            sources: list = self.data[name]['download64'].split()
+            sources: tuple = self.data[name]['download64'].split()
         else:
-            sources: list = self.data[name]['download'].split()
-        for source in sources:
-            self.urls[source] = Path(self.build_path, name)
+            sources: tuple = self.data[name]['download'].split()
+        self.urls[name] = (sources, Path(self.build_path, name))
 
     def copy_slackbuild_scripts(self, name: str) -> None:
         repo_path_package: Path = Path(self.sbo_repo[self.repository], self.data[name]['location'], name)
         if not Path(self.download_path, name).is_dir():
             shutil.copytree(repo_path_package, Path(self.download_path, name))
         print(f"{self.byellow}Copying{self.endc}: {repo_path_package} -> {Path(self.download_path, name)}")
```

### Comparing `slpkg-4.8.7/slpkg/tracking.py` & `slpkg-4.8.8/slpkg/tracking.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/logging_config.py` & `slpkg-4.8.8/slpkg/logging_config.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/main.py` & `slpkg-4.8.8/slpkg/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
-import os
 import sys
 import logging
 from pathlib import Path
 
 from slpkg.checks import Check
 from slpkg.upgrade import Upgrade
 from slpkg.configs import Configs
 from slpkg.tracking import Tracking
 from slpkg.repo_info import RepoInfo
 from slpkg.dependees import Dependees
 from slpkg.utilities import Utilities
 from slpkg.cleanings import Cleanings
 from slpkg.search import SearchPackage
 from slpkg.views.cli_menu import Usage
-from slpkg.dialog_box import DialogBox
 from slpkg.views.version import Version
+from slpkg.choose_packages import Choose
 from slpkg.views.asciibox import AsciiBox
 from slpkg.sbos.queries import SBoQueries
 from slpkg.views.help_commands import Help
 from slpkg.repositories import Repositories
 from slpkg.binaries.install import Packages
 from slpkg.dialog_configs import FormConfigs
 from slpkg.check_updates import CheckUpdates
@@ -299,15 +298,15 @@
         self.split_options_from_args()
         self.move_options()
         self.invalid_options()
         self.check_for_repositories()
 
         self.is_binary: bool = self.utils.is_binary_repo(self.repository)
         self.check = Check(self.repository)
-        self.choose = ChoosePackages(self.repository)
+        self.choose = Choose(self.repository)
 
         logging.basicConfig(filename=LoggingConfig.log_file,
                             filemode=LoggingConfig.filemode,
                             encoding=LoggingConfig.encoding,
                             level=LoggingConfig.level)
 
         logger = logging.getLogger(LoggingConfig.date_time)
@@ -754,93 +753,14 @@
     def clean_data(self) -> None:
         if len(self.args) == 1:
             self.clean.db_tables()
             raise SystemExit()
         self.usage.help_short(1)
 
 
-class ChoosePackages(Configs):
-    """ Choose packages with dialog utility and -S, --search flag. """
-
-    def __init__(self, repository: str):
-        self.repository: str = repository
-
-        self.utils = Utilities()
-        self.dialogbox = DialogBox()
-
-        self.is_binary: bool = self.utils.is_binary_repo(repository)
-
-    def packages(self, data: dict, packages: list, method: str) -> list:
-        if self.dialog:
-            height: int = 10
-            width: int = 70
-            list_height: int = 0
-            choices: list = []
-            title: str = f' Choose packages you want to {method} '
-
-            repo_packages: list = list(data.keys())
-
-            if method in ['remove', 'find']:
-                installed: list = list(self.utils.installed_packages.values())
-
-                for package in installed:
-                    package_name: str = self.utils.split_package(package)['name']
-                    package_version: str = self.utils.split_package(package)['version']
-
-                    for pkg in packages:
-                        if pkg in package or pkg == '*':
-                            choices.extend([(package_name, package_version, False, f'Package: {package}')])
-
-            elif method == 'upgrade':
-                for pkg in packages:
-                    for package in repo_packages:
-
-                        if pkg == package:
-                            inst_pkg: str = self.utils.is_package_installed(package)
-                            inst_package_version: str = self.utils.split_package(inst_pkg)['version']
-                            inst_package_build: str = self.utils.split_package(inst_pkg)['build']
-                            repo_ver: str = data[package]['version']
-
-                            if self.is_binary:
-                                bin_pkg: str = data[package]['package']
-                                repo_build_tag: str = self.utils.split_package(bin_pkg[:-4])['build']
-                            else:
-                                repo_location: str = data[package]['location']
-                                repo_build_tag: str = self.utils.read_slackbuild_build_tag(
-                                    package, repo_location, self.repository
-                                )
-
-                            choices.extend(
-                                [(package, f'{inst_package_version} -> {repo_ver}', True,
-                                  f'Installed: {package}-{inst_package_version} Build: {inst_package_build} -> '
-                                  f'Available: {repo_ver} Build: {repo_build_tag}')]
-                            )
-            else:
-                for pkg in packages:
-                    for package in repo_packages:
-
-                        if pkg in package or pkg == '*':
-                            version: str = data[package]['version']
-                            choices.extend([(package, version, False, f'Package: {package}-{version} '
-                                           f'> {self.repository}')])
-
-            if not choices:
-                return packages
-
-            text: str = f'There are {len(choices)} packages:'
-            code, packages = self.dialogbox.checklist(text, title, height, width, list_height, choices)
-            if code == 'cancel' or not packages:
-                os.system('clear')
-                raise SystemExit()
-
-            os.system('clear')
-
-        return packages
-
-
 def main() -> None:
     args: list = sys.argv
     args.pop(0)
     usage = Usage()
 
     if len(args) == 0 or '' in args:
         usage.help_short(1)
```

### Comparing `slpkg-4.8.7/slpkg/find_installed.py` & `slpkg-4.8.8/slpkg/find_installed.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/upgrade.py` & `slpkg-4.8.8/slpkg/upgrade.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/slpkg/search.py` & `slpkg-4.8.8/slpkg/search.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.7/setup.cfg` & `slpkg-4.8.8/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = slpkg
-version = 4.8.7
+version = 4.8.8
 license_file = LICENSE
 author = Dimitris Zlatanidis
 author_email = dslackw@gmail.com
 description = Package manager utility for Slackware Linux.
 long_description = file:README.rst
 url = https://dslackw.gitlab.io/slpkg/
 project_urls =
```

### Comparing `slpkg-4.8.7/slpkg.egg-info/SOURCES.txt` & `slpkg-4.8.8/slpkg.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.cfg
 setup.py
 slpkg/__init__.py
 slpkg/blacklist.py
 slpkg/check_updates.py
 slpkg/checks.py
 slpkg/checksum.py
+slpkg/choose_packages.py
 slpkg/cleanings.py
 slpkg/configs.py
 slpkg/dependees.py
 slpkg/dialog_box.py
 slpkg/dialog_configs.py
 slpkg/download_only.py
 slpkg/downloader.py
```

### Comparing `slpkg-4.8.7/slpkg.egg-info/PKG-INFO` & `slpkg-4.8.8/slpkg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slpkg
-Version: 4.8.7
+Version: 4.8.8
 Summary: Package manager utility for Slackware Linux.
 Home-page: https://dslackw.gitlab.io/slpkg/
 Author: Dimitris Zlatanidis
 Author-email: dslackw@gmail.com
 License: UNKNOWN
 Project-URL: Source, https://dslackw.gitlab.io/slpkg/
 Project-URL: Documentation, https://dslackw.gitlab.io/slpkg/
```

### Comparing `slpkg-4.8.7/README.md` & `slpkg-4.8.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -56,16 +56,16 @@
 $ slpkg tracking --pkg-version Flask awscli pychess
 ```
 <img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_tracking.png" width="900">
 
 ### Installation
 
 ```
-$ tar xvf slpkg-4.8.7.tar.gz
-$ cd slpkg-4.8.7
+$ tar xvf slpkg-4.8.8.tar.gz
+$ cd slpkg-4.8.8
 $ ./install.sh
 ```
 
 ### Requirements
 
 ```
 SQLAlchemy >= 1.4.46
@@ -82,15 +82,15 @@
 
 The majority of trials have been made in Slackware x86_64 'stable' environment.
 
 
 ### Command Line Tool Usage
 
 ```
-slpkg - version 4.8.7
+slpkg - version 4.8.8
 
 USAGE:
   slpkg [COMMAND] [OPTIONS] [FILELIST|PACKAGES...]
 
 DESCRIPTION:
   Package manager utility for Slackware.
```

### Comparing `slpkg-4.8.7/tools/gen_sbo_txt.sh` & `slpkg-4.8.8/tools/gen_sbo_txt.sh`

 * *Files identical despite different names*

