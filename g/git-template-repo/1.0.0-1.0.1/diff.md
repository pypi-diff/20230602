# Comparing `tmp/git_template_repo-1.0.0.tar.gz` & `tmp/git_template_repo-1.0.1.tar.gz`

## Comparing `git_template_repo-1.0.0.tar` & `git_template_repo-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 git_template_repo-1.0.0/.editorconfig
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 git_template_repo-1.0.0/.flake8
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 git_template_repo-1.0.0/.gitattributes
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 git_template_repo-1.0.0/git_template_repo/__init__.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 git_template_repo-1.0.0/git_template_repo/__main__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 git_template_repo-1.0.0/git_template_repo/_version.py
--rw-r--r--   0        0        0     7221 2020-02-02 00:00:00.000000 git_template_repo-1.0.0/git_template_repo/git_template_repo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 git_template_repo-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 git_template_repo-1.0.0/tests/test_commands.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 git_template_repo-1.0.0/tests/test_internal.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 git_template_repo-1.0.0/.gitignore
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 git_template_repo-1.0.0/LICENSE
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 git_template_repo-1.0.0/README.md
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 git_template_repo-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     7102 2020-02-02 00:00:00.000000 git_template_repo-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 git_template_repo-1.0.1/.editorconfig
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 git_template_repo-1.0.1/.flake8
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 git_template_repo-1.0.1/.gitattributes
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 git_template_repo-1.0.1/git_template_repo/__init__.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 git_template_repo-1.0.1/git_template_repo/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 git_template_repo-1.0.1/git_template_repo/_version.py
+-rw-r--r--   0        0        0     7260 2020-02-02 00:00:00.000000 git_template_repo-1.0.1/git_template_repo/git_template_repo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 git_template_repo-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 git_template_repo-1.0.1/tests/test_commands.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 git_template_repo-1.0.1/tests/test_internal.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 git_template_repo-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 git_template_repo-1.0.1/LICENSE
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 git_template_repo-1.0.1/README.md
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 git_template_repo-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     7102 2020-02-02 00:00:00.000000 git_template_repo-1.0.1/PKG-INFO
```

### Comparing `git_template_repo-1.0.0/git_template_repo/git_template_repo.py` & `git_template_repo-1.0.1/git_template_repo/git_template_repo.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,28 +79,28 @@
                 print("ERROR: Repository directory already exists.")
                 return 1
 
         if no_clone:
             os.chdir(clone_dir)
             make_call("git", "init")
         else:
-            make_call("git", "clone", new_repo, clone_dir)
+            make_call("git", "clone", "--no-tags", new_repo, clone_dir)
             os.chdir(clone_dir)
 
     if int(make_call("git", "rev-list", "--all", "--count")):
         print("ERROR: Can only initialize a template on an empty repository with no commits.")
         return 1
 
     make_call("git", "remote", "add", "template", template_repo)
 
     if is_sha1(template_branch):
-        make_call("git", "fetch", "template", template_branch)
+        make_call("git", "fetch", "--no-tags", "template", template_branch)
         make_call("git", "checkout", "--orphan", new_root_branch, template_branch)
     else:
-        make_call("git", "fetch", "template")
+        make_call("git", "fetch", "--no-tags", "template")
         make_call("git", "checkout", "--orphan", new_root_branch, f"template/{template_branch}")
 
     make_call("git", "add", "-A")
     make_call("git", "commit", "-m", f"Template initialization from {template_repo}.")
     make_call("git", "remote", "rm", "template")
     if push_origin and not local_new and not no_clone:
         if origin_name != "origin":
```

### Comparing `git_template_repo-1.0.0/tests/test_commands.py` & `git_template_repo-1.0.1/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `git_template_repo-1.0.0/tests/test_internal.py` & `git_template_repo-1.0.1/tests/test_internal.py`

 * *Files identical despite different names*

### Comparing `git_template_repo-1.0.0/.gitignore` & `git_template_repo-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `git_template_repo-1.0.0/LICENSE` & `git_template_repo-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `git_template_repo-1.0.0/README.md` & `git_template_repo-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `git_template_repo-1.0.0/pyproject.toml` & `git_template_repo-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `git_template_repo-1.0.0/PKG-INFO` & `git_template_repo-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-template-repo
-Version: 1.0.0
+Version: 1.0.1
 Summary: A git command for creating a git repository from another repository as a template.
 Project-URL: Homepage, https://github.com/IDI-Systems/git-template-repo
 Project-URL: Bug Tracker, https://github.com/IDI-Systems/git-template-repo
 Author-email: IDI-Systems <contact@idi-systems.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
```

