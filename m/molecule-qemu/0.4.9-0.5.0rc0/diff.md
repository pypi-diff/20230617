# Comparing `tmp/molecule-qemu-0.4.9.tar.gz` & `tmp/molecule-qemu-0.5.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecule-qemu-0.4.9.tar", last modified: Thu Jun 15 09:40:44 2023, max compression
+gzip compressed data, was "molecule-qemu-0.5.0rc0.tar", last modified: Sat Jun 17 10:33:30 2023, max compression
```

## Comparing `molecule-qemu-0.4.9.tar` & `molecule-qemu-0.5.0rc0.tar`

### file list

```diff
@@ -1,41 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:44.458329 molecule-qemu-0.4.9/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/.ansible-lint
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:44.450328 molecule-qemu-0.4.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:44.454329 molecule-qemu-0.4.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:44.454329 molecule-qemu-0.4.9/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-06-15 09:40:44.458329 molecule-qemu-0.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:44.454329 molecule-qemu-0.4.9/molecule_qemu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/molecule_qemu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:44.454329 molecule-qemu-0.4.9/molecule_qemu/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/molecule_qemu/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:44.450328 molecule-qemu-0.4.9/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:44.454329 molecule-qemu-0.4.9/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/molecule_qemu/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:44.458329 molecule-qemu-0.4.9/molecule_qemu/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)  2097152 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/molecule_qemu/playbooks/QEMU_EFI.fd
--rw-r--r--   0 runner    (1001) docker     (123)    13317 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/molecule_qemu/playbooks/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/molecule_qemu/playbooks/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:44.458329 molecule-qemu-0.4.9/molecule_qemu/playbooks/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/molecule_qemu/playbooks/templates/meta-data.j2
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/molecule_qemu/playbooks/templates/user-data.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:40:44.454329 molecule-qemu-0.4.9/molecule_qemu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-06-15 09:40:44.000000 molecule-qemu-0.4.9/molecule_qemu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-15 09:40:44.000000 molecule-qemu-0.4.9/molecule_qemu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 09:40:44.000000 molecule-qemu-0.4.9/molecule_qemu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-15 09:40:44.000000 molecule-qemu-0.4.9/molecule_qemu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 09:40:44.000000 molecule-qemu-0.4.9/molecule_qemu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 09:40:44.000000 molecule-qemu-0.4.9/molecule_qemu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 09:40:31.000000 molecule-qemu-0.4.9/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-15 09:40:44.458329 molecule-qemu-0.4.9/setup.cfg
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

### Comparing `molecule-qemu-0.4.9/.gitignore` & `molecule-qemu-0.5.0rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.9/.yamllint` & `molecule-qemu-0.5.0rc0/.yamllint`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.9/LICENSE` & `molecule-qemu-0.5.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.9/molecule_qemu/driver.py` & `molecule-qemu-0.5.0rc0/molecule_qemu/driver.py`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.9/molecule_qemu/playbooks/QEMU_EFI.fd` & `molecule-qemu-0.5.0rc0/molecule_qemu/playbooks/QEMU_EFI.fd`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.9/molecule_qemu/playbooks/create.yml` & `molecule-qemu-0.5.0rc0/molecule_qemu/playbooks/create.yml`

 * *Files 7% similar despite different names*

```diff
@@ -6,47 +6,50 @@
 
   vars:
     molecule_ephemeral_directory: "{{ lookup('env', 'MOLECULE_EPHEMERAL_DIRECTORY') }}"
     molecule_driver_directory: "{{ ( molecule_ephemeral_directory + '/../../.qemu/' ) | realpath }}"
     molecule_scenario_name: "{{ lookup('env', 'MOLECULE_SCENARIO_NAME') }}"
     molecule_project_name: "{{ lookup('env', 'MOLECULE_PROJECT_DIRECTORY') | basename }}"
     qemu_cap_hvf: false
-    qemu_vm_image_arch: "x86_64"
-    qemu_vm_image_format: "qcow2"
-    qemu_vm_memory: "1024"
-    qemu_vm_cpus: "2"
-    qemu_vm_disk: "4G"
-    qemu_vm_network: "user"
+    qemu_image_arch: "x86_64"
+    qemu_image_format: "qcow2"
+    qemu_vm_memory: "512"
+    qemu_vm_cpus: "1"
+    qemu_vm_disk: "8G"
+    qemu_network_mode: "user"
+    qemu_timeout_arp: 120
+    qemu_timeout_ssh: 600
 
   environment:
     http_proxy: "{{ lookup('ansible.builtin.env', 'http_proxy') | default(omit) }}"
     https_proxy: "{{ lookup('ansible.builtin.env', 'https_proxy') | default(omit) }}"
 
   tasks:
     ### configuration #########################################################
 
     - name: Register VMs data
       ansible.builtin.set_fact:
         instance: {
           "instance": "molecule-{{ molecule_project_name }}-{{ molecule_scenario_name }}-{{ item.name }}",
           "name": "{{ item.name }}",
 
-          "image": "{{ item.image }}",
+          "image_arch": "{{ item.image_arch | default(qemu_image_arch) }}",
+          "image_url": "{{ item.image_url }}",
           "image_checksum": "{{ item.image_checksum | default(omit) }}",
-          "image_arch": "{{ item.image_arch | default(qemu_vm_image_arch) }}",
-          "image_format": "{{ item.image_format | default(qemu_vm_image_format) }}",
+          "image_format": "{{ item.image_format | default(qemu_image_format) }}",
 
-          "ssh_port": "{{ item.ssh_port | default(22) }}",
-          "ssh_user": "{{ item.ssh_user | default('root') }}",
+          "network_mode": "{{ item.network_mode | default(qemu_network_mode) }}",
+          "network_mac": "{{ '52:54:00' | community.general.random_mac() | regex_replace('(^|:)0([0-9A-Fa-f])', '\\1\\2') }}",
+
+          "network_ssh_port": "{{ item.network_ssh_port | default(22) }}",
+          "network_ssh_user": "{{ item.network_ssh_user | default('root') }}",
 
           "vm_cpus": "{{ item.vm_cpus | default(qemu_vm_cpus) }}",
           "vm_memory": "{{ item.vm_memory | default(qemu_vm_memory) }}",
           "vm_disk": "{{ item.vm_disk | default(qemu_vm_disk) }}",
-          "vm_network": "{{ item.vm_network | default(qemu_vm_network) }}",
-          "vm_network_mac": "{{ '52:54:00' | community.general.random_mac(seed=item.name | to_json | hash('md5')) | regex_replace('(^|:)0([0-9A-Fa-f])', '\\1\\2') }}",
 
           "path_disk": "{{ molecule_ephemeral_directory }}/run/{{ item.name }}.qcow2",
           "path_pid": "{{ molecule_ephemeral_directory }}/run/{{ item.name }}.pid",
         }
       loop: "{{ molecule_yml.platforms }}"
       loop_control:
         label: "{{ item.name }}"
@@ -67,39 +70,39 @@
         fail_msg: "Molecule instances are not properly defined"
         success_msg: "Molecule instances are properly defined"
 
     - name: Assert supported VMs configuration
       ansible.builtin.assert:
         that:
           - item.image_arch in ['x86_64', 'aarch64']
-          - item.vm_network in ['user', 'vmnet-shared']
+          - item.network_mode in ['user', 'vmnet-shared']
         fail_msg: "Molecule instance {{ item.name }} configuration is not supported"
         success_msg: "Molecule instance {{ item.name }} configuration is supported"
       loop: "{{ molecule_instances }}"
       loop_control:
         label: "{{ item.name }}"
 
     - name: Assert VMs network configuration
       ansible.builtin.assert:
         that:
-          - molecule_instances | map(attribute='vm_network') | list | unique | length == 1
+          - molecule_instances | map(attribute='network_mode') | list | unique | length == 1
         fail_msg: "Network modes are mutually exclusive"
         success_msg: "Network modes are configured properly"
 
     - name: Set QEMU network
       ansible.builtin.set_fact:
-        qemu_vm_network: "{{ molecule_instances | map(attribute='vm_network') | list | unique | first }}"
+        qemu_network_mode: "{{ molecule_instances | map(attribute='network_mode') | list | unique | first }}"
 
     - name: Assert VMs ssh configuration
       ansible.builtin.assert:
         that:
-          - molecule_instances | map(attribute='ssh_port') | list | unique | length == molecule_instances | length
+          - molecule_instances | map(attribute='network_ssh_port') | list | unique | length == molecule_instances | length
         fail_msg: "Molecule instances SSH are not properly configured for 'user' network"
         success_msg: "Molecule instances SSH are properly configured for 'user' network"
-      when: qemu_vm_network == 'user'
+      when: qemu_network_mode == 'user'
 
     ### capabilities ##########################################################
 
     - name: Read kern.hv_support
       ansible.builtin.command: sysctl kern.hv_support
       register: hv_support
       changed_when: false
@@ -148,15 +151,15 @@
 
     - name: Fetch images
       ansible.builtin.get_url:
         url: "{{ item[0] }}"
         checksum: "{{ item[1] }}"
         dest: "{{ molecule_driver_directory }}/images/{{ item[0] | basename }}"
         mode: "0644"
-      loop: "{{ molecule_instances | map(attribute='image') | zip(molecule_instances | map(attribute='image_checksum')) | list | unique }}"
+      loop: "{{ molecule_instances | map(attribute='image_url') | zip(molecule_instances | map(attribute='image_checksum')) | list | unique }}"
       loop_control:
         label: "{{ item[0] | basename }}"
       register: images
 
     - name: Get images
       ansible.builtin.set_fact:
         images: "{{ images.results | map(attribute='url') | zip(images.results | map(attribute='dest')) }}"
@@ -214,42 +217,42 @@
 
     ### qemu ##################################################################
 
     - name: Create VMs disks
       ansible.builtin.command: >
         qemu-img create
         -f qcow2
-        -o backing_file={{ images_cache[item.image] }},backing_fmt={{ item.image_format }}
+        -o backing_file={{ images_cache[item.image_url] }},backing_fmt={{ item.image_format }}
         {{ item.path_disk }}
         {{ item.vm_disk }}
       args:
         creates: "{{ item.path_disk }}"
       loop: "{{ molecule_instances }}"
       loop_control:
         label: "{{ item.name }}"
 
     - name: Launch VMs as priviliged user
       ansible.builtin.set_fact:
-        qemu_privileged: "{{ (qemu_vm_network == 'vmnet-shared') | bool }}"
+        qemu_privileged: "{{ (qemu_network_mode == 'vmnet-shared') | bool }}"
 
     - name: Launch VMs
       become: "{{ qemu_privileged }}"
       ansible.builtin.command: >-
         qemu-system-{{ item.image_arch }}
         -name {{ item.name }}
         -boot d
         -cdrom {{ molecule_ephemeral_directory }}/run/cloud-init/{{ item.name }}.iso
         -hda {{ item.path_disk }}
         -m {{ item.vm_memory }}
         -smp {{ item.vm_cpus }}
-        {% if item.vm_network == 'vmnet-shared' %}
-        -nic vmnet-shared,model=virtio-net-pci,mac={{ item.vm_network_mac }}
+        {% if item.network_mode == 'vmnet-shared' %}
+        -nic vmnet-shared,model=virtio-net-pci,mac={{ item.network_mac }}
         {% endif %}
-        {% if item.vm_network == 'user' %}
-        -nic user,model=virtio-net-pci,hostfwd=tcp::{{ item.ssh_port }}-:22
+        {% if item.network_mode == 'user' %}
+        -nic user,model=virtio-net-pci,hostfwd=tcp::{{ item.network_ssh_port }}-:22
         {% endif %}
         -display none
         -daemonize
         -pidfile {{ item.path_pid }}
         {% if item.image_arch == 'aarch64' %}
         -bios {{ molecule_driver_directory }}/QEMU_EFI.fd
         -cpu cortex-a72
@@ -285,22 +288,22 @@
       loop: "{{ molecule_instances }}"
       loop_control:
         label: "{{ item.name }}"
 
     ### qemu network: vmnet-shared ############################################
 
     - name: Configure QEMU network (vmnet-shared)
-      when: qemu_vm_network == 'vmnet-shared'
+      when: qemu_network_mode == 'vmnet-shared'
       block:
         - name: Get IPv4 addresses from ARP table (vmnet-shared)
           ansible.builtin.shell: |
             set -o pipefail
-            arp -an | grep -i '{{ item.vm_network_mac }}' | awk '{print $2}' | sed 's/[()]//g'
+            arp -an | grep -i '{{ item.network_mac }}' | awk '{print $2}' | sed 's/[()]//g'
           until: molecule_instances_arp.stdout | length > 0
-          retries: 30
+          retries: "{{ qemu_timeout_arp }}"
           delay: 1
           loop: "{{ molecule_instances }}"
           loop_control:
             label: "{{ item.name }}"
           register: molecule_instances_arp
           changed_when: false
 
@@ -313,32 +316,32 @@
 
 
     ### ssh ###################################################################
 
     - name: Wait for SSH
       ansible.builtin.wait_for:
         host: "{{ molecule_instances_ipv4[item.name] }}"
-        port: "{{ item.ssh_port }}"
+        port: "{{ item.network_ssh_port }}"
         delay: 30
-        timeout: "{{ 60 * molecule_instances | length }}"
+        timeout: "{{ qemu_timeout_ssh }}"
         search_regex: "OpenSSH"
       loop: "{{ molecule_instances }}"
       loop_control:
         label: "{{ item.name }}"
 
     ### molecule ##############################################################
 
     - name: Prepare VMs config dict
       ansible.builtin.set_fact:
         instance_conf_dict: {
           "instance": "{{ item.instance }}",
           "name": "{{ item.name }}",
           "address": "{{ molecule_instances_ipv4[item.name] }}",
-          "user": "{{ item.ssh_user }}",
-          "port": "{{ item.ssh_port }}",
+          "user": "{{ item.network_ssh_user }}",
+          "port": "{{ item.network_ssh_port }}",
           "identity_file": "{{ ssh_keypair.filename }}",
           "pidfile": "{{ item.path_pid }}",
           "diskfile": "{{ item.path_disk }}",
           "privileged": "{{ qemu_privileged }}",
         }
       loop: "{{ molecule_instances }}"
       loop_control:
```

### Comparing `molecule-qemu-0.4.9/molecule_qemu/playbooks/destroy.yml` & `molecule-qemu-0.5.0rc0/molecule_qemu/playbooks/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.9/pyproject.toml` & `molecule-qemu-0.5.0rc0/pyproject.toml`

 * *Files identical despite different names*

