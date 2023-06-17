# Comparing `tmp/git_timemachine-1.3.1.tar.gz` & `tmp/git_timemachine-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_timemachine-1.3.1.tar", max compression
+gzip compressed data, was "git_timemachine-2.0.0.tar", max compression
```

## Comparing `git_timemachine-1.3.1.tar` & `git_timemachine-2.0.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rwxr-xr-x   0        0        0    35147 2023-06-15 17:39:29.797642 git_timemachine-1.3.1/LICENSE
--rwxr-xr-x   0        0        0      408 2023-06-15 17:39:29.798637 git_timemachine-1.3.1/README.md
--rwxr-xr-x   0        0        0     1024 2023-06-15 17:39:29.800604 git_timemachine-1.3.1/pyproject.toml
--rwxr-xr-x   0        0        0       87 2023-06-15 17:39:29.801629 git_timemachine-1.3.1/src/git_timemachine/__init__.py
--rwxr-xr-x   0        0        0     1033 2023-06-15 17:39:29.801629 git_timemachine-1.3.1/src/git_timemachine/__main__.py
--rwxr-xr-x   0        0        0      231 2023-06-15 17:39:29.802626 git_timemachine-1.3.1/src/git_timemachine/commands/__init__.py
--rwxr-xr-x   0        0        0     3273 2023-06-15 17:39:29.803627 git_timemachine-1.3.1/src/git_timemachine/commands/commit.py
--rwxr-xr-x   0        0        0     1176 2023-06-15 17:39:29.803627 git_timemachine-1.3.1/src/git_timemachine/commands/log.py
--rwxr-xr-x   0        0        0     2832 2023-06-15 17:39:29.804621 git_timemachine-1.3.1/src/git_timemachine/commands/migrate.py
--rwxr-xr-x   0        0        0      641 2023-06-15 17:39:29.804621 git_timemachine-1.3.1/src/git_timemachine/commands/switch_date.py
--rwxr-xr-x   0        0        0     1125 2023-06-15 17:39:29.805591 git_timemachine-1.3.1/src/git_timemachine/state.py
--rwxr-xr-x   0        0        0      951 2023-06-15 17:39:29.805591 git_timemachine-1.3.1/src/git_timemachine/utils.py
--rw-r--r--   0        0        0     1209 1970-01-01 00:00:00.000000 git_timemachine-1.3.1/PKG-INFO
+-rwxr-xr-x   0        0        0      280 2023-06-16 16:24:50.513758 git_timemachine-2.0.0/README.md
+-rwxr-xr-x   0        0        0     1042 2023-06-17 09:42:08.737421 git_timemachine-2.0.0/pyproject.toml
+-rwxr-xr-x   0        0        0       87 2023-06-16 16:25:38.438695 git_timemachine-2.0.0/src/git_timemachine/__init__.py
+-rwxr-xr-x   0        0        0     1723 2023-06-17 09:40:33.004403 git_timemachine-2.0.0/src/git_timemachine/__main__.py
+-rwxr-xr-x   0        0        0      336 2023-06-17 09:12:10.537199 git_timemachine-2.0.0/src/git_timemachine/command/__init__.py
+-rwxr-xr-x   0        0        0     3897 2023-06-17 08:51:15.374491 git_timemachine-2.0.0/src/git_timemachine/command/commit.py
+-rwxr-xr-x   0        0        0      894 2023-06-17 08:13:19.376189 git_timemachine-2.0.0/src/git_timemachine/command/config.py
+-rwxr-xr-x   0        0        0     1215 2023-06-16 17:46:11.169634 git_timemachine-2.0.0/src/git_timemachine/command/log.py
+-rwxr-xr-x   0        0        0     2593 2023-06-17 06:31:17.237148 git_timemachine-2.0.0/src/git_timemachine/command/migrate.py
+-rwxr-xr-x   0        0        0      682 2023-06-17 09:18:16.347728 git_timemachine-2.0.0/src/git_timemachine/command/session.py
+-rwxr-xr-x   0        0        0      661 2023-06-17 06:06:10.094026 git_timemachine-2.0.0/src/git_timemachine/command/switch_date.py
+-rwxr-xr-x   0        0        0     1026 2023-06-17 06:27:50.485505 git_timemachine-2.0.0/src/git_timemachine/git.py
+-rwxr-xr-x   0        0        0      423 2023-06-17 09:39:44.699950 git_timemachine-2.0.0/src/git_timemachine/session.py
+-rwxr-xr-x   0        0        0     1209 2023-06-17 08:19:16.406434 git_timemachine-2.0.0/src/git_timemachine/utils.py
+-rw-r--r--   0        0        0     1081 1970-01-01 00:00:00.000000 git_timemachine-2.0.0/PKG-INFO
```

### Comparing `git_timemachine-1.3.1/pyproject.toml` & `git_timemachine-2.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 [tool.poetry]
 name = "git-timemachine"
-version = "1.3.1"
+version = "2.0.0"
 description = "A command-line tool that helps you record commits on Git repositories at any time node."
 authors = ["HE Yaowen <he.yaowen@hotmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 homepage = "https://github.com/he-yaowen/git-timemachine"
 packages = [{include = "git_timemachine", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.12"
 click = "^8.1.3"
 tabulate = "^0.9.0"
 pygit2 = "^1.12.1"
 
 [tool.poetry.group.dev.dependencies]
-pre-commit = "^3.3.2"
+chance = "^0.110"
+pre-commit = "^3.3.3"
+pyinstaller = "^5.12.0"
 pylint = "^2.17.4"
-pytest = "^7.3.1"
+pytest = "^7.3.2"
 pytest-cov = "^4.1.0"
-pyinstaller = "^5.11.0"
 
 [tool.poetry.scripts]
 git-timemachine = "git_timemachine.__main__:cli"
 
 [tool.poe.tasks]
 gtm = "poetry run git-timemachine"
 lint = "poetry run pylint src"
```

### Comparing `git_timemachine-1.3.1/src/git_timemachine/commands/commit.py` & `git_timemachine-2.0.0/src/git_timemachine/command/commit.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,93 +1,97 @@
-import os
 import random
 from pathlib import Path
 from datetime import datetime, timedelta
 
 import click
 from tabulate import tabulate
-from pygit2 import discover_repository, Repository, Signature, GitError
-from pygit2 import GIT_STATUS_WT_NEW
+from pygit2 import discover_repository, Repository, Signature, GitError, GIT_STATUS_WT_NEW
 
-from git_timemachine.state import StateFile
-from git_timemachine.utils import print_error, index_status_texts
+from git_timemachine.utils import PropertyFile
+from git_timemachine.git import status_to_texts, create_repo_commit
 
 
 @click.command('commit')
-@click.argument('repo_dir', type=click.Path(exists=True, file_okay=False), default=Path.cwd())
+@click.option('-t', '--time', help='Time node commit with', type=str, required=False, default=None)
 @click.option('-m', '--message', help='Message describing the changes.', required=True)
-@click.option('--rand-min', help='Minimum random seconds of time increase.', type=int, default=600)
-@click.option('--rand-max', help='Maximum random seconds of time increase.', type=int, default=3600)
+@click.option('-C', 'repo_dir', help='Path of repository directory.', type=click.Path(exists=True, file_okay=False), default=Path.cwd())
 @click.option('--default-head', help='Reference name of default HEAD', type=str, default='main')
+@click.option('--rand-min', help='Random minimum seconds.', type=int, default=600)
+@click.option('--rand-max', help='Random maximum seconds.', type=int, default=3600)
+@click.option('--no-save', help='Not save the time node to states.', type=bool, is_flag=True, default=False)
+@click.option('--max-per-day', help='Maximum commits per day.', type=int, default=None)
 @click.pass_context
-def commit_command(ctx: click.Context, repo_dir: str, message: str, rand_min: int, rand_max: int, default_head: str):
-    """Record a commit on repository based on states."""
+# pylint: disable=too-many-arguments,too-many-locals
+def commit_command(ctx: click.Context, time: str, message: str, repo_dir: str, default_head: str, rand_min: int, rand_max: int, no_save: bool, max_per_day: int):
+    """Record a commit on repository at specified time node."""
 
-    states: StateFile = ctx.obj['states']
-
-    last_commit = states.get('last-commit')
-    if last_commit is None:
-        print_error('state "last-commit" not defined, current time used.')
-        states.set('last-commit', datetime.now())
-        ctx.exit()
+    states: PropertyFile = ctx.obj['states']
+    config: PropertyFile = ctx.obj['config']
 
     repo = Repository(discover_repository(repo_dir))
-    pre_commit = Path(repo.path, 'hooks', 'pre-commit')
-    if pre_commit.exists():
-        assert os.system(pre_commit) == 0
+
+    if time is None:
+        commit_time = states.get('commit-time')
+    else:
+        commit_time = datetime.fromisoformat(time)
+
+    if not repo.is_empty and commit_time.timestamp() < next(repo.walk(repo.head.target)).commit_time:
+        raise GitError('HEAD time is later than commit time.')
 
     repo_status = repo.status(untracked_files='no')
     if repo_status == {} or len([value for value in repo_status.values() if value < GIT_STATUS_WT_NEW]) < 1:
-        print_error(f'nothing to commit on "{repo_dir}".')
-        ctx.exit(1)
+        raise GitError(f'Nothing to commit on "{repo_dir}".')
 
     random.seed()
-    dt = last_commit + timedelta(seconds=random.randint(rand_min, rand_max))
+    rand_time = commit_time + timedelta(seconds=random.randint(rand_min, rand_max))
 
-    if not repo.head_is_unborn and dt.timestamp() < next(repo.walk(repo.head.target)).commit_time:
-        raise GitError('HEAD time is later than commit time.')
+    if max_per_day is None:
+        max_per_day = config.get('maxCommitsPerDay', 0)
 
-    author = Signature(
+    check_max_commits(repo, rand_time, max_per_day)
+
+    signature = Signature(
         name=repo.default_signature.name,
         email=repo.default_signature.email,
-        time=int(dt.replace(microsecond=0).timestamp()),
+        time=int(rand_time.replace(microsecond=0).timestamp()),
         encoding='utf-8',
-        offset=int(dt.tzinfo.utcoffset(dt).seconds / 60)
+        offset=int(rand_time.tzinfo.utcoffset(rand_time).seconds / 60)
     )
 
-    committer = author
-
-    parent = []
+    parents = []
 
-    if repo.head_is_unborn:
+    if repo.is_empty:
         ref_name = f'refs/heads/{default_head}'
     else:
-        parent.append(repo.head.target)
+        parents.append(repo.head.target)
         ref_name = repo.head.name
 
-    tree = repo.index.write_tree()
-
-    if tree is None:
-        print_error('failed to write index tree.')
-        ctx.exit(1)
-
-    oid = repo.create_commit(ref_name, author, committer, message, tree, parent)
-
-    if oid is None:
-        print_error('failed to create commit.')
-        ctx.exit(1)
+    oid = create_repo_commit(repo, ref_name, signature, message, parents)
 
     table = []
     for file in repo_status:
         if repo_status[file] >= GIT_STATUS_WT_NEW:
             continue
 
-        table.append([', '.join(index_status_texts(repo_status[file])), file])
+        table.append([', '.join(status_to_texts(repo_status[file])), file, oct(repo.index[file].mode & 0o100777)[2:]])
 
     print(f'commit: {oid.hex}')
-    print(f'committer: {committer.name} <{committer.email}>')
-    print(f'datetime: {datetime.fromtimestamp(committer.time).astimezone().isoformat()}')
+    print(f'committer: {signature.name} <{signature.email}>')
+    print(f'datetime: {datetime.fromtimestamp(signature.time).astimezone().isoformat()}')
     print(f'message: {message}')
     print()
-    print(tabulate(table, headers=['status', 'file']))
+    print(tabulate(table, headers=['status', 'file', 'mode']))
+
+    if not no_save:
+        states.set('commit-time', rand_time)
+
+
+def check_max_commits(repo: Repository, time: datetime, max_num: int):
+    if repo.is_empty or max_num == 0:
+        return
+
+    date_str = time.strftime('%Y-%m-%d')
+
+    commits = [commit for commit in repo.walk(repo.head.target) if datetime.fromtimestamp(commit.commit_time).strftime('%Y-%m-%d') == date_str]
 
-    states.set('last-commit', dt)
+    if len(commits) >= max_num:
+        raise RuntimeError(f'Exceeded the daily commit limit: {max_num}.')
```

### Comparing `git_timemachine-1.3.1/src/git_timemachine/commands/log.py` & `git_timemachine-2.0.0/src/git_timemachine/command/log.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from pathlib import Path
 
 import click
 from pygit2 import discover_repository, Repository
 
 
 @click.command('log')
-@click.argument('repo_dir', type=click.Path(exists=True, file_okay=False), default=Path.cwd())
+@click.option('-C', 'repo_dir', help='Path of repository directory.', type=click.Path(exists=True, file_okay=False), default=Path.cwd())
 def log_command(repo_dir: Path):
-    """Show commit logs of a repository in formatted data."""
+    """Show commit logs of a repository in JSON format."""
 
     repo = Repository(discover_repository(str(repo_dir)))
 
     click.echo(json.dumps(
         [{
             'id': commit.id.hex,
             'author': {
```

### Comparing `git_timemachine-1.3.1/src/git_timemachine/commands/migrate.py` & `git_timemachine-2.0.0/src/git_timemachine/command/migrate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,78 +1,63 @@
 import os
-from os import PathLike
 from datetime import datetime, timedelta
+from pathlib import Path
 
 import click
-from pygit2 import discover_repository, init_repository, Repository, Signature
+from pygit2 import discover_repository, init_repository, Repository, Signature, GitError
 from pygit2 import GIT_SORT_REVERSE, GIT_DIFF_REVERSE, GIT_DIFF_SHOW_BINARY, GIT_APPLY_LOCATION_BOTH
-from git_timemachine.utils import print_error
+
+from git_timemachine.git import create_repo_commit
 
 
 @click.command('migrate')
-@click.argument('src_dir', type=click.Path(exists=True, file_okay=False), default=os.getcwd())
-@click.argument('dest_dir', type=click.Path(exists=False, file_okay=False), required=False, default=None)
-@click.option('-o', '--offset', help='Time offset for each commit.', type=str, required=False)
+@click.argument('dest_dir', type=click.Path(exists=False, file_okay=False), required=True)
+@click.option('-C', 'repo_dir', help='Path of repository directory.', type=click.Path(exists=True, file_okay=False), default=Path.cwd())
 @click.option('--default-head', help='Reference name of default HEAD', type=str, default='main')
-@click.pass_context
-def migrate_command(ctx: click.Context, src_dir: PathLike, dest_dir: PathLike, offset: str, default_head: str):
-    """Migrate commit logs from a repository to another."""
-
-    if dest_dir is None:
-        dest_dir = f'{src_dir}.migrated'
+@click.option('-d', '--delta', help='Time delta for each commit.', type=str, required=False)
+def migrate_command(dest_dir: os.PathLike, repo_dir: os.PathLike, default_head: str, delta: str):
+    """Migrate commits from a repository to another."""
 
     if os.path.exists(dest_dir):
         raise FileExistsError(f'Destination directory {dest_dir} already exists.')
 
-    os.mkdir(dest_dir, 0o755)
+    delta_seconds = 0
+    if delta is not None:
+        delta_factor = {'s': 1, 'm': 60, 'h': 60 * 60, 'd': 60 * 60 * 24}
 
-    src_repo = Repository(discover_repository(str(src_dir)))
-    dest_repo = init_repository(dest_dir, initial_head=default_head)
+        if delta[-1] not in delta_factor:
+            raise ValueError(f'Unknown delta unit: {delta[-1]}')
 
-    parent = []
+        delta_seconds = int(delta[:-1]) * delta_factor[delta[-1]]
+
+    os.mkdir(dest_dir)
+
+    src_repo = Repository(discover_repository(str(repo_dir)))
+    dest_repo = init_repository(dest_dir, initial_head=default_head)
 
-    ref_name = f'refs/heads/{default_head}'
+    parents = []
 
     for commit in src_repo.walk(src_repo.head.target, GIT_SORT_REVERSE):
         if len(commit.parents) > 0:
             diff = commit.tree.diff_to_tree(commit.parents[0].tree, flags=GIT_DIFF_REVERSE | GIT_DIFF_SHOW_BINARY)
         else:
             diff = commit.tree.diff_to_tree(flags=GIT_DIFF_REVERSE | GIT_DIFF_SHOW_BINARY)
 
         dest_repo.apply(diff, location=GIT_APPLY_LOCATION_BOTH)
         dest_repo.index.write()
 
-        tree = dest_repo.index.write_tree()
+        commit_time = datetime.fromtimestamp(commit.author.time) + timedelta(seconds=delta_seconds)
 
-        if tree is None:
-            print_error('Failed to write index tree.')
-            ctx.exit(1)
-
-        seconds = 0
-        if offset is not None:
-            unit = offset[-1]
-            multi = {'s': 1, 'm': 60, 'h': 60 * 60, 'd': 60 * 60 * 24}
-
-            if unit not in multi:
-                raise ValueError(f'Unknown offset unit: {unit}')
-
-            seconds = int(offset[:-1]) * multi[unit]
-
-        dt = datetime.fromtimestamp(commit.author.time) + timedelta(seconds=seconds)
-
-        author = Signature(
+        signature = Signature(
             name=commit.author.name,
             email=commit.author.email,
-            time=int(dt.timestamp()),
+            time=int(commit_time.replace(microsecond=0).timestamp()),
             encoding='utf-8',
-            offset=int(dt.astimezone().tzinfo.utcoffset(dt).seconds / 60)
+            offset=int(commit_time.astimezone().tzinfo.utcoffset(commit_time).seconds / 60)
         )
 
-        committer = author
-
-        oid = dest_repo.create_commit(ref_name, author, committer, commit.message, tree, parent)
+        oid = create_repo_commit(dest_repo, f'refs/heads/{default_head}', signature, commit.message, parents)
 
         if oid is None:
-            print_error('Failed to create commit.')
-            ctx.exit(1)
+            raise GitError('Failed to create commit.')
 
-        parent = [dest_repo.head.target]
+        parents = [dest_repo.head.target]
```

### Comparing `git_timemachine-1.3.1/src/git_timemachine/state.py` & `git_timemachine-2.0.0/src/git_timemachine/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import json
 from os import PathLike, path
 from typing import Any
 from datetime import datetime
 
 
-class StateFile:
-    raw: dict = {}
-    filename: PathLike
+class PropertyFile:
+    raw: dict
+    filepath: PathLike
+
+    def __init__(self, filepath: PathLike):
+        self.filepath = filepath
+        self.raw = {}
 
-    def __init__(self, filename: PathLike):
-        self.filename = filename
-
-        if path.exists(filename):
-            with open(filename, 'r', encoding='utf-8') as fp:
+        if path.exists(filepath):
+            with open(filepath, 'r', encoding='utf-8') as fp:
                 self.raw = json.load(fp)
 
     def get(self, key: str, default=None) -> Any:
         if key not in self.raw:
             return default
 
         value = self.raw[key]
@@ -32,9 +33,12 @@
             self.raw[key] = {
                 'type': 'datetime',
                 'value': value.replace(microsecond=0).astimezone().isoformat()
             }
         else:
             self.raw[key] = value
 
-        with open(self.filename, 'w', encoding='utf-8') as fp:
+        with open(self.filepath, 'w', encoding='utf-8') as fp:
             json.dump(self.raw, fp, ensure_ascii=False, indent=4)
+
+    def exists(self, key: str):
+        return key in self.raw
```

### Comparing `git_timemachine-1.3.1/PKG-INFO` & `git_timemachine-2.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-timemachine
-Version: 1.3.1
+Version: 2.0.0
 Summary: A command-line tool that helps you record commits on Git repositories at any time node.
 Home-page: https://github.com/he-yaowen/git-timemachine
 License: GPL-3.0
 Author: HE Yaowen
 Author-email: he.yaowen@hotmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -19,25 +19,15 @@
 Description-Content-Type: text/markdown
 
 # git-timemachine
 
 A command-line tool that helps you record commits on [Git][1] repositories at
 any time node.
 
-## Installation
-
-git-timemachine requires python version 3.8 or higher.
-
-With pip:
-
-```
-pip install --user git-timemachine
-```
-
 ## License
 
 Copyright (C) 2022 HE Yaowen <he.yaowen@hotmail.com>
 
-The GNU General Public License (GPL) version 3, see [LICENSE](./LICENSE).
+The GNU General Public License (GPL) version 3, see [COPYING](./COPYING).
 
 [1]: https://git-scm.com/
```

