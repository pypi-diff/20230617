# Comparing `tmp/octomachinery-0.3.6.post0.tar.gz` & `tmp/octomachinery-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octomachinery-0.3.6.post0.tar", last modified: Sat Jun 17 11:55:55 2023, max compression
+gzip compressed data, was "octomachinery-0.3.7.tar", last modified: Sat Jun 17 19:37:53 2023, max compression
```

## Comparing `octomachinery-0.3.6.post0.tar` & `octomachinery-0.3.7.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.441181 octomachinery-0.3.6.post0/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/.docs-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/.github/deadpendency.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)    24092 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/.github/workflows/ci-cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-06-17 11:55:55.441181 octomachinery-0.3.6.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.441181 octomachinery-0.3.6.post0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.441181 octomachinery-0.3.6.post0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/docs/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.441181 octomachinery-0.3.6.post0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/docs/_templates/github-sponsors.html
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/docs/_templates/project-description.html
--rw-r--r--   0 runner    (1001) docker     (123)     9423 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/docs/getting-started.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/docs/howto-guides.rst
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.433181 octomachinery-0.3.6.post0/octomachinery/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.433181 octomachinery-0.3.6.post0/octomachinery/app/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.433181 octomachinery-0.3.6.post0/octomachinery/app/action/
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/app/action/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/app/action/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/app/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.433181 octomachinery-0.3.6.post0/octomachinery/app/routing/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/app/routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/app/routing/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/app/routing/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/app/routing/routers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/app/routing/webhooks_dispatcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.433181 octomachinery-0.3.6.post0/octomachinery/app/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/app/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/app/runtime/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/app/runtime/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/app/runtime/installation_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/app/runtime/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.433181 octomachinery-0.3.6.post0/octomachinery/app/server/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/app/server/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/app/server/machinery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/app/server/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.433181 octomachinery-0.3.6.post0/octomachinery/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/cli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.421181 octomachinery-0.3.6.post0/octomachinery/github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/octomachinery/github/api/
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/github/api/app_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/github/api/raw_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/github/api/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/github/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/octomachinery/github/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/github/config/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/octomachinery/github/entities/
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/github/entities/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/github/entities/app_installation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/octomachinery/github/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/github/errors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/octomachinery/github/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/github/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/github/models/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/github/models/action_outcomes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/github/models/checks_api_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/github/models/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/github/models/private_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/github/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/octomachinery/github/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/github/utils/event_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/octomachinery/routing/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/routing/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/routing/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/routing/default_router.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/routing/routers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/routing/webhooks_dispatcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/octomachinery/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/runtime/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/runtime/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/octomachinery/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/utils/asynctools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/octomachinery/utils/versiontools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.441181 octomachinery-0.3.6.post0/octomachinery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-06-17 11:55:55.000000 octomachinery-0.3.6.post0/octomachinery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-06-17 11:55:55.000000 octomachinery-0.3.6.post0/octomachinery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 11:55:55.000000 octomachinery-0.3.6.post0/octomachinery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-17 11:55:55.000000 octomachinery-0.3.6.post0/octomachinery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-17 11:55:55.000000 octomachinery-0.3.6.post0/octomachinery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 11:55:55.000000 octomachinery-0.3.6.post0/octomachinery.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-06-17 11:55:55.441181 octomachinery-0.3.6.post0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.421181 octomachinery-0.3.6.post0/tests/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/tests/app/action/
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/tests/app/action/runner_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/tests/app/routing/
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/tests/app/routing/decorators_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/tests/app/server/
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/tests/app/server/machinery_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/tests/circular_imports_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.425181 octomachinery-0.3.6.post0/tests/github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/tests/github/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/tests/github/models/private_key_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/tests/github/models/utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/tests/github/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    11810 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/tests/github/utils/event_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:55:55.437181 octomachinery-0.3.6.post0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/tests/utils/asynctools_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/tests/utils/versiontools_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-06-17 11:55:42.000000 octomachinery-0.3.6.post0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:37:53.743804 octomachinery-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-17 19:37:40.000000 octomachinery-0.3.7/.docs-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-17 19:37:40.000000 octomachinery-0.3.7/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-17 19:37:40.000000 octomachinery-0.3.7/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:37:53.739804 octomachinery-0.3.7/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-17 19:37:40.000000 octomachinery-0.3.7/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-17 19:37:40.000000 octomachinery-0.3.7/.github/deadpendency.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:37:53.739804 octomachinery-0.3.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)    24092 2023-06-17 19:37:40.000000 octomachinery-0.3.7/.github/workflows/ci-cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-17 19:37:40.000000 octomachinery-0.3.7/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-17 19:37:40.000000 octomachinery-0.3.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-17 19:37:40.000000 octomachinery-0.3.7/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-17 19:37:40.000000 octomachinery-0.3.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-06-17 19:37:40.000000 octomachinery-0.3.7/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-17 19:37:40.000000 octomachinery-0.3.7/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-17 19:37:40.000000 octomachinery-0.3.7/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-17 19:37:40.000000 octomachinery-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-06-17 19:37:53.743804 octomachinery-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-06-17 19:37:40.000000 octomachinery-0.3.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:37:53.739804 octomachinery-0.3.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:37:53.739804 octomachinery-0.3.7/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-17 19:37:40.000000 octomachinery-0.3.7/docs/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:37:53.739804 octomachinery-0.3.7/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-17 19:37:40.000000 octomachinery-0.3.7/docs/_templates/github-sponsors.html
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-17 19:37:40.000000 octomachinery-0.3.7/docs/_templates/project-description.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9423 2023-06-17 19:37:40.000000 octomachinery-0.3.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-17 19:37:40.000000 octomachinery-0.3.7/docs/getting-started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-17 19:37:40.000000 octomachinery-0.3.7/docs/howto-guides.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-17 19:37:40.000000 octomachinery-0.3.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-17 19:37:40.000000 octomachinery-0.3.7/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:37:53.719804 octomachinery-0.3.7/octomachinery/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:37:53.719804 octomachinery-0.3.7/octomachinery/app/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:37:53.719804 octomachinery-0.3.7/octomachinery/app/action/
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/app/action/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/app/action/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/app/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:37:53.723804 octomachinery-0.3.7/octomachinery/app/routing/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/app/routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/app/routing/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/app/routing/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/app/routing/routers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/app/routing/webhooks_dispatcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:37:53.723804 octomachinery-0.3.7/octomachinery/app/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/app/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/app/runtime/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/app/runtime/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/app/runtime/installation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/app/runtime/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:37:53.723804 octomachinery-0.3.7/octomachinery/app/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/app/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/app/server/machinery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/app/server/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:37:53.723804 octomachinery-0.3.7/octomachinery/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/cli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:37:53.707804 octomachinery-0.3.7/octomachinery/github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:37:53.727804 octomachinery-0.3.7/octomachinery/github/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/github/api/app_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/github/api/raw_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/github/api/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/github/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:37:53.727804 octomachinery-0.3.7/octomachinery/github/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/github/config/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:37:53.727804 octomachinery-0.3.7/octomachinery/github/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/github/entities/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/github/entities/app_installation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:37:53.727804 octomachinery-0.3.7/octomachinery/github/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/github/errors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:37:53.731804 octomachinery-0.3.7/octomachinery/github/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/github/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/github/models/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/github/models/action_outcomes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/github/models/checks_api_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/github/models/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/github/models/private_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/github/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:37:53.731804 octomachinery-0.3.7/octomachinery/github/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/github/utils/event_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:37:53.731804 octomachinery-0.3.7/octomachinery/routing/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/routing/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/routing/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/routing/default_router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/routing/routers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/routing/webhooks_dispatcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:37:53.731804 octomachinery-0.3.7/octomachinery/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/runtime/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/runtime/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:37:53.735804 octomachinery-0.3.7/octomachinery/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/utils/asynctools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-17 19:37:40.000000 octomachinery-0.3.7/octomachinery/utils/versiontools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:37:53.743804 octomachinery-0.3.7/octomachinery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-06-17 19:37:53.000000 octomachinery-0.3.7/octomachinery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-06-17 19:37:53.000000 octomachinery-0.3.7/octomachinery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 19:37:53.000000 octomachinery-0.3.7/octomachinery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-17 19:37:53.000000 octomachinery-0.3.7/octomachinery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-17 19:37:53.000000 octomachinery-0.3.7/octomachinery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 19:37:53.000000 octomachinery-0.3.7/octomachinery.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-17 19:37:40.000000 octomachinery-0.3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-17 19:37:40.000000 octomachinery-0.3.7/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-17 19:37:53.743804 octomachinery-0.3.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:37:53.735804 octomachinery-0.3.7/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:37:53.711804 octomachinery-0.3.7/tests/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:37:53.735804 octomachinery-0.3.7/tests/app/action/
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-17 19:37:40.000000 octomachinery-0.3.7/tests/app/action/runner_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:37:53.735804 octomachinery-0.3.7/tests/app/routing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-17 19:37:40.000000 octomachinery-0.3.7/tests/app/routing/decorators_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:37:53.735804 octomachinery-0.3.7/tests/app/server/
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-06-17 19:37:40.000000 octomachinery-0.3.7/tests/app/server/machinery_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-17 19:37:40.000000 octomachinery-0.3.7/tests/circular_imports_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-17 19:37:40.000000 octomachinery-0.3.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:37:53.711804 octomachinery-0.3.7/tests/github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:37:53.735804 octomachinery-0.3.7/tests/github/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-06-17 19:37:40.000000 octomachinery-0.3.7/tests/github/models/private_key_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-06-17 19:37:40.000000 octomachinery-0.3.7/tests/github/models/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:37:53.735804 octomachinery-0.3.7/tests/github/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    11810 2023-06-17 19:37:40.000000 octomachinery-0.3.7/tests/github/utils/event_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:37:53.735804 octomachinery-0.3.7/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-17 19:37:40.000000 octomachinery-0.3.7/tests/utils/asynctools_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-06-17 19:37:40.000000 octomachinery-0.3.7/tests/utils/versiontools_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-06-17 19:37:40.000000 octomachinery-0.3.7/tox.ini
```

### Comparing `octomachinery-0.3.6.post0/.github/workflows/ci-cd.yml` & `octomachinery-0.3.7/.github/workflows/ci-cd.yml`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/.github/workflows/publish-to-test-pypi.yml` & `octomachinery-0.3.7/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/.gitignore` & `octomachinery-0.3.7/.gitignore`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/.isort.cfg` & `octomachinery-0.3.7/.isort.cfg`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/.pre-commit-config.yaml` & `octomachinery-0.3.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/.pylintrc` & `octomachinery-0.3.7/.pylintrc`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/LICENSE` & `octomachinery-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/PKG-INFO` & `octomachinery-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octomachinery
-Version: 0.3.6.post0
+Version: 0.3.7
 Summary: Invisible engine driving octobot machines. Simple, yet powerful.
 Home-page: https://octomachinery.dev
 Author: Sviatoslav Sydorenko (@webknjaz)
 Author-email: wk+octomachinery@sydorenko.org.ua
 License: GPLv3+
 Project-URL: Chat: Matrix, https://matrix.to/#/#octomachinery:matrix.org
 Project-URL: Chat: Matrix (PyBA), https://matrix.to/#/#pyba:matrix.org
```

### Comparing `octomachinery-0.3.6.post0/README.rst` & `octomachinery-0.3.7/README.rst`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/docs/_static/custom.css` & `octomachinery-0.3.7/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/docs/conf.py` & `octomachinery-0.3.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/docs/getting-started.rst` & `octomachinery-0.3.7/docs/getting-started.rst`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/docs/howto-guides.rst` & `octomachinery-0.3.7/docs/howto-guides.rst`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/docs/index.rst` & `octomachinery-0.3.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery/app/action/config.py` & `octomachinery-0.3.7/octomachinery/app/action/config.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery/app/action/runner.py` & `octomachinery-0.3.7/octomachinery/app/action/runner.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery/app/config.py` & `octomachinery-0.3.7/octomachinery/app/config.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery/app/routing/webhooks_dispatcher.py` & `octomachinery-0.3.7/octomachinery/app/routing/webhooks_dispatcher.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery/app/runtime/config.py` & `octomachinery-0.3.7/octomachinery/app/runtime/config.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery/app/runtime/installation_utils.py` & `octomachinery-0.3.7/octomachinery/app/runtime/installation_utils.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery/app/runtime/utils.py` & `octomachinery-0.3.7/octomachinery/app/runtime/utils.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery/app/server/machinery.py` & `octomachinery-0.3.7/octomachinery/app/server/machinery.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery/app/server/runner.py` & `octomachinery-0.3.7/octomachinery/app/server/runner.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery/cli/__main__.py` & `octomachinery-0.3.7/octomachinery/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery/github/api/app_client.py` & `octomachinery-0.3.7/octomachinery/github/api/app_client.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery/github/api/raw_client.py` & `octomachinery-0.3.7/octomachinery/github/api/raw_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -51,35 +51,48 @@
     # pylint: disable=too-many-arguments
     async def _make_request(
             self, method: str, url: str, url_vars: Dict[str, str],
             data: Any, accept: str = None,
             jwt: Optional[str] = None,
             oauth_token: Optional[str] = None,
             content_type: str = JSON_CONTENT_TYPE,
+            extra_headers: Optional[Dict[str, str]] = None,
     ) -> Tuple[bytes, Optional[str]]:
         token = self._token
         # pylint: disable=fixme
         if iscoroutinefunction(token):  # type: ignore[arg-type]  # FIXME
             # pylint: disable=fixme
             token = await token()  # type: ignore[misc,operator]  # FIXME
         if isinstance(token, GitHubOAuthToken):
             oauth_token = str(token)
             jwt = None
         if isinstance(token, GitHubJWTToken):
             jwt = str(token)
             oauth_token = None
+        optional_kwargs = {
+            # NOTE: GidgetHub v5.3.0 introduced a new `extra_headers` argument
+            # NOTE: in this private method and the public ones. Its default
+            # NOTE: value is `None` in all cases so the only case when it's set
+            # NOTE: is when the end-users call corresponding methods with it.
+            # NOTE: And that would only be the case with modern versions of
+            # NOTE: GidgetHub. Here, we rely on this side effect to only pass
+            # NOTE: this value down the stack when the chances that GidgetHub
+            # NOTE: is modern enough are close to 100%.
+            'extra_headers': extra_headers,
+        } if extra_headers is not None else {}
         return await super()._make_request(
             method=method,
             url=url,
             url_vars=url_vars,
             data=data,
             accept=accept,
             oauth_token=oauth_token,
             jwt=jwt,
             content_type=content_type,
+            **optional_kwargs,
         )
 
     getitem = accept_preview_version(GitHubAPI.getitem)
     getiter = accept_preview_version(GitHubAPI.getiter)
     post = accept_preview_version(GitHubAPI.post)
     patch = accept_preview_version(GitHubAPI.patch)
     put = accept_preview_version(GitHubAPI.put)
```

### Comparing `octomachinery-0.3.6.post0/octomachinery/github/api/tokens.py` & `octomachinery-0.3.7/octomachinery/github/api/tokens.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery/github/api/utils.py` & `octomachinery-0.3.7/octomachinery/github/api/utils.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery/github/config/app.py` & `octomachinery-0.3.7/octomachinery/github/config/app.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery/github/entities/action.py` & `octomachinery-0.3.7/octomachinery/github/entities/action.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery/github/entities/app_installation.py` & `octomachinery-0.3.7/octomachinery/github/entities/app_installation.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery/github/errors/__init__.py` & `octomachinery-0.3.7/octomachinery/github/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery/github/models/__init__.py` & `octomachinery-0.3.7/octomachinery/github/models/__init__.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery/github/models/_compat.py` & `octomachinery-0.3.7/octomachinery/github/models/_compat.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery/github/models/action_outcomes.py` & `octomachinery-0.3.7/octomachinery/github/models/action_outcomes.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery/github/models/checks_api_requests.py` & `octomachinery-0.3.7/octomachinery/github/models/checks_api_requests.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery/github/models/events.py` & `octomachinery-0.3.7/octomachinery/github/models/events.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery/github/models/private_key.py` & `octomachinery-0.3.7/octomachinery/github/models/private_key.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery/github/models/utils.py` & `octomachinery-0.3.7/octomachinery/github/models/utils.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery/github/utils/event_utils.py` & `octomachinery-0.3.7/octomachinery/github/utils/event_utils.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery/routing/abc.py` & `octomachinery-0.3.7/octomachinery/routing/abc.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery/routing/decorators.py` & `octomachinery-0.3.7/octomachinery/routing/decorators.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery/routing/default_router.py` & `octomachinery-0.3.7/octomachinery/routing/default_router.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery/routing/routers.py` & `octomachinery-0.3.7/octomachinery/routing/routers.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery/routing/webhooks_dispatcher.py` & `octomachinery-0.3.7/octomachinery/routing/webhooks_dispatcher.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery/runtime/context.py` & `octomachinery-0.3.7/octomachinery/runtime/context.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery/runtime/utils.py` & `octomachinery-0.3.7/octomachinery/runtime/utils.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery/utils/asynctools.py` & `octomachinery-0.3.7/octomachinery/utils/asynctools.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery/utils/versiontools.py` & `octomachinery-0.3.7/octomachinery/utils/versiontools.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/octomachinery.egg-info/PKG-INFO` & `octomachinery-0.3.7/octomachinery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octomachinery
-Version: 0.3.6.post0
+Version: 0.3.7
 Summary: Invisible engine driving octobot machines. Simple, yet powerful.
 Home-page: https://octomachinery.dev
 Author: Sviatoslav Sydorenko (@webknjaz)
 Author-email: wk+octomachinery@sydorenko.org.ua
 License: GPLv3+
 Project-URL: Chat: Matrix, https://matrix.to/#/#octomachinery:matrix.org
 Project-URL: Chat: Matrix (PyBA), https://matrix.to/#/#pyba:matrix.org
```

### Comparing `octomachinery-0.3.6.post0/octomachinery.egg-info/SOURCES.txt` & `octomachinery-0.3.7/octomachinery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/pytest.ini` & `octomachinery-0.3.7/pytest.ini`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/setup.cfg` & `octomachinery-0.3.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 install_requires = 
 	aiohttp
 	anyio < 2.0.0
 	click
 	cryptography
 	environ-config >= 19.1.0
 	envparse
-	gidgethub >= 4.2.0, < 5.3
+	gidgethub >= 4.2.0
 	pyjwt[crypto]
 	pyyaml
 	sentry_sdk
 	setuptools_scm
 
 [options.packages.find]
 where = .
```

### Comparing `octomachinery-0.3.6.post0/tests/app/action/runner_test.py` & `octomachinery-0.3.7/tests/app/action/runner_test.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/tests/app/routing/decorators_test.py` & `octomachinery-0.3.7/tests/app/routing/decorators_test.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/tests/app/server/machinery_test.py` & `octomachinery-0.3.7/tests/app/server/machinery_test.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/tests/circular_imports_test.py` & `octomachinery-0.3.7/tests/circular_imports_test.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/tests/conftest.py` & `octomachinery-0.3.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/tests/github/models/private_key_test.py` & `octomachinery-0.3.7/tests/github/models/private_key_test.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/tests/github/models/utils_test.py` & `octomachinery-0.3.7/tests/github/models/utils_test.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/tests/github/utils/event_utils_test.py` & `octomachinery-0.3.7/tests/github/utils/event_utils_test.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/tests/utils/asynctools_test.py` & `octomachinery-0.3.7/tests/utils/asynctools_test.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/tests/utils/versiontools_test.py` & `octomachinery-0.3.7/tests/utils/versiontools_test.py`

 * *Files identical despite different names*

### Comparing `octomachinery-0.3.6.post0/tox.ini` & `octomachinery-0.3.7/tox.ini`

 * *Files identical despite different names*

