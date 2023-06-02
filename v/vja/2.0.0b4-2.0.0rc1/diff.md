# Comparing `tmp/vja-2.0.0b4.tar.gz` & `tmp/vja-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vja-2.0.0b4.tar", last modified: Mon Apr 24 08:34:51 2023, max compression
+gzip compressed data, was "vja-2.0.0rc1.tar", last modified: Fri Jun  2 17:51:35 2023, max compression
```

## Comparing `vja-2.0.0b4.tar` & `vja-2.0.0rc1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:34:51.204191 vja-2.0.0b4/
--rw-r--r--   0 root         (0) root         (0)     8442 2023-04-24 08:34:51.204191 vja-2.0.0b4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-04-24 08:34:51.204191 vja-2.0.0b4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      919 2023-04-24 08:33:47.000000 vja-2.0.0b4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:34:51.200190 vja-2.0.0b4/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 08:33:47.000000 vja-2.0.0b4/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1711 2023-04-24 08:33:47.000000 vja-2.0.0b4/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     2847 2023-04-24 08:33:47.000000 vja-2.0.0b4/tests/test_basic.py
--rw-rw-rw-   0 root         (0) root         (0)    10091 2023-04-24 08:33:47.000000 vja-2.0.0b4/tests/test_command.py
--rw-rw-rw-   0 root         (0) root         (0)     8844 2023-04-24 08:33:47.000000 vja-2.0.0b4/tests/test_query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:34:51.203191 vja-2.0.0b4/vja/
--rwxrwxrwx   0 root         (0) root         (0)      220 2023-04-24 08:33:47.000000 vja-2.0.0b4/vja/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6802 2023-04-24 08:33:47.000000 vja-2.0.0b4/vja/apiclient.py
--rw-rw-rw-   0 root         (0) root         (0)     2777 2023-04-24 08:33:47.000000 vja-2.0.0b4/vja/authenticate.py
--rwxrwxrwx   0 root         (0) root         (0)    17734 2023-04-24 08:33:47.000000 vja-2.0.0b4/vja/cli.py
--rwxrwxrwx   0 root         (0) root         (0)     1967 2023-04-24 08:33:47.000000 vja-2.0.0b4/vja/config.py
--rw-rw-rw-   0 root         (0) root         (0)     3736 2023-04-24 08:33:47.000000 vja-2.0.0b4/vja/filter.py
--rw-rw-rw-   0 root         (0) root         (0)     2572 2023-04-24 08:33:47.000000 vja-2.0.0b4/vja/list_service.py
--rwxrwxrwx   0 root         (0) root         (0)     6008 2023-04-24 08:33:47.000000 vja-2.0.0b4/vja/model.py
--rw-rw-rw-   0 root         (0) root         (0)     3289 2023-04-24 08:33:47.000000 vja-2.0.0b4/vja/output.py
--rw-rw-rw-   0 root         (0) root         (0)     2637 2023-04-24 08:33:47.000000 vja-2.0.0b4/vja/parse.py
--rw-rw-rw-   0 root         (0) root         (0)    10333 2023-04-24 08:33:47.000000 vja-2.0.0b4/vja/service_command.py
--rw-rw-rw-   0 root         (0) root         (0)     3043 2023-04-24 08:33:47.000000 vja-2.0.0b4/vja/service_query.py
--rw-rw-rw-   0 root         (0) root         (0)      669 2023-04-24 08:33:47.000000 vja-2.0.0b4/vja/task_service.py
--rw-rw-rw-   0 root         (0) root         (0)     2892 2023-04-24 08:33:47.000000 vja-2.0.0b4/vja/urgency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:34:51.204191 vja-2.0.0b4/vja.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8442 2023-04-24 08:34:51.000000 vja-2.0.0b4/vja.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      511 2023-04-24 08:34:51.000000 vja-2.0.0b4/vja.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 08:34:51.000000 vja-2.0.0b4/vja.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-04-24 08:34:51.000000 vja-2.0.0b4/vja.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-04-24 08:34:51.000000 vja-2.0.0b4/vja.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-24 08:34:51.000000 vja-2.0.0b4/vja.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 17:51:35.629927 vja-2.0.0rc1/
+-rw-r--r--   0 root         (0) root         (0)     9315 2023-06-02 17:51:35.629927 vja-2.0.0rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-02 17:51:35.629927 vja-2.0.0rc1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      919 2023-06-02 17:50:45.000000 vja-2.0.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 17:51:35.625927 vja-2.0.0rc1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 17:50:45.000000 vja-2.0.0rc1/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1924 2023-06-02 17:50:45.000000 vja-2.0.0rc1/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2847 2023-06-02 17:50:45.000000 vja-2.0.0rc1/tests/test_basic.py
+-rw-rw-rw-   0 root         (0) root         (0)    10651 2023-06-02 17:50:45.000000 vja-2.0.0rc1/tests/test_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     9483 2023-06-02 17:50:45.000000 vja-2.0.0rc1/tests/test_query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 17:51:35.628927 vja-2.0.0rc1/vja/
+-rwxrwxrwx   0 root         (0) root         (0)      220 2023-06-02 17:50:45.000000 vja-2.0.0rc1/vja/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6583 2023-06-02 17:50:45.000000 vja-2.0.0rc1/vja/apiclient.py
+-rw-rw-rw-   0 root         (0) root         (0)     2777 2023-06-02 17:50:45.000000 vja-2.0.0rc1/vja/authenticate.py
+-rwxrwxrwx   0 root         (0) root         (0)    17954 2023-06-02 17:50:45.000000 vja-2.0.0rc1/vja/cli.py
+-rwxrwxrwx   0 root         (0) root         (0)     1967 2023-06-02 17:50:45.000000 vja-2.0.0rc1/vja/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3830 2023-06-02 17:50:45.000000 vja-2.0.0rc1/vja/filter.py
+-rwxrwxrwx   0 root         (0) root         (0)     5707 2023-06-02 17:50:45.000000 vja-2.0.0rc1/vja/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2961 2023-06-02 17:50:45.000000 vja-2.0.0rc1/vja/output.py
+-rw-rw-rw-   0 root         (0) root         (0)     2637 2023-06-02 17:50:45.000000 vja-2.0.0rc1/vja/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     2727 2023-06-02 17:50:45.000000 vja-2.0.0rc1/vja/project_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    10412 2023-06-02 17:50:45.000000 vja-2.0.0rc1/vja/service_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     2929 2023-06-02 17:50:45.000000 vja-2.0.0rc1/vja/service_query.py
+-rw-rw-rw-   0 root         (0) root         (0)      690 2023-06-02 17:50:45.000000 vja-2.0.0rc1/vja/task_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     2892 2023-06-02 17:50:45.000000 vja-2.0.0rc1/vja/urgency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 17:51:35.629927 vja-2.0.0rc1/vja.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9315 2023-06-02 17:51:35.000000 vja-2.0.0rc1/vja.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      514 2023-06-02 17:51:35.000000 vja-2.0.0rc1/vja.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 17:51:35.000000 vja-2.0.0rc1/vja.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-02 17:51:35.000000 vja-2.0.0rc1/vja.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-06-02 17:51:35.000000 vja-2.0.0rc1/vja.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-02 17:51:35.000000 vja-2.0.0rc1/vja.egg-info/top_level.txt
```

### Comparing `vja-2.0.0b4/PKG-INFO` & `vja-2.0.0rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vja
-Version: 2.0.0b4
+Version: 2.0.0rc1
 Summary: A simple CLI for Vikunja task manager
 Home-page: https://gitlab.com/ce72/vja
 Author: ce72
 License: UNKNOWN
 Description: # CLI client for Vikunja
         
         [![pypi package version](https://img.shields.io/pypi/v/vja)](https://pypi.org/project/vja/)
@@ -13,14 +13,27 @@
         [![coverage report](https://gitlab.com/ce72/vja/badges/main/coverage.svg)](https://gitlab.com/ce72/vja/commits/main)
         
         This is a simple CLI for Vikunja > [The todo app to organize your life.](https://vikunja.io/)
         
         It provides a command line interface for adding, viewing and editing todo tasks on a Vikunja Server.
         The goal is to support a command line based task workflow ~ similar to taskwarrior.
         
+        > #### Breaking changes in vja 2.0
+        > vja 2.0 supports (and requires) the most recent Vikunja API > 0.20.4.
+        > In the wake of this transition the following breaking modifications to the vja command line interface have been
+        > introduced:
+        > - Labels: Are now given with `-l` (`-label`). (`-t` and `--tag` are no longer supported).
+        > - "Namespaces": Vikunja removed namespaces in favor of nested projects. `-n` (`--namespace`) was removed as option
+            from `vja ls`.
+        > - Projects (former "lists"): Must be given with `-o` (`--project`). `vja ls -u` may be used to filter on the project
+            or an upper project. This more or less resembles the old namespaces.
+        >
+        > Examples and more details can be found in the
+        > updated [Features.md](https://gitlab.com/ce72/vja/-/blob/main/Features.md)
+        
         ## Installation
         
         - Install from pypi:
           ```shell
           pip install vja
           vja --help
           ```
@@ -38,16 +51,16 @@
           [application]
           frontend_url=https://try.vikunja.io/
           api_url=https://try.vikunja.io/api/v1
           ```
           (If you cloned from git, you may copy the folder .vjacli to your `$HOME` directory instead.)
         - Adjust to your needs.
           `frontend_url` and `api_url` must point to your own Vikunja server.
-          Especially, the api_url must be reachable from your client. This can be verified, for example
-          by `curl https://mydomain.com/api/v1/info`
+          Especially, the api_url must be reachable from your client. This can be verified, for example,
+          by `curl https://mydomain.com/api/v1/info`.
         
         You may change the location of the configuration directory with an environment variable
         like `VJA_CONFIGDIR=/not/my/home`
         
         ### Description of configuration
         
         #### Required options
@@ -111,15 +124,14 @@
         # pip uninstall -y vja;rm -rf build dist vja.egg-info; python setup.py sdist bdist_wheel; pip install dist/*.whl;
         ```
         
         Run integration test (requires docker and docker-compose)
         
         ```shell
         docker-compose -f tests/docker-compose.yml up -d
-        ./run.sh
         VJA_CONFIGDIR=tests/.vjatest pytest
         docker-compose -f tests/docker-compose.yml down
         ```
         
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `vja-2.0.0b4/setup.py` & `vja-2.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b4/tests/conftest.py` & `vja-2.0.0rc1/tests/conftest.py`

 * *Files 23% similar despite different names*

```diff
@@ -32,15 +32,18 @@
 def _login_as_test_user():
     run_vja('vja logout')
     run_vja('vja --username=test --password=test user show')
 
 
 def _create_project_and_task():
     run_vja('vja project add test-project')
-    run_vja('vja add At least one task --force-create --priority=5 --due-date=today --tag=my_tag --favorite=True')
+    run_vja('vja project add child --parent-project-id=1')
+    run_vja('vja project add grand-child --parent-project-id=2')
+    run_vja('vja add At least one task --force-create --priority=5 --due-date=today --label=my_tag --favorite=True --project-id=1')
+    run_vja('vja add Task in subproject --force-create --project-id=3')
     run_vja('vja add A task without a label --force-create')
 
 
 def run_vja(command):
     result = subprocess.run(command.split(), capture_output=True, check=False)
     if result.returncode:
         print(f'!!! Non-zero result ({result.returncode}) from command {command}')
```

### Comparing `vja-2.0.0b4/tests/test_basic.py` & `vja-2.0.0rc1/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b4/tests/test_command.py` & `vja-2.0.0rc1/tests/test_command.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,20 +2,24 @@
 import json
 import re
 
 from tests.conftest import invoke
 from vja.cli import cli
 
 ADD_SUCCESS_PATTERN = re.compile(r'.*Created task (\d+) in project .*')
-DATE_1 = datetime.datetime(2023, 3, 30, 15, 0, 0, 0)
+TODAY = datetime.datetime.now().replace(microsecond=0)
+TODAY_ISO = TODAY.isoformat()
+YESTERDAY = TODAY + datetime.timedelta(days=-1)
+YESTERDAY_ISO = YESTERDAY.isoformat()
+TOMORROW = TODAY + datetime.timedelta(days=1)
+TOMORROW_ISO = TOMORROW.isoformat()
+DATE_1 = TODAY + datetime.timedelta(days=10)
 DATE_2 = DATE_1 + datetime.timedelta(days=1)
 DATE_1_ISO = DATE_1.isoformat()
 DATE_2_ISO = DATE_2.isoformat()
-TODAY = datetime.datetime.now()
-TODAY_ISO = TODAY.isoformat()
 
 
 class TestAddTask:
     def test_project_id(self, runner):
         res = invoke(runner, 'add title of new task --force --project=1')
         after = json_for_created_task(runner, res.output)
         assert after['project']['id'] == 1
@@ -63,51 +67,54 @@
         assert after['bucket_id'] == before['bucket_id']
 
 
 class TestEditGeneral:
     def test_edit_title(self, runner):
         before = json_for_task_id(runner, 1)
         new_title = f'{before["title"]}42'
-        res = runner.invoke(cli, ['edit', '1', '-i', f'{new_title}'])
-        assert res.exit_code == 0, res
+        invoke(runner, ['edit', '1', '-i', f'{new_title}'])
 
         after = json_for_task_id(runner, 1)
         assert after['title'] == new_title
         assert after['updated'] > before['updated']
         # other attributes remain in place
         assert after['due_date'] == before['due_date']
         assert after['reminders'] == before['reminders']
         assert after['position'] == before['position']
         assert after['project']['id'] == before['project']['id']
         assert after['created'] == before['created']
 
-    def test_edit_due_date(self, runner):
-        before = json_for_task_id(runner, 1)
+    def test_edit_due_date_without_time(self, runner):
 
-        invoke(runner, 'edit 1 --due=today')
+        invoke(runner, 'edit 1 --due=tomorrow')
 
         after = json_for_task_id(runner, 1)
-        assert after['due_date'][:10] == TODAY_ISO[:10]
-        assert after['updated'] >= before['updated']
+        assert after['due_date'] == (TOMORROW.replace(hour=0, minute=0, second=0)).isoformat()
+
+    def test_edit_due_date_with_time(self, runner):
+
+        invoke(runner, ['edit', '1', '--due=tomorrow 15:00'])
+
+        after = json_for_task_id(runner, 1)
+        assert after['due_date'] == (TOMORROW.replace(hour=15, minute=0, second=0)).isoformat()
 
     def test_unset_due_date(self, runner):
         before = json_for_task_id(runner, 1)
         assert before['due_date'] is not None
 
         invoke(runner, 'edit 1 --due-date=')
 
         after = json_for_task_id(runner, 1)
         assert after['due_date'] is None
-        assert after['updated'] >= before['updated']
 
     def test_toggle_label(self, runner):
         labels_0 = json_for_task_id(runner, 1)['labels']
-        invoke(runner, 'edit 1 --tag=tag1 --force-create')
+        invoke(runner, 'edit 1 --label=tag1 --force-create')
         labels_1 = json_for_task_id(runner, 1)['labels']
-        invoke(runner, 'edit 1 --tag=tag1')
+        invoke(runner, 'edit 1 --label=tag1')
         labels_2 = json_for_task_id(runner, 1)['labels']
 
         assert labels_0 != labels_1
         assert labels_0 == labels_2
         assert self._has_label_with_title(labels_0, 'tag1') or self._has_label_with_title(labels_1, 'tag1')
 
     def test_append_note(self, runner):
@@ -119,15 +126,15 @@
         assert note_1 == 'line1'
         assert note_2 == 'line1\nline2'
 
     def test_edit_project(self, runner):
         invoke(runner, 'project add another project')
         invoke(runner, 'edit 1 --project-id=1')
         project_1 = json_for_task_id(runner, 1)['project']['id']
-        invoke(runner, 'edit 1 -l 2')
+        invoke(runner, 'edit 1 -o 2')
         project_2 = json_for_task_id(runner, 1)['project']['id']
 
         assert project_1 == 1
         assert project_2 == 2
 
     @staticmethod
     def _has_label_with_title(labels, title):
@@ -215,24 +222,31 @@
 
         invoke(runner, 'defer 2 1d')
 
         after = json_for_task_id(runner, 2)
         assert after['due_date'] == DATE_2_ISO
         assert after['reminders'][0]['reminder'] == DATE_2_ISO
 
-    def test_dont_modify_relative_reminder(self, runner):
+    def test_dont_defer_relative_reminder(self, runner):
         invoke(runner, f'edit 2 --due-date={DATE_1_ISO} -r')
 
         invoke(runner, 'defer 2 1d')
 
         after = json_for_task_id(runner, 2)
         assert after['due_date'] == DATE_2_ISO
         assert after['reminders'][0]['relative_period'] == 0
         assert after['reminders'][0]['relative_to'] == 'due_date'
 
+    def test_defer_past_due_realtive_to_now(self, runner):
+        invoke(runner, f'edit 2 --due-date={YESTERDAY_ISO}')
+
+        invoke(runner, 'defer 2 1d')
+
+        after = json_for_task_id(runner, 2)
+        assert after['due_date'][:10] == TOMORROW_ISO[:10]
 
 class TestMultipleTasks:
     def test_edit_three_tasks(self, runner):
         invoke(runner, 'edit 1 2 3 --priority=4')
         for i in range(1, 4):
             after = json_for_task_id(runner, i)
             assert after['priority'] == 4
```

### Comparing `vja-2.0.0b4/tests/test_query.py` & `vja-2.0.0rc1/tests/test_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     def test_project_show(self, runner):
         res = invoke(runner, 'project show 1')
         assert len(res.output) > 0
 
     def test_project_ls_custom_format(self, runner):
         res = invoke(runner, 'project ls --custom-format=ids_only')
         for line in res.output:
-            assert re.match(r'^\d*$', line)
+            assert re.match(r'^-?\d*$', line)
 
 
 class TestBucket:
     def test_bucket_ls(self, runner):
         res = invoke(runner, 'bucket ls --project-id=1')
         assert re.search(r'Backlog', res.output)
 
@@ -143,15 +143,15 @@
         assert all(i['is_favorite'] for i in data)
 
     def test_task_filter_label(self, runner):
         res = invoke(runner, ['ls', '--jsonvja', '--label=my_tag'])
         data = json.loads(res.output)
         assert len(data) > 0
         assert data[0]['labels'][0]['title'] == 'my_tag'
-        res = invoke(runner, ['ls', '--jsonvja', '--label=Not created'])
+        res = invoke(runner, ['ls', '--jsonvja', '--label=unknown_label'])
         data = json.loads(res.output)
         assert len(data) == 0
 
     def test_task_filter_label_empty(self, runner):
         res = invoke(runner, ['ls', '--jsonvja', '--label='''''''])
         data = json.loads(res.output)
         assert len(data) > 0
@@ -194,31 +194,45 @@
         assert len(data) > 0
         assert all(i['urgency'] >= 10 for i in data)
         res = invoke(runner, ['ls', '--jsonvja', '--urgency=10000'])
         data = json.loads(res.output)
         assert len(data) == 0
 
     def test_task_filter_general(self, runner):
-        res = invoke(runner, ['ls', '--jsonvja', '--filter=title contains At least one'])
-        assert len(json.loads(res.output)) > 0
-        res = invoke(runner, ['ls', '--jsonvja', '--filter=title contains TASK_NOT_CREATED'])
-        assert len(json.loads(res.output)) == 0
-        res = invoke(runner, ['ls', '--jsonvja', '--filter=priority gt 2'])
-        assert len(json.loads(res.output)) > 0
-        res = invoke(runner, ['ls', '--jsonvja', '--filter=priority gt 5'])
-        assert len(json.loads(res.output)) == 0
         res = invoke(runner, ['ls', '--jsonvja', '--filter=due_date after 2 days ago'])
         assert len(json.loads(res.output)) > 0
         res = invoke(runner, ['ls', '--jsonvja', '--filter=due_date after 200 days'])
         assert len(json.loads(res.output)) == 0
         res = invoke(runner, ['ls', '--jsonvja', '--filter=due_date after 200 days'])
         assert len(json.loads(res.output)) == 0
         res = invoke(runner, ['ls', '--jsonvja', '--filter=is_favorite eq True'])
         data = json.loads(res.output)
         assert len(data) > 0
         assert all(i['is_favorite'] for i in data)
+        res = invoke(runner, ['ls', '--jsonvja', '--filter=priority gt 2'])
+        assert len(json.loads(res.output)) > 0
+        res = invoke(runner, ['ls', '--jsonvja', '--filter=priority gt 5'])
+        assert len(json.loads(res.output)) == 0
+        res = invoke(runner, ['ls', '--jsonvja', '--filter=title contains At least one'])
+        assert len(json.loads(res.output)) > 0
+        res = invoke(runner, ['ls', '--jsonvja', '--filter=title contains TASK_NOT_CREATED'])
+        assert len(json.loads(res.output)) == 0
+
+    def test_task_filter_general_label(self, runner):
+        res = invoke(runner, ['ls', '--json', '--filter=label_titles contains my_tag'])
+        data = json.loads(res.output)
+        assert len(data) > 0
+        assert all('my_tag' in _labels_from_task_json(task) for task in data)
+        res = invoke(runner, ['ls', '--jsonvja', '--filter=label_titles ne my_tag'])
+        data = json.loads(res.output)
+        assert len(data) > 0
+        assert all('my_tag' not in _labels_from_task_json(task) for task in data)
 
     def test_task_filter_general_combined(self, runner):
         res = invoke(runner, ['ls', '--jsonvja', '--filter=id gt 0', '--filter=id lt 2'])
         data = json.loads(res.output)
         assert len(data) == 1
         assert all(i['id'] == 1 for i in data)
+
+
+def _labels_from_task_json(task):
+    return ' '.join(map(lambda label: label['title'], task['labels'] or []))
```

### Comparing `vja-2.0.0b4/vja/apiclient.py` & `vja-2.0.0rc1/vja/apiclient.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     return wrapper
 
 
 class ApiClient:
     def __init__(self, api_url, token_file):
         logger.debug('Connecting to api_url %s', api_url)
         self._api_url = api_url
-        self._cache = {'projects': None, 'labels': None, 'namespaces': None, 'tasks': None}
+        self._cache = {'projects': None, 'labels': None, 'tasks': None}
         self._login = Login(api_url, token_file)
 
     def _create_url(self, path):
         return self._api_url + path
 
     @handle_http_error
     @inject_access_token
@@ -107,30 +107,25 @@
 
     def logout(self):
         self._login.logout()
 
     def get_user(self):
         return self._get_json(self._create_url('/user'))
 
-    def get_namespaces(self):
-        if self._cache['namespaces'] is None:
-            self._cache['namespaces'] = self._get_json(self._create_url('/namespaces')) or []
-        return self._cache['namespaces']
-
     def get_projects(self):
         if self._cache['projects'] is None:
             self._cache['projects'] = self._get_json(self._create_url('/projects')) or []
         return self._cache['projects']
 
     def get_project(self, project_id):
         return self._get_json(self._create_url(f'/projects/{str(project_id)}'))
 
-    def put_project(self, namespace_id, title):
-        payload = {'title': title}
-        return self._put_json(self._create_url(f'/namespaces/{str(namespace_id)}/projects'), payload=payload)
+    def put_project(self, parent_project_id, title):
+        payload = {'title': title, 'parent_project_id': parent_project_id}
+        return self._put_json(self._create_url('/projects'), payload=payload)
 
     def get_buckets(self, project_id):
         return self._get_json(self._create_url(f'/projects/{str(project_id)}/buckets'))
 
     def get_labels(self):
         if self._cache['labels'] is None:
             self._cache['labels'] = self._get_json(self._create_url('/labels')) or []
```

### Comparing `vja-2.0.0b4/vja/authenticate.py` & `vja-2.0.0rc1/vja/authenticate.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b4/vja/cli.py` & `vja-2.0.0rc1/vja/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,33 +5,33 @@
 from importlib import metadata
 
 import click
 from click_aliases import ClickAliasedGroup
 
 from vja.apiclient import ApiClient
 from vja.config import VjaConfiguration
-from vja.list_service import ListService
 from vja.output import Output
+from vja.project_service import ProjectService
 from vja.service_command import CommandService
 from vja.service_query import QueryService
 from vja.task_service import TaskService
 from vja.urgency import Urgency
 
 logger = logging.getLogger(__name__)
 
 
 class Application:
     def __init__(self):
         self._configuration = VjaConfiguration()
         api_client = ApiClient(self._configuration.get_api_url(), self._configuration.get_token_file())
-        list_service = ListService(api_client)
+        project_service = ProjectService(api_client)
         urgency_service = Urgency.from_config(self._configuration)
-        task_service = TaskService(list_service, urgency_service)
-        self._command_service = CommandService(list_service, task_service, api_client)
-        self._query_service = QueryService(list_service, task_service, api_client)
+        task_service = TaskService(project_service, urgency_service)
+        self._command_service = CommandService(project_service, task_service, api_client)
+        self._query_service = QueryService(project_service, task_service, api_client)
         self._output = Output()
 
     @property
     def command_service(self) -> CommandService:
         return self._command_service
 
     @property
@@ -96,23 +96,24 @@
 # projects
 @cli.group('project', help='Subcommand: project (see help)')
 def project_group():
     pass
 
 
 @project_group.command('add', help='Add project with title')
-@click.option('namespace_id', '-n', '--namespace-id', help='Create project in namespace, default: first namespace found')
+@click.option('parent_project_id', '-o', '--parent-project-id', '--parent_project_id', type=click.INT,
+              help='Create project as child of parent project id')
 @click.argument('title', nargs=-1, required=True)
 @with_application
-def project_add(application, title, namespace_id=None):
-    project = application.command_service.add_project(namespace_id, " ".join(title))
+def project_add(application, title, parent_project_id=None):
+    project = application.command_service.add_project(parent_project_id, " ".join(title))
     click.echo(f'Created project {project.id}')
 
 
-@project_group.command('ls', help='Print projects ... (id; title; description; namespace; namespace_id)')
+@project_group.command('ls', help='Print projects ... (id; title; description; parent_project_id)')
 @click.option('is_json', '--json', default=False, is_flag=True,
               help='Print as Vikunja json')
 @click.option('is_jsonvja', '--jsonvja', default=False, is_flag=True,
               help='Print as vja application json')
 @click.option('custom_format', '--custom-format',
               help='Format with template from .vjacli/vja.rc')
 @with_application
@@ -138,15 +139,15 @@
 # buckets
 @cli.group('bucket', help='Subcommand: kanban buckets (see help)')
 def bucket_group():
     pass
 
 
 @bucket_group.command('ls', help='Print kanban buckets of given project ... (id; title; is_done; limit; count tasks)')
-@click.option('project_id', '-l', '--list', '--project-id', '--project_id', required=True, type=click.INT,
+@click.option('project_id', '-o', '--project', '--project-id', '--project_id', required=True, type=click.INT,
               help='Show buckets of project with id')
 @click.option('is_json', '--json', default=False, is_flag=True,
               help='Print as Vikunja json')
 @click.option('is_jsonvja', '--jsonvja', default=False, is_flag=True,
               help='Print as vja application json')
 @click.option('custom_format', '--custom-format',
               help='Format with template from .vjacli/vja.rc')
@@ -187,25 +188,25 @@
     click.echo(f'Created label {label.id}')
 
 
 # tasks
 @cli.command('add', aliases=['create'],
              help='Add new task')
 @click.argument('title', required=True, nargs=-1)
-@click.option('project_id', '-l', '--folder', '--project', '--list',
+@click.option('project_id', '-o', '--project', '--project-id', '--project_id',
               help='Project (id or name), defaults to project from user settings, than to first favorite project')
 @click.option('note', '-n', '--note', '--description',
               help='Set description (note)')
 @click.option('prio', '-p', '--prio', '--priority',
               help='Set priority')
 @click.option('due', '-d', '--due', '--duedate', '--due-date', '--due_date',
               help='Set due date (supports parsedatetime expressions)')
 @click.option('favorite', '-f', '--star', '--favorite', type=click.BOOL,
               help='Mark as favorite')
-@click.option('tag', '-t', '--tag', '--label',
+@click.option('label', '-l', '--label',
               help='Set label (label must exist on server)')
 @click.option('reminder', '-r', '--alarm', '--remind', '--reminder', is_flag=False, flag_value='due',
               help='Set reminder (supports parsedatetime and timedelta expressions). '
                    'Absolute: "in 3 days at 18:00" or relative: "1h before due_date" or just -r to set equal to '
                    'due date.')
 @click.option('force_create', '--force-create', '--force', is_flag=True,
               help='Force creation of non existing label')
@@ -239,29 +240,29 @@
               help='Set title')
 @click.option('note', '-n', '--note', '--description',
               help='Set description (note)')
 @click.option('note_append', '-a', '--note-append', '--append-note', '--description-append', '--append-description',
               help='Append note to existing description separated by new line')
 @click.option('prio', '-p', '--prio', '--priority', type=click.INT,
               help='Set priority')
-@click.option('project_id', '-l', '--folder-id', '--project-id', '--list-id', '--project_id', type=click.INT,
+@click.option('project_id', '-o', '--project', '--project-id', '--project_id',
               help='Move to project with id')
 @click.option('position', '--project-position', '--project_position', '--position', type=click.INT,
               help='Set project position')
 @click.option('bucket_id', '--bucket-id', '--bucket_id', type=click.INT,
               help='Set bucket id')
 @click.option('kanban_position', '--kanban-position', '--kanban_position', type=click.INT,
               help='Set kanban position')
 @click.option('due', '-d', '--due', '--duedate', '--due-date', '--due_date',
               help='Set due date (supports parsedatetime expressions)')
 @click.option('favorite', '-f', '--favorite', '--star', type=click.BOOL,
               help='Mark as favorite')
 @click.option('completed', '-c', '--completed', '--done', type=click.BOOL,
               help='Mark as completed')
-@click.option('tag', '-t', '--tag', '--label',
+@click.option('label', '-l', '--label',
               help='Set label (label must exist on server unless called with --force-create)')
 @click.option('reminder', '-r', '--alarm', '--remind', '--reminder', is_flag=False, flag_value='due',
               help='Set reminder (supports parsedatetime and timedelta expressions). '
                    'Absolute: "in 3 days at 18:00" or relative: "1h30m before due_date" or just -r to set equal to '
                    'due date.')
 @click.option('force_create', '--force-create', '--force', is_flag=True, default=None,
               help='Force creation of non existing label')
@@ -298,15 +299,15 @@
     for task_id in task_ids:
         task = application.command_service.defer_task(task_id, delay_by)
         click.echo(f'Modified task {task.id} in project {task.project.id}')
         ctx.invoke(task_show, tasks=[task_id])
 
 
 @cli.command('ls', help='List tasks ... (task-id; priority; is_favorite; title; due_date; '
-                        'has reminder; namespace; project; labels; urgency)')
+                        'has reminder; parent-project; project; labels; urgency)')
 @click.option('is_json', '--json', default=False, is_flag=True,
               help='Print as Vikunja json')
 @click.option('is_jsonvja', '--jsonvja', default=False, is_flag=True,
               help='Print as vja application json')
 @click.option('custom_format', '--custom-format',
               help='Format with template from .vjacli/vja.rc')
 @click.option('sort_string', '--sort', '--sort-by', '--sort-string',
@@ -321,26 +322,27 @@
                    'Shortcut for --filter="due_date <operator> <value>"')
 @click.option('favorite_filter', '-f', '--favorite', '--star', type=click.BOOL,
               help='Filter by favorite flag. Shortcut for --filter="favorite_filter eq <value>"')
 @click.option('general_filter', '--filter', multiple=True,
               help='General filter. Must be like <field> <operator> <value> e.g. --filter="priority ge 2" '
                    'where <operator> in (eq, ne, gt, lt, ge, le, before, after, contains). '
                    'Multiple occurrences of --filter are allowed and will be combined with logical AND.')
-@click.option('label_filter', '-t', '--tag', '--label',
+@click.option('label_filter', '-l', '--label',
               help='Filter by label (name or id)')
-@click.option('project_filter', '-l', '--project',
+@click.option('project_filter', '-o', '--project', '--project-id', '--project_id',
               help='Filter by project (name or id)')
-@click.option('namespace_filter', '-n', '--namespace',
-              help='Filter by namespace (name or id)')
+@click.option('upper_project_filter', '-u', '--base-project', '--base', '--upper-project',
+              help='Filter by base project (name or id). '
+                   'All tasks whose project has the given argument as a ancestor are considered.')
 @click.option('priority_filter', '-p', '--prio', '--priority',
               help='Filter by priority. The TEXT value must be like <operator> <value>, '
                    'Shortcut for --filter="priority <operator> <value>"')
 @click.option('title_filter', '-i', '--title',
               help='Filter title (regex)')
-@click.option('urgency_filter', '-u', '--urgency', is_flag=False, flag_value=3, type=click.INT,
+@click.option('urgency_filter', '-u', '--urgent', '--urgency', is_flag=False, flag_value=3, type=click.INT,
               help='Filter by minimum urgency.  Shortcut for --filter="urgency ge <value>"')
 @with_application
 def task_ls(application, is_json, is_jsonvja, custom_format, include_completed, sort_string=None, **filter_args):
     if custom_format:
         custom_format = application.configuration.get_custom_format_string(custom_format)
     filter_args = {k: v for k, v in filter_args.items() if v is not None}
```

### Comparing `vja-2.0.0b4/vja/config.py` & `vja-2.0.0rc1/vja/config.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b4/vja/filter.py` & `vja-2.0.0rc1/vja/filter.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 
 def _create_single_general_filter(value: str):
     arguments = value.split(" ", 2)
     field = arguments[0]
     operation = _operators[arguments[1]]
     value = arguments[2]
-    logger.debug("filter %s: %s %s", field, operation.__name__, value)
+    logger.debug("general filter %s: %s %s", field, operation.__name__, value)
     return lambda x: _general_filter(x, field, operation, value)
 
 
 def _general_filter(task, field_name, operation, value):
     task_value = rgetattr(task, field_name)
     if task_value is not None:
         if isinstance(task_value, datetime):
@@ -65,18 +65,18 @@
 
 def _create_project_filter(value):
     if str(value).isdigit():
         return _create_general_filter([f'project.id eq {value}'])
     return _create_general_filter([f'project.title eq {value}'])
 
 
-def _create_namespace_filter(value):
+def _create_upper_project_filter(value):
     if str(value).isdigit():
-        return _create_general_filter([f'project.namespace.id eq {value}'])
-    return _create_general_filter([f'project.namespace.title eq {value}'])
+        return lambda x: x.id == int(value) or any(ancestor.id == int(value) for ancestor in x.ancestor_projects)
+    return lambda x: x.title == value or any(ancestor.title == int(value) for ancestor in x.ancestor_projects)
 
 
 def _create_title_filter(value):
     return lambda x: bool(re.search(re.compile(value), x.title))
 
 
 def _create_priority_filter(value):
@@ -102,15 +102,15 @@
 _filter_mapping = {
     'bucket_filter': _create_bucket_filter,
     'due_date_filter': _create_due_date_filter,
     'favorite_filter': _create_favorite_filter,
     'general_filter': _create_general_filter,
     'label_filter': _create_label_filter,
     'project_filter': _create_project_filter,
-    'namespace_filter': _create_namespace_filter,
+    'upper_project_filter': _create_upper_project_filter,
     'title_filter': _create_title_filter,
     'priority_filter': _create_priority_filter,
     'urgency_filter': _create_urgency_filter,
 }
 
 
 def create_filters(filter_args):
```

### Comparing `vja-2.0.0b4/vja/list_service.py` & `vja-2.0.0rc1/vja/project_service.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,22 @@
 import logging
 from typing import Optional
 
 from vja import VjaError
 from vja.apiclient import ApiClient
-from vja.model import Namespace, Project, User
+from vja.model import Project, User
 
 logger = logging.getLogger(__name__)
 
 
-class ListService:
+class ProjectService:
     def __init__(self, api_client: ApiClient):
         self._api_client = api_client
-        self._namespace_by_id: Optional[dict] = None
         self._project_by_id: Optional[dict] = None
 
-    def find_namespace_by_id(self, namespace_id: int) -> Namespace:
-        if not self._namespace_by_id:
-            self._namespace_by_id = {x['id']: Namespace.from_json(x) for x in self._api_client.get_namespaces()}
-        namespace_object = self._namespace_by_id.get(namespace_id)
-        if not namespace_object:
-            logger.warning(
-                'Inconsistent data: namespace_id %s is referring to non existing cached Namespace.', str(namespace_id))
-        return namespace_object
-
     def find_project_by_id(self, project_id: int) -> Project:
         if not self._project_by_id:
             self._project_by_id = {x['id']: self.convert_project_json(x) for x in self._api_client.get_projects()}
         return self._project_by_id.get(project_id)
 
     def find_project_by_title(self, title):
         project_objects = [self.convert_project_json(x) for x in self._api_client.get_projects()]
@@ -49,9 +39,22 @@
             if favorite_projects:
                 project_found = favorite_projects[0]
             else:
                 project_found = project_objects[0]
         return project_found
 
     def convert_project_json(self, project_json: dict) -> Project:
-        namespace = self.find_namespace_by_id(project_json['namespace_id'])
-        return Project.from_json(project_json, namespace)
+        ancestor_projects = []
+        # project_id = project_json['id']
+        # parent_project_id = project_json['parent_project_id']
+        # if parent_project_id != id find parent and add it to the ancestors and proceed with parent the same way
+        # ancestor = self.get_ancestor_project(project_id, parent_project_id)
+        # while ancestor:
+        #     ancestor_projects.append(ancestor)
+        #     ancestor = self.get_ancestor_project(ancestor.id, ancestor.parent_project_id)
+        return Project.from_json(project_json, ancestor_projects)
+
+    def get_ancestor_project(self, project_id, parent_project_id) -> Optional[Project]:
+        if project_id == parent_project_id or parent_project_id == 0 or project_id == 0:
+            return None
+        ancestor = self.find_project_by_id(parent_project_id)
+        return ancestor
```

### Comparing `vja-2.0.0b4/vja/model.py` & `vja-2.0.0rc1/vja/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,49 +56,33 @@
     @classmethod
     def from_json(cls, json):
         return cls(json, json['id'], json['username'], json['name'], json['settings']['default_project_id'])
 
 
 @dataclass(frozen=True)
 @data_dict
-class Namespace:
-    json: dict = field(repr=False)
-    id: int
-    title: str
-    description: str
-    is_archived: bool
-
-    @classmethod
-    def from_json(cls, json):
-        return cls(json, json['id'], json['title'], json['description'], json['is_archived'])
-
-    @classmethod
-    def from_json_array(cls, json_array):
-        return [Namespace.from_json(x) for x in json_array or []]
-
-
-@dataclass(frozen=True)
-@data_dict
 class Project:
     json: dict = field(repr=False)
     id: int
     title: str
     description: str
     is_favorite: bool
     is_archived: bool
-    namespace: Namespace
+    parent_project_id: int
+    ancestor_projects: typing.List['Project']
 
     @classmethod
-    def from_json(cls, json, namespace):
+    def from_json(cls, json, ancestor_projects):
         return cls(json, json['id'], json['title'], json['description'], json['is_archived'], json['is_favorite'],
-                   namespace)
+                   json['parent_project_id'],
+                   ancestor_projects)
 
     @classmethod
-    def from_json_array(cls, json_array, namespace):
-        return [Project.from_json(x, namespace) for x in json_array or []]
+    def from_json_array(cls, json_array, ancestor_projects):
+        return [Project.from_json(x, ancestor_projects) for x in json_array or []]
 
 
 @dataclass(frozen=True)
 @data_dict
 class Bucket:
     json: dict = field(repr=False)
     id: int
```

### Comparing `vja-2.0.0b4/vja/output.py` & `vja-2.0.0rc1/vja/output.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import json
 import logging
 
 import click
 
 from vja.model import User, Task, Project
 
-NAMESPACE_LIST_FORMAT_DEFAULT = '{x.id:5} {x.title:20.20} {x.description:20.20}'
-
 PROJECT_LIST_FORMAT_DEFAULT = '{x.id:5} {x.title:20.20} {x.description:20.20}  ' \
-                           '{x.namespace.title:20.20} {x.namespace.id:5}'
+                              '{x.parent_project_id:5} '
 
 BUCKET_LIST_FORMAT_DEFAULT = '{x.id:5} {x.title:20.20} {x.is_done_bucket:2} {x.limit:3} {x.count_tasks:5}'
 
 LABEL_LIST_FORMAT_DEFAULT = '{x.id:5} {x.title:20.20}'
 
 TASK_LIST_FORMAT_DEFAULT = '{x.id:5} ({x.priority}) {"*" if x.is_favorite else " "} {x.title:50.50} ' \
                            '{x.due_date.strftime("%a %d.%m %H:%M") if x.due_date else "":15.15} ' \
@@ -29,18 +27,14 @@
 
     def project(self, project: Project, is_json, is_jsonvja):
         self._dump(project, is_json, is_jsonvja)
 
     def task(self, task: Task, is_json, is_jsonvja):
         self._dump(task, is_json, is_jsonvja)
 
-    def namespace_array(self, object_array, is_json, is_jsonvja, custom_format=None):
-        line_format = custom_format or NAMESPACE_LIST_FORMAT_DEFAULT
-        self._dump_array(object_array, line_format, is_json, is_jsonvja)
-
     def project_array(self, object_array, is_json, is_jsonvja, custom_format=None):
         line_format = custom_format or PROJECT_LIST_FORMAT_DEFAULT
         self._dump_array(object_array, line_format, is_json, is_jsonvja)
 
     def bucket_array(self, object_array, is_json, is_jsonvja, custom_format=None):
         line_format = custom_format or BUCKET_LIST_FORMAT_DEFAULT
         self._dump_array(object_array, line_format, is_json, is_jsonvja)
```

### Comparing `vja-2.0.0b4/vja/parse.py` & `vja-2.0.0rc1/vja/parse.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b4/vja/service_command.py` & `vja-2.0.0rc1/vja/service_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,37 @@
+import datetime
 import logging
 
 from vja import VjaError
 from vja.apiclient import ApiClient
-from vja.list_service import ListService
 from vja.model import Label
 from vja.parse import parse_date_arg_to_iso, parse_json_date, parse_date_arg_to_timedelta, datetime_to_isoformat
+from vja.project_service import ProjectService
 from vja.task_service import TaskService
 
 logger = logging.getLogger(__name__)
 
 
 class CommandService:
-    def __init__(self, list_service: ListService, task_service: TaskService, api_client: ApiClient):
-        self._list_service = list_service
+    def __init__(self, project_service: ProjectService, task_service: TaskService, api_client: ApiClient):
+        self._project_service = project_service
         self._task_service = task_service
         self._api_client = api_client
 
     def login(self, username, password, totp_passcode):
         self._api_client.authenticate(True, username, password, totp_passcode)
 
     def logout(self):
         self._api_client.logout()
         logger.info('Logged out')
 
     # project
-    def add_project(self, namespace_id, title):
-        if not namespace_id:
-            namespaces = self._api_client.get_namespaces()
-            namespace_id = min(namespace['id'] if namespace['id'] > 0 else 99999 for namespace in namespaces)
-        project_json = self._api_client.put_project(namespace_id, title)
-        return self._list_service.convert_project_json(project_json)
+    def add_project(self, parent_project_id, title):
+        project_json = self._api_client.put_project(parent_project_id, title)
+        return self._project_service.convert_project_json(project_json)
 
     # label
     def add_label(self, title):
         label_json = self._api_client.put_label(title)
         return Label.from_json(label_json)
 
     # tasks
@@ -60,31 +58,31 @@
     def add_task(self, title, args: dict):
         args.update({'title': title})
         if args.get('project_id'):
             project_arg = args.pop('project_id')
             if str(project_arg).isdigit():
                 project_id = project_arg
             else:
-                project_id = self._list_service.find_project_by_title(project_arg).id
+                project_id = self._project_service.find_project_by_title(project_arg).id
         else:
-            project_id = self._list_service.get_default_project().id
-        tag_name = args.pop('tag') if args.get('tag') else None
+            project_id = self._project_service.get_default_project().id
+        label_name = args.pop('label') if args.get('label') else None
         is_force = args.pop('force_create') if args.get('force_create') is not None else False
 
         self._parse_reminder_arg(args.get('reminder'), args)
 
         payload = self._args_to_payload(args)
 
         if not is_force:
-            self._validate_add_task(title, tag_name)
+            self._validate_add_task(title, label_name)
         logger.debug('put task: %s', payload)
         task_json = self._api_client.put_task(project_id, payload)
         task = self._task_service.task_from_json(task_json)
 
-        label = self._label_from_name(tag_name, is_force) if tag_name else None
+        label = self._label_from_name(label_name, is_force) if label_name else None
         if label:
             self._api_client.add_label_to_task(task.id, label.id)
         return task
 
     def clone_task(self, task_id: int, title, is_clone_bucket):
         task_remote = self._api_client.get_task(task_id)
         task_remote.update({'id': None})
@@ -102,15 +100,15 @@
 
         for label in task_remote['labels']:
             self._api_client.add_label_to_task(task.id, label['id'])
         return task
 
     def edit_task(self, task_id: int, args: dict):
         task_remote = self._api_client.get_task(task_id)
-        tag_name = args.pop('tag') if args.get('tag') else None
+        label_name = args.pop('label') if args.get('label') else None
         is_force = args.pop('force_create') if args.get('force_create') is not None else False
 
         self._update_reminder(args, task_remote)
         if args.get('note_append'):
             append_note = args.pop('note_append')
             args.update({
                 'note': task_remote['description'] + '\n' + append_note if task_remote['description'] else append_note
@@ -121,15 +119,15 @@
         task_remote.update(payload)
         # make sure we do not send back the old reminder_dates
         task_remote.pop("reminder_dates", None)
         logger.debug('post task: %s', task_remote)
         task_json = self._api_client.post_task(task_id, task_remote)
         task_new = self._task_service.task_from_json(task_json)
 
-        label = self._label_from_name(tag_name, is_force) if tag_name else None
+        label = self._label_from_name(label_name, is_force) if label_name else None
         if label:
             if task_new.has_label(label):
                 self._api_client.remove_label_from_task(task_new.id, label.id)
             else:
                 self._api_client.add_label_to_task(task_new.id, label.id)
         return task_new
 
@@ -184,15 +182,20 @@
     def defer_task(self, task_id, delay_by):
         timedelta = parse_date_arg_to_timedelta(delay_by)
         args = {}
 
         task_remote = self._api_client.get_task(task_id)
         due_date = parse_json_date(task_remote['due_date'])
         if due_date:
-            args.update({'due': datetime_to_isoformat(due_date + timedelta)})
+            now = datetime.datetime.now().replace(microsecond=0)
+            if due_date < now:
+                args.update({'due': datetime_to_isoformat(now + timedelta)})
+            else:
+                args.update({'due': datetime_to_isoformat(due_date + timedelta)})
+
         old_reminders = task_remote['reminders']
         if old_reminders and len(old_reminders) > 0:
             reminder_date = parse_json_date(old_reminders[0]['reminder'])
             is_absolute_reminder = not old_reminders[0]['relative_to']
             if reminder_date and is_absolute_reminder:
                 args.update({'reminder': datetime_to_isoformat(reminder_date + timedelta)})
                 self._update_reminder(args, task_remote)
@@ -213,16 +216,16 @@
         if not label_found:
             if is_force:
                 return Label.from_json(self._api_client.put_label(name))
             logger.warning("Ignoring non existing label [%s]. You may want to execute \"label add\" first.", name)
             return None
         return label_found[0]
 
-    def _validate_add_task(self, title, tag_name):
+    def _validate_add_task(self, title, label_name):
         tasks_remote = self._api_client.get_tasks(exclude_completed=True)
         if any(task for task in tasks_remote if task['title'] == title):
             raise VjaError("Task with title does exist. You may want to run with --force-create.")
-        if tag_name:
+        if label_name:
             labels_remote = Label.from_json_array(self._api_client.get_labels())
-            if not any(label for label in labels_remote if label.title == tag_name):
+            if not any(label for label in labels_remote if label.title == label_name):
                 raise VjaError(
                     "Label does not exist. You may want to execute \"label add\" or run with --force-create.")
```

### Comparing `vja-2.0.0b4/vja/service_query.py` & `vja-2.0.0rc1/vja/service_query.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 import logging
 
 from vja.apiclient import ApiClient
 from vja.filter import create_filters
-from vja.list_service import ListService
-from vja.model import Namespace, Label, User, Bucket
+from vja.model import Label, User, Bucket
 from vja.parse import rgetattr
+from vja.project_service import ProjectService
 from vja.task_service import TaskService
 
 logger = logging.getLogger(__name__)
 DEFAULT_SORT_STRING = 'done, -urgency, due_date, -priority, project.title, title'
 
 
 class QueryService:
-    def __init__(self, list_service: ListService, task_service: TaskService, api_client: ApiClient):
-        self._list_service = list_service
+    def __init__(self, project_service: ProjectService, task_service: TaskService, api_client: ApiClient):
+        self._project_service = project_service
         self._task_service = task_service
         self._api_client = api_client
 
     # user
     def find_current_user(self):
         return User.from_json(self._api_client.get_user())
 
-    # namespace
-    def find_all_namespaces(self):
-        return Namespace.from_json_array(self._api_client.get_namespaces())
-
     # project
     def find_all_projects(self):
-        return [self._list_service.convert_project_json(project_json) for project_json in (self._api_client.get_projects())]
+        return [self._project_service.convert_project_json(project_json) for project_json in
+                (self._api_client.get_projects())]
 
     def find_project_by_id(self, project_id):
-        return self._list_service.convert_project_json(self._api_client.get_project(project_id))
+        return self._project_service.convert_project_json(self._api_client.get_project(project_id))
 
     # bucket
     def find_all_buckets_in_project(self, project_id):
         return Bucket.from_json_array(self._api_client.get_buckets(project_id))
 
     # label
     def find_all_labels(self):
@@ -67,13 +64,13 @@
                     sortable_task_value(x, field) is None, sortable_task_value(x, field)),
                 reverse=sort_field['reverse'])
         return filtered_tasks
 
 
 def sortable_task_value(task, field):
     field_name = field
-    if field in ('label', 'labels', 'tag', 'tags'):
+    if field in ('label', 'labels'):
         field_name = 'label_titles'
     field_value = rgetattr(task, field_name)
     if isinstance(field_value, str):
         return field_value.upper()
     return field_value
```

### Comparing `vja-2.0.0b4/vja/task_service.py` & `vja-2.0.0rc1/vja/task_service.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import logging
 
-from vja.list_service import ListService
 from vja.model import Task, Label
+from vja.project_service import ProjectService
 from vja.urgency import Urgency
 
 logger = logging.getLogger(__name__)
 
 
 class TaskService:
-    def __init__(self, list_service: ListService, urgency: Urgency):
-        self._list_service = list_service
+    def __init__(self, project_service: ProjectService, urgency: Urgency):
+        self._project_service = project_service
         self._urgency = urgency
 
     def task_from_json(self, task_json: dict) -> Task:
-        project_object = self._list_service.find_project_by_id(task_json['project_id'])
+        project_object = self._project_service.find_project_by_id(task_json['project_id'])
         labels = Label.from_json_array(task_json['labels'])
         task = Task.from_json(task_json, project_object, labels)
         task.urgency = self._urgency.compute_for(task)
         return task
```

### Comparing `vja-2.0.0b4/vja/urgency.py` & `vja-2.0.0rc1/vja/urgency.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0b4/vja.egg-info/PKG-INFO` & `vja-2.0.0rc1/vja.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vja
-Version: 2.0.0b4
+Version: 2.0.0rc1
 Summary: A simple CLI for Vikunja task manager
 Home-page: https://gitlab.com/ce72/vja
 Author: ce72
 License: UNKNOWN
 Description: # CLI client for Vikunja
         
         [![pypi package version](https://img.shields.io/pypi/v/vja)](https://pypi.org/project/vja/)
@@ -13,14 +13,27 @@
         [![coverage report](https://gitlab.com/ce72/vja/badges/main/coverage.svg)](https://gitlab.com/ce72/vja/commits/main)
         
         This is a simple CLI for Vikunja > [The todo app to organize your life.](https://vikunja.io/)
         
         It provides a command line interface for adding, viewing and editing todo tasks on a Vikunja Server.
         The goal is to support a command line based task workflow ~ similar to taskwarrior.
         
+        > #### Breaking changes in vja 2.0
+        > vja 2.0 supports (and requires) the most recent Vikunja API > 0.20.4.
+        > In the wake of this transition the following breaking modifications to the vja command line interface have been
+        > introduced:
+        > - Labels: Are now given with `-l` (`-label`). (`-t` and `--tag` are no longer supported).
+        > - "Namespaces": Vikunja removed namespaces in favor of nested projects. `-n` (`--namespace`) was removed as option
+            from `vja ls`.
+        > - Projects (former "lists"): Must be given with `-o` (`--project`). `vja ls -u` may be used to filter on the project
+            or an upper project. This more or less resembles the old namespaces.
+        >
+        > Examples and more details can be found in the
+        > updated [Features.md](https://gitlab.com/ce72/vja/-/blob/main/Features.md)
+        
         ## Installation
         
         - Install from pypi:
           ```shell
           pip install vja
           vja --help
           ```
@@ -38,16 +51,16 @@
           [application]
           frontend_url=https://try.vikunja.io/
           api_url=https://try.vikunja.io/api/v1
           ```
           (If you cloned from git, you may copy the folder .vjacli to your `$HOME` directory instead.)
         - Adjust to your needs.
           `frontend_url` and `api_url` must point to your own Vikunja server.
-          Especially, the api_url must be reachable from your client. This can be verified, for example
-          by `curl https://mydomain.com/api/v1/info`
+          Especially, the api_url must be reachable from your client. This can be verified, for example,
+          by `curl https://mydomain.com/api/v1/info`.
         
         You may change the location of the configuration directory with an environment variable
         like `VJA_CONFIGDIR=/not/my/home`
         
         ### Description of configuration
         
         #### Required options
@@ -111,15 +124,14 @@
         # pip uninstall -y vja;rm -rf build dist vja.egg-info; python setup.py sdist bdist_wheel; pip install dist/*.whl;
         ```
         
         Run integration test (requires docker and docker-compose)
         
         ```shell
         docker-compose -f tests/docker-compose.yml up -d
-        ./run.sh
         VJA_CONFIGDIR=tests/.vjatest pytest
         docker-compose -f tests/docker-compose.yml down
         ```
         
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

