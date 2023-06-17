# Comparing `tmp/yambs-1.8.1.tar.gz` & `tmp/yambs-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yambs-1.8.1.tar", last modified: Sat Jun 17 06:31:03 2023, max compression
+gzip compressed data, was "yambs-1.8.2.tar", last modified: Sat Jun 17 20:17:42 2023, max compression
```

## Comparing `yambs-1.8.1.tar` & `yambs-1.8.2.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:31:03.665854 yambs-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-17 06:29:55.000000 yambs-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9507 2023-06-17 06:31:03.665854 yambs-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-06-17 06:29:55.000000 yambs-1.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-17 06:29:55.000000 yambs-1.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 06:31:03.665854 yambs-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-17 06:29:55.000000 yambs-1.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:31:03.657854 yambs-1.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-17 06:29:55.000000 yambs-1.8.1/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-17 06:29:55.000000 yambs-1.8.1/tests/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:31:03.661854 yambs-1.8.1/yambs/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:31:03.661854 yambs-1.8.1/yambs/aggregation/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/aggregation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:31:03.661854 yambs-1.8.1/yambs/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/commands/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/commands/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/commands/uf2conv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:31:03.661854 yambs-1.8.1/yambs/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/config/board.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/config/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/config/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:31:03.661854 yambs-1.8.1/yambs/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:31:03.661854 yambs-1.8.1/yambs/data/includes/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/includes/chips.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/includes/infineon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/includes/microchip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/native.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:31:03.661854 yambs-1.8.1/yambs/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/schemas/Architecture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/schemas/Board.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/schemas/Chip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/schemas/Native.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/schemas/Toolchain.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/schemas/Variant.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/schemas/config_common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/schemas/targets_common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/schemas/toolchain_common.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:31:03.665854 yambs-1.8.1/yambs/data/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/templates/all.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/templates/architecture.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/templates/board.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/templates/build.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/templates/chip.ld.j2
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/templates/chip.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/templates/compile_commands.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/templates/native_all.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/templates/native_build.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/templates/native_rules.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/templates/rules.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/templates/toolchain.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/templates/variant.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/uf2families.json
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/data/yambs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:31:03.665854 yambs-1.8.1/yambs/environment/
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/environment/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:31:03.665854 yambs-1.8.1/yambs/generate/
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/generate/architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/generate/boards.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/generate/chips.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/generate/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:31:03.665854 yambs-1.8.1/yambs/generate/ninja/
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/generate/ninja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/generate/ninja/format.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/generate/toolchains.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/generate/variants.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:31:03.665854 yambs-1.8.1/yambs/translation/
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/translation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:31:03.665854 yambs-1.8.1/yambs/uf2/
--rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-06-17 06:29:55.000000 yambs-1.8.1/yambs/uf2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:31:03.661854 yambs-1.8.1/yambs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9507 2023-06-17 06:31:03.000000 yambs-1.8.1/yambs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-17 06:31:03.000000 yambs-1.8.1/yambs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 06:31:03.000000 yambs-1.8.1/yambs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-17 06:31:03.000000 yambs-1.8.1/yambs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-17 06:31:03.000000 yambs-1.8.1/yambs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-17 06:31:03.000000 yambs-1.8.1/yambs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:17:42.007165 yambs-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-17 20:16:05.000000 yambs-1.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9507 2023-06-17 20:17:42.007165 yambs-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-06-17 20:16:05.000000 yambs-1.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-17 20:16:05.000000 yambs-1.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 20:17:42.007165 yambs-1.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-17 20:16:05.000000 yambs-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:17:41.995165 yambs-1.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-17 20:16:05.000000 yambs-1.8.2/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-17 20:16:05.000000 yambs-1.8.2/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:17:41.995165 yambs-1.8.2/yambs/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:17:41.999165 yambs-1.8.2/yambs/aggregation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/aggregation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:17:41.999165 yambs-1.8.2/yambs/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/commands/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/commands/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/commands/uf2conv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:17:41.999165 yambs-1.8.2/yambs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/config/board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/config/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/config/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:17:41.999165 yambs-1.8.2/yambs/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:17:41.999165 yambs-1.8.2/yambs/data/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/data/includes/chips.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/data/includes/infineon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/data/includes/microchip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/data/native.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:17:42.003165 yambs-1.8.2/yambs/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/data/schemas/Architecture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/data/schemas/Board.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/data/schemas/Chip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/data/schemas/Native.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/data/schemas/Toolchain.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/data/schemas/Variant.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/data/schemas/config_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/data/schemas/targets_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/data/schemas/toolchain_common.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:17:42.007165 yambs-1.8.2/yambs/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/data/templates/all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/data/templates/architecture.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/data/templates/board.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/data/templates/build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/data/templates/chip.ld.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/data/templates/chip.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/data/templates/compile_commands.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/data/templates/native_all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/data/templates/native_build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/data/templates/native_rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/data/templates/rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/data/templates/toolchain.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/data/templates/variant.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/data/uf2families.json
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/data/yambs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:17:42.007165 yambs-1.8.2/yambs/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/environment/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:17:42.007165 yambs-1.8.2/yambs/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/generate/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/generate/boards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/generate/chips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/generate/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:17:42.007165 yambs-1.8.2/yambs/generate/ninja/
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/generate/ninja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/generate/ninja/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/generate/toolchains.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/generate/variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:17:42.007165 yambs-1.8.2/yambs/translation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/translation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:17:42.007165 yambs-1.8.2/yambs/uf2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-06-17 20:16:05.000000 yambs-1.8.2/yambs/uf2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:17:41.999165 yambs-1.8.2/yambs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9507 2023-06-17 20:17:41.000000 yambs-1.8.2/yambs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-17 20:17:41.000000 yambs-1.8.2/yambs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 20:17:41.000000 yambs-1.8.2/yambs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-17 20:17:41.000000 yambs-1.8.2/yambs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-17 20:17:41.000000 yambs-1.8.2/yambs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-17 20:17:41.000000 yambs-1.8.2/yambs.egg-info/top_level.txt
```

### Comparing `yambs-1.8.1/LICENSE` & `yambs-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yambs-1.8.1/PKG-INFO` & `yambs-1.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 1.8.1
+Version: 1.8.2
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
-    hash=47efb6aab42b656852a2fdb9a25350fe
+    hash=1d25551d127ed936a4712191902c78eb
     =====================================
 -->
 
-# yambs ([1.8.1](https://pypi.org/project/yambs/))
+# yambs ([1.8.2](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-1.8.1/README.md` & `yambs-1.8.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=47efb6aab42b656852a2fdb9a25350fe
+    hash=1d25551d127ed936a4712191902c78eb
     =====================================
 -->
 
-# yambs ([1.8.1](https://pypi.org/project/yambs/))
+# yambs ([1.8.2](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-1.8.1/pyproject.toml` & `yambs-1.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "yambs"
-version = "1.8.1"
+version = "1.8.2"
 description = "Yet another meta build-system."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `yambs-1.8.1/setup.py` & `yambs-1.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.1/tests/test_entry.py` & `yambs-1.8.2/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.1/yambs/aggregation/__init__.py` & `yambs-1.8.2/yambs/aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.1/yambs/app.py` & `yambs-1.8.2/yambs/app.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.1/yambs/commands/all.py` & `yambs-1.8.2/yambs/commands/all.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.1/yambs/commands/common.py` & `yambs-1.8.2/yambs/commands/common.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.1/yambs/commands/gen.py` & `yambs-1.8.2/yambs/commands/gen.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.1/yambs/commands/native.py` & `yambs-1.8.2/yambs/commands/native.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.1/yambs/commands/uf2conv.py` & `yambs-1.8.2/yambs/commands/uf2conv.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.1/yambs/config/__init__.py` & `yambs-1.8.2/yambs/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.1/yambs/config/board.py` & `yambs-1.8.2/yambs/config/board.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.1/yambs/config/common.py` & `yambs-1.8.2/yambs/config/common.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.1/yambs/data/includes/chips.yaml` & `yambs-1.8.2/yambs/data/includes/chips.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.8.1/yambs/data/includes/infineon.yaml` & `yambs-1.8.2/yambs/data/includes/infineon.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.8.1/yambs/data/includes/microchip.yaml` & `yambs-1.8.2/yambs/data/includes/microchip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.8.1/yambs/data/schemas/Chip.yaml` & `yambs-1.8.2/yambs/data/schemas/Chip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.8.1/yambs/data/schemas/Config.yaml` & `yambs-1.8.2/yambs/data/schemas/Config.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.8.1/yambs/data/templates/rules.ninja.j2` & `yambs-1.8.2/yambs/data/templates/rules.ninja.j2`

 * *Files identical despite different names*

### Comparing `yambs-1.8.1/yambs/data/uf2families.json` & `yambs-1.8.2/yambs/data/uf2families.json`

 * *Files identical despite different names*

### Comparing `yambs-1.8.1/yambs/entry.py` & `yambs-1.8.2/yambs/entry.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.1/yambs/environment/__init__.py` & `yambs-1.8.2/yambs/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.1/yambs/generate/__init__.py` & `yambs-1.8.2/yambs/generate/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.1/yambs/generate/architectures.py` & `yambs-1.8.2/yambs/generate/architectures.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.1/yambs/generate/boards.py` & `yambs-1.8.2/yambs/generate/boards.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.1/yambs/generate/chips.py` & `yambs-1.8.2/yambs/generate/chips.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.1/yambs/generate/common.py` & `yambs-1.8.2/yambs/generate/common.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.1/yambs/generate/ninja/__init__.py` & `yambs-1.8.2/yambs/generate/ninja/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from os import linesep
 from pathlib import Path
 from typing import Set, TextIO
 
 # internal
 from yambs.config.board import Board
 from yambs.environment import SourceSets
-from yambs.translation import SourceTranslator
+from yambs.translation import BUILD_DIR_VAR, SourceTranslator
 
 
 def write_source_line(
     stream: TextIO,
     source: Path,
     base: Path,
     current_sources: Set[Path],
@@ -66,36 +66,40 @@
     source = source.relative_to(base)
 
     by_suffix = {
         x: source.with_suffix(f".{x}")
         for x in ["o", "elf", "bin", "hex", "dump", "uf2"]
     }
 
-    elf = f"$build_dir/{by_suffix['elf']}"
+    elf = f"{BUILD_DIR_VAR}/{by_suffix['elf']}"
     line = f"build {elf}: link "
     offset = " " * len(line)
-    stream.write(line + f"$build_dir/{by_suffix['o']}")
+    stream.write(line + f"{BUILD_DIR_VAR}/{by_suffix['o']}")
 
     for src, trans in sources.link_sources():
         write_continuation(stream, offset)
         stream.write(str(trans.output(src.relative_to(base))))
     stream.write(linesep)
 
     # Add lines for creating binaries.
-    stream.write(f"build $build_dir/{by_suffix['bin']}: bin {elf}" + linesep)
+    stream.write(
+        f"build {BUILD_DIR_VAR}/{by_suffix['bin']}: bin {elf}" + linesep
+    )
 
     # Add an objdump target.
-    stream.write(f"build $build_dir/{by_suffix['dump']}: dump {elf}" + linesep)
+    stream.write(
+        f"build {BUILD_DIR_VAR}/{by_suffix['dump']}: dump {elf}" + linesep
+    )
 
     # Add an hex target.
-    hex_path = f"$build_dir/{by_suffix['hex']}"
+    hex_path = f"{BUILD_DIR_VAR}/{by_suffix['hex']}"
     stream.write(f"build {hex_path}: hex {elf}" + linesep)
 
     # Add a uf2 target.
-    stream.write(f"build $build_dir/{by_suffix['uf2']}: uf2 {hex_path}")
+    stream.write(f"build {BUILD_DIR_VAR}/{by_suffix['uf2']}: uf2 {hex_path}")
 
     stream.write(linesep + linesep)
 
     # Add this application to the board's data structure.
     out = by_suffix["elf"].with_suffix("")
     board.apps[str(out)] = board.build.joinpath(out)
 
@@ -154,14 +158,14 @@
         for phony, suffix in phonies:
             srcs = list(app_srcs)
             first = srcs[0].relative_to(base)
             srcs = srcs[1:]
 
             line = f"build {board}_{phony}: phony "
             offset = " " * len(line)
-            stream.write(line + f"$build_dir/{first.with_suffix(suffix)}")
+            stream.write(line + f"{BUILD_DIR_VAR}/{first.with_suffix(suffix)}")
             for src in srcs:
                 write_continuation(stream, offset)
                 src = src.relative_to(base)
-                stream.write(f"$build_dir/{src.with_suffix(suffix)}")
+                stream.write(f"{BUILD_DIR_VAR}/{src.with_suffix(suffix)}")
 
             stream.write(linesep)
```

### Comparing `yambs-1.8.1/yambs/generate/ninja/format.py` & `yambs-1.8.2/yambs/generate/ninja/format.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.1/yambs/generate/toolchains.py` & `yambs-1.8.2/yambs/generate/toolchains.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.1/yambs/generate/variants.py` & `yambs-1.8.2/yambs/generate/variants.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.1/yambs/schemas.py` & `yambs-1.8.2/yambs/schemas.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.1/yambs/translation/__init__.py` & `yambs-1.8.2/yambs/translation/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,25 +5,26 @@
 
 # built-in
 from functools import lru_cache
 from pathlib import Path
 from typing import NamedTuple, Optional
 
 HEADER_EXTENSIONS = {".h", ".hpp"}
+BUILD_DIR_VAR = "$build_dir"
 
 
 class SourceTranslator(NamedTuple):
     """
     A structure for keeping track of how source files become different types
     of output files.
     """
 
     rule: str = "cc"
     output_extension: str = ".o"
-    dest: Path = Path("$build_dir")
+    dest: Path = Path(BUILD_DIR_VAR)
 
     def output(self, path: Path) -> Path:
         """Get the output file from a given path."""
         return self.dest.joinpath(path.with_suffix(self.output_extension))
 
     @property
     def gets_linked(self) -> bool:
```

### Comparing `yambs-1.8.1/yambs/uf2/__init__.py` & `yambs-1.8.2/yambs/uf2/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.8.1/yambs.egg-info/PKG-INFO` & `yambs-1.8.2/yambs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 1.8.1
+Version: 1.8.2
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
-    hash=47efb6aab42b656852a2fdb9a25350fe
+    hash=1d25551d127ed936a4712191902c78eb
     =====================================
 -->
 
-# yambs ([1.8.1](https://pypi.org/project/yambs/))
+# yambs ([1.8.2](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-1.8.1/yambs.egg-info/SOURCES.txt` & `yambs-1.8.2/yambs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

