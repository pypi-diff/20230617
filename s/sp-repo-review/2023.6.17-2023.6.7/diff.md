# Comparing `tmp/sp_repo_review-2023.6.17.tar.gz` & `tmp/sp_repo_review-2023.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sat Jun 17 13:51:12 2023, max compression
+gzip compressed data, last modified: Wed Jun  7 22:19:41 2023, max compression
```

## Comparing `sp_repo_review-2023.6.17.tar` & `sp_repo_review-2023.6.7.tar`

### file list

```diff
@@ -1,117 +1,116 @@
--rw-r--r--   0        0        0      125 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/.git_archival.txt
--rw-r--r--   0        0        0       45 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/.gitattributes
--rw-r--r--   0        0        0     2223 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/.pre-commit-config.yaml
--rw-r--r--   0        0        0      179 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0      571 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/.readthedocs.yml
--rw-r--r--   0        0        0        6 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/.ruby-version
--rw-r--r--   0        0        0     1294 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/Gemfile
--rw-r--r--   0        0        0     2171 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/Gemfile.lock
--rw-r--r--   0        0        0     9673 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/README.md
--rw-r--r--   0        0        0     1160 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/_config.yml
--rw-r--r--   0        0        0      763 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/action.yml
--rw-r--r--   0        0        0      799 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/cookiecutter.json
--rw-r--r--   0        0        0     2125 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/copier.yml
--rw-r--r--   0        0        0      616 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/extensions.py
--rw-r--r--   0        0        0     9634 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/noxfile.py
--rw-r--r--   0        0        0      640 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      162 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/.github/dependabot.yml
--rw-r--r--   0        0        0      726 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1219 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2038 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/.github/workflows/reusable-change-detection.yml
--rw-r--r--   0        0        0     5246 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/.github/workflows/reusable-cookie.yml
--rw-r--r--   0        0        0      919 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/.github/workflows/reusable-rr-tests.yml
--rw-r--r--   0        0        0      251 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/LICENSE
--rw-r--r--   0        0        0      829 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/README.md
--rw-r--r--   0        0        0     2180 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/_includes/head.html
--rw-r--r--   0        0        0     1019 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/_includes/head_custom.html
--rw-r--r--   0        0        0      545 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/_includes/interactive_repo_review.html
--rw-r--r--   0        0        0       92 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/_includes/rr.html
--rw-r--r--   0        0        0      150 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/_includes/toc.html
--rw-r--r--   0        0        0       22 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/_sass/color_schemes/skhep.scss
--rw-r--r--   0        0        0     2611 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/_sass/custom/custom.scss
--rw-r--r--   0        0        0    15086 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/assets/favicon.ico
--rw-r--r--   0        0        0     8070 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/assets/images/logo.svg
--rw-r--r--   0        0        0      652 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/assets/js/tabs.js
--rw-r--r--   0        0        0    10211 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/assets/js/webapp.js
--rw-r--r--   0        0        0     2335 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/pages/index.md
--rw-r--r--   0        0        0     4512 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/pages/guides/coverage.md
--rw-r--r--   0        0        0    11293 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/pages/guides/gha_basic.md
--rw-r--r--   0        0        0     9205 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/pages/guides/gha_pure.md
--rw-r--r--   0        0        0     8224 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/pages/guides/gha_wheels.md
--rw-r--r--   0        0        0     2213 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/pages/guides/index.md
--rw-r--r--   0        0        0     8606 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/pages/guides/mypy.md
--rw-r--r--   0        0        0    17927 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/pages/guides/packaging_classic.md
--rw-r--r--   0        0        0     9182 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/pages/guides/packaging_simple.md
--rw-r--r--   0        0        0    14552 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/pages/guides/pytest.md
--rw-r--r--   0        0        0      932 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/pages/guides/repo_review.md
--rw-r--r--   0        0        0    28595 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/pages/guides/style.md
--rw-r--r--   0        0        0     8853 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/pages/guides/tasks.md
--rw-r--r--   0        0        0     5310 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/pages/guides/writing-docs.md
--rw-r--r--   0        0        0     7193 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/pages/patterns/data_files.md
--rw-r--r--   0        0        0      517 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/pages/patterns/index.md
--rw-r--r--   0        0        0    11200 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/pages/principles/design.md
--rw-r--r--   0        0        0      561 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/pages/principles/index.md
--rw-r--r--   0        0        0     2209 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/pages/principles/process.md
--rw-r--r--   0        0        0     4816 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/pages/tutorials/dev-environment.md
--rw-r--r--   0        0        0      998 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/pages/tutorials/index.md
--rw-r--r--   0        0        0     2557 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/pages/tutorials/module.md
--rw-r--r--   0        0        0     3272 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/pages/tutorials/packaging.md
--rw-r--r--   0        0        0     4621 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/docs/pages/tutorials/test.md
--rw-r--r--   0        0        0      246 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/src/sp_repo_review/__init__.py
--rw-r--r--   0        0        0      168 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/src/sp_repo_review/_version.py
--rw-r--r--   0        0        0      118 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/src/sp_repo_review/_version.pyi
--rw-r--r--   0        0        0      753 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/src/sp_repo_review/families.py
--rw-r--r--   0        0        0        0 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/src/sp_repo_review/py.typed
--rw-r--r--   0        0        0        0 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/src/sp_repo_review/_compat/__init__.py
--rw-r--r--   0        0        0      233 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/src/sp_repo_review/_compat/tomllib.py
--rw-r--r--   0        0        0        0 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/src/sp_repo_review/_compat/importlib/__init__.py
--rw-r--r--   0        0        0        0 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/src/sp_repo_review/_compat/importlib/resources/__init__.py
--rw-r--r--   0        0        0      256 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/src/sp_repo_review/_compat/importlib/resources/abc.py
--rw-r--r--   0        0        0      290 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/src/sp_repo_review/checks/__init__.py
--rw-r--r--   0        0        0     2849 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/src/sp_repo_review/checks/general.py
--rw-r--r--   0        0        0     5018 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/src/sp_repo_review/checks/github.py
--rw-r--r--   0        0        0     4133 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/src/sp_repo_review/checks/mypy.py
--rw-r--r--   0        0        0     3162 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/src/sp_repo_review/checks/precommit.py
--rw-r--r--   0        0        0     5339 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/src/sp_repo_review/checks/pyproject.py
--rw-r--r--   0        0        0     2868 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/src/sp_repo_review/checks/ruff.py
--rw-r--r--   0        0        0      412 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/tests/test_cmd.py
--rw-r--r--   0        0        0      597 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/tests/test_package.py
--rw-r--r--   0        0        0      125 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/.git_archival.txt
--rw-r--r--   0        0        0       32 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/.gitattributes
--rw-r--r--   0        0        0     2218 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/.gitignore
--rw-r--r--   0        0        0     2905 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0      456 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/.readthedocs.yml
--rw-r--r--   0        0        0    14168 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/LICENSE
--rw-r--r--   0        0        0     1910 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/README.md
--rw-r--r--   0        0        0     2297 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/noxfile.py
--rw-r--r--   0        0        0     8487 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/pyproject.toml
--rw-r--r--   0        0        0      123 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/{% if cookiecutter.backend in ['setuptools','pybind11'] %}MANIFEST.in{% endif %}
--rw-r--r--   0        0        0     1982 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/{% if cookiecutter.backend in ['setuptools','pybind11'] %}setup.cfg{% endif %}
--rw-r--r--   0        0        0      691 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='maturin' %}Cargo.toml{% endif %}
--rw-r--r--   0        0        0      915 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='mesonpy' %}meson.build{% endif %}
--rw-r--r--   0        0        0      727 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='pybind11' %}setup.py{% endif %}
--rw-r--r--   0        0        0      376 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='setuptools' %}setup.py{% endif %}
--rw-r--r--   0        0        0      280 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='skbuild' %}CMakeLists.txt{% endif %}
--rw-r--r--   0        0        0      102 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/{{cookiecutter.__answers}}
--rw-r--r--   0        0        0     2528 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      163 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/.github/matchers/pylint.json
--rw-r--r--   0        0        0     3394 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1573 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/.github/workflows/{% if cookiecutter.__type == 'compiled' %}wheels.yml{% endif %}
--rw-r--r--   0        0        0     2033 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/docs/conf.py
--rw-r--r--   0        0        0      286 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/docs/index.rst
--rw-r--r--   0        0        0      632 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend in ['pybind11','skbuild','mesonpy'] %}main.cpp{% endif %}
--rw-r--r--   0        0        0      562 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend=='maturin' %}lib.rs{% endif %}
--rw-r--r--   0        0        0      422 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/__init__.py
--rw-r--r--   0        0        0        0 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/py.typed
--rw-r--r--   0        0        0      117 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/{% if cookiecutter.__type=='compiled' %}_core.pyi{% endif %}
--rw-r--r--   0        0        0      118 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/{% if cookiecutter.backend in ['setuptools', 'pybind11'] %}_version.pyi{% endif %}
--rw-r--r--   0        0        0      215 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/_compat/__init__.py
--rw-r--r--   0        0        0      500 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/src/{{cookiecutter.__project_slug}}/_compat/typing.py
--rw-r--r--   0        0        0      435 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/tests/test_package.py
--rw-r--r--   0        0        0      190 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/tests/{% if cookiecutter.__type=='compiled' %}test_compiled.py{% endif %}
--rw-r--r--   0        0        0     2248 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/.gitignore
--rw-r--r--   0        0        0     1525 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/LICENSE
--rw-r--r--   0        0        0     2948 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/README-rr.md
--rw-r--r--   0        0        0     5223 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/pyproject.toml
--rw-r--r--   0        0        0     4528 2023-06-17 13:51:12.000000 sp_repo_review-2023.6.17/PKG-INFO
+-rw-r--r--   0        0        0      125 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.git_archival.txt
+-rw-r--r--   0        0        0       32 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.gitattributes
+-rw-r--r--   0        0        0     2227 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      179 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0      571 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.readthedocs.yml
+-rw-r--r--   0        0        0        6 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.ruby-version
+-rw-r--r--   0        0        0     1294 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/Gemfile
+-rw-r--r--   0        0        0     2171 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/Gemfile.lock
+-rw-r--r--   0        0        0     8658 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/README.md
+-rw-r--r--   0        0        0     1160 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/_config.yml
+-rw-r--r--   0        0        0      763 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/action.yml
+-rw-r--r--   0        0        0      563 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/cookiecutter.json
+-rw-r--r--   0        0        0     7033 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/noxfile.py
+-rw-r--r--   0        0        0      640 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      162 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.github/dependabot.yml
+-rw-r--r--   0        0        0      726 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1219 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2018 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.github/workflows/reusable-change-detection.yml
+-rw-r--r--   0        0        0     5153 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.github/workflows/reusable-cookie.yml
+-rw-r--r--   0        0        0      919 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.github/workflows/reusable-rr-tests.yml
+-rw-r--r--   0        0        0      251 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/LICENSE
+-rw-r--r--   0        0        0      730 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/README.md
+-rw-r--r--   0        0        0     2180 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/_includes/head.html
+-rw-r--r--   0        0        0     1019 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/_includes/head_custom.html
+-rw-r--r--   0        0        0      547 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/_includes/interactive_repo_review.html
+-rw-r--r--   0        0        0       92 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/_includes/rr.html
+-rw-r--r--   0        0        0      150 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/_includes/toc.html
+-rw-r--r--   0        0        0       22 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/_sass/color_schemes/skhep.scss
+-rw-r--r--   0        0        0     2611 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/_sass/custom/custom.scss
+-rw-r--r--   0        0        0    15086 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/assets/favicon.ico
+-rw-r--r--   0        0        0     8070 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/assets/images/logo.svg
+-rw-r--r--   0        0        0      652 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/assets/js/tabs.js
+-rw-r--r--   0        0        0    10234 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/assets/js/webapp.js
+-rw-r--r--   0        0        0     2219 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/index.md
+-rw-r--r--   0        0        0     4512 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/coverage.md
+-rw-r--r--   0        0        0    11293 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/gha_basic.md
+-rw-r--r--   0        0        0     9205 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/gha_pure.md
+-rw-r--r--   0        0        0     8224 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/gha_wheels.md
+-rw-r--r--   0        0        0     2162 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/index.md
+-rw-r--r--   0        0        0     8606 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/mypy.md
+-rw-r--r--   0        0        0    17927 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/packaging_classic.md
+-rw-r--r--   0        0        0     9182 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/packaging_simple.md
+-rw-r--r--   0        0        0    14552 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/pytest.md
+-rw-r--r--   0        0        0      932 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/repo_review.md
+-rw-r--r--   0        0        0    28595 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/style.md
+-rw-r--r--   0        0        0     8853 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/tasks.md
+-rw-r--r--   0        0        0     5310 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/writing-docs.md
+-rw-r--r--   0        0        0     7027 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/patterns/data_files.md
+-rw-r--r--   0        0        0      517 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/patterns/index.md
+-rw-r--r--   0        0        0    11200 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/principles/design.md
+-rw-r--r--   0        0        0      561 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/principles/index.md
+-rw-r--r--   0        0        0     2209 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/principles/process.md
+-rw-r--r--   0        0        0     4816 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/tutorials/dev-environment.md
+-rw-r--r--   0        0        0      998 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/tutorials/index.md
+-rw-r--r--   0        0        0     2557 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/tutorials/module.md
+-rw-r--r--   0        0        0     3272 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/tutorials/packaging.md
+-rw-r--r--   0        0        0     4621 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/tutorials/test.md
+-rw-r--r--   0        0        0     1063 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      168 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/hooks/pre_gen_project.py
+-rw-r--r--   0        0        0      228 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/__init__.py
+-rw-r--r--   0        0        0      166 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/_version.py
+-rw-r--r--   0        0        0      118 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/_version.pyi
+-rw-r--r--   0        0        0      753 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/families.py
+-rw-r--r--   0        0        0        0 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/py.typed
+-rw-r--r--   0        0        0        0 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/_compat/__init__.py
+-rw-r--r--   0        0        0      233 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/_compat/tomllib.py
+-rw-r--r--   0        0        0        0 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/_compat/importlib/resources/__init__.py
+-rw-r--r--   0        0        0      256 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/_compat/importlib/resources/abc.py
+-rw-r--r--   0        0        0      290 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/checks/__init__.py
+-rw-r--r--   0        0        0     2849 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/checks/general.py
+-rw-r--r--   0        0        0     5018 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/checks/github.py
+-rw-r--r--   0        0        0     4133 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/checks/mypy.py
+-rw-r--r--   0        0        0     3162 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/checks/precommit.py
+-rw-r--r--   0        0        0     5339 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/checks/pyproject.py
+-rw-r--r--   0        0        0     2868 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/checks/ruff.py
+-rw-r--r--   0        0        0      412 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/tests/test_cmd.py
+-rw-r--r--   0        0        0      597 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/tests/test_package.py
+-rw-r--r--   0        0        0      125 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.git_archival.txt
+-rw-r--r--   0        0        0       32 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.gitattributes
+-rw-r--r--   0        0        0     2218 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.gitignore
+-rw-r--r--   0        0        0     2930 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      456 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.readthedocs.yml
+-rw-r--r--   0        0        0      280 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/CMakeLists-skbuild.txt
+-rw-r--r--   0        0        0      685 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/Cargo-maturin.toml
+-rw-r--r--   0        0        0    14162 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/LICENSE
+-rw-r--r--   0        0        0      123 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/MANIFEST-setuptools,pybind11.in
+-rw-r--r--   0        0        0     1910 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/README.md
+-rw-r--r--   0        0        0      909 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/meson-mesonpy.build
+-rw-r--r--   0        0        0     2312 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/noxfile.py
+-rw-r--r--   0        0        0     8580 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/pyproject.toml
+-rw-r--r--   0        0        0      723 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/setup-pybind11.py
+-rw-r--r--   0        0        0     1980 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/setup-setuptools,pybind11.cfg
+-rw-r--r--   0        0        0      374 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/setup-setuptools.py
+-rw-r--r--   0        0        0     2533 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      163 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     3414 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1573 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/workflows/wheels-pybind11,skbuild,mesonpy,maturin.yml
+-rw-r--r--   0        0        0     2031 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/docs/conf.py
+-rw-r--r--   0        0        0      286 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/docs/index.rst
+-rw-r--r--   0        0        0      562 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/lib-maturin.rs
+-rw-r--r--   0        0        0      632 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/main-pybind11,skbuild,mesonpy.cpp
+-rw-r--r--   0        0        0      430 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/{{cookiecutter.project_slug}}/__init__.py
+-rw-r--r--   0        0        0      117 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/{{cookiecutter.project_slug}}/_core-pybind11,skbuild,mesonpy,maturin.pyi
+-rw-r--r--   0        0        0      118 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/{{cookiecutter.project_slug}}/_version-setuptools,pybind11.pyi
+-rw-r--r--   0        0        0        0 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/{{cookiecutter.project_slug}}/py.typed
+-rw-r--r--   0        0        0      213 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/{{cookiecutter.project_slug}}/_compat/__init__.py
+-rw-r--r--   0        0        0      498 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/{{cookiecutter.project_slug}}/_compat/typing.py
+-rw-r--r--   0        0        0      188 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/tests/test_compiled-pybind11,skbuild,mesonpy,maturin.py
+-rw-r--r--   0        0        0      431 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/tests/test_package.py
+-rw-r--r--   0        0        0     2248 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.gitignore
+-rw-r--r--   0        0        0     1525 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/LICENSE
+-rw-r--r--   0        0        0     2375 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/README-rr.md
+-rw-r--r--   0        0        0     5180 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/pyproject.toml
+-rw-r--r--   0        0        0     3894 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/PKG-INFO
```

### Comparing `sp_repo_review-2023.6.17/.pre-commit-config.yaml` & `sp_repo_review-2023.6.7/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
       - id: rst-directive-colons
       - id: rst-inline-touching-normal
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.3.0
     hooks:
       - id: mypy
-        files: "(src|tests)"
+        files: "(src|web|tests)"
         args: []
         additional_dependencies:
           - click
           - markdown-it-py
           - pytest
           - repo-review
           - rich
```

### Comparing `sp_repo_review-2023.6.17/.readthedocs.yml` & `sp_repo_review-2023.6.7/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/Gemfile` & `sp_repo_review-2023.6.7/Gemfile`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/Gemfile.lock` & `sp_repo_review-2023.6.7/Gemfile.lock`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/README.md` & `sp_repo_review-2023.6.7/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -3,106 +3,81 @@
 [![Actions Status][actions-badge]][actions-link]
 [![GitHub Discussion][github-discussions-badge]][github-discussions-link]
 [![Live ReadTheDocs][rtd-badge]][rtd-link]
 
 [![PyPI version][pypi-version]][pypi-link]
 [![PyPI platforms][pypi-platforms]][pypi-link]
 
-A [copier][]/[cookiecutter][] template for new Python projects based on the
-Scientific Python Developer Guide. What makes this different from other
-templates for Python packages?
+A cookiecutter template for new Python projects based on the Scientific Python
+Developer Guide. What makes this different from other cookie cutter templates
+for Python packages?
 
 - Lives with the [Scientific-Python Development Guide][]: Every decision is
-  clearly documented and every tool described, and everything is kept in sync.
+  clearly documented and every tool described.
 - Twelve different backends to choose from for building packages.
 - Template generation tested in GitHub Actions using nox.
-- Supports generation with both [copier][] and [cookiecutter][].
-- Includes several compiled backends using [pybind11][], with wheels produced
-  for all platforms using [cibuildwheel][].
+- Includes several compiled backends using pybind11, with wheels produced for
+  all platforms using cibuildwheel.
+- Follows PyPA best practices and regularly updated.
 - Provides [`sp-repo-review`][pypi-link] to evaluate existing repos against the
   guidelines, with a WebAssembly version integrated with the guide. All checks
   cross-linked.
-- Follows [PyPA][] best practices and regularly updated.
 
 Be sure you have read the [Scientific-Python Development Guide][] first, and
 possibly used them on a project or two. This is _not_ a minimal example or
 tutorial. It is a collection of useful tooling for starting a new project using
 cookiecutter, or for copying in individual files for an existing project (by
 hand, from `{{cookiecutter.project_name}}/`).
 
 During generation you can select from the following backends for your package:
 
 1. [hatch][]: This uses hatchling, a modern builder with nice file inclusion,
    extendable via plugins, and good error messages. **(Recommended for pure
    Python projects)**
-2. [flit][]: A modern, lightweight [PEP 621][] build system for pure Python
+2. [setuptools][]: The classic build system. Most powerful, but high learning
+   curve and lots of configuration required.
+3. [setuptools621][setuptools]: The classic build system, but with the new
+   standardized configuration. Python 3.7+.
+4. [pybind11][]: This is setuptools but with an C++ extension written in
+   [pybind11][] and wheels generated by [cibuildwheel][].
+5. [scikit-build][]: A scikit-build (CMake) project also using pybind11, using
+   scikit-build-core. **(Recommended for C++ projects)**
+6. [meson-python][]: A Meson project also using pybind11.
+7. [poetry][]: An all-in-one solution to pure Python projects. Replaces
+   setuptools, venv/pipenv, pip, wheel, and twine. Higher learning curve, but is
+   all-in-one. Makes some bad default assumptions for libraries.
+8. [flit][]: A modern, lightweight [PEP 621][] build system for pure Python
    projects. Replaces setuptools, no MANIFEST.in, setup.py, or setup.cfg. Low
    learning curve. Easy to bootstrap into new distributions. Difficult to get
    the right files included, little dynamic metadata support.
-3. [pdm][]: A modern, less opinionated all-in-one solution to pure Python
+9. [pdm][]: A modern, less opinionated all-in-one solution to pure Python
    projects supporting standards. Replaces setuptools, venv/pipenv, pip, wheel,
    and twine. Supports [PEP 621][].
-4. [trampolim][]: A modern [PEP 621][] builder with support for tasks, allowing
-   arbitrary Python to run during the build process if needed.
-5. [whey][]: A modern [PEP 621][] builder with some automation options for Trove
-   classifiers. Development seems to be stalled, possibly.
-6. [poetry][]: An all-in-one solution to pure Python projects. Replaces
-   setuptools, venv/pipenv, pip, wheel, and twine. Higher learning curve, but is
-   all-in-one. Makes some bad default assumptions for libraries. The only one
-   with a non-standard pyproject.toml config.
-7. [setuptools621][setuptools]: The classic build system, but with the new
-   standardized configuration. Python 3.7+.
-8. [setuptools][]: The classic build system. Most powerful, but high learning
-   curve and lots of configuration required.
-9. [pybind11][]: This is setuptools but with an C++ extension written in
-   [pybind11][] and wheels generated by [cibuildwheel][].
-10. [scikit-build][]: A scikit-build (CMake) project also using pybind11, using
-    scikit-build-core. **(Recommended for C++ projects)**
-11. [meson-python][]: A Meson project also using pybind11.
+10. [trampolim][]: A modern [PEP 621][] builder with support for tasks, allowing
+    arbitrary Python to run during the build process if needed.
+11. [whey][]: A modern [PEP 621][] builder with some automation options for
+    Trove classifiers. Development seems to be stalled, possibly.
 12. [maturin][]: A [PEP 621][] builder for Rust binary extensions.
     **(Recommended for Rust projects)**
 
 Currently, the best choice is probably hatch for pure Python projects, and
 setuptools (such as the pybind11 choice) for binary projects.
 
-#### To use (modern copier version)
-
-Install `copier` and `copier-templates-extensions`. Using [pipx][], that's:
-
-```bash
-pipx install copier
-pipx inject copier copier-templates-extensions
-```
-
-Now, run copier to generate your project:
-
-```bash
-copier copy gh:scientific-python/cookie <pkg> --UNSAFE --vcs-ref=HEAD
-```
-
-(`<pkg>` is the path to put the new project.)
-
-You will get a much, much nicer CLI experience with helpful descriptions and
-answer validation. You will also get a `.copier-answers.yml` file, which will
-allow you to perform updates in the future.
-
-> Note: Add `--vcs-ref=HEAD` to get the latest version instead of the last
-> tagged version; this is required until there's a tagged version, and still
-> recommended after that.
-
-#### To use (classic cookiecutter version)
+#### To use:
 
 Install cookiecutter, ideally with `brew install cookiecutter` if you use brew,
 otherwise with `pipx install cookiecutter` (or prepend `pipx run` to the command
 below, and skip installation). Then run:
 
 ```bash
 cookiecutter gh:scientific-python/cookie
 ```
 
+You can also use `pipx run cookiecutter` without installing.
+
 Check the key setup files, `pyproject.toml`, and possibly `setup.cfg` and
 `setup.py` (pybind11 example). Update README.md. Also update and add docs to
 `docs/`.
 
 There are a few example dependencies and a minimum Python version of 3.7, feel
 free to change it to whatever you actually need/want.
 
@@ -146,14 +121,17 @@
 
 You can test locally with [nox][]:
 
 ```console
 # See all commands
 nox -l
 
+# Run all tests and checks (takes several minutes)
+nox
+
 # Run a specific check
 nox -s "lint(setuptools)"
 
 # Run a noxfile command on the project noxfile
 nox -s "nox(whey)" -- docs
 ```
 
@@ -171,45 +149,40 @@
 projects. It currently dumps all development dependencies into a shared
 environment, causing long solve times and high chance of conflicts. It also does
 not use pre-commit properly. It also has quite a bit of custom code.
 
 #### History
 
 A lot of the guide, cookiecutter, and repo-review started out as part of
-[Scikit-HEP][]. These projects were merged, generalized, and combined with the
-[NSLS-II][] guide during the 2023 Scientific-Python Developers Summit.
+Scikit-HEP. These projects were merged, generalized, and combined with the
+NSLS-II guide during the 2023 Scientific-Python Developers Summit.
 
 <!-- prettier-ignore-start -->
 
-[actions-badge]: https://github.com/scientific-python/cookie/workflows/CI/badge.svg
-[actions-link]: https://github.com/scientific-python/cookie/actions
-[cibuildwheel]: https://cibuildwheel.readthedocs.io
-[cookiecutter]: https://cookiecutter.readthedocs.io
-[copier]: https://copier.readthedocs.io
+[actions-badge]: https://github.com/scikit-hep/cookie/workflows/CI/badge.svg
+[actions-link]: https://github.com/scikit-hep/cookie/actions
+[cibuildwheel]: https://cibuildwheel.readthedocs.io/en/stable/
 [flit]: https://flit.readthedocs.io/en/latest/
 [github-discussions-badge]: https://img.shields.io/static/v1?label=Discussions&message=Ask&color=blue&logo=github
-[github-discussions-link]: https://github.com/scientific-python/cookie/discussions
+[github-discussions-link]: https://github.com/scikit-hep/cookie/discussions
 [hatch]: https://github.com/ofek/hatch
 [hypermodern]: https://github.com/cjolowicz/cookiecutter-hypermodern-python
 [maturin]: https://maturin.rs
 [meson-python]: https://meson-python.readthedocs.io
 [nox]: https://nox.thea.codes/en/stable/
-[nsls-ii]: https://nsls-ii.github.io/scientific-python-cookiecutter/
 [pdm]: https://pdm.fming.dev
 [pep 621]: https://www.python.org/dev/peps/pep-0621
 [pipx]: https://pypa.github.io/pipx/
 [poetry]: https://python-poetry.org
-[pybind11]: https://pybind11.readthedocs.io
-[pypa]: https://www.pypa.io
+[pybind11]: https://pybind11.readthedocs.io/en/stable/
 [pypi-link]: https://pypi.org/project/sp-repo-review/
 [pypi-platforms]: https://img.shields.io/pypi/pyversions/sp-repo-review
 [pypi-version]: https://badge.fury.io/py/sp-repo-review.svg
 [rtd-badge]: https://readthedocs.org/projects/scientific-python-cookie/badge/?version=latest
 [rtd-link]: https://scientific-python-cookie.readthedocs.io/en/latest/?badge=latest
 [scientific-python development guide]: https://learn.scientific-python.org/development
-[scikit-build]: https://scikit-build.readthedocs.io
-[scikit-hep]: https://scikit-hep.org
-[setuptools]: https://setuptools.readthedocs.io
-[trampolim]: https://trampolim.readthedocs.io
-[whey]: https://whey.readthedocs.io
+[scikit-build]: https://scikit-build.readthedocs.io/en/latest/
+[setuptools]: https://setuptools.readthedocs.io/en/latest/
+[trampolim]: https://trampolim.readthedocs.io/en/latest/
+[whey]: https://whey.readthedocs.io/en/latest/
 
 <!-- prettier-ignore-end -->
```

### Comparing `sp_repo_review-2023.6.17/_config.yml` & `sp_repo_review-2023.6.7/_config.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/action.yml` & `sp_repo_review-2023.6.7/action.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/cookiecutter.json` & `sp_repo_review-2023.6.7/cookiecutter.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5333333333333333%*

 * *Differences: {"'project_type'": "['hatch', 'setuptools', 'setuptools621', 'pybind11', 'skbuild', 'mesonpy', "*

 * *                   "'poetry', 'flit', 'pdm', 'trampolim', 'whey', 'maturin']",*

 * * "'year'": '"{% now \'utc\', \'%Y\' %}"',*

 * * 'delete': "['backend', '__year', '__project_slug', '__type', '__answers']"}*

```diff
@@ -1,34 +1,31 @@
 {
-    "__answers": "",
-    "__project_slug": "{{ cookiecutter.project_name | lower | replace('-', '_') | replace('.', '_') }}",
-    "__type": "{{ 'compiled' if cookiecutter.backend in ['pybind11', 'skbuild', 'mesonpy', 'maturin'] else 'pure' }}",
-    "__year": "{% now 'utc', '%Y' %}",
     "_extensions": [
         "jinja2_time.TimeExtension"
     ],
-    "backend": [
-        "hatch",
-        "flit",
-        "pdm",
-        "trampolim",
-        "whey",
-        "poetry",
-        "setuptools621",
-        "setuptools",
-        "pybind11",
-        "skbuild",
-        "mesonpy",
-        "maturin"
-    ],
     "email": "me@email.com",
     "full_name": "My Name",
     "license": [
         "BSD",
         "Apache",
         "MIT"
     ],
     "org": "org",
     "project_name": "package",
     "project_short_description": "A great package.",
-    "url": "https://github.com/{{ cookiecutter.org }}/{{ cookiecutter.project_name }}"
+    "project_type": [
+        "hatch",
+        "setuptools",
+        "setuptools621",
+        "pybind11",
+        "skbuild",
+        "mesonpy",
+        "poetry",
+        "flit",
+        "pdm",
+        "trampolim",
+        "whey",
+        "maturin"
+    ],
+    "url": "https://github.com/{{ cookiecutter.org }}/{{ cookiecutter.project_name }}",
+    "year": "{% now 'utc', '%Y' %}"
 }
```

### Comparing `sp_repo_review-2023.6.17/noxfile.py` & `sp_repo_review-2023.6.7/noxfile.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,138 +3,74 @@
 
 sp-repo-review checks start with "rr-".
 """
 
 
 from __future__ import annotations
 
-import difflib
 import json
 import re
 import shutil
-import sys
 import urllib.request
 from pathlib import Path
 
 import nox
 
 nox.needs_version = ">=2022.1.7"
 
 DIR = Path(__file__).parent.resolve()
 with DIR.joinpath("cookiecutter.json").open() as f:
-    BACKENDS = json.load(f)["backend"]
+    BACKENDS = json.load(f)["project_type"]
 
 JOB_FILE = """\
 default_context:
   project_name: cookie-{backend}
-  backend: {backend}
+  project_type: {backend}
 """
 
 nox.options.sessions = ["lint", "tests", "native"]
 
 
-def make_copier(session: nox.Session, backend: str) -> None:
-    package_dir = Path(f"copy-{backend}")
-    if package_dir.exists():
-        shutil.rmtree(package_dir)
-
-    session.run(
-        "copier",
-        "copy",
-        f"{DIR}",
-        f"{package_dir}",
-        "--defaults",
-        "--UNSAFE",
-        "--vcs-ref=HEAD",
-        f"--data=project_name=cookie-{backend}",
-        "--data=org=org",
-        f"--data=backend={backend}",
-        "--data=full_name=My Name",
-        "--data=email=me@email.com",
-        "--data=license=BSD",
-    )
-
-    init_git(session, package_dir)
-
-    return package_dir
-
-
 def make_cookie(session: nox.Session, backend: str) -> None:
+    tmp_dir = session.create_tmp()
+    session.cd(tmp_dir)
+
     package_dir = Path(f"cookie-{backend}")
-    if package_dir.exists():
-        shutil.rmtree(package_dir)
 
     Path("input.yml").write_text(JOB_FILE.format(backend=backend), encoding="utf-8")
 
     session.run(
         "cookiecutter",
         "--no-input",
-        f"{DIR}",
+        str(DIR),
         "--config-file=input.yml",
     )
-
-    init_git(session, package_dir)
-
-    return package_dir
-
-
-def init_git(session: nox.Session, package_dir: Path) -> None:
-    session.run("git", "-C", f"{package_dir}", "init", "-q", external=True)
-    session.run("git", "-C", f"{package_dir}", "add", ".", external=True)
+    session.cd(package_dir)
+    session.run("git", "init", "-q", external=True)
+    session.run("git", "add", ".", external=True)
     session.run(
         "git",
-        "-C",
-        f"{package_dir}",
         "-c",
         "user.name=Bot",
         "-c",
         "user.email=bot@scikit-hep.org",
         "commit",
         "-qm",
         "feat: initial version",
         external=True,
     )
-    session.run("git", "-C", f"{package_dir}", "tag", "v0.1.0", external=True)
-
-
-def valid_path(path: Path):
-    return path.is_file() and not {"__pycache__", ".git", ".copier-answers.yml"} & set(
-        path.parts
-    )
-
-
-def diff_files(p1: Path, p2: Path) -> bool:
-    f1set = {p.relative_to(p1) for p in p1.rglob("*") if valid_path(p)}
-    f2set = {p.relative_to(p2) for p in p2.rglob("*") if valid_path(p)}
-
-    same = True
-
-    for f in sorted(f1set | f2set):
-        f1 = p1 / f
-        f2 = p2 / f
-        with f1.open(encoding="utf-8") as c1, f2.open(encoding="utf-8") as c2:
-            diff = list(
-                difflib.unified_diff(c1.readlines(), c2.readlines(), f"{f1}", f"{f2}")
-            )
-        if diff:
-            sys.stdout.writelines(diff)
-            same = False
-
-    return same
+    session.run("git", "tag", "v0.1.0", external=True)
 
 
 @nox.session()
 @nox.parametrize("backend", BACKENDS, ids=BACKENDS)
 def lint(session: nox.Session, backend: str) -> None:
     session.install("cookiecutter", "pre-commit")
 
-    tmp_dir = session.create_tmp()
-    session.cd(tmp_dir)
-    cookie = make_cookie(session, backend)
-    session.chdir(cookie)
+    make_cookie(session, backend)
 
     session.run(
         "pre-commit",
         "run",
         "--all-files",
         "--hook-stage=manual",
         "--show-diff-on-failure",
@@ -142,106 +78,74 @@
 
 
 @nox.session
 @nox.parametrize("backend", BACKENDS, ids=BACKENDS)
 def autoupdate(session, backend):
     session.install("cookiecutter", "pre-commit")
 
-    tmp_dir = session.create_tmp()
-    session.cd(tmp_dir)
-    cookie = make_cookie(session, backend)
-    session.chdir(cookie)
+    make_cookie(session, backend)
 
     session.run("pre-commit", "autoupdate")
     session.run("git", "diff", "--exit-code", external=True)
 
 
 @nox.session()
 @nox.parametrize("backend", BACKENDS, ids=BACKENDS)
 def tests(session, backend):
     session.install("cookiecutter")
 
-    tmp_dir = session.create_tmp()
-    session.cd(tmp_dir)
-    cookie = make_cookie(session, backend)
-    session.chdir(cookie)
+    make_cookie(session, backend)
 
     session.install(".[test]")
     session.run("python", "-m", "pytest", "-ra")
 
 
 @nox.session()
-def compare(session):
-    session.install("cookiecutter", "copier", "copier-templates-extensions")
-
-    tmp_dir = session.create_tmp()
-    session.cd(tmp_dir)
-
-    for backend in BACKENDS:
-        cookie = make_cookie(session, backend)
-        copier = make_copier(session, backend)
-
-        if diff_files(cookie, copier):
-            session.log(f"{backend} passed")
-        else:
-            session.error(f"{backend} files are not the same!")
-
-
-@nox.session()
 @nox.parametrize("backend", ("poetry", "pdm", "hatch"), ids=("poetry", "pdm", "hatch"))
 def native(session, backend):
     session.install("cookiecutter", backend)
 
-    tmp_dir = session.create_tmp()
-    session.cd(tmp_dir)
-    cookie = make_cookie(session, backend)
-    session.chdir(cookie)
+    make_cookie(session, backend)
 
     if backend == "hatch":
         session.run(backend, "env", "create")
     else:
         session.run(backend, "install")
 
     session.run(backend, "run", "pytest")
 
 
 @nox.session()
 @nox.parametrize("backend", BACKENDS, ids=BACKENDS)
 def dist(session, backend):
     session.install("cookiecutter", "build", "twine")
 
-    tmp_dir = session.create_tmp()
-    session.cd(tmp_dir)
-    cookie = make_cookie(session, backend)
-    session.chdir(cookie)
+    make_cookie(session, backend)
 
     session.run("python", "-m", "build", silent=True)
     (sdist,) = Path("dist").glob("*.tar.gz")
     (wheel,) = Path("dist").glob("*.whl")
 
     if "0.1.0" not in str(wheel):
         session.error(f"{wheel} must be version 0.1.0")
 
-    session.run("twine", "check", f"{sdist}", f"{wheel}")
+    session.run("twine", "check", str(sdist), str(wheel))
 
     dist = DIR / "dist"
     dist.mkdir(exist_ok=True)
     sdist.rename(dist / sdist.stem)
     wheel.rename(dist / wheel.stem)
 
 
 @nox.session(name="nox")
 @nox.parametrize("backend", BACKENDS, ids=BACKENDS)
 def nox_session(session, backend):
     session.install("cookiecutter", "nox")
 
-    tmp_dir = session.create_tmp()
-    session.cd(tmp_dir)
-    cookie = make_cookie(session, backend)
-    session.chdir(cookie)
+    make_cookie(session, backend)
 
     if session.posargs:
         session.run("nox", "-s", *session.posargs)
     else:
         session.run("nox")
```

### Comparing `sp_repo_review-2023.6.17/.devcontainer/devcontainer.json` & `sp_repo_review-2023.6.7/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/.github/workflows/cd.yml` & `sp_repo_review-2023.6.7/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/.github/workflows/ci.yml` & `sp_repo_review-2023.6.7/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/.github/workflows/reusable-change-detection.yml` & `sp_repo_review-2023.6.7/.github/workflows/reusable-change-detection.yml`

 * *Files 11% similar despite different names*

```diff
@@ -3,59 +3,57 @@
   workflow_call:
     outputs:
       run-cookie:
         description: Whether or not run the cookiecutter tests
         value: ${{ jobs.change-detection.outputs.run-cookie || false }}
       run-rr:
         description: Whether or not run the repo-review tests
-        value: ${{ jobs.change-detection.outputs.run-rr || false }}
+        value: ${{ jobs.change-detection.outputs.run-cookie || false }}
 
 jobs:
   change-detection:
     name: Identify source changes
     runs-on: ubuntu-latest
     timeout-minutes: 1
     outputs:
       run-cookie: ${{ steps.cookie-changes.outputs.run-cookie || false }}
       run-rr: ${{ steps.rr-changes.outputs.run-rr || false }}
     steps:
       - uses: actions/checkout@v3
 
-      - name: Changed cookie-related files
+      - name: Get a list of the changed runtime-related files
         if: github.event_name == 'pull_request'
         id: changed-cookie-files
         uses: Ana06/get-changed-files@v2.2.0
         with:
-          format: "json"
           filter: |
             {{cookiecutter.project_name}}/**
             .github/workflows/ci.yml
             .github/workflows/reusable-cookie.yml
             noxfile.py
             hooks/**
             cookiecutter.json
       - name: Set a flag for running the tests
         if: >-
           github.event_name != 'pull_request' ||
-          steps.changed-cookie-files.outputs.added_modified_renamed != '[]'
+          steps.changed-cookie-files.outputs.added_modified_renamed != ''
         id: cookie-changes
         run: echo "run-cookie=true" >> "${GITHUB_OUTPUT}"
 
-      - name: Changed sp-repo-review-related files
+      - name: Get a list of the changed runtime-related files
         if: github.event_name == 'pull_request'
         id: changed-rr-files
         uses: Ana06/get-changed-files@v2.2.0
         with:
-          format: "json"
           filter: |
             tests/**
             .github/workflows/ci.yml
             .github/workflows/reusable-rr-tests.yml
             noxfile.py
             src/**
             pyproject.toml
       - name: Set a flag for running the tests
         if: >-
           github.event_name != 'pull_request' ||
-          steps.changed-rr-files.outputs.added_modified_renamed != '[]'
+          steps.changed-rr-files.outputs.added_modified_renamed != ''
         id: rr-changes
         run: echo "run-rr=true" >> "${GITHUB_OUTPUT}"
```

### Comparing `sp_repo_review-2023.6.17/.github/workflows/reusable-cookie.yml` & `sp_repo_review-2023.6.7/.github/workflows/reusable-cookie.yml`

 * *Files 1% similar despite different names*

```diff
@@ -51,28 +51,27 @@
 
   checks:
     name: Check Python ${{ matrix.python-version }} on ${{ matrix.runs-on }}
     runs-on: ${{ matrix.runs-on }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.7", "3.12"]
+        python-version: ["3.7", "3.11", "3.12-dev"]
         runs-on: [ubuntu-latest, macos-latest, windows-latest]
 
         include:
           - python-version: pypy-3.8
             runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
 
       - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
-          allow-prereleases: true
 
       - name: Install nox
         run: pip install nox
 
       - name: Test setuptools
         run: nox -s 'tests(setuptools)'
 
@@ -116,17 +115,14 @@
       - name: Activate MSVC for Meson
         if: runner.os == 'Windows'
         uses: ilammy/msvc-dev-cmd@v1
 
       - name: Test meson-python
         run: nox -s 'tests(mesonpy)'
 
-      - name: Compare template generation
-        run: nox -s compare
-
   nox:
     name: Check included Noxfile
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
```

### Comparing `sp_repo_review-2023.6.17/.github/workflows/reusable-rr-tests.yml` & `sp_repo_review-2023.6.7/.github/workflows/reusable-rr-tests.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/docs/README.md` & `sp_repo_review-2023.6.7/docs/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # Scientific Python Library Development Guide
 
 This is maintained by the scientific Python community for the benefit of fellow
 scientists and research software engineers. The repository contains:
 
 - A guide
-- A copier/cookiecutter template that generates a template for a scientific
-  Python library
-- sp-repo-review, a plugin for [repo-review](https://repo-review.readthedocs.io)
+- A cookiecutter that generates a template for a scientific Python library
 
 ## Contributing to the documentation
 
 To build locally, install rbenv (remember to run `rbenv init` after installing,
 and `rbenv install 3.1.2`). Then:
 
 ```bash
```

### Comparing `sp_repo_review-2023.6.17/docs/_includes/head.html` & `sp_repo_review-2023.6.7/docs/_includes/head.html`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/docs/_includes/head_custom.html` & `sp_repo_review-2023.6.7/docs/_includes/head_custom.html`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/docs/_includes/interactive_repo_review.html` & `sp_repo_review-2023.6.7/docs/_includes/interactive_repo_review.html`

 * *Files 2% similar despite different names*

```diff
@@ -15,11 +15,11 @@
 <script type="text/babel">
   const root = ReactDOM.createRoot(
     document.getElementById("interactive-repo-review-root")
   );
   root.render(
     <App
       header={false}
-      deps={["sp_repo_review==2023.06.07", "repo-review==0.7.0"]}
+      deps={["sp_repo_review==2023.06.01", "repo-review==0.7.0b8"]}
     />
   );
 </script>
```

### Comparing `sp_repo_review-2023.6.17/docs/_sass/custom/custom.scss` & `sp_repo_review-2023.6.7/docs/_sass/custom/custom.scss`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/docs/assets/favicon.ico` & `sp_repo_review-2023.6.7/docs/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/docs/assets/images/logo.svg` & `sp_repo_review-2023.6.7/docs/assets/images/logo.svg`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/docs/assets/js/tabs.js` & `sp_repo_review-2023.6.7/docs/assets/js/tabs.js`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/docs/assets/js/webapp.js` & `sp_repo_review-2023.6.7/docs/assets/js/webapp.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -272,15 +272,15 @@
         /MaterialUI.ThemeProvider>
     );
 }
 
 class App extends React.Component {
     constructor(props) {
         super(props);
-        const deps_str = props.deps.join(" ");
+        const deps_str = props.deps.map((i) => `"${i}"`).join(", ");
         this.state = {
             results: [],
             repo: urlParams.get("repo") || "",
             branch: urlParams.get("branch") || "",
             msg: `${DEFAULT_MSG} Packages: ${deps_str}`,
             progress: false,
             err_msg: "",
@@ -352,15 +352,15 @@
             }
             console.log(families);
             for (const val of results_list) {
                 results[val.family].push({
                     name: val.name.toString(),
                     description: val.description.toString(),
                     state: val.result,
-                    err_msg: val.err_as_html().toString(),
+                    err_msg: val.err_markdown().toString(),
                     url: val.url.toString(),
                 });
             }
 
             this.setState({
                 results: results,
                 families: families,
```

### Comparing `sp_repo_review-2023.6.17/docs/pages/index.md` & `sp_repo_review-2023.6.7/docs/pages/index.md`

 * *Files 8% similar despite different names*

```diff
@@ -16,18 +16,17 @@
 maintainable, reusable, and shareable form? Start at the
 [tutorial]({% link pages/tutorials/index.md %}).
 
 **Learn recommended tools and best practices.** [Topical
 guides]({% link pages/guides/index.md %}) provide task-based instruction on
 topics that scientists and research software engineers may encounter as their
 projects evolve and grow. This covers everything from writing and building
-documentation to modern Python packaging. This comes with a
-[copier][]/[cookiecutter][] template for making new repos,
-[scientific-python/cookie][], and [sp-repo-review][], a tool for comparing your
-repository with the guidelines, runnable in WebAssembly.
+documentation to modern Python packaging. This comes with a cookiecutter for
+making new repos, [scientific-python/cookie][], and [sp-repo-review][], a tool
+for comparing your repository with the guidelines, runnable in WebAssembly.
 
 **Learn to write better research code.** A high-level document on
 [principles]({% link pages/principles/index.md %}) provides advice based on the
 community's collective experience building code that is easier for researchers
 to use successfully and easier to maintain over time.
 
 **Use our solutions for common tasks.** A growing collection of
@@ -43,10 +42,8 @@
 This guide also does not cover version control, but it is essential to have a
 basic facility with git to use these tools successfully. We recommend the
 [Software Carpentry lesson on git](https://swcarpentry.github.io/git-novice/).
 
 <!-- prettier-ignore-start -->
 [scientific-python/cookie]: https://github.com/scientific-python/cookie
 [sp-repo-review]: {% link pages/guides/repo_review.md %}
-[copier]: https://copier.readthedocs.io
-[cookiecutter]: https://cookiecutter.readthedocs.io
 <!-- prettier-ignore-end -->
```

### Comparing `sp_repo_review-2023.6.17/docs/pages/guides/coverage.md` & `sp_repo_review-2023.6.7/docs/pages/guides/coverage.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/docs/pages/guides/gha_basic.md` & `sp_repo_review-2023.6.7/docs/pages/guides/gha_basic.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/docs/pages/guides/gha_pure.md` & `sp_repo_review-2023.6.7/docs/pages/guides/gha_pure.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/docs/pages/guides/gha_wheels.md` & `sp_repo_review-2023.6.7/docs/pages/guides/gha_wheels.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/docs/pages/guides/index.md` & `sp_repo_review-2023.6.7/docs/pages/guides/index.md`

 * *Files 10% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 a consistent developer and user experience when working with distribution.
 
 A section on CI follows, with a [general setup guide][gha_basic], and then two
 choices for using CI to distribute your package, on for [pure Python][gha_pure],
 and one for [compiled extensions][gha_wheels]. You can read about setting up
 good tests on the [pytest page][pytest].
 
-Once you have completed the guidelines, there is a [copier][]/[cookiecutter][]
-project, [scientific-python/cookie][], that implements these guidelines and lets
-you setup a new package from a template in less than 60 seconds!
+Once you have completed the guidelines, there is a [cookiecutter][] project,
+[scientific-python/cookie][], that implements these guidelines and lets you
+setup a new package from a template in less than 60 seconds!
 
 You can also evaluate your repository against the guidelines by using
 [scientific-python-repo-review][]!
 
 <!-- prettier-ignore-start -->
 
 [tutorials]: {% link pages/tutorials/index.md %}
@@ -41,11 +41,10 @@
 [gha_basic]: {% link pages/guides/gha_basic.md %}
 [gha_pure]: {% link pages/guides/gha_pure.md %}
 [gha_wheels]: {% link pages/guides/gha_wheels.md %}
 [pytest]: {% link pages/guides/pytest.md %}
 [scientific-python-repo-review]: {% link pages/guides/repo_review.md %}
 
 [cookiecutter]: https://cookiecutter.readthedocs.io
-[copier]: https://copier.readthedocs.io
 [scientific-python/cookie]: https://github.com/scientific-python/cookie
 
 <!-- prettier-ignore-end -->
```

### Comparing `sp_repo_review-2023.6.17/docs/pages/guides/mypy.md` & `sp_repo_review-2023.6.7/docs/pages/guides/mypy.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/docs/pages/guides/packaging_classic.md` & `sp_repo_review-2023.6.7/docs/pages/guides/packaging_classic.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/docs/pages/guides/packaging_simple.md` & `sp_repo_review-2023.6.7/docs/pages/guides/packaging_simple.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/docs/pages/guides/pytest.md` & `sp_repo_review-2023.6.7/docs/pages/guides/pytest.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/docs/pages/guides/repo_review.md` & `sp_repo_review-2023.6.7/docs/pages/guides/repo_review.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/docs/pages/guides/style.md` & `sp_repo_review-2023.6.7/docs/pages/guides/style.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/docs/pages/guides/tasks.md` & `sp_repo_review-2023.6.7/docs/pages/guides/tasks.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/docs/pages/guides/writing-docs.md` & `sp_repo_review-2023.6.7/docs/pages/guides/writing-docs.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/docs/pages/patterns/data_files.md` & `sp_repo_review-2023.6.7/docs/pages/patterns/data_files.md`

 * *Files 3% similar despite different names*

```diff
@@ -36,17 +36,17 @@
   enough to simulate it accurately, you don't know enough to write useful tests
   against it.
 - Can you write a Python function that fetches the data on demand from some
   public URL? This is the approach used by projects such as scikit-learn that
   need to download large datasets for their examples and tests.
 
 If you use one these alternatives, add the names of the generated or downloaded
-files to the project's `.gitignore` file, which is provided by the
-[copier][]/[cookiecutter][] template. This helps protect you against
-accidentally committing the file to git.
+files to the project's `.gitignore` file, which was provided by the cookiecutter
+template. This helps protect you against accidentally committing the file to
+git.
 
 If the file in question is a text file and not very large (\< 100 kB) than it's
 reasonable to just bundle it with the package. If not, see the recommendation at
 the end.
 
 ## How to Package Data Files
 
@@ -197,15 +197,11 @@
     known_hash="sha256:50ef9a52c621b7c0c506ad1fe1b8ee8a158a4d7c8e50ddfce1e273a422dca3f9",
 )
 ```
 
 On repeated runs of this command, the locally cached filename would be used
 instead of downloading the data again.
 
-<!-- prettier-ignore-start -->
 [importlib_resources]: https://importlib-resources.readthedocs.io/en/latest/
 [osf.io]: https://osf.io/
 [pooch]: https://www.fatiando.org/pooch/latest/
 [zenodo]: https://zenodo.org/
-[copier]: https://copier.readthedocs.io
-[cookiecutter]: https://cookiecutter.readthedocs.io
-<!-- prettier-ignore-end -->
```

### Comparing `sp_repo_review-2023.6.17/docs/pages/patterns/index.md` & `sp_repo_review-2023.6.7/docs/pages/patterns/index.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/docs/pages/principles/design.md` & `sp_repo_review-2023.6.7/docs/pages/principles/design.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/docs/pages/principles/index.md` & `sp_repo_review-2023.6.7/docs/pages/principles/index.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/docs/pages/principles/process.md` & `sp_repo_review-2023.6.7/docs/pages/principles/process.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/docs/pages/tutorials/dev-environment.md` & `sp_repo_review-2023.6.7/docs/pages/tutorials/dev-environment.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/docs/pages/tutorials/index.md` & `sp_repo_review-2023.6.7/docs/pages/tutorials/index.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/docs/pages/tutorials/module.md` & `sp_repo_review-2023.6.7/docs/pages/tutorials/module.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/docs/pages/tutorials/packaging.md` & `sp_repo_review-2023.6.7/docs/pages/tutorials/packaging.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/docs/pages/tutorials/test.md` & `sp_repo_review-2023.6.7/docs/pages/tutorials/test.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/src/sp_repo_review/families.py` & `sp_repo_review-2023.6.7/src/sp_repo_review/families.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/src/sp_repo_review/checks/general.py` & `sp_repo_review-2023.6.7/src/sp_repo_review/checks/general.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/src/sp_repo_review/checks/github.py` & `sp_repo_review-2023.6.7/src/sp_repo_review/checks/github.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/src/sp_repo_review/checks/mypy.py` & `sp_repo_review-2023.6.7/src/sp_repo_review/checks/mypy.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/src/sp_repo_review/checks/precommit.py` & `sp_repo_review-2023.6.7/src/sp_repo_review/checks/precommit.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/src/sp_repo_review/checks/pyproject.py` & `sp_repo_review-2023.6.7/src/sp_repo_review/checks/pyproject.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/src/sp_repo_review/checks/ruff.py` & `sp_repo_review-2023.6.7/src/sp_repo_review/checks/ruff.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/tests/test_package.py` & `sp_repo_review-2023.6.7/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/.gitignore` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.gitignore`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/.pre-commit-config.yaml` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -46,25 +46,25 @@
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
     rev: "v0.0.264"
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
 
-{%- if cookiecutter.backend == "setuptools" or cookiecutter.backend == "pybind11" %}
+{%- if cookiecutter.project_type == "setuptools" or cookiecutter.project_type == "pybind11" %}
 
   - repo: https://github.com/asottile/setup-cfg-fmt
     rev: "v2.2.0"
     hooks:
       - id: setup-cfg-fmt
         args: [--include-version-classifiers, --max-py-version=3.11]
 
 {%- endif %}
 
-{%- if cookiecutter.backend in ["pybind11", "skbuild", "mesonpy"] %}
+{%- if cookiecutter.project_type in ["pybind11", "skbuild", "mesonpy"] %}
 
   - repo: https://github.com/pre-commit/mirrors-clang-format
     rev: "v16.0.2"
     hooks:
       - id: clang-format
         types_or: [c++, c, cuda]
 
@@ -93,24 +93,24 @@
     hooks:
       - id: disallow-caps
         name: Disallow improper capitalization
         language: pygrep
         entry: PyBind|Numpy|Cmake|CCache|Github|PyTest
         exclude: .pre-commit-config.yaml
 
-{%- if cookiecutter.backend in ["setuptools", "pybind11"] %}
+{%- if cookiecutter.project_type in ["setuptools", "pybind11"] %}
 
   - repo: https://github.com/mgedmin/check-manifest
     rev: "0.49"
     hooks:
       - id: check-manifest
         stages: [manual]
 {%- endif %}
 
-{%- if cookiecutter.backend == "skbuild" %}
+{%- if cookiecutter.project_type == "skbuild" %}
 
   - repo: https://github.com/cheshirekow/cmake-format-precommit
     rev: "v0.6.13"
     hooks:
       - id: cmake-format
 
 {%- endif %}
```

### Comparing `sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/LICENSE` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {%- if cookiecutter.license == "BSD" %}
 BSD 3-Clause License
 
-Copyright (c) {{ cookiecutter.__year }}, {{ cookiecutter.full_name }}.
+Copyright (c) {{ cookiecutter.year }}, {{ cookiecutter.full_name }}.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
@@ -214,29 +214,29 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright {{ cookiecutter.__year }} {{ cookiecutter.full_name }}
+   Copyright {{ cookiecutter.year }} {{ cookiecutter.full_name }}
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
 {%- elif cookiecutter.license == "MIT" %}
-Copyright {{ cookiecutter.__year }} {{ cookiecutter.full_name }}
+Copyright {{ cookiecutter.year }} {{ cookiecutter.full_name }}
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
 so, subject to the following conditions:
```

### Comparing `sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/README.md` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/README.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/noxfile.py` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/noxfile.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 import argparse
-{%- if cookiecutter.backend != "pybind11" %}
+{%- if cookiecutter.project_type != "pybind11" %}
 import shutil
 from pathlib import Path
 {%- endif %}
 
 import nox
 
-{% if cookiecutter.backend != "pybind11" -%}
+{% if cookiecutter.project_type != "pybind11" -%}
 DIR = Path(__file__).parent.resolve()
 
 {% endif -%}
 
 nox.options.sessions = ["lint", "pylint", "tests"]
 
 
@@ -79,15 +79,15 @@
         "--no-toc",
         "--force",
         "--module-first",
         "../src/{{ cookiecutter.project_name.replace('-', '_') }}",
     )
 
 
-{%- if cookiecutter.backend != "pybind11" %}
+{%- if cookiecutter.project_type != "pybind11" %}
 
 
 @nox.session
 def build(session: nox.Session) -> None:
     """
     Build an SDist and wheel.
     """
```

### Comparing `sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/pyproject.toml` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,64 +1,64 @@
 [build-system]
-{%- if cookiecutter.backend == "trampolim" %}
+{%- if cookiecutter.project_type == "trampolim" %}
 requires = ["trampolim>=0.1.0"]
 build-backend = "trampolim"
-{%- elif cookiecutter.backend == "whey" %}
+{%- elif cookiecutter.project_type == "whey" %}
 requires = ["whey>=0.0.17"]
 build-backend = "whey"
-{%- elif cookiecutter.backend == "pdm" %}
+{%- elif cookiecutter.project_type == "pdm" %}
 requires = ["pdm-backend"]
 build-backend = "pdm.backend"
-{%- elif cookiecutter.backend == "maturin" %}
+{%- elif cookiecutter.project_type == "maturin" %}
 requires = ["maturin>=0.12,<0.15"]
 build-backend = "maturin"
-{%- elif cookiecutter.backend == "hatch" %}
+{%- elif cookiecutter.project_type == "hatch" %}
 requires = ["hatchling"]
 build-backend = "hatchling.build"
-{%- elif cookiecutter.backend == "setuptools621" %}
+{%- elif cookiecutter.project_type == "setuptools621" %}
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
-{%- elif cookiecutter.backend == "flit" %}
+{%- elif cookiecutter.project_type == "flit" %}
 requires = ["flit_core >=3.4"]
 build-backend = "flit_core.buildapi"
-{%- elif cookiecutter.backend == "setuptools" %}
+{%- elif cookiecutter.project_type == "setuptools" %}
 requires = ["setuptools>=42", "setuptools_scm[toml]>=3.4"]
 build-backend = "setuptools.build_meta"
-{%- elif cookiecutter.backend == "pybind11" %}
+{%- elif cookiecutter.project_type == "pybind11" %}
 requires = ["setuptools>=42", "setuptools_scm[toml]>=3.4", "pybind11"]
 build-backend = "setuptools.build_meta"
-{%- elif cookiecutter.backend == "skbuild"  %}
+{%- elif cookiecutter.project_type == "skbuild"  %}
 requires = ["pybind11", "scikit-build-core"]
 build-backend = "scikit_build_core.build"
-{%- elif cookiecutter.backend == "mesonpy"  %}
+{%- elif cookiecutter.project_type == "mesonpy"  %}
 requires = ["pybind11", "meson-python"]
 build-backend = "mesonpy"
-{%- elif cookiecutter.backend == "poetry" %}
+{%- elif cookiecutter.project_type == "poetry" %}
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 {%- endif %}
 
-{%- if cookiecutter.backend in ["setuptools", "pybind11"] %}
+{%- if cookiecutter.project_type in ["setuptools", "pybind11"] %}
 
 
 [tool.setuptools_scm]
-write_to = "src/{{ cookiecutter.__project_slug }}/_version.py"
+write_to = "src/{{ cookiecutter.project_slug }}/_version.py"
 
 
 [tool.check-manifest]
 ignore = [
   ".github/**",
   "docs/**",
   ".pre-commit-config.yaml",
   ".readthedocs.yml",
   "src/*/_version.py",
   "noxfile.py",
 ]
 
-{%- elif cookiecutter.backend == "poetry" %}
+{%- elif cookiecutter.project_type == "poetry" %}
 
 
 [tool.poetry]
 name = "{{ cookiecutter.project_name }}"
 version = "0.1.0"
 authors = [
   "{{ cookiecutter.full_name }} <{{ cookiecutter.email }}>",
@@ -116,15 +116,15 @@
 
 
 {%- else %}
 
 
 [project]
 name = "{{ cookiecutter.project_name }}"
-{%- if cookiecutter.backend not in ["trampolim", "flit", "hatch"] %}
+{%- if cookiecutter.project_type not in ["trampolim", "flit", "hatch"] %}
 version = "0.1.0"
 {%- endif %}
 authors = [
   { name = "{{ cookiecutter.full_name }}", email = "{{ cookiecutter.email }}" },
 ]
 {%- if cookiecutter.org == "Scikit-HEP" %}
 maintainers = [
@@ -154,15 +154,15 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Scientific/Engineering",
   "Typing :: Typed",
 ]
-{%- if cookiecutter.backend in ["trampolim", "flit", "hatch"] %}
+{%- if cookiecutter.project_type in ["trampolim", "flit", "hatch"] %}
 dynamic = ["version"]
 {%- endif %}
 dependencies = [
   "typing_extensions >=3.7; python_version<'3.8'",
 ]
 
 [project.optional-dependencies]
@@ -186,32 +186,32 @@
 Homepage = "{{ cookiecutter.url }}"
 "Bug Tracker" = "{{ cookiecutter.url }}/issues"
 Discussions = "{{ cookiecutter.url }}/discussions"
 Changelog = "{{ cookiecutter.url }}/releases"
 {%- endif %}
 
 
-{%- if cookiecutter.backend == "skbuild" %}
+{%- if cookiecutter.project_type == "skbuild" %}
 [tool.scikit-build]
 minimum-version = "0.2"
 build-dir = "build/{cache_tag}"
-{%- elif cookiecutter.backend == "whey" %}
+{%- elif cookiecutter.project_type == "whey" %}
 [tool.whey]
 source-dir = "src"
-{%- elif cookiecutter.backend == "trampolim" %}
+{%- elif cookiecutter.project_type == "trampolim" %}
 [tool.trampolim]
 module-location = "src"
-{%- elif cookiecutter.backend == "hatch" %}
+{%- elif cookiecutter.project_type == "hatch" %}
 [tool.hatch]
-version.path = "src/{{ cookiecutter.__project_slug  }}/__init__.py"
+version.path = "src/{{ cookiecutter.project_slug  }}/__init__.py"
 envs.default.dependencies = [
   "pytest",
   "pytest-cov",
 ]
-{%- elif cookiecutter.backend == "pdm" %}
+{%- elif cookiecutter.project_type == "pdm" %}
 [tool.pdm.dev-dependencies]
 devtest = ["pytest", "pytest-cov"]
 {%- endif %}
 
 
 [tool.pytest.ini_options]
 minversion = "6.0"
@@ -224,15 +224,15 @@
 log_cli_level = "INFO"
 testpaths = [
   "tests",
 ]
 
 
 [tool.coverage]
-run.source = ["{{ cookiecutter.__project_slug }}"]
+run.source = ["{{ cookiecutter.project_slug }}"]
 port.exclude_lines = [
   'pragma: no cover',
   '\.\.\.',
   'if typing.TYPE_CHECKING:',
 ]
 
 [tool.mypy]
@@ -243,15 +243,15 @@
 show_error_codes = true
 enable_error_code = ["ignore-without-code", "redundant-expr", "truthy-bool"]
 warn_unreachable = true
 disallow_untyped_defs = false
 disallow_incomplete_defs = false
 
 [[tool.mypy.overrides]]
-module = "{{ cookiecutter.__project_slug  }}.*"
+module = "{{ cookiecutter.project_slug  }}.*"
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
 
 
 [tool.ruff]
 select = [
   "E", "F", "W", # flake8
@@ -279,15 +279,15 @@
   "PD",          # pandas-vet
 ]
 extend-ignore = [
   "PLR",    # Design related pylint codes
   "E501",   # Line too long
 ]
 target-version = "py37"
-typing-modules = ["{{ cookiecutter.__project_slug }}._compat.typing"]
+typing-modules = ["{{ cookiecutter.project_slug }}._compat.typing"]
 src = ["src"]
 unfixable = [
   "T20",  # Removes print statements
   "F841", # Removes unused variables
 ]
 exclude = []
 flake8-unused-arguments.ignore-variadic-names = true
@@ -296,15 +296,15 @@
 [tool.ruff.per-file-ignores]
 "tests/**" = ["T20"]
 "noxfile.py" = ["T20"]
 
 
 [tool.pylint]
 py-version = "3.7"
-ignore-paths= ["src/{{ cookiecutter.__project_slug }}/_version.py"]
+ignore-paths= ["src/{{ cookiecutter.project_slug }}/_version.py"]
 reports.output-format = "colorized"
 similarities.ignore-imports = "yes"
 messages_control.disable = [
   "design",
   "fixme",
   "line-too-long",
   "missing-module-docstring",
```

### Comparing `sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/{% if cookiecutter.backend in ['setuptools','pybind11'] %}setup.cfg{% endif %}` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/setup-setuptools,pybind11.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-name = {{ cookiecutter.__project_slug }}
+name = {{ cookiecutter.project_slug }}
 description = {{ cookiecutter.project_short_description }}
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = {{ cookiecutter.url }}
 author = {{ cookiecutter.full_name }}
 author_email = {{ cookiecutter.email }}
 {%- if cookiecutter.org == "Scikit-HEP" %}
```

### Comparing `sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='maturin' %}Cargo.toml{% endif %}` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/Cargo-maturin.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [package]
-name = "{{ cookiecutter.__project_slug }}"
+name = "{{ cookiecutter.project_slug }}"
 version = "0.1.0"
 edition = "2018"
 
 [lib]
 name = "_core"
 # "cdylib" is necessary to produce a shared library for Python to import from.
 crate-type = ["cdylib"]
 
 [package.metadata.maturin]
-name = "{{ cookiecutter.__project_slug }}._core"
-python-packages = ["{{ cookiecutter.__project_slug }}"]
+name = "{{ cookiecutter.project_slug }}._core"
+python-packages = ["{{ cookiecutter.project_slug }}"]
 python-source = "src"
 
 [dependencies]
 rand = "0.8.3"
 
 [dependencies.pyo3]
 version = "0.18.1"
```

### Comparing `sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='mesonpy' %}meson.build{% endif %}` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/meson-mesonpy.build`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 project(
-  '{{ cookiecutter.__project_slug }}',
+  '{{ cookiecutter.project_slug }}',
   'cpp',
   version: '0.1.0',
   license: '{{ cookiecutter.license }}',
   meson_version: '>= 0.64.0',
   default_options: [
     'buildtype=debugoptimized',
     'cpp_std=c++11',
   ],
 )
-name = '{{ cookiecutter.__project_slug }}'
+name = '{{ cookiecutter.project_slug }}'
 
 py_mod = import('python')
 py = py_mod.find_installation(pure: false)
 
 pybind11_config = find_program('pybind11-config')
 pybind11_config_ret = run_command(pybind11_config, ['--includes'], check: true)
 pybind11 = declare_dependency(
     include_directories: [pybind11_config_ret.stdout().split('-I')[-1].strip()],
 )
 
 install_subdir('src' / name, install_dir: py.get_install_dir() / name, strip_directory: true)
 
 py.extension_module('_core',
     'src/main.cpp',
-    subdir: '{{ cookiecutter.__project_slug }}',
+    subdir: '{{ cookiecutter.project_slug }}',
     install: true,
     dependencies : [pybind11],
     link_language : 'cpp',
     override_options: [
         'cpp_rtti=true',
     ]
 )
```

### Comparing `sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/{% if cookiecutter.backend=='pybind11' %}setup.py{% endif %}` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/setup-pybind11.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) {{ cookiecutter.__year }}, {{ cookiecutter.full_name }}
+# Copyright (c) {{ cookiecutter.year }}, {{ cookiecutter.full_name }}
 #
 # Distributed under the 3-clause BSD license, see accompanying file LICENSE
 # or {{ cookiecutter.url }} for details.
 
 from __future__ import annotations
 
 from setuptools import setup  # isort:skip
@@ -12,15 +12,15 @@
 
 # Note:
 #   Sort input source files if you glob sources to ensure bit-for-bit
 #   reproducible builds (https://github.com/pybind/python_example/pull/53)
 
 ext_modules = [
     Pybind11Extension(
-        "{{ cookiecutter.__project_slug }}._core",
+        "{{ cookiecutter.project_slug }}._core",
         ["src/main.cpp"],
         cxx_std=11,
     ),
 ]
 
 
 setup(
```

### Comparing `sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/.github/CONTRIBUTING.md` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 Nox handles everything for you, including setting up an temporary virtual
 environment for each run.
 
 # Setting up a development environment manually
 
 You can set up a development environment by running:
 
-{% if cookiecutter.backend == "poetry" -%}
+{% if cookiecutter.project_type == "poetry" -%}
 
 ```bash
 poetry install
 ```
 
 {%- else -%}
```

### Comparing `sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/.github/matchers/pylint.json` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/.github/workflows/ci.yml` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/workflows/ci.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{%- set compiled = cookiecutter.backend in ["pybind11", "maturin", "skbuild", "mesonpy"] -%}
+{%- set compiled = cookiecutter.project_type in ["pybind11", "maturin", "skbuild", "mesonpy"] -%}
 name: CI
 
 on:
   workflow_dispatch:
   pull_request:
   push:
     branches:
@@ -60,15 +60,15 @@
         with:
           fetch-depth: 0
 
       - uses: actions/setup-python@v4
         with:
           python-version: {% raw %}${{ matrix.python-version }}{% endraw %}
 
-      {%- if cookiecutter.backend == "mesonpy" %}
+      {%- if cookiecutter.project_type == "mesonpy" %}
       - name: Activate MSVC for Meson
         if: runner.os == 'Windows'
         uses: ilammy/msvc-dev-cmd@v1
       {%- endif %}
 
       - name: Install package
         run: python -m pip install .[test]
@@ -96,15 +96,15 @@
       - name: Build sdist and wheel
         run: pipx run build
 
       - uses: actions/upload-artifact@v3
         with:
           path: dist
 
-      {%- if cookiecutter.backend != "trampolim" %}
+      {%- if cookiecutter.project_type != "trampolim" %}
 
       - name: Check products
         run: pipx run twine check dist/*
 
       {%- endif %}
 
   publish:
@@ -124,13 +124,13 @@
 
       - uses: pypa/gh-action-pypi-publish@release/v1
         if: github.event_name == 'release' && github.event.action == 'published'
         with:
           # Remember to tell (test-)pypi about this repo before publishing
           # Remove this line to publish to PyPI
           repository-url: https://test.pypi.org/legacy/
-          {%- if cookiecutter.backend == "trampolim" %}
+          {%- if cookiecutter.project_type == "trampolim" %}
           # Check not supported currently by twine + trampolim
           verify-metadata: false
           {%- endif %}
 
   {%- endif %}
```

### Comparing `sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/.github/workflows/{% if cookiecutter.__type == 'compiled' %}wheels.yml{% endif %}` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/workflows/wheels-pybind11,skbuild,mesonpy,maturin.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/docs/conf.py` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Warning: do not change the path here. To use autodoc, you need to install the
 # package first.
 
 # -- Project information -----------------------------------------------------
 
 project = "{{ cookiecutter.project_name }}"
-copyright = "{{ cookiecutter.__year }}, {{ cookiecutter.full_name }}"
+copyright = "{{ cookiecutter.year }}, {{ cookiecutter.full_name }}"
 author = "{{ cookiecutter.full_name }}"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
```

### Comparing `sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend in ['pybind11','skbuild','mesonpy'] %}main.cpp{% endif %}` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/main-pybind11,skbuild,mesonpy.cpp`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/{{cookiecutter.project_name}}/src/{% if cookiecutter.backend=='maturin' %}lib.rs{% endif %}` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/lib-maturin.rs`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/.gitignore` & `sp_repo_review-2023.6.7/.gitignore`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/LICENSE` & `sp_repo_review-2023.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.17/README-rr.md` & `sp_repo_review-2023.6.7/README-rr.md`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![GitHub Discussion][github-discussions-badge]][github-discussions-link]
 [![Live ReadTheDocs][rtd-badge]][rtd-link]
 
 [![PyPI version][pypi-version]][pypi-link]
 [![PyPI platforms][pypi-platforms]][pypi-link]
 
 `sp-repo-review` provides checks based on the [Scientific-Python Development
-Guide][] at [scientific-python/cookie][] for [repo-review][].
+Guide][] at [scientific-python/cookie][].
 
 This tool can check the style of a repository. Use like this:
 
 ```bash
 pipx run 'sp-repo-review[cli]' <path to repository>
 ```
 
@@ -30,42 +30,21 @@
 
 All checks are mentioned at least in some way in the [Scientific-Python
 Development Guide][]. You should read that first - if you are not attempting to
 follow them, some of the checks might not work. For example, the guidelines
 specify pytest configuration be placed in `pyproject.toml`. If you place it
 somewhere else, then all the pytest checks will be skipped.
 
-This was originally developed for [Scikit-HEP][] before moving to Scientific
-Python.
-
-You can also use GitHub Actions:
-
-```yaml
-- uses: scientific-python/cookie@<version>
-```
-
-Or pre-commit:
-
-```yaml
-- repo: https://github.com/scientific-python/cookie
-  rev: <version>
-  hooks:
-    - id: sp-repo-review
-```
-
 <!-- prettier-ignore-start -->
 
 [actions-badge]: https://github.com/scientific-python/cookie/workflows/CI/badge.svg
 [actions-link]: https://github.com/scientific-python/cookie/actions
-[github-discussions-badge]: https://img.shields.io/static/v1?label=Discussions&message=Ask&color=blue&logo=github
-[github-discussions-link]: https://github.com/scientific-python/cookie/discussions
 [pypi-link]: https://pypi.org/project/sp-repo-review/
 [pypi-platforms]: https://img.shields.io/pypi/pyversions/sp-repo-review
 [pypi-version]: https://badge.fury.io/py/sp-repo-review.svg
-[repo-review]: https://repo-review.readthedocs.io
-[rtd-badge]: https://readthedocs.org/projects/scientific-python-cookie/badge/?version=latest
-[rtd-link]: https://scientific-python-cookie.readthedocs.io/en/latest/?badge=latest
+[docs-badge]: https://readthedocs.org/projects/scientific-python-cookie/badge/?version=latest
+[docs-link]: https://scientific-python-cookie.readthedocs.io/en/latest/?badge=latest
 [scientific-python development guide]: https://learn.scientific-python.org/development
 [scientific-python/cookie]: https://github.com/scientific-python/cookie
 [scikit-hep]: https://scikit-hep.org
 
 <!-- prettier-ignore-end -->
```

### Comparing `sp_repo_review-2023.6.17/pyproject.toml` & `sp_repo_review-2023.6.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -28,33 +28,32 @@
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Topic :: Software Development :: Quality Assurance",
   "Typing :: Typed",
 ]
 dynamic = ["version"]
 dependencies = [
   "pyyaml",
-  "repo-review~=0.7.0",
+  "repo-review>=0.7.0b4,<0.8",
 ]
 
 [project.optional-dependencies]
 cli = [
   "repo-review[cli]",
 ]
 test = [
   "pytest >=7",
 ]
 dev = [
   "pytest >=7",
 ]
 
 [project.urls]
-Guide = "https://learn.scientific-python.org/development"
-Homepage = "https://scientific-python.github.io/cookie"
+Homepage = "https://github.com/scientific-python/cookie"
+Webpage = "https://scientific-python.github.io/cookie"
 Preview = "https://scientific-python-cookie.readthedocs.io"
-Source = "https://github.com/scientific-python/cookie"
 
 
 [project.entry-points."pipx.run"]
 sp-repo-review = "repo_review.__main__:main"
 
 [project.entry-points."repo_review.checks"]
 general = "sp_repo_review.checks.general:repo_review_checks"
@@ -87,15 +86,15 @@
   'ignore:(ast.Str|Attribute s|ast.NameConstant|ast.Num) is deprecated:DeprecationWarning:_pytest',
 ]
 norecursedirs = ['{{cookiecutter.project_name}}']
 testpaths = ["tests"]
 
 
 [tool.mypy]
-files = ["src", "tests"]
+files = ["src", "web", "tests"]
 python_version = "3.10"
 warn_unused_configs = true
 strict = true
 show_error_codes = true
 enable_error_code = ["ignore-without-code", "redundant-expr", "truthy-bool"]
 warn_unreachable = true
 disallow_untyped_defs = false
```

### Comparing `sp_repo_review-2023.6.17/PKG-INFO` & `sp_repo_review-2023.6.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: sp_repo_review
-Version: 2023.6.17
+Version: 2023.6.7
 Summary: Review repos for compliance to the Scientific-Python development guidelines
-Project-URL: Guide, https://learn.scientific-python.org/development
-Project-URL: Homepage, https://scientific-python.github.io/cookie
+Project-URL: Homepage, https://github.com/scientific-python/cookie
+Project-URL: Webpage, https://scientific-python.github.io/cookie
 Project-URL: Preview, https://scientific-python-cookie.readthedocs.io
-Project-URL: Source, https://github.com/scientific-python/cookie
 Author-email: Henry Schreiner <henryfs@princeton.edu>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: WebAssembly :: Emscripten
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -22,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Requires-Dist: pyyaml
-Requires-Dist: repo-review~=0.7.0
+Requires-Dist: repo-review<0.8,>=0.7.0b4
 Provides-Extra: cli
 Requires-Dist: repo-review[cli]; extra == 'cli'
 Provides-Extra: dev
 Requires-Dist: pytest>=7; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: pytest>=7; extra == 'test'
 Description-Content-Type: text/markdown
@@ -41,15 +40,15 @@
 [![GitHub Discussion][github-discussions-badge]][github-discussions-link]
 [![Live ReadTheDocs][rtd-badge]][rtd-link]
 
 [![PyPI version][pypi-version]][pypi-link]
 [![PyPI platforms][pypi-platforms]][pypi-link]
 
 `sp-repo-review` provides checks based on the [Scientific-Python Development
-Guide][] at [scientific-python/cookie][] for [repo-review][].
+Guide][] at [scientific-python/cookie][].
 
 This tool can check the style of a repository. Use like this:
 
 ```bash
 pipx run 'sp-repo-review[cli]' <path to repository>
 ```
 
@@ -67,42 +66,21 @@
 
 All checks are mentioned at least in some way in the [Scientific-Python
 Development Guide][]. You should read that first - if you are not attempting to
 follow them, some of the checks might not work. For example, the guidelines
 specify pytest configuration be placed in `pyproject.toml`. If you place it
 somewhere else, then all the pytest checks will be skipped.
 
-This was originally developed for [Scikit-HEP][] before moving to Scientific
-Python.
-
-You can also use GitHub Actions:
-
-```yaml
-- uses: scientific-python/cookie@<version>
-```
-
-Or pre-commit:
-
-```yaml
-- repo: https://github.com/scientific-python/cookie
-  rev: <version>
-  hooks:
-    - id: sp-repo-review
-```
-
 <!-- prettier-ignore-start -->
 
 [actions-badge]: https://github.com/scientific-python/cookie/workflows/CI/badge.svg
 [actions-link]: https://github.com/scientific-python/cookie/actions
-[github-discussions-badge]: https://img.shields.io/static/v1?label=Discussions&message=Ask&color=blue&logo=github
-[github-discussions-link]: https://github.com/scientific-python/cookie/discussions
 [pypi-link]: https://pypi.org/project/sp-repo-review/
 [pypi-platforms]: https://img.shields.io/pypi/pyversions/sp-repo-review
 [pypi-version]: https://badge.fury.io/py/sp-repo-review.svg
-[repo-review]: https://repo-review.readthedocs.io
-[rtd-badge]: https://readthedocs.org/projects/scientific-python-cookie/badge/?version=latest
-[rtd-link]: https://scientific-python-cookie.readthedocs.io/en/latest/?badge=latest
+[docs-badge]: https://readthedocs.org/projects/scientific-python-cookie/badge/?version=latest
+[docs-link]: https://scientific-python-cookie.readthedocs.io/en/latest/?badge=latest
 [scientific-python development guide]: https://learn.scientific-python.org/development
 [scientific-python/cookie]: https://github.com/scientific-python/cookie
 [scikit-hep]: https://scikit-hep.org
 
 <!-- prettier-ignore-end -->
```

