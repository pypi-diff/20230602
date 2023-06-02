# Comparing `tmp/fish_databricks_jobs-0.7.7.tar.gz` & `tmp/fish_databricks_jobs-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fish_databricks_jobs-0.7.7.tar", max compression
+gzip compressed data, was "fish_databricks_jobs-0.7.8.tar", max compression
```

## Comparing `fish_databricks_jobs-0.7.7.tar` & `fish_databricks_jobs-0.7.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     4201 2023-01-13 22:26:42.639529 fish_databricks_jobs-0.7.7/README.md
--rw-r--r--   0        0        0        0 2022-12-31 17:43:55.621646 fish_databricks_jobs-0.7.7/fish_databricks_jobs/__init__.py
--rwxr-xr-x   0        0        0     3538 2023-01-13 22:26:42.640462 fish_databricks_jobs-0.7.7/fish_databricks_jobs/cli.py
--rw-r--r--   0        0        0      313 2022-12-15 01:07:10.972953 fish_databricks_jobs-0.7.7/fish_databricks_jobs/config.py
--rw-r--r--   0        0        0        0 2022-12-09 18:53:21.592021 fish_databricks_jobs-0.7.7/fish_databricks_jobs/services/__init__.py
--rw-r--r--   0        0        0     2380 2023-01-09 21:28:07.727953 fish_databricks_jobs-0.7.7/fish_databricks_jobs/services/jobs.py
--rw-r--r--   0        0        0     2042 2023-01-06 16:19:37.255829 fish_databricks_jobs-0.7.7/fish_databricks_jobs/services/permissions.py
--rw-r--r--   0        0        0      143 2022-12-31 18:38:45.554991 fish_databricks_jobs-0.7.7/fish_databricks_jobs/services/version.py
--rw-r--r--   0        0        0      632 2023-01-13 22:27:08.056935 fish_databricks_jobs-0.7.7/pyproject.toml
--rw-r--r--   0        0        0     5257 1970-01-01 00:00:00.000000 fish_databricks_jobs-0.7.7/setup.py
--rw-r--r--   0        0        0     4927 1970-01-01 00:00:00.000000 fish_databricks_jobs-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0     4201 2023-01-13 22:26:42.639529 fish_databricks_jobs-0.7.8/README.md
+-rw-r--r--   0        0        0        0 2022-12-31 17:43:55.621646 fish_databricks_jobs-0.7.8/fish_databricks_jobs/__init__.py
+-rwxr-xr-x   0        0        0     3538 2023-01-13 22:26:42.640462 fish_databricks_jobs-0.7.8/fish_databricks_jobs/cli.py
+-rw-r--r--   0        0        0      313 2022-12-15 01:07:10.972953 fish_databricks_jobs-0.7.8/fish_databricks_jobs/config.py
+-rw-r--r--   0        0        0        0 2022-12-09 18:53:21.592021 fish_databricks_jobs-0.7.8/fish_databricks_jobs/services/__init__.py
+-rw-r--r--   0        0        0     2380 2023-01-09 21:28:07.727953 fish_databricks_jobs-0.7.8/fish_databricks_jobs/services/jobs.py
+-rw-r--r--   0        0        0     2042 2023-01-06 16:19:37.255829 fish_databricks_jobs-0.7.8/fish_databricks_jobs/services/permissions.py
+-rw-r--r--   0        0        0      143 2022-12-31 18:38:45.554991 fish_databricks_jobs-0.7.8/fish_databricks_jobs/services/version.py
+-rw-r--r--   0        0        0      632 2023-06-02 18:12:29.868470 fish_databricks_jobs-0.7.8/pyproject.toml
+-rw-r--r--   0        0        0     5257 1970-01-01 00:00:00.000000 fish_databricks_jobs-0.7.8/setup.py
+-rw-r--r--   0        0        0     4927 1970-01-01 00:00:00.000000 fish_databricks_jobs-0.7.8/PKG-INFO
```

### Comparing `fish_databricks_jobs-0.7.7/README.md` & `fish_databricks_jobs-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `fish_databricks_jobs-0.7.7/fish_databricks_jobs/cli.py` & `fish_databricks_jobs-0.7.8/fish_databricks_jobs/cli.py`

 * *Files identical despite different names*

### Comparing `fish_databricks_jobs-0.7.7/fish_databricks_jobs/services/jobs.py` & `fish_databricks_jobs-0.7.8/fish_databricks_jobs/services/jobs.py`

 * *Files identical despite different names*

### Comparing `fish_databricks_jobs-0.7.7/fish_databricks_jobs/services/permissions.py` & `fish_databricks_jobs-0.7.8/fish_databricks_jobs/services/permissions.py`

 * *Files identical despite different names*

### Comparing `fish_databricks_jobs-0.7.7/pyproject.toml` & `fish_databricks_jobs-0.7.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fish-databricks-jobs"
-version = "0.7.7"
+version = "0.7.8"
 description = "cli and sdk to manage Jobs in Databricks"
 authors = ["Tim Chen <firstim@gmail.com>"]
 readme = "README.md"
 packages = [{include = "fish_databricks_jobs"}]
 homepage = "https://github.com/firstim/fish-databricks-jobs"
 
 [tool.poetry.scripts]
```

### Comparing `fish_databricks_jobs-0.7.7/setup.py` & `fish_databricks_jobs-0.7.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 entry_points = \
 {'console_scripts': ['fish-databricks-jobs = fish_databricks_jobs.cli:app',
                      'jobser = fish_databricks_jobs.cli:app']}
 
 setup_kwargs = {
     'name': 'fish-databricks-jobs',
-    'version': '0.7.7',
+    'version': '0.7.8',
     'description': 'cli and sdk to manage Jobs in Databricks',
     'long_description': '# fish-databricks-jobs \n\nfish-databricks-jobs is cli and python sdk to manage Jobs for Databricks. e.g assign permissions to multiple jobs. User can filter jobs by job name or tags.  \n\nThe functionality of current [databricks-cli(v0.17.4)](https://pypi.org/project/databricks-cli/) is limited on the `jobs` api. e.g it can not assign job permission.\n\nWith `fish-databricks-jobs`, you can assign job permission, e.g: \n\nto assign group `mygroup` with permission `can_manage` to job by filter `843966944901662`(job_id) \n```angular2html\n$ fish-databricks-jobs permission-assign mygroup --type group --level can_manage --filter 843966944901662\n```\n# Installation\nPython Version >= 3.7 \n```\n$ pip install --upgrade fish-databricks-jobs\n```\n```angular2html\n$ fish-databricks-jobs --version\nVersion: 0.6.8\n```\n# Usage\n### permission-assign\n```\n$ fish-databricks-jobs permission-assign -h\n\n Usage: fish-databricks-jobs permission-assign [OPTIONS] NAME\n\n Assign permission to user\n\n╭─ Arguments ─────────────────────────────────────────────────────────────────────────────────────────────────────────────╮\n│ *    name      TEXT  User name, group name or serive principal id. Who will receive the permisssion. [default: None]    │\n│                      [required]                                                                                         │\n╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Options ───────────────────────────────────────────────────────────────────────────────────────────────────────────────╮\n│    --type     -t      [user|principal|group]                Permission receiver type. [default: user]                   │\n│ *  --level    -l      [can_view|can_manage|can_manage_run]  Permission level. [default: None] [required]                │\n│    --filter   -f      TEXT                                  filter jobs, case insensitively. [default: None]            │\n│    --profile  -p      TEXT                                  profile name in ~/.databrickscfg [default: DEFAULT]         │\n│    --force                                                  Attempt to assign permission without prompting for          │\n│                                                             confirmation. **Use this flag with caution**                │\n│    --help     -h                                            Show this message and exit.                                 │\n╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯\n```\n### use as sdk to list jobs\nin databricks\' notebook\n```\n%pip install fish-databricks-jobs\n```\n\n```python\nfrom fish_databricks_jobs.services.jobs import JobsService, Job\nhost = f\'https://{spark.conf.get("spark.databricks.workspaceUrl")}\'\ntoken = \'exampletokenc0e27d8b91fd8c0144f0a23\'\n\njob_list = JobsService(host, token).list()\ndf = spark.createDataFrame(job_list)\n\ndisplay(df)\n```\n# Config authentication\nfish-databricks-jobs uses same config file as `databricks-cli`. e.g.`~/.databrickscfg` for macOS. Similar for Windows.\n```\n[DEFAULT]\nhost = https://example.cloud.databricks.com\ntoken = exampletokenc0e27d8b91fd8c0144f0a23\n```\n\n\n\n',
     'author': 'Tim Chen',
     'author_email': 'firstim@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/firstim/fish-databricks-jobs',
```

### Comparing `fish_databricks_jobs-0.7.7/PKG-INFO` & `fish_databricks_jobs-0.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fish-databricks-jobs
-Version: 0.7.7
+Version: 0.7.8
 Summary: cli and sdk to manage Jobs in Databricks
 Home-page: https://github.com/firstim/fish-databricks-jobs
 Author: Tim Chen
 Author-email: firstim@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

