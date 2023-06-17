# Comparing `tmp/scicookie-0.1.1.tar.gz` & `tmp/scicookie-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scicookie-0.1.1.tar", max compression
+gzip compressed data, was "scicookie-0.2.0.tar", max compression
```

## Comparing `scicookie-0.1.1.tar` & `scicookie-0.2.0.tar`

### file list

```diff
@@ -1,60 +1,61 @@
--rw-r--r--   0        0        0     1551 2023-03-31 01:35:05.906450 scicookie-0.1.1/LICENSE
--rw-r--r--   0        0        0     1711 2023-06-11 00:16:35.923043 scicookie-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-09 16:16:30.770946 scicookie-0.1.1/src/scicookie/__init__.py
--rw-r--r--   0        0        0       68 2023-06-10 22:35:28.903163 scicookie-0.1.1/src/scicookie/__main__.py
--rw-r--r--   0        0        0     3030 2023-06-10 23:23:24.579054 scicookie-0.1.1/src/scicookie/cli.py
--rw-r--r--   0        0        0     1683 2023-06-10 02:42:09.747457 scicookie-0.1.1/src/scicookie/cookiecutter.json
--rw-r--r--   0        0        0     5768 2023-06-10 02:42:47.302727 scicookie-0.1.1/src/scicookie/hooks/post_gen_project.py
--rw-r--r--   0        0        0      359 2023-03-31 01:35:05.926450 scicookie-0.1.1/src/scicookie/hooks/pre_gen_project.py
--rw-r--r--   0        0        0      657 2023-06-10 03:10:19.453895 scicookie-0.1.1/src/scicookie/logs.py
--rw-r--r--   0        0        0     1207 2023-06-10 03:10:44.538589 scicookie-0.1.1/src/scicookie/profile.py
--rw-r--r--   0        0        0     3686 2023-06-10 02:40:31.065604 scicookie-0.1.1/src/scicookie/profiles/base.yaml
--rw-r--r--   0        0        0      739 2023-06-10 02:41:11.028692 scicookie-0.1.1/src/scicookie/profiles/osl.yaml
--rw-r--r--   0        0        0     1871 2023-06-10 03:10:57.546937 scicookie-0.1.1/src/scicookie/ui.py
--rw-r--r--   0        0        0       67 2023-06-08 00:09:47.410403 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.bandit
--rw-r--r--   0        0        0      292 2023-03-31 01:35:05.954450 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.editorconfig
--rw-r--r--   0        0        0     4617 2023-06-08 00:09:47.410403 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0        0        0      892 2023-06-08 00:09:47.410403 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1712 2023-06-08 00:09:47.410403 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/documentation-report.yml
--rw-r--r--   0        0        0     2550 2023-06-08 00:09:47.418403 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0        0        0      342 2023-03-31 01:35:05.958449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0     1387 2023-06-08 00:09:47.418403 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      814 2023-05-03 14:26:42.182726 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/main.yaml
--rw-r--r--   0        0        0     1666 2023-06-08 00:09:47.418403 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1274 2023-03-31 01:35:05.962449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.gitignore
--rw-r--r--   0        0        0     3198 2023-06-09 01:51:29.564476 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2295 2023-06-08 00:58:27.913254 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.releaserc.json
--rw-r--r--   0        0        0     5996 2023-03-31 01:35:05.962449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/LICENSE
--rw-r--r--   0        0        0     2637 2023-06-08 16:24:02.893195 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/Makefile
--rw-r--r--   0        0        0     3325 2023-06-10 02:40:03.810262 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/README.md
--rw-r--r--   0        0        0     6433 2023-03-31 01:35:05.966449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/coc/CITIZEN.md
--rw-r--r--   0        0        0     6434 2023-03-31 01:35:05.966449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/coc/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     5488 2023-03-31 01:35:05.966449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_CONVENANT.md
--rw-r--r--   0        0        0     5488 2023-03-31 01:35:05.966449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_COVENANT.md
--rw-r--r--   0        0        0      175 2023-06-08 00:09:47.418403 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/conda/dev.yaml
--rw-r--r--   0        0        0     1998 2023-06-10 02:40:03.834261 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/containers/Dockerfile
--rw-r--r--   0        0        0      300 2023-06-08 00:09:47.422403 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/containers/compose.yaml
--rw-r--r--   0        0        0       20 2023-03-31 01:35:05.970449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs/changelog.md
--rw-r--r--   0        0        0     5666 2023-06-08 00:09:47.422403 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs/contributing.md
--rw-r--r--   0        0        0     1001 2023-03-31 01:35:05.970449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs/example.ipynb
--rw-r--r--   0        0        0    72342 2023-03-31 01:35:05.974449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs/images/favicon.ico
--rw-r--r--   0        0        0    20402 2023-03-31 01:35:05.974449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs/images/logo.png
--rw-r--r--   0        0        0     3386 2023-06-10 02:40:03.830261 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs/index.md
--rw-r--r--   0        0        0      996 2023-03-31 01:35:05.974449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs/installation.md
--rw-r--r--   0        0        0      967 2023-03-31 01:35:05.970449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_config.yaml
--rw-r--r--   0        0        0      151 2023-03-31 01:35:05.970449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_toc.yml
--rw-r--r--   0        0        0     4055 2023-03-31 01:35:05.970449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs-mkdocs/mkdocs.yaml
--rwxr-xr-x   0        0        0     5217 2023-06-08 00:09:47.422403 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/conf.py
--rw-r--r--   0        0        0      311 2023-03-31 01:35:05.970449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/index.rst
--rw-r--r--   0        0        0      829 2023-03-31 01:35:05.970449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/make.bat
--rw-r--r--   0        0        0       26 2023-03-31 01:35:05.970449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/readme.rst
--rw-r--r--   0        0        0    16493 2023-06-08 00:09:47.422403 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/governance/numpy_governance.md
--rw-r--r--   0        0        0     6843 2023-06-08 00:09:47.422403 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/governance/sciml_governance.md
--rw-r--r--   0        0        0     3247 2023-06-10 02:40:03.766263 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/pyproject.toml
--rw-r--r--   0        0        0     1558 2023-06-08 00:09:47.422403 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/roadmap/ignite_roadmap.md
--rw-r--r--   0        0        0       61 2023-03-31 01:35:05.974449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/tests/__init__.py
--rw-r--r--   0        0        0      317 2023-03-31 01:35:05.978449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py
--rw-r--r--   0        0        0      796 2023-06-09 02:09:33.606669 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__init__.py
--rw-r--r--   0        0        0      631 2023-06-09 02:09:46.798522 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__main__.py
--rw-r--r--   0        0        0       19 2023-03-31 01:35:05.978449 scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/{{cookiecutter.package_slug}}.py
--rw-r--r--   0        0        0      644 1970-01-01 00:00:00.000000 scicookie-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1551 2023-06-17 01:11:15.787381 scicookie-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2060 2023-06-17 01:16:30.327177 scicookie-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       77 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/__init__.py
+-rw-r--r--   0        0        0      115 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/__main__.py
+-rw-r--r--   0        0        0     3132 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/cli.py
+-rw-r--r--   0        0        0     1704 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/cookiecutter.json
+-rw-r--r--   0        0        0     5707 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      359 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/hooks/pre_gen_project.py
+-rw-r--r--   0        0        0      969 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/logs.py
+-rw-r--r--   0        0        0     1385 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/profile.py
+-rw-r--r--   0        0        0     3695 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/profiles/base.yaml
+-rw-r--r--   0        0        0      739 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/profiles/osl.yaml
+-rw-r--r--   0        0        0     2122 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/ui.py
+-rw-r--r--   0        0        0      292 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.editorconfig
+-rw-r--r--   0        0        0     4617 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0      892 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1712 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/documentation-report.yml
+-rw-r--r--   0        0        0     2550 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0        0        0      342 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0     1387 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      814 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/main.yaml
+-rw-r--r--   0        0        0     1666 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1274 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.gitignore
+-rw-r--r--   0        0        0     2867 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2295 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.releaserc.json
+-rw-r--r--   0        0        0     5996 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/LICENSE
+-rw-r--r--   0        0        0     2637 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/Makefile
+-rw-r--r--   0        0        0     3325 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/README.md
+-rw-r--r--   0        0        0     6433 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CITIZEN.md
+-rw-r--r--   0        0        0     6434 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     5488 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_CONVENANT.md
+-rw-r--r--   0        0        0     5488 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_COVENANT.md
+-rw-r--r--   0        0        0      255 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/conda/dev.yaml
+-rw-r--r--   0        0        0     1998 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/containers/Dockerfile
+-rw-r--r--   0        0        0      300 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/containers/compose.yaml
+-rw-r--r--   0        0        0       54 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs/api/references.md
+-rw-r--r--   0        0        0      182 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs/api/references.rst
+-rw-r--r--   0        0        0       20 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs/changelog.md
+-rw-r--r--   0        0        0     5666 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs/contributing.md
+-rw-r--r--   0        0        0     1116 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs/example.ipynb
+-rw-r--r--   0        0        0    72342 2023-06-17 01:11:15.795381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs/images/favicon.ico
+-rw-r--r--   0        0        0    20402 2023-06-17 01:11:15.795381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs/images/logo.png
+-rw-r--r--   0        0        0     3386 2023-06-17 01:11:15.795381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs/index.md
+-rw-r--r--   0        0        0      996 2023-06-17 01:11:15.795381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs/installation.md
+-rw-r--r--   0        0        0      967 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_config.yaml
+-rw-r--r--   0        0        0      151 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_toc.yml
+-rw-r--r--   0        0        0     4249 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs-mkdocs/mkdocs.yaml
+-rwxr-xr-x   0        0        0     5275 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/conf.py
+-rw-r--r--   0        0        0      374 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/index.rst
+-rw-r--r--   0        0        0      829 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/make.bat
+-rw-r--r--   0        0        0       30 2023-06-17 01:11:15.791381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/readme.md
+-rw-r--r--   0        0        0    16493 2023-06-17 01:11:15.795381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/governance/numpy_governance.md
+-rw-r--r--   0        0        0     6843 2023-06-17 01:11:15.795381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/governance/sciml_governance.md
+-rw-r--r--   0        0        0     4381 2023-06-17 01:11:15.795381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/pyproject.toml
+-rw-r--r--   0        0        0     1558 2023-06-17 01:11:15.795381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/roadmap/ignite_roadmap.md
+-rw-r--r--   0        0        0       61 2023-06-17 01:11:15.795381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0      317 2023-06-17 01:11:15.795381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py
+-rw-r--r--   0        0        0      809 2023-06-17 01:11:15.795381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__init__.py
+-rw-r--r--   0        0        0      631 2023-06-17 01:11:15.795381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__main__.py
+-rw-r--r--   0        0        0       19 2023-06-17 01:11:15.795381 scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/{{cookiecutter.package_slug}}.py
+-rw-r--r--   0        0        0      643 1970-01-01 00:00:00.000000 scicookie-0.2.0/PKG-INFO
```

### Comparing `scicookie-0.1.1/LICENSE` & `scicookie-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.1/pyproject.toml` & `scicookie-0.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scicookie"
-version = "0.1.1"  # semantic-release
+version = "0.2.0"  # semantic-release
 description = "Cookiecutter template for a Python package"
 authors = ["Ivan Ogasawara <ivan.ogasawara@gmail.com>"]
 license = "BSD"
 include = [
     {path = "src/scicookie/cookiecutter.json"},
     {path = "src/scicookie/{{cookiecutter.project_slug}}"},
     {path = "src/scicookie/hooks"},
@@ -13,68 +13,82 @@
 [tool.poetry.scripts]
 "scicookie" = "scicookie.__main__:app"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 cookieninja = "1.0.0"
 sh = "^2.0.4"
-pyyaml = "<6.0"
+pyyaml = ">=5"
 colorama = "^0.4.6"
 inquirer = "^3.1.3"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7"
-black = "^22"
-isort = "^5"
-pre-commit = "^2"
-flake8 = "^4"
-mypy = "^0.931"
-pytest-cov = "^3.0.0"
-pytest-cookies = "^0.6.1"
-Sphinx = "^4.4.0"
-Flake8-pyproject = "^0.9.0"
-jupyterlab = "^3.5.1"
-jupyter-book = "^0.12.3"
-myst-parser = "^0.15"
+pytest = ">=7"
+black = ">=22"
+isort = ">=5"
+pre-commit = ">=3"
+ruff = ">=0.0.272"
+mypy = ">=1"
+pytest-cov = ">=3"
+pytest-cookies = ">=0.6.1"
+Sphinx = ">=4.4"
+jupyterlab = ">=3.5.1"
+jupyter-book = ">=0.12.3"
+myst-parser = ">=0.15"
 makim = "1.8.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 79
 # note: for support "py39", we need to update black using poetry
 #       currently, it has conflicts with typing-extensions.
 target-version = ["py38"]
-force-exclude = '''
-/(
-  |  docs/*
-  |  hooks/*
-  |  {{cookiecutter.project_slug}}/*
+force-exclude = '''(?x)(
+    docs/*
+  | src/scicookie/{{cookiecutter.project_slug}}/*
+  | src/scicookie/hooks/*
   |.*\\.egg-info
-)/
-'''
+)'''  # TOML's single-quoted strings do not require escaping backslashes
 
-[tool.flake8]
-max-line-length = 79
-# Ignoring these erros will prevent conflicts with Flake8 and Jinja2 syntax.
-exclude = [
-  '.git/*',
-  '__pycache__/*',
-  'docs/*',
-  'src/scicookie/hooks/*',
-  'src/scicookie/{{cookiecutter.project_slug}}/*'
+[tool.mypy]
+no_strict_optional = false
+exclude = '''(?x)(
+      src/scicookie/{{cookiecutter.project_slug}}/
+    | src/scicookie/hooks/*
+)'''  # TOML's single-quoted strings do not require escaping backslashes
+
+[[tool.mypy.overrides]]
+module = [
+  "colorama",
+  "inquirer",
+  "sh",
+  "yaml",
 ]
+ignore_missing_imports = true
 
-[tool.isort]
-ensure_newline_before_comments = true
-line_length = 79
-multi_line_output = 3
-include_trailing_comma = true
-skip_glob = ["docs/*", "*.egg-info"]
+[tool.ruff]
+line-length = 79
+force-exclude = true
+src = ["src/scicookie"]
+exclude = [
+   'src/scicookie/\{\{cookiecutter.project_slug\}\}',
+   'src/scicookie/hooks',
+]
+select = [
+  "E",   # pycodestyle
+  "F",   # pyflakes
+  "D",   # pydocstyle
+  "YTT", # flake8-2020
+  "PL",  # PL
+  "RUF", # Ruff-specific rules
+]
 
+[tool.ruff.pydocstyle]
+convention = "numpy"
 
 [tool.pytest.ini_options]
 testpaths = [
     "tests",
 ]
```

### Comparing `scicookie-0.1.1/src/scicookie/cli.py` & `scicookie-0.2.0/src/scicookie/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Module with CLI functions."""
 import json
 import os
 import sys
 from pathlib import Path
 from typing import Union
 
 import sh
@@ -26,14 +27,15 @@
     if isinstance(answer_definition, str):
         return answer_definition
 
     return answer_definition[0]
 
 
 def call_cookiecutter(profile: Profile, answers: dict):
+    """Call coociecutter/cookieninja with the parameters from the TUI."""
     answers_profile = {}
     cookie_args = []
     questions = profile.config
 
     with open(COOKIECUTTER_FILE_PATH) as f:
         coockiecutter_config = json.load(f)
 
@@ -92,16 +94,15 @@
         p.kill()
         SciCookieLogs.raise_error(
             f"Process {pid} killed.", SciCookieErrorType.SH_KEYBOARD_INTERRUPT
         )
 
 
 def app():
-    """CLI main function."""
-
+    """Run SciCookie."""
     # note: this parameter should be provided by a CLI argument
     profile = Profile("osl")
 
     answers = make_questions(profile.config)
 
     if not answers:
         return
```

### Comparing `scicookie-0.1.1/src/scicookie/cookiecutter.json` & `scicookie-0.2.0/src/scicookie/cookiecutter.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222222%*

 * *Differences: {"'use_ruff'": "'yes'"}*

```diff
@@ -63,10 +63,11 @@
     "use_flake8": "yes",
     "use_isort": "yes",
     "use_mccabe": "yes",
     "use_mypy": "yes",
     "use_pre_commit": "yes",
     "use_pydocstyle": "yes",
     "use_pytest": "yes",
+    "use_ruff": "yes",
     "use_shellcheck": "yes",
     "use_vulture": "yes"
 }
```

### Comparing `scicookie-0.1.1/src/scicookie/hooks/post_gen_project.py` & `scicookie-0.2.0/src/scicookie/hooks/post_gen_project.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,14 +73,15 @@
 def move_selected_doc_dir():
     docs_target_dir = PROJECT_DIRECTORY / "docs"
     for file_name in os.listdir(DOCS_SPEC_DIR):
         shutil.move(DOCS_SPEC_DIR / file_name, docs_target_dir)
 
     if DOCUMENTATION_ENGINE == "sphinx":
         remove_project_file(Path("docs") / "index.md")
+        remove_project_file(Path("docs/api") / "references.md")
 
     shutil.rmtree(DOCS_SPEC_DIR)
 
 def clean_up_docs():
     remove_dirs(UNUSED_DOCS_DIRS)
     move_selected_doc_dir()
 
@@ -88,19 +89,14 @@
 def clean_up_project_layout():
     if USE_SRC_LAYOUT:
         if not os.path.exists("src"):
             os.mkdir("src")
             shutil.move('{{cookiecutter.package_slug}}', 'src')
 
 
-def clean_up_bandit():
-    if USE_BANDIT:
-        remove_project_file(PROJECT_DIRECTORY / '.bandit')
-
-
 def clean_up_code_of_conduct():
     if COC_PATH:
         shutil.move(
             COC_PATH,
             PROJECT_DIRECTORY / 'CODE_OF_CONDUCT.md'
         )
     remove_dir("coc")
@@ -188,15 +184,14 @@
 
 def post_gen():
     validation()
 
     # keep this one first, because it changes the package folder
     clean_up_project_layout()
 
-    clean_up_bandit()
     clean_up_cli()
     clean_up_code_of_conduct()
     clean_up_conda()
     clean_up_containers()
     clean_up_docs()
     clean_up_governance()
     clean_up_roadmap()
```

### Comparing `scicookie-0.1.1/src/scicookie/profiles/base.yaml` & `scicookie-0.2.0/src/scicookie/profiles/base.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -88,29 +88,30 @@
 
 documentation_engine:
   message: Select the Documentation Engine
   help: ""
   type: single-choice
   choices:
     - mkdocs
-    - argparse
+    - sphinx
     - jupyter-book
   enabled: false
 
 use_tools:
   message: Select the initial tools you want to add to your project
   help: ""
   type: multiple-choices
   choices:
     - bandit
     - black
     - blue
     - conda
     - coverage
     - flake8
+    - ruff
     - isort
     - mccabe
     - pre-commit
     - pydocstyle
     - pytest
     - shellcheck
     - vulture
```

### Comparing `scicookie-0.1.1/src/scicookie/profiles/osl.yaml` & `scicookie-0.2.0/src/scicookie/profiles/osl.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.1/src/scicookie/ui.py` & `scicookie-0.2.0/src/scicookie/ui.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+"""Define functions for the interface with the user."""
+from typing import Optional, Type, Dict
 import inquirer
-
 from scicookie.logs import SciCookieErrorType, SciCookieLogs
 
 
-def _create_question(question_id: str, question: dict):
+def _create_question(
+    question_id: str, question: dict
+) -> Optional[inquirer.questions.Question]:
     # validation
     if not question.get("enabled", False):
-        return
+        return None
 
     # config required
-    default_answer = question.get("default")
-    question_message = question.get("message")
-    question_type = question.get("type")
+    default_answer = question.get("default", "")
+    question_message = question.get("message", "")
+    question_type = question.get("type", "")
     # todo: implement help text int he prompt
     # question_help = question.get("help")
     # todo: implement depends on workflow, it needs refactoring the code
     #       because it needs access to the answer
     # question_depends_on = question.get("depends_on")
 
     question_types_available = [
@@ -39,28 +42,29 @@
             else f"{question_message} (default: {default_answer})"
         )
     }
 
     if question.get("choices"):
         content["choices"] = question.get("choices")
 
-    fn_questions = {
+    fn_questions: Dict[str, Type[inquirer.questions.Question]] = {
         "text": inquirer.Text,
         "single-choice": inquirer.List,
         "multiple-choices": inquirer.Checkbox,
         "confirm": inquirer.Confirm,
     }
 
     return fn_questions[question_type](
         question_id,
         **content,
     )
 
 
 def make_questions(questions: dict):
+    """Generate all the enabled questions."""
     questions_ui = []
 
     for question_id, question in questions.items():
         question_obj = _create_question(question_id, question)
         if question_obj:
             questions_ui.append(question_obj)
```

### Comparing `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/bug-report.yml` & `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/config.yml` & `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/documentation-report.yml` & `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/documentation-report.yml`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/feature-request.yml` & `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.github/PULL_REQUEST_TEMPLATE.md` & `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/main.yaml` & `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/release.yaml` & `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.gitignore` & `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.pre-commit-config.yaml` & `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.pre-commit-config.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,152 +1,127 @@
+{% if cookiecutter.project_layout == "src" -%}
+{% set package_path = "src/" + cookiecutter.package_slug -%}
+{% else -%}
+{% set package_path = cookiecutter.package_slug -%}
+{% endif -%}
+default_stages:
+  - commit
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.1.0
     hooks:
       - id: end-of-file-fixer
 
   - repo: local
     hooks:
 {%- if cookiecutter.use_blue == "yes" %}
-    - entry: blue
-      id: blue
+    - id: blue
       name: blue
-      exclude: |
-        (?x)(
-          docs
-        )
-      files: ""
+      entry: blue
       language: system
       pass_filenames: true
-      stages:
-        - commit
       types:
         - python
-        - file
-        - python
 {% endif -%}
 {%- if cookiecutter.use_black == "yes" %}
-    - entry: black
-      id: black
+    - id: black
       name: black
-      exclude: |
-        (?x)(
-          docs
-        )
-      files: ""
+      entry: black
       language: system
       pass_filenames: true
-      stages:
-        - commit
       types:
         - python
-        - file
-        - python
 {% endif %}
 {%- if cookiecutter.use_flake8 == "yes" %}
-    - entry: flake8
-      exclude: ^$
-      files: ""
-      id: flake8
-      language: python
+    - id: flake8
       name: flake8
+      entry: flake8
+      language: system
       pass_filenames: true
-      stages:
-        - commit
       types:
         - python
 {% endif %}
+{%- if cookiecutter.use_ruff == 'ruff' %}
+    - id: ruff
+      name: ruff
+      entry: ruff
+      language: system
+      pass_filenames: true
+      files: "{{ package_path }}"
+      types:
+        - python
+{%- endif %}
 {%- if cookiecutter.use_isort == "yes" %}
-    - entry: isort
-      exclude: "^.*/js/.*$"
-      files: ""
-      id: isort
-      language: python
+    - id: isort
       name: isort
+      entry: isort
+      language: system
       pass_filenames: true
-      stages:
-        - commit
       types:
         - python
 {% endif %}
 {%- if cookiecutter.use_mypy == "yes" %}
-    - entry: mypy
-      exclude: ^$
-      # note: it would be good to extend this to other apps as well
-      files: "{{ cookiecutter.package_slug }}/"
-      id: mypy
-      language: python
+    - id: mypy
       name: mypy
+      entry: mypy
+      language: system
+      files: "{{ package_path }}"
       pass_filenames: true
-      stages:
-        - commit
       types:
         - python
 {% endif %}
 {%- if cookiecutter.use_shellcheck == "yes" %}
-    - entry: shellcheck
-      id: shellcheck
-      language: system
+    - id: shellcheck
       name: shellcheck
-      files: .sh$
-      types:
-          - shell
+      entry: shellcheck
+      language: system
       types_or:
-          - file
-          - sh
-          - ash
-          - bash
-          - bats
-          - dash
-          - ksh
+        - sh
+        - shell
+        - ash
+        - bash
+        - bats
+        - dash
+        - ksh
 {% endif %}
 {%- if cookiecutter.use_bandit == "yes" %}
-    - entry: bandit
-      id: bandit
-      language: python
+    - id: bandit
       name: bandit
-      args: ['-iii', '-ll', .bandit]
+      entry: bandit
+      language: system
+      args: ['--configfile', 'pyproject.toml', '-iii', '-lll']
       pass_filenames: true
-      stages:
-        - commit
       types:
         - python
 {% endif %}
 {%- if cookiecutter.use_pydocstyle == "yes" %}
-    - entry: pydocstyle
-      exclude: ^$
-      files: "{{ cookiecutter.package_slug }}/"
-      id: pydocstyle
-      language: python
+    - id: pydocstyle
       name: pydocstyle
+      entry: pydocstyle
+      language: system
+      files: "{{ package_path }}"
       pass_filenames: true
-      stages:
-        - commit
       types:
         - python
 {% endif %}
 {%- if cookiecutter.use_vulture == "yes" %}
-    - entry: vulture
-      files: "{{ cookiecutter.package_slug }}/"
-      id: vulture
-      language: python
+    - id: vulture
       name: vulture
+      entry: vulture
+      language: system
+      files: "{{ package_path }}"
       description: Find unused Python code.
       pass_filenames: true
-      stages:
-        - commit
       types:
         - python
 {% endif %}
 {%- if cookiecutter.use_mccabe == "yes" %}
     - id: mccabe
       name: mccabe
-      entry: flake8 --max-complexity 10
-      language: python
-      files: "{{ cookiecutter.package_slug }}/"
+      entry: python -m mccabe --min 10
+      language: system
+      files: "{{ package_path }}"
       pass_filenames: true
-      stages:
-        - commit
       types:
         - python
 {% endif %}
 {#- keep this at the end of the file -#}
```

### Comparing `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/.releaserc.json` & `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/.releaserc.json`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/LICENSE` & `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/LICENSE`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/Makefile` & `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/README.md` & `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/README.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/coc/CITIZEN.md` & `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CITIZEN.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/coc/CODE_OF_CONDUCT.md` & `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_CONVENANT.md` & `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_CONVENANT.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_COVENANT.md` & `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_COVENANT.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/containers/Dockerfile` & `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/containers/Dockerfile`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs/contributing.md` & `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs/example.ipynb` & `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs/example.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9561011904761905%*

 * *Differences: {"'cells'": "{insert: [(2, OrderedDict([('cell_type', 'code'), ('execution_count', None), "*

 * *            "('metadata', OrderedDict()), ('outputs', []), ('source', [])]))]}",*

 * * "'metadata'": "{'language_info': {'version': '3.10.11'}}"}*

```diff
@@ -19,14 +19,21 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import {{ cookiecutter.package_slug }}"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
@@ -37,13 +44,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.8"
+            "version": "3.10.11"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs/images/favicon.ico` & `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs/images/logo.png` & `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs/index.md` & `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs/index.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs/installation.md` & `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs/installation.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_config.yaml` & `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_config.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs-mkdocs/mkdocs.yaml` & `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs-mkdocs/mkdocs.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 site_name: {{ cookiecutter.project_name}}
 site_url: {{ cookiecutter.project_url}}
 repo_url: {{ cookiecutter.git_https_upstream}}
 docs_dir: ./
 site_dir: ../build
 # extra_css:
 #   - stylesheets/extra.css
+# Page tree
+nav:
+  - index.md
+  - Installation: installation.md
+  - Changelog: changelog.md
+  - Contributing: contributing.md
+  - API: api/references.md
+  - Notebook page: example.ipynb
 theme:
   name: material
   features:
     - content.code.annotate
     - content.tabs.link
     - header.autohide
     - navigation.indexes
@@ -34,15 +42,15 @@
   #       - backends/template.md
   - mkdocstrings:
       enable_inventory: true
       handlers:
         python:
           import:
             - https://docs.python.org/3/objects.inv
-          selection:
+          options:
             docstring_style: numpy
             filters:
               - "!^Bounds"
               - "!^__class__"
               - "!^_filter_with_like"
               - "!^_find_backends"
               - "!^_key$"
@@ -67,20 +75,20 @@
               - "!^reconnect"
               - "!^select_builder_class"
               - "!^select_class"
               - "!^table_class$"
               - "!^table_expr_class"
               - "!^translator_class"
               - "!^Options$"
-          rendering:
             show_category_heading: true
             show_root_full_path: false
             show_root_heading: true
             show_root_toc_entry: true
             show_source: false
+            show_modules: true
   - mkdocs-jupyter:
       execute: true
       ignore:
         - "*.py"
       # execute_ignore: "tutorial/*Geospatial*.ipynb"
       include_source: true
       theme: dark
```

### Comparing `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/conf.py` & `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,25 +26,28 @@
 #
 # needs_sphinx = "1.0"
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named "sphinx.ext.*") or your custom ones.
 extensions = [
     "sphinx.ext.autodoc",
-    "sphinx.ext.viewcode",
-    "myst_parser"
+    "sphinx.ext.napoleon",
+    "myst_parser",
+    "nbsphinx"
 ]
 
+nbsphinx_allow_errors = True
+
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
-source_suffix = [".rst", ".md", ".ipynb"]
+source_suffix = [".rst", ".md"]
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "{{ cookiecutter.project_name }}"
 copyright = "{% now 'local', '%Y' %}, {{ cookiecutter.author_full_name }}"
@@ -65,15 +68,15 @@
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
-exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", ".ipynb_checkpoints"]
 
 # The name of the Pygments (syntax highlighting) style to use.
 pygments_style = "sphinx"
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = False
```

### Comparing `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/make.bat` & `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/make.bat`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/governance/numpy_governance.md` & `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/governance/numpy_governance.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/governance/sciml_governance.md` & `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/governance/sciml_governance.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/pyproject.toml` & `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+{% if cookiecutter.project_layout == "src" -%}
+{% set package_path = "src/" + cookiecutter.package_slug -%}
+{% else -%}
+{% set package_path = cookiecutter.package_slug -%}
+{% endif -%}
 [tool.poetry]
 name = "{{ cookiecutter.project_slug }}"
 version = "{{ cookiecutter.project_version }}"  # semantic-release
 description = "{{ cookiecutter.project_short_description }}"
 authors = ["{{ cookiecutter.author_full_name }} <{{ cookiecutter.author_email }}>"]
 license = "{{ cookiecutter.project_license }}"
 include = [
@@ -37,39 +42,42 @@
 [tool.poetry.dependencies]
 python = "^3.8.1"
 
 [tool.poetry.dev-dependencies]
 urllib3 = "<2"  # fix poetry issues
 {# keep this line here #}
 {%- if cookiecutter.use_pytest == "yes" -%}
-pytest = "^7"
+pytest = "^7.3.2"
 {% if cookiecutter.use_coverage == "yes" -%}
-pytest-cov = "^4"
+pytest-cov = "^4.1.0"
 {% endif %}
 {%- endif -%}{#- end of use_pytest -#}
 {%- if cookiecutter.use_coverage == "yes" -%}
-coverage = "^7"
+coverage = "^7.2.7"
 {% endif %}
 {%- if cookiecutter.use_blue == "yes" -%}
 blue = "^0.9.1"
 {% endif %}
 {%- if cookiecutter.use_black == "yes" -%}
-black = "^22.3"
+black = "^23.3.0"
 {% endif %}
 {%- if cookiecutter.use_isort == "yes" -%}
-isort = "^5"
+isort = "^5.12.0"
 {% endif %}
 {%- if cookiecutter.use_pre_commit -%}
-pre-commit = "^2"
+pre-commit = "^3.3.2"
 {% endif %}
 {%- if cookiecutter.use_flake8 == "yes" -%}
-flake8 = "^4"
+flake8 = ">=4.0.1, <7"
+{% endif %}
+{%- if cookiecutter.use_ruff == "yes" -%}
+ruff = "^0.0.272"
 {% endif %}
 {%- if cookiecutter.use_mypy == "yes" -%}
-mypy = "^0.931"
+mypy = "^1.3.0"
 {% endif %}
 {%- if cookiecutter.use_bandit == "yes" -%}
 bandit = "^1.7.5"
 {% endif %}
 {%- if cookiecutter.use_pydocstyle == "yes" -%}
 pydocstyle = "^6.3.0"
 {% endif %}
@@ -77,68 +85,98 @@
 vulture = "^2.7"
 {% endif %}
 {%- if cookiecutter.use_mccabe == "yes" -%}
 mccabe = "^0.6.1"
 {% endif %}
 {%- if cookiecutter.use_containers in ['Docker', 'Podman'] -%}
 # if you want to use docker-compose from your system, remove compose-go here
-compose-go = "^2.18.0"
+compose-go = "^2.18.1"
 {% endif %}
 {%- if cookiecutter.documentation_engine == 'mkdocs' -%}
-Jinja2 = "<3.1.0"
-mkdocs = ">=1.2.3,<2"
-mkdocs-exclude = ">=1.0.2,<2"
-mkdocs-jupyter = ">=0.20.0,<1"
-mkdocs-literate-nav = ">=0.4.1,<1"
-mkdocs-macros-plugin = ">=0.6.3,<1"
-mkdocs-material = ">=8.2.1,<9"
-mkdocstrings = ">=0.17.0,<0.18.0"
+Jinja2 = "^3.1.2"
+mkdocs = "^1.4.3"
+mkdocs-exclude = "^1.0.2"
+mkdocs-jupyter = "^0.24.1"
+mkdocs-literate-nav = "^0.6.0"
+mkdocs-macros-plugin = ">=0.7.0,<1"
+mkdocs-material = "^9.1.15"
+mkdocstrings = "^0.21.2"
+mkdocstrings-python = "^1.1.2"
 {% elif cookiecutter.documentation_engine == 'sphinx' -%}
-Sphinx = "^5.0.0"
-sphinx-rtd-theme = "^1.1.1"
-importlib-metadata = "^5.0.0"
-myst-parser = "^0.18.1"
+Sphinx = "^6.2.1"
+sphinx-rtd-theme = "^1.2.2"
+importlib-metadata = "^6.5.1"
+myst-parser = "^0.19.2"
+nbsphinx = "^0.9.2"
+pandoc = "^2.3"
 {% elif cookiecutter.documentation_engine == 'jupyter-book' -%}
-jupyter-book = "^0.12.3"
-myst-parser = "^0.15.0"
+jupyter-book = "^0.15.1"
+myst-parser = "^0.18.1"
 {% endif %}
 {%- if cookiecutter.use_pytest == "yes" %}
 [tool.pytest.ini_options]
 testpaths = [
     "tests",
 ]
 {% endif %}
 {%- if cookiecutter.use_blue == "yes" %}
 [tool.blue]
 line-length = 79
 target-version = ["py38"]
-force-exclude = """
-(
-  /(
-      docs/*
-    |.*\\.egg-info
-  )/
-)
-"""
+force-exclude = '''(?x)(
+    docs/*
+  | .*\\.egg-info
+)'''  # TOML's single-quoted strings do not require escaping backslashes
 {% endif %}
 {%- if cookiecutter.use_black == "yes" %}
 [tool.black]
 line-length = 79
 target-version = ["py38"]
-force-exclude = """
-(
-  /(
-      docs/*
-    |.*\\.egg-info
-  )/
-)
-"""
+force-exclude = '''(?x)(
+    docs/*
+  | .*\\.egg-info
+)'''  # TOML's single-quoted strings do not require escaping backslashes
 {% endif %}
 {%- if cookiecutter.use_isort == "yes" %}
 [tool.isort]
 ensure_newline_before_comments = true
 line_length = 79
 multi_line_output = 3
 include_trailing_comma = true
 skip_glob = ["docs/*", "*.egg-info"]
 {% endif %}
+{%- if cookiecutter.use_bandit == "yes" %}
+[tool.bandit]
+exclude_dirs = ["tests"]
+targets = "{{ package_path }}"
+{% endif %}
+{%- if cookiecutter.use_vulture == "yes" %}
+[tool.vulture]
+exclude = ["tests"]
+ignore_decorators = []
+ignore_names = []
+make_whitelist = true
+min_confidence = 80
+paths = ["{{ package_path }}"]
+sort_by_size = true
+verbose = false
+{% endif %}
+{%- if cookiecutter.use_ruff == "yes" %}
+[tool.ruff]
+line-length = 79
+force-exclude = true
+src = ["{{ package_path }}"]
+exclude = [
+  'docs',
+]
+select = [
+  "F",   # pyflakes
+]
+
+[tool.ruff.pydocstyle]
+convention = "numpy"
+{% endif %}
+{%- if cookiecutter.use_mypy == "yes" %}
+[tool.mypy]
+no_strict_optional = false
+{% endif %}
 {#- keep this line at the end of the file -#}
```

### Comparing `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/roadmap/ignite_roadmap.md` & `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/roadmap/ignite_roadmap.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__init__.py` & `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# type: ignore[attr-defined]
+# mypy: disable-error-code="attr-defined"
 """{{ cookiecutter.project_name }}."""
 {%- if cookiecutter.use_blue == "yes" %}
   {%- set QUOTE = "'" -%}
 {%- elif cookiecutter.use_black == "yes" %}
   {%- set QUOTE = '"' -%}
 {%- else %}
   {%- set QUOTE = "'" -%}
```

### Comparing `scicookie-0.1.1/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__main__.py` & `scicookie-0.2.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__main__.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.1.1/PKG-INFO` & `scicookie-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: scicookie
-Version: 0.1.1
+Version: 0.2.0
 Summary: Cookiecutter template for a Python package
 License: BSD
 Author: Ivan Ogasawara
 Author-email: ivan.ogasawara@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: cookieninja (==1.0.0)
 Requires-Dist: inquirer (>=3.1.3,<4.0.0)
-Requires-Dist: pyyaml (<6.0)
+Requires-Dist: pyyaml (>=5)
 Requires-Dist: sh (>=2.0.4,<3.0.0)
```

