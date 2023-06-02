# Comparing `tmp/resoto-plugin-digitalocean-3.5.0.tar.gz` & `tmp/resoto-plugin-digitalocean-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-digitalocean-3.5.0.tar", last modified: Fri May 26 18:24:03 2023, max compression
+gzip compressed data, was "resoto-plugin-digitalocean-3.5.1.tar", last modified: Fri Jun  2 14:55:23 2023, max compression
```

## Comparing `resoto-plugin-digitalocean-3.5.0.tar` & `resoto-plugin-digitalocean-3.5.1.tar`

### file list

```diff
@@ -1,53 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:03.665267 resoto-plugin-digitalocean-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-26 18:24:03.665267 resoto-plugin-digitalocean-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:03.657267 resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean/
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15090 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    43809 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    19972 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:03.657267 resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-26 18:24:03.000000 resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-26 18:24:03.000000 resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:24:03.000000 resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-26 18:24:03.000000 resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:24:03.000000 resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-26 18:24:03.000000 resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-26 18:24:03.000000 resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 18:24:03.665267 resoto-plugin-digitalocean-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:03.661267 resoto-plugin-digitalocean-3.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:03.665267 resoto-plugin-digitalocean-3.5.0/test/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/cdns.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/domain_records.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/domains.py
--rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/droplets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/firewalls.py
--rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/floatingip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/loadbalancers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/projectresources.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/regions.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/registry_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/registry_repository_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/spaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/ssh_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/volumes.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/vpcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23723 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:55:23.034830 resoto-plugin-digitalocean-3.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-02 14:55:23.034830 resoto-plugin-digitalocean-3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:55:23.026830 resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean/
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15090 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43638 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19972 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:55:23.026830 resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-02 14:55:23.000000 resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-02 14:55:23.000000 resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:55:23.000000 resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-02 14:55:23.000000 resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:51:36.000000 resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-02 14:55:23.000000 resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-02 14:55:23.000000 resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 14:55:23.034830 resoto-plugin-digitalocean-3.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:55:23.030830 resoto-plugin-digitalocean-3.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:55:23.034830 resoto-plugin-digitalocean-3.5.1/test/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/cdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/domain_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/droplets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/firewalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/floatingip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/loadbalancers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/projectresources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/registry_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/registry_repository_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/spaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/ssh_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/volumes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/vpcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25604 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/test_config.py
```

### Comparing `resoto-plugin-digitalocean-3.5.0/PKG-INFO` & `resoto-plugin-digitalocean-3.5.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-digitalocean
-Version: 3.5.0
+Version: 3.5.1
 Summary: Resoto DigitalOcean Collector Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/digitalocean
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/digitalocean
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 
 # resoto-plugin-digitalocean
 DigitalOcean Collector Plugin for Resoto
```

### Comparing `resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean/__init__.py` & `resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean/client.py` & `resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean/client.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean/collector.py` & `resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean/collector.py`

 * *Files 12% similar despite different names*

```diff
@@ -316,18 +316,18 @@
                 search_result = self.graph.search_first(search_attr, search_value)
                 if search_result:
                     if map_to not in search_results:
                         search_results[map_to] = []
                     search_results[map_to].append(search_result)
             if map_to not in kwargs and map_to in search_results and not str(map_to).startswith("__"):
                 search_result = search_results[map_to]
-                if len(search_result) == 1:
-                    kwargs[map_to] = search_result[0]
+                if len(search_result) == 1:  # type: ignore
+                    kwargs[map_to] = search_result[0]  # type: ignore
                 else:
-                    kwargs[map_to] = list(search_result)
+                    kwargs[map_to] = list(search_result)  # type: ignore
 
         # If the resource was referencing a zone but not a region we look up its
         # region based on the zone information we found.
         # E.g. if we know a disk is in zone us-central1-a then we can find
         # the region us-central1 from that.
         if "_zone" in kwargs and "_region" not in kwargs and isinstance(kwargs["_zone"], BaseResource):
             region = kwargs["_zone"].region(self.graph)
@@ -419,15 +419,15 @@
                             add_edge(search_result_name, is_parent)
                         else:
                             if search_result_name in search_map:
                                 add_deferred_connection(search_map, search_result_name, is_parent, edge_type)
                             else:
                                 log.error(f"Key {search_result_name} is missing in search_map")
 
-    @metrics_collect_droplets.time()  # type: ignore
+    @metrics_collect_droplets.time()
     def collect_droplets(self) -> None:
         instances = self.client.list_droplets()
 
         def get_image(droplet: Json) -> Json:
             image = droplet["image"]
             image["region"] = droplet["region"]["slug"]
             return cast(Json, image)
@@ -530,15 +530,15 @@
             },
             predecessors={
                 EdgeType.default: ["__vpcs", "__images", "__sizes", "__tags"],
                 EdgeType.delete: ["__vpcs"],
             },
         )
 
-    @metrics_collect_regions.time()  # type: ignore
+    @metrics_collect_regions.time()
     def collect_regions(self) -> None:
         regions = self.client.list_regions()
         self.collect_resource(
             regions,
             resource_class=DigitalOceanRegion,
             attr_map={
                 "id": "slug",
@@ -547,15 +547,15 @@
                 "do_region_slug": "slug",
                 "do_region_features": "features",
                 "is_available": "available",
                 "do_region_droplet_sizes": "sizes",
             },
         )
 
-    @metrics_collect_volumes.time()  # type: ignore
+    @metrics_collect_volumes.time()
     def collect_volumes(self) -> None:
         # taken from https://www.digitalocean.com/pricing/volumes
         DO_VOLUME_COST_GB_PER_HOUR = 0.000149
         volumes = self.client.list_volumes()
 
         def extract_volume_status(volume: Json) -> VolumeStatus:
             in_use = len(volume.get("droplet_ids", []) or []) > 0
@@ -584,15 +584,15 @@
                     lambda v: list(map(lambda tag: tag_id(tag), v.get("tags", []) or [])),
                 ],
             },
             predecessors={EdgeType.default: ["__users", "__tags"]},
             successors={EdgeType.delete: ["__users"]},
         )
 
-    @metrics_collect_databases.time()  # type: ignore
+    @metrics_collect_databases.time()
     def collect_databases(self) -> None:
         # this mapping was taken from the digitalocean web console.
         dbtype_to_size = {
             "db-s-1vcpu-1gb": 10,
             "db-s-1vcpu-2gb": 25,
             "db-s-2vcpu-4gb": 38,
             "db-s-4vcpu-8gb": 115,
@@ -638,15 +638,15 @@
             },
             predecessors={
                 EdgeType.default: ["__vpcs", "__tags"],
                 EdgeType.delete: ["__vpcs"],
             },
         )
 
-    @metrics_collect_vpcs.time()  # type: ignore
+    @metrics_collect_vpcs.time()
     def collect_vpcs(self) -> None:
         vpcs = self.client.list_vpcs()
         self.collect_resource(
             vpcs,
             resource_class=DigitalOceanVPC,
             attr_map={
                 "id": "id",
@@ -656,15 +656,15 @@
                 "is_default": "default",
             },
             search_map={
                 "_region": ["urn", lambda vpc: region_id(vpc["region"])],
             },
         )
 
-    @metrics_collect_projects.time()  # type: ignore
+    @metrics_collect_projects.time()
     def collect_projects(self) -> None:
         def get_resource_id(resource: Json) -> str:
             return cast(str, resource["urn"])
 
         projects = self.client.list_projects()
         project_resources = [list(map(get_resource_id, self.client.list_project_resources(p["id"]))) for p in projects]
 
@@ -689,15 +689,15 @@
             },
             successors={
                 EdgeType.default: ["__resources"],
                 EdgeType.delete: ["__resources"],
             },
         )
 
-    @metrics_collect_k8s_clusters.time()  # type: ignore
+    @metrics_collect_k8s_clusters.time()
     def collect_k8s_clusters(self) -> None:
         clusters = self.client.list_kubernetes_clusters()
         self.collect_resource(
             clusters,
             resource_class=DigitalOceanKubernetesCluster,
             attr_map={
                 "id": "id",
@@ -725,15 +725,15 @@
                 ],
                 "__vpcs": ["urn", lambda c: vpc_id(c["vpc_uuid"])],
             },
             successors={EdgeType.default: ["__nodes"], EdgeType.delete: ["__nodes"]},
             predecessors={EdgeType.default: ["__vpcs"], EdgeType.delete: ["__vpcs"]},
         )
 
-    @metrics_collect_snapshots.time()  # type: ignore
+    @metrics_collect_snapshots.time()
     def collect_snapshots(self) -> None:
         def get_resource_id(snapshot: Json) -> str:
             if snapshot["resource_type"] == "droplet":
                 return droplet_id(snapshot["resource_id"])
             else:
                 return volume_id(snapshot["resource_id"])
 
@@ -770,15 +770,15 @@
                     "urn",
                     lambda s: list(map(lambda tag: tag_id(tag), s.get("tags", []) or [])),
                 ],
             },
             predecessors={EdgeType.default: ["__resource", "__tags", "__available_regions"]},
         )
 
-    @metrics_collect_load_balancers.time()  # type: ignore
+    @metrics_collect_load_balancers.time()
     def collect_load_balancers(self) -> None:
         loadbalancers = self.client.list_load_balancers()
 
         def get_nr_nodes(lb: Json) -> int:
             size_to_nr_nodes = {
                 "lb-small": 1,
                 "lb-medium": 3,
@@ -794,14 +794,15 @@
             resource_class=DigitalOceanLoadBalancer,
             attr_map={
                 "id": "id",
                 "urn": lambda lb: loadbalancer_id(lb["id"]),
                 "public_ip_address": "ip",
                 "nr_nodes": get_nr_nodes,
                 "loadbalancer_status": "status",
+                "backends": lambda lb: [droplet_id(id) for id in (lb.get("droplet_ids", []) or [])],
                 "redirect_http_to_https": "redirect_http_to_https",
                 "enable_proxy_protocol": "enable_proxy_protocol",
                 "enable_backend_keepalive": "enable_backend_keepalive",
                 "disable_lets_encrypt_dns_records": "disable_lets_encrypt_dns_records",
             },
             search_map={
                 "_region": ["urn", lambda lb: region_id(lb["region"]["slug"])],
@@ -811,15 +812,15 @@
                     lambda lb: list(map(lambda id: droplet_id(id), lb.get("droplet_ids", []) or [])),
                 ],
             },
             predecessors={EdgeType.default: ["__vpcs"], EdgeType.delete: ["__vpcs"]},
             successors={EdgeType.default: ["__droplets"]},
         )
 
-    @metrics_collect_floating_ips.time()  # type: ignore
+    @metrics_collect_floating_ips.time()
     def collect_floating_ips(self) -> None:
         floating_ips = self.client.list_floating_ips()
         self.collect_resource(
             floating_ips,
             resource_class=DigitalOceanFloatingIP,
             attr_map={
                 "id": "ip",
@@ -834,15 +835,15 @@
                     "urn",
                     lambda ip: droplet_id(ip.get("droplet", {}).get("id", "")),
                 ],
             },
             predecessors={EdgeType.default: ["__droplet"]},
         )
 
-    @metrics_collect_spaces.time()  # type: ignore
+    @metrics_collect_spaces.time()
     def collect_spaces(self, region: DigitalOceanRegion) -> None:
         spaces = self.client.list_spaces(region.do_region_slug or "")
         self.collect_resource(
             spaces,
             resource_class=DigitalOceanSpace,
             attr_map={
                 "id": "Name",
@@ -854,15 +855,15 @@
                 "_region": [
                     "urn",
                     lambda space: region_id(region.do_region_slug or ""),
                 ],
             },
         )
 
-    @metrics_collect_apps.time()  # type: ignore
+    @metrics_collect_apps.time()
     def collect_apps(self) -> None:
         apps = self.client.list_apps()
 
         def extract_region(app: Json) -> Optional[str]:
             region_slug = next(iter(app.get("region", {}).get("data_centers", [])), None)
             if region_slug is None:
                 return None
@@ -888,15 +889,15 @@
             search_map={
                 "_region": ["urn", extract_region],
                 "__databases": ["name", extract_databases],
             },
             predecessors={EdgeType.default: ["__databases"]},
         )
 
-    @metrics_collect_cdn_endpoints.time()  # type: ignore
+    @metrics_collect_cdn_endpoints.time()
     def collect_cdn_endpoints(self) -> None:
         endpoints = self.client.list_cdn_endpoints()
         self.collect_resource(
             endpoints,
             resource_class=DigitalOceanCdnEndpoint,
             attr_map={
                 "id": "id",
@@ -905,15 +906,15 @@
                 "endpoint": "endpoint",
                 "certificate_id": "certificate_id",
                 "custom_domain": "custom_domain",
                 "ttl": "ttl",
             },
         )
 
-    @metrics_collect_certificates.time()  # type: ignore
+    @metrics_collect_certificates.time()
     def collect_certificates(self) -> None:
         certificates = self.client.list_certificates()
         self.collect_resource(
             certificates,
             resource_class=DigitalOceanCertificate,
             attr_map={
                 "id": "id",
@@ -922,15 +923,15 @@
                 "sha1_fingerprint": "sha1_fingerprint",
                 "dns_names": "dns_names",
                 "certificate_state": "state",
                 "certificate_type": "type",
             },
         )
 
-    @metrics_collect_container_registry.time()  # type: ignore
+    @metrics_collect_container_registry.time()
     def collect_container_registry(self) -> None:
         registries = self.client.get_registry_info()
         for registry in registries:
             registry["updated_at"] = registry["storage_usage_updated_at"]
             self.collect_resource(
                 [registry],
                 resource_class=DigitalOceanContainerRegistry,
@@ -994,41 +995,41 @@
                         "urn",
                         lambda t: container_registry_id(t["registry_name"]),
                     ],
                 },
                 predecessors={EdgeType.default: ["__repository", "__registry"]},
             )
 
-    @metrics_collect_ssh_keys.time()  # type: ignore
+    @metrics_collect_ssh_keys.time()
     def collect_ssh_keys(self) -> None:
         ssh_keys = self.client.list_ssh_keys()
         self.collect_resource(
             ssh_keys,
             resource_class=DigitalOceanSSHKey,
             attr_map={
                 "id": lambda k: str(k["id"]),
                 "urn": lambda k: ssh_key_id(k["id"]),
                 "public_key": "public_key",
                 "fingerprint": "fingerprint",
             },
         )
 
-    @metrics_collect_tags.time()  # type: ignore
+    @metrics_collect_tags.time()
     def collect_tags(self) -> None:
         tags = self.client.list_tags()
         self.collect_resource(
             tags,
             resource_class=DigitalOceanTag,
             attr_map={
                 "id": "name",
                 "urn": lambda t: tag_id(t["name"]),
             },
         )
 
-    @metrics_collect_domains.time()  # type: ignore
+    @metrics_collect_domains.time()
     def collect_domains(self) -> None:
         domains = self.client.list_domains()
         self.collect_resource(
             domains,
             resource_class=DigitalOceanDomain,
             attr_map={
                 "id": "name",
@@ -1066,15 +1067,15 @@
             },
             search_map={
                 "__domain": ["urn", lambda r: domain_id(r["domain_name"])],
             },
             predecessors={EdgeType.default: ["__domain"]},
         )
 
-    @metrics_collect_firewalls.time()  # type: ignore
+    @metrics_collect_firewalls.time()
     def collect_firewalls(self) -> None:
         firewalls = self.client.list_firewalls()
         self.collect_resource(
             firewalls,
             resource_class=DigitalOceanFirewall,
             attr_map={
                 "id": "id",
@@ -1095,15 +1096,15 @@
                 EdgeType.default: ["__tags"],
             },
             successors={
                 EdgeType.default: ["__droplets"],
             },
         )
 
-    @metrics_collect_alert_policies.time()  # type: ignore
+    @metrics_collect_alert_policies.time()
     def collect_alert_policies(self) -> None:
         alert_policies = self.client.list_alert_policies()
         self.collect_resource(
             alert_policies,
             resource_class=DigitalOceanAlertPolicy,
             attr_map={
                 "id": "uuid",
```

### Comparing `resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean/resources.py` & `resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean/utils.py` & `resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean/utils.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean.egg-info/PKG-INFO` & `resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-digitalocean
-Version: 3.5.0
+Version: 3.5.1
 Summary: Resoto DigitalOcean Collector Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/digitalocean
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/digitalocean
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 
 # resoto-plugin-digitalocean
 DigitalOcean Collector Plugin for Resoto
```

### Comparing `resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean.egg-info/SOURCES.txt` & `resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 MANIFEST.in
 README.md
-requirements-test.txt
-requirements.txt
+pyproject.toml
 setup.cfg
-setup.py
 resoto_plugin_digitalocean/__init__.py
 resoto_plugin_digitalocean/client.py
 resoto_plugin_digitalocean/collector.py
 resoto_plugin_digitalocean/config.py
 resoto_plugin_digitalocean/resources.py
 resoto_plugin_digitalocean/utils.py
 resoto_plugin_digitalocean.egg-info/PKG-INFO
```

### Comparing `resoto-plugin-digitalocean-3.5.0/setup.py` & `resoto-plugin-digitalocean-3.5.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,54 @@
-import os
-import pkg_resources
-from setuptools import setup, find_packages
-
-
-def read(file_name: str) -> str:
-    with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
-        return of.read()
-
-
-setup(
-    name="resoto-plugin-digitalocean",
-    version="3.5.0",
-    description="Resoto DigitalOcean Collector Plugin",
-    license="Apache 2.0",
-    packages=find_packages(),
-    long_description=read("README.md"),
-    long_description_content_type="text/markdown",
-    entry_points={
-        "resoto.plugins": ["digitalocean_collector = resoto_plugin_digitalocean:DigitalOceanCollectorPlugin"]
-    },
-    include_package_data=True,
-    zip_safe=False,
-    install_requires=[str(requirement) for requirement in pkg_resources.parse_requirements(read("requirements.txt"))],
-    setup_requires=["pytest-runner"],
-    tests_require=["pytest"],
-    classifiers=[
-        # Current project status
-        "Development Status :: 4 - Beta",
-        # Audience
-        "Intended Audience :: System Administrators",
-        "Intended Audience :: Information Technology",
-        # License information
-        "License :: OSI Approved :: Apache Software License",
-        # Supported python versions
-        "Programming Language :: Python :: 3.9",
-        # Supported OS's
-        "Operating System :: POSIX :: Linux",
-        "Operating System :: Unix",
-        # Extra metadata
-        "Environment :: Console",
-        "Natural Language :: English",
-        "Topic :: Security",
-        "Topic :: Utilities",
-    ],
-    keywords="cloud security",
-    url="https://github.com/someengineering/resoto/tree/main/plugins/digitalocean",
-)
+[project]
+name = "resoto-plugin-digitalocean"
+description = "Resoto DigitalOcean Collector Plugin"
+version = "3.5.1"
+authors = [{name="Some Engineering Inc."}]
+license = {file="LICENSE"}
+requires-python = ">=3.9"
+classifiers = [
+    # Current project status
+    "Development Status :: 4 - Beta",
+    # Audience
+    "Intended Audience :: System Administrators",
+    "Intended Audience :: Information Technology",
+    # License information
+    "License :: OSI Approved :: Apache Software License",
+    # Supported python versions
+    "Programming Language :: Python :: 3.9",
+    # Supported OS's
+    "Operating System :: POSIX :: Linux",
+    "Operating System :: Unix",
+    # Extra metadata
+    "Environment :: Console",
+    "Natural Language :: English",
+    "Topic :: Security",
+    "Topic :: Utilities",
+]
+readme = {file="README.md", content-type="text/markdown"}
+
+dependencies = [
+    "resotolib==3.5.1",
+    "boto3",
+    "requests",
+    "botocore",
+    "retrying"
+]
+
+[project.optional-dependencies]
+dev = [
+    "mypy",
+    "tzlocal",
+]
+
+[project.entry-points."resoto.plugins"]
+digitalocean_collector = "resoto_plugin_digitalocean:DigitalOceanCollectorPlugin"
+
+[project.urls]
+Documentation = "https://resoto.com"
+Source = "https://github.com/someengineering/resoto/tree/main/plugins/digitalocean"
+
+[build-system]
+requires = ["setuptools>=67.8.0", "wheel>=0.40.0", "build>=0.10.0"]
+build-backend = "setuptools.build_meta"
+
+
```

### Comparing `resoto-plugin-digitalocean-3.5.0/test/fixtures/__init__.py` & `resoto-plugin-digitalocean-3.5.1/test/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.0/test/fixtures/apps.py` & `resoto-plugin-digitalocean-3.5.1/test/fixtures/apps.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.0/test/fixtures/databases.py` & `resoto-plugin-digitalocean-3.5.1/test/fixtures/databases.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.0/test/fixtures/domain_records.py` & `resoto-plugin-digitalocean-3.5.1/test/fixtures/domain_records.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.0/test/fixtures/droplets.py` & `resoto-plugin-digitalocean-3.5.1/test/fixtures/droplets.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.0/test/fixtures/firewalls.py` & `resoto-plugin-digitalocean-3.5.1/test/fixtures/firewalls.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.0/test/fixtures/floatingip.py` & `resoto-plugin-digitalocean-3.5.1/test/fixtures/floatingip.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.0/test/fixtures/k8s.py` & `resoto-plugin-digitalocean-3.5.1/test/fixtures/k8s.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.0/test/fixtures/loadbalancers.py` & `resoto-plugin-digitalocean-3.5.1/test/fixtures/loadbalancers.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.0/test/fixtures/projectresources.py` & `resoto-plugin-digitalocean-3.5.1/test/fixtures/projectresources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.0/test/fixtures/projects.py` & `resoto-plugin-digitalocean-3.5.1/test/fixtures/projects.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.0/test/fixtures/regions.py` & `resoto-plugin-digitalocean-3.5.1/test/fixtures/regions.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.0/test/fixtures/registry_repositories.py` & `resoto-plugin-digitalocean-3.5.1/test/fixtures/registry_repositories.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.0/test/fixtures/tags.py` & `resoto-plugin-digitalocean-3.5.1/test/fixtures/tags.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.0/test/fixtures/volumes.py` & `resoto-plugin-digitalocean-3.5.1/test/fixtures/volumes.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.0/test/test_collector.py` & `resoto-plugin-digitalocean-3.5.1/test/test_collector.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,44 @@
-from resoto_plugin_digitalocean.collector import DigitalOceanTeamCollector
-from resoto_plugin_digitalocean.resources import DigitalOceanTeam, DigitalOceanVolume, DigitalOceanDropletSize
+import datetime
+from typing import Dict, Any, List, cast
+
 from resoto_plugin_digitalocean.client import StreamingWrapper
+from resoto_plugin_digitalocean.collector import DigitalOceanTeamCollector
+from resoto_plugin_digitalocean.resources import (
+    DigitalOceanTeam,
+    DigitalOceanVolume,
+    DigitalOceanDropletSize,
+    DigitalOceanRegion,
+    DigitalOceanVPC,
+    DigitalOceanImage,
+    DigitalOceanDroplet,
+    DigitalOceanDatabase,
+    DigitalOceanKubernetesCluster,
+    DigitalOceanSnapshot,
+    DigitalOceanLoadBalancer,
+    DigitalOceanFloatingIP,
+    DigitalOceanProject,
+    DigitalOceanSpace,
+    DigitalOceanApp,
+    DigitalOceanCdnEndpoint,
+    DigitalOceanCertificate,
+    DigitalOceanContainerRegistry,
+    DigitalOceanContainerRegistryRepositoryTag,
+    DigitalOceanContainerRegistryRepository,
+    DigitalOceanSSHKey,
+    DigitalOceanTag,
+    DigitalOceanDomain,
+    DigitalOceanDomainRecord,
+    DigitalOceanFirewall,
+    DigitalOceanAlertPolicy,
+)
+from resotolib.baseresources import Cloud, EdgeType, GraphRoot, InstanceStatus, VolumeStatus
 from resotolib.core.actions import CoreFeedback
+from resotolib.graph import Graph
+from resotolib.graph import sanitize
 from .fixtures import (
     droplets,
     regions,
     volumes,
     vpcs,
     databases,
     k8s,
@@ -24,23 +57,19 @@
     ssh_keys,
     tags,
     domains,
     domain_records,
     firewalls,
     alerts,
 )
-from resotolib.graph import sanitize
-from resotolib.baseresources import Cloud, EdgeType, GraphRoot, InstanceStatus, VolumeStatus
-from resotolib.graph import Graph
-import datetime
-from typing import Dict, Any, List, cast
 
 
 class ClientMock(StreamingWrapper, object):
     def __init__(self, responses: Dict[str, Any]) -> None:
+        super().__init__("none", None, None, None)
         self.responses = responses
 
     def with_feedback(self, core_feedback: CoreFeedback) -> StreamingWrapper:
         return ClientMock(self.responses)
 
     def __getattribute__(self, name):  # type: ignore
         responses = super().__getattribute__("responses")
@@ -77,15 +106,15 @@
     assert False, f"Edge {from_id} -> {to_id} not found"
 
 
 def test_collect_teams() -> None:
     do_client = ClientMock({})
     graph = prepare_graph(do_client)
 
-    team_node = graph.search_first("urn", "do:team:test_team")
+    team_node: DigitalOceanTeam = graph.search_first("urn", "do:team:test_team")  # type: ignore
     assert team_node.name == "test_team"
     assert team_node.urn == "do:team:test_team"
     assert team_node.id == "test_team"
 
 
 def test_collect_regions() -> None:
     do_client = ClientMock({"list_regions": regions, "list_droplets": droplets})
@@ -94,43 +123,43 @@
 
     check_edges(graph, "do:team:test_team", "do:region:fra1")
     check_edges(graph, "do:region:fra1", "do:droplet:289110074")
 
     # region nyc1 should not be in the graph since it has no resources in it
     assert graph.search_first("urn", "do:region:nyc1") is None
 
-    region = graph.search_first("urn", "do:region:fra1")
+    region: DigitalOceanRegion = graph.search_first("urn", "do:region:fra1")  # type: ignore
     assert region.name == "Frankfurt 1"
     assert region.id == "fra1"
     assert region.kind == "digitalocean_region"
     assert region.do_region_slug == "fra1"
     assert region.do_region_features == [
         "backups",
         "ipv6",
         "metadata",
         "install_agent",
         "storage",
         "image_transfer",
     ]
     droplet_sizes: List[str] = regions[1]["sizes"]
-    assert set(region.do_region_droplet_sizes) == set(droplet_sizes)
+    assert set(region.do_region_droplet_sizes) == set(droplet_sizes)  # type: ignore
     assert region.is_available is True
 
 
 def test_collect_vpcs() -> None:
     do_client = ClientMock(
         {
             "list_regions": regions,
             "list_vpcs": vpcs,
         }
     )
     graph = prepare_graph(do_client)
 
     check_edges(graph, "do:region:fra1", "do:vpc:0d3176ad-41e0-4021-b831-0c5c45c60959")
-    vpc = graph.search_first("urn", "do:vpc:0d3176ad-41e0-4021-b831-0c5c45c60959")
+    vpc: DigitalOceanVPC = graph.search_first("urn", "do:vpc:0d3176ad-41e0-4021-b831-0c5c45c60959")  # type: ignore
     assert vpc.urn == "do:vpc:0d3176ad-41e0-4021-b831-0c5c45c60959"
     assert vpc.name == "default-fra1"
     assert vpc.description == ""
     assert vpc.ip_range == "127.0.0.1/20"
     assert vpc.is_default is True
 
 
@@ -153,15 +182,15 @@
         "do:droplet:289110074",
         delete=True,
     )
     check_edges(graph, "do:image:101111514", "do:droplet:289110074")
     check_edges(graph, "do:size:s-1vcpu-1gb", "do:droplet:289110074")
     check_edges(graph, "do:tag:image_tag", "do:image:101111514")
     check_edges(graph, "do:tag:droplet_tag", "do:droplet:289110074")
-    image = graph.search_first("urn", "do:image:101111514")
+    image: DigitalOceanImage = graph.search_first("urn", "do:image:101111514")  # type: ignore
     assert image.urn == "do:image:101111514"
     assert image.name == "20.04 (LTS) x64"
     assert image.distribution == "Ubuntu"
     assert image.image_slug == "ubuntu-20-04-x64"
     assert image.is_public is True
     assert image.image_type == "base"
     assert image.size_gigabytes == 1
@@ -172,21 +201,21 @@
     size = cast(DigitalOceanDropletSize, graph.search_first("urn", "do:size:s-1vcpu-1gb"))
     assert size.urn == "do:size:s-1vcpu-1gb"
     assert size.instance_type == "s-1vcpu-1gb"
     assert size.instance_cores == 1
     assert size.instance_memory == 1
     assert size.ondemand_cost == 0.00744
 
-    droplet = graph.search_first("urn", "do:droplet:289110074")
+    droplet: DigitalOceanDroplet = graph.search_first("urn", "do:droplet:289110074")  # type: ignore
     assert droplet.urn == "do:droplet:289110074"
     assert droplet.name == "ubuntu-s-1vcpu-1gb-fra1-01"
     assert droplet.instance_memory == 1
     assert droplet.instance_cores == 1
     assert droplet.instance_status == InstanceStatus.RUNNING
-    assert droplet.region().urn == "do:region:fra1"
+    assert droplet.region().urn == "do:region:fra1"  # type: ignore
     assert droplet.droplet_image == "ubuntu-20-04-x64"
     assert droplet.droplet_backup_ids == ["42"]
     assert droplet.is_locked is False
     assert droplet.ctime == datetime.datetime(2022, 3, 3, 16, 26, 55, tzinfo=datetime.timezone.utc)
     assert droplet.tags == {"droplet_tag": None}
 
 
@@ -233,22 +262,22 @@
     check_edges(
         graph,
         "do:vpc:0d3176ad-41e0-4021-b831-0c5c45c60959",
         "do:dbaas:2848a998-e151-4d5a-9813-0904a44c2397",
         delete=True,
     )
     check_edges(graph, "do:tag:database_tag", "do:dbaas:2848a998-e151-4d5a-9813-0904a44c2397")
-    database = graph.search_first("urn", "do:dbaas:2848a998-e151-4d5a-9813-0904a44c2397")
+    database: DigitalOceanDatabase = graph.search_first("urn", "do:dbaas:2848a998-e151-4d5a-9813-0904a44c2397")  # type: ignore # noqa: E501
     assert database.urn == "do:dbaas:2848a998-e151-4d5a-9813-0904a44c2397"
     assert database.name == "do:dbaas:db-postgresql-fra1-82725"
     assert database.db_type == "pg"
     assert database.db_status == "online"
     assert database.db_version == "14"
     assert database.db_endpoint == "host.b.db.ondigitalocean.com"
-    assert database.region().urn == "do:region:fra1"
+    assert database.region().urn == "do:region:fra1"  # type: ignore
     assert database.instance_type == "db-s-1vcpu-1gb"
 
 
 def test_collect_k8s_clusters() -> None:
     do_client = ClientMock(
         {
             "list_regions": regions,
@@ -272,19 +301,19 @@
     )
     check_edges(
         graph,
         "do:kubernetes:e1c48631-b382-4001-2168-c47c54795a26",
         "do:droplet:290075243",
     )
 
-    cluster = graph.search_first("urn", "do:kubernetes:e1c48631-b382-4001-2168-c47c54795a26")
+    cluster: DigitalOceanKubernetesCluster = graph.search_first("urn", "do:kubernetes:e1c48631-b382-4001-2168-c47c54795a26")  # type: ignore # noqa: E501
     assert cluster.urn == "do:kubernetes:e1c48631-b382-4001-2168-c47c54795a26"
     assert cluster.name == "k8s-1-22-7-do-0-fra1-test"
     assert cluster.k8s_version == "1.22.7-do.0"
-    assert cluster.region().urn == "do:region:fra1"
+    assert cluster.region().urn == "do:region:fra1"  # type: ignore
     assert cluster.k8s_cluster_subnet == "10.244.0.0/16"
     assert cluster.k8s_service_subnet == "10.245.0.0/16"
     assert cluster.ipv4_address == "127.0.0.1"
     assert cluster.endpoint == "https://e1c48631-b382-4001-2168-c47c54795a26.k8s.ondigitalocean.com"
     assert cluster.auto_upgrade_enabled is False
     assert cluster.cluster_status == "running"
     assert cluster.surge_upgrade_enabled is True
@@ -301,15 +330,15 @@
             "list_tags": tags,
         }
     )
     graph = prepare_graph(do_client)
 
     check_edges(graph, "do:droplet:289110074", "do:snapshot:103198134")
     check_edges(graph, "do:tag:snapshot_tag", "do:snapshot:103198134")
-    snapshot = graph.search_first("urn", "do:snapshot:103198134")
+    snapshot: DigitalOceanSnapshot = graph.search_first("urn", "do:snapshot:103198134")  # type: ignore
     assert snapshot.urn == "do:snapshot:103198134"
     assert snapshot.volume_size == 25
     assert snapshot.snapshot_size_gigabytes == 2
     assert snapshot.resource_id == "289110074"
     assert snapshot.resource_type == "droplet"
 
 
@@ -336,15 +365,15 @@
         delete=True,
     )
     check_edges(
         graph,
         "do:loadbalancer:9625f517-75f0-4af8-a336-62374e68dc0d",
         "do:droplet:289110074",
     )
-    lb = graph.search_first("urn", "do:loadbalancer:9625f517-75f0-4af8-a336-62374e68dc0d")
+    lb: DigitalOceanLoadBalancer = graph.search_first("urn", "do:loadbalancer:9625f517-75f0-4af8-a336-62374e68dc0d")  # type: ignore # noqa: E501
     assert lb.urn == "do:loadbalancer:9625f517-75f0-4af8-a336-62374e68dc0d"
     assert lb.name == "fra1-load-balancer-01"
     assert lb.public_ip_address == "127.0.0.1"
     assert lb.nr_nodes == 1
     assert lb.loadbalancer_status == "new"
     assert lb.redirect_http_to_https is False
     assert lb.enable_proxy_protocol is False
@@ -358,15 +387,15 @@
             "list_regions": regions,
             "list_floating_ips": floating_ips,
             "list_droplets": droplets,
         }
     )
     graph = prepare_graph(do_client)
     check_edges(graph, "do:droplet:289110074", "do:floatingip:127.0.0.1")
-    floating_ip = graph.search_first("urn", "do:floatingip:127.0.0.1")
+    floating_ip: DigitalOceanFloatingIP = graph.search_first("urn", "do:floatingip:127.0.0.1")  # type: ignore
     assert floating_ip.urn == "do:floatingip:127.0.0.1"
     assert floating_ip.ip_address == "127.0.0.1"
     assert floating_ip.ip_address_family == "ipv4"
     assert floating_ip.is_locked is False
 
 
 def test_collect_projects() -> None:
@@ -412,15 +441,15 @@
         "do:volume:631f81d2-9fc1-11ec-800c-0a58ac14d197",
     )
     check_edges(
         graph,
         "do:project:75088298-73bd-4c8f-ba4b-91fc220d0ac7",
         "do:space:api-test-space.resoto",
     )
-    project = graph.search_first("urn", "do:project:75088298-73bd-4c8f-ba4b-91fc220d0ac7")
+    project: DigitalOceanProject = graph.search_first("urn", "do:project:75088298-73bd-4c8f-ba4b-91fc220d0ac7")  # type: ignore # noqa: E501
     assert project.owner_uuid == "d63ae7cb6500140c46fdb3585b0c1a874e195760"
     assert project.owner_id == "10225075"
     assert project.name == "Resoto DO plugin test project"
     assert project.description == "A project to validate assumptions about how API works"
     assert project.purpose == "Just trying out DigitalOcean"
     assert project.environment == "development"
     assert project.is_default is False
@@ -432,15 +461,15 @@
         {
             "list_regions": regions,
             "list_spaces": spaces,
         }
     )
     graph = prepare_graph(do_client)
     check_edges(graph, "do:region:fra1", "do:space:api-test-space.resoto")
-    space = graph.search_first("urn", "do:space:api-test-space.resoto")
+    space: DigitalOceanSpace = graph.search_first("urn", "do:space:api-test-space.resoto")  # type: ignore
     assert space.urn == "do:space:api-test-space.resoto"
     assert space.name == "api-test-space.resoto"
     assert space.ctime == datetime.datetime(2022, 2, 23, 13, 42, 21, 455000, datetime.timezone.utc)
 
 
 def test_collect_apps() -> None:
     do_client = ClientMock(
@@ -453,15 +482,15 @@
     graph = prepare_graph(do_client)
     check_edges(graph, "do:region:fra1", "do:app:5dc41512-7523-4eeb-9932-426aa570234b")
     check_edges(
         graph,
         "do:dbaas:2848a998-e151-4d5a-9813-0904a44c2397",
         "do:app:5dc41512-7523-4eeb-9932-426aa570234b",
     )
-    app = graph.search_first("urn", "do:app:5dc41512-7523-4eeb-9932-426aa570234b")
+    app: DigitalOceanApp = graph.search_first("urn", "do:app:5dc41512-7523-4eeb-9932-426aa570234b")  # type: ignore
     assert app.urn == "do:app:5dc41512-7523-4eeb-9932-426aa570234b"
     assert app.default_ingress == "https://resoto_test_app.ondigitalocean.app"
     assert app.live_url == "https://resoto_test_app.ondigitalocean.app"
     assert app.live_url_base == "https://resoto_test_app.ondigitalocean.app"
     assert app.live_domain == "resoto_test_apps.ondigitalocean.app"
 
 
@@ -474,15 +503,15 @@
     )
     graph = prepare_graph(do_client)
     check_edges(
         graph,
         "do:team:test_team",
         "do:cdn_endpoint:4edbbc3a-79a5-4950-b2d2-ae8f8f8e8e8c",
     )
-    endpoint = graph.search_first("urn", "do:cdn_endpoint:4edbbc3a-79a5-4950-b2d2-ae8f8f8e8e8c")
+    endpoint: DigitalOceanCdnEndpoint = graph.search_first("urn", "do:cdn_endpoint:4edbbc3a-79a5-4950-b2d2-ae8f8f8e8e8c")  # type: ignore # noqa: E501
     assert endpoint.urn == "do:cdn_endpoint:4edbbc3a-79a5-4950-b2d2-ae8f8f8e8e8c"
     assert endpoint.origin == "resoto_test.ams3.digitaloceanspaces.com"
     assert endpoint.endpoint == "resoto_test.ams3.cdn.digitaloceanspaces.com"
     assert endpoint.ctime == datetime.datetime(2021, 11, 16, 16, 00, 44, 0, datetime.timezone.utc)
     assert endpoint.certificate_id == "429199eb-e6c6-4ab3-bad6-f8f8f8f8f8f8"
     assert endpoint.custom_domain == "test.domain.resoto"
     assert endpoint.ttl == 3600
@@ -492,15 +521,15 @@
     do_client = ClientMock({"list_regions": regions, "list_certificates": certificates})
     graph = prepare_graph(do_client)
     check_edges(
         graph,
         "do:team:test_team",
         "do:certificate:429199eb-7137-4e2b-a15e-f74700173e3c",
     )
-    cert = graph.search_first("urn", "do:certificate:429199eb-7137-4e2b-a15e-f74700173e3c")
+    cert: DigitalOceanCertificate = graph.search_first("urn", "do:certificate:429199eb-7137-4e2b-a15e-f74700173e3c")  # type: ignore # noqa: E501
     assert cert.urn == "do:certificate:429199eb-7137-4e2b-a15e-f74700173e3c"
     assert cert.name == "cdn.resoto.test"
     assert cert.sha1_fingerprint == "5909e5e05bbce0c63c2e2523542f74700173e3c2"
     assert cert.dns_names == ["*.resoto.test", "resoto.test"]
     assert cert.certificate_state == "verified"
     assert cert.certificate_type == "custom"
 
@@ -512,34 +541,36 @@
             "get_registry_info": registry,
             "list_registry_repositories": registry_repositories,
             "list_registry_repository_tags": registry_repository_tags,
         }
     )
     graph = prepare_graph(do_client)
     check_edges(graph, "do:region:fra1", "do:cr:resoto-do-plugin-test")
-    container_registry = graph.search_first("urn", "do:cr:resoto-do-plugin-test")
+    container_registry: DigitalOceanContainerRegistry = graph.search_first("urn", "do:cr:resoto-do-plugin-test")  # type: ignore # noqa: E501
     assert container_registry.urn == "do:cr:resoto-do-plugin-test"
     assert container_registry.name == "resoto-do-plugin-test"
     assert container_registry.storage_usage_bytes == 6144
     assert container_registry.is_read_only is False
 
     check_edges(graph, "do:cr:resoto-do-plugin-test", "do:crr:resoto-do-plugin-test/hw")
-    container_registry_repository = graph.search_first("urn", "do:crr:resoto-do-plugin-test/hw")
+    container_registry_repository: DigitalOceanContainerRegistryRepository = graph.search_first("urn", "do:crr:resoto-do-plugin-test/hw")  # type: ignore # noqa: E501
     assert container_registry_repository.urn == "do:crr:resoto-do-plugin-test/hw"
     assert container_registry_repository.name == "hw"
     assert container_registry_repository.tag_count == 1
     assert container_registry_repository.manifest_count == 1
 
     check_edges(
         graph,
         "do:crr:resoto-do-plugin-test/hw",
         "do:crrt:resoto-do-plugin-test/hw:latest",
     )
     check_edges(graph, "do:cr:resoto-do-plugin-test", "do:crrt:resoto-do-plugin-test/hw:latest")
-    tag = graph.search_first("urn", "do:crrt:resoto-do-plugin-test/hw:latest")
+    tag: DigitalOceanContainerRegistryRepositoryTag = graph.search_first(  # type: ignore
+        "urn", "do:crrt:resoto-do-plugin-test/hw:latest"
+    )
     assert tag.urn == "do:crrt:resoto-do-plugin-test/hw:latest"
     assert tag.name == "latest"
     assert tag.manifest_digest == "sha256:2ce85c6b306674dcab6eae5fda252037d58f78b0e1bbd41aabf95de6cd7e4a9e"
     assert tag.compressed_size_bytes == 5164
     assert tag.size_bytes == 12660
     assert tag.mtime == datetime.datetime(2022, 3, 14, 13, 32, 40, 0, datetime.timezone.utc)
 
@@ -549,53 +580,53 @@
         {
             "list_regions": regions,
             "list_ssh_keys": ssh_keys,
         }
     )
     graph = prepare_graph(do_client)
     check_edges(graph, "do:team:test_team", "do:ssh_key:289794")
-    ssh_key = graph.search_first("urn", "do:ssh_key:289794")
+    ssh_key: DigitalOceanSSHKey = graph.search_first("urn", "do:ssh_key:289794")  # type: ignore
     assert ssh_key.urn == "do:ssh_key:289794"
     assert ssh_key.fingerprint == "3b:16:e4:bf:8b:00:8b:b8:59:8c:a9:d3:f0:19:fa:45"
     assert ssh_key.name == "Other Public Key"
     assert ssh_key.public_key == "ssh-rsa publickey keycomment"
 
 
 def test_collect_tags() -> None:
     do_client = ClientMock(
         {
             "list_regions": regions,
             "list_tags": tags,
         }
     )
     graph = prepare_graph(do_client)
-    tag = graph.search_first("urn", "do:tag:droplet_tag")
+    tag: DigitalOceanTag = graph.search_first("urn", "do:tag:droplet_tag")  # type: ignore
     assert tag.urn == "do:tag:droplet_tag"
 
 
 def test_collect_domains() -> None:
     do_client = ClientMock(
         {
             "list_regions": regions,
             "list_domains": domains,
             "list_domain_records": domain_records,
         }
     )
     graph = prepare_graph(do_client)
     check_edges(graph, "do:team:test_team", "do:domain:do-plugin-test.resoto")
-    domain = graph.search_first("urn", "do:domain:do-plugin-test.resoto")
+    domain: DigitalOceanDomain = graph.search_first("urn", "do:domain:do-plugin-test.resoto")  # type: ignore
     assert domain.ttl == 1800
     assert domain.zone_file == "$ORIGIN do-plugin-test.resoto."
 
     check_edges(graph, "do:domain:do-plugin-test.resoto", "do:domain_record:300035870")
     check_edges(graph, "do:domain:do-plugin-test.resoto", "do:domain_record:300035871")
     check_edges(graph, "do:domain:do-plugin-test.resoto", "do:domain_record:300035872")
     check_edges(graph, "do:domain:do-plugin-test.resoto", "do:domain_record:300035874")
     check_edges(graph, "do:domain:do-plugin-test.resoto", "do:domain_record:300036132")
-    domain_record = graph.search_first("urn", "do:domain_record:300035870")
+    domain_record: DigitalOceanDomainRecord = graph.search_first("urn", "do:domain_record:300035870")  # type: ignore
     assert domain_record.urn == "do:domain_record:300035870"
     assert domain_record.name == "@"
     assert domain_record.record_type == "SOA"
     assert domain_record.record_data == "1800"
     assert domain_record.record_priority is None
     assert domain_record.record_port is None
     assert domain_record.record_ttl == 1800
@@ -616,15 +647,15 @@
     graph = prepare_graph(do_client)
     check_edges(graph, "do:tag:firewall_tag", "do:firewall:fe2e76df-3e15-4895-800f-2d5b3b807711")
     check_edges(
         graph,
         "do:firewall:fe2e76df-3e15-4895-800f-2d5b3b807711",
         "do:droplet:289110074",
     )
-    firewall = graph.search_first("urn", "do:firewall:fe2e76df-3e15-4895-800f-2d5b3b807711")
+    firewall: DigitalOceanFirewall = graph.search_first("urn", "do:firewall:fe2e76df-3e15-4895-800f-2d5b3b807711")  # type: ignore # noqa: E501
     assert firewall.firewall_status == "succeeded"
     assert firewall.ctime == datetime.datetime(2022, 3, 10, 13, 10, 50, 0, datetime.timezone.utc)
 
 
 def test_alert_policies() -> None:
     do_client = ClientMock(
         {
@@ -634,11 +665,11 @@
     )
     graph = prepare_graph(do_client)
     check_edges(
         graph,
         "do:team:test_team",
         "do:alert:d916cb34-6ee3-48c0-bca5-3f3cc08db5d3",
     )
-    alert_policy = graph.search_first("urn", "do:alert:d916cb34-6ee3-48c0-bca5-3f3cc08db5d3")
+    alert_policy: DigitalOceanAlertPolicy = graph.search_first("urn", "do:alert:d916cb34-6ee3-48c0-bca5-3f3cc08db5d3")  # type: ignore # noqa: E501
     assert alert_policy.policy_type == "v1/insights/droplet/cpu"
     assert alert_policy.description == "CPU is running high"
     assert alert_policy.is_enabled is True
```

