# Comparing `tmp/octomachinery-0.3.6.tar.gz` & `tmp/octomachinery-0.3.6.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octomachinery-0.3.6.tar", last modified: Thu Apr  1 00:07:52 2021, max compression
+gzip compressed data, was "octomachinery-0.3.6.post0.tar", last modified: Sat Jun 17 11:55:55 2023, max compression
```

## Comparing `octomachinery-0.3.6.tar` & `octomachinery-0.3.6.post0.tar`

### file list

```diff
@@ -1,120 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 00:07:52.598179 octomachinery-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2021-04-01 00:07:28.000000 octomachinery-0.3.6/.docs-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2021-04-01 00:07:28.000000 octomachinery-0.3.6/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (121)      131 2021-04-01 00:07:28.000000 octomachinery-0.3.6/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 00:07:52.594179 octomachinery-0.3.6/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      268 2021-04-01 00:07:28.000000 octomachinery-0.3.6/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 00:07:52.594179 octomachinery-0.3.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1018 2021-04-01 00:07:28.000000 octomachinery-0.3.6/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (121)     4814 2021-04-01 00:07:28.000000 octomachinery-0.3.6/.github/workflows/python-tox.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1275 2021-04-01 00:07:28.000000 octomachinery-0.3.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1392 2021-04-01 00:07:28.000000 octomachinery-0.3.6/.pre-commit-config.ci.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1377 2021-04-01 00:07:28.000000 octomachinery-0.3.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    17628 2021-04-01 00:07:28.000000 octomachinery-0.3.6/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      229 2021-04-01 00:07:28.000000 octomachinery-0.3.6/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2021-04-01 00:07:28.000000 octomachinery-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6747 2021-04-01 00:07:52.598179 octomachinery-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3510 2021-04-01 00:07:28.000000 octomachinery-0.3.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 00:07:52.594179 octomachinery-0.3.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 00:07:52.594179 octomachinery-0.3.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     1389 2021-04-01 00:07:28.000000 octomachinery-0.3.6/docs/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 00:07:52.594179 octomachinery-0.3.6/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)      218 2021-04-01 00:07:28.000000 octomachinery-0.3.6/docs/_templates/github-sponsors.html
--rw-r--r--   0 runner    (1001) docker     (121)      163 2021-04-01 00:07:28.000000 octomachinery-0.3.6/docs/_templates/project-description.html
--rw-r--r--   0 runner    (1001) docker     (121)     9422 2021-04-01 00:07:28.000000 octomachinery-0.3.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2021-04-01 00:07:28.000000 octomachinery-0.3.6/docs/getting-started.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5538 2021-04-01 00:07:28.000000 octomachinery-0.3.6/docs/howto-guides.rst
--rw-r--r--   0 runner    (1001) docker     (121)      776 2021-04-01 00:07:28.000000 octomachinery-0.3.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      230 2021-04-01 00:07:28.000000 octomachinery-0.3.6/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 00:07:52.586180 octomachinery-0.3.6/octomachinery/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 00:07:52.586180 octomachinery-0.3.6/octomachinery/app/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 00:07:52.586180 octomachinery-0.3.6/octomachinery/app/action/
--rw-r--r--   0 runner    (1001) docker     (121)     1129 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/app/action/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2636 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/app/action/runner.py
--rw-r--r--   0 runner    (1001) docker     (121)     2245 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/app/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 00:07:52.586180 octomachinery-0.3.6/octomachinery/app/routing/
--rw-r--r--   0 runner    (1001) docker     (121)      219 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/app/routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/app/routing/abc.py
--rw-r--r--   0 runner    (1001) docker     (121)      161 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/app/routing/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)      218 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/app/routing/routers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4661 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/app/routing/webhooks_dispatcher.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 00:07:52.586180 octomachinery-0.3.6/octomachinery/app/runtime/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/app/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      596 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/app/runtime/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      152 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/app/runtime/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     3129 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/app/runtime/installation_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      819 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/app/runtime/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 00:07:52.586180 octomachinery-0.3.6/octomachinery/app/server/
--rw-r--r--   0 runner    (1001) docker     (121)      274 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/app/server/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     4229 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/app/server/machinery.py
--rw-r--r--   0 runner    (1001) docker     (121)     2194 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/app/server/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 00:07:52.586180 octomachinery-0.3.6/octomachinery/cli/
--rw-r--r--   0 runner    (1001) docker     (121)     6331 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/cli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 00:07:52.582179 octomachinery-0.3.6/octomachinery/github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 00:07:52.586180 octomachinery-0.3.6/octomachinery/github/api/
--rw-r--r--   0 runner    (1001) docker     (121)     4929 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/github/api/app_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2749 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/github/api/raw_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1146 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/github/api/tokens.py
--rw-r--r--   0 runner    (1001) docker     (121)     2338 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/github/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 00:07:52.586180 octomachinery-0.3.6/octomachinery/github/config/
--rw-r--r--   0 runner    (1001) docker     (121)     2477 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/github/config/app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 00:07:52.586180 octomachinery-0.3.6/octomachinery/github/entities/
--rw-r--r--   0 runner    (1001) docker     (121)     1772 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/github/entities/action.py
--rw-r--r--   0 runner    (1001) docker     (121)     2100 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/github/entities/app_installation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 00:07:52.586180 octomachinery-0.3.6/octomachinery/github/errors/
--rw-r--r--   0 runner    (1001) docker     (121)      554 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/github/errors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 00:07:52.590180 octomachinery-0.3.6/octomachinery/github/models/
--rw-r--r--   0 runner    (1001) docker     (121)     3544 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/github/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      604 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/github/models/_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     1973 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/github/models/action_outcomes.py
--rw-r--r--   0 runner    (1001) docker     (121)     7853 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/github/models/checks_api_requests.py
--rw-r--r--   0 runner    (1001) docker     (121)     9120 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/github/models/events.py
--rw-r--r--   0 runner    (1001) docker     (121)     4647 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/github/models/private_key.py
--rw-r--r--   0 runner    (1001) docker     (121)     1847 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/github/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 00:07:52.590180 octomachinery-0.3.6/octomachinery/github/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     4189 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/github/utils/event_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 00:07:52.590180 octomachinery-0.3.6/octomachinery/routing/
--rw-r--r--   0 runner    (1001) docker     (121)      204 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1010 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/routing/abc.py
--rw-r--r--   0 runner    (1001) docker     (121)      569 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/routing/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/routing/default_router.py
--rw-r--r--   0 runner    (1001) docker     (121)     3406 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/routing/routers.py
--rw-r--r--   0 runner    (1001) docker     (121)     5354 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/routing/webhooks_dispatcher.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 00:07:52.590180 octomachinery-0.3.6/octomachinery/runtime/
--rw-r--r--   0 runner    (1001) docker     (121)      587 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/runtime/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1707 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/runtime/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 00:07:52.590180 octomachinery-0.3.6/octomachinery/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     2727 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/utils/asynctools.py
--rw-r--r--   0 runner    (1001) docker     (121)     1097 2021-04-01 00:07:28.000000 octomachinery-0.3.6/octomachinery/utils/versiontools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 00:07:52.594179 octomachinery-0.3.6/octomachinery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6747 2021-04-01 00:07:52.000000 octomachinery-0.3.6/octomachinery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4856 2021-04-01 00:07:52.000000 octomachinery-0.3.6/octomachinery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-01 00:07:52.000000 octomachinery-0.3.6/octomachinery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      233 2021-04-01 00:07:52.000000 octomachinery-0.3.6/octomachinery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2021-04-01 00:07:52.000000 octomachinery-0.3.6/octomachinery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-01 00:07:52.000000 octomachinery-0.3.6/octomachinery.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      176 2021-04-01 00:07:28.000000 octomachinery-0.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      925 2021-04-01 00:07:28.000000 octomachinery-0.3.6/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     2755 2021-04-01 00:07:52.598179 octomachinery-0.3.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 00:07:52.590180 octomachinery-0.3.6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 00:07:52.582179 octomachinery-0.3.6/tests/app/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 00:07:52.590180 octomachinery-0.3.6/tests/app/action/
--rw-r--r--   0 runner    (1001) docker     (121)     3241 2021-04-01 00:07:28.000000 octomachinery-0.3.6/tests/app/action/runner_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 00:07:52.590180 octomachinery-0.3.6/tests/app/routing/
--rw-r--r--   0 runner    (1001) docker     (121)     1135 2021-04-01 00:07:28.000000 octomachinery-0.3.6/tests/app/routing/decorators_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 00:07:52.590180 octomachinery-0.3.6/tests/app/server/
--rw-r--r--   0 runner    (1001) docker     (121)     4511 2021-04-01 00:07:28.000000 octomachinery-0.3.6/tests/app/server/machinery_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2971 2021-04-01 00:07:28.000000 octomachinery-0.3.6/tests/circular_imports_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1034 2021-04-01 00:07:28.000000 octomachinery-0.3.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 00:07:52.582179 octomachinery-0.3.6/tests/github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 00:07:52.590180 octomachinery-0.3.6/tests/github/models/
--rw-r--r--   0 runner    (1001) docker     (121)     3785 2021-04-01 00:07:28.000000 octomachinery-0.3.6/tests/github/models/private_key_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3986 2021-04-01 00:07:28.000000 octomachinery-0.3.6/tests/github/models/utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 00:07:52.594179 octomachinery-0.3.6/tests/github/utils/
--rw-r--r--   0 runner    (1001) docker     (121)    11821 2021-04-01 00:07:28.000000 octomachinery-0.3.6/tests/github/utils/event_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 00:07:52.594179 octomachinery-0.3.6/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     2068 2021-04-01 00:07:28.000000 octomachinery-0.3.6/tests/utils/asynctools_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     4297 2021-04-01 00:07:28.000000 octomachinery-0.3.6/tests/utils/versiontools_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     5556 2021-04-01 00:07:28.000000 octomachinery-0.3.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.441181 octomachinery-0.3.6.post0/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/.docs-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/.github/deadpendency.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)    24092 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/.github/workflows/ci-cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-06-17 11:55:55.441181 octomachinery-0.3.6.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.441181 octomachinery-0.3.6.post0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.441181 octomachinery-0.3.6.post0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/docs/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.441181 octomachinery-0.3.6.post0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/docs/_templates/github-sponsors.html
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/docs/_templates/project-description.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9423 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/docs/getting-started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/docs/howto-guides.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.433181 octomachinery-0.3.6.post0/octomachinery/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.433181 octomachinery-0.3.6.post0/octomachinery/app/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.433181 octomachinery-0.3.6.post0/octomachinery/app/action/
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/app/action/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/app/action/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/app/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.433181 octomachinery-0.3.6.post0/octomachinery/app/routing/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/app/routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/app/routing/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/app/routing/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/app/routing/routers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/app/routing/webhooks_dispatcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.433181 octomachinery-0.3.6.post0/octomachinery/app/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/app/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/app/runtime/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/app/runtime/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/app/runtime/installation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/app/runtime/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.433181 octomachinery-0.3.6.post0/octomachinery/app/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/app/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/app/server/machinery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/app/server/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.433181 octomachinery-0.3.6.post0/octomachinery/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/cli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.421181 octomachinery-0.3.6.post0/octomachinery/github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/octomachinery/github/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/github/api/app_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/github/api/raw_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/github/api/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/github/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/octomachinery/github/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/github/config/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/octomachinery/github/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/github/entities/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/github/entities/app_installation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/octomachinery/github/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/github/errors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/octomachinery/github/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/github/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/github/models/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/github/models/action_outcomes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/github/models/checks_api_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/github/models/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/github/models/private_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/github/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/octomachinery/github/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/github/utils/event_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/octomachinery/routing/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/routing/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/routing/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/routing/default_router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/routing/routers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/routing/webhooks_dispatcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/octomachinery/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/runtime/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/runtime/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/octomachinery/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/utils/asynctools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/utils/versiontools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.441181 octomachinery-0.3.6.post0/octomachinery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-06-17 11:55:55.000000 octomachinery-0.3.6.post0/octomachinery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-06-17 11:55:55.000000 octomachinery-0.3.6.post0/octomachinery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 11:55:55.000000 octomachinery-0.3.6.post0/octomachinery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-17 11:55:55.000000 octomachinery-0.3.6.post0/octomachinery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-17 11:55:55.000000 octomachinery-0.3.6.post0/octomachinery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 11:55:55.000000 octomachinery-0.3.6.post0/octomachinery.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-06-17 11:55:55.441181 octomachinery-0.3.6.post0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.421181 octomachinery-0.3.6.post0/tests/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/tests/app/action/
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/tests/app/action/runner_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/tests/app/routing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/tests/app/routing/decorators_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/tests/app/server/
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/tests/app/server/machinery_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/tests/circular_imports_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.425181 octomachinery-0.3.6.post0/tests/github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/tests/github/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/tests/github/models/private_key_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/tests/github/models/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/tests/github/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    11810 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/tests/github/utils/event_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/tests/utils/asynctools_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/tests/utils/versiontools_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/tox.ini
```

### Comparing `octomachinery-0.3.6/.github/workflows/publish-to-test-pypi.yml` & `octomachinery-0.3.6.post0/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6/.gitignore` & `octomachinery-0.3.6.post0/.gitignore`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6/.pylintrc` & `octomachinery-0.3.6.post0/.pylintrc`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6/LICENSE` & `octomachinery-0.3.6.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6/PKG-INFO` & `octomachinery-0.3.6.post0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,127 +1,23 @@
 Metadata-Version: 2.1
 Name: octomachinery
-Version: 0.3.6
+Version: 0.3.6.post0
 Summary: Invisible engine driving octobot machines. Simple, yet powerful.
 Home-page: https://octomachinery.dev
 Author: Sviatoslav Sydorenko (@webknjaz)
 Author-email: wk+octomachinery@sydorenko.org.ua
 License: GPLv3+
-Project-URL: Bug Tracker, https://github.com/sanitizers/octomachinery/issues
+Project-URL: Chat: Matrix, https://matrix.to/#/#octomachinery:matrix.org
+Project-URL: Chat: Matrix (PyBA), https://matrix.to/#/#pyba:matrix.org
+Project-URL: Chat: Matrix (@webknjaz), https://matrix.to/#/@webknjaz:matrix.org
 Project-URL: CI: GitHub, https://github.com/sanitizers/octomachinery/actions?workflow=Build/Test/Publish
-Project-URL: Documentation, https://docs.octomachinery.dev
-Project-URL: Source Code, https://github.com/sanitizers/octomachinery
-Description: .. image:: https://img.shields.io/pypi/v/octomachinery.svg?logo=Python&logoColor=white
-           :target: https://pypi.org/project/octomachinery
-           :alt: octomachinery @ PyPI
-        
-        .. image:: https://tidelift.com/badges/package/pypi/octomachinery
-           :target: https://tidelift.com/subscription/pkg/pypi-octomachinery?utm_source=pypi-octomachinery&utm_medium=readme
-           :alt: octomachinery is available as part of the Tidelift Subscription
-        
-        .. image:: https://github.com/sanitizers/octomachinery/workflows/Build%2FTest%2FPublish/badge.svg
-           :target: https://github.com/sanitizers/octomachinery/actions?workflow=Build%2FTest%2FPublish
-           :alt: GitHub Actions CI/CD build status — Python package
-        
-        .. DO-NOT-REMOVE-docs-badges-END
-        
-        .. image:: https://img.shields.io/readthedocs/octomachinery/latest.svg?logo=Read%20The%20Docs&logoColor=white
-           :target: https://docs.octomachinery.dev/en/latest/?badge=latest
-           :alt: Documentation Status
-        
-        octomachinery: Bots Without Boilerplate
-        =======================================
-        
-        Invisible engine driving octobot machines. Simple, yet powerful.
-        
-        Web-site @ https://octomachinery.dev. Stay tuned!
-        
-        .. DO-NOT-REMOVE-docs-intro-START
-        
-        **How-to create a GitHub Bot tutorial** is ready for preview
-        @ `tutorial.octomachinery.dev
-        <https://tutorial.octomachinery.dev/en/latest/>`_
-        
-        Elevator pitch
-        --------------
-        
-        Here's how you 👍 a just-created comment:
-        
-        .. code:: python
-        
-            from octomachinery.app.server.runner import run as run_app
-            from octomachinery.routing import process_event_actions
-            from octomachinery.routing.decorators import process_webhook_payload
-            from octomachinery.runtime.context import RUNTIME_CONTEXT
-        
-        
-            @process_event_actions('issue_comment', {'created'})
-            @process_webhook_payload
-            async def on_comment(
-                    *,
-                    action, issue, comment,
-                    repository=None, sender=None,
-                    installation=None,
-                    assignee=None, changes=None,
-            ):
-                github_api = RUNTIME_CONTEXT.app_installation_client
-                comment_reactions_api_url = f'{comment["url"]}/reactions'
-                await github_api.post(
-                    comment_reactions_api_url,
-                    preview_api_version='squirrel-girl',
-                    data={'content': '+1'},
-                )
-        
-        
-            run_app(
-                name='Thumbs-Up-Bot',
-                version='1.0.0',
-                url='https://github.com/apps/thuuuuuuuuuuuuuumbs-uuuuuuuuuuuup',
-            )
-        
-        Prerequisites
-        -------------
-        
-        Python 3.7+
-        
-        Contribute octomachinery
-        ------------------------
-        
-        **Want to add something to upstream?** Feel free to submit a PR or file
-        an issue if unsure.
-        Note that PR is more likely to be accepted if it includes tests and
-        detailed description helping maintainers to understand it better 🎉
-        
-        Oh, and be pythonic, please 🐍
-        
-        **Don't know how?** Check out `How to Contribute to Open Source
-        <https://opensource.guide/how-to-contribute/>`_ article by GitHub 🚀
-        
-        License
-        -------
-        
-        The source code and the documentation in this project are released under
-        the `GPL v3 license`_.
-        
-        .. _`GPL v3 license`:
-           https://github.com/sanitizers/octomachinery/blob/master/LICENSE
-        
-        For Enterprise
-        --------------
-        
-        octomachinery is available as part of the Tidelift Subscription.
-        
-        The octomachinery maintainers and the maintainers of thousands of other packages
-        are working with Tidelift to deliver one enterprise subscription that covers
-        all of the open source you use.
-        
-        `Learn more <https://tidelift.com/subscription/pkg/pypi-octomachinery?utm_source=pypi-octomachinery&utm_medium=referral&utm_campaign=github>`_.
-        
+Project-URL: Docs: RTD, https://docs.octomachinery.dev
+Project-URL: GitHub: issues, https://github.com/sanitizers/octomachinery/issues
+Project-URL: GitHub: repo, https://github.com/sanitizers/octomachinery
 Keywords: Bot,Framework,Framework for writing GitHub Apps,GitHub,GitHub Actions,GitHub API,GitHub Apps,GitHub Checks API
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Environment :: Other Environment
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -148,7 +44,118 @@
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: testing
+License-File: LICENSE
+
+.. image:: https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/banner-direct.svg
+   :target: https://github.com/vshymanskyy/StandWithUkraine/blob/main/docs/README.md
+   :alt: SWUbanner
+
+.. image:: https://img.shields.io/pypi/v/octomachinery.svg?logo=Python&logoColor=white
+   :target: https://pypi.org/project/octomachinery
+   :alt: octomachinery @ PyPI
+
+.. image:: https://tidelift.com/badges/package/pypi/octomachinery
+   :target: https://tidelift.com/subscription/pkg/pypi-octomachinery?utm_source=pypi-octomachinery&utm_medium=readme
+   :alt: octomachinery is available as part of the Tidelift Subscription
+
+.. image:: https://github.com/sanitizers/octomachinery/workflows/Build%2FTest%2FPublish/badge.svg
+   :target: https://github.com/sanitizers/octomachinery/actions?workflow=Build%2FTest%2FPublish
+   :alt: GitHub Actions CI/CD build status — Python package
+
+.. DO-NOT-REMOVE-docs-badges-END
+
+.. image:: https://img.shields.io/readthedocs/octomachinery/latest.svg?logo=Read%20The%20Docs&logoColor=white
+   :target: https://docs.octomachinery.dev/en/latest/?badge=latest
+   :alt: Documentation Status
+
+octomachinery: Bots Without Boilerplate
+=======================================
+
+Invisible engine driving octobot machines. Simple, yet powerful.
+
+Web-site @ https://octomachinery.dev. Stay tuned!
+
+.. DO-NOT-REMOVE-docs-intro-START
+
+**How-to create a GitHub Bot tutorial** is ready for preview
+@ `tutorial.octomachinery.dev
+<https://tutorial.octomachinery.dev/en/latest/>`_
+
+Elevator pitch
+--------------
+
+Here's how you 👍 a just-created comment:
+
+.. code:: python
+
+    from octomachinery.app.server.runner import run as run_app
+    from octomachinery.routing import process_event_actions
+    from octomachinery.routing.decorators import process_webhook_payload
+    from octomachinery.runtime.context import RUNTIME_CONTEXT
+
+
+    @process_event_actions('issue_comment', {'created'})
+    @process_webhook_payload
+    async def on_comment(
+            *,
+            action, issue, comment,
+            repository=None, sender=None,
+            installation=None,
+            assignee=None, changes=None,
+    ):
+        github_api = RUNTIME_CONTEXT.app_installation_client
+        comment_reactions_api_url = f'{comment["url"]}/reactions'
+        await github_api.post(
+            comment_reactions_api_url,
+            preview_api_version='squirrel-girl',
+            data={'content': '+1'},
+        )
+
+
+    run_app(
+        name='Thumbs-Up-Bot',
+        version='1.0.0',
+        url='https://github.com/apps/thuuuuuuuuuuuuuumbs-uuuuuuuuuuuup',
+    )
+
+Prerequisites
+-------------
+
+Python 3.7+
+
+Contribute octomachinery
+------------------------
+
+**Want to add something to upstream?** Feel free to submit a PR or file
+an issue if unsure.
+Note that PR is more likely to be accepted if it includes tests and
+detailed description helping maintainers to understand it better 🎉
+
+Oh, and be pythonic, please 🐍
+
+**Don't know how?** Check out `How to Contribute to Open Source
+<https://opensource.guide/how-to-contribute/>`_ article by GitHub 🚀
+
+License
+-------
+
+The source code and the documentation in this project are released under
+the `GPL v3 license`_.
+
+.. _`GPL v3 license`:
+   https://github.com/sanitizers/octomachinery/blob/master/LICENSE
+
+For Enterprise
+--------------
+
+octomachinery is available as part of the Tidelift Subscription.
+
+The octomachinery maintainers and the maintainers of thousands of other packages
+are working with Tidelift to deliver one enterprise subscription that covers
+all of the open source you use.
+
+`Learn more <https://tidelift.com/subscription/pkg/pypi-octomachinery?utm_source=pypi-octomachinery&utm_medium=referral&utm_campaign=github>`_.
```

### Comparing `octomachinery-0.3.6/README.rst` & `octomachinery-0.3.6.post0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+.. image:: https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/banner-direct.svg
+   :target: https://github.com/vshymanskyy/StandWithUkraine/blob/main/docs/README.md
+   :alt: SWUbanner
+
 .. image:: https://img.shields.io/pypi/v/octomachinery.svg?logo=Python&logoColor=white
    :target: https://pypi.org/project/octomachinery
    :alt: octomachinery @ PyPI
 
 .. image:: https://tidelift.com/badges/package/pypi/octomachinery
    :target: https://tidelift.com/subscription/pkg/pypi-octomachinery?utm_source=pypi-octomachinery&utm_medium=readme
    :alt: octomachinery is available as part of the Tidelift Subscription
```

### Comparing `octomachinery-0.3.6/docs/_static/custom.css` & `octomachinery-0.3.6.post0/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6/docs/conf.py` & `octomachinery-0.3.6.post0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 This file does only contain a selection of the most common options. For a
 full list see the documentation:
 http://www.sphinx-doc.org/en/master/config
 """
 
 from email import message_from_string
 from itertools import chain
+
 import pkg_resources
 
 
 # -- Path setup --------------------------------------------------------------
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
```

### Comparing `octomachinery-0.3.6/docs/getting-started.rst` & `octomachinery-0.3.6.post0/docs/getting-started.rst`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6/docs/howto-guides.rst` & `octomachinery-0.3.6.post0/docs/howto-guides.rst`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6/docs/index.rst` & `octomachinery-0.3.6.post0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6/octomachinery/app/action/config.py` & `octomachinery-0.3.6.post0/octomachinery/app/action/config.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6/octomachinery/app/action/runner.py` & `octomachinery-0.3.6.post0/octomachinery/app/action/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # pylint: disable=relative-beyond-top-level
 from ...github.entities.action import GitHubAction
 # pylint: disable=relative-beyond-top-level
 from ...github.errors import GitHubActionError
 # pylint: disable=relative-beyond-top-level
 from ...github.models.action_outcomes import (
-    ActionSuccess, ActionNeutral, ActionFailure,
+    ActionFailure, ActionNeutral, ActionSuccess,
 )
 # pylint: disable=relative-beyond-top-level
 from ..config import BotAppConfig
 # pylint: disable=relative-beyond-top-level
 from ..routing import WEBHOOK_EVENTS_ROUTER
 # pylint: disable=relative-beyond-top-level
 from ..routing.abc import OctomachineryRouterBase
```

### Comparing `octomachinery-0.3.6/octomachinery/app/config.py` & `octomachinery-0.3.6.post0/octomachinery/app/config.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """GitHub App/bot configuration."""
 
-from functools import lru_cache
 import os
+from functools import lru_cache
 from typing import Optional
 
 import environ
 import envparse
 
 # pylint: disable=relative-beyond-top-level
 from ..github.config.app import GitHubAppIntegrationConfig
```

### Comparing `octomachinery-0.3.6/octomachinery/app/routing/webhooks_dispatcher.py` & `octomachinery-0.3.6.post0/octomachinery/app/routing/webhooks_dispatcher.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """GitHub webhook events dispatching logic."""
 
 import asyncio
-from functools import wraps
-from http import HTTPStatus
 import logging
 import typing
+from functools import wraps
+from http import HTTPStatus
 
 from aiohttp import web
 from gidgethub import BadRequest, ValidationFailure
 from gidgethub.sansio import validate_event as validate_webhook_payload
 
 # pylint: disable=relative-beyond-top-level,import-error
 from ...github.models.events import GidgetHubWebhookEvent
```

### Comparing `octomachinery-0.3.6/octomachinery/app/runtime/config.py` & `octomachinery-0.3.6.post0/octomachinery/app/runtime/config.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6/octomachinery/app/runtime/installation_utils.py` & `octomachinery-0.3.6.post0/octomachinery/app/runtime/installation_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Utility helpers for App/Action installations."""
 
+import typing
 from base64 import b64decode
 from http import HTTPStatus
 from io import StringIO
 from pathlib import Path
-import typing
 
 import gidgethub
+
 import yaml
 
 # pylint: disable=relative-beyond-top-level
 from ...runtime.context import RUNTIME_CONTEXT
 
 
 def _get_file_contents_from_fs(file_name: str) -> typing.Optional[str]:
```

### Comparing `octomachinery-0.3.6/octomachinery/app/runtime/utils.py` & `octomachinery-0.3.6.post0/octomachinery/app/runtime/utils.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6/octomachinery/app/server/machinery.py` & `octomachinery-0.3.6.post0/octomachinery/app/server/machinery.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Web-server constructors."""
 
 import functools
 import logging
 
 import anyio
-from aiohttp.client import ClientSession
 from aiohttp import web
+from aiohttp.client import ClientSession
 
 # pylint: disable=relative-beyond-top-level
 from ...github.api.app_client import GitHubApp
 # pylint: disable=relative-beyond-top-level
 from ...utils.asynctools import auto_cleanup_aio_tasks
 # pylint: disable=relative-beyond-top-level
 from ..routing.webhooks_dispatcher import route_github_webhook_event
```

### Comparing `octomachinery-0.3.6/octomachinery/app/server/runner.py` & `octomachinery-0.3.6.post0/octomachinery/app/server/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import logging
 import sys
 from typing import Iterable, Optional
 
 from aiohttp.web_runner import GracefulExit
 from anyio import run as run_until_complete
+
 import attr
 
 # pylint: disable=relative-beyond-top-level
 from ..config import BotAppConfig
 # pylint: disable=relative-beyond-top-level
 from ..routing import WEBHOOK_EVENTS_ROUTER
 # pylint: disable=relative-beyond-top-level
```

### Comparing `octomachinery-0.3.6/octomachinery/cli/__main__.py` & `octomachinery-0.3.6.post0/octomachinery/cli/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 #! /usr/bin/env python3
 """Octomachinery CLI entrypoint."""
 
 import asyncio
-from functools import wraps
 import importlib
-from io import TextIOWrapper
 import os
 import pathlib
-from typing import Any, Callable, Iterable, Iterator, Set
+from functools import wraps
+from io import TextIOWrapper
+from typing import (
+    Any, Callable, Dict, FrozenSet, Iterable, Iterator, Set, Union,
+)
 
 from aiohttp.client import ClientSession
+
 import click
 
 # pylint: disable=relative-beyond-top-level
 from ..app.config import BotAppConfig
 # pylint: disable=relative-beyond-top-level
 from ..app.routing.abc import OctomachineryRouterBase
 # pylint: disable=relative-beyond-top-level
 from ..app.routing.webhooks_dispatcher import route_github_event
 # pylint: disable=relative-beyond-top-level
 from ..github.api.app_client import GitHubApp
 # pylint: disable=relative-beyond-top-level
 from ..github.entities.action import GitHubAction
 # pylint: disable=relative-beyond-top-level
-from ..github.models.events import GitHubEvent
 # pylint: disable=relative-beyond-top-level
-from ..github.models.events import GitHubWebhookEvent
+from ..github.models.events import GitHubEvent, GitHubWebhookEvent
 
 
 @click.group()
 @click.pass_context
 def cli(ctx: click.Context) -> None:  # pylint: disable=unused-argument
     """Click CLI base."""
 
@@ -96,15 +98,19 @@
     except ValueError as val_err:
         ctx.fail(click.style(str(val_err), fg='red'))
 
     os.environ.update(get_extra_env_vars(gh_event, token, app, private_key))
 
     try:
         target_routers = set(
-            load_event_routers(entrypoint_module, event_routers),
+            load_event_routers(
+                entrypoint_module,
+                # pylint: disable=fixme
+                event_routers,  # type: ignore[arg-type]  # FIXME: typing
+            ),
         )
     except AttributeError as attr_err:
         ctx.fail(
             click.style(
                 f'Could not find an event router: {attr_err!s}',
                 fg='red',
             ),
@@ -119,15 +125,16 @@
     make_gh_app = GitHubApp
     if app is None:
         make_gh_app = GitHubAction
         gh_app_kwargs['metadata'] = config.action
     async with ClientSession() as http_client_session:
         github_app = make_gh_app(
             http_session=http_client_session,
-            event_routers=target_routers or None,
+            # FIXME: typing  # pylint: disable=fixme
+            event_routers=target_routers or None,  # type: ignore[arg-type]
             **gh_app_kwargs,
         )
         await route_github_event(
             github_event=gh_event, github_app=github_app,
         )
 
     click.echo(
@@ -136,30 +143,30 @@
             fg='green',
         ),
     )
 
 
 def load_event_routers(
         entrypoint_module: str = None,
-        event_routers: Set[str] = frozenset(),
+        event_routers: Union[FrozenSet[str], Set[str]] = frozenset(),
 ) -> Iterator[OctomachineryRouterBase]:
     """Yield event routers from strings."""
     if entrypoint_module is not None:
         importlib.import_module(entrypoint_module)
 
     for router_path in event_routers:
         target_sep = ':' if ':' in router_path else '.'
         module_path, _sep, target_router = router_path.rpartition(target_sep)
         yield getattr(importlib.import_module(module_path), target_router)
 
 
 def get_extra_env_vars(
         gh_event: GitHubEvent, token: str, app: int,
         private_key: TextIOWrapper,
-) -> dict:
+) -> Dict[str, str]:
     """Construct additional env vars for App or Action processing."""
     env = {}
 
     if app is not None:
         env['OCTOMACHINERY_APP_MODE'] = 'app'
 
         env['GITHUB_APP_IDENTIFIER'] = str(app)
```

### Comparing `octomachinery-0.3.6/octomachinery/github/api/app_client.py` & `octomachinery-0.3.6.post0/octomachinery/github/api/app_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 """GitHub App API client."""
 
 from __future__ import annotations
 
-from collections import defaultdict
 import logging
-from typing import Any, Iterable, TYPE_CHECKING
+from collections import defaultdict
+from typing import TYPE_CHECKING, Any, Dict, Iterable
 
 from aiohttp.client import ClientSession
 from aiohttp.client_exceptions import ClientConnectorError
+
 import attr
 import sentry_sdk
 
 # pylint: disable=relative-beyond-top-level
 from ...routing import WEBHOOK_EVENTS_ROUTER
-
 # pylint: disable=relative-beyond-top-level
-from ...utils.asynctools import (
-    amap, dict_to_kwargs_cb,
-)
+from ...utils.asynctools import amap, dict_to_kwargs_cb
 # pylint: disable=relative-beyond-top-level
 from ..config.app import GitHubAppIntegrationConfig
 # pylint: disable=relative-beyond-top-level
 from ..entities.app_installation import GitHubAppInstallation
 # pylint: disable=relative-beyond-top-level
 from ..models import GitHubAppInstallation as GitHubAppInstallationModel
 # pylint: disable=relative-beyond-top-level
 from ..models.events import GitHubEvent
 from .raw_client import RawGitHubAPI
 from .tokens import GitHubJWTToken
 
+
 if TYPE_CHECKING:
     # pylint: disable=relative-beyond-top-level
     from ...routing.abc import OctomachineryRouterBase
 
 
 logger = logging.getLogger(__name__)
 
@@ -53,15 +52,16 @@
 
     def __attrs_post_init__(self) -> None:  # pylint: disable=no-self-use
         """Initialize the Sentry SDK library."""
         # NOTE: Under the hood, it will set up the DSN from `SENTRY_DSN`
         # NOTE: env var. We don't need to care about it not existing as
         # NOTE: Sentry SDK helpers don't fail loudly and if not
         # NOTE: configured, it'll be ignored.
-        sentry_sdk.init()
+        # FIXME:  # pylint: disable=fixme
+        sentry_sdk.init()  # pylint: disable=abstract-class-instantiated
 
     async def dispatch_event(self, github_event: GitHubEvent) -> Iterable[Any]:
         """Dispatch ``github_event`` into the embedded routers."""
         return await github_event.dispatch_via(
             *self._event_routers,  # pylint: disable=not-an-iterable
         )
 
@@ -123,15 +123,17 @@
                 )),
             ),
             self,
         )
 
     async def get_installations(self):
         """Retrieve all installations with access tokens via API."""
-        installations = defaultdict(dict)
+        installations: Dict[
+                int, GitHubAppInstallation,
+        ] = defaultdict(dict)  # type: ignore[arg-type]
         async for install in amap(
                 dict_to_kwargs_cb(GitHubAppInstallationModel),
                 self.api_client.getiter(
                     '/app/installations',
                     preview_api_version='machine-man',
                 ),
         ):
```

### Comparing `octomachinery-0.3.6/octomachinery/github/api/raw_client.py` & `octomachinery-0.3.6.post0/octomachinery/github/api/raw_client.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from asyncio import iscoroutinefunction
 from typing import Any, Dict, Optional, Tuple
 
 from gidgethub.abc import JSON_CONTENT_TYPE
 from gidgethub.aiohttp import GitHubAPI
 
 # pylint: disable=relative-beyond-top-level
-from .tokens import GitHubToken, GitHubOAuthToken, GitHubJWTToken
+from .tokens import GitHubJWTToken, GitHubOAuthToken, GitHubToken
 from .utils import accept_preview_version, mark_uninitialized_in_repr
 
 
 @mark_uninitialized_in_repr
 class RawGitHubAPI(GitHubAPI):
     """A low-level GitHub API client with a pre-populated token."""
 
@@ -53,16 +53,18 @@
             self, method: str, url: str, url_vars: Dict[str, str],
             data: Any, accept: str = None,
             jwt: Optional[str] = None,
             oauth_token: Optional[str] = None,
             content_type: str = JSON_CONTENT_TYPE,
     ) -> Tuple[bytes, Optional[str]]:
         token = self._token
-        if iscoroutinefunction(token):
-            token = await token()
+        # pylint: disable=fixme
+        if iscoroutinefunction(token):  # type: ignore[arg-type]  # FIXME
+            # pylint: disable=fixme
+            token = await token()  # type: ignore[misc,operator]  # FIXME
         if isinstance(token, GitHubOAuthToken):
             oauth_token = str(token)
             jwt = None
         if isinstance(token, GitHubJWTToken):
             jwt = str(token)
             oauth_token = None
         return await super()._make_request(
```

### Comparing `octomachinery-0.3.6/octomachinery/github/api/tokens.py` & `octomachinery-0.3.6.post0/octomachinery/github/api/tokens.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6/octomachinery/github/api/utils.py` & `octomachinery-0.3.6.post0/octomachinery/github/api/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 
 def accept_preview_version(wrapped_coroutine):
     """Extend keyword-args with `preview_api_version`."""
     @wraps(wrapped_coroutine)
     def coroutine_wrapper(
             *args: Tuple[Any], **kwargs: Dict[str, Any]
-    ) -> AsyncGeneratorType:
+    ) -> AsyncGeneratorType:  # type: ignore[type-arg]
         accept_media = kwargs.pop('accept', None)
         preview_api_version = kwargs.pop('preview_api_version', None)
 
         if preview_api_version is not None:
             accept_media = accept_format(
                 version=f'{preview_api_version}-preview',
             )
@@ -60,12 +60,12 @@
         name='preview_api_version',
         annotation='Optional[str]',
         default=None,
         kind=Parameter.KEYWORD_ONLY,
     )
     wrapped_callable_params.insert(accept_pos, preview_param)
 
-    coroutine_wrapper.__signature__ = original_wrapped_signature.replace(
-        parameters=wrapped_callable_params,
+    coroutine_wrapper.__signature__ = (  # type: ignore[attr-defined]
+        original_wrapped_signature.replace(parameters=wrapped_callable_params)
     )
 
     return coroutine_wrapper
```

### Comparing `octomachinery-0.3.6/octomachinery/github/config/app.py` & `octomachinery-0.3.6.post0/octomachinery/github/config/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Config schema for a GitHub App instance details."""
 import environ
 
-
 # pylint: disable=relative-beyond-top-level
 from ..models.private_key import GitHubPrivateKey
 # pylint: disable=relative-beyond-top-level
 from ..models.utils import SecretStr
 
 
 def validate_is_not_none_if_app(
```

### Comparing `octomachinery-0.3.6/octomachinery/github/entities/action.py` & `octomachinery-0.3.6.post0/octomachinery/github/entities/action.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # pylint: disable=relative-beyond-top-level
 from ..api.raw_client import RawGitHubAPI
 # pylint: disable=relative-beyond-top-level
 from ..api.tokens import GitHubOAuthToken
 # pylint: disable=relative-beyond-top-level,import-error
 from ..models.events import GidgetHubActionEvent
 
+
 if typing.TYPE_CHECKING:
     # pylint: disable=relative-beyond-top-level
     from ...app.action.config import GitHubActionConfig
 
 
 logger = logging.getLogger(__name__)
```

### Comparing `octomachinery-0.3.6/octomachinery/github/entities/app_installation.py` & `octomachinery-0.3.6.post0/octomachinery/github/entities/app_installation.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,18 +8,16 @@
 import attr
 
 # pylint: disable=relative-beyond-top-level
 from ..api.raw_client import RawGitHubAPI
 # pylint: disable=relative-beyond-top-level
 from ..api.tokens import GitHubOAuthToken
 # pylint: disable=relative-beyond-top-level
-from ..models import (
-    GitHubAppInstallation as GitHubAppInstallationModel,
-    GitHubInstallationAccessToken,
-)
+from ..models import GitHubAppInstallation as GitHubAppInstallationModel
+from ..models import GitHubInstallationAccessToken
 
 
 if typing.TYPE_CHECKING:
     from ..api.app_client import GitHubApp
 
 
 logger = logging.getLogger(__name__)
@@ -61,13 +59,14 @@
 
         return GitHubOAuthToken(self._token.token)
 
     @property
     def api_client(self):  # noqa: D401
         """The GitHub App Installation client."""
         return RawGitHubAPI(
-            token=self._refresh_api_token,
+            # pylint: disable=fixme
+            token=self._refresh_api_token,  # type: ignore[arg-type]  # FIXME
             # pylint: disable=protected-access
             session=self.app._http_session,
             # pylint: disable=protected-access
             user_agent=self.app._config.user_agent,
         )
```

### Comparing `octomachinery-0.3.6/octomachinery/github/errors/__init__.py` & `octomachinery-0.3.6.post0/octomachinery/github/errors/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Exceptions collection related to interactions with GitHub."""
 
-import attr
 from gidgethub import GitHubException
 
+import attr
+
 # pylint: disable=relative-beyond-top-level
 from ..models.action_outcomes import ActionOutcome
 
 
 class GitHubError(GitHubException):
     """Generic GitHub-related error."""
```

### Comparing `octomachinery-0.3.6/octomachinery/github/models/__init__.py` & `octomachinery-0.3.6.post0/octomachinery/github/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Models representing objects in GitHub API."""
 
-from datetime import datetime, timezone
 import typing
+from datetime import datetime, timezone
 
 import attr
 
-from .utils import convert_datetime, SecretStr
+from .utils import SecretStr, convert_datetime
 
 
 @attr.dataclass
 class GitHubAppInstallation:  # pylint: disable=too-few-public-methods
     """
     Represents a GitHub App installed into a user or an organization profile.
```

### Comparing `octomachinery-0.3.6/octomachinery/github/models/_compat.py` & `octomachinery-0.3.6.post0/octomachinery/github/models/_compat.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Compatibility shims for the models subpackage."""
 from functools import wraps as _wraps_function
 
 from jwt import encode as _compute_jwt
+
+
 try:
     from jwt import __version__ as _pyjwt_version_str
 except ImportError:
     _pyjwt_version_str = '0.0.0'
 
 
 _pyjwt_version_info = tuple(map(int, _pyjwt_version_str.split('.')))
```

### Comparing `octomachinery-0.3.6/octomachinery/github/models/action_outcomes.py` & `octomachinery-0.3.6.post0/octomachinery/github/models/action_outcomes.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6/octomachinery/github/models/checks_api_requests.py` & `octomachinery-0.3.6.post0/octomachinery/github/models/checks_api_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
     """Checks API base check request mixin."""
 
     name: str = str_attrib()
     details_url: Optional[str] = optional_str_attrib()
     external_id: Optional[str] = optional_str_attrib()
     status: Optional[str] = attr.ib(
         default='queued',
-        validator=attr.validators.optional(
+        validator=attr.validators.optional(  # type: ignore[arg-type]
             attr.validators.in_(
                 (
                     'queued',
                     'in_progress',
                     'completed',
                 ),
             ),
```

### Comparing `octomachinery-0.3.6/octomachinery/github/models/events.py` & `octomachinery-0.3.6.post0/octomachinery/github/models/events.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """Generic GitHub event containers."""
 
 from __future__ import annotations
 
 import json
 import pathlib
-from typing import Any, Mapping, TextIO, TYPE_CHECKING, Union
 import uuid
 import warnings
+from typing import (
+    TYPE_CHECKING, Any, Iterable, Mapping, TextIO, Type, Union, cast,
+)
 
-import attr
 from gidgethub.sansio import Event as _GidgetHubEvent
 
+import attr
+
 # pylint: disable=relative-beyond-top-level
 from ...utils.asynctools import aio_gather
 # pylint: disable=relative-beyond-top-level
 from ..utils.event_utils import (
-    augment_http_headers,
-    parse_event_stub_from_fd,
-    validate_http_headers,
+    augment_http_headers, parse_event_stub_from_fd, validate_http_headers,
 )
 
+
 if TYPE_CHECKING:
     # pylint: disable=relative-beyond-top-level
     from ...app.routing.abc import OctomachineryRouterBase
 
 
 __all__ = 'GitHubEvent', 'GitHubWebhookEvent'
 
@@ -32,67 +34,69 @@
     """Return a UUID from the value."""
     if isinstance(value, uuid.UUID):
         return value
 
     return uuid.UUID(value, version=4)
 
 
-def _to_dict(value: Union[dict, bytes, str]) -> dict:
+def _to_dict(value: Union[Mapping[str, Any], bytes, str]) -> Mapping[str, Any]:
     """Return a dict from the value."""
     if isinstance(value, dict):
         return value
 
     if isinstance(value, bytes):
         value = value.decode()
 
-    return json.loads(value)
+    return json.loads(cast(str, value))
 
 
 @attr.dataclass(frozen=True)
 class GitHubEvent:
     """Representation of a generic source-agnostic GitHub event."""
 
     name: str
     """Event name."""
-    payload: dict = attr.ib(converter=_to_dict)
+    payload: Mapping[str, Any] = attr.ib(converter=_to_dict)
     """Event payload object."""
 
     # pylint: disable=no-self-use
     @payload.validator
-    def _is_payload_dict(self, attribute: str, value: dict) -> None:
+    def _is_payload_dict(
+            self, attribute: str, value: Mapping[str, Any],
+    ) -> None:
         """Verify that the attribute value is a dict.
 
         :raises ValueError: if it's not
         """
         if isinstance(value, dict):
             return
 
         raise ValueError(
             f'{value!r} is passed as {attribute!s} but it must '
             'be an instance of dict',
         )
 
     @classmethod
     def from_file(
-            cls: GitHubEvent,
+            cls: Type[GitHubEvent],
             event_name: str,
             event_path: Union[pathlib.Path, str],
     ) -> GitHubEvent:
         """Construct a GitHubEvent instance from event name and file."""
         # NOTE: This could be async but it probably doesn't matter
         # NOTE: since it's called just once during init and GitHub
         # NOTE: Action runtime only has one event to process
         # NOTE: OTOH it may slow-down tests parallelism
         # NOTE: so may deserve to be fixed
         with pathlib.Path(event_path).open() as event_source:
             return cls(event_name, json.load(event_source))
 
     @classmethod
     def from_fixture_fd(
-            cls: GitHubEvent,
+            cls: Type[GitHubEvent],
             event_fixture_fd: TextIO,
             *,
             event: str = None,
     ) -> GitHubEvent:
         """Make a GitHubEvent from a fixture fd and an optional name."""
         headers, payload = parse_event_stub_from_fd(event_fixture_fd)
         if event and 'x-github-event' in headers:
@@ -101,15 +105,15 @@
                 'or an event header in the fixture file',
             )
         event_name = event or headers['x-github-event']
         return cls(event_name, payload)
 
     @classmethod
     def from_fixture(
-            cls: GitHubEvent,
+            cls: Type[GitHubEvent],
             event_fixture_path: Union[pathlib.Path, str],
             *,
             event: str = None,
     ) -> GitHubEvent:
         """Make a GitHubEvent from a fixture and an optional name."""
         with pathlib.Path(event_fixture_path).open() as event_source:
             return cls.from_fixture_fd(event_source, event=event)
@@ -126,28 +130,27 @@
         """Produce GidgetHub Event from self."""
         return _GidgetHubEvent(
             data=self.payload,
             event=self.name,
             delivery_id=str(uuid.uuid4()),
         )
 
-    # pylint: disable=no-self-use
     async def dispatch_via(
             self,
             *routers: OctomachineryRouterBase,
             ctx: Mapping[str, Any] = None,
-    ) -> None:
+    ) -> Iterable[Any]:
         """Invoke this event handlers from different routers."""
         if not routers:
             raise ValueError('At least one router must be supplied')
 
         if ctx is None:
             ctx = {}
 
-        await aio_gather(*(
+        return await aio_gather(*(
             r.dispatch(self, **ctx)
             for r in routers
         ))
 
 
 @attr.dataclass(frozen=True)
 class GitHubWebhookEvent(GitHubEvent):
@@ -169,26 +172,26 @@
         raise ValueError(
             f'{value!r} is passed as {attribute!s} but it must '
             'be an instance of UUID v4',
         )
 
     @classmethod
     def from_file(
-            cls: GitHubWebhookEvent,
+            cls: Type[GitHubWebhookEvent],
             event_name: str,
             event_path: Union[pathlib.Path, str],
     ) -> GitHubWebhookEvent:
         """Explode when constructing from file."""
         raise RuntimeError(
             'Webhook event is not supposed to be constructed from a file',
         )
 
     @classmethod
     def from_fixture_fd(
-            cls: GitHubWebhookEvent,
+            cls: Type[GitHubWebhookEvent],
             event_fixture_fd: TextIO,
             *,
             event: str = None,
     ) -> GitHubWebhookEvent:
         """Make GitHubWebhookEvent from fixture fd and optional name."""
         headers, payload = parse_event_stub_from_fd(event_fixture_fd)
         if event and 'x-github-event' in headers:
@@ -204,26 +207,26 @@
             name=headers['x-github-event'],
             payload=payload,
             delivery_id=headers['x-github-delivery'],
         )
 
     @classmethod
     def from_fixture(
-            cls: GitHubWebhookEvent,
+            cls: Type[GitHubWebhookEvent],
             event_fixture_path: Union[pathlib.Path, str],
             *,
             event: str = None,
     ) -> GitHubWebhookEvent:
         """Make a GitHubWebhookEvent from fixture and optional name."""
         with pathlib.Path(event_fixture_path).open() as event_source:
             return cls.from_fixture_fd(event_source, event=event)
 
     @classmethod
     def from_http_request(
-            cls: GitHubWebhookEvent,
+            cls: Type[GitHubWebhookEvent],
             http_req_headers: Mapping[str, str],
             http_req_body: bytes,
     ):
         """Make a GitHubWebhookEvent from HTTP req headers and body."""
         return cls(
             name=http_req_headers['x-github-event'],
             payload=json.loads(http_req_body.decode()),
@@ -261,27 +264,29 @@
         warnings.warn(
             "Relying on GidgetHub's event class interfaces will be deprecated "
             "in the future releases. Please use 'payload' attribute to access "
             'the event name instead.',
             category=PendingDeprecationWarning,
             stacklevel=2,
         )
-        return self.payload
+        # pylint: disable=fixme
+        return self.payload  # type: ignore[attr-defined]  # FIXME
 
     @property
     def event(self):
         """Event name alias."""
         warnings.warn(
             "Relying on GidgetHub's event class interfaces will be deprecated "
             "in the future releases. Please use 'name' attribute to access "
             'the event name instead.',
             category=PendingDeprecationWarning,
             stacklevel=2,
         )
-        return self.name
+        # pylint: disable=fixme
+        return self.name  # type: ignore[attr-defined]  # FIXME
 
 
 class GidgetHubActionEvent(GidgetHubEventMixin, GitHubEvent):
     """GitHub Action event wrapper exposing GidgetHub attrs."""
 
 
 class GidgetHubWebhookEvent(GidgetHubEventMixin, GitHubWebhookEvent):
```

### Comparing `octomachinery-0.3.6/octomachinery/github/models/private_key.py` & `octomachinery-0.3.6.post0/octomachinery/github/models/private_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Private key container."""
 from hashlib import sha1 as compute_sha1_hash
 from pathlib import Path
 from time import time
 
 from cryptography.hazmat.backends import default_backend
-from cryptography.hazmat.primitives.serialization import Encoding, PublicFormat
-from cryptography.hazmat.primitives.serialization import load_pem_private_key
+from cryptography.hazmat.primitives.serialization import (
+    Encoding, PublicFormat, load_pem_private_key,
+)
 
 from ._compat import compute_jwt
 
 
 def extract_private_key_sha1_fingerprint(rsa_private_key):
     r"""Retrieve the private key SHA-1 fingerprint.
```

### Comparing `octomachinery-0.3.6/octomachinery/github/models/utils.py` & `octomachinery-0.3.6.post0/octomachinery/github/models/utils.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """A collection of utility functions helping with models."""
 
+import sys
 from datetime import datetime, timezone
 from functools import singledispatch
-import sys
 
 
 @singledispatch
 def convert_datetime(datetime_obj) -> datetime:
     """Convert arbitrary object into a datetime instance."""
     raise ValueError(
         f'The input arg type {type(datetime_obj)} is not supported',
```

### Comparing `octomachinery-0.3.6/octomachinery/github/utils/event_utils.py` & `octomachinery-0.3.6.post0/octomachinery/github/utils/event_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import contextlib
 import itertools
 import json
 from uuid import UUID, uuid4
 
 import multidict
+
 import yaml
 
 
 def _probe_yaml(event_file_fd):
     try:
         http_headers, event, extra = itertools.islice(
             itertools.chain(
```

### Comparing `octomachinery-0.3.6/octomachinery/routing/abc.py` & `octomachinery-0.3.6.post0/octomachinery/routing/abc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Octomachinery router base interface definitions."""
 
 from abc import ABCMeta
-from typing import Any, Iterator, TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Iterator
 
 from gidgethub.routing import AsyncCallback
 
+
 if TYPE_CHECKING:
     from ..github.models.events import GitHubEvent
 
 
 __all__ = ('OctomachineryRouterBase', )
```

### Comparing `octomachinery-0.3.6/octomachinery/routing/decorators.py` & `octomachinery-0.3.6.post0/octomachinery/routing/decorators.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Webhook event processing helper decorators."""
 
 from __future__ import annotations
 
 from functools import wraps
-from typing import Any, TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
+
 
 if TYPE_CHECKING:
     # pylint: disable=relative-beyond-top-level
     from ..github.models.events import GitHubEvent
 
 
 __all__ = ('process_webhook_payload', )
```

### Comparing `octomachinery-0.3.6/octomachinery/routing/default_router.py` & `octomachinery-0.3.6.post0/octomachinery/routing/default_router.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6/octomachinery/routing/routers.py` & `octomachinery-0.3.6.post0/octomachinery/routing/routers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Octomachinery event dispatchers collection."""
 
 import asyncio
 from contextlib import suppress
 from typing import Any, Iterator, Set, Union
 
-from gidgethub.routing import AsyncCallback, Router as _GidgetHubRouter
+from gidgethub.routing import AsyncCallback
+from gidgethub.routing import Router as _GidgetHubRouter
 
-from ..utils.asynctools import aio_gather
 from ..github.models.events import (
-    GidgetHubWebhookEvent, GitHubEvent,
-    _GidgetHubEvent,
+    GidgetHubWebhookEvent, GitHubEvent, _GidgetHubEvent,
 )
+from ..utils.asynctools import aio_gather
 from .abc import OctomachineryRouterBase
 
 
 __all__ = (
     'GidgetHubRouterBase',
     'ConcurrentRouter',
     'NonBlockingConcurrentRouter',
```

### Comparing `octomachinery-0.3.6/octomachinery/routing/webhooks_dispatcher.py` & `octomachinery-0.3.6.post0/octomachinery/routing/webhooks_dispatcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 """GitHub webhook events dispatching logic."""
 
 from __future__ import annotations
 
 import contextlib
 import logging
+from typing import Any, Iterable
+
+from anyio import get_cancelled_exc_class
+from anyio import sleep as async_sleep
 
-from anyio import get_cancelled_exc_class, sleep as async_sleep
 import sentry_sdk
 
 # pylint: disable=relative-beyond-top-level,import-error
-from ..runtime.context import RUNTIME_CONTEXT
-# pylint: disable=relative-beyond-top-level,import-error
 from ..github.api.app_client import GitHubApp
 # pylint: disable=relative-beyond-top-level,import-error
 from ..github.entities.action import GitHubAction
 # pylint: disable=relative-beyond-top-level,import-error
 from ..github.errors import GitHubActionError
 # pylint: disable=relative-beyond-top-level,import-error
 from ..github.models.events import GitHubEvent
+# pylint: disable=relative-beyond-top-level,import-error
+from ..runtime.context import RUNTIME_CONTEXT
 
 
 __all__ = ('route_github_event', )
 
 
 logger = logging.getLogger(__name__)
 
 
-async def route_github_event(
+# pylint: disable=fixme
+async def route_github_event(  # type: ignore[return]  # FIXME
         *,
         github_event: GitHubEvent,
         github_app: GitHubApp,
-) -> None:
+) -> Iterable[Any]:
     """Dispatch GitHub event to corresponsing handlers.
 
     Set up ``RUNTIME_CONTEXT`` before doing that. This is so
     the concrete event handlers have access to the API client
     and flags in runtime.
     """
     is_gh_action = isinstance(github_app, GitHubAction)
@@ -110,15 +114,17 @@
         logger.exception(
             'An unhandled exception happened while running webhook '
             'event handlers for "%s"...',
             github_event.name,
         )
         delivery_id_msg = (
             '' if is_gh_action
-            else f' (Delivery ID: {github_event.delivery_id!s})'
+            else ' (Delivery ID: '
+            # FIXME:  # pylint: disable=fixme
+            f'{github_event.delivery_id!s})'  # type: ignore[attr-defined]
         )
         logger.debug(
             'The payload of "%s" event%s is: %r',
             github_event.name, delivery_id_msg, github_event.payload,
         )
 
         if is_gh_action:
```

### Comparing `octomachinery-0.3.6/octomachinery/runtime/context.py` & `octomachinery-0.3.6.post0/octomachinery/runtime/context.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6/octomachinery/runtime/utils.py` & `octomachinery-0.3.6.post0/octomachinery/runtime/utils.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Runtime context helpers."""
 
 from __future__ import annotations
 
-from contextvars import ContextVar, Token
 import typing
+from contextvars import ContextVar, Token
 
 
 class ContextLookupError(AttributeError):
     """Context var lookup error."""
 
 
 class _ContextMap:
```

### Comparing `octomachinery-0.3.6/octomachinery/utils/asynctools.py` & `octomachinery-0.3.6.post0/octomachinery/utils/asynctools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Asynchronous tools set."""
 
 from functools import wraps
 from operator import itemgetter
 
-from anyio import create_queue, create_task_group as all_subtasks_awaited
+from anyio import create_queue
+from anyio import create_task_group as all_subtasks_awaited
 
 
 def auto_cleanup_aio_tasks(async_func):
     """Ensure all subtasks finish."""
     @wraps(async_func)
     async def async_func_wrapper(*args, **kwargs):
         async with all_subtasks_awaited():
```

### Comparing `octomachinery-0.3.6/octomachinery/utils/versiontools.py` & `octomachinery-0.3.6.post0/octomachinery/utils/versiontools.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """Version tools set."""
 
 import os
 from typing import Callable, Optional, Union
 
 from setuptools_scm import get_version
+from setuptools_scm.version import ScmVersion
 
 
 def get_version_from_scm_tag(
         *,
         root: str = '.',
         relative_to: Optional[str] = None,
-        local_scheme: Union[Callable, str] = 'node-and-date',
+        local_scheme: Union[
+            Callable[[ScmVersion], str], str,
+        ] = 'node-and-date',
 ) -> str:
     """Retrieve the version from SCM tag in Git or Hg."""
     try:
         return get_version(
             root=root,
             relative_to=relative_to,
             local_scheme=local_scheme,
```

### Comparing `octomachinery-0.3.6/octomachinery.egg-info/PKG-INFO` & `octomachinery-0.3.6.post0/octomachinery.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,127 +1,23 @@
 Metadata-Version: 2.1
 Name: octomachinery
-Version: 0.3.6
+Version: 0.3.6.post0
 Summary: Invisible engine driving octobot machines. Simple, yet powerful.
 Home-page: https://octomachinery.dev
 Author: Sviatoslav Sydorenko (@webknjaz)
 Author-email: wk+octomachinery@sydorenko.org.ua
 License: GPLv3+
-Project-URL: Bug Tracker, https://github.com/sanitizers/octomachinery/issues
+Project-URL: Chat: Matrix, https://matrix.to/#/#octomachinery:matrix.org
+Project-URL: Chat: Matrix (PyBA), https://matrix.to/#/#pyba:matrix.org
+Project-URL: Chat: Matrix (@webknjaz), https://matrix.to/#/@webknjaz:matrix.org
 Project-URL: CI: GitHub, https://github.com/sanitizers/octomachinery/actions?workflow=Build/Test/Publish
-Project-URL: Documentation, https://docs.octomachinery.dev
-Project-URL: Source Code, https://github.com/sanitizers/octomachinery
-Description: .. image:: https://img.shields.io/pypi/v/octomachinery.svg?logo=Python&logoColor=white
-           :target: https://pypi.org/project/octomachinery
-           :alt: octomachinery @ PyPI
-        
-        .. image:: https://tidelift.com/badges/package/pypi/octomachinery
-           :target: https://tidelift.com/subscription/pkg/pypi-octomachinery?utm_source=pypi-octomachinery&utm_medium=readme
-           :alt: octomachinery is available as part of the Tidelift Subscription
-        
-        .. image:: https://github.com/sanitizers/octomachinery/workflows/Build%2FTest%2FPublish/badge.svg
-           :target: https://github.com/sanitizers/octomachinery/actions?workflow=Build%2FTest%2FPublish
-           :alt: GitHub Actions CI/CD build status — Python package
-        
-        .. DO-NOT-REMOVE-docs-badges-END
-        
-        .. image:: https://img.shields.io/readthedocs/octomachinery/latest.svg?logo=Read%20The%20Docs&logoColor=white
-           :target: https://docs.octomachinery.dev/en/latest/?badge=latest
-           :alt: Documentation Status
-        
-        octomachinery: Bots Without Boilerplate
-        =======================================
-        
-        Invisible engine driving octobot machines. Simple, yet powerful.
-        
-        Web-site @ https://octomachinery.dev. Stay tuned!
-        
-        .. DO-NOT-REMOVE-docs-intro-START
-        
-        **How-to create a GitHub Bot tutorial** is ready for preview
-        @ `tutorial.octomachinery.dev
-        <https://tutorial.octomachinery.dev/en/latest/>`_
-        
-        Elevator pitch
-        --------------
-        
-        Here's how you 👍 a just-created comment:
-        
-        .. code:: python
-        
-            from octomachinery.app.server.runner import run as run_app
-            from octomachinery.routing import process_event_actions
-            from octomachinery.routing.decorators import process_webhook_payload
-            from octomachinery.runtime.context import RUNTIME_CONTEXT
-        
-        
-            @process_event_actions('issue_comment', {'created'})
-            @process_webhook_payload
-            async def on_comment(
-                    *,
-                    action, issue, comment,
-                    repository=None, sender=None,
-                    installation=None,
-                    assignee=None, changes=None,
-            ):
-                github_api = RUNTIME_CONTEXT.app_installation_client
-                comment_reactions_api_url = f'{comment["url"]}/reactions'
-                await github_api.post(
-                    comment_reactions_api_url,
-                    preview_api_version='squirrel-girl',
-                    data={'content': '+1'},
-                )
-        
-        
-            run_app(
-                name='Thumbs-Up-Bot',
-                version='1.0.0',
-                url='https://github.com/apps/thuuuuuuuuuuuuuumbs-uuuuuuuuuuuup',
-            )
-        
-        Prerequisites
-        -------------
-        
-        Python 3.7+
-        
-        Contribute octomachinery
-        ------------------------
-        
-        **Want to add something to upstream?** Feel free to submit a PR or file
-        an issue if unsure.
-        Note that PR is more likely to be accepted if it includes tests and
-        detailed description helping maintainers to understand it better 🎉
-        
-        Oh, and be pythonic, please 🐍
-        
-        **Don't know how?** Check out `How to Contribute to Open Source
-        <https://opensource.guide/how-to-contribute/>`_ article by GitHub 🚀
-        
-        License
-        -------
-        
-        The source code and the documentation in this project are released under
-        the `GPL v3 license`_.
-        
-        .. _`GPL v3 license`:
-           https://github.com/sanitizers/octomachinery/blob/master/LICENSE
-        
-        For Enterprise
-        --------------
-        
-        octomachinery is available as part of the Tidelift Subscription.
-        
-        The octomachinery maintainers and the maintainers of thousands of other packages
-        are working with Tidelift to deliver one enterprise subscription that covers
-        all of the open source you use.
-        
-        `Learn more <https://tidelift.com/subscription/pkg/pypi-octomachinery?utm_source=pypi-octomachinery&utm_medium=referral&utm_campaign=github>`_.
-        
+Project-URL: Docs: RTD, https://docs.octomachinery.dev
+Project-URL: GitHub: issues, https://github.com/sanitizers/octomachinery/issues
+Project-URL: GitHub: repo, https://github.com/sanitizers/octomachinery
 Keywords: Bot,Framework,Framework for writing GitHub Apps,GitHub,GitHub Actions,GitHub API,GitHub Apps,GitHub Checks API
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Environment :: Other Environment
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -148,7 +44,118 @@
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: testing
+License-File: LICENSE
+
+.. image:: https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/banner-direct.svg
+   :target: https://github.com/vshymanskyy/StandWithUkraine/blob/main/docs/README.md
+   :alt: SWUbanner
+
+.. image:: https://img.shields.io/pypi/v/octomachinery.svg?logo=Python&logoColor=white
+   :target: https://pypi.org/project/octomachinery
+   :alt: octomachinery @ PyPI
+
+.. image:: https://tidelift.com/badges/package/pypi/octomachinery
+   :target: https://tidelift.com/subscription/pkg/pypi-octomachinery?utm_source=pypi-octomachinery&utm_medium=readme
+   :alt: octomachinery is available as part of the Tidelift Subscription
+
+.. image:: https://github.com/sanitizers/octomachinery/workflows/Build%2FTest%2FPublish/badge.svg
+   :target: https://github.com/sanitizers/octomachinery/actions?workflow=Build%2FTest%2FPublish
+   :alt: GitHub Actions CI/CD build status — Python package
+
+.. DO-NOT-REMOVE-docs-badges-END
+
+.. image:: https://img.shields.io/readthedocs/octomachinery/latest.svg?logo=Read%20The%20Docs&logoColor=white
+   :target: https://docs.octomachinery.dev/en/latest/?badge=latest
+   :alt: Documentation Status
+
+octomachinery: Bots Without Boilerplate
+=======================================
+
+Invisible engine driving octobot machines. Simple, yet powerful.
+
+Web-site @ https://octomachinery.dev. Stay tuned!
+
+.. DO-NOT-REMOVE-docs-intro-START
+
+**How-to create a GitHub Bot tutorial** is ready for preview
+@ `tutorial.octomachinery.dev
+<https://tutorial.octomachinery.dev/en/latest/>`_
+
+Elevator pitch
+--------------
+
+Here's how you 👍 a just-created comment:
+
+.. code:: python
+
+    from octomachinery.app.server.runner import run as run_app
+    from octomachinery.routing import process_event_actions
+    from octomachinery.routing.decorators import process_webhook_payload
+    from octomachinery.runtime.context import RUNTIME_CONTEXT
+
+
+    @process_event_actions('issue_comment', {'created'})
+    @process_webhook_payload
+    async def on_comment(
+            *,
+            action, issue, comment,
+            repository=None, sender=None,
+            installation=None,
+            assignee=None, changes=None,
+    ):
+        github_api = RUNTIME_CONTEXT.app_installation_client
+        comment_reactions_api_url = f'{comment["url"]}/reactions'
+        await github_api.post(
+            comment_reactions_api_url,
+            preview_api_version='squirrel-girl',
+            data={'content': '+1'},
+        )
+
+
+    run_app(
+        name='Thumbs-Up-Bot',
+        version='1.0.0',
+        url='https://github.com/apps/thuuuuuuuuuuuuuumbs-uuuuuuuuuuuup',
+    )
+
+Prerequisites
+-------------
+
+Python 3.7+
+
+Contribute octomachinery
+------------------------
+
+**Want to add something to upstream?** Feel free to submit a PR or file
+an issue if unsure.
+Note that PR is more likely to be accepted if it includes tests and
+detailed description helping maintainers to understand it better 🎉
+
+Oh, and be pythonic, please 🐍
+
+**Don't know how?** Check out `How to Contribute to Open Source
+<https://opensource.guide/how-to-contribute/>`_ article by GitHub 🚀
+
+License
+-------
+
+The source code and the documentation in this project are released under
+the `GPL v3 license`_.
+
+.. _`GPL v3 license`:
+   https://github.com/sanitizers/octomachinery/blob/master/LICENSE
+
+For Enterprise
+--------------
+
+octomachinery is available as part of the Tidelift Subscription.
+
+The octomachinery maintainers and the maintainers of thousands of other packages
+are working with Tidelift to deliver one enterprise subscription that covers
+all of the open source you use.
+
+`Learn more <https://tidelift.com/subscription/pkg/pypi-octomachinery?utm_source=pypi-octomachinery&utm_medium=referral&utm_campaign=github>`_.
```

### Comparing `octomachinery-0.3.6/octomachinery.egg-info/SOURCES.txt` & `octomachinery-0.3.6.post0/octomachinery.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 .docs-requirements.txt
 .git_archival.txt
 .gitattributes
 .gitignore
-.pre-commit-config.ci.yaml
+.isort.cfg
 .pre-commit-config.yaml
 .pylintrc
 .readthedocs.yml
+.yamllint
 LICENSE
 README.rst
 mypy.ini
 pyproject.toml
 pytest.ini
 setup.cfg
 tox.ini
@@ -66,16 +67,17 @@
 ./tests/app/server/machinery_test.py
 ./tests/github/models/private_key_test.py
 ./tests/github/models/utils_test.py
 ./tests/github/utils/event_utils_test.py
 ./tests/utils/asynctools_test.py
 ./tests/utils/versiontools_test.py
 .github/FUNDING.yml
+.github/deadpendency.yaml
+.github/workflows/ci-cd.yml
 .github/workflows/publish-to-test-pypi.yml
-.github/workflows/python-tox.yml
 docs/conf.py
 docs/getting-started.rst
 docs/howto-guides.rst
 docs/index.rst
 docs/_static/custom.css
 docs/_templates/github-sponsors.html
 docs/_templates/project-description.html
```

### Comparing `octomachinery-0.3.6/setup.cfg` & `octomachinery-0.3.6.post0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-[aliases]
-dists = clean --all sdist bdist_wheel
-
 [bdist_wheel]
 universal = 0
 
 [metadata]
 name = octomachinery
 version = attr: octomachinery.utils.versiontools.get_self_version
 url = https://octomachinery.dev
 project_urls = 
-	Bug Tracker = https://github.com/sanitizers/octomachinery/issues
+	Chat: Matrix = https://matrix.to/#/#octomachinery:matrix.org
+	Chat: Matrix (PyBA) = https://matrix.to/#/#pyba:matrix.org
+	Chat: Matrix (@webknjaz) = https://matrix.to/#/@webknjaz:matrix.org
 	CI: GitHub = https://github.com/sanitizers/octomachinery/actions?workflow=Build/Test/Publish
-	Documentation = https://docs.octomachinery.dev
-	Source Code = https://github.com/sanitizers/octomachinery
+	Docs: RTD = https://docs.octomachinery.dev
+	GitHub: issues = https://github.com/sanitizers/octomachinery/issues
+	GitHub: repo = https://github.com/sanitizers/octomachinery
 description = Invisible engine driving octobot machines. Simple, yet powerful.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Sviatoslav Sydorenko (@webknjaz)
 author_email = wk+octomachinery@sydorenko.org.ua
 license = GPLv3+
 license_file = LICENSE
@@ -85,15 +85,15 @@
 install_requires = 
 	aiohttp
 	anyio < 2.0.0
 	click
 	cryptography
 	environ-config >= 19.1.0
 	envparse
-	gidgethub >= 4.2.0
+	gidgethub >= 4.2.0, < 5.3
 	pyjwt[crypto]
 	pyyaml
 	sentry_sdk
 	setuptools_scm
 
 [options.packages.find]
 where = .
```

### Comparing `octomachinery-0.3.6/tests/app/action/runner_test.py` & `octomachinery-0.3.6.post0/tests/app/action/runner_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 import json
 
 import pytest
 
 from octomachinery.app.action.config import GitHubActionConfig
 from octomachinery.app.action.runner import run
 from octomachinery.app.config import BotAppConfig
-from octomachinery.app.routing import process_event
-from octomachinery.app.routing import process_event_actions
+from octomachinery.app.routing import process_event, process_event_actions
 from octomachinery.app.runtime.config import RuntimeConfig
 from octomachinery.app.server.config import WebServerConfig
 from octomachinery.github.config.app import GitHubAppIntegrationConfig
 from octomachinery.github.errors import GitHubActionError
 from octomachinery.github.models.action_outcomes import ActionNeutral
 
 
@@ -58,17 +57,19 @@
 @pytest.fixture
 def config(monkeypatch, event_file, request):
     """Create a dummy GitHub Action config."""
     monkeypatch.setattr(
         'octomachinery.app.runtime.utils.detect_env_mode',
         lambda: 'action',
     )
-    return BotAppConfig(
+    # pylint: disable=fixme
+    return BotAppConfig(  # type: ignore[call-arg]  # FIXME
         github=GitHubAppIntegrationConfig(),
-        action=GitHubActionConfig(
+        # pylint: disable=fixme
+        action=GitHubActionConfig(  # type: ignore[call-arg]  # FIXME
             workflow='Test Workflow',
             action='Test Action',
             actor='username-or-bot',
             repository='org/repo',
             event_name=request.param,  # 'check_run'
             event_path=str(event_file),  # '/github/workflow/event.json'
             workspace='/github/workspace',
```

### Comparing `octomachinery-0.3.6/tests/app/routing/decorators_test.py` & `octomachinery-0.3.6.post0/tests/app/routing/decorators_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,18 @@
         ({'arg1': 'z'}, False),
         ({'arg3': 's'}, False),
         (dict(), False),
     ),
 )
 def test_process_webhook_payload(incoming_event, is_successful):
     """Test that @process_webhook_payload unpacks event into kw-args."""
-    event = GitHubEvent(name=None, payload=incoming_event)
+    event = GitHubEvent(
+        name=None,  # type: ignore[arg-type]
+        payload=incoming_event,
+    )
 
     if is_successful:
         assert (
             # pylint: disable=missing-kwoa,too-many-function-args
             fake_event_handler(event)
             == tuple(incoming_event.values())
         )
```

### Comparing `octomachinery-0.3.6/tests/app/server/machinery_test.py` & `octomachinery-0.3.6.post0/tests/app/server/machinery_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Test app server machinery."""
 
 import uuid
+from typing import Tuple
 
 from aiohttp.client import ClientSession
-from aiohttp.web import SockSite
 from aiohttp.test_utils import get_unused_port_socket
+from aiohttp.web import SockSite
+
 import pytest
 
 from octomachinery.app.config import BotAppConfig
 from octomachinery.app.routing import WEBHOOK_EVENTS_ROUTER
 from octomachinery.app.server.machinery import setup_server_runner
 from octomachinery.github.api.app_client import GitHubApp
 
@@ -33,20 +35,21 @@
     """Return a GitHub App ID."""
     return 0
 
 
 @pytest.fixture
 def octomachinery_config(
         github_app_id: int, rsa_private_key_bytes: bytes,
-        ephemeral_port_tcp_sock_addr: tuple,
+        ephemeral_port_tcp_sock_addr: Tuple[str, int],
 ) -> None:
     """Initialize a GitHub App bot config."""
     host, port = ephemeral_port_tcp_sock_addr
     # https://github.com/hynek/environ-config/blob/master/CHANGELOG.rst#1910-2019-09-02
-    return BotAppConfig.from_environ({  # pylint: disable=no-member
+    # pylint: disable=no-member
+    return BotAppConfig.from_environ({  # type: ignore[attr-defined]
         'GITHUB_APP_IDENTIFIER': str(github_app_id),
         'GITHUB_PRIVATE_KEY': rsa_private_key_bytes.decode(),
         'HOST': host,
         'PORT': port,
     })
```

### Comparing `octomachinery-0.3.6/tests/circular_imports_test.py` & `octomachinery-0.3.6.post0/tests/circular_imports_test.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 This ensures all internal packages can be imported right away without
 any need to import some other module before doing so.
 
 This module is based on an idea that pytest uses for self-testing:
 * https://github.com/pytest-dev/pytest/blob/d18c75b/testing/test_meta.py
 * https://twitter.com/codewithanthony/status/1229445110510735361
 """
-from itertools import chain
-from pathlib import Path
 import os
 import pkgutil
 import subprocess
 import sys
+from itertools import chain
+from pathlib import Path
 
 import pytest
 
 import octomachinery
 
 
 def _find_all_importables(pkg):
```

### Comparing `octomachinery-0.3.6/tests/github/models/private_key_test.py` & `octomachinery-0.3.6.post0/tests/github/models/private_key_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 """Tests for GitHub private key class."""
-from datetime import date
-from pathlib import Path
 import random
 import re
+from datetime import date
+from pathlib import Path
 
 import pytest
 
-from cryptography.hazmat.primitives.serialization import (
-    Encoding,
-    PublicFormat,
-)
+from cryptography.hazmat.primitives.serialization import Encoding, PublicFormat
 from jwt import decode as parse_jwt
 
 from octomachinery.github.models.private_key import GitHubPrivateKey
 
 
 @pytest.fixture
 def rsa_public_key(rsa_private_key):
```

### Comparing `octomachinery-0.3.6/tests/github/models/utils_test.py` & `octomachinery-0.3.6.post0/tests/github/models/utils_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from datetime import datetime, timezone
 from functools import partial
 
 import pytest
 
 from octomachinery.github.models.utils import (
-    convert_datetime, SecretStr, SuperSecretStr,
+    SecretStr, SuperSecretStr, convert_datetime,
 )
 
 
 # pylint: disable=invalid-name
 utc_datetime = partial(datetime, tzinfo=timezone.utc)
```

### Comparing `octomachinery-0.3.6/tests/github/utils/event_utils_test.py` & `octomachinery-0.3.6.post0/tests/github/utils/event_utils_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 """Tests for CLI utility functions."""
 
 from io import StringIO
 from textwrap import dedent
 from uuid import uuid1, uuid4
 
 import multidict
+
 import pytest
 
 from octomachinery.github.utils.event_utils import (
-    _probe_json,
-    _transform_http_headers_list_to_multidict,
-    augment_http_headers,
-    make_http_headers_from_event,
-    parse_event_stub_from_fd,
-    validate_http_headers,
+    _probe_json, _transform_http_headers_list_to_multidict,
+    augment_http_headers, make_http_headers_from_event,
+    parse_event_stub_from_fd, validate_http_headers,
 )
 
 
 UNCHANGED_UUID4_STR = str(uuid4())
 
 
 @pytest.mark.parametrize(
```

### Comparing `octomachinery-0.3.6/tests/utils/asynctools_test.py` & `octomachinery-0.3.6.post0/tests/utils/asynctools_test.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6/tests/utils/versiontools_test.py` & `octomachinery-0.3.6.post0/tests/utils/versiontools_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,20 +3,19 @@
 import contextlib
 import os
 import pathlib
 import subprocess
 import tempfile
 
 import pytest
+
 import setuptools_scm.version
 
 from octomachinery.utils.versiontools import (
-    cut_local_version_on_upload,
-    get_self_version,
-    get_version_from_scm_tag,
+    cut_local_version_on_upload, get_self_version, get_version_from_scm_tag,
 )
 
 
 @contextlib.contextmanager
 def working_directory(path):
     """Change working directory and return back to previous on exit."""
     prev_cwd = pathlib.Path.cwd()
@@ -101,19 +100,27 @@
     """Check that version is unknown outside of Git repo."""
     assert get_self_version() == 'unknown'
 
 
 def test_cut_local_version_on_upload(monkeypatch, tmp_git_repo):
     """Test that PEP440 local version isn't emitted when upload."""
     scm_node = 'gfe99188'
-    ver = setuptools_scm.version.ScmVersion(
-        'v1.1.4',
-        distance=3, node='gfe99188',
-        dirty=False, branch='master',
-    )
+    try:
+        ver = setuptools_scm.version.ScmVersion(
+            'v1.1.4',
+            distance=3, node='gfe99188',
+            dirty=False, branch='master',
+            config=setuptools_scm.config.Configuration(),
+        )
+    except AttributeError:
+        ver = setuptools_scm.version.ScmVersion(
+            'v1.1.4',
+            distance=3, node='gfe99188',
+            dirty=False, branch='master',
+        )
     assert cut_local_version_on_upload(ver) == f'+{scm_node}'
 
     with monkeypatch.context() as mp_ctx:
         mp_ctx.setenv('PYPI_UPLOAD', 'true')
         assert cut_local_version_on_upload(ver) == ''
```

### Comparing `octomachinery-0.3.6/tox.ini` & `octomachinery-0.3.6.post0/tox.ini`

 * *Files 5% similar despite different names*

```diff
@@ -30,17 +30,22 @@
   # NOTE: happens later and overrides it.
   # NOTE: With this step we're setting certain packages to the lowest
   # NOTE: versions — either limited by the runtime deps or just known
   # NOTE: to work.
   # NOTE: For example, PyJWT versions below 1.4.2 cause TypeError when
   # NOTE: the PEM key is passed as bytes.
   # Ref: https://github.com/sanitizers/octomachinery/issues/46:
-  {envpython} -m pip install 'gidgethub === 4.2.0' 'pyjwt === 1.4.2'
+  {envpython} -m pip install \
+    'cryptography == 2.4.2' \
+    'gidgethub == 4.2.0' \
+    'pyjwt == 1.4.2' \
+    'pytest-aiohttp == 0.1.0' \
+    'setuptools-scm == 1.15.4'
 setenv =
-  PYTEST_ADDOPTS = -W ignore:::jwt.api_jwt -W ignore:::jwt.algorithms
+  PYTEST_ADDOPTS = -p no:warnings
 
 
 [testenv:check-docs]
 basepython = python3
 isolated_build = true
 # `usedevelop = true` overrides `skip_install` instruction, it's unwanted
 usedevelop = false
@@ -181,23 +186,15 @@
 
 
 [testenv:pre-commit]
 isolated_build = true
 deps =
   pre-commit
   pylint === 2.7.2
-  pylint-pytest
+  pylint-pytest < 1.1.0
 commands =
   {envpython} -m pre_commit run --show-diff-on-failure {posargs:--all-files}
 
   # Print out the advise of how to install pre-commit from this env into Git:
   -{envpython} -c \
   'cmd = "{envpython} -m pre_commit install"; scr_width = len(cmd) + 10; sep = "=" * scr_width; cmd_str = "    $ " + cmd; '\
   'print("\n" + sep + "\nTo install pre-commit hooks into the Git repo, run:\n\n" + cmd_str + "\n\n" + sep + "\n")'
-
-
-[testenv:pre-commit-ci]
-isolated_build = true
-deps =
-  {[testenv:pre-commit]deps}
-commands =
-  {envpython} -m pre_commit run --show-diff-on-failure --config .pre-commit-config.ci.yaml {posargs:--all-files}
```

