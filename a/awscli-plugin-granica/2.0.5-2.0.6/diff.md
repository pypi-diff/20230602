# Comparing `tmp/awscli-plugin-granica-2.0.5.tar.gz` & `tmp/awscli-plugin-granica-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awscli-plugin-granica-2.0.5.tar", last modified: Fri Jun  2 03:45:58 2023, max compression
+gzip compressed data, was "awscli-plugin-granica-2.0.6.tar", last modified: Fri Jun  2 04:14:52 2023, max compression
```

## Comparing `awscli-plugin-granica-2.0.5.tar` & `awscli-plugin-granica-2.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:45:58.359919 awscli-plugin-granica-2.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-02 03:45:48.000000 awscli-plugin-granica-2.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-02 03:45:58.359919 awscli-plugin-granica-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-02 03:45:48.000000 awscli-plugin-granica-2.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:45:58.359919 awscli-plugin-granica-2.0.5/awscli-plugin-granica/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-02 03:45:48.000000 awscli-plugin-granica-2.0.5/awscli-plugin-granica/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-02 03:45:48.000000 awscli-plugin-granica-2.0.5/awscli-plugin-granica/bolt_cli_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-06-02 03:45:48.000000 awscli-plugin-granica-2.0.5/awscli-plugin-granica/bolt_router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:45:58.359919 awscli-plugin-granica-2.0.5/awscli_plugin_granica.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-02 03:45:58.000000 awscli-plugin-granica-2.0.5/awscli_plugin_granica.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-02 03:45:58.000000 awscli-plugin-granica-2.0.5/awscli_plugin_granica.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 03:45:58.000000 awscli-plugin-granica-2.0.5/awscli_plugin_granica.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-02 03:45:58.000000 awscli-plugin-granica-2.0.5/awscli_plugin_granica.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 03:45:58.000000 awscli-plugin-granica-2.0.5/awscli_plugin_granica.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-02 03:45:58.359919 awscli-plugin-granica-2.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-02 03:45:48.000000 awscli-plugin-granica-2.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:14:52.995455 awscli-plugin-granica-2.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-02 04:14:41.000000 awscli-plugin-granica-2.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-02 04:14:52.995455 awscli-plugin-granica-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-02 04:14:41.000000 awscli-plugin-granica-2.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:14:52.995455 awscli-plugin-granica-2.0.6/awscli-plugin-granica/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-02 04:14:41.000000 awscli-plugin-granica-2.0.6/awscli-plugin-granica/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-02 04:14:41.000000 awscli-plugin-granica-2.0.6/awscli-plugin-granica/bolt_cli_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-06-02 04:14:41.000000 awscli-plugin-granica-2.0.6/awscli-plugin-granica/bolt_router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:14:52.995455 awscli-plugin-granica-2.0.6/awscli_plugin_granica.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-02 04:14:52.000000 awscli-plugin-granica-2.0.6/awscli_plugin_granica.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-02 04:14:52.000000 awscli-plugin-granica-2.0.6/awscli_plugin_granica.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 04:14:52.000000 awscli-plugin-granica-2.0.6/awscli_plugin_granica.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-02 04:14:52.000000 awscli-plugin-granica-2.0.6/awscli_plugin_granica.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 04:14:52.000000 awscli-plugin-granica-2.0.6/awscli_plugin_granica.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-02 04:14:52.995455 awscli-plugin-granica-2.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-02 04:14:41.000000 awscli-plugin-granica-2.0.6/setup.py
```

### Comparing `awscli-plugin-granica-2.0.5/LICENSE` & `awscli-plugin-granica-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `awscli-plugin-granica-2.0.5/PKG-INFO` & `awscli-plugin-granica-2.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awscli-plugin-granica
-Version: 2.0.5
+Version: 2.0.6
 Summary: Granica plugin for AWS CLI
 Home-page: https://gitlab.com/projectn-oss/projectn-bolt-awscli
 Author: Project N
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3
@@ -30,22 +30,21 @@
 ## Configuration
 
 To configure the plugin after it has been installed, use `aws configure`:
 
 ```bash
 aws configure set plugins.granica awscli-plugin-granica
 aws [--profile PROFILE] configure set granica_custom_domain <Granica custom domain>
-aws [--profile PROFILE] configure set granica_az <preferred availability zone ID>
+aws [--profile PROFILE] configure set region <Region>
 ```
-`granica_custom_domain`
 
 For example, to activate a Granica service using an internal load balancer hosted at `https://quicksilver.us-east-1.mydomain.mycompany.com` for the `staging` AWS profile, run:
 ```bash
 aws --profile staging configure set granica_custom_domain mydomain.mycompany.com
-aws --profile staging configure set granica_az use1-az1
+aws --profile staging configure set region us-east-1
 ```
 
 ## AWS CLI v2
 
 This plugin has been tested for compatibility with [AWS CLI version 2](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html), but please take note of the [[plugins] configuration breaking changes](https://docs.aws.amazon.com/cli/latest/userguide/cliv2-migration.html#cliv2-migration-profile-plugins). In particular, you will need to add a block like:
 
 ```
```

### Comparing `awscli-plugin-granica-2.0.5/README.md` & `awscli-plugin-granica-2.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -17,22 +17,21 @@
 ## Configuration
 
 To configure the plugin after it has been installed, use `aws configure`:
 
 ```bash
 aws configure set plugins.granica awscli-plugin-granica
 aws [--profile PROFILE] configure set granica_custom_domain <Granica custom domain>
-aws [--profile PROFILE] configure set granica_az <preferred availability zone ID>
+aws [--profile PROFILE] configure set region <Region>
 ```
-`granica_custom_domain`
 
 For example, to activate a Granica service using an internal load balancer hosted at `https://quicksilver.us-east-1.mydomain.mycompany.com` for the `staging` AWS profile, run:
 ```bash
 aws --profile staging configure set granica_custom_domain mydomain.mycompany.com
-aws --profile staging configure set granica_az use1-az1
+aws --profile staging configure set region us-east-1
 ```
 
 ## AWS CLI v2
 
 This plugin has been tested for compatibility with [AWS CLI version 2](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html), but please take note of the [[plugins] configuration breaking changes](https://docs.aws.amazon.com/cli/latest/userguide/cliv2-migration.html#cliv2-migration-profile-plugins). In particular, you will need to add a block like:
 
 ```
```

### Comparing `awscli-plugin-granica-2.0.5/awscli-plugin-granica/__init__.py` & `awscli-plugin-granica-2.0.6/awscli-plugin-granica/__init__.py`

 * *Files identical despite different names*

### Comparing `awscli-plugin-granica-2.0.5/awscli-plugin-granica/bolt_cli_hooks.py` & `awscli-plugin-granica-2.0.6/awscli-plugin-granica/bolt_cli_hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,16 @@
     session = kwargs['session']
 
     if parsed_args.profile:
         session.set_config_variable('profile', parsed_args.profile)
     profile = session.get_scoped_config()
     
     region = None
-    if 'bolt_region' in profile:
-        region = profile['bolt_region']
+    if 'granica_region' in profile:
+        region = profile['granica_region']
     elif 'region' in profile:
         region = profile['region']
     else:
         try:
             region = get_region()
         except Exception as e:
             pass
```

### Comparing `awscli-plugin-granica-2.0.5/awscli-plugin-granica/bolt_router.py` & `awscli-plugin-granica-2.0.6/awscli-plugin-granica/bolt_router.py`

 * *Files identical despite different names*

### Comparing `awscli-plugin-granica-2.0.5/awscli_plugin_granica.egg-info/PKG-INFO` & `awscli-plugin-granica-2.0.6/awscli_plugin_granica.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awscli-plugin-granica
-Version: 2.0.5
+Version: 2.0.6
 Summary: Granica plugin for AWS CLI
 Home-page: https://gitlab.com/projectn-oss/projectn-bolt-awscli
 Author: Project N
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3
@@ -30,22 +30,21 @@
 ## Configuration
 
 To configure the plugin after it has been installed, use `aws configure`:
 
 ```bash
 aws configure set plugins.granica awscli-plugin-granica
 aws [--profile PROFILE] configure set granica_custom_domain <Granica custom domain>
-aws [--profile PROFILE] configure set granica_az <preferred availability zone ID>
+aws [--profile PROFILE] configure set region <Region>
 ```
-`granica_custom_domain`
 
 For example, to activate a Granica service using an internal load balancer hosted at `https://quicksilver.us-east-1.mydomain.mycompany.com` for the `staging` AWS profile, run:
 ```bash
 aws --profile staging configure set granica_custom_domain mydomain.mycompany.com
-aws --profile staging configure set granica_az use1-az1
+aws --profile staging configure set region us-east-1
 ```
 
 ## AWS CLI v2
 
 This plugin has been tested for compatibility with [AWS CLI version 2](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html), but please take note of the [[plugins] configuration breaking changes](https://docs.aws.amazon.com/cli/latest/userguide/cliv2-migration.html#cliv2-migration-profile-plugins). In particular, you will need to add a block like:
 
 ```
```

### Comparing `awscli-plugin-granica-2.0.5/setup.py` & `awscli-plugin-granica-2.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 requires = ['awscli>=1.12.13', 'botocore>=1.12.13']
 python_requires = '>=3'
 
 setup(
     name='awscli-plugin-granica',
     packages=['awscli-plugin-granica'],
-    version='2.0.5',
+    version='2.0.6',
     description='Granica plugin for AWS CLI',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Project N',
     install_requires=requires,
     python_requires=python_requires,
     classifiers=[
```

