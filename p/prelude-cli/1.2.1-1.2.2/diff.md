# Comparing `tmp/prelude-cli-1.2.1.tar.gz` & `tmp/prelude-cli-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude-cli-1.2.1.tar", last modified: Tue May 23 21:46:57 2023, max compression
+gzip compressed data, was "prelude-cli-1.2.2.tar", last modified: Fri Jun  2 17:13:20 2023, max compression
```

## Comparing `prelude-cli-1.2.1.tar` & `prelude-cli-1.2.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-23 21:46:57.208481 prelude-cli-1.2.1/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-1.2.1/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-1.2.1/MANIFEST.in
--rw-r--r--   0 pack       (501) staff       (20)      832 2023-05-23 21:46:57.208529 prelude-cli-1.2.1/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-1.2.1/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-23 21:46:57.204897 prelude-cli-1.2.1/prelude_cli/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.1/prelude_cli/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)      775 2023-05-02 14:19:17.000000 prelude-cli-1.2.1/prelude_cli/cli.py
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-05-03 13:30:52.000000 prelude-cli-1.2.1/prelude_cli/spinner.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-23 21:46:57.205799 prelude-cli-1.2.1/prelude_cli/templates/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.1/prelude_cli/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)      241 2023-05-04 16:11:50.000000 prelude-cli-1.2.1/prelude_cli/templates/template.go
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-23 21:46:57.208132 prelude-cli-1.2.1/prelude_cli/views/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.1/prelude_cli/views/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     3241 2023-05-18 20:31:39.000000 prelude-cli-1.2.1/prelude_cli/views/build.py
--rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-1.2.1/prelude_cli/views/configure.py
--rw-r--r--   0 pack       (501) staff       (20)     7276 2023-05-23 21:42:11.000000 prelude-cli-1.2.1/prelude_cli/views/detect.py
--rw-r--r--   0 pack       (501) staff       (20)     3478 2023-05-18 20:31:39.000000 prelude-cli-1.2.1/prelude_cli/views/iam.py
--rw-r--r--   0 pack       (501) staff       (20)     2279 2023-05-18 19:30:30.000000 prelude-cli-1.2.1/prelude_cli/views/partner.py
--rw-r--r--   0 pack       (501) staff       (20)     1139 2023-05-03 13:30:52.000000 prelude-cli-1.2.1/prelude_cli/views/shared.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-23 21:46:57.205618 prelude-cli-1.2.1/prelude_cli.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)      832 2023-05-23 21:46:57.000000 prelude-cli-1.2.1/prelude_cli.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      598 2023-05-23 21:46:57.000000 prelude-cli-1.2.1/prelude_cli.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2023-05-23 21:46:57.000000 prelude-cli-1.2.1/prelude_cli.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)       48 2023-05-23 21:46:57.000000 prelude-cli-1.2.1/prelude_cli.egg-info/entry_points.txt
--rw-r--r--   0 pack       (501) staff       (20)       32 2023-05-23 21:46:57.000000 prelude-cli-1.2.1/prelude_cli.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       12 2023-05-23 21:46:57.000000 prelude-cli-1.2.1/prelude_cli.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-1.2.1/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      663 2023-05-23 21:46:57.208742 prelude-cli-1.2.1/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-02 17:13:20.814235 prelude-cli-1.2.2/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-1.2.2/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-1.2.2/MANIFEST.in
+-rw-r--r--   0 pack       (501) staff       (20)      832 2023-06-02 17:13:20.814289 prelude-cli-1.2.2/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-1.2.2/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-02 17:13:20.811526 prelude-cli-1.2.2/prelude_cli/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.2/prelude_cli/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)      775 2023-05-02 14:19:17.000000 prelude-cli-1.2.2/prelude_cli/cli.py
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-05-03 13:30:52.000000 prelude-cli-1.2.2/prelude_cli/spinner.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-02 17:13:20.812461 prelude-cli-1.2.2/prelude_cli/templates/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.2/prelude_cli/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)      249 2023-06-01 16:01:25.000000 prelude-cli-1.2.2/prelude_cli/templates/template.go
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-02 17:13:20.814038 prelude-cli-1.2.2/prelude_cli/views/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.2/prelude_cli/views/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     3405 2023-06-02 13:58:42.000000 prelude-cli-1.2.2/prelude_cli/views/build.py
+-rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-1.2.2/prelude_cli/views/configure.py
+-rw-r--r--   0 pack       (501) staff       (20)     7430 2023-05-30 20:30:23.000000 prelude-cli-1.2.2/prelude_cli/views/detect.py
+-rw-r--r--   0 pack       (501) staff       (20)     3478 2023-05-18 20:31:39.000000 prelude-cli-1.2.2/prelude_cli/views/iam.py
+-rw-r--r--   0 pack       (501) staff       (20)     2279 2023-05-18 19:30:30.000000 prelude-cli-1.2.2/prelude_cli/views/partner.py
+-rw-r--r--   0 pack       (501) staff       (20)     1139 2023-05-03 13:30:52.000000 prelude-cli-1.2.2/prelude_cli/views/shared.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-02 17:13:20.812274 prelude-cli-1.2.2/prelude_cli.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)      832 2023-06-02 17:13:20.000000 prelude-cli-1.2.2/prelude_cli.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      598 2023-06-02 17:13:20.000000 prelude-cli-1.2.2/prelude_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2023-06-02 17:13:20.000000 prelude-cli-1.2.2/prelude_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)       48 2023-06-02 17:13:20.000000 prelude-cli-1.2.2/prelude_cli.egg-info/entry_points.txt
+-rw-r--r--   0 pack       (501) staff       (20)       32 2023-06-02 17:13:20.000000 prelude-cli-1.2.2/prelude_cli.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       12 2023-06-02 17:13:20.000000 prelude-cli-1.2.2/prelude_cli.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-1.2.2/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      663 2023-06-02 17:13:20.814501 prelude-cli-1.2.2/setup.cfg
```

### Comparing `prelude-cli-1.2.1/LICENSE` & `prelude-cli-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.1/PKG-INFO` & `prelude-cli-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.2.1
+Version: 1.2.2
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-cli-1.2.1/prelude_cli/cli.py` & `prelude-cli-1.2.2/prelude_cli/cli.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.1/prelude_cli/views/build.py` & `prelude-cli-1.2.2/prelude_cli/views/build.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,20 @@
 @click.option('-a', '--advisory', help='alert identifier [CVE ID, Advisory ID, etc]', default=None, type=str)
 @click.pass_obj
 @handle_api_error
 def create_test(controller, name, test, unit, advisory):
     """ Create or update a security test """
     test_id = test or str(uuid.uuid4())
     with Spinner():
-        controller.create_test(test_id=test_id, name=name, unit=unit, advisory=advisory)
+        controller.create_test(
+            test_id=test_id,
+            name=name,
+            unit=unit,
+            advisory=advisory
+        )
 
     if not test:
         basename = f'{test_id}.go'
         template = pkg_resources.read_text(templates, 'template.go')
         template = template.replace('$ID', test_id)
         template = template.replace('$NAME', name)
         template = template.replace('$UNIT', unit or '')
@@ -91,8 +96,11 @@
 
     identifier = test or test_id()
     
     if Path(path).is_file():
         upload(p=Path(path))
     else:
         for obj in Path(path).rglob('*'):
-            upload(p=Path(obj))
+            try:
+                upload(p=Path(obj))
+            except ValueError as e:
+                click.secho(e.args[0], fg='red')
```

### Comparing `prelude-cli-1.2.1/prelude_cli/views/configure.py` & `prelude-cli-1.2.2/prelude_cli/views/configure.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.1/prelude_cli/views/detect.py` & `prelude-cli-1.2.2/prelude_cli/views/detect.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,33 +183,36 @@
         click.secho('Project cloned successfully', fg='green')
 
 
 @detect.command('activity')
 @click.option('-v', '--view',
               help='retrieve a specific result view',
               default='logs', show_default=True,
-              type=click.Choice(['logs', 'days', 'insights', 'probes', 'advisories', 'tests']))
+              type=click.Choice(['logs', 'days', 'insights', 'probes', 'advisories', 'tests', 'metrics']))
 @click.option('-d', '--days', help='days to look back', default=30, type=int)
 @click.option('--tests', help='comma-separated list of test IDs', type=str)
 @click.option('--tags', help='comma-separated list of tags', type=str)
 @click.option('--endpoints', help='comma-separated list of endpoint IDs', type=str)
+@click.option('--status', help='comma-separated list of status numbers', type=str)
 @click.option('--dos', help='comma-separated list of DOS', type=str)
 @click.pass_obj
 @handle_api_error
-def describe_activity(controller, days, view, tests, tags, endpoints, dos):
+def describe_activity(controller, days, view, tests, tags, endpoints, status, dos):
     """ View my Detect results """
     filters = dict(
         start=datetime.utcnow() - timedelta(days=days),
         finish=datetime.utcnow() + timedelta(days=1)
     )
     if tests:
         filters['tests'] = tests
     if tags:
         filters['tags'] = tags
     if endpoints:
         filters['endpoints'] = endpoints
+    if status:
+        filters['statuses'] = status
     if dos:
         filters['dos'] = dos
 
     with Spinner():
         data = controller.describe_activity(view=view, filters=filters)
     print_json(data=data)
```

### Comparing `prelude-cli-1.2.1/prelude_cli/views/iam.py` & `prelude-cli-1.2.2/prelude_cli/views/iam.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.1/prelude_cli/views/partner.py` & `prelude-cli-1.2.2/prelude_cli/views/partner.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.1/prelude_cli/views/shared.py` & `prelude-cli-1.2.2/prelude_cli/views/shared.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.1/prelude_cli.egg-info/PKG-INFO` & `prelude-cli-1.2.2/prelude_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.2.1
+Version: 1.2.2
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-cli-1.2.1/prelude_cli.egg-info/SOURCES.txt` & `prelude-cli-1.2.2/prelude_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.1/setup.cfg` & `prelude-cli-1.2.2/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-cli
-version = 1.2.1
+version = 1.2.2
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers = 
@@ -13,15 +13,15 @@
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=3.8
 install_requires = 
-	prelude-sdk == 1.2.1
+	prelude-sdk == 1.2.2
 	click > 8
 	rich
 
 [options.entry_points]
 console_scripts = 
 	prelude = prelude_cli.cli:cli
```

