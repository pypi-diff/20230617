# Comparing `tmp/molecule-qemu-0.4.8.tar.gz` & `tmp/molecule-qemu-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecule-qemu-0.4.8.tar", last modified: Tue Jun 13 07:38:05 2023, max compression
+gzip compressed data, was "molecule-qemu-0.4.9.tar", last modified: Thu Jun 15 09:40:44 2023, max compression
```

## Comparing `molecule-qemu-0.4.8.tar` & `molecule-qemu-0.4.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:38:05.525043 molecule-qemu-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/.ansible-lint
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:38:05.517043 molecule-qemu-0.4.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:38:05.521043 molecule-qemu-0.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:38:05.521043 molecule-qemu-0.4.8/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-06-13 07:38:05.525043 molecule-qemu-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:38:05.521043 molecule-qemu-0.4.8/molecule_qemu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/molecule_qemu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:38:05.525043 molecule-qemu-0.4.8/molecule_qemu/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/molecule_qemu/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:38:05.521043 molecule-qemu-0.4.8/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:38:05.525043 molecule-qemu-0.4.8/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/molecule_qemu/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:38:05.525043 molecule-qemu-0.4.8/molecule_qemu/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)  2097152 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/molecule_qemu/playbooks/QEMU_EFI.fd
--rw-r--r--   0 runner    (1001) docker     (123)    13317 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/molecule_qemu/playbooks/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/molecule_qemu/playbooks/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:38:05.525043 molecule-qemu-0.4.8/molecule_qemu/playbooks/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/molecule_qemu/playbooks/templates/meta-data.j2
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/molecule_qemu/playbooks/templates/user-data.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:38:05.525043 molecule-qemu-0.4.8/molecule_qemu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-06-13 07:38:05.000000 molecule-qemu-0.4.8/molecule_qemu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-13 07:38:05.000000 molecule-qemu-0.4.8/molecule_qemu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 07:38:05.000000 molecule-qemu-0.4.8/molecule_qemu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-13 07:38:05.000000 molecule-qemu-0.4.8/molecule_qemu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 07:38:05.000000 molecule-qemu-0.4.8/molecule_qemu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 07:38:05.000000 molecule-qemu-0.4.8/molecule_qemu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-13 07:38:05.525043 molecule-qemu-0.4.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:44.458329 molecule-qemu-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/.ansible-lint
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:44.450328 molecule-qemu-0.4.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:44.454329 molecule-qemu-0.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:44.454329 molecule-qemu-0.4.9/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-06-15 09:40:44.458329 molecule-qemu-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:44.454329 molecule-qemu-0.4.9/molecule_qemu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/molecule_qemu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:44.454329 molecule-qemu-0.4.9/molecule_qemu/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/molecule_qemu/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:44.450328 molecule-qemu-0.4.9/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:44.454329 molecule-qemu-0.4.9/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/molecule_qemu/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:44.458329 molecule-qemu-0.4.9/molecule_qemu/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)  2097152 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/molecule_qemu/playbooks/QEMU_EFI.fd
+-rw-r--r--   0 runner    (1001) docker     (123)    13317 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/molecule_qemu/playbooks/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/molecule_qemu/playbooks/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:44.458329 molecule-qemu-0.4.9/molecule_qemu/playbooks/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/molecule_qemu/playbooks/templates/meta-data.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/molecule_qemu/playbooks/templates/user-data.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:44.454329 molecule-qemu-0.4.9/molecule_qemu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-06-15 09:40:44.000000 molecule-qemu-0.4.9/molecule_qemu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-15 09:40:44.000000 molecule-qemu-0.4.9/molecule_qemu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 09:40:44.000000 molecule-qemu-0.4.9/molecule_qemu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-15 09:40:44.000000 molecule-qemu-0.4.9/molecule_qemu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 09:40:44.000000 molecule-qemu-0.4.9/molecule_qemu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 09:40:44.000000 molecule-qemu-0.4.9/molecule_qemu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-15 09:40:44.458329 molecule-qemu-0.4.9/setup.cfg
```

### Comparing `molecule-qemu-0.4.8/.github/workflows/lint.yml` & `molecule-qemu-0.4.9/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.8/.github/workflows/publish.yml` & `molecule-qemu-0.4.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.8/.github/workflows/release.yml` & `molecule-qemu-0.4.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.8/.gitignore` & `molecule-qemu-0.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.8/.yamllint` & `molecule-qemu-0.4.9/.yamllint`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.8/LICENSE` & `molecule-qemu-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.8/Makefile` & `molecule-qemu-0.4.9/Makefile`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.8/PKG-INFO` & `molecule-qemu-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule-qemu
-Version: 0.4.8
+Version: 0.4.9
 Summary: Molecule QEMU
 Author-email: Andrey Gubarev <andrey@andreygubarev.com>
 License: MIT
 Project-URL: Homepage, https://github.com/andreygubarev/molecule-qemu/
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `molecule-qemu-0.4.8/README.md` & `molecule-qemu-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.8/molecule_qemu/driver.py` & `molecule-qemu-0.4.9/molecule_qemu/driver.py`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.8/molecule_qemu/playbooks/QEMU_EFI.fd` & `molecule-qemu-0.4.9/molecule_qemu/playbooks/QEMU_EFI.fd`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.8/molecule_qemu/playbooks/create.yml` & `molecule-qemu-0.4.9/molecule_qemu/playbooks/create.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.8/molecule_qemu/playbooks/destroy.yml` & `molecule-qemu-0.4.9/molecule_qemu/playbooks/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.8/molecule_qemu.egg-info/PKG-INFO` & `molecule-qemu-0.4.9/molecule_qemu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule-qemu
-Version: 0.4.8
+Version: 0.4.9
 Summary: Molecule QEMU
 Author-email: Andrey Gubarev <andrey@andreygubarev.com>
 License: MIT
 Project-URL: Homepage, https://github.com/andreygubarev/molecule-qemu/
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `molecule-qemu-0.4.8/molecule_qemu.egg-info/SOURCES.txt` & `molecule-qemu-0.4.9/molecule_qemu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.8/pyproject.toml` & `molecule-qemu-0.4.9/pyproject.toml`

 * *Files identical despite different names*

