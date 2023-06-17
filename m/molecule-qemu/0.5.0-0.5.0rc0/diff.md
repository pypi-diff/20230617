# Comparing `tmp/molecule-qemu-0.5.0.tar.gz` & `tmp/molecule-qemu-0.5.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecule-qemu-0.5.0.tar", last modified: Sat Jun 17 13:12:26 2023, max compression
+gzip compressed data, was "molecule-qemu-0.5.0rc0.tar", last modified: Sat Jun 17 10:33:30 2023, max compression
```

## Comparing `molecule-qemu-0.5.0.tar` & `molecule-qemu-0.5.0rc0.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:12:26.533716 molecule-qemu-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/.ansible-lint
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:12:26.517715 molecule-qemu-0.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:12:26.521715 molecule-qemu-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:12:26.525715 molecule-qemu-0.5.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-06-17 13:12:26.533716 molecule-qemu-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:12:26.525715 molecule-qemu-0.5.0/molecule_qemu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/molecule_qemu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:12:26.525715 molecule-qemu-0.5.0/molecule_qemu/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/molecule_qemu/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:12:26.521715 molecule-qemu-0.5.0/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:12:26.525715 molecule-qemu-0.5.0/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/molecule_qemu/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:12:26.525715 molecule-qemu-0.5.0/molecule_qemu/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)  2097152 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/molecule_qemu/playbooks/QEMU_EFI.fd
--rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/molecule_qemu/playbooks/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/molecule_qemu/playbooks/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:12:26.529715 molecule-qemu-0.5.0/molecule_qemu/playbooks/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/molecule_qemu/playbooks/templates/meta-data.j2
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/molecule_qemu/playbooks/templates/user-data.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:12:26.525715 molecule-qemu-0.5.0/molecule_qemu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-06-17 13:12:26.000000 molecule-qemu-0.5.0/molecule_qemu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-17 13:12:26.000000 molecule-qemu-0.5.0/molecule_qemu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 13:12:26.000000 molecule-qemu-0.5.0/molecule_qemu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-17 13:12:26.000000 molecule-qemu-0.5.0/molecule_qemu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-17 13:12:26.000000 molecule-qemu-0.5.0/molecule_qemu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-17 13:12:26.000000 molecule-qemu-0.5.0/molecule_qemu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-17 13:12:26.533716 molecule-qemu-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:12:26.529715 molecule-qemu-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/tests/.yamllint
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:12:26.521715 molecule-qemu-0.5.0/tests/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:12:26.529715 molecule-qemu-0.5.0/tests/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/tests/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/tests/molecule/default/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/tests/molecule/default/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/tests/molecule/default/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:12:26.529715 molecule-qemu-0.5.0/tests/molecule/network-shared/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/tests/molecule/network-shared/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/tests/molecule/network-shared/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/tests/molecule/network-shared/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/tests/molecule/network-shared/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:12:26.529715 molecule-qemu-0.5.0/tests/molecule/network-user/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/tests/molecule/network-user/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/tests/molecule/network-user/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/tests/molecule/network-user/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/tests/molecule/network-user/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:12:26.529715 molecule-qemu-0.5.0/tests/molecule/os-debian-bullseye/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/tests/molecule/os-debian-bullseye/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/tests/molecule/os-debian-bullseye/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/tests/molecule/os-debian-bullseye/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/tests/molecule/os-debian-bullseye/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:12:26.529715 molecule-qemu-0.5.0/tests/molecule/os-ubuntu-focal/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/tests/molecule/os-ubuntu-focal/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/tests/molecule/os-ubuntu-focal/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/tests/molecule/os-ubuntu-focal/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/tests/molecule/os-ubuntu-focal/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:12:26.529715 molecule-qemu-0.5.0/tests/molecule/os-ubuntu-jammy/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/tests/molecule/os-ubuntu-jammy/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/tests/molecule/os-ubuntu-jammy/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/tests/molecule/os-ubuntu-jammy/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/tests/molecule/os-ubuntu-jammy/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:12:26.529715 molecule-qemu-0.5.0/tests/molecule/platform-amd64/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/tests/molecule/platform-amd64/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/tests/molecule/platform-amd64/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/tests/molecule/platform-amd64/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/tests/molecule/platform-amd64/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:12:26.533716 molecule-qemu-0.5.0/tests/molecule/platform-arm64/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/tests/molecule/platform-arm64/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/tests/molecule/platform-arm64/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/tests/molecule/platform-arm64/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-17 13:12:12.000000 molecule-qemu-0.5.0/tests/molecule/platform-arm64/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:33:30.141567 molecule-qemu-0.5.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/.ansible-lint
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:33:30.133566 molecule-qemu-0.5.0rc0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:33:30.133566 molecule-qemu-0.5.0rc0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:33:30.133566 molecule-qemu-0.5.0rc0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-06-17 10:33:30.141567 molecule-qemu-0.5.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:33:30.133566 molecule-qemu-0.5.0rc0/molecule_qemu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/molecule_qemu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:33:30.133566 molecule-qemu-0.5.0rc0/molecule_qemu/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/molecule_qemu/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:33:30.133566 molecule-qemu-0.5.0rc0/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:33:30.133566 molecule-qemu-0.5.0rc0/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/molecule_qemu/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:33:30.137566 molecule-qemu-0.5.0rc0/molecule_qemu/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)  2097152 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/molecule_qemu/playbooks/QEMU_EFI.fd
+-rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/molecule_qemu/playbooks/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/molecule_qemu/playbooks/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:33:30.137566 molecule-qemu-0.5.0rc0/molecule_qemu/playbooks/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/molecule_qemu/playbooks/templates/meta-data.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/molecule_qemu/playbooks/templates/user-data.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:33:30.133566 molecule-qemu-0.5.0rc0/molecule_qemu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-06-17 10:33:30.000000 molecule-qemu-0.5.0rc0/molecule_qemu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-17 10:33:30.000000 molecule-qemu-0.5.0rc0/molecule_qemu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 10:33:30.000000 molecule-qemu-0.5.0rc0/molecule_qemu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-17 10:33:30.000000 molecule-qemu-0.5.0rc0/molecule_qemu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-17 10:33:30.000000 molecule-qemu-0.5.0rc0/molecule_qemu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-17 10:33:30.000000 molecule-qemu-0.5.0rc0/molecule_qemu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-17 10:33:30.141567 molecule-qemu-0.5.0rc0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:33:30.137566 molecule-qemu-0.5.0rc0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/tests/.yamllint
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:33:30.133566 molecule-qemu-0.5.0rc0/tests/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:33:30.137566 molecule-qemu-0.5.0rc0/tests/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/tests/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/tests/molecule/default/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/tests/molecule/default/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/tests/molecule/default/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:33:30.137566 molecule-qemu-0.5.0rc0/tests/molecule/network-shared/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/tests/molecule/network-shared/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/tests/molecule/network-shared/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/tests/molecule/network-shared/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/tests/molecule/network-shared/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:33:30.137566 molecule-qemu-0.5.0rc0/tests/molecule/network-user/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/tests/molecule/network-user/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/tests/molecule/network-user/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/tests/molecule/network-user/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/tests/molecule/network-user/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:33:30.137566 molecule-qemu-0.5.0rc0/tests/molecule/os-debian-bullseye/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/tests/molecule/os-debian-bullseye/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/tests/molecule/os-debian-bullseye/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/tests/molecule/os-debian-bullseye/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/tests/molecule/os-debian-bullseye/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:33:30.137566 molecule-qemu-0.5.0rc0/tests/molecule/os-ubuntu-focal/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/tests/molecule/os-ubuntu-focal/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/tests/molecule/os-ubuntu-focal/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/tests/molecule/os-ubuntu-focal/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/tests/molecule/os-ubuntu-focal/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:33:30.141567 molecule-qemu-0.5.0rc0/tests/molecule/os-ubuntu-jammy/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/tests/molecule/os-ubuntu-jammy/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/tests/molecule/os-ubuntu-jammy/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/tests/molecule/os-ubuntu-jammy/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/tests/molecule/os-ubuntu-jammy/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:33:30.141567 molecule-qemu-0.5.0rc0/tests/molecule/platform-amd64/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/tests/molecule/platform-amd64/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/tests/molecule/platform-amd64/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/tests/molecule/platform-amd64/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/tests/molecule/platform-amd64/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:33:30.141567 molecule-qemu-0.5.0rc0/tests/molecule/platform-arm64/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/tests/molecule/platform-arm64/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/tests/molecule/platform-arm64/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/tests/molecule/platform-arm64/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-17 10:33:20.000000 molecule-qemu-0.5.0rc0/tests/molecule/platform-arm64/verify.yml
```

### Comparing `molecule-qemu-0.5.0/.github/workflows/python-package.yml` & `molecule-qemu-0.5.0rc0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.5.0/.gitignore` & `molecule-qemu-0.5.0rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.5.0/.yamllint` & `molecule-qemu-0.5.0rc0/.yamllint`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.5.0/LICENSE` & `molecule-qemu-0.5.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.5.0/Makefile` & `molecule-qemu-0.5.0rc0/Makefile`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.5.0/PKG-INFO` & `molecule-qemu-0.5.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule-qemu
-Version: 0.5.0
+Version: 0.5.0rc0
 Summary: Molecule QEMU
 Author-email: Andrey Gubarev <andrey@andreygubarev.com>
 License: MIT
 Project-URL: Homepage, https://github.com/andreygubarev/molecule-qemu/
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `molecule-qemu-0.5.0/README.md` & `molecule-qemu-0.5.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.5.0/molecule_qemu/driver.py` & `molecule-qemu-0.5.0rc0/molecule_qemu/driver.py`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.5.0/molecule_qemu/playbooks/QEMU_EFI.fd` & `molecule-qemu-0.5.0rc0/molecule_qemu/playbooks/QEMU_EFI.fd`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.5.0/molecule_qemu/playbooks/create.yml` & `molecule-qemu-0.5.0rc0/molecule_qemu/playbooks/create.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.5.0/molecule_qemu/playbooks/destroy.yml` & `molecule-qemu-0.5.0rc0/molecule_qemu/playbooks/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.5.0/molecule_qemu.egg-info/PKG-INFO` & `molecule-qemu-0.5.0rc0/molecule_qemu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule-qemu
-Version: 0.5.0
+Version: 0.5.0rc0
 Summary: Molecule QEMU
 Author-email: Andrey Gubarev <andrey@andreygubarev.com>
 License: MIT
 Project-URL: Homepage, https://github.com/andreygubarev/molecule-qemu/
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `molecule-qemu-0.5.0/molecule_qemu.egg-info/SOURCES.txt` & `molecule-qemu-0.5.0rc0/molecule_qemu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.5.0/pyproject.toml` & `molecule-qemu-0.5.0rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.5.0/tests/.yamllint` & `molecule-qemu-0.5.0rc0/tests/.yamllint`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.5.0/tests/molecule/network-shared/molecule.yml` & `molecule-qemu-0.5.0rc0/tests/molecule/network-shared/molecule.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.5.0/tests/molecule/network-user/molecule.yml` & `molecule-qemu-0.5.0rc0/tests/molecule/network-user/molecule.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.5.0/tests/molecule/os-debian-bullseye/molecule.yml` & `molecule-qemu-0.5.0rc0/tests/molecule/os-debian-bullseye/molecule.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.5.0/tests/molecule/os-ubuntu-focal/molecule.yml` & `molecule-qemu-0.5.0rc0/tests/molecule/os-ubuntu-focal/molecule.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.5.0/tests/molecule/os-ubuntu-jammy/molecule.yml` & `molecule-qemu-0.5.0rc0/tests/molecule/os-ubuntu-jammy/molecule.yml`

 * *Files identical despite different names*

