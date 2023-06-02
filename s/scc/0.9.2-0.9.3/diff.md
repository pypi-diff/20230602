# Comparing `tmp/scc-0.9.2.tar.gz` & `tmp/scc-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scc-0.9.2.tar", last modified: Wed Feb 14 17:03:56 2018, max compression
+gzip compressed data, was "dist/scc-0.9.3.tar", last modified: Wed Feb 21 17:24:40 2018, max compression
```

## Comparing `scc-0.9.2.tar` & `scc-0.9.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 jamoore    (501) staff       (20)        0 2018-02-14 17:03:56.000000 scc-0.9.2/
--rw-r--r--   0 jamoore    (501) staff       (20)    15145 2015-11-19 11:08:35.000000 scc-0.9.2/LICENSE.txt
--rw-r--r--   0 jamoore    (501) staff       (20)       91 2015-11-19 11:08:35.000000 scc-0.9.2/MANIFEST.in
--rw-r--r--   0 jamoore    (501) staff       (20)     4661 2018-02-14 17:03:56.000000 scc-0.9.2/PKG-INFO
--rw-r--r--   0 jamoore    (501) staff       (20)     3000 2017-12-04 05:40:45.000000 scc-0.9.2/README.rst
--rw-r--r--   0 jamoore    (501) staff       (20)       41 2018-02-12 16:09:29.000000 scc-0.9.2/requirements.txt
-drwxr-xr-x   0 jamoore    (501) staff       (20)        0 2018-02-14 17:03:56.000000 scc-0.9.2/scc/
--rw-r--r--   0 jamoore    (501) staff       (20)        0 2015-11-19 11:08:35.000000 scc-0.9.2/scc/__init__.py
--rw-r--r--   0 jamoore    (501) staff       (20)     4724 2015-11-19 11:08:35.000000 scc-0.9.2/scc/deploy.py
--rwxr-xr-x   0 jamoore    (501) staff       (20)   135123 2018-02-14 16:55:04.000000 scc-0.9.2/scc/git.py
--rw-r--r--   0 jamoore    (501) staff       (20)     2792 2017-12-04 12:46:31.000000 scc-0.9.2/scc/main.py
--rw-r--r--   0 jamoore    (501) staff       (20)        6 2018-02-14 16:55:53.000000 scc-0.9.2/scc/RELEASE-VERSION
--rw-r--r--   0 jamoore    (501) staff       (20)     1198 2018-02-12 16:09:29.000000 scc-0.9.2/scc/version.py
-drwxr-xr-x   0 jamoore    (501) staff       (20)        0 2018-02-14 17:03:56.000000 scc-0.9.2/scc.egg-info/
--rw-r--r--   0 jamoore    (501) staff       (20)        1 2018-02-14 17:03:56.000000 scc-0.9.2/scc.egg-info/dependency_links.txt
--rw-r--r--   0 jamoore    (501) staff       (20)       46 2018-02-14 17:03:56.000000 scc-0.9.2/scc.egg-info/entry_points.txt
--rw-r--r--   0 jamoore    (501) staff       (20)     4661 2018-02-14 17:03:56.000000 scc-0.9.2/scc.egg-info/PKG-INFO
--rw-r--r--   0 jamoore    (501) staff       (20)       50 2018-02-14 17:03:56.000000 scc-0.9.2/scc.egg-info/requires.txt
--rw-r--r--   0 jamoore    (501) staff       (20)      344 2018-02-14 17:03:56.000000 scc-0.9.2/scc.egg-info/SOURCES.txt
--rw-r--r--   0 jamoore    (501) staff       (20)        4 2018-02-14 17:03:56.000000 scc-0.9.2/scc.egg-info/top_level.txt
--rw-r--r--   0 jamoore    (501) staff       (20)        1 2018-02-12 16:11:32.000000 scc-0.9.2/scc.egg-info/zip-safe
--rw-r--r--   0 jamoore    (501) staff       (20)       68 2018-02-14 17:03:56.000000 scc-0.9.2/setup.cfg
--rwxr-xr-x   0 jamoore    (501) staff       (20)     4524 2018-02-12 16:09:29.000000 scc-0.9.2/setup.py
+drwxr-xr-x   0 sbesson  (1027705065) DUNDEE\Domain Users (1133848969)        0 2018-02-21 17:24:40.000000 scc-0.9.3/
+-rw-r--r--   0 sbesson  (1027705065) DUNDEE\Domain Users (1133848969)    15145 2014-06-24 13:56:25.000000 scc-0.9.3/LICENSE.txt
+-rw-r--r--   0 sbesson  (1027705065) DUNDEE\Domain Users (1133848969)       91 2014-06-24 13:56:25.000000 scc-0.9.3/MANIFEST.in
+-rw-r--r--   0 sbesson  (1027705065) DUNDEE\Domain Users (1133848969)     4661 2018-02-21 17:24:40.000000 scc-0.9.3/PKG-INFO
+-rw-r--r--   0 sbesson  (1027705065) DUNDEE\Domain Users (1133848969)     3000 2016-10-20 11:59:52.000000 scc-0.9.3/README.rst
+-rw-r--r--   0 sbesson  (1027705065) DUNDEE\Domain Users (1133848969)       41 2018-02-12 19:25:31.000000 scc-0.9.3/requirements.txt
+drwxr-xr-x   0 sbesson  (1027705065) DUNDEE\Domain Users (1133848969)        0 2018-02-21 17:24:40.000000 scc-0.9.3/scc/
+-rw-r--r--   0 sbesson  (1027705065) DUNDEE\Domain Users (1133848969)        0 2014-06-24 13:56:25.000000 scc-0.9.3/scc/__init__.py
+-rw-r--r--   0 sbesson  (1027705065) DUNDEE\Domain Users (1133848969)     4724 2014-10-05 09:00:12.000000 scc-0.9.3/scc/deploy.py
+-rwxr-xr-x   0 sbesson  (1027705065) DUNDEE\Domain Users (1133848969)   135148 2018-02-21 17:23:17.000000 scc-0.9.3/scc/git.py
+-rw-r--r--   0 sbesson  (1027705065) DUNDEE\Domain Users (1133848969)     2792 2018-02-12 15:51:40.000000 scc-0.9.3/scc/main.py
+-rw-r--r--   0 sbesson  (1027705065) DUNDEE\Domain Users (1133848969)        6 2018-02-21 17:23:17.000000 scc-0.9.3/scc/RELEASE-VERSION
+-rw-r--r--   0 sbesson  (1027705065) DUNDEE\Domain Users (1133848969)     1198 2018-02-12 19:25:31.000000 scc-0.9.3/scc/version.py
+drwxr-xr-x   0 sbesson  (1027705065) DUNDEE\Domain Users (1133848969)        0 2018-02-21 17:24:40.000000 scc-0.9.3/scc.egg-info/
+-rw-r--r--   0 sbesson  (1027705065) DUNDEE\Domain Users (1133848969)        1 2018-02-21 17:24:40.000000 scc-0.9.3/scc.egg-info/dependency_links.txt
+-rw-r--r--   0 sbesson  (1027705065) DUNDEE\Domain Users (1133848969)       46 2018-02-21 17:24:40.000000 scc-0.9.3/scc.egg-info/entry_points.txt
+-rw-r--r--   0 sbesson  (1027705065) DUNDEE\Domain Users (1133848969)     4661 2018-02-21 17:24:40.000000 scc-0.9.3/scc.egg-info/PKG-INFO
+-rw-r--r--   0 sbesson  (1027705065) DUNDEE\Domain Users (1133848969)       50 2018-02-21 17:24:40.000000 scc-0.9.3/scc.egg-info/requires.txt
+-rw-r--r--   0 sbesson  (1027705065) DUNDEE\Domain Users (1133848969)      344 2018-02-21 17:24:40.000000 scc-0.9.3/scc.egg-info/SOURCES.txt
+-rw-r--r--   0 sbesson  (1027705065) DUNDEE\Domain Users (1133848969)        4 2018-02-21 17:24:40.000000 scc-0.9.3/scc.egg-info/top_level.txt
+-rw-r--r--   0 sbesson  (1027705065) DUNDEE\Domain Users (1133848969)        1 2018-02-21 17:24:40.000000 scc-0.9.3/scc.egg-info/zip-safe
+-rw-r--r--   0 sbesson  (1027705065) DUNDEE\Domain Users (1133848969)       68 2018-02-21 17:24:40.000000 scc-0.9.3/setup.cfg
+-rwxr-xr-x   0 sbesson  (1027705065) DUNDEE\Domain Users (1133848969)     4524 2018-02-12 19:25:31.000000 scc-0.9.3/setup.py
```

### Comparing `scc-0.9.2/LICENSE.txt` & `scc-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scc-0.9.2/PKG-INFO` & `scc-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scc
-Version: 0.9.2
+Version: 0.9.3
 Summary: OME tools for managing the git(hub) workflow
 Home-page: https://github.com/openmicroscopy/snoopycrimecop
 Author: The Open Microscopy Team
 Author-email: ome-devel@lists.openmicroscopy.org.uk
 License: GPLv2
 Description-Content-Type: UNKNOWN
 Description: Snoopy Crime Copy (SCC)
```

### Comparing `scc-0.9.2/README.rst` & `scc-0.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `scc-0.9.2/scc/deploy.py` & `scc-0.9.3/scc/deploy.py`

 * *Files identical despite different names*

### Comparing `scc-0.9.2/scc/git.py` & `scc-0.9.3/scc/git.py`

 * *Files 0% similar despite different names*

```diff
@@ -890,15 +890,15 @@
         # Combine pr filter with user/repo filters
         repo_name = "%s/%s" % (self.user_name, self.repo_name)
         for ftype in ["include", "exclude"]:
             if filters[ftype].get(repo_name, None):
                 filters[ftype].setdefault("pr", []).extend(
                     filters[ftype][repo_name])
 
-        # Loop over pull requests opened aGainst base
+        # Loop over pull requests opened against base
         pulls = self.get_pulls_by_base(filters["base"])
         excluded_pulls = {}
 
         for pull in pulls:
             pullrequest = PullRequest(pull)
             include, exclude_reason = self.filter_pull(pullrequest, filters)
 
@@ -1742,35 +1742,36 @@
                 '/' in x and not x.endswith(repo_names))
 
     def rmerge(self, filters, info=False, comment=False, commit_id="merge",
                top_message=None, update_gitmodules=False,
                set_commit_status=False, allow_empty=True, is_submodule=False):
         """Recursively merge PRs for each submodule."""
 
+        if self.repository_config is not None and \
+           "base-branch" in self.repository_config and \
+           filters["base"] != self.repository_config["base-branch"]:
+            self.log.info("Overriding base-branch from %s to %s" %
+                          (filters["base"],
+                           self.repository_config["base-branch"]))
+            filters["base"] = self.repository_config["base-branch"]
+
         updated = False
         merge_msg = ""
         merge_msg += str(self.origin) + "\n"
         merge_msg += self.origin.find_candidate_pulls(filters)
         self.origin.find_candidate_branches(
             filters, fork_filter=self.get_fork_filter(is_submodule))
         if info:
             merge_msg += self.origin.merge_info()
         else:
             self.cd(self.path)
             self.write_directories()
             presha1 = self.get_current_sha1()
-            basebranch = filters["base"]
-            if self.repository_config is not None and \
-               "base-branch" in self.repository_config:
-                self.log.info("Overriding base-branch from %s to %s" %
-                              (filters["base"],
-                               self.repository_config["base-branch"]))
-                basebranch = self.repository_config["base-branch"]
-            if self.has_remote_branch(basebranch, self.remote):
-                ff_msg, ff_log = self.fast_forward(basebranch,
+            if self.has_remote_branch(filters["base"], self.remote):
+                ff_msg, ff_log = self.fast_forward(filters["base"],
                                                    remote=self.remote)
                 merge_msg += ff_msg
                 # Scan the ff log to produce a digest of the merged PRs
                 if ff_log:
                     merge_msg += "Previously merged:\n"
                     pattern = r'Merge pull request #(\d+)'
                     for line in ff_log.split('\n'):
```

### Comparing `scc-0.9.2/scc/main.py` & `scc-0.9.3/scc/main.py`

 * *Files identical despite different names*

### Comparing `scc-0.9.2/scc/version.py` & `scc-0.9.3/scc/version.py`

 * *Files identical despite different names*

### Comparing `scc-0.9.2/scc.egg-info/PKG-INFO` & `scc-0.9.3/scc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scc
-Version: 0.9.2
+Version: 0.9.3
 Summary: OME tools for managing the git(hub) workflow
 Home-page: https://github.com/openmicroscopy/snoopycrimecop
 Author: The Open Microscopy Team
 Author-email: ome-devel@lists.openmicroscopy.org.uk
 License: GPLv2
 Description-Content-Type: UNKNOWN
 Description: Snoopy Crime Copy (SCC)
```

### Comparing `scc-0.9.2/setup.py` & `scc-0.9.3/setup.py`

 * *Files identical despite different names*

