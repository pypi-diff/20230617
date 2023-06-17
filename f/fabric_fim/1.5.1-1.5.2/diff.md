# Comparing `tmp/fabric_fim-1.5.1.tar.gz` & `tmp/fabric_fim-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric_fim-1.5.1.tar", last modified: Thu Jun 15 15:31:12 2023, max compression
+gzip compressed data, was "fabric_fim-1.5.2.tar", last modified: Sat Jun 17 00:16:08 2023, max compression
```

## Comparing `fabric_fim-1.5.1.tar` & `fabric_fim-1.5.2.tar`

### file list

```diff
@@ -1,114 +1,114 @@
--rw-r--r--   0        0        0     2208 2023-06-15 15:30:40.226765 fabric_fim-1.5.1/.gitignore
--rw-r--r--   0        0        0       26 2020-07-24 21:42:44.564662 fabric_fim-1.5.1/AUTHORS
--rw-r--r--   0        0        0     1071 2020-07-14 22:09:49.459777 fabric_fim-1.5.1/LICENSE
--rw-r--r--   0        0        0    11110 2023-06-15 15:20:12.737600 fabric_fim-1.5.1/README.md
--rw-r--r--   0        0        0    18690 2021-05-25 21:09:37.024101 fabric_fim-1.5.1/figs/fim-structure.png
--rw-r--r--   0        0        0      557 2021-03-15 22:13:52.784044 fabric_fim-1.5.1/fim/README.md
--rw-r--r--   0        0        0      103 2023-06-15 15:24:42.351103 fabric_fim-1.5.1/fim/__init__.py
--rw-r--r--   0        0        0        1 2022-04-27 22:22:19.299449 fabric_fim-1.5.1/fim/authz/__init__.py
--rw-r--r--   0        0        0    16139 2023-02-02 01:41:56.403069 fabric_fim-1.5.1/fim/authz/attribute_collector.py
--rw-r--r--   0        0        0      334 2020-09-12 23:24:52.369007 fabric_fim-1.5.1/fim/graph/README.md
--rw-r--r--   0        0        0        1 2020-09-02 18:31:38.004468 fabric_fim-1.5.1/fim/graph/__init__.py
--rw-r--r--   0        0        0    69843 2023-06-15 15:19:01.141154 fabric_fim-1.5.1/fim/graph/abc_property_graph.py
--rw-r--r--   0        0        0     4093 2023-02-02 01:41:56.406333 fabric_fim-1.5.1/fim/graph/abc_property_graph_constants.py
--rw-r--r--   0        0        0        1 2020-08-18 21:34:07.036009 fabric_fim-1.5.1/fim/graph/data/__init__.py
--rw-r--r--   0        0        0      283 2020-09-03 22:10:53.500264 fabric_fim-1.5.1/fim/graph/data/capacity_types.json
--rw-r--r--   0        0        0      100 2020-08-27 20:41:23.401941 fabric_fim-1.5.1/fim/graph/data/constraint_types.json
--rw-r--r--   0        0        0     3886 2023-06-15 15:19:01.141376 fabric_fim-1.5.1/fim/graph/data/graph_validation_rules.json
--rw-r--r--   0        0        0     3845 2023-06-15 15:19:01.141499 fabric_fim-1.5.1/fim/graph/data/graph_validation_rules_neo4j_v4.json
--rw-r--r--   0        0        0      547 2020-09-03 22:10:39.822590 fabric_fim-1.5.1/fim/graph/data/label_types.json
--rw-r--r--   0        0        0       91 2020-08-27 20:40:54.261031 fabric_fim-1.5.1/fim/graph/data/location_types.json
--rw-r--r--   0        0        0      861 2023-05-10 14:54:24.189132 fabric_fim-1.5.1/fim/graph/data/neo4j_indexes.json
--rw-r--r--   0        0        0     3320 2023-06-15 15:19:01.141615 fabric_fim-1.5.1/fim/graph/graph_util.py
--rw-r--r--   0        0        0    44293 2023-06-15 15:19:01.154588 fabric_fim-1.5.1/fim/graph/neo4j_property_graph.py
--rw-r--r--   0        0        0     6160 2022-10-06 17:38:08.214224 fabric_fim-1.5.1/fim/graph/networkx_mixin.py
--rw-r--r--   0        0        0    42211 2023-06-15 15:19:01.141889 fabric_fim-1.5.1/fim/graph/networkx_property_graph.py
--rw-r--r--   0        0        0     8354 2022-10-07 03:05:34.849246 fabric_fim-1.5.1/fim/graph/networkx_property_graph_disjoint.py
--rw-r--r--   0        0        0     1501 2021-03-15 22:13:52.788626 fabric_fim-1.5.1/fim/graph/resources/README.md
--rw-r--r--   0        0        0        1 2020-09-02 18:32:04.638774 fabric_fim-1.5.1/fim/graph/resources/__init__.py
--rw-r--r--   0        0        0     4484 2021-05-25 21:09:37.029370 fabric_fim-1.5.1/fim/graph/resources/abc_adm.py
--rw-r--r--   0        0        0    13570 2023-05-10 14:54:24.193783 fabric_fim-1.5.1/fim/graph/resources/abc_arm.py
--rw-r--r--   0        0        0     2991 2022-02-18 19:27:15.586527 fabric_fim-1.5.1/fim/graph/resources/abc_bqm.py
--rw-r--r--   0        0        0     4547 2021-03-31 01:14:29.518807 fabric_fim-1.5.1/fim/graph/resources/abc_cbm.py
--rw-r--r--   0        0        0     2297 2021-03-07 22:42:30.018249 fabric_fim-1.5.1/fim/graph/resources/neo4j_adm.py
--rw-r--r--   0        0        0     2106 2021-05-25 21:09:37.031668 fabric_fim-1.5.1/fim/graph/resources/neo4j_arm.py
--rw-r--r--   0        0        0    18591 2023-06-15 15:19:01.148045 fabric_fim-1.5.1/fim/graph/resources/neo4j_cbm.py
--rw-r--r--   0        0        0     5017 2022-02-18 19:27:15.587881 fabric_fim-1.5.1/fim/graph/resources/networkx_abqm.py
--rw-r--r--   0        0        0     2341 2021-03-07 22:42:30.020154 fabric_fim-1.5.1/fim/graph/resources/networkx_adm.py
--rw-r--r--   0        0        0     2122 2021-05-25 21:09:37.033196 fabric_fim-1.5.1/fim/graph/resources/networkx_arm.py
--rw-r--r--   0        0        0      301 2021-03-15 22:13:52.789768 fabric_fim-1.5.1/fim/graph/slices/README.md
--rw-r--r--   0        0        0        1 2020-09-02 18:32:24.788341 fabric_fim-1.5.1/fim/graph/slices/__init__.py
--rw-r--r--   0        0        0     8223 2022-02-18 19:27:15.588460 fabric_fim-1.5.1/fim/graph/slices/abc_asm.py
--rw-r--r--   0        0        0     3733 2023-05-10 14:54:24.196715 fabric_fim-1.5.1/fim/graph/slices/neo4j_asm.py
--rw-r--r--   0        0        0     4298 2021-06-04 19:43:14.989790 fabric_fim-1.5.1/fim/graph/slices/networkx_asm.py
--rw-r--r--   0        0        0     8615 2021-03-03 19:57:54.288231 fabric_fim-1.5.1/fim/graph/typed_tuples.py
--rw-r--r--   0        0        0        0 2023-02-02 01:41:56.409002 fabric_fim-1.5.1/fim/logging/__init__.py
--rw-r--r--   0        0        0     1526 2023-06-15 15:19:01.033709 fabric_fim-1.5.1/fim/logging/fim_logger.py
--rw-r--r--   0        0        0     9071 2023-02-02 01:41:56.410072 fabric_fim-1.5.1/fim/logging/log_collector.py
--rw-r--r--   0        0        0     9555 2021-03-24 00:18:51.063382 fabric_fim-1.5.1/fim/pluggable.py
--rw-r--r--   0        0        0      189 2021-06-04 19:43:14.990352 fabric_fim-1.5.1/fim/slivers/README.md
--rw-r--r--   0        0        0      217 2021-06-14 18:36:21.931262 fabric_fim-1.5.1/fim/slivers/__init__.py
--rw-r--r--   0        0        0     3641 2023-02-02 01:41:56.410512 fabric_fim-1.5.1/fim/slivers/attached_components.py
--rw-r--r--   0        0        0    13021 2023-02-02 01:41:56.411041 fabric_fim-1.5.1/fim/slivers/base_sliver.py
--rw-r--r--   0        0        0    26010 2023-06-15 15:20:12.767056 fabric_fim-1.5.1/fim/slivers/capacities_labels.py
--rw-r--r--   0        0        0    11537 2023-06-13 15:16:11.169736 fabric_fim-1.5.1/fim/slivers/component_catalog.py
--rw-r--r--   0        0        0        1 2021-03-03 19:57:54.291739 fabric_fim-1.5.1/fim/slivers/data/__init__.py
--rw-r--r--   0        0        0     1691 2023-05-10 14:54:24.202981 fabric_fim-1.5.1/fim/slivers/data/component_catalog.json
--rw-r--r--   0        0        0    76943 2022-09-10 21:18:41.714675 fabric_fim-1.5.1/fim/slivers/data/instance_sizes.json
--rw-r--r--   0        0        0    23524 2022-02-18 19:27:15.591229 fabric_fim-1.5.1/fim/slivers/delegations.py
--rw-r--r--   0        0        0     3593 2022-02-18 19:27:15.591744 fabric_fim-1.5.1/fim/slivers/gateway.py
--rw-r--r--   0        0        0      919 2021-06-29 20:04:13.972162 fabric_fim-1.5.1/fim/slivers/identifiers.py
--rw-r--r--   0        0        0     3444 2022-02-18 19:27:15.592250 fabric_fim-1.5.1/fim/slivers/instance_catalog.py
--rw-r--r--   0        0        0     3225 2023-02-02 01:41:56.413360 fabric_fim-1.5.1/fim/slivers/interface_info.py
--rw-r--r--   0        0        0     2702 2021-09-22 14:46:40.423027 fabric_fim-1.5.1/fim/slivers/json.py
--rw-r--r--   0        0        0     3869 2023-02-02 01:41:56.413720 fabric_fim-1.5.1/fim/slivers/json_data.py
--rw-r--r--   0        0        0     5983 2023-02-02 01:41:56.414203 fabric_fim-1.5.1/fim/slivers/maintenance_mode.py
--rw-r--r--   0        0        0     1566 2021-03-03 19:57:54.294274 fabric_fim-1.5.1/fim/slivers/network_attached_storage.py
--rw-r--r--   0        0        0     3910 2023-02-02 01:41:56.414662 fabric_fim-1.5.1/fim/slivers/network_link.py
--rw-r--r--   0        0        0    10209 2023-02-02 01:41:56.415082 fabric_fim-1.5.1/fim/slivers/network_node.py
--rw-r--r--   0        0        0    22026 2023-05-10 14:54:24.204710 fabric_fim-1.5.1/fim/slivers/network_service.py
--rw-r--r--   0        0        0     6795 2021-06-04 19:43:14.993329 fabric_fim-1.5.1/fim/slivers/path_info.py
--rw-r--r--   0        0        0     3024 2022-02-18 19:27:15.594931 fabric_fim-1.5.1/fim/slivers/tags.py
--rw-r--r--   0        0        0     2622 2023-02-02 01:41:56.416090 fabric_fim-1.5.1/fim/slivers/topology_diff.py
--rw-r--r--   0        0        0     8706 2022-02-18 19:27:15.595505 fabric_fim-1.5.1/fim/user/README.md
--rw-r--r--   0        0        0     1914 2023-02-02 01:41:56.417286 fabric_fim-1.5.1/fim/user/__init__.py
--rw-r--r--   0        0        0    11730 2022-09-10 21:18:41.716394 fabric_fim-1.5.1/fim/user/component.py
--rw-r--r--   0        0        0     5668 2022-09-10 21:18:41.716675 fabric_fim-1.5.1/fim/user/composite_node.py
--rw-r--r--   0        0        0     7660 2023-02-02 01:41:56.418568 fabric_fim-1.5.1/fim/user/interface.py
--rw-r--r--   0        0        0     8381 2022-09-10 21:18:41.717280 fabric_fim-1.5.1/fim/user/link.py
--rw-r--r--   0        0        0     1219 2021-03-03 19:57:54.300001 fabric_fim-1.5.1/fim/user/measurement.py
--rw-r--r--   0        0        0     9668 2023-04-05 18:48:29.319327 fabric_fim-1.5.1/fim/user/model_element.py
--rw-r--r--   0        0        0    29219 2023-05-10 14:54:24.206616 fabric_fim-1.5.1/fim/user/network_service.py
--rw-r--r--   0        0        0    22636 2023-02-14 21:58:39.970039 fabric_fim-1.5.1/fim/user/node.py
--rw-r--r--   0        0        0    58158 2023-06-01 15:42:31.904936 fabric_fim-1.5.1/fim/user/topology.py
--rw-r--r--   0        0        0        2 2023-06-15 15:19:24.419545 fabric_fim-1.5.1/fim/util/__init__.py
--rw-r--r--   0        0        0    14139 2023-06-15 15:20:12.712509 fabric_fim-1.5.1/fim/util/fim_util.py
--rw-r--r--   0        0        0      595 2021-03-13 20:40:37.643107 fabric_fim-1.5.1/fim/view_only_dict.py
--rw-r--r--   0        0        0        0 2023-02-02 01:41:56.421372 fabric_fim-1.5.1/neo4j/data/.empty
--rw-r--r--   0        0        0        0 2023-02-02 01:41:56.421489 fabric_fim-1.5.1/neo4j/imports/.empty
--rw-r--r--   0        0        0      863 2023-06-15 15:20:12.720926 fabric_fim-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     4632 2022-03-09 00:58:31.583145 fabric_fim-1.5.1/test/ad_topology_test.py
--rw-r--r--   0        0        0     4834 2022-09-10 21:18:41.719406 fabric_fim-1.5.1/test/after.graphml
--rw-r--r--   0        0        0    17550 2023-06-15 15:20:12.731835 fabric_fim-1.5.1/test/attribute_collector_test.py
--rw-r--r--   0        0        0     4696 2022-09-10 21:18:41.719615 fabric_fim-1.5.1/test/before.graphml
--rw-r--r--   0        0        0     2729 2022-09-10 21:18:41.719876 fabric_fim-1.5.1/test/catalog_test.py
--rw-r--r--   0        0        0     4319 2022-02-18 19:27:15.602412 fabric_fim-1.5.1/test/delegation_label_test.py
--rw-r--r--   0        0        0     1653 2023-02-02 01:41:56.423551 fabric_fim-1.5.1/test/maintenance_test.py
--rw-r--r--   0        0        0    51613 2023-05-10 17:34:04.562843 fabric_fim-1.5.1/test/models/advertised_topo.graphml
--rw-r--r--   0        0        0    49696 2023-05-10 17:34:04.565992 fabric_fim-1.5.1/test/models/graph-template.graphml
--rw-r--r--   0        0        0    82994 2023-05-10 17:34:04.568753 fabric_fim-1.5.1/test/models/network-am-ad.graphml
--rw-r--r--   0        0        0    57411 2023-05-10 17:34:04.571919 fabric_fim-1.5.1/test/models/site-2-am-1broker-ad.graphml
--rw-r--r--   0        0        0    52887 2023-05-10 17:34:04.574274 fabric_fim-1.5.1/test/models/site-3-am-1broker-ad.graphml
--rw-r--r--   0        0        0   131407 2023-05-10 17:34:04.575177 fabric_fim-1.5.1/test/models/site-am-2broker-ad.graphml
--rw-r--r--   0        0        0    17363 2023-06-15 15:19:01.186506 fabric_fim-1.5.1/test/modify_test.py
--rw-r--r--   0        0        0    13135 2021-05-23 19:50:30.753072 fabric_fim-1.5.1/test/networkxx_pg_disjoint_test.py
--rw-r--r--   0        0        0    14091 2021-05-23 19:50:30.753595 fabric_fim-1.5.1/test/networkxx_pg_test.py
--rw-r--r--   0        0        0     2572 2021-03-24 00:18:51.064667 fabric_fim-1.5.1/test/pluggable_test.py
--rw-r--r--   0        0        0    42428 2023-06-15 15:20:12.777803 fabric_fim-1.5.1/test/slice_topology_test.py
--rw-r--r--   0        0        0     1869 2022-04-27 22:22:19.322857 fabric_fim-1.5.1/test/sliver_json_test.py
--rw-r--r--   0        0        0     6030 2023-06-15 15:20:12.763581 fabric_fim-1.5.1/test/sliver_test.py
--rw-r--r--   0        0        0    97162 2023-02-02 01:41:56.427682 fabric_fim-1.5.1/test/substrate_topology_test.py
--rw-r--r--   0        0        0      654 2022-02-18 19:27:15.604787 fabric_fim-1.5.1/test/test_load.py
--rw-r--r--   0        0        0     2362 2022-02-18 19:27:15.605244 fabric_fim-1.5.1/test/tuple_test.py
--rw-r--r--   0        0        0    15663 2023-06-15 15:19:01.186763 fabric_fim-1.5.1/test/zz_neo4j_pg_test.py
--rw-r--r--   0        0        0    11890 1970-01-01 00:00:00.000000 fabric_fim-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     2208 2023-06-15 15:30:40.226765 fabric_fim-1.5.2/.gitignore
+-rw-r--r--   0        0        0       26 2020-07-24 21:42:44.564662 fabric_fim-1.5.2/AUTHORS
+-rw-r--r--   0        0        0     1071 2020-07-14 22:09:49.459777 fabric_fim-1.5.2/LICENSE
+-rw-r--r--   0        0        0    11110 2023-06-15 15:20:12.737600 fabric_fim-1.5.2/README.md
+-rw-r--r--   0        0        0    18690 2021-05-25 21:09:37.024101 fabric_fim-1.5.2/figs/fim-structure.png
+-rw-r--r--   0        0        0      557 2021-03-15 22:13:52.784044 fabric_fim-1.5.2/fim/README.md
+-rw-r--r--   0        0        0      103 2023-06-17 00:14:43.162647 fabric_fim-1.5.2/fim/__init__.py
+-rw-r--r--   0        0        0        1 2022-04-27 22:22:19.299449 fabric_fim-1.5.2/fim/authz/__init__.py
+-rw-r--r--   0        0        0    16139 2023-02-02 01:41:56.403069 fabric_fim-1.5.2/fim/authz/attribute_collector.py
+-rw-r--r--   0        0        0      334 2020-09-12 23:24:52.369007 fabric_fim-1.5.2/fim/graph/README.md
+-rw-r--r--   0        0        0        1 2020-09-02 18:31:38.004468 fabric_fim-1.5.2/fim/graph/__init__.py
+-rw-r--r--   0        0        0    69843 2023-06-15 15:19:01.141154 fabric_fim-1.5.2/fim/graph/abc_property_graph.py
+-rw-r--r--   0        0        0     4093 2023-02-02 01:41:56.406333 fabric_fim-1.5.2/fim/graph/abc_property_graph_constants.py
+-rw-r--r--   0        0        0        1 2020-08-18 21:34:07.036009 fabric_fim-1.5.2/fim/graph/data/__init__.py
+-rw-r--r--   0        0        0      283 2020-09-03 22:10:53.500264 fabric_fim-1.5.2/fim/graph/data/capacity_types.json
+-rw-r--r--   0        0        0      100 2020-08-27 20:41:23.401941 fabric_fim-1.5.2/fim/graph/data/constraint_types.json
+-rw-r--r--   0        0        0     3886 2023-06-15 15:19:01.141376 fabric_fim-1.5.2/fim/graph/data/graph_validation_rules.json
+-rw-r--r--   0        0        0     3845 2023-06-15 15:19:01.141499 fabric_fim-1.5.2/fim/graph/data/graph_validation_rules_neo4j_v4.json
+-rw-r--r--   0        0        0      547 2020-09-03 22:10:39.822590 fabric_fim-1.5.2/fim/graph/data/label_types.json
+-rw-r--r--   0        0        0       91 2020-08-27 20:40:54.261031 fabric_fim-1.5.2/fim/graph/data/location_types.json
+-rw-r--r--   0        0        0      861 2023-05-10 14:54:24.189132 fabric_fim-1.5.2/fim/graph/data/neo4j_indexes.json
+-rw-r--r--   0        0        0     3320 2023-06-15 15:19:01.141615 fabric_fim-1.5.2/fim/graph/graph_util.py
+-rw-r--r--   0        0        0    44293 2023-06-15 15:19:01.154588 fabric_fim-1.5.2/fim/graph/neo4j_property_graph.py
+-rw-r--r--   0        0        0     6160 2022-10-06 17:38:08.214224 fabric_fim-1.5.2/fim/graph/networkx_mixin.py
+-rw-r--r--   0        0        0    42211 2023-06-15 15:19:01.141889 fabric_fim-1.5.2/fim/graph/networkx_property_graph.py
+-rw-r--r--   0        0        0     8354 2022-10-07 03:05:34.849246 fabric_fim-1.5.2/fim/graph/networkx_property_graph_disjoint.py
+-rw-r--r--   0        0        0     1501 2021-03-15 22:13:52.788626 fabric_fim-1.5.2/fim/graph/resources/README.md
+-rw-r--r--   0        0        0        1 2020-09-02 18:32:04.638774 fabric_fim-1.5.2/fim/graph/resources/__init__.py
+-rw-r--r--   0        0        0     4484 2021-05-25 21:09:37.029370 fabric_fim-1.5.2/fim/graph/resources/abc_adm.py
+-rw-r--r--   0        0        0    13570 2023-05-10 14:54:24.193783 fabric_fim-1.5.2/fim/graph/resources/abc_arm.py
+-rw-r--r--   0        0        0     2991 2022-02-18 19:27:15.586527 fabric_fim-1.5.2/fim/graph/resources/abc_bqm.py
+-rw-r--r--   0        0        0     4547 2021-03-31 01:14:29.518807 fabric_fim-1.5.2/fim/graph/resources/abc_cbm.py
+-rw-r--r--   0        0        0     2297 2021-03-07 22:42:30.018249 fabric_fim-1.5.2/fim/graph/resources/neo4j_adm.py
+-rw-r--r--   0        0        0     2106 2021-05-25 21:09:37.031668 fabric_fim-1.5.2/fim/graph/resources/neo4j_arm.py
+-rw-r--r--   0        0        0    18591 2023-06-15 15:19:01.148045 fabric_fim-1.5.2/fim/graph/resources/neo4j_cbm.py
+-rw-r--r--   0        0        0     5017 2022-02-18 19:27:15.587881 fabric_fim-1.5.2/fim/graph/resources/networkx_abqm.py
+-rw-r--r--   0        0        0     2341 2021-03-07 22:42:30.020154 fabric_fim-1.5.2/fim/graph/resources/networkx_adm.py
+-rw-r--r--   0        0        0     2122 2021-05-25 21:09:37.033196 fabric_fim-1.5.2/fim/graph/resources/networkx_arm.py
+-rw-r--r--   0        0        0      301 2021-03-15 22:13:52.789768 fabric_fim-1.5.2/fim/graph/slices/README.md
+-rw-r--r--   0        0        0        1 2020-09-02 18:32:24.788341 fabric_fim-1.5.2/fim/graph/slices/__init__.py
+-rw-r--r--   0        0        0     8223 2022-02-18 19:27:15.588460 fabric_fim-1.5.2/fim/graph/slices/abc_asm.py
+-rw-r--r--   0        0        0     3733 2023-05-10 14:54:24.196715 fabric_fim-1.5.2/fim/graph/slices/neo4j_asm.py
+-rw-r--r--   0        0        0     4298 2021-06-04 19:43:14.989790 fabric_fim-1.5.2/fim/graph/slices/networkx_asm.py
+-rw-r--r--   0        0        0     8615 2021-03-03 19:57:54.288231 fabric_fim-1.5.2/fim/graph/typed_tuples.py
+-rw-r--r--   0        0        0        0 2023-02-02 01:41:56.409002 fabric_fim-1.5.2/fim/logging/__init__.py
+-rw-r--r--   0        0        0     1526 2023-06-15 15:19:01.033709 fabric_fim-1.5.2/fim/logging/fim_logger.py
+-rw-r--r--   0        0        0     9071 2023-02-02 01:41:56.410072 fabric_fim-1.5.2/fim/logging/log_collector.py
+-rw-r--r--   0        0        0     9555 2021-03-24 00:18:51.063382 fabric_fim-1.5.2/fim/pluggable.py
+-rw-r--r--   0        0        0      189 2021-06-04 19:43:14.990352 fabric_fim-1.5.2/fim/slivers/README.md
+-rw-r--r--   0        0        0      217 2021-06-14 18:36:21.931262 fabric_fim-1.5.2/fim/slivers/__init__.py
+-rw-r--r--   0        0        0     3641 2023-02-02 01:41:56.410512 fabric_fim-1.5.2/fim/slivers/attached_components.py
+-rw-r--r--   0        0        0    13021 2023-02-02 01:41:56.411041 fabric_fim-1.5.2/fim/slivers/base_sliver.py
+-rw-r--r--   0        0        0    26010 2023-06-15 15:20:12.767056 fabric_fim-1.5.2/fim/slivers/capacities_labels.py
+-rw-r--r--   0        0        0    11537 2023-06-13 15:16:11.169736 fabric_fim-1.5.2/fim/slivers/component_catalog.py
+-rw-r--r--   0        0        0        1 2021-03-03 19:57:54.291739 fabric_fim-1.5.2/fim/slivers/data/__init__.py
+-rw-r--r--   0        0        0     1691 2023-05-10 14:54:24.202981 fabric_fim-1.5.2/fim/slivers/data/component_catalog.json
+-rw-r--r--   0        0        0    76943 2022-09-10 21:18:41.714675 fabric_fim-1.5.2/fim/slivers/data/instance_sizes.json
+-rw-r--r--   0        0        0    23524 2022-02-18 19:27:15.591229 fabric_fim-1.5.2/fim/slivers/delegations.py
+-rw-r--r--   0        0        0     3593 2022-02-18 19:27:15.591744 fabric_fim-1.5.2/fim/slivers/gateway.py
+-rw-r--r--   0        0        0      919 2021-06-29 20:04:13.972162 fabric_fim-1.5.2/fim/slivers/identifiers.py
+-rw-r--r--   0        0        0     3444 2022-02-18 19:27:15.592250 fabric_fim-1.5.2/fim/slivers/instance_catalog.py
+-rw-r--r--   0        0        0     3225 2023-02-02 01:41:56.413360 fabric_fim-1.5.2/fim/slivers/interface_info.py
+-rw-r--r--   0        0        0     2702 2021-09-22 14:46:40.423027 fabric_fim-1.5.2/fim/slivers/json.py
+-rw-r--r--   0        0        0     3869 2023-02-02 01:41:56.413720 fabric_fim-1.5.2/fim/slivers/json_data.py
+-rw-r--r--   0        0        0     5983 2023-02-02 01:41:56.414203 fabric_fim-1.5.2/fim/slivers/maintenance_mode.py
+-rw-r--r--   0        0        0     1566 2021-03-03 19:57:54.294274 fabric_fim-1.5.2/fim/slivers/network_attached_storage.py
+-rw-r--r--   0        0        0     3910 2023-02-02 01:41:56.414662 fabric_fim-1.5.2/fim/slivers/network_link.py
+-rw-r--r--   0        0        0    10283 2023-06-16 22:13:30.912936 fabric_fim-1.5.2/fim/slivers/network_node.py
+-rw-r--r--   0        0        0    22052 2023-06-16 22:05:08.616280 fabric_fim-1.5.2/fim/slivers/network_service.py
+-rw-r--r--   0        0        0     6795 2021-06-04 19:43:14.993329 fabric_fim-1.5.2/fim/slivers/path_info.py
+-rw-r--r--   0        0        0     3024 2022-02-18 19:27:15.594931 fabric_fim-1.5.2/fim/slivers/tags.py
+-rw-r--r--   0        0        0     2622 2023-02-02 01:41:56.416090 fabric_fim-1.5.2/fim/slivers/topology_diff.py
+-rw-r--r--   0        0        0     8706 2022-02-18 19:27:15.595505 fabric_fim-1.5.2/fim/user/README.md
+-rw-r--r--   0        0        0     1914 2023-02-02 01:41:56.417286 fabric_fim-1.5.2/fim/user/__init__.py
+-rw-r--r--   0        0        0    11730 2022-09-10 21:18:41.716394 fabric_fim-1.5.2/fim/user/component.py
+-rw-r--r--   0        0        0     5668 2022-09-10 21:18:41.716675 fabric_fim-1.5.2/fim/user/composite_node.py
+-rw-r--r--   0        0        0     7660 2023-02-02 01:41:56.418568 fabric_fim-1.5.2/fim/user/interface.py
+-rw-r--r--   0        0        0     8381 2022-09-10 21:18:41.717280 fabric_fim-1.5.2/fim/user/link.py
+-rw-r--r--   0        0        0     1219 2021-03-03 19:57:54.300001 fabric_fim-1.5.2/fim/user/measurement.py
+-rw-r--r--   0        0        0     9668 2023-04-05 18:48:29.319327 fabric_fim-1.5.2/fim/user/model_element.py
+-rw-r--r--   0        0        0    29219 2023-05-10 14:54:24.206616 fabric_fim-1.5.2/fim/user/network_service.py
+-rw-r--r--   0        0        0    22636 2023-02-14 21:58:39.970039 fabric_fim-1.5.2/fim/user/node.py
+-rw-r--r--   0        0        0    58158 2023-06-01 15:42:31.904936 fabric_fim-1.5.2/fim/user/topology.py
+-rw-r--r--   0        0        0        2 2023-06-15 15:19:24.419545 fabric_fim-1.5.2/fim/util/__init__.py
+-rw-r--r--   0        0        0    14139 2023-06-15 15:20:12.712509 fabric_fim-1.5.2/fim/util/fim_util.py
+-rw-r--r--   0        0        0      595 2021-03-13 20:40:37.643107 fabric_fim-1.5.2/fim/view_only_dict.py
+-rw-r--r--   0        0        0        0 2023-02-02 01:41:56.421372 fabric_fim-1.5.2/neo4j/data/.empty
+-rw-r--r--   0        0        0        0 2023-02-02 01:41:56.421489 fabric_fim-1.5.2/neo4j/imports/.empty
+-rw-r--r--   0        0        0      863 2023-06-15 15:20:12.720926 fabric_fim-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     4632 2022-03-09 00:58:31.583145 fabric_fim-1.5.2/test/ad_topology_test.py
+-rw-r--r--   0        0        0     4834 2022-09-10 21:18:41.719406 fabric_fim-1.5.2/test/after.graphml
+-rw-r--r--   0        0        0    17550 2023-06-15 15:20:12.731835 fabric_fim-1.5.2/test/attribute_collector_test.py
+-rw-r--r--   0        0        0     4696 2022-09-10 21:18:41.719615 fabric_fim-1.5.2/test/before.graphml
+-rw-r--r--   0        0        0     2729 2022-09-10 21:18:41.719876 fabric_fim-1.5.2/test/catalog_test.py
+-rw-r--r--   0        0        0     4319 2022-02-18 19:27:15.602412 fabric_fim-1.5.2/test/delegation_label_test.py
+-rw-r--r--   0        0        0     1653 2023-02-02 01:41:56.423551 fabric_fim-1.5.2/test/maintenance_test.py
+-rw-r--r--   0        0        0    51613 2023-05-10 17:34:04.562843 fabric_fim-1.5.2/test/models/advertised_topo.graphml
+-rw-r--r--   0        0        0    49696 2023-05-10 17:34:04.565992 fabric_fim-1.5.2/test/models/graph-template.graphml
+-rw-r--r--   0        0        0    82994 2023-05-10 17:34:04.568753 fabric_fim-1.5.2/test/models/network-am-ad.graphml
+-rw-r--r--   0        0        0    57411 2023-05-10 17:34:04.571919 fabric_fim-1.5.2/test/models/site-2-am-1broker-ad.graphml
+-rw-r--r--   0        0        0    52887 2023-05-10 17:34:04.574274 fabric_fim-1.5.2/test/models/site-3-am-1broker-ad.graphml
+-rw-r--r--   0        0        0   131407 2023-05-10 17:34:04.575177 fabric_fim-1.5.2/test/models/site-am-2broker-ad.graphml
+-rw-r--r--   0        0        0    18708 2023-06-17 00:08:51.570025 fabric_fim-1.5.2/test/modify_test.py
+-rw-r--r--   0        0        0    13135 2021-05-23 19:50:30.753072 fabric_fim-1.5.2/test/networkxx_pg_disjoint_test.py
+-rw-r--r--   0        0        0    14091 2021-05-23 19:50:30.753595 fabric_fim-1.5.2/test/networkxx_pg_test.py
+-rw-r--r--   0        0        0     2572 2021-03-24 00:18:51.064667 fabric_fim-1.5.2/test/pluggable_test.py
+-rw-r--r--   0        0        0    42428 2023-06-15 15:20:12.777803 fabric_fim-1.5.2/test/slice_topology_test.py
+-rw-r--r--   0        0        0     1869 2022-04-27 22:22:19.322857 fabric_fim-1.5.2/test/sliver_json_test.py
+-rw-r--r--   0        0        0     6030 2023-06-15 15:20:12.763581 fabric_fim-1.5.2/test/sliver_test.py
+-rw-r--r--   0        0        0    97162 2023-02-02 01:41:56.427682 fabric_fim-1.5.2/test/substrate_topology_test.py
+-rw-r--r--   0        0        0      654 2022-02-18 19:27:15.604787 fabric_fim-1.5.2/test/test_load.py
+-rw-r--r--   0        0        0     2362 2022-02-18 19:27:15.605244 fabric_fim-1.5.2/test/tuple_test.py
+-rw-r--r--   0        0        0    15663 2023-06-15 15:19:01.186763 fabric_fim-1.5.2/test/zz_neo4j_pg_test.py
+-rw-r--r--   0        0        0    11890 1970-01-01 00:00:00.000000 fabric_fim-1.5.2/PKG-INFO
```

### Comparing `fabric_fim-1.5.1/.gitignore` & `fabric_fim-1.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/LICENSE` & `fabric_fim-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/README.md` & `fabric_fim-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/figs/fim-structure.png` & `fabric_fim-1.5.2/figs/fim-structure.png`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/README.md` & `fabric_fim-1.5.2/fim/README.md`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/authz/attribute_collector.py` & `fabric_fim-1.5.2/fim/authz/attribute_collector.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/graph/abc_property_graph.py` & `fabric_fim-1.5.2/fim/graph/abc_property_graph.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/graph/abc_property_graph_constants.py` & `fabric_fim-1.5.2/fim/graph/abc_property_graph_constants.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/graph/data/graph_validation_rules.json` & `fabric_fim-1.5.2/fim/graph/data/graph_validation_rules.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/graph/data/graph_validation_rules_neo4j_v4.json` & `fabric_fim-1.5.2/fim/graph/data/graph_validation_rules_neo4j_v4.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/graph/data/label_types.json` & `fabric_fim-1.5.2/fim/graph/data/label_types.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/graph/data/neo4j_indexes.json` & `fabric_fim-1.5.2/fim/graph/data/neo4j_indexes.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/graph/graph_util.py` & `fabric_fim-1.5.2/fim/graph/graph_util.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/graph/neo4j_property_graph.py` & `fabric_fim-1.5.2/fim/graph/neo4j_property_graph.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/graph/networkx_mixin.py` & `fabric_fim-1.5.2/fim/graph/networkx_mixin.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/graph/networkx_property_graph.py` & `fabric_fim-1.5.2/fim/graph/networkx_property_graph.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/graph/networkx_property_graph_disjoint.py` & `fabric_fim-1.5.2/fim/graph/networkx_property_graph_disjoint.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/graph/resources/README.md` & `fabric_fim-1.5.2/fim/graph/resources/README.md`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/graph/resources/abc_adm.py` & `fabric_fim-1.5.2/fim/graph/resources/abc_adm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/graph/resources/abc_arm.py` & `fabric_fim-1.5.2/fim/graph/resources/abc_arm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/graph/resources/abc_bqm.py` & `fabric_fim-1.5.2/fim/graph/resources/abc_bqm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/graph/resources/abc_cbm.py` & `fabric_fim-1.5.2/fim/graph/resources/abc_cbm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/graph/resources/neo4j_adm.py` & `fabric_fim-1.5.2/fim/graph/resources/neo4j_adm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/graph/resources/neo4j_arm.py` & `fabric_fim-1.5.2/fim/graph/resources/neo4j_arm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/graph/resources/neo4j_cbm.py` & `fabric_fim-1.5.2/fim/graph/resources/neo4j_cbm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/graph/resources/networkx_abqm.py` & `fabric_fim-1.5.2/fim/graph/resources/networkx_abqm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/graph/resources/networkx_adm.py` & `fabric_fim-1.5.2/fim/graph/resources/networkx_adm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/graph/resources/networkx_arm.py` & `fabric_fim-1.5.2/fim/graph/resources/networkx_arm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/graph/slices/abc_asm.py` & `fabric_fim-1.5.2/fim/graph/slices/abc_asm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/graph/slices/neo4j_asm.py` & `fabric_fim-1.5.2/fim/graph/slices/neo4j_asm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/graph/slices/networkx_asm.py` & `fabric_fim-1.5.2/fim/graph/slices/networkx_asm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/graph/typed_tuples.py` & `fabric_fim-1.5.2/fim/graph/typed_tuples.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/logging/fim_logger.py` & `fabric_fim-1.5.2/fim/logging/fim_logger.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/logging/log_collector.py` & `fabric_fim-1.5.2/fim/logging/log_collector.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/pluggable.py` & `fabric_fim-1.5.2/fim/pluggable.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/slivers/attached_components.py` & `fabric_fim-1.5.2/fim/slivers/attached_components.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/slivers/base_sliver.py` & `fabric_fim-1.5.2/fim/slivers/base_sliver.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/slivers/capacities_labels.py` & `fabric_fim-1.5.2/fim/slivers/capacities_labels.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/slivers/component_catalog.py` & `fabric_fim-1.5.2/fim/slivers/component_catalog.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/slivers/data/component_catalog.json` & `fabric_fim-1.5.2/fim/slivers/data/component_catalog.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/slivers/data/instance_sizes.json` & `fabric_fim-1.5.2/fim/slivers/data/instance_sizes.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/slivers/delegations.py` & `fabric_fim-1.5.2/fim/slivers/delegations.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/slivers/gateway.py` & `fabric_fim-1.5.2/fim/slivers/gateway.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/slivers/identifiers.py` & `fabric_fim-1.5.2/fim/slivers/identifiers.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/slivers/instance_catalog.py` & `fabric_fim-1.5.2/fim/slivers/instance_catalog.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/slivers/interface_info.py` & `fabric_fim-1.5.2/fim/slivers/interface_info.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/slivers/json.py` & `fabric_fim-1.5.2/fim/slivers/json.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/slivers/json_data.py` & `fabric_fim-1.5.2/fim/slivers/json_data.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/slivers/maintenance_mode.py` & `fabric_fim-1.5.2/fim/slivers/maintenance_mode.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/slivers/network_attached_storage.py` & `fabric_fim-1.5.2/fim/slivers/network_attached_storage.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/slivers/network_link.py` & `fabric_fim-1.5.2/fim/slivers/network_link.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/slivers/network_node.py` & `fabric_fim-1.5.2/fim/slivers/network_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,37 +197,37 @@
         if not self.attached_components_info and other_sliver.attached_components_info:
             comp_added = set(other_sliver.attached_components_info.devices.values())
 
         if self.attached_components_info and not other_sliver.attached_components_info:
             comp_removed = set(self.attached_components_info.devices.values())
 
         if self.network_service_info and other_sliver.network_service_info:
-            diff_ns = self._dict_diff(other_sliver.network_service_info.services,
-                                      other_sliver.network_service_info.services)
+            diff_ns = self._dict_diff(other_sliver.network_service_info.network_services,
+                                      other_sliver.network_service_info.network_services)
             ns_added = set(diff_ns['added'].values())
             ns_removed = set(diff_ns['removed'].values())
             # there are common network services so we check their properties
-            ns_common = self._dict_common(self.network_service_info.services,
-                                          other_sliver.network_service_info.services)
+            ns_common = self._dict_common(self.network_service_info.network_services,
+                                          other_sliver.network_service_info.network_services)
             for nsA in ns_common.values():
                 nsB = other_sliver.network_service_info.get_network_service(nsA.resource_name)
                 # compare properties
                 flag = nsA.prop_diff(nsB)
                 if flag != WhatsModifiedFlag.NONE:
                     ns_modified.append((nsA, flag))
 
         if not self.network_service_info and other_sliver.network_service_info:
-            ns_added = set(other_sliver.network_service_info.services.values())
+            ns_added = set(other_sliver.network_service_info.network_services.values())
 
         if self.network_service_info and not other_sliver.network_service_info:
-            ns_removed = set(self.network_service_info.services.values())
+            ns_removed = set(self.network_service_info.network_services.values())
 
         if len(comp_added) > 0 or len(comp_removed) > 0 or \
                 len(ns_removed) > 0 or len(ns_added) > 0 or \
-                len(comp_modified) > 0 or len(ns_modified) > 0:
+                len(comp_modified) > 0 or len(ns_modified) > 0 or len(self_modified) > 0:
             return TopologyDiff(added=TopologyDiffTuple(components=comp_added, services=ns_added, interfaces=set(),
                                                         nodes=set()),
                                 removed=TopologyDiffTuple(components=comp_removed, services=ns_removed,
                                                           interfaces=set(), nodes=set()),
                                 modified=TopologyDiffModifiedTuple(
                                     nodes=self_modified,
                                     components=comp_modified,
```

### Comparing `fabric_fim-1.5.1/fim/slivers/network_service.py` & `fabric_fim-1.5.2/fim/slivers/network_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -389,15 +389,15 @@
 
         if not self.interface_info and other_sliver.interface_info:
             ifs_added = set(other_sliver.interface_info.interfaces.values())
 
         if self.interface_info and not other_sliver.interface_info:
             ifs_removed = set(self.interface_info.interfaces.values())
 
-        if len(ifs_added) > 0 or len(ifs_removed) > 0 or len(ifs_modified) > 0:
+        if len(self_modified) > 0 or len(ifs_added) > 0 or len(ifs_removed) > 0 or len(ifs_modified) > 0:
             return TopologyDiff(added=TopologyDiffTuple(components=set(), services=set(), interfaces=ifs_added,
                                                         nodes=set()),
                                 removed=TopologyDiffTuple(components=set(), services=set(),
                                                           interfaces=ifs_removed, nodes=set()),
                                 modified=TopologyDiffModifiedTuple(
                                     nodes=list(),
                                     components=list(),
```

### Comparing `fabric_fim-1.5.1/fim/slivers/path_info.py` & `fabric_fim-1.5.2/fim/slivers/path_info.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/slivers/tags.py` & `fabric_fim-1.5.2/fim/slivers/tags.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/slivers/topology_diff.py` & `fabric_fim-1.5.2/fim/slivers/topology_diff.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/user/README.md` & `fabric_fim-1.5.2/fim/user/README.md`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/user/__init__.py` & `fabric_fim-1.5.2/fim/user/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/user/component.py` & `fabric_fim-1.5.2/fim/user/component.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/user/composite_node.py` & `fabric_fim-1.5.2/fim/user/composite_node.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/user/interface.py` & `fabric_fim-1.5.2/fim/user/interface.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/user/link.py` & `fabric_fim-1.5.2/fim/user/link.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/user/measurement.py` & `fabric_fim-1.5.2/fim/user/measurement.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/user/model_element.py` & `fabric_fim-1.5.2/fim/user/model_element.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/user/network_service.py` & `fabric_fim-1.5.2/fim/user/network_service.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/user/node.py` & `fabric_fim-1.5.2/fim/user/node.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/user/topology.py` & `fabric_fim-1.5.2/fim/user/topology.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/util/fim_util.py` & `fabric_fim-1.5.2/fim/util/fim_util.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/fim/view_only_dict.py` & `fabric_fim-1.5.2/fim/view_only_dict.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/pyproject.toml` & `fabric_fim-1.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/test/ad_topology_test.py` & `fabric_fim-1.5.2/test/ad_topology_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/test/after.graphml` & `fabric_fim-1.5.2/test/after.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/test/attribute_collector_test.py` & `fabric_fim-1.5.2/test/attribute_collector_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/test/before.graphml` & `fabric_fim-1.5.2/test/before.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/test/catalog_test.py` & `fabric_fim-1.5.2/test/catalog_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/test/delegation_label_test.py` & `fabric_fim-1.5.2/test/delegation_label_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/test/maintenance_test.py` & `fabric_fim-1.5.2/test/maintenance_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/test/models/advertised_topo.graphml` & `fabric_fim-1.5.2/test/models/advertised_topo.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/test/models/graph-template.graphml` & `fabric_fim-1.5.2/test/models/graph-template.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/test/models/network-am-ad.graphml` & `fabric_fim-1.5.2/test/models/network-am-ad.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/test/models/site-2-am-1broker-ad.graphml` & `fabric_fim-1.5.2/test/models/site-2-am-1broker-ad.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/test/models/site-3-am-1broker-ad.graphml` & `fabric_fim-1.5.2/test/models/site-3-am-1broker-ad.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/test/models/site-am-2broker-ad.graphml` & `fabric_fim-1.5.2/test/models/site-am-2broker-ad.graphml`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/test/modify_test.py` & `fabric_fim-1.5.2/test/modify_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,14 +276,36 @@
         ModifyTest.compare_diffs(diff_res, self.diff)
 
         #print(f'Result {diff_res=}')
         #print(f'\nExpected {self.diff}')
         #print(f'\nStarting Topo {self.topoA}')
         #print(f'\nFinal Topo {self.topoB}')
 
+    def testSimpleSliverDiff(self):
+        print('*** Simple Sliver diff test')
+        # just test to network services different in labels
+        tA = f.ExperimentTopology()
+        na = tA.add_node(name='nodeA', site='UKY')
+        ca = na.add_component(name='nic3', ctype=ComponentType.SharedNIC, model='ConnectX-6')
+        ns = na.add_network_service(name='ne1', nstype=ServiceType.FABNetv4, interfaces=na.interface_list,
+                                    labels=Labels(ipv4='192.168.1.1'))
+        nsS1 = tA.graph_model.build_deep_ns_sliver(node_id=ns.node_id)
+        nS1 = tA.graph_model.build_deep_node_sliver(node_id=na.node_id)
+        ns.labels = Labels(ipv4='192.168.1.2')
+        ns.capacities = Capacities(bw=100)
+        na.labels = Labels(ipv4='10.100.1.1')
+        nsS2 = tA.graph_model.build_deep_ns_sliver(node_id=ns.node_id)
+        nS2 = tA.graph_model.build_deep_node_sliver(node_id=na.node_id)
+        ns_diff = nsS1.diff(nsS2)
+        node_diff = nS1.diff(nS2)
+        self.assertEqual(ns_diff.modified.services[0][1], WhatsModifiedFlag.LABELS | WhatsModifiedFlag.CAPACITIES)
+        self.assertEqual(node_diff.modified.services[0][1], WhatsModifiedFlag.LABELS | WhatsModifiedFlag.CAPACITIES)
+        self.assertEqual(node_diff.modified.nodes[0][1], WhatsModifiedFlag.LABELS)
+        print(f' ****** {node_diff=}')
+
     def testSliverDiffs(self):
 
         print('*** Sliver diff test')
         self.modifyActions()
 
         nAA = self.topoA.nodes['NodeA']
         print(f'{nAA.components=}')
```

### Comparing `fabric_fim-1.5.1/test/networkxx_pg_disjoint_test.py` & `fabric_fim-1.5.2/test/networkxx_pg_disjoint_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/test/networkxx_pg_test.py` & `fabric_fim-1.5.2/test/networkxx_pg_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/test/pluggable_test.py` & `fabric_fim-1.5.2/test/pluggable_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/test/slice_topology_test.py` & `fabric_fim-1.5.2/test/slice_topology_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/test/sliver_json_test.py` & `fabric_fim-1.5.2/test/sliver_json_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/test/sliver_test.py` & `fabric_fim-1.5.2/test/sliver_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/test/substrate_topology_test.py` & `fabric_fim-1.5.2/test/substrate_topology_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/test/test_load.py` & `fabric_fim-1.5.2/test/test_load.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/test/tuple_test.py` & `fabric_fim-1.5.2/test/tuple_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/test/zz_neo4j_pg_test.py` & `fabric_fim-1.5.2/test/zz_neo4j_pg_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.5.1/PKG-INFO` & `fabric_fim-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric_fim
-Version: 1.5.1
+Version: 1.5.2
 Summary: FABRIC Information Model library and utilities
 Keywords: Neo4j
 Author-email: Ilya Baldin <ibaldin@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

