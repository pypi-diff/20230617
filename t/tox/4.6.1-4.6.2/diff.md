# Comparing `tmp/tox-4.6.1.tar.gz` & `tmp/tox-4.6.2.tar.gz`

## Comparing `tox-4.6.1.tar` & `tox-4.6.2.tar`

### file list

```diff
@@ -1,221 +1,221 @@
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 tox-4.6.1/tox.ini
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/__init__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/__main__.py
--rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/provision.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/py.typed
--rw-r--r--   0        0        0    19660 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/pytest.py
--rw-r--r--   0        0        0     8283 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/report.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/run.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/__init__.py
--rw-r--r--   0        0        0     6570 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/main.py
--rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/of_type.py
--rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/set_env.py
--rw-r--r--   0        0        0     9990 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/sets.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/cli/__init__.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/cli/env_var.py
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/cli/ini.py
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/cli/parse.py
--rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/cli/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/loader/__init__.py
--rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/loader/api.py
--rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/loader/convert.py
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/loader/memory.py
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/loader/section.py
--rw-r--r--   0        0        0     4835 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/loader/str_convert.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/loader/stringify.py
--rw-r--r--   0        0        0     3966 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/loader/ini/__init__.py
--rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/loader/ini/factor.py
--rw-r--r--   0        0        0    13404 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/loader/ini/replace.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/source/__init__.py
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/source/api.py
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/source/discover.py
--rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/source/ini.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/source/ini_section.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/source/legacy_toml.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/source/setup_cfg.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/source/tox_ini.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/execute/__init__.py
--rw-r--r--   0        0        0     9267 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/execute/api.py
--rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/execute/pep517_backend.py
--rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/execute/request.py
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/execute/stream.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/execute/util.py
--rw-r--r--   0        0        0    14099 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/execute/local_sub_process/__init__.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/execute/local_sub_process/read_via_thread.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/execute/local_sub_process/read_via_thread_unix.py
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/execute/local_sub_process/read_via_thread_windows.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/journal/__init__.py
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/journal/env.py
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/journal/main.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/plugin/__init__.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/plugin/inline.py
--rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/plugin/manager.py
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/plugin/spec.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/session/__init__.py
--rw-r--r--   0        0        0    18474 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/session/env_select.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/session/state.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/session/cmd/__init__.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/session/cmd/depends.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/session/cmd/devenv.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/session/cmd/exec_.py
--rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/session/cmd/legacy.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/session/cmd/list_env.py
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/session/cmd/quickstart.py
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/session/cmd/show_config.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/session/cmd/version_flag.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/session/cmd/run/__init__.py
--rw-r--r--   0        0        0    17515 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/session/cmd/run/common.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/session/cmd/run/parallel.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/session/cmd/run/sequential.py
--rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/session/cmd/run/single.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/__init__.py
--rw-r--r--   0        0        0    20287 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/api.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/errors.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/info.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/installer.py
--rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/package.py
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/register.py
--rw-r--r--   0        0        0     7824 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/runner.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/__init__.py
--rw-r--r--   0        0        0    10989 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/api.py
--rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/package.py
--rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/pip/__init__.py
--rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/pip/pip_install.py
--rw-r--r--   0        0        0     5602 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/pip/req_file.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/pip/req/__init__.py
--rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/pip/req/args.py
--rw-r--r--   0        0        0    19762 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/pip/req/file.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/pip/req/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/virtual_env/__init__.py
--rw-r--r--   0        0        0     6453 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/virtual_env/api.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/virtual_env/runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/virtual_env/package/__init__.py
--rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/virtual_env/package/cmd_builder.py
--rw-r--r--   0        0        0    17983 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/virtual_env/package/pyproject.py
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/virtual_env/package/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/util/__init__.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/util/ci.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/util/cpu.py
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/util/file_view.py
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/util/graph.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/util/path.py
--rw-r--r--   0        0        0     6767 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/util/spinner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/__init__.py
--rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 tox-4.6.1/tests/conftest.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 tox-4.6.1/tests/test_call_modes.py
--rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 tox-4.6.1/tests/test_provision.py
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 tox-4.6.1/tests/test_report.py
--rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 tox-4.6.1/tests/test_run.py
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 tox-4.6.1/tests/test_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/__init__.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/conftest.py
--rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/test_main.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/test_of_types.py
--rw-r--r--   0        0        0     5828 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/test_set_env.py
--rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/test_sets.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/test_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/cli/__init__.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/cli/conftest.py
--rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/cli/test_cli_env_var.py
--rw-r--r--   0        0        0     7422 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/cli/test_cli_ini.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/cli/test_parse.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/cli/test_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/__init__.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/test_loader.py
--rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/test_memory_loader.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/test_section.py
--rw-r--r--   0        0        0     6988 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/test_str_convert.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/ini/__init__.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/ini/conftest.py
--rw-r--r--   0        0        0     6501 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/ini/test_factor.py
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/ini/test_ini_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/ini/replace/__init__.py
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/ini/replace/conftest.py
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/ini/replace/test_replace.py
--rw-r--r--   0        0        0     7230 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/ini/replace/test_replace_env_var.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/ini/replace/test_replace_os_pathsep.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/ini/replace/test_replace_os_sep.py
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/ini/replace/test_replace_posargs.py
--rw-r--r--   0        0        0     8310 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/ini/replace/test_replace_tox_env.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/ini/replace/test_replace_tty.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/source/__init__.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/source/test_discover.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/source/test_legacy_toml.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/source/test_setup_cfg.py
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/source/test_source_ini.py
--rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 tox-4.6.1/tests/demo_pkg_inline/build.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 tox-4.6.1/tests/demo_pkg_inline/pyproject.toml
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 tox-4.6.1/tests/demo_pkg_setuptools/pyproject.toml
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tox-4.6.1/tests/demo_pkg_setuptools/setup.cfg
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 tox-4.6.1/tests/demo_pkg_setuptools/demo_pkg_setuptools/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/execute/__init__.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 tox-4.6.1/tests/execute/conftest.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 tox-4.6.1/tests/execute/test_request.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 tox-4.6.1/tests/execute/test_stream.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/execute/local_subprocess/__init__.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 tox-4.6.1/tests/execute/local_subprocess/bad_process.py
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 tox-4.6.1/tests/execute/local_subprocess/local_subprocess_sigint.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 tox-4.6.1/tests/execute/local_subprocess/test_execute_util.py
--rw-r--r--   0        0        0    14176 2020-02-02 00:00:00.000000 tox-4.6.1/tests/execute/local_subprocess/test_local_subprocess.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 tox-4.6.1/tests/execute/local_subprocess/tty_check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/journal/__init__.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 tox-4.6.1/tests/journal/test_main_journal.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 tox-4.6.1/tests/plugin/conftest.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 tox-4.6.1/tests/plugin/test_inline.py
--rw-r--r--   0        0        0     9176 2020-02-02 00:00:00.000000 tox-4.6.1/tests/plugin/test_plugin.py
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 tox-4.6.1/tests/plugin/test_plugin_custom_config_set.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/pytest_/__init__.py
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 tox-4.6.1/tests/pytest_/test_init.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/session/__init__.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 tox-4.6.1/tests/session/test_env_select.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 tox-4.6.1/tests/session/test_session_common.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/session/cmd/__init__.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 tox-4.6.1/tests/session/cmd/test_depends.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 tox-4.6.1/tests/session/cmd/test_devenv.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 tox-4.6.1/tests/session/cmd/test_exec_.py
--rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 tox-4.6.1/tests/session/cmd/test_legacy.py
--rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 tox-4.6.1/tests/session/cmd/test_list_envs.py
--rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 tox-4.6.1/tests/session/cmd/test_parallel.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 tox-4.6.1/tests/session/cmd/test_quickstart.py
--rw-r--r--   0        0        0    18755 2020-02-02 00:00:00.000000 tox-4.6.1/tests/session/cmd/test_sequential.py
--rw-r--r--   0        0        0    11254 2020-02-02 00:00:00.000000 tox-4.6.1/tests/session/cmd/test_show_config.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 tox-4.6.1/tests/session/cmd/test_state.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/session/cmd/run/__init__.py
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 tox-4.6.1/tests/session/cmd/run/test_common.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/__init__.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/test_api.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/test_info.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/test_register.py
--rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/test_tox_env_api.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/test_tox_env_runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/python/__init__.py
--rw-r--r--   0        0        0     9327 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/python/test_python_api.py
--rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/python/test_python_runner.py
--rw-r--r--   0        0        0    17085 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/python/pip/test_pip_install.py
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/python/pip/test_req_file.py
--rw-r--r--   0        0        0    22171 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/python/pip/req/test_file.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/python/test-pkg/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/python/virtual_env/__init__.py
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/python/virtual_env/test_setuptools.py
--rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/python/virtual_env/test_virtualenv_api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/python/virtual_env/package/__init__.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/python/virtual_env/package/conftest.py
--rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py
--rw-r--r--   0        0        0    10178 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/python/virtual_env/package/test_package_pyproject.py
--rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/python/virtual_env/package/test_python_package_util.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 tox-4.6.1/tests/type_check/add_config_container_factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/util/__init__.py
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 tox-4.6.1/tests/util/test_ci.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 tox-4.6.1/tests/util/test_cpu.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 tox-4.6.1/tests/util/test_graph.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 tox-4.6.1/tests/util/test_path.py
--rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 tox-4.6.1/tests/util/test_spinner.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 tox-4.6.1/.gitignore
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 tox-4.6.1/LICENSE
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 tox-4.6.1/README.md
--rw-r--r--   0        0        0     5324 2020-02-02 00:00:00.000000 tox-4.6.1/pyproject.toml
--rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 tox-4.6.1/PKG-INFO
+-rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 tox-4.6.2/tox.ini
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/__init__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/__main__.py
+-rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/provision.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/py.typed
+-rw-r--r--   0        0        0    19660 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/pytest.py
+-rw-r--r--   0        0        0     8283 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/report.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/run.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/__init__.py
+-rw-r--r--   0        0        0     6570 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/main.py
+-rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/of_type.py
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/set_env.py
+-rw-r--r--   0        0        0     9990 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/sets.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/cli/__init__.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/cli/env_var.py
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/cli/ini.py
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/cli/parse.py
+-rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/cli/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/loader/__init__.py
+-rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/loader/api.py
+-rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/loader/convert.py
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/loader/memory.py
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/loader/section.py
+-rw-r--r--   0        0        0     4835 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/loader/str_convert.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/loader/stringify.py
+-rw-r--r--   0        0        0     3966 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/loader/ini/__init__.py
+-rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/loader/ini/factor.py
+-rw-r--r--   0        0        0    13404 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/loader/ini/replace.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/source/__init__.py
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/source/api.py
+-rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/source/discover.py
+-rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/source/ini.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/source/ini_section.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/source/legacy_toml.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/source/setup_cfg.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/source/tox_ini.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/execute/__init__.py
+-rw-r--r--   0        0        0     9267 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/execute/api.py
+-rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/execute/pep517_backend.py
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/execute/request.py
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/execute/stream.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/execute/util.py
+-rw-r--r--   0        0        0    14099 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/execute/local_sub_process/__init__.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/execute/local_sub_process/read_via_thread.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/execute/local_sub_process/read_via_thread_unix.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/execute/local_sub_process/read_via_thread_windows.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/journal/__init__.py
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/journal/env.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/journal/main.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/plugin/__init__.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/plugin/inline.py
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/plugin/manager.py
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/plugin/spec.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/session/__init__.py
+-rw-r--r--   0        0        0    18474 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/session/env_select.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/session/state.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/session/cmd/__init__.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/session/cmd/depends.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/session/cmd/devenv.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/session/cmd/exec_.py
+-rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/session/cmd/legacy.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/session/cmd/list_env.py
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/session/cmd/quickstart.py
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/session/cmd/show_config.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/session/cmd/version_flag.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/session/cmd/run/__init__.py
+-rw-r--r--   0        0        0    17515 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/session/cmd/run/common.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/session/cmd/run/parallel.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/session/cmd/run/sequential.py
+-rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/session/cmd/run/single.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/__init__.py
+-rw-r--r--   0        0        0    20287 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/api.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/errors.py
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/info.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/installer.py
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/package.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/register.py
+-rw-r--r--   0        0        0     7824 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/runner.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/__init__.py
+-rw-r--r--   0        0        0    10989 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/api.py
+-rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/package.py
+-rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/pip/__init__.py
+-rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/pip/pip_install.py
+-rw-r--r--   0        0        0     5602 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/pip/req_file.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/pip/req/__init__.py
+-rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/pip/req/args.py
+-rw-r--r--   0        0        0    19762 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/pip/req/file.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/pip/req/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/virtual_env/__init__.py
+-rw-r--r--   0        0        0     6453 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/virtual_env/api.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/virtual_env/runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/virtual_env/package/__init__.py
+-rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/virtual_env/package/cmd_builder.py
+-rw-r--r--   0        0        0    17905 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/virtual_env/package/pyproject.py
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/virtual_env/package/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/util/__init__.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/util/ci.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/util/cpu.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/util/file_view.py
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/util/graph.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/util/path.py
+-rw-r--r--   0        0        0     6767 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/util/spinner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/__init__.py
+-rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 tox-4.6.2/tests/conftest.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 tox-4.6.2/tests/test_call_modes.py
+-rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 tox-4.6.2/tests/test_provision.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 tox-4.6.2/tests/test_report.py
+-rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 tox-4.6.2/tests/test_run.py
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 tox-4.6.2/tests/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/__init__.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/conftest.py
+-rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/test_main.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/test_of_types.py
+-rw-r--r--   0        0        0     5828 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/test_set_env.py
+-rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/test_sets.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/test_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/cli/__init__.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/cli/conftest.py
+-rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/cli/test_cli_env_var.py
+-rw-r--r--   0        0        0     7422 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/cli/test_cli_ini.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/cli/test_parse.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/cli/test_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/__init__.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/test_loader.py
+-rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/test_memory_loader.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/test_section.py
+-rw-r--r--   0        0        0     6988 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/test_str_convert.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/ini/__init__.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/ini/conftest.py
+-rw-r--r--   0        0        0     6501 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/ini/test_factor.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/ini/test_ini_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/ini/replace/__init__.py
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/ini/replace/conftest.py
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/ini/replace/test_replace.py
+-rw-r--r--   0        0        0     7230 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/ini/replace/test_replace_env_var.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/ini/replace/test_replace_os_pathsep.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/ini/replace/test_replace_os_sep.py
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/ini/replace/test_replace_posargs.py
+-rw-r--r--   0        0        0     8310 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/ini/replace/test_replace_tox_env.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/ini/replace/test_replace_tty.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/source/__init__.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/source/test_discover.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/source/test_legacy_toml.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/source/test_setup_cfg.py
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/source/test_source_ini.py
+-rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 tox-4.6.2/tests/demo_pkg_inline/build.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 tox-4.6.2/tests/demo_pkg_inline/pyproject.toml
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 tox-4.6.2/tests/demo_pkg_setuptools/pyproject.toml
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tox-4.6.2/tests/demo_pkg_setuptools/setup.cfg
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 tox-4.6.2/tests/demo_pkg_setuptools/demo_pkg_setuptools/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/execute/__init__.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 tox-4.6.2/tests/execute/conftest.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 tox-4.6.2/tests/execute/test_request.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 tox-4.6.2/tests/execute/test_stream.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/execute/local_subprocess/__init__.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 tox-4.6.2/tests/execute/local_subprocess/bad_process.py
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 tox-4.6.2/tests/execute/local_subprocess/local_subprocess_sigint.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 tox-4.6.2/tests/execute/local_subprocess/test_execute_util.py
+-rw-r--r--   0        0        0    14176 2020-02-02 00:00:00.000000 tox-4.6.2/tests/execute/local_subprocess/test_local_subprocess.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 tox-4.6.2/tests/execute/local_subprocess/tty_check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/journal/__init__.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 tox-4.6.2/tests/journal/test_main_journal.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 tox-4.6.2/tests/plugin/conftest.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 tox-4.6.2/tests/plugin/test_inline.py
+-rw-r--r--   0        0        0     9176 2020-02-02 00:00:00.000000 tox-4.6.2/tests/plugin/test_plugin.py
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 tox-4.6.2/tests/plugin/test_plugin_custom_config_set.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/pytest_/__init__.py
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 tox-4.6.2/tests/pytest_/test_init.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/session/__init__.py
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 tox-4.6.2/tests/session/test_env_select.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 tox-4.6.2/tests/session/test_session_common.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/session/cmd/__init__.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 tox-4.6.2/tests/session/cmd/test_depends.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 tox-4.6.2/tests/session/cmd/test_devenv.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 tox-4.6.2/tests/session/cmd/test_exec_.py
+-rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 tox-4.6.2/tests/session/cmd/test_legacy.py
+-rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 tox-4.6.2/tests/session/cmd/test_list_envs.py
+-rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 tox-4.6.2/tests/session/cmd/test_parallel.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 tox-4.6.2/tests/session/cmd/test_quickstart.py
+-rw-r--r--   0        0        0    18755 2020-02-02 00:00:00.000000 tox-4.6.2/tests/session/cmd/test_sequential.py
+-rw-r--r--   0        0        0    11254 2020-02-02 00:00:00.000000 tox-4.6.2/tests/session/cmd/test_show_config.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 tox-4.6.2/tests/session/cmd/test_state.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/session/cmd/run/__init__.py
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 tox-4.6.2/tests/session/cmd/run/test_common.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/__init__.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/test_api.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/test_info.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/test_register.py
+-rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/test_tox_env_api.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/test_tox_env_runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/python/__init__.py
+-rw-r--r--   0        0        0     9327 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/python/test_python_api.py
+-rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/python/test_python_runner.py
+-rw-r--r--   0        0        0    17085 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/python/pip/test_pip_install.py
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/python/pip/test_req_file.py
+-rw-r--r--   0        0        0    22171 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/python/pip/req/test_file.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/python/test-pkg/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/python/virtual_env/__init__.py
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/python/virtual_env/test_setuptools.py
+-rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/python/virtual_env/test_virtualenv_api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/python/virtual_env/package/__init__.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/python/virtual_env/package/conftest.py
+-rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py
+-rw-r--r--   0        0        0    11235 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/python/virtual_env/package/test_package_pyproject.py
+-rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/python/virtual_env/package/test_python_package_util.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 tox-4.6.2/tests/type_check/add_config_container_factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/util/__init__.py
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 tox-4.6.2/tests/util/test_ci.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 tox-4.6.2/tests/util/test_cpu.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 tox-4.6.2/tests/util/test_graph.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 tox-4.6.2/tests/util/test_path.py
+-rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 tox-4.6.2/tests/util/test_spinner.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 tox-4.6.2/.gitignore
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 tox-4.6.2/LICENSE
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 tox-4.6.2/README.md
+-rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 tox-4.6.2/pyproject.toml
+-rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 tox-4.6.2/PKG-INFO
```

### Comparing `tox-4.6.1/tox.ini` & `tox-4.6.2/tox.ini`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/provision.py` & `tox-4.6.2/src/tox/provision.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/pytest.py` & `tox-4.6.2/src/tox/pytest.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/report.py` & `tox-4.6.2/src/tox/report.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/run.py` & `tox-4.6.2/src/tox/run.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/config/main.py` & `tox-4.6.2/src/tox/config/main.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/config/of_type.py` & `tox-4.6.2/src/tox/config/of_type.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/config/set_env.py` & `tox-4.6.2/src/tox/config/set_env.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/config/sets.py` & `tox-4.6.2/src/tox/config/sets.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/config/types.py` & `tox-4.6.2/src/tox/config/types.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/config/cli/env_var.py` & `tox-4.6.2/src/tox/config/cli/env_var.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/config/cli/ini.py` & `tox-4.6.2/src/tox/config/cli/ini.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/config/cli/parse.py` & `tox-4.6.2/src/tox/config/cli/parse.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/config/cli/parser.py` & `tox-4.6.2/src/tox/config/cli/parser.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/config/loader/api.py` & `tox-4.6.2/src/tox/config/loader/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/config/loader/convert.py` & `tox-4.6.2/src/tox/config/loader/convert.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/config/loader/memory.py` & `tox-4.6.2/src/tox/config/loader/memory.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/config/loader/section.py` & `tox-4.6.2/src/tox/config/loader/section.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/config/loader/str_convert.py` & `tox-4.6.2/src/tox/config/loader/str_convert.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/config/loader/stringify.py` & `tox-4.6.2/src/tox/config/loader/stringify.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/config/loader/ini/__init__.py` & `tox-4.6.2/src/tox/config/loader/ini/__init__.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/config/loader/ini/factor.py` & `tox-4.6.2/src/tox/config/loader/ini/factor.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/config/loader/ini/replace.py` & `tox-4.6.2/src/tox/config/loader/ini/replace.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/config/source/api.py` & `tox-4.6.2/src/tox/config/source/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/config/source/discover.py` & `tox-4.6.2/src/tox/config/source/discover.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/config/source/ini.py` & `tox-4.6.2/src/tox/config/source/ini.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/config/source/ini_section.py` & `tox-4.6.2/src/tox/config/source/ini_section.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/config/source/legacy_toml.py` & `tox-4.6.2/src/tox/config/source/legacy_toml.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/config/source/setup_cfg.py` & `tox-4.6.2/src/tox/config/source/setup_cfg.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/execute/api.py` & `tox-4.6.2/src/tox/execute/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/execute/pep517_backend.py` & `tox-4.6.2/src/tox/execute/pep517_backend.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/execute/request.py` & `tox-4.6.2/src/tox/execute/request.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/execute/stream.py` & `tox-4.6.2/src/tox/execute/stream.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/execute/util.py` & `tox-4.6.2/src/tox/execute/util.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/execute/local_sub_process/__init__.py` & `tox-4.6.2/src/tox/execute/local_sub_process/__init__.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/execute/local_sub_process/read_via_thread.py` & `tox-4.6.2/src/tox/execute/local_sub_process/read_via_thread.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/execute/local_sub_process/read_via_thread_unix.py` & `tox-4.6.2/src/tox/execute/local_sub_process/read_via_thread_unix.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/execute/local_sub_process/read_via_thread_windows.py` & `tox-4.6.2/src/tox/execute/local_sub_process/read_via_thread_windows.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/journal/env.py` & `tox-4.6.2/src/tox/journal/env.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/journal/main.py` & `tox-4.6.2/src/tox/journal/main.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/plugin/__init__.py` & `tox-4.6.2/src/tox/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/plugin/inline.py` & `tox-4.6.2/src/tox/plugin/inline.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/plugin/manager.py` & `tox-4.6.2/src/tox/plugin/manager.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/plugin/spec.py` & `tox-4.6.2/src/tox/plugin/spec.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/session/env_select.py` & `tox-4.6.2/src/tox/session/env_select.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/session/state.py` & `tox-4.6.2/src/tox/session/state.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/session/cmd/depends.py` & `tox-4.6.2/src/tox/session/cmd/depends.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/session/cmd/devenv.py` & `tox-4.6.2/src/tox/session/cmd/devenv.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/session/cmd/exec_.py` & `tox-4.6.2/src/tox/session/cmd/exec_.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/session/cmd/legacy.py` & `tox-4.6.2/src/tox/session/cmd/legacy.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/session/cmd/list_env.py` & `tox-4.6.2/src/tox/session/cmd/list_env.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/session/cmd/quickstart.py` & `tox-4.6.2/src/tox/session/cmd/quickstart.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/session/cmd/show_config.py` & `tox-4.6.2/src/tox/session/cmd/show_config.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/session/cmd/version_flag.py` & `tox-4.6.2/src/tox/session/cmd/version_flag.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/session/cmd/run/common.py` & `tox-4.6.2/src/tox/session/cmd/run/common.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/session/cmd/run/parallel.py` & `tox-4.6.2/src/tox/session/cmd/run/parallel.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/session/cmd/run/sequential.py` & `tox-4.6.2/src/tox/session/cmd/run/sequential.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/session/cmd/run/single.py` & `tox-4.6.2/src/tox/session/cmd/run/single.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/tox_env/api.py` & `tox-4.6.2/src/tox/tox_env/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/tox_env/info.py` & `tox-4.6.2/src/tox/tox_env/info.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/tox_env/installer.py` & `tox-4.6.2/src/tox/tox_env/installer.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/tox_env/package.py` & `tox-4.6.2/src/tox/tox_env/package.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/tox_env/register.py` & `tox-4.6.2/src/tox/tox_env/register.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/tox_env/runner.py` & `tox-4.6.2/src/tox/tox_env/runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/tox_env/util.py` & `tox-4.6.2/src/tox/tox_env/util.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/tox_env/python/api.py` & `tox-4.6.2/src/tox/tox_env/python/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/tox_env/python/package.py` & `tox-4.6.2/src/tox/tox_env/python/package.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/tox_env/python/runner.py` & `tox-4.6.2/src/tox/tox_env/python/runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/tox_env/python/pip/pip_install.py` & `tox-4.6.2/src/tox/tox_env/python/pip/pip_install.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/tox_env/python/pip/req_file.py` & `tox-4.6.2/src/tox/tox_env/python/pip/req_file.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/tox_env/python/pip/req/args.py` & `tox-4.6.2/src/tox/tox_env/python/pip/req/args.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/tox_env/python/pip/req/file.py` & `tox-4.6.2/src/tox/tox_env/python/pip/req/file.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/tox_env/python/pip/req/util.py` & `tox-4.6.2/src/tox/tox_env/python/pip/req/util.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/tox_env/python/virtual_env/api.py` & `tox-4.6.2/src/tox/tox_env/python/virtual_env/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/tox_env/python/virtual_env/runner.py` & `tox-4.6.2/src/tox/tox_env/python/virtual_env/runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/tox_env/python/virtual_env/package/cmd_builder.py` & `tox-4.6.2/src/tox/tox_env/python/virtual_env/package/cmd_builder.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/tox_env/python/virtual_env/package/pyproject.py` & `tox-4.6.2/src/tox/tox_env/python/virtual_env/package/pyproject.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,21 +327,21 @@
 
 class Pep517VirtualEnvFrontend(Frontend):
     def __init__(self, root: Path, env: Pep517VirtualEnvPackager) -> None:
         super().__init__(*Frontend.create_args_from_folder(root))
         self._tox_env = env
         self._backend_executor_: LocalSubProcessPep517Executor | None = None
         into: dict[str, Any] = {}
-        pkg_cache = cached(
-            into,
-            key=lambda *args, **kwargs: "wheel" if "wheel_directory" in kwargs else "sdist",  # noqa: ARG005
-        )
-        self.build_wheel = pkg_cache(self.build_wheel)  # type: ignore[method-assign]
-        self.build_sdist = pkg_cache(self.build_sdist)  # type: ignore[method-assign]
-        self.build_editable = pkg_cache(self.build_editable)  # type: ignore[method-assign]
+
+        for build_type in ("editable", "sdist", "wheel"):  # wrap build methods in a cache wrapper
+
+            def key(*args: Any, bound_return: str = build_type, **kwargs: Any) -> str:  # noqa: ARG001
+                return bound_return
+
+            setattr(self, f"build_{build_type}", cached(into, key=key)(getattr(self, f"build_{build_type}")))
 
     @property
     def backend_cmd(self) -> Sequence[str]:
         return ["python", *self.backend_args]
 
     def _send(self, cmd: str, **kwargs: Any) -> tuple[Any, str, str]:
         try:
```

### Comparing `tox-4.6.1/src/tox/tox_env/python/virtual_env/package/util.py` & `tox-4.6.2/src/tox/tox_env/python/virtual_env/package/util.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/util/ci.py` & `tox-4.6.2/src/tox/util/ci.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/util/file_view.py` & `tox-4.6.2/src/tox/util/file_view.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/util/graph.py` & `tox-4.6.2/src/tox/util/graph.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/util/path.py` & `tox-4.6.2/src/tox/util/path.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/src/tox/util/spinner.py` & `tox-4.6.2/src/tox/util/spinner.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/conftest.py` & `tox-4.6.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/test_provision.py` & `tox-4.6.2/tests/test_provision.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/test_report.py` & `tox-4.6.2/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/test_run.py` & `tox-4.6.2/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/test_version.py` & `tox-4.6.2/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/config/test_main.py` & `tox-4.6.2/tests/config/test_main.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/config/test_of_types.py` & `tox-4.6.2/tests/config/test_of_types.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/config/test_set_env.py` & `tox-4.6.2/tests/config/test_set_env.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/config/test_sets.py` & `tox-4.6.2/tests/config/test_sets.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/config/test_types.py` & `tox-4.6.2/tests/config/test_types.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/config/cli/conftest.py` & `tox-4.6.2/tests/config/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/config/cli/test_cli_env_var.py` & `tox-4.6.2/tests/config/cli/test_cli_env_var.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/config/cli/test_cli_ini.py` & `tox-4.6.2/tests/config/cli/test_cli_ini.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/config/cli/test_parse.py` & `tox-4.6.2/tests/config/cli/test_parse.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/config/cli/test_parser.py` & `tox-4.6.2/tests/config/cli/test_parser.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/config/loader/test_loader.py` & `tox-4.6.2/tests/config/loader/test_loader.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/config/loader/test_memory_loader.py` & `tox-4.6.2/tests/config/loader/test_memory_loader.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/config/loader/test_section.py` & `tox-4.6.2/tests/config/loader/test_section.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/config/loader/test_str_convert.py` & `tox-4.6.2/tests/config/loader/test_str_convert.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/config/loader/ini/conftest.py` & `tox-4.6.2/tests/config/loader/ini/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/config/loader/ini/test_factor.py` & `tox-4.6.2/tests/config/loader/ini/test_factor.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/config/loader/ini/test_ini_loader.py` & `tox-4.6.2/tests/config/loader/ini/test_ini_loader.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/config/loader/ini/replace/conftest.py` & `tox-4.6.2/tests/config/loader/ini/replace/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/config/loader/ini/replace/test_replace.py` & `tox-4.6.2/tests/config/loader/ini/replace/test_replace.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/config/loader/ini/replace/test_replace_env_var.py` & `tox-4.6.2/tests/config/loader/ini/replace/test_replace_env_var.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/config/loader/ini/replace/test_replace_os_sep.py` & `tox-4.6.2/tests/config/loader/ini/replace/test_replace_os_sep.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/config/loader/ini/replace/test_replace_posargs.py` & `tox-4.6.2/tests/config/loader/ini/replace/test_replace_posargs.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/config/loader/ini/replace/test_replace_tox_env.py` & `tox-4.6.2/tests/config/loader/ini/replace/test_replace_tox_env.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/config/loader/ini/replace/test_replace_tty.py` & `tox-4.6.2/tests/config/loader/ini/replace/test_replace_tty.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/config/source/test_discover.py` & `tox-4.6.2/tests/config/source/test_discover.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/config/source/test_setup_cfg.py` & `tox-4.6.2/tests/config/source/test_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/config/source/test_source_ini.py` & `tox-4.6.2/tests/config/source/test_source_ini.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/demo_pkg_inline/build.py` & `tox-4.6.2/tests/demo_pkg_inline/build.py`

 * *Files 6% similar despite different names*

```diff
@@ -113,14 +113,24 @@
     return base_name
 
 
 def get_requires_for_build_wheel(config_settings: dict[str, str] | None = None) -> list[str]:  # noqa: ARG001
     return []  # pragma: no cover # only executed in non-host pythons
 
 
+if os.environ.get("BACKEND_HAS_EDITABLE"):
+
+    def build_editable(
+        wheel_directory: str,
+        config_settings: dict[str, str] | None = None,
+        metadata_directory: str | None = None,
+    ) -> str:
+        return build_wheel(wheel_directory, config_settings, metadata_directory)
+
+
 def build_sdist(sdist_directory: str, config_settings: dict[str, str] | None = None) -> str:  # noqa: ARG001
     result = f"{name}-{version}.tar.gz"  # pragma: win32 cover
     with tarfile.open(str(Path(sdist_directory) / result), "w:gz") as tar:  # pragma: win32 cover
         root = Path(__file__).parent  # pragma: win32 cover
         tar.add(str(root / "build.py"), "build.py")  # pragma: win32 cover
         tar.add(str(root / "pyproject.toml"), "pyproject.toml")  # pragma: win32 cover
     return result  # pragma: win32 cover
```

### Comparing `tox-4.6.1/tests/execute/test_request.py` & `tox-4.6.2/tests/execute/test_request.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/execute/local_subprocess/bad_process.py` & `tox-4.6.2/tests/execute/local_subprocess/bad_process.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/execute/local_subprocess/local_subprocess_sigint.py` & `tox-4.6.2/tests/execute/local_subprocess/local_subprocess_sigint.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/execute/local_subprocess/test_execute_util.py` & `tox-4.6.2/tests/execute/local_subprocess/test_execute_util.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/execute/local_subprocess/test_local_subprocess.py` & `tox-4.6.2/tests/execute/local_subprocess/test_local_subprocess.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/journal/test_main_journal.py` & `tox-4.6.2/tests/journal/test_main_journal.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/plugin/test_inline.py` & `tox-4.6.2/tests/plugin/test_inline.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/plugin/test_plugin.py` & `tox-4.6.2/tests/plugin/test_plugin.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/plugin/test_plugin_custom_config_set.py` & `tox-4.6.2/tests/plugin/test_plugin_custom_config_set.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/pytest_/test_init.py` & `tox-4.6.2/tests/pytest_/test_init.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/session/test_env_select.py` & `tox-4.6.2/tests/session/test_env_select.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/session/test_session_common.py` & `tox-4.6.2/tests/session/test_session_common.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/session/cmd/test_depends.py` & `tox-4.6.2/tests/session/cmd/test_depends.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/session/cmd/test_devenv.py` & `tox-4.6.2/tests/session/cmd/test_devenv.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/session/cmd/test_exec_.py` & `tox-4.6.2/tests/session/cmd/test_exec_.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/session/cmd/test_legacy.py` & `tox-4.6.2/tests/session/cmd/test_legacy.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/session/cmd/test_list_envs.py` & `tox-4.6.2/tests/session/cmd/test_list_envs.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/session/cmd/test_parallel.py` & `tox-4.6.2/tests/session/cmd/test_parallel.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/session/cmd/test_quickstart.py` & `tox-4.6.2/tests/session/cmd/test_quickstart.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/session/cmd/test_sequential.py` & `tox-4.6.2/tests/session/cmd/test_sequential.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/session/cmd/test_show_config.py` & `tox-4.6.2/tests/session/cmd/test_show_config.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/session/cmd/test_state.py` & `tox-4.6.2/tests/session/cmd/test_state.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/session/cmd/run/test_common.py` & `tox-4.6.2/tests/session/cmd/run/test_common.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/tox_env/test_api.py` & `tox-4.6.2/tests/tox_env/test_api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/tox_env/test_register.py` & `tox-4.6.2/tests/tox_env/test_register.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/tox_env/test_tox_env_api.py` & `tox-4.6.2/tests/tox_env/test_tox_env_api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/tox_env/test_tox_env_runner.py` & `tox-4.6.2/tests/tox_env/test_tox_env_runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/tox_env/python/test_python_api.py` & `tox-4.6.2/tests/tox_env/python/test_python_api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/tox_env/python/test_python_runner.py` & `tox-4.6.2/tests/tox_env/python/test_python_runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/tox_env/python/pip/test_pip_install.py` & `tox-4.6.2/tests/tox_env/python/pip/test_pip_install.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/tox_env/python/pip/test_req_file.py` & `tox-4.6.2/tests/tox_env/python/pip/test_req_file.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/tox_env/python/pip/req/test_file.py` & `tox-4.6.2/tests/tox_env/python/pip/req/test_file.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/tox_env/python/virtual_env/test_setuptools.py` & `tox-4.6.2/tests/tox_env/python/virtual_env/test_setuptools.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/tox_env/python/virtual_env/test_virtualenv_api.py` & `tox-4.6.2/tests/tox_env/python/virtual_env/test_virtualenv_api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/tox_env/python/virtual_env/package/conftest.py` & `tox-4.6.2/tests/tox_env/python/virtual_env/package/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py` & `tox-4.6.2/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/tox_env/python/virtual_env/package/test_package_pyproject.py` & `tox-4.6.2/tests/tox_env/python/virtual_env/package/test_package_pyproject.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,7 +259,38 @@
     result.assert_success()
     found_calls = [(i[0][0].conf.name, i[0][3].run_id) for i in execute_calls.call_args_list]
     if package == "skip":
         assert (".pkg", "install_deps") not in found_calls
     else:
         assert found_calls[0] == (".pkg", "install_requires")
         assert found_calls[1] == (".pkg", "install_deps")
+
+
+def test_pyproject_build_editable_and_wheel(tox_project: ToxProjectCreator, demo_pkg_inline: Path) -> None:
+    # test that build wheel and build editable are cached separately
+
+    ini = """
+    [testenv:.pkg]
+    set_env= BACKEND_HAS_EDITABLE=1
+    [testenv:a,b]
+    package = editable
+    [testenv:c,d]
+    package = wheel
+    """
+    proj = tox_project({"tox.ini": ini}, base=demo_pkg_inline)
+    execute_calls = proj.patch_execute(lambda r: 0 if "install" in r.run_id else None)
+
+    result = proj.run("r", "-e", "a,b,c,d", "--notest", "--workdir", str(proj.path / ".tox"))
+
+    result.assert_success()
+    found_calls = [(i[0][0].conf.name, i[0][3].run_id) for i in execute_calls.call_args_list]
+    assert found_calls == [
+        (".pkg", "_optional_hooks"),
+        (".pkg", "get_requires_for_build_wheel"),
+        (".pkg", "build_editable"),
+        ("a", "install_package"),
+        ("b", "install_package"),
+        (".pkg", "build_wheel"),
+        ("c", "install_package"),
+        ("d", "install_package"),
+        (".pkg", "_exit"),
+    ]
```

### Comparing `tox-4.6.1/tests/tox_env/python/virtual_env/package/test_python_package_util.py` & `tox-4.6.2/tests/tox_env/python/virtual_env/package/test_python_package_util.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/util/test_ci.py` & `tox-4.6.2/tests/util/test_ci.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/util/test_cpu.py` & `tox-4.6.2/tests/util/test_cpu.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/util/test_graph.py` & `tox-4.6.2/tests/util/test_graph.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/tests/util/test_spinner.py` & `tox-4.6.2/tests/util/test_spinner.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/LICENSE` & `tox-4.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/README.md` & `tox-4.6.2/README.md`

 * *Files identical despite different names*

### Comparing `tox-4.6.1/pyproject.toml` & `tox-4.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -52,46 +52,46 @@
   "chardet>=5.1",
   "colorama>=0.4.6",
   "filelock>=3.12.2",
   'importlib-metadata>=6.6; python_version < "3.8"',
   "packaging>=23.1",
   "platformdirs>=3.5.3",
   "pluggy>=1",
-  "pyproject-api>=1.5.1",
+  "pyproject-api>=1.5.2",
   'tomli>=2.0.1; python_version < "3.11"',
   'typing-extensions>=4.6.3; python_version < "3.8"',
-  "virtualenv>=20.23",
+  "virtualenv>=20.23.1",
 ]
 optional-dependencies.docs = [
   "furo>=2023.5.20",
   "sphinx>=7.0.1",
-  "sphinx-argparse-cli>=1.11",
-  "sphinx-autodoc-typehints!=1.23.4,>=1.23",
+  "sphinx-argparse-cli>=1.11.1",
+  "sphinx-autodoc-typehints!=1.23.4,>=1.23.2",
   "sphinx-copybutton>=0.5.2",
   "sphinx-inline-tabs>=2023.4.21",
   "sphinxcontrib-towncrier>=0.2.1a0",
   "towncrier>=23.6",
 ]
 optional-dependencies.testing = [
   "build[virtualenv]>=0.10",
   "covdefaults>=2.3",
   "detect-test-pollution>=1.1.1",
-  "devpi-process>=0.3",
+  "devpi-process>=0.3.1",
   "diff-cover>=7.6",
   "distlib>=0.3.6",
   "flaky>=3.7",
   "hatch-vcs>=0.3",
   "hatchling>=1.17.1",
   "psutil>=5.9.5",
   "pytest>=7.3.2",
   "pytest-cov>=4.1",
-  "pytest-mock>=3.10",
+  "pytest-mock>=3.11.1",
   "pytest-xdist>=3.3.1",
   "re-assert>=1.1",
-  'time-machine>=2.9; implementation_name != "pypy"',
+  'time-machine>=2.10; implementation_name != "pypy"',
   "wheel>=0.40",
 ]
 urls.Documentation = "https://tox.wiki"
 urls.Homepage = "http://tox.readthedocs.org"
 urls."Release Notes" = "https://tox.wiki/en/latest/changelog.html"
 urls.Source = "https://github.com/tox-dev/tox"
 urls.Tracker = "https://github.com/tox-dev/tox/issues"
@@ -102,14 +102,39 @@
 build.hooks.vcs.version-file = "src/tox/version.py"
 build.targets.sdist.include = ["/src", "/tests", "/tox.ini"]
 version.source = "vcs"
 
 [tool.black]
 line-length = 120
 
+[tool.ruff]
+select = ["ALL"]
+line-length = 120
+target-version = "py37"
+isort = {known-first-party = ["tox", "tests"], required-imports = ["from __future__ import annotations"]}
+ignore = [
+  "INP001",  # no implicit namespaces here
+  "D",  # ignore documentation for now
+  "ANN401",  # Dynamically typed expressions (typing.Any) are disallowed in `arg`"
+  "ANN101",  # Missing type annotation for `self` in method
+  "ANN102",  # Missing type annotation for `cls` in classmethod"
+  "D203",  # `one-blank-line-before-class` (D203) and `no-blank-line-before-class` (D211) are incompatible
+  "D212",  # `multi-line-summary-first-line` (D212) and `multi-line-summary-second-line` (D213) are incompatible
+  "S104",  # Possible binding to all interface
+]
+[tool.ruff.per-file-ignores]
+"tests/**/*.py" = [
+  "S101",  # asserts allowed in tests...
+  "FBT",  # don"t care about booleans as positional arguments in tests
+  "INP001", # no implicit namespace
+  "D",  # don"t care about documentation in tests
+  "S603",  # `subprocess` call: check for execution of untrusted input
+  "PLR2004",  # Magic value used in comparison, consider replacing with a constant variable
+]
+
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 addopts = "--tb=auto -ra --showlocals --no-success-flaky-report"
 
 [tool.coverage]
 html.show_contexts = true
 html.skip_covered = false
@@ -148,32 +173,7 @@
 name = "tox"
 filename = "docs/changelog.rst"
 directory = "docs/changelog"
 title_format = false
 issue_format = ":issue:`{issue}`"
 template = "docs/changelog/template.jinja2"
 # possible types, all default: feature, bugfix, doc, removal, misc
-
-[tool.ruff]
-select = ["ALL"]
-line-length = 120
-target-version = "py37"
-isort = {known-first-party = ["tox", "tests"], required-imports = ["from __future__ import annotations"]}
-ignore = [
-  "INP001",  # no implicit namespaces here
-  "D",  # ignore documentation for now
-  "ANN401",  # Dynamically typed expressions (typing.Any) are disallowed in `arg`"
-  "ANN101",  # Missing type annotation for `self` in method
-  "ANN102",  # Missing type annotation for `cls` in classmethod"
-  "D203",  # `one-blank-line-before-class` (D203) and `no-blank-line-before-class` (D211) are incompatible
-  "D212",  # `multi-line-summary-first-line` (D212) and `multi-line-summary-second-line` (D213) are incompatible
-  "S104",  # Possible binding to all interface
-]
-[tool.ruff.per-file-ignores]
-"tests/**/*.py" = [
-  "S101",  # asserts allowed in tests...
-  "FBT",  # don"t care about booleans as positional arguments in tests
-  "INP001", # no implicit namespace
-  "D",  # don"t care about documentation in tests
-  "S603",  # `subprocess` call: check for execution of untrusted input
-  "PLR2004",  # Magic value used in comparison, consider replacing with a constant variable
-]
```

### Comparing `tox-4.6.1/PKG-INFO` & `tox-4.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tox
-Version: 4.6.1
+Version: 4.6.2
 Summary: tox is a generic virtualenv management and test command line tool
 Project-URL: Documentation, https://tox.wiki
 Project-URL: Homepage, http://tox.readthedocs.org
 Project-URL: Release Notes, https://tox.wiki/en/latest/changelog.html
 Project-URL: Source, https://github.com/tox-dev/tox
 Project-URL: Tracker, https://github.com/tox-dev/tox/issues
 Author-email: Bernát Gábor <gaborjbernat@gmail.com>
@@ -34,44 +34,44 @@
 Requires-Dist: chardet>=5.1
 Requires-Dist: colorama>=0.4.6
 Requires-Dist: filelock>=3.12.2
 Requires-Dist: importlib-metadata>=6.6; python_version < '3.8'
 Requires-Dist: packaging>=23.1
 Requires-Dist: platformdirs>=3.5.3
 Requires-Dist: pluggy>=1
-Requires-Dist: pyproject-api>=1.5.1
+Requires-Dist: pyproject-api>=1.5.2
 Requires-Dist: tomli>=2.0.1; python_version < '3.11'
 Requires-Dist: typing-extensions>=4.6.3; python_version < '3.8'
-Requires-Dist: virtualenv>=20.23
+Requires-Dist: virtualenv>=20.23.1
 Provides-Extra: docs
 Requires-Dist: furo>=2023.5.20; extra == 'docs'
-Requires-Dist: sphinx-argparse-cli>=1.11; extra == 'docs'
-Requires-Dist: sphinx-autodoc-typehints!=1.23.4,>=1.23; extra == 'docs'
+Requires-Dist: sphinx-argparse-cli>=1.11.1; extra == 'docs'
+Requires-Dist: sphinx-autodoc-typehints!=1.23.4,>=1.23.2; extra == 'docs'
 Requires-Dist: sphinx-copybutton>=0.5.2; extra == 'docs'
 Requires-Dist: sphinx-inline-tabs>=2023.4.21; extra == 'docs'
 Requires-Dist: sphinx>=7.0.1; extra == 'docs'
 Requires-Dist: sphinxcontrib-towncrier>=0.2.1a0; extra == 'docs'
 Requires-Dist: towncrier>=23.6; extra == 'docs'
 Provides-Extra: testing
 Requires-Dist: build[virtualenv]>=0.10; extra == 'testing'
 Requires-Dist: covdefaults>=2.3; extra == 'testing'
 Requires-Dist: detect-test-pollution>=1.1.1; extra == 'testing'
-Requires-Dist: devpi-process>=0.3; extra == 'testing'
+Requires-Dist: devpi-process>=0.3.1; extra == 'testing'
 Requires-Dist: diff-cover>=7.6; extra == 'testing'
 Requires-Dist: distlib>=0.3.6; extra == 'testing'
 Requires-Dist: flaky>=3.7; extra == 'testing'
 Requires-Dist: hatch-vcs>=0.3; extra == 'testing'
 Requires-Dist: hatchling>=1.17.1; extra == 'testing'
 Requires-Dist: psutil>=5.9.5; extra == 'testing'
 Requires-Dist: pytest-cov>=4.1; extra == 'testing'
-Requires-Dist: pytest-mock>=3.10; extra == 'testing'
+Requires-Dist: pytest-mock>=3.11.1; extra == 'testing'
 Requires-Dist: pytest-xdist>=3.3.1; extra == 'testing'
 Requires-Dist: pytest>=7.3.2; extra == 'testing'
 Requires-Dist: re-assert>=1.1; extra == 'testing'
-Requires-Dist: time-machine>=2.9; implementation_name != 'pypy' and extra == 'testing'
+Requires-Dist: time-machine>=2.10; implementation_name != 'pypy' and extra == 'testing'
 Requires-Dist: wheel>=0.40; extra == 'testing'
 Description-Content-Type: text/markdown
 
 # tox
 
 [![PyPI](https://img.shields.io/pypi/v/tox)](https://pypi.org/project/tox/)
 [![Supported Python
```

