# Comparing `tmp/ddqa-0.3.0.tar.gz` & `tmp/ddqa-0.3.1.tar.gz`

## Comparing `ddqa-0.3.0.tar` & `ddqa-0.3.1.tar`

### file list

```diff
@@ -1,108 +1,130 @@
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ddqa-0.3.0/.gitattributes
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ddqa-0.3.0/.linkcheckerrc
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 ddqa-0.3.0/HISTORY.md
--rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 ddqa-0.3.0/mkdocs.yml
--rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 ddqa-0.3.0/pyoxidizer.bzl
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 ddqa-0.3.0/.github/dependabot.yml
--rw-r--r--   0        0        0    12900 2020-02-02 00:00:00.000000 ddqa-0.3.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 ddqa-0.3.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 ddqa-0.3.0/.github/workflows/publish-docs.yml
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 ddqa-0.3.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 ddqa-0.3.0/docs/index.md
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 ddqa-0.3.0/docs/install.md
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ddqa-0.3.0/docs/.snippets/abbrs.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ddqa-0.3.0/docs/.snippets/links.txt
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 ddqa-0.3.0/docs/assets/css/custom.css
--rw-r--r--   0        0        0    40436 2020-02-02 00:00:00.000000 ddqa-0.3.0/docs/assets/images/favicon.ico
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 ddqa-0.3.0/docs/assets/images/logo.svg
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 ddqa-0.3.0/docs/config/repo.md
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 ddqa-0.3.0/docs/config/user.md
--rw-r--r--   0        0        0   193753 2020-02-02 00:00:00.000000 ddqa-0.3.0/screenshots/config.PNG
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/__init__.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/__main__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/py.typed
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/app/__init__.py
--rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/app/core.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/app/style.py
--rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/cli/__init__.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/cli/config/__init__.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/cli/config/edit.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/cli/config/explore.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/cli/config/find.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/cli/config/restore.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/cli/config/show.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/cli/create/__init__.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/cli/status/__init__.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/cli/sync/__init__.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/config/__init__.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/config/constants.py
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/config/core.py
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/config/file.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/config/utils.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/data/__init__.py
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/data/logo.png
--rw-r--r--   0        0        0   345099 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/data/shame.png
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/models/__init__.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/models/github.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/models/jira.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/models/config/__init__.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/models/config/app.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/models/config/auth.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/models/config/repo.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/models/config/team.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/screens/__init__.py
--rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/screens/configure.py
--rw-r--r--   0        0        0    15706 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/screens/create.py
--rw-r--r--   0        0        0    17067 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/screens/status.py
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/screens/sync.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/utils/__init__.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/utils/ci.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/utils/errors.py
--rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/utils/fs.py
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/utils/git.py
--rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/utils/github.py
--rw-r--r--   0        0        0    11019 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/utils/jira.py
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/utils/network.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/utils/structures.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/utils/time.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/utils/widgets.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/widgets/__init__.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/widgets/input.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/widgets/layout.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/widgets/static.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/cli/__init__.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/cli/config/__init__.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/cli/config/test_edit.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/cli/config/test_explore.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/cli/config/test_find.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/cli/config/test_restore.py
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/cli/config/test_show.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/cli/create/__init__.py
--rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/cli/create/test_create.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/cli/status/__init__.py
--rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/cli/status/test_status.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/cli/sync/__init__.py
--rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/cli/sync/test_sync.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/helpers/__init__.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/helpers/api.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/screens/__init__.py
--rw-r--r--   0        0        0    23170 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/screens/test_configure.py
--rw-r--r--   0        0        0    34995 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/screens/test_create.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/screens/test_status.py
--rw-r--r--   0        0        0     7905 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/screens/test_sync.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/utils/test_fs.py
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/utils/test_git.py
--rw-r--r--   0        0        0    22924 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/utils/test_github.py
--rw-r--r--   0        0        0    28668 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/utils/test_jira.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/utils/test_structures.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/utils/test_time.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 ddqa-0.3.0/.gitignore
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ddqa-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 ddqa-0.3.0/README.md
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 ddqa-0.3.0/hatch.toml
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 ddqa-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 ddqa-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ddqa-0.3.1/.gitattributes
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ddqa-0.3.1/.linkcheckerrc
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 ddqa-0.3.1/HISTORY.md
+-rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 ddqa-0.3.1/mkdocs.yml
+-rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 ddqa-0.3.1/pyoxidizer.bzl
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 ddqa-0.3.1/.github/dependabot.yml
+-rw-r--r--   0        0        0    12900 2020-02-02 00:00:00.000000 ddqa-0.3.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 ddqa-0.3.1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 ddqa-0.3.1/.github/workflows/publish-docs.yml
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 ddqa-0.3.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/index.md
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/install.md
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/.snippets/abbrs.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/.snippets/links.txt
+-rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/actions/create.md
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/actions/status.md
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/css/custom.css
+-rw-r--r--   0        0        0    15039 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/creation-screen-candidate-assignments.png
+-rw-r--r--   0        0        0    94623 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/creation-screen-candidate-description.png
+-rw-r--r--   0        0        0     7207 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/creation-screen-candidate-pr-labels.png
+-rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/creation-screen-candidate-title.png
+-rw-r--r--   0        0        0    77999 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/creation-screen-candidates.png
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/creation-screen-exit.png
+-rw-r--r--   0        0        0   207825 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/creation-screen-full.png
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/creation-screen-items.png
+-rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/creation-screen-progress.png
+-rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/creation-screen-queue.png
+-rw-r--r--   0        0        0     5639 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/creation-screen-results.png
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/creation-screen-transition.png
+-rw-r--r--   0        0        0    40436 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/favicon.ico
+-rw-r--r--   0        0        0    43005 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/github-token1.png
+-rw-r--r--   0        0        0    38694 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/github-token2.png
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/logo.svg
+-rw-r--r--   0        0        0   177330 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/screen-config.png
+-rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/status-screen-filters.png
+-rw-r--r--   0        0        0   285123 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/status-screen-full.png
+-rw-r--r--   0        0        0   253690 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/status-screen-issues.png
+-rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/status-screen-metadata.png
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/status-screen-progress.png
+-rw-r--r--   0        0        0    10824 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/assets/images/status-screen-qa-status.png
+-rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/config/repo.md
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 ddqa-0.3.1/docs/config/user.md
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/__init__.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/py.typed
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/app/__init__.py
+-rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/app/core.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/app/style.py
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/cli/__init__.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/cli/config/__init__.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/cli/config/edit.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/cli/config/explore.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/cli/config/find.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/cli/config/restore.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/cli/config/show.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/cli/create/__init__.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/cli/status/__init__.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/cli/sync/__init__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/config/__init__.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/config/constants.py
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/config/core.py
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/config/file.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/config/utils.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/data/__init__.py
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/data/logo.png
+-rw-r--r--   0        0        0   345099 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/data/shame.png
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/models/__init__.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/models/github.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/models/jira.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/models/config/__init__.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/models/config/app.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/models/config/auth.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/models/config/repo.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/models/config/team.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/screens/__init__.py
+-rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/screens/configure.py
+-rw-r--r--   0        0        0    15712 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/screens/create.py
+-rw-r--r--   0        0        0    17067 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/screens/status.py
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/screens/sync.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/utils/__init__.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/utils/ci.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/utils/errors.py
+-rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/utils/fs.py
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/utils/git.py
+-rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/utils/github.py
+-rw-r--r--   0        0        0    11019 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/utils/jira.py
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/utils/network.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/utils/structures.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/utils/time.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/utils/widgets.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/widgets/__init__.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/widgets/input.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/widgets/layout.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 ddqa-0.3.1/src/ddqa/widgets/static.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/conftest.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/cli/__init__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/cli/config/__init__.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/cli/config/test_edit.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/cli/config/test_explore.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/cli/config/test_find.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/cli/config/test_restore.py
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/cli/config/test_show.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/cli/create/__init__.py
+-rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/cli/create/test_create.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/cli/status/__init__.py
+-rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/cli/status/test_status.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/cli/sync/__init__.py
+-rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/cli/sync/test_sync.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/helpers/__init__.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/helpers/api.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/screens/__init__.py
+-rw-r--r--   0        0        0    23170 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/screens/test_configure.py
+-rw-r--r--   0        0        0    34995 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/screens/test_create.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/screens/test_status.py
+-rw-r--r--   0        0        0     7905 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/screens/test_sync.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/utils/__init__.py
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/utils/test_fs.py
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/utils/test_git.py
+-rw-r--r--   0        0        0    22924 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/utils/test_github.py
+-rw-r--r--   0        0        0    28668 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/utils/test_jira.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/utils/test_structures.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 ddqa-0.3.1/tests/utils/test_time.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 ddqa-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ddqa-0.3.1/LICENSE.txt
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 ddqa-0.3.1/README.md
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 ddqa-0.3.1/hatch.toml
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 ddqa-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 ddqa-0.3.1/PKG-INFO
```

### Comparing `ddqa-0.3.0/HISTORY.md` & `ddqa-0.3.1/HISTORY.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## Unreleased
 
+## 0.3.1 - 2023-06-02
+
+***Fixed:***
+
+- Fix race condition when prematurely creating issues
+
 ## 0.3.0 - 2023-05-24
 
 ***Added:***
 
 - Upgrade Textual to 0.20.1
 - Upgrade PyApp to 0.7.0
```

### Comparing `ddqa-0.3.0/mkdocs.yml` & `ddqa-0.3.1/mkdocs.yml`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,17 @@
 
 nav:
   - About: index.md
   - Installation: install.md
   - Configuration:
     - User: config/user.md
     - Repository: config/repo.md
+  - Actions:
+    - Create items: actions/create.md
+    - View dashboard: actions/status.md
 
 plugins:
   # Built-in
   search: {}
   # Extra
   glightbox: {}
   minify:
@@ -54,14 +57,15 @@
 
 markdown_extensions:
   # Built-in
   - markdown.extensions.abbr:
   - markdown.extensions.admonition:
   - markdown.extensions.attr_list:
   - markdown.extensions.footnotes:
+  - markdown.extensions.md_in_html:
   - markdown.extensions.meta:
   - markdown.extensions.tables:
   - markdown.extensions.toc:
       permalink: true
   # Extra
   - pymdownx.arithmatex:
   - pymdownx.betterem:
```

### Comparing `ddqa-0.3.0/pyoxidizer.bzl` & `ddqa-0.3.1/pyoxidizer.bzl`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/.github/workflows/build.yml` & `ddqa-0.3.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/.github/workflows/docs.yml` & `ddqa-0.3.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/.github/workflows/publish-docs.yml` & `ddqa-0.3.1/.github/workflows/publish-docs.yml`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/.github/workflows/test.yml` & `ddqa-0.3.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/docs/index.md` & `ddqa-0.3.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/docs/assets/css/custom.css` & `ddqa-0.3.1/docs/assets/css/custom.css`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/docs/assets/images/favicon.ico` & `ddqa-0.3.1/docs/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/docs/assets/images/logo.svg` & `ddqa-0.3.1/docs/assets/images/logo.svg`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/docs/config/repo.md` & `ddqa-0.3.1/docs/config/repo.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,112 @@
 # Repository configuration
 
 -----
 
-A repository must be configured before use:
+A repository must be configured ([example](https://github.com/DataDog/integrations-core/blob/master/.ddqa/config.toml)) before use:
 
 ```toml
 global_config_source = "..."
 qa_statuses = ["..."]
 
 [teams."..."]
 github_team = "..."
 jira_project = "..."
 jira_issue_type = "..."
 jira_statuses = ["..."]
 ```
 
+The config file is located by default in your repository at `/.ddqa/config.toml` and can be overridden with the top level `--config` option.
+
 ## Core options
 
-- `global_config_source` (***required***) - This is a URL (optionally encoded in [Base64](https://en.wikipedia.org/wiki/Base64)) like `https://raw.githubusercontent.com/org/repo/master/jira.toml` that points to the raw contents of a TOML file on GitHub that contains potentially private metadata that the tool needs in order to operate. Currently, the only required information is the cloud URL and a mapping of GitHub usernames to Jira IDs:
-  ```toml
-  jira_server = "https://<ORG>.atlassian.net"
-
-  [members]
-  github-user1 = "jira-id1"
-  ```
-- `qa_statuses` (***required***) - The entries and order of this list correspond to the desired QA workflow, for example:
-  ```toml
-  qa_statuses = [
-    "TODO",
-    "Testing",
-    "Done",
-  ]
-  ```
-- `ignored_labels` - Any pull requests labeled with any of the entries will not be assigned by default:
-  ```toml
-  ignored_labels = [
-    "changelog/no-changelog",
-  ]
-  ```
+### Global config source (*required*) ### {: #global-config-source }
+
+Key: `global_config_source`
+
+This is a URL (optionally encoded in [Base64](https://en.wikipedia.org/wiki/Base64)) like `https://raw.githubusercontent.com/org/repo/master/jira.toml` that points to the raw contents of a TOML file on GitHub that contains potentially private metadata that the tool needs in order to operate. Currently, the only required information is the cloud URL and a mapping of GitHub usernames to Jira IDs:
+
+```toml
+jira_server = "https://<ORG>.atlassian.net"
+
+[members]
+github-user1 = "jira-id1"
+```
+
+### QA statuses (*required*) ### {: #qa-statuses }
+
+Key: `qa_statuses`
+
+The entries and order of this list correspond to the desired QA workflow, for example:
+
+```toml
+qa_statuses = [
+  "TODO",
+  "Testing",
+  "Done",
+]
+```
+
+### Ignored labels
+
+Key: `ignored_labels`
+
+Any pull requests labeled with any of the entries will not be assigned by default:
+
+```toml
+ignored_labels = [
+  "changelog/no-changelog",
+]
+```
 
 ## Teams
 
-Each team must be configured. The name of each team is arbitrary but should be the human readable version or a nickname. The order of teams is also arbitrary but would benefit from being ordered by teams that commit/would be assigned most frequently as manual selection would potentially require less scrolling.
+Each team must be configured.
+
+```toml
+[teams."..."]
+# Per-team options
+```
+
+The name of each team is arbitrary but should be the human readable version or a nickname. The order of teams is also arbitrary but would benefit from being ordered by teams that commit/would be assigned most frequently as manual selection would potentially require less scrolling.
+
+### GitHub team (*required*) ### {: #github-team }
+
+Key: `github_team`
+
+This is the team's GitHub name, excluding the organization `<ORG>/` prefix.
+
+### Jira project (*required*) ### {: #jira-project }
+
+Key: `jira_project`
+
+This is the team's Jira project in which issues will be created. If there exists an issue `FOO-123`, the project name is `FOO`.
+
+### Jira issue type (*required*) ### {: #jira-issue-type }
+
+Key: `jira_issue_type`
+
+This is the type of Jira issue that will be created and will most often be `Task`. The issue type can be found as the `fields.issuetype.name` returned value in the payload from the [`/rest/api/2/issue/{issueIdOrKey}`](https://developer.atlassian.com/cloud/jira/platform/rest/v2/api-group-issues/#api-rest-api-2-issue-issueidorkey-get) endpoint.
+
+### Jira statuses (*required*) ### {: #jira-statuses }
+
+Key: `jira_statuses`
+
+This is an array of Jira statuses that correspond to the order of [QA status](#qa-statuses) entries. Alternatively, this may be a mapping of [QA statuses](#qa-statuses) to Jira statuses. The available Jira statuses may be found using the [`/rest/api/2/project/{projectIdOrKey}/statuses`](https://developer.atlassian.com/cloud/jira/platform/rest/v2/api-group-projects/#api-rest-api-2-project-projectidorkey-statuses-get) endpoint.
+
+### GitHub labels
+
+Key: `github_labels`
+
+This team will be assigned by default to any pull requests that are labeled with any of the entries (as long as the pull request has no labels that match any of those defined as [ignored](#ignored-labels)).
+
+### Jira component
+
+Key: `jira_component`
+
+This is the name of a Jira [project component](https://support.atlassian.com/jira-software-cloud/docs/organize-work-with-components/) with which to create issues.
+
+### Excluded members
+
+Key: `exclude_members`
 
-- `github_team` (***required***) - This is the team's GitHub name, excluding the organization `<ORG>/` prefix
-- `jira_project` (***required***) - This is the team's Jira project in which issues will be created. If there exists an issue `FOO-123`, the project name is `FOO`.
-- `jira_issue_type` (***required***) - This is the type of Jira issue that will be created and will most often be `Task`. The issue type can be found as the `fields.issuetype.name` returned value in the payload from the [`/rest/api/2/issue/{issueIdOrKey}`](https://developer.atlassian.com/cloud/jira/platform/rest/v2/api-group-issues/#api-rest-api-2-issue-issueidorkey-get) endpoint.
-- `jira_statuses` (***required***) - This is an array of Jira statuses that map to the top-level `qa_statuses` option. Alternatively, this may be a mapping of QA statuses to Jira statuses. The available Jira statuses may be found using the [`/rest/api/2/project/{projectIdOrKey}/statuses`](https://developer.atlassian.com/cloud/jira/platform/rest/v2/api-group-projects/#api-rest-api-2-project-projectidorkey-statuses-get) endpoint.
-- `github_labels` - This team will be assigned by default to any pull requests that are labeled with any of the entries (as long as the pull request has no labels that match any of those defined in the top-level `ignored_labels` option)
-- `jira_component` - This is the name of a Jira [project component](https://support.atlassian.com/jira-software-cloud/docs/organize-work-with-components/) with which to create issues
-- `exclude_members` - This is an array of members who should be excluded from QA participation
+This is an array of GitHub usernames who should be excluded from QA participation.
```

### Comparing `ddqa-0.3.0/docs/config/user.md` & `ddqa-0.3.1/docs/config/user.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,28 @@
 # User configuration
 
 -----
 
 DDQA will always ensure valid config by loading the configuration screen if there are errors or missing required fields.
 
+<figure markdown>
+  ![Input screen](../assets/images/screen-config.png){ loading=lazy role="img" }
+</figure>
+
+!!! tip
+    To locate your personal config file you may run: `ddqa config find`
+
 ## GitHub auth
 
-You'll need to create a [personal access token (classic)](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token#personal-access-tokens-classic) with `public_repo` and `read:org` permissions and, if required by the organization, [enable SAML single sign-on](https://docs.github.com/en/enterprise-cloud@latest/authentication/authenticating-with-saml-single-sign-on/authorizing-a-personal-access-token-for-use-with-saml-single-sign-on).
+You'll need to create a [personal access token (classic)](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token#personal-access-tokens-classic) with `repo` and `read:org` permissions and, if required by the organization, [enable SAML single sign-on](https://docs.github.com/en/enterprise-cloud@latest/authentication/authenticating-with-saml-single-sign-on/authorizing-a-personal-access-token-for-use-with-saml-single-sign-on).
+
+<figure markdown>
+  ![GitHub token 1](../assets/images/github-token1.png){ loading=lazy role="img" }
+  ![GitHub token 2](../assets/images/github-token2.png){ loading=lazy role="img" }
+</figure>
 
 The following APIs are used:
 
 - `/search/issues` ([GET](https://docs.github.com/en/rest/search?apiVersion=2022-11-28#search-issues-and-pull-requests))
 - `/repos/{owner}/{repo}/pulls/{pull_number}/reviews` ([GET](https://docs.github.com/en/rest/pulls/reviews?apiVersion=2022-11-28#list-reviews-for-a-pull-request))
 - `/orgs/{org}/teams/{team_slug}/members` ([GET](https://docs.github.com/en/rest/teams/members?apiVersion=2022-11-28#list-team-members))
```

### Comparing `ddqa-0.3.0/src/ddqa/app/core.py` & `ddqa-0.3.1/src/ddqa/app/core.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/src/ddqa/cli/__init__.py` & `ddqa-0.3.1/src/ddqa/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/src/ddqa/cli/config/__init__.py` & `ddqa-0.3.1/src/ddqa/cli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/src/ddqa/cli/config/show.py` & `ddqa-0.3.1/src/ddqa/cli/config/show.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/src/ddqa/cli/create/__init__.py` & `ddqa-0.3.1/src/ddqa/cli/create/__init__.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/src/ddqa/cli/status/__init__.py` & `ddqa-0.3.1/src/ddqa/cli/status/__init__.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/src/ddqa/config/core.py` & `ddqa-0.3.1/src/ddqa/config/core.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/src/ddqa/config/file.py` & `ddqa-0.3.1/src/ddqa/config/file.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/src/ddqa/data/logo.png` & `ddqa-0.3.1/src/ddqa/data/logo.png`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/src/ddqa/data/shame.png` & `ddqa-0.3.1/src/ddqa/data/shame.png`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/src/ddqa/models/github.py` & `ddqa-0.3.1/src/ddqa/models/github.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/src/ddqa/models/jira.py` & `ddqa-0.3.1/src/ddqa/models/jira.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/src/ddqa/models/config/repo.py` & `ddqa-0.3.1/src/ddqa/models/config/repo.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/src/ddqa/screens/configure.py` & `ddqa-0.3.1/src/ddqa/screens/configure.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/src/ddqa/screens/create.py` & `ddqa-0.3.1/src/ddqa/screens/create.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         display_updated = False
 
         assignment_counts: dict[str, dict[str, int]] = defaultdict(lambda: defaultdict(int))
 
         self.app.print(f'Candidates ready for creation: {total}')
         self.sidebar.status.update('Creating...')
         async with ResponsiveNetworkClient(self.sidebar.status) as client:
-            for index, candidate in self.candidates.items():
+            for index, candidate in list(self.candidates.items()):
                 self.app.print(f'Creating issue for {candidate.data.long_display()}')
 
                 assignments: dict[str, str] = {}
                 for team, assigned in candidate.assignments.items():
                     if not assigned:
                         continue
```

### Comparing `ddqa-0.3.0/src/ddqa/screens/status.py` & `ddqa-0.3.1/src/ddqa/screens/status.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/src/ddqa/screens/sync.py` & `ddqa-0.3.1/src/ddqa/screens/sync.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/src/ddqa/utils/fs.py` & `ddqa-0.3.1/src/ddqa/utils/fs.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/src/ddqa/utils/git.py` & `ddqa-0.3.1/src/ddqa/utils/git.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/src/ddqa/utils/github.py` & `ddqa-0.3.1/src/ddqa/utils/github.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/src/ddqa/utils/jira.py` & `ddqa-0.3.1/src/ddqa/utils/jira.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/src/ddqa/utils/network.py` & `ddqa-0.3.1/src/ddqa/utils/network.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/src/ddqa/utils/structures.py` & `ddqa-0.3.1/src/ddqa/utils/structures.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/src/ddqa/utils/time.py` & `ddqa-0.3.1/src/ddqa/utils/time.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/src/ddqa/widgets/input.py` & `ddqa-0.3.1/src/ddqa/widgets/input.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/src/ddqa/widgets/layout.py` & `ddqa-0.3.1/src/ddqa/widgets/layout.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/src/ddqa/widgets/static.py` & `ddqa-0.3.1/src/ddqa/widgets/static.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/tests/conftest.py` & `ddqa-0.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/tests/cli/config/test_restore.py` & `ddqa-0.3.1/tests/cli/config/test_restore.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/tests/cli/config/test_show.py` & `ddqa-0.3.1/tests/cli/config/test_show.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/tests/cli/create/test_create.py` & `ddqa-0.3.1/tests/cli/create/test_create.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/tests/cli/status/test_status.py` & `ddqa-0.3.1/tests/cli/status/test_status.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/tests/cli/sync/test_sync.py` & `ddqa-0.3.1/tests/cli/sync/test_sync.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/tests/helpers/api.py` & `ddqa-0.3.1/tests/helpers/api.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/tests/screens/test_configure.py` & `ddqa-0.3.1/tests/screens/test_configure.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/tests/screens/test_create.py` & `ddqa-0.3.1/tests/screens/test_create.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/tests/screens/test_sync.py` & `ddqa-0.3.1/tests/screens/test_sync.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/tests/utils/test_fs.py` & `ddqa-0.3.1/tests/utils/test_fs.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/tests/utils/test_git.py` & `ddqa-0.3.1/tests/utils/test_git.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/tests/utils/test_github.py` & `ddqa-0.3.1/tests/utils/test_github.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/tests/utils/test_jira.py` & `ddqa-0.3.1/tests/utils/test_jira.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/tests/utils/test_structures.py` & `ddqa-0.3.1/tests/utils/test_structures.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/tests/utils/test_time.py` & `ddqa-0.3.1/tests/utils/test_time.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/LICENSE.txt` & `ddqa-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/README.md` & `ddqa-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/hatch.toml` & `ddqa-0.3.1/hatch.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
   "pytest-asyncio",
   "pytest-mock",
+  "pytest-randomly",
 ]
 # pre-install-commands = [
 #   "python -m pip install --disable-pip-version-check git+https://github.com/Textualize/textual.git",
 # ]
 [envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
```

### Comparing `ddqa-0.3.0/pyproject.toml` & `ddqa-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ddqa-0.3.0/PKG-INFO` & `ddqa-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddqa
-Version: 0.3.0
+Version: 0.3.1
 Summary: Datadog's QA manager for releases of GitHub repositories
 Project-URL: Source, https://github.com/DataDog/ddqa
 Author-email: "Datadog, Inc." <dev@datadoghq.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Keywords: datadog,qa,testing,tooling
 Classifier: Development Status :: 4 - Beta
```

