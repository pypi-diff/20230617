# Comparing `tmp/openllm-0.1.5.tar.gz` & `tmp/openllm-0.1.6.tar.gz`

## Comparing `openllm-0.1.5.tar` & `openllm-0.1.6.tar`

### file list

```diff
@@ -1,123 +1,145 @@
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 openllm-0.1.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 openllm-0.1.5/ADDING_NEW_MODEL.md
--rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 openllm-0.1.5/DEVELOPMENT.md
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 openllm-0.1.5/package.json
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 openllm-0.1.5/taplo.toml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 openllm-0.1.5/.github/CODEOWNERS
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 openllm-0.1.5/.github/dependabot.yml
--rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 openllm-0.1.5/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 openllm-0.1.5/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 openllm-0.1.5/.github/ISSUE_TEMPLATE/feature_request.yml
--rwxr-xr-x   0        0        0     1306 2020-02-02 00:00:00.000000 openllm-0.1.5/.github/actions/create_release_and_archive.sh
--rwxr-xr-x   0        0        0     1764 2020-02-02 00:00:00.000000 openllm-0.1.5/.github/actions/release.sh
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 openllm-0.1.5/.github/actions/setup-repo/action.yml
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 openllm-0.1.5/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 openllm-0.1.5/.github/workflows/create-releases.yml
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 openllm-0.1.5/.github/workflows/release-notes.yml
--rw-r--r--   0        0        0  1549838 2020-02-02 00:00:00.000000 openllm-0.1.5/assets/output.gif
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 openllm-0.1.5/examples/play.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/__about__.py
--rw-r--r--   0        0        0     8157 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/__init__.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/__main__.py
--rw-r--r--   0        0        0    50213 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/_configuration.py
--rw-r--r--   0        0        0    34895 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/_llm.py
--rw-r--r--   0        0        0    10649 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/_package.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/_prompt.py
--rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/_schema.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/_service.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/_types.py
--rw-r--r--   0        0        0    41496 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/cli.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/client.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/py.typed
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/__init__.py
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/auto/__init__.py
--rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/auto/configuration_auto.py
--rw-r--r--   0        0        0     9874 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/auto/factory.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/auto/modeling_auto.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/auto/modeling_flax_auto.py
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/auto/modeling_tf_auto.py
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/chatglm/__init__.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/chatglm/configuration_chatglm.py
--rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/chatglm/modeling_chatglm.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/dolly_v2/__init__.py
--rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/dolly_v2/configuration_dolly_v2.py
--rw-r--r--   0        0        0     4025 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/dolly_v2/modeling_dolly_v2.py
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/falcon/__init__.py
--rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/falcon/configuration_falcon.py
--rw-r--r--   0        0        0     5353 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/falcon/modeling_falcon.py
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/flan_t5/__init__.py
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/flan_t5/configuration_flan_t5.py
--rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/flan_t5/modeling_flan_t5.py
--rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/flan_t5/modeling_flax_flan_t5.py
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/flan_t5/modeling_tf_flan_t5.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/gpt_neox/__init__.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/gptj/__init__.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/llama/__init__.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/roberta/__init__.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/stablelm/__init__.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/stablelm/configuration_stablelm.py
--rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/stablelm/modeling_stablelm.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/starcoder/__init__.py
--rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/starcoder/configuration_starcoder.py
--rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/models/starcoder/modeling_starcoder.py
--rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/utils/__init__.py
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/utils/analytics.py
--rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/utils/codegen.py
--rw-r--r--   0        0        0    15309 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/utils/dantic.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/utils/dummy_flax_objects.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/utils/dummy_pt_and_einops_objects.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/utils/dummy_pt_objects.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/utils/dummy_tf_objects.py
--rw-r--r--   0        0        0    10442 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/utils/import_utils.py
--rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm/utils/lazy.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm_client/__init__.py
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm_client/_prompt.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm_client/cache/__init__.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm_client/cache/inmemory.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm_client/runtimes/__init__.py
--rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm_client/runtimes/base.py
--rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm_client/runtimes/grpc.py
--rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm_client/runtimes/http.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm_js/package.json
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm_js/tsconfig.cjs.json
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 openllm-0.1.5/src/openllm_js/tsconfig.json
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 openllm-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 openllm-0.1.5/tests/test_configuration.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.5/tests/_strategies/__init__.py
--rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 openllm-0.1.5/tests/_strategies/_configuration.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.5/tests/models/flan_t5/__init__.py
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 openllm-0.1.5/tests/models/flan_t5/test_modeling_flan_t5.py
--rwxr-xr-x   0        0        0      489 2020-02-02 00:00:00.000000 openllm-0.1.5/tools/add-license-headers
--rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 openllm-0.1.5/tools/assert-license-headers
--rwxr-xr-x   0        0        0      718 2020-02-02 00:00:00.000000 openllm-0.1.5/tools/assert-model-table-latest
--rwxr-xr-x   0        0        0     1901 2020-02-02 00:00:00.000000 openllm-0.1.5/tools/run-release-action
--rwxr-xr-x   0        0        0     1844 2020-02-02 00:00:00.000000 openllm-0.1.5/tools/update-optional-dependencies.py
--rwxr-xr-x   0        0        0     3559 2020-02-02 00:00:00.000000 openllm-0.1.5/tools/update-readme.py
--rw-r--r--   0        0        0    15605 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/attr/__init__.pyi
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/attr/_cmp.pyi
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/attr/_compat.pyi
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/attr/_typing_compat.pyi
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/attr/_version_info.pyi
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/attr/converters.pyi
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/attr/exceptions.pyi
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/attr/filters.pyi
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/attr/setters.pyi
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/attr/validators.pyi
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/click_option_group/__init__.pyi
--rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/click_option_group/_core.pyi
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/click_option_group/_decorators.pyi
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/click_option_group/_helpers.pyi
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/click_option_group/_version.pyi
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/deepmerge/__init__.pyi
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/deepmerge/merger.pyi
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/deepmerge/strategy/core.pyi
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/deepmerge/strategy/dict.pyi
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/deepmerge/strategy/list.pyi
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 openllm-0.1.5/typings/deepmerge/strategy/set.pyi
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 openllm-0.1.5/.gitignore
--rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.1.5/LICENSE.md
--rw-r--r--   0        0        0    13116 2020-02-02 00:00:00.000000 openllm-0.1.5/README.md
--rw-r--r--   0        0        0     6467 2020-02-02 00:00:00.000000 openllm-0.1.5/pyproject.toml
--rw-r--r--   0        0        0    15989 2020-02-02 00:00:00.000000 openllm-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 openllm-0.1.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 openllm-0.1.6/ADDING_NEW_MODEL.md
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 openllm-0.1.6/CHANGELOG.md
+-rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 openllm-0.1.6/DEVELOPMENT.md
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 openllm-0.1.6/package.json
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 openllm-0.1.6/taplo.toml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 openllm-0.1.6/.github/CODEOWNERS
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 openllm-0.1.6/.github/SECURITY.md
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 openllm-0.1.6/.github/dependabot.yml
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 openllm-0.1.6/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 openllm-0.1.6/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 openllm-0.1.6/.github/ISSUE_TEMPLATE/feature_request.yml
+-rwxr-xr-x   0        0        0     1428 2020-02-02 00:00:00.000000 openllm-0.1.6/.github/actions/create_release_and_archive.sh
+-rwxr-xr-x   0        0        0     1853 2020-02-02 00:00:00.000000 openllm-0.1.6/.github/actions/release.sh
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 openllm-0.1.6/.github/actions/setup-repo/action.yml
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 openllm-0.1.6/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 openllm-0.1.6/.github/workflows/create-releases.yml
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 openllm-0.1.6/.github/workflows/release-notes.yml
+-rw-r--r--   0        0        0  1549838 2020-02-02 00:00:00.000000 openllm-0.1.6/assets/output.gif
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 openllm-0.1.6/changelog.d/template.md.jinja
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 openllm-0.1.6/examples/bentoml-demo/bentofile.yaml
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 openllm-0.1.6/examples/bentoml-demo/service.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 openllm-0.1.6/examples/langchain-chains-demo/README.md
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 openllm-0.1.6/examples/langchain-chains-demo/bentofile.yaml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.6/examples/langchain-chains-demo/download_model.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 openllm-0.1.6/examples/langchain-chains-demo/service.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 openllm-0.1.6/examples/langchain-tools-demo/README.md
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 openllm-0.1.6/examples/langchain-tools-demo/bentofile.yaml
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 openllm-0.1.6/examples/langchain-tools-demo/bentoml_configuration.yaml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.6/examples/langchain-tools-demo/download_model.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 openllm-0.1.6/examples/langchain-tools-demo/requirements.txt
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 openllm-0.1.6/examples/langchain-tools-demo/service.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/__about__.py
+-rw-r--r--   0        0        0     8880 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/__init__.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/__main__.py
+-rw-r--r--   0        0        0    55304 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/_configuration.py
+-rw-r--r--   0        0        0    42241 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/_llm.py
+-rw-r--r--   0        0        0    12907 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/_package.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/_prompt.py
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/_schema.py
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/_service.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/_types.py
+-rw-r--r--   0        0        0    43661 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/cli.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/client.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/py.typed
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/__init__.py
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/auto/__init__.py
+-rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/auto/configuration_auto.py
+-rw-r--r--   0        0        0    12569 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/auto/factory.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/auto/modeling_auto.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/auto/modeling_flax_auto.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/auto/modeling_tf_auto.py
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/chatglm/__init__.py
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/chatglm/configuration_chatglm.py
+-rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/chatglm/modeling_chatglm.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/dolly_v2/__init__.py
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/dolly_v2/configuration_dolly_v2.py
+-rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/dolly_v2/modeling_dolly_v2.py
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/falcon/__init__.py
+-rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/falcon/configuration_falcon.py
+-rw-r--r--   0        0        0     5353 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/falcon/modeling_falcon.py
+-rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/flan_t5/__init__.py
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/flan_t5/configuration_flan_t5.py
+-rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/flan_t5/modeling_flan_t5.py
+-rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/flan_t5/modeling_flax_flan_t5.py
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/flan_t5/modeling_tf_flan_t5.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/gpt_neox/__init__.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/llama/__init__.py
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/opt/__init__.py
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/opt/configuration_opt.py
+-rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/opt/modeling_flax_opt.py
+-rw-r--r--   0        0        0     5941 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/opt/modeling_opt.py
+-rw-r--r--   0        0        0     4615 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/opt/modeling_tf_opt.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/roberta/__init__.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/stablelm/__init__.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/stablelm/configuration_stablelm.py
+-rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/stablelm/modeling_stablelm.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/starcoder/__init__.py
+-rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/starcoder/configuration_starcoder.py
+-rw-r--r--   0        0        0     5285 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/starcoder/modeling_starcoder.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/playground/README
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/playground/__init__.py
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/playground/features.py
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/playground/ft_opt_lora.py
+-rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/utils/__init__.py
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/utils/analytics.py
+-rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/utils/codegen.py
+-rw-r--r--   0        0        0    15415 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/utils/dantic.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/utils/dummy_flax_objects.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/utils/dummy_pt_and_einops_objects.py
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/utils/dummy_pt_objects.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/utils/dummy_tf_objects.py
+-rw-r--r--   0        0        0    11733 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/utils/import_utils.py
+-rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/utils/lazy.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm_client/__init__.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm_client/_prompt.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm_client/runtimes/__init__.py
+-rw-r--r--   0        0        0     7366 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm_client/runtimes/base.py
+-rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm_client/runtimes/grpc.py
+-rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm_client/runtimes/http.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm_js/package.json
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm_js/tsconfig.cjs.json
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm_js/tsconfig.json
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 openllm-0.1.6/tests/__init__.py
+-rw-r--r--   0        0        0     5566 2020-02-02 00:00:00.000000 openllm-0.1.6/tests/test_configuration.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.6/tests/_strategies/__init__.py
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 openllm-0.1.6/tests/_strategies/_configuration.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.6/tests/models/flan_t5/__init__.py
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 openllm-0.1.6/tests/models/flan_t5/test_modeling_flan_t5.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.6/tests/models/opt/__init__.py
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 openllm-0.1.6/tests/models/opt/test_modeling_opt.py
+-rwxr-xr-x   0        0        0      489 2020-02-02 00:00:00.000000 openllm-0.1.6/tools/add-license-headers
+-rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 openllm-0.1.6/tools/assert-license-headers
+-rwxr-xr-x   0        0        0      791 2020-02-02 00:00:00.000000 openllm-0.1.6/tools/assert-model-table-latest
+-rwxr-xr-x   0        0        0     1901 2020-02-02 00:00:00.000000 openllm-0.1.6/tools/run-release-action
+-rwxr-xr-x   0        0        0     2054 2020-02-02 00:00:00.000000 openllm-0.1.6/tools/update-optional-dependencies.py
+-rwxr-xr-x   0        0        0     3575 2020-02-02 00:00:00.000000 openllm-0.1.6/tools/update-readme.py
+-rw-r--r--   0        0        0    15605 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/attr/__init__.pyi
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/attr/_cmp.pyi
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/attr/_compat.pyi
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/attr/_typing_compat.pyi
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/attr/_version_info.pyi
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/attr/converters.pyi
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/attr/exceptions.pyi
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/attr/filters.pyi
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/attr/setters.pyi
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/attr/validators.pyi
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/click_option_group/__init__.pyi
+-rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/click_option_group/_core.pyi
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/click_option_group/_decorators.pyi
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/click_option_group/_helpers.pyi
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/click_option_group/_version.pyi
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/deepmerge/__init__.pyi
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/deepmerge/merger.pyi
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/deepmerge/strategy/core.pyi
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/deepmerge/strategy/dict.pyi
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/deepmerge/strategy/list.pyi
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/deepmerge/strategy/set.pyi
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 openllm-0.1.6/.gitignore
+-rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.1.6/LICENSE.md
+-rw-r--r--   0        0        0    13859 2020-02-02 00:00:00.000000 openllm-0.1.6/README.md
+-rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 openllm-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0    16980 2020-02-02 00:00:00.000000 openllm-0.1.6/PKG-INFO
```

### Comparing `openllm-0.1.5/ADDING_NEW_MODEL.md` & `openllm-0.1.6/ADDING_NEW_MODEL.md`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/package.json` & `openllm-0.1.6/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'0.1.6'"}*

```diff
@@ -11,12 +11,12 @@
     "engines": {
         "node": ">=16"
     },
     "license": "Apache 2.0",
     "name": "openllm",
     "private": true,
     "repository": "git@github.com:llmsys/OpenLLM.git",
-    "version": "0.1.5",
+    "version": "0.1.6",
     "workspaces": [
         "src/openllm_js"
     ]
 }
```

### Comparing `openllm-0.1.5/.github/dependabot.yml` & `openllm-0.1.6/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/.github/ISSUE_TEMPLATE/bug_report.yml` & `openllm-0.1.6/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/.github/ISSUE_TEMPLATE/config.yml` & `openllm-0.1.6/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/.github/ISSUE_TEMPLATE/feature_request.yml` & `openllm-0.1.6/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/.github/actions/create_release_and_archive.sh` & `openllm-0.1.6/.github/actions/create_release_and_archive.sh`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-
 set -o errexit -o nounset -o pipefail
 
 # Set by GH actions, see
 # https://docs.github.com/en/actions/learn-github-actions/environment-variables#default-environment-variables
 TAG=${GITHUB_REF_NAME#v}
 PREFIX="openllm-${TAG}"
 ARCHIVE="openllm-${TAG}.tar.gz"
@@ -37,8 +36,10 @@
 
 ## Usage
 
 All available models: \`\`\`python -m openllm.models\`\`\`
 
 To start a LLM: \`\`\`python -m openllm start dolly-v2\`\`\`
 
+Find more information about this release in the [CHANGELOG.md](https://github.com/bentoml/OpenLLM/blob/main/CHANGELOG.md)
+
 EOF
```

### Comparing `openllm-0.1.5/.github/actions/release.sh` & `openllm-0.1.6/.github/actions/release.sh`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     exit 1
 fi
 
 echo "Releasing version $RELEASE_VERSION..." && hatch version "${RELEASE_VERSION}"
 
 jq --arg release_version "${RELEASE_VERSION}" '.version = $release_version' < package.json > package.json.tmp && mv package.json.tmp package.json
 
+towncrier build --yes --version "${RELEASE_VERSION}" && git add CHANGELOG.md changelog.d
 git add src/openllm/__about__.py package.json && git commit -sm "infra: prepare for release ${RELEASE_VERSION} [generated]"
 git push origin main
 
 echo "Building artifacts for releasing..." && hatch build
 
 echo "Releasing version ${RELEASE_VERSION}" && hatch publish
```

### Comparing `openllm-0.1.5/.github/actions/setup-repo/action.yml` & `openllm-0.1.6/.github/actions/setup-repo/action.yml`

 * *Files 7% similar despite different names*

```diff
@@ -49,15 +49,15 @@
       with:
         path: ${{ steps.pip-cache-dir.outputs.dir }}
         key: ${{ steps.get-cache-key-prefix.outputs.prefix }}-pypi
         restore-keys: |
           ${{ steps.get-cache-key-prefix.outputs.prefix }}-pypi-
     - name: Install dependencies
       shell: bash
-      run: pip install -e ".[all]" hatch -vv
+      run: pip install -e ".[all]" hatch towncrier -vv
     - name: Install pyright
       shell: bash
       run: npm install -g npm@^7 pyright
     - name: Setup bufbuild/buf
       uses: bufbuild/buf-setup-action@v1.20.0
       with:
         github_token: ${{ github.token }}
```

### Comparing `openllm-0.1.5/.github/workflows/ci.yml` & `openllm-0.1.6/.github/workflows/ci.yml`

 * *Files 24% similar despite different names*

```diff
@@ -18,35 +18,20 @@
     branches: [main]
   pull_request:
   schedule:
     - cron: '0 0 * * 1/2'
 env:
   LINES: 120
   COLUMNS: 120
-  BENTOML_DO_NOT_TRACK: True
-  PYTEST_PLUGINS: bentoml.testing.pytest.plugin
+  OPENLLM_DO_NOT_TRACK: True
 # https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#defaultsrun
 defaults:
   run:
     shell: bash --noprofile --norc -exo pipefail {0}
 jobs:
-  codestyle_check:
-    runs-on: ubuntu-latest
-    if: ${{ github.event_name == 'pull_request' || github.event_name == 'push' }}
-    steps:
-      - uses: actions/checkout@v3
-        with:
-          fetch-depth: 0
-      - name: Setup CI
-        uses: ./.github/actions/setup-repo
-      - name: Format check
-        run: hatch run dev:style
-      - name: Type check
-        if: ${{ github.event_name == 'pull_request' }}
-        run: git diff --name-only --diff-filter=AM "origin/$GITHUB_BASE_REF" -z -- '*.py{,i}' | xargs -0 --no-run-if-empty hatch run dev:typing
   tests:
     runs-on: ubuntu-latest
     if: ${{ github.event_name == 'pull_request' || github.event_name == 'push' }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, macos-latest]
```

### Comparing `openllm-0.1.5/.github/workflows/create-releases.yml` & `openllm-0.1.6/.github/workflows/create-releases.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/.github/workflows/release-notes.yml` & `openllm-0.1.6/.github/workflows/release-notes.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/assets/output.gif` & `openllm-0.1.6/assets/output.gif`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/examples/play.py` & `openllm-0.1.6/examples/langchain-tools-demo/bentofile.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from __future__ import annotations
-
-import openllm
-
-model = openllm.AutoLLM.for_model("flan-t5")
+service: "service:svc"
+include:
+- "*.py"
+python:
+   requirements_txt: "./requirements.txt"
```

### Comparing `openllm-0.1.5/src/openllm/__about__.py` & `openllm-0.1.6/src/openllm/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "0.1.5"
+__version__ = "0.1.6"
```

### Comparing `openllm-0.1.5/src/openllm/__init__.py` & `openllm-0.1.6/src/openllm/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,42 +21,39 @@
 * Built-in support for StableLM, Llama, Dolly, Flan-T5, Vicuna
 * Option to bring your own fine-tuned LLMs
 * Online Serving with HTTP, gRPC, SSE(coming soon) or custom API
 * Native integration with BentoML and LangChain for custom LLM apps
 """
 from __future__ import annotations
 
-import logging as _
+import logging
 import typing as t
 
 from . import utils as utils
 from .__about__ import __version__ as __version__
 from .exceptions import MissingDependencyError
 
 if utils.DEBUG:
-    from bentoml._internal.configuration import set_debug_mode, set_quiet_mode
+    utils.set_debug_mode(True)
+    utils.set_quiet_mode(False)
 
-    set_debug_mode(True)
-    set_quiet_mode(False)
-
-    from bentoml._internal.log import configure_logging
-
-    configure_logging()
-    _.basicConfig(level=_.NOTSET)
+    utils.configure_logging()
+    logging.basicConfig(level=logging.NOTSET)
 
 
 _import_structure = {
     "_llm": ["LLM", "Runner", "LLMRunner"],
     "_configuration": ["LLMConfig"],
     "_package": ["build"],
     "exceptions": [],
     "_schema": ["GenerationInput", "GenerationOutput", "MetadataOutput"],
     "utils": [],
     "models": [],
     "client": [],
+    "playground": [],
     "cli": ["start", "start_grpc"],
     # NOTE: models
     "models.auto": [
         "AutoConfig",
         "CONFIG_MAPPING",
         "MODEL_MAPPING_NAMES",
         "MODEL_FLAX_MAPPING_NAMES",
@@ -64,14 +61,15 @@
     ],
     "models.flan_t5": ["FlanT5Config"],
     "models.dolly_v2": ["DollyV2Config"],
     "models.falcon": ["FalconConfig"],
     "models.chatglm": ["ChatGLMConfig"],
     "models.starcoder": ["StarCoderConfig"],
     "models.stablelm": ["StableLMConfig"],
+    "models.opt": ["OPTConfig"],
 }
 
 # NOTE: torch and cpm_kernels
 try:
     if not (utils.is_torch_available() and utils.is_cpm_kernels_available()):
         raise MissingDependencyError
 except MissingDependencyError:
@@ -104,68 +102,73 @@
 
     _import_structure["utils.dummy_pt_objects"] = [name for name in dir(dummy_pt_objects) if not name.startswith("_")]
 else:
     _import_structure["models.flan_t5"].extend(["FlanT5"])
     _import_structure["models.dolly_v2"].extend(["DollyV2"])
     _import_structure["models.starcoder"].extend(["StarCoder"])
     _import_structure["models.stablelm"].extend(["StableLM"])
+    _import_structure["models.opt"].extend(["OPT"])
     _import_structure["models.auto"].extend(["AutoLLM", "MODEL_MAPPING"])
 
 try:
     if not utils.is_flax_available():
         raise MissingDependencyError
 except MissingDependencyError:
     from .utils import dummy_flax_objects
 
     _import_structure["utils.dummy_flax_objects"] = [
         name for name in dir(dummy_flax_objects) if not name.startswith("_")
     ]
 else:
     _import_structure["models.flan_t5"].extend(["FlaxFlanT5"])
+    _import_structure["models.opt"].extend(["FlaxOPT"])
     _import_structure["models.auto"].extend(["AutoFlaxLLM", "MODEL_FLAX_MAPPING"])
 
 try:
     if not utils.is_tf_available():
         raise MissingDependencyError
 except MissingDependencyError:
     from .utils import dummy_tf_objects
 
     _import_structure["utils.dummy_tf_objects"] = [name for name in dir(dummy_tf_objects) if not name.startswith("_")]
 else:
     _import_structure["models.flan_t5"].extend(["TFFlanT5"])
+    _import_structure["models.opt"].extend(["TFOPT"])
     _import_structure["models.auto"].extend(["AutoTFLLM", "MODEL_TF_MAPPING"])
 
 
 # declaration for OpenLLM-related modules
 if t.TYPE_CHECKING:
     from . import cli as cli
     from . import client as client
     from . import exceptions as exceptions
     from . import models as models
-
+    from . import playground as playground
     # Specific types import
     from ._configuration import LLMConfig as LLMConfig
     from ._llm import LLM as LLM
     from ._llm import LLMRunner as LLMRunner
     from ._llm import Runner as Runner
     from ._package import build as build
     from ._schema import GenerationInput as GenerationInput
     from ._schema import GenerationOutput as GenerationOutput
     from ._schema import MetadataOutput as MetadataOutput
     from .cli import start as start
     from .cli import start_grpc as start_grpc
     from .models.auto import CONFIG_MAPPING as CONFIG_MAPPING
-    from .models.auto import MODEL_FLAX_MAPPING_NAMES as MODEL_FLAX_MAPPING_NAMES
+    from .models.auto import \
+        MODEL_FLAX_MAPPING_NAMES as MODEL_FLAX_MAPPING_NAMES
     from .models.auto import MODEL_MAPPING_NAMES as MODEL_MAPPING_NAMES
     from .models.auto import MODEL_TF_MAPPING_NAMES as MODEL_TF_MAPPING_NAMES
     from .models.auto import AutoConfig as AutoConfig
     from .models.chatglm import ChatGLMConfig as ChatGLMConfig
     from .models.dolly_v2 import DollyV2Config as DollyV2Config
     from .models.falcon import FalconConfig as FalconConfig
     from .models.flan_t5 import FlanT5Config as FlanT5Config
+    from .models.opt import OPTConfig as OPTConfig
     from .models.stablelm import StableLMConfig as StableLMConfig
     from .models.starcoder import StarCoderConfig as StarCoderConfig
 
     # NOTE: torch and cpm_kernels
     try:
         if not (utils.is_torch_available() and utils.is_cpm_kernels_available()):
             raise MissingDependencyError
@@ -189,40 +192,49 @@
     except MissingDependencyError:
         from .utils.dummy_pt_objects import *
     else:
         from .models.auto import MODEL_MAPPING as MODEL_MAPPING
         from .models.auto import AutoLLM as AutoLLM
         from .models.dolly_v2 import DollyV2 as DollyV2
         from .models.flan_t5 import FlanT5 as FlanT5
+        from .models.opt import OPT as OPT
         from .models.stablelm import StableLM as StableLM
         from .models.starcoder import StarCoder as StarCoder
 
     try:
         if not utils.is_flax_available():
             raise MissingDependencyError
     except MissingDependencyError:
         from .utils.dummy_flax_objects import *
     else:
         from .models.auto import MODEL_FLAX_MAPPING as MODEL_FLAX_MAPPING
         from .models.auto import AutoFlaxLLM as AutoFlaxLLM
         from .models.flan_t5 import FlaxFlanT5 as FlaxFlanT5
+        from .models.opt import FlaxOPT as FlaxOPT
 
     try:
         if not utils.is_tf_available():
             raise MissingDependencyError
     except MissingDependencyError:
         from .utils.dummy_tf_objects import *
     else:
         from .models.auto import MODEL_TF_MAPPING as MODEL_TF_MAPPING
         from .models.auto import AutoTFLLM as AutoTFLLM
         from .models.flan_t5 import TFFlanT5 as TFFlanT5
+        from .models.opt import TFOPT as TFOPT
 
 else:
     import sys
 
     sys.modules[__name__] = utils.LazyModule(
         __name__,
         globals()["__file__"],
         _import_structure,
         module_spec=__spec__,
-        extra_objects={"__version__": __version__},
+        extra_objects={
+            "__version__": __version__,
+            # The below is a special mapping that allows openllm to be used as a dictionary.
+            # This is purely for convenience sake, and should not be used in performance critcal
+            # code. This is also not considered as a public API.
+            "__openllm_special__": {"flax": "AutoFlaxLLM", "tf": "AutoTFLLM", "pt": "AutoLLM"},
+        },
     )
```

### Comparing `openllm-0.1.5/src/openllm/__main__.py` & `openllm-0.1.6/src/openllm/__main__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/src/openllm/_configuration.py` & `openllm-0.1.6/src/openllm/_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,35 +61,44 @@
 import inflection
 import orjson
 from cattr.gen import make_dict_unstructure_fn, override
 from deepmerge.merger import Merger
 
 import openllm
 
-from .exceptions import ForbiddenAttributeError, GpuNotAvailableError, OpenLLMException
-from .utils import DEBUG, LazyType, bentoml_cattr, codegen, dantic, first_not_none, lenient_issubclass
+from .exceptions import (ForbiddenAttributeError, GpuNotAvailableError,
+                         OpenLLMException)
+from .utils import (DEBUG, ENV_VARS_TRUE_VALUES, LazyType, bentoml_cattr,
+                    codegen, dantic, first_not_none, lenient_issubclass,
+                    non_intrusive_setattr)
 
 if hasattr(t, "Required"):
     from typing import Required
 else:
     from typing_extensions import Required
 
 if hasattr(t, "NotRequired"):
     from typing import NotRequired
 else:
     from typing_extensions import NotRequired
 
+if hasattr(t, "dataclass_transform"):
+    from typing import dataclass_transform
+else:
+    from typing_extensions import dataclass_transform
+
 _T = t.TypeVar("_T")
 
 
 if t.TYPE_CHECKING:
     import tensorflow as tf
     import torch
     import transformers
-    from attr import _CountingAttr, _make_init, _make_repr, _transform_attrs  # type: ignore
+    from attr import (_CountingAttr, _make_init, _make_repr,  # type: ignore
+                      _transform_attrs)
     from transformers.generation.beam_constraints import Constraint
 
     from ._types import ClickFunctionWrapper, F, O_co, P
 
     ReprArgs: t.TypeAlias = t.Iterable[tuple[str | None, t.Any]]
 
     DictStrAny = dict[str, t.Any]
@@ -99,15 +108,16 @@
 else:
     Constraint = t.Any
     ListStr = list
     DictStrAny = dict
     ItemgetterAny = itemgetter
     # NOTE: Using internal API from attr here, since we are actually
     # allowing subclass of openllm.LLMConfig to become 'attrs'-ish
-    from attr._make import _CountingAttr, _make_init, _make_repr, _transform_attrs
+    from attr._make import (_CountingAttr, _make_init, _make_repr,
+                            _transform_attrs)
 
     transformers = openllm.utils.LazyLoader("transformers", globals(), "transformers")
     torch = openllm.utils.LazyLoader("torch", globals(), "torch")
     tf = openllm.utils.LazyLoader("tf", globals(), "tensorflow")
 
 __all__ = ["LLMConfig"]
 
@@ -365,35 +375,31 @@
         if not _internal:
             raise RuntimeError(
                 "GenerationConfig is not meant to be used directly, "
                 "but you can access this via a LLMConfig.generation_config"
             )
         self.__attrs_init__(**attrs)
 
+    def __getitem__(self, item: str) -> t.Any:
+        if hasattr(self, item):
+            return getattr(self, item)
+        raise KeyError(f"GenerationConfig has no attribute {item}")
+
 
 bentoml_cattr.register_unstructure_hook_factory(
     lambda cls: attr.has(cls) and lenient_issubclass(cls, GenerationConfig),
     lambda cls: make_dict_unstructure_fn(
         cls,
         bentoml_cattr,
         **{k: override(omit=True) for k, v in attr.fields_dict(cls).items() if v.default in (None, attr.NOTHING)},
     ),
 )
 
 
-def _populate_value_from_env_var(
-    key: str, transform: t.Callable[[str], str] | None = None, fallback: t.Any = None
-) -> t.Any:
-    if transform is not None and callable(transform):
-        key = transform(key)
-
-    return os.environ.get(key, fallback)
-
-
-def _field_env_key(model_name: str, key: str, suffix: str | None = None) -> str:
+def _field_env_key(model_name: str, key: str, suffix: str | t.Literal[""] | None = None) -> str:
     return "_".join(filter(None, map(str.upper, ["OPENLLM", model_name, suffix.strip("_") if suffix else "", key])))
 
 
 # cached it here to save one lookup per assignment
 _object_getattribute = object.__getattribute__
 
 
@@ -406,16 +412,23 @@
     default_id: Required[str]
     model_ids: Required[ListStr]
 
     # meta
     url: str
     requires_gpu: bool
     trust_remote_code: bool
+    service_name: NotRequired[str]
     requirements: t.Optional[ListStr]
 
+    # llm implementation specifics
+    use_pipeline: bool
+    bettertransformer: bool
+    model_type: t.Literal["causal_lm", "seq2seq_lm"]
+    runtime: t.Literal["transformers", "cpp"]
+
     # naming convention, only name_type is needed to infer from the class
     # as the three below it can be determined automatically
     name_type: t.Literal["dasherize", "lowercase"]
     model_name: NotRequired[str]
     start_name: NotRequired[str]
     env: NotRequired[openllm.utils.ModelEnv]
 
@@ -423,153 +436,246 @@
     timeout: int
     workers_per_resource: t.Union[int, float]
 
     # the target generation_config class to be used.
     generation_class: t.Type[GenerationConfig]
 
 
-_ModelSettings: type[attr.AttrsInstance] = codegen.add_method_dunders(
-    type("__openllm_internal__", (ModelSettings,), {"__module__": "openllm._configuration"}),
-    attr.make_class(
-        "ModelSettings",
-        {
-            k: dantic.Field(
+def _settings_field_transformer(
+    _: type[attr.AttrsInstance], __: list[attr.Attribute[t.Any]]
+) -> list[attr.Attribute[t.Any]]:
+    return [
+        attr.Attribute.from_counting_attr(
+            k,
+            dantic.Field(
                 kw_only=False if t.get_origin(ann) is not Required else True,
                 auto_default=True,
                 use_default_converter=False,
                 type=ann,
-                metadata={
-                    "target": f"__openllm_{k}__",
-                    "required": False if t.get_origin(ann) is NotRequired else t.get_origin(ann) is Required,
-                },
+                metadata={"target": f"__openllm_{k}__"},
                 description=f"ModelSettings field for {k}.",
-            )
-            for k, ann in t.get_type_hints(ModelSettings).items()
-        },
-        bases=(DictStrAny,),
-        slots=True,
-        weakref_slot=True,
-        collect_by_mro=True,
-    ),
-    _overwrite_doc="Internal attrs representation of ModelSettings.",
-)
+            ),
+        )
+        for k, ann in t.get_type_hints(ModelSettings).items()
+    ]
 
 
-def structure_settings(cl_: type[LLMConfig], cls: type[t.Any]):
-    if not lenient_issubclass(cl_, LLMConfig):
-        raise RuntimeError(f"Given LLMConfig must be a subclass type of 'LLMConfig', got '{cl_}' instead.")
-    settings = cl_.__config__
+@attr.define(slots=True, field_transformer=_settings_field_transformer, frozen=False)
+class _ModelSettingsAttr:
+    """Internal attrs representation of ModelSettings."""
+
+    def __getitem__(self, key: str) -> t.Any:
+        if key in codegen.get_annotations(ModelSettings):
+            return _object_getattribute(self, key)
+        raise KeyError(key)
 
-    if settings is None:
-        raise RuntimeError("Given LLMConfig must have '__config__' defined.")
+    @classmethod
+    def default(cls) -> _ModelSettingsAttr:
+        _ = ModelSettings(
+            default_id="__default__",
+            model_ids=["__default__"],
+            name_type="dasherize",
+            requires_gpu=False,
+            url="",
+            use_pipeline=False,
+            model_type="causal_lm",
+            trust_remote_code=False,
+            requirements=None,
+            timeout=3600,
+            service_name="",
+            workers_per_resource=1,
+            runtime="transformers",
+        )
+        return cls(**t.cast(DictStrAny, _))
 
-    required = [i.name for i in attr.fields(cls) if i.metadata.get("required", False)]
-    if any(k not in settings for k in required):
-        raise ValueError(f"The following keys are required under '__config__': {required}")
-    if not settings["default_id"] or not settings["model_ids"]:
-        raise ValueError("Make sure that either 'default_id', 'model_ids' are not emptied under '__config__'.")
 
-    if any(k in settings for k in ("env", "start_name", "model_name")):
-        raise ValueError("The following keys are not allowed under '__config__': env, start_name, model_name")
+def structure_settings(cl_: type[LLMConfig], cls: type[_ModelSettingsAttr]):
+    if not lenient_issubclass(cl_, LLMConfig):
+        raise RuntimeError(f"Given '{cl_}' must be a subclass type of 'LLMConfig', got '{cl_}' instead.")
+
+    if not hasattr(cl_, "__config__") or getattr(cl_, "__config__") is None:
+        raise RuntimeError("Given LLMConfig must have '__config__' that is not None defined.")
+
+    assert cl_.__config__ is not None
 
-    if "generation_class" in settings:
+    if "generation_class" in cl_.__config__:
         raise ValueError(
             "'generation_class' shouldn't be defined in '__config__', rather defining "
-            f"all required attributes under '{cl_}.GenerationConfig' when defining the class."
+            f"all required attributes under '{cl_}.GenerationConfig' instead."
         )
 
     _cl_name = cl_.__name__.replace("Config", "")
-    name_type = first_not_none(settings.get("name_type"), "dasherize")
-    model_name = inflection.underscore(_cl_name) if name_type == "dasherize" else _cl_name.lower()
-    start_name = inflection.dasherize(model_name) if name_type == "dasherize" else model_name
-    partialed = functools.partial(_field_env_key, model_name=model_name, suffix="generation")
-
-    def auto_env_transformers(_: t.Any, fields: list[attr.Attribute[t.Any]]) -> list[attr.Attribute[t.Any]]:
-        _has_own_gen = codegen.has_own_attribute(cl_, "GenerationConfig")
-        return [
-            f.evolve(
-                default=_populate_value_from_env_var(
-                    partialed(key=f.name),
-                    fallback=getattr(cl_.GenerationConfig, f.name, f.default) if _has_own_gen else f.default,
-                ),
-                metadata={"env": partialed(key=f.name), "description": f.metadata.get("description", "(not provided)")},
-                converter=None,
-            )
-            for f in fields
-        ]
 
-    return cls(
-        default_id=settings["default_id"],
-        model_ids=settings["model_ids"],
-        url=settings.get("url", ""),
-        requires_gpu=settings.get("requires_gpu", False),
-        trust_remote_code=settings.get("trust_remote_code", False),
-        requirements=settings.get("requirements", None),
-        name_type=name_type,
-        model_name=model_name,
-        start_name=start_name,
-        env=openllm.utils.ModelEnv(model_name),
-        timeout=settings.get("timeout", 3600),
-        workers_per_resource=settings.get("workers_per_resource", 1),
-        generation_class=attr.make_class(
-            f"{_cl_name}GenerationConfig",
-            [],
-            bases=(GenerationConfig,),
-            slots=True,
-            weakref_slot=True,
-            frozen=False,
-            repr=True,
-            field_transformer=auto_env_transformers,
+    _settings_attr = _ModelSettingsAttr.default()
+    try:
+        cls(**t.cast(DictStrAny, cl_.__config__))
+        _settings_attr = attr.evolve(_settings_attr, **t.cast(DictStrAny, cl_.__config__))
+    except TypeError:
+        raise ValueError("Either 'default_id' or 'model_ids' are emptied under '__config__' (required fields).")
+
+    _final_value_dct: DictStrAny = {
+        "model_name": inflection.underscore(_cl_name)
+        if _settings_attr["name_type"] == "dasherize"
+        else _cl_name.lower()
+    }
+    _final_value_dct["start_name"] = (
+        inflection.dasherize(_final_value_dct["model_name"])
+        if _settings_attr["name_type"] == "dasherize"
+        else _final_value_dct["model_name"]
+    )
+    env = openllm.utils.ModelEnv(_final_value_dct["model_name"])
+    _final_value_dct["env"] = env
+
+    # bettertransformer support
+    if _settings_attr["bettertransformer"] is None:
+        _final_value_dct["bettertransformer"] = (
+            os.environ.get(env.bettertransformer, str(False)).upper() in ENV_VARS_TRUE_VALUES
+        )
+    if _settings_attr["requires_gpu"]:
+        # if requires_gpu is True, then disable BetterTransformer for quantization.
+        _final_value_dct["bettertransformer"] = False
+
+    _final_value_dct["service_name"] = f"generated_{_final_value_dct['model_name']}_service.py"
+    _final_value_dct["generation_class"] = attr.make_class(
+        f"{_cl_name}GenerationConfig",
+        [],
+        bases=(GenerationConfig,),
+        slots=True,
+        weakref_slot=True,
+        frozen=True,
+        repr=True,
+        collect_by_mro=True,
+        field_transformer=_make_env_transformer(
+            cl_,
+            _final_value_dct["model_name"],
+            suffix="generation",
+            default_callback=lambda field_name, field_default: getattr(cl_.GenerationConfig, field_name, field_default)
+            if codegen.has_own_attribute(cl_, "GenerationConfig")
+            else field_default,
+            globs={"cl_": cl_},
         ),
     )
 
+    return attr.evolve(_settings_attr, **_final_value_dct)
+
+
+bentoml_cattr.register_structure_hook(_ModelSettingsAttr, structure_settings)
+
+
+def _make_env_transformer(
+    cls: type[LLMConfig],
+    model_name: str,
+    suffix: t.LiteralString | None = None,
+    default_callback: t.Callable[[str, t.Any], t.Any] | None = None,
+    globs: DictStrAny | None = None,
+):
+    def identity(_: str, x_value: t.Any) -> t.Any:
+        return x_value
+
+    default_callback = identity if default_callback is None else default_callback
+
+    globs = {} if globs is None else globs
+    globs.update(
+        {
+            "functools": functools,
+            "__populate_env": dantic.env_converter,
+            "__default_callback": default_callback,
+            "__field_env": _field_env_key,
+            "__suffix": suffix or "",
+            "__model_name": model_name,
+        }
+    )
+
+    lines: ListStr = [
+        "__env = lambda field_name: __field_env(__model_name, field_name, __suffix)",
+        "return [",
+        "    f.evolve(",
+        "        default=__populate_env(__default_callback(f.name, f.default), __env(f.name)),",
+        "        metadata={",
+        "            'env': f.metadata.get('env', __env(f.name)),",
+        "            'description': f.metadata.get('description', '(not provided)'),",
+        "        },",
+        "    )",
+        "    for f in fields",
+        "]",
+    ]
+    fields_ann = "list[attr.Attribute[t.Any]]"
 
-bentoml_cattr.register_structure_hook(_ModelSettings, structure_settings)
+    return codegen.generate_function(
+        cls,
+        "__auto_env",
+        lines,
+        args=("_", "fields"),
+        globs=globs,
+        annotations={"_": "type[LLMConfig]", "fields": fields_ann, "return": fields_ann},
+    )
 
 
 def _setattr_class(attr_name: str, value_var: t.Any, add_dunder: bool = False):
     """
     Use the builtin setattr to set *attr_name* to *value_var*.
     We can't use the cached object.__setattr__ since we are setting
     attributes to a class.
+
+    If add_dunder to True, the generated globs should include a __add_dunder
+    value that will be used to add the dunder methods to the class for given
+    value_var
     """
-    if add_dunder:
-        return f"setattr(cls, '{attr_name}', __add_dunder(cls, {value_var}))"
-    return f"setattr(cls, '{attr_name}', {value_var})"
+    val = f"__add_dunder(cls, {value_var})" if add_dunder else value_var
+    return f"setattr(cls, '{attr_name}', {val})"
 
 
 _dunder_add = {"generation_class"}
 
 
-def _make_assignment_script(cls: type[LLMConfig], attributes: attr.AttrsInstance) -> t.Callable[..., None]:
+def _make_assignment_script(
+    cls: type[LLMConfig], attributes: attr.AttrsInstance, _prefix: t.LiteralString = "openllm"
+) -> t.Callable[..., None]:
     """Generate the assignment script with prefix attributes __openllm_<value>__"""
     args: ListStr = []
     globs: DictStrAny = {
         "cls": cls,
         "_cached_attribute": attributes,
         "_cached_getattribute_get": _object_getattribute.__get__,
         "__add_dunder": codegen.add_method_dunders,
     }
     annotations: DictStrAny = {"return": None}
 
     lines: ListStr = ["_getattr = _cached_getattribute_get(_cached_attribute)"]
     for attr_name, field in attr.fields_dict(attributes.__class__).items():
-        arg_name = field.metadata.get("target", f"__openllm_{inflection.underscore(attr_name)}__")
+        arg_name = field.metadata.get("target", f"__{_prefix}_{inflection.underscore(attr_name)}__")
         args.append(f"{attr_name}=getattr(_cached_attribute, '{attr_name}')")
         lines.append(_setattr_class(arg_name, attr_name, add_dunder=attr_name in _dunder_add))
         annotations[attr_name] = field.type
 
     return codegen.generate_function(
         cls, "__assign_attr", lines, args=("cls", *args), globs=globs, annotations=annotations
     )
 
 
 _reserved_namespace = {"__config__", "GenerationConfig"}
 
 
+@dataclass_transform(order_default=True, field_specifiers=(attr.field, dantic.Field))
+def __llm_config_transform__(cls: type[LLMConfig]) -> type[LLMConfig]:
+    kwargs: dict[str, t.Any] = {}
+    if hasattr(cls, "GenerationConfig"):
+        kwargs = {k: v for k, v in vars(cls.GenerationConfig).items() if not k.startswith("_")}
+    non_intrusive_setattr(
+        cls,
+        "__dataclass_transform__",
+        {
+            "order_default": True,
+            "field_specifiers": (attr.field, dantic.Field),
+            "kwargs": kwargs,
+        },
+    )
+    return cls
+
+
 @attr.define(slots=True)
 class LLMConfig:
     """
     ``openllm.LLMConfig`` is somewhat a hybrid combination between the performance of `attrs` with the
     easy-to-use interface that pydantic offer. It lives in between where it allows users to quickly formulate
     a LLMConfig for any LLM without worrying too much about performance. It does a few things:
 
@@ -634,19 +740,19 @@
         field1 = openllm.LLMConfig.Field(...)
     ```
     """
 
     # NOTE: The following is handled via __init_subclass__, and is only used for TYPE_CHECKING
     if t.TYPE_CHECKING:
         # NOTE: public attributes to override
-        __config__: ModelSettings | None = None
+        __config__: ModelSettings | None = Field(None)
         """Internal configuration for this LLM model. Each of the field in here will be populated
         and prefixed with __openllm_<value>__"""
 
-        GenerationConfig: type = type
+        GenerationConfig: type = Field(None)
         """Users can override this subclass of any given LLMConfig to provide GenerationConfig
         default value. For example:
 
         ```python
         class MyAwesomeModelConfig(openllm.LLMConfig):
             class GenerationConfig:
                 max_new_tokens: int = 200
@@ -657,15 +763,15 @@
         """
 
         # NOTE: Internal attributes that should only be used by OpenLLM. Users usually shouldn't
         # concern any of these. These are here for pyright not to complain.
         def __attrs_init__(self, **attrs: t.Any):
             """Generated __attrs_init__ for LLMConfig subclass that follows the attrs contract."""
 
-        __attrs_attrs__: tuple[attr.Attribute[t.Any], ...] = tuple()
+        __attrs_attrs__: tuple[attr.Attribute[t.Any], ...] = Field(None, init=False)
         """Since we are writing our own __init_subclass__, which is an alternative way for __prepare__,
         we want openllm.LLMConfig to be attrs-like dataclass that has pydantic-like interface.
         __attrs_attrs__ will be handled dynamically by __init_subclass__.
         """
 
         __openllm_hints__: DictStrAny = Field(None, init=False)
         """An internal cache of resolved types for this LLMConfig."""
@@ -674,64 +780,100 @@
         """The accepted keys for this LLMConfig."""
 
         __openllm_extras__: DictStrAny = Field(None, init=False)
         """Extra metadata for this LLMConfig."""
 
         # NOTE: The following will be populated from __config__ and also
         # considered to be public API.
+        __openllm_default_id__: str = Field(None)
+        """Return the default model to use when using 'openllm start <model_id>'.
+        This could be one of the keys in 'self.model_ids' or custom users model.
+
+        This field is required when defining under '__config__'.
+        """
+
+        __openllm_model_ids__: ListStr = Field(None)
+        """A list of supported pretrained models tag for this given runnable.
+
+        For example:
+            For FLAN-T5 impl, this would be ["google/flan-t5-small", "google/flan-t5-base",
+                                                "google/flan-t5-large", "google/flan-t5-xl", "google/flan-t5-xxl"]
+
+        This field is required when defining under '__config__'.
+        """
+
         __openllm_url__: str = Field(None, init=False)
         """The resolved url for this LLMConfig."""
 
-        __openllm_requires_gpu__: bool = False
+        __openllm_requires_gpu__: bool = Field(None, init=False)
         """Determines if this model is only available on GPU. By default it supports GPU and fallback to CPU."""
 
-        __openllm_trust_remote_code__: bool = False
+        __openllm_trust_remote_code__: bool = Field(False)
         """Whether to always trust remote code"""
 
-        __openllm_requirements__: ListStr | None = None
+        __openllm_service_name__: str = Field(None)
+        """Generated service name for this LLMConfig. By default, it is 'generated_{model_name}_service.py'"""
+
+        __openllm_requirements__: ListStr | None = Field(None)
         """The default PyPI requirements needed to run this given LLM. By default, we will depend on
         bentoml, torch, transformers."""
 
-        __openllm_env__: openllm.utils.ModelEnv = Field(None, init=False)
-        """A ModelEnv instance for this LLMConfig."""
+        __openllm_use_pipeline__: bool = Field(False)
+        """Whether this LLM will use HuggingFace Pipeline API. By default, this is set to False.
+        The reason for this to be here is because we want to access this object before loading
+        the _bentomodel. This is because we will actually download the model weights when accessing
+        _bentomodel.
+        """
 
-        __openllm_model_name__: str = ""
-        """The normalized version of __openllm_start_name__, determined by __openllm_name_type__"""
+        __openllm_bettertransformer__: bool = Field(False)
+        """Whether to use BetterTransformer for this given LLM. This depends per model
+        architecture. By default, we will use BetterTransformer for T5 and StableLM models,
+        and set to False for every other models.
+        """
 
-        __openllm_start_name__: str = ""
-        """Default name to be used with `openllm start`"""
+        __openllm_model_type__: t.Literal["causal_lm", "seq2seq_lm"] = Field("causal_lm")
+        """The model type for this given LLM. By default, it should be causal language modeling.
+        Currently supported 'causal_lm' or 'seq2seq_lm'
+        """
+
+        __openllm_runtime__: t.Literal["transformers", "cpp"] = Field("transformers")
+        """The runtime to use for this model. Possible values are `transformers` or `cpp`. See
+        LlaMA for more information."""
 
-        __openllm_name_type__: t.Literal["dasherize", "lowercase"] = "dasherize"
+        __openllm_name_type__: t.Literal["dasherize", "lowercase"] = Field("dasherize")
         """the default name typed for this model. "dasherize" will convert the name to lowercase and
         replace spaces with dashes. "lowercase" will convert the name to lowercase."""
 
-        __openllm_timeout__: int = 3600
+        __openllm_model_name__: str = Field(None)
+        """The normalized version of __openllm_start_name__, determined by __openllm_name_type__"""
+
+        __openllm_start_name__: str = Field(None)
+        """Default name to be used with `openllm start`"""
+
+        __openllm_env__: openllm.utils.ModelEnv = Field(None, init=False)
+        """A ModelEnv instance for this LLMConfig."""
+
+        __openllm_timeout__: int = Field(36000)
         """The default timeout to be set for this given LLM."""
 
-        __openllm_workers_per_resource__: int | float = 1
-        """The default number of workers per resource. By default, we will use 1 worker per resource.
+        __openllm_workers_per_resource__: int | float = Field(1)
+        """The number of workers per resource. This is used to determine the number of workers to use for this model.
+        For example, if this is set to 0.5, then OpenLLM will use 1 worker per 2 resources. If this is set to 1, then
+        OpenLLM will use 1 worker per resource. If this is set to 2, then OpenLLM will use 2 workers per resource.
+
         See StarCoder for more advanced usage. See
         https://docs.bentoml.org/en/latest/guides/scheduling.html#resource-scheduling-strategy for more details.
-        """
 
-        __openllm_default_id__: str = Field(None)
-        """Return the default model to use when using 'openllm start <model_id>'.
-        This could be one of the keys in 'self.model_ids' or custom users model."""
-
-        __openllm_model_ids__: ListStr = Field(None)
-        """A list of supported pretrained models tag for this given runnable.
-
-        For example:
-            For FLAN-T5 impl, this would be ["google/flan-t5-small", "google/flan-t5-base",
-                                                "google/flan-t5-large", "google/flan-t5-xl", "google/flan-t5-xxl"]
+        By default, it is set to 1.
         """
 
         __openllm_generation_class__: type[GenerationConfig] = Field(None, init=False)
         """The result generated GenerationConfig class for this LLMConfig. This will be used
-        to create the generation_config argument that can be used throughout the lifecycle."""
+        to create the generation_config argument that can be used throughout the lifecycle.
+        This class will also be managed internally by OpenLLM."""
 
     def __init_subclass__(cls):
         """The purpose of this __init_subclass__ is that we want all subclass of LLMConfig
         to adhere to the attrs contract, and have pydantic-like interface. This means we will
         construct all fields and metadata and hack into how attrs use some of the 'magic' construction
         to generate the fields.
 
@@ -739,46 +881,33 @@
         ModelSettings (derived from __config__) to the class.
         """
         if not cls.__name__.endswith("Config"):
             logger.warning("LLMConfig subclass should end with 'Config'. Updating to %sConfig", cls.__name__)
             cls.__name__ = f"{cls.__name__}Config"
 
         # NOTE: auto assignment attributes generated from __config__
-        _make_assignment_script(cls, bentoml_cattr.structure(cls, _ModelSettings))(cls)
+        _make_assignment_script(cls, bentoml_cattr.structure(cls, _ModelSettingsAttr))(cls)
         # process a fields under cls.__dict__ and auto convert them with dantic.Field
         cd = cls.__dict__
         anns = codegen.get_annotations(cls)
-        partialed = functools.partial(_field_env_key, model_name=cls.__openllm_model_name__)
-
-        def auto_config_env(_: type[LLMConfig], attrs: list[attr.Attribute[t.Any]]) -> list[attr.Attribute[t.Any]]:
-            return [
-                a.evolve(
-                    default=_populate_value_from_env_var(partialed(key=a.name), fallback=a.default),
-                    metadata={
-                        "env": a.metadata.get("env", partialed(key=a.name)),
-                        "description": a.metadata.get("description", "(not provided)"),
-                    },
-                )
-                for a in attrs
-            ]
 
         # _CountingAttr is the underlying representation of attr.field
         ca_names = {name for name, attr in cd.items() if isinstance(attr, _CountingAttr)}
         these: dict[str, _CountingAttr[t.Any]] = {}
         annotated_names: set[str] = set()
         for attr_name, typ in anns.items():
             if codegen.is_class_var(typ):
                 continue
             annotated_names.add(attr_name)
             val = cd.get(attr_name, attr.NOTHING)
             if not LazyType["_CountingAttr[t.Any]"](_CountingAttr).isinstance(val):
                 if val is attr.NOTHING:
-                    val = cls.Field(env=partialed(key=attr_name))
+                    val = cls.Field(env=_field_env_key(cls.__openllm_model_name__, attr_name))
                 else:
-                    val = cls.Field(default=val, env=partialed(key=attr_name))
+                    val = cls.Field(default=val, env=_field_env_key(cls.__openllm_model_name__, attr_name))
             these[attr_name] = val
         unannotated = ca_names - annotated_names
         if len(unannotated) > 0:
             missing_annotated = sorted(unannotated, key=lambda n: t.cast("_CountingAttr[t.Any]", cd.get(n)).counter)
             raise openllm.exceptions.MissingAnnotationAttributeError(
                 f"The following field doesn't have a type annotation: {missing_annotated}"
             )
@@ -788,24 +917,25 @@
         }
 
         # 'generation_config' is a special fields that wraps the GenerationConfig class
         # which is handled in _make_assignment_script
         these["generation_config"] = cls.Field(
             default=cls.__openllm_generation_class__(),
             description=inspect.cleandoc(cls.__openllm_generation_class__.__doc__ or ""),
+            type=GenerationConfig,
         )
 
         # Generate the base __attrs_attrs__ transformation here.
         attrs, base_attrs, base_attr_map = _transform_attrs(
             cls,  # the current class
             these,  # the parsed attributes we previous did
             False,  # disable auto_attribs, since we already handle these
             False,  # disable kw_only
             True,  # collect_by_mro
-            field_transformer=auto_config_env,
+            field_transformer=_make_env_transformer(cls, cls.__openllm_model_name__),
         )
         _weakref_slot = True  # slots = True
         _base_names = {a.name for a in base_attrs}
         _attr_names = tuple(a.name for a in attrs)
         _has_pre_init = bool(getattr(cls, "__attrs_pre_init__", False))
         _has_post_init = bool(getattr(cls, "__attrs_post_init__", False))
         # the protocol for attrs-decorated class
@@ -813,15 +943,15 @@
         # generate a __attrs_init__ for the subclass, since we will
         # implement a custom __init__
         cls.__attrs_init__ = codegen.add_method_dunders(
             cls,
             _make_init(
                 cls,  # cls (the attrs-decorated class)
                 attrs,  # tuple of attr.Attribute of cls
-                _has_pre_init,  # pre_initjk
+                _has_pre_init,  # pre_init
                 _has_post_init,  # post_init
                 False,  # frozen
                 True,  # slots
                 False,  # cache_hash
                 base_attr_map,  # base_attr_map
                 False,  # is_exc (check if it is exception)
                 None,  # cls_on_setattr (essentially attr.setters)
@@ -868,14 +998,15 @@
             attr.resolve_types(cls.__openllm_generation_class__, globalns=globs)
 
             cls = attr.resolve_types(cls, globalns=globs)
         # the hint cache for easier access
         cls.__openllm_hints__ = {
             f.name: f.type for ite in map(attr.fields, (cls, cls.__openllm_generation_class__)) for f in ite
         }
+        cls = __llm_config_transform__(cls)
 
     def __setattr__(self, attr: str, value: t.Any):
         if attr in _reserved_namespace:
             raise ForbiddenAttributeError(
                 f"{attr} should not be set during runtime "
                 f"as these value will be reflected during runtime. "
                 f"Instead, you can create a custom LLM subclass {self.__class__.__name__}."
@@ -893,22 +1024,15 @@
         # create a copy of the keys as cache
         _cached_keys = tuple(attrs.keys())
 
         _generation_cl_dict = attr.fields_dict(self.__openllm_generation_class__)
         if generation_config is None:
             generation_config = {k: v for k, v in attrs.items() if k in _generation_cl_dict}
         else:
-            generation_keys = {k for k in attrs if k in _generation_cl_dict}
-            if len(generation_keys) > 0:
-                logger.warning(
-                    "Both 'generation_config' and keys for 'generation_config' are passed."
-                    " The following keys in 'generation_config' will be overriden be keywords argument: %s",
-                    ", ".join(generation_keys),
-                )
-                config_merger.merge(generation_config, {k: v for k, v in attrs.items() if k in generation_keys})
+            config_merger.merge(generation_config, {k: v for k, v in attrs.items() if k in _generation_cl_dict})
 
         for k in _cached_keys:
             if k in generation_config or attrs.get(k) is None:
                 del attrs[k]
         _cached_keys = tuple(k for k in _cached_keys if k in attrs)
 
         self.__openllm_extras__ = first_not_none(__openllm_extras__, default={})
@@ -926,27 +1050,52 @@
                 "Creating %s with the following attributes: %s, generation_config=%s",
                 self.__class__.__name__,
                 _cached_keys,
                 generation_config,
             )
 
         # The rest of attrs should only be the attributes to be passed to __attrs_init__
-        self.__attrs_init__(generation_config=self.__openllm_generation_class__(**generation_config), **attrs)
+        self.__attrs_init__(generation_config=self["generation_class"](**generation_config), **attrs)
 
-    def __getattribute__(self, item: str) -> t.Any:
+    def __getitem__(self, item: str | t.Any) -> t.Any:
+        """Allowing access LLMConfig as a dictionary. The order will always evaluate as
+
+        __openllm_*__ > self.key > __openllm_generation_class__ > __openllm_extras__
+
+        This method is purely for convenience, and should not be used for performance critical code.
+        """
+        if not isinstance(item, str):
+            raise TypeError(f"LLM only supports string indexing, not {item.__class__.__name__}")
         if item in _reserved_namespace:
             raise ForbiddenAttributeError(
                 f"'{item}' is a reserved namespace for {self.__class__} and should not be access nor modified."
             )
+        internal_attributes = f"__openllm_{item}__"
+        if hasattr(self, internal_attributes):
+            return getattr(self, internal_attributes)
+        elif hasattr(self, item):
+            return getattr(self, item)
+        elif hasattr(self.__openllm_generation_class__, item):
+            return getattr(self.__openllm_generation_class__, item)
+        elif item in self.__openllm_extras__:
+            return self.__openllm_extras__[item]
+        else:
+            raise KeyError(item)
+
+    def __getattribute__(self, item: str) -> t.Any:
+        if item in _reserved_namespace:
+            raise ForbiddenAttributeError(
+                f"'{item}' belongs to a private namespace for {self.__class__} and should not be access nor modified."
+            )
         return _object_getattribute.__get__(self)(item)
 
     @classmethod
     def check_if_gpu_is_available(cls, implementation: str | None = None, force: bool = False):
         if implementation is None:
-            implementation = cls.__openllm_env__.get_framework_env()
+            implementation = cls.__openllm_env__["framework_value"]
 
         try:
             if cls.__openllm_requires_gpu__ or force:
                 if implementation in ("tf", "flax") and len(tf.config.list_physical_devices("GPU")) == 0:
                     raise OpenLLMException("Required GPU for given model")
                 else:
                     if not torch.cuda.is_available():
@@ -960,32 +1109,30 @@
                 msg = "GPU is not available"
             else:
                 msg = f"{cls} only supports running with GPU (None available)."
             raise GpuNotAvailableError(msg) from None
 
     def model_dump(self, flatten: bool = False, **_: t.Any):
         dumped = bentoml_cattr.unstructure(self)
-        generation_config = bentoml_cattr.unstructure(self.generation_config)
-        if not flatten:
-            dumped["generation_config"] = generation_config
-        else:
+        if flatten:
+            generation_config = dumped.pop("generation_config")
             dumped.update(generation_config)
         return dumped
 
     def model_dump_json(self, **kwargs: t.Any):
         return orjson.dumps(self.model_dump(**kwargs))
 
     @classmethod
     def model_construct_env(cls, **attrs: t.Any) -> t.Self:
         """A helpers that respect configuration values that
         sets from environment variables for any given configuration class.
         """
         attrs = {k: v for k, v in attrs.items() if v is not None}
 
-        model_config = cls.__openllm_env__.model_config
+        model_config = cls.__openllm_env__.config
 
         env_json_string = os.environ.get(model_config, None)
 
         if env_json_string is not None:
             try:
                 config_from_env = orjson.loads(env_json_string)
             except orjson.JSONDecodeError as e:
@@ -1012,19 +1159,19 @@
 
     def model_validate_click(self, **attrs: t.Any) -> tuple[LLMConfig, DictStrAny]:
         """Parse given click attributes into a LLMConfig and return the remaining click attributes."""
         llm_config_attrs: DictStrAny = {"generation_config": {}}
         key_to_remove: ListStr = []
 
         for k, v in attrs.items():
-            if k.startswith(f"{self.__openllm_model_name__}_generation_"):
-                llm_config_attrs["generation_config"][k[len(self.__openllm_model_name__ + "_generation_") :]] = v
+            if k.startswith(f"{self['model_name']}_generation_"):
+                llm_config_attrs["generation_config"][k[len(self["model_name"] + "_generation_") :]] = v
                 key_to_remove.append(k)
-            elif k.startswith(f"{self.__openllm_model_name__}_"):
-                llm_config_attrs[k[len(self.__openllm_model_name__ + "_") :]] = v
+            elif k.startswith(f"{self['model_name']}_"):
+                llm_config_attrs[k[len(self["model_name"] + "_") :]] = v
                 key_to_remove.append(k)
 
         return self.model_construct_env(**llm_config_attrs), {k: v for k, v in attrs.items() if k not in key_to_remove}
 
     @t.overload
     def to_generation_config(self, return_as_dict: t.Literal[False] = ...) -> transformers.GenerationConfig:
         ...
```

### Comparing `openllm-0.1.5/src/openllm/_llm.py` & `openllm-0.1.6/src/openllm/_llm.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,36 +15,44 @@
 from __future__ import annotations
 
 import copy
 import functools
 import logging
 import os
 import re
+import subprocess
+import sys
 import types
 import typing as t
 from abc import ABC, abstractmethod
 
 import attr
 import bentoml
 import inflection
 import orjson
 from bentoml._internal.models.model import ModelSignature
 from bentoml._internal.types import ModelSignatureDict
 
 import openllm
 
 from .exceptions import ForbiddenAttributeError, OpenLLMException
-from .utils import ENV_VARS_TRUE_VALUES, LazyLoader, bentoml_cattr
+from .utils import (DEBUG, LazyLoader, ModelEnv, bentoml_cattr, first_not_none,
+                    get_debug_mode, is_bitsandbytes_available,
+                    is_torch_available, non_intrusive_setattr, pkg)
 
 if t.TYPE_CHECKING:
     import torch
     import transformers
     from bentoml._internal.runner.strategy import Strategy
 
+    from .models.auto.factory import _BaseAutoLLMClass
+
     class LLMRunner(bentoml.Runner):
+        __doc__: str
+        __module__: str
         llm: openllm.LLM[t.Any, t.Any]
         config: openllm.LLMConfig
         llm_type: str
         identifying_params: dict[str, t.Any]
 
         def __call__(self, *args: t.Any, **attrs: t.Any) -> t.Any:
             ...
@@ -52,25 +60,26 @@
 else:
     LLMRunner = bentoml.Runner
     transformers = LazyLoader("transformers", globals(), "transformers")
     torch = LazyLoader("torch", globals(), "torch")
 
 logger = logging.getLogger(__name__)
 
-# NOTE: `1-2` -> text-generation and text2text-generation
 FRAMEWORK_TO_AUTOCLASS_MAPPING = {
     "pt": ("AutoModelForCausalLM", "AutoModelForSeq2SeqLM"),
     "tf": ("TFAutoModelForCausalLM", "TFAutoModelForSeq2SeqLM"),
     "flax": ("FlaxAutoModelForCausalLM", "FlaxAutoModelForSeq2SeqLM"),
 }
 
 TOKENIZER_PREFIX = "_tokenizer_"
 
 
-def convert_transformers_model_name(name: str) -> str:
+def convert_transformers_model_name(name: str | None) -> str:
+    if name is None:
+        raise ValueError("'name' cannot be None")
     if os.path.exists(os.path.dirname(name)):
         name = os.path.basename(name)
         logger.debug("Given name is a path, only returning the basename %s")
         return name
     return re.sub("[^a-zA-Z0-9]+", "-", name)
 
 
@@ -122,54 +131,53 @@
         config, attrs = t.cast(
             "tuple[transformers.PretrainedConfig, dict[str, t.Any]]",
             transformers.AutoConfig.from_pretrained(
                 model_id, return_unused_kwargs=True, trust_remote_code=trust_remote_code, **hub_attrs, **copied_attrs
             ),
         )
 
+    # NOTE: `1-2` -> text-generation and text2text-generation
     if type(config) in transformers.MODEL_FOR_CAUSAL_LM_MAPPING:
         idx = 0
     elif type(config) in transformers.MODEL_FOR_SEQ_TO_SEQ_CAUSAL_LM_MAPPING:
         idx = 1
     else:
         raise OpenLLMException(f"Model type {type(config)} is not supported yet.")
 
+    tokenizer = transformers.AutoTokenizer.from_pretrained(
+        model_id,
+        config=config,
+        trust_remote_code=trust_remote_code,
+        **hub_attrs,
+        **tokenizer_kwds,
+    )
+
+    model = getattr(
+        transformers,
+        FRAMEWORK_TO_AUTOCLASS_MAPPING[_model_framework][idx],
+    ).from_pretrained(
+        model_id,
+        *model_args,
+        config=config,
+        trust_remote_code=trust_remote_code,
+        **hub_attrs,
+        **attrs,
+    )
+
     try:
-        return bentoml.transformers.save_model(
-            tag,
-            getattr(
-                transformers,
-                FRAMEWORK_TO_AUTOCLASS_MAPPING[_model_framework][idx],
-            ).from_pretrained(
-                model_id,
-                *model_args,
-                config=config,
-                trust_remote_code=trust_remote_code,
-                **hub_attrs,
-                **attrs,
-            ),
-            custom_objects={
-                "tokenizer": transformers.AutoTokenizer.from_pretrained(
-                    model_id,
-                    config=config,
-                    trust_remote_code=trust_remote_code,
-                    **hub_attrs,
-                    **tokenizer_kwds,
-                )
-            },
-        )
+        return bentoml.transformers.save_model(tag, model, custom_objects={"tokenizer": tokenizer})
     finally:
         import gc
 
         gc.collect()
 
         # NOTE: We need to free up the cache after importing the model
         # in the case where users first run openllm start without the model
         # available locally.
-        if openllm.utils.is_torch_available() and torch.cuda.is_available():
+        if is_torch_available() and torch.cuda.is_available():
             torch.cuda.empty_cache()
 
 
 _reserved_namespace = {"config_class", "model", "tokenizer", "import_kwargs"}
 
 
 class LLMInterface(ABC):
@@ -235,29 +243,14 @@
 
     def load_model(self, tag: bentoml.Tag, *args: t.Any, **attrs: t.Any) -> t.Any:
         """This function can be implemented to override th default load_model behaviour. See falcon for
         example implementation."""
         raise NotImplementedError
 
 
-def _default_post_init(self: LLM[t.Any, t.Any]):
-    # load_in_mha: Whether to apply BetterTransformer (or Torch MultiHeadAttention) during inference load.
-    #              See https://pytorch.org/blog/a-better-transformer-for-fast-transformer-encoder-inference/
-    #              for more information.
-    # NOTE: set a default variable to transform to BetterTransformer by default for inference
-    self.load_in_mha = (
-        os.environ.get(self.config_class.__openllm_env__.bettertransformer, str(False)).upper() in ENV_VARS_TRUE_VALUES
-    )
-    if self.config_class.__openllm_requires_gpu__:
-        # For all models that requires GPU, no need to offload it to BetterTransformer
-        # use bitsandbytes instead
-
-        self.load_in_mha = False
-
-
 _M = t.TypeVar("_M")
 _T = t.TypeVar("_T")
 
 
 @attr.define(slots=True, repr=False)
 class LLM(LLMInterface, t.Generic[_M, _T]):
     if t.TYPE_CHECKING:
@@ -265,22 +258,24 @@
         __llm_trust_remote_code__: bool
         __llm_implementation__: t.Literal["pt", "tf", "flax"]
         __llm_model__: _M | None
         __llm_tokenizer__: _T | None
         __llm_tag__: bentoml.Tag | None
         __llm_bentomodel__: bentoml.Model | None
 
-        __openllm_post_init__: t.Callable[[t.Self], None] | None
-        __openllm_custom_load__: t.Callable[[t.Self, t.Any, t.Any], None] | None
-        __openllm_custom_import_kwargs__: property | None
+        __llm_post_init__: t.Callable[[t.Self], None] | None
+        __llm_custom_load__: t.Callable[[t.Self, t.Any, t.Any], None] | None
+        __llm_init_kwargs__: property | None
 
         _model_args: tuple[t.Any, ...]
         _model_attrs: dict[str, t.Any]
         _tokenizer_attrs: dict[str, t.Any]
 
+        bettertransformer: bool
+
     def __init_subclass__(cls):
         cd = cls.__dict__
         prefix_class_name_config = cls.__name__
         if prefix_class_name_config.startswith("Flax"):
             implementation = "flax"
             prefix_class_name_config = prefix_class_name_config[4:]
         elif prefix_class_name_config.startswith("TF"):
@@ -298,59 +293,54 @@
                 logger.debug(f"Using config class {cd['config_class']} for {cls.__name__}.")
         else:
             if "config_class" not in cd:
                 raise RuntimeError(
                     "Missing required key 'config_class'. Make sure to define it within the LLM subclass."
                 )
 
-        if cls.llm_post_init is not LLMInterface.llm_post_init:
-            original_llm_post_init = cd["llm_post_init"]
-
-            def wrapped_llm_post_init(self: t.Self) -> None:
-                """We need to both initialize private attributes and call the user-defined model_post_init
-                method.
-                """
-                _default_post_init(self)
-                original_llm_post_init(self)
-
-            cls.llm_post_init = wrapped_llm_post_init
-        else:
-            setattr(cls, "llm_post_init", _default_post_init)
-
         if cls.import_model is LLMInterface.import_model:
             # using the default import model
             setattr(cls, "import_model", functools.partial(import_model, _model_framework=implementation))
         else:
-            logger.debug("Using custom 'import_model' for %s", cls.__name__)
+            logger.debug("Custom 'import_model' will be used when loading modelj %s", cls.__name__)
 
-        cls.__openllm_post_init__ = None if cls.llm_post_init is LLMInterface.llm_post_init else cls.llm_post_init
-        cls.__openllm_custom_load__ = None if cls.load_model is LLMInterface.load_model else cls.load_model
-        cls.__openllm_custom_import_kwargs__ = (
-            None if cls.import_kwargs is LLMInterface.import_kwargs else cls.import_kwargs
-        )
+        cls.__llm_post_init__ = None if cls.llm_post_init is LLMInterface.llm_post_init else cls.llm_post_init
+        cls.__llm_custom_load__ = None if cls.load_model is LLMInterface.load_model else cls.load_model
+        cls.__llm_init_kwargs__ = None if cls.import_kwargs is LLMInterface.import_kwargs else cls.import_kwargs
 
         for at in {"bentomodel", "tag", "model", "tokenizer"}:
             setattr(cls, f"__llm_{at}__", None)
 
     # The following is the similar interface to HuggingFace pretrained protocol.
     @classmethod
     def from_pretrained(
         cls,
         model_id: str | None = None,
         llm_config: openllm.LLMConfig | None = None,
         *args: t.Any,
+        quantize: t.Literal["int8", "int4", "gptq"] | None = None,
+        bettertransformer: bool | None = None,
         **attrs: t.Any,
     ) -> LLM[_M, _T]:
-        return cls(model_id=model_id, llm_config=llm_config, *args, **attrs)
+        return cls(
+            model_id=model_id,
+            llm_config=llm_config,
+            *args,
+            quantize=quantize,
+            bettertransformer=bettertransformer,
+            **attrs,
+        )
 
     def __init__(
         self,
         model_id: str | None = None,
         llm_config: openllm.LLMConfig | None = None,
         *args: t.Any,
+        quantize: t.Literal["int8", "int4", "gptq"] | None = None,
+        bettertransformer: bool | None = None,
         **attrs: t.Any,
     ):
         """Initialize the LLM with given pretrained model.
 
         Note:
         - *args to be passed to the model.
         - **attrs will first be parsed to the AutoConfig, then the rest will be parsed to the import_model
@@ -419,71 +409,167 @@
             return transformers.pipeline("text-generation", model=model, tokenizer=_ref.custom_objects["tokenizer"])
         ```
 
         Args:
             model_id: The pretrained model to use. Defaults to None. If None, 'self.default_id' will be used.
             llm_config: The config to use for this LLM. Defaults to None. If not passed, OpenLLM
                         will use `config_class` to construct default configuration.
+            quantize: The quantization to use for this LLM. Defaults to None. Possible values
+                      include int8, int4 and gptq.
+            bettertransformer: Whether to use BetterTransformer with this model. Defaults to False.
             *args: The args to be passed to the model.
             **attrs: The kwargs to be passed to the model.
 
         The following are optional:
             openllm_model_version: version for this `model_id`. By default, users can ignore this if using pretrained
                                    weights as OpenLLM will use the commit_hash of given model_id.
                                    However, if `model_id` is a path, this argument is recomended to include.
         """
 
-        load_in_mha = attrs.pop("load_in_mha", False)
         openllm_model_version = attrs.pop("openllm_model_version", None)
 
+        # low_cpu_mem_usage is only available for model
+        # this is helpful on system with low memory to avoid OOM
+        low_cpu_mem_usage = attrs.pop("low_cpu_mem_usage", True)
+
+        # quantization setup
+        quantization_config = attrs.pop("quantization_config", None)
+        # 8 bit configuration
+        int8_threshold = attrs.pop("llm_int8_threshhold", 6.0)
+        cpu_offloading = attrs.pop("llm_int8_enable_fp32_cpu_offload", False)
+        int8_skip_modules: list[str] | None = attrs.pop("llm_int8_skip_modules", None)
+        int8_has_fp16_weight = attrs.pop("llm_int8_has_fp16_weight", False)
+        # 4 bit configuration
+        int4_compute_dtype = attrs.pop("llm_bnb_4bit_compute_dtype", torch.bfloat16)
+        int4_quant_type = attrs.pop("llm_bnb_4bit_quant_type", "nf4")
+        int4_use_double_quant = attrs.pop("llm_bnb_4bit_use_double_quant", True)
+
         if llm_config is not None:
-            logger.debug("Using given 'llm_config=(%s)' to initialize LLM", llm_config)
+            logger.debug("Using given 'llm_config=(%s)' to initialize LLM.", llm_config)
             self.config = llm_config
         else:
-            self.config = self.config_class(**attrs)
+            self.config = self.config_class.model_construct_env(**attrs)
             # The rests of the kwargs that is not used by the config class should be stored into __openllm_extras__.
-            attrs = self.config.__openllm_extras__
+            attrs = self.config["extras"]
+
+        if quantization_config and quantize:
+            raise ValueError(
+                """'quantization_config' and 'quantize' are mutually exclusive. Either customise
+            your quantization_config or use the quantize argument."""
+            )
+        if quantization_config is None:
+            # quantize is a openllm.LLM feature, where we can quantize the model
+            # with bitsandbytes or quantization aware training.
+            if quantize is not None:
+                if not is_bitsandbytes_available():
+                    raise RuntimeError(
+                        "Quantization requires bitsandbytes to be installed. Make "
+                        "sure to install OpenLLM with 'pip install \"openllm[fine-tune]\"'"
+                    )
+                logger.debug(
+                    "'quantize' is not None. %s will use a default 'quantization_config' for %s. "
+                    "If you want to customise the quantization config, make sure to pass your "
+                    "own 'quantization_config'",
+                    self,
+                    quantize,
+                )
+                if quantize == "int8":
+                    if int8_skip_modules is None:
+                        int8_skip_modules = []
+                    if "lm_head" not in int8_skip_modules and self.config["model_type"] == "causal_lm":
+                        logger.debug("Skipping 'lm_head' for quantization for %s", self)
+                        int8_skip_modules.append("lm_head")
+                    quantization_config = transformers.BitsAndBytesConfig(
+                        load_in_8bit=True,
+                        llm_int8_enable_fp32_cpu_offload=cpu_offloading,
+                        llm_int8_threshhold=int8_threshold,
+                        llm_int8_skip_modules=int8_skip_modules,
+                        llm_int8_has_fp16_weight=int8_has_fp16_weight,
+                    )
+                elif quantize == "int4":
+                    trf_versions = pkg.pkg_version_info("transformers")
+                    supports_kbits = trf_versions[:2] >= (4, 30)
+                    if supports_kbits:
+                        quantization_config = transformers.BitsAndBytesConfig(
+                            load_in_4bit=True,
+                            llm_bnb_4bit_compute_dtype=int4_compute_dtype,
+                            llm_bnb_4bit_quant_type=int4_quant_type,
+                            llm_bnb_4bit_use_double_quant=int4_use_double_quant,
+                        )
+                    else:
+                        logger.warning(
+                            "'quantize' is set to int4, while the current transformers version %s does not support "
+                            "k-bit quantization. k-bit quantization is supported since transformers 4.30, therefore "
+                            "make sure to install the latest version of transformers either via PyPI or "
+                            "from git source: 'pip install git+https://github.com/huggingface/transformers'.",
+                            trf_versions,
+                        )
+                elif quantize == "gptq":
+                    # TODO: support GPTQ loading quantization
+                    if model_id is None:
+                        raise RuntimeError(
+                            "'quantize=%s' requires passing custom path to quantized weights as we are unable to load "
+                            "the model on the fly. See https://github.com/qwopqwop200/GPTQ-for-LLaMa for "
+                            "instruction on how to quantize '%s' with GPTQ.",
+                            quantize,
+                            self,
+                        )
+                    raise NotImplementedError("GPTQ is not supported yet.")
+                else:
+                    raise ValueError(f"'quantize' must be one of ['int8', 'int4', 'gptq'], got {quantize} instead.")
+
+        if self.__llm_implementation__ == "pt":
+            if not self.config["use_pipeline"]:
+                attrs["low_cpu_mem_usage"] = low_cpu_mem_usage
+            attrs["quantization_config"] = quantization_config
+
+        model_kwds, tokenizer_kwds = {}, {}
+        if self.__llm_init_kwargs__:
+            if t.TYPE_CHECKING:
+                # the above meta value should determine that this LLM has custom kwargs
+                assert self.import_kwargs
+            model_kwds, tokenizer_kwds = self.import_kwargs
+            logger.debug(
+                "'%s' default kwargs for model: '%s', tokenizer: '%s'",
+                self.__class__.__name__,
+                model_kwds,
+                tokenizer_kwds,
+            )
 
         if model_id is None:
-            model_id = os.environ.get(self.config.__openllm_env__.model_id, self.config.__openllm_default_id__)
-            assert model_id is not None
+            model_id = os.environ.get(self.config["env"].model_id, self.config["default_id"])
 
         # NOTE: This is the actual given path or pretrained weight for this LLM.
+        assert model_id is not None
         self._model_id = model_id
 
         # parsing tokenizer and model kwargs
-        tokenizer_kwds = {k[len(TOKENIZER_PREFIX) :]: v for k, v in attrs.items() if k.startswith(TOKENIZER_PREFIX)}
-        for k in attrs:
-            if k in tokenizer_kwds:
-                del attrs[k]
-        # the rest of kwargs should be model kwargs
-        model_kwds = attrs
-
-        if self.import_kwargs:
-            _custom_model_kwds, _custom_tokenizer_kwds = self.import_kwargs
-            model_kwds.update(_custom_model_kwds)
-            tokenizer_kwds.update(_custom_tokenizer_kwds)
+        tokenizer_kwds.update(
+            {k[len(TOKENIZER_PREFIX) :]: v for k, v in attrs.items() if k.startswith(TOKENIZER_PREFIX)}
+        )
+        model_kwds.update({k: v for k, v in attrs.items() if not k.startswith(TOKENIZER_PREFIX)})
 
         # handle trust_remote_code
-        self.__llm_trust_remote_code__ = model_kwds.pop("trust_remote_code", self.config.__openllm_trust_remote_code__)
+        self.__llm_trust_remote_code__ = model_kwds.pop("trust_remote_code", self.config["trust_remote_code"])
 
         # NOTE: Save the args and kwargs for latter load
         self._model_args = args
         self._model_attrs = model_kwds
         self._tokenizer_attrs = tokenizer_kwds
+        self._openllm_model_version = openllm_model_version
 
-        if self.__openllm_post_init__:
+        if self.__llm_post_init__:
             self.llm_post_init()
 
-        # finally: we allow users to overwrite the load_in_mha defined by the LLM subclass.
-        if load_in_mha:
-            logger.debug("Overwriting 'load_in_mha=%s' (base load_in_mha=%s)", load_in_mha, self.load_in_mha)
-            self.load_in_mha = load_in_mha
-
-        self._openllm_model_version = openllm_model_version
+        # we set it here so that we allow subclass to overwrite bettertransformer in llm_post_init
+        if bettertransformer:
+            logger.debug("Using %r with BetterTransformer", self)
+            self.bettertransformer = bettertransformer
+        else:
+            non_intrusive_setattr(self, "bettertransformer", self.config["bettertransformer"])
 
     def __setattr__(self, attr: str, value: t.Any):
         if attr in _reserved_namespace:
             raise ForbiddenAttributeError(
                 f"{attr} should not be set during runtime "
                 f"as these value will be reflected during runtime. "
                 f"Instead, you can create a custom LLM subclass {self.__class__.__name__}."
@@ -497,123 +583,167 @@
 
     @property
     def model_id(self) -> str:
         return self._model_id
 
     @property
     def runner_name(self) -> str:
-        return f"llm-{self.config.__openllm_start_name__}-runner"
+        return f"llm-{self.config['start_name']}-runner"
 
     # NOTE: The section below defines a loose contract with langchain's LLM interface.
     @property
     def llm_type(self) -> str:
         return convert_transformers_model_name(self._model_id)
 
     @property
     def identifying_params(self) -> dict[str, t.Any]:
         return {
             "configuration": self.config.model_dump_json().decode(),
-            "model_ids": orjson.dumps(self.config.__openllm_model_ids__).decode(),
+            "model_ids": orjson.dumps(self.config["model_ids"]).decode(),
         }
 
-    def make_tag(self, model_id: str | None = None) -> bentoml.Tag:
+    @property
+    def llm_parameters(self) -> tuple[tuple[tuple[t.Any, ...], dict[str, t.Any]], dict[str, t.Any]]:
+        """Returning the processed model and tokenizer parameters to be used with
+        'import_model' or any other place that requires loading model and tokenizer.
+
+        See 'openllm.cli.download_models' for example usage.
+        It returns a tuple of (model_args, model_kwargs) & tokenizer_kwargs
+        """
+        return (self._model_args, self._model_attrs), self._tokenizer_attrs
+
+    @staticmethod
+    def make_tag(
+        model_id: str | None = None,
+        trust_remote_code: bool = False,
+        openllm_model_version: str | None = None,
+        implementation: t.Literal["pt", "flax", "tf"] = "pt",
+    ) -> bentoml.Tag:
         """Generate a ``bentoml.Tag`` from a given transformers model name.
 
         Note that this depends on your model to have a config class available.
 
         Args:
             model_id: The transformers model name or path to load the model from.
                       If it is a path, then `openllm_model_version` must be passed in as a kwarg.
             trust_remote_code: Whether to trust the remote code. Defaults to False.
-            **attrs: Additional kwargs to pass to the ``transformers.AutoConfig`` constructor.
-                    If your pass ``return_unused_kwargs=True``, it will be ignored.
+            openllm_model_version: Optional model version to be saved with this tag.
+            implementation: Given implementation for said LLM. One of t.Literal['pt', 'tf', 'flax']
 
         Returns:
             A tuple of ``bentoml.Tag`` and a dict of unused kwargs.
         """
-        if model_id is None:
-            model_id = self._model_id
         name = convert_transformers_model_name(model_id)
 
         config = t.cast(
             "transformers.PretrainedConfig",
-            transformers.AutoConfig.from_pretrained(model_id, trust_remote_code=self.__llm_trust_remote_code__),
+            transformers.AutoConfig.from_pretrained(
+                model_id,
+                trust_remote_code=trust_remote_code,
+            ),
         )
 
         model_version = getattr(config, "_commit_hash", None)
         if model_version is None:
-            if self._openllm_model_version is not None:
+            if openllm_model_version is not None:
                 logger.warning(
                     "Given %s from '%s' doesn't contain a commit hash, and 'openllm_model_version' is not given. "
                     "We will generate the tag without specific version.",
                     config.__class__,
                     model_id,
                 )
                 model_version = bentoml.Tag.from_taglike(name).make_new_version().version
             else:
-                logger.debug("Using %s for '%s' as model version", self._openllm_model_version, model_id)
-                model_version = self._openllm_model_version
+                logger.debug("Using %s for '%s' as model version", openllm_model_version, model_id)
+                model_version = openllm_model_version
 
-        return bentoml.Tag.from_taglike(f"{self.__llm_implementation__}-{name}:{model_version}")
+        return bentoml.Tag.from_taglike(f"{implementation}-{name}:{model_version}")
 
     def ensure_model_id_exists(self) -> bentoml.Model:
-        try:
-            return bentoml.transformers.get(self.tag)
-        except bentoml.exceptions.NotFound:
-            logger.info(
-                "'%s' with tag (%s) not found, importing from HuggingFace Hub.", self.__class__.__name__, self.tag
-            )
-            return self.import_model(
-                self._model_id,
-                self.tag,
-                *self._model_args,
-                tokenizer_kwds=self._tokenizer_attrs,
-                trust_remote_code=self.__llm_trust_remote_code__,
-                **self._model_attrs,
-            )
-        finally:
-            if openllm.utils.is_torch_available() and torch.cuda.is_available():
-                torch.cuda.empty_cache()
+        """This utility function will download the model if it doesn't exist yet.
+        Make sure to call this function if 'ensure_available' is not set during
+        Auto LLM initialisation.
+        """
+        output = subprocess.check_output(
+            [
+                sys.executable,
+                "-m",
+                "openllm",
+                "download",
+                self.config["start_name"],
+                "--model-id",
+                self.model_id,
+                "--output",
+                "porcelain",
+            ]
+        )
+        if DEBUG or get_debug_mode():
+            # NOTE: This usually only concern BentoML devs.
+            pattern = r"^__tag__:[^:\n]+:[^:\n]+"
+            matched = re.search(pattern, output.decode("utf-8").strip(), re.MULTILINE)
+            assert matched is not None, f"Failed to find tag from output: {output}"
+            _, _, tag = matched.group(0).partition(":")
+        else:
+            tag = output.strip().decode()
+
+        return bentoml.transformers.get(tag)
 
     @property
     def _bentomodel(self) -> bentoml.Model:
         if self.__llm_bentomodel__ is None:
-            self.__llm_bentomodel__ = self.ensure_model_id_exists()
+            # NOTE: Since PR#28, self.__llm_bentomodel__ changed from
+            # ensure_model_id_exists() into just returning the model ref.
+            # This is because we want to save a few seconds of loading time,
+            # as openllm.Runner and openllm.AutoLLM initialisation is around 700ms
+            # before #28.
+            # If users want to make sure to have the model downloaded,
+            # one should invoke `LLM.ensure_model_id_exists()` manually,
+            # or pass `ensure_available=True` into the Auto LLM initialisation.
+            self.__llm_bentomodel__ = bentoml.transformers.get(self.tag)
         return self.__llm_bentomodel__
 
     @property
     def tag(self) -> bentoml.Tag:
         if self.__llm_tag__ is None:
-            self.__llm_tag__ = self.make_tag()
+            self.__llm_tag__ = self.make_tag(
+                self._model_id,
+                self.__llm_trust_remote_code__,
+                self._openllm_model_version,
+                self.__llm_implementation__,
+            )
         return self.__llm_tag__
 
     @property
     def model(self) -> _M:
         """The model to use for this LLM. This shouldn't be set at runtime, rather let OpenLLM handle it."""
         # Run check for GPU
         self.config.check_if_gpu_is_available(implementation=self.__llm_implementation__)
 
         kwds = self._model_attrs
         kwds["trust_remote_code"] = self.__llm_trust_remote_code__
 
-        if self.load_in_mha and "_pretrained_class" not in self._bentomodel.info.metadata:
+        is_pipeline = "_pretrained_class" in self._bentomodel.info.metadata
+        # differentiate when saving tokenizer or other pretrained type.
+        is_pretrained_model = is_pipeline and "_framework" in self._bentomodel.info.metadata
+
+        if self.bettertransformer and is_pipeline and self.config["use_pipeline"]:
             # This is a pipeline, provide a accelerator args
             kwds["accelerator"] = "bettertransformer"
 
         if self.__llm_model__ is None:
-            if self.__openllm_custom_load__:
+            if self.__llm_custom_load__:
                 self.__llm_model__ = self.load_model(self.tag, *self._model_args, **kwds)
             else:
                 self.__llm_model__ = self._bentomodel.load_model(*self._model_args, **kwds)
 
-            # TODO: self.config.__openllm_runtime__: t.Literal['python', 'cpp']
             if (
-                self.load_in_mha
-                and all(i in self._bentomodel.info.metadata for i in ("_framework", "_pretrained_class"))
+                self.bettertransformer
+                and is_pretrained_model
                 and self._bentomodel.info.metadata["_framework"] == "torch"
+                and self.config["runtime"] == "transformers"
             ):
                 # BetterTransformer is currently only supported on PyTorch.
                 from optimum.bettertransformer import BetterTransformer
 
                 self.__llm_model__ = BetterTransformer.transform(self.__llm_model__)
         return t.cast(_M, self.__llm_model__)
 
@@ -628,21 +758,22 @@
                 raise openllm.exceptions.OpenLLMException(
                     "Model does not have tokenizer. Make sure to save \
                     the tokenizer within the model via 'custom_objects'.\
                     For example: bentoml.transformers.save_model(..., custom_objects={'tokenizer': tokenizer}))"
                 )
         return self.__llm_tokenizer__
 
+    # order of these fields matter here, make sure to sync it with
+    # openllm.models.auto.factory._BaseAutoLLMClass.for_model
     def to_runner(
         self,
         models: list[bentoml.Model] | None = None,
         max_batch_size: int | None = None,
         max_latency_ms: int | None = None,
         method_configs: dict[str, ModelSignatureDict | ModelSignature] | None = None,
-        embedded: bool = False,
         scheduling_strategy: type[Strategy] | None = None,
     ) -> LLMRunner:
         """Convert this LLM into a Runner.
 
         Args:
             models: Any additional ``bentoml.Model`` to be included in this given models.
                     By default, this will be determined from the model_name.
@@ -652,32 +783,32 @@
             strategy: The strategy to use for this runner.
             embedded: Whether to run this runner in embedded mode.
             scheduling_strategy: Whether to create a custom scheduling strategy for this Runner.
 
         NOTE: There are some difference between bentoml.models.get().to_runner() and LLM.to_runner(): 'name'.
         - 'name': will be generated by OpenLLM, hence users don't shouldn't worry about this.
             The generated name will be 'llm-<model-start-name>-runner' (ex: llm-dolly-v2-runner, llm-chatglm-runner)
+        - 'embedded': Will be disabled by default. There is no reason to run LLM in embedded mode.
         """
         models = models if models is not None else []
         models.append(self._bentomodel)
 
         if scheduling_strategy is None:
             from bentoml._internal.runner.strategy import DefaultStrategy
 
             scheduling_strategy = DefaultStrategy
 
         generate_sig = ModelSignature.from_dict(ModelSignatureDict(batchable=False))
         generate_iterator_sig = ModelSignature.from_dict(ModelSignatureDict(batchable=True))
         if method_configs is None:
             method_configs = {"generate": generate_sig, "generate_iterator": generate_iterator_sig}
         else:
-            generate_sig = ModelSignature.convert_signatures_dict(method_configs).get("generate", generate_sig)
-            generate_iterator_sig = ModelSignature.convert_signatures_dict(method_configs).get(
-                "generate_iterator", generate_iterator_sig
-            )
+            signatures = ModelSignature.convert_signatures_dict(method_configs)
+            generate_sig = first_not_none(signatures.get("generate"), default=generate_sig)
+            generate_iterator_sig = first_not_none(signatures.get("generate_iterator"), default=generate_iterator_sig)
 
         class _Runnable(bentoml.Runnable):
             SUPPORTED_RESOURCES = ("nvidia.com/gpu", "cpu")
             SUPPORTS_CPU_MULTI_THREADING = True
 
             llm_type: str
             identifying_params: dict[str, t.Any]
@@ -732,45 +863,45 @@
             """
             prompt, generate_kwargs, postprocess_kwargs = self.sanitize_parameters(prompt, **kwargs)
             generated_result = __self.generate.run(prompt, **generate_kwargs)
             return self.postprocess_generate(prompt, generated_result, **postprocess_kwargs)
 
         # NOTE: returning the two langchain API's to the runner
         return types.new_class(
-            inflection.camelize(self.config.__openllm_model_name__) + "Runner",
+            inflection.camelize(self.config["model_name"]) + "Runner",
             (bentoml.Runner,),
             exec_body=lambda ns: ns.update(
                 {
                     "llm_type": self.llm_type,
                     "identifying_params": self.identifying_params,
                     "llm": self,  # NOTE: self reference to LLM
                     "config": self.config,
                     "__call__": _wrapped_generate_run,
-                    "__module__": f"openllm.models.{self.config.__openllm_model_name__}",
-                    "__doc__": self.config.__openllm_env__.start_docstring,
+                    "__module__": f"openllm.models.{self.config['model_name']}",
+                    "__doc__": self.config["env"].start_docstring,
                 }
             ),
         )(
             types.new_class(
-                inflection.camelize(self.config.__openllm_model_name__) + "Runnable",
+                inflection.camelize(self.config["model_name"]) + "Runnable",
                 (_Runnable,),
                 {
                     "SUPPORTED_RESOURCES": ("nvidia.com/gpu", "cpu")
-                    if self.config.__openllm_requires_gpu__
+                    if self.config["requires_gpu"]
                     else ("nvidia.com/gpu",),
                     "llm_type": self.llm_type,
                     "identifying_params": self.identifying_params,
                 },
             ),
             name=self.runner_name,
+            embedded=False,
             models=models,
             max_batch_size=max_batch_size,
             max_latency_ms=max_latency_ms,
             method_configs=bentoml_cattr.unstructure(method_configs),
-            embedded=embedded,
             scheduling_strategy=scheduling_strategy,
         )
 
     def predict(self, prompt: str, **attrs: t.Any) -> t.Any:
         """The scikit-compatible API for self(...)"""
         return self.__call__(prompt, **attrs)
 
@@ -816,28 +947,34 @@
     embedded: t.Literal[True, False] = ...,
     scheduling_strategy: type[Strategy] | None = ...,
     **attrs: t.Any,
 ) -> LLMRunner:
     ...
 
 
-def Runner(model_name: str, **attrs: t.Any) -> LLMRunner:
+def Runner(model_name: str, ensure_available: bool = True, init_local: bool = False, **attrs: t.Any) -> LLMRunner:
     """Create a Runner for given LLM. For a list of currently supported LLM, check out 'openllm models'
 
     Args:
         model_name: Supported model name from 'openllm models'
+        ensure_available: If True, it will ensure the model is available before creating the runner.
+                          Set to False for faster creation time. Note that you will need to make sure
+                          the model for this 'model_id' is available before calling the runner.
+                          One can do this by doing the following:
+                          ```python
+                          runner = openllm.Runner("dolly-v2", ensure_available=False)
+                          runner.llm.ensure_model_id_exists()
+                          ```
+        init_local: If True, it will initialize the model locally. This is useful if you want to
+                    run the model locally. (Symmetrical to bentoml.Runner.init_local())
         **attrs: The rest of kwargs will then be passed to the LLM. Refer to the LLM documentation for the kwargs
                 behaviour
     """
-    init_local = attrs.pop("init_local", False)
-    ModelEnv = openllm.utils.ModelEnv(model_name)
-    if ModelEnv.get_framework_env() == "flax":
-        runner = openllm.AutoFlaxLLM.create_runner(model_name, **attrs)
-    elif ModelEnv.get_framework_env() == "tf":
-        runner = openllm.AutoTFLLM.create_runner(model_name, **attrs)
-    else:
-        runner = openllm.AutoLLM.create_runner(model_name, **attrs)
+    runner = t.cast(
+        "_BaseAutoLLMClass",
+        openllm[ModelEnv(model_name)["framework_value"]],  # type: ignore (internal API)
+    ).create_runner(model_name, ensure_available=ensure_available, **attrs)
 
     if init_local:
         runner.init_local(quiet=True)
 
     return runner
```

### Comparing `openllm-0.1.5/src/openllm/_package.py` & `openllm-0.1.6/src/openllm/_package.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,20 +25,23 @@
 import bentoml
 import fs
 import inflection
 from bentoml._internal.bento.build_config import DockerOptions, PythonOptions
 from bentoml._internal.configuration import get_debug_mode
 
 import openllm
-import openllm.utils as utils
-from openllm.utils import pkg
+
+from .utils import (ModelEnv, codegen, first_not_none, is_flax_available,
+                    is_tf_available, is_torch_available, pkg)
 
 if t.TYPE_CHECKING:
     from fs.base import FS
 
+    from .models.auto.factory import _BaseAutoLLMClass
+
 logger = logging.getLogger(__name__)
 
 OPENLLM_DEV_BUILD = "OPENLLM_DEV_BUILD"
 
 
 def build_editable(path: str) -> str | None:
     """Build OpenLLM if the OPENLLM_DEV_BUILD environment variable is set."""
@@ -72,36 +75,33 @@
 def construct_python_options(llm: openllm.LLM[t.Any, t.Any], llm_fs: FS) -> PythonOptions:
     # NOTE: add openllm to the default dependencies
     # if users has openllm custom built wheels, it will still respect
     # that since bentoml will always install dependencies from requirements.txt
     # first, then proceed to install everything inside the wheels/ folder.
     packages: list[str] = ["openllm"]
 
-    if llm.config.__openllm_requirements__ is not None:
-        packages.extend(llm.config.__openllm_requirements__)
+    if llm.config["requirements"] is not None:
+        packages.extend(llm.config["requirements"])
 
     if not (str(os.environ.get("BENTOML_BUNDLE_LOCAL_BUILD", False)).lower() == "false"):
         packages.append(f"bentoml>={'.'.join([str(i) for i in pkg.pkg_version_info('bentoml')])}")
 
-    to_use_framework = llm.config.__openllm_env__.get_framework_env()
-    if to_use_framework == "flax":
-        assert (
-            utils.is_flax_available()
-        ), f"Flax is not available, while {llm.config.__openllm_env__.framework} is set to 'flax'"
+    env: ModelEnv = llm.config["env"]
+    framework_envvar = env["framework_value"]
+    if framework_envvar == "flax":
+        assert is_flax_available(), f"Flax is not available, while {env.framework} is set to 'flax'"
         packages.extend(
             [
                 f"flax>={importlib.metadata.version('flax')}",
                 f"jax>={importlib.metadata.version('jax')}",
                 f"jaxlib>={importlib.metadata.version('jaxlib')}",
             ]
         )
-    elif to_use_framework == "tf":
-        assert (
-            utils.is_tf_available()
-        ), f"TensorFlow is not available, while {llm.config.__openllm_env__.framework} is set to 'tf'"
+    elif framework_envvar == "tf":
+        assert is_tf_available(), f"TensorFlow is not available, while {env.framework} is set to 'tf'"
         candidates = (
             "tensorflow",
             "tensorflow-cpu",
             "tensorflow-gpu",
             "tf-nightly",
             "tf-nightly-cpu",
             "tf-nightly-gpu",
@@ -115,123 +115,207 @@
             try:
                 _tf_version = importlib.metadata.version(candidate)
                 packages.extend([f"tensorflow>={_tf_version}"])
                 break
             except importlib.metadata.PackageNotFoundError:
                 pass
     else:
-        assert utils.is_torch_available(), "PyTorch is not available. Make sure to have it locally installed."
+        assert is_torch_available(), "PyTorch is not available. Make sure to have it locally installed."
         packages.extend([f"torch>={importlib.metadata.version('torch')}"])
 
     wheels: list[str] = []
     built_wheels = build_editable(llm_fs.getsyspath("/"))
     if built_wheels is not None:
         wheels.append(llm_fs.getsyspath(f"/{built_wheels.split('/')[-1]}"))
 
     return PythonOptions(packages=packages, wheels=wheels, lock_packages=True)
 
 
-def construct_docker_options(llm: openllm.LLM[t.Any, t.Any], _: FS, workers_per_resource: int | float) -> DockerOptions:
+def construct_docker_options(
+    llm: openllm.LLM[t.Any, t.Any],
+    _: FS,
+    workers_per_resource: int | float,
+    quantize: t.LiteralString | None,
+    bettertransformer: bool | None,
+) -> DockerOptions:
     _bentoml_config_options = os.environ.pop("BENTOML_CONFIG_OPTIONS", "")
     _bentoml_config_options_opts = [
-        "api_server.traffic.timeout=3600",  # NOTE: Currently we hardcode this value
-        f'runners."llm-{llm.config.__openllm_start_name__}-runner".traffic.timeout={llm.config.__openllm_timeout__}',
-        f'runners."llm-{llm.config.__openllm_start_name__}-runner".workers_per_resource={workers_per_resource}',
+        "api_server.traffic.timeout=36000",  # NOTE: Currently we hardcode this value
+        f'runners."llm-{llm.config["start_name"]}-runner".traffic.timeout={llm.config["timeout"]}',
+        f'runners."llm-{llm.config["start_name"]}-runner".workers_per_resource={workers_per_resource}',
     ]
     _bentoml_config_options += " " if _bentoml_config_options else "" + " ".join(_bentoml_config_options_opts)
-    return DockerOptions(
-        cuda_version="11.6",  # NOTE: Torch 2.0 currently only support 11.6 as the latest CUDA version
-        env={
-            llm.config.__openllm_env__.framework: llm.config.__openllm_env__.get_framework_env(),
-            "OPENLLM_MODEL": llm.config.__openllm_model_name__,
-            "OPENLLM_MODEL_ID": llm.model_id,
-            "BENTOML_DEBUG": str(get_debug_mode()),
-            "BENTOML_CONFIG_OPTIONS": _bentoml_config_options,
-        },
-        system_packages=["git"],
-    )
+    env: ModelEnv = llm.config["env"]
+
+    env_dict = {
+        env.framework: env.framework_value,
+        env.config: llm.config.model_dump_json().decode(),
+        "OPENLLM_MODEL": llm.config["model_name"],
+        "OPENLLM_MODEL_ID": llm.model_id,
+        "BENTOML_DEBUG": str(get_debug_mode()),
+        "BENTOML_CONFIG_OPTIONS": _bentoml_config_options,
+    }
+
+    # We need to handle None separately here, as env from subprocess doesn't
+    # accept None value.
+    _env = ModelEnv(llm.config["model_name"], bettertransformer=bettertransformer, quantize=quantize)
+
+    if _env.bettertransformer_value is not None:
+        env_dict[_env.bettertransformer] = _env.bettertransformer_value
+    if _env.quantize_value is not None:
+        env_dict[_env.quantize] = _env.quantize_value
+
+    # NOTE: Torch 2.0 currently only support 11.6 as the latest CUDA version
+    return DockerOptions(cuda_version="11.6", env=env_dict, system_packages=["git"])
 
 
 @t.overload
-def build(model_name: str, *, __cli__: t.Literal[False] = ..., **attrs: t.Any) -> bentoml.Bento:
+def build(
+    model_name: str,
+    *,
+    model_id: str | None = ...,
+    quantize: t.LiteralString | None = ...,
+    bettertransformer: bool | None = ...,
+    _workers_per_resource: int | float | None = ...,
+    _overwrite_existing_bento: bool = ...,
+    __cli__: t.Literal[False] = ...,
+    **attrs: t.Any,
+) -> bentoml.Bento:
     ...
 
 
 @t.overload
-def build(model_name: str, *, __cli__: t.Literal[True] = ..., **attrs: t.Any) -> tuple[bentoml.Bento, bool]:
+def build(
+    model_name: str,
+    *,
+    model_id: str | None = ...,
+    quantize: t.LiteralString | None = ...,
+    bettertransformer: bool | None = ...,
+    _workers_per_resource: int | float | None = ...,
+    _overwrite_existing_bento: bool = ...,
+    __cli__: t.Literal[True] = ...,
+    **attrs: t.Any,
+) -> tuple[bentoml.Bento, bool]:
     ...
 
 
-def build(model_name: str, *, __cli__: bool = False, **attrs: t.Any) -> tuple[bentoml.Bento, bool] | bentoml.Bento:
-    """Package a LLM into a Bento."""
+def _build_bento(
+    bento_tag: bentoml.Tag,
+    service_name: str,
+    llm_fs: FS,
+    llm: openllm.LLM[t.Any, t.Any],
+    workers_per_resource: int | float,
+    quantize: t.LiteralString | None,
+    bettertransformer: bool | None,
+) -> bentoml.Bento:
+    framework_envvar = llm.config["env"]["framework_value"]
+    labels = dict(llm.identifying_params)
+    labels.update({"_type": llm.llm_type, "_framework": framework_envvar})
+    logger.info("Building Bento for LLM '%s'", llm.config["start_name"])
+    return bentoml.bentos.build(
+        f"{service_name}:svc",
+        name=bento_tag.name,
+        labels=labels,
+        description=f"OpenLLM service for {llm.config['start_name']}",
+        include=[
+            f for f in llm_fs.walk.files(filter=["*.py"])
+        ],  # NOTE: By default, we are using _service.py as the default service, for now.
+        exclude=["/venv", "__pycache__/", "*.py[cod]", "*$py.class"],
+        python=construct_python_options(llm, llm_fs),
+        docker=construct_docker_options(llm, llm_fs, workers_per_resource, quantize, bettertransformer),
+        version=bento_tag.version,
+        build_ctx=llm_fs.getsyspath("/"),
+    )
+
 
-    overwrite_existing_bento = attrs.pop("_overwrite_existing_bento", False)
+def build(
+    model_name: str,
+    *,
+    model_id: str | None = None,
+    quantize: t.LiteralString | None = None,
+    bettertransformer: bool | None = None,
+    _workers_per_resource: int | float | None = None,
+    _overwrite_existing_bento: bool = False,
+    __cli__: bool = False,
+    **attrs: t.Any,
+) -> tuple[bentoml.Bento, bool] | bentoml.Bento:
+    """Package a LLM into a Bento.
+
+    The LLM will be built into a BentoService with the following structure:
+    if quantize is passed, it will instruct the model to be quantized dynamically during serving time.
+    if bettertransformer is passed, it will instruct the model to use BetterTransformer during serving time.
+
+    Other parameters including model_name, model_id and attrs will be passed to the LLM class itself.
+    """
+
+    _previously_built = False
     current_model_envvar = os.environ.pop("OPENLLM_MODEL", None)
     current_model_id_envvar = os.environ.pop("OPENLLM_MODEL_ID", None)
-    _previously_built = False
-    workers_per_resource = attrs.pop("_workers_per_resource", None)
-    model_id: str = attrs.pop("model_id", None)
 
     llm_config = openllm.AutoConfig.for_model(model_name)
 
     logger.info("Packing '%s' into a Bento with kwargs=%s...", model_name, attrs)
 
     # NOTE: We set this environment variable so that our service.py logic won't raise RuntimeError
     # during build. This is a current limitation of bentoml build where we actually import the service.py into sys.path
     try:
         os.environ["OPENLLM_MODEL"] = inflection.underscore(model_name)
 
-        to_use_framework = llm_config.__openllm_env__.get_framework_env()
-        if to_use_framework == "flax":
-            llm = openllm.AutoFlaxLLM.for_model(model_name, model_id=model_id, llm_config=llm_config, **attrs)
-        elif to_use_framework == "tf":
-            llm = openllm.AutoTFLLM.for_model(model_name, model_id=model_id, llm_config=llm_config, **attrs)
-        else:
-            llm = openllm.AutoLLM.for_model(model_name, model_id=model_id, llm_config=llm_config, **attrs)
+        framework_envvar = llm_config["env"]["framework_value"]
+        llm = t.cast(
+            "_BaseAutoLLMClass",
+            openllm[framework_envvar],  # type: ignore (internal API)
+        ).for_model(
+            model_name,
+            model_id=model_id,
+            llm_config=llm_config,
+            quantize=quantize,
+            bettertransformer=bettertransformer,
+            **attrs,
+        )
 
         os.environ["OPENLLM_MODEL_ID"] = llm.model_id
 
         labels = dict(llm.identifying_params)
-        labels.update({"_type": llm.llm_type, "_framework": to_use_framework})
-        service_name = f"generated_{llm.config.__openllm_model_name__}_service.py"
-        workers_per_resource = utils.first_not_none(
-            workers_per_resource, default=llm.config.__openllm_workers_per_resource__
-        )
+        labels.update({"_type": llm.llm_type, "_framework": framework_envvar})
+        service_name = f"generated_{llm_config['model_name']}_service.py"
+        workers_per_resource = first_not_none(_workers_per_resource, default=llm_config["workers_per_resource"])
 
-        with fs.open_fs(f"temp://llm_{llm.config.__openllm_model_name__}") as llm_fs:
+        with fs.open_fs(f"temp://llm_{llm_config['model_name']}") as llm_fs:
             # add service.py definition to this temporary folder
-            utils.codegen.write_service(model_name, llm.model_id, service_name, llm_fs)
+            codegen.write_service(model_name, llm.model_id, service_name, llm_fs)
 
             bento_tag = bentoml.Tag.from_taglike(f"{llm.llm_type}-service:{llm.tag.version}")
             try:
                 bento = bentoml.get(bento_tag)
-                if overwrite_existing_bento:
+                if _overwrite_existing_bento:
+                    logger.info("Overwriting previously saved Bento.")
                     bentoml.delete(bento_tag)
-                    raise bentoml.exceptions.NotFound("Overwriting previously saved Bento.")
+                    bento = _build_bento(
+                        bento_tag,
+                        service_name,
+                        llm_fs,
+                        llm,
+                        workers_per_resource=workers_per_resource,
+                        quantize=quantize,
+                        bettertransformer=bettertransformer,
+                    )
                 _previously_built = True
             except bentoml.exceptions.NotFound:
-                logger.info("Building Bento for LLM '%s'", llm.config.__openllm_start_name__)
-                bento = bentoml.bentos.build(
-                    f"{service_name}:svc",
-                    name=bento_tag.name,
-                    labels=labels,
-                    description=f"OpenLLM service for {llm.config.__openllm_start_name__}",
-                    include=[
-                        f for f in llm_fs.walk.files(filter=["*.py"])
-                    ],  # NOTE: By default, we are using _service.py as the default service, for now.
-                    exclude=["/venv", "__pycache__/", "*.py[cod]", "*$py.class"],
-                    python=construct_python_options(llm, llm_fs),
-                    docker=construct_docker_options(llm, llm_fs, workers_per_resource),
-                    version=bento_tag.version,
-                    build_ctx=llm_fs.getsyspath("/"),
+                logger.info("Building Bento for LLM '%s'", llm_config["start_name"])
+                bento = _build_bento(
+                    bento_tag,
+                    service_name,
+                    llm_fs,
+                    llm,
+                    workers_per_resource=workers_per_resource,
+                    quantize=quantize,
+                    bettertransformer=bettertransformer,
                 )
-            if __cli__:
-                return bento, _previously_built
-            else:
-                return bento
+            return (bento, _previously_built) if __cli__ else bento
     except Exception as e:
         logger.error("\nException caught during building LLM %s: \n", model_name, exc_info=e)
         raise
     finally:
         del os.environ["OPENLLM_MODEL"]
         del os.environ["OPENLLM_MODEL_ID"]
         # restore original OPENLLM_MODEL envvar if set.
```

### Comparing `openllm-0.1.5/src/openllm/_prompt.py` & `openllm-0.1.6/src/openllm/_prompt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/src/openllm/_schema.py` & `openllm-0.1.6/src/openllm/_schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         else:
             raise RuntimeError(f"Type {type(data)} is not yet supported.")
 
     @classmethod
     def for_model(cls, model_name: str, **attrs: t.Any) -> type[GenerationInput]:
         llm_config = openllm.AutoConfig.for_model(model_name, **attrs)
         return attr.make_class(
-            inflection.camelize(llm_config.__openllm_model_name__) + "GenerationInput",
+            inflection.camelize(llm_config["model_name"]) + "GenerationInput",
             attrs={
                 "prompt": attr.field(type=str),
                 "llm_config": attr.field(
                     type=llm_config.__class__,
                     default=llm_config,
                     converter=functools.partial(cls.convert_llm_config, cls=llm_config.__class__),
                 ),
```

### Comparing `openllm-0.1.5/src/openllm/_service.py` & `openllm-0.1.6/src/openllm/_service.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,33 +30,42 @@
 
 import openllm
 
 model = os.environ.get("OPENLLM_MODEL", "{__model_name__}")  # openllm: model name
 model_id = os.environ.get("OPENLLM_MODEL_ID", "{__model_id__}")  # openllm: model id
 
 llm_config = openllm.AutoConfig.for_model(model)
-runner = openllm.Runner(model, model_id=model_id, llm_config=llm_config)
 
-svc = bentoml.Service(name=f"llm-{llm_config.__openllm_start_name__}-service", runners=[runner])
+runner = openllm.Runner(
+    model,
+    model_id=model_id,
+    llm_config=llm_config,
+    bettertransformer=llm_config["env"]["bettertransformer_value"],
+    quantize=llm_config["env"]["quantize_value"],
+    ensure_available=False,
+    init_local=False,
+)
+
+svc = bentoml.Service(name=f"llm-{llm_config['start_name']}-service", runners=[runner])
 
 
 @svc.api(
-    input=bentoml.io.JSON.from_sample(sample={"prompt": "", "llm_config": llm_config.model_dump()}),
-    output=bentoml.io.JSON.from_sample(sample={"responses": [], "configuration": llm_config.model_dump()}),
+    input=bentoml.io.JSON.from_sample(sample={"prompt": "", "llm_config": llm_config.model_dump(flatten=True)}),
+    output=bentoml.io.JSON.from_sample(sample={"responses": [], "configuration": llm_config.model_dump(flatten=True)}),
     route="/v1/generate",
 )
 async def generate_v1(input_dict: dict[str, t.Any]) -> openllm.GenerationOutput:
     qa_inputs = openllm.GenerationInput.for_model(model)(**input_dict)
     config = qa_inputs.llm_config.model_dump()
     responses = await runner.generate.async_run(qa_inputs.prompt, **config)
     return openllm.GenerationOutput(responses=responses, configuration=config)
 
 
 @svc.api(input=bentoml.io.Text(), output=bentoml.io.JSON(), route="/v1/metadata")
 def metadata_v1(_: str) -> openllm.MetadataOutput:
     return openllm.MetadataOutput(
         model_id=model_id,
-        timeout=llm_config.__openllm_timeout__,
-        model_name=llm_config.__openllm_model_name__,
-        framework=llm_config.__openllm_env__.get_framework_env(),
+        timeout=llm_config["timeout"],
+        model_name=llm_config["model_name"],
+        framework=llm_config["env"]["framework_value"],
         configuration=llm_config.model_dump_json().decode(),
     )
```

### Comparing `openllm-0.1.5/src/openllm/_types.py` & `openllm-0.1.6/src/openllm/_types.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/src/openllm/cli.py` & `openllm-0.1.6/src/openllm/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,53 +10,61 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 CLI utilities for OpenLLM.
 
-This extends clidantic and BentoML's internal CLI CommandGroup.
+This extends BentoML's internal CLI CommandGroup.
 """
 from __future__ import annotations
 
 import functools
 import inspect
 import logging
 import os
 import re
-import contextlib
 import sys
 import time
 import traceback
 import typing as t
 
 import bentoml
 import click
 import click_option_group as cog
 import inflection
 import orjson
 import psutil
-from bentoml._internal.configuration import get_debug_mode, get_quiet_mode, set_quiet_mode
 from bentoml._internal.configuration.containers import BentoMLContainer
-from bentoml._internal.log import configure_logging, configure_server_logging
 from bentoml_cli.utils import BentoMLCommandGroup
+from simple_di import Provide, inject
 
 import openllm
 
-from .utils import DEBUG, LazyType, ModelEnv, analytics, bentoml_cattr, first_not_none
+from .__about__ import __version__
+from .exceptions import OpenLLMException
+from .utils import (DEBUG, LazyLoader, LazyType, ModelEnv, analytics,
+                    bentoml_cattr, configure_logging, configure_server_logging,
+                    first_not_none, get_debug_mode, get_quiet_mode, gpu_count,
+                    is_torch_available, set_debug_mode, set_quiet_mode)
 
 if t.TYPE_CHECKING:
+    import torch
+    from bentoml._internal.models import ModelStore
+
     from ._types import ClickFunctionWrapper, F, P
+    from .models.auto.factory import _BaseAutoLLMClass
 
     ServeCommand = t.Literal["serve", "serve-grpc"]
     OutputLiteral = t.Literal["json", "pretty", "porcelain"]
 
     TupleStrAny = tuple[str, ...]
 else:
     TupleStrAny = tuple
+    torch = LazyLoader("torch", globals(), "torch")
 
 
 logger = logging.getLogger(__name__)
 
 COLUMNS = int(os.environ.get("COLUMNS", 120))
 
 _CONTEXT_SETTINGS = {"help_option_names": ["-h", "--help"], "max_content_width": COLUMNS}
@@ -67,231 +75,181 @@
 ██║   ██║██████╔╝█████╗  ██╔██╗ ██║██║     ██║     ██╔████╔██║
 ██║   ██║██╔═══╝ ██╔══╝  ██║╚██╗██║██║     ██║     ██║╚██╔╝██║
 ╚██████╔╝██║     ███████╗██║ ╚████║███████╗███████╗██║ ╚═╝ ██║
  ╚═════╝ ╚═╝     ╚══════╝╚═╝  ╚═══╝╚══════╝╚══════╝╚═╝     ╚═╝
 """
 
 
-def _echo(text: t.Any, fg: str = "green", _with_style: bool = True, **attrs: t.Any) -> None:
-    call = click.echo
-    if _with_style:
-        attrs["fg"] = fg if not get_debug_mode() else None
-        call = click.secho
-    call(text, **attrs)
-
-
-def start_model_command(
-    model_name: str,
-    group: click.Group,
-    _context_settings: dict[str, t.Any] | None = None,
-    _serve_grpc: bool = False,
-) -> click.Command:
-    """Generate a 'click.Command' for any given LLM.
-
-    Args:
-        model_name: The name of the model
-        factory: The click.Group to add the command to
-        _context_settings: The context settings to use for the command
-        _serve_grpc: Whether to serve the model via gRPC or HTTP
-
-    Returns:
-        The click.Command for starting the model server
+class NargsOptions(cog.GroupedOption):
+    """An option that supports nargs=-1.
+    Derived from https://stackoverflow.com/a/48394004/8643197
 
-    Note that the internal commands will return the llm_config and a boolean determine
-    whether the server is run with GPU or not.
+    We mk add_to_parser to handle multiple value that is passed into this specific
+    options.
     """
-    from bentoml._internal.configuration.containers import BentoMLContainer
-    from bentoml._internal.log import configure_logging
 
-    configure_logging()
-
-    llm_config = openllm.AutoConfig.for_model(model_name)
+    def __init__(self, *args: t.Any, **attrs: t.Any):
+        nargs = attrs.pop("nargs", -1)
+        if nargs != -1:
+            raise OpenLLMException(f"'nargs' is set, and must be -1 instead of {nargs}")
+        super(NargsOptions, self).__init__(*args, **attrs)
+        self._prev_parser_process: t.Callable[[t.Any, click.parser.ParsingState], None] | None = None
+        self._nargs_parser: click.parser.Option | None = None
 
-    docstring = f"""\
-{llm_config.__openllm_env__.start_docstring}
-\b
-Available model_id(s): {llm_config.__openllm_model_ids__} [default: {llm_config.__openllm_default_id__}]
-"""
-    command_attrs: dict[str, t.Any] = {
-        "name": llm_config.__openllm_model_name__,
-        "context_settings": _context_settings or {},
-        "short_help": f"Start a LLMServer for '{model_name}' ('--help' for more details)",
-        "help": docstring,
-    }
+    def add_to_parser(self, parser: click.OptionParser, ctx: click.Context) -> None:
+        def _parser(value: t.Any, state: click.parser.ParsingState):
+            # method to hook to the parser.process
+            done = False
+            value = [value]
+            # grab everything up to the next option
+            assert self._nargs_parser is not None
+            while state.rargs and not done:
+                for prefix in self._nargs_parser.prefixes:
+                    if state.rargs[0].startswith(prefix):
+                        done = True
+                if not done:
+                    value.append(state.rargs.pop(0))
+            value = tuple(value)
 
-    aliases: list[str] = []
-    if llm_config.__openllm_name_type__ == "dasherize":
-        aliases.append(llm_config.__openllm_start_name__)
+            # call the actual process
+            assert self._prev_parser_process is not None
+            self._prev_parser_process(value, state)
 
-    command_attrs["aliases"] = aliases if len(aliases) > 0 else None
+        retval = super(NargsOptions, self).add_to_parser(parser, ctx)
+        for name in self.opts:
+            our_parser = parser._long_opt.get(name) or parser._short_opt.get(name)
+            if our_parser:
+                self._nargs_parser = our_parser
+                self._prev_parser_process = our_parser.process
+                our_parser.process = _parser
+                break
+        return retval
 
-    serve_decorator = _http_server_args if not _serve_grpc else _grpc_server_args
 
-    try:
-        llm_config.check_if_gpu_is_available()
-    except openllm.exceptions.GpuNotAvailableError:
-        # NOTE: The model requires GPU, therefore we will return a dummy command
-        command_attrs.update(
-            {
-                "short_help": "(Disabled because there is no GPU available)",
-                "help": f"""{model_name} is currently not available to run on your
-                local machine because it requires GPU for faster inference.""",
-            }
-        )
-
-        @group.command(**command_attrs)
-        def noop() -> openllm.LLMConfig:
-            _echo("No GPU available, therefore this command is disabled", fg="red")
-            analytics.track_start_init(llm_config)
-            return llm_config
+def parse_device_callback(
+    _: click.Context, params: click.Parameter, value: tuple[str, ...] | tuple[t.Literal["all"] | str] | None
+) -> t.Any:
+    if value is None:
+        return value
 
-        return noop
+    if not LazyType(TupleStrAny).isinstance(value):
+        raise RuntimeError(f"{params} only accept multiple values.")
 
-    @group.command(**command_attrs)
-    @llm_config.to_click_options
-    @serve_decorator
-    @cog.optgroup.group("General LLM Options")
-    @cog.optgroup.option("--server-timeout", type=int, default=None, help="Server timeout in seconds")
-    @model_id_option(cog.optgroup, model_env=llm_config.__openllm_env__)
-    @cog.optgroup.option(
-        "--device",
-        type=tuple,
-        cls=NargsOptions,
-        nargs=-1,
-        envvar="CUDA_VISIBLE_DEVICES",
-        callback=parse_device_callback,
-        help=f"Assign GPU devices (if available) for {model_name}.",
-        show_envvar=True,
-    )
-    @workers_per_resource_option(cog.optgroup)
-    @click.pass_context
-    def model_start(
-        ctx: click.Context,
-        server_timeout: int | None,
-        model_id: str | None,
-        workers_per_resource: float | None,
-        device: tuple[str, ...] | None,
-        **attrs: t.Any,
-    ) -> openllm.LLMConfig:
-        config, server_attrs = llm_config.model_validate_click(**attrs)
+    # NOTE: --device all is a special case
+    if len(value) == 1 and value[0] == "all":
+        return gpu_count()
 
-        if llm_config.__openllm_env__.get_framework_env() == "flax":
-            llm = openllm.AutoFlaxLLM.for_model(model_name, model_id=model_id, llm_config=config)
-        elif llm_config.__openllm_env__.get_framework_env() == "tf":
-            llm = openllm.AutoTFLLM.for_model(model_name, model_id=model_id, llm_config=config)
+    parsed: tuple[str, ...] = tuple()
+    for v in value:
+        if v == ",":
+            # NOTE: This hits when CUDA_VISIBLE_DEVICES is set
+            continue
+        if "," in v:
+            parsed += tuple(v.split(","))
         else:
-            llm = openllm.AutoLLM.for_model(model_name, model_id=model_id, llm_config=config)
+            parsed += tuple(v.split())
+    return tuple(filter(lambda x: x, parsed))
 
-        if llm.config.__openllm_requirements__ is not None and len(llm.config.__openllm_requirements__) > 0:
-            _echo(
-                f"Make sure to have the following dependencies available: {llm.config.__openllm_requirements__}",
-                fg="yellow",
-            )
 
-        # NOTE: We need to initialize llm here first to check if the model is already downloaded to
-        # avoid deadlock before the subprocess forking.
-        with open(os.devnull, "w") as devnull:
-            with contextlib.redirect_stderr(devnull), contextlib.redirect_stdout(devnull):
-                ctx.invoke(
-                    download_models,
-                    model_name=model_name,
-                    model_id=llm.model_id,
-                    output="porcelain",
-                )
+def _echo(text: t.Any, fg: str = "green", _with_style: bool = True, **attrs: t.Any) -> None:
+    call = click.echo
+    if _with_style:
+        attrs["fg"] = fg if not get_debug_mode() else None
+        call = click.secho
+    call(text, **attrs)
 
-        workers_per_resource = first_not_none(workers_per_resource, default=llm.config.__openllm_workers_per_resource__)
-        server_timeout = first_not_none(server_timeout, default=llm.config.__openllm_timeout__)
 
-        num_workers = int(1 / workers_per_resource)
-        if num_workers > 1:
-            _echo(
-                f"{model_name} requires at least {num_workers} GPUs/CPUs available per worker."
-                " Make sure that it has available resources to run inference.",
-                fg="yellow",
-            )
+output_option = click.option(
+    "-o",
+    "--output",
+    type=click.Choice(["json", "pretty", "porcelain"]),
+    default="pretty",
+    help="Showing output type.",
+    show_default=True,
+    envvar="OPENLLM_OUTPUT",
+    show_envvar=True,
+)
 
-        server_attrs.update({"working_dir": os.path.dirname(__file__)})
-        if _serve_grpc:
-            server_attrs["grpc_protocol_version"] = "v1"
-        # NOTE: currently, theres no development args in bentoml.Server. To be fixed upstream.
-        development = server_attrs.pop("development")
-        server_attrs.setdefault("production", not development)
 
-        start_env = os.environ.copy()
+def model_id_option(factory: t.Any, model_env: ModelEnv | None = None, click_type: click.ParamType | None = None):
+    envvar = None
+    if model_env is not None:
+        envvar = model_env.model_id
+    return factory.option(
+        "--model-id",
+        type=click_type if click_type else click.STRING,
+        default=None,
+        help="Optional model_id name or path for (fine-tune) weight.",
+        envvar=envvar,
+        show_envvar=True if envvar is not None else False,
+    )
 
-        # NOTE: This is to set current configuration
-        _bentoml_config_options = start_env.pop("BENTOML_CONFIG_OPTIONS", "")
-        _bentoml_config_options_opts = [
-            "tracing.sample_rate=1.0",
-            f"api_server.traffic.timeout={server_timeout}",
-            f'runners."llm-{llm.config.__openllm_start_name__}-runner".traffic.timeout={llm.config.__openllm_timeout__}',
-            f'runners."llm-{llm.config.__openllm_start_name__}-runner".workers_per_resource={workers_per_resource}',
-        ]
-        if device:
-            if len(device) > 1:
-                for idx, dev in enumerate(device):
-                    _bentoml_config_options_opts.append(
-                        f'runners."llm-{llm.config.__openllm_start_name__}-runner".resources."nvidia.com/gpu"[{idx}]={dev}'
-                    )
-            else:
-                _bentoml_config_options_opts.append(
-                    f'runners."llm-{llm.config.__openllm_start_name__}-runner".resources."nvidia.com/gpu"=[{device[0]}]'
-                )
 
-        _bentoml_config_options += " " if _bentoml_config_options else "" + " ".join(_bentoml_config_options_opts)
+def workers_per_resource_option(factory: t.Any, build: bool = False):
+    help_str = """Number of workers per resource assigned.
+    See https://docs.bentoml.org/en/latest/guides/scheduling.html#resource-scheduling-strategy
+    for more information. By default, this is set to 1."""
+    if build:
+        help_str += """\n
+    NOTE: The workers value passed into 'build' will determine how the LLM can
+    be provisioned in Kubernetes as well as in standalone container. This will
+    ensure it has the same effect with 'openllm start --workers ...'"""
+    return factory.option(
+        "--workers-per-resource",
+        default=None,
+        type=click.FLOAT,
+        help=help_str,
+        required=False,
+    )
 
-        start_env.update(
-            {
-                llm.config.__openllm_env__.framework: llm.config.__openllm_env__.get_framework_env(),
-                llm.config.__openllm_env__.model_config: llm.config.model_dump_json().decode(),
-                "OPENLLM_MODEL": model_name,
-                "OPENLLM_MODEL_ID": llm.model_id,
-                "BENTOML_DEBUG": str(get_debug_mode()),
-                "BENTOML_CONFIG_OPTIONS": _bentoml_config_options,
-                "BENTOML_HOME": os.environ.get("BENTOML_HOME", BentoMLContainer.bentoml_home.get()),
-            }
-        )
 
-        if t.TYPE_CHECKING:
-            server_cls: type[bentoml.HTTPServer] if not _serve_grpc else type[bentoml.GrpcServer]
+def quantize_option(factory: t.Any, build: bool = False):
+    help_str = (
+        "Running this model in quantized mode." if not build else "Set quantization mode for serving in deployment."
+    )
+    help_str += """\n
 
-        server_cls = getattr(bentoml, "HTTPServer" if not _serve_grpc else "GrpcServer")
-        server_attrs["timeout"] = 90
-        server = server_cls("_service.py:svc", **server_attrs)
+    GPTQ is currently working in progress and will be available soon.
 
-        try:
-            analytics.track_start_init(llm.config)
-            server.start(env=start_env, text=True, blocking=True)
-        except Exception as err:
-            _echo(f"Error caught while starting LLM Server:\n{err}", fg="red")
-            raise
-        else:
-            if not get_debug_mode():
-                _echo(
-                    f"\n🚀 Next step: run 'openllm build {model_name}' to create a Bento for {model_name}",
-                    fg="blue",
-                )
+    NOTE: Quantization is only available for PyTorch models.
+    """
+    return factory.option(
+        "--quantize",
+        type=click.Choice(["int8", "int4", "gptq"]),
+        default=None,
+        help=help_str,
+    )
 
-        # NOTE: Return the configuration for telemetry purposes.
-        return llm_config
 
-    return model_start
+def bettertransformer_option(factory: t.Any, model_env: ModelEnv | None = None):
+    envvar = None
+    if model_env is not None:
+        envvar = model_env.model_id
+    return factory.option(
+        "--bettertransformer",
+        is_flag=True,
+        default=None,
+        help="Use BetterTransformer wrapper to serve model. This will applies during serving time.",
+        envvar=envvar,
+        show_envvar=True if envvar is not None else False,
+    )
 
 
 class OpenLLMCommandGroup(BentoMLCommandGroup):
     NUMBER_OF_COMMON_PARAMS = 3
 
     @staticmethod
     def common_params(f: F[P, t.Any]) -> ClickFunctionWrapper[..., t.Any]:
         """This is not supposed to be used with unprocessed click function.
         This should be used a the last currying from common_params -> usage_tracking -> exception_handling
         """
         # The following logics is similar to one of BentoMLCommandGroup
 
-        from bentoml._internal.configuration import DEBUG_ENV_VAR, QUIET_ENV_VAR, set_debug_mode
+        from bentoml._internal.configuration import (DEBUG_ENV_VAR,
+                                                     QUIET_ENV_VAR)
 
         @click.option("-q", "--quiet", envvar=QUIET_ENV_VAR, is_flag=True, default=False, help="Suppress all output.")
         @click.option(
             "--debug", "--verbose", envvar=DEBUG_ENV_VAR, is_flag=True, default=False, help="Print out debug logs."
         )
         @click.option(
             "--do-not-track",
@@ -360,43 +318,35 @@
         """
         command_name = attrs.get("name", func.__name__)
 
         @functools.wraps(func)
         def wrapper(*args: P.args, **attrs: P.kwargs) -> t.Any:
             try:
                 return func(*args, **attrs)
-            except openllm.exceptions.OpenLLMException as err:
+            except OpenLLMException as err:
                 raise click.ClickException(
                     click.style(f"[{group.name}] '{command_name}' failed: " + err.message, fg="red")
                 ) from err
             except KeyboardInterrupt:  # NOTE: silience KeyboardInterrupt
                 pass
 
         return t.cast("ClickFunctionWrapper[..., t.Any]", wrapper)
 
-    def __init__(self, *args: t.Any, **attrs: t.Any) -> None:
-        super(OpenLLMCommandGroup, self).__init__(*args, **attrs)
-        # these two dictionaries will store known aliases for commands and groups
-        self._cached_http: dict[str, t.Any] = {}
-        self._cached_grpc: dict[str, t.Any] = {}
-
     def get_command(self, ctx: click.Context, cmd_name: str) -> click.Command | None:
         cmd_name = self.resolve_alias(cmd_name)
         if ctx.command.name == "start":
-            if cmd_name not in self._cached_http:
-                self._cached_http[cmd_name] = start_model_command(
-                    cmd_name, self, _context_settings=ctx.command.context_settings
-                )
-            return self._cached_http[cmd_name]
+            try:
+                return _cached_http[cmd_name]
+            except KeyError:
+                raise click.BadArgumentUsage(f"{cmd_name} is not a valid model identifier supported by OpenLLM.")
         elif ctx.command.name == "start-grpc":
-            if cmd_name not in self._cached_grpc:
-                self._cached_grpc[cmd_name] = start_model_command(
-                    cmd_name, self, _context_settings=ctx.command.context_settings, _serve_grpc=True
-                )
-            return self._cached_grpc[cmd_name]
+            try:
+                return _cached_grpc[cmd_name]
+            except KeyError:
+                raise click.BadArgumentUsage(f"{cmd_name} is not a valid model identifier supported by OpenLLM.")
         return super().get_command(ctx, cmd_name)
 
     def list_commands(self, ctx: click.Context) -> list[str]:
         if ctx.command.name == "start" or ctx.command.name == "start-grpc":
             return list(openllm.CONFIG_MAPPING.keys())
 
         return super().list_commands(ctx)
@@ -444,14 +394,50 @@
             return cmd
 
         # XXX: The current type coercion is not ideal, but we can really
         # loosely define it
         return t.cast("F[[t.Callable[..., t.Any]], click.Command]", wrapper)
 
 
+@click.group(cls=OpenLLMCommandGroup, context_settings=_CONTEXT_SETTINGS, name="openllm")
+@click.version_option(__version__, "--version", "-v")
+def cli():
+    """
+    \b
+     ██████╗ ██████╗ ███████╗███╗   ██╗██╗     ██╗     ███╗   ███╗
+    ██╔═══██╗██╔══██╗██╔════╝████╗  ██║██║     ██║     ████╗ ████║
+    ██║   ██║██████╔╝█████╗  ██╔██╗ ██║██║     ██║     ██╔████╔██║
+    ██║   ██║██╔═══╝ ██╔══╝  ██║╚██╗██║██║     ██║     ██║╚██╔╝██║
+    ╚██████╔╝██║     ███████╗██║ ╚████║███████╗███████╗██║ ╚═╝ ██║
+     ╚═════╝ ╚═╝     ╚══════╝╚═╝  ╚═══╝╚══════╝╚══════╝╚═╝     ╚═╝
+
+    \b
+    An open platform for operating large language models in production.
+    Fine-tune, serve, deploy, and monitor any LLMs with ease.
+    """
+
+
+@cli.group(cls=OpenLLMCommandGroup, context_settings=_CONTEXT_SETTINGS, name="start")
+def start_cli():
+    """
+    Start any LLM as a REST server.
+
+    $ openllm start <model_name> --<options> ...
+    """
+
+
+@cli.group(cls=OpenLLMCommandGroup, context_settings=_CONTEXT_SETTINGS, name="start-grpc")
+def start_grpc_cli():
+    """
+    Start any LLM as a gRPC server.
+
+    $ openllm start-grpc <model_name> --<options> ...
+    """
+
+
 # NOTE: A list of bentoml option that is not needed for parsing.
 # NOTE: User shouldn't set '--working-dir', as OpenLLM will setup this.
 # NOTE: production is also deprecated
 _IGNORED_OPTIONS = {"working_dir", "production", "protocol_version"}
 
 
 if t.TYPE_CHECKING:
@@ -493,547 +479,664 @@
     return decorator
 
 
 _http_server_args = parse_serve_args(False)
 _grpc_server_args = parse_serve_args(True)
 
 
-class NargsOptions(cog.GroupedOption):
-    """An option that supports nargs=-1.
-    Derived from https://stackoverflow.com/a/48394004/8643197
+def start_model_command(
+    model_name: str,
+    _context_settings: dict[str, t.Any] | None = None,
+    _serve_grpc: bool = False,
+) -> click.Command:
+    """Generate a 'click.Command' for any given LLM.
 
-    We mk add_to_parser to handle multiple value that is passed into this specific
-    options.
+    Args:
+        model_name: The name of the model
+        factory: The click.Group to add the command to
+        _context_settings: The context settings to use for the command
+        _serve_grpc: Whether to serve the model via gRPC or HTTP
+
+    Returns:
+        The click.Command for starting the model server
+
+    Note that the internal commands will return the llm_config and a boolean determine
+    whether the server is run with GPU or not.
     """
+    from bentoml._internal.configuration.containers import BentoMLContainer
 
-    def __init__(self, *args: t.Any, **attrs: t.Any):
-        nargs = attrs.pop("nargs", -1)
-        if nargs != -1:
-            raise openllm.exceptions.OpenLLMException(f"'nargs' is set, and must be -1 instead of {nargs}")
-        super(NargsOptions, self).__init__(*args, **attrs)
-        self._prev_parser_process: t.Callable[[t.Any, click.parser.ParsingState], None] | None = None
-        self._nargs_parser: click.parser.Option | None = None
+    configure_logging()
 
-    def add_to_parser(self, parser: click.OptionParser, ctx: click.Context) -> None:
-        def _parser(value: t.Any, state: click.parser.ParsingState):
-            # method to hook to the parser.process
-            done = False
-            value = [value]
-            # grab everything up to the next option
-            assert self._nargs_parser is not None
-            while state.rargs and not done:
-                for prefix in self._nargs_parser.prefixes:
-                    if state.rargs[0].startswith(prefix):
-                        done = True
-                if not done:
-                    value.append(state.rargs.pop(0))
-            value = tuple(value)
+    llm_config = openllm.AutoConfig.for_model(model_name)
+    env: ModelEnv = llm_config["env"]
 
-            # call the actual process
-            assert self._prev_parser_process is not None
-            self._prev_parser_process(value, state)
+    docstring = f"""\
+{env.start_docstring}
+\b
+Available model_id(s): {llm_config['model_ids']} [default: {llm_config['default_id']}]
+"""
+    command_attrs: dict[str, t.Any] = {
+        "name": llm_config["model_name"],
+        "context_settings": _context_settings or {},
+        "short_help": f"Start a LLMServer for '{model_name}' ('--help' for more details)",
+        "help": docstring,
+    }
 
-        retval = super(NargsOptions, self).add_to_parser(parser, ctx)
-        for name in self.opts:
-            our_parser = parser._long_opt.get(name) or parser._short_opt.get(name)
-            if our_parser:
-                self._nargs_parser = our_parser
-                self._prev_parser_process = our_parser.process
-                our_parser.process = _parser
-                break
-        return retval
+    aliases: list[str] = []
+    if llm_config["name_type"] == "dasherize":
+        aliases.append(llm_config["start_name"])
 
+    command_attrs["aliases"] = aliases if len(aliases) > 0 else None
 
-def parse_device_callback(
-    _: click.Context, params: click.Parameter, value: tuple[str, ...] | tuple[t.Literal["all"]] | None
-) -> t.Any:
-    if value is None:
-        return value
+    serve_decorator = _http_server_args if not _serve_grpc else _grpc_server_args
+    group = start_cli if not _serve_grpc else start_grpc_cli
 
-    if not LazyType(TupleStrAny).isinstance(value):
-        raise RuntimeError(f"{params} only accept multiple values.")
+    available_gpu = gpu_count()
+    if llm_config["requires_gpu"] and len(available_gpu) < 1:
+        # NOTE: The model requires GPU, therefore we will return a dummy command
+        command_attrs.update(
+            {
+                "short_help": "(Disabled because there is no GPU available)",
+                "help": f"""{model_name} is currently not available to run on your
+                local machine because it requires GPU for faster inference.""",
+            }
+        )
 
-    # NOTE: --device all is a special case
-    if len(value) == 1:
-        if value[0] != "all":
-            raise RuntimeError(f"{params} parameter only accept 'all' as a string value.")
-        import pynvml  # transitive dependencies of BentoML
+        @group.command(**command_attrs)
+        def noop() -> openllm.LLMConfig:
+            _echo("No GPU available, therefore this command is disabled", fg="red")
+            analytics.track_start_init(llm_config)
+            return llm_config
 
-        try:
-            pynvml.nvmlInit()
-            return tuple(range(pynvml.nvmlDeviceGetCount()))
-        except (pynvml.nvml.NVMLError, OSError):
-            logger.debug("GPU not detected. Unable to initialize pynvml lib.")
-            return ()
-        finally:
-            try:
-                pynvml.nvmlShutdown()
-            except Exception:
-                pass
+        return noop
 
-    parsed: tuple[str, ...] = tuple()
-    for v in value:
-        if v == ",":
-            # NOTE: This hits when CUDA_VISIBLE_DEVICES is set
-            continue
-        if "," in v:
-            parsed += tuple(v.split(","))
+    @group.command(**command_attrs)
+    @llm_config.to_click_options
+    @serve_decorator
+    @cog.optgroup.group("General LLM Options")
+    @cog.optgroup.option(
+        "--server-timeout",
+        type=int,
+        default=None,
+        help="Server timeout in seconds",
+    )
+    @workers_per_resource_option(cog.optgroup)
+    @model_id_option(cog.optgroup, model_env=env, click_type=click.Choice(llm_config["model_ids"]))
+    @cog.optgroup.option(
+        "--device",
+        type=tuple,
+        cls=NargsOptions,
+        nargs=-1,
+        envvar="CUDA_VISIBLE_DEVICES",
+        callback=parse_device_callback,
+        help=f"Assign GPU devices (if available) for {model_name}.",
+        show_envvar=True,
+    )
+    @quantize_option(cog.optgroup)
+    @bettertransformer_option(cog.optgroup, model_env=env)
+    @cog.optgroup.option(
+        "--fast",
+        is_flag=True,
+        default=False,
+        help="Bypass auto model checks and setup. This option is ahead-of-serving time.",
+    )
+    @click.pass_context
+    def model_start(
+        ctx: click.Context,
+        server_timeout: int | None,
+        model_id: str | None,
+        workers_per_resource: float | None,
+        device: tuple[str, ...] | None,
+        quantize: t.Literal["int8", "int4", "gptq"] | None,
+        bettertransformer: bool | None,
+        fast: bool,
+        **attrs: t.Any,
+    ) -> openllm.LLMConfig:
+        config, server_attrs = llm_config.model_validate_click(**attrs)
+
+        # Create a new model env to work with the envvar during CLI invocation
+        env = ModelEnv(config["model_name"])
+        framework_envvar = env.framework_value
+
+        if quantize:
+            gpu_available = gpu_count()
+            if len(gpu_available) < 1:
+                _echo(f"Quantization requires at least 1 GPU (got {len(gpu_available)})", fg="red")
+                ctx.exit(1)
+            if framework_envvar != "pt":
+                _echo("Quantization is currently only available for PyTorch models.", fg="red")
+                ctx.exit(1)
+
+        # We need to handle None separately here, as env from subprocess doesn't
+        # accept None value.
+        env = ModelEnv(env.model_name, bettertransformer=bettertransformer, quantize=quantize)
+
+        requirements = config["requirements"]
+        if requirements is not None and len(requirements) > 0:
+            _echo(
+                f"Make sure to have the following dependencies available: {requirements}",
+                fg="yellow",
+            )
+
+        workers_per_resource = first_not_none(workers_per_resource, default=config["workers_per_resource"])
+        server_timeout = first_not_none(server_timeout, default=config["timeout"])
+
+        num_workers = int(1 / workers_per_resource)
+        if num_workers > 1:
+            _echo(
+                f"Running '{model_name}' requires at least {num_workers} GPUs/CPUs available per worker."
+                " Make sure that it has available resources for inference.",
+                fg="yellow",
+            )
+
+        server_attrs.update({"working_dir": os.path.dirname(__file__)})
+        if _serve_grpc:
+            server_attrs["grpc_protocol_version"] = "v1"
+        # NOTE: currently, theres no development args in bentoml.Server. To be fixed upstream.
+        development = server_attrs.pop("development")
+        server_attrs.setdefault("production", not development)
+
+        # NOTE: This is to set current configuration
+        start_env = os.environ.copy()
+        _bentoml_config_options_env = start_env.pop("BENTOML_CONFIG_OPTIONS", "")
+        _bentoml_config_options_opts = [
+            "tracing.sample_rate=1.0",
+            f"api_server.traffic.timeout={server_timeout}",
+            f'runners."llm-{config["start_name"]}-runner".traffic.timeout={config["timeout"]}',
+            f'runners."llm-{config["start_name"]}-runner".workers_per_resource={workers_per_resource}',
+        ]
+        if device:
+            if len(device) > 1:
+                for idx, dev in enumerate(device):
+                    _bentoml_config_options_opts.append(
+                        f'runners."llm-{config["start_name"]}-runner".resources."nvidia.com/gpu"[{idx}]={dev}'
+                    )
+            else:
+                _bentoml_config_options_opts.append(
+                    f'runners."llm-{config["start_name"]}-runner".resources."nvidia.com/gpu"=[{device[0]}]'
+                )
+
+        _bentoml_config_options_env += (
+            " " if _bentoml_config_options_env else "" + " ".join(_bentoml_config_options_opts)
+        )
+
+        automodel_attrs = {
+            "model_id": model_id,
+            "llm_config": config,
+            "ensure_available": not fast,
+        }
+
+        if framework_envvar == "pt":
+            automodel_attrs.update({"quantize": quantize, "bettertransformer": bettertransformer})
+
+        llm = t.cast(
+            "_BaseAutoLLMClass",
+            openllm[framework_envvar],  # type: ignore (internal API)
+        ).for_model(model_name, **automodel_attrs)
+
+        start_env.update(
+            {
+                env.framework: env.framework_value,
+                env.config: llm.config.model_dump_json().decode(),
+                "OPENLLM_MODEL": model_name,
+                "OPENLLM_MODEL_ID": llm.model_id,
+                "BENTOML_DEBUG": str(get_debug_mode()),
+                "BENTOML_CONFIG_OPTIONS": _bentoml_config_options_env,
+                "BENTOML_HOME": os.environ.get("BENTOML_HOME", BentoMLContainer.bentoml_home.get()),
+            }
+        )
+
+        if env.bettertransformer_value is not None:
+            start_env[env.bettertransformer] = env.bettertransformer_value
+        if env.quantize_value is not None:
+            start_env[env.quantize] = env.quantize_value
+
+        if t.TYPE_CHECKING:
+            server_cls: type[bentoml.HTTPServer] if not _serve_grpc else type[bentoml.GrpcServer]
+
+        server_cls = getattr(bentoml, "HTTPServer" if not _serve_grpc else "GrpcServer")
+        server_attrs["timeout"] = server_timeout
+        server = server_cls("_service.py:svc", **server_attrs)
+
+        try:
+            analytics.track_start_init(llm.config)
+            server.start(env=start_env, text=True, blocking=True)
+        except Exception as err:
+            _echo(f"Error caught while starting LLM Server:\n{err}", fg="red")
+            raise
         else:
-            parsed += tuple(v.split())
-    return tuple(filter(lambda x: x, parsed))
+            if not get_debug_mode():
+                _echo(
+                    f"\n🚀 Next step: run 'openllm build {model_name}' to create a Bento for {model_name}",
+                    fg="blue",
+                )
+
+        # NOTE: Return the configuration for telemetry purposes.
+        return llm_config
+
+    return model_start
+
+
+_cached_http = {key: start_model_command(key, _context_settings=_CONTEXT_SETTINGS) for key in openllm.CONFIG_MAPPING}
+_cached_grpc = {
+    key: start_model_command(key, _context_settings=_CONTEXT_SETTINGS, _serve_grpc=True)
+    for key in openllm.CONFIG_MAPPING
+}
 
 
 def _start(
     model_name: str,
     framework: t.Literal["flax", "tf", "pt"] | None = None,
     **attrs: t.Any,
 ):
     """Python API to start a LLM server."""
     _serve_grpc = attrs.pop("_serve_grpc", False)
 
     _ModelEnv = ModelEnv(model_name)
 
     if framework is not None:
         os.environ[_ModelEnv.framework] = framework
-    start_model_command(model_name, t.cast(OpenLLMCommandGroup, cli), _serve_grpc=_serve_grpc)(
-        standalone_mode=False, **attrs
-    )
+    start_model_command(model_name, _serve_grpc=_serve_grpc)(standalone_mode=False, **attrs)
 
 
 start = functools.partial(_start, _serve_grpc=False)
 start_grpc = functools.partial(_start, _serve_grpc=True)
 
 
-output_option = click.option(
-    "-o",
-    "--output",
-    type=click.Choice(["json", "pretty", "porcelain"]),
-    default="pretty",
-    help="Showing output type.",
-    show_default=True,
-    envvar="OPENLLM_OUTPUT",
-    show_envvar=True,
-)
-
-
-def model_id_option(factory: t.Any, model_env: ModelEnv | None = None):
-    envvar = None
-    if model_env is not None:
-        envvar = model_env.model_id
-    return factory.option(
-        "--model-id",
-        type=click.STRING,
-        default=None,
-        help="Optional model_id name or path for (fine-tune) weight.",
-        envvar=envvar,
-        show_envvar=True if envvar is not None else False,
-    )
+@cli.command()
+@click.argument("model_name", type=click.Choice([inflection.dasherize(name) for name in openllm.CONFIG_MAPPING.keys()]))
+@model_id_option(click)
+@output_option
+@click.option("--overwrite", is_flag=True, help="Overwrite existing Bento for given LLM if it already exists.")
+@workers_per_resource_option(click, build=True)
+@cog.optgroup.group(cls=cog.MutuallyExclusiveOptionGroup, name="Optimisation options.")
+@quantize_option(cog.optgroup, build=True)
+@bettertransformer_option(cog.optgroup)
+def build(
+    model_name: str,
+    model_id: str | None,
+    overwrite: bool,
+    output: OutputLiteral,
+    quantize: t.Literal["int8", "int4", "gptq"] | None,
+    bettertransformer: bool | None,
+    workers_per_resource: float | None,
+):
+    """Package a given models into a Bento.
 
+    $ openllm build flan-t5
 
-def workers_per_resource_option(factory: t.Any, build: bool = False):
-    help_str = """Number of workers per resource assigned.
-    See https://docs.bentoml.org/en/latest/guides/scheduling.html#resource-scheduling-strategy
-    for more information. By default, this is set to 1."""
-    if build:
-        help_str += """\n
-    NOTE: The workers value passed into 'build' will determine how the LLM can
-    be provisioned in Kubernetes as well as in standalone container. This will
-    ensure it has the same effect with 'openllm start --workers ...'"""
-    return factory.option(
-        "--workers-per-resource",
-        default=None,
-        type=click.FLOAT,
-        help=help_str,
-        required=False,
+    \b
+    NOTE: To run a container built from this Bento with GPU support, make sure
+    to have https://github.com/NVIDIA/nvidia-container-toolkit install locally.
+    """
+    if output == "porcelain":
+        set_quiet_mode(True)
+        configure_server_logging()
+
+    if output == "pretty":
+        if overwrite:
+            _echo(f"Overwriting existing Bento for {model_name}.", fg="yellow")
+
+    bento, _previously_built = openllm.build(
+        model_name,
+        __cli__=True,
+        model_id=model_id,
+        quantize=quantize,
+        bettertransformer=bettertransformer,
+        _workers_per_resource=workers_per_resource,
+        _overwrite_existing_bento=overwrite,
     )
 
+    if output == "pretty":
+        if not get_quiet_mode():
+            _echo("\n" + OPENLLM_FIGLET, fg="white")
+            if not _previously_built:
+                _echo(f"Successfully built {bento}.", fg="green")
+            else:
+                _echo(
+                    f"'{model_name}' already has a Bento built [{bento}]. To overwrite it pass '--overwrite'.",
+                    fg="yellow",
+                )
 
-def cli_factory() -> click.Group:
-    from .__about__ import __version__
-
-    configure_logging()
-
-    model_store = BentoMLContainer.model_store.get()
-
-    @click.group(cls=OpenLLMCommandGroup, context_settings=_CONTEXT_SETTINGS, name="openllm")
-    @click.version_option(__version__, "--version", "-v")
-    def cli():
-        """
-        \b
-         ██████╗ ██████╗ ███████╗███╗   ██╗██╗     ██╗     ███╗   ███╗
-        ██╔═══██╗██╔══██╗██╔════╝████╗  ██║██║     ██║     ████╗ ████║
-        ██║   ██║██████╔╝█████╗  ██╔██╗ ██║██║     ██║     ██╔████╔██║
-        ██║   ██║██╔═══╝ ██╔══╝  ██║╚██╗██║██║     ██║     ██║╚██╔╝██║
-        ╚██████╔╝██║     ███████╗██║ ╚████║███████╗███████╗██║ ╚═╝ ██║
-         ╚═════╝ ╚═╝     ╚══════╝╚═╝  ╚═══╝╚══════╝╚══════╝╚═╝     ╚═╝
-
-        \b
-        An open platform for operating large language models in production.
-        Fine-tune, serve, deploy, and monitor any LLMs with ease.
-        """
-
-    @cli.group(cls=OpenLLMCommandGroup, context_settings=_CONTEXT_SETTINGS)
-    def start():
-        """
-        Start any LLM as a REST server.
-
-        $ openllm start <model_name> --<options> ...
-        """
+            _echo(
+                "\nPossible next steps:\n\n"
+                + "* Push to BentoCloud with `bentoml push`:\n"
+                + f"    $ bentoml push {bento.tag}\n"
+                + "* Containerize your Bento with `bentoml containerize`:\n"
+                + f"    $ bentoml containerize {bento.tag}\n"
+                + "    Tip: To enable additional BentoML feature for 'containerize', "
+                + "use '--enable-features=FEATURE[,FEATURE]' "
+                + "[see 'bentoml containerize -h' for more advanced usage]\n",
+                fg="blue",
+            )
+    elif output == "json":
+        _echo(orjson.dumps(bento.info.to_dict(), option=orjson.OPT_INDENT_2).decode())
+    else:
+        _echo(bento.tag)
+    return bento
 
-    @cli.group(cls=OpenLLMCommandGroup, context_settings=_CONTEXT_SETTINGS)
-    def start_grpc():
-        """
-        Start any LLM as a gRPC server.
 
-        $ openllm start-grpc <model_name> --<options> ...
-        """
+@cli.command()
+@output_option
+@click.option(
+    "--show-available",
+    is_flag=True,
+    default=False,
+    help="Show available models in local store (mutually exclusive with '-o porcelain').",
+)
+def models(output: OutputLiteral, show_available: bool):
+    """List all supported models.
 
-    @cli.command()
-    @click.argument(
-        "model_name", type=click.Choice([inflection.dasherize(name) for name in openllm.CONFIG_MAPPING.keys()])
-    )
-    @model_id_option(click)
-    @output_option
-    @click.option("--overwrite", is_flag=True, help="Overwrite existing Bento for given LLM if it already exists.")
-    @workers_per_resource_option(click, build=True)
-    def build(
-        model_name: str,
-        model_id: str | None,
-        overwrite: bool,
-        output: OutputLiteral,
-        workers_per_resource: float | None,
-    ):
-        """Package a given models into a Bento.
+    NOTE: '--show-available' and '-o porcelain' are mutually exclusive.
+    """
+    from ._llm import convert_transformers_model_name
 
-        $ openllm build flan-t5
+    models = tuple(inflection.dasherize(key) for key in openllm.CONFIG_MAPPING.keys())
+    if output == "porcelain":
+        if show_available:
+            raise click.BadOptionUsage(
+                "--show-available", "Cannot use '--show-available' with '-o porcelain' (mutually exclusive)."
+            )
+        _echo("\n".join(models), fg="white")
+    else:
+        failed_initialized: list[tuple[str, Exception]] = []
 
-        \b
-        NOTE: To run a container built from this Bento with GPU support, make sure
-        to have https://github.com/NVIDIA/nvidia-container-toolkit install locally.
-        """
-        if output == "porcelain":
-            set_quiet_mode(True)
-            configure_server_logging()
+        json_data: dict[
+            str, dict[t.Literal["model_id", "url", "installation", "requires_gpu", "runtime_impl"], t.Any]
+        ] = {}
+
+        # NOTE: Keep a sync list with ./tools/update-optional-dependencies.py
+        extras = ["chatglm", "falcon", "flan-t5", "starcoder"]
+
+        converted: list[str] = []
+        for m in models:
+            config = openllm.AutoConfig.for_model(m)
+            runtime_impl: tuple[t.Literal["pt", "flax", "tf"], ...] = tuple()
+            if config["model_name"] in openllm.MODEL_MAPPING_NAMES:
+                runtime_impl += ("pt",)
+            if config["model_name"] in openllm.MODEL_FLAX_MAPPING_NAMES:
+                runtime_impl += ("flax",)
+            if config["model_name"] in openllm.MODEL_TF_MAPPING_NAMES:
+                runtime_impl += ("tf",)
+            json_data[m] = {
+                "model_id": config["model_ids"],
+                "url": config["url"],
+                "requires_gpu": config["requires_gpu"],
+                "runtime_impl": runtime_impl,
+                "installation": "pip install openllm" if m not in extras else f'pip install "openllm[{m}]"',
+            }
+            converted.extend([convert_transformers_model_name(i) for i in config["model_ids"]])
+            if DEBUG:
+                try:
+                    openllm.AutoLLM.for_model(m, llm_config=config)
+                except Exception as err:
+                    failed_initialized.append((m, err))
+
+        ids_in_local_store = None
+        if show_available:
+            ids_in_local_store = {k: [i for i in bentoml.models.list() if k in i.tag.name] for k in json_data.keys()}
+            ids_in_local_store = {k: v for k, v in ids_in_local_store.items() if v}
 
         if output == "pretty":
-            if overwrite:
-                _echo(f"Overwriting existing Bento for {model_name}.", fg="yellow")
-
-        bento, _previously_built = openllm.build(
-            model_name,
-            __cli__=True,
-            model_id=model_id,
-            _workers_per_resource=workers_per_resource,
-            _overwrite_existing_bento=overwrite,
-        )
+            import tabulate
 
-        if output == "pretty":
-            if not get_quiet_mode():
-                _echo("\n" + OPENLLM_FIGLET, fg="white")
-                if not _previously_built:
-                    _echo(f"Successfully built {bento}.", fg="green")
-                else:
-                    _echo(
-                        f"'{model_name}' already has a Bento built [{bento}]. To overwrite it pass '--overwrite'.",
-                        fg="yellow",
-                    )
+            tabulate.PRESERVE_WHITESPACE = True
 
-                _echo(
-                    "\nPossible next steps:\n\n"
-                    + "* Push to BentoCloud with `bentoml push`:\n"
-                    + f"    $ bentoml push {bento.tag}\n"
-                    + "* Containerize your Bento with `bentoml containerize`:\n"
-                    + f"    $ bentoml containerize {bento.tag}\n"
-                    + "    Tip: To enable additional BentoML feature for 'containerize', "
-                    + "use '--enable-features=FEATURE[,FEATURE]' "
-                    + "[see 'bentoml containerize -h' for more advanced usage]\n",
-                    fg="blue",
+            data: list[
+                str | tuple[str, str, list[str], str, t.LiteralString, tuple[t.Literal["pt", "flax", "tf"], ...]]
+            ] = []
+            for m, v in json_data.items():
+                data.extend(
+                    [
+                        (
+                            m,
+                            v["url"],
+                            v["model_id"],
+                            v["installation"],
+                            "✅" if v["requires_gpu"] else "❌",
+                            v["runtime_impl"],
+                        )
+                    ]
                 )
-        elif output == "json":
-            _echo(orjson.dumps(bento.info.to_dict(), option=orjson.OPT_INDENT_2).decode())
-        else:
-            _echo(bento.tag)
-        return bento
-
-    @cli.command()
-    @output_option
-    @click.option(
-        "--show-available",
-        is_flag=True,
-        default=False,
-        help="Show available models in local store (mutually exclusive with '-o porcelain').",
-    )
-    def models(output: OutputLiteral, show_available: bool):
-        """List all supported models.
-
-        NOTE: '--show-available' and '-o porcelain' are mutually exclusive.
-        """
-        from ._llm import convert_transformers_model_name
+            column_widths = [
+                int(COLUMNS / 6),
+                int(COLUMNS / 6),
+                int(COLUMNS / 3),
+                int(COLUMNS / 6),
+                int(COLUMNS / 6),
+                int(COLUMNS / 9),
+            ]
+
+            if len(data) == 0 and len(failed_initialized) > 0:
+                _echo("Exception found while parsing models:\n", fg="yellow")
+                for m, err in failed_initialized:
+                    _echo(f"- {m}: ", fg="yellow", nl=False)
+                    _echo(traceback.print_exception(err, limit=3), fg="red")
+                sys.exit(1)
+
+            table = tabulate.tabulate(
+                data,
+                tablefmt="fancy_grid",
+                headers=["LLM", "URL", "Models Id", "Installation", "GPU Only", "Runtime"],
+                maxcolwidths=column_widths,
+            )
 
-        models = tuple(inflection.dasherize(key) for key in openllm.CONFIG_MAPPING.keys())
-        if output == "porcelain":
-            if show_available:
-                raise click.BadOptionUsage(
-                    "--show-available", "Cannot use '--show-available' with '-o porcelain' (mutually exclusive)."
+            formatted_table = ""
+            for line in table.split("\n"):
+                formatted_table += (
+                    "".join(f"{cell:{width}}" for cell, width in zip(line.split("\t"), column_widths)) + "\n"
                 )
-            _echo("\n".join(models), fg="white")
-        else:
-            failed_initialized: list[tuple[str, Exception]] = []
+            _echo(formatted_table, fg="white")
 
-            json_data: dict[
-                str, dict[t.Literal["model_id", "url", "installation", "requires_gpu", "runtime_impl"], t.Any]
-            ] = {}
-
-            # NOTE: Keep a sync list with ./tools/update-optional-dependencies.py
-            extras = ["chatglm", "falcon", "flan-t5", "starcoder"]
-
-            converted: list[str] = []
-            for m in models:
-                config = openllm.AutoConfig.for_model(m)
-                runtime_impl: tuple[t.Literal["pt", "flax", "tf"], ...] = tuple()
-                if config.__openllm_model_name__ in openllm.MODEL_MAPPING_NAMES:
-                    runtime_impl += ("pt",)
-                if config.__openllm_model_name__ in openllm.MODEL_FLAX_MAPPING_NAMES:
-                    runtime_impl += ("flax",)
-                if config.__openllm_model_name__ in openllm.MODEL_TF_MAPPING_NAMES:
-                    runtime_impl += ("tf",)
-                json_data[m] = {
-                    "model_id": config.__openllm_model_ids__,
-                    "url": config.__openllm_url__,
-                    "requires_gpu": config.__openllm_requires_gpu__,
-                    "runtime_impl": runtime_impl,
-                    "installation": "pip install openllm" if m not in extras else f'pip install "openllm[{m}]"',
-                }
-                converted.extend([convert_transformers_model_name(i) for i in config.__openllm_model_ids__])
-                if DEBUG:
-                    try:
-                        openllm.AutoLLM.for_model(m, llm_config=config)
-                    except Exception as err:
-                        failed_initialized.append((m, err))
+            if DEBUG and len(failed_initialized) > 0:
+                _echo("\nThe following models are supported but failed to initialize:\n")
+                for m, err in failed_initialized:
+                    _echo(f"- {m}: ", fg="blue", nl=False)
+                    _echo(err, fg="red")
 
-            ids_in_local_store = None
             if show_available:
-                ids_in_local_store = [i for i in bentoml.models.list() if any(n in i.tag.name for n in converted)]
-
-            if output == "pretty":
-                import tabulate
-
-                tabulate.PRESERVE_WHITESPACE = True
-
-                data: list[
-                    str | tuple[str, str, list[str], str, t.LiteralString, tuple[t.Literal["pt", "flax", "tf"], ...]]
-                ] = []
-                for m, v in json_data.items():
-                    data.extend(
-                        [
-                            (
-                                m,
-                                v["url"],
-                                v["model_id"],
-                                v["installation"],
-                                "✅" if v["requires_gpu"] else "❌",
-                                v["runtime_impl"],
-                            )
-                        ]
-                    )
-                column_widths = [
-                    int(COLUMNS / 6),
-                    int(COLUMNS / 6),
-                    int(COLUMNS / 3),
-                    int(COLUMNS / 6),
-                    int(COLUMNS / 6),
-                    int(COLUMNS / 9),
-                ]
-
-                if len(data) == 0 and len(failed_initialized) > 0:
-                    _echo("Exception found while parsing models:\n", fg="yellow")
-                    for m, err in failed_initialized:
-                        _echo(f"- {m}: ", fg="yellow", nl=False)
-                        _echo(traceback.print_exception(err, limit=3), fg="red")
-                    sys.exit(1)
+                assert ids_in_local_store
 
+                _available = [[k + "\n\n" * len(v), [str(i.tag) for i in v]] for k, v in ids_in_local_store.items()]
+                column_widths = [int(COLUMNS / 6), int(COLUMNS / 2)]
                 table = tabulate.tabulate(
-                    data,
+                    _available,
                     tablefmt="fancy_grid",
-                    headers=["LLM", "URL", "Models Id", "Installation", "GPU Only", "Runtime"],
+                    headers=["Model Id", "Models"],
                     maxcolwidths=column_widths,
                 )
+                _echo("The following models are available in local store:\n", fg="magenta")
 
                 formatted_table = ""
                 for line in table.split("\n"):
                     formatted_table += (
                         "".join(f"{cell:{width}}" for cell, width in zip(line.split("\t"), column_widths)) + "\n"
                     )
                 _echo(formatted_table, fg="white")
-
-                if DEBUG and len(failed_initialized) > 0:
-                    _echo("\nThe following models are supported but failed to initialize:\n")
-                    for m, err in failed_initialized:
-                        _echo(f"- {m}: ", fg="blue", nl=False)
-                        _echo(err, fg="red")
-
-                if show_available:
-                    assert ids_in_local_store
-                    _echo("The following models are available in local store:\n", fg="white")
-                    for i in ids_in_local_store:
-                        _echo(f"- {i}", fg="white")
-            else:
-                dumped: dict[str, t.Any] = json_data
-                if show_available:
-                    assert ids_in_local_store
-                    dumped["local"] = [bentoml_cattr.unstructure(i.tag) for i in ids_in_local_store]
-                _echo(
-                    orjson.dumps(
-                        dumped,
-                        option=orjson.OPT_INDENT_2,
-                    ).decode(),
-                    fg="white",
-                )
-
-        sys.exit(0)
-
-    @cli.command()
-    @click.option(
-        "-y",
-        "--yes",
-        "--assume-yes",
-        is_flag=True,
-        help="Skip confirmation when deleting a specific model",
-    )
-    def prune(yes: bool):
-        """Remove all saved models locally."""
-        available = [
-            m
-            for t in map(inflection.dasherize, openllm.CONFIG_MAPPING.keys())
-            for m in bentoml.models.list()
-            if t in m.tag.name
-        ]
-
-        for model in available:
-            if yes:
-                delete_confirmed = True
-            else:
-                delete_confirmed = click.confirm(f"delete model {model.tag}?")
-
-            if delete_confirmed:
-                model_store.delete(model.tag)
-                click.echo(f"{model} deleted.")
-
-    @cli.command(name="query")
-    @click.option(
-        "--endpoint",
-        type=click.STRING,
-        help="OpenLLM Server endpoint, i.e: http://localhost:3000",
-        envvar="OPENLLM_ENDPOINT",
-        default="http://localhost:3000",
-    )
-    @click.option("--timeout", type=click.INT, default=30, help="Default server timeout", show_default=True)
-    @click.option(
-        "--server-type", type=click.Choice(["grpc", "http"]), help="Server type", default="http", show_default=True
-    )
-    @output_option
-    @click.argument("query", type=click.STRING)
-    def query_(
-        query: str,
-        endpoint: str,
-        timeout: int,
-        server_type: t.Literal["http", "grpc"],
-        output: OutputLiteral,
-    ):
-        """Ask a LLM interactively, from a terminal.
-
-        $ openllm query --endpoint http://12.323.2.1:3000 "What is the meaning of life?"
-        """
-        if server_type == "grpc":
-            endpoint = re.sub(r"http://", "", endpoint)
-        client = (
-            openllm.client.HTTPClient(endpoint, timeout=timeout)
-            if server_type == "http"
-            else openllm.client.GrpcClient(endpoint, timeout=timeout)
-        )
-
-        if client.framework == "flax":
-            model = openllm.AutoFlaxLLM.for_model(client.model_name)
-        elif client.framework == "tf":
-            model = openllm.AutoTFLLM.for_model(client.model_name)
         else:
-            model = openllm.AutoLLM.for_model(client.model_name)
+            dumped: dict[str, t.Any] = json_data
+            if show_available:
+                assert ids_in_local_store
+                dumped["local"] = [bentoml_cattr.unstructure(i.tag) for m in ids_in_local_store.values() for i in m]
+            _echo(
+                orjson.dumps(
+                    dumped,
+                    option=orjson.OPT_INDENT_2,
+                ).decode(),
+                fg="white",
+            )
 
-        if output != "porcelain":
-            _echo(f"Processing query: {query}\n", fg="white")
+    sys.exit(0)
 
-        res = client.query(query, return_raw_response=True)
 
-        if output == "pretty":
-            formatted = model.postprocess_generate(query, res["responses"])
-            _echo("Responses: ", fg="white", nl=False)
-            _echo(formatted, fg="cyan")
-        elif output == "json":
-            _echo(orjson.dumps(res, option=orjson.OPT_INDENT_2).decode(), fg="white")
+@cli.command()
+@click.option(
+    "-y",
+    "--yes",
+    "--assume-yes",
+    is_flag=True,
+    help="Skip confirmation when deleting a specific model",
+)
+@inject
+def prune(yes: bool, model_store: ModelStore = Provide[BentoMLContainer.model_store]):
+    """Remove all saved models locally."""
+    available = [
+        m
+        for t in map(inflection.dasherize, openllm.CONFIG_MAPPING.keys())
+        for m in bentoml.models.list()
+        if t in m.tag.name
+    ]
+
+    for model in available:
+        if yes:
+            delete_confirmed = True
         else:
-            _echo(res["responses"], fg="white")
+            delete_confirmed = click.confirm(f"delete model {model.tag}?")
 
-    if t.TYPE_CHECKING:
-        assert build and models and start and start_grpc and query_ and prune
+        if delete_confirmed:
+            model_store.delete(model.tag)
+            click.echo(f"{model} deleted.")
 
-    if psutil.WINDOWS:
-        sys.stdout.reconfigure(encoding="utf-8")  # type: ignore
 
-    return cli
+@cli.command(name="query")
+@click.option(
+    "--endpoint",
+    type=click.STRING,
+    help="OpenLLM Server endpoint, i.e: http://localhost:3000",
+    envvar="OPENLLM_ENDPOINT",
+    default="http://localhost:3000",
+)
+@click.option("--timeout", type=click.INT, default=30, help="Default server timeout", show_default=True)
+@click.option(
+    "--server-type", type=click.Choice(["grpc", "http"]), help="Server type", default="http", show_default=True
+)
+@output_option
+@click.argument("query", type=click.STRING)
+def query_(
+    query: str,
+    endpoint: str,
+    timeout: int,
+    server_type: t.Literal["http", "grpc"],
+    output: OutputLiteral,
+):
+    """Ask a LLM interactively, from a terminal.
 
+    $ openllm query --endpoint http://12.323.2.1:3000 "What is the meaning of life?"
+    """
+    if server_type == "grpc":
+        endpoint = re.sub(r"http://", "", endpoint)
+    client = (
+        openllm.client.HTTPClient(endpoint, timeout=timeout)
+        if server_type == "http"
+        else openllm.client.GrpcClient(endpoint, timeout=timeout)
+    )
 
-cli = cli_factory()
+    model = t.cast(
+        "_BaseAutoLLMClass",
+        openllm[client.framework],  # type: ignore (internal API)
+    ).for_model(client.model_name)
+
+    if output != "porcelain":
+        _echo(f"Processing query: {query}\n", fg="white")
+
+    res = client.query(query, return_raw_response=True)
+
+    if output == "pretty":
+        formatted = model.postprocess_generate(query, res["responses"])
+        _echo("Responses: ", fg="white", nl=False)
+        _echo(formatted, fg="cyan")
+    elif output == "json":
+        _echo(orjson.dumps(res, option=orjson.OPT_INDENT_2).decode(), fg="white")
+    else:
+        _echo(res["responses"], fg="white")
 
 
-@cli.command()
+@cli.command(name="download")
 @click.argument(
     "model_name",
     type=click.Choice([inflection.dasherize(name) for name in openllm.CONFIG_MAPPING.keys()]),
 )
 @model_id_option(click)
 @output_option
 def download_models(model_name: str, model_id: str | None, output: OutputLiteral):
     """Setup LLM interactively.
 
     Note: This is useful for development and setup for fine-tune.
     """
+    if output == "porcelain":
+        set_quiet_mode(True)
+        configure_logging()
+
     config = openllm.AutoConfig.for_model(model_name)
-    env = config.__openllm_env__.get_framework_env()
-    if env == "flax":
-        model = openllm.AutoFlaxLLM.for_model(model_name, model_id=model_id, llm_config=config)
-    elif env == "tf":
-        model = openllm.AutoTFLLM.for_model(model_name, model_id=model_id, llm_config=config)
-    else:
-        model = openllm.AutoLLM.for_model(model_name, model_id=model_id, llm_config=config)
+    envvar = config["env"]["framework_value"]
+    model = t.cast(
+        "_BaseAutoLLMClass",
+        openllm[envvar],  # type: ignore (internal API)
+    ).for_model(model_name, model_id=model_id, llm_config=config)
 
-    if len(bentoml.models.list(model.tag)) == 0:
-        if output == "pretty":
-            _echo(f"{model.tag} does not exists yet!. Downloading...", fg="yellow", nl=True)
-        m = model.ensure_model_id_exists()
+    try:
+        _ref = bentoml.transformers.get(model.tag)
         if output == "pretty":
-            _echo(f"Saved model: {m.tag}")
+            _echo(f"{model_name} is already setup for framework '{envvar}': {str(_ref.tag)}", nl=True, fg="yellow")
         elif output == "json":
             _echo(
                 orjson.dumps(
-                    {"previously_setup": False, "framework": env, "tag": str(m.tag)}, option=orjson.OPT_INDENT_2
-                ).decode()
+                    {"previously_setup": True, "framework": envvar, "model": str(_ref.tag)}, option=orjson.OPT_INDENT_2
+                ).decode(),
+                fg="white",
             )
         else:
-            _echo(model.tag)
-    else:
-        m = bentoml.transformers.get(model.tag)
+            if DEBUG or get_debug_mode():
+                # NOTE: When debug is enabled,
+                # We will prefix the tag with __tag__ and we can use regex to correctly
+                # get the tag from 'bentoml.bentos.build|build_bentofile'
+                _echo(f"__tag__:{_ref.tag}", fg="white")
+            else:
+                _echo(_ref.tag, fg="white")
+    except bentoml.exceptions.NotFound:
         if output == "pretty":
-            _echo(f"{model_name} is already setup for framework '{env}': {str(m.tag)}", nl=True, fg="yellow")
+            _echo(
+                f"'{model.__class__.__name__}' with tag '{model.tag}'"
+                " does not exists in local store!. Saving to store...",
+                fg="yellow",
+                nl=True,
+            )
+
+        (model_args, model_attrs), tokenizer_attrs = model.llm_parameters
+        _ref = model.import_model(
+            model.model_id,
+            model.tag,
+            *model_args,
+            tokenizer_kwds=tokenizer_attrs,
+            trust_remote_code=model.__llm_trust_remote_code__,
+            **model_attrs,
+        )
+        if output == "pretty":
+            _echo(f"Saved model: {_ref.tag}")
         elif output == "json":
             _echo(
                 orjson.dumps(
-                    {"previously_setup": True, "framework": env, "model": str(m.tag)}, option=orjson.OPT_INDENT_2
-                ).decode(),
-                fg="white",
+                    {"previously_setup": False, "framework": envvar, "tag": str(_ref.tag)},
+                    option=orjson.OPT_INDENT_2,
+                ).decode()
             )
         else:
-            _echo(m.tag, fg="white")
-    return m
+            if DEBUG or get_debug_mode():
+                # NOTE: When debug is enabled,
+                # We will prefix the tag with __tag__ and we can use regex to correctly
+                # get the tag from 'bentoml.bentos.build|build_bentofile'
+                _echo(f"__tag__:{_ref.tag}")
+            else:
+                _echo(_ref.tag)
+    finally:
+        if is_torch_available() and torch.cuda.is_available():
+            torch.cuda.empty_cache()
+
+    return _ref
+
+
+if psutil.WINDOWS:
+    sys.stdout.reconfigure(encoding="utf-8")  # type: ignore
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `openllm-0.1.5/src/openllm/client.py` & `openllm-0.1.6/src/openllm/client.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/src/openllm/exceptions.py` & `openllm-0.1.6/src/openllm/exceptions.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/src/openllm/models/__init__.py` & `openllm-0.1.6/src/openllm/models/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,9 +13,10 @@
 # limitations under the License.
 
 from . import auto as auto
 from . import chatglm as chatglm
 from . import dolly_v2 as dolly_v2
 from . import falcon as falcon
 from . import flan_t5 as flan_t5
+from . import opt as opt
 from . import stablelm as stablelm
 from . import starcoder as starcoder
```

### Comparing `openllm-0.1.5/src/openllm/models/auto/__init__.py` & `openllm-0.1.6/src/openllm/models/auto/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/src/openllm/models/auto/configuration_auto.py` & `openllm-0.1.6/src/openllm/models/auto/configuration_auto.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,27 +19,35 @@
 from collections import OrderedDict
 
 import inflection
 
 import openllm
 
 if t.TYPE_CHECKING:
+    from collections import _odict_items, _odict_keys, _odict_values
+
     ConfigOrderedDict = OrderedDict[str, type[openllm.LLMConfig]]
+
+    ConfigKeysView = _odict_keys[str, type[openllm.LLMConfig]]
+    ConfigValuesView = _odict_values[str, type[openllm.LLMConfig]]
+    ConfigItemsView = _odict_items[str, type[openllm.LLMConfig]]
 else:
+    ConfigKeysView = ConfigValuesView = ConfigItemsView = t.Any
     ConfigOrderedDict = OrderedDict
 
 # NOTE: This is the entrypoint when adding new model config
 CONFIG_MAPPING_NAMES = OrderedDict(
     [
         ("flan_t5", "FlanT5Config"),
         ("dolly_v2", "DollyV2Config"),
         ("chatglm", "ChatGLMConfig"),
         ("starcoder", "StarCoderConfig"),
         ("falcon", "FalconConfig"),
         ("stablelm", "StableLMConfig"),
+        ("opt", "OPTConfig"),
     ]
 )
 
 
 class _LazyConfigMapping(ConfigOrderedDict):
     def __init__(self, mapping: OrderedDict[str, str]):
         self._mapping = mapping
@@ -59,21 +67,21 @@
             return getattr(self._modules[module_name], value)
 
         # Some of the mappings have entries model_type -> config of another model type. In that case we try to grab the
         # object at the top level.
         return getattr(openllm, value)
 
     def keys(self):
-        return list(self._mapping.keys()) + list(self._extra_content.keys())
+        return t.cast(ConfigKeysView, list(self._mapping.keys()) + list(self._extra_content.keys()))
 
     def values(self):
-        return [self[k] for k in self._mapping.keys()] + list(self._extra_content.values())
+        return t.cast(ConfigValuesView, [self[k] for k in self._mapping.keys()] + list(self._extra_content.values()))
 
     def items(self):
-        return [(k, self[k]) for k in self._mapping.keys()] + list(self._extra_content.items())
+        return t.cast(ConfigItemsView, [(k, self[k]) for k in self._mapping.keys()] + list(self._extra_content.items()))
 
     def __iter__(self):
         return iter(list(self._mapping.keys()) + list(self._extra_content.keys()))
 
     def __contains__(self, item: t.Any):
         return item in self._mapping or item in self._extra_content
 
@@ -83,15 +91,22 @@
         """
         if key in self._mapping.keys():
             raise ValueError(f"'{key}' is already used by a OpenLLM config, pick another name.")
         self._extra_content[key] = value
 
 
 CONFIG_MAPPING: dict[str, type[openllm.LLMConfig]] = _LazyConfigMapping(CONFIG_MAPPING_NAMES)
-CONFIG_NAME_ALIASES: dict[str, str] = {"chat_glm": "chatglm", "stable_lm": "stablelm", "star_coder": "starcoder"}
+
+# The below handle special alias when we call underscore to the name directly
+# without processing camelcase first.
+CONFIG_NAME_ALIASES: dict[str, str] = {
+    "chat_glm": "chatglm",
+    "stable_lm": "stablelm",
+    "star_coder": "starcoder",
+}
 
 
 class AutoConfig:
     def __init__(self, *_: t.Any, **__: t.Any):
         raise EnvironmentError("Cannot instantiate Config. Please use `Config.for_model(model_name)` instead.")
 
     @classmethod
```

### Comparing `openllm-0.1.5/src/openllm/models/auto/factory.py` & `openllm-0.1.6/src/openllm/models/auto/factory.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,31 +11,40 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import importlib
+import logging
 import types
 import typing as t
 from collections import OrderedDict
 
 import inflection
 
 import openllm
 
 from .configuration_auto import AutoConfig
 
 if t.TYPE_CHECKING:
+    from collections import _odict_items, _odict_keys, _odict_values
+
     from ..._llm import LLMRunner
 
     ConfigModelOrderedDict = OrderedDict[type[openllm.LLMConfig], type[openllm.LLM[t.Any, t.Any]]]
+    ConfigModelKeysView = _odict_keys[type[openllm.LLMConfig], type[openllm.LLM[t.Any, t.Any]]]
+    ConfigModelValuesView = _odict_values[type[openllm.LLMConfig], type[openllm.LLM[t.Any, t.Any]]]
+    ConfigModelItemsView = _odict_items[type[openllm.LLMConfig], type[openllm.LLM[t.Any, t.Any]]]
 else:
+    ConfigModelKeysView = ConfigModelValuesView = ConfigModelItemsView = t.Any
     ConfigModelOrderedDict = OrderedDict
 
+logger = logging.getLogger(__name__)
+
 
 class _BaseAutoLLMClass:
     _model_mapping: _LazyAutoMapping
 
     def __init__(self, *args: t.Any, **attrs: t.Any):
         raise EnvironmentError(
             f"Cannot instantiate {self.__class__.__name__} directly. "
@@ -46,68 +55,79 @@
     @classmethod
     def for_model(
         cls,
         model_name: str,
         model_id: str | None = None,
         return_runner_kwargs: t.Literal[False] = ...,
         llm_config: openllm.LLMConfig | None = ...,
+        ensure_available: t.Literal[False, True] = ...,
         **attrs: t.Any,
     ) -> openllm.LLM[t.Any, t.Any]:
         ...
 
     @t.overload
     @classmethod
     def for_model(
         cls,
         model_name: str,
         model_id: str | None = None,
         return_runner_kwargs: t.Literal[True] = ...,
         llm_config: openllm.LLMConfig | None = ...,
+        ensure_available: t.Literal[False, True] = ...,
         **attrs: t.Any,
     ) -> tuple[openllm.LLM[t.Any, t.Any], dict[str, t.Any]]:
         ...
 
     @classmethod
     def for_model(
         cls,
         model_name: str,
         model_id: str | None = None,
         return_runner_kwargs: bool = False,
-        llm_config: openllm.LLMConfig | None = ...,
+        llm_config: openllm.LLMConfig | None = None,
+        ensure_available: bool = False,
         **attrs: t.Any,
     ) -> openllm.LLM[t.Any, t.Any] | tuple[openllm.LLM[t.Any, t.Any], dict[str, t.Any]]:
         """The lower level API for creating a LLM instance.
 
         ```python
         >>> import openllm
         >>> llm = openllm.AutoLLM.for_model("flan-t5")
         ```
         """
-        runner_kwargs_name = [
+        # order matters here
+        runner_kwargs_name = {
             "models",
             "max_batch_size",
             "max_latency_ms",
             "method_configs",
-            "embedded",
             "scheduling_strategy",
-        ]
+        }
         to_runner_attrs = {k: v for k, v in attrs.items() if k in runner_kwargs_name}
-        for k in to_runner_attrs:
-            del attrs[k]
-        if not isinstance(llm_config, openllm.LLMConfig):
-            # The rest of kwargs is now passed to config
-            llm_config = AutoConfig.for_model(model_name, **attrs)
-        if type(llm_config) in cls._model_mapping.keys():
-            llm = cls._model_mapping[type(llm_config)].from_pretrained(model_id, llm_config=llm_config, **attrs)
+        attrs = {k: v for k, v in attrs.items() if k not in to_runner_attrs}
+        if cls._model_mapping.get(inflection.underscore(model_name), None, mapping_type="name2model"):
+            if not isinstance(llm_config, openllm.LLMConfig):
+                # The rest of kwargs is now passed to config
+                llm_config = AutoConfig.for_model(model_name, **attrs)
+                attrs = llm_config.__openllm_extras__
+            # the rest of attrs will be saved to __openllm_extras__
+            llm = cls._model_mapping[type(llm_config)].from_pretrained(
+                model_id,
+                llm_config=llm_config,
+                **llm_config.__openllm_extras__,
+            )
+            if ensure_available:
+                logger.debug("'ensure_available=True', make sure model is available within local store.")
+                llm.ensure_model_id_exists()
             if not return_runner_kwargs:
                 return llm
             return llm, to_runner_attrs
         raise ValueError(
-            f"Unrecognized configuration class {llm_config.__class__} for this kind of AutoRunner: {cls.__name__}.\n"
-            f"Runnable type should be one of {', '.join(c.__name__ for c in cls._model_mapping.keys())}."
+            f"Unrecognized configuration class {llm_config.__class__} for this kind of AutoLLM: {cls.__name__}.\n"
+            f"LLM type should be one of {', '.join(c.__name__ for c in cls._model_mapping.keys())}."
         )
 
     @classmethod
     def create_runner(cls, model_name: str, model_id: str | None = None, **attrs: t.Any) -> LLMRunner:
         """
         Create a LLM Runner for the given model name.
 
@@ -192,52 +212,85 @@
                 model_name = self._model_mapping[mtype]
                 return self._load_attr_from_module(mtype, model_name)
         raise KeyError(key)
 
     def _load_attr_from_module(self, model_type: str, attr: str) -> t.Any:
         module_name = inflection.underscore(model_type)
         if module_name not in self._modules:
-            self._modules[module_name] = openllm.utils.ModelEnv(module_name).module
+            self._modules[module_name] = importlib.import_module(f".{module_name}", "openllm.models")
         return getattribute_from_module(self._modules[module_name], attr)
 
     def keys(self):
         mapping_keys = [
             self._load_attr_from_module(key, name)
             for key, name in self._config_mapping.items()
             if key in self._model_mapping.keys()
         ]
-        return mapping_keys + list(self._extra_content.keys())
+        return t.cast(ConfigModelKeysView, mapping_keys + list(self._extra_content.keys()))
 
-    def get(self, key: openllm.LLMConfig, default: t.Any):
-        try:
-            return self.__getitem__(key)
-        except KeyError:
-            return default
+    @t.overload
+    def get(
+        self, key: type[openllm.LLMConfig], default: t.Any, mapping_type: t.Literal["default"] = "default"
+    ) -> type[openllm.LLM[t.Any, t.Any]]:
+        ...
+
+    @t.overload
+    def get(self, key: str, default: t.Any, mapping_type: t.Literal["name2model", "name2config"] = ...) -> str:
+        ...
+
+    def get(
+        self,
+        key: str | type[openllm.LLMConfig],
+        default: t.Any,
+        mapping_type: t.Literal["default", "name2config", "name2model"] = "default",
+    ) -> str | type[openllm.LLM[t.Any, t.Any]]:
+        _supported = {"default", "name2model", "name2config"}
+        if mapping_type not in _supported:
+            raise RuntimeError(f"Unknown mapping type {mapping_type} (supported: {_supported})")
+
+        if mapping_type == "default":
+            if t.TYPE_CHECKING:
+                # we check for lenient_issubclass below, but pyright is too dumb to understand
+                assert not isinstance(key, str)
+            else:
+                if not openllm.utils.lenient_issubclass(key, openllm.LLMConfig):
+                    raise KeyError(f"Key must be a type of 'openllm.LLMConfig', got {key} instead.")
+            try:
+                return self.__getitem__(key)
+            except KeyError:
+                return default
+        else:
+            mapping = self._model_mapping if mapping_type == "name2model" else self._config_mapping
+            assert isinstance(key, str), f"Key must be a string type if mapping_type={mapping_type}"
+            try:
+                return mapping.__getitem__(key)
+            except KeyError:
+                return default
 
     def __bool__(self):
         return bool(self.keys())
 
     def values(self):
         mapping_values = [
             self._load_attr_from_module(key, name)
             for key, name in self._model_mapping.items()
             if key in self._config_mapping.keys()
         ]
-        return mapping_values + list(self._extra_content.values())
+        return t.cast(ConfigModelValuesView, mapping_values + list(self._extra_content.values()))
 
     def items(self):
         mapping_items = [
             (
                 self._load_attr_from_module(key, self._config_mapping[key]),
                 self._load_attr_from_module(key, self._model_mapping[key]),
             )
             for key in self._model_mapping.keys()
             if key in self._config_mapping.keys()
         ]
-        return mapping_items + list(self._extra_content.items())
+        return t.cast(ConfigModelItemsView, mapping_items + list(self._extra_content.items()))
 
     def __iter__(self):
         return iter(self.keys())
 
     def __contains__(self, item: t.Any):
         if item in self._extra_content:
             return True
```

### Comparing `openllm-0.1.5/src/openllm/models/auto/modeling_auto.py` & `openllm-0.1.6/src/openllm/models/auto/modeling_auto.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     [
         ("flan_t5", "FlanT5"),
         ("dolly_v2", "DollyV2"),
         ("chatglm", "ChatGLM"),
         ("starcoder", "StarCoder"),
         ("falcon", "Falcon"),
         ("stablelm", "StableLM"),
+        ("opt", "OPT"),
     ]
 )
 
 MODEL_MAPPING: dict[
     type[openllm.LLMConfig], type[openllm.LLM[transformers.PreTrainedModel, transformers.PreTrainedTokenizerFast]]
 ] = _LazyAutoMapping(CONFIG_MAPPING_NAMES, MODEL_MAPPING_NAMES)
```

### Comparing `openllm-0.1.5/src/openllm/models/auto/modeling_flax_auto.py` & `openllm-0.1.6/src/openllm/models/auto/modeling_flax_auto.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,20 @@
 from .factory import _BaseAutoLLMClass, _LazyAutoMapping
 
 if t.TYPE_CHECKING:
     import transformers
 
     import openllm
 
-MODEL_FLAX_MAPPING_NAMES = OrderedDict([("flan_t5", "FlaxFlanT5")])
+MODEL_FLAX_MAPPING_NAMES = OrderedDict(
+    [
+        ("flan_t5", "FlaxFlanT5"),
+        ("opt", "FlaxOPT"),
+    ]
+)
 
 MODEL_FLAX_MAPPING: dict[
     type[openllm.LLMConfig], type[openllm.LLM[transformers.FlaxPreTrainedModel, transformers.PreTrainedTokenizerFast]]
 ] = _LazyAutoMapping(CONFIG_MAPPING_NAMES, MODEL_FLAX_MAPPING_NAMES)
 
 
 class AutoFlaxLLM(_BaseAutoLLMClass):
```

### Comparing `openllm-0.1.5/src/openllm/models/auto/modeling_tf_auto.py` & `openllm-0.1.6/src/openllm/models/auto/modeling_tf_auto.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,20 @@
 from .factory import _BaseAutoLLMClass, _LazyAutoMapping
 
 if t.TYPE_CHECKING:
     import transformers
 
     import openllm
 
-MODEL_TF_MAPPING_NAMES = OrderedDict([("flan_t5", "TFFlanT5")])
+MODEL_TF_MAPPING_NAMES = OrderedDict(
+    [
+        ("flan_t5", "TFFlanT5"),
+        ("opt", "TFOPT"),
+    ]
+)
 
 MODEL_TF_MAPPING: dict[
     type[openllm.LLMConfig], type[openllm.LLM[transformers.TFPreTrainedModel, transformers.PreTrainedTokenizerFast]]
 ] = _LazyAutoMapping(CONFIG_MAPPING_NAMES, MODEL_TF_MAPPING_NAMES)
 
 
 class AutoTFLLM(_BaseAutoLLMClass):
```

### Comparing `openllm-0.1.5/src/openllm/models/chatglm/__init__.py` & `openllm-0.1.6/src/openllm/models/chatglm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/src/openllm/models/chatglm/configuration_chatglm.py` & `openllm-0.1.6/src/openllm/models/chatglm/configuration_chatglm.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         "requirements": ["cpm_kernels", "sentencepiece"],
         "default_id": "thudm/chatglm-6b-int4",
         "model_ids": ["thudm/chatglm-6b", "thudm/chatglm-6b-int8", "thudm/chatglm-6b-int4"],
     }
 
     retain_history: bool = openllm.LLMConfig.Field(
         False,
-        description="""Whether to retain history given to the model. 
+        description="""Whether to retain history given to the model.
         If set to True, then the model will retain given history.""",
     )
 
     use_half_precision: bool = openllm.LLMConfig.Field(True, description="Whether to use half precision for model.")
 
     class GenerationConfig:
         max_new_tokens: int = 2048
```

### Comparing `openllm-0.1.5/src/openllm/models/chatglm/modeling_chatglm.py` & `openllm-0.1.6/src/openllm/models/chatglm/modeling_chatglm.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,29 +100,29 @@
         self, prompt: str, generation_result: str, *, chat_history: list[tuple[str, str]] | None = None, **attrs: t.Any
     ):
         if self.config.retain_history:
             assert chat_history is not None, "'retain_history' is True while there is no history provided."
             chat_history.append((prompt, generation_result))
         return "".join(generation_result)
 
-    @torch.inference_mode()
-    def generate(self, prompt: str, use_default_prompt_template: bool = True, **attrs: t.Any) -> str:
-        self.model.eval()
+    def generate(self, prompt: str, **attrs: t.Any) -> str:
+        with torch.inference_mode():
+            self.model.eval()
 
-        # Only use half precision if the model is not yet quantized
-        if self.config.use_half_precision:
-            self.model.half()
+            # Only use half precision if the model is not yet quantized
+            if self.config.use_half_precision:
+                self.model.half()
 
-        self.model.cuda()
+            self.model.cuda()
 
-        logit_processor: list[LogitsProcessor] = LogitsProcessorList()
-        logit_processor.append(InvalidScoreLogitsProcessor())
+            logit_processor: list[LogitsProcessor] = LogitsProcessorList()
+            logit_processor.append(InvalidScoreLogitsProcessor())
 
-        inputs = self.tokenizer([prompt], return_tensors="pt").to(self.device)
-        outputs = self.model.generate(
-            **inputs,
-            generation_config=self.config.model_construct_env(do_sample=True, **attrs).to_generation_config(),
-            logits_processor=logit_processor,
-        )
-        outputs = outputs.tolist()[0][len(inputs["input_ids"][0]) :]
-        response = self.tokenizer.decode(outputs)
-        return self.model.process_response(response)
+            inputs = self.tokenizer([prompt], return_tensors="pt").to(self.device)
+            outputs = self.model.generate(
+                **inputs,
+                generation_config=self.config.model_construct_env(do_sample=True, **attrs).to_generation_config(),
+                logits_processor=logit_processor,
+            )
+            outputs = outputs.tolist()[0][len(inputs["input_ids"][0]) :]
+            response = self.tokenizer.decode(outputs)
+            return self.model.process_response(response)
```

### Comparing `openllm-0.1.5/src/openllm/models/dolly_v2/__init__.py` & `openllm-0.1.6/src/openllm/models/dolly_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/src/openllm/models/dolly_v2/configuration_dolly_v2.py` & `openllm-0.1.6/src/openllm/models/dolly_v2/configuration_dolly_v2.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     Refer to [Databricks's Dolly page](https://github.com/databrickslabs/dolly) for more information.
     """
 
     __config__ = {
         "timeout": 3600000,
         "trust_remote_code": True,
         "url": "https://github.com/databrickslabs/dolly",
+        "use_pipeline": True,
         "default_id": "databricks/dolly-v2-3b",
         "model_ids": ["databricks/dolly-v2-3b", "databricks/dolly-v2-7b", "databricks/dolly-v2-12b"],
     }
 
     return_full_text: bool = openllm.LLMConfig.Field(
         False, description="Whether to return the full prompt to the users."
     )
```

### Comparing `openllm-0.1.5/src/openllm/models/dolly_v2/modeling_dolly_v2.py` & `openllm-0.1.6/src/openllm/models/dolly_v2/modeling_dolly_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,23 +94,23 @@
         return prompt, generate_kwargs, {}
 
     def postprocess_generate(
         self, prompt: str, generation_result: list[dict[t.Literal["generated_text"], str]], **_: t.Any
     ) -> str:
         return generation_result[0]["generated_text"]
 
-    @torch.inference_mode()
     def generate(self, prompt: str, **attrs: t.Any) -> list[dict[t.Literal["generated_text"], str]]:
-        self.model.tokenizer = self.tokenizer
-        llm_config = self.config.model_construct_env(**attrs)
-        decoded: list[dict[t.Literal["generated_text"], str]] = self.model(
-            prompt, generation_config=llm_config.to_generation_config()
-        )
+        with torch.inference_mode():
+            self.model.tokenizer = self.tokenizer
+            llm_config = self.config.model_construct_env(**attrs)
+            decoded: list[dict[t.Literal["generated_text"], str]] = self.model(
+                prompt, generation_config=llm_config.to_generation_config()
+            )
 
-        if llm_config.return_full_text:
-            return [
-                {k: f"{DEFAULT_PROMPT_TEMPLATE.format(instruction=prompt)}\n{generated}"}
-                for i in decoded
-                for k, generated in i.items()
-            ]
+            if llm_config.return_full_text:
+                return [
+                    {k: f"{DEFAULT_PROMPT_TEMPLATE.format(instruction=prompt)}\n{generated}"}
+                    for i in decoded
+                    for k, generated in i.items()
+                ]
 
-        return decoded
+            return decoded
```

### Comparing `openllm-0.1.5/src/openllm/models/falcon/__init__.py` & `openllm-0.1.6/src/openllm/models/falcon/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/src/openllm/models/falcon/configuration_falcon.py` & `openllm-0.1.6/src/openllm/models/falcon/configuration_falcon.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     """
 
     __config__ = {
         "name_type": "lowercase",
         "trust_remote_code": True,
         "requires_gpu": True,
         "timeout": int(36e6),
+        "use_pipeline": True,
         "url": "https://falconllm.tii.ae/",
         "requirements": ["einops", "xformers", "safetensors"],
         "default_id": "tiiuae/falcon-7b",
         "model_ids": [
             "tiiuae/falcon-7b",
             "tiiuae/falcon-40b",
             "tiiuae/falcon-7b-instruct",
```

### Comparing `openllm-0.1.5/src/openllm/models/falcon/modeling_falcon.py` & `openllm-0.1.6/src/openllm/models/falcon/modeling_falcon.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/src/openllm/models/flan_t5/__init__.py` & `openllm-0.1.6/src/openllm/models/flan_t5/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/src/openllm/models/flan_t5/configuration_flan_t5.py` & `openllm-0.1.6/src/openllm/models/flan_t5/configuration_flan_t5.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
         "model_ids": [
             "google/flan-t5-small",
             "google/flan-t5-base",
             "google/flan-t5-large",
             "google/flan-t5-xl",
             "google/flan-t5-xxl",
         ],
+        "model_type": "seq2seq_lm",
     }
 
     class GenerationConfig:
         temperature: float = 0.9
         max_new_tokens: int = 2048
         top_k: int = 50
         top_p: float = 0.4
```

### Comparing `openllm-0.1.5/src/openllm/models/flan_t5/modeling_flan_t5.py` & `openllm-0.1.6/src/openllm/models/flan_t5/modeling_flan_t5.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,18 +70,18 @@
             "repetition_penalty": repetition_penalty,
         }
         return prompt_text, generation_config, {}
 
     def postprocess_generate(self, prompt: str, generation_result: t.Sequence[str], **_: t.Any) -> str:
         return generation_result[0]
 
-    @torch.inference_mode()
     def generate(self, prompt: str, **attrs: t.Any) -> list[str]:
-        if torch.cuda.is_available():
-            self.model.cuda()
-        input_ids = t.cast("torch.Tensor", self.tokenizer(prompt, return_tensors="pt").input_ids).to(self.device)
-        result_tensor = self.model.generate(
-            input_ids,
-            do_sample=True,
-            generation_config=self.config.model_construct_env(**attrs).to_generation_config(),
-        )
-        return self.tokenizer.batch_decode(result_tensor, skip_special_tokens=True)
+        with torch.inference_mode():
+            if torch.cuda.is_available():
+                self.model.cuda()
+            input_ids = t.cast("torch.Tensor", self.tokenizer(prompt, return_tensors="pt").input_ids).to(self.device)
+            result_tensor = self.model.generate(
+                input_ids,
+                do_sample=True,
+                generation_config=self.config.model_construct_env(**attrs).to_generation_config(),
+            )
+            return self.tokenizer.batch_decode(result_tensor, skip_special_tokens=True)
```

### Comparing `openllm-0.1.5/src/openllm/models/flan_t5/modeling_flax_flan_t5.py` & `openllm-0.1.6/src/openllm/models/flan_t5/modeling_flax_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/src/openllm/models/flan_t5/modeling_tf_flan_t5.py` & `openllm-0.1.6/src/openllm/models/flan_t5/modeling_tf_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/src/openllm/models/gpt_neox/__init__.py` & `openllm-0.1.6/src/openllm/models/gpt_neox/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/src/openllm/models/gptj/__init__.py` & `openllm-0.1.6/src/openllm/models/llama/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/src/openllm/models/llama/__init__.py` & `openllm-0.1.6/src/openllm/models/roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/src/openllm/models/roberta/__init__.py` & `openllm-0.1.6/src/openllm_client/runtimes/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,8 +8,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-raise NotImplementedError("This module is not implemented yet.")
+from .grpc import GrpcClient as GrpcClient
+from .http import HTTPClient as HTTPClient
```

### Comparing `openllm-0.1.5/src/openllm/models/stablelm/__init__.py` & `openllm-0.1.6/src/openllm/models/stablelm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/src/openllm/models/stablelm/configuration_stablelm.py` & `openllm-0.1.6/src/openllm/models/stablelm/configuration_stablelm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/src/openllm/models/stablelm/modeling_stablelm.py` & `openllm-0.1.6/src/openllm/models/stablelm/modeling_stablelm.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,21 +43,20 @@
 
 
 class StableLM(openllm.LLM["transformers.GPTNeoXForCausalLM", "transformers.GPTNeoXTokenizerFast"]):
     __openllm_internal__ = True
 
     def llm_post_init(self):
         self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-        self.load_in_mha = True if not torch.cuda.is_available() else False
+        self.bettertransformer = True if not torch.cuda.is_available() else False
 
     @property
     def import_kwargs(self):
         model_kwds = {
             "torch_dtype": torch.float16 if torch.cuda.is_available() else torch.float32,
-            "load_in_8bit": False,
             "device_map": "auto" if torch.cuda.is_available() and torch.cuda.device_count() > 1 else None,
         }
         tokenizer_kwds: dict[str, t.Any] = {}
         return model_kwds, tokenizer_kwds
 
     def sanitize_parameters(
         self,
```

### Comparing `openllm-0.1.5/src/openllm/models/starcoder/__init__.py` & `openllm-0.1.6/src/openllm/models/starcoder/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/src/openllm/models/starcoder/configuration_starcoder.py` & `openllm-0.1.6/src/openllm/models/starcoder/configuration_starcoder.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/src/openllm/models/starcoder/modeling_starcoder.py` & `openllm-0.1.6/src/openllm/models/starcoder/modeling_starcoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,42 +43,40 @@
     def llm_post_init(self):
         self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
     @property
     def import_kwargs(self):
         model_kwds = {
             "device_map": "auto" if torch.cuda.is_available() and torch.cuda.device_count() > 1 else None,
-            "load_in_8bit": True if torch.cuda.device_count() > 1 else False,
-            "torch_dtype": torch.float16,
+            "torch_dtype": torch.float16 if torch.cuda.is_available() else torch.float32,
         }
         tokenizer_kwds = {"padding_side": "left"}
         return model_kwds, tokenizer_kwds
 
     def import_model(
         self,
         model_id: str,
         tag: bentoml.Tag,
         *model_args: t.Any,
         tokenizer_kwds: dict[str, t.Any],
         **attrs: t.Any,
     ) -> bentoml.Model:
         torch_dtype = attrs.pop("torch_dtype", torch.float16)
-        load_in_8bit = attrs.pop("load_in_8bit", True)
         device_map = attrs.pop("device_map", "auto")
 
         tokenizer = transformers.AutoTokenizer.from_pretrained(model_id, **tokenizer_kwds)
         tokenizer.add_special_tokens(
             {
                 "additional_special_tokens": [EOD, FIM_PREFIX, FIM_MIDDLE, FIM_SUFFIX, FIM_PAD],
                 "pad_token": EOD,
             }
         )
 
         model = transformers.AutoModelForCausalLM.from_pretrained(
-            model_id, torch_dtype=torch_dtype, load_in_8bit=load_in_8bit, device_map=device_map, **attrs
+            model_id, torch_dtype=torch_dtype, device_map=device_map, **attrs
         )
         try:
             return bentoml.transformers.save_model(tag, model, custom_objects={"tokenizer": tokenizer})
         finally:
             import gc
 
             # NOTE: We need to free the cache after saving here so that we can load it back later on.
@@ -118,22 +116,24 @@
         }
 
         return prompt_text, generation_config, {}
 
     def postprocess_generate(self, prompt: str, generation_result: t.Sequence[str], **_: t.Any) -> str:
         return generation_result[0]
 
-    @torch.inference_mode()
     def generate(self, prompt: str, **attrs: t.Any) -> list[str]:
-        inputs = t.cast("torch.Tensor", self.tokenizer.encode(prompt, return_tensors="pt")).to(self.device)
-        result_tensor = self.model.generate(
-            inputs,
-            do_sample=True,
-            pad_token_id=self.tokenizer.eos_token_id,
-            # eos_token_id=self.tokenizer.convert_tokens_to_ids("<|end|>"), # NOTE: this is for finetuning starcoder
-            generation_config=self.config.model_construct_env(**attrs).to_generation_config(),
-        )
-        # TODO: We will probably want to return the tokenizer here so that we can manually process this
-        # return (skip_special_tokens=False, clean_up_tokenization_spaces=False))
-        return self.tokenizer.batch_decode(
-            result_tensor[0], skip_special_tokens=True, clean_up_tokenization_spaces=True
-        )
+        with torch.inference_mode():
+            inputs = t.cast("torch.Tensor", self.tokenizer.encode(prompt, return_tensors="pt")).to(self.device)
+            result_tensor = self.model.generate(
+                inputs,
+                do_sample=True,
+                pad_token_id=self.tokenizer.eos_token_id,
+                # eos_token_id=self.tokenizer.convert_tokens_to_ids("<|end|>"), # NOTE: this is for finetuning starcoder
+                generation_config=self.config.model_construct_env(**attrs).to_generation_config(),
+            )
+            # TODO: We will probably want to return the tokenizer here so that we can manually process this
+            # return (skip_special_tokens=False, clean_up_tokenization_spaces=False))
+            return self.tokenizer.batch_decode(
+                result_tensor[0],
+                skip_special_tokens=True,
+                clean_up_tokenization_spaces=True,
+            )
```

### Comparing `openllm-0.1.5/src/openllm/utils/analytics.py` & `openllm-0.1.6/src/openllm/utils/analytics.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 @attr.define
 class StartInitEvent(_internal_analytics.schemas.EventMeta):
     model_name: str
     llm_config: t.Dict[str, t.Any] = attr.field(default=None)
 
     @staticmethod
     def handler(llm_config: openllm.LLMConfig) -> StartInitEvent:
-        return StartInitEvent(model_name=llm_config.__openllm_model_name__, llm_config=llm_config.model_dump())
+        return StartInitEvent(model_name=llm_config["model_name"], llm_config=llm_config.model_dump())
 
 
 def track_start_init(
     llm_config: openllm.LLMConfig,
 ):
     if do_not_track():
         return
```

### Comparing `openllm-0.1.5/src/openllm/utils/codegen.py` & `openllm-0.1.6/src/openllm/utils/codegen.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/src/openllm/utils/dantic.py` & `openllm-0.1.6/src/openllm/utils/dantic.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         multiple=allows_multiple(typ),
         help=field.metadata.get("description", "(No description provided)"),
         show_envvar=True,
         envvar=envvar,
     )
 
 
-def _default_converter(value: t.Any, env: str | None) -> t.Any:
+def env_converter(value: t.Any, env: str | None = None) -> t.Any:
     if env is not None:
         value = os.environ.get(env, value)
     if value is not None and isinstance(value, str):
         try:
             return orjson.loads(value.lower())
         except orjson.JSONDecodeError as err:
             raise RuntimeError(f"Failed to parse '{value}' from '{env}': {err}")
@@ -131,28 +131,29 @@
         description: the documentation for the field. Defaults to None.
         env: the environment variable to read from. Defaults to None.
         auto_default: a bool indicating whether to use the default value as the environment.
             Defaults to False. If set to True, the behaviour of this Field will also depends
             on kw_only. If kw_only=True, the this field will become 'Required' and the default
             value is omitted. If kw_only=False, then the default value will be used as before.
         use_default_converter: a bool indicating whether to use the default converter. Defaults
-            to True. If set to False, then the default converter will not be used.
+            to True. If set to False, then the default converter will not be used. The default
+            converter converts a given value from the environment variable for this given Field.
         **kwargs: The rest of the arguments are passed to attr.field
     """
     metadata = attrs.pop("metadata", {})
     if description is None:
         description = "(No description provided)"
     metadata["description"] = description
     if env is not None:
         metadata["env"] = env
     piped: list[_ValidatorType[t.Any]] = []
 
     converter = attrs.pop("converter", None)
     if use_default_converter:
-        converter = functools.partial(_default_converter, env=env)
+        converter = functools.partial(env_converter, env=env)
 
     if ge is not None:
         piped.append(attr.validators.ge(ge))
     if le is not None:
         piped.append(attr.validators.le(le))
     if validator is not None:
         piped.append(validator)
```

### Comparing `openllm-0.1.5/src/openllm/utils/dummy_flax_objects.py` & `openllm-0.1.6/src/openllm/utils/dummy_flax_objects.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,14 +22,21 @@
 class FlaxFlanT5(metaclass=DummyMetaclass):
     _backends = ["flax"]
 
     def __init__(self, *args: t.Any, **attrs: t.Any):
         require_backends(self, ["flax"])
 
 
+class FlaxOPT(metaclass=DummyMetaclass):
+    _backends = ["flax"]
+
+    def __init__(self, *args: t.Any, **attrs: t.Any):
+        require_backends(self, ["flax"])
+
+
 class AutoFlaxLLM(metaclass=DummyMetaclass):
     _backends = ["flax"]
 
     def __init__(self, *args: t.Any, **attrs: t.Any):
         require_backends(self, ["flax"])
```

### Comparing `openllm-0.1.5/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py` & `openllm-0.1.6/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/src/openllm/utils/dummy_pt_and_einops_objects.py` & `openllm-0.1.6/src/openllm/utils/dummy_pt_and_einops_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/src/openllm/utils/dummy_pt_objects.py` & `openllm-0.1.6/src/openllm/utils/dummy_pt_objects.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,14 +22,21 @@
 class FlanT5(metaclass=DummyMetaclass):
     _backends = ["torch"]
 
     def __init__(self, *args: t.Any, **attrs: t.Any):
         require_backends(self, ["torch"])
 
 
+class OPT(metaclass=DummyMetaclass):
+    _backends = ["torch"]
+
+    def __init__(self, *args: t.Any, **attrs: t.Any):
+        require_backends(self, ["torch"])
+
+
 class DollyV2(metaclass=DummyMetaclass):
     _backends = ["torch"]
 
     def __init__(self, *args: t.Any, **attrs: t.Any):
         require_backends(self, ["torch"])
```

### Comparing `openllm-0.1.5/src/openllm/utils/dummy_tf_objects.py` & `openllm-0.1.6/src/openllm/utils/dummy_tf_objects.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,14 +22,21 @@
 class TFFlanT5(metaclass=DummyMetaclass):
     _backends = ["tf"]
 
     def __init__(self, *args: t.Any, **attrs: t.Any):
         require_backends(self, ["tf"])
 
 
+class TFOPT(metaclass=DummyMetaclass):
+    _backends = ["tf"]
+
+    def __init__(self, *args: t.Any, **attrs: t.Any):
+        require_backends(self, ["tf"])
+
+
 class AutoTFLLM(metaclass=DummyMetaclass):
     _backends = ["tf"]
 
     def __init__(self, *args: t.Any, **attrs: t.Any):
         require_backends(self, ["tf"])
```

### Comparing `openllm-0.1.5/src/openllm/utils/import_utils.py` & `openllm-0.1.6/src/openllm/utils/import_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,24 +11,25 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Some imports utils are vendorred from transformers/utils/import_utils.py for performance reasons.
 """
+from __future__ import annotations
+
 import importlib
 import importlib.metadata
 import importlib.util
 import logging
 import os
 import typing as t
 from abc import ABCMeta
 from collections import OrderedDict
 
-import attr
 import inflection
 from bentoml._internal.utils import LazyLoader
 from packaging import version
 
 if t.TYPE_CHECKING:
     BackendOrderredDict = OrderedDict[str, tuple[t.Callable[[], bool], str]]
 else:
@@ -57,24 +58,29 @@
 
 
 _torch_available = importlib.util.find_spec("torch") is not None
 _tf_available = importlib.util.find_spec("tensorflow") is not None
 _flax_available = importlib.util.find_spec("jax") is not None and importlib.util.find_spec("flax") is not None
 _einops_available = _is_package_available("einops")
 _cpm_kernel_available = _is_package_available("cpm_kernels")
+_bitsandbytes_available = _is_package_available("bitsandbytes")
 
 
 def is_einops_available():
     return _einops_available
 
 
 def is_cpm_kernels_available():
     return _cpm_kernel_available
 
 
+def is_bitsandbytes_available():
+    return _bitsandbytes_available
+
+
 def is_torch_available():
     global _torch_available
     if USE_TORCH in ENV_VARS_TRUE_AND_AUTO_VALUES and USE_TF not in ENV_VARS_TRUE_VALUES:
         if _torch_available:
             try:
                 importlib.metadata.version("torch")
             except importlib.metadata.PackageNotFoundError:
@@ -227,46 +233,82 @@
 
     checks = (BACKENDS_MAPPING[backend] for backend in backends)
     failed = [msg.format(name) for available, msg in checks if not available()]
     if failed:
         raise ImportError("".join(failed))
 
 
-@attr.define
 class ModelEnv:
-    model_name: str = attr.field(converter=inflection.underscore)
-
-    @property
-    def framework(self) -> str:
-        return f"OPENLLM_{self.model_name.upper()}_FRAMEWORK"
-
-    @property
-    def model_config(self) -> str:
-        return f"OPENLLM_{self.model_name.upper()}_CONFIG"
-
-    @property
-    def model_id(self) -> str:
-        return f"OPENLLM_{self.model_name.upper()}_MODEL_ID"
+    model_name: str
 
-    @property
-    def bettertransformer(self) -> str:
-        return f"OPENLLM_{self.model_name.upper()}_BETTERTRANSFORMER"
+    if t.TYPE_CHECKING:
+        config: property
+        model_id: property
+        quantize: property
+        framework: property
+        bettertransformer: property
+
+        framework_value: property
+        quantize_value: property
+        bettertransformer_value: property
+
+    def __getitem__(self, item: str | t.Any) -> t.Any:
+        if hasattr(self, item):
+            return getattr(self, item)
+        raise KeyError(f"Key {item} not found in {self}")
+
+    def __new__(cls, model_name: str, bettertransformer: bool | None = None, quantize: t.LiteralString | None = None):
+        from .._configuration import _field_env_key
+        from . import codegen
+
+        model_name = inflection.underscore(model_name)
+
+        res = super().__new__(cls)
+        res.model_name = model_name
+
+        # gen properties env key
+        attributes = {"config", "model_id", "quantize", "framework", "bettertransformer"}
+        for att in attributes:
+            setattr(res, att, _field_env_key(model_name, att.upper()))
+
+        # gen properties env value
+        attributes_with_values = {
+            "quantize": (bool, quantize),
+            "bettertransformer": (bool, bettertransformer),
+            "framework": (str, "pt"),
+        }
+        globs: dict[str, t.Any] = {
+            "__bool_vars_value": ENV_VARS_TRUE_VALUES,
+            "__env_get": os.environ.get,
+            "self": res,
+        }
+
+        for attribute, (default_type, default_value) in attributes_with_values.items():
+            lines: list[str] = []
+            if default_type is bool:
+                lines.append(
+                    f"return str(__env_get(self['{attribute}'], str(__env_default)).upper() in __bool_vars_value)"
+                )
+            else:
+                lines.append(f"return __env_get(self['{attribute}'], __env_default)")
 
-    def gen_env_key(self, key: str) -> str:
-        return f"OPENLLM_{self.model_name.upper()}_{key.upper()}"
+            setattr(
+                res,
+                f"{attribute}_value",
+                codegen.generate_function(
+                    cls,
+                    "_env_get_" + attribute,
+                    lines,
+                    ("__env_default",),
+                    globs,
+                )(default_value),
+            )
 
-    def convert_to_bettertransformer(self) -> bool:
-        return os.environ.get(self.bettertransformer, str(False)).lower() == "true"
+        return res
 
     @property
     def start_docstring(self) -> str:
         return getattr(self.module, f"START_{self.model_name.upper()}_COMMAND_DOCSTRING")
 
     @property
     def module(self) -> LazyLoader:
         return LazyLoader(self.model_name, globals(), f"openllm.models.{self.model_name}")
-
-    def get_framework_env(self) -> t.Literal["pt", "flax", "tf"]:
-        envvar = os.environ.get(self.framework, "pt")
-        if envvar not in ("pt", "tf", "flax"):
-            raise ValueError(f"Invalid framework implementation {envvar}, must be one of 'pt', 'tf', 'flax'")
-        return envvar
```

### Comparing `openllm-0.1.5/src/openllm/utils/lazy.py` & `openllm-0.1.6/src/openllm/utils/lazy.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,14 +17,27 @@
 import importlib
 import importlib.machinery
 import itertools
 import os
 import types
 import typing as t
 
+from ..exceptions import ForbiddenAttributeError, OpenLLMException
+
+
+class UsageNotAllowedError(OpenLLMException):
+    """Raised when LazyModule.__getitem__ is forbidden."""
+
+
+class MissingAttributesError(OpenLLMException):
+    """Raised when given keys is not available in LazyModule special mapping."""
+
+
+_reserved_namespace = {"__openllm_special__"}
+
 
 class LazyModule(types.ModuleType):
     """
     Module class that surfaces all objects but only performs associated imports when the objects are requested.
     This is a direct port from transformers.utils.import_utils._LazyModule for
     backwards compatibility with transformers < 4.18
 
@@ -40,23 +53,24 @@
         import_structure: dict[str, list[str]],
         module_spec: importlib.machinery.ModuleSpec | None = None,
         extra_objects: dict[str, t.Any] | None = None,
     ):
         super().__init__(name)
         self._modules = set(import_structure.keys())
         self._class_to_module: dict[str, str] = {}
+        _extra_objects = {} if extra_objects is None else extra_objects
         for key, values in import_structure.items():
             for value in values:
                 self._class_to_module[value] = key
         # Needed for autocompletion in an IDE
         self.__all__ = list(import_structure.keys()) + list(itertools.chain(*import_structure.values()))
         self.__file__ = module_file
         self.__spec__ = module_spec
         self.__path__ = [os.path.dirname(module_file)]
-        self._objects = {} if extra_objects is None else extra_objects
+        self._objects = _extra_objects
         self._name = name
         self._import_structure = import_structure
 
     # Needed for autocompletion in an IDE
     def __dir__(self):
         result = t.cast("list[str]", super().__dir__())
         # The elements of self.__all__ that are submodules may or
@@ -64,21 +78,38 @@
         # they have been accessed or not. So we only add the
         # elements of self.__all__ that are not already in the dir.
         for attribute in self.__all__:
             if attribute not in result:
                 result.append(attribute)
         return result
 
+    def __getitem__(self, key: str) -> t.Any:
+        if self._objects.get("__openllm_special__") is None:
+            raise UsageNotAllowedError(f"'{self._name}' is not allowed to be used as a dict.")
+        _special_mapping = self._objects.get("__openllm_special__", {})
+        try:
+            if key in _special_mapping:
+                return getattr(self, _special_mapping.__getitem__(key))
+            raise MissingAttributesError(f"Requested '{key}' is not available in given mapping.")
+        except AttributeError as e:
+            raise KeyError(f"'{self._name}' has no attribute {_special_mapping[key]}") from e
+        except Exception as e:
+            raise KeyError(f"Failed to lookup '{key}' in '{self._name}'") from e
+
     def __getattr__(self, name: str) -> t.Any:
+        if name in _reserved_namespace:
+            raise ForbiddenAttributeError(
+                f"'{name}' is a reserved namespace for {self._name} and should not be access nor modified."
+            )
         if name in self._objects:
-            return self._objects[name]
+            return self._objects.__getitem__(name)
         if name in self._modules:
             value = self._get_module(name)
         elif name in self._class_to_module.keys():
-            module = self._get_module(self._class_to_module[name])
+            module = self._get_module(self._class_to_module.__getitem__(name))
             value = getattr(module, name)
         else:
             raise AttributeError(f"module {self.__name__} has no attribute {name}")
 
         setattr(self, name, value)
         return value
```

### Comparing `openllm-0.1.5/src/openllm_client/__init__.py` & `openllm-0.1.6/src/openllm_client/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/src/openllm_client/_prompt.py` & `openllm-0.1.6/src/openllm_client/_prompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
-import dataclasses
 import typing as t
 
+import attr
+
 import openllm
 from openllm._prompt import PromptFormatter
 
 if t.TYPE_CHECKING:
     DictStrStr = dict[str, str]
 else:
     DictStrStr = dict
@@ -30,21 +31,19 @@
 
 
 class PartialDict(DictStrStr):
     def __missing__(self, key: str):
         return "{" + key + "}"
 
 
-@dataclasses.dataclass(slots=True)
+@attr.define(slots=True)
 class PromptTemplate:
     template: str
     input_variables: t.Sequence[str]
 
-    model_config = {"extra": "forbid"}
-
     def to_str(self, __partial_dict__: PartialDict | None = None, **attrs: str) -> str:
         """Generate a prompt from the template and input variables"""
         if __partial_dict__:
             return _default_formatter.vformat(self.template, (), __partial_dict__)
         if not attrs:
             raise ValueError("Keyword arguments are required")
         if not all(k in attrs for k in self.input_variables):
```

### Comparing `openllm-0.1.5/src/openllm_client/cache/__init__.py` & `openllm-0.1.6/examples/langchain-chains-demo/download_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,11 +7,7 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-"""
-Cache utilities for OpenLLM client.
-"""
```

### Comparing `openllm-0.1.5/src/openllm_client/cache/inmemory.py` & `openllm-0.1.6/examples/langchain-tools-demo/download_model.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/src/openllm_client/runtimes/__init__.py` & `openllm-0.1.6/src/openllm/playground/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,10 +7,7 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-from .grpc import GrpcClient as GrpcClient
-from .http import HTTPClient as HTTPClient
```

### Comparing `openllm-0.1.5/src/openllm_client/runtimes/base.py` & `openllm-0.1.6/src/openllm_client/runtimes/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 import bentoml
 import httpx
 
 import openllm
 
 if t.TYPE_CHECKING:
+    from openllm.models.auto.factory import _BaseAutoLLMClass
 
     class AnnotatedClient(bentoml.client.Client):
         def health(self, *args: t.Any, **attrs: t.Any) -> t.Any:
             ...
 
         async def async_health(self) -> t.Any:
             ...
@@ -103,20 +104,18 @@
     @abstractmethod
     def configuration(self) -> dict[str, t.Any]:
         raise NotImplementedError
 
     @property
     def llm(self) -> openllm.LLM[t.Any, t.Any]:
         if self.__llm__ is None:
-            if self.framework == "flax":
-                self.__llm__ = openllm.AutoFlaxLLM.for_model(self.model_name)
-            elif self.framework == "tf":
-                self.__llm__ = openllm.AutoTFLLM.for_model(self.model_name)
-            else:
-                self.__llm__ = openllm.AutoLLM.for_model(self.model_name)
+            self.__llm__ = t.cast(
+                "_BaseAutoLLMClass",
+                openllm[self.framework],  # type: ignore (internal API)
+            ).for_model(self.model_name)
         return self.__llm__
 
     @property
     def config(self) -> openllm.LLMConfig:
         return self.llm.config
 
     def call(self, name: str, *args: t.Any, **attrs: t.Any) -> t.Any:
```

### Comparing `openllm-0.1.5/src/openllm_client/runtimes/grpc.py` & `openllm-0.1.6/src/openllm_client/runtimes/grpc.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/src/openllm_client/runtimes/http.py` & `openllm-0.1.6/src/openllm_client/runtimes/http.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/tests/__init__.py` & `openllm-0.1.6/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/tests/test_configuration.py` & `openllm-0.1.6/tests/test_configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,27 +19,28 @@
 import logging
 
 import pytest
 from hypothesis import assume, given
 from hypothesis import strategies as st
 
 import openllm
-from openllm._configuration import GenerationConfig, ModelSettings, _field_env_key
+from openllm._configuration import (GenerationConfig, ModelSettings,
+                                    _field_env_key)
 from openllm.utils import DEBUG
 
 from ._strategies._configuration import make_llm_config, model_settings
 
 logger = logging.getLogger(__name__)
 
 
 def test_missing_default():
-    with pytest.raises(ValueError, match="The following keys are required*"):
+    with pytest.raises(ValueError, match="Either 'default_id' or 'model_ids'*"):
         make_llm_config("MissingDefaultId", {"name_type": "lowercase", "requirements": ["bentoml"]})
 
-    with pytest.raises(ValueError, match="The following keys are required*"):
+    with pytest.raises(ValueError, match="Either 'default_id' or 'model_ids'*"):
         make_llm_config("MissingModelId", {"default_id": "huggingface/t5-tiny-testing", "requirements": ["bentoml"]})
 
 
 def test_forbidden_access():
     cl_ = make_llm_config(
         "ForbiddenAccess",
         {
@@ -63,15 +64,15 @@
     )
 
     assert openllm.utils.lenient_issubclass(cl_.__openllm_generation_class__, GenerationConfig)
 
 
 @given(model_settings())
 def test_class_normal_gen(gen_settings: ModelSettings):
-    assume(gen_settings["default_id"] and gen_settings["model_ids"])
+    assume(gen_settings["default_id"] and all(i for i in gen_settings["model_ids"]))
     cl_: type[openllm.LLMConfig] = make_llm_config("NotFullLLM", gen_settings)
     assert issubclass(cl_, openllm.LLMConfig)
     for key in gen_settings:
         assert object.__getattribute__(cl_, f"__openllm_{key}__") == gen_settings.__getitem__(key)
 
 
 @given(model_settings(), st.integers())
```

### Comparing `openllm-0.1.5/tests/_strategies/__init__.py` & `openllm-0.1.6/tests/_strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/tests/_strategies/_configuration.py` & `openllm-0.1.6/tests/_strategies/_configuration.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,14 +33,17 @@
     kwargs: dict[str, t.Any] = dict(
         default_id=st.text(min_size=1),
         model_ids=st.lists(st.text(), min_size=1),
         url=st.text(),
         requires_gpu=st.booleans(),
         trust_remote_code=st.booleans(),
         requirements=st.none() | st.lists(st.text(), min_size=1),
+        use_pipeline=st.booleans(),
+        model_type=st.sampled_from(["causal_lm", "seq2seq_lm"]),
+        runtime=st.sampled_from(["transformers", "cpp"]),
         name_type=st.sampled_from(["dasherize", "lowercase"]),
         timeout=st.integers(min_value=3600),
         workers_per_resource=st.one_of(st.integers(min_value=1), st.floats(min_value=0.1, max_value=1.0)),
     )
     return draw(st.builds(ModelSettings, **kwargs))
```

### Comparing `openllm-0.1.5/tests/models/flan_t5/__init__.py` & `openllm-0.1.6/tests/models/flan_t5/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/tests/models/flan_t5/test_modeling_flan_t5.py` & `openllm-0.1.6/tests/models/flan_t5/test_modeling_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/tools/assert-model-table-latest` & `openllm-0.1.6/tools/assert-model-table-latest`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 #!/usr/bin/env python3
 
 from __future__ import annotations
 
 import os
+import subprocess
 
 from markdown_it import MarkdownIt
 
-import openllm
-
 md = MarkdownIt()
 
 ROOT = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 with open(os.path.join(ROOT, "README.md"), "r") as f:
     readme = md.parse(f.read())
 
 # NOTE: Currently, we only have one table in README, which is the Model readme.
 table = [r for r in readme if r.type == "html_block" and r.content.startswith("<td><a")]
 
-available = len(openllm.CONFIG_MAPPING.keys())
+available = subprocess.check_output(["openllm", "models", "-o", "porcelain"]).strip().decode("utf-8").count("\n") + 1
 
 on_table = len(table)  # NOTE: minus the header
 
 if available - on_table != 0:
     print("README.md is out of date! Make sure to run ./tools/update-readme.py")
     raise SystemExit(1)
 raise SystemExit(0)
```

### Comparing `openllm-0.1.5/tools/run-release-action` & `openllm-0.1.6/tools/run-release-action`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/tools/update-optional-dependencies.py` & `openllm-0.1.6/tools/update-optional-dependencies.py`

 * *Files 23% similar despite different names*

```diff
@@ -22,32 +22,42 @@
 import inflection
 import tomlkit
 
 import openllm
 
 ROOT = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 
-FINE_TUNE_DEPS = ["peft", "bitsandbytes", "datasets", "accelerate"]
+FINE_TUNE_DEPS = ["peft", "bitsandbytes", "datasets", "accelerate", "deepspeed", "auto-gptq"]
 FLAN_T5_DEPS = ["flax", "jax", "jaxlib", "tensorflow", "keras"]
+OPENAI_DEPS = ["openai", "tiktoken"]
+
+_base_requirements = {
+    inflection.dasherize(name): config_cls.__openllm_requirements__
+    for name, config_cls in openllm.CONFIG_MAPPING.items()
+    if config_cls.__openllm_requirements__
+}
+
+# NOTE: update this table when adding new external dependencies
+_deps_table = {
+    "fine-tune": FINE_TUNE_DEPS,
+    "flan-t5": FLAN_T5_DEPS,
+    "openai": OPENAI_DEPS,
+}
+
+_base_requirements.update(_deps_table)
 
 
 def main() -> int:
     with open(os.path.join(ROOT, "pyproject.toml"), "r") as f:
         pyproject = tomlkit.parse(f.read())
 
     table = tomlkit.table()
-    table.add("fine-tune", FINE_TUNE_DEPS)
+    for name, config in _base_requirements.items():
+        table.add(name, config)
 
-    for name, config in openllm.CONFIG_MAPPING.items():
-        dashed = inflection.dasherize(name)
-        if name == "flan_t5":
-            table.add(dashed, FLAN_T5_DEPS)
-            continue
-        if config.__openllm_requirements__:
-            table.add(dashed, config.__openllm_requirements__)
     table.add("all", [f"openllm[{k}]" for k in table.keys()])
 
     pyproject["project"]["optional-dependencies"] = table
     with open(os.path.join(ROOT, "pyproject.toml"), "w") as f:
         f.write(tomlkit.dumps(pyproject))
 
     if shutil.which("taplo"):
```

### Comparing `openllm-0.1.5/tools/update-readme.py` & `openllm-0.1.6/tools/update-readme.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,21 +43,21 @@
         "URL": [],
         "CPU": [],
         "GPU": [],
         "Installation": [],
         "Model Ids": [],
     }
     max_install_len_div = 0
-    for name, config in openllm.CONFIG_MAPPING.items():
+    for name, config_cls in openllm.CONFIG_MAPPING.items():
         dashed = inflection.dasherize(name)
         formatted["Model"].append(dashed)
-        formatted["URL"].append(config.__openllm_url__)
+        formatted["URL"].append(config_cls.__openllm_url__)
         formatted["GPU"].append("✅")
-        formatted["CPU"].append("✅" if not config.__openllm_requires_gpu__ else "❌")
-        formatted["Model Ids"].append(config.__openllm_model_ids__)
+        formatted["CPU"].append("✅" if not config_cls.__openllm_requires_gpu__ else "❌")
+        formatted["Model Ids"].append(config_cls.__openllm_model_ids__)
         if dashed in deps:
             instruction = f'```bash\npip install "openllm[{dashed}]"\n```'
         else:
             instruction = "```bash\npip install openllm\n```"
         if len(instruction) > max_install_len_div:
             max_install_len_div = len(instruction)
         formatted["Installation"].append(instruction)
```

### Comparing `openllm-0.1.5/typings/attr/__init__.pyi` & `openllm-0.1.6/typings/attr/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/typings/attr/exceptions.pyi` & `openllm-0.1.6/typings/attr/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/typings/attr/validators.pyi` & `openllm-0.1.6/typings/attr/validators.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/typings/click_option_group/__init__.pyi` & `openllm-0.1.6/typings/click_option_group/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/typings/click_option_group/_core.pyi` & `openllm-0.1.6/typings/click_option_group/_core.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/typings/click_option_group/_decorators.pyi` & `openllm-0.1.6/typings/click_option_group/_decorators.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/typings/click_option_group/_helpers.pyi` & `openllm-0.1.6/typings/click_option_group/_helpers.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/typings/deepmerge/merger.pyi` & `openllm-0.1.6/typings/deepmerge/merger.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/typings/deepmerge/strategy/core.pyi` & `openllm-0.1.6/typings/deepmerge/strategy/core.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/typings/deepmerge/strategy/set.pyi` & `openllm-0.1.6/typings/deepmerge/strategy/set.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/.gitignore` & `openllm-0.1.6/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -129,7 +129,8 @@
 .pyre/
 bazel-*
 
 package-lock.json
 
 # PyCharm config
 .idea
+outputs
```

### Comparing `openllm-0.1.5/LICENSE.md` & `openllm-0.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openllm-0.1.5/README.md` & `openllm-0.1.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -5,23 +5,23 @@
     </a><a href="https://github.com/bentoml/OpenLLM/actions/workflows/ci.yml">
         <img src="https://github.com/bentoml/OpenLLM/actions/workflows/ci.yml/badge.svg?branch=main" alt="ci" />
     </a><a href="https://twitter.com/bentomlai">
         <img src="https://badgen.net/badge/icon/@bentomlai/1DA1F2?icon=twitter&label=Follow%20Us" alt="Twitter" />
     </a><a href="https://l.bentoml.com/join-openllm-discord">
         <img src="https://badgen.net/badge/icon/OpenLLM/7289da?icon=discord&label=Join%20Us" alt="Discord" />
     </a><br>
-    <p>An open platform for operating large language models(LLMs) in production.</br>
+    <p>An open platform for operating large language models (LLMs) in production.</br>
     Fine-tune, serve, deploy, and monitor any LLMs with ease.</p>
     <i></i>
 </div>
 
 ## 📖 Introduction
 
 With OpenLLM, you can run inference with any open-source large-language
-models(LLMs), deploy to the cloud or on-premises, and build powerful AI apps.
+models (LLMs), deploy to the cloud or on-premises, and build powerful AI apps.
 
 🚂 **SOTA LLMs**: built-in supports a wide range of open-source LLMs and model
 runtime, including StableLM, Falcon, Dolly, Flan-T5, ChatGLM, StarCoder and
 more.
 
 🔥 **Flexible APIs**: serve LLMs over RESTful API or gRPC with one command,
 query via WebUI, CLI, our Python/Javascript client, or any HTTP client.
@@ -247,14 +247,37 @@
 <ul><li><a href=https://huggingface.co/stabilityai/stablelm-tuned-alpha-3b><code>stabilityai/stablelm-tuned-alpha-3b</code></a></li>
 <li><a href=https://huggingface.co/stabilityai/stablelm-tuned-alpha-7b><code>stabilityai/stablelm-tuned-alpha-7b</code></a></li>
 <li><a href=https://huggingface.co/stabilityai/stablelm-base-alpha-3b><code>stabilityai/stablelm-base-alpha-3b</code></a></li>
 <li><a href=https://huggingface.co/stabilityai/stablelm-base-alpha-7b><code>stabilityai/stablelm-base-alpha-7b</code></a></li></ul>
 
 </td>
 </tr>
+<tr>
+
+<td><a href=https://huggingface.co/docs/transformers/model_doc/opt>opt</a></td>
+<td>✅</td>
+<td>✅</td>
+<td>
+
+```bash
+pip install openllm
+```
+
+</td>
+<td>
+
+<ul><li><a href=https://huggingface.co/facebook/opt-125m><code>facebook/opt-125m</code></a></li>
+<li><a href=https://huggingface.co/facebook/opt-350m><code>facebook/opt-350m</code></a></li>
+<li><a href=https://huggingface.co/facebook/opt-1.3b><code>facebook/opt-1.3b</code></a></li>
+<li><a href=https://huggingface.co/facebook/opt-2.7b><code>facebook/opt-2.7b</code></a></li>
+<li><a href=https://huggingface.co/facebook/opt-6.7b><code>facebook/opt-6.7b</code></a></li>
+<li><a href=https://huggingface.co/facebook/opt-66b><code>facebook/opt-66b</code></a></li></ul>
+
+</td>
+</tr>
 </table>
 
 <!-- update-readme.py: stop -->
 
 ### Runtime Implementations (Experimental)
 
 Different LLMs may have multiple runtime implementations. For instance, they
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
                           ****** ð¦¾ OpenLLM ******
                       [pypi_status][ci][Twitter][Discord]
-An open platform for operating large language models(LLMs) in production. Fine-
-             tune, serve, deploy, and monitor any LLMs with ease.
+  An open platform for operating large language models (LLMs) in production.
+           Fine-tune, serve, deploy, and monitor any LLMs with ease.
 ## ð Introduction With OpenLLM, you can run inference with any open-source
-large-language models(LLMs), deploy to the cloud or on-premises, and build
+large-language models (LLMs), deploy to the cloud or on-premises, and build
 powerful AI apps. ð **SOTA LLMs**: built-in supports a wide range of open-
 source LLMs and model runtime, including StableLM, Falcon, Dolly, Flan-T5,
 ChatGLM, StarCoder and more. ð¥ **Flexible APIs**: serve LLMs over RESTful
 API or gRPC with one command, query via WebUI, CLI, our Python/Javascript
 client, or any HTTP client. âï¸ **Freedom To Build**: First-class support
 for LangChain and BentoML allows you to easily create your own AI apps by
 composing LLMs with other models and services. ð¯ **Streamline Deployment**:
@@ -79,14 +79,20 @@
                                                      tuned-alpha-3b
                                                    * stabilityai/stablelm-
 stablelm  ââ```bash pip install openllm        tuned-alpha-7b
                   ```                              * stabilityai/stablelm-
                                                      base-alpha-3b
                                                    * stabilityai/stablelm-
                                                      base-alpha-7b
+                                                   * facebook/opt-125m
+                                                   * facebook/opt-350m
+opt       ââ```bash pip install openllm      * facebook/opt-1.3b
+                  ```                              * facebook/opt-2.7b
+                                                   * facebook/opt-6.7b
+                                                   * facebook/opt-66b
  ### Runtime Implementations (Experimental) Different LLMs may have multiple
 runtime implementations. For instance, they might use Pytorch (`pt`),
 Tensorflow (`tf`), or Flax (`flax`). If you wish to specify a particular
 runtime for a model, you can do so by setting the `OPENLLM_
 {MODEL_NAME}_FRAMEWORK={runtime}` environment variable before running `openllm
 start`. For example, if you want to use the Tensorflow (`tf`) implementation
 for the `flan-t5` model, you can use the following command: ```bash
```

### Comparing `openllm-0.1.5/pyproject.toml` & `openllm-0.1.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -65,19 +65,27 @@
 name = "openllm"
 readme = "README.md"
 requires-python = ">=3.8"
 
 # NOTE: Don't modify project.optional-dependencies
 # as it is managed by ./tools/update-optional-dependencies.py
 [project.optional-dependencies]
-all = ["openllm[fine-tune]", "openllm[flan-t5]", "openllm[chatglm]", "openllm[starcoder]", "openllm[falcon]"]
+all = [
+    "openllm[chatglm]",
+    "openllm[starcoder]",
+    "openllm[falcon]",
+    "openllm[fine-tune]",
+    "openllm[flan-t5]",
+    "openllm[openai]",
+]
 chatglm = ["cpm_kernels", "sentencepiece"]
 falcon = ["einops", "xformers", "safetensors"]
-fine-tune = ["peft", "bitsandbytes", "datasets", "accelerate"]
+fine-tune = ["peft", "bitsandbytes", "datasets", "accelerate", "deepspeed", "auto-gptq"]
 flan-t5 = ["flax", "jax", "jaxlib", "tensorflow", "keras"]
+openai = ["openai", "tiktoken"]
 starcoder = ["bitsandbytes"]
 
 [project.urls]
 Documentation = "https://github.com/bentoml/openllm#readme"
 Issues = "https://github.com/bentoml/openllm/issues"
 Source = "https://github.com/bentoml/openllm"
 
@@ -92,57 +100,85 @@
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/openllm", "src/openllm_client"]
 
 [tool.hatch.envs.default]
 dependencies = [
     "coverage[toml]>=6.5",
+    # NOTE: Tests strategies with Hypothesis and pytest, and snapshot testing with syrupy
     "pytest",
     "pytest-asyncio>=0.21.0",
     "pytest-xdist[psutil]",
     "pytest-cov",
     "pytest-mock",
     "pytest-randomly",
     "pytest-rerunfailures",
+    "hypothesis",
+    "syrupy",
     # NOTE: To run all hooks
     "pre-commit",
     # NOTE: Using under ./tools/update-optional-dependencies.py
     "tomlkit",
     # NOTE: Using under ./tools/update-readme.py
     "markdown-it-py",
-    # NOTE: Tests strategies with Hypothesis
-    "hypothesis",
-    # NOTE: snapshot testing
-    "syrupy",
+    # NOTE: pyright for type
+    "pyright",
+    # NOTE: towncrier for changelog
+    "towncrier",
 ]
 [tool.hatch.envs.default.scripts]
-cov = ["test-cov", "cov-report"]
+changelog = "towncrier build --version main --draft"
+cov = ["cov-test", "cov-report"]
 cov-report = ["- coverage combine", "coverage report"]
+cov-test = "coverage run -m pytest {args:tests}"
+fmt = "pre-commit run --all-files"
 setup = "pre-commit install"
 test = "pytest {args:tests}"
-test-cov = "coverage run -m pytest {args:tests}"
+typing = "pyright {args:src/openllm tests}"
+
+[tool.towncrier]
+directory = "changelog.d"
+filename = "CHANGELOG.md"
+issue_format = "[#{issue}](https://github.com/bentoml/openllm/issues/{issue})"
+name = "openllm"
+start_string = "<!-- towncrier release notes start -->\n"
+template = "changelog.d/template.md.jinja"
+title_format = ""
+underlines = ["", "", ""]
+
+[[tool.towncrier.section]]
+path = ""
+
+[[tool.towncrier.type]]
+directory = "breaking"
+name = "Backwards-incompatible Changes"
+showcontent = true
+
+[[tool.towncrier.type]]
+directory = "deprecation"
+name = "Deprecations"
+showcontent = true
+
+[[tool.towncrier.type]]
+directory = "change"
+name = "Changes"
+showcontent = true
+
+[[tool.towncrier.type]]
+directory = "feature"
+name = "Features"
+showcontent = true
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11"]
 
-[tool.hatch.envs.dev]
-dependencies = [
-    "ruff",
-    "pyright",
-    "hatch",
-    # NOTE: black for generating service file.
-    "black[jupyter]==23.3.0",
-]
-detached = true
-
-[tool.hatch.envs.dev.scripts]
-all = ["fmt", "typing"]
-fmt = ["black {args:.}", "black --pyi {args:typings/}", "ruff --fix {args:.}", "style"]
-style = ["ruff {args:.}", "black --check --diff {args:.}"]
-typing = "pyright {args:src/openllm tests}"
+[tool.interrogate]
+fail-under = 100
+verbose = 2
+whitelist-regex = ["test_.*"]
 
 [tool.pytest.ini_options]
 addopts = ["-rfEX", "-pno:warnings"]
 python_files = ["test_*.py", "*_test.py"]
 testpaths = ["tests"]
 
 [tool.black]
@@ -194,30 +230,25 @@
 convention = "google"
 
 [tool.ruff.isort]
 force-single-line = true
 known-first-party = ["openllm", "bentoml", 'transformers']
 lines-after-imports = 2
 
-[tool.ruff.flake8-quotes]
-inline-quotes = "single"
-
-[tool.ruff.flake8-tidy-imports]
-ban-relative-imports = "all"
-
 [tool.ruff.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "__init__.py" = ["E402", "F401", "F403", "F811"]
 "src/openllm/_types.py" = ["E402"]
+"src/openllm/playground/**/*" = ['E402', 'F401']
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 
 [tool.pyright]
 analysis.useLibraryCodeForTypes = true
 enableTypeIgnoreComments = true
-include = ["src/", "tests/"]
+include = ["src/", "tests/", "tools/", "examples/"]
 pythonVersion = "3.11"
 reportMissingImports = "none"
 reportMissingModuleSource = "warning"
 reportMissingTypeStubs = "warning"
 reportUnknownMemberType = "warning"
 reportUnknownVariableType = "warning"
 strictDictionaryInference = true
```

### Comparing `openllm-0.1.5/PKG-INFO` & `openllm-0.1.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openllm
-Version: 0.1.5
+Version: 0.1.6
 Summary: OpenLLM: REST/gRPC API server for running any open Large-Language Model - StableLM, Llama, Alpaca, Dolly, Flan-T5, Custom
 Project-URL: Documentation, https://github.com/bentoml/openllm#readme
 Project-URL: Issues, https://github.com/bentoml/openllm/issues
 Project-URL: Source, https://github.com/bentoml/openllm
 Author-email: Aaron Pham <aarnphm@bentoml.com>, BentoML Team <contact@bentoml.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.md
@@ -35,33 +35,39 @@
 Requires-Dist: transformers[tokenizers,torch]>=4.29.0
 Requires-Dist: typing-extensions
 Provides-Extra: all
 Requires-Dist: openllm[chatglm]; extra == 'all'
 Requires-Dist: openllm[falcon]; extra == 'all'
 Requires-Dist: openllm[fine-tune]; extra == 'all'
 Requires-Dist: openllm[flan-t5]; extra == 'all'
+Requires-Dist: openllm[openai]; extra == 'all'
 Requires-Dist: openllm[starcoder]; extra == 'all'
 Provides-Extra: chatglm
 Requires-Dist: cpm-kernels; extra == 'chatglm'
 Requires-Dist: sentencepiece; extra == 'chatglm'
 Provides-Extra: falcon
 Requires-Dist: einops; extra == 'falcon'
 Requires-Dist: safetensors; extra == 'falcon'
 Requires-Dist: xformers; extra == 'falcon'
 Provides-Extra: fine-tune
 Requires-Dist: accelerate; extra == 'fine-tune'
+Requires-Dist: auto-gptq; extra == 'fine-tune'
 Requires-Dist: bitsandbytes; extra == 'fine-tune'
 Requires-Dist: datasets; extra == 'fine-tune'
+Requires-Dist: deepspeed; extra == 'fine-tune'
 Requires-Dist: peft; extra == 'fine-tune'
 Provides-Extra: flan-t5
 Requires-Dist: flax; extra == 'flan-t5'
 Requires-Dist: jax; extra == 'flan-t5'
 Requires-Dist: jaxlib; extra == 'flan-t5'
 Requires-Dist: keras; extra == 'flan-t5'
 Requires-Dist: tensorflow; extra == 'flan-t5'
+Provides-Extra: openai
+Requires-Dist: openai; extra == 'openai'
+Requires-Dist: tiktoken; extra == 'openai'
 Provides-Extra: starcoder
 Requires-Dist: bitsandbytes; extra == 'starcoder'
 Description-Content-Type: text/markdown
 
 <div align="center">
     <h1 align="center">🦾 OpenLLM</h1>
     <a href="https://pypi.org/project/openllm">
@@ -69,23 +75,23 @@
     </a><a href="https://github.com/bentoml/OpenLLM/actions/workflows/ci.yml">
         <img src="https://github.com/bentoml/OpenLLM/actions/workflows/ci.yml/badge.svg?branch=main" alt="ci" />
     </a><a href="https://twitter.com/bentomlai">
         <img src="https://badgen.net/badge/icon/@bentomlai/1DA1F2?icon=twitter&label=Follow%20Us" alt="Twitter" />
     </a><a href="https://l.bentoml.com/join-openllm-discord">
         <img src="https://badgen.net/badge/icon/OpenLLM/7289da?icon=discord&label=Join%20Us" alt="Discord" />
     </a><br>
-    <p>An open platform for operating large language models(LLMs) in production.</br>
+    <p>An open platform for operating large language models (LLMs) in production.</br>
     Fine-tune, serve, deploy, and monitor any LLMs with ease.</p>
     <i></i>
 </div>
 
 ## 📖 Introduction
 
 With OpenLLM, you can run inference with any open-source large-language
-models(LLMs), deploy to the cloud or on-premises, and build powerful AI apps.
+models (LLMs), deploy to the cloud or on-premises, and build powerful AI apps.
 
 🚂 **SOTA LLMs**: built-in supports a wide range of open-source LLMs and model
 runtime, including StableLM, Falcon, Dolly, Flan-T5, ChatGLM, StarCoder and
 more.
 
 🔥 **Flexible APIs**: serve LLMs over RESTful API or gRPC with one command,
 query via WebUI, CLI, our Python/Javascript client, or any HTTP client.
@@ -311,14 +317,37 @@
 <ul><li><a href=https://huggingface.co/stabilityai/stablelm-tuned-alpha-3b><code>stabilityai/stablelm-tuned-alpha-3b</code></a></li>
 <li><a href=https://huggingface.co/stabilityai/stablelm-tuned-alpha-7b><code>stabilityai/stablelm-tuned-alpha-7b</code></a></li>
 <li><a href=https://huggingface.co/stabilityai/stablelm-base-alpha-3b><code>stabilityai/stablelm-base-alpha-3b</code></a></li>
 <li><a href=https://huggingface.co/stabilityai/stablelm-base-alpha-7b><code>stabilityai/stablelm-base-alpha-7b</code></a></li></ul>
 
 </td>
 </tr>
+<tr>
+
+<td><a href=https://huggingface.co/docs/transformers/model_doc/opt>opt</a></td>
+<td>✅</td>
+<td>✅</td>
+<td>
+
+```bash
+pip install openllm
+```
+
+</td>
+<td>
+
+<ul><li><a href=https://huggingface.co/facebook/opt-125m><code>facebook/opt-125m</code></a></li>
+<li><a href=https://huggingface.co/facebook/opt-350m><code>facebook/opt-350m</code></a></li>
+<li><a href=https://huggingface.co/facebook/opt-1.3b><code>facebook/opt-1.3b</code></a></li>
+<li><a href=https://huggingface.co/facebook/opt-2.7b><code>facebook/opt-2.7b</code></a></li>
+<li><a href=https://huggingface.co/facebook/opt-6.7b><code>facebook/opt-6.7b</code></a></li>
+<li><a href=https://huggingface.co/facebook/opt-66b><code>facebook/opt-66b</code></a></li></ul>
+
+</td>
+</tr>
 </table>
 
 <!-- update-readme.py: stop -->
 
 ### Runtime Implementations (Experimental)
 
 Different LLMs may have multiple runtime implementations. For instance, they
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openllm Version: 0.1.5 Summary: OpenLLM: REST/gRPC
+Metadata-Version: 2.1 Name: openllm Version: 0.1.6 Summary: OpenLLM: REST/gRPC
 API server for running any open Large-Language Model - StableLM, Llama, Alpaca,
 Dolly, Flan-T5, Custom Project-URL: Documentation, https://github.com/bentoml/
 openllm#readme Project-URL: Issues, https://github.com/bentoml/openllm/issues
 Project-URL: Source, https://github.com/bentoml/openllm Author-email: Aaron
 Pham
 bentoml.com>, BentoML Team
 bentoml.com> License-Expression: Apache-2.0 License-File: LICENSE.md Keywords:
@@ -21,32 +21,36 @@
 Requires-Python: >=3.8 Requires-Dist: attrs>=23.1.0 Requires-Dist: bentoml
 [grpc,io]>=1.0.22 Requires-Dist: cattrs>=23.1.0 Requires-Dist: httpx Requires-
 Dist: inflection Requires-Dist: optimum Requires-Dist: orjson Requires-Dist:
 tabulate[widechars]>=0.9.0 Requires-Dist: transformers
 [tokenizers,torch]>=4.29.0 Requires-Dist: typing-extensions Provides-Extra: all
 Requires-Dist: openllm[chatglm]; extra == 'all' Requires-Dist: openllm[falcon];
 extra == 'all' Requires-Dist: openllm[fine-tune]; extra == 'all' Requires-Dist:
-openllm[flan-t5]; extra == 'all' Requires-Dist: openllm[starcoder]; extra ==
-'all' Provides-Extra: chatglm Requires-Dist: cpm-kernels; extra == 'chatglm'
-Requires-Dist: sentencepiece; extra == 'chatglm' Provides-Extra: falcon
-Requires-Dist: einops; extra == 'falcon' Requires-Dist: safetensors; extra ==
-'falcon' Requires-Dist: xformers; extra == 'falcon' Provides-Extra: fine-tune
-Requires-Dist: accelerate; extra == 'fine-tune' Requires-Dist: bitsandbytes;
-extra == 'fine-tune' Requires-Dist: datasets; extra == 'fine-tune' Requires-
-Dist: peft; extra == 'fine-tune' Provides-Extra: flan-t5 Requires-Dist: flax;
-extra == 'flan-t5' Requires-Dist: jax; extra == 'flan-t5' Requires-Dist:
-jaxlib; extra == 'flan-t5' Requires-Dist: keras; extra == 'flan-t5' Requires-
-Dist: tensorflow; extra == 'flan-t5' Provides-Extra: starcoder Requires-Dist:
-bitsandbytes; extra == 'starcoder' Description-Content-Type: text/markdown
+openllm[flan-t5]; extra == 'all' Requires-Dist: openllm[openai]; extra == 'all'
+Requires-Dist: openllm[starcoder]; extra == 'all' Provides-Extra: chatglm
+Requires-Dist: cpm-kernels; extra == 'chatglm' Requires-Dist: sentencepiece;
+extra == 'chatglm' Provides-Extra: falcon Requires-Dist: einops; extra ==
+'falcon' Requires-Dist: safetensors; extra == 'falcon' Requires-Dist: xformers;
+extra == 'falcon' Provides-Extra: fine-tune Requires-Dist: accelerate; extra ==
+'fine-tune' Requires-Dist: auto-gptq; extra == 'fine-tune' Requires-Dist:
+bitsandbytes; extra == 'fine-tune' Requires-Dist: datasets; extra == 'fine-
+tune' Requires-Dist: deepspeed; extra == 'fine-tune' Requires-Dist: peft; extra
+== 'fine-tune' Provides-Extra: flan-t5 Requires-Dist: flax; extra == 'flan-t5'
+Requires-Dist: jax; extra == 'flan-t5' Requires-Dist: jaxlib; extra == 'flan-
+t5' Requires-Dist: keras; extra == 'flan-t5' Requires-Dist: tensorflow; extra
+== 'flan-t5' Provides-Extra: openai Requires-Dist: openai; extra == 'openai'
+Requires-Dist: tiktoken; extra == 'openai' Provides-Extra: starcoder Requires-
+Dist: bitsandbytes; extra == 'starcoder' Description-Content-Type: text/
+markdown
                           ****** ð¦¾ OpenLLM ******
                       [pypi_status][ci][Twitter][Discord]
-An open platform for operating large language models(LLMs) in production. Fine-
-             tune, serve, deploy, and monitor any LLMs with ease.
+  An open platform for operating large language models (LLMs) in production.
+           Fine-tune, serve, deploy, and monitor any LLMs with ease.
 ## ð Introduction With OpenLLM, you can run inference with any open-source
-large-language models(LLMs), deploy to the cloud or on-premises, and build
+large-language models (LLMs), deploy to the cloud or on-premises, and build
 powerful AI apps. ð **SOTA LLMs**: built-in supports a wide range of open-
 source LLMs and model runtime, including StableLM, Falcon, Dolly, Flan-T5,
 ChatGLM, StarCoder and more. ð¥ **Flexible APIs**: serve LLMs over RESTful
 API or gRPC with one command, query via WebUI, CLI, our Python/Javascript
 client, or any HTTP client. âï¸ **Freedom To Build**: First-class support
 for LangChain and BentoML allows you to easily create your own AI apps by
 composing LLMs with other models and services. ð¯ **Streamline Deployment**:
@@ -118,14 +122,20 @@
                                                      tuned-alpha-3b
                                                    * stabilityai/stablelm-
 stablelm  ââ```bash pip install openllm        tuned-alpha-7b
                   ```                              * stabilityai/stablelm-
                                                      base-alpha-3b
                                                    * stabilityai/stablelm-
                                                      base-alpha-7b
+                                                   * facebook/opt-125m
+                                                   * facebook/opt-350m
+opt       ââ```bash pip install openllm      * facebook/opt-1.3b
+                  ```                              * facebook/opt-2.7b
+                                                   * facebook/opt-6.7b
+                                                   * facebook/opt-66b
  ### Runtime Implementations (Experimental) Different LLMs may have multiple
 runtime implementations. For instance, they might use Pytorch (`pt`),
 Tensorflow (`tf`), or Flax (`flax`). If you wish to specify a particular
 runtime for a model, you can do so by setting the `OPENLLM_
 {MODEL_NAME}_FRAMEWORK={runtime}` environment variable before running `openllm
 start`. For example, if you want to use the Tensorflow (`tf`) implementation
 for the `flan-t5` model, you can use the following command: ```bash
```

