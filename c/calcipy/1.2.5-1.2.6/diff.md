# Comparing `tmp/calcipy-1.2.5.tar.gz` & `tmp/calcipy-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calcipy-1.2.5.tar", max compression
+gzip compressed data, was "calcipy-1.2.6.tar", max compression
```

## Comparing `calcipy-1.2.5.tar` & `calcipy-1.2.6.tar`

### file list

```diff
@@ -1,35 +1,34 @@
--rw-r--r--   0        0        0     1066 2023-05-13 11:22:49.916008 calcipy-1.2.5/LICENSE
--rw-r--r--   0        0        0      167 2023-05-23 22:23:44.941141 calcipy-1.2.5/calcipy/__init__.py
--rw-r--r--   0        0        0     1241 2023-05-13 10:55:19.213121 calcipy-1.2.5/calcipy/can_skip.py
--rw-r--r--   0        0        0      175 2023-03-02 02:58:57.029784 calcipy-1.2.5/calcipy/check_for_stale_packages/__init__.py
--rw-r--r--   0        0        0     8262 2023-05-13 00:16:53.654649 calcipy-1.2.5/calcipy/check_for_stale_packages/_check_for_stale_packages.py
--rw-r--r--   0        0        0     6436 2023-05-17 11:02:50.475557 calcipy-1.2.5/calcipy/cli.py
--rw-r--r--   0        0        0      154 2023-03-02 02:58:57.946199 calcipy-1.2.5/calcipy/code_tag_collector/__init__.py
--rw-r--r--   0        0        0    10840 2023-05-13 11:22:33.621932 calcipy-1.2.5/calcipy/code_tag_collector/_collector.py
--rw-r--r--   0        0        0      140 2023-03-02 02:58:58.498973 calcipy-1.2.5/calcipy/dot_dict/__init__.py
--rw-r--r--   0        0        0      803 2023-02-25 23:58:05.004832 calcipy-1.2.5/calcipy/dot_dict/_dot_dict.py
--rw-r--r--   0        0        0        0 2023-04-05 02:28:27.975837 calcipy-1.2.5/calcipy/experiments/__init__.py
--rw-r--r--   0        0        0     1988 2023-05-13 11:16:09.447581 calcipy-1.2.5/calcipy/experiments/check_duplicate_test_names.py
--rw-r--r--   0        0        0     3271 2023-02-23 02:19:12.613926 calcipy-1.2.5/calcipy/file_search.py
--rw-r--r--   0        0        0     1942 2023-05-17 11:00:03.480459 calcipy-1.2.5/calcipy/invoke_helpers.py
--rw-r--r--   0        0        0      162 2023-03-02 02:58:58.973806 calcipy-1.2.5/calcipy/md_writer/__init__.py
--rw-r--r--   0        0        0     7833 2023-04-22 15:51:43.990661 calcipy-1.2.5/calcipy/md_writer/_writer.py
--rw-r--r--   0        0        0      162 2023-03-02 02:58:59.584964 calcipy-1.2.5/calcipy/noxfile/__init__.py
--rw-r--r--   0        0        0     6546 2023-04-22 15:10:18.113523 calcipy-1.2.5/calcipy/noxfile/_noxfile.py
--rw-r--r--   0        0        0     1258 2023-05-17 10:59:02.930491 calcipy-1.2.5/calcipy/scripts.py
--rw-r--r--   0        0        0        0 2023-02-21 03:18:10.928974 calcipy-1.2.5/calcipy/tasks/__init__.py
--rw-r--r--   0        0        0     3488 2023-05-17 11:01:15.749443 calcipy-1.2.5/calcipy/tasks/all_tasks.py
--rw-r--r--   0        0        0     1884 2023-05-16 23:59:46.273109 calcipy-1.2.5/calcipy/tasks/cl.py
--rw-r--r--   0        0        0     1169 2023-05-17 10:45:25.212981 calcipy-1.2.5/calcipy/tasks/defaults.py
--rw-r--r--   0        0        0     3617 2023-05-16 23:59:46.277097 calcipy-1.2.5/calcipy/tasks/doc.py
--rw-r--r--   0        0        0     3893 2023-05-17 00:35:52.385145 calcipy-1.2.5/calcipy/tasks/lint.py
--rw-r--r--   0        0        0      462 2023-05-16 23:59:46.283536 calcipy-1.2.5/calcipy/tasks/nox.py
--rw-r--r--   0        0        0     1667 2023-05-17 10:56:42.232544 calcipy-1.2.5/calcipy/tasks/pack.py
--rw-r--r--   0        0        0      565 2023-05-16 23:59:46.291723 calcipy-1.2.5/calcipy/tasks/stale.py
--rw-r--r--   0        0        0     1506 2023-05-16 23:59:46.294332 calcipy-1.2.5/calcipy/tasks/tags.py
--rw-r--r--   0        0        0     3667 2023-05-16 23:59:46.301475 calcipy-1.2.5/calcipy/tasks/test.py
--rw-r--r--   0        0        0      642 2023-05-16 23:59:46.303934 calcipy-1.2.5/calcipy/tasks/types.py
--rw-r--r--   0        0        0     6651 2023-05-23 22:23:51.404030 calcipy-1.2.5/docs/README.md
--rw-r--r--   0        0        0     6547 2023-05-23 22:23:44.978905 calcipy-1.2.5/pyproject.toml
--rw-r--r--   0        0        0     9989 1970-01-01 00:00:00.000000 calcipy-1.2.5/setup.py
--rw-r--r--   0        0        0    11420 1970-01-01 00:00:00.000000 calcipy-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-17 12:45:29.997841 calcipy-1.2.6/LICENSE
+-rw-r--r--   0        0        0      167 2023-06-17 13:10:01.526420 calcipy-1.2.6/calcipy/__init__.py
+-rw-r--r--   0        0        0     1241 2023-05-13 10:55:19.213121 calcipy-1.2.6/calcipy/can_skip.py
+-rw-r--r--   0        0        0      175 2023-03-02 02:58:57.029784 calcipy-1.2.6/calcipy/check_for_stale_packages/__init__.py
+-rw-r--r--   0        0        0     8307 2023-06-17 12:44:50.659243 calcipy-1.2.6/calcipy/check_for_stale_packages/_check_for_stale_packages.py
+-rw-r--r--   0        0        0     6436 2023-05-17 11:02:50.475557 calcipy-1.2.6/calcipy/cli.py
+-rw-r--r--   0        0        0      154 2023-03-02 02:58:57.946199 calcipy-1.2.6/calcipy/code_tag_collector/__init__.py
+-rw-r--r--   0        0        0    11131 2023-06-17 12:45:50.740401 calcipy-1.2.6/calcipy/code_tag_collector/_collector.py
+-rw-r--r--   0        0        0      140 2023-03-02 02:58:58.498973 calcipy-1.2.6/calcipy/dot_dict/__init__.py
+-rw-r--r--   0        0        0      803 2023-02-25 23:58:05.004832 calcipy-1.2.6/calcipy/dot_dict/_dot_dict.py
+-rw-r--r--   0        0        0        0 2023-04-05 02:28:27.975837 calcipy-1.2.6/calcipy/experiments/__init__.py
+-rw-r--r--   0        0        0     1988 2023-05-13 11:16:09.447581 calcipy-1.2.6/calcipy/experiments/check_duplicate_test_names.py
+-rw-r--r--   0        0        0     3271 2023-02-23 02:19:12.613926 calcipy-1.2.6/calcipy/file_search.py
+-rw-r--r--   0        0        0     1942 2023-05-17 11:00:03.480459 calcipy-1.2.6/calcipy/invoke_helpers.py
+-rw-r--r--   0        0        0      162 2023-03-02 02:58:58.973806 calcipy-1.2.6/calcipy/md_writer/__init__.py
+-rw-r--r--   0        0        0     7827 2023-05-31 23:56:53.468487 calcipy-1.2.6/calcipy/md_writer/_writer.py
+-rw-r--r--   0        0        0      162 2023-03-02 02:58:59.584964 calcipy-1.2.6/calcipy/noxfile/__init__.py
+-rw-r--r--   0        0        0     6546 2023-04-22 15:10:18.113523 calcipy-1.2.6/calcipy/noxfile/_noxfile.py
+-rw-r--r--   0        0        0     1258 2023-05-17 10:59:02.930491 calcipy-1.2.6/calcipy/scripts.py
+-rw-r--r--   0        0        0        0 2023-02-21 03:18:10.928974 calcipy-1.2.6/calcipy/tasks/__init__.py
+-rw-r--r--   0        0        0     3488 2023-05-17 11:01:15.749443 calcipy-1.2.6/calcipy/tasks/all_tasks.py
+-rw-r--r--   0        0        0     1884 2023-05-16 23:59:46.273109 calcipy-1.2.6/calcipy/tasks/cl.py
+-rw-r--r--   0        0        0     1169 2023-05-17 10:45:25.212981 calcipy-1.2.6/calcipy/tasks/defaults.py
+-rw-r--r--   0        0        0     3617 2023-05-16 23:59:46.277097 calcipy-1.2.6/calcipy/tasks/doc.py
+-rw-r--r--   0        0        0     3896 2023-05-28 12:34:20.588583 calcipy-1.2.6/calcipy/tasks/lint.py
+-rw-r--r--   0        0        0      462 2023-05-16 23:59:46.283536 calcipy-1.2.6/calcipy/tasks/nox.py
+-rw-r--r--   0        0        0     1667 2023-05-17 10:56:42.232544 calcipy-1.2.6/calcipy/tasks/pack.py
+-rw-r--r--   0        0        0      565 2023-05-16 23:59:46.291723 calcipy-1.2.6/calcipy/tasks/stale.py
+-rw-r--r--   0        0        0     1506 2023-05-16 23:59:46.294332 calcipy-1.2.6/calcipy/tasks/tags.py
+-rw-r--r--   0        0        0     3667 2023-05-16 23:59:46.301475 calcipy-1.2.6/calcipy/tasks/test.py
+-rw-r--r--   0        0        0      642 2023-05-16 23:59:46.303934 calcipy-1.2.6/calcipy/tasks/types.py
+-rw-r--r--   0        0        0     6651 2023-06-17 13:10:08.138851 calcipy-1.2.6/docs/README.md
+-rw-r--r--   0        0        0     6547 2023-06-17 13:10:01.567848 calcipy-1.2.6/pyproject.toml
+-rw-r--r--   0        0        0    11268 1970-01-01 00:00:00.000000 calcipy-1.2.6/PKG-INFO
```

### Comparing `calcipy-1.2.5/LICENSE` & `calcipy-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.5/calcipy/can_skip.py` & `calcipy-1.2.6/calcipy/can_skip.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.5/calcipy/check_for_stale_packages/_check_for_stale_packages.py` & `calcipy-1.2.6/calcipy/check_for_stale_packages/_check_for_stale_packages.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,28 +197,29 @@
     stale_packages = [pack for pack in packages if not pack.datetime or pack.datetime < stale_cutoff]
     # TODO: If no stale, write out five oldest?
     if stale_packages:
         pkgs = sorted(stale_packages, key=lambda x: x.datetime or stale_cutoff)
         stale_list = '\n'.join([format_package(_p) for _p in pkgs])
         logger.warning('Found stale packages that may be a dependency risk', stale_list=stale_list)
         return True
-    oldest_date = np.amin([pack.datetime for pack in packages])  # pyright: ignore[reportGeneralTypeIssues]
-    logger.text('No stale packages found', oldest=oldest_date.humanize(), stale_threshold=stale_months)
+    if packages:
+        oldest_date = np.amin([pack.datetime for pack in packages])  # pyright: ignore[reportGeneralTypeIssues]
+        logger.text('No stale packages found', oldest=oldest_date.humanize(), stale_threshold=stale_months)
     return False
 
 
 @beartype
 def check_for_stale_packages(*, stale_months: int, path_lock: Path = LOCK, path_cache: Path = CALCIPY_CACHE) -> bool:
     """Read the cached packaging information.
 
     Args:
         stale_months: cutoff in months for when a package might be stale enough to be a risk
 
     """
     packages = _read_packages(path_lock)
     cached_packages = _read_cache(path_cache)
-    if can_skip.can_skip(prerequisites=[path_lock], targets=[path_cache]):
+    if cached_packages and can_skip.can_skip(prerequisites=[path_lock], targets=[path_cache]):
         packages = [*cached_packages.values()]
     else:
         packages = _collect_release_dates(packages, cached_packages)
         _write_cache(packages, path_cache)
     return _packages_are_stale(packages, stale_months=stale_months)
```

### Comparing `calcipy-1.2.5/calcipy/cli.py` & `calcipy-1.2.6/calcipy/cli.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.5/calcipy/code_tag_collector/_collector.py` & `calcipy-1.2.6/calcipy/code_tag_collector/_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,35 @@
 
         if comments := _search_lines(lines, regex_compiled):
             matches.append(_Tags(path_source=path_source, code_tags=comments))
 
     return matches
 
 
+@beartype
+def github_blame_url(clone_uri: str) -> str:
+    """Format the blame URL.
+
+    Args:
+        clone_uri: git remote URI
+
+    Returns:
+       str: `repo_url`
+
+    """
+    github_url = 'https://github.com/'
+    # Could be ssh or http (with or without .git)
+    # > git@github.com:KyleKing/calcipy.git
+    # > https://github.com/KyleKing/calcipy.git
+    matches = re.findall(r'^.+github.com[:/]([^.]+)(?:\.git)?$', clone_uri)
+    with suppress(IndexError):
+        return f'{github_url}{matches[0]}'
+    return ''
+
+
 @lru_cache(maxsize=128)
 @beartype
 def _git_info(cwd: Path) -> Tuple[Path, str]:
     """Collect information about the local git repository.
 
     Based on snippets from: https://gist.github.com/abackstrom/4034721#gistcomment-3982270
     and: https://github.com/rscherf/GitLink/blob/e2e7c412630246efc86de4fe71192f15bf11209e/GitLink.py
@@ -126,23 +147,18 @@
         cwd: Path to the current working directory (typically file_path.parent)
 
     Returns:
         Tuple[Path, str]: (git_dir, repo_url)
 
     """
     git_dir = Path(capture_shell('git rev-parse --show-toplevel', cwd=cwd))
-    clone_uri = 'https://github.com/'
+    clone_uri = ''
     with suppress(CalledProcessError):
         clone_uri = capture_shell('git remote get-url origin', cwd=cwd)
-    # Could be ssh or http (with or without .git)
-    # > git@github.com:KyleKing/calcipy.git
-    # > https://github.com/KyleKing/calcipy.git
-    sub_url = re.findall(r'^.+github.com[:/]([^.]+)(?:\.git)?$', clone_uri)[0]
-    repo_url = f'https://github.com/{sub_url}'
-    return git_dir, repo_url
+    return git_dir, github_blame_url(clone_uri)
 
 
 class _CollectorRow(BaseModel):
     """Each row of the Code Tag table."""
 
     tag_name: str
     comment: str
@@ -178,19 +194,20 @@
 
     # Handle uncommitted files that only have author-time and author-tz
     user = 'committer' if 'committer-tz' in blame_dict else 'author'
     dt = arrow.get(int(blame_dict[f'{user}-time']))
     tz = blame_dict[f'{user}-tz'][:3] + ':' + blame_dict[f'{user}-tz'][-2:]
     collector_row.last_edit = arrow.get(dt.isoformat()[:-6] + tz).format('YYYY-MM-DD')
 
-    # Filename may not be present if uncommitted. Use local path as fallback
-    remote_file_path = blame_dict.get('filename', rel_path.as_posix())
-    # Assumes Github format
-    git_url = f'{repo_url}/blame/{revision}/{remote_file_path}#L{old_line_number}'
-    collector_row.source_file = f'[{collector_row.source_file}]({git_url})'
+    if repo_url:
+        # Filename may not be present if uncommitted. Use local path as fallback
+        remote_file_path = blame_dict.get('filename', rel_path.as_posix())
+        # Assumes Github format
+        git_url = f'{repo_url}/blame/{revision}/{remote_file_path}#L{old_line_number}'
+        collector_row.source_file = f'[{collector_row.source_file}]({git_url})'
 
     return collector_row
 
 
 @beartype
 def _format_record(base_dir: Path, file_path: Path, comment: _CodeTag) -> _CollectorRow:
     """Format each table row for the code tag summary file. Include git permalink.
```

### Comparing `calcipy-1.2.5/calcipy/dot_dict/_dot_dict.py` & `calcipy-1.2.6/calcipy/dot_dict/_dot_dict.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.5/calcipy/experiments/check_duplicate_test_names.py` & `calcipy-1.2.6/calcipy/experiments/check_duplicate_test_names.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.5/calcipy/file_search.py` & `calcipy-1.2.6/calcipy/file_search.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.5/calcipy/invoke_helpers.py` & `calcipy-1.2.6/calcipy/invoke_helpers.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.5/calcipy/md_writer/_writer.py` & `calcipy-1.2.6/calcipy/md_writer/_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,15 @@
     language = path_source.suffix.lstrip('.')
     lines_source = [f'```{language}', *read_lines(path_source), '```']
     if not path_source.is_file():
         logger.warning('Could not locate source file', path_source=path_source)
 
     line_start = f'<!-- {{cts}} {key}={path_rel}; -->'
     line_end = '<!-- {cte} -->'
-    return [line_start, *lines_source] + [line_end]
+    return [line_start, *lines_source, line_end]
 
 
 @beartype
 def _format_cov_table(coverage_data: Dict[str, Any]) -> List[str]:
     """Format code coverage data table as markdown.
 
     Args:
@@ -209,15 +209,15 @@
     path_coverage = path_coverage or get_project_path() / 'coverage.json'
     if not path_coverage.is_file():
         msg = f'Could not locate: {path_coverage}'
         raise _ParseSkipError(msg)
     coverage_data = json.loads(path_coverage.read_text())
     lines_cov = _format_cov_table(coverage_data)
     line_end = '<!-- {cte} -->'
-    return [line, *lines_cov] + [line_end]
+    return [line, *lines_cov, line_end]
 
 
 @beartype
 def write_autoformatted_md_sections(
     handler_lookup: Optional[HandlerLookupT] = None,
     paths_md: Optional[List[Path]] = None,
 ) -> None:
```

### Comparing `calcipy-1.2.5/calcipy/noxfile/_noxfile.py` & `calcipy-1.2.6/calcipy/noxfile/_noxfile.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.5/calcipy/scripts.py` & `calcipy-1.2.6/calcipy/scripts.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.5/calcipy/tasks/all_tasks.py` & `calcipy-1.2.6/calcipy/tasks/all_tasks.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.5/calcipy/tasks/cl.py` & `calcipy-1.2.6/calcipy/tasks/cl.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.5/calcipy/tasks/defaults.py` & `calcipy-1.2.6/calcipy/tasks/defaults.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.5/calcipy/tasks/doc.py` & `calcipy-1.2.6/calcipy/tasks/doc.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.5/calcipy/tasks/lint.py` & `calcipy-1.2.6/calcipy/tasks/lint.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from corallium.log import logger
 from invoke.context import Context
 
 from ..cli import task
 from ..invoke_helpers import run
 
 # ==============================================================================
-# Ruff
+# Linting
 
 
 @beartype
 def _inner_task(
     ctx: Context,
     *,
     cli_args: str,
```

### Comparing `calcipy-1.2.5/calcipy/tasks/pack.py` & `calcipy-1.2.6/calcipy/tasks/pack.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.5/calcipy/tasks/stale.py` & `calcipy-1.2.6/calcipy/tasks/stale.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.5/calcipy/tasks/tags.py` & `calcipy-1.2.6/calcipy/tasks/tags.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.5/calcipy/tasks/test.py` & `calcipy-1.2.6/calcipy/tasks/test.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.5/calcipy/tasks/types.py` & `calcipy-1.2.6/calcipy/tasks/types.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.5/docs/README.md` & `calcipy-1.2.6/docs/README.md`

 * *Files identical despite different names*

### Comparing `calcipy-1.2.5/pyproject.toml` & `calcipy-1.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.commitizen]
-version = "1.2.5"
+version = "1.2.6"
 version_files = ["calcipy/__init__.py:^__version", "pyproject.toml:^version"]
 
 [tool.poetry]
 authors = ["Kyle King <dev.act.kyle@gmail.com>"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Framework :: Pytest",
@@ -26,15 +26,15 @@
 include = ["LICENSE"]
 keywords = ["nox", "python-poetry"]
 license = "MIT"
 maintainers = []
 name = "calcipy"
 readme = "docs/README.md"
 repository = "https://github.com/kyleking/calcipy"
-version = "1.2.5"
+version = "1.2.6"
 
 [tool.poetry.dependencies]
 python = "^3.8.12"
 arrow = {optional = true, version = ">=1.2.3"} # tags
 autopep8 = {optional = true, version = ">=2.0.1"} # flake8
 bandit = {optional = true, version = ">=1.7.4"} # lint
 beartype = ">=0.12.0"
@@ -81,15 +81,15 @@
 pytest = {optional = true, version = ">=7.2.1"} # test
 pytest-cov = {optional = true, version = ">=4.0.0"} # test
 pytest-randomly = {optional = true, version = ">=3.12.0"} # test
 pytest-watcher = {optional = true, version = ">=0.2.6"} # test
 python-box = {optional = true, version = ">=6.0.2"} # ddict
 pyyaml = {optional = true, version = ">=5.2"} # doc,tags
 requests = {optional = true, version = ">=2.31.0"} # stale
-ruff = {optional = true, version = ">=0.0.253"} # lint
+ruff = {optional = true, version = ">=0.0.272"} # lint
 semgrep = {optional = true, version = ">=1.12.1"} # lint
 tabulate = {optional = true, version = ">=0.9.0"} # tags: Required for pandas to markdown
 transitions = {optional = true, version = ">=0.9.0"} # tags: docs
 
 [tool.poetry.extras]
 ddict = ["python-box"]
 doc = [
```

### Comparing `calcipy-1.2.5/PKG-INFO` & `calcipy-1.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcipy
-Version: 1.2.5
+Version: 1.2.6
 Summary: Python package to simplify development
 Home-page: https://github.com/kyleking/calcipy
 License: MIT
 Keywords: nox,python-poetry
 Author: Kyle King
 Author-email: dev.act.kyle@gmail.com
 Requires-Python: >=3.8.12,<4.0.0
@@ -13,18 +13,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Provides-Extra: ddict
 Provides-Extra: doc
 Provides-Extra: flake8
 Provides-Extra: lint
 Provides-Extra: nox
@@ -80,15 +77,15 @@
 Requires-Dist: pytest (>=7.2.1) ; extra == "test"
 Requires-Dist: pytest-cov (>=4.0.0) ; extra == "test"
 Requires-Dist: pytest-randomly (>=3.12.0) ; extra == "test"
 Requires-Dist: pytest-watcher (>=0.2.6) ; extra == "test"
 Requires-Dist: python-box (>=6.0.2) ; extra == "ddict"
 Requires-Dist: pyyaml (>=5.2) ; extra == "doc" or extra == "tags"
 Requires-Dist: requests (>=2.31.0) ; extra == "stale"
-Requires-Dist: ruff (>=0.0.253) ; extra == "lint"
+Requires-Dist: ruff (>=0.0.272) ; extra == "lint"
 Requires-Dist: semgrep (>=1.12.1) ; extra == "lint"
 Requires-Dist: tabulate (>=0.9.0) ; extra == "tags"
 Requires-Dist: transitions (>=0.9.0) ; extra == "doc"
 Project-URL: Bug Tracker, https://github.com/kyleking/calcipy/issues
 Project-URL: Changelog, https://github.com/kyleking/calcipy/blob/main/docs/docs/CHANGELOG.md
 Project-URL: Documentation, https://calcipy.kyleking.me
 Project-URL: Repository, https://github.com/kyleking/calcipy
```

