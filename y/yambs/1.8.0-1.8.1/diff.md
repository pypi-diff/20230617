# Comparing `tmp/yambs-1.8.0.tar.gz` & `tmp/yambs-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yambs-1.8.0.tar", last modified: Thu Jun 15 06:08:37 2023, max compression
+gzip compressed data, was "yambs-1.8.1.tar", last modified: Sat Jun 17 06:31:03 2023, max compression
```

## Comparing `yambs-1.8.0.tar` & `yambs-1.8.1.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:08:37.597098 yambs-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-15 06:07:15.000000 yambs-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9488 2023-06-15 06:08:37.597098 yambs-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-06-15 06:07:15.000000 yambs-1.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-15 06:07:15.000000 yambs-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 06:08:37.597098 yambs-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-15 06:07:15.000000 yambs-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:08:37.585098 yambs-1.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-15 06:07:15.000000 yambs-1.8.0/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-15 06:07:15.000000 yambs-1.8.0/tests/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:08:37.585098 yambs-1.8.0/yambs/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:08:37.585098 yambs-1.8.0/yambs/aggregation/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/aggregation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:08:37.585098 yambs-1.8.0/yambs/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/commands/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/commands/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/commands/uf2conv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:08:37.585098 yambs-1.8.0/yambs/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/config/board.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/config/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/config/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:08:37.589098 yambs-1.8.0/yambs/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:08:37.589098 yambs-1.8.0/yambs/data/includes/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/includes/chips.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/includes/infineon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/includes/microchip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/native.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:08:37.589098 yambs-1.8.0/yambs/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/schemas/Architecture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/schemas/Board.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/schemas/Chip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/schemas/Native.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/schemas/Toolchain.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/schemas/Variant.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/schemas/config_common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/schemas/targets_common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/schemas/toolchain_common.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:08:37.589098 yambs-1.8.0/yambs/data/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/templates/all.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/templates/architecture.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/templates/board.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/templates/build.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/templates/chip.ld.j2
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/templates/chip.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/templates/compile_commands.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/templates/native_all.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/templates/native_build.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/templates/native_rules.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/templates/rules.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/templates/toolchain.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/templates/variant.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/uf2families.json
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/data/yambs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:08:37.589098 yambs-1.8.0/yambs/environment/
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/environment/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:08:37.597098 yambs-1.8.0/yambs/generate/
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/generate/architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/generate/boards.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/generate/chips.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/generate/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:08:37.597098 yambs-1.8.0/yambs/generate/ninja/
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/generate/ninja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/generate/ninja/format.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/generate/toolchains.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/generate/variants.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:08:37.597098 yambs-1.8.0/yambs/translation/
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/translation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:08:37.597098 yambs-1.8.0/yambs/uf2/
--rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-06-15 06:07:15.000000 yambs-1.8.0/yambs/uf2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:08:37.585098 yambs-1.8.0/yambs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9488 2023-06-15 06:08:37.000000 yambs-1.8.0/yambs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-15 06:08:37.000000 yambs-1.8.0/yambs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 06:08:37.000000 yambs-1.8.0/yambs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-15 06:08:37.000000 yambs-1.8.0/yambs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-15 06:08:37.000000 yambs-1.8.0/yambs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 06:08:37.000000 yambs-1.8.0/yambs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:31:03.665854 yambs-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-17 06:29:55.000000 yambs-1.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9507 2023-06-17 06:31:03.665854 yambs-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-06-17 06:29:55.000000 yambs-1.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-17 06:29:55.000000 yambs-1.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 06:31:03.665854 yambs-1.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-17 06:29:55.000000 yambs-1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:31:03.657854 yambs-1.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-17 06:29:55.000000 yambs-1.8.1/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-17 06:29:55.000000 yambs-1.8.1/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:31:03.661854 yambs-1.8.1/yambs/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:31:03.661854 yambs-1.8.1/yambs/aggregation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/aggregation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:31:03.661854 yambs-1.8.1/yambs/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/commands/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/commands/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/commands/uf2conv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:31:03.661854 yambs-1.8.1/yambs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/config/board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/config/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/config/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:31:03.661854 yambs-1.8.1/yambs/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:31:03.661854 yambs-1.8.1/yambs/data/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/includes/chips.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/includes/infineon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/includes/microchip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/native.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:31:03.661854 yambs-1.8.1/yambs/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/schemas/Architecture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/schemas/Board.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/schemas/Chip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/schemas/Native.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/schemas/Toolchain.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/schemas/Variant.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/schemas/config_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/schemas/targets_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/schemas/toolchain_common.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:31:03.665854 yambs-1.8.1/yambs/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/templates/all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/templates/architecture.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/templates/board.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/templates/build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/templates/chip.ld.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/templates/chip.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/templates/compile_commands.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/templates/native_all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/templates/native_build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/templates/native_rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/templates/rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/templates/toolchain.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/templates/variant.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/uf2families.json
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/yambs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:31:03.665854 yambs-1.8.1/yambs/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/environment/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:31:03.665854 yambs-1.8.1/yambs/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/generate/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/generate/boards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/generate/chips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/generate/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:31:03.665854 yambs-1.8.1/yambs/generate/ninja/
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/generate/ninja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/generate/ninja/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/generate/toolchains.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/generate/variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:31:03.665854 yambs-1.8.1/yambs/translation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/translation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:31:03.665854 yambs-1.8.1/yambs/uf2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/uf2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:31:03.661854 yambs-1.8.1/yambs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9507 2023-06-17 06:31:03.000000 yambs-1.8.1/yambs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-17 06:31:03.000000 yambs-1.8.1/yambs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 06:31:03.000000 yambs-1.8.1/yambs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-17 06:31:03.000000 yambs-1.8.1/yambs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-17 06:31:03.000000 yambs-1.8.1/yambs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-17 06:31:03.000000 yambs-1.8.1/yambs.egg-info/top_level.txt
```

### Comparing `yambs-1.8.0/LICENSE` & `yambs-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yambs-1.8.0/PKG-INFO` & `yambs-1.8.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 1.8.0
+Version: 1.8.1
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=c88caeb9c6d71c51d9fd724250cd248c
+    hash=47efb6aab42b656852a2fdb9a25350fe
     =====================================
 -->
 
-# yambs ([1.8.0](https://pypi.org/project/yambs/))
+# yambs ([1.8.1](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
 
@@ -177,46 +177,44 @@
 ## Sub-command Options
 
 ### `gen`
 
 ```
 $ ./venv3.11/bin/mbs gen -h
 
-usage: mbs gen [-h] [-c CONFIG] [-i] [-w]
+usage: mbs gen [-h] [-c CONFIG] [-i] [-w] [-s]
 
 options:
   -h, --help            show this help message and exit
   -c CONFIG, --config CONFIG
                         the path to the top-level configuration file (default:
                         'yambs.yaml')
   -i, --single-pass     only run a single watch iteration
   -w, --watch           whether or not to continue watching for source tree
                         changes
+  -s, --sources         whether or not to only re-generate source manifests
 
 ```
 
 ### `native`
 
 ```
 $ ./venv3.11/bin/mbs native -h
 
-usage: mbs native [-h] [-c CONFIG] [-i] [-w] [variants ...]
-
-positional arguments:
-  variants              variants to build (defaults to 'debug' if not
-                        specified)
+usage: mbs native [-h] [-c CONFIG] [-i] [-w] [-s]
 
 options:
   -h, --help            show this help message and exit
   -c CONFIG, --config CONFIG
                         the path to the top-level configuration file (default:
                         'yambs.yaml')
   -i, --single-pass     only run a single watch iteration
   -w, --watch           whether or not to continue watching for source tree
                         changes
+  -s, --sources         whether or not to only re-generate source manifests
 
 ```
 
 ### `uf2conv`
 
 ```
 $ ./venv3.11/bin/mbs uf2conv -h
```

### Comparing `yambs-1.8.0/README.md` & `yambs-1.8.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=c88caeb9c6d71c51d9fd724250cd248c
+    hash=47efb6aab42b656852a2fdb9a25350fe
     =====================================
 -->
 
-# yambs ([1.8.0](https://pypi.org/project/yambs/))
+# yambs ([1.8.1](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
 
@@ -153,46 +153,44 @@
 ## Sub-command Options
 
 ### `gen`
 
 ```
 $ ./venv3.11/bin/mbs gen -h
 
-usage: mbs gen [-h] [-c CONFIG] [-i] [-w]
+usage: mbs gen [-h] [-c CONFIG] [-i] [-w] [-s]
 
 options:
   -h, --help            show this help message and exit
   -c CONFIG, --config CONFIG
                         the path to the top-level configuration file (default:
                         'yambs.yaml')
   -i, --single-pass     only run a single watch iteration
   -w, --watch           whether or not to continue watching for source tree
                         changes
+  -s, --sources         whether or not to only re-generate source manifests
 
 ```
 
 ### `native`
 
 ```
 $ ./venv3.11/bin/mbs native -h
 
-usage: mbs native [-h] [-c CONFIG] [-i] [-w] [variants ...]
-
-positional arguments:
-  variants              variants to build (defaults to 'debug' if not
-                        specified)
+usage: mbs native [-h] [-c CONFIG] [-i] [-w] [-s]
 
 options:
   -h, --help            show this help message and exit
   -c CONFIG, --config CONFIG
                         the path to the top-level configuration file (default:
                         'yambs.yaml')
   -i, --single-pass     only run a single watch iteration
   -w, --watch           whether or not to continue watching for source tree
                         changes
+  -s, --sources         whether or not to only re-generate source manifests
 
 ```
 
 ### `uf2conv`
 
 ```
 $ ./venv3.11/bin/mbs uf2conv -h
```

### Comparing `yambs-1.8.0/pyproject.toml` & `yambs-1.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "yambs"
-version = "1.8.0"
+version = "1.8.1"
 description = "Yet another meta build-system."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `yambs-1.8.0/setup.py` & `yambs-1.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.0/tests/test_entry.py` & `yambs-1.8.1/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.0/yambs/aggregation/__init__.py` & `yambs-1.8.1/yambs/aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.0/yambs/app.py` & `yambs-1.8.1/yambs/app.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.0/yambs/commands/all.py` & `yambs-1.8.1/yambs/commands/all.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.0/yambs/commands/common.py` & `yambs-1.8.1/yambs/commands/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,14 +38,20 @@
     )
     parser.add_argument(
         "-w",
         "--watch",
         action="store_true",
         help="whether or not to continue watching for source tree changes",
     )
+    parser.add_argument(
+        "-s",
+        "--sources",
+        action="store_true",
+        help="whether or not to only re-generate source manifests",
+    )
 
 
 def run_watch(args: _Namespace, src_root: _Path, command: str) -> int:
     """Run the 'watch' command from rcmpy."""
 
     return (
         watch(
@@ -55,14 +61,15 @@
                 [
                     executable,
                     "-m",
                     PKG_NAME,
                     "-C",
                     str(args.dir),
                     command,
+                    "-s",
                     "-c",
                     str(args.config),
                 ],
                 False,  # Don't check file contents.
                 single_pass=args.single_pass,
             )
         )
```

### Comparing `yambs-1.8.0/yambs/commands/gen.py` & `yambs-1.8.1/yambs/commands/gen.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from yambs.generate import generate
 
 
 def gen_cmd(args: _Namespace) -> int:
     """Execute the gen command."""
 
     config = Config.load(path=args.config, root=args.dir)
-    generate(BuildEnvironment(config))
+    generate(BuildEnvironment(config), sources_only=args.sources)
     return run_watch(args, config.src_root, "gen")
 
 
 def add_gen_cmd(parser: _ArgumentParser) -> _CommandFunction:
     """Add gen-command arguments to its parser."""
 
     add_common_args(parser)
```

### Comparing `yambs-1.8.0/yambs/commands/native.py` & `yambs-1.8.1/yambs/commands/native.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 def native_cmd(args: _Namespace) -> int:
     """Execute the native command."""
 
     config = Native.load(
         path=args.config, root=args.dir, package_config="native.yaml"
     )
 
-    NativeBuildEnvironment(config).generate()
+    NativeBuildEnvironment(config).generate(sources_only=args.sources)
 
     return run_watch(args, config.src_root, "native")
 
 
 def add_native_cmd(parser: _ArgumentParser) -> _CommandFunction:
     """Add native-command arguments to its parser."""
```

### Comparing `yambs-1.8.0/yambs/commands/uf2conv.py` & `yambs-1.8.1/yambs/commands/uf2conv.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.0/yambs/config/__init__.py` & `yambs-1.8.1/yambs/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.0/yambs/config/board.py` & `yambs-1.8.1/yambs/config/board.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.0/yambs/config/common.py` & `yambs-1.8.1/yambs/config/common.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.0/yambs/data/includes/chips.yaml` & `yambs-1.8.1/yambs/data/includes/chips.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.8.0/yambs/data/includes/infineon.yaml` & `yambs-1.8.1/yambs/data/includes/infineon.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.8.0/yambs/data/includes/microchip.yaml` & `yambs-1.8.1/yambs/data/includes/microchip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.8.0/yambs/data/schemas/Chip.yaml` & `yambs-1.8.1/yambs/data/schemas/Chip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.8.0/yambs/data/schemas/Config.yaml` & `yambs-1.8.1/yambs/data/schemas/Config.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.8.0/yambs/data/templates/rules.ninja.j2` & `yambs-1.8.1/yambs/data/templates/rules.ninja.j2`

 * *Files identical despite different names*

### Comparing `yambs-1.8.0/yambs/data/uf2families.json` & `yambs-1.8.1/yambs/data/uf2families.json`

 * *Files identical despite different names*

### Comparing `yambs-1.8.0/yambs/entry.py` & `yambs-1.8.1/yambs/entry.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # =====================================
 # generator=datazen
 # version=3.1.2
-# hash=b91b2bf582f2f6003066e15b2489ac0f
+# hash=a0185de1511c495d696086ed16024449
 # =====================================
 
 """
 This package's command-line entry-point (boilerplate).
 """
 
 # built-in
 import argparse
 import logging
 import os
 from pathlib import Path
 import sys
 from typing import List
 
+# third-party
+from vcorelib.logging import log_time as _log_time
+
 # internal
 from yambs import DESCRIPTION, VERSION
 from yambs.app import add_app_args, entry
 
 
 def main(argv: List[str] = None) -> int:
     """Program entry-point."""
@@ -69,15 +72,16 @@
             format="%(name)-36s - %(levelname)-6s - %(message)s",
         )
 
         # change to the specified directory
         os.chdir(args.dir)
 
         # run the application
-        result = entry(args)
+        with _log_time(logging.getLogger(__name__), "Command"):
+            result = entry(args)
     except SystemExit as exc:
         result = 1
         if exc.code is not None and isinstance(exc.code, int):
             result = exc.code
 
     # return to starting dir
     os.chdir(starting_dir)
```

### Comparing `yambs-1.8.0/yambs/environment/__init__.py` & `yambs-1.8.1/yambs/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.0/yambs/environment/native.py` & `yambs-1.8.1/yambs/environment/native.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,17 +38,19 @@
             self.sources, config.src_root, self.apps, self.regular
         )
 
         self.jinja = get_jinja()
 
     def render(self, root: Path, name: str) -> None:
         """Render a template."""
+
         render_template(
             self.jinja, root, f"native_{name}", self.config.data, out=name
         )
+        self.logger.info("Rendered '%s'.", root.joinpath(name))
 
     def write_compile_line(self, stream: TextIO, path: Path) -> Path:
         """Write a single source-compile line."""
 
         translator = get_translator(path)
         from_src = path.relative_to(self.config.src_root)
 
@@ -94,30 +96,31 @@
         for elf in elfs[1:]:
             write_continuation(stream, offset)
             stream.write(str(elf))
         stream.write(linesep)
 
         return elfs
 
-    def generate(self) -> None:
+    def generate(self, sources_only: bool = False) -> None:
         """Generate ninja files."""
 
-        # Render templates.
-        generate_variants(self.jinja, self.config)
-        self.render(self.config.root, "build.ninja")
-        for template in ["all", "rules"]:
-            self.render(self.config.ninja_root, f"{template}.ninja")
+        if not sources_only:
+            # Render templates.
+            generate_variants(self.jinja, self.config)
+            self.render(self.config.root, "build.ninja")
+            for template in ["all", "rules"]:
+                self.render(self.config.ninja_root, f"{template}.ninja")
 
         # Render sources file.
-        with self.config.ninja_root.joinpath("sources.ninja").open(
-            "w"
-        ) as path_fd:
+        path = self.config.ninja_root.joinpath("sources.ninja")
+        with path.open("w") as path_fd:
             outputs = self.write_source_rules(path_fd)
+            self.logger.info("Wrote '%s'.", path)
 
         # Render apps file.
-        with self.config.ninja_root.joinpath("apps.ninja").open(
-            "w"
-        ) as path_fd:
+        path = self.config.ninja_root.joinpath("apps.ninja")
+        with path.open("w") as path_fd:
             self.write_app_rules(path_fd, outputs)
+            self.logger.info("Wrote '%s'.", path)
 
         # Render format file.
         render_format(self.config, sources_headers(self.sources))
```

### Comparing `yambs-1.8.0/yambs/generate/__init__.py` & `yambs-1.8.1/yambs/generate/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -38,33 +38,40 @@
 
     ARBITER.encode(
         env.config.ninja_root.joinpath("board_apps.json"),
         board_apps,
     )
 
 
-def generate(env: BuildEnvironment) -> None:
+def generate(env: BuildEnvironment, sources_only: bool = False) -> None:
     """Generate ninja files."""
 
     templates_dir = resource("templates", package=PKG_NAME)
     assert templates_dir is not None
 
     jinja = get_jinja()
 
-    # Render the top-level configuration. This is the only file that's
-    # generated into the root directory.
-    render_template(jinja, env.config.root, "build.ninja", env.config.data)
-
-    # Generate all other files.
-    for gen in [
-        generate_chips,
-        generate_toolchains,
-        generate_architectures,
-    ]:
-        gen(jinja, env.config)
+    if not sources_only:
+        # Render the top-level configuration. This is the only file that's
+        # generated into the root directory.
+        render_template(jinja, env.config.root, "build.ninja", env.config.data)
+
+        # Generate all other files.
+        for gen in [
+            generate_chips,
+            generate_toolchains,
+            generate_architectures,
+        ]:
+            gen(jinja, env.config)
+
+        # Render the board manifest and rules file.
+        for template in ["all.ninja", "rules.ninja"]:
+            render_template(
+                jinja, env.config.ninja_root, template, env.config.data
+            )
 
-    generate_boards(jinja, env)
+    generate_boards(jinja, env, sources_only=sources_only)
 
     create_board_apps(env)
 
     # Create format configuration.
     render_format(env.config, env.first_party_sources_headers())
```

### Comparing `yambs-1.8.0/yambs/generate/architectures.py` & `yambs-1.8.1/yambs/generate/architectures.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.0/yambs/generate/boards.py` & `yambs-1.8.1/yambs/generate/boards.py`

 * *Files 4% similar despite different names*

```diff
@@ -154,28 +154,30 @@
     # Keep track of all header files.
     env.first_party_headers.update(headers)
 
     # Populate board sources.
     return env.set_board_sources(board, all_srcs, app_srcs)
 
 
-def generate(jinja: Environment, env: BuildEnvironment) -> None:
+def generate(
+    jinja: Environment, env: BuildEnvironment, sources_only: bool = False
+) -> None:
     """Generate board-related ninja files."""
 
-    # Render the board manifest and rules file.
-    for template in ["all.ninja", "rules.ninja"]:
-        render_template(
-            jinja, env.config.ninja_root, template, env.config.data
-        )
-
-    src_root = rel(env.config.src_root)
-
     for board, raw_data in env.config.boards():
         board_root = env.config.ninja_root.joinpath("boards", board.name)
         board_root.mkdir(parents=True, exist_ok=True)
-        render_template(jinja, board_root, "board.ninja", raw_data)
 
-        # Perform source-file discovery.
-        with board_root.joinpath("sources.ninja").open("w") as path_fd:
-            sources = write_sources(path_fd, board, src_root, env)
+        if not sources_only:
+            render_template(jinja, board_root, "board.ninja", raw_data)
 
-        write_link_lines(board_root, src_root, board, sources)
+        src_root = rel(env.config.src_root)
+
+        # Perform source-file discovery.
+        with board_root.joinpath("sources.ninja").open("w") as sources_fd:
+            with board_root.joinpath("apps.ninja").open("w") as apps_fd:
+                write_link_lines(
+                    apps_fd,
+                    src_root,
+                    board,
+                    write_sources(sources_fd, board, src_root, env),
+                )
```

### Comparing `yambs-1.8.0/yambs/generate/chips.py` & `yambs-1.8.1/yambs/generate/chips.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.0/yambs/generate/common.py` & `yambs-1.8.1/yambs/generate/common.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.0/yambs/generate/ninja/__init__.py` & `yambs-1.8.1/yambs/generate/ninja/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -119,28 +119,27 @@
         for src, trans in implicit[1:]:
             write_continuation(stream, offset)
             stream.write(str(trans.output(src.relative_to(src_root))))
     stream.write(linesep + linesep)
 
 
 def write_link_lines(
-    board_root: Path, src_root: Path, board: Board, sources: SourceSets
+    stream: TextIO, src_root: Path, board: Board, sources: SourceSets
 ) -> None:
     """Write the application manifest and phony targets."""
 
     # Write the application manifest.
-    with board_root.joinpath("apps.ninja").open("w") as path_fd:
-        for app_src in sources.apps:
-            write_link_line(path_fd, app_src, src_root, board, sources)
-
-        write_generated_phony(path_fd, sources, src_root)
-
-        # Write the phony target.
-        path_fd.write("# A target to build all applications." + linesep)
-        write_phony(path_fd, sources.apps, src_root, board.name)
+    for app_src in sources.apps:
+        write_link_line(stream, app_src, src_root, board, sources)
+
+    write_generated_phony(stream, sources, src_root)
+
+    # Write the phony target.
+    stream.write("# A target to build all applications." + linesep)
+    write_phony(stream, sources.apps, src_root, board.name)
 
 
 def write_phony(
     stream: TextIO, app_srcs: Set[Path], base: Path, board: str
 ) -> None:
     """Write the phony target."""
```

### Comparing `yambs-1.8.0/yambs/generate/ninja/format.py` & `yambs-1.8.1/yambs/generate/ninja/format.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.0/yambs/generate/toolchains.py` & `yambs-1.8.1/yambs/generate/toolchains.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.0/yambs/generate/variants.py` & `yambs-1.8.1/yambs/generate/variants.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.0/yambs/schemas.py` & `yambs-1.8.1/yambs/schemas.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.0/yambs/translation/__init__.py` & `yambs-1.8.1/yambs/translation/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.0/yambs/uf2/__init__.py` & `yambs-1.8.1/yambs/uf2/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.0/yambs.egg-info/PKG-INFO` & `yambs-1.8.1/yambs.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 1.8.0
+Version: 1.8.1
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=c88caeb9c6d71c51d9fd724250cd248c
+    hash=47efb6aab42b656852a2fdb9a25350fe
     =====================================
 -->
 
-# yambs ([1.8.0](https://pypi.org/project/yambs/))
+# yambs ([1.8.1](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
 
@@ -177,46 +177,44 @@
 ## Sub-command Options
 
 ### `gen`
 
 ```
 $ ./venv3.11/bin/mbs gen -h
 
-usage: mbs gen [-h] [-c CONFIG] [-i] [-w]
+usage: mbs gen [-h] [-c CONFIG] [-i] [-w] [-s]
 
 options:
   -h, --help            show this help message and exit
   -c CONFIG, --config CONFIG
                         the path to the top-level configuration file (default:
                         'yambs.yaml')
   -i, --single-pass     only run a single watch iteration
   -w, --watch           whether or not to continue watching for source tree
                         changes
+  -s, --sources         whether or not to only re-generate source manifests
 
 ```
 
 ### `native`
 
 ```
 $ ./venv3.11/bin/mbs native -h
 
-usage: mbs native [-h] [-c CONFIG] [-i] [-w] [variants ...]
-
-positional arguments:
-  variants              variants to build (defaults to 'debug' if not
-                        specified)
+usage: mbs native [-h] [-c CONFIG] [-i] [-w] [-s]
 
 options:
   -h, --help            show this help message and exit
   -c CONFIG, --config CONFIG
                         the path to the top-level configuration file (default:
                         'yambs.yaml')
   -i, --single-pass     only run a single watch iteration
   -w, --watch           whether or not to continue watching for source tree
                         changes
+  -s, --sources         whether or not to only re-generate source manifests
 
 ```
 
 ### `uf2conv`
 
 ```
 $ ./venv3.11/bin/mbs uf2conv -h
```

### Comparing `yambs-1.8.0/yambs.egg-info/SOURCES.txt` & `yambs-1.8.1/yambs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

