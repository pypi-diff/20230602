# Comparing `tmp/vja-2.0.0rc1.tar.gz` & `tmp/vja-2.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vja-2.0.0rc1.tar", last modified: Fri Jun  2 17:51:35 2023, max compression
+gzip compressed data, was "vja-2.0.0rc2.tar", last modified: Fri Jun  2 20:48:02 2023, max compression
```

## Comparing `vja-2.0.0rc1.tar` & `vja-2.0.0rc2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 17:51:35.629927 vja-2.0.0rc1/
--rw-r--r--   0 root         (0) root         (0)     9315 2023-06-02 17:51:35.629927 vja-2.0.0rc1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-02 17:51:35.629927 vja-2.0.0rc1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      919 2023-06-02 17:50:45.000000 vja-2.0.0rc1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 17:51:35.625927 vja-2.0.0rc1/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 17:50:45.000000 vja-2.0.0rc1/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1924 2023-06-02 17:50:45.000000 vja-2.0.0rc1/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     2847 2023-06-02 17:50:45.000000 vja-2.0.0rc1/tests/test_basic.py
--rw-rw-rw-   0 root         (0) root         (0)    10651 2023-06-02 17:50:45.000000 vja-2.0.0rc1/tests/test_command.py
--rw-rw-rw-   0 root         (0) root         (0)     9483 2023-06-02 17:50:45.000000 vja-2.0.0rc1/tests/test_query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 17:51:35.628927 vja-2.0.0rc1/vja/
--rwxrwxrwx   0 root         (0) root         (0)      220 2023-06-02 17:50:45.000000 vja-2.0.0rc1/vja/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6583 2023-06-02 17:50:45.000000 vja-2.0.0rc1/vja/apiclient.py
--rw-rw-rw-   0 root         (0) root         (0)     2777 2023-06-02 17:50:45.000000 vja-2.0.0rc1/vja/authenticate.py
--rwxrwxrwx   0 root         (0) root         (0)    17954 2023-06-02 17:50:45.000000 vja-2.0.0rc1/vja/cli.py
--rwxrwxrwx   0 root         (0) root         (0)     1967 2023-06-02 17:50:45.000000 vja-2.0.0rc1/vja/config.py
--rw-rw-rw-   0 root         (0) root         (0)     3830 2023-06-02 17:50:45.000000 vja-2.0.0rc1/vja/filter.py
--rwxrwxrwx   0 root         (0) root         (0)     5707 2023-06-02 17:50:45.000000 vja-2.0.0rc1/vja/model.py
--rw-rw-rw-   0 root         (0) root         (0)     2961 2023-06-02 17:50:45.000000 vja-2.0.0rc1/vja/output.py
--rw-rw-rw-   0 root         (0) root         (0)     2637 2023-06-02 17:50:45.000000 vja-2.0.0rc1/vja/parse.py
--rw-rw-rw-   0 root         (0) root         (0)     2727 2023-06-02 17:50:45.000000 vja-2.0.0rc1/vja/project_service.py
--rw-rw-rw-   0 root         (0) root         (0)    10412 2023-06-02 17:50:45.000000 vja-2.0.0rc1/vja/service_command.py
--rw-rw-rw-   0 root         (0) root         (0)     2929 2023-06-02 17:50:45.000000 vja-2.0.0rc1/vja/service_query.py
--rw-rw-rw-   0 root         (0) root         (0)      690 2023-06-02 17:50:45.000000 vja-2.0.0rc1/vja/task_service.py
--rw-rw-rw-   0 root         (0) root         (0)     2892 2023-06-02 17:50:45.000000 vja-2.0.0rc1/vja/urgency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 17:51:35.629927 vja-2.0.0rc1/vja.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9315 2023-06-02 17:51:35.000000 vja-2.0.0rc1/vja.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      514 2023-06-02 17:51:35.000000 vja-2.0.0rc1/vja.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 17:51:35.000000 vja-2.0.0rc1/vja.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-06-02 17:51:35.000000 vja-2.0.0rc1/vja.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-06-02 17:51:35.000000 vja-2.0.0rc1/vja.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-02 17:51:35.000000 vja-2.0.0rc1/vja.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 20:48:02.571430 vja-2.0.0rc2/
+-rw-r--r--   0 root         (0) root         (0)     9315 2023-06-02 20:48:02.571430 vja-2.0.0rc2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-02 20:48:02.571430 vja-2.0.0rc2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      919 2023-06-02 20:47:19.000000 vja-2.0.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 20:48:02.568430 vja-2.0.0rc2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 20:47:19.000000 vja-2.0.0rc2/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1924 2023-06-02 20:47:19.000000 vja-2.0.0rc2/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2847 2023-06-02 20:47:19.000000 vja-2.0.0rc2/tests/test_basic.py
+-rw-rw-rw-   0 root         (0) root         (0)    10662 2023-06-02 20:47:19.000000 vja-2.0.0rc2/tests/test_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     9956 2023-06-02 20:47:19.000000 vja-2.0.0rc2/tests/test_query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 20:48:02.570430 vja-2.0.0rc2/vja/
+-rwxrwxrwx   0 root         (0) root         (0)      220 2023-06-02 20:47:19.000000 vja-2.0.0rc2/vja/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6583 2023-06-02 20:47:19.000000 vja-2.0.0rc2/vja/apiclient.py
+-rw-rw-rw-   0 root         (0) root         (0)     2777 2023-06-02 20:47:19.000000 vja-2.0.0rc2/vja/authenticate.py
+-rwxrwxrwx   0 root         (0) root         (0)    17963 2023-06-02 20:47:19.000000 vja-2.0.0rc2/vja/cli.py
+-rwxrwxrwx   0 root         (0) root         (0)     1967 2023-06-02 20:47:19.000000 vja-2.0.0rc2/vja/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3878 2023-06-02 20:47:19.000000 vja-2.0.0rc2/vja/filter.py
+-rwxrwxrwx   0 root         (0) root         (0)     5756 2023-06-02 20:47:19.000000 vja-2.0.0rc2/vja/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2955 2023-06-02 20:47:19.000000 vja-2.0.0rc2/vja/output.py
+-rw-rw-rw-   0 root         (0) root         (0)     2637 2023-06-02 20:47:19.000000 vja-2.0.0rc2/vja/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     2812 2023-06-02 20:47:19.000000 vja-2.0.0rc2/vja/project_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    10416 2023-06-02 20:47:19.000000 vja-2.0.0rc2/vja/service_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     2804 2023-06-02 20:47:19.000000 vja-2.0.0rc2/vja/service_query.py
+-rw-rw-rw-   0 root         (0) root         (0)      690 2023-06-02 20:47:19.000000 vja-2.0.0rc2/vja/task_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     2886 2023-06-02 20:47:19.000000 vja-2.0.0rc2/vja/urgency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 20:48:02.571430 vja-2.0.0rc2/vja.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9315 2023-06-02 20:48:02.000000 vja-2.0.0rc2/vja.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      514 2023-06-02 20:48:02.000000 vja-2.0.0rc2/vja.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 20:48:02.000000 vja-2.0.0rc2/vja.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-02 20:48:02.000000 vja-2.0.0rc2/vja.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-06-02 20:48:02.000000 vja-2.0.0rc2/vja.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-02 20:48:02.000000 vja-2.0.0rc2/vja.egg-info/top_level.txt
```

### Comparing `vja-2.0.0rc1/PKG-INFO` & `vja-2.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vja
-Version: 2.0.0rc1
+Version: 2.0.0rc2
 Summary: A simple CLI for Vikunja task manager
 Home-page: https://gitlab.com/ce72/vja
 Author: ce72
 License: UNKNOWN
 Description: # CLI client for Vikunja
         
         [![pypi package version](https://img.shields.io/pypi/v/vja)](https://pypi.org/project/vja/)
```

### Comparing `vja-2.0.0rc1/setup.py` & `vja-2.0.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc1/tests/conftest.py` & `vja-2.0.0rc2/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,18 +32,18 @@
 def _login_as_test_user():
     run_vja('vja logout')
     run_vja('vja --username=test --password=test user show')
 
 
 def _create_project_and_task():
     run_vja('vja project add test-project')
-    run_vja('vja project add child --parent-project-id=1')
-    run_vja('vja project add grand-child --parent-project-id=2')
+    run_vja('vja project add child --parent-project-id=2')
+    run_vja('vja project add grand-child --parent-project-id=3')
     run_vja('vja add At least one task --force-create --priority=5 --due-date=today --label=my_tag --favorite=True --project-id=1')
-    run_vja('vja add Task in subproject --force-create --project-id=3')
+    run_vja('vja add Task in subproject --force-create --project-id=4')
     run_vja('vja add A task without a label --force-create')
 
 
 def run_vja(command):
     result = subprocess.run(command.split(), capture_output=True, check=False)
     if result.returncode:
         print(f'!!! Non-zero result ({result.returncode}) from command {command}')
```

### Comparing `vja-2.0.0rc1/tests/test_basic.py` & `vja-2.0.0rc2/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc1/tests/test_command.py` & `vja-2.0.0rc2/tests/test_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import datetime
 import json
 import re
 
 from tests.conftest import invoke
-from vja.cli import cli
 
 ADD_SUCCESS_PATTERN = re.compile(r'.*Created task (\d+) in project .*')
 TODAY = datetime.datetime.now().replace(microsecond=0)
 TODAY_ISO = TODAY.isoformat()
 YESTERDAY = TODAY + datetime.timedelta(days=-1)
 YESTERDAY_ISO = YESTERDAY.isoformat()
 TOMORROW = TODAY + datetime.timedelta(days=1)
@@ -47,15 +46,15 @@
 class TestCloneTask:
     def test_clone_task(self, runner):
         before = json_for_task_id(runner, 1)
         res = invoke(runner, 'clone 1 title of new task cloned from 1')
         after = json_for_created_task(runner, res.output)
         assert after['project'] == before['project']
         assert after['due_date'] == before['due_date']
-        assert after['labels'] == before['labels']
+        assert after['label_objects'] == before['label_objects']
         assert after['title'] != before['title']
         assert after['id'] != before['id']
         assert after['created'] != before['created']
         assert after['position'] != before['position']
         assert after['kanban_position'] != before['kanban_position']
 #        assert after['bucket_id'] != before['bucket_id'] # TODO: Need to create a second bucket to test this
 
@@ -103,19 +102,19 @@
 
         invoke(runner, 'edit 1 --due-date=')
 
         after = json_for_task_id(runner, 1)
         assert after['due_date'] is None
 
     def test_toggle_label(self, runner):
-        labels_0 = json_for_task_id(runner, 1)['labels']
+        labels_0 = json_for_task_id(runner, 1)['label_objects']
         invoke(runner, 'edit 1 --label=tag1 --force-create')
-        labels_1 = json_for_task_id(runner, 1)['labels']
+        labels_1 = json_for_task_id(runner, 1)['label_objects']
         invoke(runner, 'edit 1 --label=tag1')
-        labels_2 = json_for_task_id(runner, 1)['labels']
+        labels_2 = json_for_task_id(runner, 1)['label_objects']
 
         assert labels_0 != labels_1
         assert labels_0 == labels_2
         assert self._has_label_with_title(labels_0, 'tag1') or self._has_label_with_title(labels_1, 'tag1')
 
     def test_append_note(self, runner):
         invoke(runner, 'edit 1 --note=line1')
```

### Comparing `vja-2.0.0rc1/tests/test_query.py` & `vja-2.0.0rc2/tests/test_query.py`

 * *Files 5% similar despite different names*

```diff
@@ -142,34 +142,43 @@
         assert len(data) > 0
         assert all(i['is_favorite'] for i in data)
 
     def test_task_filter_label(self, runner):
         res = invoke(runner, ['ls', '--jsonvja', '--label=my_tag'])
         data = json.loads(res.output)
         assert len(data) > 0
-        assert data[0]['labels'][0]['title'] == 'my_tag'
+        assert data[0]['label_objects'][0]['title'] == 'my_tag'
         res = invoke(runner, ['ls', '--jsonvja', '--label=unknown_label'])
         data = json.loads(res.output)
         assert len(data) == 0
 
     def test_task_filter_label_empty(self, runner):
         res = invoke(runner, ['ls', '--jsonvja', '--label='''''''])
         data = json.loads(res.output)
         assert len(data) > 0
-        assert all(len(i['labels']) == 0 for i in data)
+        assert all(len(i['label_objects']) == 0 for i in data)
 
     def test_task_filter_project(self, runner):
         res = invoke(runner, ['ls', '--jsonvja', '--project=test-project'])
         data = json.loads(res.output)
         assert len(data) > 0
         assert all(i['project']['title'] == 'test-project' for i in data)
         res = invoke(runner, ['ls', '--jsonvja', '--project=Not created'])
         data = json.loads(res.output)
         assert len(data) == 0
 
+    def test_task_filter_base_project(self, runner):
+        res = invoke(runner, ['ls', '--jsonvja', '--base-project=test-project'])
+        data = json.loads(res.output)
+        assert len(data) > 0
+        assert all(i['project']['title'] == 'test-project' or i['project']['title'] == 'grand-child' for i in data)
+        res = invoke(runner, ['ls', '--jsonvja', '--project=Not created'])
+        data = json.loads(res.output)
+        assert len(data) == 0
+
     def test_task_filter_priority(self, runner):
         res = invoke(runner, ['ls', '--jsonvja', '--priority=eq 5'])
         data = json.loads(res.output)
         assert len(data) > 0
         assert all(i['priority'] == 5 for i in data)
         res = invoke(runner, ['ls', '--jsonvja', '--priority=gt 4'])
         data = json.loads(res.output)
@@ -214,25 +223,25 @@
         assert len(json.loads(res.output)) == 0
         res = invoke(runner, ['ls', '--jsonvja', '--filter=title contains At least one'])
         assert len(json.loads(res.output)) > 0
         res = invoke(runner, ['ls', '--jsonvja', '--filter=title contains TASK_NOT_CREATED'])
         assert len(json.loads(res.output)) == 0
 
     def test_task_filter_general_label(self, runner):
-        res = invoke(runner, ['ls', '--json', '--filter=label_titles contains my_tag'])
+        res = invoke(runner, ['ls', '--jsonvja', '--filter=labels contains my_tag'])
         data = json.loads(res.output)
         assert len(data) > 0
         assert all('my_tag' in _labels_from_task_json(task) for task in data)
-        res = invoke(runner, ['ls', '--jsonvja', '--filter=label_titles ne my_tag'])
+        res = invoke(runner, ['ls', '--jsonvja', '--filter=labels ne my_tag'])
         data = json.loads(res.output)
         assert len(data) > 0
         assert all('my_tag' not in _labels_from_task_json(task) for task in data)
 
     def test_task_filter_general_combined(self, runner):
         res = invoke(runner, ['ls', '--jsonvja', '--filter=id gt 0', '--filter=id lt 2'])
         data = json.loads(res.output)
         assert len(data) == 1
         assert all(i['id'] == 1 for i in data)
 
 
 def _labels_from_task_json(task):
-    return ' '.join(map(lambda label: label['title'], task['labels'] or []))
+    return ' '.join(map(lambda label: label['title'], task['label_objects'] or []))
```

### Comparing `vja-2.0.0rc1/vja/apiclient.py` & `vja-2.0.0rc2/vja/apiclient.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc1/vja/authenticate.py` & `vja-2.0.0rc2/vja/authenticate.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc1/vja/cli.py` & `vja-2.0.0rc2/vja/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -326,15 +326,15 @@
               help='General filter. Must be like <field> <operator> <value> e.g. --filter="priority ge 2" '
                    'where <operator> in (eq, ne, gt, lt, ge, le, before, after, contains). '
                    'Multiple occurrences of --filter are allowed and will be combined with logical AND.')
 @click.option('label_filter', '-l', '--label',
               help='Filter by label (name or id)')
 @click.option('project_filter', '-o', '--project', '--project-id', '--project_id',
               help='Filter by project (name or id)')
-@click.option('upper_project_filter', '-u', '--base-project', '--base', '--upper-project',
+@click.option('upper_project_filter', '-t', '--base-project', '--top', '--base', '--upper-project',
               help='Filter by base project (name or id). '
                    'All tasks whose project has the given argument as a ancestor are considered.')
 @click.option('priority_filter', '-p', '--prio', '--priority',
               help='Filter by priority. The TEXT value must be like <operator> <value>, '
                    'Shortcut for --filter="priority <operator> <value>"')
 @click.option('title_filter', '-i', '--title',
               help='Filter title (regex)')
```

### Comparing `vja-2.0.0rc1/vja/config.py` & `vja-2.0.0rc2/vja/config.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc1/vja/filter.py` & `vja-2.0.0rc2/vja/filter.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,30 +53,30 @@
 def _create_favorite_filter(value):
     return _create_general_filter([f'is_favorite eq {value}'])
 
 
 def _create_label_filter(value):
     logger.debug("filter labels %s", value)
     if str(value).isdigit():
-        return lambda x: any(label.id == int(value) for label in x.labels)
+        return lambda x: any(label.id == int(value) for label in x.label_objects)
     if str(value).strip() == '':
-        return lambda x: not x.labels
-    return lambda x: any(label.title == value for label in x.labels)
+        return lambda x: not x.label_objects
+    return lambda x: any(label.title == value for label in x.label_objects)
 
 
 def _create_project_filter(value):
     if str(value).isdigit():
         return _create_general_filter([f'project.id eq {value}'])
     return _create_general_filter([f'project.title eq {value}'])
 
 
 def _create_upper_project_filter(value):
     if str(value).isdigit():
-        return lambda x: x.id == int(value) or any(ancestor.id == int(value) for ancestor in x.ancestor_projects)
-    return lambda x: x.title == value or any(ancestor.title == int(value) for ancestor in x.ancestor_projects)
+        return lambda x: x.project.id == int(value) or any(ancestor.id == int(value) for ancestor in x.project.ancestor_projects)
+    return lambda x: x.project.title == value or any(ancestor.title == value for ancestor in x.project.ancestor_projects)
 
 
 def _create_title_filter(value):
     return lambda x: bool(re.search(re.compile(value), x.title))
 
 
 def _create_priority_filter(value):
```

### Comparing `vja-2.0.0rc1/vja/model.py` & `vja-2.0.0rc2/vja/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,16 +54,17 @@
     default_project_id: int
 
     @classmethod
     def from_json(cls, json):
         return cls(json, json['id'], json['username'], json['name'], json['settings']['default_project_id'])
 
 
-@dataclass(frozen=True)
+@dataclass
 @data_dict
+# pylint: disable=too-many-instance-attributes
 class Project:
     json: dict = field(repr=False)
     id: int
     title: str
     description: str
     is_favorite: bool
     is_archived: bool
@@ -156,26 +157,26 @@
     repeat_mode: int
     repeat_after: timedelta
     start_date: datetime
     end_date: datetime
     percent_done: float
     done: bool
     done_at: datetime
-    labels: typing.List[Label]
+    label_objects: typing.List[Label]
     project: Project
     position: int
     bucket_id: int
     kanban_position: int
     created: datetime
     updated: datetime
     urgency: float = field(init=False)
 
     @property
-    def label_titles(self):
-        return ",".join(map(lambda label: label.title, self.labels or []))
+    def labels(self):
+        return ",".join(map(lambda label: label.title, self.label_objects or []))
 
     @classmethod
     def from_json(cls, json, project_object, labels):
         return cls(json, json['id'], json['title'], json['description'],
                    json['priority'],
                    json['is_favorite'],
                    parse_json_date(json['due_date']),
@@ -193,8 +194,8 @@
                    json['bucket_id'],
                    json['kanban_position'],
                    parse_json_date(json['created']),
                    parse_json_date(json['updated'])
                    )
 
     def has_label(self, label):
-        return any(x.id == label.id for x in self.labels)
+        return any(x.id == label.id for x in self.label_objects)
```

### Comparing `vja-2.0.0rc1/vja/output.py` & `vja-2.0.0rc2/vja/output.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 BUCKET_LIST_FORMAT_DEFAULT = '{x.id:5} {x.title:20.20} {x.is_done_bucket:2} {x.limit:3} {x.count_tasks:5}'
 
 LABEL_LIST_FORMAT_DEFAULT = '{x.id:5} {x.title:20.20}'
 
 TASK_LIST_FORMAT_DEFAULT = '{x.id:5} ({x.priority}) {"*" if x.is_favorite else " "} {x.title:50.50} ' \
                            '{x.due_date.strftime("%a %d.%m %H:%M") if x.due_date else "":15.15} ' \
                            '{"R" if x.reminders else " "} {x.project.title:20.20} ' \
-                           '{x.label_titles:20.20} {x.urgency:3.1f}'
+                           '{x.labels:20.20} {x.urgency:3.1f}'
 
 logger = logging.getLogger(__name__)
 
 
 class Output:
 
     def user(self, user: User, is_json, is_jsonvja):
```

### Comparing `vja-2.0.0rc1/vja/parse.py` & `vja-2.0.0rc2/vja/parse.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc1/vja/project_service.py` & `vja-2.0.0rc2/vja/project_service.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,52 +9,56 @@
 
 
 class ProjectService:
     def __init__(self, api_client: ApiClient):
         self._api_client = api_client
         self._project_by_id: Optional[dict] = None
 
+    def find_all_projects(self) -> [Project]:
+        if not self._project_by_id:
+            self._project_by_id = {x['id']: Project.from_json(x, []) for x in self._api_client.get_projects()}
+            self.fill_ancestors()
+        return self._project_by_id.values()
+
     def find_project_by_id(self, project_id: int) -> Project:
         if not self._project_by_id:
-            self._project_by_id = {x['id']: self.convert_project_json(x) for x in self._api_client.get_projects()}
+            self._project_by_id = {x['id']: Project.from_json(x, []) for x in self._api_client.get_projects()}
+            self.fill_ancestors()
         return self._project_by_id.get(project_id)
 
-    def find_project_by_title(self, title):
-        project_objects = [self.convert_project_json(x) for x in self._api_client.get_projects()]
+    def find_project_by_title(self, title) -> Project:
+        project_objects = [Project.from_json(x, []) for x in self._api_client.get_projects()]
         if not project_objects:
             raise VjaError('No projects exist. Go and create at least one.')
         project_found = [x for x in project_objects if x.title == title]
         if not project_found:
             raise VjaError(f'Project with title {title} does not exist.')
         return project_found[0]
 
     def get_default_project(self) -> Project:
         user = User.from_json(self._api_client.get_user())
         project_found = self.find_project_by_id(user.default_project_id)
         if not project_found:
-            project_objects = [self.convert_project_json(x) for x in self._api_client.get_projects()]
+            project_objects = [Project.from_json(x, []) for x in self._api_client.get_projects()]
             if not project_objects:
                 raise VjaError('No projects exist. Go and create at least one.')
             project_objects.sort(key=lambda x: x.id)
             favorite_projects = [x for x in project_objects if x.is_favorite]
             if favorite_projects:
                 project_found = favorite_projects[0]
             else:
                 project_found = project_objects[0]
         return project_found
 
-    def convert_project_json(self, project_json: dict) -> Project:
-        ancestor_projects = []
-        # project_id = project_json['id']
-        # parent_project_id = project_json['parent_project_id']
-        # if parent_project_id != id find parent and add it to the ancestors and proceed with parent the same way
-        # ancestor = self.get_ancestor_project(project_id, parent_project_id)
-        # while ancestor:
-        #     ancestor_projects.append(ancestor)
-        #     ancestor = self.get_ancestor_project(ancestor.id, ancestor.parent_project_id)
-        return Project.from_json(project_json, ancestor_projects)
+    def fill_ancestors(self):
+        for project in self._project_by_id.values():
+            ancestor_projects = []
+            ancestor = self.get_ancestor_project(project.id, project.parent_project_id)
+            while ancestor:
+                ancestor_projects.append(ancestor)
+                ancestor = self.get_ancestor_project(ancestor.id, ancestor.parent_project_id)
+            project.ancestor_projects = ancestor_projects
 
     def get_ancestor_project(self, project_id, parent_project_id) -> Optional[Project]:
         if project_id == parent_project_id or parent_project_id == 0 or project_id == 0:
             return None
-        ancestor = self.find_project_by_id(parent_project_id)
-        return ancestor
+        return self._project_by_id.get(parent_project_id)
```

### Comparing `vja-2.0.0rc1/vja/service_command.py` & `vja-2.0.0rc2/vja/service_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     def logout(self):
         self._api_client.logout()
         logger.info('Logged out')
 
     # project
     def add_project(self, parent_project_id, title):
         project_json = self._api_client.put_project(parent_project_id, title)
-        return self._project_service.convert_project_json(project_json)
+        return self._project_service.find_project_by_id(project_json['id'])
 
     # label
     def add_label(self, title):
         label_json = self._api_client.put_label(title)
         return Label.from_json(label_json)
 
     # tasks
```

### Comparing `vja-2.0.0rc1/vja/service_query.py` & `vja-2.0.0rc2/vja/service_query.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,19 +19,18 @@
 
     # user
     def find_current_user(self):
         return User.from_json(self._api_client.get_user())
 
     # project
     def find_all_projects(self):
-        return [self._project_service.convert_project_json(project_json) for project_json in
-                (self._api_client.get_projects())]
+        return self._project_service.find_all_projects()
 
     def find_project_by_id(self, project_id):
-        return self._project_service.convert_project_json(self._api_client.get_project(project_id))
+        return self._project_service.find_project_by_id(project_id)
 
     # bucket
     def find_all_buckets_in_project(self, project_id):
         return Bucket.from_json_array(self._api_client.get_buckets(project_id))
 
     # label
     def find_all_labels(self):
@@ -65,12 +64,12 @@
                 reverse=sort_field['reverse'])
         return filtered_tasks
 
 
 def sortable_task_value(task, field):
     field_name = field
     if field in ('label', 'labels'):
-        field_name = 'label_titles'
+        field_name = 'labels'
     field_value = rgetattr(task, field_name)
     if isinstance(field_value, str):
         return field_value.upper()
     return field_value
```

### Comparing `vja-2.0.0rc1/vja/task_service.py` & `vja-2.0.0rc2/vja/task_service.py`

 * *Files identical despite different names*

### Comparing `vja-2.0.0rc1/vja/urgency.py` & `vja-2.0.0rc2/vja/urgency.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         favorite_score = int(task.is_favorite) * self._urgency_coefficients.get('favorite_weight', 1.0)
         project_name_score = self._get_project_score(task) * self._urgency_coefficients.get('project_keyword', 1.0)
         lable_name_score = self._get_label_score(task) * self._urgency_coefficients.get('label_keyword', 1.0)
 
         return 1 + due_date_score + priority_score + favorite_score + project_name_score + lable_name_score
 
     def _get_label_score(self, task):
-        task_label_title = task.label_titles.lower()
+        task_label_title = task.labels.lower()
         return int(any(label_name.lower() in task_label_title for label_name in
                        self._label_keywords)) if self._label_keywords else 0
 
     def _get_project_score(self, task):
         task_project_title = task.project.title.lower()
         return int(any(project_name.lower() in task_project_title for project_name in
                        self._project_keywords)) if self._project_keywords else 0
```

### Comparing `vja-2.0.0rc1/vja.egg-info/PKG-INFO` & `vja-2.0.0rc2/vja.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vja
-Version: 2.0.0rc1
+Version: 2.0.0rc2
 Summary: A simple CLI for Vikunja task manager
 Home-page: https://gitlab.com/ce72/vja
 Author: ce72
 License: UNKNOWN
 Description: # CLI client for Vikunja
         
         [![pypi package version](https://img.shields.io/pypi/v/vja)](https://pypi.org/project/vja/)
```

### Comparing `vja-2.0.0rc1/vja.egg-info/SOURCES.txt` & `vja-2.0.0rc2/vja.egg-info/SOURCES.txt`

 * *Files identical despite different names*

