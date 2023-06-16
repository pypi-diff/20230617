# Comparing `tmp/cortex_command_mod_converter_engine-1.0.8.tar.gz` & `tmp/cortex_command_mod_converter_engine-1.0.9.tar.gz`

## Comparing `cortex_command_mod_converter_engine-1.0.8.tar` & `cortex_command_mod_converter_engine-1.0.9.tar`

### file list

```diff
@@ -1,89 +1,91 @@
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/example.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/test.py
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/conversion_rules/before_pre4/gibs.json
--rw-r--r--   0        0        0    21620 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/conversion_rules/before_pre4/images.json
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/conversion_rules/before_pre4/lua.json
--rw-r--r--   0        0        0    14355 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/conversion_rules/before_pre4/misc.json
--rw-r--r--   0        0        0    13372 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/conversion_rules/before_pre4/sounds.json
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/conversion_rules/pre4/images.json
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/conversion_rules/pre4/lua.json
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/conversion_rules/pre4/misc.json
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/conversion_rules/pre4/new_unit_names.json
--rw-r--r--   0        0        0     7911 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/conversion_rules/pre4/sounds.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/__init__.py
--rw-r--r--   0        0        0     8123 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/bmp_to_png.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/cfg.py
--rw-r--r--   0        0        0     7144 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/convert.py
--rw-r--r--   0        0        0     6854 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/regex_rules.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/stylua.py
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/thumbnail_generator.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/utils.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/zips.py
--rw-r--r--   0        0        0     6342 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/case_check/case_check.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/case_check/case_check_errors.py
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/ini_converting/ini_cst.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/ini_converting/ini_cst_builder.py
--rw-r--r--   0        0        0    22359 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/ini_converting/ini_rules.py
--rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/ini_converting/ini_rules_utils.py
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/ini_converting/ini_tokenizer.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/ini_converting/ini_writer.py
--rw-r--r--   0        0        0  9672192 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/stylua_executables/linux/stylua
--rwxr-xr-x   0        0        0  5359616 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/stylua_executables/windows/stylua.exe
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/__init__.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/get_test_path_from_filename.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/test_ini_conversion.py
--rw-r--r--   0        0        0    48341 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/test_ini_cst.py
--rw-r--r--   0        0        0    28514 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/test_ini_tokenizer.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/conversion/add_grip_strength_if_missing/in.ini
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/conversion/add_grip_strength_if_missing/out.ini
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/conversion/max_length_to_offsets/in.ini
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/conversion/max_length_to_offsets/out.ini
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/conversion/max_mass_to_max_inventory_mass/in.ini
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/conversion/max_mass_to_max_inventory_mass/out.ini
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/conversion/max_throttle_range_to_positive_throttle_multiplier/in.ini
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/conversion/max_throttle_range_to_positive_throttle_multiplier/out.ini
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/conversion/min_throttle_range_to_negative_throttle_multiplier/in.ini
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/conversion/min_throttle_range_to_negative_throttle_multiplier/out.ini
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/conversion/pie_menu_fix/crab/in.ini
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/conversion/pie_menu_fix/crab/out.ini
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/conversion/pie_menu_fix/dropship/in.ini
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/conversion/pie_menu_fix/dropship/out.ini
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/conversion/pie_menu_fix/firearm/in.ini
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/conversion/pie_menu_fix/firearm/out.ini
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/conversion/pie_menu_fix/human/in.ini
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/conversion/pie_menu_fix/human/out.ini
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/conversion/remove_sl_terrain_properties/in.ini
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/conversion/remove_sl_terrain_properties/out.ini
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/conversion/shovel_flash_fix/in.ini
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/conversion/shovel_flash_fix/out.ini
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/conversion/supported_game_version/add/in.ini
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/conversion/supported_game_version/add/out.ini
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/conversion/supported_game_version/update/in.ini
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/conversion/supported_game_version/update/out.ini
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/token_and_cst/comment_across_multiline_tabs.ini
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/token_and_cst/comment_before_tabs.ini
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/token_and_cst/comment_in_tabs.ini
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/token_and_cst/comments.ini
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/token_and_cst/complex.ini
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/token_and_cst/datamodule.ini
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/token_and_cst/deindentation_1.ini
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/token_and_cst/deindentation_2.ini
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/token_and_cst/deindentation_3.ini
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/token_and_cst/include_files.ini
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/token_and_cst/invalid_tabbing.ini
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/token_and_cst/lstripped_tab.ini
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/token_and_cst/multiple.ini
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/token_and_cst/nested.ini
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/token_and_cst/object_and_property.ini
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/token_and_cst/path.ini
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/token_and_cst/simple.ini
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/token_and_cst/spaces.ini
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/token_and_cst/spaces_at_start_of_line.ini
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/token_and_cst/tabbed_comment.ini
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/token_and_cst/traditional.ini
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/token_and_cst/value_on_next_line.ini
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/.gitignore
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/LICENSE
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/README.md
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/example.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/test.py
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/conversion_rules/before_pre4/gibs.json
+-rw-r--r--   0        0        0    21620 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/conversion_rules/before_pre4/images.json
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/conversion_rules/before_pre4/lua.json
+-rw-r--r--   0        0        0    14355 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/conversion_rules/before_pre4/misc.json
+-rw-r--r--   0        0        0    13372 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/conversion_rules/before_pre4/sounds.json
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/conversion_rules/pre4/images.json
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/conversion_rules/pre4/lua.json
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/conversion_rules/pre4/misc.json
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/conversion_rules/pre4/new_unit_names.json
+-rw-r--r--   0        0        0     7911 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/conversion_rules/pre4/sounds.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/__init__.py
+-rw-r--r--   0        0        0     8123 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/bmp_to_png.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/cfg.py
+-rw-r--r--   0        0        0     7569 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/convert.py
+-rw-r--r--   0        0        0     6854 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/regex_rules.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/stylua.py
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/thumbnail_generator.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/utils.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/zips.py
+-rw-r--r--   0        0        0     6342 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/case_check/case_check.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/case_check/case_check_errors.py
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/ini_converting/ini_cst.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/ini_converting/ini_cst_builder.py
+-rw-r--r--   0        0        0    22449 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/ini_converting/ini_rules.py
+-rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/ini_converting/ini_rules_utils.py
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/ini_converting/ini_tokenizer.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/ini_converting/ini_writer.py
+-rw-r--r--   0        0        0  9672192 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/stylua_executables/linux/stylua
+-rwxr-xr-x   0        0        0  5359616 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/stylua_executables/windows/stylua.exe
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/__init__.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/get_test_path_from_filename.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/test_ini_conversion.py
+-rw-r--r--   0        0        0    48341 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/test_ini_cst.py
+-rw-r--r--   0        0        0    28514 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/test_ini_tokenizer.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/conversion/add_grip_strength_if_missing/in.ini
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/conversion/add_grip_strength_if_missing/out.ini
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/conversion/max_length_to_offsets/in.ini
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/conversion/max_length_to_offsets/out.ini
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/conversion/max_mass_to_max_inventory_mass/in.ini
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/conversion/max_mass_to_max_inventory_mass/out.ini
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/conversion/max_throttle_range_to_positive_throttle_multiplier/in.ini
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/conversion/max_throttle_range_to_positive_throttle_multiplier/out.ini
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/conversion/min_throttle_range_to_negative_throttle_multiplier/in.ini
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/conversion/min_throttle_range_to_negative_throttle_multiplier/out.ini
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/conversion/pie_menu_fix/any/in.ini
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/conversion/pie_menu_fix/any/out.ini
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/conversion/pie_menu_fix/crab/in.ini
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/conversion/pie_menu_fix/crab/out.ini
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/conversion/pie_menu_fix/dropship/in.ini
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/conversion/pie_menu_fix/dropship/out.ini
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/conversion/pie_menu_fix/firearm/in.ini
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/conversion/pie_menu_fix/firearm/out.ini
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/conversion/pie_menu_fix/human/in.ini
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/conversion/pie_menu_fix/human/out.ini
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/conversion/remove_sl_terrain_properties/in.ini
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/conversion/remove_sl_terrain_properties/out.ini
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/conversion/shovel_flash_fix/in.ini
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/conversion/shovel_flash_fix/out.ini
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/conversion/supported_game_version/add/in.ini
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/conversion/supported_game_version/add/out.ini
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/conversion/supported_game_version/update/in.ini
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/conversion/supported_game_version/update/out.ini
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/token_and_cst/comment_across_multiline_tabs.ini
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/token_and_cst/comment_before_tabs.ini
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/token_and_cst/comment_in_tabs.ini
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/token_and_cst/comments.ini
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/token_and_cst/complex.ini
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/token_and_cst/datamodule.ini
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/token_and_cst/deindentation_1.ini
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/token_and_cst/deindentation_2.ini
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/token_and_cst/deindentation_3.ini
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/token_and_cst/include_files.ini
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/token_and_cst/invalid_tabbing.ini
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/token_and_cst/lstripped_tab.ini
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/token_and_cst/multiple.ini
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/token_and_cst/nested.ini
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/token_and_cst/object_and_property.ini
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/token_and_cst/path.ini
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/token_and_cst/simple.ini
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/token_and_cst/spaces.ini
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/token_and_cst/spaces_at_start_of_line.ini
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/token_and_cst/tabbed_comment.ini
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/token_and_cst/traditional.ini
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/token_and_cst/value_on_next_line.ini
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/.gitignore
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/LICENSE
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/README.md
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 cortex_command_mod_converter_engine-1.0.9/PKG-INFO
```

### Comparing `cortex_command_mod_converter_engine-1.0.8/conversion_rules/before_pre4/gibs.json` & `cortex_command_mod_converter_engine-1.0.9/conversion_rules/before_pre4/gibs.json`

 * *Files identical despite different names*

### Comparing `cortex_command_mod_converter_engine-1.0.8/conversion_rules/before_pre4/images.json` & `cortex_command_mod_converter_engine-1.0.9/conversion_rules/before_pre4/images.json`

 * *Files identical despite different names*

### Comparing `cortex_command_mod_converter_engine-1.0.8/conversion_rules/before_pre4/lua.json` & `cortex_command_mod_converter_engine-1.0.9/conversion_rules/before_pre4/lua.json`

 * *Files identical despite different names*

### Comparing `cortex_command_mod_converter_engine-1.0.8/conversion_rules/before_pre4/misc.json` & `cortex_command_mod_converter_engine-1.0.9/conversion_rules/before_pre4/misc.json`

 * *Files identical despite different names*

### Comparing `cortex_command_mod_converter_engine-1.0.8/conversion_rules/before_pre4/sounds.json` & `cortex_command_mod_converter_engine-1.0.9/conversion_rules/before_pre4/sounds.json`

 * *Files identical despite different names*

### Comparing `cortex_command_mod_converter_engine-1.0.8/conversion_rules/pre4/images.json` & `cortex_command_mod_converter_engine-1.0.9/conversion_rules/pre4/images.json`

 * *Files identical despite different names*

### Comparing `cortex_command_mod_converter_engine-1.0.8/conversion_rules/pre4/misc.json` & `cortex_command_mod_converter_engine-1.0.9/conversion_rules/pre4/misc.json`

 * *Files identical despite different names*

### Comparing `cortex_command_mod_converter_engine-1.0.8/conversion_rules/pre4/sounds.json` & `cortex_command_mod_converter_engine-1.0.9/conversion_rules/pre4/sounds.json`

 * *Files identical despite different names*

### Comparing `cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/bmp_to_png.py` & `cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/bmp_to_png.py`

 * *Files identical despite different names*

### Comparing `cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/convert.py` & `cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/convert.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import os
 import shutil
+import zipfile
 from pathlib import Path
 
 from cortex_command_mod_converter_engine import (
     bmp_to_png,
     regex_rules,
     stylua,
     utils,
@@ -17,57 +18,69 @@
     ini_writer,
 )
 
 
 def convert(
     input_mod_path,
     output_folder_path,
-    beautify_lua,
-    output_zip,
-    skip_conversion,
+    beautify_lua=True,
+    output_zip=False,
+    skip_conversion=False,
+    remove_input_mod_folder=False,
 ):
+    input_mod_path = Path(input_mod_path)
+    input_folder_path = str(input_mod_path.parent)
 
-    input_mod_name = Path(input_mod_path).name
-    input_folder_path = str(Path(input_mod_path).parent)
-    output_mod_path = Path(output_folder_path) / input_mod_name
+    if zipfile.is_zipfile(input_mod_path):
+        input_mod_name = zips.unzip(input_mod_path, input_folder_path)
+        input_mod_path = input_mod_path.with_name(input_mod_name)
+        # input_mod_path = input_mod_path.with_suffix(".rte")
+    else:
+        input_mod_name = input_mod_path.name
 
-    zips.unzip(input_mod_path, input_folder_path)
+    output_mod_path = Path(output_folder_path) / input_mod_name
 
     # TODO: Maybe give this input_mod_path instead of input_folder_path
     case_check.init_glob(output_folder_path, input_folder_path)
 
     # if cfg.progress_bar:
     #     cfg.progress_bar.segment(2)
     # cfg.progress_bar.setSubtext(f"processing file tree")
 
     conversion_rules = get_conversion_rules()
 
+    print(input_mod_path)
+    print(input_folder_path)
+    print(output_folder_path)
+
     converter_walk(
-        Path(input_mod_path),
+        input_mod_path,
         input_folder_path,
         output_folder_path,
         conversion_rules,
         skip_conversion,
     )
 
     if beautify_lua:
         stylua.stylize(output_mod_path)
 
     # if cfg.progress_bar:
     #     cfg.progress_bar.segment(utils.get_ini_files_in_dir_deep(output_mod_path) * 3)
     #     cfg.progress_bar.setSubtext("building syntax tree")
     ini_cst = ini_cst_builder.get_full_cst(
-        input_folder_path, output_folder_path, Path(input_mod_path)
+        input_folder_path, output_folder_path, input_mod_path
     )
     ini_rules.apply_rules_on_ini_cst(ini_cst, output_folder_path)
     ini_writer.write_converted_ini_cst(ini_cst, output_mod_path)
 
     if output_zip:
         zips.zip(input_mod_name, Path(output_folder_path))
 
+    shutil.rmtree(input_mod_path)
+
 
 def get_conversion_rules():
     conversion_rules = {}
 
     for folder_path, _, subfiles in os.walk("conversion_rules"):
         for filename in subfiles:
             p = folder_path / Path(filename)
```

### Comparing `cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/regex_rules.py` & `cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/regex_rules.py`

 * *Files identical despite different names*

### Comparing `cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/stylua.py` & `cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/stylua.py`

 * *Files identical despite different names*

### Comparing `cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/thumbnail_generator.py` & `cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/thumbnail_generator.py`

 * *Files identical despite different names*

### Comparing `cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/utils.py` & `cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/utils.py`

 * *Files identical despite different names*

### Comparing `cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/zips.py` & `cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/zips.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 import shutil
 import zipfile
 
 import cortex_command_mod_converter_engine.cfg as cfg
 
 
 def unzip(input_mod_path, input_folder_path):
-    if zipfile.is_zipfile(input_mod_path):
-        with zipfile.ZipFile(input_mod_path) as item:
-            item.extractall(input_folder_path)
-        os.remove(input_mod_path)
+    with zipfile.ZipFile(input_mod_path) as item:
+        item.extractall(input_folder_path)
+        extracted_name = item.namelist()[0]
+    os.remove(input_mod_path)
+    return extracted_name[:-1]
 
 
 def zip(input_mod_name, output_folder_path):
     print("Zipping '{}'".format(input_mod_name))
 
     output_mod_zip_name = input_mod_name.replace(
         ".rte", f"-{cfg.SUPPORTED_GAME_VERSION}-v1.0.rte"
```

### Comparing `cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/case_check/case_check.py` & `cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/case_check/case_check.py`

 * *Files identical despite different names*

### Comparing `cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/case_check/case_check_errors.py` & `cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/case_check/case_check_errors.py`

 * *Files identical despite different names*

### Comparing `cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/ini_converting/ini_cst.py` & `cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/ini_converting/ini_cst.py`

 * *Files identical despite different names*

### Comparing `cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/ini_converting/ini_cst_builder.py` & `cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/ini_converting/ini_cst_builder.py`

 * *Files identical despite different names*

### Comparing `cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/ini_converting/ini_rules.py` & `cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/ini_converting/ini_rules.py`

 * *Files 0% similar despite different names*

```diff
@@ -336,17 +336,17 @@
     if not ini_rules_utils.has_children(section):
         return
     if not ini_rules_utils.line_contains_property(section, "AddActor"):
         return
 
     # Pie constants (pulled from source)
     MAX_PIE_QUADRANT_SIZE = 5
-    MAX_PIE_SLICES = MAX_PIE_QUADRANT_SIZE * 4
+    # MAX_PIE_SLICES = MAX_PIE_QUADRANT_SIZE * 4
     DEFAULT_PIES = {
-        # Sizes: number of slices in the preset
+        # Sizes: number of slices in the preset. Each can be increased by mods up to 5.
         # 0 = Up, 1 = Down, 2 = Left, 3 = Right, 4 = Any
         "Actor": {
             "sizes": [1, 0, 0, 0],
             "preset": "Default Actor Pie Menu",
         },
         "AHuman": {
             "sizes": [2, 2, 2, 2],
@@ -377,48 +377,50 @@
 
     # Get all added slices, if we have any.
     slices = ini_rules_utils.get_children_with_property_shallow(section, "AddPieSlice")
     if not slices:
         return
 
     sliceDirCounts = DEFAULT_PIES[s_val]["sizes"]
-    sliceCount = sum(sliceDirCounts)
+    # sliceCount = sum(sliceDirCounts)
 
     # get the direction counts of the slices so we can change if need be.
     dirs = ini_rules_utils.get_values_of_properties_of_children_shallowly(
         [x[1] for x in slices], "Direction"
     )
 
     # TODO: Comment out pie slices when we're above the max pie slice limit.
 
     # Keep track of and update slice directions.
     for x in dirs:
         dir = int(x[0])
         line_tokens = x[1]
+        if dir == 4:
+            continue
         if sliceDirCounts[dir] == MAX_PIE_QUADRANT_SIZE:
             ini_rules_utils.set_line_value(line_tokens, 4)
         else:
             sliceDirCounts[dir] += 1
-        sliceCount += 1
+        # sliceCount += 1
 
     # get the indent of the first slice (we'll need it later)
     indent = ini_rules_utils.get_indent(slices[0][1])
     # Create the parent PieMenu and move everything inside it.
     PT = ini_tokenizer.get_tokens_from_str(("\t" * indent) + "PieMenu = PieMenu\n")
     PieMenu = ini_cst.get_cst(PT, depth=indent)[0]
     CT = ini_tokenizer.get_tokens_from_str(
         ("\t" * (indent + 1)) + f"CopyOf = {DEFAULT_PIES[s_val]['preset']}\n"
     )
     CopyOf = ini_cst.get_cst(CT, depth=indent + 1)[0]
     # indent all the existing slices by one so they can be
     # put in the pie menu appropriately
-    for i, x in slices:
+    for _, x in slices:
         ini_rules_utils.indent(x)
 
-    PieMenu.append({"type": "children", "content": [CopyOf] + [x for i, x in slices]})
+    PieMenu.append({"type": "children", "content": [CopyOf] + [x for _, x in slices]})
 
     # TODO: Don't assume the lines are read in-order.
     # Add the new PieMenu and remove the PieSlices from the section's children
     secChildren = ini_rules_utils.get_children(section)
     secChildren.insert(slices[0][0], PieMenu)
 
     for x in range(len(slices) - 1, -1, -1):
```

### Comparing `cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/ini_converting/ini_rules_utils.py` & `cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/ini_converting/ini_rules_utils.py`

 * *Files identical despite different names*

### Comparing `cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/ini_converting/ini_tokenizer.py` & `cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/ini_converting/ini_tokenizer.py`

 * *Files identical despite different names*

### Comparing `cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/ini_converting/ini_writer.py` & `cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/ini_converting/ini_writer.py`

 * *Files identical despite different names*

### Comparing `cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/stylua_executables/linux/stylua` & `cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/stylua_executables/linux/stylua`

 * *Files identical despite different names*

### Comparing `cortex_command_mod_converter_engine-1.0.8/src/cortex_command_mod_converter_engine/stylua_executables/windows/stylua.exe` & `cortex_command_mod_converter_engine-1.0.9/src/cortex_command_mod_converter_engine/stylua_executables/windows/stylua.exe`

 * *Files identical despite different names*

### Comparing `cortex_command_mod_converter_engine-1.0.8/tests/test_ini_conversion.py` & `cortex_command_mod_converter_engine-1.0.9/tests/test_ini_conversion.py`

 * *Files identical despite different names*

### Comparing `cortex_command_mod_converter_engine-1.0.8/tests/test_ini_cst.py` & `cortex_command_mod_converter_engine-1.0.9/tests/test_ini_cst.py`

 * *Files identical despite different names*

### Comparing `cortex_command_mod_converter_engine-1.0.8/tests/test_ini_tokenizer.py` & `cortex_command_mod_converter_engine-1.0.9/tests/test_ini_tokenizer.py`

 * *Files identical despite different names*

### Comparing `cortex_command_mod_converter_engine-1.0.8/tests/ini_test_files/conversion/remove_sl_terrain_properties/in.ini` & `cortex_command_mod_converter_engine-1.0.9/tests/ini_test_files/conversion/remove_sl_terrain_properties/in.ini`

 * *Files identical despite different names*

### Comparing `cortex_command_mod_converter_engine-1.0.8/LICENSE` & `cortex_command_mod_converter_engine-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cortex_command_mod_converter_engine-1.0.8/README.md` & `cortex_command_mod_converter_engine-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cortex_command_mod_converter_engine-1.0.8/pyproject.toml` & `cortex_command_mod_converter_engine-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cortex-command-mod-converter-engine"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
   { name="MyNameIsTrez", email="welfje@gmail.com" },
 ]
 description = "Automatically converts mods to the latest version of the Cortex Command Community Project."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `cortex_command_mod_converter_engine-1.0.8/PKG-INFO` & `cortex_command_mod_converter_engine-1.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cortex-command-mod-converter-engine
-Version: 1.0.8
+Version: 1.0.9
 Summary: Automatically converts mods to the latest version of the Cortex Command Community Project.
 Project-URL: Homepage, https://github.com/MyNameIsTrez/Cortex-Command-Mod-Converter-Engine
 Project-URL: Bug Tracker, https://github.com/MyNameIsTrez/Cortex-Command-Mod-Converter-Engine/issues
 Author-email: MyNameIsTrez <welfje@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

