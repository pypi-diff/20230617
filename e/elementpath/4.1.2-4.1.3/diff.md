# Comparing `tmp/elementpath-4.1.2.tar.gz` & `tmp/elementpath-4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elementpath-4.1.2.tar", last modified: Thu May  4 09:50:32 2023, max compression
+gzip compressed data, was "elementpath-4.1.3.tar", last modified: Sat Jun 17 17:41:47 2023, max compression
```

## Comparing `elementpath-4.1.2.tar` & `elementpath-4.1.3.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-04 09:50:31.998775 elementpath-4.1.2/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      223 2023-03-21 14:20:17.000000 elementpath-4.1.2/.coveragerc
--rw-r--r--   0 brunato   (1000) brunato   (1000)    15773 2023-04-28 14:38:26.000000 elementpath-4.1.2/CHANGELOG.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1131 2021-02-11 20:59:30.000000 elementpath-4.1.2/LICENSE
--rw-r--r--   0 brunato   (1000) brunato   (1000)      293 2023-03-21 14:20:17.000000 elementpath-4.1.2/MANIFEST.in
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6286 2023-05-04 09:50:31.998775 elementpath-4.1.2/PKG-INFO
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4894 2023-04-11 07:55:05.000000 elementpath-4.1.2/README.rst
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-04 09:50:31.987775 elementpath-4.1.2/doc/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      608 2018-05-04 17:54:35.000000 elementpath-4.1.2/doc/Makefile
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7748 2023-03-21 14:20:17.000000 elementpath-4.1.2/doc/advanced.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5866 2023-04-28 14:38:26.000000 elementpath-4.1.2/doc/conf.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)      346 2023-03-21 14:20:18.000000 elementpath-4.1.2/doc/index.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)      110 2018-06-15 15:57:58.000000 elementpath-4.1.2/doc/introduction.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)      815 2018-05-04 17:54:35.000000 elementpath-4.1.2/doc/make.bat
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1930 2020-08-06 17:45:39.000000 elementpath-4.1.2/doc/pratt_api.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4669 2023-02-01 12:54:01.000000 elementpath-4.1.2/doc/xpath_api.rst
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-04 09:50:31.989775 elementpath-4.1.2/elementpath/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2690 2023-04-28 14:38:26.000000 elementpath-4.1.2/elementpath/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6700 2023-03-01 07:02:51.000000 elementpath-4.1.2/elementpath/collations.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    16559 2023-02-02 15:43:11.000000 elementpath-4.1.2/elementpath/compare.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-04 09:50:31.991775 elementpath-4.1.2/elementpath/datatypes/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6425 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/datatypes/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3618 2023-03-07 17:43:44.000000 elementpath-4.1.2/elementpath/datatypes/atomic_types.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5954 2023-03-21 14:20:18.000000 elementpath-4.1.2/elementpath/datatypes/binary.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    40208 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/datatypes/datetime.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8781 2023-03-21 14:20:18.000000 elementpath-4.1.2/elementpath/datatypes/numeric.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6634 2023-03-21 14:20:18.000000 elementpath-4.1.2/elementpath/datatypes/proxies.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2906 2023-03-21 14:20:18.000000 elementpath-4.1.2/elementpath/datatypes/qname.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2396 2023-03-21 14:20:18.000000 elementpath-4.1.2/elementpath/datatypes/string.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5210 2023-03-21 14:20:18.000000 elementpath-4.1.2/elementpath/datatypes/untyped.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4302 2023-03-18 21:22:38.000000 elementpath-4.1.2/elementpath/datatypes/uri.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11175 2023-03-21 14:20:18.000000 elementpath-4.1.2/elementpath/etree.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    14835 2023-03-21 14:20:18.000000 elementpath-4.1.2/elementpath/exceptions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8913 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/helpers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5439 2023-03-21 14:20:18.000000 elementpath-4.1.2/elementpath/namespaces.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     7198 2022-07-16 19:41:23.000000 elementpath-4.1.2/elementpath/protocols.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2021-08-26 06:55:19.000000 elementpath-4.1.2/elementpath/py.typed
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-04 09:50:31.991775 elementpath-4.1.2/elementpath/regex/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1051 2022-07-16 19:41:23.000000 elementpath-4.1.2/elementpath/regex/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8295 2021-11-07 17:03:50.000000 elementpath-4.1.2/elementpath/regex/character_classes.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3703 2021-11-06 21:19:15.000000 elementpath-4.1.2/elementpath/regex/codepoints.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4035 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/regex/generate_categories.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11503 2023-03-21 14:20:18.000000 elementpath-4.1.2/elementpath/regex/patterns.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    79480 2020-08-18 19:39:53.000000 elementpath-4.1.2/elementpath/regex/unicode_categories.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    20127 2023-02-01 12:54:01.000000 elementpath-4.1.2/elementpath/regex/unicode_subsets.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6698 2023-03-21 14:20:18.000000 elementpath-4.1.2/elementpath/schema_proxy.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    13704 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/sequence_types.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    17185 2023-04-28 14:38:26.000000 elementpath-4.1.2/elementpath/serialization.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    35099 2023-04-28 14:38:26.000000 elementpath-4.1.2/elementpath/tdop.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    12572 2023-04-28 14:38:26.000000 elementpath-4.1.2/elementpath/tree_builders.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-04 09:50:31.992775 elementpath-4.1.2/elementpath/validators/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1816 2023-03-21 14:20:18.000000 elementpath-4.1.2/elementpath/validators/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1580 2023-02-01 12:54:01.000000 elementpath-4.1.2/elementpath/validators/analyze-string.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5389 2023-02-01 12:54:01.000000 elementpath-4.1.2/elementpath/validators/schema-for-json.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-04 09:50:31.992775 elementpath-4.1.2/elementpath/xpath1/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      505 2022-03-04 13:17:21.000000 elementpath-4.1.2/elementpath/xpath1/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3809 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/xpath1/_xpath1_axes.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    16819 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/xpath1/_xpath1_functions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    28752 2023-04-28 14:38:26.000000 elementpath-4.1.2/elementpath/xpath1/_xpath1_operators.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    10956 2023-03-21 14:20:18.000000 elementpath-4.1.2/elementpath/xpath1/xpath1_parser.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-04 09:50:31.993775 elementpath-4.1.2/elementpath/xpath2/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      513 2022-03-04 13:16:42.000000 elementpath-4.1.2/elementpath/xpath2/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19427 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/xpath2/_xpath2_constructors.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    60225 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/xpath2/_xpath2_functions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    30851 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/xpath2/_xpath2_operators.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    24422 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/xpath2/xpath2_parser.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)      494 2023-02-01 12:54:01.000000 elementpath-4.1.2/elementpath/xpath3.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-04 09:50:31.993775 elementpath-4.1.2/elementpath/xpath30/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      515 2023-03-01 07:02:42.000000 elementpath-4.1.2/elementpath/xpath30/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4183 2022-02-20 07:49:53.000000 elementpath-4.1.2/elementpath/xpath30/_translation_maps.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    67763 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/xpath30/_xpath30_functions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8117 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/xpath30/_xpath30_operators.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    23515 2023-03-21 14:20:18.000000 elementpath-4.1.2/elementpath/xpath30/xpath30_helpers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3766 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/xpath30/xpath30_parser.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-04 09:50:31.994775 elementpath-4.1.2/elementpath/xpath31/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      515 2022-07-27 13:53:12.000000 elementpath-4.1.2/elementpath/xpath31/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    49075 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/xpath31/_xpath31_functions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8212 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/xpath31/_xpath31_operators.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1246 2023-02-01 12:54:01.000000 elementpath-4.1.2/elementpath/xpath31/xpath31_parser.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    20580 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/xpath_context.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    30076 2023-04-28 14:38:26.000000 elementpath-4.1.2/elementpath/xpath_nodes.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6120 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/xpath_selectors.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    73761 2023-04-11 07:36:42.000000 elementpath-4.1.2/elementpath/xpath_tokens.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-04 09:50:31.990775 elementpath-4.1.2/elementpath.egg-info/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6286 2023-05-04 09:50:31.000000 elementpath-4.1.2/elementpath.egg-info/PKG-INFO
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3478 2023-05-04 09:50:31.000000 elementpath-4.1.2/elementpath.egg-info/SOURCES.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)        1 2023-05-04 09:50:31.000000 elementpath-4.1.2/elementpath.egg-info/dependency_links.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)       95 2023-05-04 09:50:31.000000 elementpath-4.1.2/elementpath.egg-info/requires.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)       12 2023-05-04 09:50:31.000000 elementpath-4.1.2/elementpath.egg-info/top_level.txt
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       31 2022-06-20 15:16:48.000000 elementpath-4.1.2/mypy.ini
--rw-r--r--   0 brunato   (1000) brunato   (1000)      160 2023-04-28 13:30:35.000000 elementpath-4.1.2/requirements-dev.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)       38 2023-05-04 09:50:31.999775 elementpath-4.1.2/setup.cfg
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2346 2023-04-28 14:38:26.000000 elementpath-4.1.2/setup.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-04 09:50:31.997775 elementpath-4.1.2/tests/
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-12-01 17:06:27.000000 elementpath-4.1.2/tests/__init__.py
--rwxr-xr-x   0 brunato   (1000) brunato   (1000)    61187 2023-03-21 14:20:18.000000 elementpath-4.1.2/tests/execute_w3c_tests.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1256 2023-02-01 12:54:01.000000 elementpath-4.1.2/tests/memory_profiling.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-04 09:50:31.997775 elementpath-4.1.2/tests/mypy_tests/
--rwxr-xr-x   0 brunato   (1000) brunato   (1000)      499 2023-04-28 12:53:02.000000 elementpath-4.1.2/tests/mypy_tests/selectors.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-05-04 09:50:31.998775 elementpath-4.1.2/tests/resources/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1217 2021-02-27 18:23:11.000000 elementpath-4.1.2/tests/resources/analyze-string.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      171 2022-07-16 19:41:23.000000 elementpath-4.1.2/tests/resources/external_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)       67 2021-02-27 18:23:11.000000 elementpath-4.1.2/tests/resources/sample.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5389 2023-02-01 12:54:01.000000 elementpath-4.1.2/tests/resources/schema-for-json.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      308 2022-07-16 19:41:23.000000 elementpath-4.1.2/tests/resources/unparsed_entity.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      170 2022-07-16 19:41:23.000000 elementpath-4.1.2/tests/resources/unused_external_entity.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      270 2022-07-16 19:41:23.000000 elementpath-4.1.2/tests/resources/unused_unparsed_entity.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      129 2022-07-16 19:41:23.000000 elementpath-4.1.2/tests/resources/with_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1864 2023-02-01 12:54:01.000000 elementpath-4.1.2/tests/test_collations.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5469 2023-03-21 14:20:18.000000 elementpath-4.1.2/tests/test_compare.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    86399 2023-03-21 14:20:18.000000 elementpath-4.1.2/tests/test_datatypes.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1114 2021-01-06 17:09:53.000000 elementpath-4.1.2/tests/test_elementpath.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19106 2023-03-21 14:20:18.000000 elementpath-4.1.2/tests/test_etree.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3715 2023-03-21 14:20:18.000000 elementpath-4.1.2/tests/test_exceptions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11284 2023-04-11 07:36:42.000000 elementpath-4.1.2/tests/test_helpers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2904 2023-03-21 14:20:18.000000 elementpath-4.1.2/tests/test_namespaces.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     2789 2022-07-16 19:41:23.000000 elementpath-4.1.2/tests/test_package.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    43489 2023-03-21 14:20:19.000000 elementpath-4.1.2/tests/test_regex.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     9798 2023-02-01 12:54:01.000000 elementpath-4.1.2/tests/test_schema_context.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    20182 2023-02-01 12:54:01.000000 elementpath-4.1.2/tests/test_schema_proxy.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3793 2023-04-28 14:38:26.000000 elementpath-4.1.2/tests/test_selectors.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    15434 2023-04-28 14:38:26.000000 elementpath-4.1.2/tests/test_sequence_types.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    17460 2023-04-28 14:38:26.000000 elementpath-4.1.2/tests/test_serialization.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    16558 2023-04-28 14:38:26.000000 elementpath-4.1.2/tests/test_tdop_parser.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7919 2023-04-28 14:38:26.000000 elementpath-4.1.2/tests/test_tree_builders.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1887 2023-04-28 13:22:02.000000 elementpath-4.1.2/tests/test_typing.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2068 2023-03-21 14:20:19.000000 elementpath-4.1.2/tests/test_validators.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    84012 2023-04-28 14:38:26.000000 elementpath-4.1.2/tests/test_xpath1_parser.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    33795 2023-03-21 14:20:19.000000 elementpath-4.1.2/tests/test_xpath2_constructors.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    86351 2023-02-01 12:54:01.000000 elementpath-4.1.2/tests/test_xpath2_functions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    67321 2023-04-11 07:36:42.000000 elementpath-4.1.2/tests/test_xpath2_parser.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    57332 2023-03-21 14:20:19.000000 elementpath-4.1.2/tests/test_xpath30.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    47783 2023-03-21 14:20:19.000000 elementpath-4.1.2/tests/test_xpath31.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    12435 2022-07-16 19:41:23.000000 elementpath-4.1.2/tests/test_xpath_context.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    17766 2023-04-28 14:38:26.000000 elementpath-4.1.2/tests/test_xpath_nodes.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    35390 2023-04-26 14:25:47.000000 elementpath-4.1.2/tests/test_xpath_tokens.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11906 2023-03-21 14:20:19.000000 elementpath-4.1.2/tests/xpath_test_class.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1574 2023-04-28 15:16:01.000000 elementpath-4.1.2/tox.ini
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-17 17:41:47.490959 elementpath-4.1.3/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      223 2023-03-21 14:20:17.000000 elementpath-4.1.3/.coveragerc
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    15969 2023-06-17 17:40:45.000000 elementpath-4.1.3/CHANGELOG.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1131 2021-02-11 20:59:30.000000 elementpath-4.1.3/LICENSE
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      293 2023-03-21 14:20:17.000000 elementpath-4.1.3/MANIFEST.in
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6286 2023-06-17 17:41:47.490959 elementpath-4.1.3/PKG-INFO
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4894 2023-04-11 07:55:05.000000 elementpath-4.1.3/README.rst
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-17 17:41:47.479959 elementpath-4.1.3/doc/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      608 2018-05-04 17:54:35.000000 elementpath-4.1.3/doc/Makefile
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7748 2023-03-21 14:20:17.000000 elementpath-4.1.3/doc/advanced.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5866 2023-06-17 17:40:45.000000 elementpath-4.1.3/doc/conf.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      346 2023-03-21 14:20:18.000000 elementpath-4.1.3/doc/index.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      110 2018-06-15 15:57:58.000000 elementpath-4.1.3/doc/introduction.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      815 2018-05-04 17:54:35.000000 elementpath-4.1.3/doc/make.bat
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1930 2020-08-06 17:45:39.000000 elementpath-4.1.3/doc/pratt_api.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4669 2023-02-01 12:54:01.000000 elementpath-4.1.3/doc/xpath_api.rst
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-17 17:41:47.481959 elementpath-4.1.3/elementpath/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2690 2023-06-17 17:40:45.000000 elementpath-4.1.3/elementpath/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6700 2023-03-01 07:02:51.000000 elementpath-4.1.3/elementpath/collations.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    16559 2023-02-02 15:43:11.000000 elementpath-4.1.3/elementpath/compare.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-17 17:41:47.483959 elementpath-4.1.3/elementpath/datatypes/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6425 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/datatypes/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3618 2023-03-07 17:43:44.000000 elementpath-4.1.3/elementpath/datatypes/atomic_types.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5954 2023-03-21 14:20:18.000000 elementpath-4.1.3/elementpath/datatypes/binary.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    40208 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/datatypes/datetime.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8781 2023-03-21 14:20:18.000000 elementpath-4.1.3/elementpath/datatypes/numeric.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6634 2023-03-21 14:20:18.000000 elementpath-4.1.3/elementpath/datatypes/proxies.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2906 2023-03-21 14:20:18.000000 elementpath-4.1.3/elementpath/datatypes/qname.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2396 2023-03-21 14:20:18.000000 elementpath-4.1.3/elementpath/datatypes/string.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5210 2023-03-21 14:20:18.000000 elementpath-4.1.3/elementpath/datatypes/untyped.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4302 2023-03-18 21:22:38.000000 elementpath-4.1.3/elementpath/datatypes/uri.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11175 2023-03-21 14:20:18.000000 elementpath-4.1.3/elementpath/etree.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    14835 2023-03-21 14:20:18.000000 elementpath-4.1.3/elementpath/exceptions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8913 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5439 2023-03-21 14:20:18.000000 elementpath-4.1.3/elementpath/namespaces.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     7198 2022-07-16 19:41:23.000000 elementpath-4.1.3/elementpath/protocols.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2021-08-26 06:55:19.000000 elementpath-4.1.3/elementpath/py.typed
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-17 17:41:47.484959 elementpath-4.1.3/elementpath/regex/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1051 2022-07-16 19:41:23.000000 elementpath-4.1.3/elementpath/regex/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8295 2021-11-07 17:03:50.000000 elementpath-4.1.3/elementpath/regex/character_classes.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3703 2021-11-06 21:19:15.000000 elementpath-4.1.3/elementpath/regex/codepoints.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4035 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/regex/generate_categories.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11503 2023-03-21 14:20:18.000000 elementpath-4.1.3/elementpath/regex/patterns.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    79480 2020-08-18 19:39:53.000000 elementpath-4.1.3/elementpath/regex/unicode_categories.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    20127 2023-02-01 12:54:01.000000 elementpath-4.1.3/elementpath/regex/unicode_subsets.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6698 2023-03-21 14:20:18.000000 elementpath-4.1.3/elementpath/schema_proxy.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    13704 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/sequence_types.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    17185 2023-04-28 14:38:26.000000 elementpath-4.1.3/elementpath/serialization.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    35099 2023-04-28 14:38:26.000000 elementpath-4.1.3/elementpath/tdop.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    12572 2023-04-28 14:38:26.000000 elementpath-4.1.3/elementpath/tree_builders.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-17 17:41:47.484959 elementpath-4.1.3/elementpath/validators/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1816 2023-03-21 14:20:18.000000 elementpath-4.1.3/elementpath/validators/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1580 2023-02-01 12:54:01.000000 elementpath-4.1.3/elementpath/validators/analyze-string.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5389 2023-02-01 12:54:01.000000 elementpath-4.1.3/elementpath/validators/schema-for-json.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-17 17:41:47.484959 elementpath-4.1.3/elementpath/xpath1/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      505 2022-03-04 13:17:21.000000 elementpath-4.1.3/elementpath/xpath1/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3809 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/xpath1/_xpath1_axes.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    16819 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/xpath1/_xpath1_functions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    28752 2023-04-28 14:38:26.000000 elementpath-4.1.3/elementpath/xpath1/_xpath1_operators.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    10956 2023-03-21 14:20:18.000000 elementpath-4.1.3/elementpath/xpath1/xpath1_parser.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-17 17:41:47.485959 elementpath-4.1.3/elementpath/xpath2/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      513 2022-03-04 13:16:42.000000 elementpath-4.1.3/elementpath/xpath2/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19427 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/xpath2/_xpath2_constructors.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    60225 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/xpath2/_xpath2_functions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    30851 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/xpath2/_xpath2_operators.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    24422 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/xpath2/xpath2_parser.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      494 2023-02-01 12:54:01.000000 elementpath-4.1.3/elementpath/xpath3.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-17 17:41:47.486959 elementpath-4.1.3/elementpath/xpath30/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      515 2023-03-01 07:02:42.000000 elementpath-4.1.3/elementpath/xpath30/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4183 2022-02-20 07:49:53.000000 elementpath-4.1.3/elementpath/xpath30/_translation_maps.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    67943 2023-06-17 17:40:45.000000 elementpath-4.1.3/elementpath/xpath30/_xpath30_functions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8117 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/xpath30/_xpath30_operators.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    23515 2023-03-21 14:20:18.000000 elementpath-4.1.3/elementpath/xpath30/xpath30_helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3766 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/xpath30/xpath30_parser.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-17 17:41:47.486959 elementpath-4.1.3/elementpath/xpath31/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      515 2022-07-27 13:53:12.000000 elementpath-4.1.3/elementpath/xpath31/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    49075 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/xpath31/_xpath31_functions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8212 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/xpath31/_xpath31_operators.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1246 2023-02-01 12:54:01.000000 elementpath-4.1.3/elementpath/xpath31/xpath31_parser.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    20580 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/xpath_context.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    30076 2023-04-28 14:38:26.000000 elementpath-4.1.3/elementpath/xpath_nodes.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6120 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/xpath_selectors.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    73761 2023-04-11 07:36:42.000000 elementpath-4.1.3/elementpath/xpath_tokens.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-17 17:41:47.482959 elementpath-4.1.3/elementpath.egg-info/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6286 2023-06-17 17:41:47.000000 elementpath-4.1.3/elementpath.egg-info/PKG-INFO
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3478 2023-06-17 17:41:47.000000 elementpath-4.1.3/elementpath.egg-info/SOURCES.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        1 2023-06-17 17:41:47.000000 elementpath-4.1.3/elementpath.egg-info/dependency_links.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       95 2023-06-17 17:41:47.000000 elementpath-4.1.3/elementpath.egg-info/requires.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       12 2023-06-17 17:41:47.000000 elementpath-4.1.3/elementpath.egg-info/top_level.txt
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       31 2022-06-20 15:16:48.000000 elementpath-4.1.3/mypy.ini
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      160 2023-04-28 13:30:35.000000 elementpath-4.1.3/requirements-dev.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       38 2023-06-17 17:41:47.490959 elementpath-4.1.3/setup.cfg
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2346 2023-06-17 17:40:45.000000 elementpath-4.1.3/setup.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-17 17:41:47.489959 elementpath-4.1.3/tests/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-12-01 17:06:27.000000 elementpath-4.1.3/tests/__init__.py
+-rwxr-xr-x   0 brunato   (1000) brunato   (1000)    61187 2023-03-21 14:20:18.000000 elementpath-4.1.3/tests/execute_w3c_tests.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1256 2023-02-01 12:54:01.000000 elementpath-4.1.3/tests/memory_profiling.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-17 17:41:47.489959 elementpath-4.1.3/tests/mypy_tests/
+-rwxr-xr-x   0 brunato   (1000) brunato   (1000)      499 2023-05-05 12:45:43.000000 elementpath-4.1.3/tests/mypy_tests/selectors.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2023-06-17 17:41:47.490959 elementpath-4.1.3/tests/resources/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1217 2021-02-27 18:23:11.000000 elementpath-4.1.3/tests/resources/analyze-string.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      171 2022-07-16 19:41:23.000000 elementpath-4.1.3/tests/resources/external_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       67 2021-02-27 18:23:11.000000 elementpath-4.1.3/tests/resources/sample.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5389 2023-02-01 12:54:01.000000 elementpath-4.1.3/tests/resources/schema-for-json.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      308 2022-07-16 19:41:23.000000 elementpath-4.1.3/tests/resources/unparsed_entity.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      170 2022-07-16 19:41:23.000000 elementpath-4.1.3/tests/resources/unused_external_entity.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      270 2022-07-16 19:41:23.000000 elementpath-4.1.3/tests/resources/unused_unparsed_entity.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      129 2022-07-16 19:41:23.000000 elementpath-4.1.3/tests/resources/with_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1864 2023-02-01 12:54:01.000000 elementpath-4.1.3/tests/test_collations.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5469 2023-03-21 14:20:18.000000 elementpath-4.1.3/tests/test_compare.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    86399 2023-03-21 14:20:18.000000 elementpath-4.1.3/tests/test_datatypes.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1114 2021-01-06 17:09:53.000000 elementpath-4.1.3/tests/test_elementpath.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19106 2023-03-21 14:20:18.000000 elementpath-4.1.3/tests/test_etree.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3715 2023-03-21 14:20:18.000000 elementpath-4.1.3/tests/test_exceptions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11284 2023-04-11 07:36:42.000000 elementpath-4.1.3/tests/test_helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2904 2023-03-21 14:20:18.000000 elementpath-4.1.3/tests/test_namespaces.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     2789 2022-07-16 19:41:23.000000 elementpath-4.1.3/tests/test_package.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    43489 2023-03-21 14:20:19.000000 elementpath-4.1.3/tests/test_regex.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     9798 2023-02-01 12:54:01.000000 elementpath-4.1.3/tests/test_schema_context.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    20182 2023-02-01 12:54:01.000000 elementpath-4.1.3/tests/test_schema_proxy.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3793 2023-04-28 14:38:26.000000 elementpath-4.1.3/tests/test_selectors.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    15434 2023-04-28 14:38:26.000000 elementpath-4.1.3/tests/test_sequence_types.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    17460 2023-04-28 14:38:26.000000 elementpath-4.1.3/tests/test_serialization.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    16558 2023-04-28 14:38:26.000000 elementpath-4.1.3/tests/test_tdop_parser.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7919 2023-04-28 14:38:26.000000 elementpath-4.1.3/tests/test_tree_builders.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1446 2023-06-17 17:40:45.000000 elementpath-4.1.3/tests/test_typing.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2068 2023-03-21 14:20:19.000000 elementpath-4.1.3/tests/test_validators.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    84397 2023-06-17 17:40:45.000000 elementpath-4.1.3/tests/test_xpath1_parser.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    33795 2023-03-21 14:20:19.000000 elementpath-4.1.3/tests/test_xpath2_constructors.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    86351 2023-02-01 12:54:01.000000 elementpath-4.1.3/tests/test_xpath2_functions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    67321 2023-04-11 07:36:42.000000 elementpath-4.1.3/tests/test_xpath2_parser.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    60913 2023-06-17 17:40:45.000000 elementpath-4.1.3/tests/test_xpath30.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    47783 2023-03-21 14:20:19.000000 elementpath-4.1.3/tests/test_xpath31.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    12435 2022-07-16 19:41:23.000000 elementpath-4.1.3/tests/test_xpath_context.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    17766 2023-04-28 14:38:26.000000 elementpath-4.1.3/tests/test_xpath_nodes.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    35390 2023-04-26 14:25:47.000000 elementpath-4.1.3/tests/test_xpath_tokens.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    12175 2023-06-17 17:40:45.000000 elementpath-4.1.3/tests/xpath_test_class.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1592 2023-06-17 17:40:45.000000 elementpath-4.1.3/tox.ini
```

### Comparing `elementpath-4.1.2/CHANGELOG.rst` & `elementpath-4.1.3/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 *********
 CHANGELOG
 *********
 
+`v4.1.3`_ (2023-06-17)
+======================
+* Fix XP30+ fn:path (issue #67)
+* Fix weak tests (issues #64 and #66)
+
 `v4.1.2`_ (2023-04-28)
 ======================
 * Add support for Python 3.12
 * Fix self shortcut operator (adding is_schema_node() to node classes)
 
 `v4.1.1`_ (2023-04-11)
 ======================
@@ -414,7 +419,8 @@
 .. _v3.0.1: https://github.com/sissaschool/elementpath/compare/v3.0.0...v3.0.1
 .. _v3.0.2: https://github.com/sissaschool/elementpath/compare/v3.0.1...v3.0.2
 .. _v4.0.0: https://github.com/sissaschool/elementpath/compare/v3.0.2...v4.0.0
 .. _v4.0.1: https://github.com/sissaschool/elementpath/compare/v4.0.0...v4.0.1
 .. _v4.1.0: https://github.com/sissaschool/elementpath/compare/v4.0.1...v4.1.0
 .. _v4.1.1: https://github.com/sissaschool/elementpath/compare/v4.1.0...v4.1.1
 .. _v4.1.2: https://github.com/sissaschool/elementpath/compare/v4.1.1...v4.1.2
+.. _v4.1.3: https://github.com/sissaschool/elementpath/compare/v4.1.2...v4.1.3
```

### Comparing `elementpath-4.1.2/LICENSE` & `elementpath-4.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/PKG-INFO` & `elementpath-4.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elementpath
-Version: 4.1.2
+Version: 4.1.3
 Summary: XPath 1.0/2.0/3.0/3.1 parsers and selectors for ElementTree and lxml
 Home-page: https://github.com/sissaschool/elementpath
 Author: Davide Brunato
 Author-email: brunato@sissa.it
 License: MIT
 Keywords: XPath,XPath2,XPath3,XPath31,Pratt-parser,ElementTree,lxml
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `elementpath-4.1.2/README.rst` & `elementpath-4.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/doc/Makefile` & `elementpath-4.1.3/doc/Makefile`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/doc/advanced.rst` & `elementpath-4.1.3/doc/advanced.rst`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/doc/conf.py` & `elementpath-4.1.3/doc/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 project = 'elementpath'
 copyright = '2018-2023, SISSA (International School for Advanced Studies)'
 author = 'Davide Brunato'
 
 # The short X.Y version
 version = '4.1'
 # The full version, including alpha/beta/rc tags
-release = '4.1.2'
+release = '4.1.3'
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `elementpath-4.1.2/doc/make.bat` & `elementpath-4.1.3/doc/make.bat`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/doc/pratt_api.rst` & `elementpath-4.1.3/doc/pratt_api.rst`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/doc/xpath_api.rst` & `elementpath-4.1.3/doc/xpath_api.rst`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/__init__.py` & `elementpath-4.1.3/elementpath/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # All rights reserved.
 # This file is distributed under the terms of the MIT License.
 # See the file 'LICENSE' in the root directory of the present
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
-__version__ = '4.1.2'
+__version__ = '4.1.3'
 __author__ = "Davide Brunato"
 __contact__ = "brunato@sissa.it"
 __copyright__ = "Copyright 2018-2023, SISSA"
 __license__ = "MIT"
 __status__ = "Production/Stable"
 
 # Imports here are considered as stable API, other internal calls may change.
```

### Comparing `elementpath-4.1.2/elementpath/collations.py` & `elementpath-4.1.3/elementpath/collations.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/compare.py` & `elementpath-4.1.3/elementpath/compare.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/datatypes/__init__.py` & `elementpath-4.1.3/elementpath/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/datatypes/atomic_types.py` & `elementpath-4.1.3/elementpath/datatypes/atomic_types.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/datatypes/binary.py` & `elementpath-4.1.3/elementpath/datatypes/binary.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/datatypes/datetime.py` & `elementpath-4.1.3/elementpath/datatypes/datetime.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/datatypes/numeric.py` & `elementpath-4.1.3/elementpath/datatypes/numeric.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/datatypes/proxies.py` & `elementpath-4.1.3/elementpath/datatypes/proxies.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/datatypes/qname.py` & `elementpath-4.1.3/elementpath/datatypes/qname.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/datatypes/string.py` & `elementpath-4.1.3/elementpath/datatypes/string.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/datatypes/untyped.py` & `elementpath-4.1.3/elementpath/datatypes/untyped.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/datatypes/uri.py` & `elementpath-4.1.3/elementpath/datatypes/uri.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/etree.py` & `elementpath-4.1.3/elementpath/etree.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/exceptions.py` & `elementpath-4.1.3/elementpath/exceptions.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/helpers.py` & `elementpath-4.1.3/elementpath/helpers.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/namespaces.py` & `elementpath-4.1.3/elementpath/namespaces.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/protocols.py` & `elementpath-4.1.3/elementpath/protocols.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/regex/__init__.py` & `elementpath-4.1.3/elementpath/regex/__init__.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/regex/character_classes.py` & `elementpath-4.1.3/elementpath/regex/character_classes.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/regex/codepoints.py` & `elementpath-4.1.3/elementpath/regex/codepoints.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/regex/generate_categories.py` & `elementpath-4.1.3/elementpath/regex/generate_categories.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/regex/patterns.py` & `elementpath-4.1.3/elementpath/regex/patterns.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/regex/unicode_categories.py` & `elementpath-4.1.3/elementpath/regex/unicode_categories.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/regex/unicode_subsets.py` & `elementpath-4.1.3/elementpath/regex/unicode_subsets.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/schema_proxy.py` & `elementpath-4.1.3/elementpath/schema_proxy.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/sequence_types.py` & `elementpath-4.1.3/elementpath/sequence_types.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/serialization.py` & `elementpath-4.1.3/elementpath/serialization.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/tdop.py` & `elementpath-4.1.3/elementpath/tdop.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/tree_builders.py` & `elementpath-4.1.3/elementpath/tree_builders.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/validators/__init__.py` & `elementpath-4.1.3/elementpath/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/validators/analyze-string.xsd` & `elementpath-4.1.3/elementpath/validators/analyze-string.xsd`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/validators/schema-for-json.xsd` & `elementpath-4.1.3/elementpath/validators/schema-for-json.xsd`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/xpath1/_xpath1_axes.py` & `elementpath-4.1.3/elementpath/xpath1/_xpath1_axes.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/xpath1/_xpath1_functions.py` & `elementpath-4.1.3/elementpath/xpath1/_xpath1_functions.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/xpath1/_xpath1_operators.py` & `elementpath-4.1.3/elementpath/xpath1/_xpath1_operators.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/xpath1/xpath1_parser.py` & `elementpath-4.1.3/elementpath/xpath1/xpath1_parser.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/xpath2/__init__.py` & `elementpath-4.1.3/elementpath/xpath2/__init__.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/xpath2/_xpath2_constructors.py` & `elementpath-4.1.3/elementpath/xpath2/_xpath2_constructors.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/xpath2/_xpath2_functions.py` & `elementpath-4.1.3/elementpath/xpath2/_xpath2_functions.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/xpath2/_xpath2_operators.py` & `elementpath-4.1.3/elementpath/xpath2/_xpath2_operators.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/xpath2/xpath2_parser.py` & `elementpath-4.1.3/elementpath/xpath2/xpath2_parser.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/xpath30/__init__.py` & `elementpath-4.1.3/elementpath/xpath30/__init__.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/xpath30/_translation_maps.py` & `elementpath-4.1.3/elementpath/xpath30/_translation_maps.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/xpath30/_xpath30_functions.py` & `elementpath-4.1.3/elementpath/xpath30/_xpath30_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1082,16 +1082,20 @@
         else:
             suffix = f'/namespace::*[Q{{{XPATH_FUNCTIONS_NAMESPACE}}}local-name()=""]'
     else:
         return []
 
     if isinstance(context.root, DocumentNode):
         root = context.root.getroot().elem
-        path = f'/Q{root.tag}[1]'
+        if root.tag.startswith('{'):
+            path = f'/Q{root.tag}[1]'
+        else:
+            path = f'/Q{{}}{root.tag}[1]'
     else:
+        # If root is an element use the function that returns the root of the tree
         root = context.root.elem
         path = 'Q{%s}root()' % XPATH_FUNCTIONS_NAMESPACE
 
     if isinstance(item, ProcessingInstructionNode):
         if item.parent is None or isinstance(item.parent, DocumentNode):
             return f'/processing-instruction({item.name})[{context.position}]'
     elif isinstance(item, CommentNode):
```

### Comparing `elementpath-4.1.2/elementpath/xpath30/_xpath30_operators.py` & `elementpath-4.1.3/elementpath/xpath30/_xpath30_operators.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/xpath30/xpath30_helpers.py` & `elementpath-4.1.3/elementpath/xpath30/xpath30_helpers.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/xpath30/xpath30_parser.py` & `elementpath-4.1.3/elementpath/xpath30/xpath30_parser.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/xpath31/__init__.py` & `elementpath-4.1.3/elementpath/xpath31/__init__.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/xpath31/_xpath31_functions.py` & `elementpath-4.1.3/elementpath/xpath31/_xpath31_functions.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/xpath31/_xpath31_operators.py` & `elementpath-4.1.3/elementpath/xpath31/_xpath31_operators.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/xpath31/xpath31_parser.py` & `elementpath-4.1.3/elementpath/xpath31/xpath31_parser.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/xpath_context.py` & `elementpath-4.1.3/elementpath/xpath_context.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/xpath_nodes.py` & `elementpath-4.1.3/elementpath/xpath_nodes.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/xpath_selectors.py` & `elementpath-4.1.3/elementpath/xpath_selectors.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath/xpath_tokens.py` & `elementpath-4.1.3/elementpath/xpath_tokens.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/elementpath.egg-info/PKG-INFO` & `elementpath-4.1.3/elementpath.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elementpath
-Version: 4.1.2
+Version: 4.1.3
 Summary: XPath 1.0/2.0/3.0/3.1 parsers and selectors for ElementTree and lxml
 Home-page: https://github.com/sissaschool/elementpath
 Author: Davide Brunato
 Author-email: brunato@sissa.it
 License: MIT
 Keywords: XPath,XPath2,XPath3,XPath31,Pratt-parser,ElementTree,lxml
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `elementpath-4.1.2/elementpath.egg-info/SOURCES.txt` & `elementpath-4.1.3/elementpath.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/setup.py` & `elementpath-4.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from setuptools import setup, find_packages
 
 with open("README.rst") as readme:
     long_description = readme.read()
 
 setup(
     name='elementpath',
-    version='4.1.2',
+    version='4.1.3',
     packages=find_packages(include=['elementpath', 'elementpath.*']),
     package_data={
         'elementpath': ['py.typed'],
         'elementpath.validators': ['analyze-string.xsd', 'schema-for-json.xsd'],
     },
     author='Davide Brunato',
     author_email='brunato@sissa.it',
```

### Comparing `elementpath-4.1.2/tests/execute_w3c_tests.py` & `elementpath-4.1.3/tests/execute_w3c_tests.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/tests/memory_profiling.py` & `elementpath-4.1.3/tests/memory_profiling.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/tests/resources/analyze-string.xsd` & `elementpath-4.1.3/tests/resources/analyze-string.xsd`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/tests/resources/schema-for-json.xsd` & `elementpath-4.1.3/tests/resources/schema-for-json.xsd`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/tests/test_collations.py` & `elementpath-4.1.3/tests/test_collations.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/tests/test_compare.py` & `elementpath-4.1.3/tests/test_compare.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/tests/test_datatypes.py` & `elementpath-4.1.3/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/tests/test_elementpath.py` & `elementpath-4.1.3/tests/test_elementpath.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/tests/test_etree.py` & `elementpath-4.1.3/tests/test_etree.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/tests/test_exceptions.py` & `elementpath-4.1.3/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/tests/test_helpers.py` & `elementpath-4.1.3/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/tests/test_namespaces.py` & `elementpath-4.1.3/tests/test_namespaces.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/tests/test_package.py` & `elementpath-4.1.3/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/tests/test_regex.py` & `elementpath-4.1.3/tests/test_regex.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/tests/test_schema_context.py` & `elementpath-4.1.3/tests/test_schema_context.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/tests/test_schema_proxy.py` & `elementpath-4.1.3/tests/test_schema_proxy.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/tests/test_selectors.py` & `elementpath-4.1.3/tests/test_selectors.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/tests/test_sequence_types.py` & `elementpath-4.1.3/tests/test_sequence_types.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/tests/test_serialization.py` & `elementpath-4.1.3/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/tests/test_tdop_parser.py` & `elementpath-4.1.3/tests/test_tdop_parser.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/tests/test_tree_builders.py` & `elementpath-4.1.3/tests/test_tree_builders.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/tests/test_typing.py` & `elementpath-4.1.3/tests/test_typing.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,50 +7,43 @@
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
 """Tests about static typing of elementpath objects."""
 
 import unittest
-import subprocess
-import re
 import sys
+import importlib
 from pathlib import Path
 
 try:
-    import mypy
+    from mypy import api as mypy_api
 except ImportError:
-    mypy = None
+    mypy_api = None
 
+try:
+    lxml_stubs_module = importlib.import_module('lxml-stubs')
+except ImportError:
+    lxml_stubs_module = None
 
-@unittest.skipIf(mypy is None, "mypy is not installed")
+
+@unittest.skipIf(mypy_api is None, "mypy is not installed")
+@unittest.skipIf(lxml_stubs_module is None, "lxml-stubs is not installed")
 @unittest.skipIf(sys.version_info < (3, 8), "Python version is lesser than 3.8")
 class TestTyping(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
         cls.cases_dir = Path(__file__).parent.joinpath('mypy_tests')
         cls.config_file = Path(__file__).parent.parent.joinpath('mypy.ini')
-        cls.error_pattern = re.compile(r'Found \d+ error', re.IGNORECASE)
-
-    def check_mypy_output(self, testfile, *options):
-        cmd = ['mypy', '--config-file', str(self.config_file), testfile]
-        if options:
-            cmd.extend(str(opt) for opt in options)
-        process = subprocess.run(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-
-        self.assertEqual(process.stderr, b'')
-        output = process.stdout.decode('utf-8').strip()
-        output_lines = output.split('\n')
-
-        self.assertGreater(len(output_lines), 0, msg=output)
-        self.assertNotRegex(output_lines[-1], self.error_pattern, msg=output)
-        return output_lines
 
     def test_selectors(self):
-        case_path = self.cases_dir.joinpath('selectors.py')
-        output_lines = self.check_mypy_output(case_path, '--strict')
-        self.assertTrue(output_lines[0].startswith('Success:'), msg='\n'.join(output_lines))
+        result = mypy_api.run([
+            '--strict',
+            '--config-file', str(self.config_file),
+            str(self.cases_dir.joinpath('selectors.py'))
+        ])
+        self.assertEqual(result[2], 0, msg=result[1] or result[0])
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `elementpath-4.1.2/tests/test_validators.py` & `elementpath-4.1.3/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/tests/test_xpath1_parser.py` & `elementpath-4.1.3/tests/test_xpath1_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 #       References:
 #           http://www.w3.org/TR/1999/REC-xpath-19991116/
 #           http://www.w3.org/TR/2010/REC-xpath20-20101214/
 #           http://www.w3.org/TR/2010/REC-xpath-functions-20101214/
 #           https://www.w3.org/Consortium/Legal/2015/doc-license
 #           https://www.w3.org/TR/charmod-norm/
 #
-import sys
 import unittest
 import io
 import math
 import pickle
 from decimal import Decimal
 from textwrap import dedent
 from typing import Optional, List, Tuple
@@ -1126,18 +1125,15 @@
         self.check_selector("count(@min | @max) = 1", root, False)
         self.check_selector("count(@min | @max) = 2", root, True)
 
     def test_sum_function(self):
         root = self.etree.XML(XML_DATA_TEST)
         context = XPathContext(root, variables=self.variables)
         self.check_value("sum($values)", 35, context)
-        if sys.version_info < (3, 12):
-            self.check_selector("sum(/values/a)", root, 13.299999999999999)
-        else:
-            self.check_selector("sum(/values/a)", root, 13.3)
+        self.check_selector("sum(/values/a)", root, 13.3)
 
         if self.parser.version == '1.0':
             self.check_selector("sum(/values/*)", root, math.isnan)
             self.wrong_syntax("sum(())")
         else:
             self.check_selector("sum(/values/*)", root, TypeError)
             self.check_value("sum(())", 0)
@@ -1675,14 +1671,25 @@
                 namespaces = {k: v for k, v in namespaces.items() if k}
 
             if isinstance(expected, set):
                 self.assertEqual(
                     set(root.xpath(path, namespaces=namespaces, **variables)), expected
                 )
                 self.assertEqual(set(results), expected)
+            elif isinstance(expected, float):
+                if math.isnan(expected):
+                    self.assertTrue(math.isnan(
+                        root.xpath(path, namespaces=namespaces, **variables)
+                    ))
+                    self.assertTrue(math.isnan(results))
+                else:
+                    self.assertAlmostEqual(
+                        root.xpath(path, namespaces=namespaces, **variables), expected
+                    )
+                    self.assertAlmostEqual(results, expected)
             elif not callable(expected):
                 self.assertEqual(root.xpath(path, namespaces=namespaces, **variables), expected)
                 self.assertEqual(results, expected)
             elif isinstance(expected, type):
                 self.assertTrue(isinstance(results, expected))
             else:
                 self.assertTrue(expected(results))
```

### Comparing `elementpath-4.1.2/tests/test_xpath2_constructors.py` & `elementpath-4.1.3/tests/test_xpath2_constructors.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/tests/test_xpath2_functions.py` & `elementpath-4.1.3/tests/test_xpath2_functions.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/tests/test_xpath2_parser.py` & `elementpath-4.1.3/tests/test_xpath2_parser.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/tests/test_xpath30.py` & `elementpath-4.1.3/tests/test_xpath30.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,36 +15,38 @@
 #       References:
 #           https://www.w3.org/TR/xpath-3/
 #           https://www.w3.org/TR/xpath-30/
 #           https://www.w3.org/TR/xpath-31/
 #           https://www.w3.org/Consortium/Legal/2015/doc-license
 #           https://www.w3.org/TR/charmod-norm/
 #
+import io
 import unittest
 import os
 import re
 import math
 import pathlib
 import platform
 import xml.etree.ElementTree as ElementTree
+from textwrap import dedent
 from typing import cast
 
 try:
     import lxml.etree as lxml_etree
 except ImportError:
     lxml_etree = None
 
 try:
     import xmlschema
 except ImportError:
     xmlschema = None
 else:
     xmlschema.XMLSchema.meta_schema.build()
 
-from elementpath import XPathContext, MissingContextError, datatypes, XPathFunction
+from elementpath import select, XPathContext, MissingContextError, datatypes, XPathFunction
 from elementpath.namespaces import XPATH_FUNCTIONS_NAMESPACE
 from elementpath.etree import is_etree_element, is_lxml_etree_document, is_etree_document
 from elementpath.xpath_nodes import ElementNode, DocumentNode
 from elementpath.xpath3 import XPath30Parser
 from elementpath.xpath30.xpath30_helpers import PICTURE_PATTERN, \
     int_to_roman, int_to_alphabetic, int_to_words
 
@@ -1175,14 +1177,101 @@
                          "-EIGHT THOUSAND NINE HUNDRED AND TWELVE")
         self.check_value("format-integer(17089674, 'Ww')",
                          "Seventeen Million Eighty-Nine Thousand Six Hundred And Seventy-Four")
 
         self.check_value("format-integer(123, '0000')", '0123')
         self.check_source("format-integer(-8912, 'W')")
 
+    def test_path_function__issue_067(self):
+        xml_sample = dedent("""
+            <root>
+                <item>
+                    <name>item 1</name>
+                    <value>value 1</value>
+                </item>
+            </root>""")
+
+        root = self.etree.parse(io.StringIO(xml_sample))
+        paths = select(root, '//*/path()', parser=self.parser.__class__)
+        expected = [
+            '/Q{}root[1]',
+            '/Q{}root[1]/Q{}item[1]',
+            '/Q{}root[1]/Q{}item[1]/Q{}name[1]',
+            '/Q{}root[1]/Q{}item[1]/Q{}value[1]'
+        ]
+        self.assertListEqual(paths, expected)
+
+        root = self.etree.XML(xml_sample)
+        paths = select(root, '//*/path()', parser=self.parser.__class__)
+
+        expected = [
+            'Q{http://www.w3.org/2005/xpath-functions}root()',
+            'Q{http://www.w3.org/2005/xpath-functions}root()/Q{}item[1]',
+            'Q{http://www.w3.org/2005/xpath-functions}root()/Q{}item[1]/Q{}name[1]',
+            'Q{http://www.w3.org/2005/xpath-functions}root()/Q{}item[1]/Q{}value[1]'
+        ]
+        self.assertListEqual(paths, expected)
+
+    def test_path_function_with_namespaces(self):
+        xml_sample = dedent("""
+            <tns:root xmlns:tns="http://xpath.test/ns">
+                <item>
+                    <name>item 1</name>
+                    <foo:value xmlns:foo="bar">value 1</foo:value>
+                </item>
+            </tns:root>""")
+
+        root = self.etree.parse(io.StringIO(xml_sample))
+        paths = select(root, '//*/path()', parser=self.parser.__class__)
+        expected = [
+            '/Q{http://xpath.test/ns}root[1]',
+            '/Q{http://xpath.test/ns}root[1]/Q{}item[1]',
+            '/Q{http://xpath.test/ns}root[1]/Q{}item[1]/Q{}name[1]',
+            '/Q{http://xpath.test/ns}root[1]/Q{}item[1]/Q{bar}value[1]'
+        ]
+        self.assertListEqual(paths, expected)
+
+        root = self.etree.XML(xml_sample)
+        paths = select(root, '//*/path()', parser=self.parser.__class__)
+
+        expected = [
+            'Q{http://www.w3.org/2005/xpath-functions}root()',
+            'Q{http://www.w3.org/2005/xpath-functions}root()/Q{}item[1]',
+            'Q{http://www.w3.org/2005/xpath-functions}root()/Q{}item[1]/Q{}name[1]',
+            'Q{http://www.w3.org/2005/xpath-functions}root()/Q{}item[1]/Q{bar}value[1]'
+        ]
+        self.assertListEqual(paths, expected)
+
+    def test_path_function_with_same_child(self):
+        xml_sample = dedent("""
+            <tns:root xmlns:tns="http://xpath.test/ns">
+                <item>
+                    <name>item 1</name>
+                    <value>value 1</value>
+                    <name>item 2</name>
+                    <name>item 3</name>
+                </item>
+                <item2/>
+                <item/>
+            </tns:root>""")
+
+        root = self.etree.parse(io.StringIO(xml_sample))
+        paths = select(root, '//*/path()', parser=self.parser.__class__)
+        expected = [
+            '/Q{http://xpath.test/ns}root[1]',
+            '/Q{http://xpath.test/ns}root[1]/Q{}item[1]',
+            '/Q{http://xpath.test/ns}root[1]/Q{}item[1]/Q{}name[1]',
+            '/Q{http://xpath.test/ns}root[1]/Q{}item[1]/Q{}value[1]',
+            '/Q{http://xpath.test/ns}root[1]/Q{}item[1]/Q{}name[2]',
+            '/Q{http://xpath.test/ns}root[1]/Q{}item[1]/Q{}name[3]',
+            '/Q{http://xpath.test/ns}root[1]/Q{}item2[1]',
+            '/Q{http://xpath.test/ns}root[1]/Q{}item[2]',
+        ]
+        self.assertListEqual(paths, expected)
+
 
 @unittest.skipIf(lxml_etree is None, "The lxml library is not installed")
 class LxmlXPath30FunctionsTest(XPath30FunctionsTest):
     etree = lxml_etree
 
 
 class XPath30ConstructorsTest(test_xpath2_constructors.XPath2ConstructorsTest):
```

### Comparing `elementpath-4.1.2/tests/test_xpath31.py` & `elementpath-4.1.3/tests/test_xpath31.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/tests/test_xpath_context.py` & `elementpath-4.1.3/tests/test_xpath_context.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/tests/test_xpath_nodes.py` & `elementpath-4.1.3/tests/test_xpath_nodes.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/tests/test_xpath_tokens.py` & `elementpath-4.1.3/tests/test_xpath_tokens.py`

 * *Files identical despite different names*

### Comparing `elementpath-4.1.2/tests/xpath_test_class.py` & `elementpath-4.1.3/tests/xpath_test_class.py`

 * *Files 5% similar despite different names*

```diff
@@ -141,32 +141,39 @@
         try:
             root_token = self.parser.parse(path)
         except ElementPathError as err:
             if isinstance(expected, type) and isinstance(err, expected):
                 return
             raise
 
-        if isinstance(expected, type) and issubclass(expected, Exception):
-            self.assertRaises(expected, root_token.evaluate, context)
-        elif isinstance(expected, float) and math.isnan(expected):
+        if isinstance(expected, type):
+            if issubclass(expected, Exception):
+                self.assertRaises(expected, root_token.evaluate, context)
+            else:
+                self.assertIsInstance(root_token.evaluate(context), expected)
+
+        elif isinstance(expected, float):
             value = root_token.evaluate(context)
-            if isinstance(value, list):
-                self.assertTrue(any(math.isnan(x) for x in value))
+            if not math.isnan(expected):
+                self.assertAlmostEqual(value, expected)
             else:
+                if isinstance(value, list):
+                    value = [x for x in value if value is not None and value != []]
+                    self.assertTrue(len(value) == 1)
+                    value = value[0]
+
+                self.assertIsInstance(value, float)
                 self.assertTrue(math.isnan(value))
 
-        elif isinstance(expected, list) and expected:
+        elif isinstance(expected, list):
             self.assertListEqual(root_token.evaluate(context), expected)
         elif isinstance(expected, set):
             self.assertEqual(set(root_token.evaluate(context)), expected)
         elif isinstance(expected, XPathFunction) or not callable(expected):
             self.assertEqual(root_token.evaluate(context), expected)
-        elif isinstance(expected, type):
-            value = root_token.evaluate(context)
-            self.assertIsInstance(value, expected)
         else:
             self.assertTrue(expected(root_token.evaluate(context)))
 
     def check_select(self, path, expected, context=None):
         """
         Checks the materialized result of the *select* method with an XPath expression.
         The selection is applied on the root token of the parsed XPath expression.
@@ -186,18 +193,18 @@
         root_token = self.parser.parse(path)
         if isinstance(expected, type) and issubclass(expected, Exception):
             self.assertRaises(expected, root_token.select, context)
         elif isinstance(expected, list):
             self.assertListEqual(list(root_token.select(context)), expected)
         elif isinstance(expected, set):
             self.assertEqual(set(root_token.select(context)), expected)
-        elif isinstance(expected, XPathFunction) or not callable(expected):
-            self.assertEqual(list(root_token.select(context)), expected)
-        else:
+        elif callable(expected):
             self.assertTrue(expected(list(root_token.parser.parse(path).select(context))))
+        else:
+            self.assertEqual(list(root_token.select(context)), expected)  # must fail
 
     def check_selector(self, path, root, expected, namespaces=None, **kwargs):
         """
         Checks using the selector API, namely the *select* function at package level.
 
         :param path: an XPath expression.
         :param root: an Element or an ElementTree instance.
@@ -213,16 +220,19 @@
                               self.parser.__class__, **kwargs)
         else:
             results = select(root, path, namespaces, self.parser.__class__, **kwargs)
             if isinstance(expected, list):
                 self.assertListEqual(results, expected)
             elif isinstance(expected, set):
                 self.assertEqual(set(results), expected)
-            elif isinstance(expected, float) and math.isnan(expected):
-                self.assertTrue(math.isnan(results))
+            elif isinstance(expected, float):
+                if math.isnan(expected):
+                    self.assertTrue(math.isnan(results))
+                else:
+                    self.assertAlmostEqual(results, expected)
             elif not callable(expected):
                 self.assertEqual(results, expected)
             elif isinstance(expected, type):
                 self.assertIsInstance(results, expected)
             else:
                 self.assertTrue(expected(results))
```

### Comparing `elementpath-4.1.2/tox.ini` & `elementpath-4.1.3/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Tox (http://tox.testrun.org/) is a tool for running tests
 # in multiple virtualenvs. This configuration file will run the
 # test suite on all supported python versions. To use it, "pip install tox"
 # and then run "tox" from this directory.
 
 [tox]
+min_version = 4.0
 envlist =
     py{37,38,39,310,311,312}, pypy3, xmlschema{20},
     docs, flake8, mypy-py{38,39,310,311,312,py3}, pytest, coverage
 skip_missing_interpreters = true
 work_dir = {tox_root}/../.tox/elementpath
 
 [testenv]
@@ -42,15 +43,15 @@
     flake8
 commands =
     flake8 elementpath
     flake8 tests
 
 [testenv:mypy-py{38,39,310,311,312,py3}]
 deps =
-    mypy==1.2.0
+    mypy==1.3.0
     xmlschema
     lxml-stubs
 commands =
     mypy --strict elementpath
     python tests/test_typing.py
 
 [testenv:coverage]
```

