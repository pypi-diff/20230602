# Comparing `tmp/git_timemachine-0.2.2.tar.gz` & `tmp/git_timemachine-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_timemachine-0.2.2.tar", max compression
+gzip compressed data, was "git_timemachine-1.3.0.tar", max compression
```

## Comparing `git_timemachine-0.2.2.tar` & `git_timemachine-1.3.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0      280 2023-04-11 18:50:29.595916 git_timemachine-0.2.2/README.md
--rw-r--r--   0        0        0      990 2023-04-11 18:50:29.596640 git_timemachine-0.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-11 18:50:29.596798 git_timemachine-0.2.2/src/git_timemachine/__init__.py
--rw-r--r--   0        0        0      771 2023-04-11 18:50:29.596923 git_timemachine-0.2.2/src/git_timemachine/__main__.py
--rw-r--r--   0        0        0      231 2023-04-11 18:50:29.597082 git_timemachine-0.2.2/src/git_timemachine/commands/__init__.py
--rw-r--r--   0        0        0     3847 2023-04-11 18:50:29.597202 git_timemachine-0.2.2/src/git_timemachine/commands/commit.py
--rw-r--r--   0        0        0     1176 2023-04-11 18:50:29.597308 git_timemachine-0.2.2/src/git_timemachine/commands/log.py
--rw-r--r--   0        0        0     2870 2023-04-11 18:50:29.597417 git_timemachine-0.2.2/src/git_timemachine/commands/migrate.py
--rw-r--r--   0        0        0      669 2023-04-11 18:50:29.597514 git_timemachine-0.2.2/src/git_timemachine/commands/switch_date.py
--rw-r--r--   0        0        0     1419 2023-04-11 18:50:29.597607 git_timemachine-0.2.2/src/git_timemachine/state.py
--rw-r--r--   0        0        0      373 2023-04-11 18:50:29.597690 git_timemachine-0.2.2/src/git_timemachine/utils.py
--rw-r--r--   0        0        0     1036 1970-01-01 00:00:00.000000 git_timemachine-0.2.2/PKG-INFO
+-rwxr-xr-x   0        0        0    35147 2023-05-02 06:28:21.000000 git_timemachine-1.3.0/LICENSE
+-rwxr-xr-x   0        0        0      408 2023-06-02 10:58:19.377074 git_timemachine-1.3.0/README.md
+-rw-r--r--   0        0        0     1024 2023-06-02 17:06:24.277346 git_timemachine-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-02 02:05:43.427329 git_timemachine-1.3.0/src/git_timemachine/__init__.py
+-rw-r--r--   0        0        0      747 2023-06-02 10:46:36.247096 git_timemachine-1.3.0/src/git_timemachine/__main__.py
+-rw-r--r--   0        0        0      231 2023-06-02 16:41:44.873985 git_timemachine-1.3.0/src/git_timemachine/commands/__init__.py
+-rw-r--r--   0        0        0     3273 2023-06-02 17:05:53.787345 git_timemachine-1.3.0/src/git_timemachine/commands/commit.py
+-rw-r--r--   0        0        0     1176 2023-06-02 02:23:15.307335 git_timemachine-1.3.0/src/git_timemachine/commands/log.py
+-rwxr-xr-x   0        0        0     2832 2023-06-02 16:43:00.203987 git_timemachine-1.3.0/src/git_timemachine/commands/migrate.py
+-rw-r--r--   0        0        0      641 2023-06-02 16:31:24.703974 git_timemachine-1.3.0/src/git_timemachine/commands/switch_date.py
+-rw-r--r--   0        0        0     1125 2023-06-02 10:31:13.707125 git_timemachine-1.3.0/src/git_timemachine/state.py
+-rw-r--r--   0        0        0      951 2023-06-02 17:02:12.764008 git_timemachine-1.3.0/src/git_timemachine/utils.py
+-rw-r--r--   0        0        0     1209 1970-01-01 00:00:00.000000 git_timemachine-1.3.0/PKG-INFO
```

### Comparing `git_timemachine-0.2.2/pyproject.toml` & `git_timemachine-1.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 [tool.poetry]
 name = "git-timemachine"
-version = "0.2.2"
-description = "A nested command-line utility that helps you record commits on Git repositories at any time node."
+version = "1.3.0"
+description = "A command-line tool that helps you record commits on Git repositories at any time node."
 authors = ["HE Yaowen <he.yaowen@hotmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
+homepage = "https://github.com/he-yaowen/git-timemachine"
 packages = [{include = "git_timemachine", from = "src"}]
 
 [tool.poetry.dependencies]
-python = ">=3.7.2,<3.12"
+python = "^3.8,<3.12"
 click = "^8.1.3"
-tabulate = "^0.8.10"
-pygit2 = "^1.9.1"
+tabulate = "^0.9.0"
+pygit2 = "^1.12.1"
 
 [tool.poetry.group.dev.dependencies]
-pre-commit = "^2.20.0"
-pyinstaller = "^5.3"
-pylint = "^2.14.5"
-pytest = "^7.1.2"
-pytest-cov = "^3.0.0"
+pre-commit = "^3.3.2"
+pylint = "^2.17.4"
+pytest = "^7.3.1"
+pytest-cov = "^4.1.0"
+pyinstaller = "^5.11.0"
 
 [tool.poetry.scripts]
 git-timemachine = "git_timemachine.__main__:cli"
 
 [tool.poe.tasks]
-init = {shell ="poetry install && poetry run pre-commit install"}
-test = "poetry run pytest --cov=src --cov-report=term-missing"
-lint = "poetry run pylint src"
-dist = "poetry run pyinstaller git-timemachine.spec"
 gtm = "poetry run git-timemachine"
+lint = "poetry run pylint src"
+test = "poetry run pytest --cov=src --cov-report=term-missing"
+postinstall = "poetry run pre-commit install"
+pyinstaller = "poetry run pyinstaller git-timemachine.spec"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `git_timemachine-0.2.2/src/git_timemachine/__main__.py` & `git_timemachine-1.3.0/src/git_timemachine/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+from os import PathLike
 from pathlib import Path
-from typing import Union
 
 import click
+
 from git_timemachine.commands import command_group
 from git_timemachine.state import StateFile
 
 
 @click.group(commands=command_group)
 @click.version_option(message='%(version)s')
 @click.option('--state-file', help='Path of state file.', type=click.Path(dir_okay=False, exists=False), is_eager=True, default=Path.home().joinpath('.git-timemachine.state'))
 @click.pass_context
-def cli(ctx: click.Context, state_file: Union[Path, str]):
-    """A nested command-line utility that helps you record commits on Git repositories at any time node."""
+def cli(ctx: click.Context, state_file: PathLike):
+    """A command-line tool that helps you record commits on Git repositories at any time node."""
 
     ctx.ensure_object(dict)
-    ctx.obj['states'] = StateFile(Path(state_file))
+    ctx.obj['states'] = StateFile(state_file)
 
 
 if __name__ == '__main__':
     # pylint: disable=no-value-for-parameter
     cli()
```

### Comparing `git_timemachine-0.2.2/src/git_timemachine/commands/commit.py` & `git_timemachine-1.3.0/src/git_timemachine/commands/commit.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,112 +2,92 @@
 import random
 from pathlib import Path
 from datetime import datetime, timedelta
 
 import click
 from tabulate import tabulate
 from pygit2 import discover_repository, Repository, Signature, GitError
-from pygit2 import GIT_STATUS_INDEX_NEW, GIT_STATUS_INDEX_RENAMED, GIT_STATUS_INDEX_MODIFIED
-from pygit2 import GIT_STATUS_INDEX_DELETED, GIT_STATUS_INDEX_TYPECHANGE, GIT_STATUS_WT_NEW
-from git_timemachine.state import StateFile
-from git_timemachine.utils import print_error
-
-
-def status_text(status: int) -> str:
-    texts = {
-        GIT_STATUS_INDEX_NEW: 'new',
-        GIT_STATUS_INDEX_MODIFIED: 'modified',
-        GIT_STATUS_INDEX_DELETED: 'deleted',
-        GIT_STATUS_INDEX_RENAMED: 'renamed',
-        GIT_STATUS_INDEX_TYPECHANGE: 'type changed'
-    }
-
-    result = []
-    for i, text in texts.items():
-        if status & i == i:
-            result.append(text)
+from pygit2 import GIT_STATUS_WT_NEW
 
-    return ', '.join(result)
+from git_timemachine.state import StateFile
+from git_timemachine.utils import print_error, index_status_texts
 
 
 @click.command('commit')
 @click.argument('repo_dir', type=click.Path(exists=True, file_okay=False), default=Path.cwd())
 @click.option('-m', '--message', help='Message describing the changes.', required=True)
 @click.option('--rand-min', help='Minimum random seconds of time increase.', type=int, default=600)
 @click.option('--rand-max', help='Maximum random seconds of time increase.', type=int, default=3600)
 @click.option('--default-head', help='Reference name of default HEAD', type=str, default='main')
 @click.pass_context
-def commit_command(ctx: click.Context, repo_dir: str, **options: dict):
-    """Record a commit on repository based on time states."""
+def commit_command(ctx: click.Context, repo_dir: str, message: str, rand_min: int, rand_max: int, default_head: str):
+    """Record a commit on repository based on states."""
 
     states: StateFile = ctx.obj['states']
-    last_commit = states.get('last-commit')
 
+    last_commit = states.get('last-commit')
     if last_commit is None:
         print_error('state "last-commit" not defined, current time used.')
         states.set('last-commit', datetime.now())
-        states.save()
         ctx.exit()
 
     repo = Repository(discover_repository(repo_dir))
     pre_commit = Path(repo.path, 'hooks', 'pre-commit')
     if pre_commit.exists():
         assert os.system(pre_commit) == 0
 
     repo_status = repo.status(untracked_files='no')
-
     if repo_status == {} or len([value for value in repo_status.values() if value < GIT_STATUS_WT_NEW]) < 1:
-        raise GitError(f'Nothing to commit on "{repo_dir}".')
+        print_error(f'nothing to commit on "{repo_dir}".')
+        ctx.exit(1)
 
     random.seed()
-    dt = last_commit + timedelta(seconds=random.randint(options['rand_min'], options['rand_max']))
+    dt = last_commit + timedelta(seconds=random.randint(rand_min, rand_max))
 
     if not repo.head_is_unborn and dt.timestamp() < next(repo.walk(repo.head.target)).commit_time:
         raise GitError('HEAD time is later than commit time.')
 
     author = Signature(
         name=repo.default_signature.name,
         email=repo.default_signature.email,
         time=int(dt.replace(microsecond=0).timestamp()),
         encoding='utf-8',
         offset=int(dt.tzinfo.utcoffset(dt).seconds / 60)
-
     )
 
     committer = author
 
     parent = []
 
     if repo.head_is_unborn:
-        ref_name = f'refs/heads/{options["default_head"]}'
+        ref_name = f'refs/heads/{default_head}'
     else:
         parent.append(repo.head.target)
         ref_name = repo.head.name
 
     tree = repo.index.write_tree()
 
     if tree is None:
-        print_error('Failed to write index tree.')
+        print_error('failed to write index tree.')
         ctx.exit(1)
 
-    oid = repo.create_commit(ref_name, author, committer, options['message'], tree, parent)
+    oid = repo.create_commit(ref_name, author, committer, message, tree, parent)
 
     if oid is None:
-        print_error('Failed to create commit.')
+        print_error('failed to create commit.')
         ctx.exit(1)
 
     table = []
     for file in repo_status:
         if repo_status[file] >= GIT_STATUS_WT_NEW:
             continue
 
-        table.append([status_text(repo_status[file]), file])
+        table.append([', '.join(index_status_texts(repo_status[file])), file])
 
     print(f'commit: {oid.hex}')
     print(f'committer: {committer.name} <{committer.email}>')
     print(f'datetime: {datetime.fromtimestamp(committer.time).astimezone().isoformat()}')
-    print(f'message: {options["message"]}')
+    print(f'message: {message}')
     print()
     print(tabulate(table, headers=['status', 'file']))
 
     states.set('last-commit', dt)
-    states.save()
```

### Comparing `git_timemachine-0.2.2/src/git_timemachine/commands/log.py` & `git_timemachine-1.3.0/src/git_timemachine/commands/log.py`

 * *Files identical despite different names*

### Comparing `git_timemachine-0.2.2/src/git_timemachine/commands/migrate.py` & `git_timemachine-1.3.0/src/git_timemachine/commands/migrate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,40 @@
-from pathlib import Path
+import os
+from os import PathLike
 from datetime import datetime, timedelta
 
 import click
 from pygit2 import discover_repository, init_repository, Repository, Signature
 from pygit2 import GIT_SORT_REVERSE, GIT_DIFF_REVERSE, GIT_DIFF_SHOW_BINARY, GIT_APPLY_LOCATION_BOTH
 from git_timemachine.utils import print_error
 
 
 @click.command('migrate')
-@click.argument('src_dir', type=click.Path(exists=True, file_okay=False), default=Path.cwd())
+@click.argument('src_dir', type=click.Path(exists=True, file_okay=False), default=os.getcwd())
 @click.argument('dest_dir', type=click.Path(exists=False, file_okay=False), required=False, default=None)
-@click.option('-o', '--offset', required=False, help='Time offset for each commit.')
+@click.option('-o', '--offset', help='Time offset for each commit.', type=str, required=False)
 @click.option('--default-head', help='Reference name of default HEAD', type=str, default='main')
 @click.pass_context
-def migrate_command(ctx: click.Context, src_dir: Path, dest_dir: Path, **options: dict):
+def migrate_command(ctx: click.Context, src_dir: PathLike, dest_dir: PathLike, offset: str, default_head: str):
     """Migrate commit logs from a repository to another."""
 
-    src_dir = Path(src_dir)
-
     if dest_dir is None:
-        dest_dir = src_dir.parent.joinpath(src_dir.name + '.migrated')
+        dest_dir = f'{src_dir}.migrated'
 
-    if dest_dir.exists():
+    if os.path.exists(dest_dir):
         raise FileExistsError(f'Destination directory {dest_dir} already exists.')
 
-    dest_dir.mkdir(0o755)
+    os.mkdir(dest_dir, 0o755)
 
-    src_repo = Repository(discover_repository(src_dir))
-    dest_repo = init_repository(dest_dir, initial_head='main')
+    src_repo = Repository(discover_repository(str(src_dir)))
+    dest_repo = init_repository(dest_dir, initial_head=default_head)
 
     parent = []
 
-    ref_name = f'refs/heads/{options["default_head"]}'
+    ref_name = f'refs/heads/{default_head}'
 
     for commit in src_repo.walk(src_repo.head.target, GIT_SORT_REVERSE):
         if len(commit.parents) > 0:
             diff = commit.tree.diff_to_tree(commit.parents[0].tree, flags=GIT_DIFF_REVERSE | GIT_DIFF_SHOW_BINARY)
         else:
             diff = commit.tree.diff_to_tree(flags=GIT_DIFF_REVERSE | GIT_DIFF_SHOW_BINARY)
 
@@ -45,22 +44,22 @@
         tree = dest_repo.index.write_tree()
 
         if tree is None:
             print_error('Failed to write index tree.')
             ctx.exit(1)
 
         seconds = 0
-        if options['offset'] is not None:
-            unit = options['offset'][-1]
+        if offset is not None:
+            unit = offset[-1]
             multi = {'s': 1, 'm': 60, 'h': 60 * 60, 'd': 60 * 60 * 24}
 
             if unit not in multi:
                 raise ValueError(f'Unknown offset unit: {unit}')
 
-            seconds = int(options['offset'][:-1]) * multi[unit]
+            seconds = int(offset[:-1]) * multi[unit]
 
         dt = datetime.fromtimestamp(commit.author.time) + timedelta(seconds=seconds)
 
         author = Signature(
             name=commit.author.name,
             email=commit.author.email,
             time=int(dt.timestamp()),
```

### Comparing `git_timemachine-0.2.2/src/git_timemachine/state.py` & `git_timemachine-1.3.0/src/git_timemachine/state.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,57 +1,40 @@
 import json
-from pathlib import Path
+from os import PathLike, path
 from typing import Any
 from datetime import datetime
 
 
-def json_encode_hook(obj: Any):
-    if isinstance(obj, datetime):
-        return {
-            'type': 'datetime',
-            'value': obj.replace(microsecond=0).astimezone().isoformat()
-        }
-
-    return obj
-
-
-def json_decode_hook(obj: dict):
-    if 'type' not in obj:
-        return obj
-
-    if obj['type'] == 'datetime':
-        return datetime.fromisoformat(obj['value'])
-
-    raise TypeError(f'Unknown state type {obj["type"]}.')
-
-
 class StateFile:
-    _data: dict = {}
-    filename: Path
+    raw: dict = {}
+    filename: PathLike
 
-    def __init__(self, filename: Path):
+    def __init__(self, filename: PathLike):
         self.filename = filename
 
-        if not filename.exists():
-            self.save()
-        else:
-            self.load()
-
-    def load(self):
-        with self.filename.open('r', encoding='utf-8') as fp:
-            self._data = json.load(fp, object_hook=json_decode_hook)
-
-    def save(self):
-        with self.filename.open('w', encoding='utf-8') as fp:
-            json.dump(self._data, fp, default=json_encode_hook, ensure_ascii=False, indent=4)
-
-    def get(self, key: str, default=None, raise_error=False) -> Any:
-        if key not in self._data:
-            if raise_error:
-                raise KeyError(f'State "{key}" not defined.')
+        if path.exists(filename):
+            with open(filename, 'r', encoding='utf-8') as fp:
+                self.raw = json.load(fp)
 
+    def get(self, key: str, default=None) -> Any:
+        if key not in self.raw:
             return default
 
-        return self._data[key]
+        value = self.raw[key]
+
+        if isinstance(value, dict) and 'type' in value:
+            if value['type'] == 'datetime':
+                return datetime.fromisoformat(value['value'])
+
+        return self.raw[key]
 
     def set(self, key: str, value: Any):
-        self._data[key] = value
+        if isinstance(value, datetime):
+            self.raw[key] = {
+                'type': 'datetime',
+                'value': value.replace(microsecond=0).astimezone().isoformat()
+            }
+        else:
+            self.raw[key] = value
+
+        with open(self.filename, 'w', encoding='utf-8') as fp:
+            json.dump(self.raw, fp, ensure_ascii=False, indent=4)
```

