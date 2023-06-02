# Comparing `tmp/gardener-cicd-cli-1.2065.0.tar.gz` & `tmp/gardener-cicd-cli-1.2066.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener-cicd-cli-1.2065.0.tar", last modified: Fri May 26 13:23:43 2023, max compression
+gzip compressed data, was "gardener-cicd-cli-1.2066.0.tar", last modified: Fri Jun  2 05:01:05 2023, max compression
```

## Comparing `gardener-cicd-cli-1.2065.0.tar` & `gardener-cicd-cli-1.2066.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:43.660949 gardener-cicd-cli-1.2065.0/
--rw-r--r--   0 root         (0) root         (0)       14 2023-05-26 13:22:41.000000 gardener-cicd-cli-1.2065.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      135 2023-05-26 13:23:43.660949 gardener-cicd-cli-1.2065.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:43.656949 gardener-cicd-cli-1.2065.0/bin/
--rwxr-xr-x   0 root         (0) root         (0)    10432 2023-05-26 13:22:41.000000 gardener-cicd-cli-1.2065.0/bin/component-cli
--rwxr-xr-x   0 root         (0) root         (0)      369 2023-05-26 13:22:41.000000 gardener-cicd-cli-1.2065.0/bin/helm
--rwxr-xr-x   0 root         (0) root         (0)     5611 2023-05-26 13:22:41.000000 gardener-cicd-cli-1.2065.0/bin/launch-dockerd.sh
--rwxr-xr-x   0 root         (0) root         (0)     3301 2023-05-26 13:22:41.000000 gardener-cicd-cli-1.2065.0/bin/purge_history
--rwxr-xr-x   0 root         (0) root         (0)      265 2023-05-26 13:22:41.000000 gardener-cicd-cli-1.2065.0/bin/yaml2json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:43.660949 gardener-cicd-cli-1.2065.0/gardener_ci/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 13:22:41.000000 gardener-cicd-cli-1.2065.0/gardener_ci/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3901 2023-05-26 13:22:41.000000 gardener-cicd-cli-1.2065.0/gardener_ci/_cfg_mgmt.py
--rw-r--r--   0 root         (0) root         (0)     1917 2023-05-26 13:22:41.000000 gardener-cicd-cli-1.2065.0/gardener_ci/_clamav.py
--rw-r--r--   0 root         (0) root         (0)     6463 2023-05-26 13:22:41.000000 gardener-cicd-cli-1.2065.0/gardener_ci/_concourse.py
--rw-r--r--   0 root         (0) root         (0)     7657 2023-05-26 13:22:41.000000 gardener-cicd-cli-1.2065.0/gardener_ci/_oci.py
--rw-r--r--   0 root         (0) root         (0)     1258 2023-05-26 13:22:41.000000 gardener-cicd-cli-1.2065.0/gardener_ci/_osinfo.py
--rw-r--r--   0 root         (0) root         (0)      380 2023-05-26 13:22:41.000000 gardener-cicd-cli-1.2065.0/gardener_ci/_slack.py
--rw-r--r--   0 root         (0) root         (0)    11329 2023-05-26 13:22:41.000000 gardener-cicd-cli-1.2065.0/gardener_ci/bdba.py
--rw-r--r--   0 root         (0) root         (0)     8458 2023-05-26 13:22:41.000000 gardener-cicd-cli-1.2065.0/gardener_ci/cd.py
--rw-r--r--   0 root         (0) root         (0)     1899 2023-05-26 13:22:41.000000 gardener-cicd-cli-1.2065.0/gardener_ci/checkmarx_cli.py
--rwxr-xr-x   0 root         (0) root         (0)     9186 2023-05-26 13:22:41.000000 gardener-cicd-cli-1.2065.0/gardener_ci/cli_gen.py
--rw-r--r--   0 root         (0) root         (0)     7669 2023-05-26 13:22:41.000000 gardener-cicd-cli-1.2065.0/gardener_ci/compliance.py
--rw-r--r--   0 root         (0) root         (0)     3188 2023-05-26 13:22:41.000000 gardener-cicd-cli-1.2065.0/gardener_ci/config.py
--rw-r--r--   0 root         (0) root         (0)     1408 2023-05-26 13:22:41.000000 gardener-cicd-cli-1.2065.0/gardener_ci/containerutil.py
--rw-r--r--   0 root         (0) root         (0)      886 2023-05-26 13:22:41.000000 gardener-cicd-cli-1.2065.0/gardener_ci/docker.py
--rw-r--r--   0 root         (0) root         (0)     2415 2023-05-26 13:22:41.000000 gardener-cicd-cli-1.2065.0/gardener_ci/elastic.py
--rw-r--r--   0 root         (0) root         (0)     3512 2023-05-26 13:22:41.000000 gardener-cicd-cli-1.2065.0/gardener_ci/gh.py
--rw-r--r--   0 root         (0) root         (0)     4935 2023-05-26 13:22:41.000000 gardener-cicd-cli-1.2065.0/gardener_ci/githubutil.py
--rw-r--r--   0 root         (0) root         (0)     3128 2023-05-26 13:22:41.000000 gardener-cicd-cli-1.2065.0/gardener_ci/ocm.py
--rw-r--r--   0 root         (0) root         (0)    12274 2023-05-26 13:22:41.000000 gardener-cicd-cli-1.2065.0/gardener_ci/pipeline.py
--rw-r--r--   0 root         (0) root         (0)     2984 2023-05-26 13:22:41.000000 gardener-cicd-cli-1.2065.0/gardener_ci/productutil_v2.py
--rw-r--r--   0 root         (0) root         (0)     2864 2023-05-26 13:22:41.000000 gardener-cicd-cli-1.2065.0/gardener_ci/whdutil.py
--rwxr-xr-x   0 root         (0) root         (0)      265 2023-05-26 13:22:41.000000 gardener-cicd-cli-1.2065.0/gardener_ci/yaml2json.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:23:43.660949 gardener-cicd-cli-1.2065.0/gardener_cicd_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      135 2023-05-26 13:23:43.000000 gardener-cicd-cli-1.2065.0/gardener_cicd_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      960 2023-05-26 13:23:43.000000 gardener-cicd-cli-1.2065.0/gardener_cicd_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 13:23:43.000000 gardener-cicd-cli-1.2065.0/gardener_cicd_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      130 2023-05-26 13:23:43.000000 gardener-cicd-cli-1.2065.0/gardener_cicd_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-05-26 13:23:43.000000 gardener-cicd-cli-1.2065.0/gardener_cicd_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-26 13:23:43.000000 gardener-cicd-cli-1.2065.0/gardener_cicd_cli.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 13:23:43.660949 gardener-cicd-cli-1.2065.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1514 2023-05-26 13:22:41.000000 gardener-cicd-cli-1.2065.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:05.230250 gardener-cicd-cli-1.2066.0/
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-02 05:00:06.000000 gardener-cicd-cli-1.2066.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      135 2023-06-02 05:01:05.230250 gardener-cicd-cli-1.2066.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:05.222250 gardener-cicd-cli-1.2066.0/bin/
+-rwxr-xr-x   0 root         (0) root         (0)    11039 2023-06-02 05:00:06.000000 gardener-cicd-cli-1.2066.0/bin/component-cli
+-rwxr-xr-x   0 root         (0) root         (0)      369 2023-06-02 05:00:06.000000 gardener-cicd-cli-1.2066.0/bin/helm
+-rwxr-xr-x   0 root         (0) root         (0)     5611 2023-06-02 05:00:06.000000 gardener-cicd-cli-1.2066.0/bin/launch-dockerd.sh
+-rwxr-xr-x   0 root         (0) root         (0)     3301 2023-06-02 05:00:06.000000 gardener-cicd-cli-1.2066.0/bin/purge_history
+-rwxr-xr-x   0 root         (0) root         (0)      265 2023-06-02 05:00:06.000000 gardener-cicd-cli-1.2066.0/bin/yaml2json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:05.230250 gardener-cicd-cli-1.2066.0/gardener_ci/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 05:00:06.000000 gardener-cicd-cli-1.2066.0/gardener_ci/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3901 2023-06-02 05:00:06.000000 gardener-cicd-cli-1.2066.0/gardener_ci/_cfg_mgmt.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-06-02 05:00:06.000000 gardener-cicd-cli-1.2066.0/gardener_ci/_clamav.py
+-rw-r--r--   0 root         (0) root         (0)     6463 2023-06-02 05:00:06.000000 gardener-cicd-cli-1.2066.0/gardener_ci/_concourse.py
+-rw-r--r--   0 root         (0) root         (0)     8114 2023-06-02 05:00:06.000000 gardener-cicd-cli-1.2066.0/gardener_ci/_oci.py
+-rw-r--r--   0 root         (0) root         (0)     1258 2023-06-02 05:00:06.000000 gardener-cicd-cli-1.2066.0/gardener_ci/_osinfo.py
+-rw-r--r--   0 root         (0) root         (0)      380 2023-06-02 05:00:06.000000 gardener-cicd-cli-1.2066.0/gardener_ci/_slack.py
+-rw-r--r--   0 root         (0) root         (0)    11329 2023-06-02 05:00:06.000000 gardener-cicd-cli-1.2066.0/gardener_ci/bdba.py
+-rw-r--r--   0 root         (0) root         (0)     8458 2023-06-02 05:00:06.000000 gardener-cicd-cli-1.2066.0/gardener_ci/cd.py
+-rw-r--r--   0 root         (0) root         (0)     1899 2023-06-02 05:00:06.000000 gardener-cicd-cli-1.2066.0/gardener_ci/checkmarx_cli.py
+-rwxr-xr-x   0 root         (0) root         (0)     9186 2023-06-02 05:00:06.000000 gardener-cicd-cli-1.2066.0/gardener_ci/cli_gen.py
+-rw-r--r--   0 root         (0) root         (0)     7669 2023-06-02 05:00:06.000000 gardener-cicd-cli-1.2066.0/gardener_ci/compliance.py
+-rw-r--r--   0 root         (0) root         (0)     3188 2023-06-02 05:00:06.000000 gardener-cicd-cli-1.2066.0/gardener_ci/config.py
+-rw-r--r--   0 root         (0) root         (0)     1408 2023-06-02 05:00:06.000000 gardener-cicd-cli-1.2066.0/gardener_ci/containerutil.py
+-rw-r--r--   0 root         (0) root         (0)      886 2023-06-02 05:00:06.000000 gardener-cicd-cli-1.2066.0/gardener_ci/docker.py
+-rw-r--r--   0 root         (0) root         (0)     2415 2023-06-02 05:00:06.000000 gardener-cicd-cli-1.2066.0/gardener_ci/elastic.py
+-rw-r--r--   0 root         (0) root         (0)     3512 2023-06-02 05:00:06.000000 gardener-cicd-cli-1.2066.0/gardener_ci/gh.py
+-rw-r--r--   0 root         (0) root         (0)     4935 2023-06-02 05:00:06.000000 gardener-cicd-cli-1.2066.0/gardener_ci/githubutil.py
+-rw-r--r--   0 root         (0) root         (0)     3128 2023-06-02 05:00:06.000000 gardener-cicd-cli-1.2066.0/gardener_ci/ocm.py
+-rw-r--r--   0 root         (0) root         (0)    12219 2023-06-02 05:00:06.000000 gardener-cicd-cli-1.2066.0/gardener_ci/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     2984 2023-06-02 05:00:06.000000 gardener-cicd-cli-1.2066.0/gardener_ci/productutil_v2.py
+-rw-r--r--   0 root         (0) root         (0)     2864 2023-06-02 05:00:06.000000 gardener-cicd-cli-1.2066.0/gardener_ci/whdutil.py
+-rwxr-xr-x   0 root         (0) root         (0)      265 2023-06-02 05:00:06.000000 gardener-cicd-cli-1.2066.0/gardener_ci/yaml2json.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 05:01:05.230250 gardener-cicd-cli-1.2066.0/gardener_cicd_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      135 2023-06-02 05:01:05.000000 gardener-cicd-cli-1.2066.0/gardener_cicd_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      960 2023-06-02 05:01:05.000000 gardener-cicd-cli-1.2066.0/gardener_cicd_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 05:01:05.000000 gardener-cicd-cli-1.2066.0/gardener_cicd_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      130 2023-06-02 05:01:05.000000 gardener-cicd-cli-1.2066.0/gardener_cicd_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-06-02 05:01:05.000000 gardener-cicd-cli-1.2066.0/gardener_cicd_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-02 05:01:05.000000 gardener-cicd-cli-1.2066.0/gardener_cicd_cli.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-02 05:01:05.230250 gardener-cicd-cli-1.2066.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1514 2023-06-02 05:00:06.000000 gardener-cicd-cli-1.2066.0/setup.py
```

### Comparing `gardener-cicd-cli-1.2065.0/bin/component-cli` & `gardener-cicd-cli-1.2066.0/bin/component-cli`

 * *Files 10% similar despite different names*

```diff
@@ -13,22 +13,40 @@
 
 import ci.util
 
 own_dir = os.path.dirname(__file__)
 
 
 def component_archive_resource_add(argv):
+  if not argv:
+    fail_and_notify_about_unsupported_command(
+      f'Usage: {" ".join(sys.argv[:1])} resources'
+    )
+
   subcmd = argv[0]
   if not subcmd in ('resources', 'resource', 'res'):
-    delegate_to_component_cli()
+    fail_and_notify_about_unsupported_command(
+      'only sub-commands `resources`, `resource`, `res` are supported',
+    )
+
+  # the only supported subcmd is `add` (also the case in original component-cli)
+  if not len(argv) > 1:
+    fail_and_notify_about_unsupported_command(
+      f'Usage: {" ".join(sys.argv[:1])} resources add'
+    )
 
-  # the only supported subcmd is `add` (also in original component-cli)
-  # -> delegate to component-cli if it is not at expected location
   if not argv[1] == 'add':
-    delegate_to_component_cli()
+    fail_and_notify_about_unsupported_command(
+      'expected subcommand `add`',
+    )
+
+  if not len(argv) >= 3:
+    fail_and_notify_about_unsupported_command(
+      'expected two positional arguments after `add` subcommand',
+    )
 
   component_descriptor_dir = argv[2]
   try:
     resources_file = argv[3]
     if not os.path.isfile(resources_file):
       resources_file = None
   except IndexError:
@@ -108,15 +126,17 @@
   print(f'added {added_resources_count} resource(s)')
   log_argv(delegated=False)
 
 
 def image_vector(argv):
   subcmd = argv[0]
   if not subcmd in ('add',):
-    delegate_to_component_cli()
+    fail_and_notify_about_unsupported_command(
+      'only `add` subcommand is allowed',
+    )
 
   # command `image-vector add`
   parser = argparse.ArgumentParser()
   parser.add_argument('--comp-desc', required=True, dest='component_descriptor_path')
   parser.add_argument('--image-vector', required=True,  dest='images_yaml_path')
   parser.add_argument(
     '--component-prefixes',
@@ -305,20 +325,21 @@
     yaml.dump(
       data=component_descriptor_dict,
       stream=f,
       Dumper=cm.EnumValueYamlDumper,
     )
     f.write('\n#generated by cc-utils\n')
 
-def delegate_to_component_cli():
-  log_argv(delegated=True)
-  path = os.environ['PATH'].replace(own_dir, '')
-  component_cli = shutil.which('component-cli', path=path)
 
-  os.execv(component_cli, sys.argv)
+def fail_and_notify_about_unsupported_command(message: str):
+  print(f'ERROR: {message}')
+  print(f'{sys.argv=}')
+  print('')
+  print('component-cli (github.com/gardener/component-cli) is deprecated and no longer available')
+  exit(1)
 
 
 def log_argv(delegated=False):
   if not (logfile := os.environ.get('commands_log')):
     return
 
   with open(logfile, 'a') as f:
@@ -328,23 +349,23 @@
 
     entry += ' '.join(sys.argv) + '\n'
 
     f.write(entry)
 
 
 def main():
-  if os.environ.get('force_legacy_component_cli', False):
-    delegate_to_component_cli()
+  if not len(sys.argv) > 1:
+    print(f'Usage: {sys.argv[0]} component-archive | image-vector')
+    exit(1)
 
-  try:
-    cmd = sys.argv[1]
-    if cmd in ('component-archive', 'componentarchive', 'archive', 'ca'):
-      return component_archive_resource_add(sys.argv[2:])
-    elif cmd in ('image-vector', 'imagevector', 'iv'):
-      return image_vector(sys.argv[2:])
-
-    delegate_to_component_cli()
-  except (KeyError, IndexError):
-    delegate_to_component_cli()
+  cmd = sys.argv[1]
+  if cmd in ('component-archive', 'componentarchive', 'archive', 'ca'):
+    return component_archive_resource_add(sys.argv[2:])
+  elif cmd in ('image-vector', 'imagevector', 'iv'):
+    return image_vector(sys.argv[2:])
+
+  fail_and_notify_about_unsupported_command(
+    'only commands `component-archive` and `imagevector` are allowed',
+  )
 
 if __name__ == '__main__':
   main()
```

### Comparing `gardener-cicd-cli-1.2065.0/bin/launch-dockerd.sh` & `gardener-cicd-cli-1.2066.0/bin/launch-dockerd.sh`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2065.0/bin/purge_history` & `gardener-cicd-cli-1.2066.0/bin/purge_history`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2065.0/gardener_ci/_cfg_mgmt.py` & `gardener-cicd-cli-1.2066.0/gardener_ci/_cfg_mgmt.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2065.0/gardener_ci/_clamav.py` & `gardener-cicd-cli-1.2066.0/gardener_ci/_clamav.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2065.0/gardener_ci/_concourse.py` & `gardener-cicd-cli-1.2066.0/gardener_ci/_concourse.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2065.0/gardener_ci/_oci.py` & `gardener-cicd-cli-1.2066.0/gardener_ci/_oci.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,18 +179,20 @@
             accept=accept,
         )
 
         pprint.pprint(manifest.as_dict())
 
         if isinstance(manifest, om.OciImageManifest):
             total_size = sum(blob.size for blob in manifest.blobs())
-            manifest_digest = hashlib.sha256(manifest_raw.content).hexdigest()
+            manifest_raw_bytes = manifest_raw.content
+            manifest_size = len(manifest_raw_bytes)
+            manifest_digest = hashlib.sha256(manifest_raw_bytes).hexdigest()
 
             print()
-            print(f'{total_size=} {manifest_digest=}')
+            print(f'{total_size=} {manifest_digest=} {manifest_size=}')
         elif isinstance(manifest, om.OciImageManifestList):
             manifest_digest = hashlib.sha256(manifest_raw.content).hexdigest()
             print()
             print(f'{manifest_digest=}')
 
     else:
         manifest = oci_client.manifest_raw(
@@ -257,15 +259,25 @@
     print(patched_ref)
 
 
 def osinfo(image_reference: str):
     oci_client = ccc.oci.oci_client()
 
     with tempfile.TemporaryFile() as tmpf:
-        manifest = oci_client.manifest(image_reference=image_reference)
+        manifest = oci_client.manifest(
+            image_reference=image_reference,
+            accept=om.MimeTypes.prefer_multiarch,
+        )
+
+        if isinstance(manifest, om.OciImageManifestList):
+            img_ref = om.OciImageReference(image_reference)
+            sub_img_ref = f'{img_ref.ref_without_tag}@{manifest.manifests[0].digest}'
+
+            manifest = oci_client.manifest(sub_img_ref)
+
         first_layer_blob = oci_client.blob(
             image_reference=image_reference,
             digest=manifest.layers[0].digest,
         )
         for chunk in first_layer_blob.iter_content(chunk_size=4096):
             tmpf.write(chunk)
```

### Comparing `gardener-cicd-cli-1.2065.0/gardener_ci/_osinfo.py` & `gardener-cicd-cli-1.2066.0/gardener_ci/_osinfo.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2065.0/gardener_ci/bdba.py` & `gardener-cicd-cli-1.2066.0/gardener_ci/bdba.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2065.0/gardener_ci/cd.py` & `gardener-cicd-cli-1.2066.0/gardener_ci/cd.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2065.0/gardener_ci/checkmarx_cli.py` & `gardener-cicd-cli-1.2066.0/gardener_ci/checkmarx_cli.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2065.0/gardener_ci/cli_gen.py` & `gardener-cicd-cli-1.2066.0/gardener_ci/cli_gen.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2065.0/gardener_ci/compliance.py` & `gardener-cicd-cli-1.2066.0/gardener_ci/compliance.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2065.0/gardener_ci/config.py` & `gardener-cicd-cli-1.2066.0/gardener_ci/config.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2065.0/gardener_ci/containerutil.py` & `gardener-cicd-cli-1.2066.0/gardener_ci/containerutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2065.0/gardener_ci/docker.py` & `gardener-cicd-cli-1.2066.0/gardener_ci/docker.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2065.0/gardener_ci/elastic.py` & `gardener-cicd-cli-1.2066.0/gardener_ci/elastic.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2065.0/gardener_ci/gh.py` & `gardener-cicd-cli-1.2066.0/gardener_ci/gh.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2065.0/gardener_ci/githubutil.py` & `gardener-cicd-cli-1.2066.0/gardener_ci/githubutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2065.0/gardener_ci/ocm.py` & `gardener-cicd-cli-1.2066.0/gardener_ci/ocm.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2065.0/gardener_ci/pipeline.py` & `gardener-cicd-cli-1.2066.0/gardener_ci/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -406,17 +406,15 @@
         '--component-name', base_component.name,
     ))
 
     env = os.environ.copy()
     env |= {
         'MAIN_REPO_DIR': repo.working_tree_dir,
         'BASE_DEFINITION_PATH': base_component_descriptor_file.name,
-        # BASE_CTF_PATH - XXX
         'COMPONENT_DESCRIPTOR_PATH': outfile,
-        # CTF_PATH - XXX
         'COMPONENT_NAME': base_component.name,
         'COMPONENT_VERSION': base_component.version,
         'EFFECTIVE_VERSION': base_component.version,
         'CURRENT_COMPONENT_REPOSITORY': component_repo,
         'ADD_DEPENDENCIES_CMD': dependencies_cmd,
     }
```

### Comparing `gardener-cicd-cli-1.2065.0/gardener_ci/productutil_v2.py` & `gardener-cicd-cli-1.2066.0/gardener_ci/productutil_v2.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2065.0/gardener_ci/whdutil.py` & `gardener-cicd-cli-1.2066.0/gardener_ci/whdutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2065.0/gardener_cicd_cli.egg-info/SOURCES.txt` & `gardener-cicd-cli-1.2066.0/gardener_cicd_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2065.0/setup.py` & `gardener-cicd-cli-1.2066.0/setup.py`

 * *Files identical despite different names*

