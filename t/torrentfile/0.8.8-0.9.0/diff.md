# Comparing `tmp/torrentfile-0.8.8.tar.gz` & `tmp/torrentfile-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torrentfile-0.8.8.tar", last modified: Thu Mar  2 10:43:51 2023, max compression
+gzip compressed data, was "torrentfile-0.9.0.tar", last modified: Fri Jun  2 12:42:24 2023, max compression
```

## Comparing `torrentfile-0.8.8.tar` & `torrentfile-0.9.0.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-03-02 10:43:51.193834 torrentfile-0.8.8/
--rw-rw-rw-   0        0        0     1879 2022-06-06 03:34:50.000000 torrentfile-0.8.8/.cbuild
--rw-rw-rw-   0        0        0     9123 2023-03-02 05:11:02.000000 torrentfile-0.8.8/CHANGELOG.md
--rw-rw-rw-   0        0        0    11560 2022-04-01 22:38:43.000000 torrentfile-0.8.8/LICENSE
--rw-rw-rw-   0        0        0      153 2023-01-14 00:36:54.000000 torrentfile-0.8.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2610 2023-03-02 04:35:28.000000 torrentfile-0.8.8/Makefile
--rw-rw-rw-   0        0        0    22470 2023-03-02 10:43:51.193834 torrentfile-0.8.8/PKG-INFO
--rw-rw-rw-   0        0        0     7644 2023-03-02 05:53:52.000000 torrentfile-0.8.8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-02 10:43:51.170080 torrentfile-0.8.8/assets/
--rw-rw-rw-   0        0        0   999094 2022-10-21 07:26:02.000000 torrentfile-0.8.8/assets/Torrentfile.gif
--rw-rw-rw-   0        0        0    67244 2022-05-08 04:09:13.000000 torrentfile-0.8.8/assets/torrentfile-icon.ico
--rw-rw-rw-   0        0        0    31493 2022-05-08 04:09:13.000000 torrentfile-0.8.8/assets/torrentfile-icon.png
--rw-rw-rw-   0        0        0    25857 2022-02-13 04:29:03.000000 torrentfile-0.8.8/assets/torrentfile.png
-drwxrwxrwx   0        0        0        0 2023-03-02 10:43:51.173109 torrentfile-0.8.8/c/
--rw-rw-rw-   0        0        0    12601 2022-04-05 09:08:46.000000 torrentfile-0.8.8/c/hasher.c
--rw-rw-rw-   0        0        0     1396 2022-04-01 22:38:43.000000 torrentfile-0.8.8/c/hasher.h
--rw-rw-rw-   0        0        0    11387 2022-04-01 22:38:43.000000 torrentfile-0.8.8/c/sha.c
--rw-rw-rw-   0        0        0     1629 2022-04-01 22:38:43.000000 torrentfile-0.8.8/c/sha.h
--rw-rw-rw-   0        0        0     2511 2023-03-02 07:28:29.000000 torrentfile-0.8.8/pyproject.toml
--rw-rw-rw-   0        0        0       13 2022-06-05 02:35:20.000000 torrentfile-0.8.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-03-02 10:43:51.194857 torrentfile-0.8.8/setup.cfg
--rw-rw-rw-   0        0        0      914 2022-08-07 23:54:01.000000 torrentfile-0.8.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-02 10:43:51.179106 torrentfile-0.8.8/tests/
--rw-rw-rw-   0        0        0    14895 2023-03-02 10:42:17.000000 torrentfile-0.8.8/tests/test_cli.py
--rw-rw-rw-   0        0        0     9288 2023-03-02 10:42:17.000000 torrentfile-0.8.8/tests/test_commands.py
--rw-rw-rw-   0        0        0     7214 2023-03-02 10:42:17.000000 torrentfile-0.8.8/tests/test_edit.py
--rw-rw-rw-   0        0        0     5171 2023-03-02 10:42:17.000000 torrentfile-0.8.8/tests/test_interactive.py
--rw-rw-rw-   0        0        0     5823 2023-03-02 10:42:17.000000 torrentfile-0.8.8/tests/test_rebuild.py
--rw-rw-rw-   0        0        0     8804 2023-03-02 10:42:17.000000 torrentfile-0.8.8/tests/test_recheck.py
--rw-rw-rw-   0        0        0     7030 2023-03-02 10:42:17.000000 torrentfile-0.8.8/tests/test_torrent.py
--rw-rw-rw-   0        0        0     6741 2023-03-02 10:42:17.000000 torrentfile-0.8.8/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-02 10:43:51.188175 torrentfile-0.8.8/torrentfile/
--rw-rw-rw-   0        0        0     1810 2023-03-02 10:42:15.000000 torrentfile-0.8.8/torrentfile/__init__.py
--rw-rw-rw-   0        0        0     1079 2023-03-02 10:42:15.000000 torrentfile-0.8.8/torrentfile/__main__.py
--rw-rw-rw-   0        0        0    17505 2023-03-02 10:42:17.000000 torrentfile-0.8.8/torrentfile/cli.py
--rw-rw-rw-   0        0        0    11276 2023-03-02 10:42:17.000000 torrentfile-0.8.8/torrentfile/commands.py
--rw-rw-rw-   0        0        0     3647 2023-03-02 06:39:30.000000 torrentfile-0.8.8/torrentfile/edit.py
--rw-rw-rw-   0        0        0    16402 2023-03-02 06:39:30.000000 torrentfile-0.8.8/torrentfile/hasher.py
--rw-rw-rw-   0        0        0    11745 2023-03-02 10:42:17.000000 torrentfile-0.8.8/torrentfile/interactive.py
--rw-rw-rw-   0        0        0     7695 2023-03-02 10:42:17.000000 torrentfile-0.8.8/torrentfile/mixins.py
--rw-rw-rw-   0        0        0    18852 2023-03-02 10:42:19.000000 torrentfile-0.8.8/torrentfile/rebuild.py
--rw-rw-rw-   0        0        0    20594 2023-03-02 10:42:17.000000 torrentfile-0.8.8/torrentfile/recheck.py
--rw-rw-rw-   0        0        0    23628 2023-03-02 10:42:17.000000 torrentfile-0.8.8/torrentfile/torrent.py
--rw-rw-rw-   0        0        0    11604 2023-03-02 10:42:17.000000 torrentfile-0.8.8/torrentfile/utils.py
--rw-rw-rw-   0        0        0      882 2023-03-02 05:07:36.000000 torrentfile-0.8.8/torrentfile/version.py
-drwxrwxrwx   0        0        0        0 2023-03-02 10:43:51.193321 torrentfile-0.8.8/torrentfile.egg-info/
--rw-rw-rw-   0        0        0    22470 2023-03-02 10:43:51.000000 torrentfile-0.8.8/torrentfile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      927 2023-03-02 10:43:51.000000 torrentfile-0.8.8/torrentfile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-02 10:43:51.000000 torrentfile-0.8.8/torrentfile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-03-02 10:43:51.000000 torrentfile-0.8.8/torrentfile.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-03-02 10:43:51.000000 torrentfile-0.8.8/torrentfile.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-02 10:43:51.000000 torrentfile-0.8.8/torrentfile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1893 2023-03-02 06:44:09.000000 torrentfile-0.8.8/tox.ini
+drwxrwxrwx   0        0        0        0 2023-06-02 12:42:24.695457 torrentfile-0.9.0/
+-rw-rw-rw-   0        0        0     1879 2022-06-06 03:34:50.000000 torrentfile-0.9.0/.cbuild
+-rw-rw-rw-   0        0        0    10935 2023-06-02 07:12:23.000000 torrentfile-0.9.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0    11560 2022-04-01 22:38:43.000000 torrentfile-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0      153 2023-01-14 00:36:54.000000 torrentfile-0.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2602 2023-06-02 07:16:26.000000 torrentfile-0.9.0/Makefile
+-rw-rw-rw-   0        0        0     9234 2023-06-02 12:42:24.694484 torrentfile-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7730 2023-06-02 07:11:55.000000 torrentfile-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 12:42:24.674872 torrentfile-0.9.0/assets/
+-rw-rw-rw-   0        0        0   999094 2022-10-21 07:26:02.000000 torrentfile-0.9.0/assets/Torrentfile.gif
+-rw-rw-rw-   0        0        0    67244 2022-05-08 04:09:13.000000 torrentfile-0.9.0/assets/torrentfile-icon.ico
+-rw-rw-rw-   0        0        0    31493 2022-05-08 04:09:13.000000 torrentfile-0.9.0/assets/torrentfile-icon.png
+-rw-rw-rw-   0        0        0    25857 2022-02-13 04:29:03.000000 torrentfile-0.9.0/assets/torrentfile.png
+-rw-rw-rw-   0        0        0    28319 2023-03-23 06:06:04.000000 torrentfile-0.9.0/assets/torrentfile_square.png
+drwxrwxrwx   0        0        0        0 2023-06-02 12:42:24.676872 torrentfile-0.9.0/c/
+-rw-rw-rw-   0        0        0    12601 2022-04-05 09:08:46.000000 torrentfile-0.9.0/c/hasher.c
+-rw-rw-rw-   0        0        0     1396 2022-04-01 22:38:43.000000 torrentfile-0.9.0/c/hasher.h
+-rw-rw-rw-   0        0        0    11387 2022-04-01 22:38:43.000000 torrentfile-0.9.0/c/sha.c
+-rw-rw-rw-   0        0        0     1629 2022-04-01 22:38:43.000000 torrentfile-0.9.0/c/sha.h
+-rw-rw-rw-   0        0        0     2658 2023-06-02 11:57:14.000000 torrentfile-0.9.0/pyproject.toml
+-rw-rw-rw-   0        0        0       13 2022-06-05 02:35:20.000000 torrentfile-0.9.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 12:42:24.695457 torrentfile-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      914 2022-08-07 23:54:01.000000 torrentfile-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 12:42:24.680890 torrentfile-0.9.0/tests/
+-rw-rw-rw-   0        0        0    16240 2023-06-02 12:41:18.000000 torrentfile-0.9.0/tests/test_cli.py
+-rw-rw-rw-   0        0        0    11034 2023-06-02 12:41:18.000000 torrentfile-0.9.0/tests/test_commands.py
+-rw-rw-rw-   0        0        0     7349 2023-06-02 12:41:18.000000 torrentfile-0.9.0/tests/test_edit.py
+-rw-rw-rw-   0        0        0     5378 2023-06-02 12:41:18.000000 torrentfile-0.9.0/tests/test_interactive.py
+-rw-rw-rw-   0        0        0     5822 2023-06-02 12:41:18.000000 torrentfile-0.9.0/tests/test_rebuild.py
+-rw-rw-rw-   0        0        0     8794 2023-06-02 12:41:18.000000 torrentfile-0.9.0/tests/test_recheck.py
+-rw-rw-rw-   0        0        0     7015 2023-06-02 12:41:18.000000 torrentfile-0.9.0/tests/test_torrent.py
+-rw-rw-rw-   0        0        0     6562 2023-06-02 12:41:18.000000 torrentfile-0.9.0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-02 12:42:24.689867 torrentfile-0.9.0/torrentfile/
+-rw-rw-rw-   0        0        0     1449 2023-06-02 07:12:23.000000 torrentfile-0.9.0/torrentfile/__init__.py
+-rw-rw-rw-   0        0        0     1079 2023-03-26 13:35:42.000000 torrentfile-0.9.0/torrentfile/__main__.py
+-rw-rw-rw-   0        0        0    17744 2023-06-02 12:41:18.000000 torrentfile-0.9.0/torrentfile/cli.py
+-rw-rw-rw-   0        0        0    12699 2023-06-02 12:41:17.000000 torrentfile-0.9.0/torrentfile/commands.py
+-rw-rw-rw-   0        0        0     3777 2023-05-03 00:46:54.000000 torrentfile-0.9.0/torrentfile/edit.py
+-rw-rw-rw-   0        0        0    16772 2023-06-02 07:11:55.000000 torrentfile-0.9.0/torrentfile/hasher.py
+-rw-rw-rw-   0        0        0    11740 2023-06-02 12:41:17.000000 torrentfile-0.9.0/torrentfile/interactive.py
+-rw-rw-rw-   0        0        0     7972 2023-06-02 12:41:17.000000 torrentfile-0.9.0/torrentfile/mixins.py
+-rw-rw-rw-   0        0        0    19284 2023-06-02 12:41:17.000000 torrentfile-0.9.0/torrentfile/rebuild.py
+-rw-rw-rw-   0        0        0    20532 2023-06-02 12:41:17.000000 torrentfile-0.9.0/torrentfile/recheck.py
+-rw-rw-rw-   0        0        0    24434 2023-06-02 12:41:18.000000 torrentfile-0.9.0/torrentfile/torrent.py
+-rw-rw-rw-   0        0        0    10731 2023-06-02 12:41:18.000000 torrentfile-0.9.0/torrentfile/utils.py
+-rw-rw-rw-   0        0        0      905 2023-06-02 07:12:23.000000 torrentfile-0.9.0/torrentfile/version.py
+drwxrwxrwx   0        0        0        0 2023-06-02 12:42:24.694484 torrentfile-0.9.0/torrentfile.egg-info/
+-rw-rw-rw-   0        0        0     9234 2023-06-02 12:42:24.000000 torrentfile-0.9.0/torrentfile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      957 2023-06-02 12:42:24.000000 torrentfile-0.9.0/torrentfile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 12:42:24.000000 torrentfile-0.9.0/torrentfile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-06-02 12:42:24.000000 torrentfile-0.9.0/torrentfile.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-06-02 12:42:24.000000 torrentfile-0.9.0/torrentfile.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-02 12:42:24.000000 torrentfile-0.9.0/torrentfile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2018 2023-05-03 00:46:54.000000 torrentfile-0.9.0/tox.ini
```

### Comparing `torrentfile-0.8.8/.cbuild` & `torrentfile-0.9.0/.cbuild`

 * *Files identical despite different names*

### Comparing `torrentfile-0.8.8/LICENSE` & `torrentfile-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torrentfile-0.8.8/Makefile` & `torrentfile-0.9.0/Makefile`

 * *Files 20% similar despite different names*

```diff
@@ -18,33 +18,24 @@
 if data['version'] != __version__:
 	data['version'] = __version__
 	json.dump(data, open("package.json", "wt"), indent=2)
 endef
 export UPDATE_PACKAGE_VERSION
 
 define RENAME_FILE
-import shutil
-import sys
-import subprocess
-import time
 from torrentfile.version import __version__
+import os
+import sys
 if sys.platform == "win32":
-	time.sleep(2)
-	subprocess.Popen(["7z", "a", "./dist/temp.zip", "./dist/torrentfile.exe"])
-	time.sleep(2)
-	shutil.copy(
-		"./dist/temp.zip",
-		"./dist/torrentfile-v" + __version__ + "-win.zip")
-else:
-	time.sleep(2)
-	subprocess.Popen(["zip", "./dist/temp.zip", "./dist/torrentfile"])
-	time.sleep(2)
-	shutil.copy(
-		"./dist/temp.zip",
-		"./dist/torrentfile-v" + __version__ + "-linux.zip")
+	inexe = "./torrentfile-windows-exec.zip"
+	exe = f"./dist/torrentfile-v{__version__}-win-exe.zip"
+	indir = "./torrentfile-windows-dir.zip"
+	dir = f"./dist/torrentfile-v{__version__}-win-dir.zip"
+	os.rename(inexe, exe)
+	os.rename(indir, dir)
 endef
 export RENAME_FILE
 
 BROWSER := python -c "$$BROWSER_PYSCRIPT"
 
 RENAME := python -c "$$RENAME_FILE"
 
@@ -69,19 +60,19 @@
 	rm -rfv .benchmarks
 	rm -rfv .codacy-coverage
 	rm -rfv node_modules
 	rm -fv torrentfile.log
 	rm -fvr -- *'/__pycache__'
 	rm -frv runner/build
 	rm -frv runner/dist
-
-extra: ## extra imports
-	pip install torrentfile torrentfileQt QStyler ebookatty --force-reinstall --no-cache --upgrade
+	rm -rfv *.zip
+	rm -fv *.spec
 
 test: ## Get coverage report
+	pip install --pre --upgrade --force-reinstall --no-cache -rrequirements.txt
 	tox
 
 docs: ## Regenerate docs from changes
 	rm -rfv docs/*
 	rm -rfv site/index.md
 	cp -rfv README.md site/index.md
 	cp -rfv CHANGELOG.md site/changelog.md
@@ -92,17 +83,19 @@
 
 push: clean test docs ## Push to github
 	git add .
 	git commit -m "$m"
 	git push
 
 setup: clean test ## setup and build repo
-	pip install --pre --upgrade --force-reinstall --no-cache -rrequirements.txt
 	python setup.py sdist bdist_wheel bdist_egg
 	pip install -e .
 	twine upload dist/*
 
-release: clean test ## create executables for release
+compile: clean test ## compile application for distribution
 	pip install pyinstaller
 	pip install -e .
-	pyinstaller ./runner/execf.spec
-	@python -c "$$RENAME_FILE"
+	pyinstaller -F --name torrentfile --icon ./assets/torrentfile-icon.ico ./bin/torrentfile
+	pyinstaller --name torrentfile --icon ./assets/torrentfile-icon.ico ./bin/torrentfile
+	7z a ./torrentfile-windows-exec.zip ./dist/torrentfile.exe
+	7z a ./torrentfile-windows-dir.zip ./dist/torrentfile
+	python -c "$$RENAME_FILE"
```

### Comparing `torrentfile-0.8.8/assets/Torrentfile.gif` & `torrentfile-0.9.0/assets/Torrentfile.gif`

 * *Files identical despite different names*

### Comparing `torrentfile-0.8.8/assets/torrentfile-icon.ico` & `torrentfile-0.9.0/assets/torrentfile-icon.ico`

 * *Files identical despite different names*

### Comparing `torrentfile-0.8.8/assets/torrentfile-icon.png` & `torrentfile-0.9.0/assets/torrentfile-icon.png`

 * *Files identical despite different names*

### Comparing `torrentfile-0.8.8/assets/torrentfile.png` & `torrentfile-0.9.0/assets/torrentfile.png`

 * *Files identical despite different names*

### Comparing `torrentfile-0.8.8/c/hasher.c` & `torrentfile-0.9.0/c/hasher.c`

 * *Files identical despite different names*

### Comparing `torrentfile-0.8.8/c/hasher.h` & `torrentfile-0.9.0/c/hasher.h`

 * *Files identical despite different names*

### Comparing `torrentfile-0.8.8/c/sha.c` & `torrentfile-0.9.0/c/sha.c`

 * *Files identical despite different names*

### Comparing `torrentfile-0.8.8/c/sha.h` & `torrentfile-0.9.0/c/sha.h`

 * *Files identical despite different names*

### Comparing `torrentfile-0.8.8/pyproject.toml` & `torrentfile-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 requires = ["setuptools>=40.8.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "torrentfile"
 authors = [{name = "alexpdev", email = "alexpdev@pm.me"}]
 description = "Terminal based command line tool for creating Bittorrent files."
-license = {file = "LICENSE"}
-version = "0.8.8"
+version = "0.9.0"
 readme = "README.md"
 requires-python = ">=3.6"
-keywords = ["Bittorrent", "torrent", "bittorrent-metafiles", "CLI"]
+keywords = ["Bittorrent", "torrent", "bittorrent-metafiles", "CLI", "torrentfile"]
 classifiers = [
     "Environment :: Console",
     "Development Status :: 4 - Beta",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
     "Intended Audience :: End Users/Desktop",
     "Intended Audience :: Developers",
     "Topic :: Utilities",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: Apache Software License",
 ]
@@ -73,15 +73,16 @@
     "W0108",
     "W0106",
     "redefined-outer-name",
     "attribute-defined-outside-init",
     "invalid-name",
     "not-callable",
     "consider-using-with",
-    "implicit-str-concat"
+    "implicit-str-concat",
+    "no-member"
 ]
 
 [tool.pylint. 'VARIABLES']
 callbacks = ["cb_", "_cb", "hook_"]
 
 [tool.pylint. 'FORMAT']
 max-line-length = 80
@@ -96,7 +97,13 @@
 max-args=15
 min-public-methods=0
 max-attributes=20
 max-statements=75
 max-branches=20
 min-similarity-lines=4
 max-locals=25
+
+[tool.isort]
+multi_line_output = 4
+length_sort_straight = true
+line_length = 80
+wrap_length = 79
```

### Comparing `torrentfile-0.8.8/setup.py` & `torrentfile-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `torrentfile-0.8.8/tests/test_cli.py` & `torrentfile-0.9.0/tests/test_cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,624 +1,647 @@
-#! /usr/bin/python3
-# -*- coding: utf-8 -*-
-
-##############################################################################
-#    Copyright (C) 2021-current alexpdev
-#
-#    Licensed under the Apache License, Version 2.0 (the "License");
-#    you may not use this file except in compliance with the License.
-#    You may obtain a copy of the License at
-#
-#        http://www.apache.org/licenses/LICENSE-2.0
-#
-#    Unless required by applicable law or agreed to in writing, software
-#    distributed under the License is distributed on an "AS IS" BASIS,
-#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#    See the License for the specific language governing permissions and
-#    limitations under the License.
-##############################################################################
-"""
-Testing functions for the command line interface.
-"""
-
-import datetime
-import os
-import sys
-
-import pyben
-import pytest
-
-from tests import dir1, dir2, file1, filemeta1, metafile1, rmpath, tempfile
-from torrentfile import execute
-from torrentfile.__main__ import main
-
-
-def test_fix():
-    """
-    Test dir1 fixture is not None.
-    """
-    assert dir1 and dir2 and metafile1 and filemeta1 and file1
-
-
-@pytest.fixture()
-def folder(dir1):
-    """
-    Yield a folder object as fixture.
-    """
-    sfolder = str(dir1)
-    torrent = sfolder + ".torrent"
-    yield (sfolder, torrent)
-    rmpath(torrent)
-
-
-def test_cli_v1(folder):
-    """
-    Basic create torrent cli command.
-    """
-    folder, torrent = folder
-    args = ["torrentfile", "create", folder, "-o", torrent]
-    sys.argv = args
-    execute()
-    assert os.path.exists(torrent)
-
-
-def test_cli_v2(folder):
-    """
-    Create torrent v2 cli command.
-    """
-    folder, torrent = folder
-    args = [
-        "torrentfile",
-        "create",
-        folder,
-        "--meta-version",
-        "2",
-        "-o",
-        torrent,
-    ]
-    sys.argv = args
-    execute()
-    assert os.path.exists(torrent)
-
-
-def test_cli_v3(folder):
-    """
-    Create hybrid torrent cli command.
-    """
-    folder, torrent = folder
-    args = [
-        "torrentfile",
-        "create",
-        folder,
-        "--meta-version",
-        "3",
-        "-o",
-        torrent,
-    ]
-    sys.argv = args
-    execute()
-    assert os.path.exists(torrent)
-
-
-def test_cli_private(folder):
-    """
-    Test private cli flag.
-    """
-    folder, torrent = folder
-    args = ["torrentfile", "create", folder, "--private", "-o", torrent]
-    sys.argv = args
-    main()
-    meta = pyben.load(torrent)
-    assert "private" in meta["info"]
-
-
-@pytest.mark.parametrize("piece_length", [2**exp for exp in range(14, 21)])
-@pytest.mark.parametrize("version", ["1", "2", "3"])
-def test_cli_piece_length(folder, piece_length, version):
-    """
-    Test piece length cli flag.
-    """
-    folder, torrent = folder
-    args = [
-        "torrentfile",
-        "-v",
-        "create",
-        folder,
-        "--piece-length",
-        str(piece_length),
-        "--meta-version",
-        version,
-        "--progress",
-        "0",
-        "-o",
-        torrent,
-    ]
-    sys.argv = args
-    execute()
-    meta = pyben.load(torrent)
-    assert meta["info"]["piece length"] == piece_length
-
-
-@pytest.mark.parametrize("piece_length", [2**exp for exp in range(14, 21)])
-@pytest.mark.parametrize("version", ["1", "2", "3"])
-def test_cli_announce(folder, piece_length, version):
-    """
-    Test announce cli flag.
-    """
-    folder, torrent = folder
-    args = [
-        "torrentfile",
-        "create",
-        folder,
-        "--piece-length",
-        str(piece_length),
-        "--meta-version",
-        version,
-        "--tracker",
-        "https://announce.org/tracker",
-        "-o",
-        torrent,
-    ]
-    sys.argv = args
-    execute()
-    meta = pyben.load(torrent)
-    assert meta["announce"] == "https://announce.org/tracker"
-
-
-@pytest.mark.parametrize("version", ["1", "2", "3"])
-def test_cli_announce_list(folder, version):
-    """
-    Test announce-list cli flag.
-    """
-    folder, torrent = folder
-    trackers = [
-        "https://announce.org/tracker",
-        "https://announce.net/tracker",
-        "https://tracker.net/announce",
-    ]
-    args = [
-        "torrentfile",
-        "create",
-        folder,
-        "--meta-version",
-        version,
-        "-o",
-        torrent,
-        "--tracker",
-    ] + trackers
-    sys.argv = args
-    execute()
-    meta = pyben.load(torrent)
-    for url in trackers:
-        assert url in [j for i in meta["announce-list"] for j in i]
-
-
-@pytest.mark.parametrize("piece_length", [2**exp for exp in range(14, 21)])
-@pytest.mark.parametrize("version", ["1", "2", "3"])
-def test_cli_comment(folder, piece_length, version):
-    """
-    Test comment cli flag.
-    """
-    folder, torrent = folder
-    args = [
-        "torrentfile",
-        "create",
-        folder,
-        "--piece-length",
-        str(piece_length),
-        "--meta-version",
-        version,
-        "--magnet",
-        "--comment",
-        "this is a comment",
-        "--progress",
-        "1",
-        "-o",
-        torrent,
-    ]
-    sys.argv = args
-    execute()
-    meta = pyben.load(torrent)
-    assert meta["info"]["comment"] == "this is a comment"
-
-
-@pytest.mark.parametrize("piece_length", [2**exp for exp in range(14, 21)])
-@pytest.mark.parametrize("version", ["1", "2", "3"])
-def test_cli_outfile(dir1, piece_length, version):
-    """
-    Test outfile cli flag.
-    """
-    outfile = dir1 + "test.torrent"
-    args = [
-        "torrentfile",
-        "create",
-        dir1,
-        "--piece-length",
-        str(piece_length),
-        "--meta-version",
-        version,
-        "-o",
-        outfile,
-        "--prog",
-        "1",
-    ]
-    sys.argv = args
-    execute()
-    assert os.path.exists(outfile)
-    rmpath(outfile)
-
-
-@pytest.mark.parametrize("piece_length", [2**exp for exp in range(14, 21)])
-@pytest.mark.parametrize("version", ["1", "2", "3"])
-def test_cli_creation_date(folder, piece_length, version):
-    """
-    Test if torrents created get an accurate timestamp.
-    """
-    folder, torrent = folder
-    args = [
-        "torrentfile",
-        "create",
-        folder,
-        "--piece-length",
-        str(piece_length),
-        "--meta-version",
-        version,
-        "--comment",
-        "this is a comment",
-        "-o",
-        torrent,
-    ]
-    sys.argv = args
-    execute()
-    meta = pyben.load(torrent)
-    num = float(meta["creation date"])
-    date = datetime.datetime.fromtimestamp(num)
-    now = datetime.datetime.now()
-    assert date.day == now.day
-    assert date.year == now.year
-    assert date.month == now.month
-
-
-@pytest.mark.parametrize("piece_length", [2**exp for exp in range(14, 21)])
-@pytest.mark.parametrize("version", ["1", "2", "3"])
-def test_cli_created_by(folder, piece_length, version):
-    """
-    Test if created torrents recieve a created by field in meta info.
-    """
-    folder, torrent = folder
-    args = [
-        "torrentfile",
-        "-q",
-        "create",
-        folder,
-        "--piece-length",
-        str(piece_length),
-        "--meta-version",
-        version,
-        "--comment",
-        "this is a comment",
-        "-o",
-        torrent,
-    ]
-    sys.argv = args
-    execute()
-    meta = pyben.load(torrent)
-    assert "TorrentFile" in meta["created by"]
-
-
-@pytest.mark.parametrize("piece_length", [2**exp for exp in range(14, 21)])
-@pytest.mark.parametrize("version", ["1", "2", "3"])
-def test_cli_web_seeds(folder, piece_length, version):
-    """
-    Test if created torrents recieve a web seeds field in meta info.
-    """
-    folder, torrent = folder
-    args = [
-        "torrentfile",
-        "create",
-        folder,
-        "--piece-length",
-        str(piece_length),
-        "--meta-version",
-        version,
-        "-w",
-        "https://webseed.url/1",
-        "https://webseed.url/2",
-        "https://webseed.url/3",
-        "-o",
-        torrent,
-    ]
-    sys.argv = args
-    execute()
-    meta = pyben.load(torrent)
-    assert "https://webseed.url/1" in meta["url-list"]
-
-
-@pytest.mark.parametrize("piece_length", [2**exp for exp in range(14, 21)])
-@pytest.mark.parametrize("version", ["1", "2", "3"])
-def test_cli_with_debug(folder, piece_length, version):
-    """
-    Test debug mode cli flag.
-    """
-    folder, torrent = folder
-    args = [
-        "torrentfile",
-        "-v",
-        "create",
-        folder,
-        "--piece-length",
-        str(piece_length),
-        "--meta-version",
-        version,
-        "--comment",
-        "this is a comment",
-        "-o",
-        torrent,
-    ]
-    sys.argv = args
-    execute()
-    assert os.path.exists(torrent)
-
-
-@pytest.mark.parametrize("piece_length", [2**exp for exp in range(14, 21)])
-@pytest.mark.parametrize("version", ["1", "2", "3"])
-def test_cli_with_source(folder, piece_length, version):
-    """
-    Test source cli flag.
-    """
-    folder, torrent = folder
-    args = [
-        "torrentfile",
-        "create",
-        folder,
-        "--piece-length",
-        str(piece_length),
-        "--meta-version",
-        version,
-        "--source",
-        "somesource",
-        "-o",
-        torrent,
-    ]
-    sys.argv = args
-    execute()
-    meta = pyben.load(torrent)
-    assert meta["info"]["source"] == "somesource"
-
-
-def test_cli_help():
-    """
-    Test showing help notice cli flag.
-    """
-    args = ["-h"]
-    sys.argv = args
-    try:
-        assert execute()
-    except SystemExit:
-        assert True
-
-
-@pytest.mark.parametrize("version", ["1", "2", "3"])
-@pytest.mark.parametrize("progress", ["0", "1"])
-def test_cli_empty_files(dir2, version, progress):
-    """
-    Test creating torrent with empty files.
-    """
-    outfile = str(dir2) + ".torrent"
-    args = [
-        "torrentfile",
-        "create",
-        str(dir2),
-        "--meta-version",
-        version,
-        "--source",
-        "somesource",
-        "--prog",
-        progress,
-        "-o",
-        outfile,
-    ]
-    sys.argv = args
-
-    def walk(root, count):
-        """
-        Traverse directory to edit files.
-        """
-        if root.is_file():
-            with open(root, "wb") as _:
-                return 1
-        elif root.is_dir():
-            for item in root.iterdir():
-                if count >= 2:
-                    break
-                count += walk(item, count)
-        return count
-
-    walk(dir2, 0)
-    execute()
-    assert os.path.exists(outfile)
-    rmpath(outfile)
-
-
-@pytest.mark.parametrize("ending", ["/", "\\"])
-def test_cli_slash_path(dir1, ending):
-    """
-    Test if output when path ends with a /.
-    """
-    outfile = str(dir1) + ".torrent"
-    if sys.platform != "win32" and ending == "\\":  # pragma: nocover
-        ending = "/"
-    args = [
-        "torrentfile",
-        "create",
-        "-o",
-        outfile,
-        "-t",
-        "https://announce1.org",
-        "--private",
-        str(dir1) + ending,
-    ]
-    sys.argv = args
-    execute()
-    assert os.path.exists(outfile)
-    rmpath(outfile)
-
-
-@pytest.mark.parametrize("sep", ["/", "\\"])
-def test_cli_slash_outpath(dir1, sep):
-    """
-    Test if output when outpath ends with a /.
-    """
-    if sys.platform != "win32":
-        sep = "/"  # pragma: nocover
-    parent = os.path.dirname(dir1) + sep
-    args = [
-        "torrentfile",
-        "create",
-        "-t",
-        "https://announce1.org",
-        "--private",
-        "-o",
-        parent,
-        str(dir1),
-    ]
-    sys.argv = args
-    execute()
-    outfile = str(dir1) + ".torrent"
-    assert os.path.exists(outfile)
-    rmpath(outfile)
-
-
-@pytest.mark.parametrize(
-    "flag", ["-t", "-w", "--announce", "--web-seed", "--http-seed"]
-)
-def test_cli_announce_path(dir1, flag):
-    """
-    Test CLI when path is placed after the trackers flag.
-    """
-    outfile = str(dir1) + ".torrent"
-    args = [
-        "torrentfile",
-        "create",
-        "-o",
-        outfile,
-        flag,
-        "https://announce1.org",
-        str(dir1),
-    ]
-    sys.argv = args
-    execute()
-    assert os.path.exists(outfile)
-    rmpath(outfile)
-
-
-def test_cli_cwd(folder):
-    """
-    Test outfile cli flag.
-    """
-    folder, _ = folder
-    args = [
-        "torrentfile",
-        "create",
-        "--cwd",
-        folder,
-    ]
-    sys.argv = args
-    current = os.getcwd()
-    name = os.path.basename(folder)
-    outfile = os.path.join(current, name) + ".torrent"
-    execute()
-    assert os.path.exists(outfile)
-    rmpath(outfile)
-
-
-@pytest.fixture()
-def build(dir2):
-    """Fixture for testing the build subcommand."""
-    dest = os.path.join(os.path.dirname(__file__), "dest")
-    if os.path.exists(dest):
-        rmpath(dest)
-        try:
-            os.makedirs(dest)
-        except FileExistsError:  # pragma: nocover
-            rmpath(dest)
-    return os.path.dirname(dir2), dest, dir2
-
-
-@pytest.mark.parametrize("size", list(range(15, 19)))
-@pytest.mark.parametrize("version", [1, 2])
-def test_rebuild_subcommand(build, version, size):
-    """Test the rebuild CLI subcommand."""
-    basedir, dest, content = build
-    args = [
-        "torrentfile",
-        "create",
-        str(content),
-        "--meta-version",
-        str(version),
-        "--piece-length",
-        str(size),
-        "-o",
-        str(content) + ".torrent",
-    ]
-    sys.argv = args
-    execute()
-    args = ["torrentfile", "rebuild", "-m", basedir, "-c", basedir, "-d", dest]
-    sys.argv = args
-    counter = execute()
-    assert counter > 0
-
-
-def test_empty_maker(dir1):
-    """Test empty create cli."""
-    args = ["torrentfile", "create", dir1, "-o", dir1 + ".torrent"]
-    sys.argv = args
-    execute()
-    assert os.path.exists(dir1 + ".torrent")
-    rmpath(dir1 + ".torrent")
-
-
-def test_rename():
-    """Test the rename command."""
-    tfile = str(tempfile())
-    args = ["torrentfile", "create", tfile, "-o", tfile + ".torrent"]
-    sys.argv = args
-    execute()
-    assert os.path.exists(tfile + ".torrent")
-    parent = os.path.dirname(tfile)
-    temp_path = os.path.join(parent, "renamed.torrent")
-    os.rename(tfile + ".torrent", temp_path)
-    print(os.listdir(parent))
-    args = ["torrentfile", "rename", temp_path]
-    sys.argv = args
-    execute()
-    assert os.path.exists(tfile + ".torrent")
-    assert not os.path.exists(temp_path)
-    rmpath(tfile + ".torrent", tfile)
-
-
-@pytest.mark.parametrize("version", ["1", "2", "3"])
-def test_cli_default_command(folder, version):
-    """Test default command by ommitting command."""
-    folder, torrent = folder
-    args = [
-        "torrentfile",
-        "-q",
-        folder,
-        "--meta-version",
-        version,
-        "-o",
-        torrent,
-    ]
-    sys.argv = args
-    execute()
-    assert os.path.exists(torrent)
-
-
-def test_cli_configfile(folder):
-    """Test config cli parameter."""
-    args = ["torrentfile", "create", "--config", folder]
-    sys.argv = args
-    try:
-        execute()
-    except FileNotFoundError:
-        assert True
+#! /usr/bin/python3
+# -*- coding: utf-8 -*-
+
+##############################################################################
+#    Copyright (C) 2021-current alexpdev
+#
+#    Licensed under the Apache License, Version 2.0 (the "License");
+#    you may not use this file except in compliance with the License.
+#    You may obtain a copy of the License at
+#
+#        http://www.apache.org/licenses/LICENSE-2.0
+#
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS,
+#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#    See the License for the specific language governing permissions and
+#    limitations under the License.
+##############################################################################
+"""
+Testing functions for the command line interface.
+"""
+
+import os
+import sys
+import datetime
+import textwrap
+
+import pyben
+import pytest
+
+from tests import dir1, dir2, file1, filemeta1, metafile1, rmpath, tempfile
+from torrentfile import execute
+from torrentfile.__main__ import main
+
+
+def test_fix():
+    """
+    Test dir1 fixture is not None.
+    """
+    assert dir1 and dir2 and metafile1 and filemeta1 and file1
+
+
+@pytest.fixture()
+def folder(dir1):
+    """
+    Yield a folder object as fixture.
+    """
+    sfolder = str(dir1)
+    torrent = sfolder + ".torrent"
+    yield (sfolder, torrent)
+    rmpath(torrent)
+
+
+def test_cli_v1(folder):
+    """
+    Basic create torrent cli command.
+    """
+    folder, torrent = folder
+    args = ["torrentfile", "create", folder, "-o", torrent]
+    sys.argv = args
+    execute()
+    assert os.path.exists(torrent)
+
+
+def test_cli_v2(folder):
+    """
+    Create torrent v2 cli command.
+    """
+    folder, torrent = folder
+    args = [
+        "torrentfile",
+        "create",
+        folder,
+        "--meta-version",
+        "2",
+        "-o",
+        torrent,
+    ]
+    sys.argv = args
+    execute()
+    assert os.path.exists(torrent)
+
+
+def test_cli_v3(folder):
+    """
+    Create hybrid torrent cli command.
+    """
+    folder, torrent = folder
+    args = [
+        "torrentfile",
+        "create",
+        folder,
+        "--meta-version",
+        "3",
+        "-o",
+        torrent,
+    ]
+    sys.argv = args
+    execute()
+    assert os.path.exists(torrent)
+
+
+def test_cli_private(folder):
+    """
+    Test private cli flag.
+    """
+    folder, torrent = folder
+    args = ["torrentfile", "create", folder, "--private", "-o", torrent]
+    sys.argv = args
+    main()
+    meta = pyben.load(torrent)
+    assert "private" in meta["info"]
+
+
+@pytest.mark.parametrize("piece_length", [2**exp for exp in range(14, 21)])
+@pytest.mark.parametrize("version", ["1", "2", "3"])
+def test_cli_piece_length(folder, piece_length, version):
+    """
+    Test piece length cli flag.
+    """
+    folder, torrent = folder
+    args = [
+        "torrentfile",
+        "-v",
+        "create",
+        folder,
+        "--piece-length",
+        str(piece_length),
+        "--meta-version",
+        version,
+        "--progress",
+        "0",
+        "-o",
+        torrent,
+    ]
+    sys.argv = args
+    execute()
+    meta = pyben.load(torrent)
+    assert meta["info"]["piece length"] == piece_length
+
+
+@pytest.mark.parametrize("piece_length", [2**exp for exp in range(14, 21)])
+@pytest.mark.parametrize("version", ["1", "2", "3"])
+def test_cli_announce(folder, piece_length, version):
+    """
+    Test announce cli flag.
+    """
+    folder, torrent = folder
+    args = [
+        "torrentfile",
+        "create",
+        folder,
+        "--piece-length",
+        str(piece_length),
+        "--meta-version",
+        version,
+        "--tracker",
+        "https://announce.org/tracker",
+        "-o",
+        torrent,
+    ]
+    sys.argv = args
+    execute()
+    meta = pyben.load(torrent)
+    assert meta["announce"] == "https://announce.org/tracker"
+
+
+@pytest.mark.parametrize("version", ["1", "2", "3"])
+def test_cli_announce_list(folder, version):
+    """
+    Test announce-list cli flag.
+    """
+    folder, torrent = folder
+    trackers = [
+        "https://announce.org/tracker",
+        "https://announce.net/tracker",
+        "https://tracker.net/announce",
+    ]
+    args = [
+        "torrentfile",
+        "create",
+        folder,
+        "--meta-version",
+        version,
+        "-o",
+        torrent,
+        "--tracker",
+    ] + trackers
+    sys.argv = args
+    execute()
+    meta = pyben.load(torrent)
+    for url in trackers:
+        assert url in [j for i in meta["announce-list"] for j in i]
+
+
+@pytest.mark.parametrize("piece_length", [2**exp for exp in range(14, 21)])
+@pytest.mark.parametrize("version", ["1", "2", "3"])
+def test_cli_comment(folder, piece_length, version):
+    """
+    Test comment cli flag.
+    """
+    folder, torrent = folder
+    args = [
+        "torrentfile",
+        "create",
+        folder,
+        "--piece-length",
+        str(piece_length),
+        "--meta-version",
+        version,
+        "--magnet",
+        "--comment",
+        "this is a comment",
+        "--progress",
+        "1",
+        "-o",
+        torrent,
+    ]
+    sys.argv = args
+    execute()
+    meta = pyben.load(torrent)
+    assert meta["info"]["comment"] == "this is a comment"
+
+
+@pytest.mark.parametrize("piece_length", [2**exp for exp in range(14, 21)])
+@pytest.mark.parametrize("version", ["1", "2", "3"])
+def test_cli_outfile(dir1, piece_length, version):
+    """
+    Test outfile cli flag.
+    """
+    outfile = dir1 + "test.torrent"
+    args = [
+        "torrentfile",
+        "create",
+        dir1,
+        "--piece-length",
+        str(piece_length),
+        "--meta-version",
+        version,
+        "-o",
+        outfile,
+        "--prog",
+        "1",
+    ]
+    sys.argv = args
+    execute()
+    assert os.path.exists(outfile)
+    rmpath(outfile)
+
+
+@pytest.mark.parametrize("piece_length", [2**exp for exp in range(14, 21)])
+@pytest.mark.parametrize("version", ["1", "2", "3"])
+def test_cli_creation_date(folder, piece_length, version):
+    """
+    Test if torrents created get an accurate timestamp.
+    """
+    folder, torrent = folder
+    args = [
+        "torrentfile",
+        "create",
+        folder,
+        "--piece-length",
+        str(piece_length),
+        "--meta-version",
+        version,
+        "--comment",
+        "this is a comment",
+        "-o",
+        torrent,
+    ]
+    sys.argv = args
+    execute()
+    meta = pyben.load(torrent)
+    num = float(meta["creation date"])
+    date = datetime.datetime.fromtimestamp(num)
+    now = datetime.datetime.now()
+    assert date.day == now.day
+    assert date.year == now.year
+    assert date.month == now.month
+
+
+@pytest.mark.parametrize("piece_length", [2**exp for exp in range(14, 21)])
+@pytest.mark.parametrize("version", ["1", "2", "3"])
+def test_cli_created_by(folder, piece_length, version):
+    """
+    Test if created torrents recieve a created by field in meta info.
+    """
+    folder, torrent = folder
+    args = [
+        "torrentfile",
+        "-q",
+        "create",
+        folder,
+        "--piece-length",
+        str(piece_length),
+        "--meta-version",
+        version,
+        "--comment",
+        "this is a comment",
+        "-o",
+        torrent,
+    ]
+    sys.argv = args
+    execute()
+    meta = pyben.load(torrent)
+    assert "TorrentFile" in meta["created by"]
+
+
+@pytest.mark.parametrize("piece_length", [2**exp for exp in range(14, 21)])
+@pytest.mark.parametrize("version", ["1", "2", "3"])
+def test_cli_web_seeds(folder, piece_length, version):
+    """
+    Test if created torrents recieve a web seeds field in meta info.
+    """
+    folder, torrent = folder
+    args = [
+        "torrentfile",
+        "create",
+        folder,
+        "--piece-length",
+        str(piece_length),
+        "--meta-version",
+        version,
+        "-w",
+        "https://webseed.url/1",
+        "https://webseed.url/2",
+        "https://webseed.url/3",
+        "-o",
+        torrent,
+    ]
+    sys.argv = args
+    execute()
+    meta = pyben.load(torrent)
+    assert "https://webseed.url/1" in meta["url-list"]
+
+
+@pytest.mark.parametrize("piece_length", [2**exp for exp in range(14, 21)])
+@pytest.mark.parametrize("version", ["1", "2", "3"])
+def test_cli_with_debug(folder, piece_length, version):
+    """
+    Test debug mode cli flag.
+    """
+    folder, torrent = folder
+    args = [
+        "torrentfile",
+        "-v",
+        "create",
+        folder,
+        "--piece-length",
+        str(piece_length),
+        "--meta-version",
+        version,
+        "--comment",
+        "this is a comment",
+        "-o",
+        torrent,
+    ]
+    sys.argv = args
+    execute()
+    assert os.path.exists(torrent)
+
+
+@pytest.mark.parametrize("piece_length", [2**exp for exp in range(14, 21)])
+@pytest.mark.parametrize("version", ["1", "2", "3"])
+def test_cli_with_source(folder, piece_length, version):
+    """
+    Test source cli flag.
+    """
+    folder, torrent = folder
+    args = [
+        "torrentfile",
+        "create",
+        folder,
+        "--piece-length",
+        str(piece_length),
+        "--meta-version",
+        version,
+        "--source",
+        "somesource",
+        "-o",
+        torrent,
+    ]
+    sys.argv = args
+    execute()
+    meta = pyben.load(torrent)
+    assert meta["info"]["source"] == "somesource"
+
+
+def test_cli_help():
+    """
+    Test showing help notice cli flag.
+    """
+    args = ["-h"]
+    sys.argv = args
+    try:
+        assert execute()
+    except SystemExit:
+        assert True
+
+
+@pytest.mark.parametrize("version", ["1", "2", "3"])
+@pytest.mark.parametrize("progress", ["0", "1"])
+def test_cli_empty_files(dir2, version, progress):
+    """
+    Test creating torrent with empty files.
+    """
+    outfile = str(dir2) + ".torrent"
+    args = [
+        "torrentfile",
+        "create",
+        str(dir2),
+        "--meta-version",
+        version,
+        "--source",
+        "somesource",
+        "--prog",
+        progress,
+        "-o",
+        outfile,
+    ]
+    sys.argv = args
+
+    def walk(root, count):
+        """
+        Traverse directory to edit files.
+        """
+        if root.is_file():
+            with open(root, "wb") as _:
+                return 1
+        elif root.is_dir():
+            for item in root.iterdir():
+                if count >= 2:
+                    break
+                count += walk(item, count)
+        return count
+
+    walk(dir2, 0)
+    execute()
+    assert os.path.exists(outfile)
+    rmpath(outfile)
+
+
+@pytest.mark.parametrize("ending", ["/", "\\"])
+def test_cli_slash_path(dir1, ending):
+    """
+    Test if output when path ends with a /.
+    """
+    outfile = str(dir1) + ".torrent"
+    if sys.platform != "win32" and ending == "\\":  # pragma: nocover
+        ending = "/"
+    args = [
+        "torrentfile",
+        "create",
+        "-o",
+        outfile,
+        "-t",
+        "https://announce1.org",
+        "--private",
+        str(dir1) + ending,
+    ]
+    sys.argv = args
+    execute()
+    assert os.path.exists(outfile)
+    rmpath(outfile)
+
+
+@pytest.mark.parametrize("sep", ["/", "\\"])
+def test_cli_slash_outpath(dir1, sep):
+    """
+    Test if output when outpath ends with a /.
+    """
+    if sys.platform != "win32":
+        sep = "/"  # pragma: nocover
+    parent = os.path.dirname(dir1) + sep
+    args = [
+        "torrentfile",
+        "create",
+        "-t",
+        "https://announce1.org",
+        "--private",
+        "-o",
+        parent,
+        str(dir1),
+    ]
+    sys.argv = args
+    execute()
+    outfile = str(dir1) + ".torrent"
+    assert os.path.exists(outfile)
+    rmpath(outfile)
+
+
+@pytest.mark.parametrize(
+    "flag", ["-t", "-w", "--announce", "--web-seed", "--http-seed"])
+def test_cli_announce_path(dir1, flag):
+    """
+    Test CLI when path is placed after the trackers flag.
+    """
+    outfile = str(dir1) + ".torrent"
+    args = [
+        "torrentfile",
+        "create",
+        "-o",
+        outfile,
+        flag,
+        "https://announce1.org",
+        str(dir1),
+    ]
+    sys.argv = args
+    execute()
+    assert os.path.exists(outfile)
+    rmpath(outfile)
+
+
+@pytest.fixture()
+def build(dir2):
+    """Fixture for testing the build subcommand."""
+    dest = os.path.join(os.path.dirname(__file__), "dest")
+    if os.path.exists(dest):
+        rmpath(dest)
+        try:
+            os.makedirs(dest)
+        except FileExistsError:  # pragma: nocover
+            rmpath(dest)
+    return os.path.dirname(dir2), dest, dir2
+
+
+@pytest.mark.parametrize("size", list(range(15, 19)))
+@pytest.mark.parametrize("version", [1, 2])
+def test_rebuild_subcommand(build, version, size):
+    """Test the rebuild CLI subcommand."""
+    basedir, dest, content = build
+    args = [
+        "torrentfile",
+        "create",
+        str(content),
+        "--meta-version",
+        str(version),
+        "--piece-length",
+        str(size),
+        "-o",
+        str(content) + ".torrent",
+    ]
+    sys.argv = args
+    execute()
+    args = ["torrentfile", "rebuild", "-m", basedir, "-c", basedir, "-d", dest]
+    sys.argv = args
+    counter = execute()
+    assert counter > 0
+
+
+def test_empty_maker(dir1):
+    """Test empty create cli."""
+    args = ["torrentfile", "create", dir1, "-o", dir1 + ".torrent"]
+    sys.argv = args
+    execute()
+    assert os.path.exists(dir1 + ".torrent")
+    rmpath(dir1 + ".torrent")
+
+
+def test_rename():
+    """Test the rename command."""
+    tfile = str(tempfile())
+    args = ["torrentfile", "create", tfile, "-o", tfile + ".torrent"]
+    sys.argv = args
+    execute()
+    assert os.path.exists(tfile + ".torrent")
+    parent = os.path.dirname(tfile)
+    temp_path = os.path.join(parent, "renamed.torrent")
+    os.rename(tfile + ".torrent", temp_path)
+    print(os.listdir(parent))
+    args = ["torrentfile", "rename", temp_path]
+    sys.argv = args
+    execute()
+    assert os.path.exists(tfile + ".torrent")
+    assert not os.path.exists(temp_path)
+    rmpath(tfile + ".torrent", tfile)
+
+
+@pytest.mark.parametrize("version", ["1", "2", "3"])
+def test_cli_default_command(folder, version):
+    """Test default command by ommitting command."""
+    folder, torrent = folder
+    args = [
+        "torrentfile",
+        "-q",
+        folder,
+        "--meta-version",
+        version,
+        "-o",
+        torrent,
+    ]
+    sys.argv = args
+    execute()
+    assert os.path.exists(torrent)
+
+
+def test_cli_configfile(folder):
+    """Test config cli parameter."""
+    folder, _ = folder
+    args = ["torrentfile", "create", "--config", folder]
+    sys.argv = args
+    try:
+        execute()
+    except FileNotFoundError:
+        assert True
+
+
+@pytest.fixture
+def configfile():
+    """Test fixture for the configfile parameter."""
+    config = """
+    [config]
+    meta-version = 3
+    piece-length = 15
+    announce = example
+    private = true
+    source = example
+    comment = comment example
+    """
+    path = os.path.join(os.path.dirname(__file__), "torrentfile.ini")
+    with open(path, "wt", encoding="utf8") as fd:
+        fd.write(textwrap.dedent(config))
+    yield path
+    rmpath(path)
+
+
+def test_cli_configfile_params(configfile, folder):
+    """Testing parameters with config file option."""
+    folder, torrent = folder
+    args = [
+        "torrentfile",
+        "create",
+        "--config",
+        "--config-path",
+        configfile,
+        "-o",
+        torrent,
+        folder,
+    ]
+    sys.argv = args
+    execute()
+    meta = pyben.load(torrent)
+    assert meta["info"]["private"] == 1
+    assert meta["info"]["source"] == "example"
+    assert meta["info"]["piece length"] == 2**15
+    assert meta["announce"] == "example"
+    assert meta["info"]["meta version"] == 2
```

### Comparing `torrentfile-0.8.8/tests/test_edit.py` & `torrentfile-0.9.0/tests/test_edit.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,17 +33,17 @@
 def test_fix():
     """
     Testing dir fixtures.
     """
     assert dir2 and metafile2 and dir1
 
 
-@pytest.mark.parametrize(
-    "announce", [["urla"], ["urlb", "urlc"], ["urla", "urlb", "urlc"]]
-)
+@pytest.mark.parametrize("announce",
+                         [["urla"], ["urlb", "urlc"], ["urla", "urlb", "urlc"]]
+                         )
 def test_edit_torrent(metafile2, announce):
     """
     Test edit torrent with announce param.
     """
     edits = {"announce": announce}
     data = edit_torrent(metafile2, edits)
     meta = pyben.load(metafile2)
@@ -83,31 +83,31 @@
     edits = {"httpseeds": httpseeds}
     data = edit_torrent(metafile2, edits)
     meta = pyben.load(metafile2)
     assert data == meta
     assert data["httpseeds"] == httpseeds.split()
 
 
-@pytest.mark.parametrize(
-    "url_list", [["urla"], ["urlb", "urlc"], ["urla", "urlb", "urlc"]]
-)
+@pytest.mark.parametrize("url_list",
+                         [["urla"], ["urlb", "urlc"], ["urla", "urlb", "urlc"]]
+                         )
 def test_edit_urllist(metafile2, url_list):
     """
     Test edit torrent with webseed param as string.
     """
     edits = {"url-list": url_list}
     data = edit_torrent(metafile2, edits)
     meta = pyben.load(metafile2)
     assert data == meta
     assert data["url-list"] == url_list
 
 
-@pytest.mark.parametrize(
-    "httpseed", [["urla"], ["urlb", "urlc"], ["urla", "urlb", "urlc"]]
-)
+@pytest.mark.parametrize("httpseed",
+                         [["urla"], ["urlb", "urlc"], ["urla", "urlb", "urlc"]]
+                         )
 def test_edit_httpseeds(metafile2, httpseed):
     """
     Test edit torrent with webseed param as string.
     """
     edits = {"httpseeds": httpseed}
     data = edit_torrent(metafile2, edits)
     meta = pyben.load(metafile2)
```

### Comparing `torrentfile-0.8.8/tests/test_interactive.py` & `torrentfile-0.9.0/tests/test_interactive.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,189 +1,188 @@
-#! /usr/bin/python3
-# -*- coding: utf-8 -*-
-
-##############################################################################
-#    Copyright (C) 2021-current alexpdev
-#
-#    Licensed under the Apache License, Version 2.0 (the "License");
-#    you may not use this file except in compliance with the License.
-#    You may obtain a copy of the License at
-#
-#        http://www.apache.org/licenses/LICENSE-2.0
-#
-#    Unless required by applicable law or agreed to in writing, software
-#    distributed under the License is distributed on an "AS IS" BASIS,
-#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#    See the License for the specific language governing permissions and
-#    limitations under the License.
-##############################################################################
-"""
-Testing functions for the command line interface.
-"""
-
-import os
-
-import pyben
-import pytest
-
-from tests import file1, file2, filemeta2, torrents
-from torrentfile.interactive import select_action
-from torrentfile.utils import normalize_piece_length
-
-MOCK = "torrentfile.interactive.get_input"
-
-
-def test_fixtures():
-    """
-    Test the fixtures used in module.
-    """
-    assert filemeta2 and file1 and file2
-
-
-def test_interactive_create(monkeypatch, file1):
-    """
-    Test creating torrent interactively.
-    """
-    mapping = [
-        "create",
-        "",
-        "",
-        "",
-        "",
-        "",
-        "",
-        "",
-        file1,
-        str(file1) + ".torrent",
-        "",
-    ]
-    it = iter(mapping)
-    monkeypatch.setattr(MOCK, lambda *_: next(it))
-    select_action()
-    assert os.path.exists(str(file1) + ".torrent")
-
-
-@pytest.mark.parametrize("version", ["1", "2", "3"])
-@pytest.mark.parametrize("piece_length", ["23", "18", "131072"])
-@pytest.mark.parametrize("announce", ["url1", "urla urlb urlc"])
-@pytest.mark.parametrize("url_list", ["ftp url2", "ftp1 ftp2 ftp3"])
-@pytest.mark.parametrize("comment", ["Some Comment", "No Comment"])
-@pytest.mark.parametrize("source", ["Do", "Ra", "Me"])
-def test_inter_create_full(
-    file1,
-    piece_length,
-    announce,
-    comment,
-    source,
-    url_list,
-    version,
-    monkeypatch,
-):
-    """
-    Test creating torrent interactively with many parameters.
-    """
-    mapping = [
-        "create",
-        piece_length,
-        announce,
-        url_list,
-        url_list,
-        comment,
-        source,
-        "Y",
-        file1,
-        str(file1) + ".torrent",
-        version,
-    ]
-    it = iter(mapping)
-    monkeypatch.setattr(MOCK, lambda *_: next(it))
-    select_action()
-    meta = pyben.load(str(file1) + ".torrent")
-    assert meta["info"]["source"] == source
-    assert meta["info"]["piece length"] == normalize_piece_length(piece_length)
-    assert meta["info"]["comment"] == comment
-    assert meta["url-list"] == url_list.split()
-
-
-@pytest.mark.parametrize("announce", ["url1"])
-@pytest.mark.parametrize("url_list", ["ftp url2", "ftp1 ftp2 ftp3"])
-@pytest.mark.parametrize("comment", ["Some Comment", "No Comment"])
-@pytest.mark.parametrize("source", ["Fa", "So", "La"])
-def test_inter_edit_full(
-    filemeta2, announce, comment, source, url_list, monkeypatch
-):
-    """
-    Test editing torrent file interactively.
-    """
-    seq = [
-        "edit",
-        filemeta2,
-        "4",
-        announce,
-        "1",
-        comment,
-        "2",
-        source,
-        "5",
-        url_list,
-        "",
-        "6",
-        "Y",
-        "DONE",
-    ]
-    it = iter(seq)
-    monkeypatch.setattr(MOCK, lambda *_: next(it))
-    select_action()
-    meta1 = pyben.load(filemeta2)
-    assert meta1["info"]["source"] == source
-    assert meta1["info"]["comment"] == comment
-    assert meta1["url-list"] == url_list.split()
-    assert meta1["info"]["private"] == 1
-
-
-@pytest.mark.parametrize("announce", ["urla urlb urlc", "urld url2"])
-@pytest.mark.parametrize("urllist", ["ftp url2", "ftp1 ftp2 ftp3"])
-@pytest.mark.parametrize("cmnt", ["Some Comment"])
-@pytest.mark.parametrize("srce", ["Do", "Ra"])
-def test_inter_edit_cli(filemeta2, announce, cmnt, srce, urllist, monkeypatch):
-    """
-    Test editing torrent interactively from CLI.
-    """
-    seq = [
-        "edit",
-        filemeta2,
-        "4",
-        announce,
-        "1",
-        cmnt,
-        "2",
-        srce,
-        "5",
-        urllist,
-        urllist,
-        "6",
-        "Y",
-        "DONE",
-    ]
-    it = iter(seq)
-    monkeypatch.setattr(MOCK, lambda *_: next(it))
-    select_action()
-    meta2 = pyben.load(filemeta2)
-    assert meta2["info"]["source"] == srce
-    assert meta2["info"]["comment"] == cmnt
-    assert meta2["url-list"] == urllist.split()
-    assert meta2["info"]["private"] == 1
-
-
-@pytest.mark.parametrize("torrentclass", torrents())
-def test_inter_recheck(torrentclass, monkeypatch, file1):
-    """
-    Test interactive recheck function.
-    """
-    outpath = str(file1) + ".torrent"
-    torrent = torrentclass(path=file1, outfile=outpath)
-    filemeta, _ = torrent.write(outfile=outpath)
-    seq = ["recheck", filemeta, str(file1)]
-    it = iter(seq)
-    monkeypatch.setattr(MOCK, lambda *_: next(it))
-    result = select_action()
-    assert result == 100
+#! /usr/bin/python3
+# -*- coding: utf-8 -*-
+
+##############################################################################
+#    Copyright (C) 2021-current alexpdev
+#
+#    Licensed under the Apache License, Version 2.0 (the "License");
+#    you may not use this file except in compliance with the License.
+#    You may obtain a copy of the License at
+#
+#        http://www.apache.org/licenses/LICENSE-2.0
+#
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS,
+#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#    See the License for the specific language governing permissions and
+#    limitations under the License.
+##############################################################################
+"""
+Testing functions for the command line interface.
+"""
+
+import os
+
+import pyben
+import pytest
+
+from tests import file1, file2, filemeta2, torrents
+from torrentfile.interactive import select_action
+from torrentfile.utils import normalize_piece_length
+
+MOCK = "torrentfile.interactive.get_input"
+
+
+def test_fixtures():
+    """
+    Test the fixtures used in module.
+    """
+    assert filemeta2 and file1 and file2
+
+
+def test_interactive_create(monkeypatch, file1):
+    """
+    Test creating torrent interactively.
+    """
+    mapping = [
+        "create",
+        "",
+        "",
+        "",
+        "",
+        "",
+        "",
+        "",
+        file1,
+        str(file1) + ".torrent",
+        "",
+    ]
+    it = iter(mapping)
+    monkeypatch.setattr(MOCK, lambda *_: next(it))
+    select_action()
+    assert os.path.exists(str(file1) + ".torrent")
+
+
+@pytest.mark.parametrize("version", ["1", "2", "3"])
+@pytest.mark.parametrize("piece_length", ["23", "18", "131072"])
+@pytest.mark.parametrize("announce", ["url1", "urla urlb urlc"])
+@pytest.mark.parametrize("url_list", ["ftp url2", "ftp1 ftp2 ftp3"])
+@pytest.mark.parametrize("comment", ["Some Comment", "No Comment"])
+@pytest.mark.parametrize("source", ["Do", "Ra", "Me"])
+def test_inter_create_full(
+    file1,
+    piece_length,
+    announce,
+    comment,
+    source,
+    url_list,
+    version,
+    monkeypatch,
+):
+    """
+    Test creating torrent interactively with many parameters.
+    """
+    mapping = [
+        "create",
+        piece_length,
+        announce,
+        url_list,
+        url_list,
+        comment,
+        source,
+        "Y",
+        file1,
+        str(file1) + ".torrent",
+        version,
+    ]
+    it = iter(mapping)
+    monkeypatch.setattr(MOCK, lambda *_: next(it))
+    select_action()
+    meta = pyben.load(str(file1) + ".torrent")
+    assert meta["info"]["source"] == source
+    assert meta["info"]["piece length"] == normalize_piece_length(piece_length)
+    assert meta["info"]["comment"] == comment
+    assert meta["url-list"] == url_list.split()
+
+
+@pytest.mark.parametrize("announce", ["url1"])
+@pytest.mark.parametrize("url_list", ["ftp url2", "ftp1 ftp2 ftp3"])
+@pytest.mark.parametrize("comment", ["Some Comment", "No Comment"])
+@pytest.mark.parametrize("source", ["Fa", "So", "La"])
+def test_inter_edit_full(filemeta2, announce, comment, source, url_list,
+                         monkeypatch):
+    """
+    Test editing torrent file interactively.
+    """
+    seq = [
+        "edit",
+        filemeta2,
+        "4",
+        announce,
+        "1",
+        comment,
+        "2",
+        source,
+        "5",
+        url_list,
+        "",
+        "6",
+        "Y",
+        "DONE",
+    ]
+    it = iter(seq)
+    monkeypatch.setattr(MOCK, lambda *_: next(it))
+    select_action()
+    meta1 = pyben.load(filemeta2)
+    assert meta1["info"]["source"] == source
+    assert meta1["info"]["comment"] == comment
+    assert meta1["url-list"] == url_list.split()
+    assert meta1["info"]["private"] == 1
+
+
+@pytest.mark.parametrize("announce", ["urla urlb urlc", "urld url2"])
+@pytest.mark.parametrize("urllist", ["ftp url2", "ftp1 ftp2 ftp3"])
+@pytest.mark.parametrize("cmnt", ["Some Comment"])
+@pytest.mark.parametrize("srce", ["Do", "Ra"])
+def test_inter_edit_cli(filemeta2, announce, cmnt, srce, urllist, monkeypatch):
+    """
+    Test editing torrent interactively from CLI.
+    """
+    seq = [
+        "edit",
+        filemeta2,
+        "4",
+        announce,
+        "1",
+        cmnt,
+        "2",
+        srce,
+        "5",
+        urllist,
+        urllist,
+        "6",
+        "Y",
+        "DONE",
+    ]
+    it = iter(seq)
+    monkeypatch.setattr(MOCK, lambda *_: next(it))
+    select_action()
+    meta2 = pyben.load(filemeta2)
+    assert meta2["info"]["source"] == srce
+    assert meta2["info"]["comment"] == cmnt
+    assert meta2["url-list"] == urllist.split()
+    assert meta2["info"]["private"] == 1
+
+
+@pytest.mark.parametrize("torrentclass", torrents())
+def test_inter_recheck(torrentclass, monkeypatch, file1):
+    """
+    Test interactive recheck function.
+    """
+    outpath = str(file1) + ".torrent"
+    torrent = torrentclass(path=file1, outfile=outpath)
+    filemeta, _ = torrent.write(outfile=outpath)
+    seq = ["recheck", filemeta, str(file1)]
+    it = iter(seq)
+    monkeypatch.setattr(MOCK, lambda *_: next(it))
+    result = select_action()
+    assert result == 100
```

### Comparing `torrentfile-0.8.8/tests/test_rebuild.py` & `torrentfile-0.9.0/tests/test_rebuild.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     Test functionality of single file torrent and single torrent.
     """
     name = pyben.load(single2[0][0])["info"]["name"]
     contents = os.path.join(single2[1][0], name)
     with open(contents, "rb") as content:
         data = content.read()
     with open(contents, "wb") as content:
-        content.write(data[: len(data) // 2])
+        content.write(data[:len(data) // 2])
     assembler = Assembler(*single2)
     counter = assembler.assemble_torrents()
     assert counter == 0
 
 
 def test_wrong_path():
     """Test rebuild command with incorrect paths."""
```

### Comparing `torrentfile-0.8.8/tests/test_recheck.py` & `torrentfile-0.9.0/tests/test_recheck.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,17 @@
 Testing functions for the progress module.
 """
 
 import os
 import sys
 from pathlib import Path
 
-from tests import (dir1, dir2, file1, file2, filemeta1, filemeta2, metafile1,
-                   metafile2, rmpath, sizedfiles, sizes)
+from tests import (
+    dir1, dir2, file1, file2, filemeta1, filemeta2, metafile1, metafile2,
+    rmpath, sizedfiles, sizes)
 from torrentfile.cli import main_script as main
 from torrentfile.recheck import Checker
 from torrentfile.utils import ArgumentError
 
 
 def test_fixtures():
     """
@@ -107,15 +108,15 @@
     def shortenfile(path):
         """
         Shorten a few files for testing purposes.
         """
         with open(path, "rb") as bfile:
             data = bfile.read()
         with open(path, "wb") as bfile:
-            bfile.write(data[: -(2**10)])
+            bfile.write(data[:-(2**10)])
 
     for item in os.listdir(dir2):
         full = os.path.join(dir2, item)
         if os.path.isfile(full):
             shortenfile(full)
 
     testdir = os.path.dirname(dir2)
```

### Comparing `torrentfile-0.8.8/tests/test_torrent.py` & `torrentfile-0.9.0/tests/test_torrent.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
     """
     Test creating a torrent file from less than a single file contents.
     """
     tfile = tempfile(exp=sze)
     with open(tfile, "rb") as binfile:
         data = binfile.read()
     with open(tfile, "wb") as binfile:
-        binfile.write(data[: -(2**9)])
+        binfile.write(data[:-(2**9)])
     outfile = str(tfile) + ".torrent"
     kwargs = {
         "path": tfile,
         "comment": "somecomment",
         "announce": "announce",
         "piece_length": piecelength,
         "outfile": outfile,
@@ -232,11 +232,11 @@
 
 
 @pytest.mark.parametrize("params", [(10, 12), (10, 15), (20, 25), (28, 32)])
 def test_progress_bar(params):
     """Testing the prog mixin with various sizes."""
     increment, total = params
     progbar = ProgMixin()
-    progbar.prog_start(1 << total, "some/fake/path", unit="bytes")
+    progbar.prog_start(1 << total, "some/fake/path")
     while progbar.prog.state < total:
         progbar.prog_update(1 << increment)
     assert progbar.prog.state >= total
```

### Comparing `torrentfile-0.8.8/tests/test_utils.py` & `torrentfile-0.9.0/tests/test_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,262 +1,259 @@
-#! /usr/bin/python3
-# -*- coding: utf-8 -*-
-
-##############################################################################
-#    Copyright (C) 2021-current alexpdev
-#
-#    Licensed under the Apache License, Version 2.0 (the "License");
-#    you may not use this file except in compliance with the License.
-#    You may obtain a copy of the License at
-#
-#        http://www.apache.org/licenses/LICENSE-2.0
-#
-#    Unless required by applicable law or agreed to in writing, software
-#    distributed under the License is distributed on an "AS IS" BASIS,
-#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#    See the License for the specific language governing permissions and
-#    limitations under the License.
-##############################################################################
-"""
-Unittest functions for testing torrentfile utils module.
-"""
-import math
-
-import pytest
-
-from tests import dir1, dir2, rmpath
-from torrentfile import utils
-from torrentfile.__main__ import main
-
-
-def test_main_exists():
-    """
-    Test if main exists
-    """
-    assert main
-
-
-@pytest.mark.parametrize("size", [156634528, 2**30, 67987, 16384, 8563945])
-def test_get_piece_length(size):
-    """
-    Test function for best piece length for given size.
-    """
-    value = utils.get_piece_length(size)
-    assert value % 1024 == 0
-
-
-@pytest.mark.parametrize("size", [156634528, 2**30, 67987, 16384, 8563945])
-def test_get_piece_length_max(size):
-    """
-    Test function for best piece length for given size maximum.
-    """
-    value = utils.get_piece_length(size)
-    assert value < 2**27
-
-
-@pytest.mark.parametrize("size", [156634528, 2**30, 67987, 16384, 8563945])
-def test_get_piece_length_min(size):
-    """
-    Test function for best piece length for given size minimum.
-    """
-    value = utils.get_piece_length(size)
-    assert value >= 2**14
-
-
-def test_get_path_length_mod(dir1):
-    """
-    Test function for the best piece length for provided path.
-    """
-    assert utils.path_piece_length(dir1) % (2**14) == 0
-
-
-def test_get_path_length_min(dir1):
-    """
-    Test function for getting piece length for folders min.
-    """
-    assert utils.path_piece_length(dir1) >= (2**14)
-
-
-def test_get_path_length_max(dir1):
-    """
-    Test function for getting piece length for folders max.
-    """
-    assert utils.path_piece_length(dir1) <= (2**27)
-
-
-def test_path_stat(dir1):
-    """
-    Test function for acquiring piece length information on folder.
-    """
-    _, _, piece_length = utils.path_stat(dir1)
-    assert piece_length % (2**14) == 0
-
-
-def test_path_stat_size(dir1):
-    """
-    Test function for acquiring total size information on folder.
-    """
-    _, totalsize, _ = utils.path_stat(dir1)
-    assert totalsize == (2**18) * 8
-
-
-def test_path_stat_filelist_size(dir1):
-    """
-    Test function for acquiring file list information on folder.
-    """
-    filelist, _, _ = utils.path_stat(dir1)
-    assert len(filelist) == 8
-
-
-def test_get_filelist(dir1):
-    """
-    Test function for get a list of files in a directory.
-    """
-    filelist = utils.get_file_list(dir1)
-    assert len(filelist) == 8
-
-
-def test_get_path_size(dir1):
-    """
-    Test function for getting total size of directory.
-    """
-    pathsize = utils.path_size(dir1)
-    assert pathsize == (2**18) * 8
-
-
-def test_filelist_total(dir1):
-    """
-    Test function for acquiring a filelist for directory.
-    """
-    total, _ = utils.filelist_total(dir1)
-    assert total == (2**18) * 8
-
-
-def test_piecelength_error_fixtures():
-    """
-    Test exception for uninterpretable piece length value.
-    """
-    try:
-        raise utils.PieceLengthValueError("message")
-    except utils.PieceLengthValueError:
-        assert True
-        assert dir1
-
-
-def test_missing_path_error():
-    """
-    Test exception for missing path parameter.
-    """
-    try:
-        raise utils.MissingPathError("message")
-    except utils.MissingPathError:
-        assert True
-        assert dir2
-
-
-@pytest.mark.parametrize("value", [5, 32, 18, 225, 16384, 256000])
-def test_next_power_2(value):
-    """
-    Test next power of 2 function in utils module.
-    """
-    result = utils.next_power_2(value)
-    log = math.log2(result)
-    assert log == int(log)
-    assert result % 2 == 0
-    assert result >= value
-
-
-@pytest.mark.parametrize(
-    "amount, result",
-    [
-        (100, "100"),
-        (1100, "1 KiB"),
-        (1_100_000, "1 MiB"),
-        (1_100_000_000, "1 GiB"),
-        (4_400_120_000, "4 GiB"),
-        (4_000_120_000, "3 GiB"),
-    ],
-)
-def test_humanize_bytes(amount, result):
-    """
-    Test humanize bytes function.
-    """
-    assert utils.humanize_bytes(amount) == result
-
-
-@pytest.mark.parametrize(
-    "amount, result", [(i, 2**i) for i in range(14, 25)]
-)
-def test_normalize_piece_length_int(amount, result):
-    """Test normalize piece length function.
-
-    Parameters
-    ----------
-    amount : `str` or `int`
-        piece length or representation
-    result : int
-        expected output.
-    """
-    assert utils.normalize_piece_length(amount) == result
-
-
-@pytest.mark.parametrize(
-    "amount, result", [(str(i), 2**i) for i in range(14, 21)]
-)
-def test_normalize_piece_length_str(amount, result):
-    """Test normalize piece length function.
-
-    Parameters
-    ----------
-    amount : `str` or `int`
-        piece length or representation
-    result : int
-        expected output.
-    """
-    assert utils.normalize_piece_length(amount) == result
-
-
-@pytest.mark.parametrize(
-    "amount", ["hello", 11, 0, 100000, 28, "zero", "fifteen"]
-)
-def test_norm_plength_errors(amount):
-    """Test function to normalize piece length errors.
-
-    Parameters
-    ----------
-    amount : any
-        arguments intended to raise an exception.
-    """
-    try:
-        assert utils.normalize_piece_length(amount)
-    except utils.PieceLengthValueError:
-        assert True
-
-
-def test_filelisttotal_missing(dir2):
-    """Test function filelist total with missing path.
-
-    Parameters
-    ----------
-    dir2 : pytest.fixture
-        fixture containing a temporary directory
-    """
-    rmpath(dir2)
-    try:
-        utils.filelist_total(dir2)
-    except utils.MissingPathError:
-        assert True
-
-
-def test_argument_error():
-    """
-    Test Argument Error.
-
-    Raises
-    ------
-    utils.ArgumentError
-        Arg error
-    """
-    try:
-        raise utils.ArgumentError("This message raised by argument error")
-    except utils.ArgumentError:
-        assert True
+#! /usr/bin/python3
+# -*- coding: utf-8 -*-
+
+##############################################################################
+#    Copyright (C) 2021-current alexpdev
+#
+#    Licensed under the Apache License, Version 2.0 (the "License");
+#    you may not use this file except in compliance with the License.
+#    You may obtain a copy of the License at
+#
+#        http://www.apache.org/licenses/LICENSE-2.0
+#
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS,
+#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#    See the License for the specific language governing permissions and
+#    limitations under the License.
+##############################################################################
+"""
+Unittest functions for testing torrentfile utils module.
+"""
+import math
+
+import pytest
+
+from tests import dir1, dir2, rmpath
+from torrentfile import utils
+from torrentfile.__main__ import main
+
+
+def test_main_exists():
+    """
+    Test if main exists
+    """
+    assert main
+
+
+@pytest.mark.parametrize("size", [156634528, 2**30, 67987, 16384, 8563945])
+def test_get_piece_length(size):
+    """
+    Test function for best piece length for given size.
+    """
+    value = utils.get_piece_length(size)
+    assert value % 1024 == 0
+
+
+@pytest.mark.parametrize("size", [156634528, 2**30, 67987, 16384, 8563945])
+def test_get_piece_length_max(size):
+    """
+    Test function for best piece length for given size maximum.
+    """
+    value = utils.get_piece_length(size)
+    assert value < 2**27
+
+
+@pytest.mark.parametrize("size", [156634528, 2**30, 67987, 16384, 8563945])
+def test_get_piece_length_min(size):
+    """
+    Test function for best piece length for given size minimum.
+    """
+    value = utils.get_piece_length(size)
+    assert value >= 2**14
+
+
+def test_get_path_length_mod(dir1):
+    """
+    Test function for the best piece length for provided path.
+    """
+    assert utils.path_piece_length(dir1) % (2**14) == 0
+
+
+def test_get_path_length_min(dir1):
+    """
+    Test function for getting piece length for folders min.
+    """
+    assert utils.path_piece_length(dir1) >= (2**14)
+
+
+def test_get_path_length_max(dir1):
+    """
+    Test function for getting piece length for folders max.
+    """
+    assert utils.path_piece_length(dir1) <= (2**27)
+
+
+def test_path_stat(dir1):
+    """
+    Test function for acquiring piece length information on folder.
+    """
+    _, _, piece_length = utils.path_stat(dir1)
+    assert piece_length % (2**14) == 0
+
+
+def test_path_stat_size(dir1):
+    """
+    Test function for acquiring total size information on folder.
+    """
+    _, totalsize, _ = utils.path_stat(dir1)
+    assert totalsize == (2**18) * 8
+
+
+def test_path_stat_filelist_size(dir1):
+    """
+    Test function for acquiring file list information on folder.
+    """
+    filelist, _, _ = utils.path_stat(dir1)
+    assert len(filelist) == 8
+
+
+def test_get_filelist(dir1):
+    """
+    Test function for get a list of files in a directory.
+    """
+    filelist = utils.get_file_list(dir1)
+    assert len(filelist) == 8
+
+
+def test_get_path_size(dir1):
+    """
+    Test function for getting total size of directory.
+    """
+    pathsize = utils.path_size(dir1)
+    assert pathsize == (2**18) * 8
+
+
+def test_filelist_total(dir1):
+    """
+    Test function for acquiring a filelist for directory.
+    """
+    total, _ = utils.filelist_total(dir1)
+    assert total == (2**18) * 8
+
+
+def test_piecelength_error_fixtures():
+    """
+    Test exception for uninterpretable piece length value.
+    """
+    try:
+        raise utils.PieceLengthValueError("message")
+    except utils.PieceLengthValueError:
+        assert True
+        assert dir1
+
+
+def test_missing_path_error():
+    """
+    Test exception for missing path parameter.
+    """
+    try:
+        raise utils.MissingPathError("message")
+    except utils.MissingPathError:
+        assert True
+        assert dir2
+
+
+@pytest.mark.parametrize("value", [5, 32, 18, 225, 16384, 256000])
+def test_next_power_2(value):
+    """
+    Test next power of 2 function in utils module.
+    """
+    result = utils.next_power_2(value)
+    log = math.log2(result)
+    assert log == int(log)
+    assert result % 2 == 0
+    assert result >= value
+
+
+@pytest.mark.parametrize(
+    "amount, result",
+    [
+        (1, f"{float(1)} Byte"),
+        (100, "100.0 Bytes"),
+        (1100, "1.1 KiB"),
+        (1_100_000, "1.0 MiB"),
+        (1_100_000_000, "1.0 GiB"),
+        (4_400_120_000, "4.1 GiB"),
+        (4_000_120_000, "3.7 GiB"),
+    ],
+)
+def test_humanize_bytes(amount, result):
+    """
+    Test humanize bytes function.
+    """
+    assert utils.humanize_bytes(amount) == result
+
+
+@pytest.mark.parametrize("amount, result", [(i, 2**i) for i in range(14, 25)])
+def test_normalize_piece_length_int(amount, result):
+    """Test normalize piece length function.
+
+    Parameters
+    ----------
+    amount : `str` or `int`
+        piece length or representation
+    result : int
+        expected output.
+    """
+    assert utils.normalize_piece_length(amount) == result
+
+
+@pytest.mark.parametrize("amount, result",
+                         [(str(i), 2**i) for i in range(14, 21)])
+def test_normalize_piece_length_str(amount, result):
+    """Test normalize piece length function.
+
+    Parameters
+    ----------
+    amount : `str` or `int`
+        piece length or representation
+    result : int
+        expected output.
+    """
+    assert utils.normalize_piece_length(amount) == result
+
+
+@pytest.mark.parametrize("amount",
+                         ["hello", 11, 0, 100000, 28, "zero", "fifteen"])
+def test_norm_plength_errors(amount):
+    """Test function to normalize piece length errors.
+
+    Parameters
+    ----------
+    amount : any
+        arguments intended to raise an exception.
+    """
+    try:
+        assert utils.normalize_piece_length(amount)
+    except utils.PieceLengthValueError:
+        assert True
+
+
+def test_filelisttotal_missing(dir2):
+    """Test function filelist total with missing path.
+
+    Parameters
+    ----------
+    dir2 : pytest.fixture
+        fixture containing a temporary directory
+    """
+    rmpath(dir2)
+    try:
+        utils.filelist_total(dir2)
+    except utils.MissingPathError:
+        assert True
+
+
+def test_argument_error():
+    """
+    Test Argument Error.
+
+    Raises
+    ------
+    utils.ArgumentError
+        Arg error
+    """
+    try:
+        raise utils.ArgumentError("This message raised by argument error")
+    except utils.ArgumentError:
+        assert True
```

### Comparing `torrentfile-0.8.8/torrentfile/__init__.py` & `torrentfile-0.9.0/torrentfile/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,24 +15,16 @@
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 ##############################################################################
 """
 Torrentfile can create Bittorrent metafiles for any content.
 
-Both Bittorrent v1 and v2 are fully supported. Also included is a torrent
-torrent file checker, which can verify a .torrent file is formated correctly
-as well as validate files and folders against metadata.
-
-Modules:
-    metafile: Creation/Validation of v1 .torrent files.
-    metafile2: Creation/Validation of v2 .torrent files.
-    torrentfile: torrentfiles Command Line Interface implementation.
-    exceptions: Custom Exceptions used in package.
-    utils: Utilities used throughout package.
+All Bittorrent versions are fully supported.  Torrentfile can also edit,
+recheck torrents contents, and create magnet URI's for torrent files.
 """
 from torrentfile.cli import execute, main
 from torrentfile.commands import create, edit, info, magnet, recheck
 from torrentfile.utils import toggle_debug_mode
 from torrentfile.version import __version__
 
 toggle_debug_mode(False)
```

### Comparing `torrentfile-0.8.8/torrentfile/__main__.py` & `torrentfile-0.9.0/torrentfile/__main__.py`

 * *Files identical despite different names*

### Comparing `torrentfile-0.8.8/torrentfile/cli.py` & `torrentfile-0.9.0/torrentfile/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,20 +35,20 @@
 Config : class
     controls logging configuration
 TorrentFileHelpFormatter : HelpFormatter
     the command line help message formatter
 """
 
 import io
-import logging
 import sys
+import logging
 from argparse import ArgumentParser, HelpFormatter
 
-from torrentfile.commands import (create, edit, info, magnet, rebuild, recheck,
-                                  rename)
+from torrentfile.commands import (
+    create, edit, get_magnet, info, rebuild, recheck, rename)
 from torrentfile.utils import toggle_debug_mode
 from torrentfile.version import __version__ as version
 
 
 class Config:
     """
     Class the controls the logging configuration and output settings.
@@ -92,30 +92,33 @@
 class TorrentFileHelpFormatter(HelpFormatter):
     """
     Formatting class for help tips provided by the CLI.
 
     Subclasses Argparse.HelpFormatter.
     """
 
-    def __init__(self, prog, width=45, max_help_positions=45):
+    def __init__(self,
+                 prog: str,
+                 width: int = 45,
+                 max_help_positions: int = 45):
         """
         Construct HelpFormat class for usage output.
 
         Parameters
         ----------
         prog : str
             Name of the program.
         width : int
             Max width of help message output.
         max_help_positions : int
             max length until line wrap.
         """
-        super().__init__(
-            prog, width=width, max_help_position=max_help_positions
-        )
+        super().__init__(prog,
+                         width=width,
+                         max_help_position=max_help_positions)
 
     def _split_lines(self, text: str, _: int) -> list:
         """
         Split multiline help messages and remove indentation.
 
         Parameters
         ----------
@@ -218,16 +221,15 @@
             args = ["-h"]
 
     parser = ArgumentParser(
         "torrentfile",
         usage="torrentfile <options>",
         description=(
             "Command line tools for creating, editing, checking, building "
-            "and interacting with Bittorrent metainfo files"
-        ),
+            "and interacting with Bittorrent meta files"),
         prefix_chars="-",
         formatter_class=TorrentFileHelpFormatter,
         conflict_handler="resolve",
     )
 
     parser.add_argument(
         "-q",
@@ -296,25 +298,21 @@
         action="store",
         dest="source",
         metavar="<source>",
         help="Add a source string. Useful for cross-seeding.",
     )
 
     create_parser.add_argument(
-        "-f",
         "--config",
         action="store_true",
         dest="config",
         help="""
         Parse torrent information from a config file. Looks in the current
         working directory, or the directory named .torrentfile in the users
-        home directory for a torrentfile.ini file. You can also use this
-        option in combination with the --config-path to specify the path to
-        the config file. See documentation for details on properly formatting
-        config file.
+        home directory for a torrentfile.ini file. See --config-path option.
         """,
     )
 
     create_parser.add_argument(
         "--config-path",
         action="store",
         metavar="<path>",
@@ -343,31 +341,24 @@
 
     create_parser.add_argument(
         "-o",
         "--out",
         action="store",
         dest="outfile",
         metavar="<path>",
-        help="Explicitly specify the path to write the file.",
-    )
-
-    create_parser.add_argument(
-        "--cwd",
-        "--current",
-        action="store_true",
-        dest="cwd",
-        help="*deprecated* Saving to current directory is default behaviour",
+        help="Explicitly specify the path to write the file .torrent file",
     )
 
     create_parser.add_argument(
         "--prog",
         "--progress",
         default="1",
         action="store",
         dest="progress",
+        metavar="<int>",
         help="""
         Set the progress bar level.
         Options = 0, 1
         (0) = Do not display progress bar.
         (1) = Display progress bar.(default)
         """,
     )
@@ -529,15 +520,32 @@
     magnet_parser.add_argument(
         "metafile",
         action="store",
         help="Path to Bittorrent meta file.",
         metavar="<*.torrent>",
     )
 
-    magnet_parser.set_defaults(func=magnet)
+    magnet_parser.add_argument(
+        "--meta-version",
+        action="store",
+        choices=["0", "1", "2", "3"],
+        default="0",
+        help="""
+        This option is only relevant for hybrid torrent files.
+        Options = 0, 1, 2, 3
+        (0) = [default] version is determined automatically
+        (1) = create V1 magnet link only
+        (2) = create V2 magnet link only
+        (3) = create a hybrid magnet link
+        """,
+        dest="meta_version",
+        metavar="<int>",
+    )
+
+    magnet_parser.set_defaults(func=get_magnet)
 
     check_parser = subparsers.add_parser(
         "recheck",
         help="Gives a detailed look at how much of the torrent is available.",
         aliases=["check", "r"],
         prefix_chars="-",
         formatter_class=TorrentFileHelpFormatter,
@@ -557,17 +565,19 @@
         help="path to content file or directory",
     )
 
     check_parser.set_defaults(func=recheck)
 
     rebuild_parser = subparsers.add_parser(
         "rebuild",
-        help="""Re-assemble files obtained from a bittorrent file into the
-                appropriate file structure for re-seeding.  Read documentation
-                for more information, or use cases.""",
+        help="""
+        Re-assemble files obtained from a bittorrent file into the
+        appropriate file structure for re-seeding.  Read documentation
+        for more information, or use cases.
+        """,
         formatter_class=TorrentFileHelpFormatter,
     )
 
     rebuild_parser.add_argument(
         "-m",
         "--metafiles",
         action="store",
@@ -575,15 +585,16 @@
         nargs="+",
         dest="metafiles",
         required=True,
         help="path(s) to .torrent file(s)/folder(s) containing .torrent files",
     )
 
     rebuild_parser.add_argument(
-        "-c" "--contents",
+        "-c"
+        "--contents",
         action="store",
         dest="contents",
         nargs="+",
         required=True,
         metavar="<contents>",
         help="folders that might contain the source contents needed to rebuld",
     )
@@ -613,31 +624,31 @@
         metavar="<target>",
         help="path to file that needs renaming.",
     )
 
     rename_parser.set_defaults(func=rename)
 
     all_commands = [
-        "create",
-        "new",
         "c",
-        "edit",
         "e",
-        "info",
         "i",
-        "magnet",
         "m",
-        "recheck",
-        "check",
         "r",
-        "rename",
-        "rebuild",
         "-i",
         "-h",
         "-V",
+        "new",
+        "edit",
+        "info",
+        "check",
+        "create",
+        "magnet",
+        "rename",
+        "rebuild",
+        "recheck",
     ]
     if not any(i for i in all_commands if i in args):
         start = 0
         while args[start] in ["-v", "-q"]:
             start += 1
         args.insert(start, "create")
 
@@ -653,12 +664,12 @@
         return args.func(args)
     return args  # pragma: nocover
 
 
 main_script = execute
 
 
-def main():
+def main() -> None:
     """
     Initiate main function for CLI script.
     """
     execute()
```

### Comparing `torrentfile-0.8.8/torrentfile/edit.py` & `torrentfile-0.9.0/torrentfile/edit.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,130 +1,130 @@
-#! /usr/bin/python3
-# -*- coding: utf-8 -*-
-
-##############################################################################
-#    Copyright (C) 2021-current alexpdev
-#
-#    Licensed under the Apache License, Version 2.0 (the "License");
-#    you may not use this file except in compliance with the License.
-#    You may obtain a copy of the License at
-#
-#        http://www.apache.org/licenses/LICENSE-2.0
-#
-#    Unless required by applicable law or agreed to in writing, software
-#    distributed under the License is distributed on an "AS IS" BASIS,
-#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#    See the License for the specific language governing permissions and
-#    limitations under the License.
-##############################################################################
-"""
-Edit torrent module.
-
-Provides a facility by which certain properties of a torrent meta file can be
-edited by the user. The various command line arguments indicate which fields
-should be edited, and what the new value should be.  Depending on what fields
-are chosen to edit, this command can trigger a new info hash which means the
-torrent will no longer be able to participate in the same swarm as the original
-unedited torrent.
-
-Keywords
---------
-private
-comment
-source
-trackers
-web-seeds
-"""
-
-import logging
-import os
-
-import pyben
-
-logger = logging.getLogger(__name__)
-
-
-def filter_empty(args: dict, meta: dict, info: dict):
-    """
-    Remove the fields that were not used by the original file creator.
-
-    Parameters
-    ----------
-    args : dict
-        Editable metafile properties from user.
-    meta : dict
-        Metafile data dictionary.
-    info : dict
-        Metafile info dictionary.
-    """
-    for key, val in list(args.items()):
-        if val is None:
-            del args[key]
-            continue
-
-        if val == "":
-            if key in meta:
-                del meta[key]
-            elif key in info:
-                del info[key]
-            del args[key]
-            logger.debug("removeing empty fields %s", val)
-
-
-def edit_torrent(metafile: str, args: dict) -> dict:
-    """
-    Edit the properties and values in a torrent meta file.
-
-    Parameters
-    ----------
-    metafile : str
-        path to the torrent meta file.
-    args : dict
-        key value pairs of the properties to be edited.
-
-    Returns
-    -------
-    dict
-        The edited and nested Meta and info dictionaries.
-    """
-    logger.debug("editing torrent file %s", metafile)
-    meta = pyben.load(metafile)
-    info = meta["info"]
-    filter_empty(args, meta, info)
-
-    if "comment" in args:
-        info["comment"] = args["comment"]
-
-    if "source" in args:
-        info["source"] = args["source"]
-
-    if "private" in args:
-        info["private"] = 1
-
-    if "announce" in args:
-        val = args.get("announce", None)
-        if isinstance(val, str):
-            vallist = val.split()
-            meta["announce"] = vallist[0]
-            meta["announce-list"] = [vallist]
-        elif isinstance(val, list):
-            meta["announce"] = val[0]
-            meta["announce-list"] = [val]
-
-    if "url-list" in args:
-        val = args.get("url-list")
-        if isinstance(val, str):
-            meta["url-list"] = val.split()
-        elif isinstance(val, list):
-            meta["url-list"] = val
-
-    if "httpseeds" in args:
-        val = args.get("httpseeds")
-        if isinstance(val, str):
-            meta["httpseeds"] = val.split()
-        elif isinstance(val, list):
-            meta["httpseeds"] = val
-
-    meta["info"] = info
-    os.remove(metafile)
-    pyben.dump(meta, metafile)
-    return meta
+#! /usr/bin/python3
+# -*- coding: utf-8 -*-
+
+##############################################################################
+#    Copyright (C) 2021-current alexpdev
+#
+#    Licensed under the Apache License, Version 2.0 (the "License");
+#    you may not use this file except in compliance with the License.
+#    You may obtain a copy of the License at
+#
+#        http://www.apache.org/licenses/LICENSE-2.0
+#
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS,
+#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#    See the License for the specific language governing permissions and
+#    limitations under the License.
+##############################################################################
+"""
+Edit torrent module.
+
+Provides a facility by which certain properties of a torrent meta file can be
+edited by the user. The various command line arguments indicate which fields
+should be edited, and what the new value should be.  Depending on what fields
+are chosen to edit, this command can trigger a new info hash which means the
+torrent will no longer be able to participate in the same swarm as the original
+unedited torrent.
+
+Keywords
+--------
+private
+comment
+source
+trackers
+web-seeds
+"""
+
+import os
+import logging
+
+import pyben
+
+logger = logging.getLogger(__name__)
+
+
+def filter_empty(args: dict, meta: dict, info: dict):
+    """
+    Remove the fields that were not used by the original file creator.
+
+    Parameters
+    ----------
+    args : dict
+        Editable metafile properties from user.
+    meta : dict
+        Metafile data dictionary.
+    info : dict
+        Metafile info dictionary.
+    """
+    for key, val in list(args.items()):
+        if val is None:
+            del args[key]
+            continue
+
+        if val == "":
+            if key in meta:
+                del meta[key]
+            elif key in info:
+                del info[key]
+            del args[key]
+            logger.debug("removeing empty fields %s", val)
+
+
+def edit_torrent(metafile: str, args: dict) -> dict:
+    """
+    Edit the properties and values in a torrent meta file.
+
+    Parameters
+    ----------
+    metafile : str
+        path to the torrent meta file.
+    args : dict
+        key value pairs of the properties to be edited.
+
+    Returns
+    -------
+    dict
+        The edited and nested Meta and info dictionaries.
+    """
+    logger.debug("editing torrent file %s", metafile)
+    meta = pyben.load(metafile)
+    info = meta["info"]
+    filter_empty(args, meta, info)
+
+    if "comment" in args:
+        info["comment"] = args["comment"]
+
+    if "source" in args:
+        info["source"] = args["source"]
+
+    if "private" in args:
+        info["private"] = 1
+
+    if "announce" in args:
+        val = args.get("announce", None)
+        if isinstance(val, str):
+            vallist = val.split()
+            meta["announce"] = vallist[0]
+            meta["announce-list"] = [vallist]
+        elif isinstance(val, list):
+            meta["announce"] = val[0]
+            meta["announce-list"] = [val]
+
+    if "url-list" in args:
+        val = args.get("url-list")
+        if isinstance(val, str):
+            meta["url-list"] = val.split()
+        elif isinstance(val, list):
+            meta["url-list"] = val
+
+    if "httpseeds" in args:
+        val = args.get("httpseeds")
+        if isinstance(val, str):
+            meta["httpseeds"] = val.split()
+        elif isinstance(val, list):
+            meta["httpseeds"] = val
+
+    meta["info"] = info
+    os.remove(metafile)
+    pyben.dump(meta, metafile)
+    return meta
```

### Comparing `torrentfile-0.8.8/torrentfile/hasher.py` & `torrentfile-0.9.0/torrentfile/hasher.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,534 +1,523 @@
-#! /usr/bin/python3
-# -*- coding: utf-8 -*-
-
-##############################################################################
-#    Copyright (C) 2021-current alexpdev
-#
-#    Licensed under the Apache License, Version 2.0 (the "License");
-#    you may not use this file except in compliance with the License.
-#    You may obtain a copy of the License at
-#
-#        http://www.apache.org/licenses/LICENSE-2.0
-#
-#    Unless required by applicable law or agreed to in writing, software
-#    distributed under the License is distributed on an "AS IS" BASIS,
-#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#    See the License for the specific language governing permissions and
-#    limitations under the License.
-##############################################################################
-"""
-Piece/File Hashers for Bittorrent meta file contents.
-"""
-
-import logging
-import os
-from hashlib import sha1, sha256  # nosec
-
-from torrentfile.mixins import CbMixin, ProgMixin
-from torrentfile.utils import next_power_2
-
-BLOCK_SIZE = 2**14  # 16KiB
-HASH_SIZE = 32
-
-logger = logging.getLogger(__name__)
-
-
-class Hasher(CbMixin, ProgMixin):
-    """
-    Piece hasher for Bittorrent V1 files.
-
-    Takes a sorted list of all file paths, calculates sha1 hash
-    for fixed size pieces of file data from each file
-    seemlessly until the last piece which may be smaller than others.
-
-    Parameters
-    ----------
-    paths : list
-        List of files.
-    piece_length : int
-        Size of chuncks to split the data into.
-    progress : int
-        default = None
-    """
-
-    def __init__(self, paths: list, piece_length: int, progress: bool = True):
-        """Generate hashes of piece length data from filelist contents."""
-        self.piece_length = piece_length
-        self.paths = paths
-        self.progress = progress
-        self.total = sum(os.path.getsize(i) for i in self.paths)
-        self.index = 0
-        self.current = open(self.paths[0], "rb")
-        if self.progress:
-            total = os.path.getsize(self.paths[0])
-            self.prog_start(total, self.paths[0], unit="bytes")
-        logger.debug("Hashing %s", str(self.paths[0]))
-
-    def __iter__(self):
-        """
-        Iterate through feed pieces.
-
-        Returns
-        -------
-        self : iterator
-            Iterator for leaves/hash pieces.
-        """
-        return self
-
-    def _handle_partial(self, arr: bytearray) -> bytearray:
-        """
-        Define the handling partial pieces that span 2 or more files.
-
-        Parameters
-        ----------
-        arr : bytearray
-            Incomplete piece containing partial data
-
-        Returns
-        -------
-        digest : bytearray
-            SHA1 digest of the complete piece.
-        """
-        while len(arr) < self.piece_length and self.next_file():
-            target = self.piece_length - len(arr)
-            temp = bytearray(target)
-            size = self.current.readinto(temp)
-            arr.extend(temp[:size])
-            self.prog_update(size)
-            if size == target:
-                break
-        return sha1(arr).digest()  # nosec
-
-    def next_file(self) -> bool:
-        """
-        Seemlessly transition to next file in file list.
-
-        Returns
-        -------
-        bool:
-            True if there is a next file otherwise False.
-        """
-        self.index += 1
-        self.prog_close()
-        if self.index < len(self.paths):
-            path = self.paths[self.index]
-            logger.debug("Hashing %s", str(path))
-            self.current.close()
-            if self.progress:
-                self.prog_start(os.path.getsize(path), path, unit="bytes")
-            self.current = open(path, "rb")
-            return True
-        return False
-
-    def __next__(self) -> bytes:
-        """
-        Generate piece-length pieces of data from input file list.
-
-        Returns
-        -------
-        bytes
-            SHA1 hash of the piece extracted.
-        """
-        while True:
-            piece = bytearray(self.piece_length)
-            size = self.current.readinto(piece)
-            if size == 0:
-                if not self.next_file():
-                    raise StopIteration
-            elif size < self.piece_length:
-                self.prog_update(size)
-                return self._handle_partial(piece[:size])
-            else:
-                self.prog_update(size)
-                return sha1(piece).digest()  # nosec
-
-
-def merkle_root(blocks: list) -> bytes:
-    """
-    Calculate the merkle root for a seq of sha256 hash digests.
-
-    Parameters
-    ----------
-    blocks : list
-        a sequence of sha256 layer hashes.
-
-    Returns
-    -------
-    bytes
-        the sha256 root hash of the merkle tree.
-    """
-    if blocks:
-        while len(blocks) > 1:
-            blocks = [
-                sha256(x + y).digest() for x, y in zip(*[iter(blocks)] * 2)
-            ]
-        return blocks[0]
-    return blocks
-
-
-class HasherV2(CbMixin, ProgMixin):
-    """
-    Calculate the root hash and piece layers for file contents.
-
-    **DEPRECATED**
-
-    Iterates over 16KiB blocks of data from given file, hashes the data,
-    then creates a hash tree from the individual block hashes until size of
-    hashed data equals the piece-length.  Then continues the hash tree until
-    root hash is calculated.
-
-    Parameters
-    ----------
-    path : str
-        Path to file.
-    piece_length : int
-        Size of layer hashes pieces.
-    progress : int
-        default = None
-    """
-
-    def __init__(self, path: str, piece_length: int, progress: bool = True):
-        """
-        Calculate and store hash information for specific file.
-
-        **DEPRECATED**
-        """
-        self.path = path
-        self.root = None
-        self.piece_layer = None
-        self.layer_hashes = []
-        self.piece_length = piece_length
-        self.num_blocks = piece_length // BLOCK_SIZE
-        if progress:
-            self.prog_start(os.path.getsize(path), path, unit="bytes")
-        with open(self.path, "rb") as fd:
-            self.process_file(fd)
-
-    def process_file(self, fd: str):
-        """
-        Calculate hashes over 16KiB chuncks of file content.
-
-        **DEPRECATED**
-
-        Parameters
-        ----------
-        fd : TextIOWrapper
-            Opened file in read mode.
-        """
-        while True:
-            blocks = []
-            leaf = bytearray(BLOCK_SIZE)
-            # generate leaves of merkle tree
-
-            for _ in range(self.num_blocks):
-                size = fd.readinto(leaf)
-                self.prog_update(size)
-                if not size:
-                    break
-                blocks.append(sha256(leaf[:size]).digest())
-
-            # blocks is empty mean eof
-            if not blocks:
-                break
-            if len(blocks) != self.num_blocks:
-                # when size of file doesn't fill the last block
-                # when the file contains multiple pieces
-                remaining = self.num_blocks - len(blocks)
-                if not self.layer_hashes:
-                    # when the there is only one block for file
-                    power2 = next_power_2(len(blocks))
-                    remaining = power2 - len(blocks)
-
-                # pad the the rest with zeroes to fill remaining space.
-                padding = [bytes(32) for _ in range(remaining)]
-                self.prog_update(HASH_SIZE * remaining)
-                blocks.extend(padding)
-            # calculate the root hash for the merkle tree up to piece-length
-
-            layer_hash = merkle_root(blocks)
-            self.cb(layer_hash)
-            self.layer_hashes.append(layer_hash)
-        self._calculate_root()
-        self.prog_close()
-
-    def _calculate_root(self):
-        """
-        Calculate root hash for the target file.
-
-        **DEPRECATED**
-        """
-        self.piece_layer = b"".join(self.layer_hashes)
-        hashes = len(self.layer_hashes)
-        if hashes > 1:
-            pow2 = next_power_2(hashes)
-            remainder = pow2 - hashes
-            pad_piece = [bytes(HASH_SIZE) for _ in range(self.num_blocks)]
-            for _ in range(remainder):
-                self.layer_hashes.append(merkle_root(pad_piece))
-        self.root = merkle_root(self.layer_hashes)
-
-
-class HasherHybrid(CbMixin, ProgMixin):
-    """
-    Calculate root and piece hashes for creating hybrid torrent file.
-
-    **DEPRECATED**
-
-    Create merkle tree layers from sha256 hashed 16KiB blocks of contents.
-    With a branching factor of 2, merge layer hashes until blocks equal
-    piece_length bytes for the piece layer, and then the root hash.
-
-    Parameters
-    ----------
-    path : str
-        path to target file.
-    piece_length : int
-        piece length for data chunks.
-    progress : int
-        default = None
-    """
-
-    def __init__(self, path: str, piece_length: int, progress: bool = True):
-        """
-        Construct Hasher class instances for each file in torrent.
-
-        **DEPRECATED**
-        """
-        self.path = path
-        self.piece_length = piece_length
-        self.pieces = []
-        self.layer_hashes = []
-        self.piece_layer = None
-        self.root = None
-        self.padding_piece = None
-        self.padding_file = None
-        if progress:
-            self.prog_start(os.path.getsize(path), path, unit="bytes")
-        self.amount = piece_length // BLOCK_SIZE
-        with open(path, "rb") as data:
-            self.process_file(data)
-
-    def _pad_remaining(self, block_count: int):
-        """
-        Generate Hash sized, 0 filled bytes for padding.
-
-        **DEPRECATED**
-
-        Parameters
-        ----------
-        block_count : int
-            current total number of blocks collected.
-
-        Returns
-        -------
-        padding : bytes
-            Padding to fill remaining portion of tree.
-        """
-        # when the there is only one block for file
-        remaining = self.amount - block_count
-        if not self.layer_hashes:
-            power2 = next_power_2(block_count)
-            remaining = power2 - block_count
-        self.prog_update(HASH_SIZE * remaining)
-        return [bytes(HASH_SIZE) for _ in range(remaining)]
-
-    def process_file(self, data: bytearray):
-        """
-        Calculate layer hashes for contents of file.
-
-        **DEPRECATED**
-
-        Parameters
-        ----------
-        data : BytesIO
-            File opened in read mode.
-        """
-        while True:
-            plength = self.piece_length
-            blocks = []
-            piece = sha1()  # nosec
-            total = 0
-            block = bytearray(BLOCK_SIZE)
-            for _ in range(self.amount):
-                size = data.readinto(block)
-                self.prog_update(size)
-                if not size:
-                    break
-                total += size
-                plength -= size
-                blocks.append(sha256(block[:size]).digest())
-                piece.update(block[:size])
-            if not blocks:
-                break
-            if len(blocks) != self.amount:
-                padding = self._pad_remaining(len(blocks))
-                blocks.extend(padding)
-            layer_hash = merkle_root(blocks)
-            self.cb(layer_hash)
-            self.layer_hashes.append(layer_hash)
-            if plength > 0:
-                self.padding_file = {
-                    "attr": "p",
-                    "length": plength,
-                    "path": [".pad", str(plength)],
-                }
-                piece.update(bytes(plength))
-            self.pieces.append(piece.digest())  # nosec
-        self._calculate_root()
-        self.prog_close()
-
-    def _calculate_root(self):
-        """
-        Calculate the root hash for opened file.
-
-        **DEPRECATED**
-        """
-        self.piece_layer = b"".join(self.layer_hashes)
-
-        if len(self.layer_hashes) > 1:
-            pad_piece = merkle_root([bytes(32) for _ in range(self.amount)])
-
-            pow2 = next_power_2(len(self.layer_hashes))
-            remainder = pow2 - len(self.layer_hashes)
-
-            self.layer_hashes += [pad_piece for _ in range(remainder)]
-        self.root = merkle_root(self.layer_hashes)
-
-
-class FileHasher(CbMixin, ProgMixin):
-    """
-    Calculate root and piece hashes for creating hybrid torrent file.
-
-    Create merkle tree layers from sha256 hashed 16KiB blocks of contents.
-    With a branching factor of 2, merge layer hashes until blocks equal
-    piece_length bytes for the piece layer, and then the root hash.
-
-    Parameters
-    ----------
-    path : str
-        path to target file.
-    piece_length : int
-        piece length for data chunks.
-    progress : int
-        default = None
-    """
-
-    def __init__(
-        self,
-        path: str,
-        piece_length: int,
-        progress: bool = True,
-        hybrid: bool = False,
-    ):
-        """
-        Construct Hasher class instances for each file in torrent.
-        """
-        self.path = path
-        self.piece_length = piece_length
-        self.pieces = []
-        self.layer_hashes = []
-        self.piece_layer = None
-        self.root = None
-        self.padding_piece = None
-        self.padding_file = None
-        self.amount = piece_length // BLOCK_SIZE
-        self.end = False
-        self.current = open(path, "rb")
-        self.hybrid = hybrid
-        if progress:
-            self.progressbar = True
-            self.prog_start(os.path.getsize(path), path, unit="bytes")
-
-    def __iter__(self):
-        """Return `self`: needed to implement iterator implementation."""
-        return self
-
-    def _pad_remaining(self, block_count: int):
-        """
-        Generate Hash sized, 0 filled bytes for padding.
-
-        Parameters
-        ----------
-        block_count : int
-            current total number of blocks collected.
-
-        Returns
-        -------
-        padding : bytes
-            Padding to fill remaining portion of tree.
-        """
-        # when the there is only one block for file
-        remaining = self.amount - block_count
-        if not self.layer_hashes:
-            power2 = next_power_2(block_count)
-            remaining = power2 - block_count
-        return [bytes(HASH_SIZE) for _ in range(remaining)]
-
-    def __next__(self) -> bytes:
-        """
-        Calculate layer hashes for contents of file.
-
-        Returns
-        -------
-        bytes
-            The layer merckle root hash.
-        """
-        if self.end:
-            self.end = False
-            raise StopIteration
-        plength = self.piece_length
-        blocks = []
-        piece = sha1()  # nosec
-        total = 0
-        block = bytearray(BLOCK_SIZE)
-        for _ in range(self.amount):
-            size = self.current.readinto(block)
-            if not size:
-                self.end = True
-                break
-            total += size
-            plength -= size
-            blocks.append(sha256(block[:size]).digest())
-            if self.hybrid:
-                piece.update(block[:size])
-        if not blocks:
-            self._calculate_root()
-            raise StopIteration
-        if len(blocks) != self.amount:
-            padding = self._pad_remaining(len(blocks))
-            blocks.extend(padding)
-        self.prog_update(total)
-        layer_hash = merkle_root(blocks)
-        self.layer_hashes.append(layer_hash)
-        self.cb(layer_hash)
-        if self.end:
-            self._calculate_root()
-            self.prog_close()
-        if self.hybrid:
-            if plength > 0:
-                self.padding_file = {
-                    "attr": "p",
-                    "length": plength,
-                    "path": [".pad", str(plength)],
-                }
-                piece.update(bytes(plength))
-            piece = piece.digest()
-            self.pieces.append(piece)
-            return layer_hash, piece
-        return layer_hash
-
-    def _calculate_root(self):
-        """
-        Calculate the root hash for opened file.
-        """
-        self.piece_layer = b"".join(self.layer_hashes)
-
-        if len(self.layer_hashes) > 1:
-            pad_piece = merkle_root([bytes(32) for _ in range(self.amount)])
-
-            pow2 = next_power_2(len(self.layer_hashes))
-            remainder = pow2 - len(self.layer_hashes)
-
-            self.layer_hashes += [pad_piece for _ in range(remainder)]
-        self.root = merkle_root(self.layer_hashes)
-        self.current.close()
+#! /usr/bin/python3
+# -*- coding: utf-8 -*-
+
+##############################################################################
+#    Copyright (C) 2021-current alexpdev
+#
+#    Licensed under the Apache License, Version 2.0 (the "License");
+#    you may not use this file except in compliance with the License.
+#    You may obtain a copy of the License at
+#
+#        http://www.apache.org/licenses/LICENSE-2.0
+#
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS,
+#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#    See the License for the specific language governing permissions and
+#    limitations under the License.
+##############################################################################
+"""
+Piece/File Hashers for Bittorrent meta file contents.
+"""
+
+import os
+import logging
+from hashlib import sha1, sha256  # nosec
+
+from torrentfile.mixins import CbMixin, ProgMixin
+from torrentfile.utils import next_power_2
+
+BLOCK_SIZE = 2**14  # 16KiB
+HASH_SIZE = 32
+
+logger = logging.getLogger(__name__)
+
+
+class Hasher(CbMixin, ProgMixin):
+    """
+    Piece hasher for Bittorrent V1 files.
+
+    Takes a sorted list of all file paths, calculates sha1 hash
+    for fixed size pieces of file data from each file
+    seemlessly until the last piece which may be smaller than others.
+
+    Parameters
+    ----------
+    paths : list
+        List of files.
+    piece_length : int
+        Size of chuncks to split the data into.
+    progress : int
+        default = None
+    """
+
+    def __init__(self, paths: list, piece_length: int, progress: bool = True):
+        """Generate hashes of piece length data from filelist contents."""
+        self.piece_length = piece_length
+        self.paths = paths
+        self.progress = progress
+        self.total = sum(os.path.getsize(i) for i in self.paths)
+        self.index = 0
+        self.current = open(self.paths[0], "rb")
+        if self.progress:
+            total = os.path.getsize(self.paths[0])
+            self.prog_start(total, self.paths[0])
+        logger.debug("Hashing %s", str(self.paths[0]))
+
+    def __iter__(self):
+        """
+        Iterate through feed pieces.
+
+        Returns
+        -------
+        self : iterator
+            Iterator for leaves/hash pieces.
+        """
+        return self
+
+    def _handle_partial(self, arr: bytearray) -> bytearray:
+        """
+        Define the handling partial pieces that span 2 or more files.
+
+        Parameters
+        ----------
+        arr : bytearray
+            Incomplete piece containing partial data
+
+        Returns
+        -------
+        digest : bytearray
+            SHA1 digest of the complete piece.
+        """
+        while len(arr) < self.piece_length and self.next_file():
+            target = self.piece_length - len(arr)
+            temp = bytearray(target)
+            size = self.current.readinto(temp)
+            arr.extend(temp[:size])
+            self.prog_update(size)
+            if size == target:
+                break
+        return sha1(arr).digest()  # nosec
+
+    def next_file(self) -> bool:
+        """
+        Seemlessly transition to next file in file list.
+
+        Returns
+        -------
+        bool:
+            True if there is a next file otherwise False.
+        """
+        self.index += 1
+        self.prog_close()
+        if self.index < len(self.paths):
+            path = self.paths[self.index]
+            logger.debug("Hashing %s", str(path))
+            self.current.close()
+            if self.progress:
+                self.prog_start(os.path.getsize(path), path)
+            self.current = open(path, "rb")
+            return True
+        return False
+
+    def __next__(self) -> bytes:
+        """
+        Generate piece-length pieces of data from input file list.
+
+        Returns
+        -------
+        bytes
+            SHA1 hash of the piece extracted.
+        """
+        while True:
+            piece = bytearray(self.piece_length)
+            size = self.current.readinto(piece)
+            if size == 0:
+                if not self.next_file():
+                    raise StopIteration
+            elif size < self.piece_length:
+                self.prog_update(size)
+                return self._handle_partial(piece[:size])
+            else:
+                self.prog_update(size)
+                return sha1(piece).digest()  # nosec
+
+
+def merkle_root(blocks: list) -> bytes:
+    """
+    Calculate the merkle root for a seq of sha256 hash digests.
+
+    Parameters
+    ----------
+    blocks : list
+        a sequence of sha256 layer hashes.
+
+    Returns
+    -------
+    bytes
+        the sha256 root hash of the merkle tree.
+    """
+    if blocks:
+        while len(blocks) > 1:
+            blocks = [
+                sha256(x + y).digest() for x, y in zip(*[iter(blocks)] * 2)
+            ]
+        return blocks[0]
+    return blocks
+
+
+class HasherV2(CbMixin, ProgMixin):
+    """
+    Calculate the root hash and piece layers for file contents.
+
+    Iterates over 16KiB blocks of data from given file, hashes the data,
+    then creates a hash tree from the individual block hashes until size of
+    hashed data equals the piece-length.  Then continues the hash tree until
+    root hash is calculated.
+
+    Parameters
+    ----------
+    path : str
+        Path to file.
+    piece_length : int
+        Size of layer hashes pieces.
+    progress : int
+        default = None
+    """
+
+    def __init__(self, path: str, piece_length: int, progress: bool = True):
+        """
+        Calculate and store hash information for specific file.
+        """
+        self.path = path
+        self.root = None
+        self.piece_layer = None
+        self.layer_hashes = []
+        self.piece_length = piece_length
+        self.num_blocks = piece_length // BLOCK_SIZE
+        if progress:
+            self.prog_start(os.path.getsize(path), path)
+        with open(self.path, "rb") as fd:
+            self.process_file(fd)
+
+    def process_file(self, fd: str):
+        """
+        Calculate hashes over 16KiB chuncks of file content.
+
+        Parameters
+        ----------
+        fd : TextIOWrapper
+            Opened file in read mode.
+        """
+        while True:
+            blocks = []
+            leaf = bytearray(BLOCK_SIZE)
+            # generate leaves of merkle tree
+
+            for _ in range(self.num_blocks):
+                size = fd.readinto(leaf)
+                self.prog_update(size)
+                if not size:
+                    break
+                blocks.append(sha256(leaf[:size]).digest())
+
+            # blocks is empty mean eof
+            if not blocks:
+                break
+            if len(blocks) != self.num_blocks:
+                # when size of file doesn't fill the last block
+                # when the file contains multiple pieces
+                remaining = self.num_blocks - len(blocks)
+                if not self.layer_hashes:
+                    # when the there is only one block for file
+                    power2 = next_power_2(len(blocks))
+                    remaining = power2 - len(blocks)
+
+                # pad the the rest with zeroes to fill remaining space.
+                padding = [bytes(32) for _ in range(remaining)]
+                self.prog_update(HASH_SIZE * remaining)
+                blocks.extend(padding)
+            # calculate the root hash for the merkle tree up to piece-length
+
+            layer_hash = merkle_root(blocks)
+            self.cb(layer_hash)
+            self.layer_hashes.append(layer_hash)
+        self._calculate_root()
+        self.prog_close()
+
+    def _calculate_root(self):
+        """
+        Calculate root hash for the target file.
+        """
+        self.piece_layer = b"".join(self.layer_hashes)
+        hashes = len(self.layer_hashes)
+        if hashes > 1:
+            pow2 = next_power_2(hashes)
+            remainder = pow2 - hashes
+            pad_piece = [bytes(HASH_SIZE) for _ in range(self.num_blocks)]
+            for _ in range(remainder):
+                self.layer_hashes.append(merkle_root(pad_piece))
+        self.root = merkle_root(self.layer_hashes)
+
+
+class HasherHybrid(CbMixin, ProgMixin):
+    """
+    Calculate root and piece hashes for creating hybrid torrent file.
+
+    Create merkle tree layers from sha256 hashed 16KiB blocks of contents.
+    With a branching factor of 2, merge layer hashes until blocks equal
+    piece_length bytes for the piece layer, and then the root hash.
+
+    Parameters
+    ----------
+    path : str
+        path to target file.
+    piece_length : int
+        piece length for data chunks.
+    progress : int
+        default = None
+    """
+
+    def __init__(self, path: str, piece_length: int, progress: bool = True):
+        """
+        Construct Hasher class instances for each file in torrent.
+        """
+        self.path = path
+        self.piece_length = piece_length
+        self.pieces = []
+        self.layer_hashes = []
+        self.piece_layer = None
+        self.root = None
+        self.padding_piece = None
+        self.padding_file = None
+        if progress:
+            self.prog_start(os.path.getsize(path), path)
+        self.amount = piece_length // BLOCK_SIZE
+        with open(path, "rb") as data:
+            self.process_file(data)
+
+    def _pad_remaining(self, block_count: int):
+        """
+        Generate Hash sized, 0 filled bytes for padding.
+
+        Parameters
+        ----------
+        block_count : int
+            current total number of blocks collected.
+
+        Returns
+        -------
+        padding : bytes
+            Padding to fill remaining portion of tree.
+        """
+        # when the there is only one block for file
+        remaining = self.amount - block_count
+        if not self.layer_hashes:
+            power2 = next_power_2(block_count)
+            remaining = power2 - block_count
+        self.prog_update(HASH_SIZE * remaining)
+        return [bytes(HASH_SIZE) for _ in range(remaining)]
+
+    def process_file(self, data: bytearray):
+        """
+        Calculate layer hashes for contents of file.
+
+        Parameters
+        ----------
+        data : BytesIO
+            File opened in read mode.
+        """
+        while True:
+            plength = self.piece_length
+            blocks = []
+            piece = sha1()  # nosec
+            total = 0
+            block = bytearray(BLOCK_SIZE)
+            for _ in range(self.amount):
+                size = data.readinto(block)
+                self.prog_update(size)
+                if not size:
+                    break
+                total += size
+                plength -= size
+                blocks.append(sha256(block[:size]).digest())
+                piece.update(block[:size])
+            if not blocks:
+                break
+            if len(blocks) != self.amount:
+                padding = self._pad_remaining(len(blocks))
+                blocks.extend(padding)
+            layer_hash = merkle_root(blocks)
+            self.cb(layer_hash)
+            self.layer_hashes.append(layer_hash)
+            if plength > 0:
+                self.padding_file = {
+                    "attr": "p",
+                    "length": plength,
+                    "path": [".pad", str(plength)],
+                }
+                piece.update(bytes(plength))
+            self.pieces.append(piece.digest())  # nosec
+        self._calculate_root()
+        self.prog_close()
+
+    def _calculate_root(self):
+        """
+        Calculate the root hash for opened file.
+
+        **DEPRECATED**
+        """
+        self.piece_layer = b"".join(self.layer_hashes)
+
+        if len(self.layer_hashes) > 1:
+            pad_piece = merkle_root([bytes(32) for _ in range(self.amount)])
+
+            pow2 = next_power_2(len(self.layer_hashes))
+            remainder = pow2 - len(self.layer_hashes)
+
+            self.layer_hashes += [pad_piece for _ in range(remainder)]
+        self.root = merkle_root(self.layer_hashes)
+
+
+class FileHasher(CbMixin, ProgMixin):
+    """
+    Calculate root and piece hashes for creating hybrid torrent file.
+
+    Create merkle tree layers from sha256 hashed 16KiB blocks of contents.
+    With a branching factor of 2, merge layer hashes until blocks equal
+    piece_length bytes for the piece layer, and then the root hash.
+
+    Parameters
+    ----------
+    path : str
+        path to target file.
+    piece_length : int
+        piece length for data chunks.
+    progress : int
+        default = None
+    """
+
+    def __init__(
+        self,
+        path: str,
+        piece_length: int,
+        progress: bool = True,
+        hybrid: bool = False,
+    ):
+        """
+        Construct Hasher class instances for each file in torrent.
+        """
+        self.path = path
+        self.piece_length = piece_length
+        self.pieces = []
+        self.layer_hashes = []
+        self.piece_layer = None
+        self.root = None
+        self.padding_piece = None
+        self.padding_file = None
+        self.amount = piece_length // BLOCK_SIZE
+        self.end = False
+        self.current = open(path, "rb")
+        self.hybrid = hybrid
+        if progress:
+            self.progressbar = True
+            self.prog_start(os.path.getsize(path), path)
+
+    def __iter__(self):
+        """Return `self`: needed to implement iterator implementation."""
+        return self
+
+    def _pad_remaining(self, block_count: int):
+        """
+        Generate Hash sized, 0 filled bytes for padding.
+
+        Parameters
+        ----------
+        block_count : int
+            current total number of blocks collected.
+
+        Returns
+        -------
+        padding : bytes
+            Padding to fill remaining portion of tree.
+        """
+        # when the there is only one block for file
+        remaining = self.amount - block_count
+        if not self.layer_hashes:
+            power2 = next_power_2(block_count)
+            remaining = power2 - block_count
+        return [bytes(HASH_SIZE) for _ in range(remaining)]
+
+    def __next__(self) -> bytes:
+        """
+        Calculate layer hashes for contents of file.
+
+        Returns
+        -------
+        bytes
+            The layer merckle root hash.
+
+        Raises
+        ------
+        StopIteration
+            Halts the iterator from progressing
+        """
+        if self.end:
+            self.end = False
+            raise StopIteration
+        plength = self.piece_length
+        blocks = []
+        piece = sha1()  # nosec
+        total = 0
+        block = bytearray(BLOCK_SIZE)
+        for _ in range(self.amount):
+            size = self.current.readinto(block)
+            if not size:
+                self.end = True
+                break
+            total += size
+            plength -= size
+            blocks.append(sha256(block[:size]).digest())
+            if self.hybrid:
+                piece.update(block[:size])
+        if not blocks:
+            self._calculate_root()
+            raise StopIteration
+        if len(blocks) != self.amount:
+            padding = self._pad_remaining(len(blocks))
+            blocks.extend(padding)
+        self.prog_update(total)
+        layer_hash = merkle_root(blocks)
+        self.layer_hashes.append(layer_hash)
+        self.cb(layer_hash)
+        if self.end:
+            self._calculate_root()
+            self.prog_close()
+        if self.hybrid:
+            if plength > 0:
+                self.padding_file = {
+                    "attr": "p",
+                    "length": plength,
+                    "path": [".pad", str(plength)],
+                }
+                piece.update(bytes(plength))
+            piece = piece.digest()
+            self.pieces.append(piece)
+            return layer_hash, piece
+        return layer_hash
+
+    def _calculate_root(self):
+        """
+        Calculate the root hash for opened file.
+        """
+        self.piece_layer = b"".join(self.layer_hashes)
+
+        if len(self.layer_hashes) > 1:
+            pad_piece = merkle_root([bytes(32) for _ in range(self.amount)])
+
+            pow2 = next_power_2(len(self.layer_hashes))
+            remainder = pow2 - len(self.layer_hashes)
+
+            self.layer_hashes += [pad_piece for _ in range(remainder)]
+        self.root = merkle_root(self.layer_hashes)
+        self.current.close()
```

### Comparing `torrentfile-0.8.8/torrentfile/interactive.py` & `torrentfile-0.9.0/torrentfile/interactive.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 """
 Module contains the procedures used for Interactive Mode.
 
 ## This module has been deprecated.
 """
 
 import os
-import shutil
 import sys
+import shutil
 
 import pyben
 
 from torrentfile.edit import edit_torrent
 from torrentfile.recheck import Checker
 from torrentfile.torrent import TorrentFile, TorrentFileHybrid, TorrentFileV2
 
@@ -136,22 +136,18 @@
     """
     Operate TorrentFile program interactively through terminal.
 
     DEPRECATION WARNING: The interactive CLI feature will be deprecated
     in the future.
     """
     showcenter("TorrentFile: Starting Interactive Mode")
-    showcenter(
-        "DEPRECATION WARNING: The interactive feature will be"
-        "deprecated in the near future."
-    )
-    action = get_input(
-        "Enter the action you wish to perform.\n"
-        "Action ( Create (c) | Edit (e) | Recheck (r) ): "
-    )
+    showcenter("DEPRECATION WARNING: The interactive feature will be"
+               "deprecated in the near future.")
+    action = get_input("Enter the action you wish to perform.\n"
+                       "Action ( Create (c) | Edit (e) | Recheck (r) ): ")
     action = action.lower()
 
     if "create" in action or action == "c":
         return create_torrent()
 
     if "check" in action or action == "r":
         return recheck_torrent()
@@ -167,17 +163,16 @@
     Check torrent download completed percentage.
 
     @Deprecated
     """
     showcenter("Check Torrent")
     msg = "Enter path to torrent contents, and corresponding torrent metafile."
     showtext(msg)
-    metafile = get_input(
-        "Conent Path (downloads/complete/torrentname):", os.path.exists
-    )
+    metafile = get_input("Conent Path (downloads/complete/torrentname):",
+                         os.path.exists)
     contents = get_input("Metafile (*.torrent): ", os.path.exists)
     checker = Checker(metafile, contents)
     results = checker.results()
     showtext(f"Completion for {metafile} is {results}%")
     return results
 
 
@@ -189,16 +184,15 @@
     """
     showcenter("Create Torrent")
     showtext(
         "\nEnter values for each of the options for the torrent creator, "
         "or leave blank for program defaults.\nSpaces are considered item "
         "seperators for options that accept a list of values.\nValues "
         "enclosed in () indicate the default value, while {} holds all "
-        "valid choices available for the option.\n\n"
-    )
+        "valid choices available for the option.\n\n")
     creator = InteractiveCreator()
     return creator
 
 
 def edit_action():
     """
     Edit the editable values of the torrent meta file.
@@ -278,18 +272,16 @@
     def edit_props(self):
         """
         Loop continuosly for edits until user signals DONE.
 
         @Deprecated
         """
         while True:
-            showcenter(
-                "Choose the number for a propert the needs editing."
-                "Enter DONE when all editing has been completed."
-            )
+            showcenter("Choose the number for a propert the needs editing."
+                       "Enter DONE when all editing has been completed.")
 
             props = {
                 1: "comment",
                 2: "source",
                 3: "private",
                 4: "tracker",
                 5: "web-seed",
@@ -311,16 +303,15 @@
                 break
 
             if prop.isdigit() and 0 < int(prop) < 6:
                 key = props[int(prop)]
                 key2 = args[int(prop)]
                 val = self.args.get(key2)
                 showtext(
-                    "Enter new property value or leave empty for no value."
-                )
+                    "Enter new property value or leave empty for no value.")
                 response = get_input(f"{key.title()} ({val}): ")
                 self.sanatize_response(key2, response)
 
             else:
                 showtext("Invalid input: Try again.")
         edit_torrent(self.metafile, self.args)
 
@@ -353,50 +344,45 @@
 
     def get_props(self):
         """
         Gather details for torrentfile from user.
 
         @Deprecated
         """
-        piece_length = get_input(
-            "Piece Length (empty=auto): ", lambda x: x.isdigit()
-        )
+        piece_length = get_input("Piece Length (empty=auto): ",
+                                 lambda x: x.isdigit())
 
         self.kwargs["piece_length"] = piece_length
-        announce = get_input(
-            "Tracker list (empty): ", lambda x: isinstance(x, str)
-        )
+        announce = get_input("Tracker list (empty): ",
+                             lambda x: isinstance(x, str))
 
         if announce:
             self.kwargs["announce"] = announce.split()
 
-        url_list = get_input(
-            "Web Seed {GetRight} list (empty): ", lambda x: isinstance(x, str)
-        )
+        url_list = get_input("Web Seed {GetRight} list (empty): ",
+                             lambda x: isinstance(x, str))
 
-        httpseeds = get_input(
-            "Web Seed {Hoffman} list (empty): ", lambda x: isinstance(x, str)
-        )
+        httpseeds = get_input("Web Seed {Hoffman} list (empty): ",
+                              lambda x: isinstance(x, str))
 
         if url_list:
             self.kwargs["url_list"] = url_list.split()
         if httpseeds:
             self.kwargs["httpseeds"] = httpseeds.split()
         comment = get_input("Comment (empty): ", None)
 
         if comment:
             self.kwargs["comment"] = comment
         source = get_input("Source (empty): ", None)
 
         if source:
             self.kwargs["source"] = source
 
-        private = get_input(
-            "Private Torrent? {Y/N}: (N)", lambda x: x in "yYnN"
-        )
+        private = get_input("Private Torrent? {Y/N}: (N)",
+                            lambda x: x in "yYnN")
 
         if private and private.lower() == "y":
             self.kwargs["private"] = 1
 
         contents = get_input("Content Path: ", os.path.exists)
         self.kwargs["path"] = contents
 
@@ -404,17 +390,16 @@
             f"Output Path ({contents}.torrent): ",
             lambda x: os.path.exists(os.path.dirname(x)),
         )
 
         if outfile:
             self.kwargs["outfile"] = outfile
 
-        meta_version = get_input(
-            "Meta Version {1,2,3}: (1)", lambda x: x in "123"
-        )
+        meta_version = get_input("Meta Version {1,2,3}: (1)",
+                                 lambda x: x in "123")
 
         showcenter(f"creating {outfile}")
 
         if meta_version == "3":
             torrent = TorrentFileHybrid(**self.kwargs)
         elif meta_version == "2":
             torrent = TorrentFileV2(**self.kwargs)
```

### Comparing `torrentfile-0.8.8/torrentfile/mixins.py` & `torrentfile-0.9.0/torrentfile/mixins.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,257 +1,259 @@
-#! /usr/bin/python3
-# -*- coding: utf-8 -*-
-
-##############################################################################
-#    Copyright (C) 2021-current alexpdev
-#
-#    Licensed under the Apache License, Version 2.0 (the "License");
-#    you may not use this file except in compliance with the License.
-#    You may obtain a copy of the License at
-#
-#        http://www.apache.org/licenses/LICENSE-2.0
-#
-#    Unless required by applicable law or agreed to in writing, software
-#    distributed under the License is distributed on an "AS IS" BASIS,
-#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#    See the License for the specific language governing permissions and
-#    limitations under the License.
-##############################################################################
-"""
-Collection of classes that can be used as Mixins with other base classes.
-
-Classes such as TorrentFile, TorrentFilev2, and all Hasher classes can use the
-progress bar mixin.  And any class is eligible to use the callback mixin.
-"""
-import math
-import os
-import shutil
-import sys
-import time
-from pathlib import Path
-
-from torrentfile.utils import debug_is_on
-
-
-class CbMixin:
-    """
-    Mixin class to set a callback during hashing procedure.
-    """
-
-    @classmethod
-    def cb(cls, *args, **kwargs):
-        """Do nothing."""
-
-    @classmethod
-    def set_callback(cls, func):
-        """
-        Assign a callback to the Hashing class.
-
-        Parameters
-        ----------
-        func : Callable
-            the callback function
-        """
-        cls.cb = func  # pragma: nocover
-
-
-class ProgressBar:
-    """
-    Holds the state and details of the terminal progress bars.
-
-    Parameters
-    ----------
-    total : int
-        the total amount to be accumulated.
-    title : str
-        the subject of the progress tracker
-    length : int
-        the width of the progress bar
-    unit : str
-        the text representation incremented
-    start : int
-        column where the progress bar should be drawn
-    """
-
-    def __init__(
-        self, total: int, title: str, length: int, unit: str, start: int
-    ):
-        """
-        Construct the progress bar object and store state of it's properties.
-        """
-        self.total = total
-        self.start = start
-        self.length = length
-        self.fill = chr(9608)
-        self.empty = chr(9617)
-        self.state = 0
-        self.unit = unit
-        self.show_total = total
-        if not unit:
-            self.unit = ""  # pragma: nocover
-        elif unit == "bytes":
-            if self.total > 1_000_000_000:
-                self.show_total = math.floor(self.total / (2**30))
-                self.unit = "GiB"
-            elif self.total > 1_000_000:
-                self.show_total = math.floor(self.total / 1048576)
-                self.unit = "MiB"
-            elif self.total > 10000:
-                self.show_total = math.floor(self.total / 1024)
-                self.unit = "KiB"
-        self.suffix = f"/{self.show_total} {self.unit}"
-        title = str(title)
-        if len(title) > start:
-            title = title[: start - 1]  # pragma: nocover
-        padding = (start - len(title)) * " "
-        self.prefix = "".join([title, padding])
-
-    def get_progress(self) -> str:
-        """
-        Return the size of the filled portion of the progress bar.
-
-        Returns
-        -------
-        str :
-            the progress bar characters
-        """
-        if self.state >= self.total:
-            fill = self.length
-        else:
-            fill = math.ceil((self.state / self.total) * self.length)
-        empt = self.length - fill
-        if self.unit == "GiB":
-            state = math.floor(self.state / (2**30))
-        elif self.unit == "MiB":
-            state = math.floor(self.state / 1048576)
-        elif self.unit == "KiB":
-            state = math.floor(self.state / 1024)
-        else:
-            state = self.state
-        progbar = ["|", self.fill * fill, self.empty * empt, "| ", str(state)]
-        return "".join(progbar)
-
-
-class ProgMixin:
-    """
-    Progress bar mixin class.
-
-    Displays progress of hashing individual files, usefull when hashing
-    really big files.
-    """
-
-    def prog_start(
-        self, total: int, path: str, length: int = 50, unit: str = None
-    ):
-        """
-        Generate a new progress bar for the given file path.
-
-        Parameters
-        ----------
-        total : int
-            the total amount of units accumulating towards.
-        path : str
-            path to file being hashed.
-        length : int
-            the number of characters of the actual progress bar.
-        unit : str
-            the text representation of the value being measured.
-        """
-        title = path
-        width = shutil.get_terminal_size().columns
-        if len(str(title)) >= width // 2:
-            parts = list(Path(title).parts)
-            while (len("//".join(parts)) > (width // 2)) and (len(parts) > 0):
-                del parts[0]
-            if parts:
-                title = os.path.join(*parts)
-            else:
-                title = os.path.basename(path)  # pragma: nocover
-        length = min(length, width // 2)
-        start = width - int(length * 1.5)
-        self.prog = ProgressBar(total, title, length, unit, start)
-
-    def prog_update(self, val: int):
-        """
-        Update progress bar.
-
-        Using the value provided, increment the progress bar by that value.
-
-        Parameters
-        ----------
-        val : int
-            the number of bytes count the progress bar should increase.
-        """
-        if self.is_active():
-            self.prog.state += val
-            pbar = self.prog.get_progress()
-            output = f"{self.prog.prefix}{pbar}{self.prog.suffix}\r"
-            sys.stdout.write(output)
-            sys.stdout.flush()
-
-    def prog_close(self):
-        """
-        Finalize the last bits of progress bar.
-
-        Increment the terminal by one line leaving the progress bar in place,
-        and deleting the progress bar object to clear a space for the next one.
-        """
-        if self.is_active():
-            sys.stdout.flush()
-            sys.stdout.write("\n")
-            del self.prog
-
-    def is_active(self) -> bool:
-        """
-        Test to see if there is an active progress bar for object.
-
-        Returns
-        -------
-        bool :
-            True if there is, otherwise False.
-        """
-        if not debug_is_on() and hasattr(self, "prog"):
-            return True
-        return False
-
-
-def waiting(msg: str, flag: list, timeout: int = 20):
-    """
-    Show loading message while thread completes processing.
-
-    Parameters
-    ----------
-    msg : str
-        Message string printed before the progress bar
-    flag : list
-        Once flag is filled exit loop
-    timeout : int
-        max amount of time to run the function.
-    """
-    then = time.time()
-    codes, fill = list(range(9617, 9620)), chr(9619)
-    size = idx = 0
-    total = shutil.get_terminal_size().columns - len(msg) - 20
-
-    def output(text: str):
-        """
-        Print parameter message to the console.
-
-        Parameters
-        ----------
-        text : str
-            output message
-        """
-        sys.stdout.write(text)
-        sys.stdout.flush()
-
-    output("\n")
-    time.sleep(0.16)
-    while len(flag) == 0:
-        time.sleep(0.16)
-        filled = (fill * size) + chr(codes[idx]) + (" " * (total - size))
-        output(f"{msg}: {filled}\r")
-        idx = idx + 1 if idx + 1 < len(codes) else 0
-        size = size + 1 if size < total else 0
-        if time.time() - then > timeout:
-            break
-    output("\n")
+#! /usr/bin/python3
+# -*- coding: utf-8 -*-
+
+##############################################################################
+#    Copyright (C) 2021-current alexpdev
+#
+#    Licensed under the Apache License, Version 2.0 (the "License");
+#    you may not use this file except in compliance with the License.
+#    You may obtain a copy of the License at
+#
+#        http://www.apache.org/licenses/LICENSE-2.0
+#
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS,
+#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#    See the License for the specific language governing permissions and
+#    limitations under the License.
+##############################################################################
+"""
+Collection of classes that can be used as Mixins with other base classes.
+
+Classes such as TorrentFile, TorrentFilev2, and all Hasher classes can use the
+progress bar mixin.  And any class is eligible to use the callback mixin.
+"""
+import os
+import sys
+import math
+import time
+import shutil
+from pathlib import Path
+
+from torrentfile.utils import debug_is_on
+
+
+class CbMixin:
+    """
+    Mixin class to set a callback hook during procedure.
+    """
+
+    @classmethod
+    def cb(cls, *args, **kwargs):
+        """Do nothing."""
+
+    @classmethod
+    def set_callback(cls, func):
+        """
+        Assign a callback to the Hashing class.
+
+        Parameters
+        ----------
+        func : Callable
+            the callback function
+        """
+        cls.cb = func  # pragma: nocover
+
+
+class ProgressBar:
+    """
+    Holds the state and details of the terminal progress bars.
+
+    Parameters
+    ----------
+    total : int
+        the total amount to be accumulated.
+    title : str
+        the subject of the progress tracker
+    length : int
+        the width of the progress bar
+    unit : str
+        the text representation incremented
+    start : int
+        column where the progress bar should be drawn
+    """
+
+    def __init__(self, total: int, title: str, length: int, unit: str,
+                 start: int):
+        """
+        Construct the progress bar object and store state of it's properties.
+        """
+        self.total = total
+        self.start = start
+        self.length = length
+        self.fill = chr(9608)
+        self.empty = chr(9617)
+        self.state = 0
+        self.unit = unit
+        self.show_total = total
+        if not unit:
+            self.unit = ""  # pragma: nocover
+        elif unit == "bytes":
+            if self.total > 1_000_000_000:
+                self.show_total = self.total / (2**30)
+                self.unit = "GiB"
+            elif self.total > 1_000_000:
+                self.show_total = self.total / 1048576
+                self.unit = "MiB"
+            elif self.total > 10000:
+                self.show_total = self.total / 1024
+                self.unit = "KiB"
+        self.suffix = f"/{self.show_total:.02f} {self.unit}"
+        title = str(title)
+        if len(title) > start:
+            title = title[:start - 1]  # pragma: nocover
+        padding = (start - len(title)) * " "
+        self.prefix = "".join([title, padding])
+
+    def get_progress(self) -> str:
+        """
+        Return the size of the filled portion of the progress bar.
+
+        Returns
+        -------
+        str :
+            the progress bar characters
+        """
+        if self.state >= self.total:
+            fill = self.length
+        else:
+            fill = math.ceil((self.state / self.total) * self.length)
+        empty = self.length - fill
+        pbar = ["|", self.fill * fill, self.empty * empty, "| "]
+        if self.unit == "GiB":
+            state = self.state / (2**30)
+        elif self.unit == "MiB":
+            state = self.state / 1048576
+        elif self.unit == "KiB":
+            state = self.state / 1024
+        else:
+            state = self.state
+        pbar.append(f"{state:.02f}")
+        return "".join(pbar)
+
+
+class ProgMixin:
+    """
+    Progress bar mixin class.
+
+    Displays progress of hashing individual files, usefull when hashing
+    really big files.
+    """
+
+    def prog_start(self,
+                   total: int,
+                   path: str,
+                   length: int = 50,
+                   unit: str = "bytes"):
+        """
+        Generate a new progress bar for the given file path.
+
+        Parameters
+        ----------
+        total : int
+            the total amount of units accumulating towards.
+        path : str
+            path to file being hashed.
+        length : int
+            the number of characters of the actual progress bar.
+        unit : str
+            the text representation of the value being measured.
+        """
+        title = path
+        width = shutil.get_terminal_size().columns
+        if len(str(title)) >= width // 2:
+            parts = list(Path(title).parts)
+            while (len("//".join(parts)) > (width // 2)) and (len(parts) > 0):
+                del parts[0]
+            if parts:
+                title = os.path.join(*parts)
+            else:
+                title = os.path.basename(path)  # pragma: nocover
+        length = min(length, width // 2)
+        start = width - int(length * 1.5)
+        self.prog = ProgressBar(total, title, length, unit, start)
+
+    def prog_update(self, val: int):
+        """
+        Update progress bar.
+
+        Using the value provided, increment the progress bar by that value.
+
+        Parameters
+        ----------
+        val : int
+            the number of bytes count the progress bar should increase.
+        """
+        if self.is_active():
+            self.prog.state += val
+            pbar = self.prog.get_progress()
+            output = f"{self.prog.prefix}{pbar}{self.prog.suffix}\r"
+            sys.stdout.write(output)
+            sys.stdout.flush()
+
+    def prog_close(self):
+        """
+        Finalize the last bits of progress bar.
+
+        Increment the terminal by one line leaving the progress bar in place,
+        and deleting the progress bar object to clear a space for the next one.
+        """
+        if self.is_active():
+            sys.stdout.flush()
+            sys.stdout.write("\n")
+            del self.prog
+
+    def is_active(self) -> bool:
+        """
+        Test to see if there is an active progress bar for object.
+
+        Returns
+        -------
+        bool :
+            True if there is, otherwise False.
+        """
+        if not debug_is_on() and hasattr(self, "prog"):
+            return True
+        return False
+
+
+def waiting(msg: str, flag: list, timeout: int = 20):
+    """
+    Show loading message while thread completes processing.
+
+    Parameters
+    ----------
+    msg : str
+        Message string printed before the progress bar
+    flag : list
+        Once flag is filled exit loop
+    timeout : int
+        max amount of time to run the function.
+    """
+    then = time.time()
+    codes, fill = list(range(9617, 9620)), chr(9619)
+    size = idx = 0
+    total = shutil.get_terminal_size().columns - len(msg) - 20
+
+    def output(text: str):
+        """
+        Print parameter message to the console.
+
+        Parameters
+        ----------
+        text : str
+            output message
+        """
+        sys.stdout.write(text)
+        sys.stdout.flush()
+
+    output("\n")
+    time.sleep(0.16)
+    while len(flag) == 0:
+        time.sleep(0.16)
+        filled = (fill * size) + chr(codes[idx]) + (" " * (total - size))
+        output(f"{msg}: {filled}\r")
+        idx = idx + 1 if idx + 1 < len(codes) else 0
+        size = size + 1 if size < total else 0
+        if time.time() - then > timeout:
+            break
+    output("\n")
```

### Comparing `torrentfile-0.8.8/torrentfile/rebuild.py` & `torrentfile-0.9.0/torrentfile/rebuild.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,616 +1,609 @@
-#! /usr/bin/python3
-# -*- coding: utf-8 -*-
-
-##############################################################################
-#    Copyright (C) 2021-current alexpdev
-#
-#    Licensed under the Apache License, Version 2.0 (the "License");
-#    you may not use this file except in compliance with the License.
-#    You may obtain a copy of the License at
-#
-#        http://www.apache.org/licenses/LICENSE-2.0
-#
-#    Unless required by applicable law or agreed to in writing, software
-#    distributed under the License is distributed on an "AS IS" BASIS,
-#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#    See the License for the specific language governing permissions and
-#    limitations under the License.
-##############################################################################
-"""
-Clases and functions for the rebuild or reassemble subcommand.
-
-Re-assemble a torrent into the propper directory structure as indicated by a
-torrent meta file, and validate the contents of each file allong the
-way. Displays a progress bar for each torrent.
-"""
-import logging
-import math
-import os
-from hashlib import sha1
-from pathlib import Path
-
-import pyben
-
-from torrentfile.hasher import HasherV2
-from torrentfile.mixins import CbMixin, ProgMixin
-from torrentfile.utils import copypath
-
-logger = logging.getLogger(__name__)
-SHA1 = 20
-
-
-class PathNode:
-    """
-    Base class representing information regarding a file included in torrent.
-    """
-
-    def __init__(
-        self,
-        start: int = None,
-        stop: int = None,
-        full: str = None,
-        filename: str = None,
-        path: str = None,
-        length: int = None,
-    ):
-        """
-        Hold file information that contributes to the contents of torrent.
-
-        Parameters
-        ----------
-        start : int, optional
-            where the piece starts, by default None
-        stop : int, optional
-            where the piece ends, by default None
-        full : str, optional
-            full path, by default None
-        filename : str, optional
-            filename, by default None
-        path : str, optional
-            parent path, by default None
-        length : int, optional
-            size, by default None
-        """
-        self.path = path
-        self.start = start
-        self.stop = stop
-        self.length = length
-        self.filename = filename
-        self.full = full
-
-    def get_part(self, path: str) -> bytes:
-        """
-        Extract the part of the file needed to complete the hash.
-
-        Parameters
-        ----------
-        path : str
-            filesystem path location of file.
-
-        Returns
-        -------
-        bytes
-            part of the file's contents
-        """
-        with open(path, "rb") as fd:
-            if self.start:
-                fd.seek(self.start)
-            if self.stop != -1:
-                partial = fd.read(self.stop - self.start)
-            else:
-                partial = fd.read()
-        return partial
-
-    def __len__(self) -> int:
-        """
-        Return size of the file.
-
-        Returns
-        -------
-        int
-            total size
-        """
-        return self.length
-
-
-class PieceNode:
-    """
-    Base class representing a single SHA1 hash block of data from a torrent.
-    """
-
-    def __init__(self, piece: bytes):
-        """
-        Store information about an individual SHA1 hash for a torrent file.
-
-        _extended_summary_
-
-        Parameters
-        ----------
-        piece : bytes
-            SHA1 hash bytes
-        """
-        self.piece = piece
-        self.paths = []
-        self.result = None
-        self.dest = None
-
-    def append(self, pathnode: PathNode):
-        """
-        Append the path argument to the paths list attribute.
-
-        Parameters
-        ----------
-        pathnode : PathNode
-            the pathnode
-        """
-        self.paths.append(pathnode)
-
-    def _find_matches(self, filemap: dict, paths: list, data: bytes) -> bool:
-        """
-        Gather relavent sections of the files in the list and check the hash.
-
-        Parameters
-        ----------
-        filemap : dict
-            dictionary containing filename and path details
-        paths : list
-            list of pathnodes
-        data : bytes
-            raw file contents
-
-        Returns
-        -------
-        bool
-            success state
-        """
-        if not paths:
-            piece_hash = sha1(data).digest()  # nosec
-            return piece_hash == self.piece
-        pathnode = paths[0]
-        filename = pathnode.filename
-        if filename not in filemap:
-            return False  # pragma: nocover
-        for loc, size in filemap[filename]:
-            if size != len(pathnode):
-                continue
-            partial = pathnode.get_part(loc)
-            val = self._find_matches(filemap, paths[1:], data + partial)
-            if val:
-                dest_path = os.path.join(self.dest, pathnode.full)
-                copypath(loc, dest_path)
-            return val
-        return False
-
-    def find_matches(self, filemap: dict, dest: str) -> bool:
-        """
-        Find the matching files for each path in the node.
-
-        Parameters
-        ----------
-        filemap : dict
-            filename and details
-        dest : str
-            target destination path
-
-        Returns
-        -------
-        bool
-            success status
-        """
-        self.dest = dest
-        self.result = self._find_matches(filemap, self.paths[:], bytes())
-        return self.result
-
-
-class Metadata(CbMixin, ProgMixin):
-    """
-    Class containing the metadata contents of a torrent file.
-    """
-
-    def __init__(self, path: str):
-        """
-        Construct metadata object for torrent info.
-
-        Parameters
-        ----------
-        path : str
-            path to the .torrent file.
-        """
-        self.path = os.path.abspath(path)
-        self.name = None
-        self.piece_length = 1
-        self.meta_version = 1
-        self.pieces = b""
-        self.piece_nodes = []
-        self.length = 0
-        self.files = []
-        self.filenames = set()
-        self.extract()
-        if self.meta_version == 2:
-            self.num_pieces = len(self.filenames)
-        else:
-            self.num_pieces = math.ceil(len(self.pieces) / SHA1)
-
-    def extract(self):
-        """
-        Decode and extract information for the .torrent file.
-        """
-        meta = pyben.load(self.path)
-        info = meta["info"]
-        self.piece_length = info["piece length"]
-        self.name = info["name"]
-        self.meta_version = info.get("meta version", 1)
-        self.pieces = info.get("pieces", bytes())
-        if self.meta_version == 2:
-            self._parse_tree(info["file tree"], [self.name])
-        elif "length" in info:
-            self.length += info["length"]
-            self.is_file = True
-            self.filenames.add(info["name"])
-            self.files.append(
-                {
-                    "path": Path(self.name).parent,
-                    "filename": self.name,
-                    "full": self.name,
-                    "length": self.length,
-                }
-            )
-        elif "files" in info:
-            for f in info["files"]:
-                path = f["path"]
-                full = os.path.join(self.name, *path)
-                self.files.append(
-                    {
-                        "path": Path(full).parent,
-                        "filename": path[-1],
-                        "full": full,
-                        "length": f["length"],
-                    }
-                )
-                self.length += f["length"]
-                self.filenames.add(path[-1])
-
-    def _map_pieces(self):
-        """
-        Create PathNode and PieceNode details for each piece in the torrent.
-        """
-        total_pieces = len(self.pieces) // SHA1
-        remainder = file_index = 0
-        current = {}
-        for i in range(total_pieces):
-            begin = SHA1 * i
-            piece = PieceNode(self.pieces[begin: begin + SHA1])
-            target = self.piece_length
-            if remainder:
-                start = current["length"] - remainder
-                if remainder < target:
-                    stop = -1
-                    target -= remainder
-                    remainder = 0
-                    file_index += 1
-                else:
-                    stop = start + target
-                    remainder -= target
-                    target -= target
-                pathnode = PathNode(start=start, stop=stop, **current)
-                piece.append(pathnode)
-            while target > 0 and file_index < len(self.files):
-                start = 0
-                current = self.files[file_index]
-                size = current["length"]
-                if size < target:
-                    stop = -1
-                    target -= size
-                    file_index += 1
-                else:
-                    stop = target
-                    remainder = size - target
-                    target = 0
-                pathnode = PathNode(start=start, stop=stop, **current)
-                piece.append(pathnode)
-            self.piece_nodes.append(piece)
-
-    def _parse_tree(self, tree: dict, partials: list):
-        """
-        Parse the file tree dictionary of the torrent metafile.
-
-        Parameters
-        ----------
-        tree : dict
-            the dictionary representation of a file tree.
-        partials : list
-            list of paths leading up to the current key value.
-        """
-        for key, val in tree.items():
-            if "" in val:
-                self.filenames.add(key)
-                path = Path(os.path.join(*partials))
-                full = Path(os.path.join(path, key))
-                length = val[""]["length"]
-                root = val[""]["pieces root"]
-                self.files.append(
-                    {
-                        "path": path,
-                        "full": full,
-                        "filename": key,
-                        "length": length,
-                        "root": root,
-                    }
-                )
-                self.length += length
-            else:
-                self._parse_tree(val, partials + [key])
-
-    def _match_v1(self, filemap: dict, dest: str):
-        """
-        Check each of the nodes against the filemap dictionary for matches.
-
-        Parameters
-        ----------
-        filemap : dict
-            filenames and filesystem information
-        dest : str
-            target destination path
-        """
-        self._map_pieces()
-        copied = []
-        for piece_node in self.piece_nodes:
-            paths = piece_node.paths
-            if len(paths) == 1 and paths[0].path in copied:
-                self._update()
-                continue
-            if piece_node.find_matches(filemap, dest):
-                for pathnode in paths:
-                    if pathnode.path not in copied:
-                        copied.append(pathnode.path)
-                        dest_path = os.path.join(dest, pathnode.path)
-                        self._update()
-                        self.cb(pathnode.path, dest_path, self.num_pieces)
-
-    def _match_v2(self, filemap: dict, dest: str):
-        """
-        Rebuild method for torrent v2 files.
-
-        Parameters
-        ----------
-        filemap : dict
-            filesystem information
-        dest : str
-            destiantion path
-        """
-        for entry in self.files:
-            filename = entry["filename"]
-            length = entry["length"]
-            if filename not in filemap:
-                continue  # pragma: nocover
-            paths = filemap[filename]
-            for path, size in paths:
-                if size == length:
-                    hasher = HasherV2(path, self.piece_length, True)
-                    if entry["root"] == hasher.root:
-                        dest_path = os.path.join(dest, entry["full"])
-                        copypath(entry["path"], dest_path)
-                        self._update()
-                        self.cb(path, dest_path, self.num_pieces)
-                        break
-
-    def rebuild(self, filemap: dict, dest: str):
-        """
-        Rebuild torrent file contents from filemap at dest.
-
-        Searches through the contents of the meta file and compares filenames
-        with those in the filemap dict, and if found checks their contents,
-        and copies them to the destination path.
-
-        Parameters
-        ----------
-        filemap : dict
-            filesystem information
-        dest : str
-            destiantion path
-        """
-        self._prog = None
-        if self.meta_version == 2:
-            self._match_v2(filemap, dest)
-        else:
-            self._match_v1(filemap, dest)
-        if self._prog is not None:
-            self.prog_close()
-
-    def _update(self):
-        """Start and updating the progress bar."""
-        if self._prog is None:
-            self._prog = True
-            self.prog_start(self.num_pieces, self.name, unit="piece")
-        self.prog_update(1)
-
-
-class Assembler(CbMixin):
-    """
-    Does most of the work in attempting the structure of torrentfiles.
-
-    Requires three paths as arguments.
-    - torrent metafile or directory containing multiple meta files
-    - directory containing the contents of meta file
-    - directory where torrents will be re-assembled
-    """
-
-    def __init__(self, metafiles: list, contents: list, dest: str):
-        """
-        Reassemble given torrent file from given cli arguments.
-
-        Rebuild metafiles and contents into their original directory
-        structure as much as possible in the destination directory.
-        Takes two paths as parameters,
-        - file or directory containing 1 or more torrent meta files
-        - path to where the contents are belived to be located.
-
-        Parameters
-        ----------
-        metafiles : str
-            path to torrent metafile or directory containing torrent metafiles.
-        contents : str
-            path to content or directory containing content that belongs to
-            torrentfile.
-        dest: str
-            path to the directory where rebuild will take place.
-        """
-        Metadata.set_callback(self._callback)
-        self.counter = 0
-        self._lastlog = None
-        self.contents = contents
-        self.dest = dest
-        self.meta_paths = metafiles
-        self.metafiles = self._get_metafiles()
-        filenames = set()
-        for meta in self.metafiles:
-            filenames |= meta.filenames
-        self.filemap = _index_contents(self.contents, filenames)
-
-    def _callback(self, filename: str, dest: str, num_pieces: int):
-        """
-        Run the callback functions associated with Mixin for copied files.
-
-        Parameters
-        ----------
-        filename : str
-            filename
-        dest : str
-            destination path
-        num_pieces : int
-            number of hash pieces
-        """
-        self.counter += 1
-        message = f"Matched:{num_pieces} {filename} -> {dest}"
-        if message != self._lastlog:
-            self._lastlog = message
-            logger.debug(message)
-
-    def assemble_torrents(self):
-        """
-        Assemble collection of torrent files into original structure.
-
-        Returns
-        -------
-        int
-            number of files copied
-        """
-        for metafile in self.metafiles:
-            logger.info(
-                "#%s Searching contents for %s", self.counter, metafile.name
-            )
-            self.rebuild(metafile)
-        return self.counter
-
-    def rebuild(self, metafile: Metadata) -> None:
-        """
-        Build the torrent file structure from contents of directory.
-
-        Traverse contents dir and compare discovered files
-        with files listed in torrent metadata and copy
-        the matches to the destination directory respecting folder
-        structures along the way.
-        """
-        metafile.rebuild(self.filemap, self.dest)
-
-    def _iter_files(self, path: str) -> list:
-        """
-        Iterate through metfiles directory createing Metafile objects.
-
-        Parameters
-        ----------
-        path : str
-            fs path
-
-        Returns
-        -------
-        list
-            list of Metadata Object
-        """
-        metafiles = []
-        for filename in os.listdir(path):
-            if filename.lower().endswith(".torrent"):
-                try:
-                    meta = Metadata(os.path.join(path, filename))
-                    metafiles.append(meta)
-                except ValueError:  # pragma: nocover
-                    self.counter -= 1
-        return metafiles
-
-    def _get_metafiles(self) -> list:
-        """
-        Collect all .torrent meta files from given directory or file.
-
-        Returns
-        -------
-        list
-            metafile objects
-        """
-        metafiles = []
-        for path in self.meta_paths:
-            if os.path.exists(path):
-                if os.path.isdir(path):
-                    metafiles += self._iter_files(path)
-                elif path.lower().endswith(".torrent"):
-                    meta = Metadata(path)
-                    metafiles.append(meta)
-        return metafiles
-
-
-def _index_contents(contents: list, filenames: set) -> dict:
-    """
-    Collect all of the filenames and their respective paths.
-
-    Parameters
-    ----------
-    contents : list
-        paths to traverse looking for filenames
-    filenames : set
-        set of filenames to look for
-
-    Returns
-    -------
-    dict
-        all filenames and their respective paths.
-    """
-    mapping = {}
-    for dirpath in contents:
-        mapped = _index_content(dirpath, filenames)
-        for key, value in mapped.items():
-            mapping.setdefault(key, [])
-            mapping[key].extend(value)
-    return mapping
-
-
-def _index_content(root: str, filenames: set) -> dict:
-    """
-    Collect filenames from directory or file.
-
-    Parameters
-    ----------
-    root : str
-        path to search for filenames
-    filenames : set
-        set of filenames to search for
-
-    Returns
-    -------
-    dict
-        filenames and their respective paths
-    """
-    filemap = {}
-    if os.path.isfile(root):
-        name = os.path.basename(root)
-        if name in filenames:
-            size = os.path.getsize(root)
-            filemap.setdefault(name, [])
-            filemap[name].append((root, size))
-        return filemap
-    if os.path.isdir(root):
-        for path in os.listdir(root):
-            fullpath = os.path.join(root, path)
-            resultmap = _index_content(fullpath, filenames)
-            for key, value in resultmap.items():
-                filemap.setdefault(key, [])
-                filemap[key].extend(value)
-    return filemap
+#! /usr/bin/python3
+# -*- coding: utf-8 -*-
+
+##############################################################################
+#    Copyright (C) 2021-current alexpdev
+#
+#    Licensed under the Apache License, Version 2.0 (the "License");
+#    you may not use this file except in compliance with the License.
+#    You may obtain a copy of the License at
+#
+#        http://www.apache.org/licenses/LICENSE-2.0
+#
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS,
+#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#    See the License for the specific language governing permissions and
+#    limitations under the License.
+##############################################################################
+"""
+Clases and functions for the rebuild or reassemble subcommand.
+
+Re-assemble a torrent into the propper directory structure as indicated by a
+torrent meta file, and validate the contents of each file allong the
+way. Displays a progress bar for each torrent.
+"""
+import os
+import math
+import logging
+from hashlib import sha1
+from pathlib import Path
+
+import pyben
+
+from torrentfile.hasher import HasherV2
+from torrentfile.mixins import CbMixin, ProgMixin
+from torrentfile.utils import copypath
+
+logger = logging.getLogger(__name__)
+SHA1 = 20
+
+
+class PathNode:
+    """
+    Base class representing information regarding a file included in torrent.
+    """
+
+    def __init__(
+        self,
+        start: int = None,
+        stop: int = None,
+        full: str = None,
+        filename: str = None,
+        path: str = None,
+        length: int = None,
+    ):
+        """
+        Hold file information that contributes to the contents of torrent.
+
+        Parameters
+        ----------
+        start : int, optional
+            where the piece starts, by default None
+        stop : int, optional
+            where the piece ends, by default None
+        full : str, optional
+            full path, by default None
+        filename : str, optional
+            filename, by default None
+        path : str, optional
+            parent path, by default None
+        length : int, optional
+            size, by default None
+        """
+        self.path = path
+        self.start = start
+        self.stop = stop
+        self.length = length
+        self.filename = filename
+        self.full = full
+
+    def get_part(self, path: str) -> bytes:
+        """
+        Extract the part of the file needed to complete the hash.
+
+        Parameters
+        ----------
+        path : str
+            filesystem path location of file.
+
+        Returns
+        -------
+        bytes
+            part of the file's contents
+        """
+        with open(path, "rb") as fd:
+            if self.start:
+                fd.seek(self.start)
+            if self.stop != -1:
+                partial = fd.read(self.stop - self.start)
+            else:
+                partial = fd.read()
+        return partial
+
+    def __len__(self) -> int:
+        """
+        Return size of the file.
+
+        Returns
+        -------
+        int
+            total size
+        """
+        return self.length
+
+
+class PieceNode:
+    """
+    Base class representing a single SHA1 hash block of data from a torrent.
+    """
+
+    def __init__(self, piece: bytes):
+        """
+        Store information about an individual SHA1 hash for a torrent file.
+
+        _extended_summary_
+
+        Parameters
+        ----------
+        piece : bytes
+            SHA1 hash bytes
+        """
+        self.piece = piece
+        self.paths = []
+        self.result = None
+        self.dest = None
+
+    def append(self, pathnode: PathNode):
+        """
+        Append the path argument to the paths list attribute.
+
+        Parameters
+        ----------
+        pathnode : PathNode
+            the pathnode
+        """
+        self.paths.append(pathnode)
+
+    def _find_matches(self, filemap: dict, paths: list, data: bytes) -> bool:
+        """
+        Gather relavent sections of the files in the list and check the hash.
+
+        Parameters
+        ----------
+        filemap : dict
+            dictionary containing filename and path details
+        paths : list
+            list of pathnodes
+        data : bytes
+            raw file contents
+
+        Returns
+        -------
+        bool
+            success state
+        """
+        if not paths:
+            piece_hash = sha1(data).digest()  # nosec
+            return piece_hash == self.piece
+        pathnode = paths[0]
+        filename = pathnode.filename
+        if filename not in filemap:
+            return False  # pragma: nocover
+        for loc, size in filemap[filename]:
+            if size != len(pathnode):
+                continue
+            partial = pathnode.get_part(loc)
+            val = self._find_matches(filemap, paths[1:], data + partial)
+            if val:
+                dest_path = os.path.join(self.dest, pathnode.full)
+                copypath(loc, dest_path)
+            return val
+        return False
+
+    def find_matches(self, filemap: dict, dest: str) -> bool:
+        """
+        Find the matching files for each path in the node.
+
+        Parameters
+        ----------
+        filemap : dict
+            filename and details
+        dest : str
+            target destination path
+
+        Returns
+        -------
+        bool
+            success status
+        """
+        self.dest = dest
+        self.result = self._find_matches(filemap, self.paths[:], bytes())
+        return self.result
+
+
+class Metadata(CbMixin, ProgMixin):
+    """
+    Class containing the metadata contents of a torrent file.
+    """
+
+    def __init__(self, path: str):
+        """
+        Construct metadata object for torrent info.
+
+        Parameters
+        ----------
+        path : str
+            path to the .torrent file.
+        """
+        self.path = os.path.abspath(path)
+        self.name = None
+        self.piece_length = 1
+        self.meta_version = 1
+        self.pieces = b""
+        self.piece_nodes = []
+        self.length = 0
+        self.files = []
+        self.filenames = set()
+        self.extract()
+        if self.meta_version == 2:
+            self.num_pieces = len(self.filenames)
+        else:
+            self.num_pieces = math.ceil(len(self.pieces) / SHA1)
+
+    def extract(self):
+        """
+        Decode and extract information for the .torrent file.
+        """
+        meta = pyben.load(self.path)
+        info = meta["info"]
+        self.piece_length = info["piece length"]
+        self.name = info["name"]
+        self.meta_version = info.get("meta version", 1)
+        self.pieces = info.get("pieces", bytes())
+        if self.meta_version == 2:
+            self._parse_tree(info["file tree"], [self.name])
+        elif "length" in info:
+            self.length += info["length"]
+            self.is_file = True
+            self.filenames.add(info["name"])
+            self.files.append({
+                "path": Path(self.name).parent,
+                "filename": self.name,
+                "full": self.name,
+                "length": self.length,
+            })
+        elif "files" in info:
+            for f in info["files"]:
+                path = f["path"]
+                full = os.path.join(self.name, *path)
+                self.files.append({
+                    "path": Path(full).parent,
+                    "filename": path[-1],
+                    "full": full,
+                    "length": f["length"],
+                })
+                self.length += f["length"]
+                self.filenames.add(path[-1])
+
+    def _map_pieces(self):
+        """
+        Create PathNode and PieceNode details for each piece in the torrent.
+        """
+        total_pieces = len(self.pieces) // SHA1
+        remainder = file_index = 0
+        current = {}
+        for i in range(total_pieces):
+            begin = SHA1 * i
+            piece = PieceNode(self.pieces[begin:begin + SHA1])
+            target = self.piece_length
+            if remainder:
+                start = current["length"] - remainder
+                if remainder < target:
+                    stop = -1
+                    target -= remainder
+                    remainder = 0
+                    file_index += 1
+                else:
+                    stop = start + target
+                    remainder -= target
+                    target -= target
+                pathnode = PathNode(start=start, stop=stop, **current)
+                piece.append(pathnode)
+            while target > 0 and file_index < len(self.files):
+                start = 0
+                current = self.files[file_index]
+                size = current["length"]
+                if size < target:
+                    stop = -1
+                    target -= size
+                    file_index += 1
+                else:
+                    stop = target
+                    remainder = size - target
+                    target = 0
+                pathnode = PathNode(start=start, stop=stop, **current)
+                piece.append(pathnode)
+            self.piece_nodes.append(piece)
+
+    def _parse_tree(self, tree: dict, partials: list):
+        """
+        Parse the file tree dictionary of the torrent metafile.
+
+        Parameters
+        ----------
+        tree : dict
+            the dictionary representation of a file tree.
+        partials : list
+            list of paths leading up to the current key value.
+        """
+        for key, val in tree.items():
+            if "" in val:
+                self.filenames.add(key)
+                path = Path(os.path.join(*partials))
+                full = Path(os.path.join(path, key))
+                length = val[""]["length"]
+                root = val[""]["pieces root"]
+                self.files.append({
+                    "path": path,
+                    "full": full,
+                    "filename": key,
+                    "length": length,
+                    "root": root,
+                })
+                self.length += length
+            else:
+                self._parse_tree(val, partials + [key])
+
+    def _match_v1(self, filemap: dict, dest: str):
+        """
+        Check each of the nodes against the filemap dictionary for matches.
+
+        Parameters
+        ----------
+        filemap : dict
+            filenames and filesystem information
+        dest : str
+            target destination path
+        """
+        self._map_pieces()
+        copied = []
+        for piece_node in self.piece_nodes:
+            paths = piece_node.paths
+            if len(paths) == 1 and paths[0].path in copied:
+                self._update()
+                continue
+            if piece_node.find_matches(filemap, dest):
+                for pathnode in paths:
+                    if pathnode.path not in copied:
+                        copied.append(pathnode.path)
+                        dest_path = os.path.join(dest, pathnode.path)
+                        self._update()
+                        self.cb(pathnode.path, dest_path, self.num_pieces)
+
+    def _match_v2(self, filemap: dict, dest: str):
+        """
+        Rebuild method for torrent v2 files.
+
+        Parameters
+        ----------
+        filemap : dict
+            filesystem information
+        dest : str
+            destiantion path
+        """
+        for entry in self.files:
+            filename = entry["filename"]
+            length = entry["length"]
+            if filename not in filemap:
+                continue  # pragma: nocover
+            paths = filemap[filename]
+            for path, size in paths:
+                if size == length:
+                    hasher = HasherV2(path, self.piece_length, True)
+                    if entry["root"] == hasher.root:
+                        dest_path = os.path.join(dest, entry["full"])
+                        copypath(entry["path"], dest_path)
+                        self._update()
+                        self.cb(path, dest_path, self.num_pieces)
+                        break
+
+    def rebuild(self, filemap: dict, dest: str):
+        """
+        Rebuild torrent file contents from filemap at dest.
+
+        Searches through the contents of the meta file and compares filenames
+        with those in the filemap dict, and if found checks their contents,
+        and copies them to the destination path.
+
+        Parameters
+        ----------
+        filemap : dict
+            filesystem information
+        dest : str
+            destiantion path
+        """
+        self._prog = None
+        if self.meta_version == 2:
+            self._match_v2(filemap, dest)
+        else:
+            self._match_v1(filemap, dest)
+        if self._prog is not None:
+            self.prog_close()
+
+    def _update(self):
+        """Start and updating the progress bar."""
+        if self._prog is None:
+            self._prog = True
+            self.prog_start(self.num_pieces, self.name, unit="piece")
+        self.prog_update(1)
+
+
+class Assembler(CbMixin):
+    """
+    Does most of the work in attempting the structure of torrentfiles.
+
+    Requires three paths as arguments.
+    - torrent metafile or directory containing multiple meta files
+    - directory containing the contents of meta file
+    - directory where torrents will be re-assembled
+    """
+
+    def __init__(self, metafiles: list, contents: list, dest: str):
+        """
+        Reassemble given torrent file from given cli arguments.
+
+        Rebuild metafiles and contents into their original directory
+        structure as much as possible in the destination directory.
+        Takes two paths as parameters,
+        - file or directory containing 1 or more torrent meta files
+        - path to where the contents are belived to be located.
+
+        Parameters
+        ----------
+        metafiles : str
+            path to torrent metafile or directory containing torrent metafiles.
+        contents : str
+            path to content or directory containing content that belongs to
+            torrentfile.
+        dest: str
+            path to the directory where rebuild will take place.
+        """
+        Metadata.set_callback(self._callback)
+        self.counter = 0
+        self._lastlog = None
+        self.contents = contents
+        self.dest = dest
+        self.meta_paths = metafiles
+        self.metafiles = self._get_metafiles()
+        filenames = set()
+        for meta in self.metafiles:
+            filenames |= meta.filenames
+        self.filemap = _index_contents(self.contents, filenames)
+
+    def _callback(self, filename: str, dest: str, num_pieces: int):
+        """
+        Run the callback functions associated with Mixin for copied files.
+
+        Parameters
+        ----------
+        filename : str
+            filename
+        dest : str
+            destination path
+        num_pieces : int
+            number of hash pieces
+        """
+        self.counter += 1
+        message = f"Matched:{num_pieces} {filename} -> {dest}"
+        if message != self._lastlog:
+            self._lastlog = message
+            logger.debug(message)
+
+    def assemble_torrents(self):
+        """
+        Assemble collection of torrent files into original structure.
+
+        Returns
+        -------
+        int
+            number of files copied
+        """
+        for metafile in self.metafiles:
+            logger.info("#%s Searching contents for %s", self.counter,
+                        metafile.name)
+            self.rebuild(metafile)
+        return self.counter
+
+    def rebuild(self, metafile: Metadata) -> None:
+        """
+        Build the torrent file structure from contents of directory.
+
+        Traverse contents dir and compare discovered files
+        with files listed in torrent metadata and copy
+        the matches to the destination directory respecting folder
+        structures along the way.
+        """
+        metafile.rebuild(self.filemap, self.dest)
+
+    def _iter_files(self, path: str) -> list:
+        """
+        Iterate through metfiles directory createing Metafile objects.
+
+        Parameters
+        ----------
+        path : str
+            fs path
+
+        Returns
+        -------
+        list
+            list of Metadata Object
+        """
+        metafiles = []
+        for filename in os.listdir(path):
+            if filename.lower().endswith(".torrent"):
+                try:
+                    meta = Metadata(os.path.join(path, filename))
+                    metafiles.append(meta)
+                except ValueError:  # pragma: nocover
+                    self.counter -= 1
+        return metafiles
+
+    def _get_metafiles(self) -> list:
+        """
+        Collect all .torrent meta files from given directory or file.
+
+        Returns
+        -------
+        list
+            metafile objects
+        """
+        metafiles = []
+        for path in self.meta_paths:
+            if os.path.exists(path):
+                if os.path.isdir(path):
+                    metafiles += self._iter_files(path)
+                elif path.lower().endswith(".torrent"):
+                    meta = Metadata(path)
+                    metafiles.append(meta)
+        return metafiles
+
+
+def _index_contents(contents: list, filenames: set) -> dict:
+    """
+    Collect all of the filenames and their respective paths.
+
+    Parameters
+    ----------
+    contents : list
+        paths to traverse looking for filenames
+    filenames : set
+        set of filenames to look for
+
+    Returns
+    -------
+    dict
+        all filenames and their respective paths.
+    """
+    mapping = {}
+    for dirpath in contents:
+        mapped = _index_content(dirpath, filenames)
+        for key, value in mapped.items():
+            mapping.setdefault(key, [])
+            mapping[key].extend(value)
+    return mapping
+
+
+def _index_content(root: str, filenames: set) -> dict:
+    """
+    Collect filenames from directory or file.
+
+    Parameters
+    ----------
+    root : str
+        path to search for filenames
+    filenames : set
+        set of filenames to search for
+
+    Returns
+    -------
+    dict
+        filenames and their respective paths
+    """
+    filemap = {}
+    if os.path.isfile(root):
+        name = os.path.basename(root)
+        if name in filenames:
+            size = os.path.getsize(root)
+            filemap.setdefault(name, [])
+            filemap[name].append((root, size))
+        return filemap
+    if os.path.isdir(root):
+        for path in os.listdir(root):
+            fullpath = os.path.join(root, path)
+            resultmap = _index_content(fullpath, filenames)
+            for key, value in resultmap.items():
+                filemap.setdefault(key, [])
+                filemap[key].extend(value)
+    return filemap
```

### Comparing `torrentfile-0.8.8/torrentfile/recheck.py` & `torrentfile-0.9.0/torrentfile/recheck.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 The CheckerClass takes a torrentfile and tha path to it's contents.
 It will then iterate through every file and directory contained
 and compare their data to values contained within the torrent file.
 Completion percentages will be printed to screen for each file and
 at the end for the torrentfile as a whole.
 """
 
-import logging
 import os
+import logging
 from hashlib import sha1, sha256  # nosec
 from pathlib import Path
 
 import pyben
 
 from torrentfile.hasher import FileHasher
 from torrentfile.mixins import ProgMixin
@@ -79,16 +79,15 @@
         path : str
             path to content or contents parent directory.
         """
         if not os.path.exists(metafile):
             raise FileNotFoundError
         if os.path.isdir(metafile):
             raise ArgumentError(
-                "The <metafile> must be a .torrent file. Not a directory"
-            )
+                "The <metafile> must be a .torrent file. Not a directory")
         self.last_log = None
         self.log_msg("Checking: %s, %s", metafile, path)
         self.metafile = metafile
         self.total = 0
         self.paths = []
         self.fileinfo = {}
         print("Extracting data from torrent file...")
@@ -137,17 +136,16 @@
         """
         Generate result percentage and store for future calls.
         """
         responses = []
         for response in self.iter_hashes():
             responses.append(response)
 
-        self.log_msg(
-            "Final result for %s recheck:  %s", self.metafile, self._result
-        )
+        self.log_msg("Final result for %s recheck:  %s", self.metafile,
+                     self._result)
 
         return self._result
 
     def log_msg(self, *args, level: int = logging.INFO):
         """
         Log message `msg` to logger and send `msg` to callback hook.
 
@@ -371,21 +369,20 @@
         ------
         piece : bytes
             hash digest for block of torrent data.
         """
         partial = bytearray()
         for i, path in enumerate(self.paths):
             total = self.fileinfo[i]["length"]
-            self.prog_start(total, path, unit="bytes")
+            self.prog_start(total, path)
             self.index = i
             if os.path.exists(path):
                 for piece in self.extract(path, partial):
-                    if (len(piece) == self.piece_length) or (
-                        i + 1 == len(self.paths)
-                    ):
+                    if (len(piece) == self.piece_length) or (i + 1 == len(
+                            self.paths)):
                         yield piece
                     else:
                         partial = piece
 
             else:
                 length = self.fileinfo[i]["length"]
                 for pad in self._gen_padding(partial, length):
@@ -579,15 +576,15 @@
             self.length = self.fileinfo[self.index]["length"]
             self.root_hash = self.fileinfo[self.index]["pieces root"]
             if self.length > self.piece_length:
                 self.pieces = self.piece_layers[self.root_hash]
             else:
                 self.pieces = self.root_hash
             path = self.paths[self.index]
-            self.prog_start(self.length, path, unit="bytes")
+            self.prog_start(self.length, path)
             self.count = 0
             if os.path.exists(self.current):
                 self.hasher = FileHasher(path, self.piece_length, progress=0)
             else:
                 self.hasher = self.Padder(self.length, self.piece_length)
             return True
         if self.index >= len(self.paths):
```

### Comparing `torrentfile-0.8.8/torrentfile/torrent.py` & `torrentfile-0.9.0/torrentfile/torrent.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,728 +1,728 @@
-#! /usr/bin/python3
-# -*- coding: utf-8 -*-
-
-##############################################################################
-#    Copyright (C) 2021-current alexpdev
-#
-#    Licensed under the Apache License, Version 2.0 (the "License");
-#    you may not use this file except in compliance with the License.
-#    You may obtain a copy of the License at
-#
-#        http://www.apache.org/licenses/LICENSE-2.0
-#
-#    Unless required by applicable law or agreed to in writing, software
-#    distributed under the License is distributed on an "AS IS" BASIS,
-#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#    See the License for the specific language governing permissions and
-#    limitations under the License.
-##############################################################################
-"""
-Classes and procedures pertaining to the creation of torrent meta files.
-
-Classes
--------
-
-- `TorrentFile`
-    construct .torrent file.
-
-- `TorrentFileV2`
-    construct .torrent v2 files using provided data.
-
-- `MetaFile`
-    base class for all MetaFile classes.
-
-Constants
----------
-
-- BLOCK_SIZE : int
-    size of leaf hashes for merkle tree.
-
-- HASH_SIZE : int
-    Length of a sha256 hash.
-
-Bittorrent V2
--------------
-
-**From Bittorrent.org Documentation pages.**
-
-*Implementation details for Bittorrent Protocol v2.*
-
-!!!Note
-    All strings in a .torrent file that contain text must be UTF-8 encoded.
-
-### Meta Version 2 Dictionary:
-
-- "announce":
-    The URL of the tracker.
-
-- "info":
-    This maps to a dictionary, with keys described below.
-
-    - "name":
-        A display name for the torrent. It is purely advisory.
-
-    - "piece length":
-        The number of bytes that each logical piece in the peer
-        protocol refers to. I.e. it sets the granularity of piece, request,
-        bitfield and have messages. It must be a power of two and at least
-        6KiB.
-
-    - "meta version":
-        An integer value, set to 2 to indicate compatibility
-        with the current revision of this specification. Version 1 is not
-        assigned to avoid confusion with BEP3. Future revisions will only
-        increment this issue to indicate an incompatible change has been made,
-        for example that hash algorithms were changed due to newly discovered
-        vulnerabilities. Lementations must check this field first and indicate
-        that a torrent is of a newer version than they can handle before
-        performing other idations which may result in more general messages
-        about invalid files. Files are mapped into this piece address space so
-        that each non-empty
-
-    - "file tree":
-        A tree of dictionaries where dictionary keys represent UTF-8
-        encoded path elements. Entries with zero-length keys describe the
-        properties of the composed path at that point. 'UTF-8 encoded'
-        context only means that if the native encoding is known at creation
-        time it must be converted to UTF-8. Keys may contain invalid UTF-8
-        sequences or characters and names that are reserved on specific
-        filesystems. Implementations must be prepared to sanitize them. On
-        platforms path components exactly matching '.' and '..' must be
-        sanitized since they could lead to directory traversal attacks and
-        conflicting path descriptions. On platforms that require UTF-8
-        path components this sanitizing step must happen after normalizing
-        overlong UTF-8 encodings.
-        File is aligned to a piece boundary and occurs in same order as
-        the file tree. The last piece of each file may be shorter than the
-        specified piece length, resulting in an alignment gap.
-
-    - "length":
-        Length of the file in bytes. Presence of this field indicates
-        that the dictionary describes a file, not a directory. Which means
-        it must not have any sibling entries.
-
-    - "pieces root":
-        For non-empty files this is the the root hash of a merkle
-        tree with a branching factor of 2, constructed from 16KiB blocks
-        of the file. The last block may be shorter than 16KiB. The
-        remaining leaf hashes beyond the end of the file required to
-        construct upper layers of the merkle tree are set to zero. As of
-        meta version 2 SHA2-256 is used as digest function for the merkle
-        tree. The hash is stored in its binary form, not as human-readable
-        string.
-
-- "piece layers":
-    A dictionary of strings. For each file in the file tree that
-    is larger than the piece size it contains one string value.
-    The keys are the merkle roots while the values consist of concatenated
-    hashes of one layer within that merkle tree. The layer is chosen so
-    that one hash covers piece length bytes. For example if the piece
-    size is 16KiB then the leaf hashes are used. If a piece size of
-    128KiB is used then 3rd layer up from the leaf hashes is used. Layer
-    hashes which exclusively cover data beyond the end of file, i.e.
-    are only needed to balance the tree, are omitted. All hashes are
-    stored in their binary format. A torrent is not valid if this field is
-    absent, the contained hashes do not match the merkle roots or are
-    not from the correct layer.
-
-!!!important
-    The file tree root dictionary itself must not be a file,
-    i.e. it must not contain a zero-length key with a dictionary containing
-    a length key.
-
-Bittorrent V1
--------------
-
-### v1 meta-dictionary
-
-- announce:
-    The URL of the tracker.
-
-- info:
-    This maps to a dictionary, with keys described below.
-
-    - `name`:
-        maps to a UTF-8 encoded string which is the suggested name to
-        save the file (or directory) as. It is purely advisory.
-
-    - `piece length`:
-        maps to the number of bytes in each piece the file is split
-        into. For the purposes of transfer, files are split into
-        fixed-size pieces which are all the same length except for
-        possibly the last one which may be truncated.
-
-    - `piece length`:
-        is almost always a power of two, most commonly 2^18 = 256 K
-
-    - `pieces`:
-        maps to a string whose length is a multiple of 20. It is to be
-        subdivided into strings of length 20, each of which is the SHA1
-        hash of the piece at the corresponding index.
-
-    - `length`:
-        In the single file case, maps to the length of the file in bytes.
-
-    - `files`:
-        If present then the download represents a single file, otherwise it
-        represents a set of files which go in a directory structure.
-        For the purposes of the other keys, the multi-file case is treated
-        as only having a single file by concatenating the files in the order
-        they appear in the files list. The files list is the value `files`
-        maps to, and is a list of dictionaries containing the following keys:
-
-        - `path`:
-            A list of UTF-8 encoded strings corresponding to subdirectory
-            names, the last of which is the actual file name
-
-        - `length`:
-            Maps to the length of the file in bytes.
-
-    - `length`:
-        Only present if the content is a single file. Maps to the length
-        of the file in bytes.
-
-!!!Note
-    In the single file case, the name key is the name of a file,
-    in the muliple file case, it's the name of a directory.
-"""
-
-import logging
-import os
-from collections.abc import Sequence
-from datetime import datetime
-
-import pyben
-
-from torrentfile import utils
-from torrentfile.hasher import FileHasher, Hasher, HasherHybrid, HasherV2
-from torrentfile.mixins import ProgMixin
-from torrentfile.version import __version__ as version
-
-logger = logging.getLogger(__name__)
-
-
-class MetaFile:
-    """
-    Base Class for all TorrentFile classes.
-
-    Parameters
-    ----------
-    path : str
-        target path to torrent content.  Default: None
-    announce : str
-        One or more tracker URL's.  Default: None
-    comment : str
-        A comment.  Default: None
-    piece_length : int
-        Size of torrent pieces.  Default: None
-    private : bool
-        For private trackers.  Default: None
-    outfile : str
-        target path to write .torrent file. Default: None
-    source : str
-        Private tracker source. Default: None
-    progress : str
-        level of progress bar displayed  Default: "1"
-    cwd : bool
-        If True change default save location to current directory
-    httpseeds : list
-        one or more web addresses where torrent content can be found.
-    url_list : list
-        one or more web addressess where torrent content exists.
-    content : str
-        alias for 'path' arg.
-    meta_version : int
-        indicates which Bittorrent protocol to use for hashing content
-    """
-
-    hasher = None
-
-    @classmethod
-    def set_callback(cls, func):
-        """
-        Assign a callback function for the Hashing class to call for each hash.
-
-        Parameters
-        ----------
-        func : function
-            The callback function which accepts a single paramter.
-        """
-        if "hasher" in vars(cls) and vars(cls)["hasher"]:
-            cls.hasher.set_callback(func)
-
-    def __init__(
-        self,
-        path=None,
-        announce=None,
-        comment=None,
-        piece_length=None,
-        private=False,
-        outfile=None,
-        source=None,
-        progress=1,
-        cwd=False,
-        httpseeds=None,
-        url_list=None,
-        content=None,
-        meta_version=None,
-        **_,
-    ):
-        """
-        Construct MetaFile superclass and assign local attributes.
-        """
-        self.private = private
-        self.cwd = cwd
-        self.outfile = outfile
-        self.progress = int(progress)
-        self.comment = comment
-        self.source = source
-        self.meta_version = meta_version
-
-        if content:
-            path = content
-        if not path:
-            if announce and len(announce) > 1 and os.path.exists(announce[-1]):
-                path = announce[-1]
-                announce = announce[:-1]
-            elif url_list and os.path.exists(url_list[-1]):
-                path = url_list[-1]
-                url_list = url_list[:-1]
-            elif httpseeds and os.path.exists(httpseeds[-1]):
-                path = httpseeds[-1]
-                httpseeds = httpseeds[:-1]
-            else:
-                raise utils.MissingPathError("Path to content is required.")
-
-        # base path to torrent content.
-        self.path = path
-
-        logger.debug("path parameter found %s", path)
-
-        # Format piece_length attribute.
-        if piece_length:
-            self.piece_length = utils.normalize_piece_length(piece_length)
-            logger.debug("piece length parameter found %s", piece_length)
-        else:
-            self.piece_length = utils.path_piece_length(self.path)
-            logger.debug("piece length calculated %s", self.piece_length)
-
-        # Assign announce URL to empty string if none provided.
-        if not announce:
-            self.announce, self.announce_list = "", [[""]]
-
-        # Most torrent clients have editting trackers as a feature.
-        elif isinstance(announce, str):
-            self.announce, self.announce_list = announce, [[announce]]
-
-        elif isinstance(announce, Sequence):
-            self.announce, self.announce_list = announce[0], [announce]
-
-        self.meta = {
-            "announce": self.announce,
-            "announce-list": self.announce_list,
-            "created by": f"TorrentFile_v{version}",
-            "creation date": int(datetime.timestamp(datetime.now())),
-            "info": {},
-        }
-        if comment:
-            self.meta["info"]["comment"] = comment
-            logger.debug("comment parameter found %s", comment)
-        if private:
-            self.meta["info"]["private"] = 1
-            logger.debug("private parameter triggered")
-        if source:
-            self.meta["info"]["source"] = source
-            logger.debug("source parameter found %s", source)
-        if url_list:
-            self.meta["url-list"] = url_list
-            logger.debug("url list parameter found %s", str(url_list))
-        if httpseeds:
-            self.meta["httpseeds"] = httpseeds
-            logger.debug("httpseeds parameter found %s", str(httpseeds))
-        self.meta["info"]["piece length"] = self.piece_length
-
-        self.meta_version = meta_version
-        parent, self.name = os.path.split(self.path)
-        if not self.name:
-            self.name = os.path.basename(parent)
-        self.meta["info"]["name"] = self.name
-
-    def assemble(self):
-        """
-        Overload in subclasses.
-
-        Raises
-        ------
-        Exception
-            NotImplementedError
-        """
-        raise NotImplementedError
-
-    def sort_meta(self):
-        """Sort the info and meta dictionaries."""
-        logger.debug("sorting dictionary keys")
-        meta = self.meta
-        meta["info"] = dict(sorted(list(meta["info"].items())))
-        meta = dict(sorted(list(meta.items())))
-        return meta
-
-    def write(self, outfile=None) -> tuple:
-        """
-        Write meta information to .torrent file.
-
-        Final step in the torrent file creation process.
-        After hashing and sorting every piece of content
-        write the contents to file using the bencode encoding.
-
-        Parameters
-        ----------
-        outfile : str
-            Destination path for .torrent file. default=None
-
-        Returns
-        -------
-        outfile : str
-            Where the .torrent file was writen.
-        meta : dict
-            .torrent meta information.
-        """
-        if outfile:
-            self.outfile = outfile
-        elif self.outfile:
-            pass
-        else:
-            self.outfile = os.path.join(os.getcwd(), self.name) + ".torrent"
-        if str(self.outfile)[-1] in "\\/":
-            self.outfile = self.outfile + (self.name + ".torrent")
-        self.meta = self.sort_meta()
-        try:
-            pyben.dump(self.meta, self.outfile)
-        except PermissionError as excp:
-            logger.error(
-                "Permission Denied: Could not write to %s", self.outfile
-            )
-            raise PermissionError from excp
-        return self.outfile, self.meta
-
-
-class TorrentFile(MetaFile, ProgMixin):
-    """
-    Class for creating Bittorrent meta files.
-
-    Construct *Torrentfile* class instance object.
-
-    Parameters
-    ----------
-    **kwargs : dict
-        Dictionary containing torrent file options.
-    """
-
-    hasher = Hasher
-
-    def __init__(self, **kwargs):
-        """
-        Construct TorrentFile instance with given keyword args.
-
-        Parameters
-        ----------
-        **kwargs : dict
-            dictionary of keyword args passed to superclass.
-        """
-        super().__init__(**kwargs)
-        logger.debug("Assembling bittorrent v1 torrent file")
-        self.assemble()
-
-    def assemble(self):
-        """
-        Assemble components of torrent metafile.
-
-        Returns
-        -------
-        dict
-            metadata dictionary for torrent file
-        """
-        info = self.meta["info"]
-        size, filelist = utils.filelist_total(self.path)
-        if os.path.isfile(self.path):
-            info["length"] = size
-        else:
-            info["files"] = [
-                {
-                    "length": os.path.getsize(path),
-                    "path": os.path.relpath(path, self.path).split(os.sep),
-                }
-                for path in filelist
-            ]
-        pieces = bytearray()
-
-        feeder = Hasher(filelist, self.piece_length, self.progress)
-        for piece in feeder:
-            pieces.extend(piece)
-
-        info["pieces"] = pieces
-
-
-class TorrentFileV2(MetaFile, ProgMixin):
-    """
-    Class for creating Bittorrent meta v2 files.
-
-    Parameters
-    ----------
-    **kwargs : dict
-        Keyword arguments for torrent file options.
-    """
-
-    hasher = HasherV2
-
-    def __init__(self, **kwargs):
-        """
-        Construct `TorrentFileV2` Class instance from given parameters.
-
-        Parameters
-        ----------
-        **kwargs : dict
-            keywword arguments to pass to superclass.
-        """
-        super().__init__(**kwargs)
-        logger.debug("Assembling bittorrent v2 torrent file")
-        self.piece_layers = {}
-        self.hashes = []
-        self.total = len(utils.get_file_list(self.path))
-        self.assemble()
-
-    def assemble(self):
-        """
-        Assemble then return the meta dictionary for encoding.
-
-        Returns
-        -------
-        meta : dict
-            Metainformation about the torrent.
-        """
-        info = self.meta["info"]
-        if os.path.isfile(self.path):
-            info["file tree"] = {info["name"]: self._traverse(self.path)}
-            info["length"] = os.path.getsize(self.path)
-            self.prog_update(info["length"])
-        else:
-            info["file tree"] = self._traverse(self.path)
-
-        info["meta version"] = 2
-        self.meta["piece layers"] = self.piece_layers
-
-    def _traverse(self, path: str) -> dict:
-        """
-        Walk directory tree.
-
-        Parameters
-        ----------
-        path : str
-            Path to file or directory.
-        """
-        if os.path.isfile(path):
-            # Calculate Size and hashes for each file.
-            size = os.path.getsize(path)
-
-            if size == 0:
-                return {"": {"length": size}}
-
-            logger.debug("Hashing %s", str(path))
-            fhash = HasherV2(path, self.piece_length, self.progress)
-
-            if size > self.piece_length:
-                self.piece_layers[fhash.root] = fhash.piece_layer
-            return {"": {"length": size, "pieces root": fhash.root}}
-
-        file_tree = {}
-        if os.path.isdir(path):
-            for name in sorted(os.listdir(path)):
-                file_tree[name] = self._traverse(os.path.join(path, name))
-        return file_tree
-
-
-class TorrentFileHybrid(MetaFile, ProgMixin):
-    """
-    Construct the Hybrid torrent meta file with provided parameters.
-
-    Parameters
-    ----------
-    **kwargs : dict
-        Keyword arguments for torrent options.
-    """
-
-    hasher = HasherHybrid
-
-    def __init__(self, **kwargs):
-        """
-        Create Bittorrent v1 v2 hybrid metafiles.
-        """
-        super().__init__(**kwargs)
-        logger.debug("Assembling bittorrent Hybrid file")
-        self.name = os.path.basename(self.path)
-        self.hashes = []
-        self.piece_layers = {}
-        self.pieces = []
-        self.files = []
-        self.total = len(utils.get_file_list(self.path))
-        self.assemble()
-
-    def assemble(self):
-        """
-        Assemble the parts of the torrentfile into meta dictionary.
-        """
-        info = self.meta["info"]
-        info["meta version"] = 2
-
-        if os.path.isfile(self.path):
-            info["file tree"] = {self.name: self._traverse(self.path)}
-            info["length"] = os.path.getsize(self.path)
-
-        else:
-            info["file tree"] = self._traverse(self.path)
-            info["files"] = self.files
-
-        info["pieces"] = b"".join(self.pieces)
-        self.meta["piece layers"] = self.piece_layers
-        return info
-
-    def _traverse(self, path: str) -> dict:
-        """
-        Build meta dictionary while walking directory.
-
-        Parameters
-        ----------
-        path : str
-            Path to target file.
-        """
-        if os.path.isfile(path):
-            file_size = os.path.getsize(path)
-
-            self.files.append(
-                {
-                    "length": file_size,
-                    "path": os.path.relpath(path, self.path).split(os.sep),
-                }
-            )
-
-            if file_size == 0:
-                return {"": {"length": file_size}}
-
-            logger.debug("Hashing %s", str(path))
-            file_hash = HasherHybrid(path, self.piece_length, self.progress)
-            self.prog_update(file_size)
-
-            if file_size > self.piece_length:
-                self.piece_layers[file_hash.root] = file_hash.piece_layer
-
-            self.hashes.append(file_hash)
-            self.pieces.extend(file_hash.pieces)
-
-            if file_hash.padding_file:
-                self.files.append(file_hash.padding_file)
-
-            return {"": {"length": file_size, "pieces root": file_hash.root}}
-
-        tree = {}
-        if os.path.isdir(path):
-            for name in sorted(os.listdir(path)):
-                tree[name] = self._traverse(os.path.join(path, name))
-        return tree
-
-
-class TorrentAssembler(MetaFile):
-    """
-    Assembler class for Bittorrent version 2 and hybrid meta files.
-
-    This differs from the TorrentFileV2 and TorrentFileHybrid, because
-    it can be used as an iterator and works for both versions.
-
-    Parameters
-    ----------
-    **kwargs : dict
-        Keyword arguments for torrent options.
-    """
-
-    hasher = FileHasher
-
-    def __init__(self, **kwargs):
-        """
-        Create Bittorrent v1 v2 hybrid metafiles.
-        """
-        super().__init__(**kwargs)
-        logger.debug("Assembling bittorrent Hybrid file")
-        self.name = os.path.basename(self.path)
-        self.hashes = []
-        self.piece_layers = {}
-        self.pieces = bytearray()
-        self.files = []
-        self.hybrid = self.meta_version == "3"
-        self.total = len(utils.get_file_list(self.path))
-        self.assemble()
-
-    def assemble(self):
-        """
-        Assemble the parts of the torrentfile into meta dictionary.
-        """
-        info = self.meta["info"]
-        info["meta version"] = 2
-
-        if os.path.isfile(self.path):
-            info["file tree"] = {self.name: self._traverse(self.path)}
-            info["length"] = os.path.getsize(self.path)
-
-        else:
-            info["file tree"] = self._traverse(self.path)
-            if self.hybrid:
-                info["files"] = self.files
-
-        if self.hybrid:
-            info["pieces"] = self.pieces
-        self.meta["piece layers"] = self.piece_layers
-        return info
-
-    def _traverse(self, path: str) -> dict:
-        """
-        Build meta dictionary while walking directory.
-
-        Parameters
-        ----------
-        path : str
-            Path to target file.
-        """
-        if os.path.isfile(path):
-            file_size = os.path.getsize(path)
-            if self.hybrid:
-                self.files.append(
-                    {
-                        "length": file_size,
-                        "path": os.path.relpath(path, self.path).split(os.sep),
-                    }
-                )
-
-            if file_size == 0:
-                return {"": {"length": file_size}}
-
-            logger.debug("Hashing %s", str(path))
-            hasher = FileHasher(
-                path, self.piece_length, progress=True, hybrid=self.hybrid
-            )
-            layers = bytearray()
-            for result in hasher:
-                if self.hybrid:
-                    layer_hash, piece = result
-                    self.pieces.extend(piece)
-                else:
-                    layer_hash = result
-                layers.extend(layer_hash)
-            if file_size > self.piece_length:
-                self.piece_layers[hasher.root] = layers
-            if self.hybrid and hasher.padding_file:
-                self.files.append(hasher.padding_file)
-
-            return {"": {"length": file_size, "pieces root": hasher.root}}
-
-        tree = {}
-        if os.path.isdir(path):
-            for name in sorted(os.listdir(path)):
-                tree[name] = self._traverse(os.path.join(path, name))
-        return tree
+#! /usr/bin/python3
+# -*- coding: utf-8 -*-
+
+##############################################################################
+#    Copyright (C) 2021-current alexpdev
+#
+#    Licensed under the Apache License, Version 2.0 (the "License");
+#    you may not use this file except in compliance with the License.
+#    You may obtain a copy of the License at
+#
+#        http://www.apache.org/licenses/LICENSE-2.0
+#
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS,
+#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#    See the License for the specific language governing permissions and
+#    limitations under the License.
+##############################################################################
+"""
+Classes and procedures pertaining to the creation of torrent meta files.
+
+Classes
+-------
+
+- `TorrentFile`
+    construct .torrent file.
+
+- `TorrentFileV2`
+    construct .torrent v2 files using provided data.
+
+- `MetaFile`
+    base class for all MetaFile classes.
+
+Constants
+---------
+
+- BLOCK_SIZE : int
+    size of leaf hashes for merkle tree.
+
+- HASH_SIZE : int
+    Length of a sha256 hash.
+
+Bittorrent V2
+-------------
+
+**From Bittorrent.org Documentation pages.**
+
+*Implementation details for Bittorrent Protocol v2.*
+
+!!!Note
+    All strings in a .torrent file that contain text must be UTF-8 encoded.
+
+### Meta Version 2 Dictionary:
+
+- "announce":
+    The URL of the tracker.
+
+- "info":
+    This maps to a dictionary, with keys described below.
+
+    - "name":
+        A display name for the torrent. It is purely advisory.
+
+    - "piece length":
+        The number of bytes that each logical piece in the peer
+        protocol refers to. I.e. it sets the granularity of piece, request,
+        bitfield and have messages. It must be a power of two and at least
+        6KiB.
+
+    - "meta version":
+        An integer value, set to 2 to indicate compatibility
+        with the current revision of this specification. Version 1 is not
+        assigned to avoid confusion with BEP3. Future revisions will only
+        increment this issue to indicate an incompatible change has been made,
+        for example that hash algorithms were changed due to newly discovered
+        vulnerabilities. Lementations must check this field first and indicate
+        that a torrent is of a newer version than they can handle before
+        performing other idations which may result in more general messages
+        about invalid files. Files are mapped into this piece address space so
+        that each non-empty
+
+    - "file tree":
+        A tree of dictionaries where dictionary keys represent UTF-8
+        encoded path elements. Entries with zero-length keys describe the
+        properties of the composed path at that point. 'UTF-8 encoded'
+        context only means that if the native encoding is known at creation
+        time it must be converted to UTF-8. Keys may contain invalid UTF-8
+        sequences or characters and names that are reserved on specific
+        filesystems. Implementations must be prepared to sanitize them. On
+        platforms path components exactly matching '.' and '..' must be
+        sanitized since they could lead to directory traversal attacks and
+        conflicting path descriptions. On platforms that require UTF-8
+        path components this sanitizing step must happen after normalizing
+        overlong UTF-8 encodings.
+        File is aligned to a piece boundary and occurs in same order as
+        the file tree. The last piece of each file may be shorter than the
+        specified piece length, resulting in an alignment gap.
+
+    - "length":
+        Length of the file in bytes. Presence of this field indicates
+        that the dictionary describes a file, not a directory. Which means
+        it must not have any sibling entries.
+
+    - "pieces root":
+        For non-empty files this is the the root hash of a merkle
+        tree with a branching factor of 2, constructed from 16KiB blocks
+        of the file. The last block may be shorter than 16KiB. The
+        remaining leaf hashes beyond the end of the file required to
+        construct upper layers of the merkle tree are set to zero. As of
+        meta version 2 SHA2-256 is used as digest function for the merkle
+        tree. The hash is stored in its binary form, not as human-readable
+        string.
+
+- "piece layers":
+    A dictionary of strings. For each file in the file tree that
+    is larger than the piece size it contains one string value.
+    The keys are the merkle roots while the values consist of concatenated
+    hashes of one layer within that merkle tree. The layer is chosen so
+    that one hash covers piece length bytes. For example if the piece
+    size is 16KiB then the leaf hashes are used. If a piece size of
+    128KiB is used then 3rd layer up from the leaf hashes is used. Layer
+    hashes which exclusively cover data beyond the end of file, i.e.
+    are only needed to balance the tree, are omitted. All hashes are
+    stored in their binary format. A torrent is not valid if this field is
+    absent, the contained hashes do not match the merkle roots or are
+    not from the correct layer.
+
+!!!important
+    The file tree root dictionary itself must not be a file,
+    i.e. it must not contain a zero-length key with a dictionary containing
+    a length key.
+
+Bittorrent V1
+-------------
+
+### v1 meta-dictionary
+
+- announce:
+    The URL of the tracker.
+
+- info:
+    This maps to a dictionary, with keys described below.
+
+    - `name`:
+        maps to a UTF-8 encoded string which is the suggested name to
+        save the file (or directory) as. It is purely advisory.
+
+    - `piece length`:
+        maps to the number of bytes in each piece the file is split
+        into. For the purposes of transfer, files are split into
+        fixed-size pieces which are all the same length except for
+        possibly the last one which may be truncated.
+
+    - `piece length`:
+        is almost always a power of two, most commonly 2^18 = 256 K
+
+    - `pieces`:
+        maps to a string whose length is a multiple of 20. It is to be
+        subdivided into strings of length 20, each of which is the SHA1
+        hash of the piece at the corresponding index.
+
+    - `length`:
+        In the single file case, maps to the length of the file in bytes.
+
+    - `files`:
+        If present then the download represents a single file, otherwise it
+        represents a set of files which go in a directory structure.
+        For the purposes of the other keys, the multi-file case is treated
+        as only having a single file by concatenating the files in the order
+        they appear in the files list. The files list is the value `files`
+        maps to, and is a list of dictionaries containing the following keys:
+
+        - `path`:
+            A list of UTF-8 encoded strings corresponding to subdirectory
+            names, the last of which is the actual file name
+
+        - `length`:
+            Maps to the length of the file in bytes.
+
+    - `length`:
+        Only present if the content is a single file. Maps to the length
+        of the file in bytes.
+
+!!!Note
+    In the single file case, the name key is the name of a file,
+    in the muliple file case, it's the name of a directory.
+"""
+
+import os
+import logging
+from collections.abc import Sequence
+from datetime import datetime
+
+import pyben
+
+from torrentfile import utils
+from torrentfile.hasher import FileHasher, Hasher, HasherHybrid, HasherV2
+from torrentfile.mixins import ProgMixin
+from torrentfile.version import __version__ as version
+
+logger = logging.getLogger(__name__)
+
+
+class MetaFile:
+    """
+    Base Class for all TorrentFile classes.
+
+    Parameters
+    ----------
+    path : str
+        target path to torrent content.  Default: None
+    announce : str
+        One or more tracker URL's.  Default: None
+    comment : str
+        A comment.  Default: None
+    piece_length : int
+        Size of torrent pieces.  Default: None
+    private : bool
+        For private trackers.  Default: None
+    outfile : str
+        target path to write .torrent file. Default: None
+    source : str
+        Private tracker source. Default: None
+    progress : str
+        level of progress bar displayed  Default: "1"
+    cwd : bool
+        If True change default save location to current directory
+    httpseeds : list
+        one or more web addresses where torrent content can be found.
+    url_list : list
+        one or more web addressess where torrent content exists.
+    content : str
+        alias for 'path' arg.
+    meta_version : int
+        indicates which Bittorrent protocol to use for hashing content
+    """
+
+    hasher = None
+
+    @classmethod
+    def set_callback(cls, func):
+        """
+        Assign a callback function for the Hashing class to call for each hash.
+
+        Parameters
+        ----------
+        func : function
+            The callback function which accepts a single paramter.
+        """
+        if "hasher" in vars(cls) and vars(cls)["hasher"]:
+            cls.hasher.set_callback(func)
+
+    def __init__(
+        self,
+        path=None,
+        announce=None,
+        comment=None,
+        piece_length=None,
+        private=False,
+        outfile=None,
+        source=None,
+        progress=1,
+        cwd=False,
+        httpseeds=None,
+        url_list=None,
+        content=None,
+        meta_version=None,
+        **_,
+    ):
+        """
+        Construct MetaFile superclass and assign local attributes.
+        """
+        self.private = private
+        self.cwd = cwd
+        self.outfile = outfile
+        self.progress = int(progress)
+        self.comment = comment
+        self.source = source
+        self.meta_version = meta_version
+
+        if content:
+            path = content
+        if not path:
+            if announce and len(announce) > 1 and os.path.exists(announce[-1]):
+                path = announce[-1]
+                announce = announce[:-1]
+            elif url_list and os.path.exists(url_list[-1]):
+                path = url_list[-1]
+                url_list = url_list[:-1]
+            elif httpseeds and os.path.exists(httpseeds[-1]):
+                path = httpseeds[-1]
+                httpseeds = httpseeds[:-1]
+            else:
+                raise utils.MissingPathError("Path to content is required.")
+
+        # base path to torrent content.
+        self.path = path
+
+        logger.debug("path parameter found %s", path)
+
+        self.meta = {
+            "created by": f"TorrentFile_v{version}",
+            "creation date": int(datetime.timestamp(datetime.now())),
+            "info": {},
+        }
+
+        # Format piece_length attribute.
+        if piece_length:
+            self.piece_length = utils.normalize_piece_length(piece_length)
+            logger.debug("piece length parameter found %s", piece_length)
+        else:
+            self.piece_length = utils.path_piece_length(self.path)
+            logger.debug("piece length calculated %s", self.piece_length)
+
+        # Assign announce URL to empty string if none provided.
+        if not announce:
+            self.announce, self.announce_list = "", [[""]]
+
+        # Most torrent clients have editting trackers as a feature.
+        elif isinstance(announce, str):
+            self.announce, self.announce_list = announce, [[announce]]
+
+        elif isinstance(announce, Sequence):
+            self.announce, self.announce_list = announce[0], [announce]
+
+        if self.announce:
+            self.meta["announce"] = self.announce
+            self.meta["announce-list"] = self.announce_list
+        if comment:
+            self.meta["info"]["comment"] = comment
+            logger.debug("comment parameter found %s", comment)
+        if private:
+            self.meta["info"]["private"] = 1
+            logger.debug("private parameter triggered")
+        if source:
+            self.meta["info"]["source"] = source
+            logger.debug("source parameter found %s", source)
+        if url_list:
+            self.meta["url-list"] = url_list
+            logger.debug("url list parameter found %s", str(url_list))
+        if httpseeds:
+            self.meta["httpseeds"] = httpseeds
+            logger.debug("httpseeds parameter found %s", str(httpseeds))
+        self.meta["info"]["piece length"] = self.piece_length
+
+        self.meta_version = meta_version
+        parent, self.name = os.path.split(self.path)
+        if not self.name:
+            self.name = os.path.basename(parent)
+        self.meta["info"]["name"] = self.name
+
+    def assemble(self):
+        """
+        Overload in subclasses.
+
+        Raises
+        ------
+        Exception
+            NotImplementedError
+        """
+        raise NotImplementedError
+
+    def sort_meta(self):
+        """Sort the info and meta dictionaries."""
+        logger.debug("sorting dictionary keys")
+        meta = self.meta
+        meta["info"] = dict(sorted(list(meta["info"].items())))
+        meta = dict(sorted(list(meta.items())))
+        return meta
+
+    def write(self, outfile=None) -> tuple:
+        """
+        Write meta information to .torrent file.
+
+        Final step in the torrent file creation process.
+        After hashing and sorting every piece of content
+        write the contents to file using the bencode encoding.
+
+        Parameters
+        ----------
+        outfile : str
+            Destination path for .torrent file. default=None
+
+        Returns
+        -------
+        outfile : str
+            Where the .torrent file was writen.
+        meta : dict
+            .torrent meta information.
+        """
+        if outfile:
+            self.outfile = outfile
+        if not self.outfile:  # pragma: nocover
+            path = os.path.join(os.getcwd(), self.name) + ".torrent"
+            self.outfile = path
+        if str(self.outfile)[-1] in "\\/":
+            self.outfile = self.outfile + (self.name + ".torrent")
+        self.meta = self.sort_meta()
+        try:
+            pyben.dump(self.meta, self.outfile)
+        except PermissionError as excp:
+            logger.error("Permission Denied: Could not write to %s",
+                         self.outfile)
+            raise PermissionError from excp
+        return self.outfile, self.meta
+
+
+class TorrentFile(MetaFile, ProgMixin):
+    """
+    Class for creating Bittorrent meta files.
+
+    Construct *Torrentfile* class instance object.
+
+    Parameters
+    ----------
+    **kwargs : dict
+        Dictionary containing torrent file options.
+    """
+
+    hasher = Hasher
+
+    def __init__(self, **kwargs):
+        """
+        Construct TorrentFile instance with given keyword args.
+
+        Parameters
+        ----------
+        **kwargs : dict
+            dictionary of keyword args passed to superclass.
+        """
+        super().__init__(**kwargs)
+        logger.debug("Assembling bittorrent v1 torrent file")
+        self.assemble()
+
+    def assemble(self):
+        """
+        Assemble components of torrent metafile.
+
+        Returns
+        -------
+        dict
+            metadata dictionary for torrent file
+        """
+        info = self.meta["info"]
+        size, filelist = utils.filelist_total(self.path)
+        if os.path.isfile(self.path):
+            info["length"] = size
+        else:
+            info["files"] = [{
+                "length":
+                os.path.getsize(path),
+                "path":
+                os.path.relpath(path, self.path).split(os.sep),
+            } for path in filelist]
+        pieces = bytearray()
+
+        feeder = Hasher(filelist, self.piece_length, self.progress)
+        for piece in feeder:
+            pieces.extend(piece)
+
+        info["pieces"] = pieces
+
+
+class TorrentFileV2(MetaFile, ProgMixin):
+    """
+    Class for creating Bittorrent meta v2 files.
+
+    Parameters
+    ----------
+    **kwargs : dict
+        Keyword arguments for torrent file options.
+    """
+
+    hasher = HasherV2
+
+    def __init__(self, **kwargs):
+        """
+        Construct `TorrentFileV2` Class instance from given parameters.
+
+        Parameters
+        ----------
+        **kwargs : dict
+            keywword arguments to pass to superclass.
+        """
+        super().__init__(**kwargs)
+        logger.debug("Assembling bittorrent v2 torrent file")
+        self.piece_layers = {}
+        self.hashes = []
+        self.total = len(utils.get_file_list(self.path))
+        self.assemble()
+
+    def assemble(self):
+        """
+        Assemble then return the meta dictionary for encoding.
+
+        Returns
+        -------
+        meta : dict
+            Metainformation about the torrent.
+        """
+        info = self.meta["info"]
+        if os.path.isfile(self.path):
+            info["file tree"] = {info["name"]: self._traverse(self.path)}
+            info["length"] = os.path.getsize(self.path)
+            self.prog_update(info["length"])
+        else:
+            info["file tree"] = self._traverse(self.path)
+
+        info["meta version"] = 2
+        self.meta["piece layers"] = self.piece_layers
+
+    def _traverse(self, path: str) -> dict:
+        """
+        Walk directory tree.
+
+        Parameters
+        ----------
+        path : str
+            Path to file or directory.
+        """
+        if os.path.isfile(path):
+            # Calculate Size and hashes for each file.
+            size = os.path.getsize(path)
+
+            if size == 0:
+                return {"": {"length": size}}
+
+            logger.debug("Hashing %s", str(path))
+            fhash = HasherV2(path, self.piece_length, self.progress)
+
+            if size > self.piece_length:
+                self.piece_layers[fhash.root] = fhash.piece_layer
+            return {"": {"length": size, "pieces root": fhash.root}}
+
+        file_tree = {}
+        if os.path.isdir(path):
+            for name in sorted(os.listdir(path)):
+                file_tree[name] = self._traverse(os.path.join(path, name))
+        return file_tree
+
+
+class TorrentFileHybrid(MetaFile, ProgMixin):
+    """
+    Construct the Hybrid torrent meta file with provided parameters.
+
+    Parameters
+    ----------
+    **kwargs : dict
+        Keyword arguments for torrent options.
+    """
+
+    hasher = HasherHybrid
+
+    def __init__(self, **kwargs):
+        """
+        Create Bittorrent v1 v2 hybrid metafiles.
+        """
+        super().__init__(**kwargs)
+        logger.debug("Assembling bittorrent Hybrid file")
+        self.name = os.path.basename(self.path)
+        self.hashes = []
+        self.piece_layers = {}
+        self.pieces = []
+        self.files = []
+        self.total = len(utils.get_file_list(self.path))
+        self.assemble()
+
+    def assemble(self):
+        """
+        Assemble the parts of the torrentfile into meta dictionary.
+        """
+        info = self.meta["info"]
+        info["meta version"] = 2
+
+        if os.path.isfile(self.path):
+            info["file tree"] = {self.name: self._traverse(self.path)}
+            info["length"] = os.path.getsize(self.path)
+
+        else:
+            info["file tree"] = self._traverse(self.path)
+            info["files"] = self.files
+
+        info["pieces"] = b"".join(self.pieces)
+        self.meta["piece layers"] = self.piece_layers
+        return info
+
+    def _traverse(self, path: str) -> dict:
+        """
+        Build meta dictionary while walking directory.
+
+        Parameters
+        ----------
+        path : str
+            Path to target file.
+        """
+        if os.path.isfile(path):
+            file_size = os.path.getsize(path)
+
+            self.files.append({
+                "length":
+                file_size,
+                "path":
+                os.path.relpath(path, self.path).split(os.sep),
+            })
+
+            if file_size == 0:
+                return {"": {"length": file_size}}
+
+            logger.debug("Hashing %s", str(path))
+            file_hash = HasherHybrid(path, self.piece_length, self.progress)
+            self.prog_update(file_size)
+
+            if file_size > self.piece_length:
+                self.piece_layers[file_hash.root] = file_hash.piece_layer
+
+            self.hashes.append(file_hash)
+            self.pieces.extend(file_hash.pieces)
+
+            if file_hash.padding_file:
+                self.files.append(file_hash.padding_file)
+
+            return {"": {"length": file_size, "pieces root": file_hash.root}}
+
+        tree = {}
+        if os.path.isdir(path):
+            for name in sorted(os.listdir(path)):
+                tree[name] = self._traverse(os.path.join(path, name))
+        return tree
+
+
+class TorrentAssembler(MetaFile):
+    """
+    Assembler class for Bittorrent version 2 and hybrid meta files.
+
+    This differs from the TorrentFileV2 and TorrentFileHybrid, because
+    it can be used as an iterator and works for both versions.
+
+    Parameters
+    ----------
+    **kwargs : dict
+        Keyword arguments for torrent options.
+    """
+
+    hasher = FileHasher
+
+    def __init__(self, **kwargs):
+        """
+        Create Bittorrent v1 v2 hybrid metafiles.
+        """
+        super().__init__(**kwargs)
+        logger.debug("Assembling bittorrent Hybrid file")
+        self.name = os.path.basename(self.path)
+        self.hashes = []
+        self.piece_layers = {}
+        self.pieces = bytearray()
+        self.files = []
+        self.hybrid = self.meta_version == "3"
+        self.total = len(utils.get_file_list(self.path))
+        self.assemble()
+
+    def assemble(self):
+        """
+        Assemble the parts of the torrentfile into meta dictionary.
+        """
+        info = self.meta["info"]
+        info["meta version"] = 2
+
+        if os.path.isfile(self.path):
+            info["file tree"] = {self.name: self._traverse(self.path)}
+            info["length"] = os.path.getsize(self.path)
+
+        else:
+            info["file tree"] = self._traverse(self.path)
+            if self.hybrid:
+                info["files"] = self.files
+
+        if self.hybrid:
+            info["pieces"] = self.pieces
+        self.meta["piece layers"] = self.piece_layers
+        return info
+
+    def _traverse(self, path: str) -> dict:
+        """
+        Build meta dictionary while walking directory.
+
+        Parameters
+        ----------
+        path : str
+            Path to target file.
+        """
+        if os.path.isfile(path):
+            file_size = os.path.getsize(path)
+            if self.hybrid:
+                self.files.append({
+                    "length":
+                    file_size,
+                    "path":
+                    os.path.relpath(path, self.path).split(os.sep),
+                })
+
+            if file_size == 0:
+                return {"": {"length": file_size}}
+
+            logger.debug("Hashing %s", str(path))
+            hasher = FileHasher(path,
+                                self.piece_length,
+                                progress=True,
+                                hybrid=self.hybrid)
+            layers = bytearray()
+            for result in hasher:
+                if self.hybrid:
+                    layer_hash, piece = result
+                    self.pieces.extend(piece)
+                else:
+                    layer_hash = result
+                layers.extend(layer_hash)
+            if file_size > self.piece_length:
+                self.piece_layers[hasher.root] = layers
+            if self.hybrid and hasher.padding_file:
+                self.files.append(hasher.padding_file)
+
+            return {"": {"length": file_size, "pieces root": hasher.root}}
+
+        tree = {}
+        if os.path.isdir(path):
+            for name in sorted(os.listdir(path)):
+                tree[name] = self._traverse(os.path.join(path, name))
+        return tree
```

### Comparing `torrentfile-0.8.8/torrentfile/version.py` & `torrentfile-0.9.0/torrentfile/version.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-#! /usr/bin/python3
-# -*- coding: utf-8 -*-
-
-##############################################################################
-#    Copyright (C) 2021-current alexpdev
-#
-#    Licensed under the Apache License, Version 2.0 (the "License");
-#    you may not use this file except in compliance with the License.
-#    You may obtain a copy of the License at
-#
-#        http://www.apache.org/licenses/LICENSE-2.0
-#
-#    Unless required by applicable law or agreed to in writing, software
-#    distributed under the License is distributed on an "AS IS" BASIS,
-#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#    See the License for the specific language governing permissions and
-#    limitations under the License.
-##############################################################################
-"""
-Holds the release version number.
-"""
-
-__version__ = "0.8.8"
+#! /usr/bin/python3
+# -*- coding: utf-8 -*-
+
+##############################################################################
+#    Copyright (C) 2021-current alexpdev
+#
+#    Licensed under the Apache License, Version 2.0 (the "License");
+#    you may not use this file except in compliance with the License.
+#    You may obtain a copy of the License at
+#
+#        http://www.apache.org/licenses/LICENSE-2.0
+#
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS,
+#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#    See the License for the specific language governing permissions and
+#    limitations under the License.
+##############################################################################
+"""
+Holds the release version number.
+"""
+
+__version__ = "0.9.0"
```

### Comparing `torrentfile-0.8.8/torrentfile.egg-info/SOURCES.txt` & `torrentfile-0.9.0/torrentfile.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 requirements.txt
 setup.py
 tox.ini
 assets/Torrentfile.gif
 assets/torrentfile-icon.ico
 assets/torrentfile-icon.png
 assets/torrentfile.png
+assets/torrentfile_square.png
 c/hasher.c
 c/hasher.h
 c/sha.c
 c/sha.h
 tests/test_cli.py
 tests/test_commands.py
 tests/test_edit.py
```

