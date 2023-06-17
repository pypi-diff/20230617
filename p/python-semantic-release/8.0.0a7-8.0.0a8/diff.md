# Comparing `tmp/python-semantic-release-8.0.0a7.tar.gz` & `tmp/python-semantic-release-8.0.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-semantic-release-8.0.0a7.tar", last modified: Sun Jun 11 19:23:09 2023, max compression
+gzip compressed data, was "python-semantic-release-8.0.0a8.tar", last modified: Tue Jun 13 17:37:59 2023, max compression
```

## Comparing `python-semantic-release-8.0.0a7.tar` & `python-semantic-release-8.0.0a8.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.863366 python-semantic-release-8.0.0a7/
--rw-r--r--   0 root         (0) root         (0)      230 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)     1084 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/LICENSE
--rw-r--r--   0 root         (0) root         (0)      153 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3110 2023-06-11 19:23:09.863366 python-semantic-release-8.0.0a7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2272 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/README.rst
--rw-r--r--   0 root         (0) root         (0)     4687 2023-06-11 19:23:01.000000 python-semantic-release-8.0.0a7/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.843366 python-semantic-release-8.0.0a7/python_semantic_release.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3110 2023-06-11 19:23:09.000000 python-semantic-release-8.0.0a7/python_semantic_release.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4221 2023-06-11 19:23:09.000000 python-semantic-release-8.0.0a7/python_semantic_release.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-11 19:23:09.000000 python-semantic-release-8.0.0a7/python_semantic_release.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       95 2023-06-11 19:23:09.000000 python-semantic-release-8.0.0a7/python_semantic_release.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      598 2023-06-11 19:23:09.000000 python-semantic-release-8.0.0a7/python_semantic_release.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-11 19:23:09.000000 python-semantic-release-8.0.0a7/python_semantic_release.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.843366 python-semantic-release-8.0.0a7/semantic_release/
--rw-r--r--   0 root         (0) root         (0)     1093 2023-06-11 19:23:01.000000 python-semantic-release-8.0.0a7/semantic_release/__init__.py
--rw-r--r--   0 root         (0) root         (0)      106 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.847366 python-semantic-release-8.0.0a7/semantic_release/changelog/
--rw-r--r--   0 root         (0) root         (0)      361 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/changelog/__init__.py
--rw-r--r--   0 root         (0) root         (0)      941 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/changelog/context.py
--rw-r--r--   0 root         (0) root         (0)     6470 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/changelog/release_history.py
--rw-r--r--   0 root         (0) root         (0)     4328 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/changelog/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.847366 python-semantic-release-8.0.0a7/semantic_release/cli/
--rw-r--r--   0 root         (0) root         (0)      451 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.847366 python-semantic-release-8.0.0a7/semantic_release/cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/cli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3246 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/cli/commands/changelog.py
--rw-r--r--   0 root         (0) root         (0)     1448 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/cli/commands/generate_config.py
--rw-r--r--   0 root         (0) root         (0)     4978 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/cli/commands/main.py
--rw-r--r--   0 root         (0) root         (0)     1298 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/cli/commands/publish.py
--rw-r--r--   0 root         (0) root         (0)    18650 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/cli/commands/version.py
--rw-r--r--   0 root         (0) root         (0)      929 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/cli/common.py
--rw-r--r--   0 root         (0) root         (0)    13718 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/cli/config.py
--rw-r--r--   0 root         (0) root         (0)       39 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/cli/const.py
--rw-r--r--   0 root         (0) root         (0)     2105 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/cli/github_actions_output.py
--rw-r--r--   0 root         (0) root         (0)     2875 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/cli/masking_filter.py
--rw-r--r--   0 root         (0) root         (0)      935 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/cli/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.851366 python-semantic-release-8.0.0a7/semantic_release/commit_parser/
--rw-r--r--   0 root         (0) root         (0)      884 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/commit_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2569 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/commit_parser/_base.py
--rw-r--r--   0 root         (0) root         (0)     4364 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/commit_parser/angular.py
--rw-r--r--   0 root         (0) root         (0)     3288 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/commit_parser/emoji.py
--rw-r--r--   0 root         (0) root         (0)     5713 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/commit_parser/scipy.py
--rw-r--r--   0 root         (0) root         (0)     3193 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/commit_parser/tag.py
--rw-r--r--   0 root         (0) root         (0)     1456 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/commit_parser/token.py
--rw-r--r--   0 root         (0) root         (0)      529 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/commit_parser/util.py
--rw-r--r--   0 root         (0) root         (0)      831 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.839366 python-semantic-release-8.0.0a7/semantic_release/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.851366 python-semantic-release-8.0.0a7/semantic_release/data/templates/
--rw-r--r--   0 root         (0) root         (0)     1059 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/data/templates/CHANGELOG.md.j2
--rw-r--r--   0 root         (0) root         (0)      465 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/data/templates/release_notes.md.j2
--rw-r--r--   0 root         (0) root         (0)     1020 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/enums.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/errors.py
--rw-r--r--   0 root         (0) root         (0)     4088 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.851366 python-semantic-release-8.0.0a7/semantic_release/hvcs/
--rw-r--r--   0 root         (0) root         (0)      300 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/hvcs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5579 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/hvcs/_base.py
--rw-r--r--   0 root         (0) root         (0)     8285 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/hvcs/gitea.py
--rw-r--r--   0 root         (0) root         (0)    10154 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/hvcs/github.py
--rw-r--r--   0 root         (0) root         (0)     5029 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/hvcs/gitlab.py
--rw-r--r--   0 root         (0) root         (0)      681 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/hvcs/token_auth.py
--rw-r--r--   0 root         (0) root         (0)     2774 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/hvcs/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.851366 python-semantic-release-8.0.0a7/semantic_release/version/
--rw-r--r--   0 root         (0) root         (0)      339 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/version/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14177 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/version/algorithm.py
--rw-r--r--   0 root         (0) root         (0)     7267 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/version/declaration.py
--rw-r--r--   0 root         (0) root         (0)     3103 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/version/translator.py
--rw-r--r--   0 root         (0) root         (0)    14060 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/semantic_release/version/version.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-11 19:23:09.863366 python-semantic-release-8.0.0a7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      466 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.839366 python-semantic-release-8.0.0a7/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.855366 python-semantic-release-8.0.0a7/tests/command_line/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/command_line/__init__.py
--rw-r--r--   0 root         (0) root         (0)      174 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/command_line/conftest.py
--rw-r--r--   0 root         (0) root         (0)     5707 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/command_line/test_changelog.py
--rw-r--r--   0 root         (0) root         (0)     1320 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/command_line/test_generate_config.py
--rw-r--r--   0 root         (0) root         (0)      641 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/command_line/test_help.py
--rw-r--r--   0 root         (0) root         (0)     1167 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/command_line/test_main.py
--rw-r--r--   0 root         (0) root         (0)     1430 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/command_line/test_publish.py
--rw-r--r--   0 root         (0) root         (0)    19966 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/command_line/test_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.855366 python-semantic-release-8.0.0a7/tests/fixtures/
--rw-r--r--   0 root         (0) root         (0)      106 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/fixtures/__init__.py
--rw-r--r--   0 root         (0) root         (0)      906 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/fixtures/commit_parsers.py
--rw-r--r--   0 root         (0) root         (0)     2235 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/fixtures/example_project.py
--rw-r--r--   0 root         (0) root         (0)    45283 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/fixtures/git_repo.py
--rw-r--r--   0 root         (0) root         (0)     4424 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/fixtures/scipy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.855366 python-semantic-release-8.0.0a7/tests/scenario/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/scenario/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46838 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/scenario/test_next_version.py
--rw-r--r--   0 root         (0) root         (0)    12186 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/scenario/test_release_history.py
--rw-r--r--   0 root         (0) root         (0)     3513 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/scenario/test_template_render.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.855366 python-semantic-release-8.0.0a7/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.855366 python-semantic-release-8.0.0a7/tests/unit/semantic_release/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.859366 python-semantic-release-8.0.0a7/tests/unit/semantic_release/changelog/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/changelog/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5005 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/changelog/test_changelog_context.py
--rw-r--r--   0 root         (0) root         (0)     2540 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/changelog/test_default_changelog.py
--rw-r--r--   0 root         (0) root         (0)     1747 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/changelog/test_release_notes.py
--rw-r--r--   0 root         (0) root         (0)     2102 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/changelog/test_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.859366 python-semantic-release-8.0.0a7/tests/unit/semantic_release/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/cli/test_config.py
--rw-r--r--   0 root         (0) root         (0)     1784 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/cli/test_github_actions_output.py
--rw-r--r--   0 root         (0) root         (0)     5768 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/cli/test_masking_filter.py
--rw-r--r--   0 root         (0) root         (0)      799 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/cli/test_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.859366 python-semantic-release-8.0.0a7/tests/unit/semantic_release/commit_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/commit_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)      140 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/commit_parser/helper.py
--rw-r--r--   0 root         (0) root         (0)     5969 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/commit_parser/test_angular.py
--rw-r--r--   0 root         (0) root         (0)     2487 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/commit_parser/test_emoji.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/commit_parser/test_scipy.py
--rw-r--r--   0 root         (0) root         (0)     2173 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/commit_parser/test_tag.py
--rw-r--r--   0 root         (0) root         (0)      648 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/commit_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)      442 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/commit_parser/test_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.863366 python-semantic-release-8.0.0a7/tests/unit/semantic_release/hvcs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/hvcs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1349 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/hvcs/test__base.py
--rw-r--r--   0 root         (0) root         (0)    22874 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/hvcs/test_gitea.py
--rw-r--r--   0 root         (0) root         (0)    24334 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/hvcs/test_github.py
--rw-r--r--   0 root         (0) root         (0)    10021 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/hvcs/test_gitlab.py
--rw-r--r--   0 root         (0) root         (0)      965 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/hvcs/test_token_auth.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/hvcs/test_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 19:23:09.863366 python-semantic-release-8.0.0a7/tests/unit/semantic_release/version/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/version/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7319 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/version/test_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     3715 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/version/test_declaration.py
--rw-r--r--   0 root         (0) root         (0)     2996 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/version/test_translator.py
--rw-r--r--   0 root         (0) root         (0)     9640 2023-06-11 19:22:32.000000 python-semantic-release-8.0.0a7/tests/unit/semantic_release/version/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:37:59.344006 python-semantic-release-8.0.0a8/
+-rw-r--r--   0 root         (0) root         (0)      230 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)     1084 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      153 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3110 2023-06-13 17:37:59.344006 python-semantic-release-8.0.0a8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2272 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/README.rst
+-rw-r--r--   0 root         (0) root         (0)     4687 2023-06-13 17:37:50.000000 python-semantic-release-8.0.0a8/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:37:59.308006 python-semantic-release-8.0.0a8/python_semantic_release.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3110 2023-06-13 17:37:59.000000 python-semantic-release-8.0.0a8/python_semantic_release.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4221 2023-06-13 17:37:59.000000 python-semantic-release-8.0.0a8/python_semantic_release.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 17:37:59.000000 python-semantic-release-8.0.0a8/python_semantic_release.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       95 2023-06-13 17:37:59.000000 python-semantic-release-8.0.0a8/python_semantic_release.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      598 2023-06-13 17:37:59.000000 python-semantic-release-8.0.0a8/python_semantic_release.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-13 17:37:59.000000 python-semantic-release-8.0.0a8/python_semantic_release.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:37:59.312006 python-semantic-release-8.0.0a8/semantic_release/
+-rw-r--r--   0 root         (0) root         (0)     1093 2023-06-13 17:37:50.000000 python-semantic-release-8.0.0a8/semantic_release/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      106 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:37:59.312006 python-semantic-release-8.0.0a8/semantic_release/changelog/
+-rw-r--r--   0 root         (0) root         (0)      361 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/changelog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      941 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/changelog/context.py
+-rw-r--r--   0 root         (0) root         (0)     6470 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/changelog/release_history.py
+-rw-r--r--   0 root         (0) root         (0)     4328 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/changelog/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:37:59.316006 python-semantic-release-8.0.0a8/semantic_release/cli/
+-rw-r--r--   0 root         (0) root         (0)      451 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:37:59.320006 python-semantic-release-8.0.0a8/semantic_release/cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3246 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/cli/commands/changelog.py
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/cli/commands/generate_config.py
+-rw-r--r--   0 root         (0) root         (0)     4978 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/cli/commands/main.py
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/cli/commands/publish.py
+-rw-r--r--   0 root         (0) root         (0)    18650 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/cli/commands/version.py
+-rw-r--r--   0 root         (0) root         (0)      929 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/cli/common.py
+-rw-r--r--   0 root         (0) root         (0)    13706 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/cli/config.py
+-rw-r--r--   0 root         (0) root         (0)       39 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/cli/const.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/cli/github_actions_output.py
+-rw-r--r--   0 root         (0) root         (0)     2875 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/cli/masking_filter.py
+-rw-r--r--   0 root         (0) root         (0)      935 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/cli/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:37:59.320006 python-semantic-release-8.0.0a8/semantic_release/commit_parser/
+-rw-r--r--   0 root         (0) root         (0)      884 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/commit_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2569 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/commit_parser/_base.py
+-rw-r--r--   0 root         (0) root         (0)     4364 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/commit_parser/angular.py
+-rw-r--r--   0 root         (0) root         (0)     3288 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/commit_parser/emoji.py
+-rw-r--r--   0 root         (0) root         (0)     5713 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/commit_parser/scipy.py
+-rw-r--r--   0 root         (0) root         (0)     3193 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/commit_parser/tag.py
+-rw-r--r--   0 root         (0) root         (0)     1456 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/commit_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)      529 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/commit_parser/util.py
+-rw-r--r--   0 root         (0) root         (0)      831 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:37:59.304006 python-semantic-release-8.0.0a8/semantic_release/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:37:59.320006 python-semantic-release-8.0.0a8/semantic_release/data/templates/
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/data/templates/CHANGELOG.md.j2
+-rw-r--r--   0 root         (0) root         (0)      465 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/data/templates/release_notes.md.j2
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/enums.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/errors.py
+-rw-r--r--   0 root         (0) root         (0)     4088 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:37:59.324006 python-semantic-release-8.0.0a8/semantic_release/hvcs/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/hvcs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5579 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/hvcs/_base.py
+-rw-r--r--   0 root         (0) root         (0)     8285 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/hvcs/gitea.py
+-rw-r--r--   0 root         (0) root         (0)    10154 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/hvcs/github.py
+-rw-r--r--   0 root         (0) root         (0)     5029 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/hvcs/gitlab.py
+-rw-r--r--   0 root         (0) root         (0)      681 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/hvcs/token_auth.py
+-rw-r--r--   0 root         (0) root         (0)     2774 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/hvcs/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:37:59.324006 python-semantic-release-8.0.0a8/semantic_release/version/
+-rw-r--r--   0 root         (0) root         (0)      339 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14177 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/version/algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     7267 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/version/declaration.py
+-rw-r--r--   0 root         (0) root         (0)     3103 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/version/translator.py
+-rw-r--r--   0 root         (0) root         (0)    14060 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/semantic_release/version/version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 17:37:59.344006 python-semantic-release-8.0.0a8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      466 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:37:59.304006 python-semantic-release-8.0.0a8/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:37:59.328006 python-semantic-release-8.0.0a8/tests/command_line/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/command_line/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      190 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/command_line/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     5707 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/command_line/test_changelog.py
+-rw-r--r--   0 root         (0) root         (0)     1320 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/command_line/test_generate_config.py
+-rw-r--r--   0 root         (0) root         (0)      641 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/command_line/test_help.py
+-rw-r--r--   0 root         (0) root         (0)     1167 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/command_line/test_main.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/command_line/test_publish.py
+-rw-r--r--   0 root         (0) root         (0)    20288 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/command_line/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:37:59.332006 python-semantic-release-8.0.0a8/tests/fixtures/
+-rw-r--r--   0 root         (0) root         (0)      106 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/fixtures/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      906 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/fixtures/commit_parsers.py
+-rw-r--r--   0 root         (0) root         (0)     2235 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/fixtures/example_project.py
+-rw-r--r--   0 root         (0) root         (0)    45283 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/fixtures/git_repo.py
+-rw-r--r--   0 root         (0) root         (0)     4424 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/fixtures/scipy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:37:59.332006 python-semantic-release-8.0.0a8/tests/scenario/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/scenario/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    46838 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/scenario/test_next_version.py
+-rw-r--r--   0 root         (0) root         (0)    12186 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/scenario/test_release_history.py
+-rw-r--r--   0 root         (0) root         (0)     3513 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/scenario/test_template_render.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:37:59.332006 python-semantic-release-8.0.0a8/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:37:59.332006 python-semantic-release-8.0.0a8/tests/unit/semantic_release/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/unit/semantic_release/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:37:59.336006 python-semantic-release-8.0.0a8/tests/unit/semantic_release/changelog/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/unit/semantic_release/changelog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5005 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/unit/semantic_release/changelog/test_changelog_context.py
+-rw-r--r--   0 root         (0) root         (0)     2540 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/unit/semantic_release/changelog/test_default_changelog.py
+-rw-r--r--   0 root         (0) root         (0)     1747 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/unit/semantic_release/changelog/test_release_notes.py
+-rw-r--r--   0 root         (0) root         (0)     2102 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/unit/semantic_release/changelog/test_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:37:59.336006 python-semantic-release-8.0.0a8/tests/unit/semantic_release/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/unit/semantic_release/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/unit/semantic_release/cli/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     1784 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/unit/semantic_release/cli/test_github_actions_output.py
+-rw-r--r--   0 root         (0) root         (0)     5768 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/unit/semantic_release/cli/test_masking_filter.py
+-rw-r--r--   0 root         (0) root         (0)      799 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/unit/semantic_release/cli/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:37:59.340006 python-semantic-release-8.0.0a8/tests/unit/semantic_release/commit_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/unit/semantic_release/commit_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      140 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/unit/semantic_release/commit_parser/helper.py
+-rw-r--r--   0 root         (0) root         (0)     5969 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/unit/semantic_release/commit_parser/test_angular.py
+-rw-r--r--   0 root         (0) root         (0)     2487 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/unit/semantic_release/commit_parser/test_emoji.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/unit/semantic_release/commit_parser/test_scipy.py
+-rw-r--r--   0 root         (0) root         (0)     2173 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/unit/semantic_release/commit_parser/test_tag.py
+-rw-r--r--   0 root         (0) root         (0)      648 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/unit/semantic_release/commit_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)      442 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/unit/semantic_release/commit_parser/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:37:59.340006 python-semantic-release-8.0.0a8/tests/unit/semantic_release/hvcs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/unit/semantic_release/hvcs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1349 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/unit/semantic_release/hvcs/test__base.py
+-rw-r--r--   0 root         (0) root         (0)    22874 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/unit/semantic_release/hvcs/test_gitea.py
+-rw-r--r--   0 root         (0) root         (0)    24334 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/unit/semantic_release/hvcs/test_github.py
+-rw-r--r--   0 root         (0) root         (0)    10021 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/unit/semantic_release/hvcs/test_gitlab.py
+-rw-r--r--   0 root         (0) root         (0)      965 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/unit/semantic_release/hvcs/test_token_auth.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/unit/semantic_release/hvcs/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:37:59.344006 python-semantic-release-8.0.0a8/tests/unit/semantic_release/version/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/unit/semantic_release/version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7319 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/unit/semantic_release/version/test_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     3715 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/unit/semantic_release/version/test_declaration.py
+-rw-r--r--   0 root         (0) root         (0)     2996 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/unit/semantic_release/version/test_translator.py
+-rw-r--r--   0 root         (0) root         (0)     9640 2023-06-13 17:37:17.000000 python-semantic-release-8.0.0a8/tests/unit/semantic_release/version/test_version.py
```

### Comparing `python-semantic-release-8.0.0a7/LICENSE` & `python-semantic-release-8.0.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/PKG-INFO` & `python-semantic-release-8.0.0a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-semantic-release
-Version: 8.0.0a7
+Version: 8.0.0a8
 Summary: Automatic Semantic Versioning for Python projects
 Author-email: Rolf Erik Lekang <me@rolflekang.com>
 License: MIT
 Project-URL: Project Url, http://github.com/python-semantic-release/python-semantic-release
 Project-URL: Homepage, https://python-semantic-release.readthedocs.io
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python-semantic-release-8.0.0a7/README.rst` & `python-semantic-release-8.0.0a8/README.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/pyproject.toml` & `python-semantic-release-8.0.0a8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # and https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-semantic-release"
-version = "8.0.0-alpha.7"
+version = "8.0.0-alpha.8"
 description = "Automatic Semantic Versioning for Python projects"
 requires-python = ">=3.7"
 license = { text = "MIT" }
 classifiers = [
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.7",
```

### Comparing `python-semantic-release-8.0.0a7/python_semantic_release.egg-info/PKG-INFO` & `python-semantic-release-8.0.0a8/python_semantic_release.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-semantic-release
-Version: 8.0.0a7
+Version: 8.0.0a8
 Summary: Automatic Semantic Versioning for Python projects
 Author-email: Rolf Erik Lekang <me@rolflekang.com>
 License: MIT
 Project-URL: Project Url, http://github.com/python-semantic-release/python-semantic-release
 Project-URL: Homepage, https://python-semantic-release.readthedocs.io
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python-semantic-release-8.0.0a7/python_semantic_release.egg-info/SOURCES.txt` & `python-semantic-release-8.0.0a8/python_semantic_release.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/python_semantic_release.egg-info/requires.txt` & `python-semantic-release-8.0.0a8/python_semantic_release.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/__init__.py` & `python-semantic-release-8.0.0a8/semantic_release/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from semantic_release.version import (
     Version as Version,
     VersionTranslator as VersionTranslator,
     next_version as next_version,
     tags_and_versions as tags_and_versions,
 )
 
-__version__ = "8.0.0-alpha.7"
+__version__ = "8.0.0-alpha.8"
 
 
 def setup_hook(argv: list[str]) -> None:
     """
     A hook to be used in setup.py to enable `python setup.py publish`.
 
     :param argv: sys.argv
```

### Comparing `python-semantic-release-8.0.0a7/semantic_release/changelog/context.py` & `python-semantic-release-8.0.0a8/semantic_release/changelog/context.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/changelog/release_history.py` & `python-semantic-release-8.0.0a8/semantic_release/changelog/release_history.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/changelog/template.py` & `python-semantic-release-8.0.0a8/semantic_release/changelog/template.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/cli/commands/changelog.py` & `python-semantic-release-8.0.0a8/semantic_release/cli/commands/changelog.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/cli/commands/generate_config.py` & `python-semantic-release-8.0.0a8/semantic_release/cli/commands/generate_config.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/cli/commands/main.py` & `python-semantic-release-8.0.0a8/semantic_release/cli/commands/main.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/cli/commands/publish.py` & `python-semantic-release-8.0.0a8/semantic_release/cli/commands/publish.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/cli/commands/version.py` & `python-semantic-release-8.0.0a8/semantic_release/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/cli/common.py` & `python-semantic-release-8.0.0a8/semantic_release/cli/common.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/cli/config.py` & `python-semantic-release-8.0.0a8/semantic_release/cli/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 
 class PublishConfig(BaseModel):
     dist_glob_patterns: Tuple[str, ...] = ("dist/*",)
     upload_to_vcs_release: bool = True
 
 
 class RawConfig(BaseModel):
-    assets: Tuple[str, ...] = ()
+    assets: List[str] = []
     branches: Dict[str, BranchConfig] = {"main": BranchConfig()}
     build_command: Optional[str] = None
     changelog: ChangelogConfig = ChangelogConfig()
     commit_author: MaybeFromEnv = EnvConfigVar(
         env="GIT_COMMIT_AUTHOR", default=DEFAULT_COMMIT_AUTHOR
     )
     commit_message: str = COMMIT_MESSAGE
@@ -213,15 +213,15 @@
     _mask_attrs_: ClassVar[List[str]] = ["hvcs_client.token"]
 
     repo: Repo
     commit_parser: CommitParser[ParseResult, ParserOptions]
     version_translator: VersionTranslator
     major_on_zero: bool
     prerelease: bool
-    assets: Tuple[str, ...]
+    assets: List[str]
     commit_author: Actor
     commit_message: str
     changelog_excluded_commit_patterns: Tuple[re.Pattern[str], ...]
     version_declarations: Tuple[VersionDeclarationABC, ...]
     hvcs_client: HvcsBase
     changelog_file: Path
     ignore_token_for_push: bool
```

### Comparing `python-semantic-release-8.0.0a7/semantic_release/cli/github_actions_output.py` & `python-semantic-release-8.0.0a8/semantic_release/cli/github_actions_output.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/cli/masking_filter.py` & `python-semantic-release-8.0.0a8/semantic_release/cli/masking_filter.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/cli/util.py` & `python-semantic-release-8.0.0a8/semantic_release/cli/util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/commit_parser/__init__.py` & `python-semantic-release-8.0.0a8/semantic_release/commit_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/commit_parser/_base.py` & `python-semantic-release-8.0.0a8/semantic_release/commit_parser/_base.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/commit_parser/angular.py` & `python-semantic-release-8.0.0a8/semantic_release/commit_parser/angular.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/commit_parser/emoji.py` & `python-semantic-release-8.0.0a8/semantic_release/commit_parser/emoji.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/commit_parser/scipy.py` & `python-semantic-release-8.0.0a8/semantic_release/commit_parser/scipy.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/commit_parser/tag.py` & `python-semantic-release-8.0.0a8/semantic_release/commit_parser/tag.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/commit_parser/token.py` & `python-semantic-release-8.0.0a8/semantic_release/commit_parser/token.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/commit_parser/util.py` & `python-semantic-release-8.0.0a8/semantic_release/commit_parser/util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/const.py` & `python-semantic-release-8.0.0a8/semantic_release/const.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/data/templates/CHANGELOG.md.j2` & `python-semantic-release-8.0.0a8/semantic_release/data/templates/CHANGELOG.md.j2`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/enums.py` & `python-semantic-release-8.0.0a8/semantic_release/enums.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/errors.py` & `python-semantic-release-8.0.0a8/semantic_release/errors.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/helpers.py` & `python-semantic-release-8.0.0a8/semantic_release/helpers.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/hvcs/_base.py` & `python-semantic-release-8.0.0a8/semantic_release/hvcs/_base.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/hvcs/gitea.py` & `python-semantic-release-8.0.0a8/semantic_release/hvcs/gitea.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/hvcs/github.py` & `python-semantic-release-8.0.0a8/semantic_release/hvcs/github.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/hvcs/gitlab.py` & `python-semantic-release-8.0.0a8/semantic_release/hvcs/gitlab.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/hvcs/token_auth.py` & `python-semantic-release-8.0.0a8/semantic_release/hvcs/token_auth.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/hvcs/util.py` & `python-semantic-release-8.0.0a8/semantic_release/hvcs/util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/version/algorithm.py` & `python-semantic-release-8.0.0a8/semantic_release/version/algorithm.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/version/declaration.py` & `python-semantic-release-8.0.0a8/semantic_release/version/declaration.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/version/translator.py` & `python-semantic-release-8.0.0a8/semantic_release/version/translator.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/semantic_release/version/version.py` & `python-semantic-release-8.0.0a8/semantic_release/version/version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/tests/command_line/test_changelog.py` & `python-semantic-release-8.0.0a8/tests/command_line/test_changelog.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 ):
     tempdir = tmp_path_factory.mktemp("test_changelog")
     shutil.rmtree(str(tempdir.resolve()))
     shutil.copytree(src=str(example_project.resolve()), dst=tempdir)
 
     result = cli_runner.invoke(main, [changelog.name, *args])
     assert result.exit_code == 2
-    assert "not in release history" in result.output.lower()
+    assert "not in release history" in result.stderr.lower()
 
 
 @pytest.mark.usefixtures("repo_with_single_branch_and_prereleases_angular_commits")
 @pytest.mark.parametrize("args", [("--post-to-release-tag", "v0.1.0")])
 def test_changelog_post_to_release(
     args, monkeypatch, tmp_path_factory, example_project, cli_runner
 ):
```

### Comparing `python-semantic-release-8.0.0a7/tests/command_line/test_generate_config.py` & `python-semantic-release-8.0.0a8/tests/command_line/test_generate_config.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/tests/command_line/test_help.py` & `python-semantic-release-8.0.0a8/tests/command_line/test_help.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/tests/command_line/test_main.py` & `python-semantic-release-8.0.0a8/tests/command_line/test_main.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/tests/command_line/test_publish.py` & `python-semantic-release-8.0.0a8/tests/command_line/test_publish.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/tests/command_line/test_version.py` & `python-semantic-release-8.0.0a8/tests/command_line/test_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,15 @@
 
     tags_after = sorted(list(repo.tags), key=lambda tag: tag.name)
     head_after = repo.head.commit
 
     assert result.exit_code == 0
     assert tags_before == tags_after
     assert head_before == head_after
-    assert result.output.rstrip("\n") == expected_stdout
+    assert result.stdout.rstrip("\n") == expected_stdout
     dcmp = filecmp.dircmp(str(example_project.resolve()), tempdir)
     differing_files = flatten_dircmp(dcmp)
     assert not differing_files
 
 
 @pytest.mark.parametrize(
     "repo",
@@ -237,15 +237,15 @@
 )
 def test_version_already_released_no_push(repo, cli_runner):
     # In these tests, unless arguments are supplied then the latest version
     # has already been released, so we expect an exit code of 2 with the message
     # to indicate that no release will be made
     result = cli_runner.invoke(main, ["--strict", version.name, "--no-push"])
     assert result.exit_code == 2
-    assert "no release will be made" in result.output.lower()
+    assert "no release will be made" in result.stderr.lower()
 
 
 @pytest.mark.parametrize(
     "repo, cli_args, expected_new_version",
     [
         *[
             (
@@ -451,24 +451,33 @@
 )
 def test_version_build_metadata_triggers_new_version(repo, cli_runner):
     # Verify we get "no version to release" without build metadata
     no_metadata_result = cli_runner.invoke(
         main, ["--strict", version.name, "--no-push"]
     )
     assert no_metadata_result.exit_code == 2
-    assert "no release will be made" in no_metadata_result.output.lower()
+    assert "no release will be made" in no_metadata_result.stderr.lower()
 
     metadata_suffix = "build.abc-12345"
     result = cli_runner.invoke(
         main, [version.name, "--no-push", "--build-metadata", metadata_suffix]
     )
     assert result.exit_code == 0
     assert repo.git.tag(l=f"*{metadata_suffix}")
 
 
+def test_version_prints_current_version_if_no_new_version(
+    repo_with_git_flow_angular_commits, cli_runner
+):
+    result = cli_runner.invoke(main, [version.name, "--no-push"])
+    assert result.exit_code == 0
+    assert "no release will be made" in result.stderr.lower()
+    assert result.stdout == "1.2.0-alpha.2\n"
+
+
 @pytest.mark.parametrize("shell", ("/usr/bin/bash", "/usr/bin/zsh", "powershell"))
 def test_version_runs_build_command(
     repo_with_git_flow_angular_commits, cli_runner, example_pyproject_toml, shell
 ):
     config = tomlkit.loads(example_pyproject_toml.read_text(encoding="utf-8"))
     build_command = config["tool"]["semantic_release"]["build_command"]
     exe = shell.split("/")[-1]
```

### Comparing `python-semantic-release-8.0.0a7/tests/fixtures/commit_parsers.py` & `python-semantic-release-8.0.0a8/tests/fixtures/commit_parsers.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/tests/fixtures/example_project.py` & `python-semantic-release-8.0.0a8/tests/fixtures/example_project.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/tests/fixtures/git_repo.py` & `python-semantic-release-8.0.0a8/tests/fixtures/git_repo.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/tests/fixtures/scipy.py` & `python-semantic-release-8.0.0a8/tests/fixtures/scipy.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/tests/scenario/test_next_version.py` & `python-semantic-release-8.0.0a8/tests/scenario/test_next_version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/tests/scenario/test_release_history.py` & `python-semantic-release-8.0.0a8/tests/scenario/test_release_history.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/tests/scenario/test_template_render.py` & `python-semantic-release-8.0.0a8/tests/scenario/test_template_render.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/tests/unit/semantic_release/changelog/test_changelog_context.py` & `python-semantic-release-8.0.0a8/tests/unit/semantic_release/changelog/test_changelog_context.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/tests/unit/semantic_release/changelog/test_default_changelog.py` & `python-semantic-release-8.0.0a8/tests/unit/semantic_release/changelog/test_default_changelog.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/tests/unit/semantic_release/changelog/test_release_notes.py` & `python-semantic-release-8.0.0a8/tests/unit/semantic_release/changelog/test_release_notes.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/tests/unit/semantic_release/changelog/test_template.py` & `python-semantic-release-8.0.0a8/tests/unit/semantic_release/changelog/test_template.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/tests/unit/semantic_release/cli/test_config.py` & `python-semantic-release-8.0.0a8/tests/unit/semantic_release/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/tests/unit/semantic_release/cli/test_github_actions_output.py` & `python-semantic-release-8.0.0a8/tests/unit/semantic_release/cli/test_github_actions_output.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/tests/unit/semantic_release/cli/test_masking_filter.py` & `python-semantic-release-8.0.0a8/tests/unit/semantic_release/cli/test_masking_filter.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/tests/unit/semantic_release/cli/test_version.py` & `python-semantic-release-8.0.0a8/tests/unit/semantic_release/cli/test_version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/tests/unit/semantic_release/commit_parser/test_angular.py` & `python-semantic-release-8.0.0a8/tests/unit/semantic_release/commit_parser/test_angular.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/tests/unit/semantic_release/commit_parser/test_emoji.py` & `python-semantic-release-8.0.0a8/tests/unit/semantic_release/commit_parser/test_emoji.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/tests/unit/semantic_release/commit_parser/test_tag.py` & `python-semantic-release-8.0.0a8/tests/unit/semantic_release/commit_parser/test_tag.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/tests/unit/semantic_release/commit_parser/test_token.py` & `python-semantic-release-8.0.0a8/tests/unit/semantic_release/commit_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/tests/unit/semantic_release/hvcs/test__base.py` & `python-semantic-release-8.0.0a8/tests/unit/semantic_release/hvcs/test__base.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/tests/unit/semantic_release/hvcs/test_gitea.py` & `python-semantic-release-8.0.0a8/tests/unit/semantic_release/hvcs/test_gitea.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/tests/unit/semantic_release/hvcs/test_github.py` & `python-semantic-release-8.0.0a8/tests/unit/semantic_release/hvcs/test_github.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/tests/unit/semantic_release/hvcs/test_gitlab.py` & `python-semantic-release-8.0.0a8/tests/unit/semantic_release/hvcs/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/tests/unit/semantic_release/hvcs/test_token_auth.py` & `python-semantic-release-8.0.0a8/tests/unit/semantic_release/hvcs/test_token_auth.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/tests/unit/semantic_release/version/test_algorithm.py` & `python-semantic-release-8.0.0a8/tests/unit/semantic_release/version/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/tests/unit/semantic_release/version/test_declaration.py` & `python-semantic-release-8.0.0a8/tests/unit/semantic_release/version/test_declaration.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/tests/unit/semantic_release/version/test_translator.py` & `python-semantic-release-8.0.0a8/tests/unit/semantic_release/version/test_translator.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a7/tests/unit/semantic_release/version/test_version.py` & `python-semantic-release-8.0.0a8/tests/unit/semantic_release/version/test_version.py`

 * *Files identical despite different names*

