# Comparing `tmp/generalpackager-0.5.7.tar.gz` & `tmp/generalpackager-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generalpackager-0.5.7.tar", last modified: Thu Feb  2 12:29:40 2023, max compression
+gzip compressed data, was "generalpackager-0.5.8.tar", last modified: Fri Jun  2 21:27:54 2023, max compression
```

## Comparing `generalpackager-0.5.7.tar` & `generalpackager-0.5.8.tar`

### file list

```diff
@@ -1,99 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 12:29:40.910038 generalpackager-0.5.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-02-02 12:29:26.000000 generalpackager-0.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-02 12:29:26.000000 generalpackager-0.5.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    39239 2023-02-02 12:29:40.910038 generalpackager-0.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    38390 2023-02-02 12:29:31.000000 generalpackager-0.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 12:29:40.906037 generalpackager-0.5.7/generalpackager/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 12:29:40.906037 generalpackager-0.5.7/generalpackager/api/
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/localmodule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 12:29:40.902037 generalpackager-0.5.7/generalpackager/api/localrepo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 12:29:40.906037 generalpackager-0.5.7/generalpackager/api/localrepo/base/
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/localrepo/base/localrepo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/localrepo/base/localrepo_git.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/localrepo/base/localrepo_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/localrepo/base/localrepo_target.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/localrepo/base/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/localrepo/base/targets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 12:29:40.906037 generalpackager-0.5.7/generalpackager/api/localrepo/node/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/localrepo/node/localrepo_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/localrepo/node/metadata_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 12:29:40.906037 generalpackager-0.5.7/generalpackager/api/localrepo/python/
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/localrepo/python/localrepo_python.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/localrepo/python/metadata_python.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/npm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/pypi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 12:29:40.906037 generalpackager-0.5.7/generalpackager/api/shared/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/shared/decos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 12:29:40.906037 generalpackager-0.5.7/generalpackager/api/shared/files/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 12:29:40.910038 generalpackager-0.5.7/generalpackager/api/shared/files/definitions/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/shared/files/definitions/commit_editmsg.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/shared/files/definitions/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/shared/files/definitions/exeproduct.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/shared/files/definitions/exetarget.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/shared/files/definitions/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/shared/files/definitions/git_exclude.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/shared/files/definitions/index_js.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/shared/files/definitions/init.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/shared/files/definitions/license.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/shared/files/definitions/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/shared/files/definitions/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/shared/files/definitions/npm_ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/shared/files/definitions/org_readme.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/shared/files/definitions/package_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/shared/files/definitions/pre_commit_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/shared/files/definitions/pre_push_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/shared/files/definitions/randomtesting.py
--rw-r--r--   0 runner    (1001) docker     (123)    12242 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/shared/files/definitions/readme.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/shared/files/definitions/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/shared/files/definitions/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/shared/files/definitions/test_js.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/shared/files/definitions/test_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/shared/files/definitions/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/shared/files/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/shared/files/file_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/shared/files/shared_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/shared/name.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/shared/owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/shared/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/api/venv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 12:29:40.910038 generalpackager-0.5.7/generalpackager/other/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/other/envvars.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/other/licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/other/packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/packager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/packager_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/packager_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/packager_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/packager_github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/packager_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/packager_pypi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/packager_relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/packager_workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 12:29:40.910038 generalpackager-0.5.7/generalpackager/test/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/test/test_generalpackager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/test/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/test/test_local_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/test/test_local_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/test/test_local_repo_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/test/test_packager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/test/test_packager_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/test/test_packager_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/test/test_packager_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/test/test_packager_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/test/test_packager_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/test/test_packager_pypi.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/test/test_packager_relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/test/test_pypi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/test/test_shared.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-02-02 12:27:24.000000 generalpackager-0.5.7/generalpackager/test/test_venv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 12:29:40.906037 generalpackager-0.5.7/generalpackager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    39239 2023-02-02 12:29:40.000000 generalpackager-0.5.7/generalpackager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-02-02 12:29:40.000000 generalpackager-0.5.7/generalpackager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 12:29:40.000000 generalpackager-0.5.7/generalpackager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-02 12:29:40.000000 generalpackager-0.5.7/generalpackager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-02 12:29:40.000000 generalpackager-0.5.7/generalpackager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-02-02 12:29:26.000000 generalpackager-0.5.7/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-02 12:29:40.910038 generalpackager-0.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-02-02 12:29:31.000000 generalpackager-0.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:54.916512 generalpackager-0.5.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-02 21:27:18.000000 generalpackager-0.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-02 21:27:18.000000 generalpackager-0.5.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    50789 2023-06-02 21:27:54.912512 generalpackager-0.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    49940 2023-06-02 21:27:26.000000 generalpackager-0.5.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:54.904512 generalpackager-0.5.8/generalpackager/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:54.908512 generalpackager-0.5.8/generalpackager/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/localmodule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:54.904512 generalpackager-0.5.8/generalpackager/api/localrepo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:54.908512 generalpackager-0.5.8/generalpackager/api/localrepo/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/localrepo/base/localrepo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/localrepo/base/localrepo_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/localrepo/base/localrepo_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/localrepo/base/localrepo_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/localrepo/base/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:54.908512 generalpackager-0.5.8/generalpackager/api/localrepo/node/
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/localrepo/node/localrepo_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/localrepo/node/metadata_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:54.908512 generalpackager-0.5.8/generalpackager/api/localrepo/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/localrepo/python/localrepo_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/localrepo/python/metadata_python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:54.908512 generalpackager-0.5.8/generalpackager/api/localrepo/top/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/localrepo/top/target_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:54.908512 generalpackager-0.5.8/generalpackager/api/package_hosts/
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/package_hosts/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/package_hosts/npm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/package_hosts/pypi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:54.908512 generalpackager-0.5.8/generalpackager/api/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/decos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:54.908512 generalpackager-0.5.8/generalpackager/api/shared/files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:54.912512 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/commit_editmsg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/exeproduct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/exetarget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/git_exclude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/gitignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/index_js.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/license.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/npm_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/org_readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/package_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/pre_commit_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/pre_push_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12255 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/test_js.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/test_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9509 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/workflow_dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/file_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/shared_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/venv_cruds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:54.912512 generalpackager-0.5.8/generalpackager/other/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/other/envvars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12684 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/other/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/packager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/packager_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/packager_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/packager_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/packager_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/packager_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/packager_pypi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/packager_relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/packager_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:54.912512 generalpackager-0.5.8/generalpackager/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/test/test_generalpackager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/test/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/test/test_local_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/test/test_local_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/test/test_local_repo_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/test/test_local_repo_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/test/test_packager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/test/test_packager_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/test/test_packager_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/test/test_packager_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/test/test_packager_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/test/test_packager_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/test/test_packager_pypi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/test/test_packager_relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/test/test_pypi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/test/test_shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/test/test_venv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:54.908512 generalpackager-0.5.8/generalpackager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    50789 2023-06-02 21:27:54.000000 generalpackager-0.5.8/generalpackager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-06-02 21:27:54.000000 generalpackager-0.5.8/generalpackager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 21:27:54.000000 generalpackager-0.5.8/generalpackager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-02 21:27:54.000000 generalpackager-0.5.8/generalpackager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-02 21:27:54.000000 generalpackager-0.5.8/generalpackager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-02 21:27:18.000000 generalpackager-0.5.8/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 21:27:54.916512 generalpackager-0.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-02 21:27:26.000000 generalpackager-0.5.8/setup.py
```

### Comparing `generalpackager-0.5.7/PKG-INFO` & `generalpackager-0.5.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: generalpackager
-Version: 0.5.7
-Summary: Tools to interface GitHub, PyPI, NPM and local modules / repos. Used for generating files to keep projects dry and synced. Tailored for ManderaGeneral for now.
-Home-page: https://github.com/ManderaGeneral/generalpackager
-Author: Rickard "Mandera" Abraham
-Author-email: rickard.abraham@gmail.com
-License: mit
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <details open>
 <summary><h1>generalpackager</h1></summary>
 
 Tools to interface GitHub, PyPI, NPM and local modules / repos. Used for generating files to keep projects dry and synced. Tailored for ManderaGeneral for now.
 
 <details>
 <summary><h2>Table of Contents</h2></summary>
@@ -38,21 +19,21 @@
 
 
 <details open>
 <summary><h2>Dependency Diagram for ManderaGeneral</h2></summary>
 
 ```mermaid
 flowchart LR
+2([library]) --> 5([packager])
+2([library]) --> 4([vector])
 3([file]) --> 5([packager])
 0([import]) --> 3([file])
-2([library]) --> 3([file])
-2([library]) --> 4([vector])
-2([library]) --> 5([packager])
 1([tool]) --> 2([library])
 0([import]) --> 2([library])
+2([library]) --> 3([file])
 click 0 "https://github.com/ManderaGeneral/generalimport"
 click 1 "https://github.com/ManderaGeneral/generaltool"
 click 2 "https://github.com/ManderaGeneral/generallibrary"
 click 3 "https://github.com/ManderaGeneral/generalfile"
 click 4 "https://github.com/ManderaGeneral/generalvector"
 click 5 "https://github.com/ManderaGeneral/generalpackager"
 style 5 fill:#482
@@ -66,251 +47,319 @@
 | `pip install`                                                                      | `generalpackager`   |
 |:-----------------------------------------------------------------------------------|:--------------------|
 | <a href='https://pypi.org/project/generallibrary[table]'>generallibrary[table]</a> | ✔️                  |
 | <a href='https://pypi.org/project/generalfile'>generalfile</a>                     | ✔️                  |
 | <a href='https://pypi.org/project/requests'>requests</a>                           | ✔️                  |
 | <a href='https://pypi.org/project/pyinstaller'>pyinstaller</a>                     | ✔️                  |
 | <a href='https://pypi.org/project/coverage'>coverage</a>                           | ✔️                  |
+| <a href='https://pypi.org/project/setuptools'>setuptools</a>                       | ✔️                  |
+| <a href='https://pypi.org/project/wheel'>wheel</a>                                 | ✔️                  |
+| <a href='https://pypi.org/project/twine'>twine</a>                                 | ✔️                  |
 </details>
 
 
 <details open>
 <summary><h2>Information</h2></summary>
 
-| Package                                                              | Ver                                                | Latest Release       | Python                                                                                                                                                                                                                                                 | Platform        | Cover   |
-|:---------------------------------------------------------------------|:---------------------------------------------------|:---------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------------|:--------|
-| [generalpackager](https://github.com/ManderaGeneral/generalpackager) | [0.5.7](https://pypi.org/project/generalpackager/) | 2023-02-02 13:29 CET | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/downloads/release/python-3100/), [3.11](https://www.python.org/downloads/release/python-3110/) | Windows, Ubuntu | 68.9 %  |
+| Package                                                              | Ver                                                | Latest Release        | Python                                                                                                                                                                                                                                                 | Platform        | Cover   |
+|:---------------------------------------------------------------------|:---------------------------------------------------|:----------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------------|:--------|
+| [generalpackager](https://github.com/ManderaGeneral/generalpackager) | [0.5.8](https://pypi.org/project/generalpackager/) | 2023-06-02 23:27 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/downloads/release/python-3100/), [3.11](https://www.python.org/downloads/release/python-3110/) | Windows, Ubuntu | 67.8 %  |
 </details>
 
 
 
 <details>
 <summary><h2>Attributes</h2></summary>
 
 <pre>
 <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/__init__.py#L1'>Module: generalpackager</a>
-├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L11'>Class: GitHub</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L11'>Class: GitHub</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L8'>Class: LocalModule</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L16'>Class: LocalRepo</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L22'>Class: Packager</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L26'>Class: PyPI</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L27'>Method: api_url</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L43'>Method: download</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L39'>Method: exists</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L96'>Method: get_description</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L64'>Method: get_owners_packages</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L83'>Method: get_topics</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L71'>Method: get_website</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L32'>Property: git_clone_command</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L36'>Property: pip_install_command</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L108'>Method: request_kwargs</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L102'>Method: set_description</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L89'>Method: set_topics</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L77'>Method: set_website</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L24'>Property: ssh_url</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L20'>Property: url</a>
-├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L8'>Class: LocalModule</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L11'>Class: GitHub</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L8'>Class: LocalModule</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L16'>Class: LocalRepo</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L22'>Class: Packager</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L26'>Class: PyPI</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L26'>Method: exists</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L67'>Method: get_all_local_modules</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L89'>Method: get_dependants</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L74'>Method: get_dependencies</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L20'>Property: module</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L41'>Property: objInfo</a>
+├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L13'>Class: GitHub</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L13'>Class: GitHub</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L9'>Class: LocalModule</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L17'>Class: LocalRepo</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L17'>Class: Packager</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L27'>Class: PyPI</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L54'>Method: api_url</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L23'>Method: format_version</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L133'>Method: get_description</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L120'>Method: get_topics</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L108'>Method: get_website</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L58'>Method: git_clone_command</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L40'>Method: is_general</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L36'>Method: name_is_general</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L71'>Property: pip_install_command</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L145'>Method: request_kwargs</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L139'>Method: set_description</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L126'>Method: set_topics</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L114'>Method: set_website</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L45'>Property: simple_name</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L51'>Property: ssh_url</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L18'>Method: tag_is_version</a>
+├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L9'>Class: LocalModule</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L13'>Class: GitHub</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L9'>Class: LocalModule</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L17'>Class: LocalRepo</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L17'>Class: Packager</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L27'>Class: PyPI</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L27'>Method: exists</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L68'>Method: get_all_local_modules</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L90'>Method: get_dependants</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L75'>Method: get_dependencies</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L21'>Property: module</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L42'>Property: objInfo</a>
 │  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/#L426'>Property: path</a>
-├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L16'>Class: LocalRepo</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L11'>Class: GitHub</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L8'>Class: LocalModule</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L16'>Class: LocalRepo</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L22'>Class: Packager</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L26'>Class: PyPI</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/targets.py#L4'>Class: Targets</a>
+├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L17'>Class: LocalRepo</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L13'>Class: GitHub</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L9'>Class: LocalModule</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L17'>Class: LocalRepo</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L17'>Class: Packager</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L27'>Class: PyPI</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L8'>Class: Targets</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/decos.py#L4'>Method: changed_files</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/decos.py#L4'>Method: clone</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/decos.py#L4'>Method: commit</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_git.py#L12'>Method: commit_message</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/commit_editmsg.py#L5'>Class: commit_editmsg_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_git.py#L11'>Method: commit_message</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/decos.py#L4'>Method: commit_sha</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_git.py#L72'>Method: commit_sha_short</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L55'>Method: exists</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L114'>Method: format_file</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L92'>Method: get_examples_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L60'>Method: get_exeproduct_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L56'>Method: get_exetarget_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L52'>Method: get_generate_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_git.py#L76'>Method: commit_sha_short</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/examples.py#L5'>Class: examples_folder</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/exeproduct.py#L5'>Class: exeproduct_folder</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/exetarget.py#L5'>Class: exetarget_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L45'>Method: exists</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L104'>Method: format_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/generate.py#L6'>Class: generate_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_git.py#L88'>Method: get_all_versions</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L88'>Method: get_examples_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L56'>Method: get_exeproduct_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L52'>Method: get_exetarget_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L27'>Method: get_file_from_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L11'>Method: get_filenames</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L17'>Method: get_files</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L22'>Method: get_files_by_relative_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L48'>Method: get_generate_path</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L16'>Method: get_git_exclude_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L64'>Method: get_git_ignore_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L72'>Method: get_index_js_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L60'>Method: get_git_ignore_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L68'>Method: get_index_js_path</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L44'>Method: get_init_path</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L28'>Method: get_license_path</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L24'>Method: get_manifest_path</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L12'>Method: get_metadata_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L68'>Method: get_npm_ignore_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L64'>Method: get_npm_ignore_path</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L8'>Method: get_org_readme_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L80'>Method: get_package_json_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L72'>Method: get_package_paths_gen</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L84'>Method: get_pre_commit_hook_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L88'>Method: get_pre_push_hook_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L48'>Method: get_randomtesting_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L76'>Method: get_package_json_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L62'>Method: get_package_paths_gen</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L80'>Method: get_pre_commit_hook_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L84'>Method: get_pre_push_hook_path</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L4'>Method: get_readme_path</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L20'>Method: get_setup_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L76'>Method: get_test_js_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L72'>Method: get_test_js_path</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L36'>Method: get_test_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L66'>Method: get_test_paths</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L56'>Method: get_test_paths</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L40'>Method: get_test_template_path</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L32'>Method: get_workflow_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_git.py#L29'>Method: git_config</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_git.py#L21'>Method: git_missing_credentials</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_git.py#L25'>Method: git_nothing_to_commit</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_git.py#L28'>Method: git_config</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/git_exclude.py#L5'>Class: git_exclude_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_git.py#L20'>Method: git_missing_credentials</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_git.py#L24'>Method: git_nothing_to_commit</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/gitignore.py#L5'>Class: gitignore_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/index_js.py#L6'>Class: index_js_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/decos.py#L4'>Method: init</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_target.py#L18'>Method: is_django</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_target.py#L22'>Method: is_exe</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L41'>Method: is_general</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_target.py#L14'>Method: is_node</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_target.py#L10'>Method: is_python</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L33'>Property: metadata</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L48'>Method: metadata_exists</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L37'>Method: name_is_general</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/init.py#L6'>Class: init_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L28'>Method: is_django</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L32'>Method: is_exe</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L40'>Method: is_general</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L24'>Method: is_node</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L20'>Method: is_python</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/license.py#L6'>Class: license_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/manifest.py#L5'>Class: manifest_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L34'>Property: metadata</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L38'>Method: metadata_exists</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/metadata.py#L5'>Class: metadata_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L36'>Method: name_is_general</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/npm_ignore.py#L5'>Class: npm_ignore_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/org_readme.py#L6'>Class: org_readme_file</a>
+│  │  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/org_readme.py#L18'>Method: get_org_description_markdown</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/package_json.py#L6'>Class: package_json_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/pre_commit_hook.py#L4'>Class: pre_commit_hook_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/pre_push_hook.py#L6'>Class: pre_push_hook_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/decos.py#L4'>Method: push</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L60'>Method: repo_exists</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L46'>Property: simple_name</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L42'>Property: target</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_target.py#L49'>Method: targetted</a>
-├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/node/localrepo_node.py#L6'>Class: LocalRepo_Node</a>
-├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L11'>Class: LocalRepo_Python</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L16'>Method: get_python_exe_path</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L21'>Method: unittest</a>
-├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L22'>Class: Packager</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L11'>Class: GitHub</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L8'>Class: LocalModule</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L16'>Class: LocalRepo</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L22'>Class: Packager</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/other/packages.py#L9'>Class: Packages</a>
-│  │  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/other/packages.py#L34'>Method: all_packages</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L26'>Class: PyPI</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/targets.py#L4'>Class: Targets</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L20'>Method: commit_and_push</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L8'>Class: readme_file</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L125'>Method: get_attributes_markdown</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L17'>Method: get_badges_dict</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L246'>Method: get_contributions_markdown</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L27'>Method: get_description_markdown</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L89'>Method: get_examples_markdown</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L195'>Method: get_footnote_markdown</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L219'>Method: get_information_markdown</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L44'>Method: get_installation_markdown</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L209'>Method: get_mermaid_markdown</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L163'>Method: get_todos</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L169'>Method: get_todos_markdown</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L204'>Method: github_link</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L137'>Method: github_link_path_line</a>
+│  │  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L189'>Method: set_collapsible</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L50'>Method: repo_exists</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/setup.py#L6'>Class: setup_file</a>
+│  │  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/setup.py#L21'>Method: get_classifiers</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L45'>Property: simple_name</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_target.py#L18'>Method: targetted</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/test.py#L5'>Class: test_folder</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/test_js.py#L6'>Class: test_js_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/test_template.py#L6'>Class: test_template_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/workflow_dev.py#L4'>Class: workflow_dev_file</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/workflow.py#L7'>Class: workflow_file</a>
+│     └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/workflow.py#L15'>Method: codeline</a>
+├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/node/localrepo_node.py#L9'>Class: LocalRepo_Node</a>
+├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L12'>Class: LocalRepo_Python</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L17'>Method: get_python_exe_path</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L57'>Method: set_easy_install_value</a>
+├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L17'>Class: Packager</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L13'>Class: GitHub</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L9'>Class: LocalModule</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L17'>Class: LocalRepo</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L17'>Class: Packager</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L37'>Class: Packages</a>
+│  │  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L62'>Method: all_packages</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L27'>Class: PyPI</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L8'>Class: Targets</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L22'>Method: commit_and_push</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/commit_editmsg.py#L5'>Class: commit_editmsg_file</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L46'>Method: compare_local_to_github</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L53'>Method: compare_local_to_pypi</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L8'>Method: create_blank_locally_python</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L32'>Method: create_github_repo</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L36'>Method: create_master_branch</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L38'>Method: compare_local_to_github</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L45'>Method: compare_local_to_pypi</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L7'>Method: create_blank_locally</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L34'>Method: create_github_repo</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L38'>Method: create_master_branch</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/examples.py#L5'>Class: examples_folder</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/exeproduct.py#L5'>Class: exeproduct_folder</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/exetarget.py#L5'>Class: exetarget_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_relations.py#L77'>Method: general_bumped_set</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_relations.py#L85'>Method: general_changed_dict</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/generate.py#L6'>Class: generate_file</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L69'>Method: generate_localfiles</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_metadata.py#L27'>Method: get_classifiers</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L61'>Method: generate_localfiles</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_metadata.py#L29'>Method: get_classifiers</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_relations.py#L38'>Method: get_dependants</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_relations.py#L23'>Method: get_dependencies</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L29'>Method: get_file_from_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L13'>Method: get_filenames</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L19'>Method: get_files</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L24'>Method: get_files_by_relative_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L27'>Method: get_file_from_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L11'>Method: get_filenames</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L17'>Method: get_files</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L22'>Method: get_files_by_relative_path</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_pypi.py#L8'>Method: get_latest_release</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_relations.py#L49'>Method: get_ordered_packagers</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_relations.py#L71'>Method: get_owners_package_names</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_metadata.py#L4'>Method: get_topics</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_metadata.py#L6'>Method: get_topics</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/git_exclude.py#L5'>Class: git_exclude_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L81'>Property: github</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L47'>Method: github_available</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L64'>Method: if_publish_bump</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L71'>Method: if_publish_upload</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L49'>Method: github_available</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/gitignore.py#L5'>Class: gitignore_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L71'>Method: if_publish_bump</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L78'>Method: if_publish_upload</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/index_js.py#L6'>Class: index_js_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/init.py#L6'>Class: init_file</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_metadata.py#L33'>Method: is_bumped</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_target.py#L18'>Method: is_django</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_target.py#L22'>Method: is_exe</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L41'>Method: is_general</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_target.py#L14'>Method: is_node</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_target.py#L10'>Method: is_python</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_metadata.py#L35'>Method: is_bumped</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L28'>Method: is_django</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L32'>Method: is_exe</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L40'>Method: is_general</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L24'>Method: is_node</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L20'>Method: is_python</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/license.py#L6'>Class: license_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L88'>Property: localmodule</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L52'>Method: localmodule_available</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L71'>Property: localrepo</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L42'>Method: localrepo_available</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L54'>Method: localmodule_available</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L73'>Property: localrepo</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L44'>Method: localrepo_available</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/manifest.py#L5'>Class: manifest_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/metadata.py#L5'>Class: metadata_file</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L37'>Method: name_is_general</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L36'>Method: name_is_general</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_environment.py#L9'>Method: new_clean_environment</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/npm_ignore.py#L5'>Class: npm_ignore_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/org_readme.py#L6'>Class: org_readme_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/package_json.py#L6'>Class: package_json_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_relations.py#L11'>Method: packagers_from_packages</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/pre_commit_hook.py#L4'>Class: pre_commit_hook_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/pre_push_hook.py#L6'>Class: pre_push_hook_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L14'>Method: push</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L95'>Property: pypi</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L60'>Method: pypi_available</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/randomtesting.py#L6'>Class: randomtesting_file</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L9'>Class: readme_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L62'>Method: pypi_available</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L8'>Class: readme_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_pypi.py#L23'>Method: reserve_name</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L18'>Method: run_ordered_methods</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L22'>Method: run_ordered_methods</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/setup.py#L6'>Class: setup_file</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L46'>Property: simple_name</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L46'>Method: summary_packagers</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L45'>Property: simple_name</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L36'>Method: summary_packagers</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L6'>Method: sync_github_metadata</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_metadata.py#L47'>Property: target</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_metadata.py#L50'>Property: target</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/test.py#L5'>Class: test_folder</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/test_js.py#L6'>Class: test_js_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/test_template.py#L6'>Class: test_template_file</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L59'>Method: upload_package_summary</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/workflow.py#L6'>Class: workflow_file</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L8'>Method: workflow_sync</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L8'>Method: workflow_unittest</a>
-└─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L26'>Class: PyPI</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L11'>Class: GitHub</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L8'>Class: LocalModule</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L16'>Class: LocalRepo</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L22'>Class: Packager</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L26'>Class: PyPI</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L47'>Method: download</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L37'>Method: exists</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L70'>Method: get_date</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L59'>Method: get_owners_packages</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L41'>Method: get_tarball_url</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L63'>Method: get_version</a>
-   └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L34'>Property: url</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L66'>Method: upload_package_summary</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/workflow_dev.py#L4'>Class: workflow_dev_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/workflow.py#L7'>Class: workflow_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L18'>Method: workflow_packagers</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L7'>Method: workflow_sync</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L7'>Method: workflow_unittest</a>
+├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L27'>Class: PyPI</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L13'>Class: GitHub</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L9'>Class: LocalModule</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L17'>Class: LocalRepo</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L17'>Class: Packager</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L27'>Class: PyPI</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L40'>Method: is_general</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L36'>Property: json_endpoint</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L36'>Method: name_is_general</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L45'>Property: simple_name</a>
+└─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L9'>Class: Venv</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L69'>Method: active</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L72'>Method: create_venv</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv_cruds.py#L69'>Property: cruds</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L85'>Method: deactivate</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L171'>Method: debug</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L54'>Method: easy_install_path</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L48'>Method: exe_name</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L66'>Method: exists</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L30'>Method: get_active_python</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L18'>Method: get_active_venv</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L24'>Method: get_active_venv_path</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L131'>Method: list_python_versions</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L120'>Method: list_venv_paths</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L52'>Method: python_exe_path</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L56'>Method: python_home_exe_path</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L55'>Method: python_home_path</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L60'>Method: python_path</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L58'>Method: python_sys_executable_path</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L117'>Method: python_version</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L50'>Method: pyvenv_cfg_path</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L51'>Method: scripts_path</a>
+   └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L53'>Method: site_packages_path</a>
 </pre>
 </details>
 
 
 <details open>
 <summary><h2>Contributions</h2></summary>
 
-Issue-creation and discussions are most welcome!
-
-Pull requests are currently not wanted, please discuss with me before investing any time
+Issue-creation, discussions and pull requests are most welcome!
 </details>
 
 
 <details>
 <summary><h2>Todo</h2></summary>
 
 | Module                                                                                                                                                      | Message                                                                                                                                                                                                          |
 |:------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L1'>packager_files.py</a>                          | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L10'>Fix create_blank, it overwrites current projects pip install.</a>                                  |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L1'>localrepo_python.py</a> | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L55'>Make sure twine is installed when trying to upload to pypi.</a>             |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L1'>localrepo_python.py</a> | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L56'>Look into private PyPI server where we could also do dry runs for test.</a> |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/metadata_python.py#L1'>metadata_python.py</a>   | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/metadata_python.py#L4'>Dynamic values in DataClass to remove LocalRepos and Metadatas.</a>           |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L1'>localrepo.py</a>                 | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L21'>Search for imports to list dependencies.</a>                                         |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L1'>pypi.py</a>                                          | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L12'>Move download to it's own package.</a>                                                                   |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L1'>pypi.py</a>                                          | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L66'>Find a faster fetch for latest PyPI version and datetime.</a>                                            |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L1'>readme.py</a>             | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L167'>Sort todos by name to decrease automatic commit changes.</a>                 |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L1'>github.py</a>                                      | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L13'>Get and Set GitHub repo private.</a>                                                                   |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/other/packages.py#L1'>packages.py</a>                                | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/other/packages.py#L11'>Generate Python file in generalpackager containing general packages.</a>                           |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L1'>packager_github.py</a>                        | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L43'>Setup env vars for project.</a>                                                                   |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L1'>packager_files.py</a>                          | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L9'>Fix create_blank, it overwrites current projects pip install.</a>                                   |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L1'>packager_github.py</a>                        | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L44'>Setup env vars for project.</a>                                                                   |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L1'>target.py</a>                               | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L39'>Generate Python file in generalpackager containing general packages.</a>                        |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L1'>readme.py</a>             | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L166'>Sort todos by name to decrease automatic commit changes.</a>                 |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L1'>pypi.py</a>                            | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L13'>Move download to it's own package.</a>                                                     |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L1'>pypi.py</a>                            | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L78'>Find a faster fetch for latest PyPI version and datetime.</a>                              |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L1'>github.py</a>                        | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L15'>Get and Set GitHub repo private.</a>                                                     |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L1'>localrepo_python.py</a> | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L77'>Make sure twine is installed when trying to upload to pypi.</a>             |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L1'>localrepo_python.py</a> | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L78'>Look into private PyPI server where we could also do dry runs for test.</a> |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L1'>localrepo.py</a>                 | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L22'>Search for imports to list dependencies.</a>                                         |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L1'>packager_api.py</a>                              | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L43'>Check that every API has create an *_available method</a>                                            |
 </details>
 
 
 <sup>
-Generated 2023-02-02 13:29 CET for commit <a href='https://github.com/ManderaGeneral/generalpackager/commit/master'>master</a>.
+Generated 2023-06-02 23:27 CEST for commit <a href='https://github.com/ManderaGeneral/generalpackager/commit/master'>master</a>.
 </sup>
 </details>
```

#### html2text {}

```diff
@@ -1,82 +1,72 @@
-Metadata-Version: 2.1 Name: generalpackager Version: 0.5.7 Summary: Tools to
-interface GitHub, PyPI, NPM and local modules / repos. Used for generating
-files to keep projects dry and synced. Tailored for ManderaGeneral for now.
-Home-page: https://github.com/ManderaGeneral/generalpackager Author: Rickard
-"Mandera" Abraham Author-email: rickard.abraham@gmail.com License: mit
-Classifier: Topic :: Software Development :: Build Tools Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: License :: OSI Approved ::
-MIT License Classifier: Operating System :: Microsoft :: Windows Classifier:
-Operating System :: POSIX :: Linux Description-Content-Type: text/markdown
-License-File: LICENSE
 ****** generalpackager ******
 Tools to interface GitHub, PyPI, NPM and local modules / repos. Used for
 generating files to keep projects dry and synced. Tailored for ManderaGeneral
 for now.
 ***** Table of Contents *****
 generalpackager
 ââ Dependency_Diagram_for_ManderaGeneral
 ââ Installation_showing_dependencies
 ââ Information
 ââ Attributes
 ââ Contributions
 ââ Todo
 
 ***** Dependency Diagram for ManderaGeneral *****
-```mermaid flowchart LR 3([file]) --> 5([packager]) 0([import]) --> 3([file]) 2
-([library]) --> 3([file]) 2([library]) --> 4([vector]) 2([library]) --> 5(
-[packager]) 1([tool]) --> 2([library]) 0([import]) --> 2([library]) click 0
+```mermaid flowchart LR 2([library]) --> 5([packager]) 2([library]) --> 4(
+[vector]) 3([file]) --> 5([packager]) 0([import]) --> 3([file]) 1([tool]) --> 2
+([library]) 0([import]) --> 2([library]) 2([library]) --> 3([file]) click 0
 "https://github.com/ManderaGeneral/generalimport" click 1 "https://github.com/
 ManderaGeneral/generaltool" click 2 "https://github.com/ManderaGeneral/
 generallibrary" click 3 "https://github.com/ManderaGeneral/generalfile" click 4
 "https://github.com/ManderaGeneral/generalvector" click 5 "https://github.com/
 ManderaGeneral/generalpackager" style 5 fill:#482 ```
 ***** Installation showing dependencies *****
 | `pip install` | `generalpackager` | |:---------------------------------------
 --------------------------------------------|:--------------------| |
 generallibrary[table] | âï¸ | | generalfile | âï¸ | | requests | âï¸ |
-| pyinstaller | âï¸ | | coverage | âï¸ |
+| pyinstaller | âï¸ | | coverage | âï¸ | | setuptools | âï¸ | | wheel
+| âï¸ | | twine | âï¸ |
 ***** Information *****
 | Package | Ver | Latest Release | Python | Platform | Cover | |:--------------
 -------------------------------------------------------|:----------------------
------------------------------|:---------------------|:-------------------------
+-----------------------------|:----------------------|:------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
-----------------------------------------------------------------|:-------------
----|:--------| | [generalpackager](https://github.com/ManderaGeneral/
-generalpackager) | [0.5.7](https://pypi.org/project/generalpackager/) | 2023-
-02-02 13:29 CET | [3.8](https://www.python.org/downloads/release/python-380/),
+-----------------------------------------------------------------|:------------
+----|:--------| | [generalpackager](https://github.com/ManderaGeneral/
+generalpackager) | [0.5.8](https://pypi.org/project/generalpackager/) | 2023-
+06-02 23:27 CEST | [3.8](https://www.python.org/downloads/release/python-380/),
 [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://
 www.python.org/downloads/release/python-3100/), [3.11](https://www.python.org/
-downloads/release/python-3110/) | Windows, Ubuntu | 68.9 % |
+downloads/release/python-3110/) | Windows, Ubuntu | 67.8 % |
 ***** Attributes *****
 Module:_generalpackager
 ââ Class:_GitHub
 â  ââ Class:_GitHub
 â  ââ Class:_LocalModule
 â  ââ Class:_LocalRepo
 â  ââ Class:_Packager
 â  ââ Class:_PyPI
 â  ââ Method:_api_url
-â  ââ Method:_download
-â  ââ Method:_exists
+â  ââ Method:_format_version
 â  ââ Method:_get_description
-â  ââ Method:_get_owners_packages
 â  ââ Method:_get_topics
 â  ââ Method:_get_website
-â  ââ Property:_git_clone_command
+â  ââ Method:_git_clone_command
+â  ââ Method:_is_general
+â  ââ Method:_name_is_general
 â  ââ Property:_pip_install_command
 â  ââ Method:_request_kwargs
 â  ââ Method:_set_description
 â  ââ Method:_set_topics
 â  ââ Method:_set_website
+â  ââ Property:_simple_name
 â  ââ Property:_ssh_url
-â  ââ Property:_url
+â  ââ Method:_tag_is_version
 ââ Class:_LocalModule
 â  ââ Class:_GitHub
 â  ââ Class:_LocalModule
 â  ââ Class:_LocalRepo
 â  ââ Class:_Packager
 â  ââ Class:_PyPI
 â  ââ Method:_exists
@@ -92,79 +82,123 @@
 â  ââ Class:_LocalRepo
 â  ââ Class:_Packager
 â  ââ Class:_PyPI
 â  ââ Class:_Targets
 â  ââ Method:_changed_files
 â  ââ Method:_clone
 â  ââ Method:_commit
+â  ââ Class:_commit_editmsg_file
 â  ââ Method:_commit_message
 â  ââ Method:_commit_sha
 â  ââ Method:_commit_sha_short
+â  ââ Class:_examples_folder
+â  ââ Class:_exeproduct_folder
+â  ââ Class:_exetarget_file
 â  ââ Method:_exists
 â  ââ Method:_format_file
+â  ââ Class:_generate_file
+â  ââ Method:_get_all_versions
 â  ââ Method:_get_examples_path
 â  ââ Method:_get_exeproduct_path
 â  ââ Method:_get_exetarget_path
+â  ââ Method:_get_file_from_path
+â  ââ Method:_get_filenames
+â  ââ Method:_get_files
+â  ââ Method:_get_files_by_relative_path
 â  ââ Method:_get_generate_path
 â  ââ Method:_get_git_exclude_path
 â  ââ Method:_get_git_ignore_path
 â  ââ Method:_get_index_js_path
 â  ââ Method:_get_init_path
 â  ââ Method:_get_license_path
 â  ââ Method:_get_manifest_path
 â  ââ Method:_get_metadata_path
 â  ââ Method:_get_npm_ignore_path
 â  ââ Method:_get_org_readme_path
 â  ââ Method:_get_package_json_path
 â  ââ Method:_get_package_paths_gen
 â  ââ Method:_get_pre_commit_hook_path
 â  ââ Method:_get_pre_push_hook_path
-â  ââ Method:_get_randomtesting_path
 â  ââ Method:_get_readme_path
 â  ââ Method:_get_setup_path
 â  ââ Method:_get_test_js_path
 â  ââ Method:_get_test_path
 â  ââ Method:_get_test_paths
 â  ââ Method:_get_test_template_path
 â  ââ Method:_get_workflow_path
 â  ââ Method:_git_config
+â  ââ Class:_git_exclude_file
 â  ââ Method:_git_missing_credentials
 â  ââ Method:_git_nothing_to_commit
+â  ââ Class:_gitignore_file
+â  ââ Class:_index_js_file
 â  ââ Method:_init
+â  ââ Class:_init_file
 â  ââ Method:_is_django
 â  ââ Method:_is_exe
 â  ââ Method:_is_general
 â  ââ Method:_is_node
 â  ââ Method:_is_python
+â  ââ Class:_license_file
+â  ââ Class:_manifest_file
 â  ââ Property:_metadata
 â  ââ Method:_metadata_exists
+â  ââ Class:_metadata_file
 â  ââ Method:_name_is_general
+â  ââ Class:_npm_ignore_file
+â  ââ Class:_org_readme_file
+â  â  ââ Method:_get_org_description_markdown
+â  ââ Class:_package_json_file
+â  ââ Class:_pre_commit_hook_file
+â  ââ Class:_pre_push_hook_file
 â  ââ Method:_push
+â  ââ Class:_readme_file
+â  â  ââ Method:_get_attributes_markdown
+â  â  ââ Method:_get_badges_dict
+â  â  ââ Method:_get_contributions_markdown
+â  â  ââ Method:_get_description_markdown
+â  â  ââ Method:_get_examples_markdown
+â  â  ââ Method:_get_footnote_markdown
+â  â  ââ Method:_get_information_markdown
+â  â  ââ Method:_get_installation_markdown
+â  â  ââ Method:_get_mermaid_markdown
+â  â  ââ Method:_get_todos
+â  â  ââ Method:_get_todos_markdown
+â  â  ââ Method:_github_link
+â  â  ââ Method:_github_link_path_line
+â  â  ââ Method:_set_collapsible
 â  ââ Method:_repo_exists
+â  ââ Class:_setup_file
+â  â  ââ Method:_get_classifiers
 â  ââ Property:_simple_name
-â  ââ Property:_target
-â  ââ Method:_targetted
+â  ââ Method:_targetted
+â  ââ Class:_test_folder
+â  ââ Class:_test_js_file
+â  ââ Class:_test_template_file
+â  ââ Class:_workflow_dev_file
+â  ââ Class:_workflow_file
+â     ââ Method:_codeline
 ââ Class:_LocalRepo_Node
 ââ Class:_LocalRepo_Python
 â  ââ Method:_get_python_exe_path
-â  ââ Method:_unittest
+â  ââ Method:_set_easy_install_value
 ââ Class:_Packager
 â  ââ Class:_GitHub
 â  ââ Class:_LocalModule
 â  ââ Class:_LocalRepo
 â  ââ Class:_Packager
 â  ââ Class:_Packages
 â  â  ââ Method:_all_packages
 â  ââ Class:_PyPI
 â  ââ Class:_Targets
 â  ââ Method:_commit_and_push
 â  ââ Class:_commit_editmsg_file
 â  ââ Method:_compare_local_to_github
 â  ââ Method:_compare_local_to_pypi
-â  ââ Method:_create_blank_locally_python
+â  ââ Method:_create_blank_locally
 â  ââ Method:_create_github_repo
 â  ââ Method:_create_master_branch
 â  ââ Class:_examples_folder
 â  ââ Class:_exeproduct_folder
 â  ââ Class:_exetarget_file
 â  ââ Method:_general_bumped_set
 â  ââ Method:_general_changed_dict
@@ -180,14 +214,15 @@
 â  ââ Method:_get_latest_release
 â  ââ Method:_get_ordered_packagers
 â  ââ Method:_get_owners_package_names
 â  ââ Method:_get_topics
 â  ââ Class:_git_exclude_file
 â  ââ Property:_github
 â  ââ Method:_github_available
+â  ââ Class:_gitignore_file
 â  ââ Method:_if_publish_bump
 â  ââ Method:_if_publish_upload
 â  ââ Class:_index_js_file
 â  ââ Class:_init_file
 â  ââ Method:_is_bumped
 â  ââ Method:_is_django
 â  ââ Method:_is_exe
@@ -208,58 +243,77 @@
 â  ââ Class:_package_json_file
 â  ââ Method:_packagers_from_packages
 â  ââ Class:_pre_commit_hook_file
 â  ââ Class:_pre_push_hook_file
 â  ââ Method:_push
 â  ââ Property:_pypi
 â  ââ Method:_pypi_available
-â  ââ Class:_randomtesting_file
 â  ââ Class:_readme_file
 â  ââ Method:_reserve_name
 â  ââ Method:_run_ordered_methods
 â  ââ Class:_setup_file
 â  ââ Property:_simple_name
 â  ââ Method:_summary_packagers
 â  ââ Method:_sync_github_metadata
 â  ââ Property:_target
 â  ââ Class:_test_folder
 â  ââ Class:_test_js_file
 â  ââ Class:_test_template_file
 â  ââ Method:_upload_package_summary
+â  ââ Class:_workflow_dev_file
 â  ââ Class:_workflow_file
+â  ââ Method:_workflow_packagers
 â  ââ Method:_workflow_sync
 â  ââ Method:_workflow_unittest
-ââ Class:_PyPI
-   ââ Class:_GitHub
-   ââ Class:_LocalModule
-   ââ Class:_LocalRepo
-   ââ Class:_Packager
-   ââ Class:_PyPI
-   ââ Method:_download
+ââ Class:_PyPI
+â  ââ Class:_GitHub
+â  ââ Class:_LocalModule
+â  ââ Class:_LocalRepo
+â  ââ Class:_Packager
+â  ââ Class:_PyPI
+â  ââ Method:_is_general
+â  ââ Property:_json_endpoint
+â  ââ Method:_name_is_general
+â  ââ Property:_simple_name
+ââ Class:_Venv
+   ââ Method:_active
+   ââ Method:_create_venv
+   ââ Property:_cruds
+   ââ Method:_deactivate
+   ââ Method:_debug
+   ââ Method:_easy_install_path
+   ââ Method:_exe_name
    ââ Method:_exists
-   ââ Method:_get_date
-   ââ Method:_get_owners_packages
-   ââ Method:_get_tarball_url
-   ââ Method:_get_version
-   ââ Property:_url
+   ââ Method:_get_active_python
+   ââ Method:_get_active_venv
+   ââ Method:_get_active_venv_path
+   ââ Method:_list_python_versions
+   ââ Method:_list_venv_paths
+   ââ Method:_python_exe_path
+   ââ Method:_python_home_exe_path
+   ââ Method:_python_home_path
+   ââ Method:_python_path
+   ââ Method:_python_sys_executable_path
+   ââ Method:_python_version
+   ââ Method:_pyvenv_cfg_path
+   ââ Method:_scripts_path
+   ââ Method:_site_packages_path
 
 ***** Contributions *****
-Issue-creation and discussions are most welcome! Pull requests are currently
-not wanted, please discuss with me before investing any time
+Issue-creation, discussions and pull requests are most welcome!
 ***** Todo *****
 | Module | Message | |:--------------------------------------------------------
 -------------------------------------------------------------------------------
 ---------------------|:--------------------------------------------------------
 -------------------------------------------------------------------------------
 --------------------------------------------------------------------------| |
 packager_files.py | Fix_create_blank,_it_overwrites_current_projects_pip
-install. | | localrepo_python.py | Make_sure_twine_is_installed_when_trying_to
-upload_to_pypi. | | localrepo_python.py | Look_into_private_PyPI_server_where
-we_could_also_do_dry_runs_for_test. | | metadata_python.py | Dynamic_values_in
-DataClass_to_remove_LocalRepos_and_Metadatas. | | localrepo.py | Search_for
-imports_to_list_dependencies. | | pypi.py | Move_download_to_it's_own_package.
-| | pypi.py | Find_a_faster_fetch_for_latest_PyPI_version_and_datetime. | |
+install. | | packager_github.py | Setup_env_vars_for_project. | | target.py |
+Generate_Python_file_in_generalpackager_containing_general_packages. | |
 readme.py | Sort_todos_by_name_to_decrease_automatic_commit_changes. | |
-github.py | Get_and_Set_GitHub_repo_private. | | packages.py | Generate_Python
-file_in_generalpackager_containing_general_packages. | | packager_github.py |
-Setup_env_vars_for_project. |  Generated 2023-02-02 13:29 CET for commit
-master.
+pypi.py | Move_download_to_it's_own_package. | | pypi.py | Find_a_faster_fetch
+for_latest_PyPI_version_and_datetime. | | github.py | Get_and_Set_GitHub_repo
+private. | | localrepo_python.py | Make_sure_twine_is_installed_when_trying_to
+upload_to_pypi. | | localrepo_python.py | Look_into_private_PyPI_server_where
+we_could_also_do_dry_runs_for_test. | | localrepo.py | Search_for_imports_to
+list_dependencies. | | packager_api.py | Check_that_every_API_has_create_an
+*_available_method |  Generated 2023-06-02 23:27 CEST for commit master.
```

### Comparing `generalpackager-0.5.7/README.md` & `generalpackager-0.5.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: generalpackager
+Version: 0.5.8
+Summary: Tools to interface GitHub, PyPI, NPM and local modules / repos. Used for generating files to keep projects dry and synced. Tailored for ManderaGeneral for now.
+Home-page: https://github.com/ManderaGeneral/generalpackager
+Author: Rickard "Mandera" Abraham
+Author-email: rickard.abraham@gmail.com
+License: mit
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <details open>
 <summary><h1>generalpackager</h1></summary>
 
 Tools to interface GitHub, PyPI, NPM and local modules / repos. Used for generating files to keep projects dry and synced. Tailored for ManderaGeneral for now.
 
 <details>
 <summary><h2>Table of Contents</h2></summary>
@@ -19,21 +38,21 @@
 
 
 <details open>
 <summary><h2>Dependency Diagram for ManderaGeneral</h2></summary>
 
 ```mermaid
 flowchart LR
+2([library]) --> 5([packager])
+2([library]) --> 4([vector])
 3([file]) --> 5([packager])
 0([import]) --> 3([file])
-2([library]) --> 3([file])
-2([library]) --> 4([vector])
-2([library]) --> 5([packager])
 1([tool]) --> 2([library])
 0([import]) --> 2([library])
+2([library]) --> 3([file])
 click 0 "https://github.com/ManderaGeneral/generalimport"
 click 1 "https://github.com/ManderaGeneral/generaltool"
 click 2 "https://github.com/ManderaGeneral/generallibrary"
 click 3 "https://github.com/ManderaGeneral/generalfile"
 click 4 "https://github.com/ManderaGeneral/generalvector"
 click 5 "https://github.com/ManderaGeneral/generalpackager"
 style 5 fill:#482
@@ -47,251 +66,319 @@
 | `pip install`                                                                      | `generalpackager`   |
 |:-----------------------------------------------------------------------------------|:--------------------|
 | <a href='https://pypi.org/project/generallibrary[table]'>generallibrary[table]</a> | ✔️                  |
 | <a href='https://pypi.org/project/generalfile'>generalfile</a>                     | ✔️                  |
 | <a href='https://pypi.org/project/requests'>requests</a>                           | ✔️                  |
 | <a href='https://pypi.org/project/pyinstaller'>pyinstaller</a>                     | ✔️                  |
 | <a href='https://pypi.org/project/coverage'>coverage</a>                           | ✔️                  |
+| <a href='https://pypi.org/project/setuptools'>setuptools</a>                       | ✔️                  |
+| <a href='https://pypi.org/project/wheel'>wheel</a>                                 | ✔️                  |
+| <a href='https://pypi.org/project/twine'>twine</a>                                 | ✔️                  |
 </details>
 
 
 <details open>
 <summary><h2>Information</h2></summary>
 
-| Package                                                              | Ver                                                | Latest Release       | Python                                                                                                                                                                                                                                                 | Platform        | Cover   |
-|:---------------------------------------------------------------------|:---------------------------------------------------|:---------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------------|:--------|
-| [generalpackager](https://github.com/ManderaGeneral/generalpackager) | [0.5.7](https://pypi.org/project/generalpackager/) | 2023-02-02 13:29 CET | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/downloads/release/python-3100/), [3.11](https://www.python.org/downloads/release/python-3110/) | Windows, Ubuntu | 68.9 %  |
+| Package                                                              | Ver                                                | Latest Release        | Python                                                                                                                                                                                                                                                 | Platform        | Cover   |
+|:---------------------------------------------------------------------|:---------------------------------------------------|:----------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------------|:--------|
+| [generalpackager](https://github.com/ManderaGeneral/generalpackager) | [0.5.8](https://pypi.org/project/generalpackager/) | 2023-06-02 23:27 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/downloads/release/python-3100/), [3.11](https://www.python.org/downloads/release/python-3110/) | Windows, Ubuntu | 67.8 %  |
 </details>
 
 
 
 <details>
 <summary><h2>Attributes</h2></summary>
 
 <pre>
 <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/__init__.py#L1'>Module: generalpackager</a>
-├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L11'>Class: GitHub</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L11'>Class: GitHub</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L8'>Class: LocalModule</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L16'>Class: LocalRepo</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L22'>Class: Packager</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L26'>Class: PyPI</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L27'>Method: api_url</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L43'>Method: download</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L39'>Method: exists</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L96'>Method: get_description</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L64'>Method: get_owners_packages</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L83'>Method: get_topics</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L71'>Method: get_website</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L32'>Property: git_clone_command</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L36'>Property: pip_install_command</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L108'>Method: request_kwargs</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L102'>Method: set_description</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L89'>Method: set_topics</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L77'>Method: set_website</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L24'>Property: ssh_url</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L20'>Property: url</a>
-├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L8'>Class: LocalModule</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L11'>Class: GitHub</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L8'>Class: LocalModule</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L16'>Class: LocalRepo</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L22'>Class: Packager</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L26'>Class: PyPI</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L26'>Method: exists</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L67'>Method: get_all_local_modules</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L89'>Method: get_dependants</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L74'>Method: get_dependencies</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L20'>Property: module</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L41'>Property: objInfo</a>
+├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L13'>Class: GitHub</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L13'>Class: GitHub</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L9'>Class: LocalModule</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L17'>Class: LocalRepo</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L17'>Class: Packager</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L27'>Class: PyPI</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L54'>Method: api_url</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L23'>Method: format_version</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L133'>Method: get_description</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L120'>Method: get_topics</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L108'>Method: get_website</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L58'>Method: git_clone_command</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L40'>Method: is_general</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L36'>Method: name_is_general</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L71'>Property: pip_install_command</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L145'>Method: request_kwargs</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L139'>Method: set_description</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L126'>Method: set_topics</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L114'>Method: set_website</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L45'>Property: simple_name</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L51'>Property: ssh_url</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L18'>Method: tag_is_version</a>
+├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L9'>Class: LocalModule</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L13'>Class: GitHub</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L9'>Class: LocalModule</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L17'>Class: LocalRepo</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L17'>Class: Packager</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L27'>Class: PyPI</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L27'>Method: exists</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L68'>Method: get_all_local_modules</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L90'>Method: get_dependants</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L75'>Method: get_dependencies</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L21'>Property: module</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L42'>Property: objInfo</a>
 │  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/#L426'>Property: path</a>
-├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L16'>Class: LocalRepo</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L11'>Class: GitHub</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L8'>Class: LocalModule</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L16'>Class: LocalRepo</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L22'>Class: Packager</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L26'>Class: PyPI</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/targets.py#L4'>Class: Targets</a>
+├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L17'>Class: LocalRepo</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L13'>Class: GitHub</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L9'>Class: LocalModule</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L17'>Class: LocalRepo</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L17'>Class: Packager</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L27'>Class: PyPI</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L8'>Class: Targets</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/decos.py#L4'>Method: changed_files</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/decos.py#L4'>Method: clone</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/decos.py#L4'>Method: commit</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_git.py#L12'>Method: commit_message</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/commit_editmsg.py#L5'>Class: commit_editmsg_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_git.py#L11'>Method: commit_message</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/decos.py#L4'>Method: commit_sha</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_git.py#L72'>Method: commit_sha_short</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L55'>Method: exists</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L114'>Method: format_file</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L92'>Method: get_examples_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L60'>Method: get_exeproduct_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L56'>Method: get_exetarget_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L52'>Method: get_generate_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_git.py#L76'>Method: commit_sha_short</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/examples.py#L5'>Class: examples_folder</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/exeproduct.py#L5'>Class: exeproduct_folder</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/exetarget.py#L5'>Class: exetarget_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L45'>Method: exists</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L104'>Method: format_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/generate.py#L6'>Class: generate_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_git.py#L88'>Method: get_all_versions</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L88'>Method: get_examples_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L56'>Method: get_exeproduct_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L52'>Method: get_exetarget_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L27'>Method: get_file_from_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L11'>Method: get_filenames</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L17'>Method: get_files</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L22'>Method: get_files_by_relative_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L48'>Method: get_generate_path</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L16'>Method: get_git_exclude_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L64'>Method: get_git_ignore_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L72'>Method: get_index_js_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L60'>Method: get_git_ignore_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L68'>Method: get_index_js_path</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L44'>Method: get_init_path</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L28'>Method: get_license_path</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L24'>Method: get_manifest_path</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L12'>Method: get_metadata_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L68'>Method: get_npm_ignore_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L64'>Method: get_npm_ignore_path</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L8'>Method: get_org_readme_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L80'>Method: get_package_json_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L72'>Method: get_package_paths_gen</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L84'>Method: get_pre_commit_hook_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L88'>Method: get_pre_push_hook_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L48'>Method: get_randomtesting_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L76'>Method: get_package_json_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L62'>Method: get_package_paths_gen</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L80'>Method: get_pre_commit_hook_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L84'>Method: get_pre_push_hook_path</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L4'>Method: get_readme_path</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L20'>Method: get_setup_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L76'>Method: get_test_js_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L72'>Method: get_test_js_path</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L36'>Method: get_test_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L66'>Method: get_test_paths</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L56'>Method: get_test_paths</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L40'>Method: get_test_template_path</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L32'>Method: get_workflow_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_git.py#L29'>Method: git_config</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_git.py#L21'>Method: git_missing_credentials</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_git.py#L25'>Method: git_nothing_to_commit</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_git.py#L28'>Method: git_config</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/git_exclude.py#L5'>Class: git_exclude_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_git.py#L20'>Method: git_missing_credentials</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_git.py#L24'>Method: git_nothing_to_commit</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/gitignore.py#L5'>Class: gitignore_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/index_js.py#L6'>Class: index_js_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/decos.py#L4'>Method: init</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_target.py#L18'>Method: is_django</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_target.py#L22'>Method: is_exe</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L41'>Method: is_general</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_target.py#L14'>Method: is_node</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_target.py#L10'>Method: is_python</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L33'>Property: metadata</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L48'>Method: metadata_exists</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L37'>Method: name_is_general</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/init.py#L6'>Class: init_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L28'>Method: is_django</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L32'>Method: is_exe</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L40'>Method: is_general</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L24'>Method: is_node</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L20'>Method: is_python</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/license.py#L6'>Class: license_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/manifest.py#L5'>Class: manifest_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L34'>Property: metadata</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L38'>Method: metadata_exists</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/metadata.py#L5'>Class: metadata_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L36'>Method: name_is_general</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/npm_ignore.py#L5'>Class: npm_ignore_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/org_readme.py#L6'>Class: org_readme_file</a>
+│  │  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/org_readme.py#L18'>Method: get_org_description_markdown</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/package_json.py#L6'>Class: package_json_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/pre_commit_hook.py#L4'>Class: pre_commit_hook_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/pre_push_hook.py#L6'>Class: pre_push_hook_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/decos.py#L4'>Method: push</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L60'>Method: repo_exists</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L46'>Property: simple_name</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L42'>Property: target</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_target.py#L49'>Method: targetted</a>
-├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/node/localrepo_node.py#L6'>Class: LocalRepo_Node</a>
-├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L11'>Class: LocalRepo_Python</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L16'>Method: get_python_exe_path</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L21'>Method: unittest</a>
-├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L22'>Class: Packager</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L11'>Class: GitHub</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L8'>Class: LocalModule</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L16'>Class: LocalRepo</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L22'>Class: Packager</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/other/packages.py#L9'>Class: Packages</a>
-│  │  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/other/packages.py#L34'>Method: all_packages</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L26'>Class: PyPI</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/targets.py#L4'>Class: Targets</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L20'>Method: commit_and_push</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L8'>Class: readme_file</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L125'>Method: get_attributes_markdown</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L17'>Method: get_badges_dict</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L246'>Method: get_contributions_markdown</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L27'>Method: get_description_markdown</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L89'>Method: get_examples_markdown</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L195'>Method: get_footnote_markdown</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L219'>Method: get_information_markdown</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L44'>Method: get_installation_markdown</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L209'>Method: get_mermaid_markdown</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L163'>Method: get_todos</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L169'>Method: get_todos_markdown</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L204'>Method: github_link</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L137'>Method: github_link_path_line</a>
+│  │  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L189'>Method: set_collapsible</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L50'>Method: repo_exists</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/setup.py#L6'>Class: setup_file</a>
+│  │  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/setup.py#L21'>Method: get_classifiers</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L45'>Property: simple_name</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_target.py#L18'>Method: targetted</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/test.py#L5'>Class: test_folder</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/test_js.py#L6'>Class: test_js_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/test_template.py#L6'>Class: test_template_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/workflow_dev.py#L4'>Class: workflow_dev_file</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/workflow.py#L7'>Class: workflow_file</a>
+│     └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/workflow.py#L15'>Method: codeline</a>
+├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/node/localrepo_node.py#L9'>Class: LocalRepo_Node</a>
+├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L12'>Class: LocalRepo_Python</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L17'>Method: get_python_exe_path</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L57'>Method: set_easy_install_value</a>
+├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L17'>Class: Packager</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L13'>Class: GitHub</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L9'>Class: LocalModule</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L17'>Class: LocalRepo</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L17'>Class: Packager</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L37'>Class: Packages</a>
+│  │  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L62'>Method: all_packages</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L27'>Class: PyPI</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L8'>Class: Targets</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L22'>Method: commit_and_push</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/commit_editmsg.py#L5'>Class: commit_editmsg_file</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L46'>Method: compare_local_to_github</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L53'>Method: compare_local_to_pypi</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L8'>Method: create_blank_locally_python</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L32'>Method: create_github_repo</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L36'>Method: create_master_branch</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L38'>Method: compare_local_to_github</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L45'>Method: compare_local_to_pypi</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L7'>Method: create_blank_locally</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L34'>Method: create_github_repo</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L38'>Method: create_master_branch</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/examples.py#L5'>Class: examples_folder</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/exeproduct.py#L5'>Class: exeproduct_folder</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/exetarget.py#L5'>Class: exetarget_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_relations.py#L77'>Method: general_bumped_set</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_relations.py#L85'>Method: general_changed_dict</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/generate.py#L6'>Class: generate_file</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L69'>Method: generate_localfiles</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_metadata.py#L27'>Method: get_classifiers</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L61'>Method: generate_localfiles</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_metadata.py#L29'>Method: get_classifiers</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_relations.py#L38'>Method: get_dependants</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_relations.py#L23'>Method: get_dependencies</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L29'>Method: get_file_from_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L13'>Method: get_filenames</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L19'>Method: get_files</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L24'>Method: get_files_by_relative_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L27'>Method: get_file_from_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L11'>Method: get_filenames</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L17'>Method: get_files</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L22'>Method: get_files_by_relative_path</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_pypi.py#L8'>Method: get_latest_release</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_relations.py#L49'>Method: get_ordered_packagers</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_relations.py#L71'>Method: get_owners_package_names</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_metadata.py#L4'>Method: get_topics</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_metadata.py#L6'>Method: get_topics</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/git_exclude.py#L5'>Class: git_exclude_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L81'>Property: github</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L47'>Method: github_available</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L64'>Method: if_publish_bump</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L71'>Method: if_publish_upload</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L49'>Method: github_available</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/gitignore.py#L5'>Class: gitignore_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L71'>Method: if_publish_bump</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L78'>Method: if_publish_upload</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/index_js.py#L6'>Class: index_js_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/init.py#L6'>Class: init_file</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_metadata.py#L33'>Method: is_bumped</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_target.py#L18'>Method: is_django</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_target.py#L22'>Method: is_exe</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L41'>Method: is_general</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_target.py#L14'>Method: is_node</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_target.py#L10'>Method: is_python</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_metadata.py#L35'>Method: is_bumped</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L28'>Method: is_django</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L32'>Method: is_exe</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L40'>Method: is_general</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L24'>Method: is_node</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L20'>Method: is_python</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/license.py#L6'>Class: license_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L88'>Property: localmodule</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L52'>Method: localmodule_available</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L71'>Property: localrepo</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L42'>Method: localrepo_available</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L54'>Method: localmodule_available</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L73'>Property: localrepo</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L44'>Method: localrepo_available</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/manifest.py#L5'>Class: manifest_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/metadata.py#L5'>Class: metadata_file</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L37'>Method: name_is_general</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L36'>Method: name_is_general</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_environment.py#L9'>Method: new_clean_environment</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/npm_ignore.py#L5'>Class: npm_ignore_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/org_readme.py#L6'>Class: org_readme_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/package_json.py#L6'>Class: package_json_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_relations.py#L11'>Method: packagers_from_packages</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/pre_commit_hook.py#L4'>Class: pre_commit_hook_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/pre_push_hook.py#L6'>Class: pre_push_hook_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L14'>Method: push</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L95'>Property: pypi</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L60'>Method: pypi_available</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/randomtesting.py#L6'>Class: randomtesting_file</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L9'>Class: readme_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L62'>Method: pypi_available</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L8'>Class: readme_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_pypi.py#L23'>Method: reserve_name</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L18'>Method: run_ordered_methods</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L22'>Method: run_ordered_methods</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/setup.py#L6'>Class: setup_file</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L46'>Property: simple_name</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L46'>Method: summary_packagers</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L45'>Property: simple_name</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L36'>Method: summary_packagers</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L6'>Method: sync_github_metadata</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_metadata.py#L47'>Property: target</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_metadata.py#L50'>Property: target</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/test.py#L5'>Class: test_folder</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/test_js.py#L6'>Class: test_js_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/test_template.py#L6'>Class: test_template_file</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L59'>Method: upload_package_summary</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/workflow.py#L6'>Class: workflow_file</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L8'>Method: workflow_sync</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L8'>Method: workflow_unittest</a>
-└─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L26'>Class: PyPI</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L11'>Class: GitHub</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L8'>Class: LocalModule</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L16'>Class: LocalRepo</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L22'>Class: Packager</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L26'>Class: PyPI</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L47'>Method: download</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L37'>Method: exists</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L70'>Method: get_date</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L59'>Method: get_owners_packages</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L41'>Method: get_tarball_url</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L63'>Method: get_version</a>
-   └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L34'>Property: url</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L66'>Method: upload_package_summary</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/workflow_dev.py#L4'>Class: workflow_dev_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/workflow.py#L7'>Class: workflow_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L18'>Method: workflow_packagers</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L7'>Method: workflow_sync</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L7'>Method: workflow_unittest</a>
+├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L27'>Class: PyPI</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L13'>Class: GitHub</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L9'>Class: LocalModule</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L17'>Class: LocalRepo</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L17'>Class: Packager</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L27'>Class: PyPI</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L40'>Method: is_general</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L36'>Property: json_endpoint</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L36'>Method: name_is_general</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L45'>Property: simple_name</a>
+└─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L9'>Class: Venv</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L69'>Method: active</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L72'>Method: create_venv</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv_cruds.py#L69'>Property: cruds</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L85'>Method: deactivate</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L171'>Method: debug</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L54'>Method: easy_install_path</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L48'>Method: exe_name</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L66'>Method: exists</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L30'>Method: get_active_python</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L18'>Method: get_active_venv</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L24'>Method: get_active_venv_path</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L131'>Method: list_python_versions</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L120'>Method: list_venv_paths</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L52'>Method: python_exe_path</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L56'>Method: python_home_exe_path</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L55'>Method: python_home_path</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L60'>Method: python_path</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L58'>Method: python_sys_executable_path</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L117'>Method: python_version</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L50'>Method: pyvenv_cfg_path</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L51'>Method: scripts_path</a>
+   └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L53'>Method: site_packages_path</a>
 </pre>
 </details>
 
 
 <details open>
 <summary><h2>Contributions</h2></summary>
 
-Issue-creation and discussions are most welcome!
-
-Pull requests are currently not wanted, please discuss with me before investing any time
+Issue-creation, discussions and pull requests are most welcome!
 </details>
 
 
 <details>
 <summary><h2>Todo</h2></summary>
 
 | Module                                                                                                                                                      | Message                                                                                                                                                                                                          |
 |:------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L1'>packager_files.py</a>                          | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L10'>Fix create_blank, it overwrites current projects pip install.</a>                                  |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L1'>localrepo_python.py</a> | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L55'>Make sure twine is installed when trying to upload to pypi.</a>             |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L1'>localrepo_python.py</a> | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L56'>Look into private PyPI server where we could also do dry runs for test.</a> |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/metadata_python.py#L1'>metadata_python.py</a>   | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/metadata_python.py#L4'>Dynamic values in DataClass to remove LocalRepos and Metadatas.</a>           |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L1'>localrepo.py</a>                 | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L21'>Search for imports to list dependencies.</a>                                         |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L1'>pypi.py</a>                                          | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L12'>Move download to it's own package.</a>                                                                   |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L1'>pypi.py</a>                                          | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L66'>Find a faster fetch for latest PyPI version and datetime.</a>                                            |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L1'>readme.py</a>             | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L167'>Sort todos by name to decrease automatic commit changes.</a>                 |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L1'>github.py</a>                                      | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L13'>Get and Set GitHub repo private.</a>                                                                   |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/other/packages.py#L1'>packages.py</a>                                | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/other/packages.py#L11'>Generate Python file in generalpackager containing general packages.</a>                           |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L1'>packager_github.py</a>                        | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L43'>Setup env vars for project.</a>                                                                   |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L1'>packager_files.py</a>                          | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L9'>Fix create_blank, it overwrites current projects pip install.</a>                                   |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L1'>packager_github.py</a>                        | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L44'>Setup env vars for project.</a>                                                                   |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L1'>target.py</a>                               | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L39'>Generate Python file in generalpackager containing general packages.</a>                        |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L1'>readme.py</a>             | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L166'>Sort todos by name to decrease automatic commit changes.</a>                 |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L1'>pypi.py</a>                            | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L13'>Move download to it's own package.</a>                                                     |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L1'>pypi.py</a>                            | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L78'>Find a faster fetch for latest PyPI version and datetime.</a>                              |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L1'>github.py</a>                        | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L15'>Get and Set GitHub repo private.</a>                                                     |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L1'>localrepo_python.py</a> | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L77'>Make sure twine is installed when trying to upload to pypi.</a>             |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L1'>localrepo_python.py</a> | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L78'>Look into private PyPI server where we could also do dry runs for test.</a> |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L1'>localrepo.py</a>                 | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L22'>Search for imports to list dependencies.</a>                                         |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L1'>packager_api.py</a>                              | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L43'>Check that every API has create an *_available method</a>                                            |
 </details>
 
 
 <sup>
-Generated 2023-02-02 13:29 CET for commit <a href='https://github.com/ManderaGeneral/generalpackager/commit/master'>master</a>.
+Generated 2023-06-02 23:27 CEST for commit <a href='https://github.com/ManderaGeneral/generalpackager/commit/master'>master</a>.
 </sup>
 </details>
```

#### html2text {}

```diff
@@ -1,70 +1,84 @@
+Metadata-Version: 2.1 Name: generalpackager Version: 0.5.8 Summary: Tools to
+interface GitHub, PyPI, NPM and local modules / repos. Used for generating
+files to keep projects dry and synced. Tailored for ManderaGeneral for now.
+Home-page: https://github.com/ManderaGeneral/generalpackager Author: Rickard
+"Mandera" Abraham Author-email: rickard.abraham@gmail.com License: mit
+Classifier: Topic :: Software Development :: Build Tools Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: License :: OSI Approved ::
+MIT License Classifier: Operating System :: Microsoft :: Windows Classifier:
+Operating System :: POSIX :: Linux Description-Content-Type: text/markdown
+License-File: LICENSE
 ****** generalpackager ******
 Tools to interface GitHub, PyPI, NPM and local modules / repos. Used for
 generating files to keep projects dry and synced. Tailored for ManderaGeneral
 for now.
 ***** Table of Contents *****
 generalpackager
 ââ Dependency_Diagram_for_ManderaGeneral
 ââ Installation_showing_dependencies
 ââ Information
 ââ Attributes
 ââ Contributions
 ââ Todo
 
 ***** Dependency Diagram for ManderaGeneral *****
-```mermaid flowchart LR 3([file]) --> 5([packager]) 0([import]) --> 3([file]) 2
-([library]) --> 3([file]) 2([library]) --> 4([vector]) 2([library]) --> 5(
-[packager]) 1([tool]) --> 2([library]) 0([import]) --> 2([library]) click 0
+```mermaid flowchart LR 2([library]) --> 5([packager]) 2([library]) --> 4(
+[vector]) 3([file]) --> 5([packager]) 0([import]) --> 3([file]) 1([tool]) --> 2
+([library]) 0([import]) --> 2([library]) 2([library]) --> 3([file]) click 0
 "https://github.com/ManderaGeneral/generalimport" click 1 "https://github.com/
 ManderaGeneral/generaltool" click 2 "https://github.com/ManderaGeneral/
 generallibrary" click 3 "https://github.com/ManderaGeneral/generalfile" click 4
 "https://github.com/ManderaGeneral/generalvector" click 5 "https://github.com/
 ManderaGeneral/generalpackager" style 5 fill:#482 ```
 ***** Installation showing dependencies *****
 | `pip install` | `generalpackager` | |:---------------------------------------
 --------------------------------------------|:--------------------| |
 generallibrary[table] | âï¸ | | generalfile | âï¸ | | requests | âï¸ |
-| pyinstaller | âï¸ | | coverage | âï¸ |
+| pyinstaller | âï¸ | | coverage | âï¸ | | setuptools | âï¸ | | wheel
+| âï¸ | | twine | âï¸ |
 ***** Information *****
 | Package | Ver | Latest Release | Python | Platform | Cover | |:--------------
 -------------------------------------------------------|:----------------------
------------------------------|:---------------------|:-------------------------
+-----------------------------|:----------------------|:------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
-----------------------------------------------------------------|:-------------
----|:--------| | [generalpackager](https://github.com/ManderaGeneral/
-generalpackager) | [0.5.7](https://pypi.org/project/generalpackager/) | 2023-
-02-02 13:29 CET | [3.8](https://www.python.org/downloads/release/python-380/),
+-----------------------------------------------------------------|:------------
+----|:--------| | [generalpackager](https://github.com/ManderaGeneral/
+generalpackager) | [0.5.8](https://pypi.org/project/generalpackager/) | 2023-
+06-02 23:27 CEST | [3.8](https://www.python.org/downloads/release/python-380/),
 [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://
 www.python.org/downloads/release/python-3100/), [3.11](https://www.python.org/
-downloads/release/python-3110/) | Windows, Ubuntu | 68.9 % |
+downloads/release/python-3110/) | Windows, Ubuntu | 67.8 % |
 ***** Attributes *****
 Module:_generalpackager
 ââ Class:_GitHub
 â  ââ Class:_GitHub
 â  ââ Class:_LocalModule
 â  ââ Class:_LocalRepo
 â  ââ Class:_Packager
 â  ââ Class:_PyPI
 â  ââ Method:_api_url
-â  ââ Method:_download
-â  ââ Method:_exists
+â  ââ Method:_format_version
 â  ââ Method:_get_description
-â  ââ Method:_get_owners_packages
 â  ââ Method:_get_topics
 â  ââ Method:_get_website
-â  ââ Property:_git_clone_command
+â  ââ Method:_git_clone_command
+â  ââ Method:_is_general
+â  ââ Method:_name_is_general
 â  ââ Property:_pip_install_command
 â  ââ Method:_request_kwargs
 â  ââ Method:_set_description
 â  ââ Method:_set_topics
 â  ââ Method:_set_website
+â  ââ Property:_simple_name
 â  ââ Property:_ssh_url
-â  ââ Property:_url
+â  ââ Method:_tag_is_version
 ââ Class:_LocalModule
 â  ââ Class:_GitHub
 â  ââ Class:_LocalModule
 â  ââ Class:_LocalRepo
 â  ââ Class:_Packager
 â  ââ Class:_PyPI
 â  ââ Method:_exists
@@ -80,79 +94,123 @@
 â  ââ Class:_LocalRepo
 â  ââ Class:_Packager
 â  ââ Class:_PyPI
 â  ââ Class:_Targets
 â  ââ Method:_changed_files
 â  ââ Method:_clone
 â  ââ Method:_commit
+â  ââ Class:_commit_editmsg_file
 â  ââ Method:_commit_message
 â  ââ Method:_commit_sha
 â  ââ Method:_commit_sha_short
+â  ââ Class:_examples_folder
+â  ââ Class:_exeproduct_folder
+â  ââ Class:_exetarget_file
 â  ââ Method:_exists
 â  ââ Method:_format_file
+â  ââ Class:_generate_file
+â  ââ Method:_get_all_versions
 â  ââ Method:_get_examples_path
 â  ââ Method:_get_exeproduct_path
 â  ââ Method:_get_exetarget_path
+â  ââ Method:_get_file_from_path
+â  ââ Method:_get_filenames
+â  ââ Method:_get_files
+â  ââ Method:_get_files_by_relative_path
 â  ââ Method:_get_generate_path
 â  ââ Method:_get_git_exclude_path
 â  ââ Method:_get_git_ignore_path
 â  ââ Method:_get_index_js_path
 â  ââ Method:_get_init_path
 â  ââ Method:_get_license_path
 â  ââ Method:_get_manifest_path
 â  ââ Method:_get_metadata_path
 â  ââ Method:_get_npm_ignore_path
 â  ââ Method:_get_org_readme_path
 â  ââ Method:_get_package_json_path
 â  ââ Method:_get_package_paths_gen
 â  ââ Method:_get_pre_commit_hook_path
 â  ââ Method:_get_pre_push_hook_path
-â  ââ Method:_get_randomtesting_path
 â  ââ Method:_get_readme_path
 â  ââ Method:_get_setup_path
 â  ââ Method:_get_test_js_path
 â  ââ Method:_get_test_path
 â  ââ Method:_get_test_paths
 â  ââ Method:_get_test_template_path
 â  ââ Method:_get_workflow_path
 â  ââ Method:_git_config
+â  ââ Class:_git_exclude_file
 â  ââ Method:_git_missing_credentials
 â  ââ Method:_git_nothing_to_commit
+â  ââ Class:_gitignore_file
+â  ââ Class:_index_js_file
 â  ââ Method:_init
+â  ââ Class:_init_file
 â  ââ Method:_is_django
 â  ââ Method:_is_exe
 â  ââ Method:_is_general
 â  ââ Method:_is_node
 â  ââ Method:_is_python
+â  ââ Class:_license_file
+â  ââ Class:_manifest_file
 â  ââ Property:_metadata
 â  ââ Method:_metadata_exists
+â  ââ Class:_metadata_file
 â  ââ Method:_name_is_general
+â  ââ Class:_npm_ignore_file
+â  ââ Class:_org_readme_file
+â  â  ââ Method:_get_org_description_markdown
+â  ââ Class:_package_json_file
+â  ââ Class:_pre_commit_hook_file
+â  ââ Class:_pre_push_hook_file
 â  ââ Method:_push
+â  ââ Class:_readme_file
+â  â  ââ Method:_get_attributes_markdown
+â  â  ââ Method:_get_badges_dict
+â  â  ââ Method:_get_contributions_markdown
+â  â  ââ Method:_get_description_markdown
+â  â  ââ Method:_get_examples_markdown
+â  â  ââ Method:_get_footnote_markdown
+â  â  ââ Method:_get_information_markdown
+â  â  ââ Method:_get_installation_markdown
+â  â  ââ Method:_get_mermaid_markdown
+â  â  ââ Method:_get_todos
+â  â  ââ Method:_get_todos_markdown
+â  â  ââ Method:_github_link
+â  â  ââ Method:_github_link_path_line
+â  â  ââ Method:_set_collapsible
 â  ââ Method:_repo_exists
+â  ââ Class:_setup_file
+â  â  ââ Method:_get_classifiers
 â  ââ Property:_simple_name
-â  ââ Property:_target
-â  ââ Method:_targetted
+â  ââ Method:_targetted
+â  ââ Class:_test_folder
+â  ââ Class:_test_js_file
+â  ââ Class:_test_template_file
+â  ââ Class:_workflow_dev_file
+â  ââ Class:_workflow_file
+â     ââ Method:_codeline
 ââ Class:_LocalRepo_Node
 ââ Class:_LocalRepo_Python
 â  ââ Method:_get_python_exe_path
-â  ââ Method:_unittest
+â  ââ Method:_set_easy_install_value
 ââ Class:_Packager
 â  ââ Class:_GitHub
 â  ââ Class:_LocalModule
 â  ââ Class:_LocalRepo
 â  ââ Class:_Packager
 â  ââ Class:_Packages
 â  â  ââ Method:_all_packages
 â  ââ Class:_PyPI
 â  ââ Class:_Targets
 â  ââ Method:_commit_and_push
 â  ââ Class:_commit_editmsg_file
 â  ââ Method:_compare_local_to_github
 â  ââ Method:_compare_local_to_pypi
-â  ââ Method:_create_blank_locally_python
+â  ââ Method:_create_blank_locally
 â  ââ Method:_create_github_repo
 â  ââ Method:_create_master_branch
 â  ââ Class:_examples_folder
 â  ââ Class:_exeproduct_folder
 â  ââ Class:_exetarget_file
 â  ââ Method:_general_bumped_set
 â  ââ Method:_general_changed_dict
@@ -168,14 +226,15 @@
 â  ââ Method:_get_latest_release
 â  ââ Method:_get_ordered_packagers
 â  ââ Method:_get_owners_package_names
 â  ââ Method:_get_topics
 â  ââ Class:_git_exclude_file
 â  ââ Property:_github
 â  ââ Method:_github_available
+â  ââ Class:_gitignore_file
 â  ââ Method:_if_publish_bump
 â  ââ Method:_if_publish_upload
 â  ââ Class:_index_js_file
 â  ââ Class:_init_file
 â  ââ Method:_is_bumped
 â  ââ Method:_is_django
 â  ââ Method:_is_exe
@@ -196,58 +255,77 @@
 â  ââ Class:_package_json_file
 â  ââ Method:_packagers_from_packages
 â  ââ Class:_pre_commit_hook_file
 â  ââ Class:_pre_push_hook_file
 â  ââ Method:_push
 â  ââ Property:_pypi
 â  ââ Method:_pypi_available
-â  ââ Class:_randomtesting_file
 â  ââ Class:_readme_file
 â  ââ Method:_reserve_name
 â  ââ Method:_run_ordered_methods
 â  ââ Class:_setup_file
 â  ââ Property:_simple_name
 â  ââ Method:_summary_packagers
 â  ââ Method:_sync_github_metadata
 â  ââ Property:_target
 â  ââ Class:_test_folder
 â  ââ Class:_test_js_file
 â  ââ Class:_test_template_file
 â  ââ Method:_upload_package_summary
+â  ââ Class:_workflow_dev_file
 â  ââ Class:_workflow_file
+â  ââ Method:_workflow_packagers
 â  ââ Method:_workflow_sync
 â  ââ Method:_workflow_unittest
-ââ Class:_PyPI
-   ââ Class:_GitHub
-   ââ Class:_LocalModule
-   ââ Class:_LocalRepo
-   ââ Class:_Packager
-   ââ Class:_PyPI
-   ââ Method:_download
+ââ Class:_PyPI
+â  ââ Class:_GitHub
+â  ââ Class:_LocalModule
+â  ââ Class:_LocalRepo
+â  ââ Class:_Packager
+â  ââ Class:_PyPI
+â  ââ Method:_is_general
+â  ââ Property:_json_endpoint
+â  ââ Method:_name_is_general
+â  ââ Property:_simple_name
+ââ Class:_Venv
+   ââ Method:_active
+   ââ Method:_create_venv
+   ââ Property:_cruds
+   ââ Method:_deactivate
+   ââ Method:_debug
+   ââ Method:_easy_install_path
+   ââ Method:_exe_name
    ââ Method:_exists
-   ââ Method:_get_date
-   ââ Method:_get_owners_packages
-   ââ Method:_get_tarball_url
-   ââ Method:_get_version
-   ââ Property:_url
+   ââ Method:_get_active_python
+   ââ Method:_get_active_venv
+   ââ Method:_get_active_venv_path
+   ââ Method:_list_python_versions
+   ââ Method:_list_venv_paths
+   ââ Method:_python_exe_path
+   ââ Method:_python_home_exe_path
+   ââ Method:_python_home_path
+   ââ Method:_python_path
+   ââ Method:_python_sys_executable_path
+   ââ Method:_python_version
+   ââ Method:_pyvenv_cfg_path
+   ââ Method:_scripts_path
+   ââ Method:_site_packages_path
 
 ***** Contributions *****
-Issue-creation and discussions are most welcome! Pull requests are currently
-not wanted, please discuss with me before investing any time
+Issue-creation, discussions and pull requests are most welcome!
 ***** Todo *****
 | Module | Message | |:--------------------------------------------------------
 -------------------------------------------------------------------------------
 ---------------------|:--------------------------------------------------------
 -------------------------------------------------------------------------------
 --------------------------------------------------------------------------| |
 packager_files.py | Fix_create_blank,_it_overwrites_current_projects_pip
-install. | | localrepo_python.py | Make_sure_twine_is_installed_when_trying_to
-upload_to_pypi. | | localrepo_python.py | Look_into_private_PyPI_server_where
-we_could_also_do_dry_runs_for_test. | | metadata_python.py | Dynamic_values_in
-DataClass_to_remove_LocalRepos_and_Metadatas. | | localrepo.py | Search_for
-imports_to_list_dependencies. | | pypi.py | Move_download_to_it's_own_package.
-| | pypi.py | Find_a_faster_fetch_for_latest_PyPI_version_and_datetime. | |
+install. | | packager_github.py | Setup_env_vars_for_project. | | target.py |
+Generate_Python_file_in_generalpackager_containing_general_packages. | |
 readme.py | Sort_todos_by_name_to_decrease_automatic_commit_changes. | |
-github.py | Get_and_Set_GitHub_repo_private. | | packages.py | Generate_Python
-file_in_generalpackager_containing_general_packages. | | packager_github.py |
-Setup_env_vars_for_project. |  Generated 2023-02-02 13:29 CET for commit
-master.
+pypi.py | Move_download_to_it's_own_package. | | pypi.py | Find_a_faster_fetch
+for_latest_PyPI_version_and_datetime. | | github.py | Get_and_Set_GitHub_repo
+private. | | localrepo_python.py | Make_sure_twine_is_installed_when_trying_to
+upload_to_pypi. | | localrepo_python.py | Look_into_private_PyPI_server_where
+we_could_also_do_dry_runs_for_test. | | localrepo.py | Search_for_imports_to
+list_dependencies. | | packager_api.py | Check_that_every_API_has_create_an
+*_available_method |  Generated 2023-06-02 23:27 CEST for commit master.
```

### Comparing `generalpackager-0.5.7/generalpackager/__init__.py` & `generalpackager-0.5.8/generalpackager/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,11 +5,14 @@
 from generalpackager.packager import Packager
 
 from generalpackager.api.localrepo.base.localrepo import LocalRepo
 from generalpackager.api.localrepo.python.localrepo_python import LocalRepo_Python
 from generalpackager.api.localrepo.node.localrepo_node import LocalRepo_Node
 
 from generalpackager.api.localmodule import LocalModule
-from generalpackager.api.github import GitHub
-from generalpackager.api.pypi import PyPI
+from generalpackager.api.package_hosts.github import GitHub
+from generalpackager.api.package_hosts.pypi import PyPI
+
+from generalpackager.api.venv import Venv
 
 interconnect(Packager, LocalRepo, LocalModule, GitHub, PyPI)
+
```

### Comparing `generalpackager-0.5.7/generalpackager/api/localmodule.py` & `generalpackager-0.5.8/generalpackager/api/localmodule.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 
 import pkg_resources
+
 from generalfile import Path
 from generallibrary import ObjInfo, deco_cache, EnvVar, get, import_module, deco_require, Log
-from generalpackager.api.shared.name import _SharedName, _SharedAPI
+from generalpackager.api.shared.name import _SharedAPI
 
 
-class LocalModule(_SharedAPI, _SharedName):
+class LocalModule(_SharedAPI):
     """ Tools to interface a Local Python Module. """
 
     # _deco_require_module = deco_require(lambda self: self.exists(), message=lambda func: f"{func.__name__} requires module.")
 
     def __init__(self, name=None):
         self._module = None
```

### Comparing `generalpackager-0.5.7/generalpackager/api/localrepo/base/localrepo.py` & `generalpackager-0.5.8/generalpackager/api/localrepo/base/localrepo.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 
 import re
 
-from generalfile import Path
-from generallibrary import deco_cache, deco_require
 from setuptools import find_namespace_packages
 
+from generalfile import Path
+from generallibrary import deco_cache, deco_require
 from generalpackager.api.localrepo.base.localrepo_git import _LocalRepo_Git
 from generalpackager.api.localrepo.base.localrepo_paths import _LocalRepo_Paths
 from generalpackager.api.localrepo.base.localrepo_target import _LocalRepo_Target
 from generalpackager.api.shared.files.shared_files import _Files
+from generalpackager.api.shared.name import _SharedAPI
 from generalpackager.api.shared.path import _SharedPath
-from generalpackager.api.shared.name import _SharedName, _SharedAPI
+from generalpackager.api.shared.protocols import LocalRepoProtocol
 
 
-class LocalRepo(_Files, _SharedAPI, _SharedName, _SharedPath, _LocalRepo_Paths, _LocalRepo_Target, _LocalRepo_Git):
+class LocalRepo(LocalRepoProtocol, _Files, _SharedAPI, _SharedPath, _LocalRepo_Paths, _LocalRepo_Target, _LocalRepo_Git):
     """ Tools to help Path interface a Local Repository.
         Base functionality.
         Inherited by classes in targets folder for extended functionality.
         Packager will chose correct class by using LocalRepo.metadata.target
         Todo: Search for imports to list dependencies. """
 
     _BASE_CLS_NAME = "LocalRepo"
@@ -27,27 +28,16 @@
 
     def __init__(self, name=None, path=None):
         pass
 
     @property
     @deco_cache()
     def metadata(self):
-        """ :rtype: generalpackager.api.localrepo.python.metadata_python.Metadata_Python or generalpackager.api.localrepo.node.metadata_node.Metadata_Node or generalpackager.api.localrepo.base.metadata.Metadata """
-        if self.path is None:
-            return None
-        else:
-            metadata = self._cls_metadata(path=self.get_metadata_path())
-            return metadata
-
-    @property
-    def target(self):
-        if self.metadata and self.metadata.exists():
-            return self.metadata.target
-        else:
-            return None
+        """ :rtype: generalpackager.api.localrepo.python.metadata_python.Metadata_Python or generalpackager.api.localrepo.node.metadata_node.Metadata_Node or generalpackager.api.localrepo.base.metadata._Metadata """
+        return self._cls_metadata(path=self.get_metadata_path())
 
     def metadata_exists(self):
         """ Needed to make deco_require be able to use this. """
         return bool(self.metadata and self.metadata.exists())
 
     def __repr__(self):
         return f"<{type(self).__name__} for '{self.path}'>"
```

### Comparing `generalpackager-0.5.7/generalpackager/api/localrepo/base/localrepo_git.py` & `generalpackager-0.5.8/generalpackager/api/localrepo/base/localrepo_git.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from generallibrary import Terminal
 from generalfile import Path
-
+from generallibrary import Terminal, Log
 from generalpackager.api.shared.decos import deco_path_as_working_dir
 
 
 class _LocalRepo_Git:
     # https://github.com/actions/checkout/issues/13#issuecomment-724415212
     RUNNER_NAME = "github-actions[bot]"
     RUNNER_EMAIL = "<41898282+github-actions[bot]@users.noreply.github.com>"
@@ -32,20 +31,25 @@
         Terminal("git", "config", "--global", "user.email", self.RUNNER_EMAIL)
 
     @deco_path_as_working_dir
     def commit(self, message=None, _recurse=True):
         """ Tries to commit. If credentials are missing then it sets them and tries once more.
 
             :param generalpackager.LocalRepo self: """
+        Log(__name__).debug(f"Commiting for {self} in working dir {Path.get_working_dir()}")
+        Terminal("git", "add", ".")
         terminal = Terminal("git", "commit", "-a", "-m", message or "No commit message", error=False)
         if terminal.success:
+            Log(__name__).debug(f"Commit success")
             return True
         elif self.git_nothing_to_commit(terminal=terminal):
+            Log(__name__).debug(f"Nothing to commit")
             return False
         elif _recurse and self.git_missing_credentials(terminal=terminal):
+            Log(__name__).debug(f"Missing credentials for commit, trying again")
             self.git_config()
             return self.commit(message=message, _recurse=False)
         else:
             raise terminal.error_result
 
     @deco_path_as_working_dir
     def push(self, url, tag=None):
@@ -77,15 +81,19 @@
 
     @deco_path_as_working_dir
     def changed_files(self):
         """ :param generalpackager.LocalRepo self: """
         ls_files = Terminal("git", "ls-files", "--modified").string_result
         return [Path(file) for file in ls_files.splitlines()]
 
-
+    def get_all_versions(self):
+        """ :param generalpackager.LocalRepo self: """
+        with self.path.as_working_dir():
+            terminal = Terminal("git", "tag", "-l", "--sort=-v:refname")
+        return terminal.string_result.splitlines()
```

### Comparing `generalpackager-0.5.7/generalpackager/api/localrepo/base/localrepo_paths.py` & `generalpackager-0.5.8/generalpackager/api/localrepo/base/localrepo_paths.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,18 +41,14 @@
         """ :param generalpackager.LocalRepo_Python or generalpackager.LocalRepo_Node self: """
         return self.get_test_path() / f"test_{self.name}.py"
     
     def get_init_path(self):
         """ :param generalpackager.LocalRepo_Python or generalpackager.LocalRepo_Node self: """
         return self.path / self.name / "__init__.py"
     
-    def get_randomtesting_path(self):
-        """ :param generalpackager.LocalRepo_Python or generalpackager.LocalRepo_Node self: """
-        return self.path / "randomtesting.py"
-    
     def get_generate_path(self):
         """ :param generalpackager.LocalRepo_Python or generalpackager.LocalRepo_Node self: """
         return self.path / "generate.py"
     
     def get_exetarget_path(self):
         """ :param generalpackager.LocalRepo_Python or generalpackager.LocalRepo_Node self: """
         return self.path / "exetarget.py"
```

### Comparing `generalpackager-0.5.7/generalpackager/api/localrepo/base/localrepo_target.py` & `generalpackager-0.5.8/generalpackager/api/shared/name.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,56 @@
+import re
 
-from generallibrary import DataClass
-
-import generalpackager.api.localrepo.base.targets
-from generalpackager.api.localrepo.base.metadata import Metadata
-from generalpackager.api.localrepo.base.targets import Targets
-
-
-class _SharedTarget:
-    def is_python(self):
-        """ :param generalpackager.Packager or generalpackager.LocalRepo self: """
-        return self.target == Targets.python
-
-    def is_node(self):
-        """ :param generalpackager.Packager or generalpackager.LocalRepo self: """
-        return self.target == Targets.node
-
-    def is_django(self):
-        """ :param generalpackager.Packager or generalpackager.LocalRepo self: """
-        return self.target == Targets.django
-
-    def is_exe(self):
-        """ :param generalpackager.Packager or generalpackager.LocalRepo self: """
-        return self.target == Targets.exe
-
-
-class _LocalRepo_Target(_SharedTarget):
-    """ Target of None is only for packages without a metadata.json file. """
-    Targets = Targets
-
-    _cls_target = None
-    _cls_metadata = Metadata
-    _cls_target_classes = {}
-
-    assert set(Metadata.field_dict_literals()["target"]) == set(Targets.field_values_defaults()), "Targets aren't synced, couldn't make this DRY."
-
-    def __init_subclass__(cls, **kwargs):
-        """ Return another LocalRepo object which has extended functionality based on target of metadata.
-
-            :param generalpackager._LocalRepos_DOCS cls: """
-        super().__init_subclass__(**kwargs)
-
-        if cls.__name__ != cls._BASE_CLS_NAME:
-            assert cls._cls_target in generalpackager.api.localrepo.base.targets.Targets.field_values_defaults()
-            assert cls._cls_metadata is not Metadata
-
-        cls._cls_target_classes[cls._cls_target] = cls
-
-    def targetted(self, target=...):
-        """ Return another LocalRepo object which has extended functionality based on target of metadata.
-
-            :param generalpackager._LocalRepos_DOCS self:
-            :param target:
-            :rtype: generalpackager._LocalRepos_DOCS """
-
-        if target is Ellipsis:
-            if self.metadata and self.metadata.exists():
-                target = self.metadata.target
-
-        if target in self._cls_target_classes:
-            return self._cls_target_classes[target](name=self.name, path=self.path)
+from generalfile import Path
+from generallibrary import deco_cache, Recycle, AutoInitBases
+from generalpackager.api.shared.target import Packages
+
+
+class _SharedName:
+    """ Inherited by _SharedAPI which is shared by all (Packager and APIs) """
+    DEFAULT_NAME = "generalpackager"
+
+    _recycle_keys = {"name": lambda name, path: _SharedName._scrub_name(name=name, path=path)}
+
+    def __init__(self, name=None, path=None):
+        self.name = self._scrub_name(name=name, path=path)
+
+    @classmethod
+    @deco_cache()
+    def _trim_partial(cls, name):
+        if name:
+            return re.match("(\w|[-.])+", name).group()
+
+    @classmethod
+    @deco_cache()
+    def _scrub_name(cls, name, path):
+        name = cls._trim_partial(name=name)
+
+        if path and hasattr(cls, "_scrub_path"):
+            path = Path(path)
+            if name and not path.endswith(name):
+                raise AttributeError(f"Both path and name was set for {cls} but {path} doesn't end with {name}.")
+
+            return path.stem()
+        return name or cls.DEFAULT_NAME
+
+    @staticmethod
+    def name_is_general(name):
+        return name in Packages.all_packages()
+
+    def is_general(self):
+        """ :param generalpackager.Packager self: """
+        return self.name_is_general(name=self.name)
+
+    @property
+    def simple_name(self):
+        """ :param generalpackager.Packager self: """
+        if self.name.startswith("general"):
+            return self.name.replace("general", "")
+        elif self.name.startswith("gen"):
+            return self.name.replace("gen", "")
         else:
-            return self
+            return self.name
 
 
+class _SharedAPI(_SharedName, Recycle, metaclass=AutoInitBases):
+    """ Shared by all (Packager and APIs). """
```

### Comparing `generalpackager-0.5.7/generalpackager/api/localrepo/base/metadata.py` & `generalpackager-0.5.8/generalpackager/api/localrepo/base/metadata.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-from typing import Literal
-
 from generalfile import ConfigFile
 from generallibrary import Ver
+from generalpackager.api.shared.target import _TARGETS_LITERAL, _DEFAULT_TARGET
 
 
-class Metadata(ConfigFile):
+class _Metadata(ConfigFile):
     enabled = True
     private = False
     name = None
-    target: Literal["python", "node", "django", "exe"] = "python"
+    target: _TARGETS_LITERAL = _DEFAULT_TARGET
     version = Ver("0.0.1")
     description = "Missing description."
     topics = []
     manifest = []
     contribute = False
 
     def _assert_correct_class_for_target(self):
```

### Comparing `generalpackager-0.5.7/generalpackager/api/localrepo/python/metadata_python.py` & `generalpackager-0.5.8/generalpackager/api/localrepo/python/metadata_python.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from generalpackager.api.localrepo.base.metadata import Metadata
+from generalpackager.api.localrepo.base.metadata import _Metadata
+from generalpackager.api.shared.target import Targets
 
-class Metadata_Python(Metadata):
-    """ Todo: Dynamic values in DataClass to remove LocalRepos and Metadatas. """
 
+
+class Metadata_Python(_Metadata):
+    target = Targets.python
     install_requires = []
     extras_require = {}
 
     def read_hook_post(self):
         extras_require = self.halt_getattr("extras_require")
         if extras_require:
             keys = [key for key in extras_require.values() if key != "full"]
```

### Comparing `generalpackager-0.5.7/generalpackager/api/shared/files/definitions/generate.py` & `generalpackager-0.5.8/generalpackager/api/shared/files/definitions/generate.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 class GenerateFile(File):
     _relative_path = "generate.py"
     aesthetic = True
 
     def _generate(self):
-        """ Generate randomtesting.py. """
+        """ Generate generate.py. """
         top = CodeLine(space_before=1)
         top.add_node(CodeLine(f"from generallibrary import Log"))
         top.add_node(CodeLine(f"from generalpackager import Packager", space_after=1))
         main = top.add_node(CodeLine(f'if __name__ == "__main__":'))
         main.add_node(CodeLine('Log("root").configure_stream(level=20)', ))
         main.add_node(CodeLine(f"""Packager("{self.packager.name}").generate_localfiles(print_out=20)""", space_after=50))
         return top
```

### Comparing `generalpackager-0.5.7/generalpackager/api/shared/files/definitions/org_readme.py` & `generalpackager-0.5.8/generalpackager/api/shared/files/definitions/org_readme.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from generallibrary import Markdown
 
 from generalpackager.api.shared.files.file import File
 
 
 class OrgReadmeFile(File):
-    target = None
+    target = File.targets.python
 
     @property
     def _relative_path(self):
         if self.packager.name == ".github":
             return "profile/README.md"
         else:
             return self.packager.readme_file.relative_path
```

### Comparing `generalpackager-0.5.7/generalpackager/api/shared/files/definitions/package_json.py` & `generalpackager-0.5.8/generalpackager/api/shared/files/definitions/package_json.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.7/generalpackager/api/shared/files/definitions/pre_push_hook.py` & `generalpackager-0.5.8/generalpackager/api/shared/files/definitions/pre_push_hook.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.7/generalpackager/api/shared/files/definitions/readme.py` & `generalpackager-0.5.8/generalpackager/api/shared/files/definitions/readme.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import re
 
 from generalfile import Path
 from generallibrary import Markdown, deco_cache, flatten, exclusive, Date, comma_and_and
-
 from generalpackager.api.shared.files.file import File
 
 
 class ReadmeFile(File):
     _relative_path = "README.md"
     aesthetic = True
 
@@ -249,15 +248,15 @@
         welcome = ["Issue-creation", "discussions"]
         contribute = self.packager.localrepo.metadata.contribute
 
         if contribute:
             welcome.append("pull requests")
         markdown.add_lines(f"{comma_and_and(*welcome, period=False)} are most welcome!",)
         if not contribute:
-            markdown.add_lines("", "Pull requests are currently not wanted, please discuss with me before investing any time")
+            markdown.add_lines("", "Please hold off on submitting pull requests until all the necessary legal issues have been sorted out.")
         return markdown
 
     def _generate(self):
         # Description
         markdown = self.get_description_markdown()
 
         # Table of contents
```

### Comparing `generalpackager-0.5.7/generalpackager/api/shared/files/definitions/setup.py` & `generalpackager-0.5.8/generalpackager/api/shared/files/definitions/setup.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.7/generalpackager/api/shared/files/definitions/test_js.py` & `generalpackager-0.5.8/generalpackager/api/shared/files/definitions/test_js.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.7/generalpackager/api/shared/files/definitions/test_template.py` & `generalpackager-0.5.8/generalpackager/api/shared/files/definitions/test_template.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 class TestTemplateFile(File):
     @property
     def _relative_path(self):
         return f"{self.packager.name}/test/test_{self.packager.name}.py"
 
     overwrite = False
     is_file = True
+    target = File.targets.python
+    aesthetic = True
 
     def _generate(self):
         top = CodeLine()
         top.add_node(CodeLine("from unittest import TestCase", space_after=2))
         top.add_node("class Test(TestCase):").add_node("def test(self):").add_node("pass")
         return top
```

### Comparing `generalpackager-0.5.7/generalpackager/api/shared/files/definitions/workflow.py` & `generalpackager-0.5.8/generalpackager/api/shared/files/definitions/workflow.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,92 @@
-from generallibrary import CodeLine, comma_and_and
+from generalpackager.api.shared.target import Targets
+from generallibrary import CodeLine, comma_and_and, plur_sing
 
 from generalpackager.api.shared.files.file import File
 
 
 class WorkflowFile(File):
+    target = File.targets.python
     _relative_path = ".github/workflows/workflow.yml"
     aesthetic = False
 
-    def _generate(self):
+    ON_MASTER = True
+    INCLUDE_ENVS = True
+
+    def codeline(self):
         workflow = CodeLine()
         workflow.indent_str = " " * 2
+        return workflow
 
+    def _generate(self):
+        workflow = self.codeline()
         workflow.add_node(self._get_name())
         workflow.add_node(self._get_triggers())
         workflow.add_node(self._get_defaults())
 
         jobs = workflow.add_node("jobs:")
         jobs.add_node(self._get_unittest_job())
         jobs.add_node(self._get_sync_job())
 
         return workflow
 
+    _commit_msg = "github.event.head_commit.message"
+    # _action_checkout = "actions/checkout@v2"
+    _action_setup_python = "actions/setup-python@v4"
+    _action_setup_ssh = "webfactory/ssh-agent@v0.7.0"
+    _matrix_os = "matrix.os"
+    _matrix_python_version = "matrix.python-version"
+    _branch = "github.ref_name"
+    _owner = "github.repository_owner"  # The repository owner's username. For example, octocat.
+    _repository = "github.repository"  # The owner and repository name. For example, octocat/Hello-World.
+
     PIP_NECESSARY_PACKAGES = (
         "setuptools",
         "wheel",
         "twine",
     )
+    REPOS_PATH = "repos"
+    MASTER_BRANCHES = (
+        "master",
+        "main",
+    )
 
-    _commit_msg = "github.event.head_commit.message"
-    _action_checkout = "actions/checkout@v2"
-    _action_setup_python = "actions/setup-python@v2"
-    _action_setup_ssh = "webfactory/ssh-agent@v0.5.3"
-    _matrix_os = "matrix.os"
-    _matrix_python_version = "matrix.python-version"
+
+    def _step_install_necessities(self):
+        run = CodeLine("run: |")
+        run.add_node("python -m pip install --upgrade pip")
+        run.add_node(f"pip install --upgrade {' '.join(self.PIP_NECESSARY_PACKAGES)}")
+        return self._get_step(f"Install necessities", run)
 
     @staticmethod
     def _var(string):
         return f"${{{{ {string} }}}}"
 
     @staticmethod
     def _commit_msg_if(*literals, **conditions):
         checks = [f"contains(github.event.head_commit.message, '[CI {key}]') == {str(value).lower()}" for key, value in conditions.items()]
         checks += list(literals)
         return f"if: {' && '.join(checks)}"
 
     def _get_name(self):
-        name = CodeLine("name: workflow")
+        name = CodeLine(f"name: {self.name}")
         return name
 
     def _get_triggers(self):
-        on = CodeLine("on: push", space_after=1)
+        on_branch_key = "branches" if self.ON_MASTER else "branches-ignore"
+
+        on = CodeLine("on:")
+        branches = on.add_node("push:").add_node(f"{on_branch_key}:")
+        for branch in self.MASTER_BRANCHES:
+            branches.add_node(f"- {branch}")
         return on
 
     def _get_defaults(self):
         defaults = CodeLine("defaults:")
-        defaults.add_node("run:").add_node("working-directory: ../../main", space_after=1)
+        defaults.add_node("run:").add_node("working-directory: ../../main")
         return defaults
 
     def _get_step(self, name, *codelines):
         step = CodeLine(f"- name: {name}")
         for codeline in codelines:
             if codeline:
                 step.add_node(codeline)
@@ -76,93 +104,158 @@
         return self._get_step(f"Set up Git SSH", f"uses: {self._action_setup_ssh}", with_)
 
     def _step_setup_python(self, version):
         with_ = CodeLine("with:")
         with_.add_node(f"python-version: '{version}'")
         return self._get_step(f"Set up python version {version}", f"uses: {self._action_setup_python}", with_)
 
-    def _step_install_necessities(self):
-        run = CodeLine("run: |")
-        run.add_node("python -m pip install --upgrade pip")
-        run.add_node(f"pip install {' '.join(self.PIP_NECESSARY_PACKAGES)}")
-        return self._get_step(f"Install necessities pip, setuptools, wheel, twine", run)
-
     def _step_install_package_pip(self, *packagers):
         """ Supply Packagers to create pip install steps for. """
         names = [p.name for p in packagers]
         run = CodeLine(f"run: pip install {' '.join(names)}")
         return self._get_step(f"Install pip packages {comma_and_and(*names, period=False)}", run)
 
-    def _step_clone_repos(self):
+    def _packagers(self, include_summary_packagers=None, target=None):
+        packagers = self.packager.get_ordered_packagers(include_private=False, include_summary_packagers=include_summary_packagers)
+        if not self.ON_MASTER:
+            dependencies = self.packager.get_parents(-1, include_self=True)
+            packagers = [packager for packager in packagers if packager in dependencies]
+
+        if target is not None:
+            packagers = [packager for packager in packagers if packager.target == target]
+        return packagers
+
+    @staticmethod
+    def _chain_bash(*commands, new_line=True):
+        delimiter = " || \\\n" if new_line else " || "
+        return delimiter.join(commands)
+
+    def _step_clone_repos(self, include_summary_packagers):
         """ Supply Packagers to create git install steps for. """
-        packagers = self.packager.get_ordered_packagers(include_private=False, include_summary_packagers=True)
+        packagers = self._packagers(include_summary_packagers=include_summary_packagers)
 
-        step = CodeLine(f"- name: Clone {len(packagers)} repos")
+        step = CodeLine(f"- name: Clone {plur_sing(len(packagers), 'repo')}")
         run = step.add_node(f"run: |")
+        run.add_node(f"mkdir {self.REPOS_PATH}")
+        run.add_node(f"cd {self.REPOS_PATH}")
+
+
+        owner = self._var(self._owner)
+        branch = self._var(self._branch)
 
         for packager in packagers:
-            run.add_node(packager.github.git_clone_command)
+            if self.ON_MASTER:
+                run.add_node(packager.github.git_clone_command(ssh=self.ON_MASTER))
+            else:
+                clone_commands = (
+                    packager.github.git_clone_command(ssh=self.ON_MASTER, owner=owner, branch=branch),
+                    packager.github.git_clone_command(ssh=self.ON_MASTER, owner=owner),
+                    packager.github.git_clone_command(ssh=self.ON_MASTER, branch=branch),
+                    packager.github.git_clone_command(ssh=self.ON_MASTER),
+                )
+                # new_line not working on windows
+                # https://stackoverflow.com/questions/59954185/github-action-split-long-command-into-multiple-lines
+                run.add_node(self._chain_bash(*clone_commands, new_line=False))
+
         return step
 
     def _step_install_repos(self):
         """ Supply Packagers to create git install steps for. """
-        packagers = self.packager.get_ordered_packagers(include_private=False)
+        packagers = self._packagers(target=Targets.python)
 
-        step = CodeLine(f"- name: Install {len(packagers)} repos")
+        step = CodeLine(f"- name: Install {plur_sing(len(packagers), 'repo')}")
         run = step.add_node(f"run: |")
+        run.add_node(f"cd {self.REPOS_PATH}")
 
         for packager in packagers:
-            if packager.target == packager.Targets.python:
+            if packager.target == Targets.python:
                 run.add_node(f"pip install -e {packager.name}[full]")
         return step
 
     def _get_env(self):
         env = CodeLine("env:")
         for packager in self.packager.get_all():
             for env_var in packager.localmodule.get_env_vars(error=False):
-                if env_var.actions_name and env_var.name not in str(env):  # Coupled to generallibrary.EnvVar
+                if env_var.actions_name and env_var.name not in str(env):
                     env.add_node(f"{env_var.name}: {env_var.actions_name}")
         if not env.get_children():
             return None
         return env
 
-    def _steps_setup(self, python_version):
+    def _steps_setup(self, python_version, include_summary_packagers):
         steps = CodeLine("steps:")
         steps.add_node(self._step_make_workdir())
-        steps.add_node(self._step_setup_ssh())
+        if self.ON_MASTER:
+            steps.add_node(self._step_setup_ssh())
         steps.add_node(self._step_setup_python(version=python_version))
         steps.add_node(self._step_install_necessities())
-        steps.add_node(self._step_clone_repos())
+        steps.add_node(self._step_clone_repos(include_summary_packagers=include_summary_packagers))
         steps.add_node(self._step_install_repos())
         return steps
 
     def _get_strategy(self):
         strategy = CodeLine("strategy:")
         matrix = strategy.add_node("matrix:")
         matrix.add_node(f"python-version: {list(self.packager.python)}")
         matrix.add_node(f"os: {[f'{os}-latest' for os in self.packager.os]}".replace("'", ""))
         return strategy
 
     def _get_unittest_job(self):
-        job = CodeLine("unittest:")
-        job.add_node(self._commit_msg_if("github.ref == 'refs/heads/master'", SKIP=False, AUTO=False))
+        job = CodeLine("unittest:" if self.ON_MASTER else "dev_unittest:")
+        job.add_node(self._commit_msg_if(SKIP=False, AUTO=False))
         job.add_node(f"runs-on: {self._var(self._matrix_os)}")
         job.add_node(self._get_strategy())
 
         python_version = self._var(self._matrix_python_version)
-        steps = job.add_node(self._steps_setup(python_version=python_version))
-        steps.add_node(self._step_run_packager_method("workflow_unittest"))
+        steps = job.add_node(self._steps_setup(python_version=python_version, include_summary_packagers=False))
+        if self.ON_MASTER:
+            steps.add_node(self._step_run_packager_method("workflow_unittest"))
+        else:
+            steps.add_node(self._step_run_simple_unittest())
         return job
 
     def _get_sync_job(self):
         job = CodeLine("sync:")
         job.add_node("needs: unittest")
         job.add_node(f"runs-on: ubuntu-latest")
-        steps = job.add_node(self._steps_setup(python_version=self.packager.python[-1]))
+        steps = job.add_node(self._steps_setup(python_version=self.packager.python[-1], include_summary_packagers=True))
         steps.add_node(self._step_run_packager_method("workflow_sync"))
         return job
 
     def _step_run_packager_method(self, method):
-        run = CodeLine(f'run: |')
+        step = self._get_step(f"Run Packager method '{method}'")
+
+        run = step.add_node(f'run: |')
+        run.add_node(f"cd {self.REPOS_PATH}")
         run.add_node(f'python -c "from generalpackager import Packager; Packager().{method}()"')
-        return self._get_step(f"Run Packager method '{method}'", run, self._get_env())
+
+        if self.INCLUDE_ENVS:
+            step.add_node(self._get_env())
+        return step
+
+    def _step_run_simple_unittest(self):
+        step = self._get_step(f"Run unittests")
+
+        run = step.add_node(f'run: |')
+        run.add_node(f"cd {self.REPOS_PATH}/{self.packager.name}/{self.packager.name}/test")
+
+        run.add_node(f'python -m unittest discover -v')
+        return step
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
```

### Comparing `generalpackager-0.5.7/generalpackager/api/shared/files/file.py` & `generalpackager-0.5.8/generalpackager/api/shared/files/file.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from logging import getLogger
 
 from generalfile import Path
-from generallibrary import deco_cache
-
-from generalpackager.api.localrepo.base.targets import Targets
+from generallibrary import deco_cache, CodeLine
+from generalpackager.api.shared.target import Targets
 
 
 class DynamicRelativePath:
     def __get__(self, instance, owner):
         if instance:
             return Path(instance._relative_path)
         else:
@@ -24,36 +23,53 @@
 
     remove = False
     overwrite = True
     is_file = True
     target = Targets.python  # Should probably default to None, and then I put python on most files
 
     def _generate(self):
-        return ""
+        return "" or CodeLine()
 
     def __init__(self, owner):
         """ :param generalpackager.Packager or generalpackager.LocalRepo owner: """
         self.owner = owner
-        self.packager = owner if type(owner).__name__ == "Packager" else None
-        self.localrepo = self.packager.localrepo if self.packager else owner
+
+    @property
+    def name(self):
+        return self.fullname[:-4] if self.fullname.endswith("File") else self.fullname
+        # return self.fullname.removesuffix("File") # 3.9+
+
+    @property
+    def fullname(self):
+        return type(self).__name__
+
+    @property
+    @deco_cache()
+    def packager(self):
+        return self.owner if type(self.owner).__name__ == "Packager" else None
+
+    @property
+    @deco_cache()
+    def localrepo(self):
+        return self.packager.localrepo if self.packager else self.owner
 
     relative_path = DynamicRelativePath()
 
     @classmethod
     def requires_instance(cls):
         return hasattr(cls._relative_path, "fget")
 
     @property
     @deco_cache()
     def path(self):
         return self.owner.path / self._relative_path
 
     def _cant_write(self, msg):
         logger = getLogger(__name__)
-        logger.info(f"Can't write '{self.relative_path}' - {msg}")
+        logger.info(f"Can't write '{self.fullname}' - {msg}")
         return False
 
     def can_write(self):
         if not self.is_file:
             return self._cant_write(".is_file is False")
 
         elif self.remove:
@@ -67,20 +83,29 @@
 
         elif self.overwrite is False and self.path.exists():
             return self._cant_write(f".overwrite is False and path {self.path} exists")
 
         else:
             return True
 
+    def get_generate_text(self):
+        """ Make all top children have one space after. """
+        text = self._generate()
+        if type(text) is CodeLine:
+            for codeline in text.get_children():
+                last_child = codeline.get_child(depth=-1, index=-1, include_self=True)
+                last_child.space_after = 1
+        return text
+
     def generate(self):
         logger = getLogger(__name__)
+
         if self.can_write():
             logger.info(f"Writing to '{self.relative_path}' for '{self.owner.name}'")
-            return self.path.text.write(text=f"{self._generate()}\n", overwrite=self.overwrite)
+            return self.path.text.write(text=f"{self.get_generate_text()}\n", overwrite=self.overwrite)
+
         elif self.remove:
             logger.info(f"Deleting '{self.relative_path}' for '{self.owner.name}'")
             self.path.delete()
-        else:
-            logger.warning(f"Generate for '{self.path}' could neither write nor remove.")
 
     def __str__(self):
         return f"<File: {self.owner.name} - {self.relative_path}>"
```

### Comparing `generalpackager-0.5.7/generalpackager/api/shared/files/file_fetcher.py` & `generalpackager-0.5.8/generalpackager/api/shared/files/file_fetcher.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.7/generalpackager/api/shared/files/shared_files.py` & `generalpackager-0.5.8/generalpackager/api/shared/files/shared_files.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-import importlib
-
-from generalfile import Path
 from generallibrary import deco_cache
 
 from generalpackager.api.shared.files.file_fetcher import FileFetcher
+from generalfile import Path
 
 
 class _Files:
     """ LocalRepo and Packager inherits this.
         Only an instance of Packager will return file instances. """
     @classmethod
     @deco_cache()
@@ -34,35 +32,37 @@
 
     commit_editmsg_file = FileFetcher()
     examples_folder = FileFetcher()
     exeproduct_folder = FileFetcher()
     exetarget_file = FileFetcher()
     generate_file = FileFetcher()
     git_exclude_file = FileFetcher()
+    gitignore_file = FileFetcher()
     index_js_file = FileFetcher()
     init_file = FileFetcher()
     license_file = FileFetcher()
     manifest_file = FileFetcher()
     metadata_file = FileFetcher()
     npm_ignore_file = FileFetcher()
     org_readme_file = FileFetcher()
     package_json_file = FileFetcher()
     pre_commit_hook_file = FileFetcher()
     pre_push_hook_file = FileFetcher()
-    randomtesting_file = FileFetcher()
     readme_file = FileFetcher()
     setup_file = FileFetcher()
     test_folder = FileFetcher()
     test_js_file = FileFetcher()
     test_template_file = FileFetcher()
     workflow_file = FileFetcher()
+    workflow_dev_file = FileFetcher()
+
 
 
+# Helper function to generate Files
 if __name__ == "__main__":
-    from generalfile import Path
     definitions = Path("./definitions").get_children()
     definitions = sorted(definitions, key=lambda path: path.name())
     for definition in definitions:
         stem = definition.stem()
         if stem.startswith("_"):
             continue
```

### Comparing `generalpackager-0.5.7/generalpackager/api/shared/name.py` & `generalpackager-0.5.8/generalpackager/packager_pypi.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,60 @@
-import re
 
 from generalfile import Path
-from generallibrary import deco_cache, Recycle, AutoInitBases
+from generallibrary import Date
+from requests import ConnectionError
+
+
+class _PackagerPypi:
+    def get_latest_release(self):
+        """ Use current datetime if bumped, otherwise fetch.
+
+            :param generalpackager.Packager self: """
+        try:
+            bumped = self.is_bumped()
+        except ConnectionError:
+            return "Failed fetching"
+
+        if bumped:
+            return Date.now()
+        else:
+            return self.pypi.get_date()
+
+    @classmethod
+    def reserve_name(cls, name):
+        """ Reserve a name on PyPI with template files.
+
+            :param generalpackager.Packager or any cls:
+            :param name: """
+        path = Path.get_cache_dir() / "python/pypi_reserve/" / name
+        packager = cls(path=path, target=cls.Targets.python)
+        packager.create_blank_locally(install=False)
+        packager.localrepo.publish()
+        path.delete()
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
 
-from generalpackager.other.packages import Packages
 
 
-class _SharedName:
-    """ Inherited by _SharedAPI which is shared by all (Packager and APIs) """
-    DEFAULT_NAME = "generalpackager"
 
-    _recycle_keys = {"name": lambda name, path: _SharedName._scrub_name(name=name, path=path)}
 
-    def __init__(self, name=None, path=None):
-        self.name = self._scrub_name(name=name, path=path)
 
-    @classmethod
-    @deco_cache()
-    def _trim_partial(cls, name):
-        if name:
-            return re.match("(\w|[-.])+", name).group()
 
-    @classmethod
-    @deco_cache()
-    def _scrub_name(cls, name, path):
-        name = cls._trim_partial(name=name)
-
-        if path and hasattr(cls, "_scrub_path"):
-            path = Path(path)
-            if name and not path.endswith(name):
-                raise AttributeError(f"Both path and name was set for {cls} but {path} doesn't end with {name}.")
-
-            return path.stem()
-        return name or cls.DEFAULT_NAME
-
-    @staticmethod
-    def name_is_general(name):
-        return name in Packages.all_packages()
-
-    def is_general(self):
-        """ :param generalpackager.Packager self: """
-        return self.name_is_general(name=self.name)
-
-    @property
-    def simple_name(self):
-        """ :param generalpackager.Packager self: """
-        if self.name.startswith("general"):
-            return self.name.replace("general", "")
-        elif self.name.startswith("gen"):
-            return self.name.replace("gen", "")
-        else:
-            return self.name
 
 
-class _SharedAPI(_SharedName, Recycle, metaclass=AutoInitBases):
-    """ Shared by all (Packager and APIs). """
```

### Comparing `generalpackager-0.5.7/generalpackager/api/shared/owner.py` & `generalpackager-0.5.8/generalpackager/api/shared/owner.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.7/generalpackager/api/shared/path.py` & `generalpackager-0.5.8/generalpackager/api/shared/path.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,25 +36,22 @@
         """ :param generalpackager.Packager cls:
             :rtype: Path or None """
         for method in (cls._resolve_path_localmodule, cls._resolve_path_workingdir_traverse_parents):
             path = method(name=name)
             if path and path.endswith(name):
                 Log().debug(f"Resolved path with '{method.__name__}' for '{name}', got '{path}'.")
                 return path
+        return Path(name)
 
     @classmethod
     @deco_cache()
     def _scrub_path(cls, name, path):
         """ :param generalpackager.Packager cls:
             :rtype: Path or None """
         name = cls._scrub_name(name=name, path=path)
-
         if path is None:
-            path = cls._resolve_path(name=name)
-
-        if path is not None:
+            return cls._resolve_path(name=name)
+        else:
             path = Path(path).absolute()
-
             if not path.endswith(name):
                 raise AttributeError(f"Path '{path}' seems to be wrong for '{name}'. Workdir is '{Path().absolute()}'.")
-
-        return path
+            return path
```

### Comparing `generalpackager-0.5.7/generalpackager/api/venv.py` & `generalpackager-0.5.8/generalpackager/api/venv.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,71 @@
 import re
 import sys
 
 from generalfile import Path
-from generallibrary import deco_cache, Ver, Terminal, debug, EnvVar, remove, DecoContext, deco_require, VerInfo, Log, \
-    join_with_str
+from generallibrary import deco_cache, Ver, Terminal, debug, DecoContext, deco_require, VerInfo, Log
+from generalpackager.api.venv_cruds import _Venv_Cruds
 
 
-class Venv(DecoContext):
-    """ Standalone API, unlike the other APIs this one is not included in Packager. """
-    PATH = EnvVar("PATH")
-    VIRTUAL_ENV = EnvVar("VIRTUAL_ENV", default=None)
+class Venv(DecoContext, _Venv_Cruds):
+    """ Standalone API of Python venv, unlike the other APIs this one is not included in Packager. """
     ver_info = VerInfo()
 
     def __init__(self, path=None):
         self.path = Path(path)
         self.previous_venv = None
 
     @classmethod
     def get_active_venv(cls):
         active_venv_path = Path.get_active_venv_path()
         if active_venv_path is not None:
             return Venv(path=active_venv_path)
 
+    @classmethod
+    def get_active_venv_path(cls):
+        active_venv = cls.get_active_venv()
+        if active_venv:
+            return active_venv.path
+
+    @classmethod
+    def get_active_python(cls, local):
+        active_venv = cls.get_active_venv()
+        if active_venv is None:
+            if local is True:
+                raise EnvironmentError("A local python path was requested but there's no active venv. Returning global instead.")
+                # Log(__name__).warning("A local python path was requested by there's no active venv. Returning global instead.")
+            return cls.python_sys_executable_path()
+        return active_venv.python_path(local=local)
+
     def before(self, *args, **kwargs):
         self.activate()
 
     def after(self, *args, **kwargs):
         if self.previous_venv:
             self.previous_venv.activate()
         else:
             self.deactivate()
 
+    def exe_name(self): return "python.exe" if self.ver_info.windows else "python"  # This is similar to Terminal requiring .cmd
+
     def pyvenv_cfg_path(self):  return self.path / "pyvenv.cfg"
     def scripts_path(self):     return self.path / self.ver_info.venv_script_path
-    def python_exe_path(self):  return self.scripts_path() / ("python.exe" if self.ver_info.windows else "python")
+    def python_exe_path(self):  return self.scripts_path() / self.exe_name()
     def site_packages_path(self):  return self.path / "Lib/site-packages"
-    def python_home_path(self): return Path(self.cfg()["home"])
+    def easy_install_path(self):  return self.site_packages_path() / "easy-install.pth"
+    def python_home_path(self): return Path(path=self.cfg()["home"])
+    def python_home_exe_path(self): return self.python_home_path() / self.exe_name()
+    @classmethod
+    def python_sys_executable_path(cls): return Path(path=sys.executable)
+
+    def python_path(self, local):
+        if local:
+            return self.python_exe_path()
+        else:
+            return self.python_home_exe_path()
 
     def exists(self):
         return self.path.is_venv()
 
     def active(self):
         return Path.get_active_venv_path() is self.path
 
@@ -51,42 +77,31 @@
         elif ver:
             python = self.list_python_versions()[ver]
         else:
             python = True
 
         return Terminal("-m", "venv", self.path, python=python).string_result
 
-    PATH_delimiter = ver_info.env_var_path_delimiter
-
-    @classmethod
-    def _remove_path_from_PATH(cls, path_to_remove):
-        paths = [Path(path=path_str) for path_str in cls.PATH.value.split(cls.PATH_delimiter)]
-        paths.remove(path_to_remove)
-        cls.PATH.value = join_with_str(delimiter=cls.PATH_delimiter, obj=paths)
-
-    @classmethod
-    def _add_path_to_PATH(cls, path_to_add):
-        cls.PATH.value = f"{path_to_add}{cls.PATH_delimiter}{cls.PATH}"
-
     @classmethod
     def deactivate(cls):
         active_venv = Venv.get_active_venv()
         if active_venv:
-            cls._remove_path_from_PATH(path_to_remove=active_venv.scripts_path())
-            remove(sys.path, str(active_venv.scripts_path()))
-            remove(sys.path, str(active_venv.site_packages_path()))
-            cls.VIRTUAL_ENV.remove()
+            active_venv.cruds.EnvVar_PATH.unset()
+            active_venv.cruds.EnvVar_VENV.unset()
+            active_venv.cruds.sys_path_scripts.unset()
+            active_venv.cruds.sys_path_site.unset()
             return active_venv
 
     @deco_require(exists)
     def activate(self):
         self.previous_venv = self.deactivate()
-        self._add_path_to_PATH(path_to_add=self.scripts_path())
-        sys.path = [str(self.path), str(self.site_packages_path())] + sys.path
-        self.VIRTUAL_ENV.value = self.path
+        self.cruds.EnvVar_PATH.set()
+        self.cruds.EnvVar_VENV.set()
+        self.cruds.sys_path_scripts.set()
+        self.cruds.sys_path_site.set()
 
         # Not sure these two do anything, doubt you can change interpreter during runtime
         # https://github.com/ManderaGeneral/generalpackager/issues/60
         sys.prefix = self.path
         sys.executable = self.python_exe_path()
 
     @deco_require(exists)
@@ -151,16 +166,14 @@
         return versions
 
     def __str__(self):
         return f"<Venv: {self.path}>"
 
     @staticmethod
     def debug():
-        import os
-        import sys
 
         debug(locals(),
               "os.environ['PATH']",
               "os.environ['VIRTUAL_ENV']",
               "sys.prefix",
               "sys.path",
               "sys.executable",
```

### Comparing `generalpackager-0.5.7/generalpackager/packager.py` & `generalpackager-0.5.8/generalpackager/packager.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,216 +1,184 @@
-00000000: 0d0a 6672 6f6d 2074 7970 696e 6720 696d  ..from typing im
-00000010: 706f 7274 204c 6974 6572 616c 0d0a 0d0a  port Literal....
-00000020: 6672 6f6d 2067 656e 6572 616c 6c69 6272  from generallibr
-00000030: 6172 7920 696d 706f 7274 204e 6574 776f  ary import Netwo
-00000040: 726b 4469 6167 7261 6d2c 2064 6563 6f5f  rkDiagram, deco_
-00000050: 6361 6368 650d 0a0d 0a66 726f 6d20 6765  cache....from ge
-00000060: 6e65 7261 6c70 6163 6b61 6765 722e 6170  neralpackager.ap
-00000070: 692e 6c6f 6361 6c72 6570 6f2e 6261 7365  i.localrepo.base
-00000080: 2e6c 6f63 616c 7265 706f 5f74 6172 6765  .localrepo_targe
-00000090: 7420 696d 706f 7274 205f 5368 6172 6564  t import _Shared
-000000a0: 5461 7267 6574 0d0a 6672 6f6d 2067 656e  Target..from gen
-000000b0: 6572 616c 7061 636b 6167 6572 2e61 7069  eralpackager.api
-000000c0: 2e73 6861 7265 642e 6669 6c65 732e 7368  .shared.files.sh
-000000d0: 6172 6564 5f66 696c 6573 2069 6d70 6f72  ared_files impor
-000000e0: 7420 5f46 696c 6573 0d0a 6672 6f6d 2067  t _Files..from g
-000000f0: 656e 6572 616c 7061 636b 6167 6572 2e61  eneralpackager.a
-00000100: 7069 2e73 6861 7265 642e 7061 7468 2069  pi.shared.path i
-00000110: 6d70 6f72 7420 5f53 6861 7265 6450 6174  mport _SharedPat
-00000120: 680d 0a66 726f 6d20 6765 6e65 7261 6c70  h..from generalp
-00000130: 6163 6b61 6765 722e 6170 692e 7368 6172  ackager.api.shar
-00000140: 6564 2e6e 616d 6520 696d 706f 7274 205f  ed.name import _
-00000150: 5368 6172 6564 4e61 6d65 2c20 5f53 6861  SharedName, _Sha
-00000160: 7265 6441 5049 0d0a 6672 6f6d 2067 656e  redAPI..from gen
-00000170: 6572 616c 7061 636b 6167 6572 2e70 6163  eralpackager.pac
-00000180: 6b61 6765 725f 6170 6920 696d 706f 7274  kager_api import
-00000190: 205f 5061 636b 6167 6572 4150 4973 0d0a   _PackagerAPIs..
-000001a0: 6672 6f6d 2067 656e 6572 616c 7061 636b  from generalpack
-000001b0: 6167 6572 2e70 6163 6b61 6765 725f 656e  ager.packager_en
-000001c0: 7669 726f 6e6d 656e 7420 696d 706f 7274  vironment import
-000001d0: 205f 5061 636b 6167 6572 456e 7669 726f   _PackagerEnviro
-000001e0: 6e6d 656e 740d 0a66 726f 6d20 6765 6e65  nment..from gene
-000001f0: 7261 6c70 6163 6b61 6765 722e 7061 636b  ralpackager.pack
-00000200: 6167 6572 5f66 696c 6573 2069 6d70 6f72  ager_files impor
-00000210: 7420 5f50 6163 6b61 6765 7246 696c 6573  t _PackagerFiles
-00000220: 0d0a 6672 6f6d 2067 656e 6572 616c 7061  ..from generalpa
-00000230: 636b 6167 6572 2e70 6163 6b61 6765 725f  ckager.packager_
-00000240: 6769 7468 7562 2069 6d70 6f72 7420 5f50  github import _P
-00000250: 6163 6b61 6765 7247 6974 4875 620d 0a66  ackagerGitHub..f
-00000260: 726f 6d20 6765 6e65 7261 6c70 6163 6b61  rom generalpacka
-00000270: 6765 722e 7061 636b 6167 6572 5f6d 6574  ger.packager_met
-00000280: 6164 6174 6120 696d 706f 7274 205f 5061  adata import _Pa
-00000290: 636b 6167 6572 4d65 7461 6461 7461 0d0a  ckagerMetadata..
-000002a0: 6672 6f6d 2067 656e 6572 616c 7061 636b  from generalpack
-000002b0: 6167 6572 2e70 6163 6b61 6765 725f 7079  ager.packager_py
-000002c0: 7069 2069 6d70 6f72 7420 5f50 6163 6b61  pi import _Packa
-000002d0: 6765 7250 7970 690d 0a66 726f 6d20 6765  gerPypi..from ge
-000002e0: 6e65 7261 6c70 6163 6b61 6765 722e 7061  neralpackager.pa
-000002f0: 636b 6167 6572 5f72 656c 6174 696f 6e73  ckager_relations
-00000300: 2069 6d70 6f72 7420 5f50 6163 6b61 6765   import _Package
-00000310: 7252 656c 6174 696f 6e73 0d0a 6672 6f6d  rRelations..from
-00000320: 2067 656e 6572 616c 7061 636b 6167 6572   generalpackager
-00000330: 2e70 6163 6b61 6765 725f 776f 726b 666c  .packager_workfl
-00000340: 6f77 2069 6d70 6f72 7420 5f50 6163 6b61  ow import _Packa
-00000350: 6765 7257 6f72 6b66 6c6f 770d 0a0d 0a0d  gerWorkflow.....
-00000360: 0a5f 5441 5247 4554 5320 3d20 4c69 7465  ._TARGETS = Lite
-00000370: 7261 6c5b 2270 7974 686f 6e22 2c20 226e  ral["python", "n
-00000380: 6f64 6522 2c20 2264 6a61 6e67 6f22 2c20  ode", "django", 
-00000390: 2265 7865 225d 2020 2320 5468 6973 2069  "exe"]  # This i
-000003a0: 7320 636f 7570 6c65 6420 746f 2067 656e  s coupled to gen
-000003b0: 6572 616c 7061 636b 6167 6572 2e61 7069  eralpackager.api
-000003c0: 2e6c 6f63 616c 7265 706f 2e62 6173 652e  .localrepo.base.
-000003d0: 7461 7267 6574 732e 5461 7267 6574 732c  targets.Targets,
-000003e0: 206e 6f74 2069 6465 616c 0d0a 0d0a 636c   not ideal....cl
-000003f0: 6173 7320 5061 636b 6167 6572 284e 6574  ass Packager(Net
-00000400: 776f 726b 4469 6167 7261 6d2c 0d0a 2020  workDiagram,..  
-00000410: 2020 2020 2020 2020 2020 2020 205f 4669               _Fi
-00000420: 6c65 732c 205f 5368 6172 6564 4150 492c  les, _SharedAPI,
-00000430: 205f 5368 6172 6564 4e61 6d65 2c20 5f53   _SharedName, _S
-00000440: 6861 7265 6454 6172 6765 742c 205f 5368  haredTarget, _Sh
-00000450: 6172 6564 5061 7468 2c0d 0a20 2020 2020  aredPath,..     
-00000460: 2020 2020 2020 2020 2020 5f50 6163 6b61            _Packa
-00000470: 6765 7247 6974 4875 622c 205f 5061 636b  gerGitHub, _Pack
-00000480: 6167 6572 4669 6c65 732c 205f 5061 636b  agerFiles, _Pack
-00000490: 6167 6572 4d65 7461 6461 7461 2c20 5f50  agerMetadata, _P
-000004a0: 6163 6b61 6765 7250 7970 692c 205f 5061  ackagerPypi, _Pa
-000004b0: 636b 6167 6572 576f 726b 666c 6f77 2c20  ckagerWorkflow, 
-000004c0: 5f50 6163 6b61 6765 7252 656c 6174 696f  _PackagerRelatio
-000004d0: 6e73 2c20 5f50 6163 6b61 6765 7241 5049  ns, _PackagerAPI
-000004e0: 732c 205f 5061 636b 6167 6572 456e 7669  s, _PackagerEnvi
-000004f0: 726f 6e6d 656e 7429 3a0d 0a20 2020 2022  ronment):..    "
-00000500: 2222 2055 7365 7320 4150 4973 2074 6f20  "" Uses APIs to 
-00000510: 6d61 6e61 6765 2027 6765 6e65 7261 6c27  manage 'general'
-00000520: 2070 6163 6b61 6765 2e0d 0a20 2020 2020   package...     
-00000530: 2020 2043 6f6e 7461 696e 7320 6d65 7468     Contains meth
-00000540: 6f64 7320 7468 6174 2072 6571 7569 7265  ods that require
-00000550: 206d 6f72 6520 7468 616e 206f 6e65 2041   more than one A
-00000560: 5049 2061 7320 7765 6c6c 2061 7320 6d65  PI as well as me
-00000570: 7468 6f64 7320 7370 6563 6966 6963 2066  thods specific f
-00000580: 6f72 204d 616e 6465 7261 4765 6e65 7261  or ManderaGenera
-00000590: 6c2e 2022 2222 0d0a 0d0a 2020 2020 6175  l. """....    au
-000005a0: 7468 6f72 203d 2027 5269 636b 6172 6420  thor = 'Rickard 
-000005b0: 224d 616e 6465 7261 2220 4162 7261 6861  "Mandera" Abraha
-000005c0: 6d27 0d0a 2020 2020 656d 6169 6c20 3d20  m'..    email = 
-000005d0: 2272 6963 6b61 7264 2e61 6272 6168 616d  "rickard.abraham
-000005e0: 4067 6d61 696c 2e63 6f6d 220d 0a20 2020  @gmail.com"..   
-000005f0: 206c 6963 656e 7365 203d 2022 6d69 7422   license = "mit"
-00000600: 0d0a 2020 2020 7079 7468 6f6e 203d 2022  ..    python = "
-00000610: 332e 3822 2c20 2233 2e39 222c 2022 332e  3.8", "3.9", "3.
-00000620: 3130 222c 2022 332e 3131 2220 2023 204f  10", "3.11"  # O
-00000630: 6e6c 7920 7375 7070 6f72 7473 2062 6173  nly supports bas
-00000640: 6963 2064 6566 696e 6974 696f 6e20 7769  ic definition wi
-00000650: 7468 2074 7570 6c65 206f 6620 6d61 6a6f  th tuple of majo
-00000660: 722e 6d69 6e6f 720d 0a20 2020 206f 7320  r.minor..    os 
-00000670: 3d20 2277 696e 646f 7773 222c 2022 7562  = "windows", "ub
-00000680: 756e 7475 2220 2023 202c 2022 6d61 636f  untu"  # , "maco
-00000690: 7322 0d0a 0d0a 2020 2020 6769 745f 6578  s"....    git_ex
-000006a0: 636c 7564 655f 6c69 6e65 7320 3d20 6e70  clude_lines = np
-000006b0: 6d5f 6967 6e6f 7265 5f6c 696e 6573 203d  m_ignore_lines =
-000006c0: 2022 2e69 6465 612f 222c 2022 6469 7374   ".idea/", "dist
-000006d0: 2f22 2c20 222e 6769 742f 222c 2022 2a2a  /", ".git/", "**
-000006e0: 7465 7374 2f74 6573 7473 2f22 2c20 222e  test/tests/", ".
-000006f0: 636f 7665 7261 6765 222c 2022 6874 6d6c  coverage", "html
-00000700: 636f 762f 220d 0a20 2020 2067 6974 5f65  cov/"..    git_e
-00000710: 7863 6c75 6465 5f6c 696e 6573 202b 3d20  xclude_lines += 
-00000720: 2262 7569 6c64 2f22 2c20 222a 2e65 6767  "build/", "*.egg
-00000730: 2d69 6e66 6f2f 222c 2022 5f5f 7079 6361  -info/", "__pyca
-00000740: 6368 655f 5f2f 222c 2022 504b 472d 494e  che__/", "PKG-IN
-00000750: 464f 2f22 2c20 2273 6574 7570 2e63 6667  FO/", "setup.cfg
-00000760: 220d 0a20 2020 206e 706d 5f69 676e 6f72  "..    npm_ignor
-00000770: 655f 6c69 6e65 7320 2b3d 2022 6e6f 6465  e_lines += "node
-00000780: 5f6d 6f64 756c 6573 2f22 2c20 222e 7061  _modules/", ".pa
-00000790: 7263 656c 2d63 6163 6865 2f22 0d0a 0d0a  rcel-cache/"....
-000007a0: 0d0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
-000007b0: 5f5f 2873 656c 662c 206e 616d 653d 4e6f  __(self, name=No
-000007c0: 6e65 2c20 7061 7468 3d4e 6f6e 652c 2074  ne, path=None, t
-000007d0: 6172 6765 743a 205f 5441 5247 4554 5320  arget: _TARGETS 
-000007e0: 3d20 2e2e 2e2c 2067 6974 6875 625f 6f77  = ..., github_ow
-000007f0: 6e65 723d 4e6f 6e65 2c20 7079 7069 5f6f  ner=None, pypi_o
-00000800: 776e 6572 3d4e 6f6e 6529 3a0d 0a20 2020  wner=None):..   
-00000810: 2020 2020 2022 2222 2053 746f 7269 6e67       """ Storing
-00000820: 2070 6172 7320 6173 2069 732e 204e 616d   pars as is. Nam
-00000830: 6520 616e 6420 7461 7267 6574 2068 6176  e and target hav
-00000840: 6520 736f 6d65 2063 7573 746f 6d20 7072  e some custom pr
-00000850: 6f70 6572 7469 6573 2e20 2222 220d 0a20  operties. """.. 
-00000860: 2020 2020 2020 2073 656c 662e 5f74 6172         self._tar
-00000870: 6765 7420 3d20 7461 7267 6574 0d0a 2020  get = target..  
-00000880: 2020 2020 2020 7365 6c66 2e5f 6769 7468        self._gith
-00000890: 7562 5f6f 776e 6572 203d 2067 6974 6875  ub_owner = githu
-000008a0: 625f 6f77 6e65 720d 0a20 2020 2020 2020  b_owner..       
-000008b0: 2073 656c 662e 5f70 7970 695f 6f77 6e65   self._pypi_owne
-000008c0: 7220 3d20 7079 7069 5f6f 776e 6572 0d0a  r = pypi_owner..
-000008d0: 0d0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
-000008e0: 686f 640d 0a20 2020 2040 6465 636f 5f63  hod..    @deco_c
-000008f0: 6163 6865 2829 0d0a 2020 2020 6465 6620  ache()..    def 
-00000900: 7375 6d6d 6172 795f 7061 636b 6167 6572  summary_packager
-00000910: 7328 293a 0d0a 2020 2020 2020 2020 2222  s():..        ""
-00000920: 2220 5061 636b 6167 6572 7320 746f 2068  " Packagers to h
-00000930: 6f6c 6420 7375 6d6d 6172 7920 6f66 2065  old summary of e
-00000940: 6e76 6972 6f6e 6d65 6e74 2e20 2222 220d  nvironment. """.
-00000950: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00000960: 5b0d 0a20 2020 2020 2020 2020 2020 2050  [..            P
-00000970: 6163 6b61 6765 7228 6e61 6d65 3d22 4d61  ackager(name="Ma
-00000980: 6e64 6572 6122 2c20 6769 7468 7562 5f6f  ndera", github_o
-00000990: 776e 6572 3d22 4d61 6e64 6572 6122 292c  wner="Mandera"),
-000009a0: 0d0a 2020 2020 2020 2020 2020 2020 5061  ..            Pa
-000009b0: 636b 6167 6572 286e 616d 653d 222e 6769  ckager(name=".gi
-000009c0: 7468 7562 222c 2067 6974 6875 625f 6f77  thub", github_ow
-000009d0: 6e65 723d 224d 616e 6465 7261 4765 6e65  ner="ManderaGene
-000009e0: 7261 6c22 292c 0d0a 2020 2020 2020 2020  ral"),..        
-000009f0: 5d0d 0a0d 0a20 2020 2064 6566 2073 7061  ]....    def spa
-00000a00: 776e 5f63 6869 6c64 7265 6e28 7365 6c66  wn_children(self
-00000a10: 293a 0d0a 2020 2020 2020 2020 2222 2220  ):..        """ 
-00000a20: 3a70 6172 616d 2067 656e 6572 616c 7061  :param generalpa
-00000a30: 636b 6167 6572 2e50 6163 6b61 6765 7220  ckager.Packager 
-00000a40: 7365 6c66 3a20 2222 220d 0a20 2020 2020  self: """..     
-00000a50: 2020 2066 6f72 2070 6163 6b61 6765 7220     for packager 
-00000a60: 696e 2073 656c 662e 6765 745f 6465 7065  in self.get_depe
-00000a70: 6e64 616e 7473 286f 6e6c 795f 6765 6e65  ndants(only_gene
-00000a80: 7261 6c3d 5472 7565 293a 0d0a 2020 2020  ral=True):..    
-00000a90: 2020 2020 2020 2020 6966 2070 6163 6b61          if packa
-00000aa0: 6765 722e 6c6f 6361 6c72 6570 6f2e 6d65  ger.localrepo.me
-00000ab0: 7461 6461 7461 2e65 6e61 626c 6564 3a0d  tadata.enabled:.
-00000ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000ad0: 2070 6163 6b61 6765 722e 7365 745f 7061   packager.set_pa
-00000ae0: 7265 6e74 2870 6172 656e 743d 7365 6c66  rent(parent=self
-00000af0: 290d 0a0d 0a20 2020 2064 6566 2073 7061  )....    def spa
-00000b00: 776e 5f70 6172 656e 7473 2873 656c 6629  wn_parents(self)
-00000b10: 3a0d 0a20 2020 2020 2020 2022 2222 203a  :..        """ :
-00000b20: 7061 7261 6d20 6765 6e65 7261 6c70 6163  param generalpac
-00000b30: 6b61 6765 722e 5061 636b 6167 6572 2073  kager.Packager s
-00000b40: 656c 663a 2022 2222 0d0a 2020 2020 2020  elf: """..      
-00000b50: 2020 666f 7220 7061 636b 6167 6572 2069    for packager i
-00000b60: 6e20 7365 6c66 2e67 6574 5f64 6570 656e  n self.get_depen
-00000b70: 6465 6e63 6965 7328 6f6e 6c79 5f67 656e  dencies(only_gen
-00000b80: 6572 616c 3d54 7275 6529 3a0d 0a20 2020  eral=True):..   
-00000b90: 2020 2020 2020 2020 2069 6620 7061 636b           if pack
-00000ba0: 6167 6572 2e6c 6f63 616c 7265 706f 2e6d  ager.localrepo.m
-00000bb0: 6574 6164 6174 612e 656e 6162 6c65 643a  etadata.enabled:
-00000bc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000bd0: 2020 7365 6c66 2e73 6574 5f70 6172 656e    self.set_paren
-00000be0: 7428 7061 7265 6e74 3d70 6163 6b61 6765  t(parent=package
-00000bf0: 7229 0d0a 0d0a 2020 2020 6465 6620 5f5f  r)....    def __
-00000c00: 7265 7072 5f5f 2873 656c 6629 3a0d 0a20  repr__(self):.. 
-00000c10: 2020 2020 2020 2022 2222 203a 7061 7261         """ :para
-00000c20: 6d20 6765 6e65 7261 6c70 6163 6b61 6765  m generalpackage
-00000c30: 722e 5061 636b 6167 6572 2073 656c 663a  r.Packager self:
-00000c40: 2022 2222 0d0a 2020 2020 2020 2020 696e   """..        in
-00000c50: 666f 203d 205b 7365 6c66 2e74 6172 6765  fo = [self.targe
-00000c60: 7420 6f72 2022 4e6f 2054 6172 6765 7422  t or "No Target"
-00000c70: 5d0d 0a20 2020 2020 2020 2069 6620 7365  ]..        if se
-00000c80: 6c66 2e70 6174 6820 6973 204e 6f6e 653a  lf.path is None:
-00000c90: 0d0a 2020 2020 2020 2020 2020 2020 696e  ..            in
-00000ca0: 666f 2e61 7070 656e 6428 224e 6f20 5061  fo.append("No Pa
-00000cb0: 7468 2229 0d0a 2020 2020 2020 2020 696e  th")..        in
-00000cc0: 666f 203d 2073 7472 2869 6e66 6f29 2e72  fo = str(info).r
-00000cd0: 6570 6c61 6365 2822 2722 2c20 2222 290d  eplace("'", "").
-00000ce0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00000cf0: 6622 3c50 6163 6b61 6765 7220 7b69 6e66  f"<Packager {inf
-00000d00: 6f7d 3a20 7b73 656c 662e 6e61 6d65 7d3e  o}: {self.name}>
-00000d10: 220d 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d  "...............
-00000d20: 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d  ................
-00000d30: 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d  ................
-00000d40: 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d  ................
-00000d50: 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d  ................
-00000d60: 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d  ................
-00000d70: 0a0d 0a0d 0a                             .....
+00000000: 0d0a 6672 6f6d 2067 656e 6572 616c 6c69  ..from generalli
+00000010: 6272 6172 7920 696d 706f 7274 204e 6574  brary import Net
+00000020: 776f 726b 4469 6167 7261 6d2c 2064 6563  workDiagram, dec
+00000030: 6f5f 6361 6368 650d 0a0d 0a66 726f 6d20  o_cache....from 
+00000040: 6765 6e65 7261 6c70 6163 6b61 6765 722e  generalpackager.
+00000050: 6170 692e 7368 6172 6564 2e74 6172 6765  api.shared.targe
+00000060: 7420 696d 706f 7274 205f 5368 6172 6564  t import _Shared
+00000070: 5461 7267 6574 2c20 5f54 4152 4745 5453  Target, _TARGETS
+00000080: 5f4c 4954 4552 414c 0d0a 6672 6f6d 2067  _LITERAL..from g
+00000090: 656e 6572 616c 7061 636b 6167 6572 2e61  eneralpackager.a
+000000a0: 7069 2e73 6861 7265 642e 6669 6c65 732e  pi.shared.files.
+000000b0: 7368 6172 6564 5f66 696c 6573 2069 6d70  shared_files imp
+000000c0: 6f72 7420 5f46 696c 6573 0d0a 6672 6f6d  ort _Files..from
+000000d0: 2067 656e 6572 616c 7061 636b 6167 6572   generalpackager
+000000e0: 2e61 7069 2e73 6861 7265 642e 7061 7468  .api.shared.path
+000000f0: 2069 6d70 6f72 7420 5f53 6861 7265 6450   import _SharedP
+00000100: 6174 680d 0a66 726f 6d20 6765 6e65 7261  ath..from genera
+00000110: 6c70 6163 6b61 6765 722e 6170 692e 7368  lpackager.api.sh
+00000120: 6172 6564 2e6e 616d 6520 696d 706f 7274  ared.name import
+00000130: 205f 5368 6172 6564 4e61 6d65 2c20 5f53   _SharedName, _S
+00000140: 6861 7265 6441 5049 0d0a 6672 6f6d 2067  haredAPI..from g
+00000150: 656e 6572 616c 7061 636b 6167 6572 2e70  eneralpackager.p
+00000160: 6163 6b61 6765 725f 6170 6920 696d 706f  ackager_api impo
+00000170: 7274 205f 5061 636b 6167 6572 4150 4973  rt _PackagerAPIs
+00000180: 0d0a 6672 6f6d 2067 656e 6572 616c 7061  ..from generalpa
+00000190: 636b 6167 6572 2e70 6163 6b61 6765 725f  ckager.packager_
+000001a0: 656e 7669 726f 6e6d 656e 7420 696d 706f  environment impo
+000001b0: 7274 205f 5061 636b 6167 6572 456e 7669  rt _PackagerEnvi
+000001c0: 726f 6e6d 656e 740d 0a66 726f 6d20 6765  ronment..from ge
+000001d0: 6e65 7261 6c70 6163 6b61 6765 722e 7061  neralpackager.pa
+000001e0: 636b 6167 6572 5f66 696c 6573 2069 6d70  ckager_files imp
+000001f0: 6f72 7420 5f50 6163 6b61 6765 7246 696c  ort _PackagerFil
+00000200: 6573 0d0a 6672 6f6d 2067 656e 6572 616c  es..from general
+00000210: 7061 636b 6167 6572 2e70 6163 6b61 6765  packager.package
+00000220: 725f 6769 7468 7562 2069 6d70 6f72 7420  r_github import 
+00000230: 5f50 6163 6b61 6765 7247 6974 4875 620d  _PackagerGitHub.
+00000240: 0a66 726f 6d20 6765 6e65 7261 6c70 6163  .from generalpac
+00000250: 6b61 6765 722e 7061 636b 6167 6572 5f6d  kager.packager_m
+00000260: 6574 6164 6174 6120 696d 706f 7274 205f  etadata import _
+00000270: 5061 636b 6167 6572 4d65 7461 6461 7461  PackagerMetadata
+00000280: 0d0a 6672 6f6d 2067 656e 6572 616c 7061  ..from generalpa
+00000290: 636b 6167 6572 2e70 6163 6b61 6765 725f  ckager.packager_
+000002a0: 7079 7069 2069 6d70 6f72 7420 5f50 6163  pypi import _Pac
+000002b0: 6b61 6765 7250 7970 690d 0a66 726f 6d20  kagerPypi..from 
+000002c0: 6765 6e65 7261 6c70 6163 6b61 6765 722e  generalpackager.
+000002d0: 7061 636b 6167 6572 5f72 656c 6174 696f  packager_relatio
+000002e0: 6e73 2069 6d70 6f72 7420 5f50 6163 6b61  ns import _Packa
+000002f0: 6765 7252 656c 6174 696f 6e73 0d0a 6672  gerRelations..fr
+00000300: 6f6d 2067 656e 6572 616c 7061 636b 6167  om generalpackag
+00000310: 6572 2e70 6163 6b61 6765 725f 776f 726b  er.packager_work
+00000320: 666c 6f77 2069 6d70 6f72 7420 5f50 6163  flow import _Pac
+00000330: 6b61 6765 7257 6f72 6b66 6c6f 770d 0a0d  kagerWorkflow...
+00000340: 0a63 6c61 7373 2050 6163 6b61 6765 7228  .class Packager(
+00000350: 4e65 7477 6f72 6b44 6961 6772 616d 2c0d  NetworkDiagram,.
+00000360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000370: 5f46 696c 6573 2c20 5f53 6861 7265 6441  _Files, _SharedA
+00000380: 5049 2c20 5f53 6861 7265 6454 6172 6765  PI, _SharedTarge
+00000390: 742c 205f 5368 6172 6564 5061 7468 2c0d  t, _SharedPath,.
+000003a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000003b0: 5f50 6163 6b61 6765 7247 6974 4875 622c  _PackagerGitHub,
+000003c0: 205f 5061 636b 6167 6572 4669 6c65 732c   _PackagerFiles,
+000003d0: 205f 5061 636b 6167 6572 4d65 7461 6461   _PackagerMetada
+000003e0: 7461 2c20 5f50 6163 6b61 6765 7250 7970  ta, _PackagerPyp
+000003f0: 692c 205f 5061 636b 6167 6572 576f 726b  i, _PackagerWork
+00000400: 666c 6f77 2c20 5f50 6163 6b61 6765 7252  flow, _PackagerR
+00000410: 656c 6174 696f 6e73 2c20 5f50 6163 6b61  elations, _Packa
+00000420: 6765 7241 5049 732c 205f 5061 636b 6167  gerAPIs, _Packag
+00000430: 6572 456e 7669 726f 6e6d 656e 7429 3a0d  erEnvironment):.
+00000440: 0a20 2020 2022 2222 2055 7365 7320 4150  .    """ Uses AP
+00000450: 4973 2074 6f20 6d61 6e61 6765 2027 6765  Is to manage 'ge
+00000460: 6e65 7261 6c27 2070 6163 6b61 6765 2e0d  neral' package..
+00000470: 0a20 2020 2020 2020 2043 6f6e 7461 696e  .        Contain
+00000480: 7320 6d65 7468 6f64 7320 7468 6174 2072  s methods that r
+00000490: 6571 7569 7265 206d 6f72 6520 7468 616e  equire more than
+000004a0: 206f 6e65 2041 5049 2061 7320 7765 6c6c   one API as well
+000004b0: 2061 7320 6d65 7468 6f64 7320 7370 6563   as methods spec
+000004c0: 6966 6963 2066 6f72 204d 616e 6465 7261  ific for Mandera
+000004d0: 4765 6e65 7261 6c2e 2022 2222 0d0a 0d0a  General. """....
+000004e0: 2020 2020 6175 7468 6f72 203d 2027 5269      author = 'Ri
+000004f0: 636b 6172 6420 224d 616e 6465 7261 2220  ckard "Mandera" 
+00000500: 4162 7261 6861 6d27 0d0a 2020 2020 656d  Abraham'..    em
+00000510: 6169 6c20 3d20 2272 6963 6b61 7264 2e61  ail = "rickard.a
+00000520: 6272 6168 616d 4067 6d61 696c 2e63 6f6d  braham@gmail.com
+00000530: 220d 0a20 2020 206c 6963 656e 7365 203d  "..    license =
+00000540: 2022 6d69 7422 0d0a 2020 2020 7079 7468   "mit"..    pyth
+00000550: 6f6e 203d 2022 332e 3822 2c20 2233 2e39  on = "3.8", "3.9
+00000560: 222c 2022 332e 3130 222c 2022 332e 3131  ", "3.10", "3.11
+00000570: 2220 2023 204f 6e6c 7920 7375 7070 6f72  "  # Only suppor
+00000580: 7473 2062 6173 6963 2064 6566 696e 6974  ts basic definit
+00000590: 696f 6e20 7769 7468 2074 7570 6c65 206f  ion with tuple o
+000005a0: 6620 6d61 6a6f 722e 6d69 6e6f 720d 0a20  f major.minor.. 
+000005b0: 2020 206f 7320 3d20 2277 696e 646f 7773     os = "windows
+000005c0: 222c 2022 7562 756e 7475 2220 2023 202c  ", "ubuntu"  # ,
+000005d0: 2022 6d61 636f 7322 0d0a 0d0a 2020 2020   "macos"....    
+000005e0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+000005f0: 662c 206e 616d 653d 4e6f 6e65 2c20 7061  f, name=None, pa
+00000600: 7468 3d4e 6f6e 652c 2074 6172 6765 743a  th=None, target:
+00000610: 205f 5441 5247 4554 535f 4c49 5445 5241   _TARGETS_LITERA
+00000620: 4c20 3d20 4e6f 6e65 2c20 6769 7468 7562  L = None, github
+00000630: 5f6f 776e 6572 3d4e 6f6e 652c 2070 7970  _owner=None, pyp
+00000640: 695f 6f77 6e65 723d 4e6f 6e65 293a 0d0a  i_owner=None):..
+00000650: 2020 2020 2020 2020 2222 2220 5374 6f72          """ Stor
+00000660: 696e 6720 7061 7273 2061 7320 6973 2e20  ing pars as is. 
+00000670: 4e61 6d65 2061 6e64 2074 6172 6765 7420  Name and target 
+00000680: 6861 7665 2073 6f6d 6520 6375 7374 6f6d  have some custom
+00000690: 2070 726f 7065 7274 6965 732e 2022 2222   properties. """
+000006a0: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+000006b0: 7461 7267 6574 203d 2074 6172 6765 740d  target = target.
+000006c0: 0a20 2020 2020 2020 2073 656c 662e 5f67  .        self._g
+000006d0: 6974 6875 625f 6f77 6e65 7220 3d20 6769  ithub_owner = gi
+000006e0: 7468 7562 5f6f 776e 6572 0d0a 2020 2020  thub_owner..    
+000006f0: 2020 2020 7365 6c66 2e5f 7079 7069 5f6f      self._pypi_o
+00000700: 776e 6572 203d 2070 7970 695f 6f77 6e65  wner = pypi_owne
+00000710: 720d 0a0d 0a20 2020 2040 636c 6173 736d  r....    @classm
+00000720: 6574 686f 640d 0a20 2020 2040 6465 636f  ethod..    @deco
+00000730: 5f63 6163 6865 2829 0d0a 2020 2020 6465  _cache()..    de
+00000740: 6620 7375 6d6d 6172 795f 7061 636b 6167  f summary_packag
+00000750: 6572 7328 636c 7329 3a0d 0a20 2020 2020  ers(cls):..     
+00000760: 2020 2022 2222 2050 6163 6b61 6765 7273     """ Packagers
+00000770: 2074 6f20 686f 6c64 2073 756d 6d61 7279   to hold summary
+00000780: 206f 6620 656e 7669 726f 6e6d 656e 742e   of environment.
+00000790: 2022 2222 0d0a 2020 2020 2020 2020 7265   """..        re
+000007a0: 7475 726e 205b 0d0a 2020 2020 2020 2020  turn [..        
+000007b0: 2020 2020 5061 636b 6167 6572 286e 616d      Packager(nam
+000007c0: 653d 224d 616e 6465 7261 222c 2067 6974  e="Mandera", git
+000007d0: 6875 625f 6f77 6e65 723d 224d 616e 6465  hub_owner="Mande
+000007e0: 7261 2229 2c0d 0a20 2020 2020 2020 2020  ra"),..         
+000007f0: 2020 2050 6163 6b61 6765 7228 6e61 6d65     Packager(name
+00000800: 3d22 2e67 6974 6875 6222 2c20 6769 7468  =".github", gith
+00000810: 7562 5f6f 776e 6572 3d22 4d61 6e64 6572  ub_owner="Mander
+00000820: 6147 656e 6572 616c 2229 2c0d 0a20 2020  aGeneral"),..   
+00000830: 2020 2020 205d 0d0a 0d0a 2020 2020 6465       ]....    de
+00000840: 6620 7370 6177 6e5f 6368 696c 6472 656e  f spawn_children
+00000850: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+00000860: 2022 2222 203a 7061 7261 6d20 6765 6e65   """ :param gene
+00000870: 7261 6c70 6163 6b61 6765 722e 5061 636b  ralpackager.Pack
+00000880: 6167 6572 2073 656c 663a 2022 2222 0d0a  ager self: """..
+00000890: 2020 2020 2020 2020 666f 7220 7061 636b          for pack
+000008a0: 6167 6572 2069 6e20 7365 6c66 2e67 6574  ager in self.get
+000008b0: 5f64 6570 656e 6461 6e74 7328 6f6e 6c79  _dependants(only
+000008c0: 5f67 656e 6572 616c 3d54 7275 6529 3a0d  _general=True):.
+000008d0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000008e0: 7061 636b 6167 6572 2e6c 6f63 616c 7265  packager.localre
+000008f0: 706f 2e6d 6574 6164 6174 612e 656e 6162  po.metadata.enab
+00000900: 6c65 643a 0d0a 2020 2020 2020 2020 2020  led:..          
+00000910: 2020 2020 2020 7061 636b 6167 6572 2e73        packager.s
+00000920: 6574 5f70 6172 656e 7428 7061 7265 6e74  et_parent(parent
+00000930: 3d73 656c 6629 0d0a 0d0a 2020 2020 6465  =self)....    de
+00000940: 6620 7370 6177 6e5f 7061 7265 6e74 7328  f spawn_parents(
+00000950: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00000960: 2222 2220 3a70 6172 616d 2067 656e 6572  """ :param gener
+00000970: 616c 7061 636b 6167 6572 2e50 6163 6b61  alpackager.Packa
+00000980: 6765 7220 7365 6c66 3a20 2222 220d 0a20  ger self: """.. 
+00000990: 2020 2020 2020 2066 6f72 2070 6163 6b61         for packa
+000009a0: 6765 7220 696e 2073 656c 662e 6765 745f  ger in self.get_
+000009b0: 6465 7065 6e64 656e 6369 6573 286f 6e6c  dependencies(onl
+000009c0: 795f 6765 6e65 7261 6c3d 5472 7565 293a  y_general=True):
+000009d0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+000009e0: 2070 6163 6b61 6765 722e 6c6f 6361 6c72   packager.localr
+000009f0: 6570 6f2e 6d65 7461 6461 7461 2e65 6e61  epo.metadata.ena
+00000a00: 626c 6564 3a0d 0a20 2020 2020 2020 2020  bled:..         
+00000a10: 2020 2020 2020 2073 656c 662e 7365 745f         self.set_
+00000a20: 7061 7265 6e74 2870 6172 656e 743d 7061  parent(parent=pa
+00000a30: 636b 6167 6572 290d 0a0d 0a20 2020 2064  ckager)....    d
+00000a40: 6566 205f 5f72 6570 725f 5f28 7365 6c66  ef __repr__(self
+00000a50: 293a 0d0a 2020 2020 2020 2020 2222 2220  ):..        """ 
+00000a60: 3a70 6172 616d 2067 656e 6572 616c 7061  :param generalpa
+00000a70: 636b 6167 6572 2e50 6163 6b61 6765 7220  ckager.Packager 
+00000a80: 7365 6c66 3a20 2222 220d 0a20 2020 2020  self: """..     
+00000a90: 2020 2069 6e66 6f20 3d20 5b73 656c 662e     info = [self.
+00000aa0: 7461 7267 6574 206f 7220 224e 6f20 5461  target or "No Ta
+00000ab0: 7267 6574 225d 0d0a 2020 2020 2020 2020  rget"]..        
+00000ac0: 696e 666f 203d 2073 7472 2869 6e66 6f29  info = str(info)
+00000ad0: 2e72 6570 6c61 6365 2822 2722 2c20 2222  .replace("'", ""
+00000ae0: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00000af0: 6e20 6622 3c50 6163 6b61 6765 7220 7b69  n f"<Packager {i
+00000b00: 6e66 6f7d 3a20 7b73 656c 662e 6e61 6d65  nfo}: {self.name
+00000b10: 7d3e 220d 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d  }>".............
+00000b20: 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d  ................
+00000b30: 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d  ................
+00000b40: 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d  ................
+00000b50: 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d  ................
+00000b60: 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d  ................
+00000b70: 0a0d 0a0d 0a0d 0a                        .......
```

### Comparing `generalpackager-0.5.7/generalpackager/packager_api.py` & `generalpackager-0.5.8/generalpackager/packager_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from generallibrary import deco_cache, Log
+from generallibrary import deco_cache
+from generalpackager.api.localrepo.top.target_helper import localrepo
 
-from generalpackager.api.github import GitHub
+from generalpackager.api.package_hosts.github import GitHub
 from generalpackager.api.localmodule import LocalModule
 from generalpackager.api.localrepo.base.localrepo import LocalRepo
-from generalpackager.api.pypi import PyPI
+from generalpackager.api.package_hosts.pypi import PyPI
 
 
 class _PackagerAPIs:
     LocalRepo = LocalRepo
     LocalModule = LocalModule
     GitHub = GitHub
     PyPI = PyPI
@@ -35,14 +36,15 @@
             if error:
                 raise self.API_NOT_AVAILABLE_ERROR(f"API '{api_name}' not available.")
             else:
                 return False
         else:
             return True
 
+    # Todo: Check that every API has create an *_available method
     def localrepo_available(self, error=False):
         """ :param generalpackager.Packager self: """
         return self._available(
             api_name="LocalRepo", error=error)
 
     def github_available(self, error=False):
         """ :param generalpackager.Packager self: """
@@ -68,17 +70,15 @@
 
     @property
     @deco_cache()
     def localrepo(self):
         """ :param generalpackager.Packager self:
             :rtype: generalpackager.LocalRepo_Python or generalpackager.LocalRepo_Node """
         self.localrepo_available(error=True)
-        localrepo = LocalRepo(name=self.name, path=self.path).targetted(target=self._target)
-        Log().debug(f"Packager {self.name} got localrepo with target {localrepo.target}")
-        return localrepo
+        return localrepo(name=self.name, path=self.path, target=self.target)
 
     @property
     @deco_cache()
     def github(self):
         """ :param generalpackager.Packager self: """
         self.github_available(error=True)
         return GitHub(name=self.name, owner=self._github_owner)
```

### Comparing `generalpackager-0.5.7/generalpackager/packager_environment.py` & `generalpackager-0.5.8/generalpackager/packager_environment.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,35 +12,44 @@
             - Clone repos
             - Editable repo installs in venv
 
             :param generalpackager.Packager or any cls: """
         path = Path(path=path)
         path.open_folder()
 
+        if python_version is None:
+            python_version = cls.python[-1]
+
         # This could be a general Path method
         if not path.empty():
             if input("Warning: Folder isn't empty, clear it? ").lower() != "y":
                 return
             path.delete_folder_content()
         elif input("Proceed with creating a new clean environment in this folder? ").lower() != "y":
             return
 
         Log("root").configure_stream()
 
-        repo_path = path / "repos"
-        venv = Venv(path / "venvs")
+        repos_path = path / "repos"
+        venvs_path = path / "venvs"
+        venv_path = venvs_path / f"python{python_version.replace('.', '')}"
+
+        node_modules_string = cls.localrepo._cls_target_classes[cls.Targets.node].NODE_MODULES
+        (path / node_modules_string).create_folder()
+
+        venv = Venv(path=venv_path)
         venv.create_venv(ver=python_version)
         venv.upgrade()
         venv.activate()
 
         for packager in cls.packagers_from_packages():  # This will get all packages
-            packager.github.download(path=repo_path)
+            packager.github.download(path=repos_path)
 
         for packager in cls.get_ordered_packagers():  # This will only get python packages
-            new_packager = cls(name=packager.name, path=repo_path / packager.name)
-            new_packager.localrepo.pip_install_editable()
+            new_packager = cls(name=packager.name, path=repos_path / packager.name)
+            new_packager.localrepo.install(editable=True)
```

### Comparing `generalpackager-0.5.7/generalpackager/packager_files.py` & `generalpackager-0.5.8/generalpackager/packager_relations.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,110 +1,90 @@
 
-from generalfile import Path
-from generallibrary import deco_cache, Timer
+from generallibrary import deco_cache, Log, flatten, remove_duplicates
 
+from generalpackager.api.shared.target import Packages
 
-class _PackagerFiles:
-    @classmethod
-    def create_blank_locally_python(cls, path, install=True):
-        """ Create a new general package locally only.
-            Todo: Fix create_blank, it overwrites current projects pip install.
-
-            :param generalpackager.Packager or Any cls:
-            :param Path or str path:
-            :param install: Whether to pip install. """
-        path = Path(path)
-        assert path.empty()
-        packager = cls(name=path.name(), path=path, target=cls.Targets.python)
-
-        packager.localrepo.metadata.write_config()
-        packager.generate_localfiles()
-
-        if install:
-            packager.localrepo.pip_install_editable()
-        # new_self = packager.get_new_packager()  # Reset caches to get updated files
-        # new_self.generate_localfiles()
-        return packager
-
-    @deco_cache()
-    def _compare_local(self, platform, aesthetic):
-        """ :param generalpackager.Packager self: """
-        def filt(path):
-            """ Filter to return True for files we want to compare. """
-            if path.match(*self.git_exclude_lines):
-                return False
-            if aesthetic is not None:
-                file = self.get_file_from_path(path=path)
-                if file is None:
-                    return True  # Probably a python file
-                return file.aesthetic is aesthetic
-            return True
-
-        unpack_target = Path.get_cache_dir() / "Python"
-        package_path = platform.download(path=unpack_target, overwrite=True)
-        return self.path.get_differing_files(target=package_path, filt=filt)
-
-    def compare_local_to_github(self, aesthetic=None):
-        """ Get a list of changed files compared to remote with optional aesthetic files.
 
-            :param generalpackager.Packager self:
-            :param aesthetic: """
-        return self._compare_local(platform=self.github, aesthetic=aesthetic)
+class _PackagerRelations:
+    Packages = Packages
 
-    def compare_local_to_pypi(self, aesthetic=None):
-        """ Get a list of changed files compared to pypi with optional aesthetic files.
+    @classmethod
+    def packagers_from_packages(cls):
+        """ Get all packagers defined in Packages even if they don't exist.
+            Paths are set to working_dir / name.
+
+            :param generalpackager.Packager or any cls: """
+        packagers = []
+        for target, names in cls.Packages.field_dict_defaults().items():
+            for name in names:
+                packager = cls(name=name, path=name, target=target)
+                packagers.append(packager)
+        return packagers
+
+    def get_dependencies(self, only_general=False):
+        """ Get a list of dependencies as Packagers.
+            Combines localmodules dependencies with localrepos install_requires.
+            Optionally only return general packages.
 
             :param generalpackager.Packager self:
-            :param aesthetic: """
-        return self._compare_local(platform=self.pypi, aesthetic=aesthetic)
-
-    def _error_on_change(self, files):
-        """ :param generalpackager.Packager self: """
-        file_paths = {file.path for file in files}
-        changed_files = {path.absolute() for path in self.localrepo.changed_files()}
-
-        changed_generated_files = file_paths.intersection(changed_files)
-        if changed_generated_files:
-            raise EnvironmentError(f"Files changed: {changed_generated_files}")
-
-    def generate_localfiles(self, include_aesthetic=True, print_out=False, error_on_change=False):
-        """ Generate all local files.
-            Returns True if any file is changed.
-
-            :param generalpackager.Packager self: """
-        with Timer(print_out=print_out):
-            # Not in files because it writes with json not text, it's also a bit unique
-            self.localrepo.metadata.name = self.name
-            self.localrepo.metadata.write_config()
-
-            files = [file for file in self.get_files() if include_aesthetic or not file.aesthetic]
-
-            for file in files:
-                file.generate()
-
-        if error_on_change and "[CI SKIP]" not in self.localrepo.commit_message():
-            self._error_on_change(files=files)
-
-
-
-
-
-
-
-
+            :param bool only_general: Whether to only return general packages. """
 
+        names = {localmodule.name for localmodule in self.localmodule.get_dependencies()}
 
+        if self.target == self.Targets.python:
+            names.update(self.localrepo.metadata.install_requires)
 
+        return [type(self)(name) for name in names if not only_general or self.name_is_general(name)]
 
+    def get_dependants(self, only_general=False):
+        """ Get a list of dependants as Packagers.
+            Same as localmodules but Packager instead of localmodule.
+            Optionally only return general packages.
 
+            :param generalpackager.Packager self:
+            :param bool only_general: Whether to only return general packages. """
+        packagers = {type(self)(localmodule.name) for localmodule in self.localmodule.get_dependants() if not only_general or self.name_is_general(localmodule.name)}
+        return list(packagers)
 
+    @classmethod
+    @deco_cache()
+    def get_ordered_packagers(cls, include_private=True, include_summary_packagers=False):
+        """ Get a list of enabled ordered packagers from the dependency chain, sorted by name in each lvl.
 
+            :param generalpackager.Packager or Any cls:
+            :param include_private:
+            :param include_summary_packagers:
+            :rtype: list[generalpackager.Packager] """
+        packagers_by_layer = cls().get_ordered(flat=False)
+        sorted_layers = [sorted(layer, key=lambda pkg: pkg.name) for layer in packagers_by_layer]
+        packagers = remove_duplicates(flatten(sorted_layers))
 
+        if not include_private:
+            packagers = [packager for packager in packagers if not packager.localrepo.metadata.private]
 
+        if include_summary_packagers:
+            packagers.extend(cls.summary_packagers())
 
+        Log().debug("Ordered packagers:", packagers)
 
+        return packagers
 
+    def get_owners_package_names(self):
+        """ Return a set of owner's packages with intersecting PyPI and GitHub, ignores enabled flag.
 
+            :param generalpackager.Packager self: """
+        return self.pypi.get_owners_packages().intersection(self.github.get_owners_packages())
 
+    def general_bumped_set(self):
+        """ Yield general packagers that have been bumped.
 
+            :param generalpackager.Packager self: """
+        for packager in self.get_ordered_packagers():
+            if packager.is_bumped():
+                yield packager
 
+    def general_changed_dict(self, aesthetic=None):
+        """ Return a dict of general packagers with changed files comparing to GitHub.
 
+            :param generalpackager.Packager self:
+            :param aesthetic: """
+        return {packager: files for packager in self.get_ordered_packagers() if (files := packager.compare_local_to_github(aesthetic=aesthetic))}
```

### Comparing `generalpackager-0.5.7/generalpackager/packager_github.py` & `generalpackager-0.5.8/generalpackager/packager_github.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,39 +7,40 @@
         """ Sync GitHub with local metadata.
 
             :param generalpackager.Packager self: """
         assert self.github.set_website(self.pypi.url).ok
         assert self.github.set_description(self.localrepo.metadata.description).ok
         assert self.github.set_topics(*self.get_topics()).ok
 
-    def push(self, tag=None):
+    def push(self, version=None):
         """ :param generalpackager.Packager self: """
-        if tag:
-            tag = f"v{self.localrepo.metadata.version}"
-        self.localrepo.push(url=self.github.ssh_url, tag=tag)
+        if version is True:
+            version = self.localrepo.metadata.version
 
-    def commit_and_push(self, message=None, tag=None):
+        version = self.GitHub.format_version(version=version)
+        self.localrepo.push(url=self.github.ssh_url, tag=version)
+
+    def commit_and_push(self, message=None, version=None):
         """ Commit and push this local repo to GitHub.
             Return short sha1 of pushed commit.
 
             :param generalpackager.Packager self: """
         # Bad hard-coded quick fix
-        if "Sync" in message and tag:
+        if "Sync" in message and version:
             message = message.replace("Sync", "Publish")
 
         if self.localrepo.commit(message=message):
-            self.push(tag=tag)
+            self.push(version=version)
 
     def create_github_repo(self):
         """ :param generalpackager.Packager self: """
         Terminal("gh", "repo", "create", f"{self.github.owner}/{self.name}")
 
     def create_master_branch(self):
         """ :param generalpackager.Packager self: """
-        # HERE **
         # repo = self.localrepo.repo
         # Create remote somehow first
         # print(repo.remote().push("head"))
 
     # Todo: Setup env vars for project.
```

### Comparing `generalpackager-0.5.7/generalpackager/packager_metadata.py` & `generalpackager-0.5.8/generalpackager/packager_metadata.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from generallibrary import deco_cache
+from generalpackager.api.localrepo.base.metadata import _Metadata
 
 
 class _PackagerMetadata:
     def get_topics(self):
         """ Get a complete list of topics by using package specific as well as hardcoded magic values.
 
             :param generalpackager.Packager self: """
@@ -40,23 +42,20 @@
         version = self.pypi.get_version()
         if version is None:
             return True
         else:
             return self.localrepo.metadata.version > version
 
     @property
+    @deco_cache()
     def target(self):
         """ :param generalpackager.Packager self: """
-        if self._target is not Ellipsis:
+        if self._target is not None:
             return self._target
-        else:
-            if self.localrepo.metadata_exists():
-                return self.localrepo.metadata.target
-            else:
-                return None
+        return _Metadata(path=self.metadata_file.path).target
 
     _lib = {
         "planning": "Development Status :: 1 - Planning",
         "pre-alpha": "Development Status :: 2 - Pre-Alpha",
         "alpha": "Development Status :: 3 - Alpha",
         "beta": "Development Status :: 4 - Beta",
         "production/Stable": "Development Status :: 5 - Production/Stable",
```

### Comparing `generalpackager-0.5.7/generalpackager/packager_workflow.py` & `generalpackager-0.5.8/generalpackager/packager_workflow.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,68 +1,75 @@
 
 from generalfile import Path
-from generallibrary import EnvVar, Log, Terminal
-
+from generallibrary import EnvVar, Log, Terminal, classproperty, deco_cache
 
 
 def workflow(func):
     def _wrapper(self):
         Log().debug("Working dir:", Path().absolute())
         Terminal.capture_output = False
         result = func(self)
         Terminal.capture_output = True
         return result
     return _wrapper
 
 
 class _PackagerWorkflow:
+    @deco_cache()
+    def workflow_packagers(cls):
+        """ :param generalpackager.Packager cls: """
+        return cls.get_ordered_packagers(include_private=False, include_summary_packagers=False)
+
     def run_ordered_methods(self, *funcs):
         """ :param generalpackager.Packager self: """
-        order = self.get_ordered_packagers()
         for func in funcs:
-            for packager in order:
+            for packager in self.workflow_packagers():
                 func(packager)
 
     @workflow
     def workflow_unittest(self):
         """ :param generalpackager.Packager self: """
+        Log("root").configure_stream()
+
         self.run_ordered_methods(
             lambda packager: packager.generate_localfiles(include_aesthetic=False),
-            lambda packager: packager.localrepo.unittest(),
+            lambda packager: packager.localrepo.run_tests(),
         )
 
     @workflow
     def workflow_sync(self):
         """ Runs in workflow once Packagers have created each LocalRepo from the latest master commit.
             It can generate new workflow, compare, and then stop workflow after commiting and pushing.
 
             :param generalpackager.Packager self: """
+        Log("root").configure_stream()
+
         trigger_repo = str(EnvVar('GITHUB_REPOSITORY')).split('/')[1]
         msg1 = f"[CI AUTO] For commit sha reference"
         msg2 = f"[CI AUTO] Sync triggered by {trigger_repo}"
 
         any_bumped = any(self.general_bumped_set())
 
         self.run_ordered_methods(
             lambda packager: packager.if_publish_bump(any_bumped=any_bumped),
             lambda packager: packager.generate_localfiles(include_aesthetic=False),
-            lambda packager: packager.localrepo.unittest(),  # Will set coverage percentage
+            lambda packager: packager.localrepo.run_tests(),  # Will set coverage percentage
             lambda packager, msg=msg1: packager.localrepo.commit(message=msg),  # Will update commit_sha
             lambda packager: packager.generate_localfiles(include_aesthetic=True),  # With coverage number and commit_sha
-            lambda packager, msg=msg2: packager.commit_and_push(message=msg, tag=packager.is_bumped()),
+            lambda packager, msg=msg2: packager.commit_and_push(message=msg, version=packager.is_bumped()),
             lambda packager: packager.if_publish_upload(),
             lambda packager: packager.sync_github_metadata(),
         )
 
         for summary_packager in self.summary_packagers():
             summary_packager.upload_package_summary(msg=msg1)
 
     def upload_package_summary(self, msg):
         """ :param generalpackager.Packager self: """
-        self.org_readme_file.generate()
+        assert self.org_readme_file.generate()
         self.commit_and_push(message=msg)
 
     def if_publish_bump(self, any_bumped):
         """ Bump if updated and any other Packager is bumped.
 
             :param generalpackager.Packager self: """
         if any_bumped and not self.is_bumped() and self.compare_local_to_pypi(aesthetic=False):
@@ -71,15 +78,15 @@
     def if_publish_upload(self):
         """ Only does anything if bumped.
             Upload to PyPI unless private.
             Upload exe if exetarget.py exists.
 
             :param generalpackager.Packager self: """
         if self.is_bumped() and not self.localrepo.metadata.private:
-            self.localrepo.upload()
+            self.localrepo.publish()
 
         # if self.localrepo.get_exetarget_path().exists():
         #     self.localrepo.generate_exe()
         #     MainframeClient().upload_exe(exe_path=self.localrepo.get_exeproduct_path(), name=self.name, version=self.localrepo.metadata.version)
```

### Comparing `generalpackager-0.5.7/generalpackager/test/test_github.py` & `generalpackager-0.5.8/generalpackager/test/test_github.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from requests import Response
-
-from generalpackager.api.github import GitHub
-
 import unittest
 
+from generalpackager.api.package_hosts.github import GitHub
+
 
 class TestGitHub(unittest.TestCase):
     def test_exists(self):
         self.assertEqual(True, GitHub("generalpackager").exists())
 
     def test_get_owners_packages(self):
         github = GitHub()
@@ -31,13 +29,13 @@
     def test_get_description(self):
         github = GitHub("generalpackager")
         description = github.get_description()
         self.assertEqual(True, len(description) > 5)
         self.assertEqual(True, github.set_description(description).ok)
 
     def test_commands(self):
-        self.assertIn("generalpackager", GitHub().git_clone_command)
+        self.assertIn("generalpackager", GitHub().git_clone_command())
         self.assertIn("generalpackager", GitHub().pip_install_command)
 
     def test_request_kwargs(self):
         self.assertIn("headers", GitHub().request_kwargs())
```

### Comparing `generalpackager-0.5.7/generalpackager/test/test_local_module.py` & `generalpackager-0.5.8/generalpackager/test/test_local_module.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from generallibrary import Log
+import unittest
 
 from generalpackager.api.localmodule import LocalModule
 
-import unittest
-
 
 class TestLocalModule(unittest.TestCase):
     def test_exists(self):
         self.assertEqual(True, LocalModule("generalpackager").exists())
         self.assertEqual(False, LocalModule("doesntexist").exists())
 
     def test_module(self):
```

### Comparing `generalpackager-0.5.7/generalpackager/test/test_local_repo.py` & `generalpackager-0.5.8/generalpackager/test/test_local_repo.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 from generalfile import Path
+from generalfile.test.test_path import PathTest
 from generallibrary import Ver
 from generalpackager.api.localrepo.base.localrepo import LocalRepo
 from generalpackager.api.localrepo.python.localrepo_python import LocalRepo_Python
-from generalfile.test.test_path import PathTest
+from generalpackager.api.localrepo.top.target_helper import localrepo
 
 
 class TestLocalRepo(PathTest):
     def test_metadata_exists(self):
-        self.assertEqual(True, LocalRepo().metadata_exists())
-        self.assertEqual(False, LocalRepo("doesntexist").metadata_exists())
+        self.assertEqual(True, localrepo().metadata_exists())
+        self.assertEqual(False, localrepo("doesntexist").metadata_exists())
 
     def test_load_metadata(self):
-        self.assertEqual(True, LocalRepo().metadata.enabled)
-        self.assertEqual("generalpackager", LocalRepo().name)
-        self.assertIsInstance(LocalRepo().metadata.version, Ver)
-        self.assertIsInstance(LocalRepo().metadata.description, str)
-        self.assertIsInstance(LocalRepo().metadata.topics, list)
-        self.assertIsInstance(LocalRepo().metadata.manifest, list)
+        self.assertEqual(True, localrepo().metadata.enabled)
+        self.assertEqual("generalpackager", localrepo().name)
+        self.assertIsInstance(localrepo().metadata.version, Ver)
+        self.assertIsInstance(localrepo().metadata.description, str)
+        self.assertIsInstance(localrepo().metadata.topics, list)
+        self.assertIsInstance(localrepo().metadata.manifest, list)
 
-        self.assertIsInstance(LocalRepo().targetted().metadata.install_requires, list)
-        self.assertIsInstance(LocalRepo().targetted().metadata.extras_require, dict)
+        self.assertIsInstance(localrepo().metadata.install_requires, list)
+        self.assertIsInstance(localrepo().metadata.extras_require, dict)
 
     def test_exists(self):
-        self.assertEqual(True, LocalRepo().exists())
-        self.assertEqual(True, LocalRepo.repo_exists(LocalRepo().path))
+        self.assertEqual(True, localrepo().exists())
+        self.assertEqual(True, LocalRepo.repo_exists(localrepo().path))
 
-        self.assertEqual(False, LocalRepo("doesntexist").exists())
+        self.assertEqual(False, localrepo("doesntexist").exists())
 
     def test_get_test_paths(self):
-        self.assertLess(2, len(list(LocalRepo().get_test_paths())))
-        self.assertIn(LocalRepo().get_test_path() / "test_local_repo.py", LocalRepo().get_test_paths())
+        self.assertLess(2, len(list(localrepo().get_test_paths())))
+        self.assertIn(localrepo().get_test_path() / "test_local_repo.py", localrepo().get_test_paths())
 
     def test_get_package_paths(self):
-        package_paths = list(LocalRepo().get_package_paths_gen())
-        self.assertIn(LocalRepo().get_test_path(), package_paths)
-        self.assertIn(LocalRepo().path / LocalRepo().name, package_paths)
-        self.assertNotIn(LocalRepo().path, package_paths)
+        package_paths = list(localrepo().get_package_paths_gen())
+        self.assertIn(localrepo().get_test_path(), package_paths)
+        self.assertIn(localrepo().path / localrepo().name, package_paths)
+        self.assertNotIn(localrepo().path, package_paths)
 
     def test_get_changed_files(self):
         local_repo = LocalRepo_Python()
         version = local_repo.metadata.version
 
         local_repo.bump_version()
         self.assertNotEqual(local_repo.metadata.version, version)
@@ -49,15 +50,15 @@
         self.assertEqual(local_repo.metadata.version, version)
 
     def test_wrong_localrepo_for_target(self):
         local_repo = LocalRepo()
         self.assertRaises(AssertionError, local_repo.bump_version)
 
     def test_targets(self):
-        self.assertEqual(LocalRepo().metadata.target, LocalRepo.Targets.python)
+        self.assertEqual(localrepo().metadata.target, LocalRepo.Targets.python)
 
     def test_format_file_function(self):
         Path("foo").text.write(
             "def camelCase():\n"
             '    """ '
             '        Bad docstrings\n'
             '    """'
@@ -95,35 +96,34 @@
         self.assertIn("generalpackager", LocalRepo().get_setup_path())
         self.assertIn("generalpackager", LocalRepo().get_manifest_path())
         self.assertIn("generalpackager", LocalRepo().get_license_path())
         self.assertIn("generalpackager", LocalRepo().get_workflow_path())
         self.assertIn("generalpackager", LocalRepo().get_test_path())
         self.assertIn("generalpackager", LocalRepo().get_test_template_path())
         self.assertIn("generalpackager", LocalRepo().get_init_path())
-        self.assertIn("generalpackager", LocalRepo().get_randomtesting_path())
         self.assertIn("generalpackager", LocalRepo().get_generate_path())
         self.assertIn("generalpackager", LocalRepo().get_exetarget_path())
         self.assertIn("generalpackager", LocalRepo().get_exeproduct_path())
         self.assertIn("generalpackager", LocalRepo().get_git_ignore_path())
         self.assertIn("generalpackager", LocalRepo().get_npm_ignore_path())
         self.assertIn("generalpackager", LocalRepo().get_index_js_path())
         self.assertIn("generalpackager", LocalRepo().get_test_js_path())
         self.assertIn("generalpackager", LocalRepo().get_package_json_path())
 
     def test_is_target(self):
-        self.assertEqual(True, LocalRepo().is_python())
-        self.assertEqual(False, LocalRepo().is_exe())
-        self.assertEqual(False, LocalRepo().is_node())
-        self.assertEqual(False, LocalRepo().is_django())
+        self.assertEqual(True, localrepo().is_python())
+        self.assertEqual(False, localrepo().is_exe())
+        self.assertEqual(False, localrepo().is_node())
+        self.assertEqual(False, localrepo().is_django())
 
     def test_repo_init(self):
-        localrepo = LocalRepo(path="hi")
-        self.assertIs(False, localrepo.exists())
-        localrepo.init()
-        self.assertIs(True, localrepo.exists())
+        repo = localrepo(path="hi")
+        self.assertIs(False, repo.exists())
+        repo.init()
+        self.assertIs(True, repo.exists())
```

### Comparing `generalpackager-0.5.7/generalpackager/test/test_packager.py` & `generalpackager-0.5.8/generalpackager/test/test_packager.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.7/generalpackager/test/test_packager_api.py` & `generalpackager-0.5.8/generalpackager/test/test_packager_api.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.7/generalpackager/test/test_packager_files.py` & `generalpackager-0.5.8/generalpackager/test/test_packager_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,30 +64,25 @@
         self.assertIn("Packager", text)
 
     def test_generate_init(self):
         packager = Packager()
         text = str(packager.init_file._generate())
         self.assertEqual(True, len(text) > 2)
 
-    def test_generate_randomtesting(self):
-        packager = Packager()
-        text = str(packager.randomtesting_file._generate())
-        self.assertIn("generalpackager", text)
-
     def test_generate_test_python(self):
         packager = Packager()
         text = str(packager.test_template_file._generate())
         self.assertIn("unittest", text)
 
     def test_all_files_by_relative_path(self):
         self.assertIn(Path("README.md"), Packager().get_files_by_relative_path())
         self.assertIn(Path("setup.py"), Packager().get_files_by_relative_path())
 
     def test_create_blank_locally_python(self):
-        Packager.create_blank_locally_python("newblank", install=False)
+        Packager("newblank").create_blank_locally(install=False)
         self.assertEqual(True, Path("newblank/README.md").exists())
         self.assertEqual(True, Path("newblank/newblank").exists())
 
     def test_file_by_relative_path(self):
         self.assertIs(Packager().readme_file, Packager().get_file_from_path("README.md"))
         self.assertIs(None, Packager().get_file_from_path("doesntexist"))
 
@@ -95,11 +90,11 @@
         self.assertIs(Packager(), Packager().org_readme_file.packager)
 
     def test_run_ordered_methods(self):
         x = []
         def a(_): x.append(1)
         def b(_): x.append(2)
         Packager().run_ordered_methods(a, b)
-        length = len(Packager().get_all())
+        length = len(Packager().workflow_packagers())
         self.assertEqual([1] * length + [2] * length, x)
```

### Comparing `generalpackager-0.5.7/generalpackager/test/test_packager_metadata.py` & `generalpackager-0.5.8/generalpackager/test/test_packager_metadata.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 
-from generalpackager import Packager
-
 import unittest
 
+from generalpackager import Packager
+
 
 class TestPackager(unittest.TestCase):
     def test_get_topics(self):
         self.assertIn("windows", Packager().get_topics())
 
     def test_get_classifiers(self):
         self.assertIn("Operating System :: Microsoft :: Windows", Packager().get_classifiers())
```

### Comparing `generalpackager-0.5.7/generalpackager/test/test_packager_node.py` & `generalpackager-0.5.8/generalpackager/test/test_packager_node.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.7/generalpackager/test/test_packager_relations.py` & `generalpackager-0.5.8/generalpackager/test/test_packager_relations.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from generallibrary import Log
+import unittest
 
 from generalpackager import Packager
 
-import unittest
-
 
 class TestPackager(unittest.TestCase):
     def test_get_ordered_packagers(self):
         self.assertLess(3, len(Packager().get_ordered_packagers()))
 
     def test_get_owners_package_names(self):
         self.assertLess(4, len(Packager().get_owners_package_names()))
```

### Comparing `generalpackager-0.5.7/generalpackager/test/test_pypi.py` & `generalpackager-0.5.8/generalpackager/test/test_pypi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 
-from generalpackager.api.pypi import PyPI
 from generalfile.test.test_path import PathTest
 from generallibrary import Date
+from generalpackager.api.package_hosts.pypi import PyPI
 
 
 class TestPyPI(PathTest):
     def test_exists(self):
         self.assertEqual(True, PyPI("generalpackager").exists())
         self.assertEqual(False, PyPI("random-package_that,cant.exist").exists())
 
     def test_get_tarball_url(self):
         pypi = PyPI("generalpackager")
-        self.assertEqual(True, pypi.name in pypi.get_tarball_url())
-        self.assertEqual(True, pypi.name in pypi.get_tarball_url(version="1.0.0"))
+        self.assertEqual(True, pypi.name in pypi._get_tarball_url())
+        self.assertEqual(True, pypi.name in pypi._get_tarball_url(version="1.0.0"))
 
     def test_download(self):
         path = PyPI("generalpackager").download(path="repo")
-        self.assertEqual(True, "generalpackager" in path.get_child())
+        self.assertTrue(path.exists())
 
         with self.assertRaises(AttributeError):
             PyPI("generalpackager").download(path="repo", version="0.0.111")
 
         path = PyPI("generalpackager").download(path="repo", version="0.0.11", overwrite=True)
-        self.assertEqual(2, len(path.get_parent().get_children()))
+        self.assertTrue(path.exists())
 
     def test_get_owners_packages(self):
         github = PyPI()
         self.assertEqual(set(), {"generallibrary", "generalfile", "generalvector", "generalpackager"}.difference(github.get_owners_packages()))
 
     def test_get_version(self):
         self.assertEqual(True, PyPI("generalpackager").get_version() > "0.2.0")
```

### Comparing `generalpackager-0.5.7/generalpackager/test/test_shared.py` & `generalpackager-0.5.8/generalpackager/test/test_shared.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.7/generalpackager/test/test_venv.py` & `generalpackager-0.5.8/generalpackager/test/test_venv.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,36 @@
+from generalfile.test.test_path import PathTest
 from generallibrary import Log
-
 from generalpackager.api.venv import Venv
-from generalfile.test.test_path import PathTest
 
-class TestPyPI(PathTest):
+
+class TestVenv(PathTest):
     def test_create_venv(self):
+        prev_venv_path = Venv.get_active_venv_path()
+
         venv = Venv("new_venv")
         self.assertEqual(False, venv.exists())
 
         venv.create_venv()
         self.assertEqual(True, venv.exists())
 
         self.assertEqual(False, venv.active())
         with venv:
             self.assertEqual(True, venv.active())
             self.assertIn(venv.path, venv.list_venv_paths())
         self.assertEqual(False, venv.active())
 
+        self.assertEqual(prev_venv_path, Venv.get_active_venv_path())
         venv.upgrade()
         venv.python_version()
+        self.assertEqual(prev_venv_path, Venv.get_active_venv_path())
+
 
     def test_list_python_versions(self):
-        Log("root").configure_stream()  # HERE ** Would be nice to configure artifact for github actions
+        Log("root").configure_stream()  # Would be nice to configure artifact for github actions https://github.com/ManderaGeneral/generallibrary/issues/25
         self.assertGreaterEqual(len(Venv.list_python_versions()), 1)
```

### Comparing `generalpackager-0.5.7/generalpackager.egg-info/PKG-INFO` & `generalpackager-0.5.8/generalpackager.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generalpackager
-Version: 0.5.7
+Version: 0.5.8
 Summary: Tools to interface GitHub, PyPI, NPM and local modules / repos. Used for generating files to keep projects dry and synced. Tailored for ManderaGeneral for now.
 Home-page: https://github.com/ManderaGeneral/generalpackager
 Author: Rickard "Mandera" Abraham
 Author-email: rickard.abraham@gmail.com
 License: mit
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3.8
@@ -38,21 +38,21 @@
 
 
 <details open>
 <summary><h2>Dependency Diagram for ManderaGeneral</h2></summary>
 
 ```mermaid
 flowchart LR
+2([library]) --> 5([packager])
+2([library]) --> 4([vector])
 3([file]) --> 5([packager])
 0([import]) --> 3([file])
-2([library]) --> 3([file])
-2([library]) --> 4([vector])
-2([library]) --> 5([packager])
 1([tool]) --> 2([library])
 0([import]) --> 2([library])
+2([library]) --> 3([file])
 click 0 "https://github.com/ManderaGeneral/generalimport"
 click 1 "https://github.com/ManderaGeneral/generaltool"
 click 2 "https://github.com/ManderaGeneral/generallibrary"
 click 3 "https://github.com/ManderaGeneral/generalfile"
 click 4 "https://github.com/ManderaGeneral/generalvector"
 click 5 "https://github.com/ManderaGeneral/generalpackager"
 style 5 fill:#482
@@ -66,251 +66,319 @@
 | `pip install`                                                                      | `generalpackager`   |
 |:-----------------------------------------------------------------------------------|:--------------------|
 | <a href='https://pypi.org/project/generallibrary[table]'>generallibrary[table]</a> | ✔️                  |
 | <a href='https://pypi.org/project/generalfile'>generalfile</a>                     | ✔️                  |
 | <a href='https://pypi.org/project/requests'>requests</a>                           | ✔️                  |
 | <a href='https://pypi.org/project/pyinstaller'>pyinstaller</a>                     | ✔️                  |
 | <a href='https://pypi.org/project/coverage'>coverage</a>                           | ✔️                  |
+| <a href='https://pypi.org/project/setuptools'>setuptools</a>                       | ✔️                  |
+| <a href='https://pypi.org/project/wheel'>wheel</a>                                 | ✔️                  |
+| <a href='https://pypi.org/project/twine'>twine</a>                                 | ✔️                  |
 </details>
 
 
 <details open>
 <summary><h2>Information</h2></summary>
 
-| Package                                                              | Ver                                                | Latest Release       | Python                                                                                                                                                                                                                                                 | Platform        | Cover   |
-|:---------------------------------------------------------------------|:---------------------------------------------------|:---------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------------|:--------|
-| [generalpackager](https://github.com/ManderaGeneral/generalpackager) | [0.5.7](https://pypi.org/project/generalpackager/) | 2023-02-02 13:29 CET | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/downloads/release/python-3100/), [3.11](https://www.python.org/downloads/release/python-3110/) | Windows, Ubuntu | 68.9 %  |
+| Package                                                              | Ver                                                | Latest Release        | Python                                                                                                                                                                                                                                                 | Platform        | Cover   |
+|:---------------------------------------------------------------------|:---------------------------------------------------|:----------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------------|:--------|
+| [generalpackager](https://github.com/ManderaGeneral/generalpackager) | [0.5.8](https://pypi.org/project/generalpackager/) | 2023-06-02 23:27 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/downloads/release/python-3100/), [3.11](https://www.python.org/downloads/release/python-3110/) | Windows, Ubuntu | 67.8 %  |
 </details>
 
 
 
 <details>
 <summary><h2>Attributes</h2></summary>
 
 <pre>
 <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/__init__.py#L1'>Module: generalpackager</a>
-├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L11'>Class: GitHub</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L11'>Class: GitHub</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L8'>Class: LocalModule</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L16'>Class: LocalRepo</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L22'>Class: Packager</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L26'>Class: PyPI</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L27'>Method: api_url</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L43'>Method: download</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L39'>Method: exists</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L96'>Method: get_description</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L64'>Method: get_owners_packages</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L83'>Method: get_topics</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L71'>Method: get_website</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L32'>Property: git_clone_command</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L36'>Property: pip_install_command</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L108'>Method: request_kwargs</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L102'>Method: set_description</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L89'>Method: set_topics</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L77'>Method: set_website</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L24'>Property: ssh_url</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L20'>Property: url</a>
-├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L8'>Class: LocalModule</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L11'>Class: GitHub</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L8'>Class: LocalModule</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L16'>Class: LocalRepo</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L22'>Class: Packager</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L26'>Class: PyPI</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L26'>Method: exists</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L67'>Method: get_all_local_modules</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L89'>Method: get_dependants</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L74'>Method: get_dependencies</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L20'>Property: module</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L41'>Property: objInfo</a>
+├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L13'>Class: GitHub</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L13'>Class: GitHub</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L9'>Class: LocalModule</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L17'>Class: LocalRepo</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L17'>Class: Packager</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L27'>Class: PyPI</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L54'>Method: api_url</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L23'>Method: format_version</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L133'>Method: get_description</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L120'>Method: get_topics</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L108'>Method: get_website</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L58'>Method: git_clone_command</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L40'>Method: is_general</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L36'>Method: name_is_general</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L71'>Property: pip_install_command</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L145'>Method: request_kwargs</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L139'>Method: set_description</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L126'>Method: set_topics</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L114'>Method: set_website</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L45'>Property: simple_name</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L51'>Property: ssh_url</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L18'>Method: tag_is_version</a>
+├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L9'>Class: LocalModule</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L13'>Class: GitHub</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L9'>Class: LocalModule</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L17'>Class: LocalRepo</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L17'>Class: Packager</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L27'>Class: PyPI</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L27'>Method: exists</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L68'>Method: get_all_local_modules</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L90'>Method: get_dependants</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L75'>Method: get_dependencies</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L21'>Property: module</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L42'>Property: objInfo</a>
 │  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/#L426'>Property: path</a>
-├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L16'>Class: LocalRepo</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L11'>Class: GitHub</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L8'>Class: LocalModule</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L16'>Class: LocalRepo</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L22'>Class: Packager</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L26'>Class: PyPI</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/targets.py#L4'>Class: Targets</a>
+├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L17'>Class: LocalRepo</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L13'>Class: GitHub</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L9'>Class: LocalModule</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L17'>Class: LocalRepo</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L17'>Class: Packager</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L27'>Class: PyPI</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L8'>Class: Targets</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/decos.py#L4'>Method: changed_files</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/decos.py#L4'>Method: clone</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/decos.py#L4'>Method: commit</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_git.py#L12'>Method: commit_message</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/commit_editmsg.py#L5'>Class: commit_editmsg_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_git.py#L11'>Method: commit_message</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/decos.py#L4'>Method: commit_sha</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_git.py#L72'>Method: commit_sha_short</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L55'>Method: exists</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L114'>Method: format_file</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L92'>Method: get_examples_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L60'>Method: get_exeproduct_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L56'>Method: get_exetarget_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L52'>Method: get_generate_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_git.py#L76'>Method: commit_sha_short</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/examples.py#L5'>Class: examples_folder</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/exeproduct.py#L5'>Class: exeproduct_folder</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/exetarget.py#L5'>Class: exetarget_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L45'>Method: exists</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L104'>Method: format_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/generate.py#L6'>Class: generate_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_git.py#L88'>Method: get_all_versions</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L88'>Method: get_examples_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L56'>Method: get_exeproduct_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L52'>Method: get_exetarget_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L27'>Method: get_file_from_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L11'>Method: get_filenames</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L17'>Method: get_files</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L22'>Method: get_files_by_relative_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L48'>Method: get_generate_path</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L16'>Method: get_git_exclude_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L64'>Method: get_git_ignore_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L72'>Method: get_index_js_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L60'>Method: get_git_ignore_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L68'>Method: get_index_js_path</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L44'>Method: get_init_path</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L28'>Method: get_license_path</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L24'>Method: get_manifest_path</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L12'>Method: get_metadata_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L68'>Method: get_npm_ignore_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L64'>Method: get_npm_ignore_path</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L8'>Method: get_org_readme_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L80'>Method: get_package_json_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L72'>Method: get_package_paths_gen</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L84'>Method: get_pre_commit_hook_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L88'>Method: get_pre_push_hook_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L48'>Method: get_randomtesting_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L76'>Method: get_package_json_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L62'>Method: get_package_paths_gen</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L80'>Method: get_pre_commit_hook_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L84'>Method: get_pre_push_hook_path</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L4'>Method: get_readme_path</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L20'>Method: get_setup_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L76'>Method: get_test_js_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L72'>Method: get_test_js_path</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L36'>Method: get_test_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L66'>Method: get_test_paths</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L56'>Method: get_test_paths</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L40'>Method: get_test_template_path</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_paths.py#L32'>Method: get_workflow_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_git.py#L29'>Method: git_config</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_git.py#L21'>Method: git_missing_credentials</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_git.py#L25'>Method: git_nothing_to_commit</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_git.py#L28'>Method: git_config</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/git_exclude.py#L5'>Class: git_exclude_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_git.py#L20'>Method: git_missing_credentials</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_git.py#L24'>Method: git_nothing_to_commit</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/gitignore.py#L5'>Class: gitignore_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/index_js.py#L6'>Class: index_js_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/decos.py#L4'>Method: init</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_target.py#L18'>Method: is_django</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_target.py#L22'>Method: is_exe</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L41'>Method: is_general</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_target.py#L14'>Method: is_node</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_target.py#L10'>Method: is_python</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L33'>Property: metadata</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L48'>Method: metadata_exists</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L37'>Method: name_is_general</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/init.py#L6'>Class: init_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L28'>Method: is_django</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L32'>Method: is_exe</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L40'>Method: is_general</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L24'>Method: is_node</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L20'>Method: is_python</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/license.py#L6'>Class: license_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/manifest.py#L5'>Class: manifest_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L34'>Property: metadata</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L38'>Method: metadata_exists</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/metadata.py#L5'>Class: metadata_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L36'>Method: name_is_general</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/npm_ignore.py#L5'>Class: npm_ignore_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/org_readme.py#L6'>Class: org_readme_file</a>
+│  │  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/org_readme.py#L18'>Method: get_org_description_markdown</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/package_json.py#L6'>Class: package_json_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/pre_commit_hook.py#L4'>Class: pre_commit_hook_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/pre_push_hook.py#L6'>Class: pre_push_hook_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/decos.py#L4'>Method: push</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L60'>Method: repo_exists</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L46'>Property: simple_name</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L42'>Property: target</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_target.py#L49'>Method: targetted</a>
-├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/node/localrepo_node.py#L6'>Class: LocalRepo_Node</a>
-├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L11'>Class: LocalRepo_Python</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L16'>Method: get_python_exe_path</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L21'>Method: unittest</a>
-├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L22'>Class: Packager</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L11'>Class: GitHub</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L8'>Class: LocalModule</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L16'>Class: LocalRepo</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L22'>Class: Packager</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/other/packages.py#L9'>Class: Packages</a>
-│  │  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/other/packages.py#L34'>Method: all_packages</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L26'>Class: PyPI</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/targets.py#L4'>Class: Targets</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L20'>Method: commit_and_push</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L8'>Class: readme_file</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L125'>Method: get_attributes_markdown</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L17'>Method: get_badges_dict</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L246'>Method: get_contributions_markdown</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L27'>Method: get_description_markdown</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L89'>Method: get_examples_markdown</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L195'>Method: get_footnote_markdown</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L219'>Method: get_information_markdown</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L44'>Method: get_installation_markdown</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L209'>Method: get_mermaid_markdown</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L163'>Method: get_todos</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L169'>Method: get_todos_markdown</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L204'>Method: github_link</a>
+│  │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L137'>Method: github_link_path_line</a>
+│  │  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L189'>Method: set_collapsible</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L50'>Method: repo_exists</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/setup.py#L6'>Class: setup_file</a>
+│  │  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/setup.py#L21'>Method: get_classifiers</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L45'>Property: simple_name</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_target.py#L18'>Method: targetted</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/test.py#L5'>Class: test_folder</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/test_js.py#L6'>Class: test_js_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/test_template.py#L6'>Class: test_template_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/workflow_dev.py#L4'>Class: workflow_dev_file</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/workflow.py#L7'>Class: workflow_file</a>
+│     └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/workflow.py#L15'>Method: codeline</a>
+├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/node/localrepo_node.py#L9'>Class: LocalRepo_Node</a>
+├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L12'>Class: LocalRepo_Python</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L17'>Method: get_python_exe_path</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L57'>Method: set_easy_install_value</a>
+├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L17'>Class: Packager</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L13'>Class: GitHub</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L9'>Class: LocalModule</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L17'>Class: LocalRepo</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L17'>Class: Packager</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L37'>Class: Packages</a>
+│  │  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L62'>Method: all_packages</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L27'>Class: PyPI</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L8'>Class: Targets</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L22'>Method: commit_and_push</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/commit_editmsg.py#L5'>Class: commit_editmsg_file</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L46'>Method: compare_local_to_github</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L53'>Method: compare_local_to_pypi</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L8'>Method: create_blank_locally_python</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L32'>Method: create_github_repo</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L36'>Method: create_master_branch</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L38'>Method: compare_local_to_github</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L45'>Method: compare_local_to_pypi</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L7'>Method: create_blank_locally</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L34'>Method: create_github_repo</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L38'>Method: create_master_branch</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/examples.py#L5'>Class: examples_folder</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/exeproduct.py#L5'>Class: exeproduct_folder</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/exetarget.py#L5'>Class: exetarget_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_relations.py#L77'>Method: general_bumped_set</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_relations.py#L85'>Method: general_changed_dict</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/generate.py#L6'>Class: generate_file</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L69'>Method: generate_localfiles</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_metadata.py#L27'>Method: get_classifiers</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L61'>Method: generate_localfiles</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_metadata.py#L29'>Method: get_classifiers</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_relations.py#L38'>Method: get_dependants</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_relations.py#L23'>Method: get_dependencies</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L29'>Method: get_file_from_path</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L13'>Method: get_filenames</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L19'>Method: get_files</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L24'>Method: get_files_by_relative_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L27'>Method: get_file_from_path</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L11'>Method: get_filenames</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L17'>Method: get_files</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/shared_files.py#L22'>Method: get_files_by_relative_path</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_pypi.py#L8'>Method: get_latest_release</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_relations.py#L49'>Method: get_ordered_packagers</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_relations.py#L71'>Method: get_owners_package_names</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_metadata.py#L4'>Method: get_topics</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_metadata.py#L6'>Method: get_topics</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/git_exclude.py#L5'>Class: git_exclude_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L81'>Property: github</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L47'>Method: github_available</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L64'>Method: if_publish_bump</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L71'>Method: if_publish_upload</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L49'>Method: github_available</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/gitignore.py#L5'>Class: gitignore_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L71'>Method: if_publish_bump</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L78'>Method: if_publish_upload</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/index_js.py#L6'>Class: index_js_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/init.py#L6'>Class: init_file</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_metadata.py#L33'>Method: is_bumped</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_target.py#L18'>Method: is_django</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_target.py#L22'>Method: is_exe</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L41'>Method: is_general</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_target.py#L14'>Method: is_node</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo_target.py#L10'>Method: is_python</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_metadata.py#L35'>Method: is_bumped</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L28'>Method: is_django</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L32'>Method: is_exe</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L40'>Method: is_general</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L24'>Method: is_node</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L20'>Method: is_python</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/license.py#L6'>Class: license_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L88'>Property: localmodule</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L52'>Method: localmodule_available</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L71'>Property: localrepo</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L42'>Method: localrepo_available</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L54'>Method: localmodule_available</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L73'>Property: localrepo</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L44'>Method: localrepo_available</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/manifest.py#L5'>Class: manifest_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/metadata.py#L5'>Class: metadata_file</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L37'>Method: name_is_general</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L36'>Method: name_is_general</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_environment.py#L9'>Method: new_clean_environment</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/npm_ignore.py#L5'>Class: npm_ignore_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/org_readme.py#L6'>Class: org_readme_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/package_json.py#L6'>Class: package_json_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_relations.py#L11'>Method: packagers_from_packages</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/pre_commit_hook.py#L4'>Class: pre_commit_hook_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/pre_push_hook.py#L6'>Class: pre_push_hook_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L14'>Method: push</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L95'>Property: pypi</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L60'>Method: pypi_available</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/randomtesting.py#L6'>Class: randomtesting_file</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L9'>Class: readme_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L62'>Method: pypi_available</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L8'>Class: readme_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_pypi.py#L23'>Method: reserve_name</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L18'>Method: run_ordered_methods</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L22'>Method: run_ordered_methods</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/setup.py#L6'>Class: setup_file</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L46'>Property: simple_name</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L46'>Method: summary_packagers</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L45'>Property: simple_name</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L36'>Method: summary_packagers</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L6'>Method: sync_github_metadata</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_metadata.py#L47'>Property: target</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_metadata.py#L50'>Property: target</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/test.py#L5'>Class: test_folder</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/test_js.py#L6'>Class: test_js_file</a>
 │  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/test_template.py#L6'>Class: test_template_file</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L59'>Method: upload_package_summary</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/workflow.py#L6'>Class: workflow_file</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L8'>Method: workflow_sync</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L8'>Method: workflow_unittest</a>
-└─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L26'>Class: PyPI</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L11'>Class: GitHub</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L8'>Class: LocalModule</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L16'>Class: LocalRepo</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L22'>Class: Packager</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L26'>Class: PyPI</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L47'>Method: download</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L37'>Method: exists</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L70'>Method: get_date</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L59'>Method: get_owners_packages</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L41'>Method: get_tarball_url</a>
-   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L63'>Method: get_version</a>
-   └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L34'>Property: url</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L66'>Method: upload_package_summary</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/workflow_dev.py#L4'>Class: workflow_dev_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/workflow.py#L7'>Class: workflow_file</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L18'>Method: workflow_packagers</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L7'>Method: workflow_sync</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_workflow.py#L7'>Method: workflow_unittest</a>
+├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L27'>Class: PyPI</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L13'>Class: GitHub</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localmodule.py#L9'>Class: LocalModule</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L17'>Class: LocalRepo</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager.py#L17'>Class: Packager</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L27'>Class: PyPI</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L40'>Method: is_general</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L36'>Property: json_endpoint</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L36'>Method: name_is_general</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/name.py#L45'>Property: simple_name</a>
+└─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L9'>Class: Venv</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L69'>Method: active</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L72'>Method: create_venv</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv_cruds.py#L69'>Property: cruds</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L85'>Method: deactivate</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L171'>Method: debug</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L54'>Method: easy_install_path</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L48'>Method: exe_name</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L66'>Method: exists</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L30'>Method: get_active_python</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L18'>Method: get_active_venv</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L24'>Method: get_active_venv_path</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L131'>Method: list_python_versions</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L120'>Method: list_venv_paths</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L52'>Method: python_exe_path</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L56'>Method: python_home_exe_path</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L55'>Method: python_home_path</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L60'>Method: python_path</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L58'>Method: python_sys_executable_path</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L117'>Method: python_version</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L50'>Method: pyvenv_cfg_path</a>
+   ├─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L51'>Method: scripts_path</a>
+   └─ <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/venv.py#L53'>Method: site_packages_path</a>
 </pre>
 </details>
 
 
 <details open>
 <summary><h2>Contributions</h2></summary>
 
-Issue-creation and discussions are most welcome!
-
-Pull requests are currently not wanted, please discuss with me before investing any time
+Issue-creation, discussions and pull requests are most welcome!
 </details>
 
 
 <details>
 <summary><h2>Todo</h2></summary>
 
 | Module                                                                                                                                                      | Message                                                                                                                                                                                                          |
 |:------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L1'>packager_files.py</a>                          | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L10'>Fix create_blank, it overwrites current projects pip install.</a>                                  |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L1'>localrepo_python.py</a> | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L55'>Make sure twine is installed when trying to upload to pypi.</a>             |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L1'>localrepo_python.py</a> | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L56'>Look into private PyPI server where we could also do dry runs for test.</a> |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/metadata_python.py#L1'>metadata_python.py</a>   | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/metadata_python.py#L4'>Dynamic values in DataClass to remove LocalRepos and Metadatas.</a>           |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L1'>localrepo.py</a>                 | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L21'>Search for imports to list dependencies.</a>                                         |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L1'>pypi.py</a>                                          | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L12'>Move download to it's own package.</a>                                                                   |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L1'>pypi.py</a>                                          | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/pypi.py#L66'>Find a faster fetch for latest PyPI version and datetime.</a>                                            |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L1'>readme.py</a>             | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L167'>Sort todos by name to decrease automatic commit changes.</a>                 |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L1'>github.py</a>                                      | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/github.py#L13'>Get and Set GitHub repo private.</a>                                                                   |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/other/packages.py#L1'>packages.py</a>                                | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/other/packages.py#L11'>Generate Python file in generalpackager containing general packages.</a>                           |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L1'>packager_github.py</a>                        | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L43'>Setup env vars for project.</a>                                                                   |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L1'>packager_files.py</a>                          | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L9'>Fix create_blank, it overwrites current projects pip install.</a>                                   |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L1'>packager_github.py</a>                        | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L44'>Setup env vars for project.</a>                                                                   |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L1'>target.py</a>                               | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L39'>Generate Python file in generalpackager containing general packages.</a>                        |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L1'>readme.py</a>             | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L166'>Sort todos by name to decrease automatic commit changes.</a>                 |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L1'>pypi.py</a>                            | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L13'>Move download to it's own package.</a>                                                     |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L1'>pypi.py</a>                            | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L78'>Find a faster fetch for latest PyPI version and datetime.</a>                              |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L1'>github.py</a>                        | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L15'>Get and Set GitHub repo private.</a>                                                     |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L1'>localrepo_python.py</a> | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L77'>Make sure twine is installed when trying to upload to pypi.</a>             |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L1'>localrepo_python.py</a> | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L78'>Look into private PyPI server where we could also do dry runs for test.</a> |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L1'>localrepo.py</a>                 | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L22'>Search for imports to list dependencies.</a>                                         |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L1'>packager_api.py</a>                              | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L43'>Check that every API has create an *_available method</a>                                            |
 </details>
 
 
 <sup>
-Generated 2023-02-02 13:29 CET for commit <a href='https://github.com/ManderaGeneral/generalpackager/commit/master'>master</a>.
+Generated 2023-06-02 23:27 CEST for commit <a href='https://github.com/ManderaGeneral/generalpackager/commit/master'>master</a>.
 </sup>
 </details>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: generalpackager Version: 0.5.7 Summary: Tools to
+Metadata-Version: 2.1 Name: generalpackager Version: 0.5.8 Summary: Tools to
 interface GitHub, PyPI, NPM and local modules / repos. Used for generating
 files to keep projects dry and synced. Tailored for ManderaGeneral for now.
 Home-page: https://github.com/ManderaGeneral/generalpackager Author: Rickard
 "Mandera" Abraham Author-email: rickard.abraham@gmail.com License: mit
 Classifier: Topic :: Software Development :: Build Tools Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
@@ -20,63 +20,65 @@
 ââ Installation_showing_dependencies
 ââ Information
 ââ Attributes
 ââ Contributions
 ââ Todo
 
 ***** Dependency Diagram for ManderaGeneral *****
-```mermaid flowchart LR 3([file]) --> 5([packager]) 0([import]) --> 3([file]) 2
-([library]) --> 3([file]) 2([library]) --> 4([vector]) 2([library]) --> 5(
-[packager]) 1([tool]) --> 2([library]) 0([import]) --> 2([library]) click 0
+```mermaid flowchart LR 2([library]) --> 5([packager]) 2([library]) --> 4(
+[vector]) 3([file]) --> 5([packager]) 0([import]) --> 3([file]) 1([tool]) --> 2
+([library]) 0([import]) --> 2([library]) 2([library]) --> 3([file]) click 0
 "https://github.com/ManderaGeneral/generalimport" click 1 "https://github.com/
 ManderaGeneral/generaltool" click 2 "https://github.com/ManderaGeneral/
 generallibrary" click 3 "https://github.com/ManderaGeneral/generalfile" click 4
 "https://github.com/ManderaGeneral/generalvector" click 5 "https://github.com/
 ManderaGeneral/generalpackager" style 5 fill:#482 ```
 ***** Installation showing dependencies *****
 | `pip install` | `generalpackager` | |:---------------------------------------
 --------------------------------------------|:--------------------| |
 generallibrary[table] | âï¸ | | generalfile | âï¸ | | requests | âï¸ |
-| pyinstaller | âï¸ | | coverage | âï¸ |
+| pyinstaller | âï¸ | | coverage | âï¸ | | setuptools | âï¸ | | wheel
+| âï¸ | | twine | âï¸ |
 ***** Information *****
 | Package | Ver | Latest Release | Python | Platform | Cover | |:--------------
 -------------------------------------------------------|:----------------------
------------------------------|:---------------------|:-------------------------
+-----------------------------|:----------------------|:------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
-----------------------------------------------------------------|:-------------
----|:--------| | [generalpackager](https://github.com/ManderaGeneral/
-generalpackager) | [0.5.7](https://pypi.org/project/generalpackager/) | 2023-
-02-02 13:29 CET | [3.8](https://www.python.org/downloads/release/python-380/),
+-----------------------------------------------------------------|:------------
+----|:--------| | [generalpackager](https://github.com/ManderaGeneral/
+generalpackager) | [0.5.8](https://pypi.org/project/generalpackager/) | 2023-
+06-02 23:27 CEST | [3.8](https://www.python.org/downloads/release/python-380/),
 [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://
 www.python.org/downloads/release/python-3100/), [3.11](https://www.python.org/
-downloads/release/python-3110/) | Windows, Ubuntu | 68.9 % |
+downloads/release/python-3110/) | Windows, Ubuntu | 67.8 % |
 ***** Attributes *****
 Module:_generalpackager
 ââ Class:_GitHub
 â  ââ Class:_GitHub
 â  ââ Class:_LocalModule
 â  ââ Class:_LocalRepo
 â  ââ Class:_Packager
 â  ââ Class:_PyPI
 â  ââ Method:_api_url
-â  ââ Method:_download
-â  ââ Method:_exists
+â  ââ Method:_format_version
 â  ââ Method:_get_description
-â  ââ Method:_get_owners_packages
 â  ââ Method:_get_topics
 â  ââ Method:_get_website
-â  ââ Property:_git_clone_command
+â  ââ Method:_git_clone_command
+â  ââ Method:_is_general
+â  ââ Method:_name_is_general
 â  ââ Property:_pip_install_command
 â  ââ Method:_request_kwargs
 â  ââ Method:_set_description
 â  ââ Method:_set_topics
 â  ââ Method:_set_website
+â  ââ Property:_simple_name
 â  ââ Property:_ssh_url
-â  ââ Property:_url
+â  ââ Method:_tag_is_version
 ââ Class:_LocalModule
 â  ââ Class:_GitHub
 â  ââ Class:_LocalModule
 â  ââ Class:_LocalRepo
 â  ââ Class:_Packager
 â  ââ Class:_PyPI
 â  ââ Method:_exists
@@ -92,79 +94,123 @@
 â  ââ Class:_LocalRepo
 â  ââ Class:_Packager
 â  ââ Class:_PyPI
 â  ââ Class:_Targets
 â  ââ Method:_changed_files
 â  ââ Method:_clone
 â  ââ Method:_commit
+â  ââ Class:_commit_editmsg_file
 â  ââ Method:_commit_message
 â  ââ Method:_commit_sha
 â  ââ Method:_commit_sha_short
+â  ââ Class:_examples_folder
+â  ââ Class:_exeproduct_folder
+â  ââ Class:_exetarget_file
 â  ââ Method:_exists
 â  ââ Method:_format_file
+â  ââ Class:_generate_file
+â  ââ Method:_get_all_versions
 â  ââ Method:_get_examples_path
 â  ââ Method:_get_exeproduct_path
 â  ââ Method:_get_exetarget_path
+â  ââ Method:_get_file_from_path
+â  ââ Method:_get_filenames
+â  ââ Method:_get_files
+â  ââ Method:_get_files_by_relative_path
 â  ââ Method:_get_generate_path
 â  ââ Method:_get_git_exclude_path
 â  ââ Method:_get_git_ignore_path
 â  ââ Method:_get_index_js_path
 â  ââ Method:_get_init_path
 â  ââ Method:_get_license_path
 â  ââ Method:_get_manifest_path
 â  ââ Method:_get_metadata_path
 â  ââ Method:_get_npm_ignore_path
 â  ââ Method:_get_org_readme_path
 â  ââ Method:_get_package_json_path
 â  ââ Method:_get_package_paths_gen
 â  ââ Method:_get_pre_commit_hook_path
 â  ââ Method:_get_pre_push_hook_path
-â  ââ Method:_get_randomtesting_path
 â  ââ Method:_get_readme_path
 â  ââ Method:_get_setup_path
 â  ââ Method:_get_test_js_path
 â  ââ Method:_get_test_path
 â  ââ Method:_get_test_paths
 â  ââ Method:_get_test_template_path
 â  ââ Method:_get_workflow_path
 â  ââ Method:_git_config
+â  ââ Class:_git_exclude_file
 â  ââ Method:_git_missing_credentials
 â  ââ Method:_git_nothing_to_commit
+â  ââ Class:_gitignore_file
+â  ââ Class:_index_js_file
 â  ââ Method:_init
+â  ââ Class:_init_file
 â  ââ Method:_is_django
 â  ââ Method:_is_exe
 â  ââ Method:_is_general
 â  ââ Method:_is_node
 â  ââ Method:_is_python
+â  ââ Class:_license_file
+â  ââ Class:_manifest_file
 â  ââ Property:_metadata
 â  ââ Method:_metadata_exists
+â  ââ Class:_metadata_file
 â  ââ Method:_name_is_general
+â  ââ Class:_npm_ignore_file
+â  ââ Class:_org_readme_file
+â  â  ââ Method:_get_org_description_markdown
+â  ââ Class:_package_json_file
+â  ââ Class:_pre_commit_hook_file
+â  ââ Class:_pre_push_hook_file
 â  ââ Method:_push
+â  ââ Class:_readme_file
+â  â  ââ Method:_get_attributes_markdown
+â  â  ââ Method:_get_badges_dict
+â  â  ââ Method:_get_contributions_markdown
+â  â  ââ Method:_get_description_markdown
+â  â  ââ Method:_get_examples_markdown
+â  â  ââ Method:_get_footnote_markdown
+â  â  ââ Method:_get_information_markdown
+â  â  ââ Method:_get_installation_markdown
+â  â  ââ Method:_get_mermaid_markdown
+â  â  ââ Method:_get_todos
+â  â  ââ Method:_get_todos_markdown
+â  â  ââ Method:_github_link
+â  â  ââ Method:_github_link_path_line
+â  â  ââ Method:_set_collapsible
 â  ââ Method:_repo_exists
+â  ââ Class:_setup_file
+â  â  ââ Method:_get_classifiers
 â  ââ Property:_simple_name
-â  ââ Property:_target
-â  ââ Method:_targetted
+â  ââ Method:_targetted
+â  ââ Class:_test_folder
+â  ââ Class:_test_js_file
+â  ââ Class:_test_template_file
+â  ââ Class:_workflow_dev_file
+â  ââ Class:_workflow_file
+â     ââ Method:_codeline
 ââ Class:_LocalRepo_Node
 ââ Class:_LocalRepo_Python
 â  ââ Method:_get_python_exe_path
-â  ââ Method:_unittest
+â  ââ Method:_set_easy_install_value
 ââ Class:_Packager
 â  ââ Class:_GitHub
 â  ââ Class:_LocalModule
 â  ââ Class:_LocalRepo
 â  ââ Class:_Packager
 â  ââ Class:_Packages
 â  â  ââ Method:_all_packages
 â  ââ Class:_PyPI
 â  ââ Class:_Targets
 â  ââ Method:_commit_and_push
 â  ââ Class:_commit_editmsg_file
 â  ââ Method:_compare_local_to_github
 â  ââ Method:_compare_local_to_pypi
-â  ââ Method:_create_blank_locally_python
+â  ââ Method:_create_blank_locally
 â  ââ Method:_create_github_repo
 â  ââ Method:_create_master_branch
 â  ââ Class:_examples_folder
 â  ââ Class:_exeproduct_folder
 â  ââ Class:_exetarget_file
 â  ââ Method:_general_bumped_set
 â  ââ Method:_general_changed_dict
@@ -180,14 +226,15 @@
 â  ââ Method:_get_latest_release
 â  ââ Method:_get_ordered_packagers
 â  ââ Method:_get_owners_package_names
 â  ââ Method:_get_topics
 â  ââ Class:_git_exclude_file
 â  ââ Property:_github
 â  ââ Method:_github_available
+â  ââ Class:_gitignore_file
 â  ââ Method:_if_publish_bump
 â  ââ Method:_if_publish_upload
 â  ââ Class:_index_js_file
 â  ââ Class:_init_file
 â  ââ Method:_is_bumped
 â  ââ Method:_is_django
 â  ââ Method:_is_exe
@@ -208,58 +255,77 @@
 â  ââ Class:_package_json_file
 â  ââ Method:_packagers_from_packages
 â  ââ Class:_pre_commit_hook_file
 â  ââ Class:_pre_push_hook_file
 â  ââ Method:_push
 â  ââ Property:_pypi
 â  ââ Method:_pypi_available
-â  ââ Class:_randomtesting_file
 â  ââ Class:_readme_file
 â  ââ Method:_reserve_name
 â  ââ Method:_run_ordered_methods
 â  ââ Class:_setup_file
 â  ââ Property:_simple_name
 â  ââ Method:_summary_packagers
 â  ââ Method:_sync_github_metadata
 â  ââ Property:_target
 â  ââ Class:_test_folder
 â  ââ Class:_test_js_file
 â  ââ Class:_test_template_file
 â  ââ Method:_upload_package_summary
+â  ââ Class:_workflow_dev_file
 â  ââ Class:_workflow_file
+â  ââ Method:_workflow_packagers
 â  ââ Method:_workflow_sync
 â  ââ Method:_workflow_unittest
-ââ Class:_PyPI
-   ââ Class:_GitHub
-   ââ Class:_LocalModule
-   ââ Class:_LocalRepo
-   ââ Class:_Packager
-   ââ Class:_PyPI
-   ââ Method:_download
+ââ Class:_PyPI
+â  ââ Class:_GitHub
+â  ââ Class:_LocalModule
+â  ââ Class:_LocalRepo
+â  ââ Class:_Packager
+â  ââ Class:_PyPI
+â  ââ Method:_is_general
+â  ââ Property:_json_endpoint
+â  ââ Method:_name_is_general
+â  ââ Property:_simple_name
+ââ Class:_Venv
+   ââ Method:_active
+   ââ Method:_create_venv
+   ââ Property:_cruds
+   ââ Method:_deactivate
+   ââ Method:_debug
+   ââ Method:_easy_install_path
+   ââ Method:_exe_name
    ââ Method:_exists
-   ââ Method:_get_date
-   ââ Method:_get_owners_packages
-   ââ Method:_get_tarball_url
-   ââ Method:_get_version
-   ââ Property:_url
+   ââ Method:_get_active_python
+   ââ Method:_get_active_venv
+   ââ Method:_get_active_venv_path
+   ââ Method:_list_python_versions
+   ââ Method:_list_venv_paths
+   ââ Method:_python_exe_path
+   ââ Method:_python_home_exe_path
+   ââ Method:_python_home_path
+   ââ Method:_python_path
+   ââ Method:_python_sys_executable_path
+   ââ Method:_python_version
+   ââ Method:_pyvenv_cfg_path
+   ââ Method:_scripts_path
+   ââ Method:_site_packages_path
 
 ***** Contributions *****
-Issue-creation and discussions are most welcome! Pull requests are currently
-not wanted, please discuss with me before investing any time
+Issue-creation, discussions and pull requests are most welcome!
 ***** Todo *****
 | Module | Message | |:--------------------------------------------------------
 -------------------------------------------------------------------------------
 ---------------------|:--------------------------------------------------------
 -------------------------------------------------------------------------------
 --------------------------------------------------------------------------| |
 packager_files.py | Fix_create_blank,_it_overwrites_current_projects_pip
-install. | | localrepo_python.py | Make_sure_twine_is_installed_when_trying_to
-upload_to_pypi. | | localrepo_python.py | Look_into_private_PyPI_server_where
-we_could_also_do_dry_runs_for_test. | | metadata_python.py | Dynamic_values_in
-DataClass_to_remove_LocalRepos_and_Metadatas. | | localrepo.py | Search_for
-imports_to_list_dependencies. | | pypi.py | Move_download_to_it's_own_package.
-| | pypi.py | Find_a_faster_fetch_for_latest_PyPI_version_and_datetime. | |
+install. | | packager_github.py | Setup_env_vars_for_project. | | target.py |
+Generate_Python_file_in_generalpackager_containing_general_packages. | |
 readme.py | Sort_todos_by_name_to_decrease_automatic_commit_changes. | |
-github.py | Get_and_Set_GitHub_repo_private. | | packages.py | Generate_Python
-file_in_generalpackager_containing_general_packages. | | packager_github.py |
-Setup_env_vars_for_project. |  Generated 2023-02-02 13:29 CET for commit
-master.
+pypi.py | Move_download_to_it's_own_package. | | pypi.py | Find_a_faster_fetch
+for_latest_PyPI_version_and_datetime. | | github.py | Get_and_Set_GitHub_repo
+private. | | localrepo_python.py | Make_sure_twine_is_installed_when_trying_to
+upload_to_pypi. | | localrepo_python.py | Look_into_private_PyPI_server_where
+we_could_also_do_dry_runs_for_test. | | localrepo.py | Search_for_imports_to
+list_dependencies. | | packager_api.py | Check_that_every_API_has_create_an
+*_available_method |  Generated 2023-06-02 23:27 CEST for commit master.
```

### Comparing `generalpackager-0.5.7/generalpackager.egg-info/SOURCES.txt` & `generalpackager-0.5.8/generalpackager.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,67 +14,72 @@
 generalpackager/packager_relations.py
 generalpackager/packager_workflow.py
 generalpackager.egg-info/PKG-INFO
 generalpackager.egg-info/SOURCES.txt
 generalpackager.egg-info/dependency_links.txt
 generalpackager.egg-info/requires.txt
 generalpackager.egg-info/top_level.txt
-generalpackager/api/github.py
 generalpackager/api/localmodule.py
-generalpackager/api/npm.py
-generalpackager/api/pypi.py
 generalpackager/api/venv.py
+generalpackager/api/venv_cruds.py
 generalpackager/api/localrepo/base/localrepo.py
 generalpackager/api/localrepo/base/localrepo_git.py
 generalpackager/api/localrepo/base/localrepo_paths.py
 generalpackager/api/localrepo/base/localrepo_target.py
 generalpackager/api/localrepo/base/metadata.py
-generalpackager/api/localrepo/base/targets.py
 generalpackager/api/localrepo/node/localrepo_node.py
 generalpackager/api/localrepo/node/metadata_node.py
 generalpackager/api/localrepo/python/localrepo_python.py
 generalpackager/api/localrepo/python/metadata_python.py
+generalpackager/api/localrepo/top/target_helper.py
+generalpackager/api/package_hosts/github.py
+generalpackager/api/package_hosts/npm.py
+generalpackager/api/package_hosts/pypi.py
 generalpackager/api/shared/decos.py
 generalpackager/api/shared/name.py
 generalpackager/api/shared/owner.py
 generalpackager/api/shared/path.py
+generalpackager/api/shared/protocols.py
+generalpackager/api/shared/target.py
 generalpackager/api/shared/files/file.py
 generalpackager/api/shared/files/file_fetcher.py
+generalpackager/api/shared/files/helpers.py
 generalpackager/api/shared/files/shared_files.py
 generalpackager/api/shared/files/definitions/commit_editmsg.py
 generalpackager/api/shared/files/definitions/examples.py
 generalpackager/api/shared/files/definitions/exeproduct.py
 generalpackager/api/shared/files/definitions/exetarget.py
 generalpackager/api/shared/files/definitions/generate.py
 generalpackager/api/shared/files/definitions/git_exclude.py
+generalpackager/api/shared/files/definitions/gitignore.py
 generalpackager/api/shared/files/definitions/index_js.py
 generalpackager/api/shared/files/definitions/init.py
 generalpackager/api/shared/files/definitions/license.py
 generalpackager/api/shared/files/definitions/manifest.py
 generalpackager/api/shared/files/definitions/metadata.py
 generalpackager/api/shared/files/definitions/npm_ignore.py
 generalpackager/api/shared/files/definitions/org_readme.py
 generalpackager/api/shared/files/definitions/package_json.py
 generalpackager/api/shared/files/definitions/pre_commit_hook.py
 generalpackager/api/shared/files/definitions/pre_push_hook.py
-generalpackager/api/shared/files/definitions/randomtesting.py
 generalpackager/api/shared/files/definitions/readme.py
 generalpackager/api/shared/files/definitions/setup.py
 generalpackager/api/shared/files/definitions/test.py
 generalpackager/api/shared/files/definitions/test_js.py
 generalpackager/api/shared/files/definitions/test_template.py
 generalpackager/api/shared/files/definitions/workflow.py
+generalpackager/api/shared/files/definitions/workflow_dev.py
 generalpackager/other/envvars.py
 generalpackager/other/licenses.py
-generalpackager/other/packages.py
 generalpackager/test/test_generalpackager.py
 generalpackager/test/test_github.py
 generalpackager/test/test_local_module.py
 generalpackager/test/test_local_repo.py
 generalpackager/test/test_local_repo_node.py
+generalpackager/test/test_local_repo_python.py
 generalpackager/test/test_packager.py
 generalpackager/test/test_packager_api.py
 generalpackager/test/test_packager_files.py
 generalpackager/test/test_packager_github.py
 generalpackager/test/test_packager_metadata.py
 generalpackager/test/test_packager_node.py
 generalpackager/test/test_packager_pypi.py
```

### Comparing `generalpackager-0.5.7/metadata.json` & `generalpackager-0.5.8/metadata.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8920454545454546%*

 * *Differences: {"'contribute'": 'True',*

 * * "'install_requires'": "{insert: [(5, 'setuptools'), (6, 'wheel'), (7, 'twine')]}",*

 * * "'version'": "'0.5.8'"}*

```diff
@@ -1,23 +1,26 @@
 {
-    "contribute": false,
+    "contribute": true,
     "description": "Tools to interface GitHub, PyPI, NPM and local modules / repos. Used for generating files to keep projects dry and synced. Tailored for ManderaGeneral for now.",
     "enabled": true,
     "extras_require": {},
     "install_requires": [
         "generallibrary[table]",
         "generalfile",
         "requests",
         "pyinstaller",
-        "coverage"
+        "coverage",
+        "setuptools",
+        "wheel",
+        "twine"
     ],
     "manifest": [
         "generalpackager/licenses/*"
     ],
     "name": "generalpackager",
     "private": false,
     "target": "python",
     "topics": [
         "tool"
     ],
-    "version": "0.5.7"
+    "version": "0.5.8"
 }
```

### Comparing `generalpackager-0.5.7/setup.py` & `generalpackager-0.5.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,24 +7,27 @@
 except FileNotFoundError:
     long_description = 'Readme missing'
 
 setup(
     name="generalpackager",
     author='Rickard "Mandera" Abraham',
     author_email="rickard.abraham@gmail.com",
-    version="0.5.7",
+    version="0.5.8",
     description="Tools to interface GitHub, PyPI, NPM and local modules / repos. Used for generating files to keep projects dry and synced. Tailored for ManderaGeneral for now.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         'generallibrary[table]',
         'generalfile',
         'requests',
         'pyinstaller',
         'coverage',
+        'setuptools',
+        'wheel',
+        'twine',
     ],
     url="https://github.com/ManderaGeneral/generalpackager",
     license="mit",
     packages=find_namespace_packages(exclude=("build*", "dist*")),
     extras_require={},
     classifiers=[
         'Topic :: Software Development :: Build Tools',
```

