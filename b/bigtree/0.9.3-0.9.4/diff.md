# Comparing `tmp/bigtree-0.9.3.tar.gz` & `tmp/bigtree-0.9.4.tar.gz`

## Comparing `bigtree-0.9.3.tar` & `bigtree-0.9.4.tar`

### file list

```diff
@@ -1,107 +1,109 @@
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 bigtree-0.9.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 bigtree-0.9.3/.readthedocs.yaml
--rw-r--r--   0        0        0    12475 2020-02-02 00:00:00.000000 bigtree-0.9.3/CHANGELOG.md
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 bigtree-0.9.3/CONTRIBUTING.md
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 bigtree-0.9.3/SECURITY.md
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 bigtree-0.9.3/.github/workflows/codecov.yml
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 bigtree-0.9.3/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 bigtree-0.9.3/.github/workflows/pytest.yml
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 bigtree-0.9.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0   757076 2020-02-02 00:00:00.000000 bigtree-0.9.3/assets/DejaVuSans.ttf
--rw-r--r--   0        0        0    20084 2020-02-02 00:00:00.000000 bigtree-0.9.3/assets/binarytree.png
--rw-r--r--   0        0        0    11224 2020-02-02 00:00:00.000000 bigtree-0.9.3/assets/custom_tree.png
--rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 bigtree-0.9.3/assets/dag_construct.png
--rw-r--r--   0        0        0    12108 2020-02-02 00:00:00.000000 bigtree-0.9.3/assets/demo.png
--rw-r--r--   0        0        0    17554 2020-02-02 00:00:00.000000 bigtree-0.9.3/assets/demo_binarytree.png
--rw-r--r--   0        0        0    19320 2020-02-02 00:00:00.000000 bigtree-0.9.3/assets/demo_dag.png
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 bigtree-0.9.3/assets/demo_pillow.png
--rw-r--r--   0        0        0    10235 2020-02-02 00:00:00.000000 bigtree-0.9.3/assets/demo_tree.png
--rw-r--r--   0        0        0   313013 2020-02-02 00:00:00.000000 bigtree-0.9.3/assets/modify_advanced.png
--rw-r--r--   0        0        0   180588 2020-02-02 00:00:00.000000 bigtree-0.9.3/assets/modify_shift_and_copy.png
--rw-r--r--   0        0        0    67777 2020-02-02 00:00:00.000000 bigtree-0.9.3/assets/tree_construct.png
--rw-r--r--   0        0        0    11482 2020-02-02 00:00:00.000000 bigtree-0.9.3/assets/weighted_tree.png
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/py.typed
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/binarytree/construct.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/dag/__init__.py
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/dag/construct.py
--rw-r--r--   0        0        0     9742 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/dag/export.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/node/__init__.py
--rw-r--r--   0        0        0    21938 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/node/basenode.py
--rw-r--r--   0        0        0    13631 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/node/binarynode.py
--rw-r--r--   0        0        0    18189 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/node/dagnode.py
--rw-r--r--   0        0        0     6718 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/node/node.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/tree/__init__.py
--rw-r--r--   0        0        0    33748 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/tree/construct.py
--rw-r--r--   0        0        0    30233 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/tree/export.py
--rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/tree/helper.py
--rw-r--r--   0        0        0    33168 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/tree/modify.py
--rw-r--r--   0        0        0    12597 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/tree/search.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/utils/__init__.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/utils/exceptions.py
--rw-r--r--   0        0        0    13884 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/utils/iterators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/workflows/__init__.py
--rw-r--r--   0        0        0     6533 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/workflows/app_calendar.py
--rw-r--r--   0        0        0     8516 2020-02-02 00:00:00.000000 bigtree-0.9.3/bigtree/workflows/app_todo.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/make.bat
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/requirements.txt
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/binarytree.rst
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/conf.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/dag.rst
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/index.rst
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/node.rst
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/others.rst
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/tree.rst
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/utils.rst
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/workflows.rst
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/_static/custom.css
--rw-r--r--   0        0        0    27138 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/_static/favicon.ico
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/_templates/layout.html
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/bigtree/binarytree/construct.rst
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/bigtree/dag/construct.rst
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/bigtree/dag/export.rst
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/bigtree/node/basenode.rst
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/bigtree/node/binarynode.rst
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/bigtree/node/dagnode.rst
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/bigtree/node/node.rst
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/bigtree/tree/construct.rst
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/bigtree/tree/export.rst
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/bigtree/tree/helper.rst
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/bigtree/tree/modify.rst
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/bigtree/tree/search.rst
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/bigtree/utils/iterators.rst
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/bigtree/workflows/app_todo.rst
--rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/others/contributing.rst
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/others/list_dir.md
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/others/merging_trees.md
--rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/others/nodes.md
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/others/tips.rst
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 bigtree-0.9.3/docs/source/others/weighted_trees.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/__init__.py
--rw-r--r--   0        0        0     9434 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/binarytree/__init__.py
--rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/binarytree/test_construct.py
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/binarytree/test_export.py
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/binarytree/test_helper.py
--rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/binarytree/test_search.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/dag/__init__.py
--rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/dag/test_construct.py
--rw-r--r--   0        0        0    13410 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/dag/test_export.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/node/__init__.py
--rw-r--r--   0        0        0    31896 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/node/test_basenode.py
--rw-r--r--   0        0        0    36199 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/node/test_binarynode.py
--rw-r--r--   0        0        0    31052 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/node/test_dagnode.py
--rw-r--r--   0        0        0    13563 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/node/test_node.py
--rw-r--r--   0        0        0    57110 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/tree/test_construct.py
--rw-r--r--   0        0        0    36938 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/tree/test_export.py
--rw-r--r--   0        0        0     4737 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/tree/test_helper.py
--rw-r--r--   0        0        0    67770 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/tree/test_modify.py
--rw-r--r--   0        0        0    17729 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/tree/test_search.py
--rw-r--r--   0        0        0    13545 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/utils/test_iterators.py
--rw-r--r--   0        0        0    17809 2020-02-02 00:00:00.000000 bigtree-0.9.3/tests/workflows/test_todo.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 bigtree-0.9.3/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 bigtree-0.9.3/LICENSE
--rw-r--r--   0        0        0    25288 2020-02-02 00:00:00.000000 bigtree-0.9.3/README.md
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 bigtree-0.9.3/pyproject.toml
--rw-r--r--   0        0        0    26396 2020-02-02 00:00:00.000000 bigtree-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 bigtree-0.9.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 bigtree-0.9.4/.readthedocs.yaml
+-rw-r--r--   0        0        0    13366 2020-02-02 00:00:00.000000 bigtree-0.9.4/CHANGELOG.md
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 bigtree-0.9.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 bigtree-0.9.4/SECURITY.md
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 bigtree-0.9.4/.github/workflows/codecov.yml
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 bigtree-0.9.4/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 bigtree-0.9.4/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 bigtree-0.9.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0   757076 2020-02-02 00:00:00.000000 bigtree-0.9.4/assets/DejaVuSans.ttf
+-rw-r--r--   0        0        0    20084 2020-02-02 00:00:00.000000 bigtree-0.9.4/assets/binarytree.png
+-rw-r--r--   0        0        0    11224 2020-02-02 00:00:00.000000 bigtree-0.9.4/assets/custom_tree.png
+-rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 bigtree-0.9.4/assets/dag_construct.png
+-rw-r--r--   0        0        0    12108 2020-02-02 00:00:00.000000 bigtree-0.9.4/assets/demo.png
+-rw-r--r--   0        0        0    17554 2020-02-02 00:00:00.000000 bigtree-0.9.4/assets/demo_binarytree.png
+-rw-r--r--   0        0        0    19320 2020-02-02 00:00:00.000000 bigtree-0.9.4/assets/demo_dag.png
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 bigtree-0.9.4/assets/demo_pillow.png
+-rw-r--r--   0        0        0    10235 2020-02-02 00:00:00.000000 bigtree-0.9.4/assets/demo_tree.png
+-rw-r--r--   0        0        0   313013 2020-02-02 00:00:00.000000 bigtree-0.9.4/assets/modify_advanced.png
+-rw-r--r--   0        0        0   180588 2020-02-02 00:00:00.000000 bigtree-0.9.4/assets/modify_shift_and_copy.png
+-rw-r--r--   0        0        0    67777 2020-02-02 00:00:00.000000 bigtree-0.9.4/assets/tree_construct.png
+-rw-r--r--   0        0        0    11482 2020-02-02 00:00:00.000000 bigtree-0.9.4/assets/weighted_tree.png
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/py.typed
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/binarytree/construct.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/dag/__init__.py
+-rw-r--r--   0        0        0     7410 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/dag/construct.py
+-rw-r--r--   0        0        0    10007 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/dag/export.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/node/__init__.py
+-rw-r--r--   0        0        0    21937 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/node/basenode.py
+-rw-r--r--   0        0        0    13630 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/node/binarynode.py
+-rw-r--r--   0        0        0    18188 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/node/dagnode.py
+-rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/node/node.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/tree/__init__.py
+-rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/tree/construct.py
+-rw-r--r--   0        0        0    30268 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/tree/export.py
+-rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/tree/helper.py
+-rw-r--r--   0        0        0    33168 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/tree/modify.py
+-rw-r--r--   0        0        0    12597 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/tree/search.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/utils/__init__.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/utils/exceptions.py
+-rw-r--r--   0        0        0    13884 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/utils/iterators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/workflows/__init__.py
+-rw-r--r--   0        0        0     6533 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/workflows/app_calendar.py
+-rw-r--r--   0        0        0     8516 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/workflows/app_todo.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/make.bat
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/requirements.txt
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/binarytree.rst
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/conf.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/dag.rst
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/index.rst
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/node.rst
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/others.rst
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/tree.rst
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/utils.rst
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/workflows.rst
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/_static/custom.css
+-rw-r--r--   0        0        0    27138 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/_static/favicon.ico
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/_templates/layout.html
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/bigtree/binarytree/construct.rst
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/bigtree/dag/construct.rst
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/bigtree/dag/export.rst
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/bigtree/node/basenode.rst
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/bigtree/node/binarynode.rst
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/bigtree/node/dagnode.rst
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/bigtree/node/node.rst
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/bigtree/tree/construct.rst
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/bigtree/tree/export.rst
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/bigtree/tree/helper.rst
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/bigtree/tree/modify.rst
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/bigtree/tree/search.rst
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/bigtree/utils/iterators.rst
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/bigtree/workflows/app_calendar.rst
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/bigtree/workflows/app_todo.rst
+-rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/others/contributing.rst
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/others/list_dir.md
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/others/merging_trees.md
+-rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/others/nodes.md
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/others/tips.rst
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/others/weighted_trees.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/__init__.py
+-rw-r--r--   0        0        0     9434 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/conftest.py
+-rw-r--r--   0        0        0     6308 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/constants.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/binarytree/__init__.py
+-rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/binarytree/test_construct.py
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/binarytree/test_export.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/binarytree/test_helper.py
+-rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/binarytree/test_search.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/dag/__init__.py
+-rw-r--r--   0        0        0     8922 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/dag/test_construct.py
+-rw-r--r--   0        0        0    15751 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/dag/test_export.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/node/__init__.py
+-rw-r--r--   0        0        0    32428 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/node/test_basenode.py
+-rw-r--r--   0        0        0    36915 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/node/test_binarynode.py
+-rw-r--r--   0        0        0    32596 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/node/test_dagnode.py
+-rw-r--r--   0        0        0    14179 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/node/test_node.py
+-rw-r--r--   0        0        0    66656 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/tree/test_construct.py
+-rw-r--r--   0        0        0    37681 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/tree/test_export.py
+-rw-r--r--   0        0        0     5089 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/tree/test_helper.py
+-rw-r--r--   0        0        0    67494 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/tree/test_modify.py
+-rw-r--r--   0        0        0    18425 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/tree/test_search.py
+-rw-r--r--   0        0        0    13544 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/utils/test_iterators.py
+-rw-r--r--   0        0        0    18086 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/workflows/test_todo.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 bigtree-0.9.4/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 bigtree-0.9.4/LICENSE
+-rw-r--r--   0        0        0    25288 2020-02-02 00:00:00.000000 bigtree-0.9.4/README.md
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 bigtree-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0    26396 2020-02-02 00:00:00.000000 bigtree-0.9.4/PKG-INFO
```

### Comparing `bigtree-0.9.3/.pre-commit-config.yaml` & `bigtree-0.9.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/CHANGELOG.md` & `bigtree-0.9.4/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,30 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.9.4] - 2023-06-18
+### Added
+- Tree Constructor: `list_to_tree_by_relation` and `dataframe_to_tree_by_relation` method to allow duplicate intermediate nodes (default is false).
+- DAG Exporter: Added `node_shape` parameter in `dag_to_dot` export function for easier way to customize node shape.
+- Misc: More test cases.
+- Misc: Added security instructions on how to raise vulnerabilities.
+- Misc: Added Calendar workflow to documentation.
+### Changed
+- Tree Constructor: `add_dict_to_tree_by_name` method rename argument from `path_attrs` to `name_attrs`.
+- Misc: Modified contributing instructions.
+### Fixed
+- Tree Exporter: `tree_to_dot` to handle cases when not all nodes have `edge_attr`.
+- DAG Exporter: `dag_to_dot` to perform dictionary copy to prevent style from being overridden for child nodes.
+- Tree Constructor: `dataframe_to_tree` to handle case when path column is not the first column.
+
 ## [0.9.3] - 2023-05-28
-### Modified
+### Changed
 - Tree Constructor: Relax type hint to `Iterable` instead of `List` for `list_to_tree` and `list_to_tree_by_relation` methods.
 ### Fixed
 - Node: Fix error message when trees have different `sep`.
 
 ## [0.9.2] - 2023-04-09
 ### Added
 - Node: Added `show` method to print tree to console.
@@ -33,15 +48,15 @@
 ## [0.8.4] - 2023-03-24
 ### Added
 - Tree Search: Implement `find_child` and `find_children` to find single child or multiple children based on user-defined condition.
 ### Changed
 - Tree and DAG Constructor: Reduce reliance on `numpy` package, only reject `None` attributes when creating tree from DataFrame (previously it rejects `[None]`).
 - Tree Helper: Get difference between two trees reduce reliance on `numpy` package, enhance test cases.
 - Tree Search: Renamed `find_children` to `find_child_by_name` for clarity.
-- Misc: Fix README for Windows installation
+- Misc: Fix README for Windows installation.
 
 ## [0.8.3] - 2023-03-16
 ### Changed
 - Workflow: Misc refactor and update log statements.
 - Misc: Fix coverage report.
 
 ## [0.8.2] - 2023-03-16
@@ -138,15 +153,15 @@
 - BaseNode and DAGNode: Type hints.
 - BNode: Node class for Binary Tree.
 - BTree Constructor: From list.
 - BNode Iterator: Level-Order Iterator.
 - Misc: Add Tips and Tricks to documentation (List Directory).
 
 ### Fixed
-- DAGNode: Fix issue of duplicated parent constructor creating duplicated children.
+- DAGNode: Fix issue of duplicate parent constructor creating duplicate children.
 
 ## [0.5.5] - 2022-11-12
 ### Added
 - Misc: More docstring examples.
 - Misc: More test cases.
 
 ### Fixed
@@ -156,15 +171,15 @@
 ### Added
 - BaseNode: Add sort() to sort children.
 - Node: Made more extendable with pre-/post-assign checks.
 - Misc: Add Tips and Tricks to documentation (Extending Nodes).
 - Misc: More test cases.
 
 ### Fixed
-- Tree Search: Type hints
+- Tree Search: Type hints.
 
 ## [0.5.3] - 2022-11-11
 ### Added
 - DAG and Tree Exporter: More customizations allowed on edges.
 - Add Tips and Tricks to documentation (Weighted Trees, Merging Trees).
 
 ### Fixed
@@ -180,44 +195,44 @@
 
 ## [0.5.0] - 2022-11-09
 ### Added
 - Misc: Clean codes and documentation.
 
 ### Changed
 - Tree Exporter: Printing tree to group multiple arguments together.
-- DAG and Tree Exporter: Export to dot able to plot multiple disjointed trees/dags, rename `bgcolor` to `bg_colour`
+- DAG and Tree Exporter: Export to dot able to plot multiple disjointed trees/dags, rename `bgcolor` to `bg_colour`.
 
 ## [0.4.6] - 2022-11-09
 ### Added
 - Tree Constructor: From DataFrame of parent-child columns.
 
 ### Changed
 - Tree Exporter: Printing tree to define node name or path, and default to const style.
-- Tree Constructor: Rename `list_to_tree_tuples` to `list_to_tree_by_relation`
-- Tree Constructor: Remove parameter `sep` for `nested_dict_to_tree`
+- Tree Constructor: Rename `list_to_tree_tuples` to `list_to_tree_by_relation`.
+- Tree Constructor: Remove parameter `sep` for `nested_dict_to_tree`.
 
 ## [0.4.5] - 2022-11-08
 ### Changed
 - Tree Exporter: Printing tree with added ability to omit null attributes.
 
 ## [0.4.4] - 2022-11-08
 ### Fixed
-- Tree Constructor: Handle adding attributes that are array-like - add array even when one of the items is null
+- Tree Constructor: Handle adding attributes that are array-like - add array even when one of the items is null.
 
 ## [0.4.3] - 2022-11-08
 ### Added
 - Node: Print format for BaseNode.
 
 ## [0.4.2] - 2022-11-08
 ### Fixed
-- Tree Constructor: For list of tuples, handle cases where parent name is None
+- Tree Constructor: For list of tuples, handle cases where parent name is None.
 
 ## [0.4.1] - 2022-11-07
 ### Fixed
-- Tree Constructor: Handle adding attributes that are array-like - error in drop_duplicate() and pd.isnull()
+- Tree Constructor: Handle adding attributes that are array-like - error in drop_duplicate() and pd.isnull().
 
 ## [0.4.0] - 2022-11-07
 ### Added
 - Tree Constructor: From list of tuples of parent-child.
 
 ## [0.3.3] - 2022-11-07
 ### Added
@@ -258,51 +273,52 @@
 - Tree Exporter: To list, nested dictionary, pandas DataFrame.
 - Tree Helper: Cloning, pruning trees, get difference between two trees.
 - Tree Modifier: Shift and copy nodes within tree and between trees.
 - Tree Search: Find single or multiple nodes based on name, attribute, or custom criteria.
 - Utility Iterator: Tree traversal methods.
 - Workflow To Do App: Tree use case with to-do list implementation.
 
-[0.9.3]: https://github.com/kayjan/bigtree/compare/v0.9.2...v0.9.3
-[0.9.2]: https://github.com/kayjan/bigtree/compare/v0.9.1...v0.9.2
-[0.9.1]: https://github.com/kayjan/bigtree/compare/v0.9.0...v0.9.1
-[0.9.0]: https://github.com/kayjan/bigtree/compare/v0.8.4...v0.9.0
-[0.8.4]: https://github.com/kayjan/bigtree/compare/v0.8.3...v0.8.4
-[0.8.3]: https://github.com/kayjan/bigtree/compare/v0.8.2...v0.8.3
-[0.8.2]: https://github.com/kayjan/bigtree/compare/v0.8.1...v0.8.2
-[0.8.1]: https://github.com/kayjan/bigtree/compare/v0.8.0...v0.8.1
-[0.8.0]: https://github.com/kayjan/bigtree/compare/v0.7.4...v0.8.0
-[0.7.4]: https://github.com/kayjan/bigtree/compare/v0.7.3...v0.7.4
-[0.7.3]: https://github.com/kayjan/bigtree/compare/v0.7.2...v0.7.3
-[0.7.2]: https://github.com/kayjan/bigtree/compare/v0.7.1...v0.7.2
-[0.7.1]: https://github.com/kayjan/bigtree/compare/v0.7.0...v0.7.1
-[0.7.0]: https://github.com/kayjan/bigtree/compare/v0.6.10...v0.7.0
-[0.6.10]: https://github.com/kayjan/bigtree/compare/v0.6.9...v0.6.10
-[0.6.9]: https://github.com/kayjan/bigtree/compare/v0.6.8...v0.6.9
-[0.6.8]: https://github.com/kayjan/bigtree/compare/v0.6.7...v0.6.8
-[0.6.7]: https://github.com/kayjan/bigtree/compare/v0.6.6...v0.6.7
-[0.6.6]: https://github.com/kayjan/bigtree/compare/v0.6.5...v0.6.6
-[0.6.5]: https://github.com/kayjan/bigtree/compare/v0.6.4...v0.6.5
-[0.6.4]: https://github.com/kayjan/bigtree/compare/v0.6.3...v0.6.4
-[0.6.3]: https://github.com/kayjan/bigtree/compare/v0.6.2...v0.6.3
-[0.6.2]: https://github.com/kayjan/bigtree/compare/v0.6.1...v0.6.2
-[0.6.1]: https://github.com/kayjan/bigtree/compare/v0.6.0...v0.6.1
-[0.6.0]: https://github.com/kayjan/bigtree/compare/v0.5.5...v0.6.0
-[0.5.5]: https://github.com/kayjan/bigtree/compare/v0.5.4...v0.5.5
-[0.5.4]: https://github.com/kayjan/bigtree/compare/v0.5.3...v0.5.4
-[0.5.3]: https://github.com/kayjan/bigtree/compare/v0.5.2...v0.5.3
-[0.5.2]: https://github.com/kayjan/bigtree/compare/v0.5.1...v0.5.2
-[0.5.1]: https://github.com/kayjan/bigtree/compare/v0.5.0...v0.5.1
-[0.5.0]: https://github.com/kayjan/bigtree/compare/v0.4.6...v0.5.0
-[0.4.6]: https://github.com/kayjan/bigtree/compare/v0.4.5...v0.4.6
-[0.4.5]: https://github.com/kayjan/bigtree/compare/v0.4.4...v0.4.5
-[0.4.4]: https://github.com/kayjan/bigtree/compare/v0.4.3...v0.4.4
-[0.4.3]: https://github.com/kayjan/bigtree/compare/v0.4.2...v0.4.3
-[0.4.2]: https://github.com/kayjan/bigtree/compare/v0.4.1...v0.4.2
-[0.4.1]: https://github.com/kayjan/bigtree/compare/v0.4.0...v0.4.1
-[0.4.0]: https://github.com/kayjan/bigtree/compare/v0.3.3...v0.4.0
-[0.3.3]: https://github.com/kayjan/bigtree/compare/v0.3.2...v0.3.3
-[0.3.2]: https://github.com/kayjan/bigtree/compare/v0.3.1...v0.3.2
-[0.3.1]: https://github.com/kayjan/bigtree/compare/v0.3.0...v0.3.1
-[0.3.0]: https://github.com/kayjan/bigtree/compare/v0.2.0...v0.3.0
-[0.2.0]: https://github.com/kayjan/bigtree/compare/v0.1.0...v0.2.0
-[0.1.0]: https://github.com/kayjan/bigtree/releases/tag/v0.1.0
+[0.9.4]: https://github.com/kayjan/bigtree/compare/0.9.3...0.9.4
+[0.9.3]: https://github.com/kayjan/bigtree/compare/0.9.2...0.9.3
+[0.9.2]: https://github.com/kayjan/bigtree/compare/0.9.1...0.9.2
+[0.9.1]: https://github.com/kayjan/bigtree/compare/0.9.0...0.9.1
+[0.9.0]: https://github.com/kayjan/bigtree/compare/0.8.4...0.9.0
+[0.8.4]: https://github.com/kayjan/bigtree/compare/0.8.3...0.8.4
+[0.8.3]: https://github.com/kayjan/bigtree/compare/0.8.2...0.8.3
+[0.8.2]: https://github.com/kayjan/bigtree/compare/0.8.1...0.8.2
+[0.8.1]: https://github.com/kayjan/bigtree/compare/0.8.0...0.8.1
+[0.8.0]: https://github.com/kayjan/bigtree/compare/0.7.4...0.8.0
+[0.7.4]: https://github.com/kayjan/bigtree/compare/0.7.3...0.7.4
+[0.7.3]: https://github.com/kayjan/bigtree/compare/0.7.2...0.7.3
+[0.7.2]: https://github.com/kayjan/bigtree/compare/0.7.1...0.7.2
+[0.7.1]: https://github.com/kayjan/bigtree/compare/0.7.0...0.7.1
+[0.7.0]: https://github.com/kayjan/bigtree/compare/0.6.10...0.7.0
+[0.6.10]: https://github.com/kayjan/bigtree/compare/0.6.9...0.6.10
+[0.6.9]: https://github.com/kayjan/bigtree/compare/0.6.8...0.6.9
+[0.6.8]: https://github.com/kayjan/bigtree/compare/0.6.7...0.6.8
+[0.6.7]: https://github.com/kayjan/bigtree/compare/0.6.6...0.6.7
+[0.6.6]: https://github.com/kayjan/bigtree/compare/0.6.5...0.6.6
+[0.6.5]: https://github.com/kayjan/bigtree/compare/0.6.4...0.6.5
+[0.6.4]: https://github.com/kayjan/bigtree/compare/0.6.3...0.6.4
+[0.6.3]: https://github.com/kayjan/bigtree/compare/0.6.2...0.6.3
+[0.6.2]: https://github.com/kayjan/bigtree/compare/0.6.1...0.6.2
+[0.6.1]: https://github.com/kayjan/bigtree/compare/0.6.0...0.6.1
+[0.6.0]: https://github.com/kayjan/bigtree/compare/0.5.5...0.6.0
+[0.5.5]: https://github.com/kayjan/bigtree/compare/0.5.4...0.5.5
+[0.5.4]: https://github.com/kayjan/bigtree/compare/0.5.3...0.5.4
+[0.5.3]: https://github.com/kayjan/bigtree/compare/0.5.2...0.5.3
+[0.5.2]: https://github.com/kayjan/bigtree/compare/0.5.1...0.5.2
+[0.5.1]: https://github.com/kayjan/bigtree/compare/0.5.0...0.5.1
+[0.5.0]: https://github.com/kayjan/bigtree/compare/0.4.6...0.5.0
+[0.4.6]: https://github.com/kayjan/bigtree/compare/0.4.5...0.4.6
+[0.4.5]: https://github.com/kayjan/bigtree/compare/0.4.4...0.4.5
+[0.4.4]: https://github.com/kayjan/bigtree/compare/0.4.3...0.4.4
+[0.4.3]: https://github.com/kayjan/bigtree/compare/0.4.2...0.4.3
+[0.4.2]: https://github.com/kayjan/bigtree/compare/0.4.1...0.4.2
+[0.4.1]: https://github.com/kayjan/bigtree/compare/0.4.0...0.4.1
+[0.4.0]: https://github.com/kayjan/bigtree/compare/0.3.3...0.4.0
+[0.3.3]: https://github.com/kayjan/bigtree/compare/0.3.2...0.3.3
+[0.3.2]: https://github.com/kayjan/bigtree/compare/0.3.1...0.3.2
+[0.3.1]: https://github.com/kayjan/bigtree/compare/0.3.0...0.3.1
+[0.3.0]: https://github.com/kayjan/bigtree/compare/0.2.0...0.3.0
+[0.2.0]: https://github.com/kayjan/bigtree/compare/0.1.0...0.2.0
+[0.1.0]: https://github.com/kayjan/bigtree/releases/tag/0.1.0
```

### Comparing `bigtree-0.9.3/SECURITY.md` & `bigtree-0.9.4/SECURITY.md`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/.github/workflows/codecov.yml` & `bigtree-0.9.4/.github/workflows/codecov.yml`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/.github/workflows/docs.yml` & `bigtree-0.9.4/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/.github/workflows/pytest.yml` & `bigtree-0.9.4/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/.github/workflows/python-publish.yml` & `bigtree-0.9.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/assets/DejaVuSans.ttf` & `bigtree-0.9.4/assets/DejaVuSans.ttf`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/assets/binarytree.png` & `bigtree-0.9.4/assets/binarytree.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/assets/custom_tree.png` & `bigtree-0.9.4/assets/custom_tree.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/assets/dag_construct.png` & `bigtree-0.9.4/assets/dag_construct.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/assets/demo.png` & `bigtree-0.9.4/assets/demo.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/assets/demo_binarytree.png` & `bigtree-0.9.4/assets/demo_binarytree.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/assets/demo_dag.png` & `bigtree-0.9.4/assets/demo_dag.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/assets/demo_pillow.png` & `bigtree-0.9.4/assets/demo_pillow.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/assets/demo_tree.png` & `bigtree-0.9.4/assets/demo_tree.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/assets/modify_advanced.png` & `bigtree-0.9.4/assets/modify_advanced.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/assets/modify_shift_and_copy.png` & `bigtree-0.9.4/assets/modify_shift_and_copy.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/assets/tree_construct.png` & `bigtree-0.9.4/assets/tree_construct.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/assets/weighted_tree.png` & `bigtree-0.9.4/assets/weighted_tree.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/bigtree/__init__.py` & `bigtree-0.9.4/bigtree/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.9.3"
+__version__ = "0.9.4"
 
 from bigtree.binarytree.construct import list_to_binarytree
 from bigtree.dag.construct import dataframe_to_dag, dict_to_dag, list_to_dag
 from bigtree.dag.export import dag_to_dataframe, dag_to_dict, dag_to_dot, dag_to_list
 from bigtree.node.basenode import BaseNode
 from bigtree.node.binarynode import BinaryNode
 from bigtree.node.dagnode import DAGNode
```

### Comparing `bigtree-0.9.3/bigtree/binarytree/construct.py` & `bigtree-0.9.4/bigtree/binarytree/construct.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/bigtree/dag/construct.py` & `bigtree-0.9.4/bigtree/dag/construct.py`

 * *Files 10% similar despite different names*

```diff
@@ -67,17 +67,18 @@
         (DAGNode)
     """
     if not len(relation_attrs):
         raise ValueError("Dictionary does not contain any data, check `relation_attrs`")
 
     # Convert dictionary to dataframe
     data = pd.DataFrame(relation_attrs).T.rename_axis("_tmp_child").reset_index()
-    assert (
-        parent_key in data
-    ), f"Parent key {parent_key} not in dictionary, check `relation_attrs` and `parent_key`"
+    if parent_key not in data:
+        raise ValueError(
+            f"Parent key {parent_key} not in dictionary, check `relation_attrs` and `parent_key`"
+        )
 
     data = data.explode(parent_key)
     return dataframe_to_dag(
         data,
         child_col="_tmp_child",
         parent_col=parent_key,
         node_type=node_type,
@@ -134,36 +135,47 @@
     if not len(data.columns):
         raise ValueError("Data does not contain any columns, check `data`")
     if not len(data):
         raise ValueError("Data does not contain any rows, check `data`")
 
     if not child_col:
         child_col = data.columns[0]
+    elif child_col not in data.columns:
+        raise ValueError("Child column not in data, check `child_col`")
     if not parent_col:
         parent_col = data.columns[1]
+    elif parent_col not in data.columns:
+        raise ValueError("Parent column not in data, check `parent_col`")
     if not len(attribute_cols):
         attribute_cols = list(data.columns)
         attribute_cols.remove(child_col)
         attribute_cols.remove(parent_col)
+    elif any([col not in data.columns for col in attribute_cols]):
+        raise ValueError(
+            "One or more attribute column(s) not in data, check `attribute_col`"
+        )
 
-    data_check = data.copy()[[child_col] + attribute_cols].drop_duplicates()
+    data_check = data.copy()[[child_col, parent_col] + attribute_cols].drop_duplicates(
+        subset=[child_col] + attribute_cols
+    )
     _duplicate_check = (
         data_check[child_col]
         .value_counts()
         .to_frame("counts")
         .rename_axis(child_col)
         .reset_index()
     )
     _duplicate_check = _duplicate_check[_duplicate_check["counts"] > 1]
     if len(_duplicate_check):
         raise ValueError(
-            f"There exists duplicate child name with different attributes\nCheck {_duplicate_check}"
+            f"There exists duplicate child name with different attributes\n"
+            f"Check {_duplicate_check}"
         )
     if sum(data[child_col].isnull()):
-        raise ValueError(f"Child name cannot be empty, check {child_col}")
+        raise ValueError(f"Child name cannot be empty, check column: {child_col}")
 
     node_dict: Dict[str, DAGNode] = dict()
     parent_node = DAGNode()
 
     for row in data.reset_index(drop=True).to_dict(orient="index").values():
         child_name = row[child_col]
         parent_name = row[parent_col]
```

### Comparing `bigtree-0.9.3/bigtree/dag/export.py` & `bigtree-0.9.4/bigtree/dag/export.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,14 +161,15 @@
 
 
 def dag_to_dot(  # type: ignore[no-untyped-def]
     dag: Union[DAGNode, List[DAGNode]],
     rankdir: str = "TB",
     bg_colour: str = "",
     node_colour: str = "",
+    node_shape: str = "",
     edge_colour: str = "",
     node_attr: str = "",
     edge_attr: str = "",
 ):
     r"""Export DAG tree or list of DAG trees to image.
     Note that node names must be unique.
     Posible node attributes include style, fillcolor, shape.
@@ -192,14 +193,16 @@
     'strict digraph G {\nrankdir=TB;\nc [label=c];\na [label=a];\na -> c;\nd [label=d];\na [label=a];\na -> d;\nc [label=c];\nb [label=b];\nb -> c;\nd [label=d];\nc [label=c];\nc -> d;\ne [label=e];\nd [label=d];\nd -> e;\n}\n'
 
     Args:
         dag (Union[DAGNode, List[DAGNode]]): DAG or list of DAGs to be exported
         rankdir (str): set direction of graph layout, defaults to 'TB', can be 'BT, 'LR', 'RL'
         bg_colour (str): background color of image, defaults to ''
         node_colour (str): fill colour of nodes, defaults to ''
+        node_shape (str): shape of nodes, defaults to None
+            Possible node_shape include "circle", "square", "diamond", "triangle"
         edge_colour (str): colour of edges, defaults to ''
         node_attr (str): node attribute for style, overrides node_colour, defaults to ''
             Possible node attributes include {"style": "filled", "fillcolor": "gold"}
         edge_attr (str): edge attribute for style, overrides edge_colour, defaults to ''
             Possible edge attributes include {"style": "bold", "label": "edge label", "color": "black"}
 
     Returns:
@@ -219,14 +222,17 @@
         graph_style = dict()
 
     if node_colour:
         node_style = dict(style="filled", fillcolor=node_colour)
     else:
         node_style = dict()
 
+    if node_shape:
+        node_style["shape"] = node_shape
+
     if edge_colour:
         edge_style = dict(color=edge_colour)
     else:
         edge_style = dict()
 
     _graph = pydot.Dot(
         graph_type="digraph", strict=True, rankdir=rankdir, **graph_style
@@ -239,31 +245,31 @@
         if not isinstance(_dag, DAGNode):
             raise ValueError(
                 "Tree should be of type `DAGNode`, or inherit from `DAGNode`"
             )
         _dag = _dag.copy()
 
         for parent_node, child_node in dag_iterator(_dag):
+            _node_style = node_style.copy()
+            _edge_style = edge_style.copy()
+
             child_name = child_node.name
-            child_node_style = node_style.copy()
             if node_attr and child_node.get_attr(node_attr):
-                child_node_style.update(child_node.get_attr(node_attr))
-            if edge_attr:
-                edge_style.update(child_node.get_attr(edge_attr))
-            pydot_child = pydot.Node(
-                name=child_name, label=child_name, **child_node_style
-            )
+                _node_style.update(child_node.get_attr(node_attr))
+            if edge_attr and child_node.get_attr(edge_attr):
+                _edge_style.update(child_node.get_attr(edge_attr))
+            pydot_child = pydot.Node(name=child_name, label=child_name, **_node_style)
             _graph.add_node(pydot_child)
 
             parent_name = parent_node.name
             parent_node_style = node_style.copy()
             if node_attr and parent_node.get_attr(node_attr):
                 parent_node_style.update(parent_node.get_attr(node_attr))
             pydot_parent = pydot.Node(
                 name=parent_name, label=parent_name, **parent_node_style
             )
             _graph.add_node(pydot_parent)
 
-            edge = pydot.Edge(parent_name, child_name, **edge_style)
+            edge = pydot.Edge(parent_name, child_name, **_edge_style)
             _graph.add_edge(edge)
 
     return _graph
```

### Comparing `bigtree-0.9.3/bigtree/node/basenode.py` & `bigtree-0.9.4/bigtree/node/basenode.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,15 +276,15 @@
                 )
 
             # Check for loop and tree structure
             if new_child is self:
                 raise LoopError("Error setting child: Node cannot be child of itself")
             if any(child is new_child for child in self.ancestors):
                 raise LoopError(
-                    "Error setting child: Node cannot be ancestors of itself"
+                    "Error setting child: Node cannot be ancestor of itself"
                 )
 
             # Check for duplicate children
             if id(new_child) in seen_children:
                 raise TreeError(
                     "Error setting child: Node cannot be added multiple times as a child"
                 )
```

### Comparing `bigtree-0.9.3/bigtree/node/binarynode.py` & `bigtree-0.9.4/bigtree/node/binarynode.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,15 +256,15 @@
                 )
 
             # Check for loop and tree structure
             if new_child is self:
                 raise LoopError("Error setting child: Node cannot be child of itself")
             if any(child is new_child for child in self.ancestors):
                 raise LoopError(
-                    "Error setting child: Node cannot be ancestors of itself"
+                    "Error setting child: Node cannot be ancestor of itself"
                 )
 
             # Check for duplicate children
             if new_child is not None:
                 if id(new_child) in seen_children:
                     raise TreeError(
                         "Error setting child: Node cannot be added multiple times as a child"
```

### Comparing `bigtree-0.9.3/bigtree/node/dagnode.py` & `bigtree-0.9.4/bigtree/node/dagnode.py`

 * *Files 0% similar despite different names*

```diff
@@ -266,15 +266,15 @@
                 )
 
             # Check for loop and tree structure
             if new_child is self:
                 raise LoopError("Error setting child: Node cannot be child of itself")
             if any(child is new_child for child in self.ancestors):
                 raise LoopError(
-                    "Error setting child: Node cannot be ancestors of itself"
+                    "Error setting child: Node cannot be ancestor of itself"
                 )
 
             # Check for duplicate children
             if id(new_child) in seen_children:
                 raise TreeError(
                     "Error setting child: Node cannot be added multiple times as a child"
                 )
```

### Comparing `bigtree-0.9.3/bigtree/node/node.py` & `bigtree-0.9.4/bigtree/node/node.py`

 * *Files 6% similar despite different names*

```diff
@@ -163,15 +163,15 @@
         self.__pre_assign_parent(new_parent)
         if new_parent is not None:
             if any(
                 child.node_name == self.node_name and child is not self
                 for child in new_parent.children
             ):
                 raise TreeError(
-                    f"Error: Duplicate node with same path\n"
+                    f"Duplicate node with same path\n"
                     f"There exist a node with same path {new_parent.path_name}{new_parent.sep}{self.node_name}"
                 )
 
     def _BaseNode__post_assign_parent(self: T, new_parent: T) -> None:
         """No rules
 
         Args:
@@ -183,24 +183,24 @@
         """Do not allow duplicate nodes of same path
 
         Args:
             new_children (List[Self]): new children to be added
         """
         self.__pre_assign_children(new_children)
         children_names = [node.node_name for node in new_children]
-        duplicated_names = [
+        duplicate_names = [
             item[0] for item in Counter(children_names).items() if item[1] > 1
         ]
-        if len(duplicated_names):
-            duplicated_names_str = " and ".join(
-                [f"{self.path_name}{self.sep}{name}" for name in duplicated_names]
+        if len(duplicate_names):
+            duplicate_names_str = " and ".join(
+                [f"{self.path_name}{self.sep}{name}" for name in duplicate_names]
             )
             raise TreeError(
-                f"Error: Duplicate node with same path\n"
-                f"Attempting to add nodes same path {duplicated_names_str}"
+                f"Duplicate node with same path\n"
+                f"Attempting to add nodes same path {duplicate_names_str}"
             )
 
     def _BaseNode__post_assign_children(self: T, new_children: List[T]) -> None:
         """No rules
 
         Args:
             new_children (List[Self]): new children to be added
```

### Comparing `bigtree-0.9.3/bigtree/tree/construct.py` & `bigtree-0.9.4/bigtree/tree/construct.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,30 +54,30 @@
     └── b
         └── c
 
     Args:
         tree (Node): existing tree
         path (str): path to be added to tree
         sep (str): path separator for input `path`
-        duplicate_name_allowed (bool): indicator if nodes with duplicated `Node` name is allowed, defaults to True
+        duplicate_name_allowed (bool): indicator if nodes with duplicate `Node` name is allowed, defaults to True
         node_attrs (Dict[str, Any]): attributes to add to node, key: attribute name, value: attribute value, optional
 
     Returns:
         (Node)
     """
     if not len(path):
         raise ValueError("Path is empty, check `path`")
 
     tree_root = tree.root
     tree_sep = tree_root.sep
     node_type = tree_root.__class__
     branch = path.lstrip(sep).rstrip(sep).split(sep)
     if branch[0] != tree_root.node_name:
         raise TreeError(
-            f"Error: Path does not have same root node, expected {tree_root.node_name}, received {branch[0]}\n"
+            f"Path does not have same root node, expected {tree_root.node_name}, received {branch[0]}\n"
             f"Check your input paths or verify that path separator `sep` is set correctly"
         )
 
     # Grow tree
     node = tree_root
     parent_node = tree_root
     for idx in range(1, len(branch)):
@@ -143,15 +143,15 @@
         └── f
 
     Args:
         tree (Node): existing tree
         path_attrs (Dict[str, Dict[str, Any]]): dictionary containing node path and attribute information,
             key: node path, value: dict of node attribute name and attribute value
         sep (str): path separator for input `path_attrs`
-        duplicate_name_allowed (bool): indicator if nodes with duplicated `Node` name is allowed, defaults to True
+        duplicate_name_allowed (bool): indicator if nodes with duplicate `Node` name is allowed, defaults to True
 
     Returns:
         (Node)
     """
     if not len(path_attrs):
         raise ValueError("Dictionary does not contain any data, check `path_attrs`")
 
@@ -165,15 +165,15 @@
             duplicate_name_allowed=duplicate_name_allowed,
             node_attrs=v,
         )
     return tree_root
 
 
 def add_dict_to_tree_by_name(
-    tree: Node, path_attrs: Dict[str, Dict[str, Any]], join_type: str = "left"
+    tree: Node, name_attrs: Dict[str, Dict[str, Any]], join_type: str = "left"
 ) -> Node:
     """Add attributes to tree, return *new* root of tree.
     Adds to existing tree from nested dictionary, ``key``: name, ``value``: dict of attribute name and attribute value.
 
     Function can return all existing tree nodes or only tree nodes that are in the input dictionary keys.
     Input dictionary keys that are not existing node names will be ignored.
     Note that if multiple nodes have the same name, attributes will be added to all nodes sharing same name.
@@ -188,30 +188,30 @@
     >>> root = add_dict_to_tree_by_name(root, name_dict)
     >>> print_tree(root, attr_list=["age"])
     a [age=90]
     └── b [age=65]
 
     Args:
         tree (Node): existing tree
-        path_attrs (Dict[str, Dict[str, Any]]): dictionary containing node name and attribute information,
+        name_attrs (Dict[str, Dict[str, Any]]): dictionary containing node name and attribute information,
             key: node name, value: dict of node attribute name and attribute value
         join_type (str): join type with attribute, default of 'left' takes existing tree nodes,
             if join_type is set to 'inner' it will only take tree nodes that are in `path_attrs` key and drop others
 
     Returns:
         (Node)
     """
     if join_type not in ["inner", "left"]:
         raise ValueError("`join_type` must be one of 'inner' or 'left'")
 
-    if not len(path_attrs):
-        raise ValueError("Dictionary does not contain any data, check `path_attrs`")
+    if not len(name_attrs):
+        raise ValueError("Dictionary does not contain any data, check `name_attrs`")
 
     # Convert dictionary to dataframe
-    data = pd.DataFrame(path_attrs).T.rename_axis("NAME").reset_index()
+    data = pd.DataFrame(name_attrs).T.rename_axis("NAME").reset_index()
     return add_dataframe_to_tree_by_name(tree, data=data, join_type=join_type)
 
 
 def add_dataframe_to_tree_by_path(
     tree: Node,
     data: pd.DataFrame,
     path_col: str = "",
@@ -264,15 +264,15 @@
         tree (Node): existing tree
         data (pd.DataFrame): data containing node path and attribute information
         path_col (str): column of data containing `path_name` information,
             if not set, it will take the first column of data
         attribute_cols (List[str]): columns of data containing node attribute information,
             if not set, it will take all columns of data except `path_col`
         sep (str): path separator for input `path_col`
-        duplicate_name_allowed (bool): indicator if nodes with duplicated `Node` name is allowed, defaults to True
+        duplicate_name_allowed (bool): indicator if nodes with duplicate `Node` name is allowed, defaults to True
 
     Returns:
         (Node)
     """
     data = data.copy()
 
     if not len(data.columns):
@@ -508,15 +508,15 @@
     │       └── h
     └── c
         └── f
 
     Args:
         paths (Iterable[str]): list containing path strings
         sep (str): path separator for input `paths` and created tree, defaults to `/`
-        duplicate_name_allowed (bool): indicator if nodes with duplicated `Node` name is allowed, defaults to True
+        duplicate_name_allowed (bool): indicator if nodes with duplicate `Node` name is allowed, defaults to True
         node_type (Type[Node]): node type of tree to be created, defaults to Node
 
     Returns:
         (Node)
     """
     if not paths:
         raise ValueError("Path list does not contain any data, check `paths`")
@@ -535,20 +535,22 @@
         )
     root_node.sep = sep
     return root_node
 
 
 def list_to_tree_by_relation(
     relations: Iterable[Tuple[str, str]],
+    allow_duplicates: bool = False,
     node_type: Type[Node] = Node,
 ) -> Node:
     """Construct tree from list of tuple containing parent-child names.
 
-    Note that node names must be unique since tree is created from parent-child names,
-    except for leaf nodes - names of leaf nodes may be repeated as there is no confusion.
+    Since tree is created from parent-child names, only names of leaf nodes may be repeated.
+    Error will be thrown if names of intermediate nodes are repeated as there will be confusion.
+    This error can be ignored by setting `allow_duplicates` to be True.
 
     >>> from bigtree import list_to_tree_by_relation, print_tree
     >>> relations_list = [("a", "b"), ("a", "c"), ("b", "d"), ("b", "e"), ("c", "f"), ("e", "g"), ("e", "h")]
     >>> root = list_to_tree_by_relation(relations_list)
     >>> print_tree(root)
     a
     ├── b
@@ -557,25 +559,31 @@
     │       ├── g
     │       └── h
     └── c
         └── f
 
     Args:
         relations (Iterable[Tuple[str, str]]): list containing tuple containing parent-child names
+        allow_duplicates (bool): allow duplicate intermediate nodes such that child node will
+            be tagged to multiple parent nodes, defaults to False
         node_type (Type[Node]): node type of tree to be created, defaults to Node
 
     Returns:
         (Node)
     """
     if not relations:
         raise ValueError("Path list does not contain any data, check `relations`")
 
     relation_data = pd.DataFrame(relations, columns=["parent", "child"])
     return dataframe_to_tree_by_relation(
-        relation_data, child_col="child", parent_col="parent", node_type=node_type
+        relation_data,
+        child_col="child",
+        parent_col="parent",
+        allow_duplicates=allow_duplicates,
+        node_type=node_type,
     )
 
 
 def dict_to_tree(
     path_attrs: Dict[str, Any],
     sep: str = "/",
     duplicate_name_allowed: bool = True,
@@ -615,15 +623,15 @@
     └── c [age=60]
         └── f [age=38]
 
     Args:
         path_attrs (Dict[str, Any]): dictionary containing path and node attribute information,
             key: path, value: dict of tree attribute and attribute value
         sep (str): path separator of input `path_attrs` and created tree, defaults to `/`
-        duplicate_name_allowed (bool): indicator if nodes with duplicated `Node` name is allowed, defaults to True
+        duplicate_name_allowed (bool): indicator if nodes with duplicate `Node` name is allowed, defaults to True
         node_type (Type[Node]): node type of tree to be created, defaults to Node
 
     Returns:
         (Node)
     """
     if not len(path_attrs):
         raise ValueError("Dictionary does not contain any data, check `path_attrs`")
@@ -680,14 +688,16 @@
         name_key (str): key of node name, value is type str
         child_key (str): key of child list, value is type list
         node_type (Type[Node]): node type of tree to be created, defaults to Node
 
     Returns:
         (Node)
     """
+    if not node_attrs:
+        raise ValueError("Dictionary does not contain any data, check `node_attrs`")
 
     def recursive_add_child(
         child_dict: Dict[str, Any], parent_node: Optional[Node] = None
     ) -> Node:
         child_dict = child_dict.copy()
         node_name = child_dict.pop(name_key)
         node_children = child_dict.pop(child_key, [])
@@ -750,15 +760,15 @@
     Args:
         data (pd.DataFrame): data containing path and node attribute information
         path_col (str): column of data containing `path_name` information,
             if not set, it will take the first column of data
         attribute_cols (List[str]): columns of data containing node attribute information,
             if not set, it will take all columns of data except `path_col`
         sep (str): path separator of input `path_col` and created tree, defaults to `/`
-        duplicate_name_allowed (bool): indicator if nodes with duplicated `Node` name is allowed, defaults to True
+        duplicate_name_allowed (bool): indicator if nodes with duplicate `Node` name is allowed, defaults to True
         node_type (Type[Node]): node type of tree to be created, defaults to Node
 
     Returns:
         (Node)
     """
     data = data.copy()
 
@@ -789,32 +799,36 @@
         )
 
     root_name = data[path_col].values[0].split(sep)[0]
     root_node = node_type(root_name)
     add_dataframe_to_tree_by_path(
         root_node,
         data,
+        path_col=path_col,
+        attribute_cols=attribute_cols,
         sep=sep,
         duplicate_name_allowed=duplicate_name_allowed,
     )
     root_node.sep = sep
     return root_node
 
 
 def dataframe_to_tree_by_relation(
     data: pd.DataFrame,
     child_col: str = "",
     parent_col: str = "",
     attribute_cols: List[str] = [],
+    allow_duplicates: bool = False,
     node_type: Type[Node] = Node,
 ) -> Node:
     """Construct tree from pandas DataFrame using parent and child names, return root of tree.
 
-    Note that node names must be unique since tree is created from parent-child names,
-    except for leaf nodes - names of leaf nodes may be repeated as there is no confusion.
+    Since tree is created from parent-child names, only names of leaf nodes may be repeated.
+    Error will be thrown if names of intermediate nodes are repeated as there will be confusion.
+    This error can be ignored by setting `allow_duplicates` to be True.
 
     `child_col` and `parent_col` specify columns for child name and parent name to construct tree.
     `attribute_cols` specify columns for node attribute for child name
     If columns are not specified, `child_col` takes first column, `parent_col` takes second column, and all other
     columns are `attribute_cols`.
 
     >>> import pandas as pd
@@ -846,14 +860,16 @@
         data (pd.DataFrame): data containing path and node attribute information
         child_col (str): column of data containing child name information, defaults to None
             if not set, it will take the first column of data
         parent_col (str): column of data containing parent name information, defaults to None
             if not set, it will take the second column of data
         attribute_cols (List[str]): columns of data containing node attribute information,
             if not set, it will take all columns of data except `child_col` and `parent_col`
+        allow_duplicates (bool): allow duplicate intermediate nodes such that child node will
+            be tagged to multiple parent nodes, defaults to False
         node_type (Type[Node]): node type of tree to be created, defaults to Node
 
     Returns:
         (Node)
     """
     data = data.copy()
 
@@ -869,37 +885,40 @@
     if not len(attribute_cols):
         attribute_cols = list(data.columns)
         attribute_cols.remove(child_col)
         attribute_cols.remove(parent_col)
 
     data_check = data.copy()[[child_col, parent_col]].drop_duplicates()
     # Filter for child nodes that are parent of other nodes
-    data_check = data_check[data_check[child_col].isin(data_check[parent_col])]
-    _duplicate_check = (
-        data_check[child_col]
-        .value_counts()
-        .to_frame("counts")
-        .rename_axis(child_col)
-        .reset_index()
-    )
-    _duplicate_check = _duplicate_check[_duplicate_check["counts"] > 1]
-    if len(_duplicate_check):
-        raise ValueError(
-            f"There exists duplicate child with different parent where the child is also a parent node.\n"
-            f"Duplicated node names should not happen, but can only exist in leaf nodes to avoid confusion.\n"
-            f"Check {_duplicate_check}"
+    if not allow_duplicates:
+        data_check = data_check[data_check[child_col].isin(data_check[parent_col])]
+        _duplicate_check = (
+            data_check[child_col]
+            .value_counts()
+            .to_frame("counts")
+            .rename_axis(child_col)
+            .reset_index()
         )
+        _duplicate_check = _duplicate_check[_duplicate_check["counts"] > 1]
+        if len(_duplicate_check):
+            raise ValueError(
+                f"There exists duplicate child with different parent where the child is also a parent node.\n"
+                f"Duplicated node names should not happen, but can only exist in leaf nodes to avoid confusion.\n"
+                f"Check {_duplicate_check}"
+            )
 
     # If parent-child contains None -> root
     root_row = data[data[parent_col].isnull()]
     root_names = list(root_row[child_col])
     if not len(root_names):
         root_names = list(set(data[parent_col]) - set(data[child_col]))
     if len(root_names) != 1:
-        raise ValueError(f"Unable to determine root node\nCheck {root_names}")
+        raise ValueError(
+            f"Unable to determine root node\nPossible root nodes: {root_names}"
+        )
     root_name = root_names[0]
     root_node = node_type(root_name)
 
     def retrieve_attr(_row: Dict[str, Any]) -> Dict[str, Any]:
         node_attrs = _row.copy()
         node_attrs["name"] = node_attrs[child_col]
         del node_attrs[child_col]
```

### Comparing `bigtree-0.9.3/bigtree/tree/export.py` & `bigtree-0.9.4/bigtree/tree/export.py`

 * *Files 1% similar despite different names*

```diff
@@ -729,15 +729,15 @@
             if child_node.path_name not in name_dict[child_label]:  # pragma: no cover
                 name_dict[child_label].append(child_node.path_name)
             child_name = child_label + str(
                 name_dict[child_label].index(child_node.path_name)
             )
             if node_attr and child_node.get_attr(node_attr):
                 _node_style.update(child_node.get_attr(node_attr))
-            if edge_attr:
+            if edge_attr and child_node.get_attr(edge_attr):
                 _edge_style.update(child_node.get_attr(edge_attr))
             node = pydot.Node(name=child_name, label=child_label, **_node_style)
             _graph.add_node(node)
             if parent_name is not None:
                 edge = pydot.Edge(parent_name, child_name, **_edge_style)
                 _graph.add_edge(edge)
             for child in child_node.children:
```

### Comparing `bigtree-0.9.3/bigtree/tree/helper.py` & `bigtree-0.9.4/bigtree/tree/helper.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/bigtree/tree/modify.py` & `bigtree-0.9.4/bigtree/tree/modify.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/bigtree/tree/search.py` & `bigtree-0.9.4/bigtree/tree/search.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/bigtree/utils/iterators.py` & `bigtree-0.9.4/bigtree/utils/iterators.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/bigtree/workflows/app_calendar.py` & `bigtree-0.9.4/bigtree/workflows/app_calendar.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/bigtree/workflows/app_todo.py` & `bigtree-0.9.4/bigtree/workflows/app_todo.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/docs/Makefile` & `bigtree-0.9.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/docs/make.bat` & `bigtree-0.9.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/docs/source/conf.py` & `bigtree-0.9.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/docs/source/index.rst` & `bigtree-0.9.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/docs/source/_static/custom.css` & `bigtree-0.9.4/docs/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/docs/source/_static/favicon.ico` & `bigtree-0.9.4/docs/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/docs/source/_templates/layout.html` & `bigtree-0.9.4/docs/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/docs/source/bigtree/dag/construct.rst` & `bigtree-0.9.4/docs/source/bigtree/dag/construct.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/docs/source/bigtree/dag/export.rst` & `bigtree-0.9.4/docs/source/bigtree/dag/export.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/docs/source/bigtree/tree/construct.rst` & `bigtree-0.9.4/docs/source/bigtree/tree/construct.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/docs/source/bigtree/tree/export.rst` & `bigtree-0.9.4/docs/source/bigtree/tree/export.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/docs/source/bigtree/tree/modify.rst` & `bigtree-0.9.4/docs/source/bigtree/tree/modify.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/docs/source/bigtree/tree/search.rst` & `bigtree-0.9.4/docs/source/bigtree/tree/search.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/docs/source/bigtree/utils/iterators.rst` & `bigtree-0.9.4/docs/source/bigtree/utils/iterators.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/docs/source/others/contributing.rst` & `bigtree-0.9.4/docs/source/others/contributing.rst`

 * *Files 6% similar despite different names*

```diff
@@ -24,28 +24,28 @@
 To check if it worked,
 
 .. code-block:: bash
 
     $ which pip
     /<some directory>/envs/bigtree_venv/bin/pip
 
-From the project folder, install the required python packages locally in editable mode.
+From the project folder, install the required python packages locally in editable mode and set up pre-commit checks.
 
 .. code-block:: bash
 
     $ python -m pip install -e ".[image]"
     $ python -m pip install pre-commit
     $ pre-commit install
 
 Developing
 -----------------------------------
 
 After making your changes, create a new branch, add and commit your changed files.
 In this example, lets assume the changed file is ``README.md``.
-If there are any pre-commit changes, do re-add and re-commit your files.
+If there are any pre-commit changes and/or comments, do modify, re-add and re-commit your files.
 
 .. code-block:: bash
 
     $ git checkout -b chore/update-readme
     $ git add README.md
     $ git commit -m "chore: updated README"
 
@@ -59,30 +59,30 @@
 -----------------------------------
 
 If there are changes related to code, please make sure that the unit tests pass and the code coverage is 100%.
 
 .. code-block:: bash
 
     $ python -m pip install pytest coverage
-    $ pytest . && coverage report --show-missing --omit='*/workflows/*'
+    $ pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=bigtree
 
 Make sure your add/update the tests and documentations accordingly.
 
 Convention and Standards
 -----------------------------------
 
 When creating branches, it is recommended to create them in the format ``type/action``. For example,
 
 .. code-block:: bash
 
     $ git checkout -b feat/add-this
 
 When performing commits, it is also recommended to follow `conventional commits <https://www.conventionalcommits.org/en/v1.0.0/>`_ when writing commit messages.
 
-During pre-commit checks, this project formats code using black and isort.
+During pre-commit checks, this project checks and formats code using ``black``, ``flake8``, ``isort``, and ``mypy``.
 
-For testing, this project uses pytest and coverage package for testing.
+For testing, this project uses ``pytest`` and ``coverage`` package for testing.
 
 Consequent Changes
 -----------------------------------
 
 Please `open an issue <https://github.com/kayjan/bigtree/issues/new/choose>`_ to discuss important changes before embarking on an implementation.
```

### Comparing `bigtree-0.9.3/docs/source/others/merging_trees.md` & `bigtree-0.9.4/docs/source/others/merging_trees.md`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/docs/source/others/nodes.md` & `bigtree-0.9.4/docs/source/others/nodes.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Extending Nodes
 
 Nodes can be extended from `BaseNode` or `Node` class to have extended functionalities or add pre-/post-assign checks.
- - For example, `Node` class extends `BaseNode` and added the ``name`` functionality with pre-assign checks to ensure no duplicated path names.
+ - For example, `Node` class extends `BaseNode` and added the ``name`` functionality with pre-assign checks to ensure no duplicate path names.
 
 ## Population Node (add functionality/method/property)
 
 ```python
 from bigtree import Node, print_tree
```

### Comparing `bigtree-0.9.3/docs/source/others/weighted_trees.md` & `bigtree-0.9.4/docs/source/others/weighted_trees.md`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/tests/conftest.py` & `bigtree-0.9.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/tests/binarytree/test_construct.py` & `bigtree-0.9.4/tests/binarytree/test_construct.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     dataframe_to_tree,
     dataframe_to_tree_by_relation,
     dict_to_tree,
     list_to_tree,
     list_to_tree_by_relation,
     nested_dict_to_tree,
 )
+from tests.constants import Constants
 from tests.node.test_binarynode import assert_binarytree_structure_root2
 
 
 class BinaryNodeA(BinaryNode):
     pass
 
 
@@ -27,24 +28,24 @@
     def tearDown(self):
         self.nums_list = None
 
     def test_list_to_binarytree(self):
         root = list_to_binarytree(self.nums_list)
         assert_binarytree_structure_root2(root)
 
+    def test_list_to_binarytree_empty_error(self):
+        with pytest.raises(ValueError) as exc_info:
+            list_to_binarytree([])
+        assert str(exc_info.value).startswith(Constants.ERROR_BINARY_EMPTY_LIST)
+
     def test_list_to_binarytree_node_type(self):
         root = list_to_binarytree(self.nums_list, node_type=BinaryNodeA)
-        assert isinstance(root, BinaryNodeA), "Node type is not `BinaryNodeA`"
+        assert isinstance(root, BinaryNodeA), Constants.ERROR_BINARY_NODE_TYPE
         assert_binarytree_structure_root2(root)
 
-    def test_list_to_binarytree_error(self):
-        with pytest.raises(ValueError) as exc_info:
-            list_to_binarytree([])
-        assert str(exc_info.value).startswith("Input list does not contain any data")
-
 
 class TestListToTree(unittest.TestCase):
     def setUp(self):
         """
         Binary Tree should have structure
         1
         ├── 2
```

### Comparing `bigtree-0.9.3/tests/binarytree/test_export.py` & `bigtree-0.9.4/tests/binarytree/test_export.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,17 @@
     print_tree,
     tree_to_dataframe,
     tree_to_dict,
     tree_to_dot,
     tree_to_nested_dict,
 )
 from tests.conftest import assert_print_statement
+from tests.constants import Constants
 
-LOCAL = False
+LOCAL = Constants.LOCAL
 
 
 class TestPrintTree:
     @staticmethod
     def test_print_tree(binarytree_node):
         expected_str = """1\n├── 2\n│   ├── 4\n│   │   └── 8\n│   └── 5\n└── 3\n    ├── 6\n    └── 7\n"""
         assert_print_statement(print_tree, expected_str, tree=binarytree_node)
```

### Comparing `bigtree-0.9.3/tests/binarytree/test_helper.py` & `bigtree-0.9.4/tests/binarytree/test_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from bigtree.tree.export import print_tree
 from bigtree.tree.helper import clone_tree, get_tree_diff, prune_tree
 from tests.conftest import assert_print_statement
 
 
 class TestCloneTree:
     @staticmethod
-    def test_clone_tree_btree(binarytree_node):
+    def test_clone_tree(binarytree_node):
         root_clone = clone_tree(binarytree_node, node_type=Node)
         assert isinstance(root_clone, Node), "Wrong type returned"
         expected_str = """1\n├── 2\n│   ├── 4\n│   │   └── 8\n│   └── 5\n└── 3\n    ├── 6\n    └── 7\n"""
         assert_print_statement(print_tree, expected_str, tree=binarytree_node)
 
 
 class TestPruneTree:
```

### Comparing `bigtree-0.9.3/tests/binarytree/test_search.py` & `bigtree-0.9.4/tests/binarytree/test_search.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/tests/dag/test_export.py` & `bigtree-0.9.4/tests/dag/test_export.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,20 +6,21 @@
     dag_to_dict,
     dag_to_dot,
     dag_to_list,
     dataframe_to_dag,
     dict_to_dag,
     list_to_dag,
 )
+from tests.constants import Constants
 from tests.node.test_dagnode import (
-    assert_dag_structure_attr_root,
     assert_dag_structure_root,
+    assert_dag_structure_root_attr,
 )
 
-LOCAL = False
+LOCAL = Constants.LOCAL
 
 
 class TestDAGToList:
     @staticmethod
     def test_dag_to_list(dag_node):
         expected = [
             ("a", "c"),
@@ -53,15 +54,15 @@
             "h": {"parents": ["g"], "age": 6},
         }
         actual = dag_to_dict(dag_node, all_attrs=True)
         assert expected == actual, f"Expected\n{expected}\nReceived\n{actual}"
 
         dag = dict_to_dag(actual)
         assert_dag_structure_root(dag)
-        assert_dag_structure_attr_root(dag)
+        assert_dag_structure_root_attr(dag)
 
     @staticmethod
     def test_dag_to_dict_attr_dict(dag_node):
         expected = {
             "a": {"AGE": 90},
             "c": {"PARENTS": ["a", "b"], "AGE": 60},
             "d": {"PARENTS": ["a", "c"], "AGE": 40},
@@ -95,15 +96,15 @@
             columns=["name", "parent", "age"],
         )
         actual = dag_to_dataframe(dag_node, all_attrs=True)
         pd.testing.assert_frame_equal(expected, actual)
 
         dag = dataframe_to_dag(actual)
         assert_dag_structure_root(dag)
-        assert_dag_structure_attr_root(dag)
+        assert_dag_structure_root_attr(dag)
 
     @staticmethod
     def test_dag_to_dataframe_attr_dict(dag_node):
         expected = pd.DataFrame(
             [
                 ["a", None, 90],
                 ["c", "a", 60],
@@ -162,68 +163,98 @@
                 expected_str in actual
             ), f"Expected {expected_str} not in actual string"
 
     @staticmethod
     def test_dag_to_dot_type_error(tree_node):
         with pytest.raises(ValueError) as exc_info:
             dag_to_dot(tree_node)
-        assert str(exc_info.value).startswith("Tree should be of type `DAGNode`")
+        assert str(exc_info.value) == Constants.ERROR_DAG_TYPE
 
     @staticmethod
-    def test_dag_to_dot_bg_color(dag_node):
+    def test_dag_to_dot_bg_colour(dag_node):
         graph = dag_to_dot(dag_node, bg_colour="blue")
         expected = """strict digraph G {\nbgcolor=blue;\na [label=a];\nc [label=c];\na -> c;\nd [label=d];\na -> d;\nc [label=c];\na [label=a];\na -> c;\nb [label=b];\nb -> c;\nd [label=d];\nc -> d;\nf [label=f];\nc -> f;\ng [label=g];\nc -> g;\nd [label=d];\na [label=a];\na -> d;\nc [label=c];\nc -> d;\ne [label=e];\nd -> e;\nf [label=f];\nd -> f;\ne [label=e];\nd [label=d];\nd -> e;\nf [label=f];\nc [label=c];\nc -> f;\nd [label=d];\nd -> f;\ng [label=g];\nc [label=c];\nc -> g;\nh [label=h];\ng -> h;\nh [label=h];\ng [label=g];\ng -> h;\nb [label=b];\nc [label=c];\nb -> c;\n}\n"""
         actual = graph.to_string()
         if LOCAL:
-            graph.write_png("tests/dag_bg.png")
+            graph.write_png("tests/dag_bg_colour.png")
         for expected_str in expected.split():
             assert (
                 expected_str in actual
             ), f"Expected {expected_str} not in actual string"
 
     @staticmethod
-    def test_dag_to_dot_fill_color(dag_node):
+    def test_dag_to_dot_fill_colour(dag_node):
         graph = dag_to_dot(dag_node, node_colour="gold")
         expected = """strict digraph G {\na [fillcolor=gold, label=a, style=filled];\nc [fillcolor=gold, label=c, style=filled];\na -> c;\nd [fillcolor=gold, label=d, style=filled];\na -> d;\nc [fillcolor=gold, label=c, style=filled];\na [fillcolor=gold, label=a, style=filled];\na -> c;\nb [fillcolor=gold, label=b, style=filled];\nb -> c;\nd [fillcolor=gold, label=d, style=filled];\nc -> d;\nf [fillcolor=gold, label=f, style=filled];\nc -> f;\ng [fillcolor=gold, label=g, style=filled];\nc -> g;\nd [fillcolor=gold, label=d, style=filled];\na [fillcolor=gold, label=a, style=filled];\na -> d;\nc [fillcolor=gold, label=c, style=filled];\nc -> d;\ne [fillcolor=gold, label=e, style=filled];\nd -> e;\nf [fillcolor=gold, label=f, style=filled];\nd -> f;\ne [fillcolor=gold, label=e, style=filled];\nd [fillcolor=gold, label=d, style=filled];\nd -> e;\nf [fillcolor=gold, label=f, style=filled];\nc [fillcolor=gold, label=c, style=filled];\nc -> f;\nd [fillcolor=gold, label=d, style=filled];\nd -> f;\ng [fillcolor=gold, label=g, style=filled];\nc [fillcolor=gold, label=c, style=filled];\nc -> g;\nh [fillcolor=gold, label=h, style=filled];\ng -> h;\nh [fillcolor=gold, label=h, style=filled];\ng [fillcolor=gold, label=g, style=filled];\ng -> h;\nb [fillcolor=gold, label=b, style=filled];\nc [fillcolor=gold, label=c, style=filled];\nb -> c;\n}\n"""
         actual = graph.to_string()
         if LOCAL:
-            graph.write_png("tests/dag_fill.png")
+            graph.write_png("tests/dag_fill_colour.png")
         for expected_str in expected.split():
             assert (
                 expected_str in actual
             ), f"Expected {expected_str} not in actual string"
 
     @staticmethod
     def test_dag_to_dot_edge_colour(dag_node):
         graph = dag_to_dot(dag_node, edge_colour="red")
         expected = """strict digraph G {\na [label=a];\nc [label=c];\na -> c  [color=red];\nd [label=d];\na -> d  [color=red];\nc [label=c];\na [label=a];\na -> c  [color=red];\nb [label=b];\nb -> c  [color=red];\nd [label=d];\nc -> d  [color=red];\nf [label=f];\nc -> f  [color=red];\ng [label=g];\nc -> g  [color=red];\nd [label=d];\na [label=a];\na -> d  [color=red];\nc [label=c];\nc -> d  [color=red];\ne [label=e];\nd -> e  [color=red];\nf [label=f];\nd -> f  [color=red];\ne [label=e];\nd [label=d];\nd -> e  [color=red];\nf [label=f];\nc [label=c];\nc -> f  [color=red];\nd [label=d];\nd -> f  [color=red];\ng [label=g];\nc [label=c];\nc -> g  [color=red];\nh [label=h];\ng -> h  [color=red];\nh [label=h];\ng [label=g];\ng -> h  [color=red];\nb [label=b];\nc [label=c];\nb -> c  [color=red];\n}\n"""
         actual = graph.to_string()
         if LOCAL:
-            graph.write_png("tests/dag_edge.png")
+            graph.write_png("tests/dag_edge_colour.png")
+        for expected_str in expected.split():
+            assert (
+                expected_str in actual
+            ), f"Expected {expected_str} not in actual string"
+
+    @staticmethod
+    def test_dag_to_dot_node_shape(dag_node):
+        graph = dag_to_dot(dag_node, node_shape="triangle")
+        expected = """strict digraph G {\nrankdir=TB;\nc [label=c, shape=triangle];\na [label=a, shape=triangle];\na -> c;\nd [label=d, shape=triangle];\na [label=a, shape=triangle];\na -> d;\nc [label=c, shape=triangle];\nb [label=b, shape=triangle];\nb -> c;\nd [label=d, shape=triangle];\nc [label=c, shape=triangle];\nc -> d;\nf [label=f, shape=triangle];\nc [label=c, shape=triangle];\nc -> f;\ng [label=g, shape=triangle];\nc [label=c, shape=triangle];\nc -> g;\ne [label=e, shape=triangle];\nd [label=d, shape=triangle];\nd -> e;\nf [label=f, shape=triangle];\nd [label=d, shape=triangle];\nd -> f;\nh [label=h, shape=triangle];\ng [label=g, shape=triangle];\ng -> h;\n}\n"""
+        actual = graph.to_string()
+        if LOCAL:
+            graph.write_png("tests/dag_node_shape.png")
         for expected_str in expected.split():
             assert (
                 expected_str in actual
             ), f"Expected {expected_str} not in actual string"
 
     @staticmethod
     def test_dag_to_dot_node_attr(dag_node_style):
         graph = dag_to_dot(dag_node_style, node_attr="node_style")
         expected = """strict digraph G {\na [fillcolor=gold, label=a, style=filled];\nc [fillcolor=gold, label=c, style=filled];\na -> c;\nd [fillcolor=gold, label=d, style=filled];\na -> d;\nc [fillcolor=blue, label=c, style=filled];\na [fillcolor=blue, label=a, style=filled];\na -> c;\nb [fillcolor=blue, label=b, style=filled];\nb -> c;\nd [fillcolor=blue, label=d, style=filled];\nc -> d;\nf [fillcolor=blue, label=f, style=filled];\nc -> f;\ng [fillcolor=blue, label=g, style=filled];\nc -> g;\nd [fillcolor=green, label=d, style=filled];\na [fillcolor=green, label=a, style=filled];\na -> d;\nc [fillcolor=green, label=c, style=filled];\nc -> d;\ne [fillcolor=green, label=e, style=filled];\nd -> e;\nf [fillcolor=green, label=f, style=filled];\nd -> f;\ne [fillcolor=green, label=e, style=filled];\nd [fillcolor=green, label=d, style=filled];\nd -> e;\nf [fillcolor=green, label=f, style=filled];\nc [fillcolor=green, label=c, style=filled];\nc -> f;\nd [fillcolor=green, label=d, style=filled];\nd -> f;\ng [fillcolor=red, label=g, style=filled];\nc [fillcolor=red, label=c, style=filled];\nc -> g;\nh [fillcolor=red, label=h, style=filled];\ng -> h;\nh [fillcolor=red, label=h, style=filled];\ng [fillcolor=red, label=g, style=filled];\ng -> h;\nb [fillcolor=blue, label=b, style=filled];\nc [fillcolor=blue, label=c, style=filled];\nb -> c;\n}\n"""
         actual = graph.to_string()
         if LOCAL:
-            graph.write_png("tests/dag_node_style.png")
+            graph.write_png("tests/dag_node_attr.png")
         for expected_str in expected.split():
             assert (
                 expected_str in actual
             ), f"Expected {expected_str} not in actual string"
 
     @staticmethod
-    def test_tree_to_dot_edge_attr(dag_node_style):
+    def test_dag_to_dot_edge_attr(dag_node_style):
         graph = dag_to_dot(dag_node_style, edge_attr="edge_style")
         expected = """strict digraph G {\nrankdir=TB;\nc [label=c];\na [label=a];\na -> c  [label=c, style=bold];\nd [label=d];\na [label=a];\na -> d  [label=1, style=bold];\nc [label=c];\nb [label=b];\nb -> c  [label=c, style=bold];\nd [label=d];\nc [label=c];\nc -> d  [label=1, style=bold];\nf [label=f];\nc [label=c];\nc -> f  [label=3, style=bold];\ng [label=g];\nc [label=c];\nc -> g  [label=4, style=bold];\ne [label=e];\nd [label=d];\nd -> e  [label=2, style=bold];\nf [label=f];\nd [label=d];\nd -> f  [label=3, style=bold];\nh [label=h];\ng [label=g];\ng -> h  [label=5, style=bold];\n}\n"""
         actual = graph.to_string()
         if LOCAL:
-            graph.write_png("tests/dag_edge_style.png")
+            graph.write_png("tests/dag_edge_attr.png")
+        for expected_str in expected.split():
+            assert (
+                expected_str in actual
+            ), f"Expected {expected_str} not in actual string"
+
+    @staticmethod
+    def test_dag_to_dot_attr_override(dag_node):
+        dag_node.children[0].set_attrs(
+            {
+                "node_style": {"style": "filled", "fillcolor": "blue"},
+                "edge_style": {"style": "bold"},
+            }
+        )
+        graph = dag_to_dot(dag_node, node_attr="node_style", edge_attr="edge_style")
+        expected = """strict digraph G {\nrankdir=TB;\nc [fillcolor=blue, label=c, style=filled];\na [label=a];\na -> c  [style=bold];\nd [label=d];\na [label=a];\na -> d;\nc [fillcolor=blue, label=c, style=filled];\nb [label=b];\nb -> c  [style=bold];\nd [label=d];\nc [fillcolor=blue, label=c, style=filled];\nc -> d;\nf [label=f];\nc [fillcolor=blue, label=c, style=filled];\nc -> f;\ng [label=g];\nc [fillcolor=blue, label=c, style=filled];\nc -> g;\ne [label=e];\nd [label=d];\nd -> e;\nf [label=f];\nd [label=d];\nd -> f;\nh [label=h];\ng [label=g];\ng -> h;\n}\n"""
+        actual = graph.to_string()
+        if LOCAL:
+            graph.write_png("tests/dag_attr_override.png")
         for expected_str in expected.split():
             assert (
                 expected_str in actual
             ), f"Expected {expected_str} not in actual string"
```

### Comparing `bigtree-0.9.3/tests/node/test_basenode.py` & `bigtree-0.9.4/tests/node/test_basenode.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import pytest
 
 from bigtree.node.basenode import BaseNode
 from bigtree.tree.helper import clone_tree
 from bigtree.utils.exceptions import LoopError, TreeError
 from bigtree.utils.iterators import preorder_iter
 from tests.conftest import assert_print_statement
+from tests.constants import Constants
 
 
 class BaseNode2(BaseNode):
     def _BaseNode__post_assign_parent(self, new_parent):
         if new_parent is not None:
             if new_parent.get_attr("val"):
                 raise Exception(
@@ -78,74 +79,42 @@
         self.c.parent = self.a
         self.d.parent = self.b
         self.e.parent = self.b
         self.f.parent = self.c
         self.g.parent = self.e
         self.h.parent = self.e
 
-        assert_tree_structure_basenode_root_generic(self.a)
+        assert_tree_structure_basenode_root(self.a)
         assert_tree_structure_basenode_root_attr(self.a)
         assert_tree_structure_basenode_self(self)
         assert_print_statement(print, "BaseNode(age=90, name=a)\n", self.a)
 
-    def test_set_parent_error(self):
+    def test_set_parents_error(self):
         with pytest.raises(ValueError) as exc_info:
             self.b.parents = [self.a]
-        assert str(exc_info.value).startswith("Attempting to set `parents` attribute")
+        assert str(exc_info.value) == Constants.ERROR_SET_PARENTS_ATTR
 
         with pytest.raises(ValueError) as exc_info:
             self.b = BaseNode(parents=[self.a])
-        assert str(exc_info.value).startswith("Attempting to set `parents` attribute")
+        assert str(exc_info.value) == Constants.ERROR_SET_PARENTS_ATTR
 
         with pytest.raises(ValueError) as exc_info:
             self.b.parents
-        assert str(exc_info.value).startswith(
-            "Attempting to access `parents` attribute"
-        )
-
-    def test_set_parent_reassign(self):
-        self.a.children = [self.b, self.c]
-        self.d.children = [self.e]
-        self.b.parent = self.d
-        assert list(self.a.children) == [
-            self.c
-        ], f"Node a children, expected {[self.c]}, received {self.a.children}"
-        assert list(self.d.children) == [
-            self.e,
-            self.b,
-        ], f"Node d children, expected {[self.e, self.b]}, received {self.d.children}"
-        assert (
-            self.b.parent == self.d
-        ), f"Node b parent, expected {self.d}, received {self.b.parent}"
-
-    def test_set_children_reassign(self):
-        self.a.children = [self.c]
-        self.b.parent = self.a
-        self.d.children = [self.e, self.b]
-        assert list(self.a.children) == [
-            self.c
-        ], f"Node a children, expected {[self.c]}, received {self.a.children}"
-        assert list(self.d.children) == [
-            self.e,
-            self.b,
-        ], f"Node d children, expected {[self.e, self.b]}, received {self.d.children}"
-        assert (
-            self.b.parent == self.d
-        ), f"Node b parent, expected {self.d}, received {self.b.parent}"
+        assert str(exc_info.value) == Constants.ERROR_GET_PARENTS_ATTR
 
     def test_set_parent(self):
         self.b.parent = self.a
         self.c.parent = self.a
         self.d.parent = self.b
         self.e.parent = self.b
         self.f.parent = self.c
         self.g.parent = self.e
         self.h.parent = self.e
 
-        assert_tree_structure_basenode_root_generic(self.a)
+        assert_tree_structure_basenode_root(self.a)
         assert_tree_structure_basenode_root_attr(self.a)
         assert_tree_structure_basenode_self(self)
 
     def test_set_parent_sort(self):
         self.h.parent = self.e
         self.g.parent = self.e
         self.f.parent = self.c
@@ -153,55 +122,55 @@
         self.d.parent = self.b
         self.c.parent = self.a
         self.b.parent = self.a
 
         self.a.sort(key=lambda x: x.name)
         self.b.sort(key=lambda x: x.name)
         self.e.sort(key=lambda x: x.name)
-        assert_tree_structure_basenode_root_generic(self.a)
+        assert_tree_structure_basenode_root(self.a)
         assert_tree_structure_basenode_root_attr(self.a)
         assert_tree_structure_basenode_self(self)
 
     def test_set_parent_rshift(self):
         self.a >> self.b
         self.a >> self.c
         self.b >> self.d
         self.b >> self.e
         self.c >> self.f
         self.e >> self.g
         self.e >> self.h
 
-        assert_tree_structure_basenode_root_generic(self.a)
+        assert_tree_structure_basenode_root(self.a)
         assert_tree_structure_basenode_root_attr(self.a)
         assert_tree_structure_basenode_self(self)
 
     def test_set_parent_lshift(self):
         self.b << self.a
         self.c << self.a
         self.d << self.b
         self.e << self.b
         self.f << self.c
         self.g << self.e
         self.h << self.e
 
-        assert_tree_structure_basenode_root_generic(self.a)
+        assert_tree_structure_basenode_root(self.a)
         assert_tree_structure_basenode_root_attr(self.a)
         assert_tree_structure_basenode_self(self)
 
     def test_set_parent_constructor(self):
         self.a = BaseNode(name="a", age=90)
         self.b = BaseNode(name="b", age=65, parent=self.a)
         self.c = BaseNode(name="c", age=60, parent=self.a)
         self.d = BaseNode(name="d", age=40, parent=self.b)
         self.e = BaseNode(name="e", age=35, parent=self.b)
         self.f = BaseNode(name="f", age=38, parent=self.c)
         self.g = BaseNode(name="g", age=10, parent=self.e)
         self.h = BaseNode(name="h", age=6, parent=self.e)
 
-        assert_tree_structure_basenode_root_generic(self.a)
+        assert_tree_structure_basenode_root(self.a)
         assert_tree_structure_basenode_root_attr(self.a)
         assert_tree_structure_basenode_self(self)
 
     def test_set_parent_null_parent(self):
         self.b.parent = self.a
         self.c.parent = self.a
         self.d.parent = self.b
@@ -213,113 +182,140 @@
         dummy = BaseNode()
         dummy.parent = self.h
         assert list(self.h.children) == [dummy]
 
         dummy.parent = None
         assert not len(list(self.h.children))
 
-        assert_tree_structure_basenode_root_generic(self.a)
+        assert_tree_structure_basenode_root(self.a)
         assert_tree_structure_basenode_root_attr(self.a)
         assert_tree_structure_basenode_self(self)
 
+    def test_set_parent_reassign(self):
+        self.a.children = [self.b, self.c]
+        self.d.children = [self.e]
+        self.b.parent = self.d
+        assert list(self.a.children) == [
+            self.c
+        ], f"Node a children, expected {[self.c]}, received {self.a.children}"
+        assert list(self.d.children) == [
+            self.e,
+            self.b,
+        ], f"Node d children, expected {[self.e, self.b]}, received {self.d.children}"
+        assert (
+            self.b.parent == self.d
+        ), f"Node b parent, expected {self.d}, received {self.b.parent}"
+
     def test_set_parent_duplicate(self):
-        # Set parent again
         self.b.parent = self.a
         self.b.parent = self.a
         assert list(self.a.children) == [self.b]
         assert self.b.parent == self.a
 
     def test_set_parent_duplicate_constructor(self):
-        # Set parent again
         self.a = BaseNode(name="a", age=90)
         self.b = BaseNode(name="b", age=65, parent=self.a)
         self.b.parent = self.a
         assert list(self.a.children) == [self.b]
         assert self.b.parent == self.a
 
     def test_set_children(self):
         self.a.children = [self.b, self.c]
         self.b.children = [self.d, self.e]
         self.c.children = [self.f]
         self.e.children = [self.g, self.h]
 
-        assert_tree_structure_basenode_root_generic(self.a)
+        assert_tree_structure_basenode_root(self.a)
         assert_tree_structure_basenode_root_attr(self.a)
         assert_tree_structure_basenode_self(self)
 
     def test_set_children_sort(self):
         self.a.children = [self.c, self.b]
         self.b.children = [self.e, self.d]
         self.c.children = [self.f]
         self.e.children = [self.h, self.g]
 
         self.a.sort(key=lambda x: x.name)
         self.b.sort(key=lambda x: x.name)
         self.e.sort(key=lambda x: x.name)
-        assert_tree_structure_basenode_root_generic(self.a)
+        assert_tree_structure_basenode_root(self.a)
         assert_tree_structure_basenode_root_attr(self.a)
         assert_tree_structure_basenode_self(self)
 
     def test_set_children_constructor(self):
         self.h = BaseNode(name="h", age=6)
         self.g = BaseNode(name="g", age=10)
         self.f = BaseNode(name="f", age=38)
         self.e = BaseNode(name="e", age=35, children=[self.g, self.h])
         self.d = BaseNode(name="d", age=40)
         self.c = BaseNode(name="c", age=60, children=[self.f])
         self.b = BaseNode(name="b", age=65, children=[self.d, self.e])
         self.a = BaseNode(name="a", age=90, children=[self.b, self.c])
 
-        assert_tree_structure_basenode_root_generic(self.a)
+        assert_tree_structure_basenode_root(self.a)
         assert_tree_structure_basenode_root_attr(self.a)
         assert_tree_structure_basenode_self(self)
 
     def test_set_children_null_children(self):
         self.a.children = [self.b, self.c]
         self.b.children = [self.d, self.e]
         self.c.children = [self.f]
         self.e.children = [self.g, self.h]
 
         dummy = BaseNode()
         self.h.children = [dummy]
         assert dummy.parent == self.h
         self.h.children = []
 
-        assert_tree_structure_basenode_root_generic(self.a)
+        assert_tree_structure_basenode_root(self.a)
         assert_tree_structure_basenode_root_attr(self.a)
         assert_tree_structure_basenode_self(self)
 
     def test_set_children_null_parent(self):
         self.a.children = [self.b, self.c]
         self.b.children = [self.d, self.e]
         self.c.children = [self.f]
         self.e.children = [self.g, self.h]
 
         dummy = BaseNode()
         self.h.children = [dummy]
         assert dummy.parent == self.h
         dummy.parent.children = []
 
-        assert_tree_structure_basenode_root_generic(self.a)
+        assert_tree_structure_basenode_root(self.a)
         assert_tree_structure_basenode_root_attr(self.a)
         assert_tree_structure_basenode_self(self)
 
-    def test_set_children_none_parent(self):
-        with pytest.raises(TypeError):
+    def test_set_children_none_parent_error(self):
+        with pytest.raises(TypeError) as exc_info:
             self.h.children = None
+        assert str(exc_info.value).startswith(Constants.ERROR_CHILDREN_TYPE)
+
+    def test_set_children_reassign(self):
+        self.a.children = [self.c]
+        self.b.parent = self.a
+        self.d.children = [self.e, self.b]
+        assert list(self.a.children) == [
+            self.c
+        ], f"Node a children, expected {[self.c]}, received {self.a.children}"
+        assert list(self.d.children) == [
+            self.e,
+            self.b,
+        ], f"Node d children, expected {[self.e, self.b]}, received {self.d.children}"
+        assert (
+            self.b.parent == self.d
+        ), f"Node b parent, expected {self.d}, received {self.b.parent}"
 
     def test_set_children_duplicate(self):
-        # Set child again
         self.a.children = [self.b]
         self.a.children = [self.b]
         assert list(self.a.children) == [self.b]
         assert self.b.parent == self.a
 
     def test_set_children_duplicate_constructor(self):
-        # Set child again
         self.a = BaseNode(children=[self.b])
         self.a.children = [self.b]
         assert list(self.a.children) == [self.b]
         assert self.b.parent == self.a
 
     def test_deep_copy_set_children(self):
         self.a.children = [self.b, self.c]
@@ -331,15 +327,15 @@
         assert (
             len(a2.children) == 2
         ), f"Expected 2 children, received {len(a2.children)}"
         assert (
             not a2.children[0] == self.b and not a2.children[1] == self.b
         ), "Copy does not copy child nodes"
         assert not a2.children == [self.b, self.c], "Copy does not copy child nodes"
-        assert_tree_structure_basenode_root_generic(a2)
+        assert_tree_structure_basenode_root(a2)
         assert_tree_structure_basenode_root_attr(a2)
 
     def test_shallow_copy_set_children(self):
         self.a.children = [self.b, self.c]
         self.b.children = [self.d, self.e]
         self.c.children = [self.f]
         self.e.children = [self.g, self.h]
@@ -348,53 +344,57 @@
         assert (
             len(a2.children) == 2
         ), f"Expected 2 children, received {len(a2.children)}"
         assert (
             a2.children[0] == self.b or a2.children[1] == self.b
         ), "Shallow copy does not copy child nodes"
         assert a2.children == (self.b, self.c), "Shallow copy does not copy child nodes"
-        assert_tree_structure_basenode_root_generic(a2)
+        assert_tree_structure_basenode_root(a2)
         assert_tree_structure_basenode_root_attr(a2)
 
-    def test_error_set_parent_type_error(self):
-        # Error: wrong type
-        with pytest.raises(TypeError):
+    def test_set_parent_type_error(self):
+        with pytest.raises(TypeError) as exc_info:
             self.a.parent = 1
+        assert str(exc_info.value).startswith(Constants.ERROR_BASENODE_PARENT_TYPE)
 
-    def test_error_set_parent_loop_error(self):
-        # Error: set self as parent
-        with pytest.raises(LoopError):
+    def test_set_parent_loop_error(self):
+        with pytest.raises(LoopError) as exc_info:
             self.a.parent = self.a
+        assert str(exc_info.value) == Constants.ERROR_LOOP_PARENT
 
-        # Error: set descendant as parent
-        with pytest.raises(LoopError):
+        with pytest.raises(LoopError) as exc_info:
             self.b.parent = self.a
             self.c.parent = self.b
             self.a.parent = self.c
+        assert str(exc_info.value) == Constants.ERROR_LOOP_ANCESTOR
 
-    def test_error_set_children_type_error(self):
-        # Error: wrong type
-        with pytest.raises(TypeError):
+    def test_set_children_type_error(self):
+        with pytest.raises(TypeError) as exc_info:
             self.a.children = [self.b, 1]
+        assert str(exc_info.value).startswith(Constants.ERROR_BASENODE_CHILDREN_TYPE)
+
+        with pytest.raises(TypeError) as exc_info:
+            self.a.children = [self.b, None]
+        assert str(exc_info.value).startswith(Constants.ERROR_BASENODE_CHILDREN_TYPE)
 
-    def test_error_set_children_loop_error(self):
-        # Error: set self as child
-        with pytest.raises(LoopError):
+    def test_set_children_loop_error(self):
+        with pytest.raises(LoopError) as exc_info:
             self.a.children = [self.b, self.a]
+        assert str(exc_info.value) == Constants.ERROR_LOOP_CHILD
 
-        # Error: set ancestor as child
-        with pytest.raises(LoopError):
+        with pytest.raises(LoopError) as exc_info:
             self.a.children = [self.b, self.c]
             self.c.children = [self.d, self.e, self.f]
             self.f.children = [self.a]
+        assert str(exc_info.value) == Constants.ERROR_LOOP_DESCENDANT
 
-    def test_error_set_children_exception(self):
-        # Error: duplicate child
-        with pytest.raises(TreeError):
+    def test_set_duplicate_children_error(self):
+        with pytest.raises(TreeError) as exc_info:
             self.a.children = [self.b, self.b]
+        assert str(exc_info.value) == Constants.ERROR_SET_DUPLICATE_CHILD
 
     def test_rollback_set_parent(self):
         a = clone_tree(self.a, BaseNode2)
         b = clone_tree(self.b, BaseNode2)
         c = clone_tree(self.c, BaseNode2)
         d = clone_tree(self.d, BaseNode2)
         e = clone_tree(self.e, BaseNode2)
@@ -608,15 +608,16 @@
             for child in children:
                 if child:
                     assert (
                         child.parent == parent
                     ), f"Node {child} parent, expected {parent}, received {child.parent}"
 
 
-def assert_tree_structure_basenode_root_generic(root):
+def assert_tree_structure_basenode_root(root):
+    """Test tree structure (i.e., ancestors, descendants, leaves, siblings, etc.)"""
     # Test ancestors
     expected = 0
     actual = len(list(root.ancestors))
     assert (
         actual == expected
     ), f"Node {root} should have {expected} ancestors, but it has {actual} ancestors"
 
@@ -718,14 +719,15 @@
     c=("c", 60),
     d=("d", 40),
     e=("e", 35),
     f=("f", 38),
     g=("g", 10),
     h=("h", 6),
 ):
+    """Test tree structure with age attributes"""
     # Test describe()
     expected = [("age", 90), ("name", "a")]
     actual = root.describe(exclude_prefix="_")
     assert (
         actual == expected
     ), f"Node description should be {expected}, but it is {actual}"
 
@@ -735,14 +737,15 @@
         actual = node.get_attr("name"), node.get_attr("age")
         assert (
             actual == expected
         ), f"Node name and age should be {expected}, but it is {actual}"
 
 
 def assert_tree_structure_basenode_self(self):
+    """Test tree structure with self object"""
     nodes = [self.a, self.b, self.c, self.d, self.e, self.f, self.g, self.h]
 
     # Test ancestors
     expected_ans = [0, 1, 1, 2, 2, 2, 3, 3]
     for node, expected in zip(nodes, expected_ans):
         actual = len(list(node.ancestors))
         assert (
```

### Comparing `bigtree-0.9.3/tests/node/test_binarynode.py` & `bigtree-0.9.4/tests/node/test_binarynode.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from bigtree.node.basenode import BaseNode
 from bigtree.node.binarynode import BinaryNode
 from bigtree.node.node import Node
 from bigtree.tree.helper import clone_tree
 from bigtree.utils.exceptions import LoopError, TreeError
 from tests.conftest import assert_print_statement
+from tests.constants import Constants
 
 
 class BinaryNode2(BinaryNode):
     def _BinaryNode__post_assign_parent(self, new_parent):
         if new_parent is not None:
             if new_parent.val == 100:
                 raise Exception(
@@ -85,100 +86,45 @@
         assert not self.h.left, f"Expected {None}, received {self.h.left}"
         assert not self.h.right, f"Expected {None}, received {self.h.right}"
         self.a.sep = "\\"
         assert (
             self.b.path_name == "\\1\\2"
         ), f"Expected \\1\\2, received {self.b.path_name}"
 
-    def test_set_parent_error(self):
+    def test_set_parents_error(self):
         with pytest.raises(ValueError) as exc_info:
             self.b.parents = [self.a]
-        assert str(exc_info.value).startswith("Attempting to set `parents` attribute")
+        assert str(exc_info.value) == Constants.ERROR_SET_PARENTS_ATTR
 
         with pytest.raises(ValueError) as exc_info:
             self.b = BinaryNode(1, parents=[self.a])
-        assert str(exc_info.value).startswith("Attempting to set `parents` attribute")
+        assert str(exc_info.value) == Constants.ERROR_SET_PARENTS_ATTR
 
         with pytest.raises(ValueError) as exc_info:
             self.b.parents
-        assert str(exc_info.value).startswith(
-            "Attempting to access `parents` attribute"
-        )
-
-    def test_set_parent_3_parent_error(self):
-        self.b.parent = self.a
-        self.c.parent = self.a
-        with pytest.raises(TreeError) as exc_info:
-            self.d.parent = self.a
-        assert str(exc_info.value).endswith("already has 2 children")
-
-    def test_set_parent_position(self):
-        self.a.children = [self.b, self.c]
-        self.b.parent = self.d
-        assert not self.a.left, f"Node a left, expected None, received {self.a.left}"
-        assert (
-            self.a.right == self.c
-        ), f"Node a right, expected {self.c}, received {self.a.right}"
-        assert (
-            self.d.left == self.b
-        ), f"Node d left, expected {self.b}, received {self.d.left}"
-        assert not self.d.right, f"Node d right, expected None, received {self.d.right}"
-
-    def test_set_parent_position_right(self):
-        self.a.children = [self.b, self.c]
-        self.e.parent = self.d
-        self.b.parent = self.d
-        assert not self.a.left, f"Node a left, expected None, received {self.a.left}"
-        assert (
-            self.a.right == self.c
-        ), f"Node a right, expected {self.c}, received {self.a.right}"
-        assert (
-            self.d.left == self.e
-        ), f"Node d left, expected {self.e}, received {self.d.left}"
-        assert (
-            self.d.right == self.b
-        ), f"Node d right, expected {self.b}, received {self.d.right}"
-
-    def test_set_children_position(self):
-        self.a.children = [self.b, self.c]
-        self.d.children = [self.b, None]
-        assert not self.a.left, f"Node a left, expected None, received {self.a.left}"
-        assert (
-            self.a.right == self.c
-        ), f"Node a right, expected {self.c}, received {self.a.right}"
-        assert (
-            self.d.left == self.b
-        ), f"Node d left, expected {self.b}, received {self.d.left}"
-        assert not self.d.right, f"Node d right, expected None, received {self.d.right}"
-
-    def test_set_children_position_right(self):
-        self.a.children = [self.b, self.c]
-        self.d.children = [self.e, self.b]
-        assert not self.a.left, f"Node a left, expected None, received {self.a.left}"
-        assert (
-            self.a.right == self.c
-        ), f"Node a right, expected {self.c}, received {self.a.right}"
-        assert (
-            self.d.left == self.e
-        ), f"Node d left, expected {self.e}, received {self.d.left}"
-        assert (
-            self.d.right == self.b
-        ), f"Node d right, expected {self.b}, received {self.d.right}"
+        assert str(exc_info.value) == Constants.ERROR_GET_PARENTS_ATTR
 
     def test_set_parent(self):
         self.b.parent = self.a
         self.c.parent = self.a
         self.d.parent = self.b
         self.e.parent = self.b
         self.f.parent = self.c
         self.g.parent = self.c
         self.d.children = [None, self.h]
 
         assert_binarytree_structure_self(self)
 
+    def test_set_parent_3_parent_error(self):
+        self.b.parent = self.a
+        self.c.parent = self.a
+        with pytest.raises(TreeError) as exc_info:
+            self.d.parent = self.a
+        assert str(exc_info.value).endswith("already has 2 children")
+
     def test_set_parent_children_insert(self):
         self.a.children = [None, None]
         self.b.parent = self.a
         self.c.parent = self.a
         self.b.children = [self.d, None]
         self.e.parent = self.b
         self.c.children = [None, self.g]
@@ -253,23 +199,48 @@
         dummy = BinaryNode(100)
         dummy.parent = self.h
         assert list(self.h.children) == [dummy, None]
 
         dummy.parent = None
         assert_binarytree_structure_self(self)
 
+    def test_set_parent_reassign(self):
+        self.a.children = [self.b, self.c]
+        self.b.parent = self.d
+        assert not self.a.left, f"Node a left, expected None, received {self.a.left}"
+        assert (
+            self.a.right == self.c
+        ), f"Node a right, expected {self.c}, received {self.a.right}"
+        assert (
+            self.d.left == self.b
+        ), f"Node d left, expected {self.b}, received {self.d.left}"
+        assert not self.d.right, f"Node d right, expected None, received {self.d.right}"
+
+    def test_set_parent_reassign_right(self):
+        self.a.children = [self.b, self.c]
+        self.e.parent = self.d
+        self.b.parent = self.d
+        assert not self.a.left, f"Node a left, expected None, received {self.a.left}"
+        assert (
+            self.a.right == self.c
+        ), f"Node a right, expected {self.c}, received {self.a.right}"
+        assert (
+            self.d.left == self.e
+        ), f"Node d left, expected {self.e}, received {self.d.left}"
+        assert (
+            self.d.right == self.b
+        ), f"Node d right, expected {self.b}, received {self.d.right}"
+
     def test_set_parent_duplicate(self):
-        # Set parent again
         self.b.parent = self.a
         self.b.parent = self.a
         assert list(self.a.children) == [self.b, None]
         assert self.b.parent == self.a
 
     def test_set_parent_duplicate_constructor(self):
-        # Set parent again
         self.a = BinaryNode(1)
         self.b = BinaryNode(2, parent=self.a)
         self.b.parent = self.a
         assert list(self.a.children) == [self.b, None]
         assert self.b.parent == self.a
 
     def test_set_left_and_right(self):
@@ -306,50 +277,45 @@
         self.a = BinaryNode(1, left=self.b, right=self.c, children=[self.b, self.c])
 
         assert_binarytree_structure_self(self)
 
     def test_set_left_and_right_and_children_constructor_error(self):
         with pytest.raises(ValueError) as exc_info:
             self.a = BinaryNode(1, left=self.b, right=self.c, children=[self.c])
-        assert str(exc_info.value).startswith("Children input must have length 2")
+        assert str(exc_info.value) == Constants.ERROR_BINARYNODE_CHILDREN_LENGTH
 
         with pytest.raises(ValueError) as exc_info:
             self.a = BinaryNode(1, left=self.b, right=self.c, children=[self.d, self.c])
-        assert str(exc_info.value).startswith(
-            "Attempting to set both left and children with mismatched values"
-        )
+        assert str(exc_info.value).startswith(Constants.ERROR_SET_LEFT_CHILDREN)
 
         with pytest.raises(ValueError) as exc_info:
             self.a = BinaryNode(1, left=self.b, right=self.c, children=[self.b, self.d])
-        assert str(exc_info.value).startswith(
-            "Attempting to set both right and children with mismatched values"
-        )
+        assert str(exc_info.value).startswith(Constants.ERROR_SET_RIGHT_CHILDREN)
 
     def test_set_left_and_right_duplicate(self):
-        # Set parent again
         self.a = BinaryNode(1, left=self.b, right=self.c)
         self.a.left = self.b
         self.a.right = self.c
         assert list(self.a.children) == [self.b, self.c]
         assert self.b.parent == self.a
         assert self.c.parent == self.a
 
-    def test_set_children_3_children_error(self):
-        with pytest.raises(ValueError) as exc_info:
-            self.a.children = [self.b, self.c, self.d]
-        assert str(exc_info.value) == "Children input must have length 2"
-
     def test_set_children(self):
         self.a.children = [self.b, self.c]
         self.b.children = [self.d, self.e]
         self.c.children = [self.f, self.g]
         self.d.children = [None, self.h]
 
         assert_binarytree_structure_self(self)
 
+    def test_set_children_3_children_error(self):
+        with pytest.raises(ValueError) as exc_info:
+            self.a.children = [self.b, self.c, self.d]
+        assert str(exc_info.value) == Constants.ERROR_BINARYNODE_CHILDREN_LENGTH
+
     def test_set_children_sort(self):
         self.a.children = [self.c, self.b]
         self.b.children = [self.e, self.d]
         self.c.children = [self.g, self.f]
         self.d.children = [None, self.h]
 
         self.a.sort(key=lambda x: x.val)
@@ -396,27 +362,52 @@
         dummy = BinaryNode(100)
         self.h.children = [dummy, None]
         assert dummy.parent == self.h
         dummy.parent.children = []
 
         assert_binarytree_structure_self(self)
 
-    def test_set_children_none_parent(self):
-        with pytest.raises(TypeError):
+    def test_set_children_none_parent_error(self):
+        with pytest.raises(TypeError) as exc_info:
             self.h.children = None
+        assert str(exc_info.value).startswith(Constants.ERROR_CHILDREN_TYPE)
+
+    def test_set_children_reassign(self):
+        self.a.children = [self.b, self.c]
+        self.d.children = [self.b, None]
+        assert not self.a.left, f"Node a left, expected None, received {self.a.left}"
+        assert (
+            self.a.right == self.c
+        ), f"Node a right, expected {self.c}, received {self.a.right}"
+        assert (
+            self.d.left == self.b
+        ), f"Node d left, expected {self.b}, received {self.d.left}"
+        assert not self.d.right, f"Node d right, expected None, received {self.d.right}"
+
+    def test_set_children_reassign_right(self):
+        self.a.children = [self.b, self.c]
+        self.d.children = [self.e, self.b]
+        assert not self.a.left, f"Node a left, expected None, received {self.a.left}"
+        assert (
+            self.a.right == self.c
+        ), f"Node a right, expected {self.c}, received {self.a.right}"
+        assert (
+            self.d.left == self.e
+        ), f"Node d left, expected {self.e}, received {self.d.left}"
+        assert (
+            self.d.right == self.b
+        ), f"Node d right, expected {self.b}, received {self.d.right}"
 
     def test_set_children_duplicate(self):
-        # Set child again
         self.a.children = [self.b, None]
         self.a.children = [self.b, None]
         assert list(self.a.children) == [self.b, None]
         assert self.b.parent == self.a
 
     def test_set_children_duplicate_constructor(self):
-        # Set child again
         self.a = BinaryNode(1, children=[self.b, None])
         self.a.children = [self.b, None]
         assert list(self.a.children) == [self.b, None]
         assert self.b.parent == self.a
 
     def test_deep_copy_set_children(self):
         self.a.children = [self.b, self.c]
@@ -430,75 +421,79 @@
         ), f"Expected 2 children, received {len(a2.children)}"
         assert (
             not a2.children[0] == self.b and not a2.children[1] == self.b
         ), "Copy does not copy child nodes"
         assert not a2.children == [self.b, self.c], "Copy does not copy child nodes"
         assert_binarytree_structure_root(a2)
 
-    def test_error_set_parent_type_error(self):
-        # Error: wrong type
-        with pytest.raises(TypeError):
+    def test_set_parent_type_error(self):
+        with pytest.raises(TypeError) as exc_info:
             self.a.parent = 1
+        assert str(exc_info.value).startswith(Constants.ERROR_BINARYNODE_TYPE)
 
         a = BaseNode()
-        with pytest.raises(TypeError):
+        with pytest.raises(TypeError) as exc_info:
             self.a.parent = a
+        assert str(exc_info.value).startswith(Constants.ERROR_BINARYNODE_TYPE)
 
         a = Node("a")
-        with pytest.raises(TypeError):
+        with pytest.raises(TypeError) as exc_info:
             self.a.parent = a
+        assert str(exc_info.value).startswith(Constants.ERROR_BINARYNODE_TYPE)
 
-    def test_error_set_parent_loop_error(self):
-        # Error: set self as parent
-        with pytest.raises(LoopError):
+    def test_set_parent_loop_error(self):
+        with pytest.raises(LoopError) as exc_info:
             self.a.parent = self.a
+        assert str(exc_info.value) == Constants.ERROR_LOOP_PARENT
 
-        # Error: set descendant as parent
-        with pytest.raises(LoopError):
+        with pytest.raises(LoopError) as exc_info:
             self.b.parent = self.a
             self.c.parent = self.b
             self.a.parent = self.c
+        assert str(exc_info.value) == Constants.ERROR_LOOP_ANCESTOR
 
-    def test_error_set_children_type_error(self):
-        # Error: wrong type
-        with pytest.raises(TypeError):
+    def test_set_children_type_error(self):
+        with pytest.raises(TypeError) as exc_info:
             self.a.children = self.b
+        assert str(exc_info.value).startswith(Constants.ERROR_CHILDREN_TYPE)
 
-        with pytest.raises(TypeError):
+        with pytest.raises(TypeError) as exc_info:
             self.a.children = [self.b, 1]
+        assert str(exc_info.value).startswith(Constants.ERROR_BINARYNODE_TYPE)
 
         a = BaseNode()
-        with pytest.raises(TypeError):
+        with pytest.raises(TypeError) as exc_info:
             self.a.children = [a, None]
+        assert str(exc_info.value).startswith(Constants.ERROR_BINARYNODE_TYPE)
 
         a = Node("a")
-        with pytest.raises(TypeError):
+        with pytest.raises(TypeError) as exc_info:
             self.a.children = [a, None]
+        assert str(exc_info.value).startswith(Constants.ERROR_BINARYNODE_TYPE)
 
-    def test_error_set_children_length_error(self):
-        # Error: wrong type
+    def test_set_children_length_error(self):
         with pytest.raises(ValueError) as exc_info:
             self.a.children = [self.b]
-        assert str(exc_info.value).startswith("Children input must have length 2")
+        assert str(exc_info.value) == Constants.ERROR_BINARYNODE_CHILDREN_LENGTH
 
-    def test_error_set_children_loop_error(self):
-        # Error: set self as child
-        with pytest.raises(LoopError):
+    def test_set_children_loop_error(self):
+        with pytest.raises(LoopError) as exc_info:
             self.a.children = [self.b, self.a]
+        assert str(exc_info.value) == Constants.ERROR_LOOP_CHILD
 
-        # Error: set ancestor as child
-        with pytest.raises(LoopError):
+        with pytest.raises(LoopError) as exc_info:
             self.a.children = [self.b, self.c]
             self.c.children = [self.d, self.e]
             self.e.children = [self.a, self.f]
+        assert str(exc_info.value) == Constants.ERROR_LOOP_DESCENDANT
 
-    def test_error_set_children_exception(self):
-        # Error: duplicate child
-        with pytest.raises(TreeError):
+    def test_set_duplicate_children_error(self):
+        with pytest.raises(TreeError) as exc_info:
             self.a.children = [self.b, self.b]
+        assert str(exc_info.value) == Constants.ERROR_SET_DUPLICATE_CHILD
 
     def test_rollback_set_parent(self):
         a = clone_tree(self.a, BinaryNode2)
         b = clone_tree(self.b, BinaryNode2)
         c = clone_tree(self.c, BinaryNode2)
         d = clone_tree(self.d, BinaryNode2)
         e = clone_tree(self.e, BinaryNode2)
@@ -745,15 +740,39 @@
             for child in children:
                 if child:
                     assert (
                         child.parent == parent
                     ), f"Node {child} parent, expected {parent}, received {child.parent}"
 
 
+def assert_binarytree_structure_root(root):
+    """Test tree structure"""
+    a = root
+    b, c = a.children
+    d, e = b.children
+    f, g = c.children
+    _, h = d.children
+
+    class Sample:
+        pass
+
+    self = Sample()
+    self.a = a
+    self.b = b
+    self.c = c
+    self.d = d
+    self.e = e
+    self.f = f
+    self.g = g
+    self.h = h
+    assert_binarytree_structure_self(self)
+
+
 def assert_binarytree_structure_self(self):
+    """Test tree structure with self object"""
     nodes = [self.a, self.b, self.c, self.d, self.e, self.f, self.g, self.h]
 
     # Test parent
     expected_ans = [None, self.a, self.a, self.b, self.b, self.c, self.c, self.d]
     for node, expected in zip(nodes, expected_ans):
         actual = node.parent
         assert expected == actual, f"Expected parent {expected}, received {actual}"
@@ -909,37 +928,39 @@
     # Test get_attr()
     expected_ans = [1, 2, 3, 4, 5, 6, 7, 8]
     for node, expected in zip(nodes, expected_ans):
         actual = node.get_attr("val")
         assert expected == actual, f"Expected right {expected}, received {actual}"
 
 
-def assert_binarytree_structure_root(root):
+def assert_binarytree_structure_root2(root):
+    """Test tree structure"""
     a = root
     b, c = a.children
     d, e = b.children
     f, g = c.children
-    _, h = d.children
+    h, _ = d.children
 
     class Sample:
         pass
 
     self = Sample()
     self.a = a
     self.b = b
     self.c = c
     self.d = d
     self.e = e
     self.f = f
     self.g = g
     self.h = h
-    assert_binarytree_structure_self(self)
+    assert_binarytree_structure_self2(self)
 
 
 def assert_binarytree_structure_self2(self):
+    """Test tree structure with self object"""
     nodes = [self.a, self.b, self.c, self.d, self.e, self.f, self.g, self.h]
 
     # Test parent
     expected_parent = [None, self.a, self.a, self.b, self.b, self.c, self.c, self.d]
     for node, expected in zip(nodes, expected_parent):
         actual = node.parent
         assert expected == actual, f"Expected parent {expected}, received {actual}"
@@ -972,29 +993,7 @@
         assert expected == actual, f"Expected right {expected}, received {actual}"
 
     # Test get_attr()
     expected_val = [1, 2, 3, 4, 5, 6, 7, 8]
     for node, expected in zip(nodes, expected_val):
         actual = node.get_attr("val")
         assert expected == actual, f"Expected attribute {expected}, received {actual}"
-
-
-def assert_binarytree_structure_root2(root):
-    a = root
-    b, c = a.children
-    d, e = b.children
-    f, g = c.children
-    h, _ = d.children
-
-    class Sample:
-        pass
-
-    self = Sample()
-    self.a = a
-    self.b = b
-    self.c = c
-    self.d = d
-    self.e = e
-    self.f = f
-    self.g = g
-    self.h = h
-    assert_binarytree_structure_self2(self)
```

### Comparing `bigtree-0.9.3/tests/node/test_dagnode.py` & `bigtree-0.9.4/tests/node/test_dagnode.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from bigtree.node.basenode import BaseNode
 from bigtree.node.dagnode import DAGNode
 from bigtree.node.node import Node
 from bigtree.utils.exceptions import LoopError, TreeError
 from bigtree.utils.iterators import dag_iterator
 from tests.conftest import assert_print_statement
+from tests.constants import Constants
 
 
 class DAGNode2(DAGNode):
     def _DAGNode__post_assign_parents(self, new_parents):
         if self.get_attr("val"):
             raise Exception("Custom error assigning parent")
         for parent in new_parents:
@@ -88,57 +89,23 @@
 
         assert_dag_structure_self(self)
         assert_dag_structure_root(self.a)
 
     def test_set_parent_error(self):
         with pytest.raises(ValueError) as exc_info:
             self.c.parent = self.a
-        assert str(exc_info.value).startswith("Attempting to set `parent` attribute")
+        assert str(exc_info.value) == Constants.ERROR_SET_PARENT_ATTR
 
         with pytest.raises(ValueError) as exc_info:
             self.c = DAGNode("b", parent=self.a)
-        assert str(exc_info.value).startswith("Attempting to set `parent` attribute")
+        assert str(exc_info.value) == Constants.ERROR_SET_PARENT_ATTR
 
         with pytest.raises(ValueError) as exc_info:
             self.c.parent
-        assert str(exc_info.value).startswith("Attempting to access `parent` attribute")
-
-    def test_set_parent_reassign(self):
-        self.a.children = [self.b, self.c]
-        self.d.children = [self.e]
-        self.b.parents = [self.d]
-        assert list(self.a.children) == [
-            self.b,
-            self.c,
-        ], f"Node a children, expected {[self.c]}, received {self.a.children}"
-        assert list(self.d.children) == [
-            self.e,
-            self.b,
-        ], f"Node d children, expected {[self.e, self.b]}, received {self.d.children}"
-        assert list(self.b.parents) == [
-            self.a,
-            self.d,
-        ], f"Node b parents, expected {[self.a, self.d]}, received {self.b.parents}"
-
-    def test_set_children_reassign(self):
-        self.a.children = [self.c]
-        self.b.parents = [self.a]
-        self.d.children = [self.e, self.b]
-        assert list(self.a.children) == [
-            self.c,
-            self.b,
-        ], f"Node a children, expected {[self.c]}, received {self.a.children}"
-        assert list(self.d.children) == [
-            self.e,
-            self.b,
-        ], f"Node d children, expected {[self.e, self.b]}, received {self.d.children}"
-        assert list(self.b.parents) == [
-            self.a,
-            self.d,
-        ], f"Node b parents, expected {[self.a, self.d]}, received {self.b.parents}"
+        assert str(exc_info.value) == Constants.ERROR_GET_PARENT_ATTR
 
     def test_set_parents(self):
         self.c.parents = [self.a, self.b]
         self.d.parents = [self.a, self.c]
         self.e.parents = [self.d]
         self.f.parents = [self.c, self.d]
         self.g.parents = [self.c]
@@ -181,28 +148,44 @@
         self.f = DAGNode(name="f", age=38, parents=[self.c, self.d])
         self.g = DAGNode(name="g", age=10, parents=[self.c])
         self.h = DAGNode(name="h", age=6, parents=[self.g])
 
         assert_dag_structure_self(self)
         assert_dag_structure_root(self.a)
 
-    def test_set_parents_none_parent(self):
+    def test_set_parents_none_parent_error(self):
         self.c.parents = [self.a]
-        with pytest.raises(TypeError):
+        with pytest.raises(TypeError) as exc_info:
             self.c.parents = None
+        assert str(exc_info.value).startswith(Constants.ERROR_DAGNODE_PARENT_TYPE)
+
+    def test_set_parent_reassign(self):
+        self.a.children = [self.b, self.c]
+        self.d.children = [self.e]
+        self.b.parents = [self.d]
+        assert list(self.a.children) == [
+            self.b,
+            self.c,
+        ], f"Node a children, expected {[self.c]}, received {self.a.children}"
+        assert list(self.d.children) == [
+            self.e,
+            self.b,
+        ], f"Node d children, expected {[self.e, self.b]}, received {self.d.children}"
+        assert list(self.b.parents) == [
+            self.a,
+            self.d,
+        ], f"Node b parents, expected {[self.a, self.d]}, received {self.b.parents}"
 
     def test_set_parent_duplicate(self):
-        # Set parent again
         self.c.parents = [self.a]
         self.c.parents = [self.a]
         assert list(self.a.children) == [self.c]
         assert list(self.c.parents) == [self.a]
 
     def test_set_parent_duplicate_constructor(self):
-        # Set parent again
         self.a = DAGNode(name="a", age=90)
         self.c = DAGNode(name="c", age=60, parents=[self.a])
         self.c.parents = [self.a]
         assert list(self.a.children) == [self.c]
         assert list(self.c.parents) == [self.a]
 
     def test_set_children(self):
@@ -227,25 +210,41 @@
         self.c.children = [self.d, self.f, self.g]
         self.b.children = [self.c]
         self.d.children = [self.e, self.f]
 
         assert_dag_structure_self(self)
         assert_dag_structure_root(self.a)
 
-    def test_set_children_none_children(self):
-        with pytest.raises(TypeError):
+    def test_set_children_none_children_error(self):
+        with pytest.raises(TypeError) as exc_info:
             self.g.children = None
+        assert str(exc_info.value).startswith(Constants.ERROR_CHILDREN_TYPE)
+
+    def test_set_children_reassign(self):
+        self.a.children = [self.c]
+        self.b.parents = [self.a]
+        self.d.children = [self.e, self.b]
+        assert list(self.a.children) == [
+            self.c,
+            self.b,
+        ], f"Node a children, expected {[self.c]}, received {self.a.children}"
+        assert list(self.d.children) == [
+            self.e,
+            self.b,
+        ], f"Node d children, expected {[self.e, self.b]}, received {self.d.children}"
+        assert list(self.b.parents) == [
+            self.a,
+            self.d,
+        ], f"Node b parents, expected {[self.a, self.d]}, received {self.b.parents}"
 
     def test_set_children_duplicate(self):
-        # Set child again
         self.a.children = [self.c]
         self.a.children = [self.c]
 
     def test_set_children_duplicate_constructor(self):
-        # Set child again
         self.a = DAGNode(children=[self.c])
         self.a.children = [self.c]
 
     def test_deep_copy_set_children(self):
         self.c.parents = [self.a, self.b]
         self.d.parents = [self.a, self.c]
         self.e.parents = [self.d]
@@ -269,77 +268,83 @@
         assert (
             len(list(a2.children)) == 2
         ), f"Expected 2 child, received {len(list(a2.children))}"
         assert (
             a2.children[0] == self.c or a2.children[1] == self.c
         ), "Shallow copy does not copy child nodes"
 
-    def test_error_set_parent_type_error(self):
-        # Error: wrong type
-        with pytest.raises(TypeError):
+    def test_set_parents_type_error(self):
+        with pytest.raises(TypeError) as exc_info:
             self.a.parents = 1
+        assert str(exc_info.value).startswith(Constants.ERROR_DAGNODE_PARENT_TYPE)
 
-        with pytest.raises(TypeError):
+        with pytest.raises(TypeError) as exc_info:
             self.a.parents = [1]
+        assert str(exc_info.value).startswith(Constants.ERROR_DAGNODE_TYPE)
 
         a = BaseNode()
-        with pytest.raises(TypeError):
+        with pytest.raises(TypeError) as exc_info:
             self.a.parents = [a]
+        assert str(exc_info.value).startswith(Constants.ERROR_DAGNODE_TYPE)
 
         a = Node("a")
-        with pytest.raises(TypeError):
+        with pytest.raises(TypeError) as exc_info:
             self.a.parents = [a]
+        assert str(exc_info.value).startswith(Constants.ERROR_DAGNODE_TYPE)
 
-    def test_error_set_parent_loop_error(self):
-        # Error: set self as parent
-        with pytest.raises(LoopError):
+    def test_set_parents_loop_error(self):
+        with pytest.raises(LoopError) as exc_info:
             self.a.parents = [self.a]
+        assert str(exc_info.value).startswith(Constants.ERROR_LOOP_PARENT)
 
-        # Error: set descendant as parent
-        with pytest.raises(LoopError):
+        with pytest.raises(LoopError) as exc_info:
             self.b.parents = [self.a]
             self.c.parents = [self.b]
             self.a.parents = [self.c]
+        assert str(exc_info.value).startswith(Constants.ERROR_LOOP_ANCESTOR)
 
-    def test_error_set_parent_exception(self):
-        # Error: duplicate child
-        with pytest.raises(TreeError):
+    def test_set_duplicate_parent_error(self):
+        with pytest.raises(TreeError) as exc_info:
             self.a.parents = [self.b, self.b]
+        assert str(exc_info.value).startswith(Constants.ERROR_SET_DUPLICATE_PARENT)
 
-    def test_error_set_children_type_error(self):
-        # Error: wrong type
-        with pytest.raises(TypeError):
+    def test_set_children_type_error(self):
+        with pytest.raises(TypeError) as exc_info:
             self.a.children = 1
+        assert str(exc_info.value).startswith(Constants.ERROR_CHILDREN_TYPE)
 
-        with pytest.raises(TypeError):
+        with pytest.raises(TypeError) as exc_info:
             self.a.children = [self.b, 1]
+        assert str(exc_info.value).startswith(Constants.ERROR_DAGNODE_TYPE)
 
         a = BaseNode()
-        with pytest.raises(TypeError):
+        with pytest.raises(TypeError) as exc_info:
             self.a.children = [a]
+        assert str(exc_info.value).startswith(Constants.ERROR_DAGNODE_TYPE)
 
         a = Node("a")
-        with pytest.raises(TypeError):
+        with pytest.raises(TypeError) as exc_info:
             self.a.children = [a]
+        assert str(exc_info.value).startswith(Constants.ERROR_DAGNODE_TYPE)
 
-    def test_error_set_children_loop_error(self):
-        # Error: set self as child
-        with pytest.raises(LoopError):
+    def test_set_children_loop_error(self):
+        with pytest.raises(LoopError) as exc_info:
             self.a.children = [self.b, self.a]
+        assert str(exc_info.value).startswith(Constants.ERROR_LOOP_CHILD)
 
-        # Error: set ancestor as child
-        with pytest.raises(LoopError):
+        with pytest.raises(LoopError) as exc_info:
             self.a.children = [self.b, self.c]
             self.c.children = [self.d, self.e, self.f]
             self.f.children = [self.a]
+        assert str(exc_info.value).startswith(Constants.ERROR_LOOP_DESCENDANT)
 
-    def test_error_set_children_exception(self):
-        # Error: duplicate child
-        with pytest.raises(TreeError):
+    def test_set_duplicate_children_error(self):
+        with pytest.raises(TreeError) as exc_info:
             self.a.children = [self.b, self.b]
+        assert str(exc_info.value).startswith(Constants.ERROR_SET_DUPLICATE_CHILD)
 
     @staticmethod
     def test_rollback_set_parents():
         a = DAGNode2(name="a", age=90)
         b = DAGNode2(name="b", age=65)
         c = DAGNode2(name="c", age=60)
         d = DAGNode2(name="d", age=40)
@@ -658,16 +663,71 @@
     def test_go_to_different_tree_error(self):
         a = DAGNode("a")
         with pytest.raises(TreeError) as exc_info:
             a.go_to(self.a)
         assert str(exc_info.value).startswith("It is not possible to go to")
 
 
+def assert_dag_structure_root(dag):
+    """Test tree structure"""
+    expected = [
+        ("a", "c"),
+        ("a", "d"),
+        ("b", "c"),
+        ("c", "d"),
+        ("c", "f"),
+        ("c", "g"),
+        ("d", "e"),
+        ("d", "f"),
+        ("g", "h"),
+    ]
+    actual = [
+        (parent.node_name, child.node_name) for parent, child in dag_iterator(dag)
+    ]
+    len_expected = 9
+    len_actual = len(actual)
+    for relation in actual:
+        if relation[1] in ["a", "b"]:
+            len_expected = 11
+            assert pd.isnull(relation[0]), f"Expected\n{relation}\nReceived\n{actual}"
+        else:
+            assert relation in expected, f"Expected\n{relation}\nReceived\n{actual}"
+    assert (
+        len_expected == len_actual
+    ), f"Expected\n{len_expected}\nReceived\n{len_actual}"
+
+
+def assert_dag_structure_root_attr(dag):
+    """Test tree structure with age attributes"""
+    expected_dict = {
+        "a": 90,
+        "b": 65,
+        "c": 60,
+        "d": 40,
+        "e": 35,
+        "f": 38,
+        "g": 10,
+        "h": 6,
+    }
+    for parent, child in dag_iterator(dag):
+        expected = expected_dict[parent.node_name]
+        actual = parent.age
+        assert (
+            expected == actual
+        ), f"For {parent}, expected\n{expected}\nReceived\n{actual}"
+
+        expected = expected_dict[child.node_name]
+        actual = child.age
+        assert (
+            expected == actual
+        ), f"For {child}, expected\n{expected}\nReceived\n{actual}"
+
+
 def assert_dag_structure_self(self):
-    """
+    """Test tree structure with self object
     Tree should have structure
     a >> c
     a >> d
     b >> c
     c >> d
     c >> f
     c >> g
@@ -837,58 +897,14 @@
         node.set_attrs({"index": expected})
         actual = node.get_attr("index")
         assert (
             actual == expected
         ), f"Node attribute should be {expected}, but it is {actual}"
 
 
-def assert_dag_structure_root(dag):
-    expected = [
-        ("a", "c"),
-        ("a", "d"),
-        ("b", "c"),
-        ("c", "d"),
-        ("c", "f"),
-        ("c", "g"),
-        ("d", "e"),
-        ("d", "f"),
-        ("g", "h"),
-    ]
-    actual = [
-        (parent.node_name, child.node_name) for parent, child in dag_iterator(dag)
-    ]
-    len_expected = 9
-    len_actual = len(actual)
-    for relation in actual:
-        if relation[1] in ["a", "b"]:
-            len_expected = 11
-            assert pd.isnull(relation[0]), f"Expected\n{relation}\nReceived\n{actual}"
-        else:
-            assert relation in expected, f"Expected\n{relation}\nReceived\n{actual}"
-    assert (
-        len_expected == len_actual
-    ), f"Expected\n{len_expected}\nReceived\n{len_actual}"
-
-
-def assert_dag_structure_attr_root(dag):
-    expected_dict = {
-        "a": 90,
-        "b": 65,
-        "c": 60,
-        "d": 40,
-        "e": 35,
-        "f": 38,
-        "g": 10,
-        "h": 6,
-    }
+def assert_dag_child_attr(dag, parent_name, child_name, child_attr, child_value):
+    """Test tree attributes"""
     for parent, child in dag_iterator(dag):
-        expected = expected_dict[parent.node_name]
-        actual = parent.age
-        assert (
-            expected == actual
-        ), f"For {parent}, expected\n{expected}\nReceived\n{actual}"
-
-        expected = expected_dict[child.node_name]
-        actual = child.age
-        assert (
-            expected == actual
-        ), f"For {child}, expected\n{expected}\nReceived\n{actual}"
+        if parent.name == parent_name and child.name == child_name:
+            expected = child_value
+            actual = child.get_attr(child_attr)
+            assert expected == actual, f"Expected {expected}, received {actual}"
```

### Comparing `bigtree-0.9.3/tests/node/test_node.py` & `bigtree-0.9.4/tests/node/test_node.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 
 import pytest
 
 from bigtree.node.node import Node
 from bigtree.utils.exceptions import LoopError, TreeError
 from bigtree.utils.iterators import preorder_iter
 from tests.conftest import assert_print_statement
+from tests.constants import Constants
 from tests.node.test_basenode import (
+    assert_tree_structure_basenode_root,
     assert_tree_structure_basenode_root_attr,
-    assert_tree_structure_basenode_root_generic,
     assert_tree_structure_basenode_self,
 )
 
 
 class TestNode(unittest.TestCase):
     def setUp(self):
         """
@@ -42,47 +43,48 @@
         self.c = None
         self.d = None
         self.e = None
         self.f = None
         self.g = None
         self.h = None
 
-    def test_empty_node_name(self):
-        with pytest.raises(TreeError):
+    def test_empty_node_name_error(self):
+        with pytest.raises(TreeError) as exc_info:
             Node()
+        assert str(exc_info.value) == Constants.ERROR_NODE_NAME
 
     def test_set_parent(self):
         self.b.parent = self.a
         self.c.parent = self.a
         self.d.parent = self.b
         self.e.parent = self.b
         self.f.parent = self.c
         self.g.parent = self.e
         self.h.parent = self.e
 
-        assert_tree_structure_basenode_root_generic(self.a)
+        assert_tree_structure_basenode_root(self.a)
         assert_tree_structure_basenode_root_attr(self.a)
         assert_tree_structure_basenode_self(self)
-        assert_tree_structure_node_root_generic(self.a)
+        assert_tree_structure_node_root(self.a)
         assert_tree_structure_node_self(self)
 
     def test_set_parent_constructor(self):
         self.a = Node(name="a", age=90)
         self.b = Node(name="b", age=65, parent=self.a)
         self.c = Node(name="c", age=60, parent=self.a)
         self.d = Node(name="d", age=40, parent=self.b)
         self.e = Node(name="e", age=35, parent=self.b)
         self.f = Node(name="f", age=38, parent=self.c)
         self.g = Node(name="g", age=10, parent=self.e)
         self.h = Node(name="h", age=6, parent=self.e)
 
-        assert_tree_structure_basenode_root_generic(self.a)
+        assert_tree_structure_basenode_root(self.a)
         assert_tree_structure_basenode_root_attr(self.a)
         assert_tree_structure_basenode_self(self)
-        assert_tree_structure_node_root_generic(self.a)
+        assert_tree_structure_node_root(self.a)
         assert_tree_structure_node_self(self)
 
     def test_set_parent_duplicate(self):
         # Set parent again
         self.b.parent = self.a
         self.b.parent = self.a
         assert list(self.a.children) == [self.b]
@@ -92,184 +94,186 @@
         # Set parent again
         self.a = Node(name="a", age=90)
         self.b = Node(name="b", age=65, parent=self.a)
         self.b.parent = self.a
         assert list(self.a.children) == [self.b]
         assert self.b.parent == self.a
 
-    def test_set_parent_sep_different_error_message(self):
+    def test_set_parent_sep_different_error(self):
         b = Node("b", sep="\\")
         self.b.parent = self.a
         with pytest.raises(TreeError) as exc_info:
             b.parent = self.a
         assert (
             str(exc_info.value)
-            == "Error: Duplicate node with same path\nThere exist a node with same path /a/b"
+            == f"{Constants.ERROR_SAME_PATH}\nThere exist a node with same path /a/b"
         )
 
     def test_set_parent_sep_root(self):
         self.b.parent = self.a
         self.c.parent = self.a
         self.d.parent = self.b
         self.e.parent = self.b
         self.f.parent = self.c
         self.g.parent = self.e
         self.h.parent = self.e
         self.a.sep = "\\"
 
-        assert_tree_structure_basenode_root_generic(self.a)
+        assert_tree_structure_basenode_root(self.a)
         assert_tree_structure_basenode_root_attr(self.a)
         assert_tree_structure_basenode_self(self)
         assert_tree_structure_node_self_sep(self)
 
     def test_set_parent_sep_child(self):
         self.b.parent = self.a
         self.c.parent = self.a
         self.d.parent = self.b
         self.e.parent = self.b
         self.f.parent = self.c
         self.g.parent = self.e
         self.h.parent = self.e
         self.h.sep = "\\"
 
-        assert_tree_structure_basenode_root_generic(self.a)
+        assert_tree_structure_basenode_root(self.a)
         assert_tree_structure_basenode_root_attr(self.a)
         assert_tree_structure_basenode_self(self)
         assert_tree_structure_node_self_sep(self)
 
     def test_set_children(self):
         self.a.children = [self.b, self.c]
         self.b.children = [self.d, self.e]
         self.c.children = [self.f]
         self.e.children = [self.g, self.h]
 
-        assert_tree_structure_basenode_root_generic(self.a)
+        assert_tree_structure_basenode_root(self.a)
         assert_tree_structure_basenode_root_attr(self.a)
         assert_tree_structure_basenode_self(self)
-        assert_tree_structure_node_root_generic(self.a)
+        assert_tree_structure_node_root(self.a)
         assert_tree_structure_node_self(self)
 
     def test_set_children_constructor(self):
         self.h = Node(name="h", age=6)
         self.g = Node(name="g", age=10)
         self.f = Node(name="f", age=38)
         self.e = Node(name="e", age=35, children=[self.g, self.h])
         self.d = Node(name="d", age=40)
         self.c = Node(name="c", age=60, children=[self.f])
         self.b = Node(name="b", age=65, children=[self.d, self.e])
         self.a = Node(name="a", age=90, children=[self.b, self.c])
 
-        assert_tree_structure_basenode_root_generic(self.a)
+        assert_tree_structure_basenode_root(self.a)
         assert_tree_structure_basenode_root_attr(self.a)
         assert_tree_structure_basenode_self(self)
-        assert_tree_structure_node_root_generic(self.a)
+        assert_tree_structure_node_root(self.a)
         assert_tree_structure_node_self(self)
 
     def test_set_children_duplicate(self):
-        # Set child again
         self.a.children = [self.b]
         self.a.children = [self.b]
 
     def test_set_children_duplicate_constructor(self):
-        # Set child again
         self.a = Node("a", children=[self.b])
         self.a.children = [self.b]
 
-    def test_children_sep_different_error_message(self):
+    def test_set_children_sep_different_error(self):
         b = Node("b", sep="\\")
         with pytest.raises(TreeError) as exc_info:
             self.a.children = [self.b, b]
         assert (
             str(exc_info.value)
-            == "Error: Duplicate node with same path\nAttempting to add nodes same path /a/b"
+            == f"{Constants.ERROR_SAME_PATH}\nAttempting to add nodes same path /a/b"
         )
 
-    def test_error_set_parent_same_path(self):
+    def test_set_parent_same_path_error(self):
         self.a = Node("a")
         self.b = Node("b", parent=self.a)
         self.c = Node("b")
-        with pytest.raises(TreeError):
+        with pytest.raises(TreeError) as exc_info:
             self.c.parent = self.a
+        assert str(exc_info.value).startswith(Constants.ERROR_SAME_PATH)
 
-    def test_error_set_parent_constructor_same_path(self):
+    def test_set_parent_constructor_same_path_error(self):
         self.a = Node("a")
         self.b = Node("b", parent=self.a)
-        with pytest.raises(TreeError):
+        with pytest.raises(TreeError) as exc_info:
             self.c = Node("b", parent=self.a)
+        assert str(exc_info.value).startswith(Constants.ERROR_SAME_PATH)
 
-    def test_error_set_children_same_path(self):
+    def test_set_children_same_path_error(self):
         self.a = Node("a")
         self.b = Node("b")
         self.c = Node("b")
-        with pytest.raises(TreeError):
+        with pytest.raises(TreeError) as exc_info:
             self.a.children = [self.b, self.c]
+        assert str(exc_info.value).startswith(Constants.ERROR_SAME_PATH)
 
-    def test_error_set_children_constructor_same_path(self):
+    def test_set_children_constructor_same_path_error(self):
         self.c = Node("b")
         self.b = Node("b")
-        with pytest.raises(TreeError):
+        with pytest.raises(TreeError) as exc_info:
             self.a = Node("a", children=[self.b, self.c])
+        assert str(exc_info.value).startswith(Constants.ERROR_SAME_PATH)
 
-    def test_error_set_children_multiple_same_path(self):
+    def test_set_children_multiple_same_path_error(self):
         self.a = Node("a")
         self.b = Node("b")
         self.c = Node("b")
         self.d = Node("c")
         self.e = Node("c")
         with pytest.raises(TreeError) as exc_info:
             self.a.children = [self.b, self.c, self.d, self.e]
         assert (
             str(exc_info.value)
-            == "Error: Duplicate node with same path\nAttempting to add nodes same path /a/b and /a/c"
+            == f"{Constants.ERROR_SAME_PATH}\nAttempting to add nodes same path /a/b and /a/c"
         )
 
-    def test_error_set_parent(self):
-        # Error: wrong type
-        with pytest.raises(TypeError):
+    def test_set_parent_error(self):
+        with pytest.raises(TypeError) as exc_info:
             self.a.parent = 1
+        assert str(exc_info.value).startswith(Constants.ERROR_BASENODE_PARENT_TYPE)
 
-        # Error: set self as parent
-        with pytest.raises(LoopError):
+        with pytest.raises(LoopError) as exc_info:
             self.a.parent = self.a
+        assert str(exc_info.value) == Constants.ERROR_LOOP_PARENT
 
-        # Error: set descendant as parent
-        with pytest.raises(LoopError):
+        with pytest.raises(LoopError) as exc_info:
             self.b.parent = self.a
             self.c.parent = self.b
             self.a.parent = self.c
+        assert str(exc_info.value) == Constants.ERROR_LOOP_ANCESTOR
 
-    def test_error_set_children(self):
-        # Error: wrong type
-        with pytest.raises(TypeError):
+    def test_set_children_error(self):
+        with pytest.raises(TypeError) as exc_info:
             self.a.children = [self.b, 1]
+        assert str(exc_info.value).startswith(Constants.ERROR_BASENODE_CHILDREN_TYPE)
 
-        # Error: set self as child
-        with pytest.raises(LoopError):
+        with pytest.raises(LoopError) as exc_info:
             self.a.children = [self.b, self.a]
+        assert str(exc_info.value) == Constants.ERROR_LOOP_CHILD
 
-        # Error: set ancestor as child
-        with pytest.raises(LoopError):
+        with pytest.raises(LoopError) as exc_info:
             self.a.children = [self.b, self.c]
             self.c.children = [self.d, self.e, self.f]
             self.f.children = [self.a]
+        assert str(exc_info.value) == Constants.ERROR_LOOP_DESCENDANT
 
-        # Error: duplicate child
-        with pytest.raises(TreeError):
+        with pytest.raises(TreeError) as exc_info:
             self.a.children = [self.b, self.b]
+        assert str(exc_info.value) == Constants.ERROR_SET_DUPLICATE_CHILD
 
     def test_go_to(self):
         self.a.children = [self.b, self.c]
         self.b.children = [self.d, self.e]
         self.c.children = [self.f]
         self.e.children = [self.g, self.h]
 
-        assert_tree_structure_basenode_root_generic(self.a)
+        assert_tree_structure_basenode_root(self.a)
         assert_tree_structure_basenode_root_attr(self.a)
         assert_tree_structure_basenode_self(self)
-        assert_tree_structure_node_root_generic(self.a)
+        assert_tree_structure_node_root(self.a)
         assert_tree_structure_node_self(self)
 
         expected_paths = [
             ["a", "b"],
             ["a", "b", "d"],
             ["a", "b", "e"],
             ["a", "b", "e", "g"],
@@ -323,15 +327,15 @@
     def test_go_to_different_tree_error(self):
         a = Node("a")
         with pytest.raises(TreeError) as exc_info:
             a.go_to(self.a)
         assert str(exc_info.value).startswith("Nodes are not from the same tree")
 
 
-def assert_tree_structure_node_root_generic(
+def assert_tree_structure_node_root(
     root,
     a="/a",
     b="/a/b",
     c="/a/c",
     d="/a/b/d",
     e="/a/b/e",
     f="/a/c/f",
```

### Comparing `bigtree-0.9.3/tests/tree/test_construct.py` & `bigtree-0.9.4/tests/tree/test_construct.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,20 +18,21 @@
     nested_dict_to_tree,
     str_to_tree,
 )
 from bigtree.tree.export import print_tree
 from bigtree.tree.search import find_name, find_names
 from bigtree.utils.exceptions import DuplicatedNodeError, TreeError
 from tests.conftest import assert_print_statement
+from tests.constants import Constants
 from tests.node.test_basenode import (
+    assert_tree_structure_basenode_root,
     assert_tree_structure_basenode_root_attr,
-    assert_tree_structure_basenode_root_generic,
 )
 from tests.node.test_node import (
-    assert_tree_structure_node_root_generic,
+    assert_tree_structure_node_root,
     assert_tree_structure_node_root_sep,
 )
 
 
 class NodeA(Node):
     pass
 
@@ -65,100 +66,116 @@
             "a/b/e",
             "a/c/f",
             "a/b/e/g",
             "a/b/e/h",
         ]
         for path in path_list:
             add_path_to_tree(self.root, path)
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
 
     def test_add_path_to_tree_leaves(self):
         for path in self.path_list:
             add_path_to_tree(self.root, path)
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
 
-    def test_add_path_to_tree_empty(self):
-        with pytest.raises(ValueError):
+    def test_add_path_to_tree_empty_error(self):
+        with pytest.raises(ValueError) as exc_info:
             add_path_to_tree(self.root, "")
+        assert str(exc_info.value) == Constants.ERROR_EMPTY_PATH
 
     def test_add_path_to_tree_sep_leading(self):
         path_list = ["/a/b/d", "/a/b/e", "/a/b/e/g", "/a/b/e/h", "/a/c/f"]
         for path in path_list:
             add_path_to_tree(self.root, path)
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
 
     def test_add_path_to_tree_sep_trailing(self):
         path_list = ["a/b/d/", "a/b/e/", "a/b/e/g/", "a/b/e/h/", "a/c/f/"]
         for path in path_list:
             add_path_to_tree(self.root, path)
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
 
-    def test_add_path_to_tree_sep_undefined(self):
+    def test_add_path_to_tree_sep_error(self):
         path_list = ["a\\b\\d", "a\\b\\e", "a\\b\\e\\g", "a\\b\\e\\h", "a\\c\\f"]
 
-        with pytest.raises(TreeError):
+        with pytest.raises(TreeError) as exc_info:
             for path in path_list:
                 add_path_to_tree(self.root, path)
+        assert str(exc_info.value).startswith(Constants.ERROR_DIFFERENT_ROOT)
 
     def test_add_path_to_tree_sep(self):
         path_list = ["a\\b\\d", "a\\b\\e", "a\\b\\e\\g", "a\\b\\e\\h", "a\\c\\f"]
 
         for path in path_list:
             add_path_to_tree(self.root, path, sep="\\")
-        assert_tree_structure_basenode_root_generic(self.root)
-        assert_tree_structure_node_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
+        assert_tree_structure_node_root(self.root)
 
     def test_add_path_to_tree_sep_tree(self):
         self.root.sep = "\\"
 
         for path in self.path_list:
             add_path_to_tree(self.root, path)
         assert_tree_structure_node_root_sep(self.root)
 
-    def test_add_path_to_tree_duplicate_node(self):
+    def test_add_path_to_tree_duplicate_node_error(self):
         path_list = [
             "a",
             "a/b",
             "a/c",
             "a/b/d",
             "a/b/e",
             "a/c/d",  # duplicate
             "a/b/e/g",
             "a/b/e/h",
         ]
 
-        with pytest.raises(DuplicatedNodeError):
+        with pytest.raises(DuplicatedNodeError) as exc_info:
             for path in path_list:
                 add_path_to_tree(self.root, path, duplicate_name_allowed=False)
+        assert str(exc_info.value).startswith("Node d already exists")
+
+    def test_add_path_to_tree_duplicate_node(self):
+        path_list = [
+            "a",
+            "a/b",
+            "a/c",
+            "a/b/d",
+            "a/b/e",
+            "a/c/d",  # duplicate
+            "a/b/e/g",
+            "a/b/e/h",
+        ]
 
         for path in path_list:
             add_path_to_tree(self.root, path)
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
 
     def test_add_path_to_tree_node_type(self):
         root = NodeA("a")
         for path in self.path_list:
             add_path_to_tree(root, path)
-        assert isinstance(root, NodeA), "Node type is not `NodeA`"
-        assert_tree_structure_basenode_root_generic(root)
+        assert isinstance(root, NodeA), Constants.ERROR_NODE_TYPE
+        assert_tree_structure_basenode_root(root)
 
-    def test_add_path_to_tree_different_root(self):
+    def test_add_path_to_tree_different_root_error(self):
         path_list = [
             "a",
             "a/b",
             "a/c",
             "a/b/d",
             "a/b/e",
             "a/c/f",
             "a/b/e/g",
             "b/b/e/h",  # different root
         ]
-        with pytest.raises(TreeError):
+        with pytest.raises(TreeError) as exc_info:
             for path in path_list:
                 add_path_to_tree(self.root, path, sep="-")
+        assert str(exc_info.value).startswith(Constants.ERROR_DIFFERENT_ROOT)
 
 
 class TestAddDictToTreeByPath(unittest.TestCase):
     def setUp(self):
         """
         Tree should have structure
         a (age=90)
@@ -184,84 +201,86 @@
 
     def tearDown(self):
         self.root = None
         self.paths = None
 
     def test_add_dict_to_tree_by_path(self):
         add_dict_to_tree_by_path(self.root, self.paths)
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
         assert_tree_structure_basenode_root_attr(self.root)
-        assert_tree_structure_node_root_generic(self.root)
+        assert_tree_structure_node_root(self.root)
 
-    def test_add_dict_to_tree_by_path_empty(self):
+    def test_add_dict_to_tree_by_path_empty_error(self):
         paths = {}
-        with pytest.raises(ValueError):
+        with pytest.raises(ValueError) as exc_info:
             add_dict_to_tree_by_path(self.root, paths)
+        assert str(exc_info.value).startswith(Constants.ERROR_EMPTY_DICT)
 
     def test_add_dict_to_tree_by_path_sep_leading(self):
         paths = {
             "/a": {"age": 90},
             "/a/b": {"age": 65},
             "/a/c": {"age": 60},
             "/a/b/d": {"age": 40},
             "/a/b/e": {"age": 35},
             "/a/c/f": {"age": 38},
             "/a/b/e/g": {"age": 10},
             "/a/b/e/h": {"age": 6},
         }
         add_dict_to_tree_by_path(self.root, paths)
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
         assert_tree_structure_basenode_root_attr(self.root)
-        assert_tree_structure_node_root_generic(self.root)
+        assert_tree_structure_node_root(self.root)
 
     def test_add_dict_to_tree_by_path_sep_trailing(self):
         paths = {
             "a/": {"age": 90},
             "a/b/": {"age": 65},
             "a/c/": {"age": 60},
             "a/b/d/": {"age": 40},
             "a/b/e/": {"age": 35},
             "a/c/f/": {"age": 38},
             "a/b/e/g/": {"age": 10},
             "a/b/e/h/": {"age": 6},
         }
         add_dict_to_tree_by_path(self.root, paths)
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
         assert_tree_structure_basenode_root_attr(self.root)
-        assert_tree_structure_node_root_generic(self.root)
+        assert_tree_structure_node_root(self.root)
 
-    def test_add_dict_to_tree_by_path_sep_undefined(self):
+    def test_add_dict_to_tree_by_path_sep_error(self):
         paths = {
             "a": {"age": 90},
             "a-b": {"age": 65},
             "a-c": {"age": 60},
             "a-b-d": {"age": 40},
             "a-b-e": {"age": 35},
             "a-c-f": {"age": 38},
             "a-b-e-g": {"age": 10},
             "a-b-e-h": {"age": 6},
         }
-        with pytest.raises(TreeError):
+        with pytest.raises(TreeError) as exc_info:
             add_dict_to_tree_by_path(self.root, paths)
+        assert str(exc_info.value).startswith(Constants.ERROR_DIFFERENT_ROOT)
 
     def test_add_dict_to_tree_by_path_sep(self):
         paths = {
             "a": {"age": 90},
             "a-b": {"age": 65},
             "a-c": {"age": 60},
             "a-b-d": {"age": 40},
             "a-b-e": {"age": 35},
             "a-c-f": {"age": 38},
             "a-b-e-g": {"age": 10},
             "a-b-e-h": {"age": 6},
         }
         add_dict_to_tree_by_path(self.root, paths, sep="-")
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
         assert_tree_structure_basenode_root_attr(self.root)
-        assert_tree_structure_node_root_generic(self.root)
+        assert_tree_structure_node_root(self.root)
 
     def test_add_dict_to_tree_by_path_sep_tree(self):
         self.root = Node("a", age=89)
         self.root.sep = "\\"
         paths = {
             "a": {"age": 90},
             "a\\b": {"age": 65},
@@ -269,56 +288,69 @@
             "a\\b\\d": {"age": 40},
             "a\\b\\e": {"age": 35},
             "a\\c\\f": {"age": 38},
             "a\\b\\e\\g": {"age": 10},
             "a\\b\\e\\h": {"age": 6},
         }
         add_dict_to_tree_by_path(self.root, paths, sep="\\")
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
         assert_tree_structure_basenode_root_attr(self.root)
         assert_tree_structure_node_root_sep(self.root)
 
-    def test_add_dict_to_tree_by_path_duplicate_node(self):
+    def test_add_dict_to_tree_by_path_duplicate_node_error(self):
         paths = {
             "a": {"age": 90},
             "a/b": {"age": 65},
             "a/c": {"age": 60},
             "a/b/d": {"age": 40},
             "a/b/e": {"age": 35},
             "a/c/d": {"age": 38},  # duplicate
             "a/b/e/g": {"age": 10},
             "a/b/e/h": {"age": 6},
         }
-        with pytest.raises(DuplicatedNodeError):
+        with pytest.raises(DuplicatedNodeError) as exc_info:
             add_dict_to_tree_by_path(self.root, paths, duplicate_name_allowed=False)
+        assert str(exc_info.value).startswith("Node d already exists")
 
+    def test_add_dict_to_tree_by_path_duplicate_node(self):
+        paths = {
+            "a": {"age": 90},
+            "a/b": {"age": 65},
+            "a/c": {"age": 60},
+            "a/b/d": {"age": 40},
+            "a/b/e": {"age": 35},
+            "a/c/d": {"age": 38},  # duplicate
+            "a/b/e/g": {"age": 10},
+            "a/b/e/h": {"age": 6},
+        }
         add_dict_to_tree_by_path(self.root, paths)
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
         assert_tree_structure_basenode_root_attr(self.root, f=("d", 38))
 
     def test_add_dict_to_tree_by_path_node_type(self):
         root = NodeA("a", age=1)
         add_dict_to_tree_by_path(root, self.paths)
-        assert isinstance(root, NodeA), "Node type is not `NodeA`"
-        assert_tree_structure_basenode_root_generic(root)
+        assert isinstance(root, NodeA), Constants.ERROR_NODE_TYPE
+        assert_tree_structure_basenode_root(root)
         assert_tree_structure_basenode_root_attr(root)
 
-    def test_add_dict_to_tree_by_path_different_root(self):
+    def test_add_dict_to_tree_by_path_different_root_error(self):
         paths = {
             "a": {"age": 90},
             "a/b": {"age": 65},
             "a/c": {"age": 60},
             "a/b/d": {"age": 40},
             "a/b/e": {"age": 35},
             "a/c/f": {"age": 38},
             "a/b/e/g": {"age": 10},
             "b/b/e/h": {"age": 6},  # different root
         }
-        with pytest.raises(TreeError):
+        with pytest.raises(TreeError) as exc_info:
             add_dict_to_tree_by_path(self.root, paths)
+        assert str(exc_info.value).startswith(Constants.ERROR_DIFFERENT_ROOT)
 
 
 class TestAddDictToTreeByName(unittest.TestCase):
     def setUp(self):
         """
         Tree should have structure
         a (age=90)
@@ -358,17 +390,17 @@
         self.f = None
         self.g = None
         self.h = None
         self.name_dict = None
 
     def test_add_dict_to_tree_by_name(self):
         root = add_dict_to_tree_by_name(self.root, self.name_dict)
-        assert_tree_structure_basenode_root_generic(root)
+        assert_tree_structure_basenode_root(root)
         assert_tree_structure_basenode_root_attr(root)
-        assert_tree_structure_node_root_generic(root)
+        assert_tree_structure_node_root(root)
 
     def test_add_dict_to_tree_by_name_different_dtype(self):
         name_dict = {
             "a": {"random": [1]},
             "b": {"random": [1, 2]},
             "c": {"random": [1, None]},
             "d": {"random": [None]},
@@ -380,58 +412,60 @@
         root = add_dict_to_tree_by_name(self.root, name_dict)
         nodes = ["a", "b", "c", "d", "e", "f", "g", "h"]
         expected_list = [[1], [1, 2], [1, None], [None], None, 0, -1, [-1]]
         for node_name, expected in zip(nodes, expected_list):
             actual = find_name(root, node_name).get_attr("random")
             assert expected == actual, f"Expected\n{expected}\nReceived\n{actual}"
 
-    def test_add_dict_to_tree_by_name_empty(self):
-        with pytest.raises(ValueError):
+    def test_add_dict_to_tree_by_name_empty_error(self):
+        with pytest.raises(ValueError) as exc_info:
             add_dict_to_tree_by_name(self.root, {})
-
-    def test_add_dict_to_tree_by_name_duplicate_in_tree(self):
-        hh = Node("h")
-        hh.parent = self.root
-        root = add_dict_to_tree_by_name(self.root, self.name_dict)
-        assert (
-            len(list(find_names(root, "h"))) == 2
-        ), "There is less node 'h' than expected"
-        for _node in list(find_names(root, "h")):
-            assert _node.age == 6
+        assert str(exc_info.value).startswith(Constants.ERROR_EMPTY_DICT)
 
     def test_add_dict_to_tree_by_name_inner_join_tree(self):
         dummy = Node("dummy")
         dummy.parent = self.b
         root = add_dict_to_tree_by_name(self.root, self.name_dict, join_type="inner")
-        assert_tree_structure_basenode_root_generic(root)
+        assert_tree_structure_basenode_root(root)
         assert_tree_structure_basenode_root_attr(root)
-        assert_tree_structure_node_root_generic(root)
+        assert_tree_structure_node_root(root)
 
     def test_add_dict_to_tree_by_name_inner_join_dict(self):
         self.name_dict["dummy"] = {"age": 100}
         root = add_dict_to_tree_by_name(self.root, self.name_dict, join_type="inner")
-        assert_tree_structure_basenode_root_generic(root)
+        assert_tree_structure_basenode_root(root)
         assert_tree_structure_basenode_root_attr(root)
-        assert_tree_structure_node_root_generic(root)
+        assert_tree_structure_node_root(root)
 
     def test_add_dict_to_tree_by_name_left_join(self):
         root = add_dict_to_tree_by_name(self.root, self.name_dict, join_type="left")
-        assert_tree_structure_basenode_root_generic(root)
+        assert_tree_structure_basenode_root(root)
         assert_tree_structure_basenode_root_attr(root)
-        assert_tree_structure_node_root_generic(root)
+        assert_tree_structure_node_root(root)
 
-    def test_add_dict_to_tree_by_name_invalid_join(self):
-        with pytest.raises(ValueError):
+    def test_add_dict_to_tree_by_name_invalid_join_error(self):
+        with pytest.raises(ValueError) as exc_info:
             add_dict_to_tree_by_name(self.root, self.name_dict, join_type="something")
+        assert str(exc_info.value).startswith(Constants.ERROR_JOIN_TYPE)
 
     def test_add_dict_to_tree_by_name_sep_tree(self):
         self.root.sep = "\\"
         root = add_dict_to_tree_by_name(self.root, self.name_dict)
         assert_tree_structure_node_root_sep(root)
 
+    def test_add_dict_to_tree_by_name_duplicate_name(self):
+        hh = Node("h", age=6)
+        hh.parent = self.root
+        root = add_dict_to_tree_by_name(self.root, self.name_dict)
+        assert (
+            len(list(find_names(root, "h"))) == 2
+        ), "There is less node 'h' than expected"
+        for _node in list(find_names(root, "h")):
+            assert _node.get_attr("age") == 6
+
     def test_add_dict_to_tree_by_name_node_type(self):
         root = NodeA("a", age=1)
         b = NodeA("b", parent=root, age=1)
         c = NodeA("c", parent=root, age=1)
         d = NodeA("d", age=1)
         e = NodeA("e")
         f = NodeA("f")
@@ -439,18 +473,18 @@
         h = NodeA("h")
         d.parent = b
         e.parent = b
         f.parent = c
         g.parent = e
         h.parent = e
         root = add_dict_to_tree_by_name(root, self.name_dict)
-        assert isinstance(root, NodeA), "Node type is not `NodeA`"
-        assert_tree_structure_basenode_root_generic(root)
+        assert isinstance(root, NodeA), Constants.ERROR_NODE_TYPE
+        assert_tree_structure_basenode_root(root)
         assert_tree_structure_basenode_root_attr(root)
-        assert_tree_structure_node_root_generic(root)
+        assert_tree_structure_node_root(root)
 
 
 class TestAddDataFrameToTreeByPath(unittest.TestCase):
     def setUp(self):
         """
         Tree should have structure
         a (age=90)
@@ -479,35 +513,53 @@
 
     def tearDown(self):
         self.root = None
         self.data = None
 
     def test_add_dataframe_to_tree_by_path(self):
         add_dataframe_to_tree_by_path(self.root, self.data)
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
         assert_tree_structure_basenode_root_attr(self.root)
-        assert_tree_structure_node_root_generic(self.root)
+        assert_tree_structure_node_root(self.root)
 
     def test_add_dataframe_to_tree_by_path_col_name(self):
         add_dataframe_to_tree_by_path(
             self.root, self.data, path_col="PATH", attribute_cols=["age"]
         )
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
+        assert_tree_structure_basenode_root_attr(self.root)
+        assert_tree_structure_node_root(self.root)
+
+    def test_add_dataframe_to_tree_by_path_col_name_reverse(self):
+        add_dataframe_to_tree_by_path(
+            self.root,
+            self.data[["age", "PATH"]],
+            path_col="PATH",
+            attribute_cols=["age"],
+        )
+        assert_tree_structure_basenode_root(self.root)
         assert_tree_structure_basenode_root_attr(self.root)
-        assert_tree_structure_node_root_generic(self.root)
+        assert_tree_structure_node_root(self.root)
+
+    def test_add_dataframe_to_tree_by_path_empty_error(self):
+        with pytest.raises(ValueError) as exc_info:
+            add_dataframe_to_tree_by_path(self.root, pd.DataFrame())
+        assert str(exc_info.value) == Constants.ERROR_EMPTY_COL
 
-    def test_add_dataframe_to_tree_by_path_empty_row(self):
+    def test_add_dataframe_to_tree_by_path_empty_row_error(self):
         data = pd.DataFrame(columns=["PATH", "age"])
-        with pytest.raises(ValueError):
+        with pytest.raises(ValueError) as exc_info:
             add_dataframe_to_tree_by_path(self.root, data)
+        assert str(exc_info.value) == Constants.ERROR_EMPTY_ROW
 
-    def test_add_dataframe_to_tree_by_path_empty_col(self):
+    def test_add_dataframe_to_tree_by_path_empty_col_error(self):
         data = pd.DataFrame()
-        with pytest.raises(ValueError):
+        with pytest.raises(ValueError) as exc_info:
             add_dataframe_to_tree_by_path(self.root, data)
+        assert str(exc_info.value) == Constants.ERROR_EMPTY_COL
 
     def test_add_dataframe_to_tree_by_path_no_attribute(self):
         data = pd.DataFrame(
             [
                 ["a"],
                 ["a/b"],
                 ["a/c"],
@@ -516,15 +568,15 @@
                 ["a/c/f"],
                 ["a/b/e/g"],
                 ["a/b/e/h"],
             ],
             columns=["PATH"],
         )
         add_dataframe_to_tree_by_path(self.root, data)
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
 
     def test_add_dataframe_to_tree_by_path_sep_leading(self):
         data = pd.DataFrame(
             [
                 ["/a", 90],
                 ["/a/b", 65],
                 ["/a/c", 60],
@@ -533,17 +585,17 @@
                 ["/a/c/f", 38],
                 ["/a/b/e/g", 10],
                 ["/a/b/e/h", 6],
             ],
             columns=["PATH", "age"],
         )
         add_dataframe_to_tree_by_path(self.root, data)
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
         assert_tree_structure_basenode_root_attr(self.root)
-        assert_tree_structure_node_root_generic(self.root)
+        assert_tree_structure_node_root(self.root)
 
     def test_add_dataframe_to_tree_by_path_sep_trailing(self):
         data = pd.DataFrame(
             [
                 ["a/", 90],
                 ["a/b/", 65],
                 ["a/c/", 60],
@@ -552,34 +604,35 @@
                 ["a/c/f/", 38],
                 ["a/b/e/g/", 10],
                 ["a/b/e/h/", 6],
             ],
             columns=["PATH", "age"],
         )
         add_dataframe_to_tree_by_path(self.root, data)
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
         assert_tree_structure_basenode_root_attr(self.root)
-        assert_tree_structure_node_root_generic(self.root)
+        assert_tree_structure_node_root(self.root)
 
-    def test_add_dataframe_to_tree_by_path_sep_undefined(self):
+    def test_add_dataframe_to_tree_by_path_sep_error(self):
         data = pd.DataFrame(
             [
                 ["a", 90],
                 ["a\\b", 65],
                 ["a\\c", 60],
                 ["a\\b\\d", 40],
                 ["a\\b\\e", 35],
                 ["a\\c\\f", 38],
                 ["a\\b\\e\\g", 10],
                 ["a\\b\\e\\h", 6],
             ],
             columns=["PATH", "age"],
         )
-        with pytest.raises(TreeError):
+        with pytest.raises(TreeError) as exc_info:
             add_dataframe_to_tree_by_path(self.root, data)
+        assert str(exc_info.value).startswith(Constants.ERROR_DIFFERENT_ROOT)
 
     def test_add_dataframe_to_tree_by_path_sep(self):
         data = pd.DataFrame(
             [
                 ["a", 90],
                 ["a\\b", 65],
                 ["a\\c", 60],
@@ -588,87 +641,122 @@
                 ["a\\c\\f", 38],
                 ["a\\b\\e\\g", 10],
                 ["a\\b\\e\\h", 6],
             ],
             columns=["PATH", "age"],
         )
         add_dataframe_to_tree_by_path(self.root, data, sep="\\")
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
         assert_tree_structure_basenode_root_attr(self.root)
-        assert_tree_structure_node_root_generic(self.root)
+        assert_tree_structure_node_root(self.root)
 
     def test_add_dataframe_to_tree_by_path_sep_tree(self):
         self.root.sep = "\\"
         add_dataframe_to_tree_by_path(self.root, self.data)
         assert_tree_structure_node_root_sep(self.root)
 
-    def test_add_dataframe_to_tree_by_path_node_type(self):
-        root = NodeA("a", age=1)
-        add_dataframe_to_tree_by_path(root, self.data)
-        assert isinstance(root, NodeA), "Node type is not `NodeA`"
-        assert_tree_structure_basenode_root_generic(root)
-        assert_tree_structure_basenode_root_attr(root)
-        assert_tree_structure_node_root_generic(root)
+    def test_add_dataframe_to_tree_by_path_duplicate_name_error(self):
+        data = pd.DataFrame(
+            [
+                ["a", 90],
+                ["a/b", 65],
+                ["a/c", 60],
+                ["a/b/d", 40],
+                ["a/b/e", 35],
+                ["a/c/d", 38],  # duplicate
+                ["a/b/e/g", 10],
+                ["a/b/e/h", 6],
+            ],
+            columns=["PATH", "age"],
+        )
+        with pytest.raises(DuplicatedNodeError) as exc_info:
+            add_dataframe_to_tree_by_path(self.root, data, duplicate_name_allowed=False)
+        assert str(exc_info.value).startswith("Node d already exists")
 
-    def test_add_dataframe_to_tree_by_path_different_root(self):
+    def test_add_dataframe_to_tree_by_path_duplicate_name(self):
         data = pd.DataFrame(
             [
                 ["a", 90],
                 ["a/b", 65],
                 ["a/c", 60],
                 ["a/b/d", 40],
                 ["a/b/e", 35],
-                ["a/c/f", 38],
+                ["a/c/d", 38],  # duplicate
                 ["a/b/e/g", 10],
-                ["b/b/e/h", 6],  # different root
+                ["a/b/e/h", 6],
             ],
             columns=["PATH", "age"],
         )
-        with pytest.raises(TreeError):
-            add_dataframe_to_tree_by_path(self.root, data)
+        add_dataframe_to_tree_by_path(self.root, data)
+        assert_tree_structure_basenode_root(self.root)
 
-    def test_add_dataframe_to_tree_by_path_duplicate(self):
+    def test_add_dataframe_to_tree_by_path_duplicate_data_error(self):
         data = pd.DataFrame(
             [
                 ["a", 90],
                 ["a/b", 65],
                 ["a/c", 60],
                 ["a/b/d", 40],
                 ["a/b/e", 35],
-                ["a/c/f", 38],
+                ["a/c/d", 38],  # duplicate
+                ["a/c/d", 35],  # duplicate
                 ["a/b/e/g", 10],
                 ["a/b/e/h", 6],
-                ["a/b/e/h", 7],  # duplicate
             ],
             columns=["PATH", "age"],
         )
-        with pytest.raises(ValueError):
+        with pytest.raises(ValueError) as exc_info:
             add_dataframe_to_tree_by_path(self.root, data)
+        assert str(exc_info.value).startswith(Constants.ERROR_DUPLICATE_PATH)
 
-    def test_add_dataframe_to_tree_by_path_duplicate_node(self):
+    def test_add_dataframe_to_tree_by_path_duplicate_data(self):
         data = pd.DataFrame(
             [
                 ["a", 90],
                 ["a/b", 65],
                 ["a/c", 60],
                 ["a/b/d", 40],
                 ["a/b/e", 35],
                 ["a/c/d", 38],  # duplicate
+                ["a/c/d", 38],  # duplicate
                 ["a/b/e/g", 10],
                 ["a/b/e/h", 6],
             ],
             columns=["PATH", "age"],
         )
-        with pytest.raises(DuplicatedNodeError):
-            add_dataframe_to_tree_by_path(self.root, data, duplicate_name_allowed=False)
-
         add_dataframe_to_tree_by_path(self.root, data)
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
         assert_tree_structure_basenode_root_attr(self.root, f=("d", 38))
-        assert_tree_structure_node_root_generic(self.root, f="/a/c/d")
+        assert_tree_structure_node_root(self.root, f="/a/c/d")
+
+    def test_add_dataframe_to_tree_by_path_node_type(self):
+        root = NodeA("a", age=1)
+        add_dataframe_to_tree_by_path(root, self.data)
+        assert isinstance(root, NodeA), Constants.ERROR_NODE_TYPE
+        assert_tree_structure_basenode_root(root)
+        assert_tree_structure_basenode_root_attr(root)
+        assert_tree_structure_node_root(root)
+
+    def test_add_dataframe_to_tree_by_path_different_root_error(self):
+        data = pd.DataFrame(
+            [
+                ["a", 90],
+                ["a/b", 65],
+                ["a/c", 60],
+                ["a/b/d", 40],
+                ["a/b/e", 35],
+                ["a/c/f", 38],
+                ["a/b/e/g", 10],
+                ["b/b/e/h", 6],  # different root
+            ],
+            columns=["PATH", "age"],
+        )
+        with pytest.raises(TreeError) as exc_info:
+            add_dataframe_to_tree_by_path(self.root, data)
+        assert str(exc_info.value).startswith(Constants.ERROR_DIFFERENT_ROOT)
 
 
 class TestAddDataFrameToTreeByName(unittest.TestCase):
     def setUp(self):
         """
         Tree should have structure
         a (age=90)
@@ -711,52 +799,61 @@
         self.f = None
         self.g = None
         self.h = None
         self.data = None
 
     def test_add_dataframe_to_tree_by_name(self):
         root = add_dataframe_to_tree_by_name(self.root, self.data)
-        assert_tree_structure_basenode_root_generic(root)
+        assert_tree_structure_basenode_root(root)
         assert_tree_structure_basenode_root_attr(root)
-        assert_tree_structure_node_root_generic(root)
-
-    def test_add_dataframe_to_tree_by_name_duplicate_in_tree(self):
-        hh = Node("h")
-        hh.parent = self.root
-        root = add_dataframe_to_tree_by_name(self.root, self.data)
-        assert (
-            len(list(find_names(root, "h"))) == 2
-        ), "There is less node 'h' than expected"
-        for _node in list(find_names(root, "h")):
-            assert _node.age == 6
+        assert_tree_structure_node_root(root)
 
     def test_add_dataframe_to_tree_by_name_col_name(self):
         root = add_dataframe_to_tree_by_name(
             self.root, self.data, name_col="NAME", attribute_cols=["age"]
         )
-        assert_tree_structure_basenode_root_generic(root)
+        assert_tree_structure_basenode_root(root)
+        assert_tree_structure_basenode_root_attr(root)
+        assert_tree_structure_node_root(root)
+
+    def test_add_dataframe_to_tree_by_name_col_name_reverse(self):
+        root = add_dataframe_to_tree_by_name(
+            self.root,
+            self.data[["age", "NAME"]],
+            name_col="NAME",
+            attribute_cols=["age"],
+        )
+        assert_tree_structure_basenode_root(root)
         assert_tree_structure_basenode_root_attr(root)
-        assert_tree_structure_node_root_generic(root)
+        assert_tree_structure_node_root(root)
 
-    def test_add_dataframe_to_tree_by_name_empty(self):
-        with pytest.raises(ValueError):
+    def test_add_dataframe_to_tree_by_name_empty_error(self):
+        with pytest.raises(ValueError) as exc_info:
             add_dataframe_to_tree_by_name(self.root, pd.DataFrame())
+        assert str(exc_info.value) == Constants.ERROR_EMPTY_COL
 
-    def test_add_dataframe_to_tree_by_name_empty_row(self):
+    def test_add_dataframe_to_tree_by_name_empty_row_error(self):
         data = pd.DataFrame(columns=["NAME", "age"])
-        with pytest.raises(ValueError):
-            add_dataframe_to_tree_by_name(self.root, data, join_type="inner")
+        with pytest.raises(ValueError) as exc_info:
+            add_dataframe_to_tree_by_name(self.root, data)
+        assert str(exc_info.value) == Constants.ERROR_EMPTY_ROW
+
+    def test_add_dataframe_to_tree_by_name_empty_col_error(self):
+        data = pd.DataFrame()
+        with pytest.raises(ValueError) as exc_info:
+            add_dataframe_to_tree_by_name(self.root, data)
+        assert str(exc_info.value) == Constants.ERROR_EMPTY_COL
 
     def test_add_dataframe_to_tree_by_name_inner_join_tree(self):
         dummy = Node("dummy")
         dummy.parent = self.b
         root = add_dataframe_to_tree_by_name(self.root, self.data, join_type="inner")
-        assert_tree_structure_basenode_root_generic(root)
+        assert_tree_structure_basenode_root(root)
         assert_tree_structure_basenode_root_attr(root)
-        assert_tree_structure_node_root_generic(root)
+        assert_tree_structure_node_root(root)
 
     def test_add_dataframe_to_tree_by_name_inner_join_data(self):
         data = pd.DataFrame(
             [
                 ["a", 90],
                 ["b", 65],
                 ["c", 60],
@@ -766,87 +863,81 @@
                 ["g", 10],
                 ["h", 6],
                 ["dummy", 100],
             ],
             columns=["NAME", "age"],
         )
         root = add_dataframe_to_tree_by_name(self.root, data, join_type="inner")
-        assert_tree_structure_basenode_root_generic(root)
+        assert_tree_structure_basenode_root(root)
         assert_tree_structure_basenode_root_attr(root)
-        assert_tree_structure_node_root_generic(root)
+        assert_tree_structure_node_root(root)
 
     def test_add_dataframe_to_tree_by_name_left_join(self):
         root = add_dataframe_to_tree_by_name(self.root, self.data, join_type="left")
-        assert_tree_structure_basenode_root_generic(root)
+        assert_tree_structure_basenode_root(root)
         assert_tree_structure_basenode_root_attr(root)
-        assert_tree_structure_node_root_generic(root)
+        assert_tree_structure_node_root(root)
 
-    def test_add_dataframe_to_tree_by_name_invalid_join(self):
-        with pytest.raises(ValueError):
+    def test_add_dataframe_to_tree_by_name_invalid_join_error(self):
+        with pytest.raises(ValueError) as exc_info:
             add_dataframe_to_tree_by_name(self.root, self.data, join_type="something")
+        assert str(exc_info.value).startswith(Constants.ERROR_JOIN_TYPE)
 
     def test_add_dataframe_to_tree_by_name_sep_tree(self):
         self.root.sep = "\\"
         root = add_dataframe_to_tree_by_name(self.root, self.data)
         assert_tree_structure_node_root_sep(root)
 
-    def test_add_dataframe_to_tree_by_name_node_type(self):
-        root = NodeA("a", age=1)
-        b = NodeA("b", parent=root, age=1)
-        c = NodeA("c", parent=root, age=1)
-        d = NodeA("d", age=1)
-        e = NodeA("e")
-        f = NodeA("f")
-        g = NodeA("g")
-        h = NodeA("h")
-        d.parent = b
-        e.parent = b
-        f.parent = c
-        g.parent = e
-        h.parent = e
-        root = add_dataframe_to_tree_by_name(root, self.data)
-        assert isinstance(root, NodeA), "Node type is not `NodeA`"
-        assert_tree_structure_basenode_root_generic(root)
-        assert_tree_structure_basenode_root_attr(root)
-        assert_tree_structure_node_root_generic(root)
+    def test_add_dataframe_to_tree_by_name_duplicate_name(self):
+        hh = Node("h")
+        hh.parent = self.root
+        root = add_dataframe_to_tree_by_name(self.root, self.data)
+        assert (
+            len(list(find_names(root, "h"))) == 2
+        ), "There is less node 'h' than expected"
+        for _node in list(find_names(root, "h")):
+            assert _node.get_attr("age") == 6
 
-    def test_add_dataframe_to_tree_by_name_duplicate(self):
+    def test_add_dataframe_to_tree_by_name_duplicate_data_error(self):
         data = pd.DataFrame(
             [
                 ["a", 90],
                 ["b", 65],
                 ["c", 60],
                 ["d", 40],
                 ["e", 35],
                 ["f", 38],
                 ["g", 10],
                 ["g", 6],  # duplicate
             ],
             columns=["NAME", "age"],
         )
-        with pytest.raises(ValueError):
+        with pytest.raises(ValueError) as exc_info:
             add_dataframe_to_tree_by_name(self.root, data)
+        assert str(exc_info.value).startswith(Constants.ERROR_DUPLICATE_NAME)
 
-    def test_add_dataframe_to_tree_by_name_duplicate_node(self):
-        root = Node("a", age=1)
-        b = Node("b", parent=root, age=1)
-        c = Node("c", parent=root, age=1)
-        d = Node("d", age=1)
-        e = Node("e")
-        f = Node("f")
-        g = Node("g")
-        h = Node("f")  # duplicate node
+    def test_add_dataframe_to_tree_by_name_node_type(self):
+        root = NodeA("a", age=1)
+        b = NodeA("b", parent=root, age=1)
+        c = NodeA("c", parent=root, age=1)
+        d = NodeA("d", age=1)
+        e = NodeA("e")
+        f = NodeA("f")
+        g = NodeA("g")
+        h = NodeA("h")
         d.parent = b
         e.parent = b
         f.parent = c
         g.parent = e
         h.parent = e
         root = add_dataframe_to_tree_by_name(root, self.data)
-        assert_tree_structure_basenode_root_generic(root)
-        assert_tree_structure_basenode_root_attr(root, h=("f", 38))
+        assert isinstance(root, NodeA), Constants.ERROR_NODE_TYPE
+        assert_tree_structure_basenode_root(root)
+        assert_tree_structure_basenode_root_attr(root)
+        assert_tree_structure_node_root(root)
 
 
 class TestStrToTree(unittest.TestCase):
     def setUp(self):
         """
         Tree should have structure
         a
@@ -858,64 +949,54 @@
         +-- c
             +-- f
         """
         self.tree_str = "a\n├── b\n│   ├── d\n│   └── e\n│       ├── g\n│       └── h\n└── c\n    └── f"
 
     def test_str_to_tree(self):
         root = str_to_tree(self.tree_str)
-        assert_tree_structure_basenode_root_generic(root)
-        assert_tree_structure_node_root_generic(root)
+        assert_tree_structure_basenode_root(root)
+        assert_tree_structure_node_root(root)
 
     def test_str_to_tree_with_prefix(self):
         root = str_to_tree(self.tree_str, tree_prefix_list=["─"])
-        assert_tree_structure_basenode_root_generic(root)
-        assert_tree_structure_node_root_generic(root)
+        assert_tree_structure_basenode_root(root)
+        assert_tree_structure_node_root(root)
 
     def test_str_to_tree_with_multiple_prefix(self):
         root = str_to_tree(self.tree_str, tree_prefix_list=["├──", "└──"])
-        assert_tree_structure_basenode_root_generic(root)
-        assert_tree_structure_node_root_generic(root)
+        assert_tree_structure_basenode_root(root)
+        assert_tree_structure_node_root(root)
 
     def test_ascii_character_error(self):
         tree_str = "a\n|-- b\n|   |-- d\n|   +-- e\n|       |-- g\n|       +-- h\n+-- c\n    +-- f"
         with pytest.raises(ValueError) as exc_info:
             str_to_tree(tree_str)
-        assert str(exc_info.value).startswith(
-            "Invalid prefix, prefix should be unicode character or whitespace, otherwise specify one or more prefixes"
-        )
+        assert str(exc_info.value).startswith(Constants.ERROR_PREFIX)
 
     def test_ascii_character_with_prefix(self):
         tree_str = "a\n|-- b\n|   |-- d\n|   +-- e\n|       |-- g\n|       +-- h\n+-- c\n    +-- f"
         root = str_to_tree(tree_str, tree_prefix_list=["-"])
-        assert_tree_structure_basenode_root_generic(root)
-        assert_tree_structure_node_root_generic(root)
+        assert_tree_structure_basenode_root(root)
+        assert_tree_structure_node_root(root)
 
-    def test_empty_string(self):
+    def test_empty_string_error(self):
         with pytest.raises(ValueError) as exc_info:
             str_to_tree("")
-        assert (
-            str(exc_info.value)
-            == "Tree string does not contain any data, check `tree_string`"
-        )
+        assert str(exc_info.value) == Constants.ERROR_EMPTY_STRING
 
-    def test_empty_newline_string(self):
+    def test_empty_newline_string_error(self):
         with pytest.raises(ValueError) as exc_info:
             str_to_tree("\n\n")
-        assert (
-            str(exc_info.value)
-            == "Tree string does not contain any data, check `tree_string`"
-        )
+        assert str(exc_info.value) == Constants.ERROR_EMPTY_STRING
 
-    def test_unequal_prefix_length(self):
+    def test_unequal_prefix_length_error(self):
         tree_str = "a\n├── b\n│  ├── d\n│   └── e\n│       ├── g\n│       └── h\n└── c\n    └── f"
         with pytest.raises(ValueError) as exc_info:
             str_to_tree(tree_str)
-        assert str(exc_info.value).startswith(
-            "Tree string have different prefix length, check branch"
-        )
+        assert str(exc_info.value).startswith(Constants.ERROR_PREFIX_LENGTH)
 
 
 class TestListToTree(unittest.TestCase):
     def setUp(self):
         """
         Tree should have structure
         a
@@ -941,86 +1022,101 @@
 
     def tearDown(self):
         self.path_list = None
         self.path_list_full = None
 
     def test_list_to_tree(self):
         root = list_to_tree(self.path_list_full)
-        assert_tree_structure_basenode_root_generic(root)
-        assert_tree_structure_node_root_generic(root)
+        assert_tree_structure_basenode_root(root)
+        assert_tree_structure_node_root(root)
 
     def test_list_to_tree_leaves(self):
         root = list_to_tree(self.path_list)
-        assert_tree_structure_basenode_root_generic(root)
-        assert_tree_structure_node_root_generic(root)
+        assert_tree_structure_basenode_root(root)
+        assert_tree_structure_node_root(root)
 
-    def test_list_to_tree_empty(self):
-        with pytest.raises(ValueError):
+    def test_list_to_tree_empty_error(self):
+        with pytest.raises(ValueError) as exc_info:
             list_to_tree("")
+        assert str(exc_info.value).startswith(Constants.ERROR_EMPTY_LIST)
 
     def test_list_to_tree_sep_leading(self):
         path_list = ["/a/b/d", "/a/b/e", "/a/b/e/g", "/a/b/e/h", "/a/c/f"]
         root = list_to_tree(path_list)
-        assert_tree_structure_basenode_root_generic(root)
-        assert_tree_structure_node_root_generic(root)
+        assert_tree_structure_basenode_root(root)
+        assert_tree_structure_node_root(root)
 
     def test_list_to_tree_sep_trailing(self):
         path_list = ["a/b/d/", "a/b/e/", "a/b/e/g/", "a/b/e/h/", "a/c/f/"]
         root = list_to_tree(path_list)
-        assert_tree_structure_basenode_root_generic(root)
-        assert_tree_structure_node_root_generic(root)
+        assert_tree_structure_basenode_root(root)
+        assert_tree_structure_node_root(root)
 
-    def test_list_to_tree_sep_undefined(self):
+    def test_list_to_tree_sep_error(self):
         path_list = ["a\\b\\d", "a\\b\\e", "a\\b\\e\\g", "a\\b\\e\\h", "a\\c\\f"]
-        with pytest.raises(TreeError):
+        with pytest.raises(TreeError) as exc_info:
             list_to_tree(path_list)
+        assert str(exc_info.value).startswith(Constants.ERROR_DIFFERENT_ROOT)
 
     def test_list_to_tree_sep(self):
         path_list = ["a\\b\\d", "a\\b\\e", "a\\b\\e\\g", "a\\b\\e\\h", "a\\c\\f"]
         root = list_to_tree(path_list, sep="\\")
-        assert_tree_structure_basenode_root_generic(root)
+        assert_tree_structure_basenode_root(root)
         assert_tree_structure_node_root_sep(root)
 
-    def test_list_to_tree_duplicate_node(self):
+    def test_list_to_tree_duplicate_node_error(self):
         path_list = [
             "a",
             "a/b",
             "a/c",
             "a/b/d",
             "a/b/e",
             "a/c/d",  # duplicate
             "a/b/e/g",
             "a/b/e/h",
         ]
-        with pytest.raises(DuplicatedNodeError):
+        with pytest.raises(DuplicatedNodeError) as exc_info:
             list_to_tree(path_list, duplicate_name_allowed=False)
+        assert str(exc_info.value).startswith("Node d already exists")
 
+    def test_list_to_tree_duplicate_node(self):
+        path_list = [
+            "a",
+            "a/b",
+            "a/c",
+            "a/b/d",
+            "a/b/e",
+            "a/c/d",  # duplicate
+            "a/b/e/g",
+            "a/b/e/h",
+        ]
         root = list_to_tree(path_list)
-        assert_tree_structure_basenode_root_generic(root)
-        assert_tree_structure_node_root_generic(root, f="/a/c/d")
+        assert_tree_structure_basenode_root(root)
+        assert_tree_structure_node_root(root, f="/a/c/d")
 
     def test_list_to_tree_node_type(self):
         root = list_to_tree(self.path_list, node_type=NodeA)
-        assert isinstance(root, NodeA), "Node type is not `NodeA`"
-        assert_tree_structure_basenode_root_generic(root)
-        assert_tree_structure_node_root_generic(root)
+        assert isinstance(root, NodeA), Constants.ERROR_NODE_TYPE
+        assert_tree_structure_basenode_root(root)
+        assert_tree_structure_node_root(root)
 
-    def test_list_to_tree_different_root(self):
+    def test_list_to_tree_different_root_error(self):
         path_list = [
             "a",
             "a/b",
             "a/c",
             "a/b/d",
             "a/b/e",
             "a/c/f",
             "a/b/e/g",
             "b/b/e/h",  # different root
         ]
-        with pytest.raises(TreeError):
+        with pytest.raises(TreeError) as exc_info:
             list_to_tree(path_list)
+        assert str(exc_info.value).startswith(Constants.ERROR_DIFFERENT_ROOT)
 
 
 class TestListToTreeByRelation(unittest.TestCase):
     def setUp(self):
         """
         Tree should have structure
         a
@@ -1062,21 +1158,26 @@
         ]
 
     def tearDown(self):
         self.relations = None
 
     def test_list_to_tree_by_relation(self):
         root = list_to_tree_by_relation(self.relations)
-        assert_tree_structure_basenode_root_generic(root)
-        assert_tree_structure_node_root_generic(root)
+        assert_tree_structure_basenode_root(root)
+        assert_tree_structure_node_root(root)
 
     def test_list_to_tree_by_relation_reverse(self):
         root = list_to_tree_by_relation(self.relations_reverse)
-        assert_tree_structure_basenode_root_generic(root)
-        assert_tree_structure_node_root_generic(root)
+        assert_tree_structure_basenode_root(root)
+        assert_tree_structure_node_root(root)
+
+    def test_list_to_tree_by_relation_empty_error(self):
+        with pytest.raises(ValueError) as exc_info:
+            list_to_tree_by_relation([])
+        assert str(exc_info.value).startswith(Constants.ERROR_EMPTY_LIST)
 
     @staticmethod
     def test_list_to_tree_by_relation_duplicate_leaf_node():
         relations = [
             ("a", "b"),
             ("a", "c"),
             ("b", "d"),
@@ -1086,30 +1187,58 @@
             ("e", "g"),
             ("e", "h"),
         ]
         root = list_to_tree_by_relation(relations)
         expected = """a\n├── b\n│   ├── d\n│   ├── e\n│   │   ├── g\n│   │   └── h\n│   └── h\n└── c\n    └── h\n"""
         assert_print_statement(print_tree, expected, tree=root, style="const")
 
+    @staticmethod
+    def test_list_to_tree_by_relation_duplicate_intermediate_node_error():
+        relations = [
+            ("a", "b"),
+            ("a", "c"),
+            ("b", "d"),
+            ("b", "e"),
+            ("c", "e"),
+            ("c", "f"),
+            ("e", "g"),  # duplicate parent
+            ("e", "h"),  # duplicate parent
+        ]
+        with pytest.raises(ValueError) as exc_info:
+            list_to_tree_by_relation(relations)
+        assert str(exc_info.value).startswith(Constants.ERROR_DUPLICATE_PARENT)
+
+    @staticmethod
+    def test_list_to_tree_by_relation_duplicate_intermediate_node():
+        relations = [
+            ("a", "b"),
+            ("a", "c"),
+            ("b", "d"),
+            ("b", "e"),
+            ("c", "e"),
+            ("c", "f"),
+            ("e", "g"),  # duplicate parent
+            ("e", "h"),  # duplicate parent
+        ]
+        root = list_to_tree_by_relation(relations, allow_duplicates=True)
+        expected = """a\n├── b\n│   ├── d\n│   └── e\n│       ├── g\n│       └── h\n└── c\n    ├── e\n    │   ├── g\n    │   └── h\n    └── f\n"""
+        assert_print_statement(print_tree, expected, tree=root)
+
     def test_list_to_tree_by_relation_empty_parent(self):
         self.relations.append((None, "a"))
         root = list_to_tree_by_relation(self.relations)
-        assert_tree_structure_basenode_root_generic(root)
-        assert_tree_structure_node_root_generic(root)
+        assert_tree_structure_basenode_root(root)
+        assert_tree_structure_node_root(root)
 
     @staticmethod
     def test_list_to_tree_by_relation_one_tuple():
         root = list_to_tree_by_relation([(None, "a")])
         assert root.max_depth == 1, "Max depth is wrong"
         assert root.node_name == "a", "Node name is wrong"
 
-    def test_list_to_tree_by_relation_empty(self):
-        with pytest.raises(ValueError):
-            list_to_tree_by_relation([])
-
     def test_list_to_tree_by_relation_switch_order(self):
         root = list_to_tree_by_relation(self.relations_switch)
         expected = """h\n├── g\n│   ├── e\n│   ├── d\n│   │   ├── b\n│   │   └── a\n│   └── a\n└── f\n    └── a\n"""
         assert_print_statement(print_tree, expected, root)
 
     def test_list_to_tree_by_relation_switch_order_reverse(self):
         root = list_to_tree_by_relation(self.relations_switch[::-1])
@@ -1142,130 +1271,146 @@
         }
 
     def tearDown(self):
         self.path_dict = None
 
     def test_dict_to_tree(self):
         root = dict_to_tree(self.path_dict)
-        assert_tree_structure_basenode_root_generic(root)
+        assert_tree_structure_basenode_root(root)
         assert_tree_structure_basenode_root_attr(root)
-        assert_tree_structure_node_root_generic(root)
+        assert_tree_structure_node_root(root)
 
-    def test_dict_to_tree_empty(self):
+    def test_dict_to_tree_empty_error(self):
         paths = {}
-        with pytest.raises(ValueError):
+        with pytest.raises(ValueError) as exc_info:
             dict_to_tree(paths)
+        assert str(exc_info.value).startswith(Constants.ERROR_EMPTY_DICT)
 
     @staticmethod
     def test_dict_to_tree_sep_leading():
         paths = {
             "/a": {"age": 90},
             "/a/b": {"age": 65},
             "/a/c": {"age": 60},
             "/a/b/d": {"age": 40},
             "/a/b/e": {"age": 35},
             "/a/c/f": {"age": 38},
             "/a/b/e/g": {"age": 10},
             "/a/b/e/h": {"age": 6},
         }
         root = dict_to_tree(paths)
-        assert_tree_structure_basenode_root_generic(root)
+        assert_tree_structure_basenode_root(root)
         assert_tree_structure_basenode_root_attr(root)
-        assert_tree_structure_node_root_generic(root)
+        assert_tree_structure_node_root(root)
 
     @staticmethod
     def test_dict_to_tree_sep_trailing():
         paths = {
             "a/": {"age": 90},
             "a/b/": {"age": 65},
             "a/c/": {"age": 60},
             "a/b/d/": {"age": 40},
             "a/b/e/": {"age": 35},
             "a/c/f/": {"age": 38},
             "a/b/e/g/": {"age": 10},
             "a/b/e/h/": {"age": 6},
         }
         root = dict_to_tree(paths)
-        assert_tree_structure_basenode_root_generic(root)
+        assert_tree_structure_basenode_root(root)
         assert_tree_structure_basenode_root_attr(root)
-        assert_tree_structure_node_root_generic(root)
+        assert_tree_structure_node_root(root)
 
     @staticmethod
-    def test_dict_to_tree_sep_undefined():
+    def test_dict_to_tree_sep_error():
         paths = {
             "a": {"age": 90},
             "a-b": {"age": 65},
             "a-c": {"age": 60},
             "a-b-d": {"age": 40},
             "a-b-e": {"age": 35},
             "a-c-f": {"age": 38},
             "a-b-e-g": {"age": 10},
             "a-b-e-h": {"age": 6},
         }
-        with pytest.raises(TreeError):
+        with pytest.raises(TreeError) as exc_info:
             dict_to_tree(paths)
+        assert str(exc_info.value).startswith(Constants.ERROR_DIFFERENT_ROOT)
 
     @staticmethod
     def test_dict_to_tree_sep():
         paths = {
             "a": {"age": 90},
             "a\\b": {"age": 65},
             "a\\c": {"age": 60},
             "a\\b\\d": {"age": 40},
             "a\\b\\e": {"age": 35},
             "a\\c\\f": {"age": 38},
             "a\\b\\e\\g": {"age": 10},
             "a\\b\\e\\h": {"age": 6},
         }
         root = dict_to_tree(paths, sep="\\")
-        assert_tree_structure_basenode_root_generic(root)
+        assert_tree_structure_basenode_root(root)
         assert_tree_structure_basenode_root_attr(root)
         assert_tree_structure_node_root_sep(root)
 
     @staticmethod
-    def test_dict_to_tree_duplicate_node():
+    def test_dict_to_tree_duplicate_node_error():
         path_dict = {
             "a": {"age": 90},
             "a/b": {"age": 65},
             "a/c": {"age": 60},
             "a/b/d": {"age": 40},
             "a/b/e": {"age": 35},
             "a/c/d": {"age": 38},  # duplicate
             "a/b/e/g": {"age": 10},
             "a/b/e/h": {"age": 6},
         }
-        with pytest.raises(DuplicatedNodeError):
+        with pytest.raises(DuplicatedNodeError) as exc_info:
             dict_to_tree(path_dict, duplicate_name_allowed=False)
+        assert str(exc_info.value).startswith("Node d already exists")
 
+    @staticmethod
+    def test_dict_to_tree_duplicate_node():
+        path_dict = {
+            "a": {"age": 90},
+            "a/b": {"age": 65},
+            "a/c": {"age": 60},
+            "a/b/d": {"age": 40},
+            "a/b/e": {"age": 35},
+            "a/c/d": {"age": 38},  # duplicate
+            "a/b/e/g": {"age": 10},
+            "a/b/e/h": {"age": 6},
+        }
         root = dict_to_tree(path_dict)
-        assert_tree_structure_basenode_root_generic(root)
+        assert_tree_structure_basenode_root(root)
         assert_tree_structure_basenode_root_attr(root, f=("d", 38))
-        assert_tree_structure_node_root_generic(root, f="/a/c/d")
+        assert_tree_structure_node_root(root, f="/a/c/d")
 
     def test_dict_to_tree_node_type(self):
         root = dict_to_tree(self.path_dict, node_type=NodeA)
-        assert isinstance(root, NodeA), "Node type is not `NodeA`"
-        assert_tree_structure_basenode_root_generic(root)
+        assert isinstance(root, NodeA), Constants.ERROR_NODE_TYPE
+        assert_tree_structure_basenode_root(root)
         assert_tree_structure_basenode_root_attr(root)
-        assert_tree_structure_node_root_generic(root)
+        assert_tree_structure_node_root(root)
 
     @staticmethod
-    def test_dict_to_tree_different_root():
+    def test_dict_to_tree_different_root_error():
         path_dict = {
             "a": {"age": 90},
             "a/b": {"age": 65},
             "a/c": {"age": 60},
             "a/b/d": {"age": 40},
             "a/b/e": {"age": 35},
             "a/c/f": {"age": 38},
             "a/b/e/g": {"age": 10},
             "b/b/e/h": {"age": 6},  # different root
         }
-        with pytest.raises(TreeError):
+        with pytest.raises(TreeError) as exc_info:
             dict_to_tree(path_dict)
+        assert str(exc_info.value).startswith(Constants.ERROR_DIFFERENT_ROOT)
 
 
 class TestNestedDictToTree(unittest.TestCase):
     def setUp(self):
         """
         Tree should have structure
         a (age=90)
@@ -1301,17 +1446,22 @@
         }
 
     def tearDown(self):
         self.path_dict = None
 
     def test_nested_dict_to_tree(self):
         root = nested_dict_to_tree(self.path_dict)
-        assert_tree_structure_basenode_root_generic(root)
+        assert_tree_structure_basenode_root(root)
         assert_tree_structure_basenode_root_attr(root)
-        assert_tree_structure_node_root_generic(root)
+        assert_tree_structure_node_root(root)
+
+    def test_nested_dict_to_tree_empty_error(self):
+        with pytest.raises(ValueError) as exc_info:
+            nested_dict_to_tree({})
+        assert str(exc_info.value).startswith(Constants.ERROR_EMPTY_DICT)
 
     @staticmethod
     def test_nested_dict_to_tree_key_name():
         path_dict = {
             "node_name": "a",
             "age": 90,
             "node_children": [
@@ -1336,24 +1486,24 @@
                     "node_children": [{"node_name": "f", "age": 38}],
                 },
             ],
         }
         root = nested_dict_to_tree(
             path_dict, name_key="node_name", child_key="node_children"
         )
-        assert_tree_structure_basenode_root_generic(root)
+        assert_tree_structure_basenode_root(root)
         assert_tree_structure_basenode_root_attr(root)
-        assert_tree_structure_node_root_generic(root)
+        assert_tree_structure_node_root(root)
 
     def test_nested_dict_to_tree_node_type(self):
         root = nested_dict_to_tree(self.path_dict, node_type=NodeA)
-        assert isinstance(root, NodeA), "Node type is not `NodeA`"
-        assert_tree_structure_basenode_root_generic(root)
+        assert isinstance(root, NodeA), Constants.ERROR_NODE_TYPE
+        assert_tree_structure_basenode_root(root)
         assert_tree_structure_basenode_root_attr(root)
-        assert_tree_structure_node_root_generic(root)
+        assert_tree_structure_node_root(root)
 
 
 class TestDataFrameToTree(unittest.TestCase):
     def setUp(self):
         """
         Tree should have structure
         a (age=90)
@@ -1380,25 +1530,31 @@
         )
 
     def tearDown(self):
         self.path_data = None
 
     def test_dataframe_to_tree(self):
         root = dataframe_to_tree(self.path_data)
-        assert_tree_structure_basenode_root_generic(root)
+        assert_tree_structure_basenode_root(root)
         assert_tree_structure_basenode_root_attr(root)
-        assert_tree_structure_node_root_generic(root)
+        assert_tree_structure_node_root(root)
 
     def test_dataframe_to_tree_col_name(self):
         root = dataframe_to_tree(
             self.path_data, path_col="PATH", attribute_cols=["age"]
         )
-        assert_tree_structure_basenode_root_generic(root)
+        assert_tree_structure_basenode_root(root)
         assert_tree_structure_basenode_root_attr(root)
-        assert_tree_structure_node_root_generic(root)
+        assert_tree_structure_node_root(root)
+
+    def test_dataframe_to_tree_col_name_reverse(self):
+        root = dataframe_to_tree(self.path_data[["age", "PATH"]], path_col="PATH")
+        assert_tree_structure_basenode_root(root)
+        assert_tree_structure_basenode_root_attr(root)
+        assert_tree_structure_node_root(root)
 
     @staticmethod
     def test_dataframe_to_tree_no_attribute():
         path_data = pd.DataFrame(
             [
                 ["a"],
                 ["a/b"],
@@ -1408,169 +1564,211 @@
                 ["a/c/f"],
                 ["a/b/e/g"],
                 ["a/b/e/h"],
             ],
             columns=["PATH"],
         )
         root = dataframe_to_tree(path_data)
-        assert_tree_structure_basenode_root_generic(root)
+        assert_tree_structure_basenode_root(root)
 
     @staticmethod
-    def test_dataframe_to_tree_empty_row():
-        data = pd.DataFrame(columns=["PATH", "age"])
-        with pytest.raises(ValueError):
-            dataframe_to_tree(data)
+    def test_dataframe_to_tree_empty_row_error():
+        path_data = pd.DataFrame(columns=["PATH", "age"])
+        with pytest.raises(ValueError) as exc_info:
+            dataframe_to_tree(path_data)
+        assert str(exc_info.value) == Constants.ERROR_EMPTY_ROW
 
     @staticmethod
-    def test_dataframe_to_tree_empty_col():
-        data = pd.DataFrame()
-        with pytest.raises(ValueError):
-            dataframe_to_tree(data)
+    def test_dataframe_to_tree_empty_col_error():
+        path_data = pd.DataFrame()
+        with pytest.raises(ValueError) as exc_info:
+            dataframe_to_tree(path_data)
+        assert str(exc_info.value) == Constants.ERROR_EMPTY_COL
 
     @staticmethod
     def test_dataframe_to_tree_sep_leading():
-        data = pd.DataFrame(
+        path_data = pd.DataFrame(
             [
                 ["/a", 90],
                 ["/a/b", 65],
                 ["/a/c", 60],
                 ["/a/b/d", 40],
                 ["/a/b/e", 35],
                 ["/a/c/f", 38],
                 ["/a/b/e/g", 10],
                 ["/a/b/e/h", 6],
             ],
             columns=["PATH", "age"],
         )
-        root = dataframe_to_tree(data)
-        assert_tree_structure_basenode_root_generic(root)
+        root = dataframe_to_tree(path_data)
+        assert_tree_structure_basenode_root(root)
         assert_tree_structure_basenode_root_attr(root)
-        assert_tree_structure_node_root_generic(root)
+        assert_tree_structure_node_root(root)
 
     def test_dataframe_to_tree_sep_trailing(self):
-        data = pd.DataFrame(
+        path_data = pd.DataFrame(
             [
                 ["a/", 90],
                 ["a/b/", 65],
                 ["a/c/", 60],
                 ["a/b/d/", 40],
                 ["a/b/e/", 35],
                 ["a/c/f/", 38],
                 ["a/b/e/g/", 10],
                 ["a/b/e/h/", 6],
             ],
             columns=["PATH", "age"],
         )
-        root = dataframe_to_tree(data)
-        assert_tree_structure_basenode_root_generic(root)
+        root = dataframe_to_tree(path_data)
+        assert_tree_structure_basenode_root(root)
         assert_tree_structure_basenode_root_attr(root)
-        assert_tree_structure_node_root_generic(root)
+        assert_tree_structure_node_root(root)
 
-    def test_dataframe_to_tree_sep_undefined(self):
-        data = pd.DataFrame(
+    def test_dataframe_to_tree_sep_error(self):
+        path_data = pd.DataFrame(
             [
                 ["a", 90],
                 ["a\\b", 65],
                 ["a\\c", 60],
                 ["a\\b\\d", 40],
                 ["a\\b\\e", 35],
                 ["a\\c\\f", 38],
                 ["a\\b\\e\\g", 10],
                 ["a\\b\\e\\h", 6],
             ],
             columns=["PATH", "age"],
         )
-        with pytest.raises(TreeError):
-            dataframe_to_tree(data)
+        with pytest.raises(TreeError) as exc_info:
+            dataframe_to_tree(path_data)
+        assert str(exc_info.value).startswith(Constants.ERROR_DIFFERENT_ROOT)
 
     def test_dataframe_to_tree_sep(self):
-        data = pd.DataFrame(
+        path_data = pd.DataFrame(
             [
                 ["a", 90],
                 ["a\\b", 65],
                 ["a\\c", 60],
                 ["a\\b\\d", 40],
                 ["a\\b\\e", 35],
                 ["a\\c\\f", 38],
                 ["a\\b\\e\\g", 10],
                 ["a\\b\\e\\h", 6],
             ],
             columns=["PATH", "age"],
         )
-        root = dataframe_to_tree(data, sep="\\")
-        assert_tree_structure_basenode_root_generic(root)
+        root = dataframe_to_tree(path_data, sep="\\")
+        assert_tree_structure_basenode_root(root)
         assert_tree_structure_basenode_root_attr(root)
         assert_tree_structure_node_root_sep(root)
 
-    def test_dataframe_to_tree_node_type(self):
-        root = dataframe_to_tree(self.path_data, node_type=NodeA)
-        assert isinstance(root, NodeA), "Node type is not `NodeA`"
-        assert_tree_structure_basenode_root_generic(root)
-        assert_tree_structure_basenode_root_attr(root)
-        assert_tree_structure_node_root_generic(root)
-
     @staticmethod
-    def test_dataframe_to_tree_different_root():
+    def test_dataframe_to_tree_duplicate_data_error():
         path_data = pd.DataFrame(
             [
                 ["a", 90],
                 ["a/b", 65],
                 ["a/c", 60],
                 ["a/b/d", 40],
                 ["a/b/e", 35],
                 ["a/c/f", 38],
                 ["a/b/e/g", 10],
-                ["b/b/e/h", 6],  # different root
+                ["a/b/e/h", 6],
+                ["a/b/e/h", 7],  # duplicate
             ],
             columns=["PATH", "age"],
         )
-        with pytest.raises(TreeError):
+        with pytest.raises(ValueError) as exc_info:
             dataframe_to_tree(path_data)
+        assert str(exc_info.value).startswith(Constants.ERROR_DUPLICATE_PATH)
 
     @staticmethod
-    def test_dataframe_to_tree_duplicate():
+    def test_dataframe_to_tree_duplicate_data():
         path_data = pd.DataFrame(
             [
                 ["a", 90],
                 ["a/b", 65],
                 ["a/c", 60],
                 ["a/b/d", 40],
                 ["a/b/e", 35],
                 ["a/c/f", 38],
                 ["a/b/e/g", 10],
                 ["a/b/e/h", 6],
-                ["a/b/e/h", 7],  # duplicate
+                ["a/b/e/h", 6],  # duplicate
             ],
             columns=["PATH", "age"],
         )
-        with pytest.raises(ValueError):
-            dataframe_to_tree(path_data)
+        root = dataframe_to_tree(path_data)
+        assert_tree_structure_basenode_root(root)
+        assert_tree_structure_basenode_root_attr(root)
+        assert_tree_structure_node_root(root)
 
     @staticmethod
-    def test_dataframe_to_tree_duplicate_node():
+    def test_dataframe_to_tree_duplicate_node_error():
         path_data = pd.DataFrame(
             [
                 ["a", 90],
                 ["a/b", 65],
                 ["a/c", 60],
                 ["a/b/d", 40],
                 ["a/b/e", 35],
                 ["a/c/d", 38],  # duplicate
                 ["a/b/e/g", 10],
                 ["a/b/e/h", 6],
             ],
             columns=["PATH", "age"],
         )
-        with pytest.raises(DuplicatedNodeError):
+        with pytest.raises(DuplicatedNodeError) as exc_info:
             dataframe_to_tree(path_data, duplicate_name_allowed=False)
+        assert str(exc_info.value).startswith("Node d already exists")
 
+    @staticmethod
+    def test_dataframe_to_tree_duplicate_node():
+        path_data = pd.DataFrame(
+            [
+                ["a", 90],
+                ["a/b", 65],
+                ["a/c", 60],
+                ["a/b/d", 40],
+                ["a/b/e", 35],
+                ["a/c/d", 38],  # duplicate
+                ["a/b/e/g", 10],
+                ["a/b/e/h", 6],
+            ],
+            columns=["PATH", "age"],
+        )
         root = dataframe_to_tree(path_data)
-        assert_tree_structure_basenode_root_generic(root)
+        assert_tree_structure_basenode_root(root)
         assert_tree_structure_basenode_root_attr(root, f=("d", 38))
-        assert_tree_structure_node_root_generic(root, f="/a/c/d")
+        assert_tree_structure_node_root(root, f="/a/c/d")
+
+    def test_dataframe_to_tree_node_type(self):
+        root = dataframe_to_tree(self.path_data, node_type=NodeA)
+        assert isinstance(root, NodeA), Constants.ERROR_NODE_TYPE
+        assert_tree_structure_basenode_root(root)
+        assert_tree_structure_basenode_root_attr(root)
+        assert_tree_structure_node_root(root)
+
+    @staticmethod
+    def test_dataframe_to_tree_different_root_error():
+        path_data = pd.DataFrame(
+            [
+                ["a", 90],
+                ["a/b", 65],
+                ["a/c", 60],
+                ["a/b/d", 40],
+                ["a/b/e", 35],
+                ["a/c/f", 38],
+                ["a/b/e/g", 10],
+                ["b/b/e/h", 6],  # different root
+            ],
+            columns=["PATH", "age"],
+        )
+        with pytest.raises(TreeError) as exc_info:
+            dataframe_to_tree(path_data)
+        assert str(exc_info.value).startswith(Constants.ERROR_DIFFERENT_ROOT)
 
 
 class TestDataFrameToTreeByRelation(unittest.TestCase):
     def setUp(self):
         self.relation_data = pd.DataFrame(
             [
                 ["a", None, 90],
@@ -1586,85 +1784,121 @@
         )
 
     def tearDown(self):
         self.relation_data = None
 
     def test_dataframe_to_tree_by_relation(self):
         root = dataframe_to_tree_by_relation(self.relation_data)
-        assert_tree_structure_basenode_root_generic(root)
+        assert_tree_structure_basenode_root(root)
         assert_tree_structure_basenode_root_attr(root)
-        assert_tree_structure_node_root_generic(root)
+        assert_tree_structure_node_root(root)
 
     def test_dataframe_to_tree_by_relation_col_name(self):
         root = dataframe_to_tree_by_relation(
             self.relation_data,
             child_col="child",
             parent_col="parent",
             attribute_cols=["age"],
         )
-        assert_tree_structure_basenode_root_generic(root)
+        assert_tree_structure_basenode_root(root)
+        assert_tree_structure_basenode_root_attr(root)
+        assert_tree_structure_node_root(root)
+
+    def test_dataframe_to_tree_by_relation_col_name_reverse(self):
+        root = dataframe_to_tree_by_relation(
+            self.relation_data[["age", "parent", "child"]],
+            child_col="child",
+            parent_col="parent",
+            attribute_cols=["age"],
+        )
+        assert_tree_structure_basenode_root(root)
         assert_tree_structure_basenode_root_attr(root)
-        assert_tree_structure_node_root_generic(root)
+        assert_tree_structure_node_root(root)
+
+    def test_dataframe_to_tree_by_relation_empty_row_error(self):
+        relation_data = pd.DataFrame(columns=["child", "parent"])
+        with pytest.raises(ValueError) as exc_info:
+            dataframe_to_tree_by_relation(relation_data)
+        assert str(exc_info.value) == Constants.ERROR_EMPTY_ROW
+
+    def test_dataframe_to_tree_by_relation_empty_col_error(self):
+        relation_data = pd.DataFrame()
+        with pytest.raises(ValueError) as exc_info:
+            dataframe_to_tree_by_relation(relation_data)
+        assert str(exc_info.value) == Constants.ERROR_EMPTY_COL
 
     @staticmethod
     def test_dataframe_to_tree_by_relation_duplicate_leaf_node():
         relation_data = pd.DataFrame(
             [
                 ["a", None, 90],
                 ["b", "a", 65],
                 ["c", "a", 60],
                 ["d", "b", 40],
                 ["e", "b", 35],
                 ["h", "b", 1],
                 ["h", "c", 2],
-                ["g", "e", 10],
-                ["h", "e", 1],
+                ["g", "e", 10],  # duplicate
+                ["h", "e", 1],  # duplicate
             ],
             columns=["child", "parent", "age"],
         )
         root = dataframe_to_tree_by_relation(relation_data)
         expected = """a\n├── b\n│   ├── d\n│   ├── e\n│   │   ├── g\n│   │   └── h\n│   └── h\n└── c\n    └── h\n"""
         assert_print_statement(print_tree, expected, tree=root, style="const")
 
     @staticmethod
-    def test_dataframe_to_tree_by_relation_empty_row():
-        data = pd.DataFrame(columns=["child", "parent"])
-        with pytest.raises(ValueError):
-            dataframe_to_tree_by_relation(data)
-
-    @staticmethod
-    def test_dataframe_to_tree_by_relation_empty_col():
-        data = pd.DataFrame()
-        with pytest.raises(ValueError):
+    def test_dataframe_to_tree_by_relation_duplicate_intermediate_node_error():
+        data = pd.DataFrame(
+            [
+                ["a", None, 90],
+                ["b", "a", 65],
+                ["c", "a", 60],
+                ["d", "b", 40],
+                ["e", "b", 35],
+                ["e", "c", 1],  # duplicate parent
+                ["f", "c", 38],
+                ["g", "e", 10],
+                ["h", "e", 6],
+            ],
+            columns=["child", "parent", "age"],
+        )
+        with pytest.raises(ValueError) as exc_info:
             dataframe_to_tree_by_relation(data)
+        assert str(exc_info.value).startswith(Constants.ERROR_DUPLICATE_PARENT)
 
     @staticmethod
-    def test_dataframe_to_tree_by_relation_duplicated_intermediate_node():
+    def test_dataframe_to_tree_by_relation_duplicate_intermediate_node():
         data = pd.DataFrame(
             [
                 ["a", None, 90],
                 ["b", "a", 65],
                 ["c", "a", 60],
                 ["d", "b", 40],
                 ["e", "b", 35],
                 ["e", "c", 1],
                 ["f", "c", 38],
                 ["g", "e", 10],
                 ["h", "e", 6],
             ],
             columns=["child", "parent", "age"],
         )
-        with pytest.raises(ValueError) as exc_info:
-            dataframe_to_tree_by_relation(data)
-        assert str(exc_info.value).startswith(
-            "There exists duplicate child with different parent"
-        )
+        root = dataframe_to_tree_by_relation(data, allow_duplicates=True)
+        actual = len(list(root.descendants))
+        assert actual == 10, f"Expected tree to have 10 descendants, received {actual}"
+
+    def test_dataframe_to_tree_by_relation_node_type(self):
+        root = dataframe_to_tree_by_relation(self.relation_data, node_type=NodeA)
+        assert isinstance(root, NodeA), Constants.ERROR_NODE_TYPE
+        assert_tree_structure_basenode_root(root)
+        assert_tree_structure_basenode_root_attr(root)
+        assert_tree_structure_node_root(root)
 
     @staticmethod
-    def test_dataframe_to_tree_by_relation_multiple_root():
+    def test_dataframe_to_tree_by_relation_different_root_error():
         data = pd.DataFrame(
             [
                 ["a", None, 90],
                 ["b", None, 65],
                 ["c", "a", 60],
                 ["e", "b", 40],
                 ["e", "b", 35],
@@ -1673,18 +1907,18 @@
                 ["g", "e", 10],
                 ["h", "e", 1],
             ],
             columns=["child", "parent", "age"],
         )
         with pytest.raises(ValueError) as exc_info:
             dataframe_to_tree_by_relation(data)
-        assert str(exc_info.value).startswith("Unable to determine root node")
+        assert str(exc_info.value).startswith(Constants.ERROR_MULTIPLE_ROOT)
 
     @staticmethod
-    def test_dataframe_to_tree_by_relation_no_root():
+    def test_dataframe_to_tree_by_relation_no_root_error():
         data = pd.DataFrame(
             [
                 ["a", "b", 90],
                 ["b", "a", 65],
                 ["c", "a", 60],
                 ["d", "b", 40],
                 ["e", "b", 35],
@@ -1693,8 +1927,8 @@
                 ["g", "e", 10],
                 ["h", "e", 1],
             ],
             columns=["child", "parent", "age"],
         )
         with pytest.raises(ValueError) as exc_info:
             dataframe_to_tree_by_relation(data)
-        assert str(exc_info.value).startswith("Unable to determine root node")
+        assert str(exc_info.value).startswith(Constants.ERROR_MULTIPLE_ROOT)
```

### Comparing `bigtree-0.9.3/tests/tree/test_export.py` & `bigtree-0.9.4/tests/tree/test_export.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,26 +7,27 @@
     tree_to_dataframe,
     tree_to_dict,
     tree_to_dot,
     tree_to_nested_dict,
     tree_to_pillow,
 )
 from tests.conftest import assert_print_statement
+from tests.constants import Constants
 from tests.node.test_basenode import (
+    assert_tree_structure_basenode_root,
     assert_tree_structure_basenode_root_attr,
-    assert_tree_structure_basenode_root_generic,
 )
-from tests.node.test_node import assert_tree_structure_node_root_generic
+from tests.node.test_node import assert_tree_structure_node_root
 
 tree_node_str = """a [age=90]\n├── b [age=65]\n│   ├── d [age=40]\n│   └── e [age=35]\n│       ├── g [age=10]
 │       └── h [age=6]\n└── c [age=60]\n    └── f [age=38]\n"""
 tree_node_no_attr_str = """a\n├── b\n│   ├── d\n│   └── e\n│       ├── g\n│       └── h\n└── c\n    └── f\n"""
 
 
-LOCAL = False
+LOCAL = Constants.LOCAL
 
 
 class TestPrintTree:
     @staticmethod
     def test_print_tree_child_node_name(tree_node):
         expected_str = """b\n├── d\n└── e\n    ├── g\n    └── h\n"""
         assert_print_statement(
@@ -115,17 +116,15 @@
             attr_bracket=["(", ")"],
         )
 
     @staticmethod
     def test_print_tree_attr_bracket_missing_error(tree_node):
         with pytest.raises(ValueError) as exc_info:
             print_tree(tree_node, all_attrs=True, attr_bracket=[""])
-        assert str(exc_info.value).startswith(
-            "Expect open and close brackets in `attr_bracket`"
-        )
+        assert str(exc_info.value).startswith(Constants.ERROR_ATTR_BRACKET)
 
     # style
     @staticmethod
     def test_print_tree_style_ansi(tree_node):
         expected_str = """a\n|-- b\n|   |-- d\n|   `-- e\n|       |-- g\n|       `-- h\n`-- c\n    `-- f\n"""
         assert_print_statement(print_tree, expected_str, tree=tree_node, style="ansi")
 
@@ -180,29 +179,25 @@
     def test_print_tree_custom_style_unequal_char_error(tree_node):
         with pytest.raises(ValueError) as exc_info:
             print_tree(
                 tree_node,
                 style="custom",
                 custom_style=["", " ", ""],
             )
-        assert str(exc_info.value).startswith(
-            "`style_stem`, `style_branch`, and `style_stem_final` are of different length"
-        )
+        assert str(exc_info.value) == Constants.ERROR_CUSTOM_STYLE_DIFFERENT_LENGTH
 
     @staticmethod
     def test_print_tree_custom_style_missing_style_error(tree_node):
         with pytest.raises(ValueError) as exc_info:
             print_tree(
                 tree_node,
                 style="custom",
                 custom_style=["", ""],
             )
-        assert str(exc_info.value).startswith(
-            "Custom style selected, please specify the style of stem, branch, and final stem in `custom_style`"
-        )
+        assert str(exc_info.value) == Constants.ERROR_CUSTOM_STYLE_SELECT
 
 
 class TestTreeToDataFrame:
     @staticmethod
     def test_tree_to_dataframe(tree_node):
         expected = pd.DataFrame(
             [
@@ -440,17 +435,17 @@
         )
         pd.testing.assert_frame_equal(expected, actual)
 
     @staticmethod
     def test_tree_to_dataframe_to_tree(tree_node):
         d = tree_to_dataframe(tree_node, all_attrs=True)
         tree = dataframe_to_tree(d)
-        assert_tree_structure_basenode_root_generic(tree)
+        assert_tree_structure_basenode_root(tree)
         assert_tree_structure_basenode_root_attr(tree)
-        assert_tree_structure_node_root_generic(tree)
+        assert_tree_structure_node_root(tree)
 
 
 class TestTreeToDict:
     @staticmethod
     def test_tree_to_dict(tree_node):
         expected = {
             "/a": {"name": "a"},
@@ -607,17 +602,17 @@
         )
         assert expected == actual, f"Expected\n{expected}\nReceived\n{actual}"
 
     @staticmethod
     def test_tree_to_dict_to_tree(tree_node):
         d = tree_to_dict(tree_node, all_attrs=True)
         tree = dict_to_tree(d)
-        assert_tree_structure_basenode_root_generic(tree)
+        assert_tree_structure_basenode_root(tree)
         assert_tree_structure_basenode_root_attr(tree)
-        assert_tree_structure_node_root_generic(tree)
+        assert_tree_structure_node_root(tree)
 
 
 class TestTreeToNestedDict:
     @staticmethod
     def test_tree_to_nested_dict(tree_node):
         expected = {
             "name": "a",
@@ -782,17 +777,17 @@
         )
         assert expected == actual, f"Expected\n{expected}\nReceived\n{actual}"
 
     @staticmethod
     def test_tree_to_nested_dict_to_tree(tree_node):
         d = tree_to_nested_dict(tree_node, all_attrs=True)
         tree = nested_dict_to_tree(d)
-        assert_tree_structure_basenode_root_generic(tree)
+        assert_tree_structure_basenode_root(tree)
         assert_tree_structure_basenode_root_attr(tree)
-        assert_tree_structure_node_root_generic(tree)
+        assert_tree_structure_node_root(tree)
 
 
 class TestTreeToDot:
     @staticmethod
     def test_tree_to_dot(tree_node):
         graph = tree_to_dot(tree_node)
         expected = """strict digraph G {\nrankdir=TB;\na0 [label=a];\nb0 [label=b];\na0 -> b0;\nd0 [label=d];\nb0 -> d0;\ne0 [label=e];\nb0 -> e0;\ng0 [label=g];\ne0 -> g0;\nh0 [label=h];\ne0 -> h0;\nc0 [label=c];\na0 -> c0;\nf0 [label=f];\nc0 -> f0;\n}\n"""
@@ -818,105 +813,123 @@
 
     @staticmethod
     def test_tree_to_dot_duplicate_names(tree_node_duplicate_names):
         graph = tree_to_dot(tree_node_duplicate_names)
         expected = """strict digraph G {\nrankdir=TB;\na0 [label=a];\na1 [label=a];\na0 -> a1;\na2 [label=a];\na1 -> a2;\nb0 [label=b];\na1 -> b0;\na3 [label=a];\nb0 -> a3;\nb1 [label=b];\nb0 -> b1;\nb2 [label=b];\na0 -> b2;\na4 [label=a];\nb2 -> a4;\n}\n"""
         actual = graph.to_string()
         if LOCAL:
-            graph.write_png("tests/tree_duplicate.png")
+            graph.write_png("tests/tree_duplicate_names.png")
         for expected_str in expected.split():
             assert (
                 expected_str in actual
             ), f"Expected {expected_str} not in actual string"
 
     @staticmethod
     def test_tree_to_dot_type_error(dag_node):
         with pytest.raises(ValueError) as exc_info:
             tree_to_dot(dag_node)
-        assert str(exc_info.value).startswith("Tree should be of type `Node`")
+        assert str(exc_info.value) == Constants.ERROR_EXPORT_NODE_TYPE
 
     @staticmethod
     def test_tree_to_dot_directed(tree_node):
         graph = tree_to_dot(tree_node, directed=False)
         expected = """strict graph G {\nrankdir=TB;\na0 [label=a];\nb0 [label=b];\na0 -- b0;\nd0 [label=d];\nb0 -- d0;\ne0 [label=e];\nb0 -- e0;\ng0 [label=g];\ne0 -- g0;\nh0 [label=h];\ne0 -- h0;\nc0 [label=c];\na0 -- c0;\nf0 [label=f];\nc0 -- f0;\n}\n"""
         actual = graph.to_string()
         if LOCAL:
             graph.write_png("tests/tree_undirected.png")
         for expected_str in expected.split():
             assert (
                 expected_str in actual
             ), f"Expected {expected_str} not in actual string"
 
     @staticmethod
-    def test_tree_to_dot_bg_color(tree_node):
+    def test_tree_to_dot_bg_colour(tree_node):
         graph = tree_to_dot(tree_node, bg_colour="blue")
         expected = """strict digraph G {\nbgcolor=blue;\nrankdir=TB;\na0 [label=a];\nb0 [label=b];\na0 -> b0;\nd0 [label=d];\nb0 -> d0;\ne0 [label=e];\nb0 -> e0;\ng0 [label=g];\ne0 -> g0;\nh0 [label=h];\ne0 -> h0;\nc0 [label=c];\na0 -> c0;\nf0 [label=f];\nc0 -> f0;\n}\n"""
         actual = graph.to_string()
         if LOCAL:
-            graph.write_png("tests/tree_bg.png")
+            graph.write_png("tests/tree_bg_colour.png")
         for expected_str in expected.split():
             assert (
                 expected_str in actual
             ), f"Expected {expected_str} not in actual string"
 
     @staticmethod
-    def test_tree_to_dot_node_colour(tree_node):
+    def test_tree_to_dot_fill_colour(tree_node):
         graph = tree_to_dot(tree_node, node_colour="gold")
         expected = """strict digraph G {\nrankdir=TB;\na0 [fillcolor=gold, label=a, style=filled];\nb0 [fillcolor=gold, label=b, style=filled];\na0 -> b0;\nd0 [fillcolor=gold, label=d, style=filled];\nb0 -> d0;\ne0 [fillcolor=gold, label=e, style=filled];\nb0 -> e0;\ng0 [fillcolor=gold, label=g, style=filled];\ne0 -> g0;\nh0 [fillcolor=gold, label=h, style=filled];\ne0 -> h0;\nc0 [fillcolor=gold, label=c, style=filled];\na0 -> c0;\nf0 [fillcolor=gold, label=f, style=filled];\nc0 -> f0;\n}\n"""
         actual = graph.to_string()
         if LOCAL:
-            graph.write_png("tests/tree_fill.png")
+            graph.write_png("tests/tree_fill_colour.png")
         for expected_str in expected.split():
             assert (
                 expected_str in actual
             ), f"Expected {expected_str} not in actual string"
 
     @staticmethod
-    def test_tree_to_dot_node_shape(tree_node):
-        graph = tree_to_dot(tree_node, node_shape="triangle")
-        expected = """strict digraph G {\nrankdir=TB;\na0 [label=a, shape=triangle];\nb0 [label=b, shape=triangle];\na0 -> b0;\nd0 [label=d, shape=triangle];\nb0 -> d0;\ne0 [label=e, shape=triangle];\nb0 -> e0;\ng0 [label=g, shape=triangle];\ne0 -> g0;\nh0 [label=h, shape=triangle];\ne0 -> h0;\nc0 [label=c, shape=triangle];\na0 -> c0;\nf0 [label=f, shape=triangle];\nc0 -> f0;\n}\n"""
+    def test_tree_to_dot_edge_colour(tree_node):
+        graph = tree_to_dot(tree_node, edge_colour="red")
+        expected = """strict digraph G {\nrankdir=TB;\na0 [label=a];\nb0 [label=b];\na0 -> b0  [color=red];\nd0 [label=d];\nb0 -> d0  [color=red];\ne0 [label=e];\nb0 -> e0  [color=red];\ng0 [label=g];\ne0 -> g0  [color=red];\nh0 [label=h];\ne0 -> h0  [color=red];\nc0 [label=c];\na0 -> c0  [color=red];\nf0 [label=f];\nc0 -> f0  [color=red];\n}\n"""
         actual = graph.to_string()
         if LOCAL:
-            graph.write_png("tests/tree_triangle.png")
+            graph.write_png("tests/tree_edge_colour.png")
         for expected_str in expected.split():
             assert (
                 expected_str in actual
             ), f"Expected {expected_str} not in actual string"
 
     @staticmethod
-    def test_tree_to_dot_edge_colour(tree_node):
-        graph = tree_to_dot(tree_node, edge_colour="red")
-        expected = """strict digraph G {\nrankdir=TB;\na0 [label=a];\nb0 [label=b];\na0 -> b0  [color=red];\nd0 [label=d];\nb0 -> d0  [color=red];\ne0 [label=e];\nb0 -> e0  [color=red];\ng0 [label=g];\ne0 -> g0  [color=red];\nh0 [label=h];\ne0 -> h0  [color=red];\nc0 [label=c];\na0 -> c0  [color=red];\nf0 [label=f];\nc0 -> f0  [color=red];\n}\n"""
+    def test_tree_to_dot_node_shape(tree_node):
+        graph = tree_to_dot(tree_node, node_shape="triangle")
+        expected = """strict digraph G {\nrankdir=TB;\na0 [label=a, shape=triangle];\nb0 [label=b, shape=triangle];\na0 -> b0;\nd0 [label=d, shape=triangle];\nb0 -> d0;\ne0 [label=e, shape=triangle];\nb0 -> e0;\ng0 [label=g, shape=triangle];\ne0 -> g0;\nh0 [label=h, shape=triangle];\ne0 -> h0;\nc0 [label=c, shape=triangle];\na0 -> c0;\nf0 [label=f, shape=triangle];\nc0 -> f0;\n}\n"""
         actual = graph.to_string()
         if LOCAL:
-            graph.write_png("tests/tree_edge.png")
+            graph.write_png("tests/tree_node_shape.png")
         for expected_str in expected.split():
             assert (
                 expected_str in actual
             ), f"Expected {expected_str} not in actual string"
 
     @staticmethod
     def test_tree_to_dot_node_attr(tree_node_style):
         graph = tree_to_dot(tree_node_style, node_attr="node_style")
         expected = """strict digraph G {\nrankdir=TB;\na0 [fillcolor=gold, label=a, style=filled];\nb0 [fillcolor=blue, label=b, style=filled];\na0 -> b0;\nd0 [fillcolor=green, label=d, style=filled];\nb0 -> d0;\ng0 [fillcolor=red, label=g, style=filled];\nd0 -> g0;\ne0 [fillcolor=green, label=e, style=filled];\nb0 -> e0;\nh0 [fillcolor=red, label=h, style=filled];\ne0 -> h0;\nc0 [fillcolor=blue, label=c, style=filled];\na0 -> c0;\nf0 [fillcolor=green, label=f, style=filled];\nc0 -> f0;\n}\n"""
         actual = graph.to_string()
         if LOCAL:
-            graph.write_png("tests/tree_node_style.png")
+            graph.write_png("tests/tree_node_attr.png")
         for expected_str in expected.split():
             assert (
                 expected_str in actual
             ), f"Expected {expected_str} not in actual string"
 
     @staticmethod
     def test_tree_to_dot_edge_attr(tree_node_style):
         graph = tree_to_dot(tree_node_style, edge_attr="edge_style")
         expected = """strict digraph G {\nrankdir=TB;\na0 [label=a];\nb0 [label=b];\na0 -> b0  [label=b, style=bold];\nd0 [label=d];\nb0 -> d0  [label=1, style=bold];\ng0 [label=g];\nd0 -> g0  [label=4, style=bold];\ne0 [label=e];\nb0 -> e0  [label=2, style=bold];\nh0 [label=h];\ne0 -> h0  [label=5, style=bold];\nc0 [label=c];\na0 -> c0  [label=c, style=bold];\nf0 [label=f];\nc0 -> f0  [label=3, style=bold];\n}\n"""
         actual = graph.to_string()
         if LOCAL:
-            graph.write_png("tests/tree_edge_style.png")
+            graph.write_png("tests/tree_edge_attr.png")
+        for expected_str in expected.split():
+            assert (
+                expected_str in actual
+            ), f"Expected {expected_str} not in actual string"
+
+    @staticmethod
+    def test_tree_to_dot_attr_override(tree_node):
+        tree_node.children[0].set_attrs(
+            {
+                "node_style": {"style": "filled", "fillcolor": "blue"},
+                "edge_style": {"style": "bold"},
+            }
+        )
+        graph = tree_to_dot(tree_node, node_attr="node_style", edge_attr="edge_style")
+        expected = """strict digraph G {\nrankdir=TB;\na0 [label=a];\nb0 [fillcolor=blue, label=b, style=filled];\na0 -> b0  [style=bold];\nd0 [label=d];\nb0 -> d0;\ne0 [label=e];\nb0 -> e0;\ng0 [label=g];\ne0 -> g0;\nh0 [label=h];\ne0 -> h0;\nc0 [label=c];\na0 -> c0;\nf0 [label=f];\nc0 -> f0;\n}\n"""
+        actual = graph.to_string()
+        if LOCAL:
+            graph.write_png("tests/tree_attr_override.png")
         for expected_str in expected.split():
             assert (
                 expected_str in actual
             ), f"Expected {expected_str} not in actual string"
 
 
 class TestTreeToPillow:
```

### Comparing `bigtree-0.9.3/tests/tree/test_helper.py` & `bigtree-0.9.4/tests/tree/test_helper.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,88 +2,93 @@
 
 from bigtree import print_tree
 from bigtree.node.basenode import BaseNode
 from bigtree.node.node import Node
 from bigtree.tree.helper import clone_tree, get_tree_diff, prune_tree
 from bigtree.utils.exceptions import NotFoundError, SearchError
 from tests.conftest import assert_print_statement
+from tests.constants import Constants
 from tests.node.test_basenode import (
+    assert_tree_structure_basenode_root,
     assert_tree_structure_basenode_root_attr,
-    assert_tree_structure_basenode_root_generic,
 )
 
 
 class TestCloneTree:
     @staticmethod
-    def test_clone_tree_wrong_type():
-        with pytest.raises(ValueError):
+    def test_clone_tree_wrong_type_error():
+        with pytest.raises(ValueError) as exc_info:
             clone_tree({}, Node)
+        assert str(exc_info.value) == Constants.ERROR_HELPER_BASENODE_TYPE
 
     @staticmethod
     def test_clone_tree_basenode_node(tree_basenode):
         root_clone = clone_tree(tree_basenode, node_type=Node)
         assert isinstance(root_clone, Node), "Wrong type returned"
-        assert_tree_structure_basenode_root_generic(root_clone)
+        assert_tree_structure_basenode_root(root_clone)
         assert_tree_structure_basenode_root_attr(root_clone)
 
     @staticmethod
     def test_clone_tree_node_basenode(tree_node):
         root_clone = clone_tree(tree_node, node_type=BaseNode)
         assert isinstance(root_clone, BaseNode), "Wrong type returned"
-        assert_tree_structure_basenode_root_generic(root_clone)
+        assert_tree_structure_basenode_root(root_clone)
         assert_tree_structure_basenode_root_attr(root_clone)
 
     @staticmethod
     def test_clone_tree_basenode_custom(tree_basenode):
         class NodeA(Node):
             pass
 
         root_clone = clone_tree(tree_basenode, node_type=NodeA)
         assert isinstance(root_clone, NodeA), "Node type is not `NodeA`"
-        assert_tree_structure_basenode_root_generic(root_clone)
+        assert_tree_structure_basenode_root(root_clone)
         assert_tree_structure_basenode_root_attr(root_clone)
 
 
 class TestPruneTree:
     @staticmethod
     def test_prune_tree(tree_node):
         # Pruned tree is a/c/f
         tree_prune = prune_tree(tree_node, "a/c")
 
-        assert_tree_structure_basenode_root_generic(tree_node)
+        assert_tree_structure_basenode_root(tree_node)
         assert_tree_structure_basenode_root_attr(tree_node)
         assert len(list(tree_prune.children)) == 1
         assert len(tree_prune.children[0].children) == 1
 
     @staticmethod
-    def test_prune_tree_multiple_path(tree_node):
+    def test_prune_tree_multiple_path_error(tree_node):
         dd = Node("d")
         dd.parent = tree_node.children[-1]
-        with pytest.raises(SearchError):
+        with pytest.raises(SearchError) as exc_info:
             prune_tree(tree_node, "d")
+        assert str(exc_info.value).startswith(Constants.ERROR_ONE_ELEMENT)
 
     @staticmethod
-    def test_prune_tree_nonexistant_path(tree_node):
-        with pytest.raises(NotFoundError):
+    def test_prune_tree_nonexistant_path_error(tree_node):
+        with pytest.raises(NotFoundError) as exc_info:
             prune_tree(tree_node, "i")
+        assert str(exc_info.value).startswith(Constants.ERROR_NOT_FOUND)
 
     @staticmethod
     def test_prune_tree_sep(tree_node):
         # Pruned tree is a/c/f
         tree_prune = prune_tree(tree_node, "a\\c", sep="\\")
 
-        assert_tree_structure_basenode_root_generic(tree_node)
+        assert_tree_structure_basenode_root(tree_node)
         assert_tree_structure_basenode_root_attr(tree_node)
         assert len(list(tree_prune.children)) == 1
         assert len(tree_prune.children[0].children) == 1
 
     @staticmethod
-    def test_prune_tree_sep_wrong(tree_node):
-        with pytest.raises(NotFoundError):
+    def test_prune_tree_sep_error(tree_node):
+        with pytest.raises(NotFoundError) as exc_info:
             prune_tree(tree_node, "a\\c")
+        assert str(exc_info.value).startswith(Constants.ERROR_NOT_FOUND)
 
 
 class TestTreeDiff:
     @staticmethod
     def test_tree_diff(tree_node):
         other_tree_node = prune_tree(tree_node, "a/c")
         _ = Node("d", parent=other_tree_node)
```

### Comparing `bigtree-0.9.3/tests/tree/test_modify.py` & `bigtree-0.9.4/tests/tree/test_modify.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 import pytest
 
 from bigtree.node.node import Node
 from bigtree.tree.export import print_tree
 from bigtree.tree.modify import copy_nodes, copy_nodes_from_tree_to_tree, shift_nodes
 from bigtree.tree.search import find_name, find_path
 from bigtree.utils.exceptions import NotFoundError, TreeError
+from tests.constants import Constants
 from tests.node.test_basenode import (
+    assert_tree_structure_basenode_root,
     assert_tree_structure_basenode_root_attr,
-    assert_tree_structure_basenode_root_generic,
 )
-from tests.node.test_node import assert_tree_structure_node_root_generic
+from tests.node.test_node import assert_tree_structure_node_root
 
 
 class TestCopyNodes(unittest.TestCase):
     def setUp(self):
         """
         Tree should have structure
         a
@@ -113,124 +114,115 @@
         from_paths = ["d"]
         to_paths = ["a/b/c/d"]
         copy_nodes(self.root, from_paths, to_paths)
         assert self.root.max_depth == 4, "Shift did not create a tree of depth 4"
         assert find_path(self.root, "a/d"), "Original node is not there"
         assert find_path(self.root, "a/b/c/d"), "Copied node is not there"
 
-    def test_copy_nodes_invalid_type(self):
+    def test_copy_nodes_invalid_type_error(self):
         with pytest.raises(ValueError) as exc_info:
             copy_nodes(self.root, {}, [])
-        assert str(exc_info.value).startswith("Invalid type")
+        assert str(exc_info.value) == Constants.ERROR_MODIFY_TYPE
 
-    def test_copy_nodes_unequal_length(self):
+    def test_copy_nodes_unequal_length_error(self):
         from_paths = ["d", "e", "g", "h", "f"]
         to_paths = ["a/b/d"]
         with pytest.raises(ValueError) as exc_info:
             copy_nodes(self.root, from_paths, to_paths)
-        assert str(exc_info.value).startswith("Paths are different length")
+        assert str(exc_info.value).startswith(Constants.ERROR_DIFFERENT_PATH_LENGTH)
 
-    def test_copy_nodes_invalid_paths(self):
+    def test_copy_nodes_invalid_paths_error(self):
         from_paths = ["d"]
         to_paths = ["a/b/e"]
         with pytest.raises(ValueError) as exc_info:
             copy_nodes(self.root, from_paths, to_paths)
-        assert str(exc_info.value).startswith("Unable to assign")
+        assert str(exc_info.value).startswith(Constants.ERROR_PATH_MISMATCH)
 
-    def test_copy_nodes_invalid_from_paths(self):
+    def test_copy_nodes_invalid_from_paths_error(self):
         from_paths = ["i"]
         to_paths = ["a/b/i"]
         with pytest.raises(NotFoundError) as exc_info:
             copy_nodes(self.root, from_paths, to_paths)
-        assert str(exc_info.value).startswith("Unable to find from_path")
+        assert str(exc_info.value).startswith(Constants.ERROR_FROM_PATH_NOT_FOUND)
 
-    def test_copy_nodes_invalid_to_paths(self):
+    def test_copy_nodes_invalid_to_paths_error(self):
         from_paths = ["d"]
         to_paths = ["aa/b/d"]
         with pytest.raises(ValueError) as exc_info:
             copy_nodes(self.root, from_paths, to_paths)
-        assert str(exc_info.value).startswith(
-            "Invalid path in `to_paths` not starting with the root node"
-        )
+        assert str(exc_info.value) == Constants.ERROR_INVALID_TO_PATH
 
     def test_copy_nodes_create_intermediate_path(self):
         from_paths = ["d"]
         to_paths = ["a/b/c/d"]
         copy_nodes(self.root, from_paths, to_paths)
         assert self.root.max_depth == 4, "Shift did not create a tree of depth 4"
 
     def test_copy_nodes_delete_error(self):
         from_paths = ["d"]
         to_paths = [None]
         with pytest.raises(ValueError) as exc_info:
             copy_nodes(self.root, from_paths, to_paths)
-        assert (
-            str(exc_info.value)
-            == "Deletion of node will not happen if `copy=True`, check your `copy` parameter."
-        )
+        assert str(exc_info.value) == Constants.ERROR_DELETION_AND_COPY
 
-    def test_copy_nodes_delete_error2(self):
         from_paths = ["d"]
         to_paths = [""]
         with pytest.raises(ValueError) as exc_info:
             copy_nodes(self.root, from_paths, to_paths)
-        assert (
-            str(exc_info.value)
-            == "Deletion of node will not happen if `copy=True`, check your `copy` parameter."
-        )
+        assert str(exc_info.value) == Constants.ERROR_DELETION_AND_COPY
 
     # sep
     def test_copy_nodes_leading_sep(self):
         from_paths = ["/d", "e", "g", "/h", "/f"]
         to_paths = ["/a/b/d", "a/b/e", "/a/b/e/g", "a/b/e/h", "/a/c/f"]
         copy_nodes(self.root, from_paths, to_paths)
 
         # Delete original nodes
         from_paths = ["/a/d", "/a/e", "/a/g", "/a/h", "/a/f"]
         to_paths = [None, None, None, None, None]
         shift_nodes(self.root, from_paths, to_paths)
 
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
         assert_tree_structure_basenode_root_attr(self.root)
-        assert_tree_structure_node_root_generic(self.root)
+        assert_tree_structure_node_root(self.root)
 
     def test_copy_nodes_trailing_sep(self):
         from_paths = ["d", "e/", "g/", "h", "f/"]
         to_paths = ["a/b/d", "a/b/e/", "a/b/e/g/", "a/b/e/h/", "a/c/f"]
         copy_nodes(self.root, from_paths, to_paths)
 
         # Delete original nodes
         from_paths = ["/a/d", "/a/e", "/a/g", "/a/h", "/a/f"]
         to_paths = [None, None, None, None, None]
         shift_nodes(self.root, from_paths, to_paths)
 
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
         assert_tree_structure_basenode_root_attr(self.root)
-        assert_tree_structure_node_root_generic(self.root)
+        assert_tree_structure_node_root(self.root)
 
-    def test_copy_nodes_sep_undefined(self):
+    def test_copy_nodes_sep_error(self):
         from_paths = ["\\d", "\\e", "\\g", "\\h", "\\f"]
         to_paths = ["a\\b\\d", "a\\b\\e", "a\\b\\e\\g", "a\\b\\e\\h", "a\\c\\f"]
         with pytest.raises(ValueError) as exc_info:
             copy_nodes(self.root, from_paths, to_paths)
-        assert str(exc_info.value).startswith("Unable to assign from_path")
+        assert str(exc_info.value).startswith(Constants.ERROR_PATH_MISMATCH)
 
     def test_copy_nodes_sep(self):
         from_paths = ["\\d", "\\e", "\\g", "\\h", "\\f"]
         to_paths = ["a\\b\\d", "a\\b\\e", "a\\b\\e\\g", "a\\b\\e\\h", "a\\c\\f"]
         copy_nodes(self.root, from_paths, to_paths, sep="\\")
 
         # Delete original nodes
         from_paths = ["\\a\\d", "\\a\\e", "\\a\\g", "\\a\\h", "\\a\\f"]
         to_paths = [None, None, None, None, None]
         shift_nodes(self.root, from_paths, to_paths, sep="\\")
 
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
         assert_tree_structure_basenode_root_attr(self.root)
-        assert_tree_structure_node_root_generic(self.root)
+        assert_tree_structure_node_root(self.root)
 
     def test_copy_nodes_sep_different(self):
         # Delete intermediate nodes
         from_paths = ["\\a\\b", "\\a\\c", "\\a\\e"]
         to_paths = [None, None, None]
         shift_nodes(self.root, from_paths, to_paths, sep="\\")
 
@@ -240,34 +232,35 @@
         copy_nodes(self.root, from_paths, to_paths, sep="\\")
 
         # Delete original nodes
         from_paths = ["\\a\\d", "\\a\\g", "\\a\\h", "\\a\\f"]
         to_paths = [None, None, None, None]
         shift_nodes(self.root, from_paths, to_paths, sep="\\")
 
-        assert_tree_structure_basenode_root_generic(self.root)
-        assert_tree_structure_node_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
+        assert_tree_structure_node_root(self.root)
 
     # skippable
-    def test_copy_nodes_skippable(self):
+    def test_copy_nodes_skippable_error(self):
         from_paths = ["i", "d", "e", "g", "h", "f"]
         to_paths = ["a/c/f/i", "a/b/d", "a/b/e", "a/b/e/g", "a/b/e/h", "a/c/f"]
-        with pytest.raises(NotFoundError):
+        with pytest.raises(NotFoundError) as exc_info:
             copy_nodes(self.root, from_paths, to_paths)
+        assert str(exc_info.value).startswith(Constants.ERROR_FROM_PATH_NOT_FOUND)
 
         copy_nodes(self.root, from_paths, to_paths, skippable=True)
 
         # Delete original nodes
         from_paths = ["a/d", "a/e", "a/g", "a/h", "a/f"]
         to_paths = [None, None, None, None, None]
         shift_nodes(self.root, from_paths, to_paths)
 
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
         assert_tree_structure_basenode_root_attr(self.root)
-        assert_tree_structure_node_root_generic(self.root)
+        assert_tree_structure_node_root(self.root)
 
     # overriding
     def test_copy_nodes_delete_and_overriding_error(self):
         new_aa = Node("aa", parent=self.root)
         new_d = Node("d")
         new_d.parent = new_aa
         from_paths = ["/a/d", "aa/d", "e", "g", "h", "f"]
@@ -287,17 +280,17 @@
         copy_nodes(self.root, from_paths, to_paths, overriding=True)
 
         # Delete original nodes
         from_paths = ["a/aa", "a/d", "a/e", "a/g", "a/h", "a/f"]
         to_paths = [None, None, None, None, None, None]
         shift_nodes(self.root, from_paths, to_paths)
 
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
         assert_tree_structure_basenode_root_attr(self.root, d=("d", 1))
-        assert_tree_structure_node_root_generic(self.root)
+        assert_tree_structure_node_root(self.root)
 
     def test_copy_nodes_overriding(self):
         from_paths = ["a/aa/bb"]
         to_paths = ["/a/bb"]
         copy_nodes(
             self.root_overriding,
             from_paths,
@@ -354,22 +347,22 @@
         cc = Node("cc")
         cc.parent = bb
 
         from_paths = ["aa/bb"]
         to_paths = ["/a/bb"]
         with pytest.raises(TreeError) as exc_info:
             copy_nodes(self.root_overriding, from_paths, to_paths, merge_children=True)
-        assert str(exc_info.value).startswith("Error: Duplicate node with same path")
+        assert str(exc_info.value).startswith(Constants.ERROR_SAME_PATH)
 
     def test_copy_nodes_same_node_error(self):
         from_paths = ["d"]
         to_paths = ["a/d"]
         with pytest.raises(TreeError) as exc_info:
             copy_nodes(self.root, from_paths, to_paths)
-        assert str(exc_info.value).startswith("Attempting to shift the same node")
+        assert str(exc_info.value).startswith(Constants.ERROR_SHIFT_SAME_NODE)
 
     def test_copy_nodes_same_node_merge_children(self):
         from_paths = ["d", "e", "g", "h", "f"]
         to_paths = ["a/b/d", "a/b/e", "a/b/e/g", "a/b/e/h", "a/c/f"]
         shift_nodes(self.root, from_paths, to_paths)
 
         from_paths = ["b"]
@@ -418,15 +411,15 @@
         dd = Node("dd")
         dd.parent = bb
 
         from_paths = ["a/aa"]
         to_paths = ["/a/bb/aa"]
         with pytest.raises(TreeError) as exc_info:
             copy_nodes(self.root_overriding, from_paths, to_paths, merge_leaves=True)
-        assert str(exc_info.value).startswith("Error: Duplicate node with same path")
+        assert str(exc_info.value).startswith(Constants.ERROR_SAME_PATH)
 
     def test_copy_nodes_same_node_merge_leaves(self):
         a = Node("a", age=90)
         self.root_other.parent = a
 
         from_paths = ["a/aa/d", "a/aa/e", "a/aa/g", "a/aa/h", "a/aa/f"]
         to_paths = ["a/aa/b/d", "a/aa/b/e", "a/aa/b/e/g", "a/aa/b/e/h", "a/aa/c/f"]
@@ -459,17 +452,17 @@
         copy_nodes(self.root, from_paths, to_paths, delete_children=True)
 
         # Delete original nodes
         from_paths = ["a/d", "a/e", "a/g", "a/h", "a/f"]
         to_paths = [None, None, None, None, None]
         shift_nodes(self.root, from_paths, to_paths)
 
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
         assert_tree_structure_basenode_root_attr(self.root)
-        assert_tree_structure_node_root_generic(self.root)
+        assert_tree_structure_node_root(self.root)
 
     # merge_children, overriding
     def test_copy_nodes_merge_children_overriding(self):
         new_aa = Node("aa", parent=self.root)
         new_bb = Node("bb", parent=new_aa)
         new_cc = Node("cc", age=1)
         new_cc.parent = new_bb
@@ -542,17 +535,15 @@
         to_paths = ["a/aa/b/d", "a/aa/b/e", "a/aa/b/e/g", "a/aa/b/e/h", "a/aa/c/f"]
         shift_nodes(a, from_paths, to_paths)
 
         from_paths = ["a/aa"]
         to_paths = ["a/bb/aa"]
         with pytest.raises(ValueError) as exc_info:
             copy_nodes(a, from_paths, to_paths, merge_children=True, merge_leaves=True)
-        assert str(exc_info.value).startswith(
-            "Invalid shifting, can only specify one type of merging"
-        )
+        assert str(exc_info.value) == Constants.ERROR_MERGE_CHILDREN_OR_LEAVES
 
     # merge_children, delete_children
     def test_copy_nodes_merge_children_and_delete_children(self):
         from_paths = ["d", "e", "g", "f"]
         to_paths = ["a/b/d", "a/b/e", "a/b/e/g", "a/c/f"]
         shift_nodes(self.root, from_paths, to_paths)
 
@@ -567,58 +558,56 @@
         )
 
         # Delete original nodes
         from_paths = ["a/h"]
         to_paths = [None]
         shift_nodes(self.root, from_paths, to_paths)
 
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
         assert_tree_structure_basenode_root_attr(self.root)
-        assert_tree_structure_node_root_generic(self.root)
+        assert_tree_structure_node_root(self.root)
 
     # merge_leaves, delete_children
     def test_copy_nodes_merge_leaves_and_delete_children(self):
         from_paths = ["d", "e", "g", "f", "h"]
         to_paths = ["a/b/d", "a/b/e", "a/b/e/g", "a/c/f", "a/i/j/k/h"]
         shift_nodes(self.root, from_paths, to_paths)
 
         from_paths = ["a/i"]
         to_paths = ["a/b/e/i"]
         copy_nodes(
             self.root, from_paths, to_paths, merge_leaves=True, delete_children=True
         )
         i = find_path(self.root, "a/i")
         i.parent = None
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
         assert_tree_structure_basenode_root_attr(self.root)
-        assert_tree_structure_node_root_generic(self.root)
+        assert_tree_structure_node_root(self.root)
 
     # with_full_path
     def test_copy_nodes_with_full_path(self):
         from_paths = ["a/d", "a/e", "a/g", "a/h", "a/f"]
         to_paths = ["a/b/d", "a/b/e", "a/b/e/g", "a/b/e/h", "a/c/f"]
         copy_nodes(self.root, from_paths, to_paths, with_full_path=True)
 
         # Delete original nodes
         from_paths = ["a/d", "a/e", "a/g", "a/h", "a/f"]
         to_paths = [None, None, None, None, None]
         shift_nodes(self.root, from_paths, to_paths, with_full_path=True)
 
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
         assert_tree_structure_basenode_root_attr(self.root)
-        assert_tree_structure_node_root_generic(self.root)
+        assert_tree_structure_node_root(self.root)
 
     def test_copy_nodes_with_full_path_error(self):
         from_paths = ["d", "e", "g", "h", "f"]
         to_paths = ["a/b/d", "a/b/e", "a/b/e/g", "a/b/e/h", "a/c/f"]
         with pytest.raises(ValueError) as exc_info:
             copy_nodes(self.root, from_paths, to_paths, with_full_path=True)
-        assert str(exc_info.value).startswith(
-            "Invalid path in `from_paths` not starting with the root node"
-        )
+        assert str(exc_info.value).startswith(Constants.ERROR_INVALID_FULL_PATH)
 
 
 class TestShiftNodes(unittest.TestCase):
     def setUp(self):
         """
         Tree should have structure
         a
@@ -712,102 +701,101 @@
     def tearDown(self):
         self.root = None
 
     def test_shift_nodes(self):
         from_paths = ["d", "e", "g", "h", "f"]
         to_paths = ["a/b/d", "a/b/e", "a/b/e/g", "a/b/e/h", "a/c/f"]
         shift_nodes(self.root, from_paths, to_paths)
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
         assert_tree_structure_basenode_root_attr(self.root)
-        assert_tree_structure_node_root_generic(self.root)
+        assert_tree_structure_node_root(self.root)
 
-    def test_shift_nodes_invalid_type(self):
+    def test_shift_nodes_invalid_type_error(self):
         with pytest.raises(ValueError) as exc_info:
             shift_nodes(self.root, {}, [])
-        assert str(exc_info.value).startswith("Invalid type")
+        assert str(exc_info.value) == Constants.ERROR_MODIFY_TYPE
 
-    def test_shift_nodes_unequal_length(self):
+    def test_shift_nodes_unequal_length_error(self):
         from_paths = ["d", "e", "g", "h", "f"]
         to_paths = ["a/b/d"]
         with pytest.raises(ValueError) as exc_info:
             shift_nodes(self.root, from_paths, to_paths)
-        assert str(exc_info.value).startswith("Paths are different length")
+        assert str(exc_info.value).startswith(Constants.ERROR_DIFFERENT_PATH_LENGTH)
 
-    def test_shift_nodes_invalid_paths(self):
+    def test_shift_nodes_invalid_paths_error(self):
         from_paths = ["d"]
         to_paths = ["a/b/e"]
         with pytest.raises(ValueError) as exc_info:
             shift_nodes(self.root, from_paths, to_paths)
-        assert str(exc_info.value).startswith("Unable to assign")
+        assert str(exc_info.value).startswith(Constants.ERROR_PATH_MISMATCH)
 
-    def test_shift_nodes_invalid_from_paths(self):
+    def test_shift_nodes_invalid_from_paths_error(self):
         from_paths = ["i"]
         to_paths = ["a/b/i"]
         with pytest.raises(NotFoundError) as exc_info:
             shift_nodes(self.root, from_paths, to_paths)
-        assert str(exc_info.value).startswith("Unable to find from_path")
+        assert str(exc_info.value).startswith(Constants.ERROR_FROM_PATH_NOT_FOUND)
 
-    def test_shift_nodes_invalid_to_paths(self):
+    def test_shift_nodes_invalid_to_paths_error(self):
         from_paths = ["d"]
         to_paths = ["aa/b/d"]
         with pytest.raises(ValueError) as exc_info:
             shift_nodes(self.root, from_paths, to_paths)
-        assert str(exc_info.value).startswith(
-            "Invalid path in `to_paths` not starting with the root node"
-        )
+        assert str(exc_info.value) == Constants.ERROR_INVALID_TO_PATH
 
     def test_shift_nodes_create_intermediate_path(self):
         from_paths = ["d"]
         to_paths = ["a/b/c/d"]
         shift_nodes(self.root, from_paths, to_paths)
         assert self.root.max_depth == 4, "Shift did not create a tree of depth 4"
 
     # sep
     def test_shift_nodes_leading_sep(self):
         from_paths = ["/d", "e", "g", "/h", "/f"]
         to_paths = ["/a/b/d", "a/b/e", "/a/b/e/g", "a/b/e/h", "/a/c/f"]
         shift_nodes(self.root, from_paths, to_paths)
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
         assert_tree_structure_basenode_root_attr(self.root)
-        assert_tree_structure_node_root_generic(self.root)
+        assert_tree_structure_node_root(self.root)
 
     def test_shift_nodes_trailing_sep(self):
         from_paths = ["d/", "e", "g/", "h", "f/"]
         to_paths = ["a/b/d/", "a/b/e", "a/b/e/g", "a/b/e/h/", "a/c/f/"]
         shift_nodes(self.root, from_paths, to_paths)
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
         assert_tree_structure_basenode_root_attr(self.root)
-        assert_tree_structure_node_root_generic(self.root)
+        assert_tree_structure_node_root(self.root)
 
-    def test_shift_nodes_sep_undefined(self):
+    def test_shift_nodes_sep_error(self):
         from_paths = ["\\d", "\\e", "\\g", "\\h", "\\f"]
         to_paths = ["a\\b\\d", "a\\b\\e", "a\\b\\e\\g", "a\\b\\e\\h", "a\\c\\f"]
         with pytest.raises(ValueError) as exc_info:
             shift_nodes(self.root, from_paths, to_paths)
-        assert str(exc_info.value).startswith("Unable to assign from_path")
+        assert str(exc_info.value).startswith(Constants.ERROR_PATH_MISMATCH)
 
     def test_shift_nodes_sep(self):
         from_paths = ["\\d", "\\e", "\\g", "\\h", "\\f"]
         to_paths = ["a\\b\\d", "a\\b\\e", "a\\b\\e\\g", "a\\b\\e\\h", "a\\c\\f"]
         shift_nodes(self.root, from_paths, to_paths, sep="\\")
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
         assert_tree_structure_basenode_root_attr(self.root)
-        assert_tree_structure_node_root_generic(self.root)
+        assert_tree_structure_node_root(self.root)
 
     # skippable
-    def test_shift_nodes_skippable(self):
+    def test_shift_nodes_skippable_error(self):
         from_paths = ["i", "d", "e", "g", "h", "f"]
         to_paths = ["a/c/f/i", "a/b/d", "a/b/e", "a/b/e/g", "a/b/e/h", "a/c/f"]
-        with pytest.raises(NotFoundError):
+        with pytest.raises(NotFoundError) as exc_info:
             shift_nodes(self.root, from_paths, to_paths)
+        assert str(exc_info.value).startswith(Constants.ERROR_FROM_PATH_NOT_FOUND)
 
         shift_nodes(self.root, from_paths, to_paths, skippable=True)
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
         assert_tree_structure_basenode_root_attr(self.root)
-        assert_tree_structure_node_root_generic(self.root)
+        assert_tree_structure_node_root(self.root)
 
     # overriding
     def test_shift_nodes_delete_and_overriding_error(self):
         new_aa = Node("aa", parent=self.root)
         new_d = Node("d")
         new_d.parent = new_aa
         from_paths = ["/a/d", "aa/d", "e", "g", "h", "f", "a/aa"]
@@ -821,17 +809,17 @@
     def test_shift_nodes_delete_and_overriding(self):
         new_aa = Node("aa", parent=self.root)
         new_d = Node("d", age=1)
         new_d.parent = new_aa
         from_paths = ["/a/d", "aa/d", "e", "g", "h", "f", "a/aa"]
         to_paths = ["a/b/d", "a/b/d", "a/b/e", "a/b/e/g", "a/b/e/h", "a/c/f", None]
         shift_nodes(self.root, from_paths, to_paths, overriding=True)
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
         assert_tree_structure_basenode_root_attr(self.root, d=("d", 1))
-        assert_tree_structure_node_root_generic(self.root)
+        assert_tree_structure_node_root(self.root)
 
     def test_shift_nodes_overriding(self):
         from_paths = ["a/aa/bb"]
         to_paths = ["/a/bb"]
         shift_nodes(
             self.root_overriding,
             from_paths,
@@ -886,22 +874,22 @@
         cc = Node("cc")
         cc.parent = bb
 
         from_paths = ["aa/bb"]
         to_paths = ["/a/bb"]
         with pytest.raises(TreeError) as exc_info:
             shift_nodes(self.root_overriding, from_paths, to_paths, merge_children=True)
-        assert str(exc_info.value).startswith("Error: Duplicate node with same path")
+        assert str(exc_info.value).startswith(Constants.ERROR_SAME_PATH)
 
     def test_shift_nodes_same_node_error(self):
         from_paths = ["d"]
         to_paths = ["a/d"]
         with pytest.raises(TreeError) as exc_info:
             shift_nodes(self.root, from_paths, to_paths)
-        assert str(exc_info.value).startswith("Attempting to shift the same node")
+        assert str(exc_info.value).startswith(Constants.ERROR_SHIFT_SAME_NODE)
 
     def test_shift_nodes_same_node_merge_children(self):
         from_paths = ["d", "e", "g", "h", "f"]
         to_paths = ["a/b/d", "a/b/e", "a/b/e/g", "a/b/e/h", "a/c/f"]
         shift_nodes(self.root, from_paths, to_paths)
 
         from_paths = ["b"]
@@ -950,15 +938,15 @@
         dd = Node("dd")
         dd.parent = bb
 
         from_paths = ["a/aa"]
         to_paths = ["/a/bb/aa"]
         with pytest.raises(TreeError) as exc_info:
             shift_nodes(self.root_overriding, from_paths, to_paths, merge_leaves=True)
-        assert str(exc_info.value).startswith("Error: Duplicate node with same path")
+        assert str(exc_info.value).startswith(Constants.ERROR_SAME_PATH)
 
     def test_shift_nodes_same_node_merge_leaves(self):
         a = Node("a", age=90)
         self.root_other.parent = a
 
         from_paths = ["a/aa/d", "a/aa/e", "a/aa/g", "a/aa/h", "a/aa/f"]
         to_paths = ["a/aa/b/d", "a/aa/b/e", "a/aa/b/e/g", "a/aa/b/e/h", "a/aa/c/f"]
@@ -988,17 +976,17 @@
         g = find_name(self.root, "g")
         h = find_name(self.root, "h")
         g.children = [Node("i"), Node("j")]
         h.children = [Node("i"), Node("j")]
         from_paths = ["d", "e", "g", "h", "f"]
         to_paths = ["a/b/d", "a/b/e", "a/b/e/g", "a/b/e/h", "a/c/f"]
         shift_nodes(self.root, from_paths, to_paths, delete_children=True)
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
         assert_tree_structure_basenode_root_attr(self.root)
-        assert_tree_structure_node_root_generic(self.root)
+        assert_tree_structure_node_root(self.root)
 
     # merge_children, overriding
     def test_shift_nodes_merge_children_overriding(self):
         new_aa = Node("aa", parent=self.root)
         new_bb = Node("bb", parent=new_aa)
         new_cc = Node("cc", age=1)
         new_cc.parent = new_bb
@@ -1073,17 +1061,15 @@
         to_paths = ["a/aa/b/d", "a/aa/b/e", "a/aa/b/e/g", "a/aa/b/e/h", "a/aa/c/f"]
         shift_nodes(a, from_paths, to_paths)
 
         from_paths = ["a/aa"]
         to_paths = ["a/bb/aa"]
         with pytest.raises(ValueError) as exc_info:
             shift_nodes(a, from_paths, to_paths, merge_children=True, merge_leaves=True)
-        assert str(exc_info.value).startswith(
-            "Invalid shifting, can only specify one type of merging"
-        )
+        assert str(exc_info.value) == Constants.ERROR_MERGE_CHILDREN_OR_LEAVES
 
     # merge_children, delete_children
     def test_shift_nodes_merge_children_and_delete_children(self):
         from_paths = ["d", "e", "g", "f"]
         to_paths = ["a/b/d", "a/b/e", "a/b/e/g", "a/c/f"]
         shift_nodes(self.root, from_paths, to_paths)
 
@@ -1092,53 +1078,51 @@
         h = find_name(self.root, "h")
         h2.parent = h
         from_paths = ["a/h"]
         to_paths = ["a/b/e/h"]
         shift_nodes(
             self.root, from_paths, to_paths, merge_children=True, delete_children=True
         )
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
         assert_tree_structure_basenode_root_attr(self.root)
-        assert_tree_structure_node_root_generic(self.root)
+        assert_tree_structure_node_root(self.root)
 
     # merge_leaves, delete_children
     def test_shift_nodes_merge_leaves_and_delete_children(self):
         from_paths = ["d", "e", "g", "f", "h"]
         to_paths = ["a/b/d", "a/b/e", "a/b/e/g", "a/c/f", "a/i/j/k/h"]
         shift_nodes(self.root, from_paths, to_paths)
 
         from_paths = ["a/i"]
         to_paths = ["a/b/e/i"]
         shift_nodes(
             self.root, from_paths, to_paths, merge_leaves=True, delete_children=True
         )
         i = find_path(self.root, "a/i")
         i.parent = None
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
         assert_tree_structure_basenode_root_attr(self.root)
-        assert_tree_structure_node_root_generic(self.root)
+        assert_tree_structure_node_root(self.root)
 
     # with_full_path
     def test_shift_nodes_with_full_path(self):
         from_paths = ["a/d", "a/e", "a/g", "a/h", "a/f"]
         to_paths = ["a/b/d", "a/b/e", "a/b/e/g", "a/b/e/h", "a/c/f"]
         shift_nodes(self.root, from_paths, to_paths, with_full_path=True)
 
-        assert_tree_structure_basenode_root_generic(self.root)
+        assert_tree_structure_basenode_root(self.root)
         assert_tree_structure_basenode_root_attr(self.root)
-        assert_tree_structure_node_root_generic(self.root)
+        assert_tree_structure_node_root(self.root)
 
     def test_shift_nodes_with_full_path_error(self):
         from_paths = ["d", "e", "g", "h", "f"]
         to_paths = ["a/b/d", "a/b/e", "a/b/e/g", "a/b/e/h", "a/c/f"]
         with pytest.raises(ValueError) as exc_info:
             shift_nodes(self.root, from_paths, to_paths, with_full_path=True)
-        assert str(exc_info.value).startswith(
-            "Invalid path in `from_paths` not starting with the root node"
-        )
+        assert str(exc_info.value).startswith(Constants.ERROR_INVALID_FULL_PATH)
 
 
 class TestCopyNodesTwoTrees(unittest.TestCase):
     def setUp(self):
         """
         Tree should have structure
         a
@@ -1223,90 +1207,88 @@
         to_paths = ["a/b", "a/c", "a/b/d", "a/b/e", "a/c/f", "a/b/e/g", "a/b/e/h"]
         copy_nodes_from_tree_to_tree(
             from_tree=self.root,
             to_tree=self.root_other,
             from_paths=from_paths,
             to_paths=to_paths,
         )
-        assert_tree_structure_basenode_root_generic(self.root_other)
+        assert_tree_structure_basenode_root(self.root_other)
         assert_tree_structure_basenode_root_attr(self.root_other)
-        assert_tree_structure_node_root_generic(self.root_other)
+        assert_tree_structure_node_root(self.root_other)
         assert self.root.max_depth == 2, "Copying changes original tree"
 
-    def test_copy_nodes_from_tree_to_tree_reversed_error(self):
+    def test_copy_nodes_from_tree_to_tree_reverse_error(self):
         from_paths = ["b", "c", "d", "e", "f", "g", "h"][::-1]
         to_paths = ["a/b", "a/c", "a/b/d", "a/b/e", "a/c/f", "a/b/e/g", "a/b/e/h"][::-1]
         with pytest.raises(TreeError) as exc_info:
             copy_nodes_from_tree_to_tree(
                 from_tree=self.root,
                 to_tree=self.root_other,
                 from_paths=from_paths,
                 to_paths=to_paths,
             )
         assert "already exists and unable to override" in str(exc_info.value)
 
-    def test_copy_nodes_from_tree_to_tree_invalid_type(self):
+    def test_copy_nodes_from_tree_to_tree_invalid_type_error(self):
         with pytest.raises(ValueError) as exc_info:
             copy_nodes_from_tree_to_tree(
                 from_tree=self.root,
                 to_tree=self.root_other,
                 from_paths={},
                 to_paths=[],
             )
-        assert str(exc_info.value).startswith("Invalid type")
+        assert str(exc_info.value) == Constants.ERROR_MODIFY_TYPE
 
-    def test_copy_nodes_from_tree_to_tree_unequal_length(self):
+    def test_copy_nodes_from_tree_to_tree_unequal_length_error(self):
         from_paths = ["d", "e", "g", "h", "f"]
         to_paths = ["a/b/d"]
         with pytest.raises(ValueError) as exc_info:
             copy_nodes_from_tree_to_tree(
                 from_tree=self.root,
                 to_tree=self.root_other,
                 from_paths=from_paths,
                 to_paths=to_paths,
             )
-        assert str(exc_info.value).startswith("Paths are different length")
+        assert str(exc_info.value).startswith(Constants.ERROR_DIFFERENT_PATH_LENGTH)
 
-    def test_copy_nodes_from_tree_to_tree_invalid_paths(self):
+    def test_copy_nodes_from_tree_to_tree_invalid_paths_error(self):
         from_paths = ["d"]
         to_paths = ["a/b/e"]
         with pytest.raises(ValueError) as exc_info:
             copy_nodes_from_tree_to_tree(
                 from_tree=self.root,
                 to_tree=self.root_other,
                 from_paths=from_paths,
                 to_paths=to_paths,
             )
-        assert str(exc_info.value).startswith("Unable to assign")
+        assert str(exc_info.value).startswith(Constants.ERROR_PATH_MISMATCH)
 
-    def test_copy_nodes_from_tree_to_tree_invalid_from_paths(self):
+    def test_copy_nodes_from_tree_to_tree_invalid_from_paths_error(self):
         from_paths = ["i"]
         to_paths = ["a/b/i"]
         with pytest.raises(NotFoundError) as exc_info:
             copy_nodes_from_tree_to_tree(
                 from_tree=self.root,
                 to_tree=self.root_other,
                 from_paths=from_paths,
                 to_paths=to_paths,
             )
-        assert str(exc_info.value).startswith("Unable to find from_path")
+        assert str(exc_info.value).startswith(Constants.ERROR_FROM_PATH_NOT_FOUND)
 
-    def test_copy_nodes_from_tree_to_tree_invalid_to_paths(self):
+    def test_copy_nodes_from_tree_to_tree_invalid_to_paths_error(self):
         from_paths = ["d"]
         to_paths = ["aa/b/d"]
         with pytest.raises(ValueError) as exc_info:
             copy_nodes_from_tree_to_tree(
                 from_tree=self.root,
                 to_tree=self.root_other,
                 from_paths=from_paths,
                 to_paths=to_paths,
             )
-        assert str(exc_info.value).startswith(
-            "Invalid path in `to_paths` not starting with the root node"
-        )
+        assert str(exc_info.value) == Constants.ERROR_INVALID_TO_PATH
 
     def test_copy_nodes_create_intermediate_path(self):
         from_paths = ["d"]
         to_paths = ["a/b/c/d"]
         copy_nodes_from_tree_to_tree(
             from_tree=self.root,
             to_tree=self.root_other,
@@ -1321,33 +1303,26 @@
         with pytest.raises(ValueError) as exc_info:
             copy_nodes_from_tree_to_tree(
                 from_tree=self.root,
                 to_tree=self.root_other,
                 from_paths=from_paths,
                 to_paths=to_paths,
             )
-        assert (
-            str(exc_info.value)
-            == "Deletion of node will not happen if `copy=True`, check your `copy` parameter."
-        )
+        assert str(exc_info.value) == Constants.ERROR_DELETION_AND_COPY
 
-    def test_copy_nodes_from_tree_to_tree_delete_error2(self):
         from_paths = ["d"]
         to_paths = [""]
         with pytest.raises(ValueError) as exc_info:
             copy_nodes_from_tree_to_tree(
                 from_tree=self.root,
                 to_tree=self.root_other,
                 from_paths=from_paths,
                 to_paths=to_paths,
             )
-        assert (
-            str(exc_info.value)
-            == "Deletion of node will not happen if `copy=True`, check your `copy` parameter."
-        )
+        assert str(exc_info.value) == Constants.ERROR_DELETION_AND_COPY
 
     # sep
     def test_copy_nodes_from_tree_to_tree_leading_sep(self):
         from_paths = ["/b", "c", "/d", "e", "g", "h", "f"]
         to_paths = [
             "/a/b",
             "a/c",
@@ -1360,17 +1335,17 @@
         copy_nodes_from_tree_to_tree(
             from_tree=self.root,
             to_tree=self.root_other,
             from_paths=from_paths,
             to_paths=to_paths,
         )
 
-        assert_tree_structure_basenode_root_generic(self.root_other)
+        assert_tree_structure_basenode_root(self.root_other)
         assert_tree_structure_basenode_root_attr(self.root_other)
-        assert_tree_structure_node_root_generic(self.root_other)
+        assert_tree_structure_node_root(self.root_other)
 
     def test_copy_nodes_from_tree_to_tree_different_sep(self):
         from_paths = ["b/", "c", "d/", "e", "g", "h", "f"]
         to_paths = [
             "a/b/",
             "a/c",
             "a/b/d",
@@ -1384,17 +1359,17 @@
             from_tree=self.root,
             to_tree=self.root_other,
             from_paths=from_paths,
             to_paths=to_paths,
         )
         self.root_other.sep = "/"
 
-        assert_tree_structure_basenode_root_generic(self.root_other)
+        assert_tree_structure_basenode_root(self.root_other)
         assert_tree_structure_basenode_root_attr(self.root_other)
-        assert_tree_structure_node_root_generic(self.root_other)
+        assert_tree_structure_node_root(self.root_other)
 
     def test_copy_nodes_from_tree_to_tree_trailing_sep(self):
         from_paths = ["b/", "c", "d/", "e", "g", "h", "f"]
         to_paths = [
             "a/b/",
             "a/c",
             "a/b/d",
@@ -1406,29 +1381,29 @@
         copy_nodes_from_tree_to_tree(
             from_tree=self.root,
             to_tree=self.root_other,
             from_paths=from_paths,
             to_paths=to_paths,
         )
 
-        assert_tree_structure_basenode_root_generic(self.root_other)
+        assert_tree_structure_basenode_root(self.root_other)
         assert_tree_structure_basenode_root_attr(self.root_other)
-        assert_tree_structure_node_root_generic(self.root_other)
+        assert_tree_structure_node_root(self.root_other)
 
-    def test_copy_nodes_from_tree_to_tree_sep_undefined(self):
+    def test_copy_nodes_from_tree_to_tree_sep_error(self):
         from_paths = ["\\d", "\\e", "\\g", "\\h", "\\f"]
         to_paths = ["a\\b\\d", "a\\b\\e", "a\\b\\e\\g", "a\\b\\e\\h", "a\\c\\f"]
         with pytest.raises(ValueError) as exc_info:
             copy_nodes_from_tree_to_tree(
                 from_tree=self.root,
                 to_tree=self.root_other,
                 from_paths=from_paths,
                 to_paths=to_paths,
             )
-        assert str(exc_info.value).startswith("Unable to assign from_path")
+        assert str(exc_info.value).startswith(Constants.ERROR_PATH_MISMATCH)
 
     def test_copy_nodes_from_tree_to_tree_sep(self):
         from_paths = ["\\b", "\\c", "\\d", "\\e", "\\g", "\\h", "\\f"]
         to_paths = [
             "a\\b",
             "a\\c",
             "a\\b\\d",
@@ -1441,50 +1416,51 @@
             from_tree=self.root,
             to_tree=self.root_other,
             from_paths=from_paths,
             to_paths=to_paths,
             sep="\\",
         )
 
-        assert_tree_structure_basenode_root_generic(self.root_other)
+        assert_tree_structure_basenode_root(self.root_other)
         assert_tree_structure_basenode_root_attr(self.root_other)
-        assert_tree_structure_node_root_generic(self.root_other)
+        assert_tree_structure_node_root(self.root_other)
 
     # skippable
-    def test_copy_nodes_skippable(self):
+    def test_copy_nodes_skippable_error(self):
         from_paths = ["i", "b", "c", "d", "e", "g", "h", "f"]
         to_paths = [
             "a/c/f/i",
             "a/b",
             "a/c",
             "a/b/d",
             "a/b/e",
             "a/b/e/g",
             "a/b/e/h",
             "a/c/f",
         ]
-        with pytest.raises(NotFoundError):
+        with pytest.raises(NotFoundError) as exc_info:
             copy_nodes_from_tree_to_tree(
                 from_tree=self.root,
                 to_tree=self.root_other,
                 from_paths=from_paths,
                 to_paths=to_paths,
             )
+        assert str(exc_info.value).startswith(Constants.ERROR_FROM_PATH_NOT_FOUND)
 
         copy_nodes_from_tree_to_tree(
             from_tree=self.root,
             to_tree=self.root_other,
             from_paths=from_paths,
             to_paths=to_paths,
             skippable=True,
         )
 
-        assert_tree_structure_basenode_root_generic(self.root_other)
+        assert_tree_structure_basenode_root(self.root_other)
         assert_tree_structure_basenode_root_attr(self.root_other)
-        assert_tree_structure_node_root_generic(self.root_other)
+        assert_tree_structure_node_root(self.root_other)
 
     # overriding
     def test_copy_nodes_from_tree_to_tree_delete_and_overriding_error(self):
         new_aa = Node("aa", parent=self.root)
         new_d = Node("d")
         new_d.parent = new_aa
         from_paths = ["/a/d", "aa/d", "e", "g", "h", "f"]
@@ -1518,17 +1494,17 @@
         copy_nodes_from_tree_to_tree(
             from_tree=self.root,
             to_tree=self.root_other,
             from_paths=from_paths,
             to_paths=to_paths,
             overriding=True,
         )
-        assert_tree_structure_basenode_root_generic(self.root_other)
+        assert_tree_structure_basenode_root(self.root_other)
         assert_tree_structure_basenode_root_attr(self.root_other, d=("d", 1))
-        assert_tree_structure_node_root_generic(self.root_other)
+        assert_tree_structure_node_root(self.root_other)
 
     def test_copy_nodes_from_tree_to_tree_overriding(self):
         from_paths = ["d", "e", "g", "h", "f"]
         to_paths = ["a/b/d", "a/b/e", "a/b/e/g", "a/b/e/h", "a/c/f"]
         shift_nodes(self.root, from_paths, to_paths)
 
         from_paths = ["a/b", "a/c"]
@@ -1536,17 +1512,17 @@
         copy_nodes_from_tree_to_tree(
             from_tree=self.root,
             to_tree=self.root_other_full_wrong,
             from_paths=from_paths,
             to_paths=to_paths,
             overriding=True,
         )
-        assert_tree_structure_basenode_root_generic(self.root_other_full_wrong)
+        assert_tree_structure_basenode_root(self.root_other_full_wrong)
         assert_tree_structure_basenode_root_attr(self.root_other_full_wrong)
-        assert_tree_structure_node_root_generic(self.root_other_full_wrong)
+        assert_tree_structure_node_root(self.root_other_full_wrong)
 
     # merge_children
     def test_copy_nodes_from_tree_to_tree_merge_children(self):
         from_paths = ["e", "g", "h"]
         to_paths = ["a/bb/e", "a/bb/e/g", "a/bb/e/h"]
         shift_nodes(self.root, from_paths, to_paths)
 
@@ -1555,17 +1531,17 @@
         copy_nodes_from_tree_to_tree(
             from_tree=self.root,
             to_tree=self.root_other_full,
             from_paths=from_paths,
             to_paths=to_paths,
             merge_children=True,
         )
-        assert_tree_structure_basenode_root_generic(self.root_other_full)
+        assert_tree_structure_basenode_root(self.root_other_full)
         assert_tree_structure_basenode_root_attr(self.root_other_full)
-        assert_tree_structure_node_root_generic(self.root_other_full)
+        assert_tree_structure_node_root(self.root_other_full)
 
     def test_copy_nodes_from_tree_to_tree_merge_children_non_overriding(self):
         from_paths = ["e", "g", "h"]
         to_paths = ["a/b/e", "a/b/e/g", "a/b/e/h"]
         shift_nodes(self.root, from_paths, to_paths)
 
         from_paths = ["a/b"]
@@ -1573,17 +1549,17 @@
         copy_nodes_from_tree_to_tree(
             from_tree=self.root,
             to_tree=self.root_other_full,
             from_paths=from_paths,
             to_paths=to_paths,
             merge_children=True,
         )
-        assert_tree_structure_basenode_root_generic(self.root_other_full)
+        assert_tree_structure_basenode_root(self.root_other_full)
         assert_tree_structure_basenode_root_attr(self.root_other_full)
-        assert_tree_structure_node_root_generic(self.root_other_full)
+        assert_tree_structure_node_root(self.root_other_full)
 
     def test_copy_nodes_from_tree_to_tree_merge_children_non_overriding_error(self):
         from_paths = ["d", "e", "g", "h", "f"]
         to_paths = ["a/b/d", "a/b/e", "a/b/e/g", "a/b/e/h", "a/c/f"]
         shift_nodes(self.root, from_paths, to_paths)
 
         from_paths = ["a/c"]
@@ -1592,15 +1568,15 @@
             copy_nodes_from_tree_to_tree(
                 from_tree=self.root,
                 to_tree=self.root_other_full,
                 from_paths=from_paths,
                 to_paths=to_paths,
                 merge_children=True,
             )
-        assert str(exc_info.value).startswith("Error: Duplicate node with same path")
+        assert str(exc_info.value).startswith(Constants.ERROR_SAME_PATH)
 
     # merge_leaves
     def test_copy_nodes_from_tree_to_tree_merge_leaves(self):
         from_paths = ["a"]
         to_paths = ["a/b/a"]
         copy_nodes_from_tree_to_tree(
             from_tree=self.root,
@@ -1632,17 +1608,17 @@
         copy_nodes_from_tree_to_tree(
             from_tree=self.root,
             to_tree=self.root_other_full,
             from_paths=from_paths,
             to_paths=to_paths,
             merge_leaves=True,
         )
-        assert_tree_structure_basenode_root_generic(self.root_other_full)
+        assert_tree_structure_basenode_root(self.root_other_full)
         assert_tree_structure_basenode_root_attr(self.root_other_full)
-        assert_tree_structure_node_root_generic(self.root_other_full)
+        assert_tree_structure_node_root(self.root_other_full)
 
     def test_copy_nodes_from_tree_to_tree_merge_leaves_non_overriding_error(self):
         from_paths = ["a/d", "a/e", "a/g", "a/h"]
         to_paths = ["a/b/d", "/a/b/e", "a/c/g", "a/c/h"]
         shift_nodes(self.root, from_paths, to_paths)
 
         from_paths = ["a/b", "a/c"]
@@ -1652,15 +1628,15 @@
             copy_nodes_from_tree_to_tree(
                 from_tree=self.root,
                 to_tree=self.root_other_full,
                 from_paths=from_paths,
                 to_paths=to_paths,
                 merge_leaves=True,
             )
-        assert str(exc_info.value).startswith("Error: Duplicate node with same path")
+        assert str(exc_info.value).startswith(Constants.ERROR_SAME_PATH)
 
     # delete_children
     def test_copy_nodes_from_tree_to_tree_delete_children(self):
         from_paths = ["a/b", "a/c", "a/d", "a/f"]
         to_paths = ["a/e/b", "a/e/b/c", "a/g/d", "a/h/f"]
         shift_nodes(self.root, from_paths, to_paths)
 
@@ -1669,17 +1645,17 @@
         copy_nodes_from_tree_to_tree(
             from_tree=self.root,
             to_tree=self.root_other_full,
             from_paths=from_paths,
             to_paths=to_paths,
             delete_children=True,
         )
-        assert_tree_structure_basenode_root_generic(self.root_other_full)
+        assert_tree_structure_basenode_root(self.root_other_full)
         assert_tree_structure_basenode_root_attr(self.root_other_full)
-        assert_tree_structure_node_root_generic(self.root_other_full)
+        assert_tree_structure_node_root(self.root_other_full)
 
     # merge_children, overriding
     def test_copy_nodes_from_tree_to_tree_merge_children_overriding(self):
         from_paths = ["d", "e", "g", "h", "f"]
         to_paths = ["a/bb/d", "a/bb/e", "a/bb/e/g", "a/bb/e/h", "a/c/f"]
         shift_nodes(self.root, from_paths, to_paths)
 
@@ -1689,17 +1665,17 @@
             from_tree=self.root,
             to_tree=self.root_other_full_wrong,
             from_paths=from_paths,
             to_paths=to_paths,
             merge_children=True,
             overriding=True,
         )
-        assert_tree_structure_basenode_root_generic(self.root_other_full_wrong)
+        assert_tree_structure_basenode_root(self.root_other_full_wrong)
         assert_tree_structure_basenode_root_attr(self.root_other_full_wrong)
-        assert_tree_structure_node_root_generic(self.root_other_full_wrong)
+        assert_tree_structure_node_root(self.root_other_full_wrong)
 
     # merge_leaves, overriding
     def test_copy_nodes_from_tree_to_tree_merge_leaves_overriding(self):
         from_paths = ["d", "e", "g", "h", "f"]
         to_paths = ["a/bb/d", "a/bb/e", "a/cc/g", "a/cc/h", "a/c/f"]
         shift_nodes(self.root, from_paths, to_paths)
 
@@ -1709,34 +1685,32 @@
             from_tree=self.root,
             to_tree=self.root_other_full_wrong,
             from_paths=from_paths,
             to_paths=to_paths,
             merge_leaves=True,
             overriding=True,
         )
-        assert_tree_structure_basenode_root_generic(self.root_other_full_wrong)
+        assert_tree_structure_basenode_root(self.root_other_full_wrong)
         assert_tree_structure_basenode_root_attr(self.root_other_full_wrong, c=("c", 1))
-        assert_tree_structure_node_root_generic(self.root_other_full_wrong)
+        assert_tree_structure_node_root(self.root_other_full_wrong)
 
     # merge_children, merge_leaves
     def test_copy_nodes_from_tree_to_tree_merge_children_and_leaf_error(self):
         from_paths = ["a"]
         to_paths = ["a"]
         with pytest.raises(ValueError) as exc_info:
             copy_nodes_from_tree_to_tree(
                 from_tree=self.root,
                 to_tree=self.root_other_full_wrong,
                 from_paths=from_paths,
                 to_paths=to_paths,
                 merge_children=True,
                 merge_leaves=True,
             )
-        assert str(exc_info.value).startswith(
-            "Invalid shifting, can only specify one type of merging"
-        )
+        assert str(exc_info.value) == Constants.ERROR_MERGE_CHILDREN_OR_LEAVES
 
     # merge_children, delete_children
     def test_copy_nodes_from_tree_to_tree_merge_children_and_delete_children(self):
         from_paths = ["e", "/b", "g", "/c", "h", "d", "f"]
         to_paths = [
             "a/bb/e",
             "a/bb/e/b",
@@ -1754,40 +1728,58 @@
             from_tree=self.root,
             to_tree=self.root_other_full,
             from_paths=from_paths,
             to_paths=to_paths,
             merge_children=True,
             delete_children=True,
         )
-        assert_tree_structure_basenode_root_generic(self.root_other_full)
+        assert_tree_structure_basenode_root(self.root_other_full)
         assert_tree_structure_basenode_root_attr(self.root_other_full)
-        assert_tree_structure_node_root_generic(self.root_other_full)
+        assert_tree_structure_node_root(self.root_other_full)
+
+    # merge_leaves, delete_children
+    def test_copy_nodes_from_tree_to_tree_merge_leaves_and_delete_children(self):
+        from_paths = ["a/e", "a/g", "a/h"]
+        to_paths = ["/a/b/e", "a/c/g", "a/c/h"]
+        shift_nodes(self.root, from_paths, to_paths)
+
+        from_paths = ["a/b", "a/c"]
+        to_paths = ["/a/b", "a/b/e/c"]
+        copy_nodes_from_tree_to_tree(
+            from_tree=self.root,
+            to_tree=self.root_other_full,
+            from_paths=from_paths,
+            to_paths=to_paths,
+            merge_leaves=True,
+            delete_children=True,
+        )
+        assert_tree_structure_basenode_root(self.root_other_full)
+        assert_tree_structure_basenode_root_attr(self.root_other_full)
+        assert_tree_structure_node_root(self.root_other_full)
 
     # with_full_path
     def test_copy_nodes_from_tree_to_tree_with_full_path(self):
         from_paths = ["a/b", "a/c", "a/d", "a/e", "a/f", "a/g", "a/h"]
         to_paths = ["a/b", "a/c", "a/b/d", "a/b/e", "a/c/f", "a/b/e/g", "a/b/e/h"]
         copy_nodes_from_tree_to_tree(
             from_tree=self.root,
             to_tree=self.root_other,
             from_paths=from_paths,
             to_paths=to_paths,
             with_full_path=True,
         )
-        assert_tree_structure_basenode_root_generic(self.root_other)
+        assert_tree_structure_basenode_root(self.root_other)
         assert_tree_structure_basenode_root_attr(self.root_other)
-        assert_tree_structure_node_root_generic(self.root_other)
+        assert_tree_structure_node_root(self.root_other)
 
     def test_copy_nodes_from_tree_to_tree_with_full_path_error(self):
         from_paths = ["d", "e", "g", "h", "f"]
         to_paths = ["a/b/d", "a/b/e", "a/b/e/g", "a/b/e/h", "a/c/f"]
         with pytest.raises(ValueError) as exc_info:
             copy_nodes_from_tree_to_tree(
                 from_tree=self.root,
                 to_tree=self.root_other,
                 from_paths=from_paths,
                 to_paths=to_paths,
                 with_full_path=True,
             )
-        assert str(exc_info.value).startswith(
-            "Invalid path in `from_paths` not starting with the root node"
-        )
+        assert str(exc_info.value).startswith(Constants.ERROR_INVALID_FULL_PATH)
```

### Comparing `bigtree-0.9.3/tests/tree/test_search.py` & `bigtree-0.9.4/tests/tree/test_search.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     find_name,
     find_names,
     find_path,
     find_paths,
     findall,
 )
 from bigtree.utils.exceptions import SearchError
+from tests.constants import Constants
 
 
 class TestSearch(unittest.TestCase):
     def setUp(self):
         """
         Tree should have structure
         a (age=90)
@@ -84,20 +85,22 @@
         actual = findall(self.a, lambda node: node.age >= 30, max_depth=2)
         expected = (self.a, self.b, self.c)
         assert (
             actual == expected
         ), f"Expected find_all to return {expected}, received {actual}"
 
     def test_find_all_max_count_error(self):
-        with pytest.raises(SearchError):
+        with pytest.raises(SearchError) as exc_info:
             findall(self.a, lambda node: node.age >= 30, max_depth=2, max_count=2)
+        assert str(exc_info.value).startswith(Constants.ERROR_TWO_ELEMENT)
 
     def test_find_all_min_count_error(self):
-        with pytest.raises(SearchError):
+        with pytest.raises(SearchError) as exc_info:
             findall(self.a, lambda node: node.age >= 30, max_depth=2, min_count=4)
+        assert str(exc_info.value).startswith(Constants.ERROR_MORE_THAN_FOUR_ELEMENT)
 
     def test_find(self):
         actual = find(self.a, lambda node: node.age == 60)
         expected = self.c
         assert (
             actual == expected
         ), f"Expected find to return {expected}, received {actual}"
@@ -112,16 +115,17 @@
         actual = find(self.b, lambda node: node.age == 60)
         expected = None
         assert (
             actual == expected
         ), f"Expected find to return {expected}, received {actual}"
 
     def test_find_error(self):
-        with pytest.raises(SearchError):
+        with pytest.raises(SearchError) as exc_info:
             find(self.a, lambda node: node.age > 5)
+        assert str(exc_info.value).startswith(Constants.ERROR_ONE_ELEMENT)
 
     def test_find_name(self):
         inputs = ["a", "b", "c", "d", "e", "f", "g", "h", "i"]
         expected_ans = [
             self.a,
             self.b,
             self.c,
@@ -219,24 +223,25 @@
         expected_ans = [None, None]
         for input_, expected in zip(inputs, expected_ans):
             actual = find_full_path(self.a, input_)
             assert (
                 actual == expected
             ), f"Expected find_full_path to return {expected}, received {actual}"
 
-    def test_find_full_wrong_root(self):
+    def test_find_full_wrong_root_error(self):
         inputs = [
             "/",
             "/b/d/",
             "/b/",
         ]
         expected_ans = [None, None, None]
         for input_, expected in zip(inputs, expected_ans):
-            with pytest.raises(ValueError):
+            with pytest.raises(ValueError) as exc_info:
                 find_full_path(self.a, input_)
+        assert str(exc_info.value).endswith("does not match the root node name a")
 
     def test_find_path(self):
         inputs = [
             "/a",
             "/a/b",
             "/a/c",
             "/a/b/d",
@@ -503,21 +508,23 @@
                 ),
             )
             expected = expected_ans[idx]
             assert (
                 actual == expected
             ), f"Expected find_children to return {expected}, received {actual} for input {input}"
 
-    def test_find_children_max_count(self):
-        with pytest.raises(SearchError):
+    def test_find_children_max_count_error(self):
+        with pytest.raises(SearchError) as exc_info:
             find_children(self.a, lambda node: node.age >= 30, max_count=1)
+        assert str(exc_info.value).startswith(Constants.ERROR_ONE_ELEMENT)
 
-    def test_find_children_min_count(self):
-        with pytest.raises(SearchError):
+    def test_find_children_min_count_error(self):
+        with pytest.raises(SearchError) as exc_info:
             find_children(self.a, lambda node: node.age >= 30, min_count=3)
+        assert str(exc_info.value).startswith(Constants.ERROR_MORE_THAN_THREE_ELEMENT)
 
     def test_find_child(self):
         inputs = [self.a, self.b, self.c, self.d, self.e, self.f, self.g, self.h]
         expected_ans = [
             self.b,
             self.e,
             self.f,
@@ -536,16 +543,17 @@
             )
             expected = expected_ans[idx]
             assert (
                 actual == expected
             ), f"Expected find_children to return {expected}, received {actual} for input {input}"
 
     def test_find_child_error(self):
-        with pytest.raises(SearchError):
+        with pytest.raises(SearchError) as exc_info:
             find_child(self.a, lambda node: node.age > 5)
+        assert str(exc_info.value).startswith(Constants.ERROR_ONE_ELEMENT)
 
     def test_find_child_by_name(self):
         inputs1 = [self.a, self.b, self.c, self.d, self.e, self.f, self.g, self.h]
         inputs2 = ["a", "b", "c", "d", "e", "f", "g", "h"]
         expected_ans = [
             [None, self.b, self.c, None, None, None, None, None],
             [None, None, None, self.d, self.e, None, None, None],
```

### Comparing `bigtree-0.9.3/tests/utils/test_iterators.py` & `bigtree-0.9.4/tests/utils/test_iterators.py`

 * *Files 0% similar despite different names*

```diff
@@ -334,15 +334,15 @@
     @staticmethod
     def test_levelorder_iter(binarytree_node):
         expected = ["1", "2", "3", "4", "5", "6", "7", "8"]
         actual = [node.node_name for node in levelorder_iter(binarytree_node)]
         assert expected == actual, f"Expected\n{expected}\nReceived\n{actual}"
 
     @staticmethod
-    def test_levelordergroup_iter2(binarytree_node):
+    def test_levelordergroup_iter(binarytree_node):
         expected = [["1"], ["2", "3"], ["4", "5", "6", "7"], ["8"]]
         actual = [
             [node.node_name for node in group]
             for group in levelordergroup_iter(binarytree_node)
         ]
         assert expected == actual, f"Expected\n{expected}\nReceived\n{actual}"
```

### Comparing `bigtree-0.9.3/tests/workflows/test_todo.py` & `bigtree-0.9.4/tests/workflows/test_todo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import unittest
 
 import pytest
 
 from bigtree import AppToDo
 from bigtree.utils.exceptions import SearchError
 from tests.conftest import assert_console_output
+from tests.constants import Constants
 
 
 class TestAppToDo(unittest.TestCase):
     def setUp(self):
         self.todoapp = AppToDo("To Do Items")
 
     def tearDown(self):
@@ -164,16 +165,17 @@
             n_children == expected_n_children
         ), f"Expected number of children to be {expected_n_children}, received {n_children}"
         assert (
             n_descendants == expected_n_descendants
         ), f"Expected number of descendants to be {expected_n_descendants}, received {n_children}"
 
     def test_add_item_type_error(self):
-        with pytest.raises(TypeError):
+        with pytest.raises(TypeError) as exc_info:
             self.todoapp.add_item(1)
+        assert str(exc_info.value) == Constants.ERROR_TODO_TYPE
 
     def test_remove_item_single(self):
         self.todoapp.add_item("Item 1")
         self.todoapp.remove_item("Item 1")
         max_depth = self.todoapp._root.max_depth
         n_children = len(list(self.todoapp._root.children))
         n_descendants = len(list(self.todoapp._root.descendants))
@@ -255,16 +257,17 @@
         assert (
             n_descendants == expected_n_descendants
         ), f"Expected number of descendants to be {expected_n_descendants}, received {n_children}"
 
     def test_remove_duplicate_item_error(self):
         self.todoapp.add_item("Item 1")
         self.todoapp.add_item("Item 1", "List 1")
-        with pytest.raises(SearchError):
+        with pytest.raises(SearchError) as exc_info:
             self.todoapp.remove_item("Item 1")
+        assert str(exc_info.value).startswith(Constants.ERROR_ONE_ELEMENT)
 
     def test_remove_item_multiple(self):
         self.todoapp.add_item(["Item 1", "Item 2"])
         self.todoapp.remove_item(["Item 1", "Item 2"])
         max_depth = self.todoapp._root.max_depth
         n_children = len(list(self.todoapp._root.children))
         n_descendants = len(list(self.todoapp._root.descendants))
@@ -297,16 +300,17 @@
             n_children == expected_n_children
         ), f"Expected number of children to be {expected_n_children}, received {n_children}"
         assert (
             n_descendants == expected_n_descendants
         ), f"Expected number of descendants to be {expected_n_descendants}, received {n_children}"
 
     def test_remove_item_error(self):
-        with pytest.raises(TypeError):
+        with pytest.raises(TypeError) as exc_info:
             self.todoapp.remove_item(1)
+        assert str(exc_info.value) == Constants.ERROR_TODO_TYPE
 
     def test_prioritize_item(self):
         self.todoapp.add_item("Item 1", "List 1")
         self.todoapp.add_item("Item 2", "List 1")
         self.todoapp.prioritize_item("Item 2")
         max_depth = self.todoapp._root.max_depth
         n_children = len(list(self.todoapp._root.children))
```

### Comparing `bigtree-0.9.3/LICENSE` & `bigtree-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/README.md` & `bigtree-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.3/pyproject.toml` & `bigtree-0.9.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -72,14 +72,15 @@
   "pandas==1.5.1",
   "sphinxemoji==0.2.0"
 ]
 
 [tool.hatch.envs.docs.scripts]
 html = "sphinx-build -M html docs/source docs/build"
 clean = "sphinx-build -M clean docs/source docs/build"
+clean-html = "sphinx-build -M html docs/source docs/build & sphinx-build -M clean docs/source docs/build"
 
 [[tool.hatch.envs.test.matrix]]
 python = ["37", "38", "39", "310", "311"]
 
 [tool.coverage.run]
 branch = true
 parallel = true
```

### Comparing `bigtree-0.9.3/PKG-INFO` & `bigtree-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigtree
-Version: 0.9.3
+Version: 0.9.4
 Summary: Tree Implementation for Python, integrated with Python list, dictionary, and pandas DataFrame.
 Project-URL: Documentation, https://bigtree.readthedocs.io
 Project-URL: Issues, https://github.com/kayjan/bigtree/issues
 Project-URL: Source, https://github.com/kayjan/bigtree
 Author-email: Kay Jan <kayjanw@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bigtree Version: 0.9.3 Summary: Tree Implementation
+Metadata-Version: 2.1 Name: bigtree Version: 0.9.4 Summary: Tree Implementation
 for Python, integrated with Python list, dictionary, and pandas DataFrame.
 Project-URL: Documentation, https://bigtree.readthedocs.io Project-URL: Issues,
 https://github.com/kayjan/bigtree/issues Project-URL: Source, https://
 github.com/kayjan/bigtree Author-email: Kay Jan
 gmail.com> License-Expression: MIT License-File: LICENSE Keywords: bigtree,tree
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3.7 Classifier:
```

